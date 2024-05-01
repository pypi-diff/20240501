# Comparing `tmp/html_text-0.6.1.tar.gz` & `tmp/html_text-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_text-0.6.1.tar", last modified: Tue Apr 23 12:01:59 2024, max compression
+gzip compressed data, was "html_text-0.6.2.tar", last modified: Wed May  1 11:55:07 2024, max compression
```

## Comparing `html_text-0.6.1.tar` & `html_text-0.6.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:59.789150 html_text-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-23 12:01:50.000000 html_text-0.6.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-23 12:01:50.000000 html_text-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-23 12:01:50.000000 html_text-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-23 12:01:59.789150 html_text-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-23 12:01:50.000000 html_text-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:59.785150 html_text-0.6.1/html_text/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-23 12:01:50.000000 html_text-0.6.1/html_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-23 12:01:50.000000 html_text-0.6.1/html_text/html_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:59.789150 html_text-0.6.1/html_text.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-23 12:01:59.000000 html_text-0.6.1/html_text.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-23 12:01:59.000000 html_text-0.6.1/html_text.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:01:59.000000 html_text-0.6.1/html_text.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:01:59.000000 html_text-0.6.1/html_text.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 12:01:59.000000 html_text-0.6.1/html_text.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 12:01:59.000000 html_text-0.6.1/html_text.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-23 12:01:59.789150 html_text-0.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1225 2024-04-23 12:01:50.000000 html_text-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:59.785150 html_text-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 12:01:50.000000 html_text-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-04-23 12:01:50.000000 html_text-0.6.1/tests/test_html_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:01:59.789150 html_text-0.6.1/tests/test_webpages/
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-23 12:01:50.000000 html_text-0.6.1/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.html
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-23 12:01:50.000000 html_text-0.6.1/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-04-23 12:01:50.000000 html_text-0.6.1/tests/test_webpages/IANA — IANA-managed Reserved Domains.html
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-23 12:01:50.000000 html_text-0.6.1/tests/test_webpages/IANA — IANA-managed Reserved Domains.txt
--rw-r--r--   0 runner    (1001) docker     (127)    67149 2024-04-23 12:01:50.000000 html_text-0.6.1/tests/test_webpages/Scrapinghub Enterprise Solutions.html
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-23 12:01:50.000000 html_text-0.6.1/tests/test_webpages/Scrapinghub Enterprise Solutions.txt
--rw-r--r--   0 runner    (1001) docker     (127)    38239 2024-04-23 12:01:50.000000 html_text-0.6.1/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.html
--rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-04-23 12:01:50.000000 html_text-0.6.1/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-04-23 12:01:50.000000 html_text-0.6.1/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.html
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-23 12:01:50.000000 html_text-0.6.1/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:55:07.425852 html_text-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-01 11:54:53.000000 html_text-0.6.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-01 11:54:53.000000 html_text-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-01 11:54:53.000000 html_text-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-01 11:55:07.425852 html_text-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-01 11:54:53.000000 html_text-0.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:55:07.421852 html_text-0.6.2/html_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-01 11:54:53.000000 html_text-0.6.2/html_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-05-01 11:54:53.000000 html_text-0.6.2/html_text/html_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:55:07.425852 html_text-0.6.2/html_text.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-01 11:55:07.000000 html_text-0.6.2/html_text.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-01 11:55:07.000000 html_text-0.6.2/html_text.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:55:07.000000 html_text-0.6.2/html_text.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:55:07.000000 html_text-0.6.2/html_text.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 11:55:07.000000 html_text-0.6.2/html_text.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 11:55:07.000000 html_text-0.6.2/html_text.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-01 11:55:07.429852 html_text-0.6.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1225 2024-05-01 11:54:53.000000 html_text-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:55:07.425852 html_text-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 11:54:53.000000 html_text-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-01 11:54:53.000000 html_text-0.6.2/tests/test_html_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:55:07.425852 html_text-0.6.2/tests/test_webpages/
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-01 11:54:53.000000 html_text-0.6.2/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-01 11:54:53.000000 html_text-0.6.2/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-05-01 11:54:53.000000 html_text-0.6.2/tests/test_webpages/IANA — IANA-managed Reserved Domains.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-01 11:54:53.000000 html_text-0.6.2/tests/test_webpages/IANA — IANA-managed Reserved Domains.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    67149 2024-05-01 11:54:53.000000 html_text-0.6.2/tests/test_webpages/Scrapinghub Enterprise Solutions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-01 11:54:53.000000 html_text-0.6.2/tests/test_webpages/Scrapinghub Enterprise Solutions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38239 2024-05-01 11:54:53.000000 html_text-0.6.2/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-05-01 11:54:53.000000 html_text-0.6.2/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-05-01 11:54:53.000000 html_text-0.6.2/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-01 11:54:53.000000 html_text-0.6.2/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.txt
```

### Comparing `html_text-0.6.1/CHANGES.rst` & `html_text-0.6.2/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 =======
 History
 =======
 
+0.6.2 (2024-05-01)
+------------------
+* Support deeper trees by using iteration instead of recursion.
+
 0.6.1 (2024-04-23)
 ------------------
 * Fixed HTML comment and processing instruction handling.
 * Use ``lxml-html-clean`` instead of ``lxml[html_clean]`` in setup.py,
   to avoid https://github.com/jazzband/pip-tools/issues/2004
 
 0.6.0 (2024-04-04)
```

### Comparing `html_text-0.6.1/LICENSE` & `html_text-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `html_text-0.6.1/PKG-INFO` & `html_text-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html_text
-Version: 0.6.1
+Version: 0.6.2
 Summary: Extract text from HTML
 Home-page: https://github.com/zytedata/html-text
 Author: Konstantin Lopukhin
 Author-email: kostia.lopuhin@gmail.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -146,25 +146,23 @@
 one intended usage of this library is for machine learning (feature extraction).
 If you want to use the text of the html page as a feature (e.g. for classification),
 this library gives you plain text that you can later feed into a standard text
 classification pipeline.
 If you feel that you need html structure as well, check out
 `webstruct <http://webstruct.readthedocs.io/en/latest/>`_ library.
 
-----
-
-.. image:: https://hyperiongray.s3.amazonaws.com/define-hg.svg
-	:target: https://www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text
-	:alt: define hyperiongray
-
 
 =======
 History
 =======
 
+0.6.2 (2024-05-01)
+------------------
+* Support deeper trees by using iteration instead of recursion.
+
 0.6.1 (2024-04-23)
 ------------------
 * Fixed HTML comment and processing instruction handling.
 * Use ``lxml-html-clean`` instead of ``lxml[html_clean]`` in setup.py,
   to avoid https://github.com/jazzband/pip-tools/issues/2004
 
 0.6.0 (2024-04-04)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: html_text Version: 0.6.1 Summary: Extract text from
+Metadata-Version: 2.1 Name: html_text Version: 0.6.2 Summary: Extract text from
 HTML Home-page: https://github.com/zytedata/html-text Author: Konstantin
 Lopukhin Author-email: kostia.lopuhin@gmail.com License: MIT license
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -72,45 +72,44 @@
 world!', ... newline_tags=newline_tags) 'Hello world!' Apart from just getting
 text from the page (e.g. for display or search), one intended usage of this
 library is for machine learning (feature extraction). If you want to use the
 text of the html page as a feature (e.g. for classification), this library
 gives you plain text that you can later feed into a standard text
 classification pipeline. If you feel that you need html structure as well,
 check out `webstruct
-webstruct.readthedocs.io/en/latest/>`_ library. ---- .. image:: https://
-hyperiongray.s3.amazonaws.com/define-hg.svg :target: https://
-www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text :alt: define
-hyperiongray ======= History ======= 0.6.1 (2024-04-23) ------------------ *
-Fixed HTML comment and processing instruction handling. * Use ``lxml-html-
-clean`` instead of ``lxml[html_clean]`` in setup.py, to avoid https://
-github.com/jazzband/pip-tools/issues/2004 0.6.0 (2024-04-04) -----------------
-- * Moved the Git repository to https://github.com/zytedata/html-text. * Added
-official support for Python 3.9-3.12. * Removed support for Python 2.7 and 3.5-
-3.7. * Switched the ``lxml`` dependency to ``lxml[html_clean]`` to support
-``lxml >= 5.2.0``. * Switch from Travis CI to GitHub Actions. * CI
-improvements. 0.5.2 (2020-07-22) ------------------ * Handle lxml Cleaner
-exceptions (a workaround for https://bugs.launchpad.net/lxml/+bug/1838497 ); *
-Python 3.8 support; * testing improvements. 0.5.1 (2019-05-27) ----------------
--- Fixed whitespace handling when ``guess_punct_space`` is False: html-text was
-producing unnecessary spaces after newlines. 0.5.0 (2018-11-19) ---------------
---- Parsel dependency is removed in this release, though parsel is still
-supported. * ``parsel`` package is no longer required to install and use html-
-text; * ``html_text.etree_to_text`` function allows to extract text from lxml
-Elements; * ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance
-with options tuned for text extraction speed and quality; * test and
-documentation improvements; * Python 3.7 support. 0.4.1 (2018-09-25) ----------
--------- Fixed a regression in 0.4.0 release: text was empty when
-``html_text.extract_text`` is called with a node with text, but without
-children. 0.4.0 (2018-09-25) ------------------ This is a backwards-
-incompatible release: by default html_text functions now add newlines after
-elements, if appropriate, to make the extracted text to look more like how it
-is rendered in a browser. To turn it off, pass ``guess_layout=False`` option to
-html_text functions. * ``guess_layout`` option to to make extracted text look
-more like how it is rendered in browser. * Add tests of layout extraction for
-real webpages. 0.3.0 (2017-10-12) ------------------ * Expose functions that
-operate on selectors, use ``.//text()`` to extract text from selector. 0.2.1
-(2017-05-29) ------------------ * Packaging fix (include CHANGES.rst) 0.2.0
-(2017-05-29) ------------------ * Fix unwanted joins of words with inline tags:
-spaces are added for inline tags too, but a heuristic is used to preserve
-punctuation without extra spaces. * Accept parsed html trees. 0.1.1 (2017-01-
-16) ------------------ * Travis-CI and codecov.io integrations added 0.1.0
-(2016-09-27) ------------------ * First release on PyPI.
+webstruct.readthedocs.io/en/latest/>`_ library. ======= History ======= 0.6.2
+(2024-05-01) ------------------ * Support deeper trees by using iteration
+instead of recursion. 0.6.1 (2024-04-23) ------------------ * Fixed HTML
+comment and processing instruction handling. * Use ``lxml-html-clean`` instead
+of ``lxml[html_clean]`` in setup.py, to avoid https://github.com/jazzband/pip-
+tools/issues/2004 0.6.0 (2024-04-04) ------------------ * Moved the Git
+repository to https://github.com/zytedata/html-text. * Added official support
+for Python 3.9-3.12. * Removed support for Python 2.7 and 3.5-3.7. * Switched
+the ``lxml`` dependency to ``lxml[html_clean]`` to support ``lxml >= 5.2.0``. *
+Switch from Travis CI to GitHub Actions. * CI improvements. 0.5.2 (2020-07-22)
+------------------ * Handle lxml Cleaner exceptions (a workaround for https://
+bugs.launchpad.net/lxml/+bug/1838497 ); * Python 3.8 support; * testing
+improvements. 0.5.1 (2019-05-27) ------------------ Fixed whitespace handling
+when ``guess_punct_space`` is False: html-text was producing unnecessary spaces
+after newlines. 0.5.0 (2018-11-19) ------------------ Parsel dependency is
+removed in this release, though parsel is still supported. * ``parsel`` package
+is no longer required to install and use html-text; *
+``html_text.etree_to_text`` function allows to extract text from lxml Elements;
+* ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance with options
+tuned for text extraction speed and quality; * test and documentation
+improvements; * Python 3.7 support. 0.4.1 (2018-09-25) ------------------ Fixed
+a regression in 0.4.0 release: text was empty when ``html_text.extract_text``
+is called with a node with text, but without children. 0.4.0 (2018-09-25) -----
+------------- This is a backwards-incompatible release: by default html_text
+functions now add newlines after elements, if appropriate, to make the
+extracted text to look more like how it is rendered in a browser. To turn it
+off, pass ``guess_layout=False`` option to html_text functions. *
+``guess_layout`` option to to make extracted text look more like how it is
+rendered in browser. * Add tests of layout extraction for real webpages. 0.3.0
+(2017-10-12) ------------------ * Expose functions that operate on selectors,
+use ``.//text()`` to extract text from selector. 0.2.1 (2017-05-29) -----------
+------- * Packaging fix (include CHANGES.rst) 0.2.0 (2017-05-29) --------------
+---- * Fix unwanted joins of words with inline tags: spaces are added for
+inline tags too, but a heuristic is used to preserve punctuation without extra
+spaces. * Accept parsed html trees. 0.1.1 (2017-01-16) ------------------ *
+Travis-CI and codecov.io integrations added 0.1.0 (2016-09-27) ----------------
+-- * First release on PyPI.
```

### Comparing `html_text-0.6.1/README.rst` & `html_text-0.6.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -123,13 +123,7 @@
 Apart from just getting text from the page (e.g. for display or search),
 one intended usage of this library is for machine learning (feature extraction).
 If you want to use the text of the html page as a feature (e.g. for classification),
 this library gives you plain text that you can later feed into a standard text
 classification pipeline.
 If you feel that you need html structure as well, check out
 `webstruct <http://webstruct.readthedocs.io/en/latest/>`_ library.
-
-----
-
-.. image:: https://hyperiongray.s3.amazonaws.com/define-hg.svg
-	:target: https://www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text
-	:alt: define hyperiongray
```

#### html2text {}

```diff
@@ -62,11 +62,8 @@
 world!', ... newline_tags=newline_tags) 'Hello world!' Apart from just getting
 text from the page (e.g. for display or search), one intended usage of this
 library is for machine learning (feature extraction). If you want to use the
 text of the html page as a feature (e.g. for classification), this library
 gives you plain text that you can later feed into a standard text
 classification pipeline. If you feel that you need html structure as well,
 check out `webstruct
-webstruct.readthedocs.io/en/latest/>`_ library. ---- .. image:: https://
-hyperiongray.s3.amazonaws.com/define-hg.svg :target: https://
-www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text :alt: define
-hyperiongray
+webstruct.readthedocs.io/en/latest/>`_ library.
```

### Comparing `html_text-0.6.1/html_text/html_text.py` & `html_text-0.6.2/html_text/html_text.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,69 +84,65 @@
     See html_text.extract_text docstring for description of the
     approach and options.
     """
     chunks = []
 
     _NEWLINE = object()
     _DOUBLE_NEWLINE = object()
+    prev = _DOUBLE_NEWLINE  # _NEWLINE, _DOUBLE_NEWLINE or content of the previous chunk (str)
 
-    class Context:
-        """ workaround for missing `nonlocal` in Python 2 """
-        # _NEWLINE, _DOUBLE_NEWLINE or content of the previous chunk (str)
-        prev = _DOUBLE_NEWLINE
-
-    def should_add_space(text, prev):
+    def should_add_space(text):
         """ Return True if extra whitespace should be added before text """
         if prev in {_NEWLINE, _DOUBLE_NEWLINE}:
             return False
         if not guess_punct_space:
             return True
         if not _has_trailing_whitespace(prev):
             if _has_punct_after(text) or _has_open_bracket_before(prev):
                 return False
         return True
 
-    def get_space_between(text, prev):
+    def get_space_between(text):
         if not text:
             return ' '
-        return ' ' if should_add_space(text, prev) else ''
+        return ' ' if should_add_space(text) else ''
 
-    def add_newlines(tag, context):
+    def add_newlines(tag):
+        nonlocal prev
         if not guess_layout:
             return
-        prev = context.prev
         if prev is _DOUBLE_NEWLINE:  # don't output more than 1 blank line
             return
         if tag in double_newline_tags:
-            context.prev = _DOUBLE_NEWLINE
             chunks.append('\n' if prev is _NEWLINE else '\n\n')
+            prev = _DOUBLE_NEWLINE
         elif tag in newline_tags:
-            context.prev = _NEWLINE
             if prev is not _NEWLINE:
                 chunks.append('\n')
+            prev = _NEWLINE
 
-    def add_text(text_content, context):
+    def add_text(text_content):
+        nonlocal prev
         text = _normalize_whitespace(text_content) if text_content else ''
         if not text:
             return
-        space = get_space_between(text, context.prev)
+        space = get_space_between(text)
         chunks.extend([space, text])
-        context.prev = text_content
+        prev = text_content
 
-    def traverse_text_fragments(tree, context, handle_tail=True):
-        """ Extract text from the ``tree``: fill ``chunks`` variable """
-        add_newlines(tree.tag, context)
-        add_text(tree.text, context)
-        for child in tree:
-            traverse_text_fragments(child, context)
-        add_newlines(tree.tag, context)
-        if handle_tail:
-            add_text(tree.tail, context)
+    # Extract text from the ``tree``: fill ``chunks`` variable
+    for event, el in lxml.etree.iterwalk(tree, events=('start', 'end')):
+        if event == 'start':
+            add_newlines(el.tag)
+            add_text(el.text)
+        elif event == 'end':
+            add_newlines(el.tag)
+            if el is not tree:
+                add_text(el.tail)
 
-    traverse_text_fragments(tree, context=Context(), handle_tail=False)
     return ''.join(chunks).strip()
 
 
 def selector_to_text(sel, guess_punct_space=True, guess_layout=True):
     """ Convert a cleaned parsel.Selector to text.
     See html_text.extract_text docstring for description of the approach
     and options.
```

### Comparing `html_text-0.6.1/html_text.egg-info/PKG-INFO` & `html_text-0.6.2/html_text.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html_text
-Version: 0.6.1
+Version: 0.6.2
 Summary: Extract text from HTML
 Home-page: https://github.com/zytedata/html-text
 Author: Konstantin Lopukhin
 Author-email: kostia.lopuhin@gmail.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -146,25 +146,23 @@
 one intended usage of this library is for machine learning (feature extraction).
 If you want to use the text of the html page as a feature (e.g. for classification),
 this library gives you plain text that you can later feed into a standard text
 classification pipeline.
 If you feel that you need html structure as well, check out
 `webstruct <http://webstruct.readthedocs.io/en/latest/>`_ library.
 
-----
-
-.. image:: https://hyperiongray.s3.amazonaws.com/define-hg.svg
-	:target: https://www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text
-	:alt: define hyperiongray
-
 
 =======
 History
 =======
 
+0.6.2 (2024-05-01)
+------------------
+* Support deeper trees by using iteration instead of recursion.
+
 0.6.1 (2024-04-23)
 ------------------
 * Fixed HTML comment and processing instruction handling.
 * Use ``lxml-html-clean`` instead of ``lxml[html_clean]`` in setup.py,
   to avoid https://github.com/jazzband/pip-tools/issues/2004
 
 0.6.0 (2024-04-04)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: html_text Version: 0.6.1 Summary: Extract text from
+Metadata-Version: 2.1 Name: html_text Version: 0.6.2 Summary: Extract text from
 HTML Home-page: https://github.com/zytedata/html-text Author: Konstantin
 Lopukhin Author-email: kostia.lopuhin@gmail.com License: MIT license
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -72,45 +72,44 @@
 world!', ... newline_tags=newline_tags) 'Hello world!' Apart from just getting
 text from the page (e.g. for display or search), one intended usage of this
 library is for machine learning (feature extraction). If you want to use the
 text of the html page as a feature (e.g. for classification), this library
 gives you plain text that you can later feed into a standard text
 classification pipeline. If you feel that you need html structure as well,
 check out `webstruct
-webstruct.readthedocs.io/en/latest/>`_ library. ---- .. image:: https://
-hyperiongray.s3.amazonaws.com/define-hg.svg :target: https://
-www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text :alt: define
-hyperiongray ======= History ======= 0.6.1 (2024-04-23) ------------------ *
-Fixed HTML comment and processing instruction handling. * Use ``lxml-html-
-clean`` instead of ``lxml[html_clean]`` in setup.py, to avoid https://
-github.com/jazzband/pip-tools/issues/2004 0.6.0 (2024-04-04) -----------------
-- * Moved the Git repository to https://github.com/zytedata/html-text. * Added
-official support for Python 3.9-3.12. * Removed support for Python 2.7 and 3.5-
-3.7. * Switched the ``lxml`` dependency to ``lxml[html_clean]`` to support
-``lxml >= 5.2.0``. * Switch from Travis CI to GitHub Actions. * CI
-improvements. 0.5.2 (2020-07-22) ------------------ * Handle lxml Cleaner
-exceptions (a workaround for https://bugs.launchpad.net/lxml/+bug/1838497 ); *
-Python 3.8 support; * testing improvements. 0.5.1 (2019-05-27) ----------------
--- Fixed whitespace handling when ``guess_punct_space`` is False: html-text was
-producing unnecessary spaces after newlines. 0.5.0 (2018-11-19) ---------------
---- Parsel dependency is removed in this release, though parsel is still
-supported. * ``parsel`` package is no longer required to install and use html-
-text; * ``html_text.etree_to_text`` function allows to extract text from lxml
-Elements; * ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance
-with options tuned for text extraction speed and quality; * test and
-documentation improvements; * Python 3.7 support. 0.4.1 (2018-09-25) ----------
--------- Fixed a regression in 0.4.0 release: text was empty when
-``html_text.extract_text`` is called with a node with text, but without
-children. 0.4.0 (2018-09-25) ------------------ This is a backwards-
-incompatible release: by default html_text functions now add newlines after
-elements, if appropriate, to make the extracted text to look more like how it
-is rendered in a browser. To turn it off, pass ``guess_layout=False`` option to
-html_text functions. * ``guess_layout`` option to to make extracted text look
-more like how it is rendered in browser. * Add tests of layout extraction for
-real webpages. 0.3.0 (2017-10-12) ------------------ * Expose functions that
-operate on selectors, use ``.//text()`` to extract text from selector. 0.2.1
-(2017-05-29) ------------------ * Packaging fix (include CHANGES.rst) 0.2.0
-(2017-05-29) ------------------ * Fix unwanted joins of words with inline tags:
-spaces are added for inline tags too, but a heuristic is used to preserve
-punctuation without extra spaces. * Accept parsed html trees. 0.1.1 (2017-01-
-16) ------------------ * Travis-CI and codecov.io integrations added 0.1.0
-(2016-09-27) ------------------ * First release on PyPI.
+webstruct.readthedocs.io/en/latest/>`_ library. ======= History ======= 0.6.2
+(2024-05-01) ------------------ * Support deeper trees by using iteration
+instead of recursion. 0.6.1 (2024-04-23) ------------------ * Fixed HTML
+comment and processing instruction handling. * Use ``lxml-html-clean`` instead
+of ``lxml[html_clean]`` in setup.py, to avoid https://github.com/jazzband/pip-
+tools/issues/2004 0.6.0 (2024-04-04) ------------------ * Moved the Git
+repository to https://github.com/zytedata/html-text. * Added official support
+for Python 3.9-3.12. * Removed support for Python 2.7 and 3.5-3.7. * Switched
+the ``lxml`` dependency to ``lxml[html_clean]`` to support ``lxml >= 5.2.0``. *
+Switch from Travis CI to GitHub Actions. * CI improvements. 0.5.2 (2020-07-22)
+------------------ * Handle lxml Cleaner exceptions (a workaround for https://
+bugs.launchpad.net/lxml/+bug/1838497 ); * Python 3.8 support; * testing
+improvements. 0.5.1 (2019-05-27) ------------------ Fixed whitespace handling
+when ``guess_punct_space`` is False: html-text was producing unnecessary spaces
+after newlines. 0.5.0 (2018-11-19) ------------------ Parsel dependency is
+removed in this release, though parsel is still supported. * ``parsel`` package
+is no longer required to install and use html-text; *
+``html_text.etree_to_text`` function allows to extract text from lxml Elements;
+* ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance with options
+tuned for text extraction speed and quality; * test and documentation
+improvements; * Python 3.7 support. 0.4.1 (2018-09-25) ------------------ Fixed
+a regression in 0.4.0 release: text was empty when ``html_text.extract_text``
+is called with a node with text, but without children. 0.4.0 (2018-09-25) -----
+------------- This is a backwards-incompatible release: by default html_text
+functions now add newlines after elements, if appropriate, to make the
+extracted text to look more like how it is rendered in a browser. To turn it
+off, pass ``guess_layout=False`` option to html_text functions. *
+``guess_layout`` option to to make extracted text look more like how it is
+rendered in browser. * Add tests of layout extraction for real webpages. 0.3.0
+(2017-10-12) ------------------ * Expose functions that operate on selectors,
+use ``.//text()`` to extract text from selector. 0.2.1 (2017-05-29) -----------
+------- * Packaging fix (include CHANGES.rst) 0.2.0 (2017-05-29) --------------
+---- * Fix unwanted joins of words with inline tags: spaces are added for
+inline tags too, but a heuristic is used to preserve punctuation without extra
+spaces. * Accept parsed html trees. 0.1.1 (2017-01-16) ------------------ *
+Travis-CI and codecov.io integrations added 0.1.0 (2016-09-27) ----------------
+-- * First release on PyPI.
```

### Comparing `html_text-0.6.1/html_text.egg-info/SOURCES.txt` & `html_text-0.6.2/html_text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.6.1/setup.py` & `html_text-0.6.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open('CHANGES.rst') as history_file:
     history = history_file.read()
 
 
 setup(
     name='html_text',
-    version='0.6.1',
+    version='0.6.2',
     description="Extract text from HTML",
     long_description=readme + '\n\n' + history,
     author="Konstantin Lopukhin",
     author_email='kostia.lopuhin@gmail.com',
     url='https://github.com/zytedata/html-text',
     packages=['html_text'],
     include_package_data=True,
```

### Comparing `html_text-0.6.1/tests/test_html_text.py` & `html_text-0.6.2/tests/test_html_text.py`

 * *Files 5% similar despite different names*

```diff
@@ -210,7 +210,27 @@
 def test_webpages(page, extracted):
     html = _load_file(page)
     expected = _load_file(extracted)
     assert extract_text(html) == expected
 
     tree = cleaner.clean_html(parse_html(html))
     assert etree_to_text(tree) == expected
+
+
+def test_deep_html():
+    """ Make sure we don't crash due to recursion limit.
+    """
+    # Build a deep tree manually as default parser would only allow
+    # for 255 depth, but deeper trees are possible with other parsers
+    n = 5000
+    parent = root = None
+    for _ in range(n):
+        el = lxml.html.Element('div')
+        el.text = 'foo'
+        if parent is None:
+            root = el
+            parent = el
+        else:
+            parent.append(el)
+            parent = el
+
+    assert extract_text(root) == ('foo\n' * n).strip()
```

### Comparing `html_text-0.6.1/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.html` & `html_text-0.6.2/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.html`

 * *Files identical despite different names*

### Comparing `html_text-0.6.1/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.txt` & `html_text-0.6.2/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.6.1/tests/test_webpages/IANA — IANA-managed Reserved Domains.html` & `html_text-0.6.2/tests/test_webpages/IANA — IANA-managed Reserved Domains.html`

 * *Files identical despite different names*

### Comparing `html_text-0.6.1/tests/test_webpages/IANA — IANA-managed Reserved Domains.txt` & `html_text-0.6.2/tests/test_webpages/IANA — IANA-managed Reserved Domains.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.6.1/tests/test_webpages/Scrapinghub Enterprise Solutions.html` & `html_text-0.6.2/tests/test_webpages/Scrapinghub Enterprise Solutions.html`

 * *Files identical despite different names*

### Comparing `html_text-0.6.1/tests/test_webpages/Scrapinghub Enterprise Solutions.txt` & `html_text-0.6.2/tests/test_webpages/Scrapinghub Enterprise Solutions.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.6.1/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.html` & `html_text-0.6.2/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.html`

 * *Files identical despite different names*

### Comparing `html_text-0.6.1/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.txt` & `html_text-0.6.2/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.6.1/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.html` & `html_text-0.6.2/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.html`

 * *Files identical despite different names*

### Comparing `html_text-0.6.1/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.txt` & `html_text-0.6.2/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.txt`

 * *Files identical despite different names*

