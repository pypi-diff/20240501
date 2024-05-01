# Comparing `tmp/musical_games-0.8.0.tar.gz` & `tmp/musical_games-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musical_games-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "musical_games-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `musical_games-0.8.0.tar` & `musical_games-0.8.1.tar`

### file list

```diff
@@ -1,114 +1,115 @@
--rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.8.0/.coveragerc
--rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.8.0/.editorconfig
--rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.8.0/.gitchangelog.rc
--rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.8.0/.gitchangelog.tpl
--rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.8.0/.gitignore
--rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.8.0/.travis.yml
--rw-r--r--   0        0        0     1368 2024-04-30 09:20:18.554865 musical_games-0.8.0/CHANGELOG.rst
--rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.8.0/LICENSE
--rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.8.0/Makefile
--rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.8.0/README.rst
--rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.8.0/docs/Makefile
--rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.8.0/docs/authors.rst
--rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.8.0/docs/conf.py
--rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/contributing.rst
--rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.8.0/docs/history.rst
--rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/index.rst
--rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/installation.rst
--rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.8.0/docs/make.bat
--rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/modules.rst
--rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.8.0/docs/musical_games.converters.rst
--rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/musical_games.dice_games.lilypond.rst
--rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/musical_games.dice_games.rst
--rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/musical_games.rst
--rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/readme.rst
--rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.8.0/docs/usage.rst
--rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/__init__.py
--rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.8.0/musical_games/__version__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/data/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.8.0/musical_games/data/dice_games/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
--rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
--rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
--rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
--rw-r--r--   0        0        0     1427 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     1774 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     2747 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      525 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
--rw-r--r--   0        0        0      624 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0      140 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/__init__.py
--rw-r--r--   0        0        0     2386 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6417 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4232 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      814 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1012 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    30414 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2516 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6431 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4063 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1184 2024-04-13 12:50:48.939772 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1382 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
--rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
--rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
--rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
--rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
--rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
--rw-r--r--   0        0        0     2868 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     4351 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3533 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1635 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
--rw-r--r--   0        0        0     2047 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
--rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/__init__.py
--rw-r--r--   0        0        0     8337 2024-04-16 05:05:56.478852 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
--rw-r--r--   0        0        0     1830 2024-04-16 05:05:56.478852 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2796 2024-04-18 10:49:11.595361 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3765 2024-04-18 10:49:11.583361 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1258 2024-04-16 05:05:56.478852 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1476 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/__init__.py
--rw-r--r--   0        0        0     1800 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2714 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3713 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1258 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1476 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0     9516 2024-04-13 12:41:41.563787 musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2535 2024-04-13 12:49:58.583773 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6431 2024-04-13 12:57:29.887761 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4166 2024-04-13 12:54:59.155765 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1184 2024-04-13 12:51:21.251771 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1382 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.8.0/musical_games/dice_games/__init__.py
--rw-r--r--   0        0        0    44061 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/dice_games/base.py
--rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.8.0/musical_games/dice_games/data_csv.py
--rw-r--r--   0        0        0    18171 2024-04-30 09:20:04.502864 musical_games-0.8.0/musical_games/dice_games/dice_games.py
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/external/__init__.py
--rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/external/base.py
--rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/external/exceptions.py
--rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/external/images.py
--rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.8.0/musical_games/external/lilypond.py
--rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.8.0/musical_games/external/midi_converters.py
--rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.8.0/musical_games/external/utils.py
--rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.8.0/musical_games/external/wav_converters.py
--rw-r--r--   0        0        0     4835 2024-04-18 13:39:38.231087 musical_games-0.8.0/musical_games/utils.py
--rw-r--r--   0        0        0     1117 2024-04-30 09:20:18.434865 musical_games-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.8.0/scripts/__init__.py
--rw-r--r--   0        0        0     1995 2024-04-18 13:39:38.231087 musical_games-0.8.0/scripts/demo_cpe_bach.py
--rw-r--r--   0        0        0     3441 2024-04-30 09:20:04.502864 musical_games-0.8.0/scripts/demo_gerlach_scottish_dance.py
--rw-r--r--   0        0        0     2228 2024-04-18 13:39:38.231087 musical_games-0.8.0/scripts/demo_kirnberger_meneut_trio.py
--rw-r--r--   0        0        0     1896 2024-04-18 13:39:38.231087 musical_games-0.8.0/scripts/demo_kirnberger_polonaise.py
--rw-r--r--   0        0        0     1898 2024-04-18 13:39:38.231087 musical_games-0.8.0/scripts/demo_mozart_contredanse.py
--rw-r--r--   0        0        0     1852 2024-04-18 13:39:38.231087 musical_games-0.8.0/scripts/demo_mozart_waltz.py
--rw-r--r--   0        0        0     2329 2024-04-18 13:39:38.231087 musical_games-0.8.0/scripts/demo_stadler_meneut_trio.py
--rw-r--r--   0        0        0    26645 2024-04-30 09:20:04.502864 musical_games-0.8.0/scripts/lilypond_copy.py
--rw-r--r--   0        0        0    29517 2024-04-30 09:20:04.502864 musical_games-0.8.0/scripts/lilypond_copy2.py
--rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.8.0/tox.ini
--rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 musical_games-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.8.1/.coveragerc
+-rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.8.1/.editorconfig
+-rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.8.1/.gitchangelog.rc
+-rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.8.1/.gitchangelog.tpl
+-rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.8.1/.gitignore
+-rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.8.1/.travis.yml
+-rw-r--r--   0        0        0     1605 2024-05-01 12:33:23.050622 musical_games-0.8.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.8.1/LICENSE
+-rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.8.1/Makefile
+-rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.8.1/README.rst
+-rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.8.1/docs/Makefile
+-rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.8.1/docs/authors.rst
+-rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.8.1/docs/conf.py
+-rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/contributing.rst
+-rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.8.1/docs/history.rst
+-rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/index.rst
+-rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/installation.rst
+-rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.8.1/docs/make.bat
+-rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/modules.rst
+-rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.8.1/docs/musical_games.converters.rst
+-rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/musical_games.dice_games.lilypond.rst
+-rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/musical_games.dice_games.rst
+-rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/musical_games.rst
+-rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/readme.rst
+-rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/usage.rst
+-rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/__init__.py
+-rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.8.1/musical_games/__version__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/data/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.8.1/musical_games/data/dice_games/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
+-rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
+-rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
+-rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
+-rw-r--r--   0        0        0     1426 2024-05-01 10:00:27.942474 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     1773 2024-05-01 10:01:07.542475 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     2746 2024-05-01 10:01:07.522475 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      524 2024-05-01 10:01:25.466475 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
+-rw-r--r--   0        0        0      623 2024-05-01 10:01:48.778476 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-30 09:20:04.502864 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/__init__.py
+-rw-r--r--   0        0        0     2217 2024-05-01 12:32:39.650622 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6412 2024-05-01 09:58:30.166473 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     6150 2024-05-01 09:58:30.166473 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1208 2024-05-01 12:32:39.650622 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     2344 2024-05-01 12:32:39.650622 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    18686 2024-05-01 09:40:49.846455 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2515 2024-05-01 10:02:26.562476 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6430 2024-05-01 10:02:36.282477 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4062 2024-05-01 10:04:40.962478 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1115 2024-05-01 10:04:40.982478 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1313 2024-05-01 10:04:40.990478 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
+-rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
+-rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
+-rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
+-rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
+-rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
+-rw-r--r--   0        0        0     2867 2024-05-01 10:06:57.106481 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     4350 2024-05-01 10:06:57.126481 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3532 2024-05-01 10:06:57.114481 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1634 2024-05-01 10:06:57.134481 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     2046 2024-05-01 10:06:57.086481 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/__init__.py
+-rw-r--r--   0        0        0     8337 2024-04-16 05:05:56.478852 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
+-rw-r--r--   0        0        0     1829 2024-05-01 10:07:32.298481 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2795 2024-05-01 10:10:19.590484 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3764 2024-05-01 10:10:19.582484 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1257 2024-05-01 10:10:19.642484 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1475 2024-05-01 10:10:19.558484 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/__init__.py
+-rw-r--r--   0        0        0     1799 2024-05-01 10:10:19.542484 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2713 2024-05-01 10:10:19.622484 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3712 2024-05-01 10:10:19.610484 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1257 2024-05-01 10:10:19.570484 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1475 2024-05-01 10:10:19.602484 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     9516 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2534 2024-05-01 10:10:19.634484 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6430 2024-05-01 10:11:25.454485 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4165 2024-05-01 10:11:25.474485 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1115 2024-05-01 10:11:25.482485 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1313 2024-05-01 10:11:25.494485 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0     2104 2024-05-01 12:32:39.650622 musical_games-0.8.1/musical_games/data/lilypond_utils/clef_changes.ly
+-rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.8.1/musical_games/dice_games/__init__.py
+-rw-r--r--   0        0        0    45031 2024-05-01 09:20:19.862435 musical_games-0.8.1/musical_games/dice_games/base.py
+-rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.8.1/musical_games/dice_games/data_csv.py
+-rw-r--r--   0        0        0    16662 2024-05-01 09:24:08.890439 musical_games-0.8.1/musical_games/dice_games/dice_games.py
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/external/__init__.py
+-rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/external/base.py
+-rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/external/exceptions.py
+-rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/external/images.py
+-rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.8.1/musical_games/external/lilypond.py
+-rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.8.1/musical_games/external/midi_converters.py
+-rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/external/utils.py
+-rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.8.1/musical_games/external/wav_converters.py
+-rw-r--r--   0        0        0     4835 2024-04-18 13:39:38.231087 musical_games-0.8.1/musical_games/utils.py
+-rw-r--r--   0        0        0     1117 2024-05-01 12:32:51.034622 musical_games-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.8.1/scripts/__init__.py
+-rw-r--r--   0        0        0     1995 2024-04-18 13:39:38.231087 musical_games-0.8.1/scripts/demo_cpe_bach.py
+-rw-r--r--   0        0        0     3501 2024-05-01 12:32:39.650622 musical_games-0.8.1/scripts/demo_gerlach_scottish_dance.py
+-rw-r--r--   0        0        0     2228 2024-04-18 13:39:38.231087 musical_games-0.8.1/scripts/demo_kirnberger_meneut_trio.py
+-rw-r--r--   0        0        0     1896 2024-04-18 13:39:38.231087 musical_games-0.8.1/scripts/demo_kirnberger_polonaise.py
+-rw-r--r--   0        0        0     1898 2024-04-18 13:39:38.231087 musical_games-0.8.1/scripts/demo_mozart_contredanse.py
+-rw-r--r--   0        0        0     1852 2024-04-18 13:39:38.231087 musical_games-0.8.1/scripts/demo_mozart_waltz.py
+-rw-r--r--   0        0        0     2329 2024-04-18 13:39:38.231087 musical_games-0.8.1/scripts/demo_stadler_meneut_trio.py
+-rw-r--r--   0        0        0    26645 2024-04-30 09:20:04.502864 musical_games-0.8.1/scripts/lilypond_copy.py
+-rw-r--r--   0        0        0    29517 2024-04-30 09:20:04.502864 musical_games-0.8.1/scripts/lilypond_copy2.py
+-rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.8.1/tox.ini
+-rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 musical_games-0.8.1/PKG-INFO
```

### Comparing `musical_games-0.8.0/.gitchangelog.rc` & `musical_games-0.8.1/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/.gitignore` & `musical_games-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/CHANGELOG.rst` & `musical_games-0.8.1/CHANGELOG.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 *********
 Changelog
 *********
 
+v0.8.1 (2024-05-01)
+===================
+
+Other
+-----
+- Improved the lilypond designs.
+- In Gerlach, fixed some errors and made the clef change only local to the one specific bar.
+- Removed stem position overwrites in the Gerlach bars.
+
+
 v0.8.0 (2024-04-30)
 ===================
 
 Added
 -----
 - Adds Gerlach's Scottish Dance. Might need some more work concerning the clef changes.
```

### Comparing `musical_games-0.8.0/LICENSE` & `musical_games-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/Makefile` & `musical_games-0.8.1/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/README.rst` & `musical_games-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/docs/Makefile` & `musical_games-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/docs/conf.py` & `musical_games-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/docs/contributing.rst` & `musical_games-0.8.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/docs/index.rst` & `musical_games-0.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/docs/make.bat` & `musical_games-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/docs/musical_games.converters.rst` & `musical_games-0.8.1/docs/musical_games.converters.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/docs/musical_games.dice_games.lilypond.rst` & `musical_games-0.8.1/docs/musical_games.dice_games.lilypond.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/docs/musical_games.dice_games.rst` & `musical_games-0.8.1/docs/musical_games.dice_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/docs/musical_games.rst` & `musical_games-0.8.1/docs/musical_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/__version__.py` & `musical_games-0.8.1/musical_games/__version__.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv` & `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv` & `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv` & `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly` & `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##t
     \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
         paper-height = 420\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
@@ -20,33 +20,33 @@
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
-                \time 4/4
             }
             {
                 \clef treble
+                \time 4/4
                 \BLOCK{ for bar in bar_collections['treble'].get_bars('piano_right_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
-                \time 4/4
             }
             {
                 \clef bass
+                \time 4/4
                 \BLOCK{ for bar in bar_collections['bass'].get_bars('piano_left_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly` & `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \include "articulate.ly"
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly` & `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
 	page-count = 1
     print-all-headers = ##t
     score-markup-spacing = #'((basic-distance . 10))
     markup-system-spacing = #'((minimum-distance = 0))
 
     scoreTitleMarkup = \markup {
@@ -52,36 +52,36 @@
     }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \key c\major
-                \time 4/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
+                \time 4/4
                 \BLOCK{ for synchronous_bar in composition_bars['treble'] }
                     \VAR{synchronous_bar.get_bars()[0].lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
                 \key c\major
-                \time 4/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
+                \time 4/4
                 \BLOCK{ for synchronous_bar in composition_bars['bass'] }
                     \VAR{synchronous_bar.get_bars()[0].lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
     >>
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly` & `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##f
     paper-height = 50\mm
     paper-width = 100\mm
 }
 \header{
     title = ""
@@ -11,18 +11,18 @@
 \score {
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \key c\major
-                \time 4/4
             }
             {
                 \clef \VAR{ table_name }
+                \time 4/4
                 \VAR{ synchronous_bar.get_bars()[0].lilypond_str }
                 \bar "|."
             }
         >>
     >>
     \layout {
         indent = 0\mm
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly` & `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##f
     paper-height = 50\mm
     paper-width = 100\mm
 }
 \header{
     title = ""
@@ -11,18 +11,18 @@
 \score {
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \key c\major
-                \time 4/4
             }
             {
                 \clef \VAR{ table_name }
+                \time 4/4
                 \BLOCK{ for synchronous_bar in synchronous_bars }
                 \VAR{ synchronous_bar.get_bars()[0].lilypond_str }
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
     >>
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly` & `musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##t
     \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
-        paper-height = 1500\mm  %% default is 297 for a4
+        paper-height = 1600\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
 \header{
     title = "Scottish dance"
-    composer = "Stadler"
+    composer = "Gerlach"
     tagline = ##f
 }
 \score {
     \header {
         piece = \markup { \fontsize #1 "Scottish dance & Trio" }
         composer = ""
         title = ""
@@ -20,46 +20,41 @@
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c \major
-                \time 2/4
             }
             {
                 \clef treble
+                \time 2/4
                 \BLOCK{ for bar in bar_collections['dance'].get_bars('piano_right_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c \major
-                \time 2/4
             }
             {
                 \clef bass
-                \override Score.BreakAlignment #'break-align-orders =
-                      #(make-vector 3 '(span-bar
-                                        breathing-sign
-                                        staff-bar
-                                        key
-                                        clef
-                                        time-signature))
+                \time 2/4
                 \BLOCK{ for bar_ind, bar in bar_collections['dance'].get_bars('piano_left_hand').items() }
                     \BLOCK{ if bar.lilypond_str.startswith('\clef') }
-                    \set Staff.forceClef = ##t \VAR{bar.lilypond_str}
+                        \set Staff.forceClef = ##t
+                        \VAR{bar.lilypond_str}
                         \BLOCK{ if not bar_collections['dance'].get_bars('piano_left_hand')[bar_ind + 1].lilypond_str.startswith('\clef') }
-                        \once \override Staff.Clef.stencil = #(lambda (grob) (bracketify-stencil (ly:clef::print grob) Y 0.2 0.2 0.1))
-                        \clef "bass"
+                            \once \override Score.BreakAlignment #'break-align-orders = #(make-vector 3 '(span-bar breathing-sign staff-bar key clef time-signature))
+                            \once \override Staff.Clef.stencil = #(lambda (grob) (bracketify-stencil (ly:clef::print grob) Y 0.2 0.2 0.1))
+                            \clef "bass"
                         \BLOCK{ endif }
                     \BLOCK{ else }
                     \VAR{bar.lilypond_str}
                     \BLOCK{endif}
                 \BLOCK{ endfor }
                 \bar "|"
             }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly` & `musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \include "articulate.ly"
 
 % dance with repeats
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
@@ -13,15 +13,15 @@
                 midiMaximumVolume = #\VAR{midi_settings.get_max_volume('dance', 'piano_right_hand')}
                 midiInstrument = #"\VAR{midi_settings.get_midi_instrument('dance', 'piano_right_hand')}"
             }
         <<
             {
                 \key c \major
                 \time 2/4
-                \tempo 4 = 100
+                \tempo 4 = 70
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
                         \VAR{composition_bars['dance'][bar_index].get_bar('piano_right_hand').lilypond_str}
@@ -41,15 +41,15 @@
                 midiMaximumVolume = #\VAR{midi_settings.get_max_volume('dance', 'piano_left_hand')}
                 midiInstrument = #"\VAR{midi_settings.get_midi_instrument('dance', 'piano_left_hand')}"
             }
         <<
             {
                 \key c \major
                 \time 2/4
-                \tempo 4 = 100
+                \tempo 4 = 70
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
 		                \VAR{composition_bars['dance'][bar_index].get_bar('piano_left_hand').lilypond_str}
@@ -143,15 +143,15 @@
                 midiMaximumVolume = #\VAR{midi_settings.get_max_volume('dance', 'piano_right_hand')}
                 midiInstrument = #"\VAR{midi_settings.get_midi_instrument('dance', 'piano_right_hand')}"
             }
         <<
             {
                 \key c \major
                 \time 2/4
-                \tempo 4 = 100
+                \tempo 4 = 70
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \BLOCK{ for bar_index in range(16) }
                     \VAR{composition_bars['dance'][bar_index].get_bar('piano_right_hand').lilypond_str}
                 \BLOCK{ endfor }
@@ -165,15 +165,15 @@
                 midiMaximumVolume = #\VAR{midi_settings.get_max_volume('dance', 'piano_left_hand')}
                 midiInstrument = #"\VAR{midi_settings.get_midi_instrument('dance', 'piano_left_hand')}"
             }
         <<
             {
                 \key c \major
                 \time 2/4
-                \tempo 4 = 100
+                \tempo 4 = 70
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
                 \BLOCK{ for bar_index in range(16) }
                     \VAR{composition_bars['dance'][bar_index].get_bar('piano_left_hand').lilypond_str}
                 \BLOCK{ endfor }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,67 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
-	print-all-headers = ##t
+	page-count = 1
+    print-all-headers = ##t
     score-markup-spacing = #'((basic-distance . 10))
     markup-system-spacing = #'((minimum-distance = 0))
-
-    \BLOCK{ if render_settings['single_page'] }
-        paper-height = 360\mm  %% default is 297 for a4
-    \BLOCK{ endif }
 }
 \header{
-    title = "Scottish Dance - Dance and Trio"
-    composer = "Gerlach"
+    title = "Menuet and Trio"
+    composer = "Kirnberger"
     tagline = ##f
 }
 \score {
     \header {
-        piece = \markup { \fontsize #1 "Scottish Dance" }
+        piece = \markup { \fontsize #1 "Menuet" }
         title = ""
         composer = ""
     }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
-                \key c \major
-                \time 2/4
+                \key d\major
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
+                \time 3/4
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
-                        \VAR{composition_bars['dance'][bar_index].get_bar('piano_right_hand').lilypond_str}
+                        \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
-                        \VAR{composition_bars['dance'][bar_index].get_bar('piano_right_hand').lilypond_str}
+                        \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
         <<
             {
-                \key c \major
-                \time 2/4
+                \key d\major
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
+                \time 3/4
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
-		                \VAR{composition_bars['dance'][bar_index].get_bar('piano_left_hand').lilypond_str}
+		                \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
-	        	\clef bass
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
-    		            \VAR{composition_bars['dance'][bar_index].get_bar('piano_left_hand').lilypond_str}
+    		            \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \once \override Score.RehearsalMark #'self-alignment-X = #right \mark \markup {\fontsize #-1 \italic "Fine"}
             }
         >>
     >>
     \layout {
@@ -80,21 +76,21 @@
         composer = ""
     }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
-                \key c \major
-                \time 2/4
+                \key d\minor
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
+                \time 3/4
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
                         \VAR{composition_bars['trio'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
@@ -102,27 +98,26 @@
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
         <<
             {
-                \key c \major
-                \time 2/4
+                \key d\minor
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
+                \time 3/4
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
 		                \VAR{composition_bars['trio'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
-	        	\clef bass
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
     		            \VAR{composition_bars['trio'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \once \override Score.RehearsalMark #'self-alignment-X = #right \mark \markup {\fontsize #-1 \italic "D.C. al Fine"}
             }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly` & `musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##f
     paper-height = 50\mm
     paper-width = 100\mm
 }
 \header{
     title = ""
@@ -10,31 +10,39 @@
 }
 \score {
     \new PianoStaff
     <<
         \new Staff
         <<
             {
-                \key c \major
-                \time 2/4
+                \BLOCK{ if table_name == 'menuet' }
+                    \key d\major
+                \BLOCK{ else }
+                    \key g\major
+                \BLOCK{ endif }
             }
             {
                 \clef treble
+                \time 3/4
                 \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
-                \key c \major
-                \time 2/4
+                \BLOCK{ if table_name == 'menuet' }
+                    \key d\major
+                \BLOCK{ else }
+                    \key g\major
+                \BLOCK{ endif }
             }
             {
                 \clef bass
+                \time 3/4
                 \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
                 \bar "|."
             }
         >>
     >>
     \layout {
         indent = 0\mm
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##f
     paper-height = 50\mm
     paper-width = 100\mm
 }
 \header{
     title = ""
@@ -10,33 +10,41 @@
 }
 \score {
     \new PianoStaff
     <<
         \new Staff
         <<
             {
-                \key c \major
-                \time 2/4
+                \BLOCK{ if table_name == 'menuet' }
+                    \key d\major
+                \BLOCK{ else }
+                    \key d\minor
+                \BLOCK{ endif }
             }
             {
                 \clef treble
+                \time 3/4
                 \BLOCK{ for synchronous_bar in synchronous_bars }
                 \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
-                \key c \major
-                \time 2/4
+                \BLOCK{ if table_name == 'menuet' }
+                    \key d\major
+                \BLOCK{ else }
+                    \key d\minor
+                \BLOCK{ endif }
             }
             {
                 \clef bass
+                \time 3/4
                 \BLOCK{ for synchronous_bar in synchronous_bars }
                 \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
     >>
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv` & `musical_games-0.8.1/scripts/lilypond_copy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,193 +1,819 @@
-"bar_index","piano_right_hand","piano_left_hand"
-"1","\stemDown d''16 [\stemDown e''16 \stemDown f''16 \stemDown d''16] \stemDown b'8 [\stemDown d''8]","{<<{\voiceOne r8 <b f'>8 \stemUp <d' f'>8 [\stemUp <b f'>8]} \new Voice {\voiceTwo g2}>>}"
-"2","\stemDown a''16 [\stemDown gis''16 \stemDown a''16 \stemDown b''16] \stemDown c'''8 [\stemDown d'''8]","\stemDown a8 [\stemDown <c' e'>8] \stemDown d8 [\stemDown <a d'>8]"
-"3","\stemDown <c'' g''>8 [\stemDown <c'' fis''>8] <b' g''>4","\stemDown <g d'>8 [\stemDown <a d'>8] <g d'>4"
-"4","\stemDown g'8 [\stemDown c''16 \stemDown d''16] \stemDown e''16 [\stemDown f''16 \stemDown g''8]","\stemDown e8 [\stemDown g8] \stemDown c'8 [\stemDown e'8]"
-"5","\stemDown e''8. [\stemDown d''16 \stemDown b'8 \stemDown b'8]","\clef ""treble""{<<{\voiceOne r8 <b e'>8 \stemUp <d' e'>8 [\stemUp <d' e'>8]} \new Voice {\voiceTwo gis2}>>}"
-"6","\stemDown cis''16 [\stemDown cis''16 \stemDown e''16 \stemDown cis''16] \stemDown a'8 [\stemDown e''8]","\clef ""bass"" {<<{\voiceOne r8 <e' g'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]} \new Voice {\voiceTwo a2}>>}"
-"7","\stemDown c''8 [\stemDown <g' e''>8] <e' c''>4","\stemDown <c' e'>8 [\stemDown c'8] c4"
-"8","\stemDown c''8 [\stemDown c''16 \stemDown b'16] \stemUp a'8 [\stemUp e'8]","\stemDown a,8 [\stemDown <a c'>8] \stemDown <a c'>8 [\stemDown <a c'>8]"
-"9","\stemDown b'8 [\stemDown a''8] \stemDown g''8 [\stemDown f''8]","{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]} \new Voice {\voiceTwo g2}>>}"
-"10","\stemUp b'8 [\stemUp g'8] g''4","\stemDown <g b d'>8 [\stemDown <g b>8] <g b>4"
-"11","\stemDown f''16 [\stemDown e''16 \stemDown f''16 \stemDown a''16] \stemDown f''8 [\stemDown b'8]","\stemDown f8 [\stemDown <a d'>8] \stemDown g8 [\stemDown <d' f'>8]"
-"12","\stemDown <e'' g''>8 [\stemDown <g' c''>8] <c'' e''>4","\stemDown c8 [\stemDown e'8] c'4"
-"13","<a' c''>4 <g' cis''>4","<f f'>4 \stemDown <a e'>8 [\stemDown es'8]"
-"14","\stemDown e''16 [\stemDown d''16 \stemDown cis''16 \stemDown e''16] d''4","{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]} \new Voice {\voiceTwo g2}>>}"
-"15","\stemUp <e' g'>8 [\stemUp <f' a'>16 \stemUp <e' g'>16] \stemUp <e' g'>8 [\stemUp <e' c''>8]","{<<{\voiceOne r8 c'8 \stemUp c'8 [\stemUp c'8]} \new Voice {\voiceTwo c2}>>}"
-"16","\stemDown g''16 [\stemDown a''16 \stemDown b''16 \stemDown c'''16] \stemDown d'''8 [\stemDown g''8]","\clef ""treble"" {<<{\voiceOne r8 <f' g'>8 \stemUp <f' g'>8 [\stemUp <f' g'>8]} \new Voice {\voiceTwo b2}>>}"
-"17","\stemDown e''8 [\grace { \stemUp d''8 } \stemDown e''8] e'4","\stemDown <e gis b>8 [\grace { \stemUp dis'8 } \stemDown e'8] e4"
-"18","\stemDown d'''16 [\stemDown cis'''16 \stemDown d'''16 \stemDown e'''16] \stemDown f'''8 [\stemDown a''8]","\clef ""bass"" {<<{\voiceOne r8 <d' f'>8 \stemUp <d' f'>8 [\stemUp <d' f'>8]} \new Voice {\voiceTwo d4 s4}>>}"
-"19","\stemDown d'''8 [\stemDown a''8] \stemDown b''8 [\stemDown e'''8]","<fis c' d'>4 \stemDown <g b d'>8 [\stemDown <gis b d'>8] |"
-"20","\stemDown g''16 [\stemDown fis''16 \stemDown fis''16 \stemDown e'''16] \stemDown e'''16 [\stemDown d'''16 \stemDown c'''16 \stemDown a''16]","{<<{\voiceOne r8 <a c'>8 \stemUp <a c'>8 [\stemUp <fis d'>8]} \new Voice {\voiceTwo d2}>>}"
-"21","\stemDown e''8 [\stemDown d''8] \stemDown a''16 [\stemDown g''16 \stemDown f''16 \stemDown d''16]","{<<{\voiceOne r8 <b f'>8 r8 <b f'>8} \new Voice {\voiceTwo g4 g4}>>}"
-"22","\stemDown c'''8 [\stemDown d'''16 \stemDown es'''16] \stemDown g''8 [\stemDown e''8]","<fis a c' es'>4 <g c' e'>4"
-"23","\stemDown e''8 [\stemDown b'8] \stemDown gis''8 [\stemDown e''8]","\stemDown g8 [\stemDown <d' e'>8] \stemDown b8 [\stemDown <d' e'>8]"
-"24","\stemDown c'''8 [\stemDown bes''8] \stemDown g''8 [\stemDown e''8]","\stemDown g8 [\stemDown <c' e'>8] \stemDown bes8 [\stemDown <c' g'>8]"
-"25","\stemDown e''8 [\stemDown c''8] \stemDown g''8 [\stemDown e''8]","{<<{\voiceOne r8 <bes c'>8 \stemUp <bes c'>8 [\stemUp <bes c'>8]} \new Voice {\voiceTwo c2}>>}"
-"26","\stemDown a'8 [\stemDown c''8] \stemDown e''8 [\stemDown a''8]","\stemDown a8 [\stemDown c'8] \stemDown e'8 [\stemDown a'8]"
-"27","\stemDown c''8 [\stemDown e''8] \stemDown a''8 [\stemDown c'''8]","{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo a2}>>}"
-"28","\stemDown e''8 [\stemDown d''8] c''4","\stemDown <g c' e'>8 [\stemDown <g b f'>8] <c' e'>4"
-"29","\stemDown d''8 [\stemDown e''16 \stemDown d''16] \stemDown a'8 [\stemDown f''8]","{<<{\voiceOne r8 <a d'>8 r8 <a d'>8} \new Voice {\voiceTwo f4 d4}>>}"
-"30","{<<{\voiceOne \stemUp e''8 [\stemUp c'''8] g''4} \new Voice {\voiceTwo c''2}>>}","\stemDown c8 [\stemDown e8] \stemDown <c' e'>8 [\stemDown g8]"
-"31","\stemDown f''16 [\stemDown e''16 \stemDown dis''16 \stemDown e''16] \stemDown c'''8 [\stemDown e''8]","\stemDown c8 [\stemDown <c' e'>8] \stemDown a8 [\stemDown <c' e'>8]"
-"32","<g' c'' e''>4 <g' b' d''>8 r8","g2"
-"33","\stemDown g''8 [\stemDown b'8] \stemDown fis''8 [\stemDown a'8]","\stemDown e8 [\stemDown <g b>8] \stemDown b,8 [\stemDown <fis b>8]"
-"34","\stemDown a''8 [\stemDown <c'' a''>8] <a' a''>4","\stemDown <a c'>8 [\stemDown <a e'>8] <a c'>4"
-"35","\stemDown c''16 [\stemDown d''16 \stemDown e''16 \stemDown c''16] \stemDown a'8 [\stemDown a''8]","{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo a2}>>}"
-"36","\stemDown a''8 [\stemDown f''8] \stemDown d''8 [\stemDown c''8]","<f a d'>4 <fis a d'>4"
-"37","\stemDown a''16 [\stemDown f''16 \stemDown e''16 \stemDown d''16] \stemDown c''16 [\stemDown g''16 \stemDown b'16 \stemDown d''16]","\stemDown f8 [\stemDown <a d'>8] \stemDown <g c' e'>8 [\stemDown <g b f'>8]"
-"38","\stemDown f''16 [\stemDown e''16 \stemDown f''16 \stemDown g''16] \stemDown a''8 [\stemDown a''8]","{<<{\voiceOne r8 <a c'>8 \stemUp <a c'>8 [\stemUp <a c'>8]} \new Voice {\voiceTwo f2}>>}"
-"39","{<<{\voiceOne \stemUp e''8 [\stemUp f''16 \stemUp e''16] \stemUp dis''8 [\stemUp e''8]} \new Voice {\voiceTwo | c''2}>>}","\stemDown c8 [\stemDown g8] \stemDown <c' e'>8 [\stemDown g8] |"
-"40","\stemUp <e' g'>8 [\stemUp <f' a'>16 \stemUp <e' g'>16] \stemDown <e' c''>8 [\stemDown <c'' e''>8]","{<<{\voiceOne r8 c'8 \stemUp c'8 [\stemUp c'8]} \new Voice {\voiceTwo c2}>>}"
-"41","\stemUp gis'16 [\stemUp a'16 \stemUp b'16 \stemUp gis'16] \stemUp e'8 [\stemUp e''8]","{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]} \new Voice {\voiceTwo e2}>>}"
-"42","\stemDown a''8 [\stemDown gis''16 \stemDown a''16] \stemDown bes''8 [\stemDown a''8]","\clef ""bass"" {<<{\voiceOne r8 <cis' e'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]} \new Voice {\voiceTwo a4 s4}>>}"
-"43","\stemDown a'8 [\stemDown bes'16 \stemDown b'16] \tuplet 3/2 {\stemDown c''8 [\stemDown f''8 \stemDown a'8]}","{<<{\voiceOne r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]} \new Voice {\voiceTwo f2}>>}"
-"44","\stemDown c'''8 [\stemDown d''8] \stemDown b''8 [\stemDown d''8]","{<<{\voiceOne r8 <fis c'>8 r8 b8} \new Voice {\voiceTwo d4 g4}>>}"
-"45","\stemDown b'8 [\stemDown d''8] \stemDown g''8 [\stemDown b''8]","{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]} \new Voice {\voiceTwo g2}>>}"
-"46","\stemDown c''8 [\stemDown e''8] g'4","\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]"
-"47","\stemDown c''8 [\stemDown e''8] g''4","\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]"
-"48","\stemDown <gis' d''>8 [\stemDown <gis' e''>8] \stemDown <a' fis''>8 [\stemDown <b' gis''>8]","\stemDown e8 [\stemDown e'8] \stemDown <dis' e'>8 [\stemDown <d' e'>8]"
-"49","\stemDown b''16 [\stemDown c'''16 \stemDown d'''16 \stemDown b''16] \stemDown g''8 [\stemDown f'''8]","{<<{\voiceOne r8 <b f'>8 \stemUp <b d'>8 [\stemUp <b d'>8]} \new Voice {\voiceTwo g2}>>}"
-"50","\stemUp c''8 [\stemUp <e' c''>8] <e' c''>4","\stemDown <c' e'>8 [\stemDown g8] c4"
-"51","\stemDown c''8 [\stemDown <g' e''>8] <e' c''>4","\stemDown <c' e'>8 [\stemDown c'8] c4"
-"52","\stemDown c''8 [\stemDown c'''8] c''4","\stemDown <c' e'>8 [\stemDown <e' g'>8] <c' e'>4"
-"53","\stemDown f''8 [\stemDown a''8] f''4","\stemDown <f a>8 [\stemDown c'8] <f a>4"
-"54","{<<{\voiceOne \stemUp b''8 [\stemUp d'''16 \stemUp b''16] \stemUp a''8 [\stemUp gis''8]} \new Voice {\voiceTwo d''4 \stemDown c''8 [\stemDown b'8]}>>}","{<<{\voiceOne r8 f'8 \stemUp e'8 [\stemUp d'8]} \new Voice {\voiceTwo f4 \stemDown e8 [\stemDown e8]}>>}"
-"55","{<<{\voiceOne \stemUp d''8 [\stemUp e''16 \stemUp d''16] \stemUp d''8 [\stemUp g''8]} \new Voice {\voiceTwo f'4 f'4}>>}","{<<{\voiceOne r8 b8 \stemUp b8 [\stemUp b8]} \new Voice {\voiceTwo g2}>>}"
-"56","\stemDown a''8 [\stemDown e''8] \stemDown cis'''8 [\stemDown e'''8]","{<<{\voiceOne r8 <cis' g'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]} \new Voice {\voiceTwo a2}>>}"
-"57","\stemDown bes'8 [\stemDown c''16 \stemDown e''16] g''4","\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]"
-"58","\stemDown g''8 [\stemDown d'''16 \stemDown dis'''16] \stemDown e'''8 [\stemDown g''8]","<g b f'>4 <g c' e'>4"
-"59","\stemDown c''16 [\stemDown d''16 \stemDown e''16 \stemDown d''16] c''4","\stemDown <g c' e'>8 [\stemDown <g b f'>8] <c' e'>4 |"
-"60","\stemDown a'8 [\stemDown d''16 \stemDown e''16] \stemDown f''16 [\stemDown g''16 \stemDown a''8]","\stemDown f8 [\stemDown a8] \stemDown d'8 [\stemDown f'8]"
-"61","\stemDown b''8 [\stemDown f''16 \stemDown b''16] \stemDown d'''8 [\stemDown f'''8]","{<<{\voiceOne r8 <f b>8 \stemUp <f b>8 [\stemUp <f b>8]} \new Voice {\voiceTwo d2}>>}"
-"62","\stemDown g''8 [\stemDown fis''16 \stemDown g''16] \stemDown as''8 [\stemDown f''16 \stemDown d''16]","<bes d' g'>4 <bes d' f'>4"
-"63","\stemDown c'''8 [\stemDown a''8] \stemDown f'''8 [\stemDown a''8]","\stemDown a8 [\stemDown <c' f'>8] \stemDown f8 [\stemDown <c' f'>8]"
-"64","\stemDown f''8 [\stemDown <c'' a''>8] <a' f''>4","\stemUp <a, c>8 [\stemUp e,8] a,,4"
-"65","\stemUp e'8 [\stemUp c''16 \stemUp e'16] \stemDown g'8 [\stemDown e''8]","{<<{\voiceOne r8 <g c'>8 \stemUp <g c'>8 [\stemUp <g c'>8]} \new Voice {\voiceTwo c2}>>}"
-"66","\stemDown g''16 [\stemDown f''16 \stemDown f''16 \stemDown d'''16] \stemDown d'''8 [\stemDown f''8]","{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]} \new Voice {\voiceTwo g2}>>}"
-"67","\stemDown c'''8 [\stemDown d'''16 \stemDown e'''16] \stemDown f'''8 [\stemDown a''8]","<g bes c'>4 <f a c'>4"
-"68","\stemDown d'''8 [\stemDown c'''8] \stemDown bes''8 [\stemDown a''8]","{<<{\voiceOne r8 f'8 r8 f'8} \new Voice {\voiceTwo c'4 d'4}>>}"
-"69","\stemDown c'''16 [\stemDown bes''16 \stemDown a''16 \stemDown g''16] \stemDown a''8 [\stemDown f''8]","{<<{\voiceOne r8 <bes e'>8 r8 <a c'>8} \new Voice {\voiceTwo c4 f4}>>}"
-"70","\stemDown g''8 [\stemDown <b' g''>8] <b' g''>4","\stemDown <g b>8 [\stemDown g8] g,4"
-"71","\stemDown d''8 [\stemDown e''16 \stemDown d''16] \stemDown c'''8 [\stemDown a''8]","{<<{\voiceOne r8 <a d'>8 \stemUp <a d'>8 [\stemUp <a d'>8]} \new Voice {\voiceTwo fis2}>>}"
-"72","\stemDown a''8 [\stemDown f''16 \stemDown d''16] \stemDown c''16 [\stemDown g''16 \stemDown b'16 \stemDown d''16]","\stemDown f8 [\stemDown <a d'>8] \stemDown <g c' e'>8 [\stemDown <g b f'>8]"
-"73","\stemDown a''16 [\stemDown b''16 \stemDown c'''16 \stemDown d'''16] \stemDown e'''8 [\stemDown gis''8]","\stemDown e8 [\stemDown <c' e'>8] \stemDown e8 [\stemDown <b d'>8]"
-"74","\stemDown d'''8 [\stemDown c'''8] \stemDown a''8 [\stemDown e''8]","{<<{\voiceOne r8 <c' e'>8 r8 <c' e'>8} \new Voice {\voiceTwo a4 a4}>>}"
-"75","\stemDown e''8 [\stemDown e''16 \stemDown d''16] \stemDown a''8 [\stemDown d''8]","{<<{\voiceOne r8 <c' d'>8 \stemUp <c' d'>8 [\stemUp <c' d'>8]} \new Voice {\voiceTwo fis2}>>}"
-"76","\stemDown a''16 [\stemDown gis''16 \stemDown a''16 \stemDown b''16] c'''4","\stemDown a8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]"
-"77","\stemUp <e' c''>8 [\stemUp <e' c''>8] \stemUp <f' d''>8 [\stemUp <g' e''>8]","\stemDown c8 [\stemDown c'8] \stemDown <b c'>8 [\stemDown <bes c'>8]"
-"78","\stemDown e''16 [\stemDown d''16 \stemDown cis''16 \stemDown d''16] \stemDown a''8 [\stemDown d''8]","\stemDown fis8 [\stemDown <a d'>8] \stemDown fis8 [\stemDown <c' d'>8]"
-"79","\stemDown c''8 [\stemDown a'8] \stemDown a''8 [\stemDown e''8] |","{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo a2}>>}"
-"80","\stemDown a''16 [\stemDown g''16 \stemDown f''16 \stemDown e''16] \stemDown f''8 [\stemDown d''8]","\stemDown d8 [\stemDown <d' f'>8] \stemDown <d' f'>8 [\stemDown <d' f'>8]"
-"81","\stemDown c'''16 [\stemDown d'''16 \stemDown e'''16 \stemDown f'''16] \stemDown g'''8 [\stemDown c'''8]","{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo g2}>>}"
-"82","\grace { \stemUp ais''8 } b''4 \grace { \stemUp ais''8 } \stemDown b''8 [\stemDown e'''8]","\stemDown e8 [\stemDown <gis d'>8] \stemDown gis8 [\stemDown <d' e'>8]"
-"83","a''2","{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo a2}>>}"
-"84","\stemDown c''8 [\stemDown e''8] \stemDown a'8 [\stemDown a''8]","{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo a2}>>}"
-"85","{<<{\voiceOne \stemUp d''16 [\stemUp cis''16 \stemUp d''16 \stemUp e''16] \stemUp f''8 [\stemUp d''8]} \new Voice {\voiceTwo f'4 r4}>>}","\stemDown bes,8 [\stemDown <bes d'>8] \stemDown <bes d'>8 [\stemDown <bes d'>8]"
-"86","\stemDown c'''8 [\stemDown a''8] \stemDown b''8 [\stemDown c'''8]","\stemDown <a c'>8 [\stemDown <fis a d'>8] \stemDown <g b f'>8 [\stemDown <a c' e'>8]"
-"87","\stemUp <e' g'>8 [\stemUp <f' a'>16 \stemUp <e' g'>16] \stemUp <e' g'>8 [\stemUp <g' e''>8]","{<<{\voiceOne r8 c'8 \stemUp c'8 [\stemUp c'8]} \new Voice {\voiceTwo c2}>>}"
-"88","\stemDown e''8 [\stemDown e''16 \stemDown d''16] \stemDown c''8 [\stemDown a'8]","\stemDown a,8 [\stemDown <a c'>8] \stemDown <a c'>8 [\stemDown <a c'>8]"
-"89","\stemDown <c'' c'''>8 [\stemDown <g'' b''>16 \stemDown <f'' a''>16] \stemDown <e'' g''>8 [\stemDown <f'' a''>8]","{<<{\voiceOne r8 c'8 \stemUp c'8 [\stemUp c'8]} \new Voice {\voiceTwo c2}>>}"
-"90","\stemDown e'''8 [\stemDown c'''8] \stemDown g''8 [\stemDown e''8]","\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]"
-"91","\stemDown g''8 [\stemDown b'8] c''4","\stemDown <g d' f'>8 [\stemDown <g d' f'>8] <c' e'>4"
-"92","\stemDown fis''16 [\stemDown g''16 \stemDown a''16 \stemDown fis''16] \stemDown d''8 [\stemDown c'''8]","{<<{\voiceOne r8 <c' d'>8 r8 <c' d'>8} \new Voice {\voiceTwo a4 fis4}>>}"
-"93","\stemDown b''8 [\stemDown e''8] \stemDown e'''8 [\stemDown e''8]","<e gis b>4 \stemDown e'8 [\stemDown e8]"
-"94","\stemDown g''8 [\stemDown c''8] \stemDown e''8 [\stemDown c'''8]","\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]"
-"95","{<<{\voiceOne \stemUp e''16 [\stemUp f''16 \stemUp d''16 \stemUp e''16] c''4} \new Voice {\voiceTwo \stemDown g'8 [\stemDown f'8] e'4}>>}","\stemDown <g c'>8 [\stemDown <g b>8] <c c'>4"
-"96","\stemDown a''16 [\stemDown g''16 \stemDown fis''16 \stemDown g''16] \stemDown c'''8 [\stemDown e''8]","\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' g'>8]"
-"97","\stemDown f''8 [\stemDown a''8] c''4","{<<{\voiceOne r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]} \new Voice {\voiceTwo a2}>>}"
-"98","\stemDown <e'' g''>8 [\stemDown <c'' e''>8] <e'' c'''>4","{<<{\voiceOne r8 c'8 c'4} \new Voice {\voiceTwo c2}>>}"
-"99","{<<{\voiceOne \stemUp a''8. \turn [\stemUp b''16] \stemUp c'''8 [\stemUp e''8]} \new Voice {\voiceTwo c''2}>>}","\stemDown <c' e'>8. [\stemDown b16] \stemDown a8 [\stemDown <c' e'>8]"
-"100","\stemDown e''8 [\stemDown c''8] \stemDown a''8 [\stemDown g''8]","{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo c2}>>}"
-"101","\stemDown <g' c'' g''>8 [\stemDown <g' c''>8] \stemDown <a' c'' f''>8 [\stemDown <c'' f'' a''>8]","e4 \stemDown f8 [\stemDown f8]"
-"102","\stemUp c''8 [\stemUp <e' c''>8] <e' c''>4","\stemDown <c' e'>8 [\stemDown g8] c4"
-"103","\stemDown b''8 [\stemDown d'''16 \stemDown b''16] \stemDown a''8 [\stemDown gis''8]","{<<{\voiceOne r8 <a b d'>8 \stemUp <e c'>8 [\stemUp <e b d'>8]} \new Voice {\voiceTwo f4 s4}>>}"
-"104","\stemDown g''16 [\stemDown f''16 \stemDown e''16 \stemDown d''16] \stemDown c''8 [\stemDown b'8]","{<<{\voiceOne r8 <a d'>8 \stemUp <e a e'>8 [\stemUp <e gis d'>8]} \new Voice {\voiceTwo f4 s4}>>}"
-"105","\stemDown a'8 [\stemDown d''8] \stemDown cis''16 [\stemDown d''16 \stemDown e''16 \stemDown d''16]","{<<{\voiceOne r8 <fis c'>8 \stemUp <fis c'>8 [\stemUp <fis c'>8]} \new Voice {\voiceTwo d2}>>}"
-"106","\stemDown gis''8 [\stemDown e''8] \stemDown a''8 [\stemDown e''8]","<e b d'>4 <e a c'>4"
-"107","\stemDown g''16 [\stemDown fis''16 \stemDown g''16 \stemDown gis''16] \stemDown a''8 [\stemDown d''8]","{<<{\voiceOne r8 <b f'>8 \stemUp <b f'>8 [\stemUp <b f'>8]} \new Voice {\voiceTwo g2}>>}"
-"108","\stemDown a''16 [\stemDown gis''16 \stemDown a''16 \stemDown b''16] \stemDown c'''8 [\stemDown a''8]","{<<{\voiceOne r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]} \new Voice {\voiceTwo f2}>>}"
-"109","{<<{\voiceOne \stemUp f''8. \turn [\stemUp g''16] a''4} \new Voice {\voiceTwo a'2}>>}","{<<{\voiceOne \stemUp a8. [\stemUp g16] f4} \new Voice {\voiceTwo c'2}>>}"
-"110","{<<{\voiceOne \stemUp a''8 [\stemUp g''8] \stemUp fis''8 [\stemUp g''8]} \new Voice {\voiceTwo b'2}>>}","\stemUp g,8 [\stemUp g8] \stemDown <d' f'>8 [\stemDown b8]"
-"111","\stemDown b''8 [\stemDown e'''16 \stemDown d'''16] \stemDown c'''8 [\stemDown a''8]","\stemDown gis8 [\stemDown <b e'>8] \stemDown a8 [\stemDown <c' e'>8]"
-"112","\stemDown b''8 [\stemDown e''8] \stemDown dis''16 [\stemDown e''16 \stemDown d''16 \stemDown b'16]","{<<{\voiceOne r8 <gis d'>8 \stemUp <gis d'>8 [\stemUp <gis d'>8]} \new Voice {\voiceTwo e2}>>}"
-"113","\stemDown e''8 [\stemDown c''8] \stemDown a''8 [\stemDown e''8]","\stemDown a,8 [\stemDown <c' e'>8] \stemDown a8 [\stemDown <c' e'>8]"
-"114","\stemDown b''8 [\stemDown d'''16 \stemDown f'''16] \stemDown e'''8 [\stemDown gis''8]","\stemDown d8 [\stemDown <a b>8] \stemDown e8 [\stemDown <b d'>8]"
-"115","\grace { \stemUp a''8 } bes''4 \grace { \stemUp a''8 } \stemDown bes''8 [\stemDown g''8]","\stemDown c8 [\stemDown <g e'>8] \stemDown <g e'>8 [\stemDown <bes e'>8]"
-"116","{<<{\voiceOne \stemUp a''8. [\stemUp g''16] \stemUp f''8 [\stemUp f''8]} \new Voice {\voiceTwo cis''4 d''4}>>}","{<<{\voiceOne r8 e'8 d'8 r8} \new Voice {\voiceTwo a4 r8 d8}>>}"
-"117","\stemDown f''8 [\stemDown g'16 \stemDown b'16] \stemDown d''8 [\stemDown a''8]","\stemDown g8 [\stemDown <b f'>8] \stemDown g8 [\stemDown <b f'>8]"
-"118","\stemDown e''8. [\stemDown f''16] \stemDown e''8 [\stemDown d''8]","{<<{\voiceOne r8 <b e'>8 \stemUp <b e'>8 [\stemUp <b e'>8]} \new Voice {\voiceTwo gis2}>>}"
-"119","\stemDown f'''8 [\stemDown e'''8] \stemDown c'''8 [\stemDown a''8]","{<<{\voiceOne r8 <a e'>8 \stemUp <a e'>8 [\stemUp <a e'>8]} \new Voice {\voiceTwo e2}>>}"
-"120","\stemUp a'8 [\stemUp <c' a'>8] <c' a'>4","\stemDown <a c'>8 [\stemDown e8] a,4"
-"121","\stemDown a'8 [\stemDown f''8] \stemDown as'16 [\stemDown f''16 \stemDown g'16 \stemDown g''16]","<d' f'>4 \stemDown <c' d'>8 [\stemDown <b d'>8]"
-"122","d''4 r4","\stemDown d8 [\stemDown f'8] d'4"
-"123","\stemDown a''8 [\stemDown f'''8] \stemDown c'''8 [\stemDown a''8]","{<<{\voiceOne r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]} \new Voice {\voiceTwo f2}>>}"
-"124","\stemDown <a' a''>8 [\stemDown <c'' a''>8] <a' a''>4","\stemDown <a c'>8 [\stemDown e8] a,4"
-"125","\stemDown c'''16 [\stemDown f'''16 \stemDown e'''16 \stemDown f'''16] \stemDown g'''16 [\stemDown f'''16 \stemDown e'''16 \stemDown d'''16]","{<<{\voiceOne r8 <c' f'>8 r8 <d' f'>8} \new Voice {\voiceTwo a4 bes4}>>}"
-"126","\stemDown e''8 [\stemDown c''8] \stemDown c'''8 [\stemDown g''8]","{<<{\voiceOne r8 <bes e'>8 \stemUp <bes e'>8 [\stemUp <bes e'>8]} \new Voice {\voiceTwo g2}>>}"
-"127","\stemDown cis''16 [\stemDown d''16 \stemDown f''16 \stemDown a''16] \stemDown g''8 [\stemDown b'8]","{<<{\voiceOne r8 <a d'>8 r8 <d' f'>8} \new Voice {\voiceTwo f4 g4}>>}"
-"128","\stemDown a''8 [\stemDown f''8] \stemDown d''8 [\stemDown b'8]","<f c' d'>4 \stemDown <g b d'>8 [\stemDown <g d' f'>8]"
-"129","\tuplet 3/2 {\grace { \stemUp b'8*3/2 } \stemDown c''8 [\stemDown e''8 \stemDown f''8]} f''4","{<<{\voiceOne r8 <a f'>8 \stemUp <a f'>8 [\stemUp <a f'>8]} \new Voice {\voiceTwo f2}>>}"
-"130","\stemUp g'8 [\stemUp a'16 \stemUp g'16] \stemDown f''8 [\stemDown d''8]","{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b f'>8]} \new Voice {\voiceTwo g2}>>}"
-"131","\grace { \stemUp dis''8 } e''4 \grace { \stemUp dis''8 } \stemDown e''8 [\stemDown cis''8]","{<<{\voiceOne r8 <cis' g'>8 \stemUp <cis' g'>8 [\stemUp <e' g'>8]} \new Voice {\voiceTwo a2}>>}"
-"132","\stemDown a''8 [\stemDown f'''8] \stemDown c'''8 [\stemDown a''8]","{<<{\voiceOne r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]} \new Voice {\voiceTwo f2}>>}"
-"133","\stemUp gis'8 [\stemUp b'8] \stemDown e''8 [\stemDown gis''8]","{<<{\voiceOne r8 <gis d'>8 \stemUp <b e'>8 [\stemUp <b e'>8]} \new Voice {\voiceTwo e2}>>}"
-"134","R2","{<<{\voiceOne a4 \stemUp c'8 [\stemUp e'8]} \new Voice {\voiceTwo a,4 \stemDown c8 [\stemDown e8]}>>}"
-"135","\stemDown g''8 [\stemDown fis''16 \stemDown g''16] \stemDown a''16 [\stemDown g''16 \stemDown f''16 \stemDown d''16]","{<<{\voiceOne r8 <b d'>8 \stemUp <b f'>8 [\stemUp <b f'>8]} \new Voice {\voiceTwo g2}>>}"
-"136","\stemUp e''8 [\stemUp e'8] e'4","\stemDown <e g b>8 [\stemDown <e g c'>8] <e g>4"
-"137","{<<{\voiceOne \stemUp d''8 [\stemUp bes''16 \stemUp d'''16] \stemUp c'''8 [\stemUp e''8]} \new Voice {\voiceTwo r8 <d' g'>8 r8 <g' bes'>8}>>}","bes4 c'4"
-"138","\stemDown a''16 [\stemDown bes''16 \stemDown c'''16 \stemDown d'''16] \stemDown bes''8 [\stemDown g''8]","{<<{\voiceOne r8 <a d'>8 r8 <bes d'>8} \new Voice {\voiceTwo fis4 g4}>>}"
-"139","\stemDown b''8 [\stemDown a''8] g''4","\stemDown <g b d'>8 [\stemDown <fis c' d'>8] <g b f'>4 |"
-"140","\stemDown bes''8 [\stemDown c'''16 \stemDown bes''16] \stemDown a''8 [\stemDown f''8]","{<<{\voiceOne r8 <c' e'>8 r8 <a c'>8} \new Voice {\voiceTwo g4 f4}>>}"
-"141","\stemDown b''16 [\stemDown a''16 \stemDown gis''16 \stemDown fis''16] \stemDown e''8 [\stemDown b''8]","{<<{\voiceOne r8 <gis d'>8 \stemUp <gis d'>8 [\stemUp <gis d'>8]} \new Voice {\voiceTwo e2}>>}"
-"142","\grace { \stemUp b''8 } \stemDown c'''8 [\stemDown b''16 \stemDown a''16] \stemDown c'''8 [\stemDown b''16 \stemDown a''16]","{<<{\voiceOne r8 <c' es'>8 r8 <c' es'>8} \new Voice {\voiceTwo fis4 f4}>>}"
-"143","{<<{\voiceOne \stemUp a''8 [\stemUp g''8] \stemUp f''8 [\stemUp d''8]} \new Voice {\voiceTwo b'2}>>}","\stemUp g,8 [\stemUp g8] \stemDown <d' f'>8 [\stemDown g8]"
-"144","\stemDown e''16 [\stemDown dis''16 \stemDown e''16 \stemDown gis''16] \stemDown b''8 [\stemDown e''8]","{<<{\voiceOne r8 <b e'>8 r8 <d' e'>8} \new Voice {\voiceTwo gis4 gis4}>>}"
-"145","\stemDown d'''8 [\stemDown e'''16 \stemDown f'''16] \stemDown f'''8 [\stemDown g''8]","<gis b f'>4 <g b f'>4"
-"146","\stemDown e'''8. [\stemDown d'''16] \stemDown b''8 [\stemDown c'''8]","{<<{\voiceOne r8 <b e'>8 \stemUp <b e'>8 [\stemUp <b e'>8]} \new Voice {\voiceTwo gis2}>>}"
-"147","\stemDown d''8 [\stemDown c'''8] \stemDown b''8 [\stemDown d''8]","\stemDown d8 [\stemDown <a f'>8] \stemDown e8 [\stemDown <b e'>8]"
-"148","\stemDown a''8 [\stemDown <c'' a''>8] <c'' a''>4","\stemDown <a c'>8 [\stemDown <a e'>8] <a c'>4"
-"149","\stemDown f''16 [\stemDown g''16 \stemDown a''16 \stemDown f''16] \stemDown d''8 [\stemDown b'8]","{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <d' f'>8]} \new Voice {\voiceTwo g2}>>}"
-"150","\stemDown d'''16 [\stemDown c'''16 \stemDown b''16 \stemDown a''16] \stemDown b''8 [\stemDown g''8]","{<<{\voiceOne r8 <c' d'>8 r8 <b d'>8} \new Voice {\voiceTwo fis4 g4}>>}"
-"151","\stemDown c'''16 [\stemDown e'''16 \stemDown f'''16 \stemDown g'''16] \stemDown a'''8 [\stemDown a'''8]","{<<{\voiceOne r8 <c' f'>8 r8 <c' f'>8} \new Voice {\voiceTwo a4 f4}>>}"
-"152","\stemDown b''8 [\stemDown d'''16 \stemDown f'''16] \stemDown e'''8 [\stemDown gis''8]","{<<{\voiceOne r8 <a b>8 r8 <b d'>8} \new Voice {\voiceTwo d4 e4}>>}"
-"153","\stemDown a''8 [\stemDown c'''16 \stemDown b''16] a''4","\stemDown <a c'>8 [\stemDown <e gis d'>8] <a c'>4"
-"154","\stemDown e''16 [\stemDown e'''16 \stemDown c'''16 \stemDown a''16] \stemDown gis''16 [\stemDown e''16 \stemDown b''16 \stemDown gis''16]","\stemDown e8 [\stemDown <c' e'>8] \stemDown <e b d'>8 [\stemDown <e b d'>8]"
-"155","\tuplet 3/2 {\stemDown e''8 [\stemDown g''8 \stemDown c''8] } a''4","\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]"
-"156","\stemDown g''16 [\stemDown a''16 \stemDown bes''16 \stemDown c'''16] \stemDown a''8 [\stemDown f''8]","{<<{\voiceOne r8 <g c'>8 r8 <a c'>8} \new Voice {\voiceTwo e4 f4}>>}"
-"157","\stemDown a''8 [\stemDown a'''8] a''4","\stemDown <a c'>8 [\stemDown e8] a,4"
-"158","\stemDown cis'''16 [\stemDown d'''16 \stemDown e'''16 \stemDown f'''16] \stemDown c'''8 [\stemDown e''8]","\clef ""treble"" \stemUp <bes d' g'>8 [\stemUp <b d' gis'>8] \stemUp <c' f' a'>8 [\stemUp <c' g' bes'>8]"
-"159","\stemDown c''8 [\stemDown b''8] \stemDown a''8 [\stemDown c''8]","\stemDown e8 [\stemDown <c' e'>8] \stemDown f8 [\stemDown <a f'>8]"
-"160","\stemDown c'''8 [\stemDown d'''16 \stemDown c'''16] \stemDown b''8 [\stemDown e''8]","{<<{\voiceOne r8 <c' e'>8 r8 <d' e'>8} \new Voice {\voiceTwo a4 gis4}>>}"
-"161","\stemDown a''8 [\stemDown gis''16 \stemDown a''16] \stemDown b''8 [\stemDown e''8]","{<<{\voiceOne r8 <b d'>8 r8 <gis d' e'>8} \new Voice {\voiceTwo f4 e4}>>}"
-"162","\stemDown d'''8 [\stemDown c'''8] \stemDown a''8 [\stemDown a''8]","\stemDown a8 [\stemDown <c' e'>8] \stemDown f8 [\stemDown <c' d'>8]"
-"163","\stemDown g''8 [\grace { \stemUp b''8 } \stemDown c'''8] \stemDown c'''8 [\stemDown c''8]","\stemDown <c e g>8 [\stemDown c'8] \stemDown c'8 [\stemDown c8]"
-"164","f'''4 \stemDown d'''8 [\stemDown a''8]","\stemDown d8 [\stemDown <d' f'>8] \stemDown <d' f'>8 [\stemDown <d' f'>8]"
-"165","\stemDown c'''8 [\stemDown a'16 \stemDown b'16] \stemDown c''16 [\stemDown c''16 \stemDown c''16 \stemDown d''16]","\stemDown <a, a>8 [\stemDown <c' e'>8] \stemDown a8 [\stemDown <c' e'>8]"
-"166","\stemDown a''8. [\stemDown g''16] \stemDown e''8 [\stemDown f''8]","{<<{\voiceOne r8 <cis' g'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]} \new Voice {\voiceTwo a2}>>}"
-"167","\stemDown a''16 [\stemDown b''16 \stemDown c'''16 \stemDown d'''16] \stemDown e'''8 [\stemDown a''8]","{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo a2}>>}"
-"168","\stemDown a''16 [\stemDown g''16 \stemDown fis''16 \stemDown g''16] \stemDown a''8 [\stemDown b''8]","{<<{\voiceOne r8 <b f'>8 \stemUp <d' f'>8 [\stemUp <d' f'>8]} \new Voice {\voiceTwo g2}>>}"
-"169","\stemDown g''8 [\stemDown fis''16 \stemDown g''16] \stemDown c'''8 [\stemDown e''8]","<g b f'>4 \stemDown <g c' e'>8 [\stemDown <g bes c'>8] |"
-"170","\stemDown a''8 [\stemDown f'''8] \stemDown c'''8 [\stemDown a''8]","\stemDown f8 [\stemDown <a f'>8] \stemDown a8 [\stemDown <c' f'>8]"
-"171","c'''4 r4","\stemDown <c' e'>8 [\stemDown g'8] <c' e'>4"
-"172","\stemDown gis''8 [\stemDown e'''8] \stemDown c'''8 [\stemDown a''8]","{<<{\voiceOne r8 <gis e'>8 r8 <c' e'>8} \new Voice {\voiceTwo e4 a4}>>}"
-"173","\stemDown e'''8 [\stemDown d'''8] c'''4","{<<{\voiceOne \stemUp g8 [\stemUp f8] e4} \new Voice {\voiceTwo c2}>>}"
-"174","{<<{\voiceOne \stemUp c'''8. [\stemUp bes''16] \stemUp a''8 [\stemUp a''8]} \new Voice {\voiceTwo c''4 \stemDown c''8 [\stemDown c''8]}>>}","{<<{\voiceOne r8 <c' e'>8 r8 <c' f'>8} \new Voice {\voiceTwo g4 f4}>>}"
-"175","\stemDown f''16 [\stemDown e''16 \stemDown e''16 \stemDown c'''16] \stemDown c'''8 [\stemDown e''8]","{<<{\voiceOne r8 <c' e'>8 r8 <c' e'>8} \new Voice {\voiceTwo g4 a4}>>}"
-"176","\stemDown <a' f''>8 [\stemDown <c'' a''>8] <a' f''>4","\stemDown a'8 [\stemDown f'8] f4"
-"177","\stemDown g''16 [\stemDown fis''16 \stemDown g''16 \stemDown d'''16] \stemDown c'''16 [\stemDown bes''16 \stemDown g''16 \stemDown e''16]","\clef ""treble"" {<<{\voiceOne r8 <d' g'>8 r8 <g' bes'>8} \new Voice {\voiceTwo bes4 c'4}>>}"
-"178","\stemDown cis''8 [\stemDown a''8] a'4","\clef ""treble"" <a a'>4 a4"
-"179","\stemDown c'''8 [\stemDown b''16 \stemDown c'''16] \stemDown e'''16 [\stemDown d'''16 \stemDown bes''16 \stemDown g''16] |","{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo g2}>>}"
-"180","\stemDown bes''16 [\stemDown a''16 \stemDown gis''16 \stemDown a''16] f''4","{<<{\voiceOne r8 <c' f'>8 r8 <c' f'>8} \new Voice {\voiceTwo f4 a4}>>}"
-"181","\grace { \stemUp b'8 } c''4 \grace { \stemUp b'8 } c''4","{<<{\voiceOne r8 <a f'>8 \stemUp <a f'>8 [\stemUp <a f'>8]} \new Voice {\voiceTwo f2}>>}"
-"182","\stemDown c'''8 [\stemDown b''8] a''4","{<<{\voiceOne \stemUp <c' e'>8 [\stemUp d'8] c'4} \new Voice {\voiceTwo a2}>>}"
-"183","\stemDown c''16 [\stemDown d''16 \stemDown e''16 \stemDown f''16] \stemDown g''8 [\stemDown bes''8]","{<<{\voiceOne r8 <c' e'>8 r8 <c' e'>8} \new Voice {\voiceTwo bes4 g4}>>}"
-"184","\stemDown c''8 [\stemDown b'8] a'4","{<<{\voiceOne \stemUp e'8 [\stemUp d'8] c'4} \new Voice {\voiceTwo a2}>>}"
-"185","\stemDown bes''8 [\stemDown c'''16 \stemDown d'''16] \stemDown c'''8 [\stemDown f''8]","<g c' e'>4 <a c' f'>4"
-"186","\tuplet 3/2 {\stemDown d''8 [\stemDown f''8 \stemDown a''8] } a''4","\stemDown d8 [\stemDown <d' f'>8] \stemDown <d' f'>8 [\stemDown <d' f'>8]"
-"187","\grace { \stemUp c''8 } \stemDown e''8 [\grace { \stemUp e''8 } \stemDown g''8] \grace { \stemUp g''8 } \stemDown bes''8 [\grace {\stemUp bes''8 } \stemDown d'''8]","\grace {s8} {<<{\voiceOne r8 <c' e'>8 r8 <c' e'>8} \new Voice {\voiceTwo bes4 g4}>>}"
-"188","\stemDown c''8 [\stemDown e''8] c'''4","\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]"
-"189","\tuplet 3/2 {\stemDown a''8 [\stemDown gis''8 \stemDown g''8] } \stemDown g''8 [\stemDown f''8]","\clef ""treble"" {<<{\voiceOne r8 <d' f' g'>8 \stemUp <d' f' g'>8 [\stemUp <d' f' g'>8]} \new Voice {\voiceTwo b2}>>}"
-"190","\stemDown a''8 [\stemDown c'''8] a''4","\stemDown <a c'>8 [\stemDown <a e'>8] <a c'>4"
-"191","\stemDown g''16 [\stemDown f''16 \stemDown e''16 \stemDown g''16] f''4","\stemDown d8 [\stemDown <a f'>8] \stemDown <a f'>8 [\stemDown <a f'>8]"
-"192","\stemDown f''8 [\stemDown <c'' a''>8] <a' f''>4","\stemUp <f, a,>8 [\stemUp c,8] a,,4"
+__author__ = 'Robbert Harms'
+__date__ = '2024-04-29'
+__maintainer__ = 'Robbert Harms'
+__email__ = 'robbert@xkls.nl'
+__licence__ = 'LGPL v3'
+
+from pathlib import Path
+
+from musical_games.dice_games.base import SimpleBarCollection, SimpleBar
+from musical_games.dice_games.data_csv import SimpleBarCollectionCSVWriter
+
+piano_right_hand_voice_1 = r"""\stemDown d''16 [\stemDown e''16 \stemDown f''16 \stemDown d''16] \stemDown b'8 [\stemDown d''8]
+\stemDown a''16 [\stemDown gis''16 \stemDown a''16 \stemDown b''16] \stemDown c'''8 [\stemDown d'''8]
+\stemDown <c'' g''>8 [\stemDown <c'' fis''>8] <b' g''>4
+\stemDown g'8 [\stemDown c''16 \stemDown d''16] \stemDown e''16 [\stemDown f''16 \stemDown g''8]
+\stemDown e''8. [\stemDown d''16] \stemDown b'8 [\stemDown b'8]
+\stemDown cis''16 [\stemDown cis''16 \stemDown e''16 \stemDown cis''16] \stemDown a'8 [\stemDown e''8]
+\stemDown c''8 [\stemDown <g' e''>8] <e' c''>4
+\stemDown c''8 [\stemDown c''16 \stemDown b'16] \stemUp a'8 [\stemUp e'8]
+\stemDown b'8 [\stemDown a''8] \stemDown g''8 [\stemDown f''8]
+\stemUp b'8 [\stemUp g'8] g''4
+\stemDown f''16 [\stemDown e''16 \stemDown f''16 \stemDown a''16] \stemDown f''8 [\stemDown b'8]
+\stemDown <e'' g''>8 [\stemDown <g' c''>8] <c'' e''>4
+<a' c''>4 <g' cis''>4
+\stemDown e''16 [\stemDown d''16 \stemDown cis''16 \stemDown e''16] d''4
+\stemUp <e' g'>8 [\stemUp <f' a'>16 \stemUp <e' g'>16] \stemUp <e' g'>8 [\stemUp <e' c''>8]
+\stemDown g''16 [\stemDown a''16 \stemDown b''16 \stemDown c'''16] \stemDown d'''8 [\stemDown g''8]
+\stemDown e''8 [\grace { \stemUp d''8 } \stemDown e''8] e'4
+\stemDown d'''16 [\stemDown cis'''16 \stemDown d'''16 \stemDown e'''16] \stemDown f'''8 [\stemDown a''8]
+\stemDown d'''8 [\stemDown a''8] \stemDown b''8 [\stemDown e'''8]
+\stemDown g''16 [\stemDown fis''16 \stemDown fis''16 \stemDown e'''16] \stemDown e'''16 [\stemDown d'''16 \stemDown c'''16 \stemDown a''16]
+\stemDown e''8 [\stemDown d''8] \stemDown a''16 [\stemDown g''16 \stemDown f''16 \stemDown d''16]
+\stemDown c'''8 [\stemDown d'''16 \stemDown es'''16] \stemDown g''8 [\stemDown e''8]
+\stemDown e''8 [\stemDown b'8] \stemDown gis''8 [\stemDown e''8]
+\stemDown c'''8 [\stemDown bes''8] \stemDown g''8 [\stemDown e''8]
+\stemDown e''8 [\stemDown c''8] \stemDown g''8 [\stemDown e''8]
+\stemDown a'8 [\stemDown c''8] \stemDown e''8 [\stemDown a''8]
+\stemDown c''8 [\stemDown e''8] \stemDown a''8 [\stemDown c'''8]
+\stemDown e''8 [\stemDown d''8] c''4
+\stemDown d''8 [\stemDown e''16 \stemDown d''16] \stemDown a'8 [\stemDown f''8]
+\stemUp e''8 [\stemUp c'''8] g''4
+\stemDown f''16 [\stemDown e''16 \stemDown dis''16 \stemDown e''16] \stemDown c'''8 [\stemDown e''8]
+<g' c'' e''>4 <g' b' d''>8 r8
+\stemDown g''8 [\stemDown b'8] \stemDown fis''8 [\stemDown a'8]
+\stemDown a''8 [\stemDown <c'' a''>8] <a' a''>4
+\stemDown c''16 [\stemDown d''16 \stemDown e''16 \stemDown c''16] \stemDown a'8 [\stemDown a''8]
+\stemDown a''8 [\stemDown f''8] \stemDown d''8 [\stemDown c''8]
+\stemDown a''16 [\stemDown f''16 \stemDown e''16 \stemDown d''16] \stemDown c''16 [\stemDown g''16 \stemDown b'16 \stemDown d''16]
+\stemDown f''16 [\stemDown e''16 \stemDown f''16 \stemDown g''16] \stemDown a''8 [\stemDown a''8]
+\stemUp e''8 [\stemUp f''16 \stemUp e''16] \stemUp dis''8 [\stemUp e''8]
+\stemUp <e' g'>8 [\stemUp <f' a'>16 \stemUp <e' g'>16] \stemDown <e' c''>8 [\stemDown <c'' e''>8]
+\stemUp gis'16 [\stemUp a'16 \stemUp b'16 \stemUp gis'16] \stemUp e'8 [\stemUp e''8]
+\stemDown a''8 [\stemDown gis''16 \stemDown a''16] \stemDown bes''8 [\stemDown a''8]
+\stemDown a'8 [\stemDown bes'16 \stemDown b'16] \tuplet 3/2 {\stemDown c''8 [\stemDown f''8 \stemDown a'8]}
+\stemDown c'''8 [\stemDown d''8] \stemDown b''8 [\stemDown d''8]
+\stemDown b'8 [\stemDown d''8] \stemDown g''8 [\stemDown b''8]
+\stemDown c''8 [\stemDown e''8] g'4
+\stemDown c''8 [\stemDown e''8] g''4
+\stemDown <gis' d''>8 [\stemDown <gis' e''>8] \stemDown <a' fis''>8 [\stemDown <b' gis''>8]
+\stemDown b''16 [\stemDown c'''16 \stemDown d'''16 \stemDown b''16] \stemDown g''8 [\stemDown f'''8]
+\stemUp c''8 [\stemUp <e' c''>8] <e' c''>4
+\stemDown c''8 [\stemDown <g' e''>8] <e' c''>4
+\stemDown c''8 [\stemDown c'''8] c''4
+\stemDown f''8 [\stemDown a''8] f''4
+\stemUp b''8 [\stemUp d'''16 \stemUp b''16] \stemUp a''8 [\stemUp gis''8]
+\stemUp d''8 [\stemUp e''16 \stemUp d''16] \stemUp d''8 [\stemUp g''8]
+\stemDown a''8 [\stemDown e''8] \stemDown cis'''8 [\stemDown e'''8]
+\stemDown bes'8 [\stemDown c''16 \stemDown e''16] g''4
+\stemDown g''8 [\stemDown d'''16 \stemDown dis'''16] \stemDown e'''8 [\stemDown g''8]
+\stemDown c''16 [\stemDown d''16 \stemDown e''16 \stemDown d''16] c''4
+\stemDown a'8 [\stemDown d''16 \stemDown e''16] \stemDown f''16 [\stemDown g''16 \stemDown a''8]
+\stemDown b''8 [\stemDown f''16 \stemDown b''16] \stemDown d'''8 [\stemDown f'''8]
+\stemDown g''8 [\stemDown fis''16 \stemDown g''16] \stemDown as''8 [\stemDown f''16 \stemDown d''16]
+\stemDown c'''8 [\stemDown a''8] \stemDown f'''8 [\stemDown a''8]
+\stemDown f''8 [\stemDown <c'' a''>8] <a' f''>4
+\stemUp e'8 [\stemUp c''16 \stemUp e'16] \stemDown g'8 [\stemDown e''8]
+\stemDown g''16 [\stemDown f''16 \stemDown f''16 \stemDown d'''16] \stemDown d'''8 [\stemDown f''8]
+\stemDown c'''8 [\stemDown d'''16 \stemDown e'''16] \stemDown f'''8 [\stemDown a''8]
+\stemDown d'''8 [\stemDown c'''8] \stemDown bes''8 [\stemDown a''8]
+\stemDown c'''16 [\stemDown bes''16 \stemDown a''16 \stemDown g''16] \stemDown a''8 [\stemDown f''8]
+\stemDown g''8 [\stemDown <b' g''>8] <b' g''>4
+\stemDown d''8 [\stemDown e''16 \stemDown d''16] \stemDown c'''8 [\stemDown a''8]
+\stemDown a''8 [\stemDown f''16 \stemDown d''16] \stemDown c''16 [\stemDown g''16 \stemDown b'16 \stemDown d''16]
+\stemDown a''16 [\stemDown b''16 \stemDown c'''16 \stemDown d'''16] \stemDown e'''8 [\stemDown gis''8]
+\stemDown d'''8 [\stemDown c'''8] \stemDown a''8 [\stemDown e''8]
+\stemDown e''8 [\stemDown e''16 \stemDown d''16] \stemDown a''8 [\stemDown d''8]
+\stemDown a''16 [\stemDown gis''16 \stemDown a''16 \stemDown b''16] c'''4
+\stemUp <e' c''>8 [\stemUp <e' c''>8] \stemUp <f' d''>8 [\stemUp <g' e''>8]
+\stemDown e''16 [\stemDown d''16 \stemDown cis''16 \stemDown d''16] \stemDown a''8 [\stemDown d''8]
+\stemDown c''8 [\stemDown a'8] \stemDown a''8 [\stemDown e''8] |
+\stemDown a''16 [\stemDown g''16 \stemDown f''16 \stemDown e''16] \stemDown f''8 [\stemDown d''8]
+\stemDown c'''16 [\stemDown d'''16 \stemDown e'''16 \stemDown f'''16] \stemDown g'''8 [\stemDown c'''8]
+\grace { \stemUp ais''8 } b''4 \grace { \stemUp ais''8 } \stemDown b''8 [\stemDown e'''8]
+a''2
+\stemDown c''8 [\stemDown e''8] \stemDown a'8 [\stemDown a''8]
+\stemUp d''16 [\stemUp cis''16 \stemUp d''16 \stemUp e''16] \stemUp f''8 [\stemUp d''8]
+\stemDown c'''8 [\stemDown a''8] \stemDown b''8 [\stemDown c'''8]
+\stemUp <e' g'>8 [\stemUp <f' a'>16 \stemUp <e' g'>16] \stemUp <e' g'>8 [\stemUp <g' e''>8]
+\stemDown e''8 [\stemDown e''16 \stemDown d''16] \stemDown c''8 [\stemDown a'8]
+\stemDown <c'' c'''>8 [\stemDown <g'' b''>16 \stemDown <f'' a''>16] \stemDown <e'' g''>8 [\stemDown <f'' a''>8]
+\stemDown e'''8 [\stemDown c'''8] \stemDown g''8 [\stemDown e''8]
+\stemDown g''8 [\stemDown b'8] c''4
+\stemDown fis''16 [\stemDown g''16 \stemDown a''16 \stemDown fis''16] \stemDown d''8 [\stemDown c'''8]
+\stemDown b''8 [\stemDown e''8] \stemDown e'''8 [\stemDown e''8]
+\stemDown g''8 [\stemDown c''8] \stemDown e''8 [\stemDown c'''8]
+\stemUp e''16 [\stemUp f''16 \stemUp d''16 \stemUp e''16] c''4
+\stemDown a''16 [\stemDown g''16 \stemDown fis''16 \stemDown g''16] \stemDown c'''8 [\stemDown e''8]
+\stemDown f''8 [\stemDown a''8] c''4
+\stemDown <e'' g''>8 [\stemDown <c'' e''>8] <e'' c'''>4
+\stemUp a''8. \turn [\stemUp b''16] \stemUp c'''8 [\stemUp e''8]
+\stemDown e''8 [\stemDown c''8] \stemDown a''8 [\stemDown g''8]
+\stemDown <g' c'' g''>8 [\stemDown <g' c''>8] \stemDown <a' c'' f''>8 [\stemDown <c'' f'' a''>8]
+\stemUp c''8 [\stemUp <e' c''>8] <e' c''>4
+\stemDown b''8 [\stemDown d'''16 \stemDown b''16] \stemDown a''8 [\stemDown gis''8]
+\stemDown g''16 [\stemDown f''16 \stemDown e''16 \stemDown d''16] \stemDown c''8 [\stemDown b'8]
+\stemDown a'8 [\stemDown d''8] \stemDown cis''16 [\stemDown d''16 \stemDown e''16 \stemDown d''16]
+\stemDown gis''8 [\stemDown e''8] \stemDown a''8 [\stemDown e''8]
+\stemDown g''16 [\stemDown fis''16 \stemDown g''16 \stemDown gis''16] \stemDown a''8 [\stemDown d''8]
+\stemDown a''16 [\stemDown gis''16 \stemDown a''16 \stemDown b''16] \stemDown c'''8 [\stemDown a''8]
+\stemUp f''8. \turn [\stemUp g''16] a''4
+\stemUp a''8 [\stemUp g''8] \stemUp fis''8 [\stemUp g''8]
+\stemDown b''8 [\stemDown e'''16 \stemDown d'''16] \stemDown c'''8 [\stemDown a''8]
+\stemDown b''8 [\stemDown e''8] \stemDown dis''16 [\stemDown e''16 \stemDown d''16 \stemDown b'16]
+\stemDown e''8 [\stemDown c''8] \stemDown a''8 [\stemDown e''8]
+\stemDown b''8 [\stemDown d'''16 \stemDown f'''16] \stemDown e'''8 [\stemDown gis''8]
+\grace { \stemUp a''8 } bes''4 \grace { \stemUp a''8 } \stemDown bes''8 [\stemDown g''8]
+\stemUp a''8. [\stemUp g''16] \stemUp f''8 [\stemUp f''8]
+\stemDown f''8 [\stemDown g'16 \stemDown b'16] \stemDown d''8 [\stemDown a''8]
+\stemDown e''8. [\stemDown f''16] \stemDown e''8 [\stemDown d''8]
+\stemDown f'''8 [\stemDown e'''8] \stemDown c'''8 [\stemDown a''8]
+\stemUp a'8 [\stemUp <c' a'>8] <c' a'>4
+\stemDown a'8 [\stemDown f''8] \stemDown as'16 [\stemDown f''16 \stemDown g'16 \stemDown g''16]
+d''4 r4
+\stemDown a''8 [\stemDown f'''8] \stemDown c'''8 [\stemDown a''8]
+\stemDown <a' a''>8 [\stemDown <c'' a''>8] <a' a''>4
+\stemDown c'''16 [\stemDown f'''16 \stemDown e'''16 \stemDown f'''16] \stemDown g'''16 [\stemDown f'''16 \stemDown e'''16 \stemDown d'''16]
+\stemDown e''8 [\stemDown c''8] \stemDown c'''8 [\stemDown g''8]
+\stemDown cis''16 [\stemDown d''16 \stemDown f''16 \stemDown a''16] \stemDown g''8 [\stemDown b'8]
+\stemDown a''8 [\stemDown f''8] \stemDown d''8 [\stemDown b'8]
+\tuplet 3/2 {\grace { \stemUp b'8*3/2 } \stemDown c''8 [\stemDown e''8 \stemDown f''8]} f''4
+\stemUp g'8 [\stemUp a'16 \stemUp g'16] \stemDown f''8 [\stemDown d''8]
+\grace { \stemUp dis''8 } e''4 \grace { \stemUp dis''8 } \stemDown e''8 [\stemDown cis''8]
+\stemDown a''8 [\stemDown f'''8] \stemDown c'''8 [\stemDown a''8]
+\stemUp gis'8 [\stemUp b'8] \stemDown e''8 [\stemDown gis''8]
+R2
+\stemDown g''8 [\stemDown fis''16 \stemDown g''16] \stemDown a''16 [\stemDown g''16 \stemDown f''16 \stemDown d''16]
+\stemUp e''8 [\stemUp e'8] e'4
+\stemUp d''8 [\stemUp bes''16 \stemUp d'''16] \stemUp c'''8 [\stemUp e''8]
+\stemDown a''16 [\stemDown bes''16 \stemDown c'''16 \stemDown d'''16] \stemDown bes''8 [\stemDown g''8]
+\stemDown b''8 [\stemDown a''8] g''4
+\stemDown bes''8 [\stemDown c'''16 \stemDown bes''16] \stemDown a''8 [\stemDown f''8]
+\stemDown b''16 [\stemDown a''16 \stemDown gis''16 \stemDown fis''16] \stemDown e''8 [\stemDown b''8]
+\grace { \stemUp b''8 } \stemDown c'''8 [\stemDown b''16 \stemDown a''16] \stemDown c'''8 [\stemDown b''16 \stemDown a''16]
+\stemUp a''8 [\stemUp g''8] \stemUp f''8 [\stemUp d''8]
+\stemDown e''16 [\stemDown dis''16 \stemDown e''16 \stemDown gis''16] \stemDown b''8 [\stemDown e''8]
+\stemDown d'''8 [\stemDown e'''16 \stemDown f'''16] \stemDown f'''8 [\stemDown g''8]
+\stemDown e'''8. [\stemDown d'''16] \stemDown b''8 [\stemDown c'''8]
+\stemDown d''8 [\stemDown c'''8] \stemDown b''8 [\stemDown d''8]
+\stemDown a''8 [\stemDown <c'' a''>8] <c'' a''>4
+\stemDown f''16 [\stemDown g''16 \stemDown a''16 \stemDown f''16] \stemDown d''8 [\stemDown b'8]
+\stemDown d'''16 [\stemDown c'''16 \stemDown b''16 \stemDown a''16] \stemDown b''8 [\stemDown g''8]
+\stemDown c'''16 [\stemDown e'''16 \stemDown f'''16 \stemDown g'''16] \stemDown a'''8 [\stemDown a'''8]
+\stemDown b''8 [\stemDown d'''16 \stemDown f'''16] \stemDown e'''8 [\stemDown gis''8]
+\stemDown a''8 [\stemDown c'''16 \stemDown b''16] a''4
+\stemDown e''16 [\stemDown e'''16 \stemDown c'''16 \stemDown a''16] \stemDown gis''16 [\stemDown e''16 \stemDown b''16 \stemDown gis''16]
+\tuplet 3/2 {\stemDown e''8 [\stemDown g''8 \stemDown c''8] } a''4
+\stemDown g''16 [\stemDown a''16 \stemDown bes''16 \stemDown c'''16] \stemDown a''8 [\stemDown f''8]
+\stemDown a''8 [\stemDown a'''8] a''4
+\stemDown cis'''16 [\stemDown d'''16 \stemDown e'''16 \stemDown f'''16] \stemDown c'''8 [\stemDown e''8]
+\stemDown c''8 [\stemDown b''8] \stemDown a''8 [\stemDown c''8]
+\stemDown c'''8 [\stemDown d'''16 \stemDown c'''16] \stemDown b''8 [\stemDown e''8]
+\stemDown a''8 [\stemDown gis''16 \stemDown a''16] \stemDown b''8 [\stemDown e''8]
+\stemDown d'''8 [\stemDown c'''8] \stemDown a''8 [\stemDown a''8]
+\stemDown g''8 [\grace { \stemUp b''8 } \stemDown c'''8] \stemDown c'''8 [\stemDown c''8]
+f'''4 \stemDown d'''8 [\stemDown a''8]
+\stemDown c'''8 [\stemDown a'16 \stemDown b'16] \stemDown c''16 [\stemDown c''16 \stemDown c''16 \stemDown d''16]
+\stemDown a''8. [\stemDown g''16] \stemDown e''8 [\stemDown f''8]
+\stemDown a''16 [\stemDown b''16 \stemDown c'''16 \stemDown d'''16] \stemDown e'''8 [\stemDown a''8]
+\stemDown a''16 [\stemDown g''16 \stemDown fis''16 \stemDown g''16] \stemDown a''8 [\stemDown b''8]
+\stemDown g''8 [\stemDown fis''16 \stemDown g''16] \stemDown c'''8 [\stemDown e''8]
+\stemDown a''8 [\stemDown f'''8] \stemDown c'''8 [\stemDown a''8]
+c'''4 r4
+\stemDown gis''8 [\stemDown e'''8] \stemDown c'''8 [\stemDown a''8]
+\stemDown e'''8 [\stemDown d'''8] c'''4
+\stemUp c'''8. [\stemUp bes''16] \stemUp a''8 [\stemUp a''8]
+\stemDown f''16 [\stemDown e''16 \stemDown e''16 \stemDown c'''16] \stemDown c'''8 [\stemDown e''8]
+\stemDown <a' f''>8 [\stemDown <c'' a''>8] <a' f''>4
+\stemDown g''16 [\stemDown fis''16 \stemDown g''16 \stemDown d'''16] \stemDown c'''16 [\stemDown bes''16 \stemDown g''16 \stemDown e''16]
+\stemDown cis''8 [\stemDown a''8] a'4
+\stemDown c'''8 [\stemDown b''16 \stemDown c'''16] \stemDown e'''16 [\stemDown d'''16 \stemDown bes''16 \stemDown g''16] |
+\stemDown bes''16 [\stemDown a''16 \stemDown gis''16 \stemDown a''16] f''4
+\grace { \stemUp b'8 } c''4 \grace { \stemUp b'8 } c''4
+\stemDown c'''8 [\stemDown b''8] a''4
+\stemDown c''16 [\stemDown d''16 \stemDown e''16 \stemDown f''16] \stemDown g''8 [\stemDown bes''8]
+\stemDown c''8 [\stemDown b'8] a'4
+\stemDown bes''8 [\stemDown c'''16 \stemDown d'''16] \stemDown c'''8 [\stemDown f''8]
+\tuplet 3/2 {\stemDown d''8 [\stemDown f''8 \stemDown a''8] } a''4
+\grace { \stemUp c''8 } \stemDown e''8 [\grace { \stemUp e''8 } \stemDown g''8] \grace { \stemUp g''8 } \stemDown bes''8 [\grace {\stemUp bes''8 } \stemDown d'''8]
+\stemDown c''8 [\stemDown e''8] c'''4
+\tuplet 3/2 {\stemDown a''8 [\stemDown gis''8 \stemDown g''8] } \stemDown g''8 [\stemDown f''8]
+\stemDown a''8 [\stemDown c'''8] a''4
+\stemDown g''16 [\stemDown f''16 \stemDown e''16 \stemDown g''16] f''4
+\stemDown f''8 [\stemDown <c'' a''>8] <a' f''>4"""
+
+piano_right_hand_voice_2 = r"""s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+c''2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+| c''2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+d''4 \stemDown c''8 [\stemDown b'8]
+f'4 f'4
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+f'4 r4
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+\stemDown g'8 [\stemDown f'8] e'4
+s2
+s2
+s2
+c''2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+a'2
+b'2
+s2
+s2
+s2
+s2
+s2
+cis''4 d''4
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+r8 <d' g'>8 r8 <g' bes'>8
+s2
+s2
+s2
+s2
+s2
+b'2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+c''4 \stemDown c''8 [\stemDown c''8]
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2
+s2"""
+
+piano_left_hand_voice_1 = r"""r8 <b f'>8 \stemUp <d' f'>8 [\stemUp <b f'>8]
+\stemDown a8 [\stemDown <c' e'>8] \stemDown d8 [\stemDown <a d'>8]
+\stemDown <g d'>8 [\stemDown <a d'>8] <g d'>4
+\stemDown e8 [\stemDown g8] \stemDown c'8 [\stemDown e'8]
+\clef "treble" r8 <b e'>8 \stemUp <d' e'>8 [\stemUp <d' e'>8]
+\clef "bass" r8 <e' g'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]
+\stemDown <c' e'>8 [\stemDown c'8] c4
+\stemDown a,8 [\stemDown <a c'>8] \stemDown <a c'>8 [\stemDown <a c'>8]
+r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]
+\stemDown <g b d'>8 [\stemDown <g b>8] <g b>4
+\stemDown f8 [\stemDown <a d'>8] \stemDown g8 [\stemDown <d' f'>8]
+\stemDown c8 [\stemDown e'8] c'4
+<f f'>4 \stemDown <a e'>8 [\stemDown es'8]
+r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]
+r8 c'8 \stemUp c'8 [\stemUp c'8]
+\clef "treble" r8 <f' g'>8 \stemUp <f' g'>8 [\stemUp <f' g'>8]
+\clef "bass" \stemDown <e gis b>8 [\grace { \stemUp dis'8 } \stemDown e'8] e4
+r8 <d' f'>8 \stemUp <d' f'>8 [\stemUp <d' f'>8]
+<fis c' d'>4 \stemDown <g b d'>8 [\stemDown <gis b d'>8] |
+r8 <a c'>8 \stemUp <a c'>8 [\stemUp <fis d'>8]
+r8 <b f'>8 r8 <b f'>8
+<fis a c' es'>4 <g c' e'>4
+\stemDown g8 [\stemDown <d' e'>8] \stemDown b8 [\stemDown <d' e'>8]
+\stemDown g8 [\stemDown <c' e'>8] \stemDown bes8 [\stemDown <c' g'>8]
+r8 <bes c'>8 \stemUp <bes c'>8 [\stemUp <bes c'>8]
+\stemDown a8 [\stemDown c'8] \stemDown e'8 [\stemDown a'8]
+r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+\stemDown <g c' e'>8 [\stemDown <g b f'>8] <c' e'>4
+r8 <a d'>8 r8 <a d'>8
+\stemDown c8 [\stemDown e8] \stemDown <c' e'>8 [\stemDown g8]
+\stemDown c8 [\stemDown <c' e'>8] \stemDown a8 [\stemDown <c' e'>8]
+g2
+\stemDown e8 [\stemDown <g b>8] \stemDown b,8 [\stemDown <fis b>8]
+\stemDown <a c'>8 [\stemDown <a e'>8] <a c'>4
+r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+<f a d'>4 <fis a d'>4
+\stemDown f8 [\stemDown <a d'>8] \stemDown <g c' e'>8 [\stemDown <g b f'>8]
+r8 <a c'>8 \stemUp <a c'>8 [\stemUp <a c'>8]
+\stemDown c8 [\stemDown g8] \stemDown <c' e'>8 [\stemDown g8] |
+r8 c'8 \stemUp c'8 [\stemUp c'8]
+r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]
+r8 <cis' e'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]
+r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]
+r8 <fis c'>8 r8 b8
+r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]
+\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
+\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
+\stemDown e8 [\stemDown e'8] \stemDown <dis' e'>8 [\stemDown <d' e'>8]
+r8 <b f'>8 \stemUp <b d'>8 [\stemUp <b d'>8]
+\stemDown <c' e'>8 [\stemDown g8] c4
+\stemDown <c' e'>8 [\stemDown c'8] c4
+\stemDown <c' e'>8 [\stemDown <e' g'>8] <c' e'>4
+\stemDown <f a>8 [\stemDown c'8] <f a>4
+r8 f'8 \stemUp e'8 [\stemUp d'8]
+r8 b8 \stemUp b8 [\stemUp b8]
+r8 <cis' g'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]
+\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
+<g b f'>4 <g c' e'>4
+\stemDown <g c' e'>8 [\stemDown <g b f'>8] <c' e'>4 |
+\stemDown f8 [\stemDown a8] \stemDown d'8 [\stemDown f'8]
+r8 <f b>8 \stemUp <f b>8 [\stemUp <f b>8]
+<bes d' g'>4 <bes d' f'>4
+\stemDown a8 [\stemDown <c' f'>8] \stemDown f8 [\stemDown <c' f'>8]
+\stemUp <a, c>8 [\stemUp e,8] a,,4
+r8 <g c'>8 \stemUp <g c'>8 [\stemUp <g c'>8]
+r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]
+<g bes c'>4 <f a c'>4
+r8 f'8 r8 f'8
+r8 <bes e'>8 r8 <a c'>8
+\stemDown <g b>8 [\stemDown g8] g,4
+r8 <a d'>8 \stemUp <a d'>8 [\stemUp <a d'>8]
+\stemDown f8 [\stemDown <a d'>8] \stemDown <g c' e'>8 [\stemDown <g b f'>8]
+\stemDown e8 [\stemDown <c' e'>8] \stemDown e8 [\stemDown <b d'>8]
+r8 <c' e'>8 r8 <c' e'>8
+r8 <c' d'>8 \stemUp <c' d'>8 [\stemUp <c' d'>8]
+\stemDown a8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
+\stemDown c8 [\stemDown c'8] \stemDown <b c'>8 [\stemDown <bes c'>8]
+\stemDown fis8 [\stemDown <a d'>8] \stemDown fis8 [\stemDown <c' d'>8]
+r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+\stemDown d8 [\stemDown <d' f'>8] \stemDown <d' f'>8 [\stemDown <d' f'>8]
+r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+\stemDown e8 [\stemDown <gis d'>8] \stemDown gis8 [\stemDown <d' e'>8]
+r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+\stemDown bes,8 [\stemDown <bes d'>8] \stemDown <bes d'>8 [\stemDown <bes d'>8]
+\stemDown <a c'>8 [\stemDown <fis a d'>8] \stemDown <g b f'>8 [\stemDown <a c' e'>8]
+r8 c'8 \stemUp c'8 [\stemUp c'8]
+\stemDown a,8 [\stemDown <a c'>8] \stemDown <a c'>8 [\stemDown <a c'>8]
+r8 c'8 \stemUp c'8 [\stemUp c'8]
+\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
+\stemDown <g d' f'>8 [\stemDown <g d' f'>8] <c' e'>4
+r8 <c' d'>8 r8 <c' d'>8
+<e gis b>4 \stemDown e'8 [\stemDown e8]
+\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
+\stemDown <g c'>8 [\stemDown <g b>8] <c c'>4
+\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' g'>8]
+r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]
+r8 c'8 c'4
+\stemDown <c' e'>8. [\stemDown b16] \stemDown a8 [\stemDown <c' e'>8]
+r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+e4 \stemDown f8 [\stemDown f8]
+\stemDown <c' e'>8 [\stemDown g8] c4
+r8 <a b d'>8 \stemUp <e c'>8 [\stemUp <e b d'>8]
+r8 <a d'>8 \stemUp <e a e'>8 [\stemUp <e gis d'>8]
+r8 <fis c'>8 \stemUp <fis c'>8 [\stemUp <fis c'>8]
+<e b d'>4 <e a c'>4
+r8 <b f'>8 \stemUp <b f'>8 [\stemUp <b f'>8]
+r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]
+\stemUp a8. [\stemUp g16] f4
+\stemUp g,8 [\stemUp g8] \stemDown <d' f'>8 [\stemDown b8]
+\stemDown gis8 [\stemDown <b e'>8] \stemDown a8 [\stemDown <c' e'>8]
+r8 <gis d'>8 \stemUp <gis d'>8 [\stemUp <gis d'>8]
+\stemDown a,8 [\stemDown <c' e'>8] \stemDown a8 [\stemDown <c' e'>8]
+\stemDown d8 [\stemDown <a b>8] \stemDown e8 [\stemDown <b d'>8]
+\stemDown c8 [\stemDown <g e'>8] \stemDown <g e'>8 [\stemDown <bes e'>8]
+r8 e'8 d'8 r8
+\stemDown g8 [\stemDown <b f'>8] \stemDown g8 [\stemDown <b f'>8]
+r8 <b e'>8 \stemUp <b e'>8 [\stemUp <b e'>8]
+r8 <a e'>8 \stemUp <a e'>8 [\stemUp <a e'>8]
+\stemDown <a c'>8 [\stemDown e8] a,4
+<d' f'>4 \stemDown <c' d'>8 [\stemDown <b d'>8]
+\stemDown d8 [\stemDown f'8] d'4
+r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]
+\stemDown <a c'>8 [\stemDown e8] a,4
+r8 <c' f'>8 r8 <d' f'>8
+r8 <bes e'>8 \stemUp <bes e'>8 [\stemUp <bes e'>8]
+r8 <a d'>8 r8 <d' f'>8
+<f c' d'>4 \stemDown <g b d'>8 [\stemDown <g d' f'>8]
+r8 <a f'>8 \stemUp <a f'>8 [\stemUp <a f'>8]
+r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b f'>8]
+r8 <cis' g'>8 \stemUp <cis' g'>8 [\stemUp <e' g'>8]
+r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]
+r8 <gis d'>8 \stemUp <b e'>8 [\stemUp <b e'>8]
+a4 \stemUp c'8 [\stemUp e'8]
+r8 <b d'>8 \stemUp <b f'>8 [\stemUp <b f'>8]
+\stemDown <e g b>8 [\stemDown <e g c'>8] <e g>4
+bes4 c'4
+r8 <a d'>8 r8 <bes d'>8
+\stemDown <g b d'>8 [\stemDown <fis c' d'>8] <g b f'>4 |
+r8 <c' e'>8 r8 <a c'>8
+r8 <gis d'>8 \stemUp <gis d'>8 [\stemUp <gis d'>8]
+r8 <c' es'>8 r8 <c' es'>8
+\stemUp g,8 [\stemUp g8] \stemDown <d' f'>8 [\stemDown g8]
+r8 <b e'>8 r8 <d' e'>8
+<gis b f'>4 <g b f'>4
+r8 <b e'>8 \stemUp <b e'>8 [\stemUp <b e'>8]
+\stemDown d8 [\stemDown <a f'>8] \stemDown e8 [\stemDown <b e'>8]
+\stemDown <a c'>8 [\stemDown <a e'>8] <a c'>4
+r8 <b d'>8 \stemUp <b d'>8 [\stemUp <d' f'>8]
+r8 <c' d'>8 r8 <b d'>8
+r8 <c' f'>8 r8 <c' f'>8
+r8 <a b>8 r8 <b d'>8
+\stemDown <a c'>8 [\stemDown <e gis d'>8] <a c'>4
+\stemDown e8 [\stemDown <c' e'>8] \stemDown <e b d'>8 [\stemDown <e b d'>8]
+\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
+r8 <g c'>8 r8 <a c'>8
+\stemDown <a c'>8 [\stemDown e8] a,4
+\clef "treble" \stemUp <bes d' g'>8 [\stemUp <b d' gis'>8] \stemUp <c' f' a'>8 [\stemUp <c' g' bes'>8]
+\clef "bass" \stemDown e8 [\stemDown <c' e'>8] \stemDown f8 [\stemDown <a f'>8]
+r8 <c' e'>8 r8 <d' e'>8
+r8 <b d'>8 r8 <gis d' e'>8
+\stemDown a8 [\stemDown <c' e'>8] \stemDown f8 [\stemDown <c' d'>8]
+\stemDown <c e g>8 [\stemDown c'8] \stemDown c'8 [\stemDown c8]
+\stemDown d8 [\stemDown <d' f'>8] \stemDown <d' f'>8 [\stemDown <d' f'>8]
+\stemDown <a, a>8 [\stemDown <c' e'>8] \stemDown a8 [\stemDown <c' e'>8]
+r8 <cis' g'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]
+r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+r8 <b f'>8 \stemUp <d' f'>8 [\stemUp <d' f'>8]
+<g b f'>4 \stemDown <g c' e'>8 [\stemDown <g bes c'>8] |
+\stemDown f8 [\stemDown <a f'>8] \stemDown a8 [\stemDown <c' f'>8]
+\stemDown <c' e'>8 [\stemDown g'8] <c' e'>4
+r8 <gis e'>8 r8 <c' e'>8
+\stemUp g8 [\stemUp f8] e4
+r8 <c' e'>8 r8 <c' f'>8
+r8 <c' e'>8 r8 <c' e'>8
+\stemDown a'8 [\stemDown f'8] f4
+\clef "treble" r8 <d' g'>8 r8 <g' bes'>8
+<a a'>4 a4
+\clef "bass" r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+r8 <c' f'>8 r8 <c' f'>8
+r8 <a f'>8 \stemUp <a f'>8 [\stemUp <a f'>8]
+\stemUp <c' e'>8 [\stemUp d'8] c'4
+r8 <c' e'>8 r8 <c' e'>8
+\stemUp e'8 [\stemUp d'8] c'4
+<g c' e'>4 <a c' f'>4
+\stemDown d8 [\stemDown <d' f'>8] \stemDown <d' f'>8 [\stemDown <d' f'>8]
+r8 <c' e'>8 r8 <c' e'>8
+\stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
+\clef "treble" r8 <d' f' g'>8 \stemUp <d' f' g'>8 [\stemUp <d' f' g'>8]
+\clef "bass" \stemDown <a c'>8 [\stemDown <a e'>8] <a c'>4
+\stemDown d8 [\stemDown <a f'>8] \stemDown <a f'>8 [\stemDown <a f'>8]
+\stemUp <f, a,>8 [\stemUp c,8] a,,4"""
+
+piano_left_hand_voice_2 = r"""g2
+s2
+s2
+s2
+gis2
+a2
+s2
+s2
+g2
+s2
+s2
+s2
+s2
+g2
+c2
+b2
+s2
+d4 s4
+s2
+d2
+g4 g4
+s2
+s2
+s2
+c2
+s2
+a2
+s2
+f4 d4
+s2
+s2
+s2
+s2
+s2
+a2
+s2
+s2
+f2
+s2
+c2
+e2
+a4 s4
+f2
+d4 g4
+g2
+s2
+s2
+s2
+g2
+s2
+s2
+s2
+s2
+f4 \stemDown e8 [\stemDown e8]
+g2
+a2
+s2
+s2
+s2
+s2
+d2
+s2
+s2
+s2
+c2
+g2
+s2
+c'4 d'4
+c4 f4
+s2
+fis2
+s2
+s2
+a4 a4
+fis2
+s2
+s2
+s2
+a2
+s2
+g2
+s2
+a2
+a2
+s2
+s2
+c2
+s2
+c2
+s2
+s2
+a4 fis4
+s2
+s2
+s2
+s2
+a2
+c2
+s2
+c2
+s2
+s2
+f4 s4
+f4 s4
+d2
+s2
+g2
+f2
+c'2
+s2
+s2
+e2
+s2
+s2
+s2
+a4 r8 d8
+s2
+gis2
+e2
+s2
+s2
+s2
+f2
+s2
+a4 bes4
+g2
+f4 g4
+s2
+f2
+g2
+a2
+f2
+e2
+a,4 \stemDown c8 [\stemDown e8]
+g2
+s2
+s2
+fis4 g4
+s2
+g4 f4
+e2
+fis4 f4
+s2
+gis4 gis4
+s2
+gis2
+s2
+s2
+g2
+fis4 g4
+a4 f4
+d4 e4
+s2
+s2
+s2
+e4 f4
+s2
+s2
+s2
+a4 gis4
+f4 e4
+s2
+s2
+s2
+s2
+a2
+a2
+g2
+s2
+s2
+s2
+e4 a4
+c2
+g4 f4
+g4 a4
+s2
+bes4 c'4
+s2
+g2
+f4 a4
+f2
+a2
+bes4 g4
+a2
+s2
+s2
+bes4 g4
+s2
+b2
+s2
+s2
+s2"""
+
+rh_v_1 = piano_right_hand_voice_1.split('\n')
+rh_v_2 = piano_right_hand_voice_2.split('\n')
+
+lh_v_1 = piano_left_hand_voice_1.split('\n')
+lh_v_2 = piano_left_hand_voice_2.split('\n')
+
+voice_format = r'{{<<{{\voiceOne {voice_1}}} \new Voice {{\voiceTwo {voice_2}}}>>}}'
+
+
+piano_right_hand = []
+for rhv1, rhv2 in zip(rh_v_1, rh_v_2):
+    if rhv2.startswith('s2'):
+        piano_right_hand.append(rhv1.strip())
+    else:
+        piano_right_hand.append(voice_format.format(voice_1=rhv1.strip(), voice_2=rhv2.strip()))
+
+
+piano_left_hand = []
+for lhv1, lhv2 in zip(lh_v_1, lh_v_2):
+    if lhv2.startswith('s2'):
+        piano_left_hand.append(lhv1.strip())
+    else:
+        piano_left_hand.append(voice_format.format(voice_1=lhv1.strip(), voice_2=lhv2.strip()))
+
+
+sync_bars = {}
+for ind, (piano_right_hand, piano_left_hand) in enumerate(zip(piano_right_hand, piano_left_hand)):
+    sync_bars[ind + 1] = {'piano_right_hand': SimpleBar(piano_right_hand),
+                          'piano_left_hand': SimpleBar(piano_left_hand)}
+
+a = SimpleBarCollection(sync_bars)
+
+writer = SimpleBarCollectionCSVWriter()
+writer.write_csv(a, Path('/tmp/scottish_dance_bars.csv'))
+
+print()
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##t
     \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
         paper-height = 1400\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
@@ -20,33 +20,33 @@
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\major
-                \time 3/4
             }
             {
                 \clef treble
+                \time 3/4
                 \BLOCK{ for bar in bar_collections['menuet'].get_bars('piano_right_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\major
-                \time 3/4
             }
             {
                 \clef bass
+                \time 3/4
                 \BLOCK{ for bar in bar_collections['menuet'].get_bars('piano_left_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
@@ -62,33 +62,33 @@
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\minor
-                \time 3/4
             }
             {
                 \clef treble
+                \time 3/4
                 \BLOCK{ for bar in bar_collections['trio'].get_bars('piano_right_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\minor
-                \time 3/4
             }
             {
                 \clef bass
+                \time 3/4
                 \BLOCK{ for bar in bar_collections['trio'].get_bars('piano_left_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \include "articulate.ly"
 
 % menuet with repeats
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
-	page-count = 1
-    print-all-headers = ##t
+	print-all-headers = ##t
     score-markup-spacing = #'((basic-distance . 10))
     markup-system-spacing = #'((minimum-distance = 0))
+
+    \BLOCK{ if render_settings['single_page'] }
+        paper-height = 360\mm  %% default is 297 for a4
+    \BLOCK{ endif }
 }
 \header{
     title = "Menuet and Trio"
-    composer = "Kirnberger"
+    composer = "Stadler"
     tagline = ##f
 }
 \score {
     \header {
         piece = \markup { \fontsize #1 "Menuet" }
         title = ""
         composer = ""
     }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \key d\major
-                \time 3/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
+                \time 3/4
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
                         \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
@@ -40,20 +43,20 @@
                 }
             }
         >>
         \new Staff
         <<
             {
                 \key d\major
-                \time 3/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
+                \time 3/4
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
 		                \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
@@ -76,21 +79,21 @@
         composer = ""
     }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
-                \key d\minor
-                \time 3/4
+                \key g\major
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
+                \time 3/4
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
                         \VAR{composition_bars['trio'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
@@ -98,21 +101,21 @@
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
         <<
             {
-                \key d\minor
-                \time 3/4
+                \key g\major
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
+                \time 3/4
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
 		                \VAR{composition_bars['trio'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##f
     paper-height = 50\mm
     paper-width = 100\mm
 }
 \header{
     title = ""
@@ -12,39 +12,37 @@
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \BLOCK{ if table_name == 'menuet' }
                     \key d\major
-                    \time 3/4
                 \BLOCK{ else }
                     \key d\minor
-                    \time 3/4
                 \BLOCK{ endif }
             }
             {
                 \clef treble
+                \time 3/4
                 \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
                 \BLOCK{ if table_name == 'menuet' }
                     \key d\major
-                    \time 3/4
                 \BLOCK{ else }
                     \key d\minor
-                    \time 3/4
                 \BLOCK{ endif }
             }
             {
                 \clef bass
+                \time 3/4
                 \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
                 \bar "|."
             }
         >>
     >>
     \layout {
         indent = 0\mm
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly` & `musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##f
     paper-height = 50\mm
     paper-width = 100\mm
 }
 \header{
     title = ""
@@ -12,41 +12,39 @@
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \BLOCK{ if table_name == 'menuet' }
                     \key d\major
-                    \time 3/4
                 \BLOCK{ else }
-                    \key d\minor
-                    \time 3/4
+                    \key g\major
                 \BLOCK{ endif }
             }
             {
                 \clef treble
+                \time 3/4
                 \BLOCK{ for synchronous_bar in synchronous_bars }
                 \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
                 \BLOCK{ if table_name == 'menuet' }
                     \key d\major
-                    \time 3/4
                 \BLOCK{ else }
-                    \key d\minor
-                    \time 3/4
+                    \key g\major
                 \BLOCK{ endif }
             }
             {
                 \clef bass
+                \time 3/4
                 \BLOCK{ for synchronous_bar in synchronous_bars }
                 \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
     >>
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##t
 
     \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
         paper-height = 3400\mm  %% default is 297 for a4
     \BLOCK{ endif }
@@ -20,72 +20,72 @@
     }
     <<
         \new Staff
         <<
             \set Staff.instrumentName = #"Violin #1 "
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
-                \key d\major
-                \time 3/4
                 \override Score.RehearsalMark.direction = #down
+                \key d\major
             }
             {
                 \clef treble
+                \time 3/4
                 \BLOCK{ for bar in bar_collections['polonaise'].get_bars('violin_1').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             \set Staff.instrumentName = #"Violin #2 "
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
-                \key d\major
-                \time 3/4
                 \override Score.RehearsalMark.direction = #down
+                \key d\major
             }
             {
                 \clef treble
+                \time 3/4
                 \BLOCK{ for bar in bar_collections['polonaise'].get_bars('violin_2').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new PianoStaff
         <<
             \set PianoStaff.instrumentName = #"Piano"
             \new Staff
             <<
                 {
                     \override Score.BarNumber.break-visibility = ##(#t #t #t)
-                    \key d\major
-                    \time 3/4
                     \override Score.RehearsalMark.direction = #down
+                    \key d\major
                 }
                 {
                     \clef treble
+                    \time 3/4
                     \BLOCK{ for bar in bar_collections['polonaise'].get_bars('piano_right_hand').values() }
                         \VAR{bar.lilypond_str}
                     \BLOCK{ endfor }
                     \bar "|"
                 }
             >>
             \new Staff
             <<
                 {
                     \override Score.BarNumber.break-visibility = ##(#t #t #t)
-                    \key d\major
-                    \time 3/4
                     \override Score.RehearsalMark.direction = #down
+                    \key d\major
                 }
                 {
                     \clef bass
+                    \time 3/4
                     \BLOCK{ for bar in bar_collections['polonaise'].get_bars('piano_left_hand').values() }
                         \VAR{bar.lilypond_str}
                     \BLOCK{ endfor }
                     \bar "|"
                 }
             >>
         >>
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \include "articulate.ly"
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##t
     score-markup-spacing = #'((basic-distance . 10))
     markup-system-spacing = #'((minimum-distance = 0))
     system-system-spacing = #'((basic-distance . 15))
 
     \BLOCK{ if render_settings['single_page'] }
@@ -22,72 +22,72 @@
     }
     <<
         \new Staff
         <<
             \set Staff.instrumentName = #"Violin #1 "
             {
                 \key d\major
-                \time 3/4
                 \tempo 4 = 70
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
+                \time 3/4
                 \BLOCK{ for bar_index in range(14) }
                     \VAR{composition_bars['polonaise'][bar_index].get_bar('violin_1').lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             \set Staff.instrumentName = #"Violin #2 "
             {
                 \key d\major
-                \time 3/4
                 \tempo 4 = 70
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
+                \time 3/4
                 \BLOCK{ for bar_index in range(14) }
                     \VAR{composition_bars['polonaise'][bar_index].get_bar('violin_2').lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new PianoStaff
         <<
             \set PianoStaff.instrumentName = #"Piano"
             \new Staff
             <<
                 {
                     \key d\major
-                    \time 3/4
                     \tempo 4 = 70
                     \override Score.RehearsalMark.direction = #down
                 }
                 {
                     \clef treble
+                    \time 3/4
                     \BLOCK{ for bar_index in range(14) }
                         \VAR{composition_bars['polonaise'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                     \bar "|."
                 }
             >>
             \new Staff
             <<
                 {
                     \key d\major
-                    \time 3/4
                     \tempo 4 = 70
                     \override Score.RehearsalMark.direction = #down
                 }
                 {
                     \clef bass
+                    \time 3/4
                     \BLOCK{ for bar_index in range(14) }
                         \VAR{composition_bars['polonaise'][bar_index].get_bar('piano_left_hand').lilypond_str}
                         \BLOCK{ if bar_index == 1}
                             \mark \markup { \musicglyph #"scripts.segno" }
                         \BLOCK{ elif bar_index == 5 }
                             \bar "||"
                             \once \override Score.RehearsalMark #'self-alignment-X = #right \mark \markup {\fontsize #-1 \italic "Fine"}
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##f
     paper-height = 100\mm
     paper-width = 150\mm
 }
 \header{
     title = ""
@@ -12,58 +12,58 @@
     \new PianoStaff
     <<
         \new Staff
         <<
             \set Staff.instrumentName = #"Violin #1 "
             {
                 \key d\major
-                \time 3/4
             }
             {
                 \clef treble
+                \time 3/4
                 \VAR{ synchronous_bar.get_bar('violin_1').lilypond_str }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             \set Staff.instrumentName = #"Violin #2 "
             {
                 \key d\major
-                \time 3/4
             }
             {
                 \clef treble
+                \time 3/4
                 \VAR{ synchronous_bar.get_bar('violin_2').lilypond_str }
                 \bar "|."
             }
         >>
         \new PianoStaff
         <<
             \set PianoStaff.instrumentName = #"Piano"
             \new Staff
             <<
                 {
                     \key d\major
-                    \time 3/4
                 }
                 {
                     \clef treble
+                    \time 3/4
                     \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
                     \bar "|."
                 }
             >>
             \new Staff
             <<
                 {
                     \key d\major
-                    \time 3/4
                 }
                 {
                     \clef bass
+                    \time 3/4
                     \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
                     \bar "|."
                 }
             >>
         >>
     >>
 }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly` & `musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,54 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##f
-    paper-height = 100\mm
-    paper-width = 150\mm
+    paper-height = 50\mm
+    paper-width = 100\mm
 }
 \header{
     title = ""
     tagline = ##f
 }
 \score {
+    \header {
+        piece = \markup { \fontsize #1 "" }
+        title = ""
+    }
     \new PianoStaff
     <<
         \new Staff
         <<
-            \set Staff.instrumentName = #"Violin #1 "
             {
-                \key d\major
-                \time 3/4
+                \key c\major
             }
             {
                 \clef treble
+                \time 3/8
                 \BLOCK{ for synchronous_bar in synchronous_bars }
-                \VAR{ synchronous_bar.get_bar('violin_1').lilypond_str }
+                \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
         <<
-            \set Staff.instrumentName = #"Violin #2 "
             {
-                \key d\major
-                \time 3/4
+                \key c\major
             }
             {
-                \clef treble
+                \clef bass
+                \time 3/8
                 \BLOCK{ for synchronous_bar in synchronous_bars }
-                \VAR{ synchronous_bar.get_bar('violin_2').lilypond_str }
+                    \BLOCK{ if synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str != '' }
+                        <<{\voiceOne \VAR{synchronous_bar.get_bar('piano_left_hand').lilypond_str}} \new Voice {\voiceTwo \VAR{synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str}}>>
+                    \BLOCK{ else }
+                        \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
+                    \BLOCK{ endif }
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
-        \new PianoStaff
-        <<
-            \set PianoStaff.instrumentName = #"Piano"
-            \new Staff
-            <<
-                {
-                    \key d\major
-                    \time 3/4
-                }
-                {
-                    \clef treble
-                    \BLOCK{ for synchronous_bar in synchronous_bars }
-                    \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
-                    \BLOCK{ endfor }
-                    \bar "|."
-                }
-            >>
-            \new Staff
-            <<
-                {
-                    \key d\major
-                    \time 3/4
-                }
-                {
-                    \clef bass
-                    \BLOCK{ for synchronous_bar in synchronous_bars }
-                    \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
-                    \BLOCK{ endfor }
-                    \bar "|."
-                }
-            >>
-        >>
     >>
+    \layout {
+        indent = #0
+    }
 }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv` & `musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly` & `musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##t
 
     \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
         paper-height = 1200\mm  %% default is 297 for a4
     \BLOCK{ endif }
@@ -21,33 +21,33 @@
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
-                \time 2/4
             }
             {
                 \clef treble
+                \time 2/4
                 \BLOCK{ for bar in bar_collections['contredanse'].get_bars('piano_right_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
-                \time 2/4
             }
             {
                 \clef bass
+                \time 2/4
                 \BLOCK{ for bar_ind, bar in bar_collections['contredanse'].get_bars('piano_left_hand').items() }
                     \BLOCK{ if bar_collections['contredanse'].get_bar('piano_left_hand_alternative', bar_ind).lilypond_str != '' }
                         <<{\voiceOne \VAR{bar.lilypond_str}} \new Voice {\voiceTwo \VAR{bar_collections['contredanse'].get_bar('piano_left_hand_alternative', bar_ind).lilypond_str}}>>
                     \BLOCK{ else }
                         \VAR{bar.lilypond_str}
                     \BLOCK{ endif }
                 \BLOCK{ endfor }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly` & `musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \include "articulate.ly"
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly` & `musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##t
     score-markup-spacing = #'((basic-distance . 10))
     markup-system-spacing = #'((minimum-distance = 0))
     system-system-spacing = #'((basic-distance . 15))
 
     scoreTitleMarkup = \markup {
@@ -52,20 +52,20 @@
     }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \key c\major
-                \time 2/4
                 \tempo 4 = 70
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
+                \time 2/4
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(7) }
                         \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
 
                 \alternative { {\VAR{composition_bars['contredanse'][7].get_bar('piano_right_hand').lilypond_str}} {\VAR{composition_bars['contredanse'][7].get_bar('piano_right_hand').lilypond_str}} }
@@ -77,20 +77,20 @@
                 }
             }
         >>
         \new Staff
         <<
             {
                 \key c\major
-                \time 2/4
                 \tempo 4 = 70
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
+                \time 2/4
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(7) }
 		                \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 
                 \alternative { {\VAR{composition_bars['contredanse'][7].get_bar('piano_left_hand').lilypond_str}} {\VAR{composition_bars['contredanse'][7].get_bar('piano_left_hand_alternative').lilypond_str}} }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly` & `musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##f
     paper-height = 50\mm
     paper-width = 100\mm
 }
 \header{
     title = ""
@@ -15,30 +15,30 @@
     }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \key c\major
-                \time 2/4
             }
             {
                 \clef treble
+                \time 2/4
                 \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
                 \key c\major
-                \time 2/4
             }
             {
                 \clef bass
+                \time 2/4
                 \BLOCK{ if synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str != '' }
                     <<{\voiceOne \VAR{synchronous_bar.get_bar('piano_left_hand').lilypond_str}} \new Voice {\voiceTwo \VAR{synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str}}>>
                 \BLOCK{ else }
                     \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
                 \BLOCK{ endif }
                 \bar "|."
             }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly` & `musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##f
     paper-height = 50\mm
     paper-width = 100\mm
 }
 \header{
     title = ""
@@ -15,32 +15,32 @@
     }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \key c\major
-                \time 2/4
             }
             {
                 \clef treble
+                \time 2/4
                 \BLOCK{ for synchronous_bar in synchronous_bars }
                 \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
                 \key c\major
-                \time 2/4
             }
             {
                 \clef bass
+                \time 2/4
                 \BLOCK{ for synchronous_bar in synchronous_bars }
                     \BLOCK{ if synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str != '' }
                         <<{\voiceOne \VAR{synchronous_bar.get_bar('piano_left_hand').lilypond_str}} \new Voice {\voiceTwo \VAR{synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str}}>>
                     \BLOCK{ else }
                         \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
                     \BLOCK{ endif }
                 \BLOCK{ endfor }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly` & `musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##t
 
     \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
         paper-height = 1200\mm  %% default is 297 for a4
     \BLOCK{ endif }
@@ -21,33 +21,33 @@
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
-                \time 3/8
             }
             {
                 \clef treble
+                \time 3/8
                 \BLOCK{ for bar in bar_collections['waltz'].get_bars('piano_right_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
-                \time 3/8
             }
             {
                 \clef bass
+                \time 3/8
                 \BLOCK{ for bar_ind, bar in bar_collections['waltz'].get_bars('piano_left_hand').items() }
                     \BLOCK{ if bar_collections['waltz'].get_bar('piano_left_hand_alternative', bar_ind).lilypond_str != '' }
                         <<{\voiceOne \VAR{bar.lilypond_str}} \new Voice {\voiceTwo \VAR{bar_collections['waltz'].get_bar('piano_left_hand_alternative', bar_ind).lilypond_str}}>>
                     \BLOCK{ else }
                         \VAR{bar.lilypond_str}
                     \BLOCK{ endif }
                 \BLOCK{ endfor }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly` & `musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \include "articulate.ly"
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly` & `musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##t
     score-markup-spacing = #'((basic-distance . 10))
     markup-system-spacing = #'((minimum-distance = 0))
     system-system-spacing = #'((basic-distance . 15))
 
     scoreTitleMarkup = \markup {
@@ -52,20 +52,20 @@
     }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \key c\major
-                \time 3/8
                 \tempo 8 = 110
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
+                \time 3/8
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(7) }
                         \VAR{composition_bars['waltz'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
 
                 \alternative { {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}} {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}} }
@@ -77,20 +77,20 @@
                 }
             }
         >>
         \new Staff
         <<
             {
                 \key c\major
-                \time 3/8
                 \tempo 8 = 110
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
+                \time 3/8
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(7) }
 		                \VAR{composition_bars['waltz'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 
                 \alternative { {\VAR{composition_bars['waltz'][7].get_bar('piano_left_hand').lilypond_str}} {\VAR{composition_bars['waltz'][7].get_bar('piano_left_hand_alternative').lilypond_str}} }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly` & `musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##f
     paper-height = 50\mm
     paper-width = 100\mm
 }
 \header{
     title = ""
@@ -15,30 +15,30 @@
     }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \key c\major
-                \time 3/8
             }
             {
                 \clef treble
+                \time 3/8
                 \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
                 \key c\major
-                \time 3/8
             }
             {
                 \clef bass
+                \time 3/8
                 \BLOCK{ if synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str != '' }
                     <<{\voiceOne \VAR{synchronous_bar.get_bar('piano_left_hand').lilypond_str}} \new Voice {\voiceTwo \VAR{synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str}}>>
                 \BLOCK{ else }
                     \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
                 \BLOCK{ endif }
                 \bar "|."
             }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv` & `musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##t
     \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
         paper-height = 2800\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
@@ -20,33 +20,33 @@
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\major
-                \time 3/4
             }
             {
                 \clef treble
+                \time 3/4
                 \BLOCK{ for bar in bar_collections['menuet'].get_bars('piano_right_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\major
-                \time 3/4
             }
             {
                 \clef bass
+                \time 3/4
                 \BLOCK{ for bar in bar_collections['menuet'].get_bars('piano_left_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
@@ -63,33 +63,33 @@
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key g\major
-                \time 3/4
             }
             {
                 \clef treble
+                \time 3/4
                 \BLOCK{ for bar in bar_collections['trio'].get_bars('piano_right_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key g\major
-                \time 3/4
             }
             {
                 \clef bass
+                \time 3/4
                 \BLOCK{ for bar in bar_collections['trio'].get_bars('piano_left_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\version "2.19.81"
+\version "2.22.1"
 \include "articulate.ly"
 
 % menuet with repeats
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly` & `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,77 @@
-\version "2.19.81"
+\version "2.22.1"
 \paper {
     print-all-headers = ##f
-    paper-height = 50\mm
-    paper-width = 100\mm
+    paper-height = 100\mm
+    paper-width = 150\mm
 }
 \header{
     title = ""
     tagline = ##f
 }
 \score {
     \new PianoStaff
     <<
         \new Staff
         <<
+            \set Staff.instrumentName = #"Violin #1 "
             {
-                \BLOCK{ if table_name == 'menuet' }
-                    \key d\major
-                    \time 3/4
-                \BLOCK{ else }
-                    \key g\major
-                    \time 3/4
-                \BLOCK{ endif }
+                \key d\major
             }
             {
                 \clef treble
+                \time 3/4
                 \BLOCK{ for synchronous_bar in synchronous_bars }
-                \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
+                \VAR{ synchronous_bar.get_bar('violin_1').lilypond_str }
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
         <<
+            \set Staff.instrumentName = #"Violin #2 "
             {
-                \BLOCK{ if table_name == 'menuet' }
-                    \key d\major
-                    \time 3/4
-                \BLOCK{ else }
-                    \key g\major
-                    \time 3/4
-                \BLOCK{ endif }
+                \key d\major
             }
             {
-                \clef bass
+                \clef treble
+                \time 3/4
                 \BLOCK{ for synchronous_bar in synchronous_bars }
-                \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
+                \VAR{ synchronous_bar.get_bar('violin_2').lilypond_str }
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
+        \new PianoStaff
+        <<
+            \set PianoStaff.instrumentName = #"Piano"
+            \new Staff
+            <<
+                {
+                    \key d\major
+                }
+                {
+                    \clef treble
+                    \time 3/4
+                    \BLOCK{ for synchronous_bar in synchronous_bars }
+                    \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
+                    \BLOCK{ endfor }
+                    \bar "|."
+                }
+            >>
+            \new Staff
+            <<
+                {
+                    \key d\major
+                }
+                {
+                    \clef bass
+                    \time 3/4
+                    \BLOCK{ for synchronous_bar in synchronous_bars }
+                    \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
+                    \BLOCK{ endfor }
+                    \bar "|."
+                }
+            >>
+        >>
     >>
-    \layout {
-        indent = 0\mm
-    }
 }
```

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv` & `musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv` & `musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/dice_games/base.py` & `musical_games-0.8.1/musical_games/dice_games/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,16 @@
         self._author = author
         self._title = title
         self._dice_tables = dice_tables
         self._bar_collections = bar_collections
         self._jinja2_environment = jinja2_environment
         self._default_midi_settings = default_midi_settings
 
+    @classmethod
+
     @property
     def author(self) -> str:
         return self._author
 
     @property
     def title(self) -> str:
         return self._title
@@ -341,14 +343,35 @@
                                   midi_settings: MidiSettings | None = None) -> LilypondScore:
         midi_settings = midi_settings or self.get_default_midi_settings()
         template = self._jinja2_environment.get_template('composition_midi.ly')
         composition_bars = self.bar_selection_to_bars(bar_selection)
         return SimpleLilypondScore(template.render(composition_bars=composition_bars, midi_settings=midi_settings))
 
     @staticmethod
+    def _generate_jinja2_environment(data_name: str) -> jinja2.Environment:
+        """Generate a standard jinja2 environment for a musical game.
+
+        This assumes the lilypond templates for the dice game are kept in the package in the data directory:
+        ``data/dice_games/<data_name>/lilypond``. In addition, it will add the lilypond utility directory to the
+        loader.
+
+        Args:
+            data_name: the data name of this dice games' data
+
+        Returns:
+            A jinj2 environment to provide to the dice game.
+        """
+        template_loader = jinja2.ChoiceLoader([
+            jinja2.PackageLoader('musical_games', f'data/dice_games/{data_name}/lilypond'),
+            jinja2.PackageLoader('musical_games', 'data/lilypond_utils'),
+        ])
+        env_options = SimpleDiceGame._standard_jinja2_environment_options() | {'loader': template_loader}
+        return jinja2.Environment(**env_options)
+
+    @staticmethod
     def _standard_jinja2_environment_options():
         """Get a set of standard jinja2 environment options you can use in your templates."""
         return dict(
             block_start_string=r'\BLOCK{',
             block_end_string='}',
             variable_start_string=r'\VAR{',
             variable_end_string='}',
```

### Comparing `musical_games-0.8.0/musical_games/dice_games/data_csv.py` & `musical_games-0.8.1/musical_games/dice_games/data_csv.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/dice_games/dice_games.py` & `musical_games-0.8.1/musical_games/dice_games/dice_games.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,32 +38,29 @@
                 [4, 13, 22, 31, 40, 49],
                 [5, 14, 23, 32, 41, 50],
                 [6, 15, 24, 33, 42, 51],
                 [7, 16, 25, 34, 43, 52],
                 [8, 17, 26, 35, 44, 53],
                 [9, 18, 27, 36, 45, 54]]),
         }
+        data_name = 'cpe_bach_counterpoint'
 
         csv_reader = SimpleBarCollectionCSVReader()
         treble_bars = csv_reader.read_csv(resources.files('musical_games')
-                                          / 'data/dice_games/cpe_bach_counterpoint/bars_treble.csv')
+                                          / f'data/dice_games/{data_name}/bars_treble.csv')
         bass_bars = csv_reader.read_csv(resources.files('musical_games')
-                                        / 'data/dice_games/cpe_bach_counterpoint/bars_bass.csv')
-
-        template_loader = jinja2.PackageLoader('musical_games', f'data/dice_games/cpe_bach_counterpoint/lilypond')
-        env_options = self._standard_jinja2_environment_options() | {'loader': template_loader}
-        jinja2_environment = jinja2.Environment(**env_options)
+                                        / f'data/dice_games/{data_name}/bars_bass.csv')
 
         midi_settings = SimpleMidiSettings(
             {'treble': {'piano_right_hand': 'acoustic grand'}, 'bass': {'piano_left_hand': 'acoustic grand'}},
             {'treble': {'piano_right_hand': 0}, 'bass': {'piano_left_hand': 0}},
             {'treble': {'piano_right_hand': 1}, 'bass': {'piano_left_hand': 0.75}})
 
         super().__init__('C.P.E. Bach', 'Counterpoint', dice_tables, {'treble': treble_bars, 'bass': bass_bars},
-                         jinja2_environment, midi_settings)
+                         self._generate_jinja2_environment(data_name), midi_settings)
 
 
 class KirnbergerMenuetTrio(SimpleDiceGame):
 
     def __init__(self):
         """Implementation of a Menuet and Trio dice game by Kirnberger.
 
@@ -81,35 +78,32 @@
                 [81, 57, 67, 2, 90, 41, 24, 56, 94, 47, 62, 72, 25, 64, 48, 87],
                 [78, 45, 30, 65, 14, 33, 10, 73, 40, 55, 46, 17, 31, 85, 11, 76],
                 [8, 69, 26, 53, 43, 95, 88, 63, 79, 5, 3, 60, 54, 21, 42, 82],
                 [84, 6, 4, 22, 51, 12, 83, 92, 58, 93, 66, 23, 15, 13, 27, 32],
                 [39, 28, 18, 35, 89, 75, 61, 96, 7, 91, 70, 1, 74, 44, 52, 50],
                 [59, 71, 37, 16, 86, 49, 77, 20, 38, 68, 19, 29, 80, 36, 34, 9]]),
         }
+        data_name = 'kirnberger_menuet_trio'
 
         csv_reader = SimpleBarCollectionCSVReader()
         bar_collections = {'menuet': csv_reader.read_csv(resources.files('musical_games') /
-                                                         'data/dice_games/kirnberger_menuet_trio/menuet_bars.csv'),
+                                                         f'data/dice_games/{data_name}/menuet_bars.csv'),
                            'trio': csv_reader.read_csv(resources.files('musical_games') /
-                                                       'data/dice_games/kirnberger_menuet_trio/trio_bars.csv')}
-
-        template_loader = jinja2.PackageLoader('musical_games', f'data/dice_games/kirnberger_menuet_trio/lilypond')
-        env_options = self._standard_jinja2_environment_options() | {'loader': template_loader}
-        jinja2_environment = jinja2.Environment(**env_options)
+                                                       f'data/dice_games/{data_name}/trio_bars.csv')}
 
         midi_settings = SimpleMidiSettings(
             {'menuet': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'},
              'trio': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
             {'menuet': {'piano_right_hand': 0, 'piano_left_hand': 0},
              'trio': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'menuet': {'piano_right_hand': 1, 'piano_left_hand': 0.75},
              'trio': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
 
         super().__init__('Kirnberger', 'Menuet and Trio', dice_tables, bar_collections,
-                         jinja2_environment, midi_settings)
+                         self._generate_jinja2_environment(data_name), midi_settings)
 
 
 class KirnbergerPolonaise(SimpleDiceGame):
 
     def __init__(self):
         """Implementation of a Polonaise dice game by Kirnberger.
 
@@ -125,33 +119,30 @@
                 [72, 30, 4, 28, 22, 64, 69, 63, 7, 47, 19, 31, 81, 55],
                 [114, 112, 126, 87, 89, 88, 90, 93, 86, 94, 96, 85, 95, 104],
                 [123, 116, 137, 110, 91, 98, 129, 99, 107, 122, 105, 93, 106, 121],
                 [131, 147, 143, 113, 101, 115, 103, 140, 111, 145, 133, 109, 117, 125],
                 [138, 151, 118, 124, 141, 127, 142, 149, 97, 134, 120, 100, 119, 132],
                 [144, 153, 146, 128, 150, 154, 152, 102, 135, 148, 136, 108, 130, 139]])
         }
+        data_name = 'kirnberger_polonaise'
 
         csv_reader = SimpleBarCollectionCSVReader()
         bar_collections = {'polonaise': csv_reader.read_csv(resources.files('musical_games') /
-                                                            'data/dice_games/kirnberger_polonaise/polonaise_bars.csv')}
-
-        template_loader = jinja2.PackageLoader('musical_games', f'data/dice_games/kirnberger_polonaise/lilypond')
-        env_options = self._standard_jinja2_environment_options() | {'loader': template_loader}
-        jinja2_environment = jinja2.Environment(**env_options)
+                                                            f'data/dice_games/{data_name}/polonaise_bars.csv')}
 
         midi_settings = SimpleMidiSettings(
             {'polonaise': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand',
                            'violin_1': 'Violin', 'violin_2': 'Violin'}},
             {'polonaise': {'piano_right_hand': 0, 'piano_left_hand': 0,
                            'violin_1': 0, 'violin_2': 0}},
             {'polonaise': {'piano_right_hand': 0.75, 'piano_left_hand': 0.6,
                            'violin_1': 0.8625, 'violin_2': 0.8625}})
 
         super().__init__('Kirnberger', 'Polonaise', dice_tables, bar_collections,
-                         jinja2_environment, midi_settings)
+                         self._generate_jinja2_environment(data_name), midi_settings)
 
 
 class MozartContredanse(SimpleDiceGame):
 
     def __init__(self):
         """Implementation of a Contredanse dice game by Mozart."""
         dice_tables = {
@@ -164,30 +155,28 @@
                 [165, 152, 112, 15, 147, 27, 73, 102, 144, 104, 87, 107, 128, 48, 109, 74],
                 [7, 81, 131, 37, 21, 125, 49, 115, 116, 133, 72, 141, 94, 80, 129, 65],
                 [142, 106, 40, 69, 43, 140, 23, 89, 66, 124, 26, 84, 75, 103, 96, 127],
                 [99, 68, 86, 139, 120, 92, 143, 83, 93, 55, 29, 51, 42, 110, 108, 98],
                 [85, 45, 90, 158, 82, 123, 78, 58, 61, 34, 119, 46, 59, 54, 60, 47],
                 [145, 97, 6, 121, 56, 67, 63, 16, 50, 79, 175, 76, 113, 88, 53, 118]])
         }
+        data_name = 'mozart_contredanse'
 
         csv_reader = SimpleBarCollectionCSVReader()
         bar_collections = {'contredanse': csv_reader.read_csv(resources.files('musical_games') /
-                                                        'data/dice_games/mozart_contredanse/contredanse_bars.csv')}
-
-        template_loader = jinja2.PackageLoader('musical_games', f'data/dice_games/mozart_contredanse/lilypond')
-        env_options = self._standard_jinja2_environment_options() | {'loader': template_loader}
-        jinja2_environment = jinja2.Environment(**env_options)
+                                                        f'data/dice_games/{data_name}/contredanse_bars.csv')}
 
         midi_settings = SimpleMidiSettings(
             {'contredanse': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
             {'contredanse': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'contredanse': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
 
         super().__init__('Mozart', 'Contredanse', dice_tables, bar_collections,
-                         jinja2_environment, midi_settings)
+                         self._generate_jinja2_environment(data_name), midi_settings)
+
 
 class MozartWaltz(SimpleDiceGame):
 
     def __init__(self):
         """Implementation of a Waltz dice game by Mozart."""
         dice_tables = {
             'waltz': SimpleDiceTable.from_lists([
@@ -199,30 +188,27 @@
                 [104, 157, 27, 167, 154, 68, 118, 91, 138, 71, 150, 29, 101, 162, 23, 151],
                 [152, 60, 171, 53, 99, 133, 21, 127, 16, 155, 57, 175, 43, 168, 89, 172],
                 [119, 84, 114, 50, 140, 86, 169, 94, 120, 88, 48, 166, 51, 115, 72, 111],
                 [98, 142, 42, 156, 75, 129, 62, 123, 65, 77, 19, 82, 137, 38, 149, 8],
                 [3, 87, 165, 61, 135, 47, 147, 33, 102, 4, 31, 164, 144, 59, 173, 78],
                 [54, 130, 10, 103, 28, 37, 106, 5, 35, 20, 108, 92, 12, 124, 44, 131]])
         }
+        data_name = 'mozart_waltz'
 
         csv_reader = SimpleBarCollectionCSVReader()
         bar_collections = {'waltz': csv_reader.read_csv(resources.files('musical_games') /
-                                                        'data/dice_games/mozart_waltz/waltz_bars.csv')}
-
-        template_loader = jinja2.PackageLoader('musical_games', f'data/dice_games/mozart_waltz/lilypond')
-        env_options = self._standard_jinja2_environment_options() | {'loader': template_loader}
-        jinja2_environment = jinja2.Environment(**env_options)
+                                                        f'data/dice_games/{data_name}/waltz_bars.csv')}
 
         midi_settings = SimpleMidiSettings(
             {'waltz': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
             {'waltz': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'waltz': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
 
         super().__init__('Mozart', 'Waltz', dice_tables, bar_collections,
-                         jinja2_environment, midi_settings)
+                         self._generate_jinja2_environment(data_name), midi_settings)
 
 
 class StadlerMenuetTrio(SimpleDiceGame):
 
     def __init__(self):
         """Implementation of a Menuet and Trio dice game by Stadler.
 
@@ -247,72 +233,66 @@
                 [72, 6, 59, 25, 81, 41, 89, 13, 36, 5, 46, 79, 30, 95, 19, 66],
                 [56, 82, 42, 74, 14, 7, 26, 71, 76, 20, 64, 84, 8, 35, 47, 88],
                 [75, 39, 54, 1, 65, 43, 15, 80, 9, 34, 93, 48, 69, 58, 90, 21],
                 [40, 73, 16, 68, 29, 55, 2, 61, 22, 67, 49, 77, 57, 87, 33, 10],
                 [83, 3, 28, 53, 37, 17, 44, 70, 63, 85, 32, 96, 12, 23, 50, 91],
                 [18, 45, 62, 38, 4, 27, 52, 94, 11, 92, 24, 86, 51, 60, 78, 31]]),
         }
+        data_name = 'stadler_menuet_trio'
 
         csv_reader = SimpleBarCollectionCSVReader()
         bar_collections = {'menuet': csv_reader.read_csv(resources.files('musical_games') /
-                                                         'data/dice_games/stadler_menuet_trio/menuet_bars.csv'),
+                                                         f'data/dice_games/{data_name}/menuet_bars.csv'),
                            'trio': csv_reader.read_csv(resources.files('musical_games') /
-                                                       'data/dice_games/stadler_menuet_trio/trio_bars.csv')}
-
-        template_loader = jinja2.PackageLoader('musical_games', f'data/dice_games/stadler_menuet_trio/lilypond')
-        env_options = self._standard_jinja2_environment_options() | {'loader': template_loader}
-        jinja2_environment = jinja2.Environment(**env_options)
+                                                       f'data/dice_games/{data_name}/trio_bars.csv')}
 
         midi_settings = SimpleMidiSettings(
             {'menuet': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'},
              'trio': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
             {'menuet': {'piano_right_hand': 0, 'piano_left_hand': 0},
              'trio': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'menuet': {'piano_right_hand': 1, 'piano_left_hand': 0.75},
              'trio': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
 
         super().__init__('Stadler', 'Menuet and Trio', dice_tables, bar_collections,
-                         jinja2_environment, midi_settings)
+                         self._generate_jinja2_environment(data_name), midi_settings)
 
 
 class GerlachScottishDance(SimpleDiceGame):
 
     def __init__(self):
         """Implementation of a Scottish dance dice game by Gerlach."""
         dice_tables = {
             'dance': SimpleDiceTable.from_lists([
                 [(65, 14), (29, 17), (108, 96), (37, 50), (41, 35), (92, 139), (49, 90), (11, 59)],
                 [(77, 109), (9, 28), (48, 99), (21, 7), (6, 80), (1, 47), (107, 31), (127, 51)],
                 [(15, 87), (55, 95), (144, 74), (104, 120), (130, 100), (71, 150), (111, 69), (72, 102)],
                 [(89, 12), (75, 3), (66, 175), (20, 70), (149, 46), (117, 94), (19, 86), (128, 52)],
                 [(40, 98), (36, 10), (78, 44), (33, 136), (39, 110), (143, 30), (58, 67), (22, 91)],
-                [(8, 88), (101, 32), (60, 4), (106, 93), (105, 45), (112, 27), (61, 119), (103, 48)]]),
+                [(8, 88), (101, 32), (60, 4), (106, 93), (105, 45), (112, 27), (61, 119), (103, 148)]]),
             'trio': SimpleDiceTable.from_lists([
                 [(13, 85), (126, 180), (125, 68), (177, 192), (187, 63), (24, 97), (145, 185), (137, 176)],
                 [(165, 113), (23, 76), (82, 2), (154, 190), (5, 84), (161, 182), (174, 116), (54, 124)],
                 [(43, 57), (135, 188), (56, 18), (189, 163), (25, 38), (166, 122), (179, 123), (169, 53)],
                 [(181, 129), (131, 186), (115, 170), (62, 178), (183, 132), (168, 171), (81, 151), (158, 64)],
                 [(134, 26), (118, 184), (160, 140), (114, 34), (42, 164), (146, 83), (141, 162), (73, 153)],
                 [(79, 191), (121, 155), (138, 156), (16, 173), (133, 167), (142, 172), (147, 159), (152, 157)]]),
         }
+        data_name = 'gerlach_scottish_dance'
 
         csv_reader = SimpleBarCollectionCSVReader()
         bars = csv_reader.read_csv(resources.files('musical_games') /
-                                   'data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv')
+                                   f'data/dice_games/{data_name}/scottish_dance_bars.csv')
 
         bar_collections = {'dance': bars,
                            'trio': bars}
 
-        template_loader = jinja2.PackageLoader('musical_games', f'data/dice_games/gerlach_scottish_dance/lilypond')
-        env_options = self._standard_jinja2_environment_options() | {'loader': template_loader}
-        jinja2_environment = jinja2.Environment(**env_options)
-
         midi_settings = SimpleMidiSettings(
             {'dance': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'},
              'trio': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
             {'dance': {'piano_right_hand': 0, 'piano_left_hand': 0},
              'trio': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'dance': {'piano_right_hand': 1, 'piano_left_hand': 0.75},
              'trio': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
 
         super().__init__('Gerlach', 'Scottish dance', dice_tables, bar_collections,
-                         jinja2_environment, midi_settings)
+                         self._generate_jinja2_environment(data_name), midi_settings)
```

### Comparing `musical_games-0.8.0/musical_games/external/base.py` & `musical_games-0.8.1/musical_games/external/base.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/external/images.py` & `musical_games-0.8.1/musical_games/external/images.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/external/lilypond.py` & `musical_games-0.8.1/musical_games/external/lilypond.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/external/midi_converters.py` & `musical_games-0.8.1/musical_games/external/midi_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/external/utils.py` & `musical_games-0.8.1/musical_games/external/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/external/wav_converters.py` & `musical_games-0.8.1/musical_games/external/wav_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/musical_games/utils.py` & `musical_games-0.8.1/musical_games/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/pyproject.toml` & `musical_games-0.8.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "musical_games"
 description = "Implementation of musical dice games from the 18th century."
 readme = "README.rst"
-version = "0.8.0"
+version = "0.8.1"
 requires-python = ">=3.11"
 keywords = ["Musical games", "Dice games", "Piano music"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
```

### Comparing `musical_games-0.8.0/scripts/demo_cpe_bach.py` & `musical_games-0.8.1/scripts/demo_cpe_bach.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/scripts/demo_gerlach_scottish_dance.py` & `musical_games-0.8.1/scripts/demo_gerlach_scottish_dance.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,37 +13,37 @@
 
 out_dir = Path('/tmp/test')
 
 dice_game = GerlachScottishDance()
 
 dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
 auto_convert_lilypond_file(out_dir / 'overview.ly')
-
-dice_game.compile_single_bar('dance', 5).to_file(out_dir / 'bar_dance_1.ly')
-auto_convert_lilypond_file(out_dir / 'bar_dance_1.ly')
-dice_game.compile_single_bar('trio', 5).to_file(out_dir / 'bar_trio_1.ly')
-auto_convert_lilypond_file(out_dir / 'bar_trio_1.ly')
+#
+dice_game.compile_single_bar('dance', 6).to_file(out_dir / 'bar_dance_6.ly')
+auto_convert_lilypond_file(out_dir / 'bar_dance_6.ly')
+dice_game.compile_single_bar('trio', 158).to_file(out_dir / 'bar_trio_158.ly')
+auto_convert_lilypond_file(out_dir / 'bar_trio_158.ly')
 
 dice_game.compile_single_dice_table_element('dance',
                                             dice_game.get_dice_tables()['dance'].get_elements()[0]).to_file(
     out_dir / 'single_dice_table_element_dance_0.ly')
 auto_convert_lilypond_file(out_dir / 'single_dice_table_element_dance_0.ly')
 
 dice_game.compile_single_dice_table_element('trio',
-                                            dice_game.get_dice_tables()['trio'].get_elements()[0]).to_file(
-    out_dir / 'single_dice_table_element_trio_0.ly')
-auto_convert_lilypond_file(out_dir / 'single_dice_table_element_trio_0.ly')
+                                            dice_game.get_dice_tables()['trio'].get_element(3, 7)).to_file(
+    out_dir / 'single_dice_table_element_trio_3_7.ly')
+auto_convert_lilypond_file(out_dir / 'single_dice_table_element_trio_3_7.ly')
 
 print(dice_game.get_duplicate_dice_table_elements('dance'))
 print(dice_game.get_duplicate_dice_table_elements('trio'))
 print(dice_game.count_unique_compositions(count_duplicates=True))
 print(dice_game.count_unique_compositions(count_duplicates=False))
 
 dice_tables = dice_game.get_dice_tables()
-row_ind = 0
+row_ind = 3
 bar_selection = GroupedStaffsBarSelection({
     'dance': [
         dice_tables['dance'].get_element(row_ind, 0),
         dice_tables['dance'].get_element(row_ind, 1),
         dice_tables['dance'].get_element(row_ind, 2),
         dice_tables['dance'].get_element(row_ind, 3),
         dice_tables['dance'].get_element(row_ind, 4),
@@ -66,17 +66,17 @@
 # bar_selection = dice_game.get_random_bar_selection(seed=1)
 pprint(bar_selection)
 
 dice_game.compile_composition_score(bar_selection,
                                     comment='Test', single_page=True).to_file(out_dir / 'composition_pdf.ly')
 auto_convert_lilypond_file(out_dir / 'composition_pdf.ly')
 
-midi_settings = dice_game.get_default_midi_settings()
-my_midi_settings = midi_settings.with_updated_instrument('flute', 'dance', 'piano_right_hand')
-
-dice_game.compile_composition_audio(bar_selection,
-    midi_settings=my_midi_settings).to_file(out_dir / 'composition_midi.ly')
-
-auto_convert_lilypond_file(
-    out_dir / 'composition_midi.ly',
-    soundfont=Path('/home/robbert/programming/python/opus_infinity.org/soundfonts/Musyng_Kite.sf2'))
-
+# midi_settings = dice_game.get_default_midi_settings()
+# my_midi_settings = midi_settings.with_updated_instrument('flute', 'dance', 'piano_right_hand')
+#
+# dice_game.compile_composition_audio(bar_selection,
+#                                     midi_settings=my_midi_settings).to_file(out_dir / 'composition_midi.ly')
+#
+# auto_convert_lilypond_file(
+#     out_dir / 'composition_midi.ly',
+#     soundfont=Path('/home/robbert/programming/python/opus_infinity.org/soundfonts/Musyng_Kite.sf2'))
+#
```

### Comparing `musical_games-0.8.0/scripts/demo_kirnberger_meneut_trio.py` & `musical_games-0.8.1/scripts/demo_kirnberger_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/scripts/demo_kirnberger_polonaise.py` & `musical_games-0.8.1/scripts/demo_kirnberger_polonaise.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/scripts/demo_mozart_contredanse.py` & `musical_games-0.8.1/scripts/demo_mozart_contredanse.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/scripts/demo_mozart_waltz.py` & `musical_games-0.8.1/scripts/demo_mozart_waltz.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/scripts/demo_stadler_meneut_trio.py` & `musical_games-0.8.1/scripts/demo_stadler_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/scripts/lilypond_copy.py` & `musical_games-0.8.1/scripts/lilypond_copy2.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 __licence__ = 'LGPL v3'
 
 from pathlib import Path
 
 from musical_games.dice_games.base import SimpleBarCollection, SimpleBar
 from musical_games.dice_games.data_csv import SimpleBarCollectionCSVWriter
 
-piano_right_hand_voice_1 = r"""\stemDown d''16 [\stemDown e''16 \stemDown f''16 \stemDown d''16] \stemDown b'8 [\stemDown d''8]
+piano_right_hand = r"""
+\stemDown d''16 [\stemDown e''16 \stemDown f''16 \stemDown d''16] \stemDown b'8 [\stemDown d''8]
 \stemDown a''16 [\stemDown gis''16 \stemDown a''16 \stemDown b''16] \stemDown c'''8 [\stemDown d'''8]
 \stemDown <c'' g''>8 [\stemDown <c'' fis''>8] <b' g''>4
 \stemDown g'8 [\stemDown c''16 \stemDown d''16] \stemDown e''16 [\stemDown f''16 \stemDown g''8]
-\stemDown e''8. [\stemDown d''16] \stemDown b'8 [\stemDown b'8]
+\stemDown e''8. [\stemDown d''16 \stemDown b'8 \stemDown b'8]
 \stemDown cis''16 [\stemDown cis''16 \stemDown e''16 \stemDown cis''16] \stemDown a'8 [\stemDown e''8]
 \stemDown c''8 [\stemDown <g' e''>8] <e' c''>4
 \stemDown c''8 [\stemDown c''16 \stemDown b'16] \stemUp a'8 [\stemUp e'8]
 \stemDown b'8 [\stemDown a''8] \stemDown g''8 [\stemDown f''8]
 \stemUp b'8 [\stemUp g'8] g''4
 \stemDown f''16 [\stemDown e''16 \stemDown f''16 \stemDown a''16] \stemDown f''8 [\stemDown b'8]
 \stemDown <e'' g''>8 [\stemDown <g' c''>8] <c'' e''>4
@@ -34,40 +35,40 @@
 \stemDown e''8 [\stemDown b'8] \stemDown gis''8 [\stemDown e''8]
 \stemDown c'''8 [\stemDown bes''8] \stemDown g''8 [\stemDown e''8]
 \stemDown e''8 [\stemDown c''8] \stemDown g''8 [\stemDown e''8]
 \stemDown a'8 [\stemDown c''8] \stemDown e''8 [\stemDown a''8]
 \stemDown c''8 [\stemDown e''8] \stemDown a''8 [\stemDown c'''8]
 \stemDown e''8 [\stemDown d''8] c''4
 \stemDown d''8 [\stemDown e''16 \stemDown d''16] \stemDown a'8 [\stemDown f''8]
-\stemUp e''8 [\stemUp c'''8] g''4
+{<<{\voiceOne \stemUp e''8 [\stemUp c'''8] g''4} \new Voice {\voiceTwo c''2}>>}
 \stemDown f''16 [\stemDown e''16 \stemDown dis''16 \stemDown e''16] \stemDown c'''8 [\stemDown e''8]
 <g' c'' e''>4 <g' b' d''>8 r8
 \stemDown g''8 [\stemDown b'8] \stemDown fis''8 [\stemDown a'8]
 \stemDown a''8 [\stemDown <c'' a''>8] <a' a''>4
 \stemDown c''16 [\stemDown d''16 \stemDown e''16 \stemDown c''16] \stemDown a'8 [\stemDown a''8]
 \stemDown a''8 [\stemDown f''8] \stemDown d''8 [\stemDown c''8]
 \stemDown a''16 [\stemDown f''16 \stemDown e''16 \stemDown d''16] \stemDown c''16 [\stemDown g''16 \stemDown b'16 \stemDown d''16]
 \stemDown f''16 [\stemDown e''16 \stemDown f''16 \stemDown g''16] \stemDown a''8 [\stemDown a''8]
-\stemUp e''8 [\stemUp f''16 \stemUp e''16] \stemUp dis''8 [\stemUp e''8]
+{<<{\voiceOne \stemUp e''8 [\stemUp f''16 \stemUp e''16] \stemUp dis''8 [\stemUp e''8]} \new Voice {\voiceTwo | c''2}>>}
 \stemUp <e' g'>8 [\stemUp <f' a'>16 \stemUp <e' g'>16] \stemDown <e' c''>8 [\stemDown <c'' e''>8]
 \stemUp gis'16 [\stemUp a'16 \stemUp b'16 \stemUp gis'16] \stemUp e'8 [\stemUp e''8]
 \stemDown a''8 [\stemDown gis''16 \stemDown a''16] \stemDown bes''8 [\stemDown a''8]
 \stemDown a'8 [\stemDown bes'16 \stemDown b'16] \tuplet 3/2 {\stemDown c''8 [\stemDown f''8 \stemDown a'8]}
 \stemDown c'''8 [\stemDown d''8] \stemDown b''8 [\stemDown d''8]
 \stemDown b'8 [\stemDown d''8] \stemDown g''8 [\stemDown b''8]
 \stemDown c''8 [\stemDown e''8] g'4
 \stemDown c''8 [\stemDown e''8] g''4
 \stemDown <gis' d''>8 [\stemDown <gis' e''>8] \stemDown <a' fis''>8 [\stemDown <b' gis''>8]
 \stemDown b''16 [\stemDown c'''16 \stemDown d'''16 \stemDown b''16] \stemDown g''8 [\stemDown f'''8]
 \stemUp c''8 [\stemUp <e' c''>8] <e' c''>4
 \stemDown c''8 [\stemDown <g' e''>8] <e' c''>4
 \stemDown c''8 [\stemDown c'''8] c''4
 \stemDown f''8 [\stemDown a''8] f''4
-\stemUp b''8 [\stemUp d'''16 \stemUp b''16] \stemUp a''8 [\stemUp gis''8]
-\stemUp d''8 [\stemUp e''16 \stemUp d''16] \stemUp d''8 [\stemUp g''8]
+{<<{\voiceOne \stemUp b''8 [\stemUp d'''16 \stemUp b''16] \stemUp a''8 [\stemUp gis''8]} \new Voice {\voiceTwo d''4 \stemDown c''8 [\stemDown b'8]}>>}
+{<<{\voiceOne \stemUp d''8 [\stemUp e''16 \stemUp d''16] \stemUp d''8 [\stemUp g''8]} \new Voice {\voiceTwo f'4 f'4}>>}
 \stemDown a''8 [\stemDown e''8] \stemDown cis'''8 [\stemDown e'''8]
 \stemDown bes'8 [\stemDown c''16 \stemDown e''16] g''4
 \stemDown g''8 [\stemDown d'''16 \stemDown dis'''16] \stemDown e'''8 [\stemDown g''8]
 \stemDown c''16 [\stemDown d''16 \stemDown e''16 \stemDown d''16] c''4
 \stemDown a'8 [\stemDown d''16 \stemDown e''16] \stemDown f''16 [\stemDown g''16 \stemDown a''8]
 \stemDown b''8 [\stemDown f''16 \stemDown b''16] \stemDown d'''8 [\stemDown f'''8]
 \stemDown g''8 [\stemDown fis''16 \stemDown g''16] \stemDown as''8 [\stemDown f''16 \stemDown d''16]
@@ -89,46 +90,46 @@
 \stemDown e''16 [\stemDown d''16 \stemDown cis''16 \stemDown d''16] \stemDown a''8 [\stemDown d''8]
 \stemDown c''8 [\stemDown a'8] \stemDown a''8 [\stemDown e''8] |
 \stemDown a''16 [\stemDown g''16 \stemDown f''16 \stemDown e''16] \stemDown f''8 [\stemDown d''8]
 \stemDown c'''16 [\stemDown d'''16 \stemDown e'''16 \stemDown f'''16] \stemDown g'''8 [\stemDown c'''8]
 \grace { \stemUp ais''8 } b''4 \grace { \stemUp ais''8 } \stemDown b''8 [\stemDown e'''8]
 a''2
 \stemDown c''8 [\stemDown e''8] \stemDown a'8 [\stemDown a''8]
-\stemUp d''16 [\stemUp cis''16 \stemUp d''16 \stemUp e''16] \stemUp f''8 [\stemUp d''8]
+{<<{\voiceOne \stemUp d''16 [\stemUp cis''16 \stemUp d''16 \stemUp e''16] \stemUp f''8 [\stemUp d''8]} \new Voice {\voiceTwo f'4 r4}>>}
 \stemDown c'''8 [\stemDown a''8] \stemDown b''8 [\stemDown c'''8]
 \stemUp <e' g'>8 [\stemUp <f' a'>16 \stemUp <e' g'>16] \stemUp <e' g'>8 [\stemUp <g' e''>8]
 \stemDown e''8 [\stemDown e''16 \stemDown d''16] \stemDown c''8 [\stemDown a'8]
 \stemDown <c'' c'''>8 [\stemDown <g'' b''>16 \stemDown <f'' a''>16] \stemDown <e'' g''>8 [\stemDown <f'' a''>8]
 \stemDown e'''8 [\stemDown c'''8] \stemDown g''8 [\stemDown e''8]
 \stemDown g''8 [\stemDown b'8] c''4
 \stemDown fis''16 [\stemDown g''16 \stemDown a''16 \stemDown fis''16] \stemDown d''8 [\stemDown c'''8]
 \stemDown b''8 [\stemDown e''8] \stemDown e'''8 [\stemDown e''8]
 \stemDown g''8 [\stemDown c''8] \stemDown e''8 [\stemDown c'''8]
-\stemUp e''16 [\stemUp f''16 \stemUp d''16 \stemUp e''16] c''4
+{<<{\voiceOne \stemUp e''16 [\stemUp f''16 \stemUp d''16 \stemUp e''16] c''4} \new Voice {\voiceTwo \stemDown g'8 [\stemDown f'8] e'4}>>}
 \stemDown a''16 [\stemDown g''16 \stemDown fis''16 \stemDown g''16] \stemDown c'''8 [\stemDown e''8]
 \stemDown f''8 [\stemDown a''8] c''4
 \stemDown <e'' g''>8 [\stemDown <c'' e''>8] <e'' c'''>4
-\stemUp a''8. \turn [\stemUp b''16] \stemUp c'''8 [\stemUp e''8]
+{<<{\voiceOne \stemUp a''8. \turn [\stemUp b''16] \stemUp c'''8 [\stemUp e''8]} \new Voice {\voiceTwo c''2}>>}
 \stemDown e''8 [\stemDown c''8] \stemDown a''8 [\stemDown g''8]
 \stemDown <g' c'' g''>8 [\stemDown <g' c''>8] \stemDown <a' c'' f''>8 [\stemDown <c'' f'' a''>8]
 \stemUp c''8 [\stemUp <e' c''>8] <e' c''>4
 \stemDown b''8 [\stemDown d'''16 \stemDown b''16] \stemDown a''8 [\stemDown gis''8]
 \stemDown g''16 [\stemDown f''16 \stemDown e''16 \stemDown d''16] \stemDown c''8 [\stemDown b'8]
 \stemDown a'8 [\stemDown d''8] \stemDown cis''16 [\stemDown d''16 \stemDown e''16 \stemDown d''16]
 \stemDown gis''8 [\stemDown e''8] \stemDown a''8 [\stemDown e''8]
 \stemDown g''16 [\stemDown fis''16 \stemDown g''16 \stemDown gis''16] \stemDown a''8 [\stemDown d''8]
 \stemDown a''16 [\stemDown gis''16 \stemDown a''16 \stemDown b''16] \stemDown c'''8 [\stemDown a''8]
-\stemUp f''8. \turn [\stemUp g''16] a''4
-\stemUp a''8 [\stemUp g''8] \stemUp fis''8 [\stemUp g''8]
+{<<{\voiceOne \stemUp f''8. \turn [\stemUp g''16] a''4} \new Voice {\voiceTwo a'2}>>}
+{<<{\voiceOne \stemUp a''8 [\stemUp g''8] \stemUp fis''8 [\stemUp g''8]} \new Voice {\voiceTwo b'2}>>}
 \stemDown b''8 [\stemDown e'''16 \stemDown d'''16] \stemDown c'''8 [\stemDown a''8]
 \stemDown b''8 [\stemDown e''8] \stemDown dis''16 [\stemDown e''16 \stemDown d''16 \stemDown b'16]
 \stemDown e''8 [\stemDown c''8] \stemDown a''8 [\stemDown e''8]
 \stemDown b''8 [\stemDown d'''16 \stemDown f'''16] \stemDown e'''8 [\stemDown gis''8]
 \grace { \stemUp a''8 } bes''4 \grace { \stemUp a''8 } \stemDown bes''8 [\stemDown g''8]
-\stemUp a''8. [\stemUp g''16] \stemUp f''8 [\stemUp f''8]
+{<<{\voiceOne \stemUp a''8. [\stemUp g''16] \stemUp f''8 [\stemUp f''8]} \new Voice {\voiceTwo cis''4 d''4}>>}
 \stemDown f''8 [\stemDown g'16 \stemDown b'16] \stemDown d''8 [\stemDown a''8]
 \stemDown e''8. [\stemDown f''16] \stemDown e''8 [\stemDown d''8]
 \stemDown f'''8 [\stemDown e'''8] \stemDown c'''8 [\stemDown a''8]
 \stemUp a'8 [\stemUp <c' a'>8] <c' a'>4
 \stemDown a'8 [\stemDown f''8] \stemDown as'16 [\stemDown f''16 \stemDown g'16 \stemDown g''16]
 d''4 r4
 \stemDown a''8 [\stemDown f'''8] \stemDown c'''8 [\stemDown a''8]
@@ -141,21 +142,21 @@
 \stemUp g'8 [\stemUp a'16 \stemUp g'16] \stemDown f''8 [\stemDown d''8]
 \grace { \stemUp dis''8 } e''4 \grace { \stemUp dis''8 } \stemDown e''8 [\stemDown cis''8]
 \stemDown a''8 [\stemDown f'''8] \stemDown c'''8 [\stemDown a''8]
 \stemUp gis'8 [\stemUp b'8] \stemDown e''8 [\stemDown gis''8]
 R2
 \stemDown g''8 [\stemDown fis''16 \stemDown g''16] \stemDown a''16 [\stemDown g''16 \stemDown f''16 \stemDown d''16]
 \stemUp e''8 [\stemUp e'8] e'4
-\stemUp d''8 [\stemUp bes''16 \stemUp d'''16] \stemUp c'''8 [\stemUp e''8]
+{<<{\voiceOne \stemUp d''8 [\stemUp bes''16 \stemUp d'''16] \stemUp c'''8 [\stemUp e''8]} \new Voice {\voiceTwo r8 <d' g'>8 r8 <g' bes'>8}>>}
 \stemDown a''16 [\stemDown bes''16 \stemDown c'''16 \stemDown d'''16] \stemDown bes''8 [\stemDown g''8]
 \stemDown b''8 [\stemDown a''8] g''4
 \stemDown bes''8 [\stemDown c'''16 \stemDown bes''16] \stemDown a''8 [\stemDown f''8]
 \stemDown b''16 [\stemDown a''16 \stemDown gis''16 \stemDown fis''16] \stemDown e''8 [\stemDown b''8]
 \grace { \stemUp b''8 } \stemDown c'''8 [\stemDown b''16 \stemDown a''16] \stemDown c'''8 [\stemDown b''16 \stemDown a''16]
-\stemUp a''8 [\stemUp g''8] \stemUp f''8 [\stemUp d''8]
+{<<{\voiceOne \stemUp a''8 [\stemUp g''8] \stemUp f''8 [\stemUp d''8]} \new Voice {\voiceTwo b'2}>>}
 \stemDown e''16 [\stemDown dis''16 \stemDown e''16 \stemDown gis''16] \stemDown b''8 [\stemDown e''8]
 \stemDown d'''8 [\stemDown e'''16 \stemDown f'''16] \stemDown f'''8 [\stemDown g''8]
 \stemDown e'''8. [\stemDown d'''16] \stemDown b''8 [\stemDown c'''8]
 \stemDown d''8 [\stemDown c'''8] \stemDown b''8 [\stemDown d''8]
 \stemDown a''8 [\stemDown <c'' a''>8] <c'' a''>4
 \stemDown f''16 [\stemDown g''16 \stemDown a''16 \stemDown f''16] \stemDown d''8 [\stemDown b'8]
 \stemDown d'''16 [\stemDown c'''16 \stemDown b''16 \stemDown a''16] \stemDown b''8 [\stemDown g''8]
@@ -178,15 +179,15 @@
 \stemDown a''16 [\stemDown b''16 \stemDown c'''16 \stemDown d'''16] \stemDown e'''8 [\stemDown a''8]
 \stemDown a''16 [\stemDown g''16 \stemDown fis''16 \stemDown g''16] \stemDown a''8 [\stemDown b''8]
 \stemDown g''8 [\stemDown fis''16 \stemDown g''16] \stemDown c'''8 [\stemDown e''8]
 \stemDown a''8 [\stemDown f'''8] \stemDown c'''8 [\stemDown a''8]
 c'''4 r4
 \stemDown gis''8 [\stemDown e'''8] \stemDown c'''8 [\stemDown a''8]
 \stemDown e'''8 [\stemDown d'''8] c'''4
-\stemUp c'''8. [\stemUp bes''16] \stemUp a''8 [\stemUp a''8]
+{<<{\voiceOne \stemUp c'''8. [\stemUp bes''16] \stemUp a''8 [\stemUp a''8]} \new Voice {\voiceTwo c''4 \stemDown c''8 [\stemDown c''8]}>>}
 \stemDown f''16 [\stemDown e''16 \stemDown e''16 \stemDown c'''16] \stemDown c'''8 [\stemDown e''8]
 \stemDown <a' f''>8 [\stemDown <c'' a''>8] <a' f''>4
 \stemDown g''16 [\stemDown fis''16 \stemDown g''16 \stemDown d'''16] \stemDown c'''16 [\stemDown bes''16 \stemDown g''16 \stemDown e''16]
 \stemDown cis''8 [\stemDown a''8] a'4
 \stemDown c'''8 [\stemDown b''16 \stemDown c'''16] \stemDown e'''16 [\stemDown d'''16 \stemDown bes''16 \stemDown g''16] |
 \stemDown bes''16 [\stemDown a''16 \stemDown gis''16 \stemDown a''16] f''4
 \grace { \stemUp b'8 } c''4 \grace { \stemUp b'8 } c''4
@@ -196,624 +197,219 @@
 \stemDown bes''8 [\stemDown c'''16 \stemDown d'''16] \stemDown c'''8 [\stemDown f''8]
 \tuplet 3/2 {\stemDown d''8 [\stemDown f''8 \stemDown a''8] } a''4
 \grace { \stemUp c''8 } \stemDown e''8 [\grace { \stemUp e''8 } \stemDown g''8] \grace { \stemUp g''8 } \stemDown bes''8 [\grace {\stemUp bes''8 } \stemDown d'''8]
 \stemDown c''8 [\stemDown e''8] c'''4
 \tuplet 3/2 {\stemDown a''8 [\stemDown gis''8 \stemDown g''8] } \stemDown g''8 [\stemDown f''8]
 \stemDown a''8 [\stemDown c'''8] a''4
 \stemDown g''16 [\stemDown f''16 \stemDown e''16 \stemDown g''16] f''4
-\stemDown f''8 [\stemDown <c'' a''>8] <a' f''>4"""
-
-piano_right_hand_voice_2 = r"""s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-c''2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-| c''2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-d''4 \stemDown c''8 [\stemDown b'8]
-f'4 f'4
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-f'4 r4
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-\stemDown g'8 [\stemDown f'8] e'4
-s2
-s2
-s2
-c''2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-a'2
-b'2
-s2
-s2
-s2
-s2
-s2
-cis''4 d''4
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-r8 <d' g'>8 r8 <g' bes'>8
-s2
-s2
-s2
-s2
-s2
-b'2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-c''4 \stemDown c''8 [\stemDown c''8]
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2
-s2"""
+\stemDown f''8 [\stemDown <c'' a''>8] <a' f''>4
+"""
 
-piano_left_hand_voice_1 = r"""r8 <b f'>8 \stemUp <d' f'>8 [\stemUp <b f'>8]
+piano_left_hand = r"""
+{<<{\voiceOne r8 <b f'>8 \stemUp <d' f'>8 [\stemUp <b f'>8]} \new Voice {\voiceTwo g2}>>}
 \stemDown a8 [\stemDown <c' e'>8] \stemDown d8 [\stemDown <a d'>8]
 \stemDown <g d'>8 [\stemDown <a d'>8] <g d'>4
 \stemDown e8 [\stemDown g8] \stemDown c'8 [\stemDown e'8]
-\clef "treble" r8 <b e'>8 \stemUp <d' e'>8 [\stemUp <d' e'>8]
-\clef "bass" r8 <e' g'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]
+\clef "treble"{<<{\voiceOne r8 <b e'>8 \stemUp <d' e'>8 [\stemUp <d' e'>8]} \new Voice {\voiceTwo gis2}>>}
+\clef "bass" {<<{\voiceOne r8 <e' g'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]} \new Voice {\voiceTwo a2}>>}
 \stemDown <c' e'>8 [\stemDown c'8] c4
 \stemDown a,8 [\stemDown <a c'>8] \stemDown <a c'>8 [\stemDown <a c'>8]
-r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]
+{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]} \new Voice {\voiceTwo g2}>>}
 \stemDown <g b d'>8 [\stemDown <g b>8] <g b>4
 \stemDown f8 [\stemDown <a d'>8] \stemDown g8 [\stemDown <d' f'>8]
 \stemDown c8 [\stemDown e'8] c'4
 <f f'>4 \stemDown <a e'>8 [\stemDown es'8]
-r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]
-r8 c'8 \stemUp c'8 [\stemUp c'8]
-\clef "treble" r8 <f' g'>8 \stemUp <f' g'>8 [\stemUp <f' g'>8]
-\clef "bass" \stemDown <e gis b>8 [\grace { \stemUp dis'8 } \stemDown e'8] e4
-r8 <d' f'>8 \stemUp <d' f'>8 [\stemUp <d' f'>8]
+{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]} \new Voice {\voiceTwo g2}>>}
+{<<{\voiceOne r8 c'8 \stemUp c'8 [\stemUp c'8]} \new Voice {\voiceTwo c2}>>}
+\clef "treble" {<<{\voiceOne r8 <f' g'>8 \stemUp <f' g'>8 [\stemUp <f' g'>8]} \new Voice {\voiceTwo b2}>>}
+\stemDown <e gis b>8 [\grace { \stemUp dis'8 } \stemDown e'8] e4
+\clef "bass" {<<{\voiceOne r8 <d' f'>8 \stemUp <d' f'>8 [\stemUp <d' f'>8]} \new Voice {\voiceTwo d4 s4}>>}
 <fis c' d'>4 \stemDown <g b d'>8 [\stemDown <gis b d'>8] |
-r8 <a c'>8 \stemUp <a c'>8 [\stemUp <fis d'>8]
-r8 <b f'>8 r8 <b f'>8
+{<<{\voiceOne r8 <a c'>8 \stemUp <a c'>8 [\stemUp <fis d'>8]} \new Voice {\voiceTwo d2}>>}
+{<<{\voiceOne r8 <b f'>8 r8 <b f'>8} \new Voice {\voiceTwo g4 g4}>>}
 <fis a c' es'>4 <g c' e'>4
 \stemDown g8 [\stemDown <d' e'>8] \stemDown b8 [\stemDown <d' e'>8]
 \stemDown g8 [\stemDown <c' e'>8] \stemDown bes8 [\stemDown <c' g'>8]
-r8 <bes c'>8 \stemUp <bes c'>8 [\stemUp <bes c'>8]
+{<<{\voiceOne r8 <bes c'>8 \stemUp <bes c'>8 [\stemUp <bes c'>8]} \new Voice {\voiceTwo c2}>>}
 \stemDown a8 [\stemDown c'8] \stemDown e'8 [\stemDown a'8]
-r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo a2}>>}
 \stemDown <g c' e'>8 [\stemDown <g b f'>8] <c' e'>4
-r8 <a d'>8 r8 <a d'>8
+{<<{\voiceOne r8 <a d'>8 r8 <a d'>8} \new Voice {\voiceTwo f4 d4}>>}
 \stemDown c8 [\stemDown e8] \stemDown <c' e'>8 [\stemDown g8]
 \stemDown c8 [\stemDown <c' e'>8] \stemDown a8 [\stemDown <c' e'>8]
 g2
 \stemDown e8 [\stemDown <g b>8] \stemDown b,8 [\stemDown <fis b>8]
 \stemDown <a c'>8 [\stemDown <a e'>8] <a c'>4
-r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo a2}>>}
 <f a d'>4 <fis a d'>4
 \stemDown f8 [\stemDown <a d'>8] \stemDown <g c' e'>8 [\stemDown <g b f'>8]
-r8 <a c'>8 \stemUp <a c'>8 [\stemUp <a c'>8]
+{<<{\voiceOne r8 <a c'>8 \stemUp <a c'>8 [\stemUp <a c'>8]} \new Voice {\voiceTwo f2}>>}
 \stemDown c8 [\stemDown g8] \stemDown <c' e'>8 [\stemDown g8] |
-r8 c'8 \stemUp c'8 [\stemUp c'8]
-r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]
-r8 <cis' e'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]
-r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]
-r8 <fis c'>8 r8 b8
-r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]
+{<<{\voiceOne r8 c'8 \stemUp c'8 [\stemUp c'8]} \new Voice {\voiceTwo c2}>>}
+{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]} \new Voice {\voiceTwo e2}>>}
+\clef "bass" {<<{\voiceOne r8 <cis' e'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]} \new Voice {\voiceTwo a4 s4}>>}
+{<<{\voiceOne r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]} \new Voice {\voiceTwo f2}>>}
+{<<{\voiceOne r8 <fis c'>8 r8 b8} \new Voice {\voiceTwo d4 g4}>>}
+{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]} \new Voice {\voiceTwo g2}>>}
 \stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
 \stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
 \stemDown e8 [\stemDown e'8] \stemDown <dis' e'>8 [\stemDown <d' e'>8]
-r8 <b f'>8 \stemUp <b d'>8 [\stemUp <b d'>8]
+{<<{\voiceOne r8 <b f'>8 \stemUp <b d'>8 [\stemUp <b d'>8]} \new Voice {\voiceTwo g2}>>}
 \stemDown <c' e'>8 [\stemDown g8] c4
 \stemDown <c' e'>8 [\stemDown c'8] c4
 \stemDown <c' e'>8 [\stemDown <e' g'>8] <c' e'>4
 \stemDown <f a>8 [\stemDown c'8] <f a>4
-r8 f'8 \stemUp e'8 [\stemUp d'8]
-r8 b8 \stemUp b8 [\stemUp b8]
-r8 <cis' g'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]
+{<<{\voiceOne r8 f'8 \stemUp e'8 [\stemUp d'8]} \new Voice {\voiceTwo f4 \stemDown e8 [\stemDown e8]}>>}
+{<<{\voiceOne r8 b8 \stemUp b8 [\stemUp b8]} \new Voice {\voiceTwo g2}>>}
+{<<{\voiceOne r8 <cis' g'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]} \new Voice {\voiceTwo a2}>>}
 \stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
 <g b f'>4 <g c' e'>4
 \stemDown <g c' e'>8 [\stemDown <g b f'>8] <c' e'>4 |
 \stemDown f8 [\stemDown a8] \stemDown d'8 [\stemDown f'8]
-r8 <f b>8 \stemUp <f b>8 [\stemUp <f b>8]
+{<<{\voiceOne r8 <f b>8 \stemUp <f b>8 [\stemUp <f b>8]} \new Voice {\voiceTwo d2}>>}
 <bes d' g'>4 <bes d' f'>4
 \stemDown a8 [\stemDown <c' f'>8] \stemDown f8 [\stemDown <c' f'>8]
 \stemUp <a, c>8 [\stemUp e,8] a,,4
-r8 <g c'>8 \stemUp <g c'>8 [\stemUp <g c'>8]
-r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]
+{<<{\voiceOne r8 <g c'>8 \stemUp <g c'>8 [\stemUp <g c'>8]} \new Voice {\voiceTwo c2}>>}
+{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b d'>8]} \new Voice {\voiceTwo g2}>>}
 <g bes c'>4 <f a c'>4
-r8 f'8 r8 f'8
-r8 <bes e'>8 r8 <a c'>8
+{<<{\voiceOne r8 f'8 r8 f'8} \new Voice {\voiceTwo c'4 d'4}>>}
+{<<{\voiceOne r8 <bes e'>8 r8 <a c'>8} \new Voice {\voiceTwo c4 f4}>>}
 \stemDown <g b>8 [\stemDown g8] g,4
-r8 <a d'>8 \stemUp <a d'>8 [\stemUp <a d'>8]
+{<<{\voiceOne r8 <a d'>8 \stemUp <a d'>8 [\stemUp <a d'>8]} \new Voice {\voiceTwo fis2}>>}
 \stemDown f8 [\stemDown <a d'>8] \stemDown <g c' e'>8 [\stemDown <g b f'>8]
 \stemDown e8 [\stemDown <c' e'>8] \stemDown e8 [\stemDown <b d'>8]
-r8 <c' e'>8 r8 <c' e'>8
-r8 <c' d'>8 \stemUp <c' d'>8 [\stemUp <c' d'>8]
+{<<{\voiceOne r8 <c' e'>8 r8 <c' e'>8} \new Voice {\voiceTwo a4 a4}>>}
+{<<{\voiceOne r8 <c' d'>8 \stemUp <c' d'>8 [\stemUp <c' d'>8]} \new Voice {\voiceTwo fis2}>>}
 \stemDown a8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
 \stemDown c8 [\stemDown c'8] \stemDown <b c'>8 [\stemDown <bes c'>8]
 \stemDown fis8 [\stemDown <a d'>8] \stemDown fis8 [\stemDown <c' d'>8]
-r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo a2}>>}
 \stemDown d8 [\stemDown <d' f'>8] \stemDown <d' f'>8 [\stemDown <d' f'>8]
-r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo g2}>>}
 \stemDown e8 [\stemDown <gis d'>8] \stemDown gis8 [\stemDown <d' e'>8]
-r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
-r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo a2}>>}
+{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo a2}>>}
 \stemDown bes,8 [\stemDown <bes d'>8] \stemDown <bes d'>8 [\stemDown <bes d'>8]
 \stemDown <a c'>8 [\stemDown <fis a d'>8] \stemDown <g b f'>8 [\stemDown <a c' e'>8]
-r8 c'8 \stemUp c'8 [\stemUp c'8]
+{<<{\voiceOne r8 c'8 \stemUp c'8 [\stemUp c'8]} \new Voice {\voiceTwo c2}>>}
 \stemDown a,8 [\stemDown <a c'>8] \stemDown <a c'>8 [\stemDown <a c'>8]
-r8 c'8 \stemUp c'8 [\stemUp c'8]
+{<<{\voiceOne r8 c'8 \stemUp c'8 [\stemUp c'8]} \new Voice {\voiceTwo c2}>>}
 \stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
 \stemDown <g d' f'>8 [\stemDown <g d' f'>8] <c' e'>4
-r8 <c' d'>8 r8 <c' d'>8
+{<<{\voiceOne r8 <c' d'>8 r8 <c' d'>8} \new Voice {\voiceTwo a4 fis4}>>}
 <e gis b>4 \stemDown e'8 [\stemDown e8]
 \stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
 \stemDown <g c'>8 [\stemDown <g b>8] <c c'>4
 \stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' g'>8]
-r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]
-r8 c'8 c'4
+{<<{\voiceOne r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]} \new Voice {\voiceTwo a2}>>}
+{<<{\voiceOne r8 c'8 c'4} \new Voice {\voiceTwo c2}>>}
 \stemDown <c' e'>8. [\stemDown b16] \stemDown a8 [\stemDown <c' e'>8]
-r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
+{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo c2}>>}
 e4 \stemDown f8 [\stemDown f8]
 \stemDown <c' e'>8 [\stemDown g8] c4
-r8 <a b d'>8 \stemUp <e c'>8 [\stemUp <e b d'>8]
-r8 <a d'>8 \stemUp <e a e'>8 [\stemUp <e gis d'>8]
-r8 <fis c'>8 \stemUp <fis c'>8 [\stemUp <fis c'>8]
+{<<{\voiceOne r8 <a b d'>8 \stemUp <e c'>8 [\stemUp <e b d'>8]} \new Voice {\voiceTwo f4 s4}>>}
+{<<{\voiceOne r8 <a d'>8 \stemUp <e a e'>8 [\stemUp <e gis d'>8]} \new Voice {\voiceTwo f4 s4}>>}
+{<<{\voiceOne r8 <fis c'>8 \stemUp <fis c'>8 [\stemUp <fis c'>8]} \new Voice {\voiceTwo d2}>>}
 <e b d'>4 <e a c'>4
-r8 <b f'>8 \stemUp <b f'>8 [\stemUp <b f'>8]
-r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]
-\stemUp a8. [\stemUp g16] f4
+{<<{\voiceOne r8 <b f'>8 \stemUp <b f'>8 [\stemUp <b f'>8]} \new Voice {\voiceTwo g2}>>}
+{<<{\voiceOne r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]} \new Voice {\voiceTwo f2}>>}
+{<<{\voiceOne \stemUp a8. [\stemUp g16] f4} \new Voice {\voiceTwo c'2}>>}
 \stemUp g,8 [\stemUp g8] \stemDown <d' f'>8 [\stemDown b8]
 \stemDown gis8 [\stemDown <b e'>8] \stemDown a8 [\stemDown <c' e'>8]
-r8 <gis d'>8 \stemUp <gis d'>8 [\stemUp <gis d'>8]
+{<<{\voiceOne r8 <gis d'>8 \stemUp <gis d'>8 [\stemUp <gis d'>8]} \new Voice {\voiceTwo e2}>>}
 \stemDown a,8 [\stemDown <c' e'>8] \stemDown a8 [\stemDown <c' e'>8]
 \stemDown d8 [\stemDown <a b>8] \stemDown e8 [\stemDown <b d'>8]
 \stemDown c8 [\stemDown <g e'>8] \stemDown <g e'>8 [\stemDown <bes e'>8]
-r8 e'8 d'8 r8
+{<<{\voiceOne r8 e'8 d'8 r8} \new Voice {\voiceTwo a4 r8 d8}>>}
 \stemDown g8 [\stemDown <b f'>8] \stemDown g8 [\stemDown <b f'>8]
-r8 <b e'>8 \stemUp <b e'>8 [\stemUp <b e'>8]
-r8 <a e'>8 \stemUp <a e'>8 [\stemUp <a e'>8]
+{<<{\voiceOne r8 <b e'>8 \stemUp <b e'>8 [\stemUp <b e'>8]} \new Voice {\voiceTwo gis2}>>}
+{<<{\voiceOne r8 <a e'>8 \stemUp <a e'>8 [\stemUp <a e'>8]} \new Voice {\voiceTwo e2}>>}
 \stemDown <a c'>8 [\stemDown e8] a,4
 <d' f'>4 \stemDown <c' d'>8 [\stemDown <b d'>8]
 \stemDown d8 [\stemDown f'8] d'4
-r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]
+{<<{\voiceOne r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]} \new Voice {\voiceTwo f2}>>}
 \stemDown <a c'>8 [\stemDown e8] a,4
-r8 <c' f'>8 r8 <d' f'>8
-r8 <bes e'>8 \stemUp <bes e'>8 [\stemUp <bes e'>8]
-r8 <a d'>8 r8 <d' f'>8
+{<<{\voiceOne r8 <c' f'>8 r8 <d' f'>8} \new Voice {\voiceTwo a4 bes4}>>}
+{<<{\voiceOne r8 <bes e'>8 \stemUp <bes e'>8 [\stemUp <bes e'>8]} \new Voice {\voiceTwo g2}>>}
+{<<{\voiceOne r8 <a d'>8 r8 <d' f'>8} \new Voice {\voiceTwo f4 g4}>>}
 <f c' d'>4 \stemDown <g b d'>8 [\stemDown <g d' f'>8]
-r8 <a f'>8 \stemUp <a f'>8 [\stemUp <a f'>8]
-r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b f'>8]
-r8 <cis' g'>8 \stemUp <cis' g'>8 [\stemUp <e' g'>8]
-r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]
-r8 <gis d'>8 \stemUp <b e'>8 [\stemUp <b e'>8]
-a4 \stemUp c'8 [\stemUp e'8]
-r8 <b d'>8 \stemUp <b f'>8 [\stemUp <b f'>8]
+{<<{\voiceOne r8 <a f'>8 \stemUp <a f'>8 [\stemUp <a f'>8]} \new Voice {\voiceTwo f2}>>}
+{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <b f'>8]} \new Voice {\voiceTwo g2}>>}
+{<<{\voiceOne r8 <cis' g'>8 \stemUp <cis' g'>8 [\stemUp <e' g'>8]} \new Voice {\voiceTwo a2}>>}
+{<<{\voiceOne r8 <c' f'>8 \stemUp <c' f'>8 [\stemUp <c' f'>8]} \new Voice {\voiceTwo f2}>>}
+{<<{\voiceOne r8 <gis d'>8 \stemUp <b e'>8 [\stemUp <b e'>8]} \new Voice {\voiceTwo e2}>>}
+{<<{\voiceOne a4 \stemUp c'8 [\stemUp e'8]} \new Voice {\voiceTwo a,4 \stemDown c8 [\stemDown e8]}>>}
+{<<{\voiceOne r8 <b d'>8 \stemUp <b f'>8 [\stemUp <b f'>8]} \new Voice {\voiceTwo g2}>>}
 \stemDown <e g b>8 [\stemDown <e g c'>8] <e g>4
 bes4 c'4
-r8 <a d'>8 r8 <bes d'>8
+{<<{\voiceOne r8 <a d'>8 r8 <bes d'>8} \new Voice {\voiceTwo fis4 g4}>>}
 \stemDown <g b d'>8 [\stemDown <fis c' d'>8] <g b f'>4 |
-r8 <c' e'>8 r8 <a c'>8
-r8 <gis d'>8 \stemUp <gis d'>8 [\stemUp <gis d'>8]
-r8 <c' es'>8 r8 <c' es'>8
+{<<{\voiceOne r8 <c' e'>8 r8 <a c'>8} \new Voice {\voiceTwo g4 f4}>>}
+{<<{\voiceOne r8 <gis d'>8 \stemUp <gis d'>8 [\stemUp <gis d'>8]} \new Voice {\voiceTwo e2}>>}
+{<<{\voiceOne r8 <c' es'>8 r8 <c' es'>8} \new Voice {\voiceTwo fis4 f4}>>}
 \stemUp g,8 [\stemUp g8] \stemDown <d' f'>8 [\stemDown g8]
-r8 <b e'>8 r8 <d' e'>8
+{<<{\voiceOne r8 <b e'>8 r8 <d' e'>8} \new Voice {\voiceTwo gis4 gis4}>>}
 <gis b f'>4 <g b f'>4
-r8 <b e'>8 \stemUp <b e'>8 [\stemUp <b e'>8]
+{<<{\voiceOne r8 <b e'>8 \stemUp <b e'>8 [\stemUp <b e'>8]} \new Voice {\voiceTwo gis2}>>}
 \stemDown d8 [\stemDown <a f'>8] \stemDown e8 [\stemDown <b e'>8]
 \stemDown <a c'>8 [\stemDown <a e'>8] <a c'>4
-r8 <b d'>8 \stemUp <b d'>8 [\stemUp <d' f'>8]
-r8 <c' d'>8 r8 <b d'>8
-r8 <c' f'>8 r8 <c' f'>8
-r8 <a b>8 r8 <b d'>8
+{<<{\voiceOne r8 <b d'>8 \stemUp <b d'>8 [\stemUp <d' f'>8]} \new Voice {\voiceTwo g2}>>}
+{<<{\voiceOne r8 <c' d'>8 r8 <b d'>8} \new Voice {\voiceTwo fis4 g4}>>}
+{<<{\voiceOne r8 <c' f'>8 r8 <c' f'>8} \new Voice {\voiceTwo a4 f4}>>}
+{<<{\voiceOne r8 <a b>8 r8 <b d'>8} \new Voice {\voiceTwo d4 e4}>>}
 \stemDown <a c'>8 [\stemDown <e gis d'>8] <a c'>4
 \stemDown e8 [\stemDown <c' e'>8] \stemDown <e b d'>8 [\stemDown <e b d'>8]
 \stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
-r8 <g c'>8 r8 <a c'>8
+{<<{\voiceOne r8 <g c'>8 r8 <a c'>8} \new Voice {\voiceTwo e4 f4}>>}
 \stemDown <a c'>8 [\stemDown e8] a,4
 \clef "treble" \stemUp <bes d' g'>8 [\stemUp <b d' gis'>8] \stemUp <c' f' a'>8 [\stemUp <c' g' bes'>8]
-\clef "bass" \stemDown e8 [\stemDown <c' e'>8] \stemDown f8 [\stemDown <a f'>8]
-r8 <c' e'>8 r8 <d' e'>8
-r8 <b d'>8 r8 <gis d' e'>8
+\stemDown e8 [\stemDown <c' e'>8] \stemDown f8 [\stemDown <a f'>8]
+{<<{\voiceOne r8 <c' e'>8 r8 <d' e'>8} \new Voice {\voiceTwo a4 gis4}>>}
+{<<{\voiceOne r8 <b d'>8 r8 <gis d' e'>8} \new Voice {\voiceTwo f4 e4}>>}
 \stemDown a8 [\stemDown <c' e'>8] \stemDown f8 [\stemDown <c' d'>8]
 \stemDown <c e g>8 [\stemDown c'8] \stemDown c'8 [\stemDown c8]
 \stemDown d8 [\stemDown <d' f'>8] \stemDown <d' f'>8 [\stemDown <d' f'>8]
 \stemDown <a, a>8 [\stemDown <c' e'>8] \stemDown a8 [\stemDown <c' e'>8]
-r8 <cis' g'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]
-r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
-r8 <b f'>8 \stemUp <d' f'>8 [\stemUp <d' f'>8]
+{<<{\voiceOne r8 <cis' g'>8 \stemUp <cis' g'>8 [\stemUp <cis' g'>8]} \new Voice {\voiceTwo a2}>>}
+{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo a2}>>}
+{<<{\voiceOne r8 <b f'>8 \stemUp <d' f'>8 [\stemUp <d' f'>8]} \new Voice {\voiceTwo g2}>>}
 <g b f'>4 \stemDown <g c' e'>8 [\stemDown <g bes c'>8] |
 \stemDown f8 [\stemDown <a f'>8] \stemDown a8 [\stemDown <c' f'>8]
 \stemDown <c' e'>8 [\stemDown g'8] <c' e'>4
-r8 <gis e'>8 r8 <c' e'>8
-\stemUp g8 [\stemUp f8] e4
-r8 <c' e'>8 r8 <c' f'>8
-r8 <c' e'>8 r8 <c' e'>8
+{<<{\voiceOne r8 <gis e'>8 r8 <c' e'>8} \new Voice {\voiceTwo e4 a4}>>}
+{<<{\voiceOne \stemUp g8 [\stemUp f8] e4} \new Voice {\voiceTwo c2}>>}
+{<<{\voiceOne r8 <c' e'>8 r8 <c' f'>8} \new Voice {\voiceTwo g4 f4}>>}
+{<<{\voiceOne r8 <c' e'>8 r8 <c' e'>8} \new Voice {\voiceTwo g4 a4}>>}
 \stemDown a'8 [\stemDown f'8] f4
-\clef "treble" r8 <d' g'>8 r8 <g' bes'>8
-<a a'>4 a4
-\clef "bass" r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]
-r8 <c' f'>8 r8 <c' f'>8
-r8 <a f'>8 \stemUp <a f'>8 [\stemUp <a f'>8]
-\stemUp <c' e'>8 [\stemUp d'8] c'4
-r8 <c' e'>8 r8 <c' e'>8
-\stemUp e'8 [\stemUp d'8] c'4
+\clef "treble" {<<{\voiceOne r8 <d' g'>8 r8 <g' bes'>8} \new Voice {\voiceTwo bes4 c'4}>>}
+\clef "treble" <a a'>4 a4
+{<<{\voiceOne r8 <c' e'>8 \stemUp <c' e'>8 [\stemUp <c' e'>8]} \new Voice {\voiceTwo g2}>>}
+{<<{\voiceOne r8 <c' f'>8 r8 <c' f'>8} \new Voice {\voiceTwo f4 a4}>>}
+{<<{\voiceOne r8 <a f'>8 \stemUp <a f'>8 [\stemUp <a f'>8]} \new Voice {\voiceTwo f2}>>}
+{<<{\voiceOne \stemUp <c' e'>8 [\stemUp d'8] c'4} \new Voice {\voiceTwo a2}>>}
+{<<{\voiceOne r8 <c' e'>8 r8 <c' e'>8} \new Voice {\voiceTwo bes4 g4}>>}
+{<<{\voiceOne \stemUp e'8 [\stemUp d'8] c'4} \new Voice {\voiceTwo a2}>>}
 <g c' e'>4 <a c' f'>4
 \stemDown d8 [\stemDown <d' f'>8] \stemDown <d' f'>8 [\stemDown <d' f'>8]
-r8 <c' e'>8 r8 <c' e'>8
+{<<{\voiceOne r8 <c' e'>8 r8 <c' e'>8} \new Voice {\voiceTwo bes4 g4}>>}
 \stemDown c8 [\stemDown <c' e'>8] \stemDown <c' e'>8 [\stemDown <c' e'>8]
-\clef "treble" r8 <d' f' g'>8 \stemUp <d' f' g'>8 [\stemUp <d' f' g'>8]
-\clef "bass" \stemDown <a c'>8 [\stemDown <a e'>8] <a c'>4
+\clef "treble" {<<{\voiceOne r8 <d' f' g'>8 \stemUp <d' f' g'>8 [\stemUp <d' f' g'>8]} \new Voice {\voiceTwo b2}>>}
+\stemDown <a c'>8 [\stemDown <a e'>8] <a c'>4
 \stemDown d8 [\stemDown <a f'>8] \stemDown <a f'>8 [\stemDown <a f'>8]
-\stemUp <f, a,>8 [\stemUp c,8] a,,4"""
-
-piano_left_hand_voice_2 = r"""g2
-s2
-s2
-s2
-gis2
-a2
-s2
-s2
-g2
-s2
-s2
-s2
-s2
-g2
-c2
-b2
-s2
-d4 s4
-s2
-d2
-g4 g4
-s2
-s2
-s2
-c2
-s2
-a2
-s2
-f4 d4
-s2
-s2
-s2
-s2
-s2
-a2
-s2
-s2
-f2
-s2
-c2
-e2
-a4 s4
-f2
-d4 g4
-g2
-s2
-s2
-s2
-g2
-s2
-s2
-s2
-s2
-f4 \stemDown e8 [\stemDown e8]
-g2
-a2
-s2
-s2
-s2
-s2
-d2
-s2
-s2
-s2
-c2
-g2
-s2
-c'4 d'4
-c4 f4
-s2
-fis2
-s2
-s2
-a4 a4
-fis2
-s2
-s2
-s2
-a2
-s2
-g2
-s2
-a2
-a2
-s2
-s2
-c2
-s2
-c2
-s2
-s2
-a4 fis4
-s2
-s2
-s2
-s2
-a2
-c2
-s2
-c2
-s2
-s2
-f4 s4
-f4 s4
-d2
-s2
-g2
-f2
-c'2
-s2
-s2
-e2
-s2
-s2
-s2
-a4 r8 d8
-s2
-gis2
-e2
-s2
-s2
-s2
-f2
-s2
-a4 bes4
-g2
-f4 g4
-s2
-f2
-g2
-a2
-f2
-e2
-a,4 \stemDown c8 [\stemDown e8]
-g2
-s2
-s2
-fis4 g4
-s2
-g4 f4
-e2
-fis4 f4
-s2
-gis4 gis4
-s2
-gis2
-s2
-s2
-g2
-fis4 g4
-a4 f4
-d4 e4
-s2
-s2
-s2
-e4 f4
-s2
-s2
-s2
-a4 gis4
-f4 e4
-s2
-s2
-s2
-s2
-a2
-a2
-g2
-s2
-s2
-s2
-e4 a4
-c2
-g4 f4
-g4 a4
-s2
-bes4 c'4
-s2
-g2
-f4 a4
-f2
-a2
-bes4 g4
-a2
-s2
-s2
-bes4 g4
-s2
-b2
-s2
-s2
-s2"""
-
-rh_v_1 = piano_right_hand_voice_1.split('\n')
-rh_v_2 = piano_right_hand_voice_2.split('\n')
-
-lh_v_1 = piano_left_hand_voice_1.split('\n')
-lh_v_2 = piano_left_hand_voice_2.split('\n')
-
-voice_format = r'{{<<{{\voiceOne {voice_1}}} \new Voice {{\voiceTwo {voice_2}}}>>}}'
-
-
-piano_right_hand = []
-for rhv1, rhv2 in zip(rh_v_1, rh_v_2):
-    if rhv2.startswith('s2'):
-        piano_right_hand.append(rhv1.strip())
-    else:
-        piano_right_hand.append(voice_format.format(voice_1=rhv1.strip(), voice_2=rhv2.strip()))
-
-
-piano_left_hand = []
-for lhv1, lhv2 in zip(lh_v_1, lh_v_2):
-    if lhv2.startswith('s2'):
-        piano_left_hand.append(lhv1.strip())
-    else:
-        piano_left_hand.append(voice_format.format(voice_1=lhv1.strip(), voice_2=lhv2.strip()))
+\stemUp <f, a,>8 [\stemUp c,8] a,,4
+"""
 
+right_hand_bars = piano_right_hand.split('\n')
+left_hand_bars = piano_left_hand.split('\n')
 
 sync_bars = {}
-for ind, (piano_right_hand, piano_left_hand) in enumerate(zip(piano_right_hand, piano_left_hand)):
-    sync_bars[ind + 1] = {'piano_right_hand': SimpleBar(piano_right_hand),
-                          'piano_left_hand': SimpleBar(piano_left_hand)}
+for ind, (piano_right_hand_bar, piano_left_hand_bar) in enumerate(zip(right_hand_bars[1:-1], left_hand_bars[1:-1])):
+    sync_bars[ind + 1] = {'piano_right_hand': SimpleBar(piano_right_hand_bar),
+                          'piano_left_hand': SimpleBar(piano_left_hand_bar)}
 
 a = SimpleBarCollection(sync_bars)
 
 writer = SimpleBarCollectionCSVWriter()
-writer.write_csv(a, Path('/tmp/scottish_dance_bars.csv'))
+writer.write_csv(a, Path('/home/robbert/programming/python/musical-games/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars2.csv'))
 
 print()
```

### Comparing `musical_games-0.8.0/tox.ini` & `musical_games-0.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.0/PKG-INFO` & `musical_games-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musical_games
-Version: 0.8.0
+Version: 0.8.1
 Summary: Implementation of musical dice games from the 18th century.
 Keywords: Musical games,Dice games,Piano music
 Author-email: Robbert Harms <robbert@xkls.nl>
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

