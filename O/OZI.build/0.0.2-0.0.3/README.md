# Comparing `tmp/OZI.build-0.0.2.tar.gz` & `tmp/OZI.build-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI.build-0.0.2.tar", last modified: Wed May  1 02:34:39 2024, max compression
+gzip compressed data, was "OZI.build-0.0.3.tar", last modified: Wed May  1 04:03:10 2024, max compression
```

## Comparing `OZI.build-0.0.2.tar` & `OZI.build-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 02:34:39.867702 OZI.build-0.0.2/
--rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 02:26:23.000000 OZI.build-0.0.2/.gitignore
--rw-rw-r--   0 ross      (1000) ross      (1000)      422 2024-05-01 02:26:23.000000 OZI.build-0.0.2/.gitlab-ci.yml
--rw-rw-r--   0 ross      (1000) ross      (1000)    11359 2024-05-01 02:26:23.000000 OZI.build-0.0.2/COPYING
--rw-rw-r--   0 ross      (1000) ross      (1000)      482 2024-05-01 02:26:23.000000 OZI.build-0.0.2/README.rst
--rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 02:26:23.000000 OZI.build-0.0.2/__init__.py
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 02:34:39.867702 OZI.build-0.0.2/doc/
--rwxrwxr-x   0 ross      (1000) ross      (1000)      650 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/generate_doc.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1105 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/index.md
--rw-rw-r--   0 ross      (1000) ross      (1000)      623 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     3388 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/pyproject-gen.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     4171 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/pyproject.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     1339 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/pyproject.md.in
--rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 02:26:23.000000 OZI.build-0.0.2/doc/sitemap.txt
--rw-rw-r--   0 ross      (1000) ross      (1000)      164 2024-05-01 02:26:23.000000 OZI.build-0.0.2/meson.build
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 02:34:39.867702 OZI.build-0.0.2/ozi_build/
--rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 02:26:23.000000 OZI.build-0.0.2/ozi_build/__init__.py
--rw-rw-r--   0 ross      (1000) ross      (1000)    14042 2024-05-01 02:26:23.000000 OZI.build-0.0.2/ozi_build/buildapi.py
--rw-rw-r--   0 ross      (1000) ross      (1000)      230 2024-05-01 02:26:23.000000 OZI.build-0.0.2/ozi_build/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     4275 2024-05-01 02:26:23.000000 OZI.build-0.0.2/ozi_build/pep425tags.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     3540 2024-05-01 02:26:23.000000 OZI.build-0.0.2/ozi_build/schema.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1080 2024-05-01 02:26:23.000000 OZI.build-0.0.2/pyproject.toml
--rwxrwxr-x   0 ross      (1000) ross      (1000)       73 2024-05-01 02:26:23.000000 OZI.build-0.0.2/release
--rw-rw-r--   0 ross      (1000) ross      (1000)     1353 2024-05-01 02:34:39.875702 OZI.build-0.0.2/PKG-INFO
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 04:03:10.665827 OZI.build-0.0.3/
+-rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 04:01:24.000000 OZI.build-0.0.3/.gitignore
+-rw-rw-r--   0 ross      (1000) ross      (1000)      422 2024-05-01 04:01:24.000000 OZI.build-0.0.3/.gitlab-ci.yml
+-rw-rw-r--   0 ross      (1000) ross      (1000)    11359 2024-05-01 04:01:24.000000 OZI.build-0.0.3/COPYING
+-rw-rw-r--   0 ross      (1000) ross      (1000)      482 2024-05-01 04:01:24.000000 OZI.build-0.0.3/README.rst
+-rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 04:01:24.000000 OZI.build-0.0.3/__init__.py
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 04:03:10.665827 OZI.build-0.0.3/doc/
+-rwxrwxr-x   0 ross      (1000) ross      (1000)      651 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/generate_doc.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1105 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/index.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)      623 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3388 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/pyproject-gen.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4171 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/pyproject.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1339 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/pyproject.md.in
+-rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 04:01:24.000000 OZI.build-0.0.3/doc/sitemap.txt
+-rw-rw-r--   0 ross      (1000) ross      (1000)      164 2024-05-01 04:01:24.000000 OZI.build-0.0.3/meson.build
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 04:03:10.665827 OZI.build-0.0.3/ozi_build/
+-rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 04:01:24.000000 OZI.build-0.0.3/ozi_build/__init__.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)    14363 2024-05-01 04:01:24.000000 OZI.build-0.0.3/ozi_build/buildapi.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)      230 2024-05-01 04:01:24.000000 OZI.build-0.0.3/ozi_build/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4275 2024-05-01 04:01:24.000000 OZI.build-0.0.3/ozi_build/pep425tags.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3509 2024-05-01 04:01:24.000000 OZI.build-0.0.3/ozi_build/schema.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1102 2024-05-01 04:01:24.000000 OZI.build-0.0.3/pyproject.toml
+-rwxrwxr-x   0 ross      (1000) ross      (1000)       73 2024-05-01 04:01:24.000000 OZI.build-0.0.3/release
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1353 2024-05-01 04:03:10.673827 OZI.build-0.0.3/PKG-INFO
```

### Comparing `OZI.build-0.0.2/COPYING` & `OZI.build-0.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.2/doc/generate_doc.py` & `OZI.build-0.0.3/doc/generate_doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import sys
 
 sys.path.insert(0, os.path.join(os.path.dirname(__file__), '..'))
 
 from mesonpep517 import schema
 
+
 def generate_doc():
     fields_desc = ""
     for option, desc in schema.VALID_OPTIONS.items():
         fields_desc += "### `%s`" % option
         if desc.get("optional"):
             fields_desc += " (Optional)"
         fields_desc += "\n\n"
```

### Comparing `OZI.build-0.0.2/doc/index.md` & `OZI.build-0.0.3/doc/index.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.2/doc/meson.build` & `OZI.build-0.0.3/doc/meson.build`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.2/doc/pyproject-gen.md` & `OZI.build-0.0.3/doc/pyproject-gen.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.2/doc/pyproject.md` & `OZI.build-0.0.3/doc/pyproject.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.2/doc/pyproject.md.in` & `OZI.build-0.0.3/doc/pyproject.md.in`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.2/ozi_build/buildapi.py` & `OZI.build-0.0.3/ozi_build/buildapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """PEP-517 compliant buildsystem API"""
+
 import contextlib
-import sysconfig
+import json
 import logging
-import sys
-import tempfile
-import tarfile
 import os
-import json
 import subprocess
-
+import sys
+import sysconfig
+import tarfile
+import tempfile
 from gzip import GzipFile
 from pathlib import Path
+
 from wheel.wheelfile import WheelFile
 
 if sys.version_info >= (3, 11):
     import tomllib as toml
 elif sys.version_info < (3, 11):
     import tomli as toml
 
-from .pep425tags import get_abbr_impl, get_abi_tag, get_impl_ver, get_platform_tag
+from .pep425tags import get_abbr_impl
+from .pep425tags import get_abi_tag
+from .pep425tags import get_impl_ver
+from .pep425tags import get_platform_tag
 from .schema import VALID_OPTIONS
+
 log = logging.getLogger(__name__)
 
 
 def meson(*args, config_settings=None, builddir=''):
     try:
         return subprocess.check_output(['meson'] + list(args))
     except subprocess.CalledProcessError as e:
@@ -42,16 +47,16 @@
             print("Could not open %s" % fulllog)
             pass
         raise e
 
 
 def meson_configure(*args, config_settings=None):
     if 'MESON_ARGS' in os.environ:
-       args = os.environ.get('MESON_ARGS').split(' ') + list(args)
-       print("USING MESON_ARGS: %s" % args)
+        args = os.environ.get('MESON_ARGS').split(' ') + list(args)
+        print("USING MESON_ARGS: %s" % args)
     args = list(args)
     args.append('-Dlibdir=lib')
 
     meson(*args, builddir=args[0], config_settings=config_settings)
 
 
 PKG_INFO = """\
@@ -82,24 +87,33 @@
 
     def validate_options(self):
         options = VALID_OPTIONS.copy()
         options['version'] = {}
         options['module'] = {}
         for field, value in self.__metadata.items():
             if field not in options:
-                raise RuntimeError("%s is not a valid option in the `[tool.ozi-build.metadata]` section, "
-                    "got value: %s" % (field, value))
+                raise RuntimeError(
+                    "%s is not a valid option in the `[tool.ozi-build.metadata]` section, "
+                    "got value: %s" % (field, value)
+                )
             del options[field]
 
         for field, desc in options.items():
             if desc.get('required'):
-                raise RuntimeError("%s is mandatory in the `[tool.ozi-build.metadata] section but was not found" % field)
+                raise RuntimeError(
+                    "%s is mandatory in the `[tool.ozi-build.metadata] section but was not found"
+                    % field
+                )
 
     def __introspect(self, introspect_type):
-        with open(os.path.join(self.__builddir, 'meson-info', 'intro-' + introspect_type + '.json')) as f:
+        with open(
+            os.path.join(
+                self.__builddir, 'meson-info', 'intro-' + introspect_type + '.json'
+            )
+        ) as f:
             return json.load(f)
 
     def set_builddir(self, builddir):
         self.__builddir = builddir
         project = self.__introspect('projectinfo')
 
         self['version'] = project['version']
@@ -120,18 +134,20 @@
         return key in self.__metadata
 
     @staticmethod
     def __get_config():
         with open('pyproject.toml', 'rb') as f:
             config = toml.load(f)
             try:
-                metadata = config['tool']['ozi-build']['metadata']
+                config['tool']['ozi-build']['metadata']
             except KeyError:
-                raise RuntimeError("`[tool.ozi-build.metadata]` section is mandatory "
-                    "for the meson backend")
+                raise RuntimeError(
+                    "`[tool.ozi-build.metadata]` section is mandatory "
+                    "for the meson backend"
+                )
 
             return config
 
     def get(self, key, default=None):
         return self.__metadata.get(key, default)
 
     def get_metadata(self):
@@ -140,53 +156,57 @@
             'version': self['version'],
         }
 
         if 'pkg-info-file' in self:
             res = '\n'.join(PKG_INFO.split('\n')[:3]).format(**meta) + '\n'
             with open(self['pkg-info-file'], 'r') as f:
                 orig_lines = f.readlines()
-                for l in orig_lines:
-                    if l.startswith('Metadata-Version:') or \
-                            l.startswith('Version:'):
+                for line in orig_lines:
+                    if line.startswith('Metadata-Version:') or line.startswith(
+                        'Version:'
+                    ):
                         continue
-                    res += l
+                    res += line
 
-            return  res
+            return res
 
         res = PKG_INFO.format(**meta)
 
         for key in [
-                'summary',
-                'home-page',
-                'author',
-                'author-email',
-                'maintainer',
-                'maintainer-email',
-                'license']:
+            'summary',
+            'home-page',
+            'author',
+            'author-email',
+            'maintainer',
+            'maintainer-email',
+            'license',
+        ]:
             if key in self:
                 res += '{}: {}\n'.format(key.capitalize(), self[key])
 
         for key, mdata_key in [
-                ('requires', 'Requires-Dist'),
-                ('classifiers', 'Classifier'),
-                ('project-urls', 'Project-URL')]:
+            ('requires', 'Requires-Dist'),
+            ('classifiers', 'Classifier'),
+            ('project-urls', 'Project-URL'),
+        ]:
 
             vals = self.get(key, [])
             for val in vals:
                 res += '{}: {}\n'.format(mdata_key, val)
 
         description = ''
         description_content_type = 'text/plain'
         if 'description-file' in self:
             description_file = Path(self['description-file'])
             with open(description_file, 'r') as f:
                 description = f.read()
 
             description_content_type = readme_ext_to_content_type.get(
-                description_file.suffix.lower(), description_content_type)
+                description_file.suffix.lower(), description_content_type
+            )
         elif 'description' in self:
             description = self['description']
 
         if description:
             res += 'Description-Content-Type: {}\n'.format(description_content_type)
             res += 'Description:\n\n' + description
 
@@ -234,51 +254,50 @@
 def _write_wheel_file(f, supports_py2, is_pure):
     f.write(wheel_file_template.format(str(is_pure).lower()))
     if is_pure:
         if supports_py2:
             f.write("Tag: py2-none-any\n")
         f.write("Tag: py3-none-any\n")
     else:
-        f.write("Tag: {0}{1}-{2}-{3}\n".format(
-            get_abbr_impl(),
-            get_impl_ver(),
-            get_abi_tag(),
-            get_platform_tag()
-        ))
+        f.write(
+            "Tag: {0}{1}-{2}-{3}\n".format(
+                get_abbr_impl(), get_impl_ver(), get_abi_tag(), get_platform_tag()
+            )
+        )
 
 
 def check_is_pure(installed):
     variables = sysconfig.get_config_vars()
-    suffix = variables.get('EXT_SUFFIX') or variables.get(
-        'SO') or variables.get('.so')
+    suffix = variables.get('EXT_SUFFIX') or variables.get('SO') or variables.get('.so')
     # msys2's python3 has "-cpython-36m.dll", we have to be clever
     split = suffix.rsplit('.', 1)
     suffix = split.pop(-1)
 
     for installpath in installed.values():
         if "site-packages" in installpath:
             if installpath.split('.')[-1] == suffix:
                 return False
 
     return True
 
 
-def prepare_metadata_for_build_wheel(metadata_directory,
-                                     config_settings=None,
-                                     builddir=None,
-                                     config=None):
+def prepare_metadata_for_build_wheel(
+    metadata_directory, config_settings=None, builddir=None, config=None
+):
     """Creates {metadata_directory}/foo-1.2.dist-info"""
     if not builddir:
         builddir = tempfile.TemporaryDirectory().name
         meson_configure(builddir, config_settings=config_settings)
     if not config:
         config = Config(builddir)
 
-    dist_info = Path(metadata_directory, '{}-{}.dist-info'.format(
-                     config['module'], config['version']))
+    dist_info = Path(
+        metadata_directory,
+        '{}-{}.dist-info'.format(config['module'], config['version']),
+    )
     dist_info.mkdir(exist_ok=True)
 
     is_pure = check_is_pure(config.installed)
     with (dist_info / 'WHEEL').open('w') as f:
         _write_wheel_file(f, False, is_pure)
 
     with (dist_info / 'METADATA').open('w') as f:
@@ -298,63 +317,72 @@
                           pep425tags.get_impl_ver(),
                           pep425tags.get_abi_tag())
 )
 """
 
 
 def get_abi(python):
-    return subprocess.check_output([python, '-c', GET_CHECK]).decode('utf-8').strip('\n')
+    return (
+        subprocess.check_output([python, '-c', GET_CHECK]).decode('utf-8').strip('\n')
+    )
 
 
 class WheelBuilder:
     def __init__(self):
-        self.wheel_zip = None
+        self.wheel_zip = None  # type: ignore
         self.builddir = tempfile.TemporaryDirectory()
         self.installdir = tempfile.TemporaryDirectory()
 
     def build(self, wheel_directory, config_settings, metadata_dir):
         config = Config()
 
-        args = [self.builddir.name, '--prefix', self.installdir.name] + config.get('meson-options', [])
+        args = [self.builddir.name, '--prefix', self.installdir.name] + config.get(
+            'meson-options', []
+        )
         meson_configure(*args, config_settings=config_settings)
         config.set_builddir(self.builddir.name)
 
         metadata_dir = prepare_metadata_for_build_wheel(
-            wheel_directory, builddir=self.builddir.name,
-            config=config)
+            wheel_directory, builddir=self.builddir.name, config=config
+        )
 
         is_pure = check_is_pure(config.installed)
-        platform_tag = config.get(
-            'platforms',
-            'any' if is_pure else get_platform_tag()
-        )
+        platform_tag = config.get('platforms', 'any' if is_pure else get_platform_tag())
 
         if not is_pure:
             python = 'python3'
             option_build = config.get('meson-python-option-name')
             if not option_build:
                 python = 'python3'
-                log.warning("meson-python-option-name not specified in the " +
-                    "[tool.mesonpep517.metadata] section, assuming `python3`")
+                log.warning(
+                    "meson-python-option-name not specified in the "
+                    + "[tool.ozi-build.metadata] section, assuming `python3`"
+                )
             else:
                 for opt in config.options:
                     if opt['name'] == 'python_version':
                         python = opt['value']
                         break
             abi = get_abi(python)
         else:
-            abi = '{}-none'.format(config.get('requires-python', 'py3'))
+            abi = '{}-none'.format(config.get('requires-python', f'py3{sys.version_info[1]}'))
 
         target_fp = wheel_directory / '{}-{}-{}-{}.whl'.format(
-            config['module'], config['version'], abi, platform_tag,)
+            config['module'],
+            config['version'],
+            abi,
+            platform_tag,
+        )
 
-        self.wheel_zip = WheelFile(str(target_fp), 'w')
+        self.wheel_zip: WheelFile = WheelFile(str(target_fp), 'w')
         for f in os.listdir(str(wheel_directory / metadata_dir)):
-            self.wheel_zip.write(str(wheel_directory / metadata_dir / f),
-                arcname=str(Path(metadata_dir) / f))
+            self.wheel_zip.write(
+                str(wheel_directory / metadata_dir / f),
+                arcname=str(Path(metadata_dir) / f),
+            )
 
         # Make sure everything is built
         meson('install', '-C', self.builddir.name)
         self.pack_files(config)
         self.wheel_zip.close()
         return str(target_fp)
 
@@ -368,53 +396,57 @@
             elif "dist-packages" in installpath:
                 while os.path.basename(installpath) != 'dist-packages':
                     installpath = os.path.dirname(installpath)
                 self.wheel_zip.write_files(installpath)
                 break
 
 
-def build_wheel(wheel_directory,
-                config_settings=None,
-                metadata_directory=None):
+def build_wheel(wheel_directory, config_settings=None, metadata_directory=None):
     """Builds a wheel, places it in wheel_directory"""
-    return WheelBuilder().build(Path(
-        wheel_directory), config_settings, metadata_directory)
+    return WheelBuilder().build(
+        Path(wheel_directory), config_settings, metadata_directory
+    )
 
 
 def build_sdist(sdist_directory, config_settings=None):
     """Builds an sdist, places it in sdist_directory"""
     distdir = Path(sdist_directory)
     with tempfile.TemporaryDirectory() as builddir:
         with tempfile.TemporaryDirectory() as installdir:
-            meson(builddir, '--prefix', installdir,
-                  config_settings=config_settings,
-                  builddir=builddir)
+            meson(
+                builddir,
+                '--prefix',
+                installdir,
+                config_settings=config_settings,
+                builddir=builddir,
+            )
 
             config = Config(builddir)
             meson('dist', '-C', builddir)
 
             tf_dir = '{}-{}'.format(config['module'], config['version'])
             mesondistfilename = '%s.tar.xz' % tf_dir
             mesondisttar = tarfile.open(
-                Path(builddir) / 'meson-dist' / mesondistfilename)
+                Path(builddir) / 'meson-dist' / mesondistfilename
+            )
             for entry in mesondisttar:
-                #GOOD: Check that entry is safe
+                # GOOD: Check that entry is safe
                 if os.path.isabs(entry.name) or ".." in entry.name:
                     raise ValueError("Illegal tar archive entry")
                 mesondisttar.extract(entry, installdir)
             pkg_info = config.get_metadata()
             distfilename = '%s.tar.gz' % tf_dir
             target = distdir / distfilename
             source_date_epoch = os.environ.get('SOURCE_DATE_EPOCH', '')
             mtime = int(source_date_epoch) if source_date_epoch else None
             with GzipFile(str(target), mode='wb', mtime=mtime) as gz:
                 with cd(installdir):
-                    with tarfile.TarFile(str(target), mode='w',
-                                         fileobj=gz,
-                                         format=tarfile.PAX_FORMAT) as tf:
+                    with tarfile.TarFile(
+                        str(target), mode='w', fileobj=gz, format=tarfile.PAX_FORMAT
+                    ) as tf:
                         tf.add(tf_dir, recursive=True)
                         pkginfo_path = Path(installdir) / tf_dir / 'PKG-INFO'
                         with open(pkginfo_path, mode='w') as fpkginfo:
                             fpkginfo.write(pkg_info)
                             fpkginfo.flush()
                             tf.add(Path(tf_dir) / 'PKG-INFO')
     return target.name
```

### Comparing `OZI.build-0.0.2/ozi_build/pep425tags.py` & `OZI.build-0.0.3/ozi_build/pep425tags.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.2/ozi_build/schema.py` & `OZI.build-0.0.3/ozi_build/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,124 +1,104 @@
 VALID_OPTIONS = {
-    "author": {
-        "description": "Your name"
-    },
-
+    "author": {"description": "Your name"},
     "author-email": {
         "description": """Your email address
 
 e.g. for ozi-build itself:
 
 ``` toml
 [tool.ozi-build.metadata]
 author="Thibault Saunier"
 author-email="tsaunier@gnome.org"
 ```"""
     },
-
     "classifiers": {
         "description": "A list of [classifiers](https://pypi.python.org/pypi?%3Aaction=list_classifiers)."
     },
-
     "description": {
         "description": "The description of the project as a string if you do not want to specify 'description-file'"
     },
-
     "description-file": {
         "description": """A path (relative to the .toml file) to a file containing a longer description
 of your package to show on PyPI. This should be written in reStructuredText
   Markdown or plain text, and the filename should have the appropriate extension
   (`.rst`, `.md` or `.txt`)."""
     },
-
     "home-page": {
         "description": """A string containing the URL for the package's home page.
 
 Example:
 
 `http://www.example.com/~cschultz/bvote/`"""
     },
-
     "license": {
         "description": """Text indicating the license covering the distribution. This text can be either a valid license expression as defined in [pep639](https://www.python.org/dev/peps/pep-0639/#id88) or any free text."""
     },
-
     "maintainer": {
         "description": "Name of current maintainer of the project (if different from author)"
     },
-
     "maintainer-email": {
         "description": """Maintainer email address
 
 Example:
 
 ``` toml
 [tool.ozi-build.metadata]
 maintainer="Robin Goode"
 maintainer-email="rgoode@example.org"
 ```"""
     },
-
     "meson-options": {
         "description": """A list of default meson options to set, can be overriden and expended through the `MESON_ARGS`
 environement variable at build time."""
     },
-
     "meson-python-option-name": {
         "description": """The name of the meson options that is used in the meson build definition
 to set the python installation when using
 [`python.find_installation()`](http://mesonbuild.com/Python-module.html#find_installation)."""
     },
-
     "module": {
         "description": "The name of the module, will use the meson project name if not specified"
     },
-
     "pkg-info-file": {
         "description": """Pass a PKG-INFO file direcly usable.
 
 > ! NOTE: All other keys will be ignored if you pass an already prepared `PKG-INFO`
 > file
 """
     },
-
     "platforms": {
         "description": "Supported Python platforms, can be 'any', py3, etc..."
     },
-
     "project-urls": {
         "description": """A list of `Type, url` as described in the
 [pep345](https://www.python.org/dev/peps/pep-0345/#project-url-multiple-use).
 For example:
 
 ``` toml
 project-urls = [
     "Source, https://gitlab.com/OZI-Project/OZI.build",
 ]
 ```"""
     },
-
     "requires": {
         "description": """A list of other packages from PyPI that this package needs. Each package may
 be followed by a version specifier like ``(>=4.1)`` or ``>=4.1``, and/or an
 [environment marker](https://www.python.org/dev/peps/pep-0345/#environment-markers)
 after a semicolon. For example:
 
 ``` toml
       requires = [
           "requests >=2.6",
           "configparser; python_version == '2.7'",
       ]
 ```"""
     },
-
     "requires-python": {
         "description": """A version specifier for the versions of Python this requires, e.g. ``~=3.3`` or
 ``>=3.3,<4`` which are equivalents."""
     },
-
     "summary": {
         "required": True,
-        "description": "A one sentence summary about the package"
+        "description": "A one sentence summary about the package",
     },
-
 }
```

### Comparing `OZI.build-0.0.2/pyproject.toml` & `OZI.build-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 description-file="README.rst"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
+requires-python="py3"
 requires = ["wheel>0.33", "meson[ninja]>1.1.0", 'tomli>=2.0.0;python_version<"3.11"', "setuptools"]
 project-urls= [
     "Source, https://github.com/OZI-Project/OZI.build",
     "Documentation, https://thiblahute.gitlab.io/mesonpep517/",
 ]
 
 [tool.setuptools.packages.find]
```

### Comparing `OZI.build-0.0.2/PKG-INFO` & `OZI.build-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OZI.build
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create pep517 compliant packages from the meson build system, OZI-maintained fork.
 Home-page: https://github.com/OZI-Project/OZI.build
 Author: Thibault Saunier
 Author-email: tsaunier@gnome.org
 Maintainer: Eden Rose Duff MSc
 Maintainer-email: help@oziproject.dev
 Requires-Dist: wheel>0.33
```

