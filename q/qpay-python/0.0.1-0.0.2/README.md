# Comparing `tmp/qpay_python-0.0.1.tar.gz` & `tmp/qpay_python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qpay_python-0.0.1.tar", max compression
+gzip compressed data, was "qpay_python-0.0.2.tar", max compression
```

## Comparing `qpay_python-0.0.1.tar` & `qpay_python-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2801 2024-04-20 18:26:31.214979 qpay_python-0.0.1/README.md
--rw-r--r--   0        0        0     1490 2024-04-20 18:26:37.019010 qpay_python-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      107 2024-04-20 18:26:31.214979 qpay_python-0.0.1/qpay/__init__.py
--rw-r--r--   0        0        0     2954 2024-04-20 18:26:31.214979 qpay_python-0.0.1/qpay/auth.py
--rw-r--r--   0        0        0      496 2024-04-20 18:26:31.214979 qpay_python-0.0.1/qpay/exceptions.py
--rw-r--r--   0        0        0     5447 2024-04-20 18:26:31.214979 qpay_python-0.0.1/qpay/main.py
--rw-r--r--   0        0        0      371 2024-04-20 18:26:31.214979 qpay_python-0.0.1/qpay/singleton.py
--rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 qpay_python-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2802 2024-05-01 00:42:38.810092 qpay_python-0.0.2/README.md
+-rw-r--r--   0        0        0     1490 2024-05-01 00:42:54.466278 qpay_python-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-05-01 00:42:38.814092 qpay_python-0.0.2/qpay/__init__.py
+-rw-r--r--   0        0        0     2954 2024-05-01 00:42:38.814092 qpay_python-0.0.2/qpay/auth.py
+-rw-r--r--   0        0        0      496 2024-05-01 00:42:38.814092 qpay_python-0.0.2/qpay/exceptions.py
+-rw-r--r--   0        0        0     4552 2024-05-01 00:42:38.814092 qpay_python-0.0.2/qpay/main.py
+-rw-r--r--   0        0        0      371 2024-05-01 00:42:38.814092 qpay_python-0.0.2/qpay/singleton.py
+-rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 qpay_python-0.0.2/PKG-INFO
```

### Comparing `qpay_python-0.0.1/README.md` & `qpay_python-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align="center">
-  QPayClient
+  QPay Python
 </h1>
 
 <p align="center">
   <a href="https://github.com/khasbilegt/qpay-python/">
     <img src="https://img.shields.io/github/actions/workflow/status/khasbilegt/qpay-python/qa.yml?label=CI&logo=github&style=for-the-badge" alt="ci status">
   </a>
   <a href="https://codecov.io/github/khasbilegt/qpay-python">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-                           ************ QQPPaayyCClliieenntt ************
+                           ************ QQPPaayy PPyytthhoonn ************
                              _[_c_i_ _s_t_a_t_u_s_]_[_c_o_d_e_c_o_v_]
                     _[_p_y_p_i_ _l_i_n_k_][supported python versions]
  _Ð__Ñ__Ð_¸_Ð_³_Ð_»_Ð_°_Ñ_ â¢ _Ð_¥_Ó_©_Ð_³_Ð_¶_Ò_¯_Ò_¯_Ð_»_Ñ__Ð_»_Ñ__Ñ__Ð_½_Ð_´_ _Ð_¾_Ñ__Ð_¾_Ð_»_Ñ__Ð_¾_Ñ_ â¢ _Ð__Ð_¸_Ñ__Ð_µ_Ð_½_Ð_·
    QPay v2 Ð³Ò¯Ð¹Ð»Ð³ÑÑÐ½Ð¸Ð¹ ÑÐµÑÐ²Ð¸ÑÒ¯Ò¯Ð´Ð¸Ð¹Ð³ Python ÑÑÐ»Ð½Ð¸Ð¹
            Ð¾ÑÑÐ¸Ð½Ð´ Ð°ÑÐ¸Ð³Ð»Ð°ÑÐ°Ð´ Ð·Ð¾ÑÐ¸ÑÐ»ÑÐ°Ð½ ÑÐ°Ð½
 ### QPayClient -Ð³ Ð°ÑÐ¸Ð³Ð»Ð°Ñ Ð¥Ð°Ð¼Ð³Ð¸Ð¹Ð½ ÑÑÐ»ÑÑÐ´ `QPayClient` -Ñ
 Ð¾Ð±ÑÐµÐºÑ Ò¯Ò¯ÑÐ³ÑÐ¶ Ð°Ð²Ð½Ð°. ÐÐ½Ð³ÑÑÐ¸Ð¹Ð½ ÑÑÐ»Ð´ KKTÐ¢ Ð¥Ð¥Ð -
```

### Comparing `qpay_python-0.0.1/pyproject.toml` & `qpay_python-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qpay-python"
-version = "0.0.1"
+version = "0.0.2"
 description = "QPay v2 SDK client for Python projects"
 authors = ["khasbilegt <khasbilegt.ts@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/khasbilegt/qpay-python"
 repository = "https://github.com/khasbilegt/qpay-python"
 keywords = ["python", "qpay", "sdk", "payment", "qr", "finance"]
@@ -27,15 +27,15 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
 pydantic = "^2.7.0"
 
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.2.0"
+ruff = "^0.4.1"
 pre-commit = "^3.5.0"
 pytest = "^7.4.3"
 requests-mock = "^1.12.1"
 pytest-cov = "^5.0.0"
 mypy = "^1.9.0"
 types-requests = "^2.31.0.20240406"
```

### Comparing `qpay_python-0.0.1/qpay/auth.py` & `qpay_python-0.0.2/qpay/auth.py`

 * *Files identical despite different names*

### Comparing `qpay_python-0.0.1/qpay/main.py` & `qpay_python-0.0.2/qpay/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from datetime import datetime
 from decimal import Decimal
 from typing import Literal
 from urllib.parse import urljoin
 
 import requests
 from pydantic import BaseModel, Field, field_serializer
 
@@ -26,45 +25,32 @@
     urls: list[URL] = Field(
         description="Аппликейшнээс банкны аппликейшнруу үсрэх Deeplink"
     )
 
 
 class Payment(BaseModel):
     id: str = Field(alias="payment_id", description="QPay-ээс үүссэн гүйлгээний дугаар")
-    date: datetime = Field(alias="payment_date", description="Гүйлгээний огноо")
-    payment_status: Literal["NEW", "FAILED", "PAID", "REFUNDED"] = Field(
+    status: Literal["NEW", "FAILED", "PAID", "REFUNDED"] = Field(
+        alias="payment_status",
         description="Гүйлгээ төлөв NEW: Гүйлгээ үүсгэгдсэн"
         "FAILED: Гүйлгээ амжилтгүй"
         "PAID: Төлөгдсөн"
-        "REFUNDED: Гүйлгээ буцаагдсан"
+        "REFUNDED: Гүйлгээ буцаагдсан",
     )
-    fee: Decimal = Field(alias="payment_fee", description="Шимтгэлийн дүн")
     amount: Decimal = Field(alias="payment_amount", description="Гүйлгээний үнийн дүн")
     currency: Literal["MNT"] = Field(
         alias="payment_currency", description="Гүйлгээний валют"
     )
     wallet: str = Field(
         alias="payment_wallet", description="Гүйлгээ хийсэн воллетийн дугаар"
     )
-    transaction_type: Literal["P2P", "CARD"] = Field(
-        description="Гүйлгээний төрөл P2P: Дансны гүйлгээ CARD: Картын гүйлгээ"
+    type: Literal["P2P", "CARD"] = Field(
+        alias="payment_type",
+        description="Гүйлгээний төрөл P2P: Дансны гүйлгээ CARD: Картын гүйлгээ",
     )
-    # payment_name: str = Field(description="Төлбөрийн нэр: Юнивишн")
-    # payment_description: str = Field(description="Гүйлгээний утга: Юнивишн төлбөр")
-    # qr_code: str = Field(description="Гүйлгээнд ашиглагдсан QR код")
-    # paid_by: Literal["P2P", "CARD"] = Field(
-    #     description="Гүйлгээний төрөл P2P: Дансны гүйлгээ CARD: Картын гүйлгээ"
-    # )
-    # object_type: Literal["MERCHANT", "INVOICE", "QR"] = Field(
-    #     description="Обьектын төрөл"
-    # )
-    # object_id: str = Field(
-    #     description="Обьектын төрөл INVOICE үед нэхэмлэхийн код (invoice_code)"
-    #     "Обьектын төрөл QR үед QR код"
-    # )
 
 
 class CreateInvoicePayload(BaseModel):
     invoice_code: str = Field(description="QPay-ээс өгсөн нэхэмжлэхийн код")
     sender_invoice_no: str = Field(
         description="Байгууллагаас үүсгэх давтагдашгүй нэхэмжлэлийн дугаар"
     )
@@ -110,14 +96,17 @@
         response = self._request("post", "invoice", json=payload.model_dump())
         return Invoice(**response)
 
     def invoice_cancel(self, invoice_id: str) -> bool:
         response = self._request("delete", f"invoice/{invoice_id}")
         return "error" not in response
 
-    def payment_check(self, invoice_id: str) -> list[Payment]:
+    def payment_check(self, invoice_id: str) -> bool:
         response = self._request(
             "post",
             "payment/check",
             json={"object_type": "INVOICE", "object_id": invoice_id},
         )
-        return [Payment(**payment) for payment in response["rows"]]
+
+        if (rows := response["rows"]) and (len(rows) == 1) and (payment := rows[0]):
+            return payment["payment_status"] == "PAID"
+        return False
```

### Comparing `qpay_python-0.0.1/PKG-INFO` & `qpay_python-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qpay-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: QPay v2 SDK client for Python projects
 Home-page: https://github.com/khasbilegt/qpay-python
 License: MIT
 Keywords: python,qpay,sdk,payment,qr,finance
 Author: khasbilegt
 Author-email: khasbilegt.ts@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -22,15 +22,15 @@
 Classifier: Typing :: Typed
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/khasbilegt/qpay-python
 Description-Content-Type: text/markdown
 
 <h1 align="center">
-  QPayClient
+  QPay Python
 </h1>
 
 <p align="center">
   <a href="https://github.com/khasbilegt/qpay-python/">
     <img src="https://img.shields.io/github/actions/workflow/status/khasbilegt/qpay-python/qa.yml?label=CI&logo=github&style=for-the-badge" alt="ci status">
   </a>
   <a href="https://codecov.io/github/khasbilegt/qpay-python">
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: qpay-python Version: 0.0.1 Summary: QPay v2 SDK
+Metadata-Version: 2.1 Name: qpay-python Version: 0.0.2 Summary: QPay v2 SDK
 client for Python projects Home-page: https://github.com/khasbilegt/qpay-python
 License: MIT Keywords: python,qpay,sdk,payment,qr,finance Author: khasbilegt
 Author-email: khasbilegt.ts@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
 Framework :: Pydantic Classifier: Framework :: Pytest Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Build Tools Classifier: Typing :: Typed
 Requires-Dist: pydantic (>=2.7.0,<3.0.0) Requires-Dist: requests
 (>=2.31.0,<3.0.0) Project-URL: Repository, https://github.com/khasbilegt/qpay-
 python Description-Content-Type: text/markdown
-                           ************ QQPPaayyCClliieenntt ************
+                           ************ QQPPaayy PPyytthhoonn ************
                              _[_c_i_ _s_t_a_t_u_s_]_[_c_o_d_e_c_o_v_]
                     _[_p_y_p_i_ _l_i_n_k_][supported python versions]
  _Ð__Ñ__Ð_¸_Ð_³_Ð_»_Ð_°_Ñ_ â¢ _Ð_¥_Ó_©_Ð_³_Ð_¶_Ò_¯_Ò_¯_Ð_»_Ñ__Ð_»_Ñ__Ñ__Ð_½_Ð_´_ _Ð_¾_Ñ__Ð_¾_Ð_»_Ñ__Ð_¾_Ñ_ â¢ _Ð__Ð_¸_Ñ__Ð_µ_Ð_½_Ð_·
    QPay v2 Ð³Ò¯Ð¹Ð»Ð³ÑÑÐ½Ð¸Ð¹ ÑÐµÑÐ²Ð¸ÑÒ¯Ò¯Ð´Ð¸Ð¹Ð³ Python ÑÑÐ»Ð½Ð¸Ð¹
            Ð¾ÑÑÐ¸Ð½Ð´ Ð°ÑÐ¸Ð³Ð»Ð°ÑÐ°Ð´ Ð·Ð¾ÑÐ¸ÑÐ»ÑÐ°Ð½ ÑÐ°Ð½
 ### QPayClient -Ð³ Ð°ÑÐ¸Ð³Ð»Ð°Ñ Ð¥Ð°Ð¼Ð³Ð¸Ð¹Ð½ ÑÑÐ»ÑÑÐ´ `QPayClient` -Ñ
 Ð¾Ð±ÑÐµÐºÑ Ò¯Ò¯ÑÐ³ÑÐ¶ Ð°Ð²Ð½Ð°. ÐÐ½Ð³ÑÑÐ¸Ð¹Ð½ ÑÑÐ»Ð´ KKTÐ¢ Ð¥Ð¥Ð -
```

