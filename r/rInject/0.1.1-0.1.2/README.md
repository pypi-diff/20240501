# Comparing `tmp/rInject-0.1.1.tar.gz` & `tmp/rinject-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rInject-0.1.1.tar", last modified: Sun Jul 19 13:43:46 2020, max compression
+gzip compressed data, was "rinject-0.1.2.tar", last modified: Wed May  1 07:03:43 2024, max compression
```

## Comparing `rInject-0.1.1.tar` & `rinject-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 stevemccartney   (501) staff       (20)        0 2020-07-19 13:43:46.951731 rInject-0.1.1/
--rw-r--r--   0 stevemccartney   (501) staff       (20)     1902 2020-07-19 13:43:46.950026 rInject-0.1.1/PKG-INFO
--rw-r--r--   0 stevemccartney   (501) staff       (20)      912 2020-07-12 20:44:48.000000 rInject-0.1.1/README.md
-drwxr-xr-x   0 stevemccartney   (501) staff       (20)        0 2020-07-19 13:43:46.943357 rInject-0.1.1/rInject.egg-info/
--rw-r--r--   0 stevemccartney   (501) staff       (20)     1902 2020-07-19 13:43:46.000000 rInject-0.1.1/rInject.egg-info/PKG-INFO
--rw-r--r--   0 stevemccartney   (501) staff       (20)      192 2020-07-19 13:43:46.000000 rInject-0.1.1/rInject.egg-info/SOURCES.txt
--rw-r--r--   0 stevemccartney   (501) staff       (20)        1 2020-07-19 13:43:46.000000 rInject-0.1.1/rInject.egg-info/dependency_links.txt
--rw-r--r--   0 stevemccartney   (501) staff       (20)       14 2020-07-19 13:43:46.000000 rInject-0.1.1/rInject.egg-info/requires.txt
--rw-r--r--   0 stevemccartney   (501) staff       (20)        8 2020-07-19 13:43:46.000000 rInject-0.1.1/rInject.egg-info/top_level.txt
-drwxr-xr-x   0 stevemccartney   (501) staff       (20)        0 2020-07-19 13:43:46.945500 rInject-0.1.1/rinject/
--rw-r--r--   0 stevemccartney   (501) staff       (20)     5007 2020-07-19 13:39:40.000000 rInject-0.1.1/rinject/__init__.py
--rw-r--r--   0 stevemccartney   (501) staff       (20)       38 2020-07-19 13:43:46.952210 rInject-0.1.1/setup.cfg
--rw-r--r--   0 stevemccartney   (501) staff       (20)      891 2020-07-19 13:40:30.000000 rInject-0.1.1/setup.py
+drwxr-xr-x   0 stevemccartney   (501) staff       (20)        0 2024-05-01 07:03:43.609767 rinject-0.1.2/
+-rw-r--r--   0 stevemccartney   (501) staff       (20)      552 2024-05-01 07:00:35.000000 rinject-0.1.2/LICENSE
+-rw-r--r--   0 stevemccartney   (501) staff       (20)     1529 2024-05-01 07:03:43.609493 rinject-0.1.2/PKG-INFO
+-rw-r--r--   0 stevemccartney   (501) staff       (20)      912 2024-05-01 07:00:35.000000 rinject-0.1.2/README.md
+drwxr-xr-x   0 stevemccartney   (501) staff       (20)        0 2024-05-01 07:03:43.609081 rinject-0.1.2/rInject.egg-info/
+-rw-r--r--   0 stevemccartney   (501) staff       (20)     1529 2024-05-01 07:03:43.000000 rinject-0.1.2/rInject.egg-info/PKG-INFO
+-rw-r--r--   0 stevemccartney   (501) staff       (20)      223 2024-05-01 07:03:43.000000 rinject-0.1.2/rInject.egg-info/SOURCES.txt
+-rw-r--r--   0 stevemccartney   (501) staff       (20)        1 2024-05-01 07:03:43.000000 rinject-0.1.2/rInject.egg-info/dependency_links.txt
+-rw-r--r--   0 stevemccartney   (501) staff       (20)       14 2024-05-01 07:03:43.000000 rinject-0.1.2/rInject.egg-info/requires.txt
+-rw-r--r--   0 stevemccartney   (501) staff       (20)        8 2024-05-01 07:03:43.000000 rinject-0.1.2/rInject.egg-info/top_level.txt
+drwxr-xr-x   0 stevemccartney   (501) staff       (20)        0 2024-05-01 07:03:43.608408 rinject-0.1.2/rinject/
+-rw-r--r--   0 stevemccartney   (501) staff       (20)     5007 2024-05-01 07:00:35.000000 rinject-0.1.2/rinject/__init__.py
+-rw-r--r--   0 stevemccartney   (501) staff       (20)       38 2024-05-01 07:03:43.609823 rinject-0.1.2/setup.cfg
+-rw-r--r--   0 stevemccartney   (501) staff       (20)      889 2024-05-01 07:01:03.000000 rinject-0.1.2/setup.py
+drwxr-xr-x   0 stevemccartney   (501) staff       (20)        0 2024-05-01 07:03:43.608721 rinject-0.1.2/tests/
+-rw-r--r--   0 stevemccartney   (501) staff       (20)     2893 2024-05-01 07:00:35.000000 rinject-0.1.2/tests/test_injector.py
```

### Comparing `rInject-0.1.1/PKG-INFO` & `rinject-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 Metadata-Version: 2.1
 Name: rInject
-Version: 0.1.1
+Version: 0.1.2
 Summary: A flexible (annotations or keys) but simple dependency injection library for Python 3.
 Home-page: https://github.com/stevemccartney/rinject
 Author: Steve McCartney
 Author-email: python@reconvergent.com
 License: Apache 2.0
-Description: # rInject
-        
-        A flexible (annotations or keys) but simple dependency injection library for Python 3.
-        
-        
-        ## Installation
-        
-        ```pip install rinject```
-        
-        
-        ## Usage
-        
-        ```python
-        from rinject import Injector
-        from datetime import datetime
-        
-        
-        injector = Injector()
-        
-        
-        class A:
-            def __init__(self, greeting: str):
-                self.greeting = greeting
-        
-            def __call__(self, name: str):
-                print(f"{self.greeting} {name}")
-        
-        
-        class B:
-            def __init__(self, a: A, name: str):
-                self.a = a
-                self.name = name
-        
-            def __call__(self):
-                self.a(self.name)
-        
-        
-        if __name__ == "__main__":
-            injector.register_value("greeting", "Hello")
-            injector.register_instance(A, A)
-            injector.register_instance(B, B)
-            injector.register_factory("name", lambda: "Steve@" + datetime.utcnow().isoformat())
-        
-            b = injector.resolve(B)
-            b()  # outputs => Hello Steve
-        
-            b2 = injector.resolve(B)
-            assert b is b2
-        ```
-        
-        
 Keywords: dependency injection inject injector di dic
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8.*
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+
+# rInject
+
+A flexible (annotations or keys) but simple dependency injection library for Python 3.
+
+
+## Installation
+
+```pip install rinject```
+
+
+## Usage
+
+```python
+from rinject import Injector
+from datetime import datetime
+
+
+injector = Injector()
+
+
+class A:
+    def __init__(self, greeting: str):
+        self.greeting = greeting
+
+    def __call__(self, name: str):
+        print(f"{self.greeting} {name}")
+
+
+class B:
+    def __init__(self, a: A, name: str):
+        self.a = a
+        self.name = name
+
+    def __call__(self):
+        self.a(self.name)
+
+
+if __name__ == "__main__":
+    injector.register_value("greeting", "Hello")
+    injector.register_instance(A, A)
+    injector.register_instance(B, B)
+    injector.register_factory("name", lambda: "Steve@" + datetime.utcnow().isoformat())
+
+    b = injector.resolve(B)
+    b()  # outputs => Hello Steve
+
+    b2 = injector.resolve(B)
+    assert b is b2
+```
+
```

### Comparing `rInject-0.1.1/README.md` & `rinject-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rInject-0.1.1/rInject.egg-info/PKG-INFO` & `rinject-0.1.2/rInject.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 Metadata-Version: 2.1
 Name: rInject
-Version: 0.1.1
+Version: 0.1.2
 Summary: A flexible (annotations or keys) but simple dependency injection library for Python 3.
 Home-page: https://github.com/stevemccartney/rinject
 Author: Steve McCartney
 Author-email: python@reconvergent.com
 License: Apache 2.0
-Description: # rInject
-        
-        A flexible (annotations or keys) but simple dependency injection library for Python 3.
-        
-        
-        ## Installation
-        
-        ```pip install rinject```
-        
-        
-        ## Usage
-        
-        ```python
-        from rinject import Injector
-        from datetime import datetime
-        
-        
-        injector = Injector()
-        
-        
-        class A:
-            def __init__(self, greeting: str):
-                self.greeting = greeting
-        
-            def __call__(self, name: str):
-                print(f"{self.greeting} {name}")
-        
-        
-        class B:
-            def __init__(self, a: A, name: str):
-                self.a = a
-                self.name = name
-        
-            def __call__(self):
-                self.a(self.name)
-        
-        
-        if __name__ == "__main__":
-            injector.register_value("greeting", "Hello")
-            injector.register_instance(A, A)
-            injector.register_instance(B, B)
-            injector.register_factory("name", lambda: "Steve@" + datetime.utcnow().isoformat())
-        
-            b = injector.resolve(B)
-            b()  # outputs => Hello Steve
-        
-            b2 = injector.resolve(B)
-            assert b is b2
-        ```
-        
-        
 Keywords: dependency injection inject injector di dic
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8.*
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+
+# rInject
+
+A flexible (annotations or keys) but simple dependency injection library for Python 3.
+
+
+## Installation
+
+```pip install rinject```
+
+
+## Usage
+
+```python
+from rinject import Injector
+from datetime import datetime
+
+
+injector = Injector()
+
+
+class A:
+    def __init__(self, greeting: str):
+        self.greeting = greeting
+
+    def __call__(self, name: str):
+        print(f"{self.greeting} {name}")
+
+
+class B:
+    def __init__(self, a: A, name: str):
+        self.a = a
+        self.name = name
+
+    def __call__(self):
+        self.a(self.name)
+
+
+if __name__ == "__main__":
+    injector.register_value("greeting", "Hello")
+    injector.register_instance(A, A)
+    injector.register_instance(B, B)
+    injector.register_factory("name", lambda: "Steve@" + datetime.utcnow().isoformat())
+
+    b = injector.resolve(B)
+    b()  # outputs => Hello Steve
+
+    b2 = injector.resolve(B)
+    assert b is b2
+```
+
```

### Comparing `rInject-0.1.1/rinject/__init__.py` & `rinject-0.1.2/rinject/__init__.py`

 * *Files identical despite different names*

### Comparing `rInject-0.1.1/setup.py` & `rinject-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     readme = f.read()
 
 setup(
     name="rInject",
     description="A flexible (annotations or keys) but simple dependency injection library for Python 3.",
     long_description=readme,
     long_description_content_type="text/markdown",
-    version="0.1.1",
+    version="0.1.2",
     author="Steve McCartney",
     author_email="python@reconvergent.com",
     url="https://github.com/stevemccartney/rinject",
     packages=["rinject"],
     include_package_data=True,
-    python_requires=">=3.8.*",
+    python_requires=">=3.8",
     extras_require={"dev": ["pytest"]},
     license="Apache 2.0",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.8",
     ],
```

