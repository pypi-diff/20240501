# Comparing `tmp/grugstream-0.0.8.tar.gz` & `tmp/grugstream-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grugstream-0.0.8.tar", max compression
+gzip compressed data, was "grugstream-0.0.9.tar", max compression
```

## Comparing `grugstream-0.0.8.tar` & `grugstream-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     8612 2023-10-25 22:55:50.584218 grugstream-0.0.8/README.md
--rw-r--r--   0        0        0       65 2023-10-25 22:55:50.584218 grugstream-0.0.8/grugstream/__init__.py
--rw-r--r--   0        0        0       90 2023-10-25 22:55:50.584218 grugstream-0.0.8/grugstream/acknowledgement.py
--rw-r--r--   0        0        0    55986 2023-10-25 22:55:50.584218 grugstream-0.0.8/grugstream/core.py
--rw-r--r--   0        0        0      339 2023-10-25 22:55:50.584218 grugstream-0.0.8/grugstream/exceptions.py
--rw-r--r--   0        0        0     2440 2023-10-25 22:55:50.584218 grugstream-0.0.8/grugstream/subscriber.py
--rw-r--r--   0        0        0     1862 2023-10-25 22:55:50.584218 grugstream-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     9465 1970-01-01 00:00:00.000000 grugstream-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     8612 2023-10-25 23:16:22.963672 grugstream-0.0.9/README.md
+-rw-r--r--   0        0        0       65 2023-10-25 23:16:22.963672 grugstream-0.0.9/grugstream/__init__.py
+-rw-r--r--   0        0        0       90 2023-10-25 23:16:22.967671 grugstream-0.0.9/grugstream/acknowledgement.py
+-rw-r--r--   0        0        0    58967 2023-10-25 23:16:22.967671 grugstream-0.0.9/grugstream/core.py
+-rw-r--r--   0        0        0      339 2023-10-25 23:16:22.967671 grugstream-0.0.9/grugstream/exceptions.py
+-rw-r--r--   0        0        0     2440 2023-10-25 23:16:22.967671 grugstream-0.0.9/grugstream/subscriber.py
+-rw-r--r--   0        0        0     1862 2023-10-25 23:16:22.967671 grugstream-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     9465 1970-01-01 00:00:00.000000 grugstream-0.0.9/PKG-INFO
```

### Comparing `grugstream-0.0.8/README.md` & `grugstream-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `grugstream-0.0.8/grugstream/core.py` & `grugstream-0.0.9/grugstream/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,57 @@
                         break
                     ack = await subscriber.on_next(item)
                 await subscriber.on_completed()
 
         return IterableObservable()
 
     @staticmethod
+    def from_iterable_thunk(thunk: Callable[[], Iterable[A]]) -> "Observable[A]":
+        """Create an Observable from a thunk that returns an iterable.
+        This is useful if you want to re-evaluate the iterable each time.
+        For example, generators can only be iterated once, so you can use this to
+        re-evaluate the generator each time.
+
+        Parameters
+        ----------
+        thunk : Callable
+            The iterable source to convert to an Observable
+
+        Returns
+        -------
+        Observable
+            An Observable emitting the values from the iterable
+
+        Examples
+        --------
+
+        def gen():
+            for i in range(3):
+                yield i
+
+        >>> obs = Observable.from_iterable_thunk(lambda: [1, 2, 3])
+        >>> await obs.to_list()
+        [1, 2, 3]
+        >>> await obs.to_list() # can be called multiple times, each time it will re-evaluate the thunk
+        [1, 2, 3]
+        """
+
+        class IterableObservable(Observable[A]):  # type: ignore
+            async def subscribe(self, subscriber: Subscriber[A]) -> None:
+                iterable_ = thunk()
+                ack = Acknowledgement.ok
+                for item in iterable_:
+                    if ack != Acknowledgement.ok:  # If not OK, then stop.
+                        break
+                    ack = await subscriber.on_next(item)
+                await subscriber.on_completed()
+
+        return IterableObservable()
+
+    @staticmethod
     def from_async_iterable(iterable: AsyncIterable[A]) -> "Observable[A]":
         """Create an Observable from an asynchronous iterable.
 
         Parameters
         ----------
         iterable : AsyncIterable
             The asynchronous iterable to convert to an Observable.
@@ -201,14 +244,55 @@
                     if ack != Acknowledgement.ok:
                         break
                     ack = await subscriber.on_next(item)
                 await subscriber.on_completed()
 
         return AsyncIterableObservable()
 
+    @staticmethod
+    def from_async_iterable_thunk(thunk: Callable[[], AsyncIterable[A]]) -> "Observable[A]":
+        """Create an Observable from a thunk that returns an iterable.
+        This is useful if you want to re-evaluate the iterable each time.
+        For example, generators can only be iterated once, so you can use this to
+        re-evaluate the generator each time.
+
+        Parameters
+        ----------
+        thunk : Callable
+            The asynchronous iterable to convert to an Observable.
+
+        Returns
+        -------
+        Observable
+            An Observable emitting values from the async iterable.
+
+        Examples
+        --------
+        >>> async def gen():
+        >>>     yield 1
+        >>>     yield 2
+        >>> obs = Observable.from_async_iterable_thunk(lambda: gen())
+        >>> await obs.to_list()
+        [1, 2]
+        >>> await obs.to_list() # can be called multiple times, each time it will re-evaluate the thunk
+        [1, 2]
+        """
+
+        class AsyncIterableObservable(Observable[A]):  # type: ignore
+            async def subscribe(self, subscriber: Subscriber[A]) -> None:
+                generator = thunk()
+                ack = Acknowledgement.ok
+                async for item in generator:
+                    if ack != Acknowledgement.ok:
+                        break
+                    ack = await subscriber.on_next(item)
+                await subscriber.on_completed()
+
+        return AsyncIterableObservable()
+
     @classmethod
     def from_receive_stream(cls, stream: MemoryObjectReceiveStream[A]) -> "Observable[A]":
         async def async_iterator() -> AsyncIterable[A]:
             async with stream:
                 async for item in stream:
                     yield item
 
@@ -237,15 +321,15 @@
 
         async def async_iterator() -> AsyncIterable[str]:
             async with await anyio.open_file(file_path) as f:
                 async for line in f:
                     line_without_newline = line.rstrip('\n')
                     yield line_without_newline
 
-        return Observable.from_async_iterable(async_iterator())
+        return Observable.from_async_iterable_thunk(lambda: async_iterator())
 
     @staticmethod
     def from_interval(seconds: float) -> 'Observable[int]':
         """Create an Observable emitting incremental numbers periodically.
 
         Emits an infinite sequence of incremental integers, with time
         period of `seconds` between each emission.
```

### Comparing `grugstream-0.0.8/grugstream/subscriber.py` & `grugstream-0.0.9/grugstream/subscriber.py`

 * *Files identical despite different names*

### Comparing `grugstream-0.0.8/pyproject.toml` & `grugstream-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "grugstream"
-version = "0.0.8"
+version = "0.0.9"
 homepage = "https://github.com/thejaminator/grugstream"
 description = "The grugstream library provides an easy way to work with asynchronous/ reactive / streaming programming."
 authors = ["James Chua <chuajamessh@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `grugstream-0.0.8/PKG-INFO` & `grugstream-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grugstream
-Version: 0.0.8
+Version: 0.0.9
 Summary: The grugstream library provides an easy way to work with asynchronous/ reactive / streaming programming.
 Home-page: https://github.com/thejaminator/grugstream
 License: MIT
 Author: James Chua
 Author-email: chuajamessh@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

