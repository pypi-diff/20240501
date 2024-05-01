# Comparing `tmp/orquestra_sdk-0.62.0-py3-none-any.whl.zip` & `tmp/orquestra_sdk-0.63.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,114 +1,138 @@
-Zip file size: 224946 bytes, number of entries: 112
--rw-r--r--  2.0 unx     1911 b- defN 20-Feb-02 00:00 orquestra/sdk/__init__.py
--rw-r--r--  2.0 unx    10179 b- defN 20-Feb-02 00:00 orquestra/sdk/exceptions.py
+Zip file size: 237492 bytes, number of entries: 136
+-rw-r--r--  2.0 unx     2051 b- defN 20-Feb-02 00:00 orquestra/sdk/__init__.py
+-rw-r--r--  2.0 unx     2892 b- defN 20-Feb-02 00:00 orquestra/sdk/exceptions.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 orquestra/sdk/py.typed
--rw-r--r--  2.0 unx      204 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/__init__.py
--rw-r--r--  2.0 unx     8254 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_ast.py
--rw-r--r--  2.0 unx    16509 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_config.py
--rw-r--r--  2.0 unx     2880 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_dates.py
--rw-r--r--  2.0 unx    42709 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_dsl.py
--rw-r--r--  2.0 unx     3512 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_env.py
--rw-r--r--  2.0 unx     2155 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_exec_ctx.py
--rw-r--r--  2.0 unx     2577 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_factory.py
--rw-r--r--  2.0 unx     3774 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_git_url_utils.py
--rw-r--r--  2.0 unx     3858 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_graphs.py
--rw-r--r--  2.0 unx    14392 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_in_process_runtime.py
--rw-r--r--  2.0 unx     1484 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_jwt.py
--rw-r--r--  2.0 unx     1144 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_regex.py
--rw-r--r--  2.0 unx     1404 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_retry.py
--rw-r--r--  2.0 unx     4948 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_services.py
--rw-r--r--  2.0 unx    32576 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_traversal.py
--rw-r--r--  2.0 unx     4608 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_viz.py
--rw-r--r--  2.0 unx    23964 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_workflow.py
--rw-r--r--  2.0 unx     8458 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/abc.py
--rw-r--r--  2.0 unx     4826 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/dispatch.py
--rw-r--r--  2.0 unx     6168 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/loader.py
--rw-r--r--  2.0 unx     7032 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/serde.py
--rw-r--r--  2.0 unx      763 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_api/__init__.py
--rw-r--r--  2.0 unx    14594 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_api/_config.py
--rw-r--r--  2.0 unx    12860 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_api/_task_run.py
--rw-r--r--  2.0 unx    32163 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_api/_wf_run.py
--rw-r--r--  2.0 unx      204 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_driver/__init__.py
--rw-r--r--  2.0 unx    30006 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_driver/_ce_runtime.py
--rw-r--r--  2.0 unx    51898 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_driver/_client.py
--rw-r--r--  2.0 unx     6062 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_driver/_exceptions.py
--rw-r--r--  2.0 unx    17690 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_driver/_models.py
--rw-r--r--  2.0 unx     3247 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_logs/_interfaces.py
--rw-r--r--  2.0 unx     6791 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_logs/_markers.py
--rw-r--r--  2.0 unx     1326 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_logs/_models.py
--rw-r--r--  2.0 unx      849 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_logs/_regrouping.py
--rw-r--r--  2.0 unx      204 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_spaces/__init__.py
--rw-r--r--  2.0 unx     2728 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_spaces/_api.py
--rw-r--r--  2.0 unx     2357 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_spaces/_resolver.py
--rw-r--r--  2.0 unx      704 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_spaces/_structs.py
--rw-r--r--  2.0 unx      383 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_storage/__init__.py
--rw-r--r--  2.0 unx     4496 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_storage/orqdantic.py
--rw-r--r--  2.0 unx      204 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_testing/__init__.py
--rw-r--r--  2.0 unx     4061 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_testing/_connections.py
--rw-r--r--  2.0 unx     9430 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_testing/_example_wfs.py
--rw-r--r--  2.0 unx     1754 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_testing/_ipc.py
--rw-r--r--  2.0 unx      261 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_testing/_long_import.py
--rw-r--r--  2.0 unx      950 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/_testing/_reloaders.py
--rw-r--r--  2.0 unx    18206 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_arg_resolvers.py
--rw-r--r--  2.0 unx      697 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_cli_logs.py
--rw-r--r--  2.0 unx     4350 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_dumpers.py
--rw-r--r--  2.0 unx    13592 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_entry.py
--rw-r--r--  2.0 unx    31566 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_repos.py
--rw-r--r--  2.0 unx     2209 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_config/_list.py
--rw-r--r--  2.0 unx     5381 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_login/_login.py
--rw-r--r--  2.0 unx     1749 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_login/_login_server.py
--rw-r--r--  2.0 unx     2645 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_services/_down.py
--rw-r--r--  2.0 unx     1323 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_services/_status.py
--rw-r--r--  2.0 unx     2574 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_services/_up.py
--rw-r--r--  2.0 unx     3226 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_task/_logs.py
--rw-r--r--  2.0 unx     3614 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_task/_results.py
--rw-r--r--  2.0 unx      373 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_ui/__init__.py
--rw-r--r--  2.0 unx     6308 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_ui/_click_default_group.py
--rw-r--r--  2.0 unx     8358 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_ui/_errors.py
--rw-r--r--  2.0 unx     1686 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_ui/_models.py
--rw-r--r--  2.0 unx    17739 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_ui/_presenters.py
--rw-r--r--  2.0 unx    10907 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_ui/_prompts.py
--rw-r--r--  2.0 unx     3983 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_workflow/_list.py
--rw-r--r--  2.0 unx     4105 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_workflow/_logs.py
--rw-r--r--  2.0 unx     3128 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_workflow/_results.py
--rw-r--r--  2.0 unx     2594 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_workflow/_stop.py
--rw-r--r--  2.0 unx     5198 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_workflow/_submit.py
--rw-r--r--  2.0 unx     2132 b- defN 20-Feb-02 00:00 orquestra/sdk/_base/cli/_workflow/_view.py
--rw-r--r--  2.0 unx      204 b- defN 20-Feb-02 00:00 orquestra/sdk/_ray/__init__.py
--rw-r--r--  2.0 unx    25840 b- defN 20-Feb-02 00:00 orquestra/sdk/_ray/_build_workflow.py
--rw-r--r--  2.0 unx     8255 b- defN 20-Feb-02 00:00 orquestra/sdk/_ray/_client.py
--rw-r--r--  2.0 unx    30665 b- defN 20-Feb-02 00:00 orquestra/sdk/_ray/_dag.py
--rw-r--r--  2.0 unx      946 b- defN 20-Feb-02 00:00 orquestra/sdk/_ray/_id_gen.py
--rw-r--r--  2.0 unx     9527 b- defN 20-Feb-02 00:00 orquestra/sdk/_ray/_ray_logs.py
--rw-r--r--  2.0 unx     1482 b- defN 20-Feb-02 00:00 orquestra/sdk/_ray/_wf_metadata.py
--rw-r--r--  2.0 unx      341 b- defN 20-Feb-02 00:00 orquestra/sdk/dremio/__init__.py
--rw-r--r--  2.0 unx     2916 b- defN 20-Feb-02 00:00 orquestra/sdk/dremio/_api.py
--rw-r--r--  2.0 unx      832 b- defN 20-Feb-02 00:00 orquestra/sdk/dremio/_env_var_reader.py
--rw-r--r--  2.0 unx      662 b- defN 20-Feb-02 00:00 orquestra/sdk/dremio/_flight_facade.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/__init__.py
+-rw-r--r--  2.0 unx      204 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/__init__.py
+-rw-r--r--  2.0 unx     8110 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_ast.py
+-rw-r--r--  2.0 unx    16525 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_config.py
+-rw-r--r--  2.0 unx    47276 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_dsl.py
+-rw-r--r--  2.0 unx     2414 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_env.py
+-rw-r--r--  2.0 unx     2683 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_factory.py
+-rw-r--r--  2.0 unx     2085 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_git_url_utils.py
+-rw-r--r--  2.0 unx    14448 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_in_process_runtime.py
+-rw-r--r--  2.0 unx     1504 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_jwt.py
+-rw-r--r--  2.0 unx     1404 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_retry.py
+-rw-r--r--  2.0 unx     3678 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_services.py
+-rw-r--r--  2.0 unx    32711 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_traversal.py
+-rw-r--r--  2.0 unx     4616 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_viz.py
+-rw-r--r--  2.0 unx    24596 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_workflow.py
+-rw-r--r--  2.0 unx     6188 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/loader.py
+-rw-r--r--  2.0 unx      878 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_api/__init__.py
+-rw-r--r--  2.0 unx    14647 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_api/_config.py
+-rw-r--r--  2.0 unx    12987 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_api/_task_run.py
+-rw-r--r--  2.0 unx    34562 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_api/_wf_run.py
+-rw-r--r--  2.0 unx      204 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_driver/__init__.py
+-rw-r--r--  2.0 unx    30007 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_driver/_ce_runtime.py
+-rw-r--r--  2.0 unx    51919 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_driver/_client.py
+-rw-r--r--  2.0 unx     6062 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_driver/_exceptions.py
+-rw-r--r--  2.0 unx    17720 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_driver/_models.py
+-rw-r--r--  2.0 unx      204 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_spaces/__init__.py
+-rw-r--r--  2.0 unx     2786 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_spaces/_api.py
+-rw-r--r--  2.0 unx     2385 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_spaces/_resolver.py
+-rw-r--r--  2.0 unx      204 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_testing/__init__.py
+-rw-r--r--  2.0 unx     4266 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_testing/_connections.py
+-rw-r--r--  2.0 unx     9817 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_testing/_example_wfs.py
+-rw-r--r--  2.0 unx     1754 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_testing/_ipc.py
+-rw-r--r--  2.0 unx      261 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_testing/_long_import.py
+-rw-r--r--  2.0 unx      950 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/_testing/_reloaders.py
+-rw-r--r--  2.0 unx    18205 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_arg_resolvers.py
+-rw-r--r--  2.0 unx      686 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_cli_logs.py
+-rw-r--r--  2.0 unx     5494 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_dumpers.py
+-rw-r--r--  2.0 unx    13768 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_entry.py
+-rw-r--r--  2.0 unx    31605 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_repos.py
+-rw-r--r--  2.0 unx     2200 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_config/_list.py
+-rw-r--r--  2.0 unx     5397 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_login/_login.py
+-rw-r--r--  2.0 unx     1749 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_login/_login_server.py
+-rw-r--r--  2.0 unx     2653 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_services/_down.py
+-rw-r--r--  2.0 unx     1331 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_services/_status.py
+-rw-r--r--  2.0 unx     2582 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_services/_up.py
+-rw-r--r--  2.0 unx     3288 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_task/_logs.py
+-rw-r--r--  2.0 unx     3630 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_task/_results.py
+-rw-r--r--  2.0 unx      373 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_ui/__init__.py
+-rw-r--r--  2.0 unx     6308 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_ui/_click_default_group.py
+-rw-r--r--  2.0 unx     8365 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_ui/_errors.py
+-rw-r--r--  2.0 unx     1703 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_ui/_models.py
+-rw-r--r--  2.0 unx    17802 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_ui/_presenters.py
+-rw-r--r--  2.0 unx    10915 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_ui/_prompts.py
+-rw-r--r--  2.0 unx     4007 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_workflow/_list.py
+-rw-r--r--  2.0 unx     4205 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_workflow/_logs.py
+-rw-r--r--  2.0 unx     3144 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_workflow/_results.py
+-rw-r--r--  2.0 unx     2618 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_workflow/_stop.py
+-rw-r--r--  2.0 unx     5206 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_workflow/_submit.py
+-rw-r--r--  2.0 unx     2148 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/_base/cli/_workflow/_view.py
+-rw-r--r--  2.0 unx      341 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/dremio/__init__.py
+-rw-r--r--  2.0 unx     2916 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/dremio/_api.py
+-rw-r--r--  2.0 unx      840 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/dremio/_env_var_reader.py
+-rw-r--r--  2.0 unx      662 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/dremio/_flight_facade.py
+-rw-r--r--  2.0 unx      528 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/mlflow/__init__.py
+-rw-r--r--  2.0 unx     8903 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/mlflow/_connection_utils.py
+-rw-r--r--  2.0 unx     1102 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/secrets/__init__.py
+-rw-r--r--  2.0 unx     7717 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/secrets/_api.py
+-rw-r--r--  2.0 unx     2516 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/secrets/_auth.py
+-rw-r--r--  2.0 unx     8350 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/secrets/_client.py
+-rw-r--r--  2.0 unx     1249 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/secrets/_exceptions.py
+-rw-r--r--  2.0 unx     1782 b- defN 20-Feb-02 00:00 orquestra/sdk/_client/secrets/_models.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 orquestra/sdk/_ray/__init__.py
+-rw-r--r--  2.0 unx      436 b- defN 20-Feb-02 00:00 orquestra/sdk/_ray/_build_workflow.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 orquestra/sdk/_runtime/__init__.py
+-rw-r--r--  2.0 unx      204 b- defN 20-Feb-02 00:00 orquestra/sdk/_runtime/_ray/__init__.py
+-rw-r--r--  2.0 unx    27980 b- defN 20-Feb-02 00:00 orquestra/sdk/_runtime/_ray/_build_workflow.py
+-rw-r--r--  2.0 unx     8263 b- defN 20-Feb-02 00:00 orquestra/sdk/_runtime/_ray/_client.py
+-rw-r--r--  2.0 unx    30785 b- defN 20-Feb-02 00:00 orquestra/sdk/_runtime/_ray/_dag.py
+-rw-r--r--  2.0 unx     1458 b- defN 20-Feb-02 00:00 orquestra/sdk/_runtime/_ray/_dirs.py
+-rw-r--r--  2.0 unx     1096 b- defN 20-Feb-02 00:00 orquestra/sdk/_runtime/_ray/_env.py
+-rw-r--r--  2.0 unx      946 b- defN 20-Feb-02 00:00 orquestra/sdk/_runtime/_ray/_id_gen.py
+-rw-r--r--  2.0 unx     9463 b- defN 20-Feb-02 00:00 orquestra/sdk/_runtime/_ray/_ray_logs.py
+-rw-r--r--  2.0 unx     1517 b- defN 20-Feb-02 00:00 orquestra/sdk/_runtime/_ray/_wf_metadata.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 orquestra/sdk/_runtime/_ray/_logs/__init__.py
+-rw-r--r--  2.0 unx     7022 b- defN 20-Feb-02 00:00 orquestra/sdk/_runtime/_ray/_logs/_markers.py
+-rw-r--r--  2.0 unx      296 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/__init__.py
+-rw-r--r--  2.0 unx     3845 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/_graphs.py
+-rw-r--r--  2.0 unx     1144 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/_regex.py
+-rw-r--r--  2.0 unx     8454 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/abc.py
+-rw-r--r--  2.0 unx     4796 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/dispatch.py
+-rw-r--r--  2.0 unx    10212 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/exceptions.py
+-rw-r--r--  2.0 unx     7012 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/serde.py
+-rw-r--r--  2.0 unx      103 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/_spaces/__init__.py
+-rw-r--r--  2.0 unx      692 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/_spaces/_structs.py
+-rw-r--r--  2.0 unx      355 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/dates/__init__.py
+-rw-r--r--  2.0 unx     2880 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/dates/_dates.py
+-rw-r--r--  2.0 unx      181 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/exec_ctx/__init__.py
+-rw-r--r--  2.0 unx     2155 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/exec_ctx/_exec_ctx.py
+-rw-r--r--  2.0 unx      318 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/kubernetes/__init__.py
+-rw-r--r--  2.0 unx     2449 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/kubernetes/quantity.py
+-rw-r--r--  2.0 unx      309 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/logs/__init__.py
+-rw-r--r--  2.0 unx     3223 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/logs/_interfaces.py
+-rw-r--r--  2.0 unx     1326 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/logs/_models.py
+-rw-r--r--  2.0 unx      849 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/logs/_regrouping.py
+-rw-r--r--  2.0 unx      383 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/orqdantic/__init__.py
+-rw-r--r--  2.0 unx     4496 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/orqdantic/orqdantic.py
+-rw-r--r--  2.0 unx      471 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/packaging/__init__.py
+-rw-r--r--  2.0 unx     2235 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/packaging/_versions.py
+-rw-r--r--  2.0 unx      274 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/schema/__init__.py
+-rw-r--r--  2.0 unx     1472 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/schema/_compat.py
+-rw-r--r--  2.0 unx     1625 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/schema/configs.py
+-rw-r--r--  2.0 unx    15413 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/schema/ir.py
+-rw-r--r--  2.0 unx     2132 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/schema/responses.py
+-rw-r--r--  2.0 unx     2955 b- defN 20-Feb-02 00:00 orquestra/sdk/_shared/schema/workflow_run.py
+-rw-r--r--  2.0 unx      377 b- defN 20-Feb-02 00:00 orquestra/sdk/dremio/__init__.py
 -rw-r--r--  2.0 unx      204 b- defN 20-Feb-02 00:00 orquestra/sdk/examples/__init__.py
--rw-r--r--  2.0 unx     1590 b- defN 20-Feb-02 00:00 orquestra/sdk/examples/exportable_wf.py
+-rw-r--r--  2.0 unx     1572 b- defN 20-Feb-02 00:00 orquestra/sdk/examples/exportable_wf.py
 -rw-r--r--  2.0 unx     1075 b- defN 20-Feb-02 00:00 orquestra/sdk/examples/workflow_defs.py
--rw-r--r--  2.0 unx      318 b- defN 20-Feb-02 00:00 orquestra/sdk/kubernetes/__init__.py
--rw-r--r--  2.0 unx     2449 b- defN 20-Feb-02 00:00 orquestra/sdk/kubernetes/quantity.py
--rw-r--r--  2.0 unx      528 b- defN 20-Feb-02 00:00 orquestra/sdk/mlflow/__init__.py
--rw-r--r--  2.0 unx     8966 b- defN 20-Feb-02 00:00 orquestra/sdk/mlflow/_connection_utils.py
--rw-r--r--  2.0 unx      427 b- defN 20-Feb-02 00:00 orquestra/sdk/packaging/__init__.py
--rw-r--r--  2.0 unx     4139 b- defN 20-Feb-02 00:00 orquestra/sdk/packaging/_versions.py
--rw-r--r--  2.0 unx      204 b- defN 20-Feb-02 00:00 orquestra/sdk/schema/__init__.py
--rw-r--r--  2.0 unx     1472 b- defN 20-Feb-02 00:00 orquestra/sdk/schema/_compat.py
--rw-r--r--  2.0 unx     1630 b- defN 20-Feb-02 00:00 orquestra/sdk/schema/configs.py
--rw-r--r--  2.0 unx    15293 b- defN 20-Feb-02 00:00 orquestra/sdk/schema/ir.py
--rw-r--r--  2.0 unx     2137 b- defN 20-Feb-02 00:00 orquestra/sdk/schema/responses.py
--rw-r--r--  2.0 unx     3000 b- defN 20-Feb-02 00:00 orquestra/sdk/schema/workflow_run.py
--rw-r--r--  2.0 unx     1102 b- defN 20-Feb-02 00:00 orquestra/sdk/secrets/__init__.py
--rw-r--r--  2.0 unx     7595 b- defN 20-Feb-02 00:00 orquestra/sdk/secrets/_api.py
--rw-r--r--  2.0 unx     2500 b- defN 20-Feb-02 00:00 orquestra/sdk/secrets/_auth.py
--rw-r--r--  2.0 unx     8350 b- defN 20-Feb-02 00:00 orquestra/sdk/secrets/_client.py
--rw-r--r--  2.0 unx     1249 b- defN 20-Feb-02 00:00 orquestra/sdk/secrets/_exceptions.py
--rw-r--r--  2.0 unx     1767 b- defN 20-Feb-02 00:00 orquestra/sdk/secrets/_models.py
-?rw-r--r--  2.0 unx    17501 b- defN 20-Feb-02 00:00 orquestra_sdk-0.62.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 orquestra_sdk-0.62.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx       60 b- defN 20-Feb-02 00:00 orquestra_sdk-0.62.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    11357 b- defN 20-Feb-02 00:00 orquestra_sdk-0.62.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx    10324 b- defN 20-Feb-02 00:00 orquestra_sdk-0.62.0.dist-info/RECORD
-112 files, 760148 bytes uncompressed, 208410 bytes compressed:  72.6%
+-rw-r--r--  2.0 unx      299 b- defN 20-Feb-02 00:00 orquestra/sdk/kubernetes/__init__.py
+-rw-r--r--  2.0 unx      399 b- defN 20-Feb-02 00:00 orquestra/sdk/kubernetes/quantity.py
+-rw-r--r--  2.0 unx      548 b- defN 20-Feb-02 00:00 orquestra/sdk/mlflow/__init__.py
+-rw-r--r--  2.0 unx      437 b- defN 20-Feb-02 00:00 orquestra/sdk/packaging/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 orquestra/sdk/schema/__init__.py
+-rw-r--r--  2.0 unx      662 b- defN 20-Feb-02 00:00 orquestra/sdk/schema/configs.py
+-rw-r--r--  2.0 unx     1789 b- defN 20-Feb-02 00:00 orquestra/sdk/schema/ir.py
+-rw-r--r--  2.0 unx      734 b- defN 20-Feb-02 00:00 orquestra/sdk/schema/responses.py
+-rw-r--r--  2.0 unx      781 b- defN 20-Feb-02 00:00 orquestra/sdk/schema/workflow_run.py
+-rw-r--r--  2.0 unx      428 b- defN 20-Feb-02 00:00 orquestra/sdk/secrets/__init__.py
+?rw-r--r--  2.0 unx    18219 b- defN 20-Feb-02 00:00 orquestra_sdk-0.63.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 orquestra_sdk-0.63.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx       68 b- defN 20-Feb-02 00:00 orquestra_sdk-0.63.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    11357 b- defN 20-Feb-02 00:00 orquestra_sdk-0.63.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx    13253 b- defN 20-Feb-02 00:00 orquestra_sdk-0.63.0.dist-info/RECORD
+136 files, 784800 bytes uncompressed, 215950 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -3,335 +3,407 @@
 
 Filename: orquestra/sdk/exceptions.py
 Comment: 
 
 Filename: orquestra/sdk/py.typed
 Comment: 
 
-Filename: orquestra/sdk/_base/__init__.py
+Filename: orquestra/sdk/_client/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_ast.py
+Filename: orquestra/sdk/_client/_base/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_config.py
+Filename: orquestra/sdk/_client/_base/_ast.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_dates.py
+Filename: orquestra/sdk/_client/_base/_config.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_dsl.py
+Filename: orquestra/sdk/_client/_base/_dsl.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_env.py
+Filename: orquestra/sdk/_client/_base/_env.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_exec_ctx.py
+Filename: orquestra/sdk/_client/_base/_factory.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_factory.py
+Filename: orquestra/sdk/_client/_base/_git_url_utils.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_git_url_utils.py
+Filename: orquestra/sdk/_client/_base/_in_process_runtime.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_graphs.py
+Filename: orquestra/sdk/_client/_base/_jwt.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_in_process_runtime.py
+Filename: orquestra/sdk/_client/_base/_retry.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_jwt.py
+Filename: orquestra/sdk/_client/_base/_services.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_regex.py
+Filename: orquestra/sdk/_client/_base/_traversal.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_retry.py
+Filename: orquestra/sdk/_client/_base/_viz.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_services.py
+Filename: orquestra/sdk/_client/_base/_workflow.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_traversal.py
+Filename: orquestra/sdk/_client/_base/loader.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_viz.py
+Filename: orquestra/sdk/_client/_base/_api/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_workflow.py
+Filename: orquestra/sdk/_client/_base/_api/_config.py
 Comment: 
 
-Filename: orquestra/sdk/_base/abc.py
+Filename: orquestra/sdk/_client/_base/_api/_task_run.py
 Comment: 
 
-Filename: orquestra/sdk/_base/dispatch.py
+Filename: orquestra/sdk/_client/_base/_api/_wf_run.py
 Comment: 
 
-Filename: orquestra/sdk/_base/loader.py
+Filename: orquestra/sdk/_client/_base/_driver/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/_base/serde.py
+Filename: orquestra/sdk/_client/_base/_driver/_ce_runtime.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_api/__init__.py
+Filename: orquestra/sdk/_client/_base/_driver/_client.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_api/_config.py
+Filename: orquestra/sdk/_client/_base/_driver/_exceptions.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_api/_task_run.py
+Filename: orquestra/sdk/_client/_base/_driver/_models.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_api/_wf_run.py
+Filename: orquestra/sdk/_client/_base/_spaces/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_driver/__init__.py
+Filename: orquestra/sdk/_client/_base/_spaces/_api.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_driver/_ce_runtime.py
+Filename: orquestra/sdk/_client/_base/_spaces/_resolver.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_driver/_client.py
+Filename: orquestra/sdk/_client/_base/_testing/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_driver/_exceptions.py
+Filename: orquestra/sdk/_client/_base/_testing/_connections.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_driver/_models.py
+Filename: orquestra/sdk/_client/_base/_testing/_example_wfs.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_logs/_interfaces.py
+Filename: orquestra/sdk/_client/_base/_testing/_ipc.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_logs/_markers.py
+Filename: orquestra/sdk/_client/_base/_testing/_long_import.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_logs/_models.py
+Filename: orquestra/sdk/_client/_base/_testing/_reloaders.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_logs/_regrouping.py
+Filename: orquestra/sdk/_client/_base/cli/_arg_resolvers.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_spaces/__init__.py
+Filename: orquestra/sdk/_client/_base/cli/_cli_logs.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_spaces/_api.py
+Filename: orquestra/sdk/_client/_base/cli/_dumpers.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_spaces/_resolver.py
+Filename: orquestra/sdk/_client/_base/cli/_entry.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_spaces/_structs.py
+Filename: orquestra/sdk/_client/_base/cli/_repos.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_storage/__init__.py
+Filename: orquestra/sdk/_client/_base/cli/_config/_list.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_storage/orqdantic.py
+Filename: orquestra/sdk/_client/_base/cli/_login/_login.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_testing/__init__.py
+Filename: orquestra/sdk/_client/_base/cli/_login/_login_server.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_testing/_connections.py
+Filename: orquestra/sdk/_client/_base/cli/_services/_down.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_testing/_example_wfs.py
+Filename: orquestra/sdk/_client/_base/cli/_services/_status.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_testing/_ipc.py
+Filename: orquestra/sdk/_client/_base/cli/_services/_up.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_testing/_long_import.py
+Filename: orquestra/sdk/_client/_base/cli/_task/_logs.py
 Comment: 
 
-Filename: orquestra/sdk/_base/_testing/_reloaders.py
+Filename: orquestra/sdk/_client/_base/cli/_task/_results.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_arg_resolvers.py
+Filename: orquestra/sdk/_client/_base/cli/_ui/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_cli_logs.py
+Filename: orquestra/sdk/_client/_base/cli/_ui/_click_default_group.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_dumpers.py
+Filename: orquestra/sdk/_client/_base/cli/_ui/_errors.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_entry.py
+Filename: orquestra/sdk/_client/_base/cli/_ui/_models.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_repos.py
+Filename: orquestra/sdk/_client/_base/cli/_ui/_presenters.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_config/_list.py
+Filename: orquestra/sdk/_client/_base/cli/_ui/_prompts.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_login/_login.py
+Filename: orquestra/sdk/_client/_base/cli/_workflow/_list.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_login/_login_server.py
+Filename: orquestra/sdk/_client/_base/cli/_workflow/_logs.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_services/_down.py
+Filename: orquestra/sdk/_client/_base/cli/_workflow/_results.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_services/_status.py
+Filename: orquestra/sdk/_client/_base/cli/_workflow/_stop.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_services/_up.py
+Filename: orquestra/sdk/_client/_base/cli/_workflow/_submit.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_task/_logs.py
+Filename: orquestra/sdk/_client/_base/cli/_workflow/_view.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_task/_results.py
+Filename: orquestra/sdk/_client/dremio/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_ui/__init__.py
+Filename: orquestra/sdk/_client/dremio/_api.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_ui/_click_default_group.py
+Filename: orquestra/sdk/_client/dremio/_env_var_reader.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_ui/_errors.py
+Filename: orquestra/sdk/_client/dremio/_flight_facade.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_ui/_models.py
+Filename: orquestra/sdk/_client/mlflow/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_ui/_presenters.py
+Filename: orquestra/sdk/_client/mlflow/_connection_utils.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_ui/_prompts.py
+Filename: orquestra/sdk/_client/secrets/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_workflow/_list.py
+Filename: orquestra/sdk/_client/secrets/_api.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_workflow/_logs.py
+Filename: orquestra/sdk/_client/secrets/_auth.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_workflow/_results.py
+Filename: orquestra/sdk/_client/secrets/_client.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_workflow/_stop.py
+Filename: orquestra/sdk/_client/secrets/_exceptions.py
 Comment: 
 
-Filename: orquestra/sdk/_base/cli/_workflow/_submit.py
-Comment: 
-
-Filename: orquestra/sdk/_base/cli/_workflow/_view.py
+Filename: orquestra/sdk/_client/secrets/_models.py
 Comment: 
 
 Filename: orquestra/sdk/_ray/__init__.py
 Comment: 
 
 Filename: orquestra/sdk/_ray/_build_workflow.py
 Comment: 
 
-Filename: orquestra/sdk/_ray/_client.py
+Filename: orquestra/sdk/_runtime/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/_ray/_dag.py
+Filename: orquestra/sdk/_runtime/_ray/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/_ray/_id_gen.py
+Filename: orquestra/sdk/_runtime/_ray/_build_workflow.py
 Comment: 
 
-Filename: orquestra/sdk/_ray/_ray_logs.py
+Filename: orquestra/sdk/_runtime/_ray/_client.py
 Comment: 
 
-Filename: orquestra/sdk/_ray/_wf_metadata.py
+Filename: orquestra/sdk/_runtime/_ray/_dag.py
 Comment: 
 
-Filename: orquestra/sdk/dremio/__init__.py
+Filename: orquestra/sdk/_runtime/_ray/_dirs.py
 Comment: 
 
-Filename: orquestra/sdk/dremio/_api.py
+Filename: orquestra/sdk/_runtime/_ray/_env.py
 Comment: 
 
-Filename: orquestra/sdk/dremio/_env_var_reader.py
+Filename: orquestra/sdk/_runtime/_ray/_id_gen.py
 Comment: 
 
-Filename: orquestra/sdk/dremio/_flight_facade.py
+Filename: orquestra/sdk/_runtime/_ray/_ray_logs.py
 Comment: 
 
-Filename: orquestra/sdk/examples/__init__.py
+Filename: orquestra/sdk/_runtime/_ray/_wf_metadata.py
 Comment: 
 
-Filename: orquestra/sdk/examples/exportable_wf.py
+Filename: orquestra/sdk/_runtime/_ray/_logs/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/examples/workflow_defs.py
+Filename: orquestra/sdk/_runtime/_ray/_logs/_markers.py
 Comment: 
 
-Filename: orquestra/sdk/kubernetes/__init__.py
+Filename: orquestra/sdk/_shared/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/kubernetes/quantity.py
+Filename: orquestra/sdk/_shared/_graphs.py
 Comment: 
 
-Filename: orquestra/sdk/mlflow/__init__.py
+Filename: orquestra/sdk/_shared/_regex.py
 Comment: 
 
-Filename: orquestra/sdk/mlflow/_connection_utils.py
+Filename: orquestra/sdk/_shared/abc.py
 Comment: 
 
-Filename: orquestra/sdk/packaging/__init__.py
+Filename: orquestra/sdk/_shared/dispatch.py
 Comment: 
 
-Filename: orquestra/sdk/packaging/_versions.py
+Filename: orquestra/sdk/_shared/exceptions.py
 Comment: 
 
-Filename: orquestra/sdk/schema/__init__.py
+Filename: orquestra/sdk/_shared/serde.py
 Comment: 
 
-Filename: orquestra/sdk/schema/_compat.py
+Filename: orquestra/sdk/_shared/_spaces/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/schema/configs.py
+Filename: orquestra/sdk/_shared/_spaces/_structs.py
 Comment: 
 
-Filename: orquestra/sdk/schema/ir.py
+Filename: orquestra/sdk/_shared/dates/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/schema/responses.py
+Filename: orquestra/sdk/_shared/dates/_dates.py
 Comment: 
 
-Filename: orquestra/sdk/schema/workflow_run.py
+Filename: orquestra/sdk/_shared/exec_ctx/__init__.py
 Comment: 
 
-Filename: orquestra/sdk/secrets/__init__.py
+Filename: orquestra/sdk/_shared/exec_ctx/_exec_ctx.py
+Comment: 
+
+Filename: orquestra/sdk/_shared/kubernetes/__init__.py
+Comment: 
+
+Filename: orquestra/sdk/_shared/kubernetes/quantity.py
+Comment: 
+
+Filename: orquestra/sdk/_shared/logs/__init__.py
+Comment: 
+
+Filename: orquestra/sdk/_shared/logs/_interfaces.py
+Comment: 
+
+Filename: orquestra/sdk/_shared/logs/_models.py
+Comment: 
+
+Filename: orquestra/sdk/_shared/logs/_regrouping.py
+Comment: 
+
+Filename: orquestra/sdk/_shared/orqdantic/__init__.py
+Comment: 
+
+Filename: orquestra/sdk/_shared/orqdantic/orqdantic.py
+Comment: 
+
+Filename: orquestra/sdk/_shared/packaging/__init__.py
+Comment: 
+
+Filename: orquestra/sdk/_shared/packaging/_versions.py
+Comment: 
+
+Filename: orquestra/sdk/_shared/schema/__init__.py
+Comment: 
+
+Filename: orquestra/sdk/_shared/schema/_compat.py
 Comment: 
 
-Filename: orquestra/sdk/secrets/_api.py
+Filename: orquestra/sdk/_shared/schema/configs.py
 Comment: 
 
-Filename: orquestra/sdk/secrets/_auth.py
+Filename: orquestra/sdk/_shared/schema/ir.py
 Comment: 
 
-Filename: orquestra/sdk/secrets/_client.py
+Filename: orquestra/sdk/_shared/schema/responses.py
 Comment: 
 
-Filename: orquestra/sdk/secrets/_exceptions.py
+Filename: orquestra/sdk/_shared/schema/workflow_run.py
 Comment: 
 
-Filename: orquestra/sdk/secrets/_models.py
+Filename: orquestra/sdk/dremio/__init__.py
+Comment: 
+
+Filename: orquestra/sdk/examples/__init__.py
+Comment: 
+
+Filename: orquestra/sdk/examples/exportable_wf.py
+Comment: 
+
+Filename: orquestra/sdk/examples/workflow_defs.py
+Comment: 
+
+Filename: orquestra/sdk/kubernetes/__init__.py
+Comment: 
+
+Filename: orquestra/sdk/kubernetes/quantity.py
+Comment: 
+
+Filename: orquestra/sdk/mlflow/__init__.py
+Comment: 
+
+Filename: orquestra/sdk/packaging/__init__.py
+Comment: 
+
+Filename: orquestra/sdk/schema/__init__.py
+Comment: 
+
+Filename: orquestra/sdk/schema/configs.py
+Comment: 
+
+Filename: orquestra/sdk/schema/ir.py
+Comment: 
+
+Filename: orquestra/sdk/schema/responses.py
+Comment: 
+
+Filename: orquestra/sdk/schema/workflow_run.py
+Comment: 
+
+Filename: orquestra/sdk/secrets/__init__.py
 Comment: 
 
-Filename: orquestra_sdk-0.62.0.dist-info/METADATA
+Filename: orquestra_sdk-0.63.0.dist-info/METADATA
 Comment: 
 
-Filename: orquestra_sdk-0.62.0.dist-info/WHEEL
+Filename: orquestra_sdk-0.63.0.dist-info/WHEEL
 Comment: 
 
-Filename: orquestra_sdk-0.62.0.dist-info/entry_points.txt
+Filename: orquestra_sdk-0.63.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: orquestra_sdk-0.62.0.dist-info/licenses/LICENSE
+Filename: orquestra_sdk-0.63.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: orquestra_sdk-0.62.0.dist-info/RECORD
+Filename: orquestra_sdk-0.63.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orquestra/sdk/__init__.py

```diff
@@ -1,46 +1,53 @@
 ################################################################################
-# © Copyright 2021-2023 Zapata Computing Inc.
+# © Copyright 2021-2024 Zapata Computing Inc.
 ################################################################################
 """Orquestra SDK allows to define computational workflows using Python DSL."""
 
-from . import mlflow, secrets
-from ._base._api import (
+from ._client import mlflow, secrets
+from ._client._base._api import (
+    CurrentExecutionCtx,
     CurrentRunIDs,
     RuntimeConfig,
     TaskRun,
     WorkflowRun,
+    current_exec_ctx,
     current_run_ids,
     list_workflow_run_summaries,
     list_workflow_runs,
     migrate_config_file,
 )
-from ._base._dsl import (
+from ._client._base._dsl import (
     ArtifactFuture,
     DataAggregation,
     GithubImport,
     GitImport,
     GitImportWithAuth,
     Import,
     InlineImport,
     LocalImport,
     PythonImports,
     Resources,
     Secret,
     TaskDef,
     task,
 )
-from ._base._logs._interfaces import LogOutput, WorkflowLogs
-from ._base._spaces._api import list_projects, list_workspaces
-from ._base._spaces._structs import Project, ProjectRef, Workspace
-from ._base._workflow import NotATaskWarning, WorkflowDef, WorkflowTemplate, workflow
+from ._client._base._spaces._api import list_projects, list_workspaces
+from ._client._base._workflow import (
+    NotATaskWarning,
+    WorkflowDef,
+    WorkflowTemplate,
+    workflow,
+)
+from ._shared import Project, ProjectRef, Workspace
+from ._shared.logs import LogOutput, WorkflowLogs
 
 # It's already in a public module, but we'll re-export it under `orquestra.sdk.*` anyway
 # because it's commonly used to filter task runs.
-from .schema.workflow_run import State
+from ._shared.schema.workflow_run import State
 
 __all__ = [
     "ArtifactFuture",
     "DataAggregation",
     "current_run_ids",
     "GithubImport",
     "GitImport",
@@ -70,8 +77,10 @@
     "workflow",
     "Project",
     "ProjectRef",
     "State",
     "Workspace",
     "CurrentRunIDs",
     "LogOutput",
+    "CurrentExecutionCtx",
+    "current_exec_ctx",
 ]
```

## orquestra/sdk/exceptions.py

```diff
@@ -1,359 +1,99 @@
 ################################################################################
-# © Copyright 2022-2023 Zapata Computing Inc.
+# © Copyright 2024 Zapata Computing Inc.
 ################################################################################
+# THIS FILE IS A SHIM TO REEXPORT SYMBOLS AS PUBLIC API
+# DO NOT PUT ANY LOGIC INTO THIS FILE.
 
-"""Custom exceptions for the SDK."""
-
-import typing as t
-from dataclasses import dataclass
-
-from orquestra.sdk.schema import configs, ir
-from orquestra.sdk.schema.workflow_run import State, TaskInvocationId, WorkflowRunId
-
-
-class WorkflowSyntaxError(Exception):
-    """Raised when there is a syntax error in the workflow definition."""
-
-    def __init__(self, msg: str):
-        super().__init__(msg)
-        self.msg = msg
-
-
-class VersionMismatch(Warning):
-    def __init__(self, msg: str, actual: ir.Version, needed: t.Optional[ir.Version]):
-        super().__init__(msg)
-        self.actual = actual
-        self.needed = needed
-
-
-class DirtyGitRepo(Warning):
-    """Raised when there are uncommitted changes in the git repo."""
-
-    pass
-
-
-class BaseRuntimeError(Exception):
-    """Base class for runtime errors."""
-
-    def __init__(self, message: t.Optional[str] = None):
-        super().__init__(message)
-        self.message = message
-
-
-# Generic
-class NotFoundError(BaseRuntimeError):
-    """Raised when the specified runtime, workflow, result, or artifact is not found."""
-
-    pass
-
-
-class UserTaskFailedError(BaseRuntimeError):
-    """Raised when a task run fails during execution.
-
-    The actual exception that stopped the task from execution is chained as
-    ``raise TaskRunFailedError(...) from e``. This is a workaround for
-    de/serialization of exceptions defined in 3rd-party libraries.
-    """
-
-    def __init__(
-        self,
-        msg: str,
-        wf_run_id: WorkflowRunId = "",
-        task_inv_id: TaskInvocationId = "",
-    ):
-        super().__init__(msg)
-        self.wf_run_id = wf_run_id
-        self.task_inv_id = task_inv_id
-
-
-# Config Errors
-class ConfigFileNotFoundError(BaseRuntimeError):
-    """Raised when the configuration file cannot be identified."""
-
-    pass
-
-
-class ConfigNameNotFoundError(BaseRuntimeError):
-    """Raised if the specified config is not stored in the config file."""
-
-    pass
-
-
-class EnvVarNotFoundError(NotFoundError):
-    """Raised when the required environment variable's value couldn't be read."""
-
-    def __init__(self, msg: str, var_name: str):
-        super().__init__(msg)
-        self.var_name = var_name
-
-
-class RuntimeConfigError(BaseRuntimeError):
-    """Raised when one or more configuration options do not relate to the runtime."""
-
-    pass
-
-
-class LocalConfigLoginError(BaseRuntimeError):
-    """Raised when trying to log in using a config that relates to local execution."""
-
-    pass
-
-
-class QERemoved(BaseRuntimeError):
-    """Raised when attempting to use QE."""
-
-
-# Workflow Definition Errors
-class WorkflowDefinitionModuleNotFound(NotFoundError):
-    """Raised when loading workflow definitions module failed."""
-
-    def __init__(self, module_name: str, sys_path: t.Sequence[str]):
-        self.module_name = module_name
-        # 'sys.path' is often mutated. Let's guard against this action-at-a-distance.
-        self.sys_path = list(sys_path)
-
-
-class NoWorkflowDefinitionsFound(NotFoundError):
-    """Raised when there's no workflow definitions in the specified module."""
-
-    def __init__(self, module_name: str):
-        self.module_name = module_name
-
-
-class InvalidWorkflowDefinitionError(BaseRuntimeError):
-    """Raised when a workflow definition is invalid.
-
-    This may be due to errors in the definition, or failure to meet runtime
-    requirements.
-    """
-
-    pass
-
-
-# Task Definition Errors
-class InvalidTaskDefinitionError(BaseRuntimeError):
-    """Raised when a task definition is invalid."""
-
-    pass
-
-
-class NodesInTaskResourcesWarning(Warning):
-    """Raised when a "nodes" resource is passed to a Task.
-
-    Nodes currently only apply to workflows and this option will be ignored.
-    """
-
-
-# Workflow Errors
-class InvalidWorkflowRunLogsError(BaseRuntimeError):
-    """Raised when workflow logs cannot be decoded."""
-
-    pass
-
-
-class TaskRunLogsNotFound(NotFoundError):
-    """Raised when a task run logs cannot be found, or the ID is invalid."""
-
-    def __init__(self, wf_run_id: WorkflowRunId, task_inv_id: TaskInvocationId):
-        self.wf_run_id = wf_run_id
-        self.task_inv_id = task_inv_id
-        super().__init__()
-
-
-class WorkflowRunNotSucceeded(BaseRuntimeError):
-    """Raised when a succeeded workflow is required but it is found in another state."""
-
-    def __init__(self, message: str, state: State):
-        super().__init__(message)
-        self.state = state
-
-
-class WorkflowRunNotFinished(BaseRuntimeError):
-    """Raised when a finished workflow is required but an unfinished one is found."""
-
-    def __init__(self, message: str, state: State):
-        super().__init__(message)
-        self.state = state
-
-
-class WorkflowRunCanNotBeTerminated(BaseRuntimeError):
-    """Raised when an attempt to terminate a workflow run fails."""
-
-    pass
-
-
-class WorkflowRunNotFoundError(NotFoundError):
-    """Raised when no run with the specified ID is found."""
-
-    pass
-
-
-class RuntimeQuerySummaryError(NotFoundError):
-    """Raised when of the queried runtimes could find this workflow run.
-
-    We need this class on the Python API layer to produce a pretty-printed visual
-    output in the CLI.
-
-    Args:
-        wf_run_id: identifier of the workflow run we were looking for.
-        not_found_runtimes: runtimes we queried and the reponse was "this workflow run
-            is not found"
-        unauthorized_runtimes: runtimes we queried and the reponse was "you're not
-            authorized to access this resource"
-        not_running_runtimes: runtimes we queried but the cluster wasn't running
-    """
-
-    @dataclass(frozen=True)
-    class RuntimeInfo:
-        runtime_name: configs.RuntimeName
-        config_name: t.Optional[configs.ConfigName]
-        server_uri: t.Optional[str]
-
-    def __init__(
-        self,
-        wf_run_id: WorkflowRunId,
-        not_found_runtimes: t.Sequence[RuntimeInfo],
-        unauthorized_runtimes: t.Sequence[RuntimeInfo],
-        not_running_runtimes: t.Sequence[RuntimeInfo],
-    ):
-        not_found_configs = [info.config_name for info in not_found_runtimes]
-        unauthorized_configs = [info.config_name for info in unauthorized_runtimes]
-        not_running_configs = [info.config_name for info in not_running_runtimes]
-        super().__init__(
-            message=(
-                "Couldn't find a config that knows about workflow run ID"
-                f" {wf_run_id} \n"
-                f"Configs with 'not found' response: {not_found_configs}.\n"
-                f"Configs with 'unauthorized' response: {unauthorized_configs}.\n"
-                f"Configs that weren't up: {not_running_configs}."
-            )
-        )
-        self.wf_run_id = wf_run_id
-        self.not_found_runtimes = not_found_runtimes
-        self.unauthorized_runtimes = unauthorized_runtimes
-        self.not_running_runtimes = not_running_runtimes
-
-
-class WorkflowRunNotStarted(WorkflowRunNotFoundError):
-    """Raised when a started workflow is required but an unstarted one is found."""
-
-    pass
-
-
-class TaskRunNotFound(NotFoundError):
-    """Raised when a task hasn't completed yet, or the ID is invalid."""
-
-    pass
-
-
-class TaskInvocationNotFoundError(NotFoundError):
-    """Raised when we can't find a Task Invocation that matches the provided ID."""
-
-    def __init__(self, invocation_id: ir.TaskInvocationId):
-        super().__init__()
-        self.invocation_id = invocation_id
-
-
-class WorkflowResultsNotReadyError(NotFoundError):
-    """Raised when a workflow has succeeded, but the results are not ready yet."""
-
-
-class WorkflowRunIDNotFoundError(NotFoundError):
-    """Raised when we can't recover the ID for this Workflow Run."""
-
-    # Note that this is different to the WorkflowRunNotFoundError.
-    # We have an ID but can't find the workflow: WorkflowRunNotFoundError
-    # We have a workflow but can't recover the ID: WorkflowRunIDNotFoundError
-
-
-class OrquestraSDKVersionMismatchWarning(Warning):
-    """Raised when there are multiple SDK dependency declarations for one task env."""
-
-
-# Auth Errors
-class UnauthorizedError(BaseRuntimeError):
-    """Raised when the remote cluster rejects the auth token."""
-
-    pass
-
-
-class ExpiredTokenError(BaseRuntimeError):
-    """Raised when the auth token is expired."""
-
-    pass
-
-
-class InvalidTokenError(BaseRuntimeError):
-    """Raised when an auth token is not a JWT."""
-
-    pass
-
-
-class RemoteConnectionError(BaseRuntimeError):
-    """Raised when we could not get the connection to the remote Orquestra cluster."""
-
-    def __init__(self, uri: str):
-        self.uri = uri
-        super().__init__(uri)
-
-
-# Ray Errors
-class RayActorNameClashError(BaseRuntimeError):
-    """Raised when multiple Ray actors exist with the same name."""
-
-    pass
-
-
-class RayNotRunningError(ConnectionError):
-    """Raised when there isn't a running ray instance."""
-
-    pass
-
-
-# CLI Exceptions
-class UserCancelledPrompt(BaseRuntimeError):
-    """Raised when the user cancels a CLI prompt."""
-
-    pass
-
-
-class LoginURLUnavailableError(BaseRuntimeError):
-    """Raised when the login URL for is unavailable."""
-
-    def __init__(self, base_uri: str):
-        self.base_uri = base_uri
-
-
-class NoOptionsAvailableError(NotFoundError):
-    """Raised when the user would choose options, but no options are available."""
-
-    pass
-
-
-class InProcessFromCLIError(NotFoundError):
-    """Raised when the user requests the in-process runtime when using the CLI."""
-
-
-# Unsupported features
-class UnsupportedRuntimeFeature(Warning):
-    """Raised when a requested feature is not supported on the selected runtime."""
-
-    pass
-
-
-class ProjectInvalidError(BaseRuntimeError):
-    """When there is insufficient information provided to identify a unique project."""
-
-    pass
-
-
-class WorkspacesNotSupportedError(BaseRuntimeError):
-    """When a non-workspaces supporting runtime gets a workspaces-related request."""
-
-    pass
-
-
-class IgnoredFieldWarning(Warning):
-    """Raised when a requested feature is not supported on the selected runtime."""
-
-    pass
+from orquestra.sdk._shared.exceptions import (
+    BaseRuntimeError,
+    ConfigFileNotFoundError,
+    ConfigNameNotFoundError,
+    DirtyGitRepo,
+    EnvVarNotFoundError,
+    ExpiredTokenError,
+    IgnoredFieldWarning,
+    InProcessFromCLIError,
+    InvalidTaskDefinitionError,
+    InvalidTokenError,
+    InvalidWorkflowDefinitionError,
+    InvalidWorkflowRunLogsError,
+    LocalConfigLoginError,
+    LoginURLUnavailableError,
+    NodesInTaskResourcesWarning,
+    NoOptionsAvailableError,
+    NotFoundError,
+    NoWorkflowDefinitionsFound,
+    OrquestraSDKVersionMismatchWarning,
+    ProjectInvalidError,
+    QERemoved,
+    RayActorNameClashError,
+    RayNotRunningError,
+    RemoteConnectionError,
+    RuntimeConfigError,
+    RuntimeQuerySummaryError,
+    TaskInvocationNotFoundError,
+    TaskRunLogsNotFound,
+    TaskRunNotFound,
+    UnauthorizedError,
+    UnsupportedRuntimeFeature,
+    UserCancelledPrompt,
+    UserTaskFailedError,
+    VersionMismatch,
+    WorkflowDefinitionModuleNotFound,
+    WorkflowResultsNotReadyError,
+    WorkflowRunCanNotBeTerminated,
+    WorkflowRunIDNotFoundError,
+    WorkflowRunNotFinished,
+    WorkflowRunNotFoundError,
+    WorkflowRunNotStarted,
+    WorkflowRunNotSucceeded,
+    WorkflowSyntaxError,
+    WorkspacesNotSupportedError,
+)
+
+__all__ = [
+    "BaseRuntimeError",
+    "ConfigFileNotFoundError",
+    "ConfigNameNotFoundError",
+    "DirtyGitRepo",
+    "EnvVarNotFoundError",
+    "ExpiredTokenError",
+    "IgnoredFieldWarning",
+    "InProcessFromCLIError",
+    "InvalidTaskDefinitionError",
+    "InvalidTokenError",
+    "InvalidWorkflowDefinitionError",
+    "InvalidWorkflowRunLogsError",
+    "LocalConfigLoginError",
+    "LoginURLUnavailableError",
+    "NoOptionsAvailableError",
+    "NoWorkflowDefinitionsFound",
+    "NodesInTaskResourcesWarning",
+    "NotFoundError",
+    "OrquestraSDKVersionMismatchWarning",
+    "ProjectInvalidError",
+    "QERemoved",
+    "RayActorNameClashError",
+    "RayNotRunningError",
+    "RemoteConnectionError",
+    "RuntimeConfigError",
+    "RuntimeQuerySummaryError",
+    "TaskInvocationNotFoundError",
+    "TaskRunLogsNotFound",
+    "TaskRunNotFound",
+    "UnauthorizedError",
+    "UnsupportedRuntimeFeature",
+    "UserCancelledPrompt",
+    "UserTaskFailedError",
+    "VersionMismatch",
+    "WorkflowDefinitionModuleNotFound",
+    "WorkflowResultsNotReadyError",
+    "WorkflowRunCanNotBeTerminated",
+    "WorkflowRunIDNotFoundError",
+    "WorkflowRunNotFinished",
+    "WorkflowRunNotFoundError",
+    "WorkflowRunNotStarted",
+    "WorkflowRunNotSucceeded",
+    "WorkflowSyntaxError",
+    "WorkspacesNotSupportedError",
+]
```

## orquestra/sdk/_ray/__init__.py

```diff
@@ -1,13 +0,0 @@
-00000000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000020: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000050: 0a23 20c2 a920 436f 7079 7269 6768 7420  .# .. Copyright 
-00000060: 3230 3233 205a 6170 6174 6120 436f 6d70  2023 Zapata Comp
-00000070: 7574 696e 6720 496e 632e 0a23 2323 2323  uting Inc..#####
-00000080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000000a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000000b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000000c0: 2323 2323 2323 2323 2323 230a            ###########.
```

## orquestra/sdk/_ray/_build_workflow.py

```diff
@@ -1,663 +1,10 @@
 ################################################################################
-# © Copyright 2023 - 2024 Zapata Computing Inc.
+# © Copyright 2024 Zapata Computing Inc.
 ################################################################################
-"""Translates IR workflow def into a Ray workflow."""
-import os
-import re
-import time
-import typing as t
-import warnings
-from functools import singledispatch
-from pathlib import Path
+# THIS FILE IS A SHIM TO REEXPORT SYMBOLS FOR BACKWARDS COMPATIBILITY
+# WITH OLD WORKFLOW RESULTS.
+# DO NOT PUT ANY LOGIC INTO THIS FILE.
 
-import pydantic
-from packaging import version
-from typing_extensions import assert_never
+from orquestra.sdk._runtime._ray._build_workflow import TaskResult
 
-from orquestra.sdk.packaging import get_installed_version
-
-from .. import exceptions, secrets
-from .._base import _exec_ctx, _git_url_utils, _graphs, _services, dispatch, serde
-from .._base._env import (
-    RAY_DOWNLOAD_GIT_IMPORTS_ENV,
-    RAY_SET_CUSTOM_IMAGE_RESOURCES_ENV,
-)
-from .._base._logs import _markers
-from .._base._regex import SEMVER_REGEX
-from ..kubernetes.quantity import parse_quantity
-from ..schema import ir, responses, workflow_run
-from . import _client, _id_gen
-from ._wf_metadata import InvUserMetadata, pydatic_to_json_dict
-
-DEFAULT_IMAGE_TEMPLATE = "hub.nexus.orquestra.io/zapatacomputing/orquestra-sdk-base:{}"
-
-
-def _get_default_image(template: str, sdk_version: str, num_gpus: t.Optional[int]):
-    image = template.format(sdk_version)
-    if num_gpus is not None and num_gpus > 0:
-        image = f"{image}-cuda"
-    return image
-
-
-def _arg_from_graph(argument_id: ir.ArgumentId, workflow_def: ir.WorkflowDef):
-    try:
-        return workflow_def.constant_nodes[argument_id]
-    except KeyError:
-        pass
-
-    try:
-        return workflow_def.secret_nodes[argument_id]
-    except KeyError:
-        pass
-
-    # If we reach this point, we MUST be an artifact.
-    # Any exception raised here (i.e. KeyError) means something major went wrong.
-    return workflow_def.artifact_nodes[argument_id]
-
-
-def _locate_user_fn(fn_ref: ir.FunctionRef):
-    """Extract the underlying user functions from a 'fn_ref'.
-
-    Dereferences 'fn_ref', loads the module attribute, and extracts the underlying user
-    function if it was a TaskDef.
-    """
-    obj: t.Any = dispatch.locate_fn_ref(fn_ref)
-
-    # dsl.task() wraps a callable in a TaskDef object. We need to locate the
-    # underlying user function, not the Task object.
-    try:
-        return obj._TaskDef__sdk_task_body
-    except AttributeError:
-        return obj
-
-
-def _aggregate_outputs(*args):
-    if len(args) == 1:
-        return args[0]
-    return args
-
-
-class TaskResult(t.NamedTuple):
-    packed: responses.WorkflowResult
-    unpacked: t.Tuple[responses.WorkflowResult, ...]
-
-
-class ArgumentUnwrapper:
-    """Unwraps arguments (constants, secrets, artifacts) before passing to a task."""
-
-    def __init__(
-        self,
-        user_fn: t.Callable,
-        args_artifact_nodes: t.Mapping[int, ir.ArtifactNode],
-        kwargs_artifact_nodes: t.Mapping[str, ir.ArtifactNode],
-        deserialize: bool,
-    ):
-        """Initilaiser for the ArgumentUnwrapper.
-
-        Args:
-            user_fn: the task function to wrap.
-            args_artifact_nodes: A map of positional argument index to workflow artifact
-                node.
-                This is to assist with unpacking artifact results.
-                Not all positional arguments will be included, i.e. a constant or secret
-            kwargs_artifact_nodes: A map of keyword argument name to workflow artifact
-                node.
-                This is to assist with unpacking artifact results.
-                Not all positional arguments will be included, i.e. a constant or secret
-            deserialize: If true, we will first deserialize the argument before passing
-                to the task function.
-                If false, the serialized argument is passed to the underlying task
-                function.
-                This is used to avoid the deserialization problem of having the Python
-                dependencies for Pickles when aggregating the outputs of a workflow.
-        """
-        self._user_fn = user_fn
-        self._args_artifact_nodes = args_artifact_nodes
-        self._kwargs_artifact_nodes = kwargs_artifact_nodes
-        self._deserialize = deserialize
-
-    def _get_metadata(self, key: t.Union[int, str]) -> t.Optional[ir.ArtifactNode]:
-        if isinstance(key, int):
-            return self._args_artifact_nodes.get(key)
-        elif isinstance(key, str):
-            return self._kwargs_artifact_nodes.get(key)
-        else:
-            assert_never(key)
-
-    def _unpack_argument(
-        self,
-        arg: t.Union[ir.ConstantNode, ir.SecretNode, TaskResult],
-        meta_key: t.Union[int, str],
-    ):
-        if isinstance(arg, (ir.ConstantNodeJSON, ir.ConstantNodePickle)):
-            return serde.deserialize(arg) if self._deserialize else arg
-        elif isinstance(arg, ir.SecretNode):
-            return (
-                secrets.get(
-                    arg.secret_name,
-                    config_name=arg.secret_config,
-                    workspace_id=arg.workspace_id,
-                )
-                if self._deserialize
-                else arg
-            )
-        elif isinstance(arg, TaskResult):
-            meta = self._get_metadata(meta_key)
-            if meta is None or meta.artifact_index is None:
-                return (
-                    serde.deserialize(arg.packed) if self._deserialize else arg.packed
-                )
-            else:
-                return (
-                    serde.deserialize(arg.unpacked[meta.artifact_index])
-                    if self._deserialize
-                    else arg.unpacked[meta.artifact_index]
-                )
-        else:
-            assert_never(arg)
-
-    def __call__(self, *wrapped_args, **wrapped_kwargs):
-        args = []
-        kwargs = {}
-
-        for i, arg in enumerate(wrapped_args):
-            args.append(self._unpack_argument(arg, i))
-
-        for name, kwarg in wrapped_kwargs.items():
-            kwargs[name] = self._unpack_argument(kwarg, name)
-
-        return self._user_fn(*args, **kwargs)
-
-
-SENTINEL = "dry_run task output"
-
-
-def _generate_nop_function(output_metadata: ir.TaskOutputMetadata):
-    def nop(*_, **__):
-        if not output_metadata.is_subscriptable:
-            return SENTINEL
-        else:
-            return (SENTINEL,) * output_metadata.n_outputs
-
-    return nop
-
-
-def _get_user_function(
-    user_fn_ref, dry_run, output_metadata: t.Optional[ir.TaskOutputMetadata]
-):
-    # Ref is None only in case of the data aggregation step
-    if user_fn_ref is None:
-        return _aggregate_outputs
-    elif not dry_run:
-        return _locate_user_fn(user_fn_ref)
-    else:
-        assert output_metadata is not None
-        return _generate_nop_function(output_metadata)
-
-
-def _make_ray_dag_node(
-    client: _client.RayClient,
-    ray_options: t.Mapping,
-    ray_args: t.Iterable[t.Any],
-    ray_kwargs: t.Mapping[str, t.Any],
-    args_artifact_nodes: t.Mapping,
-    kwargs_artifact_nodes: t.Mapping,
-    user_fn_ref: t.Optional[ir.FunctionRef],
-    output_metadata: t.Optional[ir.TaskOutputMetadata],
-    dry_run: bool,
-) -> _client.FunctionNode:
-    """Prepares a Ray task that fits a single ir.TaskInvocation.
-
-    The result is a node in a Ray DAG.
-
-    Args:
-        client: Ray API facade.
-        ray_options: dict passed to _client.RayClient.add_options().
-        ray_args: constants or futures required to build the DAG.
-        ray_kwargs: constants or futures required to build the DAG.
-        args_artifact_nodes: a map of positional arg index to artifact node
-            see ArgumentUnwrapper.
-        kwargs_artifact_nodes: a map of keyword arg name to artifact node
-            see ArgumentUnwrapper.
-        user_fn_ref: function reference for a function to be executed by Ray.
-            if None - executes data aggregation step.
-        output_metadata: output metadata for the user task function.
-            Keeps number of outputs and if the output is subscriptable.
-        dry_run: Run the task without actually executing any user code.
-            Useful for testing infrastructure, dependency imports, etc.
-    """
-    current_path = Path.cwd()
-
-    @client.remote
-    def _ray_remote(*inner_args, **inner_kwargs):
-        with _exec_ctx.ray():
-            # We need to emit task start marker log as soon as possible. Otherwise, we
-            # risk an exception won't be visible to the user.
-            #
-            # TODO: make the IDs required and raise an error if they're not present.
-            # https://zapatacomputing.atlassian.net/browse/ORQSDK-530
-            wf_run_id, task_inv_id, _ = get_current_ids()
-            with _markers.capture_logs(
-                logs_dir=_services.redirected_logs_dir(),
-                wf_run_id=wf_run_id,
-                task_inv_id=task_inv_id,
-            ):
-                dispatch.ensure_sys_paths([str(current_path)])
-
-                # True for all the steps except data aggregation
-                serialization = user_fn_ref is not None
-
-                # Try-except block covers _get_user_function and wrapped() because:
-                # _get_user_function un-pickles the inlineImported functions - and this
-                # operation can already cause exceptions
-                # wrapped() calls user function, which catches all the exceptions
-                # that happens within user code
-                try:
-                    user_fn = _get_user_function(user_fn_ref, dry_run, output_metadata)
-
-                    wrapped = ArgumentUnwrapper(
-                        user_fn=user_fn,
-                        args_artifact_nodes=args_artifact_nodes,
-                        kwargs_artifact_nodes=kwargs_artifact_nodes,
-                        deserialize=serialization,
-                    )
-
-                    wrapped_return = wrapped(*inner_args, **inner_kwargs)
-                except Exception as e:
-                    assert wf_run_id is not None
-                    assert task_inv_id is not None
-                    _client.save_task_postrun_metadata(
-                        wf_run_id,
-                        task_inv_id,
-                        {"end_time": time.time(), "failed": True},
-                    )
-
-                    raise exceptions.UserTaskFailedError(
-                        f"User task with task invocation id:{task_inv_id} failed.",
-                        wf_run_id if wf_run_id else "",
-                        task_inv_id if task_inv_id else "",
-                    ) from e
-
-                packed: responses.WorkflowResult = (
-                    serde.result_from_artifact(wrapped_return, ir.ArtifactFormat.AUTO)
-                    if serialization
-                    else wrapped_return
-                )
-                unpacked: t.Tuple[responses.WorkflowResult, ...]
-
-                if output_metadata is not None and output_metadata.n_outputs > 1:
-                    unpacked = tuple(
-                        (
-                            serde.result_from_artifact(
-                                wrapped_return[i], ir.ArtifactFormat.AUTO
-                            )
-                            if serialization
-                            else wrapped_return[i]
-                        )
-                        for i in range(output_metadata.n_outputs)
-                    )
-                else:
-                    unpacked = (packed,)
-                return TaskResult(
-                    packed=packed,
-                    unpacked=unpacked,
-                )
-
-    named_remote = client.add_options(_ray_remote, **ray_options)
-    dag_node = named_remote.bind(*ray_args, **ray_kwargs)
-
-    return dag_node
-
-
-def _gen_task_run_id(wf_run_id: str, invocation: ir.TaskInvocation):
-    """
-    Loosely corresponds to the "unified ID" in the tagging design doc:
-    https://zapatacomputing.atlassian.net/wiki/spaces/ORQSRUN/pages/479920161/Logging+Tagging.
-
-    Assumed to be globally unique.
-
-    Example value: "wf.multioutput_wf.91aa7aa@invocation-3-task-make-company-name.91e4b"
-    """  # noqa: D205, D212
-    inv_id = invocation.id
-    hex_str = _id_gen.gen_short_uid(char_length=5)
-
-    return f"{wf_run_id}@{inv_id}.{hex_str}"
-
-
-@singledispatch
-def _pip_string(_: ir.Import) -> t.List[str]:
-    return []
-
-
-@_pip_string.register
-def _(imp: ir.PythonImports):
-    return [serde.stringify_package_spec(package) for package in imp.packages]
-
-
-@_pip_string.register
-def _(imp: ir.GitImport):
-    # Only download Git imports if a specific environment variable is set
-    # Short circuit the Git import otherwise
-    if os.getenv(RAY_DOWNLOAD_GIT_IMPORTS_ENV) != "1":
-        return []
-    protocol = imp.repo_url.protocol
-    if not protocol.startswith("git+"):
-        protocol = f"git+{protocol}"
-    url = _git_url_utils.build_git_url(imp.repo_url, protocol)
-    return [f"{url}@{imp.git_ref}"]
-
-
-def _import_pip_env(
-    ir_invocation: ir.TaskInvocation,
-    wf: ir.WorkflowDef,
-    imports_pip_string: t.Dict[ir.ImportId, t.List[str]],
-) -> t.List[str]:
-    """Gather a list of python imports required for the task.
-
-    Args:
-        ir_invocation: The task invocation to be executed in this environment.
-        wf: The overall workflow definition.
-        imports_pip_string: a mapping between the ID and the list of pip strings for a
-            specific import
-
-    Returns:
-        A list consisting of the python imports declared in the task definition, and the
-            current Orquestra SDK version. The latter is included to prevent tasks from
-            executing with different SDK versions to the head node.
-    """
-    task_def = wf.tasks[ir_invocation.task_id]
-    imports = [
-        wf.imports[id_]
-        for id_ in (
-            task_def.source_import_id,
-            *(task_def.dependency_import_ids or []),
-        )
-    ]
-
-    current_sdk_version: str = get_installed_version("orquestra-sdk")
-
-    sdk_dependency = None
-    pip_list = [
-        chunk
-        for imp in imports
-        for chunk in imports_pip_string[imp.id]
-        if not (sdk_dependency := re.match(r"^orquestra-sdk([<|!|=|>|~].*)?$", chunk))
-    ]
-
-    # If the task definition includes the SDK, warn the user that this does nothing.
-    if sdk_dependency:
-        warnings.warn(
-            f"The definition for task `{ir_invocation.task_id}` "
-            f"declares `{sdk_dependency[0]}` as a dependency. "
-            "The current SDK version "
-            + (f"({current_sdk_version}) " if current_sdk_version else "")
-            + "is automatically installed in task environments. "
-            "The specified dependency will be ignored.",
-            exceptions.OrquestraSDKVersionMismatchWarning,
-        )
-
-    # Don't add sdk dependency if submitting from a prerelease or dev version.
-    parsed_sdk_version = version.parse(current_sdk_version)
-    if not (parsed_sdk_version.is_devrelease or parsed_sdk_version.is_prerelease):
-        pip_list += [f"orquestra-sdk=={current_sdk_version}"]
-
-    return pip_list
-
-
-def _normalise_prerelease_version(version: str) -> t.Optional[str]:
-    """Remove prerelease version information from the version string."""
-    match = re.match(SEMVER_REGEX, version)
-    assert match, f"Version {version} did not parse as valid SemVer."
-    vernums = [int(match.group("major")), int(match.group("minor"))]
-    if match.group("patch"):
-        vernums.append(int(match.group("patch")))
-
-    # If the version is a prerelease, go back to the previous iteration.
-    if match.group("prerelease"):
-        vernums[-1] -= 1
-
-    # Safety hatch - returning a version less than 0.1 is nonsensical.
-    if vernums[0:2] == [0, 0]:
-        return None
-
-    return ".".join([str(vernum) for vernum in vernums])
-
-
-def _gather_args(arg_ids, workflow_def, ray_futures):
-    ray_args = []
-    ray_args_artifact_nodes: t.Dict[int, t.Optional[ir.ArtifactNode]] = {}
-    for i, arg_id in enumerate(arg_ids):
-        ir_node = _arg_from_graph(arg_id, workflow_def)
-        if isinstance(ir_node, ir.ArtifactNode):
-            ray_args.append(ray_futures[arg_id])
-            ray_args_artifact_nodes[i] = ir_node
-        else:
-            ray_args.append(ir_node)
-            ray_args_artifact_nodes[i] = None
-
-    return tuple(ray_args), ray_args_artifact_nodes
-
-
-def _gather_kwargs(kwargs, workflow_def, ray_futures):
-    ray_kwargs = {}
-    ray_kwargs_artifact_nodes: t.Dict[str, t.Optional[ir.ArtifactNode]] = {}
-    for name, kwarg_id in kwargs.items():
-        ir_node = _arg_from_graph(kwarg_id, workflow_def)
-        if isinstance(ir_node, ir.ArtifactNode):
-            ray_kwargs[name] = ray_futures[kwarg_id]
-            ray_kwargs_artifact_nodes[name] = ir_node
-        else:
-            ray_kwargs[name] = ir_node
-            ray_kwargs_artifact_nodes[name] = None
-
-    return ray_kwargs, ray_kwargs_artifact_nodes
-
-
-def _ray_resources_for_custom_image(image_name: str) -> t.Mapping[str, float]:
-    """
-    Custom Ray resources we set to power running Orquestra tasks on custom Docker
-    images.
-    The values are coupled with Compute Engine server-side set up.
-    """  # noqa: D205, D212
-    # The format for custom image strings is described in the ADR:
-    # https://zapatacomputing.atlassian.net/wiki/spaces/ORQSRUN/pages/688259073/2023-05-05+Ray+resources+syntax+for+custom+images
-    return {f"image:{image_name}": 1}
-
-
-def make_ray_dag(
-    client: _client.RayClient,
-    workflow_def: ir.WorkflowDef,
-    workflow_run_id: workflow_run.WorkflowRunId,
-    dry_run: bool,
-):
-    # a mapping of "artifact ID" <-> "the ray Future needed to get the value"
-    ray_futures: t.Dict[ir.ArtifactNodeId, t.Any] = {}
-
-    # this resolves all imports to their final "pip string" once,
-    # instead of per-task invocation
-    imports_pip_strings = {
-        id_: _pip_string(imp) for id_, imp in workflow_def.imports.items()
-    }
-
-    for invocation in _graphs.iter_invocations_topologically(workflow_def):
-        user_task = workflow_def.tasks[invocation.task_id]
-        pos_args, pos_args_artifact_nodes = _gather_args(
-            invocation.args_ids, workflow_def, ray_futures
-        )
-        kwargs, kwargs_artifact_nodes = _gather_kwargs(
-            invocation.kwargs_ids, workflow_def, ray_futures
-        )
-        # We want to store both the TaskInvocation.id and TaskRun.id. We use
-        # TaskInvocation.id to refer to Ray tasks later. Solution: Ray task
-        # name for identification and Ray metadata for anything else.
-        inv_metadata = InvUserMetadata(
-            task_run_id=_gen_task_run_id(
-                wf_run_id=workflow_run_id, invocation=invocation
-            ),
-            task_invocation_id=invocation.id,
-        )
-
-        pip = _import_pip_env(invocation, workflow_def, imports_pip_strings)
-
-        ray_options = {
-            # We're using task invocation ID as the Ray "task ID" instead of task run ID
-            # because it's easier to query this way. Use the "user_metadata" to get both
-            # identifiers.
-            "name": invocation.id,
-            "metadata": pydatic_to_json_dict(inv_metadata),
-            # If there are any python packages to install for step - set runtime env
-            "runtime_env": (_client.RuntimeEnv(pip=pip) if len(pip) > 0 else None),
-            "catch_exceptions": False,
-            # We only want to execute workflow tasks once by default.
-            # This is so there is only one task run ID per task, for scenarios where
-            # this is used (like in MLflow). We allow setting this variable on
-            # task-level for some particular edge-cases like memory leaks inside
-            # 3rd party libraries - so in case of the OOMKilled worker it can be
-            # restarted.
-            # By default, Ray will only retry tasks that fail due to a "system error".
-            # For example, if the worker process crashes or exits early.
-            # Normal Python exceptions are NOT retried.
-            "max_retries": user_task.max_retries if user_task.max_retries else 0,
-        }
-
-        # Non-custom task resources
-        if invocation.resources is not None:
-            if invocation.resources.cpu is not None:
-                cpu = parse_quantity(invocation.resources.cpu)
-                cpu_int = cpu.to_integral_value()
-                ray_options["num_cpus"] = int(cpu_int) if cpu == cpu_int else float(cpu)
-            if invocation.resources.memory is not None:
-                memory = parse_quantity(invocation.resources.memory)
-                memory_int = memory.to_integral_value()
-                ray_options["memory"] = (
-                    int(memory_int) if memory == memory_int else float(memory)
-                )
-            if invocation.resources.gpu is not None:
-                # Fractional GPUs not supported currently
-                gpu = int(float(invocation.resources.gpu))
-                ray_options["num_gpus"] = gpu
-
-        # Set custom image
-        if os.getenv(RAY_SET_CUSTOM_IMAGE_RESOURCES_ENV) is not None:
-            # This makes an assumption that only "new" IRs will get to this point
-            assert workflow_def.metadata is not None, "Expected a >=0.45.0 IR"
-            sdk_version = workflow_def.metadata.sdk_version.original
-
-            # Custom "Ray resources" request. The entries need to correspond to the ones
-            # used when starting the Ray cluster. See also:
-            # https://docs.ray.io/en/latest/ray-core/scheduling/resources.html#custom-resources
-            ray_options["resources"] = _ray_resources_for_custom_image(
-                invocation.custom_image
-                or user_task.custom_image
-                or _get_default_image(
-                    DEFAULT_IMAGE_TEMPLATE, sdk_version, ray_options.get("num_gpus")
-                )
-            )
-
-        ray_result = _make_ray_dag_node(
-            client=client,
-            ray_options=ray_options,
-            ray_args=pos_args,
-            ray_kwargs=kwargs,
-            args_artifact_nodes=pos_args_artifact_nodes,
-            kwargs_artifact_nodes=kwargs_artifact_nodes,
-            user_fn_ref=user_task.fn_ref,
-            output_metadata=user_task.output_metadata,
-            dry_run=dry_run,
-        )
-
-        for output_id in invocation.output_ids:
-            ray_futures[output_id] = ray_result
-
-    # Gather futures for the last, fake task, and decide what args we need to unwrap.
-    pos_args, pos_args_artifact_nodes = _gather_args(
-        workflow_def.output_ids, workflow_def, ray_futures
-    )
-    last_future = _make_ray_dag_node(
-        client=client,
-        # The last step is implicit; it doesn't map to any user-defined Task
-        # Invocation. We don't need to assign any metadata to it.
-        ray_options={
-            "name": None,
-            "metadata": None,
-            "runtime_env": None,
-            "catch_exceptions": True,
-            # Set to avoid retrying when the worker crashes.
-            # See the comment with the invocation's options for more details.
-            "max_retries": 0,
-            # Custom "Ray resources" request. We don't need any for the aggregation
-            # step.
-            "resources": None,
-        },
-        ray_args=pos_args,
-        ray_kwargs={},
-        args_artifact_nodes=pos_args_artifact_nodes,
-        kwargs_artifact_nodes={},
-        user_fn_ref=None,
-        output_metadata=ir.TaskOutputMetadata(
-            n_outputs=len(pos_args), is_subscriptable=False
-        ),
-        dry_run=False,
-    )
-
-    # Data aggregation step is run with catch_exceptions=True - so it returns tuple of
-    # return value and Exception. Here the exception is caught and rethrown in more
-    # user-friendly fashion
-    @client.remote
-    def handle_data_aggregation_error(result: t.Tuple[t.Any, Exception]):
-        # The exception field will be None on success.
-        err = result[1]
-        if err is not None:
-            if isinstance(err, _client.TaskError):
-                raise exceptions.InvalidWorkflowDefinitionError(
-                    "Data Aggregation step failed. It might be caused by the return "
-                    "object being dependent on task-scope installed library. Please "
-                    "return objects that are available for the interpreter. "
-                ) from err
-            else:
-                raise err
-        else:
-            return result[0]
-
-    return handle_data_aggregation_error.bind(last_future)
-
-
-def get_current_ids() -> (
-    t.Tuple[
-        t.Optional[workflow_run.WorkflowRunId],
-        t.Optional[ir.TaskInvocationId],
-        t.Optional[workflow_run.TaskRunId],
-    ]
-):
-    """Use Ray context to figure out the IDs of the currently running workflow and task.
-
-    The returned TaskInvocationID and TaskRunID are None if we weren't able to get them
-    from the current Ray context.
-    """
-    # NOTE: this is tightly coupled with how we create Ray workflow DAG, how we assign
-    # IDs and metadata.
-    client = _client.RayClient()
-
-    try:
-        wf_run_id = client.get_current_workflow_id()
-    except AssertionError:
-        # Ray has an 'assert' about checking the workflow context outside of a workflow
-        return None, None, None
-
-    # We don't need to care what kind of ID it is, we only need it to get the metadata
-    # dict.
-    ray_task_name = client.get_current_task_id()
-    task_meta: dict = client.get_task_metadata(
-        workflow_id=wf_run_id, name=ray_task_name
-    )
-
-    try:
-        user_meta = InvUserMetadata.model_validate(task_meta.get("user_metadata"))
-    except pydantic.ValidationError:
-        # This ray task wasn't annotated with InvUserMetadata. It happens when
-        # `get_current_ids()` is used from a context that's not a regular Orquestra Task
-        # run. One example is the one-off task that we use to construct Ray DAG inside a
-        # Ray worker process.
-        return wf_run_id, None, None
-
-    return wf_run_id, user_meta.task_invocation_id, user_meta.task_run_id
+__all__ = ["TaskResult"]
```

## orquestra/sdk/dremio/__init__.py

```diff
@@ -1,10 +1,11 @@
 ################################################################################
-# © Copyright 2023-2024 Zapata Computing Inc.
+# © Copyright 2024 Zapata Computing Inc.
 ################################################################################
-"""Utility for reading data from Dremio managed by Orquestra."""
+# THIS FILE IS A SHIM TO REEXPORT SYMBOLS AS PUBLIC API
+# DO NOT PUT ANY LOGIC INTO THIS FILE.
 
-from ._api import DremioClient
+from .._client.dremio import DremioClient
 
 __all__ = [
     "DremioClient",
 ]
```

## orquestra/sdk/examples/exportable_wf.py

```diff
@@ -8,36 +8,36 @@
 
 # public API
 import orquestra.sdk as sdk
 
 
 @sdk.task(
     source_import=sdk.GitImport(
-        repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
+        repo_url="git@github.com:zapata-engineering/orquestra-sdk.git",
         git_ref="main",
     ),
 )
 def capitalize(text: str) -> str:
     return text.capitalize()
 
 
 @sdk.task(
     source_import=sdk.GitImport(
-        repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
+        repo_url="git@github.com:zapata-engineering/orquestra-sdk.git",
         git_ref="main",
     ),
 )
 def make_greeting(first, last, additional_message: t.Optional[str] = None) -> str:
     return f"hello, {first} {last}!{additional_message or ''}"
 
 
 @sdk.task(
     n_outputs=2,
     source_import=sdk.GitImport(
-        repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
+        repo_url="git@github.com:zapata-engineering/orquestra-sdk.git",
         git_ref="main",
     ),
 )
 def multi_output_test():
     return "hello", "there"
```

## orquestra/sdk/kubernetes/__init__.py

```diff
@@ -1,6 +1,5 @@
 ################################################################################
-# © Copyright 2023 Zapata Computing Inc.
+# © Copyright 2024 Zapata Computing Inc.
 ################################################################################
-
-# This module is vendored from https://github.com/kubernetes-client/python
-# See each source file for copyright.
+# THIS FILE IS A SHIM TO REEXPORT SYMBOLS AS PUBLIC API
+# DO NOT PUT ANY LOGIC INTO THIS FILE.
```

## orquestra/sdk/kubernetes/quantity.py

```diff
@@ -1,88 +1,9 @@
-# Copyright 2019 The Kubernetes Authors.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+################################################################################
+# © Copyright 2024 Zapata Computing Inc.
+################################################################################
+# THIS FILE IS A SHIM TO REEXPORT SYMBOLS AS PUBLIC API
+# DO NOT PUT ANY LOGIC INTO THIS FILE.
 
-from decimal import Decimal, InvalidOperation
-from typing import Any
+from orquestra.sdk._shared.kubernetes.quantity import parse_quantity
 
-
-def parse_quantity(quantity: Any):
-    """Parse kubernetes canonical form quantity like 200Mi to a decimal number.
-
-    Supported SI suffixes:
-    base1024: Ki | Mi | Gi | Ti | Pi | Ei
-    base1000: n | u | m | "" | k | M | G | T | P | E
-
-    See:
-    https://github.com/kubernetes/apimachinery/blob/master/pkg/api/resource/quantity.go
-
-    Args:
-        quantity: kubernetes canonical form quantity
-
-    Returns:
-        Decimal
-
-    Raises:
-        ValueError: on invalid or unknown input
-    """
-    if isinstance(quantity, (int, float, Decimal)):
-        return Decimal(quantity)
-
-    exponents = {
-        "n": -3,
-        "u": -2,
-        "m": -1,
-        "K": 1,
-        "k": 1,
-        "M": 2,
-        "G": 3,
-        "T": 4,
-        "P": 5,
-        "E": 6,
-    }
-
-    quantity = str(quantity)
-    number = quantity
-    suffix = None
-    if len(quantity) >= 2 and quantity[-1] == "i":
-        if quantity[-2] in exponents:
-            number = quantity[:-2]
-            suffix = quantity[-2:]
-    elif len(quantity) >= 1 and quantity[-1] in exponents:
-        number = quantity[:-1]
-        suffix = quantity[-1:]
-
-    try:
-        number = Decimal(number)
-    except InvalidOperation:
-        raise ValueError("Invalid number format: {}".format(number))
-
-    if suffix is None:
-        return number
-
-    if suffix.endswith("i"):
-        base = 1024
-    elif len(suffix) == 1:
-        base = 1000
-    else:
-        raise ValueError("{} has unknown suffix".format(quantity))
-
-    # handle SI inconsistency
-    if suffix == "ki":
-        raise ValueError("{} has unknown suffix".format(quantity))
-
-    if suffix[0] not in exponents:
-        raise ValueError("{} has unknown suffix".format(quantity))
-
-    exponent = Decimal(exponents[suffix[0]])
-    return number * (base**exponent)
+__all__ = ["parse_quantity"]
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## orquestra/sdk/mlflow/__init__.py

```diff
@@ -1,14 +1,14 @@
 ################################################################################
-# © Copyright 2023 Zapata Computing Inc.
+# © Copyright 2024 Zapata Computing Inc.
 ################################################################################
+# THIS FILE IS A SHIM TO REEXPORT SYMBOLS AS PUBLIC API
+# DO NOT PUT ANY LOGIC INTO THIS FILE.
 
-"""A set of Orquestra utilities relating to interacting with MLFlow."""
-
-from ._connection_utils import (
+from .._client.mlflow import (
     get_current_user,
     get_temp_artifacts_dir,
     get_tracking_token,
     get_tracking_uri,
 )
 
 __all__ = [
```

## orquestra/sdk/packaging/__init__.py

```diff
@@ -1,17 +1,9 @@
 ################################################################################
-# © Copyright 2023 Zapata Computing Inc.
+# © Copyright 2024 Zapata Computing Inc.
 ################################################################################
+# THIS FILE IS A SHIM TO REEXPORT SYMBOLS AS PUBLIC API
+# DO NOT PUT ANY LOGIC INTO THIS FILE.
 
-from ._versions import (
-    InstalledImport,
-    PackagingError,
-    execute_task,
-    get_installed_version,
-)
+from orquestra.sdk._shared.packaging import PackagingError, get_installed_version
 
-__all__ = [
-    "InstalledImport",
-    "PackagingError",
-    "execute_task",
-    "get_installed_version",
-]
+__all__ = ["get_installed_version", "PackagingError"]
```

## orquestra/sdk/schema/__init__.py

```diff
@@ -1,13 +0,0 @@
-00000000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000020: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000050: 0a23 20c2 a920 436f 7079 7269 6768 7420  .# .. Copyright 
-00000060: 3230 3233 205a 6170 6174 6120 436f 6d70  2023 Zapata Comp
-00000070: 7574 696e 6720 496e 632e 0a23 2323 2323  uting Inc..#####
-00000080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000000a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000000b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000000c0: 2323 2323 2323 2323 2323 230a            ###########.
```

## orquestra/sdk/schema/configs.py

```diff
@@ -1,56 +1,23 @@
 ################################################################################
-# © Copyright 2023 - 2024 Zapata Computing Inc.
+# © Copyright 2024 Zapata Computing Inc.
 ################################################################################
-from enum import Enum
-from typing import Any, Dict, Literal
+# THIS FILE IS A SHIM TO REEXPORT SYMBOLS AS PUBLIC API
+# DO NOT PUT ANY LOGIC INTO THIS FILE.
 
-from .._base._storage import BaseModel
-
-CONFIG_FILE_CURRENT_VERSION = "0.0.2"
-
-ConfigName = str
-
-
-class RuntimeName(str, Enum):
-    RAY_LOCAL = "RAY_LOCAL"
-    CE_REMOTE = "CE_REMOTE"
-    QE_REMOTE = "QE_REMOTE"
-    IN_PROCESS = "IN_PROCESS"
-
-    def __format__(self, format_spec: str) -> str:
-        return format(self.value, format_spec)
-
-
-RemoteRuntime = Literal[RuntimeName.CE_REMOTE]
-
-
-class RuntimeConfiguration(BaseModel):
-    config_name: ConfigName
-    runtime_name: RuntimeName
-    runtime_options: Dict[str, Any] = {}
-
-    def __str__(self):
-        outstr = (
-            f"RuntimeConfiguration '{self.config_name}' with parameters:\n"
-            f"- runtime name: {self.runtime_name}\n"
-            "- runtime options:"
-        )
-        for key in self.runtime_options:
-            outstr += f"\n  - {key}: {self.runtime_options[key]}"
-        return outstr
-
-
-class RuntimeConfigurationFile(BaseModel):
-    """This schema is for the storage of "Runtime configurations".
-
-    The major version number should be bumped when:
-
-    * The values inside the configuration file are modified, for example if
-      the ``configs`` option is renamed or the type is changed.
-
-    * The shape of ``RuntimeConfiguration`` changes.
-    """
-
-    version: str
-    configs: Dict[ConfigName, RuntimeConfiguration]
-    default_config_name: ConfigName = "local"
+from orquestra.sdk._shared.schema.configs import (
+    CONFIG_FILE_CURRENT_VERSION,
+    ConfigName,
+    RemoteRuntime,
+    RuntimeConfiguration,
+    RuntimeConfigurationFile,
+    RuntimeName,
+)
+
+__all__ = [
+    "CONFIG_FILE_CURRENT_VERSION",
+    "ConfigName",
+    "RuntimeName",
+    "RemoteRuntime",
+    "RuntimeConfiguration",
+    "RuntimeConfigurationFile",
+]
```

## orquestra/sdk/schema/ir.py

```diff
@@ -1,466 +1,85 @@
 ################################################################################
-# © Copyright 2021 - 2024 Zapata Computing Inc.
+# © Copyright 2024 Zapata Computing Inc.
 ################################################################################
-"""Workflow Intermediate Representation.
+# THIS FILE IS A SHIM TO REEXPORT SYMBOLS AS PUBLIC API
+# DO NOT PUT ANY LOGIC INTO THIS FILE.
 
-The classes here are used only for purposes of schema definition. Every data
-structure here is JSON-serializable.
-"""
-
-import enum
-import typing as t
-import warnings
-
-import pydantic
-from typing_extensions import Annotated
-
-from .._base._storage import BaseModel, GpuResourceType, field_validator
-
-ImportId = str
-SecretNodeId = str
-
-
-class SecretNode(BaseModel):
-    """A reference to a secret stored in an external secret/config service."""
-
-    # Workflow-scope unique ID used to refer from task invocations
-    id: SecretNodeId
-
-    # Serialized value
-    secret_name: str
-
-    # Secret config
-    # This is only used locally, and we expect this to be None (or ignored) on remote
-    # runtimes.
-    secret_config: t.Optional[str] = None
-
-    # Workspace ID
-    # This is used locally and remotely to get a secret from a specific workspace
-    workspace_id: t.Optional[str] = None
-
-
-class GitURL(BaseModel):
-    original_url: str
-    protocol: str
-    user: t.Optional[str] = None
-    password: t.Optional[SecretNode] = None
-    host: str
-    port: t.Optional[int] = None
-    path: str
-    query: t.Optional[str] = None
-
-
-class GitImport(BaseModel):
-    id: ImportId
-    repo_url: GitURL
-    git_ref: str
-
-    # we need this in the JSON to know which class to use when deserializing
-    type: t.Literal["GIT_IMPORT"] = "GIT_IMPORT"
-
-    @field_validator("repo_url", mode="before")
-    def _backwards_compatible_repo_url(cls, v):
-        """Allows older models with a string URL to be imported."""
-        # Prevent circular imports
-        from .._base._git_url_utils import parse_git_url
-
-        if not isinstance(v, str):
-            return v
-
-        return parse_git_url(v)
-
-
-class LocalImport(BaseModel):
-    """Used to specify that the source code is only available locally.
-
-    (e.g. not committed to any git repo).
-    """
-
-    id: ImportId
-
-    # we need this in the JSON to know which class to use when deserializing
-    type: t.Literal["LOCAL_IMPORT"] = "LOCAL_IMPORT"
-
-
-class InlineImport(BaseModel):
-    id: ImportId
-    type: t.Literal["INLINE_IMPORT"] = "INLINE_IMPORT"
-
-
-class PackageSpec(BaseModel):
-    # noqa E501
-    """Representation of single package import.
-
-    The fields in this class are based on:
-    https://packaging.pypa.io/en/latest/requirements.html#packaging.requirements.Requirement
-
-    Look there for more information about valid string values.
-    """
-
-    name: str
-    extras: t.List[str]
-    version_constraints: t.List[str]
-    environment_markers: str
-
-
-class PythonImports(BaseModel):
-    """List of imports for given task."""
-
-    id: ImportId
-
-    # List of pip packages
-    packages: t.List[PackageSpec]
-    # List of pip options to put at start of the requirements
-    pip_options: t.List[str]
-
-    type: t.Literal["PYTHON_IMPORT"] = "PYTHON_IMPORT"
-
-
-# If we need more import types, add them here.
-Import = t.Union[GitImport, LocalImport, PythonImports, InlineImport]
-
-
-TaskDefId = str
-
-
-class ModuleFunctionRef(BaseModel):
-    # Required to dereference function for execution.
-    module: str
-    function_name: str
-
-    # Needed by Orquestra Studio to power jump-to-definition.
-    file_path: t.Optional[str] = None
-    line_number: t.Optional[int] = None
-
-    # We need this in the JSON to know which class to use when deserializing
-    type: t.Literal["MODULE_FUNCTION_REF"] = "MODULE_FUNCTION_REF"
-
-
-class FileFunctionRef(BaseModel):
-    # Required to dereference function for execution.
-    file_path: str
-    function_name: str
-
-    # Needed by Orquestra Studio to power jump-to-definition. `file_path` can
-    # be used for both execution and jump-to-definition.
-    line_number: t.Optional[int] = None
-
-    # We need this in the JSON to know which class to use when deserializing
-    type: t.Literal["FILE_FUNCTION_REF"] = "FILE_FUNCTION_REF"
-
-
-class InlineFunctionRef(BaseModel):
-    function_name: str
-    # Required to dereference function for execution. The function object is serialized
-    # using `dill`, base64-encoded, and chunked to workaround JSON string length limits.
-    encoded_function: t.List[str]
-
-    # We need this in the JSON to know which class to use when deserializing
-    type: t.Literal["INLINE_FUNCTION_REF"] = "INLINE_FUNCTION_REF"
-
-
-FunctionRef = t.Union[ModuleFunctionRef, FileFunctionRef, InlineFunctionRef]
-
-
-class Resources(BaseModel):
-    cpu: t.Optional[str] = None
-    memory: t.Optional[str] = None
-    disk: t.Optional[str] = None
-    gpu: GpuResourceType = None
-
-    # nodes should be a positive integer representing the number of nodes assigned
-    # to a workflow. If None, the runtime will choose.
-    # This only applies to workflows and not tasks.
-    nodes: t.Optional[int] = None
-
-
-class DataAggregation(BaseModel):
-    run: t.Optional[bool] = None
-    resources: t.Optional[Resources] = None
-
-
-ParameterName = str
-
-
-class ParameterKind(str, enum.Enum):
-    # Currently this uses the same naming as Python.
-    # We only use a subset of Python's kinds, however.
-    # See: https://docs.python.org/3/library/inspect.html#inspect.Parameter.kind
-    POSITIONAL_OR_KEYWORD = "POSITIONAL_OR_KEYWORD"
-    VAR_POSITIONAL = "VAR_POSITIONAL"
-    VAR_KEYWORD = "VAR_KEYWORD"
-
-
-class TaskParameter(BaseModel):
-    name: ParameterName
-    kind: ParameterKind
-    # If we need more metadata related to parameters, like type hints or default values,
-    # it should be added here.
-
-
-class TaskOutputMetadata(BaseModel):
-    """Information about the data shape returned by a task function."""
-
-    # If yes, it's possible to unpack the output in the workflow like:
-    # foo, bar = my_task()
-    #
-    # Separate from `n_outputs` to handle cases like:
-    # foo, = my_task()
-    is_subscriptable: bool
-
-    # Number of artifacts we can populate with the task results.
-    n_outputs: int
-
-
-class TaskDef(BaseModel):
-    # workflow-unique ID used to refer from task invocations
-    id: TaskDefId
-
-    fn_ref: FunctionRef
-
-    # `source_import_id` & `dependency_import_ids` are references to imports defined in
-    # Workflow.imports.
-
-    # List of abstract inputs that the task requires, but without the values yet.
-    # Kinda like function signature.
-    # None means we do not know the parameters for this Task (e.g. an external task)
-    # An empty list [] means a Task with no parameters
-    parameters: t.Optional[t.List[TaskParameter]] = None
-
-    # Statically inferred from the task function. See also `TaskOutputMetadata`'s
-    # docstring.
-    # 'None' for IRs generated with orquestra-sdk<=0.45.1. Not empty for newer SDK
-    # versions.
-    output_metadata: t.Optional[TaskOutputMetadata] = None
-
-    # ID of the import that contains the callable function
-    source_import_id: ImportId
-
-    # IDs of the imports that are needed at runtime to allow running the callable
-    dependency_import_ids: t.Optional[t.List[ImportId]] = None
-
-    resources: t.Optional[Resources] = None
-
-    max_retries: t.Optional[int] = None
-    # Hints the runtime to run this task in a docker container with this image. Has no
-    # effect if the runtime doesn't support it.
-    custom_image: t.Optional[str] = None
-
-
-class ArtifactFormat(str, enum.Enum):
-    """List of formats we allow for serializing constants & artifacts."""
-
-    # Try to figure out best serialization format based on object type at run time.
-    AUTO = "AUTO"
-
-    # Pickle -> Base64 string
-    ENCODED_PICKLE = "ENCODED_PICKLE"
-
-    # The artifact is serialized to a JSON string. Artifact value must be
-    # JSON-serializable.
-    JSON = "JSON"
-
-    # Unsupported yet. This is for demonstration purposes only at the moment.
-    NUMPY_ARRAY = "NUMPY_ARRAY"
-
-
-TaskInvocationId = str
-TaskNodeId = str
-ArtifactNodeId = str
-ConstantNodeId = str
-
-
-class ArtifactNode(BaseModel):
-    # Workflow-scope unique ID used to refer from task invocations. If the task has
-    # multiple outputs they will have distinct `id`s.
-    id: ArtifactNodeId
-
-    # artifact metadata below
-
-    # Optional name that can be used if human-readable strings are needed. If present,
-    # it's an addition to `id`, doesn't replace it.
-    custom_name: t.Optional[str] = None
-
-    # Tells runtime how to serialize artifact value after task invocation returns it.
-    # At the moment it's unknown where exactly the artifacts will be persisted, but some
-    # serialization will likely be needed somewhere.
-    serialization_format: ArtifactFormat = ArtifactFormat.AUTO
-
-    # Index of the variable when destructuring task result in the workflow function. If
-    # the workflow contained `foo, bar = my_task()`, `foo`'s index is 0 and `bar`'s
-    # index is 1. This is used by some runtimes to extract the artifact value from the
-    # output tuple.
-    #
-    # `None` if the task result isn't destructured in the workflow function.
-    artifact_index: t.Optional[int] = None
-
-
-class ConstantNodeJSON(BaseModel):
-    """Piece of data that already exists at workflow submission time.
-
-    The value is directly embedded in the workflow. To support arbitrary data shapes we
-    keep the value in a serialized form. This Node contains only JSON-serializable
-    values.
-    """
-
-    # Workflow-scope unique ID used to refer from task invocations
-    id: ConstantNodeId
-
-    # Serialized value
-    value: str
-    serialization_format: t.Literal[ArtifactFormat.JSON] = ArtifactFormat.JSON
-
-    # Human-readable string that can be rendered on the UI to represent the value.
-    value_preview: pydantic.constr(max_length=12)  # type: ignore
-
-
-class ConstantNodePickle(BaseModel):
-    """Piece of data that already exists at workflow submission time.
-
-    The value is directly embedded in the workflow. To support arbitrary data shapes we
-    keep the value in a serialized form. Pickling constants is a fallback for storing
-    values that are not JSON-serializable.
-    """
-
-    # Workflow-scope unique ID used to refer from task invocations
-    id: ConstantNodeId
-
-    # Serialized value
-    chunks: t.List[str]
-    serialization_format: t.Literal[
-        ArtifactFormat.ENCODED_PICKLE
-    ] = ArtifactFormat.ENCODED_PICKLE
-
-    # Human-readable string that can be rendered on the UI to represent the value.
-    value_preview: pydantic.constr(max_length=12)  # type: ignore
-
-
-# General ConstantNode that can hold constants that are not JSON-serializable
-ConstantNode = t.Union[ConstantNodeJSON, ConstantNodePickle]
-# ID of a node that can be a task argument. Multiple node types can be task inputs.
-# This is contrary to the outputs; only artifact nodes can be task outputs.
-ArgumentId = t.Union[ArtifactNodeId, ConstantNodeId, SecretNodeId]
-
-
-class TaskInvocation(BaseModel):
-    id: TaskInvocationId
-
-    # What task should be executed.
-    task_id: TaskDefId
-
-    args_ids: t.List[ArgumentId]
-    # Key: task parameter name. Should match one of parameters of the `Task` referenced
-    #     by `task_id`.
-    # Value: id of the constant or artifact that will contain the value at runtime.
-    kwargs_ids: t.Dict[ParameterName, ArgumentId]
-
-    # Where to store the returned values.
-    output_ids: t.List[ArtifactNodeId]
-
-    # TaskInvocation specific resources
-    resources: t.Optional[Resources] = None
-
-    # Specification for custom image more scoped than TaskDef custom_image field
-    # if not set, will fall back to TaskDef custom_image
-    custom_image: t.Optional[str] = None
-
-
-WorkflowDefName = str
-
-
-class Version(BaseModel):
-    original: str
-    major: int
-    minor: int
-    patch: int
-    is_prerelease: bool
-
-
-class WorkflowMetadata(BaseModel):
-    sdk_version: Version
-    python_version: Version
-
-
-class WorkflowDef(BaseModel):
-    """The main data structure for intermediate workflow representation.
-
-    The structure is as flat as possible with relation based on "id"s, e.g. a single
-    task invocation has a relation to the task it invokes, argument artifacts or
-    constants and returned artifacts.
-    """
-
-    name: WorkflowDefName
-
-    # Used by Orquestra Studio to power jump-to-definition (file_path + line_number).
-    fn_ref: FunctionRef
-
-    # nodes with IDs & metadata
-    imports: t.Dict[ImportId, Import]
-    tasks: t.Dict[TaskDefId, TaskDef]
-    artifact_nodes: t.Dict[ArtifactNodeId, ArtifactNode]
-    constant_nodes: t.Dict[ConstantNodeId, ConstantNode]
-    secret_nodes: t.Dict[SecretNodeId, SecretNode] = {}
-
-    # The actual graph in form node clusters ("invocations"). Each task invocation is a
-    # small subgraph with TaskNode in the center and connections to data nodes
-    # (ArtifactNode or ConstantNode). This representation allows to easily specify order
-    # of arguments or returned values.
-    task_invocations: t.Dict[TaskInvocationId, TaskInvocation]
-
-    # IDs of the nodes that are considered as workflow outputs. The referenced nodes
-    # can be constants or artifacts.
-    output_ids: t.List[ArgumentId]
-
-    data_aggregation: t.Optional[DataAggregation] = None
-
-    # Metadata defaults to None to allow older JSON to be loaded
-    metadata: Annotated[
-        t.Optional[WorkflowMetadata], pydantic.Field(validate_default=True)
-    ] = None
-
-    # The resources that are available for the workflow to use.
-    # If none, the runtime will decide.
-    resources: t.Optional[Resources] = None
-
-    @field_validator("metadata", mode="after")
-    def sdk_version_up_to_date(cls, v: t.Optional[WorkflowMetadata]):
-        # Workaround for circular imports
-        from orquestra.sdk import exceptions
-        from orquestra.sdk.packaging import _versions
-        from orquestra.sdk.schema import _compat
-
-        current_version = _versions.get_current_sdk_version()
-
-        if v is None:
-            warnings.warn(
-                exceptions.VersionMismatch(
-                    (
-                        "Attempting to read a workflow definition generated with an "
-                        "old version of Orquestra Workflow SDK. Please consider "
-                        "re-running your workflow or downgrading orquestra-sdk. "
-                        "For more information visit: https://docs.orquestra.io/docs/core/sdk/guides/version-compatibility.html"  # noqa: E501
-                    ),
-                    actual=current_version,
-                    needed=None,
-                )
-            )
-            return v
-
-        if not _compat.versions_are_compatible(
-            generated_at=v.sdk_version, current=current_version
-        ):
-            warnings.warn(
-                exceptions.VersionMismatch(
-                    (
-                        "Attempting to read a workflow definition generated with a "
-                        "different version of Orquestra Workflow SDK. "
-                        "Please consider re-running your workflow or installing "
-                        f"'orquestra-sdk=={v.sdk_version.original}'. "
-                        "For more information visit: https://docs.orquestra.io/docs/core/sdk/guides/version-compatibility.html"  # noqa: E501
-                    ),
-                    actual=current_version,
-                    needed=v.sdk_version,
-                )
-            )
-
-        return v
+from orquestra.sdk._shared.schema.ir import (
+    ArgumentId,
+    ArtifactFormat,
+    ArtifactNode,
+    ArtifactNodeId,
+    ConstantNode,
+    ConstantNodeId,
+    ConstantNodeJSON,
+    ConstantNodePickle,
+    DataAggregation,
+    FileFunctionRef,
+    FunctionRef,
+    GitImport,
+    GitURL,
+    Import,
+    ImportId,
+    InlineFunctionRef,
+    InlineImport,
+    LocalImport,
+    ModuleFunctionRef,
+    PackageSpec,
+    ParameterKind,
+    ParameterName,
+    PythonImports,
+    Resources,
+    SecretNode,
+    SecretNodeId,
+    TaskDef,
+    TaskDefId,
+    TaskInvocation,
+    TaskInvocationId,
+    TaskNodeId,
+    TaskOutputMetadata,
+    TaskParameter,
+    Version,
+    WorkflowDef,
+    WorkflowDefName,
+    WorkflowMetadata,
+)
+
+__all__ = [
+    "ArgumentId",
+    "ArtifactFormat",
+    "ArtifactNode",
+    "ArtifactNodeId",
+    "ConstantNode",
+    "ConstantNodeId",
+    "ConstantNodeJSON",
+    "ConstantNodePickle",
+    "DataAggregation",
+    "FileFunctionRef",
+    "FunctionRef",
+    "GitImport",
+    "GitURL",
+    "Import",
+    "ImportId",
+    "InlineFunctionRef",
+    "InlineImport",
+    "LocalImport",
+    "ModuleFunctionRef",
+    "PackageSpec",
+    "ParameterKind",
+    "ParameterName",
+    "PythonImports",
+    "Resources",
+    "SecretNode",
+    "SecretNodeId",
+    "TaskDef",
+    "TaskDefId",
+    "TaskInvocation",
+    "TaskInvocationId",
+    "TaskNodeId",
+    "TaskOutputMetadata",
+    "TaskParameter",
+    "Version",
+    "WorkflowDef",
+    "WorkflowDefName",
+    "WorkflowMetadata",
+]
```

## orquestra/sdk/schema/responses.py

```diff
@@ -1,81 +1,27 @@
 ################################################################################
-# © Copyright 2022 - 2024 Zapata Computing Inc.
+# © Copyright 2024 Zapata Computing Inc.
 ################################################################################
-"""Models for responses from the CLI.
+# THIS FILE IS A SHIM TO REEXPORT SYMBOLS AS PUBLIC API
+# DO NOT PUT ANY LOGIC INTO THIS FILE.
 
-The classes here are used only for purposes of schema definition. Every data
-structure here is JSON-serializable.
-"""
-
-import enum
-import typing as t
-
-from pydantic import Field
-from typing_extensions import Annotated
-
-from .._base._storage import BaseModel
-from .ir import ArtifactFormat
-
-
-class ResponseFormat(enum.Enum):
-    PLAIN_TEXT = "text"
-    JSON = "json"
-    DEFAULT = PLAIN_TEXT
-
-
-class ResponseStatusCode(enum.Enum):
-    UNKNOWN_ERROR = -1
-    OK = 0
-    PERMISSION_ERROR = 1
-    NOT_FOUND = 2
-    NOT_A_DIRECTORY = 3
-    PROJECT_EXISTS = 4
-    INVALID_PROJECT = 5
-    INVALID_TASK_DEF = 6
-    INVALID_WORKFLOW_DEF = 7
-    INVALID_WORKFLOW_DEFS_SYNTAX = 8
-    INVALID_WORKFLOW_RUN = 9
-    WORKFLOW_RUN_NOT_FOUND = 10
-    CONNECTION_ERROR = 11
-    UNAUTHORIZED = 12
-    SERVICES_ERROR = 13
-    INVALID_CLI_COMMAND_ERROR = 14
-    USER_CANCELLED = 15
-
-
-class ResponseMetadata(BaseModel):
-    success: bool
-    code: ResponseStatusCode
-    message: str
-
-
-class JSONResult(BaseModel):
-    # Output value dumped to a flat JSON string.
-    value: str
-    serialization_format: t.Literal[ArtifactFormat.JSON] = ArtifactFormat.JSON
-
-
-class PickleResult(BaseModel):
-    # Output value dumped to a pickle byte string, encoded as base64, and split into
-    # chunks. Chunking is required because some JSON parsers have limitation on max
-    # string field length.
-    chunks: t.List[str]
-    serialization_format: t.Literal[
-        ArtifactFormat.ENCODED_PICKLE
-    ] = ArtifactFormat.ENCODED_PICKLE
-
-
-WorkflowResult = Annotated[
-    t.Union[JSONResult, PickleResult], Field(discriminator="serialization_format")
+from orquestra.sdk._shared.schema.responses import (
+    ComputeEngineWorkflowResult,
+    JSONResult,
+    PickleResult,
+    ResponseFormat,
+    ResponseMetadata,
+    ResponseStatusCode,
+    ServiceResponse,
+    WorkflowResult,
+)
+
+__all__ = [
+    "ResponseFormat",
+    "ResponseStatusCode",
+    "ResponseMetadata",
+    "JSONResult",
+    "PickleResult",
+    "WorkflowResult",
+    "ComputeEngineWorkflowResult",
+    "ServiceResponse",
 ]
-
-
-class ComputeEngineWorkflowResult(BaseModel):
-    results: t.Tuple[WorkflowResult, ...]
-    type: t.Literal["ComputeEngineWorkflowResult"] = "ComputeEngineWorkflowResult"
-
-
-class ServiceResponse(BaseModel):
-    name: str
-    is_running: bool
-    info: t.Optional[str]
```

## orquestra/sdk/schema/workflow_run.py

```diff
@@ -1,116 +1,33 @@
 ################################################################################
-# © Copyright 2022 - 2024 Zapata Computing Inc.
+# © Copyright 2024 Zapata Computing Inc.
 ################################################################################
-"""Workflow Run model.
+# THIS FILE IS A SHIM TO REEXPORT SYMBOLS AS PUBLIC API
+# DO NOT PUT ANY LOGIC INTO THIS FILE.
 
-The classes here are used only for purposes of schema definition. Every data
-structure here is JSON-serializable.
-"""
-
-import enum
-import typing as t
-import warnings
-
-from orquestra.sdk._base._dates import Instant
-from orquestra.sdk.schema.ir import TaskInvocationId, WorkflowDef
-
-from .._base._storage import BaseModel
-
-WorkflowRunId = str
-TaskRunId = str
-WorkspaceId = str
-ProjectId = str
-
-
-class State(enum.Enum):
-    WAITING = "WAITING"
-    RUNNING = "RUNNING"
-    SUCCEEDED = "SUCCEEDED"
-    TERMINATED = "TERMINATED"
-    FAILED = "FAILED"
-    ERROR = "ERROR"
-    KILLED = "KILLED"
-    UNKNOWN = "UNKNOWN"
-
-    @classmethod
-    def _missing_(cls, value):
-        return cls.UNKNOWN
-
-    def is_completed(self) -> bool:
-        """Check whether the state indicates that execution of the wf run has ended.
-
-        Returns:
-            True if the execution has ended for any reason, False if the workflow run
-                is waiting or running.
-        """
-        if self == self.UNKNOWN:
-            warnings.warn("Cannot determine the workflow run state.")
-
-        return self in (
-            self.SUCCEEDED,
-            self.TERMINATED,
-            self.FAILED,
-            self.ERROR,
-            self.KILLED,
-        )
-
-
-class RunStatus(BaseModel):
-    state: State
-    start_time: t.Optional[Instant]
-    end_time: t.Optional[Instant]
-
-
-class TaskRun(BaseModel):
-    id: TaskRunId
-    invocation_id: TaskInvocationId
-    status: RunStatus
-    message: t.Optional[str] = None
-
-
-class WorkflowRunOnlyID(BaseModel):
-    """A WorkflowRun that only contains the ID."""
-
-    id: WorkflowRunId
-
-
-class WorkflowRunMinimal(WorkflowRunOnlyID):
-    """The minimal amount of information to create a WorkflowRun in the public API."""
-
-    workflow_def: WorkflowDef
-
-
-class WorkflowRun(WorkflowRunMinimal):
-    """A full workflow run with TaskRuns and WorkflowRun status."""
-
-    task_runs: t.List[TaskRun]
-    status: RunStatus
-    message: t.Optional[str] = None
-
-
-class WorkflowRunSummary(WorkflowRunOnlyID):
-    """A summary overview of a workflow run."""
-
-    status: RunStatus
-    owner: t.Optional[str]
-    """
-    The email address of the account that submitted this workflow run.
-
-    For local runs, this field is not populated.
-    """
-    total_task_runs: int
-    completed_task_runs: int
-    dry_run: t.Optional[bool]
-
-    @staticmethod
-    def from_workflow_run(wf: WorkflowRun) -> "WorkflowRunSummary":
-        return WorkflowRunSummary(
-            id=wf.id,
-            status=wf.status,
-            owner=None,
-            total_task_runs=len(wf.workflow_def.task_invocations),
-            completed_task_runs=sum(
-                1 for tr in wf.task_runs if tr.status.state == State.SUCCEEDED
-            ),
-            dry_run=None,
-        )
+from orquestra.sdk._shared.schema.workflow_run import (
+    ProjectId,
+    RunStatus,
+    State,
+    TaskRun,
+    TaskRunId,
+    WorkflowRun,
+    WorkflowRunId,
+    WorkflowRunMinimal,
+    WorkflowRunOnlyID,
+    WorkflowRunSummary,
+    WorkspaceId,
+)
+
+__all__ = [
+    "WorkflowRunId",
+    "TaskRunId",
+    "WorkspaceId",
+    "ProjectId",
+    "State",
+    "RunStatus",
+    "TaskRun",
+    "WorkflowRunOnlyID",
+    "WorkflowRunMinimal",
+    "WorkflowRun",
+    "WorkflowRunSummary",
+]
```

## orquestra/sdk/secrets/__init__.py

```diff
@@ -1,29 +1,14 @@
 ################################################################################
-# © Copyright 2022-2023 Zapata Computing Inc.
+# © Copyright 2024 Zapata Computing Inc.
 ################################################################################
-"""Utility for accessing secrets managed by Orquestra.
+# THIS FILE IS A SHIM TO REEXPORT SYMBOLS AS PUBLIC API
+# DO NOT PUT ANY LOGIC INTO THIS FILE.
 
-You can use it both within an Orquestra Task code and a standalone script.
-
-The secrets values are always stored on an Orquestra server, even if you're using
-this class on your local machine.
-
-This module's behavior depends on the execution context (in a standalone REPL/script,
-in a workflow on the Local Runtime, in a workflow on Orquestra Platform).
-
-When you're using ``orquestra.sdk.secrets`` on your machine (inside a standalone script
-or with the Local Ray Runtime), this class uses cluster credentials read from your
-config file (set by ``orq login``).
-
-When ``orquestra.sdk.secrets`` is used inside a task running remotely on the Orquestra
-Platform, it uses a server-side authorization mechanism handled automatically.
-"""
-
-from ._api import delete, get, list, set
+from orquestra.sdk._client.secrets import delete, get, list, set
 
 __all__ = [
     "delete",
     "get",
     "list",
     "set",
 ]
```

## Comparing `orquestra/sdk/_base/_ast.py` & `orquestra/sdk/_client/_base/_ast.py`

 * *Files 13% similar despite different names*

```diff
@@ -62,61 +62,66 @@
 
     def _fail_single(
         self,
         node: ast.AST,
         message: str,
     ):
         LOG.debug(message)
+        self._add_single()
+
+    def _add_single(self):
         self.outputs.add(_AstReturnMetadata(is_subscriptable=False, n_outputs=1))
 
+    def _add_sequence(self, node, elements: t.List[ast.expr]):
+        # If there is a starred node in the list, then unpacking is used
+        if any(isinstance(e, ast.Starred) for e in elements):
+            self._fail_single(node, "Cannot infer number of outputs with unpacking")
+            return
+
+        n_elements = len(elements)
+        if n_elements == 0:
+            # Empty list counts as a single output, similarly to void functions
+            # having a single `None` output.
+            self._add_single()
+        else:
+            self.outputs.add(
+                _AstReturnMetadata(is_subscriptable=True, n_outputs=n_elements)
+            )
+
     def visit_Constant(self, node):
-        self.outputs.add(_AstReturnMetadata(is_subscriptable=False, n_outputs=1))
+        self._add_single()
 
     def visit_Name(self, node):
-        self.outputs.add(_AstReturnMetadata(is_subscriptable=False, n_outputs=1))
+        self._add_single()
 
     def visit_Attribute(self, node):
-        self.visit_Name(node)
+        self._add_single()
 
     def visit_JoinedStr(self, node):
         # f-strings
-        self.visit_Constant(node)
+        self._add_single()
 
     def visit_Set(self, node):
         # Sets are python objects and are not subscriptable
-        self.outputs.add(_AstReturnMetadata(is_subscriptable=False, n_outputs=1))
+        self._add_single()
 
     def visit_Tuple(self, node):
-        self.visit_List(node)
+        self._add_sequence(node, node.elts)
 
     def visit_List(self, node):
-        # If there is a starred node in the list, then unpacking is used
-        is_starred = [isinstance(e, ast.Starred) for e in node.elts]
-        if any(is_starred):
-            self._fail_single(node, "Cannot infer number of outputs with unpacking")
-            return
-
-        n_elements = len(node.elts)
-        if n_elements == 0:
-            # Empty list counts as a single output, similarly to void functions
-            # having a single `None` output.
-            self.outputs.add(_AstReturnMetadata(is_subscriptable=False, n_outputs=1))
-        else:
-            self.outputs.add(
-                _AstReturnMetadata(is_subscriptable=True, n_outputs=n_elements)
-            )
+        self._add_sequence(node, node.elts)
 
     def visit_Dict(self, node):
         # "None" inside the keys means there is dictionary unpacking being used
         # If None is used as a key, it is represented by an AST node
         if None in node.keys:
             self._fail_single(node, "Cannot infer number of outputs with unpacking")
             return
 
-        self.outputs.add(_AstReturnMetadata(is_subscriptable=False, n_outputs=1))
+        self._add_single()
 
     def generic_visit(self, node):
         self._fail_single(node, f"Assuming a single output for node {repr(type(node))}")
 
 
 def normalize_indents(source: str) -> str:
     lines = source.splitlines()
```

## Comparing `orquestra/sdk/_base/_config.py` & `orquestra/sdk/_client/_base/_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from pathlib import Path
 from typing import Any, List, Mapping, Optional, Union
 from urllib.parse import ParseResult, urlparse
 
 import filelock
 from pydantic import ValidationError
 
-import orquestra.sdk.exceptions as exceptions
-from orquestra.sdk.schema.configs import (
+import orquestra.sdk._shared.exceptions as exceptions
+from orquestra.sdk._shared.schema.configs import (
     CONFIG_FILE_CURRENT_VERSION,
     ConfigName,
     RuntimeConfiguration,
     RuntimeConfigurationFile,
     RuntimeName,
 )
```

## Comparing `orquestra/sdk/_base/_dates.py` & `orquestra/sdk/_shared/dates/_dates.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/_base/_dsl.py` & `orquestra/sdk/_client/_base/_dsl.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,30 +26,32 @@
     Iterable,
     List,
     NamedTuple,
     Optional,
     Tuple,
     TypeVar,
     Union,
-    cast,
     overload,
 )
 
-from typing_extensions import ParamSpec
-
 if TYPE_CHECKING:
-    import pip_api
+    from pip_api._parse_requirements import Requirement
 
 import wrapt  # type: ignore
 
 # Needed for fully-qualified type annotations.
 import orquestra.sdk
+from orquestra.sdk._shared.exceptions import (
+    DirtyGitRepo,
+    InvalidTaskDefinitionError,
+    WorkflowSyntaxError,
+)
+from orquestra.sdk._shared.kubernetes.quantity import parse_quantity
+from orquestra.sdk._shared.packaging import PackagingError, get_installed_version
 
-from ..exceptions import DirtyGitRepo, InvalidTaskDefinitionError, WorkflowSyntaxError
-from ..kubernetes.quantity import parse_quantity
 from . import _ast
 
 # ----- SDK exceptions  -----
 
 
 class NoRemoteRepo(Exception):
     pass
@@ -80,14 +82,17 @@
     "Invalid usage of a Secret object. Secrets are not "
     "available when building the workflow graph and cannot"
     " be used as strings. If you need to use a Secret's"
     " value, this must be done inside of a task."
 )
 
 
+_TaskReturn = TypeVar("_TaskReturn")
+
+
 class Secret(NamedTuple):
     name: str
     # Config name is only used for the local runtimes where we can't infer the location
     # where we get a secret's value from.
     # This matches the behaviour of `sdk.secrets.get` where the config name is used to
     # get a secret when running locally.
     config_name: Optional[str] = None
@@ -135,15 +140,15 @@
     """A task import that uses a Git repository."""
 
     repo_url: str
     git_ref: str
 
     @staticmethod
     def infer(
-        local_repo_path: Union[str, os.PathLike] = Path("."),
+        local_repo_path: Union[str, os.PathLike] = Path(""),
         git_ref: Optional[str] = None,
     ) -> "DeferredGitImport":
         """Get local Git info for a specific local repo.
 
         The current git repo info is retrieved as default.
 
         Args:
@@ -276,16 +281,16 @@
         self._file: Optional[Path]
         if file is not None:
             self._file = pathlib.Path(file)
         else:
             self._file = None
         self._packages = packages
 
-    def resolved(self) -> List[pip_api.Requirement]:
-        import pip_api
+    def resolved(self) -> List[Requirement]:
+        from pip_api._parse_requirements import Requirement, parse_requirements
 
         # on Windows file cannot be reopened when it's opened with delete=True
         # So the temp file is closed first and then deleted manually.
         tmp_file = NamedTemporaryFile(mode="w+", delete=False)
         if self._file is not None:
             # gather all requirements from file
             with open(self._file) as file:
@@ -294,25 +299,23 @@
                 tmp_file.write(line)
         # gather all requirements passed by the user
         for package in self._packages:
             tmp_file.write(f"{package}\n")
         tmp_file.flush()
         tmp_file.close()
         # reading all requirements as one parse to avoid conflicts
-        requirements = pip_api.parse_requirements(
+        requirements = parse_requirements(
             pathlib.Path(tmp_file.name), include_invalid=False
         )
         os.unlink(tmp_file.name)
 
         # with include_invalid - parsing will never return invalid_requirement type,
         # but mypy doesn't detect that, so this list comp. is to satisfy mypy
         # (and make it type-safe just-in-case
-        return [
-            req for req in requirements.values() if isinstance(req, pip_api.Requirement)
-        ]
+        return [req for req in requirements.values() if isinstance(req, Requirement)]
 
     def __eq__(self, other):
         if not isinstance(other, PythonImports):
             return False
 
         return self._file == other._file and self._packages == other._packages
 
@@ -483,60 +486,58 @@
                 category=UnknownPlaceholderInCustomNameWarning,
             )
         else:
             format_dict[ph] = signature.arguments[ph]
     return custom_name.format(**format_dict)
 
 
-_P = ParamSpec("_P")
-_R = TypeVar("_R")
-
-
-class TaskDef(Generic[_P, _R], wrapt.ObjectProxy):
+class TaskDef(wrapt.ObjectProxy, Generic[_TaskReturn]):
     """A function exposed to Orquestra.
 
     This is the result of applying the @task decorator.
 
     We do some magic to transform Python code in the workflow function decorated
     function to build the computational workflow graph. Use the `.model` property to
     get the serializable form.
     """
 
     # The fully-qualified type hint is a workaround for docs' autoapi not being able to
     # resolve symbols.
 
     def __init__(
         self,
-        fn: Callable[_P, _R],
-        output_metadata: "orquestra.sdk._base._dsl.TaskOutputMetadata",
+        fn: Callable[..., _TaskReturn],
+        output_metadata: "orquestra.sdk._client._base._dsl.TaskOutputMetadata",  # pyright: ignore # NOQA
         source_import: Optional[Import] = None,
         parameters: Optional[OrderedDict] = None,
         dependency_imports: Optional[Tuple[Import, ...]] = None,
         resources: Resources = Resources(),
         custom_image: Optional[str] = None,
         custom_name: Optional[str] = None,
         fn_ref: Optional[FunctionRef] = None,
         max_retries: Optional[int] = None,
+        env_vars: Optional[Dict[str, str]] = None,
     ):
         if isinstance(fn, BuiltinFunctionType):
             raise NotImplementedError("Built-in functions are not supported as Tasks")
-        super(TaskDef, self).__init__(fn)
+        super().__init__(fn)
         self.__sdk_task_body = fn
         self._fn_ref = fn_ref
         self._fn_name = fn.__name__
         self._output_metadata = output_metadata
         self._parameters = parameters
         self._resources = resources
         self._custom_image = custom_image
         self._custom_name = custom_name
         self._dependency_imports = dependency_imports
         self._use_default_dependency_imports = dependency_imports is None
         self._source_import = source_import
         self._use_default_source_import = source_import is None
         self._max_retries = max_retries
+        self._env_vars = env_vars
 
         # task itself is not part of any workflow yet. Don't pass wf defaults
         self._resolve_task_source_data()
 
     @property
     def n_outputs(self):
         warnings.warn(
@@ -599,15 +600,17 @@
         """
         try:
             self._validate_task_not_in_main()
             self._validate_task_resources()
         except InvalidTaskDefinitionError:
             raise
 
-    def __call__(self, *args: _P.args, **kwargs: _P.kwargs) -> _R:
+    def __call__(
+        self, *args: Union[ArtifactFuture, Any], **kwargs: Union[ArtifactFuture, Any]
+    ) -> ArtifactFuture[_TaskReturn]:
         try:
             signature = inspect.signature(self.__sdk_task_body).bind(*args, **kwargs)
         except TypeError as exc:
             # Check if an error is generated when the args and kwargs of the task call
             # are bonded to the args and kwargs of the task function.
             summary = traceback.StackSummary.extract(
                 traceback.walk_stack(None)
@@ -623,26 +626,24 @@
             if re.match(missing_self_arg, str(exc)):
                 error_message = (
                     f"The task {self._fn_name} seems to be a method, if so"
                     " modify it to not be a method.\n"
                 ) + error_message
             raise WorkflowSyntaxError(error_message) from exc
 
-        return cast(
-            _R,
-            ArtifactFuture(
-                TaskInvocation(
-                    self,
-                    args=args,
-                    kwargs=tuple(kwargs.items()),
-                    resources=self._resources,
-                    custom_name=parse_custom_name(self._custom_name, signature),
-                    custom_image=self._custom_image,
-                )
-            ),
+        return ArtifactFuture(
+            TaskInvocation(
+                self,
+                args=args,
+                kwargs=tuple(kwargs.items()),
+                resources=self._resources,
+                custom_name=parse_custom_name(self._custom_name, signature),
+                custom_image=self._custom_image,
+                env_vars=self._env_vars,
+            )
         )
 
     def _resolve_task_source_data(
         self, wf_default_source_import: Optional[Import] = None
     ):
         # if user set source import explicitly, we use that import
         # else we either take wf default, or base on if the session is interactive
@@ -675,15 +676,15 @@
             self._dependency_imports = wf_default_dependency_imports
 
 
 # TaskInvocation is using a Plain Old Python Object on purpose:
 # Using POPO instead of a NamedTuple means each instance of TaskInvocation
 # is unique, even if they share the exact same attributes. This is required
 # for the traversal of the graph.
-class TaskInvocation:
+class TaskInvocation(Generic[_TaskReturn]):
     task: TaskDef
 
     args: Tuple[Argument, ...]
 
     # NOTE: Some time ago we needed this to be hashable, hence we went with a tuple of
     # key-value pairs instead of a mapping. It can be changed to a dict.
     kwargs: Tuple[Tuple[str, Argument], ...]
@@ -692,39 +693,42 @@
 
     # invocation metadata below
     resources: Resources = Resources()
     custom_image: Optional[str] = None
 
     def __init__(
         self,
-        task: TaskDef,
+        task: TaskDef[_TaskReturn],
         args: Tuple[Argument, ...],
         kwargs: Tuple[Tuple[str, Argument], ...],
         type: str = "task_invocation",
         resources: Resources = Resources(),
         custom_name: Optional[str] = None,
         custom_image: Optional[str] = None,
+        env_vars: Optional[Dict[str, str]] = None,
     ):
         self.task = task
         self.args = args
         self.kwargs = kwargs
         self.resources = resources
         self.type = type
         self.custom_name = custom_name
         self.custom_image = custom_image
+        self.env_vars = env_vars
 
     def _asdict(self) -> Dict[str, Any]:
         return {
             "task": self.task,
             "args": self.args,
             "kwargs": self.kwargs,
             "type": self.type,
             "resources": self.resources,
             "custom_name": self.custom_name,
             "custom_image": self.custom_image,
+            "env_vars": self.env_vars,
         }
 
 
 class Sentinel(Enum):
     NO_UPDATE = object()
 
 
@@ -737,32 +741,34 @@
     # See: orquestra.sdk.schema.ir.ArtifactFormat
     #
     # Add more cases here when we allow users to specify artifact format explicitly.
     # This has to be accompanied by corresponding implementation in orquestra.sdk._base.
     AUTO = "AUTO"
 
 
-class ArtifactFuture:
+class ArtifactFuture(Generic[_TaskReturn]):
     DEFAULT_CUSTOM_NAME = None
     DEFAULT_SERIALIZATION_FORMAT = ArtifactFormat.AUTO
 
     def __init__(
         self,
-        invocation: orquestra.sdk._base._dsl.TaskInvocation,
+        invocation: TaskInvocation[_TaskReturn],
         output_index: Optional[int] = None,
         custom_name: Optional[str] = DEFAULT_CUSTOM_NAME,
-        serialization_format: orquestra.sdk._base._dsl.ArtifactFormat = DEFAULT_SERIALIZATION_FORMAT,  # noqa: E501
+        serialization_format: ArtifactFormat = DEFAULT_SERIALIZATION_FORMAT,
+        env_vars: Optional[Dict[str, str]] = None,
     ):
         self.invocation = invocation
         # if the invocation returns multiple values, this the index in the output
         # sequence
         self.output_index = output_index
         # metadata below
         self.custom_name = custom_name
         self.serialization_format = serialization_format
+        self.env_vars = env_vars
 
     def __repr__(self):
         return (
             "ArtifactFuture("
             f"invocation={self.invocation}, "
             f"output_index={self.output_index}, "
             f"custom_name={self.custom_name}, "
@@ -816,27 +822,33 @@
     # The fully-qualified type hint is a workaround for docs' autoapi not being able to
     # resolve symbols.
 
     def with_invocation_meta(
         self,
         *,
         cpu: Optional[
-            Union[str, "orquestra.sdk._base._dsl.Sentinel"]
+            Union[str, "orquestra.sdk._client._base._dsl.Sentinel"]  # pyright: ignore
         ] = Sentinel.NO_UPDATE,
         memory: Optional[
-            Union[str, "orquestra.sdk._base._dsl.Sentinel"]
+            Union[str, "orquestra.sdk._client._base._dsl.Sentinel"]  # pyright: ignore
         ] = Sentinel.NO_UPDATE,
         disk: Optional[
-            Union[str, "orquestra.sdk._base._dsl.Sentinel"]
+            Union[str, "orquestra.sdk._client._base._dsl.Sentinel"]  # pyright: ignore
         ] = Sentinel.NO_UPDATE,
         gpu: Optional[
-            Union[str, "orquestra.sdk._base._dsl.Sentinel"]
+            Union[str, "orquestra.sdk._client._base._dsl.Sentinel"]  # pyright: ignore
         ] = Sentinel.NO_UPDATE,
         custom_image: Optional[
-            Union[str, "orquestra.sdk._base._dsl.Sentinel"]
+            Union[str, "orquestra.sdk._client._base._dsl.Sentinel"]  # pyright: ignore
+        ] = Sentinel.NO_UPDATE,
+        env_vars: Optional[
+            Union[
+                Dict[str, str],
+                "orquestra.sdk._client._base._dsl.Sentinel",  # pyright: ignore
+            ]
         ] = Sentinel.NO_UPDATE,
     ) -> "ArtifactFuture":
         """
         Assigns optional metadata related to task invocation used to generate this
         artifact.
 
         Doesn't modify existing invocations, returns a new one.
@@ -849,14 +861,15 @@
 
         Args:
             cpu: amount of cpu assigned to the task invocation
             memory: amount of memory assigned to the task invocation
             disk: amount of disk assigned to the task invocation
             gpu: amount of gpu assigned to the task invocation
             custom_image: docker image used to run the task invocation
+            env_vars: dict of environmental variables to be used in task
         """  # noqa: D205, D212
         self._check_if_destructured(
             fn_name=self.invocation.task._fn_name,
             assign_type="invocation metadata",
         )
 
         # Only use the new properties if they have not been changed.
@@ -876,21 +889,27 @@
         new_custom_image: Optional[str]
 
         if custom_image is not Sentinel.NO_UPDATE:
             new_custom_image = custom_image
         else:
             new_custom_image = invocation.custom_image
 
+        if env_vars is not Sentinel.NO_UPDATE:
+            new_env_vars = env_vars
+        else:
+            new_env_vars = invocation.env_vars
+
         new_invocation = TaskInvocation(
             task=invocation.task,
             args=invocation.args,
             kwargs=invocation.kwargs,
             resources=new_resources,
             custom_name=invocation.custom_name,
             custom_image=new_custom_image,
+            env_vars=new_env_vars,
         )
 
         return ArtifactFuture(
             invocation=new_invocation,
             output_index=self.output_index,
             custom_name=self.custom_name,
             serialization_format=self.serialization_format,
@@ -899,24 +918,24 @@
     # The fully-qualified type hint is a workaround for docs' autoapi not being able to
     # resolve symbols.
 
     def with_resources(
         self,
         *,
         cpu: Optional[
-            Union[str, "orquestra.sdk._base._dsl.Sentinel"]
+            Union[str, "orquestra.sdk._client._base._dsl.Sentinel"]  # pyright: ignore
         ] = Sentinel.NO_UPDATE,
         memory: Optional[
-            Union[str, "orquestra.sdk._base._dsl.Sentinel"]
+            Union[str, "orquestra.sdk._client._base._dsl.Sentinel"]  # pyright: ignore
         ] = Sentinel.NO_UPDATE,
         disk: Optional[
-            Union[str, "orquestra.sdk._base._dsl.Sentinel"]
+            Union[str, "orquestra.sdk._client._base._dsl.Sentinel"]  # pyright: ignore
         ] = Sentinel.NO_UPDATE,
         gpu: Optional[
-            Union[str, "orquestra.sdk._base._dsl.Sentinel"]
+            Union[str, "orquestra.sdk._client._base._dsl.Sentinel"]  # pyright: ignore
         ] = Sentinel.NO_UPDATE,
     ) -> "ArtifactFuture":
         """
         Assigns optional metadata related to task invocation used to generate this
         artifact.
 
         Doesn't modify existing invocations, returns a new one.
@@ -940,15 +959,15 @@
 
     # The fully-qualified type hint is a workaround for docs' autoapi not being able to
     # resolve symbols.
 
     def with_custom_image(
         self,
         custom_image: Optional[
-            Union[str, "orquestra.sdk._base._dsl.Sentinel"]
+            Union[str, "orquestra.sdk._client._base._dsl.Sentinel"]  # pyright: ignore
         ] = Sentinel.NO_UPDATE,
     ) -> "ArtifactFuture":
         """
         Assigns optional metadata related to task invocation used to generate this
         artifact.
 
         Doesn't modify existing invocations, returns a new one.
@@ -965,14 +984,49 @@
         self._check_if_destructured(
             fn_name=self.invocation.task._fn_name,
             assign_type="custom image",
         )
 
         return self.with_invocation_meta(custom_image=custom_image)
 
+    def with_env_variables(
+        self,
+        env_vars: Optional[
+            Union[
+                Dict[str, str],
+                "orquestra.sdk._client._base._dsl.Sentinel",  # pyright: ignore
+            ]  # pyright: ignore
+        ] = Sentinel.NO_UPDATE,
+    ) -> "ArtifactFuture":
+        """
+        Assigns optional metadata related to task invocation used to generate this
+        artifact.
+
+        Doesn't modify existing invocations, returns a new one.
+
+        Env vars passed to that function are directly passed to Ray runtime_env object.
+        This function overwrites env_vars set by the `env_vars` parameter in the task,
+        it does not append them.
+
+        Example usage::
+
+            text = capitalize("hello").with_env_variables(
+                {"MY_VAR_NAME": "MY_VAR_VALUE"}
+            )
+
+        Args:
+            env_vars: dict of all env variables to be set before task starts executing
+        """  # noqa: D205, D212
+        self._check_if_destructured(
+            fn_name=self.invocation.task._fn_name,
+            assign_type="env_vars",
+        )
+
+        return self.with_invocation_meta(env_vars=env_vars)
+
     def _check_if_destructured(self, fn_name: str, assign_type: str):
         """Check if an ArtifactFuture has been destructured.
 
         The fn_name and assign_type are used to construct an informative error message
         if the ArtifactFuture is destructured.
 
         Args:
@@ -1078,58 +1132,63 @@
             "Complex function detected, falling back to a single output. "
             f"Hypotheses: {visitor.outputs}"
         )
         return TaskOutputMetadata(is_subscriptable=False, n_outputs=1)
 
 
 @overload
-def task(fn: Callable[_P, _R]) -> TaskDef[_P, _R]:
+def task(fn: Callable[..., _TaskReturn]) -> TaskDef[_TaskReturn]:
     ...
 
 
 @overload
 def task(
     *,
     source_import: Optional[Import] = None,
     dependency_imports: Union[Iterable[Import], Import, None] = None,
     resources: Resources = Resources(),
     n_outputs: Optional[int] = None,
     custom_image: Optional[str] = None,
     custom_name: Optional[str] = None,
     max_retries: Optional[int] = None,
-) -> Callable[[Callable[_P, _R]], TaskDef[_P, _R]]:
+    env_vars: Optional[Dict[str, str]] = None,
+) -> Callable[[Callable[..., _TaskReturn]], TaskDef[_TaskReturn]]:
     ...
 
 
 @overload
 def task(
-    fn: Callable[_P, _R],
+    fn: Callable[..., _TaskReturn],
     *,
     source_import: Optional[Import] = None,
     dependency_imports: Union[Iterable[Import], Import, None] = None,
     resources: Resources = Resources(),
     n_outputs: Optional[int] = None,
     custom_image: Optional[str] = None,
     custom_name: Optional[str] = None,
     max_retries: Optional[int] = None,
-) -> TaskDef[_P, _R]:
+    env_vars: Optional[Dict[str, str]] = None,
+) -> TaskDef[_TaskReturn]:
     ...
 
 
 def task(
-    fn: Optional[Callable[_P, _R]] = None,
+    fn: Optional[Callable[..., _TaskReturn]] = None,
     *,
     source_import: Optional[Import] = None,
     dependency_imports: Union[Iterable[Import], Import, None] = None,
     resources: Resources = Resources(),
     n_outputs: Optional[int] = None,
     custom_image: Optional[str] = None,
     custom_name: Optional[str] = None,
     max_retries: Optional[int] = None,
-) -> Union[TaskDef[_P, _R], Callable[[Callable[_P, _R]], TaskDef[_P, _R]]]:
+    env_vars: Optional[Dict[str, str]] = None,
+) -> Union[
+    TaskDef[_TaskReturn], Callable[[Callable[..., _TaskReturn]], TaskDef[_TaskReturn]]
+]:
     """Wraps a function into an Orquestra Task.
 
     The result is something you can use inside your `@sdk.workflow` function. If you
     need to call the task's underlying function directly, see
     ``orquestra.sdk.packaging.execute_task()``.
 
     Args:
@@ -1158,15 +1217,16 @@
             Also only first 128 characters of the name will be used
         max_retries: Maximum number of times a worker will try to retry after failure.
             Useful if worker is killed by random events, or memory leaks from previously
             executed tasks.
             WARNING: retried workers might cause issues in MLflow logging, as retried
             workers share the same invocation ID, MLflow identifier will be shared
             between them.
-
+        env_vars: environmental variables that will be set on a worker before
+            the task is scheduled
     Raises:
         ValueError: when a task has fewer than 1 outputs.
     """
     task_dependency_imports: Optional[Tuple[Import, ...]]
 
     if dependency_imports is None:
         task_dependency_imports = None
@@ -1175,15 +1235,15 @@
     elif dependency_imports is not None:
         task_dependency_imports = tuple(dependency_imports)
 
     if n_outputs is not None:
         if n_outputs <= 0:
             raise ValueError("A task should have at least one output")
 
-    def _inner(fn: Callable[_P, _R]):
+    def _inner(fn: Callable):
         # Assume if a user has specified the number of outputs, then this output is
         # subscriptable
         output_metadata: TaskOutputMetadata
         if n_outputs is not None:
             output_metadata = TaskOutputMetadata(
                 is_subscriptable=True, n_outputs=n_outputs
             )
@@ -1196,15 +1256,73 @@
             dependency_imports=task_dependency_imports,
             resources=resources,
             parameters=_get_parameters(fn),
             output_metadata=output_metadata,
             custom_image=custom_image,
             custom_name=custom_name,
             max_retries=max_retries,
+            env_vars=env_vars,
         )
 
         return task_def
 
     if fn is None:
         return _inner
     else:
         return _inner(fn)
+
+
+def InstalledImport(
+    *,
+    package_name: str,
+    version_match: Optional[str] = None,
+    fallback: Optional[Import] = None,
+) -> Import:
+    """Returns PythonImports for a task for the installed version of a package.
+
+    On an error, if a fallback is provided, the fallback is returned instead.
+
+    Args:
+        package_name: the package to use as the import.
+        version_match: a regex string to match the installed version.
+        fallback: a fallback import to return if there are any issues
+            in finding the package version.
+
+    Raises:
+        PackagingError: If there are any issues finding an installed package and no
+            fallback is provided.
+
+    Returns:
+        Either a PythonImports for package_name at the installed version or `fallback`.
+
+    """
+    try:
+        version = get_installed_version(package_name)
+        if version_match is not None:
+            if re.match(version_match, version) is None:
+                raise PackagingError(
+                    f"Package version mismatch: "
+                    f"{package_name}=={version}\n"
+                    f'Expected version to match "{version_match}"'
+                )
+    except PackagingError as e:
+        if fallback is not None:
+            return fallback
+        raise e
+
+    return PythonImports(f"{package_name}=={version}")
+
+
+def execute_task(task: TaskDef, args: tuple, kwargs: dict):
+    """A helper method to testing tasks by executing them outside of the workflow graph.
+
+    Use only for unittesting code.
+
+    Args:
+        task: the task you want to execute.
+        args: the positional arguments to pass to the task.
+        kwargs: the keyword arguments to pass to the task.
+
+    Returns:
+        the result of executing a task.
+    """
+    return task._TaskDef__sdk_task_body(*args, **kwargs)
```

## Comparing `orquestra/sdk/_base/_env.py` & `orquestra/sdk/_client/_base/_env.py`

 * *Files 22% similar despite different names*

```diff
@@ -48,62 +48,14 @@
 
 ORQ_VERBOSE = "ORQ_VERBOSE"
 """
 If set to a truthy value, enables printing debug information when running the ``orq``
 CLI commands.
 """
 
-ORQ_TASK_RUN_LOGS_DIR = "ORQ_TASK_RUN_LOGS_DIR"
-"""
-Used to set the storage location for task logs
-"""
-
-# --------------------------------- Ray --------------------------------------
-
-RAY_TEMP_PATH_ENV = "ORQ_RAY_TEMP_PATH"
-"""
-Used to configure the location of Ray's temp storage
-Example:
-    ORQ_RAY_TEMP_PATH=/tmp/ray/temp
-"""
-
-RAY_STORAGE_PATH_ENV = "ORQ_RAY_STORAGE_PATH"
-"""
-Used to configure the location of Ray's persistent storage
-Example:
-    ORQ_RAY_STORAGE_PATH=/tmp/ray/storage
-"""
-
-RAY_PLASMA_PATH_ENV = "ORQ_RAY_PLASMA_PATH"
-"""
-Used to configure the location of Ray's plasma storage
-Example:
-    ORQ_RAY_PLASMA_PATH=/tmp/ray/plasma
-"""
-
-RAY_DOWNLOAD_GIT_IMPORTS_ENV = "ORQ_RAY_DOWNLOAD_GIT_IMPORTS"
-"""
-Used to configure if Ray downloads Git imports
-Example:
-    ORQ_RAY_DOWNLOAD_GIT_IMPORTS=1
-"""
-
-RAY_GLOBAL_WF_RUN_ID_ENV = "GLOBAL_WF_RUN_ID"
-"""
-Used to set the workflow run ID in a Ray workflow
-"""
-
-RAY_SET_CUSTOM_IMAGE_RESOURCES_ENV = "ORQ_RAY_SET_CUSTOM_IMAGE_RESOURCES"
-"""
-Used to configure if Ray uses custom images
-Example:
-    ORQ_RAY_SET_CUSTOM_IMAGE_RESOURCES=1
-"""
-
-
 # --------------------------------- MLFlow -----------------------------------
 
 MLFLOW_CR_NAME = "ORQ_MLFLOW_CR_NAME"
 """
 Used to set the MLFlow CR name.
 """
```

## Comparing `orquestra/sdk/_base/_exec_ctx.py` & `orquestra/sdk/_shared/exec_ctx/_exec_ctx.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/_base/_factory.py` & `orquestra/sdk/_client/_base/_factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 
-from orquestra.sdk import exceptions
-from orquestra.sdk._base.abc import RuntimeInterface
-from orquestra.sdk.schema.configs import RuntimeConfiguration, RuntimeName
+from orquestra.sdk._shared import exceptions
+from orquestra.sdk._shared.abc import RuntimeInterface
+from orquestra.sdk._shared.schema.configs import RuntimeConfiguration, RuntimeName
 
 
 def build_runtime_from_config(
     config: RuntimeConfiguration, verbose: bool = False
 ) -> RuntimeInterface:
     """Centralized place to get runtime object based on config.
 
@@ -16,53 +16,55 @@
     classes. This factory function solves the problem of figuring out which
     class to use.
     """
     # Imports are deferred to cut down on the import graph for CLI latency. The
     # subgraphs for Ray and for CE are distinct, and both take a lot of time to
     # import.
     if config.runtime_name == RuntimeName.RAY_LOCAL:
-        import orquestra.sdk._ray._dag
+        import orquestra.sdk._runtime._ray._dag
 
-        return orquestra.sdk._ray._dag.RayRuntime(
+        return orquestra.sdk._runtime._ray._dag.RayRuntime(
             config=config,
         )
     elif config.runtime_name == RuntimeName.IN_PROCESS:
-        import orquestra.sdk._base._in_process_runtime
+        import orquestra.sdk._client._base._in_process_runtime
 
-        return orquestra.sdk._base._in_process_runtime.InProcessRuntime()
+        return orquestra.sdk._client._base._in_process_runtime.InProcessRuntime()
     elif config.runtime_name == RuntimeName.CE_REMOTE:
         return _build_ce_runtime(config, verbose)
     elif config.runtime_name == RuntimeName.QE_REMOTE:
         raise exceptions.QERemoved(
             "QE support has been removed. "
             f"Use CE by logging in again with `orq login -c {config.config_name}`"
         )
     else:
         raise exceptions.NotFoundError(f"Unknown runtime: {config.runtime_name}")
 
 
 def _build_ce_runtime(config: RuntimeConfiguration, verbose: bool):
-    import orquestra.sdk._base._driver._ce_runtime
-    import orquestra.sdk._base._driver._client
+    import orquestra.sdk._client._base._driver._ce_runtime
+    import orquestra.sdk._client._base._driver._client
 
     # We're using a reusable session to allow shared headers
     # In the future we can store cookies, etc too.
 
     try:
         base_uri = config.runtime_options["uri"]
         token = config.runtime_options["token"]
     except KeyError as e:
         raise exceptions.RuntimeConfigError(
             "Invalid CE configuration. Did you login first?"
         ) from e
 
-    uri_provider = orquestra.sdk._base._driver._client.ExternalUriProvider(base_uri)
+    uri_provider = orquestra.sdk._client._base._driver._client.ExternalUriProvider(
+        base_uri
+    )
 
-    client = orquestra.sdk._base._driver._client.DriverClient.from_token(
+    client = orquestra.sdk._client._base._driver._client.DriverClient.from_token(
         token=token, uri_provider=uri_provider
     )
 
-    return orquestra.sdk._base._driver._ce_runtime.CERuntime(
+    return orquestra.sdk._client._base._driver._ce_runtime.CERuntime(
         config=config,
         client=client,
         verbose=verbose,
     )
```

## Comparing `orquestra/sdk/_base/_git_url_utils.py` & `orquestra/sdk/_client/_base/_git_url_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,77 +4,29 @@
 
 import re
 from typing import Optional
 
 from urllib3.exceptions import LocationParseError
 from urllib3.util import parse_url
 
-from .. import secrets
-from ..schema.ir import GitURL
+from orquestra.sdk._shared.schema.ir import GitURL
 
 
 def _split_auth(auth_value: Optional[str]):
     if auth_value is None:
         return None, None
 
     split_auth = auth_value.split(":")
 
     if len(split_auth) == 1:
         return split_auth[0], None
     else:
         return split_auth[0], ":".join(split_auth[1:])
 
 
-def build_git_url(url: GitURL, protocol_override: Optional[str] = None) -> str:
-    """Returns a usable string from a GitURL.
-
-    This will get the password from the secrets API, if required.
-
-    Args:
-        url: the GitURL to build the URL string from
-        protocol_override: Ignore the protocol defined in the URL and build the URL
-            using a different protocol.
-
-    Raises:
-        ValueError: when the protocol is not recognised.
-    """
-    protocol = protocol_override or url.protocol
-    user = url.user or "git"
-    port = f":{url.port}" if url.port is not None else ""
-
-    # Dereference secret used as password
-    if url.password is not None:
-        secret = secrets.get(
-            url.password.secret_name,
-            config_name=url.password.secret_config,
-            workspace_id=url.password.workspace_id,
-        )
-        password = f":{secret}"
-    else:
-        password = ""
-
-    if protocol == "ssh":
-        if url.port is None:
-            return f"{user}@{url.host}:{url.path}"
-        else:
-            return f"ssh://{user}{password}@{url.host}{port}/{url.path}"
-    elif protocol in ("git+ssh", "ssh+git", "ftp", "ftps"):
-        return f"{protocol}://{user}{password}@{url.host}{port}/{url.path}"
-    elif protocol in ("http", "https", "git+https", "git+http"):
-        if url.user is None and url.password is None:
-            return f"{protocol}://{url.host}{port}/{url.path}"
-        else:
-            return f"{protocol}://{user}{password}@{url.host}{port}/{url.path}"
-    else:
-        if protocol == url.protocol:
-            return url.original_url
-        else:
-            raise ValueError(f"Unknown protocol: `{protocol}`")
-
-
 def parse_git_url(url: str) -> GitURL:
     """Parse a git URL from a string.
 
     Accepted formats:
 
     * ``<protocol>://[<user>@]<host>[:<port>]/<path>[?<query>]``
     * ``<user>@<host>:<path>``
```

## Comparing `orquestra/sdk/_base/_graphs.py` & `orquestra/sdk/_shared/_graphs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 import typing as t
 from copy import copy
 
-from orquestra.sdk.schema import ir
+from .schema import ir
 
 Node = str
 
 # Graph uses dict with Nones instead of set because dict is ordered, and set is not
 # and we need the order to be deterministic
 Graph = t.Dict[Node, t.Dict[Node, None]]
```

## Comparing `orquestra/sdk/_base/_in_process_runtime.py` & `orquestra/sdk/_client/_base/_in_process_runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,35 +4,38 @@
 """In-process implementation of the runtime interface."""
 
 import typing as t
 import warnings
 from contextlib import contextmanager
 from datetime import timedelta
 
-from orquestra.sdk import exceptions
-from orquestra.sdk._base import _dates, abc
-from orquestra.sdk._base._spaces._structs import ProjectRef
-from orquestra.sdk.schema import ir
-from orquestra.sdk.schema.responses import WorkflowResult
-from orquestra.sdk.schema.workflow_run import (
+from orquestra.sdk import secrets
+from orquestra.sdk._shared import (
+    ProjectRef,
+    abc,
+    exceptions,
+    iter_invocations_topologically,
+    serde,
+)
+from orquestra.sdk._shared.dates import Instant
+from orquestra.sdk._shared.dates import now as dates_now
+from orquestra.sdk._shared.dispatch import locate_fn_ref
+from orquestra.sdk._shared.schema import ir
+from orquestra.sdk._shared.schema.responses import WorkflowResult
+from orquestra.sdk._shared.schema.workflow_run import (
     RunStatus,
     State,
     TaskRun,
     TaskRunId,
     WorkflowRun,
     WorkflowRunId,
     WorkflowRunSummary,
     WorkspaceId,
 )
 
-from .. import secrets
-from . import serde
-from ._graphs import iter_invocations_topologically
-from .dispatch import locate_fn_ref
-
 WfRunId = str
 ArtifactValue = t.Any
 TaskOutputs = t.Tuple[ArtifactValue, ...]
 
 global_current_run_ids: t.Optional[
     t.Tuple[WorkflowRunId, ir.TaskInvocationId, TaskRunId]
 ] = None
@@ -114,16 +117,16 @@
 
     def __init__(self):
         self._output_store: t.Dict[WfRunId, TaskOutputs] = {}
         self._artifact_store: t.Dict[
             WfRunId, t.Dict[ir.ArtifactNodeId, ArtifactValue]
         ] = {}
         self._workflow_def_store: t.Dict[WfRunId, ir.WorkflowDef] = {}
-        self._start_time_store: t.Dict[WfRunId, _dates.Instant] = {}
-        self._end_time_store: t.Dict[WfRunId, _dates.Instant] = {}
+        self._start_time_store: t.Dict[WfRunId, Instant] = {}
+        self._end_time_store: t.Dict[WfRunId, Instant] = {}
 
     def _gen_next_run_id(self, wf_def: ir.WorkflowDef):
         return f"{wf_def.name}-{len(self._output_store) + 1}"
 
     def create_workflow_run(
         self,
         workflow_def: ir.WorkflowDef,
@@ -141,15 +144,15 @@
             warnings.warn(
                 "InProcessRuntime doesn't support `dry_run`."
                 " A Regular task code will be executed.",
                 category=exceptions.UnsupportedRuntimeFeature,
             )
         run_id = self._gen_next_run_id(workflow_def)
 
-        self._start_time_store[run_id] = _dates.now()
+        self._start_time_store[run_id] = dates_now()
 
         # We deserialize the constants in one go, instead of as needed
         consts: t.Dict[ir.ConstantNodeId, t.Any] = {
             id: serde.deserialize(node)
             for id, node in workflow_def.constant_nodes.items()
         }
         for id, secret in workflow_def.secret_nodes.items():
@@ -192,15 +195,15 @@
 
         # Ordinary functions return `obj` or `tuple(obj, obj)`
         outputs = tuple(
             _get_args(consts, self._artifact_store[run_id], workflow_def.output_ids)
         )
         self._output_store[run_id] = outputs
 
-        self._end_time_store[run_id] = _dates.now()
+        self._end_time_store[run_id] = dates_now()
         self._workflow_def_store[run_id] = workflow_def
         return run_id
 
     def get_workflow_run_outputs_non_blocking(
         self, workflow_run_id: WfRunId
     ) -> t.Tuple[WorkflowResult, ...]:
         return (
@@ -301,15 +304,15 @@
             state: Only return runs of runs with the specified status.
             workspace: Only return runs from the specified workspace. Not supported
                 on this runtime.
 
         Returns:
                 A list of the workflow runs
         """
-        now = _dates.now()
+        now = dates_now()
 
         if state is not None:
             if not isinstance(state, list):
                 state_list = [state]
             else:
                 state_list = state
         else:
```

## Comparing `orquestra/sdk/_base/_jwt.py` & `orquestra/sdk/_client/_base/_jwt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ################################################################################
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 import jwt
 
-from ..exceptions import ExpiredTokenError, InvalidTokenError
+from orquestra.sdk._shared.exceptions import ExpiredTokenError, InvalidTokenError
 
 
 def check_jwt_without_signature_verification(token: str):
     """Checks a token and ensures it is a JWT and it is not expired.
 
     Note: This DOES NOT CRYPTOGRAPHICALY VERIFY THE TOKEN.
     Only used as a sanity check when reading a token from the CLI.
```

## Comparing `orquestra/sdk/_base/_regex.py` & `orquestra/sdk/_shared/_regex.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/_base/_retry.py` & `orquestra/sdk/_client/_base/_retry.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/_base/_traversal.py` & `orquestra/sdk/_client/_base/_traversal.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,23 @@
 import typing as t
 import warnings
 from collections import OrderedDict
 from functools import singledispatch
 
 from pip_api._parse_requirements import Requirement
 
-from orquestra.sdk.schema import ir, responses
+from orquestra.sdk._shared import exceptions, serde
+from orquestra.sdk._shared.exec_ctx import workflow_build
+from orquestra.sdk._shared.packaging import (
+    get_current_python_version,
+    get_current_sdk_version,
+)
+from orquestra.sdk._shared.schema import ir, responses
 
-from .. import exceptions
-from ..packaging._versions import get_current_python_version, get_current_sdk_version
-from . import _dsl, _exec_ctx, _git_url_utils, _workflow, serde
+from . import _dsl, _git_url_utils, _workflow
 
 N_BYTES_IN_HASH = 8
 
 
 def _make_key(obj: t.Any):
     """Returns a hashable key for all types.
 
@@ -332,15 +336,15 @@
             for arg in [*invocation.args, *[arg for _, arg in invocation.kwargs]]:
                 if _make_key(arg) not in traversed_nodes:
                     traversal_list.append(arg)
         yield current_node
 
 
 @singledispatch
-def _make_import_id(imp: _dsl.Import, import_hash: str):
+def _make_import_id(imp: _dsl.Import, import_hash: str) -> str:
     raise TypeError(f"Unknown import: {type(imp)}")
 
 
 @_make_import_id.register
 def _(imp: _dsl.LocalImport, import_hash: str):
     return f"local-{import_hash}"
 
@@ -348,15 +352,15 @@
 @_make_import_id.register(_dsl.GitImport)
 @_make_import_id.register(_dsl.GitImportWithAuth)
 def _(imp: t.Union[_dsl.GitImport, _dsl.GitImportWithAuth], import_hash: str):
     # Remove git@, https://, and .git from repo_url
     proj_name = re.sub("https://|.git|git@", "", imp.repo_url)
     # Replace all non-alphanumeric characters with an underscore.
     # multiple special characters are grouped together with a single underscore
-    # For example: github_com_zapatacomputing_orquestra_sdk
+    # For example: github_com_zapata_engineering_orquestra_sdk
     proj_name = re.sub("[^A-Za-z0-9]+", "_", proj_name)
     return f"git-{import_hash}_{proj_name}"
 
 
 @_make_import_id.register
 def _(imp: _dsl.PythonImports, import_hash: str):
     # Imports might be too long to include in the ID
@@ -746,20 +750,21 @@
         ),
         task_id=task_models_dict[invocation.task].id,
         args_ids=args_ids,
         kwargs_ids=kwargs_ids,
         output_ids=graph.output_ids_for_invocation(invocation),
         resources=_make_resources_model(invocation.resources),
         custom_image=invocation.custom_image,
+        env_vars=invocation.env_vars,
     )
 
 
 def extract_root_futures(wf_def: _workflow.WorkflowDef) -> t.Sequence[_dsl.Argument]:
     """Executes the ``wf_def`` function to get the workflow output futures."""
-    with _exec_ctx.workflow_build():
+    with workflow_build():
         futures = wf_def._fn(*wf_def._workflow_args, **wf_def._workflow_kwargs)
 
     if not isinstance(futures, collections.abc.Sequence) or isinstance(futures, str):
         return (futures,)
     else:
         return futures
```

## Comparing `orquestra/sdk/_base/_viz.py` & `orquestra/sdk/_client/_base/_viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import itertools
 import typing as t
 from dataclasses import dataclass
 
 import graphviz  # type: ignore
 
-from orquestra.sdk.schema import ir
+from orquestra.sdk._shared.schema import ir
 
 NodeId = str
 
 
 @dataclass(frozen=True)
 class Node:
     id: NodeId
```

## Comparing `orquestra/sdk/_base/_workflow.py` & `orquestra/sdk/_client/_base/_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     TypeVar,
     Union,
     overload,
 )
 
 from typing_extensions import ParamSpec
 
-import orquestra.sdk.schema.ir as ir
-from orquestra.sdk import exceptions
-from orquestra.sdk.exceptions import WorkflowSyntaxError
-from orquestra.sdk.schema.workflow_run import ProjectId, WorkspaceId
+import orquestra.sdk._shared.schema.ir as ir
+from orquestra.sdk import secrets
+from orquestra.sdk._shared import exceptions
+from orquestra.sdk._shared.exceptions import WorkflowSyntaxError
+from orquestra.sdk._shared.schema.workflow_run import ProjectId, WorkspaceId
 
-from .. import secrets
 from . import _api, _dsl, loader
 from ._ast import CallVisitor, NodeReference, NodeReferenceType, normalize_indents
 from ._dsl import (
     DataAggregation,
     FunctionRef,
     Import,
     ImportTypes,
@@ -110,15 +110,15 @@
                 this workflow def has a "GitImport" and the git repo that contains it
                 has uncommitted changes.
             orquestra.sdk.exceptions.WorkflowSyntaxError: when there are no tasks
                 defined for this workflow.
             orquestra.sdk.exceptions.InvalidTaskDefinitionError: when there is invalid
                 task used inside this workflow
         """
-        from orquestra.sdk._base import _traversal
+        from orquestra.sdk._client._base import _traversal
 
         futures = _traversal.extract_root_futures(self)
         model = _traversal.flatten_graph(self, futures)
 
         if len(model.task_invocations) < 1:
             helpstr = f"The workflow '{model.name}' "
             if not isinstance(model.fn_ref, ir.InlineFunctionRef):
@@ -140,17 +140,17 @@
         Jupyter renders it natively.
 
         Note: rendering an image of the result graph requires a system-wide installation
         of graphviz. For installation instructions see:
         https://graphviz.readthedocs.io/en/stable/manual.html#installation
         """
         # Defer import to avoid 120ms latency toll for everything.
-        import orquestra.sdk._base._viz
+        import orquestra.sdk._client._base._viz
 
-        return orquestra.sdk._base._viz.wf_def_to_graphviz(self.model)
+        return orquestra.sdk._client._base._viz.wf_def_to_graphviz(self.model)
 
     def run(
         self,
         config: Union[_api.RuntimeConfig, str],
         project_dir: Optional[Union[str, Path]] = None,
         workspace_id: Optional[WorkspaceId] = None,
         project_id: Optional[ProjectId] = None,
@@ -239,14 +239,16 @@
             name=self._name,
             workflow_fn=self._fn,
             fn_ref=self._fn_ref,
             resources=new_resources,
             data_aggregation=self._data_aggregation,
             workflow_args=self._workflow_args,
             workflow_kwargs=self._workflow_kwargs,
+            default_source_import=self.default_source_import,
+            default_dependency_imports=self.default_dependency_imports,
         )
 
 
 class WorkflowTemplate(Generic[_P, _R]):
     """Result of applying the `@workflow` decorator to a function."""
 
     def __init__(
@@ -543,14 +545,28 @@
     custom_name: Optional[str] = None,
     default_source_import: Optional[Import] = None,
     default_dependency_imports: Optional[Iterable[Import]] = None,
 ) -> Callable[[Callable[_P, _R]], WorkflowTemplate[_P, _R]]:
     ...
 
 
+@overload
+def workflow(
+    fn: Callable[_P, _R],
+    *,
+    resources: Optional[_dsl.Resources] = None,
+    head_node_resources: Optional[_dsl.Resources] = None,
+    data_aggregation: Optional[Union[DataAggregation, bool]] = None,
+    custom_name: Optional[str] = None,
+    default_source_import: Optional[Import] = None,
+    default_dependency_imports: Optional[Iterable[Import]] = None,
+) -> WorkflowTemplate[_P, _R]:
+    ...
+
+
 def workflow(
     fn: Optional[Callable[_P, _R]] = None,
     *,
     resources: Optional[_dsl.Resources] = None,
     head_node_resources: Optional[_dsl.Resources] = None,
     data_aggregation: Optional[Union[DataAggregation, bool]] = None,
     custom_name: Optional[str] = None,
```

## Comparing `orquestra/sdk/_base/abc.py` & `orquestra/sdk/_shared/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 This module shouldn't contain any implementation, only interface definitions.
 """
 
 import typing as t
 from abc import ABC, abstractmethod
 from datetime import timedelta
 
-from ..exceptions import WorkspacesNotSupportedError
-from ..schema.ir import TaskInvocationId, WorkflowDef
-from ..schema.responses import WorkflowResult
-from ..schema.workflow_run import (
+from orquestra.sdk._shared.exceptions import WorkspacesNotSupportedError
+
+from ._spaces import Project, ProjectRef, Workspace
+from .logs import LogOutput, LogReader, WorkflowLogs
+from .schema.ir import TaskInvocationId, WorkflowDef
+from .schema.responses import WorkflowResult
+from .schema.workflow_run import (
     State,
     WorkflowRun,
     WorkflowRunId,
     WorkflowRunMinimal,
     WorkflowRunSummary,
     WorkspaceId,
 )
-from ._logs._interfaces import LogOutput, LogReader, WorkflowLogs
-from ._spaces._structs import Project, ProjectRef, Workspace
 
 # A typealias that hints where we expect raw artifact values.
 ArtifactValue = t.Any
 
 
 class RuntimeInterface(ABC, LogReader):
     """The main abstraction for managing Orquestra workflows.
```

## Comparing `orquestra/sdk/_base/dispatch.py` & `orquestra/sdk/_shared/dispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import importlib
 import importlib.util
 import os
 import sys
 import typing as t
 from functools import singledispatch
 
-from orquestra.sdk._base import serde
-from orquestra.sdk.schema import ir
+from ..schema import ir
+from . import serde
 
 
 def _locate_callable(fn_ref_dict) -> t.Callable:
     fn_ref: ir.FunctionRef
     if fn_ref_dict["type"] == "MODULE_FUNCTION_REF":
         fn_ref = ir.ModuleFunctionRef.model_validate(fn_ref_dict)
         return locate_fn_ref(fn_ref)
```

## Comparing `orquestra/sdk/_base/loader.py` & `orquestra/sdk/_client/_base/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import importlib
 import importlib.machinery
 import sys
 import types
 import typing as t
 from importlib import abc
 
-from . import dispatch
+from orquestra.sdk._shared import dispatch
 
 
 class FakeImportedAttribute:
     MSG = "This object has been faked by the import loader"
 
     def __getitem__(self, _):
         raise RuntimeError(self.MSG)
```

## Comparing `orquestra/sdk/_base/serde.py` & `orquestra/sdk/_shared/serde.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 from contextlib import contextmanager
 from dataclasses import dataclass
 from functools import singledispatch
 from pathlib import Path
 
 import cloudpickle  # type: ignore
 
-from orquestra.sdk.schema import ir, responses
-
-from .._base._storage import TypeAdapter
+from .orqdantic import TypeAdapter
+from .schema import ir, responses
 
 CHUNK_SIZE = 40_000
 ENCODING = "base64"
 PICKLE_PROTOCOL = 4
 
 
 class _JSONTupleEncoder(json.JSONEncoder):
```

## Comparing `orquestra/sdk/_base/_api/_config.py` & `orquestra/sdk/_client/_base/_api/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 import json
 import logging
 import typing as t
 import warnings
 
 from packaging.version import parse as parse_version
 
-from orquestra.sdk._base._factory import build_runtime_from_config
-
-from ...exceptions import ConfigFileNotFoundError, ConfigNameNotFoundError
-from ...schema.configs import (
+from orquestra.sdk._shared.abc import RuntimeInterface
+from orquestra.sdk._shared.exceptions import (
+    ConfigFileNotFoundError,
+    ConfigNameNotFoundError,
+)
+from orquestra.sdk._shared.schema.configs import (
     CONFIG_FILE_CURRENT_VERSION,
     ConfigName,
     RuntimeConfiguration,
     RuntimeName,
 )
+
 from .. import _config
-from ..abc import RuntimeInterface
+from .._factory import build_runtime_from_config
 
 
 class RuntimeConfig:
     """Encompasses the configuration with which a workflow can be run.
 
     Intended to be used with the WorkflowDef class to create a run with the desired
     configuration.
```

## Comparing `orquestra/sdk/_base/_api/_task_run.py` & `orquestra/sdk/_client/_base/_api/_task_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 
 import typing as t
 from collections import namedtuple
 from itertools import chain
 
-from orquestra.sdk._base import serde
-from orquestra.sdk._base._logs._interfaces import LogOutput
-from orquestra.sdk.schema import ir
-from orquestra.sdk.schema.responses import WorkflowResult
-from orquestra.sdk.schema.workflow_run import State, TaskInvocationId
-from orquestra.sdk.schema.workflow_run import TaskRun as TaskRunModel
-from orquestra.sdk.schema.workflow_run import TaskRunId, WorkflowRunId
-
-from ..._base import _exec_ctx
-from ...exceptions import TaskRunNotFound, WorkflowRunIDNotFoundError
-from ..abc import ArtifactValue, RuntimeInterface
-from ..serde import deserialize_constant
+from orquestra.sdk._shared import serde
+from orquestra.sdk._shared.abc import ArtifactValue, RuntimeInterface
+from orquestra.sdk._shared.exceptions import TaskRunNotFound, WorkflowRunIDNotFoundError
+from orquestra.sdk._shared.exec_ctx import ExecContext, get_current_exec_context
+from orquestra.sdk._shared.logs import LogOutput
+from orquestra.sdk._shared.schema import ir
+from orquestra.sdk._shared.schema.responses import WorkflowResult
+from orquestra.sdk._shared.schema.workflow_run import State, TaskInvocationId
+from orquestra.sdk._shared.schema.workflow_run import TaskRun as TaskRunModel
+from orquestra.sdk._shared.schema.workflow_run import TaskRunId, WorkflowRunId
+from orquestra.sdk._shared.serde import deserialize_constant
 
 
 class TaskRun:
     """Represents execution of a single task."""
 
     class _InputUnavailable:
         def __str__(self):
@@ -265,21 +264,21 @@
         ModuleNotFoundError: when Ray isn't installed.
         WorkflowRunIDNotFoundError: When the workflow run ID can't be recovered.
 
     Returns:
         The IDs associated with the current run, in a named tuple. See: CurrentRunIDs
     """
     # Deferred import in case Ray isn't installed
-    import orquestra.sdk._ray._build_workflow
+    import orquestra.sdk._runtime._ray._build_workflow
 
     (
         wf_run_id,
         task_inv_id,
         task_run_id,
-    ) = orquestra.sdk._ray._build_workflow.get_current_ids()
+    ) = orquestra.sdk._runtime._ray._build_workflow.get_current_ids()
 
     if wf_run_id is None:
         raise WorkflowRunIDNotFoundError("Could not recover Workflow Run ID")
 
     return CurrentRunIDs(wf_run_id, task_inv_id, task_run_id)
 
 
@@ -332,17 +331,17 @@
         The workflow run, task invocation, and task run IDs associated with the current
             run, in a named tuple. See: CurrentRunIDs
 
     Raises:
         WorkflowRunIDNotFoundError: When the workflow run ID cannot be recovered.
         NotImplementedError: When the execution context is not one of the covered cases.
     """
-    context = _exec_ctx.get_current_exec_context()
+    context = get_current_exec_context()
 
-    if context == _exec_ctx.ExecContext.RAY:
+    if context == ExecContext.RAY:
         return _get_ray_backend_ids()
-    elif context == _exec_ctx.ExecContext.DIRECT:
+    elif context == ExecContext.DIRECT:
         return _get_in_process_backend_ids()
 
     raise NotImplementedError(
         f"Got unexpected global context {context}. Please report this as a bug."
     )
```

## Comparing `orquestra/sdk/_base/_api/_wf_run.py` & `orquestra/sdk/_client/_base/_api/_wf_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 ################################################################################
 
 """User-facing ``WorkflowRun`` object.
 
 WorkflowRun represents, and allows interaction with, an individual workflow run.
 """
 
+import os
 import re
 import sys
 import time
 import typing as t
 import warnings
 from datetime import timedelta
 from functools import cached_property
 from pathlib import Path
+from urllib.parse import urlparse
 
-from ...exceptions import (
+from orquestra.sdk._shared import ProjectRef, iter_invocations_topologically, serde
+from orquestra.sdk._shared.abc import RuntimeInterface
+from orquestra.sdk._shared.exceptions import (
     ConfigFileNotFoundError,
     ConfigNameNotFoundError,
     ProjectInvalidError,
     QERemoved,
     RayNotRunningError,
     RemoteConnectionError,
     RuntimeQuerySummaryError,
@@ -28,33 +32,33 @@
     VersionMismatch,
     WorkflowRunCanNotBeTerminated,
     WorkflowRunNotFinished,
     WorkflowRunNotFoundError,
     WorkflowRunNotSucceeded,
     WorkspacesNotSupportedError,
 )
-from ...schema import ir
-from ...schema.configs import ConfigName
-from ...schema.responses import WorkflowResult
-from ...schema.workflow_run import ProjectId, State
-from ...schema.workflow_run import TaskRun as TaskRunModel
-from ...schema.workflow_run import TaskRunId
-from ...schema.workflow_run import WorkflowRun as WorkflowRunModel
-from ...schema.workflow_run import (
+from orquestra.sdk._shared.exec_ctx import ExecContext, get_current_exec_context
+from orquestra.sdk._shared.logs import WorkflowLogs
+from orquestra.sdk._shared.schema import ir
+from orquestra.sdk._shared.schema.configs import ConfigName
+from orquestra.sdk._shared.schema.responses import WorkflowResult
+from orquestra.sdk._shared.schema.workflow_run import ProjectId, State
+from orquestra.sdk._shared.schema.workflow_run import TaskRun as TaskRunModel
+from orquestra.sdk._shared.schema.workflow_run import TaskRunId
+from orquestra.sdk._shared.schema.workflow_run import WorkflowRun as WorkflowRunModel
+from orquestra.sdk._shared.schema.workflow_run import (
     WorkflowRunId,
     WorkflowRunMinimal,
     WorkflowRunSummary,
     WorkspaceId,
 )
-from .. import serde
-from .._graphs import iter_invocations_topologically
-from .._logs._interfaces import WorkflowLogs
+
+from .._config import IN_PROCESS_CONFIG_NAME, RAY_CONFIG_NAME_ALIAS
+from .._env import CURRENT_CLUSTER_ENV, CURRENT_PROJECT_ENV, CURRENT_WORKSPACE_ENV
 from .._spaces._resolver import resolve_studio_ref, resolve_studio_workspace_ref
-from .._spaces._structs import ProjectRef
-from ..abc import RuntimeInterface
 from ._config import RuntimeConfig, resolve_config
 from ._task_run import TaskRun
 
 
 class WorkflowRun:
     """Represents a single "execution" of a workflow.
 
@@ -871,7 +875,68 @@
         "- s or S: seconds\n"
         "For example:\n"
         '- "9h32m" = 9 hours and 32 minutes,\n'
         '- "8H6S" = 8 hours and 6 seconds,\n'
         '- "10m" = 10 minutes,\n'
         '- "3D6h8M13s" = 3 days, 6 hours, 8 minutes and 13 seconds.'
     )
+
+
+def _get_workspace_and_project_ids() -> (
+    t.Tuple[t.Optional[WorkspaceId], t.Optional[ProjectId]]
+):
+    if not os.getenv(CURRENT_CLUSTER_ENV):
+        return None, None
+
+    return os.getenv(CURRENT_WORKSPACE_ENV), os.getenv(CURRENT_PROJECT_ENV)
+
+
+def _generate_cluster_uri_name(uri: str) -> str:
+    return str(urlparse(uri).path).split(".")[0]
+
+
+def _get_config_context() -> str:
+    cluster_uri = os.getenv(CURRENT_CLUSTER_ENV)
+    if not cluster_uri:
+        context = get_current_exec_context()
+        if context == ExecContext.RAY:
+            return RAY_CONFIG_NAME_ALIAS
+        elif context == ExecContext.DIRECT:
+            return IN_PROCESS_CONFIG_NAME
+        else:
+            raise NotImplementedError(
+                f"Got unexpected global context {context}. Please report this as a bug."
+            )
+
+    return _generate_cluster_uri_name(cluster_uri)
+
+
+class CurrentExecutionCtx(t.NamedTuple):
+    config_name: ConfigName
+    workspace_id: t.Optional[WorkspaceId]
+    project_id: t.Optional[ProjectId]
+
+
+def current_exec_ctx() -> CurrentExecutionCtx:
+    """Get the backend IDs related to current workflow execution context.
+
+    config_name is the name of the config used to execute current workflow.
+
+    workspace_id  and project_id are the workspace and project
+    in which the workflow is executed. If run locally, they are set to None.
+
+    This function is intended to be used within the task code in the following way::
+
+        @sdk.task
+        def t():
+            config_name, workspace_id, project_id =  sdk.current_exec_ctx()
+            ...
+
+    Returns:
+        The config, workspace and project IDs associated with the current
+            run, in a named tuple. See: CurrentWorkflowIDs
+    """
+    config = _get_config_context()
+    workspace_id, project_id = _get_workspace_and_project_ids()
+    return CurrentExecutionCtx(
+        config_name=config, workspace_id=workspace_id, project_id=project_id
+    )
```

## Comparing `orquestra/sdk/_base/_driver/_ce_runtime.py` & `orquestra/sdk/_client/_base/_driver/_ce_runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,35 +3,47 @@
 ################################################################################
 """RuntimeInterface implementation that uses Compute Engine."""
 import warnings
 from datetime import timedelta
 from pathlib import Path
 from typing import Dict, List, Optional, Protocol, Sequence, Union
 
-from orquestra.sdk import Project, ProjectRef, Workspace, exceptions
-from orquestra.sdk._base import _retry, serde
-from orquestra.sdk._base._logs import _regrouping
-from orquestra.sdk._base._logs._interfaces import LogOutput, WorkflowLogs
-from orquestra.sdk._base._logs._models import LogAccumulator, LogStreamType
-from orquestra.sdk._base.abc import RuntimeInterface
-from orquestra.sdk.exceptions import IgnoredFieldWarning
-from orquestra.sdk.kubernetes.quantity import parse_quantity
-from orquestra.sdk.schema.configs import RuntimeConfiguration
-from orquestra.sdk.schema.ir import ArtifactFormat, TaskInvocationId, WorkflowDef
-from orquestra.sdk.schema.responses import ComputeEngineWorkflowResult, WorkflowResult
-from orquestra.sdk.schema.workflow_run import (
+from orquestra.sdk._shared import Project, ProjectRef, Workspace, exceptions, serde
+from orquestra.sdk._shared.abc import RuntimeInterface
+from orquestra.sdk._shared.exceptions import IgnoredFieldWarning
+from orquestra.sdk._shared.kubernetes.quantity import parse_quantity
+from orquestra.sdk._shared.logs import (
+    LogAccumulator,
+    LogOutput,
+    LogStreamType,
+    WorkflowLogs,
+    is_env_setup,
+    is_worker,
+)
+from orquestra.sdk._shared.schema.configs import RuntimeConfiguration
+from orquestra.sdk._shared.schema.ir import (
+    ArtifactFormat,
+    TaskInvocationId,
+    WorkflowDef,
+)
+from orquestra.sdk._shared.schema.responses import (
+    ComputeEngineWorkflowResult,
+    WorkflowResult,
+)
+from orquestra.sdk._shared.schema.workflow_run import (
     State,
     TaskRunId,
     WorkflowRun,
     WorkflowRunId,
     WorkflowRunMinimal,
     WorkflowRunSummary,
     WorkspaceId,
 )
 
+from ..._base import _retry
 from . import _client, _exceptions, _models
 
 
 class PaginatedListFunc(Protocol):
     """Protocol for functions passed to CERuntime._list_wf_runs()."""
 
     def __call__(
@@ -608,21 +620,21 @@
                 # If a task's logs aren't available, keep going
                 pass
 
         for m in messages:
             # Default to "log.out" if no log filenames
             path = Path(m.ray_filename)
             stream = LogStreamType.by_file(path)
-            if _regrouping.is_worker(path=path):
+            if is_worker(path=path):
                 # We previously added Ray worker logs under task logs with
                 # "UNKNOWN TASK INV".
                 # Now, we get task logs from the CE API directly and add the
                 # worker logs to "other".
                 other_logs.add_line_by_stream(stream, m.log)
-            elif _regrouping.is_env_setup(path=path):
+            elif is_env_setup(path=path):
                 env_logs.add_line_by_stream(stream, m.log)
             else:
                 # Reasons for the "other" logs: future proofness and empathy. The server
                 # might return events from more files in the future. We want to let the
                 # user see it even this version of the SDK doesn't know how to
                 # categorize it. Noisy data is better than no data when the user is
                 # trying to find a bug.
```

## Comparing `orquestra/sdk/_base/_driver/_client.py` & `orquestra/sdk/_client/_base/_driver/_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,28 +15,30 @@
 from typing import Generic, List, Mapping, Optional, Tuple, TypeVar, Union, cast
 from urllib.parse import urljoin
 
 import pydantic
 import requests
 from requests import codes
 
-from orquestra.sdk import ProjectRef, exceptions
-from orquestra.sdk._base._spaces._api import make_workspace_zri
-from orquestra.sdk.schema.ir import WorkflowDef
-from orquestra.sdk.schema.responses import ComputeEngineWorkflowResult, WorkflowResult
-from orquestra.sdk.schema.workflow_run import (
+from orquestra.sdk._shared import VERSION_REGEX, ProjectRef, exceptions
+from orquestra.sdk._shared.orqdantic import TypeAdapter
+from orquestra.sdk._shared.schema.ir import WorkflowDef
+from orquestra.sdk._shared.schema.responses import (
+    ComputeEngineWorkflowResult,
+    WorkflowResult,
+)
+from orquestra.sdk._shared.schema.workflow_run import (
     State,
     WorkflowRun,
     WorkflowRunMinimal,
     WorkflowRunSummary,
     WorkspaceId,
 )
 
-from ..._base._storage import TypeAdapter
-from .._regex import VERSION_REGEX
+from .._spaces._api import make_workspace_zri
 from . import _exceptions, _models
 
 
 def _match_unsupported_version(error_detail: str):
     # We try to match format of the error message to parse the supported and
     # submitted versions.
     # If we fail, we return None and carry on.
```

## Comparing `orquestra/sdk/_base/_driver/_exceptions.py` & `orquestra/sdk/_client/_base/_driver/_exceptions.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/_base/_driver/_models.py` & `orquestra/sdk/_client/_base/_driver/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,28 @@
     TypeVar,
     Union,
 )
 
 import pydantic
 from typing_extensions import Annotated
 
-from orquestra.sdk._base._dates import Instant
-from orquestra.sdk.schema.ir import WorkflowDef
-from orquestra.sdk.schema.workflow_run import (
+from orquestra.sdk._shared.dates import Instant
+from orquestra.sdk._shared.orqdantic import BaseModel
+from orquestra.sdk._shared.schema.ir import WorkflowDef
+from orquestra.sdk._shared.schema.workflow_run import (
     ProjectId,
     RunStatus,
     State,
     TaskRun,
     WorkflowRun,
     WorkflowRunMinimal,
     WorkflowRunSummary,
     WorkspaceId,
 )
 
-from ..._base._storage import BaseModel
-
 WorkflowDefID = str
 WorkflowRunID = str
 TaskRunID = str
 TaskInvocationID = str
 WorkflowRunArtifactID = str
 WorkflowRunResultID = str
```

## Comparing `orquestra/sdk/_base/_logs/_interfaces.py` & `orquestra/sdk/_shared/logs/_interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 """Logs-related interfaces."""
 import typing as t
 from dataclasses import dataclass
 from enum import Enum
 
-from orquestra.sdk.schema.ir import TaskInvocationId
-from orquestra.sdk.schema.workflow_run import WorkflowRunId
+from ..schema.ir import TaskInvocationId
+from ..schema.workflow_run import WorkflowRunId
 
 
 @dataclass(frozen=True)
 class LogOutput:
     out: t.List[str]
     err: t.List[str]
```

## Comparing `orquestra/sdk/_base/_logs/_markers.py` & `orquestra/sdk/_runtime/_ray/_logs/_markers.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 import sys
 import traceback
 import typing as t
 from contextlib import contextmanager
 from dataclasses import dataclass
 from pathlib import Path
 
-from orquestra.sdk.schema.ir import TaskInvocationId
-from orquestra.sdk.schema.workflow_run import WorkflowRunId
-
-from .. import _dates
+from orquestra.sdk._shared.dates import Instant, from_isoformat, local_isoformat
+from orquestra.sdk._shared.dates import now as dates_now
+from orquestra.sdk._shared.schema.ir import TaskInvocationId
+from orquestra.sdk._shared.schema.workflow_run import WorkflowRunId
 
 ORQ_MARKER_PREFIX = "ORQ-MARKER:"
 ORQ_MARKER_PATTERN = re.compile(re.escape(ORQ_MARKER_PREFIX) + r"(.+)")
 
 
 UNKNOWN_WF_RUN_ID = "unknown-wf-run-id"
 UNKNOWN_TASK_INV_ID = "unknown-task-inv-id"
@@ -33,30 +33,30 @@
 def print_start(wf_run_id: WorkflowRunId, task_inv_id: TaskInvocationId):
     """Emits "task start" marker to stdout and stderr.
 
     Required for task-log correlation.
 
     See: ORQSDK-951 and ORQSDK-952 for deprecation strategy
     """
-    now = _dates.now()
+    now = dates_now()
     marker = TaskStartMarker(
         wf_run_id=wf_run_id, task_inv_id=task_inv_id, timestamp=now
     )
     print(marker.line)
     print(marker.line, file=sys.stderr)
 
 
 def print_end(wf_run_id: WorkflowRunId, task_inv_id: TaskInvocationId):
     """Emits "task end" marker to stdout and stderr.
 
     Required for task-log correlation.
 
     See: ORQSDK-951 and ORQSDK-952 for deprecation strategy
     """
-    now = _dates.now()
+    now = dates_now()
     marker = TaskEndMarker(wf_run_id=wf_run_id, task_inv_id=task_inv_id, timestamp=now)
     print(marker.line)
     print(marker.line, file=sys.stderr)
 
 
 @contextmanager
 def capture_logs(
@@ -120,15 +120,17 @@
     log_path = logs_dir / "wf" / wf_run_id / "task"
     out_path = log_path / f"{task_inv_id}.out"
     err_path = log_path / f"{task_inv_id}.err"
 
     log_path.mkdir(parents=True, exist_ok=True)
 
     with open(out_path, "a") as out_f, open(err_path, "a") as err_f:
-        with wurlitzer.pipes(stdout=out_f, stderr=err_f):
+        # wurlizner lacks type annotations, thus we do pyright ignore
+        # https://github.com/minrk/wurlitzer/issues/80
+        with wurlitzer.pipes(stdout=out_f, stderr=err_f):  # pyright: ignore
             try:
                 yield
             except Exception as e:
                 traceback.print_exception(type(e), e, e.__traceback__)
                 raise
 
 
@@ -138,21 +140,21 @@
 
     See: ORQSDK-951 and ORQSDK-952 for deprecation strategy
     """
 
     event = "task_start"
     wf_run_id: WorkflowRunId
     task_inv_id: TaskInvocationId
-    timestamp: _dates.Instant
+    timestamp: Instant
 
     @property
     def line(self) -> str:
         event = {
             "event": self.event,
-            "timestamp": _dates.local_isoformat(self.timestamp),
+            "timestamp": local_isoformat(self.timestamp),
             "wf_run_id": self.wf_run_id,
             "task_inv_id": self.task_inv_id,
         }
         return f"{ORQ_MARKER_PREFIX}{json.dumps(event)}"
 
 
 @dataclass(frozen=True)
@@ -161,21 +163,21 @@
 
     See: ORQSDK-951 and ORQSDK-952 for deprecation strategy
     """
 
     event = "task_end"
     wf_run_id: t.Optional[WorkflowRunId]
     task_inv_id: t.Optional[TaskInvocationId]
-    timestamp: _dates.Instant
+    timestamp: Instant
 
     @property
     def line(self) -> str:
         event = {
             "event": self.event,
-            "timestamp": _dates.local_isoformat(self.timestamp),
+            "timestamp": local_isoformat(self.timestamp),
             **({"wf_run_id": self.wf_run_id} if self.wf_run_id else {}),
             **({"task_inv_id": self.task_inv_id} if self.task_inv_id else {}),
         }
         return f"{ORQ_MARKER_PREFIX}{json.dumps(event)}"
 
 
 Marker = t.Union[TaskStartMarker, TaskEndMarker]
@@ -203,19 +205,19 @@
 
     event_dict = json.loads(match.group(1))
     try:
         if event_dict["event"] == TaskStartMarker.event:
             return TaskStartMarker(
                 wf_run_id=event_dict["wf_run_id"],
                 task_inv_id=event_dict["task_inv_id"],
-                timestamp=_dates.from_isoformat(event_dict["timestamp"]),
+                timestamp=from_isoformat(event_dict["timestamp"]),
             )
         elif event_dict["event"] == TaskEndMarker.event:
             return TaskEndMarker(
                 wf_run_id=event_dict.get("wf_run_id"),
                 task_inv_id=event_dict.get("task_inv_id"),
-                timestamp=_dates.from_isoformat(event_dict["timestamp"]),
+                timestamp=from_isoformat(event_dict["timestamp"]),
             )
         else:
             return None
     except KeyError:
         return None
```

## Comparing `orquestra/sdk/_base/_logs/_models.py` & `orquestra/sdk/_shared/logs/_models.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/_base/_logs/_regrouping.py` & `orquestra/sdk/_shared/logs/_regrouping.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/_base/_spaces/_api.py` & `orquestra/sdk/_client/_base/_spaces/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 import typing as t
 
-from orquestra.sdk.exceptions import ConfigNameNotFoundError
+from orquestra.sdk._shared import Project, Workspace
+from orquestra.sdk._shared.exceptions import ConfigNameNotFoundError
+from orquestra.sdk._shared.schema.configs import ConfigName
+from orquestra.sdk._shared.schema.workflow_run import WorkspaceId
 
-from ...schema.configs import ConfigName
-from ...schema.workflow_run import WorkspaceId
 from .._api._config import RuntimeConfig, resolve_config
-from ._structs import Project, Workspace
 
 
 def list_workspaces(
     config: t.Union[ConfigName, "RuntimeConfig"],
 ) -> t.Sequence[Workspace]:
     """Get the list of all workspaces available to a user.
```

## Comparing `orquestra/sdk/_base/_spaces/_resolver.py` & `orquestra/sdk/_client/_base/_spaces/_resolver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 import os
 from typing import Optional
 
-from orquestra.sdk.exceptions import ProjectInvalidError
-from orquestra.sdk.schema.workflow_run import ProjectId, WorkspaceId
+from orquestra.sdk._shared import ProjectRef
+from orquestra.sdk._shared.exceptions import ProjectInvalidError
+from orquestra.sdk._shared.schema.workflow_run import ProjectId, WorkspaceId
 
 from .._env import CURRENT_PROJECT_ENV, CURRENT_WORKSPACE_ENV
-from ._structs import ProjectRef
 
 
 def resolve_studio_ref(
     workspace_id: Optional[WorkspaceId],
     project_id: Optional[ProjectId],
 ) -> Optional[ProjectRef]:
     """Resolve the workspace and project IDs from the passed args or environment vars.
```

## Comparing `orquestra/sdk/_base/_spaces/_structs.py` & `orquestra/sdk/_shared/_spaces/_structs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 from dataclasses import dataclass
 
-from orquestra.sdk.schema.workflow_run import ProjectId, WorkspaceId
+from ..schema.workflow_run import ProjectId, WorkspaceId
 
 
 @dataclass(frozen=True)
 class ProjectRef:
     workspace_id: WorkspaceId
     project_id: ProjectId
```

## Comparing `orquestra/sdk/_base/_storage/orqdantic.py` & `orquestra/sdk/_shared/orqdantic/orqdantic.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/_base/_testing/_connections.py` & `orquestra/sdk/_client/_base/_testing/_connections.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import platform
 import random
 import shutil
 import typing as t
 from contextlib import contextmanager
 from pathlib import Path
 
-from orquestra.sdk._ray import _dag
+from orquestra.sdk._runtime._ray import _dag
 
 
 @contextmanager
 def ray_suitable_temp_dir():
     """Context manager that generates a temporary directory.
 
     The content of the directory is removed at content at exit.
@@ -66,14 +66,18 @@
     To do that, set the 'RAY_CLUSTER_URL' env variable.
     `RAY_CLUSTER_URL="auto"` tells Ray to discover a running cluster.
 
     Yields the params used to initialize the connection.
     """
     cluster_url_env = os.getenv("RAY_CLUSTER_URL")
 
+    # variable used for testing of overwriting env variables in worker nodes.
+    # it needs to be set before ray cluster is started
+    os.environ["MY_NEW_SECRET_ENV"] = "SET_BEFORE_RAY_STARTS"
+
     with ray_suitable_temp_dir() as tmp_path:
         if cluster_url_env is not None:
             # Connecting to a background cluster?
             # - Use the address from the env var.
             # - Can't pass storage path.
             # - We shouldn't pass temp dir path either.
             address = cluster_url_env
```

## Comparing `orquestra/sdk/_base/_testing/_example_wfs.py` & `orquestra/sdk/_client/_base/_testing/_example_wfs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 ################################################################################
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 import time
 from typing import Optional, Sequence, Tuple
 
 import orquestra.sdk as sdk
-import orquestra.sdk._base._testing._ipc as ipc
+
+from . import _ipc as ipc
 
 
 @sdk.task
 def make_greeting(name, company_name):
     return f"yooooo {name} from {company_name}"
 
 
@@ -79,27 +80,27 @@
 @sdk.task
 def make_company_name(last_name: str):
     return f"{last_name} computing"
 
 
 @sdk.task(
     source_import=sdk.GitImport(
-        repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
+        repo_url="git@github.com:zapata-engineering/orquestra-sdk.git",
         git_ref="main",
     ),
     dependency_imports=[],
 )
 def make_greeting_message(first, last, additional_message: Optional[str] = None) -> str:
     return f"hello, {first} {last}!{additional_message or ''}"
 
 
 @sdk.task(
     n_outputs=2,
     source_import=sdk.GitImport(
-        repo_url="git@github.com:zapatacomputing/orquestra-workflow-sdk.git",
+        repo_url="git@github.com:zapata-engineering/orquestra-sdk.git",
         git_ref="main",
     ),
     dependency_imports=[],
 )
 def multi_output_test():
     return "hello", "there"
 
@@ -319,17 +320,17 @@
 @sdk.workflow
 def wf_with_log(msg: str):
     return [add_with_log(12, 34, msg)]
 
 
 @sdk.task
 def get_exec_ctx() -> str:
-    import orquestra.sdk._base._exec_ctx
+    import orquestra.sdk._shared.exec_ctx
 
-    ctx = orquestra.sdk._base._exec_ctx.global_context
+    ctx = orquestra.sdk._shared.exec_ctx.get_current_exec_context()
     return ctx.name
 
 
 @sdk.workflow
 def wf_with_exec_ctx():
     return [get_exec_ctx()]
 
@@ -398,7 +399,28 @@
 def cause_env_setup_error():
     """This WF errors out during environment setup so we can test how it is handled.
 
     Jinja2 relies on a higher version of MarkupSafe, so the dependency imports for the
     cause_env_setup_error_task task will cause pip to throw an error.
     """
     return [cause_env_setup_error_task()]
+
+
+class GetEnvWhileReduce:
+    def __init__(self):
+        import os
+
+        self.val = os.getenv("MY_UNIQUE_ENV")
+
+    def __reduce__(self):
+        return (GetEnvWhileReduce, tuple())
+
+
+@sdk.task(env_vars={"MY_UNIQUE_ENV": "MY_UNIQUE_VALUE"})
+def get_env_task(obj):
+    return obj.val
+
+
+@sdk.workflow
+def get_env_before_task_executes_task():
+    obj = GetEnvWhileReduce()
+    return [get_env_task(obj)]
```

## Comparing `orquestra/sdk/_base/_testing/_ipc.py` & `orquestra/sdk/_client/_base/_testing/_ipc.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/_base/_testing/_reloaders.py` & `orquestra/sdk/_client/_base/_testing/_reloaders.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/_base/cli/_arg_resolvers.py` & `orquestra/sdk/_client/_base/cli/_arg_resolvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 resolve the information from other sources.
 This module contains the CLI argument resolution logic extracted as components reusable
 across similar CLI commands.
 """
 import typing as t
 import warnings
 
-from orquestra.sdk import exceptions
-from orquestra.sdk._base import _services
-from orquestra.sdk._base._config import IN_PROCESS_CONFIG_NAME
-from orquestra.sdk._base._logs._interfaces import WorkflowLogs
-from orquestra.sdk.schema.configs import ConfigName
-from orquestra.sdk.schema.ir import TaskInvocationId
-from orquestra.sdk.schema.workflow_run import (
+from orquestra.sdk._shared import exceptions
+from orquestra.sdk._shared.logs import WorkflowLogs
+from orquestra.sdk._shared.schema.configs import ConfigName
+from orquestra.sdk._shared.schema.ir import TaskInvocationId
+from orquestra.sdk._shared.schema.workflow_run import (
     ProjectId,
     State,
     TaskRunId,
     WorkflowRun,
     WorkflowRunId,
     WorkspaceId,
 )
 
+from ..._base import _services
+from ..._base._config import IN_PROCESS_CONFIG_NAME
 from . import _repos
 from ._ui import _presenters, _prompts
 
 
 def _check_for_in_process(config_names: t.Sequence[ConfigName]):
     if IN_PROCESS_CONFIG_NAME in config_names:
         raise exceptions.InProcessFromCLIError()
```

## Comparing `orquestra/sdk/_base/cli/_dumpers.py` & `orquestra/sdk/_client/_base/cli/_dumpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ################################################################################
-# © Copyright 2023 Zapata Computing Inc.
+# © Copyright 2023-2024 Zapata Computing Inc.
 ################################################################################
 
 """Code that stores values on disk as a result of a CLI command."""
 import typing as t
 from functools import singledispatchmethod
 from pathlib import Path
 
-from orquestra.sdk._base import serde
-from orquestra.sdk._base._logs._interfaces import WorkflowLogs
-from orquestra.sdk.schema.workflow_run import TaskInvocationId, WorkflowRunId
+from orquestra.sdk._shared import serde
+from orquestra.sdk._shared.logs import LogOutput, WorkflowLogs
+from orquestra.sdk._shared.schema.workflow_run import TaskInvocationId, WorkflowRunId
 
 
 class WFOutputDumper:
     """Writes a workflow run's output artifacts to a file."""
 
     def dump(
         self,
@@ -74,63 +74,93 @@
     """Writes logs to files."""
 
     @staticmethod
     def _get_logs_file(
         dir_path: Path,
         wf_run_id: WorkflowRunId,
         log_type: t.Optional[WorkflowLogs.WorkflowLogTypeName] = None,
+        is_stderr: bool = False,
     ) -> Path:
         dir_path.mkdir(parents=True, exist_ok=True)
+        extension = "err" if is_stderr else "log"
         if log_type:
             return (
-                dir_path / f"{wf_run_id}_{log_type.value.lower().replace(' ', '_')}.log"
+                dir_path
+                / f"{wf_run_id}_{log_type.value.lower().replace(' ', '_')}.{extension}"
             )
-        return dir_path / f"{wf_run_id}.log"
+        return dir_path / f"{wf_run_id}.{extension}"
 
     def dump(
         self,
-        logs: t.Union[t.Mapping[TaskInvocationId, t.Sequence[str]], t.Sequence[str]],
+        logs: t.Union[
+            t.Mapping[TaskInvocationId, t.Sequence[str]],
+            t.Sequence[str],
+            LogOutput,
+            t.Mapping[TaskInvocationId, LogOutput],
+        ],
         wf_run_id: WorkflowRunId,
         dir_path: Path,
         log_type: t.Optional[WorkflowLogs.WorkflowLogTypeName] = None,
     ):
         """Save logs from wf into a file.
 
         Creates missing directories.
         Generates filenames based on ``wf_run_id``.
         No standard errors are expected to be raised.
         """
         logs_file = self._get_logs_file(dir_path, wf_run_id, log_type=log_type)
+        err_logs_file = self._get_logs_file(
+            dir_path, wf_run_id, log_type=log_type, is_stderr=True
+        )
 
-        log_lines = self._construct_output_log_lines(logs)
+        out_lines, err_lines = self._construct_output_log_lines(logs)
 
         with logs_file.open("w") as f:
-            f.writelines(log_lines)
+            f.writelines("\n".join(out_lines))
+
+        with err_logs_file.open("w") as f:
+            f.writelines("\n".join(err_lines))
 
-        return logs_file
+        return logs_file, err_logs_file
 
     @singledispatchmethod
     @staticmethod
-    def _construct_output_log_lines(_, *args) -> t.List[str]:
+    def _construct_output_log_lines(*args) -> t.Tuple[t.List[str], t.List[str]]:
         """Construct a list of log lines to be printed.
 
         This method has overloads for dict and list arguments.
         """
         raise NotImplementedError(
             f"No log lines constructor for args {args}"
         )  # pragma: no cover
 
+    @_construct_output_log_lines.register(LogOutput)
+    @staticmethod
+    def _(logs: LogOutput) -> t.Tuple[t.List[str], t.List[str]]:
+        return logs.out, logs.err
+
     @_construct_output_log_lines.register(dict)
     @staticmethod
-    def _(logs: dict) -> t.List[str]:
+    def _(
+        logs: t.Union[
+            t.Mapping[TaskInvocationId, t.Sequence[str]],
+            t.Mapping[TaskInvocationId, LogOutput],
+        ]
+    ) -> t.Tuple[t.List[str], t.List[str]]:
         outlines = []
-        for task_invocation in logs:
-            outlines.append(f"Logs for task invocation: {task_invocation}:\n\n")
-            for log in logs[task_invocation]:
-                outlines.append(log + "\n")
-            outlines.append("\n\n")
-        return outlines
+        errlines = []
+        for task_invocation_id, log_values in logs.items():
+            outlines.append(f"stdout logs for task invocation: {task_invocation_id}:\n")
+            errlines.append(f"stderr logs for task invocation: {task_invocation_id}:\n")
+            if isinstance(log_values, LogOutput):
+                outlines.extend(log_values.out)
+                errlines.extend(log_values.err)
+            else:
+                outlines.extend(log_values)
+            outlines.append("\n")
+            errlines.append("\n")
+        return outlines, errlines
 
     @_construct_output_log_lines.register(list)
     @staticmethod
-    def _(logs: list) -> t.List[str]:
-        return [log + "\n" for log in logs]
+    def _(logs: list) -> t.Tuple[t.List[str], t.List[str]]:
+        return logs, []
```

## Comparing `orquestra/sdk/_base/cli/_entry.py` & `orquestra/sdk/_client/_base/cli/_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 """
 import typing as t
 from pathlib import Path
 
 import click
 import cloup
 
-from orquestra.sdk._base.cli._ui._click_default_group import DefaultGroup
-from orquestra.sdk.schema.configs import RuntimeName
+from orquestra.sdk._shared.schema.configs import RuntimeName
 
 from . import _cli_logs
+from ._ui._click_default_group import DefaultGroup
 
 # Adds '-h' alias for '--help'
 CLICK_CTX_SETTINGS = {"help_option_names": ["-h", "--help"]}
 
 DOWNLOAD_DIR_OPTION = cloup.option(
     "--download-dir",
     help=(
@@ -422,16 +422,19 @@
     up,
     down,
     status,
     restart,
 )
 
 
+# Ignoring pyright errors as this class inherits typing issues form 3rd party code
 # region: login
-class GroupWithDefaultCommand(cloup.Group, DefaultGroup):
+class GroupWithDefaultCommand(  # pyright: ignore[reportIncompatibleMethodOverride, reportIncompatibleVariableOverride] # noqa: E501
+    cloup.Group, DefaultGroup
+):
     ...
 
     def get_help(self, ctx) -> str:
         # Hack to get the help for `orq login` to make sense
         sub = super().get_help(ctx).split("\n")
         return auth.get_help(ctx) + "\n\n" + "\n".join(sub[sub.index("Commands:") :])
```

## Comparing `orquestra/sdk/_base/cli/_repos.py` & `orquestra/sdk/_client/_base/cli/_repos.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,39 +14,40 @@
 from functools import singledispatch
 from types import ModuleType
 
 import requests
 from typing_extensions import assert_never
 
 from orquestra import sdk
-from orquestra.sdk import exceptions
-from orquestra.sdk._base import _config, _dates, loader
-from orquestra.sdk._base._driver._client import DriverClient, ExternalUriProvider
-from orquestra.sdk._base._jwt import check_jwt_without_signature_verification
-from orquestra.sdk._base._logs._interfaces import LogOutput, WorkflowLogs
-from orquestra.sdk._base.abc import ArtifactValue
-from orquestra.sdk.schema import _compat
-from orquestra.sdk.schema.configs import (
+from orquestra.sdk._shared import exceptions
+from orquestra.sdk._shared.abc import ArtifactValue
+from orquestra.sdk._shared.dates import from_unix_time
+from orquestra.sdk._shared.logs import LogOutput, WorkflowLogs
+from orquestra.sdk._shared.schema import result_is_packed
+from orquestra.sdk._shared.schema.configs import (
     ConfigName,
     RemoteRuntime,
     RuntimeConfiguration,
     RuntimeName,
 )
-from orquestra.sdk.schema.ir import TaskInvocationId, WorkflowDef
-from orquestra.sdk.schema.workflow_run import (
+from orquestra.sdk._shared.schema.ir import TaskInvocationId, WorkflowDef
+from orquestra.sdk._shared.schema.workflow_run import (
     ProjectId,
     State,
     TaskRun,
     TaskRunId,
     WorkflowRun,
     WorkflowRunId,
     WorkflowRunSummary,
     WorkspaceId,
 )
 
+from ..._base import _config, loader
+from ..._base._driver._client import DriverClient, ExternalUriProvider
+from ..._base._jwt import check_jwt_without_signature_verification
 from ._ui import _models as ui_models
 
 
 def _find_first(f: t.Callable[[t.Any], bool], it: t.Iterable):
     return next(filter(f, it))
 
 
@@ -371,15 +372,15 @@
         # on the IR.
         task_outputs = task_run.get_outputs()
 
         wf_def = wf_run.get_status_model().workflow_def
         invocation = wf_def.task_invocations[task_inv_id]
         task_def = wf_def.tasks[invocation.task_id]
 
-        if _compat.result_is_packed(task_def=task_def):
+        if result_is_packed(task_def=task_def):
             # We expect ``task_outputs`` to be an iterable already.
             outputs_tuple = tuple(task_outputs)
         else:
             # ``task_outputs`` is likely to be a single object. We need to wrap it.
             outputs_tuple = (task_outputs,)
 
         return outputs_tuple
@@ -650,15 +651,15 @@
 
         Returns:
             A WFList containing summary lines for the specified workflows.
         """
         wf_runs.sort(
             key=lambda wf_run: wf_run.status.start_time
             if wf_run.status.start_time
-            else _dates.from_unix_time(0)
+            else from_unix_time(0)
         )
 
         return ui_models.WFList(wf_rows=[_ui_model_from_wf(wf) for wf in wf_runs])
 
 
 class ConfigRepo:
     """Wraps accessing ~/.orquestra/config.json."""
```

## Comparing `orquestra/sdk/_base/cli/_config/_list.py` & `orquestra/sdk/_client/_base/cli/_config/_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 
 """Code for 'orq login --list'."""
-from orquestra.sdk._base._jwt import check_jwt_without_signature_verification
-from orquestra.sdk.exceptions import ExpiredTokenError, InvalidTokenError
+from orquestra.sdk._shared.exceptions import ExpiredTokenError, InvalidTokenError
 
+from ..._jwt import check_jwt_without_signature_verification
 from .. import _repos
 from .._ui import _presenters, _prompts
 
 
 class Action:
     """Encapsulates app-related logic for handling ``orq login --list``."""
```

## Comparing `orquestra/sdk/_base/cli/_login/_login.py` & `orquestra/sdk/_client/_base/cli/_login/_login.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ################################################################################
 """Code for 'orq login'."""
 import asyncio
 import typing as t
 
 from aiohttp import web
 
-from orquestra.sdk.exceptions import LocalConfigLoginError, UserCancelledPrompt
-from orquestra.sdk.schema.configs import RemoteRuntime
+from orquestra.sdk._shared.exceptions import LocalConfigLoginError, UserCancelledPrompt
+from orquestra.sdk._shared.schema.configs import RemoteRuntime
 
 from .. import _arg_resolvers, _repos
 from .._ui import _presenters, _prompts
 from ._login_server import LoginServer
 
 
 class Action:
```

## Comparing `orquestra/sdk/_base/cli/_login/_login_server.py` & `orquestra/sdk/_client/_base/cli/_login/_login_server.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/_base/cli/_services/_down.py` & `orquestra/sdk/_client/_base/cli/_services/_down.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 import subprocess
 from typing import Optional
 
-from orquestra.sdk.schema.responses import ServiceResponse
+from orquestra.sdk._shared.schema.responses import ServiceResponse
 
 from .. import _arg_resolvers
 from .._ui import _presenters
 
 
 class Action:
     """Encapsulates app-related logic for handling ``orq services down``.
```

## Comparing `orquestra/sdk/_base/cli/_services/_status.py` & `orquestra/sdk/_client/_base/cli/_services/_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
-from orquestra.sdk.schema.responses import ServiceResponse
+from orquestra.sdk._shared.schema.responses import ServiceResponse
 
 from .. import _arg_resolvers
 from .._ui import _presenters
 
 
 class Action:
     """Encapsulates app-related logic for handling ``orq services status``.
```

## Comparing `orquestra/sdk/_base/cli/_services/_up.py` & `orquestra/sdk/_client/_base/cli/_services/_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 import subprocess
 from typing import Optional
 
-from orquestra.sdk.schema.responses import ServiceResponse
+from orquestra.sdk._shared.schema.responses import ServiceResponse
 
 from .. import _arg_resolvers
 from .._ui import _presenters
 
 
 class Action:
     """Encapsulates app-related logic for handling ``orq services up``.
```

## Comparing `orquestra/sdk/_base/cli/_task/_logs.py` & `orquestra/sdk/_client/_base/cli/_task/_logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 """Code for 'orq workflow logs'."""
 import typing as t
 from pathlib import Path
 
-from orquestra.sdk.schema.configs import ConfigName
-from orquestra.sdk.schema.workflow_run import TaskInvocationId, WorkflowRunId
+from orquestra.sdk._shared.schema.configs import ConfigName
+from orquestra.sdk._shared.schema.workflow_run import TaskInvocationId, WorkflowRunId
 
 from .. import _arg_resolvers, _dumpers, _repos
 from .._ui import _presenters
 
 
 class Action:
     """Encapsulates app-related logic for handling ``orq workflow logs``."""
@@ -74,15 +74,16 @@
         logs = self._wf_run_repo.get_task_logs(
             wf_run_id=resolved_wf_run_id,
             task_inv_id=resolver_task_inv_id,
             config_name=resolved_config,
         )
 
         if download_dir is not None:
-            dump_path = self._dumper.dump(
+            dump_paths = self._dumper.dump(
                 logs=logs,
                 wf_run_id=resolved_wf_run_id,
                 dir_path=download_dir,
             )
-            self._logs_presenter.show_dumped_wf_logs(dump_path)
+            for dump_path in dump_paths:
+                self._logs_presenter.show_dumped_wf_logs(dump_path)
         else:
             self._logs_presenter.show_logs(logs)
```

## Comparing `orquestra/sdk/_base/cli/_task/_results.py` & `orquestra/sdk/_client/_base/cli/_task/_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 """Code for 'orq task results'."""
 import typing as t
 from pathlib import Path
 
-from orquestra.sdk.schema.configs import ConfigName
-from orquestra.sdk.schema.workflow_run import TaskRunId, WorkflowRunId
+from orquestra.sdk._shared.schema.configs import ConfigName
+from orquestra.sdk._shared.schema.workflow_run import TaskRunId, WorkflowRunId
 
 from .. import _arg_resolvers, _dumpers, _repos
 from .._ui import _presenters
 
 
 class Action:
     """Encapsulates app-related logic for handling ``orq task results``."""
```

## Comparing `orquestra/sdk/_base/cli/_ui/_click_default_group.py` & `orquestra/sdk/_client/_base/cli/_ui/_click_default_group.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/_base/cli/_ui/_errors.py` & `orquestra/sdk/_client/_base/cli/_ui/_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 
 import click
 import rich
 from rich.box import SIMPLE_HEAVY
 from rich.console import Console
 from rich.table import Column, Table
 
-from orquestra.sdk import exceptions
-from orquestra.sdk._base._config import IN_PROCESS_CONFIG_NAME, RAY_CONFIG_NAME_ALIAS
-from orquestra.sdk.schema.responses import ResponseStatusCode
+from orquestra.sdk._shared import exceptions
+from orquestra.sdk._shared.schema.responses import ResponseStatusCode
+
+from ...._base._config import IN_PROCESS_CONFIG_NAME, RAY_CONFIG_NAME_ALIAS
 
 
 def _compact_tb(tb: TracebackType):
     return "{}:{}:{}".format(
         tb.tb_frame.f_code.co_name,
         Path(tb.tb_frame.f_code.co_filename).name,
         tb.tb_lineno,
```

## Comparing `orquestra/sdk/_base/cli/_ui/_models.py` & `orquestra/sdk/_client/_base/cli/_ui/_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 Ideally, most data transformations would be already done (like counting the number of
 inished tasks) but should be easy to assert on in tests (e.g. we prefer ``Instant``
 objects instead of date strings).
 """
 import typing as t
 from dataclasses import dataclass
 
-from orquestra.sdk._base._dates import Instant
-from orquestra.sdk.schema import ir
-from orquestra.sdk.schema.workflow_run import RunStatus, WorkflowRunId
+from orquestra.sdk._shared.dates import Instant
+from orquestra.sdk._shared.schema import ir
+from orquestra.sdk._shared.schema.workflow_run import RunStatus, WorkflowRunId
 
 
 @dataclass(frozen=True)
 class WFRunSummary:
     """UI model for ``orq wf view``."""
 
     @dataclass(frozen=True)
```

## Comparing `orquestra/sdk/_base/cli/_ui/_presenters.py` & `orquestra/sdk/_client/_base/cli/_ui/_presenters.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,27 @@
 from rich.live import Live
 from rich.pretty import Pretty
 from rich.rule import Rule
 from rich.spinner import Spinner
 from rich.table import Column, Table
 from tabulate import tabulate
 
-from orquestra.sdk._base import _dates, _env, serde
-from orquestra.sdk._base._dates import Instant
-from orquestra.sdk._base._logs._interfaces import LogOutput, WorkflowLogs
-from orquestra.sdk.schema import responses
-from orquestra.sdk.schema.configs import ConfigName, RuntimeConfiguration, RuntimeName
-from orquestra.sdk.schema.ir import ArtifactFormat
-from orquestra.sdk.schema.workflow_run import TaskInvocationId, WorkflowRunId
+from orquestra.sdk._shared import serde
+from orquestra.sdk._shared.dates import Instant, from_unix_time
+from orquestra.sdk._shared.logs import LogOutput, WorkflowLogs
+from orquestra.sdk._shared.schema import responses
+from orquestra.sdk._shared.schema.configs import (
+    ConfigName,
+    RuntimeConfiguration,
+    RuntimeName,
+)
+from orquestra.sdk._shared.schema.ir import ArtifactFormat
+from orquestra.sdk._shared.schema.workflow_run import TaskInvocationId, WorkflowRunId
 
+from ...._base import _env
 from . import _errors
 from . import _models as ui_models
 
 
 class RichPresenter:
     def __init__(self, console: Optional[Console] = None):
         self._console = console or Console()
@@ -417,15 +422,15 @@
         # Label is <wf_id> <start_time> tabulated nicely to create good-looking
         # table
         # There is also expectations that labels correspond to matching wfs list indices
         wfs = sorted(
             wfs,
             key=lambda wf: wf.status.start_time
             if wf.status.start_time
-            else _dates.from_unix_time(0),
+            else from_unix_time(0),
             reverse=True,
         )
 
         labels = [[wf.id, _format_datetime(wf.status.start_time)] for wf in wfs]
         tabulated_labels = tabulate(labels, tablefmt="plain").split("\n")
 
         return wfs, tabulated_labels
```

## Comparing `orquestra/sdk/_base/cli/_ui/_prompts.py` & `orquestra/sdk/_client/_base/cli/_ui/_prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import typing as t
 import warnings
 from typing import overload
 
 from inquirer import errors  # type: ignore # noqa
 
-from orquestra.sdk import exceptions
+from orquestra.sdk._shared import exceptions
 
 # One of our transitive dependencies shows DeprecationWarnings related to invalid usage
 # of distutils. There's nothing we can do about it, so until it's fixed upstream we can
 # safely ignore it. See: https://github.com/fmoo/python-editor/issues/35
 warnings.filterwarnings("ignore", module="editor")
 
 import inquirer  # type: ignore # noqa
```

## Comparing `orquestra/sdk/_base/cli/_workflow/_list.py` & `orquestra/sdk/_client/_base/cli/_workflow/_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ################################################################################
 # © Copyright 2022 - 2023 Zapata Computing Inc.
 ################################################################################
 """Code for 'orq workflow list'."""
 import typing as t
 
-from orquestra.sdk import exceptions as exceptions
-from orquestra.sdk.schema.configs import ConfigName
-from orquestra.sdk.schema.workflow_run import WorkflowRunSummary, WorkspaceId
+from orquestra.sdk._shared import exceptions as exceptions
+from orquestra.sdk._shared.schema.configs import ConfigName
+from orquestra.sdk._shared.schema.workflow_run import WorkflowRunSummary, WorkspaceId
 
 from .. import _arg_resolvers, _repos
 from .._ui import _presenters
 
 
 class Action:
     """Encapsulates app-related logic for handling ``orq workflow list``.
```

## Comparing `orquestra/sdk/_base/cli/_workflow/_logs.py` & `orquestra/sdk/_client/_base/cli/_workflow/_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 """Code for 'orq workflow logs'."""
 import typing as t
 import warnings
 from pathlib import Path
 
-from orquestra.sdk._base._logs._interfaces import WorkflowLogs
-from orquestra.sdk.schema.configs import ConfigName
-from orquestra.sdk.schema.workflow_run import WorkflowRunId
+from orquestra.sdk._shared.logs import WorkflowLogs
+from orquestra.sdk._shared.schema.configs import ConfigName
+from orquestra.sdk._shared.schema.workflow_run import WorkflowRunId
 
 from .. import _arg_resolvers, _dumpers, _repos
 from .._ui import _presenters
 
 
 class Action:
     """Encapsulates app-related logic for handling ``orq workflow logs``."""
@@ -101,17 +101,19 @@
 
             log = logs.get_log_type(log_type)
 
             if len(log) < 1:
                 warnings.warn(f"No {log_type} logs found.", category=UserWarning)
                 continue
             if download_dir:
-                dump_path = self._dumper.dump(
+                dump_paths = self._dumper.dump(
                     logs=log,
                     wf_run_id=resolved_wf_run_id,
                     dir_path=download_dir,
                     log_type=log_type,
                 )
-
-                self._logs_presenter.show_dumped_wf_logs(dump_path, log_type=log_type)
+                for dump_path in dump_paths:
+                    self._logs_presenter.show_dumped_wf_logs(
+                        dump_path, log_type=log_type
+                    )
             else:
                 self._logs_presenter.show_logs(log, log_type=log_type)
```

## Comparing `orquestra/sdk/_base/cli/_workflow/_results.py` & `orquestra/sdk/_client/_base/cli/_workflow/_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 """Code for 'orq workflow results'."""
 import typing as t
 from pathlib import Path
 
-from orquestra.sdk.schema.configs import ConfigName
-from orquestra.sdk.schema.workflow_run import WorkflowRunId
+from orquestra.sdk._shared.schema.configs import ConfigName
+from orquestra.sdk._shared.schema.workflow_run import WorkflowRunId
 
 from .. import _arg_resolvers, _dumpers, _repos
 from .._ui import _presenters
 
 
 class Action:
     """Encapsulates app-related logic for handling ``orq workflow results``."""
```

## Comparing `orquestra/sdk/_base/cli/_workflow/_stop.py` & `orquestra/sdk/_client/_base/cli/_workflow/_stop.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 """Code for 'orq workflow stop'."""
 import typing as t
 
-from orquestra.sdk import exceptions
-from orquestra.sdk.schema.configs import ConfigName
-from orquestra.sdk.schema.workflow_run import WorkflowRunId
+from orquestra.sdk._shared import exceptions
+from orquestra.sdk._shared.schema.configs import ConfigName
+from orquestra.sdk._shared.schema.workflow_run import WorkflowRunId
 
 from .. import _arg_resolvers, _repos
 from .._ui import _presenters
 
 
 class Action:
     """Encapsulates app-related logic for handling ``orq workflow stop``.
```

## Comparing `orquestra/sdk/_base/cli/_workflow/_submit.py` & `orquestra/sdk/_client/_base/cli/_workflow/_submit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 """Code for 'orq workflow submit'."""
 import typing as t
 
-from orquestra.sdk import exceptions
+from orquestra.sdk._shared import exceptions
 
 from .. import _arg_resolvers, _repos
 from .._ui import _presenters, _prompts
 
 
 class Action:
     """Encapsulates app-related logic for handling ``orq workflow submit``.
```

## Comparing `orquestra/sdk/_base/cli/_workflow/_view.py` & `orquestra/sdk/_client/_base/cli/_workflow/_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ################################################################################
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 """Code for 'orq workflow view'."""
 import typing as t
 
-from orquestra.sdk.schema.configs import ConfigName
-from orquestra.sdk.schema.workflow_run import WorkflowRunId
+from orquestra.sdk._shared.schema.configs import ConfigName
+from orquestra.sdk._shared.schema.workflow_run import WorkflowRunId
 
 from .. import _arg_resolvers, _repos
 from .._ui import _presenters
 
 
 class Action:
     """Encapsulates app-related logic for handling ``orq workflow view``.
```

## Comparing `orquestra/sdk/_ray/_client.py` & `orquestra/sdk/_runtime/_ray/_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ################################################################################
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 """Facade module for Ray API."""
 import typing as t
 
-from orquestra.sdk.exceptions import (
+from orquestra.sdk._shared.exceptions import (
     NotFoundError,
     UserTaskFailedError,
     WorkflowRunNotFoundError,
 )
 
 try:
     import ray
```

## Comparing `orquestra/sdk/_ray/_dag.py` & `orquestra/sdk/_runtime/_ray/_dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,45 +9,46 @@
 import logging
 import os
 import re
 import typing as t
 import warnings
 from datetime import timedelta
 
-from orquestra.sdk.schema.responses import WorkflowResult
-
-from .. import exceptions
-from .._base import _dates, _services, serde
-from .._base._env import RAY_GLOBAL_WF_RUN_ID_ENV
-from .._base._logs._interfaces import LogReader
-from .._base._spaces._structs import ProjectRef
-from .._base.abc import RuntimeInterface
-from ..schema import ir
-from ..schema.configs import RuntimeConfiguration
-from ..schema.workflow_run import (
+from orquestra.sdk._shared import ProjectRef, exceptions, serde
+from orquestra.sdk._shared.abc import RuntimeInterface
+from orquestra.sdk._shared.dates import Instant, from_unix_time
+from orquestra.sdk._shared.dates import now as dates_now
+from orquestra.sdk._shared.logs import LogReader
+from orquestra.sdk._shared.schema import ir
+from orquestra.sdk._shared.schema.configs import RuntimeConfiguration
+from orquestra.sdk._shared.schema.responses import WorkflowResult
+from orquestra.sdk._shared.schema.workflow_run import (
     RunStatus,
     State,
     TaskInvocationId,
     TaskRun,
     WorkflowRun,
     WorkflowRunId,
     WorkflowRunSummary,
     WorkspaceId,
 )
+
 from . import _client, _id_gen, _ray_logs
 from ._build_workflow import TaskResult, make_ray_dag
+from ._dirs import ray_temp_path
+from ._env import RAY_GLOBAL_WF_RUN_ID_ENV
 from ._wf_metadata import WfUserMetadata, pydatic_to_json_dict
 
 
 def _instant_from_timestamp(
     unix_timestamp: t.Optional[float],
-) -> t.Optional[_dates.Instant]:
+) -> t.Optional[Instant]:
     if unix_timestamp is None:
         return None
-    return _dates.from_unix_time(unix_timestamp)
+    return from_unix_time(unix_timestamp)
 
 
 def _generate_wf_run_id(wf_def: ir.WorkflowDef):
     """Implements the "tagging" design doc.
 
     Doc:
     https://zapatacomputing.atlassian.net/wiki/spaces/ORQSRUN/pages/479920161/Logging+Tagging.
@@ -301,17 +302,15 @@
             _temp_dir=config.runtime_options["temp_dir"],
             configure_logging=config.runtime_options["configure_logging"],
         )
         self.startup(ray_params)
 
         self._config = config
 
-        self._log_reader: LogReader = _ray_logs.DirectLogReader(
-            _services.ray_temp_path()
-        )
+        self._log_reader: LogReader = _ray_logs.DirectLogReader(ray_temp_path())
 
     @classmethod
     def startup(cls, ray_params: RayParams):
         """Initialize a global Ray connection.
 
         If you need a separate connection with different params, you need to call
         .shutdown first().
@@ -502,15 +501,15 @@
     def _normalize_endtimes(model: WorkflowRun) -> WorkflowRun:
         """Set the current time as end_time for tasks and workflows that don't have one.
 
         Ray doesn't provide an end time for terminated tasks and workflows.
         This brought some issues on Workflow Driver, we so fill up the missing status
         fields with the current datetime for all terminated tasks and workflow.
         """
-        now: _dates.Instant = _dates.now()
+        now: Instant = dates_now()
         new_model = model.model_copy(deep=True)
 
         if model.status.start_time is not None and model.status.end_time is None:
             assert now >= model.status.start_time
             new_model.status.end_time = now
 
         for task in new_model.task_runs:
@@ -719,15 +718,15 @@
             state: Only return runs of runs with the specified status.
             workspace: Only return runs from the specified workspace. Not supported
                 on this runtime.
 
         Returns:
                 A list of the workflow runs
         """
-        now = _dates.now()
+        now = dates_now()
 
         if state is not None:
             if not isinstance(state, list):
                 state_list = [state]
             else:
                 state_list = state
         else:
```

## Comparing `orquestra/sdk/_ray/_id_gen.py` & `orquestra/sdk/_runtime/_ray/_id_gen.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/_ray/_ray_logs.py` & `orquestra/sdk/_runtime/_ray/_ray_logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,27 @@
 # © Copyright 2022 - 2023 Zapata Computing Inc.
 ################################################################################
 """Class to get logs from Ray for particular Workflow, both historical and live."""
 import typing as t
 from pathlib import Path
 from typing import Iterator
 
-from orquestra.sdk._base._logs import _markers, _regrouping
-from orquestra.sdk._base._logs._interfaces import LogOutput, WorkflowLogs
-from orquestra.sdk._base._logs._models import LogAccumulator, LogStreamType
-from orquestra.sdk._base._services import redirected_logs_dir
-from orquestra.sdk.schema.ir import TaskInvocationId
-from orquestra.sdk.schema.workflow_run import WorkflowRunId
+from orquestra.sdk._shared.logs import (
+    LogAccumulator,
+    LogOutput,
+    LogStreamType,
+    WorkflowLogs,
+    is_env_setup,
+    is_worker,
+)
+from orquestra.sdk._shared.schema.ir import TaskInvocationId
+from orquestra.sdk._shared.schema.workflow_run import WorkflowRunId
+
+from ._dirs import redirected_logs_dir
+from ._logs import _markers
 
 
 class CapturedLogLines(t.NamedTuple):
     captured_lines: t.Sequence[str]
     workflow_run_id: WorkflowRunId
     task_invocation_id: TaskInvocationId
 
@@ -29,19 +36,19 @@
 
         yield real_path
 
         seen_paths.add(real_path)
 
 
 def iter_user_log_paths(ray_temp: Path) -> t.Iterator[Path]:
-    return filter(_regrouping.is_worker, _iter_logs_paths(ray_temp))
+    return filter(is_worker, _iter_logs_paths(ray_temp))
 
 
 def iter_env_log_paths(ray_temp: Path) -> t.Iterator[Path]:
-    return filter(_regrouping.is_env_setup, _iter_logs_paths(ray_temp))
+    return filter(is_env_setup, _iter_logs_paths(ray_temp))
 
 
 def _iter_log_lines(paths: t.Iterable[Path]) -> t.Iterator[bytes]:
     for path in paths:
         with path.open("rb") as f:
             yield from f
```

## Comparing `orquestra/sdk/_ray/_wf_metadata.py` & `orquestra/sdk/_runtime/_ray/_wf_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ################################################################################
 # © Copyright 2023 - 2024 Zapata Computing Inc.
 ################################################################################
 
 import json
 import typing as t
 
-from .._base._storage import BaseModel
-from ..schema import ir, workflow_run
+from orquestra.sdk._shared.orqdantic import BaseModel
+from orquestra.sdk._shared.schema import ir, workflow_run
 
 
 class WfUserMetadata(BaseModel):
     """Information about a workflow run we store as a Ray metadata dict.
 
     Pydantic helps us check that the thing we read from Ray is indeed a dictionary we
     set (i.e. it has proper fields).
```

## Comparing `orquestra/sdk/dremio/_api.py` & `orquestra/sdk/_client/dremio/_api.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/dremio/_env_var_reader.py` & `orquestra/sdk/_client/dremio/_env_var_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ################################################################################
 # © Copyright 2023-2024 Zapata Computing Inc.
 ################################################################################
 import os
 
-from orquestra.sdk.exceptions import EnvVarNotFoundError
+from orquestra.sdk._shared.exceptions import EnvVarNotFoundError
 
 
 class EnvVarReader:
     def __init__(self, var_name: str):
         self._var_name = var_name
 
     def read(self) -> str:
```

## Comparing `orquestra/sdk/dremio/_flight_facade.py` & `orquestra/sdk/_client/dremio/_flight_facade.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/mlflow/_connection_utils.py` & `orquestra/sdk/_client/mlflow/_connection_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 import warnings
 from pathlib import Path
 from typing import Optional, Tuple
 
 from requests import Response, Session
 
 from orquestra import sdk
-from orquestra.sdk._base import _env
-from orquestra.sdk._base._config import read_config
-from orquestra.sdk._base._env import CURRENT_USER_ENV
-from orquestra.sdk._base._jwt import get_email_from_jwt_token
-from orquestra.sdk._base._services import ORQUESTRA_BASE_PATH
-from orquestra.sdk._base._spaces._api import make_workspace_url, make_workspace_zri
-from orquestra.sdk.exceptions import ConfigNameNotFoundError, RuntimeConfigError
+from orquestra.sdk._shared.exceptions import ConfigNameNotFoundError, RuntimeConfigError
+
+from .._base import _env
+from .._base._config import read_config
+from .._base._env import CURRENT_USER_ENV
+from .._base._jwt import get_email_from_jwt_token
+from .._base._services import ORQUESTRA_BASE_PATH
+from .._base._spaces._api import make_workspace_url, make_workspace_zri
 
 DEFAULT_TEMP_ARTIFACTS_DIR: Path = ORQUESTRA_BASE_PATH / "mlflow" / "artifacts"
 RESOURCE_CATALOG_URI: str = "http://orquestra-resource-catalog.resource-catalog"
 
 
 # region: private
 def _is_executing_remoteley() -> bool:
```

## Comparing `orquestra/sdk/schema/_compat.py` & `orquestra/sdk/_shared/schema/_compat.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/secrets/_api.py` & `orquestra/sdk/_client/secrets/_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 ################################################################################
 # © Copyright 2022 - 2023 Zapata Computing Inc.
 ################################################################################
 """Code for user-facing utilities related to secrets."""
 import typing as t
 
-from .. import exceptions as sdk_exc
-from .._base import _dsl, _exec_ctx
-from ..schema.configs import ConfigName
-from ..schema.workflow_run import WorkspaceId
+from orquestra.sdk._shared import exceptions as sdk_exc
+from orquestra.sdk._shared.exec_ctx import ExecContext, get_current_exec_context
+from orquestra.sdk._shared.schema.configs import ConfigName
+from orquestra.sdk._shared.schema.workflow_run import WorkspaceId
+
+from .._base import _dsl
 from . import _auth, _exceptions, _models
 
 
 def _translate_to_zri(workspace_id: WorkspaceId, secret_name: str) -> str:
     """Create ZRI from workspace_id and secret_name."""
     return f"zri:v1::0:{workspace_id}:secret:{secret_name}"
 
@@ -47,15 +49,15 @@
     Returns:
         Either:
         - the value of the secret
         - if used inside a workflow function (a function decorated with @sdk.workflow),
             this function will return a "future" which will be used to retrieve the
             secret at execution time.
     """
-    if _exec_ctx.global_context == _exec_ctx.ExecContext.WORKFLOW_BUILD:
+    if get_current_exec_context() == ExecContext.WORKFLOW_BUILD:
         return t.cast(
             str,
             _dsl.Secret(name=name, config_name=config_name, workspace_id=workspace_id),
         )
 
     try:
         client = _auth.authorized_client(config_name)
```

## Comparing `orquestra/sdk/secrets/_auth.py` & `orquestra/sdk/_client/secrets/_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ################################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 import os
 import typing as t
 from pathlib import Path
 
-from orquestra.sdk import exceptions
-from orquestra.sdk.schema.configs import ConfigName
+from orquestra.sdk._shared import exceptions
+from orquestra.sdk._shared.schema.configs import ConfigName
 
 from .._base import _config
 from .._base._env import PASSPORT_FILE_ENV
 from ._client import SecretsClient
 
 # We assume that we can access the Config Service under a well-known URI if the passport
 # auth is being used. This relies on the DNS configuration on the remote cluster.
```

## Comparing `orquestra/sdk/secrets/_client.py` & `orquestra/sdk/_client/secrets/_client.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/secrets/_exceptions.py` & `orquestra/sdk/_client/secrets/_exceptions.py`

 * *Files identical despite different names*

## Comparing `orquestra/sdk/secrets/_models.py` & `orquestra/sdk/_client/secrets/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ################################################################################
 """Models for accessing the Config Service API.
 
 API spec: https://github.com/zapatacomputing/config-service/tree/main/openapi/src
 """
 from typing import Optional
 
-from .._base._storage import BaseModel
+from orquestra.sdk._shared.orqdantic import BaseModel
 
 SecretName = str
 SecretValue = str
 ResourceGroup = str
 WorkspaceId = str
```

## Comparing `orquestra_sdk-0.62.0.dist-info/METADATA` & `orquestra_sdk-0.63.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: orquestra-sdk
-Version: 0.62.0
+Version: 0.63.0
 Summary: Compose Orquestra workflows using a Python DSL
-Project-URL: Homepage, https://github.com/zapatacomputing/orquestra-workflow-sdk
+Project-URL: Homepage, https://github.com/zapata-engineering/orquestra-sdk
 Project-URL: Documentation, https://docs.orquestra.io
-Project-URL: Repository, https://github.com/zapatacomputing/orquestra-workflow-sdk.git
-Project-URL: Issues, https://github.com/zapatacomputing/orquestra-workflow-sdk/issues
+Project-URL: Repository, https://github.com/zapata-engineering/orquestra-sdk.git
+Project-URL: Issues, https://github.com/zapata-engineering/orquestra-sdk/issues
 Author-email: "Zapata Computing Inc." <info@zapatacomputing.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -224,47 +224,61 @@
 Requires-Dist: gitpython
 Requires-Dist: graphviz
 Requires-Dist: importlib-metadata>=4.0
 Requires-Dist: inquirer>=3.0
 Requires-Dist: packaging>=21
 Requires-Dist: pandas>=1.4
 Requires-Dist: pip-api>=0.0.30
-Requires-Dist: pyarrow>=10.0
+Requires-Dist: pyarrow<16.0,>=10.0
 Requires-Dist: pydantic>1.10.7
 Requires-Dist: pyjwt>=2.6
 Requires-Dist: requests>=2.28
 Requires-Dist: rich>=13.5
 Requires-Dist: tabulate
 Requires-Dist: typing-extensions>=4.1.0
 Requires-Dist: wrapt
 Requires-Dist: wurlitzer>=3.0
 Provides-Extra: all
-Requires-Dist: orquestra-sdk[ray]; extra == 'all'
+Requires-Dist: async-timeout; extra == 'all'
+Requires-Dist: ray[default]==2.9.0; extra == 'all'
 Provides-Extra: dev
+Requires-Dist: async-timeout; extra == 'dev'
 Requires-Dist: black~=23.7; extra == 'dev'
 Requires-Dist: diff-cover; extra == 'dev'
 Requires-Dist: flake8-pyproject>=1.2.3; extra == 'dev'
 Requires-Dist: flake8>=4.0.0; extra == 'dev'
 Requires-Dist: freezegun; extra == 'dev'
+Requires-Dist: furo==2023.7.26; extra == 'dev'
 Requires-Dist: isort~=5.9.0; extra == 'dev'
+Requires-Dist: jinja2>=3.0.0; extra == 'dev'
 Requires-Dist: mlflow-skinny; extra == 'dev'
 Requires-Dist: mypy~=0.910; extra == 'dev'
 Requires-Dist: numpy; extra == 'dev'
-Requires-Dist: orquestra-sdk[all,docs]; extra == 'dev'
 Requires-Dist: pydoclint; extra == 'dev'
 Requires-Dist: pymarkdownlnt; extra == 'dev'
 Requires-Dist: pyright!=1.1.340,!=1.1.341; extra == 'dev'
 Requires-Dist: pytest-cov>=2.12; extra == 'dev'
 Requires-Dist: pytest-dependency; extra == 'dev'
 Requires-Dist: pytest-httpserver; extra == 'dev'
 Requires-Dist: pytest-timeout>=2.0.0; extra == 'dev'
 Requires-Dist: pytest>=6.2; extra == 'dev'
+Requires-Dist: ray[default]==2.9.0; extra == 'dev'
 Requires-Dist: responses!=0.24,>=0.20; extra == 'dev'
-Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: ruff>=0.2.0; extra == 'dev'
 Requires-Dist: scikit-learn; extra == 'dev'
+Requires-Dist: sphinx-autoapi==2.1.1; extra == 'dev'
+Requires-Dist: sphinx-autobuild==2021.3.14; extra == 'dev'
+Requires-Dist: sphinx-click==4.4.0; extra == 'dev'
+Requires-Dist: sphinx-copybutton==0.5.2; extra == 'dev'
+Requires-Dist: sphinx-design==0.4.1; extra == 'dev'
+Requires-Dist: sphinx-togglebutton==0.3.2; extra == 'dev'
+Requires-Dist: sphinx<7.0,>6.0; extra == 'dev'
+Requires-Dist: sphinxcontrib-autoprogram==0.1.8; extra == 'dev'
+Requires-Dist: sphinxcontrib-youtube==1.2.0; extra == 'dev'
+Requires-Dist: sphinxemoji==0.2.0; extra == 'dev'
 Requires-Dist: types-psutil; extra == 'dev'
 Requires-Dist: types-pygments; extra == 'dev'
 Requires-Dist: types-requests; extra == 'dev'
 Requires-Dist: types-setuptools; extra == 'dev'
 Requires-Dist: types-tabulate; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo==2023.7.26; extra == 'docs'
@@ -307,12 +321,12 @@
 
 ## Usage
 
 Please refer to the [Orquestra Workflow SDK docs](https://docs.orquestra.io/docs/core/sdk/).
 
 ## Bug Reporting
 
-If you'd like to report a bug/issue please create a [new issue using one of the templates](https://github.com/zapatacomputing/orquestra-workflow-sdk/issues).
+If you'd like to report a bug/issue please create a [new issue using one of the templates](https://github.com/zapata-engineering/orquestra-sdk/issues).
 
 ## Contributing
 
 Please see our [CONTRIBUTING.md](CONTRIBUTING.md) for more information on contributing to Orquestra Workflow SDK.
```

## Comparing `orquestra_sdk-0.62.0.dist-info/licenses/LICENSE` & `orquestra_sdk-0.63.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

