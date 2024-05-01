# Comparing `tmp/fastapi_user_limiter-0.2.0.tar.gz` & `tmp/fastapi_user_limiter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_user_limiter-0.2.0.tar", last modified: Tue Apr 30 13:04:11 2024, max compression
+gzip compressed data, was "fastapi_user_limiter-0.3.0.tar", last modified: Tue Apr 30 14:19:32 2024, max compression
```

## Comparing `fastapi_user_limiter-0.2.0.tar` & `fastapi_user_limiter-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:04:11.792475 fastapi_user_limiter-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-30 13:04:11.792475 fastapi_user_limiter-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-30 13:04:03.000000 fastapi_user_limiter-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 13:04:03.000000 fastapi_user_limiter-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:04:11.792475 fastapi_user_limiter-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:04:11.792475 fastapi_user_limiter-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:04:11.792475 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:04:03.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-30 13:04:03.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter/limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:04:11.792475 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-30 13:04:11.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-30 13:04:11.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:04:11.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 13:04:11.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 13:04:11.000000 fastapi_user_limiter-0.2.0/src/fastapi_user_limiter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:19:32.012859 fastapi_user_limiter-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-30 14:19:32.012859 fastapi_user_limiter-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-30 14:19:24.000000 fastapi_user_limiter-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 14:19:24.000000 fastapi_user_limiter-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:19:32.012859 fastapi_user_limiter-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:19:32.012859 fastapi_user_limiter-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:19:32.012859 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:19:24.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-30 14:19:24.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:19:32.012859 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-30 14:19:32.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-30 14:19:32.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:19:32.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 14:19:32.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 14:19:32.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/top_level.txt
```

### Comparing `fastapi_user_limiter-0.2.0/PKG-INFO` & `fastapi_user_limiter-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_limiter
-Version: 0.2.0
+Version: 0.3.0
 Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
 Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,53 +22,37 @@
 First install Redis, then install the package using:
 ```
 pip install fastapi-user-limiter
 ```
 
 ## Usage
 
-You can use the `rate_limit` decorator to put a single rate limit on an endpoint:
+You can use the `rate_limit` function as a FastAPI Dependency to add one or several rate limiters to an endpoint:
 
 ```python
-from fastapi_user_limiter.limiter import RateLimiter, rate_limit
-from fastapi import FastAPI, Request
+from fastapi_user_limiter.limiter import RateLimiterConnection, rate_limiter
+from fastapi import FastAPI, Depends
 
 app = FastAPI()
-rate_limiter = RateLimiter()
 
-# 2 requests max per 5 seconds
-@app.get("/single")
-@rate_limit(rate_limiter, 2, 5)
-async def read_single(request: Request):
-    return {"Hello": "World"}
-
-```
-
-To put multiple rate limits on the same endpoint (with different window size and maximum request counts), use the
-`multi_rate_limit` decorator. Each `multi_rate_limit` decorator on a particular endpoint requires an ID as its first arg.
-This ID must be unique among the `multi_rate_limit` decorators on that endpoint:
-
-```python
-from fastapi_user_limiter.limiter import RateLimiter, multi_rate_limit
-from fastapi import FastAPI, Request
 
-app = FastAPI()
-rate_limiter = RateLimiter()
+# Max 2 requests per 5 seconds
+@app.get("/single",
+         dependencies=[Depends(rate_limiter(RateLimiterConnection(), 2, 5))])
+async def read_single():
+    return {"Hello": "World"}
 
 
-# 1 request max per second, 3 requests max per 10 seconds
-@app.get("/multi")
-@multi_rate_limit(1, rate_limiter, 1, 1)
-@multi_rate_limit(2, rate_limiter, 3, 10)
-async def read_multi(request: Request):
-    return {"Hello": "There"}
+# Max 1 requests per second and max 3 requests per 10 seconds
+@app.get("/multi/{some_param}", dependencies=[
+    Depends(rate_limiter(RateLimiterConnection(), 1, 1)),
+    Depends(rate_limiter(RateLimiterConnection(), 3, 10))
+])
+async def read_multi(some_param: str):
+    return {"Hello": f"There {some_param}"}
 ```
 
-The aforementioned examples can be found in `example.py` (use ` uvicorn example:app --reload` to run).
-
-
-**NOTE**: Every endpoint handler with the rate limiter decorator needs to have `request` (of type `fastapi.Request`)
-as its first argument.
+The aforementioned examples and more can be found in `example.py` (use ` uvicorn example:app --reload` to run).
 
 ## Future features
 
 The package will soon have the additional feature of allowing each user account to have a different rate limit for each endpoint.
```

### Comparing `fastapi_user_limiter-0.2.0/README.md` & `fastapi_user_limiter-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -7,53 +7,37 @@
 First install Redis, then install the package using:
 ```
 pip install fastapi-user-limiter
 ```
 
 ## Usage
 
-You can use the `rate_limit` decorator to put a single rate limit on an endpoint:
+You can use the `rate_limit` function as a FastAPI Dependency to add one or several rate limiters to an endpoint:
 
 ```python
-from fastapi_user_limiter.limiter import RateLimiter, rate_limit
-from fastapi import FastAPI, Request
+from fastapi_user_limiter.limiter import RateLimiterConnection, rate_limiter
+from fastapi import FastAPI, Depends
 
 app = FastAPI()
-rate_limiter = RateLimiter()
 
-# 2 requests max per 5 seconds
-@app.get("/single")
-@rate_limit(rate_limiter, 2, 5)
-async def read_single(request: Request):
-    return {"Hello": "World"}
-
-```
-
-To put multiple rate limits on the same endpoint (with different window size and maximum request counts), use the
-`multi_rate_limit` decorator. Each `multi_rate_limit` decorator on a particular endpoint requires an ID as its first arg.
-This ID must be unique among the `multi_rate_limit` decorators on that endpoint:
-
-```python
-from fastapi_user_limiter.limiter import RateLimiter, multi_rate_limit
-from fastapi import FastAPI, Request
 
-app = FastAPI()
-rate_limiter = RateLimiter()
+# Max 2 requests per 5 seconds
+@app.get("/single",
+         dependencies=[Depends(rate_limiter(RateLimiterConnection(), 2, 5))])
+async def read_single():
+    return {"Hello": "World"}
 
 
-# 1 request max per second, 3 requests max per 10 seconds
-@app.get("/multi")
-@multi_rate_limit(1, rate_limiter, 1, 1)
-@multi_rate_limit(2, rate_limiter, 3, 10)
-async def read_multi(request: Request):
-    return {"Hello": "There"}
+# Max 1 requests per second and max 3 requests per 10 seconds
+@app.get("/multi/{some_param}", dependencies=[
+    Depends(rate_limiter(RateLimiterConnection(), 1, 1)),
+    Depends(rate_limiter(RateLimiterConnection(), 3, 10))
+])
+async def read_multi(some_param: str):
+    return {"Hello": f"There {some_param}"}
 ```
 
-The aforementioned examples can be found in `example.py` (use ` uvicorn example:app --reload` to run).
-
-
-**NOTE**: Every endpoint handler with the rate limiter decorator needs to have `request` (of type `fastapi.Request`)
-as its first argument.
+The aforementioned examples and more can be found in `example.py` (use ` uvicorn example:app --reload` to run).
 
 ## Future features
 
 The package will soon have the additional feature of allowing each user account to have a different rate limit for each endpoint.
```

### Comparing `fastapi_user_limiter-0.2.0/pyproject.toml` & `fastapi_user_limiter-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastapi_user_limiter"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Ramtin Yazdanian", email="ramtin.yazdanian@epfl.ch" }
 ]
 description = "Rate-limiter for FastAPI with the possibility of user-based rate limits"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `fastapi_user_limiter-0.2.0/src/fastapi_user_limiter/limiter.py` & `fastapi_user_limiter-0.3.0/src/fastapi_user_limiter/limiter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import redis.asyncio as redis
 from fastapi import Request, HTTPException, status
 import time
-from functools import wraps
 import random
 
 
 DEFAULT_REDIS_URL = 'redis://localhost:6379/1'
 
 
-class RateLimiter:
+class RateLimiterConnection:
     def __init__(self, redis_url: str = None):
         if redis_url is None:
             redis_url = DEFAULT_REDIS_URL
         self.redis_url = redis_url
         self.redis = None
 
     async def init_redis(self):
@@ -61,35 +60,16 @@
 
 
 def get_rate_limited_message(max_requests, window):
     return (f"Too many requests, no more than {max_requests} requests "
             f"are allowed every {window} seconds.")
 
 
-def rate_limit(rate_limiter: RateLimiter, max_requests: int, window: int):
-    def decorator(func):
-        @wraps(func)
-        async def wrapper(request: Request, *args, **kwargs):
-            key = f"rate_limit:{request.client.host}:{request.url.path}"
-            if await rate_limiter.is_rate_limited(key, max_requests, window):
-                raise HTTPException(
-                    status_code=status.HTTP_429_TOO_MANY_REQUESTS,
-                    detail=get_rate_limited_message(max_requests, window)
-                )
-            return await func(request, *args, **kwargs)
-        return wrapper
-    return decorator
-
-
-def multi_rate_limit(limiter_id: int, rate_limiter: RateLimiter, max_requests: int, window: int):
-    def decorator(func):
-        @wraps(func)
-        async def wrapper(request: Request, *args, **kwargs):
-            key = f"rate_limit:{request.client.host}:{request.url.path}:{limiter_id}"
-            if await rate_limiter.is_rate_limited(key, max_requests, window):
-                raise HTTPException(
-                    status_code=status.HTTP_429_TOO_MANY_REQUESTS,
-                    detail=get_rate_limited_message(max_requests, window)
-                )
-            return await func(request, *args, **kwargs)
-        return wrapper
-    return decorator
+def rate_limiter(rl: RateLimiterConnection, max_requests: int, window: int):
+    async def _rate_limit(request: Request):
+        key = f"rate_limit:{request.url.path}:{window}:{max_requests}:{request.client.host}"
+        if await rl.is_rate_limited(key, max_requests, window):
+            raise HTTPException(
+                status_code=status.HTTP_429_TOO_MANY_REQUESTS,
+                detail=get_rate_limited_message(max_requests, window)
+            )
+    return _rate_limit
```

### Comparing `fastapi_user_limiter-0.2.0/src/fastapi_user_limiter.egg-info/PKG-INFO` & `fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_limiter
-Version: 0.2.0
+Version: 0.3.0
 Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
 Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,53 +22,37 @@
 First install Redis, then install the package using:
 ```
 pip install fastapi-user-limiter
 ```
 
 ## Usage
 
-You can use the `rate_limit` decorator to put a single rate limit on an endpoint:
+You can use the `rate_limit` function as a FastAPI Dependency to add one or several rate limiters to an endpoint:
 
 ```python
-from fastapi_user_limiter.limiter import RateLimiter, rate_limit
-from fastapi import FastAPI, Request
+from fastapi_user_limiter.limiter import RateLimiterConnection, rate_limiter
+from fastapi import FastAPI, Depends
 
 app = FastAPI()
-rate_limiter = RateLimiter()
 
-# 2 requests max per 5 seconds
-@app.get("/single")
-@rate_limit(rate_limiter, 2, 5)
-async def read_single(request: Request):
-    return {"Hello": "World"}
-
-```
-
-To put multiple rate limits on the same endpoint (with different window size and maximum request counts), use the
-`multi_rate_limit` decorator. Each `multi_rate_limit` decorator on a particular endpoint requires an ID as its first arg.
-This ID must be unique among the `multi_rate_limit` decorators on that endpoint:
-
-```python
-from fastapi_user_limiter.limiter import RateLimiter, multi_rate_limit
-from fastapi import FastAPI, Request
 
-app = FastAPI()
-rate_limiter = RateLimiter()
+# Max 2 requests per 5 seconds
+@app.get("/single",
+         dependencies=[Depends(rate_limiter(RateLimiterConnection(), 2, 5))])
+async def read_single():
+    return {"Hello": "World"}
 
 
-# 1 request max per second, 3 requests max per 10 seconds
-@app.get("/multi")
-@multi_rate_limit(1, rate_limiter, 1, 1)
-@multi_rate_limit(2, rate_limiter, 3, 10)
-async def read_multi(request: Request):
-    return {"Hello": "There"}
+# Max 1 requests per second and max 3 requests per 10 seconds
+@app.get("/multi/{some_param}", dependencies=[
+    Depends(rate_limiter(RateLimiterConnection(), 1, 1)),
+    Depends(rate_limiter(RateLimiterConnection(), 3, 10))
+])
+async def read_multi(some_param: str):
+    return {"Hello": f"There {some_param}"}
 ```
 
-The aforementioned examples can be found in `example.py` (use ` uvicorn example:app --reload` to run).
-
-
-**NOTE**: Every endpoint handler with the rate limiter decorator needs to have `request` (of type `fastapi.Request`)
-as its first argument.
+The aforementioned examples and more can be found in `example.py` (use ` uvicorn example:app --reload` to run).
 
 ## Future features
 
 The package will soon have the additional feature of allowing each user account to have a different rate limit for each endpoint.
```

