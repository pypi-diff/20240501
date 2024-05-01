# Comparing `tmp/mkdoxy-1.2.2.tar.gz` & `tmp/mkdoxy-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdoxy-1.2.2.tar", last modified: Fri Apr 19 09:27:28 2024, max compression
+gzip compressed data, was "mkdoxy-1.2.3.tar", last modified: Wed May  1 09:18:55 2024, max compression
```

## Comparing `mkdoxy-1.2.2.tar` & `mkdoxy-1.2.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-19 09:27:28.119857 mkdoxy-1.2.2/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.2.2/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     5843 2024-04-19 09:27:28.119613 mkdoxy-1.2.2/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     4473 2024-04-18 23:45:18.000000 mkdoxy-1.2.2/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-19 09:27:28.113539 mkdoxy-1.2.2/mkdoxy/
--rw-r--r--   0 kuba       (501) staff       (20)     2935 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/DoxyTagParser.py
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.2.2/mkdoxy/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      303 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/cache.py
--rw-r--r--   0 kuba       (501) staff       (20)     3585 2024-04-19 08:51:39.000000 mkdoxy-1.2.2/mkdoxy/constants.py
--rw-r--r--   0 kuba       (501) staff       (20)     5619 2024-04-18 23:46:38.000000 mkdoxy-1.2.2/mkdoxy/doxygen.py
--rw-r--r--   0 kuba       (501) staff       (20)     9921 2024-04-18 23:45:10.000000 mkdoxy-1.2.2/mkdoxy/doxyrun.py
--rw-r--r--   0 kuba       (501) staff       (20)      603 2024-04-03 00:10:24.000000 mkdoxy-1.2.2/mkdoxy/filters.py
--rw-r--r--   0 kuba       (501) staff       (20)     2414 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/finder.py
--rw-r--r--   0 kuba       (501) staff       (20)    13298 2024-04-18 23:45:14.000000 mkdoxy-1.2.2/mkdoxy/generatorAuto.py
--rw-r--r--   0 kuba       (501) staff       (20)    20151 2024-04-19 09:23:21.000000 mkdoxy-1.2.2/mkdoxy/generatorBase.py
--rw-r--r--   0 kuba       (501) staff       (20)    15034 2024-04-03 00:10:24.000000 mkdoxy-1.2.2/mkdoxy/generatorSnippets.py
--rw-r--r--   0 kuba       (501) staff       (20)     5320 2024-04-03 00:10:24.000000 mkdoxy-1.2.2/mkdoxy/markdown.py
--rw-r--r--   0 kuba       (501) staff       (20)    26618 2024-04-18 23:46:44.000000 mkdoxy-1.2.2/mkdoxy/node.py
--rw-r--r--   0 kuba       (501) staff       (20)     9076 2024-04-19 08:51:39.000000 mkdoxy-1.2.2/mkdoxy/plugin.py
--rw-r--r--   0 kuba       (501) staff       (20)    11689 2024-04-18 23:46:45.000000 mkdoxy-1.2.2/mkdoxy/property.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-19 09:27:28.118267 mkdoxy-1.2.2/mkdoxy/templates/
--rw-r--r--   0 kuba       (501) staff       (20)      517 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/templates/annotated.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      380 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/templates/classes.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      544 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/templates/code.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      614 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/templates/error.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      214 2024-04-03 00:10:24.000000 mkdoxy-1.2.2/mkdoxy/templates/example.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      582 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/templates/examples.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      408 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/templates/files.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      499 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/templates/hierarchy.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      438 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/templates/index.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      797 2024-04-18 23:45:18.000000 mkdoxy-1.2.2/mkdoxy/templates/memDef.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     1698 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/templates/memTab.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     4673 2024-04-18 23:45:14.000000 mkdoxy-1.2.2/mkdoxy/templates/member.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      426 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/templates/modules.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      414 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/templates/namespaces.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      272 2024-04-03 00:10:24.000000 mkdoxy-1.2.2/mkdoxy/templates/page.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      465 2024-04-03 00:10:24.000000 mkdoxy-1.2.2/mkdoxy/templates/programlisting.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      233 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/templates/relatedPages.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     3534 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/mkdoxy/utils.py
--rw-r--r--   0 kuba       (501) staff       (20)     9999 2024-04-18 23:46:47.000000 mkdoxy-1.2.2/mkdoxy/xml_parser.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-19 09:27:28.118785 mkdoxy-1.2.2/mkdoxy.egg-info/
--rw-r--r--   0 kuba       (501) staff       (20)     5843 2024-04-19 09:27:28.000000 mkdoxy-1.2.2/mkdoxy.egg-info/PKG-INFO
--rwxr-xr-x   0 kuba       (501) staff       (20)     1127 2024-04-19 09:27:28.000000 mkdoxy-1.2.2/mkdoxy.egg-info/SOURCES.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        1 2024-04-19 09:27:28.000000 mkdoxy-1.2.2/mkdoxy.egg-info/dependency_links.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)       47 2024-04-19 09:27:28.000000 mkdoxy-1.2.2/mkdoxy.egg-info/entry_points.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)      143 2024-04-19 09:27:28.000000 mkdoxy-1.2.2/mkdoxy.egg-info/requires.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        7 2024-04-19 09:27:28.000000 mkdoxy-1.2.2/mkdoxy.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)       62 2024-04-02 23:57:40.000000 mkdoxy-1.2.2/pyproject.toml
--rw-r--r--   0 kuba       (501) staff       (20)       38 2024-04-19 09:27:28.119896 mkdoxy-1.2.2/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)     1841 2024-04-19 09:24:03.000000 mkdoxy-1.2.2/setup.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-04-19 09:27:28.118501 mkdoxy-1.2.2/tests/
--rw-r--r--   0 kuba       (501) staff       (20)     2390 2024-04-03 00:10:24.000000 mkdoxy-1.2.2/tests/test_doxyrun.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-01 09:18:55.291480 mkdoxy-1.2.3/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.2.3/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     5843 2024-05-01 09:18:55.291229 mkdoxy-1.2.3/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     4473 2024-04-18 23:45:18.000000 mkdoxy-1.2.3/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-01 09:18:55.285937 mkdoxy-1.2.3/mkdoxy/
+-rw-r--r--   0 kuba       (501) staff       (20)     2935 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/DoxyTagParser.py
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.2.3/mkdoxy/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      303 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/cache.py
+-rw-r--r--   0 kuba       (501) staff       (20)     3585 2024-04-19 08:51:39.000000 mkdoxy-1.2.3/mkdoxy/constants.py
+-rw-r--r--   0 kuba       (501) staff       (20)     5619 2024-04-18 23:46:38.000000 mkdoxy-1.2.3/mkdoxy/doxygen.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9806 2024-05-01 08:49:31.000000 mkdoxy-1.2.3/mkdoxy/doxyrun.py
+-rw-r--r--   0 kuba       (501) staff       (20)      603 2024-04-03 00:10:24.000000 mkdoxy-1.2.3/mkdoxy/filters.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2414 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/finder.py
+-rw-r--r--   0 kuba       (501) staff       (20)    13298 2024-04-18 23:45:14.000000 mkdoxy-1.2.3/mkdoxy/generatorAuto.py
+-rw-r--r--   0 kuba       (501) staff       (20)    20151 2024-05-01 09:14:08.000000 mkdoxy-1.2.3/mkdoxy/generatorBase.py
+-rw-r--r--   0 kuba       (501) staff       (20)    15506 2024-05-01 09:11:13.000000 mkdoxy-1.2.3/mkdoxy/generatorSnippets.py
+-rw-r--r--   0 kuba       (501) staff       (20)     5320 2024-04-03 00:10:24.000000 mkdoxy-1.2.3/mkdoxy/markdown.py
+-rw-r--r--   0 kuba       (501) staff       (20)    26618 2024-04-18 23:46:44.000000 mkdoxy-1.2.3/mkdoxy/node.py
+-rw-r--r--   0 kuba       (501) staff       (20)     8941 2024-05-01 08:49:31.000000 mkdoxy-1.2.3/mkdoxy/plugin.py
+-rw-r--r--   0 kuba       (501) staff       (20)    11689 2024-04-18 23:46:45.000000 mkdoxy-1.2.3/mkdoxy/property.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-01 09:18:55.289900 mkdoxy-1.2.3/mkdoxy/templates/
+-rw-r--r--   0 kuba       (501) staff       (20)      517 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/annotated.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      380 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/classes.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      544 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/code.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      614 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/error.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      214 2024-04-03 00:10:24.000000 mkdoxy-1.2.3/mkdoxy/templates/example.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      582 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/examples.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      408 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/files.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      499 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/hierarchy.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      438 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/index.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      797 2024-04-18 23:45:18.000000 mkdoxy-1.2.3/mkdoxy/templates/memDef.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     1698 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/memTab.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     4673 2024-04-18 23:45:14.000000 mkdoxy-1.2.3/mkdoxy/templates/member.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      426 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/modules.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      414 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/namespaces.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      272 2024-04-03 00:10:24.000000 mkdoxy-1.2.3/mkdoxy/templates/page.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      465 2024-04-03 00:10:24.000000 mkdoxy-1.2.3/mkdoxy/templates/programlisting.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      233 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/templates/relatedPages.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     3534 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/mkdoxy/utils.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9999 2024-04-18 23:46:47.000000 mkdoxy-1.2.3/mkdoxy/xml_parser.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-01 09:18:55.290388 mkdoxy-1.2.3/mkdoxy.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)     5843 2024-05-01 09:18:55.000000 mkdoxy-1.2.3/mkdoxy.egg-info/PKG-INFO
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1127 2024-05-01 09:18:55.000000 mkdoxy-1.2.3/mkdoxy.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        1 2024-05-01 09:18:55.000000 mkdoxy-1.2.3/mkdoxy.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)       47 2024-05-01 09:18:55.000000 mkdoxy-1.2.3/mkdoxy.egg-info/entry_points.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)      143 2024-05-01 09:18:55.000000 mkdoxy-1.2.3/mkdoxy.egg-info/requires.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        7 2024-05-01 09:18:55.000000 mkdoxy-1.2.3/mkdoxy.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       62 2024-04-02 23:57:40.000000 mkdoxy-1.2.3/pyproject.toml
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2024-05-01 09:18:55.291518 mkdoxy-1.2.3/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1841 2024-05-01 09:15:31.000000 mkdoxy-1.2.3/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-01 09:18:55.290115 mkdoxy-1.2.3/tests/
+-rw-r--r--   0 kuba       (501) staff       (20)     2390 2024-04-03 00:10:24.000000 mkdoxy-1.2.3/tests/test_doxyrun.py
```

### Comparing `mkdoxy-1.2.2/LICENSE` & `mkdoxy-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/PKG-INFO` & `mkdoxy-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.2.2
+Version: 1.2.3
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.2 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.3 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
```

### Comparing `mkdoxy-1.2.2/README.md` & `mkdoxy-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/DoxyTagParser.py` & `mkdoxy-1.2.3/mkdoxy/DoxyTagParser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/constants.py` & `mkdoxy-1.2.3/mkdoxy/constants.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/doxygen.py` & `mkdoxy-1.2.3/mkdoxy/doxygen.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/doxyrun.py` & `mkdoxy-1.2.3/mkdoxy/doxyrun.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     def __init__(
         self,
         doxygenBinPath: str,
         doxygenSource: str,
         tempDoxyFolder: str,
         doxyCfgNew,
         doxyConfigFile: Optional[str] = None,
-        runPath: Optional[str] = None,
     ):
         """! Constructor.
         Default Doxygen config options:
 
         - INPUT: <doxygenSource>
         - OUTPUT_DIRECTORY: <tempDoxyFolder>
         - DOXYFILE_ENCODING: UTF-8
@@ -54,15 +53,14 @@
 
         self.doxygenBinPath: str = doxygenBinPath
         self.doxygenSource: str = doxygenSource
         self.tempDoxyFolder: str = tempDoxyFolder
         self.doxyConfigFile: Optional[str] = doxyConfigFile
         self.hashFileName: str = "hashChanges.yaml"
         self.hashFilePath: PurePath = PurePath.joinpath(Path(self.tempDoxyFolder), Path(self.hashFileName))
-        self.runPath: Optional[str] = runPath
         self.doxyCfg: dict = self.setDoxyCfg(doxyCfgNew)
 
     def setDoxyCfg(self, doxyCfgNew: dict) -> dict:
         """! Set the Doxygen configuration.
         @details If a custom Doxygen config file is provided, it will be used. Otherwise, default options will be used.
         @details Order of application of parameters:
         @details 1. Custom Doxygen config file
@@ -220,15 +218,14 @@
         @details
         """
         doxyBuilder = Popen(
             [self.doxygenBinPath, "-"],
             stdout=PIPE,
             stdin=PIPE,
             stderr=PIPE,
-            cwd=self.runPath,
         )
         (doxyBuilder.communicate(self.dox_dict2str(self.doxyCfg).encode("utf-8"))[0].decode().strip())
         # log.info(self.destinationDir)
         # log.info(stdout_data)
 
     def checkAndRun(self):
         """! Check if the source files have changed since the last run and run Doxygen if they have.
```

### Comparing `mkdoxy-1.2.2/mkdoxy/filters.py` & `mkdoxy-1.2.3/mkdoxy/filters.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/finder.py` & `mkdoxy-1.2.3/mkdoxy/finder.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/generatorAuto.py` & `mkdoxy-1.2.3/mkdoxy/generatorAuto.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/generatorBase.py` & `mkdoxy-1.2.3/mkdoxy/generatorBase.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/generatorSnippets.py` & `mkdoxy-1.2.3/mkdoxy/generatorSnippets.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,61 +55,67 @@
         path = pathlib.PurePath(self.page.url).parts
         self.pageUrlPrefix = "".join("../" for _ in range(len(path) - 1))
 
     def generate(self):
         if self.is_doxy_inactive(self.config):
             return self.markdown  # doxygen is inactive return unchanged markdown
 
-        matches = re.finditer(regexIncorrect, self.markdown, re.MULTILINE)
-        for match in reversed(list(matches)):
-            snippet = match.group()
-            project_name = match.group("project") or "<project_name>"
-
-            snippet_config = self.config.copy()
-            snippet_config.update(self.try_load_yaml(match.group("yaml"), project_name, snippet, self.config))
-
-            if self.is_doxy_inactive(snippet_config):
-                continue
-
-            replacement = (
-                self.incorrect_argument(project_name, "", snippet_config, snippet)
-                if self.is_project_exist(project_name)
-                else self.incorrect_project(project_name, snippet_config, snippet)
-            )
-            self.replace_markdown(match.start(), match.end(), replacement)
+        try:
+            matches = re.finditer(regexIncorrect, self.markdown, re.MULTILINE)
+            for match in reversed(list(matches)):
+                snippet = match.group()
+                project_name = match.group("project") or "<project_name>"
+
+                snippet_config = self.config.copy()
+                snippet_config.update(self.try_load_yaml(match.group("yaml"), project_name, snippet, self.config))
+
+                if self.is_doxy_inactive(snippet_config):
+                    continue
+
+                replacement = (
+                    self.incorrect_argument(project_name, "", snippet_config, snippet)
+                    if self.is_project_exist(project_name)
+                    else self.incorrect_project(project_name, snippet_config, snippet)
+                )
+                self.replace_markdown(match.start(), match.end(), replacement)
 
-        matches = re.finditer(regexShort, self.markdown, re.MULTILINE)
-        for match in reversed(list(matches)):
-            snippet = match.group()
-            argument = match.group("argument").lower()
-            project_name = match.group("project")
-
-            snippet_config = self.config.copy()
-            snippet_config.update(self.try_load_yaml(match.group("yaml"), project_name, snippet, self.config))
-
-            if self.is_doxy_inactive(snippet_config):
-                continue
-
-            replaceStr = self.call_doxy_by_name(snippet, project_name, argument, snippet_config)
-            self.replace_markdown(match.start(), match.end(), replaceStr)
-
-        matches = re.finditer(regexLong, self.markdown, re.MULTILINE)
-        for match in reversed(list(matches)):
-            snippet = match.group()
-            argument = match.group("argument").lower()
-            project_name = match.group("project")
-            # log.debug(f"\nArgument: {argument}")
-
-            # config has been updated by yaml
-            snippet_config = self.config.copy()
-            snippet_config.update(self.try_load_yaml(match.group("yaml"), project_name, snippet, self.config))
-
-            replaceStr = self.call_doxy_by_name(snippet, project_name, argument, snippet_config)
-            self.replace_markdown(match.start(), match.end(), replaceStr)
-        return self.markdown
+            matches = re.finditer(regexShort, self.markdown, re.MULTILINE)
+            for match in reversed(list(matches)):
+                snippet = match.group()
+                argument = match.group("argument").lower()
+                project_name = match.group("project")
+
+                snippet_config = self.config.copy()
+                snippet_config.update(self.try_load_yaml(match.group("yaml"), project_name, snippet, self.config))
+
+                if self.is_doxy_inactive(snippet_config):
+                    continue
+
+                replaceStr = self.call_doxy_by_name(snippet, project_name, argument, snippet_config)
+                self.replace_markdown(match.start(), match.end(), replaceStr)
+
+            matches = re.finditer(regexLong, self.markdown, re.MULTILINE)
+            for match in reversed(list(matches)):
+                snippet = match.group()
+                argument = match.group("argument").lower()
+                project_name = match.group("project")
+                # log.debug(f"\nArgument: {argument}")
+
+                # config has been updated by yaml
+                snippet_config = self.config.copy()
+                snippet_config.update(self.try_load_yaml(match.group("yaml"), project_name, snippet, self.config))
+
+                replaceStr = self.call_doxy_by_name(snippet, project_name, argument, snippet_config)
+                self.replace_markdown(match.start(), match.end(), replaceStr)
+            return self.markdown
+        except Exception as e:
+            basename = pathlib.Path(__file__).name
+            log.error(f"Error in {self.page.url} page. Incorrect doxy snippet or error in file {basename}")
+            log.error(f"Error: {e}")
+            return self.markdown
 
     def try_load_yaml(self, yaml_raw: str, project: str, snippet: str, config: dict) -> dict:
         try:
             return yaml.safe_load(yaml_raw)
         except yaml.YAMLError:
             log.error(f"YAML error in {project} project on page {self.page.url}")
             self.doxyError(
@@ -374,16 +380,16 @@
         self._recurs_setLinkPrefixNodes(nodes, self.pageUrlPrefix + project + "/")
         return self.generatorBase[project].fileindex(nodes, config)
 
     def doxyNodeIsNone(self, project: str, config: dict, snippet: str) -> str:
         return self.doxyError(
             project,
             config,
-            "Node is None",
-            "Node is None",
+            f"Could not find coresponding snippet for project {project}",
+            f"Config: {config}",
             "yaml",
             snippet,
         )
 
 
 ### Create documentation generator callbacks END
```

### Comparing `mkdoxy-1.2.2/mkdoxy/markdown.py` & `mkdoxy-1.2.3/mkdoxy/markdown.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/node.py` & `mkdoxy-1.2.3/mkdoxy/node.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/plugin.py` & `mkdoxy-1.2.3/mkdoxy/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """@package mkdoxy.plugin
 MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 
 MkDoxy is a MkDocs plugin for generating documentation from Doxygen XML files.
 """
 
 import logging
-import os
 from pathlib import Path, PurePath
 
 from mkdocs import exceptions
 from mkdocs.config import Config, base, config_options
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure import files, pages
 
@@ -110,22 +109,20 @@
 
             if self.config.get("save-api"):
                 tempDirApi = tempDir("", self.config.get("save-api"), project_name)
             else:
                 tempDirApi = tempDir(config["site_dir"], "assets/.doxy/", project_name)
 
             # Check src changes -> run Doxygen
-            runPath = os.path.dirname(config.config_file_path) if config.config_file_path else None
             doxygenRun = DoxygenRun(
                 self.config["doxygen-bin-path"],
                 project_data.get("src-dirs"),
                 tempDirApi,
                 project_data.get("doxy-cfg", {}),
                 project_data.get("doxy-cfg-file", ""),
-                runPath,
             )
             if doxygenRun.checkAndRun():
                 log.info("  -> generating Doxygen files")
             else:
                 log.info("  -> skip generating Doxygen files (nothing changes)")
 
             # Parse XML to basic structure
```

### Comparing `mkdoxy-1.2.2/mkdoxy/property.py` & `mkdoxy-1.2.3/mkdoxy/property.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/templates/annotated.jinja2` & `mkdoxy-1.2.3/mkdoxy/templates/annotated.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/templates/code.jinja2` & `mkdoxy-1.2.3/mkdoxy/templates/code.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/templates/error.jinja2` & `mkdoxy-1.2.3/mkdoxy/templates/error.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/templates/examples.jinja2` & `mkdoxy-1.2.3/mkdoxy/templates/examples.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/templates/memDef.jinja2` & `mkdoxy-1.2.3/mkdoxy/templates/memDef.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/templates/memTab.jinja2` & `mkdoxy-1.2.3/mkdoxy/templates/memTab.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/templates/member.jinja2` & `mkdoxy-1.2.3/mkdoxy/templates/member.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/utils.py` & `mkdoxy-1.2.3/mkdoxy/utils.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy/xml_parser.py` & `mkdoxy-1.2.3/mkdoxy/xml_parser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/mkdoxy.egg-info/PKG-INFO` & `mkdoxy-1.2.3/mkdoxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.2.2
+Version: 1.2.3
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.2 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.2.3 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
```

### Comparing `mkdoxy-1.2.2/mkdoxy.egg-info/SOURCES.txt` & `mkdoxy-1.2.3/mkdoxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.2.2/setup.py` & `mkdoxy-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     with open("requirements.txt") as f:
         return f.read().splitlines()
 
 
 # https://pypi.org/project/mkdoxy/
 setup(
     name="mkdoxy",
-    version="1.2.2",
+    version="1.2.3",
     description="MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords="mkdoxy, python, open-source, documentation, mkdocs, doxygen, multilanguage, code-snippets, code, snippets, documentation-generator",  # noqa: E501
     url="https://github.com/JakubAndrysek/MkDoxy",
     author="Jakub Andrýsek",
     author_email="email@kubaandrysek.cz",
```

### Comparing `mkdoxy-1.2.2/tests/test_doxyrun.py` & `mkdoxy-1.2.3/tests/test_doxyrun.py`

 * *Files identical despite different names*

