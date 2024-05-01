# Comparing `tmp/pywaclient-1.6.5.tar.gz` & `tmp/pywaclient-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywaclient-1.6.5.tar", last modified: Fri Feb 16 18:31:45 2024, max compression
+gzip compressed data, was "dist/pywaclient-1.6.6.tar", last modified: Wed May  1 13:43:57 2024, max compression
```

## Comparing `pywaclient-1.6.5.tar` & `pywaclient-1.6.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 18:31:45.000000 pywaclient-1.6.5/
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-02-16 18:31:35.000000 pywaclient-1.6.5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      296 2024-02-16 18:31:35.000000 pywaclient-1.6.5/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-02-16 18:31:35.000000 pywaclient-1.6.5/LICENCE
--rw-r--r--   0 root         (0) root         (0)     7184 2024-02-16 18:31:45.000000 pywaclient-1.6.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6792 2024-02-16 18:31:35.000000 pywaclient-1.6.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 18:31:45.000000 pywaclient-1.6.5/pywaclient/
--rw-rw-rw-   0 root         (0) root         (0)      605 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3560 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 18:31:45.000000 pywaclient-1.6.5/pywaclient/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)     7038 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/articles.py
--rw-rw-rw-   0 root         (0) root         (0)     2242 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/block_templates.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/canvas.py
--rw-rw-rw-   0 root         (0) root         (0)      833 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/categories.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/chronicles.py
--rw-rw-rw-   0 root         (0) root         (0)      784 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/eras.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/histories.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/images.py
--rw-rw-rw-   0 root         (0) root         (0)     6023 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/manuscripts.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/map_marker_types.py
--rw-rw-rw-   0 root         (0) root         (0)     2900 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/maps.py
--rw-rw-rw-   0 root         (0) root         (0)     3076 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/notebooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/rpg_system.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/secrets.py
--rw-rw-rw-   0 root         (0) root         (0)      808 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/subscriber_groups.py
--rw-rw-rw-   0 root         (0) root         (0)     2282 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/timelines.py
--rw-rw-rw-   0 root         (0) root         (0)     2804 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/users.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/variables.py
--rw-rw-rw-   0 root         (0) root         (0)    15501 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/endpoints/worlds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 18:31:45.000000 pywaclient-1.6.5/pywaclient/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)     3488 2024-02-16 18:31:35.000000 pywaclient-1.6.5/pywaclient/exceptions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 18:31:45.000000 pywaclient-1.6.5/pywaclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7184 2024-02-16 18:31:45.000000 pywaclient-1.6.5/pywaclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1855 2024-02-16 18:31:45.000000 pywaclient-1.6.5/pywaclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-16 18:31:45.000000 pywaclient-1.6.5/pywaclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-02-16 18:31:45.000000 pywaclient-1.6.5/pywaclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-02-16 18:31:45.000000 pywaclient-1.6.5/pywaclient.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-02-16 18:31:35.000000 pywaclient-1.6.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-16 18:31:45.000000 pywaclient-1.6.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-02-16 18:31:35.000000 pywaclient-1.6.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 18:31:45.000000 pywaclient-1.6.5/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 18:31:45.000000 pywaclient-1.6.5/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)     1266 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/data/block.json
--rw-rw-rw-   0 root         (0) root         (0)     2469 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/data/form_schema.json
--rw-rw-rw-   0 root         (0) root         (0)     1015 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/init_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_article_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1638 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_block_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3926 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_block_template_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_block_template_part_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1836 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_canvas_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_category_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_character_relationships.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_chronicle_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_history_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_image_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3772 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_manuscript_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_map_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_notebook_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)      906 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_organization_diplomacy.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_parse_response.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_rpg_system_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     4154 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_secret_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1873 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_subscriber_group_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3542 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_timeline_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_user_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_variable_collection_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1679 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_variable_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     5133 2024-02-16 18:31:35.000000 pywaclient-1.6.5/tests/test_world_endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:43:57.000000 pywaclient-1.6.6/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-05-01 13:43:46.000000 pywaclient-1.6.6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-05-01 13:43:46.000000 pywaclient-1.6.6/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-01 13:43:46.000000 pywaclient-1.6.6/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     7184 2024-05-01 13:43:57.000000 pywaclient-1.6.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6792 2024-05-01 13:43:46.000000 pywaclient-1.6.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:43:57.000000 pywaclient-1.6.6/pywaclient/
+-rw-rw-rw-   0 root         (0) root         (0)      605 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3560 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:43:57.000000 pywaclient-1.6.6/pywaclient/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)     7038 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/articles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2242 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/block_templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/canvas.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/categories.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/chronicles.py
+-rw-rw-rw-   0 root         (0) root         (0)      784 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/eras.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/histories.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/images.py
+-rw-rw-rw-   0 root         (0) root         (0)     6023 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/manuscripts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/map_marker_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2900 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/maps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3076 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/notebooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/rpg_system.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/subscriber_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     2282 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/timelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/users.py
+-rw-rw-rw-   0 root         (0) root         (0)     2268 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/variables.py
+-rw-rw-rw-   0 root         (0) root         (0)    15501 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/endpoints/worlds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:43:57.000000 pywaclient-1.6.6/pywaclient/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)     3488 2024-05-01 13:43:46.000000 pywaclient-1.6.6/pywaclient/exceptions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:43:57.000000 pywaclient-1.6.6/pywaclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7184 2024-05-01 13:43:57.000000 pywaclient-1.6.6/pywaclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1855 2024-05-01 13:43:57.000000 pywaclient-1.6.6/pywaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 13:43:57.000000 pywaclient-1.6.6/pywaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-01 13:43:57.000000 pywaclient-1.6.6/pywaclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-01 13:43:57.000000 pywaclient-1.6.6/pywaclient.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-01 13:43:46.000000 pywaclient-1.6.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-01 13:43:57.000000 pywaclient-1.6.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-05-01 13:43:46.000000 pywaclient-1.6.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:43:57.000000 pywaclient-1.6.6/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:43:57.000000 pywaclient-1.6.6/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/data/block.json
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/data/form_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/init_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_article_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_block_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3926 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_block_template_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_block_template_part_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_canvas_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_category_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_character_relationships.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_chronicle_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_history_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_image_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3772 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_manuscript_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_map_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_notebook_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      906 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_organization_diplomacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_parse_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_rpg_system_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     4154 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_secret_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1873 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_subscriber_group_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3542 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_timeline_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_user_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2605 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_variable_collection_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_variable_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     5133 2024-05-01 13:43:46.000000 pywaclient-1.6.6/tests/test_world_endpoint.py
```

### Comparing `pywaclient-1.6.5/LICENCE` & `pywaclient-1.6.6/LICENCE`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/PKG-INFO` & `pywaclient-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaclient
-Version: 1.6.5
+Version: 1.6.6
 Summary: A simple wrapper client library for the World Anvil API.
 Home-page: https://gitlab.com/SoulLink/world-anvil-api-client
 Author: Jonas Waeber
 Author-email: jonaswaeber@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pywaclient-1.6.5/README.md` & `pywaclient-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/__init__.py` & `pywaclient-1.6.6/pywaclient/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/api.py` & `pywaclient-1.6.6/pywaclient/api.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/__init__.py` & `pywaclient-1.6.6/pywaclient/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/articles.py` & `pywaclient-1.6.6/pywaclient/endpoints/articles.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/block_templates.py` & `pywaclient-1.6.6/pywaclient/endpoints/block_templates.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/blocks.py` & `pywaclient-1.6.6/pywaclient/endpoints/blocks.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/canvas.py` & `pywaclient-1.6.6/pywaclient/endpoints/canvas.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/categories.py` & `pywaclient-1.6.6/pywaclient/endpoints/categories.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/chronicles.py` & `pywaclient-1.6.6/pywaclient/endpoints/chronicles.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/eras.py` & `pywaclient-1.6.6/pywaclient/endpoints/eras.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/histories.py` & `pywaclient-1.6.6/pywaclient/endpoints/histories.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/images.py` & `pywaclient-1.6.6/pywaclient/endpoints/images.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/manuscripts.py` & `pywaclient-1.6.6/pywaclient/endpoints/manuscripts.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/map_marker_types.py` & `pywaclient-1.6.6/pywaclient/endpoints/map_marker_types.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/maps.py` & `pywaclient-1.6.6/pywaclient/endpoints/maps.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/notebooks.py` & `pywaclient-1.6.6/pywaclient/endpoints/notebooks.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/rpg_system.py` & `pywaclient-1.6.6/pywaclient/endpoints/rpg_system.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/secrets.py` & `pywaclient-1.6.6/pywaclient/endpoints/secrets.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/subscriber_groups.py` & `pywaclient-1.6.6/pywaclient/endpoints/subscriber_groups.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/timelines.py` & `pywaclient-1.6.6/pywaclient/endpoints/timelines.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/users.py` & `pywaclient-1.6.6/pywaclient/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/variables.py` & `pywaclient-1.6.6/pywaclient/endpoints/variables.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,27 +25,24 @@
 class VariableCollectionCrudEndpoint(CrudEndpoint):
 
     def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'variablecollection')
         self.variable = VariableCrudEndpoint(client)
         self.path_variables = f"{self.path}/variables"
 
-    def variables(self, world_id: str, variable_collection_id: str, complete: bool = True, limit: int = 50,
+    def variables(self, variable_collection_id: str, complete: bool = True, limit: int = 50,
                   offset: int = 0) -> Iterable[Dict[str, Any]]:
         """
         List all variables by a category given, filtered with a limit of entities shown and an offset.
 
-        :param world_id:                The id of the world the variables should be returned from.
         :param variable_collection_id:  The id of the variable collection to return the variables from.
         :param complete                 Ignore limit and offset and return all the variables as an iterable. Will fetch a new batch
                                         every 50 variables.
         :param limit:                   Determines how many variables are returned. Value between 1 and 50.
         :param offset:                  Determines the offset at which variables are returned. Has to be a positive integer.
         :return:
         """
         if complete:
-            return self._scroll_collection(self.path_variables, {'id': world_id}, 'entities', 'variableCollection',
-                                           variable_collection_id)
+            return self._scroll_collection(self.path_variables, {'id': variable_collection_id}, 'entities')
         return self._post_request(self.path_variables,
-                                  {'id': world_id},
-                                  {'limit': limit, 'offset': offset,
-                                   'variableCollection': {'id': variable_collection_id}})['entities']
+                                  {'id': variable_collection_id},
+                                  {'limit': limit, 'offset': offset})['entities']
```

### Comparing `pywaclient-1.6.5/pywaclient/endpoints/worlds.py` & `pywaclient-1.6.6/pywaclient/endpoints/worlds.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient/exceptions/__init__.py` & `pywaclient-1.6.6/pywaclient/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/pywaclient.egg-info/PKG-INFO` & `pywaclient-1.6.6/pywaclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaclient
-Version: 1.6.5
+Version: 1.6.6
 Summary: A simple wrapper client library for the World Anvil API.
 Home-page: https://gitlab.com/SoulLink/world-anvil-api-client
 Author: Jonas Waeber
 Author-email: jonaswaeber@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pywaclient-1.6.5/pywaclient.egg-info/SOURCES.txt` & `pywaclient-1.6.6/pywaclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/setup.py` & `pywaclient-1.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/data/block.json` & `pywaclient-1.6.6/tests/data/block.json`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/data/form_schema.json` & `pywaclient-1.6.6/tests/data/form_schema.json`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/init_client.py` & `pywaclient-1.6.6/tests/init_client.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_article_endpoint.py` & `pywaclient-1.6.6/tests/test_article_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_block_endpoint.py` & `pywaclient-1.6.6/tests/test_block_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_block_template_endpoint.py` & `pywaclient-1.6.6/tests/test_block_template_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_block_template_part_endpoint.py` & `pywaclient-1.6.6/tests/test_block_template_part_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_canvas_endpoint.py` & `pywaclient-1.6.6/tests/test_canvas_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_category_endpoint.py` & `pywaclient-1.6.6/tests/test_category_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_character_relationships.py` & `pywaclient-1.6.6/tests/test_character_relationships.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_chronicle_endpoint.py` & `pywaclient-1.6.6/tests/test_chronicle_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_history_endpoint.py` & `pywaclient-1.6.6/tests/test_history_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_image_endpoint.py` & `pywaclient-1.6.6/tests/test_image_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_manuscript_endpoint.py` & `pywaclient-1.6.6/tests/test_manuscript_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_map_endpoint.py` & `pywaclient-1.6.6/tests/test_map_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_notebook_endpoint.py` & `pywaclient-1.6.6/tests/test_notebook_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_organization_diplomacy.py` & `pywaclient-1.6.6/tests/test_organization_diplomacy.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_parse_response.py` & `pywaclient-1.6.6/tests/test_parse_response.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_rpg_system_endpoint.py` & `pywaclient-1.6.6/tests/test_rpg_system_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_secret_endpoint.py` & `pywaclient-1.6.6/tests/test_secret_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_subscriber_group_endpoint.py` & `pywaclient-1.6.6/tests/test_subscriber_group_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_timeline_endpoint.py` & `pywaclient-1.6.6/tests/test_timeline_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_user_endpoint.py` & `pywaclient-1.6.6/tests/test_user_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.5/tests/test_variable_collection_endpoint.py` & `pywaclient-1.6.6/tests/test_variable_endpoint.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,47 +20,32 @@
             "title": "Variables Collection",
             "description": "All variables used in this world.",
             "world": world_id,
             "prefix": "test-prefix",
             "state": "public"
         }
     )
-    test_variableCollection_2 = client.variable_collection.put(
+    test_variable_1 = client.variable.put(
         {
-            "title": "Variables Collection 2",
-            "description": "All variables used in this world.",
-            "world": world_id,
-            "prefix": "test-prefix-2",
-            "state": "public"
+            "k": "key",
+            "v": "value",
+            "type": "string",
+            "collection": test_variableCollection_1['id'],
+            "world": world_id
         }
     )
-    response_patch_variableCollection_2 = client.variable_collection.patch(
-        test_variableCollection_2['id'],
+    response_patch_variable_1 = client.variable.patch(
+        test_variable_1['id'],
         {
-            'description': 'Update this variable collection with a new excerpt.'
+            'v': 'This is a new value for the variable.'
         }
     )
 
-    full_test_variableCollection_2 = client.variable_collection.get(
-        test_variableCollection_2['id'],
+    full_test_variable_1 = client.variable.get(
+        test_variable_1['id'],
         2
     )
 
-    assert full_test_variableCollection_2['description'] == 'Update this variable collection with a new excerpt.'
-
-    for i in range(50):
-        test_variable_1 = client.variable.put(
-            {
-                "k": str(i),
-                "t": "title",
-                "v": "value",
-                "type": "string",
-                "collection": test_variableCollection_1['id'],
-                "world": world_id
-            }
-        )
-
-    for x in client.variable_collection.variables(world_id, test_variableCollection_1['id']):
-        print(x)
+    assert full_test_variable_1['v'] == 'This is a new value for the variable.'
 
-    # client.variableCollection.delete(test_variableCollection_1['id'])
-    client.variable_collection.delete(test_variableCollection_2['id'])
+    client.variable_collection.delete(test_variableCollection_1['id'])
+    client.variable.delete(test_variable_1['id'])
```

### Comparing `pywaclient-1.6.5/tests/test_world_endpoint.py` & `pywaclient-1.6.6/tests/test_world_endpoint.py`

 * *Files identical despite different names*

