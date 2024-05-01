# Comparing `tmp/django_environment_config-0.0.5.tar.gz` & `tmp/django_environment_config-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_environment_config-0.0.5.tar", max compression
+gzip compressed data, was "django_environment_config-0.1.0.tar", max compression
```

## Comparing `django_environment_config-0.0.5.tar` & `django_environment_config-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2705 2024-04-30 07:17:18.348220 django_environment_config-0.0.5/LICENSE
--rw-r--r--   0        0        0     2148 2024-04-30 07:17:18.348220 django_environment_config-0.0.5/README.md
--rw-r--r--   0        0        0       64 2024-04-30 07:17:18.348220 django_environment_config-0.0.5/env_config/__init__.py
--rw-r--r--   0        0        0     4547 2024-04-30 07:17:18.348220 django_environment_config-0.0.5/env_config/base.py
--rw-r--r--   0        0        0      364 2024-04-30 07:17:18.348220 django_environment_config-0.0.5/env_config/constants.py
--rw-r--r--   0        0        0      901 2024-04-30 07:17:18.348220 django_environment_config-0.0.5/env_config/errors.py
--rw-r--r--   0        0        0        0 2024-04-30 07:17:18.348220 django_environment_config-0.0.5/env_config/py.typed
--rw-r--r--   0        0        0     1210 2024-04-30 07:17:18.348220 django_environment_config-0.0.5/env_config/typing.py
--rw-r--r--   0        0        0    11566 2024-04-30 07:17:18.348220 django_environment_config-0.0.5/env_config/values.py
--rw-r--r--   0        0        0        0 2024-04-30 07:17:18.348220 django_environment_config-0.0.5/env_config_pytest_plugin/__init__.py
--rw-r--r--   0        0        0      792 2024-04-30 07:17:18.348220 django_environment_config-0.0.5/env_config_pytest_plugin/hooks.py
--rw-r--r--   0        0        0     8728 2024-04-30 07:17:18.352220 django_environment_config-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3640 1970-01-01 00:00:00.000000 django_environment_config-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2889 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3152 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/README.md
+-rw-r--r--   0        0        0       64 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/__init__.py
+-rw-r--r--   0        0        0     4558 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/base.py
+-rw-r--r--   0        0        0      364 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/constants.py
+-rw-r--r--   0        0        0     1058 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/errors.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/py.typed
+-rw-r--r--   0        0        0     1210 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/typing.py
+-rw-r--r--   0        0        0    12049 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config/values.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config_pytest_plugin/__init__.py
+-rw-r--r--   0        0        0      792 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/env_config_pytest_plugin/hooks.py
+-rw-r--r--   0        0        0     8728 2024-05-01 15:47:36.879834 django_environment_config-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 django_environment_config-0.1.0/PKG-INFO
```

### Comparing `django_environment_config-0.0.5/LICENSE` & `django_environment_config-0.1.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -16,36 +16,43 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
----------------- Original Licence for `django-configurations` ----------------
+end of terms and conditions
 
-Copyright (c) 2012-2023, Jannis Leidel and other contributors.
-All rights reserved.
+The externally maintained libraries from which parts of the Software is derived
+are:
 
-Redistribution and use in source and binary forms, with or without modification,
-are permitted provided that the following conditions are met:
+- django-configurations, licensed as follows:
+    """
 
-    1. Redistributions of source code must retain the above copyright notice,
-       this list of conditions and the following disclaimer.
-
-    2. Redistributions in binary form must reproduce the above copyright
-       notice, this list of conditions and the following disclaimer in the
-       documentation and/or other materials provided with the distribution.
-
-    3. Neither the name of django-configurations nor the names of its
-       contributors may be used to endorse or promote products derived from
-       this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
-ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
-ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+    Copyright (c) 2012-2023, Jannis Leidel and other contributors.
+    All rights reserved.
+
+    Redistribution and use in source and binary forms, with or without modification,
+    are permitted provided that the following conditions are met:
+
+        1. Redistributions of source code must retain the above copyright notice,
+           this list of conditions and the following disclaimer.
+
+        2. Redistributions in binary form must reproduce the above copyright
+           notice, this list of conditions and the following disclaimer in the
+           documentation and/or other materials provided with the distribution.
+
+        3. Neither the name of django-configurations nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+
+    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+    ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+    WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+    DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
+    ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+    (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+    LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+    ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+    (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+    SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+  """
```

### Comparing `django_environment_config-0.0.5/README.md` & `django_environment_config-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -19,15 +19,44 @@
 
 **Source Code**: [https://github.com/MrThearMan/django-environment-config/](https://github.com/MrThearMan/django-environment-config/)
 
 **Contributing**: [https://github.com/MrThearMan/django-environment-config/blob/main/CONTRIBUTING.md](https://github.com/MrThearMan/django-environment-config/blob/main/CONTRIBUTING.md)
 
 ---
 
-Configure django settings for multiple environments.
+Inspired by [django-configurations], this library aims to provide a simple way to configure
+settings for different environments in Django applications. For example, you might want to
+have different settings for local development compared to production, and different still when
+running automated tests or in checks in you CI.
+
+## Overview
+
+Environments are defined with a simple class-based configuration in the `settings.py` module.
+
+```python
+from env_config import Environment, values
+
+class Example(Environment):
+    DEBUG = True
+    SECRET_KEY = values.StringValue()
+    ALLOWED_HOSTS = values.ListValue(default=["*"])
+    DATABASES = values.DatabaseURLValue()
+```
+
+The Environment must be selected by setting the `DJANGO_SETTINGS_ENVIRONMENT`
+environment variable to the name of the class.
+
+```shell
+DJANGO_SETTINGS_ENVIRONMENT=Example python manage.py runserver
+```
+
+Check out the [docs] for more information.
+
+[django-configurations]: https://github.com/jazzband/django-configurations
+[docs]: https://mrthearman.github.io/django-environment-config/
 
 [coverage-badge]: https://coveralls.io/repos/github/MrThearMan/django-environment-config/badge.svg?branch=main
 [status-badge]: https://img.shields.io/github/actions/workflow/status/MrThearMan/django-environment-config/test.yml?branch=main
 [pypi-badge]: https://img.shields.io/pypi/v/django-environment-config
 [licence-badge]: https://img.shields.io/github/license/MrThearMan/django-environment-config
 [repo-badge]: https://img.shields.io/github/last-commit/MrThearMan/django-environment-config
 [issues-badge]: https://img.shields.io/github/issues-raw/MrThearMan/django-environment-config
```

### Comparing `django_environment_config-0.0.5/env_config/base.py` & `django_environment_config-0.1.0/env_config/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,35 +36,35 @@
         *,
         dotenv_path: StrPath | None | Undefined = Undefined,
         use_environ: bool = False,
     ) -> None:
         """
         When a subclass of environment is created, try to immediately load the settings
         and set them in the module globals where the environment is defined, if the environment matches
-        what has been selected in the `DJANGO_SETTINGS_ENVIRONMENT` environment variable.
+        what has been selected with the `DJANGO_SETTINGS_ENVIRONMENT` environment variable.
 
         :param dotenv_path: The path to the `.env` file to load. If set to `None`, the `.env` file will not be loaded.
                             By default, `python-dotenv` will try to find the `.env` file automatically.
         :param use_environ: If set to `True`, use environment variables instead of using a `.env` file.
         """
         env: str | None = os.environ.get(ENV_NAME)
         if env is None:  # pragma: no cover
             msg = f"Environment variable {ENV_NAME!r} must be set before subclassing 'Environment'"
             raise ValueError(msg)
 
-        # If the environment does not match, do not load environment or even the `.env` file.
-        if cls.__name__ != env:
+        # If the environment does not match, do not load the environment or even the `.env` file.
+        if cls.__name__.casefold() != env.casefold():
             return
 
         # If set to `None` explicitly, or using environment, do not load a `.env` file.
         if dotenv_path is None or use_environ:
             dotenv_path = Undefined
 
-        # If not given, set it to `None` so that `python-dotenv` will use
-        # `dotenv.main.find_dotenv` to find the `.env` file automatically.
+        # If not given, set it to `None` so the `dotenv.main.find_dotenv`
+        # will try to find the `.env` file automatically.
         elif dotenv_path is Undefined:
             dotenv_path = None
 
         dotenv: dict[str, str] | Undefined
         if use_environ:
             dotenv = os.environ.copy()
         elif dotenv_path is not Undefined:
@@ -97,16 +97,16 @@
         """
 
     @classmethod
     def setup(cls, *, stack_level: int = 1) -> None:
         """Load settings and set them in the module globals where the environment is defined."""
         settings = cls.load_settings()
         stack = inspect.stack()
-        caller_globals: dict[str, Any] = stack[stack_level].frame.f_globals
-        caller_globals.update(**settings)
+        module_globals: dict[str, Any] = stack[stack_level].frame.f_globals
+        module_globals.update(**settings)
 
     @classmethod
     def post_setup(cls) -> None:
         """Hook for doing additional setup after the settings have been loaded."""
 
     @classmethod
     def load_settings(cls) -> dict[str, Any]:
```

### Comparing `django_environment_config-0.0.5/env_config/errors.py` & `django_environment_config-0.1.0/env_config/errors.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 if TYPE_CHECKING:
     from env_config import Environment
 
 
 __all__ = [
     "DjangoEnvConfigError",
     "MissingEnvValueError",
+    "MissingExtraDependencyError",
 ]
 
 
 class DjangoEnvConfigError(Exception):
     """Base class for all Django Environment Config errors."""
 
 
@@ -25,7 +26,11 @@
         msg = f"Value {name!r} in environment {env.__name__!r}"
         if env.dotenv_path is not Undefined:
             msg += " not defined in the .env file and value does not have a default"
         else:
             msg += " needs a default value since environment does not define a `dotenv_path`"
 
         super().__init__(msg)
+
+
+class MissingExtraDependencyError(DjangoEnvConfigError):
+    """Base class for all Django Environment Config errors."""
```

### Comparing `django_environment_config-0.0.5/env_config/typing.py` & `django_environment_config-0.1.0/env_config/typing.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.0.5/env_config/values.py` & `django_environment_config-0.1.0/env_config/values.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from decimal import Decimal
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from django.utils.module_loading import import_string
 
 from .constants import Undefined
-from .errors import MissingEnvValueError
+from .errors import MissingEnvValueError, MissingExtraDependencyError
 from .typing import Any, CacheConfig, DBConfig, DBConfigExtra, Generator, Generic, Mapping, Sequence, TypeVar, Unpack
 
 if TYPE_CHECKING:
     from .base import Environment
 
 
 __all__ = [
@@ -47,55 +47,52 @@
 
 
 class Value(ABC, Generic[T]):
     def __init__(
         self,
         *,
         default: T | None = Undefined,
-        env_name: str | Undefined = Undefined,
-        nullable: bool = False,
+        env_name: str | None | Undefined = Undefined,
     ) -> None:
         """
         Value descriptor for an environment variable.
 
         :param default: The default value to use if the environment variable is not set.
         :param env_name: The name of the environment variable to use. If not given, the name of the field is used.
+                         Set this to `None` to skip loading the value from the environment.
         """
         self.default: T | None = default
         self.name: str = env_name
-        self.nullable: bool = nullable
+        self.skip_env: bool = env_name is None
 
         # Use a map to store the value per environment so that we can have
         # different values for environments what inherit from each other.
         self.value_by_environment: dict[type[Environment], Any] = defaultdict(lambda: Undefined)
         super().__init__()
 
     def __set_name__(self, env: type[Environment], name: str) -> None:
         """Called after the owner Environment-class is created with this field as a class attribute."""
-        if self.name is Undefined:
+        if self.name in (Undefined, None):
             self.name = name
 
     def __get__(self, _: Environment | None, env: type[Environment]) -> T:
         """Called when accessing the field on the class or an instance of the class."""
         if self.value_by_environment[env] is not Undefined:
             return self.value_by_environment[env]
 
         self.value_by_environment[env] = self.get_for_environment(env)
         return self.value_by_environment[env]
 
     def get_for_environment(self, env: type[Environment]) -> T:
-        value = self.default if env.dotenv is Undefined else env.dotenv.get(self.name, self.default)
+        value = self.default if env.dotenv is Undefined or self.skip_env else env.dotenv.get(self.name, self.default)
         if value is Undefined:
             raise MissingEnvValueError(name=self.name, env=env)
 
         if value is None:
-            if self.nullable:
-                return None
-            msg = f"Value for {self.name!r} cannot be None"
-            raise ValueError(msg)
+            return None
 
         return self.convert(value)
 
     @abstractmethod
     def convert(self, value: str | T) -> T:  # pragma: no cover
         """Convert the given value into the proper representation."""
         raise NotImplementedError
@@ -160,26 +157,25 @@
 
     def convert(self, value: str) -> str:
         import_string(value)
         return value
 
 
 class SequenceValue(Value, ABC, Generic[T]):
-    def __init__(  # noqa: PLR0913
+    def __init__(
         self,
         child: Value[T] | None = None,
         *,
         default: Sequence[T] | None = Undefined,
         env_name: str | Undefined = Undefined,
-        nullable: bool = False,
         delimiter: str = ",",
     ) -> None:
         self.child = child or StringValue()
         self.delimiter = delimiter
-        super().__init__(default=default, env_name=env_name, nullable=nullable)
+        super().__init__(default=default, env_name=env_name)
 
     def iterate(self, value: str | Sequence[Any]) -> Generator[T, None, None]:
         seq = value.split(self.delimiter) if isinstance(value, str) else value
         for item in seq:
             if not item:
                 continue
 
@@ -210,22 +206,21 @@
 class MappingValue(Value, ABC, Generic[T]):
     def __init__(  # noqa: PLR0913
         self,
         child: Value[T] | None = None,
         *,
         default: Mapping[str, T] | None = Undefined,
         env_name: str | Undefined = Undefined,
-        nullable: bool = False,
         kv_delimiter: str = "=",
         item_delimiter: str = ";",
     ) -> None:
         self.child = child or StringValue()
         self.kv_delimiter = kv_delimiter
         self.item_delimiter = item_delimiter
-        super().__init__(default=default, env_name=env_name, nullable=nullable)
+        super().__init__(default=default, env_name=env_name)
 
     def iterate(self, value: str | Mapping[str, Any]) -> Generator[tuple[str, Any], None, None]:
         seq = value.split(self.item_delimiter) if isinstance(value, str) else value.items()
 
         for item in seq:
             if not item:
                 continue
@@ -291,19 +286,18 @@
     """Parses env variables into a string value, and validates that it matches the given regex."""
 
     def __init__(
         self,
         *,
         regex: str,
         default: str | None = Undefined,
-        nullable: bool = False,
         env_name: str | Undefined = Undefined,
     ) -> None:
         self.regex = regex
-        super().__init__(default=default, env_name=env_name, nullable=nullable)
+        super().__init__(default=default, env_name=env_name)
 
     def convert(self, value: str) -> str:
         from django.core.validators import RegexValidator
 
         RegexValidator(regex=self.regex)(value)
         return value
 
@@ -312,19 +306,18 @@
     """Parses env variable into a string value, and can optionally validate that the path exists."""
 
     def __init__(
         self,
         *,
         default: str | None = Undefined,
         env_name: str | Undefined = Undefined,
-        nullable: bool = False,
         check_exists: bool = True,
     ) -> None:
         self.check_exists = check_exists
-        super().__init__(default=default, env_name=env_name, nullable=nullable)
+        super().__init__(default=default, env_name=env_name)
 
     def convert(self, value: str) -> str:
         path = Path(value).absolute()
         if self.check_exists and not path.exists():
             msg = f"Path '{path}' does not exist"
             raise ValueError(msg)
 
@@ -346,15 +339,23 @@
         self.params = params
         super().__init__(default=default, env_name=env_name)
 
     def convert(self, value: str | DBConfig) -> dict[str, DBConfig]:
         if not isinstance(value, str):
             return {self.db_alias: value}
 
-        from dj_database_url import parse
+        try:
+            from dj_database_url import parse
+        except ImportError as error:  # pragma: no cover
+            msg = (
+                "You must install the 'db' extra dependency "
+                "(e.g., `pip install django-environment-config[db]`) "
+                "to use the DatabaseURLValue."
+            )
+            raise MissingExtraDependencyError(msg) from error
 
         config = parse(value, **self.params)
         return {self.db_alias: config}
 
 
 class CacheURLValue(Value[CacheConfig | str]):
     """Load a cache configuration from a URL."""
@@ -369,11 +370,19 @@
         self.cache_alias = cache_alias
         super().__init__(default=default, env_name=env_name)
 
     def convert(self, value: str | CacheConfig) -> dict[str, CacheConfig]:
         if not isinstance(value, str):
             return {self.cache_alias: value}
 
-        from django_cache_url import parse
+        try:
+            from django_cache_url import parse
+        except ImportError as error:  # pragma: no cover
+            msg = (
+                "You must install the 'cache' extra dependency "
+                "(e.g., `pip install django-environment-config[cache]`) "
+                "to use the CacheURLValue."
+            )
+            raise MissingExtraDependencyError(msg) from error
 
         config = parse(value)
         return {self.cache_alias: config}
```

### Comparing `django_environment_config-0.0.5/env_config_pytest_plugin/hooks.py` & `django_environment_config-0.1.0/env_config_pytest_plugin/hooks.py`

 * *Files identical despite different names*

### Comparing `django_environment_config-0.0.5/pyproject.toml` & `django_environment_config-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-environment-config"
-version = "0.0.5"
+version = "0.1.0"
 description = "Configure django settings for multiple environments."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "env_config" },
     { include = "env_config_pytest_plugin" },
```

