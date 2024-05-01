# Comparing `tmp/lifeomic_patient_ml_types-9.1.0.tar.gz` & `tmp/lifeomic_patient_ml_types-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeomic_patient_ml_types-9.1.0.tar", max compression
+gzip compressed data, was "lifeomic_patient_ml_types-9.2.0.tar", max compression
```

## Comparing `lifeomic_patient_ml_types-9.1.0.tar` & `lifeomic_patient_ml_types-9.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    16910 2024-04-30 18:15:45.387156 lifeomic_patient_ml_types-9.1.0/lifeomic_patient_ml_types/schemas.py
--rw-r--r--   0        0        0      970 2024-04-30 18:17:02.335293 lifeomic_patient_ml_types-9.1.0/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-9.1.0/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-9.1.0/PKG-INFO
+-rw-r--r--   0        0        0    18210 2024-05-01 13:22:37.945237 lifeomic_patient_ml_types-9.2.0/lifeomic_patient_ml_types/schemas.py
+-rw-r--r--   0        0        0      970 2024-05-01 13:23:48.877090 lifeomic_patient_ml_types-9.2.0/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-9.2.0/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-9.2.0/PKG-INFO
```

### Comparing `lifeomic_patient_ml_types-9.1.0/lifeomic_patient_ml_types/schemas.py` & `lifeomic_patient_ml_types-9.2.0/lifeomic_patient_ml_types/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 class MlProblemDefinitionBase(BaseModel):
     class Config:
         extra = Extra.allow
 
     retrainEvery: Optional[float] = None
     """
     If provided, the model will automatically be retrained if this many milliseconds have passed since the last run. Models will not be retrained more frequently than once per day, and this policy is only checked once per day, so more than this many milliseconds may actually pass before the model is retrained.
+    @deprecated use `ModelConfig.trainingApproach.retrainEvery` instead.
     """
 
 
 class LabelDefinitionBase(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -315,14 +316,18 @@
     """
     The hyperparameter search space to explore during hyperparameter tuning.
     """
     maxTrials: Optional[int] = Field(None, ge=1, le=30)
     """
     The maximum number of candidate models to consider in a given model run.
     """
+    retrainEvery: Optional[float] = None
+    """
+    If provided, the model will automatically be retrained if this many milliseconds have passed since the last run. Models will not be retrained more frequently than once per day, and this policy is only checked once per day, so more than this many milliseconds may actually pass before the model is retrained.
+    """
 
 
 class TrainingApproach(BaseModel):
     __root__: TuningJobTrainingApproach
 
 
 class DeployApproachBase(BaseModel):
@@ -346,22 +351,34 @@
     type: Literal["cloud"]
 
 
 class DeployApproach(BaseModel):
     __root__: Union[EdgeDeployApproach, CloudDeployApproach]
 
 
+class DatasetConfigBase(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    name: str
+    description: str
+
+
 class ModelConfigBase(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: str
     description: str
     trainingApproach: TrainingApproach
     deployApproach: DeployApproach
+    datasetId: Optional[str] = None
+    """
+    The ID of the configuration that defines the dataset this model will be trained on.
+    """
 
 
 class Metric(BaseModel):
     class Config:
         extra = Extra.forbid
 
     name: str
@@ -581,25 +598,44 @@
     __root__: Union[ImageSegmentationProblemInput, ImageClassificationProblemInput]
 
 
 class MlProblemDefinition(BaseModel):
     __root__: Union[ImageSegmentationProblem, ImageClassificationProblem]
 
 
+class DatasetConfigInput(DatasetConfigBase):
+    problemDefinition: MlProblemDefinitionInput
+
+
+class DatasetConfig(DatasetConfigBase):
+    id: str
+    """
+    UUID uniquely identifying this dataset config.
+    """
+    accountId: str
+    problemDefinition: MlProblemDefinition
+
+
 class ModelConfigInput(ModelConfigBase):
     problemDefinition: MlProblemDefinitionInput
+    """
+    @deprecated Define a problem definition in a separate `DatasetConfig` and associate it with the model config using `ModelConfig.datasetId`.
+    """
 
 
 class ModelConfig(ModelConfigBase):
     id: str
     """
     UUID uniquely identifying this model config.
     """
     accountId: str
     problemDefinition: MlProblemDefinition
+    """
+    @deprecated Define a problem definition in a separate `DatasetConfig` and associate it with the model config using `ModelConfig.datasetId`.
+    """
     deployedId: Optional[str] = None
     """
     The ID of the model version currently deployed for this model config.
     @deprecated use championId instead
     """
     championId: Optional[str] = None
     """
```

### Comparing `lifeomic_patient_ml_types-9.1.0/pyproject.toml` & `lifeomic_patient_ml_types-9.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lifeomic-patient-ml-types"
-version = "9.1.0"
+version = "9.2.0"
 description = "Shared types for the patient-ml-service repos."
 authors = ["LifeOmic <development@lifeomic.com>"]
 license = "UNLICENSED"
 
 [tool.poe.tasks]
 format = "black lifeomic_patient_ml_types"
 lint = "pyright lifeomic_patient_ml_types"
```

