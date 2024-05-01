# Comparing `tmp/nearness-0.1.0.tar.gz` & `tmp/nearness-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nearness-0.1.0.tar", max compression
+gzip compressed data, was "nearness-0.1.1.tar", max compression
```

## Comparing `nearness-0.1.0.tar` & `nearness-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1075 2024-02-04 10:05:20.712579 nearness-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     7224 2024-02-04 10:05:20.712579 nearness-0.1.0/README.md
--rw-r--r--   0        0        0     7065 2024-02-04 10:05:20.716579 nearness-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2666 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/__init__.py
--rw-r--r--   0        0        0     4699 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_annoy.py
--rw-r--r--   0        0        0     4020 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_autofaiss.py
--rw-r--r--   0        0        0       78 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_base/__init__.py
--rw-r--r--   0        0        0     2107 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_base/_config.py
--rw-r--r--   0        0        0     1212 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_base/_experimental.py
--rw-r--r--   0        0        0    17943 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_base/_neighbors.py
--rw-r--r--   0        0        0     4325 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_faiss.py
--rw-r--r--   0        0        0     2297 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_hnsw.py
--rw-r--r--   0        0        0     4638 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_jax.py
--rw-r--r--   0        0        0     3767 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_numpy.py
--rw-r--r--   0        0        0     8060 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_scann.py
--rw-r--r--   0        0        0     2417 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_scipy.py
--rw-r--r--   0        0        0     2089 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_sklearn.py
--rw-r--r--   0        0        0     2884 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/_torch.py
--rw-r--r--   0        0        0        0 2024-02-04 10:05:20.716579 nearness-0.1.0/src/nearness/py.typed
--rw-r--r--   0        0        0     9544 1970-01-01 00:00:00.000000 nearness-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-01 17:32:34.246774 nearness-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     7224 2024-05-01 17:32:34.246774 nearness-0.1.1/README.md
+-rw-r--r--   0        0        0     7085 2024-05-01 17:32:34.250774 nearness-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2666 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/__init__.py
+-rw-r--r--   0        0        0     4700 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_annoy.py
+-rw-r--r--   0        0        0     4020 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_autofaiss.py
+-rw-r--r--   0        0        0       78 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_base/__init__.py
+-rw-r--r--   0        0        0     2107 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_base/_config.py
+-rw-r--r--   0        0        0     1212 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_base/_experimental.py
+-rw-r--r--   0        0        0    18596 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_base/_neighbors.py
+-rw-r--r--   0        0        0     3568 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_faiss.py
+-rw-r--r--   0        0        0     2297 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_hnsw.py
+-rw-r--r--   0        0        0     4638 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_jax.py
+-rw-r--r--   0        0        0     3767 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_numpy.py
+-rw-r--r--   0        0        0     8060 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_scann.py
+-rw-r--r--   0        0        0     2417 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_scipy.py
+-rw-r--r--   0        0        0     2089 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_sklearn.py
+-rw-r--r--   0        0        0     2884 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/_torch.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:32:34.250774 nearness-0.1.1/src/nearness/py.typed
+-rw-r--r--   0        0        0     9544 1970-01-01 00:00:00.000000 nearness-0.1.1/PKG-INFO
```

### Comparing `nearness-0.1.0/LICENSE.txt` & `nearness-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nearness-0.1.0/README.md` & `nearness-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nearness-0.1.0/pyproject.toml` & `nearness-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nearness"
-version = "0.1.0"
+version = "0.1.1"
 description = "An easy-to-use interface for (approximate) nearest neighbors algorithms."
 readme = "README.md"
 authors = ["David Muhr <muhrdavid+github@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/davnn/nearness"
 packages = [{ include = "nearness", from = "src" }]
 
@@ -62,26 +62,26 @@
 autofaiss = ["autofaiss", "faiss-cpu"]
 faiss = ["faiss-cpu"]
 torch = ["torch"]
 scann = ["scann"]
 jax = ["jax"]
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^8.0.0"
+pytest = "^8.2.0"
 pytest-html = "^4.1.1"
-hypothesis = "^6.97.5"
-coverage = "^7.4.1"
-pytest-cov = "^4.1.0"
-coverage-badge = "^1.1.0"
-ruff = "^0.2.0"
-pre-commit = "^3.6.0"
-black = "^24.1.1"
-pyright = "^1.1.349"
-bandit = "^1.7.7"
-safety = "^3.0.1"
+hypothesis = "^6.100.2"
+coverage = "^7.5.0"
+pytest-cov = "^5.0.0"
+coverage-badge = "^1.1.1"
+ruff = "^0.4.2"
+pre-commit = "^3.7.0"
+black = "^24.4.2"
+pyright = "^1.1.360"
+bandit = "^1.7.8"
+safety = "^3.1.0"
 notebook = "^7.0.4"
 pytest-benchmark = "^4.0.0"
 
 [[tool.poetry.source]]
 name = "torch-cpu"
 url = "https://download.pytorch.org/whl/cpu"
 priority = "explicit"
@@ -196,8 +196,8 @@
 branch = true
 
 [tool.coverage.paths]
 source = ["src/nearness"]
 
 [tool.coverage.report]
 show_missing = true
-exclude_lines = ["pragma: no cover", "@overload", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
+exclude_lines = ["pragma: no cover", "@overload", "@abstractmethod", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
```

### Comparing `nearness-0.1.0/src/nearness/__init__.py` & `nearness-0.1.1/src/nearness/__init__.py`

 * *Files identical despite different names*

### Comparing `nearness-0.1.0/src/nearness/_annoy.py` & `nearness-0.1.1/src/nearness/_annoy.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self._index: AnnoyIndex | None = None
 
         # mmap the raw annoy index
         if (path := self.parameters.load_index_path) is not None:
             index = AnnoyIndex(self.parameters.load_index_dim, self.parameters.metric)
             index.load(str(path))
             self._index = index
-            self.is_fitted = True
+            self.__fitted__ = True
 
     @overload
     def fit(self, data: Iterable[Real[NumpyArray, "d"]]) -> "AnnoyNeighbors": ...
 
     @overload
     def fit(self, data: Real[NumpyArray, "n d"]) -> "AnnoyNeighbors": ...
```

### Comparing `nearness-0.1.0/src/nearness/_autofaiss.py` & `nearness-0.1.1/src/nearness/_autofaiss.py`

 * *Files identical despite different names*

### Comparing `nearness-0.1.0/src/nearness/_base/_config.py` & `nearness-0.1.1/src/nearness/_base/_config.py`

 * *Files identical despite different names*

### Comparing `nearness-0.1.0/src/nearness/_base/_experimental.py` & `nearness-0.1.1/src/nearness/_base/_experimental.py`

 * *Files identical despite different names*

### Comparing `nearness-0.1.0/src/nearness/_base/_neighbors.py` & `nearness-0.1.1/src/nearness/_base/_neighbors.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,39 +83,49 @@
 
         # same for the parameters, we set the parameters before the call such that they are usable in ``__init__``
         thread_local.parameters = _create_parameter_class(parameters, kwargs)
         cls._parameters_ = thread_local.parameters  # type: ignore[reportUninitializedInstanceVariable]
         logger.info("Determined parameters as '%s'", cls._parameters_)
 
         # now we set all the relevant attributes on the ``instance``, as they should not be class-bound.
-        # order is important here as ``__wrap_fit_method`` and ``__wrap_check_method`` depend on the set attributes
+        # order is important here as ``_wrap_fit_method`` and ``_wrap_check_method`` depend on the set attributes
         obj = type.__call__(cls, **kwargs)
         obj._parameters_, obj._config_ = cls._parameters_, cls._config_  # noqa: SLF001
         # make sure that the wrapped methods are in sync when the config is changed after class instantiation
         obj._config_.register_callback(  # noqa: SLF001
             "methods_require_fit",
             partial(cls._check_callback, obj=obj),
         )
+        if not hasattr(obj, "__fitted__"):
+            msg = (
+                f"Instantiated {obj}, but missing the '__fitted__' attribute, which is automatically set to False in "
+                f"'NearestNeighbors.__init__', did you forget to call 'super().__init__()' in the '__init__' of "
+                f"{obj}? Assuming that '__fitted__' is 'False'."
+            )
+            warn(msg, stacklevel=1)
+            obj.__fitted__ = False
+        if not obj.__fitted__:
+            # __fitted__ might be true if the index is pre-loaded in the ``__init__``.
+            cls._wrap_check_method(obj)
         cls._wrap_fit_method(obj)
-        cls._wrap_check_method(obj)
         del cls._parameters_
         del cls._config_
         return obj
 
     def _check_callback(cls, _: Any, *, obj: "NearestNeighbors") -> None:
-        """A callback to refresh the ``__fitted__`` attributes when the 'methods_require_fit' attribute is set ."""
+        """A callback to refresh the ``__fitted__`` attributes when the 'methods_require_fit' attribute is updated."""
         if not obj.is_fitted:  # if the object is already fitted there is no need to wrap any methods
             cls._wrap_check_method(obj)
 
     def _wrap_fit_method(cls, obj: "NearestNeighbors") -> None:
-        """Wrap the ``fit`` method to ensure it sets the ``__fitted__`` attribute and unwraps the query methods.
+        """Wrap the ``fit`` method to ensure it sets ``is_fitted`` to ``True``, which unwraps the query method checks.
 
         This feels a bit like magic, but the alternatives would be to:
-        1. Add a decorator to every ``fit`` method that sets ``__fitted__``.
-        2. Set the ``__fitted__`` attribute on every ``fit``-like method and check for ``__fitted__`` everywhere.
+        1. Add a decorator to every ``fit`` method that sets ``is_fitted`` to ``True``.
+        2. Set ``is_fitted`` on every ``fit``-like method and check for ``is_fitted`` everywhere.
         """
         fit = obj.fit
 
         @wraps(fit)
         def wrapper(*args: Any, **kwargs: Any) -> Any:
             result = fit(*args, **kwargs)
             logger.debug("Called wrapped fit method with successful fit result, setting '__fitted__'.")
@@ -169,15 +179,15 @@
                 warn(msg, stacklevel=1)
 
     def _unwrap_check_method(cls, obj: "NearestNeighbors") -> None:
         """Unwrap all existing methods in ``methods_require_fit`` to disable the ``__fitted__`` check.
 
         This is just a performance optimization, it retrieves the original method and removes the implicitly
         generated function wrapper (decorator). It should be safe to unwrap the methods if ``__fitted__``
-        is only set in ``fit``, but unsafe when ``__fitted__`` is manually set to ``False`` after ``fit``.
+        is set in ``fit``, but unsafe when ``__fitted__`` is manually set to ``False`` after ``fit``.
         """
         logger.debug("Starting to unwrap all fit checking methods.")
         for method_name in obj._config_.methods_require_fit:  # noqa: SLF001
             # we set an __requires_fit__ attribute on the wrapper, because using ``__wrapped__`` alone is not
             # safe (methods also use ``__wrapped__`` starting with Python 3.10)
             if hasattr(obj, method_name) and hasattr(method := getattr(obj, method_name), "__check__"):
                 logger.debug("Unwrapping method '%s'.", method_name)
@@ -193,15 +203,17 @@
 
     The default interface to all methods is based on NumPy N-dimensional arrays, but implementations might ``overload``
     the methods such that other data types can be implemented. An important consideration for all possible methods
     and overloads is that they should be type stable, preferably allowing only floating-point arrays as input
     and returning floating-point distances of equal type as output.
     """
 
-    __fitted__ = False
+    def __init__(self) -> None:
+        super().__init__()
+        self.__fitted__ = False
 
     @abstractmethod
     def fit(self, data: np.ndarray) -> Self:
         """Learn an index structure based on a matrix of points.
 
         :param data: matrix of ``size x dim``.
         :return: reference to object (``self``).
@@ -341,14 +353,15 @@
     def is_fitted(self, value: bool) -> None:
         if value:
             NearestNeighbors._unwrap_check_method(self)
 
         if not value:
             NearestNeighbors._wrap_check_method(self)
 
+        # this variable is initialized in the metaclass
         self.__fitted__ = value
 
     @property
     def config(self) -> "Config":
         return self._config_
 
     @property
@@ -363,15 +376,15 @@
 def _create_parameter_class(
     parameters: dict[str, inspect.Parameter],
     kwargs: dict[str, Any],
 ) -> "types.Parameters":  # type: ignore[reportGeneralTypeIssues]
     empty = inspect.Parameter.empty
     parameter_types = [(k, Any if (a := v.annotation) is empty else a) for k, v in parameters.items()]
     parameter_values = {k: kwargs.get(k, v.default) for k, v in parameters.items()}
-    return make_dataclass("Parameters", parameter_types)(**parameter_values)  # type: ignore[reportArgumentType]
+    return make_dataclass("Parameters", parameter_types)(**parameter_values)
 
 
 def _create_check_wrapper(obj: NearestNeighbors, method: Callable[..., Any]) -> Callable[..., Any]:
     @wraps(method)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
         logger.debug("Called method with fit check enabled.")
         if not obj.is_fitted:
```

### Comparing `nearness-0.1.0/src/nearness/_faiss.py` & `nearness-0.1.1/src/nearness/_faiss.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import faiss
-import numpy as np
 from safecheck import Float, Float32, Int64, NumpyArray, typecheck
-from typing_extensions import Any, Protocol, runtime_checkable
+from typing_extensions import Protocol, runtime_checkable
 
 from ._base import NearestNeighbors
 
 
 @runtime_checkable
 class FaissIndexFactory(Protocol):
     def __call__(self, dim: int) -> faiss.Index: ...
@@ -38,37 +37,24 @@
 
     @typecheck
     def __init__(
         self,
         *,
         index_or_factory: str | FaissIndexFactory | faiss.Index = "Flat",
         add_data_on_fit: bool = True,
-        sample_train_points: int | float | None = None,
-        sample_with_replacement: bool = False,
-        rng: Any = None,  # types are validated by default_rng
     ) -> None:
         super().__init__()
-        self.parameters.rng = rng if isinstance(rng, np.random.Generator) else np.random.default_rng(rng)
-
         # to be defined in ``fit``
         self._index: faiss.Index | None = None
 
     @typecheck
     def fit(self, data: Float[NumpyArray, "n d"]) -> "FaissNeighbors":
-        n_samples, dim = data.shape
+        _, dim = data.shape
         self._index = self._create_index(dim)
-        if (n_train := self.parameters.sample_train_points) is not None:
-            if isinstance(n_train, float):
-                # we make sure float is 0 < float < 1 in ``__init__``
-                n_train = int(n_train * n_samples)
-
-            sample = self.parameters.rng.choice(data, size=n_train, replace=self.parameters.sample_with_replacement)
-            self._index.train(sample)  # type: ignore[reportGeneralTypeIssues]
-        else:
-            self._index.train(data)  # type: ignore[reportGeneralTypeIssues]
+        self._index.train(data)  # type: ignore[reportGeneralTypeIssues]
 
         if self.parameters.add_data_on_fit:
             # data might be added directly on fit, or using the ``add`` method
             self._index.add(data)  # type: ignore[reportGeneralTypeIssues]
 
         return self
```

### Comparing `nearness-0.1.0/src/nearness/_hnsw.py` & `nearness-0.1.1/src/nearness/_hnsw.py`

 * *Files identical despite different names*

### Comparing `nearness-0.1.0/src/nearness/_jax.py` & `nearness-0.1.1/src/nearness/_jax.py`

 * *Files identical despite different names*

### Comparing `nearness-0.1.0/src/nearness/_numpy.py` & `nearness-0.1.1/src/nearness/_numpy.py`

 * *Files identical despite different names*

### Comparing `nearness-0.1.0/src/nearness/_scann.py` & `nearness-0.1.1/src/nearness/_scann.py`

 * *Files identical despite different names*

### Comparing `nearness-0.1.0/src/nearness/_scipy.py` & `nearness-0.1.1/src/nearness/_scipy.py`

 * *Files identical despite different names*

### Comparing `nearness-0.1.0/src/nearness/_sklearn.py` & `nearness-0.1.1/src/nearness/_sklearn.py`

 * *Files identical despite different names*

### Comparing `nearness-0.1.0/src/nearness/_torch.py` & `nearness-0.1.1/src/nearness/_torch.py`

 * *Files identical despite different names*

### Comparing `nearness-0.1.0/PKG-INFO` & `nearness-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nearness
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy-to-use interface for (approximate) nearest neighbors algorithms.
 Home-page: https://github.com/davnn/nearness
 License: MIT
 Author: David Muhr
 Author-email: muhrdavid+github@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 3 - Alpha
```

