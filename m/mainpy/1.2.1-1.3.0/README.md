# Comparing `tmp/mainpy-1.2.1.tar.gz` & `tmp/mainpy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainpy-1.2.1.tar", max compression
+gzip compressed data, was "mainpy-1.3.0.tar", max compression
```

## Comparing `mainpy-1.2.1.tar` & `mainpy-1.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2022-03-15 19:48:00.774000 mainpy-1.2.1/LICENSE
--rw-r--r--   0        0        0     3984 2024-02-29 21:46:48.434408 mainpy-1.2.1/README.md
--rw-r--r--   0        0        0     3649 2024-02-29 21:32:01.225077 mainpy-1.2.1/mainpy/__init__.py
--rw-r--r--   0        0        0        0 2022-04-02 14:23:11.563699 mainpy-1.2.1/mainpy/py.typed
--rw-r--r--   0        0        0     6141 2024-02-29 21:48:52.361389 mainpy-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     5131 1970-01-01 00:00:00.000000 mainpy-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-03-15 19:48:00.774000 mainpy-1.3.0/LICENSE
+-rw-r--r--   0        0        0     4042 2024-05-01 16:21:35.772569 mainpy-1.3.0/README.md
+-rw-r--r--   0        0        0     4288 2024-05-01 16:21:35.772569 mainpy-1.3.0/mainpy/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-02 14:23:11.563699 mainpy-1.3.0/mainpy/py.typed
+-rw-r--r--   0        0        0     6650 2024-05-01 16:21:35.772569 mainpy-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5383 1970-01-01 00:00:00.000000 mainpy-1.3.0/PKG-INFO
```

### Comparing `mainpy-1.2.1/LICENSE` & `mainpy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mainpy-1.2.1/README.md` & `mainpy-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # `@main`.py
 
 -----
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/mainpy.svg)][PYPI]
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/mainpy.svg)][PYPI]
-[![PyPI license](https://img.shields.io/pypi/l/mainpy.svg)][PYPI]
-[![Actions status](https://github.com/jorenham/mainpy/workflows/CI/badge.svg)][CI]
-[![Pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)][PYRIGHT]
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)][RUFF]
+[![mainpy - pypi version](https://img.shields.io/pypi/v/mainpy.svg)][PYPI]
+[![mainpy - python versions](https://img.shields.io/pypi/pyversions/mainpy.svg)][PYPI]
+[![mainpy - license](https://img.shields.io/pypi/l/mainpy.svg)][PYPI]
+[![mainpy - workflow status](https://github.com/jorenham/mainpy/workflows/CI/badge.svg)][CI]
+[![mainpy - basedpyright](https://img.shields.io/badge/basedpyright-checked-42b983)][BASEDPYRIGHT]
+[![mainpy - ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)][RUFF]
 
 -----
 
 ## Basic Examples
 
 Instead of the verbose "boilerplate"
 
@@ -59,15 +59,14 @@
 def async_app(): ...
 
 # do things before running async_app()
 
 main(async_app)
 ```
 
-
 ## External Libraries
 
 Even though `mainpy` requires no other dependencies than `typing_extensions`
 (on Python < 3.10), it has optional support for [`uvloop`][UVLOOP], and plays
 nicely with popular CLI libraries, e.g. [`click`][CLICK] and [`typer`][TYPER].
 
 ### `uvloop`
@@ -162,15 +161,15 @@
 
 ```shell
 pip install mainpy[uvloop]
 ```
 
 [PYPI]: https://pypi.org/project/mainpy/
 [CI]: https://github.com/jorenham/mainpy/actions
-[PYRIGHT]: https://microsoft.github.io/pyright/
+[BASEDPYRIGHT]: https://detachhead.github.io/basedpyright/
 [RUFF]: https://github.com/astral-sh/ruff
 [UVLOOP]: https://github.com/MagicStack/uvloop
 [CLICK]: https://github.com/pallets/click
 [TYPER]: https://github.com/tiangolo/typer
 [DEVMODE]: https://docs.python.org/3/library/devmode.html
 [FAULTHANDLER]: https://docs.python.org/3/library/faulthandler.html
 [WARNINGS]: https://docs.python.org/3/library/warnings.html
```

### Comparing `mainpy-1.2.1/mainpy/__init__.py` & `mainpy-1.3.0/mainpy/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,41 @@
 from __future__ import annotations
 
 import asyncio
-import functools
-import importlib.util
 import inspect
 import os
 import sys
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Coroutine,
     Protocol,
     TypeVar,
     cast,
+    final,
     overload,
 )
 
 
 if TYPE_CHECKING:
     import contextvars
 
-
-if sys.version_info < (3, 10):
-    from typing_extensions import TypeAlias
+if sys.version_info < (3, 11):
+    from typing_extensions import Never, TypeAlias
 else:
-    from typing import TypeAlias
+    from typing import Never, TypeAlias
 
 __all__ = ('main',)
 
-
 _R = TypeVar('_R')
-_F = TypeVar('_F', bound=Callable[..., Any])
+_F = TypeVar('_F', bound=Callable[[], Any])
 
 _SFunc: TypeAlias = Callable[[], _R]
-_AFunc: TypeAlias = _SFunc[Coroutine[Any, None, _R]]
-
-
-class _MainDecorator(Protocol):
-    @overload
-    def __call__(self, __f: _AFunc[_R], /) -> _R: ...
-    @overload
-    def __call__(self, __f: _SFunc[_R], /) -> _R: ...
+_AFunc: TypeAlias = Callable[[], Coroutine[Any, Any, _R]]
 
 
 def _infer_debug() -> bool:
     flags = sys.flags
 
     if flags.debug or flags.dev_mode:
         return True
@@ -53,118 +43,145 @@
     if '--debug' in sys.argv[1:]:
         return True
 
     env_debug = os.environ.get('DEBUG', '0')
     try:
         env_debug = int(env_debug)
     except ValueError as e:
-        raise OSError(
-            f'Invalid value for `DEBUG` env var: {env_debug!r}',
-        ) from e
+        errmsg = f'Invalid value for `DEBUG` env var: {env_debug!r}'
+        raise OSError(errmsg) from e
 
     return bool(env_debug)
 
 
 def _infer_uvloop() -> bool:
     """Check whether uvloop is installed."""
     if 'uvloop' in sys.modules:
         return True
 
+    import importlib.util
+
     return importlib.util.find_spec('uvloop') is not None
 
 
-def _enable_debug():
+def _enable_debug() -> None:
     """Enable debug mode."""
     env = os.environ
 
     if not env.get('PYTHONWARNINGS'):
         import warnings
 
         warnings.simplefilter('always')
 
     if not (env.get('PYTHONDEVMODE') or env.get('PYTHONFAULTHANDLER')):
         import faulthandler
 
         faulthandler.enable()
 
 
-@overload
-def main(__f: _AFunc[_R], /) -> _R | _AFunc[_R]: ...
-@overload
-def main(__f: _SFunc[_R], /) -> _R | _SFunc[_R]: ...
+@final
+class _MainDecorator(Protocol):
+    @overload
+    def __call__(self, func: _AFunc[_R]) -> _AFunc[_R] | _R: ...
+    @overload
+    def __call__(self, func: _SFunc[_R]) -> _SFunc[_R] | _R: ...
+
 
 @overload
 def main(
+    func: None = ...,
+    /,
     *,
     debug: bool | None = ...,
     is_async: bool | None = ...,
     use_uvloop: bool | None = ...,
     context: contextvars.Context | None = ...,
 ) -> _MainDecorator: ...
+@overload
+def main(
+    func: _AFunc[_R],
+    /,
+    *,
+    debug: bool | None = ...,
+    is_async: bool | None = ...,
+    use_uvloop: bool | None = ...,
+    context: contextvars.Context | None = ...,
+) -> _AFunc[_R] | _R: ...
+@overload
+def main(
+    func: _SFunc[_R],
+    /,
+    *,
+    debug: bool | None = ...,
+    is_async: bool | None = ...,
+    use_uvloop: bool | None = ...,
+    context: contextvars.Context | None = ...,
+) -> _SFunc[_R] | _R: ...
 
 
 def main(
-    func: _F | None = None,
+    func: _AFunc[_R] | _SFunc[_R] | None = None,
     /,
     *,
     debug: bool | None = None,
     is_async: bool | None = None,
     use_uvloop: bool | None = None,
     context: contextvars.Context | None = None,
-) -> _MainDecorator | _F | Any:
+) -> _MainDecorator | _AFunc[_R] | _SFunc[_R] | _R:
     """
     Decorate a function to be the main entrypoint.
     """
     if func is None:
-        return cast(
-            _MainDecorator,
-            functools.partial(
-                main,
+        def _main(_func: _F, /) -> _F | object:
+            return main(
+                _func,
                 debug=debug,
                 is_async=is_async,
                 use_uvloop=use_uvloop,
                 context=context,
-            ),
-        )
+            )
+
+        return cast(_MainDecorator, _main)
 
     if not callable(func):
-        raise TypeError(f'expected a callable, got {func!r}')
+        errmsg = f'expected a callable, got {type(func)}'
+        raise TypeError(errmsg)
 
     if func.__module__ != '__main__':
         frame = inspect.currentframe()
         if not frame or frame.f_globals.get('__name__') != '__main__':
             return func
 
-    if debug or debug is None and _infer_debug():
+    if debug or (debug is None and _infer_debug()):
         _enable_debug()
 
-    if (
-        is_async is False
-        or is_async is None and not asyncio.iscoroutinefunction(func)
+    if is_async is False or (
+        is_async is None
+        and not asyncio.iscoroutinefunction(func)
     ):
-        return func()
+        return cast(_R, func())
 
     if use_uvloop is None:
         use_uvloop = _infer_uvloop()
 
     if sys.version_info < (3, 11):
         if use_uvloop:
-            import uvloop
+            import uvloop  # pyright: ignore[reportMissingImports]
 
             uvloop.install()  # pyright: ignore[reportUnknownMemberType]
 
-        return asyncio.run(func(), debug=debug)
+        return asyncio.run(cast(Coroutine[Any, Any, _R], func()), debug=debug)
 
     loop_factory = None
     if use_uvloop:
         import uvloop
 
         loop_factory = uvloop.new_event_loop
 
     with asyncio.Runner(debug=debug, loop_factory=loop_factory) as runner:
         return runner.run(func(), context=context)
 
 
 @main
-def __main():
+def __main() -> Never:  # pyright: ignore[reportUnusedFunction]
     # this should never run
     raise AssertionError
```

### Comparing `mainpy-1.2.1/pyproject.toml` & `mainpy-1.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,128 +1,148 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "mainpy"
-version = "1.2.1"
+version = "1.3.0"
 description = "Simplify your project's main entrypoint definition with @main"
 authors = ["Joren Hammudoglu <jhammudoglu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jorenham/mainpy"
+documentation = "https://github.com/jorenham/mainpy?tab=readme-ov-file#mainpy"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Natural Language :: English",
-    "Topic :: Software Development",
-    "Topic :: Utilities",
+    "Operating System :: OS Independent",
     "Typing :: Typed",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
 ]
 
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/jorenham/mainpy/issues"
+"Changelog" = "https://github.com/jorenham/mainpy/releases"
+
+[tool.poetry.extras]
+uvloop = ["uvloop"]
+
 [tool.poetry.dependencies]
 python = "^3.8"
-typing_extensions = {version = "^4.1", python = "<3.10"}
+typing_extensions = {version = "^4.1", python = "<3.11"}
 
 [tool.poetry.dependencies.uvloop]
 version = ">=0.14,<1.0"
 optional = true
 markers = 'sys_platform != "win32"'
+python = "<3.13"
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = {version = "^3.7.0", python = ">=3.9"}
+tox = "^4.15.0"
 
 [tool.poetry.group.lint.dependencies]
+sp-repo-review = {version = "^2024.4.23", extras = ["cli"], python = ">=3.10"}
 codespell = "^2.2.6"
-ruff = "^0.3.0"
-
-[tool.poetry.group.typecheck.dependencies]
-pyright = "^1.1.351"
-pytest = "^8.0"  # needed to infer annotations when linting
+ruff = "^0.4.2"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^8.0"
+pytest = "^8.2.0"
+
+[tool.poetry.group.typecheck.dependencies]
+basedpyright = "^1.11.0"
+typing_extensions = "*"
+pytest = "*"
 
 [tool.poetry.group.test-github]
 optional = true
 [tool.poetry.group.test-github.dependencies]
-pytest-github-actions-annotate-failures = ">=0.2,<1.0"
+pytest-github-actions-annotate-failures = ">=0.2.0,<1"
+
+
+[tool.pytest.ini_options]
+addopts = ["-ra", "--strict-markers", "--strict-config"]
+filterwarnings = ["error"]
+log_cli_level = "INFO"
+minversion = "8.0"
+testpaths = ["tests"]
+xfail_strict = true
+
+
+[tool.codespell]
+context = 2
 
-[tool.poetry.extras]
-uvloop = ["uvloop"]
 
-[tool.pyright]
+[tool.basedpyright]
 include = ["mainpy", "tests"]
 exclude = [
     "**/__pycache__",
     ".git",
     ".github",
-    ".hypothesis",
     ".pytest_cache",
     ".ruff_cache",
     ".vscode",
     "dist",
 ]
+ignore = ["**/.venv"]
+stubPath = "."
 venvPath = "."
 venv = ".venv"
 pythonVersion = "3.8"
 pythonPlatform = "All"
-typeCheckingMode = "strict"
-useLibraryCodeForTypes = true
-
-deprecateTypingAliases = true
-disableBytesTypePromotions = true
-reportPropertyTypeMismatch = "warning"
-reportMissingImports = false  # uvloop is optional
-reportMissingModuleSource = false  # typing_extensions not needed on py310+
-reportMissingTypeStubs = false
-reportUnusedImport = "warning"
-reportUnusedClass = "warning"
-reportUnusedFunction = false  # @main decorated functions
-reportUnusedVariable = "warning"
-reportConstantRedefinition = "warning"
-reportInconsistentConstructor = "warning"
-reportMissingTypeArgument = "warning"
-reportUninitializedInstanceVariable = "warning"
-reportCallInDefaultInitializer = "warning"
-reportUnnecessaryIsInstance = "warning"
-reportUnnecessaryCast = "warning"
-reportUnnecessaryComparison = "warning"
-reportUnnecessaryContains = "warning"
-reportUnusedCallResult = "warning"
-reportUnusedExpression = "warning"
-reportUnnecessaryTypeIgnoreComment = false  # some aren't needed with `uvloop`
-reportMatchNotExhaustive = "warning"
-reportShadowedImports = "warning"
+typeCheckingMode = "all"
+reportAny = false
+reportUnusedCallResult = false
+reportInvalidCast = false
+# this appears to be broken since pyright 1.1.359
+reportUntypedFunctionDecorator = false
+# because of `sys.version_info()` conditionals
+reportUnreachable = false
+
+
+[tool.repo-review]
+ignore = [
+    "PY004",    # README.md >> docs/
+    "PC110",    # optype's style >> (black | ruff-format)
+    "PC140",    # (based)pyright >> mypy (by several orders of magnitude)
+    "PC170",    # no .rst
+    "PC180",    # no .css or .js
+    "MY",       # (based)pyright >> mypy (by several orders of magnitude)
+    "RTD",      # README.md >> rtd
+]
 
 
 [tool.ruff]
 src = ["mainpy", "tests"]
 target-version = "py38"
 line-length = 79
 indent-width = 4
+show-fixes = true
 force-exclude = true
-extend-exclude = [
-    ".github",
-    ".vscode",
-    ".venv",
-    "py.typed",
-]
+extend-exclude = [".github", ".vscode"]
 
 [tool.ruff.lint]
 ignore-init-module-imports = true
 preview = true
 select = [
     "F",        # pyflakes
     "E",        # pycodestyle error
     "W",        # pycodestyle warning
     "I",        # isort
     "N",        # pep8-naming
     "UP",       # pyupgrade
     "YTT",      # flake8-2020
     "ANN",      # flake8-annotations
     "ASYNC",    # flake8-async
+    "TRIO",     # flake8-trio
     "S",        # flake8-bandit
     "BLE",      # flake8-blind-except
     "B",        # flake8-bugbear
     "A",        # flake8-builtins
     "COM",      # flake8-commas
     "C4",       # flake8-comprehensions
     "DTZ",      # flake8-datetimez
@@ -143,90 +163,98 @@
     "SLF",      # flake8-self
     "SLOT",     # flake8-slots
     "SIM",      # flake8-simplify
     "TID",      # flake8-tidy-imports
     "TCH",      # flake8-type-checking
     "ARG",      # flake8-unused-arguments
     "PTH",      # flake8-use-pathlib
+    "TD",       # flake8-todos
+    "FIX",      # flake8-fixme
     "ERA",      # eradicate
+    "PD",       # pandas-vet
     "PGH",      # pygrep-hooks
     "PL",       # pylint
     "TRY",      # tryceratops
     "FLY",      # flynt
+    "NPY",      # numpy
+    "AIR",      # airflow
     "PERF",     # perflint,
     "FURB",     # refurb
     "LOG",      # flake8-logging
     "RUF",      # ruff
 ]
-extend-ignore = [
-    # flake8-annotations
-    "ANN001",   # missing-type-function-argument (deprecated)
-    "ANN002",   # missing-type-args (deprecated)
-    "ANN401",   # any-type
-    # flake8-bandit
-    "S101",     # assert
-    # pylint
-    "PLC0415",  # import-outside-top-level
-    "PLW1641",  # eq-without-hash (bug: doesn't consider super)
-    # tryceratops
-    "TRY003",   # raise-vanilla-args
-    # ruff
-    "RUF021",   # parenthesize-chained-operators
+ignore = [
+    "ANN401",   # flake8-annotations: any-type
+    "PLC0415",  # pylint: import-outside-top-level
 ]
 [tool.ruff.lint.per-file-ignores]
-"**/__init__.py" = [
-    "F401",     # pyflakes: unused-import
-]
 "tests/*" = [
-    "D",        # pydocstyle
+    "S",        # flake8-bandit
     "ANN",      # flake8-annotations
     "ARG001",   # flake8-unused-arguments: unused-function-argument
     "SLF001",   # flake8-self: private-member-access
-    "PT004",    # flake8-pytest-style: pytest-missing-fixture-name-underscore
 ]
 
 [tool.ruff.lint.pycodestyle]
 max-line-length = 79
 
 [tool.ruff.lint.isort]
 case-sensitive = true
 combine-as-imports = true
-force-wrap-aliases = true
 known-first-party = ["mainpy"]
 lines-after-imports = 2
 lines-between-types = 0
-no-lines-before = ["future", "local-folder"]
-split-on-trailing-comma = false
-
-[tool.ruff.lint.pydocstyle]
-convention = "google"
-ignore-decorators = ["typing.overload"]
-
-[tool.ruff.lint.flake8-annotations]
-suppress-none-returning = true
 
 [tool.ruff.lint.flake8-quotes]
 inline-quotes = "single"
 
+[tool.ruff.lint.flake8-type-checking]
+strict = true
+
 [tool.ruff.format]
 docstring-code-format = true
-quote-style = "single"
 indent-style = "space"
 line-ending = "lf"
+quote-style = "single"
 skip-magic-trailing-comma = true
 
 
-[tool.codespell]
-skip = "./dist,./site,*.lock,*.pyc"
-context = 2
-
-
-[tool.pytest.ini_options]
-minversion = "8.0"
-addopts = [
-    "-ra",
-    "--strict-markers",
-    "--strict-config",
-]
-xfail_strict = true
-testpaths = ["tests"]
-filterwarnings = ["error"]
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+isolated_build = true
+requires =
+    tox>=4
+envlist =
+    py{38,312,313}
+    codespell
+    ruff
+    basedpyright
+
+[testenv]
+description = pytest
+skip_install = true
+allowlist_externals = poetry
+commands_pre = poetry install --without=lint --extras=uvloop --sync
+commands = poetry run pytest
+
+[testenv:codespell]
+description = codespell
+skip_install = true
+allowlist_externals = poetry
+commands_pre = poetry install --only=lint --no-root --sync
+commands = poetry run codespell .
+
+[testenv:ruff]
+description = ruff check
+skip_install = true
+allowlist_externals = poetry
+commands_pre = poetry install --only=lint --no-root --sync
+commands = poetry run ruff check
+
+[testenv:basedpyright]
+description = basedpyright
+skip_install = true
+allowlist_externals = poetry
+commands_pre = poetry install --only=typecheck --no-root --sync
+commands = poetry run basedpyright
+"""
```

### Comparing `mainpy-1.2.1/PKG-INFO` & `mainpy-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: mainpy
-Version: 1.2.1
+Version: 1.3.0
 Summary: Simplify your project's main entrypoint definition with @main
 Home-page: https://github.com/jorenham/mainpy
 License: MIT
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development
-Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Typing :: Typed
 Provides-Extra: uvloop
-Requires-Dist: typing_extensions (>=4.1,<5.0) ; python_version < "3.10"
-Requires-Dist: uvloop (>=0.14,<1.0) ; (sys_platform != "win32") and (extra == "uvloop")
+Requires-Dist: typing_extensions (>=4.1,<5.0) ; python_version < "3.11"
+Requires-Dist: uvloop (>=0.14,<1.0) ; (sys_platform != "win32" and python_version < "3.13") and (extra == "uvloop")
+Project-URL: Bug Tracker, https://github.com/jorenham/mainpy/issues
+Project-URL: Changelog, https://github.com/jorenham/mainpy/releases
+Project-URL: Documentation, https://github.com/jorenham/mainpy?tab=readme-ov-file#mainpy
 Project-URL: Repository, https://github.com/jorenham/mainpy
 Description-Content-Type: text/markdown
 
 # `@main`.py
 
 -----
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/mainpy.svg)][PYPI]
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/mainpy.svg)][PYPI]
-[![PyPI license](https://img.shields.io/pypi/l/mainpy.svg)][PYPI]
-[![Actions status](https://github.com/jorenham/mainpy/workflows/CI/badge.svg)][CI]
-[![Pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)][PYRIGHT]
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)][RUFF]
+[![mainpy - pypi version](https://img.shields.io/pypi/v/mainpy.svg)][PYPI]
+[![mainpy - python versions](https://img.shields.io/pypi/pyversions/mainpy.svg)][PYPI]
+[![mainpy - license](https://img.shields.io/pypi/l/mainpy.svg)][PYPI]
+[![mainpy - workflow status](https://github.com/jorenham/mainpy/workflows/CI/badge.svg)][CI]
+[![mainpy - basedpyright](https://img.shields.io/badge/basedpyright-checked-42b983)][BASEDPYRIGHT]
+[![mainpy - ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)][RUFF]
 
 -----
 
 ## Basic Examples
 
 Instead of the verbose "boilerplate"
 
@@ -87,15 +88,14 @@
 def async_app(): ...
 
 # do things before running async_app()
 
 main(async_app)
 ```
 
-
 ## External Libraries
 
 Even though `mainpy` requires no other dependencies than `typing_extensions`
 (on Python < 3.10), it has optional support for [`uvloop`][UVLOOP], and plays
 nicely with popular CLI libraries, e.g. [`click`][CLICK] and [`typer`][TYPER].
 
 ### `uvloop`
@@ -190,15 +190,15 @@
 
 ```shell
 pip install mainpy[uvloop]
 ```
 
 [PYPI]: https://pypi.org/project/mainpy/
 [CI]: https://github.com/jorenham/mainpy/actions
-[PYRIGHT]: https://microsoft.github.io/pyright/
+[BASEDPYRIGHT]: https://detachhead.github.io/basedpyright/
 [RUFF]: https://github.com/astral-sh/ruff
 [UVLOOP]: https://github.com/MagicStack/uvloop
 [CLICK]: https://github.com/pallets/click
 [TYPER]: https://github.com/tiangolo/typer
 [DEVMODE]: https://docs.python.org/3/library/devmode.html
 [FAULTHANDLER]: https://docs.python.org/3/library/faulthandler.html
 [WARNINGS]: https://docs.python.org/3/library/warnings.html
```

