# Comparing `tmp/cloudreve-1.0.0.tar.gz` & `tmp/cloudreve-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudreve-1.0.0.tar", last modified: Tue Apr 30 17:40:53 2024, max compression
+gzip compressed data, was "cloudreve-1.0.1.tar", last modified: Wed May  1 03:40:30 2024, max compression
```

## Comparing `cloudreve-1.0.0.tar` & `cloudreve-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 17:40:53.594403 cloudreve-1.0.0/
--rw-rw-rw-   0        0        0    35823 2024-04-30 15:03:13.000000 cloudreve-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1865 2024-04-30 17:40:53.594403 cloudreve-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      991 2024-04-30 17:30:16.000000 cloudreve-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-30 17:40:53.594403 cloudreve-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1308 2024-04-30 17:37:11.000000 cloudreve-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 17:40:53.566362 cloudreve-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 17:40:53.576888 cloudreve-1.0.0/src/cloudreve/
--rw-rw-rw-   0        0        0       28 2024-04-30 17:10:56.000000 cloudreve-1.0.0/src/cloudreve/__init__.py
--rw-rw-rw-   0        0        0     8432 2024-04-30 17:30:38.000000 cloudreve-1.0.0/src/cloudreve/models.py
-drwxrwxrwx   0        0        0        0 2024-04-30 17:40:53.592403 cloudreve-1.0.0/src/cloudreve.egg-info/
--rw-rw-rw-   0        0        0     1865 2024-04-30 17:40:53.000000 cloudreve-1.0.0/src/cloudreve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-04-30 17:40:53.000000 cloudreve-1.0.0/src/cloudreve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 17:40:53.000000 cloudreve-1.0.0/src/cloudreve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-30 17:40:53.000000 cloudreve-1.0.0/src/cloudreve.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-30 17:40:53.000000 cloudreve-1.0.0/src/cloudreve.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 03:40:30.837207 cloudreve-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2024-04-30 15:03:13.000000 cloudreve-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1926 2024-05-01 03:40:30.836206 cloudreve-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1052 2024-05-01 03:26:50.000000 cloudreve-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 03:40:30.837207 cloudreve-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1308 2024-05-01 03:40:08.000000 cloudreve-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:40:30.794603 cloudreve-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 03:40:30.804602 cloudreve-1.0.1/src/cloudreve/
+-rw-rw-rw-   0        0        0       28 2024-04-30 17:10:56.000000 cloudreve-1.0.1/src/cloudreve/__init__.py
+-rw-rw-rw-   0        0        0    11459 2024-05-01 03:39:59.000000 cloudreve-1.0.1/src/cloudreve/models.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:40:30.832638 cloudreve-1.0.1/src/cloudreve.egg-info/
+-rw-rw-rw-   0        0        0     1926 2024-05-01 03:40:30.000000 cloudreve-1.0.1/src/cloudreve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-05-01 03:40:30.000000 cloudreve-1.0.1/src/cloudreve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 03:40:30.000000 cloudreve-1.0.1/src/cloudreve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-01 03:40:30.000000 cloudreve-1.0.1/src/cloudreve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-01 03:40:30.000000 cloudreve-1.0.1/src/cloudreve.egg-info/top_level.txt
```

### Comparing `cloudreve-1.0.0/LICENSE` & `cloudreve-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudreve-1.0.0/PKG-INFO` & `cloudreve-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudreve
-Version: 1.0.0
+Version: 1.0.1
 Summary: SDK for Cloudreve sites
 Home-page: https://github.com/yxzlwz/cloudreve-sdk
 Author: yxzlwz
 Author-email: yxzlwz@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,15 +30,15 @@
 
 ## 示例
 
 ```python
 from cloudreve import Cloudreve
 
 # 初始化
-conn = Cloudreve('https://cloud.yixiangzhilv.com')
+conn = Cloudreve('http://127.0.0.1:5212')
 
 # 登录
 conn.login('admin@cloudreve.org', '123456')
 
 # 获取文件ID
 file_id = conn.get_id('/hello.py')
 
@@ -59,14 +59,17 @@
 conn.copy('/hello.py', '/python')
 
 # 重命名文件
 conn.rename(file_id, 'world.py')
 
 # 移动文件
 conn.move('/world.py', '/python')
+
+# 上传文件
+conn.upload('/my_file_backup.py', 'D:/my_file.py')
 ```
 
 ## 联系我们
 
 - Email：yxzlwz@gmail.com
 - TG 群：https://t.me/+XW2ok10N8DExMDU1
```

### Comparing `cloudreve-1.0.0/README.md` & `cloudreve-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 ## 示例
 
 ```python
 from cloudreve import Cloudreve
 
 # 初始化
-conn = Cloudreve('https://cloud.yixiangzhilv.com')
+conn = Cloudreve('http://127.0.0.1:5212')
 
 # 登录
 conn.login('admin@cloudreve.org', '123456')
 
 # 获取文件ID
 file_id = conn.get_id('/hello.py')
 
@@ -36,13 +36,16 @@
 conn.copy('/hello.py', '/python')
 
 # 重命名文件
 conn.rename(file_id, 'world.py')
 
 # 移动文件
 conn.move('/world.py', '/python')
+
+# 上传文件
+conn.upload('/my_file_backup.py', 'D:/my_file.py')
 ```
 
 ## 联系我们
 
 - Email：yxzlwz@gmail.com
 - TG 群：https://t.me/+XW2ok10N8DExMDU1
```

### Comparing `cloudreve-1.0.0/setup.py` & `cloudreve-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as fh:
     readme = fh.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='cloudreve',
-    version='1.0.0',
+    version='1.0.1',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     include_package_data=True,
     license='GPLv3',
     description='SDK for Cloudreve sites',
     long_description=readme,
     long_description_content_type='text/markdown',
```

### Comparing `cloudreve-1.0.0/src/cloudreve/models.py` & `cloudreve-1.0.1/src/cloudreve/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from requests import Session
+from pathlib import Path
+
+from requests import Session, request
 from urllib.parse import quote_plus
 
 
 def generate_src(file_id, is_dir) -> dict:
     src = {
         'items': [],
         'dirs': [],
@@ -270,7 +272,87 @@
         创建文件夹
         @param dir_path: 文件夹路径
         '''
 
         dir_path = revise_file_path(dir_path)
 
         self.request('put', '/directory', json={'path': dir_path})
+
+    def upload_to_local(self, local_file: Path, sessionID, chunkSize, expires):
+        with open(local_file, 'rb') as file:
+            file_data = file.read()
+            self.request(
+                'post',
+                f'/file/upload/{sessionID}/0',
+                headers={
+                    'Content-Type': 'application/octet-stream',
+                },
+                data=file_data,
+            )
+
+    def upload_to_onedrive(self, local_file: Path, sessionID, chunkSize,
+                           expires, uploadURLs):
+        upload_url = uploadURLs[0]
+        file_size = local_file.stat().st_size
+        with open(local_file, 'rb') as file:
+            for i in range(0, file_size, chunkSize):
+                start = i
+                end = min(i + chunkSize, file_size) - 1
+                request(
+                    'put',
+                    upload_url,
+                    headers={
+                        'Content-Type': 'application/octet-stream',
+                        'Content-Range': f'bytes {start}-{end}/{file_size}',
+                    },
+                    data=file.read(chunkSize),
+                )
+        self.request('post', f'/callback/onedrive/finish/{sessionID}', json={})
+
+    def upload(self,
+               file_path,
+               local_file_path,
+               policy_id=None,
+               policy_type=None):
+        '''
+        上传文件通用方法
+        @param file_path: 文件目标路径
+        @param local_file_path: 本地文件路径
+        @param policy_id: 存储策略ID（可选）
+        @param policy_type: 存储策略类型（可选）
+        当且仅当存储策略ID和类型同时存在时参数生效，否则程序将通过list方法获取存储策略信息
+        '''
+
+        local_file = Path(local_file_path)
+        if not local_file.is_file():
+            raise FileNotFoundError(f'{local_file_path} is not a file')
+
+        dir = file_path[:file_path.rfind('/')] or '/'
+        name = file_path[file_path.rfind('/') + 1:]
+
+        if not (policy_id and policy_type):
+            policy = self.list(dir)['policy']
+            policy_id, policy_type = policy['id'], policy['type']
+
+        body = {
+            'path': dir,
+            'name': name,
+            'size': local_file.stat().st_size,
+            'last_modified': int(local_file.stat().st_mtime * 1000),
+            'policy_id': policy_id,
+            'mime_type': '',
+        }
+
+        r = self.request('put', '/file/upload', json=body)
+
+        if policy_type == 'local':
+            return self.upload_to_local(
+                local_file=local_file,
+                **r,
+            )
+        elif policy_type == 'onedrive':
+            return self.upload_to_onedrive(
+                local_file=local_file,
+                **r,
+            )
+        else:
+            raise ValueError(f'Policy type {policy_type} is not currently supported')
```

### Comparing `cloudreve-1.0.0/src/cloudreve.egg-info/PKG-INFO` & `cloudreve-1.0.1/src/cloudreve.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudreve
-Version: 1.0.0
+Version: 1.0.1
 Summary: SDK for Cloudreve sites
 Home-page: https://github.com/yxzlwz/cloudreve-sdk
 Author: yxzlwz
 Author-email: yxzlwz@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,15 +30,15 @@
 
 ## 示例
 
 ```python
 from cloudreve import Cloudreve
 
 # 初始化
-conn = Cloudreve('https://cloud.yixiangzhilv.com')
+conn = Cloudreve('http://127.0.0.1:5212')
 
 # 登录
 conn.login('admin@cloudreve.org', '123456')
 
 # 获取文件ID
 file_id = conn.get_id('/hello.py')
 
@@ -59,14 +59,17 @@
 conn.copy('/hello.py', '/python')
 
 # 重命名文件
 conn.rename(file_id, 'world.py')
 
 # 移动文件
 conn.move('/world.py', '/python')
+
+# 上传文件
+conn.upload('/my_file_backup.py', 'D:/my_file.py')
 ```
 
 ## 联系我们
 
 - Email：yxzlwz@gmail.com
 - TG 群：https://t.me/+XW2ok10N8DExMDU1
```

