# Comparing `tmp/csvkit-1.5.0.tar.gz` & `tmp/csvkit-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvkit-1.5.0.tar", last modified: Thu Mar 28 15:27:03 2024, max compression
+gzip compressed data, was "csvkit-2.0.0.tar", last modified: Wed May  1 19:52:12 2024, max compression
```

## Comparing `csvkit-1.5.0.tar` & `csvkit-2.0.0.tar`

### file list

```diff
@@ -1,220 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.185437 csvkit-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-28 15:26:39.000000 csvkit-1.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22509 2024-03-28 15:26:39.000000 csvkit-1.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-28 15:26:39.000000 csvkit-1.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-28 15:26:39.000000 csvkit-1.5.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-28 15:26:39.000000 csvkit-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-03-28 15:27:03.185437 csvkit-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-28 15:26:39.000000 csvkit-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.105436 csvkit-1.5.0/csvkit/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    20594 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.109436 csvkit-1.5.0/csvkit/convert/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/convert/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/convert/geojs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/grep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.109436 csvkit-1.5.0/csvkit/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/csvclean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/csvcut.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/csvformat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/csvgrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/csvjoin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11422 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/csvjson.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/csvlook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/csvpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/csvsort.py
--rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/csvsql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/csvstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    14522 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/csvstat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/in2csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-03-28 15:26:39.000000 csvkit-1.5.0/csvkit/utilities/sql2csv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.181437 csvkit-1.5.0/csvkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-03-28 15:27:03.000000 csvkit-1.5.0/csvkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-03-28 15:27:03.000000 csvkit-1.5.0/csvkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 15:27:03.000000 csvkit-1.5.0/csvkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-28 15:27:03.000000 csvkit-1.5.0/csvkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-28 15:27:03.000000 csvkit-1.5.0/csvkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-28 15:27:03.000000 csvkit-1.5.0/csvkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.113436 csvkit-1.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.101436 csvkit-1.5.0/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.113436 csvkit-1.5.0/docs/_build/man/
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/csvclean.1
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/csvcut.1
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/csvformat.1
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/csvgrep.1
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/csvjoin.1
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/csvjson.1
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/csvlook.1
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/csvpy.1
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/csvsort.1
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/csvsql.1
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/csvstack.1
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/csvstat.1
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/in2csv.1
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-03-28 15:26:58.000000 csvkit-1.5.0/docs/_build/man/sql2csv.1
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/common_arguments.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/release.rst
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.117437 csvkit-1.5.0/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/csvclean.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/csvcut.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/csvformat.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/csvgrep.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/csvjoin.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/csvjson.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/csvlook.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/csvpy.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/csvsort.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/csvsql.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/csvstack.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/csvstat.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/in2csv.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/scripts/sql2csv.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/tricks.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.117437 csvkit-1.5.0/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/tutorial/1_getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/tutorial/2_examining_the_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/tutorial/3_power_tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/tutorial/4_going_elsewhere.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-28 15:26:39.000000 csvkit-1.5.0/docs/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.129437 csvkit-1.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/bad.csv
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/bad_skip_lines.csv
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/blanks.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/blanks_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/date_like_number.csv
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/dummy.csv
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/dummy.csv.bz2
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/dummy.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/dummy.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    59904 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/dummy.xls
--rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/dummy.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/dummy2.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/dummy3.csv
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/dummy_col_shuffled.csv
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/dummy_col_shuffled_ragged.csv
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/empty.csv
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/foo1.csv
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/foo2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/iris.csv
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/irismeta.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/join_a.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/join_a_short.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/join_b.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/join_no_header_row.csv
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/join_short.csv
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/mac_newlines.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/no_header_row.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/no_header_row2.csv
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/no_header_row3.csv
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/null_byte.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/optional_quote_characters.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.129437 csvkit-1.5.0/examples/realdata/
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/Datagov_FY10_EDU_recp_by_State.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/FY09_EDU_Recipients_by_State.csv
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/README.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/acs2012_5yr_population.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.177437 csvkit-1.5.0/examples/realdata/census_2000/
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/census_2000/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   472720 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/census_2000/VROUTFSJ.TXt
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/census_2000/census2000_geo_schema.csv
--rw-r--r--   0 runner    (1001) docker     (127)   156931 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/census_2000/determination.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/census_2000/determination_schema.csv
--rw-r--r--   0 runner    (1001) docker     (127) 38031210 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/census_2000/usgeo.upl
--rw-r--r--   0 runner    (1001) docker     (127)   402000 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/census_2000/usgeo_excerpt.upl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.177437 csvkit-1.5.0/examples/realdata/census_2010/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/census_2010/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/census_2010/census2010_geo_schema.csv
--rw-r--r--   0 runner    (1001) docker     (127)   228268 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/census_2010/ilgeo2010_excerpt.csv
--rw-r--r--   0 runner    (1001) docker     (127)   501000 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/census_2010/ilgeo2010_excerpt.pl
--rw-r--r--   0 runner    (1001) docker     (127)   137910 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/event-notification-rpt-lastmonth.txt
--rw-r--r--   0 runner    (1001) docker     (127)   212083 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/ks_1033_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)    65331 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/realdata/ne_1033_data.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/sheets.xls
--rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/sheets.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/sheetsxls_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/sheetsxlsx_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/sniff_limit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/sort_ints_nulls.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test.sql
--rw-r--r--   0 runner    (1001) docker     (127)    18944 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test.xls
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_date_format.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_date_format_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_extra_header.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_geo.csv
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_geojson.csv
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_geojson.json
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_ignore_case.csv
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_latin1.csv
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_latin1.sql
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_literal_order.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_locale.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_locale_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_numeric_date_format.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_precision.csv
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_query.sql
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_skip_lines.csv
--rw-r--r--   0 runner    (1001) docker     (127)    19968 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_skip_lines.xls
--rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_skip_lines.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_utf16_big.csv
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_utf16_little.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_utf8.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/test_utf8_bom.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testdbf.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testdbf_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testfixed
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testfixed_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testfixed_schema.csv
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testfixed_schema_no_inference.csv
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testfixed_skip_lines
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testjson.json
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testjson_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testjson_multiline.json
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testjson_multiline_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testjson_nested.json
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testjson_nested_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testxls_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testxls_unicode_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testxlsx_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testxlsx_noinference_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-28 15:26:39.000000 csvkit-1.5.0/examples/testxlsx_unicode_converted.csv
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-28 15:27:03.185437 csvkit-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-28 15:26:39.000000 csvkit-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.181437 csvkit-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.181437 csvkit-1.5.0/tests/test_convert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_convert/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_convert/test_fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_grep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:27:03.181437 csvkit-1.5.0/tests/test_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/test_csvclean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/test_csvcut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/test_csvformat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/test_csvgrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/test_csvjoin.py
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/test_csvjson.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/test_csvlook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/test_csvsort.py
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/test_csvsql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/test_csvstack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/test_csvstat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/test_in2csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/test_utilities/test_sql2csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-03-28 15:26:39.000000 csvkit-1.5.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.548107 csvkit-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-01 19:52:02.000000 csvkit-2.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26398 2024-05-01 19:52:02.000000 csvkit-2.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-01 19:52:02.000000 csvkit-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-01 19:52:02.000000 csvkit-2.0.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-01 19:52:02.000000 csvkit-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-01 19:52:12.548107 csvkit-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-01 19:52:02.000000 csvkit-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.468107 csvkit-2.0.0/csvkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.468107 csvkit-2.0.0/csvkit/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/convert/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/convert/geojs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/grep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.472107 csvkit-2.0.0/csvkit/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/csvclean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/csvcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/csvformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/csvgrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/csvjoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11422 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/csvjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/csvlook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/csvpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/csvsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12023 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/csvsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/csvstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14522 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/csvstat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/in2csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-01 19:52:02.000000 csvkit-2.0.0/csvkit/utilities/sql2csv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.548107 csvkit-2.0.0/csvkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-01 19:52:12.000000 csvkit-2.0.0/csvkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-01 19:52:12.000000 csvkit-2.0.0/csvkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:52:12.000000 csvkit-2.0.0/csvkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-01 19:52:12.000000 csvkit-2.0.0/csvkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-01 19:52:12.000000 csvkit-2.0.0/csvkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 19:52:12.000000 csvkit-2.0.0/csvkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.472107 csvkit-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.464106 csvkit-2.0.0/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.476107 csvkit-2.0.0/docs/_build/man/
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/csvclean.1
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/csvcut.1
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/csvformat.1
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/csvgrep.1
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/csvjoin.1
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/csvjson.1
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/csvlook.1
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/csvpy.1
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/csvsort.1
+-rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/csvsql.1
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/csvstack.1
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/csvstat.1
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/in2csv.1
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-01 19:52:09.000000 csvkit-2.0.0/docs/_build/man/sql2csv.1
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/common_arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.480106 csvkit-2.0.0/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/csvclean.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/csvcut.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/csvformat.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/csvgrep.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/csvjoin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/csvjson.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/csvlook.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/csvpy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/csvsort.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/csvsql.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/csvstack.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/csvstat.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/in2csv.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/scripts/sql2csv.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/tricks.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.480106 csvkit-2.0.0/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/tutorial/1_getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/tutorial/2_examining_the_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/tutorial/3_power_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/tutorial/4_going_elsewhere.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-01 19:52:02.000000 csvkit-2.0.0/docs/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.492107 csvkit-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/bad.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/bad_skip_lines.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/blanks.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/blanks_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/date_like_number.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/dummy.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/dummy.csv.bz2
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/dummy.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/dummy.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    59904 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/dummy.xls
+-rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/dummy.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/dummy2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/dummy3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/dummy_col_shuffled.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/dummy_col_shuffled_ragged.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/foo1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/foo2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/irismeta.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/join_a.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/join_a_short.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/join_b.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/join_no_header_row.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/join_short.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/mac_newlines.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/no_header_row.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/no_header_row2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/no_header_row3.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/null_byte.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/optional_quote_characters.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.492107 csvkit-2.0.0/examples/realdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/Datagov_FY10_EDU_recp_by_State.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/FY09_EDU_Recipients_by_State.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/README.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/acs2012_5yr_population.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.540107 csvkit-2.0.0/examples/realdata/census_2000/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/census_2000/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   472720 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/census_2000/VROUTFSJ.TXt
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/census_2000/census2000_geo_schema.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   156931 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/census_2000/determination.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/census_2000/determination_schema.csv
+-rw-r--r--   0 runner    (1001) docker     (127) 38031210 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/census_2000/usgeo.upl
+-rw-r--r--   0 runner    (1001) docker     (127)   402000 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/census_2000/usgeo_excerpt.upl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.540107 csvkit-2.0.0/examples/realdata/census_2010/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/census_2010/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/census_2010/census2010_geo_schema.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   228268 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/census_2010/ilgeo2010_excerpt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   501000 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/census_2010/ilgeo2010_excerpt.pl
+-rw-r--r--   0 runner    (1001) docker     (127)   137910 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/event-notification-rpt-lastmonth.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   212083 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/ks_1033_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    65331 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/realdata/ne_1033_data.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/sheets.xls
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/sheets.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/sheetsxls_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/sheetsxlsx_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/sniff_limit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/sort_ints_nulls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    18944 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_date_format.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_date_format_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_empty_columns.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_empty_columns_long_row.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_empty_columns_short_row.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_extra_header.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_geo.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_geojson.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_geojson.json
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_header_newline.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_ignore_case.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_join_short_rows.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_latin1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_latin1.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_literal_order.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_locale.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_locale_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_numeric_date_format.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_precision.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_query.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_skip_lines.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    19968 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_skip_lines.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_skip_lines.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_utf16_big.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_utf16_little.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_utf8.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/test_utf8_bom.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testdbf.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testdbf_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testfixed
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testfixed_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testfixed_schema.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testfixed_schema_no_inference.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testfixed_skip_lines
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testjson.json
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testjson_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testjson_multiline.json
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testjson_multiline_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testjson_nested.json
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testjson_nested_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testxls_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testxls_unicode_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testxlsx_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testxlsx_noinference_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 19:52:02.000000 csvkit-2.0.0/examples/testxlsx_unicode_converted.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-01 19:52:12.548107 csvkit-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-01 19:52:02.000000 csvkit-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.544107 csvkit-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.544107 csvkit-2.0.0/tests/test_convert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_convert/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_convert/test_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_grep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:12.548107 csvkit-2.0.0/tests/test_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/test_csvclean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/test_csvcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/test_csvformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/test_csvgrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/test_csvjoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24984 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/test_csvjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/test_csvlook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/test_csvsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/test_csvsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/test_csvstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/test_csvstat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/test_in2csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/test_utilities/test_sql2csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-01 19:52:02.000000 csvkit-2.0.0/tests/utils.py
```

### Comparing `csvkit-1.5.0/AUTHORS.rst` & `csvkit-2.0.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/CHANGELOG.rst` & `csvkit-2.0.0/CHANGELOG.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,431 +1,475 @@
+2.0.0 - May 1, 2024
+-------------------
+
+This is the first major release since December 27, 2016. Thank you to all :ref:`contributors<authors>`, including 44 new contributors since 1.0.0!
+
+Want to use csvkit programmatically? Check out `agate <https://agate.readthedocs.io/en/latest/>`__, used internally by csvkit.
+
+**BACKWARDS-INCOMPATIBLE CHANGES:**
+
+-  :doc:`/scripts/csvclean` now writes its output to standard output and its errors to standard error, instead of to ``basename_out.csv`` and ``basename_err.csv`` files. Consequently:
+
+   -  The :code:`--dry-run` option is removed. The :code:`--dry-run` option changed error output from the CSV format used in ``basename_err.csv`` files to a prosaic format like ``Line 1: Expected 2 columns, found 3 columns``.
+   -  Summary information like ``No errors.``, ``42 errors logged to basename_err.csv`` and ``42 rows were joined/reduced to 24 rows after eliminating expected internal line breaks.`` is not written.
+
+-  :doc:`/scripts/csvclean` no longer reports or fixes errors by default; it errors if no checks or fixes are enabled. Opt in to the original behavior using the :code:`--length-mismatch` and :code:`--join-short-rows` options. See new options below.
+-  :doc:`/scripts/csvclean` no longer omits rows with errors from the output. Opt in to the original behavior using the :code:`--omit-error-rows` option.
+-  :doc:`/scripts/csvclean` joins short rows using a newline by default, instead of a space. Restore the original behavior using the :code:`--separator " "` option.
+
+In brief, to restore the original behavior for :doc:`/scripts/csvclean`:
+
+.. code-block:: bash
+
+   csvclean --length-mismatch --omit-error-rows --join-short-rows --separator " " myfile.csv
+
+Other changes:
+
+-  feat: :doc:`/scripts/csvclean` adds the options:
+
+   -  :code:`--length-mismatch`, to error on data rows that are shorter or longer than the header row
+   -  :code:`--empty-columns`, to error on empty columns
+   -  :code:`--enable-all-checks`, to enable all error reporting
+   -  :code:`--omit-error-rows`, to omit data rows that contain errors, from standard output
+   -  :code:`--label LABEL`, to add a "label" column to standard error
+   -  :code:`--header-normalize-space`, to strip leading and trailing whitespace and replace sequences of whitespace characters by a single space in the header
+   -  :code:`--join-short-rows`, to merge short rows into a single row
+   -  :code:`--separator SEPARATOR`, to change the string with which to join short rows (default is newline)
+   -  :code:`--fill-short-rows`, to fill short rows with the missing cells
+   -  :code:`--fillvalue FILLVALUE`, to change the value with which to fill short rows (default is none)
+
+-  feat: The :code:`--quoting` option accepts 4 (`csv.QUOTE_STRINGS <https://docs.python.org/3/library/csv.html#csv.QUOTE_STRINGS>`__) and 5 (`csv.QUOTE_NOTNULL <https://docs.python.org/3/library/csv.html#csv.QUOTE_NOTNULL>`__) on Python 3.12.
+-  feat: :doc:`/scripts/csvformat`: The :code:`--out-quoting` option accepts 4 (`csv.QUOTE_STRINGS <https://docs.python.org/3/library/csv.html#csv.QUOTE_STRINGS>`__) and 5 (`csv.QUOTE_NOTNULL <https://docs.python.org/3/library/csv.html#csv.QUOTE_NOTNULL>`__) on Python 3.12.
+-  fix: :doc:`/scripts/csvformat`: The :code:`--out-quoting` option works with 2 (`csv.QUOTE_NONUMERIC <https://docs.python.org/3/library/csv.html#csv.QUOTE_NOTNUMERIC>`__). Use the :code:`--locale` option to set the locale of any formatted numbers.
+-  fix: :doc:`/scripts/csvclean`: The :code:`--join-short-rows` option no longer reports length mismatch errors that were fixed.
+
 1.5.0 - March 28, 2024
 ----------------------
 
-* feat: Add support for Zstandard files with the ``.zst`` extension, if the ``zstandard`` package is installed.
-* feat: :doc:`/scripts/csvformat` adds a :code:`--out-asv` (:code:`--A`) option to use the ASCII unit separator and record separator.
-* feat: :doc:`/scripts/csvsort` adds a :code:`--ignore-case` (:code:`--i`) option to perform case-independent sorting.
+-  feat: Add support for Zstandard files with the ``.zst`` extension, if the ``zstandard`` package is installed.
+-  feat: :doc:`/scripts/csvformat` adds a :code:`--out-asv` (:code:`--A`) option to use the ASCII unit separator and record separator.
+-  feat: :doc:`/scripts/csvsort` adds a :code:`--ignore-case` (:code:`--i`) option to perform case-independent sorting.
 
 1.4.0 - February 13, 2024
 -------------------------
 
-* feat: :doc:`/scripts/csvpy` adds the options:
+-  feat: :doc:`/scripts/csvpy` adds the options:
 
-   * :code:`--no-number-ellipsis`, to disable the ellipsis (``…``) if max precision is exceeded, for example, when using ``table.print_table()``
-   * :code:`--sniff-limit``
-   * :code:`--no-inference``
-
-* feat: :doc:`/scripts/csvpy` removes the ``--linenumbers`` and ``--zero`` output options, which had no effect.
-* feat: :doc:`/scripts/in2csv` adds a :code:`--reset-dimensions` option to `recalculate <https://openpyxl.readthedocs.io/en/stable/optimized.html#worksheet-dimensions>`_ the dimensions of an XLSX file, instead of trusting the file's metadata. csvkit's dependency `agate-excel <https://agate-excel.readthedocs.io/en/latest/>`_ 0.4.0 automatically recalculates the dimensions if the file's metadata expresses dimensions of "A1:A1" (a single cell).
-* fix: :doc:`/scripts/csvlook` only reads up to :code:`--max-rows` rows instead of the entire file.
-* fix: :doc:`/scripts/csvpy` supports the existing input options:
-
-   * :code:`--locale`
-   * :code:`--blanks`
-   * :code:`--null-value`
-   * :code:`--date-format`
-   * :code:`--datetime-format`
-   * :code:`--skip-lines`
-
-* fix: :doc:`/scripts/csvpy`: :code:`--maxfieldsize` no longer errors when :code:`--dict` is set.
-* fix: :doc:`/scripts/csvstack`: :code:`--maxfieldsize` no longer errors when :code:`--no-header-row` isn't set.
-* fix: :doc:`/scripts/in2csv`: :code:`--write-sheets` no longer errors when standard input is an XLS or XLSX file.
-* Update minimum agate version to 1.6.3.
+   -  :code:`--no-number-ellipsis`, to disable the ellipsis (``…``) if max precision is exceeded, for example, when using ``table.print_table()``
+   -  :code:`--sniff-limit``
+   -  :code:`--no-inference``
+
+-  feat: :doc:`/scripts/csvpy` removes the :code:`--linenumbers` and :code:`--zero` output options, which had no effect.
+-  feat: :doc:`/scripts/in2csv` adds a :code:`--reset-dimensions` option to `recalculate <https://openpyxl.readthedocs.io/en/stable/optimized.html#worksheet-dimensions>`_ the dimensions of an XLSX file, instead of trusting the file's metadata. csvkit's dependency `agate-excel <https://agate-excel.readthedocs.io/en/latest/>`_ 0.4.0 automatically recalculates the dimensions if the file's metadata expresses dimensions of "A1:A1" (a single cell).
+-  fix: :doc:`/scripts/csvlook` only reads up to :code:`--max-rows` rows instead of the entire file.
+-  fix: :doc:`/scripts/csvpy` supports the existing input options:
+
+   -  :code:`--locale`
+   -  :code:`--blanks`
+   -  :code:`--null-value`
+   -  :code:`--date-format`
+   -  :code:`--datetime-format`
+   -  :code:`--skip-lines`
+
+-  fix: :doc:`/scripts/csvpy`: :code:`--maxfieldsize` no longer errors when :code:`--dict` is set.
+-  fix: :doc:`/scripts/csvstack`: :code:`--maxfieldsize` no longer errors when :code:`--no-header-row` isn't set.
+-  fix: :doc:`/scripts/in2csv`: :code:`--write-sheets` no longer errors when standard input is an XLS or XLSX file.
+-  Update minimum agate version to 1.6.3.
 
 1.3.0 - October 18, 2023
 ------------------------
 
-* :doc:`/scripts/csvformat` adds a :code:`--skip-header` (:code:`-E`) option to not output a header row.
-* :doc:`/scripts/csvlook` adds a :code:`--max-precision` option to set the maximum number of decimal places to display.
-* :doc:`/scripts/csvlook` adds a :code:`--no-number-ellipsis` option to disable the ellipsis (``…``) if :code:`--max-precision` is exceeded. (Requires agate 1.9.0 or greater.)
-* :doc:`/scripts/csvstat` supports the :code:`--no-inference` (:code:`-I`), :code:`--locale` (:code:`-L`), :code:`--blanks`, :code:`--date-format` and :code:`datetime-format` options.
-* :doc:`/scripts/csvstat` reports a "Non-null values" statistic (or a :code:`nonnulls` column when :code:`--csv` is set).
-* :doc:`/scripts/csvstat` adds a :code:`--non-nulls` option to only output counts of non-null values.
-* :doc:`/scripts/csvstat` reports a "Most decimal places" statistic (or a :code:`maxprecision` column when :code:`--csv` is set).
-* :doc:`/scripts/csvstat` adds a :code:`--max-precision` option to only output the most decimal places.
-* :doc:`/scripts/csvstat` adds a :code:`--json` option to output results as JSON text.
-* :doc:`/scripts/csvstat` adds an :code:`--indent` option to indent the JSON text when :code:`--json` is set.
-* :doc:`/scripts/in2csv` adds a :code:`--use-sheet-names` option to use the sheet names as file names when :code:`--write-sheets` is set.
-* feat: Add a :code:`--null-value` option to commands with the :code:`--blanks` option, to convert additional values to NULL.
-* fix: Reconfigure the encoding of standard input according to the :code:`--encoding` option, which defaults to ``utf-8-sig``. Affected users no longer need to set the ``PYTHONIOENCODING`` environment variable.
-* fix: Prompt the user if additional input is expected (i.e. if no input file or piped data is provided) in :doc:`/scripts/csvjoin`, :doc:`/scripts/csvsql` and :doc:`/scripts/csvstack`.
-* fix: No longer errors if a NUL byte occurs in an input file.
-* Add Python 3.12 support.
+-  :doc:`/scripts/csvformat` adds a :code:`--skip-header` (:code:`-E`) option to not output a header row.
+-  :doc:`/scripts/csvlook` adds a :code:`--max-precision` option to set the maximum number of decimal places to display.
+-  :doc:`/scripts/csvlook` adds a :code:`--no-number-ellipsis` option to disable the ellipsis (``…``) if :code:`--max-precision` is exceeded. (Requires agate 1.9.0 or greater.)
+-  :doc:`/scripts/csvstat` supports the :code:`--no-inference` (:code:`-I`), :code:`--locale` (:code:`-L`), :code:`--blanks`, :code:`--date-format` and :code:`datetime-format` options.
+-  :doc:`/scripts/csvstat` reports a "Non-null values" statistic (or a :code:`nonnulls` column when :code:`--csv` is set).
+-  :doc:`/scripts/csvstat` adds a :code:`--non-nulls` option to only output counts of non-null values.
+-  :doc:`/scripts/csvstat` reports a "Most decimal places" statistic (or a :code:`maxprecision` column when :code:`--csv` is set).
+-  :doc:`/scripts/csvstat` adds a :code:`--max-precision` option to only output the most decimal places.
+-  :doc:`/scripts/csvstat` adds a :code:`--json` option to output results as JSON text.
+-  :doc:`/scripts/csvstat` adds an :code:`--indent` option to indent the JSON text when :code:`--json` is set.
+-  :doc:`/scripts/in2csv` adds a :code:`--use-sheet-names` option to use the sheet names as file names when :code:`--write-sheets` is set.
+-  feat: Add a :code:`--null-value` option to commands with the :code:`--blanks` option, to convert additional values to NULL.
+-  fix: Reconfigure the encoding of standard input according to the :code:`--encoding` option, which defaults to ``utf-8-sig``. Affected users no longer need to set the ``PYTHONIOENCODING`` environment variable.
+-  fix: Prompt the user if additional input is expected (i.e. if no input file or piped data is provided) in :doc:`/scripts/csvjoin`, :doc:`/scripts/csvsql` and :doc:`/scripts/csvstack`.
+-  fix: No longer errors if a NUL byte occurs in an input file.
+-  Add Python 3.12 support.
 
 1.2.0 - October 4, 2023
 -----------------------
 
-* fix: :doc:`/scripts/csvjoin` uses the correct columns when performing a ``--right`` join.
-* Add SQLAlchemy 2 support.
-* Drop Python 3.7 support (end-of-life was June 5, 2023).
+-  fix: :doc:`/scripts/csvjoin` uses the correct columns when performing a :code:`--right` join.
+-  Add SQLAlchemy 2 support.
+-  Drop Python 3.7 support (end-of-life was June 5, 2023).
 
 1.1.1 - February 22, 2023
 -------------------------
 
-* feat: :doc:`/scripts/csvstack` handles files with columns in different orders or with different names.
+-  feat: :doc:`/scripts/csvstack` handles files with columns in different orders or with different names.
 
 1.1.0 - January 3, 2023
 -----------------------
 
-* feat: :doc:`/scripts/csvsql` accepts multiple :code:`--query` command-line arguments.
-* feat: :doc:`/scripts/csvstat` adds :code:`--no-grouping-separator` and :code:`--decimal-format` options.
-* Add Python 3.11 support.
-* Drop Python 3.6 support (end-of-life was December 23, 2021).
-* Drop Python 2.7 support (end-of-life was January 1, 2020).
+-  feat: :doc:`/scripts/csvsql` accepts multiple :code:`--query` command-line arguments.
+-  feat: :doc:`/scripts/csvstat` adds :code:`--no-grouping-separator` and :code:`--decimal-format` options.
+-  Add Python 3.11 support.
+-  Drop Python 3.6 support (end-of-life was December 23, 2021).
+-  Drop Python 2.7 support (end-of-life was January 1, 2020).
 
 1.0.7 - March 6, 2022
 ---------------------
 
-* fix: :doc:`/scripts/csvcut` extracts the correct columns when :code:`--line-numbers` is set.
-* fix: Restore Python 2.7 support in edge cases.
-* feat: Use 1024 byte sniff-limit by default across csvkit. Improve csvstat performance up to 10x.
-* feat: Add support for ``.xz`` (LZMA) compressed input files.
-* Add Python 3.10 support.
-* Drop Python 3.5 support (end-of-life was September 30, 2020).
+-  fix: :doc:`/scripts/csvcut` extracts the correct columns when :code:`--line-numbers` is set.
+-  fix: Restore Python 2.7 support in edge cases.
+-  feat: Use 1024 byte sniff-limit by default across csvkit. Improve csvstat performance up to 10x.
+-  feat: Add support for ``.xz`` (LZMA) compressed input files.
+-  Add Python 3.10 support.
+-  Drop Python 3.5 support (end-of-life was September 30, 2020).
 
 1.0.6 - July 13, 2021
 ---------------------
 
 Changes:
 
-* :doc:`/scripts/csvstat` no longer prints "Row count: " when :code:`--count` is set.
-* :doc:`/scripts/csvclean`, :doc:`/scripts/csvcut`, :doc:`/scripts/csvgrep` no longer error if standard input is null.
+-  :doc:`/scripts/csvstat` no longer prints "Row count: " when :code:`--count` is set.
+-  :doc:`/scripts/csvclean`, :doc:`/scripts/csvcut`, :doc:`/scripts/csvgrep` no longer error if standard input is null.
 
 Fixes:
 
-* :doc:`/scripts/csvformat` creates default headers when :code:`--no-header-row` is set, as documented.
-* :doc:`/scripts/csvstack` no longer errors when :code:`--no-header-row` is combined with :code:`--groups` or :code:`--filenames`.
+-  :doc:`/scripts/csvformat` creates default headers when :code:`--no-header-row` is set, as documented.
+-  :doc:`/scripts/csvstack` no longer errors when :code:`--no-header-row` is combined with :code:`--groups` or :code:`--filenames`.
 
 1.0.5 - March 2, 2020
 ---------------------
 
 Changes:
 
-* Drop Python 3.4 support (end-of-life was March 18, 2019).
+-  Drop Python 3.4 support (end-of-life was March 18, 2019).
 
 Improvements:
 
-* Output error message for memory error even if not :code:`--verbose`.
+-  Output error message for memory error even if not :code:`--verbose`.
 
 Fixes:
 
-* Fix regression in 1.0.4, which caused numbers like ``4.5`` to be parsed as dates.
-* :doc:`/scripts/in2csv` Fix error reporting if :code:`--names` used with non-Excel file.
+-  Fix regression in 1.0.4, which caused numbers like ``4.5`` to be parsed as dates.
+-  :doc:`/scripts/in2csv` Fix error reporting if :code:`--names` used with non-Excel file.
 
 1.0.4 - March 16, 2019
 ----------------------
 
 Changes:
 
-* Drop Python 3.3 support (end-of-life was September 29, 2017).
+-  Drop Python 3.3 support (end-of-life was September 29, 2017).
 
 Improvements:
 
-* :doc:`/scripts/csvsql` adds a :code:`--chunk-size` option to set the chunk size when batch inserting into a table.
-* csvkit is tested against Python 3.7.
+-  :doc:`/scripts/csvsql` adds a :code:`--chunk-size` option to set the chunk size when batch inserting into a table.
+-  csvkit is tested against Python 3.7.
 
 Fixes:
 
-* :code:`--names` works with :code:`--skip-lines`.
-* Dates and datetimes without punctuation can be parsed with :code:`--date-format` and :code:`datetime-format`.
-* Error messages about column indices use 1-based numbering unless :code:`--zero` is set.
-* :doc:`/scripts/csvcut` no longer errors on :code:`--delete-empty-rows` with short rows.
-* :doc:`/scripts/csvjoin` no longer errors if given a single file.
-* :doc:`/scripts/csvsql` supports UPDATE commands.
-* :doc:`/scripts/csvstat` no longer errors on non-finite numbers.
-* :doc:`/scripts/csvstat` respects all command-line arguments when :code:`--count` is set.
-* :doc:`/scripts/in2csv` CSV-to-CSV conversion respects :code:`--linenumbers` when buffering.
-* :doc:`/scripts/in2csv` writes XLS sheets without encoding errors in Python 2.
+-  :code:`--names` works with :code:`--skip-lines`.
+-  Dates and datetimes without punctuation can be parsed with :code:`--date-format` and :code:`datetime-format`.
+-  Error messages about column indices use 1-based numbering unless :code:`--zero` is set.
+-  :doc:`/scripts/csvcut` no longer errors on :code:`--delete-empty-rows` with short rows.
+-  :doc:`/scripts/csvjoin` no longer errors if given a single file.
+-  :doc:`/scripts/csvsql` supports UPDATE commands.
+-  :doc:`/scripts/csvstat` no longer errors on non-finite numbers.
+-  :doc:`/scripts/csvstat` respects all command-line arguments when :code:`--count` is set.
+-  :doc:`/scripts/in2csv` CSV-to-CSV conversion respects :code:`--linenumbers` when buffering.
+-  :doc:`/scripts/in2csv` writes XLS sheets without encoding errors in Python 2.
 
 1.0.3 - March 11, 2018
 ----------------------
 
 Improvements:
 
-* :doc:`/scripts/csvgrep` adds a :code:`--any-match` (:code:`-a`) flag to select rows where any column matches instead of all columns.
-* :doc:`/scripts/csvjson` no longer emits a property if its value is null.
-* :doc:`/scripts/csvjson` adds :code:`--type` and :code:`--geometry` options to emit non-Point GeoJSON features.
-* :doc:`/scripts/csvjson` adds a :code:`--no-bbox` option to disable the calculation of a bounding box.
-* :doc:`/scripts/csvjson` supports :code:`--stream` for newline-delimited GeoJSON.
-* :doc:`/scripts/csvsql` adds a :code:`--unique-constraint` option to list names of columns to include in a UNIQUE constraint.
-* :doc:`/scripts/csvsql` adds :code:`--before-insert` and :code:`--after-insert` options to run commands before and after the INSERT command.
-* :doc:`/scripts/csvpy` reports an error message if input is provided via STDIN.
-* :doc:`/scripts/in2csv` adds a :code:`--encoding-xls` option to specify the encoding of the input XLS file.
-* :doc:`/scripts/in2csv` supports :code:`--no-header-row` on XLS and XLSX files.
-* Suppress agate warning about column names not specified when using :code:`--no-header-row`.
-* Prompt the user if additional input is expected (i.e. if no input file or piped data is provided).
-* Update to `agate-excel 0.2.2 <https://agate-excel.readthedocs.io/en/latest/#changelog>`_, `agate-sql 0.5.3 <https://agate-sql.readthedocs.io/en/latest/#changelog>`_.
+-  :doc:`/scripts/csvgrep` adds a :code:`--any-match` (:code:`-a`) flag to select rows where any column matches instead of all columns.
+-  :doc:`/scripts/csvjson` no longer emits a property if its value is null.
+-  :doc:`/scripts/csvjson` adds :code:`--type` and :code:`--geometry` options to emit non-Point GeoJSON features.
+-  :doc:`/scripts/csvjson` adds a :code:`--no-bbox` option to disable the calculation of a bounding box.
+-  :doc:`/scripts/csvjson` supports :code:`--stream` for newline-delimited GeoJSON.
+-  :doc:`/scripts/csvsql` adds a :code:`--unique-constraint` option to list names of columns to include in a UNIQUE constraint.
+-  :doc:`/scripts/csvsql` adds :code:`--before-insert` and :code:`--after-insert` options to run commands before and after the INSERT command.
+-  :doc:`/scripts/csvpy` reports an error message if input is provided via STDIN.
+-  :doc:`/scripts/in2csv` adds a :code:`--encoding-xls` option to specify the encoding of the input XLS file.
+-  :doc:`/scripts/in2csv` supports :code:`--no-header-row` on XLS and XLSX files.
+-  Suppress agate warning about column names not specified when using :code:`--no-header-row`.
+-  Prompt the user if additional input is expected (i.e. if no input file or piped data is provided).
+-  Update to `agate-excel 0.2.2 <https://agate-excel.readthedocs.io/en/latest/#changelog>`_, `agate-sql 0.5.3 <https://agate-sql.readthedocs.io/en/latest/#changelog>`_.
 
 Fixes:
 
-* :doc:`/scripts/csvgrep` accepts utf-8 arguments to the :code:`--match` and :code:`--regex` options in Python 2.
-* :doc:`/scripts/csvjson` streams input and output only if :code:`--snifflimit` is :code:`0`.
-* :doc:`/scripts/csvsql` sets a DECIMAL's precision and scale and a VARCHAR's length to avoid dialect-specific errors.
-* :doc:`/scripts/csvstack` no longer opens all files at once.
-* :doc:`/scripts/in2csv` respects :code:`--no-header-row` when :code:`--no-inference` is set.
-* :doc:`/scripts/in2csv` CSV-to-CSV conversion streams input and output only if :code:`--snifflimit` is :code:`0`.
-* :doc:`/scripts/in2csv` supports GeoJSON files with: ``geometry`` set to ``null``, missing Point ``coordinates``, altitude coordinate values.
+-  :doc:`/scripts/csvgrep` accepts utf-8 arguments to the :code:`--match` and :code:`--regex` options in Python 2.
+-  :doc:`/scripts/csvjson` streams input and output only if :code:`--snifflimit` is :code:`0`.
+-  :doc:`/scripts/csvsql` sets a DECIMAL's precision and scale and a VARCHAR's length to avoid dialect-specific errors.
+-  :doc:`/scripts/csvstack` no longer opens all files at once.
+-  :doc:`/scripts/in2csv` respects :code:`--no-header-row` when :code:`--no-inference` is set.
+-  :doc:`/scripts/in2csv` CSV-to-CSV conversion streams input and output only if :code:`--snifflimit` is :code:`0`.
+-  :doc:`/scripts/in2csv` supports GeoJSON files with: ``geometry`` set to ``null``, missing Point ``coordinates``, altitude coordinate values.
 
 csvkit is no longer tested on PyPy.
 
 1.0.2 - April 28, 2017
 ----------------------
 
 Improvements:
 
-* Add a :code:`--version` flag.
-* Add a :code:`--skip-lines` option to skip initial lines (e.g. comments, copyright notices, empty rows).
-* Add a :code:`--locale` option to set the locale of any formatted numbers.
-* Add a :code:`--date-format` option to set a strptime date format string.
-* Add a :code:`--datetime-format` option to set a strptime datetime format string.
-* Make :code:`--blanks` a common argument across all tools.
-* :code:`-I` is the short option for :code:`--no-inference`.
-* :doc:`/scripts/csvclean`, :doc:`/scripts/csvformat`, :doc:`/scripts/csvjson`, :doc:`/scripts/csvpy` support :code:`--no-header-row`.
-* :doc:`/scripts/csvclean` is faster and no longer requires exponential time in the worst case.
-* :doc:`/scripts/csvformat` supports :code:`--linenumbers` and `--zero` (no-op).
-* :doc:`/scripts/csvjoin` supports :code:`--snifflimit` and :code:`--no-inference`.
-* :doc:`/scripts/csvpy` supports :code:`--linenumbers` (no-op) and :code:`--zero` (no-op).
-* :doc:`/scripts/csvsql` adds a :code:`--prefix` option to add expressions like OR IGNORE or OR REPLACE following the INSERT keyword.
-* :doc:`/scripts/csvsql` adds a :code:`--overwrite` flag to drop any existing table with the same name before creating.
-* :doc:`/scripts/csvsql` accepts a file name for the :code:`--query` option.
-* :doc:`/scripts/csvsql` supports :code:`--linenumbers` (no-op).
-* :doc:`/scripts/csvsql` adds a :code:`--create-if-not-exists` flag to not abort if the table already exists.
-* :doc:`/scripts/csvstat` adds a :code:`--freq-count` option to set the maximum number of frequent values to display.
-* :doc:`/scripts/csvstat` supports :code:`--linenumbers` (no-op).
-* :doc:`/scripts/in2csv` adds a :code:`--names` flag to print Excel sheet names.
-* :doc:`/scripts/in2csv` adds a :code:`--write-sheets` option to write the named Excel sheets to files.
-* :doc:`/scripts/sql2csv` adds an :code:`--encoding` option to specify the encoding of the input query file.
+-  Add a :code:`--version` flag.
+-  Add a :code:`--skip-lines` option to skip initial lines (e.g. comments, copyright notices, empty rows).
+-  Add a :code:`--locale` option to set the locale of any formatted numbers.
+-  Add a :code:`--date-format` option to set a strptime date format string.
+-  Add a :code:`--datetime-format` option to set a strptime datetime format string.
+-  Make :code:`--blanks` a common argument across all tools.
+-  :code:`-I` is the short option for :code:`--no-inference`.
+-  :doc:`/scripts/csvclean`, :doc:`/scripts/csvformat`, :doc:`/scripts/csvjson`, :doc:`/scripts/csvpy` support :code:`--no-header-row`.
+-  :doc:`/scripts/csvclean` is faster and no longer requires exponential time in the worst case.
+-  :doc:`/scripts/csvformat` supports :code:`--linenumbers` and `--zero` (no-op).
+-  :doc:`/scripts/csvjoin` supports :code:`--snifflimit` and :code:`--no-inference`.
+-  :doc:`/scripts/csvpy` supports :code:`--linenumbers` (no-op) and :code:`--zero` (no-op).
+-  :doc:`/scripts/csvsql` adds a :code:`--prefix` option to add expressions like OR IGNORE or OR REPLACE following the INSERT keyword.
+-  :doc:`/scripts/csvsql` adds a :code:`--overwrite` flag to drop any existing table with the same name before creating.
+-  :doc:`/scripts/csvsql` accepts a file name for the :code:`--query` option.
+-  :doc:`/scripts/csvsql` supports :code:`--linenumbers` (no-op).
+-  :doc:`/scripts/csvsql` adds a :code:`--create-if-not-exists` flag to not abort if the table already exists.
+-  :doc:`/scripts/csvstat` adds a :code:`--freq-count` option to set the maximum number of frequent values to display.
+-  :doc:`/scripts/csvstat` supports :code:`--linenumbers` (no-op).
+-  :doc:`/scripts/in2csv` adds a :code:`--names` flag to print Excel sheet names.
+-  :doc:`/scripts/in2csv` adds a :code:`--write-sheets` option to write the named Excel sheets to files.
+-  :doc:`/scripts/sql2csv` adds an :code:`--encoding` option to specify the encoding of the input query file.
 
 Fixes:
 
-* :doc:`/scripts/csvgrep` no longer ignores common arguments if :code:`--linenumbers` is set.
-* :doc:`/scripts/csvjson` supports Decimal.
-* :doc:`/scripts/csvpy` again supports IPython.
-* :doc:`/scripts/csvsql` restores support for :code:`--no-constraints` and :code:`--db-schema`.
-* :doc:`/scripts/csvstat` no longer crashes when :code:`--freq` is set.
-* :doc:`/scripts/in2csv` restores support for :code:`--no-inference` for Excel files.
-* :doc:`/scripts/in2csv` restores support for converting Excel files from standard input.
-* :doc:`/scripts/in2csv` accepts utf-8 arguments to the :code:`--sheet` option in Python 2.
+-  :doc:`/scripts/csvgrep` no longer ignores common arguments if :code:`--linenumbers` is set.
+-  :doc:`/scripts/csvjson` supports Decimal.
+-  :doc:`/scripts/csvpy` again supports IPython.
+-  :doc:`/scripts/csvsql` restores support for :code:`--no-constraints` and :code:`--db-schema`.
+-  :doc:`/scripts/csvstat` no longer crashes when :code:`--freq` is set.
+-  :doc:`/scripts/in2csv` restores support for :code:`--no-inference` for Excel files.
+-  :doc:`/scripts/in2csv` restores support for converting Excel files from standard input.
+-  :doc:`/scripts/in2csv` accepts utf-8 arguments to the :code:`--sheet` option in Python 2.
 
 1.0.1 - December 29, 2016
 -------------------------
 
 This is a minor release which fixes several bugs reported in the :code:`1.0.0` release earlier this week. It also significantly improves the output of :doc:`/scripts/csvstat` and adds a :code:`--csv` output option to that command.
 
-* :doc:`/scripts/csvstat` no longer crashes when a :code:`Number` column has :code:`None` as a frequent value. (#738)
-* :doc:`/scripts/csvlook` documents that output tables are Markdown-compatible. (#734)
-* :doc:`/scripts/csvstat` adds a :code:`--csv` flag for tabular output. (#584)
-* :doc:`/scripts/csvstat` output is easier to read. (#714)
-* :doc:`/scripts/csvpy` has a better description when using the :code:`--agate` flag. (#729)
-* Fix a Python 2.6 bug preventing :doc:`/scripts/csvjson` from parsing utf-8 files. (#732)
-* Update required version of unittest to latest. (#727)
+-  :doc:`/scripts/csvstat` no longer crashes when a :code:`Number` column has :code:`None` as a frequent value. (#738)
+-  :doc:`/scripts/csvlook` documents that output tables are Markdown-compatible. (#734)
+-  :doc:`/scripts/csvstat` adds a :code:`--csv` flag for tabular output. (#584)
+-  :doc:`/scripts/csvstat` output is easier to read. (#714)
+-  :doc:`/scripts/csvpy` has a better description when using the :code:`--agate` flag. (#729)
+-  Fix a Python 2.6 bug preventing :doc:`/scripts/csvjson` from parsing utf-8 files. (#732)
+-  Update required version of unittest to latest. (#727)
 
 1.0.0 - December 27, 2016
 -------------------------
 
 This is the first major release of csvkit in a very long time. The entire backend has been rewritten to leverage the `agate <https://agate.rtfd.io>`_ data analysis library, which was itself inspired by csvkit. The new backend provides better type detection accuracy, as well as some new features.
 
 Because of the long and complex cycle behind this release, the list of changes should not be considered exhaustive. In particular, the output format of some tools may have changed in small ways. Any existing data pipelines using csvkit should be tested as part of the upgrade.
 
 Much of the credit for this release goes to `James McKinney <https://github.com/jpmckinney>`_, who has almost single-handedly kept the csvkit fire burning for a year. Thanks, James!
 
 Backwards-incompatible changes:
 
-* :doc:`/scripts/csvjoin` renames duplicate columns with integer suffixes to prevent collisions in output.
-* :doc:`/scripts/csvsql` generates ``DateTime`` columns instead of ``Time`` columns.
-* :doc:`/scripts/csvsql` generates ``Decimal`` columns instead of ``Integer``, ``BigInteger``, and ``Float`` columns.
-* :doc:`/scripts/csvsql` no longer generates max-length constraints for text columns.
-* The ``--doublequote`` long flag is gone, and the ``-b`` short flag is an alias for ``--no-doublequote``.
-* When using the ``--columns`` or ``--not-columns`` options, you must not have spaces around the comma-separated values, unless the column names contain spaces.
-* When sorting, null values are greater than other values instead of less than.
-* ``CSVKitReader``, ``CSVKitWriter``, ``CSVKitDictReader``, and ``CSVKitDictWriter`` have been removed. Use ``agate.csv.reader``, ``agate.csv.writer``, ``agate.csv.DictReader`` and ``agate.csv.DictWriter``.
-* Drop Python 2.6 support (end-of-life was October 29, 2013).
-* Drop support for older versions of PyPy.
-* If ``--no-header-row`` is set, the output has column names ``a``, ``b``, ``c``, etc. instead of ``column1``, ``column2``, ``column3``, etc.
-* csvlook renders a simpler, markdown-compatible table.
+-  :doc:`/scripts/csvjoin` renames duplicate columns with integer suffixes to prevent collisions in output.
+-  :doc:`/scripts/csvsql` generates ``DateTime`` columns instead of ``Time`` columns.
+-  :doc:`/scripts/csvsql` generates ``Decimal`` columns instead of ``Integer``, ``BigInteger``, and ``Float`` columns.
+-  :doc:`/scripts/csvsql` no longer generates max-length constraints for text columns.
+-  The ``--doublequote`` long flag is gone, and the ``-b`` short flag is an alias for ``--no-doublequote``.
+-  When using the ``--columns`` or ``--not-columns`` options, you must not have spaces around the comma-separated values, unless the column names contain spaces.
+-  When sorting, null values are greater than other values instead of less than.
+-  ``CSVKitReader``, ``CSVKitWriter``, ``CSVKitDictReader``, and ``CSVKitDictWriter`` have been removed. Use ``agate.csv.reader``, ``agate.csv.writer``, ``agate.csv.DictReader`` and ``agate.csv.DictWriter``.
+-  Drop Python 2.6 support (end-of-life was October 29, 2013).
+-  Drop support for older versions of PyPy.
+-  If ``--no-header-row`` is set, the output has column names ``a``, ``b``, ``c``, etc. instead of ``column1``, ``column2``, ``column3``, etc.
+-  csvlook renders a simpler, markdown-compatible table.
 
 Improvements:
 
-* csvkit is tested against Python 3.6. (#702)
-* ``import csvkit as csv`` defers to agate readers/writers.
-* :doc:`/scripts/csvgrep` supports ``--no-header-row``.
-* :doc:`/scripts/csvjoin` supports ``--no-header-row``.
-* :doc:`/scripts/csvjson` streams input and output if the ``--stream`` and ``--no-inference`` flags are set.
-* :doc:`/scripts/csvjson` supports ``--snifflimit`` and ``--no-inference``.
-* :doc:`/scripts/csvlook` adds ``--max-rows``, ``--max-columns`` and ``--max-column-width`` options.
-* :doc:`/scripts/csvlook` supports ``--snifflimit`` and ``--no-inference``.
-* :doc:`/scripts/csvpy` supports ``--agate`` to read a CSV file into an agate table.
-* ``csvsql`` supports custom `SQLAlchemy dialects <https://docs.sqlalchemy.org/en/latest/dialects/>`_.
-* :doc:`/scripts/csvstat` supports ``--names``.
-* :doc:`/scripts/in2csv` CSV-to-CSV conversion streams input and output if the ``--no-inference`` flag is set.
-* :doc:`/scripts/in2csv` CSV-to-CSV conversion uses ``agate.Table``.
-* :doc:`/scripts/in2csv` GeoJSON conversion adds columns for geometry type, longitude and latitude.
-* Documentation: Update tool usage, remove shell prompts, document connection string, correct typos.
+-  csvkit is tested against Python 3.6. (#702)
+-  ``import csvkit as csv`` defers to agate readers/writers.
+-  :doc:`/scripts/csvgrep` supports ``--no-header-row``.
+-  :doc:`/scripts/csvjoin` supports ``--no-header-row``.
+-  :doc:`/scripts/csvjson` streams input and output if the ``--stream`` and ``--no-inference`` flags are set.
+-  :doc:`/scripts/csvjson` supports ``--snifflimit`` and ``--no-inference``.
+-  :doc:`/scripts/csvlook` adds ``--max-rows``, ``--max-columns`` and ``--max-column-width`` options.
+-  :doc:`/scripts/csvlook` supports ``--snifflimit`` and ``--no-inference``.
+-  :doc:`/scripts/csvpy` supports ``--agate`` to read a CSV file into an agate table.
+-  ``csvsql`` supports custom `SQLAlchemy dialects <https://docs.sqlalchemy.org/en/latest/dialects/>`_.
+-  :doc:`/scripts/csvstat` supports ``--names``.
+-  :doc:`/scripts/in2csv` CSV-to-CSV conversion streams input and output if the ``--no-inference`` flag is set.
+-  :doc:`/scripts/in2csv` CSV-to-CSV conversion uses ``agate.Table``.
+-  :doc:`/scripts/in2csv` GeoJSON conversion adds columns for geometry type, longitude and latitude.
+-  Documentation: Update tool usage, remove shell prompts, document connection string, correct typos.
 
 Fixes:
 
-* Fixed numerous instances of open files not being closed before utilities exit.
-* Change ``-b``, ``--doublequote`` to ``--no-doublequote``, as doublequote is True by default.
-* :doc:`/scripts/in2csv` DBF conversion works with Python 3.
-* :doc:`/scripts/in2csv` correctly guesses format when file has an uppercase extension.
-* :doc:`/scripts/in2csv` correctly interprets ``--no-inference``.
-* :doc:`/scripts/in2csv` again supports nested JSON objects (fixes regression).
-* :doc:`/scripts/in2csv` with ``--format geojson`` prints a JSON object instead of ``OrderedDict([(...)])``.
-* :doc:`/scripts/csvclean` with standard input works on Windows.
-* :doc:`/scripts/csvgrep` returns the input file's line numbers if the ``--linenumbers`` flag is set.
-* :doc:`/scripts/csvgrep` can match multiline values.
-* :doc:`/scripts/csvgrep` correctly operates on ragged rows.
-* :doc:`/scripts/csvsql` correctly escapes ``%``` characters in SQL queries.
-* :doc:`/scripts/csvsql` adds standard input only if explicitly requested.
-* :doc:`/scripts/csvstack` supports stacking a single file.
-* :doc:`/scripts/csvstat` always reports frequencies.
-* The ``any_match`` argument of ``FilteringCSVReader`` works correctly.
-* All tools handle empty files without error.
+-  Fixed numerous instances of open files not being closed before utilities exit.
+-  Change ``-b``, ``--doublequote`` to ``--no-doublequote``, as doublequote is True by default.
+-  :doc:`/scripts/in2csv` DBF conversion works with Python 3.
+-  :doc:`/scripts/in2csv` correctly guesses format when file has an uppercase extension.
+-  :doc:`/scripts/in2csv` correctly interprets ``--no-inference``.
+-  :doc:`/scripts/in2csv` again supports nested JSON objects (fixes regression).
+-  :doc:`/scripts/in2csv` with ``--format geojson`` prints a JSON object instead of ``OrderedDict([(...)])``.
+-  :doc:`/scripts/csvclean` with standard input works on Windows.
+-  :doc:`/scripts/csvgrep` returns the input file's line numbers if the ``--linenumbers`` flag is set.
+-  :doc:`/scripts/csvgrep` can match multiline values.
+-  :doc:`/scripts/csvgrep` correctly operates on ragged rows.
+-  :doc:`/scripts/csvsql` correctly escapes ``%``` characters in SQL queries.
+-  :doc:`/scripts/csvsql` adds standard input only if explicitly requested.
+-  :doc:`/scripts/csvstack` supports stacking a single file.
+-  :doc:`/scripts/csvstat` always reports frequencies.
+-  The ``any_match`` argument of ``FilteringCSVReader`` works correctly.
+-  All tools handle empty files without error.
 
 0.9.1 - March 31, 2015
 ----------------------
 
-* Add Antonio Lima to AUTHORS.
-* Add support for ndjson. (#329)
-* Add missing docs for csvcut -C. (#227)
-* Reorganize docs so TOC works better. (#339)
-* Render docs locally with RTD theme.
-* Fix header in "tricks" docs.
-* Add install instructions to tutorial. (#331)
-* Add killer examples to doc index. (#328)
-* Reorganize doc index
-* Fix broken csvkit module documentation. (#327)
-* Fix version of openpyxl to work around encoding issue. (#391, #288)
+-  Add Antonio Lima to AUTHORS.
+-  Add support for ndjson. (#329)
+-  Add missing docs for csvcut -C. (#227)
+-  Reorganize docs so TOC works better. (#339)
+-  Render docs locally with RTD theme.
+-  Fix header in "tricks" docs.
+-  Add install instructions to tutorial. (#331)
+-  Add killer examples to doc index. (#328)
+-  Reorganize doc index
+-  Fix broken csvkit module documentation. (#327)
+-  Fix version of openpyxl to work around encoding issue. (#391, #288)
 
 0.9.0 - September 8, 2014
 -------------------------
 
-* Write missing sections of the tutorial. (#32)
-* Remove -q arg from sql2csv (conflicts with common flag).
-* Fix csvjoin in case where left dataset rows without all columns.
-* Rewrote tutorial based on LESO data. (#324)
-* Don't error in csvjson if lat/lon columns are null. (#326)
-* Maintain field order in output of csvjson.
-* Add unit test for json in2csv. (#77)
-* Maintain key order when converting JSON into CSV. (#325.)
-* Upgrade python-dateutil to version 2.2 (#304)
-* Fix sorting of columns with null values. (#302)
-* Added release documentation.
-* Fill out short rows with null values. (#313)
-* Fix unicode output for csvlook and csvstat. (#315)
-* Add documentation for --zero. (#323)
-* Fix Integrity error when inserting zero rows in database with csvsql. (#299)
-* Add Michael Mior to AUTHORS. (#305)
-* Add --count option to CSVStat.
-* Implement csvformat.
-* Fix bug causing CSVKitDictWriter to output 'utf-8' for blank fields.
+-  Write missing sections of the tutorial. (#32)
+-  Remove -q arg from sql2csv (conflicts with common flag).
+-  Fix csvjoin in case where left dataset rows without all columns.
+-  Rewrote tutorial based on LESO data. (#324)
+-  Don't error in csvjson if lat/lon columns are null. (#326)
+-  Maintain field order in output of csvjson.
+-  Add unit test for json in2csv. (#77)
+-  Maintain key order when converting JSON into CSV. (#325.)
+-  Upgrade python-dateutil to version 2.2 (#304)
+-  Fix sorting of columns with null values. (#302)
+-  Added release documentation.
+-  Fill out short rows with null values. (#313)
+-  Fix unicode output for csvlook and csvstat. (#315)
+-  Add documentation for --zero. (#323)
+-  Fix Integrity error when inserting zero rows in database with csvsql. (#299)
+-  Add Michael Mior to AUTHORS. (#305)
+-  Add --count option to CSVStat.
+-  Implement csvformat.
+-  Fix bug causing CSVKitDictWriter to output 'utf-8' for blank fields.
 
 0.8.0 - July 27, 2014
 ---------------------
 
-* Add pnaimoli to AUTHORS.
-* Fix column specification in csvstat. (#236)
-* Added "Tips and Tricks" documentation. (#297, #298)
-* Add Espartaco Palma to AUTHORS.
-* Remove unnecessary enumerate calls. (#292)
-* Deprecated DBF support for Python 3+.
-* Add support for Python 3.3 and 3.4 (#239)
+-  Add pnaimoli to AUTHORS.
+-  Fix column specification in csvstat. (#236)
+-  Added "Tips and Tricks" documentation. (#297, #298)
+-  Add Espartaco Palma to AUTHORS.
+-  Remove unnecessary enumerate calls. (#292)
+-  Deprecated DBF support for Python 3+.
+-  Add support for Python 3.3 and 3.4 (#239)
 
 0.7.3 - April 27, 2014
 ----------------------
 
-* Fix date handling with openpyxl > 2.0 (#285)
-* Add Kristina Durivage to AUTHORS. (#243)
-* Added Richard Low to AUTHORS.
-* Support SQL queries "directly" on CSV files. (#276)
-* Add Tasneem Raja to AUTHORS.
-* Fix off-by-one error in open ended column ranges. (#238)
-* Add Matt Pettis to AUTHORS.
-* Add line numbers flag to csvlook (#244)
-* Only install argparse for Python < 2.7. (#224)
-* Add Diego Rabatone Oliveira to AUTHORS.
-* Add Ryan Murphy to AUTHORS.
-* Fix DBF dependency. (#270)
+-  Fix date handling with openpyxl > 2.0 (#285)
+-  Add Kristina Durivage to AUTHORS. (#243)
+-  Added Richard Low to AUTHORS.
+-  Support SQL queries "directly" on CSV files. (#276)
+-  Add Tasneem Raja to AUTHORS.
+-  Fix off-by-one error in open ended column ranges. (#238)
+-  Add Matt Pettis to AUTHORS.
+-  Add line numbers flag to csvlook (#244)
+-  Only install argparse for Python < 2.7. (#224)
+-  Add Diego Rabatone Oliveira to AUTHORS.
+-  Add Ryan Murphy to AUTHORS.
+-  Fix DBF dependency. (#270)
 
 0.7.2 - March 24, 2014
 ----------------------
 
-* Fix CHANGELOG for release.
+-  Fix CHANGELOG for release.
 
 0.7.1 - March 24, 2014
 ----------------------
 
-* Fix homepage url in setup.py.
+-  Fix homepage url in setup.py.
 
 0.7.0 - March 24, 2014
 ----------------------
 
-* Fix XLSX datetime normalization bug. (#223)
-* Add raistlin7447 to AUTHORS.
-* Merged sql2csv utility (#259).
-* Add Jeroen Janssens to AUTHORS.
-* Validate csvsql DB connections before parsing CSVs. (#257)
-* Clarify install process for Ubuntu. (#249)
-* Clarify docs for --escapechar. (#242)
-* Make ``import csvkit`` API compatible with ``import csv``.
-* Update Travis CI link. (#258)
-* Add Sébastien Fievet to AUTHORS.
-* Use case-sensitive name for SQLAlchemy (#237)
-* Add Travis Swicegood to AUTHORS.
+-  Fix XLSX datetime normalization bug. (#223)
+-  Add raistlin7447 to AUTHORS.
+-  Merged sql2csv utility (#259).
+-  Add Jeroen Janssens to AUTHORS.
+-  Validate csvsql DB connections before parsing CSVs. (#257)
+-  Clarify install process for Ubuntu. (#249)
+-  Clarify docs for --escapechar. (#242)
+-  Make ``import csvkit`` API compatible with ``import csv``.
+-  Update Travis CI link. (#258)
+-  Add Sébastien Fievet to AUTHORS.
+-  Use case-sensitive name for SQLAlchemy (#237)
+-  Add Travis Swicegood to AUTHORS.
 
 0.6.1 - August 20, 2013
 -----------------------
 
-* Fix CHANGELOG for release.
+-  Fix CHANGELOG for release.
 
 0.6.0 - August 20, 2013
 -----------------------
 
-* Add Chris Rosenthal to AUTHORS.
-* Fix multi-file input to csvsql. (#193)
-* Passing --snifflimit=0 to disable dialect sniffing. (#190)
-* Add aarcro to the AUTHORS file.
-* Improve performance of csvgrep. (#204)
-* Add Matt Dudys to AUTHORS.
-* Add support for --skipinitialspace. (#201)
-* Add Joakim Lundborg to AUTHORS.
-* Add --no-inference option to in2csv and csvsql. (#206)
-* Add Federico Scrinzi to AUTHORS file.
-* Add --no-header-row to all tools. (#189)
-* Fix csvstack blowing up on empty files. (#209)
-* Add Chris Rosenthal to AUTHORS file.
-* Add --db-schema option to csvsql. (#216)
-* Add Shane StClair to AUTHORS file.
-* Add --no-inference support to csvsort. (#222)
+-  Add Chris Rosenthal to AUTHORS.
+-  Fix multi-file input to csvsql. (#193)
+-  Passing --snifflimit=0 to disable dialect sniffing. (#190)
+-  Add aarcro to the AUTHORS file.
+-  Improve performance of csvgrep. (#204)
+-  Add Matt Dudys to AUTHORS.
+-  Add support for --skipinitialspace. (#201)
+-  Add Joakim Lundborg to AUTHORS.
+-  Add --no-inference option to in2csv and csvsql. (#206)
+-  Add Federico Scrinzi to AUTHORS file.
+-  Add --no-header-row to all tools. (#189)
+-  Fix csvstack blowing up on empty files. (#209)
+-  Add Chris Rosenthal to AUTHORS file.
+-  Add --db-schema option to csvsql. (#216)
+-  Add Shane StClair to AUTHORS file.
+-  Add --no-inference support to csvsort. (#222)
 
 0.5.0 - August 21, 2012
 -----------------------
 
-* Implement geojson support in csvjson. (#159)
-* Optimize writing of eight bit codecs. (#175)
-* Created csvpy. (#44)
-* Support --not-columns for excluding columns. (#137)
-* Add Jan Schulz to AUTHORS file.
-* Add Windows scripts. (#111, #176)
-* csvjoin, csvsql and csvstack no longer hold open all files. (#178)
-* Added Noah Hoffman to AUTHORS.
-* Make csvlook output compatible with emacs table markup. (#174)
+-  Implement geojson support in csvjson. (#159)
+-  Optimize writing of eight bit codecs. (#175)
+-  Created csvpy. (#44)
+-  Support --not-columns for excluding columns. (#137)
+-  Add Jan Schulz to AUTHORS file.
+-  Add Windows scripts. (#111, #176)
+-  csvjoin, csvsql and csvstack no longer hold open all files. (#178)
+-  Added Noah Hoffman to AUTHORS.
+-  Make csvlook output compatible with emacs table markup. (#174)
 
 0.4.4 - May 1, 2012
 -------------------
 
-* Add Derek Wilson to AUTHORS.
-* Add Kevin Schaul to AUTHORS.
-* Add DBF support to in2csv. (#11, #160)
-* Support --zero option for zero-based column indexing. (#144)
-* Support mixing nulls and blanks in string columns.
-* Add --blanks option to csvsql. (#149)
-* Add multi-file (glob) support to csvsql. (#146)
-* Add Gregory Temchenko to AUTHORS.
-* Add --no-create option to csvsql. (#148)
-* Add Anton Ian Sipos to AUTHORS.
-* Fix broken pipe errors. (#150)
+-  Add Derek Wilson to AUTHORS.
+-  Add Kevin Schaul to AUTHORS.
+-  Add DBF support to in2csv. (#11, #160)
+-  Support --zero option for zero-based column indexing. (#144)
+-  Support mixing nulls and blanks in string columns.
+-  Add --blanks option to csvsql. (#149)
+-  Add multi-file (glob) support to csvsql. (#146)
+-  Add Gregory Temchenko to AUTHORS.
+-  Add --no-create option to csvsql. (#148)
+-  Add Anton Ian Sipos to AUTHORS.
+-  Fix broken pipe errors. (#150)
 
 0.4.3 - February 20, 2012
 -------------------------
 
-* Begin CHANGELOG (a bit late, I'll admit).
+-  Begin CHANGELOG (a bit late, I'll admit).
```

### Comparing `csvkit-1.5.0/CONTRIBUTING.rst` & `csvkit-2.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/COPYING` & `csvkit-2.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/PKG-INFO` & `csvkit-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvkit
-Version: 1.5.0
+Version: 2.0.0
 Summary: A suite of command-line tools for working with CSV, the king of tabular file formats.
 Home-page: https://github.com/wireservice/csvkit
 Author: Christopher Groskopf and James McKinney
 Author-email: chrisgroskopf@gmail.com
 License: MIT
 Project-URL: Documentation, https://csvkit.readthedocs.io/en/latest/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `csvkit-1.5.0/README.rst` & `csvkit-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/__init__.py` & `csvkit-2.0.0/csvkit/__init__.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/cli.py` & `csvkit-2.0.0/csvkit/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-
 import argparse
 import bz2
 import csv
 import datetime
 import decimal
 import gzip
 import itertools
@@ -18,14 +17,16 @@
 from csvkit.exceptions import ColumnIdentifierError, RequiredHeaderError
 
 try:
     import zstandard
 except ImportError:
     zstandard = None
 
+QUOTING_CHOICES = sorted(getattr(csv, name) for name in dir(csv) if name.startswith('QUOTE_'))
+
 
 class LazyFile:
     """
     A proxy for a File object that delays opening it until
     a read method is called.
 
     Currently this implements only the minimum methods to be useful,
@@ -64,27 +65,34 @@
 
 
 class CSVKitUtility:
     description = ''
     epilog = ''
     override_flags = ''
 
-    def __init__(self, args=None, output_file=None):
+    def __init__(self, args=None, output_file=None, error_file=None):
         """
         Perform argument processing and other setup for a CSVKitUtility.
         """
         self._init_common_parser()
         self.add_arguments()
         self.args = self.argparser.parse_args(args)
+
         # Output file is only set during testing.
         if output_file is None:
             self.output_file = sys.stdout
         else:
             self.output_file = output_file
 
+        # Error file is only set during testing.
+        if error_file is None:
+            self.error_file = sys.stderr
+        else:
+            self.error_file = error_file
+
         self.reader_kwargs = self._extract_csv_reader_kwargs()
         self.writer_kwargs = self._extract_csv_writer_kwargs()
 
         self._install_exception_handler()
 
         # Ensure SIGPIPE doesn't throw an exception
         # Prevents [Errno 32] Broken pipe errors, e.g. when piping to 'head'
@@ -159,25 +167,25 @@
                 help='Specify that the input CSV file is delimited with tabs. Overrides "-d".')
         if 'q' not in self.override_flags:
             self.argparser.add_argument(
                 '-q', '--quotechar', dest='quotechar',
                 help='Character used to quote strings in the input CSV file.')
         if 'u' not in self.override_flags:
             self.argparser.add_argument(
-                '-u', '--quoting', dest='quoting', type=int, choices=[0, 1, 2, 3],
-                help='Quoting style used in the input CSV file. 0 = Quote Minimal, 1 = Quote All, '
-                     '2 = Quote Non-numeric, 3 = Quote None.')
+                '-u', '--quoting', dest='quoting', type=int, choices=QUOTING_CHOICES,
+                help='Quoting style used in the input CSV file: 0 quote minimal, 1 quote all, '
+                     '2 quote non-numeric, 3 quote none.')
         if 'b' not in self.override_flags:
             self.argparser.add_argument(
                 '-b', '--no-doublequote', dest='doublequote', action='store_false',
                 help='Whether or not double quotes are doubled in the input CSV file.')
         if 'p' not in self.override_flags:
             self.argparser.add_argument(
                 '-p', '--escapechar', dest='escapechar',
-                help='Character used to escape the delimiter if --quoting 3 ("Quote None") is specified and to escape '
+                help='Character used to escape the delimiter if --quoting 3 ("quote none") is specified and to escape '
                      'the QUOTECHAR if --no-doublequote is specified.')
         if 'z' not in self.override_flags:
             self.argparser.add_argument(
                 '-z', '--maxfieldsize', dest='field_size_limit', type=int,
                 help='Maximum length of a single field in the input CSV file.')
         if 'e' not in self.override_flags:
             self.argparser.add_argument(
@@ -232,15 +240,15 @@
         if 'zero' not in self.override_flags:
             self.argparser.add_argument(
                 '--zero', dest='zero_based', action='store_true',
                 help='When interpreting or displaying column numbers, use zero-based numbering instead of the default '
                      '1-based numbering.')
 
         self.argparser.add_argument(
-            '-V', '--version', action='version', version='%(prog)s 1.5.0',
+            '-V', '--version', action='version', version='%(prog)s 2.0.0',
             help='Display version information and exit.')
 
     def _open_input_file(self, path, opened=False):
         """
         Open the input file specified on the command line.
         """
         if not path or path == '-':
@@ -326,20 +334,21 @@
             type_kwargs = {'null_values': []}
         else:
             type_kwargs = {'null_values': list(DEFAULT_NULL_VALUES)}
         for null_value in getattr(self.args, 'null_values', []):
             type_kwargs['null_values'].append(null_value)
 
         text_type = agate.Text(**type_kwargs)
+        number_type = agate.Number(locale=self.args.locale, **type_kwargs)
 
-        if self.args.no_inference:
+        if getattr(self.args, 'no_inference', None):
             types = [text_type]
+        elif getattr(self.args, 'out_quoting', None) == 2:
+            types = [number_type, text_type]
         else:
-            number_type = agate.Number(locale=self.args.locale, **type_kwargs)
-
             # See the order in the `agate.TypeTester` class.
             types = [
                 agate.Boolean(**type_kwargs),
                 agate.TimeDelta(**type_kwargs),
                 agate.Date(date_format=self.args.date_format, **type_kwargs),
                 agate.DateTime(datetime_format=self.args.datetime_format, **type_kwargs),
                 text_type,
```

### Comparing `csvkit-1.5.0/csvkit/convert/fixed.py` & `csvkit-2.0.0/csvkit/convert/fixed.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/convert/geojs.py` & `csvkit-2.0.0/csvkit/convert/geojs.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/grep.py` & `csvkit-2.0.0/csvkit/grep.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/utilities/csvcut.py` & `csvkit-2.0.0/csvkit/utilities/csvcut.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/utilities/csvformat.py` & `csvkit-2.0.0/csvkit/utilities/csvformat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 import itertools
 import sys
 
 import agate
 
-from csvkit.cli import CSVKitUtility, make_default_headers
+from csvkit.cli import QUOTING_CHOICES, CSVKitUtility, make_default_headers
 
 
 class CSVFormat(CSVKitUtility):
     description = 'Convert a CSV file to a custom output format.'
-    override_flags = ['L', 'blanks', 'date-format', 'datetime-format']
+    override_flags = ['blanks', 'date-format', 'datetime-format']
 
     def add_arguments(self):
         self.argparser.add_argument(
             '-E', '--skip-header', dest='skip_header', action='store_true',
             help='Do not output a header row.')
         self.argparser.add_argument(
             '-D', '--out-delimiter', dest='out_delimiter',
@@ -25,17 +25,17 @@
             '-A', '--out-asv', dest='out_asv', action='store_true',
             help='Specify that the output file is delimited with the ASCII unit separator and record separator. '
                  'Overrides "-T", "-D" and "-M".')
         self.argparser.add_argument(
             '-Q', '--out-quotechar', dest='out_quotechar',
             help='Character used to quote strings in the output file.')
         self.argparser.add_argument(
-            '-U', '--out-quoting', dest='out_quoting', type=int, choices=[0, 1, 2, 3],
-            help='Quoting style used in the output file. 0 = Quote Minimal, 1 = Quote All, '
-                 '2 = Quote Non-numeric, 3 = Quote None.')
+            '-U', '--out-quoting', dest='out_quoting', type=int, choices=QUOTING_CHOICES,
+            help='Quoting style used in the output file: 0 quote minimal, 1 quote all, '
+                 '2 quote non-numeric, 3 quote none.')
         self.argparser.add_argument(
             '-B', '--out-no-doublequote', dest='out_doublequote', action='store_false',
             help='Whether or not double quotes are doubled in the output file.')
         self.argparser.add_argument(
             '-P', '--out-escapechar', dest='out_escapechar',
             help='Character used to escape the delimiter in the output file if --quoting 3 ("Quote None") is '
                  'specified and to escape the QUOTECHAR if --out-no-doublequote is specified.')
@@ -68,26 +68,41 @@
 
         return kwargs
 
     def main(self):
         if self.additional_input_expected():
             sys.stderr.write('No input file or piped data provided. Waiting for standard input:\n')
 
-        reader = agate.csv.reader(self.skip_lines(), **self.reader_kwargs)
         writer = agate.csv.writer(self.output_file, **self.writer_kwargs)
-        if self.args.no_header_row:
-            # Peek at a row to get the number of columns.
-            _row = next(reader)
-            headers = make_default_headers(len(_row))
-            reader = itertools.chain([headers, _row], reader)
 
-        if self.args.skip_header:
-            next(reader)
+        if self.args.out_quoting == 2:
+            table = agate.Table.from_csv(
+                self.input_file,
+                skip_lines=self.args.skip_lines,
+                column_types=self.get_column_types(),
+                **self.reader_kwargs,
+            )
+
+            # table.to_csv() has no option to omit the column names.
+            if not self.args.skip_header:
+                writer.writerow(table.column_names)
+
+            writer.writerows(table.rows)
+        else:
+            reader = agate.csv.reader(self.skip_lines(), **self.reader_kwargs)
+            if self.args.no_header_row:
+                # Peek at a row to get the number of columns.
+                _row = next(reader)
+                headers = make_default_headers(len(_row))
+                reader = itertools.chain([headers, _row], reader)
 
-        writer.writerows(reader)
+            if self.args.skip_header:
+                next(reader)
+
+            writer.writerows(reader)
 
 
 def launch_new_instance():
     utility = CSVFormat()
     utility.run()
```

### Comparing `csvkit-1.5.0/csvkit/utilities/csvgrep.py` & `csvkit-2.0.0/csvkit/utilities/csvgrep.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/utilities/csvjoin.py` & `csvkit-2.0.0/csvkit/utilities/csvjoin.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/utilities/csvjson.py` & `csvkit-2.0.0/csvkit/utilities/csvjson.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/utilities/csvlook.py` & `csvkit-2.0.0/csvkit/utilities/csvlook.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/utilities/csvpy.py` & `csvkit-2.0.0/csvkit/utilities/csvpy.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/utilities/csvsort.py` & `csvkit-2.0.0/csvkit/utilities/csvsort.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/utilities/csvsql.py` & `csvkit-2.0.0/csvkit/utilities/csvsql.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/utilities/csvstack.py` & `csvkit-2.0.0/csvkit/utilities/csvstack.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/utilities/csvstat.py` & `csvkit-2.0.0/csvkit/utilities/csvstat.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit/utilities/in2csv.py` & `csvkit-2.0.0/csvkit/utilities/in2csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
             '-y', '--snifflimit', dest='sniff_limit', type=int, default=1024,
             help='Limit CSV dialect sniffing to the specified number of bytes. '
                  'Specify "0" to disable sniffing entirely, or "-1" to sniff the entire file.')
         self.argparser.add_argument(
             '-I', '--no-inference', dest='no_inference', action='store_true',
             help='Disable type inference (and --locale, --date-format, --datetime-format) when parsing CSV input.')
 
+    # This is called only from open_excel_input_file(), but is a separate method to use caching.
     @functools.lru_cache
     def stdin(self):
         return sys.stdin.buffer.read()
 
     def open_excel_input_file(self, path):
         if not path or path == '-':
             return BytesIO(self.stdin())
```

### Comparing `csvkit-1.5.0/csvkit/utilities/sql2csv.py` & `csvkit-2.0.0/csvkit/utilities/sql2csv.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/csvkit.egg-info/PKG-INFO` & `csvkit-2.0.0/csvkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvkit
-Version: 1.5.0
+Version: 2.0.0
 Summary: A suite of command-line tools for working with CSV, the king of tabular file formats.
 Home-page: https://github.com/wireservice/csvkit
 Author: Christopher Groskopf and James McKinney
 Author-email: chrisgroskopf@gmail.com
 License: MIT
 Project-URL: Documentation, https://csvkit.readthedocs.io/en/latest/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `csvkit-1.5.0/csvkit.egg-info/SOURCES.txt` & `csvkit-2.0.0/csvkit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -117,19 +117,24 @@
 examples/sniff_limit.csv
 examples/sort_ints_nulls.csv
 examples/test.sql
 examples/test.xls
 examples/test.xlsx
 examples/test_date_format.csv
 examples/test_date_format_converted.csv
+examples/test_empty_columns.csv
+examples/test_empty_columns_long_row.csv
+examples/test_empty_columns_short_row.csv
 examples/test_extra_header.csv
 examples/test_geo.csv
 examples/test_geojson.csv
 examples/test_geojson.json
+examples/test_header_newline.csv
 examples/test_ignore_case.csv
+examples/test_join_short_rows.csv
 examples/test_latin1.csv
 examples/test_latin1.sql
 examples/test_literal_order.csv
 examples/test_locale.csv
 examples/test_locale_converted.csv
 examples/test_numeric_date_format.csv
 examples/test_precision.csv
```

### Comparing `csvkit-1.5.0/csvkit.egg-info/entry_points.txt` & `csvkit-2.0.0/csvkit.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/Makefile` & `csvkit-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/_build/man/csvcut.1` & `csvkit-2.0.0/docs/_build/man/csvcut.1`

 * *Files 9% similar despite different names*

```diff
@@ -23,25 +23,24 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "CSVCUT" "1" "Mar 28, 2024" "1.5.0" "csvkit"
+.TH "CSVCUT" "1" "May 01, 2024" "2.0.0" "csvkit"
 .SH NAME
 csvcut \- csvcut Documentation
 .SH DESCRIPTION
 .sp
 Filters and truncates CSV files. Like the Unix \(dqcut\(dq command, but for tabular data:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 usage: csvcut [\-h] [\-d DELIMITER] [\-t] [\-q QUOTECHAR] [\-u {0,1,2,3}] [\-b]
               [\-p ESCAPECHAR] [\-z FIELD_SIZE_LIMIT] [\-e ENCODING] [\-S] [\-H]
               [\-K SKIP_LINES] [\-v] [\-l] [\-\-zero] [\-V] [\-n] [\-c COLUMNS]
               [\-C NOT_COLUMNS] [\-x]
               [FILE]
 
 Filter and truncate CSV files. Like the Unix \(dqcut\(dq command, but for tabular
@@ -61,16 +60,15 @@
                         all columns.
   \-C NOT_COLUMNS, \-\-not\-columns NOT_COLUMNS
                         A comma\-separated list of column indices, names or
                         ranges to be excluded, e.g. \(dq1,id,3\-5\(dq. Defaults to no
                         columns.
   \-x, \-\-delete\-empty\-rows
                         After cutting, delete rows which are completely empty.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 See also: \fI\%Arguments common to all tools\fP\&.
 .sp
 \fBNOTE:\fP
 .INDENT 0.0
@@ -88,125 +86,109 @@
 .SH EXAMPLES
 .SS Print columns
 .sp
 Print the indices and names of all columns:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 $ csvcut \-n examples/realdata/FY09_EDU_Recipients_by_State.csv
   1: State Name
   2: State Abbreviate
   3: Code
   4: Montgomery GI Bill\-Active Duty
   5: Montgomery GI Bill\- Selective Reserve
   6: Dependents\(aq Educational Assistance
   7: Reserve Educational Assistance Program
   8: Post\-Vietnam Era Veteran\(aqs Educational Assistance Program
   9: TOTAL
  10:
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Print only the names of all columns, by removing the indices with the \fBcut\fP command:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 $ csvcut \-n examples/realdata/FY09_EDU_Recipients_by_State.csv | cut \-c6\-
 State Name
 State Abbreviate
 Code
 Montgomery GI Bill\-Active Duty
 Montgomery GI Bill\- Selective Reserve
 Dependents\(aq Educational Assistance
 Reserve Educational Assistance Program
 Post\-Vietnam Era Veteran\(aqs Educational Assistance Program
 TOTAL
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SS Extract columns
 .sp
 Extract the first and third columns:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvcut \-c 1,3 examples/realdata/FY09_EDU_Recipients_by_State.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Extract columns named \(dqTOTAL\(dq and \(dqState Name\(dq (in that order):
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvcut \-c TOTAL,\(dqState Name\(dq examples/realdata/FY09_EDU_Recipients_by_State.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Extract a column that may not exist in all files:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 echo d, | csvjoin examples/dummy.csv \- | csvcut \-c d
  echo d, | csvjoin examples/join_no_header_row.csv \- | csvcut \-c d
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SS Other
 .sp
 Add line numbers to a file, making no other changes:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvcut \-l examples/realdata/FY09_EDU_Recipients_by_State.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Display a column\(aqs unique values:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvcut \-c 1 examples/realdata/FY09_EDU_Recipients_by_State.csv | sed 1d | sort | uniq
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Or:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvcut \-c 1 examples/realdata/FY09_EDU_Recipients_by_State.csv | csvsql \-\-query \(aqSELECT DISTINCT(\(dqState Name\(dq) FROM stdin\(aq
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH AUTHOR
 Christopher Groskopf and contributors
 .SH COPYRIGHT
 2016, Christopher Groskopf and James McKinney
 .\" Generated by docutils manpage writer.
```

### Comparing `csvkit-1.5.0/docs/_build/man/csvformat.1` & `csvkit-2.0.0/docs/_build/man/csvformat.1`

 * *Files 18% similar despite different names*

```diff
@@ -23,29 +23,28 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "CSVFORMAT" "1" "Mar 28, 2024" "1.5.0" "csvkit"
+.TH "CSVFORMAT" "1" "May 01, 2024" "2.0.0" "csvkit"
 .SH NAME
 csvformat \- csvformat Documentation
 .SH DESCRIPTION
 .sp
 Convert a CSV file to a custom output format.:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 usage: csvformat [\-h] [\-d DELIMITER] [\-t] [\-q QUOTECHAR] [\-u {0,1,2,3}] [\-b]
-                 [\-p ESCAPECHAR] [\-z FIELD_SIZE_LIMIT] [\-e ENCODING] [\-S] [\-H]
-                 [\-K SKIP_LINES] [\-v] [\-l] [\-\-zero] [\-V] [\-E]
-                 [\-D OUT_DELIMITER] [\-T] [\-A] [\-Q OUT_QUOTECHAR]
+                 [\-p ESCAPECHAR] [\-z FIELD_SIZE_LIMIT] [\-e ENCODING]
+                 [\-L LOCALE] [\-S] [\-H] [\-K SKIP_LINES] [\-v] [\-l] [\-\-zero] [\-V]
+                 [\-E] [\-D OUT_DELIMITER] [\-T] [\-A] [\-Q OUT_QUOTECHAR]
                  [\-U {0,1,2,3}] [\-B] [\-P OUT_ESCAPECHAR]
                  [\-M OUT_LINETERMINATOR]
                  [FILE]
 
 Convert a CSV file to a custom output format.
 
 positional arguments:
@@ -61,80 +60,71 @@
                         Overrides \(dq\-D\(dq.
   \-A, \-\-out\-asv         Specify that the output file is delimited with the
                         ASCII unit separator and record separator. Overrides
                         \(dq\-T\(dq, \(dq\-D\(dq and \(dq\-M\(dq.
   \-Q OUT_QUOTECHAR, \-\-out\-quotechar OUT_QUOTECHAR
                         Character used to quote strings in the output file.
   \-U {0,1,2,3}, \-\-out\-quoting {0,1,2,3}
-                        Quoting style used in the output file. 0 = Quote
-                        Minimal, 1 = Quote All, 2 = Quote Non\-numeric, 3 =
-                        Quote None.
+                        Quoting style used in the output file: 0 quote
+                        minimal, 1 quote all, 2 quote non\-numeric, 3 quote
+                        none.
   \-B, \-\-out\-no\-doublequote
                         Whether or not double quotes are doubled in the output
                         CSV file.
   \-P OUT_ESCAPECHAR, \-\-out\-escapechar OUT_ESCAPECHAR
                         Character used to escape the delimiter in the output
                         CSV file if \-\-quoting 3 (\(dqQuote None\(dq) is specified
                         and to escape the QUOTECHAR if \-\-out\-no\-doublequote is
                         specified.
   \-M OUT_LINETERMINATOR, \-\-out\-lineterminator OUT_LINETERMINATOR
                         Character used to terminate lines in the output file.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 See also: \fI\%Arguments common to all tools\fP\&.
 .SH EXAMPLES
 .sp
 Convert a comma\-separated file to a pipe\-delimited file:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvformat \-D \(dq|\(dq examples/dummy.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Convert to carriage return line\-endings:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvformat \-M $\(aq\er\(aq examples/dummy.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Convert to a tab\-delimited file (TSV) with no doubling of double quotes:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 printf \(aqkey,value\en1,\(dqa \(dq\(dqquoted\(dq\(dq string\(dq\(aq | csvformat \-T \-Q🐍
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 To avoid escaping quote characters when using \fB\-\-quoting 3\fP, add \fB\-\-out\-quotechar \(dq\(dq\fP:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvformat \-u3 \-U3 \-Q🐍 examples/optional_quote_characters.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH AUTHOR
 Christopher Groskopf and contributors
 .SH COPYRIGHT
 2016, Christopher Groskopf and James McKinney
 .\" Generated by docutils manpage writer.
```

### Comparing `csvkit-1.5.0/docs/_build/man/csvgrep.1` & `csvkit-2.0.0/docs/_build/man/csvgrep.1`

 * *Files 9% similar despite different names*

```diff
@@ -23,25 +23,24 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "CSVGREP" "1" "Mar 28, 2024" "1.5.0" "csvkit"
+.TH "CSVGREP" "1" "May 01, 2024" "2.0.0" "csvkit"
 .SH NAME
 csvgrep \- csvgrep Documentation
 .SH DESCRIPTION
 .sp
 Filter tabular data to only those rows where certain columns contain a given value or match a regular expression:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 usage: csvgrep [\-h] [\-d DELIMITER] [\-t] [\-q QUOTECHAR] [\-u {0,1,2,3}] [\-b]
                [\-p ESCAPECHAR] [\-z FIELD_SIZE_LIMIT] [\-e ENCODING] [\-S] [\-H]
                [\-K SKIP_LINES] [\-v] [\-l] [\-\-zero] [\-V] [\-n] [\-c COLUMNS]
                [\-m PATTERN] [\-r REGEX] [\-f MATCHFILE] [\-i] [\-a]
                [FILE]
 
 Search CSV files. Like the Unix \(dqgrep\(dq command, but for tabular data.
@@ -64,81 +63,87 @@
   \-f MATCHFILE, \-\-file MATCHFILE
                         A path to a file. For each row, if any line in the
                         file (stripped of line separators) is an exact match
                         of the cell value, the row matches.
   \-i, \-\-invert\-match    Select non\-matching rows, instead of matching rows.
   \-a  \-\-any\-match       Select rows in which any column matches, instead of
                         all columns.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 See also: \fI\%Arguments common to all tools\fP\&.
 .sp
 NOTE: Even though \(aq\-m\(aq, \(aq\-r\(aq, and \(aq\-f\(aq are listed as \(dqoptional\(dq arguments, you must specify one of them.
 .SH EXAMPLES
 .sp
 Search for the row relating to Illinois:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvgrep \-c 1 \-m ILLINOIS examples/realdata/FY09_EDU_Recipients_by_State.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Search for rows relating to states with names beginning with the letter \(dqI\(dq:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvgrep \-c 1 \-r \(dq^I\(dq examples/realdata/FY09_EDU_Recipients_by_State.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Search for rows that do not contain an empty state cell:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvgrep \-c 1 \-r \(dq^$\(dq \-i examples/realdata/FY09_EDU_Recipients_by_State.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Perform a case\-insensitive search:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvgrep \-c 1 \-r \(dq(?i)illinois\(dq examples/realdata/FY09_EDU_Recipients_by_State.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
-Get the indices of the columns that contain matching text (\fB\ex1e\fP is the \fI\%Record Separator (RS) character\fP):
+Remove comment rows:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
+printf \(dqa,b\en1,2\en# a comment\en3,4\(dq | csvgrep \-\-invert\-match \-c1 \-r \(aq^#\(aq
+.EE
+.UNINDENT
+.UNINDENT
+.sp
+Get the indices of the columns that contain matching text (\fB\ex1e\fP is the \X'tty: link https://en.wikipedia.org/wiki/C0_and_C1_control_codes#Field_separators'\fI\%Record Separator (RS) character\fP\X'tty: link'):
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.EX
 csvgrep \-m 22 \-a \-c 1\- examples/realdata/FY09_EDU_Recipients_by_State.csv | csvformat \-M $\(aq\ex1e\(aq | xargs \-d $\(aq\ex1e\(aq \-n1 sh \-c \(aqecho $0 | csvcut \-n\(aq | grep 22
-.ft P
-.fi
+.EE
+.UNINDENT
+.UNINDENT
+.sp
+\fBNOTE:\fP
+.INDENT 0.0
+.INDENT 3.5
+This last example is not performant.
 .UNINDENT
 .UNINDENT
 .SH AUTHOR
 Christopher Groskopf and contributors
 .SH COPYRIGHT
 2016, Christopher Groskopf and James McKinney
 .\" Generated by docutils manpage writer.
```

### Comparing `csvkit-1.5.0/docs/_build/man/csvjoin.1` & `csvkit-2.0.0/docs/_build/man/csvjoin.1`

 * *Files 7% similar despite different names*

```diff
@@ -23,25 +23,24 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "CSVJOIN" "1" "Mar 28, 2024" "1.5.0" "csvkit"
+.TH "CSVJOIN" "1" "May 01, 2024" "2.0.0" "csvkit"
 .SH NAME
 csvjoin \- csvjoin Documentation
 .SH DESCRIPTION
 .sp
 Merges two or more CSV tables together using a method analogous to SQL JOIN operation. By default it performs an inner join, but full outer, left outer, and right outer are also available via flags. Key columns are specified with the \-c flag (either a single column which exists in all tables, or a comma\-separated list of columns with one corresponding to each). If the columns flag is not provided then the tables will be merged \(dqsequentially\(dq, that is they will be merged in row order with no filtering:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 usage: csvjoin [\-h] [\-d DELIMITER] [\-t] [\-q QUOTECHAR] [\-u {0,1,2,3}] [\-b]
                [\-p ESCAPECHAR] [\-z FIELD_SIZE_LIMIT] [\-e ENCODING] [\-L LOCALE]
                [\-S] [\-\-blanks] [\-\-null\-value NULL_VALUES [NULL_VALUES ...]]
                [\-\-date\-format DATE_FORMAT] [\-\-datetime\-format DATETIME_FORMAT]
                [\-H] [\-K SKIP_LINES] [\-v] [\-l] [\-\-zero] [\-V] [\-c COLUMNS]
                [\-\-outer] [\-\-left] [\-\-right] [\-y SNIFF_LIMIT] [\-I]
                [FILE [FILE ...]]
@@ -73,53 +72,46 @@
   \-y SNIFF_LIMIT, \-\-snifflimit SNIFF_LIMIT
                         Limit CSV dialect sniffing to the specified number of
                         bytes. Specify \(dq0\(dq to disable sniffing.
   \-I, \-\-no\-inference    Disable type inference when parsing CSV input.
 
 Note that the join operation requires reading all files into memory. Don\(aqt try
 this on very large files.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 See also: \fI\%Arguments common to all tools\fP\&.
 .SH EXAMPLES
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvjoin \-c 1 examples/join_a.csv examples/join_b.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Add two empty columns to the right of a CSV:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 echo \(dq,\(dq | csvjoin examples/dummy.csv \-
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Add a single column to the right of a CSV:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 echo \(dqnew\-column\(dq | csvjoin examples/dummy.csv \-
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH AUTHOR
 Christopher Groskopf and contributors
 .SH COPYRIGHT
 2016, Christopher Groskopf and James McKinney
 .\" Generated by docutils manpage writer.
```

### Comparing `csvkit-1.5.0/docs/_build/man/csvjson.1` & `csvkit-2.0.0/docs/_build/man/csvjson.1`

 * *Files 2% similar despite different names*

```diff
@@ -23,25 +23,24 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "CSVJSON" "1" "Mar 28, 2024" "1.5.0" "csvkit"
+.TH "CSVJSON" "1" "May 01, 2024" "2.0.0" "csvkit"
 .SH NAME
 csvjson \- csvjson Documentation
 .SH DESCRIPTION
 .sp
 Converts a CSV file into JSON or GeoJSON (depending on flags):
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 usage: csvjson [\-h] [\-d DELIMITER] [\-t] [\-q QUOTECHAR] [\-u {0,1,2,3}] [\-b]
                [\-p ESCAPECHAR] [\-z FIELD_SIZE_LIMIT] [\-e ENCODING] [\-L LOCALE]
                [\-S] [\-\-blanks] [\-\-null\-value NULL_VALUES [NULL_VALUES ...]]
                [\-\-date\-format DATE_FORMAT] [\-\-datetime\-format DATETIME_FORMAT]
                [\-H] [\-K SKIP_LINES] [\-v] [\-l] [\-\-zero] [\-V] [\-i INDENT]
                [\-k KEY] [\-\-lat LAT] [\-\-lon LON] [\-\-type TYPE]
                [\-\-geometry GEOMETRY] [\-\-crs CRS] [\-\-no\-bbox] [\-\-stream]
@@ -79,28 +78,26 @@
   \-\-stream              Output JSON as a stream of newline\-separated objects,
                         rather than an as an array.
   \-y SNIFF_LIMIT, \-\-snifflimit SNIFF_LIMIT
                         Limit CSV dialect sniffing to the specified number of
                         bytes. Specify \(dq0\(dq to disable sniffing.
   \-I, \-\-no\-inference    Disable type inference (and \-\-locale, \-\-date\-format,
                         \-\-datetime\-format) when parsing CSV input.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 See also: \fI\%Arguments common to all tools\fP\&.
 .SH EXAMPLES
 .sp
 Convert veteran\(aqs education dataset to JSON keyed by state abbreviation:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 $ csvjson \-k \(dqState Abbreviate\(dq \-i 4 examples/realdata/FY09_EDU_Recipients_by_State.csv
 {
     \(dqAL\(dq: {
         \(dqState Name\(dq: \(dqALABAMA\(dq,
         \(dqState Abbreviate\(dq: \(dqAL\(dq,
         \(dqCode\(dq: 1.0,
         \(dqMontgomery GI Bill\-Active Duty\(dq: 6718.0,
@@ -111,25 +108,23 @@
         \(dqTOTAL\(dq: 12426.0,
         \(dqj\(dq: null
     },
     \(dq...\(dq: {
         \(dq...\(dq: \(dq...\(dq
     }
 }
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Convert locations of public art into GeoJSON:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 $ csvjson \-\-lat latitude \-\-lon longitude \-\-k slug \-\-crs EPSG:4269 \-i 4 examples/test_geo.csv
 {
     \(dqtype\(dq: \(dqFeatureCollection\(dq,
     \(dqbbox\(dq: [
         \-95.334619,
         32.299076986939205,
         \-95.250699,
@@ -171,16 +166,15 @@
     \(dqcrs\(dq: {
         \(dqtype\(dq: \(dqname\(dq,
         \(dqproperties\(dq: {
             \(dqname\(dq: \(dqEPSG:4269\(dq
         }
     }
 }
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH AUTHOR
 Christopher Groskopf and contributors
 .SH COPYRIGHT
 2016, Christopher Groskopf and James McKinney
 .\" Generated by docutils manpage writer.
```

### Comparing `csvkit-1.5.0/docs/_build/man/csvlook.1` & `csvkit-2.0.0/docs/_build/man/csvlook.1`

 * *Files 19% similar despite different names*

```diff
@@ -23,25 +23,24 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "CSVLOOK" "1" "Mar 28, 2024" "1.5.0" "csvkit"
+.TH "CSVLOOK" "1" "May 01, 2024" "2.0.0" "csvkit"
 .SH NAME
 csvlook \- csvlook Documentation
 .SH DESCRIPTION
 .sp
 Renders a CSV to the command line in a Markdown\-compatible, fixed\-width format:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 usage: csvlook [\-h] [\-d DELIMITER] [\-t] [\-q QUOTECHAR] [\-u {0,1,2,3}] [\-b]
                [\-p ESCAPECHAR] [\-z FIELD_SIZE_LIMIT] [\-e ENCODING] [\-L LOCALE]
                [\-S] [\-\-blanks] [\-\-null\-value NULL_VALUES [NULL_VALUES ...]]
                [\-\-date\-format DATE_FORMAT] [\-\-datetime\-format DATETIME_FORMAT]
                [\-H] [\-K SKIP_LINES] [\-v] [\-l] [\-\-zero] [\-V]
                [\-\-max\-rows MAX_ROWS] [\-\-max\-columns MAX_COLUMNS]
                [\-\-max\-column\-width MAX_COLUMN_WIDTH]
@@ -71,16 +70,15 @@
   \-\-no\-number\-ellipsis  Disable the ellipsis if \-\-max\-precision is exceeded.
   \-y SNIFF_LIMIT, \-\-snifflimit SNIFF_LIMIT
                         Limit CSV dialect sniffing to the specified number of
                         bytes. Specify \(dq0\(dq to disable sniffing entirely, or
                         \(dq\-1\(dq to sniff the entire file.
   \-I, \-\-no\-inference    Disable type inference when parsing the input. This
                         disables the reformatting of values.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 If a table is too wide to display properly try piping the output to \fBless \-S\fP or truncating it using \fI\%csvcut\fP\&.
 .sp
 If the table is too long, try filtering it down with grep or piping the output to \fBless\fP\&.
 .sp
@@ -94,57 +92,49 @@
 .UNINDENT
 .SH EXAMPLES
 .sp
 Basic use:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvlook examples/testfixed_converted.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 This tool is especially useful as a final operation when piping through other tools:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvcut \-c 9,1 examples/realdata/FY09_EDU_Recipients_by_State.csv | csvlook
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 If a data row contains more cells than the header row, csvlook will error. To fix the header row, use \fI\%csvclean\fP\&.
 .sp
 To ignore the extra cells, instead:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvcut \-C \(dq\(dq examples/bad.csv | csvlook
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 If these rows are at the top of the file (for example, copyright notices), you can skip the rows:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvlook \-\-skip\-lines 1 examples/bad.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 This error can also occur if csvlook incorrectly deduces (\(dqsniffs\(dq) the CSV format. To disable CSV sniffing, set \fB\-\-snifflimit 0\fP and then, if necessary, set the \fB\-\-delimiter\fP and \fB\-\-quotechar\fP options yourself. Or, set \fB\-\-snifflimit \-1\fP to use the entire file as the sample, instead of the first 1024 bytes.
 .SH AUTHOR
 Christopher Groskopf and contributors
 .SH COPYRIGHT
```

### Comparing `csvkit-1.5.0/docs/_build/man/csvpy.1` & `csvkit-2.0.0/docs/_build/man/csvpy.1`

 * *Files 4% similar despite different names*

```diff
@@ -23,25 +23,24 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "CSVPY" "1" "Mar 28, 2024" "1.5.0" "csvkit"
+.TH "CSVPY" "1" "May 01, 2024" "2.0.0" "csvkit"
 .SH NAME
 csvpy \- csvpy Documentation
 .SH DESCRIPTION
 .sp
 Loads a CSV file into a \fBagate.csv.Reader\fP object and then drops into a Python shell so the user can inspect the data however they see fit:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 usage: csvpy [\-h] [\-d DELIMITER] [\-t] [\-q QUOTECHAR] [\-u {0,1,2,3}] [\-b]
              [\-p ESCAPECHAR] [\-z FIELD_SIZE_LIMIT] [\-e ENCODING] [\-L LOCALE]
              [\-S] [\-\-blanks] [\-\-null\-value NULL_VALUES [NULL_VALUES ...]]
              [\-\-date\-format DATE_FORMAT] [\-\-datetime\-format DATETIME_FORMAT]
              [\-H] [\-K SKIP_LINES] [\-v] [\-l] [\-\-zero] [\-V] [\-\-dict] [\-\-agate]
              [\-\-no\-number\-ellipsis] [\-y SNIFF_LIMIT] [\-I]
              [FILE]
@@ -59,16 +58,15 @@
   \-\-no\-number\-ellipsis  Disable the ellipsis if the max precision is exceeded.
   \-y SNIFF_LIMIT, \-\-snifflimit SNIFF_LIMIT
                         Limit CSV dialect sniffing to the specified number of
                         bytes. Specify \(dq0\(dq to disable sniffing entirely, or
                         \(dq\-1\(dq to sniff the entire file.
   \-I, \-\-no\-inference    Disable type inference when parsing the input. This
                         disables the reformatting of values.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 This tool will automatically use the IPython shell if it is installed, otherwise it will use the running Python shell.
 .sp
 \fBNOTE:\fP
 .INDENT 0.0
@@ -80,58 +78,52 @@
 See also: \fI\%Arguments common to all tools\fP\&.
 .SH EXAMPLES
 .sp
 Basic use:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B $ csvpy examples/dummy.csv
 Welcome! \(dqexamples/dummy.csv\(dq has been loaded in a reader object named \(dqreader\(dq.
 >>> next(reader)
 [\(aqa\(aq, \(aqb\(aq, \(aqc\(aq]
 .UNINDENT
 .sp
 As a dictionary:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 $ csvpy \-\-dict examples/dummy.csv
 Welcome! \(dqexamples/dummy.csv\(dq has been loaded in a DictReader object named \(dqreader\(dq.
 >>> next(reader)
 {\(aqa\(aq: \(aq1\(aq, \(aqc\(aq: \(aq3\(aq, \(aqb\(aq: \(aq2\(aq}
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 As an agate table:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 $ csvpy \-\-agate examples/dummy.csv
 Welcome! \(dqexamples/dummy.csv\(dq has been loaded in a from_csv object named \(dqreader\(dq.
 >>> reader.print_table()
 |    a | b | c |
 | \-\-\-\- | \- | \- |
 | True | 2 | 3 |
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH AUTHOR
 Christopher Groskopf and contributors
 .SH COPYRIGHT
 2016, Christopher Groskopf and James McKinney
 .\" Generated by docutils manpage writer.
```

### Comparing `csvkit-1.5.0/docs/_build/man/csvsort.1` & `csvkit-2.0.0/docs/_build/man/csvsort.1`

 * *Files 6% similar despite different names*

```diff
@@ -23,25 +23,24 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "CSVSORT" "1" "Mar 28, 2024" "1.5.0" "csvkit"
+.TH "CSVSORT" "1" "May 01, 2024" "2.0.0" "csvkit"
 .SH NAME
 csvsort \- csvsort Documentation
 .SH DESCRIPTION
 .sp
 Sort CSV files. Like the Unix \(dqsort\(dq command, but for tabular data:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 usage: csvsort [\-h] [\-d DELIMITER] [\-t] [\-q QUOTECHAR] [\-u {0,1,2,3}] [\-b]
                [\-p ESCAPECHAR] [\-z FIELD_SIZE_LIMIT] [\-e ENCODING] [\-L LOCALE]
                [\-S] [\-\-blanks] [\-\-null\-value NULL_VALUES [NULL_VALUES ...]]
                [\-\-date\-format DATE_FORMAT] [\-\-datetime\-format DATETIME_FORMAT]
                [\-H] [\-K SKIP_LINES] [\-v] [\-l] [\-\-zero] [\-V] [\-n] [\-c COLUMNS]
                [\-r] [\-i] [\-y SNIFF_LIMIT] [\-I]
                [FILE]
@@ -62,16 +61,15 @@
                         columns.
   \-r, \-\-reverse         Sort in descending order.
   \-i, \-\-ignore\-case     Perform case\-independent sorting.
   \-y SNIFF_LIMIT, \-\-snifflimit SNIFF_LIMIT
                         Limit CSV dialect sniffing to the specified number of
                         bytes. Specify \(dq0\(dq to disable sniffing.
   \-I, \-\-no\-inference    Disable type inference when parsing the input.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 See also: \fI\%Arguments common to all tools\fP\&.
 .sp
 \fBNOTE:\fP
 .INDENT 0.0
@@ -81,31 +79,27 @@
 .UNINDENT
 .SH EXAMPLES
 .sp
 Sort the veteran\(aqs education benefits table by the \(dqTOTAL\(dq column:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvsort \-c 9 examples/realdata/FY09_EDU_Recipients_by_State.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 View the five states with the most individuals claiming veteran\(aqs education benefits:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvcut \-c 1,9 examples/realdata/FY09_EDU_Recipients_by_State.csv | csvsort \-r \-c 2 | head \-n 5
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH AUTHOR
 Christopher Groskopf and contributors
 .SH COPYRIGHT
 2016, Christopher Groskopf and James McKinney
 .\" Generated by docutils manpage writer.
```

### Comparing `csvkit-1.5.0/docs/_build/man/csvsql.1` & `csvkit-2.0.0/docs/_build/man/csvsql.1`

 * *Files 17% similar despite different names*

```diff
@@ -23,25 +23,24 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "CSVSQL" "1" "Mar 28, 2024" "1.5.0" "csvkit"
+.TH "CSVSQL" "1" "May 01, 2024" "2.0.0" "csvkit"
 .SH NAME
 csvsql \- csvsql Documentation
 .SH DESCRIPTION
 .sp
 Generate SQL statements for a CSV file or execute those statements directly on a database. In the latter case supports both creating tables and inserting data:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 usage: csvsql [\-h] [\-d DELIMITER] [\-t] [\-q QUOTECHAR] [\-u {0,1,2,3}] [\-b]
               [\-p ESCAPECHAR] [\-z FIELD_SIZE_LIMIT] [\-e ENCODING] [\-L LOCALE]
               [\-S] [\-\-blanks] [\-\-null\-value NULL_VALUES [NULL_VALUES ...]]
               [\-\-date\-format DATE_FORMAT] [\-\-datetime\-format DATETIME_FORMAT]
               [\-H] [\-K SKIP_LINES] [\-v] [\-l] [\-\-zero] [\-V]
               [\-i {firebird,mssql,mysql,oracle,postgresql,sqlite,sybase}]
               [\-\-db CONNECTION_STRING] [\-\-query QUERIES] [\-\-insert]
@@ -99,180 +98,157 @@
   \-y SNIFF_LIMIT, \-\-snifflimit SNIFF_LIMIT
                         Limit CSV dialect sniffing to the specified number of
                         bytes. Specify \(dq0\(dq to disable sniffing.
   \-I, \-\-no\-inference    Disable type inference when parsing the input.
   \-\-chunk\-size CHUNK_SIZE
                         Chunk size for batch insert into the table. Requires
                         \-\-insert.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 See also: \fI\%Arguments common to all tools\fP\&.
 .sp
-For information on connection strings and supported dialects refer to the \fI\%SQLAlchemy documentation\fP\&.
+For information on connection strings and supported dialects refer to the \X'tty: link https://www.sqlalchemy.org/docs/dialects/'\fI\%SQLAlchemy documentation\fP\X'tty: link'\&.
 .sp
-If you prefer not to enter your password in the connection string, store the password securely in a \fI\%PostgreSQL Password File\fP, a \fI\%MySQL Options File\fP or similar files for other systems.
+If you prefer not to enter your password in the connection string, store the password securely in a \X'tty: link https://www.postgresql.org/docs/9.1/static/libpq-pgpass.html'\fI\%PostgreSQL Password File\fP\X'tty: link', a \X'tty: link https://dev.mysql.com/doc/refman/5.7/en/option-files.html'\fI\%MySQL Options File\fP\X'tty: link' or similar files for other systems.
 .sp
 \fBNOTE:\fP
 .INDENT 0.0
 .INDENT 3.5
-Using the \fB\-\-query\fP option may cause rounding (in Python 2) or introduce \fI\%Python floating point issues\fP (in Python 3).
+Using the \fB\-\-query\fP option may cause rounding (in Python 2) or introduce \X'tty: link https://docs.python.org/3/tutorial/floatingpoint.html'\fI\%Python floating point issues\fP\X'tty: link' (in Python 3).
 .UNINDENT
 .UNINDENT
 .sp
 \fBNOTE:\fP
 .INDENT 0.0
 .INDENT 3.5
 If the CSV file was created from a JSON file using \fI\%in2csv\fP, remember to quote SQL columns properly. For example:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 echo \(aq{\(dqa\(dq:{\(dqb\(dq:\(dqc\(dq},\(dqd\(dq:\(dqe\(dq}\(aq | in2csv \-f ndjson | csvsql \-\-query \(aqSELECT \(dqa/b\(dq FROM stdin\(aq
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .sp
 \fBNOTE:\fP
 .INDENT 0.0
 .INDENT 3.5
-Alternatives to \fI\%csvsql\fP are \fI\%q\fP and \fI\%textql\fP\&.
+Alternatives to \fI\%csvsql\fP are \X'tty: link https://github.com/harelba/q'\fI\%q\fP\X'tty: link' and \X'tty: link https://github.com/dinedal/textql'\fI\%textql\fP\X'tty: link'\&.
 .UNINDENT
 .UNINDENT
 .SH EXAMPLES
 .SS Generate SQL statements
 .sp
 Generate a statement in the PostgreSQL dialect:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvsql \-i postgresql examples/realdata/FY09_EDU_Recipients_by_State.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SS Interact with a SQL database
 .sp
 Create a table and import data from the CSV directly into PostgreSQL:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 createdb test
 csvsql \-\-db postgresql:///test \-\-tables fy09 \-\-insert examples/realdata/FY09_EDU_Recipients_by_State.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 For large tables it may not be practical to process the entire table. One solution to this is to analyze a sample of the table. In this case it can be useful to turn off length limits and null checks with the \fB\-\-no\-constraints\fP option:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 head \-n 20 examples/realdata/FY09_EDU_Recipients_by_State.csv | csvsql \-\-no\-constraints \-\-tables fy09
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Create tables for an entire directory of CSVs and import data from those files directly into PostgreSQL:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 createdb test
 csvsql \-\-db postgresql:///test \-\-insert examples/*_converted.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 If those CSVs have identical headers, you can import them into the same table by using \fI\%csvstack\fP first:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 createdb test
 csvstack examples/dummy?.csv | csvsql \-\-db postgresql:///test \-\-insert
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SS Query and output CSV files using SQL
 .sp
 You can use csvsql to \(dqdirectly\(dq query one or more CSV files. Please note that this will create an in\-memory SQLite database, so it won\(aqt be very fast:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvsql \-\-query  \(dqSELECT m.usda_id, avg(i.sepal_length) AS mean_sepal_length FROM iris AS i JOIN irismeta AS m ON (i.species = m.species) GROUP BY m.species\(dq examples/iris.csv examples/irismeta.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Group rows by one column:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvsql \-\-query \(dqSELECT * FROM \(aqdummy3\(aq GROUP BY a\(dq examples/dummy3.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Concatenate two columns:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvsql \-\-query \(dqSELECT a || b FROM \(aqdummy3\(aq\(dq \-\-no\-inference examples/dummy3.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 If a column contains null values, you must \fBCOALESCE\fP the column:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvsql \-\-query \(dqSELECT a || COALESCE(b, \(aq\(aq) FROM \(aqsort_ints_nulls\(aq\(dq \-\-no\-inference examples/sort_ints_nulls.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 The \fBUPDATE\fP SQL statement produces no output. Remember to \fBSELECT\fP the columns and rows you want:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvsql \-\-query \(dqUPDATE \(aqdummy3\(aq SET a = \(aqfoo\(aq; SELECT * FROM \(aqdummy3\(aq\(dq examples/dummy3.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH AUTHOR
 Christopher Groskopf and contributors
 .SH COPYRIGHT
 2016, Christopher Groskopf and James McKinney
 .\" Generated by docutils manpage writer.
```

### Comparing `csvkit-1.5.0/docs/_build/man/csvstack.1` & `csvkit-2.0.0/docs/_build/man/csvstack.1`

 * *Files 6% similar despite different names*

```diff
@@ -23,25 +23,24 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "CSVSTACK" "1" "Mar 28, 2024" "1.5.0" "csvkit"
+.TH "CSVSTACK" "1" "May 01, 2024" "2.0.0" "csvkit"
 .SH NAME
 csvstack \- csvstack Documentation
 .SH DESCRIPTION
 .sp
 Stack up the rows from multiple CSV files, optionally adding a grouping value to each row:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 usage: csvstack [\-h] [\-d DELIMITER] [\-t] [\-q QUOTECHAR] [\-u {0,1,2,3}] [\-b]
                 [\-p ESCAPECHAR] [\-z FIELD_SIZE_LIMIT] [\-e ENCODING] [\-S] [\-H]
                 [\-K SKIP_LINES] [\-v] [\-l] [\-\-zero] [\-V] [\-g GROUPS]
                 [\-n GROUP_NAME] [\-\-filenames]
                 [FILE [FILE ...]]
 
 Stack up the rows from multiple CSV files, optionally adding a grouping value.
@@ -58,16 +57,15 @@
                         added to the output as a new column. You may specify a
                         name for the new column using the \-n flag.
   \-n GROUP_NAME, \-\-group\-name GROUP_NAME
                         A name for the grouping column, e.g. \(dqyear\(dq. Only used
                         when also specifying \-g.
   \-\-filenames           Use the filename of each input file as its grouping
                         value. When specified, \-g will be ignored.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 See also: \fI\%Arguments common to all tools\fP\&.
 .sp
 \fBWARNING:\fP
 .INDENT 0.0
@@ -77,31 +75,27 @@
 .UNINDENT
 .SH EXAMPLES
 .sp
 Join a set of files for different years:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvstack \-g 2009,2010 examples/realdata/FY09_EDU_Recipients_by_State.csv examples/realdata/Datagov_FY10_EDU_recp_by_State.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Add a single column to the left of a CSV:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvstack \-n NEWCOL \-g \(dq\(dq examples/dummy.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH AUTHOR
 Christopher Groskopf and contributors
 .SH COPYRIGHT
 2016, Christopher Groskopf and James McKinney
 .\" Generated by docutils manpage writer.
```

### Comparing `csvkit-1.5.0/docs/_build/man/csvstat.1` & `csvkit-2.0.0/docs/_build/man/csvstat.1`

 * *Files 5% similar despite different names*

```diff
@@ -23,25 +23,24 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "CSVSTAT" "1" "Mar 28, 2024" "1.5.0" "csvkit"
+.TH "CSVSTAT" "1" "May 01, 2024" "2.0.0" "csvkit"
 .SH NAME
 csvstat \- csvstat Documentation
 .SH DESCRIPTION
 .sp
 Prints descriptive statistics for all columns in a CSV file. Will intelligently determine the type of each column and then print analysis relevant to that type (ranges for dates, mean and median for integers, etc.):
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 usage: csvstat [\-h] [\-d DELIMITER] [\-t] [\-q QUOTECHAR] [\-u {0,1,2,3}] [\-b]
                [\-p ESCAPECHAR] [\-z FIELD_SIZE_LIMIT] [\-e ENCODING] [\-L LOCALE]
                [\-S] [\-\-blanks] [\-\-null\-value NULL_VALUES [NULL_VALUES ...]]
                [\-\-date\-format DATE_FORMAT] [\-\-datetime\-format DATETIME_FORMAT]
                [\-H] [\-K SKIP_LINES] [\-v] [\-l] [\-\-zero] [\-V] [\-\-csv] [\-\-json]
                [\-i INDENT] [\-n] [\-c COLUMNS] [\-\-type] [\-\-nulls] [\-\-non\-nulls]
                [\-\-unique] [\-\-min] [\-\-max] [\-\-sum] [\-\-mean] [\-\-median]
@@ -92,66 +91,59 @@
                         Do not use grouping separators in decimal numbers.
   \-y SNIFF_LIMIT, \-\-snifflimit SNIFF_LIMIT
                         Limit CSV dialect sniffing to the specified number of
                         bytes. Specify \(dq0\(dq to disable sniffing entirely, or
                         \(dq\-1\(dq to sniff the entire file.
   \-I, \-\-no\-inference    Disable type inference when parsing the input. Disable
                         reformatting of values.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 See also: \fI\%Arguments common to all tools\fP\&.
 .SH EXAMPLES
 .sp
 Basic use:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvstat examples/realdata/FY09_EDU_Recipients_by_State.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 When an statistic name is passed, only that stat will be printed:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 $ csvstat \-\-min examples/realdata/FY09_EDU_Recipients_by_State.csv
   1. State Name: None
   2. State Abbreviate: None
   3. Code: 1
   4. Montgomery GI Bill\-Active Duty: 435
   5. Montgomery GI Bill\- Selective Reserve: 48
   6. Dependents\(aq Educational Assistance: 118
   7. Reserve Educational Assistance Program: 60
   8. Post\-Vietnam Era Veteran\(aqs Educational Assistance Program: 1
   9. TOTAL: 768
  10. j: None
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 If a single stat \fIand\fP a single column are requested, only a value will be returned:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 $ csvstat \-c 4 \-\-mean examples/realdata/FY09_EDU_Recipients_by_State.csv
 6,263.904
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH AUTHOR
 Christopher Groskopf and contributors
 .SH COPYRIGHT
 2016, Christopher Groskopf and James McKinney
 .\" Generated by docutils manpage writer.
```

### Comparing `csvkit-1.5.0/docs/_build/man/in2csv.1` & `csvkit-2.0.0/docs/_build/man/in2csv.1`

 * *Files 8% similar despite different names*

```diff
@@ -23,42 +23,39 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "IN2CSV" "1" "Mar 28, 2024" "1.5.0" "csvkit"
+.TH "IN2CSV" "1" "May 01, 2024" "2.0.0" "csvkit"
 .SH NAME
 in2csv \- in2csv Documentation
 .SH DESCRIPTION
 .sp
 Converts various tabular data formats into CSV.
 .sp
 Converting fixed width requires that you provide a schema file with the \(dq\-s\(dq option. The schema file should have the following format:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 column,start,length
 name,0,30
 birthday,30,10
 age,40,3
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 The header line is required though the columns may be in any order:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 usage: in2csv [\-h] [\-d DELIMITER] [\-t] [\-q QUOTECHAR] [\-u {0,1,2,3}] [\-b]
               [\-p ESCAPECHAR] [\-z FIELD_SIZE_LIMIT] [\-e ENCODING] [\-L LOCALE]
               [\-S] [\-\-blanks] [\-\-null\-value NULL_VALUES [NULL_VALUES ...]]
               [\-\-date\-format DATE_FORMAT] [\-\-datetime\-format DATETIME_FORMAT]
               [\-H] [\-K SKIP_LINES] [\-v] [\-l] [\-\-zero] [\-V]
               [\-f {csv,dbf,fixed,geojson,json,ndjson,xls,xlsx}] [\-s SCHEMA]
               [\-k KEY] [\-n] [\-\-sheet SHEET] [\-\-write\-sheets WRITE_SHEETS]
@@ -95,16 +92,15 @@
   \-y SNIFF_LIMIT, \-\-snifflimit SNIFF_LIMIT
                         Limit CSV dialect sniffing to the specified number of
                         bytes. Specify \(dq0\(dq to disable sniffing.
   \-I, \-\-no\-inference    Disable type inference (and \-\-locale, \-\-date\-format,
                         \-\-datetime\-format) when parsing CSV input.
 
  Some command\-line flags only pertain to specific input formats.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 See also: \fI\%Arguments common to all tools\fP\&.
 .sp
 \fBNOTE:\fP
 .INDENT 0.0
@@ -119,125 +115,109 @@
 If an XLS looks identical to an XLSX when viewed in Excel, they may not be identical as CSV. For example, XLSX has an integer type, but XLS doesn\(aqt. Numbers that look like integers from an XLS will have decimals in CSV, but those from an XLSX won\(aqt.
 .UNINDENT
 .UNINDENT
 .sp
 \fBNOTE:\fP
 .INDENT 0.0
 .INDENT 3.5
-To convert from HTML, consider \fI\%messytables\fP\&.
+To convert from HTML, consider \X'tty: link https://messytables.readthedocs.io/'\fI\%messytables\fP\X'tty: link'\&.
 .UNINDENT
 .UNINDENT
 .SH EXAMPLES
 .sp
 Convert the 2000 census geo headers file from fixed\-width to CSV and from latin\-1 encoding to utf8:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 in2csv \-e iso\-8859\-1 \-f fixed \-s examples/realdata/census_2000/census2000_geo_schema.csv examples/realdata/census_2000/usgeo_excerpt.upl
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 \fBNOTE:\fP
 .INDENT 0.0
 .INDENT 3.5
 A library of fixed\-width schemas is maintained in the \fBffs\fP project:
 .sp
-\fI\%https://github.com/wireservice/ffs\fP
+\X'tty: link https://github.com/wireservice/ffs'\fI\%https://github.com/wireservice/ffs\fP\X'tty: link'
 .UNINDENT
 .UNINDENT
 .sp
 Convert an Excel .xls file:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 in2csv examples/test.xls
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Standardize the formatting of a CSV file (quoting, line endings, etc.):
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 in2csv examples/realdata/FY09_EDU_Recipients_by_State.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Fetch csvkit\(aqs open issues from the GitHub API, convert the JSON response into a CSV and write it to a file:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 curl https://api.github.com/repos/wireservice/csvkit/issues?state=open | in2csv \-f json \-v
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Convert a DBase DBF file to an equivalent CSV:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 in2csv examples/testdbf.dbf
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 This tool names unnamed headers. To avoid that behavior, run:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 in2csv \-\-no\-header\-row examples/test.xlsx | tail \-n +2
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH TROUBLESHOOTING
 .sp
 If an error like the following occurs when providing an input file in CSV or Excel format:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 ValueError: Row 0 has 11 values, but Table only has 1 columns.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Then the input file might have initial rows before the header and data rows. You can skip such rows with \fB\-\-skip\-lines\fP (\fB\-K\fP):
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 in2csv \-\-skip\-lines 3 examples/test_skip_lines.csv
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
-If an XLSX file yields too few rows or too few columns, then the application that created the file might have \fI\%incorrectly set the worksheet\(aqs dimensions\fP\&. Try again with the \fB\-\-reset\-dimensions\fP option.
+If an XLSX file yields too few rows or too few columns, then the application that created the file might have \X'tty: link https://openpyxl.readthedocs.io/en/stable/optimized.html#worksheet-dimensions'\fI\%incorrectly set the worksheet\(aqs dimensions\fP\X'tty: link'\&. Try again with the \fB\-\-reset\-dimensions\fP option.
 .SH AUTHOR
 Christopher Groskopf and contributors
 .SH COPYRIGHT
 2016, Christopher Groskopf and James McKinney
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `csvkit-1.5.0/docs/_build/man/sql2csv.1` & `csvkit-2.0.0/docs/_build/man/sql2csv.1`

 * *Files 7% similar despite different names*

```diff
@@ -23,25 +23,24 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SQL2CSV" "1" "Mar 28, 2024" "1.5.0" "csvkit"
+.TH "SQL2CSV" "1" "May 01, 2024" "2.0.0" "csvkit"
 .SH NAME
 sql2csv \- sql2csv Documentation
 .SH DESCRIPTION
 .sp
 Executes arbitrary commands against a SQL database and outputs the results as a CSV:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 usage: sql2csv [\-h] [\-v] [\-l] [\-V] [\-\-db CONNECTION_STRING] [\-\-query QUERY]
                [\-e ENCODING] [\-H]
                [FILE]
 
 Execute an SQL query on a database and output the result to a CSV file.
 
 positional arguments:
@@ -53,68 +52,59 @@
   \-\-db CONNECTION_STRING
                         An sqlalchemy connection string to connect to a
                         database.
   \-\-query QUERY         The SQL query to execute. Overrides FILE and STDIN.
   \-e ENCODING, \-\-encoding ENCODING
                         Specify the encoding of the input query file.
   \-H, \-\-no\-header\-row   Do not output column names.
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH EXAMPLES
 .sp
 Load sample data into a table using \fI\%csvsql\fP and then query it using \fIsql2csv\fP:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 csvsql \-\-db \(dqsqlite:///dummy.db\(dq \-\-tables \(dqtest\(dq \-\-insert examples/dummy.csv
 sql2csv \-\-db \(dqsqlite:///dummy.db\(dq \-\-query \(dqselect * from test\(dq
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 Load data about financial aid recipients into PostgreSQL. Then find the three states that received the most, while also filtering out empty rows:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 createdb recipients
 csvsql \-\-db \(dqpostgresql:///recipients\(dq \-\-tables \(dqfy09\(dq \-\-insert examples/realdata/FY09_EDU_Recipients_by_State.csv
 sql2csv \-\-db \(dqpostgresql:///recipients\(dq \-\-query \(dqselect * from fy09 where \e\(dqState Name\e\(dq != \(aq\(aq order by fy09.\e\(dqTOTAL\e\(dq limit 3\(dq
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
 You can even use it as a simple SQL calculator (in this example an in\-memory SQLite database is used as the default):
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 sql2csv \-\-query \(dqselect 300 * 47 % 14 * 27 + 7000\(dq
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .sp
-The connection string \fI\%accepts parameters\fP\&. For example, to set the encoding of a MySQL database:
+The connection string \X'tty: link https://docs.sqlalchemy.org/en/rel_1_0/core/engines.html#engine-creation-api'\fI\%accepts parameters\fP\X'tty: link'\&. For example, to set the encoding of a MySQL database:
 .INDENT 0.0
 .INDENT 3.5
 .sp
-.nf
-.ft C
+.EX
 sql2csv \-\-db \(aqmysql://user:pass@host/database?charset=utf8\(aq \-\-query \(dqSELECT myfield FROM mytable\(dq
-.ft P
-.fi
+.EE
 .UNINDENT
 .UNINDENT
 .SH AUTHOR
 Christopher Groskopf and contributors
 .SH COPYRIGHT
 2016, Christopher Groskopf and James McKinney
 .\" Generated by docutils manpage writer.
```

### Comparing `csvkit-1.5.0/docs/cli.rst` & `csvkit-2.0.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/common_arguments.rst` & `csvkit-2.0.0/docs/common_arguments.rst`

 * *Files 9% similar despite different names*

```diff
@@ -9,22 +9,22 @@
    -d DELIMITER, --delimiter DELIMITER
                          Delimiting character of the input CSV file.
    -t, --tabs            Specify that the input CSV file is delimited with
                          tabs. Overrides "-d".
    -q QUOTECHAR, --quotechar QUOTECHAR
                          Character used to quote strings in the input CSV file.
    -u {0,1,2,3}, --quoting {0,1,2,3}
-                         Quoting style used in the input CSV file. 0 = Quote
-                         Minimal, 1 = Quote All, 2 = Quote Non-numeric, 3 =
-                         Quote None.
+                         Quoting style used in the input CSV file: 0 quote
+                         minimal, 1 quote all, 2 quote non-numeric, 3 quote
+                         none.
    -b, --no-doublequote  Whether or not double quotes are doubled in the input
                          CSV file.
    -p ESCAPECHAR, --escapechar ESCAPECHAR
                          Character used to escape the delimiter if --quoting 3
-                         ("Quote None") is specified and to escape the
+                         ("quote none") is specified and to escape the
                          QUOTECHAR if --no-doublequote is specified.
    -z FIELD_SIZE_LIMIT, --maxfieldsize FIELD_SIZE_LIMIT
                          Maximum length of a single field in the input CSV
                          file.
    -e ENCODING, --encoding ENCODING
                          Specify the encoding of the input CSV file.
    -L LOCALE, --locale LOCALE
```

### Comparing `csvkit-1.5.0/docs/conf.py` & `csvkit-2.0.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 sys.path.insert(0, os.path.abspath('..'))
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'csvkit'
 copyright = '2016, Christopher Groskopf and James McKinney'
-version = '1.5.0'
+version = '2.0.0'
 release = version
 
 # -- General configuration -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.autodoc',
```

### Comparing `csvkit-1.5.0/docs/contributing.rst` & `csvkit-2.0.0/docs/contributing.rst`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 For performance reasons tools should always offer streaming when possible. If a new feature would undermine streaming functionality it must be balanced against the utility of having a tool that can efficiently operate over large datasets.
 
 Currently, the following tools stream:
 
 * :doc:`/scripts/csvclean`
 * :doc:`/scripts/csvcut`
-* :doc:`/scripts/csvformat`
+* :doc:`/scripts/csvformat` unless :code:`--quoting 2` is set
 * :doc:`/scripts/csvgrep`
 * :doc:`/scripts/csvstack`
 * :doc:`/scripts/sql2csv`
 
 Currently, the following tools buffer:
 
 * :doc:`/scripts/csvjoin`
```

### Comparing `csvkit-1.5.0/docs/index.rst` & `csvkit-2.0.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,16 @@
    @Manual{csvkit,
      title = "csvkit",
      author = "Christopher Groskopf and contributors",
      year = "2016",
      url = "https://csvkit.readthedocs.org/"
    }
 
+.. _authors:
+
 Authors
 =======
 
 .. include:: ../AUTHORS.rst
 
 Indices and tables
 ==================
```

### Comparing `csvkit-1.5.0/docs/scripts/csvclean.rst` & `csvkit-2.0.0/docs/scripts/csvsort.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,60 @@
-========
-csvclean
-========
+=======
+csvsort
+=======
 
 Description
 ===========
 
-Cleans a CSV file of common syntax errors:
-
-* reports rows that have a different number of columns than the header row
-* attempts to correct the CSV by joining short rows into a single row
-
-Note that every csvkit tool does the following:
-
-* removes optional quote characters, unless the `--quoting` (`-u`) option is set to change this behavior
-* changes the field delimiter to a comma, if the input delimiter is set with the `--delimiter` (`-d`) or `--tabs` (`-t`) options
-* changes the record delimiter to a line feed (LF or ``\n``)
-* changes the quote character to a double-quotation mark, if the character is set with the `--quotechar` (`-q`) option
-* changes the character encoding to UTF-8, if the input encoding is set with the `--encoding` (`-e`) option
-
-Outputs [basename]_out.csv and [basename]_err.csv, the former containing all valid rows and the latter containing all error rows along with line numbers and descriptions:
+Sort CSV files. Like the Unix "sort" command, but for tabular data:
 
 .. code-block:: none
 
-   usage: csvclean [-h] [-d DELIMITER] [-t] [-q QUOTECHAR] [-u {0,1,2,3}] [-b]
-                   [-p ESCAPECHAR] [-z FIELD_SIZE_LIMIT] [-e ENCODING] [-S] [-H]
-                   [-K SKIP_LINES] [-v] [-l] [--zero] [-V] [-n]
-                   [FILE]
+   usage: csvsort [-h] [-d DELIMITER] [-t] [-q QUOTECHAR] [-u {0,1,2,3}] [-b]
+                  [-p ESCAPECHAR] [-z FIELD_SIZE_LIMIT] [-e ENCODING] [-L LOCALE]
+                  [-S] [--blanks] [--null-value NULL_VALUES [NULL_VALUES ...]]
+                  [--date-format DATE_FORMAT] [--datetime-format DATETIME_FORMAT]
+                  [-H] [-K SKIP_LINES] [-v] [-l] [--zero] [-V] [-n] [-c COLUMNS]
+                  [-r] [-i] [-y SNIFF_LIMIT] [-I]
+                  [FILE]
 
-   Fix common errors in a CSV file.
+   Sort CSV files. Like the Unix "sort" command, but for tabular data.
 
    positional arguments:
      FILE                  The CSV file to operate on. If omitted, will accept
                            input as piped data via STDIN.
 
    optional arguments:
      -h, --help            show this help message and exit
-     -n, --dry-run         Do not create output files. Information about what
-                           would have been done will be printed to STDERR.
+     -n, --names           Display column names and indices from the input CSV
+                           and exit.
+     -c COLUMNS, --columns COLUMNS
+                           A comma-separated list of column indices, names or
+                           ranges to sort by, e.g. "1,id,3-5". Defaults to all
+                           columns.
+     -r, --reverse         Sort in descending order.
+     -i, --ignore-case     Perform case-independent sorting.
+     -y SNIFF_LIMIT, --snifflimit SNIFF_LIMIT
+                           Limit CSV dialect sniffing to the specified number of
+                           bytes. Specify "0" to disable sniffing.
+     -I, --no-inference    Disable type inference when parsing the input.
 
 See also: :doc:`../common_arguments`.
 
+.. note::
+
+    If your file is large, try :code:`sort -t, file.csv` instead.
+
 Examples
 ========
 
-Test a file with known bad rows:
+Sort the veteran's education benefits table by the "TOTAL" column:
 
-.. code-block:: console
+.. code-block:: bash
 
-   $ csvclean -n examples/bad.csv
-   Line 1: Expected 3 columns, found 4 columns
-   Line 2: Expected 3 columns, found 2 columns
+   csvsort -c 9 examples/realdata/FY09_EDU_Recipients_by_State.csv
 
-To change the line ending from line feed (LF or ``\n``) to carriage return and line feed (CRLF or ``\r\n``) use:
+View the five states with the most individuals claiming veteran's education benefits:
 
 .. code-block:: bash
 
-   csvformat -M $'\r\n' examples/dummy.csv
+   csvcut -c 1,9 examples/realdata/FY09_EDU_Recipients_by_State.csv | csvsort -r -c 2 | head -n 5
```

### Comparing `csvkit-1.5.0/docs/scripts/csvcut.rst` & `csvkit-2.0.0/docs/scripts/csvcut.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/scripts/csvformat.rst` & `csvkit-2.0.0/docs/scripts/csvformat.rst`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 ===========
 
 Convert a CSV file to a custom output format.:
 
 .. code-block:: none
 
    usage: csvformat [-h] [-d DELIMITER] [-t] [-q QUOTECHAR] [-u {0,1,2,3}] [-b]
-                    [-p ESCAPECHAR] [-z FIELD_SIZE_LIMIT] [-e ENCODING] [-S] [-H]
-                    [-K SKIP_LINES] [-v] [-l] [--zero] [-V] [-E]
-                    [-D OUT_DELIMITER] [-T] [-A] [-Q OUT_QUOTECHAR]
+                    [-p ESCAPECHAR] [-z FIELD_SIZE_LIMIT] [-e ENCODING]
+                    [-L LOCALE] [-S] [-H] [-K SKIP_LINES] [-v] [-l] [--zero] [-V]
+                    [-E] [-D OUT_DELIMITER] [-T] [-A] [-Q OUT_QUOTECHAR]
                     [-U {0,1,2,3}] [-B] [-P OUT_ESCAPECHAR]
                     [-M OUT_LINETERMINATOR]
                     [FILE]
 
    Convert a CSV file to a custom output format.
 
    positional arguments:
@@ -32,17 +32,17 @@
                            Overrides "-D".
      -A, --out-asv         Specify that the output file is delimited with the
                            ASCII unit separator and record separator. Overrides
                            "-T", "-D" and "-M".
      -Q OUT_QUOTECHAR, --out-quotechar OUT_QUOTECHAR
                            Character used to quote strings in the output file.
      -U {0,1,2,3}, --out-quoting {0,1,2,3}
-                           Quoting style used in the output file. 0 = Quote
-                           Minimal, 1 = Quote All, 2 = Quote Non-numeric, 3 =
-                           Quote None.
+                           Quoting style used in the output file: 0 quote
+                           minimal, 1 quote all, 2 quote non-numeric, 3 quote
+                           none.
      -B, --out-no-doublequote
                            Whether or not double quotes are doubled in the output
                            CSV file.
      -P OUT_ESCAPECHAR, --out-escapechar OUT_ESCAPECHAR
                            Character used to escape the delimiter in the output
                            CSV file if --quoting 3 ("Quote None") is specified
                            and to escape the QUOTECHAR if --out-no-doublequote is
```

### Comparing `csvkit-1.5.0/docs/scripts/csvgrep.rst` & `csvkit-2.0.0/docs/scripts/csvgrep.rst`

 * *Files 5% similar despite different names*

```diff
@@ -67,12 +67,22 @@
 
 Perform a case-insensitive search:
 
 .. code-block:: bash
 
    csvgrep -c 1 -r "(?i)illinois" examples/realdata/FY09_EDU_Recipients_by_State.csv
 
+Remove comment rows:
+
+.. code-block:: bash
+
+   printf "a,b\n1,2\n# a comment\n3,4" | csvgrep --invert-match -c1 -r '^#'
+
 Get the indices of the columns that contain matching text (``\x1e`` is the `Record Separator (RS) character <https://en.wikipedia.org/wiki/C0_and_C1_control_codes#Field_separators>`_):
 
 .. code-block::
 
    csvgrep -m 22 -a -c 1- examples/realdata/FY09_EDU_Recipients_by_State.csv | csvformat -M $'\x1e' | xargs -d $'\x1e' -n1 sh -c 'echo $0 | csvcut -n' | grep 22
+
+.. note::
+
+   This last example is not performant.
```

### Comparing `csvkit-1.5.0/docs/scripts/csvjoin.rst` & `csvkit-2.0.0/docs/scripts/csvjoin.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/scripts/csvjson.rst` & `csvkit-2.0.0/docs/scripts/csvjson.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/scripts/csvlook.rst` & `csvkit-2.0.0/docs/scripts/csvlook.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/scripts/csvpy.rst` & `csvkit-2.0.0/docs/scripts/csvpy.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/scripts/csvsql.rst` & `csvkit-2.0.0/docs/scripts/csvsql.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/scripts/csvstack.rst` & `csvkit-2.0.0/docs/scripts/csvstack.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/scripts/csvstat.rst` & `csvkit-2.0.0/docs/scripts/csvstat.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/scripts/in2csv.rst` & `csvkit-2.0.0/docs/scripts/in2csv.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/scripts/sql2csv.rst` & `csvkit-2.0.0/docs/scripts/sql2csv.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/tricks.rst` & `csvkit-2.0.0/docs/tricks.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/tutorial/1_getting_started.rst` & `csvkit-2.0.0/docs/tutorial/1_getting_started.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/tutorial/2_examining_the_data.rst` & `csvkit-2.0.0/docs/tutorial/2_examining_the_data.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/tutorial/3_power_tools.rst` & `csvkit-2.0.0/docs/tutorial/3_power_tools.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/docs/tutorial/4_going_elsewhere.rst` & `csvkit-2.0.0/docs/tutorial/4_going_elsewhere.rst`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/dummy.xls` & `csvkit-2.0.0/examples/dummy.xls`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/dummy.xlsx` & `csvkit-2.0.0/examples/dummy.xlsx`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/iris.csv` & `csvkit-2.0.0/examples/iris.csv`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/Datagov_FY10_EDU_recp_by_State.csv` & `csvkit-2.0.0/examples/realdata/Datagov_FY10_EDU_recp_by_State.csv`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/FY09_EDU_Recipients_by_State.csv` & `csvkit-2.0.0/examples/realdata/FY09_EDU_Recipients_by_State.csv`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/acs2012_5yr_population.csv` & `csvkit-2.0.0/examples/realdata/acs2012_5yr_population.csv`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/census_2000/README.txt` & `csvkit-2.0.0/examples/realdata/census_2000/README.txt`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/census_2000/VROUTFSJ.TXt` & `csvkit-2.0.0/examples/realdata/census_2000/VROUTFSJ.TXt`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/census_2000/census2000_geo_schema.csv` & `csvkit-2.0.0/examples/realdata/census_2000/census2000_geo_schema.csv`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/census_2000/determination.csv` & `csvkit-2.0.0/examples/realdata/census_2000/determination.csv`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/census_2000/determination_schema.csv` & `csvkit-2.0.0/examples/realdata/census_2000/determination_schema.csv`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/census_2000/usgeo.upl` & `csvkit-2.0.0/examples/realdata/census_2000/usgeo.upl`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/census_2000/usgeo_excerpt.upl` & `csvkit-2.0.0/examples/realdata/census_2000/usgeo_excerpt.upl`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/census_2010/README.txt` & `csvkit-2.0.0/examples/realdata/census_2010/README.txt`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/census_2010/census2010_geo_schema.csv` & `csvkit-2.0.0/examples/realdata/census_2010/census2010_geo_schema.csv`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/census_2010/ilgeo2010_excerpt.csv` & `csvkit-2.0.0/examples/realdata/census_2010/ilgeo2010_excerpt.csv`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/census_2010/ilgeo2010_excerpt.pl` & `csvkit-2.0.0/examples/realdata/census_2010/ilgeo2010_excerpt.pl`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/event-notification-rpt-lastmonth.txt` & `csvkit-2.0.0/examples/realdata/event-notification-rpt-lastmonth.txt`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/ks_1033_data.csv` & `csvkit-2.0.0/examples/realdata/ks_1033_data.csv`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/realdata/ne_1033_data.xlsx` & `csvkit-2.0.0/examples/realdata/ne_1033_data.xlsx`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/sheets.xls` & `csvkit-2.0.0/examples/sheets.xls`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/sheets.xlsx` & `csvkit-2.0.0/examples/sheets.xlsx`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/test.xls` & `csvkit-2.0.0/examples/test.xls`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/test.xlsx` & `csvkit-2.0.0/examples/test.xlsx`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/test_geo.csv` & `csvkit-2.0.0/examples/test_geo.csv`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/test_geojson.json` & `csvkit-2.0.0/examples/test_geojson.json`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/test_skip_lines.xls` & `csvkit-2.0.0/examples/test_skip_lines.xls`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/test_skip_lines.xlsx` & `csvkit-2.0.0/examples/test_skip_lines.xlsx`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/testdbf.dbf` & `csvkit-2.0.0/examples/testdbf.dbf`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/testdbf_converted.csv` & `csvkit-2.0.0/examples/testdbf_converted.csv`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/testjson.json` & `csvkit-2.0.0/examples/testjson.json`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/examples/testjson_nested.json` & `csvkit-2.0.0/examples/testjson_nested.json`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/setup.py` & `csvkit-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='csvkit',
-    version='1.5.0',
+    version='2.0.0',
     description='A suite of command-line tools for working with CSV, the king of tabular file formats.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Christopher Groskopf and James McKinney',
     author_email='chrisgroskopf@gmail.com',
     url='https://github.com/wireservice/csvkit',
     license='MIT',
```

### Comparing `csvkit-1.5.0/tests/performance.py` & `csvkit-2.0.0/tests/performance.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/tests/test_cleanup.py` & `csvkit-2.0.0/tests/test_cleanup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,26 +8,26 @@
     def test_fix_rows(self):
         """Test to ensure that row merging yields correct results."""
         start = [['1', '2', '3'],
                  [''],
                  ['abc'],
                  ['4', '5'],
                  ]
-        fixed = join_rows(start)
+        fixed = join_rows(start, ' ')
         self.assertEqual(4, len(fixed))
         self.assertEqual(start[0][0], fixed[0])
         self.assertEqual(start[0][1], fixed[1])
         self.assertEqual(" ".join([start[0][-1], start[1][0], start[2][0], start[3][0]]), fixed[2])
         self.assertEqual(start[3][1], fixed[3])
 
     def test_real_world_join_fail(self):
         start = [['168772', '1102', '$0.23 TO $0.72', 'HOUR', '1.5%'],
                  ['GROSS', '1.5% '],
                  ['GROSS', '430938']]
-        fixed = join_rows(start)
+        fixed = join_rows(start, ' ')
         self.assertEqual(7, len(fixed))
         self.assertEqual(start[0][0], fixed[0])
         self.assertEqual(start[0][1], fixed[1])
         self.assertEqual(start[0][2], fixed[2])
         self.assertEqual(start[0][3], fixed[3])
         expected4 = " ".join([start[0][-1], start[1][0]])
         self.assertEqual(expected4, fixed[4])
```

### Comparing `csvkit-1.5.0/tests/test_cli.py` & `csvkit-2.0.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/tests/test_convert/test_convert.py` & `csvkit-2.0.0/tests/test_convert/test_convert.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/tests/test_convert/test_fixed.py` & `csvkit-2.0.0/tests/test_convert/test_fixed.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/tests/test_grep.py` & `csvkit-2.0.0/tests/test_grep.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/tests/test_utilities/test_csvclean.py` & `csvkit-2.0.0/tests/test_utilities/test_csvsort.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,112 +1,100 @@
 import io
-import os
 import sys
 from unittest.mock import patch
 
-from csvkit.utilities.csvclean import CSVClean, launch_new_instance
-from tests.utils import CSVKitTestCase, EmptyFileTests
+from csvkit.utilities.csvsort import CSVSort, launch_new_instance
+from tests.utils import ColumnsTests, CSVKitTestCase, EmptyFileTests, NamesTests, stdin_as_string
 
 
-class TestCSVClean(CSVKitTestCase, EmptyFileTests):
-    Utility = CSVClean
-
-    def tearDown(self):
-        output_file = "stdin_out.csv"
-        if os.path.isfile(output_file):
-            os.remove(output_file)
-
-    def assertCleaned(self, basename, output_lines, error_lines, additional_args=[]):
-        args = [f'examples/{basename}.csv'] + additional_args
-        output_file = io.StringIO()
-
-        utility = CSVClean(args, output_file)
-        utility.run()
-
-        output_file.close()
-
-        output_file = f'examples/{basename}_out.csv'
-        error_file = f'examples/{basename}_err.csv'
-
-        self.assertEqual(os.path.exists(output_file), bool(output_lines))
-        self.assertEqual(os.path.exists(error_file), bool(error_lines))
-
-        try:
-            if output_lines:
-                with open(output_file) as f:
-                    for line in output_lines:
-                        self.assertEqual(next(f), line)
-                    self.assertRaises(StopIteration, next, f)
-            if error_lines:
-                with open(error_file) as f:
-                    for line in error_lines:
-                        self.assertEqual(next(f), line)
-                    self.assertRaises(StopIteration, next, f)
-        finally:
-            if output_lines:
-                os.remove(output_file)
-            if error_lines:
-                os.remove(error_file)
+class TestCSVSort(CSVKitTestCase, ColumnsTests, EmptyFileTests, NamesTests):
+    Utility = CSVSort
 
     def test_launch_new_instance(self):
-        with patch.object(sys, 'argv', [self.Utility.__name__.lower(), 'examples/bad.csv']):
+        with patch.object(sys, 'argv', [self.Utility.__name__.lower(), 'examples/dummy.csv']):
             launch_new_instance()
 
-    def test_skip_lines(self):
-        self.assertCleaned('bad_skip_lines', [
-            'column_a,column_b,column_c\n',
-            '0,mixed types.... uh oh,17\n',
-        ], [
-            'line_number,msg,column_a,column_b,column_c\n',
-            '1,"Expected 3 columns, found 4 columns",1,27,,I\'m too long!\n',
-            '2,"Expected 3 columns, found 2 columns",,I\'m too short!\n',
-        ], ['--skip-lines', '3'])
-
-    def test_simple(self):
-        self.assertCleaned('bad', [
-            'column_a,column_b,column_c\n',
-            '0,mixed types.... uh oh,17\n',
-        ], [
-            'line_number,msg,column_a,column_b,column_c\n',
-            '1,"Expected 3 columns, found 4 columns",1,27,,I\'m too long!\n',
-            '2,"Expected 3 columns, found 2 columns",,I\'m too short!\n',
+    def test_runs(self):
+        self.assertRows(['examples/test_utf8.csv'], [
+            ['foo', 'bar', 'baz'],
+            ['1', '2', '3'],
+            ['4', '5', 'ʤ'],
+        ])
+
+    def test_encoding(self):
+        self.assertRows(['-e', 'latin1', 'examples/test_latin1.csv'], [
+            ['a', 'b', 'c'],
+            ['1', '2', '3'],
+            ['4', '5', '©'],
+        ])
+
+    def test_sort_string_reverse(self):
+        reader = self.get_output_as_reader(['-c', '1', '-r', 'examples/testxls_converted.csv'])
+        test_order = ['text', 'Unicode! Σ', 'This row has blanks',
+                      'Chicago Tribune', 'Chicago Sun-Times', 'Chicago Reader']
+        new_order = [str(r[0]) for r in reader]
+        self.assertEqual(test_order, new_order)
+
+    def test_sort_date(self):
+        reader = self.get_output_as_reader(['-c', '2', 'examples/testxls_converted.csv'])
+        test_order = ['text', 'Chicago Tribune', 'Chicago Sun-Times',
+                      'Chicago Reader', 'This row has blanks', 'Unicode! Σ']
+        new_order = [str(r[0]) for r in reader]
+        self.assertEqual(test_order, new_order)
+
+    def test_ignore_case(self):
+        self.assertRows(['-i', 'examples/test_ignore_case.csv'], [
+            ['a', 'b', 'c'],
+            ['3', '2009-01-01', 'd'],
+            ['20', '2001-01-01', 'c'],
+            ['20', '2002-01-01', 'b'],
+            ['100', '2003-01-01', 'a'],
+            ['100', '2003-01-01', 'A'],
         ])
 
+    def test_no_blanks(self):
+        reader = self.get_output_as_reader(['examples/blanks.csv'])
+        test_order = [
+            ['a', 'b', 'c', 'd', 'e', 'f'],
+            ['', '', '', '', '', ''],
+        ]
+        new_order = list(reader)
+        self.assertEqual(test_order, new_order)
+
+    def test_blanks(self):
+        reader = self.get_output_as_reader(['--blanks', 'examples/blanks.csv'])
+        test_order = [
+            ['a', 'b', 'c', 'd', 'e', 'f'],
+            ['', 'NA', 'N/A', 'NONE', 'NULL', '.'],
+        ]
+        new_order = list(reader)
+        self.assertEqual(test_order, new_order)
+
     def test_no_header_row(self):
-        self.assertCleaned('no_header_row', [
-            '1,2,3\n',
-        ], [])
-
-    def test_removes_optional_quote_characters(self):
-        self.assertCleaned('optional_quote_characters', [
-            'a,b,c\n',
-            '1,2,3\n',
-        ], [])
-
-    def test_changes_line_endings(self):
-        self.assertCleaned('mac_newlines', [
-            'a,b,c\n',
-            '1,2,3\n',
-            '"Once upon\n',
-            'a time",5,6\n',
-        ], [])
-
-    def test_changes_character_encoding(self):
-        self.assertCleaned('test_latin1', [
-            'a,b,c\n',
-            '1,2,3\n',
-            '4,5,©\n',
-        ], [], ['-e', 'latin1'])
-
-    def test_removes_bom(self):
-        self.assertCleaned('test_utf8_bom', [
-            'foo,bar,baz\n',
-            '1,2,3\n',
-            '4,5,ʤ\n',
-        ], [], [])
-
-    def test_dry_run(self):
-        output = self.get_output_as_io(['-n', 'examples/bad.csv'])
-        self.assertFalse(os.path.exists('examples/bad_err.csv'))
-        self.assertFalse(os.path.exists('examples/bad_out.csv'))
-        self.assertEqual(next(output)[:6], 'Line 1')
-        self.assertEqual(next(output)[:6], 'Line 2')
+        self.assertRows(['--no-header-row', '--no-inference', 'examples/no_header_row.csv'], [
+            ['a', 'b', 'c'],
+            ['1', '2', '3'],
+        ])
+
+    def test_no_inference(self):
+        reader = self.get_output_as_reader(['--no-inference', '-c', '1', 'examples/test_literal_order.csv'])
+        test_order = ['a', '192', '27', '3']
+        new_order = [str(r[0]) for r in reader]
+        self.assertEqual(test_order, new_order)
+
+    def test_sort_t_and_nulls(self):
+        reader = self.get_output_as_reader(['-c', '2', 'examples/sort_ints_nulls.csv'])
+        test_order = ['b', '1', '2', '']
+        new_order = [str(r[1]) for r in reader]
+        self.assertEqual(test_order, new_order)
+
+    def test_stdin(self):
+        input_file = io.BytesIO(b'a,b,c\n4,5,6\n1,2,3\n')
+
+        with stdin_as_string(input_file):
+            self.assertLines([], [
+                'a,b,c',
+                '1,2,3',
+                '4,5,6',
+            ])
+
+        input_file.close()
```

### Comparing `csvkit-1.5.0/tests/test_utilities/test_csvcut.py` & `csvkit-2.0.0/tests/test_utilities/test_csvcut.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/tests/test_utilities/test_csvgrep.py` & `csvkit-2.0.0/tests/test_utilities/test_csvgrep.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,22 @@
     default_args = ['-c', '1', '-m', '1']
     columns_args = ['-m', '1']
 
     def test_launch_new_instance(self):
         with patch.object(sys, 'argv', [self.Utility.__name__.lower()] + self.default_args + ['examples/dummy.csv']):
             launch_new_instance()
 
+    def test_options(self):
+        for args, message in (
+            ([], 'You must specify at least one column to search using the -c option.'),
+            (['-c', '1'], 'One of -r, -m or -f must be specified, unless using the -n option.'),
+        ):
+            with self.subTest(args=args):
+                self.assertError(launch_new_instance, args, message)
+
     def test_skip_lines(self):
         self.assertRows(['--skip-lines', '3', '-c', '1', '-m', '1', 'examples/test_skip_lines.csv'], [
             ['a', 'b', 'c'],
             ['1', '2', '3'],
         ])
 
     def test_match(self):
```

### Comparing `csvkit-1.5.0/tests/test_utilities/test_csvjoin.py` & `csvkit-2.0.0/tests/test_utilities/test_csvjoin.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,35 @@
     Utility = CSVJoin
     default_args = ['examples/dummy.csv', '-']
 
     def test_launch_new_instance(self):
         with patch.object(sys, 'argv', [self.Utility.__name__.lower(), 'examples/join_a.csv', 'examples/join_b.csv']):
             launch_new_instance()
 
+    def test_options(self):
+        for args, message in (
+            (
+                ['-c' '1,2'],
+                'The number of join column names must match the number of files, '
+                'or be a single column name that exists in all files.',
+            ),
+            (['-c', '1', '--left', '--right'], 'It is not valid to specify both a left and a right join.'),
+        ):
+            with self.subTest(args=args):
+                self.assertError(launch_new_instance, args, message)
+
+    def test_join_options(self):
+        for option in ('--left', '--right', '--outer'):
+            with self.subTest(option=option):
+                self.assertError(
+                    launch_new_instance,
+                    [option],
+                    'You must provide join column names when performing an outer join.',
+                )
+
     def test_sequential(self):
         output = self.get_output_as_io(['examples/join_a.csv', 'examples/join_b.csv'])
         self.assertEqual(len(output.readlines()), 4)
 
     def test_inner(self):
         output = self.get_output_as_io(['-c', 'a', 'examples/join_a.csv', 'examples/join_b.csv'])
         self.assertEqual(len(output.readlines()), 3)
```

### Comparing `csvkit-1.5.0/tests/test_utilities/test_csvjson.py` & `csvkit-2.0.0/tests/test_utilities/test_csvjson.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,32 @@
 class TestCSVJSON(CSVKitTestCase, EmptyFileTests):
     Utility = CSVJSON
 
     def test_launch_new_instance(self):
         with patch.object(sys, 'argv', [self.Utility.__name__.lower(), 'examples/dummy.csv']):
             launch_new_instance()
 
+    def test_options(self):
+        self.assertError(
+            launch_new_instance,
+            ['--key', 'value', '--stream'],
+            '--key is only allowed with --stream when --lat and --lon are also specified.',
+        )
+
+    def test_latlon_options(self):
+        for option, message in (
+            ('lat', '--lon is required whenever --lat is specified.'),
+            ('lon', '--lat is required whenever --lon is specified.'),
+            ('crs', '--crs is only allowed when --lat and --lon are also specified.'),
+            ('type', '--type is only allowed when --lat and --lon are also specified.'),
+            ('geometry', '--geometry is only allowed when --lat and --lon are also specified.'),
+        ):
+            with self.subTest(option=option):
+                self.assertError(launch_new_instance, [f'--{option}', 'value'], message)
+
     def test_simple(self):
         js = json.loads(self.get_output(['examples/dummy.csv']))
         self.assertDictEqual(js[0], {'a': True, 'c': 3.0, 'b': 2.0})
 
     def test_sniff_limit(self):
         js = json.loads(self.get_output(['examples/sniff_limit.csv']))
         self.assertDictEqual(js[0], {'a': True, 'c': 3.0, 'b': 2.0})
```

### Comparing `csvkit-1.5.0/tests/test_utilities/test_csvlook.py` & `csvkit-2.0.0/tests/test_utilities/test_csvlook.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/tests/test_utilities/test_csvsql.py` & `csvkit-2.0.0/tests/test_utilities/test_csvsql.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,52 @@
 class TestCSVSQL(CSVKitTestCase, EmptyFileTests):
     Utility = CSVSQL
 
     def test_launch_new_instance(self):
         with patch.object(sys, 'argv', [self.Utility.__name__.lower(), 'examples/dummy.csv']):
             launch_new_instance()
 
+    def test_options(self):
+        for args, message in (
+            (
+                ['--db', 'sqlite:///:memory:', '--dialect', 'sqlite'],
+                'The --dialect option is only valid when neither --db nor --query are specified.',
+            ),
+            (
+                ['--insert'],
+                'The --insert option is only valid when either --db or --query is specified.',
+            ),
+            (
+                ['--db', 'sqlite:///:memory:', '--insert', '--no-create', '--overwrite'],
+                'The --overwrite option is only valid if --no-create is not specified.',
+            ),
+            (
+                ['--db', 'sqlite:///:memory:', '--insert', '--no-create', '--create-if-not-exists'],
+                'The --no-create and --create-if-not-exists options are mutually exclusive.',
+            ),
+        ):
+            with self.subTest(args=args):
+                self.assertError(launch_new_instance, args, message)
+
+    def test_insert_options(self):
+        for args in (
+            ['--no-create'],
+            ['--create-if-not-exists'],
+            ['--overwrite'],
+            ['--before-insert'],
+            ['--after-insert'],
+            ['--chunk-size', '1'],
+        ):
+            with self.subTest(args=args):
+                self.assertError(
+                    launch_new_instance,
+                    args,
+                    f'The {args[0]} option is only valid if --insert is also specified.'
+                )
+
     def setUp(self):
         self.db_file = 'foo.db'
 
     def tearDown(self):
         if os.path.exists(self.db_file):
             os.remove(self.db_file)
```

### Comparing `csvkit-1.5.0/tests/test_utilities/test_csvstack.py` & `csvkit-2.0.0/tests/test_utilities/test_csvstack.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,21 @@
     Utility = CSVStack
     default_args = ['-']
 
     def test_launch_new_instance(self):
         with patch.object(sys, 'argv', [self.Utility.__name__.lower(), 'examples/dummy.csv']):
             launch_new_instance()
 
+    def test_options(self):
+        self.assertError(
+            launch_new_instance,
+            ['-g', '1,2'],
+            'The number of grouping values must be equal to the number of CSV files being stacked.',
+        )
+
     def test_skip_lines(self):
         self.assertRows(['--skip-lines', '3', 'examples/test_skip_lines.csv', 'examples/test_skip_lines.csv'], [
             ['a', 'b', 'c'],
             ['1', '2', '3'],
             ['1', '2', '3'],
         ])
```

### Comparing `csvkit-1.5.0/tests/test_utilities/test_csvstat.py` & `csvkit-2.0.0/tests/test_utilities/test_csvstat.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,30 @@
 class TestCSVStat(CSVKitTestCase, ColumnsTests, EmptyFileTests, NamesTests):
     Utility = CSVStat
 
     def test_launch_new_instance(self):
         with patch.object(sys, 'argv', [self.Utility.__name__.lower(), 'examples/dummy.csv']):
             launch_new_instance()
 
+    def test_options(self):
+        self.assertError(
+            launch_new_instance,
+            ['--min', '--max'],
+            'Only one operation argument may be specified (--mean, --median, etc).',
+        )
+
+    def test_format_options(self):
+        for option in ('csv', 'json', 'count'):
+            with self.subTest(option=option):
+                self.assertError(
+                    launch_new_instance,
+                    ['--min', f'--{option}'],
+                    f'You may not specify --{option} and an operation (--mean, --median, etc) at the same time.',
+                )
+
     def test_runs(self):
         # Test that csvstat doesn't error on UTF-8 input.
         self.get_output(['examples/test_utf8.csv'])
 
     def test_encoding(self):
         # Test that csvstat doesn't error on Latin-1 input.
         self.get_output(['-e', 'latin1', 'examples/test_latin1.csv'])
```

### Comparing `csvkit-1.5.0/tests/test_utilities/test_in2csv.py` & `csvkit-2.0.0/tests/test_utilities/test_in2csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,41 @@
 
     def test_version(self):
         with self.assertRaises(SystemExit) as e:
             self.get_output(['-V'])
 
         self.assertEqual(e.exception.code, 0)
 
+    def test_args(self):
+        for args in ([], ['-']):
+            with self.subTest(args=args):
+                self.assertError(
+                    launch_new_instance,
+                    [],
+                    'You must specify a format when providing input as piped data via STDIN.',
+                    args=args,
+                )
+
+    def test_options(self):
+        for options, args, message in (
+            (
+                [],
+                ['dummy.unknown'],
+                'Unable to automatically determine the format of the input file. '
+                'Try specifying a format with --format.',
+            ),
+            (
+                ['-n'],
+                ['dummy.csv'],
+                'You cannot use the -n or --names options with non-Excel files.',
+            ),
+        ):
+            with self.subTest(args=options + args):
+                self.assertError(launch_new_instance, options, message, args=args)
+
     def test_locale(self):
         self.assertConverted('csv', 'examples/test_locale.csv',
                              'examples/test_locale_converted.csv', ['--locale', 'de_DE'])
 
     def test_no_blanks(self):
         self.assertConverted('csv', 'examples/blanks.csv', 'examples/blanks_converted.csv')
```

### Comparing `csvkit-1.5.0/tests/test_utilities/test_sql2csv.py` & `csvkit-2.0.0/tests/test_utilities/test_sql2csv.py`

 * *Files identical despite different names*

### Comparing `csvkit-1.5.0/tests/utils.py` & `csvkit-2.0.0/tests/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 """
 
 import io
 import sys
 import unittest
 import warnings
-from contextlib import contextmanager
+from contextlib import contextmanager, redirect_stderr
+from unittest.mock import patch
 
 import agate
 
 from csvkit.exceptions import ColumnIdentifierError, RequiredHeaderError
 
 
 @contextmanager
@@ -35,15 +36,15 @@
     yield
     sys.stderr = temp
 
 
 @contextmanager
 def stdin_as_string(content):
     temp = sys.stdin
-    sys.stdin = io.TextIOWrapper(content)
+    sys.stdin = io.TextIOWrapper(io.BufferedReader(content))
     yield
     sys.stdin = temp
 
 
 class CSVKitTestCase(unittest.TestCase):
     warnings.filterwarnings(action='ignore', module='agate')
 
@@ -63,14 +64,29 @@
 
     def get_output_as_list(self, args):
         return self.get_output(args).split('\n')
 
     def get_output_as_reader(self, args):
         return agate.csv.reader(self.get_output_as_io(args))
 
+    def assertError(self, launch_new_instance, options, message, args=None):
+        command = self.Utility.__name__.lower()
+
+        if args is None:
+            args = ['examples/dummy.csv']
+
+        f = io.StringIO()
+        with redirect_stderr(f):
+            with patch.object(sys, 'argv', [command] + options + args):
+                with self.assertRaises(SystemExit) as e:
+                    launch_new_instance()
+
+        self.assertEqual(e.exception.code, 2)
+        self.assertEqual(f.getvalue().splitlines()[-1], f'{command}: error: {message}')
+
     def assertRows(self, args, rows):
         reader = self.get_output_as_reader(args)
 
         for row in rows:
             self.assertEqual(next(reader), row)
 
         self.assertRaises(StopIteration, next, reader)
```

