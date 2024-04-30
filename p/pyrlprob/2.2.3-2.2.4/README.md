# Comparing `tmp/pyrlprob-2.2.3.tar.gz` & `tmp/pyrlprob-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrlprob-2.2.3.tar", last modified: Mon Apr 29 21:01:59 2024, max compression
+gzip compressed data, was "pyrlprob-2.2.4.tar", last modified: Tue Apr 30 22:29:31 2024, max compression
```

## Comparing `pyrlprob-2.2.3.tar` & `pyrlprob-2.2.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1073 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/LICENSE.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)      301 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/MANIFEST.in
--rw-r--r--   0 lorenzof (332258323) domainusers (245600513)     2800 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/PKG-INFO
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1787 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/README.md
--rw-------   0 lorenzof (332258323) domainusers (245600513)      103 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyproject.toml
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.084192 pyrlprob-2.2.3/pyrlprob/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      250 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1157 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/__main__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)    16762 2024-04-29 20:54:47.000000 pyrlprob-2.2.3/pyrlprob/base_funs.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)      661 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/commands.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.084192 pyrlprob-2.2.3/pyrlprob/include/
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.084192 pyrlprob-2.2.3/pyrlprob/include/pyrlprob/
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2938 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/include/pyrlprob/binding.cpp
--rw-------   0 lorenzof (332258323) domainusers (245600513)     5140 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/include/pyrlprob/mdp.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     3818 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/include/pyrlprob/mdp_vec.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     4114 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/include/pyrlprob/py_mdp.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     7733 2024-02-16 19:04:09.000000 pyrlprob-2.2.3/pyrlprob/mdp.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.084192 pyrlprob-2.2.3/pyrlprob/models/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      151 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/pyrlprob/models/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)    29760 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/pyrlprob/models/models.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)    14323 2024-04-29 20:57:36.000000 pyrlprob-2.2.3/pyrlprob/problem.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.084192 pyrlprob-2.2.3/pyrlprob/tests/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      477 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/__init__.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      210 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)      390 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/binding.cpp
--rw-------   0 lorenzof (332258323) domainusers (245600513)     6849 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d.cpp
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2063 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1830 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d.py
--rwx------   0 lorenzof (332258323) domainusers (245600513)   463776 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
--rw-------   0 lorenzof (332258323) domainusers (245600513)      696 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d_dyn.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1405 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/rk4.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1358 2024-02-16 18:24:51.000000 pyrlprob-2.2.3/pyrlprob/tests/landing1d_cpp.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1961 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/pyrlprob/tests/landing1d_gtrxl_py.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1637 2024-02-16 19:31:26.000000 pyrlprob-2.2.3/pyrlprob/tests/landing1d_load.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1811 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/pyrlprob/tests/landing1d_lstm_py.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1341 2024-02-16 19:10:05.000000 pyrlprob-2.2.3/pyrlprob/tests/landing1d_py.yaml
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/pyrlprob/tests/py_tests/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      190 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     4931 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/landing1d.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)      974 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/landing1d_dyn.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     6379 2024-02-16 18:26:17.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/landing1d_gym.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      428 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      691 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      331 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      560 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1064 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      496 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      433 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      713 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      520 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      456 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      582 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      732 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      639 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      497 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      714 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      615 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     5902 2024-04-29 20:57:24.000000 pyrlprob-2.2.3/pyrlprob/tests/test_landing1d.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2813 2024-02-16 17:36:47.000000 pyrlprob-2.2.3/pyrlprob/tests/test_multiple_gym.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/pyrlprob/tune/
--rw-------   0 lorenzof (332258323) domainusers (245600513)       87 2024-02-16 18:28:30.000000 pyrlprob-2.2.3/pyrlprob/tune/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     3393 2024-02-16 18:35:28.000000 pyrlprob-2.2.3/pyrlprob/tune/tune.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/pyrlprob/utils/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      546 2022-11-23 23:28:53.000000 pyrlprob-2.2.3/pyrlprob/utils/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     3446 2024-04-29 19:06:24.000000 pyrlprob-2.2.3/pyrlprob/utils/auxiliary.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     4722 2024-02-16 19:07:37.000000 pyrlprob-2.2.3/pyrlprob/utils/callbacks.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2835 2024-02-16 19:07:46.000000 pyrlprob-2.2.3/pyrlprob/utils/plots.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-29 21:01:59.084192 pyrlprob-2.2.3/pyrlprob.egg-info/
--rw-r--r--   0 lorenzof (332258323) domainusers (245600513)     2800 2024-04-29 21:01:58.000000 pyrlprob-2.2.3/pyrlprob.egg-info/PKG-INFO
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2633 2024-04-29 21:01:58.000000 pyrlprob-2.2.3/pyrlprob.egg-info/SOURCES.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)        1 2024-04-29 21:01:58.000000 pyrlprob-2.2.3/pyrlprob.egg-info/dependency_links.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)      219 2024-04-29 21:01:58.000000 pyrlprob-2.2.3/pyrlprob.egg-info/requires.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)        9 2024-04-29 21:01:58.000000 pyrlprob-2.2.3/pyrlprob.egg-info/top_level.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)       38 2024-04-29 21:01:59.088192 pyrlprob-2.2.3/setup.cfg
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1278 2024-04-29 20:58:42.000000 pyrlprob-2.2.3/setup.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.098610 pyrlprob-2.2.4/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1073 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/LICENSE.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      301 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/MANIFEST.in
+-rw-r--r--   0 lorenzof (332258323) domainusers (245600513)     2808 2024-04-30 22:29:31.098610 pyrlprob-2.2.4/PKG-INFO
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1787 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/README.md
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      103 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyproject.toml
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.082611 pyrlprob-2.2.4/pyrlprob/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      250 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1157 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/__main__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)    16762 2024-04-29 20:54:47.000000 pyrlprob-2.2.4/pyrlprob/base_funs.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      661 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/commands.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.082611 pyrlprob-2.2.4/pyrlprob/include/
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.086611 pyrlprob-2.2.4/pyrlprob/include/pyrlprob/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2938 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/include/pyrlprob/binding.cpp
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     5140 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/include/pyrlprob/mdp.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     3818 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/include/pyrlprob/mdp_vec.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     4114 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/include/pyrlprob/py_mdp.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     7733 2024-02-16 19:04:09.000000 pyrlprob-2.2.4/pyrlprob/mdp.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.086611 pyrlprob-2.2.4/pyrlprob/models/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      151 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/pyrlprob/models/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)    29760 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/pyrlprob/models/models.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)    14323 2024-04-29 20:57:36.000000 pyrlprob-2.2.4/pyrlprob/problem.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.086611 pyrlprob-2.2.4/pyrlprob/tests/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      477 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/__init__.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.086611 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      210 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      390 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/binding.cpp
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     6849 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d.cpp
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2063 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1830 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d.py
+-rwx------   0 lorenzof (332258323) domainusers (245600513)   463776 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      696 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d_dyn.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1405 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/rk4.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1358 2024-02-16 18:24:51.000000 pyrlprob-2.2.4/pyrlprob/tests/landing1d_cpp.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1961 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/pyrlprob/tests/landing1d_gtrxl_py.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1637 2024-02-16 19:31:26.000000 pyrlprob-2.2.4/pyrlprob/tests/landing1d_load.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1811 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/pyrlprob/tests/landing1d_lstm_py.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1341 2024-02-16 19:10:05.000000 pyrlprob-2.2.4/pyrlprob/tests/landing1d_py.yaml
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.094611 pyrlprob-2.2.4/pyrlprob/tests/py_tests/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      190 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     4931 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/landing1d.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      974 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/landing1d_dyn.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     6379 2024-02-16 18:26:17.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/landing1d_gym.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.098610 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      428 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      691 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      331 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      560 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1064 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      496 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      433 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      713 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      520 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      456 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      582 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      732 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      639 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      497 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      714 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      615 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     5902 2024-04-29 20:57:24.000000 pyrlprob-2.2.4/pyrlprob/tests/test_landing1d.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2813 2024-02-16 17:36:47.000000 pyrlprob-2.2.4/pyrlprob/tests/test_multiple_gym.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.098610 pyrlprob-2.2.4/pyrlprob/tune/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)       87 2024-02-16 18:28:30.000000 pyrlprob-2.2.4/pyrlprob/tune/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     3393 2024-02-16 18:35:28.000000 pyrlprob-2.2.4/pyrlprob/tune/tune.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.098610 pyrlprob-2.2.4/pyrlprob/utils/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      546 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/utils/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     3446 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/pyrlprob/utils/auxiliary.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     4722 2024-02-16 19:07:37.000000 pyrlprob-2.2.4/pyrlprob/utils/callbacks.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2835 2024-02-16 19:07:46.000000 pyrlprob-2.2.4/pyrlprob/utils/plots.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.086611 pyrlprob-2.2.4/pyrlprob.egg-info/
+-rw-r--r--   0 lorenzof (332258323) domainusers (245600513)     2808 2024-04-30 22:29:30.000000 pyrlprob-2.2.4/pyrlprob.egg-info/PKG-INFO
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2633 2024-04-30 22:29:30.000000 pyrlprob-2.2.4/pyrlprob.egg-info/SOURCES.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)        1 2024-04-30 22:29:30.000000 pyrlprob-2.2.4/pyrlprob.egg-info/dependency_links.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      227 2024-04-30 22:29:30.000000 pyrlprob-2.2.4/pyrlprob.egg-info/requires.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)        9 2024-04-30 22:29:30.000000 pyrlprob-2.2.4/pyrlprob.egg-info/top_level.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)       38 2024-04-30 22:29:31.098610 pyrlprob-2.2.4/setup.cfg
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1286 2024-04-30 22:29:06.000000 pyrlprob-2.2.4/setup.py
```

### Comparing `pyrlprob-2.2.3/LICENSE.txt` & `pyrlprob-2.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/PKG-INFO` & `pyrlprob-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.2.3
+Version: 2.2.4
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 Requires-Dist: pybind11
 Requires-Dist: pytest
 Requires-Dist: ray==1.6.0
 Requires-Dist: scipy
 Requires-Dist: scikit-image
 Requires-Dist: opencv-python; platform_machine == "x86_64"
 Requires-Dist: tabulate
-Requires-Dist: tensorflow
+Requires-Dist: tensorflow==2.15.0
 Requires-Dist: tensorboardx; platform_machine == "x86_64"
 Requires-Dist: torch
 Requires-Dist: typing
 Requires-Dist: PyYAML
 Requires-Dist: protobuf==3.20.3
 
 <p align="center">
```

### Comparing `pyrlprob-2.2.3/README.md` & `pyrlprob-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/__main__.py` & `pyrlprob-2.2.4/pyrlprob/__main__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/base_funs.py` & `pyrlprob-2.2.4/pyrlprob/base_funs.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/commands.py` & `pyrlprob-2.2.4/pyrlprob/commands.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/include/pyrlprob/binding.cpp` & `pyrlprob-2.2.4/pyrlprob/include/pyrlprob/binding.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/include/pyrlprob/mdp.h` & `pyrlprob-2.2.4/pyrlprob/include/pyrlprob/mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/include/pyrlprob/mdp_vec.h` & `pyrlprob-2.2.4/pyrlprob/include/pyrlprob/mdp_vec.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/include/pyrlprob/py_mdp.h` & `pyrlprob-2.2.4/pyrlprob/include/pyrlprob/py_mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/mdp.py` & `pyrlprob-2.2.4/pyrlprob/mdp.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/models/models.py` & `pyrlprob-2.2.4/pyrlprob/models/models.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/problem.py` & `pyrlprob-2.2.4/pyrlprob/problem.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d.cpp` & `pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d.h` & `pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d.py` & `pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so` & `pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/landing1d_dyn.h` & `pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d_dyn.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/cpp_tests/rk4.h` & `pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/rk4.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/landing1d_cpp.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/landing1d_cpp.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/landing1d_gtrxl_py.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/landing1d_gtrxl_py.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/landing1d_load.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/landing1d_load.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/landing1d_lstm_py.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/landing1d_lstm_py.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/landing1d_py.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/landing1d_py.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/landing1d.py` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/landing1d_dyn.py` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/landing1d_dyn.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/landing1d_gym.py` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/landing1d_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml` & `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/test_landing1d.py` & `pyrlprob-2.2.4/pyrlprob/tests/test_landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tests/test_multiple_gym.py` & `pyrlprob-2.2.4/pyrlprob/tests/test_multiple_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/tune/tune.py` & `pyrlprob-2.2.4/pyrlprob/tune/tune.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/utils/__init__.py` & `pyrlprob-2.2.4/pyrlprob/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/utils/auxiliary.py` & `pyrlprob-2.2.4/pyrlprob/utils/auxiliary.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/utils/callbacks.py` & `pyrlprob-2.2.4/pyrlprob/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob/utils/plots.py` & `pyrlprob-2.2.4/pyrlprob/utils/plots.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/pyrlprob.egg-info/PKG-INFO` & `pyrlprob-2.2.4/pyrlprob.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.2.3
+Version: 2.2.4
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 Requires-Dist: pybind11
 Requires-Dist: pytest
 Requires-Dist: ray==1.6.0
 Requires-Dist: scipy
 Requires-Dist: scikit-image
 Requires-Dist: opencv-python; platform_machine == "x86_64"
 Requires-Dist: tabulate
-Requires-Dist: tensorflow
+Requires-Dist: tensorflow==2.15.0
 Requires-Dist: tensorboardx; platform_machine == "x86_64"
 Requires-Dist: torch
 Requires-Dist: typing
 Requires-Dist: PyYAML
 Requires-Dist: protobuf==3.20.3
 
 <p align="center">
```

### Comparing `pyrlprob-2.2.3/pyrlprob.egg-info/SOURCES.txt` & `pyrlprob-2.2.4/pyrlprob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.3/setup.py` & `pyrlprob-2.2.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='pyrlprob',
-    version='2.2.3',
+    version='2.2.4',
     author='Lorenzo Federici',
     author_email = 'federicilorenzo94@gmail.com',
     description = 'Train Gym-derived environments in Python/C++ through Ray RLlib',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/LorenzoFederici/pyrlprob',
     classifiers = [
@@ -27,15 +27,15 @@
         'pybind11',
         'pytest',
         'ray==1.6.0',
         'scipy',
         'scikit-image',
         'opencv-python; platform_machine=="x86_64"',
         'tabulate',
-        'tensorflow',
+        'tensorflow==2.15.0',
         'tensorboardx; platform_machine=="x86_64"',
         'torch',
         'typing',
         'PyYAML',
         'protobuf==3.20.3'
     ],
     packages = find_packages(),
```

