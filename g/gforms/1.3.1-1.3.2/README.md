# Comparing `tmp/gforms-1.3.1.tar.gz` & `tmp/gforms-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gforms-1.3.1.tar", last modified: Sat Mar 18 13:51:12 2023, max compression
+gzip compressed data, was "gforms-1.3.2.tar", last modified: Wed May  1 20:36:19 2024, max compression
```

## Comparing `gforms-1.3.1.tar` & `gforms-1.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:51:12.796942 gforms-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-18 13:50:59.000000 gforms-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-03-18 13:51:12.796942 gforms-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-18 13:50:59.000000 gforms-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:51:12.796942 gforms-1.3.1/gforms/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-18 13:50:59.000000 gforms-1.3.1/gforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26221 2023-03-18 13:50:59.000000 gforms-1.3.1/gforms/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    31250 2023-03-18 13:50:59.000000 gforms-1.3.1/gforms/elements_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-03-18 13:50:59.000000 gforms-1.3.1/gforms/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    36851 2023-03-18 13:50:59.000000 gforms-1.3.1/gforms/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-18 13:50:59.000000 gforms-1.3.1/gforms/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-03-18 13:50:59.000000 gforms-1.3.1/gforms/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-18 13:50:59.000000 gforms-1.3.1/gforms/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-03-18 13:50:59.000000 gforms-1.3.1/gforms/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:51:12.796942 gforms-1.3.1/gforms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-03-18 13:51:12.000000 gforms-1.3.1/gforms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-18 13:51:12.000000 gforms-1.3.1/gforms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 13:51:12.000000 gforms-1.3.1/gforms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-18 13:51:12.000000 gforms-1.3.1/gforms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-18 13:51:12.000000 gforms-1.3.1/gforms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-18 13:51:12.796942 gforms-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-18 13:50:59.000000 gforms-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:36:19.095749 gforms-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 20:36:11.000000 gforms-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-01 20:36:19.095749 gforms-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-01 20:36:11.000000 gforms-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:36:19.095749 gforms-1.3.2/gforms/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-01 20:36:11.000000 gforms-1.3.2/gforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26221 2024-05-01 20:36:11.000000 gforms-1.3.2/gforms/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31250 2024-05-01 20:36:11.000000 gforms-1.3.2/gforms/elements_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-01 20:36:11.000000 gforms-1.3.2/gforms/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36856 2024-05-01 20:36:11.000000 gforms-1.3.2/gforms/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-01 20:36:11.000000 gforms-1.3.2/gforms/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-01 20:36:11.000000 gforms-1.3.2/gforms/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-01 20:36:11.000000 gforms-1.3.2/gforms/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-05-01 20:36:11.000000 gforms-1.3.2/gforms/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:36:19.095749 gforms-1.3.2/gforms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-01 20:36:19.000000 gforms-1.3.2/gforms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 20:36:19.000000 gforms-1.3.2/gforms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:36:19.000000 gforms-1.3.2/gforms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-01 20:36:19.000000 gforms-1.3.2/gforms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 20:36:19.000000 gforms-1.3.2/gforms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:36:19.095749 gforms-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-01 20:36:11.000000 gforms-1.3.2/setup.py
```

### Comparing `gforms-1.3.1/LICENSE` & `gforms-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gforms-1.3.1/PKG-INFO` & `gforms-1.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: gforms
-Version: 1.3.1
+Version: 1.3.2
 Summary: Google Forms wrapper for Python
 Home-page: https://github.com/vvd170501/python-gforms
 Author: vvd170501
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: requests
+Requires-Dist: typing-extensions; python_version < "3.8"
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
 
 # GForms
 
 A python wrapper for public Google Forms.
 
 **This package does not implement form editing / sharing / other actions with user-owned forms**
```

### Comparing `gforms-1.3.1/README.md` & `gforms-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `gforms-1.3.1/gforms/elements.py` & `gforms-1.3.2/gforms/elements.py`

 * *Files identical despite different names*

### Comparing `gforms-1.3.1/gforms/elements_base.py` & `gforms-1.3.2/gforms/elements_base.py`

 * *Files identical despite different names*

### Comparing `gforms-1.3.1/gforms/errors.py` & `gforms-1.3.2/gforms/errors.py`

 * *Files identical despite different names*

### Comparing `gforms-1.3.1/gforms/form.py` & `gforms-1.3.2/gforms/form.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,36 +71,39 @@
         # First block
         CONFIRMATION_MSG = 0
         SHOW_RESUBMIT_LINK = 1
         SHOW_SUMMARY = 2
         EDIT_RESPONSES = 3
         # Second block. The first 4 elements may be None
         SHOW_PROGRESSBAR = 0
-        # Signin requirement is not present in form data?
-        # Both values (this and MAYBE_SUBMIT_ONCE) are false for a form with a file upload element.
         SUBMIT_ONCE = 1  # None(default/not set?) == False?
         SHUFFLE_QUESTIONS = 2
         RECEIPT = 3
-        COLLECT_EMAILS = 4
-        DISABLE_AUTOSAVE = 5  # may be missing
-        # 17.03.2023: Now there's a 7th field (index 6), seems like it's always present.
-        # Its value is 3 if COLLECT_EMAILS is enabled, and 1 otherwise.
-        # Other known settings don't affect this field.
+        OLD_COLLECT_EMAILS = 4  # Not used anymore, seems to always be None
+        DISABLE_AUTOSAVE = 5  # May be missing in old forms
+        COLLECT_EMAILS = 6
 
         # Quiz block
-        # It's possible to create a form with IMMEDIATE_GRADES ==  COLLECT_EMAILS == 0
         GRADES_SETTINGS = 0
         SHOW_MISSED = 2
         SHOW_CORRECT = 3
         SHOW_POINTS = 4
         IMMEDIATE_GRADES = 1
         IS_QUIZ = 2
 
+    class CollectEmails(Enum):
+        NO = 1
+        VERIFIED = 2
+        USER_INPUT = 3  # "Responder input" - same behavior as the old "collect emails" flag
+
+        def __bool__(self):
+            return self != self.NO
+
     class SendReceipt(Enum):
-        UNUSED = None  # value is None when collect_emails is False
+        UNUSED = None  # value was None with collect_emails = False (01.05.2023 - default is 2, but old forms still have None)
         OPT_IN = 1
         NEVER = 2
         ALWAYS = 3
 
     def parse(self, form_data):
         # any block may be missing
         first_block = form_data[self._Index.FIRST_BLOCK]
@@ -113,28 +116,28 @@
             self.show_summary = bool(first_block[self._Index.SHOW_SUMMARY])
             self.edit_responses = bool(first_block[self._Index.EDIT_RESPONSES])
         if second_block is not None:
             self.show_progressbar = bool(second_block[self._Index.SHOW_PROGRESSBAR])
             self.submit_once = bool(second_block[self._Index.SUBMIT_ONCE])
             self.shuffle_questions = bool(second_block[self._Index.SHUFFLE_QUESTIONS])
             self.send_receipt = self.SendReceipt(second_block[self._Index.RECEIPT])
-            self.collect_emails = bool(list_get(second_block, self._Index.COLLECT_EMAILS, False))
             self.disable_autosave = bool(list_get(second_block, self._Index.DISABLE_AUTOSAVE, False))
+            self.collect_emails = self.CollectEmails(list_get(second_block, self._Index.COLLECT_EMAILS, self.CollectEmails.NO))
         if quiz is not None:
             self.is_quiz = bool(list_get(quiz, self._Index.IS_QUIZ, False))
         if self.is_quiz:
             self.immediate_grades = bool(quiz[self._Index.IMMEDIATE_GRADES])
             grades_settings = quiz[self._Index.GRADES_SETTINGS]
             self.show_missed = bool(grades_settings[self._Index.SHOW_MISSED])
             self.show_correct_answers = bool(grades_settings[self._Index.SHOW_CORRECT])
             self.show_points = bool(grades_settings[self._Index.SHOW_POINTS])
 
     def __init__(self):
         """Initializes all settings with a default value."""
-        self.collect_emails = False
+        self.collect_emails = self.CollectEmails.NO
         self.send_receipt = self.SendReceipt.UNUSED
         self.submit_once = False
         self.show_summary = False
         self.edit_responses = False
 
         self.show_progressbar = False
         self.shuffle_questions = False
@@ -213,15 +216,15 @@
         is_loaded: Indicates if this form was properly loaded and parsed.
     """
 
     class _DocIndex:
         FORM = 1
         NAME = 3
         URL = 14  # Unused.
-        MAYBE_SUBMIT_ONCE = 18  # Duplicate / other meaning? Currently unused
+        SIGNIN_REQUIRED = 18
 
     class _FormIndex:
         DESCRIPTION = 0
         ELEMENTS = 1
         STYLE = 4  # Not implemented
         TITLE = 8
 
@@ -245,17 +248,18 @@
     _history: Optional[str]
     _draft: Optional[str]
 
     @property
     def requires_signin(self):
         """If True, the user must use a google account to submit this form."""
         # NOTE also should be true for forms with file upload,
-        # but now (06 Sep 2021) such forms can't be loaded (HTTP Unauthorized on the first page)
-        # Signin requirement may depend on other form elements (if they are added in future).
-        return self.settings.submit_once
+        # but as of 01 May 2024, such forms have _signin_required == False for some reason.
+        # These forms can't be loaded anyway (request is redirected to the sign-in page),
+        # so this case is not handled.
+        return self._signin_required
 
     @property
     def is_validated(self):
         """Indicates if this form was successfully validated and may be submitted."""
         return len(self._unvalidated_pages) == 0 and self._found_full_path
 
     def __init__(self):
@@ -528,14 +532,15 @@
     def _clear(self):
         self.url = None
         self.name = None
         self.title = None
         self.description = None
         self.pages = []
         self.settings = Settings()
+        self._signin_required = False
         self.is_loaded = False
 
         self._prefilled_data = {}
         self._first_page = None
 
         self._selected_pages = set()
         self._unvalidated_pages = set()
@@ -598,15 +603,16 @@
         self.name = data[self._DocIndex.NAME]
         form = data[self._DocIndex.FORM]
         self.title = form[self._FormIndex.TITLE]
         if not self.title:
             self.title = self.name
         self.description = form[self._FormIndex.DESCRIPTION]
 
-        self.settings.parse(form)  # NOTE may need data[18] in future
+        self.settings.parse(form)
+        self._signin_required = data[self._DocIndex.SIGNIN_REQUIRED]
 
         self._add_page(Page.first())
         self._selected_pages = {self.pages[0]}  # The first page will be submitted for any path.
         # A single-page form (even with action elements)
         # doesn't require a path check (actions are ignored).
         self._found_full_path = True
```

### Comparing `gforms-1.3.1/gforms/media.py` & `gforms-1.3.2/gforms/media.py`

 * *Files identical despite different names*

### Comparing `gforms-1.3.1/gforms/options.py` & `gforms-1.3.2/gforms/options.py`

 * *Files identical despite different names*

### Comparing `gforms-1.3.1/gforms/util.py` & `gforms-1.3.2/gforms/util.py`

 * *Files identical despite different names*

### Comparing `gforms-1.3.1/gforms/validators.py` & `gforms-1.3.2/gforms/validators.py`

 * *Files identical despite different names*

### Comparing `gforms-1.3.1/gforms.egg-info/PKG-INFO` & `gforms-1.3.2/gforms.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: gforms
-Version: 1.3.1
+Version: 1.3.2
 Summary: Google Forms wrapper for Python
 Home-page: https://github.com/vvd170501/python-gforms
 Author: vvd170501
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: requests
+Requires-Dist: typing-extensions; python_version < "3.8"
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
 
 # GForms
 
 A python wrapper for public Google Forms.
 
 **This package does not implement form editing / sharing / other actions with user-owned forms**
```

### Comparing `gforms-1.3.1/setup.py` & `gforms-1.3.2/setup.py`

 * *Files identical despite different names*

