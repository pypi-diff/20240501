# Comparing `tmp/oaas_sdk_py-0.2.4.tar.gz` & `tmp/oaas_sdk_py-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaas_sdk_py-0.2.4.tar", last modified: Mon Mar 25 22:31:32 2024, max compression
+gzip compressed data, was "oaas_sdk_py-0.2.5.tar", last modified: Wed May  1 20:04:05 2024, max compression
```

## Comparing `oaas_sdk_py-0.2.4.tar` & `oaas_sdk_py-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 22:31:32.202051 oaas_sdk_py-0.2.4/
--rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      323 2024-03-25 22:31:32.201046 oaas_sdk_py-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.2.4/README.md
--rw-rw-rw-   0        0        0      497 2024-03-25 22:28:39.000000 oaas_sdk_py-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-25 22:31:32.202051 oaas_sdk_py-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-25 22:31:32.187616 oaas_sdk_py-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2024-03-25 22:31:32.191629 oaas_sdk_py-0.2.4/src/oaas_sdk_py/
--rw-rw-rw-   0        0        0     9651 2024-03-25 22:28:39.000000 oaas_sdk_py-0.2.4/src/oaas_sdk_py/__init__.py
--rw-rw-rw-   0        0        0     1869 2024-03-25 22:28:39.000000 oaas_sdk_py-0.2.4/src/oaas_sdk_py/model.py
-drwxrwxrwx   0        0        0        0 2024-03-25 22:31:32.200048 oaas_sdk_py-0.2.4/src/oaas_sdk_py.egg-info/
--rw-rw-rw-   0        0        0      323 2024-03-25 22:31:32.000000 oaas_sdk_py-0.2.4/src/oaas_sdk_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-03-25 22:31:32.000000 oaas_sdk_py-0.2.4/src/oaas_sdk_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 22:31:32.000000 oaas_sdk_py-0.2.4/src/oaas_sdk_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-03-25 22:31:32.000000 oaas_sdk_py-0.2.4/src/oaas_sdk_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-25 22:31:32.000000 oaas_sdk_py-0.2.4/src/oaas_sdk_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 20:04:05.238904 oaas_sdk_py-0.2.5/
+-rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      323 2024-05-01 20:04:05.237898 oaas_sdk_py-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.2.5/README.md
+-rw-rw-rw-   0        0        0      497 2024-05-01 20:03:34.000000 oaas_sdk_py-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 20:04:05.238904 oaas_sdk_py-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 20:04:05.224624 oaas_sdk_py-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 20:04:05.229698 oaas_sdk_py-0.2.5/src/oaas_sdk_py/
+-rw-rw-rw-   0        0        0     9873 2024-05-01 19:49:33.000000 oaas_sdk_py-0.2.5/src/oaas_sdk_py/__init__.py
+-rw-rw-rw-   0        0        0     1869 2024-03-25 22:28:39.000000 oaas_sdk_py-0.2.5/src/oaas_sdk_py/model.py
+drwxrwxrwx   0        0        0        0 2024-05-01 20:04:05.235861 oaas_sdk_py-0.2.5/src/oaas_sdk_py.egg-info/
+-rw-rw-rw-   0        0        0      323 2024-05-01 20:04:05.000000 oaas_sdk_py-0.2.5/src/oaas_sdk_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-05-01 20:04:05.000000 oaas_sdk_py-0.2.5/src/oaas_sdk_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 20:04:05.000000 oaas_sdk_py-0.2.5/src/oaas_sdk_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-01 20:04:05.000000 oaas_sdk_py-0.2.5/src/oaas_sdk_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-01 20:04:05.000000 oaas_sdk_py-0.2.5/src/oaas_sdk_py.egg-info/top_level.txt
```

### Comparing `oaas_sdk_py-0.2.4/LICENSE` & `oaas_sdk_py-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oaas_sdk_py-0.2.4/src/oaas_sdk_py/__init__.py` & `oaas_sdk_py-0.2.5/src/oaas_sdk_py/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,31 +99,37 @@
             self.allocate_url_dict = self.allocate_url_dict | resp_dict
         return self.allocate_url_dict
 
     async def upload_byte_data(self,
                                session: ClientSession,
                                key: str,
                                data: bytes) -> None:
-        if self.allocate_url_dict is None:
+        if key in self.task.output_keys:
+            url = self.task.output_keys[key]
+        elif self.allocate_url_dict is None:
             await self.allocate_file(session)
-        url = self.allocate_url_dict[key]
+            url = self.allocate_url_dict[key]
+        else:
+            url = self.allocate_url_dict[key]
         if url is None:
             raise OaasException(f"The output object not accept '{key}' as key")
         resp = await session.put(url, data=data)
         if not resp.ok:
             raise OaasException("Got error when put the data to S3")
         self.task.output_obj.updated_keys.append(key)
 
     async def upload_main_byte_data(self,
                                     session: ClientSession,
                                     key: str,
                                     data: bytes) -> None:
         if self.allocate_main_url_dict is None:
             await self.allocate_main_file(session)
-        url = self.allocate_main_url_dict[key]
+            url = self.allocate_main_url_dict[key]
+        else:
+            url = self.allocate_url_dict[key]
         if url is None:
             raise OaasException(f"The main object not accept '{key}' as key")
         resp = await session.put(url, data=data)
         if not resp.ok:
             raise OaasException("Got error when put the data to S3")
         self.task.main_obj.updated_keys.append(key)
```

### Comparing `oaas_sdk_py-0.2.4/src/oaas_sdk_py/model.py` & `oaas_sdk_py-0.2.5/src/oaas_sdk_py/model.py`

 * *Files identical despite different names*

