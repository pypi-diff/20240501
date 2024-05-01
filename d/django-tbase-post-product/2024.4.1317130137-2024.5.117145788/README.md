# Comparing `tmp/django_tbase_post_product-2024.4.1317130137.tar.gz` & `tmp/django_tbase_post_product-2024.5.117145788.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2024.4.1317130137.tar", last modified: Sat Apr 13 13:09:13 2024, max compression
+gzip compressed data, was "django_tbase_post_product-2024.5.117145788.tar", last modified: Wed May  1 15:53:49 2024, max compression
```

## Comparing `django_tbase_post_product-2024.4.1317130137.tar` & `django_tbase_post_product-2024.5.117145788.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.168593 django_tbase_post_product-2024.4.1317130137/
--rw-rw-r--   0 terry     (1000) terry     (1000)      143 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.4.1317130137/MANIFEST.in
--rw-rw-r--   0 terry     (1000) terry     (1000)     1900 2024-04-13 13:09:13.168593 django_tbase_post_product-2024.4.1317130137/PKG-INFO
--rw-rw-r--   0 terry     (1000) terry     (1000)     1577 2024-04-13 13:07:21.000000 django_tbase_post_product-2024.4.1317130137/README.md
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.160593 django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/
--rw-rw-r--   0 terry     (1000) terry     (1000)     1900 2024-04-13 13:09:13.000000 django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/PKG-INFO
--rw-rw-r--   0 terry     (1000) terry     (1000)     1983 2024-04-13 13:09:13.000000 django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/SOURCES.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)        1 2024-04-13 13:09:13.000000 django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/dependency_links.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       83 2024-04-13 13:09:13.000000 django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/requires.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       11 2024-04-13 13:09:13.000000 django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/top_level.txt
--rw-rw-r--   0 terry     (1000) terry     (1000)       38 2024-04-13 13:09:13.168593 django_tbase_post_product-2024.4.1317130137/setup.cfg
--rw-rw-r--   0 terry     (1000) terry     (1000)     2305 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.4.1317130137/setup.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/
--rw-rw-r--   0 terry     (1000) terry     (1000)     7569 2024-03-12 15:28:36.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/0001_initial.py
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     6331 2024-03-13 03:45:25.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/admin.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      146 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/apps.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/migrations/
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-12-03 07:39:38.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/migrations/__init__.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    10357 2024-04-13 13:06:33.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/models.py
--rw-rw-r--   0 terry     (1000) terry     (1000)      616 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/sitemaps.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.160593 django_tbase_post_product-2024.4.1317130137/tbase_post/static/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/static/images/
--rw-rw-r--   0 terry     (1000) terry     (1000)    59619 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
--rw-rw-r--   0 terry     (1000) terry     (1000)       94 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/
--rw-rw-r--   0 terry     (1000) terry     (1000)     5494 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/article_list_by_tag.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2994 2024-04-13 11:28:01.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/blog_index.html
--rw-rw-r--   0 terry     (1000) terry     (1000)    11325 2024-04-13 11:36:48.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/detail.html
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/
--rw-rw-r--   0 terry     (1000) terry     (1000)      732 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/amazon_ads.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      591 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/amazon_link.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      884 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/hitcount_lowest_post.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      818 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/hitcount_top_post.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     1946 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/last_update.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     1796 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/related_post_by_tags.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      827 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/seo_top_links.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      569 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/tags.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      132 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/templ.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      576 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/youtube_player.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2109 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/last_index.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      255 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_detail copy.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     4751 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_detail.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      426 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_list.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     2483 2024-03-13 03:47:25.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_post_detail.html
--rw-rw-r--   0 terry     (1000) terry     (1000)     4733 2024-03-13 03:36:27.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_post_list.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      765 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post_list.html
--rw-rw-r--   0 terry     (1000) terry     (1000)      391 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templates/sitemap.xml
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.164593 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/
--rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__init__.py
-drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-04-13 13:09:13.168593 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/
--rw-rw-r--   0 terry     (1000) terry     (1000)      196 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)      190 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     6290 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)     4111 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc
--rw-rw-r--   0 terry     (1000) terry     (1000)    11661 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/post_extras.py
--rw-rw-r--   0 terry     (1000) terry     (1000)       60 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/tests.py
--rw-rw-r--   0 terry     (1000) terry     (1000)     1571 2024-03-13 03:17:25.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/urls.py
--rw-rw-r--   0 terry     (1000) terry     (1000)    11928 2024-03-13 03:43:23.000000 django_tbase_post_product-2024.4.1317130137/tbase_post/views.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.994354 django_tbase_post_product-2024.5.117145788/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      143 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.5.117145788/MANIFEST.in
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1961 2024-05-01 15:53:49.994354 django_tbase_post_product-2024.5.117145788/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1639 2024-05-01 15:48:38.000000 django_tbase_post_product-2024.5.117145788/README.md
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.990354 django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1961 2024-05-01 15:53:49.000000 django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/PKG-INFO
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1983 2024-05-01 15:53:49.000000 django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)        1 2024-05-01 15:53:49.000000 django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       83 2024-05-01 15:53:49.000000 django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/requires.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       11 2024-05-01 15:53:49.000000 django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/top_level.txt
+-rw-rw-r--   0 terry     (1000) terry     (1000)       38 2024-05-01 15:53:49.994354 django_tbase_post_product-2024.5.117145788/setup.cfg
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2305 2023-12-03 08:49:22.000000 django_tbase_post_product-2024.5.117145788/setup.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.990354 django_tbase_post_product-2024.5.117145788/tbase_post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     7569 2024-03-12 15:28:36.000000 django_tbase_post_product-2024.5.117145788/tbase_post/0001_initial.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/__init__.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     6331 2024-03-13 03:45:25.000000 django_tbase_post_product-2024.5.117145788/tbase_post/admin.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      146 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/apps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.990354 django_tbase_post_product-2024.5.117145788/tbase_post/migrations/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2023-12-03 07:39:38.000000 django_tbase_post_product-2024.5.117145788/tbase_post/migrations/__init__.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)    10357 2024-04-13 13:06:33.000000 django_tbase_post_product-2024.5.117145788/tbase_post/models.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)      616 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/sitemaps.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.986354 django_tbase_post_product-2024.5.117145788/tbase_post/static/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.990354 django_tbase_post_product-2024.5.117145788/tbase_post/static/images/
+-rw-rw-r--   0 terry     (1000) terry     (1000)    59619 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-rw-r--   0 terry     (1000) terry     (1000)       94 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.990354 django_tbase_post_product-2024.5.117145788/tbase_post/templates/
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.990354 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/
+-rw-rw-r--   0 terry     (1000) terry     (1000)     5494 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/article_list_by_tag.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2994 2024-04-13 11:28:01.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/blog_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)    11328 2024-05-01 15:47:31.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/detail.html
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.994354 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      732 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/amazon_ads.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      591 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/amazon_link.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      884 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/hitcount_lowest_post.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      818 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/hitcount_top_post.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1926 2024-05-01 15:53:21.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/last_update.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1822 2024-05-01 15:53:08.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      827 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/seo_top_links.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      569 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/tags.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      132 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/templ.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      576 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/youtube_player.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2109 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/last_index.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      255 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_detail copy.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4751 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_detail.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      426 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_list.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     2483 2024-03-13 03:47:25.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_post_detail.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4733 2024-03-13 03:36:27.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_post_list.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      765 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/post_list.html
+-rw-rw-r--   0 terry     (1000) terry     (1000)      391 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templates/sitemap.xml
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.994354 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/
+-rw-rw-r--   0 terry     (1000) terry     (1000)        0 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__init__.py
+drwxrwxr-x   0 terry     (1000) terry     (1000)        0 2024-05-01 15:53:49.994354 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/
+-rw-rw-r--   0 terry     (1000) terry     (1000)      196 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)      190 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     6290 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)     4111 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc
+-rw-rw-r--   0 terry     (1000) terry     (1000)    11661 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/post_extras.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)       60 2024-03-12 16:23:05.000000 django_tbase_post_product-2024.5.117145788/tbase_post/tests.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)     1571 2024-03-13 03:17:25.000000 django_tbase_post_product-2024.5.117145788/tbase_post/urls.py
+-rw-rw-r--   0 terry     (1000) terry     (1000)    11928 2024-03-13 03:43:23.000000 django_tbase_post_product-2024.5.117145788/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2024.4.1317130137/PKG-INFO` & `django_tbase_post_product-2024.5.117145788/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tbase_post_product
-Version: 2024.4.1317130137
+Version: 2024.5.117145788
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
@@ -33,14 +33,18 @@
 
  ]
 ```
 
 
 ## 更新
 
+- 2024/05/1
+注销掉底部广告（banner-amazon-footer）
+
+
 - 2024/04/13
 优化展示
 
 - 2024/03/13
 添加post对应提示词列表，添加对应跳转
 
 - 2024/03/12
```

### Comparing `django_tbase_post_product-2024.4.1317130137/README.md` & `django_tbase_post_product-2024.5.117145788/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 
  ]
 ```
 
 
 ## 更新
 
+- 2024/05/1
+注销掉底部广告（banner-amazon-footer）
+
+
 - 2024/04/13
 优化展示
 
 - 2024/03/13
 添加post对应提示词列表，添加对应跳转
 
 - 2024/03/12
```

### Comparing `django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tbase-post-product
-Version: 2024.4.1317130137
+Version: 2024.5.117145788
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
@@ -33,14 +33,18 @@
 
  ]
 ```
 
 
 ## 更新
 
+- 2024/05/1
+注销掉底部广告（banner-amazon-footer）
+
+
 - 2024/04/13
 优化展示
 
 - 2024/03/13
 添加post对应提示词列表，添加对应跳转
 
 - 2024/03/12
```

### Comparing `django_tbase_post_product-2024.4.1317130137/django_tbase_post_product.egg-info/SOURCES.txt` & `django_tbase_post_product-2024.5.117145788/django_tbase_post_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/setup.py` & `django_tbase_post_product-2024.5.117145788/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/0001_initial.py` & `django_tbase_post_product-2024.5.117145788/tbase_post/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/admin.py` & `django_tbase_post_product-2024.5.117145788/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/models.py` & `django_tbase_post_product-2024.5.117145788/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/sitemaps.py` & `django_tbase_post_product-2024.5.117145788/tbase_post/sitemaps.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg` & `django_tbase_post_product-2024.5.117145788/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/article_list_by_tag.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/article_list_by_tag.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/blog_index.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/blog_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/detail.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/detail.html`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
 $('#banner-amazon').html(htmlStr)
 
 data={}
 var htmlStr = template('banner-img-tpl', data)
 $('#banner-img').html(htmlStr)
 data={}
 var htmlStr = template('banner-amazon-footer-tpl', data)
-$('#banner-amazon-footer').html(htmlStr)
+// $('#banner-amazon-footer').html(htmlStr)
 
 </script>
 
  
 <!--标签-->
 {% tags object.tags 5 object.pk %}
  <!--标签end-->
```

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/amazon_ads.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/amazon_ads.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/amazon_link.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/amazon_link.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/hitcount_lowest_post.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/hitcount_lowest_post.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/hitcount_top_post.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/hitcount_top_post.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/last_update.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/last_update.html`

 * *Files 7% similar despite different names*

```diff
@@ -3,55 +3,47 @@
 # 加载标签
 load post_extras
 
 使用示例：
 last_update 5
 
 -->
-{% load cache %}
-{% cache 3600 last_update_block pk %}
+<!-- {% load cache %}
+{% cache 3600 last_update_block pk %} -->
 
 <div class="last_update">
   <h2 class="text-gray-800 text-lg font-medium mb-2">{{title}}</h2>
   <div class="list-disc" >
 
 
     {%for item in page_obj%}
-    
-    
-    
+     
           <div class="max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700 my-2">
             <a  rel="nofollow" href="{% url 'detail_view' item.pk %}" >
-                <img class="h-60 mx-auto" src="{{ item.article_img}}" alt="" />
+                <img class="h-60 mx-auto" src="{{ item.article_img}}" alt="{{item}}" />
             </a>
             <div class="p-5">
                 <a  href="{% url 'detail_view' item.pk %}"  >
-                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">{{item|truncatechars:32}}</h5>
+                    <h5 class="mb-2 text-1xl font-bold tracking-tight text-gray-900 dark:text-white">{{item|truncatechars:32}}</h5>
                 </a>
                 <!-- <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">{{item|truncatechars:32}}
     
                 </p>
                 <a rel="nofollow" href="{% url 'detail_view' item.pk %}" class="inline-flex items-center px-3 py-2 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
                     Read more
                      <svg class="w-3.5 h-3.5 ml-2" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 10">
                         <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 5h12m0 0L9 1m4 4L9 9"/>
                     </svg>
                 </a> -->
             </div>
         </div>
-        
-    
-    
-    
-    
-    
-    
+ 
     
             <!-- <a href="{% url 'detail_view' item.pk %}" class="">{{item|truncatechars:32}}</a> -->
         <!-- </li> -->
     {%endfor%}
       <!-- </ul> -->
     
     </div>
 </div>
 
-{% endcache %}
+<!-- {% endcache %} -->
```

#### html2text {}

```diff
@@ -1,6 +1,5 @@
-{% load cache %} {% cache 3600 last_update_block pk %}
 ********** {{{{ttiittllee}}}} **********
 {%for item in page_obj%}
+_[_{_{_i_t_e_m_}_}_]
 _**_**_ _{{_{{_ii_tt_ee_mm_||_tt_rr_uu_nn_cc_aa_tt_ee_cc_hh_aa_rr_ss_::_33_22_}}_}}_ _**_**
 {%endfor%}
-{% endcache %}
```

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/related_post_by_tags.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/related_post_by_tags.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-{% load cache %}
-{% cache 3600 related_post_by_tags_block pk %}
+<!-- {% load cache %}
+{% cache 3600 related_post_by_tags_block pk %} -->
 <div>
       <h2 class="text-gray-800 text-lg font-medium mb-2">{{title}}</h2>
         <!-- <ul class="list-disc pl-4"> -->
 
           <div class="list-disc" >
 
 
@@ -20,19 +20,19 @@
     <!-- <li class="mb-2"> -->
 
 
 
 
       <div class="max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700 my-2">
         <a  rel="nofollow" href="{% url 'detail_view' item.pk %}" >
-            <img class="h-60 mx-auto" src="{{ item.article_img}}" alt="" />
+            <img class="h-60 mx-auto" src="{{ item.article_img}}" alt="{{item}}" />
         </a>
         <div class="p-5">
             <a  href="{% url 'detail_view' item.pk %}"  >
-                <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">{{item|truncatechars:32}}</h5>
+                <h5 class="mb-2 text-1xl font-bold tracking-tight text-gray-900 dark:text-white">{{item|truncatechars:32}}</h5>
             </a>
             <!-- <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">{{item|truncatechars:32}}
 
             </p>
             <a rel="nofollow" href="{% url 'detail_view' item.pk %}" class="inline-flex items-center px-3 py-2 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
                 Read more
                  <svg class="w-3.5 h-3.5 ml-2" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 10">
@@ -52,8 +52,8 @@
         <!-- <a href="{% url 'detail_view' item.pk %}" class="">{{item|truncatechars:32}}</a> -->
     <!-- </li> -->
 {%endfor%}
   <!-- </ul> -->
 
 </div>
 </div>
-{% endcache %}
+<!-- {% endcache %} -->
```

#### html2text {}

```diff
@@ -1,6 +1,5 @@
-{% load cache %} {% cache 3600 related_post_by_tags_block pk %}
 ********** {{{{ttiittllee}}}} **********
 {%for item in page_obj%}
+_[_{_{_i_t_e_m_}_}_]
 _**_**_ _{{_{{_ii_tt_ee_mm_||_tt_rr_uu_nn_cc_aa_tt_ee_cc_hh_aa_rr_ss_::_33_22_}}_}}_ _**_**
 {%endfor%}
-{% endcache %}
```

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/seo_top_links.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/seo_top_links.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/tags.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/tags.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/extras/youtube_player.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/extras/youtube_player.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/last_index.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/last_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_detail.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_detail.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_post_detail.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_post_detail.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post/prompt_task_post_list.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post/prompt_task_post_list.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templates/post_list.html` & `django_tbase_post_product-2024.5.117145788/tbase_post/templates/post_list.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc` & `django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc` & `django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/__pycache__/post_extras.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/templatetags/post_extras.py` & `django_tbase_post_product-2024.5.117145788/tbase_post/templatetags/post_extras.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/urls.py` & `django_tbase_post_product-2024.5.117145788/tbase_post/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2024.4.1317130137/tbase_post/views.py` & `django_tbase_post_product-2024.5.117145788/tbase_post/views.py`

 * *Files identical despite different names*

