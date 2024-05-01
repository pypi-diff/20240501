# Comparing `tmp/subsetter-0.2.0.tar.gz` & `tmp/subsetter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subsetter-0.2.0.tar", last modified: Wed Apr  3 18:39:50 2024, max compression
+gzip compressed data, was "subsetter-0.3.0.tar", last modified: Wed May  1 07:01:45 2024, max compression
```

## Comparing `subsetter-0.2.0.tar` & `subsetter-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-04-03 18:39:50.089532 subsetter-0.2.0/
--rw-rw-r--   0 msg       (1000) msg       (1000)     1493 2023-08-14 00:07:05.000000 subsetter-0.2.0/LICENSE
--rw-r--r--   0 msg       (1000) msg       (1000)     6221 2024-04-03 18:39:50.089532 subsetter-0.2.0/PKG-INFO
--rw-rw-r--   0 msg       (1000) msg       (1000)     5195 2024-03-31 20:57:36.000000 subsetter-0.2.0/README.md
--rw-rw-r--   0 msg       (1000) msg       (1000)     1406 2024-03-25 08:03:09.000000 subsetter-0.2.0/pyproject.toml
--rw-rw-r--   0 msg       (1000) msg       (1000)     1108 2024-04-03 18:39:50.089532 subsetter-0.2.0/setup.cfg
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-04-03 18:39:50.089532 subsetter-0.2.0/subsetter/
--rw-rw-r--   0 msg       (1000) msg       (1000)        0 2023-08-14 00:07:05.000000 subsetter-0.2.0/subsetter/__init__.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    10087 2024-04-03 17:58:11.000000 subsetter-0.2.0/subsetter/__main__.py
--rw-rw-r--   0 msg       (1000) msg       (1000)       22 2024-03-31 21:08:43.000000 subsetter-0.2.0/subsetter/_version.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    13189 2024-03-25 08:26:43.000000 subsetter-0.2.0/subsetter/common.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    20926 2024-03-25 08:26:43.000000 subsetter-0.2.0/subsetter/filters.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    12813 2024-04-03 17:41:00.000000 subsetter-0.2.0/subsetter/metadata.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    14794 2024-04-03 17:45:07.000000 subsetter-0.2.0/subsetter/planner.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    15505 2024-04-03 18:06:20.000000 subsetter-0.2.0/subsetter/sampler.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     4569 2024-03-25 01:41:44.000000 subsetter-0.2.0/subsetter/solver.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     2654 2024-03-25 05:27:01.000000 subsetter-0.2.0/subsetter/sql_dialects.py
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-04-03 18:39:50.089532 subsetter-0.2.0/subsetter.egg-info/
--rw-r--r--   0 msg       (1000) msg       (1000)     6221 2024-04-03 18:39:50.000000 subsetter-0.2.0/subsetter.egg-info/PKG-INFO
--rw-rw-r--   0 msg       (1000) msg       (1000)      508 2024-04-03 18:39:50.000000 subsetter-0.2.0/subsetter.egg-info/SOURCES.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)        1 2024-04-03 18:39:50.000000 subsetter-0.2.0/subsetter.egg-info/dependency_links.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)       54 2024-04-03 18:39:50.000000 subsetter-0.2.0/subsetter.egg-info/entry_points.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)      133 2024-04-03 18:39:50.000000 subsetter-0.2.0/subsetter.egg-info/requires.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)       10 2024-04-03 18:39:50.000000 subsetter-0.2.0/subsetter.egg-info/top_level.txt
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-04-03 18:39:50.089532 subsetter-0.2.0/tests/
--rw-rw-r--   0 msg       (1000) msg       (1000)     7317 2024-03-25 07:55:35.000000 subsetter-0.2.0/tests/test_filters.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     2333 2024-03-25 08:05:34.000000 subsetter-0.2.0/tests/test_planner_live.py
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-01 07:01:45.003337 subsetter-0.3.0/
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1493 2023-08-14 00:07:05.000000 subsetter-0.3.0/LICENSE
+-rw-r--r--   0 msg       (1000) msg       (1000)     5260 2024-05-01 07:01:45.003337 subsetter-0.3.0/PKG-INFO
+-rw-rw-r--   0 msg       (1000) msg       (1000)     4234 2024-04-26 07:16:28.000000 subsetter-0.3.0/README.md
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1406 2024-03-25 08:03:09.000000 subsetter-0.3.0/pyproject.toml
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1108 2024-05-01 07:01:45.003337 subsetter-0.3.0/setup.cfg
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-01 07:01:44.999337 subsetter-0.3.0/subsetter/
+-rw-rw-r--   0 msg       (1000) msg       (1000)        0 2023-08-14 00:07:05.000000 subsetter-0.3.0/subsetter/__init__.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     9844 2024-04-22 04:48:05.000000 subsetter-0.3.0/subsetter/__main__.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)       22 2024-04-23 01:12:27.000000 subsetter-0.3.0/subsetter/_version.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     3543 2024-04-15 04:56:03.000000 subsetter-0.3.0/subsetter/common.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    20926 2024-03-25 08:26:43.000000 subsetter-0.3.0/subsetter/filters.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     9676 2024-04-24 08:31:13.000000 subsetter-0.3.0/subsetter/metadata.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    11194 2024-04-22 04:48:05.000000 subsetter-0.3.0/subsetter/plan_model.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    13820 2024-04-30 04:49:33.000000 subsetter-0.3.0/subsetter/planner.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    21639 2024-04-30 04:49:47.000000 subsetter-0.3.0/subsetter/sampler.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     4859 2024-05-01 06:44:40.000000 subsetter-0.3.0/subsetter/solver.py
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-01 07:01:45.003337 subsetter-0.3.0/subsetter.egg-info/
+-rw-r--r--   0 msg       (1000) msg       (1000)     5260 2024-05-01 07:01:44.000000 subsetter-0.3.0/subsetter.egg-info/PKG-INFO
+-rw-rw-r--   0 msg       (1000) msg       (1000)      519 2024-05-01 07:01:44.000000 subsetter-0.3.0/subsetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)        1 2024-05-01 07:01:44.000000 subsetter-0.3.0/subsetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)       54 2024-05-01 07:01:44.000000 subsetter-0.3.0/subsetter.egg-info/entry_points.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)      133 2024-05-01 07:01:44.000000 subsetter-0.3.0/subsetter.egg-info/requires.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)       10 2024-05-01 07:01:44.000000 subsetter-0.3.0/subsetter.egg-info/top_level.txt
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-05-01 07:01:45.003337 subsetter-0.3.0/tests/
+-rw-rw-r--   0 msg       (1000) msg       (1000)     7317 2024-03-25 07:55:35.000000 subsetter-0.3.0/tests/test_filters.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1686 2024-04-22 04:48:05.000000 subsetter-0.3.0/tests/test_live.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     5203 2024-05-01 06:38:45.000000 subsetter-0.3.0/tests/test_solver.py
```

### Comparing `subsetter-0.2.0/LICENSE` & `subsetter-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `subsetter-0.2.0/PKG-INFO` & `subsetter-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subsetter
-Version: 0.2.0
+Version: 0.3.0
 Summary: MySQL database subsetting CLI tool
 Home-page: http://github.com/msg555/subsetter/
 Author: Mark Gordon
 Author-email: msg555@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -26,112 +26,96 @@
 Requires-Dist: pymysql~=1.0; extra == "mysql"
 Provides-Extra: postgres
 Requires-Dist: psycopg2-binary~=2.0; extra == "postgres"
 
 # Subsetter
 
 Subsetter is a Python utility that can be used for subsetting portions of
-mysql databases. _Subsetting_ is the action extracting a smaller set of rows
+relational databases. _Subsetting_ is the action extracting a smaller set of rows
 from your database that still maintain expected foreign-key relationships
 between your data. This can be useful for testing against a small but
 realistic dataset or for generating sample data for use in demonstrations.
 This tool also supports filtering that allows you to remove/anonymize rows that
 may contain sensitive data.
 
 Similar tools include Tonic.ai's platform and [condenser](https://github.com/TonicAI/condenser).
 This is meant to be a simple CLI tool that overcomes many of the difficulties in
 using `condenser.
 
 ## Limitations
 
-Be aware that subsetting is a hard problem. The planner tool is meant to do a
-bit of "magic" to generate a plan. For some organizations this will entirely
-match their needs, for others this may only be a starting point. For this reason
-the subsetter splits its function into a "planning" phase and a "sampling"
-phase. The output of the planning phase can be examined and modified and fed
-into the sampling phase which is responsible for the mechanics of filtering
-and loading data into the destination.
-
-Additionally the subsetter tool takes an approach of "one table, one query". This
-means that the subsetter will sample each table using a single query that can
-optionally reference some previously sampled rows from other tables. In
-particular, this tool cannot generically sample a transitive closure of foreign
-key relationships if schemas contain relationship cycles that aren't innately
-closed.
+The subsetter tool takes an approach of "one table, one query". This means that
+the subsetter will sample each table using only a single query. It cannot
+support calculating a full transitive closure of foreign key relationships for
+schemas that contain cycles. In general, as long as your schema contains no
+foreign key cycles and no target is reachable from another target, the subsetter
+will be able to automatically generate a plan that can sample your data.
 
 # Usage
 
 ## Create a sampling plan
 
 The first step in subsetting a database is to generate a sampling plan. A
-sampling plan defines the query that will be used to sample each table
-
-is nothing more than an ordered sequence of SQL describing how
-to sample each requested database table. You'll want to create a configuration
-file similar to [planner_config.sample.yaml](planner_config.sample.yaml) that
-tells the planner what tables you want to sample along with any additional
-constraints that should be considered. Then you can create a plan with the
-below command:
+sampling plan defines the queries that will be used to sample each table.
+You'll want to create a configuration file similar to
+[planner_config.example.yaml](planner_config.example.yaml) that tells the
+planner what tables you want to sample along with any additional constraints
+that should be considered. Then you can create a plan with the below command:
 
 ```sh
-python -m subsetter plan -c my-config.yaml > plan.yaml
+subsetter plan -c my-config.yaml > plan.yaml
 ```
 
-If you inspect the generated plan file you will see SQL for each database table.
-Some tables may have a `materialize: true` flag; these are sampled tables that
-need to be referenced by other sampled tables. You may see some queries use a
-placeholder `<SAMPLED>` identifier; this means the query is referencing the
-already sampled data for that table rather than the original source table.
-
-Generally, you can make arbitrary changes to the SQL listed in the plan with the
-constraint that each query can only access the sampling results from
-tables marked as _materialized_ that appear earlier in the plan.
+If you inspect the generated plan YAML document you will see a syntax tree
+that defines how each table will be sampled, potentially referencing other
+tables. Queries can reference either source tables or previously sampled tables.
+If you need to customize the way that tables are sampled beyond what the planner
+can automatically produce this is the place to do it. If needed, you can even
+write direct SQL here.
 
 ## Sample a database with a plan
 
 The sample sub-command will sample rows from the source database into your
 target output (either a database or as json files) using a plan generated
 using the plan sub-command. This tool will **not** copy schema from the source
 database. Any sampled tables must already exist in the destination database.
 Additionally you must pass `--truncate` if you wish to clear any existing data
 in the sampled tables that may interfere with the sampling process.
 
 ```sh
-export SUBSET_DESTINATION_PASSWORD=my-db-password
-python -m subsetter sample --plan my-plan.yaml mysql --host my-db-host --user my-db-user
+subsetter sample --config my-sample-config.yaml --plan my-plan.yaml --truncate
 ```
+
 The sampling process proceeds in three phases:
 
 1. If `--truncate` is specified any tables about to be sampled will be first truncated.
-2. Any _materialized_ tables in the plan will be sampled into temporary tables
-on the source database in the order listed in the plan file.
-3. Data is copied for each table from the source to destination. The ordering
-may differ from the plan file in order to adhere to foreign key constraints.
+2. Any sampled tables that are referenced by other tables will first be
+materialized into temporary tables on the source database.
+3. Data is copied for each table from the source to destination.
 
 The sampler also supports filters which allow you to transform and anonymize your
 data using simple column filters. See
 [sampler_config.sample.yaml](sampler_config.sample.yaml) for more details on what
 filters are available and how to configure them.
 
 ## Plan and sample in one action
 
 There's also a `subset` subcommand to perform the `plan` and `sample` actions
-back-to-back. This will automatically feed the generated plan into the sampler,
+together. This will automatically feed the generated plan into the sampler,
 in addition to ensuring the same source database configuration is used for
 each.
 
 ```sh
-export SUBSET_DESTINATION_PASSWORD=my-db-password
-python -m subsetter subset --plan-config my-config.yaml mysql --host my-db-host --user my-db-user
+subsetter subset --plan-config my-plan-config.yaml --sample-config my-sample-config.yaml
 ```
 
 # Sampling Multiplicity
 
 Sampling usually means condensing a large dataset into a semantically consistent
 small dataset. However, there are times that what you really want to do is
 create a semantically consistent large dataset from your existing data. The
-sampler has support through this by setting the multiplicity factor.
+sampler has support for this by setting the multiplicity factor.
 
 Multiplicity works by creating multiple copies of your sampled dataset in your
 output database. To ensure these datasets do not collide it remaps all foreign
 keys into a new key-space. Note that this process assumes your foreign keys are
 opaque integers identifiers.
```

### Comparing `subsetter-0.2.0/README.md` & `subsetter-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,92 @@
 # Subsetter
 
 Subsetter is a Python utility that can be used for subsetting portions of
-mysql databases. _Subsetting_ is the action extracting a smaller set of rows
+relational databases. _Subsetting_ is the action extracting a smaller set of rows
 from your database that still maintain expected foreign-key relationships
 between your data. This can be useful for testing against a small but
 realistic dataset or for generating sample data for use in demonstrations.
 This tool also supports filtering that allows you to remove/anonymize rows that
 may contain sensitive data.
 
 Similar tools include Tonic.ai's platform and [condenser](https://github.com/TonicAI/condenser).
 This is meant to be a simple CLI tool that overcomes many of the difficulties in
 using `condenser.
 
 ## Limitations
 
-Be aware that subsetting is a hard problem. The planner tool is meant to do a
-bit of "magic" to generate a plan. For some organizations this will entirely
-match their needs, for others this may only be a starting point. For this reason
-the subsetter splits its function into a "planning" phase and a "sampling"
-phase. The output of the planning phase can be examined and modified and fed
-into the sampling phase which is responsible for the mechanics of filtering
-and loading data into the destination.
-
-Additionally the subsetter tool takes an approach of "one table, one query". This
-means that the subsetter will sample each table using a single query that can
-optionally reference some previously sampled rows from other tables. In
-particular, this tool cannot generically sample a transitive closure of foreign
-key relationships if schemas contain relationship cycles that aren't innately
-closed.
+The subsetter tool takes an approach of "one table, one query". This means that
+the subsetter will sample each table using only a single query. It cannot
+support calculating a full transitive closure of foreign key relationships for
+schemas that contain cycles. In general, as long as your schema contains no
+foreign key cycles and no target is reachable from another target, the subsetter
+will be able to automatically generate a plan that can sample your data.
 
 # Usage
 
 ## Create a sampling plan
 
 The first step in subsetting a database is to generate a sampling plan. A
-sampling plan defines the query that will be used to sample each table
-
-is nothing more than an ordered sequence of SQL describing how
-to sample each requested database table. You'll want to create a configuration
-file similar to [planner_config.sample.yaml](planner_config.sample.yaml) that
-tells the planner what tables you want to sample along with any additional
-constraints that should be considered. Then you can create a plan with the
-below command:
+sampling plan defines the queries that will be used to sample each table.
+You'll want to create a configuration file similar to
+[planner_config.example.yaml](planner_config.example.yaml) that tells the
+planner what tables you want to sample along with any additional constraints
+that should be considered. Then you can create a plan with the below command:
 
 ```sh
-python -m subsetter plan -c my-config.yaml > plan.yaml
+subsetter plan -c my-config.yaml > plan.yaml
 ```
 
-If you inspect the generated plan file you will see SQL for each database table.
-Some tables may have a `materialize: true` flag; these are sampled tables that
-need to be referenced by other sampled tables. You may see some queries use a
-placeholder `<SAMPLED>` identifier; this means the query is referencing the
-already sampled data for that table rather than the original source table.
-
-Generally, you can make arbitrary changes to the SQL listed in the plan with the
-constraint that each query can only access the sampling results from
-tables marked as _materialized_ that appear earlier in the plan.
+If you inspect the generated plan YAML document you will see a syntax tree
+that defines how each table will be sampled, potentially referencing other
+tables. Queries can reference either source tables or previously sampled tables.
+If you need to customize the way that tables are sampled beyond what the planner
+can automatically produce this is the place to do it. If needed, you can even
+write direct SQL here.
 
 ## Sample a database with a plan
 
 The sample sub-command will sample rows from the source database into your
 target output (either a database or as json files) using a plan generated
 using the plan sub-command. This tool will **not** copy schema from the source
 database. Any sampled tables must already exist in the destination database.
 Additionally you must pass `--truncate` if you wish to clear any existing data
 in the sampled tables that may interfere with the sampling process.
 
 ```sh
-export SUBSET_DESTINATION_PASSWORD=my-db-password
-python -m subsetter sample --plan my-plan.yaml mysql --host my-db-host --user my-db-user
+subsetter sample --config my-sample-config.yaml --plan my-plan.yaml --truncate
 ```
+
 The sampling process proceeds in three phases:
 
 1. If `--truncate` is specified any tables about to be sampled will be first truncated.
-2. Any _materialized_ tables in the plan will be sampled into temporary tables
-on the source database in the order listed in the plan file.
-3. Data is copied for each table from the source to destination. The ordering
-may differ from the plan file in order to adhere to foreign key constraints.
+2. Any sampled tables that are referenced by other tables will first be
+materialized into temporary tables on the source database.
+3. Data is copied for each table from the source to destination.
 
 The sampler also supports filters which allow you to transform and anonymize your
 data using simple column filters. See
 [sampler_config.sample.yaml](sampler_config.sample.yaml) for more details on what
 filters are available and how to configure them.
 
 ## Plan and sample in one action
 
 There's also a `subset` subcommand to perform the `plan` and `sample` actions
-back-to-back. This will automatically feed the generated plan into the sampler,
+together. This will automatically feed the generated plan into the sampler,
 in addition to ensuring the same source database configuration is used for
 each.
 
 ```sh
-export SUBSET_DESTINATION_PASSWORD=my-db-password
-python -m subsetter subset --plan-config my-config.yaml mysql --host my-db-host --user my-db-user
+subsetter subset --plan-config my-plan-config.yaml --sample-config my-sample-config.yaml
 ```
 
 # Sampling Multiplicity
 
 Sampling usually means condensing a large dataset into a semantically consistent
 small dataset. However, there are times that what you really want to do is
 create a semantically consistent large dataset from your existing data. The
-sampler has support through this by setting the multiplicity factor.
+sampler has support for this by setting the multiplicity factor.
 
 Multiplicity works by creating multiple copies of your sampled dataset in your
 output database. To ensure these datasets do not collide it remaps all foreign
 keys into a new key-space. Note that this process assumes your foreign keys are
 opaque integers identifiers.
```

### Comparing `subsetter-0.2.0/pyproject.toml` & `subsetter-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `subsetter-0.2.0/setup.cfg` & `subsetter-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `subsetter-0.2.0/subsetter/__main__.py` & `subsetter-0.3.0/subsetter/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,21 +45,14 @@
             "-o",
             "--output",
             default=None,
             required=False,
             help="Output path for plan, writes to stdout by default",
             dest="plan_output",
         )
-        parser.add_argument(
-            "--sql",
-            default=False,
-            const=True,
-            action="store_const",
-            help="Write raw SQL queries in plan instead of syntax tree form",
-        )
 
 
 def _add_sample_args(parser, *, subset_action: bool = False):
     if not subset_action:
         parser.add_argument(
             "-p",
             "--plan",
@@ -232,26 +225,26 @@
         )
         sys.exit(1)
 
 
 def _main_plan(args):
     config = _get_plan_config(args)
     config.source = _get_source_database_config(args, overlay=config.source)
-    plan = Planner(config).plan(output_sql=args.sql)
+    plan = Planner(config).plan()
     try:
         ctx = contextlib.nullcontext(sys.stdout)
         if args.plan_output:
             ctx = open(args.plan_output, "w", encoding="utf-8")
         with ctx as fplan:
             yaml.dump(
                 plan.dict(exclude_unset=True, by_alias=True),
                 stream=fplan,
                 default_flow_style=False,
                 width=2**20,
-                sort_keys=False,
+                sort_keys=True,
             )
     except IOError as exc:
         LOGGER.error(
             "Could not write plan to output file %r: %s", args.plan_output, exc
         )
         sys.exit(1)
```

### Comparing `subsetter-0.2.0/subsetter/filters.py` & `subsetter-0.3.0/subsetter/filters.py`

 * *Files identical despite different names*

### Comparing `subsetter-0.2.0/subsetter/metadata.py` & `subsetter-0.3.0/subsetter/metadata.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,245 +1,138 @@
 import collections
 import dataclasses
-import itertools
 import logging
 from fnmatch import fnmatch
-from typing import Any, Dict, List, Optional, Set, TextIO, Tuple
+from typing import Dict, List, Optional, Set, TextIO, Tuple
 
 import sqlalchemy as sa
 
 from subsetter.common import parse_table_name
-from subsetter.solver import reverse_graph
+from subsetter.plan_model import SQLTableIdentifier
+from subsetter.solver import toposort
 
 LOGGER = logging.getLogger(__name__)
 
 # We use lists as queues in a couple places. This is well defined by upsets pylint.
 # pylint: disable=modified-iterating-list
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True, order=True)
 class ForeignKey:
     columns: Tuple[str, ...]
     dst_schema: str
     dst_table: str
     dst_columns: Tuple[str, ...]
 
-
-@dataclasses.dataclass(frozen=True)
-class ColumnDefinition:
-    type_: str
-    default: Any
-    comment: Optional[str]
-    nullable: bool
+    @classmethod
+    def from_schema(cls, fk: sa.ForeignKeyConstraint) -> "ForeignKey":
+        assert fk.referred_table.schema is not None
+        return cls(
+            columns=tuple(col.name for col in fk.columns),
+            dst_schema=fk.referred_table.schema,
+            dst_table=fk.referred_table.name,
+            dst_columns=tuple(elem.column.name for elem in fk.elements),
+        )
 
 
 class TableMetadata:
     def __init__(
         self,
-        *,
-        schema: str,
-        name: str,
-        columns: Dict[str, ColumnDefinition],
-        primary_key: Tuple[str, ...],
-        foreign_keys: List[ForeignKey],
+        table_obj: sa.Table,
     ) -> None:
-        self.schema = schema
-        self.name = name
-        self.columns = columns
-        self.primary_key = primary_key
-        self.foreign_keys = list(foreign_keys)
+        assert table_obj.schema is not None
+        self.table_obj = table_obj
+        self.schema = table_obj.schema
+        self.name = table_obj.name
+        self.primary_key = tuple(
+            column.name for column in table_obj.primary_key.columns
+        )
+        self.foreign_keys = [
+            ForeignKey.from_schema(fk) for fk in table_obj.foreign_key_constraints
+        ]
         self.rev_foreign_keys: List[ForeignKey] = []
 
     def __str__(self) -> str:
         return f"{self.schema}.{self.name}"
 
-    def __repr__(self) -> str:
-        return f"{self.schema}.{self.name}"
-
-
-def _get_fks_mysql(engine: sa.engine.Engine) -> Dict[Tuple[str, str], List[ForeignKey]]:
-    """
-    Optimized query to load all foreign key relationships for a mysql database
-    """
-
-    @dataclasses.dataclass(order=True)
-    class FKConstraint:
-        ordinal_position: int
-        table_schema: str
-        table_name: str
-        column_name: str
-        dst_table_schema: str
-        dst_table_name: str
-        dst_column_name: str
-
-    fk_constraints: Dict[Tuple[str, str], List[FKConstraint]] = collections.defaultdict(
-        list
-    )
-    with engine.connect() as conn:
-        result = conn.execute(
-            sa.text(
-                "SELECT constraint_schema, constraint_name, ordinal_position, "
-                "table_schema, table_name, column_name, "
-                "referenced_table_schema, referenced_table_name, referenced_column_name "
-                "FROM information_schema.key_column_usage WHERE referenced_table_name is not NULL"
-            )
-        )
-        for row in result:
-            constraint_schema = row[0]
-            constraint_name = row[1]
-            fk_constraints[(constraint_schema, constraint_name)].append(
-                FKConstraint(*row[2:9])
-            )
-
-    all_fks: Dict[Tuple[str, str], List[ForeignKey]] = collections.defaultdict(list)
-    for cnst_list in fk_constraints.values():
-        cnst_list.sort()
-
-        # Assert that ordinal positions make sense
-        assert all(
-            cnst.ordinal_position == ind + 1 for ind, cnst in enumerate(cnst_list)
-        )
-
-        src_schema = cnst_list[0].table_schema
-        src_table = cnst_list[0].table_name
-        dst_schema = cnst_list[0].dst_table_schema
-        dst_table = cnst_list[0].dst_table_name
-
-        # Assert that all constraints refer to the same pair of tables
-        assert all(
-            (
-                cnst.table_schema,
-                cnst.table_name,
-                cnst.dst_table_schema,
-                cnst.dst_table_name,
-            )
-            == (src_schema, src_table, dst_schema, dst_table)
-            for cnst in cnst_list
-        )
-
-        all_fks[(src_schema, src_table)].append(
-            ForeignKey(
-                columns=tuple(cnst.column_name for cnst in cnst_list),
-                dst_schema=dst_schema,
-                dst_table=dst_table,
-                dst_columns=tuple(cnst.dst_column_name for cnst in cnst_list),
-            )
-        )
-
-    return all_fks
-
-
-def _get_fks_generic(
-    engine: sa.engine.Engine,
-) -> Dict[Tuple[str, str], List[ForeignKey]]:
-    """
-    Generic implementation to load all foreign key relationships using the
-    SQLAlchemy inspector interface.
-    """
-    result = {}
-
-    inspector = sa.inspect(engine)
-    for schema in inspector.get_schema_names():
-        for table_key, table_fks in inspector.get_multi_foreign_keys(schema).items():
-            result[(table_key[0] or schema, table_key[1])] = [
-                ForeignKey(
-                    columns=tuple(key["constrained_columns"]),
-                    dst_schema=key["referred_schema"] or schema,
-                    dst_table=key["referred_table"],
-                    dst_columns=tuple(key["referred_columns"]),
-                )
-                for key in table_fks
-            ]
-
-    return result
-
-
-def _get_fks(engine: sa.engine.Engine) -> Dict[Tuple[str, str], List[ForeignKey]]:
-    if engine.name == "mysql":
-        return _get_fks_mysql(engine)
-    return _get_fks_generic(engine)
-
 
 class DatabaseMetadata:
-    def __init__(self) -> None:
-        self.tables: Dict[Tuple[str, str], TableMetadata] = {}
+    def __init__(
+        self,
+        metadata_obj: sa.MetaData,
+        tables: Dict[Tuple[str, str], TableMetadata],
+        *,
+        supports_temp_reopen: bool = True,
+    ) -> None:
+        self.metadata_obj = metadata_obj
+        self.tables = tables
+        self.supports_temp_reopen = supports_temp_reopen
+        self.temp_tables: Dict[Tuple[str, str, int], sa.Table] = {}
 
     @classmethod
     def from_engine(
         cls,
         engine,
         select: List[str],
         *,
         close_forward=False,
         close_backward=False,
     ) -> Tuple["DatabaseMetadata", List[Tuple[str, str]]]:
-        all_fks = _get_fks(engine)
-        all_rev_fks = collections.defaultdict(list)
-        for (schema, table_name), foreign_keys in all_fks.items():
-            for foreign_key in foreign_keys:
-                all_rev_fks[(foreign_key.dst_schema, foreign_key.dst_table)].append(
-                    ForeignKey(
-                        columns=foreign_key.dst_columns,
-                        dst_schema=schema,
-                        dst_table=table_name,
-                        dst_columns=foreign_key.columns,
-                    )
-                )
 
-        meta = cls()
         inspector = sa.inspect(engine)
-
-        table_queue = []
-        table_set = set()
+        metadata_obj = sa.MetaData()
         for schema in inspector.get_schema_names():
-            for table_name in inspector.get_table_names(schema=schema):
-                if not any(
-                    fnmatch(f"{schema}.{table_name}", select_pattern)
-                    for select_pattern in select
-                ):
-                    continue
-                table_set.add((schema, table_name))
-                table_queue.append((schema, table_name))
-        num_selected_tables = len(table_queue)
+            metadata_obj.reflect(bind=engine, schema=schema)
 
-        for schema, table_name in table_queue:
-            # TODO: Consider using inspector.get_multi_columns
-            # TODO: Consider using inspector.get_multi_pk_constraint
-            col_specs = inspector.get_columns(table_name, schema=schema)
-            table = TableMetadata(
-                schema=schema,
-                name=table_name,
-                columns={
-                    column["name"]: ColumnDefinition(
-                        type_=column["type"],
-                        default=column["default"],
-                        comment=column["comment"],
-                        nullable=column["nullable"],
-                    )
-                    for column in col_specs
-                },
-                primary_key=tuple(
-                    inspector.get_pk_constraint(table_name, schema=schema).get(
-                        "constrained_columns", []
-                    )
-                ),
-                foreign_keys=all_fks[(schema, table_name)],
-            )
-
-            for foreign_key in itertools.chain(
-                all_fks[(table.schema, table.name)] if close_forward else (),
-                all_rev_fks[(table.schema, table.name)] if close_backward else (),
-            ):
-                if (foreign_key.dst_schema, foreign_key.dst_table) not in table_set:
-                    table_set.add((foreign_key.dst_schema, foreign_key.dst_table))
-                    table_queue.append((foreign_key.dst_schema, foreign_key.dst_table))
+        table_set: Set[Tuple[str, str]] = set()
+        table_queue: List[Tuple[str, str]] = []
+        for table_id, table_obj in metadata_obj.tables.items():
+            assert table_obj.schema is not None
+            if any(fnmatch(table_id, select_pattern) for select_pattern in select):
+                table_set.add((table_obj.schema, table_obj.name))
+                table_queue.append((table_obj.schema, table_obj.name))
 
-            meta.tables[(schema, table_name)] = table
+        table_deps: Dict[Tuple[str, str], List[Tuple[str, str]]] = (
+            collections.defaultdict(list)
+        )
+        for table_obj in metadata_obj.tables.values():
+            assert table_obj.schema is not None
+            for fk in table_obj.foreign_key_constraints:
+                ref_table_obj = fk.referred_table
+                assert ref_table_obj.schema is not None
+                if close_forward:
+                    table_deps[(table_obj.schema, table_obj.name)].append(
+                        (ref_table_obj.schema, ref_table_obj.name)
+                    )
+                if close_backward:
+                    table_deps[(ref_table_obj.schema, ref_table_obj.name)].append(
+                        (table_obj.schema, table_obj.name)
+                    )
 
-        return meta, table_queue[num_selected_tables:]
+        num_selected_tables = len(table_queue)
+        for schema, table in table_queue:
+            table_obj = metadata_obj.tables[f"{schema}.{table}"]
+            for ref_schema, ref_table in table_deps[(schema, table)]:
+                if (ref_schema, ref_table) not in table_set:
+                    table_set.add((ref_schema, ref_table))
+                    table_queue.append((ref_schema, ref_table))
+
+        return (
+            cls(
+                metadata_obj,
+                {
+                    (schema, table): TableMetadata(
+                        metadata_obj.tables[f"{schema}.{table}"]
+                    )
+                    for schema, table in table_queue
+                },
+                supports_temp_reopen=engine.dialect.name != "mysql",
+            ),
+            table_queue[num_selected_tables:],
+        )
 
     def infer_missing_foreign_keys(self) -> None:
         pk_map: Dict[Tuple[str, Tuple[str, ...]], Optional[TableMetadata]] = {}
         for table in self.tables.values():
             if not table.primary_key:
                 continue
             if table.primary_key in pk_map:
@@ -247,22 +140,22 @@
                 pk_map[(table.schema, table.primary_key)] = None
             else:
                 pk_map[(table.schema, table.primary_key)] = table
 
         # Only infer single column primary keys
         for table in self.tables.values():
             fks = set(table.foreign_keys)
-            for col in table.columns:
-                dst_table = pk_map.get((table.schema, (col,)))
+            for col in table.table_obj.columns:
+                dst_table = pk_map.get((table.schema, (col.name,)))
                 if dst_table is not None and dst_table is not table:
                     fk = ForeignKey(
-                        columns=(col,),
+                        columns=(col.name,),
                         dst_schema=dst_table.schema,
                         dst_table=dst_table.name,
-                        dst_columns=(col,),
+                        dst_columns=(col.name,),
                     )
                     if fk not in fks:
                         LOGGER.info(
                             "Inferring foreign key %s->%s on %r",
                             table,
                             dst_table,
                             fk.columns,
@@ -297,32 +190,17 @@
                         fk.dst_schema,
                         fk.dst_table,
                         fk.columns,
                     )
             table.foreign_keys = fk_out
 
     def toposort(self) -> List[TableMetadata]:
-        graph = self.as_graph()
-        graph_rev = reverse_graph(graph)
-        deg = {u: set(edges) for u, edges in graph.items()}
-        order = []
-
-        for u, edges in deg.items():
-            if not edges:
-                order.append(u)
-
-        for u in order:
-            for v in graph_rev[u]:
-                deg[v].discard(u)
-                if not deg[v]:
-                    order.append(v)
-
-        if len(order) < len(graph):
-            raise ValueError("Cycle detected in schema graph")
-        return [self.tables[parse_table_name(u)] for u in order]
+        return [  # type: ignore
+            self.tables[parse_table_name(u)] for u in toposort(self.as_graph())
+        ]
 
     def compute_reverse_keys(self) -> None:
         for table in self.tables.values():
             for fk in table.foreign_keys:
                 self.tables[(fk.dst_schema, fk.dst_table)].rev_foreign_keys.append(
                     ForeignKey(
                         columns=fk.dst_columns,
@@ -330,28 +208,45 @@
                         dst_table=table.name,
                         dst_columns=fk.columns,
                     )
                 )
 
     def as_graph(
         self, *, ignore_tables: Optional[Set[Tuple[str, str]]] = None
-    ) -> Dict[str, List[str]]:
+    ) -> Dict[str, Set[str]]:
         if ignore_tables is None:
             ignore_tables = set()
         return {
-            f"{table.schema}.{table.name}": [
+            f"{table.schema}.{table.name}": {
                 f"{fk.dst_schema}.{fk.dst_table}"
                 for fk in table.foreign_keys
                 if (fk.dst_schema, fk.dst_table) not in ignore_tables
                 and (fk.dst_schema, fk.dst_table) in self.tables
-            ]
+            }
             for table in self.tables.values()
             if (table.schema, table.name) not in ignore_tables
         }
 
+    def sql_build_context(self):
+        reference_count = {}
+
+        def _context(ident: SQLTableIdentifier) -> sa.Table:
+            if ident.sampled:
+                if self.supports_temp_reopen:
+                    index = 0
+                else:
+                    index = reference_count.get(
+                        (ident.table_schema, ident.table_name), 0
+                    )
+                    reference_count[(ident.table_schema, ident.table_name)] = index + 1
+                return self.temp_tables[(ident.table_schema, ident.table_name, index)]
+            return self.tables[(ident.table_schema, ident.table_name)].table_obj
+
+        return _context
+
     def output_graphviz(self, fout: TextIO) -> None:
         def _dot_label(lbl: TableMetadata) -> str:
             return f'"{str(lbl)}"'
 
         fout.write("digraph {\n")
         for table in self.tables.values():
             fout.write("  ")
```

### Comparing `subsetter-0.2.0/subsetter/planner.py` & `subsetter-0.3.0/subsetter/planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import logging
-import os
-from typing import Any, Dict, List, Optional, Set, Tuple, Union
+from typing import Dict, List, Optional, Set, Tuple, Union
 
 from pydantic import BaseModel, Field
 
-from subsetter.common import (
-    DEFAULT_DIALECT,
-    DatabaseConfig,
+from subsetter.common import DatabaseConfig, parse_table_name
+from subsetter.metadata import DatabaseMetadata, ForeignKey, TableMetadata
+from subsetter.plan_model import (
     SQLKnownOperator,
     SQLLiteralType,
     SQLStatementSelect,
     SQLStatementUnion,
     SQLTableIdentifier,
     SQLTableQuery,
     SQLWhereClause,
     SQLWhereClauseAnd,
+    SQLWhereClauseIn,
     SQLWhereClauseOperator,
     SQLWhereClauseOr,
     SQLWhereClauseRandom,
     SQLWhereClauseSQL,
-    parse_table_name,
+    SubsetPlan,
 )
-from subsetter.metadata import DatabaseMetadata, ForeignKey, TableMetadata
-from subsetter.solver import dfs, order_graph, reverse_graph, subgraph
-from subsetter.sql_dialects import SQLDialectEncoder
+from subsetter.solver import order_graph
 
 LOGGER = logging.getLogger(__name__)
 
 
 class PlannerConfig(BaseModel):
     class TargetConfig(BaseModel):
         all_: bool = Field(False, alias="all")
@@ -58,37 +56,27 @@
     targets: Dict[str, TargetConfig]
     ignore: List[str] = []
     passthrough: List[str] = []
     ignore_fks: List[IgnoreFKConfig] = []
     extra_fks: List[ExtraFKConfig] = []
     infer_foreign_keys: bool = False
     normalize_foreign_keys: bool = False
-    output_sql: bool = False
-
-
-class SubsetPlan(BaseModel):
-    queries: Dict[str, SQLTableQuery]
 
 
 class Planner:
     def __init__(self, config: PlannerConfig) -> None:
         self.config = config
         self.engine = self.config.source.database_engine(env_prefix="SUBSET_SOURCE_")
-        self.sql_enc = SQLDialectEncoder.from_dialect(
-            self.config.source.dialect
-            or os.getenv("SUBSET_SOURCE_DIALECT", "")  # type: ignore
-            or DEFAULT_DIALECT
-        )
         self.meta: DatabaseMetadata
         self.ignore_tables = {parse_table_name(table) for table in config.ignore}
         self.passthrough_tables = {
             parse_table_name(table) for table in config.passthrough
         }
 
-    def plan(self, output_sql: bool = False) -> SubsetPlan:
+    def plan(self) -> SubsetPlan:
         LOGGER.info("Scanning schema")
         meta, extra_tables = DatabaseMetadata.from_engine(
             self.engine,
             self.config.select,
             close_forward=True,
         )
         self.meta = meta
@@ -125,60 +113,45 @@
                         table_schema=schema,
                         table_name=table_name,
                     ),
                 )
             )
 
         processed = set()
-        remaining = {parse_table_name(table) for table in order}
         for table in order:
             schema, table_name = parse_table_name(table)
             processed.add((schema, table_name))
-            remaining.remove((schema, table_name))
             queries[table] = self._plan_table(
                 self.meta.tables[(schema, table_name)],
                 processed,
-                remaining,
                 target=self.config.targets.get(table),
             )
 
-        if output_sql:
-            for table, query in queries.items():
-                if not query.statement:
-                    continue
-                sql_params: Dict[str, Any] = {}
-                queries[table] = SQLTableQuery(
-                    sql=query.statement.build(self.sql_enc, sql_params),
-                    sql_params=sql_params,
-                    materialize=query.materialize,
-                )
-
         return SubsetPlan(queries=queries)
 
     def _solve_order(self) -> List[str]:
         """
         Attempts to compute an ordering of non-passthrough, non-ignored tables
         satisfies all constraints.
         """
         source = ""
         graph = self.meta.as_graph(
             ignore_tables=self.passthrough_tables | self.ignore_tables
         )
-        graph[source] = list(self.config.targets)
+        graph[source] = set(self.config.targets)
+        order = order_graph(graph, source)[1:]
 
-        visited: Dict[str, int] = {}
-        dfs(reverse_graph(graph, union=True), source, visited=visited)
-        for u in graph:
-            if u not in visited:
+        order_st = set(order)
+        for table in graph:
+            if table and table not in order_st:
                 LOGGER.warning(
-                    "warning: no relationship found to %s, ignoring table", u
+                    "warning: no relationship found to %s, ignoring table", table
                 )
-        graph = subgraph(graph, set(visited))
 
-        return order_graph(graph, source)
+        return order
 
     def _add_extra_fks(self) -> None:
         """Add in additional foreign keys requested."""
         for extra_fk in self.config.extra_fks:
             src_schema, src_table_name = parse_table_name(extra_fk.src_table)
             dst_schema, dst_table_name = parse_table_name(extra_fk.dst_table)
             table = self.meta.tables.get((src_schema, src_table_name))
@@ -267,60 +240,78 @@
 
         self.passthrough_tables -= not_found_tables
 
     def _plan_table(
         self,
         table: TableMetadata,
         processed: Set[Tuple[str, str]],
-        remaining: Set[Tuple[str, str]],
         target: Optional[PlannerConfig.TargetConfig] = None,
     ) -> SQLTableQuery:
-        materialize = False
         fk_constraints: List[SQLWhereClause] = []
-        for fk in table.foreign_keys + table.rev_foreign_keys:
-            dst_key = (fk.dst_schema, fk.dst_table)
-            if dst_key not in processed:
-                if dst_key in remaining:
-                    dst_target = self.config.targets.get(
-                        f"{fk.dst_schema}.{fk.dst_table}"
-                    )
-                    if not dst_target or not dst_target.all_:
-                        materialize = True
-                continue
 
-            if not target or not target.all_:
-                fk_constraints.append(
-                    SQLWhereClauseOperator(
-                        type_="operator",
-                        operator="in",
-                        columns=list(fk.columns),
-                        values=SQLStatementSelect(
-                            type_="select",
-                            columns=list(fk.dst_columns),
-                            from_=SQLTableIdentifier(
-                                table_schema=fk.dst_schema,
-                                table_name=fk.dst_table,
-                                sampled=True,
-                            ),
-                        ),
-                    )
-                )
+        foreign_keys = sorted(
+            fk
+            for fk in table.foreign_keys
+            if (fk.dst_schema, fk.dst_table) in processed
+        )
+        rev_foreign_keys = sorted(
+            fk
+            for fk in table.rev_foreign_keys
+            if (fk.dst_schema, fk.dst_table) in processed
+        )
+
+        # Make sure the solver gave us something reasonable
+        assert not foreign_keys or not rev_foreign_keys
+        if target:
+            assert not foreign_keys
+            if target.all_:
+                rev_foreign_keys.clear()
+
+        fk_constraints = [
+            SQLWhereClauseIn(
+                type_="in",
+                columns=list(fk.columns),
+                values=SQLStatementSelect(
+                    type_="select",
+                    columns=list(fk.dst_columns),
+                    from_=SQLTableIdentifier(
+                        table_schema=fk.dst_schema,
+                        table_name=fk.dst_table,
+                        sampled=True,
+                    ),
+                ),
+            )
+            for fk in foreign_keys or rev_foreign_keys
+        ]
+
+        fk_constraint: SQLWhereClause
+        if foreign_keys:
+            fk_constraint = SQLWhereClauseAnd(
+                type_="and",
+                conditions=fk_constraints,
+            )
+        else:
+            fk_constraint = SQLWhereClauseOr(
+                type_="or",
+                conditions=fk_constraints,
+            )
 
         conf_constraints = self.config.table_constraints.get(
             f"{table.schema}.{table.name}", []
         )
         conf_constraints_sql: List[SQLWhereClause] = []
+        all_columns = {column.name for column in table.table_obj.columns}
         for conf_constraint in conf_constraints:
-            if conf_constraint.column in table.columns:
+            if conf_constraint.column in all_columns:
                 conf_constraints_sql.append(
                     SQLWhereClauseOperator(
                         type_="operator",
                         operator=conf_constraint.operator,
-                        columns=[conf_constraint.column],
-                        values=conf_constraint.value,
+                        column=conf_constraint.column,
+                        value=conf_constraint.value,
                     )
                 )
 
         # Calculate initial foreign-key / config constraint statement
         statements: List[SQLStatementSelect] = [
             SQLStatementSelect(
                 type_="select",
@@ -328,18 +319,15 @@
                     table_schema=table.schema,
                     table_name=table.name,
                 ),
                 where=SQLWhereClauseAnd(
                     type_="and",
                     conditions=[
                         *conf_constraints_sql,
-                        SQLWhereClauseOr(
-                            type_="or",
-                            conditions=fk_constraints,
-                        ),
+                        fk_constraint,
                     ],
                 ),
             )
         ]
 
         # If targetted also calculate target constraint statement
         if target:
@@ -363,29 +351,28 @@
                 target_constraints.append(
                     SQLWhereClauseOr(
                         type_="or",
                         conditions=[
                             SQLWhereClauseOperator(
                                 type_="operator",
                                 operator="like",
-                                columns=[column],
-                                values=pattern,
+                                column=column,
+                                value=pattern,
                             )
                             for pattern in patterns
                         ],
                     )
                 )
 
             for column, in_list in target.in_.items():
                 target_constraints.append(
-                    SQLWhereClauseOperator(
-                        type_="operator",
-                        operator="in",
+                    SQLWhereClauseIn(
+                        type_="in",
                         columns=[column],
-                        values=in_list,
+                        values=[in_list],
                     )
                 )
 
             if target.all_:
                 target_constraints.clear()
 
             statements.append(
@@ -400,10 +387,9 @@
                 )
             )
 
         return SQLTableQuery(
             statement=SQLStatementUnion(
                 type_="union",
                 statements=statements,
-            ).simplify(),
-            materialize=materialize,
+            ).simplify()
         )
```

### Comparing `subsetter-0.2.0/subsetter.egg-info/PKG-INFO` & `subsetter-0.3.0/subsetter.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subsetter
-Version: 0.2.0
+Version: 0.3.0
 Summary: MySQL database subsetting CLI tool
 Home-page: http://github.com/msg555/subsetter/
 Author: Mark Gordon
 Author-email: msg555@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -26,112 +26,96 @@
 Requires-Dist: pymysql~=1.0; extra == "mysql"
 Provides-Extra: postgres
 Requires-Dist: psycopg2-binary~=2.0; extra == "postgres"
 
 # Subsetter
 
 Subsetter is a Python utility that can be used for subsetting portions of
-mysql databases. _Subsetting_ is the action extracting a smaller set of rows
+relational databases. _Subsetting_ is the action extracting a smaller set of rows
 from your database that still maintain expected foreign-key relationships
 between your data. This can be useful for testing against a small but
 realistic dataset or for generating sample data for use in demonstrations.
 This tool also supports filtering that allows you to remove/anonymize rows that
 may contain sensitive data.
 
 Similar tools include Tonic.ai's platform and [condenser](https://github.com/TonicAI/condenser).
 This is meant to be a simple CLI tool that overcomes many of the difficulties in
 using `condenser.
 
 ## Limitations
 
-Be aware that subsetting is a hard problem. The planner tool is meant to do a
-bit of "magic" to generate a plan. For some organizations this will entirely
-match their needs, for others this may only be a starting point. For this reason
-the subsetter splits its function into a "planning" phase and a "sampling"
-phase. The output of the planning phase can be examined and modified and fed
-into the sampling phase which is responsible for the mechanics of filtering
-and loading data into the destination.
-
-Additionally the subsetter tool takes an approach of "one table, one query". This
-means that the subsetter will sample each table using a single query that can
-optionally reference some previously sampled rows from other tables. In
-particular, this tool cannot generically sample a transitive closure of foreign
-key relationships if schemas contain relationship cycles that aren't innately
-closed.
+The subsetter tool takes an approach of "one table, one query". This means that
+the subsetter will sample each table using only a single query. It cannot
+support calculating a full transitive closure of foreign key relationships for
+schemas that contain cycles. In general, as long as your schema contains no
+foreign key cycles and no target is reachable from another target, the subsetter
+will be able to automatically generate a plan that can sample your data.
 
 # Usage
 
 ## Create a sampling plan
 
 The first step in subsetting a database is to generate a sampling plan. A
-sampling plan defines the query that will be used to sample each table
-
-is nothing more than an ordered sequence of SQL describing how
-to sample each requested database table. You'll want to create a configuration
-file similar to [planner_config.sample.yaml](planner_config.sample.yaml) that
-tells the planner what tables you want to sample along with any additional
-constraints that should be considered. Then you can create a plan with the
-below command:
+sampling plan defines the queries that will be used to sample each table.
+You'll want to create a configuration file similar to
+[planner_config.example.yaml](planner_config.example.yaml) that tells the
+planner what tables you want to sample along with any additional constraints
+that should be considered. Then you can create a plan with the below command:
 
 ```sh
-python -m subsetter plan -c my-config.yaml > plan.yaml
+subsetter plan -c my-config.yaml > plan.yaml
 ```
 
-If you inspect the generated plan file you will see SQL for each database table.
-Some tables may have a `materialize: true` flag; these are sampled tables that
-need to be referenced by other sampled tables. You may see some queries use a
-placeholder `<SAMPLED>` identifier; this means the query is referencing the
-already sampled data for that table rather than the original source table.
-
-Generally, you can make arbitrary changes to the SQL listed in the plan with the
-constraint that each query can only access the sampling results from
-tables marked as _materialized_ that appear earlier in the plan.
+If you inspect the generated plan YAML document you will see a syntax tree
+that defines how each table will be sampled, potentially referencing other
+tables. Queries can reference either source tables or previously sampled tables.
+If you need to customize the way that tables are sampled beyond what the planner
+can automatically produce this is the place to do it. If needed, you can even
+write direct SQL here.
 
 ## Sample a database with a plan
 
 The sample sub-command will sample rows from the source database into your
 target output (either a database or as json files) using a plan generated
 using the plan sub-command. This tool will **not** copy schema from the source
 database. Any sampled tables must already exist in the destination database.
 Additionally you must pass `--truncate` if you wish to clear any existing data
 in the sampled tables that may interfere with the sampling process.
 
 ```sh
-export SUBSET_DESTINATION_PASSWORD=my-db-password
-python -m subsetter sample --plan my-plan.yaml mysql --host my-db-host --user my-db-user
+subsetter sample --config my-sample-config.yaml --plan my-plan.yaml --truncate
 ```
+
 The sampling process proceeds in three phases:
 
 1. If `--truncate` is specified any tables about to be sampled will be first truncated.
-2. Any _materialized_ tables in the plan will be sampled into temporary tables
-on the source database in the order listed in the plan file.
-3. Data is copied for each table from the source to destination. The ordering
-may differ from the plan file in order to adhere to foreign key constraints.
+2. Any sampled tables that are referenced by other tables will first be
+materialized into temporary tables on the source database.
+3. Data is copied for each table from the source to destination.
 
 The sampler also supports filters which allow you to transform and anonymize your
 data using simple column filters. See
 [sampler_config.sample.yaml](sampler_config.sample.yaml) for more details on what
 filters are available and how to configure them.
 
 ## Plan and sample in one action
 
 There's also a `subset` subcommand to perform the `plan` and `sample` actions
-back-to-back. This will automatically feed the generated plan into the sampler,
+together. This will automatically feed the generated plan into the sampler,
 in addition to ensuring the same source database configuration is used for
 each.
 
 ```sh
-export SUBSET_DESTINATION_PASSWORD=my-db-password
-python -m subsetter subset --plan-config my-config.yaml mysql --host my-db-host --user my-db-user
+subsetter subset --plan-config my-plan-config.yaml --sample-config my-sample-config.yaml
 ```
 
 # Sampling Multiplicity
 
 Sampling usually means condensing a large dataset into a semantically consistent
 small dataset. However, there are times that what you really want to do is
 create a semantically consistent large dataset from your existing data. The
-sampler has support through this by setting the multiplicity factor.
+sampler has support for this by setting the multiplicity factor.
 
 Multiplicity works by creating multiple copies of your sampled dataset in your
 output database. To ensure these datasets do not collide it remaps all foreign
 keys into a new key-space. Note that this process assumes your foreign keys are
 opaque integers identifiers.
```

### Comparing `subsetter-0.2.0/tests/test_filters.py` & `subsetter-0.3.0/tests/test_filters.py`

 * *Files identical despite different names*

