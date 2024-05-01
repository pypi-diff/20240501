# Comparing `tmp/wagtail-cjkcms-24.3.2.tar.gz` & `tmp/wagtail_cjkcms-24.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-cjkcms-24.3.2.tar", last modified: Wed Mar 20 09:05:10 2024, max compression
+gzip compressed data, was "wagtail_cjkcms-24.5.1.tar", last modified: Wed May  1 20:41:15 2024, max compression
```

## Comparing `wagtail-cjkcms-24.3.2.tar` & `wagtail_cjkcms-24.5.1.tar`

### file list

```diff
@@ -1,465 +1,470 @@
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.380681 wagtail-cjkcms-24.3.2/
--rw-r--r--   0 dev       (1000) dev       (1000)     4888 2024-03-20 09:03:02.000000 wagtail-cjkcms-24.3.2/CHANGELOG.md
--rw-r--r--   0 dev       (1000) dev       (1000)     1538 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/LICENSE
--rw-r--r--   0 dev       (1000) dev       (1000)      158 2024-02-18 21:07:46.000000 wagtail-cjkcms-24.3.2/MANIFEST.in
--rw-r--r--   0 dev       (1000) dev       (1000)     3106 2024-03-20 09:05:10.380681 wagtail-cjkcms-24.3.2/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)     1613 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/README.md
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.280681 wagtail-cjkcms-24.3.2/cjkcms/
--rw-r--r--   0 dev       (1000) dev       (1000)      272 2024-03-20 09:03:19.000000 wagtail-cjkcms-24.3.2/cjkcms/__init__.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.284681 wagtail-cjkcms-24.3.2/cjkcms/api/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/api/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2832 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/api/mailchimp.py
--rw-r--r--   0 dev       (1000) dev       (1000)      173 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/apps.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.284681 wagtail-cjkcms-24.3.2/cjkcms/bin/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/bin/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)     5763 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/bin/cjkcms.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.284681 wagtail-cjkcms-24.3.2/cjkcms/blocks/
--rw-r--r--   0 dev       (1000) dev       (1000)     3402 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/blocks/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)    11616 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/blocks/base_blocks.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.284681 wagtail-cjkcms-24.3.2/cjkcms/blocks/content/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/blocks/content/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1967 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/blocks/content/events.py
--rw-r--r--   0 dev       (1000) dev       (1000)     8890 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/blocks/content_blocks.py
--rw-r--r--   0 dev       (1000) dev       (1000)     9543 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/blocks/html_blocks.py
--rw-r--r--   0 dev       (1000) dev       (1000)     3406 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/blocks/layout_blocks.py
--rw-r--r--   0 dev       (1000) dev       (1000)      171 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/blocks/searchable_html_block.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.284681 wagtail-cjkcms-24.3.2/cjkcms/draftail/
--rw-r--r--   0 dev       (1000) dev       (1000)      240 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/draftail/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)     3250 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/draftail/draftail_extensions.py
--rw-r--r--   0 dev       (1000) dev       (1000)     3191 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/fields.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.284681 wagtail-cjkcms-24.3.2/cjkcms/finders/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/finders/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2760 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/finders/oembed.py
--rw-r--r--   0 dev       (1000) dev       (1000)      361 2024-02-18 13:58:21.000000 wagtail-cjkcms-24.3.2/cjkcms/forms.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1833 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/image_formats.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.268682 wagtail-cjkcms-24.3.2/cjkcms/management/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.284681 wagtail-cjkcms-24.3.2/cjkcms/management/commands/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/management/commands/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)      453 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/management/commands/clear-embeds.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2565 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/management/commands/import-csv.py
--rw-r--r--   0 dev       (1000) dev       (1000)      951 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/management/commands/init-collections.py
--rw-r--r--   0 dev       (1000) dev       (1000)     3560 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/management/commands/init-navbar.py
--rw-r--r--   0 dev       (1000) dev       (1000)     3820 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/management/commands/init-website.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.288681 wagtail-cjkcms-24.3.2/cjkcms/migrations/
--rw-r--r--   0 dev       (1000) dev       (1000)  2070677 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0001_initial.py
--rw-r--r--   0 dev       (1000) dev       (1000)      924 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
--rw-r--r--   0 dev       (1000) dev       (1000)      727 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1026 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1708 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2885 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
--rw-r--r--   0 dev       (1000) dev       (1000)      593 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1334 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py
--rw-r--r--   0 dev       (1000) dev       (1000)      685 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0009_navbar_language.py
--rw-r--r--   0 dev       (1000) dev       (1000)     3479 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0010_filmstrip_filmpanel.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1393 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1466 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0012_remove_analyticssettings_ga_tracking_id_and_more.py
--rw-r--r--   0 dev       (1000) dev       (1000)      780 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0013_socialmediasettings_location.py
--rw-r--r--   0 dev       (1000) dev       (1000)      818 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0014_navbar_alignment.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1467 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0015_eventcalendar.py
--rw-r--r--   0 dev       (1000) dev       (1000)      918 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0016_layoutsettings_breadcrumb_icon_and_more.py
--rw-r--r--   0 dev       (1000) dev       (1000)      788 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0017_layoutsettings_default_seo_image.py
--rw-r--r--   0 dev       (1000) dev       (1000)      478 2024-02-18 13:58:42.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0018_layoutsettings_search_format.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1220 2024-02-18 22:01:17.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0019_layoutsettings_searchbox_input_class_and_more.py
--rw-r--r--   0 dev       (1000) dev       (1000)      922 2024-03-11 19:20:33.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/0020_socialmediasettings_github_and_more.py
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/migrations/__init__.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.288681 wagtail-cjkcms-24.3.2/cjkcms/models/
--rw-r--r--   0 dev       (1000) dev       (1000)      232 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/models/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)      665 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/models/admin_sidebar.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2356 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/models/cms_models.py
--rw-r--r--   0 dev       (1000) dev       (1000)     6302 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/models/integration_models.py
--rw-r--r--   0 dev       (1000) dev       (1000)    24525 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/models/page_models.py
--rw-r--r--   0 dev       (1000) dev       (1000)    16837 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/models/snippet_models.py
--rw-r--r--   0 dev       (1000) dev       (1000)    22404 2024-03-11 19:19:42.000000 wagtail-cjkcms-24.3.2/cjkcms/models/wagtailsettings_models.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.268682 wagtail-cjkcms-24.3.2/cjkcms/project_template/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.292682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/
--rw-r--r--   0 dev       (1000) dev       (1000)      722 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/.editorconfig
--rw-r--r--   0 dev       (1000) dev       (1000)      364 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/.gitattributes
--rw-r--r--   0 dev       (1000) dev       (1000)      275 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/.gitignore
--rw-r--r--   0 dev       (1000) dev       (1000)      792 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/README.md
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.292682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/__init__.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.292682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/blocks/
--rw-r--r--   0 dev       (1000) dev       (1000)      137 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/blocks/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2141 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/blocks/blocks.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.292682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/migrations/
--rw-r--r--   0 dev       (1000) dev       (1000)     4981 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/migrations/0001_initial.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2047 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/migrations/0002_create_homepage.py
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/migrations/__init__.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.292682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/models/
--rw-r--r--   0 dev       (1000) dev       (1000)      383 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/models/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)     3106 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/models/cms_models.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.268682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/templates/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.268682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/templates/home/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.292682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/templates/home/blocks/
--rw-r--r--   0 dev       (1000) dev       (1000)     2282 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/templates/home/blocks/event_presentation.html
--rw-r--r--   0 dev       (1000) dev       (1000)      678 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/manage.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.292682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/__init__.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.292682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/settings/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/settings/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)     5477 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/settings/base.py
--rw-r--r--   0 dev       (1000) dev       (1000)      324 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/settings/dev.py
--rw-r--r--   0 dev       (1000) dev       (1000)      705 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/settings/local.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1595 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/settings/production.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.268682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/static/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.292682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/static/css/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/static/css/devsite.css
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.292682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/static/js/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/static/js/devsite.js
--rw-r--r--   0 dev       (1000) dev       (1000)      911 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/urls.py
--rw-r--r--   0 dev       (1000) dev       (1000)      432 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/wsgi.py
--rw-r--r--   0 dev       (1000) dev       (1000)      123 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/requirements.txt
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.292682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/search/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/search/__init__.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.268682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/search/templates/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.292682 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/search/templates/search/
--rw-r--r--   0 dev       (1000) dev       (1000)     1097 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/search/templates/search/search.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1019 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/search/views.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.296682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/
--rw-r--r--   0 dev       (1000) dev       (1000)      245 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/.babelrc
--rw-r--r--   0 dev       (1000) dev       (1000)      159 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/.browserslistrc
--rw-r--r--   0 dev       (1000) dev       (1000)      722 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/.editorconfig
--rw-r--r--   0 dev       (1000) dev       (1000)      277 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/.eslintrc
--rw-r--r--   0 dev       (1000) dev       (1000)      364 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/.gitattributes
--rw-r--r--   0 dev       (1000) dev       (1000)      270 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/.gitignore
--rw-r--r--   0 dev       (1000) dev       (1000)       13 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/.nvmrc
--rw-r--r--   0 dev       (1000) dev       (1000)      182 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/.stylelintrc.json
--rw-r--r--   0 dev       (1000) dev       (1000)      792 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/README.md
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.296682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/
--rw-r--r--   0 dev       (1000) dev       (1000)      131 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/.gitignore
--rw-r--r--   0 dev       (1000) dev       (1000)      733 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/README.md
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.268682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/src/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.296682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/src/application/
--rw-r--r--   0 dev       (1000) dev       (1000)      577 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/src/application/app.js
--rw-r--r--   0 dev       (1000) dev       (1000)      226 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/src/application/app2.js
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.296682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/src/components/
--rw-r--r--   0 dev       (1000) dev       (1000)       41 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/src/components/sidebar.js
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.296682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/src/styles/
--rw-r--r--   0 dev       (1000) dev       (1000)      378 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/src/styles/index.scss
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.296682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/vendors/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/vendors/.gitkeep
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.296682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/vendors/images/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/vendors/images/.gitkeep
--rw-r--r--   0 dev       (1000) dev       (1000)   104442 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/vendors/images/sample.jpg
--rw-r--r--   0 dev       (1000) dev       (1000)    25891 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/vendors/images/webpack.png
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.296682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/webpack/
--rw-r--r--   0 dev       (1000) dev       (1000)     1473 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/webpack/webpack.common.js
--rw-r--r--   0 dev       (1000) dev       (1000)     1716 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/webpack/webpack.config.dev.js
--rw-r--r--   0 dev       (1000) dev       (1000)      986 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/webpack/webpack.config.prod.js
--rw-r--r--   0 dev       (1000) dev       (1000)     1485 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/webpack/webpack.config.watch.js
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.296682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/__init__.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.296682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/blocks/
--rw-r--r--   0 dev       (1000) dev       (1000)      137 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/blocks/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2141 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/blocks/blocks.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.296682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/migrations/
--rw-r--r--   0 dev       (1000) dev       (1000)     4981 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/migrations/0001_initial.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2047 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/migrations/0002_create_homepage.py
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/migrations/__init__.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.300681 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/models/
--rw-r--r--   0 dev       (1000) dev       (1000)      391 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/models/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)     3106 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/models/cms_models.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.272682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/templates/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.272682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/templates/home/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.300681 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/templates/home/blocks/
--rw-r--r--   0 dev       (1000) dev       (1000)     2282 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/templates/home/blocks/event_presentation.html
--rw-r--r--   0 dev       (1000) dev       (1000)      678 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/manage.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1743 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/package.json
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.300681 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/__init__.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.300681 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/settings/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/settings/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)     5648 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/settings/base.py
--rw-r--r--   0 dev       (1000) dev       (1000)      324 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/settings/dev.py
--rw-r--r--   0 dev       (1000) dev       (1000)      705 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/settings/local.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1593 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/settings/production.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.272682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/static/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.300681 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/static/css/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/static/css/devsite.css
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.300681 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/static/js/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/static/js/devsite.js
--rw-r--r--   0 dev       (1000) dev       (1000)      911 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/urls.py
--rw-r--r--   0 dev       (1000) dev       (1000)      432 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/wsgi.py
--rw-r--r--   0 dev       (1000) dev       (1000)      188 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/requirements.txt
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.300681 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/search/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/search/__init__.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.272682 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/search/templates/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.300681 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/search/templates/search/
--rw-r--r--   0 dev       (1000) dev       (1000)     1097 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/search/templates/search/search.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1019 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/search/views.py
--rw-r--r--   0 dev       (1000) dev       (1000)      125 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/search_urls.py
--rw-r--r--   0 dev       (1000) dev       (1000)    19119 2024-02-18 21:48:29.000000 wagtail-cjkcms-24.3.2/cjkcms/settings.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.272682 wagtail-cjkcms-24.3.2/cjkcms/static/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.272682 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.308681 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/bi/
--rw-r--r--   0 dev       (1000) dev       (1000)    93729 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/bi/bootstrap-icons.css
--rw-r--r--   0 dev       (1000) dev       (1000)    49971 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/bi/bootstrap-icons.json
--rw-r--r--   0 dev       (1000) dev       (1000)    55169 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/bi/bootstrap-icons.scss
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.308681 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/bi/fonts/
--rw-r--r--   0 dev       (1000) dev       (1000)   164360 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
--rw-r--r--   0 dev       (1000) dev       (1000)   121340 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.312681 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/css/
--rw-r--r--   0 dev       (1000) dev       (1000)      846 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/css/cjkcms-admin.css
--rw-r--r--   0 dev       (1000) dev       (1000)     1104 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/css/cjkcms-editor.css
--rw-r--r--   0 dev       (1000) dev       (1000)     4746 2024-02-18 15:35:57.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/css/cjkcms-front.css
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.272682 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.312681 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/avatars/
--rw-r--r--   0 dev       (1000) dev       (1000)      535 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/avatars/default.png
--rw-r--r--   0 dev       (1000) dev       (1000)      384 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/avatars/default.svg
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.316681 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/icons/
--rw-r--r--   0 dev       (1000) dev       (1000)      581 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/icons/calendar-day.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      268 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/icons/caret-right-fill.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      289 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/icons/caret-right.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      291 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/icons/chevron-right.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      705 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/icons/quote.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      252 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/icons/slash.svg
--rw-r--r--   0 dev       (1000) dev       (1000)     1374 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/icons/world.svg
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.316681 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/logos/
--rw-r--r--   0 dev       (1000) dev       (1000)     4166 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
--rw-r--r--   0 dev       (1000) dev       (1000)     4218 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.320681 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/patterns/
--rw-r--r--   0 dev       (1000) dev       (1000)    47935 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
--rw-r--r--   0 dev       (1000) dev       (1000)    31707 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
--rw-r--r--   0 dev       (1000) dev       (1000)    38190 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.320681 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/js/
--rw-r--r--   0 dev       (1000) dev       (1000)      444 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/js/cjkcms-editor.js
--rw-r--r--   0 dev       (1000) dev       (1000)     5579 2024-03-20 08:58:55.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/js/cjkcms-front.js
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.320681 wagtail-cjkcms-24.3.2/cjkcms/static/cookieconsent/
--rw-r--r--   0 dev       (1000) dev       (1000)    18803 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cookieconsent/cookieconsent.css
--rw-r--r--   0 dev       (1000) dev       (1000)    18743 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/static/cookieconsent/cookieconsent.js
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.320681 wagtail-cjkcms-24.3.2/cjkcms/templates/
--rw-r--r--   0 dev       (1000) dev       (1000)     4176 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/404.html
--rw-r--r--   0 dev       (1000) dev       (1000)     4802 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/500.html
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.320681 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.336681 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/
--rw-r--r--   0 dev       (1000) dev       (1000)     1443 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/accordion_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      974 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/article_block_card.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1132 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
--rw-r--r--   0 dev       (1000) dev       (1000)      188 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/base_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)     2634 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/base_link_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      740 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/button_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      746 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      856 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_blurb.html
--rw-r--r--   0 dev       (1000) dev       (1000)      786 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_foot.html
--rw-r--r--   0 dev       (1000) dev       (1000)      730 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_head.html
--rw-r--r--   0 dev       (1000) dev       (1000)      771 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_head_foot.html
--rw-r--r--   0 dev       (1000) dev       (1000)      990 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_horizontal.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1104 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
--rw-r--r--   0 dev       (1000) dev       (1000)      786 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_img.html
--rw-r--r--   0 dev       (1000) dev       (1000)     2618 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_landing1.html
--rw-r--r--   0 dev       (1000) dev       (1000)     2758 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_landing2.html
--rw-r--r--   0 dev       (1000) dev       (1000)      678 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
--rw-r--r--   0 dev       (1000) dev       (1000)      450 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
--rw-r--r--   0 dev       (1000) dev       (1000)      277 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
--rw-r--r--   0 dev       (1000) dev       (1000)      276 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
--rw-r--r--   0 dev       (1000) dev       (1000)     2698 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/carousel_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      406 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/column_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      137 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/document_link_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      920 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/download_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      103 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/embed_video_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      308 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/event_calendar_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)       95 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/external_link_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1484 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/film_strip_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      424 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/grid_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      200 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/h1_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      200 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/h2_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      200 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/h3_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      790 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/hero_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      275 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/image_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1400 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      627 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/image_link_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1020 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/modal_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      164 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/page_link_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      787 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
--rw-r--r--   0 dev       (1000) dev       (1000)      642 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
--rw-r--r--   0 dev       (1000) dev       (1000)      361 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
--rw-r--r--   0 dev       (1000) dev       (1000)      956 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
--rw-r--r--   0 dev       (1000) dev       (1000)      858 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagelist_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      610 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1224 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
--rw-r--r--   0 dev       (1000) dev       (1000)      200 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      793 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
--rw-r--r--   0 dev       (1000) dev       (1000)      244 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pricelist_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      513 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1155 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/public_event_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      353 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/quote_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      852 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
--rw-r--r--   0 dev       (1000) dev       (1000)      998 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
--rw-r--r--   0 dev       (1000) dev       (1000)      216 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)       91 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/rich_text_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1095 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/table_block.html
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.336681 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/cookieconsent/
--rw-r--r--   0 dev       (1000) dev       (1000)     3672 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/cookieconsent/languages.html
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.340681 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/formfields/
--rw-r--r--   0 dev       (1000) dev       (1000)      267 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/formfields/date.html
--rw-r--r--   0 dev       (1000) dev       (1000)      416 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/formfields/datetime.html
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.340681 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/formfields/mailchimp/
--rw-r--r--   0 dev       (1000) dev       (1000)     9267 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
--rw-r--r--   0 dev       (1000) dev       (1000)     6469 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
--rw-r--r--   0 dev       (1000) dev       (1000)      793 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
--rw-r--r--   0 dev       (1000) dev       (1000)      264 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/formfields/time.html
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.344681 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/
--rw-r--r--   0 dev       (1000) dev       (1000)      449 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/align-center.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      462 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/align-left.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      447 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/align-right.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      891 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/card-grid.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      570 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/check-square-o.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      274 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/columns.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      356 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/desktop.svg
--rw-r--r--   0 dev       (1000) dev       (1000)     1083 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/font-decrease.svg
--rw-r--r--   0 dev       (1000) dev       (1000)     1117 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/font-increase.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      568 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/font.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      289 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/google.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      810 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      663 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/hashtag.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      837 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/header.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      832 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/list-alt.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      456 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/map.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      445 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/newspaper-o.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      718 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      632 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/recycle.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      171 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/stop.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      502 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/th-large.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      759 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/universal-access.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      545 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/usd.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      222 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/window-maximize.svg
--rw-r--r--   0 dev       (1000) dev       (1000)      196 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/window-minimize.svg
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.344681 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/includes/
--rw-r--r--   0 dev       (1000) dev       (1000)      286 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
--rw-r--r--   0 dev       (1000) dev       (1000)      689 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
--rw-r--r--   0 dev       (1000) dev       (1000)      579 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/includes/classifier_nav.html
--rw-r--r--   0 dev       (1000) dev       (1000)      268 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/includes/form_honeypot.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1061 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/includes/pagination.html
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.344681 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/includes/stream_forms/
--rw-r--r--   0 dev       (1000) dev       (1000)      532 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.356681 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/
--rw-r--r--   0 dev       (1000) dev       (1000)     2002 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/article_index_page.html
--rw-r--r--   0 dev       (1000) dev       (1000)     2031 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/article_page.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1018 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/article_page.search.html
--rw-r--r--   0 dev       (1000) dev       (1000)     9488 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/base.html
--rw-r--r--   0 dev       (1000) dev       (1000)      248 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/form_page_landing.html
--rw-r--r--   0 dev       (1000) dev       (1000)       50 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/home_page.html
--rw-r--r--   0 dev       (1000) dev       (1000)      491 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/page.mini.html
--rw-r--r--   0 dev       (1000) dev       (1000)     2613 2024-02-18 15:50:24.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/search.html
--rw-r--r--   0 dev       (1000) dev       (1000)      582 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/search_result.html
--rw-r--r--   0 dev       (1000) dev       (1000)      594 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/web_page.html
--rw-r--r--   0 dev       (1000) dev       (1000)      378 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/web_page_notitle.html
--rw-r--r--   0 dev       (1000) dev       (1000)      122 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/robots.txt
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.360681 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/
--rw-r--r--   0 dev       (1000) dev       (1000)       31 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/actionbar.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1943 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1311 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/breadcrumbs.html
--rw-r--r--   0 dev       (1000) dev       (1000)      430 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/footer.html
--rw-r--r--   0 dev       (1000) dev       (1000)     1377 2024-03-11 19:24:53.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/frontend_assets.html
--rw-r--r--   0 dev       (1000) dev       (1000)      510 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
--rw-r--r--   0 dev       (1000) dev       (1000)     2983 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/navbar.html
--rw-r--r--   0 dev       (1000) dev       (1000)      836 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html
--rw-r--r--   0 dev       (1000) dev       (1000)     2293 2024-02-18 22:17:50.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/navbar_search.html
--rw-r--r--   0 dev       (1000) dev       (1000)      330 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/social_media.html
--rw-r--r--   0 dev       (1000) dev       (1000)     2829 2024-03-11 19:17:03.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/social_media_icons.html
--rw-r--r--   0 dev       (1000) dev       (1000)      173 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/social_media_nav_block.html
--rw-r--r--   0 dev       (1000) dev       (1000)      158 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/tracking_g3.html
--rw-r--r--   0 dev       (1000) dev       (1000)      832 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/tracking_g4.html
--rw-r--r--   0 dev       (1000) dev       (1000)      694 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/tracking_matomo.html
--rw-r--r--   0 dev       (1000) dev       (1000)      230 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/tracking_matomo_noscript.html
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.360681 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/widgets/
--rw-r--r--   0 dev       (1000) dev       (1000)     1444 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.276682 wagtail-cjkcms-24.3.2/cjkcms/templates/wagtailadmin/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.360681 wagtail-cjkcms-24.3.2/cjkcms/templates/wagtailadmin/block_forms/
--rw-r--r--   0 dev       (1000) dev       (1000)      839 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
--rw-r--r--   0 dev       (1000) dev       (1000)      550 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/wagtailadmin/block_forms/struct.html
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.360681 wagtail-cjkcms-24.3.2/cjkcms/templates/wagtailadmin/shared/
--rw-r--r--   0 dev       (1000) dev       (1000)      885 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.364681 wagtail-cjkcms-24.3.2/cjkcms/templates/wagtailadmin/tables/
--rw-r--r--   0 dev       (1000) dev       (1000)      578 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templates/wagtailadmin/tables/thumbnail_cell.html
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.364681 wagtail-cjkcms-24.3.2/cjkcms/templatetags/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templatetags/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)      327 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templatetags/auth_extras.py
--rw-r--r--   0 dev       (1000) dev       (1000)     8495 2024-02-18 21:41:31.000000 wagtail-cjkcms-24.3.2/cjkcms/templatetags/cjkcms_tags.py
--rw-r--r--   0 dev       (1000) dev       (1000)     4962 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templatetags/friendly_loader.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1127 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templatetags/gravatar.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1223 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/templatetags/txtutils_tags.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.368681 wagtail-cjkcms-24.3.2/cjkcms/tests/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)      242 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/manage.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.276682 wagtail-cjkcms-24.3.2/cjkcms/tests/media/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.368681 wagtail-cjkcms-24.3.2/cjkcms/tests/media/images/
--rw-r--r--   0 dev       (1000) dev       (1000)     1938 2024-02-18 17:38:22.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/media/images/test.original.png
--rw-r--r--   0 dev       (1000) dev       (1000)     1938 2024-03-20 09:04:13.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/media/images/test_3tYv0uS.original.png
--rw-r--r--   0 dev       (1000) dev       (1000)     1938 2024-03-11 19:28:39.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/media/images/test_d8sVYy7.original.png
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.368681 wagtail-cjkcms-24.3.2/cjkcms/tests/media/original_images/
--rw-r--r--   0 dev       (1000) dev       (1000)     2306 2024-02-18 17:38:22.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/media/original_images/test.png
--rw-r--r--   0 dev       (1000) dev       (1000)     2306 2024-03-20 09:04:13.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/media/original_images/test_3tYv0uS.png
--rw-r--r--   0 dev       (1000) dev       (1000)     2306 2024-03-11 19:28:39.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/media/original_images/test_d8sVYy7.png
--rw-r--r--   0 dev       (1000) dev       (1000)     2556 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/settings.py
--rw-r--r--   0 dev       (1000) dev       (1000)     6906 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/test_advsettings.py
--rw-r--r--   0 dev       (1000) dev       (1000)     4226 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/test_articlepages.py
--rw-r--r--   0 dev       (1000) dev       (1000)     3506 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/test_bin.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2364 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/test_draftail_extensions.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2489 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/test_finders_oembed.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2629 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/test_gravatar.py
--rw-r--r--   0 dev       (1000) dev       (1000)     4919 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/test_search_blocks.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2665 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/test_settings.py
--rw-r--r--   0 dev       (1000) dev       (1000)     5313 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/test_templatetags.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2832 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/test_urls.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1520 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/test_webpage.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.368681 wagtail-cjkcms-24.3.2/cjkcms/tests/testapp/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/testapp/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)      169 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/testapp/apps.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.368681 wagtail-cjkcms-24.3.2/cjkcms/tests/testapp/migrations/
--rw-r--r--   0 dev       (1000) dev       (1000)     4942 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/testapp/migrations/0001_initial.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1999 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/testapp/migrations/0002_create_homepage.py
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/testapp/migrations/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)      488 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/testapp/models.py
--rw-r--r--   0 dev       (1000) dev       (1000)      850 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/tests/urls.py
--rw-r--r--   0 dev       (1000) dev       (1000)      506 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/urls.py
--rw-r--r--   0 dev       (1000) dev       (1000)     2006 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/utils.py
--rw-r--r--   0 dev       (1000) dev       (1000)     4488 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/views.py
--rw-r--r--   0 dev       (1000) dev       (1000)     6543 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/wagtail_hooks.py
--rw-r--r--   0 dev       (1000) dev       (1000)     1745 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/cjkcms/widgets.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.372681 wagtail-cjkcms-24.3.2/docs/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.276682 wagtail-cjkcms-24.3.2/docs/api_reference/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.372681 wagtail-cjkcms-24.3.2/docs/api_reference/api/
--rw-r--r--   0 dev       (1000) dev       (1000)       55 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/api_reference/api/mailchimp.md
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.372681 wagtail-cjkcms-24.3.2/docs/api_reference/blocks/
--rw-r--r--   0 dev       (1000) dev       (1000)      489 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/api_reference/blocks/content_blocks.md
--rw-r--r--   0 dev       (1000) dev       (1000)      381 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/api_reference/blocks/html_blocks.md
--rw-r--r--   0 dev       (1000) dev       (1000)      109 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/api_reference/blocks/layout_blocks.md
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.372681 wagtail-cjkcms-24.3.2/docs/api_reference/models/
--rw-r--r--   0 dev       (1000) dev       (1000)      138 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/api_reference/models/settings_models.md
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.372681 wagtail-cjkcms-24.3.2/docs/api_reference/templatetags/
--rw-r--r--   0 dev       (1000) dev       (1000)       52 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/api_reference/templatetags/cjkcms_tags.md
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.376681 wagtail-cjkcms-24.3.2/docs/configuration/
--rw-r--r--   0 dev       (1000) dev       (1000)      351 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/configuration/index.md
--rw-r--r--   0 dev       (1000) dev       (1000)     1589 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/configuration/webpack.md
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.376681 wagtail-cjkcms-24.3.2/docs/faq/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/faq/index.md
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.376681 wagtail-cjkcms-24.3.2/docs/getting-started/
--rw-r--r--   0 dev       (1000) dev       (1000)      993 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/getting-started/01.quick-start.md
--rw-r--r--   0 dev       (1000) dev       (1000)     1238 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/getting-started/02.folders-and-environment.md
--rw-r--r--   0 dev       (1000) dev       (1000)      997 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/getting-started/03.installation.md
--rw-r--r--   0 dev       (1000) dev       (1000)     4202 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/getting-started/04.configuration.md
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.376681 wagtail-cjkcms-24.3.2/docs/how-to/
--rw-r--r--   0 dev       (1000) dev       (1000)     1031 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/how-to/change-layout.md
--rw-r--r--   0 dev       (1000) dev       (1000)     1481 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/how-to/oembed_finder.md
--rw-r--r--   0 dev       (1000) dev       (1000)      575 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/index.md
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.380681 wagtail-cjkcms-24.3.2/docs/management_commands/
--rw-r--r--   0 dev       (1000) dev       (1000)      318 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/management_commands/clear-embeds.md
--rw-r--r--   0 dev       (1000) dev       (1000)      193 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/management_commands/index.md
--rw-r--r--   0 dev       (1000) dev       (1000)      420 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/management_commands/init-collections.md
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.380681 wagtail-cjkcms-24.3.2/docs/manual/
--rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/manual/index.md
--rw-r--r--   0 dev       (1000) dev       (1000)       56 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/requirements.txt
--rw-r--r--   0 dev       (1000) dev       (1000)      982 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/unit_testing.md
--rw-r--r--   0 dev       (1000) dev       (1000)     1221 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/docs/why-another-cms.md
--rw-r--r--   0 dev       (1000) dev       (1000)     1723 2024-02-18 20:37:52.000000 wagtail-cjkcms-24.3.2/pyproject.toml
--rw-r--r--   0 dev       (1000) dev       (1000)       87 2024-02-18 20:13:12.000000 wagtail-cjkcms-24.3.2/requirements.txt
--rw-r--r--   0 dev       (1000) dev       (1000)      254 2024-03-20 09:05:10.380681 wagtail-cjkcms-24.3.2/setup.cfg
--rw-r--r--   0 dev       (1000) dev       (1000)       38 2024-02-16 08:56:45.000000 wagtail-cjkcms-24.3.2/setup.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2024-03-20 09:05:10.380681 wagtail-cjkcms-24.3.2/wagtail_cjkcms.egg-info/
--rw-r--r--   0 dev       (1000) dev       (1000)     3106 2024-03-20 09:05:10.000000 wagtail-cjkcms-24.3.2/wagtail_cjkcms.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)    16798 2024-03-20 09:05:10.000000 wagtail-cjkcms-24.3.2/wagtail_cjkcms.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-03-20 09:05:10.000000 wagtail-cjkcms-24.3.2/wagtail_cjkcms.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       50 2024-03-20 09:05:10.000000 wagtail-cjkcms-24.3.2/wagtail_cjkcms.egg-info/entry_points.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       88 2024-03-20 09:05:10.000000 wagtail-cjkcms-24.3.2/wagtail_cjkcms.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        7 2024-03-20 09:05:10.000000 wagtail-cjkcms-24.3.2/wagtail_cjkcms.egg-info/top_level.txt
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.736903 wagtail_cjkcms-24.5.1/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     6631 2024-05-01 20:39:56.000000 wagtail_cjkcms-24.5.1/CHANGELOG.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1538 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/LICENSE
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      158 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/MANIFEST.in
+-rw-r--r--   0 grzegorz  (1000) grzegorz  (1000)     3106 2024-05-01 20:41:15.736903 wagtail_cjkcms-24.5.1/PKG-INFO
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1613 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/README.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.556903 wagtail_cjkcms-24.5.1/cjkcms/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      272 2024-05-01 20:35:18.000000 wagtail_cjkcms-24.5.1/cjkcms/__init__.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.556903 wagtail_cjkcms-24.5.1/cjkcms/api/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/api/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2832 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/api/mailchimp.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      173 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/apps.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.556903 wagtail_cjkcms-24.5.1/cjkcms/bin/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/bin/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     5763 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/bin/cjkcms.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.560903 wagtail_cjkcms-24.5.1/cjkcms/blocks/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     3402 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/blocks/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    11616 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/blocks/base_blocks.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.564903 wagtail_cjkcms-24.5.1/cjkcms/blocks/content/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/blocks/content/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1967 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/blocks/content/events.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     8890 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/blocks/content_blocks.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     9543 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/blocks/html_blocks.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     3406 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/blocks/layout_blocks.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      171 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/blocks/searchable_html_block.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.564903 wagtail_cjkcms-24.5.1/cjkcms/draftail/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      240 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/draftail/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     3250 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/draftail/draftail_extensions.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     3191 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/fields.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.564903 wagtail_cjkcms-24.5.1/cjkcms/finders/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/finders/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2760 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/finders/oembed.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      361 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/forms.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1833 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/image_formats.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.504903 wagtail_cjkcms-24.5.1/cjkcms/management/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.568903 wagtail_cjkcms-24.5.1/cjkcms/management/commands/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/management/commands/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      453 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/management/commands/clear-embeds.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2565 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/management/commands/import-csv.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      951 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/management/commands/init-collections.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     3560 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/management/commands/init-navbar.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     3820 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/management/commands/init-website.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.588903 wagtail_cjkcms-24.5.1/cjkcms/migrations/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)  2070677 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0001_initial.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      924 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      727 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1026 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1708 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2885 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      593 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1334 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      685 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0009_navbar_language.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     3479 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0010_filmstrip_filmpanel.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1393 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1466 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0012_remove_analyticssettings_ga_tracking_id_and_more.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      780 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0013_socialmediasettings_location.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      818 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0014_navbar_alignment.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1467 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0015_eventcalendar.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      918 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0016_layoutsettings_breadcrumb_icon_and_more.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      788 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0017_layoutsettings_default_seo_image.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      478 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0018_layoutsettings_search_format.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1220 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0019_layoutsettings_searchbox_input_class_and_more.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      922 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0020_socialmediasettings_github_and_more.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2106 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/0021_remove_layoutsettings_navbar_color_scheme_and_more.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/migrations/__init__.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.592903 wagtail_cjkcms-24.5.1/cjkcms/models/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      232 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/models/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      665 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/models/admin_sidebar.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2356 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/models/cms_models.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     6302 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/models/integration_models.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    24525 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/models/page_models.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    16837 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/models/snippet_models.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    22467 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/models/wagtailsettings_models.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.512903 wagtail_cjkcms-24.5.1/cjkcms/project_template/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.596903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      722 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/.editorconfig
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      364 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/.gitattributes
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      275 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/.gitignore
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      792 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/README.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.596903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/__init__.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.596903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/blocks/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      137 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/blocks/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2141 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/blocks/blocks.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.596903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/migrations/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4981 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/migrations/0001_initial.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2047 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/migrations/0002_create_homepage.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/migrations/__init__.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.596903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/models/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      383 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/models/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     3106 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/models/cms_models.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.508903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/templates/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.508903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/templates/home/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.600903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/templates/home/blocks/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2282 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/templates/home/blocks/event_presentation.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      678 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/manage.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.600903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/__init__.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.600903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/settings/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/settings/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     5477 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/settings/base.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      324 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/settings/dev.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      705 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/settings/local.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1595 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/settings/production.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.512903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/static/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.604903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/static/css/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/static/css/devsite.css
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.604903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/static/js/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/static/js/devsite.js
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      911 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/urls.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      432 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/wsgi.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      123 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/requirements.txt
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.604903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/search/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/search/__init__.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.512903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/search/templates/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.604903 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/search/templates/search/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1097 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/search/templates/search/search.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1019 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/search/views.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.608903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      245 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/.babelrc
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      159 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/.browserslistrc
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      722 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/.editorconfig
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      277 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/.eslintrc
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      364 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/.gitattributes
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      270 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/.gitignore
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       13 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/.nvmrc
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      182 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/.stylelintrc.json
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      792 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/README.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.608903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      131 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/.gitignore
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      733 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/README.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.516903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/src/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.612903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/src/application/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      577 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/src/application/app.js
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      226 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/src/application/app2.js
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.612903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/src/components/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       41 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/src/components/sidebar.js
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.612903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/src/styles/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      378 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/src/styles/index.scss
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.612903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/vendors/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/vendors/.gitkeep
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.612903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/vendors/images/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/vendors/images/.gitkeep
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)   104442 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/vendors/images/sample.jpg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    25891 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/vendors/images/webpack.png
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.616903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/webpack/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1473 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/webpack/webpack.common.js
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1716 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/webpack/webpack.config.dev.js
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      986 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/webpack/webpack.config.prod.js
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1485 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/webpack/webpack.config.watch.js
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.616903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/__init__.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.616903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/blocks/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      137 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/blocks/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2141 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/blocks/blocks.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.620903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/migrations/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4981 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/migrations/0001_initial.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2047 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/migrations/0002_create_homepage.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/migrations/__init__.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.620903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/models/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      391 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/models/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     3106 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/models/cms_models.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.516903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/templates/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.520903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/templates/home/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.620903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/templates/home/blocks/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2282 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/templates/home/blocks/event_presentation.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      678 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/manage.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1743 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/package.json
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.624903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/__init__.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.628903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/settings/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/settings/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     5648 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/settings/base.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      324 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/settings/dev.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      705 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/settings/local.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1593 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/settings/production.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.520903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/static/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.628903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/static/css/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/static/css/devsite.css
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.628903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/static/js/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/static/js/devsite.js
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      911 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/urls.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      432 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/wsgi.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      188 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/requirements.txt
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.628903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/search/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/search/__init__.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.520903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/search/templates/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.628903 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/search/templates/search/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1097 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/search/templates/search/search.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1019 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/search/views.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      125 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/search_urls.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    19370 2024-05-01 16:48:29.000000 wagtail_cjkcms-24.5.1/cjkcms/settings.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.524903 wagtail_cjkcms-24.5.1/cjkcms/static/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.524903 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.632903 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/bi/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    93729 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/bi/bootstrap-icons.css
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    49971 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/bi/bootstrap-icons.json
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    55169 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/bi/bootstrap-icons.scss
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.636903 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/bi/fonts/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)   164360 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)   121340 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.636903 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/css/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      846 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/css/cjkcms-admin.css
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2432 2024-05-01 17:10:51.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/css/cjkcms-custom-theme-disabled.css
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1104 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/css/cjkcms-editor.css
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4853 2024-05-01 20:33:53.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/css/cjkcms-front.css
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.524903 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.640903 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/avatars/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      535 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/avatars/default.png
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      384 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/avatars/default.svg
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.644903 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/icons/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      581 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/icons/calendar-day.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      268 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/icons/caret-right-fill.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      289 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/icons/caret-right.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      291 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/icons/chevron-right.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      705 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/icons/quote.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      252 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/icons/slash.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1374 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/icons/world.svg
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.644903 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/logos/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4166 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4218 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.644903 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/patterns/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    47935 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    31707 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    38190 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.648903 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/js/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      444 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/js/cjkcms-editor.js
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     5579 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/js/cjkcms-front.js
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.648903 wagtail_cjkcms-24.5.1/cjkcms/static/cookieconsent/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    18803 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cookieconsent/cookieconsent.css
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    18743 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/cookieconsent/cookieconsent.js
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.528903 wagtail_cjkcms-24.5.1/cjkcms/static/vendor/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.528903 wagtail_cjkcms-24.5.1/cjkcms/static/vendor/mdb/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.652903 wagtail_cjkcms-24.5.1/cjkcms/static/vendor/mdb/css/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)   392610 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/vendor/mdb/css/mdb.dark.min.css
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)   377096 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/vendor/mdb/css/mdb.min.css
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.656903 wagtail_cjkcms-24.5.1/cjkcms/static/vendor/mdb/js/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)   124476 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/static/vendor/mdb/js/mdb.umd.min.js
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.656903 wagtail_cjkcms-24.5.1/cjkcms/templates/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4176 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/404.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4802 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/500.html
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.656903 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.680903 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1443 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/accordion_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      974 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/article_block_card.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1132 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      188 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/base_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2634 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/base_link_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      740 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/button_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      746 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      856 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_blurb.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      786 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_foot.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      730 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_head.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      771 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      990 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1104 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      786 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_img.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2618 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_landing1.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2758 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_landing2.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      678 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      450 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      277 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      276 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2698 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/carousel_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      406 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/column_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      137 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/document_link_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      920 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/download_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      103 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/embed_video_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      308 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/event_calendar_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       95 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/external_link_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1484 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/film_strip_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      424 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/grid_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      200 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/h1_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      200 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/h2_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      200 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/h3_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      790 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/hero_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      275 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/image_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1400 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      627 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/image_link_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1020 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/modal_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      164 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/page_link_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      787 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      642 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      361 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      956 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      858 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagelist_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      610 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1224 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      200 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      793 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      244 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pricelist_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      513 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1155 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/public_event_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      353 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/quote_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      852 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      998 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      216 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       91 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/rich_text_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1095 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/table_block.html
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.680903 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/cookieconsent/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     3672 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/cookieconsent/languages.html
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.680903 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/formfields/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      267 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/formfields/date.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      416 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/formfields/datetime.html
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.680903 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/formfields/mailchimp/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     9267 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     6469 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      793 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      264 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/formfields/time.html
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.692903 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      449 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/align-center.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      462 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/align-left.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      447 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/align-right.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      891 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/card-grid.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      570 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/check-square-o.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      274 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/columns.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      356 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/desktop.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1083 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/font-decrease.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1117 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/font-increase.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      568 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/font.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      289 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/google.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      810 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      663 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/hashtag.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      837 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/header.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      832 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/list-alt.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      456 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/map.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      445 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/newspaper-o.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      718 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      632 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/recycle.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      171 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/stop.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      502 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/th-large.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      759 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/universal-access.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      545 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/usd.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      222 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/window-maximize.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      196 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/window-minimize.svg
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.692903 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/includes/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      286 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      689 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      579 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/includes/classifier_nav.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      268 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/includes/form_honeypot.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1061 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/includes/pagination.html
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.692903 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/includes/stream_forms/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      532 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.696903 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2002 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/article_index_page.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2031 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/article_page.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1018 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/article_page.search.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     9509 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/base.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      248 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/form_page_landing.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       50 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/home_page.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      506 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/page.mini.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2613 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/search.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      582 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/search_result.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      594 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/web_page.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      378 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/web_page_notitle.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      122 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/robots.txt
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.704903 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       31 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/actionbar.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1943 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1311 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/breadcrumbs.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      430 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/footer.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1656 2024-05-01 16:52:08.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      510 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2983 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/navbar.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      836 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2293 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/navbar_search.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      330 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/social_media.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2829 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/social_media_icons.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      173 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/social_media_nav_block.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      158 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/tracking_g3.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      832 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      694 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/tracking_matomo.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      230 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/tracking_matomo_noscript.html
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.704903 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/widgets/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1444 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.532903 wagtail_cjkcms-24.5.1/cjkcms/templates/wagtailadmin/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.704903 wagtail_cjkcms-24.5.1/cjkcms/templates/wagtailadmin/block_forms/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      839 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      550 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/wagtailadmin/block_forms/struct.html
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.704903 wagtail_cjkcms-24.5.1/cjkcms/templates/wagtailadmin/shared/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      885 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.708903 wagtail_cjkcms-24.5.1/cjkcms/templates/wagtailadmin/tables/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      578 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templates/wagtailadmin/tables/thumbnail_cell.html
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.708903 wagtail_cjkcms-24.5.1/cjkcms/templatetags/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templatetags/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      327 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templatetags/auth_extras.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     8721 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templatetags/cjkcms_tags.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4962 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templatetags/friendly_loader.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1127 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templatetags/gravatar.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1223 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/templatetags/txtutils_tags.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.716903 wagtail_cjkcms-24.5.1/cjkcms/tests/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      242 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/manage.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.536903 wagtail_cjkcms-24.5.1/cjkcms/tests/media/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.716903 wagtail_cjkcms-24.5.1/cjkcms/tests/media/images/
+-rw-r--r--   0 grzegorz  (1000) grzegorz  (1000)     1938 2024-05-01 17:23:39.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/media/images/test.original.png
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.716903 wagtail_cjkcms-24.5.1/cjkcms/tests/media/original_images/
+-rw-r--r--   0 grzegorz  (1000) grzegorz  (1000)     2306 2024-05-01 17:23:39.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/media/original_images/test.png
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2556 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/settings.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     6906 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/test_advsettings.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4226 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/test_articlepages.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     3506 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/test_bin.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2364 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/test_draftail_extensions.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2489 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/test_finders_oembed.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2629 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/test_gravatar.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4919 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/test_search_blocks.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2665 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/test_settings.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     5313 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/test_templatetags.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2832 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/test_urls.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1520 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/test_webpage.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.716903 wagtail_cjkcms-24.5.1/cjkcms/tests/testapp/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/testapp/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      169 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/testapp/apps.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.720903 wagtail_cjkcms-24.5.1/cjkcms/tests/testapp/migrations/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4942 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/testapp/migrations/0001_initial.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1999 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/testapp/migrations/0002_create_homepage.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/testapp/migrations/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      488 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/testapp/models.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      850 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/tests/urls.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      506 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/urls.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2006 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/utils.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4488 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/views.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     6543 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/wagtail_hooks.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1745 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/cjkcms/widgets.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.720903 wagtail_cjkcms-24.5.1/docs/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.540903 wagtail_cjkcms-24.5.1/docs/api_reference/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.720903 wagtail_cjkcms-24.5.1/docs/api_reference/api/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       55 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/api_reference/api/mailchimp.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.724903 wagtail_cjkcms-24.5.1/docs/api_reference/blocks/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      489 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/api_reference/blocks/content_blocks.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      381 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/api_reference/blocks/html_blocks.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      109 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/api_reference/blocks/layout_blocks.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.724903 wagtail_cjkcms-24.5.1/docs/api_reference/models/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      138 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/api_reference/models/settings_models.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.724903 wagtail_cjkcms-24.5.1/docs/api_reference/templatetags/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       52 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/api_reference/templatetags/cjkcms_tags.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.724903 wagtail_cjkcms-24.5.1/docs/configuration/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      351 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/configuration/index.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1589 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/configuration/webpack.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.724903 wagtail_cjkcms-24.5.1/docs/faq/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/faq/index.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.728903 wagtail_cjkcms-24.5.1/docs/getting-started/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      993 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/getting-started/01.quick-start.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1238 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/getting-started/02.folders-and-environment.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      997 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/getting-started/03.installation.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4202 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/getting-started/04.configuration.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.728903 wagtail_cjkcms-24.5.1/docs/how-to/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1031 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/how-to/change-layout.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1481 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/how-to/oembed_finder.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      575 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/index.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.732903 wagtail_cjkcms-24.5.1/docs/management_commands/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      318 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/management_commands/clear-embeds.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      193 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/management_commands/index.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      420 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/management_commands/init-collections.md
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.732903 wagtail_cjkcms-24.5.1/docs/manual/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/manual/index.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       56 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/requirements.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      982 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/unit_testing.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1221 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/docs/why-another-cms.md
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1723 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/pyproject.toml
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       87 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/requirements.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      264 2024-05-01 20:41:15.736903 wagtail_cjkcms-24.5.1/setup.cfg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       38 2024-05-01 15:47:50.000000 wagtail_cjkcms-24.5.1/setup.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2024-05-01 20:41:15.736903 wagtail_cjkcms-24.5.1/wagtail_cjkcms.egg-info/
+-rw-r--r--   0 grzegorz  (1000) grzegorz  (1000)     3106 2024-05-01 20:41:15.000000 wagtail_cjkcms-24.5.1/wagtail_cjkcms.egg-info/PKG-INFO
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    16855 2024-05-01 20:41:15.000000 wagtail_cjkcms-24.5.1/wagtail_cjkcms.egg-info/SOURCES.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        1 2024-05-01 20:41:15.000000 wagtail_cjkcms-24.5.1/wagtail_cjkcms.egg-info/dependency_links.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       50 2024-05-01 20:41:15.000000 wagtail_cjkcms-24.5.1/wagtail_cjkcms.egg-info/entry_points.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       88 2024-05-01 20:41:15.000000 wagtail_cjkcms-24.5.1/wagtail_cjkcms.egg-info/requires.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        7 2024-05-01 20:41:15.000000 wagtail_cjkcms-24.5.1/wagtail_cjkcms.egg-info/top_level.txt
```

### Comparing `wagtail-cjkcms-24.3.2/CHANGELOG.md` & `wagtail_cjkcms-24.5.1/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,17 +10,38 @@
 
 ## [Unreleased]
 ### Added
 ### Changed
 ### Fixed
 ### Removed
 
+## [24.5.1] - 2024-05-01
+### Added
+ - Support for custom bs/mdb variables: when layout->theme set to "custom", loads /static/cjkcms/css/cjkcms-custom-theme.css. Define this file in your project using e.g. template copied from /static/cjkcms/css/cjkcms-custom-theme-disabled.css and redefine any css vars
+ - Support for stretched-link in any Button Link, including in any card. To achieve a stretched link, add "stretched-link" to custom css classes in button's advanced settings. To achieve an invisible button link (e.g. image link), add "stretched-link zero-sized" to custom css of the button.
+
+
+## [24.3.3] - 2024-03-21
+### Added
+ - Correct processing of theme_css and theme_js for both full URLs (https:...) and local static paths (local/path/to.css)
+ - Support for client-side theme switching in both bootstrap and mdbootstrap
+### Fixed
+ - Problem with stretched-link not working in mdbootstrap when btn class used (required updating mdb-uikit to 7.x)
+### Changed
+ - MDB light and dark now packaged with the CMS, not loaded from CDN
+ - !!! Breaking change: navbar_color_scheme setting renamed to color_scheme and used as data-mdb/bs-theme setting for theme switching
+ - !!! Breaking configuration changes in Layout settings: navbar_collapse_mode, navbar_format, navbar_langselector and frontend_theme:
+   changed choices in the model from None to [], this may result in re-setting these settings in Backend->Settings->Layout to defaults.
+   Check each website after updating the CMS for layout of the HP, navbar collapse screen width, and theme layout.
+
 ## [24.3.2] - 2024-03-20
 ### Fixed
  - Renamed "libs" to "cjkcms_libs" in frontend scripts, to avoid name clash with htmx
+ Note: turns out, this was a misdiagnosed issue, there was no clash. But, it is better to have a more specific variable name,
+ rather than a generic "libs", so we'll keep this change.
 
 
 ## [24.3.1] - 2024-03-11
 ### Added
  - Missing social media fields in settings/social-media, and icons, including new X to replace Twitter
  - Updated fontawesome CDN call to v.6.5.1 to include new X icon.
```

### Comparing `wagtail-cjkcms-24.3.2/LICENSE` & `wagtail_cjkcms-24.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/PKG-INFO` & `wagtail_cjkcms-24.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-cjkcms
-Version: 24.3.2
+Version: 24.5.1
 Summary: Wagtail Content Management System, installable as a Django app into any Wagtail 4.1.x/5.x/6.x site.
 Author-email: Grzegorz Krol <gk@cjk.pl>
 License: BSD-3-Clause
 Project-URL: Homepage, https://cjkcms.com
 Project-URL: Repository, https://github.com/cjkpl/wagtail-cjkcms
 Keywords: wagtail,django,cms
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-cjkcms-24.3.2/README.md` & `wagtail_cjkcms-24.5.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/api/mailchimp.py` & `wagtail_cjkcms-24.5.1/cjkcms/api/mailchimp.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/bin/cjkcms.py` & `wagtail_cjkcms-24.5.1/cjkcms/bin/cjkcms.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/blocks/__init__.py` & `wagtail_cjkcms-24.5.1/cjkcms/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/blocks/base_blocks.py` & `wagtail_cjkcms-24.5.1/cjkcms/blocks/base_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/blocks/content/events.py` & `wagtail_cjkcms-24.5.1/cjkcms/blocks/content/events.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/blocks/content_blocks.py` & `wagtail_cjkcms-24.5.1/cjkcms/blocks/content_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/blocks/html_blocks.py` & `wagtail_cjkcms-24.5.1/cjkcms/blocks/html_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/blocks/layout_blocks.py` & `wagtail_cjkcms-24.5.1/cjkcms/blocks/layout_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/draftail/draftail_extensions.py` & `wagtail_cjkcms-24.5.1/cjkcms/draftail/draftail_extensions.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/fields.py` & `wagtail_cjkcms-24.5.1/cjkcms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/finders/oembed.py` & `wagtail_cjkcms-24.5.1/cjkcms/finders/oembed.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/image_formats.py` & `wagtail_cjkcms-24.5.1/cjkcms/image_formats.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/management/commands/import-csv.py` & `wagtail_cjkcms-24.5.1/cjkcms/management/commands/import-csv.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/management/commands/init-collections.py` & `wagtail_cjkcms-24.5.1/cjkcms/management/commands/init-collections.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/management/commands/init-navbar.py` & `wagtail_cjkcms-24.5.1/cjkcms/management/commands/init-navbar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/management/commands/init-website.py` & `wagtail_cjkcms-24.5.1/cjkcms/management/commands/init-website.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0001_initial.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0009_navbar_language.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0009_navbar_language.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0010_filmstrip_filmpanel.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0010_filmstrip_filmpanel.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0012_remove_analyticssettings_ga_tracking_id_and_more.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0012_remove_analyticssettings_ga_tracking_id_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0013_socialmediasettings_location.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0013_socialmediasettings_location.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0014_navbar_alignment.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0014_navbar_alignment.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0015_eventcalendar.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0015_eventcalendar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0016_layoutsettings_breadcrumb_icon_and_more.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0016_layoutsettings_breadcrumb_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0017_layoutsettings_default_seo_image.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0017_layoutsettings_default_seo_image.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0019_layoutsettings_searchbox_input_class_and_more.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0019_layoutsettings_searchbox_input_class_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/migrations/0020_socialmediasettings_github_and_more.py` & `wagtail_cjkcms-24.5.1/cjkcms/migrations/0020_socialmediasettings_github_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/models/admin_sidebar.py` & `wagtail_cjkcms-24.5.1/cjkcms/models/admin_sidebar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/models/cms_models.py` & `wagtail_cjkcms-24.5.1/cjkcms/models/cms_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/models/integration_models.py` & `wagtail_cjkcms-24.5.1/cjkcms/models/integration_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/models/page_models.py` & `wagtail_cjkcms-24.5.1/cjkcms/models/page_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/models/snippet_models.py` & `wagtail_cjkcms-24.5.1/cjkcms/models/snippet_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/models/wagtailsettings_models.py` & `wagtail_cjkcms-24.5.1/cjkcms/models/wagtailsettings_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,25 +157,14 @@
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
         related_name="default_seo_image",
         verbose_name=_("Default SEO Image"),
     )
 
-    navbar_color_scheme = models.CharField(
-        blank=True,
-        max_length=50,
-        choices=None,
-        default="",
-        verbose_name=_("Navbar color scheme"),
-        help_text=_(
-            "Optimizes text and other navbar elements for use with light or dark backgrounds."
-        ),  # noqa
-    )
-
     navbar_class = models.CharField(
         blank=True,
         max_length=255,
         default="",
         verbose_name=_("Navbar CSS class"),
         help_text=_(
             'Custom classes applied to navbar e.g. "bg-light", "bg-dark", "bg-primary".'
@@ -195,25 +184,25 @@
         default=False,
         verbose_name=_("Full width navbar contents"),
         help_text=_("Content within the navbar will fill edge to edge."),
     )
     navbar_collapse_mode = models.CharField(
         blank=True,
         max_length=50,
-        choices=None,
+        choices=[],
         default="",
         verbose_name=_("Collapse navbar menu"),
         help_text=_(
             "Control on what screen sizes to show and collapse the navbar menu links."
         ),
     )
     navbar_format = models.CharField(
         blank=True,
         max_length=50,
-        choices=None,
+        choices=[],
         default="",
         verbose_name=_("Navbar format"),
     )
 
     navbar_search = models.BooleanField(
         default=True,
         verbose_name=_("Search box"),
@@ -256,37 +245,53 @@
         ),
     )
 
     navbar_langselector = models.CharField(
         blank=True,
         null=True,
         max_length=255,
-        choices=None,
+        choices=[],
         default=None,
         verbose_name=_("Language selector"),
         help_text=_("Choose lang choice selector"),
     )
 
     breadcrumbs = models.BooleanField(
         default=False,
         verbose_name=_("Breadcrumbs"),
         help_text=_("Show breadcrumbs in page header"),
     )
+
     breadcrumb_icon = models.CharField(
         blank=True,
         max_length=32,
         default="slash",
         verbose_name=_("Breadcrumb icon"),
         help_text=_("Bootstrap icon name. See docs for built-in options."),
     )
 
+    color_scheme = models.CharField(
+        blank=True,
+        max_length=50,
+        choices=[],
+        default="",
+        verbose_name=_("Color scheme"),
+        help_text=_("Default light/dark/custom theme. (MD/Bootstrap only)"),  # noqa
+    )
+
+    light_dark_switch = models.BooleanField(
+        default=False,
+        verbose_name=_("Light/Dark switch"),
+        help_text=_("Show switch to toggle light/dark theme (MD/Bootstrap only)"),
+    )
+
     frontend_theme = models.CharField(
         blank=True,
         max_length=50,
-        choices=None,
+        choices=[],
         default="",
         verbose_name=_("Theme variant"),
         help_text=cms_settings.CJKCMS_FRONTEND_THEME_HELP,
     )
 
     awesome_cdn = models.BooleanField(
         default=False,
@@ -357,15 +362,14 @@
         InlinePanel(
             "site_navbar",
             help_text=_("Choose one or more navbars"),
             heading=_("Site Navbars"),
         ),
         MultiFieldPanel(
             [
-                FieldPanel("navbar_color_scheme"),
                 FieldPanel("navbar_class"),
                 FieldPanel("navbar_fixed"),
                 FieldPanel("navbar_wrapper_fluid"),
                 FieldPanel("navbar_content_fluid"),
                 FieldPanel("navbar_collapse_mode"),
                 FieldPanel("navbar_format"),
                 FieldPanel("navbar_langselector"),
@@ -392,14 +396,15 @@
         InlinePanel(
             "site_footer",
             help_text=_("Choose one or more footers"),
             heading=_("Site Footers"),
         ),
         MultiFieldPanel(
             [
+                FieldPanel("color_scheme"),
                 FieldPanel("frontend_theme"),
                 FieldPanel("base_template"),
                 FieldPanel("awesome_cdn"),
                 FieldPanel("bootstrap_icons"),
                 FieldPanel("custom_font"),
                 FieldPanel("font_url"),
                 FieldPanel("font_family"),
@@ -425,16 +430,16 @@
         self._meta.get_field(
             "frontend_theme"
         ).choices = cms_settings.CJKCMS_FRONTEND_THEME_CHOICES  # type: ignore
         self._meta.get_field(
             "navbar_collapse_mode"
         ).choices = cms_settings.CJKCMS_FRONTEND_NAVBAR_COLLAPSE_MODE_CHOICES  # type: ignore
         self._meta.get_field(
-            "navbar_color_scheme"
-        ).choices = cms_settings.CJKCMS_FRONTEND_NAVBAR_COLOR_SCHEME_CHOICES  # type: ignore
+            "color_scheme"
+        ).choices = cms_settings.CJKCMS_FRONTEND_COLOR_SCHEME_CHOICES  # type: ignore
         self._meta.get_field(
             "navbar_format"
         ).choices = cms_settings.CJKCMS_FRONTEND_NAVBAR_FORMAT_CHOICES  # type: ignore
         self._meta.get_field(
             "search_format"
         ).choices = cms_settings.CJKCMS_FRONTEND_SEARCH_FORMAT_CHOICES  # type: ignore
         self._meta.get_field(
@@ -443,17 +448,15 @@
         # Set default dynamically.
         if not self.id:  # type: ignore # if new record / id not yet assigned
             self.frontend_theme = cms_settings.CJKCMS_FRONTEND_THEME_DEFAULT
             self.navbar_class = cms_settings.CJKCMS_FRONTEND_NAVBAR_CLASS_DEFAULT
             self.navbar_collapse_mode = (
                 cms_settings.CJKCMS_FRONTEND_NAVBAR_COLLAPSE_MODE_DEFAULT
             )
-            self.navbar_color_scheme = (
-                cms_settings.CJKCMS_FRONTEND_NAVBAR_COLOR_SCHEME_DEFAULT
-            )
+            self.color_scheme = cms_settings.CJKCMS_FRONTEND_COLOR_SCHEME_DEFAULT
             self.navbar_format = cms_settings.CJKCMS_FRONTEND_NAVBAR_FORMAT_DEFAULT
             self.search_format = cms_settings.CJKCMS_FRONTEND_SEARCH_FORMAT_DEFAULT
             self.base_template = cms_settings.CJKCMS_BASE_TEMPLATE_DEFAULT
 
 
 class NavbarOrderable(Orderable, models.Model):
     navbar_chooser = ParentalKey(
```

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/.editorconfig` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/.editorconfig`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/README.md` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/blocks/blocks.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/blocks/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/migrations/0001_initial.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/migrations/0002_create_homepage.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/models/cms_models.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/models/cms_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/home/templates/home/blocks/event_presentation.html` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/home/templates/home/blocks/event_presentation.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/manage.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/settings/base.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/settings/local.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/settings/local.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/settings/production.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/settings/production.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/project_name/urls.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/search/templates/search/search.html` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/search/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/basic/search/views.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/basic/search/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/.editorconfig` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/.editorconfig`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/README.md` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/README.md` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/src/application/app.js` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/src/application/app.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/vendors/images/sample.jpg` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/vendors/images/sample.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/vendors/images/webpack.png` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/vendors/images/webpack.png`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/webpack/webpack.common.js` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/webpack/webpack.common.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/webpack/webpack.config.dev.js` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/webpack/webpack.config.dev.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/webpack/webpack.config.prod.js` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/webpack/webpack.config.prod.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/frontend/webpack/webpack.config.watch.js` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/frontend/webpack/webpack.config.watch.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/blocks/blocks.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/blocks/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/migrations/0001_initial.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/migrations/0002_create_homepage.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/models/cms_models.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/models/cms_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/home/templates/home/blocks/event_presentation.html` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/home/templates/home/blocks/event_presentation.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/manage.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/package.json` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/package.json`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/settings/base.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/settings/local.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/settings/local.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/settings/production.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/settings/production.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/project_name/urls.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/search/templates/search/search.html` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/search/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/project_template/webpack/search/views.py` & `wagtail_cjkcms-24.5.1/cjkcms/project_template/webpack/search/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/settings.py` & `wagtail_cjkcms-24.5.1/cjkcms/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -85,18 +85,19 @@
     CJKCMS_LANGUAGE_SELECTOR_DEFAULT: Optional[str] = None
     CJKCMS_LANGUAGE_SELECTOR_CHOICES = [
         (None, "None"),
         ("cjkcms/snippets/navbar_lang_selector.html", "Menu Dropdown Selector"),
         ("cjkcms/snippets/bottom_corner_lang_selector.html", "Bottom Corner Selector"),
     ]
 
-    CJKCMS_FRONTEND_NAVBAR_COLOR_SCHEME_DEFAULT = "navbar-light"
-    CJKCMS_FRONTEND_NAVBAR_COLOR_SCHEME_CHOICES = [
-        ("navbar-light", "Light - for use with a light-colored navbar"),
-        ("navbar-dark", "Dark - for use with a dark-colored navbar"),
+    CJKCMS_FRONTEND_COLOR_SCHEME_DEFAULT = "light"
+    CJKCMS_FRONTEND_COLOR_SCHEME_CHOICES = [
+        ("light", "Light theme"),
+        ("dark", "Dark theme"),
+        ("custom", "Custom from cjkcms-custom-theme.css"),
     ]
 
     CJKCMS_FRONTEND_NAVBAR_CLASS_DEFAULT = "bg-light"
 
     CJKCMS_FRONTEND_NAVBAR_COLLAPSE_MODE_DEFAULT = "navbar-expand-lg"
     CJKCMS_FRONTEND_NAVBAR_COLLAPSE_MODE_CHOICES = [
         ("", "Never show menu - Always collapse menu behind a button"),
@@ -110,16 +111,16 @@
     ]
 
     CJKCMS_FRONTEND_THEME_HELP = "Change the source of your Bootstrap theme."
     CJKCMS_FRONTEND_THEME_DEFAULT = "bootstrap5"
     CJKCMS_FRONTEND_THEME_CHOICES = (
         ("bootstrap5", "Default - Bootstrap 5 (CDN)"),
         ("python-webpack", "Python Webpack Boilerplate by Michael Yin"),
-        ("mdb.light", "MDBootstrap 5 (CDN)"),
-        ("mdb.dark", "MDBootstrap 5 dark (CDN)"),
+        ("mdb.light", "MDBootstrap 5 (local)"),
+        ("mdb.dark", "MDBootstrap 5 dark (local)"),
         ("bootswatch.cerulean", "Bootswatch Cerulean (CDN)"),
         ("bootswatch.cosmo", "Bootswatch Cosmo (CDN)"),
         ("bootswatch.cyborg", "Bootswatch Cyborg (CDN)"),
         ("bootswatch.darkly", "Bootswatch Darkly (CDN)"),
         ("bootswatch.flatly", "Bootswatch Flatly (CDN)"),
         ("bootswatch.journal", "Bootswatch Journal (CDN)"),
         ("bootswatch.litera", "Bootswatch Litera (CDN)"),
@@ -145,124 +146,132 @@
 
     # create a list of tuples, each tuple is a (name, [css url, js url]),
     # for each theme defined in FRONTEND_THEME_CHOICES
 
     CJKCMS_THEME_FILES = {
         "python-webpack": ["@include", "@include"],  # this entry will be ignored
         "bootstrap5": [
-            "https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/css/bootstrap.min.css",
-            "https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/js/bootstrap.bundle.min.js",
+            "https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.3/css/bootstrap.min.css",
+            "https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.3/js/bootstrap.bundle.min.js",
         ],
-        "mdb.light": [
-            "https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.4.2/mdb.min.css",
-            "https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.4.2/mdb.min.js",
-        ],
-        "mdb.dark": [
-            "https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.4.2/mdb.dark.min.css",
-            "https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.4.2/mdb.min.js",
+        # "mdb.light": [
+        #     "https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/7.2.0/mdb.min.css",
+        #     "https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/7.2.0/mdb.umd.min.js",
+        # ],
+        # "mdb.dark": [
+        #     "https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/7.2.0/mdb.dark.min.css",
+        #     "https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/7.2.0/mdb.umd.min.js",
+        # ],
+        "mdb.light": [  # 7.2.0
+            "vendor/mdb/css/mdb.min.css",
+            "vendor/mdb/js/mdb.umd.min.js",
+        ],
+        "mdb.dark": [  # 7.2.0
+            "vendor/mdb/css/mdb.dark.min.css",
+            "vendor/mdb/js/mdb.umd.min.js",
         ],
         "bootswatch.cerulean": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/cerulean/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/cerulean/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.cosmo": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/cosmo/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/cosmo/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.cyborg": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/cyborg/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/cyborg/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.darkly": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/darkly/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/darkly/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.flatly": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/flatly/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/flatly/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.journal": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/journal/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/journal/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.litera": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/litera/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/litera/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.lumen": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/lumen/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/lumen/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.lux": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/lux/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/lux/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.materia": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/materia/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/materia/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.minty": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/minty/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/minty/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.morph": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/morph/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/morph/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.pulse": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/pulse/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/pulse/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.quartz": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/quartz/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/quartz/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.sandstone": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/sandstone/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/sandstone/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.simplex": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/simplex/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/simplex/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.sketchy": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/sketchy/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/sketchy/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.slate": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/slate/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/slate/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.solar": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/solar/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/solar/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.spacelab": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/spacelab/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/spacelab/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.superhero": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/superhero/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/superhero/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.united": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/united/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/united/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.vapor": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/vapor/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/vapor/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.yeti": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/yeti/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/yeti/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
         "bootswatch.zephyr": [
-            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.2/dist/zephyr/bootstrap.min.css",
-            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js",
+            "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/zephyr/bootstrap.min.css",
+            "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js",
         ],
     }
 
     CJKCMS_FRONTEND_TEMPLATES_BLOCKS = {
         "cardblock": [
             ("cjkcms/blocks/card_block.html", "Card"),
             ("cjkcms/blocks/card_horizontal.html", "Horizontal Card"),
```

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/bi/bootstrap-icons.css` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/bi/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/bi/bootstrap-icons.json` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/bi/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/bi/bootstrap-icons.scss` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/bi/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/css/cjkcms-admin.css` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/css/cjkcms-admin.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/css/cjkcms-editor.css` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/css/cjkcms-editor.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/css/cjkcms-front.css` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/css/cjkcms-front.css`

 * *Files 6% similar despite different names*

```diff
@@ -296,10 +296,15 @@
 
 #id_s {
   margin-bottom: 0;
   margin-top: 0;
   border: gray 1px solid;
 }
 
-/* .form-control .is-valid {
-  padding-right: 12px;
-} */
+/* this can be used to create a stretched-link with a hidden button */
+.zero-sized {
+  opacity: 0;
+  overflow: hidden;
+  height: 0;
+  width: 0;
+  display: block;
+}
```

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/avatars/default.png` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/avatars/default.png`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/icons/calendar-day.svg` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/icons/calendar-day.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/icons/quote.svg` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/icons/world.svg` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/icons/world.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/patterns/pattern1.jpg` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/patterns/pattern2.jpg` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/images/patterns/pattern3.jpg` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cjkcms/js/cjkcms-front.js` & `wagtail_cjkcms-24.5.1/cjkcms/static/cjkcms/js/cjkcms-front.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cookieconsent/cookieconsent.css` & `wagtail_cjkcms-24.5.1/cjkcms/static/cookieconsent/cookieconsent.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/static/cookieconsent/cookieconsent.js` & `wagtail_cjkcms-24.5.1/cjkcms/static/cookieconsent/cookieconsent.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/404.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/404.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/500.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/500.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/accordion_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/accordion_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/article_block_card.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/article_block_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/article_masonry_card.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/base_link_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/base_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/button_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/button_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_blurb.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_blurb.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_foot.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_head.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_head.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_head_foot.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_horizontal.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_horizontal2.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_img.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_img.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_landing1.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_landing1.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/card_landing2.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/card_landing2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/carousel_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/carousel_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/download_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/download_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/film_strip_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/film_strip_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/hero_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/hero_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/image_gallery_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/image_link_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/image_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/modal_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/modal_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagelist_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagelist_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pagepreview_card.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/public_event_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/public_event_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/blocks/table_block.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/blocks/table_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/cookieconsent/languages.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/cookieconsent/languages.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/card-grid.svg` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/card-grid.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/check-square-o.svg` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/check-square-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/font-decrease.svg` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/font-decrease.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/font-increase.svg` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/font-increase.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/font.svg` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/font.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/hashtag.svg` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/hashtag.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/header.svg` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/header.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/list-alt.svg` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/list-alt.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/puzzle-piece.svg` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/recycle.svg` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/recycle.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/universal-access.svg` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/universal-access.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/icons/usd.svg` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/icons/usd.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/includes/classifier_nav.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/includes/classifier_nav.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/includes/pagination.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/article_index_page.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/article_index_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/article_page.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/article_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/article_page.search.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/article_page.search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/base.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/base.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% spaceless %}
 {% load i18n static friendly_loader cjkcms_tags wagtailcore_tags wagtailimages_tags wagtailsettings_tags wagtailuserbar %}
 {% get_settings %}{% get_current_language as LANGUAGE_CODE %}
 {% if settings.cjkcms.LayoutSettings.frontend_theme %}{% friendly_load webpack_loader static %}{% endif %}
 {% wagtail_site as site %}
 <!doctype html>
 {% endspaceless %}
-<html prefix="og: http://ogp.me/ns#" lang="{{ LANGUAGE_CODE }}" >
+<html prefix="og: http://ogp.me/ns#" lang="{{ LANGUAGE_CODE }}" data-mdb-theme="dark">
 {% block base_head %}
   <head>
         <script>{# Pass in CMS variables to JavaScript #}
             cjkcms_site_url = "{{site.root_url}}";
             cjkcms_external_new_tab = {{settings.cjkcms.GeneralSettings.external_new_tab|yesno:"true,false"}};
         </script>
         <meta charset="utf-8" />
```

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/search.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/search_result.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/search_result.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/pages/web_page.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/pages/web_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/breadcrumbs.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/frontend_assets.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,22 @@
             {% stylesheet_pack 'app' %}
         {% endif_has_tag %}
     {% else %}
         <link href="{% theme_css %}" 
             rel="stylesheet" 
             crossorigin="anonymous">
     {% endif %}
+
+    {% if settings.cjkcms.LayoutSettings.color_scheme == 'custom' %}
+        <!-- Load local css variables sheet to override default colors etc -->
+        <link
+            href="{% static 'cjkcms/css/cjkcms-custom-theme.css' %}"
+            rel="stylesheet">
+    {% endif %}
+
     {% if settings.cjkcms.LayoutSettings.bootstrap_icons %}
         <!-- Bootstrap icons (local) -->
         <link
             href="{% static 'cjkcms/bi/bootstrap-icons.css' %}"
             rel="stylesheet">
     {% endif %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% load friendly_loader wagtailcore_tags wagtailsettings_tags cjkcms_tags
 static %} {% friendly_load webpack_loader %} {% if
 settings.cjkcms.LayoutSettings.frontend_theme == 'python-webpack' %} {# use
 python-webpack from Michael Yin #} {% if_has_tag stylesheet_pack %} {%
 stylesheet_pack 'app' %} {% endif_has_tag %} {% else %}
+{% endif %} {% if settings.cjkcms.LayoutSettings.color_scheme == 'custom' %}
 {% endif %} {% if settings.cjkcms.LayoutSettings.bootstrap_icons %}
 {% endif %} {% if settings.cjkcms.LayoutSettings.awesome_cdn %}
 {% endif %} {% if settings.cjkcms.LayoutSettings.custom_font %}
 {% endif %}
```

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/navbar.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/navbar.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/navbar_search.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/navbar_search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/social_media_icons.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/social_media_icons.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/tracking_g4.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/snippets/tracking_matomo.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/snippets/tracking_matomo.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/wagtailadmin/block_forms/struct.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/wagtailadmin/block_forms/struct.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templates/wagtailadmin/tables/thumbnail_cell.html` & `wagtail_cjkcms-24.5.1/cjkcms/templates/wagtailadmin/tables/thumbnail_cell.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templatetags/cjkcms_tags.py` & `wagtail_cjkcms-24.5.1/cjkcms/templatetags/cjkcms_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,26 +80,33 @@
 
 
 @register.simple_tag
 def brand_logo_square():
     return cms_settings.CJKCMS_BRAND_LOGO_SQUARE
 
 
+def static_or_url(value: str) -> str:
+    # If value is a URL, return value, else return static(value)
+    if value.startswith("https"):
+        return value
+    return f"{settings.STATIC_URL}{value}"
+
+
 @register.simple_tag(takes_context=True)
 def theme_css(context):
     layout = LayoutSettings.for_request(context["request"])
     theme = layout.frontend_theme or "bootstrap5"
-    return cms_settings.CJKCMS_THEME_FILES[theme][0]
+    return static_or_url(cms_settings.CJKCMS_THEME_FILES[theme][0])
 
 
 @register.simple_tag(takes_context=True)
 def theme_js(context):
     layout = LayoutSettings.for_request(context["request"])
     theme = layout.frontend_theme or "bootstrap5"
-    return cms_settings.CJKCMS_THEME_FILES[theme][1]
+    return static_or_url(cms_settings.CJKCMS_THEME_FILES[theme][1])
 
 
 @register.simple_tag
 def is_menu_item_dropdown(value):
     return len(value.get("sub_links", [])) > 0 or (
         value.get("show_child_links", False)
         and len(value.get("page", []).get_children().live()) > 0
@@ -128,15 +135,15 @@
 def get_navbar_css(context):
     layout = LayoutSettings.for_request(context["request"])
     fixed = "fixed-top" if layout.navbar_fixed else ""
     return " ".join(
         [
             fixed,
             layout.navbar_collapse_mode,
-            layout.navbar_color_scheme,
+            layout.color_scheme,
             layout.navbar_format,
             layout.navbar_class,
         ]
     )
 
 
 @register.simple_tag(takes_context=True)
```

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templatetags/friendly_loader.py` & `wagtail_cjkcms-24.5.1/cjkcms/templatetags/friendly_loader.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templatetags/gravatar.py` & `wagtail_cjkcms-24.5.1/cjkcms/templatetags/gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/templatetags/txtutils_tags.py` & `wagtail_cjkcms-24.5.1/cjkcms/templatetags/txtutils_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/media/images/test.original.png` & `wagtail_cjkcms-24.5.1/cjkcms/tests/media/images/test.original.png`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/media/original_images/test.png` & `wagtail_cjkcms-24.5.1/cjkcms/tests/media/original_images/test.png`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/settings.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/test_advsettings.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/test_advsettings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/test_articlepages.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/test_articlepages.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/test_bin.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/test_bin.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/test_draftail_extensions.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/test_draftail_extensions.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/test_finders_oembed.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/test_finders_oembed.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/test_gravatar.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/test_gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/test_search_blocks.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/test_search_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/test_settings.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/test_templatetags.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/test_urls.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/test_webpage.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/test_webpage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/testapp/migrations/0001_initial.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/testapp/migrations/0002_create_homepage.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/testapp/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/tests/urls.py` & `wagtail_cjkcms-24.5.1/cjkcms/tests/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/utils.py` & `wagtail_cjkcms-24.5.1/cjkcms/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/views.py` & `wagtail_cjkcms-24.5.1/cjkcms/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/wagtail_hooks.py` & `wagtail_cjkcms-24.5.1/cjkcms/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/cjkcms/widgets.py` & `wagtail_cjkcms-24.5.1/cjkcms/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/docs/configuration/webpack.md` & `wagtail_cjkcms-24.5.1/docs/configuration/webpack.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/docs/getting-started/01.quick-start.md` & `wagtail_cjkcms-24.5.1/docs/getting-started/01.quick-start.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/docs/getting-started/02.folders-and-environment.md` & `wagtail_cjkcms-24.5.1/docs/getting-started/02.folders-and-environment.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/docs/getting-started/03.installation.md` & `wagtail_cjkcms-24.5.1/docs/getting-started/03.installation.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/docs/getting-started/04.configuration.md` & `wagtail_cjkcms-24.5.1/docs/getting-started/04.configuration.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/docs/how-to/change-layout.md` & `wagtail_cjkcms-24.5.1/docs/how-to/change-layout.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/docs/how-to/oembed_finder.md` & `wagtail_cjkcms-24.5.1/docs/how-to/oembed_finder.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/docs/index.md` & `wagtail_cjkcms-24.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/docs/unit_testing.md` & `wagtail_cjkcms-24.5.1/docs/unit_testing.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/docs/why-another-cms.md` & `wagtail_cjkcms-24.5.1/docs/why-another-cms.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/pyproject.toml` & `wagtail_cjkcms-24.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-24.3.2/wagtail_cjkcms.egg-info/PKG-INFO` & `wagtail_cjkcms-24.5.1/wagtail_cjkcms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-cjkcms
-Version: 24.3.2
+Version: 24.5.1
 Summary: Wagtail Content Management System, installable as a Django app into any Wagtail 4.1.x/5.x/6.x site.
 Author-email: Grzegorz Krol <gk@cjk.pl>
 License: BSD-3-Clause
 Project-URL: Homepage, https://cjkcms.com
 Project-URL: Repository, https://github.com/cjkpl/wagtail-cjkcms
 Keywords: wagtail,django,cms
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-cjkcms-24.3.2/wagtail_cjkcms.egg-info/SOURCES.txt` & `wagtail_cjkcms-24.5.1/wagtail_cjkcms.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 cjkcms/migrations/0014_navbar_alignment.py
 cjkcms/migrations/0015_eventcalendar.py
 cjkcms/migrations/0016_layoutsettings_breadcrumb_icon_and_more.py
 cjkcms/migrations/0017_layoutsettings_default_seo_image.py
 cjkcms/migrations/0018_layoutsettings_search_format.py
 cjkcms/migrations/0019_layoutsettings_searchbox_input_class_and_more.py
 cjkcms/migrations/0020_socialmediasettings_github_and_more.py
+cjkcms/migrations/0021_remove_layoutsettings_navbar_color_scheme_and_more.py
 cjkcms/migrations/__init__.py
 cjkcms/models/__init__.py
 cjkcms/models/admin_sidebar.py
 cjkcms/models/cms_models.py
 cjkcms/models/integration_models.py
 cjkcms/models/page_models.py
 cjkcms/models/snippet_models.py
@@ -146,14 +147,15 @@
 cjkcms/project_template/webpack/search/templates/search/search.html
 cjkcms/static/cjkcms/bi/bootstrap-icons.css
 cjkcms/static/cjkcms/bi/bootstrap-icons.json
 cjkcms/static/cjkcms/bi/bootstrap-icons.scss
 cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
 cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
 cjkcms/static/cjkcms/css/cjkcms-admin.css
+cjkcms/static/cjkcms/css/cjkcms-custom-theme-disabled.css
 cjkcms/static/cjkcms/css/cjkcms-editor.css
 cjkcms/static/cjkcms/css/cjkcms-front.css
 cjkcms/static/cjkcms/images/avatars/default.png
 cjkcms/static/cjkcms/images/avatars/default.svg
 cjkcms/static/cjkcms/images/icons/calendar-day.svg
 cjkcms/static/cjkcms/images/icons/caret-right-fill.svg
 cjkcms/static/cjkcms/images/icons/caret-right.svg
@@ -166,14 +168,17 @@
 cjkcms/static/cjkcms/images/patterns/pattern1.jpg
 cjkcms/static/cjkcms/images/patterns/pattern2.jpg
 cjkcms/static/cjkcms/images/patterns/pattern3.jpg
 cjkcms/static/cjkcms/js/cjkcms-editor.js
 cjkcms/static/cjkcms/js/cjkcms-front.js
 cjkcms/static/cookieconsent/cookieconsent.css
 cjkcms/static/cookieconsent/cookieconsent.js
+cjkcms/static/vendor/mdb/css/mdb.dark.min.css
+cjkcms/static/vendor/mdb/css/mdb.min.css
+cjkcms/static/vendor/mdb/js/mdb.umd.min.js
 cjkcms/templates/404.html
 cjkcms/templates/500.html
 cjkcms/templates/cjkcms/robots.txt
 cjkcms/templates/cjkcms/blocks/accordion_block.html
 cjkcms/templates/cjkcms/blocks/article_block_card.html
 cjkcms/templates/cjkcms/blocks/article_masonry_card.html
 cjkcms/templates/cjkcms/blocks/base_block.html
@@ -317,19 +322,15 @@
 cjkcms/tests/test_search_blocks.py
 cjkcms/tests/test_settings.py
 cjkcms/tests/test_templatetags.py
 cjkcms/tests/test_urls.py
 cjkcms/tests/test_webpage.py
 cjkcms/tests/urls.py
 cjkcms/tests/media/images/test.original.png
-cjkcms/tests/media/images/test_3tYv0uS.original.png
-cjkcms/tests/media/images/test_d8sVYy7.original.png
 cjkcms/tests/media/original_images/test.png
-cjkcms/tests/media/original_images/test_3tYv0uS.png
-cjkcms/tests/media/original_images/test_d8sVYy7.png
 cjkcms/tests/testapp/__init__.py
 cjkcms/tests/testapp/apps.py
 cjkcms/tests/testapp/models.py
 cjkcms/tests/testapp/migrations/0001_initial.py
 cjkcms/tests/testapp/migrations/0002_create_homepage.py
 cjkcms/tests/testapp/migrations/__init__.py
 docs/index.md
```

