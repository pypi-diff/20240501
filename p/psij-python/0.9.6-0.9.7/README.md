# Comparing `tmp/psij-python-0.9.6.tar.gz` & `tmp/psij-python-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psij-python-0.9.6.tar", last modified: Mon Apr  8 19:34:53 2024, max compression
+gzip compressed data, was "psij-python-0.9.7.tar", last modified: Wed May  1 04:39:00 2024, max compression
```

## Comparing `psij-python-0.9.6.tar` & `psij-python-0.9.7.tar`

### file list

```diff
@@ -1,105 +1,107 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.593047 psij-python-0.9.6/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1065 2024-04-08 19:34:25.000000 psij-python-0.9.6/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      399 2024-04-08 19:34:53.593047 psij-python-0.9.6/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      904 2024-04-08 19:34:25.000000 psij-python-0.9.6/README.md
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-08 19:34:53.593047 psij-python-0.9.6/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     1221 2024-04-08 19:34:25.000000 psij-python-0.9.6/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.585047 psij-python-0.9.6/src/
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/
--rw-rw-r--   0 mike      (1000) mike      (1000)     3577 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      243 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/__main__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4766 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/_plugins.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4875 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3003 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/exceptions.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/executors/
--rw-rw-r--   0 mike      (1000) mike      (1000)      341 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/__init__.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/executors/batch/
--rw-rw-r--   0 mike      (1000) mike      (1000)       86 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    31379 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/batch_scheduler_executor.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/executors/batch/cobalt/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1769 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/cobalt/cobalt.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)     5704 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/cobalt.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      807 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/escape_functions.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/executors/batch/lsf/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1824 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/lsf/lsf.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)     6177 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/lsf.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/executors/batch/pbs/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1596 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/pbs/pbs_classic.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)     1685 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/pbs/pbspro.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)      988 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/pbs.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     7118 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/pbs_base.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1138 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/pbs_classic.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3248 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/script_generator.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij/executors/batch/slurm/
--rw-rw-r--   0 mike      (1000) mike      (1000)     3235 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/slurm/slurm.mustache
--rw-rw-r--   0 mike      (1000) mike      (1000)     9839 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/slurm.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2343 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/batch/template_function_library.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     7359 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/flux.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    15054 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/local.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6220 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/executors/rp.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    10706 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6367 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_attributes.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    14194 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_executor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2721 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_executor_config.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4624 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_launcher.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    12790 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_spec.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4985 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_state.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1995 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/job_status.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4280 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launcher.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.593047 psij-python-0.9.6/src/psij/launchers/
--rw-rw-r--   0 mike      (1000) mike      (1000)      623 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      557 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/aprun.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      554 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/jsrun.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      692 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/mpirun.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1718 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/multiple.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     8023 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/script_based_launcher.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.593047 psij-python-0.9.6/src/psij/launchers/scripts/
--rw-rw-r--   0 mike      (1000) mike      (1000)       69 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      300 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/aprun_launch.sh
--rwxrwxr-x   0 mike      (1000) mike      (1000)      307 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/jsrun_launch.sh
--rwxrwxr-x   0 mike      (1000) mike      (1000)      812 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/launcher_lib.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      546 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/mpi_launch.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      594 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/multi_launch.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      236 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/single_launch.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      274 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/scripts/srun_launch.sh
--rw-rw-r--   0 mike      (1000) mike      (1000)      643 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/single.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      660 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/launchers/srun.py
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/py.typed
--rw-rw-r--   0 mike      (1000) mike      (1000)     9052 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/resource_spec.py
--rw-rw-r--   0 mike      (1000) mike      (1000)    10549 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/serialize.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1881 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij/utils.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      168 2024-04-08 19:34:50.000000 psij-python-0.9.6/src/psij/version.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.589047 psij-python-0.9.6/src/psij-descriptors/
--rw-rw-r--   0 mike      (1000) mike      (1000)      217 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/aprun_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      262 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/cobalt_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      616 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/core_descriptors.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      248 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/flux_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      216 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/jsrun_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      250 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/lsf_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      564 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/pbs_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      285 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/rp_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      258 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/slurm_descriptor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      214 2024-04-08 19:34:25.000000 psij-python-0.9.6/src/psij-descriptors/srun_descriptor.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.593047 psij-python-0.9.6/src/psij_python.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      399 2024-04-08 19:34:53.000000 psij-python-0.9.6/src/psij_python.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     2821 2024-04-08 19:34:53.000000 psij-python-0.9.6/src/psij_python.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-08 19:34:53.000000 psij-python-0.9.6/src/psij_python.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       88 2024-04-08 19:34:53.000000 psij-python-0.9.6/src/psij_python.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       22 2024-04-08 19:34:53.000000 psij-python-0.9.6/src/psij_python.egg-info/top_level.txt
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-08 19:34:53.593047 psij-python-0.9.6/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)     2192 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_callbacks.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     4938 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_doc_examples.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     7986 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_executor.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      994 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_executor_loading.py
--rwxrwxr-x   0 mike      (1000) mike      (1000)      316 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_executor_versions.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      610 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_infrastructure.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_issue_387_1.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_issue_387_2.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_issue_387_3.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      589 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_issue_435.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1606 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_job_spec.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2159 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_mpi.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1209 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_nodefile.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3289 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_resources.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      836 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_serialization.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      911 2024-04-08 19:34:25.000000 psij-python-0.9.6/tests/test_wait.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.137713 psij-python-0.9.7/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1065 2024-05-01 04:36:19.000000 psij-python-0.9.7/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)       25 2024-05-01 04:36:19.000000 psij-python-0.9.7/MANIFEST.in
+-rw-rw-r--   0 mike      (1000) mike      (1000)      414 2024-05-01 04:39:00.137713 psij-python-0.9.7/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      904 2024-05-01 04:36:19.000000 psij-python-0.9.7/README.md
+-rw-rw-r--   0 mike      (1000) mike      (1000)       87 2024-05-01 04:36:19.000000 psij-python-0.9.7/requirements.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-05-01 04:39:00.137713 psij-python-0.9.7/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1213 2024-05-01 04:36:19.000000 psij-python-0.9.7/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.129711 psij-python-0.9.7/src/
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3577 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      243 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/__main__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4766 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/_plugins.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4875 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3003 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/exceptions.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/executors/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      341 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/__init__.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/executors/batch/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       86 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    31379 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/batch_scheduler_executor.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/executors/batch/cobalt/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1759 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/cobalt/cobalt.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5704 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/cobalt.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      807 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/escape_functions.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/executors/batch/lsf/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1814 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/lsf/lsf.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6177 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/lsf.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/executors/batch/pbs/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1586 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/pbs/pbs_classic.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1675 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/pbs/pbspro.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)      988 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/pbs.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7118 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/pbs_base.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1138 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/pbs_classic.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3248 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/script_generator.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/executors/batch/slurm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3225 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/slurm/slurm.mustache
+-rw-rw-r--   0 mike      (1000) mike      (1000)     9839 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/slurm.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2343 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/batch/template_function_library.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7359 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/flux.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    15054 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/local.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6220 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/executors/rp.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    10706 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7127 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_attributes.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    14194 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_executor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2721 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_executor_config.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4624 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_launcher.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    12790 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_spec.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4985 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_state.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1995 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/job_status.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4280 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launcher.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/launchers/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      623 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      557 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/aprun.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      554 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/jsrun.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      692 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/mpirun.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1718 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/multiple.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     8023 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/script_based_launcher.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij/launchers/scripts/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       69 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      300 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/aprun_launch.sh
+-rwxrwxr-x   0 mike      (1000) mike      (1000)      307 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/jsrun_launch.sh
+-rwxrwxr-x   0 mike      (1000) mike      (1000)      812 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/launcher_lib.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      546 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/mpi_launch.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      594 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/multi_launch.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      236 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/single_launch.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      274 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/scripts/srun_launch.sh
+-rw-rw-r--   0 mike      (1000) mike      (1000)      643 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/single.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      660 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/launchers/srun.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/py.typed
+-rw-rw-r--   0 mike      (1000) mike      (1000)     9052 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/resource_spec.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)    10549 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/serialize.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1881 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij/utils.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      168 2024-05-01 04:38:57.000000 psij-python-0.9.7/src/psij/version.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.133712 psij-python-0.9.7/src/psij-descriptors/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      217 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/aprun_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      262 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/cobalt_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      616 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/core_descriptors.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      248 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/flux_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      216 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/jsrun_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      250 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/lsf_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      564 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/pbs_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      285 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/rp_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      258 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/slurm_descriptor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      214 2024-05-01 04:36:19.000000 psij-python-0.9.7/src/psij-descriptors/srun_descriptor.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.137713 psij-python-0.9.7/src/psij_python.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      414 2024-05-01 04:39:00.000000 psij-python-0.9.7/src/psij_python.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2850 2024-05-01 04:39:00.000000 psij-python-0.9.7/src/psij_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-05-01 04:39:00.000000 psij-python-0.9.7/src/psij_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       88 2024-05-01 04:39:00.000000 psij-python-0.9.7/src/psij_python.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       22 2024-05-01 04:39:00.000000 psij-python-0.9.7/src/psij_python.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-01 04:39:00.137713 psij-python-0.9.7/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2192 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_callbacks.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4938 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_doc_examples.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7981 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_executor.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      994 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_executor_loading.py
+-rwxrwxr-x   0 mike      (1000) mike      (1000)      316 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_executor_versions.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      610 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_infrastructure.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_issue_387_1.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_issue_387_2.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      254 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_issue_387_3.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      589 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_issue_435.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1606 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_job_spec.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2159 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_mpi.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1209 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_nodefile.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3289 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_resources.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      836 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_serialization.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      911 2024-05-01 04:36:19.000000 psij-python-0.9.7/tests/test_wait.py
```

### Comparing `psij-python-0.9.6/LICENSE` & `psij-python-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/README.md` & `psij-python-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/setup.py` & `psij-python-0.9.7/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,16 +8,15 @@
     with open('requirements.txt') as f:
         install_requires = f.readlines()
 
     setup(
         name='psij-python',
         version=VERSION,
 
-        description='''This is an implementation of the PSI/J (Portable Submission Interface for Jobs)
-        specification.''',
+        description='''This is an implementation of the PSI/J (Portable Submission Interface for Jobs) specification.''',
 
         author='The ExaWorks Team',
         author_email='hategan@mcs.anl.gov',
 
         url='https://github.com/exaworks/psij-python',
 
         classifiers=[
```

### Comparing `psij-python-0.9.6/src/psij/__init__.py` & `psij-python-0.9.7/src/psij/__init__.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/_plugins.py` & `psij-python-0.9.7/src/psij/_plugins.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/descriptor.py` & `psij-python-0.9.7/src/psij/descriptor.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/exceptions.py` & `psij-python-0.9.7/src/psij/exceptions.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/executors/batch/batch_scheduler_executor.py` & `psij-python-0.9.7/src/psij/executors/batch/batch_scheduler_executor.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/executors/batch/cobalt/cobalt.mustache` & `psij-python-0.9.7/src/psij/executors/batch/cobalt/cobalt.mustache`

 * *Files 14% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 #COBALT --queue={{.}}
     {{/queue_name}}
     {{!Like PBS, Cobalt uses specially named queues for reservations, so we send the job to the
     respective queue when a reservation ID is specified.}}
     {{#reservation_id}}
 #COBALT --queue={{.}}
     {{/reservation_id}}
-    {{#project_name}}
+    {{#account}}
 #COBALT --project={{.}}
-    {{/project_name}}
+    {{/account}}
 {{/job.spec.attributes}}
 
 {{#custom_attributes}}
     {{#cobalt}}
 #COBALT --{{key}}="{{value}}"
     {{/cobalt}}
 {{/custom_attributes}}
```

### Comparing `psij-python-0.9.6/src/psij/executors/batch/cobalt.py` & `psij-python-0.9.7/src/psij/executors/batch/cobalt.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/executors/batch/escape_functions.py` & `psij-python-0.9.7/src/psij/executors/batch/escape_functions.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/executors/batch/lsf/lsf.mustache` & `psij-python-0.9.7/src/psij/executors/batch/lsf/lsf.mustache`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,18 @@
 {{/formatted_job_duration}}
 
 {{#job.spec.attributes}}
     {{#queue_name}}
 #BSUB -q "{{.}}"
     {{/queue_name}}
 
-    {{#project_name}}
+    {{#account}}
 #BSUB -G "{{.}}"
 #BSUB -P "{{.}}"
-    {{/project_name}}
+    {{/account}}
 
     {{#reservation_id}}
 #BSUB -U "{{.}}"
     {{/reservation_id}}
 
     {{#custom_attributes.lsf}}
 #BSUB -{{key}} "{{value}}"
```

### Comparing `psij-python-0.9.6/src/psij/executors/batch/lsf.py` & `psij-python-0.9.7/src/psij/executors/batch/lsf.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/executors/batch/pbs/pbs_classic.mustache` & `psij-python-0.9.7/src/psij/executors/batch/pbs/pbs_classic.mustache`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 {{/job.spec.resources}}
 
 {{#formatted_job_duration}}
 #PBS -l walltime={{.}}
 {{/formatted_job_duration}}
 
 {{#job.spec.attributes}}
-    {{#project_name}}
-#PBS -P {{.}}
-    {{/project_name}}
+    {{#account}}
+#PBS -A {{.}}
+    {{/account}}
     {{#queue_name}}
 #PBS -q {{.}}
     {{/queue_name}}
     {{!PBS uses specially named queues for reservations, so we send the job to the respective
     queue when a reservation ID is specified.}}
     {{#reservation_id}}
 #PBS -q {{.}}
```

### Comparing `psij-python-0.9.6/src/psij/executors/batch/pbs/pbspro.mustache` & `psij-python-0.9.7/src/psij/executors/batch/pbs/pbspro.mustache`

 * *Files 12% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 {{/job.spec.resources}}
 
 {{#formatted_job_duration}}
 #PBS -l walltime={{.}}
 {{/formatted_job_duration}}
 
 {{#job.spec.attributes}}
-    {{#project_name}}
-#PBS -P {{.}}
-    {{/project_name}}
+    {{#account}}
+#PBS -A {{.}}
+    {{/account}}
     {{#queue_name}}
 #PBS -q {{.}}
     {{/queue_name}}
     {{!PBS uses specially named queues for reservations, so we send the job to the respective
     queue when a reservation ID is specified.}}
     {{#reservation_id}}
 #PBS -q {{.}}
```

### Comparing `psij-python-0.9.6/src/psij/executors/batch/pbs.py` & `psij-python-0.9.7/src/psij/executors/batch/pbs.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/executors/batch/pbs_base.py` & `psij-python-0.9.7/src/psij/executors/batch/pbs_base.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/executors/batch/pbs_classic.py` & `psij-python-0.9.7/src/psij/executors/batch/pbs_classic.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/executors/batch/script_generator.py` & `psij-python-0.9.7/src/psij/executors/batch/script_generator.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/executors/batch/slurm/slurm.mustache` & `psij-python-0.9.7/src/psij/executors/batch/slurm/slurm.mustache`

 * *Files 6% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 {{/formatted_job_duration}}
 
 {{#job.spec.attributes}}
     {{#queue_name}}
 #SBATCH --partition="{{.}}"
     {{/queue_name}}
 
-    {{#project_name}}
+    {{#account}}
 #SBATCH --account="{{.}}"
-    {{/project_name}}
+    {{/account}}
 
     {{#reservation_id}}
 #SBATCH --reservation="{{.}}"
     {{/reservation_id}}
 {{/job.spec.attributes}}
 
 {{#custom_attributes}}
```

### Comparing `psij-python-0.9.6/src/psij/executors/batch/slurm.py` & `psij-python-0.9.7/src/psij/executors/batch/slurm.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/executors/batch/template_function_library.py` & `psij-python-0.9.7/src/psij/executors/batch/template_function_library.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/executors/flux.py` & `psij-python-0.9.7/src/psij/executors/flux.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/executors/local.py` & `psij-python-0.9.7/src/psij/executors/local.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/executors/rp.py` & `psij-python-0.9.7/src/psij/executors/rp.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/job.py` & `psij-python-0.9.7/src/psij/job.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/job_attributes.py` & `psij-python-0.9.7/src/psij/job_attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,39 @@
+import logging
 import re
 from datetime import timedelta
 from typing import Optional, Dict
 
 from typeguard import check_argument_types
 
 
+logger = logging.getLogger(__name__)
+
+
 _WALLTIME_FMT_ERROR = 'Unknown walltime format: %s. Accepted formats are hh:mm:ss, ' \
                       'hh:mm, mm, or n\\s*[h|m|s].'
 
 
 class JobAttributes(object):
     """A class containing ancillary job information that describes how a job is to be run."""
 
     def __init__(self, duration: timedelta = timedelta(minutes=10),
-                 queue_name: Optional[str] = None, project_name: Optional[str] = None,
+                 queue_name: Optional[str] = None, account: Optional[str] = None,
                  reservation_id: Optional[str] = None,
-                 custom_attributes: Optional[Dict[str, object]] = None) -> None:
+                 custom_attributes: Optional[Dict[str, object]] = None,
+                 project_name: Optional[str] = None) -> None:
         """
         :param duration: Specifies the duration (walltime) of the job. A job whose execution
             exceeds its walltime can be terminated forcefully.
         :param queue_name: If a backend supports multiple queues, this parameter can be used to
             instruct the backend to send this job to a particular queue.
-        :param project_name: If a backend supports multiple projects for billing purposes, setting
-            this attribute instructs the backend to bill the indicated project for the resources
-            consumed by this job.
+        :param account: An account to use for billing purposes. Please note that the executor
+            implementation (or batch scheduler) may use a different term for the option used for
+            accounting/billing purposes, such as `project`. However, scheduler must map this
+            attribute to the accounting/billing option in the underlying execution mechanism.
         :param reservation_id: Allows specifying an advanced reservation ID. Advanced reservations
             enable the pre-allocation of a set of resources/compute nodes for a certain duration
             such that jobs can be run immediately, without waiting in the queue for resources to
             become available.
         :param custom_attributes: Specifies a dictionary of custom attributes. Implementations of
             :class:`~psij.JobExecutor` define and are responsible for interpreting custom
             attributes.
@@ -35,19 +41,21 @@
             or underlying job execution mechanism that cannot otherwise be passed using the classes
             and properties provided by PSI/J. A specific example is that of the subclasses of
             :class:`~psij.executors.batch.batch_scheduler_executor.BatchSchedulerExecutor`, which
             look for custom attributes prefixed with their name and a dot (e.g., `slurm.constraint`,
             `pbs.c`, `lsf.core_isolation`) and translate them into the corresponding batch
             scheduler directives (e.g., `#SLURM --constraint=...`, `#PBS -c ...`,
             `#BSUB -core_isolation ...`).
+        :param project_name: Deprecated. Please use the `account` attribute.
 
         All constructor parameters are accessible as properties.
         """
         assert check_argument_types()
 
+        self.account = account
         self.duration = duration
         self.queue_name = queue_name
         self.project_name = project_name
         self.reservation_id = reservation_id
         self._custom_attributes = custom_attributes
 
     def set_custom_attribute(self, name: str, value: object) -> None:
@@ -82,28 +90,28 @@
         attrs
             A dictionary with the custom attributes to set.
         """
         self._custom_attributes = attrs
 
     def __repr__(self) -> str:
         """Returns a string representation of this object."""
-        return 'JobAttributes(duration={}, queue_name={}, project_name={}, reservation_id={}, ' \
-               'custom_attributes={})'.format(self.duration, self.queue_name, self.project_name,
+        return 'JobAttributes(duration={}, queue_name={}, account={}, reservation_id={}, ' \
+               'custom_attributes={})'.format(self.duration, self.queue_name, self.account,
                                               self.reservation_id, self._custom_attributes)
 
     def __eq__(self, o: object) -> bool:
         """
         Tests if this JobAttributes object is equal to another object.
 
         The objects are equal if all their properties are equal.
         """
         if not isinstance(o, JobAttributes):
             return False
 
-        for prop_name in ['duration', 'queue_name', 'project_name', 'reservation_id',
+        for prop_name in ['duration', 'queue_name', 'account', 'reservation_id',
                           'custom_attributes']:
             if getattr(self, prop_name) != getattr(o, prop_name):
                 return False
 
         return True
 
     @staticmethod
@@ -146,7 +154,18 @@
             if unit == 'h':
                 return timedelta(hours=val)
             elif unit == 'm':
                 return timedelta(minutes=val)
             elif unit == 's':
                 return timedelta(seconds=val)
         raise ValueError(_WALLTIME_FMT_ERROR % walltime)
+
+    @property
+    def project_name(self) -> Optional[str]:
+        """Deprecated. Please use the `account` attribute."""
+        return self.account
+
+    @project_name.setter
+    def project_name(self, project_name: Optional[str]) -> None:
+        logger.warning('The "project_name" attribute is deprecated. Please use the "account" '
+                       'attribute instead.')
+        self.account = project_name
```

### Comparing `psij-python-0.9.6/src/psij/job_executor.py` & `psij-python-0.9.7/src/psij/job_executor.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/job_executor_config.py` & `psij-python-0.9.7/src/psij/job_executor_config.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/job_launcher.py` & `psij-python-0.9.7/src/psij/job_launcher.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/job_spec.py` & `psij-python-0.9.7/src/psij/job_spec.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/job_state.py` & `psij-python-0.9.7/src/psij/job_state.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/job_status.py` & `psij-python-0.9.7/src/psij/job_status.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/launcher.py` & `psij-python-0.9.7/src/psij/launcher.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/launchers/__init__.py` & `psij-python-0.9.7/src/psij/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/launchers/aprun.py` & `psij-python-0.9.7/src/psij/launchers/aprun.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/launchers/jsrun.py` & `psij-python-0.9.7/src/psij/launchers/jsrun.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/launchers/mpirun.py` & `psij-python-0.9.7/src/psij/launchers/mpirun.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/launchers/multiple.py` & `psij-python-0.9.7/src/psij/launchers/multiple.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/launchers/script_based_launcher.py` & `psij-python-0.9.7/src/psij/launchers/script_based_launcher.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/launchers/scripts/launcher_lib.sh` & `psij-python-0.9.7/src/psij/launchers/scripts/launcher_lib.sh`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/launchers/scripts/mpi_launch.sh` & `psij-python-0.9.7/src/psij/launchers/scripts/mpi_launch.sh`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/launchers/scripts/multi_launch.sh` & `psij-python-0.9.7/src/psij/launchers/scripts/multi_launch.sh`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/launchers/single.py` & `psij-python-0.9.7/src/psij/launchers/single.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/launchers/srun.py` & `psij-python-0.9.7/src/psij/launchers/srun.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/resource_spec.py` & `psij-python-0.9.7/src/psij/resource_spec.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/serialize.py` & `psij-python-0.9.7/src/psij/serialize.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij/utils.py` & `psij-python-0.9.7/src/psij/utils.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij-descriptors/core_descriptors.py` & `psij-python-0.9.7/src/psij-descriptors/core_descriptors.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij-descriptors/pbs_descriptor.py` & `psij-python-0.9.7/src/psij-descriptors/pbs_descriptor.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/src/psij_python.egg-info/SOURCES.txt` & `psij-python-0.9.7/src/psij_python.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 src/psij/__init__.py
 src/psij/__main__.py
 src/psij/_plugins.py
 src/psij/descriptor.py
 src/psij/exceptions.py
 src/psij/job.py
```

### Comparing `psij-python-0.9.6/tests/test_callbacks.py` & `psij-python-0.9.7/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/tests/test_doc_examples.py` & `psij-python-0.9.7/tests/test_doc_examples.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/tests/test_executor.py` & `psij-python-0.9.7/tests/test_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,11 +216,11 @@
     spec = JobSpec(resources=res, attributes=attrs)
     spec.launcher = 'single'
     job = Job(spec=spec)
 
     prefix = _get_attr_prefix(exec_name)
     _check_str_attrs(ex, job, ['executable', 'directory'],
                      lambda k, v: setattr(spec, k, v))
-    _check_str_attrs(ex, job, ['queue_name', 'project_name', 'reservation_id'],
+    _check_str_attrs(ex, job, ['queue_name', 'account', 'reservation_id'],
                      lambda k, v: setattr(attrs, k, v))
     _check_str_attrs(ex, job, [prefix + '.cust_attr1', prefix + '.cust_attr2'],
                      lambda k, v: c_attrs.__setitem__(k, v))
```

### Comparing `psij-python-0.9.6/tests/test_executor_loading.py` & `psij-python-0.9.7/tests/test_executor_loading.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/tests/test_infrastructure.py` & `psij-python-0.9.7/tests/test_infrastructure.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/tests/test_issue_435.py` & `psij-python-0.9.7/tests/test_issue_435.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/tests/test_job_spec.py` & `psij-python-0.9.7/tests/test_job_spec.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/tests/test_mpi.py` & `psij-python-0.9.7/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/tests/test_nodefile.py` & `psij-python-0.9.7/tests/test_nodefile.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/tests/test_resources.py` & `psij-python-0.9.7/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/tests/test_serialization.py` & `psij-python-0.9.7/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `psij-python-0.9.6/tests/test_wait.py` & `psij-python-0.9.7/tests/test_wait.py`

 * *Files identical despite different names*

