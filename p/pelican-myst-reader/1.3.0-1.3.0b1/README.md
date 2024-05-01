# Comparing `tmp/pelican_myst_reader-1.3.0.tar.gz` & `tmp/pelican_myst_reader-1.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_myst_reader-1.3.0.tar", max compression
+gzip compressed data, was "pelican_myst_reader-1.3.0b1.tar", max compression
```

## Comparing `pelican_myst_reader-1.3.0.tar` & `pelican_myst_reader-1.3.0b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    34523 2024-05-01 11:17:35.876897 pelican_myst_reader-1.3.0/LICENSE
--rw-r--r--   0        0        0     9905 2024-05-01 11:17:35.876897 pelican_myst_reader-1.3.0/README.md
--rw-r--r--   0        0        0       73 2024-05-01 11:17:35.876897 pelican_myst_reader-1.3.0/pelican/plugins/myst_reader/__init__.py
--rw-r--r--   0        0        0      654 2024-05-01 11:17:35.876897 pelican_myst_reader-1.3.0/pelican/plugins/myst_reader/_docutils_renderer.py
--rw-r--r--   0        0        0     2373 2024-05-01 11:17:35.876897 pelican_myst_reader-1.3.0/pelican/plugins/myst_reader/_sphinx_renderer.py
--rw-r--r--   0        0        0      107 2024-05-01 11:17:35.876897 pelican_myst_reader-1.3.0/pelican/plugins/myst_reader/exceptions.py
--rw-r--r--   0        0        0    14255 2024-05-01 11:17:35.876897 pelican_myst_reader-1.3.0/pelican/plugins/myst_reader/myst_reader.py
--rw-r--r--   0        0        0     2400 2024-05-01 11:17:35.876897 pelican_myst_reader-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    11618 1970-01-01 00:00:00.000000 pelican_myst_reader-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-02 11:46:22.218201 pelican_myst_reader-1.3.0b1/LICENSE
+-rw-r--r--   0        0        0     9819 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/README.md
+-rw-r--r--   0        0        0       72 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/pelican/plugins/myst_reader/__init__.py
+-rw-r--r--   0        0        0      654 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/pelican/plugins/myst_reader/_docutils_renderer.py
+-rw-r--r--   0        0        0     2373 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/pelican/plugins/myst_reader/_sphinx_renderer.py
+-rw-r--r--   0        0        0      107 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/pelican/plugins/myst_reader/exceptions.py
+-rw-r--r--   0        0        0    14245 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/pelican/plugins/myst_reader/myst_reader.py
+-rw-r--r--   0        0        0     2361 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/pyproject.toml
+-rw-r--r--   0        0        0    11470 1970-01-01 00:00:00.000000 pelican_myst_reader-1.3.0b1/PKG-INFO
```

### Comparing `pelican_myst_reader-1.3.0/LICENSE` & `pelican_myst_reader-1.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_myst_reader-1.3.0/README.md` & `pelican_myst_reader-1.3.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -201,19 +201,15 @@
 
 ## Contributing
 
 Contributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].
 
 To start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.
 
-Special thanks to
-- [Kevin Deldycke](https://kevin.deldycke.com/)
-- [Pierre Augier](http://legi.grenoble-inp.fr/people/Pierre.Augier/)
-
-for their improvements and feedback on this plugin. Kudos to the [pelican-pandoc-reader](https://pypi.org/project/pelican-pandoc-reader/) plugin which provided the foundation to build this plugin on.
+Special thanks to [Justin Mayer](https://justinmayer.com), [Erwin Janssen](https://github.com/ErwinJanssen), [Joseph Reagle](https://github.com/reagle) and [Deniz Turgut](https://github.com/avaris) for their improvements and feedback on this plugin.
 
 [existing issues]: https://github.com/ashwinvis/myst-reader/issues
 [Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html
 
 ## License
 
 This project is licensed under the AGPL-3.0 license.
```

### Comparing `pelican_myst_reader-1.3.0/pelican/plugins/myst_reader/_docutils_renderer.py` & `pelican_myst_reader-1.3.0b1/pelican/plugins/myst_reader/_docutils_renderer.py`

 * *Files identical despite different names*

### Comparing `pelican_myst_reader-1.3.0/pelican/plugins/myst_reader/_sphinx_renderer.py` & `pelican_myst_reader-1.3.0b1/pelican/plugins/myst_reader/_sphinx_renderer.py`

 * *Files identical despite different names*

### Comparing `pelican_myst_reader-1.3.0/pelican/plugins/myst_reader/myst_reader.py` & `pelican_myst_reader-1.3.0b1/pelican/plugins/myst_reader/myst_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Reader that processes MyST Markdown and returns HTML5."""
-
 from __future__ import annotations
 
 from copy import deepcopy
 from enum import Enum
 from io import StringIO
 import math
 import os
@@ -359,15 +358,15 @@
                         conf=self.docutils_settings,
                         parser=self.docutils_parser,
                     ),
                     RENDERER.DOCUTILS,
                 )
             except docutils.utils.SystemMessage as err:
                 raise MystReaderContentError(
-                    f"Malformed content or front-matter metadata:\n{err}"
+                    "Malformed content or front-matter metadata"
                 ) from err
 
     @staticmethod
     def _find_bibs(source_path: str) -> list[str]:
         """Find bibliographies recursively in the sourcepath given."""
         bib_files = []
         filename = os.path.splitext(os.path.basename(source_path))[0]
```

### Comparing `pelican_myst_reader-1.3.0/pyproject.toml` & `pelican_myst_reader-1.3.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "pelican-myst-reader"
-version = "1.3.0"
+version = "1.3.0b1"
 description = "Pelican plugin for converting MyST's Markdown variant to HTML."
 authors = ["Ashwin Vishnu <dev@fluid.quest>"]
 license = "AGPL-3.0"
 readme = "README.md"
 keywords = ["pelican", "plugin", "markdown", "myst"]
 repository = "https://github.com/ashwinvis/myst-reader"
 documentation = "https://docs.getpelican.com"
 packages = [
     { include = "pelican" },
 ]
 
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Framework :: Pelican",
     "Framework :: Pelican :: Plugins",
     "Intended Audience :: End Users/Desktop",
     "Operating System :: OS Independent",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -35,19 +35,18 @@
 beautifulsoup4 = "^4.9.3"
 myst-parser = "^2.0.0"
 docutils = ">=0.17"
 sphinxcontrib-bibtex = "~2.5.0"
 pyyaml = "^6.0"
 
 [tool.poetry.group.tests.dependencies]
-pytest = "^7.0"
+pytest = "^6.0"
 pytest-cov = "^2.8"
 pytest-pythonpath = "^0.7.3"
 pytest-sugar = "^0.9.4"
-pytest-subtests = "^0.12.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.8.0"
 flake8 = "^3.9.2"
 flake8-black = "^0.2.0"
 invoke = "^1.3"
 isort = "^5.8.0"
```

### Comparing `pelican_myst_reader-1.3.0/PKG-INFO` & `pelican_myst_reader-1.3.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: pelican-myst-reader
-Version: 1.3.0
+Version: 1.3.0b1
 Summary: Pelican plugin for converting MyST's Markdown variant to HTML.
 Home-page: https://github.com/ashwinvis/myst-reader
 License: AGPL-3.0
 Keywords: pelican,plugin,markdown,myst
 Author: Ashwin Vishnu
 Author-email: dev@fluid.quest
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: markdown
 Requires-Dist: beautifulsoup4 (>=4.9.3,<5.0.0)
 Requires-Dist: docutils (>=0.17)
 Requires-Dist: markdown (>=3.2.2,<4.0.0) ; extra == "markdown"
 Requires-Dist: markdown-word-count (>=0.0.1,<0.0.2)
@@ -240,19 +239,15 @@
 
 ## Contributing
 
 Contributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].
 
 To start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.
 
-Special thanks to
-- [Kevin Deldycke](https://kevin.deldycke.com/)
-- [Pierre Augier](http://legi.grenoble-inp.fr/people/Pierre.Augier/)
-
-for their improvements and feedback on this plugin. Kudos to the [pelican-pandoc-reader](https://pypi.org/project/pelican-pandoc-reader/) plugin which provided the foundation to build this plugin on.
+Special thanks to [Justin Mayer](https://justinmayer.com), [Erwin Janssen](https://github.com/ErwinJanssen), [Joseph Reagle](https://github.com/reagle) and [Deniz Turgut](https://github.com/avaris) for their improvements and feedback on this plugin.
 
 [existing issues]: https://github.com/ashwinvis/myst-reader/issues
 [Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html
 
 ## License
 
 This project is licensed under the AGPL-3.0 license.
```

