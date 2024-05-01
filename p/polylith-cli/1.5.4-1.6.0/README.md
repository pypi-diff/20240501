# Comparing `tmp/polylith_cli-1.5.4.tar.gz` & `tmp/polylith_cli-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polylith_cli-1.5.4.tar", max compression
+gzip compressed data, was "polylith_cli-1.6.0.tar", max compression
```

## Comparing `polylith_cli-1.5.4.tar` & `polylith_cli-1.6.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     4873 2024-02-09 08:50:51.459764 polylith_cli-1.5.4/README.md
--rw-r--r--   0        0        0       84 2024-04-25 07:49:10.693931 polylith_cli-1.5.4/polylith_cli/polylith/alias/__init__.py
--rw-r--r--   0        0        0      620 2024-01-16 09:46:59.989578 polylith_cli-1.5.4/polylith_cli/polylith/alias/core.py
--rw-r--r--   0        0        0      249 2024-04-25 07:49:10.688415 polylith_cli-1.5.4/polylith_cli/polylith/bricks/__init__.py
--rw-r--r--   0        0        0      576 2024-04-25 07:49:10.689487 polylith_cli-1.5.4/polylith_cli/polylith/bricks/base.py
--rw-r--r--   0        0        0      986 2024-04-25 07:49:10.689977 polylith_cli-1.5.4/polylith_cli/polylith/bricks/brick.py
--rw-r--r--   0        0        0     1108 2024-04-25 07:49:10.689144 polylith_cli-1.5.4/polylith_cli/polylith/bricks/component.py
--rw-r--r--   0        0        0      109 2024-04-25 07:49:10.722700 polylith_cli-1.5.4/polylith_cli/polylith/check/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-25 07:49:10.722238 polylith_cli-1.5.4/polylith_cli/polylith/check/collect.py
--rw-r--r--   0        0        0     1051 2023-03-13 14:27:27.458511 polylith_cli-1.5.4/polylith_cli/polylith/check/grouping.py
--rw-r--r--   0        0        0     2811 2024-04-25 07:49:10.723790 polylith_cli-1.5.4/polylith_cli/polylith/check/report.py
--rw-r--r--   0        0        0       61 2024-04-25 07:49:10.700404 polylith_cli-1.5.4/polylith_cli/polylith/cli/__init__.py
--rw-r--r--   0        0        0       68 2024-04-25 07:49:10.702282 polylith_cli-1.5.4/polylith_cli/polylith/cli/__main__.py
--rw-r--r--   0        0        0     3956 2024-04-25 07:49:10.702109 polylith_cli-1.5.4/polylith_cli/polylith/cli/core.py
--rw-r--r--   0        0        0     2210 2024-04-25 07:49:10.700262 polylith_cli-1.5.4/polylith_cli/polylith/cli/create.py
--rw-r--r--   0        0        0      647 2024-02-15 14:19:22.606210 polylith_cli-1.5.4/polylith_cli/polylith/cli/options.py
--rw-r--r--   0        0        0      156 2024-04-25 07:49:10.716363 polylith_cli-1.5.4/polylith_cli/polylith/commands/__init__.py
--rw-r--r--   0        0        0     1196 2024-04-25 07:49:10.715849 polylith_cli-1.5.4/polylith_cli/polylith/commands/check.py
--rw-r--r--   0        0        0      645 2024-04-25 07:49:10.716199 polylith_cli-1.5.4/polylith_cli/polylith/commands/create.py
--rw-r--r--   0        0        0     1385 2024-04-25 07:49:10.715292 polylith_cli-1.5.4/polylith_cli/polylith/commands/deps.py
--rw-r--r--   0        0        0     1497 2024-04-25 07:49:10.717008 polylith_cli-1.5.4/polylith_cli/polylith/commands/diff.py
--rw-r--r--   0        0        0      679 2024-04-25 07:49:10.717369 polylith_cli-1.5.4/polylith_cli/polylith/commands/info.py
--rw-r--r--   0        0        0     1596 2024-04-25 07:49:10.718106 polylith_cli-1.5.4/polylith_cli/polylith/commands/libs.py
--rw-r--r--   0        0        0      628 2024-04-25 07:49:10.714539 polylith_cli-1.5.4/polylith_cli/polylith/commands/sync.py
--rw-r--r--   0        0        0      558 2024-04-25 07:49:10.690442 polylith_cli-1.5.4/polylith_cli/polylith/configuration/__init__.py
--rw-r--r--   0        0        0     2184 2024-04-25 07:49:10.691482 polylith_cli-1.5.4/polylith_cli/polylith/configuration/core.py
--rw-r--r--   0        0        0      202 2024-04-25 07:49:10.711454 polylith_cli-1.5.4/polylith_cli/polylith/deps/__init__.py
--rw-r--r--   0        0        0      681 2024-04-25 07:49:10.711775 polylith_cli-1.5.4/polylith_cli/polylith/deps/core.py
--rw-r--r--   0        0        0     4479 2024-04-25 07:49:10.714110 polylith_cli-1.5.4/polylith_cli/polylith/deps/report.py
--rw-r--r--   0        0        0      109 2024-04-25 07:49:10.694907 polylith_cli-1.5.4/polylith_cli/polylith/development/__init__.py
--rw-r--r--   0        0        0      234 2024-04-25 07:49:10.695084 polylith_cli-1.5.4/polylith_cli/polylith/development/development.py
--rw-r--r--   0        0        0       86 2024-04-25 07:49:10.697599 polylith_cli-1.5.4/polylith_cli/polylith/diff/__init__.py
--rw-r--r--   0        0        0     2247 2024-04-25 07:49:10.697450 polylith_cli-1.5.4/polylith_cli/polylith/diff/collect.py
--rw-r--r--   0        0        0     2141 2024-04-25 07:49:10.698555 polylith_cli-1.5.4/polylith_cli/polylith/diff/report.py
--rw-r--r--   0        0        0       79 2024-04-25 07:49:10.718509 polylith_cli-1.5.4/polylith_cli/polylith/dirs/__init__.py
--rw-r--r--   0        0        0      280 2024-04-25 07:49:10.718385 polylith_cli-1.5.4/polylith_cli/polylith/dirs/dirs.py
--rw-r--r--   0        0        0      339 2024-04-25 07:49:10.725850 polylith_cli-1.5.4/polylith_cli/polylith/distributions/__init__.py
--rw-r--r--   0        0        0     1018 2024-04-25 07:49:10.725677 polylith_cli-1.5.4/polylith_cli/polylith/distributions/collect.py
--rw-r--r--   0        0        0     1546 2024-01-22 14:07:16.217821 polylith_cli-1.5.4/polylith_cli/polylith/distributions/core.py
--rw-r--r--   0        0        0       83 2024-04-25 07:49:10.711295 polylith_cli-1.5.4/polylith_cli/polylith/files/__init__.py
--rw-r--r--   0        0        0      145 2022-11-04 07:17:35.623526 polylith_cli-1.5.4/polylith_cli/polylith/files/files.py
--rw-r--r--   0        0        0      162 2024-04-25 07:49:10.698741 polylith_cli-1.5.4/polylith_cli/polylith/imports/__init__.py
--rw-r--r--   0        0        0     1730 2023-07-29 11:51:13.392045 polylith_cli-1.5.4/polylith_cli/polylith/imports/parser.py
--rw-r--r--   0        0        0      475 2024-04-25 07:49:10.709613 polylith_cli-1.5.4/polylith_cli/polylith/info/__init__.py
--rw-r--r--   0        0        0     1632 2024-04-25 07:49:10.709425 polylith_cli-1.5.4/polylith_cli/polylith/info/collect.py
--rw-r--r--   0        0        0     3039 2024-04-25 07:49:10.711035 polylith_cli-1.5.4/polylith_cli/polylith/info/report.py
--rw-r--r--   0        0        0      102 2024-04-25 07:49:10.693764 polylith_cli-1.5.4/polylith_cli/polylith/interface/__init__.py
--rw-r--r--   0        0        0      875 2024-04-25 07:49:10.693626 polylith_cli-1.5.4/polylith_cli/polylith/interface/interfaces.py
--rw-r--r--   0        0        0      225 2024-04-25 07:49:10.703715 polylith_cli-1.5.4/polylith_cli/polylith/libs/__init__.py
--rw-r--r--   0        0        0     1400 2024-04-25 07:49:10.703554 polylith_cli-1.5.4/polylith_cli/polylith/libs/grouping.py
--rw-r--r--   0        0        0     5887 2024-04-25 07:49:10.706985 polylith_cli-1.5.4/polylith_cli/polylith/libs/report.py
--rw-r--r--   0        0        0     4408 2024-01-16 08:29:38.285478 polylith_cli-1.5.4/polylith_cli/polylith/libs/stdlib.py
--rw-r--r--   0        0        0      410 2024-04-25 07:49:10.707692 polylith_cli-1.5.4/polylith_cli/polylith/project/__init__.py
--rw-r--r--   0        0        0      852 2024-04-25 07:49:10.707503 polylith_cli-1.5.4/polylith_cli/polylith/project/create.py
--rw-r--r--   0        0        0     1458 2024-04-25 07:49:10.708626 polylith_cli-1.5.4/polylith_cli/polylith/project/get.py
--rw-r--r--   0        0        0      433 2023-04-01 08:55:53.793395 polylith_cli-1.5.4/polylith_cli/polylith/project/parser.py
--rw-r--r--   0        0        0      944 2024-02-09 08:50:51.449381 polylith_cli-1.5.4/polylith_cli/polylith/project/templates.py
--rw-r--r--   0        0        0      153 2024-04-25 07:49:10.702898 polylith_cli-1.5.4/polylith_cli/polylith/readme/__init__.py
--rw-r--r--   0        0        0     1091 2024-04-25 07:49:10.702750 polylith_cli-1.5.4/polylith_cli/polylith/readme/readme.py
--rw-r--r--   0        0        0      525 2024-04-25 07:49:10.724038 polylith_cli-1.5.4/polylith_cli/polylith/repo/__init__.py
--rw-r--r--   0        0        0      852 2024-04-25 07:49:10.725178 polylith_cli-1.5.4/polylith_cli/polylith/repo/get.py
--rw-r--r--   0        0        0     1964 2024-02-09 08:50:51.451835 polylith_cli-1.5.4/polylith_cli/polylith/repo/repo.py
--rw-r--r--   0        0        0       69 2024-04-25 07:49:10.690237 polylith_cli-1.5.4/polylith_cli/polylith/reporting/__init__.py
--rw-r--r--   0        0        0      208 2024-02-15 14:02:37.811309 polylith_cli-1.5.4/polylith_cli/polylith/reporting/theme.py
--rw-r--r--   0        0        0      225 2024-04-25 07:49:10.721000 polylith_cli-1.5.4/polylith_cli/polylith/sync/__init__.py
--rw-r--r--   0        0        0     1031 2024-04-25 07:49:10.720834 polylith_cli-1.5.4/polylith_cli/polylith/sync/collect.py
--rw-r--r--   0        0        0      983 2024-04-25 07:49:10.721536 polylith_cli-1.5.4/polylith_cli/polylith/sync/report.py
--rw-r--r--   0        0        0     3901 2024-04-25 07:49:10.720315 polylith_cli-1.5.4/polylith_cli/polylith/sync/update.py
--rw-r--r--   0        0        0       82 2024-04-25 07:49:10.694308 polylith_cli-1.5.4/polylith_cli/polylith/test/__init__.py
--rw-r--r--   0        0        0      965 2024-04-25 07:49:10.694736 polylith_cli-1.5.4/polylith_cli/polylith/test/tests.py
--rw-r--r--   0        0        0      457 2024-04-25 07:49:10.691697 polylith_cli-1.5.4/polylith_cli/polylith/toml/__init__.py
--rw-r--r--   0        0        0     2918 2024-04-25 07:49:10.693161 polylith_cli-1.5.4/polylith_cli/polylith/toml/core.py
--rw-r--r--   0        0        0       87 2024-04-25 07:49:10.696225 polylith_cli-1.5.4/polylith_cli/polylith/workspace/__init__.py
--rw-r--r--   0        0        0     1198 2024-04-25 07:49:10.695553 polylith_cli-1.5.4/polylith_cli/polylith/workspace/create.py
--rw-r--r--   0        0        0      937 2024-04-25 07:49:10.696082 polylith_cli-1.5.4/polylith_cli/polylith/workspace/paths.py
--rw-r--r--   0        0        0      605 2024-04-25 07:49:10.687924 polylith_cli-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     5668 1970-01-01 00:00:00.000000 polylith_cli-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     4873 2024-02-09 08:50:51.459764 polylith_cli-1.6.0/README.md
+-rw-r--r--   0        0        0       84 2024-05-01 07:10:35.940103 polylith_cli-1.6.0/polylith_cli/polylith/alias/__init__.py
+-rw-r--r--   0        0        0      620 2024-01-16 09:46:59.989578 polylith_cli-1.6.0/polylith_cli/polylith/alias/core.py
+-rw-r--r--   0        0        0      249 2024-05-01 07:10:35.934194 polylith_cli-1.6.0/polylith_cli/polylith/bricks/__init__.py
+-rw-r--r--   0        0        0      576 2024-05-01 07:10:35.935471 polylith_cli-1.6.0/polylith_cli/polylith/bricks/base.py
+-rw-r--r--   0        0        0      986 2024-05-01 07:10:35.935982 polylith_cli-1.6.0/polylith_cli/polylith/bricks/brick.py
+-rw-r--r--   0        0        0     1108 2024-05-01 07:10:35.935073 polylith_cli-1.6.0/polylith_cli/polylith/bricks/component.py
+-rw-r--r--   0        0        0      109 2024-05-01 07:10:35.968361 polylith_cli-1.6.0/polylith_cli/polylith/check/__init__.py
+-rw-r--r--   0        0        0     1343 2024-05-01 07:10:35.967883 polylith_cli-1.6.0/polylith_cli/polylith/check/collect.py
+-rw-r--r--   0        0        0     1051 2023-03-13 14:27:27.458511 polylith_cli-1.6.0/polylith_cli/polylith/check/grouping.py
+-rw-r--r--   0        0        0     2811 2024-05-01 07:10:35.969420 polylith_cli-1.6.0/polylith_cli/polylith/check/report.py
+-rw-r--r--   0        0        0       61 2024-05-01 07:10:35.946471 polylith_cli-1.6.0/polylith_cli/polylith/cli/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-01 07:10:35.948356 polylith_cli-1.6.0/polylith_cli/polylith/cli/__main__.py
+-rw-r--r--   0        0        0     3956 2024-05-01 07:10:35.948198 polylith_cli-1.6.0/polylith_cli/polylith/cli/core.py
+-rw-r--r--   0        0        0     2210 2024-05-01 07:10:35.946320 polylith_cli-1.6.0/polylith_cli/polylith/cli/create.py
+-rw-r--r--   0        0        0      647 2024-02-15 14:19:22.606210 polylith_cli-1.6.0/polylith_cli/polylith/cli/options.py
+-rw-r--r--   0        0        0      156 2024-05-01 07:10:35.962151 polylith_cli-1.6.0/polylith_cli/polylith/commands/__init__.py
+-rw-r--r--   0        0        0     1196 2024-05-01 07:10:35.961665 polylith_cli-1.6.0/polylith_cli/polylith/commands/check.py
+-rw-r--r--   0        0        0      645 2024-05-01 07:10:35.961996 polylith_cli-1.6.0/polylith_cli/polylith/commands/create.py
+-rw-r--r--   0        0        0     1385 2024-05-01 07:10:35.961116 polylith_cli-1.6.0/polylith_cli/polylith/commands/deps.py
+-rw-r--r--   0        0        0     1497 2024-05-01 07:10:35.962761 polylith_cli-1.6.0/polylith_cli/polylith/commands/diff.py
+-rw-r--r--   0        0        0      679 2024-05-01 07:10:35.963120 polylith_cli-1.6.0/polylith_cli/polylith/commands/info.py
+-rw-r--r--   0        0        0     1596 2024-05-01 07:10:35.963843 polylith_cli-1.6.0/polylith_cli/polylith/commands/libs.py
+-rw-r--r--   0        0        0      628 2024-05-01 07:10:35.960388 polylith_cli-1.6.0/polylith_cli/polylith/commands/sync.py
+-rw-r--r--   0        0        0      558 2024-05-01 07:10:35.936455 polylith_cli-1.6.0/polylith_cli/polylith/configuration/__init__.py
+-rw-r--r--   0        0        0     2184 2024-05-01 07:10:35.937494 polylith_cli-1.6.0/polylith_cli/polylith/configuration/core.py
+-rw-r--r--   0        0        0      202 2024-05-01 07:10:35.957371 polylith_cli-1.6.0/polylith_cli/polylith/deps/__init__.py
+-rw-r--r--   0        0        0      681 2024-05-01 07:10:35.957696 polylith_cli-1.6.0/polylith_cli/polylith/deps/core.py
+-rw-r--r--   0        0        0     4479 2024-05-01 07:10:35.959933 polylith_cli-1.6.0/polylith_cli/polylith/deps/report.py
+-rw-r--r--   0        0        0      109 2024-05-01 07:10:35.941053 polylith_cli-1.6.0/polylith_cli/polylith/development/__init__.py
+-rw-r--r--   0        0        0      234 2024-05-01 07:10:35.941225 polylith_cli-1.6.0/polylith_cli/polylith/development/development.py
+-rw-r--r--   0        0        0       86 2024-05-01 07:10:35.943690 polylith_cli-1.6.0/polylith_cli/polylith/diff/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-01 07:10:35.943531 polylith_cli-1.6.0/polylith_cli/polylith/diff/collect.py
+-rw-r--r--   0        0        0     2141 2024-05-01 07:10:35.944662 polylith_cli-1.6.0/polylith_cli/polylith/diff/report.py
+-rw-r--r--   0        0        0       79 2024-05-01 07:10:35.964235 polylith_cli-1.6.0/polylith_cli/polylith/dirs/__init__.py
+-rw-r--r--   0        0        0      280 2024-05-01 07:10:35.964119 polylith_cli-1.6.0/polylith_cli/polylith/dirs/dirs.py
+-rw-r--r--   0        0        0      339 2024-05-01 07:10:35.971252 polylith_cli-1.6.0/polylith_cli/polylith/distributions/__init__.py
+-rw-r--r--   0        0        0     1018 2024-05-01 07:10:35.971106 polylith_cli-1.6.0/polylith_cli/polylith/distributions/collect.py
+-rw-r--r--   0        0        0     1546 2024-01-22 14:07:16.217821 polylith_cli-1.6.0/polylith_cli/polylith/distributions/core.py
+-rw-r--r--   0        0        0       83 2024-05-01 07:10:35.957214 polylith_cli-1.6.0/polylith_cli/polylith/files/__init__.py
+-rw-r--r--   0        0        0      145 2022-11-04 07:17:35.623526 polylith_cli-1.6.0/polylith_cli/polylith/files/files.py
+-rw-r--r--   0        0        0      162 2024-05-01 07:10:35.944849 polylith_cli-1.6.0/polylith_cli/polylith/imports/__init__.py
+-rw-r--r--   0        0        0     1730 2023-07-29 11:51:13.392045 polylith_cli-1.6.0/polylith_cli/polylith/imports/parser.py
+-rw-r--r--   0        0        0      475 2024-05-01 07:10:35.955575 polylith_cli-1.6.0/polylith_cli/polylith/info/__init__.py
+-rw-r--r--   0        0        0     1632 2024-05-01 07:10:35.955383 polylith_cli-1.6.0/polylith_cli/polylith/info/collect.py
+-rw-r--r--   0        0        0     3039 2024-05-01 07:10:35.956957 polylith_cli-1.6.0/polylith_cli/polylith/info/report.py
+-rw-r--r--   0        0        0      102 2024-05-01 07:10:35.939940 polylith_cli-1.6.0/polylith_cli/polylith/interface/__init__.py
+-rw-r--r--   0        0        0      875 2024-05-01 07:10:35.939794 polylith_cli-1.6.0/polylith_cli/polylith/interface/interfaces.py
+-rw-r--r--   0        0        0      225 2024-05-01 07:10:35.949768 polylith_cli-1.6.0/polylith_cli/polylith/libs/__init__.py
+-rw-r--r--   0        0        0     1400 2024-05-01 07:10:35.949602 polylith_cli-1.6.0/polylith_cli/polylith/libs/grouping.py
+-rw-r--r--   0        0        0     5887 2024-05-01 07:10:35.952975 polylith_cli-1.6.0/polylith_cli/polylith/libs/report.py
+-rw-r--r--   0        0        0     4408 2024-01-16 08:29:38.285478 polylith_cli-1.6.0/polylith_cli/polylith/libs/stdlib.py
+-rw-r--r--   0        0        0      410 2024-05-01 07:10:35.953695 polylith_cli-1.6.0/polylith_cli/polylith/project/__init__.py
+-rw-r--r--   0        0        0      852 2024-05-01 07:10:35.953512 polylith_cli-1.6.0/polylith_cli/polylith/project/create.py
+-rw-r--r--   0        0        0     1458 2024-05-01 07:10:35.954607 polylith_cli-1.6.0/polylith_cli/polylith/project/get.py
+-rw-r--r--   0        0        0      433 2023-04-01 08:55:53.793395 polylith_cli-1.6.0/polylith_cli/polylith/project/parser.py
+-rw-r--r--   0        0        0      944 2024-02-09 08:50:51.449381 polylith_cli-1.6.0/polylith_cli/polylith/project/templates.py
+-rw-r--r--   0        0        0      153 2024-05-01 07:10:35.948955 polylith_cli-1.6.0/polylith_cli/polylith/readme/__init__.py
+-rw-r--r--   0        0        0     1091 2024-05-01 07:10:35.948812 polylith_cli-1.6.0/polylith_cli/polylith/readme/readme.py
+-rw-r--r--   0        0        0      525 2024-05-01 07:10:35.969662 polylith_cli-1.6.0/polylith_cli/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      852 2024-05-01 07:10:35.970620 polylith_cli-1.6.0/polylith_cli/polylith/repo/get.py
+-rw-r--r--   0        0        0     1964 2024-02-09 08:50:51.451835 polylith_cli-1.6.0/polylith_cli/polylith/repo/repo.py
+-rw-r--r--   0        0        0       69 2024-05-01 07:10:35.936249 polylith_cli-1.6.0/polylith_cli/polylith/reporting/__init__.py
+-rw-r--r--   0        0        0      208 2024-02-15 14:02:37.811309 polylith_cli-1.6.0/polylith_cli/polylith/reporting/theme.py
+-rw-r--r--   0        0        0      225 2024-05-01 07:10:35.966677 polylith_cli-1.6.0/polylith_cli/polylith/sync/__init__.py
+-rw-r--r--   0        0        0     1031 2024-05-01 07:10:35.966505 polylith_cli-1.6.0/polylith_cli/polylith/sync/collect.py
+-rw-r--r--   0        0        0      983 2024-05-01 07:10:35.967203 polylith_cli-1.6.0/polylith_cli/polylith/sync/report.py
+-rw-r--r--   0        0        0     3901 2024-05-01 07:10:35.965996 polylith_cli-1.6.0/polylith_cli/polylith/sync/update.py
+-rw-r--r--   0        0        0       82 2024-05-01 07:10:35.940473 polylith_cli-1.6.0/polylith_cli/polylith/test/__init__.py
+-rw-r--r--   0        0        0      965 2024-05-01 07:10:35.940888 polylith_cli-1.6.0/polylith_cli/polylith/test/tests.py
+-rw-r--r--   0        0        0      457 2024-05-01 07:10:35.937721 polylith_cli-1.6.0/polylith_cli/polylith/toml/__init__.py
+-rw-r--r--   0        0        0     3244 2024-05-01 07:10:35.939309 polylith_cli-1.6.0/polylith_cli/polylith/toml/core.py
+-rw-r--r--   0        0        0       87 2024-05-01 07:10:35.942349 polylith_cli-1.6.0/polylith_cli/polylith/workspace/__init__.py
+-rw-r--r--   0        0        0     1198 2024-05-01 07:10:35.941685 polylith_cli-1.6.0/polylith_cli/polylith/workspace/create.py
+-rw-r--r--   0        0        0      937 2024-05-01 07:10:35.942203 polylith_cli-1.6.0/polylith_cli/polylith/workspace/paths.py
+-rw-r--r--   0        0        0      605 2024-05-01 07:10:35.933714 polylith_cli-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5668 1970-01-01 00:00:00.000000 polylith_cli-1.6.0/PKG-INFO
```

### Comparing `polylith_cli-1.5.4/README.md` & `polylith_cli-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/alias/core.py` & `polylith_cli-1.6.0/polylith_cli/polylith/alias/core.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/bricks/base.py` & `polylith_cli-1.6.0/polylith_cli/polylith/bricks/base.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/bricks/brick.py` & `polylith_cli-1.6.0/polylith_cli/polylith/bricks/brick.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/bricks/component.py` & `polylith_cli-1.6.0/polylith_cli/polylith/bricks/component.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/check/collect.py` & `polylith_cli-1.6.0/polylith_cli/polylith/check/collect.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/check/grouping.py` & `polylith_cli-1.6.0/polylith_cli/polylith/check/grouping.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/check/report.py` & `polylith_cli-1.6.0/polylith_cli/polylith/check/report.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/cli/core.py` & `polylith_cli-1.6.0/polylith_cli/polylith/cli/core.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/cli/create.py` & `polylith_cli-1.6.0/polylith_cli/polylith/cli/create.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/cli/options.py` & `polylith_cli-1.6.0/polylith_cli/polylith/cli/options.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/commands/check.py` & `polylith_cli-1.6.0/polylith_cli/polylith/commands/check.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/commands/create.py` & `polylith_cli-1.6.0/polylith_cli/polylith/commands/create.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/commands/deps.py` & `polylith_cli-1.6.0/polylith_cli/polylith/commands/deps.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/commands/diff.py` & `polylith_cli-1.6.0/polylith_cli/polylith/commands/diff.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/commands/info.py` & `polylith_cli-1.6.0/polylith_cli/polylith/commands/info.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/commands/libs.py` & `polylith_cli-1.6.0/polylith_cli/polylith/commands/libs.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/commands/sync.py` & `polylith_cli-1.6.0/polylith_cli/polylith/commands/sync.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/configuration/__init__.py` & `polylith_cli-1.6.0/polylith_cli/polylith/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/configuration/core.py` & `polylith_cli-1.6.0/polylith_cli/polylith/configuration/core.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/deps/core.py` & `polylith_cli-1.6.0/polylith_cli/polylith/deps/core.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/deps/report.py` & `polylith_cli-1.6.0/polylith_cli/polylith/deps/report.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/diff/collect.py` & `polylith_cli-1.6.0/polylith_cli/polylith/diff/collect.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/diff/report.py` & `polylith_cli-1.6.0/polylith_cli/polylith/diff/report.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/distributions/collect.py` & `polylith_cli-1.6.0/polylith_cli/polylith/distributions/collect.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/distributions/core.py` & `polylith_cli-1.6.0/polylith_cli/polylith/distributions/core.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/imports/parser.py` & `polylith_cli-1.6.0/polylith_cli/polylith/imports/parser.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/info/collect.py` & `polylith_cli-1.6.0/polylith_cli/polylith/info/collect.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/info/report.py` & `polylith_cli-1.6.0/polylith_cli/polylith/info/report.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/interface/interfaces.py` & `polylith_cli-1.6.0/polylith_cli/polylith/interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/libs/grouping.py` & `polylith_cli-1.6.0/polylith_cli/polylith/libs/grouping.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/libs/report.py` & `polylith_cli-1.6.0/polylith_cli/polylith/libs/report.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/libs/stdlib.py` & `polylith_cli-1.6.0/polylith_cli/polylith/libs/stdlib.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/project/create.py` & `polylith_cli-1.6.0/polylith_cli/polylith/project/create.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/project/get.py` & `polylith_cli-1.6.0/polylith_cli/polylith/project/get.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/project/templates.py` & `polylith_cli-1.6.0/polylith_cli/polylith/project/templates.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/readme/readme.py` & `polylith_cli-1.6.0/polylith_cli/polylith/readme/readme.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/repo/__init__.py` & `polylith_cli-1.6.0/polylith_cli/polylith/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/repo/get.py` & `polylith_cli-1.6.0/polylith_cli/polylith/repo/get.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/repo/repo.py` & `polylith_cli-1.6.0/polylith_cli/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/sync/collect.py` & `polylith_cli-1.6.0/polylith_cli/polylith/sync/collect.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/sync/report.py` & `polylith_cli-1.6.0/polylith_cli/polylith/sync/report.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/sync/update.py` & `polylith_cli-1.6.0/polylith_cli/polylith/sync/update.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/test/tests.py` & `polylith_cli-1.6.0/polylith_cli/polylith/test/tests.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/toml/core.py` & `polylith_cli-1.6.0/polylith_cli/polylith/toml/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,21 +53,28 @@
         version = v.get('version', '')
         name = k + str.replace(f'{extras}', "'", '') if extras else k
         parsed = {name: version}
     else:
         parsed = {k: v}
     return {**acc, **parsed}
 
+def get_pep_621_optional_dependencies(data) -> List[str]:
+    groups = data['project'].get('optional-dependencies', {})
+    matrix = [v for v in groups.values()] if isinstance(groups, dict) else []
+    return sum(matrix, [])
+
 def parse_project_dependencies(data) -> dict:
     if repo.is_poetry(data):
         deps = data['tool']['poetry'].get('dependencies', {})
         res: dict = reduce(parse_poetry_dependency, deps.items(), {})
         return res
     deps = data['project'].get('dependencies', [])
-    return {k: v for dep in deps for (k, v) in parse_pep_621_dependency(dep).items()}
+    optional_deps = get_pep_621_optional_dependencies(data)
+    all_deps = deps + optional_deps
+    return {k: v for dep in all_deps for (k, v) in parse_pep_621_dependency(dep).items()}
 
 def get_project_dependencies(data) -> dict:
     items = parse_project_dependencies(data)
     return {'items': items, 'source': repo.default_toml}
 
 def read_toml_document(path: Path) -> tomlkit.TOMLDocument:
     with path.open(encoding='utf-8', errors='ignore') as f:
```

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/workspace/create.py` & `polylith_cli-1.6.0/polylith_cli/polylith/workspace/create.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/polylith_cli/polylith/workspace/paths.py` & `polylith_cli-1.6.0/polylith_cli/polylith/workspace/paths.py`

 * *Files identical despite different names*

### Comparing `polylith_cli-1.5.4/pyproject.toml` & `polylith_cli-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polylith-cli"
-version = "1.5.4"
+version = "1.6.0"
 description = "Python tooling support for the Polylith Architecture"
 authors = ['David Vujic']
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 license = "MIT"
 readme = "README.md"
```

### Comparing `polylith_cli-1.5.4/PKG-INFO` & `polylith_cli-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polylith-cli
-Version: 1.5.4
+Version: 1.6.0
 Summary: Python tooling support for the Polylith Architecture
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 License: MIT
 Author: David Vujic
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

