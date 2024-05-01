# Comparing `tmp/OZI.build-0.0.1.tar.gz` & `tmp/OZI.build-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI.build-0.0.1.tar", last modified: Wed Feb 21 22:15:58 2024, max compression
+gzip compressed data, was "OZI.build-0.0.2.tar", last modified: Wed May  1 02:34:39 2024, max compression
```

## Comparing `OZI.build-0.0.1.tar` & `OZI.build-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-02-21 22:15:58.864753 OZI.build-0.0.1/
--rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-02-21 22:15:40.000000 OZI.build-0.0.1/.gitignore
--rw-rw-r--   0 ross      (1000) ross      (1000)      422 2024-02-21 22:15:40.000000 OZI.build-0.0.1/.gitlab-ci.yml
--rw-rw-r--   0 ross      (1000) ross      (1000)    11359 2024-02-21 22:15:40.000000 OZI.build-0.0.1/COPYING
--rw-rw-r--   0 ross      (1000) ross      (1000)      482 2024-02-21 22:15:40.000000 OZI.build-0.0.1/README.rst
--rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-02-21 22:15:40.000000 OZI.build-0.0.1/__init__.py
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-02-21 22:15:58.860753 OZI.build-0.0.1/doc/
--rwxrwxr-x   0 ross      (1000) ross      (1000)      650 2024-02-21 22:15:40.000000 OZI.build-0.0.1/doc/generate_doc.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1105 2024-02-21 22:15:40.000000 OZI.build-0.0.1/doc/index.md
--rw-rw-r--   0 ross      (1000) ross      (1000)      623 2024-02-21 22:15:40.000000 OZI.build-0.0.1/doc/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     3388 2024-02-21 22:15:40.000000 OZI.build-0.0.1/doc/pyproject-gen.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     3839 2024-02-21 22:15:40.000000 OZI.build-0.0.1/doc/pyproject.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     1339 2024-02-21 22:15:40.000000 OZI.build-0.0.1/doc/pyproject.md.in
--rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-02-21 22:15:40.000000 OZI.build-0.0.1/doc/sitemap.txt
--rw-rw-r--   0 ross      (1000) ross      (1000)      147 2024-02-21 22:15:40.000000 OZI.build-0.0.1/meson.build
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-02-21 22:15:58.864753 OZI.build-0.0.1/ozi_build/
--rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-02-21 22:15:40.000000 OZI.build-0.0.1/ozi_build/__init__.py
--rw-rw-r--   0 ross      (1000) ross      (1000)    13782 2024-02-21 22:15:40.000000 OZI.build-0.0.1/ozi_build/buildapi.py
--rw-rw-r--   0 ross      (1000) ross      (1000)      132 2024-02-21 22:15:40.000000 OZI.build-0.0.1/ozi_build/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     4275 2024-02-21 22:15:40.000000 OZI.build-0.0.1/ozi_build/pep425tags.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     3540 2024-02-21 22:15:40.000000 OZI.build-0.0.1/ozi_build/schema.py
--rw-rw-r--   0 ross      (1000) ross      (1000)      921 2024-02-21 22:15:40.000000 OZI.build-0.0.1/pyproject.toml
--rwxrwxr-x   0 ross      (1000) ross      (1000)       73 2024-02-21 22:15:40.000000 OZI.build-0.0.1/release
--rw-rw-r--   0 ross      (1000) ross      (1000)     1310 2024-02-21 22:15:58.868753 OZI.build-0.0.1/PKG-INFO
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 02:34:39.867702 OZI.build-0.0.2/
+-rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 02:26:23.000000 OZI.build-0.0.2/.gitignore
+-rw-rw-r--   0 ross      (1000) ross      (1000)      422 2024-05-01 02:26:23.000000 OZI.build-0.0.2/.gitlab-ci.yml
+-rw-rw-r--   0 ross      (1000) ross      (1000)    11359 2024-05-01 02:26:23.000000 OZI.build-0.0.2/COPYING
+-rw-rw-r--   0 ross      (1000) ross      (1000)      482 2024-05-01 02:26:23.000000 OZI.build-0.0.2/README.rst
+-rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 02:26:23.000000 OZI.build-0.0.2/__init__.py
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 02:34:39.867702 OZI.build-0.0.2/doc/
+-rwxrwxr-x   0 ross      (1000) ross      (1000)      650 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/generate_doc.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1105 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/index.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)      623 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3388 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/pyproject-gen.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4171 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/pyproject.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1339 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/pyproject.md.in
+-rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/sitemap.txt
+-rw-rw-r--   0 ross      (1000) ross      (1000)      164 2024-05-01 02:26:23.000000 OZI.build-0.0.2/meson.build
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 02:34:39.867702 OZI.build-0.0.2/ozi_build/
+-rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 02:26:23.000000 OZI.build-0.0.2/ozi_build/__init__.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)    14042 2024-05-01 02:26:23.000000 OZI.build-0.0.2/ozi_build/buildapi.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)      230 2024-05-01 02:26:23.000000 OZI.build-0.0.2/ozi_build/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4275 2024-05-01 02:26:23.000000 OZI.build-0.0.2/ozi_build/pep425tags.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3540 2024-05-01 02:26:23.000000 OZI.build-0.0.2/ozi_build/schema.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1080 2024-05-01 02:26:23.000000 OZI.build-0.0.2/pyproject.toml
+-rwxrwxr-x   0 ross      (1000) ross      (1000)       73 2024-05-01 02:26:23.000000 OZI.build-0.0.2/release
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1353 2024-05-01 02:34:39.875702 OZI.build-0.0.2/PKG-INFO
```

### Comparing `OZI.build-0.0.1/COPYING` & `OZI.build-0.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.1/doc/generate_doc.py` & `OZI.build-0.0.2/doc/generate_doc.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.1/doc/index.md` & `OZI.build-0.0.2/doc/index.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.1/doc/meson.build` & `OZI.build-0.0.2/doc/meson.build`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.1/doc/pyproject-gen.md` & `OZI.build-0.0.2/doc/pyproject-gen.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.1/doc/pyproject.md` & `OZI.build-0.0.2/doc/pyproject.md`

 * *Files 22% similar despite different names*

```diff
@@ -17,114 +17,134 @@
 ## Metadata section
 
 > NOTE: The project version and name are extracted from the `meson.build`
 > [`project()`](http://mesonbuild.com/Reference-manual.html#project) section.
 
 This section is called `[tool.mesonpep517.metadata]` in the file.
 
-### `pkg-info-file` (Optional)
-
-Pass a PKG-INFO file direcly usable.
-
-> ! NOTE: All other keys will be ignored if you pass an already prepared `PKG-INFO`
-> file
-
-
 ### `author`
 
 Your name
 
 ### `author-email`
 
 Your email address
 
 e.g. for mesonpep517 itself:
 
 ``` toml
 [tool.mesonpep517.metadata]
-Author="Thibault Saunier"
-Author-email="tsaunier@gnome.org"
+author="Thibault Saunier"
+author-email="tsaunier@gnome.org"
 ```
 
-### `summary`
+### `classifiers`
 
-A one sentence summary about the package
+A list of [classifiers](https://pypi.python.org/pypi?%3Aaction=list_classifiers).
 
-### `meson-python-option-name` (Optional)
+### `description`
 
-The name of the meson options that is used in the meson build definition
-to set the python installation when using
-[`python.find_installation()`](http://mesonbuild.com/Python-module.html#find_installation).
+The description of the project as a string if you do not want to specify 'description-file'
 
-### `meson-options` (Optional)
+### `description-file`
 
-A list of default meson options to set, can be overriden and expended through the `MESON_ARGS`
-environement variable at build time.
+A path (relative to the .toml file) to a file containing a longer description
+of your package to show on PyPI. This should be written in reStructuredText
+  Markdown or plain text, and the filename should have the appropriate extension
+  (`.rst`, `.md` or `.txt`).
 
-### `requires` (Optional)
+### `home-page`
 
-A list of other packages from PyPI that this package needs. Each package may
-be followed by a version specifier like ``(>=4.1)`` or ``>=4.1``, and/or an
-[environment marker](https://www.python.org/dev/peps/pep-0345/#environment-markers)
-after a semicolon. For example:
+A string containing the URL for the package's home page.
+
+Example:
+
+`http://www.example.com/~cschultz/bvote/`
+
+### `license`
+
+Text indicating the license covering the distribution. This text can be either a valid license expression as defined in [pep639](https://www.python.org/dev/peps/pep-0639/#id88) or any free text.
+
+### `maintainer`
+
+Name of current maintainer of the project (if different from author)
+
+### `maintainer-email`
+
+Maintainer email address
+
+Example:
 
 ``` toml
-      requires = [
-          "requests >=2.6",
-          "configparser; python_version == '2.7'",
-      ]
+[tool.mesonpep517.metadata]
+maintainer="Robin Goode"
+maintainer-email="rgoode@example.org"
 ```
 
-### `description-file` (Optional)
+### `meson-options`
 
-A path (relative to the .toml file) to a file containing a longer description
-of your package to show on PyPI. This should be written in reStructuredText
-  Markdown or plain text, and the filename should have the appropriate extension
-  (`.rst`, `.md` or `.txt`).
+A list of default meson options to set, can be overriden and expended through the `MESON_ARGS`
+environement variable at build time.
 
-### `description` (Optional)
+### `meson-python-option-name`
 
-The description of the project as a string if you do not want to specify 'description-file'
+The name of the meson options that is used in the meson build definition
+to set the python installation when using
+[`python.find_installation()`](http://mesonbuild.com/Python-module.html#find_installation).
 
-### `classifiers` (Optional)
+### `module`
 
-A list of [classifiers](https://pypi.python.org/pypi?%3Aaction=list_classifiers).
+The name of the module, will use the meson project name if not specified
 
-### `requires-python` (Optional)
+### `pkg-info-file`
 
-A version specifier for the versions of Python this requires, e.g. ``~=3.3`` or
-``>=3.3,<4`` which are equivalents.
+Pass a PKG-INFO file direcly usable.
+
+> ! NOTE: All other keys will be ignored if you pass an already prepared `PKG-INFO`
+> file
+
+
+### `platforms`
 
-### `project-urls` (Optional)
+Supported Python platforms, can be 'any', py3, etc...
+
+### `project-urls`
 
 A list of `Type, url` as described in the
 [pep345](https://www.python.org/dev/peps/pep-0345/#project-url-multiple-use).
 For example:
 
 ``` toml
 project-urls = [
     "Source, https://gitlab.com/thiblahute/mesonpep517",
 ]
 ```
 
-### `home-page` (Optional)
-
-A string containing the URL for the package's home page.
+### `requires`
 
-Example:
+A list of other packages from PyPI that this package needs. Each package may
+be followed by a version specifier like ``(>=4.1)`` or ``>=4.1``, and/or an
+[environment marker](https://www.python.org/dev/peps/pep-0345/#environment-markers)
+after a semicolon. For example:
 
-`http://www.example.com/~cschultz/bvote/`
+``` toml
+      requires = [
+          "requests >=2.6",
+          "configparser; python_version == '2.7'",
+      ]
+```
 
-### `platforms` (Optional)
+### `requires-python`
 
-Supported python platforms, can be 'any', py3, etc...
+A version specifier for the versions of Python this requires, e.g. ``~=3.3`` or
+``>=3.3,<4`` which are equivalents.
 
-### `module` (Optional)
+### `summary`
 
-The name of the module, will use the meson project name if not specified
+A one sentence summary about the package
 
 
 ## Entry points section (Optionnal)
 
 You can declare [entry points](http://entrypoints.readthedocs.io/en/latest/)
 in the `[tools.mesonpep517.entry-points]` section. It is a list of
 'entrypointname = module:funcname` strings, for example for console
```

### Comparing `OZI.build-0.0.1/doc/pyproject.md.in` & `OZI.build-0.0.2/doc/pyproject.md.in`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.1/ozi_build/buildapi.py` & `OZI.build-0.0.2/ozi_build/buildapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 if sys.version_info >= (3, 11):
     import tomllib as toml
 elif sys.version_info < (3, 11):
     import tomli as toml
 
 from .pep425tags import get_abbr_impl, get_abi_tag, get_impl_ver, get_platform_tag
 from .schema import VALID_OPTIONS
-
 log = logging.getLogger(__name__)
 
 
-
 def meson(*args, config_settings=None, builddir=''):
     try:
         return subprocess.check_output(['meson'] + list(args))
     except subprocess.CalledProcessError as e:
         stdout = ''
         stderr = ''
         if e.stdout:
@@ -224,15 +222,15 @@
 
 # For now, we require all dependencies to build either a wheel or an sdist.
 get_requires_for_build_sdist = get_requires_for_build_wheel
 
 
 wheel_file_template = """\
 Wheel-Version: 1.0
-Generator: ozi-build
+Generator: ozi_build
 Root-Is-Purelib: {}
 """
 
 
 def _write_wheel_file(f, supports_py2, is_pure):
     f.write(wheel_file_template.format(str(is_pure).lower()))
     if is_pure:
@@ -363,14 +361,19 @@
     def pack_files(self, config):
         for _, installpath in config.installed.items():
             if "site-packages" in installpath:
                 while os.path.basename(installpath) != 'site-packages':
                     installpath = os.path.dirname(installpath)
                 self.wheel_zip.write_files(installpath)
                 break
+            elif "dist-packages" in installpath:
+                while os.path.basename(installpath) != 'dist-packages':
+                    installpath = os.path.dirname(installpath)
+                self.wheel_zip.write_files(installpath)
+                break
 
 
 def build_wheel(wheel_directory,
                 config_settings=None,
                 metadata_directory=None):
     """Builds a wheel, places it in wheel_directory"""
     return WheelBuilder().build(Path(
```

### Comparing `OZI.build-0.0.1/ozi_build/pep425tags.py` & `OZI.build-0.0.2/ozi_build/pep425tags.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.1/ozi_build/schema.py` & `OZI.build-0.0.2/ozi_build/schema.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.1/pyproject.toml` & `OZI.build-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 [build-system]
-requires = ["wheel>0.33", "meson", "toml", "setuptools"]
-backend-path = "."
+requires = [
+    "wheel>0.33",
+    "meson[ninja]>1.1.0",
+    'tomli>=2.0.0;python_version<"3.11"',
+    "setuptools>=64",
+]
+backend-path = [".", "ozi_build"]
 build-backend = "ozi_build.buildapi"
 
 [tool.ozi-build.metadata]
 author="Thibault Saunier"
 author-email="tsaunier@gnome.org"
 maintainer="Eden Rose Duff MSc"
 maintainer-email="help@oziproject.dev"
 summary="Create pep517 compliant packages from the meson build system, OZI-maintained fork."
 home-page="https://github.com/OZI-Project/OZI.build"
-requires-python="py3"
 description-file="README.rst"
-platforms="any"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-requires = ["wheel>0.33", "meson", "toml", "setuptools"]
+requires = ["wheel>0.33", "meson[ninja]>1.1.0", 'tomli>=2.0.0;python_version<"3.11"', "setuptools"]
 project-urls= [
     "Source, https://github.com/OZI-Project/OZI.build",
     "Documentation, https://thiblahute.gitlab.io/mesonpep517/",
 ]
+
+[tool.setuptools.packages.find]
+where = ["ozi_build"]
+namespaces = false
```

### Comparing `OZI.build-0.0.1/PKG-INFO` & `OZI.build-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: OZI.build
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create pep517 compliant packages from the meson build system, OZI-maintained fork.
 Home-page: https://github.com/OZI-Project/OZI.build
 Author: Thibault Saunier
 Author-email: tsaunier@gnome.org
 Maintainer: Eden Rose Duff MSc
 Maintainer-email: help@oziproject.dev
 Requires-Dist: wheel>0.33
-Requires-Dist: meson
-Requires-Dist: toml
+Requires-Dist: meson[ninja]>1.1.0
+Requires-Dist: tomli>=2.0.0;python_version<"3.11"
 Requires-Dist: setuptools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Source, https://github.com/OZI-Project/OZI.build
 Project-URL: Documentation, https://thiblahute.gitlab.io/mesonpep517/
```

