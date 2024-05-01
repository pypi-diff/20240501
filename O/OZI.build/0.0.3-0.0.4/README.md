# Comparing `tmp/OZI.build-0.0.3.tar.gz` & `tmp/OZI.build-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI.build-0.0.3.tar", last modified: Wed May  1 04:03:10 2024, max compression
+gzip compressed data, was "OZI.build-0.0.4.tar", last modified: Wed May  1 14:51:38 2024, max compression
```

## Comparing `OZI.build-0.0.3.tar` & `OZI.build-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 04:03:10.665827 OZI.build-0.0.3/
--rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 04:01:24.000000 OZI.build-0.0.3/.gitignore
--rw-rw-r--   0 ross      (1000) ross      (1000)      422 2024-05-01 04:01:24.000000 OZI.build-0.0.3/.gitlab-ci.yml
--rw-rw-r--   0 ross      (1000) ross      (1000)    11359 2024-05-01 04:01:24.000000 OZI.build-0.0.3/COPYING
--rw-rw-r--   0 ross      (1000) ross      (1000)      482 2024-05-01 04:01:24.000000 OZI.build-0.0.3/README.rst
--rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 04:01:24.000000 OZI.build-0.0.3/__init__.py
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 04:03:10.665827 OZI.build-0.0.3/doc/
--rwxrwxr-x   0 ross      (1000) ross      (1000)      651 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/generate_doc.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1105 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/index.md
--rw-rw-r--   0 ross      (1000) ross      (1000)      623 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     3388 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/pyproject-gen.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     4171 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/pyproject.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     1339 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/pyproject.md.in
--rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/sitemap.txt
--rw-rw-r--   0 ross      (1000) ross      (1000)      164 2024-05-01 04:01:24.000000 OZI.build-0.0.3/meson.build
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 04:03:10.665827 OZI.build-0.0.3/ozi_build/
--rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 04:01:24.000000 OZI.build-0.0.3/ozi_build/__init__.py
--rw-rw-r--   0 ross      (1000) ross      (1000)    14363 2024-05-01 04:01:24.000000 OZI.build-0.0.3/ozi_build/buildapi.py
--rw-rw-r--   0 ross      (1000) ross      (1000)      230 2024-05-01 04:01:24.000000 OZI.build-0.0.3/ozi_build/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     4275 2024-05-01 04:01:24.000000 OZI.build-0.0.3/ozi_build/pep425tags.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     3509 2024-05-01 04:01:24.000000 OZI.build-0.0.3/ozi_build/schema.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1102 2024-05-01 04:01:24.000000 OZI.build-0.0.3/pyproject.toml
--rwxrwxr-x   0 ross      (1000) ross      (1000)       73 2024-05-01 04:01:24.000000 OZI.build-0.0.3/release
--rw-rw-r--   0 ross      (1000) ross      (1000)     1353 2024-05-01 04:03:10.673827 OZI.build-0.0.3/PKG-INFO
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 14:51:38.911227 OZI.build-0.0.4/
+-rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 14:49:25.000000 OZI.build-0.0.4/.gitignore
+-rw-rw-r--   0 ross      (1000) ross      (1000)      422 2024-05-01 14:49:25.000000 OZI.build-0.0.4/.gitlab-ci.yml
+-rw-rw-r--   0 ross      (1000) ross      (1000)    11359 2024-05-01 14:49:25.000000 OZI.build-0.0.4/COPYING
+-rw-rw-r--   0 ross      (1000) ross      (1000)      482 2024-05-01 14:49:25.000000 OZI.build-0.0.4/README.rst
+-rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 14:49:25.000000 OZI.build-0.0.4/__init__.py
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 14:51:38.907226 OZI.build-0.0.4/doc/
+-rwxrwxr-x   0 ross      (1000) ross      (1000)      651 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/generate_doc.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1105 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/index.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)      623 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3388 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/pyproject-gen.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4171 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/pyproject.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1339 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/pyproject.md.in
+-rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/sitemap.txt
+-rw-rw-r--   0 ross      (1000) ross      (1000)      164 2024-05-01 14:49:25.000000 OZI.build-0.0.4/meson.build
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 14:51:38.911227 OZI.build-0.0.4/ozi_build/
+-rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 14:49:25.000000 OZI.build-0.0.4/ozi_build/__init__.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)    14745 2024-05-01 14:49:25.000000 OZI.build-0.0.4/ozi_build/buildapi.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)      230 2024-05-01 14:49:25.000000 OZI.build-0.0.4/ozi_build/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4297 2024-05-01 14:49:25.000000 OZI.build-0.0.4/ozi_build/pep425tags.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3509 2024-05-01 14:49:25.000000 OZI.build-0.0.4/ozi_build/schema.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1132 2024-05-01 14:49:25.000000 OZI.build-0.0.4/pyproject.toml
+-rwxrwxr-x   0 ross      (1000) ross      (1000)       73 2024-05-01 14:49:25.000000 OZI.build-0.0.4/release
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1353 2024-05-01 14:51:38.915227 OZI.build-0.0.4/PKG-INFO
```

### Comparing `OZI.build-0.0.3/COPYING` & `OZI.build-0.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.3/doc/generate_doc.py` & `OZI.build-0.0.4/doc/generate_doc.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.3/doc/index.md` & `OZI.build-0.0.4/doc/index.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.3/doc/meson.build` & `OZI.build-0.0.4/doc/meson.build`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.3/doc/pyproject-gen.md` & `OZI.build-0.0.4/doc/pyproject-gen.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.3/doc/pyproject.md` & `OZI.build-0.0.4/doc/pyproject.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.3/doc/pyproject.md.in` & `OZI.build-0.0.4/doc/pyproject.md.in`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.3/ozi_build/buildapi.py` & `OZI.build-0.0.4/ozi_build/buildapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """PEP-517 compliant buildsystem API"""
 
 import contextlib
 import json
 import logging
 import os
+import shutil
 import subprocess
 import sys
 import sysconfig
 import tarfile
 import tempfile
 from gzip import GzipFile
 from pathlib import Path
@@ -34,20 +35,22 @@
     except subprocess.CalledProcessError as e:
         stdout = ''
         stderr = ''
         if e.stdout:
             stdout = e.stdout.decode()
         if e.stderr:
             stderr = e.stderr.decode()
-        print("Could not run meson: %s\n%s" % (stdout, stderr), file=sys.stderr)
+        print(
+            "Could not run meson: %s\n%s" % (stdout, stderr), file=sys.stderr
+        )
         try:
             fulllog = os.path.join(builddir, 'meson-logs', 'meson-log.txt')
             with open(fulllog) as f:
                 print("Full log: %s" % f.read())
-        except:
+        except IOError:
             print("Could not open %s" % fulllog)
             pass
         raise e
 
 
 def meson_configure(*args, config_settings=None):
     if 'MESON_ARGS' in os.environ:
@@ -74,15 +77,17 @@
 }
 
 
 class Config:
     def __init__(self, builddir=None):
         config = self.__get_config()
         self.__metadata = config['tool']['ozi-build']['metadata']
-        self.__entry_points = config['tool']['ozi-build'].get('entry-points', [])
+        self.__entry_points = config['tool']['ozi-build'].get(
+            'entry-points', []
+        )
         self.installed = []
         self.options = []
         self.builddir = None
         if builddir:
             self.set_builddir(builddir)
 
     def validate_options(self):
@@ -103,15 +108,17 @@
                     "%s is mandatory in the `[tool.ozi-build.metadata] section but was not found"
                     % field
                 )
 
     def __introspect(self, introspect_type):
         with open(
             os.path.join(
-                self.__builddir, 'meson-info', 'intro-' + introspect_type + '.json'
+                self.__builddir,
+                'meson-info',
+                'intro-' + introspect_type + '.json',
             )
         ) as f:
             return json.load(f)
 
     def set_builddir(self, builddir):
         self.__builddir = builddir
         project = self.__introspect('projectinfo')
@@ -157,17 +164,17 @@
         }
 
         if 'pkg-info-file' in self:
             res = '\n'.join(PKG_INFO.split('\n')[:3]).format(**meta) + '\n'
             with open(self['pkg-info-file'], 'r') as f:
                 orig_lines = f.readlines()
                 for line in orig_lines:
-                    if line.startswith('Metadata-Version:') or line.startswith(
-                        'Version:'
-                    ):
+                    if line.startswith(
+                        'Metadata-Version:'
+                    ) or line.startswith('Version:'):
                         continue
                     res += line
 
             return res
 
         res = PKG_INFO.format(**meta)
 
@@ -203,15 +210,17 @@
             description_content_type = readme_ext_to_content_type.get(
                 description_file.suffix.lower(), description_content_type
             )
         elif 'description' in self:
             description = self['description']
 
         if description:
-            res += 'Description-Content-Type: {}\n'.format(description_content_type)
+            res += 'Description-Content-Type: {}\n'.format(
+                description_content_type
+            )
             res += 'Description:\n\n' + description
 
         return res
 
     def get_entry_points(self):
         res = ''
         for group_name in sorted(self.__entry_points):
@@ -256,28 +265,35 @@
     if is_pure:
         if supports_py2:
             f.write("Tag: py2-none-any\n")
         f.write("Tag: py3-none-any\n")
     else:
         f.write(
             "Tag: {0}{1}-{2}-{3}\n".format(
-                get_abbr_impl(), get_impl_ver(), get_abi_tag(), get_platform_tag()
+                get_abbr_impl(),
+                get_impl_ver(),
+                get_abi_tag(),
+                get_platform_tag(),
             )
         )
 
 
 def check_is_pure(installed):
     variables = sysconfig.get_config_vars()
-    suffix = variables.get('EXT_SUFFIX') or variables.get('SO') or variables.get('.so')
+    suffix = (
+        variables.get('EXT_SUFFIX')
+        or variables.get('SO')
+        or variables.get('.so')
+    )
     # msys2's python3 has "-cpython-36m.dll", we have to be clever
     split = suffix.rsplit('.', 1)
     suffix = split.pop(-1)
 
     for installpath in installed.values():
-        if "site-packages" in installpath:
+        if "site-packages" in installpath or "dist-packages" in installpath:
             if installpath.split('.')[-1] == suffix:
                 return False
 
     return True
 
 
 def prepare_metadata_for_build_wheel(
@@ -318,71 +334,78 @@
                           pep425tags.get_abi_tag())
 )
 """
 
 
 def get_abi(python):
     return (
-        subprocess.check_output([python, '-c', GET_CHECK]).decode('utf-8').strip('\n')
+        subprocess.check_output([python, '-c', GET_CHECK])
+        .decode('utf-8')
+        .strip('\n')
     )
 
 
 class WheelBuilder:
     def __init__(self):
         self.wheel_zip = None  # type: ignore
         self.builddir = tempfile.TemporaryDirectory()
         self.installdir = tempfile.TemporaryDirectory()
 
     def build(self, wheel_directory, config_settings, metadata_dir):
         config = Config()
 
-        args = [self.builddir.name, '--prefix', self.installdir.name] + config.get(
-            'meson-options', []
-        )
+        args = [
+            self.builddir.name,
+            '--prefix',
+            self.installdir.name,
+        ] + config.get('meson-options', [])
         meson_configure(*args, config_settings=config_settings)
         config.set_builddir(self.builddir.name)
 
         metadata_dir = prepare_metadata_for_build_wheel(
             wheel_directory, builddir=self.builddir.name, config=config
         )
 
         is_pure = check_is_pure(config.installed)
-        platform_tag = config.get('platforms', 'any' if is_pure else get_platform_tag())
-
+        platform_tag = config.get(
+            'platforms', 'any' if is_pure else get_platform_tag()
+        )
+        option_build = config.get('meson-python-option-name')
+        python = 'python3'
+        if not option_build:
+            log.warning(
+                "meson-python-option-name not specified in the "
+                + "[tool.ozi-build.metadata] section, assuming `python3`"
+            )
+        else:
+            for opt in config.options:
+                if opt['name'] == 'python_version':
+                    python = opt['value']
+                    break
         if not is_pure:
-            python = 'python3'
-            option_build = config.get('meson-python-option-name')
-            if not option_build:
-                python = 'python3'
-                log.warning(
-                    "meson-python-option-name not specified in the "
-                    + "[tool.ozi-build.metadata] section, assuming `python3`"
-                )
-            else:
-                for opt in config.options:
-                    if opt['name'] == 'python_version':
-                        python = opt['value']
-                        break
             abi = get_abi(python)
         else:
-            abi = '{}-none'.format(config.get('requires-python', f'py3{sys.version_info[1]}'))
+            abi = '{}-none'.format(
+                config.get('requires-python', get_abi(python))
+            )
 
         target_fp = wheel_directory / '{}-{}-{}-{}.whl'.format(
             config['module'],
             config['version'],
             abi,
             platform_tag,
         )
 
         self.wheel_zip: WheelFile = WheelFile(str(target_fp), 'w')
         for f in os.listdir(str(wheel_directory / metadata_dir)):
             self.wheel_zip.write(
                 str(wheel_directory / metadata_dir / f),
                 arcname=str(Path(metadata_dir) / f),
             )
+        shutil.rmtree(Path(wheel_directory) / metadata_dir)
 
         # Make sure everything is built
         meson('install', '-C', self.builddir.name)
         self.pack_files(config)
         self.wheel_zip.close()
         return str(target_fp)
 
@@ -396,15 +419,17 @@
             elif "dist-packages" in installpath:
                 while os.path.basename(installpath) != 'dist-packages':
                     installpath = os.path.dirname(installpath)
                 self.wheel_zip.write_files(installpath)
                 break
 
 
-def build_wheel(wheel_directory, config_settings=None, metadata_directory=None):
+def build_wheel(
+    wheel_directory, config_settings=None, metadata_directory=None
+):
     """Builds a wheel, places it in wheel_directory"""
     return WheelBuilder().build(
         Path(wheel_directory), config_settings, metadata_directory
     )
 
 
 def build_sdist(sdist_directory, config_settings=None):
@@ -437,15 +462,18 @@
             distfilename = '%s.tar.gz' % tf_dir
             target = distdir / distfilename
             source_date_epoch = os.environ.get('SOURCE_DATE_EPOCH', '')
             mtime = int(source_date_epoch) if source_date_epoch else None
             with GzipFile(str(target), mode='wb', mtime=mtime) as gz:
                 with cd(installdir):
                     with tarfile.TarFile(
-                        str(target), mode='w', fileobj=gz, format=tarfile.PAX_FORMAT
+                        str(target),
+                        mode='w',
+                        fileobj=gz,
+                        format=tarfile.PAX_FORMAT,
                     ) as tf:
                         tf.add(tf_dir, recursive=True)
                         pkginfo_path = Path(installdir) / tf_dir / 'PKG-INFO'
                         with open(pkginfo_path, mode='w') as fpkginfo:
                             fpkginfo.write(pkg_info)
                             fpkginfo.flush()
                             tf.add(Path(tf_dir) / 'PKG-INFO')
```

### Comparing `OZI.build-0.0.3/ozi_build/pep425tags.py` & `OZI.build-0.0.4/ozi_build/pep425tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,17 @@
     impl = get_abbr_impl()
     if not soabi and impl in ("cp", "pp") and hasattr(sys, "maxunicode"):
         d = ""
         m = ""
         u = ""
 
         precond = impl == "cp"
-        if get_flag("Py_DEBUG", hasattr(sys, "gettotalrefcount"), warn=precond):
+        if get_flag(
+            "Py_DEBUG", hasattr(sys, "gettotalrefcount"), warn=precond
+        ):
             d = "d"
 
         precond = impl == "cp" and sys.version_info < (3, 3)
         if sys.version_info < (3, 8) and get_flag(
             "WITH_PYMALLOC", (impl == "cp"), warn=precond
         ):
             m = "m"
```

### Comparing `OZI.build-0.0.3/ozi_build/schema.py` & `OZI.build-0.0.4/ozi_build/schema.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.3/pyproject.toml` & `OZI.build-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     'tomli>=2.0.0;python_version<"3.11"',
     "setuptools>=64",
 ]
 backend-path = [".", "ozi_build"]
 build-backend = "ozi_build.buildapi"
 
 [tool.ozi-build.metadata]
+meson-python-option-name=true
 author="Thibault Saunier"
 author-email="tsaunier@gnome.org"
 maintainer="Eden Rose Duff MSc"
 maintainer-email="help@oziproject.dev"
 summary="Create pep517 compliant packages from the meson build system, OZI-maintained fork."
 home-page="https://github.com/OZI-Project/OZI.build"
 description-file="README.rst"
```

### Comparing `OZI.build-0.0.3/PKG-INFO` & `OZI.build-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OZI.build
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create pep517 compliant packages from the meson build system, OZI-maintained fork.
 Home-page: https://github.com/OZI-Project/OZI.build
 Author: Thibault Saunier
 Author-email: tsaunier@gnome.org
 Maintainer: Eden Rose Duff MSc
 Maintainer-email: help@oziproject.dev
 Requires-Dist: wheel>0.33
```

