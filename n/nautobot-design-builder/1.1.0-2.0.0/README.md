# Comparing `tmp/nautobot_design_builder-1.1.0.tar.gz` & `tmp/nautobot_design_builder-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_design_builder-1.1.0.tar", max compression
+gzip compressed data, was "nautobot_design_builder-2.0.0.tar", max compression
```

## Comparing `nautobot_design_builder-1.1.0.tar` & `nautobot_design_builder-2.0.0.tar`

### file list

```diff
@@ -1,83 +1,61 @@
--rw-r--r--   0        0        0      591 2024-04-01 19:05:22.854016 nautobot_design_builder-1.1.0/LICENSE
--rw-r--r--   0        0        0     3305 2024-04-01 19:05:22.854016 nautobot_design_builder-1.1.0/README.md
--rw-r--r--   0        0        0     1271 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/__init__.py
--rw-r--r--   0        0        0    13473 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/context.py
--rw-r--r--   0        0        0        0 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/__init__.py
--rw-r--r--   0        0        0    22178 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/ext.py
--rw-r--r--   0        0        0        0 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/__init__.py
--rw-r--r--   0        0        0     1086 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/test_ext.py
--rw-r--r--   0        0        0      789 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/lookup_extension.yaml
--rw-r--r--   0        0        0     2630 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/bgp_extension.yaml
--rw-r--r--   0        0        0     1990 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/cable_connections.yaml
--rw-r--r--   0        0        0     1244 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/child_prefix.yaml
--rw-r--r--   0        0        0     1469 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/next_prefix.yaml
--rw-r--r--   0        0        0      725 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/next_prefix_by_role_and_tenant.yaml
--rw-r--r--   0        0        0     2822 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/bgp_extension.yaml
--rw-r--r--   0        0        0     2268 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/cable_connections.yaml
--rw-r--r--   0        0        0     1434 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/child_prefix.yaml
--rw-r--r--   0        0        0     1659 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/next_prefix.yaml
--rw-r--r--   0        0        0      915 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/next_prefix_by_role_and_tenant.yaml
--rw-r--r--   0        0        0     2246 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/debug.py
--rw-r--r--   0        0        0    35386 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/design.py
--rw-r--r--   0        0        0    10636 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/design_job.py
--rw-r--r--   0        0        0     8244 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/errors.py
--rw-r--r--   0        0        0    11551 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/ext.py
--rw-r--r--   0        0        0    14290 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/fields.py
--rw-r--r--   0        0        0     4030 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/git.py
--rw-r--r--   0        0        0     4014 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/helpers.py
--rw-r--r--   0        0        0     5967 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/jinja2.py
--rw-r--r--   0        0        0     4226 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/logging.py
--rw-r--r--   0        0        0       57 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/management/__init__.py
--rw-r--r--   0        0        0       57 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/management/commands/__init__.py
--rw-r--r--   0        0        0     1297 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/management/commands/build_design.py
--rw-r--r--   0        0        0      631 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/management/commands/install_demo_designs.py
--rw-r--r--   0        0        0     2867 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/__init__.py
--rw-r--r--   0        0        0      228 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/context.py
--rw-r--r--   0        0        0      312 2024-04-01 19:05:22.862016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/sub_designs/__init__.py
--rw-r--r--   0        0        0       71 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/templates/design_with_ref_error.yaml.j2
--rw-r--r--   0        0        0       30 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/templates/design_with_validation_error.yaml.j2
--rw-r--r--   0        0        0       49 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/templates/simple_design.yaml.j2
--rw-r--r--   0        0        0       51 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/templates/simple_design_2.yaml.j2
--rw-r--r--   0        0        0       81 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/templates/simple_design_3.yaml.j2
--rw-r--r--   0        0        0       13 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/templates/simple_report.md.j2
--rw-r--r--   0        0        0     2972 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/test_designs.py
--rw-r--r--   0        0        0     6436 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_builder.py
--rw-r--r--   0        0        0     6941 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_context.py
--rw-r--r--   0        0        0     8225 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_data_sources.py
--rw-r--r--   0        0        0     4961 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_design_job.py
--rw-r--r--   0        0        0     3804 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_errors.py
--rw-r--r--   0        0        0     3890 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_ext.py
--rw-r--r--   0        0        0     2761 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_jinja.py
--rw-r--r--   0        0        0      669 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/many_to_many.yaml
--rw-r--r--   0        0        0      422 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/assign_tags_by_name.yaml
--rw-r--r--   0        0        0      412 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/assign_tags_by_ref.yaml
--rw-r--r--   0        0        0     6639 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/complex_design1.yaml
--rw-r--r--   0        0        0     2332 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_by_ref.yaml
--rw-r--r--   0        0        0     1510 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_mlag.yaml
--rw-r--r--   0        0        0      800 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_rack.yaml
--rw-r--r--   0        0        0      895 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_or_update_relationships.yaml
--rw-r--r--   0        0        0      213 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/create_tags.yaml
--rw-r--r--   0        0        0     1360 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/custom_relationship_by_label.yaml
--rw-r--r--   0        0        0     1370 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/custom_relationship_by_slug.yaml
--rw-r--r--   0        0        0     1000 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/device_primary_ip.yaml
--rw-r--r--   0        0        0      337 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/git_repo.yaml
--rw-r--r--   0        0        0     1078 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/interface_addresses.yaml
--rw-r--r--   0        0        0     1039 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/nested_create.yaml
--rw-r--r--   0        0        0     1221 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/nested_update.yaml
--rw-r--r--   0        0        0     1282 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/one_to_one.yaml
--rw-r--r--   0        0        0      505 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/prefixes.yaml
--rw-r--r--   0        0        0     1615 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/custom_relationship_by_key.yaml
--rw-r--r--   0        0        0     1605 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/custom_relationship_by_label.yaml
--rw-r--r--   0        0        0      258 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/git_repo.yaml
--rw-r--r--   0        0        0     1480 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/interface_addresses.yaml
--rw-r--r--   0        0        0      815 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/ip_address_with_namespace.yaml
--rw-r--r--   0        0        0     1284 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/nested_create.yaml
--rw-r--r--   0        0        0      703 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/prefixes.yaml
--rw-r--r--   0        0        0      310 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/roll_back.yaml
--rw-r--r--   0        0        0      632 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/simple_create.yaml
--rw-r--r--   0        0        0      547 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/simple_update.yaml
--rw-r--r--   0        0        0      478 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/update_with_ref.yaml
--rw-r--r--   0        0        0    12483 2024-04-01 19:05:22.866016 nautobot_design_builder-1.1.0/nautobot_design_builder/util.py
--rw-r--r--   0        0        0     3599 2024-04-01 19:05:30.169982 nautobot_design_builder-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4426 1970-01-01 00:00:00.000000 nautobot_design_builder-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2024-05-01 17:00:04.100200 nautobot_design_builder-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3305 2024-05-01 17:00:04.100200 nautobot_design_builder-2.0.0/README.md
+-rw-r--r--   0        0        0     1271 2024-05-01 17:00:04.104200 nautobot_design_builder-2.0.0/nautobot_design_builder/__init__.py
+-rw-r--r--   0        0        0    13473 2024-05-01 17:00:04.104200 nautobot_design_builder-2.0.0/nautobot_design_builder/context.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:00:04.104200 nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/__init__.py
+-rw-r--r--   0        0        0    22178 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/ext.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/__init__.py
+-rw-r--r--   0        0        0      349 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/test_ext.py
+-rw-r--r--   0        0        0     2822 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/testdata/bgp_extension.yaml
+-rw-r--r--   0        0        0     2268 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/testdata/cable_connections.yaml
+-rw-r--r--   0        0        0     1434 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/testdata/child_prefix.yaml
+-rw-r--r--   0        0        0      789 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/testdata/lookup_extension.yaml
+-rw-r--r--   0        0        0     1659 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/testdata/next_prefix.yaml
+-rw-r--r--   0        0        0      915 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/testdata/next_prefix_by_role_and_tenant.yaml
+-rw-r--r--   0        0        0     2246 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/debug.py
+-rw-r--r--   0        0        0    35386 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/design.py
+-rw-r--r--   0        0        0     9754 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/design_job.py
+-rw-r--r--   0        0        0     8244 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/errors.py
+-rw-r--r--   0        0        0    11551 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/ext.py
+-rw-r--r--   0        0        0    14124 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/fields.py
+-rw-r--r--   0        0        0     4030 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/git.py
+-rw-r--r--   0        0        0     4014 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/helpers.py
+-rw-r--r--   0        0        0     5967 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/jinja2.py
+-rw-r--r--   0        0        0     3422 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/logging.py
+-rw-r--r--   0        0        0       57 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/management/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/management/commands/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/management/commands/build_design.py
+-rw-r--r--   0        0        0      631 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/management/commands/install_demo_designs.py
+-rw-r--r--   0        0        0     2280 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/designs/__init__.py
+-rw-r--r--   0        0        0      228 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/designs/context.py
+-rw-r--r--   0        0        0      312 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/designs/sub_designs/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/designs/templates/design_with_ref_error.yaml.j2
+-rw-r--r--   0        0        0       30 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/designs/templates/design_with_validation_error.yaml.j2
+-rw-r--r--   0        0        0       49 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/designs/templates/simple_design.yaml.j2
+-rw-r--r--   0        0        0       51 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/designs/templates/simple_design_2.yaml.j2
+-rw-r--r--   0        0        0       81 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/designs/templates/simple_design_3.yaml.j2
+-rw-r--r--   0        0        0       13 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/designs/templates/simple_report.md.j2
+-rw-r--r--   0        0        0     2793 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/designs/test_designs.py
+-rw-r--r--   0        0        0     5717 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/test_builder.py
+-rw-r--r--   0        0        0     6941 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/test_context.py
+-rw-r--r--   0        0        0     8225 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/test_data_sources.py
+-rw-r--r--   0        0        0     4466 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/test_design_job.py
+-rw-r--r--   0        0        0     3804 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/test_errors.py
+-rw-r--r--   0        0        0     3890 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/test_ext.py
+-rw-r--r--   0        0        0     2761 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/test_jinja.py
+-rw-r--r--   0        0        0     1615 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/custom_relationship_by_key.yaml
+-rw-r--r--   0        0        0     1605 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/custom_relationship_by_label.yaml
+-rw-r--r--   0        0        0      258 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/git_repo.yaml
+-rw-r--r--   0        0        0     1480 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/interface_addresses.yaml
+-rw-r--r--   0        0        0      815 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/ip_address_with_namespace.yaml
+-rw-r--r--   0        0        0      669 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/many_to_many.yaml
+-rw-r--r--   0        0        0     1284 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/nested_create.yaml
+-rw-r--r--   0        0        0      703 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/prefixes.yaml
+-rw-r--r--   0        0        0      310 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/roll_back.yaml
+-rw-r--r--   0        0        0      632 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/simple_create.yaml
+-rw-r--r--   0        0        0      547 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/simple_update.yaml
+-rw-r--r--   0        0        0      478 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/update_with_ref.yaml
+-rw-r--r--   0        0        0    12335 2024-05-01 17:00:04.108200 nautobot_design_builder-2.0.0/nautobot_design_builder/util.py
+-rw-r--r--   0        0        0     3535 2024-05-01 17:00:11.836305 nautobot_design_builder-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4346 1970-01-01 00:00:00.000000 nautobot_design_builder-2.0.0/PKG-INFO
```

### Comparing `nautobot_design_builder-1.1.0/LICENSE` & `nautobot_design_builder-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/README.md` & `nautobot_design_builder-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/__init__.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/context.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/context.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/ext.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/ext.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/lookup_extension.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/testdata/lookup_extension.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/bgp_extension.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/testdata/bgp_extension.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 ---
 extensions:
   - "nautobot_design_builder.contrib.ext.BGPPeeringExtension"
 designs:
-  - sites:
-      - "!create_or_update:name": "Site"
-        status__name: "Active"
-
-    device_roles:
-      - "!create_or_update:name": "test-role"
+  - roles:
+      - name: "test-role"
+        content_types:
+          - "!get:app_label": "dcim"
+            "!get:model": "device"
+    prefixes:
+      - status__name: "Active"
+        prefix: "192.168.1.0/24"
+
+    location_types:
+      - name: "Site"
+        content_types:
+          - "!get:app_label": "dcim"
+            "!get:model": "device"
+        locations:
+          - name: "Site"
+            status__name: "Active"
 
     manufacturers:
       - "!create_or_update:name": "test-manufacturer"
 
     device_types:
       - manufacturer__name: "test-manufacturer"
         "!create_or_update:model": "test-type"
@@ -19,58 +30,56 @@
     autonomous_systems:
       - "!create_or_update:asn": 64500
         status__name: "Active"
 
     devices:
       - "!create_or_update:name": "device1"
         status__name: "Active"
-        site__name: "Site"
-        device_role__name: "test-role"
+        location__name: "Site"
+        role__name: "test-role"
         device_type__model: "test-type"
         interfaces:
           - "!create_or_update:name": "Ethernet1/1"
             type: "virtual"
             status__name: "Active"
-            ip_addresses:
-              - "!create_or_update:address": "192.168.1.1/24"
-                status__name: "Active"
+            ip_address_assignments:
+              - ip_address:
+                  "!create_or_update:address": "192.168.1.1/24"
+                  status__name: "Active"
         bgp_routing_instances:
           - "!create_or_update:autonomous_system__asn": 64500
             "!ref": "device1-instance"
             status__name: "Active"
 
       - "!create_or_update:name": "device2"
         status__name: "Active"
-        site__name: "Site"
-        device_role__name: "test-role"
+        location__name: "Site"
+        role__name: "test-role"
         device_type__model: "test-type"
         interfaces:
           - "!create_or_update:name": "Ethernet1/1"
             type: "virtual"
             status__name: "Active"
-            ip_addresses:
-              - "!create_or_update:address": "192.168.1.2/24"
-                status__name: "Active"
+            ip_address_assignments:
+              - ip_address:
+                  "!create_or_update:address": "192.168.1.2/24"
+                  status__name: "Active"
         bgp_routing_instances:
           - "!create_or_update:autonomous_system__asn": 64500
             "!ref": "device2-instance"
             status__name: "Active"
 
     bgp_peerings:
       - "!bgp_peering":
           endpoint_a:
             "!create_or_update:routing_instance__device__name": "device1"
-            "!create_or_update:source_ip":
-              "!get:interface__device__name": "device1"
-              "!get:interface__name": "Ethernet1/1"
+            "!create_or_update:source_ip__address": "192.168.1.1/24"
           endpoint_z:
             "!create_or_update:routing_instance__device__name": "device2"
-            "!create_or_update:source_ip":
-              "!get:interface__device__name": "device2"
-              "!get:interface__name": "Ethernet1/1"
+            "!create_or_update:source_ip__address": "192.168.1.2/24"
         status__name: "Active"
 checks:
   - equal:
       - model: "nautobot_bgp_models.models.PeerEndpoint"
         query: {routing_instance__device__name: "device1"}
         attribute: "peering"
       - model: "nautobot_bgp_models.models.PeerEndpoint"
```

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/cable_connections.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/interface_addresses.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,54 @@
 ---
-extensions:
-  - "nautobot_design_builder.contrib.ext.CableConnectionExtension"
 designs:
-  - sites:
-      - "!create_or_update:name": "Site"
-        status__name: "Active"
-    device_roles:
-      - "!create_or_update:name": "test-role"
-    manufacturers:
-      - "!create_or_update:name": "test-manufacturer"
+  - manufacturers:
+      - name: "manufacturer1"
+
     device_types:
-      - manufacturer__name: "test-manufacturer"
-        "!create_or_update:model": "test-type"
-    devices:
-      - "!create_or_update:name": "Device 1"
-        "!ref": "device1"
-        site__name: "Site"
-        status__name: "Active"
-        device_role__name: "test-role"
-        device_type__model: "test-type"
-        interfaces:
-          - "!create_or_update:name": "GigabitEthernet1"
-            type: "1000base-t"
+      - manufacturer__name: "manufacturer1"
+        model: "model name"
+        u_height: 1
+
+    roles:
+      - name: "device role"
+        content_types:
+          - "!get:app_label": "dcim"
+            "!get:model": "device"
+
+    location_types:
+      - name: "Site"
+        content_types:
+          - "!get:app_label": "dcim"
+            "!get:model": "device"
+        locations:
+          - name: "site_1"
             status__name: "Active"
-      - "!create_or_update:name": "Device 2"
-        site__name: "Site"
+
+    prefixes:
+      - prefix: "192.168.56.0/24"
+        status__name: "Active"
+        "!ref": "parent_prefix"
+
+    devices:
+      - name: "device_1"
+        location__name: "site_1"
         status__name: "Active"
-        device_role__name: "test-role"
-        device_type__model: "test-type"
+        device_type__model: "model name"
+        role__name: "device role"
         interfaces:
-          - "!create_or_update:name": "GigabitEthernet1"
-            type: "1000base-t"
+          - name: "Ethernet1/1"
+            type: "virtual"
             status__name: "Active"
-            "!connect_cable":
-              status__name: "Planned"
-              to:
-                device: "!ref:device1"
-                name: "GigabitEthernet1"
-  # Second design, same as the first, checks for
-  # cable connection idempotence
-  - devices:
-      - "!create_or_update:name": "Device 1"
-        "!ref": "device1"
-      - "!create_or_update:name": "Device 2"
-        interfaces:
-          - "!create_or_update:name": "GigabitEthernet1"
-            "!connect_cable":
-              status__name: "Planned"
-              to:
-                device: "!ref:device1"
-                name: "GigabitEthernet1"
-
+            ip_address_assignments:
+              - ip_address:
+                  "!create_or_update:address": "192.168.56.1/24"
+                  "!create_or_update:parent": "!ref:parent_prefix"
+                  status__name: "Active"
 checks:
-  - connected:
-      - model: "nautobot.dcim.models.Interface"
-        query: {device__name: "Device 1", name: "GigabitEthernet1"}
-      - model: "nautobot.dcim.models.Interface"
-        query: {device__name: "Device 2", name: "GigabitEthernet1"}
+  - model_exists:
+      model: "nautobot.ipam.models.IPAddress"
+      query: {address: "192.168.56.1/24"}
+  - equal:
+      - model: "nautobot.ipam.models.IPAddressToInterface"
+        query: {interface__name: "Ethernet1/1"}
+        attribute: "ip_address"
+      - model: "nautobot.ipam.models.IPAddress"
```

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/child_prefix.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/testdata/next_prefix.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,61 @@
 ---
 extensions:
   - "nautobot_design_builder.contrib.ext.NextPrefixExtension"
-  - "nautobot_design_builder.contrib.ext.ChildPrefixExtension"
 designs:
   - tenants:
       - name: "Nautobot Airports"
     roles:
       - name: "Video"
+        content_types:
+          - "!get:app_label": "ipam"
+            "!get:model": "prefix"
       - name: "Servers"
-    prefixes:
+        content_types:
+          - "!get:app_label": "ipam"
+            "!get:model": "prefix"
+  - prefixes:
       - prefix: "10.0.0.0/23"
         status__name: "Active"
         tenant__name: "Nautobot Airports"
         role__name: "Servers"
       - prefix: "10.0.2.0/23"
         status__name: "Active"
         tenant__name: "Nautobot Airports"
         role__name: "Video"
       - "!next_prefix":
           prefix:
             - "10.0.0.0/23"
+            - "10.0.2.0/23"
           length: 24
         status__name: "Active"
-        "!ref": "parent_prefix"
-      - "!child_prefix":
-          parent: "!ref:parent_prefix"
-          offset: "0.0.0.0/25"
-        status__name: "Active"
-      - "!child_prefix":
-          parent: "!ref:parent_prefix"
-          offset: "0.0.0.128/25"
+      - "!next_prefix":
+          prefix:
+            - "10.0.0.0/23"
+            - "10.0.2.0/23"
+          length: 24
+        status__name: "Active"
+      - "!next_prefix":
+          prefix:
+            - "10.0.0.0/23"
+            - "10.0.2.0/23"
+          length: 24
+        status__name: "Active"
+      - "!next_prefix":
+          prefix:
+            - "10.0.0.0/23"
+            - "10.0.2.0/23"
+          length: 24
         status__name: "Active"
 checks:
   - model_exists:
       model: "nautobot.ipam.models.Prefix"
       query: {prefix: "10.0.0.0/24"}
   - model_exists:
       model: "nautobot.ipam.models.Prefix"
-      query: {prefix: "10.0.0.0/25"}
+      query: {prefix: "10.0.1.0/24"}
+  - model_exists:
+      model: "nautobot.ipam.models.Prefix"
+      query: {prefix: "10.0.2.0/24"}
   - model_exists:
       model: "nautobot.ipam.models.Prefix"
-      query: {prefix: "10.0.0.128/25"}
+      query: {prefix: "10.0.3.0/24"}
```

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v1/next_prefix_by_role_and_tenant.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/testdata/child_prefix.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 ---
 extensions:
   - "nautobot_design_builder.contrib.ext.NextPrefixExtension"
+  - "nautobot_design_builder.contrib.ext.ChildPrefixExtension"
 designs:
   - tenants:
       - name: "Nautobot Airports"
     roles:
       - name: "Video"
+        content_types:
+          - "!get:app_label": "ipam"
+            "!get:model": "prefix"
       - name: "Servers"
-    prefixes:
+        content_types:
+          - "!get:app_label": "ipam"
+            "!get:model": "prefix"
+  - prefixes:
       - prefix: "10.0.0.0/23"
         status__name: "Active"
         tenant__name: "Nautobot Airports"
         role__name: "Servers"
       - prefix: "10.0.2.0/23"
         status__name: "Active"
         tenant__name: "Nautobot Airports"
         role__name: "Video"
       - "!next_prefix":
-          role__name: "Video"
-          tenant__name: "Nautobot Airports"
+          prefix:
+            - "10.0.0.0/23"
           length: 24
         status__name: "Active"
+        "!ref": "parent_prefix"
+      - "!child_prefix":
+          parent: "!ref:parent_prefix"
+          offset: "0.0.0.0/25"
+        status__name: "Active"
+      - "!child_prefix":
+          parent: "!ref:parent_prefix"
+          offset: "0.0.0.128/25"
+        status__name: "Active"
 checks:
   - model_exists:
       model: "nautobot.ipam.models.Prefix"
-      query: {prefix: "10.0.2.0/24"}
+      query: {prefix: "10.0.0.0/24"}
+  - model_exists:
+      model: "nautobot.ipam.models.Prefix"
+      query: {prefix: "10.0.0.0/25"}
+  - model_exists:
+      model: "nautobot.ipam.models.Prefix"
+      query: {prefix: "10.0.0.128/25"}
```

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/cable_connections.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/testdata/cable_connections.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/contrib/tests/testdata/nautobot_v2/child_prefix.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/contrib/tests/testdata/next_prefix_by_role_and_tenant.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 ---
 extensions:
   - "nautobot_design_builder.contrib.ext.NextPrefixExtension"
-  - "nautobot_design_builder.contrib.ext.ChildPrefixExtension"
 designs:
   - tenants:
       - name: "Nautobot Airports"
     roles:
       - name: "Video"
         content_types:
           - "!get:app_label": "ipam"
@@ -20,30 +19,15 @@
         tenant__name: "Nautobot Airports"
         role__name: "Servers"
       - prefix: "10.0.2.0/23"
         status__name: "Active"
         tenant__name: "Nautobot Airports"
         role__name: "Video"
       - "!next_prefix":
-          prefix:
-            - "10.0.0.0/23"
+          role__name: "Video"
+          tenant__name: "Nautobot Airports"
           length: 24
         status__name: "Active"
-        "!ref": "parent_prefix"
-      - "!child_prefix":
-          parent: "!ref:parent_prefix"
-          offset: "0.0.0.0/25"
-        status__name: "Active"
-      - "!child_prefix":
-          parent: "!ref:parent_prefix"
-          offset: "0.0.0.128/25"
-        status__name: "Active"
 checks:
   - model_exists:
       model: "nautobot.ipam.models.Prefix"
-      query: {prefix: "10.0.0.0/24"}
-  - model_exists:
-      model: "nautobot.ipam.models.Prefix"
-      query: {prefix: "10.0.0.0/25"}
-  - model_exists:
-      model: "nautobot.ipam.models.Prefix"
-      query: {prefix: "10.0.0.128/25"}
+      query: {prefix: "10.0.2.0/24"}
```

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/debug.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/debug.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/design.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/design.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/design_job.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/design_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,53 +8,46 @@
 import yaml
 
 from django.db import transaction
 from django.core.files.base import ContentFile
 
 from jinja2 import TemplateError
 
-from nautobot.extras.jobs import Job
+from nautobot.apps.jobs import Job, DryRunVar
 from nautobot.extras.models import FileProxy
 
 from nautobot_design_builder.errors import DesignImplementationError, DesignModelError
 from nautobot_design_builder.jinja2 import new_template_environment
 from nautobot_design_builder.logging import LoggingMixin
 from nautobot_design_builder.design import Environment
 from nautobot_design_builder.context import Context
-from .util import nautobot_version
 
 
 class DesignJob(Job, ABC, LoggingMixin):  # pylint: disable=too-many-instance-attributes
     """The base Design Job class that all specific Design Builder jobs inherit from.
 
     DesignJob is an abstract base class that all design implementations must implement.
     Any design that is to be included in the list of Jobs in Nautobot *must* include
     a Meta class.
     """
 
-    if nautobot_version >= "2.0.0":
-        from nautobot.extras.jobs import DryRunVar  # pylint: disable=no-name-in-module,import-outside-toplevel
-
-        dryrun = DryRunVar()
+    dryrun = DryRunVar()
 
     @classmethod
     @abstractmethod
     def Meta(cls) -> Job.Meta:  # pylint: disable=invalid-name
         """Design jobs must provide either a Meta class method or a Meta class."""
 
     def __init__(self, *args, **kwargs):
         """Initialize the design job."""
         # rendered designs
         self.environment: Environment = None
         self.designs = {}
-        # TODO: Remove this when we no longer support Nautobot 1.x
-        self.rendered = None
         self.rendered_design = None
-        self.failed = False
-        self.report = None
+        self.rendered = None
 
         super().__init__(*args, **kwargs)
 
     def post_implementation(self, context: Context, environment: Environment):
         """Similar to Nautobot job's `post_run` method, but will be called after a design is implemented.
 
         Any design job that requires additional work to be completed after the design
@@ -63,24 +56,14 @@
         transaction has been committed.
 
         Args:
             context (Context): The render context that was used for rendering the design files.
             environment (Environment): The build environment that consumed the rendered design files. This is useful for accessing the design journal.
         """
 
-    def post_run(self):
-        """Method that will run after the main Nautobot job has executed."""
-        # TODO: This is not supported in Nautobot 2 and the entire method
-        # should be removed once we no longer support Nautobot 1.
-        if self.rendered:
-            self.job_result.data["output"] = self.rendered
-
-        self.job_result.data["designs"] = self.designs
-        self.job_result.data["report"] = self.report
-
     def render(self, context: Context, filename: str) -> str:
         """High level function to render the Jinja design templates into YAML.
 
         Args:
             context (Context object): a tree of variables that can include templates for values
             filename (str): file name of the Jinja design template
 
@@ -150,18 +133,18 @@
         )
 
     def implement_design(self, context, design_file, commit):
         """Render the design_file template using the provided render context."""
         design = self.render_design(context, design_file)
         self.environment.implement_design(design, commit)
 
-    def run(self, **kwargs):  # pylint: disable=arguments-differ
+    def run(self, dryrun: bool, **kwargs):  # pylint: disable=arguments-differ
         """Render the design and implement it within a build Environment object."""
         try:
-            return self._run_in_transaction(**kwargs)
+            return self._run_in_transaction(dryrun, **kwargs)
         finally:
             if self.rendered:
                 rendered_design = path.basename(self.rendered_design)
                 rendered_design, _ = path.splitext(rendered_design)
                 if not rendered_design.endswith(".yaml") and not rendered_design.endswith(".yml"):
                     rendered_design = f"{rendered_design}.yaml"
                 self.save_design_file(rendered_design, self.rendered)
@@ -170,87 +153,75 @@
                 # this should remove the .j2
                 output_file, _ = path.splitext(output_file)
                 if not output_file.endswith(".yaml") and not output_file.endswith(".yml"):
                     output_file = f"{output_file}.yaml"
                 self.save_design_file(output_file, yaml.safe_dump(design))
 
     @transaction.atomic
-    def _run_in_transaction(self, **kwargs):  # pylint: disable=too-many-branches
+    def _run_in_transaction(self, dryrun: bool, **data):  # pylint: disable=too-many-branches
         """Render the design and implement it within a build Environment object.
 
         This version of `run` is wrapped in a transaction and will roll back database changes
         on error. In general, this method should only be called by the `run` method.
         """
         self.log_info(message=f"Building {getattr(self.Meta, 'name')}")
         extensions = getattr(self.Meta, "extensions", [])
         self.environment = Environment(job_result=self.job_result, extensions=extensions)
 
         design_files = None
 
-        if nautobot_version < "2.0.0":
-            commit = kwargs["commit"]
-            data = kwargs["data"]
-        else:
-            commit = not kwargs.pop("dryrun", True)
-            data = kwargs
-
         if hasattr(self.Meta, "context_class"):
             context = self.Meta.context_class(data=data, job_result=self.job_result)
             context.validate()
         else:
             context = {}
 
         if hasattr(self.Meta, "design_file"):
             design_files = [self.Meta.design_file]
         elif hasattr(self.Meta, "design_files"):
             design_files = self.Meta.design_files
         else:
             self.log_failure(message="No design template specified for design.")
-            self.failed = True
-            return
+            raise DesignImplementationError("No design template specified for design.")
 
         sid = transaction.savepoint()
 
         try:
             for design_file in design_files:
-                self.implement_design(context, design_file, commit)
-            if commit:
+                self.implement_design(context, design_file, not dryrun)
+            if not dryrun:
                 self.post_implementation(context, self.environment)
                 if hasattr(self.Meta, "report"):
-                    self.report = self.render_report(context, self.environment.journal)
-                    self.log_success(message=self.report)
-                    if nautobot_version >= "2.0":
-                        self.save_design_file("report.md", self.report)
+                    report = self.render_report(context, self.environment.journal)
+                    output_filename: str = path.basename(getattr(self.Meta, "report"))
+                    if output_filename.endswith(".j2"):
+                        output_filename = output_filename[0:-3]
+                    self.log_success(message=report)
+                    self.save_design_file(output_filename, report)
             else:
                 transaction.savepoint_rollback(sid)
                 self.log_info(
                     message=f"{self.name} can be imported successfully - No database changes made",
                 )
         except (DesignImplementationError, DesignModelError) as ex:
             transaction.savepoint_rollback(sid)
             self.log_failure(message="Failed to implement design")
             self.log_failure(message=str(ex))
-            self.failed = True
-            if nautobot_version >= "2":
-                raise ex
+            raise ex
         except Exception as ex:
             transaction.savepoint_rollback(sid)
-            self.failed = True
             raise ex
 
     def save_design_file(self, filename, content):
         """Save some content to a job file.
 
         This is only supported on Nautobot 2.0 and greater.
 
         Args:
             filename (str): The name of the file to save.
             content (str): The content to save to the file.
         """
-        if nautobot_version < "2.0":
-            return
-
         FileProxy.objects.create(
             name=filename,
             job_result=self.job_result,
             file=ContentFile(content.encode("utf-8"), name=filename),
         )
```

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/errors.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/errors.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/ext.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/ext.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/fields.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 from taggit.managers import TaggableManager
 
 from nautobot.core.graphql.utils import str_to_var_name
 from nautobot.extras.models import Relationship, RelationshipAssociation
 
 from nautobot_design_builder.errors import DesignImplementationError
 from nautobot_design_builder.debug import debug_set
-from nautobot_design_builder.util import nautobot_version
 
 if TYPE_CHECKING:
     from .design import ModelInstance
     from django.db.models.manager import Manager
 
 
 class ModelField(ABC):
@@ -291,18 +290,15 @@
         if self.relationship.source_type == ContentType.objects.get_for_model(model_class.model_class):
             self.related_model = relationship.destination_type.model_class()
             field_name = str(self.relationship.get_label("source"))
         else:
             self.related_model = relationship.source_type.model_class()
             field_name = str(self.relationship.get_label("destination"))
         self.__set_name__(model_class, str_to_var_name(field_name))
-        if nautobot_version < "2.0.0":
-            self.key_name = self.relationship.slug
-        else:
-            self.key_name = self.relationship.key
+        self.key_name = self.relationship.key
 
     @debug_set
     def __set__(self, obj: "ModelInstance", values):  # noqa:D105
         """Add an association between the created object and the given value.
 
         Args:
             values (Model): The related objects to add.
```

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/git.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/git.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/helpers.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/helpers.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/jinja2.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/jinja2.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/logging.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/logging.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,26 @@
 """Defines logging capability for design builder."""
 
 import logging
 
 from nautobot.extras.choices import LogLevelChoices
 from nautobot.extras.models import JobResult
 
-from .util import nautobot_version
-
-if nautobot_version < "2.0.0":
-    # MIN_VERSION: 2.0.0
-    _logger_to_level_choices = {
-        logging.DEBUG: LogLevelChoices.LOG_INFO,
-        logging.INFO: LogLevelChoices.LOG_INFO,
-        logging.WARNING: LogLevelChoices.LOG_WARNING,
-        logging.ERROR: LogLevelChoices.LOG_FAILURE,  # pylint: disable=no-member
-        logging.CRITICAL: LogLevelChoices.LOG_FAILURE,  # pylint: disable=no-member
-    }
-    LOG_INFO = LogLevelChoices.LOG_INFO
-    LOG_DEBUG = LogLevelChoices.LOG_INFO
-    LOG_SUCCESS = LogLevelChoices.LOG_SUCCESS  # pylint: disable=no-member
-    LOG_WARNING = LogLevelChoices.LOG_WARNING
-    LOG_FAILURE = LogLevelChoices.LOG_FAILURE  # pylint: disable=no-member
-    # /MIN_VERSION: 2.0.0
-else:
-    _logger_to_level_choices = {
-        logging.DEBUG: LogLevelChoices.LOG_DEBUG,  # pylint: disable=no-member
-        logging.INFO: LogLevelChoices.LOG_INFO,
-        logging.WARNING: LogLevelChoices.LOG_WARNING,
-        logging.ERROR: LogLevelChoices.LOG_ERROR,  # pylint: disable=no-member
-        logging.CRITICAL: LogLevelChoices.LOG_CRITICAL,  # pylint: disable=no-member
-    }
-    LOG_INFO = LogLevelChoices.LOG_INFO
-    LOG_DEBUG = LogLevelChoices.LOG_DEBUG  # pylint: disable=no-member
-    LOG_SUCCESS = LogLevelChoices.LOG_INFO
-    LOG_WARNING = LogLevelChoices.LOG_WARNING
-    LOG_FAILURE = LogLevelChoices.LOG_ERROR  # pylint: disable=no-member
+_logger_to_level_choices = {
+    logging.DEBUG: LogLevelChoices.LOG_DEBUG,  # pylint: disable=no-member
+    logging.INFO: LogLevelChoices.LOG_INFO,
+    logging.WARNING: LogLevelChoices.LOG_WARNING,
+    logging.ERROR: LogLevelChoices.LOG_ERROR,  # pylint: disable=no-member
+    logging.CRITICAL: LogLevelChoices.LOG_CRITICAL,  # pylint: disable=no-member
+}
+LOG_INFO = LogLevelChoices.LOG_INFO
+LOG_DEBUG = LogLevelChoices.LOG_DEBUG  # pylint: disable=no-member
+LOG_SUCCESS = LogLevelChoices.LOG_INFO
+LOG_WARNING = LogLevelChoices.LOG_WARNING
+LOG_FAILURE = LogLevelChoices.LOG_ERROR  # pylint: disable=no-member
 
 
 class JobResultHandler(logging.Handler):
     """JobResultHandler is a logging handler that will copy logged messages to a JobResult."""
 
     def __init__(self, job_result: JobResult):
         """Initialize the JobResultHandler.
```

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/management/commands/build_design.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/management/commands/build_design.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/management/commands/install_demo_designs.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/management/commands/install_demo_designs.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/designs/test_designs.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/designs/test_designs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Design jobs used for unit testing."""
 
+from nautobot.apps.jobs import register_jobs
+
 from nautobot_design_builder.design_job import DesignJob
 from nautobot_design_builder.ext import Extension
-from nautobot_design_builder.util import nautobot_version
 
 
 class SimpleDesign(DesignJob):
     """Simple design job."""
 
     class Meta:  # pylint: disable=too-few-public-methods
         name = "Simple Design"
@@ -79,19 +80,16 @@
     """Design job that has objects with failing validation."""
 
     class Meta:  # pylint: disable=too-few-public-methods
         name = "Design with validation errors"
         design_file = "templates/design_with_validation_error.yaml.j2"
 
 
-if nautobot_version >= "2.0":
-    from nautobot.apps.jobs import register_jobs  # pylint: disable=import-error, no-name-in-module
-
-    register_jobs(
-        SimpleDesign,
-        SimpleDesignReport,
-        MultiDesignJob,
-        MultiDesignJobWithError,
-        DesignJobWithExtensions,
-        DesignWithRefError,
-        DesignWithValidationError,
-    )
+register_jobs(
+    SimpleDesign,
+    SimpleDesignReport,
+    MultiDesignJob,
+    MultiDesignJobWithError,
+    DesignJobWithExtensions,
+    DesignWithRefError,
+    DesignWithValidationError,
+)
```

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_context.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_data_sources.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/test_data_sources.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_design_job.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/test_design_job.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,113 +5,95 @@
 from django.core.exceptions import ValidationError
 
 from nautobot.dcim.models import Manufacturer
 
 from nautobot_design_builder.errors import DesignImplementationError, DesignValidationError
 from nautobot_design_builder.tests import DesignTestCase
 from nautobot_design_builder.tests.designs import test_designs
-from nautobot_design_builder.util import nautobot_version
 
 
 class TestDesignJob(DesignTestCase):
     """Test running design jobs."""
 
     @patch("nautobot_design_builder.design_job.Environment")
     def test_simple_design_commit(self, environment: Mock):
         job = self.get_mocked_job(test_designs.SimpleDesign)
-        job.run(data={}, commit=True)
+        job.run(data={}, dryrun=False)
         self.assertIsNotNone(job.job_result)
         environment.assert_called()
         self.assertDictEqual(
             {"manufacturers": {"name": "Test Manufacturer"}},
             job.designs[test_designs.SimpleDesign.Meta.design_file],
         )
         environment.return_value.roll_back.assert_not_called()
 
     def test_simple_design_rollback(self):
         job1 = self.get_mocked_job(test_designs.SimpleDesign)
-        job1.run(data={}, commit=True)
-        self.assertFalse(job1.failed)
+        job1.run(data={}, dryrun=False)
         self.assertEqual(1, Manufacturer.objects.all().count())
         job2 = self.get_mocked_job(test_designs.SimpleDesign3)
-        if nautobot_version < "2":
-            job2.run(data={}, commit=True)
-        else:
-            self.assertRaises(DesignValidationError, job2.run, data={}, commit=True)
-        self.assertTrue(job2.failed)
+        self.assertRaises(DesignValidationError, job2.run, data={}, dryrun=False)
         self.assertEqual(1, Manufacturer.objects.all().count())
 
     def test_simple_design_report(self):
         job = self.get_mocked_job(test_designs.SimpleDesignReport)
-        job.run(data={}, commit=True)
-        self.assertJobSuccess(job)
-        self.assertEqual("Report output", job.report)
+        job.run(data={}, dryrun=False)
+        self.assertIn("simple_report.md", job.saved_files)  # pylint:disable=no-member
+        self.assertEqual("Report output", job.saved_files["simple_report.md"])  # pylint:disable=no-member
 
     def test_multiple_design_files(self):
         job = self.get_mocked_job(test_designs.MultiDesignJob)
-        job.run(data={}, commit=True)
+        job.run(data={}, dryrun=False)
         self.assertDictEqual(
             {"manufacturers": {"name": "Test Manufacturer"}},
             job.designs[test_designs.MultiDesignJob.Meta.design_files[0]],
         )
         self.assertDictEqual(
             {"manufacturers": {"name": "Test Manufacturer 1"}},
             job.designs[test_designs.MultiDesignJob.Meta.design_files[1]],
         )
 
     def test_multiple_design_files_with_roll_back(self):
         self.assertEqual(0, Manufacturer.objects.all().count())
         job = self.get_mocked_job(test_designs.MultiDesignJobWithError)
-        if nautobot_version < "2":
-            job.run(data={}, commit=True)
-        else:
-            self.assertRaises(DesignValidationError, job.run, data={}, commit=True)
+        self.assertRaises(DesignValidationError, job.run, data={}, dryrun=False)
 
         self.assertEqual(0, Manufacturer.objects.all().count())
 
     @patch("nautobot_design_builder.design_job.Environment")
     def test_custom_extensions(self, environment: Mock):
         job = self.get_mocked_job(test_designs.DesignJobWithExtensions)
-        job.run(data={}, commit=True)
+        job.run(data={}, dryrun=False)
         environment.assert_called_once_with(
             job_result=job.job_result,
             extensions=test_designs.DesignJobWithExtensions.Meta.extensions,
         )
 
 
 class TestDesignJobLogging(DesignTestCase):
     """Test that the design job logs errors correctly."""
 
     @patch("nautobot_design_builder.design_job.Environment")
     def test_simple_design_implementation_error(self, environment: Mock):
         environment.return_value.implement_design.side_effect = DesignImplementationError("Broken")
         job = self.get_mocked_job(test_designs.SimpleDesign)
-        if nautobot_version < "2":
-            job.run(data={}, commit=True)
-        else:
-            self.assertRaises(DesignImplementationError, job.run, data={}, commit=True)
+        self.assertRaises(DesignImplementationError, job.run, data={}, dryrun=True)
         self.assertTrue(job.failed)
         job.job_result.log.assert_called()
         self.assertEqual("Broken", self.logged_messages[-1]["message"])
 
     def test_invalid_ref(self):
         job = self.get_mocked_job(test_designs.DesignWithRefError)
-        if nautobot_version < "2":
-            job.run(data={}, commit=True)
-        else:
-            self.assertRaises(DesignImplementationError, job.run, data={}, commit=True)
+        self.assertRaises(DesignImplementationError, job.run, data={}, dryrun=False)
         message = self.logged_messages[-1]["message"]
         self.assertEqual("No ref named manufacturer has been saved in the design.", message)
 
     def test_failed_validation(self):
         job = self.get_mocked_job(test_designs.DesignWithValidationError)
-        if nautobot_version < "2":
-            job.run(data={}, commit=True)
-        else:
-            self.assertRaises(DesignValidationError, job.run, data={}, commit=True)
+        self.assertRaises(DesignValidationError, job.run, data={}, dryrun=False)
         message = self.logged_messages[-1]["message"]
 
         want_error = DesignValidationError("Manufacturer")
         want_error.__cause__ = ValidationError(
             {
                 "name": "This field cannot be blank.",
             }
```

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_errors.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_ext.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/test_jinja.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/many_to_many.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/many_to_many.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/custom_relationship_by_label.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/custom_relationship_by_label.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 ---
 extensions:
   - "nautobot_design_builder.contrib.ext.LookupExtension"
 designs:
   - relationships:
-      - name: "Device to VLANS"
-        slug: "device-to-vlans"
+      - label: "Device to VLANS"
+        key: "device_to_vlans"
         type: "many-to-many"
         "!lookup:source_type":
           app_label: "dcim"
           model: "device"
         "!lookup:destination_type":
           app_label: "ipam"
           model: "vlan"
+
     manufacturers:
       - name: "manufacturer1"
 
     device_types:
       - manufacturer__name: "manufacturer1"
         model: "model name"
         u_height: 1
 
-    device_roles:
+    roles:
       - name: "device role"
-
-    sites:
-      - name: "site_1"
-        status__name: "Active"
+        content_types:
+          - "!get:app_label": "dcim"
+            "!get:model": "device"
+
+    location_types:
+      - name: "Site"
+        content_types:
+          - "!get:app_label": "dcim"
+            "!get:model": "device"
+        locations:
+          - name: "site_1"
+            status__name: "Active"
 
     vlans:
       - "!create_or_update:vid": 42
         name: "The Answer"
         status__name: "Active"
 
     devices:
       - name: "device_1"
-        site__name: "site_1"
+        location__name: "site_1"
         status__name: "Active"
         device_type__model: "model name"
-        device_role__name: "device role"
+        role__name: "device role"
         vlans:
           - "!get:vid": 42
           - vid: "43"
             name: "Better Answer"
             status__name: "Active"
 checks:
   - model_exists:
       model: "nautobot.ipam.models.VLAN"
       query: {vid: "43"}
 
-  - equal:
+  - count_equal:
       - model: "nautobot.extras.models.RelationshipAssociation"
-        query: {relationship__name: "Device to VLANS"}
+        query: {relationship__label: "Device to VLANS"}
         attribute: "destination"
       - model: "nautobot.ipam.models.VLAN"
```

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/custom_relationship_by_slug.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/custom_relationship_by_key.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 ---
 extensions:
   - "nautobot_design_builder.contrib.ext.LookupExtension"
 designs:
   - relationships:
-      - name: "Device to VLANS"
-        slug: "device-to-vlans"
+      - label: "Device to VLANS"
+        key: "device_to_vlans"
         type: "many-to-many"
         "!lookup:source_type":
           app_label: "dcim"
           model: "device"
         "!lookup:destination_type":
           app_label: "ipam"
           model: "vlan"
+
     manufacturers:
       - name: "manufacturer1"
 
     device_types:
       - manufacturer__name: "manufacturer1"
         model: "model name"
         u_height: 1
 
-    device_roles:
+    roles:
       - name: "device role"
-
-    sites:
-      - name: "site_1"
-        status__name: "Active"
+        content_types:
+          - "!get:app_label": "dcim"
+            "!get:model": "device"
+
+    location_types:
+      - name: "Site"
+        content_types:
+          - "!get:app_label": "dcim"
+            "!get:model": "device"
+        locations:
+          - name: "site_1"
+            status__name: "Active"
 
     vlans:
       - "!create_or_update:vid": 42
         name: "The Answer"
         status__name: "Active"
 
     devices:
       - name: "device_1"
-        site__name: "site_1"
+        location__name: "site_1"
         status__name: "Active"
         device_type__model: "model name"
-        device_role__name: "device role"
-        device-to-vlans:
+        role__name: "device role"
+        device_to_vlans:
           - "!get:vid": 42
           - vid: "43"
             name: "Better Answer"
             status__name: "Active"
 checks:
   - model_exists:
       model: "nautobot.ipam.models.VLAN"
       query: {vid: "43"}
 
-  - equal:
+  - count_equal:
       - model: "nautobot.extras.models.RelationshipAssociation"
-        query: {relationship__name: "Device to VLANS"}
+        query: {relationship__label: "Device to VLANS"}
         attribute: "destination"
       - model: "nautobot.ipam.models.VLAN"
```

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v1/device_primary_ip.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/nested_create.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -4,35 +4,46 @@
       - name: "manufacturer1"
 
     device_types:
       - manufacturer__name: "manufacturer1"
         model: "model name"
         u_height: 1
 
-    device_roles:
+    roles:
       - name: "device role"
+        content_types:
+          - "!get:app_label": "dcim"
+            "!get:model": "device"
 
-    sites:
-      - name: "site_1"
-        status__name: "Active"
+    location_types:
+      - name: "Site"
+        content_types:
+          - "!get:app_label": "dcim"
+            "!get:model": "device"
+        locations:
+          - name: "site_1"
+            status__name: "Active"
 
     devices:
       - name: "device_1"
-        site__name: "site_1"
+        location__name: "site_1"
         status__name: "Active"
         device_type__model: "model name"
-        device_role__name: "device role"
+        role__name: "device role"
         interfaces:
           - name: "Ethernet1/1"
             type: "virtual"
             status__name: "Active"
             description: "description for Ethernet1/1"
-            ip_addresses:
-              - address: "192.168.56.1/24"
-                status__name: "Active"
-        primary_ip4: {"!get:address": "192.168.56.1/24", "deferred": true}
 checks:
   - equal:
+      - model: "nautobot.dcim.models.Interface"
+        query: {name: "Ethernet1/1"}
+        attribute: "device"
+      - model: "nautobot.dcim.models.Device"
+        query: {name: "device_1"}
+  - equal:
       - model: "nautobot.dcim.models.Device"
         query: {name: "device_1"}
-        attribute: "primary_ip4.address.__str__"
-      - value: "192.168.56.1/24"
+        attribute: "location"
+      - model: "nautobot.dcim.models.Location"
+        query: {name: "site_1"}
```

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/ip_address_with_namespace.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/ip_address_with_namespace.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/nautobot_v2/prefixes.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/prefixes.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/simple_create.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/simple_create.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/tests/testdata/simple_update.yaml` & `nautobot_design_builder-2.0.0/nautobot_design_builder/tests/testdata/simple_update.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_design_builder-1.1.0/nautobot_design_builder/util.py` & `nautobot_design_builder-2.0.0/nautobot_design_builder/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 from types import ModuleType
 from typing import Iterator, Tuple, Type, TYPE_CHECKING
 from packaging.version import Version
 from packaging.specifiers import Specifier
 import yaml
 
 from django.conf import settings
+
 import nautobot
-from nautobot.extras.models import GitRepository
 
+from nautobot.apps.jobs import register_jobs
+from nautobot.extras.models import GitRepository
 
 from nautobot_design_builder import metadata
 
 if TYPE_CHECKING:
     from nautobot_design_builder.design_job import DesignJob
     from typing import Dict, List
 
@@ -291,21 +293,15 @@
     frame.f_globals["jobs"] = []
     for class_name, cls in designs.items():
         new_cls = type(class_name, (cls,), {})
         new_cls.__module__ = frame.f_globals["__name__"]
         frame.f_globals[class_name] = new_cls
         frame.f_globals["jobs"].append(new_cls)
 
-    if nautobot_version >= "2":
-        try:
-            from nautobot.apps.jobs import register_jobs  # pylint:disable=import-outside-toplevel
-
-            register_jobs(*frame.f_globals["jobs"])
-        except ImportError:
-            pass
+        register_jobs(*frame.f_globals["jobs"])
 
 
 def get_design_class(path: str, module_name: str, class_name: str) -> Type["DesignJob"]:
     """Retrieve the Python class using a filesystem path, module name and class name.
 
     Args:
         path (str): filesystem path to the package containing the module.
```

### Comparing `nautobot_design_builder-1.1.0/pyproject.toml` & `nautobot_design_builder-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-design-builder"
-version = "v1.1.0"
+version = "v2.0.0"
 description = "Nautobot app that uses design templates to easily create data objects in Nautobot with minimal input from a user."
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-app-design-builder"
 repository = "https://github.com/nautobot/nautobot-app-design-builder"
 keywords = ["nautobot", "nautobot-plugin"]
@@ -24,48 +24,47 @@
 packages = [
     { include = "nautobot_design_builder" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 # Used for local development
-nautobot = ">=1.6.0,<=2.9999"
-nautobot-bgp-models = { version = "*", optional = true }
+nautobot = ">=2.0.3,<=2.9999"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "*"
 black = "*"
 coverage = "*"
 django-debug-toolbar = "*"
 flake8 = "*"
 invoke = "*"
 ipython = "*"
+nautobot-bgp-models = "*"
 pydocstyle = "*"
 pylint = "*"
 pylint-django = "*"
 pylint-nautobot = "*"
 yamllint = "*"
 toml = "*"
 Markdown = "*"
 
 # Rendering docs to HTML
 mkdocs = "1.5.2"
 # Material for MkDocs theme
-mkdocs-material = "9.2.4"
+mkdocs-material = "9.1.15"
 # Render custom markdown for version added/changed/remove notes
 mkdocs-version-annotations = "1.0.0"
 # Automatic documentation from sources, for MkDocs
 mkdocstrings = "0.22.0"
 mkdocstrings-python = "1.5.2"
 gitpython = "^3.1.41"
 snakeviz = "^2.2.0"
 
 [tool.poetry.extras]
 nautobot = ["nautobot"]
-contrib = ["nautobot-bgp-models"]
 
 [tool.black]
 line-length = 120
 target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '''
 (
```

### Comparing `nautobot_design_builder-1.1.0/PKG-INFO` & `nautobot_design_builder-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-design-builder
-Version: 1.1.0
+Version: 2.0.0
 Summary: Nautobot app that uses design templates to easily create data objects in Nautobot with minimal input from a user.
 Home-page: https://github.com/nautobot/nautobot-app-design-builder
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: opensource@networktocode.com
 Requires-Python: >=3.8.1,<3.12
@@ -12,18 +12,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Provides-Extra: contrib
 Provides-Extra: nautobot
-Requires-Dist: nautobot (>=1.6.0,<=2.9999) ; extra == "nautobot"
-Requires-Dist: nautobot-bgp-models ; extra == "contrib"
+Requires-Dist: nautobot (>=2.0.3,<=2.9999) ; extra == "nautobot"
 Project-URL: Repository, https://github.com/nautobot/nautobot-app-design-builder
 Description-Content-Type: text/markdown
 
 # Nautobot Design Builder
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/nautobot/nautobot-app-design-builder/develop/docs/images/icon-nautobot-design-builder.png" class="logo" height="200px">
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 2.1 Name: nautobot-design-builder Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: nautobot-design-builder Version: 2.0.0 Summary:
 Nautobot app that uses design templates to easily create data objects in
 Nautobot with minimal input from a user. Home-page: https://github.com/
 nautobot/nautobot-app-design-builder License: Apache-2.0 Keywords:
 nautobot,nautobot-plugin Author: Network to Code, LLC Author-email:
 opensource@networktocode.com Requires-Python: >=3.8.1,<3.12 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.8 Provides-Extra: contrib Provides-Extra: nautobot
-Requires-Dist: nautobot (>=1.6.0,<=2.9999) ; extra == "nautobot" Requires-Dist:
-nautobot-bgp-models ; extra == "contrib" Project-URL: Repository, https://
+Language :: Python :: 3.8 Provides-Extra: nautobot Requires-Dist: nautobot
+(>=2.0.3,<=2.9999) ; extra == "nautobot" Project-URL: Repository, https://
 github.com/nautobot/nautobot-app-design-builder Description-Content-Type: text/
 markdown # Nautobot Design Builder
    [https://raw.githubusercontent.com/nautobot/nautobot-app-design-builder/
              develop/docs/images/icon-nautobot-design-builder.png]
   _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_a_p_p_-_d_e_s_i_g_n_-_b_u_i_l_d_e_r_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/
  _c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-_a_p_p_-
  _d_e_s_i_g_n_-_b_u_i_l_d_e_r_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_d_e_s_i_g_n_-_b_u_i_l_d_e_r_]
```

