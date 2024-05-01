# Comparing `tmp/magplan-3.2.0.tar.gz` & `tmp/magplan-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magplan-3.2.0.tar", max compression
+gzip compressed data, was "magplan-3.3.0.tar", max compression
```

## Comparing `magplan-3.2.0.tar` & `magplan-3.3.0.tar`

### file list

```diff
@@ -1,120 +1,123 @@
--rw-r--r--   0        0        0     6010 2023-12-13 19:44:22.000000 magplan-3.2.0/README.md
--rw-r--r--   0        0        0      807 2024-04-15 15:40:15.811782 magplan-3.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/__init__.py
--rw-r--r--   0        0        0     2211 2024-04-15 10:08:49.788255 magplan-3.2.0/src/magplan/admin.py
--rw-r--r--   0        0        0       86 2024-04-15 10:08:49.747321 magplan-3.2.0/src/magplan/apps.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/conf/__init__.py
--rw-r--r--   0        0        0     1720 2024-04-15 10:12:07.553740 magplan-3.2.0/src/magplan/conf/settings.py
--rw-r--r--   0        0        0      556 2024-04-15 10:08:49.770398 magplan-3.2.0/src/magplan/context_processors.py
--rw-r--r--   0        0        0     2908 2024-04-15 10:08:49.819748 magplan-3.2.0/src/magplan/dynamic_preferences_registry.py
--rw-r--r--   0        0        0  3415905 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/fixtures/db_test.json
--rw-r--r--   0        0        0    11011 2024-04-15 10:12:07.758358 magplan-3.2.0/src/magplan/forms.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/integrations/__init__.py
--rw-r--r--   0        0        0      732 2024-04-15 10:08:49.769775 magplan-3.2.0/src/magplan/integrations/images.py
--rw-r--r--   0        0        0     4936 2024-04-15 14:14:42.235067 magplan-3.2.0/src/magplan/integrations/posts.py
--rw-r--r--   0        0        0     1823 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39873 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2456 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40385 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/management/__init__.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/management/commands/__init__.py
--rw-r--r--   0        0        0      351 2024-04-15 10:08:49.771456 magplan-3.2.0/src/magplan/management/commands/render.py
--rw-r--r--   0        0        0      748 2024-04-15 10:12:07.526323 magplan-3.2.0/src/magplan/middleware.py
--rw-r--r--   0        0        0    17533 2024-04-15 10:12:07.987087 magplan-3.2.0/src/magplan/migrations/0001_initial.py
--rw-r--r--   0        0        0    10857 2024-04-15 10:12:07.853222 magplan-3.2.0/src/magplan/migrations/0002_auto_20201115_1140.py
--rw-r--r--   0        0        0      541 2024-04-15 10:08:49.809744 magplan-3.2.0/src/magplan/migrations/0003_auto_20201121_1750.py
--rw-r--r--   0        0        0      611 2024-04-15 10:08:49.820296 magplan-3.2.0/src/magplan/migrations/0004_post_features.py
--rw-r--r--   0        0        0     1424 2024-04-15 10:12:07.568938 magplan-3.2.0/src/magplan/migrations/0005_auto_20210213_1556.py
--rw-r--r--   0        0        0     1005 2024-04-15 10:12:07.568958 magplan-3.2.0/src/magplan/migrations/0006_auto_20210316_1840.py
--rw-r--r--   0        0        0      620 2024-04-15 10:12:07.553793 magplan-3.2.0/src/magplan/migrations/0007_auto_20210316_1900.py
--rw-r--r--   0        0        0     1652 2024-04-15 10:12:07.607046 magplan-3.2.0/src/magplan/migrations/0008_auto_20210318_0108.py
--rw-r--r--   0        0        0      610 2024-04-15 10:12:07.588161 magplan-3.2.0/src/magplan/migrations/0009_auto_20210523_1641.py
--rw-r--r--   0        0        0     2846 2024-04-15 10:12:07.654210 magplan-3.2.0/src/magplan/migrations/0010_auto_20210624_1041.py
--rw-r--r--   0        0        0     1274 2024-04-15 10:12:07.610111 magplan-3.2.0/src/magplan/migrations/0011_auto_20210624_1817.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/migrations/__init__.py
--rw-r--r--   0        0        0    28265 2024-04-15 15:22:19.092989 magplan-3.2.0/src/magplan/models.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/tasks/__init__.py
--rw-r--r--   0        0        0     3873 2024-04-15 10:12:07.677598 magplan-3.2.0/src/magplan/tasks/send_idea_comment_notification.py
--rw-r--r--   0        0        0      468 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/tasks/send_idea_notification.py
--rw-r--r--   0        0        0     4260 2024-04-15 10:12:07.684118 magplan-3.2.0/src/magplan/tasks/send_post_comment_notification.py
--rw-r--r--   0        0        0      543 2024-04-15 10:08:49.906811 magplan-3.2.0/src/magplan/tasks/upload_post_to_wp.py
--rw-r--r--   0        0        0     1790 2024-04-15 10:12:07.676796 magplan-3.2.0/src/magplan/tasks/utils.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/__init__.py
--rw-r--r--   0        0        0     1510 2024-04-15 10:12:07.706967 magplan-3.2.0/src/magplan/templates/_test_issues.py
--rw-r--r--   0        0        0      758 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/email/_vote_from_email.html
--rw-r--r--   0        0        0      416 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/email/assigned_to_you.html
--rw-r--r--   0        0        0      701 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/email/idea_approved.html
--rw-r--r--   0        0        0      634 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/email/new_comment.html
--rw-r--r--   0        0        0      370 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/email/new_idea.html
--rw-r--r--   0        0        0     8503 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/layout_plan.html
--rw-r--r--   0        0        0      893 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/articles/advert.html
--rw-r--r--   0        0        0      860 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/articles/archived.html
--rw-r--r--   0        0        0      855 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/articles/default.html
--rw-r--r--   0        0        0     3053 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/articles/index.html
--rw-r--r--   0        0        0      911 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/articles/whitelisted.html
--rw-r--r--   0        0        0     4121 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/authors/_form.html
--rw-r--r--   0        0        0      541 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/authors/edit.html
--rw-r--r--   0        0        0      869 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/authors/index.html
--rw-r--r--   0        0        0      480 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/authors/new.html
--rw-r--r--   0        0        0     1077 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/authors/show.html
--rw-r--r--   0        0        0      595 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/ideas/_approve_ideas.html
--rw-r--r--   0        0        0      786 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/ideas/_authors_list.html
--rw-r--r--   0        0        0     2332 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/ideas/_form_base.html
--rw-r--r--   0        0        0     1088 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/ideas/_vote.html
--rw-r--r--   0        0        0     1521 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/ideas/_voting_results.html
--rw-r--r--   0        0        0     3959 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/ideas/index.html
--rw-r--r--   0        0        0     3149 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/ideas/show.html
--rw-r--r--   0        0        0     4404 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/index/index.html
--rw-r--r--   0        0        0     1786 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/issues/_form.html
--rw-r--r--   0        0        0     1202 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/issues/index.html
--rw-r--r--   0        0        0      477 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/issues/new.html
--rw-r--r--   0        0        0      837 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/issues/show.html
--rw-r--r--   0        0        0      573 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/partials/_navbar.sites.html
--rw-r--r--   0        0        0     1395 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/partials/_navbar_header_links.html
--rw-r--r--   0        0        0     2797 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/partials/comments.html
--rw-r--r--   0        0        0     2252 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/partials/navbar.html
--rw-r--r--   0        0        0     3180 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/partials/posts_table.html
--rw-r--r--   0        0        0      956 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/posts/_admin_set_stage.html
--rw-r--r--   0        0        0     6970 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/posts/_attachments.html
--rw-r--r--   0        0        0      768 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/posts/_field_col.html
--rw-r--r--   0        0        0     3389 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/posts/_form_base.html
--rw-r--r--   0        0        0     3359 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/posts/_form_meta.html
--rw-r--r--   0        0        0      286 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/posts/_paywall_alert.html
--rw-r--r--   0        0        0     1063 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/posts/_progress.html
--rw-r--r--   0        0        0      882 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/posts/_schedule.html
--rw-r--r--   0        0        0     2437 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/posts/_stages.html
--rw-r--r--   0        0        0     8559 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/posts/edit.html
--rw-r--r--   0        0        0     9102 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/posts/show.html
--rw-r--r--   0        0        0      345 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/preferences/index.html
--rw-r--r--   0        0        0      804 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/sections/index.html
--rw-r--r--   0        0        0     1607 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templates/magplan/stages/index.html
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/templatetags/__init__.py
--rw-r--r--   0        0        0     6000 2024-04-15 10:08:50.138892 magplan-3.2.0/src/magplan/templatetags/filters.py
--rw-r--r--   0        0        0     2814 2024-04-15 10:12:07.760751 magplan-3.2.0/src/magplan/urls.py
--rw-r--r--   0        0        0     1248 2024-04-15 15:19:59.641866 magplan-3.2.0/src/magplan/utils.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/views/__init__.py
--rw-r--r--   0        0        0      898 2024-04-15 10:12:07.737198 magplan-3.2.0/src/magplan/views/api.py
--rw-r--r--   0        0        0     6435 2024-04-15 10:08:50.142325 magplan-3.2.0/src/magplan/views/articles.py
--rw-r--r--   0        0        0     3113 2024-04-15 10:12:07.834135 magplan-3.2.0/src/magplan/views/authors.py
--rw-r--r--   0        0        0     7975 2024-04-15 10:12:07.938557 magplan-3.2.0/src/magplan/views/ideas.py
--rw-r--r--   0        0        0     3321 2024-04-15 10:12:07.842747 magplan-3.2.0/src/magplan/views/index.py
--rw-r--r--   0        0        0     1894 2024-04-15 10:12:07.826409 magplan-3.2.0/src/magplan/views/issues.py
--rw-r--r--   0        0        0    16832 2024-04-15 10:12:08.117594 magplan-3.2.0/src/magplan/views/posts.py
--rw-r--r--   0        0        0     1134 2024-04-15 10:12:07.855150 magplan-3.2.0/src/magplan/views/preferences.py
--rw-r--r--   0        0        0      336 2024-04-15 10:08:50.139487 magplan-3.2.0/src/magplan/views/sections.py
--rw-r--r--   0        0        0      473 2024-04-15 10:08:50.139462 magplan-3.2.0/src/magplan/views/stages.py
--rw-r--r--   0        0        0      390 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/xmd/README.md
--rw-r--r--   0        0        0       27 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/xmd/__init__.py
--rw-r--r--   0        0        0     2909 2024-04-15 10:12:07.925445 magplan-3.2.0/src/magplan/xmd/lexers.py
--rw-r--r--   0        0        0      874 2024-04-15 10:08:50.159967 magplan-3.2.0/src/magplan/xmd/mappers.py
--rw-r--r--   0        0        0     1397 2024-04-15 10:08:50.169892 magplan-3.2.0/src/magplan/xmd/markdown.py
--rw-r--r--   0        0        0     2561 2024-04-15 10:12:07.910598 magplan-3.2.0/src/magplan/xmd/renderer.py
--rw-r--r--   0        0        0      313 2024-04-15 10:08:50.175035 magplan-3.2.0/src/magplan/xmd/templates.py
--rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/xmd/tests/__init__.py
--rw-r--r--   0        0        0       72 2023-12-15 21:31:27.000000 magplan-3.2.0/src/magplan/xmd/tests/conftest.py
--rw-r--r--   0        0        0     5167 2024-04-15 10:12:08.002177 magplan-3.2.0/src/magplan/xmd/tests/test_lexer.py
--rw-r--r--   0        0        0     1526 2024-04-15 10:12:07.944020 magplan-3.2.0/src/magplan/xmd/tests/test_renderer.py
--rw-r--r--   0        0        0     1296 2024-04-15 10:12:07.954891 magplan-3.2.0/src/magplan/xmd/tests/test_utils.py
--rw-r--r--   0        0        0      478 2024-04-15 10:08:50.208773 magplan-3.2.0/src/magplan/xmd/utils.py
--rw-r--r--   0        0        0      957 2024-04-15 10:08:50.224860 magplan-3.2.0/src/magplan/xmd/xmd.py
--rw-r--r--   0        0        0     7220 1970-01-01 00:00:00.000000 magplan-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6010 2023-12-13 19:44:22.000000 magplan-3.3.0/README.md
+-rw-r--r--   0        0        0      807 2024-05-01 06:20:25.333973 magplan-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-05-01 06:06:18.172458 magplan-3.3.0/src/magplan/__init__.py
+-rw-r--r--   0        0        0     2277 2024-05-01 06:14:12.298346 magplan-3.3.0/src/magplan/admin.py
+-rw-r--r--   0        0        0      401 2024-05-01 06:14:08.015571 magplan-3.3.0/src/magplan/apps.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/conf/__init__.py
+-rw-r--r--   0        0        0     1627 2024-05-01 06:17:13.407396 magplan-3.3.0/src/magplan/conf/settings.py
+-rw-r--r--   0        0        0      556 2024-04-15 10:08:49.770398 magplan-3.3.0/src/magplan/context_processors.py
+-rw-r--r--   0        0        0     2862 2024-05-01 06:14:08.095870 magplan-3.3.0/src/magplan/dynamic_preferences_registry.py
+-rw-r--r--   0        0        0  3415905 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/fixtures/db_test.json
+-rw-r--r--   0        0        0    10989 2024-05-01 06:14:08.419960 magplan-3.3.0/src/magplan/forms.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/integrations/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-15 10:08:49.769775 magplan-3.3.0/src/magplan/integrations/images.py
+-rw-r--r--   0        0        0     4936 2024-05-01 06:14:08.129489 magplan-3.3.0/src/magplan/integrations/posts.py
+-rw-r--r--   0        0        0     1823 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39873 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2456 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40385 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/management/commands/__init__.py
+-rw-r--r--   0        0        0      352 2024-05-01 06:06:17.521795 magplan-3.3.0/src/magplan/management/commands/render.py
+-rw-r--r--   0        0        0      748 2024-05-01 06:14:08.058580 magplan-3.3.0/src/magplan/middleware.py
+-rw-r--r--   0        0        0    17534 2024-05-01 06:14:08.624734 magplan-3.3.0/src/magplan/migrations/0001_initial.py
+-rw-r--r--   0        0        0    10857 2024-05-01 06:14:08.530027 magplan-3.3.0/src/magplan/migrations/0002_auto_20201115_1140.py
+-rw-r--r--   0        0        0      541 2024-04-15 10:08:49.809744 magplan-3.3.0/src/magplan/migrations/0003_auto_20201121_1750.py
+-rw-r--r--   0        0        0      611 2024-04-15 10:08:49.820296 magplan-3.3.0/src/magplan/migrations/0004_post_features.py
+-rw-r--r--   0        0        0     1424 2024-04-15 10:12:07.568938 magplan-3.3.0/src/magplan/migrations/0005_auto_20210213_1556.py
+-rw-r--r--   0        0        0     1005 2024-05-01 06:06:17.394818 magplan-3.3.0/src/magplan/migrations/0006_auto_20210316_1840.py
+-rw-r--r--   0        0        0      620 2024-05-01 06:06:17.361434 magplan-3.3.0/src/magplan/migrations/0007_auto_20210316_1900.py
+-rw-r--r--   0        0        0     1652 2024-05-01 06:06:17.358361 magplan-3.3.0/src/magplan/migrations/0008_auto_20210318_0108.py
+-rw-r--r--   0        0        0      610 2024-04-15 10:12:07.588161 magplan-3.3.0/src/magplan/migrations/0009_auto_20210523_1641.py
+-rw-r--r--   0        0        0     2847 2024-05-01 06:06:17.371144 magplan-3.3.0/src/magplan/migrations/0010_auto_20210624_1041.py
+-rw-r--r--   0        0        0     1274 2024-04-15 10:12:07.610111 magplan-3.3.0/src/magplan/migrations/0011_auto_20210624_1817.py
+-rw-r--r--   0        0        0      984 2024-05-01 06:06:18.388900 magplan-3.3.0/src/magplan/migrations/0012_alter_attachment_meta_alter_comment_meta_and_more.py
+-rw-r--r--   0        0        0     1818 2024-05-01 06:14:08.213881 magplan-3.3.0/src/magplan/migrations/0013_sitepreferencemodel.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/migrations/__init__.py
+-rw-r--r--   0        0        0    28566 2024-05-01 06:14:12.851359 magplan-3.3.0/src/magplan/models.py
+-rw-r--r--   0        0        0      200 2024-05-01 06:06:18.391401 magplan-3.3.0/src/magplan/registries.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/tasks/__init__.py
+-rw-r--r--   0        0        0     3873 2024-05-01 06:14:12.297514 magplan-3.3.0/src/magplan/tasks/send_idea_comment_notification.py
+-rw-r--r--   0        0        0      468 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/tasks/send_idea_notification.py
+-rw-r--r--   0        0        0     4260 2024-05-01 06:14:12.298004 magplan-3.3.0/src/magplan/tasks/send_post_comment_notification.py
+-rw-r--r--   0        0        0      542 2024-05-01 06:06:17.480250 magplan-3.3.0/src/magplan/tasks/upload_post_to_wp.py
+-rw-r--r--   0        0        0     1790 2024-05-01 06:14:08.227137 magplan-3.3.0/src/magplan/tasks/utils.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/__init__.py
+-rw-r--r--   0        0        0     1511 2024-05-01 06:14:12.276731 magplan-3.3.0/src/magplan/templates/_test_issues.py
+-rw-r--r--   0        0        0      758 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/email/_vote_from_email.html
+-rw-r--r--   0        0        0      416 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/email/assigned_to_you.html
+-rw-r--r--   0        0        0      701 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/email/idea_approved.html
+-rw-r--r--   0        0        0      634 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/email/new_comment.html
+-rw-r--r--   0        0        0      370 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/email/new_idea.html
+-rw-r--r--   0        0        0     8503 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/layout_plan.html
+-rw-r--r--   0        0        0      893 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/articles/advert.html
+-rw-r--r--   0        0        0      860 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/articles/archived.html
+-rw-r--r--   0        0        0      855 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/articles/default.html
+-rw-r--r--   0        0        0     3053 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/articles/index.html
+-rw-r--r--   0        0        0      911 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/articles/whitelisted.html
+-rw-r--r--   0        0        0     4121 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/authors/_form.html
+-rw-r--r--   0        0        0      541 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/authors/edit.html
+-rw-r--r--   0        0        0      869 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/authors/index.html
+-rw-r--r--   0        0        0      480 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/authors/new.html
+-rw-r--r--   0        0        0     1077 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/authors/show.html
+-rw-r--r--   0        0        0      595 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/ideas/_approve_ideas.html
+-rw-r--r--   0        0        0      786 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/ideas/_authors_list.html
+-rw-r--r--   0        0        0     2332 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/ideas/_form_base.html
+-rw-r--r--   0        0        0     1088 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/ideas/_vote.html
+-rw-r--r--   0        0        0     1521 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/ideas/_voting_results.html
+-rw-r--r--   0        0        0     3959 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/ideas/index.html
+-rw-r--r--   0        0        0     3149 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/ideas/show.html
+-rw-r--r--   0        0        0     4404 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/index/index.html
+-rw-r--r--   0        0        0     1786 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/issues/_form.html
+-rw-r--r--   0        0        0     1202 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/issues/index.html
+-rw-r--r--   0        0        0      477 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/issues/new.html
+-rw-r--r--   0        0        0      837 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/issues/show.html
+-rw-r--r--   0        0        0      573 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/partials/_navbar.sites.html
+-rw-r--r--   0        0        0     1395 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/partials/_navbar_header_links.html
+-rw-r--r--   0        0        0     2797 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/partials/comments.html
+-rw-r--r--   0        0        0     2252 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/partials/navbar.html
+-rw-r--r--   0        0        0     3180 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/partials/posts_table.html
+-rw-r--r--   0        0        0      956 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/posts/_admin_set_stage.html
+-rw-r--r--   0        0        0     6970 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/posts/_attachments.html
+-rw-r--r--   0        0        0      768 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/posts/_field_col.html
+-rw-r--r--   0        0        0     3389 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/posts/_form_base.html
+-rw-r--r--   0        0        0     3359 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/posts/_form_meta.html
+-rw-r--r--   0        0        0      286 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/posts/_paywall_alert.html
+-rw-r--r--   0        0        0     1063 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/posts/_progress.html
+-rw-r--r--   0        0        0      882 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/posts/_schedule.html
+-rw-r--r--   0        0        0     2437 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/posts/_stages.html
+-rw-r--r--   0        0        0     8559 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/posts/edit.html
+-rw-r--r--   0        0        0     9102 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/posts/show.html
+-rw-r--r--   0        0        0      345 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/preferences/index.html
+-rw-r--r--   0        0        0      804 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/sections/index.html
+-rw-r--r--   0        0        0     1607 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templates/magplan/stages/index.html
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/templatetags/__init__.py
+-rw-r--r--   0        0        0     6000 2024-05-01 06:06:17.346132 magplan-3.3.0/src/magplan/templatetags/filters.py
+-rw-r--r--   0        0        0     2814 2024-05-01 06:14:12.331038 magplan-3.3.0/src/magplan/urls.py
+-rw-r--r--   0        0        0     1248 2024-04-15 15:19:59.641866 magplan-3.3.0/src/magplan/utils.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/views/__init__.py
+-rw-r--r--   0        0        0      898 2024-04-15 10:12:07.737198 magplan-3.3.0/src/magplan/views/api.py
+-rw-r--r--   0        0        0     6435 2024-05-01 06:14:12.410162 magplan-3.3.0/src/magplan/views/articles.py
+-rw-r--r--   0        0        0     3041 2024-05-01 06:14:08.519369 magplan-3.3.0/src/magplan/views/authors.py
+-rw-r--r--   0        0        0     7950 2024-05-01 06:14:12.432610 magplan-3.3.0/src/magplan/views/ideas.py
+-rw-r--r--   0        0        0     3321 2024-05-01 06:14:08.537681 magplan-3.3.0/src/magplan/views/index.py
+-rw-r--r--   0        0        0     1859 2024-05-01 06:14:08.558308 magplan-3.3.0/src/magplan/views/issues.py
+-rw-r--r--   0        0        0    16990 2024-05-01 06:14:12.645881 magplan-3.3.0/src/magplan/views/posts.py
+-rw-r--r--   0        0        0     1134 2024-05-01 06:14:08.564285 magplan-3.3.0/src/magplan/views/preferences.py
+-rw-r--r--   0        0        0      337 2024-05-01 06:06:17.714358 magplan-3.3.0/src/magplan/views/sections.py
+-rw-r--r--   0        0        0      474 2024-05-01 06:06:17.782732 magplan-3.3.0/src/magplan/views/stages.py
+-rw-r--r--   0        0        0      390 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/xmd/README.md
+-rw-r--r--   0        0        0       27 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/xmd/__init__.py
+-rw-r--r--   0        0        0     2909 2024-05-01 06:14:08.651159 magplan-3.3.0/src/magplan/xmd/lexers.py
+-rw-r--r--   0        0        0      874 2024-04-15 10:08:50.159967 magplan-3.3.0/src/magplan/xmd/mappers.py
+-rw-r--r--   0        0        0     1397 2024-04-15 10:08:50.169892 magplan-3.3.0/src/magplan/xmd/markdown.py
+-rw-r--r--   0        0        0     2561 2024-05-01 06:14:08.666180 magplan-3.3.0/src/magplan/xmd/renderer.py
+-rw-r--r--   0        0        0      313 2024-04-15 10:08:50.175035 magplan-3.3.0/src/magplan/xmd/templates.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.3.0/src/magplan/xmd/tests/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-01 06:06:17.586779 magplan-3.3.0/src/magplan/xmd/tests/conftest.py
+-rw-r--r--   0        0        0     5168 2024-05-01 06:14:08.736635 magplan-3.3.0/src/magplan/xmd/tests/test_lexer.py
+-rw-r--r--   0        0        0     1526 2024-05-01 06:14:08.660016 magplan-3.3.0/src/magplan/xmd/tests/test_renderer.py
+-rw-r--r--   0        0        0     1274 2024-05-01 06:06:18.926242 magplan-3.3.0/src/magplan/xmd/tests/test_utils.py
+-rw-r--r--   0        0        0      478 2024-04-15 10:08:50.208773 magplan-3.3.0/src/magplan/xmd/utils.py
+-rw-r--r--   0        0        0      957 2024-04-15 10:08:50.224860 magplan-3.3.0/src/magplan/xmd/xmd.py
+-rw-r--r--   0        0        0     7220 1970-01-01 00:00:00.000000 magplan-3.3.0/PKG-INFO
```

### Comparing `magplan-3.2.0/README.md` & `magplan-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/pyproject.toml` & `magplan-3.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magplan"
-version = "3.2.0"
+version = "3.3.0"
 description = ""
 authors = ["Ilya Rusanen <ilya@rusanen.co.uk>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "^1.34.0"
```

### Comparing `magplan-3.2.0/src/magplan/admin.py` & `magplan-3.3.0/src/magplan/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Register your models here.
 from django.contrib import admin
 from django.contrib.auth.admin import UserAdmin as BaseUserAdmin
 from django_admin_listfilter_dropdown.filters import RelatedDropdownFilter
 
 from magplan.models import (
-    User,
-    Post,
+    Attachment,
     Comment,
+    Idea,
     Issue,
-    Stage,
     Magazine,
+    Post,
     Section,
-    Idea,
-    Attachment,
+    SitePreferenceModel,
+    Stage,
+    User,
 )
 
 
 class UserAdmin(BaseUserAdmin):
     ordering = ["profile__l_name"]
 
     list_display = [
@@ -97,7 +98,8 @@
 admin.site.register(Comment, CommentAdmin)
 admin.site.register(Issue)
 admin.site.register(Stage, StageAdmin)
 admin.site.register(Magazine)
 admin.site.register(Section, SectionAdmin)
 admin.site.register(Idea, IdeaAdmin)
 admin.site.register(Attachment, AttachmentAdmin)
+admin.site.register(SitePreferenceModel)
```

### Comparing `magplan-3.2.0/src/magplan/conf/settings.py` & `magplan-3.3.0/src/magplan/conf/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from django.conf import settings as django_settings
 
 SYSTEM_USER_ID = getattr(django_settings, "SYSTEM_USER_ID", "foo@bar.baz")
 PLAN_EMAIL_FROM = getattr(django_settings, "PLAN_EMAIL_FROM", "foo@bar.baz")
 EXTERNAL_PARSER_URL = getattr(django_settings, "EXTERNAL_PARSER_URL", None)
 EXTERNAL_PARSER_TOKEN = getattr(django_settings, "EXTERNAL_PARSER_TOKEN", None)
-PLAN_POSTS_INSTANCE_CHUNK = getattr(
-    django_settings, "PLAN_POSTS_INSTANCE_CHUNK", None
-)
+
 PLAN_EMAIL_SUBJECT_PREFIX = getattr(
     django_settings, "PLAN_EMAIL_SUBJECT_PREFIX", "[magplan]"
 )
 
 APP_HOST = getattr(django_settings, "APP_HOST", "magpplan.example.com")
 APP_URL = getattr(django_settings, "APP_URL", "https://magpplan.example.com")
 APP_ENV = getattr(django_settings, "APP_ENV", "PRODUCTION")
```

### Comparing `magplan-3.2.0/src/magplan/context_processors.py` & `magplan-3.3.0/src/magplan/context_processors.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/dynamic_preferences_registry.py` & `magplan-3.3.0/src/magplan/dynamic_preferences_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 from django import forms
-from django.contrib.sites.models import Site
 from dynamic_preferences.preferences import Section
-from dynamic_preferences.types import ChoicePreference
+from dynamic_preferences.types import ChoicePreference, StringPreference
 from dynamic_preferences.users.registries import user_preferences_registry
 
+from magplan.registries import site_preferences_registry
+
+general = Section("general")
 plan = Section("magplan")
 
 
+@site_preferences_registry.register
+class PrePostContentChunkTemplate(StringPreference):
+    section = general
+    name = "pre_post_content_chunk_template"
+    default = "Content links are places here"
+
+
 @user_preferences_registry.register
 class PlanUILanguage(ChoicePreference):
     name = "ui_language"
     section = plan
     choices = [("en", "English"), ("ru", "Русский")]
     default = "ru"
     widget = forms.Select(attrs={"class": "form-control"})
@@ -65,17 +74,7 @@
     choices = [
         ("yes", "Да"),
         ("no", "Нет"),
     ]
     default = "yes"
     widget = forms.Select(attrs={"class": "form-control"})
     verbose_name = "Присылать уведомелния о новых идеях?"
-
-
-@user_preferences_registry.register
-class PlanCurrentSite(ChoicePreference):
-    name = "current_site"
-    section = plan
-    choices = [(str(s.id), s.name) for s in Site.objects.all()]
-    default = "1"
-    widget = forms.Select(attrs={"class": "form-control"})
-    verbose_name = "Текущий сайт"
```

### Comparing `magplan-3.2.0/src/magplan/fixtures/db_test.json` & `magplan-3.3.0/src/magplan/fixtures/db_test.json`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/forms.py` & `magplan-3.3.0/src/magplan/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import namedtuple
 
 from django import forms
 from django.forms import ModelForm
 from django_ace import AceWidget
 
-from magplan.models import Idea, Post, Comment, Section, Issue, User, Profile
+from magplan.models import Comment, Idea, Issue, Post, Profile, Section, User
 
 SelectChoice = namedtuple("SelectChoice", ["slug", "title"])
 IDEA_AUTHOR_SELF_CHOICE = SelectChoice("SELF", "Напишу сам")
 
 
 class UserModelForm(ModelForm):
     class Meta:
@@ -376,17 +376,15 @@
         empty_label=None,
         widget=forms.Select(attrs={"class": "form-control", "rows": 5}),
     )
 
 
 class WhitelistedPostExtendedModelForm(PostDirectCreateModelForm):
     section = forms.ModelChoiceField(
-        queryset=Section.objects.filter(
-            is_archived=False, is_whitelisted=True
-        ),
+        queryset=Section.objects.filter(is_archived=False, is_whitelisted=True),
         label="Рубрика",
         empty_label=None,
         widget=forms.Select(attrs={"class": "form-control", "rows": 5}),
     )
 
 
 class AdPostExtendedModelForm(PostDirectCreateModelForm):
```

### Comparing `magplan-3.2.0/src/magplan/integrations/images.py` & `magplan-3.3.0/src/magplan/integrations/images.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/integrations/posts.py` & `magplan-3.3.0/src/magplan/integrations/posts.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/locale/en/LC_MESSAGES/django.mo` & `magplan-3.3.0/src/magplan/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/locale/en/LC_MESSAGES/django.po` & `magplan-3.3.0/src/magplan/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/locale/ru/LC_MESSAGES/django.mo` & `magplan-3.3.0/src/magplan/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/locale/ru/LC_MESSAGES/django.po` & `magplan-3.3.0/src/magplan/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/middleware.py` & `magplan-3.3.0/src/magplan/middleware.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/migrations/0001_initial.py` & `magplan-3.3.0/src/magplan/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.1.2 on 2020-11-15 11:40
 
 import datetime
+
 import django.contrib.postgres.fields.jsonb
-from django.db import migrations, models
 import django.utils.timezone
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = []
```

### Comparing `magplan-3.2.0/src/magplan/migrations/0002_auto_20201115_1140.py` & `magplan-3.3.0/src/magplan/migrations/0002_auto_20201115_1140.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Generated by Django 3.1.2 on 2020-11-15 11:40
 
 import django.contrib.auth.models
 import django.contrib.postgres.fields.jsonb
+import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
-import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
```

### Comparing `magplan-3.2.0/src/magplan/migrations/0003_auto_20201121_1750.py` & `magplan-3.3.0/src/magplan/migrations/0003_auto_20201121_1750.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/migrations/0004_post_features.py` & `magplan-3.3.0/src/magplan/migrations/0004_post_features.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/migrations/0005_auto_20210213_1556.py` & `magplan-3.3.0/src/magplan/migrations/0005_auto_20210213_1556.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/migrations/0006_auto_20210316_1840.py` & `magplan-3.3.0/src/magplan/migrations/0006_auto_20210316_1840.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by Django 3.1.6 on 2021-03-16 15:40
 
 import django.contrib.sites.managers
-from django.db import migrations, models
 import django.db.models.deletion
 import django.db.models.manager
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ("sites", "0002_alter_domain_unique"),
         ("magplan", "0005_auto_20210213_1556"),
```

### Comparing `magplan-3.2.0/src/magplan/migrations/0007_auto_20210316_1900.py` & `magplan-3.3.0/src/magplan/migrations/0007_auto_20210316_1900.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by Django 3.1.6 on 2021-03-16 16:00
 
 import django.contrib.sites.managers
-from django.db import migrations
 import django.db.models.manager
+from django.db import migrations
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ("magplan", "0006_auto_20210316_1840"),
     ]
```

### Comparing `magplan-3.2.0/src/magplan/migrations/0008_auto_20210318_0108.py` & `magplan-3.3.0/src/magplan/migrations/0008_auto_20210318_0108.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by Django 3.1.6 on 2021-03-17 22:08
 
 import django.contrib.sites.managers
-from django.db import migrations, models
 import django.db.models.deletion
 import django.db.models.manager
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ("sites", "0002_alter_domain_unique"),
         ("magplan", "0007_auto_20210316_1900"),
```

### Comparing `magplan-3.2.0/src/magplan/migrations/0009_auto_20210523_1641.py` & `magplan-3.3.0/src/magplan/migrations/0009_auto_20210523_1641.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/migrations/0010_auto_20210624_1041.py` & `magplan-3.3.0/src/magplan/migrations/0010_auto_20210624_1041.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.4 on 2021-06-24 07:41
 
 import django.contrib.sites.managers
-from django.db import migrations, models
 import django.db.models.deletion
 import django.db.models.manager
+from django.db import migrations, models
+
 import magplan.models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ("sites", "0002_alter_domain_unique"),
```

### Comparing `magplan-3.2.0/src/magplan/migrations/0011_auto_20210624_1817.py` & `magplan-3.3.0/src/magplan/migrations/0011_auto_20210624_1817.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/models.py` & `magplan-3.3.0/src/magplan/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 import mimetypes
 import os
 import typing as tp
 import urllib
 from typing import List
 
 import django
-from django.db.models import JSONField
 import html2text
 import requests
 from botocore.exceptions import ClientError
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.contenttypes.fields import (
-    GenericRelation,
     GenericForeignKey,
+    GenericRelation,
 )
 from django.contrib.contenttypes.models import ContentType
 from django.contrib.sites.managers import CurrentSiteManager
 from django.contrib.sites.models import Site
 from django.core.mail import EmailMultiAlternatives
 from django.db import models
-from django.db.models import Q, QuerySet
+from django.db.models import JSONField, Q, QuerySet
 from django.db.models.signals import post_save, pre_save
 from django.dispatch import receiver
 from django.template.loader import render_to_string
 from django.utils import timezone
+from dynamic_preferences.models import PerInstancePreferenceModel
 
 from magplan.conf import settings as config
 from magplan.integrations.images import S3Client
 from magplan.integrations.posts import replace_images_paths, update_ext_db_xmd
 from magplan.xmd import render_md
 from magplan.xmd.mappers import s3_public_mapper as s3_image_mapper
 
@@ -141,17 +141,15 @@
 
 class Profile(AbstractBase):
     is_public = models.BooleanField(null=False, blank=False, default=False)
     user = models.OneToOneField(
         User, on_delete=models.CASCADE, related_name="profile"
     )
     f_name = models.CharField("Имя", max_length=255, blank=True, null=True)
-    m_name = models.CharField(
-        "Отчество", max_length=255, blank=True, null=True
-    )
+    m_name = models.CharField("Отчество", max_length=255, blank=True, null=True)
     l_name = models.CharField("Фамилия", max_length=255, blank=True, null=True)
     n_name = models.CharField("Ник", max_length=255, blank=True, null=True)
     bio = models.TextField("Био", blank=True, null=True)
 
     # Global fields
     f_name_generic = models.CharField(
         "Имя латинницей", max_length=255, blank=True, null=True
@@ -188,17 +186,15 @@
     title = models.CharField(null=False, blank=False, max_length=255)
     description = models.TextField(null=True, blank=False)
     sort = models.SmallIntegerField(null=False, blank=False, default=0)
     color = models.CharField(
         null=False, blank=False, default="000000", max_length=6
     )
     is_archived = models.BooleanField(null=False, blank=False, default=False)
-    is_whitelisted = models.BooleanField(
-        null=False, blank=False, default=False
-    )
+    is_whitelisted = models.BooleanField(null=False, blank=False, default=False)
 
 
 class Magazine(AbstractBase):
     slug = models.SlugField(null=False, blank=False, max_length=255)
     title = models.CharField(null=False, blank=False, max_length=255)
     description = models.TextField(null=False, blank=True)
 
@@ -288,17 +284,15 @@
         max_length=255, null=True, blank=True, verbose_name="Новые автор"
     )
     authors = models.ManyToManyField(
         User, verbose_name="Авторы", related_name="authors", blank=True
     )
 
     def voted(self, user):
-        vote = next(
-            (v for v in self.votes.all() if v.user_id == user.id), None
-        )
+        vote = next((v for v in self.votes.all() if v.user_id == user.id), None)
 
         if vote:
             return True
         return False
 
     def _send_vote_notification(self, recipient: User) -> None:
         subject = f"Новая идея «{self.title}». Голосуйте!"
@@ -916,7 +910,19 @@
                 published_date: datetime.date = target_issue.published_at
                 published_datetime: datetime.datetime = (
                     datetime.datetime.combine(
                         published_date, datetime.datetime.min.time()
                     )
                 )
                 instance.published_at = published_datetime
+
+
+class SitePreferenceModel(PerInstancePreferenceModel):
+
+    instance = models.ForeignKey(
+        Site, on_delete=models.CASCADE, related_name="sites"
+    )
+
+    class Meta:
+        # Specifying the app_label here is mandatory for backward
+        # compatibility reasons, see #96
+        app_label = "magplan"
```

### Comparing `magplan-3.2.0/src/magplan/tasks/send_idea_comment_notification.py` & `magplan-3.3.0/src/magplan/tasks/send_idea_comment_notification.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from __future__ import absolute_import, unicode_literals
 
 import logging
 import os
 from typing import Set
 
 import html2text
-from magplan.conf import settings as config
+from celery import shared_task
 from django.contrib.contenttypes.models import ContentType
 from django.core.mail import EmailMultiAlternatives
 from django.template.loader import render_to_string
 
-from celery import shared_task
+from magplan.conf import settings as config
 from magplan.models import Comment, User
 from magplan.tasks.utils import (
     _can_recieve_notification,
     _get_whitelisted_recipients,
 )
 
 RECIEVE_NOTIFICATIONS_PERMISSION = "main.recieve_idea_email_updates"
```

### Comparing `magplan-3.2.0/src/magplan/tasks/send_post_comment_notification.py` & `magplan-3.3.0/src/magplan/tasks/send_post_comment_notification.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/tasks/upload_post_to_wp.py` & `magplan-3.3.0/src/magplan/tasks/upload_post_to_wp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Create your tasks here
 from __future__ import absolute_import, unicode_literals
 
 import logging
 
 from celery import shared_task
 
-from magplan.models import Post
 from magplan.integrations.posts import Lock
-
+from magplan.models import Post
 
 logger = logging.getLogger()
 
 
 @shared_task
 def upload_post_to_wp(post_id: int) -> None:
     logger.info("Starting task upload_post_to_wp...")
```

### Comparing `magplan-3.2.0/src/magplan/tasks/utils.py` & `magplan-3.3.0/src/magplan/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/_test_issues.py` & `magplan-3.3.0/src/magplan/templates/_test_issues.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from datetime import datetime
+
 from django.test import Client, TestCase
+from django.urls import reverse
+from main.models import Issue
 from plan.tests import (
-    _User,
-    _Sections,
-    _Section,
-    _Stages,
+    _Issue,
     _Post,
     _Postype,
-    _Issue,
+    _Section,
+    _Sections,
+    _Stages,
+    _User,
 )
-from django.urls import reverse
-from datetime import datetime
-from main.models import Issue
 
 
 class TestCreate(TestCase):
     @classmethod
     def setUpTestData(cls):
         cls.user = _User()
```

### Comparing `magplan-3.2.0/src/magplan/templates/email/_vote_from_email.html` & `magplan-3.3.0/src/magplan/templates/email/_vote_from_email.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/email/idea_approved.html` & `magplan-3.3.0/src/magplan/templates/email/idea_approved.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/email/new_comment.html` & `magplan-3.3.0/src/magplan/templates/email/new_comment.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/layout_plan.html` & `magplan-3.3.0/src/magplan/templates/layout_plan.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/articles/advert.html` & `magplan-3.3.0/src/magplan/templates/magplan/articles/advert.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/articles/archived.html` & `magplan-3.3.0/src/magplan/templates/magplan/articles/archived.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/articles/default.html` & `magplan-3.3.0/src/magplan/templates/magplan/articles/default.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/articles/index.html` & `magplan-3.3.0/src/magplan/templates/magplan/articles/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/articles/whitelisted.html` & `magplan-3.3.0/src/magplan/templates/magplan/articles/whitelisted.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/authors/_form.html` & `magplan-3.3.0/src/magplan/templates/magplan/authors/_form.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/authors/edit.html` & `magplan-3.3.0/src/magplan/templates/magplan/authors/edit.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/authors/index.html` & `magplan-3.3.0/src/magplan/templates/magplan/authors/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/authors/show.html` & `magplan-3.3.0/src/magplan/templates/magplan/authors/show.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/ideas/_approve_ideas.html` & `magplan-3.3.0/src/magplan/templates/magplan/ideas/_approve_ideas.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/ideas/_authors_list.html` & `magplan-3.3.0/src/magplan/templates/magplan/ideas/_authors_list.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/ideas/_form_base.html` & `magplan-3.3.0/src/magplan/templates/magplan/ideas/_form_base.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/ideas/_vote.html` & `magplan-3.3.0/src/magplan/templates/magplan/ideas/_vote.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/ideas/_voting_results.html` & `magplan-3.3.0/src/magplan/templates/magplan/ideas/_voting_results.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/ideas/index.html` & `magplan-3.3.0/src/magplan/templates/magplan/ideas/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/ideas/show.html` & `magplan-3.3.0/src/magplan/templates/magplan/ideas/show.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/index/index.html` & `magplan-3.3.0/src/magplan/templates/magplan/index/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/issues/_form.html` & `magplan-3.3.0/src/magplan/templates/magplan/issues/_form.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/issues/index.html` & `magplan-3.3.0/src/magplan/templates/magplan/issues/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/issues/show.html` & `magplan-3.3.0/src/magplan/templates/magplan/issues/show.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/partials/_navbar.sites.html` & `magplan-3.3.0/src/magplan/templates/magplan/partials/_navbar.sites.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/partials/_navbar_header_links.html` & `magplan-3.3.0/src/magplan/templates/magplan/partials/_navbar_header_links.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/partials/comments.html` & `magplan-3.3.0/src/magplan/templates/magplan/partials/comments.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/partials/navbar.html` & `magplan-3.3.0/src/magplan/templates/magplan/partials/navbar.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/partials/posts_table.html` & `magplan-3.3.0/src/magplan/templates/magplan/partials/posts_table.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/posts/_admin_set_stage.html` & `magplan-3.3.0/src/magplan/templates/magplan/posts/_admin_set_stage.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/posts/_attachments.html` & `magplan-3.3.0/src/magplan/templates/magplan/posts/_attachments.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/posts/_field_col.html` & `magplan-3.3.0/src/magplan/templates/magplan/posts/_field_col.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/posts/_form_base.html` & `magplan-3.3.0/src/magplan/templates/magplan/posts/_form_base.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/posts/_form_meta.html` & `magplan-3.3.0/src/magplan/templates/magplan/posts/_form_meta.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/posts/_progress.html` & `magplan-3.3.0/src/magplan/templates/magplan/posts/_progress.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/posts/_schedule.html` & `magplan-3.3.0/src/magplan/templates/magplan/posts/_schedule.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/posts/_stages.html` & `magplan-3.3.0/src/magplan/templates/magplan/posts/_stages.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/posts/edit.html` & `magplan-3.3.0/src/magplan/templates/magplan/posts/edit.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/posts/show.html` & `magplan-3.3.0/src/magplan/templates/magplan/posts/show.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/sections/index.html` & `magplan-3.3.0/src/magplan/templates/magplan/sections/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templates/magplan/stages/index.html` & `magplan-3.3.0/src/magplan/templates/magplan/stages/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/templatetags/filters.py` & `magplan-3.3.0/src/magplan/templatetags/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import List
 
 from django import template
 from django.conf import settings
 from django.urls import reverse
 from django.utils.functional import SimpleLazyObject
 
-from magplan.models import Vote, Comment
+from magplan.models import Comment, Vote
 from magplan.utils import safe_cast
-from magplan.views import posts, ideas
+from magplan.views import ideas, posts
 
 register = template.Library()
 
 MAX_VOTE_OPTIONS_NUMBER = len(Vote.SCORE_CHOICES)
 VOTE_SCORE_STEP = 100 // (MAX_VOTE_OPTIONS_NUMBER - 1)
 FAILBACK_VOTE_INDEX = 2
 CSS_COLORS = (
```

### Comparing `magplan-3.2.0/src/magplan/urls.py` & `magplan-3.3.0/src/magplan/urls.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # from django.conf.urls import url
 from django.urls import path
 
 from magplan.views import (
-    sections,
-    stages,
+    api,
     articles,
-    ideas,
     authors,
+    ideas,
     index,
     issues,
     posts,
-    api,
     preferences,
+    sections,
+    stages,
 )
 
 urlpatterns = [
     path("sections/", sections.index, name="sections_index"),
     path("stages/", stages.index, name="stages_index"),
     path(
         "ideas/<int:idea_id>/comments/", ideas.comments, name="ideas_comments"
```

### Comparing `magplan-3.2.0/src/magplan/utils.py` & `magplan-3.3.0/src/magplan/utils.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/views/api.py` & `magplan-3.3.0/src/magplan/views/api.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/views/articles.py` & `magplan-3.3.0/src/magplan/views/articles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import datetime
 import typing as tp
 
 from django.contrib.auth.decorators import login_required
 from django.db.models import Q, QuerySet
 from django.http import HttpRequest
-from django.shortcuts import render, redirect
+from django.shortcuts import redirect, render
 from django.urls import reverse
 from django.utils.timezone import now
 
 from magplan.forms import (
-    WhitelistedPostExtendedModelForm,
     AdPostExtendedModelForm,
-    DefaultPostModelForm,
     ArchivedPostModelForm,
+    DefaultPostModelForm,
+    WhitelistedPostExtendedModelForm,
 )
 from magplan.models import Post, Stage, User
 from magplan.utils import get_current_site
 
 
 def _get_filtered_posts_queryset(
     filter_: tp.Optional[str], current_user: User, queryset: QuerySet = None
```

### Comparing `magplan-3.2.0/src/magplan/views/authors.py` & `magplan-3.3.0/src/magplan/views/authors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from django.contrib import messages
-from django.contrib.auth.decorators import login_required
-from django.contrib.auth.decorators import permission_required
+from django.contrib.auth.decorators import login_required, permission_required
 from django.db.models import Q
-from django.shortcuts import render, redirect
+from django.shortcuts import redirect, render
 
-from magplan.models import User, Post
-from magplan.forms import UserModelForm, ProfileModelForm
+from magplan.forms import ProfileModelForm, UserModelForm
+from magplan.models import Post, User
 
 
 @login_required
 @permission_required("magplan.manage_authors")
 def index(request):
     users = (
         User.objects.prefetch_related("profile")
@@ -28,17 +27,15 @@
 
         if user_form.is_valid() and profile_form.is_valid():
             user = user_form.save(commit=False)
             # Authors should be inactive by default
             user.is_active = False
             user.save()
 
-            profile_form = ProfileModelForm(
-                request.POST, instance=user.profile
-            )
+            profile_form = ProfileModelForm(request.POST, instance=user.profile)
             profile_form.save()
 
             messages.add_message(
                 request, messages.INFO, f"Автор «{user}» успешно создан"
             )
 
             return redirect("authors_edit", user.id)
```

### Comparing `magplan-3.2.0/src/magplan/views/ideas.py` & `magplan-3.3.0/src/magplan/views/ideas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import datetime
 import os
-from typing import List, Tuple, Optional
+from typing import List, Optional, Tuple
 
 import django_filters
 import html2text
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required
 from django.core.mail import EmailMultiAlternatives
 from django.db.models import Count
 from django.shortcuts import redirect, render
 from django.template.loader import render_to_string
 from django.urls import reverse
+
 from magplan.conf import settings as config
 from magplan.forms import (
+    IDEA_AUTHOR_SELF_CHOICE,
     CommentModelForm,
     IdeaModelForm,
     PostBaseModelForm,
-    IDEA_AUTHOR_SELF_CHOICE,
 )
 from magplan.models import Idea, Issue, Vote
 from magplan.tasks.send_idea_comment_notification import (
     send_idea_comment_notification,
 )
 from magplan.tasks.send_idea_notification import send_idea_notification
 from magplan.utils import safe_cast
@@ -155,16 +156,15 @@
 @login_required
 def show(request, idea_id):
     idea = Idea.objects.prefetch_related("votes__user").get(id=idea_id)
     initial_issues_suggesion, issues_suggesions = _get_suggestion_issues()
     form = PostBaseModelForm(
         initial={
             "issues": initial_issues_suggesion,
-            "finished_at": datetime.datetime.now()
-            + datetime.timedelta(days=3),
+            "finished_at": datetime.datetime.now() + datetime.timedelta(days=3),
         },
         instance=idea,
     )
 
     api_authors_search_url = reverse("api_authors_search")
     api_issues_search_url = reverse("api_issues_search")
 
@@ -204,17 +204,15 @@
 
     if score not in allowed_scored:
         score = Vote.SCORE_50
 
     vote.score = score
     vote.save()
 
-    messages.add_message(
-        request, messages.SUCCESS, "Ваш голос учтен. Спасибо!"
-    )
+    messages.add_message(request, messages.SUCCESS, "Ваш голос учтен. Спасибо!")
 
     return redirect("ideas_show", idea_id=idea.id)
 
 
 @login_required
 def approve(request, idea_id):
     idea = Idea.objects.prefetch_related("votes__user").get(id=idea_id)
```

### Comparing `magplan-3.2.0/src/magplan/views/index.py` & `magplan-3.3.0/src/magplan/views/index.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/views/issues.py` & `magplan-3.3.0/src/magplan/views/issues.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from django.shortcuts import render
-from magplan.models import Issue, Magazine
 from django.contrib.auth.decorators import login_required
+from django.shortcuts import HttpResponse, redirect, render
+
 from magplan.forms import IssueModelForm
-from django.shortcuts import render, HttpResponse, redirect
+from magplan.models import Issue, Magazine
 
 
 # Create your views here.
 @login_required
 def index(request):
     issues = (
         Issue.on_current_site.all()
```

### Comparing `magplan-3.2.0/src/magplan/views/posts.py` & `magplan-3.3.0/src/magplan/views/posts.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,42 +4,44 @@
 from typing import List, Optional
 from zipfile import ZIP_DEFLATED, ZipFile
 
 import html2text
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required
+from django.contrib.sites.models import Site
 from django.core.mail import EmailMultiAlternatives
 from django.db import transaction
 from django.http import HttpRequest, HttpResponseForbidden
-from django.shortcuts import HttpResponse, redirect, render
-from django.shortcuts import get_object_or_404
+from django.shortcuts import HttpResponse, get_object_or_404, redirect, render
 from django.template import Context, Template
 from django.template.loader import render_to_string
 from django.urls import reverse
+from slugify import slugify
+
 from magplan.conf import settings as config
 from magplan.forms import (
     CommentModelForm,
     PostBaseModelForm,
     PostExtendedModelForm,
     PostMetaForm,
 )
 from magplan.models import (
     Attachment,
     Comment,
     Idea,
     Post,
     Stage,
     User,
+    current_site_id,
 )
 from magplan.tasks.send_post_comment_notification import (
     send_post_comment_notification,
 )
 from magplan.tasks.upload_post_to_wp import upload_post_to_wp
-from slugify import slugify
 
 IMAGE_MIME_TYPE_JPEG = "image/jpeg"
 IMAGE_MIME_TYPES = {
     "image/gif",
     IMAGE_MIME_TYPE_JPEG,
     "image/png",
 }
@@ -51,15 +53,23 @@
     Used to render some arbitrary HTML code in a context of Post instance.
     Useful to provide sensitive HTML template, which can't be committed
     into Git repository directly or may vary for each particular instance.
 
     :param post: Post instance to use in template
     :return: Rendered template string
     """
-    instance_template = Template(config.PLAN_POSTS_INSTANCE_CHUNK)
+
+    site = Site.objects.get(id=current_site_id())
+    chunk: Optional[str] = site.preferences[
+        "general__pre_post_content_chunk_template"
+    ]
+    if not chunk:
+        return ""
+
+    instance_template = Template(chunk)
     instance_chunk = instance_template.render(Context({"post": post}))
     return instance_chunk
 
 
 def _create_system_comment(
     action_type, user, post, changelog=None, attachments=None, stage=None
 ) -> Comment:
@@ -291,17 +301,15 @@
 @login_required
 def edit(request, post_id):
     post = Post.objects.prefetch_related(
         "editor", "authors", "stage", "section", "issues"
     ).get(id=post_id)
 
     if request.method == "POST":
-        form = PostExtendedModelForm(
-            request.POST, request.FILES, instance=post
-        )
+        form = PostExtendedModelForm(request.POST, request.FILES, instance=post)
 
         attachments_files = request.FILES.getlist("attachments")
         featured_image_files = request.FILES.getlist("featured_image")
         attachments = _save_attachments(
             attachments_files,
             post,
             request.user.user,
@@ -406,17 +414,15 @@
         if not _authorize_stage_change(request.user.user, post, new_stage_id):
             return HttpResponseForbidden()
 
         stage = Stage.objects.get(id=new_stage_id)
 
         # set deadline to current stage durtion. If no duration, append 1 day
         duration = stage.duration if stage.duration else 1
-        post.finished_at = post.finished_at + +datetime.timedelta(
-            days=duration
-        )
+        post.finished_at = post.finished_at + +datetime.timedelta(days=duration)
         post.stage = stage
         post.imprint_updater(request.user.user)
         post.save()
         messages.add_message(
             request, messages.INFO, "Текущий этап статьи «%s» обновлен" % post
         )
```

### Comparing `magplan-3.2.0/src/magplan/views/preferences.py` & `magplan-3.3.0/src/magplan/views/preferences.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/xmd/lexers.py` & `magplan-3.3.0/src/magplan/xmd/lexers.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/xmd/mappers.py` & `magplan-3.3.0/src/magplan/xmd/mappers.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/xmd/markdown.py` & `magplan-3.3.0/src/magplan/xmd/markdown.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/xmd/renderer.py` & `magplan-3.3.0/src/magplan/xmd/renderer.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/src/magplan/xmd/tests/test_lexer.py` & `magplan-3.3.0/src/magplan/xmd/tests/test_lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from unittest import TestCase
 
-from tests.plan.tasks.test_utils import get_
 from xmd.lexers import PanelBlockLexer
 
+from tests.plan.tasks.test_utils import get_
+
 
 class TestPanelBlockLexer(TestCase):
     def setUp(self):
         self.lexer = PanelBlockLexer()
 
     def test_basic(self):
         markdown = "[ Panel title\n" "\n" "Panel content\n" "\n" "]"
```

### Comparing `magplan-3.2.0/src/magplan/xmd/tests/test_renderer.py` & `magplan-3.3.0/src/magplan/xmd/tests/test_renderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 wrapped inside `<p></p>\n`. Thats why every block
 
 test should include this wrapper tag.
 """
 
 from io import BytesIO
 from unittest import TestCase
-from unittest.mock import patch, Mock
+from unittest.mock import Mock, patch
 
 import pytest
 from django.core.files import File
 from django_dynamic_fixture import G
 
 from magplan.models import Attachment
-from magplan.xmd.renderer import XMDRenderer
 from magplan.xmd.mappers import plan_internal_mapper
+from magplan.xmd.renderer import XMDRenderer
 
 
 @pytest.mark.django_db
 class TestImage(TestCase):
     MOCK_SRC = "dummy.jpg"
     MOCK_TITLE = "title"
     MOCK_ALT_TEXT = "alt_text"
```

### Comparing `magplan-3.2.0/src/magplan/xmd/tests/test_utils.py` & `magplan-3.3.0/src/magplan/xmd/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,11 +32,9 @@
         # So e're checking only filename matches.
         filename = get_attachment_original_filename(
             "user_friendly_filename1.jpg", self.attachments
         )
         assert "file1" in filename
 
     def test_non_existing_filename(self):
-        filename = get_attachment_original_filename(
-            "404.jpg", self.attachments
-        )
+        filename = get_attachment_original_filename("404.jpg", self.attachments)
         assert not filename
```

### Comparing `magplan-3.2.0/src/magplan/xmd/xmd.py` & `magplan-3.3.0/src/magplan/xmd/xmd.py`

 * *Files identical despite different names*

### Comparing `magplan-3.2.0/PKG-INFO` & `magplan-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magplan
-Version: 3.2.0
+Version: 3.3.0
 Summary: 
 Author: Ilya Rusanen
 Author-email: ilya@rusanen.co.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

