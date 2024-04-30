# Comparing `tmp/django_monkey_patches-2.9.1.tar.gz` & `tmp/django_monkey_patches-3.0.0.tar.gz`

## Comparing `django_monkey_patches-2.9.1.tar` & `django_monkey_patches-3.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/README_printable.md
--rwxr-xr-x   0        0        0     1646 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/build_and_checks.sh
--rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/build_readme.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches/__init__.py
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches/django__base_cache__make_cache_key.py
--rw-r--r--   0        0        0    15568 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches/django__orm__prefetch.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches/django__query_set.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches/django__query_set__get.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches/django__query_set__get_or_create.py
--rw-r--r--   0        0        0    33746 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches/django__query_wrapper.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches/django__test_case__tear_down.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches/django_rest_framework__field__get_request.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
--rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches.egg-info/PKG-INFO
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches.egg-info/requires.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/src/django_monkey_patches.egg-info/top_level.txt
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/COPYING.LESSER
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/pyproject.toml
--rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 django_monkey_patches-2.9.1/PKG-INFO
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/README_printable.md
+-rwxr-xr-x   0        0        0     1646 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/build_and_checks.sh
+-rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/build_readme.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/__init__.py
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__base_cache__make_cache_key.py
+-rw-r--r--   0        0        0    15568 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__orm__prefetch.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_set.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_set__get.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_set__get_or_create.py
+-rw-r--r--   0        0        0    37274 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_wrapper.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django__test_case__tear_down.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django_rest_framework__field__get_request.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
+-rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/requires.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/COPYING.LESSER
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    13519 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.0/PKG-INFO
```

### Comparing `django_monkey_patches-2.9.1/README_printable.md` & `django_monkey_patches-3.0.0/README_printable.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 [![CodeFactor-badge]][CodeFactor-package-page]
 [![CodeClimateMaintainability-badge]][CodeClimateM13y-package-page]
 [![Codacy-badge]][Codacy-package-page]
 ![GitHub-top-language-badge]
 ![GitHub-license-badge]
 ![PyPI-python-version-badge]
 ![GitHub-code-size-in-bytes-badge]
-[![GitHub-sponsors-badge]][GitHub-sponsors-page]
 
 | **A collection of monkey patches to improve Django framework** |
 
 
 ## Use
 
 Each monkey-patch `beautiful_patch` should be available
@@ -121,11 +120,7 @@
 
 [PyPI-python-version-badge]: https://img.shields.io/pypi/pyversions/\
 django-monkey-patches
 
 [GitHub-code-size-in-bytes-badge]: https://img.shields.io/github/\
 languages/code-size/llyaudet/django-monkey-patches
 
-[GitHub-sponsors-badge]: https://img.shields.io/github/sponsors/\
-LLyaudet
-
-[GitHub-sponsors-page]: https://github.com/sponsors/LLyaudet
```

### Comparing `django_monkey_patches-2.9.1/build_and_checks.sh` & `django_monkey_patches-3.0.0/build_and_checks.sh`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/build_readme.sh` & `django_monkey_patches-3.0.0/build_readme.sh`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py` & `django_monkey_patches-3.0.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/src/django_monkey_patches/django__base_cache__make_cache_key.py` & `django_monkey_patches-3.0.0/src/django_monkey_patches/django__base_cache__make_cache_key.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/src/django_monkey_patches/django__orm__prefetch.py` & `django_monkey_patches-3.0.0/src/django_monkey_patches/django__orm__prefetch.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py` & `django_monkey_patches-3.0.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/src/django_monkey_patches/django__query_set.py` & `django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_set.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/src/django_monkey_patches/django__query_set__get.py` & `django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_set__get.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/src/django_monkey_patches/django__query_set__get_or_create.py` & `django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_set__get_or_create.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/src/django_monkey_patches/django__query_wrapper.py` & `django_monkey_patches-3.0.0/src/django_monkey_patches/django__query_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 A full-featured custom query wrapper and constants to control it,
 plus functions to customize part of its behavior.
 The goal is to give back full control to the developper
 by enabling debug, etc. that will be localized to a problem to solve
 without making the whole application unusable/slow in production.
 """
 
+# pylint: disable=too-many-lines
+
+import os
 import re
 import time
 import traceback
 
 # pylint: disable-next=import-error
 from django.db import connections
 
@@ -90,14 +93,36 @@
 # Please, look at the message at the beginning of
 # get_extra_data_template_for_set_of_queries_v1(),
 # and submit an issue if needed.
 # Otherwise, there may be a "new v1" that will break your code.
 # The other backward compatible problems should normally be adressed.
 
 
+def get_reference_pid():
+    """
+    A central function needed because Django connections can be shared
+    between multiple processes.
+    """
+
+    return connections.django_monkey_patches_reference_pids.get(
+        os.getpid(), os.getpid()
+    )
+
+
+def get_connection_dict(connection):
+    """
+    Always use this method
+    if you don't want compatibility problems later.
+    """
+
+    return connection.django_monkey_patches_dict.get(
+        get_reference_pid()
+    )
+
+
 def custom_query_wrapper_v1(execute, sql, params, many, context):
     """
     This custom query wrapper features many options
     to help debug and profile database queries.
     You should be able to do anything you want with it.
     Below, are given data structures and a POST_EXECUTION_CALLBACK
     that should handle most of your use cases.
@@ -172,17 +197,17 @@
     end_time = None
     duration = None
     if TIME_QUERIES:
         end_time = time.time()
         duration = end_time - start_time
 
     if COUNT_QUERIES:
-        connections.django_monkey_patches_dict["query_count"] += 1
+        get_connection_dict(connections)["query_count"] += 1
         connection = context["connection"]
-        connection.django_monkey_patches_dict["query_count"] += 1
+        get_connection_dict(connection)["query_count"] += 1
 
     if POST_EXECUTION_CALLBACK is not None:
         result = POST_EXECUTION_CALLBACK(
             execute,
             sql,
             params,
             many,
@@ -487,45 +512,94 @@
         # the bottom-up post-processing makes more sense.
         # (Think sorting sub-results, etc.)
     }
     result.update(result_content)
     return result
 
 
+def get_connection_stack(connection):
+    """
+    Always use this method
+    if you don't want compatibility problems later.
+    """
+
+    return connection.django_monkey_patches_stash_stack.get(
+        get_reference_pid()
+    )
+
+
+def is_globally_init():
+    """
+    Since Django connections are shared between processes
+    in many cases,
+    tell if these connections already have the dicts linked
+    to this patch.
+    """
+
+    return hasattr(connections, "django_monkey_patches_dict")
+
+
+def is_locally_init():
+    """
+    Since Django connections are shared between processes
+    in many cases,
+    tell if these connections already have the dicts linked
+    to this patch.
+    And test if these dicts have values for the current reference_pid.
+    """
+
+    return (
+        is_globally_init()
+        and connections.django_monkey_patches_dict.get(
+            get_reference_pid()
+        )
+        is not None
+    )
+
+
 def init_connections_extra_data(
     get_extra_data_template_callback,
     manager=None,
     empty_stash_stack=False,
 ):
     """
     You should call this function or a custom one
     before using the custom query wrapper.
     """
 
-    connections.django_monkey_patches_dict = (
+    if not is_globally_init():
+        connections.django_monkey_patches_reference_pids = {}
+        connections.django_monkey_patches_dict = {}
+        connections.django_monkey_patches_stash_stack = {}
+        for connection_key in connections:
+            connection = connections[connection_key]
+            connection.django_monkey_patches_reference_pids = {}
+            connection.django_monkey_patches_dict = {}
+            connection.django_monkey_patches_stash_stack = {}
+
+    connections.django_monkey_patches_dict[get_reference_pid()] = (
         get_extra_data_template_callback()
     )
-    if empty_stash_stack or not hasattr(
-        connections, "django_monkey_patches_stash_stack"
-    ):
-        connections.django_monkey_patches_stash_stack = (
-            get_managed_list(manager)
-        )
+    if empty_stash_stack or get_connection_stack(connections) is None:
+        connections.django_monkey_patches_stash_stack[
+            get_reference_pid()
+        ] = get_managed_list(manager)
 
     for connection_key in connections:
         connection = connections[connection_key]
-        connection.django_monkey_patches_dict = (
+        connection.django_monkey_patches_dict[get_reference_pid()] = (
             get_extra_data_template_callback()
         )
-        if empty_stash_stack or not hasattr(
-            connection, "django_monkey_patches_stash_stack"
+        if (
+            empty_stash_stack
+            or get_connection_stack(connection) is None
         ):
-            connection.django_monkey_patches_stash_stack = (
-                get_managed_list(manager)
-            )
+            connection.django_monkey_patches_stash_stack[
+                get_reference_pid()
+            ] = get_managed_list(manager)
 
 
 # pylint: disable-next=too-many-arguments
 def init_connections_extra_data_v1(
     manager=None,
     empty_stash_stack=False,
     query_fields=None,
@@ -592,16 +666,18 @@
 ):
     """
     The entry-point function to insert query data in relevant dicts.
     It should be your default POST_EXECUTION_CALLBACK.
     """
 
     all_dicts = [
-        connections.django_monkey_patches_dict,
-        context["connection"].django_monkey_patches_dict,
+        connections.django_monkey_patches_dict[get_reference_pid()],
+        context["connection"].django_monkey_patches_dict[
+            get_reference_pid()
+        ],
     ]
     data = {
         "execute": execute,
         "sql": sql,
         "params": params,
         "many": many,
         "context": context,
@@ -708,17 +784,21 @@
 
 def synthetize_connections_extra_data_v1():
     """
     The entry-point function to call synthetize_extra_data_dict_v1()
     on all root extra data dicts.
     """
 
-    extra_data_dicts = [connections.django_monkey_patches_dict]
+    extra_data_dicts = [
+        connections.django_monkey_patches_dict[get_reference_pid()]
+    ]
     extra_data_dicts.extend(
-        connections[connection_key].django_monkey_patches_dict
+        connections[connection_key].django_monkey_patches_dict[
+            get_reference_pid()
+        ]
         for connection_key in connections
     )
     for extra_data_dict in extra_data_dicts:
         synthetize_extra_data_dict_v1(extra_data_dict)
 
 
 def synthetize_extra_data_dict_v1(extra_data_dict):
@@ -810,27 +890,35 @@
 
 def stash_extra_data_dicts(reinit_after_stash=None):
     """
     Stash current django_monkey_patches_dicts
     in django_monkey_patches_stash_stacks.
     """
 
-    connections.django_monkey_patches_stash_stack.append(
-        connections.django_monkey_patches_dict
+    connections.django_monkey_patches_stash_stack[
+        get_reference_pid()
+    ].append(
+        connections.django_monkey_patches_dict[get_reference_pid()]
     )
 
     if reinit_after_stash is None:
-        connections.django_monkey_patches_dict = None
+        connections.django_monkey_patches_dict[
+            get_reference_pid()
+        ] = None
     for connection_key in connections:
         connection = connections[connection_key]
-        connection.django_monkey_patches_stash_stack.append(
-            connection.django_monkey_patches_dict
+        connection.django_monkey_patches_stash_stack[
+            get_reference_pid()
+        ].append(
+            connection.django_monkey_patches_dict[get_reference_pid()]
         )
         if reinit_after_stash is None:
-            connection.django_monkey_patches_dict = None
+            connection.django_monkey_patches_dict[
+                get_reference_pid()
+            ] = None
 
     if reinit_after_stash:
         reinit_after_stash()
 
 
 # pylint: disable-next=too-many-arguments
 def stash_extra_data_dicts_and_reinit_v1(
@@ -885,24 +973,55 @@
 
 def pop_extra_data_dicts():
     """
     Pop last dicts in django_monkey_patches_stash_stacks
     to django_monkey_patches_dicts.
     """
 
-    connections.django_monkey_patches_dict = (
-        connections.django_monkey_patches_stash_stack.pop()
+    connections.django_monkey_patches_dict[get_reference_pid()] = (
+        connections.django_monkey_patches_stash_stack[
+            get_reference_pid()
+        ].pop()
     )
     for connection_key in connections:
         connection = connections[connection_key]
-        connection.django_monkey_patches_dict = (
-            connection.django_monkey_patches_stash_stack.pop()
+        connection.django_monkey_patches_dict[get_reference_pid()] = (
+            connection.django_monkey_patches_stash_stack[
+                get_reference_pid()
+            ].pop()
         )
 
 
+def patch_rq_v1():
+    """
+    A function to apply a patch to rq needed to follow pids between
+    parent and child processes in Django-rq.
+    """
+
+    # pylint: disable-next=import-error,import-outside-toplevel
+    from rq.worker import Worker
+
+    original_fork_work_horse = Worker.fork_work_horse
+    original_main_work_horse = Worker.main_work_horse
+
+    def fork_work_horse(self, job, queue):
+        job.reference_pid = os.getpid()
+        return original_fork_work_horse(self, job, queue)
+
+    def main_work_horse(self, job, queue):
+        connections.django_monkey_patches_reference_pids[
+            os.getpid()
+        ] = job.reference_pid
+        return original_main_work_horse(self, job, queue)
+
+    Worker.fork_work_horse = fork_work_horse
+    Worker.main_work_horse = main_work_horse
+    return (original_fork_work_horse, original_main_work_horse)
+
+
 # You should extract the data to logs or files,
 # during execution or at the end,
 # using custom insertion_callback or post_processing_callback.
 # Here is an example of intermediate complexity
 # using all of the above.
 #
 # from contextlib import ExitStack
@@ -936,21 +1055,21 @@
 #
 # class CustomQueryWrapperMiddleware:
 #     def __init__(self, get_response):
 #         self.get_response = get_response
 #
 #     def __call__(self, request):
 #         init_connections_extra_data_v1()
-#         connection.django_monkey_patches_dict[
+#         connection.django_monkey_patches_dict[get_reference_pid()][
 #             "allocated_subsets_extra_data"
 #         ] = {"per_sql_signature_v1": {},}
-#         connection.django_monkey_patches_dict[
+#         connection.django_monkey_patches_dict[get_reference_pid()][
 #             "allocated_subsets_key_callback"
 #         ] = {"per_sql_signature_v1": get_sql_signature_v1,}
-#         connection.django_monkey_patches_dict[
+#         connection.django_monkey_patches_dict[get_reference_pid()][
 #             "allocated_subsets_init_callback"
 #         ] = {
 #             "per_sql_signature_v1": (
 #                 lambda x, y: (
 #                     get_extra_data_template_for_set_of_queries_v1(
 #                         query_fields=[
 #                             "sql",
@@ -965,28 +1084,32 @@
 #                             get_full_query_v1,
 #                         ],
 #                     )
 #                 )
 #             ),
 #         }
 #
-#         connection.django_monkey_patches_dict[
+#         connection.django_monkey_patches_dict[get_reference_pid()][
 #             "bottom_up_post_processing_callback"
 #         ] = (
 #             lambda x: (
 #               apply_reorder_dict_by_total_duration_of_sub_dicts_to(
 #                 x["allocated_subsets_extra_data"],
 #                 "per_sql_signature_v1",
 #               )
 #             )
 #         )
 #         with ExitStack() as exit_stack:
 #             wrap_connections(exit_stack, custom_query_wrapper_v1)
 #             response = self.get_response(request)
 #             synthetize_connections_extra_data_v1()
 #             # dump to file or log:
-#             # connections.django_monkey_patches_dict
+#             # connections.django_monkey_patches_dict[
+#             #     get_reference_pid()
+#             # ]
 #             # for connection_key in connections:
 #             #     some_connection = connections[connection_key]
 #             #     # dump to file or log:
-#             #     # some_connection.django_monkey_patches_dict
+#             #     # some_connection.django_monkey_patches_dict[
+#             #     #     get_reference_pid()
+#             #     # ]
 #             return response
```

### Comparing `django_monkey_patches-2.9.1/src/django_monkey_patches/django__test_case__tear_down.py` & `django_monkey_patches-3.0.0/src/django_monkey_patches/django__test_case__tear_down.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/src/django_monkey_patches/django_rest_framework__field__get_request.py` & `django_monkey_patches-3.0.0/src/django_monkey_patches/django_rest_framework__field__get_request.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py` & `django_monkey_patches-3.0.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/src/django_monkey_patches.egg-info/PKG-INFO` & `django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/src/django_monkey_patches.egg-info/SOURCES.txt` & `django_monkey_patches-3.0.0/src/django_monkey_patches.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/COPYING` & `django_monkey_patches-3.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/COPYING.LESSER` & `django_monkey_patches-3.0.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.9.1/README.md` & `django_monkey_patches-3.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 [![CodeFactor-badge]][CodeFactor-package-page]
 [![CodeClimateMaintainability-badge]][CodeClimateM13y-package-page]
 [![Codacy-badge]][Codacy-package-page]
 ![GitHub-top-language-badge]
 ![GitHub-license-badge]
 ![PyPI-python-version-badge]
 ![GitHub-code-size-in-bytes-badge]
-[![GitHub-sponsors-badge]][GitHub-sponsors-page]
 
 | **A collection of monkey patches to improve Django framework** |
 
 
 ## Use
 
 Each monkey-patch `beautiful_patch` should be available
@@ -104,10 +103,7 @@
 
 [GitHub-license-badge]: https://img.shields.io/github/license/llyaudet/django-monkey-patches
 
 [PyPI-python-version-badge]: https://img.shields.io/pypi/pyversions/django-monkey-patches
 
 [GitHub-code-size-in-bytes-badge]: https://img.shields.io/github/languages/code-size/llyaudet/django-monkey-patches
 
-[GitHub-sponsors-badge]: https://img.shields.io/github/sponsors/LLyaudet
-
-[GitHub-sponsors-page]: https://github.com/sponsors/LLyaudet
```

### Comparing `django_monkey_patches-2.9.1/pyproject.toml` & `django_monkey_patches-3.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-monkey-patches"
-version = "2.9.1"
+version = "3.0.0"
 description = """\
 Add monkey-patches to correct and enhance your favorite framework\
 """
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
```

### Comparing `django_monkey_patches-2.9.1/PKG-INFO` & `django_monkey_patches-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-monkey-patches
-Version: 2.9.1
+Version: 3.0.0
 Summary: Add monkey-patches to correct and enhance your favorite framework
 Project-URL: Homepage, https://github.com/LLyaudet/django-monkey-patches
 Project-URL: Bug Tracker, https://github.com/LLyaudet/django-monkey-patches/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -194,15 +194,14 @@
 [![CodeFactor-badge]][CodeFactor-package-page]
 [![CodeClimateMaintainability-badge]][CodeClimateM13y-package-page]
 [![Codacy-badge]][Codacy-package-page]
 ![GitHub-top-language-badge]
 ![GitHub-license-badge]
 ![PyPI-python-version-badge]
 ![GitHub-code-size-in-bytes-badge]
-[![GitHub-sponsors-badge]][GitHub-sponsors-page]
 
 | **A collection of monkey patches to improve Django framework** |
 
 
 ## Use
 
 Each monkey-patch `beautiful_patch` should be available
@@ -290,10 +289,7 @@
 
 [GitHub-license-badge]: https://img.shields.io/github/license/llyaudet/django-monkey-patches
 
 [PyPI-python-version-badge]: https://img.shields.io/pypi/pyversions/django-monkey-patches
 
 [GitHub-code-size-in-bytes-badge]: https://img.shields.io/github/languages/code-size/llyaudet/django-monkey-patches
 
-[GitHub-sponsors-badge]: https://img.shields.io/github/sponsors/LLyaudet
-
-[GitHub-sponsors-page]: https://github.com/sponsors/LLyaudet
```

