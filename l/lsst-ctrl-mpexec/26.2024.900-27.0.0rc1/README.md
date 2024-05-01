# Comparing `tmp/lsst-ctrl-mpexec-26.2024.900.tar.gz` & `tmp/lsst_ctrl_mpexec-27.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-ctrl-mpexec-26.2024.900.tar", last modified: Thu Feb 29 10:22:41 2024, max compression
+gzip compressed data, was "lsst_ctrl_mpexec-27.0.0rc1.tar", last modified: Wed May  1 21:18:49 2024, max compression
```

## Comparing `lsst-ctrl-mpexec-26.2024.900.tar` & `lsst_ctrl_mpexec-27.0.0rc1.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.155057 lsst-ctrl-mpexec-26.2024.900/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-02-29 10:22:41.155057 lsst-ctrl-mpexec-26.2024.900/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.139056 lsst-ctrl-mpexec-26.2024.900/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.139056 lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/
--rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/configuring-pipetask-tasks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/pipetask.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.139056 lsst-ctrl-mpexec-26.2024.900/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.143056 lsst-ctrl-mpexec-26.2024.900/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.143056 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.143056 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.147056 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.147056 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.147056 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/optionGroups.py
--rw-r--r--   0 runner    (1001) docker     (127)    18341 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/pipetask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.147056 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/confirmable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/pre_exec_init_qbb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/purge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/run_qbb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/update_graph_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    41298 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cmdLineFwk.py
--rw-r--r--   0 runner    (1001) docker     (127)    13673 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/dotTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/execFixupDataId.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/executionGraphFixup.py
--rw-r--r--   0 runner    (1001) docker     (127)     9238 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/mpGraphExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)    21671 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/preExecInit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/quantumGraphExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/separablePipelineExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/showInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/simple_pipeline_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    23338 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/singleQuantumExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/taskFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:22:40.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.151056 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-02-29 10:22:41.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-02-29 10:22:41.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:22:41.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-29 10:22:41.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-29 10:22:41.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:22:41.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:22:40.000000 lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-29 10:22:41.155057 lsst-ctrl-mpexec-26.2024.900/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:22:41.151056 lsst-ctrl-mpexec-26.2024.900/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdCleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdPurge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdReport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdUpdateGraphRun.py
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cliScript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cliUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    46275 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_cmdLineFwk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_dotTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    30387 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_executors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_preExecInit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    27390 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_separablePipelineExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15981 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_simple_pipeline_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-02-29 10:22:29.000000 lsst-ctrl-mpexec-26.2024.900/tests/test_taskFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:49.410920 lsst_ctrl_mpexec-27.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-01 21:18:49.410920 lsst_ctrl_mpexec-27.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:49.394920 lsst_ctrl_mpexec-27.0.0rc1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:49.398920 lsst_ctrl_mpexec-27.0.0rc1/doc/lsst.ctrl.mpexec/
+-rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/doc/lsst.ctrl.mpexec/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/doc/lsst.ctrl.mpexec/configuring-pipetask-tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/doc/lsst.ctrl.mpexec/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/doc/lsst.ctrl.mpexec/pipetask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:49.394920 lsst_ctrl_mpexec-27.0.0rc1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:49.398920 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:49.398920 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:49.402920 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:49.402920 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:49.402920 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:49.402920 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/opt/optionGroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19210 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/pipetask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:49.406920 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/confirmable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/pre_exec_init_qbb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/purge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/run_qbb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/update_graph_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41717 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cmdLineFwk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13913 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/dotTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/execFixupDataId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/executionGraphFixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27923 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/mpGraphExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19881 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/preExecInit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/quantumGraphExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/separablePipelineExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16065 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/showInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/simple_pipeline_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25906 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/singleQuantumExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/taskFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:18:49.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:49.410920 lsst_ctrl_mpexec-27.0.0rc1/python/lsst_ctrl_mpexec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-01 21:18:49.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst_ctrl_mpexec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-01 21:18:49.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst_ctrl_mpexec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:18:49.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst_ctrl_mpexec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-01 21:18:49.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst_ctrl_mpexec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-01 21:18:49.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst_ctrl_mpexec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 21:18:49.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst_ctrl_mpexec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:18:48.000000 lsst_ctrl_mpexec-27.0.0rc1/python/lsst_ctrl_mpexec.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-01 21:18:49.410920 lsst_ctrl_mpexec-27.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:18:49.410920 lsst_ctrl_mpexec-27.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_cliCmdCleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_cliCmdPurge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_cliCmdQgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_cliCmdReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_cliCmdUpdateGraphRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_cliScript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_cliUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46363 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_cmdLineFwk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_dotTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31497 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_preExecInit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27234 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_separablePipelineExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16813 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_simple_pipeline_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-01 21:18:43.000000 lsst_ctrl_mpexec-27.0.0rc1/tests/test_taskFactory.py
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/PKG-INFO` & `lsst_ctrl_mpexec-27.0.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-mpexec
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: Pipeline execution infrastructure for the Rubin Observatory LSST Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_mpexec
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/README.rst` & `lsst_ctrl_mpexec-27.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/bsd_license.txt` & `lsst_ctrl_mpexec-27.0.0rc1/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/CHANGES.rst` & `lsst_ctrl_mpexec-27.0.0rc1/doc/lsst.ctrl.mpexec/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/configuring-pipetask-tasks.rst` & `lsst_ctrl_mpexec-27.0.0rc1/doc/lsst.ctrl.mpexec/configuring-pipetask-tasks.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/doc/lsst.ctrl.mpexec/index.rst` & `lsst_ctrl_mpexec-27.0.0rc1/doc/lsst.ctrl.mpexec/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/gpl-v3.0.txt` & `lsst_ctrl_mpexec-27.0.0rc1/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/pyproject.toml` & `lsst_ctrl_mpexec-27.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/__init__.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/__init__.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/__init__.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/__init__.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/cmd/__init__.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/cmd/commands.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/cmd/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from functools import partial
 from tempfile import NamedTemporaryFile
 from typing import Any
 
 import click
 import coverage
 import lsst.pipe.base.cli.opt as pipeBaseOpts
+from lsst.ctrl.mpexec import Report
 from lsst.ctrl.mpexec.showInfo import ShowInfo
 from lsst.daf.butler.cli.opt import (
     config_file_option,
     config_option,
     confirm_option,
     options_file_option,
     processes_option,
@@ -173,25 +174,34 @@
 @ctrlMpExecOpts.butler_options()
 @option_section(sectionText="")
 @options_file_option()
 @catch_and_exit
 def qgraph(ctx: click.Context, **kwargs: Any) -> None:
     """Build and optionally save quantum graph."""
     kwargs = _collectActions(ctx, **kwargs)
+    summary = kwargs.pop("summary", None)
     with coverage_context(kwargs):
         show = ShowInfo(kwargs.pop("show", []))
         pipeline = script.build(**kwargs, show=show)
         if show.handled and not show.unhandled:
             print(
                 "No quantum graph generated. The --show option was given and all options were processed.",
                 file=sys.stderr,
             )
             return
-        if script.qgraph(pipelineObj=pipeline, **kwargs, show=show) is None:
+        if (qgraph := script.qgraph(pipelineObj=pipeline, **kwargs, show=show)) is None:
             raise click.ClickException("QuantumGraph was empty; CRITICAL logs above should provide details.")
+        # QuantumGraph-only summary call here since script.qgraph also called
+        # by run methods.
+        if summary:
+            report = Report(qgraphSummary=qgraph.getSummary())
+            with open(summary, "w") as out:
+                # Do not save fields that are not set.
+                out.write(report.model_dump_json(exclude_none=True, indent=2))
+
         _unhandledShow(show, "qgraph")
 
 
 @click.command(cls=PipetaskCommand, epilog=epilog)
 @ctrlMpExecOpts.run_options()
 @catch_and_exit
 def run(ctx: click.Context, **kwargs: Any) -> None:
@@ -325,20 +335,28 @@
     """
     script.update_graph_run(qgraph, run, output_qgraph, metadata_run_key, update_graph_id)
 
 
 @click.command(cls=PipetaskCommand)
 @repo_argument()
 @ctrlMpExecOpts.qgraph_argument()
-@click.argument("output_yaml", type=click.Path(exists=False))
+@click.option("--full-output-filename", default="", help="Summarize report in a yaml file")
 @click.option("--logs/--no-logs", default=True, help="Get butler log datasets for extra information.")
-def report(repo: str, qgraph: str, output_yaml: str, logs: bool = True) -> None:
+@click.option(
+    "--show-errors",
+    is_flag=True,
+    default=False,
+    help="Pretty-print a dict of errors from failed"
+    " quanta to the screen. Note: the default is to output a yaml file with error information"
+    " (data_ids and associated messages) to the current working directory instead.",
+)
+def report(
+    repo: str, qgraph: str, full_output_filename: str = "", logs: bool = True, show_errors: bool = False
+) -> None:
     """Write a yaml file summarizing the produced and missing expected datasets
     in a quantum graph.
 
     REPO is the location of the butler/registry config file.
 
     QGRAPH is the URL to a serialized Quantum Graph file.
-
-    OUTPUT_YAML is the URL to store the summary report.
     """
-    script.report(repo, qgraph, output_yaml, logs)
+    script.report(repo, qgraph, full_output_filename, logs, show_errors)
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/__init__.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/arguments.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/optionGroups.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/opt/optionGroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
             ctrlMpExecOpts.qgraph_datastore_records_option(),
             ctrlMpExecOpts.skip_existing_in_option(),
             ctrlMpExecOpts.skip_existing_option(),
             ctrlMpExecOpts.clobber_outputs_option(),
             ctrlMpExecOpts.save_qgraph_option(),
             ctrlMpExecOpts.save_single_quanta_option(),
             ctrlMpExecOpts.qgraph_dot_option(),
+            ctrlMpExecOpts.summary_option(),
             ctrlMpExecOpts.save_execution_butler_option(),
             ctrlMpExecOpts.clobber_execution_butler_option(),
             ctrlMpExecOpts.target_datastore_root_option(),
             transfer_option_no_short(
                 help=unwrap(
                     """Data transfer mode for the execution butler datastore.
                     Defaults to "copy" if --target-datastore-root is provided.
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/opt/options.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/opt/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,19 +24,26 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 from collections.abc import Iterable, Mapping
+from typing import TYPE_CHECKING
 
 import click
 from lsst.daf.butler.cli.utils import MWOptionDecorator, MWPath, split_commas, unwrap
 from lsst.utils.doImport import doImportType
 
+if TYPE_CHECKING:
+    # Avoid regular module-scope import of test-only code that tinkers with the
+    # storage class singleton.
+    from lsst.pipe.base.tests.mocks import ForcedFailure
+
+
 butler_config_option = MWOptionDecorator(
     "-b", "--butler-config", help="Location of the gen3 butler/registry config file."
 )
 
 
 data_query_option = MWOptionDecorator(
     "-d", "--data-query", help="User data selection expression.", metavar="QUERY"
@@ -461,56 +468,69 @@
     multiple=True,
     help="Names of input dataset types that should not be mocked.",
 )
 
 
 def parse_mock_failure(
     ctx: click.Context, param: click.Option, value: Iterable[str] | None
-) -> Mapping[str, tuple[str, type[Exception] | None]]:
+) -> Mapping[str, ForcedFailure]:
     """Parse the --mock-failure option values into the mapping accepted by
     `~lsst.pipe.base.tests.mocks.mock_task_defs`.
 
     Parameters
     ----------
     ctx : `click.Context`
         Context provided by Click.
     param : `click.Option`
         Click option.
     value : `~collections.abc.Iterable` [`str`] or `None`
         Value from option.
     """
-    result: dict[str, tuple[str, type[Exception] | None]] = {}
+    # Avoid regular module-scope import of test-only code that tinkers with the
+    # storage class singleton.
+    from lsst.pipe.base.tests.mocks import ForcedFailure
+
+    result: dict[str, ForcedFailure] = {}
     if value is None:
         return result
     for entry in value:
         try:
-            task_label, error_type_name, where = entry.split(":", 2)
+            task_label, error_type_name, where, *rest = entry.split(":")
+            if rest:
+                (memory_required,) = rest
+            else:
+                memory_required = None
         except ValueError:
             raise click.UsageError(
                 f"Invalid value for --mock-failure option: {entry!r}; "
-                "expected a string of the form 'task:error:where'."
+                "expected a string of the form 'task:error:where[:mem]'."
             ) from None
         error_type = doImportType(error_type_name) if error_type_name else None
-        result[task_label] = (where, error_type)
+        result[task_label] = ForcedFailure(where, error_type, memory_required)
     return result
 
 
 mock_failure_option = MWOptionDecorator(
     "--mock-failure",
     callback=parse_mock_failure,
     metavar="LABEL:EXCEPTION:WHERE",
     default=None,
     multiple=True,
     help=unwrap(
         """Specifications for tasks that should be configured to fail
-        when mocking execution.  This is a colon-separated 3-tuple, where the
-        first entry the task label, the second the fully-qualified exception
-        type (empty for ValueError, and the third a string (which typically
-        needs to be quoted to be passed as one argument value by the shell) of
-        the form passed to --where, indicating which data IDs should fail."""
+        when mocking execution.  This is a colon-separated 3-tuple or 4-tuple,
+        where the first entry the task label, the second the fully-qualified
+        exception type (empty for ValueError, and the third a string (which
+        typically needs to be quoted to be passed as one argument value by the
+        shell) of the form passed to --where, indicating which data IDs should
+        fail.  The final optional term is the memory "required" by the task
+        (with units recognized by astropy), which will cause the error to only
+        occur if the "available" memory (according to
+        ExecutionResources.max_mem) is less than this value.  Note that actual
+        memory usage is irrelevant here; this is all mock behavior."""
     ),
 )
 
 
 clobber_execution_butler_option = MWOptionDecorator(
     "--clobber-execution-butler",
     help=unwrap(
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/pipetask.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/pipetask.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/__init__.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/build.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/build.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/cleanup.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/cleanup.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/confirmable.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/confirmable.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/pre_exec_init_qbb.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/pre_exec_init_qbb.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/purge.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/purge.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/qgraph.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/qgraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 from types import SimpleNamespace
 
-from lsst.pipe.base.graphBuilder import DatasetQueryConstraintVariant
+from lsst.pipe.base.all_dimensions_quantum_graph_builder import DatasetQueryConstraintVariant
 
 from ... import CmdLineFwk
 
 _log = logging.getLogger(__name__)
 
 
 def qgraph(  # type: ignore
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/report.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/executionGraphFixup.py`

 * *Files 27% similar despite different names*

```diff
@@ -21,37 +21,49 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from lsst.daf.butler import Butler
+__all__ = ["ExecutionGraphFixup"]
+
+from abc import ABC, abstractmethod
+
 from lsst.pipe.base import QuantumGraph
-from lsst.pipe.base.execution_reports import QuantumGraphExecutionReport
 
 
-def report(butler_config: str, qgraph_uri: str, output_yaml: str, logs: bool = True) -> None:
-    """Write a yaml file summarizing the produced and missing expected datasets
-    in a quantum graph.
-
-    Parameters
-    ----------
-    butler_config : `str`
-        The Butler used for this report. This should match the Butler used
-        for the run associated with the executed quantum graph.
-    qgraph_uri : `str`
-        The uri of the location of said quantum graph.
-    output_yaml : `str`
-        The name to be used for the summary yaml file.
-    logs : `bool`
-        Get butler log datasets for extra information.
-
-    See Also
-    --------
-    lsst.pipe.base.QuantumGraphExecutionReport.make_reports : Making reports.
-    lsst.pipe.base.QuantumGraphExecutionReport.write_summary_yaml : Summaries.
+class ExecutionGraphFixup(ABC):
+    """Interface for classes which update quantum graphs before execution.
+
+    Primary goal of this class is to modify quanta dependencies which may
+    not be possible to reflect in a quantum graph using standard tools.
+    One known use case for that is to guarantee particular execution order
+    of visits in CI jobs for cases when outcome depends on the processing
+    order of visits (e.g. AP association pipeline).
+
+    Instances of this class receive pre-ordered sequence of quanta
+    (`~lsst.pipe.base.QuantumGraph` instances) and they are allowed to
+    modify quanta data in place, for example update ``dependencies`` field to
+    add additional dependencies. Returned list of quanta will be re-ordered
+    once again by the graph executor to reflect new dependencies.
     """
-    butler = Butler.from_config(butler_config, writeable=False)
-    qgraph = QuantumGraph.loadUri(qgraph_uri)
-    report = QuantumGraphExecutionReport.make_reports(butler, qgraph)
-    report.write_summary_yaml(butler, output_yaml, do_store_logs=logs)
+
+    @abstractmethod
+    def fixupQuanta(self, graph: QuantumGraph) -> QuantumGraph:
+        """Update quanta in a graph.
+
+        Potentially anything in the graph could be changed if it does not
+        break executor assumptions. If modifications result in a dependency
+        cycle the executor will raise an exception.
+
+        Parameters
+        ----------
+        graph : QuantumGraph
+            Quantum Graph that will be executed by the executor.
+
+        Returns
+        -------
+        graph : QuantumGraph
+            Modified graph.
+        """
+        raise NotImplementedError
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/run.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/run.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/run_qbb.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/run_qbb.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/script/update_graph_run.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/script/update_graph_run.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cli/utils.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cli/utils.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/cmdLineFwk.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/cmdLineFwk.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,67 +31,66 @@
 from __future__ import annotations
 
 __all__ = ["CmdLineFwk"]
 
 import atexit
 import contextlib
 import copy
-import datetime
-import getpass
 import logging
 import shutil
-from collections.abc import Iterable, Mapping, Sequence
+from collections.abc import Mapping, Sequence
 from types import SimpleNamespace
 
 import astropy.units as u
 import lsst.utils.timer
 from astropy.table import Table
 from lsst.daf.butler import (
     Butler,
     CollectionType,
     Config,
     DatasetId,
-    DatasetRef,
     DatasetType,
     DimensionUniverse,
     LimitedButler,
     Quantum,
     QuantumBackedButler,
     Registry,
 )
 from lsst.daf.butler.datastore.cache_manager import DatastoreCacheManager
 from lsst.daf.butler.datastore.record_data import DatastoreRecordData
 from lsst.daf.butler.direct_butler import DirectButler
 from lsst.daf.butler.registry import MissingCollectionError, RegistryDefaults
 from lsst.daf.butler.registry.wildcards import CollectionWildcard
 from lsst.pipe.base import (
     ExecutionResources,
-    GraphBuilder,
     Instrument,
     Pipeline,
-    PipelineDatasetTypes,
+    PipelineGraph,
     QuantumGraph,
-    TaskDef,
     TaskFactory,
     buildExecutionButler,
 )
+from lsst.pipe.base.all_dimensions_quantum_graph_builder import AllDimensionsQuantumGraphBuilder
+from lsst.pipe.base.pipeline_graph import NodeType
 from lsst.utils import doImportType
+from lsst.utils.logging import getLogger
 from lsst.utils.threads import disable_implicit_threading
 
 from .dotTools import graph2dot, pipeline2dot
 from .executionGraphFixup import ExecutionGraphFixup
 from .mpGraphExecutor import MPGraphExecutor
 from .preExecInit import PreExecInit, PreExecInitLimited
+from .reports import Report
 from .singleQuantumExecutor import SingleQuantumExecutor
 
 # ----------------------------------
 #  Local non-exported definitions --
 # ----------------------------------
 
-_LOG = logging.getLogger(__name__)
+_LOG = getLogger(__name__)
 
 
 class _OutputChainedCollectionInfo:
     """A helper class for handling command-line arguments related to an output
     `~lsst.daf.butler.CollectionType.CHAINED` collection.
 
     Parameters
@@ -411,24 +410,24 @@
         """
         defined, cache_dir = DatastoreCacheManager.set_fallback_cache_directory_if_unset()
         if defined:
             atexit.register(shutil.rmtree, cache_dir, ignore_errors=True)
             _LOG.debug("Defining shared datastore cache directory to %s", cache_dir)
 
     @classmethod
-    def makeWriteButler(cls, args: SimpleNamespace, taskDefs: Iterable[TaskDef] | None = None) -> Butler:
+    def makeWriteButler(cls, args: SimpleNamespace, pipeline_graph: PipelineGraph | None = None) -> Butler:
         """Return a read-write butler initialized to write to and read from
         the collections specified by the given command-line arguments.
 
         Parameters
         ----------
         args : `types.SimpleNamespace`
             Parsed command-line arguments.  See class documentation for the
             construction parameter of the same name.
-        taskDefs : iterable of `TaskDef`, optional
+        pipeline_graph : `lsst.pipe.base.PipelineGraph`, optional
             Definitions for tasks in a pipeline. This argument is only needed
             if ``args.replace_run`` is `True` and ``args.prune_replaced`` is
             "unstore".
 
         Returns
         -------
         butler : `lsst.daf.butler.Butler`
@@ -442,20 +441,25 @@
         if self.output is not None:
             chainDefinition = list(self.output.chain if self.output.exists else self.inputs)
             if args.replace_run:
                 replaced = chainDefinition.pop(0)
                 if args.prune_replaced == "unstore":
                     # Remove datasets from datastore
                     with butler.transaction():
-                        refs: Iterable[DatasetRef] = butler.registry.queryDatasets(..., collections=replaced)
-                        # we want to remove regular outputs but keep
-                        # initOutputs, configs, and versions.
-                        if taskDefs is not None:
-                            initDatasetNames = set(PipelineDatasetTypes.initOutputNames(taskDefs))
-                            refs = [ref for ref in refs if ref.datasetType.name not in initDatasetNames]
+                        # we want to remove regular outputs from this pipeline,
+                        # but keep initOutputs, configs, and versions.
+                        if pipeline_graph is not None:
+                            refs = [
+                                ref
+                                for ref in butler.registry.queryDatasets(..., collections=replaced)
+                                if (
+                                    (producer := pipeline_graph.producer_of(ref.datasetType.name)) is not None
+                                    and producer.key.node_type is NodeType.TASK  # i.e. not TASK_INIT
+                                )
+                            ]
                         butler.pruneDatasets(refs, unstore=True, disassociate=False)
                 elif args.prune_replaced == "purge":
                     # Erase entire collection and all datasets, need to remove
                     # collection from its chain collection first.
                     with butler.transaction():
                         butler.registry.setCollectionChain(self.output.name, chainDefinition, flatten=True)
                         butler.removeRuns([replaced], unstore=True)
@@ -614,74 +618,71 @@
 
             # pipeline can not be provided in this case
             if pipeline:
                 raise ValueError("Pipeline must not be given when quantum graph is read from file.")
             if args.show_qgraph_header:
                 print(QuantumGraph.readHeader(args.qgraph))
         else:
-            task_defs = list(pipeline.toExpandedPipeline())
+            pipeline_graph = pipeline.to_graph()
             if args.mock:
-                from lsst.pipe.base.tests.mocks import mock_task_defs
+                from lsst.pipe.base.tests.mocks import mock_pipeline_graph
 
-                task_defs = mock_task_defs(
-                    task_defs,
+                pipeline_graph = mock_pipeline_graph(
+                    pipeline_graph,
                     unmocked_dataset_types=args.unmocked_dataset_types,
                     force_failures=args.mock_failure,
                 )
             # make execution plan (a.k.a. DAG) for pipeline
-            graphBuilder = GraphBuilder(
-                butler.registry,
-                skipExistingIn=args.skip_existing_in,
-                clobberOutputs=args.clobber_outputs,
-                datastore=butler._datastore if args.qgraph_datastore_records else None,
+            graph_builder = AllDimensionsQuantumGraphBuilder(
+                pipeline_graph,
+                butler,
+                where=args.data_query,
+                skip_existing_in=args.skip_existing_in if args.skip_existing_in is not None else (),
+                clobber=args.clobber_outputs,
+                dataset_query_constraint=args.dataset_query_constraint,
+                input_collections=collections,
+                output_run=run,
             )
             # accumulate metadata
             metadata = {
                 "input": args.input,
                 "output": args.output,
                 "butler_argument": args.butler_config,
                 "output_run": run,
                 "extend_run": args.extend_run,
                 "skip_existing_in": args.skip_existing_in,
                 "skip_existing": args.skip_existing,
                 "data_query": args.data_query,
-                "user": getpass.getuser(),
-                "time": f"{datetime.datetime.now()}",
             }
             assert run is not None, "Butler output run collection must be defined"
-            qgraph = graphBuilder.makeGraph(
-                task_defs,
-                collections,
-                run,
-                args.data_query,
-                metadata=metadata,
-                datasetQueryConstraint=args.dataset_query_constraint,
-                dataId=pipeline.get_data_id(butler.dimensions),
-            )
+            qgraph = graph_builder.build(metadata, attach_datastore_records=args.qgraph_datastore_records)
             if args.show_qgraph_header:
                 qgraph.buildAndPrintHeader()
 
         if len(qgraph) == 0:
             # Nothing to do.
             return None
         self._summarize_qgraph(qgraph)
 
         if args.save_qgraph:
+            _LOG.verbose("Writing QuantumGraph to %r.", args.save_qgraph)
             qgraph.saveUri(args.save_qgraph)
 
         if args.save_single_quanta:
             for quantumNode in qgraph:
                 sqgraph = qgraph.subset(quantumNode)
                 uri = args.save_single_quanta.format(quantumNode)
                 sqgraph.saveUri(uri)
 
         if args.qgraph_dot:
+            _LOG.verbose("Writing quantum graph DOT visualization to %r.", args.qgraph_dot)
             graph2dot(qgraph, args.qgraph_dot)
 
         if args.execution_butler_location:
+            _LOG.verbose("Writing execution butler to %r.", args.execution_butler_location)
             butler = Butler.from_config(args.butler_config)
             assert isinstance(butler, DirectButler), "Execution butler needs DirectButler"
             newArgs = copy.deepcopy(args)
 
             def builderShim(butler: Butler) -> Butler:
                 assert isinstance(butler, DirectButler), "Execution butler needs DirectButler"
                 newArgs.butler_config = butler._config
@@ -771,15 +772,15 @@
             args.skip_existing = True
         else:
             args.clobber_outputs = False
 
         # Make butler instance. QuantumGraph should have an output run defined,
         # but we ignore it here and let command line decide actual output run.
         if butler is None:
-            butler = _ButlerFactory.makeWriteButler(args, graph.iterTaskGraph())
+            butler = _ButlerFactory.makeWriteButler(args, graph.pipeline_graph)
 
         if args.skip_existing:
             args.skip_existing_in += (butler.run,)
 
         # Enable lsstDebug debugging. Note that this is done once in the
         # main process before PreExecInit and it is also repeated before
         # running each task in SingleQuantumExecutor (which may not be
@@ -833,33 +834,28 @@
                 if args.summary:
                     report = executor.getReport()
                     if report:
                         with open(args.summary, "w") as out:
                             # Do not save fields that are not set.
                             out.write(report.model_dump_json(exclude_none=True, indent=2))
 
-    def _generateTaskTable(self, qgraph: QuantumGraph) -> Table:
+    def _generateTaskTable(self) -> Table:
         """Generate astropy table listing the number of quanta per task for a
         given quantum graph.
 
-        Parameters
-        ----------
-        qgraph : `lsst.pipe.base.graph.graph.QuantumGraph`
-            A QuantumGraph object.
-
         Returns
         -------
         qg_task_table : `astropy.table.table.Table`
             An astropy table containing columns: Quanta and Tasks.
         """
         qg_quanta, qg_tasks = [], []
-        for task_def in qgraph.iterTaskGraph():
-            num_qnodes = qgraph.getNumberOfQuantaForTask(task_def)
-            qg_quanta.append(num_qnodes)
-            qg_tasks.append(task_def.label)
+        for task_label, task_info in self.report.qgraphSummary.qgraphTaskSummaries.items():
+            qg_tasks.append(task_label)
+            qg_quanta.append(task_info.numQuanta)
+
         qg_task_table = Table(dict(Quanta=qg_quanta, Tasks=qg_tasks))
         return qg_task_table
 
     def _summarize_qgraph(self, qgraph: QuantumGraph) -> int:
         """Report a summary of the quanta in the graph.
 
         Parameters
@@ -872,16 +868,17 @@
         n_quanta : `int`
             The number of quanta in the graph.
         """
         n_quanta = len(qgraph)
         if n_quanta == 0:
             _LOG.info("QuantumGraph contains no quanta.")
         else:
+            self.report = Report(qgraphSummary=qgraph.getSummary())
             if _LOG.isEnabledFor(logging.INFO):
-                qg_task_table = self._generateTaskTable(qgraph)
+                qg_task_table = self._generateTaskTable()
                 qg_task_table_formatted = "\n".join(qg_task_table.pformat_all())
                 quanta_str = "quantum" if n_quanta == 1 else "quanta"
                 n_tasks = len(qgraph.taskGraph)
                 n_tasks_plural = "" if n_tasks == 1 else "s"
                 _LOG.info(
                     "QuantumGraph contains %d %s for %d task%s, graph ID: %r\n%s",
                     n_quanta,
@@ -996,14 +993,16 @@
         quantumExecutor = SingleQuantumExecutor(
             butler=None,
             taskFactory=task_factory,
             enableLsstDebug=args.enableLsstDebug,
             exitOnKnownError=args.fail_fast,
             limited_butler_factory=_butler_factory,
             resources=resources,
+            clobberOutputs=True,
+            skipExisting=True,
         )
 
         timeout = self.MP_TIMEOUT if args.timeout is None else args.timeout
         executor = MPGraphExecutor(
             numProc=args.processes,
             timeout=timeout,
             startMethod=args.start_method,
@@ -1016,8 +1015,8 @@
                 executor.execute(qgraph)
         finally:
             if args.summary:
                 report = executor.getReport()
                 if report:
                     with open(args.summary, "w") as out:
                         # Do not save fields that are not set.
-                        out.write(report.json(exclude_none=True, indent=2))
+                        out.write(report.model_dump_json(exclude_none=True, indent=2))
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/dotTools.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/dotTools.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 # -------------------------------
 #  Imports of standard modules --
 # -------------------------------
 import html
 import io
 import re
+import warnings
 from collections.abc import Iterable
 from typing import TYPE_CHECKING, Any
 
 # -----------------------------
 #  Imports for other modules --
 # -----------------------------
 from lsst.daf.butler import DatasetType, DimensionUniverse
@@ -276,15 +277,19 @@
     print("digraph Pipeline {", file=file)
     _renderDefault("graph", _ATTRIBS["defaultGraph"], file)
     _renderDefault("node", _ATTRIBS["defaultNode"], file)
     _renderDefault("edge", _ATTRIBS["defaultEdge"], file)
 
     allDatasets: set[str | tuple[str, str]] = set()
     if isinstance(pipeline, Pipeline):
-        pipeline = pipeline.toExpandedPipeline()
+        # TODO: DM-40639 will rewrite this code and finish off the deprecation
+        # of toExpandedPipeline.
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", category=FutureWarning)
+            pipeline = pipeline.toExpandedPipeline()
 
     # The next two lines are a workaround until DM-29658 at which time metadata
     # connections should start working with the above code
     labelToTaskName = {}
     metadataNodesToLink = set()
 
     for idx, taskDef in enumerate(sorted(pipeline, key=lambda x: x.label)):
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/execFixupDataId.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/execFixupDataId.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/log_capture.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/log_capture.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,21 +29,24 @@
 
 __all__ = ["LogCapture"]
 
 import logging
 import os
 import shutil
 import tempfile
+import warnings
 from collections.abc import Iterator
 from contextlib import contextmanager, suppress
 from logging import FileHandler
 
 from lsst.daf.butler import Butler, FileDataset, LimitedButler, Quantum
 from lsst.daf.butler.logging import ButlerLogRecordHandler, ButlerLogRecords, ButlerMDC, JsonLogFormatter
 from lsst.pipe.base import InvalidQuantumError, TaskDef
+from lsst.pipe.base.pipeline_graph import TaskNode
+from lsst.utils.introspection import find_outside_stacklevel
 
 _LOG = logging.getLogger(__name__)
 
 
 class _LogCaptureFlag:
     """Simple flag to enable/disable log-to-butler saving."""
 
@@ -81,91 +84,109 @@
         return cls(butler, None)
 
     @classmethod
     def from_full(cls, butler: Butler) -> LogCapture:
         return cls(butler, butler)
 
     @contextmanager
-    def capture_logging(self, taskDef: TaskDef, quantum: Quantum) -> Iterator[_LogCaptureFlag]:
+    def capture_logging(
+        self, task_node: TaskDef | TaskNode, /, quantum: Quantum
+    ) -> Iterator[_LogCaptureFlag]:
         """Configure logging system to capture logs for execution of this task.
 
         Parameters
         ----------
-        taskDef : `lsst.pipe.base.TaskDef`
-            The task definition.
+        task_node : `lsst.pipe.base.TaskDef` or \
+                `~lsst.pipe.base.pipeline_graph.TaskNode`
+            The task definition.  Support for `~lsst.pipe.base.TaskDef` is
+            deprecated and will be removed after v27.
         quantum : `~lsst.daf.butler.Quantum`
             Single Quantum instance.
 
         Notes
         -----
         Expected to be used as a context manager to ensure that logging
         records are inserted into the butler once the quantum has been
         executed:
 
         .. code-block:: py
 
-           with self.capture_logging(taskDef, quantum):
+           with self.capture_logging(task_node, quantum):
                # Run quantum and capture logs.
 
         Ths method can also setup logging to attach task- or
         quantum-specific information to log messages. Potentially this can
         take into account some info from task configuration as well.
         """
         # include quantum dataId and task label into MDC
-        mdc = {"LABEL": taskDef.label, "RUN": ""}
+        mdc = {"LABEL": task_node.label, "RUN": ""}
         if quantum.dataId:
             mdc["LABEL"] += f":{quantum.dataId}"
         if self.full_butler is not None:
             mdc["RUN"] = self.full_butler.run or ""
         ctx = _LogCaptureFlag()
 
+        if isinstance(task_node, TaskDef):
+            # TODO: remove this block and associated docs and annotations on
+            # DM-40443.
+            log_dataset_name = task_node.logOutputDatasetName
+            warnings.warn(
+                "Passing TaskDef instances to LogCapture is deprecated and will not be supported after v27.",
+                FutureWarning,
+                find_outside_stacklevel("lsst.ctrl.mpexec"),
+            )
+        else:
+            log_dataset_name = (
+                task_node.log_output.dataset_type_name if task_node.log_output is not None else None
+            )
+
         # Add a handler to the root logger to capture execution log output.
-        if taskDef.logOutputDatasetName is not None:
+        if log_dataset_name is not None:
             # Either accumulate into ButlerLogRecords or stream JSON records to
             # file and ingest that (ingest is possible only with full butler).
             if self.stream_json_logs and self.full_butler is not None:
                 # Create the log file in a temporary directory rather than
                 # creating a temporary file. This is necessary because
                 # temporary files are created with restrictive permissions
                 # and during file ingest these permissions persist in the
                 # datastore. Using a temp directory allows us to create
                 # a file with umask default permissions.
                 tmpdir = tempfile.mkdtemp(prefix="butler-temp-logs-")
 
                 # Construct a file to receive the log records and "touch" it.
-                log_file = os.path.join(tmpdir, f"butler-log-{taskDef.label}.json")
+                log_file = os.path.join(tmpdir, f"butler-log-{task_node.label}.json")
                 with open(log_file, "w"):
                     pass
                 log_handler_file = FileHandler(log_file)
                 log_handler_file.setFormatter(JsonLogFormatter())
                 logging.getLogger().addHandler(log_handler_file)
 
                 try:
                     with ButlerMDC.set_mdc(mdc):
                         yield ctx
                 finally:
                     # Ensure that the logs are stored in butler.
                     logging.getLogger().removeHandler(log_handler_file)
                     log_handler_file.close()
                     if ctx.store:
-                        self._ingest_log_records(quantum, taskDef.logOutputDatasetName, log_file)
+                        self._ingest_log_records(quantum, log_dataset_name, log_file)
                     shutil.rmtree(tmpdir, ignore_errors=True)
 
             else:
                 log_handler_memory = ButlerLogRecordHandler()
                 logging.getLogger().addHandler(log_handler_memory)
 
                 try:
                     with ButlerMDC.set_mdc(mdc):
                         yield ctx
                 finally:
                     # Ensure that the logs are stored in butler.
                     logging.getLogger().removeHandler(log_handler_memory)
                     if ctx.store:
-                        self._store_log_records(quantum, taskDef.logOutputDatasetName, log_handler_memory)
+                        self._store_log_records(quantum, log_dataset_name, log_handler_memory)
                     log_handler_memory.records.clear()
 
         else:
             with ButlerMDC.set_mdc(mdc):
                 yield ctx
 
     def _store_log_records(
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/mpGraphExecutor.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/mpGraphExecutor.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,16 +39,17 @@
 import threading
 import time
 from collections.abc import Iterable
 from enum import Enum
 from typing import Literal
 
 from lsst.daf.butler.cli.cliLog import CliLog
-from lsst.pipe.base import InvalidQuantumError, TaskDef
+from lsst.pipe.base import InvalidQuantumError
 from lsst.pipe.base.graph.graph import QuantumGraph, QuantumNode
+from lsst.pipe.base.pipeline_graph import TaskNode
 from lsst.utils.threads import disable_implicit_threading
 
 from .executionGraphFixup import ExecutionGraphFixup
 from .quantumGraphExecutor import QuantumExecutor, QuantumGraphExecutor
 from .reports import ExecutionStatus, QuantumReport, Report
 
 _LOG = logging.getLogger(__name__)
@@ -110,45 +111,45 @@
             Executor for single quantum.
         startMethod : `str`, optional
             Start method from `multiprocessing` module.
         """
         # Unpickling of quantum has to happen after butler/executor, this is
         # why it is pickled manually here.
         quantum_pickle = pickle.dumps(self.qnode.quantum)
-        taskDef = self.qnode.taskDef
+        task_node = self.qnode.task_node
         self._rcv_conn, snd_conn = multiprocessing.Pipe(False)
         logConfigState = CliLog.configState
 
         mp_ctx = multiprocessing.get_context(startMethod)
         self.process = mp_ctx.Process(  # type: ignore[attr-defined]
             target=_Job._executeJob,
-            args=(quantumExecutor, taskDef, quantum_pickle, logConfigState, snd_conn),
+            args=(quantumExecutor, task_node, quantum_pickle, logConfigState, snd_conn),
             name=f"task-{self.qnode.quantum.dataId}",
         )
         # mypy is getting confused by multiprocessing.
         assert self.process is not None
         self.process.start()
         self.started = time.time()
         self._state = JobState.RUNNING
 
     @staticmethod
     def _executeJob(
         quantumExecutor: QuantumExecutor,
-        taskDef: TaskDef,
+        task_node: TaskNode,
         quantum_pickle: bytes,
         logConfigState: list,
         snd_conn: multiprocessing.connection.Connection,
     ) -> None:
         """Execute a job with arguments.
 
         Parameters
         ----------
         quantumExecutor : `QuantumExecutor`
             Executor for single quantum.
-        taskDef : `bytes`
+        task_node : `lsst.pipe.base.pipeline_graph.TaskNode`
             Task definition structure.
         quantum_pickle : `bytes`
             Quantum for this task execution in pickled form.
         snd_conn : `multiprocessing.Connection`
             Connection to send job report to parent process.
         """
         # This terrible hack is a workaround for Python threading bug:
@@ -163,15 +164,15 @@
         if logConfigState and not CliLog.configState:
             # means that we are in a new spawned Python process and we have to
             # re-initialize logging
             CliLog.replayConfigState(logConfigState)
 
         quantum = pickle.loads(quantum_pickle)
         try:
-            quantumExecutor.execute(taskDef, quantum)
+            quantumExecutor.execute(task_node, quantum)
         finally:
             # If sending fails we do not want this new exception to be exposed.
             try:
                 report = quantumExecutor.getReport()
                 snd_conn.send(report)
             except Exception:
                 pass
@@ -212,15 +213,15 @@
             # Likely due to the process killed, but there may be other reasons.
             # Exit code should not be None, this is to keep mypy happy.
             exitcode = self.process.exitcode if self.process.exitcode is not None else -1
             assert self.qnode.quantum.dataId is not None, "Quantum DataId cannot be None"
             report = QuantumReport.from_exit_code(
                 exitCode=exitcode,
                 dataId=self.qnode.quantum.dataId,
-                taskLabel=self.qnode.taskDef.label,
+                taskLabel=self.qnode.task_node.label,
             )
         if self.terminated:
             # Means it was killed, assume it's due to timeout
             report.status = ExecutionStatus.TIMEOUT
         return report
 
     def failMessage(self) -> str:
@@ -241,15 +242,15 @@
         elif exitcode > 0:
             msg = f"Task {self} failed, exit code={exitcode}"
         else:
             msg = ""
         return msg
 
     def __str__(self) -> str:
-        return f"<{self.qnode.taskDef} dataId={self.qnode.quantum.dataId}>"
+        return f"<{self.qnode.task_node.label} dataId={self.qnode.quantum.dataId}>"
 
 
 class _JobList:
     """Simple list of _Job instances with few convenience methods.
 
     Parameters
     ----------
@@ -399,15 +400,15 @@
         if startMethod is None:
             startMethod = "spawn"
         self.startMethod = startMethod
 
     def execute(self, graph: QuantumGraph) -> None:
         # Docstring inherited from QuantumGraphExecutor.execute
         graph = self._fixupQuanta(graph)
-        self.report = Report()
+        self.report = Report(qgraphSummary=graph.getSummary())
         try:
             if self.numProc > 1:
                 self._executeQuantaMP(graph, self.report)
             else:
                 self._executeQuantaInProcess(graph, self.report)
         except Exception as exc:
             self.report.set_exception(exc)
@@ -454,39 +455,42 @@
         report : `Report`
             Object for reporting execution status.
         """
         successCount, totalCount = 0, len(graph)
         failedNodes: set[QuantumNode] = set()
         for qnode in graph:
             assert qnode.quantum.dataId is not None, "Quantum DataId cannot be None"
+            task_node = qnode.task_node
 
             # Any failed inputs mean that the quantum has to be skipped.
             inputNodes = graph.determineInputsToQuantumNode(qnode)
             if inputNodes & failedNodes:
                 _LOG.error(
                     "Upstream job failed for task <%s dataId=%s>, skipping this task.",
-                    qnode.taskDef,
+                    task_node.label,
                     qnode.quantum.dataId,
                 )
                 failedNodes.add(qnode)
                 failed_quantum_report = QuantumReport(
-                    status=ExecutionStatus.SKIPPED, dataId=qnode.quantum.dataId, taskLabel=qnode.taskDef.label
+                    status=ExecutionStatus.SKIPPED,
+                    dataId=qnode.quantum.dataId,
+                    taskLabel=task_node.label,
                 )
                 report.quantaReports.append(failed_quantum_report)
                 continue
 
             _LOG.debug("Executing %s", qnode)
             try:
-                self.quantumExecutor.execute(qnode.taskDef, qnode.quantum)
+                self.quantumExecutor.execute(task_node, qnode.quantum)
                 successCount += 1
             except Exception as exc:
                 if self.pdb and sys.stdin.isatty() and sys.stdout.isatty():
                     _LOG.error(
                         "Task <%s dataId=%s> failed; dropping into pdb.",
-                        qnode.taskDef,
+                        task_node.label,
                         qnode.quantum.dataId,
                         exc_info=exc,
                     )
                     try:
                         pdb = importlib.import_module(self.pdb)
                     except ImportError as imp_exc:
                         raise MPGraphExecutorError(
@@ -497,22 +501,22 @@
                             f"Specified debugger module ({self.pdb}) can't debug with post_mortem",
                         ) from exc
                     pdb.post_mortem(exc.__traceback__)
                 failedNodes.add(qnode)
                 report.status = ExecutionStatus.FAILURE
                 if self.failFast:
                     raise MPGraphExecutorError(
-                        f"Task <{qnode.taskDef} dataId={qnode.quantum.dataId}> failed."
+                        f"Task <{task_node.label} dataId={qnode.quantum.dataId}> failed."
                     ) from exc
                 else:
                     # Note that there could be exception safety issues, which
                     # we presently ignore.
                     _LOG.error(
                         "Task <%s dataId=%s> failed; processing will continue for remaining tasks.",
-                        qnode.taskDef,
+                        task_node.label,
                         qnode.quantum.dataId,
                         exc_info=exc,
                     )
             finally:
                 # sqlalchemy has some objects that can last until a garbage
                 # collection cycle is run, which can happen at unpredictable
                 # times, run a collection loop here explicitly.
@@ -549,18 +553,18 @@
         _LOG.debug("Using %r for multiprocessing start method", self.startMethod)
 
         # re-pack input quantum data into jobs list
         jobs = _JobList(graph)
 
         # check that all tasks can run in sub-process
         for job in jobs.jobs:
-            taskDef = job.qnode.taskDef
-            if not taskDef.taskClass.canMultiprocess:
+            task_node = job.qnode.task_node
+            if not task_node.task_class.canMultiprocess:
                 raise MPGraphExecutorError(
-                    f"Task {taskDef.taskName} does not support multiprocessing; use single process"
+                    f"Task {task_node.label!r} does not support multiprocessing; use single process"
                 )
 
         finishedCount, failedCount = 0, 0
         while jobs.pending or jobs.running:
             _LOG.debug("#pendingJobs: %s", len(jobs.pending))
             _LOG.debug("#runningJobs: %s", len(jobs.running))
 
@@ -621,15 +625,15 @@
                 for job in jobs.pending:
                     jobInputNodes = graph.determineInputsToQuantumNode(job.qnode)
                     assert job.qnode.quantum.dataId is not None, "Quantum DataId cannot be None"
                     if jobInputNodes & jobs.failedNodes:
                         quantum_report = QuantumReport(
                             status=ExecutionStatus.SKIPPED,
                             dataId=job.qnode.quantum.dataId,
-                            taskLabel=job.qnode.taskDef.label,
+                            taskLabel=job.qnode.task_node.label,
                         )
                         report.quantaReports.append(quantum_report)
                         jobs.setJobState(job, JobState.FAILED_DEP)
                         _LOG.error("Upstream job failed for task %s, skipping this task.", job)
 
             # see if we can start more jobs
             if len(jobs.running) < self.numProc:
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/preExecInit.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/preExecInit.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,17 +38,19 @@
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Any
 
 # -----------------------------
 #  Imports for other modules --
 # -----------------------------
 from lsst.daf.butler import DatasetRef, DatasetType
-from lsst.daf.butler.registry import ConflictingDefinitionError
-from lsst.pipe.base import PipelineDatasetTypes
-from lsst.pipe.base import automatic_connection_constants as acc
+from lsst.daf.butler.registry import ConflictingDefinitionError, MissingDatasetTypeError
+from lsst.pipe.base.automatic_connection_constants import (
+    PACKAGES_INIT_OUTPUT_NAME,
+    PACKAGES_INIT_OUTPUT_STORAGE_CLASS,
+)
 from lsst.utils.packages import Packages
 
 if TYPE_CHECKING:
     from lsst.daf.butler import Butler, LimitedButler
     from lsst.pipe.base import QuantumGraph, TaskDef, TaskFactory
 
 _LOG = logging.getLogger(__name__)
@@ -179,15 +181,17 @@
         TypeError
             Raised if the type of existing object in butler is different from
             new data.
         """
         _LOG.debug("Will save InitOutputs for all tasks")
         for taskDef in self._task_iter(graph):
             init_input_refs = graph.initInputRefs(taskDef) or []
-            task = self.taskFactory.makeTask(taskDef, self.butler, init_input_refs)
+            task = self.taskFactory.makeTask(
+                graph.pipeline_graph.tasks[taskDef.label], self.butler, init_input_refs
+            )
             for name in taskDef.connections.initOutputs:
                 attribute = getattr(taskDef.connections, name)
                 init_output_refs = graph.initOutputRefs(taskDef) or []
                 init_output_ref, obj_from_store = self._find_dataset(init_output_refs, attribute.name)
                 if init_output_ref is None:
                     raise ValueError(f"Cannot find dataset reference for init output {name} in a graph")
                 init_output_var = getattr(task, name)
@@ -283,15 +287,15 @@
 
         # start transaction to rollback any changes on exceptions
         with self.transaction():
             # Packages dataset ref is stored in graph's global init outputs,
             # but it may be also be missing.
 
             packages_ref, old_packages = self._find_dataset(
-                graph.globalInitOutputRefs(), PipelineDatasetTypes.packagesDatasetName
+                graph.globalInitOutputRefs(), PACKAGES_INIT_OUTPUT_NAME
             )
             if packages_ref is None:
                 return
 
             if old_packages is not None:
                 # Note that because we can only detect python modules that have
                 # been imported, the stored list of products may be more or
@@ -402,105 +406,62 @@
     def transaction(self) -> Iterator[None]:
         # dosctring inherited
         with self.full_butler.transaction():
             yield
 
     def initializeDatasetTypes(self, graph: QuantumGraph, registerDatasetTypes: bool = False) -> None:
         # docstring inherited
-        pipeline = graph.taskGraph
-        pipelineDatasetTypes = PipelineDatasetTypes.fromPipeline(
-            pipeline, registry=self.full_butler.registry, include_configs=True, include_packages=True
+        missing_dataset_types: set[str] = set()
+        dataset_types = [node.dataset_type for node in graph.pipeline_graph.dataset_types.values()]
+        dataset_types.append(
+            DatasetType(
+                PACKAGES_INIT_OUTPUT_NAME, self.butler.dimensions.empty, PACKAGES_INIT_OUTPUT_STORAGE_CLASS
+            )
         )
-        # The "registry dataset types" saved with the QG have had their storage
-        # classes carefully resolved by PipelineGraph, whereas the dataset
-        # types from PipelineDatasetTypes are a mess because it uses
-        # NamedValueSet and that ignores storage classes.  It will be fully
-        # removed here (and deprecated everywhere) on DM-40441.
-        # Note that these "registry dataset types" include dataset types that
-        # are not actually registered yet; they're the PipelineGraph's
-        # determination of what _should_ be registered.
-        registry_storage_classes = {
-            dataset_type.name: dataset_type.storageClass_name for dataset_type in graph.registryDatasetTypes()
-        }
-        registry_storage_classes[acc.PACKAGES_INIT_OUTPUT_NAME] = acc.PACKAGES_INIT_OUTPUT_STORAGE_CLASS
-        dataset_types: Iterable[DatasetType]
-        for dataset_types, is_input in (
-            (pipelineDatasetTypes.initIntermediates, True),
-            (pipelineDatasetTypes.initOutputs, False),
-            (pipelineDatasetTypes.intermediates, True),
-            (pipelineDatasetTypes.outputs, False),
-        ):
-            dataset_types = [
-                (
-                    # The registry dataset types do not include components, but
-                    # we don't support storage class overrides for those in
-                    # other contexts anyway, and custom-built QGs may not have
-                    # the registry dataset types field populated at all.x
-                    dataset_type.overrideStorageClass(registry_storage_classes[dataset_type.name])
-                    if dataset_type.name in registry_storage_classes
-                    else dataset_type
-                )
-                for dataset_type in dataset_types
-            ]
-            self._register_output_dataset_types(registerDatasetTypes, dataset_types, is_input)
-
-    def _register_output_dataset_types(
-        self, registerDatasetTypes: bool, datasetTypes: Iterable[DatasetType], is_input: bool
-    ) -> None:
-        def _check_compatibility(datasetType: DatasetType, expected: DatasetType, is_input: bool) -> bool:
-            # These are output dataset types so check for compatibility on put.
-            is_compatible = expected.is_compatible_with(datasetType)
-
-            if is_input:
-                # This dataset type is also used for input so must be
-                # compatible on get as ell.
-                is_compatible = is_compatible and datasetType.is_compatible_with(expected)
-
-            if is_compatible:
-                _LOG.debug(
-                    "The dataset type configurations differ (%s from task != %s from registry) "
-                    "but the storage classes are compatible. Can continue.",
-                    datasetType,
-                    expected,
-                )
-            return is_compatible
-
-        missing_datasetTypes = set()
-        for datasetType in datasetTypes:
-            # Only composites are registered, no components, and by this point
-            # the composite should already exist.
-            if registerDatasetTypes and not datasetType.isComponent():
-                _LOG.debug("Registering DatasetType %s with registry", datasetType)
-                # this is a no-op if it already exists and is consistent,
-                # and it raises if it is inconsistent.
+        for dataset_type in dataset_types:
+            # Resolving the PipelineGraph when building the QuantumGraph should
+            # have already guaranteed that this is the registry dataset type
+            # and that all references to it use compatible storage classes,
+            # so we don't need another check for compatibility here; if the
+            # dataset type doesn't match the registry that's already a problem.
+            if registerDatasetTypes:
+                _LOG.debug("Registering DatasetType %s with registry", dataset_type.name)
                 try:
-                    self.full_butler.registry.registerDatasetType(datasetType)
+                    self.full_butler.registry.registerDatasetType(dataset_type)
                 except ConflictingDefinitionError:
-                    if not _check_compatibility(
-                        datasetType, self.full_butler.get_dataset_type(datasetType.name), is_input
-                    ):
-                        raise
+                    expected = self.full_butler.registry.getDatasetType(dataset_type.name)
+                    raise ConflictingDefinitionError(
+                        f"DatasetType definition in registry has changed since the QuantumGraph was built: "
+                        f"{dataset_type} (graph) != {expected} (registry)."
+                    )
             else:
-                _LOG.debug("Checking DatasetType %s against registry", datasetType)
+                _LOG.debug("Checking DatasetType %s against registry", dataset_type.name)
                 try:
-                    expected = self.full_butler.get_dataset_type(datasetType.name)
-                except KeyError:
-                    # Likely means that --register-dataset-types is forgotten.
-                    missing_datasetTypes.add(datasetType.name)
+                    expected = self.full_butler.registry.getDatasetType(dataset_type.name)
+                except MissingDatasetTypeError:
+                    # Likely means that --register-dataset-types is forgotten,
+                    # but we could also get here if there is a prerequisite
+                    # input that is optional and none were found in this repo;
+                    # that is not an error.  And we don't bother to check if
+                    # they are optional here, since the fact that we were able
+                    # to make the QG says that they were, since there couldn't
+                    # have been any datasets if the dataset types weren't
+                    # registered.
+                    if not graph.pipeline_graph.dataset_types[dataset_type.name].is_prerequisite:
+                        missing_dataset_types.add(dataset_type.name)
                     continue
-                if expected != datasetType:
-                    if not _check_compatibility(datasetType, expected, is_input):
-                        raise ValueError(
-                            f"DatasetType configuration does not match Registry: {datasetType} != {expected}"
-                        )
-
-        if missing_datasetTypes:
-            plural = "s" if len(missing_datasetTypes) != 1 else ""
-            raise KeyError(
-                f"Missing dataset type definition{plural}: {', '.join(missing_datasetTypes)}. "
+                if expected != dataset_type:
+                    raise ConflictingDefinitionError(
+                        f"DatasetType definition in registry has changed since the QuantumGraph was built: "
+                        f"{dataset_type} (graph) != {expected} (registry)."
+                    )
+        if missing_dataset_types:
+            plural = "s" if len(missing_dataset_types) != 1 else ""
+            raise MissingDatasetTypeError(
+                f"Missing dataset type definition{plural}: {', '.join(missing_dataset_types)}. "
                 "Dataset types have to be registered with either `butler register-dataset-type` or "
                 "passing `--register-dataset-types` option to `pipetask run`."
             )
 
 
 class PreExecInitLimited(PreExecInitBase):
     """Initialization of registry for QuantumGraph execution.
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/quantumGraphExecutor.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/quantumGraphExecutor.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,33 +33,36 @@
 from typing import TYPE_CHECKING
 
 from .reports import QuantumReport, Report
 
 if TYPE_CHECKING:
     from lsst.daf.butler import Quantum
     from lsst.pipe.base import QuantumGraph, TaskDef
+    from lsst.pipe.base.pipeline_graph import TaskNode
 
 
 class QuantumExecutor(ABC):
     """Class which abstracts execution of a single Quantum.
 
     In general implementation should not depend on execution model and
     execution should always happen in-process. Main reason for existence
     of this class is to provide do-nothing implementation that can be used
     in the unit tests.
     """
 
     @abstractmethod
-    def execute(self, taskDef: TaskDef, quantum: Quantum) -> Quantum:
+    def execute(self, task_node: TaskNode | TaskDef, /, quantum: Quantum) -> Quantum:
         """Execute single quantum.
 
         Parameters
         ----------
-        taskDef : `~lsst.pipe.base.TaskDef`
-            Task definition structure.
+        task_node : `~lsst.pipe.base.TaskDef` or \
+                `~lsst.pipe.base.pipeline_graph.TaskNode`
+            Task definition structure.  `~lsst.pipe.base.TaskDef` support is
+            deprecated and will be removed after v27.
         quantum : `~lsst.daf.butler.Quantum`
             Quantum for this execution.
 
         Returns
         -------
         quantum : `~lsst.daf.butler.Quantum`
             The quantum actually executed.
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/reports.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 import enum
 import sys
 from typing import Any
 
 import pydantic
 from lsst.daf.butler import DataCoordinate, DataId, DataIdValue
+from lsst.pipe.base import QgraphSummary
 from lsst.utils.introspection import get_full_type_name
 
 
 def _serializeDataId(dataId: DataId) -> dict[str, DataIdValue]:
     if isinstance(dataId, DataCoordinate):
         return dict(dataId.required)
     else:
@@ -191,14 +192,17 @@
             exitCode=exitCode,
         )
 
 
 class Report(pydantic.BaseModel):
     """Execution report for the whole job with one or few quanta."""
 
+    qgraphSummary: QgraphSummary
+    """Summary report about QuantumGraph."""
+
     status: ExecutionStatus = ExecutionStatus.SUCCESS
     """Job status."""
 
     cmdLine: list[str] | None = None
     """Command line for the whole job."""
 
     exitCode: int | None = None
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/separablePipelineExecutor.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/separablePipelineExecutor.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,42 +32,45 @@
     "SeparablePipelineExecutor",
 ]
 
 
 import datetime
 import getpass
 import logging
+import warnings
 from collections.abc import Iterable, Mapping
 from typing import Any, Protocol
 
 import lsst.pipe.base
 import lsst.resources
 from lsst.daf.butler import Butler
+from lsst.pipe.base.all_dimensions_quantum_graph_builder import (
+    AllDimensionsQuantumGraphBuilder,
+    DatasetQueryConstraintVariant,
+)
+from lsst.pipe.base.quantum_graph_builder import QuantumGraphBuilder
+from lsst.utils.introspection import find_outside_stacklevel
 
 from .mpGraphExecutor import MPGraphExecutor
 from .preExecInit import PreExecInit
 from .quantumGraphExecutor import QuantumGraphExecutor
 from .singleQuantumExecutor import SingleQuantumExecutor
 from .taskFactory import TaskFactory
 
 _LOG = logging.getLogger(__name__)
 
 
-# Only way to keep black, flake8, and mypy all happy
-_dqc = lsst.pipe.base._datasetQueryConstraints
-
-
 class _GraphBuilderLike(Protocol):
     def makeGraph(
         self,
         pipeline: lsst.pipe.base.Pipeline | Iterable[lsst.pipe.base.pipeline.TaskDef],
         collections: Any,
         run: str,
         userQuery: str | None,
-        datasetQueryConstraint: _dqc.DatasetQueryConstraintVariant = _dqc._ALL,
+        datasetQueryConstraint: DatasetQueryConstraintVariant = DatasetQueryConstraintVariant.ALL,
         metadata: Mapping[str, Any] | None = None,
         bind: Mapping[str, Any] | None = None,
     ) -> lsst.pipe.base.QuantumGraph:
         pass
 
 
 class SeparablePipelineExecutor:
@@ -172,64 +175,104 @@
         -------
         pipeline : `lsst.pipe.base.Pipeline`
             The fully-built pipeline.
         """
         return lsst.pipe.base.Pipeline.from_uri(pipeline_uri)
 
     def make_quantum_graph(
-        self, pipeline: lsst.pipe.base.Pipeline, where: str = "", builder: _GraphBuilderLike | None = None
+        self,
+        pipeline: lsst.pipe.base.Pipeline,
+        where: str = "",
+        builder: _GraphBuilderLike | None = None,
+        *,
+        builder_class: type[QuantumGraphBuilder] = AllDimensionsQuantumGraphBuilder,
+        attach_datastore_records: bool = False,
+        **kwargs: Any,
     ) -> lsst.pipe.base.QuantumGraph:
         """Build a quantum graph from a pipeline and input datasets.
 
         Parameters
         ----------
         pipeline : `lsst.pipe.base.Pipeline`
             The pipeline for which to generate a quantum graph.
         where : `str`, optional
-            A data ID query that constrains the quanta generated.
+            A data ID query that constrains the quanta generated.  Must not be
+            provided if a custom ``builder_class`` is given and that class does
+            not accept ``where`` as a construction argument.
         builder : `lsst.pipe.base.GraphBuilder`-like, optional
             A graph builder that implements a
             `~lsst.pipe.base.GraphBuilder.makeGraph` method. By default, a new
-            instance of `lsst.pipe.base.GraphBuilder` is used.
+            instance of `lsst.pipe.base.GraphBuilder` is used.  Deprecated in
+            favor of ``builder_class`` and will be removed after v27.
+        builder_class : `type` [ \
+                `lsst.pipe.base.quantum_graph_builder.QuantumGraphBuilder` ], \
+                optional
+            Quantum graph builder implementation.  Ignored if ``builder`` is
+            provided.
+        attach_datastore_records : `bool`, optional
+            Whether to attach datastore records.  These are currently used only
+            by `lsst.daf.butler.QuantumBackedButler`, which is not used by
+            `SeparablePipelineExecutor` for execution.
+        **kwargs
+            Additional keyword arguments are forwarded to ``builder_class``
+            when a quantum graph builder instance is constructed.  All
+            arguments accepted by the
+            `~lsst.pipe.base.quantum_graph_builder.QuantumGraphBuilder` base
+            class are provided automatically (from explicit arguments to this
+            method and executor attributes) and do not need to be included
+            as keyword arguments.
 
         Returns
         -------
         graph : `lsst.pipe.base.QuantumGraph`
             The quantum graph for ``pipeline`` as run on the datasets
             identified by ``where``.
 
         Notes
         -----
         This method does no special handling of empty quantum graphs. If
         needed, clients can use `len` to test if the returned graph is empty.
         """
-        if not builder:
-            builder = lsst.pipe.base.GraphBuilder(
-                self._butler.registry,
-                skipExistingIn=self._skip_existing_in,
-                clobberOutputs=self._clobber_output,
-            )
-
         metadata = {
             "input": self._butler.collections,
             "output_run": self._butler.run,
             "skip_existing_in": self._skip_existing_in,
             "skip_existing": bool(self._skip_existing_in),
             "data_query": where,
             "user": getpass.getuser(),
             "time": str(datetime.datetime.now()),
         }
-        assert self._butler.run is not None, "Butler output run collection must be defined"
-        graph = builder.makeGraph(
-            pipeline,
-            self._butler.collections,
-            self._butler.run,
-            userQuery=where,
-            metadata=metadata,
-        )
+        if builder:
+            warnings.warn(
+                "The 'builder' argument to SeparablePipelineBuilder.make_quantum_graph "
+                "is deprecated in favor of 'builder_class', and will be removed after v27.",
+                FutureWarning,
+                find_outside_stacklevel("lsst.ctrl.mpexec"),
+            )
+            assert self._butler.run is not None, "Butler output run collection must be defined"
+            graph = builder.makeGraph(
+                pipeline,
+                self._butler.collections,
+                self._butler.run,
+                userQuery=where,
+                metadata=metadata,
+            )
+        else:
+            if where:
+                # Only pass 'where' if it's actually provided, since some
+                # QuantumGraphBuilder subclasses may not accept it.
+                kwargs["where"] = where
+            qg_builder = builder_class(
+                pipeline.to_graph(),
+                self._butler,
+                skip_existing_in=self._skip_existing_in,
+                clobber=self._clobber_output,
+                **kwargs,
+            )
+            graph = qg_builder.build(metadata=metadata, attach_datastore_records=attach_datastore_records)
         _LOG.info(
             "QuantumGraph contains %d quanta for %d tasks, graph ID: %r",
             len(graph),
             len(graph.taskGraph),
             graph.graphID,
         )
         return graph
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/showInfo.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/showInfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,21 +227,21 @@
             matConfig = re.search(r"^(?:(\w+)::)?(?:config.)?(.+)?", showArgs)
             assert matConfig is not None, "regex always matches"
             taskName = matConfig.group(1)
             pattern = matConfig.group(2)
             if pattern:
                 stream = _FilteredStream(pattern, stream=stream)
 
-        tasks = util.filterTasks(pipeline, taskName)
+        tasks = util.filterTaskNodes(pipeline.to_graph(), taskName)
         if not tasks:
             raise ValueError(f"Pipeline has no tasks named {taskName}")
 
-        for taskDef in tasks:
-            print(f"### Configuration for task `{taskDef.label}'", file=self.stream)
-            taskDef.config.saveToStream(stream, root="config", skipImports=not dumpFullConfig)
+        for task_node in tasks:
+            print(f"### Configuration for task `{task_node.label}'", file=self.stream)
+            task_node.config.saveToStream(stream, root="config", skipImports=not dumpFullConfig)
 
     def _showConfigHistory(self, pipeline: Pipeline, showArgs: str) -> None:
         """Show history for task configuration.
 
         Parameters
         ----------
         pipeline : `lsst.pipe.base.Pipeline`
@@ -254,64 +254,64 @@
         matHistory = re.search(r"^(?:(\w+)::)?(?:config[.])?(.+)", showArgs)
         if matHistory:
             taskName = matHistory.group(1)
             pattern = matHistory.group(2)
         if not pattern:
             raise ValueError("Please provide a value with --show history (e.g. history=Task::param)")
 
-        tasks = util.filterTasks(pipeline, taskName)
+        tasks = util.filterTaskNodes(pipeline.to_graph(), taskName)
         if not tasks:
             raise ValueError(f"Pipeline has no tasks named {taskName}")
 
         found = False
-        for taskDef in tasks:
-            config = taskDef.config
+        for task_node in tasks:
+            config = task_node.config
 
             # Look for any matches in the config hierarchy for this name
             for nmatch, thisName in enumerate(fnmatch.filter(config.names(), pattern)):
                 if nmatch > 0:
                     print("", file=self.stream)
 
                 cpath, _, cname = thisName.rpartition(".")
                 try:
                     if not cpath:
                         # looking for top-level field
-                        hconfig = taskDef.config
+                        hconfig = task_node.config
                     else:
                         hconfig = eval("config." + cpath, {}, {"config": config})
                 except AttributeError:
                     print(
-                        f"Error: Unable to extract attribute {cpath} from task {taskDef.label}",
+                        f"Error: Unable to extract attribute {cpath} from task {task_node.label}",
                         file=sys.stderr,
                     )
                     hconfig = None
 
                 # Sometimes we end up with a non-Config so skip those
                 if isinstance(hconfig, pexConfig.Config | pexConfig.ConfigurableInstance) and hasattr(
                     hconfig, cname
                 ):
-                    print(f"### Configuration field for task `{taskDef.label}'", file=self.stream)
+                    print(f"### Configuration field for task `{task_node.label}'", file=self.stream)
                     print(pexConfigHistory.format(hconfig, cname), file=self.stream)
                     found = True
 
         if not found:
             raise ValueError(f"None of the tasks has field matching {pattern}")
 
     def _showTaskHierarchy(self, pipeline: Pipeline) -> None:
         """Print task hierarchy to stdout
 
         Parameters
         ----------
         pipeline : `lsst.pipe.base.Pipeline`
             Pipeline definition.
         """
-        for taskDef in pipeline.toExpandedPipeline():
-            print(f"### Subtasks for task `{taskDef.taskName}'", file=self.stream)
+        for task_node in pipeline.to_graph().tasks.values():
+            print(f"### Subtasks for task `{task_node.task_class_name}'", file=self.stream)
 
-            for configName, taskName in util.subTaskIter(taskDef.config):
+            for configName, taskName in util.subTaskIter(task_node.config):
                 print(f"{configName}: {taskName}", file=self.stream)
 
     def _showGraph(self, graph: QuantumGraph) -> None:
         """Print quanta information to stdout
 
         Parameters
         ----------
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/simple_pipeline_executor.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/simple_pipeline_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,28 +25,31 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 __all__ = ("SimplePipelineExecutor",)
 
+import warnings
 from collections.abc import Iterable, Iterator, Mapping
 from typing import Any
 
 from lsst.daf.butler import Butler, CollectionType, Quantum
 from lsst.pex.config import Config
 from lsst.pipe.base import (
     ExecutionResources,
-    GraphBuilder,
     Instrument,
     Pipeline,
+    PipelineGraph,
     PipelineTask,
     QuantumGraph,
     TaskDef,
 )
+from lsst.pipe.base.all_dimensions_quantum_graph_builder import AllDimensionsQuantumGraphBuilder
+from lsst.utils.introspection import find_outside_stacklevel
 
 from .preExecInit import PreExecInit
 from .singleQuantumExecutor import SingleQuantumExecutor
 from .taskFactory import TaskFactory
 
 
 class SimplePipelineExecutor:
@@ -73,16 +76,16 @@
     consistently.
 
     This class is intended primarily to support unit testing and small-scale
     integration testing of `~lsst.pipe.base.PipelineTask` classes.  It
     deliberately lacks many features present in the command-line-only
     ``pipetask`` tool in order to keep the implementation simple.  Python
     callers that need more sophistication should call lower-level tools like
-    `~lsst.pipe.base.GraphBuilder`, `PreExecInit`, and `SingleQuantumExecutor`
-    directly.
+    `~lsst.pipe.base.quantum_graph_builder.QuantumGraphBuilder`, `PreExecInit`,
+    and `SingleQuantumExecutor` directly.
     """
 
     def __init__(
         self,
         quantum_graph: QuantumGraph,
         butler: Butler,
         resources: ExecutionResources | None = None,
@@ -225,66 +228,120 @@
         if label is None:
             label = task_class._DefaultName
         if not isinstance(config, task_class.ConfigClass):
             raise TypeError(
                 f"Invalid config class type: expected {task_class.ConfigClass.__name__}, "
                 f"got {type(config).__name__}."
             )
-        task_def = TaskDef(taskName=task_class.__name__, config=config, label=label, taskClass=task_class)
-        return cls.from_pipeline([task_def], butler=butler, where=where, bind=bind, resources=resources)
+        pipeline_graph = PipelineGraph()
+        pipeline_graph.add_task(label=label, task_class=task_class, config=config)
+        return cls.from_pipeline_graph(
+            pipeline_graph, butler=butler, where=where, bind=bind, resources=resources
+        )
 
     @classmethod
     def from_pipeline(
         cls,
         pipeline: Pipeline | Iterable[TaskDef],
         *,
         where: str = "",
         bind: Mapping[str, Any] | None = None,
         butler: Butler,
         resources: ExecutionResources | None = None,
-        **kwargs: Any,
     ) -> SimplePipelineExecutor:
         """Create an executor by building a QuantumGraph from an in-memory
         pipeline.
 
         Parameters
         ----------
         pipeline : `~lsst.pipe.base.Pipeline` or \
                 `~collections.abc.Iterable` [ `~lsst.pipe.base.TaskDef` ]
             A Python object describing the tasks to run, along with their
-            labels and configuration.
+            labels and configuration.  Passing `~lsst.pipe.base.TaskDef`
+            objects is deprecated and will not be supported after v27.
         where : `str`, optional
             Data ID query expression that constraints the quanta generated.
         bind : `~collections.abc.Mapping`, optional
             Mapping containing literal values that should be injected into the
             ``where`` expression, keyed by the identifiers they replace.
         butler : `~lsst.daf.butler.Butler`
             Butler that manages all I/O.  `prep_butler` can be used to create
             one.
         resources : `~lsst.pipe.base.ExecutionResources`
             The resources available to each quantum being executed.
-        **kwargs : `~typing.Any`
-            Unused.
 
         Returns
         -------
         executor : `SimplePipelineExecutor`
             An executor instance containing the constructed
             `~lsst.pipe.base.QuantumGraph` and `~lsst.daf.butler.Butler`,
             ready for `run` to be called.
         """
         if isinstance(pipeline, Pipeline):
-            pipeline = list(pipeline.toExpandedPipeline())
+            pipeline_graph = pipeline.to_graph()
         else:
-            pipeline = list(pipeline)
-        graph_builder = GraphBuilder(butler.registry)
-        assert butler.run is not None, "Butler output run collection must be defined"
-        quantum_graph = graph_builder.makeGraph(
-            pipeline, collections=butler.collections, run=butler.run, userQuery=where, bind=bind
+            # TODO: disable this block and adjust docs and annotations
+            # on DM-40443.
+            warnings.warn(
+                "Passing TaskDefs to SimplePipelineExecutor.from_pipeline is deprecated "
+                "and will be removed after v27.",
+                category=FutureWarning,
+                stacklevel=find_outside_stacklevel("lsst.ctrl.mpexec"),
+            )
+            pipeline_graph = PipelineGraph()
+            for task_def in pipeline:
+                pipeline_graph.add_task(
+                    task_def.label, task_def.taskClass, task_def.config, connections=task_def.connections
+                )
+        return cls.from_pipeline_graph(
+            pipeline_graph, where=where, bind=bind, butler=butler, resources=resources
         )
+
+    @classmethod
+    def from_pipeline_graph(
+        cls,
+        pipeline_graph: PipelineGraph,
+        *,
+        where: str = "",
+        bind: Mapping[str, Any] | None = None,
+        butler: Butler,
+        resources: ExecutionResources | None = None,
+    ) -> SimplePipelineExecutor:
+        """Create an executor by building a QuantumGraph from an in-memory
+        pipeline graph.
+
+        Parameters
+        ----------
+        pipeline_graph : `~lsst.pipe.base.PipelineGraph`
+            A Python object describing the tasks to run, along with their
+            labels and configuration, in graph form.  Will be resolved against
+            the given ``butler``, with any existing resolutions ignored.
+        where : `str`, optional
+            Data ID query expression that constraints the quanta generated.
+        bind : `~collections.abc.Mapping`, optional
+            Mapping containing literal values that should be injected into the
+            ``where`` expression, keyed by the identifiers they replace.
+        butler : `~lsst.daf.butler.Butler`
+            Butler that manages all I/O.  `prep_butler` can be used to create
+            one.  Must have its `~Butler.run` and `~Butler.collections` not
+            empty and not `None`.
+        resources : `~lsst.pipe.base.ExecutionResources`
+            The resources available to each quantum being executed.
+
+        Returns
+        -------
+        executor : `SimplePipelineExecutor`
+            An executor instance containing the constructed
+            `~lsst.pipe.base.QuantumGraph` and `~lsst.daf.butler.Butler`,
+            ready for `run` to be called.
+        """
+        quantum_graph_builder = AllDimensionsQuantumGraphBuilder(
+            pipeline_graph, butler, where=where, bind=bind
+        )
+        quantum_graph = quantum_graph_builder.build(attach_datastore_records=False)
         return cls(quantum_graph=quantum_graph, butler=butler, resources=resources)
 
     def run(self, register_dataset_types: bool = False, save_versions: bool = True) -> list[Quantum]:
         """Run all the quanta in the `~lsst.pipe.base.QuantumGraph` in
         topological order.
 
         Use this method to run all quanta in the graph.  Use
@@ -352,8 +409,10 @@
         )
         single_quantum_executor = SingleQuantumExecutor(self.butler, task_factory, resources=self.resources)
         # Important that this returns a generator expression rather than being
         # a generator itself; that is what makes the PreExecInit stuff above
         # happen immediately instead of when the first quanta is executed,
         # which might be useful for callers who want to check the state of the
         # repo in between.
-        return (single_quantum_executor.execute(qnode.taskDef, qnode.quantum) for qnode in self.quantum_graph)
+        return (
+            single_quantum_executor.execute(qnode.task_node, qnode.quantum) for qnode in self.quantum_graph
+        )
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/singleQuantumExecutor.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/singleQuantumExecutor.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 # -------------------------------
 #  Imports of standard modules --
 # -------------------------------
 import logging
 import sys
 import time
+import warnings
 from collections import defaultdict
 from collections.abc import Callable
 from itertools import chain
 from typing import Any, cast
 
 from lsst.daf.butler import (
     Butler,
@@ -56,18 +57,20 @@
     NoWorkFound,
     PipelineTask,
     QuantumContext,
     RepeatableQuantumError,
     TaskDef,
     TaskFactory,
 )
+from lsst.pipe.base.pipeline_graph import PipelineGraph, TaskNode
 
 # During metadata transition phase, determine metadata class by
 # asking pipe_base
 from lsst.pipe.base.task import _TASK_FULL_METADATA_TYPE, _TASK_METADATA_TYPE
+from lsst.utils.introspection import find_outside_stacklevel
 from lsst.utils.timer import logInfo
 
 # -----------------------------
 #  Imports for other modules --
 # -----------------------------
 from .log_capture import LogCapture
 from .quantumGraphExecutor import QuantumExecutor
@@ -111,26 +114,32 @@
         InvalidQuantumError.
     limited_butler_factory : `Callable`, optional
         A method that creates a `~lsst.daf.butler.LimitedButler` instance
         for a given Quantum. This parameter must be defined if ``butler`` is
         `None`. If ``butler`` is not `None` then this parameter is ignored.
     resources : `~lsst.pipe.base.ExecutionResources`, optional
         The resources available to this quantum when executing.
+    skipExisting : `bool`, optional
+        If `True`, skip quanta whose metadata datasets are already stored.
+        Unlike ``skipExistingIn``, this works with limited butlers as well as
+        full butlers.  Always set to `True` if ``skipExistingIn`` matches
+        ``butler.run``.
     """
 
     def __init__(
         self,
         butler: Butler | None,
         taskFactory: TaskFactory,
         skipExistingIn: Any = None,
         clobberOutputs: bool = False,
         enableLsstDebug: bool = False,
         exitOnKnownError: bool = False,
         limited_butler_factory: Callable[[Quantum], LimitedButler] | None = None,
         resources: ExecutionResources | None = None,
+        skipExisting: bool = False,
     ):
         self.butler = butler
         self.taskFactory = taskFactory
         self.enableLsstDebug = enableLsstDebug
         self.clobberOutputs = clobberOutputs
         self.exitOnKnownError = exitOnKnownError
         self.limited_butler_factory = limited_butler_factory
@@ -139,47 +148,68 @@
 
         if self.butler is None:
             assert limited_butler_factory is not None, "limited_butler_factory is needed when butler is None"
 
         # Find whether output run is in skipExistingIn.
         # TODO: This duplicates logic in GraphBuilder, would be nice to have
         # better abstraction for this some day.
-        self.skipExisting = False
+        self.skipExisting = skipExisting
         if self.butler is not None and skipExistingIn:
             skip_collections_wildcard = CollectionWildcard.from_expression(skipExistingIn)
             # As optimization check in the explicit list of names first
             self.skipExisting = self.butler.run in skip_collections_wildcard.strings
             if not self.skipExisting:
                 # need to flatten it and check again
                 self.skipExisting = self.butler.run in self.butler.registry.queryCollections(
                     skipExistingIn,
                     collectionTypes=CollectionType.RUN,
                 )
 
-    def execute(self, taskDef: TaskDef, quantum: Quantum) -> Quantum:
+    def execute(self, task_node: TaskDef | TaskNode, /, quantum: Quantum) -> Quantum:
         # Docstring inherited from QuantumExecutor.execute
         assert quantum.dataId is not None, "Quantum DataId cannot be None"
 
+        task_node = self._conform_task_def(task_node)
         if self.butler is not None:
             self.butler.registry.refresh()
 
         # Catch any exception and make a report based on that.
         try:
-            result = self._execute(taskDef, quantum)
-            self.report = QuantumReport(dataId=quantum.dataId, taskLabel=taskDef.label)
+            result = self._execute(task_node, quantum)
+            self.report = QuantumReport(dataId=quantum.dataId, taskLabel=task_node.label)
             return result
         except Exception as exc:
             self.report = QuantumReport.from_exception(
                 exception=exc,
                 dataId=quantum.dataId,
-                taskLabel=taskDef.label,
+                taskLabel=task_node.label,
             )
             raise
 
-    def _execute(self, taskDef: TaskDef, quantum: Quantum) -> Quantum:
+    def _conform_task_def(self, task_node: TaskDef | TaskNode) -> TaskNode:
+        """Convert the given object to a TaskNode and emit a deprecation
+        warning if it isn't one already.
+        """
+        # TODO: remove this function and all call points on DM-40443, and
+        # fix annotations and docstrings for those methods as well.
+        if isinstance(task_node, TaskDef):
+            warnings.warn(
+                "Passing TaskDef to SingleQuantumExecutor methods is deprecated "
+                "and will not be supported after v27.",
+                FutureWarning,
+                find_outside_stacklevel("lsst.ctrl.mpexec"),
+            )
+            # Convert to a real TaskNode to avoid a warnings cascade.
+            pipeline_graph = PipelineGraph()
+            return pipeline_graph.add_task(
+                task_node.label, task_node.taskClass, task_node.config, connections=task_node.connections
+            )
+        return task_node
+
+    def _execute(self, task_node: TaskNode, /, quantum: Quantum) -> Quantum:
         """Execute the quantum.
 
         Internal implementation of `execute()`.
         """
         startTime = time.time()
 
         # Make a limited butler instance if needed (which should be QBB if full
@@ -192,224 +222,238 @@
             assert self.limited_butler_factory is not None
             limited_butler = self.limited_butler_factory(quantum)
 
         if self.butler is not None:
             log_capture = LogCapture.from_full(self.butler)
         else:
             log_capture = LogCapture.from_limited(limited_butler)
-        with log_capture.capture_logging(taskDef, quantum) as captureLog:
+        with log_capture.capture_logging(task_node, quantum) as captureLog:
             # Save detailed resource usage before task start to metadata.
             quantumMetadata = _TASK_METADATA_TYPE()
             logInfo(None, "prep", metadata=quantumMetadata)  # type: ignore[arg-type]
 
-            _LOG.info("Preparing execution of quantum for label=%s dataId=%s.", taskDef.label, quantum.dataId)
+            _LOG.info(
+                "Preparing execution of quantum for label=%s dataId=%s.", task_node.label, quantum.dataId
+            )
 
             # check whether to skip or delete old outputs, if it returns True
             # or raises an exception do not try to store logs, as they may be
             # already in butler.
             captureLog.store = False
-            if self.checkExistingOutputs(quantum, taskDef, limited_butler):
+            if self.checkExistingOutputs(quantum, task_node, limited_butler):
                 _LOG.info(
                     "Skipping already-successful quantum for label=%s dataId=%s.",
-                    taskDef.label,
+                    task_node.label,
                     quantum.dataId,
                 )
                 return quantum
             captureLog.store = True
 
             try:
-                quantum = self.updatedQuantumInputs(quantum, taskDef, limited_butler)
+                quantum = self.updatedQuantumInputs(quantum, task_node, limited_butler)
             except NoWorkFound as exc:
                 _LOG.info(
                     "Nothing to do for task '%s' on quantum %s; saving metadata and skipping: %s",
-                    taskDef.label,
+                    task_node.label,
                     quantum.dataId,
                     str(exc),
                 )
                 # Make empty metadata that looks something like what a
                 # do-nothing task would write (but we don't bother with empty
                 # nested PropertySets for subtasks).  This is slightly
                 # duplicative with logic in pipe_base that we can't easily call
                 # from here; we'll fix this on DM-29761.
                 logInfo(None, "end", metadata=quantumMetadata)  # type: ignore[arg-type]
                 fullMetadata = _TASK_FULL_METADATA_TYPE()
-                fullMetadata[taskDef.label] = _TASK_METADATA_TYPE()
+                fullMetadata[task_node.label] = _TASK_METADATA_TYPE()
                 fullMetadata["quantum"] = quantumMetadata
-                self.writeMetadata(quantum, fullMetadata, taskDef, limited_butler)
+                self.writeMetadata(quantum, fullMetadata, task_node, limited_butler)
                 return quantum
 
             # enable lsstDebug debugging
             if self.enableLsstDebug:
                 try:
                     _LOG.debug("Will try to import debug.py")
                     import debug  # type: ignore # noqa:F401
                 except ImportError:
                     _LOG.warn("No 'debug' module found.")
 
             # initialize global state
             self.initGlobals(quantum)
 
             # Ensure that we are executing a frozen config
-            taskDef.config.freeze()
+            task_node.config.freeze()
             logInfo(None, "init", metadata=quantumMetadata)  # type: ignore[arg-type]
             init_input_refs = list(quantum.initInputs.values())
 
             _LOG.info(
                 "Constructing task and executing quantum for label=%s dataId=%s.",
-                taskDef.label,
+                task_node.label,
                 quantum.dataId,
             )
-            task = self.taskFactory.makeTask(taskDef, limited_butler, init_input_refs)
+            task = self.taskFactory.makeTask(task_node, limited_butler, init_input_refs)
             logInfo(None, "start", metadata=quantumMetadata)  # type: ignore[arg-type]
             try:
-                self.runQuantum(task, quantum, taskDef, limited_butler)
+                self.runQuantum(task, quantum, task_node, limited_butler)
             except Exception as e:
                 _LOG.error(
                     "Execution of task '%s' on quantum %s failed. Exception %s: %s",
-                    taskDef.label,
+                    task_node.label,
                     quantum.dataId,
                     e.__class__.__name__,
                     str(e),
                 )
                 raise
             logInfo(None, "end", metadata=quantumMetadata)  # type: ignore[arg-type]
             fullMetadata = task.getFullMetadata()
             fullMetadata["quantum"] = quantumMetadata
-            self.writeMetadata(quantum, fullMetadata, taskDef, limited_butler)
+            self.writeMetadata(quantum, fullMetadata, task_node, limited_butler)
             stopTime = time.time()
             _LOG.info(
                 "Execution of task '%s' on quantum %s took %.3f seconds",
-                taskDef.label,
+                task_node.label,
                 quantum.dataId,
                 stopTime - startTime,
             )
         return quantum
 
-    def checkExistingOutputs(self, quantum: Quantum, taskDef: TaskDef, limited_butler: LimitedButler) -> bool:
+    def checkExistingOutputs(
+        self, quantum: Quantum, task_node: TaskDef | TaskNode, /, limited_butler: LimitedButler
+    ) -> bool:
         """Decide whether this quantum needs to be executed.
 
         If only partial outputs exist then they are removed if
         ``clobberOutputs`` is True, otherwise an exception is raised.
 
+        The ``LimitedButler`` is used for everything, and should be set to
+        ``self.butler`` if no separate ``LimitedButler`` is available.
+
         Parameters
         ----------
         quantum : `~lsst.daf.butler.Quantum`
             Quantum to check for existing outputs.
-        taskDef : `~lsst.pipe.base.TaskDef`
-            Task definition structure.
+        task_node : `~lsst.pipe.base.TaskDef` or \
+                `~lsst.pipe.base.pipeline_graph.TaskNode`
+            Task definition structure.  `~lsst.pipe.base.TaskDef` support is
+            deprecated and will be removed after v27.
         limited_butler : `~lsst.daf.butler.LimitedButler`
-            Butler to use for querying.
+            Butler to use for querying and clobbering.
 
         Returns
         -------
         exist : `bool`
             `True` if ``self.skipExisting`` is defined, and a previous
             execution of this quanta appears to have completed successfully
             (either because metadata was written or all datasets were written).
             `False` otherwise.
 
         Raises
         ------
         RuntimeError
             Raised if some outputs exist and some not.
         """
+        task_node = self._conform_task_def(task_node)
+
         if not self.butler:
             # Skip/prune logic only works for full butler.
             return False
 
         if self.skipExisting:
             _LOG.debug(
                 "Checking existence of metadata from previous execution of label=%s dataId=%s.",
-                taskDef.label,
+                task_node.label,
                 quantum.dataId,
             )
             # Metadata output exists; this is sufficient to assume the previous
             # run was successful and should be skipped.
-            [metadata_ref] = quantum.outputs[taskDef.metadataDatasetName]
+            [metadata_ref] = quantum.outputs[task_node.metadata_output.dataset_type_name]
             if metadata_ref is not None:
                 if limited_butler.stored(metadata_ref):
                     return True
 
         # Find and prune (partial) outputs if `self.clobberOutputs` is set.
         _LOG.debug(
-            "Looking for existing outputs in the way for label=%s dataId=%s.", taskDef.label, quantum.dataId
+            "Looking for existing outputs in the way for label=%s dataId=%s.", task_node.label, quantum.dataId
         )
-        ref_dict = self.butler.stored_many(chain.from_iterable(quantum.outputs.values()))
+        ref_dict = limited_butler.stored_many(chain.from_iterable(quantum.outputs.values()))
         existingRefs = [ref for ref, exists in ref_dict.items() if exists]
         missingRefs = [ref for ref, exists in ref_dict.items() if not exists]
         if existingRefs:
             if not missingRefs:
                 # Full outputs exist.
                 if self.skipExisting:
                     return True
                 elif self.clobberOutputs:
                     _LOG.info("Removing complete outputs for quantum %s: %s", quantum, existingRefs)
-                    self.butler.pruneDatasets(existingRefs, disassociate=True, unstore=True, purge=True)
+                    limited_butler.pruneDatasets(existingRefs, disassociate=True, unstore=True, purge=True)
                 else:
                     raise RuntimeError(
                         f"Complete outputs exists for a quantum {quantum} "
                         "and neither clobberOutputs nor skipExisting is set: "
-                        f"collection={self.butler.run} existingRefs={existingRefs}"
+                        f"existingRefs={existingRefs}"
                     )
             else:
                 # Partial outputs from a failed quantum.
                 _LOG.debug(
-                    "Partial outputs exist for quantum %s collection=%s existingRefs=%s missingRefs=%s",
+                    "Partial outputs exist for quantum %s existingRefs=%s missingRefs=%s",
                     quantum,
-                    self.butler.run,
                     existingRefs,
                     missingRefs,
                 )
                 if self.clobberOutputs:
                     # only prune
-                    _LOG.info("Removing partial outputs for task %s: %s", taskDef, existingRefs)
-                    self.butler.pruneDatasets(existingRefs, disassociate=True, unstore=True, purge=True)
+                    _LOG.info("Removing partial outputs for task %s: %s", task_node.label, existingRefs)
+                    limited_butler.pruneDatasets(existingRefs, disassociate=True, unstore=True, purge=True)
                     return False
                 else:
                     raise RuntimeError(
                         "Registry inconsistency while checking for existing quantum outputs:"
-                        f" quantum={quantum} collection={self.butler.run} existingRefs={existingRefs}"
+                        f" quantum={quantum} existingRefs={existingRefs}"
                         f" missingRefs={missingRefs}"
                     )
 
         # By default always execute.
         return False
 
     def updatedQuantumInputs(
-        self, quantum: Quantum, taskDef: TaskDef, limited_butler: LimitedButler
+        self, quantum: Quantum, task_node: TaskDef | TaskNode, /, limited_butler: LimitedButler
     ) -> Quantum:
         """Update quantum with extra information, returns a new updated
         Quantum.
 
         Some methods may require input DatasetRefs to have non-None
         ``dataset_id``, but in case of intermediate dataset it may not be
         filled during QuantumGraph construction. This method will retrieve
         missing info from registry.
 
         Parameters
         ----------
         quantum : `~lsst.daf.butler.Quantum`
             Single Quantum instance.
-        taskDef : `~lsst.pipe.base.TaskDef`
-            Task definition structure.
+        task_node : `~lsst.pipe.base.TaskDef` or \
+                `~lsst.pipe.base.pipeline_graph.TaskNode`
+            Task definition structure.  `~lsst.pipe.base.TaskDef` support is
+            deprecated and will be removed after v27.
         limited_butler : `~lsst.daf.butler.LimitedButler`
             Butler to use for querying.
 
         Returns
         -------
         update : `~lsst.daf.butler.Quantum`
             Updated Quantum instance.
         """
+        task_node = self._conform_task_def(task_node)
+
         anyChanges = False
         updatedInputs: defaultdict[DatasetType, list] = defaultdict(list)
         for key, refsForDatasetType in quantum.inputs.items():
             _LOG.debug(
                 "Checking existence of input '%s' for label=%s dataId=%s.",
                 key.name,
-                taskDef.label,
+                task_node.label,
                 quantum.dataId,
             )
             newRefsForDatasetType = updatedInputs[key]
             stored = limited_butler.stored_many(refsForDatasetType)
             for ref in refsForDatasetType:
                 if stored[ref]:
                     newRefsForDatasetType.append(ref)
@@ -428,77 +472,88 @@
         # which we'll let propagate up.  This is exactly what we run during QG
         # generation, because a task shouldn't care whether an input is missing
         # because some previous task didn't produce it, or because it just
         # wasn't there during QG generation.
         namedUpdatedInputs = NamedKeyDict[DatasetType, list[DatasetRef]](updatedInputs.items())
         helper = AdjustQuantumHelper(namedUpdatedInputs, quantum.outputs)
         if anyChanges:
-            _LOG.debug("Running adjustQuantum for label=%s dataId=%s.", taskDef.label, quantum.dataId)
+            _LOG.debug("Running adjustQuantum for label=%s dataId=%s.", task_node.label, quantum.dataId)
             assert quantum.dataId is not None, "Quantum DataId cannot be None"
-            helper.adjust_in_place(taskDef.connections, label=taskDef.label, data_id=quantum.dataId)
+            helper.adjust_in_place(task_node.get_connections(), label=task_node.label, data_id=quantum.dataId)
         return Quantum(
             taskName=quantum.taskName,
             taskClass=quantum.taskClass,
             dataId=quantum.dataId,
             initInputs=quantum.initInputs,
             inputs=helper.inputs,
             outputs=helper.outputs,
         )
 
     def runQuantum(
-        self, task: PipelineTask, quantum: Quantum, taskDef: TaskDef, limited_butler: LimitedButler
+        self,
+        task: PipelineTask,
+        quantum: Quantum,
+        task_node: TaskDef | TaskNode,
+        /,
+        limited_butler: LimitedButler,
     ) -> None:
         """Execute task on a single quantum.
 
         Parameters
         ----------
         task : `~lsst.pipe.base.PipelineTask`
             Task object.
         quantum : `~lsst.daf.butler.Quantum`
             Single Quantum instance.
-        taskDef : `~lsst.pipe.base.TaskDef`
-            Task definition structure.
+        task_node : `~lsst.pipe.base.TaskDef` or \
+                `~lsst.pipe.base.pipeline_graph.TaskNode`
+            Task definition structure.  `~lsst.pipe.base.TaskDef` support is
+            deprecated and will be removed after v27.
         limited_butler : `~lsst.daf.butler.LimitedButler`
             Butler to use for dataset I/O.
         """
+        task_node = self._conform_task_def(task_node)
+
         # Create a butler that operates in the context of a quantum
         butlerQC = QuantumContext(limited_butler, quantum, resources=self.resources)
 
         # Get the input and output references for the task
-        inputRefs, outputRefs = taskDef.connections.buildDatasetRefs(quantum)
+        inputRefs, outputRefs = task_node.get_connections().buildDatasetRefs(quantum)
 
         # Call task runQuantum() method.  Catch a few known failure modes and
         # translate them into specific
         try:
             task.runQuantum(butlerQC, inputRefs, outputRefs)
         except NoWorkFound as err:
             # Not an error, just an early exit.
-            _LOG.info("Task '%s' on quantum %s exited early: %s", taskDef.label, quantum.dataId, str(err))
+            _LOG.info("Task '%s' on quantum %s exited early: %s", task_node.label, quantum.dataId, str(err))
             pass
         except RepeatableQuantumError as err:
             if self.exitOnKnownError:
-                _LOG.warning("Caught repeatable quantum error for %s (%s):", taskDef, quantum.dataId)
+                _LOG.warning("Caught repeatable quantum error for %s (%s):", task_node.label, quantum.dataId)
                 _LOG.warning(err, exc_info=True)
                 sys.exit(err.EXIT_CODE)
             else:
                 raise
         except InvalidQuantumError as err:
-            _LOG.fatal("Invalid quantum error for %s (%s): %s", taskDef, quantum.dataId)
+            _LOG.fatal("Invalid quantum error for %s (%s): %s", task_node.label, quantum.dataId)
             _LOG.fatal(err, exc_info=True)
             sys.exit(err.EXIT_CODE)
 
     def writeMetadata(
-        self, quantum: Quantum, metadata: Any, taskDef: TaskDef, limited_butler: LimitedButler
+        self, quantum: Quantum, metadata: Any, task_node: TaskDef | TaskNode, /, limited_butler: LimitedButler
     ) -> None:
         # DatasetRef has to be in the Quantum outputs, can lookup by name
+        task_node = self._conform_task_def(task_node)
         try:
-            [ref] = quantum.outputs[taskDef.metadataDatasetName]
+            [ref] = quantum.outputs[task_node.metadata_output.dataset_type_name]
         except LookupError as exc:
             raise InvalidQuantumError(
-                f"Quantum outputs is missing metadata dataset type {taskDef.metadataDatasetName};"
+                "Quantum outputs is missing metadata dataset type "
+                f"{task_node.metadata_output.dataset_type_name};"
                 " this could happen due to inconsistent options between QuantumGraph generation"
                 " and execution"
             ) from exc
         limited_butler.put(metadata, ref)
 
     def initGlobals(self, quantum: Quantum) -> None:
         """Initialize global state needed for task execution.
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst/ctrl/mpexec/taskFactory.py` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst/ctrl/mpexec/taskFactory.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,44 +26,63 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 __all__ = ["TaskFactory"]
 
 import logging
+import warnings
 from collections.abc import Iterable
 from typing import TYPE_CHECKING, Any
 
+from lsst.pipe.base import TaskDef
 from lsst.pipe.base import TaskFactory as BaseTaskFactory
+from lsst.pipe.base.pipeline_graph import TaskNode
+from lsst.utils.introspection import find_outside_stacklevel
 
 if TYPE_CHECKING:
     from lsst.daf.butler import DatasetRef, LimitedButler
-    from lsst.pipe.base import PipelineTask, TaskDef
+    from lsst.pipe.base import PipelineTask
 
 _LOG = logging.getLogger(__name__)
 
 
 class TaskFactory(BaseTaskFactory):
     """Class instantiating PipelineTasks."""
 
     def makeTask(
-        self, taskDef: TaskDef, butler: LimitedButler, initInputRefs: Iterable[DatasetRef] | None
+        self,
+        task_node: TaskDef | TaskNode,
+        /,
+        butler: LimitedButler,
+        initInputRefs: Iterable[DatasetRef] | None,
     ) -> PipelineTask:
         # docstring inherited
-
-        config = taskDef.config
-
-        # Get init inputs from butler.
+        config = task_node.config
         init_inputs: dict[str, Any] = {}
-        if initInputRefs:
-            connections = config.connections.ConnectionsClass(config=config)
-            for name in connections.initInputs:
-                attribute = getattr(connections, name)
-                dataset_type_name = attribute.name
-                for ref in initInputRefs:
-                    if ref.datasetType.name == dataset_type_name:
-                        init_inputs[name] = butler.get(ref)
-                        break
-
+        init_input_refs_by_dataset_type = {}
+        if initInputRefs is not None:
+            init_input_refs_by_dataset_type = {ref.datasetType.name: ref for ref in initInputRefs}
+        if isinstance(task_node, TaskDef):
+            # TODO: remove this block on DM-40443, along with type annotation.
+            warnings.warn(
+                "Passing TaskDef to TaskFactory is deprecated and will not be supported after v27.",
+                FutureWarning,
+                find_outside_stacklevel("lsst.pipe.base"),
+            )
+            task_class = task_node.taskClass
+            assert task_class is not None
+            if init_input_refs_by_dataset_type:
+                connections = config.connections.ConnectionsClass(config=config)
+                for name in connections.initInputs:
+                    attribute = getattr(connections, name)
+                    init_inputs[name] = butler.get(init_input_refs_by_dataset_type[attribute.name])
+        else:
+            task_class = task_node.task_class
+            if init_input_refs_by_dataset_type:
+                for read_edge in task_node.init.inputs.values():
+                    init_inputs[read_edge.connection_name] = butler.get(
+                        init_input_refs_by_dataset_type[read_edge.dataset_type_name]
+                    )
         # make task instance
-        task = taskDef.taskClass(config=config, initInputs=init_inputs, name=taskDef.label)
+        task = task_class(config=config, initInputs=init_inputs, name=task_node.label)
         return task
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/PKG-INFO` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst_ctrl_mpexec.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-mpexec
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: Pipeline execution infrastructure for the Rubin Observatory LSST Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_mpexec
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/python/lsst_ctrl_mpexec.egg-info/SOURCES.txt` & `lsst_ctrl_mpexec-27.0.0rc1/python/lsst_ctrl_mpexec.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 python/lsst_ctrl_mpexec.egg-info/dependency_links.txt
 python/lsst_ctrl_mpexec.egg-info/entry_points.txt
 python/lsst_ctrl_mpexec.egg-info/requires.txt
 python/lsst_ctrl_mpexec.egg-info/top_level.txt
 python/lsst_ctrl_mpexec.egg-info/zip-safe
 tests/test_cliCmdCleanup.py
 tests/test_cliCmdPurge.py
+tests/test_cliCmdQgraph.py
 tests/test_cliCmdReport.py
 tests/test_cliCmdUpdateGraphRun.py
 tests/test_cliScript.py
 tests/test_cliUtils.py
 tests/test_cmdLineFwk.py
 tests/test_dotTools.py
 tests/test_executors.py
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdCleanup.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_cliCmdCleanup.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdPurge.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_cliCmdPurge.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdReport.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_cliCmdQgraph.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,69 +21,62 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for ctrl_mpexec CLI update-graph-run subcommand."""
+"""Unit tests for ctrl_mpexec CLI qgraph subcommand."""
 
 import os
 import unittest
 
-import yaml
+from lsst.ctrl.mpexec import Report
 from lsst.ctrl.mpexec.cli.pipetask import cli as pipetask_cli
 from lsst.daf.butler.cli.utils import LogCliRunner, clickResultMsg
 from lsst.daf.butler.tests.utils import makeTestTempDir, removeTestTempDir
 from lsst.pipe.base.tests.simpleQGraph import makeSimpleQGraph
-from lsst.pipe.base.tests.util import check_output_run
-from yaml.loader import SafeLoader
 
 TESTDIR = os.path.abspath(os.path.dirname(__file__))
 
 
-class ReportTest(unittest.TestCase):
-    """Test executing "pipetask report" command."""
+class QgraphTest(unittest.TestCase):
+    """Test executing "pipetask qgraph" command."""
 
     def setUp(self) -> None:
         self.runner = LogCliRunner()
         self.root = makeTestTempDir(TESTDIR)
 
     def tearDown(self) -> None:
         removeTestTempDir(self.root)
 
-    def test_report(self):
-        """Test for making a report on the produced and missing expected
-        datasets in a quantum graph. in a graph.
-        """
+    def test_qgraph_summary(self):
+        """Test for making a summary of a QuantumGraph."""
         metadata = {"output_run": "run"}
         butler, qgraph = makeSimpleQGraph(
             run="run",
             root=self.root,
             metadata=metadata,
         )
-        # Check that we can get the proper run collection from the qgraph
-        self.assertEqual(check_output_run(qgraph, "run"), [])
 
         graph_uri = os.path.join(self.root, "graph.qgraph")
         qgraph.saveUri(graph_uri)
 
-        test_filename = os.path.join(self.root, "report_test.yaml")
+        test_filename = os.path.join(self.root, "summary.json")
 
         result = self.runner.invoke(
             pipetask_cli,
-            ["report", self.root, graph_uri, test_filename, "--no-logs"],
+            ["qgraph", "--butler-config", self.root, "--qgraph", graph_uri, "--summary", test_filename],
             input="no",
         )
-
         # Check that we can read from the command line
         self.assertEqual(result.exit_code, 0, clickResultMsg(result))
 
         # Check that we can open and read the file produced by make_reports
         with open(test_filename) as f:
-            report_output_dict = yaml.load(f, Loader=SafeLoader)
-        self.assertIsNotNone(report_output_dict["task0"])
-        self.assertIsNotNone(report_output_dict["task0"]["failed_quanta"])
+            summary = Report.model_validate_json(f.read())
+        self.assertEqual(summary.qgraphSummary.outputRun, "run")
+        self.assertEqual(len(summary.qgraphSummary.qgraphTaskSummaries), 5)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_cliCmdUpdateGraphRun.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_cliCmdUpdateGraphRun.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_cliScript.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_cliScript.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_cliUtils.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_cliUtils.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_cmdLineFwk.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_cmdLineFwk.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     Instrument,
     Pipeline,
     PipelineTaskConfig,
     PipelineTaskConnections,
     QuantumGraph,
     TaskDef,
 )
-from lsst.pipe.base.graphBuilder import DatasetQueryConstraintVariant as DQCVariant
+from lsst.pipe.base.all_dimensions_quantum_graph_builder import DatasetQueryConstraintVariant as DQCVariant
 from lsst.pipe.base.script import transfer_from_graph
 from lsst.pipe.base.tests.simpleQGraph import (
     AddTask,
     AddTaskFactoryMock,
     makeSimpleButler,
     makeSimplePipeline,
     makeSimpleQGraph,
@@ -360,26 +360,26 @@
         self.assertIsInstance(pipeline, Pipeline)
         self.assertEqual(len(pipeline), 3)
 
         # single task pipeline with config overrides, need real task class
         actions = [_ACTION_ADD_TASK(f"{_TASK_CLASS}:task"), _ACTION_CONFIG("task:addend=100")]
         args = _makeArgs(pipeline_actions=actions)
         pipeline = fwk.makePipeline(args)
-        taskDefs = list(pipeline.toExpandedPipeline())
-        self.assertEqual(len(taskDefs), 1)
-        self.assertEqual(taskDefs[0].config.addend, 100)
+        pipeline_graph = pipeline.to_graph()
+        self.assertEqual(len(pipeline_graph.tasks), 1)
+        self.assertEqual(next(iter(pipeline_graph.tasks.values())).config.addend, 100)
 
         overrides = b"config.addend = 1000\n"
         with makeTmpFile(overrides) as tmpname:
             actions = [_ACTION_ADD_TASK(f"{_TASK_CLASS}:task"), _ACTION_CONFIG_FILE("task:" + tmpname)]
             args = _makeArgs(pipeline_actions=actions)
             pipeline = fwk.makePipeline(args)
-            taskDefs = list(pipeline.toExpandedPipeline())
-            self.assertEqual(len(taskDefs), 1)
-            self.assertEqual(taskDefs[0].config.addend, 1000)
+            pipeline_graph = pipeline.to_graph()
+            self.assertEqual(len(pipeline_graph.tasks), 1)
+            self.assertEqual(next(iter(pipeline_graph.tasks.values())).config.addend, 1000)
 
         # Check --instrument option, for now it only checks that it does not
         # crash.
         actions = [_ACTION_ADD_TASK(f"{_TASK_CLASS}:task"), _ACTION_ADD_INSTRUMENT("Instrument")]
         args = _makeArgs(pipeline_actions=actions)
         pipeline = fwk.makePipeline(args)
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_dotTools.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_dotTools.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_executors.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_executors.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     MPTimeoutError,
     QuantumExecutor,
     QuantumReport,
     SingleQuantumExecutor,
 )
 from lsst.ctrl.mpexec.execFixupDataId import ExecFixupDataId
 from lsst.daf.butler.tests.utils import makeTestTempDir, removeTestTempDir
-from lsst.pipe.base import NodeId
+from lsst.pipe.base import NodeId, QgraphSummary, QgraphTaskSummary
 from lsst.pipe.base.tests.simpleQGraph import AddTaskFactoryMock, makeSimpleQGraph
 
 logging.basicConfig(level=logging.DEBUG)
 
 _LOG = logging.getLogger(__name__)
 
 TESTDIR = os.path.abspath(os.path.dirname(__file__))
@@ -76,27 +76,27 @@
         if mp:
             # in multiprocess mode use shared list
             manager = Manager()
             self.quanta = manager.list()
         self.report = None
         self._execute_called = False
 
-    def execute(self, taskDef, quantum):
-        _LOG.debug("QuantumExecutorMock.execute: taskDef=%s dataId=%s", taskDef, quantum.dataId)
+    def execute(self, task_node, /, quantum):
+        _LOG.debug("QuantumExecutorMock.execute: task_node=%s dataId=%s", task_node, quantum.dataId)
         self._execute_called = True
-        if taskDef.taskClass:
+        if task_node.task_class:
             try:
                 # only works for one of the TaskMock classes below
-                taskDef.taskClass().runQuantum()
-                self.report = QuantumReport(dataId=quantum.dataId, taskLabel=taskDef.label)
+                task_node.task_class().runQuantum()
+                self.report = QuantumReport(dataId=quantum.dataId, taskLabel=task_node.label)
             except Exception as exc:
                 self.report = QuantumReport.from_exception(
                     exception=exc,
                     dataId=quantum.dataId,
-                    taskLabel=taskDef.label,
+                    taskLabel=task_node.label,
                 )
                 raise
         self.quanta.append(quantum)
         return quantum
 
     def getReport(self):
         if not self._execute_called:
@@ -137,23 +137,24 @@
 class QuantumIterDataMock:
     """Simple class to mock QuantumIterData.
 
     Parameters
     ----------
     index : `int`
         The index of this mock.
-    taskDef : `TaskDefMock`
+    task_node : `TaskNodeMock`
         Mocked task definition.
     **dataId : `~typing.Any`
         The data ID of the mocked quantum.
     """
 
-    def __init__(self, index, taskDef, **dataId):
+    def __init__(self, index, task_node, **dataId):
         self.index = index
-        self.taskDef = taskDef
+        self.taskDef = task_node
+        self.task_node = task_node
         self.quantum = QuantumMock(dataId)
         self.dependencies = set()
         self.nodeId = NodeId(index, "DummyBuildString")
 
 
 class QuantumGraphMock:
     """Mock for quantum graph.
@@ -175,25 +176,25 @@
         yield from nx.topological_sort(self._graph)
 
     def __len__(self):
         return len(self._graph)
 
     def findTaskDefByLabel(self, label):
         for q in self:
-            if q.taskDef.label == label:
+            if q.task_node.label == label:
                 return q.taskDef
 
     def getQuantaForTask(self, taskDef):
         nodes = self.getNodesForTask(taskDef)
         return {q.quantum for q in nodes}
 
     def getNodesForTask(self, taskDef):
         quanta = set()
         for q in self:
-            if q.taskDef == taskDef:
+            if q.task_node.label == taskDef.label:
                 quanta.add(q)
         return quanta
 
     @property
     def graph(self):
         return self._graph
 
@@ -204,14 +205,38 @@
         result = set()
         for n in node.dependencies:
             for otherNode in self:
                 if otherNode.index == n:
                     result.add(otherNode)
         return result
 
+    def getSummary(self):
+        summary = QgraphSummary(
+            graphID="1712445133.605479-3902002",
+            cmdLine="mock_pipetask -a 1 -b 2 -c 3 4 5 6",
+            pipeBaseVersion="1.1.1",
+            creationUTC="",
+            inputCollection=["mock_input"],
+            outputCollection="mock_output",
+            outputRun="mock_run",
+        )
+        for q in self:
+            qts = summary.qgraphTaskSummaries.setdefault(
+                q.taskDef.label, QgraphTaskSummary(taskLabel=q.taskDef.label)
+            )
+            qts.numQuanta += 1
+
+            for k in ["in1", "in2", "in3"]:
+                qts.numInputs[k] += 1
+
+            for k in ["out1", "out2", "out3"]:
+                qts.numOutputs[k] += 1
+
+        return summary
+
 
 class TaskMockMP:
     """Simple mock class for task supporting multiprocessing."""
 
     canMultiprocess = True
 
     def runQuantum(self):
@@ -253,52 +278,51 @@
 
 class TaskMockNoMP:
     """Simple mock class for task not supporting multiprocessing."""
 
     canMultiprocess = False
 
 
-class TaskDefMock:
-    """Simple mock class for task definition in a pipeline.
+class TaskNodeMock:
+    """Simple mock class for task definition in a pipeline graph.
 
     Parameters
     ----------
-    taskName : `str`, optional
-        The name of the task.
+    label : `str`
+        Label of the task in the pipeline.
+    task_class : `type`
+        Subclass of `lsst.pipe.base.PipelineTask`.
     config : `PipelineTaskConfig`, optional
-        Config to use for this task.
-    taskClass : `type`, optional
-        The class of the task.
-    label : `str`, optional
-        Task label.
+        Configuration for the task.
     """
 
-    def __init__(self, taskName="Task", config=None, taskClass=TaskMockMP, label="task1"):
-        self.taskName = taskName
-        self.config = config
-        self.taskClass = taskClass
+    def __init__(self, label="task1", task_class=TaskMockMP, config=None):
         self.label = label
+        # taskClass to look like TaskDef, task_class to look like TaskNode.
+        self.taskClass = task_class
+        self.task_class = task_class
+        self.config = config
 
     def __str__(self):
-        return f"TaskDefMock(taskName={self.taskName}, taskClass={self.taskClass.__name__})"
+        return f"TaskNodeMock({self.label}, {self.taskClass.__name__})"
 
 
 def _count_status(report, status):
     """Count number of quanta witha a given status."""
     return len([qrep for qrep in report.quantaReports if qrep.status is status])
 
 
 class MPGraphExecutorTestCase(unittest.TestCase):
     """A test case for MPGraphExecutor class."""
 
     def test_mpexec_nomp(self):
         """Make simple graph and execute."""
-        taskDef = TaskDefMock()
+        task_node = TaskNodeMock()
         qgraph = QuantumGraphMock(
-            [QuantumIterDataMock(index=i, taskDef=taskDef, detector=i) for i in range(3)]
+            [QuantumIterDataMock(index=i, task_node=task_node, detector=i) for i in range(3)]
         )
 
         # run in single-process mode
         qexec = QuantumExecutorMock()
         mpexec = MPGraphExecutor(numProc=1, timeout=100, quantumExecutor=qexec)
         mpexec.execute(qgraph)
         self.assertEqual(qexec.getDataIds("detector"), [0, 1, 2])
@@ -310,17 +334,17 @@
         self.assertTrue(all(qrep.status == ExecutionStatus.SUCCESS for qrep in report.quantaReports))
         self.assertTrue(all(qrep.exitCode is None for qrep in report.quantaReports))
         self.assertTrue(all(qrep.exceptionInfo is None for qrep in report.quantaReports))
         self.assertTrue(all(qrep.taskLabel == "task1" for qrep in report.quantaReports))
 
     def test_mpexec_mp(self):
         """Make simple graph and execute."""
-        taskDef = TaskDefMock()
+        task_node = TaskNodeMock()
         qgraph = QuantumGraphMock(
-            [QuantumIterDataMock(index=i, taskDef=taskDef, detector=i) for i in range(3)]
+            [QuantumIterDataMock(index=i, task_node=task_node, detector=i) for i in range(3)]
         )
 
         methods = ["spawn"]
         if sys.platform == "linux":
             methods.append("forkserver")
 
         for method in methods:
@@ -339,55 +363,55 @@
                 self.assertTrue(all(qrep.status == ExecutionStatus.SUCCESS for qrep in report.quantaReports))
                 self.assertTrue(all(qrep.exitCode == 0 for qrep in report.quantaReports))
                 self.assertTrue(all(qrep.exceptionInfo is None for qrep in report.quantaReports))
                 self.assertTrue(all(qrep.taskLabel == "task1" for qrep in report.quantaReports))
 
     def test_mpexec_nompsupport(self):
         """Try to run MP for task that has no MP support which should fail."""
-        taskDef = TaskDefMock(taskClass=TaskMockNoMP)
+        task_node = TaskNodeMock(task_class=TaskMockNoMP)
         qgraph = QuantumGraphMock(
-            [QuantumIterDataMock(index=i, taskDef=taskDef, detector=i) for i in range(3)]
+            [QuantumIterDataMock(index=i, task_node=task_node, detector=i) for i in range(3)]
         )
 
         # run in multi-process mode
         qexec = QuantumExecutorMock()
         mpexec = MPGraphExecutor(numProc=3, timeout=100, quantumExecutor=qexec)
-        with self.assertRaisesRegex(MPGraphExecutorError, "Task Task does not support multiprocessing"):
+        with self.assertRaisesRegex(MPGraphExecutorError, "Task 'task1' does not support multiprocessing"):
             mpexec.execute(qgraph)
 
     def test_mpexec_fixup(self):
         """Make simple graph and execute, add dependencies by executing fixup
         code.
         """
-        taskDef = TaskDefMock()
+        task_node = TaskNodeMock()
 
         for reverse in (False, True):
             qgraph = QuantumGraphMock(
-                [QuantumIterDataMock(index=i, taskDef=taskDef, detector=i) for i in range(3)]
+                [QuantumIterDataMock(index=i, task_node=task_node, detector=i) for i in range(3)]
             )
 
             qexec = QuantumExecutorMock()
             fixup = ExecFixupDataId("task1", "detector", reverse=reverse)
             mpexec = MPGraphExecutor(numProc=1, timeout=100, quantumExecutor=qexec, executionGraphFixup=fixup)
             mpexec.execute(qgraph)
 
             expected = [0, 1, 2]
             if reverse:
                 expected = list(reversed(expected))
             self.assertEqual(qexec.getDataIds("detector"), expected)
 
     def test_mpexec_timeout(self):
         """Fail due to timeout."""
-        taskDef = TaskDefMock()
-        taskDefSleep = TaskDefMock(taskClass=TaskMockLongSleep)
+        task_node = TaskNodeMock()
+        task_nodeSleep = TaskNodeMock(task_class=TaskMockLongSleep)
         qgraph = QuantumGraphMock(
             [
-                QuantumIterDataMock(index=0, taskDef=taskDef, detector=0),
-                QuantumIterDataMock(index=1, taskDef=taskDefSleep, detector=1),
-                QuantumIterDataMock(index=2, taskDef=taskDef, detector=2),
+                QuantumIterDataMock(index=0, task_node=task_node, detector=0),
+                QuantumIterDataMock(index=1, task_node=task_nodeSleep, detector=1),
+                QuantumIterDataMock(index=2, task_node=task_node, detector=2),
             ]
         )
 
         # with failFast we'll get immediate MPTimeoutError
         qexec = QuantumExecutorMock(mp=True)
         mpexec = MPGraphExecutor(numProc=3, timeout=1, quantumExecutor=qexec, failFast=True)
         with self.assertRaises(MPTimeoutError):
@@ -418,21 +442,21 @@
         self.assertGreater(len(report.quantaReports), 0)
         self.assertGreater(_count_status(report, ExecutionStatus.TIMEOUT), 0)
         self.assertTrue(any(qrep.exitCode < 0 for qrep in report.quantaReports))
         self.assertTrue(all(qrep.exceptionInfo is None for qrep in report.quantaReports))
 
     def test_mpexec_failure(self):
         """Failure in one task should not stop other tasks."""
-        taskDef = TaskDefMock()
-        taskDefFail = TaskDefMock(taskClass=TaskMockFail)
+        task_node = TaskNodeMock()
+        task_node_fail = TaskNodeMock(task_class=TaskMockFail)
         qgraph = QuantumGraphMock(
             [
-                QuantumIterDataMock(index=0, taskDef=taskDef, detector=0),
-                QuantumIterDataMock(index=1, taskDef=taskDefFail, detector=1),
-                QuantumIterDataMock(index=2, taskDef=taskDef, detector=2),
+                QuantumIterDataMock(index=0, task_node=task_node, detector=0),
+                QuantumIterDataMock(index=1, task_node=task_node_fail, detector=1),
+                QuantumIterDataMock(index=2, task_node=task_node, detector=2),
             ]
         )
 
         qexec = QuantumExecutorMock(mp=True)
         mpexec = MPGraphExecutor(numProc=3, timeout=100, quantumExecutor=qexec)
         with self.assertRaisesRegex(MPGraphExecutorError, "One or more tasks failed"):
             mpexec.execute(qgraph)
@@ -446,22 +470,22 @@
         self.assertEqual(_count_status(report, ExecutionStatus.FAILURE), 1)
         self.assertEqual(_count_status(report, ExecutionStatus.SUCCESS), 2)
         self.assertTrue(any(qrep.exitCode > 0 for qrep in report.quantaReports))
         self.assertTrue(any(qrep.exceptionInfo is not None for qrep in report.quantaReports))
 
     def test_mpexec_failure_dep(self):
         """Failure in one task should skip dependents."""
-        taskDef = TaskDefMock()
-        taskDefFail = TaskDefMock(taskClass=TaskMockFail)
+        task_node = TaskNodeMock()
+        task_node_fail = TaskNodeMock(task_class=TaskMockFail)
         qdata = [
-            QuantumIterDataMock(index=0, taskDef=taskDef, detector=0),
-            QuantumIterDataMock(index=1, taskDef=taskDefFail, detector=1),
-            QuantumIterDataMock(index=2, taskDef=taskDef, detector=2),
-            QuantumIterDataMock(index=3, taskDef=taskDef, detector=3),
-            QuantumIterDataMock(index=4, taskDef=taskDef, detector=4),
+            QuantumIterDataMock(index=0, task_node=task_node, detector=0),
+            QuantumIterDataMock(index=1, task_node=task_node_fail, detector=1),
+            QuantumIterDataMock(index=2, task_node=task_node, detector=2),
+            QuantumIterDataMock(index=3, task_node=task_node, detector=3),
+            QuantumIterDataMock(index=4, task_node=task_node, detector=4),
         ]
         qdata[2].dependencies.add(1)
         qdata[4].dependencies.add(3)
         qdata[4].dependencies.add(2)
 
         qgraph = QuantumGraphMock(qdata)
 
@@ -481,22 +505,22 @@
         self.assertEqual(_count_status(report, ExecutionStatus.SUCCESS), 2)
         self.assertEqual(_count_status(report, ExecutionStatus.SKIPPED), 2)
         self.assertTrue(any(qrep.exitCode > 0 for qrep in report.quantaReports))
         self.assertTrue(any(qrep.exceptionInfo is not None for qrep in report.quantaReports))
 
     def test_mpexec_failure_dep_nomp(self):
         """Failure in one task should skip dependents, in-process version."""
-        taskDef = TaskDefMock()
-        taskDefFail = TaskDefMock(taskClass=TaskMockFail)
+        task_node = TaskNodeMock()
+        task_node_fail = TaskNodeMock(task_class=TaskMockFail)
         qdata = [
-            QuantumIterDataMock(index=0, taskDef=taskDef, detector=0),
-            QuantumIterDataMock(index=1, taskDef=taskDefFail, detector=1),
-            QuantumIterDataMock(index=2, taskDef=taskDef, detector=2),
-            QuantumIterDataMock(index=3, taskDef=taskDef, detector=3),
-            QuantumIterDataMock(index=4, taskDef=taskDef, detector=4),
+            QuantumIterDataMock(index=0, task_node=task_node, detector=0),
+            QuantumIterDataMock(index=1, task_node=task_node_fail, detector=1),
+            QuantumIterDataMock(index=2, task_node=task_node, detector=2),
+            QuantumIterDataMock(index=3, task_node=task_node, detector=3),
+            QuantumIterDataMock(index=4, task_node=task_node, detector=4),
         ]
         qdata[2].dependencies.add(1)
         qdata[4].dependencies.add(3)
         qdata[4].dependencies.add(2)
 
         qgraph = QuantumGraphMock(qdata)
 
@@ -520,23 +544,23 @@
 
     def test_mpexec_failure_failfast(self):
         """Fast fail stops quickly.
 
         Timing delay of task #3 should be sufficient to process
         failure and raise exception.
         """
-        taskDef = TaskDefMock()
-        taskDefFail = TaskDefMock(taskClass=TaskMockFail)
-        taskDefLongSleep = TaskDefMock(taskClass=TaskMockLongSleep)
+        task_node = TaskNodeMock()
+        task_node_fail = TaskNodeMock(task_class=TaskMockFail)
+        task_nodeLongSleep = TaskNodeMock(task_class=TaskMockLongSleep)
         qdata = [
-            QuantumIterDataMock(index=0, taskDef=taskDef, detector=0),
-            QuantumIterDataMock(index=1, taskDef=taskDefFail, detector=1),
-            QuantumIterDataMock(index=2, taskDef=taskDef, detector=2),
-            QuantumIterDataMock(index=3, taskDef=taskDefLongSleep, detector=3),
-            QuantumIterDataMock(index=4, taskDef=taskDef, detector=4),
+            QuantumIterDataMock(index=0, task_node=task_node, detector=0),
+            QuantumIterDataMock(index=1, task_node=task_node_fail, detector=1),
+            QuantumIterDataMock(index=2, task_node=task_node, detector=2),
+            QuantumIterDataMock(index=3, task_node=task_nodeLongSleep, detector=3),
+            QuantumIterDataMock(index=4, task_node=task_node, detector=4),
         ]
         qdata[1].dependencies.add(0)
         qdata[2].dependencies.add(1)
         qdata[4].dependencies.add(3)
         qdata[4].dependencies.add(2)
 
         qgraph = QuantumGraphMock(qdata)
@@ -555,21 +579,21 @@
         self.assertGreater(len(report.quantaReports), 0)
         self.assertEqual(_count_status(report, ExecutionStatus.FAILURE), 1)
         self.assertTrue(any(qrep.exitCode > 0 for qrep in report.quantaReports))
         self.assertTrue(any(qrep.exceptionInfo is not None for qrep in report.quantaReports))
 
     def test_mpexec_crash(self):
         """Check task crash due to signal."""
-        taskDef = TaskDefMock()
-        taskDefCrash = TaskDefMock(taskClass=TaskMockCrash)
+        task_node = TaskNodeMock()
+        task_node_crash = TaskNodeMock(task_class=TaskMockCrash)
         qgraph = QuantumGraphMock(
             [
-                QuantumIterDataMock(index=0, taskDef=taskDef, detector=0),
-                QuantumIterDataMock(index=1, taskDef=taskDefCrash, detector=1),
-                QuantumIterDataMock(index=2, taskDef=taskDef, detector=2),
+                QuantumIterDataMock(index=0, task_node=task_node, detector=0),
+                QuantumIterDataMock(index=1, task_node=task_node_crash, detector=1),
+                QuantumIterDataMock(index=2, task_node=task_node, detector=2),
             ]
         )
 
         qexec = QuantumExecutorMock(mp=True)
         mpexec = MPGraphExecutor(numProc=3, timeout=100, quantumExecutor=qexec)
         with self.assertRaisesRegex(MPGraphExecutorError, "One or more tasks failed"):
             mpexec.execute(qgraph)
@@ -583,21 +607,21 @@
         self.assertEqual(_count_status(report, ExecutionStatus.FAILURE), 1)
         self.assertEqual(_count_status(report, ExecutionStatus.SUCCESS), 2)
         self.assertTrue(any(qrep.exitCode == -signal.SIGILL for qrep in report.quantaReports))
         self.assertTrue(all(qrep.exceptionInfo is None for qrep in report.quantaReports))
 
     def test_mpexec_crash_failfast(self):
         """Check task crash due to signal with --fail-fast."""
-        taskDef = TaskDefMock()
-        taskDefCrash = TaskDefMock(taskClass=TaskMockCrash)
+        task_node = TaskNodeMock()
+        task_node_crash = TaskNodeMock(task_class=TaskMockCrash)
         qgraph = QuantumGraphMock(
             [
-                QuantumIterDataMock(index=0, taskDef=taskDef, detector=0),
-                QuantumIterDataMock(index=1, taskDef=taskDefCrash, detector=1),
-                QuantumIterDataMock(index=2, taskDef=taskDef, detector=2),
+                QuantumIterDataMock(index=0, task_node=task_node, detector=0),
+                QuantumIterDataMock(index=1, task_node=task_node_crash, detector=1),
+                QuantumIterDataMock(index=2, task_node=task_node, detector=2),
             ]
         )
 
         qexec = QuantumExecutorMock(mp=True)
         mpexec = MPGraphExecutor(numProc=3, timeout=100, quantumExecutor=qexec, failFast=True)
         with self.assertRaisesRegex(MPGraphExecutorError, "failed, killed by signal 4 .Illegal instruction"):
             mpexec.execute(qgraph)
@@ -608,17 +632,17 @@
         )
         self.assertEqual(_count_status(report, ExecutionStatus.FAILURE), 1)
         self.assertTrue(any(qrep.exitCode == -signal.SIGILL for qrep in report.quantaReports))
         self.assertTrue(all(qrep.exceptionInfo is None for qrep in report.quantaReports))
 
     def test_mpexec_num_fd(self):
         """Check that number of open files stays reasonable."""
-        taskDef = TaskDefMock()
+        task_node = TaskNodeMock()
         qgraph = QuantumGraphMock(
-            [QuantumIterDataMock(index=i, taskDef=taskDef, detector=i) for i in range(20)]
+            [QuantumIterDataMock(index=i, task_node=task_node, detector=i) for i in range(20)]
         )
 
         this_proc = psutil.Process()
         num_fds_0 = this_proc.num_fds()
 
         # run in multi-process mode, the order of results is not defined
         qexec = QuantumExecutorMock(mp=True)
@@ -650,15 +674,15 @@
 
         nodes = list(qgraph)
         self.assertEqual(len(nodes), nQuanta)
         node = nodes[0]
 
         taskFactory = AddTaskFactoryMock()
         executor = SingleQuantumExecutor(butler, taskFactory)
-        executor.execute(node.taskDef, node.quantum)
+        executor.execute(node.task_node, node.quantum)
         self.assertEqual(taskFactory.countExec, 1)
 
         # There must be one dataset of task's output connection
         refs = list(butler.registry.queryDatasets("add_dataset1", collections=butler.run))
         self.assertEqual(len(refs), 1)
 
     def test_skip_existing_execute(self) -> None:
@@ -668,25 +692,25 @@
 
         nodes = list(qgraph)
         self.assertEqual(len(nodes), nQuanta)
         node = nodes[0]
 
         taskFactory = AddTaskFactoryMock()
         executor = SingleQuantumExecutor(butler, taskFactory)
-        executor.execute(node.taskDef, node.quantum)
+        executor.execute(node.task_node, node.quantum)
         self.assertEqual(taskFactory.countExec, 1)
 
         refs = list(butler.registry.queryDatasets("add_dataset1", collections=butler.run))
         self.assertEqual(len(refs), 1)
         dataset_id_1 = refs[0].id
 
         # Re-run it with skipExistingIn, it should not run.
         assert butler.run is not None
         executor = SingleQuantumExecutor(butler, taskFactory, skipExistingIn=[butler.run])
-        executor.execute(node.taskDef, node.quantum)
+        executor.execute(node.task_node, node.quantum)
         self.assertEqual(taskFactory.countExec, 1)
 
         refs = list(butler.registry.queryDatasets("add_dataset1", collections=butler.run))
         self.assertEqual(len(refs), 1)
         dataset_id_2 = refs[0].id
         self.assertEqual(dataset_id_1, dataset_id_2)
 
@@ -697,15 +721,15 @@
 
         nodes = list(qgraph)
         self.assertEqual(len(nodes), nQuanta)
         node = nodes[0]
 
         taskFactory = AddTaskFactoryMock()
         executor = SingleQuantumExecutor(butler, taskFactory)
-        executor.execute(node.taskDef, node.quantum)
+        executor.execute(node.task_node, node.quantum)
         self.assertEqual(taskFactory.countExec, 1)
 
         refs = list(butler.registry.queryDatasets("add_dataset1", collections=butler.run))
         self.assertEqual(len(refs), 1)
         dataset_id_1 = refs[0].id
 
         original_dataset = butler.get(refs[0])
@@ -718,30 +742,30 @@
 
         # Re-run it with clobberOutputs and skipExistingIn, it should not
         # clobber but should skip instead.
         assert butler.run is not None
         executor = SingleQuantumExecutor(
             butler, taskFactory, skipExistingIn=[butler.run], clobberOutputs=True
         )
-        executor.execute(node.taskDef, node.quantum)
+        executor.execute(node.task_node, node.quantum)
         self.assertEqual(taskFactory.countExec, 1)
 
         refs = list(butler.registry.queryDatasets("add_dataset1", collections=butler.run))
         self.assertEqual(len(refs), 1)
         dataset_id_2 = refs[0].id
         self.assertEqual(dataset_id_1, dataset_id_2)
 
         second_dataset = butler.get(refs[0])
         self.assertEqual(list(second_dataset), list(replacement))
 
         # Re-run it with clobberOutputs but without skipExistingIn, it should
         # clobber.
         assert butler.run is not None
         executor = SingleQuantumExecutor(butler, taskFactory, clobberOutputs=True)
-        executor.execute(node.taskDef, node.quantum)
+        executor.execute(node.task_node, node.quantum)
         self.assertEqual(taskFactory.countExec, 2)
 
         refs = list(butler.registry.queryDatasets("add_dataset1", collections=butler.run))
         self.assertEqual(len(refs), 1)
         dataset_id_3 = refs[0].id
 
         third_dataset = butler.get(refs[0])
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_preExecInit.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_preExecInit.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_reports.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_reports.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import unittest
 
 from lsst.ctrl.mpexec import ExecutionStatus, QuantumReport, Report
+from lsst.pipe.base import QgraphSummary
 
 
 class ReportsTestCase(unittest.TestCase):
     """A test case for reports module."""
 
     def test_quantumReport(self):
         """Test for QuantumReport class."""
@@ -70,27 +71,29 @@
         self.assertEqual(qr.dataId, dataId)
         self.assertEqual(qr.taskLabel, taskLabel)
         self.assertEqual(qr.exitCode, 1)
         self.assertIsNone(qr.exceptionInfo)
 
     def test_report(self):
         """Test for Report class."""
-        report = Report()
+        report = Report(qgraphSummary=QgraphSummary(graphID="uuid"))
         self.assertEqual(report.status, ExecutionStatus.SUCCESS)
         self.assertIsNotNone(report.cmdLine)
         self.assertIsNone(report.exitCode)
         self.assertIsNone(report.exceptionInfo)
 
         dataId = {"instrument": "LSST"}
         taskLabel = "task"
 
         qr = QuantumReport.from_exception(
             exception=RuntimeError("runtime error"), dataId=dataId, taskLabel=taskLabel
         )
-        report = Report(status=ExecutionStatus.FAILURE, exitCode=-1)
+        report = Report(
+            status=ExecutionStatus.FAILURE, exitCode=-1, qgraphSummary=QgraphSummary(graphID="uuid")
+        )
         report.set_exception(RuntimeError("runtime error"))
         report.quantaReports.append(qr)
         self.assertEqual(report.status, ExecutionStatus.FAILURE)
         self.assertEqual(report.exitCode, -1)
         self.assertEqual(report.exceptionInfo.className, "RuntimeError")
         self.assertEqual(report.exceptionInfo.message, "runtime error")
         self.assertEqual(len(report.quantaReports), 1)
@@ -99,15 +102,17 @@
         """Test for conversion to/from JSON."""
         dataId = {"instrument": "LSST"}
         taskLabel = "task"
 
         qr = QuantumReport.from_exception(
             exception=RuntimeError("runtime error"), dataId=dataId, taskLabel=taskLabel
         )
-        report = Report(status=ExecutionStatus.FAILURE, exitCode=-1)
+        report = Report(
+            status=ExecutionStatus.FAILURE, exitCode=-1, qgraphSummary=QgraphSummary(graphID="uuid")
+        )
         report.set_exception(RuntimeError("runtime error"))
         report.quantaReports.append(qr)
         json = report.model_dump_json(exclude_none=True, indent=2)
         self.assertIsInstance(json, str)
 
         report = Report.model_validate_json(json)
         self.assertEqual(report.status, ExecutionStatus.FAILURE)
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_separablePipelineExecutor.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_separablePipelineExecutor.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 import unittest
 
 import lsst.daf.butler
 import lsst.daf.butler.tests as butlerTests
 import lsst.pex.config
 import lsst.utils.tests
 from lsst.ctrl.mpexec import SeparablePipelineExecutor
-from lsst.pipe.base import Instrument, Pipeline, PipelineDatasetTypes, TaskMetadata
+from lsst.pipe.base import Instrument, Pipeline, TaskMetadata
+from lsst.pipe.base.automatic_connection_constants import PACKAGES_INIT_OUTPUT_NAME
+from lsst.pipe.base.quantum_graph_builder import OutputExistsError
 from lsst.resources import ResourcePath
 
 TESTDIR = os.path.abspath(os.path.dirname(__file__))
 
 
 class SeparablePipelineExecutorTests(lsst.utils.tests.TestCase):
     """Test the SeparablePipelineExecutor API with a trivial task."""
@@ -78,24 +80,24 @@
         self.butler.put({"zero": 0}, "input")
         graph = executor.make_quantum_graph(pipeline)
 
         butlerTests.addDatasetType(self.butler, "output", set(), "StructuredDataDict")
         butlerTests.addDatasetType(self.butler, "b_config", set(), "Config")
         butlerTests.addDatasetType(self.butler, "b_log", set(), "ButlerLogRecords")
         butlerTests.addDatasetType(self.butler, "b_metadata", set(), "TaskMetadata")
-        butlerTests.addDatasetType(self.butler, PipelineDatasetTypes.packagesDatasetName, set(), "Packages")
+        butlerTests.addDatasetType(self.butler, PACKAGES_INIT_OUTPUT_NAME, set(), "Packages")
 
         executor.pre_execute_qgraph(
             graph,
             register_dataset_types=False,
             save_init_outputs=False,
             save_versions=False,
         )
         self.assertFalse(self.butler.exists("a_config", {}, collections=[self.butler.run]))
-        self.assertFalse(self.butler.exists(PipelineDatasetTypes.packagesDatasetName, {}))
+        self.assertFalse(self.butler.exists(PACKAGES_INIT_OUTPUT_NAME, {}))
 
     def test_pre_execute_qgraph_unconnected(self):
         # Unconnected graph; see
         # test_make_quantum_graph_nowhere_skippartial_clobber.
         executor = SeparablePipelineExecutor(
             self.butler,
             skip_existing_in=[self.butler.run],
@@ -106,43 +108,43 @@
         self.butler.put({"zero": 0}, "intermediate")
         graph = executor.make_quantum_graph(pipeline)
 
         butlerTests.addDatasetType(self.butler, "output", set(), "StructuredDataDict")
         butlerTests.addDatasetType(self.butler, "b_config", set(), "Config")
         butlerTests.addDatasetType(self.butler, "b_log", set(), "ButlerLogRecords")
         butlerTests.addDatasetType(self.butler, "b_metadata", set(), "TaskMetadata")
-        butlerTests.addDatasetType(self.butler, PipelineDatasetTypes.packagesDatasetName, set(), "Packages")
+        butlerTests.addDatasetType(self.butler, PACKAGES_INIT_OUTPUT_NAME, set(), "Packages")
 
         executor.pre_execute_qgraph(
             graph,
             register_dataset_types=False,
             save_init_outputs=False,
             save_versions=False,
         )
         self.assertFalse(self.butler.exists("a_config", {}, collections=[self.butler.run]))
-        self.assertFalse(self.butler.exists(PipelineDatasetTypes.packagesDatasetName, {}))
+        self.assertFalse(self.butler.exists(PACKAGES_INIT_OUTPUT_NAME, {}))
 
     def test_pre_execute_qgraph_empty(self):
         executor = SeparablePipelineExecutor(self.butler)
         graph = lsst.pipe.base.QuantumGraph({}, universe=self.butler.dimensions)
 
         butlerTests.addDatasetType(self.butler, "output", set(), "StructuredDataDict")
         butlerTests.addDatasetType(self.butler, "b_config", set(), "Config")
         butlerTests.addDatasetType(self.butler, "b_log", set(), "ButlerLogRecords")
         butlerTests.addDatasetType(self.butler, "b_metadata", set(), "TaskMetadata")
-        butlerTests.addDatasetType(self.butler, PipelineDatasetTypes.packagesDatasetName, set(), "Packages")
+        butlerTests.addDatasetType(self.butler, PACKAGES_INIT_OUTPUT_NAME, set(), "Packages")
 
         executor.pre_execute_qgraph(
             graph,
             register_dataset_types=False,
             save_init_outputs=False,
             save_versions=False,
         )
         self.assertFalse(self.butler.exists("a_config", {}, collections=[self.butler.run]))
-        self.assertFalse(self.butler.exists(PipelineDatasetTypes.packagesDatasetName, {}))
+        self.assertFalse(self.butler.exists(PACKAGES_INIT_OUTPUT_NAME, {}))
 
     def test_pre_execute_qgraph_register(self):
         executor = SeparablePipelineExecutor(self.butler)
         pipeline = Pipeline.fromFile(self.pipeline_file)
         self.butler.put({"zero": 0}, "input")
         graph = executor.make_quantum_graph(pipeline)
 
@@ -154,58 +156,58 @@
         )
         self.assertEqual({d.name for d in self.butler.registry.queryDatasetTypes("output")}, {"output"})
         self.assertEqual(
             {d.name for d in self.butler.registry.queryDatasetTypes("b_*")},
             {"b_config", "b_log", "b_metadata"},
         )
         self.assertFalse(self.butler.exists("a_config", {}, collections=[self.butler.run]))
-        self.assertFalse(self.butler.exists(PipelineDatasetTypes.packagesDatasetName, {}))
+        self.assertFalse(self.butler.exists(PACKAGES_INIT_OUTPUT_NAME, {}))
 
     def test_pre_execute_qgraph_init_outputs(self):
         # Too hard to make a quantum graph from scratch.
         executor = SeparablePipelineExecutor(self.butler)
         pipeline = Pipeline.fromFile(self.pipeline_file)
         self.butler.put({"zero": 0}, "input")
         graph = executor.make_quantum_graph(pipeline)
 
         butlerTests.addDatasetType(self.butler, "output", set(), "StructuredDataDict")
         butlerTests.addDatasetType(self.butler, "b_config", set(), "Config")
         butlerTests.addDatasetType(self.butler, "b_log", set(), "ButlerLogRecords")
         butlerTests.addDatasetType(self.butler, "b_metadata", set(), "TaskMetadata")
-        butlerTests.addDatasetType(self.butler, PipelineDatasetTypes.packagesDatasetName, set(), "Packages")
+        butlerTests.addDatasetType(self.butler, PACKAGES_INIT_OUTPUT_NAME, set(), "Packages")
 
         executor.pre_execute_qgraph(
             graph,
             register_dataset_types=False,
             save_init_outputs=True,
             save_versions=False,
         )
         self.assertTrue(self.butler.exists("a_config", {}, collections=[self.butler.run]))
-        self.assertFalse(self.butler.exists(PipelineDatasetTypes.packagesDatasetName, {}))
+        self.assertFalse(self.butler.exists(PACKAGES_INIT_OUTPUT_NAME, {}))
 
     def test_pre_execute_qgraph_versions(self):
         executor = SeparablePipelineExecutor(self.butler)
         pipeline = Pipeline.fromFile(self.pipeline_file)
         self.butler.put({"zero": 0}, "input")
         graph = executor.make_quantum_graph(pipeline)
 
         butlerTests.addDatasetType(self.butler, "output", set(), "StructuredDataDict")
         butlerTests.addDatasetType(self.butler, "b_config", set(), "Config")
         butlerTests.addDatasetType(self.butler, "b_log", set(), "ButlerLogRecords")
         butlerTests.addDatasetType(self.butler, "b_metadata", set(), "TaskMetadata")
-        butlerTests.addDatasetType(self.butler, PipelineDatasetTypes.packagesDatasetName, set(), "Packages")
+        butlerTests.addDatasetType(self.butler, PACKAGES_INIT_OUTPUT_NAME, set(), "Packages")
 
         executor.pre_execute_qgraph(
             graph,
             register_dataset_types=False,
             save_init_outputs=True,
             save_versions=True,
         )
         self.assertTrue(self.butler.exists("a_config", {}, collections=[self.butler.run]))
-        self.assertTrue(self.butler.exists(PipelineDatasetTypes.packagesDatasetName, {}))
+        self.assertTrue(self.butler.exists(PACKAGES_INIT_OUTPUT_NAME, {}))
 
     def test_init_badinput(self):
         butler = lsst.daf.butler.Butler.from_config(butler=self.butler, collections=[], run="foo")
 
         with self.assertRaises(ValueError):
             SeparablePipelineExecutor(butler)
 
@@ -218,29 +220,27 @@
     def test_make_pipeline_full(self):
         executor = SeparablePipelineExecutor(self.butler)
         for uri in [
             self.pipeline_file,
             ResourcePath(self.pipeline_file),
             ResourcePath(self.pipeline_file).geturl(),
         ]:
-            pipeline = executor.make_pipeline(uri)
-            self.assertEqual(len(pipeline), 2)
-            self.assertEqual({t.label for t in pipeline}, {"a", "b"})
+            pipeline_graph = executor.make_pipeline(uri).to_graph()
+            self.assertEqual(set(pipeline_graph.tasks), {"a", "b"})
 
     def test_make_pipeline_subset(self):
         executor = SeparablePipelineExecutor(self.butler)
         path = self.pipeline_file + "#a"
         for uri in [
             path,
             ResourcePath(path),
             ResourcePath(path).geturl(),
         ]:
-            pipeline = executor.make_pipeline(uri)
-            self.assertEqual(len(pipeline), 1)
-            self.assertEqual({t.label for t in pipeline}, {"a"})
+            pipeline_graph = executor.make_pipeline(uri).to_graph()
+            self.assertEqual(set(pipeline_graph.tasks), {"a"})
 
     def test_make_quantum_graph_nowhere_noskip_noclobber(self):
         executor = SeparablePipelineExecutor(self.butler, skip_existing_in=None, clobber_output=False)
         pipeline = Pipeline.fromFile(self.pipeline_file)
 
         self.butler.put({"zero": 0}, "input")
 
@@ -255,15 +255,15 @@
         pipeline = Pipeline.fromFile(self.pipeline_file)
 
         self.butler.put({"zero": 0}, "input")
         self.butler.put({"zero": 0}, "intermediate")
         self.butler.put(lsst.daf.butler.ButlerLogRecords.from_records([]), "a_log")
         self.butler.put(TaskMetadata(), "a_metadata")
 
-        with self.assertRaises(lsst.pipe.base.graphBuilder.OutputExistsError):
+        with self.assertRaises(OutputExistsError):
             executor.make_quantum_graph(pipeline)
 
     # TODO: need more complex task and Butler to test
     # make_quantum_graph(where=...)
 
     def test_make_quantum_graph_nowhere_skipnone_noclobber(self):
         executor = SeparablePipelineExecutor(
@@ -308,15 +308,15 @@
             clobber_output=False,
         )
         pipeline = Pipeline.fromFile(self.pipeline_file)
 
         self.butler.put({"zero": 0}, "input")
         self.butler.put({"zero": 0}, "intermediate")
 
-        with self.assertRaises(lsst.pipe.base.graphBuilder.OutputExistsError):
+        with self.assertRaises(OutputExistsError):
             executor.make_quantum_graph(pipeline)
 
     def test_make_quantum_graph_nowhere_noskip_clobber(self):
         executor = SeparablePipelineExecutor(self.butler, skip_existing_in=None, clobber_output=True)
         pipeline = Pipeline.fromFile(self.pipeline_file)
 
         self.butler.put({"zero": 0}, "input")
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_simple_pipeline_executor.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_simple_pipeline_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 import tempfile
 import unittest
 from typing import Any
 
 import lsst.daf.butler
 import lsst.utils.tests
 from lsst.ctrl.mpexec import SimplePipelineExecutor
-from lsst.pipe.base import Struct, TaskDef, TaskMetadata, connectionTypes
+from lsst.pipe.base import PipelineGraph, Struct, TaskMetadata, connectionTypes
+from lsst.pipe.base.pipeline_graph import IncompatibleDatasetTypeError
 from lsst.pipe.base.tests.no_dimensions import (
     NoDimensionsTestConfig,
     NoDimensionsTestConnections,
     NoDimensionsTestTask,
 )
 from lsst.utils.introspection import get_full_type_name
 
@@ -144,30 +145,29 @@
         `SimplePipelineExecutor.as_generator` method.
         """
         executor = SimplePipelineExecutor.from_task_class(NoDimensionsTestTask, butler=self.butler)
         (quantum,) = executor.as_generator(register_dataset_types=True)
         self.assertEqual(self.butler.get("output"), {"zero": 0, "one": 1})
 
     def _configure_pipeline(self, config_a_cls, config_b_cls, storageClass_a=None, storageClass_b=None):
-        """Configure a pipeline with from_pipeline."""
+        """Configure a pipeline with from_pipeline_graph."""
         config_a = config_a_cls()
         config_a.connections.output = "intermediate"
         if storageClass_a:
             config_a.outputSC = storageClass_a
         config_b = config_b_cls()
         config_b.connections.input = "intermediate"
         if storageClass_b:
             config_b.outputSC = storageClass_b
         config_b.key = "two"
         config_b.value = 2
-        task_defs = [
-            TaskDef(label="a", taskClass=NoDimensionsTestTask, config=config_a),
-            TaskDef(label="b", taskClass=NoDimensionsTestTask, config=config_b),
-        ]
-        executor = SimplePipelineExecutor.from_pipeline(task_defs, butler=self.butler)
+        pipeline_graph = PipelineGraph()
+        pipeline_graph.add_task("a", NoDimensionsTestTask, config_a)
+        pipeline_graph.add_task("b", NoDimensionsTestTask, config_b)
+        executor = SimplePipelineExecutor.from_pipeline_graph(pipeline_graph, butler=self.butler)
         return executor
 
     def _test_logs(self, log_output, input_type_a, output_type_a, input_type_b, output_type_b):
         """Check the expected input types received by tasks A and B.
 
         Note that these are the types as seen from the perspective of the task,
         so they must be consistent with the task's connections, but may not be
@@ -250,16 +250,16 @@
             quanta = executor.run(register_dataset_types=True, save_versions=False)
         # a has been told to return a TaskMetadata but this will convert to
         # dict on read by b.
         # b returns a dict and that is converted to TaskMetadata on put.
         self._test_logs(cm.output, "dict", "lsst.pipe.base.TaskMetadata", "dict", "dict")
 
         self.assertEqual(len(quanta), 2)
-        self.assertEqual(self.butler.get("intermediate"), TaskMetadata.from_dict({"zero": 0, "one": 1}))
-        self.assertEqual(self.butler.get("output"), TaskMetadata.from_dict({"zero": 0, "one": 1, "two": 2}))
+        self.assertEqual(self.butler.get("intermediate").to_dict(), {"zero": 0, "one": 1})
+        self.assertEqual(self.butler.get("output").to_dict(), {"zero": 0, "one": 1, "two": 2})
 
     def test_from_pipeline_input_differ(self):
         """Run pipeline but input definition in registry differs."""
         # This config declares that the pipeline takes a TaskMetadata
         # as input but registry already thinks it has a StructureDataDict.
         executor = self._configure_pipeline(NoDimensionsTestConfig2, NoDimensionsTestTask.ConfigClass)
 
@@ -267,51 +267,67 @@
             quanta = executor.run(register_dataset_types=True, save_versions=False)
         self._test_logs(cm.output, "lsst.pipe.base.TaskMetadata", "dict", "dict", "dict")
 
         self.assertEqual(len(quanta), 2)
         self.assertEqual(self.butler.get("intermediate"), {"zero": 0, "one": 1})
         self.assertEqual(self.butler.get("output"), {"zero": 0, "one": 1, "two": 2})
 
-    def test_from_pipeline_inconsistent_dataset_types(self):
-        """Generate the QG (by initializing the executor), then register the
-        dataset type with a different storage class than the QG should have
-        predicted, to make sure execution fails as it should.
+    def test_from_pipeline_incompatible(self):
+        """Test that we cannot make a QG if the registry and pipeline have
+        incompatible storage classes for a dataset type.
         """
-        executor = self._configure_pipeline(
-            NoDimensionsTestTask.ConfigClass, NoDimensionsTestTask.ConfigClass
-        )
-
         # Incompatible output dataset type.
         self.butler.registry.registerDatasetType(
             lsst.daf.butler.DatasetType(
                 "output",
                 dimensions=self.butler.dimensions.empty,
                 storageClass="StructuredDataList",
             )
         )
+        with self.assertRaisesRegex(
+            IncompatibleDatasetTypeError, "Incompatible definition.*StructuredDataDict.*StructuredDataList.*"
+        ):
+            self._configure_pipeline(NoDimensionsTestTask.ConfigClass, NoDimensionsTestTask.ConfigClass)
 
+    def test_from_pipeline_registry_changed(self):
+        """Run pipeline, but change registry dataset types between making the
+        QG and executing it.
+
+        This only fails with full-butler execution; we don't have a way to
+        prevent it with QBB.
+        """
+        executor = self._configure_pipeline(
+            NoDimensionsTestTask.ConfigClass, NoDimensionsTestTask.ConfigClass
+        )
+        self.butler.registry.registerDatasetType(
+            lsst.daf.butler.DatasetType(
+                "output",
+                dimensions=self.butler.dimensions.empty,
+                storageClass="TaskMetadataLike",  # even compatible is not okay
+            )
+        )
         with self.assertRaisesRegex(
-            ValueError, "StructuredDataDict.*inconsistent with registry definition.*StructuredDataList"
+            lsst.daf.butler.registry.ConflictingDefinitionError,
+            ".*definition in registry has changed.*StructuredDataDict.*TaskMetadataLike.*",
         ):
             executor.run(register_dataset_types=True, save_versions=False)
 
     def test_from_pipeline_metadata(self):
         """Test two tasks where the output uses metadata from input."""
         # Must configure a special pipeline for this test.
         config_a = NoDimensionsTestTask.ConfigClass()
         config_a.connections.output = "intermediate"
         config_b = NoDimensionsMetadataTestTask.ConfigClass()
         config_b.connections.input = "intermediate"
         config_b.key = "two"
         config_b.value = 2
-        task_defs = [
-            TaskDef(label="a", taskClass=NoDimensionsTestTask, config=config_a),
-            TaskDef(label="b", taskClass=NoDimensionsMetadataTestTask, config=config_b),
-        ]
-        executor = SimplePipelineExecutor.from_pipeline(task_defs, butler=self.butler)
+        pipeline_graph = PipelineGraph()
+        pipeline_graph.add_task("a", NoDimensionsTestTask, config=config_a)
+        pipeline_graph.add_task("b", NoDimensionsMetadataTestTask, config=config_b)
+        executor = SimplePipelineExecutor.from_pipeline_graph(pipeline_graph, butler=self.butler)
 
         with self.assertLogs("test_simple_pipeline_executor", level="INFO") as cm:
             quanta = executor.run(register_dataset_types=True, save_versions=False)
         self.assertIn(f"Received task metadata ({get_full_type_name(dict)})", "".join(cm.output))
 
         self.assertEqual(len(quanta), 2)
         self.assertEqual(self.butler.get("intermediate"), {"zero": 0, "one": 1})
```

### Comparing `lsst-ctrl-mpexec-26.2024.900/tests/test_taskFactory.py` & `lsst_ctrl_mpexec-27.0.0rc1/tests/test_taskFactory.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 import tempfile
 import unittest
 from typing import TYPE_CHECKING
 
 import lsst.daf.butler.tests as butlerTests
 import lsst.pex.config as pexConfig
 from lsst.ctrl.mpexec import TaskFactory
-from lsst.pipe.base import PipelineTaskConfig, PipelineTaskConnections, TaskDef, connectionTypes
+from lsst.pipe.base import PipelineGraph, PipelineTaskConfig, PipelineTaskConnections, connectionTypes
 
 if TYPE_CHECKING:
     from lsst.daf.butler import Butler, DatasetRef
 
 # Storage class to use for tests of fakes.
 _FAKE_STORAGE_CLASS = "StructuredDataDict"
 
@@ -110,23 +110,25 @@
         catalog = self._dummyCatalog()
         refs = {}
         for dataset_type in ("fakeInitInput", "fakeInitOutput", "fakeInput", "fakeOutput"):
             refs[dataset_type] = butler.put(catalog, dataset_type)
         return butler, refs
 
     def testDefaultConfigLabel(self) -> None:
-        task_def = TaskDef(taskClass=self.constructor, label=None, config=None)
+        pipeline_graph = PipelineGraph()
+        task_node = pipeline_graph.add_task(None, self.constructor)
         butler, _ = self._tempButler()
-        self.factory.makeTask(taskDef=task_def, butler=butler, initInputRefs=[])
+        self.factory.makeTask(task_node, butler=butler, initInputRefs=[])
         self.constructor.assert_called_with(config=FakeConfig(), initInputs={}, name="FakeTask")
 
     def testAllArgs(self) -> None:
         config = self._alteredConfig()
-        task_def = TaskDef(taskClass=self.constructor, label="no-name", config=config)
+        pipeline_graph = PipelineGraph()
+        task_node = pipeline_graph.add_task("no-name", self.constructor, config=config)
         butler, refs = self._tempButler()
-        self.factory.makeTask(taskDef=task_def, butler=butler, initInputRefs=[refs["fakeInitInput"]])
+        self.factory.makeTask(task_node, butler=butler, initInputRefs=[refs["fakeInitInput"]])
         catalog = butler.get("fakeInitInput")
         self.constructor.assert_called_with(config=config, initInputs={"initInput": catalog}, name="no-name")
 
 
 if __name__ == "__main__":
     unittest.main()
```

