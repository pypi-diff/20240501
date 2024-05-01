# Comparing `tmp/sphinxnotes-isso-1.0a2.tar.gz` & `tmp/sphinxnotes_isso-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxnotes-isso-1.0a2.tar", last modified: Tue Mar 23 04:27:12 2021, max compression
+gzip compressed data, was "sphinxnotes_isso-1.1.tar", last modified: Wed May  1 05:20:27 2024, max compression
```

## Comparing `sphinxnotes-isso-1.0a2.tar` & `sphinxnotes_isso-1.1.tar`

### file list

```diff
@@ -1,29 +1,44 @@
-drwxr-xr-x   0 la        (1000) users      (100)        0 2021-03-23 04:27:12.592874 sphinxnotes-isso-1.0a2/
--rw-r--r--   0 la        (1000) users      (100)     1520 2021-03-04 03:41:11.000000 sphinxnotes-isso-1.0a2/LICENSE
--rw-r--r--   0 la        (1000) users      (100)       76 2021-03-04 03:35:18.000000 sphinxnotes-isso-1.0a2/MANIFEST.in
--rw-r--r--   0 la        (1000) users      (100)     1251 2021-03-23 04:27:12.592874 sphinxnotes-isso-1.0a2/PKG-INFO
--rw-r--r--   0 la        (1000) users      (100)      296 2021-03-04 03:51:45.000000 sphinxnotes-isso-1.0a2/README.rst
-drwxr-xr-x   0 la        (1000) users      (100)        0 2021-03-23 04:27:12.592874 sphinxnotes-isso-1.0a2/doc/
--rw-r--r--   0 la        (1000) users      (100)      657 2021-03-04 03:35:18.000000 sphinxnotes-isso-1.0a2/doc/Makefile
-drwxr-xr-x   0 la        (1000) users      (100)        0 2021-03-23 04:27:12.592874 sphinxnotes-isso-1.0a2/doc/__pycache__/
--rw-r--r--   0 la        (1000) users      (100)      815 2021-03-04 03:35:18.000000 sphinxnotes-isso-1.0a2/doc/__pycache__/project.cpython-39.pyc
-drwxr-xr-x   0 la        (1000) users      (100)        0 2021-03-23 04:27:12.592874 sphinxnotes-isso-1.0a2/doc/_images/
--rw-r--r--   0 la        (1000) users      (100)    15941 2021-03-04 03:35:18.000000 sphinxnotes-isso-1.0a2/doc/_images/sphinx-notes.png
--rw-r--r--   0 la        (1000) users      (100)     2774 2021-03-13 09:07:52.000000 sphinxnotes-isso-1.0a2/doc/conf.py
--rw-r--r--   0 la        (1000) users      (100)     2142 2021-03-23 04:15:07.000000 sphinxnotes-isso-1.0a2/doc/index.rst
--rw-r--r--   0 la        (1000) users      (100)      795 2021-03-04 03:35:18.000000 sphinxnotes-isso-1.0a2/doc/make.bat
--rw-r--r--   0 la        (1000) users      (100)        0 2021-03-04 03:36:33.000000 sphinxnotes-isso-1.0a2/doc/requirements.txt
--rw-r--r--   0 la        (1000) users      (100)       38 2021-03-23 04:27:12.592874 sphinxnotes-isso-1.0a2/setup.cfg
--rw-r--r--   0 la        (1000) users      (100)     1509 2021-03-04 03:42:34.000000 sphinxnotes-isso-1.0a2/setup.py
-drwxr-xr-x   0 la        (1000) users      (100)        0 2021-03-23 04:27:12.589541 sphinxnotes-isso-1.0a2/sphinxnotes/
-drwxr-xr-x   0 la        (1000) users      (100)        0 2021-03-23 04:27:12.592874 sphinxnotes-isso-1.0a2/sphinxnotes/isso/
--rw-r--r--   0 la        (1000) users      (100)     4012 2021-03-23 04:15:48.000000 sphinxnotes-isso-1.0a2/sphinxnotes/isso/__init__.py
-drwxr-xr-x   0 la        (1000) users      (100)        0 2021-03-23 04:27:12.592874 sphinxnotes-isso-1.0a2/sphinxnotes_isso.egg-info/
--rw-r--r--   0 la        (1000) users      (100)     1251 2021-03-23 04:27:12.000000 sphinxnotes-isso-1.0a2/sphinxnotes_isso.egg-info/PKG-INFO
--rw-r--r--   0 la        (1000) users      (100)      539 2021-03-23 04:27:12.000000 sphinxnotes-isso-1.0a2/sphinxnotes_isso.egg-info/SOURCES.txt
--rw-r--r--   0 la        (1000) users      (100)        1 2021-03-23 04:27:12.000000 sphinxnotes-isso-1.0a2/sphinxnotes_isso.egg-info/dependency_links.txt
--rw-r--r--   0 la        (1000) users      (100)       58 2021-03-23 04:27:12.000000 sphinxnotes-isso-1.0a2/sphinxnotes_isso.egg-info/entry_points.txt
--rw-r--r--   0 la        (1000) users      (100)       12 2021-03-23 04:27:12.000000 sphinxnotes-isso-1.0a2/sphinxnotes_isso.egg-info/namespace_packages.txt
--rw-r--r--   0 la        (1000) users      (100)        1 2021-03-23 04:27:12.000000 sphinxnotes-isso-1.0a2/sphinxnotes_isso.egg-info/not-zip-safe
--rw-r--r--   0 la        (1000) users      (100)        7 2021-03-23 04:27:12.000000 sphinxnotes-isso-1.0a2/sphinxnotes_isso.egg-info/requires.txt
--rw-r--r--   0 la        (1000) users      (100)       12 2021-03-23 04:27:12.000000 sphinxnotes-isso-1.0a2/sphinxnotes_isso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:27.729390 sphinxnotes_isso-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:27.721390 sphinxnotes_isso-1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:27.725391 sphinxnotes_isso-1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:27.725391 sphinxnotes_isso-1.1/.sphinxnotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:27.725391 sphinxnotes_isso-1.1/.sphinxnotes/template/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/.sphinxnotes/template/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-01 05:20:27.729390 sphinxnotes_isso-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:27.729390 sphinxnotes_isso-1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:27.729390 sphinxnotes_isso-1.1/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/docs/_images/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:27.729390 sphinxnotes_isso-1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)    15941 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/docs/_static/sphinx-notes.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:27.729390 sphinxnotes_isso-1.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/docs/_templates/confval.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/docs/_templates/example.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/docs/_templates/version.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/docs/conf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 05:20:27.729390 sphinxnotes_isso-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:27.725391 sphinxnotes_isso-1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:27.725391 sphinxnotes_isso-1.1/src/sphinxnotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:27.729390 sphinxnotes_isso-1.1/src/sphinxnotes/isso/
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-01 05:20:19.000000 sphinxnotes_isso-1.1/src/sphinxnotes/isso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:27.729390 sphinxnotes_isso-1.1/src/sphinxnotes_isso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-01 05:20:27.000000 sphinxnotes_isso-1.1/src/sphinxnotes_isso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-01 05:20:27.000000 sphinxnotes_isso-1.1/src/sphinxnotes_isso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:20:27.000000 sphinxnotes_isso-1.1/src/sphinxnotes_isso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-01 05:20:27.000000 sphinxnotes_isso-1.1/src/sphinxnotes_isso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 05:20:27.000000 sphinxnotes_isso-1.1/src/sphinxnotes_isso.egg-info/top_level.txt
```

### Comparing `sphinxnotes-isso-1.0a2/LICENSE` & `sphinxnotes_isso-1.1/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2021, Sphinx Notes
+Copyright (c) 2024, Shengyu Zhang
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
@@ -22,8 +22,8 @@
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `sphinxnotes-isso-1.0a2/doc/Makefile` & `sphinxnotes_isso-1.1/docs/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+# This file is generated from sphinx-notes/cookiecutter.
+# You need to consider modifying the TEMPLATE or modifying THIS FILE.
+
 # Minimal makefile for Sphinx documentation
-#
 
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
+# You can set these variables from the command line.
+SPHINXOPTS    =
+SPHINXBUILD   = python3 -msphinx
 SOURCEDIR     = .
 BUILDDIR      = _build
 
 default: html
 
 # Put it first so that "make" without argument is like "make help".
 help:
```

### Comparing `sphinxnotes-isso-1.0a2/doc/_images/sphinx-notes.png` & `sphinxnotes_isso-1.1/docs/_static/sphinx-notes.png`

 * *Files identical despite different names*

### Comparing `sphinxnotes-isso-1.0a2/sphinxnotes/isso/__init__.py` & `sphinxnotes_isso-1.1/src/sphinxnotes/isso/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,32 +14,35 @@
 import posixpath
 
 from docutils import nodes
 from docutils.parsers.rst import directives, Directive
 
 if TYPE_CHECKING:
     from sphinx.application import Sphinx
+from sphinx.util import logging
 
 __title__= 'sphinxnotes-isso'
-__license__ = 'BSD',
-__version__ = '1.0a2'
+__license__ = 'BSD'
+__version__ = '1.0'
 __author__ = 'Shengyu Zhang'
 __url__ = 'https://sphinx-notes.github.io/isso'
 __description__ = 'Sphinx extension for embeding Isso comments in documents'
 __keywords__ = 'documentation, sphinx, extension, comment, isso, disqus'
 
 # Isso client configuration items
 # https://posativ.org/isso/docs/configuration/client/
 CONFIG_ITEMS = ['isso_css', 'isso_lang', 'isso_reply_to_self',
              'isso_require_author', 'isso_require_email',
              'isso_max_comments_top', 'isso_max_comments_nested',
              'isso_reveal_on_click', 'isso_avatar', 'isso_avatar_bg',
              'isso_avatar_fg', 'isso_vote', 'isso_vote_levels',
              'isso_feed']
 
+logger = logging.getLogger(__name__)
+
 def ext_config_to_isso_config(key:str, value:Any) -> Tuple[str,str]:
     assert key in CONFIG_ITEMS
     key = 'data-' + key.replace('_', '-')
     if isinstance(value, str):
         pass
     elif isinstance(value, bool):
         value = str(value).lower()
@@ -51,41 +54,57 @@
 class IssoNode(nodes.General, nodes.Element):
 
     @staticmethod
     def visit(self, node):
         kwargs = {
             'data-isso-id': node['thread-id'],
         }
+        if node.get('thread-title'):
+            kwargs['data-title'] = node['thread-title']
         self.body.append(self.starttag(node, 'section', '', **kwargs))
 
+
     @staticmethod
     def depart(self, _):
         self.body.append('</section>')
 
 
 class IssoDirective(Directive):
     """Isso ".. isso::" rst directive."""
 
     option_spec = {
-        'id': directives.unchanged
+        'id': directives.unchanged,
+        'title': directives.unchanged,
     }
 
     def run(self):
         """Executed by Sphinx.
         :returns: Single IssoNode instance with config values passed as arguments.
         :rtype: list
         """
 
         node = IssoNode()
         node['ids'] = ['isso-thread']
-        node['thread-id'] = self.options.get('id') or \
-            '/' + self.state.document.settings.env.docname
+        if self.options.get('id'):
+            thread_id = self.options.get('id')
+            if not thread_id.startswith('/'):
+                logger.warning('isso thread-id should starts with slash', location=node)
+            node['thread-id'] = thread_id
+        else:
+            node['thread-id'] = '/' + self.state.document.settings.env.docname
+        if self.options.get('title'):
+            node['thread-title'] = self.options.get('title')
+        else:
+            title = self.state.document.next_node(nodes.title)
+            if title:
+                node['thread-title'] = title.astext()
 
         return [node]
 
+
 def on_html_page_context(app:Sphinx, pagename:str, templatename:str, context,
                          doctree:nodes.document) -> None:
     """Called when the HTML builder has created a context dictionary to render a template with.
 
     Conditionally adding isso client script to <head /> if the directive is used in a page.
 
     :param sphinx.application.Sphinx app: Sphinx application object.
@@ -108,15 +127,15 @@
                 issocfg, issoval = ext_config_to_isso_config(cfg, val)
                 kwargs[issocfg] = issoval
         js_path = posixpath.join(app.config.isso_url, 'js/embed.min.js')
         app.add_js_file(js_path, **kwargs)
 
 
 def setup(app:Sphinx):
-    app.add_config_value('isso_url', None, {})
+    app.add_config_value('isso_url', None, '')
     for cfg in CONFIG_ITEMS:
-        app.add_config_value(cfg, None, {})
+        app.add_config_value(cfg, None, '')
     app.add_directive('isso', IssoDirective)
     app.add_node(IssoNode, html=(IssoNode.visit, IssoNode.depart))
     app.connect('html-page-context', on_html_page_context)
 
     return {'version': __version__}
```

