# Comparing `tmp/tryton-7.2.0.tar.gz` & `tmp/tryton-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryton-7.2.0.tar", last modified: Mon Apr 29 15:55:22 2024, max compression
+gzip compressed data, was "tryton-7.2.1.tar", last modified: Wed May  1 09:13:37 2024, max compression
```

## Comparing `tryton-7.2.0.tar` & `tryton-7.2.1.tar`

### file list

```diff
@@ -1,369 +1,369 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.139330 tryton-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)    19169 2024-04-29 15:30:59.000000 tryton-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-29 15:30:59.000000 tryton-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 tryton-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-02-04 18:51:26.000000 tryton-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2545 2024-04-29 15:55:22.135997 tryton-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-04-15 07:12:15.000000 tryton-7.2.0/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.115997 tryton-7.2.0/bin/
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2055 2024-03-17 11:01:36.000000 tryton-7.2.0/bin/tryton
--rw-r--r--   0 ced       (1000) ced       (1000)     1101 2023-01-16 14:00:21.000000 tryton-7.2.0/catalan.nsh
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/darwin/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.115997 tryton-7.2.0/darwin/gtk-3.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3255 2023-01-16 14:00:21.000000 tryton-7.2.0/darwin/gtk-3.0/gdk-pixbuf.loaders
--rw-r--r--   0 ced       (1000) ced       (1000)     1863 2023-01-16 14:00:21.000000 tryton-7.2.0/darwin/gtk-3.0/gtk.immodules
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.115997 tryton-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2222 2024-04-27 16:30:39.000000 tryton-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5990 2023-04-15 07:12:15.000000 tryton-7.2.0/doc/glossary.rst
--rwxr-xr-x   0 ced       (1000) ced       (1000)      290 2023-04-15 07:12:15.000000 tryton-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2023-04-15 07:12:15.000000 tryton-7.2.0/doc/installation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 tryton-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-02-04 18:51:27.000000 tryton-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)    19223 2024-04-27 16:30:39.000000 tryton-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-01-16 14:00:21.000000 tryton-7.2.0/english.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1796 2023-01-16 14:00:21.000000 tryton-7.2.0/farsi.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1089 2023-01-16 14:00:21.000000 tryton-7.2.0/french.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1082 2023-01-16 14:00:21.000000 tryton-7.2.0/german.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)      487 2024-04-22 12:14:36.000000 tryton-7.2.0/make-darwin-installer.sh
--rw-r--r--   0 ced       (1000) ced       (1000)      323 2023-04-15 07:12:15.000000 tryton-7.2.0/make-win32-installer.sh
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-01-16 14:00:21.000000 tryton-7.2.0/portuguese.nsh
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4571 2024-04-29 13:17:17.000000 tryton-7.2.0/setup-freeze.py
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2024-04-29 15:55:22.139330 tryton-7.2.0/setup.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     5822 2023-04-15 07:12:15.000000 tryton-7.2.0/setup.nsi
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4471 2024-04-27 16:30:39.000000 tryton-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1039 2023-01-16 14:00:21.000000 tryton-7.2.0/slovenian.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)     1095 2023-01-16 14:00:21.000000 tryton-7.2.0/spanish.nsh
--rw-r--r--   0 ced       (1000) ced       (1000)      278 2024-03-17 11:01:36.000000 tryton-7.2.0/tox.ini
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.119331 tryton-7.2.0/tryton/
--rw-r--r--   0 ced       (1000) ced       (1000)     1926 2024-04-29 15:30:54.000000 tryton-7.2.0/tryton/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.119331 tryton-7.2.0/tryton/action/
--rw-r--r--   0 ced       (1000) ced       (1000)      189 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/action/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6758 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/action/main.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2874 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)      990 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3323 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/client.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/common/
--rw-r--r--   0 ced       (1000) ced       (1000)     2446 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/common/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2048 2024-04-22 12:01:28.000000 tryton-7.2.0/tryton/common/button.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6611 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/common/cellrendererbinary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3023 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/cellrendererbutton.py
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/common/cellrendererclickablepixbuf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      473 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/cellrenderercombo.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2348 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/cellrendererfloat.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1094 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/cellrendererinteger.py
--rw-r--r--   0 ced       (1000) ced       (1000)      881 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/cellrenderertext.py
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/cellrenderertoggle.py
--rw-r--r--   0 ced       (1000) ced       (1000)    49195 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/common/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3035 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/common/completion.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20394 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/common/datetime_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18457 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/common/domain_inversion.py
--rw-r--r--   0 ced       (1000) ced       (1000)    29157 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/common/domain_parser.py
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/common/entry_position.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1848 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/common/environment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2471 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/focus.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14404 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/htmltextbuffer.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3644 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/common/number_entry.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5779 2024-03-17 11:01:36.000000 tryton-7.2.0/tryton/common/popup_menu.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11247 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/richtext.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8538 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/common/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)      766 2024-03-17 11:01:36.000000 tryton-7.2.0/tryton/common/tempfile.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3180 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/common/underline.py
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/common/widget_style.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9270 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/config.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.115997 tryton-7.2.0/tryton/data/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/bg/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/bg/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     8720 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/bg/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    22191 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/bg/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/ca/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/ca/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19439 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/ca/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21181 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/ca/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/cs/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/cs/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     4634 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/cs/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    18523 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/cs/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/de/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/de/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19988 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/de/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21762 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/de/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/es/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/es/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19720 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/es/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21683 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/es/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/es_419/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     7060 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    16689 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/et/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/et/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    13450 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/et/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19223 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/et/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/fa/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/fa/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    16677 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/fa/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    23114 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/fa/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/fi/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/fi/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/fi/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    14303 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/fi/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/fr/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/fr/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    20364 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/fr/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21907 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/fr/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/hu/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/hu/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    17126 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/hu/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21213 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/hu/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/id/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/id/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     6983 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/id/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    16252 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/id/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/it/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/it/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    15005 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/it/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20145 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/it/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/ja_JP/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     7061 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    36736 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/lo/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/lo/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18359 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/lo/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    27674 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/lo/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/lt/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/lt/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    16169 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/lt/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21211 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/lt/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/nl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/nl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19339 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/nl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20912 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/nl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/pl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.122664 tryton-7.2.0/tryton/data/locale/pl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    17502 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/pl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20594 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/pl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/pt/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/pt/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    15086 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/pt/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20696 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/pt/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/ro/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/ro/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    19655 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/ro/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    21097 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/ro/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/ru/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/ru/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     9949 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/ru/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    22633 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/ru/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/sl/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/sl/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18877 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/sl/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    20515 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/sl/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/tr/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/tr/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)     1696 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/tr/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    14840 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/tr/LC_MESSAGES/tryton.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14091 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/tryton.pot
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/uk/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/uk/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    22925 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/uk/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    25573 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/uk/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.112664 tryton-7.2.0/tryton/data/locale/zh_CN/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.125997 tryton-7.2.0/tryton/data/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 ced       (1000) ced       (1000)    18082 2024-04-29 15:30:55.000000 tryton-7.2.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo
--rw-r--r--   0 ced       (1000) ced       (1000)    19744 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.115997 tryton-7.2.0/tryton/data/pixmaps/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.129330 tryton-7.2.0/tryton/data/pixmaps/tryton/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-add.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-archive.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-arrow-down.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      483 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-arrow-left.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-arrow-right.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-arrow-up.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-attach.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-back.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-02-04 18:51:26.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-barcode-scanner.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-bookmark-border.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      209 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-bookmark.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-bookmarks.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      325 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-cancel.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-clear.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      251 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-close.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      286 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-copy.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-create.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-date.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-delete.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-download.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-drag.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-email.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-error.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-exit.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-export.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-filter.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-align-center.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-align-justify.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-align-left.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-align-right.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      379 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-bold.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-color-text.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      198 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-italic.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-format-underline.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-forward.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-history.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-icon.png
--rw-r--r--   0 ced       (1000) ced       (1000)     1447 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-icon.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      330 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-import.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      246 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-info.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-launch.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-link.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      350 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-log.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-menu.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-note.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-ok.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-open.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-print.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-public.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-question.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-refresh.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      167 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-remove.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-save.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-search.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      175 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-send.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-sound-off.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-sound-on.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-star-border.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-star.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      221 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-switch.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-translate.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      558 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-unarchive.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-undo.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      200 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-warning.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    26698 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton.icns
--rw-r--r--   0 ced       (1000) ced       (1000)    62686 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton.ico
--rw-r--r--   0 ced       (1000) ced       (1000)     1603 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/data/pixmaps/tryton/tryton.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.129330 tryton-7.2.0/tryton/data/sounds/
--rw-r--r--   0 ced       (1000) ced       (1000)    18650 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/sounds/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)    25190 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/sounds/danger.wav
--rw-r--r--   0 ced       (1000) ced       (1000)    47812 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/data/sounds/success.wav
--rw-r--r--   0 ced       (1000) ced       (1000)     1889 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/device_cookie.py
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1388 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/fingerprints.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.129330 tryton-7.2.0/tryton/gui/
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    42451 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/main.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/
--rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1726 2024-04-29 15:30:59.000000 tryton-7.2.0/tryton/gui/window/about.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3693 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/attachment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1903 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/board.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3495 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/code_scanner.py
--rw-r--r--   0 ced       (1000) ced       (1000)    30067 2024-03-17 11:01:36.000000 tryton-7.2.0/tryton/gui/window/dblogin.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13577 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    34496 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/form.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1498 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/gui/window/infobar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2615 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/limit.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4568 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/log.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1673 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/nomodal.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1319 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/note.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3936 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/preference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4362 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/revision.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11187 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/tabcontent.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/view_board/
--rw-r--r--   0 ced       (1000) ced       (1000)      201 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_board/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5502 2024-04-13 15:40:11.000000 tryton-7.2.0/tryton/gui/window/view_board/action.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_board/view_board.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/view_form/
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/view_form/model/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/gui/window/view_form/model/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    44900 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/view_form/model/field.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18391 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/view_form/model/group.py
--rw-r--r--   0 ced       (1000) ced       (1000)    28847 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/view_form/model/record.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/view_form/screen/
--rw-r--r--   0 ced       (1000) ced       (1000)      191 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/screen/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    53483 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/view_form/screen/screen.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/view_form/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     4386 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6078 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/gui/window/view_form/view/calendar_.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.132664 tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5611 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9781 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22623 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8334 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5951 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6525 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1229 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/checkbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22276 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/dictionary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3340 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/document.py
--rw-r--r--   0 ced       (1000) ced       (1000)      733 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3984 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/image.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3088 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12987 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14507 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3690 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23379 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1397 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/progressbar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1759 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4948 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2815 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/richtextbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3510 2023-05-30 16:04:29.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7600 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/state_widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5703 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/textbox.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1619 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5102 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/url.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10682 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6499 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/view_form/view/graph.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8752 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/bar.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15976 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/graph.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10359 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/line.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7241 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/pie.py
--rw-r--r--   0 ced       (1000) ced       (1000)    51754 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/view_form/view/list.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6984 2024-02-04 18:51:27.000000 tryton-7.2.0/tryton/gui/window/view_form/view/list_form.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton/gui/window/view_form/view/list_gtk/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton/gui/window/view_form/view/list_gtk/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13835 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/view_form/view/list_gtk/editabletree.py
--rw-r--r--   0 ced       (1000) ced       (1000)    51643 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/view_form/view/list_gtk/widget.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25839 2024-02-22 09:33:24.000000 tryton-7.2.0/tryton/gui/window/view_form/view/screen_container.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13513 2024-01-27 09:58:52.000000 tryton-7.2.0/tryton/gui/window/win_csv.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21199 2024-03-17 11:01:36.000000 tryton-7.2.0/tryton/gui/window/win_export.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19456 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/gui/window/win_form.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9601 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/win_import.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5975 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/gui/window/win_search.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1736 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/gui/window/window.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14972 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/gui/window/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13986 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/jsonrpc.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton/plugins/
--rw-r--r--   0 ced       (1000) ced       (1000)     1449 2024-04-29 13:17:17.000000 tryton-7.2.0/tryton/plugins/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton/plugins/translation/
--rw-r--r--   0 ced       (1000) ced       (1000)      697 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/plugins/translation/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23751 2024-04-27 16:30:39.000000 tryton-7.2.0/tryton/pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5513 2024-04-22 12:14:37.000000 tryton-7.2.0/tryton/rpc.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1428 2023-06-10 11:39:56.000000 tryton-7.2.0/tryton/tests/test_common.py
--rw-r--r--   0 ced       (1000) ced       (1000)    43500 2024-04-13 15:19:53.000000 tryton-7.2.0/tryton/tests/test_common_domain_parser.py
--rw-r--r--   0 ced       (1000) ced       (1000)      649 2023-04-15 07:12:16.000000 tryton-7.2.0/tryton/tests/test_common_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3538 2023-04-15 07:12:15.000000 tryton-7.2.0/tryton/tests/test_common_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6659 2024-03-17 11:01:36.000000 tryton-7.2.0/tryton/translate.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1222 2023-01-16 14:00:21.000000 tryton-7.2.0/tryton.desktop
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/tryton.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2545 2024-04-29 15:55:21.000000 tryton-7.2.0/tryton.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    10960 2024-04-29 15:55:22.000000 tryton-7.2.0/tryton.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:55:21.000000 tryton-7.2.0/tryton.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:54.000000 tryton-7.2.0/tryton.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:55:21.000000 tryton-7.2.0/tryton.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        7 2024-04-29 15:55:21.000000 tryton-7.2.0/tryton.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.115997 tryton-7.2.0/win32/
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:55:22.135997 tryton-7.2.0/win32/gtk-3.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     3421 2023-01-16 14:00:21.000000 tryton-7.2.0/win32/gtk-3.0/gdk-pixbuf.loaders
--rw-r--r--   0 ced       (1000) ced       (1000)        0 2023-01-16 14:00:21.000000 tryton-7.2.0/win32/gtk-3.0/gtk.immodules
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.193041 tryton-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19270 2024-05-01 09:13:34.000000 tryton-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-05-01 09:13:33.000000 tryton-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 tryton-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:21:00.000000 tryton-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2545 2024-05-01 09:13:37.193041 tryton-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-30 17:21:00.000000 tryton-7.2.1/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.169709 tryton-7.2.1/bin/
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     2055 2024-04-30 17:21:00.000000 tryton-7.2.1/bin/tryton
+-rw-r--r--   0 ced       (1000) ced       (1000)     1101 2024-04-30 17:21:00.000000 tryton-7.2.1/catalan.nsh
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/darwin/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.169709 tryton-7.2.1/darwin/gtk-3.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3255 2024-04-30 17:21:00.000000 tryton-7.2.1/darwin/gtk-3.0/gdk-pixbuf.loaders
+-rw-r--r--   0 ced       (1000) ced       (1000)     1863 2024-04-30 17:21:00.000000 tryton-7.2.1/darwin/gtk-3.0/gtk.immodules
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.173042 tryton-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2222 2024-04-30 17:21:00.000000 tryton-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5990 2024-04-30 17:21:00.000000 tryton-7.2.1/doc/glossary.rst
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      290 2024-04-30 17:21:00.000000 tryton-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2024-04-30 17:21:00.000000 tryton-7.2.1/doc/installation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 tryton-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 tryton-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)    19223 2024-04-30 17:21:00.000000 tryton-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      984 2024-04-30 17:21:00.000000 tryton-7.2.1/english.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1796 2024-04-30 17:21:00.000000 tryton-7.2.1/farsi.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1089 2024-04-30 17:21:00.000000 tryton-7.2.1/french.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1082 2024-04-30 17:21:00.000000 tryton-7.2.1/german.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)      487 2024-04-30 17:21:00.000000 tryton-7.2.1/make-darwin-installer.sh
+-rw-r--r--   0 ced       (1000) ced       (1000)      323 2024-04-30 17:21:00.000000 tryton-7.2.1/make-win32-installer.sh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2024-04-30 17:21:00.000000 tryton-7.2.1/portuguese.nsh
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4571 2024-04-30 17:21:00.000000 tryton-7.2.1/setup-freeze.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2024-05-01 09:13:37.226374 tryton-7.2.1/setup.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5822 2024-04-30 17:21:00.000000 tryton-7.2.1/setup.nsi
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4471 2024-04-30 17:21:00.000000 tryton-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1039 2024-04-30 17:21:00.000000 tryton-7.2.1/slovenian.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)     1095 2024-04-30 17:21:00.000000 tryton-7.2.1/spanish.nsh
+-rw-r--r--   0 ced       (1000) ced       (1000)      278 2024-04-30 17:21:00.000000 tryton-7.2.1/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.173042 tryton-7.2.1/tryton/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1926 2024-04-30 17:21:06.000000 tryton-7.2.1/tryton/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.173042 tryton-7.2.1/tryton/action/
+-rw-r--r--   0 ced       (1000) ced       (1000)      189 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/action/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6758 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/action/main.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2874 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      990 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3323 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/client.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/common/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2446 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2048 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/button.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6611 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/cellrendererbinary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3023 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/cellrendererbutton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      706 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/cellrendererclickablepixbuf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      473 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/cellrenderercombo.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2348 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/cellrendererfloat.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1094 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/cellrendererinteger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      881 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/cellrenderertext.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/cellrenderertoggle.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    49195 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3035 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/completion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20394 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/datetime_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18457 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/domain_inversion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    29157 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/domain_parser.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/entry_position.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1848 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/environment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2471 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/focus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14404 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/htmltextbuffer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3644 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/number_entry.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5779 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/popup_menu.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11247 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/richtext.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8538 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      766 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/tempfile.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3180 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      714 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/underline.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/common/widget_style.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9270 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/config.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.169709 tryton-7.2.1/tryton/data/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/bg/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8720 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/bg/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    22353 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/bg/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/ca/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    20327 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/ca/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21574 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/ca/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/cs/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4634 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/cs/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    18675 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/cs/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/de/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/de/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    20876 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/de/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    22140 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/de/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/es/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/es/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    20586 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/es/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    22042 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/es/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/es_419/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7060 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    16845 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/es_419/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/et/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/et/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    13450 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/et/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19370 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/et/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/fa/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16677 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/fa/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    23271 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/fa/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/fi/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/fi/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    14424 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/fi/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/fr/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    21119 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/fr/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    22315 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/fr/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/hu/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    17126 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/hu/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21371 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/hu/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/id/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/id/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6983 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/id/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    16373 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/id/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/it/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/it/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    15005 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/it/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20299 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/it/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/ja_JP/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7061 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    36736 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/lo/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/lo/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18359 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/lo/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    27885 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/lo/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/lt/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16169 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/lt/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21377 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/lt/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/nl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    20094 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/nl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21267 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/nl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/pl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.176375 tryton-7.2.1/tryton/data/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    20027 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/pl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21139 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/pl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/pt/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.179708 tryton-7.2.1/tryton/data/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    15086 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/pt/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20852 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/pt/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/ro/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.179708 tryton-7.2.1/tryton/data/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    19655 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/ro/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    21253 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/ro/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.166375 tryton-7.2.1/tryton/data/locale/ru/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.179708 tryton-7.2.1/tryton/data/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     9949 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/ru/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    22823 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/ru/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.169709 tryton-7.2.1/tryton/data/locale/sl/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.179708 tryton-7.2.1/tryton/data/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18877 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/sl/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    20672 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/sl/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.169709 tryton-7.2.1/tryton/data/locale/tr/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.179708 tryton-7.2.1/tryton/data/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1696 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/tr/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    14961 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/tr/LC_MESSAGES/tryton.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14145 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/tryton.pot
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.169709 tryton-7.2.1/tryton/data/locale/uk/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.179708 tryton-7.2.1/tryton/data/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    22925 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/uk/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    25755 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/uk/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.169709 tryton-7.2.1/tryton/data/locale/zh_CN/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.179708 tryton-7.2.1/tryton/data/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18082 2024-05-01 09:13:30.000000 tryton-7.2.1/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo
+-rw-r--r--   0 ced       (1000) ced       (1000)    19892 2024-04-30 17:21:59.000000 tryton-7.2.1/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.169709 tryton-7.2.1/tryton/data/pixmaps/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.183042 tryton-7.2.1/tryton/data/pixmaps/tryton/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-add.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-archive.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-arrow-down.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      483 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-arrow-left.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-arrow-right.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-arrow-up.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-attach.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-back.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-barcode-scanner.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-bookmark-border.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      209 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-bookmark.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-bookmarks.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      325 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-cancel.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-clear.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      251 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-close.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      286 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-copy.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-create.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-date.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-delete.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-download.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-drag.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-email.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-error.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-exit.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-export.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-filter.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-format-align-center.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-format-align-justify.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-format-align-left.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-format-align-right.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      379 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-format-bold.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-format-color-text.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      198 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-format-italic.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-format-underline.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-forward.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-history.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-icon.png
+-rw-r--r--   0 ced       (1000) ced       (1000)     1447 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-icon.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      330 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-import.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      246 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-info.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-launch.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-link.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      350 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-log.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      195 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-menu.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-note.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      199 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-ok.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-open.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-print.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-public.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-question.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-refresh.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      167 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-remove.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-save.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-search.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      175 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-send.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-sound-off.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-sound-on.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-star-border.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-star.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      221 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-switch.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-translate.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      558 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-unarchive.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-undo.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      200 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-warning.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    26698 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton.icns
+-rw-r--r--   0 ced       (1000) ced       (1000)    62686 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton.ico
+-rw-r--r--   0 ced       (1000) ced       (1000)     1603 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/pixmaps/tryton/tryton.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.183042 tryton-7.2.1/tryton/data/sounds/
+-rw-r--r--   0 ced       (1000) ced       (1000)    18650 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/sounds/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)    25190 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/sounds/danger.wav
+-rw-r--r--   0 ced       (1000) ced       (1000)    47812 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/data/sounds/success.wav
+-rw-r--r--   0 ced       (1000) ced       (1000)     1889 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/device_cookie.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1388 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/fingerprints.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.183042 tryton-7.2.1/tryton/gui/
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    42451 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/main.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.186375 tryton-7.2.1/tryton/gui/window/
+-rw-r--r--   0 ced       (1000) ced       (1000)      191 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1726 2024-05-01 09:13:33.000000 tryton-7.2.1/tryton/gui/window/about.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3693 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/attachment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1903 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/board.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3495 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/code_scanner.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    30067 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/dblogin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13577 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    34496 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/form.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1498 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/infobar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2615 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/limit.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4568 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1673 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/nomodal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1319 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/note.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3936 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/preference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4362 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/revision.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11187 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/tabcontent.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.186375 tryton-7.2.1/tryton/gui/window/view_board/
+-rw-r--r--   0 ced       (1000) ced       (1000)      201 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_board/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5502 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_board/action.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1810 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_board/view_board.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.186375 tryton-7.2.1/tryton/gui/window/view_form/
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.186375 tryton-7.2.1/tryton/gui/window/view_form/model/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/model/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    44900 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/model/field.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18391 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/model/group.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    28847 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/model/record.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.186375 tryton-7.2.1/tryton/gui/window/view_form/screen/
+-rw-r--r--   0 ced       (1000) ced       (1000)      191 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/screen/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    53483 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/screen/screen.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.186375 tryton-7.2.1/tryton/gui/window/view_form/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4386 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6078 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/calendar_.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.186375 tryton-7.2.1/tryton/gui/window/view_form/view/calendar_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/calendar_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5611 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9781 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22623 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.189708 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8334 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5951 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6525 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1229 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/checkbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22276 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/dictionary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3340 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/document.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      733 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3984 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/image.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3088 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12987 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14507 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3690 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23379 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1397 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/progressbar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1759 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4948 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2815 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/richtextbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3510 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7600 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/state_widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5703 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/textbox.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1619 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5102 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/url.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10682 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6499 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/graph.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.189708 tryton-7.2.1/tryton/gui/window/view_form/view/graph_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/graph_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8752 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/graph_gtk/bar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15976 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/graph_gtk/graph.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10359 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/graph_gtk/line.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7241 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/graph_gtk/pie.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    51754 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/list.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6984 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/list_form.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.189708 tryton-7.2.1/tryton/gui/window/view_form/view/list_gtk/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/list_gtk/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13835 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/list_gtk/editabletree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    51643 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/list_gtk/widget.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25839 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/view_form/view/screen_container.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13513 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/win_csv.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21199 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/win_export.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19456 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/win_form.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9601 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/win_import.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5975 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/win_search.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1736 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/window.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14972 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/gui/window/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13986 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/jsonrpc.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.189708 tryton-7.2.1/tryton/plugins/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1449 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/plugins/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.189708 tryton-7.2.1/tryton/plugins/translation/
+-rw-r--r--   0 ced       (1000) ced       (1000)      697 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/plugins/translation/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23751 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5513 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/rpc.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.189708 tryton-7.2.1/tryton/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1428 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/tests/test_common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    43500 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/tests/test_common_domain_parser.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      649 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/tests/test_common_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3538 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/tests/test_common_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6659 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton/translate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1222 2024-04-30 17:21:00.000000 tryton-7.2.1/tryton.desktop
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.189708 tryton-7.2.1/tryton.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2545 2024-05-01 09:13:36.000000 tryton-7.2.1/tryton.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    10960 2024-05-01 09:13:37.000000 tryton-7.2.1/tryton.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:13:36.000000 tryton-7.2.1/tryton.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:13:36.000000 tryton-7.2.1/tryton.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-05-01 09:13:36.000000 tryton-7.2.1/tryton.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        7 2024-05-01 09:13:36.000000 tryton-7.2.1/tryton.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.169709 tryton-7.2.1/win32/
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:13:37.189708 tryton-7.2.1/win32/gtk-3.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3421 2024-04-30 17:21:00.000000 tryton-7.2.1/win32/gtk-3.0/gdk-pixbuf.loaders
+-rw-r--r--   0 ced       (1000) ced       (1000)        0 2024-04-30 17:21:00.000000 tryton-7.2.1/win32/gtk-3.0/gtk.immodules
```

### Comparing `tryton-7.2.0/CHANGELOG` & `tryton-7.2.1/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.2.1 - 2024-05-01
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Read xxx2Many fields using the dotted notation
 * Display XML ID on Log window
 * Use operators when converting PYSON to string
 * Add contextual menu to copy cell and column
```

### Comparing `tryton-7.2.0/COPYRIGHT` & `tryton-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/LICENSE` & `tryton-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/PKG-INFO` & `tryton-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tryton
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton desktop client
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `tryton-7.2.0/bin/tryton` & `tryton-7.2.1/bin/tryton`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/catalan.nsh` & `tryton-7.2.1/catalan.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/darwin/gtk-3.0/gdk-pixbuf.loaders` & `tryton-7.2.1/darwin/gtk-3.0/gdk-pixbuf.loaders`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/darwin/gtk-3.0/gtk.immodules` & `tryton-7.2.1/darwin/gtk-3.0/gtk.immodules`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/doc/conf.py` & `tryton-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/doc/glossary.rst` & `tryton-7.2.1/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/doc/installation.rst` & `tryton-7.2.1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/doc/usage.rst` & `tryton-7.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/english.nsh` & `tryton-7.2.1/english.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/farsi.nsh` & `tryton-7.2.1/farsi.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/french.nsh` & `tryton-7.2.1/french.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/german.nsh` & `tryton-7.2.1/german.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/portuguese.nsh` & `tryton-7.2.1/portuguese.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/setup-freeze.py` & `tryton-7.2.1/setup-freeze.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/setup.nsi` & `tryton-7.2.1/setup.nsi`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/setup.py` & `tryton-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/slovenian.nsh` & `tryton-7.2.1/slovenian.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/spanish.nsh` & `tryton-7.2.1/spanish.nsh`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/__init__.py` & `tryton-7.2.1/tryton/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-__version__ = "7.2.0"
+__version__ = "7.2.1"
 import locale
 
 import gi
 
 gi.require_version('Gtk', '3.0')
 gi.require_version('Gdk', '3.0')
 gi.require_foreign('cairo')
```

### Comparing `tryton-7.2.0/tryton/action/main.py` & `tryton-7.2.1/tryton/action/main.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/bus.py` & `tryton-7.2.1/tryton/bus.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/cache.py` & `tryton-7.2.1/tryton/cache.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/client.py` & `tryton-7.2.1/tryton/client.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/__init__.py` & `tryton-7.2.1/tryton/common/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/button.py` & `tryton-7.2.1/tryton/common/button.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/cellrendererbinary.py` & `tryton-7.2.1/tryton/common/cellrendererbinary.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/cellrendererbutton.py` & `tryton-7.2.1/tryton/common/cellrendererbutton.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/cellrendererclickablepixbuf.py` & `tryton-7.2.1/tryton/common/cellrendererclickablepixbuf.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/cellrendererfloat.py` & `tryton-7.2.1/tryton/common/cellrendererfloat.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/cellrendererinteger.py` & `tryton-7.2.1/tryton/common/cellrendererinteger.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/cellrenderertext.py` & `tryton-7.2.1/tryton/common/cellrenderertext.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/common.py` & `tryton-7.2.1/tryton/common/common.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/completion.py` & `tryton-7.2.1/tryton/common/completion.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/datetime_.py` & `tryton-7.2.1/tryton/common/datetime_.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/domain_inversion.py` & `tryton-7.2.1/tryton/common/domain_inversion.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/domain_parser.py` & `tryton-7.2.1/tryton/common/domain_parser.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/environment.py` & `tryton-7.2.1/tryton/common/environment.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/focus.py` & `tryton-7.2.1/tryton/common/focus.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/htmltextbuffer.py` & `tryton-7.2.1/tryton/common/htmltextbuffer.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/number_entry.py` & `tryton-7.2.1/tryton/common/number_entry.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/popup_menu.py` & `tryton-7.2.1/tryton/common/popup_menu.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/richtext.py` & `tryton-7.2.1/tryton/common/richtext.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/selection.py` & `tryton-7.2.1/tryton/common/selection.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/tempfile.py` & `tryton-7.2.1/tryton/common/tempfile.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/timedelta.py` & `tryton-7.2.1/tryton/common/timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/common/underline.py` & `tryton-7.2.1/tryton/common/underline.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/config.py` & `tryton-7.2.1/tryton/config.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/data/locale/bg/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/bg/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: bg\n"
 "Language-Team: bg <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/bg/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/bg/LC_MESSAGES/tryton.po`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,16 @@
 
 msgid "No"
 msgstr ""
 
 msgid "Yes"
 msgstr ""
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "Грешка при достъп"
 
 msgid "This record has been modified while you were editing it."
 msgstr ""
 
 msgid "Cancel saving"
 msgstr ""
@@ -115,14 +116,17 @@
 msgid "Close"
 msgstr ""
 
 #, fuzzy
 msgid "Application Error"
 msgstr "Грешка в приложението!"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "Съобщаване за грешка"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr ""
 
@@ -131,20 +135,23 @@
 
 msgid "A new version is available!"
 msgstr ""
 
 msgid "Download"
 msgstr ""
 
+msgid "Concurrency Exception"
+msgstr "Грешка при достъп"
+
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Не може да се свърже със сървъра!"
 
 #, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr ""
 
 msgid "Too many requests. Try again later."
 msgstr ""
 
 msgid "Not Found."
 msgstr ""
@@ -768,14 +775,20 @@
 
 msgid "Model:"
 msgstr "Модел:"
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 #, fuzzy
 msgid "Created by:"
 msgstr "Дата на създаване:"
 
 #, fuzzy
 msgid "Created at:"
 msgstr "Дата на създаване:"
```

### Comparing `tryton-7.2.0/tryton/data/locale/ca/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/ca/LC_MESSAGES/tryton.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ca\n"
 "Language-Team: ca <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -78,14 +78,21 @@
 
 msgid "<i>Search...</i>"
 msgstr "<i>Cerca...</i>"
 
 msgid "A new version is available!"
 msgstr "Hi ha una nova versió disponible!"
 
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+"S'ha enviat una sol·licitud per restablir la contrasenya.\n"
+"Si us plau, comproveu la vostra bústia de correu."
+
 msgid "A_ttachments..."
 msgstr "Adjun_ts..."
 
 msgid "About..."
 msgstr "Quant a..."
 
 msgid "Action"
@@ -243,20 +250,32 @@
 
 msgid "Compare: %s"
 msgstr "Compara: %s"
 
 msgid "Concurrency Exception"
 msgstr "Excepció de concurrència"
 
+msgid "Concurrency Warning"
+msgstr "Avís de concurrència"
+
 msgid "Connect the Tryton server"
 msgstr "Connecta amb el servidor Tryton"
 
 msgid "Copy"
 msgstr "Copia"
 
+msgid "Copy Column"
+msgstr "Copia columna"
+
+msgid "Copy Row"
+msgstr "Copia fila"
+
+msgid "Copy Rows"
+msgstr "Copia les files"
+
 msgid "Copy URL into clipboard"
 msgstr "Copia l'URL al porta-retalls"
 
 msgid "Copy _URL..."
 msgstr "Copia l'_URL..."
 
 msgid "Copy selected rows"
@@ -321,14 +340,17 @@
 
 msgid "Delete selected record <Del>"
 msgstr "Elimina el registre seleccionat <Supr>"
 
 msgid "Delimiter:"
 msgstr "Separador:"
 
+msgid "Details"
+msgstr "Detalls"
+
 msgid "Detection failed"
 msgstr "Ha fallat la detecció"
 
 msgid "Digits"
 msgstr "Dígits"
 
 msgid "Discard changes"
@@ -384,14 +406,17 @@
 
 msgid "Encoding:"
 msgstr "Codificació:"
 
 msgid "Error"
 msgstr "Error"
 
+msgid "Error: \"%s\". Try again later."
+msgstr "Error: \"%s\". Proveu-ho de nou més tard."
+
 msgid "Expand all rows"
 msgstr "Expandeix totes les files"
 
 msgid "Expand row"
 msgstr "Expandeix fila"
 
 msgid "Expand/Collapse"
@@ -474,14 +499,17 @@
 
 msgid "Incompatible version of the server."
 msgstr "El client no és compatible amb la versió del servidor."
 
 msgid "Insert copied rows"
 msgstr "Inserta les files copiades"
 
+msgid "Invalid response id (%s) expected %s"
+msgstr "ID de resposta (%s) invàlido. S'esperava %s"
+
 msgid "Italic"
 msgstr "Cursiva"
 
 msgid "Justify"
 msgstr "Justificar"
 
 msgid "Keyboard Shortcuts..."
@@ -534,14 +562,17 @@
 
 msgid "Mark line for removal"
 msgstr "Marcar línia per eliminar"
 
 msgid "Model:"
 msgstr "Model:"
 
+msgid "Module:"
+msgstr "Mòdul:"
+
 msgid "Month"
 msgstr "Mes"
 
 msgid "Move Cursor"
 msgstr "Mou cursor"
 
 msgid "Move down"
@@ -651,14 +682,17 @@
 
 msgid "PDA Mode"
 msgstr "Mode PDA"
 
 msgid "PNG image (*.png)"
 msgstr "Imatge PNG (*.png)"
 
+msgid "Paste Rows"
+msgstr "Enganxa files"
+
 msgid "Paste copied text"
 msgstr "Enganxa el text seleccionat"
 
 msgid "Play Sound for Code Scanner"
 msgstr "Activa el so del escàner de codis"
 
 msgid "Pre-validation"
@@ -759,14 +793,17 @@
 
 msgid "Report..."
 msgstr "Informe..."
 
 msgid "Reports"
 msgstr "Informes"
 
+msgid "Reset forgotten password"
+msgstr "Restableix la contrasenya"
+
 msgid "Revision"
 msgstr "Revisió"
 
 msgid "Revision:"
 msgstr "Revisió:"
 
 msgid "Save"
@@ -852,14 +889,17 @@
 
 msgid "Send"
 msgstr "Envia"
 
 msgid "Send an e-mail using the record"
 msgstr "Envia un correu electrònic utilitzant el registre"
 
+msgid "Send you an email to reset your password."
+msgstr "Reb un correu electrònic per restablir la teva contrasenya."
+
 msgid "Shortcuts"
 msgstr "Dreceres"
 
 msgid "Show active records"
 msgstr "Mostra registres actius"
 
 msgid "Show bookmarks of filters"
@@ -1016,14 +1056,17 @@
 
 msgid "Working now on the duplicated record(s)."
 msgstr "Està treballant amb un registre(s) duplicat."
 
 msgid "Write Anyway"
 msgstr "Desa de totes formes"
 
+msgid "XML ID:"
+msgstr "ID XML:"
+
 msgid "Y"
 msgstr "A"
 
 msgid "Yes"
 msgstr "Si"
 
 msgid "You have to select one record."
```

### Comparing `tryton-7.2.0/tryton/data/locale/ca/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/ca/LC_MESSAGES/tryton.po`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 msgstr "Indica el nom:port del servidor"
 
 msgid "disable thread usage"
 msgstr "desactiva l'ús de fils"
 
 #, python-format
 msgid "Invalid response id (%s) expected %s"
-msgstr ""
+msgstr "ID de resposta (%s) invàlido. S'esperava %s"
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "No s'ha pogut establir l'idioma %s"
 
 msgid ", "
 msgstr ", "
@@ -80,16 +80,16 @@
 
 msgid "No"
 msgstr "No"
 
 msgid "Yes"
 msgstr "Si"
 
-msgid "Concurrency Exception"
-msgstr "Excepció de concurrència"
+msgid "Concurrency Warning"
+msgstr "Avís de concurrència"
 
 msgid "This record has been modified while you were editing it."
 msgstr "Aquest registre ha estat modificat mentre l'editàveu."
 
 msgid "Cancel saving"
 msgstr "No desis els canvis"
 
@@ -111,14 +111,17 @@
 
 msgid "Close"
 msgstr "Tanca"
 
 msgid "Application Error"
 msgstr "Error d'aplicació"
 
+msgid "Details"
+msgstr "Detalls"
+
 msgid "Report Bug"
 msgstr "Informa de l'error"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "URL de comprovació: %s"
 
@@ -127,37 +130,42 @@
 
 msgid "A new version is available!"
 msgstr "Hi ha una nova versió disponible!"
 
 msgid "Download"
 msgstr "Baixa"
 
+msgid "Concurrency Exception"
+msgstr "Excepció de concurrència"
+
 msgid "Could not get a session."
 msgstr "No s'ha pogut obtenir una sessió."
 
-#, fuzzy, python-format
-msgid "Error \"%s\". Try again later."
-msgstr "Massa peticions. Proveu-ho de nou més tard."
+#, python-format
+msgid "Error: \"%s\". Try again later."
+msgstr "Error: \"%s\". Proveu-ho de nou més tard."
 
 msgid "Too many requests. Try again later."
 msgstr "Massa peticions. Proveu-ho de nou més tard."
 
 msgid "Not Found."
 msgstr "No s'han trobat."
 
 msgid "Reset forgotten password"
-msgstr ""
+msgstr "Restableix la contrasenya"
 
 msgid "Send you an email to reset your password."
-msgstr ""
+msgstr "Reb un correu electrònic per restablir la teva contrasenya."
 
 msgid ""
 "A request to reset your password has been sent.\n"
 "Please check your mailbox."
 msgstr ""
+"S'ha enviat una sol·licitud per restablir la contrasenya.\n"
+"Si us plau, comproveu la vostra bústia de correu."
 
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Cerca...</i>"
 
@@ -723,14 +731,20 @@
 
 msgid "Model:"
 msgstr "Model:"
 
 msgid "ID:"
 msgstr "Identificador:"
 
+msgid "Module:"
+msgstr "Mòdul:"
+
+msgid "XML ID:"
+msgstr "ID XML:"
+
 msgid "Created by:"
 msgstr "Creat per:"
 
 msgid "Created at:"
 msgstr "Creat el:"
 
 msgid "Last Modified by:"
@@ -1096,28 +1110,25 @@
 
 msgid "Image size too large."
 msgstr "La mida de la imatge és massa gran."
 
 msgid "Copy"
 msgstr "Copia"
 
-#, fuzzy
 msgid "Copy Row"
-msgstr "_Copia l'URL"
+msgstr "Copia fila"
 
-#, fuzzy
 msgid "Copy Rows"
-msgstr "_Copia l'URL"
+msgstr "Copia les files"
 
 msgid "Copy Column"
-msgstr ""
+msgstr "Copia columna"
 
-#, fuzzy
 msgid "Paste Rows"
-msgstr "Enganxa"
+msgstr "Enganxa files"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Obre filtres"
```

### Comparing `tryton-7.2.0/tryton/data/locale/cs/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/cs/LC_MESSAGES/tryton.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: cs\n"
 "Language-Team: cs <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=((n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/cs/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/cs/LC_MESSAGES/tryton.po`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,16 @@
 
 msgid "No"
 msgstr ""
 
 msgid "Yes"
 msgstr ""
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "Výjimka při souběhu"
 
 msgid "This record has been modified while you were editing it."
 msgstr ""
 
 msgid "Cancel saving"
 msgstr ""
@@ -115,14 +116,17 @@
 msgid "Close"
 msgstr ""
 
 #, fuzzy
 msgid "Application Error"
 msgstr "Chyba aplikace!"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "Nahlásit chybu"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr ""
 
@@ -131,20 +135,23 @@
 
 msgid "A new version is available!"
 msgstr ""
 
 msgid "Download"
 msgstr ""
 
+msgid "Concurrency Exception"
+msgstr "Výjimka při souběhu"
+
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Nelze se spojit se serverem!"
 
 #, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr ""
 
 msgid "Too many requests. Try again later."
 msgstr ""
 
 msgid "Not Found."
 msgstr ""
@@ -780,14 +787,20 @@
 
 msgid "Model:"
 msgstr "Model:"
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 #, fuzzy
 msgid "Created by:"
 msgstr "Datum vytvoření:"
 
 #, fuzzy
 msgid "Created at:"
 msgstr "Datum vytvoření:"
```

### Comparing `tryton-7.2.0/tryton/data/locale/de/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/de/LC_MESSAGES/tryton.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -78,14 +78,21 @@
 
 msgid "<i>Search...</i>"
 msgstr "<i>Suche...</i>"
 
 msgid "A new version is available!"
 msgstr "Eine neue Version ist verfügbar!"
 
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+"Eine Anfrage zum Zurücksetzen Ihres Passworts wurde gesendet.\n"
+"Bitte überprüfen Sie Ihr Postfach."
+
 msgid "A_ttachments..."
 msgstr "A_nhänge..."
 
 msgid "About..."
 msgstr "Über..."
 
 msgid "Action"
@@ -243,20 +250,32 @@
 
 msgid "Compare: %s"
 msgstr "Vergleichen: %s"
 
 msgid "Concurrency Exception"
 msgstr "Aktualisierungskonflikt"
 
+msgid "Concurrency Warning"
+msgstr "Aktualisierungskonflikt"
+
 msgid "Connect the Tryton server"
 msgstr "Verbindung zum Tryton Server herstellen"
 
 msgid "Copy"
 msgstr "Kopieren"
 
+msgid "Copy Column"
+msgstr "Spalte kopieren"
+
+msgid "Copy Row"
+msgstr "Zeile kopieren"
+
+msgid "Copy Rows"
+msgstr "Zeilen kopieren"
+
 msgid "Copy URL into clipboard"
 msgstr "URL in Zwischenablage kopieren"
 
 msgid "Copy _URL..."
 msgstr "_URL kopieren..."
 
 msgid "Copy selected rows"
@@ -321,14 +340,17 @@
 
 msgid "Delete selected record <Del>"
 msgstr "Ausgewählte Datensätze löschen <Entf>"
 
 msgid "Delimiter:"
 msgstr "Feldtrenner:"
 
+msgid "Details"
+msgstr "Details"
+
 msgid "Detection failed"
 msgstr "Lesen der Datei fehlgeschlagen"
 
 msgid "Digits"
 msgstr "Nachkommastellen"
 
 msgid "Discard changes"
@@ -384,14 +406,17 @@
 
 msgid "Encoding:"
 msgstr "Zeichenkodierung:"
 
 msgid "Error"
 msgstr "Fehler"
 
+msgid "Error: \"%s\". Try again later."
+msgstr "Fehler: \"%s\". Bitte versuchen Sie es später erneut."
+
 msgid "Expand all rows"
 msgstr "Alle Zeilen ausklappen"
 
 msgid "Expand row"
 msgstr "Zeile ausklappen"
 
 msgid "Expand/Collapse"
@@ -474,14 +499,17 @@
 
 msgid "Incompatible version of the server."
 msgstr "Inkompatible Serverversion."
 
 msgid "Insert copied rows"
 msgstr "Kopierte Zeilen einfügen"
 
+msgid "Invalid response id (%s) expected %s"
+msgstr "Ungültige Antwort-ID (%s) erwartet %s"
+
 msgid "Italic"
 msgstr "Kursiv"
 
 msgid "Justify"
 msgstr "Blocksatz"
 
 msgid "Keyboard Shortcuts..."
@@ -534,14 +562,17 @@
 
 msgid "Mark line for removal"
 msgstr "Zeile zum Entfernen markieren"
 
 msgid "Model:"
 msgstr "Modell:"
 
+msgid "Module:"
+msgstr "Modul:"
+
 msgid "Month"
 msgstr "Monat"
 
 msgid "Move Cursor"
 msgstr "Cursor bewegen"
 
 msgid "Move down"
@@ -651,14 +682,17 @@
 
 msgid "PDA Mode"
 msgstr "Einspaltiger Modus"
 
 msgid "PNG image (*.png)"
 msgstr "PNG-Bild (*.png)"
 
+msgid "Paste Rows"
+msgstr "Zeilen Einfügen"
+
 msgid "Paste copied text"
 msgstr "Ausgewählten Text einfügen"
 
 msgid "Play Sound for Code Scanner"
 msgstr "Ton für Barcode Scanner wiedergeben"
 
 msgid "Pre-validation"
@@ -759,14 +793,17 @@
 
 msgid "Report..."
 msgstr "Berichte..."
 
 msgid "Reports"
 msgstr "Berichte"
 
+msgid "Reset forgotten password"
+msgstr "Vergessenes Passwort zurücksetzen"
+
 msgid "Revision"
 msgstr "Bearbeitung"
 
 msgid "Revision:"
 msgstr "Bearbeitung:"
 
 msgid "Save"
@@ -852,14 +889,17 @@
 
 msgid "Send"
 msgstr "Senden"
 
 msgid "Send an e-mail using the record"
 msgstr "Eine E-Mail basierend auf diesem Datensatz versenden"
 
+msgid "Send you an email to reset your password."
+msgstr "E-Mail zum Zurücksetzen des Passworts senden."
+
 msgid "Shortcuts"
 msgstr "Tastenkombinationen"
 
 msgid "Show active records"
 msgstr "Aktive Datensätze anzeigen"
 
 msgid "Show bookmarks of filters"
@@ -1019,14 +1059,17 @@
 
 msgid "Working now on the duplicated record(s)."
 msgstr "Sie arbeiten nun an dem/den duplizierten Datensatz/Datensätzen."
 
 msgid "Write Anyway"
 msgstr "Überschreiben"
 
+msgid "XML ID:"
+msgstr "XML-ID:"
+
 msgid "Y"
 msgstr "J"
 
 msgid "Yes"
 msgstr "Ja"
 
 msgid "You have to select one record."
```

### Comparing `tryton-7.2.0/tryton/data/locale/de/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/de/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 msgstr "Den Server mit Hostname:Port angeben."
 
 msgid "disable thread usage"
 msgstr "Threading deaktivieren"
 
 #, python-format
 msgid "Invalid response id (%s) expected %s"
-msgstr ""
+msgstr "Ungültige Antwort-ID (%s) erwartet %s"
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Kann locale %s nicht setzen."
 
 msgid ", "
 msgstr ", "
@@ -80,15 +80,15 @@
 
 msgid "No"
 msgstr "Nein"
 
 msgid "Yes"
 msgstr "Ja"
 
-msgid "Concurrency Exception"
+msgid "Concurrency Warning"
 msgstr "Aktualisierungskonflikt"
 
 msgid "This record has been modified while you were editing it."
 msgstr ""
 "Dieser Datensatz wurde anderweitig geändert, während Sie ihn bearbeitet "
 "haben."
 
@@ -113,14 +113,17 @@
 
 msgid "Close"
 msgstr "Schließen"
 
 msgid "Application Error"
 msgstr "Anwendungsfehler"
 
+msgid "Details"
+msgstr "Details"
+
 msgid "Report Bug"
 msgstr "Fehler melden"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "Überprüfung der URL: %s"
 
@@ -129,37 +132,42 @@
 
 msgid "A new version is available!"
 msgstr "Eine neue Version ist verfügbar!"
 
 msgid "Download"
 msgstr "Herunterladen"
 
+msgid "Concurrency Exception"
+msgstr "Aktualisierungskonflikt"
+
 msgid "Could not get a session."
 msgstr "Die Session-Anforderung ist fehlgeschlagen."
 
-#, fuzzy, python-format
-msgid "Error \"%s\". Try again later."
-msgstr "Zu viele Anfragen. Bitte versuchen Sie es später erneut."
+#, python-format
+msgid "Error: \"%s\". Try again later."
+msgstr "Fehler: \"%s\". Bitte versuchen Sie es später erneut."
 
 msgid "Too many requests. Try again later."
 msgstr "Zu viele Anfragen. Bitte versuchen Sie es später erneut."
 
 msgid "Not Found."
 msgstr "Nicht gefunden."
 
 msgid "Reset forgotten password"
-msgstr ""
+msgstr "Vergessenes Passwort zurücksetzen"
 
 msgid "Send you an email to reset your password."
-msgstr ""
+msgstr "E-Mail zum Zurücksetzen des Passworts senden."
 
 msgid ""
 "A request to reset your password has been sent.\n"
 "Please check your mailbox."
 msgstr ""
+"Eine Anfrage zum Zurücksetzen Ihres Passworts wurde gesendet.\n"
+"Bitte überprüfen Sie Ihr Postfach."
 
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Suche...</i>"
 
@@ -730,14 +738,20 @@
 
 msgid "Model:"
 msgstr "Modell:"
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr "Modul:"
+
+msgid "XML ID:"
+msgstr "XML-ID:"
+
 msgid "Created by:"
 msgstr "Erstellt von:"
 
 msgid "Created at:"
 msgstr "Erstellt am:"
 
 msgid "Last Modified by:"
@@ -1103,28 +1117,25 @@
 
 msgid "Image size too large."
 msgstr "Bild ist zu groß."
 
 msgid "Copy"
 msgstr "Kopieren"
 
-#, fuzzy
 msgid "Copy Row"
-msgstr "URL kopieren"
+msgstr "Zeile kopieren"
 
-#, fuzzy
 msgid "Copy Rows"
-msgstr "URL kopieren"
+msgstr "Zeilen kopieren"
 
 msgid "Copy Column"
-msgstr ""
+msgstr "Spalte kopieren"
 
-#, fuzzy
 msgid "Paste Rows"
-msgstr "Einfügen"
+msgstr "Zeilen Einfügen"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Filter öffnen"
```

### Comparing `tryton-7.2.0/tryton/data/locale/es/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/es/LC_MESSAGES/tryton.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es\n"
 "Language-Team: es <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -78,14 +78,21 @@
 
 msgid "<i>Search...</i>"
 msgstr "<i>Buscar...</i>"
 
 msgid "A new version is available!"
 msgstr "Esta disponible una nueva versión!"
 
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+"Se ha mandado una solicitud para restablecer tu contraseña.\n"
+"Por favor revisa tu buzón de correo."
+
 msgid "A_ttachments..."
 msgstr "Adjun_tos..."
 
 msgid "About..."
 msgstr "Acerca de..."
 
 msgid "Action"
@@ -243,20 +250,32 @@
 
 msgid "Compare: %s"
 msgstr "Comparar: %s"
 
 msgid "Concurrency Exception"
 msgstr "Excepción de concurrencia"
 
+msgid "Concurrency Warning"
+msgstr "Aviso de concurrencia"
+
 msgid "Connect the Tryton server"
 msgstr "Conectar con el servidor Tryton"
 
 msgid "Copy"
 msgstr "Copiar"
 
+msgid "Copy Column"
+msgstr "Copiar columna"
+
+msgid "Copy Row"
+msgstr "Copiar fila"
+
+msgid "Copy Rows"
+msgstr "Copiar filas"
+
 msgid "Copy URL into clipboard"
 msgstr "Copiar la URL al portapapeles"
 
 msgid "Copy _URL..."
 msgstr "Copiar _URL..."
 
 msgid "Copy selected rows"
@@ -321,14 +340,17 @@
 
 msgid "Delete selected record <Del>"
 msgstr "Eliminar registro seleccionado <Supr>"
 
 msgid "Delimiter:"
 msgstr "Separador:"
 
+msgid "Details"
+msgstr "Detalles"
+
 msgid "Detection failed"
 msgstr "Ha fallado la detección"
 
 msgid "Digits"
 msgstr "Dígitos"
 
 msgid "Discard changes"
@@ -384,14 +406,17 @@
 
 msgid "Encoding:"
 msgstr "Codificación:"
 
 msgid "Error"
 msgstr "Error"
 
+msgid "Error: \"%s\". Try again later."
+msgstr "Error: \"%s\" Inténtelo de nuevo más tarde."
+
 msgid "Expand all rows"
 msgstr "Expandir todas las filas"
 
 msgid "Expand row"
 msgstr "Expandir fila"
 
 msgid "Expand/Collapse"
@@ -474,14 +499,17 @@
 
 msgid "Incompatible version of the server."
 msgstr "El cliente no es compatible con la versión del servidor."
 
 msgid "Insert copied rows"
 msgstr "Insertar filas copiadas"
 
+msgid "Invalid response id (%s) expected %s"
+msgstr "ID de respuesta (%s) invàlido. Se esperaba %s"
+
 msgid "Italic"
 msgstr "Cursiva"
 
 msgid "Justify"
 msgstr "Justificar"
 
 msgid "Keyboard Shortcuts..."
@@ -534,14 +562,17 @@
 
 msgid "Mark line for removal"
 msgstr "Marcar para eliminar"
 
 msgid "Model:"
 msgstr "Modelo:"
 
+msgid "Module:"
+msgstr "Modulo:"
+
 msgid "Month"
 msgstr "Mes"
 
 msgid "Move Cursor"
 msgstr "Mover cursor"
 
 msgid "Move down"
@@ -651,14 +682,17 @@
 
 msgid "PDA Mode"
 msgstr "Modo PDA"
 
 msgid "PNG image (*.png)"
 msgstr "Imagen PNG (*.png)"
 
+msgid "Paste Rows"
+msgstr "Pegar filas"
+
 msgid "Paste copied text"
 msgstr "Pegar texto seleccionado"
 
 msgid "Play Sound for Code Scanner"
 msgstr "Activar el sonido del escáner de códigos"
 
 msgid "Pre-validation"
@@ -759,14 +793,17 @@
 
 msgid "Report..."
 msgstr "Informe..."
 
 msgid "Reports"
 msgstr "Informes"
 
+msgid "Reset forgotten password"
+msgstr "Restablecer contraseña"
+
 msgid "Revision"
 msgstr "Revisión"
 
 msgid "Revision:"
 msgstr "Versión:"
 
 msgid "Save"
@@ -852,14 +889,17 @@
 
 msgid "Send"
 msgstr "Enviar"
 
 msgid "Send an e-mail using the record"
 msgstr "Enviar un correo electrónico usando el registro"
 
+msgid "Send you an email to reset your password."
+msgstr "Recibe un correo para restablecer tu contraseña."
+
 msgid "Shortcuts"
 msgstr "Atajos"
 
 msgid "Show active records"
 msgstr "Mostrar registros activos"
 
 msgid "Show bookmarks of filters"
@@ -1016,14 +1056,17 @@
 
 msgid "Working now on the duplicated record(s)."
 msgstr "Ahora está trabajando en el/los registro(s) duplicado(s)."
 
 msgid "Write Anyway"
 msgstr "Guardar de todas formas"
 
+msgid "XML ID:"
+msgstr "ID XML:"
+
 msgid "Y"
 msgstr "A"
 
 msgid "Yes"
 msgstr "Sí"
 
 msgid "You have to select one record."
```

### Comparing `tryton-7.2.0/tryton/data/locale/es/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/es/LC_MESSAGES/tryton.po`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 msgstr "Indica el nombre:puerto del servidor"
 
 msgid "disable thread usage"
 msgstr "desactivar el uso de hilos"
 
 #, python-format
 msgid "Invalid response id (%s) expected %s"
-msgstr ""
+msgstr "ID de respuesta (%s) invàlido. Se esperaba %s"
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "No se ha podido establecer el idioma %s"
 
 msgid ", "
 msgstr ", "
@@ -84,16 +84,16 @@
 
 msgid "No"
 msgstr "No"
 
 msgid "Yes"
 msgstr "Sí"
 
-msgid "Concurrency Exception"
-msgstr "Excepción de concurrencia"
+msgid "Concurrency Warning"
+msgstr "Aviso de concurrencia"
 
 msgid "This record has been modified while you were editing it."
 msgstr "Este registro ha sido modificado mientras lo editaba."
 
 msgid "Cancel saving"
 msgstr "No guardes los cambios"
 
@@ -115,14 +115,17 @@
 
 msgid "Close"
 msgstr "Cerrar"
 
 msgid "Application Error"
 msgstr "Error de aplicación"
 
+msgid "Details"
+msgstr "Detalles"
+
 msgid "Report Bug"
 msgstr "Informar del error"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "URL de comprobación: %s"
 
@@ -131,37 +134,42 @@
 
 msgid "A new version is available!"
 msgstr "Esta disponible una nueva versión!"
 
 msgid "Download"
 msgstr "Descargar"
 
+msgid "Concurrency Exception"
+msgstr "Excepción de concurrencia"
+
 msgid "Could not get a session."
 msgstr "No se ha podido obtener una sesión."
 
-#, fuzzy, python-format
-msgid "Error \"%s\". Try again later."
-msgstr "Demasiadas peticiones. Inténtelo de nuevo más tarde."
+#, python-format
+msgid "Error: \"%s\". Try again later."
+msgstr "Error: \"%s\" Inténtelo de nuevo más tarde."
 
 msgid "Too many requests. Try again later."
 msgstr "Demasiadas peticiones. Inténtelo de nuevo más tarde."
 
 msgid "Not Found."
 msgstr "No se ha encontrado."
 
 msgid "Reset forgotten password"
-msgstr ""
+msgstr "Restablecer contraseña"
 
 msgid "Send you an email to reset your password."
-msgstr ""
+msgstr "Recibe un correo para restablecer tu contraseña."
 
 msgid ""
 "A request to reset your password has been sent.\n"
 "Please check your mailbox."
 msgstr ""
+"Se ha mandado una solicitud para restablecer tu contraseña.\n"
+"Por favor revisa tu buzón de correo."
 
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Buscar...</i>"
 
@@ -727,14 +735,20 @@
 
 msgid "Model:"
 msgstr "Modelo:"
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr "Modulo:"
+
+msgid "XML ID:"
+msgstr "ID XML:"
+
 msgid "Created by:"
 msgstr "Creado por:"
 
 msgid "Created at:"
 msgstr "Creado el:"
 
 msgid "Last Modified by:"
@@ -1100,28 +1114,25 @@
 
 msgid "Image size too large."
 msgstr "El tamaño de la imagen es muy grande."
 
 msgid "Copy"
 msgstr "Copiar"
 
-#, fuzzy
 msgid "Copy Row"
-msgstr "_Copiar la URL"
+msgstr "Copiar fila"
 
-#, fuzzy
 msgid "Copy Rows"
-msgstr "_Copiar la URL"
+msgstr "Copiar filas"
 
 msgid "Copy Column"
-msgstr ""
+msgstr "Copiar columna"
 
-#, fuzzy
 msgid "Paste Rows"
-msgstr "Pegar"
+msgstr "Pegar filas"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Abrir filtros"
```

### Comparing `tryton-7.2.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/es_419/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es_419\n"
 "Language-Team: es_419 <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/es_419/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/es_419/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,16 @@
 
 msgid "No"
 msgstr "No"
 
 msgid "Yes"
 msgstr "Sí"
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "Excepción de concurrencia"
 
 msgid "This record has been modified while you were editing it."
 msgstr "Este registro ha sido modificado mientras lo editaba."
 
 msgid "Cancel saving"
 msgstr ""
@@ -110,14 +111,17 @@
 
 msgid "Close"
 msgstr "Cerrar"
 
 msgid "Application Error"
 msgstr "Error de aplicación"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "Informar del error"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr ""
 
@@ -126,19 +130,22 @@
 
 msgid "A new version is available!"
 msgstr ""
 
 msgid "Download"
 msgstr "Descargar"
 
+msgid "Concurrency Exception"
+msgstr "Excepción de concurrencia"
+
 msgid "Could not get a session."
 msgstr ""
 
 #, fuzzy, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr "Demasiadas peticiones. Inténtalo de nuevo más tarde."
 
 msgid "Too many requests. Try again later."
 msgstr "Demasiadas peticiones. Inténtalo de nuevo más tarde."
 
 msgid "Not Found."
 msgstr ""
@@ -723,14 +730,20 @@
 
 msgid "Model:"
 msgstr ""
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 msgid "Created by:"
 msgstr "Creado por:"
 
 msgid "Created at:"
 msgstr "Fecha de creación:"
 
 msgid "Last Modified by:"
```

### Comparing `tryton-7.2.0/tryton/data/locale/et/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/et/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: et\n"
 "Language-Team: et <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/et/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/et/LC_MESSAGES/tryton.po`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,16 @@
 
 msgid "No"
 msgstr "Ei"
 
 msgid "Yes"
 msgstr "Jah"
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "Konkurentsi erand"
 
 msgid "This record has been modified while you were editing it."
 msgstr "Seda kirjet on muudetud."
 
 msgid "Cancel saving"
 msgstr "Tühista salvestamine"
@@ -110,14 +111,17 @@
 
 msgid "Close"
 msgstr "Sulge"
 
 msgid "Application Error"
 msgstr "Rakenduse viga"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "Teatvita veast"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "Kontrolli URLi: %s"
 
@@ -127,20 +131,23 @@
 
 msgid "A new version is available!"
 msgstr "Uus versioon on saadaval!"
 
 msgid "Download"
 msgstr "Allalaadimine"
 
+msgid "Concurrency Exception"
+msgstr "Konkurentsi erand"
+
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Ei saanud serveriga ühendust"
 
 #, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr ""
 
 msgid "Too many requests. Try again later."
 msgstr ""
 
 #, fuzzy
 msgid "Not Found."
@@ -740,14 +747,20 @@
 
 msgid "Model:"
 msgstr "Mudel:"
 
 msgid "ID:"
 msgstr "ID"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 #, fuzzy
 msgid "Created by:"
 msgstr "Loomise kuupäev"
 
 #, fuzzy
 msgid "Created at:"
 msgstr "Loomise kuupäev"
```

### Comparing `tryton-7.2.0/tryton/data/locale/fa/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/fa/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fa\n"
 "Language-Team: fa <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/fa/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/fa/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,16 @@
 
 msgid "No"
 msgstr "خیر"
 
 msgid "Yes"
 msgstr "بله"
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "همزمانی استثنا"
 
 msgid "This record has been modified while you were editing it."
 msgstr "این پرونده در حالی که شما در حال ویرایش آن بوید، اصلاح شد."
 
 msgid "Cancel saving"
 msgstr "لغو ذخیره کردن"
@@ -110,14 +111,17 @@
 
 msgid "Close"
 msgstr "بستن"
 
 msgid "Application Error"
 msgstr "خطای برنامه"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "گزارش اشکال(باگ)"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "بررسی URL : %s"
 
@@ -127,20 +131,23 @@
 
 msgid "A new version is available!"
 msgstr "نسخه جدید در دسترس می باشد!"
 
 msgid "Download"
 msgstr "دانلود"
 
+msgid "Concurrency Exception"
+msgstr "همزمانی استثنا"
+
 #, fuzzy
 msgid "Could not get a session."
 msgstr "نمی تواند به سرور متصل شود"
 
 #, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr ""
 
 msgid "Too many requests. Try again later."
 msgstr ""
 
 #, fuzzy
 msgid "Not Found."
@@ -745,14 +752,20 @@
 
 msgid "Model:"
 msgstr "مدل:"
 
 msgid "ID:"
 msgstr "شناسه:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 #, fuzzy
 msgid "Created by:"
 msgstr "تاریخ ایجاد"
 
 #, fuzzy
 msgid "Created at:"
 msgstr "تاریخ ایجاد"
```

### Comparing `tryton-7.2.0/tryton/data/locale/fi/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/fi/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 msgid "No"
 msgstr ""
 
 msgid "Yes"
 msgstr ""
 
-msgid "Concurrency Exception"
+msgid "Concurrency Warning"
 msgstr ""
 
 msgid "This record has been modified while you were editing it."
 msgstr ""
 
 msgid "Cancel saving"
 msgstr ""
@@ -111,14 +111,17 @@
 
 msgid "Close"
 msgstr ""
 
 msgid "Application Error"
 msgstr ""
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr ""
 
 #, python-format
 msgid "Check URL: %s"
 msgstr ""
 
@@ -127,19 +130,22 @@
 
 msgid "A new version is available!"
 msgstr ""
 
 msgid "Download"
 msgstr ""
 
+msgid "Concurrency Exception"
+msgstr ""
+
 msgid "Could not get a session."
 msgstr ""
 
 #, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr ""
 
 msgid "Too many requests. Try again later."
 msgstr ""
 
 msgid "Not Found."
 msgstr ""
@@ -720,14 +726,20 @@
 
 msgid "Model:"
 msgstr ""
 
 msgid "ID:"
 msgstr ""
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 msgid "Created by:"
 msgstr ""
 
 msgid "Created at:"
 msgstr ""
 
 msgid "Last Modified by:"
```

### Comparing `tryton-7.2.0/tryton/data/locale/fr/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/fr/LC_MESSAGES/tryton.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -78,14 +78,21 @@
 
 msgid "<i>Search...</i>"
 msgstr "<i>Recherche...</i>"
 
 msgid "A new version is available!"
 msgstr "Un nouvelle version est disponible !"
 
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+"Une demande de réinitialisation de votre mot de passe a été envoyée.\n"
+"Veuillez vérifier votre boîte aux lettres."
+
 msgid "A_ttachments..."
 msgstr "_Pièce jointes..."
 
 msgid "About..."
 msgstr "À Propos..."
 
 msgid "Action"
@@ -243,20 +250,32 @@
 
 msgid "Compare: %s"
 msgstr "Comparer : %s"
 
 msgid "Concurrency Exception"
 msgstr "Erreur d'accès concurrent"
 
+msgid "Concurrency Warning"
+msgstr "Avertissement de concurrence"
+
 msgid "Connect the Tryton server"
 msgstr "Se connecter au serveur Tryton"
 
 msgid "Copy"
 msgstr "Copier"
 
+msgid "Copy Column"
+msgstr "Copier la colonne"
+
+msgid "Copy Row"
+msgstr "Copier la ligne"
+
+msgid "Copy Rows"
+msgstr "Copier les lignes"
+
 msgid "Copy URL into clipboard"
 msgstr "Copier l'URL dans le presse-papiers"
 
 msgid "Copy _URL..."
 msgstr "Copier l'_URL..."
 
 msgid "Copy selected rows"
@@ -321,14 +340,17 @@
 
 msgid "Delete selected record <Del>"
 msgstr "Supprimer l'enregistrement sélectionné<Del>"
 
 msgid "Delimiter:"
 msgstr "Délimiteur :"
 
+msgid "Details"
+msgstr "Détails"
+
 msgid "Detection failed"
 msgstr "La détection a échoué"
 
 msgid "Digits"
 msgstr "Chiffres"
 
 msgid "Discard changes"
@@ -384,16 +406,16 @@
 
 msgid "Encoding:"
 msgstr "Codage :"
 
 msgid "Error"
 msgstr "Erreur"
 
-msgid "Error \"%s\". Try again later."
-msgstr "Erreur « %s ». Réessayez plus tard."
+msgid "Error: \"%s\". Try again later."
+msgstr "Erreur : « %s ». Réessayez plus tard."
 
 msgid "Expand all rows"
 msgstr "Déplier toutes les lignes"
 
 msgid "Expand row"
 msgstr "Déplier la ligne"
 
@@ -540,14 +562,17 @@
 
 msgid "Mark line for removal"
 msgstr "Marquer la ligne pour enlèvement"
 
 msgid "Model:"
 msgstr "Modèle :"
 
+msgid "Module:"
+msgstr "Module :"
+
 msgid "Month"
 msgstr "Mois"
 
 msgid "Move Cursor"
 msgstr "Déplacer le curseur"
 
 msgid "Move down"
@@ -657,14 +682,17 @@
 
 msgid "PDA Mode"
 msgstr "Mode PDA"
 
 msgid "PNG image (*.png)"
 msgstr "image PNG (*.png)"
 
+msgid "Paste Rows"
+msgstr "Coller les lignes"
+
 msgid "Paste copied text"
 msgstr "Coller le texte copié"
 
 msgid "Play Sound for Code Scanner"
 msgstr "Jouer du son pour le scanner de code"
 
 msgid "Pre-validation"
@@ -765,14 +793,17 @@
 
 msgid "Report..."
 msgstr "Rapport..."
 
 msgid "Reports"
 msgstr "Rapports"
 
+msgid "Reset forgotten password"
+msgstr "Réinitialiser le mot de passe oublié"
+
 msgid "Revision"
 msgstr "Révision"
 
 msgid "Revision:"
 msgstr "Révision :"
 
 msgid "Save"
@@ -858,14 +889,17 @@
 
 msgid "Send"
 msgstr "Envoyer"
 
 msgid "Send an e-mail using the record"
 msgstr "Envoyer un e-mail en utilisant l'enregistrement"
 
+msgid "Send you an email to reset your password."
+msgstr "Envoyez-vous un email pour réinitialiser votre mot de passe."
+
 msgid "Shortcuts"
 msgstr "Raccourcis"
 
 msgid "Show active records"
 msgstr "Montrer les enregistrements actifs"
 
 msgid "Show bookmarks of filters"
@@ -1023,14 +1057,17 @@
 
 msgid "Working now on the duplicated record(s)."
 msgstr "Sur les enregistrement(s) dupliqué(s) maintenant."
 
 msgid "Write Anyway"
 msgstr "Écraser"
 
+msgid "XML ID:"
+msgstr "XML ID :"
+
 msgid "Y"
 msgstr "A"
 
 msgid "Yes"
 msgstr "Oui"
 
 msgid "You have to select one record."
```

### Comparing `tryton-7.2.0/tryton/data/locale/fr/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/fr/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,16 @@
 
 msgid "No"
 msgstr "Non"
 
 msgid "Yes"
 msgstr "Oui"
 
-msgid "Concurrency Exception"
-msgstr "Erreur d'accès concurrent"
+msgid "Concurrency Warning"
+msgstr "Avertissement de concurrence"
 
 msgid "This record has been modified while you were editing it."
 msgstr ""
 "Cet enregistrement a été modifié pendant que vous étiez en train de "
 "l'éditer."
 
 msgid "Cancel saving"
@@ -113,14 +113,17 @@
 
 msgid "Close"
 msgstr "Fermer"
 
 msgid "Application Error"
 msgstr "Erreur applicative"
 
+msgid "Details"
+msgstr "Détails"
+
 msgid "Report Bug"
 msgstr "Rapporter un bogue"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "Vérification de l'URL : %s"
 
@@ -129,37 +132,42 @@
 
 msgid "A new version is available!"
 msgstr "Un nouvelle version est disponible !"
 
 msgid "Download"
 msgstr "Télécharger"
 
+msgid "Concurrency Exception"
+msgstr "Erreur d'accès concurrent"
+
 msgid "Could not get a session."
 msgstr "Impossible d'obtenir une session."
 
 #, python-format
-msgid "Error \"%s\". Try again later."
-msgstr "Erreur « %s ». Réessayez plus tard."
+msgid "Error: \"%s\". Try again later."
+msgstr "Erreur : « %s ». Réessayez plus tard."
 
 msgid "Too many requests. Try again later."
 msgstr "Trop de demandes. Réessayez plus tard."
 
 msgid "Not Found."
 msgstr "Pas trouvé."
 
 msgid "Reset forgotten password"
-msgstr ""
+msgstr "Réinitialiser le mot de passe oublié"
 
 msgid "Send you an email to reset your password."
-msgstr ""
+msgstr "Envoyez-vous un email pour réinitialiser votre mot de passe."
 
 msgid ""
 "A request to reset your password has been sent.\n"
 "Please check your mailbox."
 msgstr ""
+"Une demande de réinitialisation de votre mot de passe a été envoyée.\n"
+"Veuillez vérifier votre boîte aux lettres."
 
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Recherche...</i>"
 
@@ -727,14 +735,20 @@
 
 msgid "Model:"
 msgstr "Modèle :"
 
 msgid "ID:"
 msgstr "ID :"
 
+msgid "Module:"
+msgstr "Module :"
+
+msgid "XML ID:"
+msgstr "XML ID :"
+
 msgid "Created by:"
 msgstr "Crée par :"
 
 msgid "Created at:"
 msgstr "Crée le :"
 
 msgid "Last Modified by:"
@@ -1100,28 +1114,25 @@
 
 msgid "Image size too large."
 msgstr "Taille de l'image trop grande."
 
 msgid "Copy"
 msgstr "Copier"
 
-#, fuzzy
 msgid "Copy Row"
-msgstr "_Copier l'URL"
+msgstr "Copier la ligne"
 
-#, fuzzy
 msgid "Copy Rows"
-msgstr "_Copier l'URL"
+msgstr "Copier les lignes"
 
 msgid "Copy Column"
-msgstr ""
+msgstr "Copier la colonne"
 
-#, fuzzy
 msgid "Paste Rows"
-msgstr "Coller"
+msgstr "Coller les lignes"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Ouvrir les filtres"
```

### Comparing `tryton-7.2.0/tryton/data/locale/hu/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/hu/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: hu\n"
 "Language-Team: hu <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/hu/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/hu/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,16 @@
 
 msgid "No"
 msgstr "Nem"
 
 msgid "Yes"
 msgstr "Igen"
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "Egyidejű módosítási hiba"
 
 msgid "This record has been modified while you were editing it."
 msgstr ""
 "Ezt a rekordot valaki más módosította az idő alatt, míg Ön dolgozott rajta."
 
 msgid "Cancel saving"
@@ -113,14 +114,17 @@
 
 msgid "Close"
 msgstr "Bezárás"
 
 msgid "Application Error"
 msgstr "Alkalmazáshiba"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "A hiba jelentése"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr ""
 
@@ -129,20 +133,23 @@
 
 msgid "A new version is available!"
 msgstr "Új verzió elérhető!"
 
 msgid "Download"
 msgstr "Letöltés"
 
+msgid "Concurrency Exception"
+msgstr "Egyidejű módosítási hiba"
+
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Nem sikerült csatlakozni a kiszolgálóhoz."
 
 #, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr ""
 
 msgid "Too many requests. Try again later."
 msgstr ""
 
 #, fuzzy
 msgid "Not Found."
@@ -733,14 +740,20 @@
 
 msgid "Model:"
 msgstr "Elem:"
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 msgid "Created by:"
 msgstr "Létrehozta:"
 
 msgid "Created at:"
 msgstr "Létrehozás dátuma:"
 
 #, fuzzy
```

### Comparing `tryton-7.2.0/tryton/data/locale/id/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/id/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: id\n"
 "Language-Team: id <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/id/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/id/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 msgid "No"
 msgstr "Tidak"
 
 msgid "Yes"
 msgstr "Ya"
 
-msgid "Concurrency Exception"
+msgid "Concurrency Warning"
 msgstr ""
 
 msgid "This record has been modified while you were editing it."
 msgstr "Rekaman ini telah diubah selagi Anda menyuntingnya."
 
 msgid "Cancel saving"
 msgstr "Batalkan penyimpanan"
@@ -107,14 +107,17 @@
 
 msgid "Close"
 msgstr "Tutup"
 
 msgid "Application Error"
 msgstr ""
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "Melaporkan Kesalahan"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "Periksa URL: %s"
 
@@ -123,20 +126,23 @@
 
 msgid "A new version is available!"
 msgstr "Versi baru tersedia!"
 
 msgid "Download"
 msgstr "Unduh"
 
+msgid "Concurrency Exception"
+msgstr ""
+
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Tidak dapat terhubung ke server."
 
 #, fuzzy, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr "Terlalu banyak permintaan. Coba lagi nanti."
 
 msgid "Too many requests. Try again later."
 msgstr "Terlalu banyak permintaan. Coba lagi nanti."
 
 msgid "Not Found."
 msgstr ""
@@ -719,14 +725,20 @@
 
 msgid "Model:"
 msgstr "Model:"
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 msgid "Created by:"
 msgstr "Dibuat oleh:"
 
 msgid "Created at:"
 msgstr "Dibuat pada:"
 
 msgid "Last Modified by:"
```

### Comparing `tryton-7.2.0/tryton/data/locale/it/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/it/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: it\n"
 "Language-Team: it <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/it/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/it/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,16 @@
 
 msgid "No"
 msgstr "No"
 
 msgid "Yes"
 msgstr "Sì"
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "Eccezione di concorrenza"
 
 msgid "This record has been modified while you were editing it."
 msgstr "Questo record è stato modificato mentre lo stavi compilando."
 
 msgid "Cancel saving"
 msgstr "Annulla il salvataggio"
@@ -111,14 +112,17 @@
 
 msgid "Close"
 msgstr "Chiudi"
 
 msgid "Application Error"
 msgstr "Errore dell'applicazione"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "Segnala l'errore"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "Controlla URL: %s"
 
@@ -127,20 +131,23 @@
 
 msgid "A new version is available!"
 msgstr "Una nuova versione è disponibile!"
 
 msgid "Download"
 msgstr "Scarica"
 
+msgid "Concurrency Exception"
+msgstr "Eccezione di concorrenza"
+
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Impossibile connettersi al server."
 
 #, fuzzy, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr "Troppe richieste. Riprovare più tardi."
 
 msgid "Too many requests. Try again later."
 msgstr "Troppe richieste. Riprovare più tardi."
 
 #, fuzzy
 msgid "Not Found."
@@ -735,14 +742,20 @@
 
 msgid "Model:"
 msgstr "Modello:"
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 msgid "Created by:"
 msgstr "Creato da:"
 
 msgid "Created at:"
 msgstr "Creato il:"
 
 #, fuzzy
```

### Comparing `tryton-7.2.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja_JP\n"
 "Language-Team: ja_JP <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/ja_JP/LC_MESSAGES/tryton.po`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/data/locale/lo/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/lo/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: lo\n"
 "Language-Team: lo <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/lo/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/lo/LC_MESSAGES/tryton.po`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,16 @@
 
 msgid "No"
 msgstr ""
 
 msgid "Yes"
 msgstr "ແມ່ນ"
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "ຍົກເວັ້ນການເຂົ້າເຖິງພ້ອມກັນ"
 
 msgid "This record has been modified while you were editing it."
 msgstr ""
 
 msgid "Cancel saving"
 msgstr ""
@@ -114,14 +115,17 @@
 msgid "Close"
 msgstr ""
 
 #, fuzzy
 msgid "Application Error"
 msgstr "ໂປຣແກຣມ ມີຂໍ້ຜິດພາດ!"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "ລາຍງານຂໍ້ຜິດພາດ"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr ""
 
@@ -130,20 +134,23 @@
 
 msgid "A new version is available!"
 msgstr ""
 
 msgid "Download"
 msgstr ""
 
+msgid "Concurrency Exception"
+msgstr "ຍົກເວັ້ນການເຂົ້າເຖິງພ້ອມກັນ"
+
 #, fuzzy
 msgid "Could not get a session."
 msgstr "ບໍ່ສາມາດເຊື່ອມຕໍ່ກັບແມ່ຂ່າຍໄດ້"
 
 #, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr ""
 
 msgid "Too many requests. Try again later."
 msgstr ""
 
 #, fuzzy
 msgid "Not Found."
@@ -757,14 +764,20 @@
 
 msgid "Model:"
 msgstr "ແບບ:"
 
 msgid "ID:"
 msgstr "ເລກລໍາດັບ:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 #, fuzzy
 msgid "Created by:"
 msgstr "ວັນທີສ້າງ"
 
 #, fuzzy
 msgid "Created at:"
 msgstr "ວັນທີສ້າງ"
```

### Comparing `tryton-7.2.0/tryton/data/locale/lt/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/lt/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: lt\n"
 "Language-Team: lt <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "(n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/lt/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/lt/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,16 @@
 
 msgid "No"
 msgstr "Ne"
 
 msgid "Yes"
 msgstr "Taip"
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "Lygiagretaus duomenų rašymo klaida"
 
 msgid "This record has been modified while you were editing it."
 msgstr "Kol jūs taisėte šį įrašą, jis buvo pakeistas."
 
 msgid "Cancel saving"
 msgstr "Nutraukti įrašymą"
@@ -110,14 +111,17 @@
 
 msgid "Close"
 msgstr "Užverti"
 
 msgid "Application Error"
 msgstr "Programos klaida"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "Pranešti apie klaidą"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "Pasirinkti URL: %s"
 
@@ -127,20 +131,23 @@
 
 msgid "A new version is available!"
 msgstr "Yra prieinama nauja versija!"
 
 msgid "Download"
 msgstr "Atsisiųsti"
 
+msgid "Concurrency Exception"
+msgstr "Lygiagretaus duomenų rašymo klaida"
+
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Nepavyko prisijungti prie serverio"
 
 #, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr ""
 
 msgid "Too many requests. Try again later."
 msgstr ""
 
 #, fuzzy
 msgid "Not Found."
@@ -742,14 +749,20 @@
 
 msgid "Model:"
 msgstr "Modelis:"
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 #, fuzzy
 msgid "Created by:"
 msgstr "Sukūręs naudotojas"
 
 #, fuzzy
 msgid "Created at:"
 msgstr "Sukūrimo data"
```

### Comparing `tryton-7.2.0/tryton/data/locale/nl/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/nl/LC_MESSAGES/tryton.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: nl\n"
 "Language-Team: nl <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -78,14 +78,21 @@
 
 msgid "<i>Search...</i>"
 msgstr "<i>Zoek...</i>"
 
 msgid "A new version is available!"
 msgstr "Er is een nieuwe versie beschikbaar!"
 
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+"Een verzoek om uw wachtwoord te resetten is verstuurd.\n"
+"Controller uw mailbox."
+
 msgid "A_ttachments..."
 msgstr "_Bijlagen..."
 
 msgid "About..."
 msgstr "Over..."
 
 msgid "Action"
@@ -243,20 +250,32 @@
 
 msgid "Compare: %s"
 msgstr "Vergelijk: %s"
 
 msgid "Concurrency Exception"
 msgstr "Simultaan gebruik error"
 
+msgid "Concurrency Warning"
+msgstr "Simultaan gebruik waarschuwing"
+
 msgid "Connect the Tryton server"
 msgstr "Verbind met Tryton server"
 
 msgid "Copy"
 msgstr "Kopieer"
 
+msgid "Copy Column"
+msgstr "Kopieer kolom"
+
+msgid "Copy Row"
+msgstr "Kopieer regel"
+
+msgid "Copy Rows"
+msgstr "Kopieer regels"
+
 msgid "Copy URL into clipboard"
 msgstr "Kopieer URL naar het klembord"
 
 msgid "Copy _URL..."
 msgstr "Kopieer _URL..."
 
 msgid "Copy selected rows"
@@ -321,14 +340,17 @@
 
 msgid "Delete selected record <Del>"
 msgstr "Geselecteerde record verwijderen <Del>"
 
 msgid "Delimiter:"
 msgstr "Scheidingsteken:"
 
+msgid "Details"
+msgstr "Details"
+
 msgid "Detection failed"
 msgstr "Detecteren faalde"
 
 msgid "Digits"
 msgstr "Decimalen"
 
 msgid "Discard changes"
@@ -384,16 +406,16 @@
 
 msgid "Encoding:"
 msgstr "Codering:"
 
 msgid "Error"
 msgstr "Fout"
 
-msgid "Error \"%s\". Try again later."
-msgstr "Te veel verzoeken\"%s\". Probeer het later nog eens."
+msgid "Error: \"%s\". Try again later."
+msgstr "Error: \"%s\". Probeer het later nog eens."
 
 msgid "Expand all rows"
 msgstr "Alle rijen uitvouwen"
 
 msgid "Expand row"
 msgstr "Rij uitvouwen"
 
@@ -477,14 +499,17 @@
 
 msgid "Incompatible version of the server."
 msgstr "Onjuiste versie van de server."
 
 msgid "Insert copied rows"
 msgstr "Gekopieerde regels invoegen"
 
+msgid "Invalid response id (%s) expected %s"
+msgstr "Ongeldige reactie id (%s) verwacht werd %s"
+
 msgid "Italic"
 msgstr "Cursief"
 
 msgid "Justify"
 msgstr "Uitvullen"
 
 msgid "Keyboard Shortcuts..."
@@ -537,14 +562,17 @@
 
 msgid "Mark line for removal"
 msgstr "Markeer regel voor verwijderen"
 
 msgid "Model:"
 msgstr "Model:"
 
+msgid "Module:"
+msgstr "Module:"
+
 msgid "Month"
 msgstr "Maand"
 
 msgid "Move Cursor"
 msgstr "Beweeg cursor"
 
 msgid "Move down"
@@ -654,14 +682,17 @@
 
 msgid "PDA Mode"
 msgstr "PDA-modus"
 
 msgid "PNG image (*.png)"
 msgstr "PNG afbeelding (*.png)"
 
+msgid "Paste Rows"
+msgstr "Plak regels"
+
 msgid "Paste copied text"
 msgstr "Plak geselecteerde tekst"
 
 msgid "Play Sound for Code Scanner"
 msgstr "Geluid afspelen bij barcode scanner"
 
 msgid "Pre-validation"
@@ -762,14 +793,17 @@
 
 msgid "Report..."
 msgstr "Rapport..."
 
 msgid "Reports"
 msgstr "Rapporten"
 
+msgid "Reset forgotten password"
+msgstr "Reset vergeten wachtwoord"
+
 msgid "Revision"
 msgstr "Revisie"
 
 msgid "Revision:"
 msgstr "Revisie:"
 
 msgid "Save"
@@ -855,14 +889,17 @@
 
 msgid "Send"
 msgstr "Verzenden"
 
 msgid "Send an e-mail using the record"
 msgstr "Stuur een e-mail met behulp van het record"
 
+msgid "Send you an email to reset your password."
+msgstr "Stuurt u een email om het wachtwoord te resetten."
+
 msgid "Shortcuts"
 msgstr "Snelkoppelingen"
 
 msgid "Show active records"
 msgstr "Geef actieve records weer"
 
 msgid "Show bookmarks of filters"
@@ -1019,14 +1056,17 @@
 
 msgid "Working now on the duplicated record(s)."
 msgstr "Aan het werk op het(de) gekopieerde record(s)."
 
 msgid "Write Anyway"
 msgstr "Overschrijven"
 
+msgid "XML ID:"
+msgstr "XML id:"
+
 msgid "Y"
 msgstr "J"
 
 msgid "Yes"
 msgstr "Ja"
 
 msgid "You have to select one record."
```

### Comparing `tryton-7.2.0/tryton/data/locale/nl/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/nl/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 msgstr "specificeer de hostnaam:poort"
 
 msgid "disable thread usage"
 msgstr "schakel gebruik van threads uit"
 
 #, python-format
 msgid "Invalid response id (%s) expected %s"
-msgstr ""
+msgstr "Ongeldige reactie id (%s) verwacht werd %s"
 
 #, python-format
 msgid "Unable to set locale %s"
 msgstr "Kan omgeving %s niet instellen"
 
 msgid ", "
 msgstr ", "
@@ -80,16 +80,16 @@
 
 msgid "No"
 msgstr "Nee"
 
 msgid "Yes"
 msgstr "Ja"
 
-msgid "Concurrency Exception"
-msgstr "Simultaan gebruik error"
+msgid "Concurrency Warning"
+msgstr "Simultaan gebruik waarschuwing"
 
 msgid "This record has been modified while you were editing it."
 msgstr "Dit record werd gewijzigd terwijl u het aan het bewerken was."
 
 msgid "Cancel saving"
 msgstr "Annuleer opslaan"
 
@@ -111,14 +111,17 @@
 
 msgid "Close"
 msgstr "Sluiten"
 
 msgid "Application Error"
 msgstr "Applicatiefout"
 
+msgid "Details"
+msgstr "Details"
+
 msgid "Report Bug"
 msgstr "Programmafout melden"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "Controleer URL: %s"
 
@@ -127,37 +130,42 @@
 
 msgid "A new version is available!"
 msgstr "Er is een nieuwe versie beschikbaar!"
 
 msgid "Download"
 msgstr "Download"
 
+msgid "Concurrency Exception"
+msgstr "Simultaan gebruik error"
+
 msgid "Could not get a session."
 msgstr "Kan geen sessie krijgen."
 
 #, python-format
-msgid "Error \"%s\". Try again later."
-msgstr "Te veel verzoeken\"%s\". Probeer het later nog eens."
+msgid "Error: \"%s\". Try again later."
+msgstr "Error: \"%s\". Probeer het later nog eens."
 
 msgid "Too many requests. Try again later."
 msgstr "Te veel verzoeken. Probeer het later nog eens."
 
 msgid "Not Found."
 msgstr "Niet gevonden."
 
 msgid "Reset forgotten password"
-msgstr ""
+msgstr "Reset vergeten wachtwoord"
 
 msgid "Send you an email to reset your password."
-msgstr ""
+msgstr "Stuurt u een email om het wachtwoord te resetten."
 
 msgid ""
 "A request to reset your password has been sent.\n"
 "Please check your mailbox."
 msgstr ""
+"Een verzoek om uw wachtwoord te resetten is verstuurd.\n"
+"Controller uw mailbox."
 
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
 msgstr "<i>Zoek...</i>"
 
@@ -723,14 +731,20 @@
 
 msgid "Model:"
 msgstr "Model:"
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr "Module:"
+
+msgid "XML ID:"
+msgstr "XML id:"
+
 msgid "Created by:"
 msgstr "Aangemaakt door:"
 
 msgid "Created at:"
 msgstr "Aanmaakdatum:"
 
 msgid "Last Modified by:"
@@ -1096,28 +1110,25 @@
 
 msgid "Image size too large."
 msgstr "Afbeelding te groot."
 
 msgid "Copy"
 msgstr "Kopieer"
 
-#, fuzzy
 msgid "Copy Row"
-msgstr "_Kopieer URL"
+msgstr "Kopieer regel"
 
-#, fuzzy
 msgid "Copy Rows"
-msgstr "_Kopieer URL"
+msgstr "Kopieer regels"
 
 msgid "Copy Column"
-msgstr ""
+msgstr "Kopieer kolom"
 
-#, fuzzy
 msgid "Paste Rows"
-msgstr "Plakken"
+msgstr "Plak regels"
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
 msgstr "Open filters"
```

### Comparing `tryton-7.2.0/tryton/data/locale/pl/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/pl/LC_MESSAGES/tryton.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: pl\n"
 "Language-Team: pl <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
@@ -16,14 +16,17 @@
 
 msgid "\"%s\" is not valid according to its domain."
 msgstr "\"%s\" jest nieprawidłowy pod względem swojej domeny."
 
 msgid "\"%s\" is required."
 msgstr "\"%s\" jest wymagany."
 
+msgid "#ERROR"
+msgstr "#BŁĄD"
+
 msgid "%d record imported."
 msgstr "Rekord %d został zaimportowany."
 
 msgid "%d record saved."
 msgstr "%d rekord został zapisany."
 
 msgid "%d records imported."
@@ -40,14 +43,17 @@
 
 msgid "%s (string)"
 msgstr "%s (string)"
 
 msgid "%s%%"
 msgstr "%s%%"
 
+msgid "%s/Record Name"
+msgstr "%s/Nazwa rekordu"
+
 msgid ", "
 msgstr ", "
 
 msgid ",..."
 msgstr ",..."
 
 msgid ".."
@@ -73,14 +79,21 @@
 
 msgid "<i>Search...</i>"
 msgstr "<i>Szukaj...</i>"
 
 msgid "A new version is available!"
 msgstr "Nowa wersja jest dostępna!"
 
+msgid ""
+"A request to reset your password has been sent.\n"
+"Please check your mailbox."
+msgstr ""
+"Żądanie zresetowania hasła zostało wysłane.\n"
+"Sprawdź skrzynkę pocztową."
+
 msgid "A_ttachments..."
 msgstr "Załączniki..."
 
 msgid "About..."
 msgstr "O programie..."
 
 msgid "Action"
@@ -94,14 +107,17 @@
 
 msgid "Add a note to the record"
 msgstr "Dodaj notatkę do rekordu"
 
 msgid "Add an attachment to the record"
 msgstr "Dodaj załącznik do rekordu"
 
+msgid "Add and New"
+msgstr "Dodaj i utwórz nowy"
+
 msgid "Add existing record"
 msgstr "Dodaj istniejący rekord"
 
 msgid "Add field names"
 msgstr "Dodaj nazwy pól"
 
 msgid "Add new profile"
@@ -130,14 +146,17 @@
 
 msgid "Application Error"
 msgstr "Błąd aplikacji"
 
 msgid "Application Shortcuts"
 msgstr "Skróty aplikacji"
 
+msgid "Apply changes"
+msgstr "Zatwierdź zmiany"
+
 msgid "Are you sure to remove this record?"
 msgstr "Czy na pewno usunąć wybrany rekord?"
 
 msgid "Are you sure to remove those records?"
 msgstr "Czy na pewno usunąć wybrane rekordy?"
 
 msgid "Attachment (%s)"
@@ -155,15 +174,15 @@
 msgid "Bcc:"
 msgstr "UDW:"
 
 msgid "Body"
 msgstr "Treść"
 
 msgid "Bold"
-msgstr "Pogrubiony"
+msgstr "Pogrubienie"
 
 msgid "Bookmark Name:"
 msgstr "Dodaj nazwę zakładek:"
 
 msgid "Bookmark this filter"
 msgstr "Dodaj filtr do zakładek"
 
@@ -211,14 +230,20 @@
 
 msgid "Close"
 msgstr "Zamknij"
 
 msgid "Close Tab"
 msgstr "Zamknij kartę"
 
+msgid "Code"
+msgstr "Kod"
+
+msgid "Code Scanner"
+msgstr "Skaner kodów"
+
 msgid "Collapse all rows"
 msgstr "Zwiń wszystkie wiersze"
 
 msgid "Collapse row"
 msgstr "Zwiń wiersz"
 
 msgid "Compare"
@@ -226,31 +251,52 @@
 
 msgid "Compare: %s"
 msgstr "Porównaj: %s"
 
 msgid "Concurrency Exception"
 msgstr "Wyjątek równoczesnego zapisu danych"
 
+msgid "Concurrency Warning"
+msgstr "Ostrzeżenie o równoczesnym zapisie danych"
+
 msgid "Connect the Tryton server"
 msgstr "Połącz z serwerem Tryton"
 
 msgid "Copy"
 msgstr "Kopiuj"
 
+msgid "Copy Column"
+msgstr "Skopiuj kolumnę"
+
+msgid "Copy Row"
+msgstr "Skopiuj wiersz"
+
+msgid "Copy Rows"
+msgstr "Skopiuj wiersze"
+
 msgid "Copy URL into clipboard"
 msgstr "Skopiuj adres URL do schowka"
 
 msgid "Copy _URL..."
 msgstr "Skopiuj adres URL..."
 
+msgid "Copy selected rows"
+msgstr "Skopiuj wybrane wiersze"
+
 msgid "Copy selected text"
 msgstr "Skopiuj zaznaczony tekst"
 
 msgid "Could not connect to the server."
-msgstr "Nie można połączyć się z serwerem."
+msgstr "Brak dostępu do serwera."
+
+msgid "Could not get a session."
+msgstr "Nie udało się ustanowić sesji."
+
+msgid "Create \"%s\"..."
+msgstr "Utwórz \"%s\"..."
 
 msgid "Create a new record"
 msgstr "Utwórz nowy rekord"
 
 msgid "Create a new record <F3>"
 msgstr "Utwórz nowy rekord <F3>"
 
@@ -262,26 +308,32 @@
 
 msgid "Created at"
 msgstr "Data utworzenia"
 
 msgid "Created at:"
 msgstr "Data utworzenia:"
 
+msgid "Created by"
+msgstr "Utworzył"
+
 msgid "Created by:"
 msgstr "Utworzył:"
 
 msgid "Cut selected text"
 msgstr "Wytnij zaznaczony tekst"
 
 msgid "Database:"
 msgstr "Baza danych:"
 
 msgid "Date Format"
 msgstr "Format daty"
 
+msgid "Day"
+msgstr "Dzień"
+
 msgid "Default"
 msgstr "Domyślnie"
 
 msgid "Delete"
 msgstr "Usuń"
 
 msgid "Delete selected record"
@@ -289,29 +341,41 @@
 
 msgid "Delete selected record <Del>"
 msgstr "Usuń zaznaczony rekord <Del>"
 
 msgid "Delimiter:"
 msgstr "Separator:"
 
+msgid "Details"
+msgstr "Szczegóły"
+
+msgid "Detection failed"
+msgstr "Wykrycie nie powiodło się"
+
 msgid "Digits"
 msgstr "Cyfry"
 
+msgid "Discard changes"
+msgstr "Odrzuć zmiany"
+
 msgid "Display format"
 msgstr "Wyświetl format"
 
 msgid "Displayed date format"
 msgstr "Wyświetlany format daty"
 
 msgid "Displayed value"
 msgstr "Wyświetlana wartość"
 
 msgid "Do you want to proceed?"
 msgstr "Czy chcesz kontynuować?"
 
+msgid "Documentation..."
+msgstr "Dokumentacja..."
+
 msgid "Download"
 msgstr "Pobierz"
 
 msgid "E-Mail..."
 msgstr "E-mail..."
 
 msgid "E-mail %s"
@@ -331,32 +395,41 @@
 
 msgid "Edited at"
 msgstr "Data modyfikacji"
 
 msgid "Edited by"
 msgstr "Zmodyfikował"
 
+msgid "Edition"
+msgstr "Edycja"
+
 msgid "Edition Shortcuts"
 msgstr "Skróty edycji"
 
 msgid "Encoding:"
 msgstr "Kodowanie:"
 
 msgid "Error"
 msgstr "Błąd"
 
+msgid "Error: \"%s\". Try again later."
+msgstr "Błąd: \"%s\". Spróbuj ponownie później."
+
 msgid "Expand all rows"
 msgstr "Rozwiń wszystkie wiersze"
 
 msgid "Expand row"
 msgstr "Rozwiń wiersz"
 
 msgid "Expand/Collapse"
 msgstr "Rozwiń/Zwiń"
 
+msgid "Export failed"
+msgstr "Eksport nie powiódł się"
+
 msgid "False"
 msgstr "Nie"
 
 msgid "Favorites"
 msgstr "Ulubione"
 
 msgid "Fetching databases list"
@@ -364,14 +437,17 @@
 
 msgid "Field name"
 msgstr "Nazwa pola"
 
 msgid "File to Import:"
 msgstr "Plik do zaimportowania:"
 
+msgid "Files"
+msgstr "Pliki"
+
 msgid "Find"
 msgstr "Znajdź"
 
 msgid "Foreground Color"
 msgstr "Kolor czcionki"
 
 msgid "Form"
@@ -415,26 +491,41 @@
 
 msgid "Image size too large."
 msgstr "Za duży rozmiar obrazka."
 
 msgid "Images"
 msgstr "Obrazki"
 
+msgid "Import failed"
+msgstr "Import nie powiódł się"
+
 msgid "Incompatible version of the server."
-msgstr "Niewłaściwa wersja serwera."
+msgstr "Niekompatybilna wersja serwera."
+
+msgid "Insert copied rows"
+msgstr "Wstaw skopiowane wiersze"
+
+msgid "Invalid response id (%s) expected %s"
+msgstr "Nieprawidłowy identyfikator odpowiedzi (%s). Oczekiwano %s"
 
 msgid "Italic"
 msgstr "Kursywa"
 
 msgid "Justify"
 msgstr "Wyjustowanie"
 
 msgid "Keyboard Shortcuts..."
 msgstr "Skróty klawiszowe..."
 
+msgid "Last Modified at:"
+msgstr "Ostatnio zmodyfikowano:"
+
+msgid "Last Modified by:"
+msgstr "Zmodyfikował:"
+
 msgid "Launch action"
 msgstr "Uruchom akcję"
 
 msgid "Limit"
 msgstr "Limit"
 
 msgid "Limit:"
@@ -472,14 +563,20 @@
 
 msgid "Mark line for removal"
 msgstr "Zaznacz wiersz do usunięcia"
 
 msgid "Model:"
 msgstr "Model:"
 
+msgid "Module:"
+msgstr "Moduł:"
+
+msgid "Month"
+msgstr "Miesiąc"
+
 msgid "Move Cursor"
 msgstr "Przesuń kursor"
 
 msgid "Move down"
 msgstr "Przesuń w dół"
 
 msgid "Move down of one page"
@@ -532,14 +629,17 @@
 
 msgid "No other language available."
 msgstr "Brak innych języków."
 
 msgid "No result found."
 msgstr "Nie znaleziono wyniku."
 
+msgid "Not Found."
+msgstr "Nie znaleziono."
+
 msgid "Note (%d/%d)"
 msgstr "Notatka (%d/%d)"
 
 msgid "Notes (%s)"
 msgstr "Notatki (%s)"
 
 msgid "Notes..."
@@ -583,29 +683,38 @@
 
 msgid "PDA Mode"
 msgstr "Tryb PDA"
 
 msgid "PNG image (*.png)"
 msgstr "Obrazek w formacie PNG (*.png)"
 
+msgid "Paste Rows"
+msgstr "Wklej wiersze"
+
 msgid "Paste copied text"
 msgstr "Wklej zaznaczony tekst"
 
+msgid "Play Sound for Code Scanner"
+msgstr "Odtwórz dźwięk dla skanera kodów"
+
 msgid "Pre-validation"
 msgstr "Wstępna walidacja"
 
 msgid "Preference"
 msgstr "Preferencje"
 
 msgid "Preferences"
 msgstr "Preferencje"
 
 msgid "Preferences..."
 msgstr "Preferencje..."
 
+msgid "Preview"
+msgstr "Podgląd"
+
 msgid "Previous"
 msgstr "Poprzedni"
 
 msgid "Previous Record"
 msgstr "Poprzedni rekord"
 
 msgid "Previous entry"
@@ -661,14 +770,17 @@
 
 msgid "Remove \"%s\""
 msgstr "Usuń \"%s\""
 
 msgid "Remove <Del>"
 msgstr "Usuń <Del>"
 
+msgid "Remove File"
+msgstr "Usuń plik"
+
 msgid "Remove selected profile"
 msgstr "Usuń wybrany profil"
 
 msgid "Remove selected record"
 msgstr "Usuń wybrany rekord"
 
 msgid "Remove this bookmark"
@@ -682,14 +794,17 @@
 
 msgid "Report..."
 msgstr "Utwórz raport..."
 
 msgid "Reports"
 msgstr "Raporty"
 
+msgid "Reset forgotten password"
+msgstr "Zresetuj zapomniane hasło"
+
 msgid "Revision"
 msgstr "Rewizja"
 
 msgid "Revision:"
 msgstr "Rewizja:"
 
 msgid "Save"
@@ -703,20 +818,26 @@
 
 msgid "Save Column Width"
 msgstr "Zapisz szerokość kolumny"
 
 msgid "Save Tree State"
 msgstr "Zapamiętaj stan drzewa"
 
+msgid "Save and New"
+msgstr "Zapisz i utwórz nowy"
+
 msgid "Save this record"
 msgstr "Zapisz rekord"
 
 msgid "Save your current version"
 msgstr "Zapisz swoją bieżącą wersję"
 
+msgid "Scan"
+msgstr "Skanuj"
+
 msgid "Search"
 msgstr "Szukaj"
 
 msgid "Search %s"
 msgstr "Szukaj %s"
 
 msgid "Search Limit Settings"
@@ -733,14 +854,17 @@
 
 msgid "See the modified version"
 msgstr "Zobacz zmienioną wersję"
 
 msgid "Select"
 msgstr "Wybierz"
 
+msgid "Select File"
+msgstr "Wybierz plik"
+
 msgid "Select a color"
 msgstr "Wybierz kolor"
 
 msgid "Select a revision"
 msgstr "Wybierz rewizję"
 
 msgid "Select all"
@@ -766,14 +890,17 @@
 
 msgid "Send"
 msgstr "Wyślij"
 
 msgid "Send an e-mail using the record"
 msgstr "Wyślij e-mail używając rekordu"
 
+msgid "Send you an email to reset your password."
+msgstr "Wyślij wiadomość, aby zresetować hasło."
+
 msgid "Shortcuts"
 msgstr "Skróty"
 
 msgid "Show active records"
 msgstr "Pokaż aktywne rekordy"
 
 msgid "Show bookmarks of filters"
@@ -880,19 +1007,22 @@
 msgid "Unable to set view tree state"
 msgstr "Brak możliwości ustawienia stanu widoku drzewa"
 
 msgid "Undelete selected record <Ins>"
 msgstr "Przywróć zaznaczony rekord <Ins>"
 
 msgid "Underline"
-msgstr "Podkreślenie"
+msgstr "Podkreśl"
 
 msgid "Unknown"
 msgstr "Nieznany"
 
+msgid "Unknown column header \"%s\""
+msgstr "Nieznany nagłówek kolumny \"%s\""
+
 msgid "Unmark line for deletion"
 msgstr "Odznacz wiersz do usunięcia"
 
 msgid "Unselect all"
 msgstr "Odznacz wszystko"
 
 msgid "Use locale format"
@@ -903,14 +1033,17 @@
 
 msgid "Username:"
 msgstr "Użytkownik:"
 
 msgid "Value"
 msgstr "Wartość"
 
+msgid "View Logs..."
+msgstr "Przeglądaj logi..."
+
 msgid "View _Logs..."
 msgstr "Przeglądaj dziennik..."
 
 msgid "Week"
 msgstr "Tydzień"
 
 msgid "What is the name of this export?"
@@ -924,14 +1057,17 @@
 
 msgid "Working now on the duplicated record(s)."
 msgstr "Pracujesz na zduplikowanym(ch) rekordzie(ch)."
 
 msgid "Write Anyway"
 msgstr "Zapisz"
 
+msgid "XML ID:"
+msgstr "XML ID:"
+
 msgid "Y"
 msgstr "R"
 
 msgid "Yes"
 msgstr "Tak"
 
 msgid "You have to select one record."
@@ -1029,14 +1165,17 @@
 
 msgid "d"
 msgstr "d"
 
 msgid "development mode"
 msgstr "tryb dewelopera"
 
+msgid "disable thread usage"
+msgstr "wyłącz użycie wątku"
+
 msgid "go back"
 msgstr "wstecz"
 
 msgid "go forward"
 msgstr "dalej"
 
 msgid "h"
@@ -1059,14 +1198,17 @@
 
 msgid "s"
 msgstr "s"
 
 msgid "specify alternate config file"
 msgstr "podaj alternatywny plik konfiguracji"
 
+msgid "specify the file used to output logging information"
+msgstr "określ plik używany do wysyłania informacji rejestrujących"
+
 msgid "specify the log level: DEBUG, INFO, WARNING, ERROR, CRITICAL"
 msgstr "podaj poziom rejestrowania: DEBUG, INFO, WARNING, ERROR, CRITICAL"
 
 msgid "specify the login user"
 msgstr "podaj login użytkownika"
 
 msgid "specify the server hostname:port"
```

### Comparing `tryton-7.2.0/tryton/data/locale/pl/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/pt/LC_MESSAGES/tryton.po`

 * *Files 19% similar despite different names*

```diff
@@ -2,152 +2,162 @@
 # Copyright (C) 2016 Tryton
 # This file is distributed under the same license as the tryton project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgid "specify alternate config file"
-msgstr "podaj alternatywny plik konfiguracji"
+msgstr "especificar arquivo de configuração alternativo"
 
 msgid "development mode"
-msgstr "tryb dewelopera"
+msgstr "modo de desenvolvimento"
 
 msgid "logging everything at INFO level"
-msgstr "rejestrowanie wszystkiego na poziomie INFO"
+msgstr "Registrar (log) tudo com nível INFO"
 
 msgid "specify the log level: DEBUG, INFO, WARNING, ERROR, CRITICAL"
-msgstr "podaj poziom rejestrowania: DEBUG, INFO, WARNING, ERROR, CRITICAL"
+msgstr ""
+"Especifique o nível de registro (log level): DEBUG, INFO, WARNING, ERROR, "
+"CRITICAL"
 
 msgid "specify the file used to output logging information"
 msgstr ""
 
 msgid "specify the login user"
-msgstr "podaj login użytkownika"
+msgstr "Especifique o nome do usuário"
 
 msgid "specify the server hostname:port"
-msgstr "podaj nazwę:port serwera"
+msgstr "Especifique o servidor hostname:porta"
 
 msgid "disable thread usage"
 msgstr ""
 
 #, python-format
 msgid "Invalid response id (%s) expected %s"
 msgstr ""
 
 #, python-format
 msgid "Unable to set locale %s"
-msgstr "Nie można ustawić lokalizacji %s"
+msgstr "Não foi possível definir as configurações regionais %s"
 
 msgid ", "
 msgstr ", "
 
 msgid ",..."
-msgstr ",..."
+msgstr ""
 
 #, python-format
 msgid "%s (%s)"
 msgstr "%s (%s)"
 
 msgid "Select your action"
-msgstr "Wybierz akcję"
+msgstr "Selecione sua ação"
 
 msgid "No action defined."
-msgstr "Brak zdefiniowanej akcji."
+msgstr "Nenhuma ação definida."
 
 msgid "By: "
-msgstr "Przez: "
+msgstr "Por: "
 
 msgid "Selection"
-msgstr "Zaznaczenie"
+msgstr "Seleção"
 
 msgid "Cancel"
-msgstr "Anuluj"
+msgstr "Cancelar"
 
 msgid "OK"
 msgstr "OK"
 
 msgid "Your selection:"
-msgstr "Twoje zaznaczenie:"
+msgstr "Sua seleção:"
 
 msgid "Save As..."
-msgstr "Zapisz jako..."
+msgstr "Salvar como..."
 
 msgid "Do you want to proceed?"
-msgstr "Czy chcesz kontynuować?"
+msgstr "Você deseja prosseguir?"
 
 msgid "Always ignore this warning."
-msgstr "Zawsze ignoruj takie ostrzeżenie."
+msgstr "Sempre ignorar este aviso."
 
 msgid "No"
-msgstr "Nie"
+msgstr "Não"
 
 msgid "Yes"
-msgstr "Tak"
+msgstr "Sim"
 
-msgid "Concurrency Exception"
-msgstr "Wyjątek równoczesnego zapisu danych"
+#, fuzzy
+msgid "Concurrency Warning"
+msgstr "Exceção de concorrência"
 
 msgid "This record has been modified while you were editing it."
-msgstr "Ten rekord został zmodyfikowany w trakcie twojej edycji."
+msgstr "Este registro foi modificado enquanto você o editava."
 
 msgid "Cancel saving"
-msgstr "Anuluj zapis"
+msgstr "Cancelar"
 
 msgid "Compare"
-msgstr "Porównaj"
+msgstr "Comparar"
 
 msgid "See the modified version"
-msgstr "Zobacz zmienioną wersję"
+msgstr "Ver versão modificada"
 
 msgid "Write Anyway"
-msgstr "Zapisz"
+msgstr "Gravar mesmo assim"
 
 msgid "Save your current version"
-msgstr "Zapisz swoją bieżącą wersję"
+msgstr "Gravar sua versão atual"
 
-#, python-format
+#, fuzzy, python-format
 msgid "Compare: %s"
-msgstr "Porównaj: %s"
+msgstr "Comparar: %s"
 
 msgid "Close"
-msgstr "Zamknij"
+msgstr "Fechar"
 
 msgid "Application Error"
-msgstr "Błąd aplikacji"
+msgstr "Erro no programa"
+
+msgid "Details"
+msgstr ""
 
 msgid "Report Bug"
-msgstr "Zgłoś błąd"
+msgstr "Reportar erro (bug)"
 
 #, python-format
 msgid "Check URL: %s"
-msgstr "Sprawdź URL: %s"
+msgstr "Verificar URL: %s"
 
+#, fuzzy
 msgid "Unable to check for new version."
-msgstr "Nie można sprawdzić dostępności nowej wersji."
+msgstr "Não foi possível verificar por nova versão"
 
 msgid "A new version is available!"
-msgstr "Nowa wersja jest dostępna!"
+msgstr "Nova versão disponível!"
 
 msgid "Download"
-msgstr "Pobierz"
+msgstr "Baixar"
+
+msgid "Concurrency Exception"
+msgstr "Exceção de concorrência"
 
 #, fuzzy
 msgid "Could not get a session."
-msgstr "Nie można połączyć się z serwerem."
+msgstr "Não foi possível se conectar ao servidor"
 
-#, fuzzy, python-format
-msgid "Error \"%s\". Try again later."
-msgstr "Za dużo połączeń. Spróbuj później."
+#, python-format
+msgid "Error: \"%s\". Try again later."
+msgstr ""
 
 msgid "Too many requests. Try again later."
-msgstr "Za dużo połączeń. Spróbuj później."
+msgstr ""
 
 #, fuzzy
 msgid "Not Found."
-msgstr "Nie znaleziono wyniku."
+msgstr "Nenhum resultado encontrado."
 
 msgid "Reset forgotten password"
 msgstr ""
 
 msgid "Send you an email to reset your password."
 msgstr ""
 
@@ -156,1096 +166,1123 @@
 "Please check your mailbox."
 msgstr ""
 
 msgid "..."
 msgstr "..."
 
 msgid "<i>Search...</i>"
-msgstr "<i>Szukaj...</i>"
+msgstr "<i>Buscar...</i>"
 
 msgid "<i>Create...</i>"
-msgstr "<i>Utwórz...</i>"
+msgstr "<i>Criar...</i>"
 
 #, fuzzy, python-format
 msgid "Create \"%s\"..."
-msgstr "Utwórz „%s”..."
+msgstr "Crie \"%s\"..."
 
 msgid "Value"
-msgstr "Wartość"
+msgstr "Valor"
 
 msgid "Displayed value"
-msgstr "Wyświetlana wartość"
+msgstr "Valor exibido"
 
 msgid "Format"
-msgstr "Format"
+msgstr "Formato"
 
 msgid "Display format"
-msgstr "Wyświetl format"
+msgstr "Formato de exibição"
 
 msgid "Open the calendar"
-msgstr "Otwórz kalendarz"
+msgstr "Abrir o calendário"
 
 msgid "Date Format"
-msgstr "Format daty"
+msgstr "Formato de Data"
 
 msgid "Displayed date format"
-msgstr "Wyświetlany format daty"
+msgstr "Formato de data exibido"
 
 msgid "y"
-msgstr "t"
+msgstr "s"
 
 msgid "True"
-msgstr "Tak"
+msgstr "Verdadeiro"
 
 msgid "t"
-msgstr "p"
+msgstr "v"
 
 msgid "False"
-msgstr "Nie"
+msgstr "Falso"
 
 msgid "Digits"
-msgstr "Cyfry"
+msgstr ""
 
 msgid "The number of decimal"
-msgstr "Liczba miejsc dziesiętnych"
+msgstr ""
 
+#, fuzzy
 msgid "Template"
-msgstr "Szablon"
+msgstr "Relacionar"
 
 msgid "Edit..."
-msgstr "Edycja..."
+msgstr "Editar..."
 
 #, fuzzy
 msgid "View Logs..."
-msgstr "Przeglądaj dziennik..."
+msgstr "Ver _Logs..."
 
 msgid "Attachments..."
-msgstr "Załączniki..."
+msgstr "Anexos..."
 
 msgid "Notes..."
-msgstr "Notatki..."
+msgstr "Notas..."
 
 msgid "Actions..."
-msgstr "Akcje..."
+msgstr "Ações..."
 
 msgid "Relate..."
-msgstr "Otwórz..."
+msgstr "Relacionado..."
 
 msgid "Report..."
-msgstr "Utwórz raport..."
+msgstr "Relatório..."
 
 msgid "Print..."
-msgstr "Wydrukuj..."
+msgstr "Imprimir..."
 
 msgid "E-Mail..."
 msgstr "E-mail..."
 
 msgid "Bold"
-msgstr "Pogrubiony"
+msgstr ""
 
 msgid "Italic"
-msgstr "Kursywa"
+msgstr ""
 
 msgid "Underline"
-msgstr "Podkreślenie"
+msgstr ""
 
 msgid "Align Left"
-msgstr "Wyrównanie do lewej"
+msgstr ""
 
 msgid "Align Center"
-msgstr "Wyrównanie do środka"
+msgstr ""
 
 msgid "Align Right"
-msgstr "Wyrównanie do prawej"
+msgstr ""
 
 msgid "Justify"
-msgstr "Wyjustowanie"
+msgstr ""
 
 msgid "Foreground Color"
-msgstr "Kolor czcionki"
+msgstr ""
 
 msgid "Select a color"
-msgstr "Wybierz kolor"
+msgstr "Selecione uma cor"
 
 msgid "Y"
-msgstr "R"
+msgstr "A"
 
 msgid "M"
 msgstr "M"
 
 msgid "w"
-msgstr "t"
+msgstr "s"
 
 msgid "d"
 msgstr "d"
 
 msgid "h"
-msgstr "g"
+msgstr "h"
 
 msgid "m"
 msgstr "m"
 
 msgid "s"
 msgstr "s"
 
 msgid "Preferences..."
-msgstr "Preferencje..."
+msgstr "Preferências..."
 
 msgid "Toolbar"
-msgstr "Pasek narzędzi"
+msgstr "Barra de Ferramentas"
 
 msgid "Default"
-msgstr "Domyślnie"
+msgstr "Padrão"
 
 msgid "Text and Icons"
-msgstr "Tekst i ikony"
+msgstr "Texto e Ícones"
 
 msgid "Text"
-msgstr "Tekst"
+msgstr "Texto"
 
 msgid "Icons"
-msgstr "Ikony"
+msgstr "Ícones"
 
 msgid "Form"
-msgstr "Formularz"
+msgstr "Formulário"
 
 msgid "Save Column Width"
-msgstr "Zapisz szerokość kolumny"
+msgstr ""
 
 msgid "Save Tree State"
-msgstr "Zapamiętaj stan drzewa"
+msgstr "Gravar Estado da Árvore"
 
 msgid "Spell Checking"
-msgstr "Sprawdzanie pisowni"
+msgstr "Verificar Ortografia"
 
 msgid "Play Sound for Code Scanner"
 msgstr ""
 
 msgid "PDA Mode"
-msgstr "Tryb PDA"
+msgstr "Modo dispositivo portátil"
 
 msgid "Search Limit..."
-msgstr "Ograniczenie wyszukiwania..."
+msgstr "Limite de Buscas..."
 
 msgid "Check Version"
-msgstr "Sprawdź wersję"
+msgstr "Verificar Versão"
 
 msgid "Options"
-msgstr "Opcje"
+msgstr "Opções"
 
 #, fuzzy
 msgid "Documentation..."
-msgstr "Akcje..."
+msgstr "Ações..."
 
 msgid "Keyboard Shortcuts..."
-msgstr "Skróty klawiszowe..."
+msgstr "Atalhos..."
 
 msgid "About..."
-msgstr "O programie..."
+msgstr "Sobre..."
 
 msgid "Help"
-msgstr "Pomoc"
+msgstr "Ajuda"
 
 msgid "No result found."
-msgstr "Nie znaleziono wyniku."
+msgstr "Nenhum resultado encontrado."
 
 msgid "Favorites"
-msgstr "Ulubione"
+msgstr "Favoritos"
 
 msgid "Manage..."
-msgstr "Zarządzaj..."
+msgstr "Gerenciar..."
 
 msgid "Action"
-msgstr "Akcja"
+msgstr "Ação"
 
 msgid ""
 "The following action requires to close all tabs.\n"
 "Do you want to continue?"
 msgstr ""
-"Wykonanie polecenia wymaga zamknięcia wszystkich kart.\n"
-"Czy chcesz kontynuować?"
+"A ação seguinte requer que todas as abas sejam fechadas.\n"
+"Você deseja prosseguir?"
 
 msgid "Application Shortcuts"
-msgstr "Skróty aplikacji"
+msgstr "Atalhos"
 
 msgid "Global"
-msgstr "Globalne"
+msgstr "Globais"
 
 msgid "Preferences"
-msgstr "Preferencje"
+msgstr "Preferências"
 
 msgid "Search menu"
-msgstr "Menu wyszukiwania"
+msgstr "Menu de busca"
 
 msgid "Toggle menu"
-msgstr "Menu boczne"
+msgstr "Menu"
 
 msgid "Previous tab"
-msgstr "Poprzednia karta"
+msgstr "Aba Anterior"
 
 msgid "Next tab"
-msgstr "Następna karta"
+msgstr "Próxima Aba"
 
 msgid "Shortcuts"
-msgstr "Skróty"
+msgstr "Atalhos"
 
 msgid "Quit"
-msgstr "Zakończ"
+msgstr "Sair"
 
 msgid "Edition Shortcuts"
-msgstr "Skróty edycji"
+msgstr "Atalhos de Edição"
 
 msgid "Text Entries"
-msgstr "Wpisy tekstowe"
+msgstr "Campos de texto"
 
 msgid "Cut selected text"
-msgstr "Wytnij zaznaczony tekst"
+msgstr "Recortar o texto selecionado"
 
 msgid "Copy selected text"
-msgstr "Skopiuj zaznaczony tekst"
+msgstr "Copiar o texto selecionado"
 
 msgid "Paste copied text"
-msgstr "Wklej zaznaczony tekst"
+msgstr "Colar o texto copiado"
 
 msgid "Next entry"
-msgstr "Następny wpis"
+msgstr "Próximo campo"
 
 msgid "Previous entry"
-msgstr "Poprzedni wpis"
+msgstr "Campo anterior"
 
 msgid "Relation Entries"
-msgstr "Powiązane wpisy"
+msgstr "Campos de relação"
 
 msgid "Create new relation"
-msgstr "Utwórz nowe odniesienie"
+msgstr "Criar nova relação"
 
 msgid "Open/Search relation"
-msgstr "Otwórz/Szukaj odniesienie"
+msgstr "Abrir/Buscar relação"
 
 msgid "List Entries"
-msgstr "Lista wpisów"
+msgstr "Campos em lista"
 
 msgid "Switch view"
-msgstr "Przełącz widok"
+msgstr "Alternar exibição"
 
 msgid "Create/Select new line"
-msgstr "Utwórz/Wybierz nowy wiersz"
+msgstr ""
 
 msgid "Open relation"
-msgstr "Utwórz odnośnik"
+msgstr "Abrir relação"
 
 msgid "Mark line for deletion/removal"
-msgstr "Zaznacz wiersz do usunięcia"
+msgstr ""
 
 msgid "Mark line for removal"
-msgstr "Zaznacz wiersz do usunięcia"
+msgstr ""
 
 msgid "Unmark line for deletion"
-msgstr "Odznacz wiersz do usunięcia"
+msgstr "Desmarcar linha para apagar"
 
 msgid "List/Tree Shortcuts"
-msgstr "Skróty listy/drzewa"
+msgstr "Atalhos da tela de Lista/Árvore"
 
 msgid "Move Cursor"
-msgstr "Przesuń kursor"
+msgstr "Mover cursor"
 
 msgid "Move right"
-msgstr "Przesuń w prawo"
+msgstr "Mover para a direita"
 
 msgid "Move left"
-msgstr "Przesuń w lewo"
+msgstr "Mover para a esquerda"
 
 msgid "Move up"
-msgstr "Przesuń w górę"
+msgstr "Mover para cima"
 
 msgid "Move down"
-msgstr "Przesuń w dół"
+msgstr "Mover para baixo"
 
 msgid "Move up of one page"
-msgstr "Przesuń w górę o jedną stronę"
+msgstr "Mover uma página para cima"
 
 msgid "Move down of one page"
-msgstr "Przesuń w dół o jedną stronę"
+msgstr "Mover uma página para baixo"
 
 msgid "Move to top"
-msgstr "Przesuń do góry"
+msgstr "Mover para o topo"
 
 msgid "Move to bottom"
-msgstr "Przesuń do dołu"
+msgstr "Mover para o final"
 
 msgid "Move to parent"
-msgstr "Przesuń do elementu nadrzędnego"
+msgstr "Mover para o pai"
 
 #, fuzzy
 msgid "Edition"
-msgstr "Edycja"
+msgstr "Editar"
 
 #, fuzzy
 msgid "Copy selected rows"
-msgstr "Skopiuj zaznaczony tekst"
+msgstr "Copiar o texto selecionado"
 
 msgid "Insert copied rows"
 msgstr ""
 
 msgid "Select all"
-msgstr "Zaznacz wszystko"
+msgstr "Selecionar todos"
 
 msgid "Unselect all"
-msgstr "Odznacz wszystko"
+msgstr "Desmarcar Todos"
 
 msgid "Select parent"
-msgstr "Zaznacz element nadrzędny"
+msgstr "Selecionar pai"
 
 msgid "Select/Activate current row"
-msgstr "Zaznacz/Aktywuj bieżący wiersz"
+msgstr "Selecionar/Ativar linha atual"
 
 msgid "Toggle selection"
-msgstr "Przełącz zaznaczenie"
+msgstr "Alternar seleção"
 
 msgid "Expand/Collapse"
-msgstr "Rozwiń/Zwiń"
+msgstr "Expandir/Recolher"
 
 msgid "Expand row"
-msgstr "Rozwiń wiersz"
+msgstr "Expandir a linha"
 
 msgid "Collapse row"
-msgstr "Zwiń wiersz"
+msgstr "Recolher a linha"
 
 msgid "Toggle row"
-msgstr "Przełącz wiersz"
+msgstr "Alternar linha"
 
 msgid "Collapse all rows"
-msgstr "Zwiń wszystkie wiersze"
+msgstr "Recolher todas as linhas"
 
 msgid "Expand all rows"
-msgstr "Rozwiń wszystkie wiersze"
+msgstr "Expandir todas as linhas"
 
 msgid "Close Tab"
-msgstr "Zamknij kartę"
+msgstr "Fechar Aba"
 
 msgid "modularity, scalability and security"
-msgstr "modułowy, skalowalny i bezpieczny"
+msgstr "modularidade, escalabilidade e segurança"
 
 msgid "translator-credits"
-msgstr "Wojciech Warczakowski"
+msgstr ""
+"Felipe Morato\n"
+"Pedro"
 
 #, python-format
 msgid "Attachments (%s)"
-msgstr "Załączniki (%s)"
+msgstr "Anexos (%s)"
 
 msgid "Code Scanner"
 msgstr ""
 
 msgid "Code"
 msgstr ""
 
 msgid "Profile Editor"
-msgstr "Edytor profili"
+msgstr "Editor de Perfil"
 
 msgid "Profile"
-msgstr "Profil"
+msgstr "Perfil"
 
 msgid "Add new profile"
-msgstr "Dodaj nowy profil"
+msgstr "Adicionar novo perfil"
 
 msgid "Remove selected profile"
-msgstr "Usuń wybrany profil"
+msgstr "Remover perfil selecionado"
 
 msgid "Host:"
-msgstr "Host:"
+msgstr "Servidor:"
 
 msgid "Database:"
-msgstr "Baza danych:"
+msgstr "Banco de Dados:"
 
 msgid "Fetching databases list"
-msgstr "Pobieranie listy baz danych"
+msgstr "Obtendo a lista de bancos de dados"
 
 msgid "Username:"
-msgstr "Użytkownik:"
+msgstr "Usuário:"
 
+#, fuzzy
 msgid "Incompatible version of the server."
-msgstr "Niewłaściwa wersja serwera."
+msgstr "Versão do servidor incompatível"
 
+#, fuzzy
 msgid "Could not connect to the server."
-msgstr "Nie można połączyć się z serwerem."
+msgstr "Não foi possível se conectar ao servidor"
 
 msgid "Login"
-msgstr "Login"
+msgstr "Entrar"
 
 msgid "_Cancel"
-msgstr "Anuluj"
+msgstr "_Cancelar"
 
 msgid "Cancel connection to the Tryton server"
-msgstr "Anuluj połączenie z serwerem Tryton"
+msgstr "Cancelar a conexão com o servidor do Tryton"
 
 msgid "C_onnect"
-msgstr "Połącz"
+msgstr "C_onectar"
 
 msgid "Connect the Tryton server"
-msgstr "Połącz z serwerem Tryton"
+msgstr "Conectar ao servidor do Tryton"
 
 msgid "Profile:"
-msgstr "Profil:"
+msgstr "Perfil:"
 
 msgid "Host / Database information"
-msgstr "Informacje o hoście / bazie danych"
+msgstr "Informações do Servidor / Banco de Dados"
 
 msgid "User name:"
-msgstr "Użytkownik:"
+msgstr "Nome de Usuário:"
 
+#, fuzzy
 msgid "Unable to complete email entry"
-msgstr "Brak możliwości ukończenia edycji e-maila"
+msgstr "Não é possível apagar o assistente %s"
 
-#, python-format
+#, fuzzy, python-format
 msgid "E-mail %s"
-msgstr "E-mail %s"
+msgstr "Email %s"
 
 msgid "To:"
-msgstr "Do:"
+msgstr "Para:"
 
+#, fuzzy
 msgid "Cc:"
-msgstr "DW:"
+msgstr "CC:"
 
 msgid "Bcc:"
-msgstr "UDW:"
+msgstr ""
 
 msgid "Subject:"
-msgstr "Temat:"
+msgstr "Assunto:"
 
+#, fuzzy
 msgid "Body"
-msgstr "Treść"
+msgstr "Conteúdo:"
 
+#, fuzzy
 msgid "Reports"
-msgstr "Raporty"
+msgstr "Relatório"
 
+#, fuzzy
 msgid "Attachments"
-msgstr "Załączniki"
+msgstr "Anexo:"
 
 msgid "Files"
 msgstr ""
 
 msgid "Send"
-msgstr "Wyślij"
+msgstr ""
 
 #, fuzzy
 msgid "Select File"
-msgstr "Zaznacz wszystko"
+msgstr "Selecionar todos"
 
 #, fuzzy
 msgid "Remove File"
-msgstr "Usuń <Del>"
+msgstr "Remover <Del>"
 
 msgid "Select"
-msgstr "Wybierz"
+msgstr "Selecionar"
 
 msgid "Add..."
-msgstr "Dodaj..."
+msgstr "Adicionar..."
 
 #, fuzzy
 msgid "Preview"
-msgstr "Poprzedni"
+msgstr "Anterior"
 
 msgid "Previous"
-msgstr "Poprzedni"
+msgstr "Anterior"
 
 msgid "Next"
-msgstr "Następny"
+msgstr "Próximo"
 
-#, python-format
+#, fuzzy, python-format
 msgid "Attachment (%s)"
-msgstr "Załącznik (%s)"
+msgstr "Anexos (%s)"
 
 #, python-format
 msgid "Note (%d/%d)"
-msgstr "Notatka (%d/%d)"
+msgstr ""
 
 msgid "You have to select one record."
-msgstr "Musisz wybrać jeden rekord."
+msgstr "Você precisa selecionar um registo."
 
 msgid "Are you sure to remove this record?"
-msgstr "Czy na pewno usunąć wybrany rekord?"
+msgstr "Você tem certeza que deseja apagar este registro?"
 
 msgid "Are you sure to remove those records?"
-msgstr "Czy na pewno usunąć wybrane rekordy?"
+msgstr "Você tem certeza que deseja apagar estes registros?"
 
 msgid "Records not removed."
-msgstr "Rekordy nie zostały usunięte."
+msgstr "Registros não apagados."
 
 msgid "Records removed."
-msgstr "Rekordy zostały usunięte."
+msgstr "Registos apagados."
 
 msgid "Working now on the duplicated record(s)."
-msgstr "Pracujesz na zduplikowanym(ch) rekordzie(ch)."
+msgstr "Trabalhando agora no(s) registo(s) duplicado(s)"
 
 msgid "Record saved."
-msgstr "Rekord został zapisany."
+msgstr "Registo gravado."
 
 msgid ""
 "This record has been modified\n"
 "do you want to save it?"
 msgstr ""
-"Rekord został zmodyfikowany.\n"
-"Czy chcesz go zapisać?"
+"Este registo foi modificado\n"
+"você deseja gravá-lo?"
 
 msgid "Launch action"
-msgstr "Uruchom akcję"
+msgstr "Executar ação"
 
 msgid "Relate"
-msgstr "Odnośnik"
+msgstr "Relacionar"
 
 msgid "Open related records"
-msgstr "Otwórz powiązane rekordy"
+msgstr "Abrir registos relacionados"
 
 msgid "Report"
-msgstr "Raport"
+msgstr "Relatório"
 
 msgid "Open report"
-msgstr "Otwórz raport"
+msgstr "Abrir relatório"
 
 msgid "Print"
-msgstr "Wydruk"
+msgstr "Imprimir"
 
 msgid "Print report"
-msgstr "Drukuj raport"
+msgstr "Imprimir relatório"
 
 msgid "_Copy URL"
-msgstr "Skopiuj adres URL"
+msgstr "_Copiar URL"
 
 msgid "Copy URL into clipboard"
-msgstr "Skopiuj adres URL do schowka"
+msgstr "Copiar URL para a área de transferência"
 
 msgid "Unknown"
-msgstr "Nieznany"
+msgstr "Desconhecido"
 
 msgid "Limit"
-msgstr "Limit"
+msgstr "Limite"
 
 msgid "Search Limit Settings"
-msgstr "Ustawienia limitu wyszukiwania"
+msgstr "Preferências de limite de buscas"
 
 msgid "Limit:"
-msgstr "Limit:"
+msgstr "Limite:"
 
 #, python-format
 msgid "Logs (%s)"
-msgstr "Logi (%s)"
+msgstr "Histórico (%s)"
 
 msgid "Model:"
-msgstr "Model:"
+msgstr "Modelo:"
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
+#, fuzzy
 msgid "Created by:"
-msgstr "Utworzył:"
+msgstr "Data de criação"
 
+#, fuzzy
 msgid "Created at:"
-msgstr "Data utworzenia:"
+msgstr "Data de criação"
 
 #, fuzzy
 msgid "Last Modified by:"
-msgstr "Autor ostatniej modyfikacji:"
+msgstr "Última Modificação por:"
 
 #, fuzzy
 msgid "Last Modified at:"
-msgstr "Data ostatniej modyfikacji:"
+msgstr "Data da última modificação:"
 
 #, python-format
 msgid "Notes (%s)"
-msgstr "Notatki (%s)"
+msgstr "Notas (%s)"
 
 msgid "Edit User Preferences"
-msgstr "Edytuj preferencje użytkownika"
+msgstr "Editar preferências do usuário"
 
 msgid "Preference"
-msgstr "Preferencje"
+msgstr "Preferência"
 
 msgid "Revision"
-msgstr "Rewizja"
+msgstr "Revisão"
 
 msgid "Select a revision"
-msgstr "Wybierz rewizję"
+msgstr "Selecione uma revisão"
 
 msgid "Revision:"
-msgstr "Rewizja:"
+msgstr "Revisão:"
 
 msgid "_Switch View"
-msgstr "Przełącz widok"
+msgstr "_Alternar Exibição"
 
 msgid "Switch View"
-msgstr "Przełącz widok"
+msgstr "Alternar"
 
 msgid "_Previous"
-msgstr "Poprzedni"
+msgstr "_Anterior"
 
 msgid "Previous Record"
-msgstr "Poprzedni rekord"
+msgstr "Registro Anterior"
 
 msgid "_Next"
-msgstr "Następny"
+msgstr "_Próximo"
 
 msgid "Next Record"
-msgstr "Następny rekord"
+msgstr "Próximo Registro"
 
 msgid "_Search"
-msgstr "Szukaj"
+msgstr "_Buscar"
 
 msgid "_New"
-msgstr "Nowy"
+msgstr "_Novo"
 
 msgid "Create a new record"
-msgstr "Utwórz nowy rekord"
+msgstr "Criar novo registro"
 
 msgid "_Save"
-msgstr "Zapisz"
+msgstr "_Salvar"
 
 msgid "Save this record"
-msgstr "Zapisz rekord"
+msgstr "Gravar este registro"
 
 msgid "_Reload/Undo"
-msgstr "Odśwież/Przywróć"
+msgstr "_Recarregar/Desfazer"
 
 msgid "Reload/Undo"
-msgstr "Odśwież/Przywróć"
+msgstr "Recarregar/Desfazer"
 
 msgid "_Duplicate"
-msgstr "Duplikuj"
+msgstr "_Duplicado"
 
 msgid "_Delete..."
-msgstr "Usuń..."
+msgstr "_Apagar..."
 
 msgid "View _Logs..."
-msgstr "Przeglądaj dziennik..."
+msgstr "Ver _Logs..."
 
 msgid "Show revisions..."
-msgstr "Pokaż rewizje..."
+msgstr "Mostrar revisões..."
 
 msgid "A_ttachments..."
-msgstr "Załączniki..."
+msgstr "A_nexos..."
 
 msgid "Add an attachment to the record"
-msgstr "Dodaj załącznik do rekordu"
+msgstr "Adicionar um anexo ao registro"
 
 msgid "_Notes..."
-msgstr "Notatki..."
+msgstr "_Notas..."
 
 msgid "Add a note to the record"
-msgstr "Dodaj notatkę do rekordu"
+msgstr "Adicionar uma nota ao registro"
 
 msgid "_Actions..."
-msgstr "Akcje..."
+msgstr "_Ações..."
 
 msgid "_Relate..."
-msgstr "Odnośnik..."
+msgstr "_Relacionar"
 
 msgid "_Report..."
-msgstr "Raport..."
+msgstr "_Relatório..."
 
 msgid "_Print..."
-msgstr "Wydruk..."
+msgstr "_Imprimir..."
 
 msgid "_E-Mail..."
-msgstr "E-mail..."
+msgstr "_E-Mail..."
 
+#, fuzzy
 msgid "Send an e-mail using the record"
-msgstr "Wyślij e-mail używając rekordu"
+msgstr "Adicionar uma nota ao registro"
 
 msgid "_Export Data..."
-msgstr "Eksportuj dane..."
+msgstr "_Exportar Dados..."
 
 msgid "_Import Data..."
-msgstr "Importuj dane..."
+msgstr "_Importar Dados..."
 
 msgid "Copy _URL..."
-msgstr "Skopiuj adres URL..."
+msgstr "Copiar _URL..."
 
 msgid "_Close Tab"
-msgstr "Zamknij kartę"
+msgstr "_Fechar aba"
 
 msgid "<b>All fields</b>"
-msgstr "<b>Wszystkie pola</b>"
+msgstr "<b>Todos os campos</b>"
 
 msgid "_Add"
-msgstr "Dodaj"
+msgstr "_Adicionar"
 
 msgid "_Remove"
-msgstr "Usuń"
+msgstr "_Remover"
 
 msgid "_Clear"
-msgstr "Wyczyść"
+msgstr "_Limpar"
 
 msgid "<b>Fields selected</b>"
-msgstr "<b>Pola wybrane</b>"
+msgstr "<b>Campos selecionados</b>"
 
 msgid "CSV Parameters"
-msgstr "Parametry CSV"
+msgstr "Parâmetros CSV"
 
 msgid "Delimiter:"
-msgstr "Separator:"
+msgstr "Delimitador:"
 
 msgid "Quote char:"
-msgstr "Znak cudzysłowu:"
+msgstr "Caractere de citação:"
 
 msgid "Encoding:"
-msgstr "Kodowanie:"
+msgstr "Codificação:"
 
 msgid "Use locale format"
-msgstr "Użyj formatu lokalnego"
+msgstr ""
 
 msgid "Field name"
-msgstr "Nazwa pola"
+msgstr "Nome do campo"
 
 #, python-format
 msgid "CSV Export: %s"
-msgstr "Eksport do CSV: %s"
+msgstr "Exportar CSV: %s"
 
 msgid "_Save Export"
-msgstr "Zapisz eksport"
+msgstr "_Gravar exportação"
 
+#, fuzzy
 msgid "_URL Export"
-msgstr "Eksport URL"
+msgstr "_Gravar exportação"
 
 msgid "_Delete Export"
-msgstr "Usuń eksport"
+msgstr "_Apagar exportação"
 
 msgid "<b>Predefined exports</b>"
-msgstr "<b>Predefiniowane eksporty</b>"
+msgstr "<b>Exportações pré-definidas</b>"
 
 msgid "Name"
-msgstr "Nazwa"
+msgstr "Nome"
 
 msgid "Open"
-msgstr "Otwórz"
+msgstr "Abrir"
 
 msgid "Save"
-msgstr "Zapisz"
+msgstr "Gravar"
 
+#, fuzzy
 msgid "Listed Records"
-msgstr "Wymienione rekordy"
+msgstr "Editar o registro selecionado <F2>"
 
+#, fuzzy
 msgid "Selected Records"
-msgstr "Wybrane rekordy"
+msgstr "Editar o registro selecionado <F2>"
 
 msgid "Ignore search limit"
-msgstr "Ignoruj limit wyszukiwań"
+msgstr ""
 
+#, fuzzy
 msgid "Add field names"
-msgstr "Dodaj nazwy pól"
+msgstr "Adicionar _nomes de campos"
 
 #, python-format
 msgid "%s (string)"
-msgstr "%s (string)"
+msgstr "%s (texto)"
 
 #, python-format
 msgid "%s (model name)"
-msgstr "%s (model name)"
+msgstr "%s (nome do modelo)"
 
 #, fuzzy, python-format
 msgid "%s/Record Name"
-msgstr "%s (record name)"
+msgstr "%s (nome do registro)"
 
 msgid "What is the name of this export?"
-msgstr "Jaka jest nazwa tego eksportu?"
+msgstr "Qual é o nome dessa exportação?"
 
 #, python-format
 msgid "Override '%s' definition?"
-msgstr "Czy nadpisać definicję '%s'?"
+msgstr "Sobrescrever a definição '%s'?"
 
 #, python-format
 msgid "%d record saved."
-msgstr "%d rekord został zapisany."
+msgstr "%d registro gravado."
 
 #, python-format
 msgid "%d records saved."
-msgstr "%d rekordy zostały zapisane."
+msgstr "%d registros gravados."
 
 msgid "Export failed"
 msgstr ""
 
 msgid "Link"
-msgstr "Link"
+msgstr "Vínculo"
 
 msgid "Delete"
-msgstr "Usuń"
+msgstr "Apagar"
 
 msgid "Discard changes"
 msgstr ""
 
 msgid "Save and New"
 msgstr ""
 
 #, fuzzy
 msgid "Add and New"
-msgstr "Dodaj wartość"
+msgstr "Adicionar valor"
 
 msgid "Add"
-msgstr "Dodaj"
+msgstr "Adicionar"
 
 msgid "Apply changes"
 msgstr ""
 
 msgid "Switch"
-msgstr "Przełącz"
+msgstr "Alternar"
 
 msgid "Remove <Del>"
-msgstr "Usuń <Del>"
+msgstr "Remover <Del>"
 
 msgid "Create a new record <F3>"
-msgstr "Utwórz nowy rekord <F3>"
+msgstr "Criar novo registro <F3>"
 
 msgid "Delete selected record <Del>"
-msgstr "Usuń zaznaczony rekord <Del>"
+msgstr "Apagar o registro selecionado <Del>"
 
 msgid "Undelete selected record <Ins>"
-msgstr "Przywróć zaznaczony rekord <Ins>"
+msgstr "Recuperar o registro selecionado <Ins>"
 
 #, python-format
 msgid "CSV Import: %s"
-msgstr "Import z CSV: %s"
+msgstr "Importar CSV: %s"
 
 msgid "_Auto-Detect"
-msgstr "Rozpoznaj"
+msgstr "_Auto-Detectar"
 
 msgid "File to Import:"
-msgstr "Plik do zaimportowania:"
+msgstr "Arquivo para importar:"
 
 msgid "Open..."
-msgstr "Otwórz..."
+msgstr "Abrir..."
 
 msgid "Lines to Skip:"
-msgstr "Wiersze do ominięcia:"
+msgstr "Linhas a ignorar:"
 
 msgid "You must select an import file first."
-msgstr "Wybierz plik do zaimportowania."
+msgstr "Primeiro você deve selecionar um arquivo para importar."
 
 msgid "Detection failed"
 msgstr ""
 
 #, python-format
 msgid "Unknown column header \"%s\""
 msgstr ""
 
 msgid "Error"
-msgstr "Błąd"
+msgstr "Erro"
 
 msgid "Import failed"
 msgstr ""
 
 #, python-format
 msgid "%d record imported."
-msgstr "Rekord %d został zaimportowany."
+msgstr "%d registros importados."
 
 #, python-format
 msgid "%d records imported."
-msgstr "Rekordy %d zostały zaimportowane."
+msgstr "%d registros importados."
 
 msgid "Search"
-msgstr "Szukaj"
+msgstr "Busca"
 
 msgid "New"
-msgstr "Nowy"
+msgstr "Novo"
 
 #, python-format
 msgid "Search %s"
-msgstr "Szukaj %s"
+msgstr "Buscar %s"
 
 msgid "Wizard"
-msgstr "Kreator"
+msgstr "Assistente"
 
 msgid "ID"
 msgstr "ID"
 
 #, fuzzy
 msgid "Created by"
-msgstr "Utworzył:"
+msgstr "Data de criação"
 
+#, fuzzy
 msgid "Created at"
-msgstr "Data utworzenia"
+msgstr "Data de criação"
 
+#, fuzzy
 msgid "Edited by"
-msgstr "Zmodyfikował"
+msgstr "Editar"
 
+#, fuzzy
 msgid "Edited at"
-msgstr "Data modyfikacji"
+msgstr "Editar"
 
 msgid "Unable to set view tree state"
-msgstr "Brak możliwości ustawienia stanu widoku drzewa"
+msgstr "Não foi possível definir o estado da visão em árvore"
 
-#, python-format
+#, fuzzy, python-format
 msgid "\"%s\" is not valid according to its domain."
-msgstr "\"%s\" jest nieprawidłowy pod względem swojej domeny."
+msgstr "\"%s\" não é válido de acordo com seu domínio"
 
-#, python-format
+#, fuzzy, python-format
 msgid "\"%s\" is required."
-msgstr "\"%s\" jest wymagany."
+msgstr "\"%s\" é obrigatório"
 
-#, python-format
+#, fuzzy, python-format
 msgid "The values of \"%s\" are not valid."
-msgstr "Wartości \"%s\" nie są prawidłowe."
+msgstr "Os valores de \"%s\" não são válidos"
 
 msgid "Pre-validation"
-msgstr "Wstępna walidacja"
+msgstr "Pré-validação"
 
 msgid ":"
 msgstr ":"
 
 msgid "Scan"
 msgstr ""
 
 msgid "Image Size"
-msgstr "Rozmiar obrazka"
+msgstr "Tamanho da imagem"
 
 msgid "Width:"
-msgstr "Szerokość:"
+msgstr "Largura:"
 
 msgid "Height:"
-msgstr "Wysokość:"
+msgstr "Altura:"
 
 msgid "PNG image (*.png)"
-msgstr "Obrazek w formacie PNG (*.png)"
+msgstr "Imagem PNG (*.png)"
 
 msgid "Save As"
-msgstr "Zapisz jako"
+msgstr "Salvar como"
 
 msgid "Image size too large."
-msgstr "Za duży rozmiar obrazka."
+msgstr "Imagem muito grande."
 
 msgid "Copy"
-msgstr "Kopiuj"
+msgstr ""
 
 #, fuzzy
 msgid "Copy Row"
-msgstr "Skopiuj adres URL"
+msgstr "_Copiar URL"
 
 #, fuzzy
 msgid "Copy Rows"
-msgstr "Skopiuj adres URL"
+msgstr "_Copiar URL"
 
 msgid "Copy Column"
 msgstr ""
 
-#, fuzzy
 msgid "Paste Rows"
-msgstr "Wklej"
+msgstr ""
 
 msgid ".."
 msgstr ".."
 
 msgid "Open filters"
-msgstr "Otwórz filtry"
+msgstr "Abrir filtros"
 
 msgid "Show bookmarks of filters"
-msgstr "Pokaż zakładki filtrów"
+msgstr "Mostrar filtros favoritos"
 
 msgid "Remove this bookmark"
-msgstr "Usuń zakładkę"
+msgstr "Remover este favorito"
 
 msgid "Bookmark this filter"
-msgstr "Dodaj filtr do zakładek"
+msgstr "Marcar este filtro como favorito"
 
 msgid "Show active records"
-msgstr "Pokaż aktywne rekordy"
+msgstr "Mostrar registros ativos"
 
 msgid "Show inactive records"
-msgstr "Pokaż nieaktywne rekordy"
+msgstr "Mostrar registros inativos"
 
 msgid "Bookmark Name:"
-msgstr "Dodaj nazwę zakładek:"
+msgstr "Nome do favorito:"
 
 msgid "Find"
-msgstr "Znajdź"
+msgstr "Localizar"
 
 msgid "Today"
-msgstr "Dzisiaj"
+msgstr "Hoje"
 
 msgid "go back"
-msgstr "wstecz"
+msgstr "voltar"
 
 msgid "go forward"
-msgstr "dalej"
+msgstr "avançar"
 
 msgid "previous year"
-msgstr "poprzedni rok"
+msgstr "ano anterior"
 
 msgid "next year"
-msgstr "następny rok"
+msgstr "próximo ano"
 
 msgid "Day"
 msgstr ""
 
 msgid "Week"
-msgstr "Tydzień"
+msgstr "Semana"
 
 #, fuzzy
 msgid "Month"
-msgstr "Widok miesiąca"
+msgstr "Visão Mensal"
 
 msgid "Select..."
-msgstr "Wybierz..."
+msgstr "Selecionar..."
 
 msgid "Clear"
-msgstr "Wyczyść"
+msgstr "Limpar"
 
 msgid "All files"
-msgstr "Wszystkie pliki"
+msgstr "Todos os arquivos"
 
 msgid "Show plain text"
-msgstr "Pokaż tekst"
+msgstr "Mostrar em formato texto"
 
 msgid "Add value"
-msgstr "Dodaj wartość"
+msgstr "Adicionar valor"
 
 #, python-format
 msgid "Remove \"%s\""
-msgstr "Usuń \"%s\""
+msgstr "Remover \"%s\""
 
 msgid "Images"
-msgstr "Obrazki"
+msgstr "Imagens"
 
 msgid "Add existing record"
-msgstr "Dodaj istniejący rekord"
+msgstr "Adicionar um registro existente"
 
 msgid "Remove selected record"
-msgstr "Usuń wybrany rekord"
+msgstr "Remover o registro selecionado"
 
 msgid "Open the record <F2>"
-msgstr "Otwórz rekord <F2>"
+msgstr "Abrir o registro <F2>"
 
 msgid "Clear the field <Del>"
-msgstr "Wyczyść pole <Del>"
+msgstr "Apagar o registro <Del>"
 
 msgid "Search a record <F2>"
-msgstr "Szukaj rekord <F2>"
+msgstr "Buscar um registro <F2>"
 
+#, fuzzy
 msgid "Edit selected record"
-msgstr "Edytuj wybrany rekord"
+msgstr "Editar o registro selecionado <F2>"
 
+#, fuzzy
 msgid "Delete selected record"
-msgstr "Usuń wybrany rekord"
+msgstr "Remover o registro selecionado"
 
 #, python-format
 msgid "%s%%"
 msgstr "%s%%"
 
 msgid "Choose a language"
-msgstr "Wybierz język"
+msgstr ""
 
 msgid "Translation"
-msgstr "Tłumaczenie"
+msgstr "Tradução"
 
 msgid "Edit"
-msgstr "Edycja"
+msgstr "Editar"
 
 msgid "Fuzzy"
-msgstr "Niejasne"
+msgstr "Vago"
 
 msgid "You need to save the record before adding translations."
-msgstr "Musisz zapisać rekord przed dodaniem tłumaczeń."
+msgstr "Você precisa salvar o registro antes de adicionar traduções."
 
 msgid "No other language available."
-msgstr "Brak innych języków."
+msgstr "Não há outros idiomas disponíveis."
 
 msgid "#ERROR"
 msgstr ""
 
 msgid "Translate view"
-msgstr "Widok tłumaczenia"
+msgstr "Traduzir visão"
```

### Comparing `tryton-7.2.0/tryton/data/locale/pt/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/pt/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: pt\n"
 "Language-Team: pt <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/ro/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/ro/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ro\n"
 "Language-Team: ro <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n==1 ? 0 : (n==0 || (n%100 > 0 && n%100 < "
 "20)) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/ro/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/ro/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,16 @@
 
 msgid "No"
 msgstr "Nu"
 
 msgid "Yes"
 msgstr "Da"
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "Excepție de concurgență"
 
 msgid "This record has been modified while you were editing it."
 msgstr "Această înregistrare a fost modificată în timp ce o editați."
 
 msgid "Cancel saving"
 msgstr "Anulați salvarea"
@@ -107,14 +108,17 @@
 
 msgid "Close"
 msgstr "Închidere"
 
 msgid "Application Error"
 msgstr "Eroare de aplicație"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "Raporteati eroare"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "Verificați adresa URL: %s"
 
@@ -123,19 +127,22 @@
 
 msgid "A new version is available!"
 msgstr "O nouă versiune este disponibilă!"
 
 msgid "Download"
 msgstr "Descarca"
 
+msgid "Concurrency Exception"
+msgstr "Excepție de concurgență"
+
 msgid "Could not get a session."
 msgstr "Nu s-a putut găsi o sesiune."
 
 #, fuzzy, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr "Prea multe cereri. Încercați mai târziu."
 
 msgid "Too many requests. Try again later."
 msgstr "Prea multe cereri. Încercați mai târziu."
 
 msgid "Not Found."
 msgstr "Niciun rezultat găsit."
@@ -719,14 +726,20 @@
 
 msgid "Model:"
 msgstr "Model:"
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 msgid "Created by:"
 msgstr "Creat de:"
 
 msgid "Created at:"
 msgstr "Creat la:"
 
 msgid "Last Modified by:"
```

### Comparing `tryton-7.2.0/tryton/data/locale/ru/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/ru/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ru\n"
 "Language-Team: ru <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/ru/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/ru/LC_MESSAGES/tryton.po`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,16 @@
 
 msgid "No"
 msgstr ""
 
 msgid "Yes"
 msgstr ""
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "Прерывание конкурентных записей"
 
 msgid "This record has been modified while you were editing it."
 msgstr ""
 
 msgid "Cancel saving"
 msgstr ""
@@ -116,14 +117,17 @@
 msgid "Close"
 msgstr ""
 
 #, fuzzy
 msgid "Application Error"
 msgstr "Ошибка приложения!"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "Сообщить об ошибке"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr ""
 
@@ -132,20 +136,23 @@
 
 msgid "A new version is available!"
 msgstr ""
 
 msgid "Download"
 msgstr ""
 
+msgid "Concurrency Exception"
+msgstr "Прерывание конкурентных записей"
+
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Не удается подключиться к серверу!"
 
 #, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr ""
 
 msgid "Too many requests. Try again later."
 msgstr ""
 
 #, fuzzy
 msgid "Not Found."
@@ -772,14 +779,20 @@
 
 msgid "Model:"
 msgstr "Модель:"
 
 msgid "ID:"
 msgstr "Номер строки"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 #, fuzzy
 msgid "Created by:"
 msgstr "Дата создания"
 
 #, fuzzy
 msgid "Created at:"
 msgstr "Дата создания"
```

### Comparing `tryton-7.2.0/tryton/data/locale/sl/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/sl/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: sl\n"
 "Language-Team: sl <LL@li.org>\n"
 "Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
 "n%100==4 ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/sl/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/sl/LC_MESSAGES/tryton.po`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,16 @@
 
 msgid "No"
 msgstr "Ne"
 
 msgid "Yes"
 msgstr "Da"
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "Izjema sočasnega izvajanja"
 
 msgid "This record has been modified while you were editing it."
 msgstr "Ta zapis je bil spremenjen med urejanjem."
 
 msgid "Cancel saving"
 msgstr "Prekliči shranjevanje"
@@ -111,14 +112,17 @@
 
 msgid "Close"
 msgstr "Zapri"
 
 msgid "Application Error"
 msgstr "Programska napaka"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "Prijava programske napake"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "Preveri URL: %s"
 
@@ -127,19 +131,22 @@
 
 msgid "A new version is available!"
 msgstr "Nova različica programa je na voljo!"
 
 msgid "Download"
 msgstr "Prenesi"
 
+msgid "Concurrency Exception"
+msgstr "Izjema sočasnega izvajanja"
+
 msgid "Could not get a session."
 msgstr "Ni mogoče vzpostaviti seje."
 
 #, fuzzy, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr "Preveč poslanih zahtev. Poskusite kasneje."
 
 msgid "Too many requests. Try again later."
 msgstr "Preveč poslanih zahtev. Poskusite kasneje."
 
 msgid "Not Found."
 msgstr "Ni najdeno."
@@ -724,14 +731,20 @@
 
 msgid "Model:"
 msgstr "Model:"
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 msgid "Created by:"
 msgstr "Ustvaril:"
 
 msgid "Created at:"
 msgstr "Ustvarjeno ob:"
 
 msgid "Last Modified by:"
```

### Comparing `tryton-7.2.0/tryton/data/locale/tr/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/tr/LC_MESSAGES/tryton.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: tr\n"
 "Language-Team: tr <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/tr/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/tr/LC_MESSAGES/tryton.po`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 msgid "No"
 msgstr ""
 
 msgid "Yes"
 msgstr ""
 
-msgid "Concurrency Exception"
+msgid "Concurrency Warning"
 msgstr ""
 
 msgid "This record has been modified while you were editing it."
 msgstr ""
 
 msgid "Cancel saving"
 msgstr ""
@@ -112,14 +112,17 @@
 msgid "Close"
 msgstr ""
 
 #, fuzzy
 msgid "Application Error"
 msgstr "Uygulama Hatası."
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "Hatayı Raporla"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr ""
 
@@ -128,19 +131,22 @@
 
 msgid "A new version is available!"
 msgstr ""
 
 msgid "Download"
 msgstr ""
 
+msgid "Concurrency Exception"
+msgstr ""
+
 msgid "Could not get a session."
 msgstr ""
 
 #, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr ""
 
 msgid "Too many requests. Try again later."
 msgstr ""
 
 msgid "Not Found."
 msgstr ""
@@ -723,14 +729,20 @@
 
 msgid "Model:"
 msgstr ""
 
 msgid "ID:"
 msgstr ""
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 msgid "Created by:"
 msgstr ""
 
 msgid "Created at:"
 msgstr ""
 
 msgid "Last Modified by:"
```

### Comparing `tryton-7.2.0/tryton/data/locale/tryton.pot` & `tryton-7.2.1/tryton/data/locale/tryton.pot`

 * *Files 0% similar despite different names*

```diff
@@ -717,14 +717,20 @@
 
 msgid "Model:"
 msgstr ""
 
 msgid "ID:"
 msgstr ""
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 msgid "Created by:"
 msgstr ""
 
 msgid "Created at:"
 msgstr ""
 
 msgid "Last Modified by:"
```

### Comparing `tryton-7.2.0/tryton/data/locale/uk/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/uk/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: uk\n"
 "Language-Team: uk <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/uk/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/uk/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,16 @@
 
 msgid "No"
 msgstr "Ні"
 
 msgid "Yes"
 msgstr "Так"
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "Виняток одночасного доступу"
 
 msgid "This record has been modified while you were editing it."
 msgstr "Цей запис було змінено, поки ви його редагували."
 
 msgid "Cancel saving"
 msgstr "Скасувати збереження"
@@ -107,14 +108,17 @@
 
 msgid "Close"
 msgstr "Закрити"
 
 msgid "Application Error"
 msgstr "Помилка програми"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "Повідомити про помилку"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "Перевірка URL: %s"
 
@@ -123,20 +127,23 @@
 
 msgid "A new version is available!"
 msgstr "Доступна нова версія!"
 
 msgid "Download"
 msgstr "Завантажити"
 
+msgid "Concurrency Exception"
+msgstr "Виняток одночасного доступу"
+
 #, fuzzy
 msgid "Could not get a session."
 msgstr "Не вдалося підключитися до сервера."
 
 #, fuzzy, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr "Дуже багато запитів. Спробуйте ще раз пізніше."
 
 msgid "Too many requests. Try again later."
 msgstr "Дуже багато запитів. Спробуйте ще раз пізніше."
 
 #, fuzzy
 msgid "Not Found."
@@ -727,14 +734,20 @@
 
 msgid "Model:"
 msgstr "Модель:"
 
 msgid "ID:"
 msgstr "ID:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 msgid "Created by:"
 msgstr "Ким створено:"
 
 msgid "Created at:"
 msgstr "Коли створено:"
 
 msgid "Last Modified by:"
```

### Comparing `tryton-7.2.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo` & `tryton-7.2.1/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-29 17:30+0200\n"
+"POT-Creation-Date: 2024-05-01 11:13+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_CN\n"
 "Language-Team: zh_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `tryton-7.2.0/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po` & `tryton-7.2.1/tryton/data/locale/zh_CN/LC_MESSAGES/tryton.po`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,16 @@
 
 msgid "No"
 msgstr "否"
 
 msgid "Yes"
 msgstr "是"
 
-msgid "Concurrency Exception"
+#, fuzzy
+msgid "Concurrency Warning"
 msgstr "并行操作异常"
 
 msgid "This record has been modified while you were editing it."
 msgstr "在你编辑的时候，这条记录已经被更改."
 
 msgid "Cancel saving"
 msgstr "取消保存"
@@ -110,14 +111,17 @@
 
 msgid "Close"
 msgstr "关闭"
 
 msgid "Application Error"
 msgstr "程序错误"
 
+msgid "Details"
+msgstr ""
+
 msgid "Report Bug"
 msgstr "报告Bug"
 
 #, python-format
 msgid "Check URL: %s"
 msgstr "检查URL: %s"
 
@@ -126,19 +130,22 @@
 
 msgid "A new version is available!"
 msgstr "有新版本可用！"
 
 msgid "Download"
 msgstr "下载"
 
+msgid "Concurrency Exception"
+msgstr "并行操作异常"
+
 msgid "Could not get a session."
 msgstr "无法获取会话。"
 
 #, fuzzy, python-format
-msgid "Error \"%s\". Try again later."
+msgid "Error: \"%s\". Try again later."
 msgstr "请求太多，请稍后重试."
 
 msgid "Too many requests. Try again later."
 msgstr "请求太多，请稍后重试."
 
 msgid "Not Found."
 msgstr "无符合条件的数据."
@@ -722,14 +729,20 @@
 
 msgid "Model:"
 msgstr "模型:"
 
 msgid "ID:"
 msgstr "标识:"
 
+msgid "Module:"
+msgstr ""
+
+msgid "XML ID:"
+msgstr ""
+
 msgid "Created by:"
 msgstr "创建者:"
 
 msgid "Created at:"
 msgstr "创建日期:"
 
 msgid "Last Modified by:"
```

### Comparing `tryton-7.2.0/tryton/data/pixmaps/tryton/LICENSE` & `tryton-7.2.1/tryton/data/pixmaps/tryton/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-icon.png` & `tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-icon.png`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-icon.svg` & `tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-icon.svg`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/data/pixmaps/tryton/tryton-unarchive.svg` & `tryton-7.2.1/tryton/data/pixmaps/tryton/tryton-unarchive.svg`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/data/pixmaps/tryton/tryton.icns` & `tryton-7.2.1/tryton/data/pixmaps/tryton/tryton.icns`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/data/pixmaps/tryton/tryton.ico` & `tryton-7.2.1/tryton/data/pixmaps/tryton/tryton.ico`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/data/pixmaps/tryton/tryton.svg` & `tryton-7.2.1/tryton/data/pixmaps/tryton/tryton.svg`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/data/sounds/LICENSE` & `tryton-7.2.1/tryton/data/sounds/LICENSE`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/data/sounds/danger.wav` & `tryton-7.2.1/tryton/data/sounds/danger.wav`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/data/sounds/success.wav` & `tryton-7.2.1/tryton/data/sounds/success.wav`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/device_cookie.py` & `tryton-7.2.1/tryton/device_cookie.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/fingerprints.py` & `tryton-7.2.1/tryton/fingerprints.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/main.py` & `tryton-7.2.1/tryton/gui/main.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/about.py` & `tryton-7.2.1/tryton/gui/window/about.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/attachment.py` & `tryton-7.2.1/tryton/gui/window/attachment.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/board.py` & `tryton-7.2.1/tryton/gui/window/board.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/code_scanner.py` & `tryton-7.2.1/tryton/gui/window/code_scanner.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/dblogin.py` & `tryton-7.2.1/tryton/gui/window/dblogin.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/email_.py` & `tryton-7.2.1/tryton/gui/window/email_.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/form.py` & `tryton-7.2.1/tryton/gui/window/form.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/infobar.py` & `tryton-7.2.1/tryton/gui/window/infobar.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/limit.py` & `tryton-7.2.1/tryton/gui/window/limit.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/log.py` & `tryton-7.2.1/tryton/gui/window/log.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/nomodal.py` & `tryton-7.2.1/tryton/gui/window/nomodal.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/note.py` & `tryton-7.2.1/tryton/gui/window/note.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/preference.py` & `tryton-7.2.1/tryton/gui/window/preference.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/revision.py` & `tryton-7.2.1/tryton/gui/window/revision.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/tabcontent.py` & `tryton-7.2.1/tryton/gui/window/tabcontent.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_board/action.py` & `tryton-7.2.1/tryton/gui/window/view_board/action.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_board/view_board.py` & `tryton-7.2.1/tryton/gui/window/view_board/view_board.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/model/field.py` & `tryton-7.2.1/tryton/gui/window/view_form/model/field.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/model/group.py` & `tryton-7.2.1/tryton/gui/window/view_form/model/group.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/model/record.py` & `tryton-7.2.1/tryton/gui/window/view_form/model/record.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/screen/screen.py` & `tryton-7.2.1/tryton/gui/window/view_form/screen/screen.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/__init__.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/calendar_.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/calendar_gtk/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/calendar_gtk/dates_period.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/calendar_gtk/toolbar.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/binary.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/binary.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/calendar_.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/calendar_.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/char.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/char.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/checkbox.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/checkbox.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/dictionary.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/dictionary.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/document.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/document.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/float.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/float.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/image.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/image.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/integer.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/integer.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/many2many.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/many2many.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/many2one.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/many2one.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/multiselection.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/multiselection.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/one2many.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/one2many.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/progressbar.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/progressbar.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/pyson.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/pyson.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/reference.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/reference.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/richtextbox.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/richtextbox.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/selection.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/selection.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/state_widget.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/state_widget.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/textbox.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/textbox.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/timedelta.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/url.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/url.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/form_gtk/widget.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/form_gtk/widget.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/graph.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/graph.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/bar.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/graph_gtk/bar.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/graph.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/graph_gtk/graph.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/line.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/graph_gtk/line.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/graph_gtk/pie.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/graph_gtk/pie.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/list.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/list.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/list_form.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/list_form.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/list_gtk/editabletree.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/list_gtk/editabletree.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/list_gtk/widget.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/list_gtk/widget.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/view_form/view/screen_container.py` & `tryton-7.2.1/tryton/gui/window/view_form/view/screen_container.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/win_csv.py` & `tryton-7.2.1/tryton/gui/window/win_csv.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/win_export.py` & `tryton-7.2.1/tryton/gui/window/win_export.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/win_form.py` & `tryton-7.2.1/tryton/gui/window/win_form.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/win_import.py` & `tryton-7.2.1/tryton/gui/window/win_import.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/win_search.py` & `tryton-7.2.1/tryton/gui/window/win_search.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/window.py` & `tryton-7.2.1/tryton/gui/window/window.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/gui/window/wizard.py` & `tryton-7.2.1/tryton/gui/window/wizard.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/jsonrpc.py` & `tryton-7.2.1/tryton/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/plugins/__init__.py` & `tryton-7.2.1/tryton/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/plugins/translation/__init__.py` & `tryton-7.2.1/tryton/plugins/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/pyson.py` & `tryton-7.2.1/tryton/pyson.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/rpc.py` & `tryton-7.2.1/tryton/rpc.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/tests/test_common.py` & `tryton-7.2.1/tryton/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/tests/test_common_domain_parser.py` & `tryton-7.2.1/tryton/tests/test_common_domain_parser.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/tests/test_common_selection.py` & `tryton-7.2.1/tryton/tests/test_common_selection.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/tests/test_common_timedelta.py` & `tryton-7.2.1/tryton/tests/test_common_timedelta.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton/translate.py` & `tryton-7.2.1/tryton/translate.py`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton.desktop` & `tryton-7.2.1/tryton.desktop`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/tryton.egg-info/PKG-INFO` & `tryton-7.2.1/tryton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tryton
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton desktop client
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `tryton-7.2.0/tryton.egg-info/SOURCES.txt` & `tryton-7.2.1/tryton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tryton-7.2.0/win32/gtk-3.0/gdk-pixbuf.loaders` & `tryton-7.2.1/win32/gtk-3.0/gdk-pixbuf.loaders`

 * *Files identical despite different names*

