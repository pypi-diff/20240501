# Comparing `tmp/pulumi_materialize-0.2.0.tar.gz` & `tmp/pulumi_materialize-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_materialize-0.2.0.tar", last modified: Thu Apr 25 15:05:38 2024, max compression
+gzip compressed data, was "pulumi_materialize-0.2.1.tar", last modified: Wed May  1 15:55:28 2024, max compression
```

## Comparing `pulumi_materialize-0.2.0.tar` & `pulumi_materialize-0.2.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:05:38.318382 pulumi_materialize-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-25 15:05:38.318382 pulumi_materialize-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:05:38.314382 pulumi_materialize-0.2.0/pulumi_materialize/
--rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   215981 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/app_password.py
--rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/cloud_region.py
--rw-r--r--   0 runner    (1001) docker     (127)    31153 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    26842 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/cluster_replica.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:05:38.314382 pulumi_materialize-0.2.0/pulumi_materialize/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    38924 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    27833 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)    46174 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_confluent_schema_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    54306 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    47019 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)    49006 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    28437 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/connection_ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_cluster_replicas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_current_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_current_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_egress_ips.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_materialized_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_scim_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_scim_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_sinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_sso_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_system_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/get_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    15563 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_cluster_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17766 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20573 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_connection_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_database_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    18429 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    18124 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_schema_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17366 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    20461 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_secret_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17346 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_system_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17558 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    20743 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_table_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    20405 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_type_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    16984 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/grant_view.py
--rw-r--r--   0 runner    (1001) docker     (127)    24878 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    28616 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (127)   247075 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/region.py
--rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/role_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16381 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    15515 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/scim2_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/scim2_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/scim2_group_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9640 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/scim2_group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    21139 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    44082 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/sink_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    68779 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/source_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    41574 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/source_loadgen.py
--rw-r--r--   0 runner    (1001) docker     (127)    36122 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/source_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)    41674 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/source_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    37565 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/source_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    24196 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/sso_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/sso_default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/sso_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/sso_role_group_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/system_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    27574 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:05:38.314382 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/pulumi_materialize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:05:38.318382 pulumi_materialize-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-25 15:05:38.000000 pulumi_materialize-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:55:28.732998 pulumi_materialize-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-01 15:55:28.732998 pulumi_materialize-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:55:28.728999 pulumi_materialize-0.2.1/pulumi_materialize/
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   215981 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/app_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/cloud_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31143 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26832 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/cluster_replica.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:55:28.732998 pulumi_materialize-0.2.1/pulumi_materialize/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38914 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27823 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46164 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_confluent_schema_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54296 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47009 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48996 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28427 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_cluster_replicas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_current_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_current_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_egress_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_materialized_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_scim_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_scim_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_sso_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_system_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_cluster_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17756 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20563 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_connection_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13270 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_database_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18419 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18114 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_schema_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20451 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_secret_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17336 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_system_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17548 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20733 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_table_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17156 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_type_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16974 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24868 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28606 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)   247075 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12773 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/role_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15515 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/scim2_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/scim2_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/scim2_group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9640 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/scim2_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21129 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44072 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/sink_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68769 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/source_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41564 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/source_loadgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36112 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/source_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41664 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/source_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37555 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/source_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24196 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/sso_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/sso_default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/sso_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/sso_role_group_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/system_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22074 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27564 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:55:28.732998 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:55:28.732998 pulumi_materialize-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/setup.py
```

### Comparing `pulumi_materialize-0.2.0/PKG-INFO` & `pulumi_materialize-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_materialize
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Pulumi package for creating and managing materialize cloud resources.
 Home-page: https://github.com/MaterializeInc/terraform-provider-materialize
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaterializeInc/terraform-provider-materialize
 Keywords: pulumi materialize category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_materialize-0.2.0/README.md` & `pulumi_materialize-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/__init__.py` & `pulumi_materialize-0.2.1/pulumi_materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/_inputs.py` & `pulumi_materialize-0.2.1/pulumi_materialize/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/_utilities.py` & `pulumi_materialize-0.2.1/pulumi_materialize/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/app_password.py` & `pulumi_materialize-0.2.1/pulumi_materialize/app_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/cloud_region.py` & `pulumi_materialize-0.2.1/pulumi_materialize/cloud_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/cluster.py` & `pulumi_materialize-0.2.1/pulumi_materialize/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,15 +637,15 @@
         """
         The owernship role of the object.
         """
         return pulumi.get(self, "ownership_role")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="replicationFactor")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/cluster_replica.py` & `pulumi_materialize-0.2.1/pulumi_materialize/cluster_replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -567,15 +567,15 @@
         """
         The identifier for the replica.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/config/vars.py` & `pulumi_materialize-0.2.1/pulumi_materialize/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/connection_aws.py` & `pulumi_materialize-0.2.1/pulumi_materialize/connection_aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -788,15 +788,15 @@
         """
         The fully qualified name of the connection.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/connection_aws_privatelink.py` & `pulumi_materialize-0.2.1/pulumi_materialize/connection_aws_privatelink.py`

 * *Files 0% similar despite different names*

```diff
@@ -601,15 +601,15 @@
         """
         The fully qualified name of the connection.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/connection_confluent_schema_registry.py` & `pulumi_materialize-0.2.1/pulumi_materialize/connection_confluent_schema_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -816,15 +816,15 @@
         """
         The fully qualified name of the connection.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/connection_kafka.py` & `pulumi_materialize-0.2.1/pulumi_materialize/connection_kafka.py`

 * *Files 0% similar despite different names*

```diff
@@ -992,15 +992,15 @@
         """
         The fully qualified name of the connection.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="saslMechanisms")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/connection_mysql.py` & `pulumi_materialize-0.2.1/pulumi_materialize/connection_mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -919,15 +919,15 @@
         """
         The fully qualified name of the connection.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/connection_postgres.py` & `pulumi_materialize-0.2.1/pulumi_materialize/connection_postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -969,15 +969,15 @@
         """
         The fully qualified name of the connection.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/connection_ssh_tunnel.py` & `pulumi_materialize-0.2.1/pulumi_materialize/connection_ssh_tunnel.py`

 * *Files 0% similar despite different names*

```diff
@@ -667,15 +667,15 @@
         """
         The fully qualified name of the connection.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/database.py` & `pulumi_materialize-0.2.1/pulumi_materialize/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,13 +340,13 @@
         """
         The owernship role of the object.
         """
         return pulumi.get(self, "ownership_role")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_cluster_replicas.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_cluster_replicas.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_clusters.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_clusters.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_connections.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_materialized_views.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,150 +7,150 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
-    'GetConnectionsResult',
-    'AwaitableGetConnectionsResult',
-    'get_connections',
-    'get_connections_output',
+    'GetMaterializedViewsResult',
+    'AwaitableGetMaterializedViewsResult',
+    'get_materialized_views',
+    'get_materialized_views_output',
 ]
 
 @pulumi.output_type
-class GetConnectionsResult:
+class GetMaterializedViewsResult:
     """
-    A collection of values returned by GetConnections.
+    A collection of values returned by GetMaterializedViews.
     """
-    def __init__(__self__, connections=None, database_name=None, id=None, region=None, schema_name=None):
-        if connections and not isinstance(connections, list):
-            raise TypeError("Expected argument 'connections' to be a list")
-        pulumi.set(__self__, "connections", connections)
+    def __init__(__self__, database_name=None, id=None, materialized_views=None, region=None, schema_name=None):
         if database_name and not isinstance(database_name, str):
             raise TypeError("Expected argument 'database_name' to be a str")
         pulumi.set(__self__, "database_name", database_name)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if materialized_views and not isinstance(materialized_views, list):
+            raise TypeError("Expected argument 'materialized_views' to be a list")
+        pulumi.set(__self__, "materialized_views", materialized_views)
         if region and not isinstance(region, str):
             raise TypeError("Expected argument 'region' to be a str")
         pulumi.set(__self__, "region", region)
         if schema_name and not isinstance(schema_name, str):
             raise TypeError("Expected argument 'schema_name' to be a str")
         pulumi.set(__self__, "schema_name", schema_name)
 
     @property
-    @pulumi.getter
-    def connections(self) -> Sequence['outputs.GetConnectionsConnectionResult']:
-        """
-        The connections in the account
-        """
-        return pulumi.get(self, "connections")
-
-    @property
     @pulumi.getter(name="databaseName")
     def database_name(self) -> Optional[str]:
         """
-        Limit connections to a specific database
+        Limit materialized views to a specific database
         """
         return pulumi.get(self, "database_name")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter(name="materializedViews")
+    def materialized_views(self) -> Sequence['outputs.GetMaterializedViewsMaterializedViewResult']:
+        """
+        The materialized views in the account
+        """
+        return pulumi.get(self, "materialized_views")
+
+    @property
     @pulumi.getter
     def region(self) -> str:
         """
         The region in which the resource is located.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
     def schema_name(self) -> Optional[str]:
         """
-        Limit connections to a specific schema within a specific database
+        Limit materialized views to a specific schema within a specific database
         """
         return pulumi.get(self, "schema_name")
 
 
-class AwaitableGetConnectionsResult(GetConnectionsResult):
+class AwaitableGetMaterializedViewsResult(GetMaterializedViewsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetConnectionsResult(
-            connections=self.connections,
+        return GetMaterializedViewsResult(
             database_name=self.database_name,
             id=self.id,
+            materialized_views=self.materialized_views,
             region=self.region,
             schema_name=self.schema_name)
 
 
-def get_connections(database_name: Optional[str] = None,
-                    region: Optional[str] = None,
-                    schema_name: Optional[str] = None,
-                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetConnectionsResult:
+def get_materialized_views(database_name: Optional[str] = None,
+                           region: Optional[str] = None,
+                           schema_name: Optional[str] = None,
+                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMaterializedViewsResult:
     """
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_materialize as materialize
 
-    all = materialize.get_connections()
-    materialize = materialize.get_connections(database_name="materialize")
-    materialize_schema = materialize.get_connections(database_name="materialize",
+    all = materialize.get_materialized_views()
+    materialize = materialize.get_materialized_views(database_name="materialize")
+    materialize_schema = materialize.get_materialized_views(database_name="materialize",
         schema_name="schema")
     ```
 
 
-    :param str database_name: Limit connections to a specific database
+    :param str database_name: Limit materialized views to a specific database
     :param str region: The region in which the resource is located.
-    :param str schema_name: Limit connections to a specific schema within a specific database
+    :param str schema_name: Limit materialized views to a specific schema within a specific database
     """
     __args__ = dict()
     __args__['databaseName'] = database_name
     __args__['region'] = region
     __args__['schemaName'] = schema_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('materialize:index/getConnections:GetConnections', __args__, opts=opts, typ=GetConnectionsResult).value
+    __ret__ = pulumi.runtime.invoke('materialize:index/getMaterializedViews:GetMaterializedViews', __args__, opts=opts, typ=GetMaterializedViewsResult).value
 
-    return AwaitableGetConnectionsResult(
-        connections=pulumi.get(__ret__, 'connections'),
+    return AwaitableGetMaterializedViewsResult(
         database_name=pulumi.get(__ret__, 'database_name'),
         id=pulumi.get(__ret__, 'id'),
+        materialized_views=pulumi.get(__ret__, 'materialized_views'),
         region=pulumi.get(__ret__, 'region'),
         schema_name=pulumi.get(__ret__, 'schema_name'))
 
 
-@_utilities.lift_output_func(get_connections)
-def get_connections_output(database_name: Optional[pulumi.Input[Optional[str]]] = None,
-                           region: Optional[pulumi.Input[Optional[str]]] = None,
-                           schema_name: Optional[pulumi.Input[Optional[str]]] = None,
-                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetConnectionsResult]:
+@_utilities.lift_output_func(get_materialized_views)
+def get_materialized_views_output(database_name: Optional[pulumi.Input[Optional[str]]] = None,
+                                  region: Optional[pulumi.Input[Optional[str]]] = None,
+                                  schema_name: Optional[pulumi.Input[Optional[str]]] = None,
+                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMaterializedViewsResult]:
     """
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_materialize as materialize
 
-    all = materialize.get_connections()
-    materialize = materialize.get_connections(database_name="materialize")
-    materialize_schema = materialize.get_connections(database_name="materialize",
+    all = materialize.get_materialized_views()
+    materialize = materialize.get_materialized_views(database_name="materialize")
+    materialize_schema = materialize.get_materialized_views(database_name="materialize",
         schema_name="schema")
     ```
 
 
-    :param str database_name: Limit connections to a specific database
+    :param str database_name: Limit materialized views to a specific database
     :param str region: The region in which the resource is located.
-    :param str schema_name: Limit connections to a specific schema within a specific database
+    :param str schema_name: Limit materialized views to a specific schema within a specific database
     """
     ...
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_current_cluster.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_current_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_current_database.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_current_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_databases.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_databases.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_egress_ips.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_egress_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_indexes.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_indexes.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_roles.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_schemas.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_schemas.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_scim_configs.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_scim_configs.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_scim_groups.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_scim_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_secrets.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_sinks.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_sinks.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_sources.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_sources.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_sso_config.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_sso_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_system_parameters.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_system_parameters.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_tables.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_tables.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_types.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/get_views.py` & `pulumi_materialize-0.2.1/pulumi_materialize/get_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_cluster.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_cluster_default_privilege.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_cluster_default_privilege.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="targetRoleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_connection.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_connection_default_privilege.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_connection_default_privilege.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_database.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_database_default_privilege.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_database_default_privilege.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="targetRoleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_materialized_view.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_materialized_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_role.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         """
         The role name to add to role_name as a member.
         """
         return pulumi.get(self, "member_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_schema.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,15 +357,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_schema_default_privilege.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_schema_default_privilege.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="targetRoleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_secret.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_secret.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,15 +399,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_secret_default_privilege.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_secret_default_privilege.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_source.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_system_privilege.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_system_privilege.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         """
         The system privilege to grant.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_table.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_table_default_privilege.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_table_default_privilege.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,15 +409,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_type.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_type_default_privilege.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_type_default_privilege.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/grant_view.py` & `pulumi_materialize-0.2.1/pulumi_materialize/grant_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,15 @@
         """
         The privilege to grant to the object.
         """
         return pulumi.get(self, "privilege")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/index.py` & `pulumi_materialize-0.2.1/pulumi_materialize/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,15 +595,15 @@
         """
         The fully qualified name of the index.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/materialized_view.py` & `pulumi_materialize-0.2.1/pulumi_materialize/materialized_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,15 +613,15 @@
         """
         The fully qualified name of the materialized view.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/outputs.py` & `pulumi_materialize-0.2.1/pulumi_materialize/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/provider.py` & `pulumi_materialize-0.2.1/pulumi_materialize/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/region.py` & `pulumi_materialize-0.2.1/pulumi_materialize/region.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/role.py` & `pulumi_materialize-0.2.1/pulumi_materialize/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,13 +321,13 @@
         """
         The fully qualified name of the role.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/role_parameter.py` & `pulumi_materialize-0.2.1/pulumi_materialize/role_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         __props__.__dict__["role_name"] = role_name
         __props__.__dict__["variable_name"] = variable_name
         __props__.__dict__["variable_value"] = variable_value
         return RoleParameter(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="roleName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/schema.py` & `pulumi_materialize-0.2.1/pulumi_materialize/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,13 +387,13 @@
         """
         The fully qualified name of the schema.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/scim2_configuration.py` & `pulumi_materialize-0.2.1/pulumi_materialize/scim2_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/scim2_group.py` & `pulumi_materialize-0.2.1/pulumi_materialize/scim2_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/scim2_group_roles.py` & `pulumi_materialize-0.2.1/pulumi_materialize/scim2_group_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/scim2_group_users.py` & `pulumi_materialize-0.2.1/pulumi_materialize/scim2_group_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/secret.py` & `pulumi_materialize-0.2.1/pulumi_materialize/secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,15 +468,15 @@
         """
         The fully qualified name of the secret.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/sink_kafka.py` & `pulumi_materialize-0.2.1/pulumi_materialize/sink_kafka.py`

 * *Files 0% similar despite different names*

```diff
@@ -947,15 +947,15 @@
         """
         The fully qualified name of the sink.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/source_kafka.py` & `pulumi_materialize-0.2.1/pulumi_materialize/source_kafka.py`

 * *Files 0% similar despite different names*

```diff
@@ -1416,15 +1416,15 @@
         """
         The fully qualified name of the source.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/source_loadgen.py` & `pulumi_materialize-0.2.1/pulumi_materialize/source_loadgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -849,15 +849,15 @@
         """
         The fully qualified name of the source.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/source_mysql.py` & `pulumi_materialize-0.2.1/pulumi_materialize/source_mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -720,15 +720,15 @@
         """
         The fully qualified name of the source.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/source_postgres.py` & `pulumi_materialize-0.2.1/pulumi_materialize/source_postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -807,15 +807,15 @@
         """
         The fully qualified name of the source.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/source_webhook.py` & `pulumi_materialize-0.2.1/pulumi_materialize/source_webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -797,15 +797,15 @@
         """
         The fully qualified name of the source.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/sso_config.py` & `pulumi_materialize-0.2.1/pulumi_materialize/sso_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/sso_default_roles.py` & `pulumi_materialize-0.2.1/pulumi_materialize/sso_default_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/sso_domain.py` & `pulumi_materialize-0.2.1/pulumi_materialize/sso_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/sso_role_group_mapping.py` & `pulumi_materialize-0.2.1/pulumi_materialize/sso_role_group_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/system_parameter.py` & `pulumi_materialize-0.2.1/pulumi_materialize/system_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         """
         The name of the system parameter.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/table.py` & `pulumi_materialize-0.2.1/pulumi_materialize/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,15 +510,15 @@
         """
         The fully qualified name of the table.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/type.py` & `pulumi_materialize-0.2.1/pulumi_materialize/type.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,15 +613,15 @@
         """
         The fully qualified name of the type.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="rowProperties")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/user.py` & `pulumi_materialize-0.2.1/pulumi_materialize/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize/view.py` & `pulumi_materialize-0.2.1/pulumi_materialize/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,15 +518,15 @@
         """
         The fully qualified name of the view.
         """
         return pulumi.get(self, "qualified_sql_name")
 
     @property
     @pulumi.getter
-    def region(self) -> pulumi.Output[Optional[str]]:
+    def region(self) -> pulumi.Output[str]:
         """
         The region to use for the resource connection. If not set, the default region is used.
         """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="schemaName")
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize.egg-info/PKG-INFO` & `pulumi_materialize-0.2.1/pulumi_materialize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-materialize
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Pulumi package for creating and managing materialize cloud resources.
 Home-page: https://github.com/MaterializeInc/terraform-provider-materialize
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaterializeInc/terraform-provider-materialize
 Keywords: pulumi materialize category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_materialize-0.2.0/pulumi_materialize.egg-info/SOURCES.txt` & `pulumi_materialize-0.2.1/pulumi_materialize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.0/setup.py` & `pulumi_materialize-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.2.0"
+VERSION = "0.2.1"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "materialize Pulumi Package - Development Version"
```

