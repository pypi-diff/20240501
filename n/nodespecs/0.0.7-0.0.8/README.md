# Comparing `tmp/nodespecs-0.0.7.tar.gz` & `tmp/nodespecs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodespecs-0.0.7.tar", last modified: Mon Apr 29 18:55:28 2024, max compression
+gzip compressed data, was "nodespecs-0.0.8.tar", last modified: Wed May  1 16:27:48 2024, max compression
```

## Comparing `nodespecs-0.0.7.tar` & `nodespecs-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 18:55:28.903619 nodespecs-0.0.7/
--rw-rw-rw-   0        0        0     1098 2024-04-13 00:06:04.000000 nodespecs-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     7013 2024-04-29 18:55:28.901621 nodespecs-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5132 2024-04-29 18:54:55.000000 nodespecs-0.0.7/README.md
--rw-rw-rw-   0        0        0      899 2024-04-29 18:18:43.000000 nodespecs-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 18:55:28.903619 nodespecs-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 18:55:28.860757 nodespecs-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 18:55:28.899628 nodespecs-0.0.7/src/nodespecs.egg-info/
--rw-rw-rw-   0        0        0     7013 2024-04-29 18:55:28.000000 nodespecs-0.0.7/src/nodespecs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2024-04-29 18:55:28.000000 nodespecs-0.0.7/src/nodespecs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 18:55:28.000000 nodespecs-0.0.7/src/nodespecs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-29 18:55:28.000000 nodespecs-0.0.7/src/nodespecs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-04-29 18:55:28.000000 nodespecs-0.0.7/src/nodespecs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-29 18:55:28.000000 nodespecs-0.0.7/src/nodespecs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 18:55:28.896638 nodespecs-0.0.7/src/specs/
--rw-rw-rw-   0        0        0      158 2024-04-29 18:13:46.000000 nodespecs-0.0.7/src/specs/__init__.py
--rw-rw-rw-   0        0        0      271 2024-04-18 19:09:52.000000 nodespecs-0.0.7/src/specs/__main__.py
--rw-rw-rw-   0        0        0     1479 2024-04-23 13:35:21.000000 nodespecs-0.0.7/src/specs/benchmark.py
--rw-rw-rw-   0        0        0      488 2024-04-23 20:58:02.000000 nodespecs-0.0.7/src/specs/cmd.py
--rw-rw-rw-   0        0        0     2783 2024-04-29 18:53:57.000000 nodespecs-0.0.7/src/specs/comm.py
--rw-rw-rw-   0        0        0    86524 2024-04-12 15:14:05.000000 nodespecs-0.0.7/src/specs/cpuinfo.py
--rw-rw-rw-   0        0        0     7189 2024-04-25 04:50:36.000000 nodespecs-0.0.7/src/specs/hardware.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:27:48.848773 nodespecs-0.0.8/
+-rw-rw-rw-   0        0        0     1098 2024-04-13 00:06:04.000000 nodespecs-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     7653 2024-05-01 16:27:48.845782 nodespecs-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5756 2024-05-01 15:19:14.000000 nodespecs-0.0.8/README.md
+-rw-rw-rw-   0        0        0      902 2024-05-01 15:31:23.000000 nodespecs-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 16:27:48.848773 nodespecs-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 16:27:48.802201 nodespecs-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 16:27:48.843785 nodespecs-0.0.8/src/nodespecs.egg-info/
+-rw-rw-rw-   0        0        0     7653 2024-05-01 16:27:48.000000 nodespecs-0.0.8/src/nodespecs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2024-05-01 16:27:48.000000 nodespecs-0.0.8/src/nodespecs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 16:27:48.000000 nodespecs-0.0.8/src/nodespecs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-01 16:27:48.000000 nodespecs-0.0.8/src/nodespecs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-05-01 16:27:48.000000 nodespecs-0.0.8/src/nodespecs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-01 16:27:48.000000 nodespecs-0.0.8/src/nodespecs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 16:27:48.835817 nodespecs-0.0.8/src/specs/
+-rw-rw-rw-   0        0        0      210 2024-05-01 15:49:09.000000 nodespecs-0.0.8/src/specs/__init__.py
+-rw-rw-rw-   0        0        0      777 2024-05-01 16:26:19.000000 nodespecs-0.0.8/src/specs/__main__.py
+-rw-rw-rw-   0        0        0     1545 2024-05-01 16:16:52.000000 nodespecs-0.0.8/src/specs/benchmark.py
+-rw-rw-rw-   0        0        0      488 2024-04-23 20:58:02.000000 nodespecs-0.0.8/src/specs/cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-01 16:27:48.840799 nodespecs-0.0.8/src/specs/communicate/
+-rw-rw-rw-   0        0        0    17137 2024-05-01 15:19:14.000000 nodespecs-0.0.8/src/specs/communicate/pp.py
+-rw-rw-rw-   0        0        0     2783 2024-05-01 15:44:00.000000 nodespecs-0.0.8/src/specs/communicate/tcpsocket.py
+-rw-rw-rw-   0        0        0    86524 2024-04-12 15:14:05.000000 nodespecs-0.0.8/src/specs/cpuinfo.py
+-rw-rw-rw-   0        0        0     7675 2024-05-01 16:16:25.000000 nodespecs-0.0.8/src/specs/hardware.py
```

### Comparing `nodespecs-0.0.7/LICENSE` & `nodespecs-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.7/PKG-INFO` & `nodespecs-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodespecs
-Version: 0.0.7
+Version: 0.0.8
 Summary: The specs summarize utilities for computer instance
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2024 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -15,20 +15,20 @@
 Keywords: cpu,gpu,benchmark
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: psutil>=5.9.5
 Requires-Dist: tabulate>=0.8.0
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: GPUtil; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: psutil>=5.9.5; extra == "dev"
 
 # hardwareSummary
 Extracting and Fetching all system and hardware information such as os details, CPU and GPU information, disk and network usage in Python using platform, psutil and gputil libraries.
 
 
 
 ### install and use with pip
@@ -87,32 +87,32 @@
 sudo apt install python3-pip
 git clone https://github.com/jinsanity07git/hardwareSummary && python3 hardwareSummary/hardware.py && python3 hardwareSummary/cpu-benchmark.py
 ```
 
 
 
 ### CPU collection
-
-| Nickname                      | CPU                                            | Arch   | OS         | Benchmarking | Comb                                                         | Score |
-| ----------------------------- | ---------------------------------------------- | ------ | ---------- | ------------ | ------------------------------------------------------------ | ----- |
-| TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows    | 15.654       | Core-i9-14900KF                                              | 39.25 |
-| TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10 | 12.991       | Core-i9-13900K                                               | 38.76 |
-| Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows    | 23.852       | Core-i7-11800H                                               | 13.47 |
-| TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows    | 26.723       | Core-i7-9700K                                                | 9.45  |
-| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64 | Linux      | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
-| WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux      | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
-| TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window     | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
-| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64 | Linux      | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
-| TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64  | Windows    | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
-| google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64 | Linux      | 43.078       |                                                              |       |
-| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64 | Linux      | 49.396       |                                                              |       |
-| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64  | Windows    | 62.969       |                                                              |       |
-| Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64 | Linux      | 98.732       | EPYC-7551                                                    | 14.67 |
-
-
+| Nickname                      | CPU                                            | Arch   | OS            | Benchmarking | Comb                                                         | Score |
+| ----------------------------- | ---------------------------------------------- | ------ | ------------- | ------------ | ------------------------------------------------------------ | ----- |
+| TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows       | 15.654       | Core-i9-14900KF                                              | 39.25 |
+| TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10    | 12.991       | Core-i9-13900K                                               | 38.76 |
+| Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows       | 23.852       | Core-i7-11800H                                               | 13.47 |
+| TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows       | 26.723       | Core-i7-9700K                                                | 9.45  |
+| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64 | Linux         | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
+| WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux         | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
+| TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window        | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
+| 2018 Macbook pro              | Intel(R) Core(TM) i7-8559U CPU @ 2.70GHz       | x86_64 | Darwin 22.1.0 | 37.105       | [Core-i7-8559U](https://technical.city/en/cpu/Core-i7-8559U) | 5.38  |
+| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64 | Linux         | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
+| TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64  | Windows       | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
+| Jquant                        | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux         | 40.128       | Xeon-Platinum-8163                                           |       |
+| google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64 | Linux         | 43.078       |                                                              |       |
+| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64 | Linux         | 49.396       |                                                              |       |
+| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64  | Windows       | 62.969       |                                                              |       |
+| Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64 | Linux         | 98.732       | EPYC-7551                                                    | 14.67 |
+| mini PC                       | Intel(R) Atom(TM) x5-Z8350 CPU @ 1.44GHz       | x86_64 | Linux         | 135.107      | Atom-x5-Z8350                                                | 0.57  |
 
 ### GPU collection
 
 
 
 | id    | name                    | total memory | Synthetic benchmark | CUDA API |
 | ----- | ----------------------- | ------------ | ------------------- | -------- |
```

### Comparing `nodespecs-0.0.7/README.md` & `nodespecs-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -59,32 +59,32 @@
 sudo apt install python3-pip
 git clone https://github.com/jinsanity07git/hardwareSummary && python3 hardwareSummary/hardware.py && python3 hardwareSummary/cpu-benchmark.py
 ```
 
 
 
 ### CPU collection
-
-| Nickname                      | CPU                                            | Arch   | OS         | Benchmarking | Comb                                                         | Score |
-| ----------------------------- | ---------------------------------------------- | ------ | ---------- | ------------ | ------------------------------------------------------------ | ----- |
-| TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows    | 15.654       | Core-i9-14900KF                                              | 39.25 |
-| TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10 | 12.991       | Core-i9-13900K                                               | 38.76 |
-| Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows    | 23.852       | Core-i7-11800H                                               | 13.47 |
-| TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows    | 26.723       | Core-i7-9700K                                                | 9.45  |
-| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64 | Linux      | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
-| WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux      | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
-| TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window     | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
-| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64 | Linux      | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
-| TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64  | Windows    | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
-| google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64 | Linux      | 43.078       |                                                              |       |
-| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64 | Linux      | 49.396       |                                                              |       |
-| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64  | Windows    | 62.969       |                                                              |       |
-| Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64 | Linux      | 98.732       | EPYC-7551                                                    | 14.67 |
-
-
+| Nickname                      | CPU                                            | Arch   | OS            | Benchmarking | Comb                                                         | Score |
+| ----------------------------- | ---------------------------------------------- | ------ | ------------- | ------------ | ------------------------------------------------------------ | ----- |
+| TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows       | 15.654       | Core-i9-14900KF                                              | 39.25 |
+| TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10    | 12.991       | Core-i9-13900K                                               | 38.76 |
+| Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows       | 23.852       | Core-i7-11800H                                               | 13.47 |
+| TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows       | 26.723       | Core-i7-9700K                                                | 9.45  |
+| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64 | Linux         | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
+| WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux         | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
+| TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window        | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
+| 2018 Macbook pro              | Intel(R) Core(TM) i7-8559U CPU @ 2.70GHz       | x86_64 | Darwin 22.1.0 | 37.105       | [Core-i7-8559U](https://technical.city/en/cpu/Core-i7-8559U) | 5.38  |
+| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64 | Linux         | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
+| TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64  | Windows       | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
+| Jquant                        | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux         | 40.128       | Xeon-Platinum-8163                                           |       |
+| google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64 | Linux         | 43.078       |                                                              |       |
+| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64 | Linux         | 49.396       |                                                              |       |
+| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64  | Windows       | 62.969       |                                                              |       |
+| Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64 | Linux         | 98.732       | EPYC-7551                                                    | 14.67 |
+| mini PC                       | Intel(R) Atom(TM) x5-Z8350 CPU @ 1.44GHz       | x86_64 | Linux         | 135.107      | Atom-x5-Z8350                                                | 0.57  |
 
 ### GPU collection
 
 
 
 | id    | name                    | total memory | Synthetic benchmark | CUDA API |
 | ----- | ----------------------- | ------------ | ------------------- | -------- |
```

### Comparing `nodespecs-0.0.7/pyproject.toml` & `nodespecs-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nodespecs"
-version = "0.0.7"
+version = "0.0.8"
 description = "The specs summarize utilities for computer instance"
 readme = "README.md"
 authors = [{ name = "jinsanity", email = "jinsanityff@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["cpu", "gpu", "benchmark"]
 dependencies = [
-    "psutil >= 5.9.5",
     "tabulate >= 0.8.0",
     'tomli; python_version < "3.11"',
 ]
 requires-python = ">=3.6"
 
 [project.optional-dependencies]
-dev = ["GPUtil","pip-tools"]
+dev = ["GPUtil","pip-tools",
+       "psutil >= 5.9.5"]
 
 [project.urls]
 Homepage = "https://github.com/jinsanity07git/hardwareSummary"
 
 [project.scripts]
 realpython = "specs.__main__:main"
```

### Comparing `nodespecs-0.0.7/src/nodespecs.egg-info/PKG-INFO` & `nodespecs-0.0.8/src/nodespecs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodespecs
-Version: 0.0.7
+Version: 0.0.8
 Summary: The specs summarize utilities for computer instance
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2024 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -15,20 +15,20 @@
 Keywords: cpu,gpu,benchmark
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: psutil>=5.9.5
 Requires-Dist: tabulate>=0.8.0
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: GPUtil; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: psutil>=5.9.5; extra == "dev"
 
 # hardwareSummary
 Extracting and Fetching all system and hardware information such as os details, CPU and GPU information, disk and network usage in Python using platform, psutil and gputil libraries.
 
 
 
 ### install and use with pip
@@ -87,32 +87,32 @@
 sudo apt install python3-pip
 git clone https://github.com/jinsanity07git/hardwareSummary && python3 hardwareSummary/hardware.py && python3 hardwareSummary/cpu-benchmark.py
 ```
 
 
 
 ### CPU collection
-
-| Nickname                      | CPU                                            | Arch   | OS         | Benchmarking | Comb                                                         | Score |
-| ----------------------------- | ---------------------------------------------- | ------ | ---------- | ------------ | ------------------------------------------------------------ | ----- |
-| TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows    | 15.654       | Core-i9-14900KF                                              | 39.25 |
-| TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10 | 12.991       | Core-i9-13900K                                               | 38.76 |
-| Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows    | 23.852       | Core-i7-11800H                                               | 13.47 |
-| TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows    | 26.723       | Core-i7-9700K                                                | 9.45  |
-| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64 | Linux      | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
-| WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux      | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
-| TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window     | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
-| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64 | Linux      | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
-| TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64  | Windows    | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
-| google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64 | Linux      | 43.078       |                                                              |       |
-| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64 | Linux      | 49.396       |                                                              |       |
-| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64  | Windows    | 62.969       |                                                              |       |
-| Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64 | Linux      | 98.732       | EPYC-7551                                                    | 14.67 |
-
-
+| Nickname                      | CPU                                            | Arch   | OS            | Benchmarking | Comb                                                         | Score |
+| ----------------------------- | ---------------------------------------------- | ------ | ------------- | ------------ | ------------------------------------------------------------ | ----- |
+| TC17<br />TC16                | Intel(R) Core(TM) i9-14900KF                   | AMD64  | Windows       | 15.654       | Core-i9-14900KF                                              | 39.25 |
+| TC14                          | 13th Gen Intel(R) Core(TM) i9-13900K           | AMD64  | Windows 10    | 12.991       | Core-i9-13900K                                               | 38.76 |
+| Dell Precision 3561           | 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz | AMD64  | Windows       | 23.852       | Core-i7-11800H                                               | 13.47 |
+| TC07                          | Intel(R) Core(TM) i7-9700K CPU @ 3.60GHz       | AMD64  | Windows       | 26.723       | Core-i7-9700K                                                | 9.45  |
+| AWS `t2.micro`                | Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz      | x86_64 | Linux         | 27.785       | [Core-i7-9700K](https://technical.city/en/cpu/Core-i7-9700K) | 8.81  |
+| WUYING: 8 vCPU / 16 GiB Linux | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux         | 33.572       | [Xeon-Platinum-8163](https://versus.com/en/intel-xeon-gold-6126-vs-intel-xeon-platinum-8168) |       |
+| TC03<br />TC11                | Intel(R) Xeon(R) Gold 6248R CPU @ 3.00GHz      | AMD64  | Window        | 34.612       | Xeon-Gold-6248R                                              | 23.26 |
+| 2018 Macbook pro              | Intel(R) Core(TM) i7-8559U CPU @ 2.70GHz       | x86_64 | Darwin 22.1.0 | 37.105       | [Core-i7-8559U](https://technical.city/en/cpu/Core-i7-8559U) | 5.38  |
+| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | x86_64 | Linux         | 38.685       | [Xeon-Gold-6126](https://technical.city/en/cpu/Xeon-Gold-6126) | 12.21 |
+| TC01                          | Intel(R) Xeon(R) CPU E5-2643 v4 @ 3.40GHz      | AMD64  | Windows       | 39.258       | Xeon-E5-2643-v4                                              | 7.62  |
+| Jquant                        | Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz   | x86_64 | Linux         | 40.128       | Xeon-Platinum-8163                                           |       |
+| google colab free tier        | Intel(R) Xeon(R) CPU @ 2.20GHz                 | x86_64 | Linux         | 43.078       |                                                              |       |
+| aws cloudshell                | Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz | x86_64 | Linux         | 49.396       |                                                              |       |
+| JVM                           | Intel(R) Xeon(R) Gold 6126 CPU @ 2.60GHz       | AMD64  | Windows       | 62.969       |                                                              |       |
+| Oracle 1G-1G-0.5Gbps          | AMD EPYC 7551 32-Core Processor                | x86_64 | Linux         | 98.732       | EPYC-7551                                                    | 14.67 |
+| mini PC                       | Intel(R) Atom(TM) x5-Z8350 CPU @ 1.44GHz       | x86_64 | Linux         | 135.107      | Atom-x5-Z8350                                                | 0.57  |
 
 ### GPU collection
 
 
 
 | id    | name                    | total memory | Synthetic benchmark | CUDA API |
 | ----- | ----------------------- | ------------ | ------------------- | -------- |
```

### Comparing `nodespecs-0.0.7/src/specs/benchmark.py` & `nodespecs-0.0.8/src/specs/benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 #Python CPU Benchmark by Alex Dedyura (Windows, macOS, Linux)
 #https://github.com/alexdedyura/cpu-benchmark
 
 import time
 import platform
 from . import cpuinfo
 
-def bench_cpu():
-  print('Python CPU Benchmark by Alex Dedyura (Windows, macOS(Darwin), Linux)')
+def info_plat():
   print('CPU: ' + cpuinfo.get_cpu_info().get('brand_raw', "Unknown"))
   print('Arch: ' + cpuinfo.get_cpu_info().get('arch_string_raw', "Unknown"))
   print('OS: ' + platform.system(), platform.release())
   print('Python: ' + platform.python_version())
 
+
+def bench_cpu():
+  print('Python CPU Benchmark (Windows, macOS(Darwin), Linux)')
+  info_plat()
   print('\nBenchmarking: \n')
 
   start_benchmark = 10000 # change this if you like (sample: 1000, 5000, etc)
   start_benchmark = int(start_benchmark)
 
   repeat_benchmark = 10 # attemps, change this if you like (sample: 3, 5, etc)
   repeat_benchmark = int(repeat_benchmark)
@@ -38,8 +41,12 @@
     end = time.perf_counter()
     duration = (end - start)
     duration = round(duration, 3)
     average_benchmark += duration
     print('Time: ' + str(duration) + 's')
 
   average_benchmark = round(average_benchmark / repeat_benchmark, 3)
-  print('Average (from {} repeats): {}s'.format(repeat_benchmark, average_benchmark))
+  print('Average (from {} repeats): {}s'.format(repeat_benchmark, average_benchmark))
+
+
+if __name__ == "__main__":
+  info_plat()
```

### Comparing `nodespecs-0.0.7/src/specs/comm.py` & `nodespecs-0.0.8/src/specs/communicate/tcpsocket.py`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.7/src/specs/cpuinfo.py` & `nodespecs-0.0.8/src/specs/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.7/src/specs/hardware.py` & `nodespecs-0.0.8/src/specs/hardware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 #Be ready to enjoy your python code--UTB
 # https://www.thepythoncode.com/article/get-hardware-system-information-python
 #
 
 import platform
 from datetime import datetime
 from . import cpuinfo
+import importlib
 
 def check_imp():
     import sys
     import subprocess
     try:
         import psutil
         return True
     except ModuleNotFoundError as e:
         # Extract the name of the missing module
         missing_module = str(e).split("'")[1]
         print(f"Attempting to install missing module: {missing_module}")
         subprocess.check_call([sys.executable, "-m", "pip", "install", missing_module])
         return False
 
-psenv = False
-while not psenv:
-    psenv = check_imp()
-if psenv:
-    import psutil
+
+def ensure_lib(module_name):
+    def decorator(func):
+        def wrapper(*args, **kwargs):
+            if module_name not in globals():
+                try:
+                    globals()[module_name] = importlib.import_module(module_name)
+                except ImportError:
+                    raise ImportError(f"Module {module_name} is required but not installed.")
+            return func(*args, **kwargs)
+        return wrapper
+    return decorator
     
 def get_size(bytes, suffix="B"):
     """
     Scale bytes to its proper format
     e.g:
         1253656 => '1.20MB'
         1253656678 => '1.17GB'
@@ -44,23 +52,24 @@
     print(f"System: {uname.system}")
     print(f"Node Name: {uname.node}")
     print(f"Release: {uname.release}")
     print(f"Version: {uname.version}")
     print(f"Machine: {uname.machine}")
     print(f"Processor: {uname.processor}")
 
+@ensure_lib('psutil')
 def boot_time():
     # Boot Time
     print("="*40, "Boot Time", "="*40)
     boot_time_timestamp = psutil.boot_time()
     bt = datetime.fromtimestamp(boot_time_timestamp)
     print(f"Boot Time: {bt.year}/{bt.month}/{bt.day} {bt.hour}:{bt.minute}:{bt.second}")
 
+@ensure_lib('psutil')
 def info_cpu():
-    import psutil
     # let's print CPU information
     print("="*40, "CPU Info", "="*40)
     
     print('CPU: ' + cpuinfo.get_cpu_info().get('brand_raw', "Unknown"))
     # number of cores
     print("Physical cores:", psutil.cpu_count(logical=False))
     print("Total cores:", psutil.cpu_count(logical=True))
@@ -74,15 +83,15 @@
         print("CPU Usage Per Core:")
         for i, percentage in enumerate(psutil.cpu_percent(percpu=True, interval=1)):
             print(f"{f'Core':>8} {i:>2}: {percentage :>6}%")
         print(f"Total CPU Usage: {psutil.cpu_percent()}%")
     except FileNotFoundError:
         pass
 
-
+@ensure_lib('psutil')
 def info_mem():
     # Memory Information
     print("="*40, "Memory Information", "="*40)
     # get the memory details
     svmem = psutil.virtual_memory()
     print(f"Total: {get_size(svmem.total)}")
     print(f"Available: {get_size(svmem.available)}")
@@ -117,14 +126,15 @@
         print(f"  Free: {get_size(partition_usage.free)}")
         print(f"  Percentage: {partition_usage.percent}%")
     # get IO statistics since boot
     disk_io = psutil.disk_io_counters()
     print(f"Total read: {get_size(disk_io.read_bytes)}")
     print(f"Total write: {get_size(disk_io.write_bytes)}")
 
+@ensure_lib('psutil')
 def info_net():
     # Network information
     print("="*40, "Network Information", "="*40)
     # get all network interfaces (virtual and physical)
     if_addrs = psutil.net_if_addrs()
     for interface_name, interface_addresses in if_addrs.items():
         for address in interface_addresses:
@@ -189,11 +199,12 @@
             ))
 
         print(tabulate(list_gpus, headers=("id", "name", "load", "free memory", "used memory", "total memory",
                                         "temperature", "uuid")))
         
 
 if __name__ == "__main__":
+    boot_time()
     info_sys()
     info_cpu()
     info_mem()
     # info_gpu()
```

