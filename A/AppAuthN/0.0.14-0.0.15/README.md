# Comparing `tmp/AppAuthN-0.0.14.tar.gz` & `tmp/AppAuthN-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppAuthN-0.0.14.tar", last modified: Fri Mar  1 06:04:17 2024, max compression
+gzip compressed data, was "AppAuthN-0.0.15.tar", last modified: Wed May  1 07:01:55 2024, max compression
```

## Comparing `AppAuthN-0.0.14.tar` & `AppAuthN-0.0.15.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-01 06:04:17.320807 AppAuthN-0.0.14/
--rw-rw-rw-   0        0        0     1091 2024-02-26 10:52:10.000000 AppAuthN-0.0.14/LICENSE
--rw-rw-rw-   0        0        0      101 2024-03-01 06:04:17.315813 AppAuthN-0.0.14/PKG-INFO
--rw-rw-rw-   0        0        0      912 2024-02-29 05:43:05.000000 AppAuthN-0.0.14/README.md
--rw-rw-rw-   0        0        0       42 2024-03-01 06:04:17.321806 AppAuthN-0.0.14/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-03-01 06:04:03.000000 AppAuthN-0.0.14/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-01 06:04:17.195883 AppAuthN-0.0.14/src/
-drwxrwxrwx   0        0        0        0 2024-03-01 06:04:17.267838 AppAuthN-0.0.14/src/AppAuthN/
--rw-rw-rw-   0        0        0     4224 2024-03-01 06:03:30.000000 AppAuthN-0.0.14/src/AppAuthN/CertificationReceiver.py
--rw-rw-rw-   0        0        0     1746 2024-02-29 12:52:55.000000 AppAuthN-0.0.14/src/AppAuthN/CloseLoopCounter.py
--rw-rw-rw-   0        0        0     2567 2024-03-01 06:02:21.000000 AppAuthN-0.0.14/src/AppAuthN/InferenceResult.py
--rw-rw-rw-   0        0        0        0 2024-02-26 10:52:10.000000 AppAuthN-0.0.14/src/AppAuthN/__init__.py
--rw-rw-rw-   0        0        0      577 2024-03-01 06:03:03.000000 AppAuthN-0.0.14/src/AppAuthN/config.json
-drwxrwxrwx   0        0        0        0 2024-03-01 06:04:17.309813 AppAuthN-0.0.14/src/AppAuthN.egg-info/
--rw-rw-rw-   0        0        0      101 2024-03-01 06:04:16.000000 AppAuthN-0.0.14/src/AppAuthN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2024-03-01 06:04:17.000000 AppAuthN-0.0.14/src/AppAuthN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-01 06:04:16.000000 AppAuthN-0.0.14/src/AppAuthN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-01 06:04:16.000000 AppAuthN-0.0.14/src/AppAuthN.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-01 06:04:16.000000 AppAuthN-0.0.14/src/AppAuthN.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 07:01:55.315994 AppAuthN-0.0.15/
+-rw-rw-rw-   0        0        0     1091 2024-02-26 10:52:10.000000 AppAuthN-0.0.15/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-05-01 07:01:55.313076 AppAuthN-0.0.15/PKG-INFO
+-rw-rw-rw-   0        0        0     1075 2024-05-01 06:59:51.000000 AppAuthN-0.0.15/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 07:01:55.315994 AppAuthN-0.0.15/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-01 07:00:15.000000 AppAuthN-0.0.15/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:01:55.252645 AppAuthN-0.0.15/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 07:01:55.289011 AppAuthN-0.0.15/src/AppAuthN/
+-rw-rw-rw-   0        0        0     4489 2024-05-01 06:56:15.000000 AppAuthN-0.0.15/src/AppAuthN/CertificationReceiver.py
+-rw-rw-rw-   0        0        0     1748 2024-05-01 06:57:34.000000 AppAuthN-0.0.15/src/AppAuthN/CloseLoopCounter.py
+-rw-rw-rw-   0        0        0     2580 2024-05-01 06:57:01.000000 AppAuthN-0.0.15/src/AppAuthN/InferenceResult.py
+-rw-rw-rw-   0        0        0        0 2024-02-26 10:52:10.000000 AppAuthN-0.0.15/src/AppAuthN/__init__.py
+-rw-rw-rw-   0        0        0      638 2024-05-01 06:55:40.000000 AppAuthN-0.0.15/src/AppAuthN/config.json
+drwxrwxrwx   0        0        0        0 2024-05-01 07:01:55.309999 AppAuthN-0.0.15/src/AppAuthN.egg-info/
+-rw-rw-rw-   0        0        0      101 2024-05-01 07:01:54.000000 AppAuthN-0.0.15/src/AppAuthN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2024-05-01 07:01:54.000000 AppAuthN-0.0.15/src/AppAuthN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 07:01:54.000000 AppAuthN-0.0.15/src/AppAuthN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-01 07:01:54.000000 AppAuthN-0.0.15/src/AppAuthN.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-01 07:01:54.000000 AppAuthN-0.0.15/src/AppAuthN.egg-info/top_level.txt
```

### Comparing `AppAuthN-0.0.14/LICENSE` & `AppAuthN-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `AppAuthN-0.0.14/README.md` & `AppAuthN-0.0.15/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -9,34 +9,36 @@
     ```bash
    pip install AppAuthN
     
 2. 進行註冊
 
     ```python
     #模型
-    import CertificationReceiver as register
-    api = <url>
-    register.kongapi(api)
+    import AppAuthN.CertificationReceiver as register
+    register_api = <url>
+    inference_api = <url>
+    register.kongapi(register_api, inference_api)
 
     register_data = {
-        "application_token": "1234",
-        "position_uid": "6543",
-        "inference_client_uid": "5678"
+        "application_uid": <application_uid>,
+        "application_token": <application_token>,
+        "position_uid": <position_uid>,
+        "inference_client_name": <inference_client_name>,
     }
     register.send_register_request(register_data)
 
 3. 進行推論：
 
    ```python
     #模型
-    import InferenceResult as inference
+    import AppAuthN.InferenceResult as infer
     raw_data = {
         "application_uid": <application_uid>,
         "position_uid": <position_uid>,
-        "inference_client_uid": <inference_client_uid>,
+        "inference_client_name": <inference_client_name>,
         "value": <value>
     }
     inference.send_rawdata(raw_data)
 
 # 注意事项
 
 -請確保提供有效的输入，否則驗證可能會失败。
```

### Comparing `AppAuthN-0.0.14/src/AppAuthN/CertificationReceiver.py` & `AppAuthN-0.0.15/src/AppAuthN/CertificationReceiver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import hashlib
 import json, os, requests
 import time
 
-def kongapi(api_url):
+def kongapi(api_url_with_register, api_url_with_inference):
     data = data_mgt.read_json()
-    data["api_url"] = api_url
+    data["api_url_with_R"] = api_url_with_register
+    data["api_url_with_I"] = api_url_with_inference
     data_mgt.write_json(data)
 
 ## 驗證certificate.hash
 def generate_hash(data):
     # Combine values into a single string
-    combined_string = f"""{data["register"]["application_token"]}{data["register"]["position_uid"]}{data["register"]["inference_client_uid"]}"""
+    combined_string = f"""{data["register"]["application_token"]}{data["register"]["position_uid"]}{data["register"]["inference_client_name"]}"""
 
     # Create a hash object using SHA-256 (you can choose a different algorithm)
     # Get the hexadecimal representation of the hash
     hash_value = hashlib.sha256(combined_string.encode()).hexdigest()
     #print("local_hash_value:", hash_value)
     return hash_value
 
@@ -37,25 +38,27 @@
         with open(self.json_file_path, "w") as json_file:
             json.dump(data, json_file, indent=2)
 
 
 ## interact with inference_layer
 def send_register_request(register_data):
     data = data_mgt.read_json()
+    data["register"]["application_uid"] = register_data["application_uid"]
     data["register"]["application_token"] = register_data["application_token"]
-    data["register"]["inference_client_uid"] = register_data["inference_client_uid"]
+    data["register"]["inference_client_name"] = register_data["inference_client_name"]
     data["register"]["position_uid"] = register_data["position_uid"]
 
     # API endpoint for registration
-    registration_endpoint = f"""{data["api_url"]}/certificate"""
+    registration_endpoint = f"""{data["api_url_with_R"]}/certificate"""
 
     # Data to be sent in the POST request
     payload = {
+        "application_uid": data["register"]["application_uid"],
         "application_token": data["register"]["application_token"],
-        "inference_client_uid": data["register"]["inference_client_uid"],
+        "inference_client_name": data["register"]["inference_client_name"],
         "position_uid": data["register"]["position_uid"]
     }
     # print("Data to be sent:")
     # print(json.dumps(payload, indent=2))
 
     try:
         # Make the POST request
```

### Comparing `AppAuthN-0.0.14/src/AppAuthN/CloseLoopCounter.py` & `AppAuthN-0.0.15/src/AppAuthN/CloseLoopCounter.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     closed_loop_endpoint = f"""{data["api_url"]}/closed-loop-{data["closed_loop"]["position_uid"]}"""
 
     data["closed_loop"]["value"] = global_counter.get_value()
     payload = {
         "application_uid": data["closed_loop"]["application_uid"],
         "position_uid": data["closed_loop"]["position_uid"],
         "packet_uid": data["closed_loop"]["packet_uid"],
-        "inference_client_uid": data["closed_loop"]["inference_client_uid"],
+        "inference_client_name": data["closed_loop"]["inference_client_name"],
         "value": data["closed_loop"]["value"]
     }
     # print("Data to be sent:")
     # print(json.dumps(payload, indent=2))
 
     try:
         # Make the POST request
```

### Comparing `AppAuthN-0.0.14/src/AppAuthN/InferenceResult.py` & `AppAuthN-0.0.15/src/AppAuthN/InferenceResult.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 
 ## send rawdata to inference layer for receiving inference result
 def send_rawdata(rawdata):
     data = data_mgt.read_json()
     check_identity(data)
     data["raw_data"]["application_uid"] = rawdata["application_uid"]
     data["raw_data"]["position_uid"] = rawdata["position_uid"]
-    data["raw_data"]["inference_client_uid"] = rawdata["inference_client_uid"]
+    data["raw_data"]["inference_client_name"] = rawdata["inference_client_name"]
     data["raw_data"]["value"] = rawdata["value"]
     # print("merge_data", data)
 
     # API endpoint for inference_service
-    inference_service_endpoint = f"""{data["api_url"]}/inference-service-{data["raw_data"]["position_uid"]}"""
+    inference_service_endpoint = f"""{data["api_url_with_I"]}/inference-service-{data["raw_data"]["position_uid"]}"""
 
     data["raw_data"]["packet_uid"] = str(int(data["raw_data"]["packet_uid"])+1)
     payload = {
         "application_uid": data["raw_data"]["application_uid"],
         "position_uid": data["raw_data"]["position_uid"],
         "packet_uid": data["raw_data"]["packet_uid"],
-        "inference_client_uid": data["raw_data"]["inference_client_uid"],
+        "inference_client_name": data["raw_data"]["inference_client_name"],
         "value": data["raw_data"]["value"]
     }
     data["closed_loop"]["application_uid"] = data["raw_data"]["application_uid"]
     data["closed_loop"]["position_uid"] = data["raw_data"]["position_uid"]
     data["closed_loop"]["packet_uid"] = data["raw_data"]["packet_uid"]
-    data["closed_loop"]["inference_client_uid"] = data["raw_data"]["inference_client_uid"]
+    data["closed_loop"]["inference_client_name"] = data["raw_data"]["inference_client_name"]
     # print("Data to be sent:")
     # print(json.dumps(payload, indent=2))
 
     try:
         # Make the POST request
         global_counter.reset()
         response = requests.post(inference_service_endpoint, json=payload)
```

### Comparing `AppAuthN-0.0.14/src/AppAuthN/config.json` & `AppAuthN-0.0.15/src/AppAuthN/config.json`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-00000000: 7b0d 0a20 2022 6170 695f 7572 6c22 3a20  {..  "api_url": 
-00000010: 2222 2c0d 0a20 2022 7265 6769 7374 6572  "",..  "register
-00000020: 223a 207b 0d0a 2020 2020 2261 7070 6c69  ": {..    "appli
-00000030: 6361 7469 6f6e 5f74 6f6b 656e 223a 2022  cation_token": "
-00000040: 222c 0d0a 2020 2020 2270 6f73 6974 696f  ",..    "positio
-00000050: 6e5f 7569 6422 3a20 2222 2c0d 0a20 2020  n_uid": "",..   
-00000060: 2022 696e 6665 7265 6e63 655f 636c 6965   "inference_clie
-00000070: 6e74 5f75 6964 223a 2022 220d 0a20 207d  nt_uid": ""..  }
-00000080: 2c0d 0a20 2022 636c 6f73 6564 5f6c 6f6f  ,..  "closed_loo
-00000090: 7022 3a20 7b0d 0a20 2020 2022 6170 706c  p": {..    "appl
-000000a0: 6963 6174 696f 6e5f 7569 6422 3a20 2222  ication_uid": ""
-000000b0: 2c0d 0a20 2020 2022 706f 7369 7469 6f6e  ,..    "position
-000000c0: 5f75 6964 223a 2022 222c 0d0a 2020 2020  _uid": "",..    
-000000d0: 2270 6163 6b65 745f 7569 6422 3a20 2222  "packet_uid": ""
-000000e0: 2c0d 0a20 2020 2022 696e 6665 7265 6e63  ,..    "inferenc
-000000f0: 655f 636c 6965 6e74 5f75 6964 223a 2022  e_client_uid": "
-00000100: 222c 0d0a 2020 2020 2276 616c 7565 223a  ",..    "value":
-00000110: 200d 0a20 207d 2c0d 0a20 2022 6365 7274   ..  },..  "cert
-00000120: 6966 6963 6174 655f 7265 6365 6976 6572  ificate_receiver
-00000130: 223a 207b 0d0a 2020 2020 2273 7461 7475  ": {..    "statu
-00000140: 7322 3a20 2222 2c0d 0a20 2020 2022 6365  s": "",..    "ce
-00000150: 7274 6966 6963 6174 6522 3a20 2222 0d0a  rtificate": ""..
-00000160: 2020 7d2c 0d0a 2020 2272 6573 756c 745f    },..  "result_
-00000170: 7265 6365 6976 6572 223a 207b 0d0a 2020  receiver": {..  
-00000180: 2020 2273 7461 7475 7322 3a20 2222 2c0d    "status": "",.
-00000190: 0a20 2020 2022 7661 6c75 6522 3a20 2222  .    "value": ""
-000001a0: 0d0a 2020 7d2c 0d0a 2020 2272 6177 5f64  ..  },..  "raw_d
-000001b0: 6174 6122 3a20 7b0d 0a20 2020 2022 6170  ata": {..    "ap
-000001c0: 706c 6963 6174 696f 6e5f 7569 6422 3a20  plication_uid": 
-000001d0: 2222 2c0d 0a20 2020 2022 706f 7369 7469  "",..    "positi
-000001e0: 6f6e 5f75 6964 223a 2022 222c 0d0a 2020  on_uid": "",..  
-000001f0: 2020 2270 6163 6b65 745f 7569 6422 3a20    "packet_uid": 
-00000200: 2231 3133 3222 2c0d 0a20 2020 2022 696e  "1132",..    "in
-00000210: 6665 7265 6e63 655f 636c 6965 6e74 5f75  ference_client_u
-00000220: 6964 223a 2022 222c 0d0a 2020 2020 2276  id": "",..    "v
-00000230: 616c 7565 223a 2022 220d 0a20 207d 0d0a  alue": ""..  }..
-00000240: 7d                                       }
+00000000: 7b0d 0a20 2022 6170 695f 7572 6c5f 7769  {..  "api_url_wi
+00000010: 7468 5f52 223a 2022 222c 0d0a 2020 2261  th_R": "",..  "a
+00000020: 7069 5f75 726c 5f77 6974 685f 4922 3a20  pi_url_with_I": 
+00000030: 2222 2c0d 0a20 2022 7265 6769 7374 6572  "",..  "register
+00000040: 223a 207b 0d0a 2020 2020 2261 7070 6c69  ": {..    "appli
+00000050: 6361 7469 6f6e 5f75 6964 223a 2022 222c  cation_uid": "",
+00000060: 0d0a 2020 2020 2261 7070 6c69 6361 7469  ..    "applicati
+00000070: 6f6e 5f74 6f6b 656e 223a 2022 222c 0d0a  on_token": "",..
+00000080: 2020 2020 2270 6f73 6974 696f 6e5f 7569      "position_ui
+00000090: 6422 3a20 2222 2c0d 0a20 2020 2022 696e  d": "",..    "in
+000000a0: 6665 7265 6e63 655f 636c 6965 6e74 5f6e  ference_client_n
+000000b0: 616d 6522 3a20 2222 0d0a 2020 7d2c 0d0a  ame": ""..  },..
+000000c0: 2020 2263 6c6f 7365 645f 6c6f 6f70 223a    "closed_loop":
+000000d0: 207b 0d0a 2020 2020 2261 7070 6c69 6361   {..    "applica
+000000e0: 7469 6f6e 5f75 6964 223a 2022 222c 0d0a  tion_uid": "",..
+000000f0: 2020 2020 2270 6f73 6974 696f 6e5f 7569      "position_ui
+00000100: 6422 3a20 2222 2c0d 0a20 2020 2022 7061  d": "",..    "pa
+00000110: 636b 6574 5f75 6964 223a 2022 222c 0d0a  cket_uid": "",..
+00000120: 2020 2020 2269 6e66 6572 656e 6365 5f63      "inference_c
+00000130: 6c69 656e 745f 6e61 6d65 223a 2022 222c  lient_name": "",
+00000140: 0d0a 2020 2020 2276 616c 7565 223a 2022  ..    "value": "
+00000150: 220d 0a20 207d 2c0d 0a20 2022 6365 7274  "..  },..  "cert
+00000160: 6966 6963 6174 655f 7265 6365 6976 6572  ificate_receiver
+00000170: 223a 207b 0d0a 2020 2020 2273 7461 7475  ": {..    "statu
+00000180: 7322 3a20 2222 2c0d 0a20 2020 2022 6365  s": "",..    "ce
+00000190: 7274 6966 6963 6174 6522 3a20 2222 0d0a  rtificate": ""..
+000001a0: 2020 7d2c 0d0a 2020 2272 6573 756c 745f    },..  "result_
+000001b0: 7265 6365 6976 6572 223a 207b 0d0a 2020  receiver": {..  
+000001c0: 2020 2273 7461 7475 7322 3a20 2222 2c0d    "status": "",.
+000001d0: 0a20 2020 2022 7661 6c75 6522 3a20 2222  .    "value": ""
+000001e0: 0d0a 2020 7d2c 0d0a 2020 2272 6177 5f64  ..  },..  "raw_d
+000001f0: 6174 6122 3a20 7b0d 0a20 2020 2022 6170  ata": {..    "ap
+00000200: 706c 6963 6174 696f 6e5f 7569 6422 3a20  plication_uid": 
+00000210: 2222 2c0d 0a20 2020 2022 706f 7369 7469  "",..    "positi
+00000220: 6f6e 5f75 6964 223a 2022 222c 0d0a 2020  on_uid": "",..  
+00000230: 2020 2270 6163 6b65 745f 7569 6422 3a20    "packet_uid": 
+00000240: 2222 2c0d 0a20 2020 2022 696e 6665 7265  "",..    "infere
+00000250: 6e63 655f 636c 6965 6e74 5f6e 616d 6522  nce_client_name"
+00000260: 3a20 2222 2c0d 0a20 2020 2022 7661 6c75  : "",..    "valu
+00000270: 6522 3a20 2222 0d0a 2020 7d0d 0a7d       e": ""..  }..}
```

