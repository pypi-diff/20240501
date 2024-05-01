# Comparing `tmp/natlinkcore-5.3.7.tar.gz` & `tmp/natlinkcore-5.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natlinkcore-5.3.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "natlinkcore-5.3.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `natlinkcore-5.3.7.tar` & `natlinkcore-5.3.8.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0     1797 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/pyproject.toml
--rw-r--r--   0        0        0     2479 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/readme.md
--rw-r--r--   0        0        0     2872 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/DefaultConfig/_config_instructions.py
--rw-r--r--   0        0        0      945 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/DefaultConfig/_information_config.py
--rw-r--r--   0        0        0     1626 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/DefaultConfig/natlink.ini
--rw-r--r--   0        0        0     5466 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/Index.htm
--rw-r--r--   0        0        0     3486 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_globals.py
--rw-r--r--   0        0        0    12976 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_mouse.py
--rw-r--r--   0        0        0     1725 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_repeatthat.py
--rw-r--r--   0        0        0     1273 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample1.py
--rw-r--r--   0        0        0     2025 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample2.py
--rw-r--r--   0        0        0     2014 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample3.py
--rw-r--r--   0        0        0     1224 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample4.py
--rw-r--r--   0        0        0     2320 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample5.py
--rw-r--r--   0        0        0     4218 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample8.py
--rw-r--r--   0        0        0      772 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample9.py
--rw-r--r--   0        0        0      578 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sleeping.py
--rw-r--r--   0        0        0     2924 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/excel_sample7.py
--rw-r--r--   0        0        0     1751 2023-10-08 18:23:21.674630 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/natspeak_sample6.py
--rw-r--r--   0        0        0    15323 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/trainuser.py
--rw-r--r--   0        0        0     7169 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/transcribe.py
--rw-r--r--   0        0        0    15374 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/wiki.css
--rw-r--r--   0        0        0    11218 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/windict.py
--rw-r--r--   0        0        0    10122 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/winspch.py
--rw-r--r--   0        0        0     3989 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/winword_styles_sample.py
--rw-r--r--   0        0        0    10824 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/wordpad.py
--rw-r--r--   0        0        0       38 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/__init__.py
--rw-r--r--   0        0        0     2742 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_debug_natlink.py
--rw-r--r--   0        0        0     1403 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_sample7.py
--rw-r--r--   0        0        0     1878 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_sample_callback.py
--rw-r--r--   0        0        0     1437 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_sample_directory_information.py
--rw-r--r--   0        0        0     2899 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_sample_natlinkstatus.py
--rw-r--r--   0        0        0     1731 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_sample_runmimic.py
--rw-r--r--   0        0        0     1339 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_samplehypothesis.py
--rw-r--r--   0        0        0      642 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/__init__.py
--rw-r--r--   0        0        0     4846 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/_natlink_core.pyi
--rw-r--r--   0        0        0     2253 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/callbackhandler.py
--rw-r--r--   0        0        0     9723 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/config.py
--rw-r--r--   0        0        0     1436 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/configure/README.md
--rw-r--r--   0        0        0       76 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/configure/__init__.py
--rw-r--r--   0        0        0      930 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/configure/list of functions.txt
--rw-r--r--   0        0        0      740 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/configure/natlink_extensions.py
--rw-r--r--   0        0        0    15149 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/configure/natlinkconfig_cli.py
--rw-r--r--   0        0        0     8432 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/configure/natlinkconfig_gui.py
--rw-r--r--   0        0        0    29422 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/configure/natlinkconfigfunctions.py
--rw-r--r--   0        0        0    31456 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/gramparser.py
--rw-r--r--   0        0        0    29575 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/loader.py
--rw-r--r--   0        0        0     4846 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/natlink.pyi
--rw-r--r--   0        0        0    32027 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/natlinkstatus.py
--rw-r--r--   0        0        0    15049 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/natlinktimer.py
--rw-r--r--   0        0        0    52024 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/natlinkutils.py
--rw-r--r--   0        0        0    17506 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/nsformat.py
--rw-r--r--   0        0        0        0 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/py.typed
--rw-r--r--   0        0        0     7321 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/readwritefile.py
--rw-r--r--   0        0        0     2827 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/redirect_output.py
--rw-r--r--   0        0        0     1307 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/singleton.py
--rw-r--r--   0        0        0     3341 2023-10-08 18:23:21.678629 natlinkcore-5.3.7/src/natlinkcore/tkinter_dialogs.py
--rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 natlinkcore-5.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1797 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1680 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/readme.md
+-rw-r--r--   0        0        0     2872 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/DefaultConfig/_config_instructions.py
+-rw-r--r--   0        0        0      945 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/DefaultConfig/_information_config.py
+-rw-r--r--   0        0        0     1626 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/DefaultConfig/natlink.ini
+-rw-r--r--   0        0        0     5466 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/Index.htm
+-rw-r--r--   0        0        0     3486 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_globals.py
+-rw-r--r--   0        0        0    12976 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_mouse.py
+-rw-r--r--   0        0        0     1725 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_repeatthat.py
+-rw-r--r--   0        0        0     1273 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample1.py
+-rw-r--r--   0        0        0     2025 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample2.py
+-rw-r--r--   0        0        0     2014 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample3.py
+-rw-r--r--   0        0        0     1224 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample4.py
+-rw-r--r--   0        0        0     2320 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample5.py
+-rw-r--r--   0        0        0     4218 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample8.py
+-rw-r--r--   0        0        0      772 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample9.py
+-rw-r--r--   0        0        0      578 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sleeping.py
+-rw-r--r--   0        0        0     2924 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/excel_sample7.py
+-rw-r--r--   0        0        0     1751 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/natspeak_sample6.py
+-rw-r--r--   0        0        0    15323 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/trainuser.py
+-rw-r--r--   0        0        0     7169 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/transcribe.py
+-rw-r--r--   0        0        0    15374 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/wiki.css
+-rw-r--r--   0        0        0    11218 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/windict.py
+-rw-r--r--   0        0        0    10122 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/winspch.py
+-rw-r--r--   0        0        0     3989 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/winword_styles_sample.py
+-rw-r--r--   0        0        0    10824 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/wordpad.py
+-rw-r--r--   0        0        0       38 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/__init__.py
+-rw-r--r--   0        0        0     2742 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_debug_natlink.py
+-rw-r--r--   0        0        0     1403 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_sample7.py
+-rw-r--r--   0        0        0     5208 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_sample_activatedeactivate.py
+-rw-r--r--   0        0        0     1878 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_sample_callback.py
+-rw-r--r--   0        0        0     1437 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_sample_directory_information.py
+-rw-r--r--   0        0        0     2899 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_sample_natlinkstatus.py
+-rw-r--r--   0        0        0     1731 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_sample_runmimic.py
+-rw-r--r--   0        0        0     1339 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_samplehypothesis.py
+-rw-r--r--   0        0        0      642 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/__init__.py
+-rw-r--r--   0        0        0     4846 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/_natlink_core.pyi
+-rw-r--r--   0        0        0     2253 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/callbackhandler.py
+-rw-r--r--   0        0        0     9723 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/config.py
+-rw-r--r--   0        0        0     1436 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/configure/README.md
+-rw-r--r--   0        0        0       76 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/configure/__init__.py
+-rw-r--r--   0        0        0      930 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/configure/list of functions.txt
+-rw-r--r--   0        0        0      740 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/configure/natlink_extensions.py
+-rw-r--r--   0        0        0    15149 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/configure/natlinkconfig_cli.py
+-rw-r--r--   0        0        0     8432 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/configure/natlinkconfig_gui.py
+-rw-r--r--   0        0        0    29422 2024-01-27 20:41:26.525332 natlinkcore-5.3.8/src/natlinkcore/configure/natlinkconfigfunctions.py
+-rw-r--r--   0        0        0    31456 2024-01-27 20:41:26.529332 natlinkcore-5.3.8/src/natlinkcore/gramparser.py
+-rw-r--r--   0        0        0    29944 2024-01-27 20:41:26.529332 natlinkcore-5.3.8/src/natlinkcore/loader.py
+-rw-r--r--   0        0        0     4846 2024-01-27 20:41:26.529332 natlinkcore-5.3.8/src/natlinkcore/natlink.pyi
+-rw-r--r--   0        0        0    32027 2024-01-27 20:41:26.529332 natlinkcore-5.3.8/src/natlinkcore/natlinkstatus.py
+-rw-r--r--   0        0        0    15049 2024-01-27 20:41:26.529332 natlinkcore-5.3.8/src/natlinkcore/natlinktimer.py
+-rw-r--r--   0        0        0    52138 2024-01-27 20:41:26.529332 natlinkcore-5.3.8/src/natlinkcore/natlinkutils.py
+-rw-r--r--   0        0        0    17506 2024-01-27 20:41:26.529332 natlinkcore-5.3.8/src/natlinkcore/nsformat.py
+-rw-r--r--   0        0        0        0 2024-01-27 20:41:26.529332 natlinkcore-5.3.8/src/natlinkcore/py.typed
+-rw-r--r--   0        0        0     7321 2024-01-27 20:41:26.529332 natlinkcore-5.3.8/src/natlinkcore/readwritefile.py
+-rw-r--r--   0        0        0     2827 2024-01-27 20:41:26.529332 natlinkcore-5.3.8/src/natlinkcore/redirect_output.py
+-rw-r--r--   0        0        0     1307 2024-01-27 20:41:26.529332 natlinkcore-5.3.8/src/natlinkcore/singleton.py
+-rw-r--r--   0        0        0     3341 2024-01-27 20:41:26.529332 natlinkcore-5.3.8/src/natlinkcore/tkinter_dialogs.py
+-rw-r--r--   0        0        0     2783 1970-01-01 00:00:00.000000 natlinkcore-5.3.8/PKG-INFO
```

### Comparing `natlinkcore-5.3.7/pyproject.toml` & `natlinkcore-5.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/readme.md` & `natlinkcore-5.3.8/readme.md`

 * *Files 21% similar despite different names*

```diff
@@ -5,55 +5,35 @@
  Please refer to the README file in the project repository [https://github.com/dictation-toolbox/natlink](https://github.com/dictation-toolbox/natlink) for more information about natlink.
 
 ## Installing from PyPi
 You can install from [The Python Package Index (PyPI)](https://pypi.org/) with 
 
 `py -m pip install natlinkcore`
 
+Note that natlinkcore will not install if you have not installed Natlink first.  Natlink is installed through running an installer.
+
  
 ## Test Framework
 Tests use the [pytest](https://docs.pytest.org/) framework.  
 For developers, if you are developing on the project, please add tests for any new features or bug
 fixes.  
 
 Mandy Python IDEs such as [Visual Studio Code](https://code.visualstudio.com/) have build in support for test frameworks and make it easy to run and debug pytest.   see [Visual Studio Code for testing](https://code.visualstudio.com/docs/python/testing).
 
 
 ## Building the Python Package Locally
 
-The build happens through a powershell script.  You don't have to know much powershell.  
-The powershell script runs the tests using [pytest](https://docs.pytest.org/).  
-
-The package is built with [Flit](https://flit.pypa.io/).  The package will be produced in
-dist/natlinkcore-x.y.z-py3-none-any.whl.  To install it `py -m pip install dist/natlinkcore-x.y.z-py3-none-any.whl` replacing x.y with the version numbers.
-
-Normally if you are developing natlinkcore, you will with instead to install with `py -m pip install -e .`, which will
-let you make and test changes without reinstalling natlinkcore with pip.  **Note the flit install --symlink or --pth-file options are problematic so just use pip.**
-
-
-To start a powershell from the command prompt, type `powershell`.
-
-To build the package:
-
+`py -m build` to build the Python package locally.
 
-`py -m flit build`   from powershell or command prompt, which will run the the tests in natlinkcore/test, then build the the package.
-
-
-To publish the package to [The Python Package Index (PyPI)](https://pypi.org/)
-
-`publish_natlinkcore` from powershell.
-
-
- 
+Publishing to PyPi is done through the [trusted publisher mechanism](https://docs.pypi.org/trusted-publishers/using-a-publisher/) when a release is created on github using github actions. 
 
 
 ## Publishing checklist
 Before you bump the version number in __init__.py and publish:
 - Check the pyroject.toml file for package dependancies.  Do you need a specfic or newer version of
 a dependancy such as dtactions?  Then add or update the version # requirement in dtactions.  
-- don't publish if the tests are failing.   The `publish_natlinkcore` will prevent this, please don't work around it.
 
 ## Debugging Instructions
 
 Read the detailed developer instructions for setting up the debugger.  You can look in this projects tree until 
 documentation/developers.rst.
```

### Comparing `natlinkcore-5.3.7/src/natlinkcore/DefaultConfig/_config_instructions.py` & `natlinkcore-5.3.8/src/natlinkcore/DefaultConfig/_config_instructions.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/DefaultConfig/_information_config.py` & `natlinkcore-5.3.8/src/natlinkcore/DefaultConfig/_information_config.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/DefaultConfig/natlink.ini` & `natlinkcore-5.3.8/src/natlinkcore/DefaultConfig/natlink.ini`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/Index.htm` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/Index.htm`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_globals.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_globals.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_mouse.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_mouse.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_repeatthat.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_repeatthat.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample1.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample1.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample2.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample2.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample3.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample3.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample4.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample4.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample5.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample5.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample8.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample8.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample9.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sample9.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sleeping.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/_sleeping.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/excel_sample7.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/excel_sample7.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/natspeak_sample6.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/natspeak_sample6.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/trainuser.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/trainuser.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/transcribe.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/transcribe.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/wiki.css` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/wiki.css`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/windict.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/windict.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/winspch.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/winspch.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/winword_styles_sample.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/winword_styles_sample.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/OriginalSampleMacros/wordpad.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/OriginalSampleMacros/wordpad.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_debug_natlink.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_debug_natlink.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_sample7.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_sample7.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_sample_callback.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_sample_callback.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_sample_directory_information.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_sample_directory_information.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_sample_natlinkstatus.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_sample_natlinkstatus.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_sample_runmimic.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_sample_runmimic.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/SampleMacros/_samplehypothesis.py` & `natlinkcore-5.3.8/src/natlinkcore/SampleMacros/_samplehypothesis.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/__init__.py` & `natlinkcore-5.3.8/src/natlinkcore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''Python portion of Natlink, a compatibility module for Dragon Naturally Speaking
 The python stuff including test modules'''
-__version__="5.3.7"
+__version__="5.3.8"
 #pylint:disable=
 from pathlib import Path
 
 def getThisDir(fileOfModule):
     """get directory of calling module
     """
     return Path(fileOfModule).parent
```

### Comparing `natlinkcore-5.3.7/src/natlinkcore/_natlink_core.pyi` & `natlinkcore-5.3.8/src/natlinkcore/_natlink_core.pyi`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/callbackhandler.py` & `natlinkcore-5.3.8/src/natlinkcore/callbackhandler.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/config.py` & `natlinkcore-5.3.8/src/natlinkcore/config.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/configure/README.md` & `natlinkcore-5.3.8/src/natlinkcore/configure/README.md`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/configure/list of functions.txt` & `natlinkcore-5.3.8/src/natlinkcore/configure/list of functions.txt`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/configure/natlink_extensions.py` & `natlinkcore-5.3.8/src/natlinkcore/configure/natlink_extensions.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/configure/natlinkconfig_cli.py` & `natlinkcore-5.3.8/src/natlinkcore/configure/natlinkconfig_cli.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/configure/natlinkconfig_gui.py` & `natlinkcore-5.3.8/src/natlinkcore/configure/natlinkconfig_gui.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/configure/natlinkconfigfunctions.py` & `natlinkcore-5.3.8/src/natlinkcore/configure/natlinkconfigfunctions.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/gramparser.py` & `natlinkcore-5.3.8/src/natlinkcore/gramparser.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/loader.py` & `natlinkcore-5.3.8/src/natlinkcore/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import importlib
 import importlib.machinery
 import importlib.util
 import logging
 import os
 import copy
 import sys
-import sysconfig
+import sys
 import time
 import traceback
-import debugpy
 import winreg
 import configparser
 from pathlib import Path
 from types import ModuleType
 from typing import List, Dict, Set, Iterable, Any, Tuple, Callable
+import debugpy
 
 import natlink
 from natlinkcore.config import LogLevel, NatlinkConfig, expand_path
 from natlinkcore.readwritefile import ReadWriteFile
 from natlinkcore.callbackhandler import CallbackHandler
 from natlinkcore.singleton import Singleton
 # the possible languages (for get_user_language) (runs at start and on_change_callback, user)
@@ -66,14 +66,18 @@
         self._post_load_callback =  CallbackHandler('post_load')
         self._on_mic_on_callback = CallbackHandler('on_mic_on')
         self._on_mic_off_callback = CallbackHandler('on_mic_off')
         self._on_begin_utterance_callback = CallbackHandler('on_begin_utterance')
         self.seen: Set[Path] = set()     # start empty in trigger_load
         self.bom = self.encoding = self.config_text = ''   # getconfigsetting and writeconfigsetting
         self.dap_started=False
+        # for shorter logger.debug messages
+        self.prev_module_info = None
+
+
 
     def set_on_begin_utterance_callback(self, func: Callable[[], None]) -> None:
         self._on_begin_utterance_callback.set(func)
 
     def set_on_mic_on_callback(self, func: Callable[[], None]) -> None:
         self._on_mic_on_callback.set(func)
     
@@ -424,15 +428,21 @@
             self.logger.debug('on_change_callback called with: "mic", "off"')
             self._on_mic_off_callback.run()
         else:
             self.logger.debug(f'on_change_callback unhandled: change_type: "{change_type}", args: "{args}"')
             
 
     def on_begin_callback(self, module_info: Tuple[str, str, int]) -> None:
-        self.logger.debug(f'on_begin_callback called with: moduleInfo: {module_info}')
+        if module_info != self.prev_module_info:
+            prog_name = Path(module_info[0]).stem
+            self.logger.debug(f'-on_begin_callback, new module info: ( (...){prog_name}, {module_info[1]}, {module_info[2]} )')
+            self.prev_module_info = module_info
+        else:
+            self.logger.debug('-on_begin_callback, same moduleInfo')
+            
         self._on_begin_utterance_callback.run()
        
         prog_name = Path(module_info[0].lower()).stem
         if prog_name not in self.prog_names_visited:
             self.prog_names_visited.add(prog_name)
             self.trigger_load()
         elif self.load_on_begin_utterance:
@@ -619,28 +629,28 @@
 
     # choose between .natlink/natlink.ini in home or the fallback_directory:         
     return [join(home, config_sub_dir, natlink_inifile), fallback_config_file]
 
 def run() -> None:
     logger = logging.getLogger('natlink')
     try:
-        # TODO: remove this hack. As of October 2021, win32api does not load properly, except if
-        # the package pywin32_system32 is explictly put on new dll_directory white-list
-        pywin32_dir = os.path.join(sysconfig.get_path('platlib'), "pywin32_system32")
-        if os.path.isdir(pywin32_dir):
-            os.add_dll_directory(pywin32_dir)
+        # # TODO: remove this hack. As of October 2021, win32api does not load properly, except if
+        # # the package pywin32_system32 is explictly put on new dll_directory white-list
+        # pywin32_dir = os.path.join(sysconfig.get_path('platlib'), "pywin32_system32")
+        # if os.path.isdir(pywin32_dir):
+        #     os.add_dll_directory(pywin32_dir)
         
         config = NatlinkConfig.from_first_found_file(config_locations())
         dap_started=False
         print(f"testing dap , enabled {config.dap_enabled} port {config.dap_port}")
         try:
             if config.dap_enabled:
-                print(f"Debugpy.configure ...")
+                print("Debugpy.configure ...")
                 debugpy.configure(python=f"{python_exec}")
-                print(f"Debugpy.listen ...")
+                print("Debugpy.listen ...")
  
                 debugpy.listen(config.dap_port)
                 dap_started=True
 
                 print(f"DAP Started on Port {config.dap_port} in {__file__}")
                 if config.dap_wait_for_debugger_attach_on_startup:
                     print(" waiting for debugger to attach")
```

### Comparing `natlinkcore-5.3.7/src/natlinkcore/natlink.pyi` & `natlinkcore-5.3.8/src/natlinkcore/natlink.pyi`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/natlinkstatus.py` & `natlinkcore-5.3.8/src/natlinkcore/natlinkstatus.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/natlinktimer.py` & `natlinkcore-5.3.8/src/natlinkcore/natlinktimer.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/natlinkutils.py` & `natlinkcore-5.3.8/src/natlinkcore/natlinkutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,16 @@
       A utility function which determines whether moduleInfo matches a
       specified module name and window title.  Returns window handle on
       match and None on mismatch. Note that moduleInfo may be ("","",0)
       which we should handle cleanly.
 
 
 """
-#pylint:disable=C0116, C0209, C0302, R0902, W0702, E1101, W0703
+#pylint:disable=C0116, C0209, C0302, R0902, W0702, E1101, W0703, R1735
+#pylint:disable=W0237    # inconsistent calling sequences for different classes 
 
 import os
 import os.path
 import copy
 import struct
 import sys
 import traceback
@@ -359,16 +360,15 @@
     # if that member function is defined.
 
     def callIfExists(self, funcName, argList):
         try:
             func = getattr(self, funcName)
         except AttributeError:
             return None
-        else:
-            return func(*argList)
+        return func(*argList)
         
 
 #---------------------------------------------------------------------------
 # GrammarBase
 #
 # This is the basic grammar class.  All user grammar classes should use this
 # as the base class.
@@ -710,124 +710,126 @@
         while self.validLists:
             self.validLists.pop()
         self.exclusiveState = 0
         self.is_loaded = False
 
     def activate(self, ruleName, window=0, exclusive=None, noError=0):
         #pylint:disable=W0221, W0613
-        # TODO: remove debugLoad (via logger)
-        # TODO: noError is not used
-        if debugLoad:
-            print(f'GrammarBase, activate ruleName "{ruleName}" in window {window}, exclusive: {exclusive}')
+        debug_print(f'GrammarBase, activate ruleName "{ruleName}" in window {window}, exclusive: {exclusive}')
         if ruleName not in self.validRules:
-            raise ValueError( "rule %s was not exported in the grammar" % ruleName)
+            if not noError or debug_print:
+                print(f'rule "{ruleName}" was not exported in the grammar')
+            return
+        
         if ruleName in self.activeRules:
             if window == self.activeRules[ruleName]:
-                if debugLoad:
-                    print('rule %s already active for window %s'% (ruleName, window))
+                if not noError or debug_print:
+                    print(f'rule "{ruleName}" already active for window {window}')
                 return
-            if debugLoad:
-                print('change rule %s from window %s to window %s'% (ruleName, self.activeRules[ruleName], window))
+            debug_print(f'change rule "{ruleName}" from window {self.activeRules[ruleName]} to {window}')
             self.gramObj.deactivate(ruleName)
-        # if debugLoad: print('activate rule %s (window: %s)'% (ruleName, window))
-        self.gramObj.activate(ruleName,window)
+        # debug_print( print('activate rule %s (window: %s)'% (ruleName, window))
+        self.gramObj.activate(ruleName, window)
         self.activeRules[ruleName] = window
         if not exclusive is None:
-            if debugLoad:
-                print(f'set exclusive mode to {exclusive} for rule "{ruleName}"')
+            debug_print(f'set exclusive mode to {exclusive} for rule "{ruleName}"')
             self.setExclusive(exclusive)
 
-    def deactivate(self, ruleName, noError=0):
+    def deactivate(self, ruleName, noError=0, dpi16trick=True):
         #pylint:disable=W0221
+        debug_print(f'deactivate: {ruleName}, activeRules: {self.activeRules}')
         if ruleName not in self.validRules:
             if noError:
                 return
             raise ValueError(f'rule "{ruleName}" was not exported in the grammar')
         if ruleName not in self.activeRules:
-            if noError:
-                return
-            raise ValueError( "rule %s is not active (activeRules: %s)"% (ruleName, self.activeRules))
-        if debugLoad:
-            print('deactivate rule %s'% ruleName)
+            if not noError:
+                print(f'rule "{ruleName}" is not active, no need to deactivate (activeRules: {set(self.activeRules.keys())})')
+            return
+        debug_print('deactivate rule %s'% ruleName)
+        if dpi16trick:
+            # now deactivate  all and activate other rules again
+            # be sure, this one is not called recursive!!
+            active_rules = copy.copy(self.activeRules)
+            del active_rules[ruleName]
+            self.deactivateAll()
+            for rule, window in active_rules.items():
+                self.activate(rule, window)
+            return
+        # previous behaviour (as long as dpi16trick is not changed in call)
         self.gramObj.deactivate(ruleName)
         del self.activeRules[ruleName]
 
     def activateSet(self, ruleNames, window=0, exclusive=None):
         """activate a set of rules.
 
+        dpi16: deactivate all and activate the new rules.
         """
         #pylint:disable=R0912
-        if isinstance(ruleNames, list):
-            rulenames = copy.copy(ruleNames) # so we can pop items
-        elif isinstance(ruleNames, tuple):
-            rulenames = list(ruleNames) # so we can pop items
-        else:
-            raise TypeError("activateSet, ruleNames (%s) must be a list or a tuple, not: %s"%
-                            (repr(ruleNames), type(ruleNames)))
-        activeKeys = list(self.activeRules.keys())
-        for x in activeKeys:
-
-            curWindow = self.activeRules[x]
-            if x in rulenames:
-                if curWindow == window:
-                    rulenames.remove(x)
-                else:
-                    self.deactivate(x)
+        debug_print(f'activateSet: {ruleNames}, window: {window}')
+        active_rules = set(self.activeRules.keys())
+        if set(ruleNames) == active_rules:
+            for rule in ruleNames:
+                if not (rule in self.activeRules and self.activeRules[rule] == window):
+                    break
             else:
-                # if same window, deactivate, otherwise just leave...
-                # deactivate direct to gramObj here:
-                if window == curWindow:
-                    if debugLoad:
-                        print('activateSet, do not want %s, so deactivate, same window: %s'% (x, curWindow))
-                    self.deactivate(x)
-                elif window == 0:
-                    if debugLoad:
-                        print('activateSet, deactivate rule %s (global), previous window: %s'% (x, curWindow))
-                    self.deactivate(x)
-                elif curWindow == 0:
-                    if debugLoad:
-                        print('activateSet, deactivate global rule %s, new window window: %s'% (x, window))
-                    self.deactivate(x)
-                else:
-                    if debugLoad:
-                        print('activateSet, deactivate not needed, different window: rule %s, previous window: %s new window: %s'% (x, curWindow, window))             
-        for x in rulenames:
+                debug_print(f'activateSet {ruleNames} not needed, set is already active for window: {window}')
+                return
+
+        self.deactivateAll()
+          
+        for x in ruleNames:
             self.activate(x, window)
         if not exclusive is None:
             self.setExclusive(exclusive)
 
-    def deactivateSet(self, ruleNames, noError=0):
-        if not type(ruleNames ) in (list, tuple):
-            raise TypeError("deactivateSet, ruleNames (%s) must be a list or a tuple, not: %s"%
-                            (repr(ruleNames), type(ruleNames)))
-        for x in ruleNames:
-            self.deactivate(x, noError=noError)
+    def deactivateSet(self, ruleNames):
+        debug_print(f'deactivateSet: {ruleNames}')
+        rule_names = set(ruleNames)
+        prev_rules = copy.copy(self.activeRules)
+        if prev_rules:
+            active_names = set(prev_rules.keys())
+        else:
+            debug_print(f'deactiveSet "{ruleNames}", no rules are active in this grammar')
+            return
+        if not active_names.intersection(ruleNames):
+            debug_print(f'deactiveSet, ruleNames {ruleNames} are not active in this grammar: {active_names}')
+            return
+        remain_names = active_names - rule_names
+        self.deactivateAll()
+        for x in remain_names:
+            window = prev_rules[x]
+            self.activate(x, window)
 
     def activateAll(self, window=0, exclusive=None, exceptlist=None):
         """activate all rules
         
         as experiment first deactivate all rules before doing so
         """
-        allRules = copy.copy(self.validRules)
+        all_rules = set(self.validRules)
         if exceptlist:
             for x in exceptlist:
-                allRules.remove(x)
-            # if debugLoad: print('activateAll except %s'% exceptlist)
+                if x in all_rules:
+                    print(f'discard from allRules: {x}')
+                    all_rules.discard(x)
+            print(f'activateAll except {exceptlist}: {all_rules}')
             
-        self.activateSet(allRules, window=window, exclusive=exclusive)
+        self.activateSet(all_rules, window=window, exclusive=exclusive)
         if not exclusive is None:
             self.setExclusive(exclusive)
 
     def _deactivateAll(self):
         """deactivate all rules, no change of exclusive state
         """
         activeRules = list(self.activeRules.keys())
         
         for x in activeRules:
-            self.deactivate(x)
+            debug_print(f'deactivate rule {x}')
+            self.gramObj.deactivate(x)
+        self.activeRules = {}
 
     def deactivateAll(self):
         """deactivate all rules and reset explicit the exclusive state of the grammar
         """
         self._deactivateAll()
         self.setExclusive(0)
 
@@ -1306,7 +1308,13 @@
     for x in fullResults:
         if x[1] in _dict:
             _dict[x[1]].append(x[0])
         else:
             _dict[x[1]] = [x[0]]
     return _dict
 
+def debug_print(msg):
+    """depends on variable debugLoad at top of module
+    """
+    if debugLoad:
+        print(msg)
+
```

### Comparing `natlinkcore-5.3.7/src/natlinkcore/nsformat.py` & `natlinkcore-5.3.8/src/natlinkcore/nsformat.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/readwritefile.py` & `natlinkcore-5.3.8/src/natlinkcore/readwritefile.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/redirect_output.py` & `natlinkcore-5.3.8/src/natlinkcore/redirect_output.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/singleton.py` & `natlinkcore-5.3.8/src/natlinkcore/singleton.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/src/natlinkcore/tkinter_dialogs.py` & `natlinkcore-5.3.8/src/natlinkcore/tkinter_dialogs.py`

 * *Files identical despite different names*

### Comparing `natlinkcore-5.3.7/PKG-INFO` & `natlinkcore-5.3.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natlinkcore
-Version: 5.3.7
+Version: 5.3.8
 Summary: Python portion of Natlink, a compatibility module for Dragon Naturally Speaking
 Author-email: "Quintijn Hoogenboom (maintainer)" <q.hoogenboom@antenna.nl>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
@@ -31,56 +31,36 @@
  Please refer to the README file in the project repository [https://github.com/dictation-toolbox/natlink](https://github.com/dictation-toolbox/natlink) for more information about natlink.
 
 ## Installing from PyPi
 You can install from [The Python Package Index (PyPI)](https://pypi.org/) with 
 
 `py -m pip install natlinkcore`
 
+Note that natlinkcore will not install if you have not installed Natlink first.  Natlink is installed through running an installer.
+
  
 ## Test Framework
 Tests use the [pytest](https://docs.pytest.org/) framework.  
 For developers, if you are developing on the project, please add tests for any new features or bug
 fixes.  
 
 Mandy Python IDEs such as [Visual Studio Code](https://code.visualstudio.com/) have build in support for test frameworks and make it easy to run and debug pytest.   see [Visual Studio Code for testing](https://code.visualstudio.com/docs/python/testing).
 
 
 ## Building the Python Package Locally
 
-The build happens through a powershell script.  You don't have to know much powershell.  
-The powershell script runs the tests using [pytest](https://docs.pytest.org/).  
-
-The package is built with [Flit](https://flit.pypa.io/).  The package will be produced in
-dist/natlinkcore-x.y.z-py3-none-any.whl.  To install it `py -m pip install dist/natlinkcore-x.y.z-py3-none-any.whl` replacing x.y with the version numbers.
-
-Normally if you are developing natlinkcore, you will with instead to install with `py -m pip install -e .`, which will
-let you make and test changes without reinstalling natlinkcore with pip.  **Note the flit install --symlink or --pth-file options are problematic so just use pip.**
-
-
-To start a powershell from the command prompt, type `powershell`.
-
-To build the package:
-
+`py -m build` to build the Python package locally.
 
-`py -m flit build`   from powershell or command prompt, which will run the the tests in natlinkcore/test, then build the the package.
-
-
-To publish the package to [The Python Package Index (PyPI)](https://pypi.org/)
-
-`publish_natlinkcore` from powershell.
-
-
- 
+Publishing to PyPi is done through the [trusted publisher mechanism](https://docs.pypi.org/trusted-publishers/using-a-publisher/) when a release is created on github using github actions. 
 
 
 ## Publishing checklist
 Before you bump the version number in __init__.py and publish:
 - Check the pyroject.toml file for package dependancies.  Do you need a specfic or newer version of
 a dependancy such as dtactions?  Then add or update the version # requirement in dtactions.  
-- don't publish if the tests are failing.   The `publish_natlinkcore` will prevent this, please don't work around it.
 
 ## Debugging Instructions
 
 Read the detailed developer instructions for setting up the debugger.  You can look in this projects tree until 
 documentation/developers.rst.
```

