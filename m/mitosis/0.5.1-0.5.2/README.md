# Comparing `tmp/mitosis-0.5.1.tar.gz` & `tmp/mitosis-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitosis-0.5.1.tar", last modified: Mon Apr 29 19:09:25 2024, max compression
+gzip compressed data, was "mitosis-0.5.2.tar", last modified: Wed May  1 00:43:30 2024, max compression
```

## Comparing `mitosis-0.5.1.tar` & `mitosis-0.5.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.110498 mitosis-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-29 19:09:14.000000 mitosis-0.5.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.102498 mitosis-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.102498 mitosis-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-29 19:09:14.000000 mitosis-0.5.1/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-29 19:09:14.000000 mitosis-0.5.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-29 19:09:14.000000 mitosis-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-29 19:09:14.000000 mitosis-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-29 19:09:14.000000 mitosis-0.5.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-29 19:09:14.000000 mitosis-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16259 2024-04-29 19:09:25.110498 mitosis-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-04-29 19:09:14.000000 mitosis-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.102498 mitosis-0.5.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.102498 mitosis-0.5.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-29 19:09:14.000000 mitosis-0.5.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-29 19:09:14.000000 mitosis-0.5.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.106498 mitosis-0.5.1/mitosis/
--rw-r--r--   0 runner    (1001) docker     (127)    21349 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.106498 mitosis-0.5.1/mitosis/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/bad_return_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/mock_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/mock_paper.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/mock_part1.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/mock_part2.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/pyproject_malformed.toml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/pyproject_missing.toml
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/test_pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.106498 mitosis-0.5.1/mitosis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16259 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-29 19:09:14.000000 mitosis-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-29 19:09:25.110498 mitosis-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:30.249099 mitosis-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 00:43:19.000000 mitosis-0.5.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:30.237099 mitosis-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:30.241099 mitosis-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-01 00:43:19.000000 mitosis-0.5.2/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-01 00:43:19.000000 mitosis-0.5.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-01 00:43:19.000000 mitosis-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-01 00:43:19.000000 mitosis-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-01 00:43:19.000000 mitosis-0.5.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-01 00:43:19.000000 mitosis-0.5.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-01 00:43:19.000000 mitosis-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16259 2024-05-01 00:43:30.249099 mitosis-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-05-01 00:43:19.000000 mitosis-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:30.237099 mitosis-0.5.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:30.241099 mitosis-0.5.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-01 00:43:19.000000 mitosis-0.5.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-01 00:43:19.000000 mitosis-0.5.2/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:30.241099 mitosis-0.5.2/mitosis/
+-rw-r--r--   0 runner    (1001) docker     (127)    21349 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-01 00:43:30.000000 mitosis-0.5.2/mitosis/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:30.245099 mitosis-0.5.2/mitosis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/tests/bad_return_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/tests/mock_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/tests/mock_paper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/tests/mock_part1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/tests/mock_part2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/tests/pyproject_malformed.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/tests/pyproject_missing.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-01 00:43:19.000000 mitosis-0.5.2/mitosis/tests/test_pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:43:30.245099 mitosis-0.5.2/mitosis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16259 2024-05-01 00:43:30.000000 mitosis-0.5.2/mitosis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-01 00:43:30.000000 mitosis-0.5.2/mitosis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:43:30.000000 mitosis-0.5.2/mitosis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 00:43:30.000000 mitosis-0.5.2/mitosis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-01 00:43:30.000000 mitosis-0.5.2/mitosis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:43:30.000000 mitosis-0.5.2/mitosis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-01 00:43:19.000000 mitosis-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-01 00:43:30.249099 mitosis-0.5.2/setup.cfg
```

### Comparing `mitosis-0.5.1/.github/workflows/main.yaml` & `mitosis-0.5.2/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.1/.github/workflows/release.yaml` & `mitosis-0.5.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.1/.gitignore` & `mitosis-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.1/.pre-commit-config.yaml` & `mitosis-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.1/LICENSE` & `mitosis-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.1/PKG-INFO` & `mitosis-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitosis
-Version: 0.5.1
+Version: 0.5.2
 Summary: Reproduce Machine Learning experiments easily
 Author-email: Jake Stevens-Haas <jacob.stevens.haas@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/Jacob-Stevens-Haas/mitosis
 Keywords: Machine Learning,Science,Mathematics,Experiments
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `mitosis-0.5.1/README.md` & `mitosis-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.1/docs/source/conf.py` & `mitosis-0.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.1/mitosis/__init__.py` & `mitosis-0.5.2/mitosis/__init__.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.1/mitosis/__main__.py` & `mitosis-0.5.2/mitosis/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,17 @@
             all_steps[step_name],
             ep_dict.get(step_name, []),
             lp_dict.get(step_name, []),
         )
         for step_name in all_steps.keys()
     ]
 
-    folder = _disk.locate_trial_folder(trials_folder=args.folder, proj_file=args.config)
+    folder = _disk.locate_trial_folder(
+        trials_folder=args.trials_folder, proj_file=args.config
+    )
     return {
         "steps": exp_steps,
         "debug": args.debug,
         "trials_folder": folder,
     }
```

### Comparing `mitosis-0.5.1/mitosis/_disk.py` & `mitosis-0.5.2/mitosis/_disk.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.1/mitosis/_typing.py` & `mitosis-0.5.2/mitosis/_typing.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.1/mitosis/tests/test_all.py` & `mitosis-0.5.2/mitosis/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.1/mitosis/tests/test_cli.py` & `mitosis-0.5.2/mitosis/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import contextlib
+import os
 import sys
 from argparse import Namespace
 from io import StringIO
 from typing import Generator
 
 import pytest
 
@@ -24,15 +25,15 @@
 )
 def test_legacy_module(params, eval_params):
     args = Namespace(
         experiment=[],
         module="mitosis.tests.mock_legacy",
         debug=True,
         config="pyproject.toml",
-        folder=None,
+        trials_folder=None,
         eval_param=eval_params,
         param=params,
     )
     result = _process_cl_args(args)
     assert len(result["steps"]) == 1
     assert result["steps"][0].name == "mitosis.tests.mock_legacy"
     assert result["steps"][0].action == run
@@ -41,25 +42,44 @@
 
 def test_experiment_arg():
     args = Namespace(
         experiment=["data", "fit_eval"],
         module=None,
         debug=True,
         config="mitosis/tests/test_pyproject.toml",
-        folder=None,
+        trials_folder=None,
         eval_param=["data.extra=True"],
         param=["data.length=test", "fit_eval.metric=test"],
     )
     result = _process_cl_args(args)
     assert len(result["steps"]) == 2
     assert [step.name for step in result["steps"]] == ["data", "fit_eval"]
     assert result["steps"][0].action == Klass.gen_data
     assert id(result["steps"][1].lookup) == id(meth_config)
 
 
+def test_folder_arg(tmp_path):
+    parser = _create_parser()
+    args = parser.parse_args(["-m", "mitosis.tests.mock_legacy", "-F", "foo"])
+
+    @contextlib.contextmanager
+    def change_cwd(new_pth: os.PathLike) -> Generator[None, None, None]:
+        temp = os.getcwd()
+        try:
+            os.chdir(new_pth)
+            yield
+        finally:
+            os.chdir(temp)
+
+    with change_cwd(tmp_path):
+        result = _process_cl_args(args)["trials_folder"]
+    expected = tmp_path / "foo"
+    assert result == expected
+
+
 def test_argparse_options():
     parser = _create_parser()
     args = parser.parse_args(
         ["-m", "mod", "-d", "--config", "foo.toml", "-F", "foo/bar"]
     )
     assert args.experiment == []
     assert args.module == "mod"
```

### Comparing `mitosis-0.5.1/mitosis.egg-info/PKG-INFO` & `mitosis-0.5.2/mitosis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitosis
-Version: 0.5.1
+Version: 0.5.2
 Summary: Reproduce Machine Learning experiments easily
 Author-email: Jake Stevens-Haas <jacob.stevens.haas@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/Jacob-Stevens-Haas/mitosis
 Keywords: Machine Learning,Science,Mathematics,Experiments
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `mitosis-0.5.1/mitosis.egg-info/SOURCES.txt` & `mitosis-0.5.2/mitosis.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
+CITATION.cff
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 .github/workflows/main.yaml
 .github/workflows/release.yaml
 docs/source/conf.py
```

### Comparing `mitosis-0.5.1/pyproject.toml` & `mitosis-0.5.2/pyproject.toml`

 * *Files identical despite different names*

