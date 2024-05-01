# Comparing `tmp/caltechdata_api-1.6.0.tar.gz` & `tmp/caltechdata_api-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caltechdata_api-1.6.0.tar", last modified: Fri Apr 19 22:17:10 2024, max compression
+gzip compressed data, was "caltechdata_api-1.6.1.tar", last modified: Wed May  1 19:51:59 2024, max compression
```

## Comparing `caltechdata_api-1.6.0.tar` & `caltechdata_api-1.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:17:10.670002 caltechdata_api-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-19 22:17:10.670002 caltechdata_api-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:17:10.670002 caltechdata_api-1.6.0/caltechdata_api/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/caltechdata_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/caltechdata_write.py
--rw-r--r--   0 runner    (1001) docker     (127)    22623 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/customize_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/download_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/get_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/get_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/md_to_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/caltechdata_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:17:10.670002 caltechdata_api-1.6.0/caltechdata_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-19 22:17:10.000000 caltechdata_api-1.6.0/caltechdata_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 22:17:10.000000 caltechdata_api-1.6.0/caltechdata_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:17:10.000000 caltechdata_api-1.6.0/caltechdata_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 22:17:10.000000 caltechdata_api-1.6.0/caltechdata_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 22:17:10.000000 caltechdata_api-1.6.0/caltechdata_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 22:17:10.000000 caltechdata_api-1.6.0/caltechdata_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:17:10.670002 caltechdata_api-1.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4774 2024-04-19 22:17:05.000000 caltechdata_api-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:59.909529 caltechdata_api-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-01 19:51:55.000000 caltechdata_api-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-01 19:51:59.909529 caltechdata_api-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-01 19:51:55.000000 caltechdata_api-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:59.909529 caltechdata_api-1.6.1/caltechdata_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-01 19:51:55.000000 caltechdata_api-1.6.1/caltechdata_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-05-01 19:51:55.000000 caltechdata_api-1.6.1/caltechdata_api/caltechdata_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-05-01 19:51:55.000000 caltechdata_api-1.6.1/caltechdata_api/caltechdata_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24763 2024-05-01 19:51:55.000000 caltechdata_api-1.6.1/caltechdata_api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-05-01 19:51:55.000000 caltechdata_api-1.6.1/caltechdata_api/customize_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-01 19:51:55.000000 caltechdata_api-1.6.1/caltechdata_api/download_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-01 19:51:55.000000 caltechdata_api-1.6.1/caltechdata_api/get_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-01 19:51:55.000000 caltechdata_api-1.6.1/caltechdata_api/get_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-01 19:51:55.000000 caltechdata_api-1.6.1/caltechdata_api/md_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-01 19:51:55.000000 caltechdata_api-1.6.1/caltechdata_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:59.909529 caltechdata_api-1.6.1/caltechdata_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-01 19:51:59.000000 caltechdata_api-1.6.1/caltechdata_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-01 19:51:59.000000 caltechdata_api-1.6.1/caltechdata_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:51:59.000000 caltechdata_api-1.6.1/caltechdata_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 19:51:59.000000 caltechdata_api-1.6.1/caltechdata_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 19:51:59.000000 caltechdata_api-1.6.1/caltechdata_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 19:51:59.000000 caltechdata_api-1.6.1/caltechdata_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:51:59.909529 caltechdata_api-1.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4773 2024-05-01 19:51:55.000000 caltechdata_api-1.6.1/setup.py
```

### Comparing `caltechdata_api-1.6.0/LICENSE` & `caltechdata_api-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.6.0/PKG-INFO` & `caltechdata_api-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caltechdata_api
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python wrapper for CaltechDATA API.
 Home-page: https://github.com/caltechlibrary/caltechdata_api
 Author: Thomas E Morrell
 Author-email: tmorrell@caltech.edu
 License: https://data.caltech.edu/license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `caltechdata_api-1.6.0/README.md` & `caltechdata_api-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.6.0/caltechdata_api/caltechdata_edit.py` & `caltechdata_api-1.6.1/caltechdata_api/caltechdata_edit.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.6.0/caltechdata_api/caltechdata_write.py` & `caltechdata_api-1.6.1/caltechdata_api/caltechdata_write.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.6.0/caltechdata_api/cli.py` & `caltechdata_api-1.6.1/caltechdata_api/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import requests
 import s3fs
 from caltechdata_api import caltechdata_write, caltechdata_edit
 from .md_to_json import parse_readme_to_json
 import json
 import os
-import configparser
+from cryptography.fernet import Fernet
 
 CALTECHDATA_API = "https://data.caltech.edu/api/names?q=identifiers.identifier:{}"
 ORCID_API = "https://orcid.org/"
 HEADERS = {"Accept": "application/json"}
 
 name = ""
 affiliationIdentifierScheme = ""
@@ -17,34 +17,68 @@
 
 awardNumber = ""
 awardTitle = ""
 funderIdentifier = ""
 funderIdentifierType = ""
 funderName = ""
 
+home_directory = os.path.expanduser("~")
+caltechdata_directory = os.path.join(home_directory, ".caltechdata")
 
-CONFIG_FILE = "caltechdata_config.ini"
 
+if not os.path.exists(caltechdata_directory):
+    os.makedirs(caltechdata_directory)
 
-def get_or_set_token():
-    config = configparser.ConfigParser()
 
-    if os.path.isfile(CONFIG_FILE):
-        config.read(CONFIG_FILE)
-        if "CaltechDATA" in config and "token" in config["CaltechDATA"]:
-            return config["CaltechDATA"]["token"]
+def generate_key():
+    return Fernet.generate_key()
+
+
+# Load the key from a file or generate a new one if not present
+def load_or_generate_key():
+    key_file = os.path.join(caltechdata_directory, "key.key")
+    if os.path.exists(key_file):
+        with open(key_file, "rb") as f:
+            return f.read()
     else:
+        key = generate_key()
+        with open(key_file, "wb") as f:
+            f.write(key)
+        return key
+
+
+# Encrypt the token
+def encrypt_token(token, key):
+    f = Fernet(key)
+    return f.encrypt(token.encode())
+
+
+# Decrypt the token
+def decrypt_token(encrypted_token, key):
+    f = Fernet(key)
+    return f.decrypt(encrypted_token).decode()
+
+
+# Function to get or set token
+def get_or_set_token():
+    key = load_or_generate_key()
+    token_file = os.path.join(caltechdata_directory, "token.txt")
+    try:
+        with open(token_file, "rb") as f:
+            encrypted_token = f.read()
+            token = decrypt_token(encrypted_token, key)
+            return token
+    except FileNotFoundError:
         while True:
-            token = get_user_input("Enter your CaltechDATA token: ")
-            confirm_token = get_user_input("Confirm your CaltechDATA token: ")
+            token = input("Enter your CaltechDATA token: ").strip()
+            confirm_token = input("Confirm your CaltechDATA token: ").strip()
             if token == confirm_token:
-                config.add_section("CaltechDATA")
-                config.set("CaltechDATA", "token", token)
-                with open(CONFIG_FILE, "w") as configfile:
-                    config.write(configfile)
+                encrypted_token = encrypt_token(token, key)
+                with open(token_file, "wb") as f:
+                    f.write(encrypted_token)
                 return token
             else:
                 print("Tokens do not match. Please try again.")
 
 
 def welcome_message():
     print("Welcome to CaltechDATA CLI")
@@ -212,34 +246,50 @@
             print(
                 f"Error: ORCID identifier not found or invalid. Please check the ORCID identifier and try again."
             )
             return None, None
     return family_name, given_name
 
 
+def write_s3cmd_config(access_key, secret_key, endpoint):
+    configf = os.path.join(home_directory, ".s3cfg")
+    if not os.path.exists(key_file):
+        with open(configf, "w") as file:
+            file.write(
+                f"""[default]
+            access_key = {access_key}
+            host_base = {endpoint}
+            host_bucket = %(bucket).{endpoint}
+            secret_key = {secret_key}
+            """
+            )
+
+
 def upload_supporting_file(record_id=None):
     filepath = ""
-    file_link = ""
+    filepaths = []
+    file_links = []
     while True:
         choice = get_user_input(
             "Do you want to upload or link data files? (upload/link/n): "
         ).lower()
         if choice == "link":
-            endpoint = "https://sdsc.osn.xsede.org/"
+            endpoint = "sdsc.osn.xsede.org"
             path = "ini230004-bucket01/"
-
             if not record_id:
-                record_id = get_user_input("Folder where OSN files are uploaded")
-
+                access_key = get_user_input("Enter the access key: ")
+                secret_key = get_user_input("Enter the secret key: ")
+                write_s3cmd_config(access_key, secret_key, endpoint)
+                print("""S3 connection configured.""")
+                break
+            endpoint = f"https://{endpoint}/"
             s3 = s3fs.S3FileSystem(anon=True, client_kwargs={"endpoint_url": endpoint})
             # Find the files
             files = s3.glob(path + record_id + "/*")
 
-            file_links = []
-
             for link in files:
                 fname = link.split("/")[-1]
                 if "." not in fname:
                     # If there is a directory, get files
                     folder_files = s3.glob(link + "/*")
                     for file in folder_files:
                         name = file.split("/")[-1]
@@ -260,41 +310,46 @@
             return filepath, file_links
         elif choice == "upload":
             print("Current files in the directory:")
             files = [
                 f for f in os.listdir() if not f.endswith(".json") and os.path.isfile(f)
             ]
             print("\n".join(files))
-            filename = get_user_input(
-                "Enter the filename to upload as a supporting file: "
-            )
-            if filename in files:
-                file_size = os.path.getsize(filename)
-                if file_size > 1024 * 1024 * 1024:
-                    file_link = get_user_input(
-                        "Enter the S3 link to the file (File size is more than 1GB): "
-                    )
-                    if file_link:
-                        return filepath, file_link
+            while True:
+                filename = get_user_input(
+                    "Enter the filename to upload as a supporting file (or 'n' to finish): "
+                )
+                if filename == "n":
+                    break
+                if filename in files:
+                    file_size = os.path.getsize(filename)
+                    if file_size > 1024 * 1024 * 1024:
+                        print(
+                            """The file is greater than 1 GB. Please upload the
+                        metadata to CaltechDATA, and you'll be provided
+                        instructions to upload the files to S3 directly."""
+                        )
                     else:
-                        print("Link is required for files larger than 1GB.")
-                        continue
+                        filepath = os.path.abspath(filename)
+                        filepaths.append(filepath)
                 else:
-                    filepath = os.path.abspath(filename)
-                    break
-            else:
-                print(
-                    f"Error: File '{filename}' not found. Please enter a valid filename."
-                )
+                    print(
+                        f"Error: File '{filename}' not found. Please enter a valid filename."
+                    )
+
+            add_more = get_user_input("Do you want to add more files? (y/n): ").lower()
+            if add_more != "y":
+                break
+
         elif choice == "n":
             break
         else:
             print("Invalid input. Please enter 'link' or 'upload' or 'n'.")
 
-    return filepath, file_link
+    return filepaths, file_links
 
 
 def upload_data_from_file():
     while True:
         print("Current JSON files in the directory:")
         files = [f for f in os.listdir() if f.endswith(".json") and os.path.isfile(f)]
         print("\n".join(files))
@@ -357,15 +412,17 @@
                     )
                 else:
                     response = caltechdata_write(
                         existing_data, token, production=False, publish=False
                     )
                 rec_id = response
                 print(
-                    f"You can view and publish this record at https://data.caltechlibrary.dev/uploads/{rec_id}"
+                    f"""You can view and publish this record at https://data.caltechlibrary.dev/uploads/{rec_id}
+                    If you need to upload large files to S3, you can type
+                    `s3cmd put DATA_FILE s3://ini230004-bucket01/{rec_id}/"""
                 )
                 break
             else:
                 print("Going back to the main menu.")
         elif choice == "create":
             args = parse_arguments()
             family_name, given_name = get_names(args["orcid"])
@@ -420,15 +477,17 @@
                     )
                 else:
                     response = caltechdata_write(
                         metadata, token, production=False, publish=False
                     )
                 rec_id = response
                 print(
-                    f"You can view and publish this record at https://data.caltechlibrary.dev/uploads/{rec_id}"
+                    f"""You can view and publish this record at https://data.caltechlibrary.dev/uploads/{rec_id}
+                    If you need to upload large files to S3, you can type
+                    `s3cmd put DATA_FILE s3://ini230004-bucket01/{rec_id}/"""
                 )
                 with open(response + ".json", "w") as file:
                     json.dump(metadata, file, indent=2)
                 break
             else:
                 break
         else:
@@ -470,15 +529,15 @@
                 token=token,
                 file_links=file_link,
                 production=False,
                 publish=False,
             )
         rec_id = response
         print(
-            f"You can view and publish this record at https://data.caltechlibrary.dev/uploads/{rec_id}"
+            f"You can view and publish this record at https://data.caltechlibrary.dev/uploads/{rec_id}\n"
         )
 
 
 def download_file_by_id(record_id, token=None):
     url = f"https://data.caltechlibrary.dev/api/records/{record_id}"
 
     headers = {
```

### Comparing `caltechdata_api-1.6.0/caltechdata_api/customize_schema.py` & `caltechdata_api-1.6.1/caltechdata_api/customize_schema.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.6.0/caltechdata_api/download_file.py` & `caltechdata_api-1.6.1/caltechdata_api/download_file.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.6.0/caltechdata_api/get_files.py` & `caltechdata_api-1.6.1/caltechdata_api/get_files.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.6.0/caltechdata_api/get_metadata.py` & `caltechdata_api-1.6.1/caltechdata_api/get_metadata.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.6.0/caltechdata_api/utils.py` & `caltechdata_api-1.6.1/caltechdata_api/utils.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.6.0/caltechdata_api.egg-info/PKG-INFO` & `caltechdata_api-1.6.1/caltechdata_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caltechdata-api
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python wrapper for CaltechDATA API.
 Home-page: https://github.com/caltechlibrary/caltechdata_api
 Author: Thomas E Morrell
 Author-email: tmorrell@caltech.edu
 License: https://data.caltech.edu/license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `caltechdata_api-1.6.0/caltechdata_api.egg-info/SOURCES.txt` & `caltechdata_api-1.6.1/caltechdata_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.6.0/setup.py` & `caltechdata_api-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 # What packages are required for this module to be executed?
 REQUIRED = [
     "requests",
     "datacite>1.1.0",
     "tqdm>=4.62.3",
     "pyyaml",
     "s3fs",
-    "configparser",
-    "awscli",
+    "cryptography",
+    "s3cmd",
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

