# Comparing `tmp/mphapi-0.3.0.tar.gz` & `tmp/mphapi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mphapi-0.3.0.tar", max compression
+gzip compressed data, was "mphapi-0.4.0.tar", max compression
```

## Comparing `mphapi-0.3.0.tar` & `mphapi-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      210 2024-04-10 01:49:16.715908 mphapi-0.3.0/mphapi/__init__.py
--rw-r--r--   0        0        0    10567 2024-04-18 05:33:37.948236 mphapi-0.3.0/mphapi/claim.py
--rw-r--r--   0        0        0     6297 2024-04-10 01:49:16.715908 mphapi-0.3.0/mphapi/client.py
--rw-r--r--   0        0        0     1504 2024-04-10 01:49:16.715908 mphapi-0.3.0/mphapi/date.py
--rw-r--r--   0        0        0     9773 2024-04-18 21:05:52.023884 mphapi-0.3.0/mphapi/pricing.py
--rw-r--r--   0        0        0     2958 2024-04-10 01:49:16.715908 mphapi-0.3.0/mphapi/response.py
--rw-r--r--   0        0        0      342 2024-04-18 21:06:44.638423 mphapi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 mphapi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      210 2024-04-10 01:49:16.715908 mphapi-0.4.0/mphapi/__init__.py
+-rw-r--r--   0        0        0    11518 2024-05-01 02:21:58.782494 mphapi-0.4.0/mphapi/claim.py
+-rw-r--r--   0        0        0     6297 2024-04-10 01:49:16.715908 mphapi-0.4.0/mphapi/client.py
+-rw-r--r--   0        0        0     1504 2024-04-10 01:49:16.715908 mphapi-0.4.0/mphapi/date.py
+-rw-r--r--   0        0        0      604 2024-05-01 02:21:58.782494 mphapi-0.4.0/mphapi/fields.py
+-rw-r--r--   0        0        0    10159 2024-05-01 02:21:58.782494 mphapi-0.4.0/mphapi/pricing.py
+-rw-r--r--   0        0        0     2958 2024-04-10 01:49:16.715908 mphapi-0.4.0/mphapi/response.py
+-rw-r--r--   0        0        0      342 2024-05-01 02:21:58.782494 mphapi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 mphapi-0.4.0/PKG-INFO
```

### Comparing `mphapi-0.3.0/mphapi/claim.py` & `mphapi-0.4.0/mphapi/claim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,68 @@
 from enum import Enum, IntEnum
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import AliasGenerator, BaseModel, ConfigDict, Field
-from pydantic.alias_generators import to_camel
+from pydantic import BaseModel, Field
 
 from .date import Date
-
-camel_case_model_config = ConfigDict(
-    alias_generator=AliasGenerator(
-        validation_alias=to_camel, serialization_alias=to_camel
-    ),
-    populate_by_name=True,
-)
+from .fields import camel_case_model_config, field_name
 
 
 class FormType(str, Enum):
     """Type of form used to submit the claim. Can be HCFA or UB-04 (from CLM05_02)"""
 
-    HCFA = "HCFA"
     UB_04 = "UB-04"
+    HCFA = "HCFA"
 
 
 class BillTypeSequence(str, Enum):
     """Where the claim is at in its billing lifecycle (e.g. 0: Non-Pay, 1: Admit Through
     Discharge, 7: Replacement, etc.) (from CLM05_03)
     """
 
-    NON_PAY = "G"
-    ADMIT_THROUGH_DISCHARGE = "H"
-    FIRST_INTERIM = "I"
-    CONTINUING_INTERIM = "J"
-    LAST_INTERIM = "K"
-    LATE_CHARGE = "M"
-    FIRST_INTERIM_DEPRECATED = "P"
-    REPLACEMENT = "Q"
-    VOID_OR_CANCEL = "0"
-    FINAL_CLAIM = "1"
-    CWF_ADJUSTMENT = "2"
-    CMS_ADJUSTMENT = "3"
-    INTERMEDIARY_ADJUSTMENT = "4"
-    OTHER_ADJUSTMENT = "5"
-    OIG_ADJUSTMENT = "6"
-    MSP_ADJUSTMENT = "7"
-    QIO_ADJUSTMENT = "8"
-    PROVIDER_ADJUSTMENT = "9"
+    NON_PAY = "0"
+    ADMIT_THROUGH_DISCHARGE = "1"
+    FIRST_INTERIM = "2"
+    CONTINUING_INTERIM = "3"
+    LAST_INTERIM = "4"
+    LATE_CHARGE = "5"
+    FIRST_INTERIM_DEPRECATED = "6"
+    REPLACEMENT = "7"
+    VOID_OR_CANCEL = "8"
+    FINAL_CLAIM = "9"
+    CWF_ADJUSTMENT = "G"
+    CMS_ADJUSTMENT = "H"
+    INTERMEDIARY_ADJUSTMENT = "I"
+    OTHER_ADJUSTMENT = "J"
+    OIG_ADJUSTMENT = "K"
+    MSP_ADJUSTMENT = "M"
+    QIO_ADJUSTMENT = "P"
+    PROVIDER_ADJUSTMENT = "Q"
 
 
 class SexType(IntEnum):
     """Biological sex of the patient for clinical purposes"""
 
     UNKNOWN = 0
     MALE = 1
     FEMALE = 2
 
 
 class Provider(BaseModel):
+    """
+    Provider represents the service provider that rendered healthcare services on behalf of the patient.
+    This can be found in Loop 2000A and/or Loop 2310 NM101-77 at the claim level, and may also be overridden at the service level in the 2400 loop
+    """
+
     model_config = camel_case_model_config
 
     npi: str
     """National Provider Identifier of the provider (from NM109, required)"""
 
-    provider_tax_id: Optional[str] = None
+    provider_tax_id: Annotated[Optional[str], field_name("providerTaxID")] = None
     """City of the provider (from N401, highly recommended)"""
 
     provider_phones: Optional[list[str]] = None
     """Address line 1 of the provider (from N301, highly recommended)"""
 
     provider_faxes: Optional[list[str]] = None
     """Commercial number of the provider used by some payers (from REF G2, optional)"""
@@ -98,39 +96,38 @@
 
     provider_city: Optional[str] = None
     """Fax numbers of the provider (from PER, optional)"""
 
     provider_state: Optional[str] = None
     """Address line 2 of the provider (from N302, optional)"""
 
-    provider_zip: str
+    provider_zip: Annotated[str, field_name("providerZIP")]
     """ZIP code of the provider (from N403, required)"""
 
 
 class ValueCode(BaseModel):
-    """Code indicating the type of value provided (from HIxx_02)"""
-
     model_config = camel_case_model_config
 
     code: str
+    """Code indicating the type of value provided (from HIxx_02)"""
 
-    """Amount associated with the value code (from HIxx_05)"""
     amount: float
+    """Amount associated with the value code (from HIxx_05)"""
 
 
 class Diagnosis(BaseModel):
-    """Principal ICD diagnosis for the patient (from HI ABK or BK)"""
+    """Principal, Other Diagnosis, Admitting Diagnosis, External Cause of Injury"""
 
     model_config = camel_case_model_config
 
     code: str
-    """ICD code for the diagnosis"""
+    """ICD-10 diagnosis code (from HIxx_02)"""
 
     description: Optional[str] = None
-    """Description of the diagnosis"""
+    """Flag indicates whether diagnosis was present at the time of admission (from HIxx_09)"""
 
 
 class Service(BaseModel):
     model_config = camel_case_model_config
 
     provider: Optional[Provider] = None
     """Additional provider information specific to this service item"""
@@ -140,14 +137,16 @@
 
     rev_code: Optional[str] = None
     """Revenue code (from SV2_01)"""
 
     procedure_code: Optional[str] = None
     """Procedure code (from SV101_02 / SV202_02)"""
 
+    hipps_code: Optional[str] = None
+
     procedure_modifiers: Optional[list[str]] = None
     """Procedure modifiers (from SV101_03, 4, 5, 6 / SV202_03, 4, 5, 6)"""
 
     drug_code: Optional[str] = None
     """National Drug Code (from LIN03)"""
 
     date_from: Optional[Date] = None
@@ -173,56 +172,62 @@
 
     place_of_service: Optional[str] = None
     """Place of service code (from SV105)"""
 
     diagnosis_pointers: Optional[list[int]] = None
     """Diagnosis pointers (from SV107)"""
 
-    ambulance_pickup_zip: Optional[str] = None
+    ambulance_pickup_zip: Annotated[Optional[str], field_name("ambulancePickupZIP")] = (
+        None
+    )
     """ZIP code where ambulance picked up patient. Supplied if different than claim-level value (from NM1 PW)"""
 
 
 class Claim(Provider, BaseModel):
     model_config = camel_case_model_config
 
-    claim_id: Optional[str] = None
+    claim_id: Annotated[Optional[str], field_name("claimID")] = None
     """Unique identifier for the claim (from REF D9)"""
 
     plan_code: Optional[str] = None
     """Identifies the subscriber's plan (from SBR03)"""
 
     patient_sex: Optional[SexType] = None
     """Biological sex of the patient for clinical purposes (from DMG02). 0:Unknown, 1:Male,
     2:Female
     """
 
     patient_date_of_birth: Optional[Date] = None
     """Patient date of birth (from DMG03)"""
 
-    patient_height_in_cm: Optional[float] = None
+    patient_height_in_cm: Annotated[
+        Optional[float], field_name("patientHeightInCM")
+    ] = None
     """Patient height in centimeters (from HI value A9, MEA value HT)"""
 
-    patient_weight_in_kg: Optional[float] = None
+    patient_weight_in_kg: Annotated[
+        Optional[float], field_name("patientWeightInKG")
+    ] = None
     """Patient weight in kilograms (from HI value A8, PAT08, CR102 [ambulance only])"""
 
-    ambulance_pickup_zip: Optional[str] = None
+    ambulance_pickup_zip: Annotated[Optional[str], field_name("ambulancePickupZIP")] = (
+        None
+    )
     """Location where patient was picked up in ambulance (from HI with HIxx_01=BE and HIxx_02=A0
     or NM1 loop with NM1 PW)
     """
 
     form_type: Optional[FormType] = None
     """Type of form used to submit the claim. Can be HCFA or UB-04 (from CLM05_02)"""
 
-    bill_type_or_pos: Optional[str] = None
+    bill_type_or_pos: Annotated[Optional[str], field_name("billTypeOrPOS")] = None
     """Describes type of facility where services were rendered (from CLM05_01)"""
 
     bill_type_sequence: Optional[BillTypeSequence] = None
-    """Where the claim is at in its billing lifecycle (e.g. 0: Non-Pay, 1: Admit Through
-    Discharge, 7: Replacement, etc.) (from CLM05_03)
-    """
+    """Where the claim is at in its billing lifecycle (e.g. 0: Non-Pay, 1: Admit Through Discharge, 7: Replacement, etc.) (from CLM05_03)"""
 
     billed_amount: Optional[float] = None
     """Billed amount from provider (from CLM02)"""
 
     allowed_amount: Optional[float] = None
     """Amount allowed by the plan for payment. Both member and plan responsibility (non-EDI)"""
 
@@ -268,65 +273,65 @@
     services: list[Service] = Field(min_length=1)
     """One or more services provided to the patient (from LX loop)"""
 
 
 class RateSheetService(BaseModel):
     model_config = camel_case_model_config
 
-    procedure_code: str
+    procedure_code: Optional[str] = None
     """Procedure code (from SV101_02 / SV202_02)"""
 
-    procedure_modifiers: list[str]
+    procedure_modifiers: Optional[list[str]] = None
     """Procedure modifiers (from SV101_03, 4, 5, 6 / SV202_03, 4, 5, 6)"""
 
-    billed_amount: float
+    billed_amount: Optional[float] = None
     """Billed charge for the service (from SV102 / SV203)"""
 
-    allowed_amount: float
+    allowed_amount: Optional[float] = None
     """Plan allowed amount for the service (non-EDI)"""
 
 
 class RateSheet(BaseModel):
     npi: str
     """National Provider Identifier of the provider (from NM109, required)"""
 
-    provider_first_name: str
+    provider_first_name: Optional[str] = None
     """First name of the provider (NM104, highly recommended)"""
 
-    provider_last_name: str
+    provider_last_name: Optional[str] = None
     """Last name of the provider (from NM103, highly recommended)"""
 
-    provider_org_name: str
+    provider_org_name: Optional[str] = None
     """Organization name of the provider (from NM103, highly recommended)"""
 
-    provider_address: str
+    provider_address: Optional[str] = None
     """Address of the provider (from N301, highly recommended)"""
 
-    provider_city: str
+    provider_city: Optional[str] = None
     """City of the provider (from N401, highly recommended)"""
 
-    provider_state: str
+    provider_state: Optional[str] = None
     """State of the provider (from N402, highly recommended)"""
 
-    provider_zip: str
+    provider_zip: Annotated[str, field_name("providerZIP")]
     """ZIP code of the provider (from N403, required)"""
 
-    form_type: FormType
+    form_type: Optional[FormType] = None
     """Type of form used to submit the claim. Can be HCFA or UB-04 (from CLM05_02)"""
 
-    bill_type_or_pos: str
+    bill_type_or_pos: Annotated[Optional[str], field_name("billTypeOrPOS")] = None
     """Describes type of facility where services were rendered (from CLM05_01)"""
 
-    drg: str
+    drg: Optional[str] = None
     """Diagnosis Related Group for inpatient services (from HI DR)"""
 
-    billed_amount: float
+    billed_amount: Optional[float] = None
     """Billed amount from provider (from CLM02)"""
 
-    allowed_amount: float
+    allowed_amount: Optional[float] = None
     """Amount allowed by the plan for payment. Both member and plan responsibility (non-EDI)"""
 
-    paid_amount: float
+    paid_amount: Optional[float] = None
     """Amount paid by the plan for the claim (non-EDI)"""
 
-    services: list[RateSheetService]
+    services: Optional[list[RateSheetService]] = None
     """One or more services provided to the patient (from LX loop)"""
```

### Comparing `mphapi-0.3.0/mphapi/client.py` & `mphapi-0.4.0/mphapi/client.py`

 * *Files identical despite different names*

### Comparing `mphapi-0.3.0/mphapi/date.py` & `mphapi-0.4.0/mphapi/date.py`

 * *Files identical despite different names*

### Comparing `mphapi-0.3.0/mphapi/pricing.py` & `mphapi-0.4.0/mphapi/pricing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
-from typing import Optional
+from typing import Annotated, Optional
 
 from pydantic import BaseModel, Field
 
-from .claim import camel_case_model_config
+from .fields import camel_case_model_config, field_name
 from .response import ResponseError
 
 
 class ClaimRepricingCode(str, Enum):
     """claim-level repricing codes"""
 
     MEDICARE = "MED"
@@ -16,40 +16,46 @@
     SINGLE_CASE_AGREEMENT = "SCA"
     NEEDS_MORE_INFO = "IFO"
 
 
 class LineRepricingCode(str, Enum):
     # line-level Medicare repricing codes
     MEDICARE = "MED"
-    SYNTHETIC_MEDICARE = "SYN"
-    COST_PERCENT = "CST"
     MEDICARE_PERCENT = "MPT"
     MEDICARE_NO_OUTLIER = "MNO"
+    SYNTHETIC_MEDICARE = "SYN"
     BILLED_PERCENT = "BIL"
     FEE_SCHEDULE = "FSC"
     PER_DIEM = "PDM"
     FLAT_RATE = "FLT"
+    COST_PERCENT = "CST"
     LIMITED_TO_BILLED = "LTB"
 
     # line-level zero dollar repricing explanations
+    NOT_REPRICED_PER_REQUEST = "NRP"
     NOT_ALLOWED_BY_MEDICARE = "NAM"
     PACKAGED = "PKG"
     NEEDS_MORE_INFO = "IFO"
     PROCEDURE_CODE_PROBLEM = "CPB"
-    NOT_REPRICED_PER_REQUEST = "NRP"
 
 
 class HospitalType(str, Enum):
     ACUTE_CARE = "Acute Care Hospitals"
     CRITICAL_ACCESS = "Critical Access Hospitals"
     CHILDRENS = "Childrens"
     PSYCHIATRIC = "Psychiatric"
     ACUTE_CARE_DOD = "Acute Care - Department of Defense"
 
 
+class RuralIndicator(str, Enum):
+    RURAL = "R"
+    SUPER_RURAL = "B"
+    URBAN = ""
+
+
 class InpatientPriceDetail(BaseModel):
     """InpatientPriceDetail contains pricing details for an inpatient claim"""
 
     model_config = camel_case_model_config
 
     drg: Optional[str] = None
     """Diagnosis Related Group (DRG) code used to price the claim"""
@@ -105,20 +111,14 @@
     full_or_partial_device_credit_offset_amount: float
     """Credit for devices that are supplied for free or at a reduced cost"""
 
     terminated_device_procedure_offset_amount: float
     """Credit for devices that are not used due to a terminated procedure"""
 
 
-class RuralIndicator(str, Enum):
-    RURAL = "R"
-    SUPER_RURAL = "B"
-    URBAN = ""
-
-
 class ProviderDetail(BaseModel):
     """
     ProviderDetail contains basic information about the provider and/or locality used for pricing.
     Not all fields are returned with every pricing request. For example, the CMS Certification
     Number (CCN) is only returned for facilities which have a CCN such as hospitals.
     """
 
@@ -181,80 +181,80 @@
 
 
 class PricedService(BaseModel):
     """PricedService contains the results of a pricing request for a single service line"""
 
     model_config = camel_case_model_config
 
-    line_number: str
+    line_number: Optional[str] = None
     """Number of the service line item (copied from input)"""
 
     provider_detail: Optional[ProviderDetail] = None
     """Provider Details used when pricing the service if different than the claim"""
 
-    medicare_amount: float
+    medicare_amount: Optional[float] = None
     """Amount Medicare would pay for the service"""
 
-    allowed_amount: float
+    allowed_amount: Optional[float] = None
     """Allowed amount based on a contract or RBP pricing"""
 
-    allowed_calculation_error: str
-    """Reason the allowed amount was not calculated"""
-
-    repricing_code: LineRepricingCode
+    medicare_repricing_code: Optional[LineRepricingCode] = None
     """Explains the methodology used to calculate Medicare"""
 
-    repricing_note: str
+    medicare_repricing_note: Optional[str] = None
+    """Note explaining approach for pricing or reason for error"""
+
+    allowed_repricing_code: Optional[LineRepricingCode] = None
+    """Explains the methodology used to calculate allowed amount"""
+
+    allowed_repricing_note: Optional[str] = None
     """Note explaining approach for pricing or reason for error"""
 
-    technical_component_amount: float
+    technical_component_amount: Optional[float] = None
     """Amount Medicare would pay for the technical component"""
 
-    professional_component_amount: float
+    professional_component_amount: Optional[float] = None
     """Amount Medicare would pay for the professional component"""
 
-    medicare_std_dev: float
+    medicare_std_dev: Optional[float] = None
     """Standard deviation of the estimated Medicare amount (estimates service only)"""
 
-    medicare_source: str
+    medicare_source: Optional[str] = None
     """Source of the Medicare amount (e.g. physician fee schedule, OPPS, etc.)"""
 
-    pricer_result: str
+    pricer_result: Optional[str] = None
     """Pricing service return details"""
 
-    status_indicator: str
+    status_indicator: Optional[str] = None
     """Code which gives more detail about how Medicare pays for the service"""
 
-    payment_indicator: str
+    payment_indicator: Optional[str] = None
     """Text which explains the type of payment for Medicare"""
 
-    payment_apc: str
+    payment_apc: Annotated[Optional[str], field_name("paymentAPC")] = None
     """Ambulatory Payment Classification"""
 
     edit_detail: Optional[LineEdits] = None
     """Errors which cause the line item to be unable to be priced"""
 
 
 class Pricing(BaseModel):
     """Pricing contains the results of a pricing request"""
 
     model_config = camel_case_model_config
 
-    claim_id: Optional[str] = None
+    claim_id: Annotated[Optional[str], field_name(alias="claimID")] = None
     """The unique identifier for the claim (copied from input)"""
 
     medicare_amount: Optional[float] = None
     """The amount Medicare would pay for the service"""
 
     allowed_amount: Optional[float] = None
     """The allowed amount based on a contract or RBP pricing"""
 
-    allowed_calculation_error: Optional[str] = None
-    """The reason the allowed amount was not calculated"""
-
     medicare_repricing_code: Optional[ClaimRepricingCode] = None
     """Explains the methodology used to calculate Medicare (MED or IFO)"""
 
     medicare_repricing_note: Optional[str] = None
     """Note explaining approach for pricing or reason for error"""
 
     allowed_repricing_code: Optional[ClaimRepricingCode] = None
```

### Comparing `mphapi-0.3.0/mphapi/response.py` & `mphapi-0.4.0/mphapi/response.py`

 * *Files identical despite different names*

