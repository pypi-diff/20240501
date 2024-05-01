# Comparing `tmp/django-haystack-3.2.dev0.tar.gz` & `tmp/django_haystack-3.3b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-haystack-3.2.dev0.tar", last modified: Thu Mar 17 23:46:06 2022, max compression
+gzip compressed data, was "django_haystack-3.3b2.tar", last modified: Wed May  1 20:46:23 2024, max compression
```

## Comparing `django-haystack-3.2.dev0.tar` & `django_haystack-3.3b2.tar`

### file list

```diff
@@ -1,297 +1,299 @@
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.885418 django-haystack-3.2.dev0/
--rw-r--r--   0 cadams     (501) staff       (20)      506 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/.editorconfig
--rw-r--r--   0 cadams     (501) staff       (20)     6234 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/.gitchangelog.rc
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.852016 django-haystack-3.2.dev0/.github/
--rw-r--r--   0 cadams     (501) staff       (20)      312 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/.github/issue_template.md
--rw-r--r--   0 cadams     (501) staff       (20)      536 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/.github/pull_request_template.md
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.852643 django-haystack-3.2.dev0/.github/workflows/
--rw-r--r--   0 cadams     (501) staff       (20)      571 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 cadams     (501) staff       (20)      349 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/.github/workflows/docs.yml
--rw-r--r--   0 cadams     (501) staff       (20)      441 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/.github/workflows/flake8.yml
--rw-r--r--   0 cadams     (501) staff       (20)      495 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/.github/workflows/publish.yml
--rw-r--r--   0 cadams     (501) staff       (20)     1749 2022-03-17 23:44:59.000000 django-haystack-3.2.dev0/.github/workflows/test.yml
--rw-r--r--   0 cadams     (501) staff       (20)      196 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/.gitignore
--rw-r--r--   0 cadams     (501) staff       (20)     1023 2022-02-03 00:15:33.000000 django-haystack-3.2.dev0/.pre-commit-config.yaml
--rw-r--r--   0 cadams     (501) staff       (20)     8312 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/AUTHORS
--rw-r--r--   0 cadams     (501) staff       (20)     4119 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/CONTRIBUTING.md
--rw-r--r--   0 cadams     (501) staff       (20)     1607 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/LICENSE
--rw-r--r--   0 cadams     (501) staff       (20)      126 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/MANIFEST.in
--rw-r--r--   0 cadams     (501) staff       (20)     4231 2022-03-17 23:46:06.885512 django-haystack-3.2.dev0/PKG-INFO
--rw-r--r--   0 cadams     (501) staff       (20)     2566 2022-03-17 23:44:59.000000 django-haystack-3.2.dev0/README.rst
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.853243 django-haystack-3.2.dev0/django_haystack.egg-info/
--rw-r--r--   0 cadams     (501) staff       (20)     4231 2022-03-17 23:46:06.000000 django-haystack-3.2.dev0/django_haystack.egg-info/PKG-INFO
--rw-r--r--   0 cadams     (501) staff       (20)     8455 2022-03-17 23:46:06.000000 django-haystack-3.2.dev0/django_haystack.egg-info/SOURCES.txt
--rw-r--r--   0 cadams     (501) staff       (20)        1 2022-03-17 23:46:06.000000 django-haystack-3.2.dev0/django_haystack.egg-info/dependency_links.txt
--rw-r--r--   0 cadams     (501) staff       (20)        1 2022-03-17 23:46:06.000000 django-haystack-3.2.dev0/django_haystack.egg-info/not-zip-safe
--rw-r--r--   0 cadams     (501) staff       (20)       49 2022-03-17 23:46:06.000000 django-haystack-3.2.dev0/django_haystack.egg-info/requires.txt
--rw-r--r--   0 cadams     (501) staff       (20)        9 2022-03-17 23:46:06.000000 django-haystack-3.2.dev0/django_haystack.egg-info/top_level.txt
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.860072 django-haystack-3.2.dev0/docs/
--rw-r--r--   0 cadams     (501) staff       (20)     2492 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/Makefile
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.860345 django-haystack-3.2.dev0/docs/_build/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/_build/.gitignore
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.860453 django-haystack-3.2.dev0/docs/_static/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/_static/.gitignore
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.860547 django-haystack-3.2.dev0/docs/_templates/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/_templates/.gitignore
--rw-r--r--   0 cadams     (501) staff       (20)     1323 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/admin.rst
--rw-r--r--   0 cadams     (501) staff       (20)     1704 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/architecture_overview.rst
--rw-r--r--   0 cadams     (501) staff       (20)     7500 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/autocomplete.rst
--rw-r--r--   0 cadams     (501) staff       (20)     4268 2022-02-03 00:15:33.000000 django-haystack-3.2.dev0/docs/backend_support.rst
--rw-r--r--   0 cadams     (501) staff       (20)    11360 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/best_practices.rst
--rw-r--r--   0 cadams     (501) staff       (20)     3746 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/boost.rst
--rw-r--r--   0 cadams     (501) staff       (20)   186657 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/changelog.rst
--rw-r--r--   0 cadams     (501) staff       (20)     6665 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/conf.py
--rw-r--r--   0 cadams     (501) staff       (20)     5426 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/contributing.rst
--rw-r--r--   0 cadams     (501) staff       (20)      820 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/creating_new_backends.rst
--rw-r--r--   0 cadams     (501) staff       (20)     4763 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/debugging.rst
--rw-r--r--   0 cadams     (501) staff       (20)    11391 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/faceting.rst
--rw-r--r--   0 cadams     (501) staff       (20)     4882 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/faq.rst
--rw-r--r--   0 cadams     (501) staff       (20)     3239 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/glossary.rst
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.860781 django-haystack-3.2.dev0/docs/haystack_theme/
--rw-r--r--   0 cadams     (501) staff       (20)      631 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/haystack_theme/layout.html
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.860917 django-haystack-3.2.dev0/docs/haystack_theme/static/
--rw-r--r--   0 cadams     (501) staff       (20)     1326 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/haystack_theme/static/documentation.css
--rw-r--r--   0 cadams     (501) staff       (20)       24 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/haystack_theme/theme.conf
--rw-r--r--   0 cadams     (501) staff       (20)     3184 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/highlighting.rst
--rw-r--r--   0 cadams     (501) staff       (20)     2800 2022-02-03 00:15:33.000000 django-haystack-3.2.dev0/docs/index.rst
--rw-r--r--   0 cadams     (501) staff       (20)     5136 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/inputtypes.rst
--rw-r--r--   0 cadams     (501) staff       (20)     8039 2022-02-03 00:15:33.000000 django-haystack-3.2.dev0/docs/installing_search_engines.rst
--rw-r--r--   0 cadams     (501) staff       (20)    10024 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/management_commands.rst
--rw-r--r--   0 cadams     (501) staff       (20)    10121 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/migration_from_1_to_2.rst
--rw-r--r--   0 cadams     (501) staff       (20)     7264 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/multiple_index.rst
--rw-r--r--   0 cadams     (501) staff       (20)     3162 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/other_apps.rst
--rw-r--r--   0 cadams     (501) staff       (20)     1609 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/python3.rst
--rw-r--r--   0 cadams     (501) staff       (20)     2628 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/rich_content_extraction.rst
--rw-r--r--   0 cadams     (501) staff       (20)     2379 2022-03-17 23:44:53.000000 django-haystack-3.2.dev0/docs/running_tests.rst
--rw-r--r--   0 cadams     (501) staff       (20)     3853 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/searchbackend_api.rst
--rw-r--r--   0 cadams     (501) staff       (20)     7427 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/searchfield_api.rst
--rw-r--r--   0 cadams     (501) staff       (20)    22347 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/searchindex_api.rst
--rw-r--r--   0 cadams     (501) staff       (20)     8860 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/searchquery_api.rst
--rw-r--r--   0 cadams     (501) staff       (20)    31840 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/searchqueryset_api.rst
--rw-r--r--   0 cadams     (501) staff       (20)     1889 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/searchresult_api.rst
--rw-r--r--   0 cadams     (501) staff       (20)     8374 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/settings.rst
--rw-r--r--   0 cadams     (501) staff       (20)     4822 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/signal_processors.rst
--rw-r--r--   0 cadams     (501) staff       (20)    14261 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/spatial.rst
--rw-r--r--   0 cadams     (501) staff       (20)     2086 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/templatetags.rst
--rw-r--r--   0 cadams     (501) staff       (20)      723 2022-02-03 00:15:33.000000 django-haystack-3.2.dev0/docs/toc.rst
--rw-r--r--   0 cadams     (501) staff       (20)    15044 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/tutorial.rst
--rw-r--r--   0 cadams     (501) staff       (20)      343 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/utils.rst
--rw-r--r--   0 cadams     (501) staff       (20)    15471 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/docs/views_and_forms.rst
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.861162 django-haystack-3.2.dev0/example_project/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/example_project/__init__.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.861520 django-haystack-3.2.dev0/example_project/bare_bones_app/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/example_project/bare_bones_app/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)      506 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/example_project/bare_bones_app/models.py
--rw-r--r--   0 cadams     (501) staff       (20)      394 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/example_project/bare_bones_app/search_indexes.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.861944 django-haystack-3.2.dev0/example_project/regular_app/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/example_project/regular_app/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)     1230 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/example_project/regular_app/models.py
--rw-r--r--   0 cadams     (501) staff       (20)     1234 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/example_project/regular_app/search_indexes.py
--rw-r--r--   0 cadams     (501) staff       (20)     1295 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/example_project/settings.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.841926 django-haystack-3.2.dev0/example_project/templates/
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.841968 django-haystack-3.2.dev0/example_project/templates/search/
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.842059 django-haystack-3.2.dev0/example_project/templates/search/indexes/
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.862095 django-haystack-3.2.dev0/example_project/templates/search/indexes/bare_bones_app/
--rw-r--r--   0 cadams     (501) staff       (20)       35 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/example_project/templates/search/indexes/bare_bones_app/cat_text.txt
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.862232 django-haystack-3.2.dev0/example_project/templates/search/indexes/regular_app/
--rw-r--r--   0 cadams     (501) staff       (20)      125 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/example_project/templates/search/indexes/regular_app/dog_text.txt
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.865344 django-haystack-3.2.dev0/haystack/
--rw-r--r--   0 cadams     (501) staff       (20)     2585 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)     6183 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/admin.py
--rw-r--r--   0 cadams     (501) staff       (20)      963 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/apps.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.867059 django-haystack-3.2.dev0/haystack/backends/
--rw-r--r--   0 cadams     (501) staff       (20)    36622 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/backends/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)    13882 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/backends/elasticsearch2_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)    17457 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/backends/elasticsearch5_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)    20528 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/backends/elasticsearch7_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)    39695 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/backends/elasticsearch_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)     3927 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/backends/simple_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)    35754 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/backends/solr_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)    38346 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/backends/whoosh_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)     1612 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/constants.py
--rw-r--r--   0 cadams     (501) staff       (20)     1138 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/exceptions.py
--rw-r--r--   0 cadams     (501) staff       (20)    15708 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/fields.py
--rw-r--r--   0 cadams     (501) staff       (20)     3994 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/forms.py
--rw-r--r--   0 cadams     (501) staff       (20)     3992 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/generic_views.py
--rw-r--r--   0 cadams     (501) staff       (20)    18702 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/indexes.py
--rw-r--r--   0 cadams     (501) staff       (20)     4452 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/inputs.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.867248 django-haystack-3.2.dev0/haystack/management/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/management/__init__.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.867978 django-haystack-3.2.dev0/haystack/management/commands/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/management/commands/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)     7236 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/management/commands/build_solr_schema.py
--rw-r--r--   0 cadams     (501) staff       (20)     2265 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/management/commands/clear_index.py
--rw-r--r--   0 cadams     (501) staff       (20)      766 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/management/commands/haystack_info.py
--rw-r--r--   0 cadams     (501) staff       (20)     2177 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/management/commands/rebuild_index.py
--rw-r--r--   0 cadams     (501) staff       (20)    16129 2022-02-03 00:15:33.000000 django-haystack-3.2.dev0/haystack/management/commands/update_index.py
--rw-r--r--   0 cadams     (501) staff       (20)     3569 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/manager.py
--rw-r--r--   0 cadams     (501) staff       (20)     8819 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/models.py
--rw-r--r--   0 cadams     (501) staff       (20)     2823 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/panels.py
--rw-r--r--   0 cadams     (501) staff       (20)    26126 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/query.py
--rw-r--r--   0 cadams     (501) staff       (20)      272 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/routers.py
--rw-r--r--   0 cadams     (501) staff       (20)     3054 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/signals.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.842443 django-haystack-3.2.dev0/haystack/templates/
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.868159 django-haystack-3.2.dev0/haystack/templates/panels/
--rw-r--r--   0 cadams     (501) staff       (20)     1353 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/templates/panels/haystack.html
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.868494 django-haystack-3.2.dev0/haystack/templates/search_configuration/
--rw-r--r--   0 cadams     (501) staff       (20)    58455 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/templates/search_configuration/schema.xml
--rw-r--r--   0 cadams     (501) staff       (20)    57423 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/templates/search_configuration/solrconfig.xml
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.868954 django-haystack-3.2.dev0/haystack/templatetags/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/templatetags/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)     4320 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/templatetags/highlight.py
--rw-r--r--   0 cadams     (501) staff       (20)     3438 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/templatetags/more_like_this.py
--rw-r--r--   0 cadams     (501) staff       (20)      132 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/urls.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.869727 django-haystack-3.2.dev0/haystack/utils/
--rw-r--r--   0 cadams     (501) staff       (20)     2519 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/utils/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)     1030 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/utils/app_loading.py
--rw-r--r--   0 cadams     (501) staff       (20)     2036 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/utils/geo.py
--rw-r--r--   0 cadams     (501) staff       (20)     5645 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/utils/highlighting.py
--rw-r--r--   0 cadams     (501) staff       (20)    12818 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/utils/loading.py
--rw-r--r--   0 cadams     (501) staff       (20)      468 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/utils/log.py
--rw-r--r--   0 cadams     (501) staff       (20)      150 2022-03-17 23:46:06.000000 django-haystack-3.2.dev0/haystack/version.py
--rw-r--r--   0 cadams     (501) staff       (20)     6925 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/haystack/views.py
--rw-r--r--   0 cadams     (501) staff       (20)      302 2022-02-03 00:12:35.000000 django-haystack-3.2.dev0/pyproject.toml
--rw-r--r--   0 cadams     (501) staff       (20)      200 2022-03-17 23:46:06.886018 django-haystack-3.2.dev0/setup.cfg
--rw-r--r--   0 cadams     (501) staff       (20)     1930 2022-03-17 23:44:59.000000 django-haystack-3.2.dev0/setup.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.873181 django-haystack-3.2.dev0/test_haystack/
--rw-r--r--   0 cadams     (501) staff       (20)      489 2022-03-17 23:44:53.000000 django-haystack-3.2.dev0/test_haystack/__init__.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.873912 django-haystack-3.2.dev0/test_haystack/core/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)      307 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/admin.py
--rw-r--r--   0 cadams     (501) staff       (20)      350 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/custom_identifier.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.874135 django-haystack-3.2.dev0/test_haystack/core/fixtures/
--rw-r--r--   0 cadams     (501) staff       (20)     1826 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/fixtures/base_data.json
--rw-r--r--   0 cadams     (501) staff       (20)    15018 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/fixtures/bulk_data.json
--rw-r--r--   0 cadams     (501) staff       (20)     2732 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/models.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.874437 django-haystack-3.2.dev0/test_haystack/core/templates/
--rw-r--r--   0 cadams     (501) staff       (20)       26 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/templates/404.html
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/templates/base.html
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.874551 django-haystack-3.2.dev0/test_haystack/core/templates/search/
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.874785 django-haystack-3.2.dev0/test_haystack/core/templates/search/indexes/
--rw-r--r--   0 cadams     (501) staff       (20)        5 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/templates/search/indexes/bar.txt
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.875429 django-haystack-3.2.dev0/test_haystack/core/templates/search/indexes/core/
--rw-r--r--   0 cadams     (501) staff       (20)       25 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/templates/search/indexes/core/mockmodel_content.txt
--rw-r--r--   0 cadams     (501) staff       (20)       24 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/templates/search/indexes/core/mockmodel_extra.txt
--rw-r--r--   0 cadams     (501) staff       (20)       25 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/templates/search/indexes/core/mockmodel_template.txt
--rw-r--r--   0 cadams     (501) staff       (20)       25 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/templates/search/indexes/core/mockmodel_text.txt
--rw-r--r--   0 cadams     (501) staff       (20)        5 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/templates/search/indexes/foo.txt
--rw-r--r--   0 cadams     (501) staff       (20)       26 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/templates/search/search.html
--rw-r--r--   0 cadams     (501) staff       (20)       29 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/templates/test_suggestion.html
--rw-r--r--   0 cadams     (501) staff       (20)      813 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/core/urls.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.875748 django-haystack-3.2.dev0/test_haystack/discovery/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/discovery/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)      338 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/discovery/models.py
--rw-r--r--   0 cadams     (501) staff       (20)      394 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/discovery/search_indexes.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.843076 django-haystack-3.2.dev0/test_haystack/discovery/templates/
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.843112 django-haystack-3.2.dev0/test_haystack/discovery/templates/search/
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.875882 django-haystack-3.2.dev0/test_haystack/discovery/templates/search/indexes/
--rw-r--r--   0 cadams     (501) staff       (20)       37 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/discovery/templates/search/indexes/bar_text.txt
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.876590 django-haystack-3.2.dev0/test_haystack/elasticsearch2_tests/
--rw-r--r--   0 cadams     (501) staff       (20)      942 2022-03-17 23:44:53.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch2_tests/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)    65707 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch2_tests/test_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)     3508 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch2_tests/test_inputs.py
--rw-r--r--   0 cadams     (501) staff       (20)     9966 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch2_tests/test_query.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.877159 django-haystack-3.2.dev0/test_haystack/elasticsearch5_tests/
--rw-r--r--   0 cadams     (501) staff       (20)      942 2022-03-17 23:44:53.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch5_tests/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)    65708 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch5_tests/test_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)     3508 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch5_tests/test_inputs.py
--rw-r--r--   0 cadams     (501) staff       (20)     8393 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch5_tests/test_query.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.877980 django-haystack-3.2.dev0/test_haystack/elasticsearch7_tests/
--rw-r--r--   0 cadams     (501) staff       (20)      942 2022-03-17 23:44:53.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch7_tests/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)    67491 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch7_tests/test_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)     3508 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch7_tests/test_inputs.py
--rw-r--r--   0 cadams     (501) staff       (20)     8401 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch7_tests/test_query.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.878574 django-haystack-3.2.dev0/test_haystack/elasticsearch_tests/
--rw-r--r--   0 cadams     (501) staff       (20)     1130 2022-03-17 23:44:53.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch_tests/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)    68913 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch_tests/test_elasticsearch_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)    10955 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch_tests/test_elasticsearch_query.py
--rw-r--r--   0 cadams     (501) staff       (20)     3507 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/elasticsearch_tests/test_inputs.py
--rw-r--r--   0 cadams     (501) staff       (20)     5356 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/mocks.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.879154 django-haystack-3.2.dev0/test_haystack/multipleindex/
--rw-r--r--   0 cadams     (501) staff       (20)      539 2022-03-17 23:44:53.000000 django-haystack-3.2.dev0/test_haystack/multipleindex/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)      338 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/multipleindex/models.py
--rw-r--r--   0 cadams     (501) staff       (20)      225 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/multipleindex/routers.py
--rw-r--r--   0 cadams     (501) staff       (20)      808 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/multipleindex/search_indexes.py
--rw-r--r--   0 cadams     (501) staff       (20)    12215 2022-03-17 23:44:53.000000 django-haystack-3.2.dev0/test_haystack/multipleindex/tests.py
--rw-r--r--   0 cadams     (501) staff       (20)      352 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/results_per_page_urls.py
--rwxr-xr-x   0 cadams     (501) staff       (20)      561 2022-03-17 23:44:53.000000 django-haystack-3.2.dev0/test_haystack/run_tests.py
--rw-r--r--   0 cadams     (501) staff       (20)     4101 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/settings.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.879608 django-haystack-3.2.dev0/test_haystack/simple_tests/
--rw-r--r--   0 cadams     (501) staff       (20)       58 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/simple_tests/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)      764 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/simple_tests/search_indexes.py
--rw-r--r--   0 cadams     (501) staff       (20)     8670 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/simple_tests/test_simple_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)     1221 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/simple_tests/test_simple_query.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.880720 django-haystack-3.2.dev0/test_haystack/solr_tests/
--rw-r--r--   0 cadams     (501) staff       (20)      122 2022-03-17 23:44:53.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/__init__.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.880852 django-haystack-3.2.dev0/test_haystack/solr_tests/content_extraction/
--rw-r--r--   0 cadams     (501) staff       (20)    48184 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/content_extraction/test.pdf
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.881613 django-haystack-3.2.dev0/test_haystack/solr_tests/server/
--rw-r--r--   0 cadams     (501) staff       (20)       11 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/server/.gitignore
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.881935 django-haystack-3.2.dev0/test_haystack/solr_tests/server/confdir/
--rw-r--r--   0 cadams     (501) staff       (20)    60187 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/server/confdir/schema.xml
--rw-r--r--   0 cadams     (501) staff       (20)    57364 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/server/confdir/solrconfig.xml
--rwxr-xr-x   0 cadams     (501) staff       (20)     1684 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/server/get-solr-download-url.py
--rwxr-xr-x   0 cadams     (501) staff       (20)     2125 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/server/start-solr-test-server.sh
--rwxr-xr-x   0 cadams     (501) staff       (20)      915 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/server/wait-for-solr
--rw-r--r--   0 cadams     (501) staff       (20)     2721 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/test_admin.py
--rw-r--r--   0 cadams     (501) staff       (20)     3738 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/test_inputs.py
--rw-r--r--   0 cadams     (501) staff       (20)    61151 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/test_solr_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)    12753 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/test_solr_management_commands.py
--rw-r--r--   0 cadams     (501) staff       (20)     9812 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/test_solr_query.py
--rw-r--r--   0 cadams     (501) staff       (20)     2493 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/solr_tests/test_templatetags.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.882471 django-haystack-3.2.dev0/test_haystack/spatial/
--rw-r--r--   0 cadams     (501) staff       (20)       63 2022-03-17 23:44:53.000000 django-haystack-3.2.dev0/test_haystack/spatial/__init__.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.882593 django-haystack-3.2.dev0/test_haystack/spatial/fixtures/
--rw-r--r--   0 cadams     (501) staff       (20)     3179 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/spatial/fixtures/sample_spatial_data.json
--rw-r--r--   0 cadams     (501) staff       (20)      986 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/spatial/models.py
--rw-r--r--   0 cadams     (501) staff       (20)      736 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/spatial/search_indexes.py
--rw-r--r--   0 cadams     (501) staff       (20)    11273 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/spatial/test_spatial.py
--rw-r--r--   0 cadams     (501) staff       (20)     3503 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_altered_internal_names.py
--rw-r--r--   0 cadams     (501) staff       (20)     2356 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_loading.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.883282 django-haystack-3.2.dev0/test_haystack/test_app_using_appconfig/
--rw-r--r--   0 cadams     (501) staff       (20)       73 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_using_appconfig/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)      179 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_using_appconfig/apps.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.883540 django-haystack-3.2.dev0/test_haystack/test_app_using_appconfig/migrations/
--rw-r--r--   0 cadams     (501) staff       (20)      655 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_using_appconfig/migrations/0001_initial.py
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_using_appconfig/migrations/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)      113 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_using_appconfig/models.py
--rw-r--r--   0 cadams     (501) staff       (20)      272 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_using_appconfig/search_indexes.py
--rw-r--r--   0 cadams     (501) staff       (20)      346 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_using_appconfig/tests.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.883623 django-haystack-3.2.dev0/test_haystack/test_app_with_hierarchy/
--rw-r--r--   0 cadams     (501) staff       (20)       78 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_with_hierarchy/__init__.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.883744 django-haystack-3.2.dev0/test_haystack/test_app_with_hierarchy/contrib/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_with_hierarchy/contrib/__init__.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.883827 django-haystack-3.2.dev0/test_haystack/test_app_with_hierarchy/contrib/django/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_with_hierarchy/contrib/django/__init__.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.883992 django-haystack-3.2.dev0/test_haystack/test_app_with_hierarchy/contrib/django/hierarchal_app_django/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_with_hierarchy/contrib/django/hierarchal_app_django/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)      214 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_with_hierarchy/contrib/django/hierarchal_app_django/models.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.884302 django-haystack-3.2.dev0/test_haystack/test_app_without_models/
--rw-r--r--   0 cadams     (501) staff       (20)        0 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_without_models/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)      131 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_without_models/urls.py
--rw-r--r--   0 cadams     (501) staff       (20)       95 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_app_without_models/views.py
--rw-r--r--   0 cadams     (501) staff       (20)     2480 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_backends.py
--rw-r--r--   0 cadams     (501) staff       (20)     2119 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_discovery.py
--rw-r--r--   0 cadams     (501) staff       (20)    23313 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_fields.py
--rw-r--r--   0 cadams     (501) staff       (20)     6322 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_forms.py
--rw-r--r--   0 cadams     (501) staff       (20)     2523 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_generic_views.py
--rw-r--r--   0 cadams     (501) staff       (20)    32476 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_indexes.py
--rw-r--r--   0 cadams     (501) staff       (20)     3522 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_inputs.py
--rw-r--r--   0 cadams     (501) staff       (20)    15245 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_loading.py
--rw-r--r--   0 cadams     (501) staff       (20)     5159 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_management_commands.py
--rw-r--r--   0 cadams     (501) staff       (20)     9533 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_managers.py
--rw-r--r--   0 cadams     (501) staff       (20)     8275 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_models.py
--rw-r--r--   0 cadams     (501) staff       (20)    37888 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_query.py
--rw-r--r--   0 cadams     (501) staff       (20)     4922 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_templatetags.py
--rw-r--r--   0 cadams     (501) staff       (20)    15305 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_utils.py
--rw-r--r--   0 cadams     (501) staff       (20)    10887 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/test_views.py
--rw-r--r--   0 cadams     (501) staff       (20)      469 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/utils.py
-drwxr-xr-x   0 cadams     (501) staff       (20)        0 2022-03-17 23:46:06.885256 django-haystack-3.2.dev0/test_haystack/whoosh_tests/
--rw-r--r--   0 cadams     (501) staff       (20)       58 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/whoosh_tests/__init__.py
--rw-r--r--   0 cadams     (501) staff       (20)     1301 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/whoosh_tests/test_forms.py
--rw-r--r--   0 cadams     (501) staff       (20)     3281 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/whoosh_tests/test_inputs.py
--rw-r--r--   0 cadams     (501) staff       (20)    55237 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/whoosh_tests/test_whoosh_backend.py
--rw-r--r--   0 cadams     (501) staff       (20)     3753 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/whoosh_tests/test_whoosh_management_commands.py
--rw-r--r--   0 cadams     (501) staff       (20)     7513 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/whoosh_tests/test_whoosh_query.py
--rw-r--r--   0 cadams     (501) staff       (20)     1258 2022-02-02 23:58:20.000000 django-haystack-3.2.dev0/test_haystack/whoosh_tests/testcases.py
--rw-r--r--   0 cadams     (501) staff       (20)      780 2022-03-17 23:44:59.000000 django-haystack-3.2.dev0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.332048 django_haystack-3.3b2/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-01 20:46:17.000000 django_haystack-3.3b2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-01 20:46:17.000000 django_haystack-3.3b2/.gitchangelog.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.292047 django_haystack-3.3b2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-01 20:46:17.000000 django_haystack-3.3b2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-01 20:46:17.000000 django_haystack-3.3b2/.github/issue_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-01 20:46:17.000000 django_haystack-3.3b2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.292047 django_haystack-3.3b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-01 20:46:17.000000 django_haystack-3.3b2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-01 20:46:17.000000 django_haystack-3.3b2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-01 20:46:17.000000 django_haystack-3.3b2/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-01 20:46:17.000000 django_haystack-3.3b2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-01 20:46:17.000000 django_haystack-3.3b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-01 20:46:17.000000 django_haystack-3.3b2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-01 20:46:17.000000 django_haystack-3.3b2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-01 20:46:17.000000 django_haystack-3.3b2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-01 20:46:17.000000 django_haystack-3.3b2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-01 20:46:17.000000 django_haystack-3.3b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-01 20:46:17.000000 django_haystack-3.3b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-01 20:46:23.332048 django_haystack-3.3b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-01 20:46:17.000000 django_haystack-3.3b2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.328047 django_haystack-3.3b2/django_haystack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-01 20:46:23.000000 django_haystack-3.3b2/django_haystack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-05-01 20:46:23.000000 django_haystack-3.3b2/django_haystack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:46:23.000000 django_haystack-3.3b2/django_haystack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:46:22.000000 django_haystack-3.3b2/django_haystack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-01 20:46:23.000000 django_haystack-3.3b2/django_haystack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 20:46:23.000000 django_haystack-3.3b2/django_haystack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.300047 django_haystack-3.3b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.300047 django_haystack-3.3b2/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/_build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.300047 django_haystack-3.3b2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.300047 django_haystack-3.3b2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/_templates/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/admin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/architecture_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/autocomplete.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/backend_support.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/best_practices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/boost.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   186660 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/creating_new_backends.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/debugging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/faceting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.300047 django_haystack-3.3b2/docs/haystack_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/haystack_theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.300047 django_haystack-3.3b2/docs/haystack_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/haystack_theme/static/documentation.css
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/haystack_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/highlighting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/inputtypes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/installing_search_engines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/management_commands.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/migration_from_1_to_2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/multiple_index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/other_apps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/python3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/rich_content_extraction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/running_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/searchbackend_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/searchfield_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22347 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/searchindex_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/searchquery_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    31840 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/searchqueryset_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/searchresult_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8374 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/signal_processors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/spatial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/templatetags.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/toc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15489 2024-05-01 20:46:17.000000 django_haystack-3.3b2/docs/views_and_forms.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.300047 django_haystack-3.3b2/example_project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/example_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.304047 django_haystack-3.3b2/example_project/bare_bones_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/example_project/bare_bones_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-01 20:46:17.000000 django_haystack-3.3b2/example_project/bare_bones_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 20:46:17.000000 django_haystack-3.3b2/example_project/bare_bones_app/search_indexes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.304047 django_haystack-3.3b2/example_project/regular_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/example_project/regular_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-01 20:46:17.000000 django_haystack-3.3b2/example_project/regular_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-01 20:46:17.000000 django_haystack-3.3b2/example_project/regular_app/search_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 20:46:17.000000 django_haystack-3.3b2/example_project/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.288047 django_haystack-3.3b2/example_project/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.288047 django_haystack-3.3b2/example_project/templates/search/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.288047 django_haystack-3.3b2/example_project/templates/search/indexes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.304047 django_haystack-3.3b2/example_project/templates/search/indexes/bare_bones_app/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 20:46:17.000000 django_haystack-3.3b2/example_project/templates/search/indexes/bare_bones_app/cat_text.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.304047 django_haystack-3.3b2/example_project/templates/search/indexes/regular_app/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-01 20:46:17.000000 django_haystack-3.3b2/example_project/templates/search/indexes/regular_app/dog_text.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.304047 django_haystack-3.3b2/haystack/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.308047 django_haystack-3.3b2/haystack/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)    36622 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/backends/elasticsearch2_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17283 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/backends/elasticsearch5_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20354 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/backends/elasticsearch7_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39281 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/backends/elasticsearch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/backends/simple_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35355 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/backends/solr_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38367 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/backends/whoosh_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15675 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/generic_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18702 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.308047 django_haystack-3.3b2/haystack/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.308047 django_haystack-3.3b2/haystack/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/management/commands/build_solr_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/management/commands/clear_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/management/commands/haystack_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/management/commands/rebuild_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16117 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/management/commands/update_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/panels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26089 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/routers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.288047 django_haystack-3.3b2/haystack/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.308047 django_haystack-3.3b2/haystack/templates/panels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/templates/panels/haystack.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.308047 django_haystack-3.3b2/haystack/templates/search_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)    58455 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/templates/search_configuration/schema.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    57423 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/templates/search_configuration/solrconfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.308047 django_haystack-3.3b2/haystack/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/templatetags/highlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/templatetags/more_like_this.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.312048 django_haystack-3.3b2/haystack/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/utils/app_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/utils/geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/utils/highlighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12817 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/utils/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-01 20:46:23.000000 django_haystack-3.3b2/haystack/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-01 20:46:17.000000 django_haystack-3.3b2/haystack/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-01 20:46:17.000000 django_haystack-3.3b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:46:23.332048 django_haystack-3.3b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.312048 django_haystack-3.3b2/test_haystack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.316048 django_haystack-3.3b2/test_haystack/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/custom_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.316048 django_haystack-3.3b2/test_haystack/core/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/fixtures/base_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15018 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/fixtures/bulk_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.316048 django_haystack-3.3b2/test_haystack/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.316048 django_haystack-3.3b2/test_haystack/core/templates/search/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.316048 django_haystack-3.3b2/test_haystack/core/templates/search/indexes/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/templates/search/indexes/bar.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.316048 django_haystack-3.3b2/test_haystack/core/templates/search/indexes/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/templates/search/indexes/core/mockmodel_content.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/templates/search/indexes/core/mockmodel_extra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/templates/search/indexes/core/mockmodel_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/templates/search/indexes/core/mockmodel_text.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/templates/search/indexes/foo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/templates/search/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/templates/test_suggestion.html
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/core/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.316048 django_haystack-3.3b2/test_haystack/discovery/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/discovery/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/discovery/search_indexes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.288047 django_haystack-3.3b2/test_haystack/discovery/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.288047 django_haystack-3.3b2/test_haystack/discovery/templates/search/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.316048 django_haystack-3.3b2/test_haystack/discovery/templates/search/indexes/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/discovery/templates/search/indexes/bar_text.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.316048 django_haystack-3.3b2/test_haystack/elasticsearch2_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch2_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65707 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch2_tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch2_tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch2_tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.320047 django_haystack-3.3b2/test_haystack/elasticsearch5_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch5_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65708 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch5_tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch5_tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch5_tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.320047 django_haystack-3.3b2/test_haystack/elasticsearch7_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch7_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67491 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch7_tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch7_tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch7_tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.320047 django_haystack-3.3b2/test_haystack/elasticsearch_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68912 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch_tests/test_elasticsearch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch_tests/test_elasticsearch_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/elasticsearch_tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.320047 django_haystack-3.3b2/test_haystack/multipleindex/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/multipleindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/multipleindex/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/multipleindex/routers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/multipleindex/search_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12773 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/multipleindex/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/results_per_page_urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      377 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.320047 django_haystack-3.3b2/test_haystack/simple_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/simple_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/simple_tests/search_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8669 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/simple_tests/test_simple_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/simple_tests/test_simple_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.324047 django_haystack-3.3b2/test_haystack/solr_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.324047 django_haystack-3.3b2/test_haystack/solr_tests/content_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)    48184 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/content_extraction/test.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.324047 django_haystack-3.3b2/test_haystack/solr_tests/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/server/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.324047 django_haystack-3.3b2/test_haystack/solr_tests/server/confdir/
+-rw-r--r--   0 runner    (1001) docker     (127)    60187 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/server/confdir/schema.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    57364 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/server/confdir/solrconfig.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1684 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/server/get-solr-download-url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/server/setup-solr-test-server-in-docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2125 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/server/start-solr-test-server.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/server/wait-for-solr
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61143 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/test_solr_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13058 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/test_solr_management_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/test_solr_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/solr_tests/test_templatetags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.324047 django_haystack-3.3b2/test_haystack/spatial/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/spatial/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.324047 django_haystack-3.3b2/test_haystack/spatial/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/spatial/fixtures/sample_spatial_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/spatial/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/spatial/search_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/spatial/test_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_altered_internal_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.324047 django_haystack-3.3b2/test_haystack/test_app_using_appconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_using_appconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_using_appconfig/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.328047 django_haystack-3.3b2/test_haystack/test_app_using_appconfig/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_using_appconfig/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_using_appconfig/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_using_appconfig/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_using_appconfig/search_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_using_appconfig/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.328047 django_haystack-3.3b2/test_haystack/test_app_with_hierarchy/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_with_hierarchy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.328047 django_haystack-3.3b2/test_haystack/test_app_with_hierarchy/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_with_hierarchy/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.328047 django_haystack-3.3b2/test_haystack/test_app_with_hierarchy/contrib/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_with_hierarchy/contrib/django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.328047 django_haystack-3.3b2/test_haystack/test_app_with_hierarchy/contrib/django/hierarchal_app_django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_with_hierarchy/contrib/django/hierarchal_app_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_with_hierarchy/contrib/django/hierarchal_app_django/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.328047 django_haystack-3.3b2/test_haystack/test_app_without_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_without_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_without_models/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_app_without_models/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_django_config_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23313 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_generic_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32458 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15245 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_management_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38021 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15305 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10887 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:46:23.328047 django_haystack-3.3b2/test_haystack/whoosh_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/whoosh_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/whoosh_tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/whoosh_tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55232 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/whoosh_tests/test_whoosh_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/whoosh_tests/test_whoosh_management_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/whoosh_tests/test_whoosh_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-01 20:46:17.000000 django_haystack-3.3b2/test_haystack/whoosh_tests/testcases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-01 20:46:17.000000 django_haystack-3.3b2/tox.ini
```

### Comparing `django-haystack-3.2.dev0/.gitchangelog.rc` & `django_haystack-3.3b2/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/.github/pull_request_template.md` & `django_haystack-3.3b2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/.pre-commit-config.yaml` & `django_haystack-3.3b2/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,54 @@
 exclude: ".*/vendor/.*"
 repos:
-    - repo: https://github.com/PyCQA/isort
-      rev: 5.10.1
-      hooks:
-          - id: isort
-    - repo: https://github.com/psf/black
-      rev: 22.1.0
-      hooks:
-          - id: black
-    - repo: https://github.com/pre-commit/pre-commit-hooks
-      rev: v4.1.0
-      hooks:
-          - id: check-added-large-files
-            args: ["--maxkb=128"]
-          - id: check-ast
-          - id: check-byte-order-marker
-          - id: check-case-conflict
-          - id: check-docstring-first
-          - id: check-executables-have-shebangs
-          - id: check-json
-          - id: check-merge-conflict
-          - id: check-symlinks
-          - id: check-xml
-          - id: check-yaml
-          - id: debug-statements
-          - id: detect-private-key
-          - id: end-of-file-fixer
-          - id: mixed-line-ending
-            args: ["--fix=lf"]
-          - id: pretty-format-json
-            args: ["--autofix", "--no-sort-keys", "--indent=4"]
-          - id: trailing-whitespace
+  - repo: https://github.com/adamchainz/django-upgrade
+    rev: 1.15.0
+    hooks:
+      - id: django-upgrade
+        args: [--target-version, "5.0"] # Replace with Django version
+
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.2
+    hooks:
+      - id: ruff
+        # args: [ --fix, --exit-non-zero-on-fix ]
+
+  - repo: https://github.com/PyCQA/isort
+    rev: 5.13.2
+    hooks:
+      - id: isort
+
+  - repo: https://github.com/psf/black
+    rev: 24.4.2
+    hooks:
+      - id: black
+
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.6.0
+    hooks:
+      - id: check-added-large-files
+        args: ["--maxkb=128"]
+      - id: check-ast
+      - id: check-byte-order-marker
+      - id: check-case-conflict
+      - id: check-docstring-first
+      - id: check-executables-have-shebangs
+      - id: check-json
+      - id: check-merge-conflict
+      - id: check-symlinks
+      - id: check-toml
+      - id: check-xml
+      - id: check-yaml
+      - id: debug-statements
+      - id: detect-private-key
+      - id: end-of-file-fixer
+      - id: mixed-line-ending
+        args: ["--fix=lf"]
+      - id: pretty-format-json
+        args: ["--autofix", "--no-sort-keys", "--indent=4"]
+      - id: trailing-whitespace
+
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: v4.0.0-alpha.8
+    hooks:
+      - id: prettier
+        types_or: [json, toml, xml, yaml]
```

### Comparing `django-haystack-3.2.dev0/AUTHORS` & `django_haystack-3.3b2/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/CONTRIBUTING.md` & `django_haystack-3.3b2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/LICENSE` & `django_haystack-3.3b2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/PKG-INFO` & `django_haystack-3.3b2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,117 @@
 Metadata-Version: 2.1
 Name: django-haystack
-Version: 3.2.dev0
+Version: 3.3b2
 Summary: Pluggable search for Django.
-Home-page: http://haystacksearch.org/
-Author: Daniel Lindsley
-Author-email: daniel@toastdriven.com
-License: UNKNOWN
+Author-email: Daniel Lindsley <daniel@toastdriven.com>
 Project-URL: Documentation, https://django-haystack.readthedocs.io
+Project-URL: Homepage, http://haystacksearch.org/
 Project-URL: Source, https://github.com/django-haystack/django-haystack
-Description: .. image:: https://github.com/django-haystack/django-haystack/actions/workflows/test.yml/badge.svg
-              :target: https://github.com/django-haystack/django-haystack/actions/workflows/test.yml
-        .. image:: https://img.shields.io/pypi/v/django-haystack.svg
-              :target: https://pypi.python.org/pypi/django-haystack/
-        .. image:: https://img.shields.io/pypi/pyversions/django-haystack.svg
-              :target: https://pypi.python.org/pypi/django-haystack/
-        .. image:: https://img.shields.io/pypi/dm/django-haystack.svg
-              :target: https://pypi.python.org/pypi/django-haystack/
-        .. image:: https://readthedocs.org/projects/django-haystack/badge/
-              :target: https://django-haystack.readthedocs.io/
-        .. image:: https://img.shields.io/badge/code%20style-black-000.svg
-              :target: https://github.com/psf/black
-        .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
-              :target: https://pycqa.github.io/isort/
-        
-        ========
-        Haystack
-        ========
-        
-        :author: Daniel Lindsley
-        :date: 2013/07/28
-        
-        Haystack provides modular search for Django. It features a unified, familiar
-        API that allows you to plug in different search backends (such as Solr_,
-        Elasticsearch_, Whoosh_, Xapian_, etc.) without having to modify your code.
-        
-        .. _Solr: http://lucene.apache.org/solr/
-        .. _Elasticsearch: https://www.elastic.co/products/elasticsearch
-        .. _Whoosh: https://github.com/mchaput/whoosh/
-        .. _Xapian: http://xapian.org/
-        
-        Haystack is BSD licensed, plays nicely with third-party app without needing to
-        modify the source and supports advanced features like faceting, More Like This,
-        highlighting, spatial search and spelling suggestions.
-        
-        You can find more information at http://haystacksearch.org/.
-        
-        
-        Getting Help
-        ============
-        
-        There is a mailing list (http://groups.google.com/group/django-haystack/)
-        available for general discussion and an IRC channel (#haystack on
-        irc.freenode.net).
-        
-        
-        Documentation
-        =============
-        
-        * Development version: http://docs.haystacksearch.org/
-        * v2.8.X: https://django-haystack.readthedocs.io/en/v2.8.1/
-        * v2.7.X: https://django-haystack.readthedocs.io/en/v2.7.0/
-        * v2.6.X: https://django-haystack.readthedocs.io/en/v2.6.0/
-        
-        See the `changelog <docs/changelog.rst>`_
-        
-        Requirements
-        ============
-        
-        Haystack has a relatively easily-met set of requirements.
-        
-        * Python 3.6+
-        * A supported version of Django: https://www.djangoproject.com/download/#supported-versions
-        
-        Additionally, each backend has its own requirements. You should refer to
-        https://django-haystack.readthedocs.io/en/latest/installing_search_engines.html for more
-        details.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
+Requires-Dist: Django>=3.2
+Requires-Dist: packaging
 Provides-Extra: elasticsearch
+Requires-Dist: elasticsearch<8,>=5; extra == "elasticsearch"
+Provides-Extra: testing
+Requires-Dist: coverage; extra == "testing"
+Requires-Dist: geopy==2; extra == "testing"
+Requires-Dist: pysolr>=3.7; extra == "testing"
+Requires-Dist: python-dateutil; extra == "testing"
+Requires-Dist: requests; extra == "testing"
+Requires-Dist: whoosh<3.0,>=2.5.4; extra == "testing"
+
+.. image:: https://github.com/django-haystack/django-haystack/actions/workflows/test.yml/badge.svg
+      :target: https://github.com/django-haystack/django-haystack/actions/workflows/test.yml
+.. image:: https://img.shields.io/pypi/v/django-haystack.svg
+      :target: https://pypi.python.org/pypi/django-haystack/
+.. image:: https://img.shields.io/pypi/pyversions/django-haystack.svg
+      :target: https://pypi.python.org/pypi/django-haystack/
+.. image:: https://img.shields.io/pypi/dm/django-haystack.svg
+      :target: https://pypi.python.org/pypi/django-haystack/
+.. image:: https://readthedocs.org/projects/django-haystack/badge/
+      :target: https://django-haystack.readthedocs.io/
+.. image:: https://img.shields.io/badge/code%20style-black-000.svg
+      :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+      :target: https://pycqa.github.io/isort/
+
+========
+Haystack
+========
+
+:author: Daniel Lindsley
+:date: 2013/07/28
+
+Haystack provides modular search for Django. It features a unified, familiar
+API that allows you to plug in different search backends (such as Solr_,
+Elasticsearch_, Whoosh_, Xapian_, etc.) without having to modify your code.
+
+.. _Solr: http://lucene.apache.org/solr/
+.. _Elasticsearch: https://www.elastic.co/products/elasticsearch
+.. _Whoosh: https://github.com/mchaput/whoosh/
+.. _Xapian: http://xapian.org/
+
+Haystack is BSD licensed, plays nicely with third-party app without needing to
+modify the source and supports advanced features like faceting, More Like This,
+highlighting, spatial search and spelling suggestions.
+
+You can find more information at http://haystacksearch.org/.
+
+
+Getting Help
+============
+
+There is a mailing list (http://groups.google.com/group/django-haystack/)
+available for general discussion and an IRC channel (#haystack on
+irc.freenode.net).
+
+
+Documentation
+=============
+
+* Development version: http://docs.haystacksearch.org/
+* v2.8.X: https://django-haystack.readthedocs.io/en/v2.8.1/
+* v2.7.X: https://django-haystack.readthedocs.io/en/v2.7.0/
+* v2.6.X: https://django-haystack.readthedocs.io/en/v2.6.0/
+
+See the `changelog <docs/changelog.rst>`_
+
+Requirements
+============
+
+Haystack has a relatively easily-met set of requirements.
+
+* A supported version of Python: https://devguide.python.org/versions/#supported-versions
+* A supported version of Django: https://www.djangoproject.com/download/#supported-versions
+
+Additionally, each backend has its own requirements. You should refer to
+https://django-haystack.readthedocs.io/en/latest/installing_search_engines.html for more
+details.
+
+Experimental support for Django v5.0
+====================================
+
+The current release on PyPI_ does not yet support Django v5.0.
+
+.. _PyPI: https://pypi.org/project/django-haystack/
+
+To run on Django v5.0, please install by using:
+``pip install git+https://github.com/django-haystack/django-haystack.git``
```

### Comparing `django-haystack-3.2.dev0/README.rst` & `django_haystack-3.3b2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -55,13 +55,23 @@
 See the `changelog <docs/changelog.rst>`_
 
 Requirements
 ============
 
 Haystack has a relatively easily-met set of requirements.
 
-* Python 3.6+
+* A supported version of Python: https://devguide.python.org/versions/#supported-versions
 * A supported version of Django: https://www.djangoproject.com/download/#supported-versions
 
 Additionally, each backend has its own requirements. You should refer to
 https://django-haystack.readthedocs.io/en/latest/installing_search_engines.html for more
 details.
+
+Experimental support for Django v5.0
+====================================
+
+The current release on PyPI_ does not yet support Django v5.0.
+
+.. _PyPI: https://pypi.org/project/django-haystack/
+
+To run on Django v5.0, please install by using:
+``pip install git+https://github.com/django-haystack/django-haystack.git``
```

### Comparing `django-haystack-3.2.dev0/django_haystack.egg-info/PKG-INFO` & `django_haystack-3.3b2/django_haystack.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,117 @@
 Metadata-Version: 2.1
 Name: django-haystack
-Version: 3.2.dev0
+Version: 3.3b2
 Summary: Pluggable search for Django.
-Home-page: http://haystacksearch.org/
-Author: Daniel Lindsley
-Author-email: daniel@toastdriven.com
-License: UNKNOWN
+Author-email: Daniel Lindsley <daniel@toastdriven.com>
 Project-URL: Documentation, https://django-haystack.readthedocs.io
+Project-URL: Homepage, http://haystacksearch.org/
 Project-URL: Source, https://github.com/django-haystack/django-haystack
-Description: .. image:: https://github.com/django-haystack/django-haystack/actions/workflows/test.yml/badge.svg
-              :target: https://github.com/django-haystack/django-haystack/actions/workflows/test.yml
-        .. image:: https://img.shields.io/pypi/v/django-haystack.svg
-              :target: https://pypi.python.org/pypi/django-haystack/
-        .. image:: https://img.shields.io/pypi/pyversions/django-haystack.svg
-              :target: https://pypi.python.org/pypi/django-haystack/
-        .. image:: https://img.shields.io/pypi/dm/django-haystack.svg
-              :target: https://pypi.python.org/pypi/django-haystack/
-        .. image:: https://readthedocs.org/projects/django-haystack/badge/
-              :target: https://django-haystack.readthedocs.io/
-        .. image:: https://img.shields.io/badge/code%20style-black-000.svg
-              :target: https://github.com/psf/black
-        .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
-              :target: https://pycqa.github.io/isort/
-        
-        ========
-        Haystack
-        ========
-        
-        :author: Daniel Lindsley
-        :date: 2013/07/28
-        
-        Haystack provides modular search for Django. It features a unified, familiar
-        API that allows you to plug in different search backends (such as Solr_,
-        Elasticsearch_, Whoosh_, Xapian_, etc.) without having to modify your code.
-        
-        .. _Solr: http://lucene.apache.org/solr/
-        .. _Elasticsearch: https://www.elastic.co/products/elasticsearch
-        .. _Whoosh: https://github.com/mchaput/whoosh/
-        .. _Xapian: http://xapian.org/
-        
-        Haystack is BSD licensed, plays nicely with third-party app without needing to
-        modify the source and supports advanced features like faceting, More Like This,
-        highlighting, spatial search and spelling suggestions.
-        
-        You can find more information at http://haystacksearch.org/.
-        
-        
-        Getting Help
-        ============
-        
-        There is a mailing list (http://groups.google.com/group/django-haystack/)
-        available for general discussion and an IRC channel (#haystack on
-        irc.freenode.net).
-        
-        
-        Documentation
-        =============
-        
-        * Development version: http://docs.haystacksearch.org/
-        * v2.8.X: https://django-haystack.readthedocs.io/en/v2.8.1/
-        * v2.7.X: https://django-haystack.readthedocs.io/en/v2.7.0/
-        * v2.6.X: https://django-haystack.readthedocs.io/en/v2.6.0/
-        
-        See the `changelog <docs/changelog.rst>`_
-        
-        Requirements
-        ============
-        
-        Haystack has a relatively easily-met set of requirements.
-        
-        * Python 3.6+
-        * A supported version of Django: https://www.djangoproject.com/download/#supported-versions
-        
-        Additionally, each backend has its own requirements. You should refer to
-        https://django-haystack.readthedocs.io/en/latest/installing_search_engines.html for more
-        details.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
+Requires-Dist: Django>=3.2
+Requires-Dist: packaging
 Provides-Extra: elasticsearch
+Requires-Dist: elasticsearch<8,>=5; extra == "elasticsearch"
+Provides-Extra: testing
+Requires-Dist: coverage; extra == "testing"
+Requires-Dist: geopy==2; extra == "testing"
+Requires-Dist: pysolr>=3.7; extra == "testing"
+Requires-Dist: python-dateutil; extra == "testing"
+Requires-Dist: requests; extra == "testing"
+Requires-Dist: whoosh<3.0,>=2.5.4; extra == "testing"
+
+.. image:: https://github.com/django-haystack/django-haystack/actions/workflows/test.yml/badge.svg
+      :target: https://github.com/django-haystack/django-haystack/actions/workflows/test.yml
+.. image:: https://img.shields.io/pypi/v/django-haystack.svg
+      :target: https://pypi.python.org/pypi/django-haystack/
+.. image:: https://img.shields.io/pypi/pyversions/django-haystack.svg
+      :target: https://pypi.python.org/pypi/django-haystack/
+.. image:: https://img.shields.io/pypi/dm/django-haystack.svg
+      :target: https://pypi.python.org/pypi/django-haystack/
+.. image:: https://readthedocs.org/projects/django-haystack/badge/
+      :target: https://django-haystack.readthedocs.io/
+.. image:: https://img.shields.io/badge/code%20style-black-000.svg
+      :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+      :target: https://pycqa.github.io/isort/
+
+========
+Haystack
+========
+
+:author: Daniel Lindsley
+:date: 2013/07/28
+
+Haystack provides modular search for Django. It features a unified, familiar
+API that allows you to plug in different search backends (such as Solr_,
+Elasticsearch_, Whoosh_, Xapian_, etc.) without having to modify your code.
+
+.. _Solr: http://lucene.apache.org/solr/
+.. _Elasticsearch: https://www.elastic.co/products/elasticsearch
+.. _Whoosh: https://github.com/mchaput/whoosh/
+.. _Xapian: http://xapian.org/
+
+Haystack is BSD licensed, plays nicely with third-party app without needing to
+modify the source and supports advanced features like faceting, More Like This,
+highlighting, spatial search and spelling suggestions.
+
+You can find more information at http://haystacksearch.org/.
+
+
+Getting Help
+============
+
+There is a mailing list (http://groups.google.com/group/django-haystack/)
+available for general discussion and an IRC channel (#haystack on
+irc.freenode.net).
+
+
+Documentation
+=============
+
+* Development version: http://docs.haystacksearch.org/
+* v2.8.X: https://django-haystack.readthedocs.io/en/v2.8.1/
+* v2.7.X: https://django-haystack.readthedocs.io/en/v2.7.0/
+* v2.6.X: https://django-haystack.readthedocs.io/en/v2.6.0/
+
+See the `changelog <docs/changelog.rst>`_
+
+Requirements
+============
+
+Haystack has a relatively easily-met set of requirements.
+
+* A supported version of Python: https://devguide.python.org/versions/#supported-versions
+* A supported version of Django: https://www.djangoproject.com/download/#supported-versions
+
+Additionally, each backend has its own requirements. You should refer to
+https://django-haystack.readthedocs.io/en/latest/installing_search_engines.html for more
+details.
+
+Experimental support for Django v5.0
+====================================
+
+The current release on PyPI_ does not yet support Django v5.0.
+
+.. _PyPI: https://pypi.org/project/django-haystack/
+
+To run on Django v5.0, please install by using:
+``pip install git+https://github.com/django-haystack/django-haystack.git``
```

### Comparing `django-haystack-3.2.dev0/django_haystack.egg-info/SOURCES.txt` & `django_haystack-3.3b2/django_haystack.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 .editorconfig
 .gitchangelog.rc
 .gitignore
 .pre-commit-config.yaml
+.readthedocs.yaml
 AUTHORS
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
-setup.py
 tox.ini
+.github/dependabot.yml
 .github/issue_template.md
 .github/pull_request_template.md
 .github/workflows/codeql-analysis.yml
 .github/workflows/docs.yml
-.github/workflows/flake8.yml
-.github/workflows/publish.yml
+.github/workflows/pypi-release.yml
 .github/workflows/test.yml
 django_haystack.egg-info/PKG-INFO
 django_haystack.egg-info/SOURCES.txt
 django_haystack.egg-info/dependency_links.txt
 django_haystack.egg-info/not-zip-safe
 django_haystack.egg-info/requires.txt
 django_haystack.egg-info/top_level.txt
@@ -131,14 +130,15 @@
 test_haystack/results_per_page_urls.py
 test_haystack/run_tests.py
 test_haystack/settings.py
 test_haystack/test_altered_internal_names.py
 test_haystack/test_app_loading.py
 test_haystack/test_backends.py
 test_haystack/test_discovery.py
+test_haystack/test_django_config_detection.py
 test_haystack/test_fields.py
 test_haystack/test_forms.py
 test_haystack/test_generic_views.py
 test_haystack/test_indexes.py
 test_haystack/test_inputs.py
 test_haystack/test_loading.py
 test_haystack/test_management_commands.py
@@ -201,14 +201,15 @@
 test_haystack/solr_tests/test_solr_backend.py
 test_haystack/solr_tests/test_solr_management_commands.py
 test_haystack/solr_tests/test_solr_query.py
 test_haystack/solr_tests/test_templatetags.py
 test_haystack/solr_tests/content_extraction/test.pdf
 test_haystack/solr_tests/server/.gitignore
 test_haystack/solr_tests/server/get-solr-download-url.py
+test_haystack/solr_tests/server/setup-solr-test-server-in-docker.sh
 test_haystack/solr_tests/server/start-solr-test-server.sh
 test_haystack/solr_tests/server/wait-for-solr
 test_haystack/solr_tests/server/confdir/schema.xml
 test_haystack/solr_tests/server/confdir/solrconfig.xml
 test_haystack/spatial/__init__.py
 test_haystack/spatial/models.py
 test_haystack/spatial/search_indexes.py
```

### Comparing `django-haystack-3.2.dev0/docs/Makefile` & `django_haystack-3.3b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/admin.rst` & `django_haystack-3.3b2/docs/admin.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/architecture_overview.rst` & `django_haystack-3.3b2/docs/architecture_overview.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/autocomplete.rst` & `django_haystack-3.3b2/docs/autocomplete.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/backend_support.rst` & `django_haystack-3.3b2/docs/backend_support.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/best_practices.rst` & `django_haystack-3.3b2/docs/best_practices.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/boost.rst` & `django_haystack-3.3b2/docs/boost.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/changelog.rst` & `django_haystack-3.3b2/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -896,15 +896,15 @@
   Thanks to Ana Carolina (@anacarolinats) and Steve Bussetti (@sbussetti)
   for the patch.
 - Merge pull request #1281 from itbabu/python35. [Justin Caratzas]
 
   Add python 3.5 to tests
 - Add python 3.5 to tests. [Marco Badan]
 
-  ref: https://docs.djangoproject.com/en/1.9/faq/install/#what-python-version-can-i-use-with-django
+  ref: https://docs.djangoproject.com/en/stable/faq/install/#what-python-version-can-i-use-with-django
 - SearchQuerySet: don’t trigger backend access in __repr__ [Chris Adams]
 
   This can lead to confusing errors or performance issues by
   triggering backend access at unexpected locations such as
   logging.
 
   Closes #1278
```

### Comparing `django-haystack-3.2.dev0/docs/conf.py` & `django_haystack-3.3b2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import os
-import sys
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 # sys.path.append(os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
```

### Comparing `django-haystack-3.2.dev0/docs/contributing.rst` & `django_haystack-3.3b2/docs/contributing.rst`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
   * This is done so as not to include extraneous commits, as some people submit
     pull reqs based on their git master that has other things applied to it.
 
 * A set of commits should be squashed down to a single commit.
 
   * ``git merge --squash`` is a good tool for performing this, as is
     ``git rebase -i HEAD~N``.
-  * This is done to prevent anyone using the git repo from accidently pulling
+  * This is done to prevent anyone using the git repo from accidentally pulling
     work-in-progress commits.
 
 * Commit messages should use past tense, describe what changed & thank anyone
   involved. Examples::
 
     """Added support for the latest version of Whoosh (v2.3.2)."""
     """Fixed a bug in ``solr_backend.py``. Thanks to joeschmoe for the report!"""
```

### Comparing `django-haystack-3.2.dev0/docs/creating_new_backends.rst` & `django_haystack-3.3b2/docs/creating_new_backends.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/debugging.rst` & `django_haystack-3.3b2/docs/debugging.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/faceting.rst` & `django_haystack-3.3b2/docs/faceting.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/faq.rst` & `django_haystack-3.3b2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/glossary.rst` & `django_haystack-3.3b2/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/haystack_theme/layout.html` & `django_haystack-3.3b2/docs/haystack_theme/layout.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% extends "basic/layout.html" %}
 
 {%- block extrahead %}
-    <link rel="stylesheet" href="http://haystacksearch.org/css/front.css" media="screen">
+    <link rel="stylesheet" href="https://haystacksearch.org/css/front.css" media="screen">
     <link rel="stylesheet" href="_static/documentation.css" media="screen">
 {% endblock %}
 
 {%- block header %}
     <div id="header">
         <h1>Haystack</h1>
         <p>Modular search for Django</p>
```

### Comparing `django-haystack-3.2.dev0/docs/haystack_theme/static/documentation.css` & `django_haystack-3.3b2/docs/haystack_theme/static/documentation.css`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/highlighting.rst` & `django_haystack-3.3b2/docs/highlighting.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/index.rst` & `django_haystack-3.3b2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/inputtypes.rst` & `django_haystack-3.3b2/docs/inputtypes.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/installing_search_engines.rst` & `django_haystack-3.3b2/docs/installing_search_engines.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/management_commands.rst` & `django_haystack-3.3b2/docs/management_commands.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/migration_from_1_to_2.rst` & `django_haystack-3.3b2/docs/migration_from_1_to_2.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/multiple_index.rst` & `django_haystack-3.3b2/docs/multiple_index.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/other_apps.rst` & `django_haystack-3.3b2/docs/other_apps.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/python3.rst` & `django_haystack-3.3b2/docs/python3.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 installation. The API is completely backward-compatible, so you should be able
 to run your existing software without modification.
 
 Virtually all tests pass under both Python 2 & 3, with a small number of
 expected failures under Python (typically related to ordering, see below).
 
 .. _`six`: http://pythonhosted.org/six/
-.. _`Django`: https://docs.djangoproject.com/en/1.5/topics/python3/#str-and-unicode-methods
+.. _`Django`: https://docs.djangoproject.com/en/stable/topics/python3/#str-and-unicode-methods
 
 
 Supported Backends
 ==================
 
 The following backends are fully supported under Python 3. However, you may
 need to update these dependencies if you have a pre-existing setup.
```

### Comparing `django-haystack-3.2.dev0/docs/rich_content_extraction.rst` & `django_haystack-3.3b2/docs/rich_content_extraction.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/running_tests.rst` & `django_haystack-3.3b2/docs/running_tests.rst`

 * *Files 7% similar despite different names*

```diff
@@ -25,25 +25,21 @@
 ``Haystack`` is maintained with all tests passing at all times, so if you
 receive any errors during testing, please check your setup and file a report if
 the errors persist.
 
 To run just a portion of the tests you can use the script ``run_tests.py`` and
 just specify the files or directories you wish to run, for example::
 
-    cd test_haystack
-    ./run_tests.py whoosh_tests test_loading.py
+    python test_haystack/run_tests.py whoosh_tests test_loading.py
 
-The ``run_tests.py`` script is just a tiny wrapper around the nose_ library and
-any options you pass to it will be passed on; including ``--help`` to get a
-list of possible options::
+The ``run_tests.py`` script is just a tiny wrapper around the Django test
+command and any options you pass to it will be passed on; including ``--help``
+to get a list of possible options::
 
-    cd test_haystack
-    ./run_tests.py --help
-
-.. _nose: https://nose.readthedocs.io/en/latest/
+    python test_haystack/run_tests.py --help
 
 Configuring Solr
 ================
 
 Haystack assumes that you have a Solr server running on port ``9001`` which
 uses the schema and configuration provided in the
 ``test_haystack/solr_tests/server/`` directory. For convenience, a script is
@@ -63,8 +59,8 @@
 
 If you want to run the geo-django tests you may need to review the
 `GeoDjango GEOS and GDAL settings`_ before running these commands::
 
 	cd test_haystack
 	./run_tests.py elasticsearch_tests
 
-.. _GeoDjango GEOS and GDAL settings: https://docs.djangoproject.com/en/1.7/ref/contrib/gis/install/geolibs/#geos-library-path
+.. _GeoDjango GEOS and GDAL settings: https://docs.djangoproject.com/en/stable/ref/contrib/gis/install/geolibs/#geos-library-path
```

### Comparing `django-haystack-3.2.dev0/docs/searchbackend_api.rst` & `django_haystack-3.3b2/docs/searchbackend_api.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/searchfield_api.rst` & `django_haystack-3.3b2/docs/searchfield_api.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/searchindex_api.rst` & `django_haystack-3.3b2/docs/searchindex_api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
 
 Note that this is NOT a recommended approach to storing geographic data in a
 search engine (there is no formal suggestion on this as support is usually
 non-existent), merely an example of how to extend existing fields.
 
 .. note::
 
-   This method is analagous to Django's ``Field.clean`` methods.
+   This method is analogous to Django's ``Field.clean`` methods.
 
 
 Adding New Fields
 =================
 
 If you have an existing ``SearchIndex`` and you add a new field to it, Haystack
 will add this new data on any updates it sees after that point. However, this
```

### Comparing `django-haystack-3.2.dev0/docs/searchquery_api.rst` & `django_haystack-3.3b2/docs/searchquery_api.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/searchqueryset_api.rst` & `django_haystack-3.3b2/docs/searchqueryset_api.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/searchresult_api.rst` & `django_haystack-3.3b2/docs/searchresult_api.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/settings.rst` & `django_haystack-3.3b2/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/signal_processors.rst` & `django_haystack-3.3b2/docs/signal_processors.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/spatial.rst` & `django_haystack-3.3b2/docs/spatial.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 can provide this type of search.
 
 In addition, Haystack tries to implement these features in a way that is as
 close to GeoDjango_ as possible. There are some differences, which we'll
 highlight throughout this guide. Additionally, while the support isn't as
 comprehensive as PostGIS (for example), it is still quite useful.
 
-.. _GeoDjango: https://docs.djangoproject.com/en/1.11/ref/contrib/gis/
+.. _GeoDjango: https://docs.djangoproject.com/en/stable/ref/contrib/gis/
 
 
 Additional Requirements
 =======================
 
 The spatial functionality has only one non-included, non-available-in-Django
 dependency:
@@ -257,15 +257,16 @@
 kilometers, though Haystack will use the ``D`` object's conversion utilities to
 get it there). It is slower than``within`` but very exact & can involve fewer
 calculations on your part.
 
 Examples::
 
     from haystack.query import SearchQuerySet
-    from django.contrib.gis.geos import Point, D
+    from django.contrib.gis.geos import Point
+    from django.contrib.gis.measure import D
 
     ninth_and_mass = Point(-95.23592948913574, 38.96753407043678)
     # Within a two miles.
     max_dist = D(mi=2)
 
     # 'location' is the fieldname from our ``SearchIndex``...
 
@@ -300,15 +301,16 @@
 
 So like GeoDjango, Haystack exposes a method to signify that you want to
 include these calculated distances on results.
 
 Examples::
 
     from haystack.query import SearchQuerySet
-    from django.contrib.gis.geos import Point, D
+    from django.contrib.gis.geos import Point
+    from django.contrib.gis.measure import D
 
     ninth_and_mass = Point(-95.23592948913574, 38.96753407043678)
 
     # On a bounding box...
     downtown_bottom_left = Point(-95.23947, 38.9637903)
     downtown_top_right = Point(-95.23362278938293, 38.973081081164715)
 
@@ -318,15 +320,16 @@
     sqs = SearchQuerySet().dwithin('location', ninth_and_mass, D(mi=2)).distance('location', ninth_and_mass)
 
 You can even apply a different field, for instance if you calculate results of
 key, well-cached hotspots in town but want distances from the user's current
 position::
 
     from haystack.query import SearchQuerySet
-    from django.contrib.gis.geos import Point, D
+    from django.contrib.gis.geos import Point
+    from django.contrib.gis.measure import D
 
     ninth_and_mass = Point(-95.23592948913574, 38.96753407043678)
     user_loc = Point(-95.23455619812012, 38.97240128290697)
 
     sqs = SearchQuerySet().dwithin('location', ninth_and_mass, D(mi=2)).distance('location', user_loc)
 
 .. note::
@@ -359,15 +362,16 @@
 ``-distance`` **ONLY**, you'll get geographic ordering. Additionally, you must
 have a call to ``.distance()`` somewhere in the chain, otherwise there is no
 distance information on the results & nothing to sort by.
 
 Examples::
 
     from haystack.query import SearchQuerySet
-    from django.contrib.gis.geos import Point, D
+    from django.contrib.gis.geos import Point
+    from django.contrib.gis.measure import D
 
     ninth_and_mass = Point(-95.23592948913574, 38.96753407043678)
     downtown_bottom_left = Point(-95.23947, 38.9637903)
     downtown_top_right = Point(-95.23362278938293, 38.973081081164715)
 
     # Non-geo ordering.
     sqs = SearchQuerySet().within('location', downtown_bottom_left, downtown_top_right).order_by('title')
```

### Comparing `django-haystack-3.2.dev0/docs/templatetags.rst` & `django_haystack-3.3b2/docs/templatetags.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/toc.rst` & `django_haystack-3.3b2/docs/toc.rst`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/docs/tutorial.rst` & `django_haystack-3.3b2/docs/tutorial.rst`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     class Note(models.Model):
         user = models.ForeignKey(User)
         pub_date = models.DateTimeField()
         title = models.CharField(max_length=200)
         body = models.TextField()
 
-        def __unicode__(self):
+        def __str__(self):
             return self.title
 
 Finally, before starting with Haystack, you will want to choose a search
 backend to get started. There is a quick-start guide to
 :doc:`installing_search_engines`, though you may want to defer to each engine's
 official instructions.
```

### Comparing `django-haystack-3.2.dev0/docs/views_and_forms.rst` & `django_haystack-3.3b2/docs/views_and_forms.rst`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 .. note::
 
     As of version 2.4 the views in ``haystack.views.SearchView`` are deprecated in
     favor of the new generic views in ``haystack.generic_views.SearchView``
     which use the standard Django `class-based views`_ which are available in
     every version of Django which is supported by Haystack.
 
-.. _class-based views: https://docs.djangoproject.com/en/1.7/topics/class-based-views/
+.. _class-based views: https://docs.djangoproject.com/en/stable/topics/class-based-views/
 
 Haystack comes with some default, simple views & forms as well as some
 django-style views to help you get started and to cover the common cases.
 Included is a way to provide:
 
   * Basic, query-only search.
   * Search by models.
@@ -133,23 +133,23 @@
 .. note::
 
     As of version 2.4 the views in ``haystack.views.SearchView`` are deprecated in
     favor of the new generic views in ``haystack.generic_views.SearchView``
     which use the standard Django `class-based views`_ which are available in
     every version of Django which is supported by Haystack.
 
-.. _class-based views: https://docs.djangoproject.com/en/1.7/topics/class-based-views/
+.. _class-based views: https://docs.djangoproject.com/en/stable/topics/class-based-views/
 
 New Django Class Based Views
 ----------------------------
 
  .. versionadded:: 2.4.0
 
 The views in ``haystack.generic_views.SearchView`` inherit from Django’s standard
-`FormView <https://docs.djangoproject.com/en/1.7/ref/class-based-views/generic-editing/#formview>`_.
+`FormView <https://docs.djangoproject.com/en/stable/ref/class-based-views/generic-editing/#formview>`_.
 The example views can be customized like any other Django class-based view as
 demonstrated in this example which filters the search results in ``get_queryset``::
 
     # views.py
     from datetime import date
 
     from haystack.generic_views import SearchView
@@ -228,17 +228,17 @@
 | ``extra_context()``   | `get_context_data()`_                     |
 +-----------------------+-------------------------------------------+
 | ``create_response()`` | `dispatch()`_ or ``get()`` and ``post()`` |
 +-----------------------+-------------------------------------------+
 | ``get_query()``       | `get_queryset()`_                         |
 +-----------------------+-------------------------------------------+
 
-.. _get_context_data(): https://docs.djangoproject.com/en/1.7/ref/class-based-views/mixins-simple/#django.views.generic.base.ContextMixin.get_context_data
-.. _dispatch(): https://docs.djangoproject.com/en/1.7/ref/class-based-views/base/#django.views.generic.base.View.dispatch
-.. _get_queryset(): https://docs.djangoproject.com/en/1.7/ref/class-based-views/mixins-multiple-object/#django.views.generic.list.MultipleObjectMixin.get_queryset
+.. _get_context_data(): https://docs.djangoproject.com/en/stable/ref/class-based-views/mixins-simple/#django.views.generic.base.ContextMixin.get_context_data
+.. _dispatch(): https://docs.djangoproject.com/en/stable/ref/class-based-views/base/#django.views.generic.base.View.dispatch
+.. _get_queryset(): https://docs.djangoproject.com/en/stable/ref/class-based-views/mixins-multiple-object/#django.views.generic.list.MultipleObjectMixin.get_queryset
 
 
 Old-Style Views
 ---------------
 
  .. deprecated:: 2.4.0
```

### Comparing `django-haystack-3.2.dev0/example_project/regular_app/models.py` & `django_haystack-3.3b2/example_project/regular_app/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,12 +32,12 @@
         if self.owner_last_name:
             return "%s %s" % (self.name, self.owner_last_name)
 
         return self.name
 
 
 class Toy(models.Model):
-    dog = models.ForeignKey(Dog, related_name="toys")
+    dog = models.ForeignKey(Dog, on_delete=models.CASCADE, related_name="toys")
     name = models.CharField(max_length=60)
 
     def __str__(self):
         return "%s's %s" % (self.dog.name, self.name)
```

### Comparing `django-haystack-3.2.dev0/example_project/regular_app/search_indexes.py` & `django_haystack-3.3b2/example_project/regular_app/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/example_project/settings.py` & `django_haystack-3.3b2/example_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/__init__.py` & `django_haystack-3.3b2/haystack/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
+from importlib.metadata import PackageNotFoundError, version
+
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
-from pkg_resources import DistributionNotFound, get_distribution, parse_version
+from packaging.version import Version
 
 from haystack.constants import DEFAULT_ALIAS
 from haystack.utils import loading
 
 __author__ = "Daniel Lindsley"
 
 try:
-    pkg_distribution = get_distribution("django-haystack")
-    __version__ = pkg_distribution.version
-    version_info = pkg_distribution.parsed_version
-except DistributionNotFound:
+    __version__ = version("django-haystack")
+    version_info = Version(__version__)
+except PackageNotFoundError:
     __version__ = "0.0.dev0"
-    version_info = parse_version(__version__)
-
-default_app_config = "haystack.apps.HaystackConfig"
-
+    version_info = Version(__version__)
 
 # Help people clean up from 1.X.
 if hasattr(settings, "HAYSTACK_SITECONF"):
     raise ImproperlyConfigured(
         "The HAYSTACK_SITECONF setting is no longer used & can be removed."
     )
 if hasattr(settings, "HAYSTACK_SEARCH_ENGINE"):
```

### Comparing `django-haystack-3.2.dev0/haystack/admin.py` & `django_haystack-3.3b2/haystack/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django import VERSION as django_version
 from django.contrib.admin.options import ModelAdmin, csrf_protect_m
 from django.contrib.admin.views.main import SEARCH_VAR, ChangeList
 from django.core.exceptions import PermissionDenied
 from django.core.paginator import InvalidPage, Paginator
 from django.shortcuts import render
 from django.utils.encoding import force_str
 from django.utils.translation import ngettext
@@ -11,15 +12,18 @@
 from haystack.query import SearchQuerySet
 from haystack.utils import get_model_ct_tuple
 
 
 class SearchChangeList(ChangeList):
     def __init__(self, **kwargs):
         self.haystack_connection = kwargs.pop("haystack_connection", DEFAULT_ALIAS)
-        super().__init__(**kwargs)
+        super_kwargs = kwargs
+        if django_version[0] >= 4:
+            super_kwargs["search_help_text"] = "Search..."
+        super().__init__(**super_kwargs)
 
     def get_results(self, request):
         if SEARCH_VAR not in request.GET:
             return super().get_results(request)
 
         # Note that pagination is 0-based, not 1-based.
         sqs = (
```

### Comparing `django-haystack-3.2.dev0/haystack/apps.py` & `django_haystack-3.3b2/haystack/apps.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/backends/__init__.py` & `django_haystack-3.3b2/haystack/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/backends/elasticsearch2_backend.py` & `django_haystack-3.3b2/haystack/backends/elasticsearch2_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,29 +75,25 @@
                     self.conn,
                     actions=actions,
                     index=self.index_name,
                     **self._get_doc_type_option(),
                 )
                 self.conn.indices.refresh(index=self.index_name)
 
-        except elasticsearch.TransportError as e:
+        except elasticsearch.TransportError:
             if not self.silently_fail:
                 raise
 
             if models is not None:
-                self.log.error(
-                    "Failed to clear Elasticsearch index of models '%s': %s",
+                self.log.exception(
+                    "Failed to clear Elasticsearch index of models '%s'",
                     ",".join(models_to_delete),
-                    e,
-                    exc_info=True,
                 )
             else:
-                self.log.error(
-                    "Failed to clear Elasticsearch index: %s", e, exc_info=True
-                )
+                self.log.exception("Failed to clear Elasticsearch index")
 
     def build_search_kwargs(
         self,
         query_string,
         sort_by=None,
         start_offset=0,
         end_offset=None,
@@ -317,23 +313,21 @@
             raw_results = self.conn.search(
                 body=mlt_query,
                 index=self.index_name,
                 _source=True,
                 **self._get_doc_type_option(),
                 **params,
             )
-        except elasticsearch.TransportError as e:
+        except elasticsearch.TransportError:
             if not self.silently_fail:
                 raise
 
-            self.log.error(
-                "Failed to fetch More Like This from Elasticsearch for document '%s': %s",
+            self.log.exception(
+                "Failed to fetch More Like This from Elasticsearch for document '%s'",
                 doc_id,
-                e,
-                exc_info=True,
             )
             raw_results = {}
 
         return self._process_results(raw_results, result_class=result_class)
 
     def _process_results(
         self,
```

### Comparing `django-haystack-3.2.dev0/haystack/backends/elasticsearch5_backend.py` & `django_haystack-3.3b2/haystack/backends/elasticsearch5_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,29 +71,25 @@
                     self.conn,
                     actions=actions,
                     index=self.index_name,
                     **self._get_doc_type_option(),
                 )
                 self.conn.indices.refresh(index=self.index_name)
 
-        except elasticsearch.TransportError as e:
+        except elasticsearch.TransportError:
             if not self.silently_fail:
                 raise
 
             if models is not None:
-                self.log.error(
-                    "Failed to clear Elasticsearch index of models '%s': %s",
+                self.log.exception(
+                    "Failed to clear Elasticsearch index of models '%s'",
                     ",".join(models_to_delete),
-                    e,
-                    exc_info=True,
                 )
             else:
-                self.log.error(
-                    "Failed to clear Elasticsearch index: %s", e, exc_info=True
-                )
+                self.log.exception("Failed to clear Elasticsearch index")
 
     def build_search_kwargs(
         self,
         query_string,
         sort_by=None,
         start_offset=0,
         end_offset=None,
@@ -407,23 +403,21 @@
             raw_results = self.conn.search(
                 body=mlt_query,
                 index=self.index_name,
                 _source=True,
                 **self._get_doc_type_option(),
                 **params,
             )
-        except elasticsearch.TransportError as e:
+        except elasticsearch.TransportError:
             if not self.silently_fail:
                 raise
 
-            self.log.error(
-                "Failed to fetch More Like This from Elasticsearch for document '%s': %s",
+            self.log.exception(
+                "Failed to fetch More Like This from Elasticsearch for document '%s'",
                 doc_id,
-                e,
-                exc_info=True,
             )
             raw_results = {}
 
         return self._process_results(raw_results, result_class=result_class)
 
     def _process_results(
         self,
```

### Comparing `django-haystack-3.2.dev0/haystack/backends/elasticsearch7_backend.py` & `django_haystack-3.3b2/haystack/backends/elasticsearch7_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,29 +139,25 @@
                 bulk(
                     self.conn,
                     actions=actions,
                     index=self.index_name,
                 )
                 self.conn.indices.refresh(index=self.index_name)
 
-        except elasticsearch.TransportError as e:
+        except elasticsearch.TransportError:
             if not self.silently_fail:
                 raise
 
             if models is not None:
-                self.log.error(
-                    "Failed to clear Elasticsearch index of models '%s': %s",
+                self.log.exception(
+                    "Failed to clear Elasticsearch index of models '%s'",
                     ",".join(models_to_delete),
-                    e,
-                    exc_info=True,
                 )
             else:
-                self.log.error(
-                    "Failed to clear Elasticsearch index: %s", e, exc_info=True
-                )
+                self.log.exception("Failed to clear Elasticsearch index")
 
     def build_search_kwargs(
         self,
         query_string,
         sort_by=None,
         start_offset=0,
         end_offset=None,
@@ -475,23 +471,21 @@
                         }
                     }
                 }
 
             raw_results = self.conn.search(
                 body=mlt_query, index=self.index_name, _source=True, **params
             )
-        except elasticsearch.TransportError as e:
+        except elasticsearch.TransportError:
             if not self.silently_fail:
                 raise
 
-            self.log.error(
-                "Failed to fetch More Like This from Elasticsearch for document '%s': %s",
+            self.log.exception(
+                "Failed to fetch More Like This from Elasticsearch for document '%s'",
                 doc_id,
-                e,
-                exc_info=True,
             )
             raw_results = {}
 
         return self._process_results(raw_results, result_class=result_class)
 
     def _process_hits(self, raw_results):
         return raw_results.get("hits", {}).get("total", {}).get("value", 0)
```

### Comparing `django-haystack-3.2.dev0/haystack/backends/elasticsearch_backend.py` & `django_haystack-3.3b2/haystack/backends/elasticsearch_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,21 +195,19 @@
     def _prepare_object(self, index, obj):
         return index.full_prepare(obj)
 
     def update(self, index, iterable, commit=True):
         if not self.setup_complete:
             try:
                 self.setup()
-            except elasticsearch.TransportError as e:
+            except elasticsearch.TransportError:
                 if not self.silently_fail:
                     raise
 
-                self.log.error(
-                    "Failed to add documents to Elasticsearch: %s", e, exc_info=True
-                )
+                self.log.exception("Failed to add documents to Elasticsearch")
                 return
 
         prepped_docs = []
 
         for obj in iterable:
             try:
                 prepped_data = self._prepare_object(index, obj)
@@ -219,24 +217,23 @@
                 for key, value in prepped_data.items():
                     final_data[key] = self._from_python(value)
                 final_data["_id"] = final_data[ID]
 
                 prepped_docs.append(final_data)
             except SkipDocument:
                 self.log.debug("Indexing for object `%s` skipped", obj)
-            except elasticsearch.TransportError as e:
+            except elasticsearch.TransportError:
                 if not self.silently_fail:
                     raise
 
                 # We'll log the object identifier but won't include the actual object
                 # to avoid the possibility of that generating encoding errors while
                 # processing the log message:
-                self.log.error(
-                    "%s while preparing object for update" % e.__class__.__name__,
-                    exc_info=True,
+                self.log.exception(
+                    "Preparing object for update",
                     extra={"data": {"index": index, "object": get_identifier(obj)}},
                 )
 
         bulk(
             self.conn,
             prepped_docs,
             index=self.index_name,
@@ -248,45 +245,41 @@
 
     def remove(self, obj_or_string, commit=True):
         doc_id = get_identifier(obj_or_string)
 
         if not self.setup_complete:
             try:
                 self.setup()
-            except elasticsearch.TransportError as e:
+            except elasticsearch.TransportError:
                 if not self.silently_fail:
                     raise
 
-                self.log.error(
-                    "Failed to remove document '%s' from Elasticsearch: %s",
+                self.log.exception(
+                    "Failed to remove document '%s' from Elasticsearch",
                     doc_id,
-                    e,
-                    exc_info=True,
                 )
                 return
 
         try:
             self.conn.delete(
                 index=self.index_name,
                 id=doc_id,
                 ignore=404,
                 **self._get_doc_type_option(),
             )
 
             if commit:
                 self.conn.indices.refresh(index=self.index_name)
-        except elasticsearch.TransportError as e:
+        except elasticsearch.TransportError:
             if not self.silently_fail:
                 raise
 
-            self.log.error(
-                "Failed to remove document '%s' from Elasticsearch: %s",
+            self.log.exception(
+                "Failed to remove document '%s' from Elasticsearch",
                 doc_id,
-                e,
-                exc_info=True,
             )
 
     def clear(self, models=None, commit=True):
         # We actually don't want to do this here, as mappings could be
         # very different.
         # if not self.setup_complete:
         #     self.setup()
@@ -301,39 +294,35 @@
                 self.existing_mapping = {}
             else:
                 models_to_delete = []
 
                 for model in models:
                     models_to_delete.append("%s:%s" % (DJANGO_CT, get_model_ct(model)))
 
-                # Delete by query in Elasticsearch asssumes you're dealing with
+                # Delete by query in Elasticsearch assumes you're dealing with
                 # a ``query`` root object. :/
                 query = {
                     "query": {"query_string": {"query": " OR ".join(models_to_delete)}}
                 }
                 self.conn.delete_by_query(
                     index=self.index_name,
                     body=query,
                     **self._get_doc_type_option(),
                 )
-        except elasticsearch.TransportError as e:
+        except elasticsearch.TransportError:
             if not self.silently_fail:
                 raise
 
             if models is not None:
-                self.log.error(
-                    "Failed to clear Elasticsearch index of models '%s': %s",
+                self.log.exception(
+                    "Failed to clear Elasticsearch index of models '%s'",
                     ",".join(models_to_delete),
-                    e,
-                    exc_info=True,
                 )
             else:
-                self.log.error(
-                    "Failed to clear Elasticsearch index: %s", e, exc_info=True
-                )
+                self.log.exception("Failed to clear Elasticsearch index")
 
     def build_search_kwargs(
         self,
         query_string,
         sort_by=None,
         start_offset=0,
         end_offset=None,
@@ -584,23 +573,21 @@
         try:
             raw_results = self.conn.search(
                 body=search_kwargs,
                 index=self.index_name,
                 _source=True,
                 **self._get_doc_type_option(),
             )
-        except elasticsearch.TransportError as e:
+        except elasticsearch.TransportError:
             if not self.silently_fail:
                 raise
 
-            self.log.error(
-                "Failed to query Elasticsearch using '%s': %s",
+            self.log.exception(
+                "Failed to query Elasticsearch using '%s'",
                 query_string,
-                e,
-                exc_info=True,
             )
             raw_results = {}
 
         return self._process_results(
             raw_results,
             highlight=kwargs.get("highlight"),
             result_class=kwargs.get("result_class", SearchResult),
@@ -648,23 +635,21 @@
             raw_results = self.conn.mlt(
                 index=self.index_name,
                 id=doc_id,
                 mlt_fields=[field_name],
                 **self._get_doc_type_option(),
                 **params,
             )
-        except elasticsearch.TransportError as e:
+        except elasticsearch.TransportError:
             if not self.silently_fail:
                 raise
 
-            self.log.error(
-                "Failed to fetch More Like This from Elasticsearch for document '%s': %s",
+            self.log.exception(
+                "Failed to fetch More Like This from Elasticsearch for document '%s'",
                 doc_id,
-                e,
-                exc_info=True,
             )
             raw_results = {}
 
         return self._process_results(raw_results, result_class=result_class)
 
     def _process_hits(self, raw_results):
         return raw_results.get("hits", {}).get("total", 0)
@@ -688,17 +673,19 @@
             result_class = SearchResult
 
         if self.include_spelling and "suggest" in raw_results:
             raw_suggest = raw_results["suggest"].get("suggest")
             if raw_suggest:
                 spelling_suggestion = " ".join(
                     [
-                        word["text"]
-                        if len(word["options"]) == 0
-                        else word["options"][0]["text"]
+                        (
+                            word["text"]
+                            if len(word["options"]) == 0
+                            else word["options"][0]["text"]
+                        )
                         for word in raw_suggest
                     ]
                 )
 
         if "facets" in raw_results:
             facets = {"fields": {}, "dates": {}, "queries": {}}
 
@@ -967,15 +954,15 @@
                 "startswith",
                 "endswith",
                 "fuzzy",
             ]:
                 if value.input_type_name == "exact":
                     query_frag = prepared_value
                 else:
-                    # Iterate over terms & incorportate the converted form of each into the query.
+                    # Iterate over terms & incorporate the converted form of each into the query.
                     terms = []
 
                     if isinstance(prepared_value, str):
                         for possible_value in prepared_value.split(" "):
                             terms.append(
                                 filter_types[filter_type]
                                 % self.backend._from_python(possible_value)
```

### Comparing `django-haystack-3.2.dev0/haystack/backends/simple_backend.py` & `django_haystack-3.3b2/haystack/backends/simple_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A very basic, ORM-based backend for simple search during tests.
 """
+
 from functools import reduce
 from warnings import warn
 
 from django.db.models import Q
 
 from haystack import connections
 from haystack.backends import (
@@ -52,15 +53,15 @@
                     for term in query_string.split():
                         queries = []
 
                         for field in model._meta.fields:
                             if hasattr(field, "related"):
                                 continue
 
-                            if not field.get_internal_type() in (
+                            if field.get_internal_type() not in (
                                 "TextField",
                                 "CharField",
                                 "SlugField",
                             ):
                                 continue
 
                             queries.append(Q(**{"%s__icontains" % field.name: term}))
```

### Comparing `django-haystack-3.2.dev0/haystack/backends/solr_backend.py` & `django_haystack-3.3b2/haystack/backends/solr_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,44 +87,41 @@
             except UnicodeDecodeError:
                 if not self.silently_fail:
                     raise
 
                 # We'll log the object identifier but won't include the actual object
                 # to avoid the possibility of that generating encoding errors while
                 # processing the log message:
-                self.log.error(
+                self.log.exception(
                     "UnicodeDecodeError while preparing object for update",
-                    exc_info=True,
                     extra={"data": {"index": index, "object": get_identifier(obj)}},
                 )
 
         if len(docs) > 0:
             try:
                 self.conn.add(docs, commit=commit, boost=index.get_field_weights())
-            except (IOError, SolrError) as e:
+            except (IOError, SolrError):
                 if not self.silently_fail:
                     raise
 
-                self.log.error("Failed to add documents to Solr: %s", e, exc_info=True)
+                self.log.exception("Failed to add documents to Solr")
 
     def remove(self, obj_or_string, commit=True):
         solr_id = get_identifier(obj_or_string)
 
         try:
             kwargs = {"commit": commit, "id": solr_id}
             self.conn.delete(**kwargs)
-        except (IOError, SolrError) as e:
+        except (IOError, SolrError):
             if not self.silently_fail:
                 raise
 
-            self.log.error(
-                "Failed to remove document '%s' from Solr: %s",
+            self.log.exception(
+                "Failed to remove document '%s' from Solr",
                 solr_id,
-                e,
-                exc_info=True,
             )
 
     def clear(self, models=None, commit=True):
         if models is not None:
             assert isinstance(models, (list, tuple))
 
         try:
@@ -138,44 +135,40 @@
                     models_to_delete.append("%s:%s" % (DJANGO_CT, get_model_ct(model)))
 
                 self.conn.delete(q=" OR ".join(models_to_delete), commit=commit)
 
             if commit:
                 # Run an optimize post-clear. http://wiki.apache.org/solr/FAQ#head-9aafb5d8dff5308e8ea4fcf4b71f19f029c4bb99
                 self.conn.optimize()
-        except (IOError, SolrError) as e:
+        except (IOError, SolrError):
             if not self.silently_fail:
                 raise
 
             if models is not None:
-                self.log.error(
-                    "Failed to clear Solr index of models '%s': %s",
+                self.log.exception(
+                    "Failed to clear Solr index of models '%s'",
                     ",".join(models_to_delete),
-                    e,
-                    exc_info=True,
                 )
             else:
-                self.log.error("Failed to clear Solr index: %s", e, exc_info=True)
+                self.log.exception("Failed to clear Solr index")
 
     @log_query
     def search(self, query_string, **kwargs):
         if len(query_string) == 0:
             return {"results": [], "hits": 0}
 
         search_kwargs = self.build_search_kwargs(query_string, **kwargs)
 
         try:
             raw_results = self.conn.search(query_string, **search_kwargs)
-        except (IOError, SolrError) as e:
+        except (IOError, SolrError):
             if not self.silently_fail:
                 raise
 
-            self.log.error(
-                "Failed to query Solr using '%s': %s", query_string, e, exc_info=True
-            )
+            self.log.exception("Failed to query Solr using '%s'", query_string)
             raw_results = EmptyResults()
 
         return self._process_results(
             raw_results,
             highlight=kwargs.get("highlight"),
             result_class=kwargs.get("result_class", SearchResult),
             distance_point=kwargs.get("distance_point"),
@@ -200,15 +193,14 @@
         models=None,
         limit_to_registered_models=None,
         result_class=None,
         stats=None,
         collate=None,
         **extra_kwargs
     ):
-
         index = haystack.connections[self.connection_alias].get_unified_index()
 
         kwargs = {"fl": "* score", "df": index.document_field}
 
         if fields:
             if isinstance(fields, (list, set)):
                 fields = " ".join(fields)
@@ -271,41 +263,42 @@
 
         if facets is not None:
             kwargs["facet"] = "on"
             kwargs["facet.field"] = facets.keys()
 
             for facet_field, options in facets.items():
                 for key, value in options.items():
-                    kwargs[
-                        "f.%s.facet.%s" % (facet_field, key)
-                    ] = self.conn._from_python(value)
+                    kwargs["f.%s.facet.%s" % (facet_field, key)] = (
+                        self.conn._from_python(value)
+                    )
 
         if date_facets is not None:
             kwargs["facet"] = "on"
             kwargs["facet.%s" % self.date_facet_field] = date_facets.keys()
             kwargs["facet.%s.other" % self.date_facet_field] = "none"
 
             for key, value in date_facets.items():
-                kwargs[
-                    "f.%s.facet.%s.start" % (key, self.date_facet_field)
-                ] = self.conn._from_python(value.get("start_date"))
-                kwargs[
-                    "f.%s.facet.%s.end" % (key, self.date_facet_field)
-                ] = self.conn._from_python(value.get("end_date"))
+                kwargs["f.%s.facet.%s.start" % (key, self.date_facet_field)] = (
+                    self.conn._from_python(value.get("start_date"))
+                )
+                kwargs["f.%s.facet.%s.end" % (key, self.date_facet_field)] = (
+                    self.conn._from_python(value.get("end_date"))
+                )
                 gap_by_string = value.get("gap_by").upper()
                 gap_string = "%d%s" % (value.get("gap_amount"), gap_by_string)
 
                 if value.get("gap_amount") != 1:
                     gap_string += "S"
 
-                kwargs[
-                    "f.%s.facet.%s.gap" % (key, self.date_facet_field)
-                ] = "+%s/%s" % (
-                    gap_string,
-                    gap_by_string,
+                kwargs["f.%s.facet.%s.gap" % (key, self.date_facet_field)] = (
+                    "+%s/%s"
+                    % (
+                        gap_string,
+                        gap_by_string,
+                    )
                 )
 
         if query_facets is not None:
             kwargs["facet"] = "on"
             kwargs["facet.query"] = [
                 "%s:%s" % (field, value) for field, value in query_facets
             ]
@@ -446,23 +439,20 @@
         if narrow_queries:
             params["fq"] = list(narrow_queries)
 
         query = "%s:%s" % (ID, get_identifier(model_instance))
 
         try:
             raw_results = self.conn.more_like_this(query, field_name, **params)
-        except (IOError, SolrError) as e:
+        except (IOError, SolrError):
             if not self.silently_fail:
                 raise
 
-            self.log.error(
-                "Failed to fetch More Like This from Solr for document '%s': %s",
-                query,
-                e,
-                exc_info=True,
+            self.log.exception(
+                "Failed to fetch More Like This from Solr for document '%s'", query
             )
             raw_results = EmptyResults()
 
         return self._process_results(raw_results, result_class=result_class)
 
     def _process_results(
         self, raw_results, highlight=False, result_class=None, distance_point=None
@@ -510,19 +500,17 @@
                             facets[key][facet_field]["counts"][1::2],
                         )
                     )
 
         if self.include_spelling and hasattr(raw_results, "spellcheck"):
             try:
                 spelling_suggestions = self.extract_spelling_suggestions(raw_results)
-            except Exception as exc:
-                self.log.error(
+            except Exception:
+                self.log.exception(
                     "Error extracting spelling suggestions: %s",
-                    exc,
-                    exc_info=True,
                     extra={"data": {"spellcheck": raw_results.spellcheck}},
                 )
 
                 if not self.silently_fail:
                     raise
 
                 spelling_suggestions = None
@@ -743,19 +731,17 @@
                         Extracted full-text content, if applicable
             :metadata:
                         key:value pairs of text strings
         """
 
         try:
             return self.conn.extract(file_obj, **kwargs)
-        except Exception as e:
+        except Exception:
             self.log.warning(
-                "Unable to extract file contents: %s",
-                e,
-                exc_info=True,
+                "Unable to extract file contents",
                 extra={"data": {"file": file_obj}},
             )
             return None
 
 
 class SolrSearchQuery(BaseSearchQuery):
     def matching_all_fragment(self):
@@ -815,15 +801,15 @@
                 "startswith",
                 "endswith",
                 "fuzzy",
             ]:
                 if value.input_type_name == "exact":
                     query_frag = prepared_value
                 else:
-                    # Iterate over terms & incorportate the converted form of each into the query.
+                    # Iterate over terms & incorporate the converted form of each into the query.
                     terms = []
 
                     for possible_value in prepared_value.split(" "):
                         terms.append(
                             filter_types[filter_type]
                             % self.backend.conn._from_python(possible_value)
                         )
```

### Comparing `django-haystack-3.2.dev0/haystack/backends/whoosh_backend.py` & `django_haystack-3.3b2/haystack/backends/whoosh_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import os
 import re
 import shutil
 import threading
 import warnings
+from datetime import date, datetime
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
-from django.utils.datetime_safe import date, datetime
 from django.utils.encoding import force_str
 
 from haystack.backends import (
     BaseEngine,
     BaseSearchBackend,
     BaseSearchQuery,
     EmptyResults,
@@ -126,15 +126,21 @@
         """
         from haystack import connections
 
         new_index = False
 
         # Make sure the index is there.
         if self.use_file_storage and not os.path.exists(self.path):
-            os.makedirs(self.path)
+            try:
+                os.makedirs(self.path)
+            except Exception:
+                raise IOError(
+                    "The directory of your Whoosh index '%s' (cwd='%s') cannot be created for the current user/group."
+                    % (self.path, os.getcwd())
+                )
             new_index = True
 
         if self.use_file_storage and not os.access(self.path, os.W_OK):
             raise IOError(
                 "The path to your Whoosh index '%s' is not writable for the current user/group."
                 % self.path
             )
@@ -266,24 +272,23 @@
 
                 # Document boosts aren't supported in Whoosh 2.5.0+.
                 if "boost" in doc:
                     del doc["boost"]
 
                 try:
                     writer.update_document(**doc)
-                except Exception as e:
+                except Exception:
                     if not self.silently_fail:
                         raise
 
                     # We'll log the object identifier but won't include the actual object
                     # to avoid the possibility of that generating encoding errors while
                     # processing the log message:
-                    self.log.error(
-                        "%s while preparing object for update" % e.__class__.__name__,
-                        exc_info=True,
+                    self.log.exception(
+                        "Preparing object for update",
                         extra={"data": {"index": index, "object": get_identifier(obj)}},
                     )
 
         if len(iterable) > 0:
             # For now, commit no matter what, as we run into locking issues otherwise.
             writer.commit()
             if writer.ident is not None:
@@ -294,23 +299,21 @@
             self.setup()
 
         self.index = self.index.refresh()
         whoosh_id = get_identifier(obj_or_string)
 
         try:
             self.index.delete_by_query(q=self.parser.parse('%s:"%s"' % (ID, whoosh_id)))
-        except Exception as e:
+        except Exception:
             if not self.silently_fail:
                 raise
 
-            self.log.error(
-                "Failed to remove document '%s' from Whoosh: %s",
+            self.log.exception(
+                "Failed to remove document '%s' from Whoosh",
                 whoosh_id,
-                e,
-                exc_info=True,
             )
 
     def clear(self, models=None, commit=True):
         if not self.setup_complete:
             self.setup()
 
         self.index = self.index.refresh()
@@ -326,27 +329,25 @@
 
                 for model in models:
                     models_to_delete.append("%s:%s" % (DJANGO_CT, get_model_ct(model)))
 
                 self.index.delete_by_query(
                     q=self.parser.parse(" OR ".join(models_to_delete))
                 )
-        except Exception as e:
+        except Exception:
             if not self.silently_fail:
                 raise
 
             if models is not None:
-                self.log.error(
-                    "Failed to clear Whoosh index of models '%s': %s",
+                self.log.exception(
+                    "Failed to clear Whoosh index of models '%s'",
                     ",".join(models_to_delete),
-                    e,
-                    exc_info=True,
                 )
             else:
-                self.log.error("Failed to clear Whoosh index: %s", e, exc_info=True)
+                self.log.exception("Failed to clear Whoosh index")
 
     def delete_index(self):
         # Per the Whoosh mailing list, if wiping out everything from the index,
         # it's much more efficient to simply delete the index files.
         if self.use_file_storage and os.path.exists(self.path):
             shutil.rmtree(self.path)
         elif not self.use_file_storage:
@@ -925,16 +926,15 @@
         return value
 
 
 class WhooshSearchQuery(BaseSearchQuery):
     def _convert_datetime(self, date):
         if hasattr(date, "hour"):
             return force_str(date.strftime("%Y%m%d%H%M%S"))
-        else:
-            return force_str(date.strftime("%Y%m%d000000"))
+        return force_str(date.strftime("%Y%m%d000000"))
 
     def clean(self, query_fragment):
         """
         Provides a mechanism for sanitizing user input before presenting the
         value to the backend.
 
         Whoosh 1.X differs here in that you can no longer use a backslash
@@ -1015,15 +1015,15 @@
                 "startswith",
                 "endswith",
                 "fuzzy",
             ]:
                 if value.input_type_name == "exact":
                     query_frag = prepared_value
                 else:
-                    # Iterate over terms & incorportate the converted form of each into the query.
+                    # Iterate over terms & incorporate the converted form of each into the query.
                     terms = []
 
                     if isinstance(prepared_value, str):
                         possible_values = prepared_value.split(" ")
                     else:
                         if is_datetime is True:
                             prepared_value = self._convert_datetime(prepared_value)
```

### Comparing `django-haystack-3.2.dev0/haystack/constants.py` & `django_haystack-3.3b2/haystack/constants.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/exceptions.py` & `django_haystack-3.3b2/haystack/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/fields.py` & `django_haystack-3.3b2/haystack/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import datetime
 import re
 from inspect import ismethod
 
 from django.template import loader
-from django.utils import datetime_safe
 
 from haystack.exceptions import SearchFieldError
 from haystack.utils import get_model_ct_tuple
 
 
 class NOT_PROVIDED:
     pass
@@ -391,15 +391,15 @@
             return None
 
         if isinstance(value, str):
             match = DATE_REGEX.search(value)
 
             if match:
                 data = match.groupdict()
-                return datetime_safe.date(
+                return datetime.date(
                     int(data["year"]), int(data["month"]), int(data["day"])
                 )
             else:
                 raise SearchFieldError(
                     "Date provided to '%s' field doesn't appear to be a valid date string: '%s'"
                     % (self.instance_name, value)
                 )
@@ -424,15 +424,15 @@
             return None
 
         if isinstance(value, str):
             match = DATETIME_REGEX.search(value)
 
             if match:
                 data = match.groupdict()
-                return datetime_safe.datetime(
+                return datetime.datetime(
                     int(data["year"]),
                     int(data["month"]),
                     int(data["day"]),
                     int(data["hour"]),
                     int(data["minute"]),
                     int(data["second"]),
                 )
```

### Comparing `django-haystack-3.2.dev0/haystack/forms.py` & `django_haystack-3.3b2/haystack/forms.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/generic_views.py` & `django_haystack-3.3b2/haystack/generic_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,17 @@
         return context
 
     def get_queryset(self):
         qs = super().get_queryset()
         for field in self.facet_fields:
             qs = qs.facet(field)
 
-        for field in self.date_facet_fields:
-            qs = qs.date_facet(**field)
+        if self.date_facet_fields:
+            for field in self.date_facet_fields:
+                qs = qs.date_facet(**field)
 
         return qs
 
 
 class SearchView(SearchMixin, FormView):
     """A view class for searching a Haystack managed search index"""
 
@@ -123,16 +124,15 @@
         Handles GET requests and instantiates a blank version of the form.
         """
         form_class = self.get_form_class()
         form = self.get_form(form_class)
 
         if form.is_valid():
             return self.form_valid(form)
-        else:
-            return self.form_invalid(form)
+        return self.form_invalid(form)
 
 
 class FacetedSearchView(FacetedSearchMixin, SearchView):
     """
     A view class for searching a Haystack managed search index with
     facets
     """
```

### Comparing `django-haystack-3.2.dev0/haystack/indexes.py` & `django_haystack-3.3b2/haystack/indexes.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/inputs.py` & `django_haystack-3.3b2/haystack/inputs.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/management/commands/build_solr_schema.py` & `django_haystack-3.3b2/haystack/management/commands/build_solr_schema.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/management/commands/clear_index.py` & `django_haystack-3.3b2/haystack/management/commands/clear_index.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/management/commands/haystack_info.py` & `django_haystack-3.3b2/haystack/management/commands/haystack_info.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/management/commands/rebuild_index.py` & `django_haystack-3.3b2/haystack/management/commands/rebuild_index.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/management/commands/update_index.py` & `django_haystack-3.3b2/haystack/management/commands/update_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,14 @@
     end,
     total,
     verbosity=1,
     commit=True,
     max_retries=DEFAULT_MAX_RETRIES,
     last_max_pk=None,
 ):
-
     # Get a clone of the QuerySet so that the cache doesn't bloat up
     # in memory. Useful when reindexing large amounts of data.
     # the query must be ordered by PK in order to get the max PK in each batch
     small_cache_qs = qs.all().order_by("pk")
 
     # If we got the max seen PK from last batch, use it to restrict the qs
     # to values above; this optimises the query for Postgres as not to
@@ -140,15 +139,15 @@
             }
 
             error_msg = "Failed indexing %(start)s - %(end)s (retry %(retries)s/%(max_retries)s): %(exc)s"
             if not is_parent_process:
                 error_msg += " (pid %(pid)s): %(exc)s"
 
             if retries >= max_retries:
-                LOG.error(error_msg, error_context, exc_info=True)
+                LOG.exception(error_msg, error_context)
                 raise
             elif verbosity >= 2:
                 LOG.warning(error_msg, error_context, exc_info=True)
 
             # If going to try again, sleep a bit before
             time.sleep(2**retries)
```

### Comparing `django-haystack-3.2.dev0/haystack/manager.py` & `django_haystack-3.3b2/haystack/manager.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/models.py` & `django_haystack-3.3b2/haystack/models.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/panels.py` & `django_haystack-3.3b2/haystack/panels.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/query.py` & `django_haystack-3.3b2/haystack/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,14 @@
             for model in models_pks:
                 loaded_objects[model] = self._load_model_objects(
                     model, models_pks[model]
                 )
 
         for result in results:
             if self._load_all:
-
                 model_objects = loaded_objects.get(result.model, {})
                 # Try to coerce a primary key object that matches the models pk
                 # We have to deal with semi-arbitrary keys being cast from strings (UUID, int, etc)
                 if model_objects:
                     result_klass = type(next(iter(model_objects)))
                     result.pk = result_klass(result.pk)
 
@@ -310,32 +309,30 @@
             except StopIteration:
                 # There's nothing left, even though the bound is higher.
                 pass
 
         # Cache should be full enough for our needs.
         if is_slice:
             return self._result_cache[start:bound]
-        else:
-            return self._result_cache[start]
+        return self._result_cache[start]
 
     # Methods that return a SearchQuerySet.
     def all(self):  # noqa A003
         """Returns all results for the query."""
         return self._clone()
 
     def none(self):
         """Returns an empty result list for the query."""
         return self._clone(klass=EmptySearchQuerySet)
 
     def filter(self, *args, **kwargs):  # noqa A003
         """Narrows the search based on certain attributes and the default operator."""
         if DEFAULT_OPERATOR == "OR":
             return self.filter_or(*args, **kwargs)
-        else:
-            return self.filter_and(*args, **kwargs)
+        return self.filter_and(*args, **kwargs)
 
     def exclude(self, *args, **kwargs):
         """Narrows the search by ensuring certain attributes are not included."""
         clone = self._clone()
         clone.query.add_filter(~SQ(*args, **kwargs))
         return clone
```

### Comparing `django-haystack-3.2.dev0/haystack/signals.py` & `django_haystack-3.3b2/haystack/signals.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/templates/panels/haystack.html` & `django_haystack-3.3b2/haystack/templates/panels/haystack.html`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/templates/search_configuration/schema.xml` & `django_haystack-3.3b2/haystack/templates/search_configuration/schema.xml`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/templates/search_configuration/solrconfig.xml` & `django_haystack-3.3b2/haystack/templates/search_configuration/solrconfig.xml`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/templatetags/highlight.py` & `django_haystack-3.3b2/haystack/templatetags/highlight.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/templatetags/more_like_this.py` & `django_haystack-3.3b2/haystack/templatetags/more_like_this.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,19 @@
 
             sqs = sqs.more_like_this(model_instance)
 
             if self.limit is not None:
                 sqs = sqs[: self.limit]
 
             context[self.varname] = sqs
-        except Exception as exc:
-            logging.warning(
-                "Unhandled exception rendering %r: %s", self, exc, exc_info=True
+        except Exception:
+            logging.exception(
+                "Unhandled exception rendering %r",
+                self,
+                level=logging.WARNING,
             )
 
         return ""
 
 
 @register.tag
 def more_like_this(parser, token):
@@ -69,15 +71,15 @@
         {% more_like_this entry as related_content limit 5  %}
 
         # Pull just the top 5 similar entries or comments.
         {% more_like_this entry as related_content for "blog.entry,comments.comment" limit 5  %}
     """
     bits = token.split_contents()
 
-    if not len(bits) in (4, 6, 8):
+    if len(bits) not in (4, 6, 8):
         raise template.TemplateSyntaxError(
             "'%s' tag requires either 3, 5 or 7 arguments." % bits[0]
         )
 
     model = bits[1]
 
     if bits[2] != "as":
```

### Comparing `django-haystack-3.2.dev0/haystack/utils/__init__.py` & `django_haystack-3.3b2/haystack/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import importlib
 import re
 
 from django.conf import settings
 
 from haystack.constants import DJANGO_CT, DJANGO_ID, ID
-from haystack.utils.highlighting import Highlighter  # noqa=F401
+from haystack.utils.highlighting import Highlighter  # noqa: F401
 
 IDENTIFIER_REGEX = re.compile(r"^[\w\d_]+\.[\w\d_]+\.[\w\d-]+$")
 
 
 def default_get_identifier(obj_or_string):
     """
     Get an unique identifier for the object or a string representing the
```

### Comparing `django-haystack-3.2.dev0/haystack/utils/app_loading.py` & `django_haystack-3.3b2/haystack/utils/app_loading.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/utils/geo.py` & `django_haystack-3.3b2/haystack/utils/geo.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/utils/highlighting.py` & `django_haystack-3.3b2/haystack/utils/highlighting.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/haystack/utils/loading.py` & `django_haystack-3.3b2/haystack/utils/loading.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,14 @@
     def get_index_fieldname(self, field):
         if not self._built:
             self.build()
 
         return self._fieldnames.get(field) or field
 
     def get_index(self, model_klass):
-
         indexes = self.get_indexes()
 
         if model_klass not in indexes:
             raise NotHandled("The model %s is not registered" % model_klass)
 
         return indexes[model_klass]
```

### Comparing `django-haystack-3.2.dev0/haystack/views.py` & `django_haystack-3.3b2/haystack/views.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/core/fixtures/base_data.json` & `django_haystack-3.3b2/test_haystack/core/fixtures/base_data.json`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/core/fixtures/bulk_data.json` & `django_haystack-3.3b2/test_haystack/core/fixtures/bulk_data.json`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/core/models.py` & `django_haystack-3.3b2/test_haystack/core/models.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/core/urls.py` & `django_haystack-3.3b2/test_haystack/core/urls.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch2_tests/__init__.py` & `django_haystack-3.3b2/test_haystack/elasticsearch2_tests/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
+import os
 import unittest
-import warnings
 
 from django.conf import settings
 
 from haystack.utils import log as logging
 
-warnings.simplefilter("ignore", Warning)
 
-
-def setup():
+def load_tests(loader, standard_tests, pattern):
     log = logging.getLogger("haystack")
     try:
         import elasticsearch
 
         if not ((2, 0, 0) <= elasticsearch.__version__ < (3, 0, 0)):
             raise ImportError
         from elasticsearch import Elasticsearch, exceptions
@@ -25,7 +23,13 @@
     url = settings.HAYSTACK_CONNECTIONS["elasticsearch"]["URL"]
     es = Elasticsearch(url)
     try:
         es.info()
     except exceptions.ConnectionError as e:
         log.error("elasticsearch not running on %r" % url, exc_info=True)
         raise unittest.SkipTest("elasticsearch not running on %r" % url, e)
+
+    package_tests = loader.discover(
+        start_dir=os.path.dirname(__file__), pattern=pattern
+    )
+    standard_tests.addTests(package_tests)
+    return standard_tests
```

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch2_tests/test_backend.py` & `django_haystack-3.3b2/test_haystack/elasticsearch2_tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch2_tests/test_inputs.py` & `django_haystack-3.3b2/test_haystack/elasticsearch2_tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch2_tests/test_query.py` & `django_haystack-3.3b2/test_haystack/elasticsearch2_tests/test_query.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch5_tests/__init__.py` & `django_haystack-3.3b2/test_haystack/elasticsearch7_tests/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+import os
 import unittest
-import warnings
 
 from django.conf import settings
 
 from haystack.utils import log as logging
 
-warnings.simplefilter("ignore", Warning)
 
-
-def setup():
+def load_tests(loader, standard_tests, pattern):
     log = logging.getLogger("haystack")
     try:
         import elasticsearch
 
-        if not ((5, 0, 0) <= elasticsearch.__version__ < (6, 0, 0)):
+        if not ((7, 0, 0) <= elasticsearch.__version__ < (8, 0, 0)):
             raise ImportError
         from elasticsearch import Elasticsearch, exceptions
     except ImportError:
         log.error(
-            "Skipping ElasticSearch 5 tests: 'elasticsearch>=5.0.0,<6.0.0' not installed."
+            "Skipping ElasticSearch 7 tests: 'elasticsearch>=7.0.0,<8.0.0' not installed."
         )
-        raise unittest.SkipTest("'elasticsearch>=5.0.0,<6.0.0' not installed.")
+        raise unittest.SkipTest("'elasticsearch>=7.0.0,<8.0.0' not installed.")
 
     url = settings.HAYSTACK_CONNECTIONS["elasticsearch"]["URL"]
     es = Elasticsearch(url)
     try:
         es.info()
     except exceptions.ConnectionError as e:
         log.error("elasticsearch not running on %r" % url, exc_info=True)
         raise unittest.SkipTest("elasticsearch not running on %r" % url, e)
+
+    package_tests = loader.discover(
+        start_dir=os.path.dirname(__file__), pattern=pattern
+    )
+    standard_tests.addTests(package_tests)
+    return standard_tests
```

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch5_tests/test_backend.py` & `django_haystack-3.3b2/test_haystack/elasticsearch5_tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch5_tests/test_inputs.py` & `django_haystack-3.3b2/test_haystack/elasticsearch5_tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch5_tests/test_query.py` & `django_haystack-3.3b2/test_haystack/elasticsearch5_tests/test_query.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch7_tests/__init__.py` & `django_haystack-3.3b2/test_haystack/elasticsearch5_tests/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+import os
 import unittest
-import warnings
 
 from django.conf import settings
 
 from haystack.utils import log as logging
 
-warnings.simplefilter("ignore", Warning)
 
-
-def setup():
+def load_tests(loader, standard_tests, pattern):
     log = logging.getLogger("haystack")
     try:
         import elasticsearch
 
-        if not ((7, 0, 0) <= elasticsearch.__version__ < (8, 0, 0)):
+        if not ((5, 0, 0) <= elasticsearch.__version__ < (6, 0, 0)):
             raise ImportError
         from elasticsearch import Elasticsearch, exceptions
     except ImportError:
         log.error(
-            "Skipping ElasticSearch 7 tests: 'elasticsearch>=7.0.0,<8.0.0' not installed."
+            "Skipping ElasticSearch 5 tests: 'elasticsearch>=5.0.0,<6.0.0' not installed."
         )
-        raise unittest.SkipTest("'elasticsearch>=7.0.0,<8.0.0' not installed.")
+        raise unittest.SkipTest("'elasticsearch>=5.0.0,<6.0.0' not installed.")
 
     url = settings.HAYSTACK_CONNECTIONS["elasticsearch"]["URL"]
     es = Elasticsearch(url)
     try:
         es.info()
     except exceptions.ConnectionError as e:
         log.error("elasticsearch not running on %r" % url, exc_info=True)
         raise unittest.SkipTest("elasticsearch not running on %r" % url, e)
+
+    package_tests = loader.discover(
+        start_dir=os.path.dirname(__file__), pattern=pattern
+    )
+    standard_tests.addTests(package_tests)
+    return standard_tests
```

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch7_tests/test_backend.py` & `django_haystack-3.3b2/test_haystack/elasticsearch7_tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch7_tests/test_inputs.py` & `django_haystack-3.3b2/test_haystack/elasticsearch7_tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch7_tests/test_query.py` & `django_haystack-3.3b2/test_haystack/elasticsearch7_tests/test_query.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch_tests/__init__.py` & `django_haystack-3.3b2/test_haystack/elasticsearch_tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,16 @@
+import os
 import unittest
-import warnings
 
 from django.conf import settings
 
 from haystack.utils import log as logging
 
-warnings.simplefilter("ignore", Warning)
 
-
-def setup():
+def load_tests(loader, standard_tests, pattern):
     log = logging.getLogger("haystack")
     try:
         import elasticsearch
 
         if not ((1, 0, 0) <= elasticsearch.__version__ < (2, 0, 0)):
             raise ImportError
         from elasticsearch import Elasticsearch, ElasticsearchException
@@ -32,7 +30,13 @@
             exc_info=True,
         )
         raise unittest.SkipTest(
             "elasticsearch not running on %r"
             % settings.HAYSTACK_CONNECTIONS["elasticsearch"]["URL"],
             e,
         )
+
+    package_tests = loader.discover(
+        start_dir=os.path.dirname(__file__), pattern=pattern
+    )
+    standard_tests.addTests(package_tests)
+    return standard_tests
```

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch_tests/test_elasticsearch_backend.py` & `django_haystack-3.3b2/test_haystack/elasticsearch_tests/test_elasticsearch_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,14 @@
             }
         )
 
         self.assertEqual(backend.conn.transport.max_retries, 42)
 
 
 class ElasticSearchMockUnifiedIndex(UnifiedIndex):
-
     spy_args = None
 
     def get_index(self, model_klass):
         if self.spy_args is not None:
             self.spy_args.setdefault("get_index", []).append(model_klass)
         return super().get_index(model_klass)
```

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch_tests/test_elasticsearch_query.py` & `django_haystack-3.3b2/test_haystack/elasticsearch_tests/test_elasticsearch_query.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/elasticsearch_tests/test_inputs.py` & `django_haystack-3.3b2/test_haystack/elasticsearch_tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/mocks.py` & `django_haystack-3.3b2/test_haystack/mocks.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/multipleindex/search_indexes.py` & `django_haystack-3.3b2/test_haystack/multipleindex/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/multipleindex/tests.py` & `django_haystack-3.3b2/test_haystack/multipleindex/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from django.apps import apps
 from django.db import models
 
-from haystack import connections
+from haystack import connection_router, connections
 from haystack.exceptions import NotHandled
 from haystack.query import SearchQuerySet
-from haystack.signals import BaseSignalProcessor
+from haystack.signals import BaseSignalProcessor, RealtimeSignalProcessor
 
 from ..whoosh_tests.testcases import WhooshTestCase
 from .models import Bar, Foo
 from .search_indexes import BarIndex, FooIndex
 
 
 class MultipleIndexTestCase(WhooshTestCase):
@@ -187,14 +188,30 @@
 
     def teardown(self):
         self.teardown_ran = True
         super().teardown()
 
 
 class SignalProcessorTestCase(WhooshTestCase):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+        config = apps.get_app_config("haystack")
+        cls._old_sp = config.signal_processor
+        config.signal_processor = RealtimeSignalProcessor(
+            connections, connection_router
+        )
+
+    @classmethod
+    def tearDown(cls):
+        config = apps.get_app_config("haystack")
+        config.signal_processor.teardown()
+        config.signal_processor = cls._old_sp
+        super().tearDown()
+
     def setUp(self):
         super().setUp()
 
         # Blatantly wrong data, just for assertion purposes.
         self.fake_connections = {}
         self.fake_router = []
```

### Comparing `django-haystack-3.2.dev0/test_haystack/settings.py` & `django_haystack-3.3b2/test_haystack/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 SECRET_KEY = "Please do not spew DeprecationWarnings"
 
 # Haystack settings for running tests.
 DATABASES = {
     "default": {"ENGINE": "django.db.backends.sqlite3", "NAME": "haystack_tests.db"}
 }
 
+# Use BigAutoField as the default auto field for all models
+DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
+
 INSTALLED_APPS = [
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "haystack",
@@ -30,14 +33,15 @@
 
 TEMPLATES = [
     {
         "BACKEND": "django.template.backends.django.DjangoTemplates",
         "APP_DIRS": True,
         "OPTIONS": {
             "context_processors": [
+                "django.template.context_processors.request",
                 "django.contrib.auth.context_processors.auth",
                 "django.contrib.messages.context_processors.messages",
             ]
         },
     }
 ]
```

### Comparing `django-haystack-3.2.dev0/test_haystack/simple_tests/search_indexes.py` & `django_haystack-3.3b2/test_haystack/simple_tests/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/simple_tests/test_simple_backend.py` & `django_haystack-3.3b2/test_haystack/simple_tests/test_simple_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,14 @@
         self.backend.update(self.index, self.sample_objs)
         self.assertEqual(self.backend.search("*")["hits"], 24)
 
         # Unsupported by 'simple'. Should see empty results.
         self.assertEqual(self.backend.more_like_this(self.sample_objs[0])["hits"], 0)
 
     def test_score_field_collision(self):
-
         index = connections["simple"].get_unified_index().get_index(ScoreMockModel)
         sample_objs = ScoreMockModel.objects.all()
 
         self.backend.update(index, self.sample_objs)
 
         # 42 is the in the match, which will be removed from the result
         self.assertEqual(self.backend.search("42")["results"][0].score, 0)
```

### Comparing `django-haystack-3.2.dev0/test_haystack/simple_tests/test_simple_query.py` & `django_haystack-3.3b2/test_haystack/simple_tests/test_simple_query.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/solr_tests/content_extraction/test.pdf` & `django_haystack-3.3b2/test_haystack/solr_tests/content_extraction/test.pdf`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/solr_tests/server/confdir/schema.xml` & `django_haystack-3.3b2/test_haystack/solr_tests/server/confdir/schema.xml`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/solr_tests/server/confdir/solrconfig.xml` & `django_haystack-3.3b2/test_haystack/solr_tests/server/confdir/solrconfig.xml`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/solr_tests/server/get-solr-download-url.py` & `django_haystack-3.3b2/test_haystack/solr_tests/server/get-solr-download-url.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/solr_tests/server/start-solr-test-server.sh` & `django_haystack-3.3b2/test_haystack/solr_tests/server/start-solr-test-server.sh`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/solr_tests/server/wait-for-solr` & `django_haystack-3.3b2/test_haystack/solr_tests/server/wait-for-solr`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/solr_tests/test_admin.py` & `django_haystack-3.3b2/test_haystack/solr_tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/solr_tests/test_inputs.py` & `django_haystack-3.3b2/test_haystack/solr_tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/solr_tests/test_solr_backend.py` & `django_haystack-3.3b2/test_haystack/solr_tests/test_solr_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from decimal import Decimal
 from unittest.mock import patch
 
 import pysolr
 from django.conf import settings
 from django.test import TestCase
 from django.test.utils import override_settings
-from pkg_resources import parse_version
+from packaging.version import Version
 
 from haystack import connections, indexes, reset_search_queries
 from haystack.exceptions import SkipDocument
 from haystack.inputs import AltParser, AutoQuery, Raw
 from haystack.models import SearchResult
 from haystack.query import SQ, RelatedSearchQuerySet, SearchQuerySet
 from haystack.utils.loading import UnifiedIndex
@@ -416,15 +416,15 @@
         self.assertEqual(
             [
                 result.highlighted["text"][0]
                 for result in self.sb.search("Index", highlight=highlight_dict)[
                     "results"
                 ]
             ],
-            ["<i>Indexed</i>!\n1", "<i>Indexed</i>!\n2", "<i>Indexed</i>!\n3"],
+            ["<i>Indexed</i>!\n1\n", "<i>Indexed</i>!\n2\n", "<i>Indexed</i>!\n3\n"],
         )
 
         # full-form highlighting options
         highlight_dict = {"hl.simple.pre": "<i>", "hl.simple.post": "</i>"}
         self.assertEqual(
             [
                 result.highlighted["text"][0]
@@ -1646,15 +1646,15 @@
                 "core.afourthmockmodel.2",
                 "core.afourthmockmodel.4",
             ],
         )
 
 
 @unittest.skipIf(
-    parse_version(pysolr.__version__) < parse_version("3.1.1"),
+    Version(pysolr.__version__) < Version("3.1.1"),
     "content extraction requires pysolr > 3.1.1",
 )
 class LiveSolrContentExtractionTestCase(TestCase):
     def setUp(self):
         super().setUp()
 
         self.sb = connections["solr"].get_backend()
```

### Comparing `django-haystack-3.2.dev0/test_haystack/solr_tests/test_solr_management_commands.py` & `django_haystack-3.3b2/test_haystack/solr_tests/test_solr_management_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import datetime
 import os
+import shutil
+import tempfile
 from io import StringIO
 from tempfile import mkdtemp
 from unittest.mock import patch
 
 import pysolr
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
@@ -198,32 +200,33 @@
         call_command("clear_index", interactive=False, verbosity=0)
         self.assertEqual(self.solr.search("*:*").hits, 0)
 
         call_command("update_index", verbosity=2, workers=2, batchsize=5, commit=False)
         self.assertEqual(self.solr.search("*:*").hits, 0)
 
     def test_build_schema_wrong_backend(self):
-
         settings.HAYSTACK_CONNECTIONS["whoosh"] = {
             "ENGINE": "haystack.backends.whoosh_backend.WhooshEngine",
             "PATH": mkdtemp(prefix="dummy-path-"),
         }
 
         connections["whoosh"]._index = self.ui
         self.assertRaises(
             ImproperlyConfigured, call_command, "build_solr_schema", using="whoosh"
         )
 
     def test_build_schema(self):
-
         # Stow.
         oldhdf = constants.DOCUMENT_FIELD
         oldui = connections["solr"].get_unified_index()
         oldurl = settings.HAYSTACK_CONNECTIONS["solr"]["URL"]
 
+        conf_dir = tempfile.mkdtemp()
+        with open(os.path.join(conf_dir, "managed-schema"), "w+") as fp:
+            pass
         try:
             needle = "Th3S3cr3tK3y"
             constants.DOCUMENT_FIELD = (
                 needle  # Force index to use new key for document_fields
             )
             settings.HAYSTACK_CONNECTIONS["solr"]["URL"] = (
                 settings.HAYSTACK_CONNECTIONS["solr"]["URL"].rsplit("/", 1)[0]
@@ -232,18 +235,14 @@
 
             ui = UnifiedIndex()
             ui.build(indexes=[SolrMockSecretKeySearchIndex()])
             connections["solr"]._index = ui
 
             rendered_file = StringIO()
 
-            script_dir = os.path.realpath(os.path.dirname(__file__))
-            conf_dir = os.path.join(
-                script_dir, "server", "solr", "server", "solr", "mgmnt", "conf"
-            )
             schema_file = os.path.join(conf_dir, "schema.xml")
             solrconfig_file = os.path.join(conf_dir, "solrconfig.xml")
 
             self.assertTrue(
                 os.path.isdir(conf_dir), msg="Expected %s to be a directory" % conf_dir
             )
 
@@ -259,33 +258,41 @@
             with open(solrconfig_file) as s:
                 self.assertGreater(s.read().find('name="df">%s' % needle), -1)
 
             self.assertTrue(
                 os.path.isfile(os.path.join(conf_dir, "managed-schema.old"))
             )
 
-            call_command("build_solr_schema", using="solr", reload_core=True)
-
-            os.rename(schema_file, "%s.bak" % schema_file)
-            self.assertRaises(
-                CommandError,
-                call_command,
-                "build_solr_schema",
-                using="solr",
-                reload_core=True,
-            )
+            with patch(
+                "haystack.management.commands.build_solr_schema.requests.get"
+            ) as mock_request:
+                call_command("build_solr_schema", using="solr", reload_core=True)
+
+            with patch(
+                "haystack.management.commands.build_solr_schema.requests.get"
+            ) as mock_request:
+                mock_request.return_value.ok = False
+
+                self.assertRaises(
+                    CommandError,
+                    call_command,
+                    "build_solr_schema",
+                    using="solr",
+                    reload_core=True,
+                )
 
             call_command("build_solr_schema", using="solr", filename=schema_file)
             with open(schema_file) as s:
                 self.assertGreater(s.read().find('name="%s' % needle), -1)
         finally:
             # reset
             constants.DOCUMENT_FIELD = oldhdf
             connections["solr"]._index = oldui
             settings.HAYSTACK_CONNECTIONS["solr"]["URL"] = oldurl
+            shutil.rmtree(conf_dir, ignore_errors=True)
 
 
 class AppModelManagementCommandTestCase(TestCase):
     fixtures = ["base_data", "bulk_data.json"]
 
     def setUp(self):
         super().setUp()
```

### Comparing `django-haystack-3.2.dev0/test_haystack/solr_tests/test_solr_query.py` & `django_haystack-3.3b2/test_haystack/solr_tests/test_solr_query.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/solr_tests/test_templatetags.py` & `django_haystack-3.3b2/test_haystack/solr_tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/spatial/fixtures/sample_spatial_data.json` & `django_haystack-3.3b2/test_haystack/spatial/fixtures/sample_spatial_data.json`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/spatial/models.py` & `django_haystack-3.3b2/test_haystack/spatial/models.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/spatial/search_indexes.py` & `django_haystack-3.3b2/test_haystack/spatial/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/spatial/test_spatial.py` & `django_haystack-3.3b2/test_haystack/spatial/test_spatial.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
     using = "solr"
 
     def setUp(self):
         from django.contrib.gis.geos import Point
 
         super().setUp()
         self.ui = connections[self.using].get_unified_index()
+        self.ui.reset()
         self.checkindex = self.ui.get_index(Checkin)
         self.checkindex.reindex(using=self.using)
         self.sqs = SearchQuerySet().using(self.using)
 
         self.downtown_pnt = Point(-95.23592948913574, 38.97127105172941)
         self.downtown_bottom_left = Point(-95.23947, 38.9637903)
         self.downtown_top_right = Point(-95.23362278938293, 38.973081081164715)
```

### Comparing `django-haystack-3.2.dev0/test_haystack/test_altered_internal_names.py` & `django_haystack-3.3b2/test_haystack/test_altered_internal_names.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/test_app_loading.py` & `django_haystack-3.3b2/test_haystack/test_app_loading.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/test_app_using_appconfig/migrations/0001_initial.py` & `django_haystack-3.3b2/test_haystack/test_app_using_appconfig/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="MicroBlogPost",
             fields=[
                 (
```

### Comparing `django-haystack-3.2.dev0/test_haystack/test_backends.py` & `django_haystack-3.3b2/test_haystack/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/test_discovery.py` & `django_haystack-3.3b2/test_haystack/test_discovery.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/test_fields.py` & `django_haystack-3.3b2/test_haystack/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/test_forms.py` & `django_haystack-3.3b2/test_haystack/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/test_generic_views.py` & `django_haystack-3.3b2/test_haystack/test_generic_views.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/test_indexes.py` & `django_haystack-3.3b2/test_haystack/test_indexes.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,16 +683,15 @@
     class Meta:
         model = MockModel
         fields = ["author", "foo"]
 
     def get_index_fieldname(self, f):
         if f.name == "author":
             return "author_bar"
-        else:
-            return f.name
+        return f.name
 
 
 class YetAnotherBasicModelSearchIndex(indexes.ModelSearchIndex, indexes.Indexable):
     text = indexes.CharField(document=True)
 
     class Meta:
         model = AThirdMockModel
```

### Comparing `django-haystack-3.2.dev0/test_haystack/test_inputs.py` & `django_haystack-3.3b2/test_haystack/test_inputs.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/test_loading.py` & `django_haystack-3.3b2/test_haystack/test_loading.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/test_management_commands.py` & `django_haystack-3.3b2/test_haystack/test_management_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,30 +73,30 @@
     @patch("haystack.management.commands.clear_index.Command.handle", return_value="")
     def test_rebuild_index(self, mock_handle_clear, mock_handle_update):
         call_command("rebuild_index", interactive=False)
 
         self.assertTrue(mock_handle_clear.called)
         self.assertTrue(mock_handle_update.called)
 
-    @patch("haystack.management.commands.update_index.Command.handle")
-    @patch("haystack.management.commands.clear_index.Command.handle")
+    @patch("haystack.management.commands.update_index.Command.handle", return_value="")
+    @patch("haystack.management.commands.clear_index.Command.handle", return_value="")
     def test_rebuild_index_nocommit(self, *mocks):
         call_command("rebuild_index", interactive=False, commit=False)
 
         for m in mocks:
             self.assertEqual(m.call_count, 1)
 
             args, kwargs = m.call_args
 
             self.assertIn("commit", kwargs)
             self.assertEqual(False, kwargs["commit"])
 
     @patch("haystack.management.commands.clear_index.Command.handle", return_value="")
     @patch("haystack.management.commands.update_index.Command.handle", return_value="")
-    def test_rebuild_index_nocommit(self, update_mock, clear_mock):
+    def test_rebuild_index_nocommit_two(self, update_mock, clear_mock):
         """
         Confirm that command-line option parsing produces the same results as using call_command() directly,
         mostly as a sanity check for the logic in rebuild_index which combines the option_lists for its
         component commands.
         """
         from haystack.management.commands.rebuild_index import Command
```

### Comparing `django-haystack-3.2.dev0/test_haystack/test_managers.py` & `django_haystack-3.3b2/test_haystack/test_managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,19 +238,19 @@
         # Test the case where spelling support is disabled.
         sqs = self.search_index.objects.filter(content="Indx")
         self.assertEqual(sqs.spelling_suggestion(), None)
         self.assertEqual(sqs.spelling_suggestion(preferred_query=None), None)
 
     def test_values(self):
         sqs = self.search_index.objects.auto_query("test").values("id")
-        self.assert_(isinstance(sqs, ValuesSearchQuerySet))
+        self.assertIsInstance(sqs, ValuesSearchQuerySet)
 
     def test_valueslist(self):
         sqs = self.search_index.objects.auto_query("test").values_list("id")
-        self.assert_(isinstance(sqs, ValuesListSearchQuerySet))
+        self.assertIsInstance(sqs, ValuesListSearchQuerySet)
 
 
 class CustomManagerTestCase(TestCase):
     fixtures = ["bulk_data.json"]
 
     def setUp(self):
         super().setUp()
```

### Comparing `django-haystack-3.2.dev0/test_haystack/test_models.py` & `django_haystack-3.3b2/test_haystack/test_models.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/test_query.py` & `django_haystack-3.3b2/test_haystack/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,20 @@
             "<SQ: AND ((foo__content=bar AND foo__content=bar) AND ((foo__content=bar OR foo__content=bar) OR NOT ((foo__content=bar AND NOT (foo__content=bar)))))>",
         )
 
 
 class BaseSearchQueryTestCase(TestCase):
     fixtures = ["base_data.json", "bulk_data.json"]
 
+    @classmethod
+    def setUpClass(cls):
+        for connection in connections.all():
+            connection.get_unified_index().reset()
+        super().setUpClass()
+
     def setUp(self):
         super().setUp()
         self.bsq = BaseSearchQuery()
 
     def test_get_count(self):
         self.bsq.add_filter(SQ(foo="bar"))
         self.assertRaises(NotImplementedError, self.bsq.get_count)
@@ -438,15 +444,15 @@
 
     def test_len(self):
         self.assertEqual(len(self.msqs), 23)
 
     def test_repr(self):
         reset_search_queries()
         self.assertEqual(len(connections["default"].queries), 0)
-        self.assertRegexpMatches(
+        self.assertRegex(
             repr(self.msqs),
             r"^<SearchQuerySet: query=<test_haystack.mocks.MockSearchQuery object"
             r" at 0x[0-9A-Fa-f]+>, using=None>$",
         )
 
     def test_iter(self):
         reset_search_queries()
@@ -963,42 +969,42 @@
             repr(sqs.query.query_filter.children[1]), repr(sqs2.query.query_filter)
         )
 
 
 class ValuesQuerySetTestCase(SearchQuerySetTestCase):
     def test_values_sqs(self):
         sqs = self.msqs.auto_query("test").values("id")
-        self.assert_(isinstance(sqs, ValuesSearchQuerySet))
+        self.assertIsInstance(sqs, ValuesSearchQuerySet)
 
         # We'll do a basic test to confirm that slicing works as expected:
-        self.assert_(isinstance(sqs[0], dict))
-        self.assert_(isinstance(sqs[0:5][0], dict))
+        self.assertIsInstance(sqs[0], dict)
+        self.assertIsInstance(sqs[0:5][0], dict)
 
     def test_valueslist_sqs(self):
         sqs = self.msqs.auto_query("test").values_list("id")
 
-        self.assert_(isinstance(sqs, ValuesListSearchQuerySet))
-        self.assert_(isinstance(sqs[0], (list, tuple)))
-        self.assert_(isinstance(sqs[0:1][0], (list, tuple)))
+        self.assertIsInstance(sqs, ValuesListSearchQuerySet)
+        self.assertIsInstance(sqs[0], (list, tuple))
+        self.assertIsInstance(sqs[0:1][0], (list, tuple))
 
         self.assertRaises(
             TypeError,
             self.msqs.auto_query("test").values_list,
             "id",
             "score",
             flat=True,
         )
 
         flat_sqs = self.msqs.auto_query("test").values_list("id", flat=True)
-        self.assert_(isinstance(sqs, ValuesListSearchQuerySet))
+        self.assertIsInstance(sqs, ValuesListSearchQuerySet)
 
         # Note that this will actually be None because a mocked sqs lacks
         # anything else:
-        self.assert_(flat_sqs[0] is None)
-        self.assert_(flat_sqs[0:1][0] is None)
+        self.assertIsNone(flat_sqs[0])
+        self.assertIsNone(flat_sqs[0:1][0])
 
 
 class EmptySearchQuerySetTestCase(TestCase):
     def setUp(self):
         super().setUp()
         self.esqs = EmptySearchQuerySet()
```

### Comparing `django-haystack-3.2.dev0/test_haystack/test_templatetags.py` & `django_haystack-3.3b2/test_haystack/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/test_utils.py` & `django_haystack-3.3b2/test_haystack/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/test_views.py` & `django_haystack-3.3b2/test_haystack/test_views.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/whoosh_tests/test_forms.py` & `django_haystack-3.3b2/test_haystack/whoosh_tests/test_forms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for Whoosh spelling suggestions"""
+
 from django.conf import settings
 from django.http import HttpRequest
 
 from haystack.forms import SearchForm
 from haystack.query import SearchQuerySet
 from haystack.views import SearchView
```

### Comparing `django-haystack-3.2.dev0/test_haystack/whoosh_tests/test_inputs.py` & `django_haystack-3.3b2/test_haystack/whoosh_tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/whoosh_tests/test_whoosh_backend.py` & `django_haystack-3.3b2/test_haystack/whoosh_tests/test_whoosh_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import unittest
-from datetime import timedelta
+from datetime import date, datetime, timedelta
 from decimal import Decimal
 
 from django.conf import settings
 from django.test import TestCase
 from django.test.utils import override_settings
-from django.utils.datetime_safe import date, datetime
 from whoosh.analysis import SpaceSeparatedTokenizer, SubstitutionFilter
 from whoosh.fields import BOOLEAN, DATETIME, KEYWORD, NUMERIC, TEXT
 from whoosh.qparser import QueryParser
 
 from haystack import connections, indexes, reset_search_queries
 from haystack.exceptions import SearchBackendError, SkipDocument
 from haystack.inputs import AutoQuery
@@ -111,14 +110,15 @@
     text_auto = indexes.EdgeNgramField(model_attr="foo")
     name_auto = indexes.EdgeNgramField(model_attr="author")
 
     def get_model(self):
         return MockModel
 
 
+@override_settings(USE_TZ=False)
 class WhooshSearchBackendTestCase(WhooshTestCase):
     fixtures = ["bulk_data.json"]
 
     def setUp(self):
         super().setUp()
 
         self.old_ui = connections["whoosh"].get_unified_index()
```

### Comparing `django-haystack-3.2.dev0/test_haystack/whoosh_tests/test_whoosh_management_commands.py` & `django_haystack-3.3b2/test_haystack/whoosh_tests/test_whoosh_management_commands.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/whoosh_tests/test_whoosh_query.py` & `django_haystack-3.3b2/test_haystack/whoosh_tests/test_whoosh_query.py`

 * *Files identical despite different names*

### Comparing `django-haystack-3.2.dev0/test_haystack/whoosh_tests/testcases.py` & `django_haystack-3.3b2/test_haystack/whoosh_tests/testcases.py`

 * *Files identical despite different names*

