# Comparing `tmp/referencing_loaders-2024.5.1.tar.gz` & `tmp/referencing_loaders-2024.5.2.tar.gz`

## Comparing `referencing_loaders-2024.5.1.tar` & `referencing_loaders-2024.5.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/.readthedocs.yml
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/noxfile.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/test-requirements.in
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/test-requirements.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/.github/SECURITY.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/docs/conf.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/docs/index.rst
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/docs/requirements.in
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/docs/requirements.txt
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/referencing_loaders/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/referencing_loaders/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/referencing_loaders/tests/__init__.py
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/referencing_loaders/tests/test_loaders.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/COPYING
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/README.rst
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/pyproject.toml
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.1/PKG-INFO
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/.readthedocs.yml
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/noxfile.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/test-requirements.in
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/test-requirements.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/.github/SECURITY.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/.github/release.yml
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/docs/conf.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/docs/index.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/docs/requirements.in
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/docs/requirements.txt
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/referencing_loaders/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/referencing_loaders/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/referencing_loaders/tests/__init__.py
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/referencing_loaders/tests/test_loaders.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/COPYING
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/README.rst
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 referencing_loaders-2024.5.2/PKG-INFO
```

### Comparing `referencing_loaders-2024.5.1/.pre-commit-config.yaml` & `referencing_loaders-2024.5.2/.pre-commit-config.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-ast
       - id: check-toml
       - id: check-vcs-permalinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.2.2"
+    rev: "v0.4.2"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/PyCQA/isort
     rev: 5.13.2
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 24.2.0
+    rev: 24.4.2
     hooks:
       - name: black
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v4.0.0-alpha.8"
     hooks:
```

### Comparing `referencing_loaders-2024.5.1/noxfile.py` & `referencing_loaders-2024.5.2/noxfile.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 PACKAGE = ROOT / "referencing_loaders"
 
 REQUIREMENTS = dict(
     docs=DOCS / "requirements.txt",
     tests=ROOT / "test-requirements.txt",
 )
 REQUIREMENTS_IN = [  # this is actually ordered, as files depend on each other
-    path.parent / f"{path.stem}.in" for path in REQUIREMENTS.values()
+    (path.parent / f"{path.stem}.in", path) for path in REQUIREMENTS.values()
 ]
 
 SUPPORTED = ["3.8", "3.9", "3.10", "pypy3.10", "3.11", "3.12"]
 LATEST = SUPPORTED[-1]
 
+nox.options.default_venv_backend = "uv|virtualenv"
 nox.options.sessions = []
 
 
 def session(default=True, python=LATEST, **kwargs):  # noqa: D103
     def _session(fn):
         if default:
             nox.options.sessions.append(kwargs.get("name", fn.__name__))
@@ -158,17 +159,17 @@
 @session(default=False)
 def requirements(session):
     """
     Update the project's pinned requirements.
 
     You should commit the result afterwards.
     """
-    session.install("pip-tools")
-    for each in REQUIREMENTS_IN:
-        session.run(
-            "pip-compile",
-            "--resolver",
-            "backtracking",
-            "--strip-extras",
-            "-U",
-            each.relative_to(ROOT),
-        )
+    if session.venv_backend == "uv":
+        cmd = ["uv", "pip", "compile"]
+    else:
+        session.install("pip-tools")
+        cmd = ["pip-compile", "--resolver", "backtracking", "--strip-extras"]
+
+    for each, out in REQUIREMENTS_IN:
+        # otherwise output files end up with silly absolute path comments...
+        relative = each.relative_to(ROOT)
+        session.run(*cmd, "--upgrade", "--output-file", out, relative)
```

### Comparing `referencing_loaders-2024.5.1/.github/SECURITY.md` & `referencing_loaders-2024.5.2/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `referencing_loaders-2024.5.1/.github/workflows/ci.yml` & `referencing_loaders-2024.5.2/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 name: CI
 
 on:
   push:
+    branches-ignore:
+      - "wip*"
+    tags:
+      - "v*"
   pull_request:
   release:
     types: [published]
   schedule:
     # Daily at 7:4
     - cron: "4 7 * * *"
+  workflow_dispatch:
 
 env:
   PIP_DISABLE_PIP_VERSION_CHECK: "1"
   PIP_NO_PYTHON_VERSION_WARNING: "1"
 
 jobs:
-  pre-commit:
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v4
-      - uses: actions/setup-python@v5
-        with:
-          python-version: "3.x"
-      - uses: pre-commit/action@v3.0.1
-
   list:
     runs-on: ubuntu-latest
     outputs:
       noxenvs: ${{ steps.noxenvs-matrix.outputs.noxenvs }}
     steps:
       - uses: actions/checkout@v4
       - name: Set up nox
-        uses: wntrblm/nox@2024.03.02
+        uses: wntrblm/nox@2024.04.15
       - id: noxenvs-matrix
         run: |
           echo >>$GITHUB_OUTPUT noxenvs=$(
             nox --list-sessions --json | jq '[.[].session]'
           )
 
   ci:
     needs: list
     runs-on: ${{ matrix.os }}
+
     strategy:
       fail-fast: false
       matrix:
         os: [macos-latest, ubuntu-latest]
         noxenv: ${{ fromJson(needs.list.outputs.noxenvs) }}
         posargs: [""]
         include:
@@ -66,16 +63,20 @@
             3.8
             3.9
             3.10
             3.11
             3.12
             pypy3.10
           allow-prereleases: true
+          cache: pip
+      - name: Set up uv
+        uses: hynek/setup-cached-uv@v1
       - name: Set up nox
-        uses: wntrblm/nox@2024.03.02
+        uses: wntrblm/nox@2024.04.15
+
       - name: Run nox
         run: nox -s "${{ matrix.noxenv }}" -- ${{ matrix.posargs }}
 
   packaging:
     needs: ci
     runs-on: ubuntu-latest
     environment:
@@ -86,14 +87,15 @@
       id-token: write
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
+          cache: pip
           python-version: "3.x"
       - name: Install dependencies
         run: python -m pip install build
       - name: Create packages
         run: python -m build .
       - name: Publish to PyPI
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
```

### Comparing `referencing_loaders-2024.5.1/docs/conf.py` & `referencing_loaders-2024.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `referencing_loaders-2024.5.1/docs/requirements.txt` & `referencing_loaders-2024.5.2/docs/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,85 +1,73 @@
-#
-# This file is autogenerated by pip-compile with Python 3.12
-# by the following command:
-#
-#    pip-compile --strip-extras docs/requirements.in
-#
+# This file was autogenerated by uv via the following command:
+#    uv pip compile --output-file docs/requirements.txt docs/requirements.in
 alabaster==0.7.16
     # via sphinx
 attrs==23.2.0
     # via referencing
 babel==2.14.0
     # via sphinx
 beautifulsoup4==4.12.3
     # via furo
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-docutils==0.20.1
+docutils==0.21.2
     # via sphinx
-furo==2024.1.29
-    # via -r docs/requirements.in
-idna==3.6
+furo==2024.4.27
+idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.3
     # via sphinx
 markupsafe==2.1.5
     # via jinja2
 packaging==24.0
     # via sphinx
-pyenchant==3.2.2
+pyenchant==3.3.0rc1
     # via sphinxcontrib-spelling
 pygments==2.17.2
     # via
     #   furo
     #   pygments-github-lexers
     #   sphinx
 pygments-github-lexers==0.0.5
-    # via -r docs/requirements.in
-referencing==0.33.0
+referencing==0.35.0
     # via referencing-loaders
-file:.#egg=referencing-loaders
-    # via -r docs/requirements.in
+referencing-loaders @ file:.#egg=referencing-loaders
 requests==2.31.0
     # via sphinx
 rpds-py==0.18.0
     # via referencing
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
-    #   -r docs/requirements.in
     #   furo
     #   sphinx-basic-ng
     #   sphinx-copybutton
     #   sphinxcontrib-spelling
     #   sphinxext-opengraph
 sphinx-basic-ng==1.0.0b2
     # via furo
 sphinx-copybutton==0.5.2
-    # via -r docs/requirements.in
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 sphinxcontrib-spelling==8.0.0
-    # via -r docs/requirements.in
 sphinxext-opengraph==0.9.1
-    # via -r docs/requirements.in
 url-py==0.10.0
-    # via -r docs/requirements.in
 urllib3==2.2.1
     # via requests
```

### Comparing `referencing_loaders-2024.5.1/referencing_loaders/__init__.py` & `referencing_loaders-2024.5.2/referencing_loaders/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,17 @@
     """
     Load some resources recursively from a given directory path.
 
     Subdirectories are defaulted to the first version seen (starting from
     the root) -- though it still is often a good idea to explicitly indicate
     what specification every resource is written for internally.
     """
-    return _from_walked(_walk(root))
+    return _from_walked(
+        each for each in _walk(root) if each.name.endswith(".json")
+    )
 
 
 def _walk(path: Path) -> Iterable[Path]:
     walk = getattr(path, "walk", None)
     if walk is None:
         for dir, _, files in os.walk(path):  # pragma: no cover
             for file in files:
@@ -57,17 +59,15 @@
 def from_traversable(root: Traversable) -> Iterable[tuple[URI, Resource[Any]]]:
     """
     Load some resources from a given `importlib.resources` traversable.
 
     (I.e. load schemas from data within a Python package.)
     """
     return _from_walked(
-        each
-        for each in _walk_traversable(root)
-        if not each.name.endswith((".py", ".pyc", ".pyo"))
+        each for each in _walk_traversable(root) if each.name.endswith(".json")
     )
 
 
 def _from_walked(
     paths: Iterable[Path | Traversable],
 ) -> Iterable[tuple[URI, Resource[Any]]]:
     specification: Specification[Any] | None = None
```

### Comparing `referencing_loaders-2024.5.1/referencing_loaders/tests/test_loaders.py` & `referencing_loaders-2024.5.2/referencing_loaders/tests/test_loaders.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,14 +83,31 @@
     )
 
     resources = loaders.from_path(tmp_path)
     registry = EMPTY_REGISTRY.with_resources(resources)
     assert registry.crawl() == expected.crawl()
 
 
+def test_hidden_files_are_ignored(tmp_path):
+    schema_path, schema = tmp_path / "schema.json", {
+        "$schema": "https://json-schema.org/draft/2020-12/schema",
+        "$id": "http://example.com/",
+    }
+    hidden_path = tmp_path / ".hidden"
+
+    schema_path.write_text(json.dumps(schema))
+    hidden_path.write_text("total nonsense")
+
+    expected = Registry().with_contents([(schema_path.as_uri(), schema)])
+
+    resources = loaders.from_path(tmp_path)
+    registry = EMPTY_REGISTRY.with_resources(resources)
+    assert registry.crawl() == expected.crawl()
+
+
 def test_empty(tmp_path):
     registry = EMPTY_REGISTRY.with_resources(loaders.from_path(tmp_path))
     assert registry == EMPTY_REGISTRY
 
 
 def test_traversable(tmp_path):
     package = tmp_path / "foo"
```

### Comparing `referencing_loaders-2024.5.1/COPYING` & `referencing_loaders-2024.5.2/COPYING`

 * *Files identical despite different names*

### Comparing `referencing_loaders-2024.5.1/README.rst` & `referencing_loaders-2024.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `referencing_loaders-2024.5.1/pyproject.toml` & `referencing_loaders-2024.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `referencing_loaders-2024.5.1/PKG-INFO` & `referencing_loaders-2024.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: referencing-loaders
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: Loading resources from various locations into referencing registries
 Project-URL: Homepage, https://github.com/python-jsonschema/referencing-loaders
 Project-URL: Issues, https://github.com/python-jsonschema/referencing-loaders/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/python-jsonschema/referencing-loaders
 Author-email: Julian Berman <Julian+referencing-loaders@GrayVines.com>
 License-File: COPYING
```

