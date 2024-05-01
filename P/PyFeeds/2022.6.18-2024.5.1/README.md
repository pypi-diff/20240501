# Comparing `tmp/PyFeeds-2022.6.18.tar.gz` & `tmp/pyfeeds-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFeeds-2022.6.18.tar", last modified: Sat Jun 18 13:12:18 2022, max compression
+gzip compressed data, was "pyfeeds-2024.5.1.tar", last modified: Wed May  1 14:58:19 2024, max compression
```

## Comparing `PyFeeds-2022.6.18.tar` & `pyfeeds-2024.5.1.tar`

### file list

```diff
@@ -1,128 +1,120 @@
-drwxr-xr-x   0 flo       (1000) flo       (1000)        0 2022-06-18 13:12:18.679033 PyFeeds-2022.6.18/
--rw-r--r--   0 flo       (1000) flo       (1000)    34520 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/LICENSE
--rw-r--r--   0 flo       (1000) flo       (1000)      123 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/MANIFEST.in
--rw-r--r--   0 flo       (1000) flo       (1000)     7563 2022-06-18 13:12:18.679033 PyFeeds-2022.6.18/PKG-INFO
-drwxr-xr-x   0 flo       (1000) flo       (1000)        0 2022-06-18 13:12:18.669033 PyFeeds-2022.6.18/PyFeeds.egg-info/
--rw-r--r--   0 flo       (1000) flo       (1000)     7563 2022-06-18 13:12:18.000000 PyFeeds-2022.6.18/PyFeeds.egg-info/PKG-INFO
--rw-r--r--   0 flo       (1000) flo       (1000)     3149 2022-06-18 13:12:18.000000 PyFeeds-2022.6.18/PyFeeds.egg-info/SOURCES.txt
--rw-r--r--   0 flo       (1000) flo       (1000)        1 2022-06-18 13:12:18.000000 PyFeeds-2022.6.18/PyFeeds.egg-info/dependency_links.txt
--rw-r--r--   0 flo       (1000) flo       (1000)       42 2022-06-18 13:12:18.000000 PyFeeds-2022.6.18/PyFeeds.egg-info/entry_points.txt
--rw-r--r--   0 flo       (1000) flo       (1000)      203 2022-06-18 13:12:18.000000 PyFeeds-2022.6.18/PyFeeds.egg-info/requires.txt
--rw-r--r--   0 flo       (1000) flo       (1000)        6 2022-06-18 13:12:18.000000 PyFeeds-2022.6.18/PyFeeds.egg-info/top_level.txt
--rw-r--r--   0 flo       (1000) flo       (1000)     6638 2021-08-08 06:10:48.000000 PyFeeds-2022.6.18/README.rst
-drwxr-xr-x   0 flo       (1000) flo       (1000)        0 2022-06-18 13:12:18.669033 PyFeeds-2022.6.18/docs/
--rw-r--r--   0 flo       (1000) flo       (1000)      605 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/Makefile
--rw-r--r--   0 flo       (1000) flo       (1000)     7189 2020-05-16 09:54:13.000000 PyFeeds-2022.6.18/docs/api.rst
--rw-r--r--   0 flo       (1000) flo       (1000)     5299 2022-06-18 13:06:28.000000 PyFeeds-2022.6.18/docs/conf.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2495 2020-05-16 09:47:11.000000 PyFeeds-2022.6.18/docs/configure.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      590 2021-08-08 06:10:48.000000 PyFeeds-2022.6.18/docs/contribute.rst
--rw-r--r--   0 flo       (1000) flo       (1000)     8498 2021-08-08 17:13:55.000000 PyFeeds-2022.6.18/docs/development.rst
--rw-r--r--   0 flo       (1000) flo       (1000)     1266 2022-06-18 13:02:39.000000 PyFeeds-2022.6.18/docs/docker.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      598 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/docs/get.rst
--rw-r--r--   0 flo       (1000) flo       (1000)     2288 2020-05-16 09:54:13.000000 PyFeeds-2022.6.18/docs/index.rst
--rw-r--r--   0 flo       (1000) flo       (1000)       47 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/license.rst
--rw-r--r--   0 flo       (1000) flo       (1000)     1001 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/quickstart.rst
-drwxr-xr-x   0 flo       (1000) flo       (1000)        0 2022-06-18 13:12:18.672366 PyFeeds-2022.6.18/docs/spiders/
--rw-r--r--   0 flo       (1000) flo       (1000)      295 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/addendum.org.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      342 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/ak.ciando.com.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      852 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/arstechnica.com.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      273 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/atv.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      489 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/biblioweb.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      275 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/cbird.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      687 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/docs/spiders/derstandard.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      296 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/docs/spiders/dietiwag.org.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      614 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/docs/spiders/economist.com.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      921 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/docs/spiders/falter.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      647 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/docs/spiders/ft.com.rst
--rw-r--r--   0 flo       (1000) flo       (1000)     1575 2020-05-16 09:47:11.000000 PyFeeds-2022.6.18/docs/spiders/generic.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      320 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/indiehackers.com.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      290 2022-06-18 13:02:39.000000 PyFeeds-2022.6.18/docs/spiders/keycloak.org.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      502 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/konsument.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      757 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/docs/spiders/kurier.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      253 2021-08-08 06:16:51.000000 PyFeeds-2022.6.18/docs/spiders/lbg.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      669 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/lwn.net.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      654 2021-08-08 17:13:17.000000 PyFeeds-2022.6.18/docs/spiders/momoxfashion.com.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      622 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/nachrichten.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      299 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/docs/spiders/npr.org.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      293 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/oe1.orf.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      857 2021-08-08 06:13:39.000000 PyFeeds-2022.6.18/docs/spiders/orf.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      275 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/profil.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      290 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/puls4.com.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      650 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/docs/spiders/python-patterns.guide.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      626 2020-06-14 08:00:17.000000 PyFeeds-2022.6.18/docs/spiders/riskommunal.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      311 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/docs/spiders/servustv.com.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      626 2020-05-16 07:38:32.000000 PyFeeds-2022.6.18/docs/spiders/spotify.com.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      312 2018-09-14 15:08:13.000000 PyFeeds-2022.6.18/docs/spiders/theoatmeal.com.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      530 2020-05-21 09:52:14.000000 PyFeeds-2022.6.18/docs/spiders/tinyletter.com.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      269 2020-07-12 09:15:21.000000 PyFeeds-2022.6.18/docs/spiders/trend.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      305 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/docs/spiders/tuwien.ac.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      311 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/tvthek.orf.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      538 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/uebermedien.de.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      270 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/usenix.org.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      341 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/verbraucherrecht.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      423 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/vice.com.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      318 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/wienerlinien.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      624 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/docs/spiders/wienerzeitung.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)      310 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/docs/spiders/zeit.diebin.at.rst
--rw-r--r--   0 flo       (1000) flo       (1000)     1261 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/docs/spiders.rst
-drwxr-xr-x   0 flo       (1000) flo       (1000)        0 2022-06-18 13:12:18.675699 PyFeeds-2022.6.18/feeds/
--rw-r--r--   0 flo       (1000) flo       (1000)       26 2022-06-18 13:06:28.000000 PyFeeds-2022.6.18/feeds/__init__.py
--rw-r--r--   0 flo       (1000) flo       (1000)     7744 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/cache.py
--rw-r--r--   0 flo       (1000) flo       (1000)     3904 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/cli.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2086 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/feeds/default_settings.py
--rw-r--r--   0 flo       (1000) flo       (1000)      461 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/feeds/downloadermiddlewares.py
--rw-r--r--   0 flo       (1000) flo       (1000)      267 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/feeds/exceptions.py
--rw-r--r--   0 flo       (1000) flo       (1000)     8077 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/exporters.py
--rw-r--r--   0 flo       (1000) flo       (1000)     1308 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/feeds/items.py
--rw-r--r--   0 flo       (1000) flo       (1000)    14459 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/loaders.py
--rw-r--r--   0 flo       (1000) flo       (1000)     3388 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/pipelines.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2079 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/settings.py
--rw-r--r--   0 flo       (1000) flo       (1000)     3283 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spidermiddlewares.py
-drwxr-xr-x   0 flo       (1000) flo       (1000)        0 2022-06-18 13:12:18.679033 PyFeeds-2022.6.18/feeds/spiders/
--rw-r--r--   0 flo       (1000) flo       (1000)     1150 2020-05-16 07:38:32.000000 PyFeeds-2022.6.18/feeds/spiders/__init__.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2616 2020-09-25 18:17:45.000000 PyFeeds-2022.6.18/feeds/spiders/addendum_org.py
--rw-r--r--   0 flo       (1000) flo       (1000)     1794 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/ak_ciando_com.py
--rw-r--r--   0 flo       (1000) flo       (1000)     3501 2022-06-11 11:36:37.000000 PyFeeds-2022.6.18/feeds/spiders/arstechnica_com.py
--rw-r--r--   0 flo       (1000) flo       (1000)     1905 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/atv_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     3591 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/biblioweb_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     1334 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/cbird_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     6458 2021-08-08 06:10:48.000000 PyFeeds-2022.6.18/feeds/spiders/derstandard_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2556 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/dietiwag_org.py
--rw-r--r--   0 flo       (1000) flo       (1000)     3300 2021-08-08 06:10:48.000000 PyFeeds-2022.6.18/feeds/spiders/economist_com.py
--rw-r--r--   0 flo       (1000) flo       (1000)    11414 2022-06-11 11:36:37.000000 PyFeeds-2022.6.18/feeds/spiders/falter_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     3129 2022-06-11 11:36:37.000000 PyFeeds-2022.6.18/feeds/spiders/ft_com.py
--rw-r--r--   0 flo       (1000) flo       (1000)     3892 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/generic.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2474 2020-05-16 07:38:32.000000 PyFeeds-2022.6.18/feeds/spiders/indiehackers_com.py
--rw-r--r--   0 flo       (1000) flo       (1000)     1258 2022-06-18 13:02:39.000000 PyFeeds-2022.6.18/feeds/spiders/keycloak_org.py
--rw-r--r--   0 flo       (1000) flo       (1000)     3489 2022-06-18 13:02:39.000000 PyFeeds-2022.6.18/feeds/spiders/konsument_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     7944 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/kurier_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     1716 2020-06-14 08:00:17.000000 PyFeeds-2022.6.18/feeds/spiders/lbg_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     9643 2022-06-11 11:36:37.000000 PyFeeds-2022.6.18/feeds/spiders/lwn_net.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2521 2021-08-08 17:13:17.000000 PyFeeds-2022.6.18/feeds/spiders/momoxfashion_com.py
--rw-r--r--   0 flo       (1000) flo       (1000)     4935 2022-06-11 11:36:37.000000 PyFeeds-2022.6.18/feeds/spiders/nachrichten_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2811 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/npr_org.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2827 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/oe1_orf_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)    11896 2022-06-11 11:36:37.000000 PyFeeds-2022.6.18/feeds/spiders/orf_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)      635 2020-09-25 17:49:46.000000 PyFeeds-2022.6.18/feeds/spiders/profil_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2653 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/puls4_com.py
--rw-r--r--   0 flo       (1000) flo       (1000)     1247 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/python_patterns_guide.py
--rw-r--r--   0 flo       (1000) flo       (1000)     3628 2020-09-25 18:17:46.000000 PyFeeds-2022.6.18/feeds/spiders/riskommunal.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2631 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/servustv_com.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2218 2020-05-16 07:38:32.000000 PyFeeds-2022.6.18/feeds/spiders/spotify_com.py
--rw-r--r--   0 flo       (1000) flo       (1000)     1807 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/theoatmeal_com.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2388 2020-09-25 18:17:46.000000 PyFeeds-2022.6.18/feeds/spiders/tinyletter_com.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2750 2022-06-11 11:36:37.000000 PyFeeds-2022.6.18/feeds/spiders/trend_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2383 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/tuwien_ac_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     5648 2022-06-11 11:36:37.000000 PyFeeds-2022.6.18/feeds/spiders/tvthek_orf_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     4498 2022-06-11 11:36:37.000000 PyFeeds-2022.6.18/feeds/spiders/uebermedien_de.py
--rw-r--r--   0 flo       (1000) flo       (1000)     2566 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/usenix_org.py
--rw-r--r--   0 flo       (1000) flo       (1000)     1387 2022-06-18 13:02:39.000000 PyFeeds-2022.6.18/feeds/spiders/verbraucherrecht_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     3163 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/vice_com.py
--rw-r--r--   0 flo       (1000) flo       (1000)     1954 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/wienerlinien_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     4058 2021-08-08 06:10:48.000000 PyFeeds-2022.6.18/feeds/spiders/wienerzeitung_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)     1015 2021-03-21 08:31:01.000000 PyFeeds-2022.6.18/feeds/spiders/zeitdiebin_at.py
--rw-r--r--   0 flo       (1000) flo       (1000)      482 2020-05-15 12:27:52.000000 PyFeeds-2022.6.18/feeds/utils.py
--rw-r--r--   0 flo       (1000) flo       (1000)     3649 2021-08-08 17:13:17.000000 PyFeeds-2022.6.18/feeds.cfg.dist
--rw-r--r--   0 flo       (1000) flo       (1000)      118 2018-08-21 19:44:42.000000 PyFeeds-2022.6.18/scrapy.cfg
--rw-r--r--   0 flo       (1000) flo       (1000)       38 2022-06-18 13:12:18.679033 PyFeeds-2022.6.18/setup.cfg
--rw-r--r--   0 flo       (1000) flo       (1000)     1599 2022-06-18 13:06:28.000000 PyFeeds-2022.6.18/setup.py
+drwxr-xr-x   0 flo       (1000) flo       (1000)        0 2024-05-01 14:58:19.333079 pyfeeds-2024.5.1/
+-rw-r--r--   0 flo       (1000) flo       (1000)    34520 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/LICENSE
+-rw-r--r--   0 flo       (1000) flo       (1000)      123 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/MANIFEST.in
+-rw-r--r--   0 flo       (1000) flo       (1000)     7835 2024-05-01 14:58:19.333079 pyfeeds-2024.5.1/PKG-INFO
+drwxr-xr-x   0 flo       (1000) flo       (1000)        0 2024-05-01 14:58:19.333079 pyfeeds-2024.5.1/PyFeeds.egg-info/
+-rw-r--r--   0 flo       (1000) flo       (1000)     7835 2024-05-01 14:58:19.000000 pyfeeds-2024.5.1/PyFeeds.egg-info/PKG-INFO
+-rw-r--r--   0 flo       (1000) flo       (1000)     2855 2024-05-01 14:58:19.000000 pyfeeds-2024.5.1/PyFeeds.egg-info/SOURCES.txt
+-rw-r--r--   0 flo       (1000) flo       (1000)        1 2024-05-01 14:58:19.000000 pyfeeds-2024.5.1/PyFeeds.egg-info/dependency_links.txt
+-rw-r--r--   0 flo       (1000) flo       (1000)       41 2024-05-01 14:58:19.000000 pyfeeds-2024.5.1/PyFeeds.egg-info/entry_points.txt
+-rw-r--r--   0 flo       (1000) flo       (1000)      173 2024-05-01 14:58:19.000000 pyfeeds-2024.5.1/PyFeeds.egg-info/requires.txt
+-rw-r--r--   0 flo       (1000) flo       (1000)        6 2024-05-01 14:58:19.000000 pyfeeds-2024.5.1/PyFeeds.egg-info/top_level.txt
+-rw-r--r--   0 flo       (1000) flo       (1000)     6493 2024-04-28 07:31:02.000000 pyfeeds-2024.5.1/README.rst
+drwxr-xr-x   0 flo       (1000) flo       (1000)        0 2024-05-01 14:58:19.313079 pyfeeds-2024.5.1/docs/
+-rw-r--r--   0 flo       (1000) flo       (1000)      605 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/Makefile
+-rw-r--r--   0 flo       (1000) flo       (1000)     7189 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/docs/api.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)     5297 2024-05-01 14:57:12.000000 pyfeeds-2024.5.1/docs/conf.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     2495 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/docs/configure.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)     1005 2022-07-27 17:47:12.000000 pyfeeds-2024.5.1/docs/contribute.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)     8366 2024-05-01 14:57:12.000000 pyfeeds-2024.5.1/docs/development.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)     1266 2022-07-27 17:47:12.000000 pyfeeds-2024.5.1/docs/docker.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      598 2024-04-25 18:23:30.000000 pyfeeds-2024.5.1/docs/get.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)     2143 2024-04-27 19:38:31.000000 pyfeeds-2024.5.1/docs/index.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)       47 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/license.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)     1001 2018-09-11 17:53:18.000000 pyfeeds-2024.5.1/docs/quickstart.rst
+drwxr-xr-x   0 flo       (1000) flo       (1000)        0 2024-05-01 14:58:19.319746 pyfeeds-2024.5.1/docs/spiders/
+-rw-r--r--   0 flo       (1000) flo       (1000)      852 2018-09-11 17:53:18.000000 pyfeeds-2024.5.1/docs/spiders/arstechnica.com.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      273 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/spiders/atv.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      489 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/spiders/biblioweb.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      275 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/spiders/cbird.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      687 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/docs/spiders/derstandard.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      614 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/docs/spiders/economist.com.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)     1024 2023-01-13 16:37:35.000000 pyfeeds-2024.5.1/docs/spiders/falter.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      647 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/docs/spiders/ft.com.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      583 2024-05-01 14:57:12.000000 pyfeeds-2024.5.1/docs/spiders/gem2go.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)     1575 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/docs/spiders/generic.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      320 2018-09-11 17:53:18.000000 pyfeeds-2024.5.1/docs/spiders/indiehackers.com.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      502 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/spiders/konsument.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      757 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/docs/spiders/kurier.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      253 2022-05-10 18:00:07.000000 pyfeeds-2024.5.1/docs/spiders/lbg.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      669 2018-09-11 17:53:18.000000 pyfeeds-2024.5.1/docs/spiders/lwn.net.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      654 2022-05-10 18:00:07.000000 pyfeeds-2024.5.1/docs/spiders/momoxfashion.com.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      622 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/spiders/nachrichten.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      299 2020-12-09 20:12:54.000000 pyfeeds-2024.5.1/docs/spiders/npr.org.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      293 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/spiders/oe1.orf.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      857 2022-05-10 18:00:07.000000 pyfeeds-2024.5.1/docs/spiders/orf.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      275 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/spiders/profil.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      290 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/spiders/puls4.com.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      650 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/docs/spiders/python-patterns.guide.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      311 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/docs/spiders/servustv.com.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      626 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/docs/spiders/spotify.com.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      312 2018-09-12 15:40:22.000000 pyfeeds-2024.5.1/docs/spiders/theoatmeal.com.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      269 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/docs/spiders/trend.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      305 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/docs/spiders/tuwien.ac.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      311 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/spiders/tvthek.orf.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      538 2018-09-11 17:53:18.000000 pyfeeds-2024.5.1/docs/spiders/uebermedien.de.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      321 2024-04-27 19:38:31.000000 pyfeeds-2024.5.1/docs/spiders/usenix.org.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      341 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/spiders/verbraucherrecht.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      423 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/spiders/vice.com.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      318 2018-08-21 10:17:24.000000 pyfeeds-2024.5.1/docs/spiders/wienerlinien.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      624 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/docs/spiders/wienerzeitung.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)      310 2018-09-11 17:53:18.000000 pyfeeds-2024.5.1/docs/spiders/zeit.diebin.at.rst
+-rw-r--r--   0 flo       (1000) flo       (1000)     1261 2020-12-09 20:12:54.000000 pyfeeds-2024.5.1/docs/spiders.rst
+drwxr-xr-x   0 flo       (1000) flo       (1000)        0 2024-05-01 14:58:19.323079 pyfeeds-2024.5.1/feeds/
+-rw-r--r--   0 flo       (1000) flo       (1000)       25 2024-05-01 14:57:12.000000 pyfeeds-2024.5.1/feeds/__init__.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     7710 2024-04-25 17:36:22.000000 pyfeeds-2024.5.1/feeds/cache.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     3904 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/cli.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     2280 2024-04-25 17:36:22.000000 pyfeeds-2024.5.1/feeds/default_settings.py
+-rw-r--r--   0 flo       (1000) flo       (1000)      461 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/feeds/downloadermiddlewares.py
+-rw-r--r--   0 flo       (1000) flo       (1000)      267 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/feeds/exceptions.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     8077 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/exporters.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     1308 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/feeds/items.py
+-rw-r--r--   0 flo       (1000) flo       (1000)    14459 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/loaders.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     3388 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/pipelines.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     2079 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/settings.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     3251 2024-04-25 17:36:22.000000 pyfeeds-2024.5.1/feeds/spidermiddlewares.py
+drwxr-xr-x   0 flo       (1000) flo       (1000)        0 2024-05-01 14:58:19.333079 pyfeeds-2024.5.1/feeds/spiders/
+-rw-r--r--   0 flo       (1000) flo       (1000)     1150 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/feeds/spiders/__init__.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     3501 2022-05-10 18:00:07.000000 pyfeeds-2024.5.1/feeds/spiders/arstechnica_com.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     1905 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/atv_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     3591 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/biblioweb_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     1334 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/cbird_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     6458 2022-05-10 18:00:07.000000 pyfeeds-2024.5.1/feeds/spiders/derstandard_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     3056 2022-07-27 17:47:12.000000 pyfeeds-2024.5.1/feeds/spiders/economist_com.py
+-rw-r--r--   0 flo       (1000) flo       (1000)    13307 2023-01-13 16:37:35.000000 pyfeeds-2024.5.1/feeds/spiders/falter_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     3129 2022-05-10 18:00:07.000000 pyfeeds-2024.5.1/feeds/spiders/ft_com.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     4095 2024-05-01 14:57:12.000000 pyfeeds-2024.5.1/feeds/spiders/gem2go.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     3892 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/generic.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     2474 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/feeds/spiders/indiehackers_com.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     3489 2022-07-27 17:47:12.000000 pyfeeds-2024.5.1/feeds/spiders/konsument_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     7944 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/kurier_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     1716 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/feeds/spiders/lbg_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     9643 2022-05-10 18:00:07.000000 pyfeeds-2024.5.1/feeds/spiders/lwn_net.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     2559 2022-07-27 17:47:12.000000 pyfeeds-2024.5.1/feeds/spiders/momoxfashion_com.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     4935 2022-05-10 18:00:07.000000 pyfeeds-2024.5.1/feeds/spiders/nachrichten_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     2811 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/npr_org.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     2827 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/oe1_orf_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)    11896 2022-05-10 18:00:07.000000 pyfeeds-2024.5.1/feeds/spiders/orf_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)      635 2020-08-08 12:33:13.000000 pyfeeds-2024.5.1/feeds/spiders/profil_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     2653 2024-04-27 19:38:35.000000 pyfeeds-2024.5.1/feeds/spiders/puls4_com.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     1247 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/python_patterns_guide.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     2631 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/servustv_com.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     2218 2020-07-20 10:59:30.000000 pyfeeds-2024.5.1/feeds/spiders/spotify_com.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     1807 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/theoatmeal_com.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     2750 2022-05-10 18:00:07.000000 pyfeeds-2024.5.1/feeds/spiders/trend_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     2383 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/tuwien_ac_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     5609 2024-04-25 17:35:03.000000 pyfeeds-2024.5.1/feeds/spiders/tvthek_orf_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     4498 2022-05-10 18:00:07.000000 pyfeeds-2024.5.1/feeds/spiders/uebermedien_de.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     1359 2024-04-27 19:38:31.000000 pyfeeds-2024.5.1/feeds/spiders/usenix_org.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     1387 2022-07-27 17:47:12.000000 pyfeeds-2024.5.1/feeds/spiders/verbraucherrecht_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     3163 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/vice_com.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     1954 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/wienerlinien_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     4058 2022-05-10 18:00:07.000000 pyfeeds-2024.5.1/feeds/spiders/wienerzeitung_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     1015 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/feeds/spiders/zeitdiebin_at.py
+-rw-r--r--   0 flo       (1000) flo       (1000)      482 2024-04-28 09:03:08.000000 pyfeeds-2024.5.1/feeds/utils.py
+-rw-r--r--   0 flo       (1000) flo       (1000)     3601 2024-05-01 14:57:12.000000 pyfeeds-2024.5.1/feeds.cfg.dist
+-rw-r--r--   0 flo       (1000) flo       (1000)       95 2024-04-25 17:36:22.000000 pyfeeds-2024.5.1/scrapy.cfg
+-rw-r--r--   0 flo       (1000) flo       (1000)       38 2024-05-01 14:58:19.333079 pyfeeds-2024.5.1/setup.cfg
+-rw-r--r--   0 flo       (1000) flo       (1000)     1578 2024-05-01 14:57:12.000000 pyfeeds-2024.5.1/setup.py
+drwxr-xr-x   0 flo       (1000) flo       (1000)        0 2024-05-01 14:58:19.333079 pyfeeds-2024.5.1/tests/
+-rw-r--r--   0 flo       (1000) flo       (1000)      400 2021-02-02 17:46:19.000000 pyfeeds-2024.5.1/tests/test_loaders.py
```

### Comparing `PyFeeds-2022.6.18/LICENSE` & `pyfeeds-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/PKG-INFO` & `pyfeeds-2024.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 Metadata-Version: 2.1
 Name: PyFeeds
-Version: 2022.6.18
+Version: 2024.5.1
 Summary: DIY Atom feeds in times of social media and paywalls
 Home-page: https://github.com/PyFeeds/PyFeeds
 Author: Florian Preinstorfer, Lukas Anzinger
 Author-email: florian@nblock.org, lukas@lukasanzinger.at
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Scrapy
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: dateparser
+Requires-Dist: feedparser
+Requires-Dist: itemloaders
+Requires-Dist: lxml[html_clean]
+Requires-Dist: python-dateutil
+Requires-Dist: pyxdg
+Requires-Dist: readability-lxml
+Requires-Dist: scrapy
+Requires-Dist: scrapy-inline-requests
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
 
 Feeds
 =====
 
 |pypi| |support| |licence|
 
 |readthedocs|
@@ -92,15 +104,15 @@
 
 .. code-block:: bash
 
    $ pip install https://github.com/pyfeeds/pyfeeds/archive/master.tar.gz
 
 After installation ``feeds`` is available in your virtual environment.
 
-Feeds supports Python 3.7+.
+Feeds supports Python 3.8+.
 
 Quickstart
 ----------
 
 * List all available spiders::
 
   $ feeds list
@@ -139,16 +151,14 @@
   but in "real-time", i.e. on (HTTP) request.
 * `Full-Text RSS <https://bitbucket.org/fivefilters/full-text-rss>`_ converts
   feeds to contain the full article and not only a teaser based on heuristics
   and rules. Feeds are converted in "real-time", i.e. on request basis.
 * `f43.me <https://github.com/j0k3r/f43.me>`_ converts feeds to contain the
   full article and also improves articles by adding links to the comment
   sections of Hacker News and Reddit. Feeds are converted periodically.
-* `python-ftr <https://github.com/1flow/python-ftr>`_ is a library to extract
-  content from pages. A partial reimplementation of Full-Text RSS.
 
 How to contribute
 -----------------
 
 Issues
 ~~~~~~
 
@@ -199,9 +209,7 @@
 .. |readthedocs| image:: https://img.shields.io/readthedocs/pyfeeds/latest.svg?style=flat-square&label=Read%20the%20Docs
    :alt: Read the documentation at https://pyfeeds.readthedocs.io/en/latest/
    :target: https://pyfeeds.readthedocs.io/en/latest/
 
 .. |pyfeedsci| image:: https://github.com/PyFeeds/PyFeeds/workflows/PyFeeds%20CI/badge.svg
     :target: https://github.com/PyFeeds/PyFeeds/actions?query=workflow%3A%22PyFeeds+CI%22
     :alt: GitHub PyFeeds CI
-
-
```

### Comparing `PyFeeds-2022.6.18/PyFeeds.egg-info/PKG-INFO` & `pyfeeds-2024.5.1/PyFeeds.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 Metadata-Version: 2.1
 Name: PyFeeds
-Version: 2022.6.18
+Version: 2024.5.1
 Summary: DIY Atom feeds in times of social media and paywalls
 Home-page: https://github.com/PyFeeds/PyFeeds
 Author: Florian Preinstorfer, Lukas Anzinger
 Author-email: florian@nblock.org, lukas@lukasanzinger.at
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Scrapy
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: dateparser
+Requires-Dist: feedparser
+Requires-Dist: itemloaders
+Requires-Dist: lxml[html_clean]
+Requires-Dist: python-dateutil
+Requires-Dist: pyxdg
+Requires-Dist: readability-lxml
+Requires-Dist: scrapy
+Requires-Dist: scrapy-inline-requests
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
 
 Feeds
 =====
 
 |pypi| |support| |licence|
 
 |readthedocs|
@@ -92,15 +104,15 @@
 
 .. code-block:: bash
 
    $ pip install https://github.com/pyfeeds/pyfeeds/archive/master.tar.gz
 
 After installation ``feeds`` is available in your virtual environment.
 
-Feeds supports Python 3.7+.
+Feeds supports Python 3.8+.
 
 Quickstart
 ----------
 
 * List all available spiders::
 
   $ feeds list
@@ -139,16 +151,14 @@
   but in "real-time", i.e. on (HTTP) request.
 * `Full-Text RSS <https://bitbucket.org/fivefilters/full-text-rss>`_ converts
   feeds to contain the full article and not only a teaser based on heuristics
   and rules. Feeds are converted in "real-time", i.e. on request basis.
 * `f43.me <https://github.com/j0k3r/f43.me>`_ converts feeds to contain the
   full article and also improves articles by adding links to the comment
   sections of Hacker News and Reddit. Feeds are converted periodically.
-* `python-ftr <https://github.com/1flow/python-ftr>`_ is a library to extract
-  content from pages. A partial reimplementation of Full-Text RSS.
 
 How to contribute
 -----------------
 
 Issues
 ~~~~~~
 
@@ -199,9 +209,7 @@
 .. |readthedocs| image:: https://img.shields.io/readthedocs/pyfeeds/latest.svg?style=flat-square&label=Read%20the%20Docs
    :alt: Read the documentation at https://pyfeeds.readthedocs.io/en/latest/
    :target: https://pyfeeds.readthedocs.io/en/latest/
 
 .. |pyfeedsci| image:: https://github.com/PyFeeds/PyFeeds/workflows/PyFeeds%20CI/badge.svg
     :target: https://github.com/PyFeeds/PyFeeds/actions?query=workflow%3A%22PyFeeds+CI%22
     :alt: GitHub PyFeeds CI
-
-
```

### Comparing `PyFeeds-2022.6.18/PyFeeds.egg-info/SOURCES.txt` & `pyfeeds-2024.5.1/PyFeeds.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,45 +18,40 @@
 docs/development.rst
 docs/docker.rst
 docs/get.rst
 docs/index.rst
 docs/license.rst
 docs/quickstart.rst
 docs/spiders.rst
-docs/spiders/addendum.org.rst
-docs/spiders/ak.ciando.com.rst
 docs/spiders/arstechnica.com.rst
 docs/spiders/atv.at.rst
 docs/spiders/biblioweb.at.rst
 docs/spiders/cbird.at.rst
 docs/spiders/derstandard.at.rst
-docs/spiders/dietiwag.org.rst
 docs/spiders/economist.com.rst
 docs/spiders/falter.at.rst
 docs/spiders/ft.com.rst
+docs/spiders/gem2go.rst
 docs/spiders/generic.rst
 docs/spiders/indiehackers.com.rst
-docs/spiders/keycloak.org.rst
 docs/spiders/konsument.at.rst
 docs/spiders/kurier.at.rst
 docs/spiders/lbg.at.rst
 docs/spiders/lwn.net.rst
 docs/spiders/momoxfashion.com.rst
 docs/spiders/nachrichten.at.rst
 docs/spiders/npr.org.rst
 docs/spiders/oe1.orf.at.rst
 docs/spiders/orf.at.rst
 docs/spiders/profil.at.rst
 docs/spiders/puls4.com.rst
 docs/spiders/python-patterns.guide.rst
-docs/spiders/riskommunal.rst
 docs/spiders/servustv.com.rst
 docs/spiders/spotify.com.rst
 docs/spiders/theoatmeal.com.rst
-docs/spiders/tinyletter.com.rst
 docs/spiders/trend.at.rst
 docs/spiders/tuwien.ac.at.rst
 docs/spiders/tvthek.orf.at.rst
 docs/spiders/uebermedien.de.rst
 docs/spiders/usenix.org.rst
 docs/spiders/verbraucherrecht.at.rst
 docs/spiders/vice.com.rst
@@ -73,48 +68,44 @@
 feeds/items.py
 feeds/loaders.py
 feeds/pipelines.py
 feeds/settings.py
 feeds/spidermiddlewares.py
 feeds/utils.py
 feeds/spiders/__init__.py
-feeds/spiders/addendum_org.py
-feeds/spiders/ak_ciando_com.py
 feeds/spiders/arstechnica_com.py
 feeds/spiders/atv_at.py
 feeds/spiders/biblioweb_at.py
 feeds/spiders/cbird_at.py
 feeds/spiders/derstandard_at.py
-feeds/spiders/dietiwag_org.py
 feeds/spiders/economist_com.py
 feeds/spiders/falter_at.py
 feeds/spiders/ft_com.py
+feeds/spiders/gem2go.py
 feeds/spiders/generic.py
 feeds/spiders/indiehackers_com.py
-feeds/spiders/keycloak_org.py
 feeds/spiders/konsument_at.py
 feeds/spiders/kurier_at.py
 feeds/spiders/lbg_at.py
 feeds/spiders/lwn_net.py
 feeds/spiders/momoxfashion_com.py
 feeds/spiders/nachrichten_at.py
 feeds/spiders/npr_org.py
 feeds/spiders/oe1_orf_at.py
 feeds/spiders/orf_at.py
 feeds/spiders/profil_at.py
 feeds/spiders/puls4_com.py
 feeds/spiders/python_patterns_guide.py
-feeds/spiders/riskommunal.py
 feeds/spiders/servustv_com.py
 feeds/spiders/spotify_com.py
 feeds/spiders/theoatmeal_com.py
-feeds/spiders/tinyletter_com.py
 feeds/spiders/trend_at.py
 feeds/spiders/tuwien_ac_at.py
 feeds/spiders/tvthek_orf_at.py
 feeds/spiders/uebermedien_de.py
 feeds/spiders/usenix_org.py
 feeds/spiders/verbraucherrecht_at.py
 feeds/spiders/vice_com.py
 feeds/spiders/wienerlinien_at.py
 feeds/spiders/wienerzeitung_at.py
-feeds/spiders/zeitdiebin_at.py
+feeds/spiders/zeitdiebin_at.py
+tests/test_loaders.py
```

### Comparing `PyFeeds-2022.6.18/README.rst` & `pyfeeds-2024.5.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 .. code-block:: bash
 
    $ pip install https://github.com/pyfeeds/pyfeeds/archive/master.tar.gz
 
 After installation ``feeds`` is available in your virtual environment.
 
-Feeds supports Python 3.7+.
+Feeds supports Python 3.8+.
 
 Quickstart
 ----------
 
 * List all available spiders::
 
   $ feeds list
@@ -114,16 +114,14 @@
   but in "real-time", i.e. on (HTTP) request.
 * `Full-Text RSS <https://bitbucket.org/fivefilters/full-text-rss>`_ converts
   feeds to contain the full article and not only a teaser based on heuristics
   and rules. Feeds are converted in "real-time", i.e. on request basis.
 * `f43.me <https://github.com/j0k3r/f43.me>`_ converts feeds to contain the
   full article and also improves articles by adding links to the comment
   sections of Hacker News and Reddit. Feeds are converted periodically.
-* `python-ftr <https://github.com/1flow/python-ftr>`_ is a library to extract
-  content from pages. A partial reimplementation of Full-Text RSS.
 
 How to contribute
 -----------------
 
 Issues
 ~~~~~~
```

### Comparing `PyFeeds-2022.6.18/docs/Makefile` & `pyfeeds-2024.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/api.rst` & `pyfeeds-2024.5.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/conf.py` & `pyfeeds-2024.5.1/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,25 +43,25 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "feeds"
-copyright = "2022, Florian Preinstorfer, Lukas Anzinger"
+copyright = "2024, Florian Preinstorfer, Lukas Anzinger"
 author = "Florian Preinstorfer, Lukas Anzinger"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "2022.6.18"
+version = "2024.5.1"
 # The full version, including alpha/beta/rc tags.
-release = "2022.6.18"
+release = "2024.5.1"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
```

### Comparing `PyFeeds-2022.6.18/docs/configure.rst` & `pyfeeds-2024.5.1/docs/configure.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/development.rst` & `pyfeeds-2024.5.1/docs/development.rst`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,14 @@
 Custom extraction
 ~~~~~~~~~~~~~~~~~
 These spiders take an existing RSS feed and inline the article content while
 cleaning up the content (removing share buttons, etc.):
 
   * :ref:`spider_arstechnica.com`
   * :ref:`spider_derstandard.at`
-  * :ref:`spider_dietiwag.org`
   * :ref:`spider_ft.com`
   * :ref:`spider_lwn.net`
   * :ref:`spider_orf.at`
   * :ref:`spider_profil.at`
 
 Paywalled content
 ~~~~~~~~~~~~~~~~~
@@ -123,15 +122,14 @@
 Some websites don't offer any feed at all. In such cases we have to find an
 efficient way to detect new content and extract it.
 
 Utilizing an API
 ~~~~~~~~~~~~~~~~
 Some use a REST API which we can use to fetch the content.
 
-  * :ref:`spider_addendum.org`
   * :ref:`spider_falter.at`
   * :ref:`spider_indiehackers.com`
   * :ref:`spider_kurier.at`
   * :ref:`spider_oe1.orf.at`
   * :ref:`spider_tvthek.orf.at`
   * :ref:`spider_vice.com`
 
@@ -142,26 +140,24 @@
   * :ref:`spider_trend.at`
 
 Custom extraction
 ~~~~~~~~~~~~~~~~~
 The last resort is to find a page that lists the newest articles and start
 scraping from there.
 
-  * :ref:`spider_ak.ciando.com`
   * :ref:`spider_atv.at`
   * :ref:`spider_biblioweb.at`
   * :ref:`spider_cbird.at`
   * :ref:`spider_economist.com`
   * :ref:`spider_lbg.at`
   * :ref:`spider_npr.org`
   * :ref:`spider_puls4.com`
   * :ref:`spider_python-patterns.guide`
-  * :ref:`spider_riskommunal`
+  * :ref:`spider_gem2go`
   * :ref:`spider_servustv.com`
-  * :ref:`spider_tinyletter.com`
   * :ref:`spider_tuwien.ac.at`
   * :ref:`spider_momoxfashion.com`
   * :ref:`spider_usenix.org`
   * :ref:`spider_verbraucherrecht.at`
   * :ref:`spider_wienerlinien.at`
   * :ref:`spider_zeit.diebin.at`
```

### Comparing `PyFeeds-2022.6.18/docs/docker.rst` & `pyfeeds-2024.5.1/docs/docker.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/get.rst` & `pyfeeds-2024.5.1/docs/get.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 
 .. code-block:: bash
 
    $ pip install https://github.com/pyfeeds/pyfeeds/archive/master.tar.gz
 
 After installation ``feeds`` is available in your virtual environment.
 
-Feeds supports Python 3.7+.
+Feeds supports Python 3.8+.
```

### Comparing `PyFeeds-2022.6.18/docs/index.rst` & `pyfeeds-2024.5.1/docs/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -43,16 +43,14 @@
   but in "real-time", i.e. on (HTTP) request.
 * `Full-Text RSS <https://bitbucket.org/fivefilters/full-text-rss>`_ converts
   feeds to contain the full article and not only a teaser based on heuristics
   and rules. Feeds are converted in "real-time", i.e. on request basis.
 * `f43.me <https://github.com/j0k3r/f43.me>`_ converts feeds to contain the
   full article and also improves articles by adding links to the comment
   sections of Hacker News and Reddit. Feeds are converted periodically.
-* `python-ftr <https://github.com/1flow/python-ftr>`_ is a library to extract
-  content from pages. A partial reimplementation of Full-Text RSS.
 
 Authors
 -------
 Feeds is written and maintained by `Florian Preinstorfer <https://nblock.org>`_
 and `Lukas Anzinger <https://www.notinventedhere.org>`_.
 
 .. _Scrapy: https://www.scrapy.org
```

### Comparing `PyFeeds-2022.6.18/docs/quickstart.rst` & `pyfeeds-2024.5.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/arstechnica.com.rst` & `pyfeeds-2024.5.1/docs/spiders/arstechnica.com.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/derstandard.at.rst` & `pyfeeds-2024.5.1/docs/spiders/derstandard.at.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/economist.com.rst` & `pyfeeds-2024.5.1/docs/spiders/economist.com.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/falter.at.rst` & `pyfeeds-2024.5.1/docs/spiders/falter.at.rst`

 * *Files 18% similar despite different names*

```diff
@@ -10,31 +10,34 @@
 
 .. code-block:: ini
 
    # List of spiders to run by default, one per line.
    spiders =
      falter.at
 
-Falter_ has a paywall for certain articles. If you want to crawl paid articles,
-please provide ``abonr`` (subscription number) and ``password``.
+Falter_ has a paywall for certain articles. If you want to crawl paid
+articles, please provide ``abonr`` (subscription number) and ``password``.
 
 ``pages`` accepts ``magazine`` for the Falter newspaper and
-``lokalfuehrer_reviews``, ``lokalfuehrer_newest`` for restaurant and
-``streams`` for movie streams. By default all are scraped.
+``lokalfuehrer_reviews``, ``lokalfuehrer_newest`` for restaurant, ``streams``
+for movie streams and ``events`` for events. By default all are scraped.
 
 ``blogs`` accepts slugs for the blogs from https://cms.falter.at/blogs/.
 
+``region`` accepts a region for events, e.g. ``wien`` (default).
+
 .. code-block:: ini
 
    [falter.at]
    abonr =
    password =
    pages =
        magazine
        lokalfuehrer_reviews
        lokalfuehrer_newest
        streams
+       events
    blogs =
        lingens
        thinktank
 
 .. _Falter: https://www.falter.at
```

### Comparing `PyFeeds-2022.6.18/docs/spiders/ft.com.rst` & `pyfeeds-2024.5.1/docs/spiders/ft.com.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/generic.rst` & `pyfeeds-2024.5.1/docs/spiders/generic.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/kurier.at.rst` & `pyfeeds-2024.5.1/docs/spiders/kurier.at.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/lwn.net.rst` & `pyfeeds-2024.5.1/docs/spiders/lwn.net.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/momoxfashion.com.rst` & `pyfeeds-2024.5.1/docs/spiders/momoxfashion.com.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/nachrichten.at.rst` & `pyfeeds-2024.5.1/docs/spiders/nachrichten.at.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/orf.at.rst` & `pyfeeds-2024.5.1/docs/spiders/orf.at.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/python-patterns.guide.rst` & `pyfeeds-2024.5.1/docs/spiders/python-patterns.guide.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/riskommunal.rst` & `pyfeeds-2024.5.1/docs/spiders/gem2go.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-.. _spider_riskommunal:
+.. _spider_gem2go:
 
-riskommunal
------------
+gem2go
+------
 News from your local town or community, if their website is maintained with
-`RIS Kommunal <https://info.riskommunal.net/>`_.
+`GEM2GO <https://www.gem2go.at/>`_.
 
 Configuration
 ~~~~~~~~~~~~~
-Add ``riskommunal`` to the list of spiders:
+Add ``gem2go`` to the list of spiders:
 
 .. code-block:: ini
 
    # List of spiders to run by default, one per line.
    spiders =
-     riskommunal
+     gem2go
 
 At least one url is required. The local community or town website typically has
 a "News" or "Neuigkeiten" URL that you may use.
 
 .. code-block:: ini
 
-   [riskommunal]
+   [gem2go]
    urls =
        http://yourlocalcommunity.tld/News
        https://mytown.tld/BUeRGERSERVICE/Neuigkeiten
```

### Comparing `PyFeeds-2022.6.18/docs/spiders/spotify.com.rst` & `pyfeeds-2024.5.1/docs/spiders/spotify.com.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/uebermedien.de.rst` & `pyfeeds-2024.5.1/docs/spiders/uebermedien.de.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders/wienerzeitung.at.rst` & `pyfeeds-2024.5.1/docs/spiders/wienerzeitung.at.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/docs/spiders.rst` & `pyfeeds-2024.5.1/docs/spiders.rst`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/cache.py` & `pyfeeds-2024.5.1/feeds/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from collections import defaultdict
 from datetime import datetime, timezone
 from time import time
 
 import scrapy
 from scrapy.extensions.httpcache import DummyPolicy, FilesystemCacheStorage
 from scrapy.utils.python import to_bytes
-from scrapy.utils.request import request_fingerprint
+from scrapy.utils.request import fingerprint
 
 logger = logging.getLogger(__name__)
 
 
 class FeedsCachePolicy(DummyPolicy):
     def should_cache_response(self, response, request):
         # We cache all responses regardless of HTTP code.
@@ -88,15 +88,15 @@
             metadata["cache_expires"] = request.meta["cache_expires"].total_seconds()
         metadata["type"] = "response"
         # Write it back.
         rpath = self._get_request_path(spider, request)
         self._write_meta_to_path(rpath, metadata)
 
     def _get_request_path(self, spider, request):
-        key = request_fingerprint(request, include_headers=["Cookie"])
+        key = fingerprint(request, include_headers=["Cookie"]).hex()
         return os.path.join(self.cachedir, spider.name, key[0:2], key)
 
     def retrieve_object(self, spider, key):
         metadata = self._read_meta(spider, key)
         if metadata is None:
             return None
         path = self._get_key_path(spider, key)
@@ -181,16 +181,16 @@
     def remove_cache_entry(self, cache_entry_path, remove_parents=False):
         meta = self._read_meta_from_path(cache_entry_path)
         if meta is None:
             return
 
         if remove_parents and "parents" in meta:
             spider_root = os.path.dirname(os.path.dirname(cache_entry_path))
-            for fingerprint in meta["parents"]:
-                path = os.path.join(spider_root, fingerprint[0:2], fingerprint)
+            for fpr in meta["parents"]:
+                path = os.path.join(spider_root, fpr[0:2], fpr)
                 self.remove_cache_entry(path, remove_parents=False)
 
         shutil.rmtree(cache_entry_path, ignore_errors=True)
 
 
 class FeedsCacheInMemoryStorage:
     def __init__(self):
```

### Comparing `PyFeeds-2022.6.18/feeds/cli.py` & `pyfeeds-2024.5.1/feeds/cli.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/default_settings.py` & `pyfeeds-2024.5.1/feeds/default_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,7 +63,11 @@
 # Set default level to info.
 # Can be overriden with --loglevel parameter.
 LOG_LEVEL = logging.INFO
 
 # Stats collection is disabled by default.
 # Can be overriden with --stats parameter.
 STATS_CLASS = "scrapy.statscollectors.DummyStatsCollector"
+
+# Set settings whose default value is deprecated to a future-proof value
+REQUEST_FINGERPRINTER_IMPLEMENTATION = "2.7"
+TWISTED_REACTOR = "twisted.internet.asyncioreactor.AsyncioSelectorReactor"
```

### Comparing `PyFeeds-2022.6.18/feeds/exporters.py` & `pyfeeds-2024.5.1/feeds/exporters.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/items.py` & `pyfeeds-2024.5.1/feeds/items.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/loaders.py` & `pyfeeds-2024.5.1/feeds/loaders.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/pipelines.py` & `pyfeeds-2024.5.1/feeds/pipelines.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/settings.py` & `pyfeeds-2024.5.1/feeds/settings.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spidermiddlewares.py` & `pyfeeds-2024.5.1/feeds/spidermiddlewares.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from copy import copy
 
 from scrapy import Request, signals
 from scrapy.exceptions import NotConfigured
 from scrapy.spidermiddlewares.httperror import HttpError
 from scrapy.utils.misc import load_object
-from scrapy.utils.request import request_fingerprint
+from scrapy.utils.request import fingerprint
 
 from feeds.exceptions import DropResponse
 
 logger = logging.getLogger(__name__)
 
 
 class FeedsHttpErrorMiddleware:
@@ -68,16 +68,16 @@
             request.meta["fingerprints"] = []
         logger.debug(
             "Parent fingerprints for request {}: {}".format(
                 request, request.meta["fingerprints"]
             )
         )
         if not request.meta.get("dont_cache", False):
-            fingerprint = request_fingerprint(request, include_headers=["Cookie"])
-            request.meta["fingerprints"].append(fingerprint)
+            fpr = fingerprint(request, include_headers=["Cookie"])
+            request.meta["fingerprints"].append(fpr)
         else:
             logger.debug(f"Skipping fingerprinting uncached request {request}")
 
     def process_spider_exception(self, response, exception, spider):
         # Note that due to Scrapy bug #220 this is *not* called if DropResponse is
         # raised from a generator.
         # See also https://github.com/scrapy/scrapy/issues/220.
```

### Comparing `PyFeeds-2022.6.18/feeds/spiders/__init__.py` & `pyfeeds-2024.5.1/feeds/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/addendum_org.py` & `pyfeeds-2024.5.1/feeds/spiders/indiehackers_com.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,70 @@
 import json
+from datetime import datetime
 
 import scrapy
 
 from feeds.loaders import FeedEntryItemLoader
 from feeds.spiders import FeedsSpider
 
 
-class AddendumOrgSpider(FeedsSpider):
-    name = "addendum.org"
-    start_urls = ["https://www.addendum.org/api/wp/v2/posts"]
+class IndieHackersComSpider(FeedsSpider):
+    name = "indiehackers.com"
 
-    feed_title = "Addendum"
-    feed_subtitle = "das, was fehlt"
+    feed_title = "Indie Hackers"
     feed_link = f"https://www.{name}"
-    feed_logo = f"{feed_link}/content/themes/qvv/img/logoAdd.png"
-    feed_icon = f"{feed_link}/content/themes/qvv/img/favicons/favicon-16x16.png"
+    feed_logo = f"{feed_link}/images/favicons/favicon--192x192.png"
+    feed_icon = f"{feed_link}/images/favicons/favicon--16x16.png"
+
+    custom_settings = {"DOWNLOAD_DELAY": 1.0}
+
+    def start_requests(self):
+        yield scrapy.Request(
+            "https://n86t1r3owz-1.algolianet.com/1/indexes/*/queries?"
+            + "x-algolia-agent=Algolia%20for%20JavaScript%20(3.35.1)%3B%20Browser"
+            + "%20(lite)&x-algolia-application-id=N86T1R3OWZ&"
+            + "x-algolia-api-key=5140dac5e87f47346abbda1a34ee70c3",
+            method="POST",
+            body=(
+                '{"requests":[{"indexName":"interviews_publishedAt_desc",'
+                + '"params":"query=&page=0&hitsPerPage=20"}]}'
+            ),
+            meta={"dont_cache": True},
+        )
 
     def parse(self, response):
-        posts = json.loads(response.text)
-        for post in posts:
-            il = FeedEntryItemLoader()
-            il.add_value("title", post["title"]["rendered"])
-            il.add_value("link", post["link"])
-            il.add_value("updated", post["modified"])
+        response = json.loads(response.text)
+        interviews = response["results"][0]["hits"]
+        for interview in interviews:
             yield scrapy.Request(
-                post["link"],
-                self._parse_article,
-                meta={"il": il},
+                f"{self.feed_link}/interview/{interview['interviewId']}",
+                self._parse_interview,
+                meta={
+                    "categories": interview["_tags"],
+                    "updated": interview["publishedAt"],
+                },
             )
 
-    def _parse_article(self, response):
+    def _parse_interview(self, response):
         remove_elems = [
-            ".article-header .title",
-            ".article-header .date",
-            ".paragraph-comments-sticky",
-            ".qvv-spinner",
-            ".article-image.mobile",
-            ".image-copyright",
-            ".article-image-copyright",
-            ".vertical-slider-mobile-image",
-            ".quote-box",
-            ".icon-end-of-article",
-            ".article-teaser-card",
-            ".content-row:contains('Lesen Sie auch:')",
-            ".article-footer ~ div",
-            ".article-footer",
-            ".cta-box",
-            ".slide-image .mobile",
-            ".slide-text .credit",
-            ".article-play",
-            ".top-tag",
+            ".shareable-quote",
+            ".share-bar",
+            # Remove the last two h2s and all paragraphs below.
+            ".interview-body > h2:last-of-type ~ p",
+            ".interview-body > h2:last-of-type",
+            ".interview-body > h2:last-of-type ~ p",
+            ".interview-body > h2:last-of-type",
         ]
-        change_tags = {
-            ".summary": "strong",
-            ".article-captioned-image-2": "figure",
-            ".keyplayer-card": "figure",
-            ".keyplayer-card .text-wrapper": "figcaption",
-            ".article-captioned-image": "figure",
-            ".article-captioned-image .image-caption": "figcaption",
-            ".slide": "figure",
-            ".slide-text .caption": "figcaption",
-            ".bg-white": "blockquote",
-            ".collapse-box": "blockquote",
-        }
         il = FeedEntryItemLoader(
+            timezone="UTC",
             response=response,
             base_url=self.feed_link,
             remove_elems=remove_elems,
-            change_tags=change_tags,
-            parent=response.meta["il"],
         )
-        il.add_css("content_html", ".article-wrapper")
-        il.add_css("author_name", ".article-author-link ::text")
-        il.add_css("category", ".top-tag ::text")
-        yield il.load_item()
+        il.add_value("link", response.url)
+        il.add_css("title", "h1::text")
+        il.add_css("author_name", "header .user-link__name::text")
+        il.add_css("content_html", ".interview-body")
+        il.add_value(
+            "updated", datetime.utcfromtimestamp(response.meta["updated"] / 1000)
+        )
+        return il.load_item()
```

### Comparing `PyFeeds-2022.6.18/feeds/spiders/arstechnica_com.py` & `pyfeeds-2024.5.1/feeds/spiders/arstechnica_com.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/atv_at.py` & `pyfeeds-2024.5.1/feeds/spiders/atv_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/biblioweb_at.py` & `pyfeeds-2024.5.1/feeds/spiders/biblioweb_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/cbird_at.py` & `pyfeeds-2024.5.1/feeds/spiders/cbird_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/derstandard_at.py` & `pyfeeds-2024.5.1/feeds/spiders/derstandard_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/economist_com.py` & `pyfeeds-2024.5.1/feeds/spiders/economist_com.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import scrapy
+from itemloaders.processors import TakeFirst
 
 from feeds.exceptions import DropResponse
 from feeds.loaders import FeedEntryItemLoader
 from feeds.spiders import FeedsSpider
 from feeds.utils import generate_feed_header
 
 
@@ -20,25 +21,25 @@
             self._ressorts = set(self._ressorts.split())
         else:
             self.logger.error("No ressorts given!")
             return
 
         for ressort in self._ressorts:
             yield scrapy.Request(
-                f"https://www.{self.name}/{ressort}/",
+                f"https://www.{self.name}/{ressort}",
                 meta={"dont_cache": True, "ressort": ressort},
             )
 
     def parse(self, response):
         if not self._titles.get(response.meta["ressort"]):
             self._titles[response.meta["ressort"]] = response.css(
                 "h1.section-collection-headline ::text"
             ).extract_first()
 
-        for path in response.css(".headline-link::attr('href')").extract():
+        for path in response.css("h3 a::attr('href')").extract():
             url = response.urljoin(path)
             yield scrapy.Request(
                 url, self._parse_article, meta={"ressort": response.meta["ressort"]}
             )
 
     def feed_headers(self):
         for ressort in self._ressorts:
@@ -58,34 +59,25 @@
         title = response.css('meta[property="og:title"]::attr(content)').extract_first()
         if not title:
             raise DropResponse(
                 f"Skipping {response.url} because ran into bot detection",
                 transient=True,
             )
 
-        remove_elems = [
-            "meta",
-            ".ds-share-list",
-            ".advert",
-            ".layout-article-links",
-            ".ds-chapter-list",
-            ".layout-article-meta",
-        ]
         change_tags = {
-            ".article__lead-image": "figure",
-            ".article__description": "h2",
-            ".article__footnote": "i",
+            "small": "span",
+            ".article-text": "p",
         }
         il = FeedEntryItemLoader(
-            response=response,
-            base_url=f"https://{self.name}",
-            remove_elems=remove_elems,
-            change_tags=change_tags,
+            response=response, base_url=f"https://{self.name}", change_tags=change_tags
         )
         il.add_value("link", response.url)
         il.add_value("title", title)
-        il.add_css("updated", "time.article__dateline-datetime::attr('datetime')")
-        il.add_css("content_html", ".article__lead-image")
-        il.add_css("content_html", ".article__description")
-        il.add_css("content_html", ".layout-article-body")
+        il.add_css("updated", "time::attr('datetime')")
+        il.add_css("content_html", "article section figure img", TakeFirst())
+        il.add_css("content_html", "article section h2")
+        il.add_css(
+            "content_html",
+            ".article__body-text, .article-text, article__body-text-image",
+        )
         il.add_value("path", response.meta["ressort"])
         return il.load_item()
```

### Comparing `PyFeeds-2022.6.18/feeds/spiders/falter_at.py` & `pyfeeds-2024.5.1/feeds/spiders/falter_at.py`

 * *Files 9% similar despite different names*

```diff
@@ -82,14 +82,26 @@
                 ("https://www.{}/api/kino?has_stream=true&mode=movie&c=100").format(
                     self.name
                 ),
                 self.parse_movies,
                 meta={"dont_cache": True, "movies": "streams"},
             )
 
+        if "events" in self.pages:
+            region = self.settings.get("FEEDS_SPIDER_FALTER_AT_REGION", "wien")
+            for i in range(10):
+                yield scrapy.Request(
+                    (
+                        "https://www.{}/api/events?mode=event&is_recommended=true"
+                        + "&region={}&c=100&f={}"
+                    ).format(self.name, region, 100 * i),
+                    self.parse_events,
+                    meta={"dont_cache": True, "region": region},
+                )
+
         blogs = self.settings.get("FEEDS_SPIDER_FALTER_AT_BLOGS")
         if blogs:
             self.blogs = blogs.split()
         else:
             self.blogs = []
 
         for blog in self.blogs:
@@ -189,14 +201,43 @@
                 if key.startswith("has_") and value:
                     il.add_value("category", key.replace("has_", ""))
                 elif key.startswith("is_") and value:
                     il.add_value("category", key.replace("is_", ""))
             il.add_value("updated", entry["index_date"])
             yield il.load_item()
 
+    def parse_events(self, response):
+        entries = json.loads(response.text)["hits"]
+        for entry in entries:
+            il = FeedEntryItemLoader(response=response, base_url=f"https://{self.name}")
+            il.add_value("path", "events")
+            il.add_value(
+                "link", "https://www.{}/event/{}".format(self.name, entry["prod_id"])
+            )
+            if entry["kat"]:
+                il.add_value("title", entry["kat"]["kat"])
+            il.add_value("title", entry["prod"])
+            if entry["additional_info"]:
+                il.add_value("content_html", f"<h2>{entry['additional_info']}</h2>")
+            il.add_value("content_html", entry["comment"])
+            if entry["images"]:
+                il.add_value(
+                    "content_html",
+                    '<img src="https://faltercdn2.falter.at/events/1080/{}">'.format(
+                        entry["images"][0]["filename"]
+                    ),
+                )
+            for key, value in entry.items():
+                if key.startswith("has_") and value:
+                    il.add_value("category", key.replace("has_", ""))
+                elif key.startswith("is_") and value:
+                    il.add_value("category", key.replace("is_", ""))
+            il.add_value("updated", entry["index_date"])
+            yield il.load_item()
+
     def parse_archive(self, response):
         # The perks of having a JavaScript frontend ...
         issues = json.loads(
             response.css("router-view").re_first("<router-view :data='([^']+)'>")
         )["issues"]
         latest_issue_date = dateutil_parse(
             issues[sorted(issues.keys())[-1]][-1], ignoretz=True
@@ -258,15 +299,15 @@
 
         for link in response.css("div[id^=post-] a::attr(href)").extract():
             yield scrapy.Request(
                 link, self.parse_blog_article, meta={"blog": response.meta["blog"]}
             )
 
     def parse_blog_article(self, response):
-        remove_elems = [".ad-component", ".wp-caption-text"]
+        remove_elems = [".ad-component", ".wp-caption-text", ".alert"]
         il = FeedEntryItemLoader(
             response=response,
             remove_elems=remove_elems,
             base_url=f"https://cms.{self.name}",
             timezone="Europe/Vienna",
             dayfirst=True,
             yearfirst=False,
```

### Comparing `PyFeeds-2022.6.18/feeds/spiders/ft_com.py` & `pyfeeds-2024.5.1/feeds/spiders/ft_com.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/generic.py` & `pyfeeds-2024.5.1/feeds/spiders/generic.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/keycloak_org.py` & `pyfeeds-2024.5.1/feeds/spiders/verbraucherrecht_at.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import scrapy
 
 from feeds.loaders import FeedEntryItemLoader
 from feeds.spiders import FeedsSpider
 
 
-class KeycloakOrgSpider(FeedsSpider):
-    name = "keycloak.org"
-    allowed_domains = [name]
-    start_urls = [f"https://www.{name}/blog-archive.html"]
-
-    feed_title = "Keycloak"
-    feed_subtitle = "Recent blog posts from Keycloak"
-    feed_link = f"https://www.{name}/blog"
-    feed_icon = f"https://www.{name}/resources/favicon.ico"
-    feed_logo = f"https://www.{name}/resources/images/keycloak_logo_200px.svg"
+class VerbraucherrechtAtSpider(FeedsSpider):
+    name = "verbraucherrecht.at"
+    start_urls = [f"https://{name}/aktuelle-news/5202"]
+
+    feed_title = "Verbraucherrecht"
+    feed_subtitle = "Neuigkeiten rund um Konsumentenschutz und Verbraucherrechte"
+    feed_author_name = "Verein für Konsumenteninformation"
+    feed_link = f"https://{name}"
+    feed_icon = f"https://{name}/themes/custom/wdm/images/favicon/favicon-vki.ico"
+    feed_logo = f"https://{name}/themes/custom/wdm/images/logo/logo-vki-verbraucherrecht.svg"  # noqa
 
     def parse(self, response):
-        for url in response.css("div.kc-article ul li a::attr('href')").getall():
-            yield scrapy.Request(response.urljoin(url), self.parse_article)
+        # Fetch only the current news page and deliberately ignore old news.
+        for url in response.css("div.view-content a::attr('href')").getall():
+            yield scrapy.Request(url, self.parse_article)
 
     def parse_article(self, response):
         il = FeedEntryItemLoader(
-            selector=response.css("div.kc-article"),
+            selector=response.css("div.content"),
             timezone="Europe/Vienna",
-            remove_elems=["h1", "p.blog-date", "div.alert-warning"],
+            remove_elems=["div.wrap>h1", "div#article-stat"],
+            dayfirst=True,
+            yearfirst=False,
         )
         il.add_css("title", "h1::text")
         il.add_value("link", response.url)
-        il.add_css("updated", "p.blog-date::text", re=r"^(.*\d{4})")
-        il.add_css("author_name", "p.blog-date::text", re=r"by (.*)$")
-        il.add_css("content_html", "div.kc-article")
+        il.add_css("updated", "time::attr('datetime')")
+        il.add_css("content_html", "div.content")
         return il.load_item()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyFeeds-2022.6.18/feeds/spiders/konsument_at.py` & `pyfeeds-2024.5.1/feeds/spiders/konsument_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/kurier_at.py` & `pyfeeds-2024.5.1/feeds/spiders/kurier_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/lbg_at.py` & `pyfeeds-2024.5.1/feeds/spiders/lbg_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/lwn_net.py` & `pyfeeds-2024.5.1/feeds/spiders/lwn_net.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/momoxfashion_com.py` & `pyfeeds-2024.5.1/feeds/spiders/momoxfashion_com.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from urllib.parse import urljoin
 
 import scrapy
 
 from feeds.loaders import FeedEntryItemLoader
 from feeds.spiders import FeedsSpider
 from feeds.utils import generate_feed_header
@@ -34,18 +35,18 @@
             return
 
         for item in response.css(".thumbnail"):
             il = FeedEntryItemLoader(selector=item, base_url=self._base_url)
             il.add_css("title", ".item_brand_text ::text")
             il.add_css("title", ".item-title ::text")
             il.add_css("title", ".current-price ::text")
-            il.add_value(
-                "link",
-                response.urljoin(item.css(".item-link::attr(href)").extract_first()),
+            link = response.urljoin(
+                re.sub(r"\?.*", "", item.css(".item-link::attr(href)").extract_first())
             )
+            il.add_value("link", link)
             image_url = item.css(".item-image::attr(data-bg)").re_first(
                 r"url\(([^)]+)\)"
             )
             il.add_value("content_html", f'<img src="{image_url}">')
             il.add_css("content_html", ".item-des-container")
             il.add_value("path", response.meta["path"])
             yield il.load_item()
```

### Comparing `PyFeeds-2022.6.18/feeds/spiders/nachrichten_at.py` & `pyfeeds-2024.5.1/feeds/spiders/nachrichten_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/npr_org.py` & `pyfeeds-2024.5.1/feeds/spiders/npr_org.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/oe1_orf_at.py` & `pyfeeds-2024.5.1/feeds/spiders/oe1_orf_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/orf_at.py` & `pyfeeds-2024.5.1/feeds/spiders/orf_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/profil_at.py` & `pyfeeds-2024.5.1/feeds/spiders/profil_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/puls4_com.py` & `pyfeeds-2024.5.1/feeds/spiders/puls4_com.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import scrapy
 
 from feeds.loaders import FeedEntryItemLoader
 from feeds.spiders import FeedsSpider
 
 
-class Pusl4ComSpider(FeedsSpider):
+class Puls4ComSpider(FeedsSpider):
     name = "puls4.com"
     start_urls = ["https://www.puls4.com/api/json-fe/page/sendungen"]
 
     feed_icon = (
         "https://www.puls4.com/bundles/wundermanpuls4/images/" + "favicon/favicon.png"
     )
```

### Comparing `PyFeeds-2022.6.18/feeds/spiders/python_patterns_guide.py` & `pyfeeds-2024.5.1/feeds/spiders/python_patterns_guide.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/riskommunal.py` & `pyfeeds-2024.5.1/feeds/spiders/gem2go.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-from urllib.parse import urlparse
+from urllib.parse import urljoin, urlparse
 
 import scrapy
 
 from feeds.loaders import FeedEntryItemLoader
 from feeds.spiders import FeedsSpider
 from feeds.utils import generate_feed_header
 
 
-class RisKommunalSpider(FeedsSpider):
-    name = "riskommunal"
+class Gem2GoSpider(FeedsSpider):
+    name = "gem2go"
     custom_settings = {"COOKIES_ENABLED": True}
     allowed_domains = []
     cookies = {"ris-cookie": "g7750", "ris_cookie_setting": "g7750"}
 
     _sites = []
     _titles = {}
     _subtitles = {}
     _links = {}
-    _icons = {}
 
     def feed_headers(self):
         for site in self._sites:
             yield generate_feed_header(
                 title=self._titles.get(site),
                 subtitle=self._subtitles.get(site),
                 link=self._links.get(site),
-                icon=self._icons.get(site),
                 path=site,
             )
 
     def start_requests(self):
-        urls = self.settings.get("FEEDS_SPIDER_RISKOMMUNAL_URLS")
+        urls = self.settings.get("FEEDS_SPIDER_GEM2GO_URLS")
         if not urls:
             self.logger.error("Please specify url(s) in the config file!")
             return
 
         for url in urls.split():
             parsed = urlparse(url)
             site = parsed.netloc
@@ -48,62 +46,66 @@
                 cookies=self.cookies,
                 meta={"dont_cache": True, "site": site},
             )
 
     def parse(self, response):
         site = response.meta["site"]
 
-        title = response.css("meta[property='og:title']::attr('content')").get()
+        title = response.css("meta[property='og:title']::attr(content)").get()
         self._titles[site] = title
         self._subtitles[site] = f"Neuigkeiten aus {title}"
 
-        icon = response.css("link[rel='icon']::attr('href')").get()
-        if icon and icon.startswith("/"):
-            icon = f"{self._links[site]}{icon}"
-        self._icons[site] = icon
-
-        for selector in response.css("div.newslist div[class*='float_left']"):
-            updated = selector.css("p.float_right::text").get()
-            if not updated:
-                # Do not care about "archived news"
-                continue
-
-            url = selector.css("a::attr('href')").get()
-            if not url:
-                # Ignore articles without a link
-                continue
-
-            if url.startswith("/"):
-                url = f"{self._links[site]}{url}"
-
-            yield scrapy.Request(
-                url,
-                self.parse_article,
-                cookies=self.cookies,
-                meta={"site": site, "updated": updated},
-            )
+        # Sites use different versions of the same "CMS". Extract the "news"
+        # container first and for each container scrape the article URL and the
+        # publication date.
+        for query_container, query_updated in [
+            ("div.newslist div[class*='float_left']", "p.float_right::text"),
+            (".bemCard", ".card-footer .bemContainer--date::text"),
+        ]:
+            for selector in response.css(query_container):
+                url = selector.css("a::attr(href)").get()
+                if not url:
+                    # Ignore articles without a link
+                    continue
+
+                # The publication date might be present only on the overview page,
+                # only on the article page or mix and match on both.
+                updated = selector.css(query_updated).get()
+
+                yield scrapy.Request(
+                    urljoin(self._links[site], url),
+                    self.parse_article,
+                    cookies=self.cookies,
+                    meta={"site": site, "updated": updated},
+                )
 
     def parse_article(self, response):
         site = response.meta["site"]
         il = FeedEntryItemLoader(
             response=response,
             timezone="Europe/Vienna",
             base_url=self._links[site],
             dayfirst=True,
             yearfirst=False,
             remove_elems=[
+                "div#main-content-header",
                 "div.main-content h1:first-of-type",
+                "div.newsdatum_container",
                 "p#ctl00_ctl00_ctl00_cph_col_a_cph_content_cph_content_detail_p_date",
-                "div#main-content-header",
+                "span.bemContainer--publishDate",
+                "span.bemContainer--readingTime",
             ],
         )
         il.add_value("path", site)
         il.add_value("link", response.url)
         il.add_value("updated", response.meta["updated"])
-        il.add_css("title", "div.main-content h1:first-of-type::text")
+        il.add_css("updated", ".bemContainer--publishDate ::text")
+        il.add_css("updated", ".newsdatum_container ::text")
+        il.add_css("updated", "p[id$='detail_p_date'] ::text")
+        il.add_css("title", "div.main-content h1:first-of-type ::text")
         il.add_css("content_html", "div.main-content")
 
         yield il.load_item()
 
     def _allow_domain(self, domain):
         self.allowed_domains.append(domain)
         for mw in self.crawler.engine.scraper.spidermw.middlewares:
```

### Comparing `PyFeeds-2022.6.18/feeds/spiders/servustv_com.py` & `pyfeeds-2024.5.1/feeds/spiders/servustv_com.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/spotify_com.py` & `pyfeeds-2024.5.1/feeds/spiders/spotify_com.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/theoatmeal_com.py` & `pyfeeds-2024.5.1/feeds/spiders/theoatmeal_com.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/trend_at.py` & `pyfeeds-2024.5.1/feeds/spiders/trend_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/tuwien_ac_at.py` & `pyfeeds-2024.5.1/feeds/spiders/tuwien_ac_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/tvthek_orf_at.py` & `pyfeeds-2024.5.1/feeds/spiders/tvthek_orf_at.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         il.add_value(
             "content_html",
             '<img src="{}">'.format(item["playlist"]["preview_image_url"]),
         )
         if item["description"]:
             il.add_value("content_html", item["description"].replace("\r\n", "<br>"))
         il.add_value("updated", item["date"])
-        il.add_value("link", item["url"].replace("api-tvthek.orf.at", "tvthek.orf.at"))
+        il.add_value("link", item["share_body"])
         # Check how many segments are part of this episode.
         if len(item["_embedded"]["segments"]) == 1:
             # If only one segment, item["sources"] contains invalid links.
             # We use the first embedded segment instead.
             # This is also how mediathekviewweb.de works.
             item["sources"] = item["_embedded"]["segments"][0]["sources"]
```

### Comparing `PyFeeds-2022.6.18/feeds/spiders/uebermedien_de.py` & `pyfeeds-2024.5.1/feeds/spiders/uebermedien_de.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/vice_com.py` & `pyfeeds-2024.5.1/feeds/spiders/vice_com.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/wienerlinien_at.py` & `pyfeeds-2024.5.1/feeds/spiders/wienerlinien_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/wienerzeitung_at.py` & `pyfeeds-2024.5.1/feeds/spiders/wienerzeitung_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds/spiders/zeitdiebin_at.py` & `pyfeeds-2024.5.1/feeds/spiders/zeitdiebin_at.py`

 * *Files identical despite different names*

### Comparing `PyFeeds-2022.6.18/feeds.cfg.dist` & `pyfeeds-2024.5.1/feeds.cfg.dist`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,11 @@
 
 #[economist.com]
 #ressorts =
 #    finance-and-economics
 #    special-report
 #    leaders
 
-#[tinyletter.com]
-#accounts =
-#    dabeaz
-
-#[riskommunal]
+#[gem2go]
 #urls =
 #    http://yourlocalcommunity.tld/News
 #    https://mytown.tld/BUeRGERSERVICE/Neuigkeiten
```

### Comparing `PyFeeds-2022.6.18/setup.py` & `pyfeeds-2024.5.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 from setuptools import find_packages, setup
 
 with open("README.rst") as f:
     long_description = f.read()
 
 setup(
     name="PyFeeds",
-    version="2022.6.18",
+    version="2024.5.1",
     description="DIY Atom feeds in times of social media and paywalls",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Florian Preinstorfer, Lukas Anzinger",
     author_email="florian@nblock.org, lukas@lukasanzinger.at",
     url="https://github.com/PyFeeds/PyFeeds",
     packages=find_packages(exclude=["tests"]),
     include_package_data=True,
     install_requires=[
-        "Click>=6.6",
-        "Scrapy>=2.2",
-        "dateparser>=0.5.1",
+        "click",
+        "dateparser",
         "feedparser",
-        "lxml>=3.5.0",
-        "python-dateutil>=2.7.3",
-        "pyxdg>=0.26",
-        "readability-lxml>=0.7",
+        "itemloaders",
+        "lxml[html_clean]",
+        "python-dateutil",
+        "pyxdg",
+        "readability-lxml",
+        "scrapy",
         "scrapy-inline-requests",
-        "itemloaders",  # explicit dependency of Scrapy > 2.2.1
     ],
     extras_require={
         "docs": ["sphinx", "sphinx_rtd_theme"],
         "test": ["pytest"],
     },
     entry_points={"console_scripts": ["feeds=feeds.cli:main"]},
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Framework :: Scrapy",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Internet :: WWW/HTTP",
     ],
 )
```

