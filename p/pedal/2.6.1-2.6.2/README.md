# Comparing `tmp/pedal-2.6.1.tar.gz` & `tmp/pedal-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedal-2.6.1.tar", last modified: Thu Mar 21 14:38:54 2024, max compression
+gzip compressed data, was "pedal-2.6.2.tar", last modified: Wed May  1 17:07:48 2024, max compression
```

## Comparing `pedal-2.6.1.tar` & `pedal-2.6.2.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:54.236972 pedal-2.6.1/
--rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:22.000000 pedal-2.6.1/LICENSE
--rw-rw-rw-   0        0        0     2584 2024-03-21 14:38:54.236972 pedal-2.6.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:53.599170 pedal-2.6.1/Pedal.egg-info/
--rw-rw-rw-   0        0        0     2584 2024-03-21 14:38:53.000000 pedal-2.6.1/Pedal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4651 2024-03-21 14:38:53.000000 pedal-2.6.1/Pedal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 14:38:53.000000 pedal-2.6.1/Pedal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-03-21 14:38:53.000000 pedal-2.6.1/Pedal.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-03-21 14:38:53.000000 pedal-2.6.1/Pedal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-21 14:38:53.000000 pedal-2.6.1/Pedal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1953 2024-03-16 16:19:59.000000 pedal-2.6.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:53.594180 pedal-2.6.1/pedal/
--rw-rw-rw-   0        0        0      995 2023-07-04 14:03:46.000000 pedal-2.6.1/pedal/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:53.626458 pedal-2.6.1/pedal/assertions/
--rw-rw-rw-   0        0        0      617 2024-03-17 00:21:44.000000 pedal-2.6.1/pedal/assertions/__init__.py
--rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:32.000000 pedal-2.6.1/pedal/assertions/classes.py
--rw-rw-rw-   0        0        0    15454 2024-03-17 00:21:49.000000 pedal-2.6.1/pedal/assertions/commands.py
--rw-rw-rw-   0        0        0       73 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/assertions/constants.py
--rw-rw-rw-   0        0        0    20355 2023-05-27 15:44:32.000000 pedal-2.6.1/pedal/assertions/feedbacks.py
--rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:06.000000 pedal-2.6.1/pedal/assertions/functions.py
--rw-rw-rw-   0        0        0     4153 2023-06-23 17:06:56.000000 pedal-2.6.1/pedal/assertions/organizers.py
--rw-rw-rw-   0        0        0      702 2023-07-13 15:41:56.000000 pedal-2.6.1/pedal/assertions/positive.py
--rw-rw-rw-   0        0        0    35690 2024-03-21 14:34:46.000000 pedal-2.6.1/pedal/assertions/runtime.py
--rw-rw-rw-   0        0        0     3468 2023-12-31 15:00:16.000000 pedal-2.6.1/pedal/assertions/setup.py
--rw-rw-rw-   0        0        0    38765 2023-12-31 15:01:17.000000 pedal-2.6.1/pedal/assertions/static.py
--rw-rw-rw-   0        0        0    10685 2024-03-19 18:12:48.000000 pedal-2.6.1/pedal/assertions/testing_libraries.py
--rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/assertions/unittest.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:53.686111 pedal-2.6.1/pedal/cait/
--rw-rw-rw-   0        0        0      445 2020-10-17 20:34:58.000000 pedal-2.6.1/pedal/cait/__init__.py
--rw-rw-rw-   0        0        0     2255 2023-05-27 15:47:14.000000 pedal-2.6.1/pedal/cait/ast_helpers.py
--rw-rw-rw-   0        0        0    11275 2023-06-23 17:10:08.000000 pedal-2.6.1/pedal/cait/ast_map.py
--rw-rw-rw-   0        0        0    10523 2023-06-23 17:10:22.000000 pedal-2.6.1/pedal/cait/cait_api.py
--rw-rw-rw-   0        0        0    23519 2023-12-31 14:59:10.000000 pedal-2.6.1/pedal/cait/cait_node.py
--rw-rw-rw-   0        0        0       59 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/cait/constants.py
--rw-rw-rw-   0        0        0     4722 2023-10-24 16:41:24.000000 pedal-2.6.1/pedal/cait/find_node.py
--rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:48.000000 pedal-2.6.1/pedal/cait/stretchy_tree_matching.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:53.720239 pedal-2.6.1/pedal/command_line/
--rw-rw-rw-   0        0        0       94 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/command_line/__init__.py
--rw-rw-rw-   0        0        0     8203 2024-03-20 22:17:30.000000 pedal-2.6.1/pedal/command_line/command_line.py
--rw-rw-rw-   0        0        0     7301 2023-05-27 15:42:10.000000 pedal-2.6.1/pedal/command_line/mocks.py
--rw-rw-rw-   0        0        0    24755 2023-07-13 13:42:54.000000 pedal-2.6.1/pedal/command_line/modes.py
--rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:54.000000 pedal-2.6.1/pedal/command_line/report.py
--rw-rw-rw-   0        0        0     3549 2023-06-23 17:18:16.000000 pedal-2.6.1/pedal/command_line/verify.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:53.773110 pedal-2.6.1/pedal/core/
--rw-rw-rw-   0        0        0      107 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/core/__init__.py
--rw-rw-rw-   0        0        0    10592 2024-03-20 23:33:19.000000 pedal-2.6.1/pedal/core/commands.py
--rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/core/environment.py
--rw-rw-rw-   0        0        0      707 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/core/errors.py
--rw-rw-rw-   0        0        0    22286 2024-03-20 23:33:26.000000 pedal-2.6.1/pedal/core/feedback.py
--rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/core/feedback_category.py
--rw-rw-rw-   0        0        0     7655 2023-07-17 17:10:40.000000 pedal-2.6.1/pedal/core/final_feedback.py
--rw-rw-rw-   0        0        0     8070 2024-03-16 17:12:33.000000 pedal-2.6.1/pedal/core/formatting.py
--rw-rw-rw-   0        0        0     1962 2023-05-26 21:48:16.000000 pedal-2.6.1/pedal/core/location.py
--rw-rw-rw-   0        0        0    14415 2024-03-20 23:33:35.000000 pedal-2.6.1/pedal/core/report.py
--rw-rw-rw-   0        0        0      822 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/core/resolver.py
--rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:12.000000 pedal-2.6.1/pedal/core/scoring.py
--rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:10.000000 pedal-2.6.1/pedal/core/submission.py
--rw-rw-rw-   0        0        0      405 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/core/tag.py
--rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:36.000000 pedal-2.6.1/pedal/core/tool.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:53.821903 pedal-2.6.1/pedal/environments/
--rw-rw-rw-   0        0        0      670 2023-06-14 15:19:34.000000 pedal-2.6.1/pedal/environments/__init__.py
--rw-rw-rw-   0        0        0     3065 2023-06-28 02:43:08.000000 pedal-2.6.1/pedal/environments/blockpy.py
--rw-rw-rw-   0        0        0    10495 2024-03-21 13:50:35.000000 pedal-2.6.1/pedal/environments/gradescope.py
--rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:50.000000 pedal-2.6.1/pedal/environments/jupyter.py
--rw-rw-rw-   0        0        0    10369 2023-05-26 21:13:04.000000 pedal-2.6.1/pedal/environments/nbgrader.py
--rw-rw-rw-   0        0        0      369 2023-06-08 11:46:54.000000 pedal-2.6.1/pedal/environments/none.py
--rw-rw-rw-   0        0        0      766 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/environments/sandbox.py
--rw-rw-rw-   0        0        0     3572 2023-06-28 02:44:26.000000 pedal-2.6.1/pedal/environments/standard.py
--rw-rw-rw-   0        0        0     5985 2024-03-16 17:22:53.000000 pedal-2.6.1/pedal/environments/terminal.py
--rw-rw-rw-   0        0        0     6671 2023-12-31 15:03:49.000000 pedal-2.6.1/pedal/environments/vpl.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:53.832643 pedal-2.6.1/pedal/extensions/
--rw-rw-rw-   0        0        0        0 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/extensions/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-26 20:49:41.000000 pedal-2.6.1/pedal/extensions/drafter.py
--rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:34.000000 pedal-2.6.1/pedal/extensions/microbit.py
--rw-rw-rw-   0        0        0    11956 2023-11-06 22:48:58.000000 pedal-2.6.1/pedal/extensions/plotting.py
--rw-rw-rw-   0        0        0       81 2022-07-17 15:14:08.000000 pedal-2.6.1/pedal/extensions/turtles.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:53.840140 pedal-2.6.1/pedal/questions/
--rw-rw-rw-   0        0        0      669 2021-12-05 16:49:54.000000 pedal-2.6.1/pedal/questions/__init__.py
--rw-rw-rw-   0        0        0       66 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/questions/constants.py
--rw-rw-rw-   0        0        0      624 2021-09-15 19:16:12.000000 pedal-2.6.1/pedal/questions/feedbacks.py
--rw-rw-rw-   0        0        0     6043 2023-05-27 15:45:44.000000 pedal-2.6.1/pedal/questions/graders.py
--rw-rw-rw-   0        0        0     3477 2023-05-26 21:13:58.000000 pedal-2.6.1/pedal/questions/loader.py
--rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:26.000000 pedal-2.6.1/pedal/questions/pool.py
--rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:16.000000 pedal-2.6.1/pedal/questions/questions.py
--rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:30.000000 pedal-2.6.1/pedal/questions/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:53.861313 pedal-2.6.1/pedal/resolvers/
--rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:58.000000 pedal-2.6.1/pedal/resolvers/__init__.py
--rw-rw-rw-   0        0        0      650 2023-05-27 15:46:00.000000 pedal-2.6.1/pedal/resolvers/core.py
--rw-rw-rw-   0        0        0     1983 2023-06-20 18:25:56.000000 pedal-2.6.1/pedal/resolvers/export.py
--rw-rw-rw-   0        0        0     1823 2023-06-23 17:14:56.000000 pedal-2.6.1/pedal/resolvers/full.py
--rw-rw-rw-   0        0        0     1545 2023-05-26 21:21:48.000000 pedal-2.6.1/pedal/resolvers/sectional.py
--rw-rw-rw-   0        0        0      268 2021-01-26 15:52:28.000000 pedal-2.6.1/pedal/resolvers/silent.py
--rw-rw-rw-   0        0        0     4830 2024-03-20 23:33:56.000000 pedal-2.6.1/pedal/resolvers/simple.py
--rw-rw-rw-   0        0        0     1237 2023-12-31 15:03:33.000000 pedal-2.6.1/pedal/resolvers/statistics.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:53.893139 pedal-2.6.1/pedal/sandbox/
--rw-rw-rw-   0        0        0      662 2023-05-13 15:07:04.000000 pedal-2.6.1/pedal/sandbox/__init__.py
--rw-rw-rw-   0        0        0    19045 2024-03-16 17:38:09.000000 pedal-2.6.1/pedal/sandbox/commands.py
--rw-rw-rw-   0        0        0       72 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/sandbox/constants.py
--rw-rw-rw-   0        0        0     9807 2023-05-26 21:46:00.000000 pedal-2.6.1/pedal/sandbox/data.py
--rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:20.000000 pedal-2.6.1/pedal/sandbox/exceptions.py
--rw-rw-rw-   0        0        0    10503 2023-06-29 17:39:30.000000 pedal-2.6.1/pedal/sandbox/feedbacks.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:53.923122 pedal-2.6.1/pedal/sandbox/library/
--rw-rw-rw-   0        0        0      222 2022-07-17 15:26:48.000000 pedal-2.6.1/pedal/sandbox/library/__init__.py
--rw-rw-rw-   0        0        0     5032 2023-05-27 15:46:10.000000 pedal-2.6.1/pedal/sandbox/library/designer.py
--rw-rw-rw-   0        0        0     2930 2024-03-20 23:32:55.000000 pedal-2.6.1/pedal/sandbox/library/drafter.py
--rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:42.000000 pedal-2.6.1/pedal/sandbox/library/matplotlib.py
--rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:52.000000 pedal-2.6.1/pedal/sandbox/library/microbit.py
--rw-rw-rw-   0        0        0     3404 2023-05-27 15:46:28.000000 pedal-2.6.1/pedal/sandbox/library/turtles.py
--rw-rw-rw-   0        0        0    11278 2024-03-20 23:34:03.000000 pedal-2.6.1/pedal/sandbox/mocked.py
--rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:24.000000 pedal-2.6.1/pedal/sandbox/result.py
--rw-rw-rw-   0        0        0    39748 2024-03-19 16:52:57.000000 pedal-2.6.1/pedal/sandbox/sandbox.py
--rw-rw-rw-   0        0        0     5048 2023-05-27 15:46:24.000000 pedal-2.6.1/pedal/sandbox/timeout.py
--rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:50.000000 pedal-2.6.1/pedal/sandbox/tracer.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:53.977949 pedal-2.6.1/pedal/source/
--rw-rw-rw-   0        0        0      914 2023-05-27 15:44:58.000000 pedal-2.6.1/pedal/source/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/source/constants.py
--rw-rw-rw-   0        0        0     6481 2023-10-23 14:17:44.000000 pedal-2.6.1/pedal/source/feedbacks.py
--rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/source/sections.py
--rw-rw-rw-   0        0        0     7716 2023-06-10 14:14:44.000000 pedal-2.6.1/pedal/source/source.py
--rw-rw-rw-   0        0        0      484 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/source/substitutions.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:54.040161 pedal-2.6.1/pedal/tifa/
--rw-rw-rw-   0        0        0     3046 2023-05-27 15:47:24.000000 pedal-2.6.1/pedal/tifa/__init__.py
--rw-rw-rw-   0        0        0     2449 2023-06-23 17:12:00.000000 pedal-2.6.1/pedal/tifa/commands.py
--rw-rw-rw-   0        0        0       91 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/tifa/constants.py
--rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:36.000000 pedal-2.6.1/pedal/tifa/contexts.py
--rw-rw-rw-   0        0        0    23656 2023-05-22 16:40:10.000000 pedal-2.6.1/pedal/tifa/feedbacks.py
--rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/tifa/identifier.py
--rw-rw-rw-   0        0        0      908 2022-06-07 19:06:46.000000 pedal-2.6.1/pedal/tifa/settings.py
--rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:16.000000 pedal-2.6.1/pedal/tifa/state.py
--rw-rw-rw-   0        0        0    24283 2023-06-23 17:17:24.000000 pedal-2.6.1/pedal/tifa/tifa_core.py
--rw-rw-rw-   0        0        0    42771 2024-02-11 21:16:12.000000 pedal-2.6.1/pedal/tifa/tifa_visitor.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:54.074975 pedal-2.6.1/pedal/types/
--rw-rw-rw-   0        0        0       86 2022-06-09 18:41:54.000000 pedal-2.6.1/pedal/types/__init__.py
--rw-rw-rw-   0        0        0     9162 2023-05-27 15:45:12.000000 pedal-2.6.1/pedal/types/builtin.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:54.126843 pedal-2.6.1/pedal/types/library/
--rw-rw-rw-   0        0        0      192 2022-07-26 18:00:28.000000 pedal-2.6.1/pedal/types/library/__init__.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:47:00.000000 pedal-2.6.1/pedal/types/library/cs1_curriculum.py
--rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:18.000000 pedal-2.6.1/pedal/types/library/designer.py
--rw-rw-rw-   0        0        0     1566 2024-03-18 19:08:34.000000 pedal-2.6.1/pedal/types/library/drafter.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:51:18.000000 pedal-2.6.1/pedal/types/library/matplotlib.py
--rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:26.000000 pedal-2.6.1/pedal/types/library/microbit.py
--rw-rw-rw-   0        0        0      441 2022-11-28 05:52:08.000000 pedal-2.6.1/pedal/types/library/turtles.py
--rw-rw-rw-   0        0        0    51484 2023-10-19 16:31:12.000000 pedal-2.6.1/pedal/types/new_types.py
--rw-rw-rw-   0        0        0    15264 2023-12-31 15:01:54.000000 pedal-2.6.1/pedal/types/normalize.py
--rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:54.000000 pedal-2.6.1/pedal/types/operations.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:54.205300 pedal-2.6.1/pedal/utilities/
--rw-rw-rw-   0        0        0      524 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/utilities/__init__.py
--rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:02.000000 pedal-2.6.1/pedal/utilities/ast_tools.py
--rw-rw-rw-   0        0        0     6559 2023-06-23 17:07:42.000000 pedal-2.6.1/pedal/utilities/comparisons.py
--rw-rw-rw-   0        0        0      679 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/utilities/dictionaries.py
--rw-rw-rw-   0        0        0    10097 2023-10-23 14:37:31.000000 pedal-2.6.1/pedal/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:42.000000 pedal-2.6.1/pedal/utilities/files.py
--rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/utilities/operators.py
--rw-rw-rw-   0        0        0     8215 2023-06-27 13:50:08.000000 pedal-2.6.1/pedal/utilities/progsnap.py
--rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/utilities/sorting.py
--rw-rw-rw-   0        0        0      486 2023-10-20 17:11:10.000000 pedal-2.6.1/pedal/utilities/system.py
--rw-rw-rw-   0        0        0     3759 2024-03-16 17:17:25.000000 pedal-2.6.1/pedal/utilities/text.py
--rw-rw-rw-   0        0        0      769 2020-10-17 16:15:24.000000 pedal-2.6.1/pedal/utilities/types.py
--rw-rw-rw-   0        0        0      121 2024-03-21 14:38:54.239099 pedal-2.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1227 2024-03-21 14:36:46.000000 pedal-2.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:38:54.235974 pedal-2.6.1/tests/
--rw-rw-rw-   0        0        0     5505 2024-03-19 17:40:49.000000 pedal-2.6.1/tests/test_assertion_dataclasses.py
--rw-rw-rw-   0        0        0     9161 2024-03-16 17:19:05.000000 pedal-2.6.1/tests/test_assertion_functions.py
--rw-rw-rw-   0        0        0     7341 2023-07-13 16:06:18.000000 pedal-2.6.1/tests/test_assertion_static.py
--rw-rw-rw-   0        0        0    21852 2024-03-21 14:35:10.000000 pedal-2.6.1/tests/test_assertions_runtime.py
--rw-rw-rw-   0        0        0    39776 2021-03-12 21:12:48.000000 pedal-2.6.1/tests/test_cait.py
--rw-rw-rw-   0        0        0     8398 2020-10-17 16:15:24.000000 pedal-2.6.1/tests/test_cait_node.py
--rw-rw-rw-   0        0        0     7217 2024-03-20 23:32:55.000000 pedal-2.6.1/tests/test_drafter.py
--rw-rw-rw-   0        0        0     3668 2023-06-23 15:39:52.000000 pedal-2.6.1/tests/test_environment_nbgrader.py
--rw-rw-rw-   0        0        0     7069 2023-10-06 22:35:25.000000 pedal-2.6.1/tests/test_environment_terminal.py
--rw-rw-rw-   0        0        0     1981 2024-03-19 16:19:32.000000 pedal-2.6.1/tests/test_formatter.py
--rw-rw-rw-   0        0        0     5277 2020-10-17 18:51:26.000000 pedal-2.6.1/tests/test_loader.py
--rw-rw-rw-   0        0        0     7460 2022-07-21 17:05:16.000000 pedal-2.6.1/tests/test_microbits.py
--rw-rw-rw-   0        0        0     9212 2024-03-19 16:27:06.000000 pedal-2.6.1/tests/test_plots.py
--rw-rw-rw-   0        0        0     6693 2022-05-01 16:50:18.000000 pedal-2.6.1/tests/test_questions.py
--rw-rw-rw-   0        0        0      574 2023-05-22 16:21:26.000000 pedal-2.6.1/tests/test_report.py
--rw-rw-rw-   0        0        0    12213 2023-06-29 16:59:50.000000 pedal-2.6.1/tests/test_resolver.py
--rw-rw-rw-   0        0        0    20855 2023-06-29 17:37:04.000000 pedal-2.6.1/tests/test_sandbox.py
--rw-rw-rw-   0        0        0     5296 2023-07-13 16:26:26.000000 pedal-2.6.1/tests/test_sneks_functions.py
--rw-rw-rw-   0        0        0     5511 2023-06-29 17:01:24.000000 pedal-2.6.1/tests/test_source.py
--rw-rw-rw-   0        0        0     2084 2024-03-19 18:11:41.000000 pedal-2.6.1/tests/test_testing_libraries.py
--rw-rw-rw-   0        0        0    54206 2023-10-20 16:46:11.000000 pedal-2.6.1/tests/test_tifa.py
--rw-rw-rw-   0        0        0     3209 2020-10-17 16:15:24.000000 pedal-2.6.1/tests/test_toolkit.py
--rw-rw-rw-   0        0        0     2013 2022-06-16 15:36:22.000000 pedal-2.6.1/tests/test_types.py
--rw-rw-rw-   0        0        0     1712 2023-06-29 17:37:08.000000 pedal-2.6.1/tests/test_user_feedback.py
--rw-rw-rw-   0        0        0     1466 2020-11-01 17:56:24.000000 pedal-2.6.1/tests/test_utilities_progsnap.py
--rw-rw-rw-   0        0        0     2533 2020-10-17 16:15:24.000000 pedal-2.6.1/tests/test_utilities_sorting.py
--rw-rw-rw-   0        0        0     3738 2023-06-29 17:01:16.000000 pedal-2.6.1/tests/test_vpl.py
--rw-rw-rw-   0        0        0     3734 2023-10-06 23:29:36.000000 pedal-2.6.1/tests/test_wheatchaff_game.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.332453 pedal-2.6.2/
+-rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:22.000000 pedal-2.6.2/LICENSE
+-rw-rw-rw-   0        0        0     2584 2024-05-01 17:07:48.331444 pedal-2.6.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.208932 pedal-2.6.2/Pedal.egg-info/
+-rw-rw-rw-   0        0        0     2584 2024-05-01 17:07:48.000000 pedal-2.6.2/Pedal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4659 2024-05-01 17:07:48.000000 pedal-2.6.2/Pedal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 17:07:48.000000 pedal-2.6.2/Pedal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-01 17:07:48.000000 pedal-2.6.2/Pedal.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-01 17:07:48.000000 pedal-2.6.2/Pedal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-01 17:07:48.000000 pedal-2.6.2/Pedal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1953 2024-03-16 16:19:59.000000 pedal-2.6.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.203935 pedal-2.6.2/pedal/
+-rw-rw-rw-   0        0        0      995 2023-07-04 14:03:46.000000 pedal-2.6.2/pedal/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.219932 pedal-2.6.2/pedal/assertions/
+-rw-rw-rw-   0        0        0      617 2024-03-17 00:21:44.000000 pedal-2.6.2/pedal/assertions/__init__.py
+-rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:32.000000 pedal-2.6.2/pedal/assertions/classes.py
+-rw-rw-rw-   0        0        0    16626 2024-05-01 17:00:37.000000 pedal-2.6.2/pedal/assertions/commands.py
+-rw-rw-rw-   0        0        0       73 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/assertions/constants.py
+-rw-rw-rw-   0        0        0    20355 2023-05-27 15:44:32.000000 pedal-2.6.2/pedal/assertions/feedbacks.py
+-rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:06.000000 pedal-2.6.2/pedal/assertions/functions.py
+-rw-rw-rw-   0        0        0     4153 2023-06-23 17:06:56.000000 pedal-2.6.2/pedal/assertions/organizers.py
+-rw-rw-rw-   0        0        0      702 2023-07-13 15:41:56.000000 pedal-2.6.2/pedal/assertions/positive.py
+-rw-rw-rw-   0        0        0    35690 2024-03-21 14:34:46.000000 pedal-2.6.2/pedal/assertions/runtime.py
+-rw-rw-rw-   0        0        0     3468 2023-12-31 15:00:16.000000 pedal-2.6.2/pedal/assertions/setup.py
+-rw-rw-rw-   0        0        0    38765 2024-04-15 15:54:04.000000 pedal-2.6.2/pedal/assertions/static.py
+-rw-rw-rw-   0        0        0    10685 2024-03-19 18:12:48.000000 pedal-2.6.2/pedal/assertions/testing_libraries.py
+-rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/assertions/unittest.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.225940 pedal-2.6.2/pedal/cait/
+-rw-rw-rw-   0        0        0      445 2020-10-17 20:34:58.000000 pedal-2.6.2/pedal/cait/__init__.py
+-rw-rw-rw-   0        0        0     2255 2023-05-27 15:47:14.000000 pedal-2.6.2/pedal/cait/ast_helpers.py
+-rw-rw-rw-   0        0        0    11275 2023-06-23 17:10:08.000000 pedal-2.6.2/pedal/cait/ast_map.py
+-rw-rw-rw-   0        0        0    10523 2023-06-23 17:10:22.000000 pedal-2.6.2/pedal/cait/cait_api.py
+-rw-rw-rw-   0        0        0    23519 2023-12-31 14:59:10.000000 pedal-2.6.2/pedal/cait/cait_node.py
+-rw-rw-rw-   0        0        0       59 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/cait/constants.py
+-rw-rw-rw-   0        0        0     4722 2023-10-24 16:41:24.000000 pedal-2.6.2/pedal/cait/find_node.py
+-rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:48.000000 pedal-2.6.2/pedal/cait/stretchy_tree_matching.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.230942 pedal-2.6.2/pedal/command_line/
+-rw-rw-rw-   0        0        0       94 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/command_line/__init__.py
+-rw-rw-rw-   0        0        0     8480 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/command_line/command_line.py
+-rw-rw-rw-   0        0        0     7301 2023-05-27 15:42:10.000000 pedal-2.6.2/pedal/command_line/mocks.py
+-rw-rw-rw-   0        0        0    24755 2023-07-13 13:42:54.000000 pedal-2.6.2/pedal/command_line/modes.py
+-rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:54.000000 pedal-2.6.2/pedal/command_line/report.py
+-rw-rw-rw-   0        0        0     3549 2023-06-23 17:18:16.000000 pedal-2.6.2/pedal/command_line/verify.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.243929 pedal-2.6.2/pedal/core/
+-rw-rw-rw-   0        0        0      107 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/core/__init__.py
+-rw-rw-rw-   0        0        0    10898 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/core/commands.py
+-rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/core/environment.py
+-rw-rw-rw-   0        0        0      707 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/core/errors.py
+-rw-rw-rw-   0        0        0    22848 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/core/feedback.py
+-rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/core/feedback_category.py
+-rw-rw-rw-   0        0        0     7655 2023-07-17 17:10:40.000000 pedal-2.6.2/pedal/core/final_feedback.py
+-rw-rw-rw-   0        0        0     8070 2024-03-16 17:12:33.000000 pedal-2.6.2/pedal/core/formatting.py
+-rw-rw-rw-   0        0        0     1962 2023-05-26 21:48:16.000000 pedal-2.6.2/pedal/core/location.py
+-rw-rw-rw-   0        0        0    14783 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/core/report.py
+-rw-rw-rw-   0        0        0      822 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/core/resolver.py
+-rw-rw-rw-   0        0        0     4450 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/core/scoring.py
+-rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:10.000000 pedal-2.6.2/pedal/core/submission.py
+-rw-rw-rw-   0        0        0      405 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/core/tag.py
+-rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:36.000000 pedal-2.6.2/pedal/core/tool.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.251935 pedal-2.6.2/pedal/environments/
+-rw-rw-rw-   0        0        0      670 2023-06-14 15:19:34.000000 pedal-2.6.2/pedal/environments/__init__.py
+-rw-rw-rw-   0        0        0     3065 2023-06-28 02:43:08.000000 pedal-2.6.2/pedal/environments/blockpy.py
+-rw-rw-rw-   0        0        0    10495 2024-03-21 13:50:35.000000 pedal-2.6.2/pedal/environments/gradescope.py
+-rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:50.000000 pedal-2.6.2/pedal/environments/jupyter.py
+-rw-rw-rw-   0        0        0    10369 2023-05-26 21:13:04.000000 pedal-2.6.2/pedal/environments/nbgrader.py
+-rw-rw-rw-   0        0        0      369 2023-06-08 11:46:54.000000 pedal-2.6.2/pedal/environments/none.py
+-rw-rw-rw-   0        0        0      766 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/environments/sandbox.py
+-rw-rw-rw-   0        0        0     3572 2023-06-28 02:44:26.000000 pedal-2.6.2/pedal/environments/standard.py
+-rw-rw-rw-   0        0        0     5991 2024-05-01 16:59:10.000000 pedal-2.6.2/pedal/environments/terminal.py
+-rw-rw-rw-   0        0        0     6671 2023-12-31 15:03:49.000000 pedal-2.6.2/pedal/environments/vpl.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.254935 pedal-2.6.2/pedal/extensions/
+-rw-rw-rw-   0        0        0        0 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/extensions/__init__.py
+-rw-rw-rw-   0        0        0      192 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/extensions/drafter.py
+-rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:34.000000 pedal-2.6.2/pedal/extensions/microbit.py
+-rw-rw-rw-   0        0        0    11956 2023-11-06 22:48:58.000000 pedal-2.6.2/pedal/extensions/plotting.py
+-rw-rw-rw-   0        0        0       81 2022-07-17 15:14:08.000000 pedal-2.6.2/pedal/extensions/turtles.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.259935 pedal-2.6.2/pedal/questions/
+-rw-rw-rw-   0        0        0      669 2021-12-05 16:49:54.000000 pedal-2.6.2/pedal/questions/__init__.py
+-rw-rw-rw-   0        0        0       66 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/questions/constants.py
+-rw-rw-rw-   0        0        0      624 2021-09-15 19:16:12.000000 pedal-2.6.2/pedal/questions/feedbacks.py
+-rw-rw-rw-   0        0        0     6043 2023-05-27 15:45:44.000000 pedal-2.6.2/pedal/questions/graders.py
+-rw-rw-rw-   0        0        0     3477 2023-05-26 21:13:58.000000 pedal-2.6.2/pedal/questions/loader.py
+-rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:26.000000 pedal-2.6.2/pedal/questions/pool.py
+-rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:16.000000 pedal-2.6.2/pedal/questions/questions.py
+-rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:30.000000 pedal-2.6.2/pedal/questions/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.266444 pedal-2.6.2/pedal/resolvers/
+-rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:58.000000 pedal-2.6.2/pedal/resolvers/__init__.py
+-rw-rw-rw-   0        0        0      650 2023-05-27 15:46:00.000000 pedal-2.6.2/pedal/resolvers/core.py
+-rw-rw-rw-   0        0        0     1983 2023-06-20 18:25:56.000000 pedal-2.6.2/pedal/resolvers/export.py
+-rw-rw-rw-   0        0        0     1823 2023-06-23 17:14:56.000000 pedal-2.6.2/pedal/resolvers/full.py
+-rw-rw-rw-   0        0        0     1545 2023-05-26 21:21:48.000000 pedal-2.6.2/pedal/resolvers/sectional.py
+-rw-rw-rw-   0        0        0      268 2021-01-26 15:52:28.000000 pedal-2.6.2/pedal/resolvers/silent.py
+-rw-rw-rw-   0        0        0     4980 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/resolvers/simple.py
+-rw-rw-rw-   0        0        0     1237 2023-12-31 15:03:33.000000 pedal-2.6.2/pedal/resolvers/statistics.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.274444 pedal-2.6.2/pedal/sandbox/
+-rw-rw-rw-   0        0        0      662 2023-05-13 15:07:04.000000 pedal-2.6.2/pedal/sandbox/__init__.py
+-rw-rw-rw-   0        0        0    19045 2024-03-16 17:38:09.000000 pedal-2.6.2/pedal/sandbox/commands.py
+-rw-rw-rw-   0        0        0       72 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/sandbox/constants.py
+-rw-rw-rw-   0        0        0     9807 2023-05-26 21:46:00.000000 pedal-2.6.2/pedal/sandbox/data.py
+-rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:20.000000 pedal-2.6.2/pedal/sandbox/exceptions.py
+-rw-rw-rw-   0        0        0    10503 2023-06-29 17:39:30.000000 pedal-2.6.2/pedal/sandbox/feedbacks.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.279446 pedal-2.6.2/pedal/sandbox/library/
+-rw-rw-rw-   0        0        0      285 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/sandbox/library/__init__.py
+-rw-rw-rw-   0        0        0     5032 2023-05-27 15:46:10.000000 pedal-2.6.2/pedal/sandbox/library/designer.py
+-rw-rw-rw-   0        0        0     3709 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/sandbox/library/drafter_library.py
+-rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:42.000000 pedal-2.6.2/pedal/sandbox/library/matplotlib.py
+-rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:52.000000 pedal-2.6.2/pedal/sandbox/library/microbit.py
+-rw-rw-rw-   0        0        0     3404 2023-05-27 15:46:28.000000 pedal-2.6.2/pedal/sandbox/library/turtles.py
+-rw-rw-rw-   0        0        0    11640 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/sandbox/mocked.py
+-rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:24.000000 pedal-2.6.2/pedal/sandbox/result.py
+-rw-rw-rw-   0        0        0    40746 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/sandbox/sandbox.py
+-rw-rw-rw-   0        0        0     5048 2023-05-27 15:46:24.000000 pedal-2.6.2/pedal/sandbox/timeout.py
+-rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:50.000000 pedal-2.6.2/pedal/sandbox/tracer.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.283444 pedal-2.6.2/pedal/source/
+-rw-rw-rw-   0        0        0      914 2023-05-27 15:44:58.000000 pedal-2.6.2/pedal/source/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/source/constants.py
+-rw-rw-rw-   0        0        0     6481 2023-10-23 14:17:44.000000 pedal-2.6.2/pedal/source/feedbacks.py
+-rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/source/sections.py
+-rw-rw-rw-   0        0        0     7716 2023-06-10 14:14:44.000000 pedal-2.6.2/pedal/source/source.py
+-rw-rw-rw-   0        0        0      484 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/source/substitutions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.291444 pedal-2.6.2/pedal/tifa/
+-rw-rw-rw-   0        0        0     3046 2023-05-27 15:47:24.000000 pedal-2.6.2/pedal/tifa/__init__.py
+-rw-rw-rw-   0        0        0     2449 2023-06-23 17:12:00.000000 pedal-2.6.2/pedal/tifa/commands.py
+-rw-rw-rw-   0        0        0       91 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/tifa/constants.py
+-rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:36.000000 pedal-2.6.2/pedal/tifa/contexts.py
+-rw-rw-rw-   0        0        0    23656 2023-05-22 16:40:10.000000 pedal-2.6.2/pedal/tifa/feedbacks.py
+-rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/tifa/identifier.py
+-rw-rw-rw-   0        0        0      908 2022-06-07 19:06:46.000000 pedal-2.6.2/pedal/tifa/settings.py
+-rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:16.000000 pedal-2.6.2/pedal/tifa/state.py
+-rw-rw-rw-   0        0        0    24283 2023-06-23 17:17:24.000000 pedal-2.6.2/pedal/tifa/tifa_core.py
+-rw-rw-rw-   0        0        0    44027 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/tifa/tifa_visitor.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.295445 pedal-2.6.2/pedal/types/
+-rw-rw-rw-   0        0        0       86 2022-06-09 18:41:54.000000 pedal-2.6.2/pedal/types/__init__.py
+-rw-rw-rw-   0        0        0     9162 2023-05-27 15:45:12.000000 pedal-2.6.2/pedal/types/builtin.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.301448 pedal-2.6.2/pedal/types/library/
+-rw-rw-rw-   0        0        0      228 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/types/library/__init__.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:47:00.000000 pedal-2.6.2/pedal/types/library/cs1_curriculum.py
+-rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:18.000000 pedal-2.6.2/pedal/types/library/designer.py
+-rw-rw-rw-   0        0        0     1665 2024-05-01 16:59:07.000000 pedal-2.6.2/pedal/types/library/drafter.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:51:18.000000 pedal-2.6.2/pedal/types/library/matplotlib.py
+-rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:26.000000 pedal-2.6.2/pedal/types/library/microbit.py
+-rw-rw-rw-   0        0        0      441 2022-11-28 05:52:08.000000 pedal-2.6.2/pedal/types/library/turtles.py
+-rw-rw-rw-   0        0        0    51484 2023-10-19 16:31:12.000000 pedal-2.6.2/pedal/types/new_types.py
+-rw-rw-rw-   0        0        0    15264 2023-12-31 15:01:54.000000 pedal-2.6.2/pedal/types/normalize.py
+-rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:54.000000 pedal-2.6.2/pedal/types/operations.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.309449 pedal-2.6.2/pedal/utilities/
+-rw-rw-rw-   0        0        0      524 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:02.000000 pedal-2.6.2/pedal/utilities/ast_tools.py
+-rw-rw-rw-   0        0        0     6559 2023-06-23 17:07:42.000000 pedal-2.6.2/pedal/utilities/comparisons.py
+-rw-rw-rw-   0        0        0      679 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/utilities/dictionaries.py
+-rw-rw-rw-   0        0        0    10097 2023-10-23 14:37:31.000000 pedal-2.6.2/pedal/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:42.000000 pedal-2.6.2/pedal/utilities/files.py
+-rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/utilities/operators.py
+-rw-rw-rw-   0        0        0     8215 2023-06-27 13:50:08.000000 pedal-2.6.2/pedal/utilities/progsnap.py
+-rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/utilities/sorting.py
+-rw-rw-rw-   0        0        0      486 2023-10-20 17:11:10.000000 pedal-2.6.2/pedal/utilities/system.py
+-rw-rw-rw-   0        0        0     3759 2024-03-16 17:17:25.000000 pedal-2.6.2/pedal/utilities/text.py
+-rw-rw-rw-   0        0        0      769 2020-10-17 16:15:24.000000 pedal-2.6.2/pedal/utilities/types.py
+-rw-rw-rw-   0        0        0      121 2024-05-01 17:07:48.336445 pedal-2.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1227 2024-05-01 17:07:26.000000 pedal-2.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:07:48.331444 pedal-2.6.2/tests/
+-rw-rw-rw-   0        0        0     5505 2024-03-19 17:40:49.000000 pedal-2.6.2/tests/test_assertion_dataclasses.py
+-rw-rw-rw-   0        0        0     9242 2024-05-01 17:01:00.000000 pedal-2.6.2/tests/test_assertion_functions.py
+-rw-rw-rw-   0        0        0     7341 2023-07-13 16:06:18.000000 pedal-2.6.2/tests/test_assertion_static.py
+-rw-rw-rw-   0        0        0    21852 2024-03-21 14:35:10.000000 pedal-2.6.2/tests/test_assertions_runtime.py
+-rw-rw-rw-   0        0        0    39776 2021-03-12 21:12:48.000000 pedal-2.6.2/tests/test_cait.py
+-rw-rw-rw-   0        0        0     8398 2020-10-17 16:15:24.000000 pedal-2.6.2/tests/test_cait_node.py
+-rw-rw-rw-   0        0        0     7225 2024-05-01 16:59:07.000000 pedal-2.6.2/tests/test_drafter.py
+-rw-rw-rw-   0        0        0     3668 2023-06-23 15:39:52.000000 pedal-2.6.2/tests/test_environment_nbgrader.py
+-rw-rw-rw-   0        0        0     7107 2024-05-01 17:02:27.000000 pedal-2.6.2/tests/test_environment_terminal.py
+-rw-rw-rw-   0        0        0     1981 2024-03-19 16:19:32.000000 pedal-2.6.2/tests/test_formatter.py
+-rw-rw-rw-   0        0        0     5277 2020-10-17 18:51:26.000000 pedal-2.6.2/tests/test_loader.py
+-rw-rw-rw-   0        0        0     7460 2022-07-21 17:05:16.000000 pedal-2.6.2/tests/test_microbits.py
+-rw-rw-rw-   0        0        0     9212 2024-03-19 16:27:06.000000 pedal-2.6.2/tests/test_plots.py
+-rw-rw-rw-   0        0        0     6693 2022-05-01 16:50:18.000000 pedal-2.6.2/tests/test_questions.py
+-rw-rw-rw-   0        0        0      574 2023-05-22 16:21:26.000000 pedal-2.6.2/tests/test_report.py
+-rw-rw-rw-   0        0        0    13082 2024-05-01 16:59:07.000000 pedal-2.6.2/tests/test_resolver.py
+-rw-rw-rw-   0        0        0    20855 2023-06-29 17:37:04.000000 pedal-2.6.2/tests/test_sandbox.py
+-rw-rw-rw-   0        0        0     5296 2023-07-13 16:26:26.000000 pedal-2.6.2/tests/test_sneks_functions.py
+-rw-rw-rw-   0        0        0     5511 2023-06-29 17:01:24.000000 pedal-2.6.2/tests/test_source.py
+-rw-rw-rw-   0        0        0     2084 2024-03-19 18:11:41.000000 pedal-2.6.2/tests/test_testing_libraries.py
+-rw-rw-rw-   0        0        0    56754 2024-05-01 16:59:07.000000 pedal-2.6.2/tests/test_tifa.py
+-rw-rw-rw-   0        0        0     3209 2020-10-17 16:15:24.000000 pedal-2.6.2/tests/test_toolkit.py
+-rw-rw-rw-   0        0        0     2013 2022-06-16 15:36:22.000000 pedal-2.6.2/tests/test_types.py
+-rw-rw-rw-   0        0        0     1712 2023-06-29 17:37:08.000000 pedal-2.6.2/tests/test_user_feedback.py
+-rw-rw-rw-   0        0        0     1466 2020-11-01 17:56:24.000000 pedal-2.6.2/tests/test_utilities_progsnap.py
+-rw-rw-rw-   0        0        0     2533 2020-10-17 16:15:24.000000 pedal-2.6.2/tests/test_utilities_sorting.py
+-rw-rw-rw-   0        0        0     3738 2023-06-29 17:01:16.000000 pedal-2.6.2/tests/test_vpl.py
+-rw-rw-rw-   0        0        0     3734 2023-10-06 23:29:36.000000 pedal-2.6.2/tests/test_wheatchaff_game.py
```

### Comparing `pedal-2.6.1/LICENSE` & `pedal-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/PKG-INFO` & `pedal-2.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pedal
-Version: 2.6.1
+Version: 2.6.2
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Keywords: feedback education teaching program analysis tifa cait sandbox pedal grading grader grade
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pedal-2.6.1/Pedal.egg-info/PKG-INFO` & `pedal-2.6.2/Pedal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pedal
-Version: 2.6.1
+Version: 2.6.2
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Keywords: feedback education teaching program analysis tifa cait sandbox pedal grading grader grade
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pedal-2.6.1/Pedal.egg-info/SOURCES.txt` & `pedal-2.6.2/Pedal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 pedal/sandbox/mocked.py
 pedal/sandbox/result.py
 pedal/sandbox/sandbox.py
 pedal/sandbox/timeout.py
 pedal/sandbox/tracer.py
 pedal/sandbox/library/__init__.py
 pedal/sandbox/library/designer.py
-pedal/sandbox/library/drafter.py
+pedal/sandbox/library/drafter_library.py
 pedal/sandbox/library/matplotlib.py
 pedal/sandbox/library/microbit.py
 pedal/sandbox/library/turtles.py
 pedal/source/__init__.py
 pedal/source/constants.py
 pedal/source/feedbacks.py
 pedal/source/sections.py
```

### Comparing `pedal-2.6.1/README.rst` & `pedal-2.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/__init__.py` & `pedal-2.6.2/pedal/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/assertions/__init__.py` & `pedal-2.6.2/pedal/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/assertions/classes.py` & `pedal-2.6.2/pedal/assertions/classes.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/assertions/commands.py` & `pedal-2.6.2/pedal/assertions/commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,320 +1,333 @@
-"""
-Unifying collection of all the commands in ``pedal.assertions``.
-"""
-from pedal.core.commands import gently
-from pedal.core.scoring import Score, combine_scores
-from pedal.sandbox.commands import call, clear_student_data, run, get_sandbox, CommandBlock
-from pedal.assertions.static import *
-from pedal.assertions.runtime import *
-from pedal.assertions.runtime import _FIELDS
-from pedal.assertions.positive import close_output, correct_output
-from pedal.types.new_types import is_subtype
-from pedal.assertions.testing_libraries import *
-
-try:
-    from dataclasses import fields
-except:
-    fields = None
-
-
-class unit_test(assert_group):
-    justification_template = ("Some of the feedback in this group was triggered.",
-                              "None of the feedback in this group was triggered.")
-
-    def __init__(self, function_name, given_partial_credit=None, given_score=None, **kwargs):
-        super().__init__(function_name, **kwargs)
-        self.given_partial_credit = given_partial_credit
-        self.given_score = given_score
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        super().__exit__(exc_type, exc_value, traceback)
-        if self.given_partial_credit is False:
-            self.score = self.given_score
-        else:
-            self.valence = self.POSITIVE_VALENCE
-            self.score = combine_scores([success.score for success in self.successes],
-                                        [failure.score for failure in self.failures] +
-                                        [error.score for error in self.errors])
-        return False
-
-
-_unit_test_class = unit_test
-
-
-def unit_test(function, *tests, else_message=None, else_message_template=None,
-              score=None, partial_credit=False,
-              assert_function=None, context=None, **kwargs):
-    """
-    Helper function for quickly unit testing.
-
-    * Specify exact score for each test case, individually | list[str]
-    * Specify exact score for each test case, with single value | str
-    * Specify total score for all test cases, no partial credit | False, using `score`
-    * Specify total score for all test cases, divide by # of cases passed | True, using `score`
-
-    Args:
-        assert_function: Override the assert function (defaults to assert_equal)
-        function (str): The name of the function to test.
-        *tests (): The test cases to run. Each test case is a tuple of the input/output pairs.
-        else_message (str): The message to present as a positive if the
-             tests all pass.
-        else_message_template (str): The template for the else_message, to be formatted.
-        score (str): The score to give overall/per test case, depending on
-            partial_credit.
-        partial_credit (bool or str or list[str]): Whether to give credit for
-            each unit test as a percentage of the whole (True), or to only give
-            points for passing all the tests (False). Defaults to False.
-            If a list is passed, those scores will be used per test case.
-        context (Sandbox or CommandBlock): The context to run the function in.
-        **kwargs ():
-
-    Returns:
-
-    """
-    if assert_function is None:
-        assert_function = assert_equal
-    each_score = partial_credit_logic(tests, score, partial_credit)
-    # Handle context
-    if context is True:
-        context = get_sandbox().get_context()
-    elif context:
-        if isinstance(context, Sandbox):
-            context = context.get_context()
-        elif isinstance(context, CommandBlock):
-            context = context.context
-        else:
-            context = get_sandbox().get_context(context._actual_context_id)
-    unit_test_context = _unit_test_class(function,
-                                         else_message=else_message,
-                                         else_message_template=else_message_template,
-                                         context=context, given_partial_credit=partial_credit,
-                                         given_score=score, **kwargs)
-    if not tests:
-        return unit_test_context
-    # TODO: Make it so unit_test can document its cases
-    with unit_test_context as group_result:
-        for test_index, test in enumerate(tests):
-            args, expected = test
-            if isinstance(args, str):
-                assert_function(call(function, args_locals=[args]), expected, score=each_score[test_index], **kwargs)
-            else:
-                assert_function(call(function, *args), expected, score=each_score[test_index], **kwargs)
-
-    return not group_result
-
-
-class check_dataclass_error(RuntimeAssertionFeedback):
-    justification = "Value is not a dataclass"
-    _expected_verb = "to be"
-    _inverse_operator = "is not"
-
-    def __init__(self, value, **kwargs):
-        super().__init__(SandboxedValue(value), ExactValue("a dataclass"), **kwargs)
-
-def check_dataclass_instance(value, dataclass, else_message=None, score=None, partial_credit=False, **kwargs):
-    report = kwargs.get('report', MAIN_REPORT)
-    name = dataclass.__name__
-    # Check that we weren't given an error
-    if isinstance(value, Exception):
-        return check_dataclass_error(value, score=score, **kwargs)
-        #return gently(f"I evaluated the name {report.format.name(name)} and expected the result to be a dataclass. "
-        #              f"However, there was an error instead.",
-        #              label="check_dataclass_error", score=score, **kwargs)
-    # Get the students' instance as a Pedal Type
-    value_pedal_type = get_pedal_type_from_value(unwrap_value(value), evaluate)
-    # Convert the instructor's version to a Pedal type
-    evaluated_expected_type = evaluate(dataclass) if isinstance(dataclass, str) else dataclass
-    expected_pedal_type = normalize_type(evaluated_expected_type, evaluate)
-    if not isinstance(expected_pedal_type, Exception):
-        expected_pedal_type = expected_pedal_type.as_type()
-        expected_pedal_type_name = expected_pedal_type.singular_name
-    else:
-        expected_pedal_type_name = ""
-    # Make sure the students' version is an actual dataclass
-    singular_name = share_sandbox_context(value_pedal_type.singular_name, value)
-    if not hasattr(unwrap_value(value), _FIELDS):
-        return check_dataclass_error(value, score=score, **kwargs)
-        #return gently(f"I evaluated the name {report.format.name(name)} and expected the result to be a dataclass. "
-        #              f"However, the result was a {report.format.python_expression(str(type(unwrap_value(value))))}",
-        #              label="check_dataclass_missing", score=score, **kwargs)
-    if not fields:
-        return gently("Dataclasses are not supported in this version of Python", label="dataclasses_not_supported")
-    # Now Check the fields
-    actual_fields = {field.name: get_pedal_type_from_value(getattr(unwrap_value(value), field.name), evaluate) for field
-                     in fields(unwrap_value(value))}
-    expected_fields = {field.name: field.type for field in fields(dataclass)}
-    # Number of fields
-    expected_arity = len(expected_fields)
-    actual_arity = len(actual_fields)
-    if actual_arity < expected_arity:
-        return too_few_fields(name, actual_arity, expected_arity, **kwargs)
-    elif actual_arity > expected_arity:
-        return too_many_fields(name, actual_arity, expected_arity, **kwargs)
-    # Checks each field's name and type
-    for actual_field_name, actual_field_type in actual_fields.items():
-        if actual_field_name not in expected_fields:
-            return unknown_field(name, actual_field_name, **kwargs)
-        expected_field_type = expected_fields[actual_field_name]
-        expected_field_type = normalize_type(expected_field_type, evaluate).as_type()
-        try:
-            actual_field_type = normalize_type(actual_field_type, evaluate).as_type()
-        except ValueError as e:
-            return invalid_field_type(name, actual_field_name, actual_field_type, expected_field_type, **kwargs)
-        if not is_subtype(actual_field_type, expected_field_type):
-            return wrong_fields_type(name, actual_field_name, actual_field_type,
-                                     expected_field_type, **kwargs)
-    return None
-
-
-class wheat_chaff_game_class(assert_group):
-    message_template = """
-I ran your test cases against some of my own implementations of {name:name}.
-I had {wheat_count} programs I expected to pass, and {chaff_count} programs I expected to fail.
-{wheat_outcome}{chaff_outcome}
-{wheat_names}{chaff_names}
-"""
-
-    def __init__(self, name, wheats, chaffs, **kwargs):
-        super().__init__(name=name, **kwargs)
-        self.wheats = wheats
-        self.correct_wheats = []
-        self.chaffs = chaffs
-        self.correct_chaffs = []
-        self.points = 0
-        self.points_possible = 2
-        self.fields['name'] = name
-        self.fields['wheat_count'] = len(wheats)
-        self.fields['chaff_count'] = len(chaffs)
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        self.report.stop_group(self)
-        self.format_message()
-        self._handle_condition()
-        return False
-
-    def format_message(self):
-        missing_wheats = len(self.wheats) - len(self.correct_wheats)
-        if missing_wheats:
-            self.fields['wheat_outcome'] = f"Your tests did not pass {missing_wheats} of my good programs.\n"
-            names = "\n".join([name for name in self.wheats.keys() if name not in self.correct_wheats])
-            self.fields[
-                'wheat_names'] = "Here are the names for the good programs that incorrectly failed on your test cases:\n" + self.report.format.output(
-                names) + "\n"
-        else:
-            self.fields['wheat_outcome'] = "Your tests passed all of my good programs.\n"
-            self.fields['wheat_names'] = ""
-        missing_chaffs = len(self.chaffs) - len(self.correct_chaffs)
-        if missing_chaffs:
-            self.fields['chaff_outcome'] = f"Your tests did not catch {missing_chaffs} of my bad programs.\n"
-            names = "\n".join([name for name in self.chaffs.keys() if name not in self.correct_chaffs])
-            self.fields[
-                'chaff_names'] = "Here are the names for the bad programs that incorrectly passed your tests:\n" + self.report.format.output(
-                names)
-        else:
-            self.fields['chaff_outcome'] = "At least one of your tests correctly failed for all of my bad programs.\n"
-            self.fields['chaff_names'] = ""
-
-    def wheat_outcome(self, wheat, success):
-        if success:
-            self.points += 1 / len(self.wheats)
-            self.correct_wheats.append(wheat)
-
-    def chaff_outcome(self, chaff, failure):
-        if failure:
-            self.points += 1 / len(self.chaffs)
-            self.correct_chaffs.append(chaff)
-
-
-
-    def condition(self):
-        correct = len(self.correct_wheats) + len(self.correct_chaffs)
-        possible = len(self.wheats) + len(self.chaffs)
-        return correct < possible
-
-
-def partial_credit_logic(cases, score, partial_credit):
-    if isinstance(partial_credit, bool):
-        if partial_credit:
-            # Specify total score for all test cases, divide by # of cases passed | True, using `score`
-            if score:
-                return [str(Score.parse(score) / len(cases)) for case in cases]
-            else:
-                return [None for case in cases]
-        else:
-            # Specify total score for all test cases, no partial credit | False, using `score`
-            return [None for case in cases]
-    elif isinstance(partial_credit, (int, str, float)):
-        # Specify exact score for each test case, with single value | str
-        return [partial_credit for case in cases]
-    else:
-        # Specify exact score for each test case, individually | list[str]
-        return partial_credit
-
-
-def get_success_passed_failed_total_reason(student):
-    student = get_student_data()
-    if 'assert_equal' not in student:
-        return False, 0, 0, 0, "Failed to import `assert_equal`"
-    assert_equal = student['assert_equal']
-    if not hasattr(assert_equal, 'student_tests'):
-        return False, 0, 0, 0, "The `assert_equal` function has been modified."
-    student_tests = assert_equal.student_tests
-    return True, student_tests.successes, student_tests.failures, student_tests.tests, ''
-
-
-def check_type_signature(function_name, function, type_signature, type_failures):
-    if type_signature is None:
-        return function
-
-    def check_types(*args, **kwargs):
-        if len(type_signature)-1 != len(args):
-            type_failures.append(TypeError(f"Expected {len(type_signature)-1} arguments, but got {len(args)}"))
-        for i, (arg, expected_type) in enumerate(zip(args, type_signature[:-1])):
-            expected_type, _ = type_to_pedal_type(expected_type)
-            arg = value_to_pedal_type(arg)
-            if not is_subtype(arg, expected_type):
-                type_failures.append(f"Argument {i} should be {expected_type}, but got {type(arg)}")
-        result = function(*args, **kwargs)
-        expected_type, _ = type_to_pedal_type(type_signature[-1])
-        result_type = value_to_pedal_type(result)
-        if not is_subtype(result_type, expected_type):
-            type_failures.append(f"Expected return type of {expected_type}, but got {result_type}")
-        return result
-
-    return check_types
-
-
-def wheat_chaff_game(function_name, wheats, chaffs,
-                     else_message=None, score=None, partial_credit=True, type_signature=None,
-                     **kwargs):
-    report = kwargs.get('report', MAIN_REPORT)
-    each_score = partial_credit_logic([0] * (len(wheats) + len(chaffs)), score, partial_credit)
-    type_failures = []
-    with wheat_chaff_game_class(function_name, wheats, chaffs, **kwargs) as group_result:
-        sandbox = get_sandbox(report)
-        last = 0
-        for kind, iterator in [("wheat", wheats.items()), ("chaff", chaffs.items())]:
-            for i, (name, wheat) in enumerate(iterator, start=last):
-                clear_student_data()
-                student = get_student_data(report)
-                student[function_name] = check_type_signature(function_name, wheat, type_signature, type_failures)
-                result = run(report=report, before='from bakery import assert_equal\nassert_equal.student_tests.reset()')
-                success, passed, failed, total, reason = get_success_passed_failed_total_reason(result)
-                if kind == 'wheat':
-                    group_result.wheat_outcome(name, not sandbox.exception and not failed and success and passed)
-                else:
-                    group_result.chaff_outcome(name, sandbox.exception or failed or not success)
-                if 'assert_equal' in student:
-                    student['assert_equal'].student_tests.reset()
-                last = i
-
-    if type_failures:
-        return gently(f"""I ran your test cases against some of my own implementations of {function_name}.
-At least one of your tests had the wrong parameter or return type.
-Make sure that all of your tests have valid types.""", label='wheat_chaff_game_types', title='Invalid Type for Test', **kwargs)
-    if partial_credit is False:
-        group_result.score = score
-    else:
-        group_result.valence = group_result.POSITIVE_VALENCE
-        group_result.score = group_result.points / group_result.points_possible
-    return not group_result
+"""
+Unifying collection of all the commands in ``pedal.assertions``.
+"""
+from pedal.core.commands import gently
+from pedal.core.scoring import Score, combine_scores
+from pedal.sandbox.commands import call, clear_student_data, run, get_sandbox, CommandBlock
+from pedal.assertions.static import *
+from pedal.assertions.runtime import *
+from pedal.assertions.runtime import _FIELDS
+from pedal.assertions.positive import close_output, correct_output
+from pedal.types.new_types import is_subtype
+from pedal.assertions.testing_libraries import *
+
+try:
+    from dataclasses import fields
+except:
+    fields = None
+
+
+class unit_test(assert_group):
+    justification_template = ("Some of the feedback in this group was triggered.",
+                              "None of the feedback in this group was triggered.")
+
+    """def __init__(self, function_name, given_partial_credit=None, given_score=None, **kwargs):
+        super().__init__(function_name, **kwargs)
+        self.given_partial_credit = given_partial_credit
+        self.given_score = given_score
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        super().__exit__(exc_type, exc_value, traceback)
+        if self.given_partial_credit is False:
+            self.score = self.given_score
+        else:
+            self.valence = self.POSITIVE_VALENCE
+            self.score = combine_scores([success.score for success in self.successes],
+                                        [failure.score for failure in self.failures] +
+                                        [error.score for error in self.errors])
+        return False"""
+
+
+_unit_test_class = unit_test
+
+
+def unit_test(function, *tests, else_message=None, else_message_template=None,
+              score=None, partial_credit=False,
+              assert_function=None, context=None, **kwargs):
+    """
+    Helper function for quickly unit testing.
+
+    * Specify exact score for each test case, individually | list[str]
+    * Specify exact score for each test case, with single value | str
+    * Specify total score for all test cases, no partial credit | False, using `score`
+    * Specify total score for all test cases, divide by # of cases passed | True, using `score`
+
+    Args:
+        assert_function: Override the assert function (defaults to assert_equal)
+        function (str): The name of the function to test.
+        *tests (): The test cases to run. Each test case is a tuple of the input/output pairs.
+        else_message (str): The message to present as a positive if the
+             tests all pass.
+        else_message_template (str): The template for the else_message, to be formatted.
+        score (str): The score to give overall/per test case, depending on
+            partial_credit.
+        partial_credit (bool or str or list[str]): Whether to give credit for
+            each unit test as a percentage of the whole (True), or to only give
+            points for passing all the tests (False). Defaults to False.
+            If a list is passed, those scores will be used per test case.
+        context (Sandbox or CommandBlock): The context to run the function in.
+        **kwargs ():
+
+    Returns:
+
+    """
+    if assert_function is None:
+        assert_function = assert_equal
+    each_score = partial_credit_logic(tests, score, partial_credit)
+    # Handle context
+    if context is True:
+        context = get_sandbox().get_context()
+    elif context:
+        if isinstance(context, Sandbox):
+            context = context.get_context()
+        elif isinstance(context, CommandBlock):
+            context = context.context
+        else:
+            context = get_sandbox().get_context(context._actual_context_id)
+    #if not tests:
+    #    return _unit_test_class(function,
+    #                             else_message=else_message,
+    #                             else_message_template=else_message_template,
+    #                             context=context, given_partial_credit=partial_credit,
+    #                             given_score=score, **kwargs)
+    # TODO: Make it so unit_test can document its cases
+    #with _unit_test_class(function,
+    #                     else_message=else_message,
+    #                     else_message_template=else_message_template,
+    #                     context=context, given_partial_credit=partial_credit,
+    #                     given_score=score, **kwargs) as group_result:
+    with _unit_test_class(function, else_message=else_message,
+                          else_message_template=else_message_template,
+                          context=context, **kwargs) as group_result:
+        for test_index, test in enumerate(tests):
+            args, expected = test
+            if isinstance(args, str):
+                assert_function(call(function, args_locals=[args]), expected, score=each_score[test_index], **kwargs)
+            else:
+                assert_function(call(function, *args), expected, score=each_score[test_index], **kwargs)
+    if partial_credit is False:
+        group_result.score = score
+    else:
+        group_result.valence = group_result.POSITIVE_VALENCE
+        group_result.score = combine_scores([success.score for success in group_result.successes],
+                                            [failure.score for failure in group_result.failures] +
+                                            [error.score for error in group_result.errors])
+
+    return not group_result
+
+
+class check_dataclass_error(RuntimeAssertionFeedback):
+    justification = "Value is not a dataclass"
+    _expected_verb = "to be"
+    _inverse_operator = "is not"
+
+    def __init__(self, value, **kwargs):
+        super().__init__(SandboxedValue(value), ExactValue("a dataclass"), **kwargs)
+
+def check_dataclass_instance(value, dataclass, else_message=None, score=None, partial_credit=False, **kwargs):
+    report = kwargs.get('report', MAIN_REPORT)
+    name = dataclass.__name__
+    # Check that we weren't given an error
+    if isinstance(value, Exception):
+        return check_dataclass_error(value, score=score, **kwargs)
+        #return gently(f"I evaluated the name {report.format.name(name)} and expected the result to be a dataclass. "
+        #              f"However, there was an error instead.",
+        #              label="check_dataclass_error", score=score, **kwargs)
+    # Get the students' instance as a Pedal Type
+    value_pedal_type = get_pedal_type_from_value(unwrap_value(value), evaluate)
+    # Convert the instructor's version to a Pedal type
+    evaluated_expected_type = evaluate(dataclass) if isinstance(dataclass, str) else dataclass
+    expected_pedal_type = normalize_type(evaluated_expected_type, evaluate)
+    if not isinstance(expected_pedal_type, Exception):
+        expected_pedal_type = expected_pedal_type.as_type()
+        expected_pedal_type_name = expected_pedal_type.singular_name
+    else:
+        expected_pedal_type_name = ""
+    # Make sure the students' version is an actual dataclass
+    singular_name = share_sandbox_context(value_pedal_type.singular_name, value)
+    if not hasattr(unwrap_value(value), _FIELDS):
+        return check_dataclass_error(value, score=score, **kwargs)
+        #return gently(f"I evaluated the name {report.format.name(name)} and expected the result to be a dataclass. "
+        #              f"However, the result was a {report.format.python_expression(str(type(unwrap_value(value))))}",
+        #              label="check_dataclass_missing", score=score, **kwargs)
+    if not fields:
+        return gently("Dataclasses are not supported in this version of Python", label="dataclasses_not_supported")
+    # Now Check the fields
+    actual_fields = {field.name: get_pedal_type_from_value(getattr(unwrap_value(value), field.name), evaluate) for field
+                     in fields(unwrap_value(value))}
+    expected_fields = {field.name: field.type for field in fields(dataclass)}
+    # Number of fields
+    expected_arity = len(expected_fields)
+    actual_arity = len(actual_fields)
+    if actual_arity < expected_arity:
+        return too_few_fields(name, actual_arity, expected_arity, **kwargs)
+    elif actual_arity > expected_arity:
+        return too_many_fields(name, actual_arity, expected_arity, **kwargs)
+    # Checks each field's name and type
+    for actual_field_name, actual_field_type in actual_fields.items():
+        if actual_field_name not in expected_fields:
+            return unknown_field(name, actual_field_name, **kwargs)
+        expected_field_type = expected_fields[actual_field_name]
+        expected_field_type = normalize_type(expected_field_type, evaluate).as_type()
+        try:
+            actual_field_type = normalize_type(actual_field_type, evaluate).as_type()
+        except ValueError as e:
+            return invalid_field_type(name, actual_field_name, actual_field_type, expected_field_type, **kwargs)
+        if not is_subtype(actual_field_type, expected_field_type):
+            return wrong_fields_type(name, actual_field_name, actual_field_type,
+                                     expected_field_type, **kwargs)
+    return None
+
+
+class wheat_chaff_game_class(assert_group):
+    message_template = """
+I ran your test cases against some of my own implementations of {name:name}.
+I had {wheat_count} programs I expected to pass, and {chaff_count} programs I expected to fail.
+{wheat_outcome}{chaff_outcome}
+{wheat_names}{chaff_names}
+"""
+
+    def __init__(self, name, wheats, chaffs, **kwargs):
+        super().__init__(name=name, **kwargs)
+        self.wheats = wheats
+        self.correct_wheats = []
+        self.chaffs = chaffs
+        self.correct_chaffs = []
+        self.points = 0
+        self.points_possible = 2
+        self.fields['name'] = name
+        self.fields['wheat_count'] = len(wheats)
+        self.fields['chaff_count'] = len(chaffs)
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.report.stop_group(self)
+        self.format_message()
+        self._handle_condition()
+        return False
+
+    def format_message(self):
+        missing_wheats = len(self.wheats) - len(self.correct_wheats)
+        if missing_wheats:
+            self.fields['wheat_outcome'] = f"Your tests did not pass {missing_wheats} of my good programs.\n"
+            names = "\n".join([name for name in self.wheats.keys() if name not in self.correct_wheats])
+            self.fields[
+                'wheat_names'] = "Here are the names for the good programs that incorrectly failed on your test cases:\n" + self.report.format.output(
+                names) + "\n"
+        else:
+            self.fields['wheat_outcome'] = "Your tests passed all of my good programs.\n"
+            self.fields['wheat_names'] = ""
+        missing_chaffs = len(self.chaffs) - len(self.correct_chaffs)
+        if missing_chaffs:
+            self.fields['chaff_outcome'] = f"Your tests did not catch {missing_chaffs} of my bad programs.\n"
+            names = "\n".join([name for name in self.chaffs.keys() if name not in self.correct_chaffs])
+            self.fields[
+                'chaff_names'] = "Here are the names for the bad programs that incorrectly passed your tests:\n" + self.report.format.output(
+                names)
+        else:
+            self.fields['chaff_outcome'] = "At least one of your tests correctly failed for all of my bad programs.\n"
+            self.fields['chaff_names'] = ""
+
+    def wheat_outcome(self, wheat, success):
+        if success:
+            self.points += 1 / len(self.wheats)
+            self.correct_wheats.append(wheat)
+
+    def chaff_outcome(self, chaff, failure):
+        if failure:
+            self.points += 1 / len(self.chaffs)
+            self.correct_chaffs.append(chaff)
+
+
+
+    def condition(self):
+        correct = len(self.correct_wheats) + len(self.correct_chaffs)
+        possible = len(self.wheats) + len(self.chaffs)
+        return correct < possible
+
+
+def partial_credit_logic(cases, score, partial_credit):
+    if isinstance(partial_credit, bool):
+        if partial_credit:
+            # Specify total score for all test cases, divide by # of cases passed | True, using `score`
+            if score:
+                return [str(Score.parse(score) / len(cases)) for case in cases]
+            else:
+                return [None for case in cases]
+        else:
+            # Specify total score for all test cases, no partial credit | False, using `score`
+            return [None for case in cases]
+    elif isinstance(partial_credit, (int, str, float)):
+        # Specify exact score for each test case, with single value | str
+        return [partial_credit for case in cases]
+    else:
+        # Specify exact score for each test case, individually | list[str]
+        return partial_credit
+
+
+def get_success_passed_failed_total_reason(student):
+    student = get_student_data()
+    if 'assert_equal' not in student:
+        return False, 0, 0, 0, "Failed to import `assert_equal`"
+    assert_equal = student['assert_equal']
+    if not hasattr(assert_equal, 'student_tests'):
+        return False, 0, 0, 0, "The `assert_equal` function has been modified."
+    student_tests = assert_equal.student_tests
+    return True, student_tests.successes, student_tests.failures, student_tests.tests, ''
+
+
+def check_type_signature(function_name, function, type_signature, type_failures):
+    if type_signature is None:
+        return function
+
+    def check_types(*args, **kwargs):
+        if len(type_signature)-1 != len(args):
+            type_failures.append(TypeError(f"Expected {len(type_signature)-1} arguments, but got {len(args)}"))
+        for i, (arg, expected_type) in enumerate(zip(args, type_signature[:-1])):
+            expected_type, _ = type_to_pedal_type(expected_type)
+            arg = value_to_pedal_type(arg)
+            if not is_subtype(arg, expected_type):
+                type_failures.append(f"Argument {i} should be {expected_type}, but got {type(arg)}")
+        result = function(*args, **kwargs)
+        expected_type, _ = type_to_pedal_type(type_signature[-1])
+        result_type = value_to_pedal_type(result)
+        if not is_subtype(result_type, expected_type):
+            type_failures.append(f"Expected return type of {expected_type}, but got {result_type}")
+        return result
+
+    return check_types
+
+
+def wheat_chaff_game(function_name, wheats, chaffs,
+                     else_message=None, score=None, partial_credit=True, type_signature=None,
+                     **kwargs):
+    report = kwargs.get('report', MAIN_REPORT)
+    each_score = partial_credit_logic([0] * (len(wheats) + len(chaffs)), score, partial_credit)
+    type_failures = []
+    with wheat_chaff_game_class(function_name, wheats, chaffs, **kwargs) as group_result:
+        sandbox = get_sandbox(report)
+        last = 0
+        for kind, iterator in [("wheat", wheats.items()), ("chaff", chaffs.items())]:
+            for i, (name, wheat) in enumerate(iterator, start=last):
+                clear_student_data()
+                student = get_student_data(report)
+                student[function_name] = check_type_signature(function_name, wheat, type_signature, type_failures)
+                result = run(report=report, before='from bakery import assert_equal\nassert_equal.student_tests.reset()')
+                success, passed, failed, total, reason = get_success_passed_failed_total_reason(result)
+                if kind == 'wheat':
+                    group_result.wheat_outcome(name, not sandbox.exception and not failed and success and passed)
+                else:
+                    group_result.chaff_outcome(name, sandbox.exception or failed or not success)
+                if 'assert_equal' in student:
+                    student['assert_equal'].student_tests.reset()
+                last = i
+
+    if type_failures:
+        return gently(f"""I ran your test cases against some of my own implementations of {function_name}.
+At least one of your tests had the wrong parameter or return type.
+Make sure that all of your tests have valid types.""", label='wheat_chaff_game_types', title='Invalid Type for Test', **kwargs)
+    if partial_credit is False:
+        group_result.score = score
+    else:
+        group_result.valence = group_result.POSITIVE_VALENCE
+        group_result.score = group_result.points / group_result.points_possible
+    return not group_result
```

### Comparing `pedal-2.6.1/pedal/assertions/feedbacks.py` & `pedal-2.6.2/pedal/assertions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/assertions/functions.py` & `pedal-2.6.2/pedal/assertions/functions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/assertions/organizers.py` & `pedal-2.6.2/pedal/assertions/organizers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/assertions/positive.py` & `pedal-2.6.2/pedal/assertions/positive.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/assertions/runtime.py` & `pedal-2.6.2/pedal/assertions/runtime.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/assertions/setup.py` & `pedal-2.6.2/pedal/assertions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/assertions/static.py` & `pedal-2.6.2/pedal/assertions/static.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/assertions/testing_libraries.py` & `pedal-2.6.2/pedal/assertions/testing_libraries.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/assertions/unittest.py` & `pedal-2.6.2/pedal/assertions/unittest.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/cait/ast_helpers.py` & `pedal-2.6.2/pedal/cait/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/cait/ast_map.py` & `pedal-2.6.2/pedal/cait/ast_map.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/cait/cait_api.py` & `pedal-2.6.2/pedal/cait/cait_api.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/cait/cait_node.py` & `pedal-2.6.2/pedal/cait/cait_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/cait/find_node.py` & `pedal-2.6.2/pedal/cait/find_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/cait/stretchy_tree_matching.py` & `pedal-2.6.2/pedal/cait/stretchy_tree_matching.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/command_line/command_line.py` & `pedal-2.6.2/pedal/command_line/command_line.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,168 +1,170 @@
-"""
-A tool for running Pedal from the Command Line
-
-./pedal command line interface
-    simple example (single ICS, single student file)
-    simple sandbox for just quickly running students code with no frills or extra behavior
-        Maybe this is the "default" ICS?
-    unit test a given curriculum (many ICS, many student files per)
-    regrade some assignments, spit out subject/assignment/context (one ICS, many many student files)
-    get summary stats from ProgSnap file (many ICS, many submissions
-    Spit out the justifications alongside the potential feedback`
-    Run the students code in a sandbox and spit out the runtime results
-
-ProgSnap file with submissions AND assignments (+other info)
-    Just one parameter then
-ProgSnap file with only submissions, ICS is separate
-    Two parameters
-Single ICS file
-    Single student file
-    Archive Format
-        Regular directory
-        ZIP
-        ProgSnap Folder
-        ProgSnap SQL
-    Structure
-        Each file is a python file representing their submission:
-            .+\.py
-            Could have accompanying Markdown file
-        Each folder is a submission
-            .+/.+\.py
-Folder of ICS files
-    Potentially, submissions are within an accompanying "submissions" folder
-    Regex for matching ICS files?
-
-
-
-argparse options
-    -i <instructor_control_script | python file or directory of scripts>
-    -s <student_submission | single python file, directory of files, progsnap file>
-    -o <output_file>
-    -f <output format: Feedback, Grade, Debug mode, Unit Tests, research stats, Sandbox>
-
-For each ICS we want to run
-    For each student submission
-        safely run it
-    Potentially combine results
-
-Config settings
-    seed
-    create_missing_outputs
-"""
-
-import argparse
-from pedal.command_line.modes import MODES
-from pedal.environments import ALL_ENVIRONMENTS
-
-
-def main(args=None):
-    """
-    Actually runs Pedal from the command line.
-
-    Args:
-        args (argparse.Namespace): The arguments parsed from the command line.
-    """
-    # Get command line arguments, unless we were explicitly given them.
-    if args is None:
-        args = parse_args()
-    pipeline = MODES.PIPELINES[args.mode]
-    return pipeline(args).execute()
-
-
-def parse_args(reduced_mode=False):
-    """ Parse the arguments passed into the command line. """
-    parser = argparse.ArgumentParser(description='Run instructor control '
-                                                 'script on student submissions.')
-    parser.add_argument('mode', help="What kind of Pedal analysis you're running",
-                        choices=list(MODES.PIPELINES))
-    if not reduced_mode:
-        parser.add_argument('instructor', help='The path to the instructor control '
-                                               'script, or multiple scripts.')
-    parser.add_argument('submissions', help='The path to the student submissions.'
-                                            ' Defaults to a folder named '
-                                            'submissions adjacent to the '
-                                            'instructor control script.',
-                        default='submissions',
-                        nargs='?')
-    parser.add_argument("--alternate_filenames",
-                        help="A semicolon separated list of potential filenames to try if the main isn't found.",
-                        default="")
-    # TODO: Handle output to file
-    parser.add_argument('--output', '-o',
-                        help='The output file path for the result. Defaults to stdout.',
-                        default='stdout')
-    parser.add_argument('--config', '-c',
-                        help="Uses the configuration file to get settings.")
-    parser.add_argument('--create_output', '-m',
-                        help="In verify mode, creates any missing outputs.",
-                        action='store_true')
-    parser.add_argument('--environment', '-e',
-                        help="Sets the environment context for this script, which"
-                             " can run special setups and override tools as"
-                             " needed.", default='standard', choices=ALL_ENVIRONMENTS)
-    parser.add_argument('--instructor_name',
-                        help="Sets the name of the instructor file to something"
-                             " more friendly. If not given, then will default"
-                             " to the instructor filename.", default=None)
-    parser.add_argument('--progsnap_profile',
-                        default='blockpy', # TODO: Change this biased default
-                        help="Uses the given profile's default settings for"
-                             " loading in a ProgSnap2 dataset",
-                        )
-    parser.add_argument('--include_scripts', help='An optional filter to '
-                                                  'only include certain scripts',
-                        default=None)
-    parser.add_argument('--limit', help='An optional limit to how many'
-                                        ' submissions are run. Mostly for testing'
-                                        ' purposes.',
-                        default=None)
-    parser.add_argument('--resolver', help='Choose a different resolver to use (the name of a function defined in the instructor control script).',
-                        default='resolve')
-    parser.add_argument('--ics_direct', help="Give the instructor code directly"
-                                             " instead of loading from a file.",
-                        default=False, action='store_true')
-    # TODO: Elegant way of skipping specific, common phases
-    parser.add_argument('--skip_tifa', help="Skip using TIFA in the environment",
-                        default=False, action='store_true')
-    parser.add_argument('--skip_run', help="Skip automatically running student code in the environment",
-                        default=False, action='store_true')
-    parser.add_argument('--progsnap_events', help="Choose what level of event"
-                                                  " to capture from Progsnap event"
-                                                  " logs.",
-                        default='run', choices=['run', 'edit', 'last', 'compile'])
-    parser.add_argument('--cache', help='Use the given directory to hold the cache.'
-                                        ' You can use "./" to use the current directory.',
-                        default=False)
-    # TODO: Want to allow for multiple threads too to parallel process data (faster!)
-    parser.add_argument('--threaded', help='Run the instructor script in a separate thread to avoid'
-                                           ' timeout crashes.',
-                        default=False)
-    parser.add_argument('--log_level', help="Set the logging level for Pedal.",
-                        choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
-                        default="ERROR")
-    '''
-    parser.add_argument('--include_submissions', help='An optional REGEX filter '
-                                                      'to only include certain submissions')
-    parser.add_argument('--exclude_submissions', help='An optional REGEX filter '
-                                                      'to remove certain submissions')
-    parser.add_argument('--include_scripts', help='An optional REGEX filter to '
-                                                  'only include certain scripts')
-    parser.add_argument('--exclude_scripts', help='An optional REGEX filter to '
-                                                  'remove certain scripts')
-    parser.add_argument('--parallel_scripts', help="Which style to use for "
-                                                   "running scripts in parallel.",
-                        choices=["threads", "processes", "none"])
-    '''
-    args = parser.parse_args()
-    if args.instructor_name is None:
-        args.instructor_name = args.instructor
-    return args
-
-
-if __name__ == '__main__':
-    main()
-
-# If scripts is a single python file
-# If scripts is a folder
-# If scripts is a zip file
-# If scripts is a ProgSnap SQL file
+"""
+A tool for running Pedal from the Command Line
+
+./pedal command line interface
+    simple example (single ICS, single student file)
+    simple sandbox for just quickly running students code with no frills or extra behavior
+        Maybe this is the "default" ICS?
+    unit test a given curriculum (many ICS, many student files per)
+    regrade some assignments, spit out subject/assignment/context (one ICS, many many student files)
+    get summary stats from ProgSnap file (many ICS, many submissions
+    Spit out the justifications alongside the potential feedback`
+    Run the students code in a sandbox and spit out the runtime results
+
+ProgSnap file with submissions AND assignments (+other info)
+    Just one parameter then
+ProgSnap file with only submissions, ICS is separate
+    Two parameters
+Single ICS file
+    Single student file
+    Archive Format
+        Regular directory
+        ZIP
+        ProgSnap Folder
+        ProgSnap SQL
+    Structure
+        Each file is a python file representing their submission:
+            .+\.py
+            Could have accompanying Markdown file
+        Each folder is a submission
+            .+/.+\.py
+Folder of ICS files
+    Potentially, submissions are within an accompanying "submissions" folder
+    Regex for matching ICS files?
+
+
+
+argparse options
+    -i <instructor_control_script | python file or directory of scripts>
+    -s <student_submission | single python file, directory of files, progsnap file>
+    -o <output_file>
+    -f <output format: Feedback, Grade, Debug mode, Unit Tests, research stats, Sandbox>
+
+For each ICS we want to run
+    For each student submission
+        safely run it
+    Potentially combine results
+
+Config settings
+    seed
+    create_missing_outputs
+"""
+
+import argparse
+from pedal.command_line.modes import MODES
+from pedal.environments import ALL_ENVIRONMENTS
+
+
+def main(args=None):
+    """
+    Actually runs Pedal from the command line.
+
+    Args:
+        args (argparse.Namespace): The arguments parsed from the command line.
+    """
+    # Get command line arguments, unless we were explicitly given them.
+    if args is None:
+        args = parse_args()
+    pipeline = MODES.PIPELINES[args.mode]
+    return pipeline(args).execute()
+
+
+def parse_args(reduced_mode=False):
+    """ Parse the arguments passed into the command line. """
+    parser = argparse.ArgumentParser(description='Run instructor control '
+                                                 'script on student submissions.')
+    parser.add_argument('mode', help="What kind of Pedal analysis you're running",
+                        choices=list(MODES.PIPELINES))
+    if not reduced_mode:
+        parser.add_argument('instructor', help='The path to the instructor control '
+                                               'script, or multiple scripts.')
+    parser.add_argument('submissions', help='The path to the student submissions.'
+                                            ' Defaults to a folder named '
+                                            'submissions adjacent to the '
+                                            'instructor control script.',
+                        default='submissions',
+                        nargs='?')
+    parser.add_argument("--alternate_filenames",
+                        help="A semicolon separated list of potential filenames to try if the main isn't found.",
+                        default="")
+    # TODO: Handle output to file
+    parser.add_argument('--output', '-o',
+                        help='The output file path for the result. Defaults to stdout.',
+                        default='stdout')
+    parser.add_argument('--config', '-c',
+                        help="Uses the configuration file to get settings.")
+    parser.add_argument('--create_output', '-m',
+                        help="In verify mode, creates any missing outputs.",
+                        action='store_true')
+    parser.add_argument('--environment', '-e',
+                        help="Sets the environment context for this script, which"
+                             " can run special setups and override tools as"
+                             " needed.", default='standard', choices=ALL_ENVIRONMENTS)
+    parser.add_argument('--instructor_name',
+                        help="Sets the name of the instructor file to something"
+                             " more friendly. If not given, then will default"
+                             " to the instructor filename.", default=None)
+    parser.add_argument('--progsnap_profile',
+                        default='blockpy', # TODO: Change this biased default
+                        help="Uses the given profile's default settings for"
+                             " loading in a ProgSnap2 dataset",
+                        )
+    parser.add_argument('--include_scripts', help='An optional filter to '
+                                                  'only include certain scripts',
+                        default=None)
+    parser.add_argument('--limit', help='An optional limit to how many'
+                                        ' submissions are run. Mostly for testing'
+                                        ' purposes.',
+                        default=None)
+    parser.add_argument('--resolver', help='Choose a different resolver to use (the name of a function defined in the instructor control script).',
+                        default='resolve')
+    parser.add_argument('--ics_direct', help="Give the instructor code directly"
+                                             " instead of loading from a file.",
+                        default=False, action='store_true')
+    # TODO: Elegant way of skipping specific, common phases
+    parser.add_argument('--skip_tifa', help="Skip using TIFA in the environment",
+                        default=False, action='store_true')
+    parser.add_argument('--skip_run', help="Skip automatically running student code in the environment",
+                        default=False, action='store_true')
+    parser.add_argument('--progsnap_events', help="Choose what level of event"
+                                                  " to capture from Progsnap event"
+                                                  " logs.",
+                        default='run', choices=['run', 'edit', 'last', 'compile'])
+    parser.add_argument('--cache', help='Use the given directory to hold the cache.'
+                                        ' You can use "./" to use the current directory.',
+                        default=False)
+    # TODO: Want to allow for multiple threads too to parallel process data (faster!)
+    parser.add_argument('--threaded', help='Run the instructor script in a separate thread to avoid'
+                                           ' timeout crashes.',
+                        default=False)
+    parser.add_argument('--log_level', help="Set the logging level for Pedal.",
+                        choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
+                        default="ERROR")
+    parser.add_argument('--gpt-api-key', help='Set the GPT API key',
+                        default=None)
+    '''
+    parser.add_argument('--include_submissions', help='An optional REGEX filter '
+                                                      'to only include certain submissions')
+    parser.add_argument('--exclude_submissions', help='An optional REGEX filter '
+                                                      'to remove certain submissions')
+    parser.add_argument('--include_scripts', help='An optional REGEX filter to '
+                                                  'only include certain scripts')
+    parser.add_argument('--exclude_scripts', help='An optional REGEX filter to '
+                                                  'remove certain scripts')
+    parser.add_argument('--parallel_scripts', help="Which style to use for "
+                                                   "running scripts in parallel.",
+                        choices=["threads", "processes", "none"])
+    '''
+    args = parser.parse_args()
+    if args.instructor_name is None:
+        args.instructor_name = args.instructor
+    return args
+
+
+if __name__ == '__main__':
+    main()
+
+# If scripts is a single python file
+# If scripts is a folder
+# If scripts is a zip file
+# If scripts is a ProgSnap SQL file
```

### Comparing `pedal-2.6.1/pedal/command_line/mocks.py` & `pedal-2.6.2/pedal/command_line/mocks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/command_line/modes.py` & `pedal-2.6.2/pedal/command_line/modes.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/command_line/report.py` & `pedal-2.6.2/pedal/command_line/report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/command_line/verify.py` & `pedal-2.6.2/pedal/command_line/verify.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/core/commands.py` & `pedal-2.6.2/pedal/core/commands.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,307 +1,307 @@
-"""
-Imperative style commands for constructing feedback in a convenient way.
-Uses a global report object (MAIN_REPORT).
-"""
-
-__all__ = ['feedback', 'set_success', 'set_correct', 'compliment', 'give_partial', 'explain',
-           'gently', 'hide_correctness', 'suppress', 'log', 'debug',
-           'system_error', 'clear_report', 'get_all_feedback', 'guidance',
-           'contextualize_report', 'Feedback', 'get_submission', 'set_formatter']
-
-from pedal.core.feedback import (Feedback, FeedbackKind, FeedbackCategory,
-                                 FeedbackResponse)
-from pedal.core.report import MAIN_REPORT
-
-from pedal.core.submission import Submission
-
-#: Lowercase "function" version that works like other Core Feedback Functions.
-feedback = Feedback
-
-
-# TODO: force_success function, which ignores errors to give the points.
-
-class set_correct(FeedbackResponse):
-    """
-    **(Feedback Function)**
-
-    Creates Successful feedback for the user, indicating that the entire
-    assignment is done.
-    """
-    title = "Complete"
-    message_template = "Great work!"
-    score = 1
-    correct = True
-    category = FeedbackCategory.COMPLETE
-    kind = FeedbackKind.RESULT
-    valence = Feedback.POSITIVE_VALENCE
-
-
-set_success = set_correct
-
-
-class compliment(FeedbackResponse):
-    """
-    Create a positive feedback for the user, potentially on a specific line of
-    code.
-    """
-    category = FeedbackCategory.INSTRUCTOR
-    kind = FeedbackKind.COMPLIMENT
-    valence = Feedback.POSITIVE_VALENCE
-    correct = True
-
-    def __init__(self, message=None, title=None, message_template=None, **kwargs):
-        if title is None:
-            title = message
-        if message is None and message_template is None:
-            raise ValueError("compliment requires at least either message or message_template")
-        super().__init__(message=message, title=title, message_template=message_template, **kwargs)
-
-
-class give_partial(FeedbackResponse):
-    """ Increases the user's current score by the `score`. """
-    title = "Partial Credit"
-    message_template = "Partial credit"
-    category = FeedbackCategory.INSTRUCTOR
-    kind = FeedbackKind.RESULT
-    valence = Feedback.POSITIVE_VALENCE
-    correct = None
-    muted = True
-
-    def __init__(self, value, **kwargs):
-        super().__init__(score=value, **kwargs)
-
-
-class explain(FeedbackResponse):
-    """ Give a high-priority piece of negative feedback to the student. """
-    title = "Instructor Feedback"
-    muted = False
-    category = Feedback.CATEGORIES.INSTRUCTOR
-    kind = FeedbackKind.MISTAKE
-    valence = Feedback.NEGATIVE_VALENCE
-
-    def __init__(self, message=None, message_template=None, **kwargs):
-        if message is None and message_template is None:
-            raise ValueError("explain requires at least either message or message_template")
-        super().__init__(message=message, message_template=message_template, **kwargs)
-
-
-class gently(FeedbackResponse):
-    """
-    Give a low-priority piece of negative feedback to the student.
-
-    Args:
-        message (str): The feedback message to show to the student.
-
-    """
-    title = "Instructor Feedback"
-    priority = Feedback.CATEGORIES.STUDENT
-    muted = False
-    category = Feedback.CATEGORIES.INSTRUCTOR
-    kind = FeedbackKind.MISTAKE
-    valence = Feedback.NEGATIVE_VALENCE
-
-    def __init__(self, message=None, message_template=None, **kwargs):
-        if message is None and message_template is None:
-            raise ValueError("gently requires at least either message or message_template")
-        super().__init__(message=message, message_template=message_template, **kwargs)
-
-
-class guidance(FeedbackResponse):
-    """ Give instructions about a question. """
-    title = "Instructor Guidance"
-    category = Feedback.CATEGORIES.INSTRUCTIONS
-    kind = FeedbackKind.INSTRUCTIONAL
-    valence = Feedback.NEUTRAL_VALENCE
-
-    def __init__(self, message=None, message_template=None, **kwargs):
-        if message is None and message_template is None:
-            raise ValueError("compliment requires at least either message or message_template")
-        super().__init__(message=message, message_template=message_template, **kwargs)
-
-
-def hide_correctness(report=MAIN_REPORT):
-    """
-    Force the report to not indicate score/correctness.
-
-    Args:
-        report (:py:class:`pedal.core.report.Report`): The report object to
-            hide correctness on.
-    """
-    report.hide_correctness()
-
-
-def suppress(category=None, label=True, fields=None, report=MAIN_REPORT):
-    """
-    Hides a given category or label within a category from being considered
-    by the resolver.
-
-    Args:
-        category (str): The general feedback category to suppress within.
-            Should be a member of
-            :py:class:`pedal.core.feedback_category.FeedbackCategory`.
-        label (str or bool): The specific feedback label to suppress, or
-            True if all the labels within this category should be suppressed.
-        fields (dict): The fields that will be exactly matched to suppress a
-            given feedback. The keys should be strings.
-        report (:py:class:`~pedal.core.report.Report`): The report object to
-            suppress information within.
-    """
-    report.suppress(category, label, fields)
-
-
-def log(*items, sep=" ", **kwargs):
-    """
-    Attach logging information to the Report as a piece of feedback.
-
-    Args:
-        sep: The separator to use between items (defaults to space).
-        items (Any): Any set of values to log information about. Will be
-            converted to strings using `str` if not already strings.
-
-    Returns:
-
-    """
-    kwargs.setdefault('category', Feedback.CATEGORIES.SYSTEM)
-    kwargs.setdefault('muted', True)
-    kwargs.setdefault('valence', Feedback.NEUTRAL_VALENCE)
-    message = sep.join(item if isinstance(item, str) else str(item)
-                       for item in items)
-    feedback(message=message, label="log", **kwargs)
-
-
-def debug(*items, **kwargs):
-    """
-    Attach logging information to the Report as a piece of feedback.
-    Works at a higher priority than :py:func:`~pedal.core.commands.log` and
-    does not attempt to convert to strings.
-
-    TODO: Consider updating to match `log`
-
-    Args:
-        items (Any): Any set of values to log information about. Will be
-            converted to strings using `str` if not already strings.
-
-    Returns:
-
-    """
-    kwargs.setdefault('category', Feedback.CATEGORIES.SYSTEM)
-    kwargs.setdefault('muted', True)
-    kwargs.setdefault('priority', 'high')
-    kwargs.setdefault('valence', Feedback.NEGATIVE_VALENCE)
-    for item in items:
-        item = item
-        cloned_kwargs = kwargs.copy()
-        cloned_kwargs.setdefault('message', item)
-        feedback(label="debug", **kwargs)
-
-
-def clear_report(report=MAIN_REPORT):
-    """
-    Removes all existing data from the report, including any submissions,
-    suppressions, feedback, and Tool data.
-
-    Args:
-        report: The report to clear (defaults to the
-            :py:data:`pedal.core.report.MAIN_REPORT`).
-    """
-    report.clear()
-
-
-def contextualize_report(submission, filename='answer.py', clear=True,
-                         report=MAIN_REPORT):
-    """
-    Updates the report with the submission. By default, clears out any old
-    information in the report. You can pass in either an actual
-    :py:class:`~pedal.core.submission.Submission` or a string representing
-    the code of the submission.
-
-    Args:
-        submission (str or Submission):
-        filename (str or None): If the `submission` was not a
-            :py:class:`~pedal.core.submission.Submission`, then this will be
-            used as the filename for the code given in ``submission``.
-        clear (bool): Whether or not to clear the report before attaching
-            the submission.
-        report: The report to attach this feedback to (defaults to the
-            :py:data:`~pedal.core.report.MAIN_REPORT`).
-    """
-    if not isinstance(submission, Submission):
-        submission = Submission(files={filename: submission})
-    if clear:
-        report.clear()
-    report.contextualize(submission)
-
-
-def get_submission(report=MAIN_REPORT) -> Submission:
-    """
-    Get the current submission from the given report, or the default MAIN_REPORT.
-
-    Args:
-        report: The report to attach this feedback to (defaults to the
-            :py:data:`~pedal.core.report.MAIN_REPORT`).
-
-    Returns:
-        Submission: The current submission
-    """
-    return report.submission
-
-
-def get_all_feedback(report=MAIN_REPORT):
-    """
-    Gives access to the list of feedback from the report. Usually, you won't
-    need this; but if you want to build on the results of earlier tools, it
-    can be a useful mechanism.
-
-    TODO: Provide mechanisms for conveniently searching feedback
-
-    Args:
-        report (:py:class:`~pedal.core.report.Report`): The report to attach
-            this feedback to (defaults to the
-            :py:data:`~pedal.core.report.MAIN_REPORT`).
-
-    Returns:
-        List[:py:class:`~pedal.core.feedback.Feedback`]: A list of feedback
-            objects from the report.
-    """
-    return report.feedback
-
-
-class system_error(FeedbackResponse):
-    """
-    Call this function to indicate that something has gone wrong at the system
-    level with Pedal. Ideally, this doesn't happen, but sometimes errors
-    cascade and its polite for tools to suggest that they are not working
-    correctly. These will not usually be reported to the student.
-    """
-    title = "System Error"
-    category = Feedback.CATEGORIES.SYSTEM
-    kind = FeedbackKind.META
-    valence = Feedback.NEUTRAL_VALENCE
-    muted = True
-
-
-# TODO: set_line_offset(offset, filename='answer.py')
-
-def set_formatter(formatter, report=MAIN_REPORT):
-    """
-    Set the formatter for the given report.
-
-    Args:
-        formatter (Formatter): The formatter class to use. If you wish to use an instance instead,
-            you'll need to call `set_formatter` on the report instance instead.
-        report (:py:class:`~pedal.core.report.Report`): The report to attach
-            this feedback to (defaults to the
-            :py:data:`~pedal.core.report.MAIN_REPORT`).
-    """
-    report.set_formatter(formatter(report))
-
-
-def set_pools(pools, report=MAIN_REPORT):
-    """
-    Ability to have A/B testing on a per-feedback basis.
-
-    Args:
-        pools (int or list[str]): Either the number of pools or the names of the pools. If a number is given,
-            the pools are given the identifiers A/B/C/etc.
-    """
+"""
+Imperative style commands for constructing feedback in a convenient way.
+Uses a global report object (MAIN_REPORT).
+"""
+
+__all__ = ['feedback', 'set_success', 'set_correct', 'compliment', 'give_partial', 'explain',
+           'gently', 'hide_correctness', 'suppress', 'log', 'debug',
+           'system_error', 'clear_report', 'get_all_feedback', 'guidance',
+           'contextualize_report', 'Feedback', 'get_submission', 'set_formatter']
+
+from pedal.core.feedback import (Feedback, FeedbackKind, FeedbackCategory,
+                                 FeedbackResponse)
+from pedal.core.report import MAIN_REPORT
+
+from pedal.core.submission import Submission
+
+#: Lowercase "function" version that works like other Core Feedback Functions.
+feedback = Feedback
+
+
+# TODO: force_success function, which ignores errors to give the points.
+
+class set_correct(FeedbackResponse):
+    """
+    **(Feedback Function)**
+
+    Creates Successful feedback for the user, indicating that the entire
+    assignment is done.
+    """
+    title = "Complete"
+    message_template = "Great work!"
+    score = 1
+    correct = True
+    category = FeedbackCategory.COMPLETE
+    kind = FeedbackKind.RESULT
+    valence = Feedback.POSITIVE_VALENCE
+
+
+set_success = set_correct
+
+
+class compliment(FeedbackResponse):
+    """
+    Create a positive feedback for the user, potentially on a specific line of
+    code.
+    """
+    category = FeedbackCategory.INSTRUCTOR
+    kind = FeedbackKind.COMPLIMENT
+    valence = Feedback.POSITIVE_VALENCE
+    correct = True
+
+    def __init__(self, message=None, title=None, message_template=None, **kwargs):
+        if title is None:
+            title = message
+        if message is None and message_template is None:
+            raise ValueError("compliment requires at least either message or message_template")
+        super().__init__(message=message, title=title, message_template=message_template, **kwargs)
+
+
+class give_partial(FeedbackResponse):
+    """ Increases the user's current score by the `score`. """
+    title = "Partial Credit"
+    message_template = "Partial credit"
+    category = FeedbackCategory.INSTRUCTOR
+    kind = FeedbackKind.RESULT
+    valence = Feedback.POSITIVE_VALENCE
+    correct = None
+    muted = True
+
+    def __init__(self, value, **kwargs):
+        super().__init__(score=value, **kwargs)
+
+
+class explain(FeedbackResponse):
+    """ Give a high-priority piece of negative feedback to the student. """
+    title = "Instructor Feedback"
+    muted = False
+    category = Feedback.CATEGORIES.INSTRUCTOR
+    kind = FeedbackKind.MISTAKE
+    valence = Feedback.NEGATIVE_VALENCE
+
+    def __init__(self, message=None, message_template=None, **kwargs):
+        if message is None and message_template is None:
+            raise ValueError("explain requires at least either message or message_template")
+        super().__init__(message=message, message_template=message_template, **kwargs)
+
+
+class gently(FeedbackResponse):
+    """
+    Give a low-priority piece of negative feedback to the student.
+
+    Args:
+        message (str): The feedback message to show to the student.
+
+    """
+    title = "Instructor Feedback"
+    priority = Feedback.CATEGORIES.STUDENT
+    muted = False
+    category = Feedback.CATEGORIES.INSTRUCTOR
+    kind = FeedbackKind.MISTAKE
+    valence = Feedback.NEGATIVE_VALENCE
+
+    def __init__(self, message=None, message_template=None, **kwargs):
+        if message is None and message_template is None:
+            raise ValueError("gently requires at least either message or message_template")
+        super().__init__(message=message, message_template=message_template, **kwargs)
+
+
+class guidance(FeedbackResponse):
+    """ Give instructions about a question. """
+    title = "Instructor Guidance"
+    category = Feedback.CATEGORIES.INSTRUCTIONS
+    kind = FeedbackKind.INSTRUCTIONAL
+    valence = Feedback.NEUTRAL_VALENCE
+
+    def __init__(self, message=None, message_template=None, **kwargs):
+        if message is None and message_template is None:
+            raise ValueError("compliment requires at least either message or message_template")
+        super().__init__(message=message, message_template=message_template, **kwargs)
+
+
+def hide_correctness(report=MAIN_REPORT):
+    """
+    Force the report to not indicate score/correctness.
+
+    Args:
+        report (:py:class:`pedal.core.report.Report`): The report object to
+            hide correctness on.
+    """
+    report.hide_correctness()
+
+
+def suppress(category=None, label=True, fields=None, report=MAIN_REPORT):
+    """
+    Hides a given category or label within a category from being considered
+    by the resolver.
+
+    Args:
+        category (str): The general feedback category to suppress within.
+            Should be a member of
+            :py:class:`pedal.core.feedback_category.FeedbackCategory`.
+        label (str or bool): The specific feedback label to suppress, or
+            True if all the labels within this category should be suppressed.
+        fields (dict): The fields that will be exactly matched to suppress a
+            given feedback. The keys should be strings.
+        report (:py:class:`~pedal.core.report.Report`): The report object to
+            suppress information within.
+    """
+    report.suppress(category, label, fields)
+
+
+def log(*items, sep=" ", **kwargs):
+    """
+    Attach logging information to the Report as a piece of feedback.
+
+    Args:
+        sep: The separator to use between items (defaults to space).
+        items (Any): Any set of values to log information about. Will be
+            converted to strings using `str` if not already strings.
+
+    Returns:
+
+    """
+    kwargs.setdefault('category', Feedback.CATEGORIES.SYSTEM)
+    kwargs.setdefault('muted', True)
+    kwargs.setdefault('valence', Feedback.NEUTRAL_VALENCE)
+    message = sep.join(item if isinstance(item, str) else str(item)
+                       for item in items)
+    feedback(message=message, label="log", **kwargs)
+
+
+def debug(*items, **kwargs):
+    """
+    Attach logging information to the Report as a piece of feedback.
+    Works at a higher priority than :py:func:`~pedal.core.commands.log` and
+    does not attempt to convert to strings.
+
+    TODO: Consider updating to match `log`
+
+    Args:
+        items (Any): Any set of values to log information about. Will be
+            converted to strings using `str` if not already strings.
+
+    Returns:
+
+    """
+    kwargs.setdefault('category', Feedback.CATEGORIES.SYSTEM)
+    kwargs.setdefault('muted', True)
+    kwargs.setdefault('priority', 'high')
+    kwargs.setdefault('valence', Feedback.NEGATIVE_VALENCE)
+    for item in items:
+        item = item
+        cloned_kwargs = kwargs.copy()
+        cloned_kwargs.setdefault('message', item)
+        feedback(label="debug", **kwargs)
+
+
+def clear_report(report=MAIN_REPORT):
+    """
+    Removes all existing data from the report, including any submissions,
+    suppressions, feedback, and Tool data.
+
+    Args:
+        report: The report to clear (defaults to the
+            :py:data:`pedal.core.report.MAIN_REPORT`).
+    """
+    report.clear()
+
+
+def contextualize_report(submission, filename='answer.py', clear=True,
+                         report=MAIN_REPORT):
+    """
+    Updates the report with the submission. By default, clears out any old
+    information in the report. You can pass in either an actual
+    :py:class:`~pedal.core.submission.Submission` or a string representing
+    the code of the submission.
+
+    Args:
+        submission (str or Submission):
+        filename (str or None): If the `submission` was not a
+            :py:class:`~pedal.core.submission.Submission`, then this will be
+            used as the filename for the code given in ``submission``.
+        clear (bool): Whether or not to clear the report before attaching
+            the submission.
+        report: The report to attach this feedback to (defaults to the
+            :py:data:`~pedal.core.report.MAIN_REPORT`).
+    """
+    if not isinstance(submission, Submission):
+        submission = Submission(files={filename: submission})
+    if clear:
+        report.clear()
+    report.contextualize(submission)
+
+
+def get_submission(report=MAIN_REPORT) -> Submission:
+    """
+    Get the current submission from the given report, or the default MAIN_REPORT.
+
+    Args:
+        report: The report to attach this feedback to (defaults to the
+            :py:data:`~pedal.core.report.MAIN_REPORT`).
+
+    Returns:
+        Submission: The current submission
+    """
+    return report.submission
+
+
+def get_all_feedback(report=MAIN_REPORT):
+    """
+    Gives access to the list of feedback from the report. Usually, you won't
+    need this; but if you want to build on the results of earlier tools, it
+    can be a useful mechanism.
+
+    TODO: Provide mechanisms for conveniently searching feedback
+
+    Args:
+        report (:py:class:`~pedal.core.report.Report`): The report to attach
+            this feedback to (defaults to the
+            :py:data:`~pedal.core.report.MAIN_REPORT`).
+
+    Returns:
+        List[:py:class:`~pedal.core.feedback.Feedback`]: A list of feedback
+            objects from the report.
+    """
+    return report.feedback
+
+
+class system_error(FeedbackResponse):
+    """
+    Call this function to indicate that something has gone wrong at the system
+    level with Pedal. Ideally, this doesn't happen, but sometimes errors
+    cascade and its polite for tools to suggest that they are not working
+    correctly. These will not usually be reported to the student.
+    """
+    title = "System Error"
+    category = Feedback.CATEGORIES.SYSTEM
+    kind = FeedbackKind.META
+    valence = Feedback.NEUTRAL_VALENCE
+    muted = True
+
+
+# TODO: set_line_offset(offset, filename='answer.py')
+
+def set_formatter(formatter, report=MAIN_REPORT):
+    """
+    Set the formatter for the given report.
+
+    Args:
+        formatter (Formatter): The formatter class to use. If you wish to use an instance instead,
+            you'll need to call `set_formatter` on the report instance instead.
+        report (:py:class:`~pedal.core.report.Report`): The report to attach
+            this feedback to (defaults to the
+            :py:data:`~pedal.core.report.MAIN_REPORT`).
+    """
+    report.set_formatter(formatter(report))
+
+
+def set_pools(pools, report=MAIN_REPORT):
+    """
+    Ability to have A/B testing on a per-feedback basis.
+
+    Args:
+        pools (int or list[str]): Either the number of pools or the names of the pools. If a number is given,
+            the pools are given the identifiers A/B/C/etc.
+    """
     report.set_pools(pools)
```

### Comparing `pedal-2.6.1/pedal/core/environment.py` & `pedal-2.6.2/pedal/core/environment.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/core/errors.py` & `pedal-2.6.2/pedal/core/errors.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/core/feedback.py` & `pedal-2.6.2/pedal/core/feedback.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,562 +1,562 @@
-"""
-Simple data classes for storing feedback to present to learners.
-"""
-
-__all__ = ['Feedback', 'FeedbackKind', 'FeedbackCategory',
-           "CompositeFeedbackFunction",
-           "FeedbackResponse"]
-
-from pedal.core.formatting import wrap_fields
-from pedal.core.location import Location
-from pedal.core.report import MAIN_REPORT
-from pedal.core.feedback_category import FeedbackKind, FeedbackCategory, FeedbackStatus
-
-PEDAL_DEVELOPERS = ["Austin Cory Bart <acbart@udel.edu>",
-                    "Luke Gusukuma <lukesg08@vt.edu>"]
-
-
-class FeedbackRegistry:
-    def __init__(self):
-        self._registered_feedback = {}
-
-
-class Feedback:
-    """
-    A class for storing raw feedback.
-
-    Attributes:
-        label (str): An internal name for this specific piece of feedback. The
-            label should be an underscore-separated string following the same
-            conventions as names in Python. They do not have to be globally
-            unique, but labels should be as unique as possible (especially
-            within a category).
-        tool (str, optional): An internal name for indicating the tool that created
-            this feedback. Should be taken directly from the Tool itself. If `None`, then
-            this was not created by a tool but directly by the control script.
-        category (str): A human-presentable name showable to the learner, indicating what
-            sort of feedback this falls into (e.g., "runtime", "syntax", "algorithm").
-            More than one feedback will be in a category, but a feedback cannot be in
-            more than one category.
-        kind (str): The pedagogical role of this feedback, e.g., "misconception", "mistake",
-            "hint", "constraint". Usually, a piece of Feedback is pointing out a mistake,
-            but feedback can also be used for various other purposes.
-        justification (str): An instructor-facing string briefly describing why this
-            feedback was selected. Serves as a "TL;DR" for this feedback category, useful
-            for debugging why a piece of feedback appeared.
-        justification_template (str): A markdown-formatted message template that will
-            be used if a ``justification`` is None. Any ``fields`` will be injected
-            into the template IF the ``condition`` is met.
-        priority (str): An indication of how important this feedback is relative to other types
-            of feedback in the same category. Might be "high/medium/low". Exactly how this
-            gets used is up to the resolver, but typically it helps break ties.
-        valence (int): Indicates whether this is negative, positive, or neutral feedback.
-            Either 1, -1, or 0.
-
-        title (str, optional): A formal, student-facing title for this feedback. If None, indicates
-            that the :py:attr:`~pedal.core.feedback.Feedback.label` should be used instead.
-        message (str): A markdown-formatted message (aka also supporting HTML) that could be rendered
-            to the user.
-        message_template (str): A markdown-formatted message template that will
-            be used if a ``message`` is None. Any ``fields`` will be injected
-            into the template IF the ``condition`` is met.
-        fields (Dict[str,Any]): The raw data that was used to interpolate the
-            template to produce the message.
-        location (:py:attr:`~pedal.core.location.Location` or int): Information
-            about specific locations relevant to this message.
-
-        score (int): A numeric score to modify the students' total score, indicating their overall performance.
-            It is ultimately up to the Resolver to decide how to combine all the different scores; a typical
-            strategy would be to add all the scores together for any non-muted feedback.
-        correct (bool): Indicates that the entire submission should be considered correct (success) and that the
-            task is now finished.
-        muted (bool): Whether this piece of feedback is something that should be shown to a student. There are
-            various use cases for muted feedback: they can serve as flags for later conditionals, suppressed
-            default kinds of feedback, or perhaps feedback that is interesting for analysis but not pedagogically
-            helpful to give to the student. They will still contribute to overall score, but not to the correctness
-            of the submission.
-        unscored (bool): Whether this piece of feedback contributes to the score/correctness.
-
-        else_message (str): A string to render as a message when a
-            NEGATIVE valence feedback is NOT triggered, or a POSITIVE valence
-            feedback IS triggered.
-        else_message_template (str): Similar to the ``message_template``, but for the ``else_message``.
-
-        activate (bool): Used for default feedback objects without a custom
-            condition, to indicate whether they should be considered triggered.
-            Defaults to True; setting this to False means that the feedback
-            object will be deactivated. Note that most inheriting Feedback
-            Functions will not respect this parameter.
-
-        author (List[str]): A list of names/emails that indicate who created this piece of feedback. They can be
-            either names, emails, or combinations in the style of `"Cory Bart <acbart@udel.edu>"`.
-        version (str): A version string in the style of Semantic Version (semvar) such as `"0.0.1"`. The last (third)
-            digit should be incremented for small bug fixes/changes. The middle (second) digit should be used for more
-            serious and intense changes. The first digit should be incremented when changes are made on exposure to
-            learners or some other evidence-based motivation.
-        tags (list[:py:class:`~pedal.core.tag.Tag`]): Any tags that you want to
-            attach to this feedback.
-
-        parent (int, str, or `pedal.core.feedback.Feedback`): Information about
-            what logical grouping within the submission this belongs to.
-            Various tools can chunk up a submission (e.g., by section), they
-            can use this field to keep track of how that decision was made.
-            Resolvers can also use this information to organize feedback or to
-            report multiple categories.
-        report (:py:class:`~pedal.core.report.Report`): The Report object to
-            attach this feedback to. Defaults to MAIN_REPORT. Unspecified fields
-            will be filled in by inspecting the current Feedback Function
-            context.
-    """
-
-    POSITIVE_VALENCE = 1
-    NEUTRAL_VALENCE = 0
-    NEGATIVE_VALENCE = -1
-    CATEGORIES = FeedbackCategory
-    KINDS = FeedbackKind
-
-    DEFAULT_FEEDBACK_MESSAGE = "No feedback message provided"
-    DEFAULT_JUSTIFICATION_MESSAGE = "No justification provided"
-    DEFAULT_ELSE_MESSAGE = None
-
-    label = None
-    category = None
-    justification = None
-    justification_template = None
-    constant_fields = None
-    fields = None
-    field_names = None
-    kind = None
-    title = None
-    message = None
-    message_template = None
-    else_message = None
-    else_message_template = None
-    priority = None
-    valence = None
-    location = None
-    score = None
-    correct = None
-    muted = None
-    unscored = None
-    tool = None
-    version = '1.0.0'
-    author = PEDAL_DEVELOPERS
-    tags = None
-    parent = None
-
-    activate: bool
-    _status: str
-    _exception: Exception or None
-    _met_condition: bool
-    _stored_args: tuple
-    _stored_kwargs: dict
-    _override_backups = None
-    _pools = {}
-
-    resolved_score = None
-    unused_message = None
-
-    # MAIN_REPORT
-
-    def __init__(self, *args, label=None,
-                 category=None, justification=None,
-                 fields=None, field_names=None,
-                 kind=None, title=None,
-                 message=None, message_template=None,
-                 else_message=None, else_message_template=None,
-                 priority=None, valence=None,
-                 location=None, score=None, correct=None,
-                 muted=None, unscored=None,
-                 tool=None, version=None, author=None,
-                 tags=None, parent=None, report=MAIN_REPORT,
-                 delay_condition=False, activate=True,
-                 **kwargs):
-        # Internal data
-        self.report = report
-        # Metadata
-        if label is not None:
-            self.label = label
-        else:
-            self.label = self.__class__.__name__
-        # Condition
-        if category is not None:
-            self.category = category
-        if justification is not None:
-            self.justification = justification
-        self.activate = activate
-        # Response
-        if kind is not None:
-            self.kind = kind
-        if priority is not None:
-            self.priority = priority
-        if valence is not None:
-            self.valence = valence
-
-        # Presentation
-        if fields is not None:
-            self.fields = fields
-        else:
-            self.fields = {}
-        if self.constant_fields is not None:
-            self.fields.update(self.constant_fields)
-        if field_names is not None:
-            self.field_names = field_names
-            # TODO: Should this be taken from `fields` if nothing is provided?
-        if title is not None:
-            self.title = title
-        elif self.title is None:
-            self.title = label
-        if message is not None:
-            self.message = message
-        if message_template is not None:
-            self.message_template = message_template
-        if else_message is not None:
-            self.else_message = else_message
-        if else_message_template is not None:
-            self.else_message_template = else_message_template
-
-        # Locations
-        if isinstance(location, int):
-            location = Location(location)
-        # TODO: Handle tuples (Line, Col) and (Filename, Line, Col), and
-        #  possibly lists thereof
-        if location is not None:
-            self.location = location
-        # Result
-        if score is not None:
-            self.score = score
-        if correct is not None:
-            self.correct = correct
-        if muted is not None:
-            self.muted = muted
-        if unscored is not None:
-            self.unscored = unscored
-        # Metadata
-        if tool is not None:
-            self.tool = tool
-        if version is not None:
-            self.version = version
-        if author is not None:
-            self.author = author
-        if tags is not None:
-            self.tags = tags
-        # Organizational
-        if parent is not None:
-            self.parent = parent
-        if self.parent is None:
-            # Might inherit from Report's current group
-            self.parent = self.report.get_current_group()
-        if self.field_names is not None:
-            for field_name in self.field_names:
-                self.fields[field_name] = kwargs.get(field_name)
-        for key, value in kwargs.items():
-            self.fields[key] = value
-        if 'location' not in self.fields and self.location is not None:
-            self.fields['location'] = self.location
-        # Potentially delay the condition check
-        self._stored_args = args
-        self._stored_kwargs = kwargs
-        if delay_condition:
-            self._met_condition = False
-            self._status = FeedbackStatus.DELAYED
-        else:
-            self._handle_condition()
-
-    def _handle_condition(self):
-        """ Actually handle the condition check, updating message and report. """
-        # Self-attach to a given report?
-        self._exception = None
-        try:
-            self._met_condition = self.condition(*self._stored_args, **self._stored_kwargs)
-            # Generate the message field as needed
-            self.justification = self._get_justification(self._met_condition)
-            if self._met_condition:
-                self.message = self._get_message()
-                self._status = FeedbackStatus.ACTIVE
-            else:
-                self.else_message = self._get_else_message()
-                self.message = self.else_message
-                try:
-                    self.unused_message = self._get_message()
-                except Exception:
-                    self.unused_message = ""
-                self._status = FeedbackStatus.INACTIVE
-        except Exception as e:
-            self._met_condition = False
-            self._exception = e
-            self._status = FeedbackStatus.ERROR
-        if self.report is not None:
-            if self._met_condition:
-                self.report.add_feedback(self)
-            else:
-                self.report.add_ignored_feedback(self)
-        # Free up these temporary fields after condition is handled
-        # del self._stored_args
-        # del self._stored_kwargs
-        if self._exception is not None:
-            raise self._exception
-
-    def condition(self, *args, **kwargs):
-        """
-        Detect if this feedback is present in the code.
-        Defaults to true through the `activate` parameter.
-
-        Returns:
-            bool: Whether this feedback's condition was detected.
-        """
-        return self.activate
-
-    def _get_message(self):
-        """
-        Determines the appropriate value for the message. It will attempt
-        to use this instance's message, but if it's not available then it will
-        try to generate one from the message_template. Then, it returns a
-        generic message.
-
-        You can override this to create a truly dynamic message, if you want.
-
-        Returns:
-            str: The message for this feedback.
-        """
-        if self.message is not None:
-            return self.message
-        if self.message_template is not None:
-            fields = wrap_fields(self.report.format, self.fields)
-            return self.message_template.format(**fields)
-        return self.DEFAULT_FEEDBACK_MESSAGE
-
-    def _get_else_message(self):
-        """
-        Determines the appropriate value for the else_message. It will attempt
-        to use this instance's else_message, but if it's not available then it will
-        try to generate one from the else_message_template. Then, it returns ``None``
-        instead (since usually we don't provide positive feedback).
-
-        You can override this to create a truly dynamic else_message, if you want.
-
-        Returns:
-            str: The else_message for this feedback.
-        """
-        if self.else_message is not None:
-            return self.else_message
-        if self.else_message_template is not None:
-            fields = wrap_fields(self.report.format, self.fields)
-            return self.else_message_template.format(**fields)
-        return self.DEFAULT_ELSE_MESSAGE
-
-    def _get_justification(self, met_condition):
-        """
-        Determines the appropriate value for the justification. It first checks
-        if there is a `justification` already present, but if it's not available
-        then it will attempt to generate one from the `justification_template`. Then,
-        it returns a generic message.
-
-        You can override this to create a truly dynamic justification, if you want.
-
-        Returns:
-            str: The justification for this feedback.
-        """
-        if self.justification is not None:
-            if isinstance(self.justification, str):
-                if met_condition:
-                    return self.justification
-                else:
-                    return "The following condition was not met: " + self.justification
-            else:
-                met, unmet = self.justification
-                return met if met_condition else unmet
-        if self.justification_template is not None:
-            if isinstance(self.justification_template, str):
-                template = "The following condition was not met: " + self.justification_template
-            else:
-                met, unmet = self.justification_template
-                template = met if met_condition else unmet
-            fields = wrap_fields(self.report.format, self.fields)
-            return template.format(**fields)
-        return self.DEFAULT_JUSTIFICATION_MESSAGE
-
-    def _get_child_feedback(self, feedback, active):
-        """ Callback function that Reports will call when a new piece of
-        feedback is being considered. By default, does nothing. This is useful
-        for :py:class:`pedal.core.group.FeedbackGroup`, most other feedbacks
-        will just not care.
-
-        The ``active`` parameter controls whether the condition for the
-        feedback was met. """
-
-    def __xor__(self, other):
-        """
-        Allows you to have two mutually exclusive conditions. Only one condition will be activated.
-
-        Args:
-            other:
-
-        Returns:
-
-        """
-        if isinstance(other, Feedback):
-            self.muted = bool(self) and not bool(other)
-            self.unscored = self.muted
-            other.muted = bool(other) and not bool(self)
-            other.unscored = other.muted
-        if isinstance(other, bool):
-            self.muted = bool(self) and not bool(other)
-            self.unscored = self.muted
-
-    def __rxor__(self, other):
-        return self.__xor__(other)
-
-    def __bool__(self):
-        return bool(self._met_condition)
-
-    def __str__(self):
-        """
-        Create a string representation of this piece of Feedback for quick, dev purposes.
-        Returns:
-            str: String representation
-        """
-        return "<Feedback ({},{})>".format(self.category, self.label)
-
-    def __repr__(self):
-        """
-        Create a string representation of this piece of Feedback that displays considerably more information.
-        Returns:
-            str: String representation with more data
-        """
-        metadata = ""
-        if self.tool is not None:
-            metadata += ", tool=" + self.tool
-        if self.category is not None:
-            metadata += ", category=" + self.category
-        if self.priority is not None:
-            metadata += ", priority=" + self.priority
-        if self.parent is not None:
-            metadata += ", parent=" + str(self.parent.label)
-        if self.fields is not None:
-            metadata += ", " + ", ".join(f"{field}={value!r}" for field, value in self.fields.items())
-        return "Feedback({}{})".format(self.label, metadata)
-
-    def update_location(self, location):
-        """ Updates both the fields and location attribute.
-        TODO: Handle less information intelligently. """
-        if isinstance(location, int):
-            location = Location(location)
-        self.location = location
-        self.fields['location'] = location
-
-    def _fields_to_json(self):
-        return self.fields.copy()
-
-    def to_json(self):
-        return {
-            'correct': self.correct,
-            'score': self.score,
-            'title': self.title,
-            'message': self.message,
-            'label': self.label,
-            'active': bool(self),
-            'muted': self.muted,
-            'unscored': self.unscored,
-            'category': self.category,
-            'kind': self.kind,
-            'valence': self.valence,
-            'version': self.version,
-            'fields': self._fields_to_json(),
-            'justification': self.justification,
-            'priority': self.priority,
-            'location': self.location.to_json() if self.location is not None else None
-        }
-
-    @classmethod
-    def override(cls, report=MAIN_REPORT, **fields):
-        if cls._override_backups is None:
-            cls._override_backups = {}
-        for field, new_value in fields.items():
-            if field not in cls._override_backups:
-                cls._override_backups[field] = getattr(cls, field)
-            setattr(cls, field, new_value)
-        report.override_feedback(cls)
-
-    @classmethod
-    def _restore_overrides(cls):
-        for field, old_value in cls._override_backups.items():
-            setattr(cls, field, old_value)
-        cls._override_backups.clear()
-
-
-    @classmethod
-    def override_for_pool(cls, pool, **fields):
-        if isinstance(pool, str):
-            pool = [pool]
-        for each_pool in pool:
-            if each_pool not in cls._pools:
-                cls._pools[each_pool] = {}
-            cls._pools[each_pool].update(fields)
-
-    def _finalize(self):
-        # TODO: Move this to be earlier, when we create a feedback.
-        #       Otherwise there might be fields that are not interpolated correctly!
-        possible_overrides = self._pools.get(self.report.chosen_pool)
-        if possible_overrides:
-            for key, value in possible_overrides.items():
-                setattr(self, key, value)
-
-
-class FeedbackResponse(Feedback):
-    """
-    An extension of :py:class:`~pedal.core.feedback.Feedback` that is meant
-    to indicate that the class should not have any condition behind its
-    response.
-    """
-
-
-def CompositeFeedbackFunction(*functions):
-    """
-    Decorator for functions that return multiple types of feedback functions.
-
-    Args:
-        functions (callable): A list of callable functions.
-
-    Returns:
-        callable: The decorated function.
-    """
-
-    def CompositeFeedbackFunction_with_attrs(function):
-        """
-
-        Args:
-            function:
-
-        Returns:
-
-        """
-        CompositeFeedbackFunction_with_attrs.functions = functions
-        return function
-
-    return CompositeFeedbackFunction_with_attrs
-
-
-class FeedbackGroup(Feedback):
-    """
-    An extension of :py:class:`~pedal.core.feedback.Feedback` that is meant
-    to indicate that this class will start a new Group context within the report
-    and do something interesting with any children it gets.
-    """
-
-
-DEFAULT_CATEGORY_PRIORITY = [
-    "highest",
-    # Static
-    Feedback.CATEGORIES.SYNTAX,
-    Feedback.CATEGORIES.MISTAKES,
-    Feedback.CATEGORIES.INSTRUCTOR,
-    Feedback.CATEGORIES.ALGORITHMIC,
-    # Dynamic
-    Feedback.CATEGORIES.RUNTIME,
-    Feedback.CATEGORIES.STUDENT,
-    Feedback.CATEGORIES.SPECIFICATION,
-    Feedback.CATEGORIES.POSITIVE,
-    Feedback.CATEGORIES.INSTRUCTIONS,
-    Feedback.CATEGORIES.UNKNOWN,
-    "lowest"
-]
+"""
+Simple data classes for storing feedback to present to learners.
+"""
+
+__all__ = ['Feedback', 'FeedbackKind', 'FeedbackCategory',
+           "CompositeFeedbackFunction",
+           "FeedbackResponse"]
+
+from pedal.core.formatting import wrap_fields
+from pedal.core.location import Location
+from pedal.core.report import MAIN_REPORT
+from pedal.core.feedback_category import FeedbackKind, FeedbackCategory, FeedbackStatus
+
+PEDAL_DEVELOPERS = ["Austin Cory Bart <acbart@udel.edu>",
+                    "Luke Gusukuma <lukesg08@vt.edu>"]
+
+
+class FeedbackRegistry:
+    def __init__(self):
+        self._registered_feedback = {}
+
+
+class Feedback:
+    """
+    A class for storing raw feedback.
+
+    Attributes:
+        label (str): An internal name for this specific piece of feedback. The
+            label should be an underscore-separated string following the same
+            conventions as names in Python. They do not have to be globally
+            unique, but labels should be as unique as possible (especially
+            within a category).
+        tool (str, optional): An internal name for indicating the tool that created
+            this feedback. Should be taken directly from the Tool itself. If `None`, then
+            this was not created by a tool but directly by the control script.
+        category (str): A human-presentable name showable to the learner, indicating what
+            sort of feedback this falls into (e.g., "runtime", "syntax", "algorithm").
+            More than one feedback will be in a category, but a feedback cannot be in
+            more than one category.
+        kind (str): The pedagogical role of this feedback, e.g., "misconception", "mistake",
+            "hint", "constraint". Usually, a piece of Feedback is pointing out a mistake,
+            but feedback can also be used for various other purposes.
+        justification (str): An instructor-facing string briefly describing why this
+            feedback was selected. Serves as a "TL;DR" for this feedback category, useful
+            for debugging why a piece of feedback appeared.
+        justification_template (str): A markdown-formatted message template that will
+            be used if a ``justification`` is None. Any ``fields`` will be injected
+            into the template IF the ``condition`` is met.
+        priority (str): An indication of how important this feedback is relative to other types
+            of feedback in the same category. Might be "high/medium/low". Exactly how this
+            gets used is up to the resolver, but typically it helps break ties.
+        valence (int): Indicates whether this is negative, positive, or neutral feedback.
+            Either 1, -1, or 0.
+
+        title (str, optional): A formal, student-facing title for this feedback. If None, indicates
+            that the :py:attr:`~pedal.core.feedback.Feedback.label` should be used instead.
+        message (str): A markdown-formatted message (aka also supporting HTML) that could be rendered
+            to the user.
+        message_template (str): A markdown-formatted message template that will
+            be used if a ``message`` is None. Any ``fields`` will be injected
+            into the template IF the ``condition`` is met.
+        fields (Dict[str,Any]): The raw data that was used to interpolate the
+            template to produce the message.
+        location (:py:attr:`~pedal.core.location.Location` or int): Information
+            about specific locations relevant to this message.
+
+        score (int): A numeric score to modify the students' total score, indicating their overall performance.
+            It is ultimately up to the Resolver to decide how to combine all the different scores; a typical
+            strategy would be to add all the scores together for any non-muted feedback.
+        correct (bool): Indicates that the entire submission should be considered correct (success) and that the
+            task is now finished.
+        muted (bool): Whether this piece of feedback is something that should be shown to a student. There are
+            various use cases for muted feedback: they can serve as flags for later conditionals, suppressed
+            default kinds of feedback, or perhaps feedback that is interesting for analysis but not pedagogically
+            helpful to give to the student. They will still contribute to overall score, but not to the correctness
+            of the submission.
+        unscored (bool): Whether this piece of feedback contributes to the score/correctness.
+
+        else_message (str): A string to render as a message when a
+            NEGATIVE valence feedback is NOT triggered, or a POSITIVE valence
+            feedback IS triggered.
+        else_message_template (str): Similar to the ``message_template``, but for the ``else_message``.
+
+        activate (bool): Used for default feedback objects without a custom
+            condition, to indicate whether they should be considered triggered.
+            Defaults to True; setting this to False means that the feedback
+            object will be deactivated. Note that most inheriting Feedback
+            Functions will not respect this parameter.
+
+        author (List[str]): A list of names/emails that indicate who created this piece of feedback. They can be
+            either names, emails, or combinations in the style of `"Cory Bart <acbart@udel.edu>"`.
+        version (str): A version string in the style of Semantic Version (semvar) such as `"0.0.1"`. The last (third)
+            digit should be incremented for small bug fixes/changes. The middle (second) digit should be used for more
+            serious and intense changes. The first digit should be incremented when changes are made on exposure to
+            learners or some other evidence-based motivation.
+        tags (list[:py:class:`~pedal.core.tag.Tag`]): Any tags that you want to
+            attach to this feedback.
+
+        parent (int, str, or `pedal.core.feedback.Feedback`): Information about
+            what logical grouping within the submission this belongs to.
+            Various tools can chunk up a submission (e.g., by section), they
+            can use this field to keep track of how that decision was made.
+            Resolvers can also use this information to organize feedback or to
+            report multiple categories.
+        report (:py:class:`~pedal.core.report.Report`): The Report object to
+            attach this feedback to. Defaults to MAIN_REPORT. Unspecified fields
+            will be filled in by inspecting the current Feedback Function
+            context.
+    """
+
+    POSITIVE_VALENCE = 1
+    NEUTRAL_VALENCE = 0
+    NEGATIVE_VALENCE = -1
+    CATEGORIES = FeedbackCategory
+    KINDS = FeedbackKind
+
+    DEFAULT_FEEDBACK_MESSAGE = "No feedback message provided"
+    DEFAULT_JUSTIFICATION_MESSAGE = "No justification provided"
+    DEFAULT_ELSE_MESSAGE = None
+
+    label = None
+    category = None
+    justification = None
+    justification_template = None
+    constant_fields = None
+    fields = None
+    field_names = None
+    kind = None
+    title = None
+    message = None
+    message_template = None
+    else_message = None
+    else_message_template = None
+    priority = None
+    valence = None
+    location = None
+    score = None
+    correct = None
+    muted = None
+    unscored = None
+    tool = None
+    version = '1.0.0'
+    author = PEDAL_DEVELOPERS
+    tags = None
+    parent = None
+
+    activate: bool
+    _status: str
+    _exception: Exception or None
+    _met_condition: bool
+    _stored_args: tuple
+    _stored_kwargs: dict
+    _override_backups = None
+    _pools = {}
+
+    resolved_score = None
+    unused_message = None
+
+    # MAIN_REPORT
+
+    def __init__(self, *args, label=None,
+                 category=None, justification=None,
+                 fields=None, field_names=None,
+                 kind=None, title=None,
+                 message=None, message_template=None,
+                 else_message=None, else_message_template=None,
+                 priority=None, valence=None,
+                 location=None, score=None, correct=None,
+                 muted=None, unscored=None,
+                 tool=None, version=None, author=None,
+                 tags=None, parent=None, report=MAIN_REPORT,
+                 delay_condition=False, activate=True,
+                 **kwargs):
+        # Internal data
+        self.report = report
+        # Metadata
+        if label is not None:
+            self.label = label
+        else:
+            self.label = self.__class__.__name__
+        # Condition
+        if category is not None:
+            self.category = category
+        if justification is not None:
+            self.justification = justification
+        self.activate = activate
+        # Response
+        if kind is not None:
+            self.kind = kind
+        if priority is not None:
+            self.priority = priority
+        if valence is not None:
+            self.valence = valence
+
+        # Presentation
+        if fields is not None:
+            self.fields = fields
+        else:
+            self.fields = {}
+        if self.constant_fields is not None:
+            self.fields.update(self.constant_fields)
+        if field_names is not None:
+            self.field_names = field_names
+            # TODO: Should this be taken from `fields` if nothing is provided?
+        if title is not None:
+            self.title = title
+        elif self.title is None:
+            self.title = label
+        if message is not None:
+            self.message = message
+        if message_template is not None:
+            self.message_template = message_template
+        if else_message is not None:
+            self.else_message = else_message
+        if else_message_template is not None:
+            self.else_message_template = else_message_template
+
+        # Locations
+        if isinstance(location, int):
+            location = Location(location)
+        # TODO: Handle tuples (Line, Col) and (Filename, Line, Col), and
+        #  possibly lists thereof
+        if location is not None:
+            self.location = location
+        # Result
+        if score is not None:
+            self.score = score
+        if correct is not None:
+            self.correct = correct
+        if muted is not None:
+            self.muted = muted
+        if unscored is not None:
+            self.unscored = unscored
+        # Metadata
+        if tool is not None:
+            self.tool = tool
+        if version is not None:
+            self.version = version
+        if author is not None:
+            self.author = author
+        if tags is not None:
+            self.tags = tags
+        # Organizational
+        if parent is not None:
+            self.parent = parent
+        if self.parent is None:
+            # Might inherit from Report's current group
+            self.parent = self.report.get_current_group()
+        if self.field_names is not None:
+            for field_name in self.field_names:
+                self.fields[field_name] = kwargs.get(field_name)
+        for key, value in kwargs.items():
+            self.fields[key] = value
+        if 'location' not in self.fields and self.location is not None:
+            self.fields['location'] = self.location
+        # Potentially delay the condition check
+        self._stored_args = args
+        self._stored_kwargs = kwargs
+        if delay_condition:
+            self._met_condition = False
+            self._status = FeedbackStatus.DELAYED
+        else:
+            self._handle_condition()
+
+    def _handle_condition(self):
+        """ Actually handle the condition check, updating message and report. """
+        # Self-attach to a given report?
+        self._exception = None
+        try:
+            self._met_condition = self.condition(*self._stored_args, **self._stored_kwargs)
+            # Generate the message field as needed
+            self.justification = self._get_justification(self._met_condition)
+            if self._met_condition:
+                self.message = self._get_message()
+                self._status = FeedbackStatus.ACTIVE
+            else:
+                self.else_message = self._get_else_message()
+                self.message = self.else_message
+                try:
+                    self.unused_message = self._get_message()
+                except Exception:
+                    self.unused_message = ""
+                self._status = FeedbackStatus.INACTIVE
+        except Exception as e:
+            self._met_condition = False
+            self._exception = e
+            self._status = FeedbackStatus.ERROR
+        if self.report is not None:
+            if self._met_condition:
+                self.report.add_feedback(self)
+            else:
+                self.report.add_ignored_feedback(self)
+        # Free up these temporary fields after condition is handled
+        # del self._stored_args
+        # del self._stored_kwargs
+        if self._exception is not None:
+            raise self._exception
+
+    def condition(self, *args, **kwargs):
+        """
+        Detect if this feedback is present in the code.
+        Defaults to true through the `activate` parameter.
+
+        Returns:
+            bool: Whether this feedback's condition was detected.
+        """
+        return self.activate
+
+    def _get_message(self):
+        """
+        Determines the appropriate value for the message. It will attempt
+        to use this instance's message, but if it's not available then it will
+        try to generate one from the message_template. Then, it returns a
+        generic message.
+
+        You can override this to create a truly dynamic message, if you want.
+
+        Returns:
+            str: The message for this feedback.
+        """
+        if self.message is not None:
+            return self.message
+        if self.message_template is not None:
+            fields = wrap_fields(self.report.format, self.fields)
+            return self.message_template.format(**fields)
+        return self.DEFAULT_FEEDBACK_MESSAGE
+
+    def _get_else_message(self):
+        """
+        Determines the appropriate value for the else_message. It will attempt
+        to use this instance's else_message, but if it's not available then it will
+        try to generate one from the else_message_template. Then, it returns ``None``
+        instead (since usually we don't provide positive feedback).
+
+        You can override this to create a truly dynamic else_message, if you want.
+
+        Returns:
+            str: The else_message for this feedback.
+        """
+        if self.else_message is not None:
+            return self.else_message
+        if self.else_message_template is not None:
+            fields = wrap_fields(self.report.format, self.fields)
+            return self.else_message_template.format(**fields)
+        return self.DEFAULT_ELSE_MESSAGE
+
+    def _get_justification(self, met_condition):
+        """
+        Determines the appropriate value for the justification. It first checks
+        if there is a `justification` already present, but if it's not available
+        then it will attempt to generate one from the `justification_template`. Then,
+        it returns a generic message.
+
+        You can override this to create a truly dynamic justification, if you want.
+
+        Returns:
+            str: The justification for this feedback.
+        """
+        if self.justification is not None:
+            if isinstance(self.justification, str):
+                if met_condition:
+                    return self.justification
+                else:
+                    return "The following condition was not met: " + self.justification
+            else:
+                met, unmet = self.justification
+                return met if met_condition else unmet
+        if self.justification_template is not None:
+            if isinstance(self.justification_template, str):
+                template = "The following condition was not met: " + self.justification_template
+            else:
+                met, unmet = self.justification_template
+                template = met if met_condition else unmet
+            fields = wrap_fields(self.report.format, self.fields)
+            return template.format(**fields)
+        return self.DEFAULT_JUSTIFICATION_MESSAGE
+
+    def _get_child_feedback(self, feedback, active):
+        """ Callback function that Reports will call when a new piece of
+        feedback is being considered. By default, does nothing. This is useful
+        for :py:class:`pedal.core.group.FeedbackGroup`, most other feedbacks
+        will just not care.
+
+        The ``active`` parameter controls whether the condition for the
+        feedback was met. """
+
+    def __xor__(self, other):
+        """
+        Allows you to have two mutually exclusive conditions. Only one condition will be activated.
+
+        Args:
+            other:
+
+        Returns:
+
+        """
+        if isinstance(other, Feedback):
+            self.muted = bool(self) and not bool(other)
+            self.unscored = self.muted
+            other.muted = bool(other) and not bool(self)
+            other.unscored = other.muted
+        if isinstance(other, bool):
+            self.muted = bool(self) and not bool(other)
+            self.unscored = self.muted
+
+    def __rxor__(self, other):
+        return self.__xor__(other)
+
+    def __bool__(self):
+        return bool(self._met_condition)
+
+    def __str__(self):
+        """
+        Create a string representation of this piece of Feedback for quick, dev purposes.
+        Returns:
+            str: String representation
+        """
+        return "<Feedback ({},{})>".format(self.category, self.label)
+
+    def __repr__(self):
+        """
+        Create a string representation of this piece of Feedback that displays considerably more information.
+        Returns:
+            str: String representation with more data
+        """
+        metadata = ""
+        if self.tool is not None:
+            metadata += ", tool=" + self.tool
+        if self.category is not None:
+            metadata += ", category=" + self.category
+        if self.priority is not None:
+            metadata += ", priority=" + self.priority
+        if self.parent is not None:
+            metadata += ", parent=" + str(self.parent.label)
+        if self.fields is not None:
+            metadata += ", " + ", ".join(f"{field}={value!r}" for field, value in self.fields.items())
+        return "Feedback({}{})".format(self.label, metadata)
+
+    def update_location(self, location):
+        """ Updates both the fields and location attribute.
+        TODO: Handle less information intelligently. """
+        if isinstance(location, int):
+            location = Location(location)
+        self.location = location
+        self.fields['location'] = location
+
+    def _fields_to_json(self):
+        return self.fields.copy()
+
+    def to_json(self):
+        return {
+            'correct': self.correct,
+            'score': self.score,
+            'title': self.title,
+            'message': self.message,
+            'label': self.label,
+            'active': bool(self),
+            'muted': self.muted,
+            'unscored': self.unscored,
+            'category': self.category,
+            'kind': self.kind,
+            'valence': self.valence,
+            'version': self.version,
+            'fields': self._fields_to_json(),
+            'justification': self.justification,
+            'priority': self.priority,
+            'location': self.location.to_json() if self.location is not None else None
+        }
+
+    @classmethod
+    def override(cls, report=MAIN_REPORT, **fields):
+        if cls._override_backups is None:
+            cls._override_backups = {}
+        for field, new_value in fields.items():
+            if field not in cls._override_backups:
+                cls._override_backups[field] = getattr(cls, field)
+            setattr(cls, field, new_value)
+        report.override_feedback(cls)
+
+    @classmethod
+    def _restore_overrides(cls):
+        for field, old_value in cls._override_backups.items():
+            setattr(cls, field, old_value)
+        cls._override_backups.clear()
+
+
+    @classmethod
+    def override_for_pool(cls, pool, **fields):
+        if isinstance(pool, str):
+            pool = [pool]
+        for each_pool in pool:
+            if each_pool not in cls._pools:
+                cls._pools[each_pool] = {}
+            cls._pools[each_pool].update(fields)
+
+    def _finalize(self):
+        # TODO: Move this to be earlier, when we create a feedback.
+        #       Otherwise there might be fields that are not interpolated correctly!
+        possible_overrides = self._pools.get(self.report.chosen_pool)
+        if possible_overrides:
+            for key, value in possible_overrides.items():
+                setattr(self, key, value)
+
+
+class FeedbackResponse(Feedback):
+    """
+    An extension of :py:class:`~pedal.core.feedback.Feedback` that is meant
+    to indicate that the class should not have any condition behind its
+    response.
+    """
+
+
+def CompositeFeedbackFunction(*functions):
+    """
+    Decorator for functions that return multiple types of feedback functions.
+
+    Args:
+        functions (callable): A list of callable functions.
+
+    Returns:
+        callable: The decorated function.
+    """
+
+    def CompositeFeedbackFunction_with_attrs(function):
+        """
+
+        Args:
+            function:
+
+        Returns:
+
+        """
+        CompositeFeedbackFunction_with_attrs.functions = functions
+        return function
+
+    return CompositeFeedbackFunction_with_attrs
+
+
+class FeedbackGroup(Feedback):
+    """
+    An extension of :py:class:`~pedal.core.feedback.Feedback` that is meant
+    to indicate that this class will start a new Group context within the report
+    and do something interesting with any children it gets.
+    """
+
+
+DEFAULT_CATEGORY_PRIORITY = [
+    "highest",
+    # Static
+    Feedback.CATEGORIES.SYNTAX,
+    Feedback.CATEGORIES.MISTAKES,
+    Feedback.CATEGORIES.INSTRUCTOR,
+    Feedback.CATEGORIES.ALGORITHMIC,
+    # Dynamic
+    Feedback.CATEGORIES.RUNTIME,
+    Feedback.CATEGORIES.STUDENT,
+    Feedback.CATEGORIES.SPECIFICATION,
+    Feedback.CATEGORIES.POSITIVE,
+    Feedback.CATEGORIES.INSTRUCTIONS,
+    Feedback.CATEGORIES.UNKNOWN,
+    "lowest"
+]
```

### Comparing `pedal-2.6.1/pedal/core/feedback_category.py` & `pedal-2.6.2/pedal/core/feedback_category.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/core/final_feedback.py` & `pedal-2.6.2/pedal/core/final_feedback.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/core/formatting.py` & `pedal-2.6.2/pedal/core/formatting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/core/location.py` & `pedal-2.6.2/pedal/core/location.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/core/report.py` & `pedal-2.6.2/pedal/core/report.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,368 +1,368 @@
-"""
-File that holds the the Report class and the global MAIN_REPORT.
-
-Note that you can make other Reports, but that doesn't actually seem to be
-useful very often. Usually you want to just rely on the global MAIN_REPORT.
-"""
-
-__all__ = ['Report', 'MAIN_REPORT']
-import logging
-import random
-
-from pedal.core.errors import PedalToolNotRegistered, PedalToolAlreadyRegistered
-from pedal.core.feedback_category import FeedbackCategory
-
-
-# TODO: Mechanism for checking whether a piece of feedback is in the report
-from pedal.core.formatting import Formatter
-from pedal.core.tool import ToolRegistration
-
-log = logging.getLogger(__name__)
-
-
-class Report:
-    """
-    A class for storing Feedback generated by Tools, along with any auxiliary
-    data that the Tool might want to provide for other tools.
-
-    Attributes:
-        submission (:py:class:`~pedal.core.submission.Submission`): The
-            contextualized submission information.
-        feedback (list[:py:class:`~pedal.core.feedback.Feedback`]): The raw
-            feedback generated for this Report so far.
-        suppressions (list[tuple[str, str]]): The categories and labels that
-            have been suppressed so far.
-        hiddens (set[str]): The parts of the final response that should be
-            hidden. This can globally hide the 'correct', 'score', etc.
-        group (int or str): The label for the current group. Feedback given
-            by a Tool will automatically receive the current `group`. This
-            is used by the Source tool, for example, in order to group feedback
-            by sections and the :py:func:`pedal.assertions.commands.unit_test`
-            function to combine results.
-        group_names (dict[group, str]): A printable, student-facing name for the
-            group. When a group needs to be rendered out to the user, this
-            will override whatever label was going to be presented instead.
-        hooks (dict[str, list[callable]): A dictionary mapping events to
-            a list of callable functions. Tools can register functions on
-            hooks to have them executed when the event is triggered by another
-            tool. For example, the Assertions tool has hooks on the Source tool
-            to trigger assertion resolutions before advancing to next sections.
-        _tool_data (dict[str, Any]): Maps tool names to their data. The
-                                       namespace for a tool can be used to
-                                       store whatever they want, but will
-                                       probably be in a dictionary itself.
-        resolves (list[Any]): The result of having previously called a
-            resolver. This allows you to check if a report has previously
-            been resolved, or do something with that data.
-        result (FinalFeedback): The FinalFeedback (distinct from a Feedback) that was
-            generated as a result of resolving this Report, or None if the Report is
-            not yet resolved.
-    """
-    #: dict[str, dict]: The
-    #: tools registered for this report, available via their names.
-    TOOLS = {}
-
-    def __init__(self):
-        """
-        Creates a new Report instance.
-        """
-        self._tool_data = {}
-        self.feedback = []
-        self.ignored_feedback = []
-        self.suppressions = {}
-        self.suppressed_labels = {}
-        self.hiddens = set()
-        self.groups = []
-        self.group = None
-        self.group_names = {}
-        self.hooks = {}
-        self.class_hooks = {}
-        self.submission = None
-        self.format = Formatter()
-        self.result = None
-        self.resolves = []
-        self.pools = []
-        self.chosen_pool = None
-        self.overridden_feedbacks = set()
-        log.debug("New Pedal Report created.")
-
-    def clear(self):
-        """
-        Resets the entire report back to its starting form,
-        including deleting any attached submissions, tool data, and feedbacks.
-        It will also reset any overridden fields of feedback classes.
-        However, it will not affect class hooks.
-        """
-        self.feedback.clear()
-        self.ignored_feedback.clear()
-        self.suppressions.clear()
-        self.suppressed_labels.clear()
-        self.hiddens.clear()
-        self._tool_data.clear()
-        self.group = None
-        self.groups.clear()
-        self.group_names.clear()
-        self.hooks.clear()
-        self.submission = None
-        self.result = None
-        self.resolves.clear()
-        self.format = Formatter()
-        self.clear_overridden_feedback()
-
-    def full_clear(self):
-        """ This totally resets the report, including any class hooks. """
-        self.clear()
-        self.class_hooks.clear()
-
-    def clear_overridden_feedback(self):
-        for feedback in self.overridden_feedbacks:
-            feedback._restore_overrides()
-        self.overridden_feedbacks.clear()
-
-    def override_feedback(self, feedback_class):
-        self.overridden_feedbacks.add(feedback_class)
-
-    def set_pools(self, pools):
-        if isinstance(pools, int):
-            pools = list('ABCDEFGHIJKLMNOPQRSTUVWXYZ'[:pools])
-        self.pools = pools
-
-    def contextualize(self, submission):
-        """
-        Attach the given submission to this report.
-
-        Args:
-            submission (:py:class:`pedal.core.submission.Submission`): The
-                submission to attach to this report.
-        """
-        self.submission = submission
-
-    def hide_correctness(self):
-        """
-        Suppress the RESULT category entirely, so that the report doesn't
-        indicate whether or not the submission was correct.
-        TODO: Make this just a regular command.
-        """
-        self.hiddens.add('correct')
-        self.hiddens.add('score')
-
-    def add_feedback(self, feedback):
-        """
-        Attaches the given feedback object to this report.
-
-        Args:
-            feedback (:py:class:`~pedal.core.feedback.Feedback`): The feedback
-                object to attach.
-
-        Returns:
-            :py:class:`~pedal.core.feedback.Feedback`: The attached feedback.
-        """
-        self.feedback.append(feedback)
-        if not isinstance(feedback.parent, (int, str)) and feedback.parent is not None:
-            feedback.parent._get_child_feedback(feedback, True)
-        self.execute_hooks('pedal.report', 'add_feedback', (feedback,))
-        return feedback
-
-    def add_ignored_feedback(self, feedback):
-        """
-        Attaches the given feedback object to this report, but only in the
-        ignored list. That means it should not be considered by the Resolver,
-        since its condition did not apply to the code. Some Resolvers like
-        to know about feedback that was not reached.
-
-        Args:
-            feedback (:py:class:`~pedal.core.feedback.Feedback`): The feedback
-                object to attach.
-
-        Returns:
-            :py:class:`~pedal.core.feedback.Feedback`: The attached feedback.
-        """
-        self.ignored_feedback.append(feedback)
-        if feedback.parent is not None:
-            feedback.parent._get_child_feedback(feedback, False)
-        return feedback
-
-    def suppress(self, category=None, label=True, fields=None):
-        """
-        Suggest that an entire category or label within a category ignored by
-        the resolver.
-        TODO: Currently, only global suppression is supported.
-
-        Args:
-            category (str): The category of feedback to suppress.
-            label (bool or str): A specific label to match against and suppress.
-            fields (dict of key/values): The fields that will be matched exactly to
-                suppress.
-        """
-        if fields is None:
-            fields = {}
-        if category is None:
-            if label not in self.suppressed_labels:
-                self.suppressed_labels[label] = []
-            self.suppressed_labels[label].append(fields)
-        else:
-            category = category.lower()
-            if isinstance(label, str):
-                label = label.lower()
-            if category in FeedbackCategory.ALIASES:
-                category = FeedbackCategory.ALIASES[category]
-            if category not in self.suppressions:
-                self.suppressions[category] = {}
-            if label not in self.suppressions[category]:
-                self.suppressions[category][label] = []
-            self.suppressions[category][label].append(fields)
-
-    def add_hook(self, event, function):
-        """
-        Register the `function` to be executed when the given `event` is
-        triggered.
-        
-        Args:
-            event (str): An event name. Multiple functions can be triggered for
-                the same `event`. The format is as follows: `"namespace.function.extra"`
-                The `".extra"` component is optional to add further nuance, but
-                the general idea is that you are referring to functions that,
-                when called, should trigger other functions to be called first.
-                The namespace is typically a tool or module.
-            function (callable): A callable function. This function should
-                accept a keyword parameter named `report`; this report will be passed
-                as as that argument.
-        """
-        if event not in self.hooks:
-            self.hooks[event] = []
-        self.hooks[event].append(function)
-
-    @classmethod
-    def add_class_hook(cls, event, function):
-        """ Similar to ``add_hook``, except attaches them to the class, so
-        they will be executed for ALL report subclasses. """
-        if event not in cls.class_hooks:
-            cls.class_hooks[event] = []
-        cls.class_hooks[event].append(function)
-
-    def execute_hooks(self, tool, event_name, arguments=None, keyword_arguments=None):
-        """
-        Trigger the functions for all of the associated hooks.
-        Hooks will be called with this report as a keyword `report` argument.
-
-        Args:
-            tool (str): The name of the tool, to namespace events by.
-            event_name (str): The event name (separate words with periods).
-            arguments (tuple[any]): The arguments to be passed to the callback function.
-            keyword_arguments (dict[str, any]): The keyword arguments to be passed to the callback funciton.
-        """
-        if arguments is None:
-            arguments = tuple()
-        if keyword_arguments is None:
-            keyword_arguments = {}
-        event = tool + '.' + event_name
-        if event in self.class_hooks:
-            for function in self.class_hooks[event]:
-                function(report=self, *arguments, **keyword_arguments)
-        if event in self.hooks:
-            for function in self.hooks[event]:
-                function(report=self, *arguments, **keyword_arguments)
-
-    def __getitem__(self, tool_name):
-        """
-        Support retrieving a tool's data from the report using square bracket
-        syntax. So, for example, you can do `MAIN_REPORT['tifa']` and get its
-        data dictionary. If the tool has been registered, but not initialized
-        for this report, then the tool will be
-        :py:method:`pedal.core.tool.reset` first. Otherwise, throws an error
-        that the tool does not exist.
-
-        Args:
-            tool_name (str): The formal name of the tool, most likely specified
-                in its `constants.py` file.
-
-        Returns:
-            dict: The data associated with that tool.
-        """
-        if tool_name not in self._tool_data:
-            if tool_name not in self.TOOLS:
-                raise PedalToolNotRegistered(tool_name, list(self.TOOLS.keys()))
-            self.TOOLS[tool_name].reset(report=self)
-        return self._tool_data[tool_name]
-
-    def __setitem__(self, tool_name, value):
-        """
-        Update the tool's current data. Should largely not be used by anyone.
-        In fact, this could seriously damage the relationships between tools.
-
-        Args:
-            tool_name (str): The name of the tool.
-            value (dict): The new data to set as this tool's namespace.
-        """
-        self._tool_data[tool_name] = value
-
-    def __contains__(self, tool_name):
-        """
-        Determine if the given `tool_name` is available through this report.
-        Args:
-            tool_name (str): The name of a tool.
-
-        Returns:
-            bool: Whether the tool is available.
-        """
-        return tool_name in self._tool_data
-
-    def set_formatter(self, formatter):
-        """
-        Update the formatter with the new option.
-
-        Args:
-            formatter (:py:class:`pedal.core.formatting.Formatter`): The new
-                formatter to use.
-        """
-        self.format = formatter
-
-    @classmethod
-    def register_tool(cls, tool_name: str, reset_function):
-        """
-        Identifies that the given Tool should be made available.
-        Args:
-            tool_name: A unique string identifying this tool.
-            reset_function: The function to call to reset the Tool.
-
-        Returns:
-
-        """
-        if tool_name in cls.TOOLS:
-            raise PedalToolAlreadyRegistered(tool_name)
-        cls.TOOLS[tool_name] = ToolRegistration(tool_name, reset_function)
-
-    def get_current_group(self):
-        if self.groups:
-            return self.groups[-1]
-        else:
-            return None
-
-    def start_group(self, group):
-        self.groups.append(group)
-
-    def stop_group(self, group):
-        """
-        TODO: Should this prematurely end other groups? If so, do they get a
-            callback event to do any wrapup?
-        """
-        if self.groups:
-            self.groups.remove(group)
-
-    def finalize_pools(self):
-        if self.pools:
-            self.chosen_pool = random.choice(self.pools)
-
-    def finalize_feedbacks(self):
-        self.finalize_pools()
-        for feedback in self.feedback + self.ignored_feedback:
-            feedback._finalize()
-
-#: The global Report object. Meant to be used as a default singleton
-#: for any tool, so that instructors do not have to create their own Report.
-#: Of course, all APIs are expected to work with a given Report, and only
-#: default to this Report when no others are given.
-#: Ideally, the average instructor will never know this exists.
-MAIN_REPORT = Report()
-
-# TODO: Give a mechanism for "freezing" a report that you can keep around.
+"""
+File that holds the the Report class and the global MAIN_REPORT.
+
+Note that you can make other Reports, but that doesn't actually seem to be
+useful very often. Usually you want to just rely on the global MAIN_REPORT.
+"""
+
+__all__ = ['Report', 'MAIN_REPORT']
+import logging
+import random
+
+from pedal.core.errors import PedalToolNotRegistered, PedalToolAlreadyRegistered
+from pedal.core.feedback_category import FeedbackCategory
+
+
+# TODO: Mechanism for checking whether a piece of feedback is in the report
+from pedal.core.formatting import Formatter
+from pedal.core.tool import ToolRegistration
+
+log = logging.getLogger(__name__)
+
+
+class Report:
+    """
+    A class for storing Feedback generated by Tools, along with any auxiliary
+    data that the Tool might want to provide for other tools.
+
+    Attributes:
+        submission (:py:class:`~pedal.core.submission.Submission`): The
+            contextualized submission information.
+        feedback (list[:py:class:`~pedal.core.feedback.Feedback`]): The raw
+            feedback generated for this Report so far.
+        suppressions (list[tuple[str, str]]): The categories and labels that
+            have been suppressed so far.
+        hiddens (set[str]): The parts of the final response that should be
+            hidden. This can globally hide the 'correct', 'score', etc.
+        group (int or str): The label for the current group. Feedback given
+            by a Tool will automatically receive the current `group`. This
+            is used by the Source tool, for example, in order to group feedback
+            by sections and the :py:func:`pedal.assertions.commands.unit_test`
+            function to combine results.
+        group_names (dict[group, str]): A printable, student-facing name for the
+            group. When a group needs to be rendered out to the user, this
+            will override whatever label was going to be presented instead.
+        hooks (dict[str, list[callable]): A dictionary mapping events to
+            a list of callable functions. Tools can register functions on
+            hooks to have them executed when the event is triggered by another
+            tool. For example, the Assertions tool has hooks on the Source tool
+            to trigger assertion resolutions before advancing to next sections.
+        _tool_data (dict[str, Any]): Maps tool names to their data. The
+                                       namespace for a tool can be used to
+                                       store whatever they want, but will
+                                       probably be in a dictionary itself.
+        resolves (list[Any]): The result of having previously called a
+            resolver. This allows you to check if a report has previously
+            been resolved, or do something with that data.
+        result (FinalFeedback): The FinalFeedback (distinct from a Feedback) that was
+            generated as a result of resolving this Report, or None if the Report is
+            not yet resolved.
+    """
+    #: dict[str, dict]: The
+    #: tools registered for this report, available via their names.
+    TOOLS = {}
+
+    def __init__(self):
+        """
+        Creates a new Report instance.
+        """
+        self._tool_data = {}
+        self.feedback = []
+        self.ignored_feedback = []
+        self.suppressions = {}
+        self.suppressed_labels = {}
+        self.hiddens = set()
+        self.groups = []
+        self.group = None
+        self.group_names = {}
+        self.hooks = {}
+        self.class_hooks = {}
+        self.submission = None
+        self.format = Formatter()
+        self.result = None
+        self.resolves = []
+        self.pools = []
+        self.chosen_pool = None
+        self.overridden_feedbacks = set()
+        log.debug("New Pedal Report created.")
+
+    def clear(self):
+        """
+        Resets the entire report back to its starting form,
+        including deleting any attached submissions, tool data, and feedbacks.
+        It will also reset any overridden fields of feedback classes.
+        However, it will not affect class hooks.
+        """
+        self.feedback.clear()
+        self.ignored_feedback.clear()
+        self.suppressions.clear()
+        self.suppressed_labels.clear()
+        self.hiddens.clear()
+        self._tool_data.clear()
+        self.group = None
+        self.groups.clear()
+        self.group_names.clear()
+        self.hooks.clear()
+        self.submission = None
+        self.result = None
+        self.resolves.clear()
+        self.format = Formatter()
+        self.clear_overridden_feedback()
+
+    def full_clear(self):
+        """ This totally resets the report, including any class hooks. """
+        self.clear()
+        self.class_hooks.clear()
+
+    def clear_overridden_feedback(self):
+        for feedback in self.overridden_feedbacks:
+            feedback._restore_overrides()
+        self.overridden_feedbacks.clear()
+
+    def override_feedback(self, feedback_class):
+        self.overridden_feedbacks.add(feedback_class)
+
+    def set_pools(self, pools):
+        if isinstance(pools, int):
+            pools = list('ABCDEFGHIJKLMNOPQRSTUVWXYZ'[:pools])
+        self.pools = pools
+
+    def contextualize(self, submission):
+        """
+        Attach the given submission to this report.
+
+        Args:
+            submission (:py:class:`pedal.core.submission.Submission`): The
+                submission to attach to this report.
+        """
+        self.submission = submission
+
+    def hide_correctness(self):
+        """
+        Suppress the RESULT category entirely, so that the report doesn't
+        indicate whether or not the submission was correct.
+        TODO: Make this just a regular command.
+        """
+        self.hiddens.add('correct')
+        self.hiddens.add('score')
+
+    def add_feedback(self, feedback):
+        """
+        Attaches the given feedback object to this report.
+
+        Args:
+            feedback (:py:class:`~pedal.core.feedback.Feedback`): The feedback
+                object to attach.
+
+        Returns:
+            :py:class:`~pedal.core.feedback.Feedback`: The attached feedback.
+        """
+        self.feedback.append(feedback)
+        if not isinstance(feedback.parent, (int, str)) and feedback.parent is not None:
+            feedback.parent._get_child_feedback(feedback, True)
+        self.execute_hooks('pedal.report', 'add_feedback', (feedback,))
+        return feedback
+
+    def add_ignored_feedback(self, feedback):
+        """
+        Attaches the given feedback object to this report, but only in the
+        ignored list. That means it should not be considered by the Resolver,
+        since its condition did not apply to the code. Some Resolvers like
+        to know about feedback that was not reached.
+
+        Args:
+            feedback (:py:class:`~pedal.core.feedback.Feedback`): The feedback
+                object to attach.
+
+        Returns:
+            :py:class:`~pedal.core.feedback.Feedback`: The attached feedback.
+        """
+        self.ignored_feedback.append(feedback)
+        if feedback.parent is not None:
+            feedback.parent._get_child_feedback(feedback, False)
+        return feedback
+
+    def suppress(self, category=None, label=True, fields=None):
+        """
+        Suggest that an entire category or label within a category ignored by
+        the resolver.
+        TODO: Currently, only global suppression is supported.
+
+        Args:
+            category (str): The category of feedback to suppress.
+            label (bool or str): A specific label to match against and suppress.
+            fields (dict of key/values): The fields that will be matched exactly to
+                suppress.
+        """
+        if fields is None:
+            fields = {}
+        if category is None:
+            if label not in self.suppressed_labels:
+                self.suppressed_labels[label] = []
+            self.suppressed_labels[label].append(fields)
+        else:
+            category = category.lower()
+            if isinstance(label, str):
+                label = label.lower()
+            if category in FeedbackCategory.ALIASES:
+                category = FeedbackCategory.ALIASES[category]
+            if category not in self.suppressions:
+                self.suppressions[category] = {}
+            if label not in self.suppressions[category]:
+                self.suppressions[category][label] = []
+            self.suppressions[category][label].append(fields)
+
+    def add_hook(self, event, function):
+        """
+        Register the `function` to be executed when the given `event` is
+        triggered.
+        
+        Args:
+            event (str): An event name. Multiple functions can be triggered for
+                the same `event`. The format is as follows: `"namespace.function.extra"`
+                The `".extra"` component is optional to add further nuance, but
+                the general idea is that you are referring to functions that,
+                when called, should trigger other functions to be called first.
+                The namespace is typically a tool or module.
+            function (callable): A callable function. This function should
+                accept a keyword parameter named `report`; this report will be passed
+                as as that argument.
+        """
+        if event not in self.hooks:
+            self.hooks[event] = []
+        self.hooks[event].append(function)
+
+    @classmethod
+    def add_class_hook(cls, event, function):
+        """ Similar to ``add_hook``, except attaches them to the class, so
+        they will be executed for ALL report subclasses. """
+        if event not in cls.class_hooks:
+            cls.class_hooks[event] = []
+        cls.class_hooks[event].append(function)
+
+    def execute_hooks(self, tool, event_name, arguments=None, keyword_arguments=None):
+        """
+        Trigger the functions for all of the associated hooks.
+        Hooks will be called with this report as a keyword `report` argument.
+
+        Args:
+            tool (str): The name of the tool, to namespace events by.
+            event_name (str): The event name (separate words with periods).
+            arguments (tuple[any]): The arguments to be passed to the callback function.
+            keyword_arguments (dict[str, any]): The keyword arguments to be passed to the callback funciton.
+        """
+        if arguments is None:
+            arguments = tuple()
+        if keyword_arguments is None:
+            keyword_arguments = {}
+        event = tool + '.' + event_name
+        if event in self.class_hooks:
+            for function in self.class_hooks[event]:
+                function(report=self, *arguments, **keyword_arguments)
+        if event in self.hooks:
+            for function in self.hooks[event]:
+                function(report=self, *arguments, **keyword_arguments)
+
+    def __getitem__(self, tool_name):
+        """
+        Support retrieving a tool's data from the report using square bracket
+        syntax. So, for example, you can do `MAIN_REPORT['tifa']` and get its
+        data dictionary. If the tool has been registered, but not initialized
+        for this report, then the tool will be
+        :py:method:`pedal.core.tool.reset` first. Otherwise, throws an error
+        that the tool does not exist.
+
+        Args:
+            tool_name (str): The formal name of the tool, most likely specified
+                in its `constants.py` file.
+
+        Returns:
+            dict: The data associated with that tool.
+        """
+        if tool_name not in self._tool_data:
+            if tool_name not in self.TOOLS:
+                raise PedalToolNotRegistered(tool_name, list(self.TOOLS.keys()))
+            self.TOOLS[tool_name].reset(report=self)
+        return self._tool_data[tool_name]
+
+    def __setitem__(self, tool_name, value):
+        """
+        Update the tool's current data. Should largely not be used by anyone.
+        In fact, this could seriously damage the relationships between tools.
+
+        Args:
+            tool_name (str): The name of the tool.
+            value (dict): The new data to set as this tool's namespace.
+        """
+        self._tool_data[tool_name] = value
+
+    def __contains__(self, tool_name):
+        """
+        Determine if the given `tool_name` is available through this report.
+        Args:
+            tool_name (str): The name of a tool.
+
+        Returns:
+            bool: Whether the tool is available.
+        """
+        return tool_name in self._tool_data
+
+    def set_formatter(self, formatter):
+        """
+        Update the formatter with the new option.
+
+        Args:
+            formatter (:py:class:`pedal.core.formatting.Formatter`): The new
+                formatter to use.
+        """
+        self.format = formatter
+
+    @classmethod
+    def register_tool(cls, tool_name: str, reset_function):
+        """
+        Identifies that the given Tool should be made available.
+        Args:
+            tool_name: A unique string identifying this tool.
+            reset_function: The function to call to reset the Tool.
+
+        Returns:
+
+        """
+        if tool_name in cls.TOOLS:
+            raise PedalToolAlreadyRegistered(tool_name)
+        cls.TOOLS[tool_name] = ToolRegistration(tool_name, reset_function)
+
+    def get_current_group(self):
+        if self.groups:
+            return self.groups[-1]
+        else:
+            return None
+
+    def start_group(self, group):
+        self.groups.append(group)
+
+    def stop_group(self, group):
+        """
+        TODO: Should this prematurely end other groups? If so, do they get a
+            callback event to do any wrapup?
+        """
+        if self.groups:
+            self.groups.remove(group)
+
+    def finalize_pools(self):
+        if self.pools:
+            self.chosen_pool = random.choice(self.pools)
+
+    def finalize_feedbacks(self):
+        self.finalize_pools()
+        for feedback in self.feedback + self.ignored_feedback:
+            feedback._finalize()
+
+#: The global Report object. Meant to be used as a default singleton
+#: for any tool, so that instructors do not have to create their own Report.
+#: Of course, all APIs are expected to work with a given Report, and only
+#: default to this Report when no others are given.
+#: Ideally, the average instructor will never know this exists.
+MAIN_REPORT = Report()
+
+# TODO: Give a mechanism for "freezing" a report that you can keep around.
```

### Comparing `pedal-2.6.1/pedal/core/resolver.py` & `pedal-2.6.2/pedal/core/resolver.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/core/scoring.py` & `pedal-2.6.2/pedal/core/scoring.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,121 @@
-"""
-Class for managing custom score objects (e.g., "+20%").
-"""
-import re
-
-SCORE_PATTERN = re.compile(r"(!*)([+\-/*])?([\d.]+)(%)?(.*)")
-
-class Score:
-    def __init__(self, invert, operator, value, percentage, leftovers):
-        self.invert = invert
-        self.operator = operator
-        self.value = value
-        self.percentage = percentage
-        self.leftovers = leftovers
-
-    @classmethod
-    def parse(cls, score):
-        match = SCORE_PATTERN.match(score)
-        if not match:
-            # TODO: Add context of feedback being processed
-            raise ValueError(f"Invalid Score string: {score}")
-        invert = bool(len(match.group(1)) % 2)
-        operator = match.group(2)
-        value = float(match.group(3))
-        percentage = bool(match.group(4) == "%")
-        leftovers = match.group(5)
-        if percentage:
-            value = value / 100.0
-        return Score(invert, operator, value, percentage, leftovers)
-
-    def __truediv__(self, other):
-        if isinstance(other, (int, float)):
-            return Score(self.invert, self.operator, self.value/other, self.percentage, self.leftovers)
-        return NotImplemented(f"Division is not supported between a Score and a {type(other)}")
-
-    def __mul__(self, other):
-        if isinstance(other, (int, float)):
-            return Score(self.invert, self.operator, self.value*other, self.percentage, self.leftovers)
-        return NotImplemented(f"Multiplication is not supported between a Score and a {type(other)}")
-
-    def __rmul__(self, other):
-        return self.__mul__(other)
-
-    def __add__(self, other):
-        if isinstance(other, (int, float)):
-            return Score(self.invert, self.operator, self.value+other, self.percentage, self.leftovers)
-        return NotImplemented(f"Addition is not supported between a Score and a {type(other)}")
-
-    def __radd__(self, other):
-        return self.__add__(other)
-
-    def __sub__(self, other):
-        if isinstance(other, (int, float)):
-            return Score(self.invert, self.operator, self.value-other, self.percentage, self.leftovers)
-        return NotImplemented(f"Subtraction is not supported between a Score and a {type(other)}")
-
-    def __str__(self):
-        value = self.value
-        if self.percentage:
-            # TODO: Being careless with rounding here.
-            value *= 100
-        value = str(round(value))
-        operator = self.operator
-        if not operator:
-            operator = "+"
-        return (
-            ("!" if self.invert else "")+operator+value +
-            ("%" if self.percentage else "")+self.leftovers
-        )
-
-    def to_percent_string(self):
-        value = self.value * 100
-        value = str(round(value))
-        operator = "+" if not self.operator else self.operator
-        return ("!" if self.invert else "") + operator + value + "%" + self.leftovers
-
-    def add_to_current(self, current):
-        if self.operator in ("+", None, "") and not self.invert:
-            current += self.value
-        elif self.operator == "-" and not self.invert:
-            current -= self.value
-        elif self.operator == "*" and not self.invert:
-            current *= self.value
-        elif self.operator == "/" and not self.invert:
-            current /= self.value
-        return current
-
-
-def combine_scores(scores, invert_scores=None) -> float:
-    """
-    Combines the scores (and possible invert_scores) into a single number.
-    Args:
-        scores ():
-        invert_scores ():
-
-    Returns:
-        total_score (float): Two decimal place float of final result.
-    """
-    total = 0
-    for score in scores:
-        if isinstance(score, (int, float)):
-            total += score
-        elif isinstance(score, str):
-            total = Score.parse(score).add_to_current(total)
-    if invert_scores:
-        for score in invert_scores:
-            if isinstance(score, str):
-                total = Score.parse("!"+score).add_to_current(total)
-    return round(total, 2)
+"""
+Class for managing custom score objects (e.g., "+20%").
+"""
+import re
+
+SCORE_PATTERN = re.compile(r"(!*)([+\-/*])?([\d.]+)(%)?(.*)")
+
+class Score:
+    def __init__(self, invert, operator, value, percentage, leftovers):
+        self.invert = invert
+        self.operator = operator
+        self.value = value
+        self.percentage = percentage
+        self.leftovers = leftovers
+
+    @classmethod
+    def parse(cls, score):
+        match = SCORE_PATTERN.match(score)
+        if not match:
+            # TODO: Add context of feedback being processed
+            raise ValueError(f"Invalid Score string: {score}")
+        invert = bool(len(match.group(1)) % 2)
+        operator = match.group(2)
+        value = float(match.group(3))
+        percentage = bool(match.group(4) == "%")
+        leftovers = match.group(5)
+        if percentage:
+            value = value / 100.0
+        return Score(invert, operator, value, percentage, leftovers)
+
+    def __truediv__(self, other):
+        if isinstance(other, (int, float)):
+            return Score(self.invert, self.operator, self.value/other, self.percentage, self.leftovers)
+        return NotImplemented(f"Division is not supported between a Score and a {type(other)}")
+
+    def __mul__(self, other):
+        if isinstance(other, (int, float)):
+            return Score(self.invert, self.operator, self.value*other, self.percentage, self.leftovers)
+        return NotImplemented(f"Multiplication is not supported between a Score and a {type(other)}")
+
+    def __rmul__(self, other):
+        return self.__mul__(other)
+
+    def __add__(self, other):
+        if isinstance(other, (int, float)):
+            return Score(self.invert, self.operator, self.value+other, self.percentage, self.leftovers)
+        return NotImplemented(f"Addition is not supported between a Score and a {type(other)}")
+
+    def __radd__(self, other):
+        return self.__add__(other)
+
+    def __sub__(self, other):
+        if isinstance(other, (int, float)):
+            return Score(self.invert, self.operator, self.value-other, self.percentage, self.leftovers)
+        return NotImplemented(f"Subtraction is not supported between a Score and a {type(other)}")
+
+    def __str__(self):
+        value = self.value
+        if self.percentage:
+            # TODO: Being careless with rounding here.
+            value *= 100
+        value = str(round(value))
+        operator = self.operator
+        if not operator:
+            operator = "+"
+        return (
+            ("!" if self.invert else "")+operator+value +
+            ("%" if self.percentage else "")+self.leftovers
+        )
+
+    def to_percent_string(self):
+        value = self.value * 100
+        value = str(round(value))
+        operator = "+" if not self.operator else self.operator
+        return ("!" if self.invert else "") + operator + value + "%" + self.leftovers
+
+    def add_to_current(self, current):
+        """
+        if self.operator == "+":
+            if not self.invert:
+                current += self.value
+            else:
+                current -= self.value
+        elif self.operator == "-":
+            if not self.invert:
+                current -= self.value
+            else:
+                current += self.value
+        """
+        if self.operator in (None, "", "+") and not self.invert:
+            current += self.value
+        elif self.operator == "-" and not self.invert:
+            current -= self.value
+        elif self.operator == "*" and not self.invert:
+            current *= self.value
+        elif self.operator == "/" and not self.invert:
+            current /= self.value
+        return current
+
+
+def combine_scores(scores, invert_scores=None) -> float:
+    """
+    Combines the scores (and possible invert_scores) into a single number.
+    Args:
+        scores ():
+        invert_scores ():
+
+    Returns:
+        total_score (float): Two decimal place float of final result.
+    """
+    total = 0
+    for score in scores:
+        if isinstance(score, (int, float)):
+            total += score
+        elif isinstance(score, str):
+            total = Score.parse(score).add_to_current(total)
+    if invert_scores:
+        for score in invert_scores:
+            if isinstance(score, str):
+                total = Score.parse("!"+score).add_to_current(total)
+    return round(total, 2)
```

### Comparing `pedal-2.6.1/pedal/core/submission.py` & `pedal-2.6.2/pedal/core/submission.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/core/tool.py` & `pedal-2.6.2/pedal/core/tool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/environments/__init__.py` & `pedal-2.6.2/pedal/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/environments/blockpy.py` & `pedal-2.6.2/pedal/environments/blockpy.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/environments/gradescope.py` & `pedal-2.6.2/pedal/environments/gradescope.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/environments/jupyter.py` & `pedal-2.6.2/pedal/environments/jupyter.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/environments/nbgrader.py` & `pedal-2.6.2/pedal/environments/nbgrader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/environments/sandbox.py` & `pedal-2.6.2/pedal/environments/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/environments/standard.py` & `pedal-2.6.2/pedal/environments/standard.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/environments/terminal.py` & `pedal-2.6.2/pedal/environments/terminal.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,30 +55,30 @@
 
 
 @make_resolver
 def resolve_on_terminal(report=MAIN_REPORT):
     # print("\033[47m", "-" * 35, "FEEDBACK", "-" * 35, "\033[0m", file=file)
     feedback = resolve(report)
     print("")
-    print(f"{REVERSE}FEEDBACK{RESET} Based on your code, here are some tips and recommendations:\n")
+    print(f"{REVERSE} FEEDBACK {RESET} Based on your code, here are some tips and recommendations:\n")
     if feedback.correct:
         print(f"{BOLD_GREEN}{CHECKMARK}{RESET}️  Your code ran successfully.\n")
         print(f"{feedback.message}")
     else:
         print(f"{BOLD_RED}{CROSSMARK}{RESET}  {feedback.title}\n")
         print(f"{feedback.message}")
     print("")
 
     # if feedback.category not in (FeedbackCategory.SYNTAX, FeedbackCategory.RUNTIME):
     # Print out the first runtime/syntax error that we encounter
     for python_error in get_python_errors(report):
         if python_error:
             python_error_native_message = to_native_message(python_error)
             if python_error_native_message:
-                print(f"{REVERSE}TERMINAL OUTPUT{RESET} For reference, here is the original Python error:")
+                print(f"{REVERSE} TERMINAL OUTPUT {RESET} For reference, here is the original Python error:")
                 print(python_error_native_message)
         break
     return feedback
 
 
 def to_native_message(error):
     if not any(field in error.fields for field in ['traceback_message', 'exception_name', 'exception_message']):
@@ -125,15 +125,15 @@
         if not skip_tifa:
             tifa_analysis(report=self.report)
         if inputs:
             set_input(inputs)
         if skip_run:
             student = get_sandbox(report=report)
         else:
-            print(f"{REVERSE}YOUR CODE{RESET} We ran your code. Here's the output:\n")
+            print(f"{REVERSE} YOUR CODE {RESET} We ran your code. Here's the output:\n")
             if trace:
                 start_trace()
             if real_io:
                 allow_real_io()
             student = run(report=report, threaded=threaded)
             if real_io:
                 block_real_io()
```

### Comparing `pedal-2.6.1/pedal/environments/vpl.py` & `pedal-2.6.2/pedal/environments/vpl.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/extensions/microbit.py` & `pedal-2.6.2/pedal/extensions/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/extensions/plotting.py` & `pedal-2.6.2/pedal/extensions/plotting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/questions/__init__.py` & `pedal-2.6.2/pedal/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/questions/feedbacks.py` & `pedal-2.6.2/pedal/questions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/questions/graders.py` & `pedal-2.6.2/pedal/questions/graders.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/questions/loader.py` & `pedal-2.6.2/pedal/questions/loader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/questions/pool.py` & `pedal-2.6.2/pedal/questions/pool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/questions/questions.py` & `pedal-2.6.2/pedal/questions/questions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/questions/setup.py` & `pedal-2.6.2/pedal/questions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/resolvers/__init__.py` & `pedal-2.6.2/pedal/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/resolvers/core.py` & `pedal-2.6.2/pedal/resolvers/core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/resolvers/export.py` & `pedal-2.6.2/pedal/resolvers/export.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/resolvers/full.py` & `pedal-2.6.2/pedal/resolvers/full.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/resolvers/sectional.py` & `pedal-2.6.2/pedal/resolvers/sectional.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/resolvers/simple.py` & `pedal-2.6.2/pedal/resolvers/simple.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-"""
-Perhaps better named "single" instead, this returns exactly one piece of feedback.
-
-
-# Scoring
-
-Some more notes on scoring.
-
-NEGATIVE feedback function that IS TRIGGERED will subtract it's percentage.
-    i.e., a bad thing happened
-NEGATIVE feedback function that is NOT triggered will not subtract it's percentage.
-POSITIVE feedback function that IS triggered will add it's percentage.
-POSITIVE feedback function that is NOT triggered will not add it's percentage.
-
-What happens when you have no `score` given? It's just a None. Probably should
-    default to doing nothing, right? Just gets skipped in calculating the score.
-
-
-Valence  | Triggered? | Operator | Result | Example
----------------------------------------------------
-Positive | Yes        | +        | Add 5  | compliment()
-Negative | Yes        | +        | 0      | assert_equal()
-Positive | No         | +        | 0      | compliment()
-Negative | No         | +        | Add 5  | assert_equal()
-Positive | Yes        | -        | 0      | compliment()
-Negative | Yes        | -        | Sub 5  | assert_equal()
-Positive | No         | -        | Sub 5  | compliment() * Weird situation
-Negative | No         | -        | 0      | assert_equal()
-
-"+N": Default behavior for a float argument
-"+N%": allows you to use whole numbers ("+20%" == "+.2" == .2)
-"+N/Z": allows you to specify the total number of points consistently.
-"-N"
-"-N%"
-"*N"
-"*N%"
-"/N"
-"/N%"
-"=N": set the score absolutely
-"=N%": set the score to the percentage
-"^N" or "^N%": Cap the maximum number of points possible
-"_N" or "_N%": Cap the minimum number of points possible
-
-How do scores work within a group? How do you specify that point allocations
-happen within a group, or absolutely overall?
-* Unit test - we control, this so teacher API is for "this function overall"
-* Sections - teachers write statement level stuff
-* Phase - teachers write statement level stuff
-
-So I think scores default to their current group OR global depending on context.
-You can override a score given within a group to be global using "global"?
-    "+N% global"
-
-You could also have "scoring modes" to change default behavior.
-    { (Feedback.NEGATIVE, None): "=0%" }
-    set_score_mode("Negative None is =0%")
-        If you encounter a Negative None, then the score gets set to 0%.
-
-I'd like to be able to use constants too, I think.
-    set_grading_constant("UNITTESTS", .25)
-    "+UNITTESTS%"
-    "+DEFINITION%"
-
-```python
-# Give 5% if this does not get triggered
-assert_equal(4, 5, score="+5%")
-
-# Give 5% if this does get triggered
-give_partial("+5%")
-```
-
-"""
-from pedal.core.report import MAIN_REPORT
-from pedal.core.final_feedback import FinalFeedback, set_correct_no_errors
-from pedal.core.feedback import Feedback, DEFAULT_CATEGORY_PRIORITY
-from pedal.resolvers.core import make_resolver
-
-
-def by_priority(feedback):
-    """
-    Converts a feedback into a numeric representation for sorting.
-
-    Args:
-        feedback (Feedback): The feedback object to convert
-    Returns:
-        float: A decimal number representing the feedback's relative priority.
-    """
-    category = Feedback.CATEGORIES.UNKNOWN
-    if feedback.category is not None:
-        category = feedback.category.lower()
-    priority = 'medium'
-    if feedback.priority is not None:
-        priority = feedback.priority.lower()
-        priority = Feedback.CATEGORIES.ALIASES.get(priority, priority)
-    if category in DEFAULT_CATEGORY_PRIORITY:
-        value = DEFAULT_CATEGORY_PRIORITY.index(category)
-    else:
-        value = len(DEFAULT_CATEGORY_PRIORITY)
-    if priority in DEFAULT_CATEGORY_PRIORITY:
-        value = DEFAULT_CATEGORY_PRIORITY.index(priority)
-        priority = 'medium'
-    offset = priority_offset(priority)
-    return value + offset
-
-
-def priority_offset(priority):
-    """
-
-    Args:
-        priority:
-
-    Returns:
-
-    """
-    if priority == 'low':
-        return .7
-    elif priority == 'medium':
-        return .5
-    elif priority == 'high':
-        return .3
-    else:
-        return .1
-
-
-@make_resolver
-def resolve(report=MAIN_REPORT, priority_key=by_priority):
-    """
-    Args:
-        priority_key: The key function to sort feedbacks by
-        report (Report): The report object to resolve down. Defaults to the
-                         global MAIN_REPORT
-
-    Returns
-        str: A string of HTML feedback to be delivered
-    """
-    # Prepare feedbacks
-    report.finalize_feedbacks()
-    feedbacks = report.feedback + report.ignored_feedback
-    feedbacks.sort(key=priority_key)
-    # Create the initial final feedback
-    final = set_correct_no_errors(report)
-    # Process each feedback in turn
-    for feedback in feedbacks:
-        final.merge(feedback)
-    # Override empty message
-    final.finalize()
-    report.result = final
-    report.resolves.append(final)
-    return final
-
+"""
+Perhaps better named "single" instead, this returns exactly one piece of feedback.
+
+
+# Scoring
+
+Some more notes on scoring.
+
+NEGATIVE feedback function that IS TRIGGERED will subtract it's percentage.
+    i.e., a bad thing happened
+NEGATIVE feedback function that is NOT triggered will not subtract it's percentage.
+POSITIVE feedback function that IS triggered will add it's percentage.
+POSITIVE feedback function that is NOT triggered will not add it's percentage.
+
+What happens when you have no `score` given? It's just a None. Probably should
+    default to doing nothing, right? Just gets skipped in calculating the score.
+
+
+Valence  | Triggered? | Operator | Result | Example
+---------------------------------------------------
+Positive | Yes        | +        | Add 5  | compliment()
+Negative | Yes        | +        | 0      | assert_equal()
+Positive | No         | +        | 0      | compliment()
+Negative | No         | +        | Add 5  | assert_equal()
+Positive | Yes        | -        | 0      | compliment()
+Negative | Yes        | -        | Sub 5  | assert_equal()
+Positive | No         | -        | Sub 5  | compliment() * Weird situation
+Negative | No         | -        | 0      | assert_equal()
+
+"+N": Default behavior for a float argument
+"+N%": allows you to use whole numbers ("+20%" == "+.2" == .2)
+"+N/Z": allows you to specify the total number of points consistently.
+"-N"
+"-N%"
+"*N"
+"*N%"
+"/N"
+"/N%"
+"=N": set the score absolutely
+"=N%": set the score to the percentage
+"^N" or "^N%": Cap the maximum number of points possible
+"_N" or "_N%": Cap the minimum number of points possible
+
+How do scores work within a group? How do you specify that point allocations
+happen within a group, or absolutely overall?
+* Unit test - we control, this so teacher API is for "this function overall"
+* Sections - teachers write statement level stuff
+* Phase - teachers write statement level stuff
+
+So I think scores default to their current group OR global depending on context.
+You can override a score given within a group to be global using "global"?
+    "+N% global"
+
+You could also have "scoring modes" to change default behavior.
+    { (Feedback.NEGATIVE, None): "=0%" }
+    set_score_mode("Negative None is =0%")
+        If you encounter a Negative None, then the score gets set to 0%.
+
+I'd like to be able to use constants too, I think.
+    set_grading_constant("UNITTESTS", .25)
+    "+UNITTESTS%"
+    "+DEFINITION%"
+
+```python
+# Give 5% if this does not get triggered
+assert_equal(4, 5, score="+5%")
+
+# Give 5% if this does get triggered
+give_partial("+5%")
+```
+
+"""
+from pedal.core.report import MAIN_REPORT
+from pedal.core.final_feedback import FinalFeedback, set_correct_no_errors
+from pedal.core.feedback import Feedback, DEFAULT_CATEGORY_PRIORITY
+from pedal.resolvers.core import make_resolver
+
+
+def by_priority(feedback):
+    """
+    Converts a feedback into a numeric representation for sorting.
+
+    Args:
+        feedback (Feedback): The feedback object to convert
+    Returns:
+        float: A decimal number representing the feedback's relative priority.
+    """
+    category = Feedback.CATEGORIES.UNKNOWN
+    if feedback.category is not None:
+        category = feedback.category.lower()
+    priority = 'medium'
+    if feedback.priority is not None:
+        priority = feedback.priority.lower()
+        priority = Feedback.CATEGORIES.ALIASES.get(priority, priority)
+    if category in DEFAULT_CATEGORY_PRIORITY:
+        value = DEFAULT_CATEGORY_PRIORITY.index(category)
+    else:
+        value = len(DEFAULT_CATEGORY_PRIORITY)
+    if priority in DEFAULT_CATEGORY_PRIORITY:
+        value = DEFAULT_CATEGORY_PRIORITY.index(priority)
+        priority = 'medium'
+    offset = priority_offset(priority)
+    return value + offset
+
+
+def priority_offset(priority):
+    """
+
+    Args:
+        priority:
+
+    Returns:
+
+    """
+    if priority == 'low':
+        return .7
+    elif priority == 'medium':
+        return .5
+    elif priority == 'high':
+        return .3
+    else:
+        return .1
+
+
+@make_resolver
+def resolve(report=MAIN_REPORT, priority_key=by_priority):
+    """
+    Args:
+        priority_key: The key function to sort feedbacks by
+        report (Report): The report object to resolve down. Defaults to the
+                         global MAIN_REPORT
+
+    Returns
+        str: A string of HTML feedback to be delivered
+    """
+    # Prepare feedbacks
+    report.finalize_feedbacks()
+    feedbacks = report.feedback + report.ignored_feedback
+    feedbacks.sort(key=priority_key)
+    # Create the initial final feedback
+    final = set_correct_no_errors(report)
+    # Process each feedback in turn
+    for feedback in feedbacks:
+        final.merge(feedback)
+    # Override empty message
+    final.finalize()
+    report.result = final
+    report.resolves.append(final)
+    return final
+
```

### Comparing `pedal-2.6.1/pedal/resolvers/statistics.py` & `pedal-2.6.2/pedal/resolvers/statistics.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/sandbox/__init__.py` & `pedal-2.6.2/pedal/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/sandbox/commands.py` & `pedal-2.6.2/pedal/sandbox/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/sandbox/data.py` & `pedal-2.6.2/pedal/sandbox/data.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/sandbox/exceptions.py` & `pedal-2.6.2/pedal/sandbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/sandbox/feedbacks.py` & `pedal-2.6.2/pedal/sandbox/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/sandbox/library/designer.py` & `pedal-2.6.2/pedal/sandbox/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/sandbox/library/drafter.py` & `pedal-2.6.2/pedal/sandbox/library/drafter_library.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,80 @@
+from dataclasses import dataclass
 from pedal.sandbox.mocked import MockModuleExposing, MethodExposer
 from pedal.sandbox.mocked import MockModule
 from pedal.utilities.system import IS_PYTHON_36
+from functools import wraps
+
+try:
+    import drafter
+except:
+    drafter = None
 
 
 def friendly_urls(url: str) -> str:
     if url.strip("/") == "index":
         return "/"
     if not url.startswith('/'):
         url = '/' + url
     return url
 
 
+@dataclass
+class GenericComponent:
+    def __init__(self, name, *args, **kwargs):
+        self.name = name
+        self.args = args
+        self.kwargs = kwargs
+
+
+def _load_drafter_component(name):
+
+    @wraps(name)
+    def call_drafter_component(*args, **kwargs):
+        if drafter is not None:
+            component = getattr(drafter, name)
+            # Component Button <class 'drafter.Button'> (MockDrafter(), 'Change the Message', <function change_message>) {}
+            # raise Exception(f"Component {name} {component} {args} {kwargs}")
+            return component(*args[1:], **kwargs)
+        else:
+            return GenericComponent(name, *args, **kwargs)
+
+    return call_drafter_component
+
+
 class MockDrafter(MockModuleExposing):
     """
     Mock Drafter library that can be used to capture data from the students' program execution.
     """
     expose = MethodExposer()
     UNKNOWN_FUNCTIONS = []
 
     def __init__(self):
         super().__init__()
         self.original_routes = []
         self.routes = {}
         self._unknown_calls = []
         self.server_started = False
+        self.state = None
 
     def __repr__(self):
         return f"MockDrafter()"
 
     def __str__(self):
         return f"<MockDrafter()>"
 
     def add_route(self, url, func):
         self.original_routes.append((url, func))
         url = friendly_urls(url)
         self.routes[url] = func
 
     @expose
-    def start_server(self):
+    def start_server(self, initial_state):
         self.server_started = True
+        self.state = initial_state
 
     @expose
     def show_debug_information(self):
         pass
 
     @expose
     def hide_debug_information(self):
@@ -60,33 +92,22 @@
             if url is None:
                 local_url = func.__name__
             self.add_route(local_url, func)
             return func
 
         return make_route
 
-    @staticmethod
-    def _load_drafter_component(name):
-
-        def call_drafter_component(*args, **kwargs):
-            import drafter
-            return getattr(drafter, name)(*args, **kwargs)
-
-        return call_drafter_component
-
-    COMPONENTS = ['BulletedList', 'Button', 'CheckBox',
-                  'Header', 'HorizontalRule', 'Image', 'LineBreak', 'Link', 'LinkContent',
-                  'NumberedList', 'Page', 'PageContent', 'SelectBox',
-                  'SubmitButton', 'Table', 'Text', 'TextArea', 'TextBox']
-    for component in COMPONENTS:
-        expose.add_with_name(_load_drafter_component(component), component)
-
-
-
-
+COMPONENTS = ['BulletedList', 'Button', 'CheckBox',
+              'Header', 'HorizontalRule', 'Image', 'LineBreak', 'Link', 'LinkContent',
+              'NumberedList', 'Page', 'PageContent', 'SelectBox', 'Span', "Argument",
+              'SubmitButton', 'Table', 'Text', 'TextArea', 'TextBox']
+for component in COMPONENTS:
+    loaded_component = _load_drafter_component(component)
+    setattr(MockDrafter, component, loaded_component)
+    MockDrafter.expose.add_with_name(loaded_component, component)
 
 
 
 """
 route, start_server
 'show_debug_information', 
 'hide_debug_information',
```

### Comparing `pedal-2.6.1/pedal/sandbox/library/matplotlib.py` & `pedal-2.6.2/pedal/sandbox/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/sandbox/library/microbit.py` & `pedal-2.6.2/pedal/sandbox/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/sandbox/library/turtles.py` & `pedal-2.6.2/pedal/sandbox/library/turtles.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/sandbox/mocked.py` & `pedal-2.6.2/pedal/sandbox/mocked.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,362 +1,362 @@
-"""
-Mocked functions that can be used to prevent malicious or accidental `eval`
-behavior.
-"""
-import re
-import sys
-import types
-from io import StringIO
-
-from pedal.core.report import Report
-from pedal.sandbox.exceptions import (SandboxNoMoreInputsException,
-                                      SandboxPreventModule)
-from pedal.utilities.system import IS_PYTHON_36
-
-
-def do_nothing(*args, **kwargs):
-    """ A function that does absolutely nothing. """
-
-
-def _disabled_compile(source, filename, mode, flags=0, dont_inherit=False):
-    """
-    A version of the built-in `compile` method that fails with a runtime
-    error.
-    """
-    raise RuntimeError("You are not allowed to call 'compile'.")
-
-
-def _disabled_eval(object, globals=globals(), locals=None):
-    """
-    A version of the built-in `eval` method that fails with a runtime
-    error.
-    """
-    raise RuntimeError("You are not allowed to call 'eval'.")
-
-
-# -------------------------------------------------------------
-
-
-def _disabled_exec(object, globals=globals(), locals=None):
-    """
-    A version of the built-in `exec` method that fails with a runtime
-    error.
-    """
-    raise RuntimeError("You are not allowed to call 'exec'.")
-
-
-# -------------------------------------------------------------
-
-
-def _disabled_globals():
-    """
-    A version of the built-in `globals` method that fails with a runtime
-    error.
-    """
-    raise RuntimeError("You are not allowed to call 'globals'.")
-
-
-class FunctionNotAllowed(Exception):
-    """ Exception created when a function that is not allowed is used. """
-
-
-def disabled_builtin(name):
-    """
-
-    Args:
-        name:
-
-    Returns:
-
-    """
-    def _disabled_version(*args, **kwargs):
-        raise FunctionNotAllowed("You are not allowed to call '{}'.".format(name))
-    return _disabled_version
-
-
-# TODO: This needs to be a field in the Sandbox object's data
-_OPEN_FORBIDDEN_NAMES = re.compile(r"(^[./])|(\.py$)")
-_OPEN_FORBIDDEN_MODES = re.compile(r"[wa+]")
-
-# TODO: Allow the user to give a function instead of a REGEX
-# TODO: We need to mock the whole OS library, honestly, not just `open`
-def create_open_function(report: Report, forbidden_names=_OPEN_FORBIDDEN_NAMES, forbidden_modes=_OPEN_FORBIDDEN_MODES):
-    """
-    Creates a new version of the `open` built-in that will avoid looking at certain filenames,
-    and will also respect the given Report's Submission's Files.
-
-    Args:
-        report:
-
-    Returns:
-
-    """
-    def _restricted_open(name, mode='r', buffering=-1):
-        if forbidden_names.search(name):
-            raise RuntimeError("The filename you passed to 'open' is restricted.")
-        elif forbidden_modes.search(mode):
-            raise RuntimeError("You are not allowed to 'open' files for writing.")
-        elif report.submission and name in report.submission.files:
-            return StringIO(report.submission.files[name])
-        else:
-            return ORIGINAL_BUILTINS['open'](name, mode, buffering)
-    return _restricted_open
-
-# TODO: Allow this to be flexible
-
-
-def create_import_function(report: Report, sandbox):
-    """
-    Creates a new version of the `__import__` function (which is used by the import keyword)
-    that will not let students import Pedal or its submodules.
-
-    Args:
-        report:
-
-    Returns:
-
-    """
-    def _restricted_import(module_name, globals=None, locals=None, fromlist=(), level=0):
-        filename = module_name.replace(".", "/")+".py"
-        if module_name == 'pedal' or module_name.startswith('pedal.'):
-            raise RuntimeError("You cannot import pedal!")
-        elif report.submission and filename in report.submission.files:
-            if module_name not in sys.modules:
-                contents = report.submission.files[filename]
-                return sandbox._import(contents, module_name, filename, sandbox.threaded)
-        return ORIGINAL_BUILTINS['__import__'](module_name, globals, locals, fromlist, level)
-    return _restricted_import
-
-
-try:
-    __builtins__
-except NameError:
-    _default_builtins = {'globals': globals,
-                         'locals': locals,
-                         'open': open,
-                         'input': input,
-                         '__import__': __import__}
-else:
-    if isinstance(__builtins__, types.ModuleType):
-        _default_builtins = __builtins__.__dict__
-    else:
-        _default_builtins = __builtins__
-
-ORIGINAL_BUILTINS = {
-    'globals': _default_builtins['globals'],
-    'locals': _default_builtins['locals'],
-    'open': _default_builtins['open'],
-    'input': _default_builtins['input'],
-    'print': _default_builtins.get('print'),
-    'exec': _default_builtins.get('exec', _disabled_exec),
-    'eval': _default_builtins.get('eval', _disabled_eval),
-    'compile': _default_builtins.get('compile', _disabled_compile),
-    'exit': disabled_builtin('exit'),
-    '__import__': _default_builtins['__import__']
-}
-
-
-def make_inputs(input_list, repeat=None):
-    """
-    Helper function for creating mock user input.
-
-    Params:
-        input_list (list of str): The list of inputs to be returned
-    Returns:
-        function (str=>str): The mock input function that is returned, which
-                             will return the next element of input_list each
-                             time it is called.
-    """
-    generator = iter(input_list)
-
-    def mock_input(prompt=''):
-        """
-
-        Args:
-            prompt:
-
-        Returns:
-
-        """
-        print(prompt)
-        try:
-            return next(generator)
-        except StopIteration as SI:
-            if repeat is None:
-                # TODO: Make this a custom exception
-                raise SandboxNoMoreInputsException("User had no more input to give.")
-            else:
-                return repeat
-
-    return mock_input
-
-
-class PrintingStringIO(StringIO):
-    _ORIGINAL_STDOUT = sys.stdout
-
-    def __init__(self, stdout=None, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._original_stdout = self._ORIGINAL_STDOUT if stdout is None else stdout
-
-    def write(self, s):
-        self._original_stdout.write(s)
-        return super().write(s)
-
-    def flush(self):
-        self._original_stdout.flush()
-        return super().flush()
-
-    def writelines(self, lines):
-        self._original_stdout.writelines(lines)
-        return super().writelines(lines)
-
-
-def make_fake_output(also_print=False) -> StringIO:
-    """
-    Creates a fake output stream that can be used to capture the output
-    of a function. This is useful for testing functions that print things.
-
-    Args:
-        also_print (bool): Whether to also print the output to the console.
-
-    Returns:
-        StringIO: The fake output stream.
-    """
-    fake_output = StringIO()
-
-
-    return fake_output
-
-
-def create_module(module_names):
-    """
-    Creates empty ModuleTypes based on the ``module_name``. Correctly
-    creates parent modules for submodules as needed to fill in the path.
-
-    Args:
-        module_name: A dot-separated string of modules, as if for ``import``. A list of
-            names can also be passed in instead. If multiple names are given, they should all have the same root!
-
-    Returns:
-        :py:class:`types.ModuleType`: The root module created.
-        dict[str, :py:class:`types.ModuleType`]: A dictionary of newly created
-            modules, including the root and the actual target.
-        :py:class:`types.ModuleType`: The target module created.
-    """
-    if isinstance(module_names, str):
-        module_names = [module_names]
-    if not module_names:
-        raise ValueError("No modules provided; need at least one module to create!")
-    root = None
-    modules = {}
-    for module_name in module_names:
-        submodule_names = module_name.split(".")
-        if root is None:
-            root = types.ModuleType(submodule_names[0])
-        modules[submodule_names[0]] = root
-        reconstructed_path = submodule_names[0]
-        for submodule_name in submodule_names[1:]:
-            reconstructed_path += "." + submodule_name
-            new_submodule = types.ModuleType(reconstructed_path)
-            setattr(root, submodule_name, new_submodule)
-            modules[reconstructed_path] = new_submodule
-    return root, modules, modules[module_names[0]]
-
-
-class MockModule:
-    SUBMODULES = {}
-
-    def _generate_patches(self):
-        return {k: v for k, v in vars(self).items()
-                if not k.startswith('_')}
-
-    def add_to_module(self, main_module, submodules=None):
-        for name, value in self._generate_patches().items():
-            setattr(main_module, name, value)
-        for submodule_name in self.SUBMODULES:
-            property_name = submodule_name.split('.', maxsplit=1)[1]
-            mock_submodule = getattr(main_module, property_name)
-            # the actual created Module object
-            submodule = submodules[submodule_name]
-            # Populate the actual module object with the fake submodule's data
-            mock_submodule.add_to_module(submodule)
-            # Update the main module to point to the actual module, instead of the fake submodule
-            setattr(main_module, property_name, submodule)
-
-
-class MockDictModule(MockModule):
-    def __init__(self, fields):
-        self.fields = fields
-
-    def _generate_patches(self):
-        return self.fields
-
-
-class BlockedModule(MockModule):
-    def __init__(self, name):
-        self.module_name = name
-
-    def _generate_patches(self):
-        return {'__getattr__': self.getter}
-
-    def getter(self, key):
-        """ If anything asks, we prevent the module. Except for __file__. """
-        # Needed to support coverage - it's okay to ask who I am.
-        if key == '__file__':
-            return self.module_name
-        else:
-            self.prevent_module()
-
-    def prevent_module(self, *args, **kwargs):
-        """
-
-        Args:
-            **kwargs:
-        """
-        raise SandboxPreventModule(f"You cannot import `{self.module_name}` from student code.")
-
-
-class MockPedal(BlockedModule):
-    """ TODO: Deprecated? """
-    module_name = "pedal"
-
-
-def generic_function_capture(self, function_name):
-    def _call(*args, **kwargs):
-        """ This function does nothing. """
-        # TODO: Capture name; does this need to be a decorated function?
-        self._unknown_calls.append((function_name, args, kwargs))
-    return _call
-
-
-class MethodExposer:
-    def __init__(self):
-        self.tracked_functions = {}
-
-    def __call__(self, function):
-        self.tracked_functions[function.__name__] = function
-        return function
-
-    def add_with_name(self, function, name):
-        self.tracked_functions[name] = function
-        return function
-
-
-class MockModuleExposing(MockModule):
-    expose: MethodExposer
-    UNKNOWN_FUNCTIONS: list
-
-    def get_submodules(self):
-        return {}
-
-    def _generate_patches(self):
-        # Use function descriptor to get a bound version of each method
-        fields = {n: f.__get__(self) for n, f in self.expose.tracked_functions.items()}
-        fields.update({
-            name: generic_function_capture(self, name)
-            for name in self.UNKNOWN_FUNCTIONS
-        })
-        fields.update(self.get_submodules())
-        return fields
-
-
-from pedal.sandbox.library import *
+"""
+Mocked functions that can be used to prevent malicious or accidental `eval`
+behavior.
+"""
+import re
+import sys
+import types
+from io import StringIO
+
+from pedal.core.report import Report
+from pedal.sandbox.exceptions import (SandboxNoMoreInputsException,
+                                      SandboxPreventModule)
+from pedal.utilities.system import IS_PYTHON_36
+
+
+def do_nothing(*args, **kwargs):
+    """ A function that does absolutely nothing. """
+
+
+def _disabled_compile(source, filename, mode, flags=0, dont_inherit=False):
+    """
+    A version of the built-in `compile` method that fails with a runtime
+    error.
+    """
+    raise RuntimeError("You are not allowed to call 'compile'.")
+
+
+def _disabled_eval(object, globals=globals(), locals=None):
+    """
+    A version of the built-in `eval` method that fails with a runtime
+    error.
+    """
+    raise RuntimeError("You are not allowed to call 'eval'.")
+
+
+# -------------------------------------------------------------
+
+
+def _disabled_exec(object, globals=globals(), locals=None):
+    """
+    A version of the built-in `exec` method that fails with a runtime
+    error.
+    """
+    raise RuntimeError("You are not allowed to call 'exec'.")
+
+
+# -------------------------------------------------------------
+
+
+def _disabled_globals():
+    """
+    A version of the built-in `globals` method that fails with a runtime
+    error.
+    """
+    raise RuntimeError("You are not allowed to call 'globals'.")
+
+
+class FunctionNotAllowed(Exception):
+    """ Exception created when a function that is not allowed is used. """
+
+
+def disabled_builtin(name):
+    """
+
+    Args:
+        name:
+
+    Returns:
+
+    """
+    def _disabled_version(*args, **kwargs):
+        raise FunctionNotAllowed("You are not allowed to call '{}'.".format(name))
+    return _disabled_version
+
+
+# TODO: This needs to be a field in the Sandbox object's data
+_OPEN_FORBIDDEN_NAMES = re.compile(r"(^[./])|(\.py$)")
+_OPEN_FORBIDDEN_MODES = re.compile(r"[wa+]")
+
+# TODO: Allow the user to give a function instead of a REGEX
+# TODO: We need to mock the whole OS library, honestly, not just `open`
+def create_open_function(report: Report, forbidden_names=_OPEN_FORBIDDEN_NAMES, forbidden_modes=_OPEN_FORBIDDEN_MODES):
+    """
+    Creates a new version of the `open` built-in that will avoid looking at certain filenames,
+    and will also respect the given Report's Submission's Files.
+
+    Args:
+        report:
+
+    Returns:
+
+    """
+    def _restricted_open(name, mode='r', buffering=-1):
+        if forbidden_names.search(name):
+            raise RuntimeError("The filename you passed to 'open' is restricted.")
+        elif forbidden_modes.search(mode):
+            raise RuntimeError("You are not allowed to 'open' files for writing.")
+        elif report.submission and name in report.submission.files:
+            return StringIO(report.submission.files[name])
+        else:
+            return ORIGINAL_BUILTINS['open'](name, mode, buffering)
+    return _restricted_open
+
+# TODO: Allow this to be flexible
+
+
+def create_import_function(report: Report, sandbox):
+    """
+    Creates a new version of the `__import__` function (which is used by the import keyword)
+    that will not let students import Pedal or its submodules.
+
+    Args:
+        report:
+
+    Returns:
+
+    """
+    def _restricted_import(module_name, globals=None, locals=None, fromlist=(), level=0):
+        filename = module_name.replace(".", "/")+".py"
+        if module_name == 'pedal' or module_name.startswith('pedal.'):
+            raise RuntimeError("You cannot import pedal!")
+        elif report.submission and filename in report.submission.files:
+            if module_name not in sys.modules:
+                contents = report.submission.files[filename]
+                return sandbox._import(contents, module_name, filename, sandbox.threaded)
+        return ORIGINAL_BUILTINS['__import__'](module_name, globals, locals, fromlist, level)
+    return _restricted_import
+
+
+try:
+    __builtins__
+except NameError:
+    _default_builtins = {'globals': globals,
+                         'locals': locals,
+                         'open': open,
+                         'input': input,
+                         '__import__': __import__}
+else:
+    if isinstance(__builtins__, types.ModuleType):
+        _default_builtins = __builtins__.__dict__
+    else:
+        _default_builtins = __builtins__
+
+ORIGINAL_BUILTINS = {
+    'globals': _default_builtins['globals'],
+    'locals': _default_builtins['locals'],
+    'open': _default_builtins['open'],
+    'input': _default_builtins['input'],
+    'print': _default_builtins.get('print'),
+    'exec': _default_builtins.get('exec', _disabled_exec),
+    'eval': _default_builtins.get('eval', _disabled_eval),
+    'compile': _default_builtins.get('compile', _disabled_compile),
+    'exit': disabled_builtin('exit'),
+    '__import__': _default_builtins['__import__']
+}
+
+
+def make_inputs(input_list, repeat=None):
+    """
+    Helper function for creating mock user input.
+
+    Params:
+        input_list (list of str): The list of inputs to be returned
+    Returns:
+        function (str=>str): The mock input function that is returned, which
+                             will return the next element of input_list each
+                             time it is called.
+    """
+    generator = iter(input_list)
+
+    def mock_input(prompt=''):
+        """
+
+        Args:
+            prompt:
+
+        Returns:
+
+        """
+        print(prompt)
+        try:
+            return next(generator)
+        except StopIteration as SI:
+            if repeat is None:
+                # TODO: Make this a custom exception
+                raise SandboxNoMoreInputsException("User had no more input to give.")
+            else:
+                return repeat
+
+    return mock_input
+
+
+class PrintingStringIO(StringIO):
+    _ORIGINAL_STDOUT = sys.stdout
+
+    def __init__(self, stdout=None, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._original_stdout = self._ORIGINAL_STDOUT if stdout is None else stdout
+
+    def write(self, s):
+        self._original_stdout.write(s)
+        return super().write(s)
+
+    def flush(self):
+        self._original_stdout.flush()
+        return super().flush()
+
+    def writelines(self, lines):
+        self._original_stdout.writelines(lines)
+        return super().writelines(lines)
+
+
+def make_fake_output(also_print=False) -> StringIO:
+    """
+    Creates a fake output stream that can be used to capture the output
+    of a function. This is useful for testing functions that print things.
+
+    Args:
+        also_print (bool): Whether to also print the output to the console.
+
+    Returns:
+        StringIO: The fake output stream.
+    """
+    fake_output = StringIO()
+
+
+    return fake_output
+
+
+def create_module(module_names):
+    """
+    Creates empty ModuleTypes based on the ``module_name``. Correctly
+    creates parent modules for submodules as needed to fill in the path.
+
+    Args:
+        module_name: A dot-separated string of modules, as if for ``import``. A list of
+            names can also be passed in instead. If multiple names are given, they should all have the same root!
+
+    Returns:
+        :py:class:`types.ModuleType`: The root module created.
+        dict[str, :py:class:`types.ModuleType`]: A dictionary of newly created
+            modules, including the root and the actual target.
+        :py:class:`types.ModuleType`: The target module created.
+    """
+    if isinstance(module_names, str):
+        module_names = [module_names]
+    if not module_names:
+        raise ValueError("No modules provided; need at least one module to create!")
+    root = None
+    modules = {}
+    for module_name in module_names:
+        submodule_names = module_name.split(".")
+        if root is None:
+            root = types.ModuleType(submodule_names[0])
+        modules[submodule_names[0]] = root
+        reconstructed_path = submodule_names[0]
+        for submodule_name in submodule_names[1:]:
+            reconstructed_path += "." + submodule_name
+            new_submodule = types.ModuleType(reconstructed_path)
+            setattr(root, submodule_name, new_submodule)
+            modules[reconstructed_path] = new_submodule
+    return root, modules, modules[module_names[0]]
+
+
+class MockModule:
+    SUBMODULES = {}
+
+    def _generate_patches(self):
+        return {k: v for k, v in vars(self).items()
+                if not k.startswith('_')}
+
+    def add_to_module(self, main_module, submodules=None):
+        for name, value in self._generate_patches().items():
+            setattr(main_module, name, value)
+        for submodule_name in self.SUBMODULES:
+            property_name = submodule_name.split('.', maxsplit=1)[1]
+            mock_submodule = getattr(main_module, property_name)
+            # the actual created Module object
+            submodule = submodules[submodule_name]
+            # Populate the actual module object with the fake submodule's data
+            mock_submodule.add_to_module(submodule)
+            # Update the main module to point to the actual module, instead of the fake submodule
+            setattr(main_module, property_name, submodule)
+
+
+class MockDictModule(MockModule):
+    def __init__(self, fields):
+        self.fields = fields
+
+    def _generate_patches(self):
+        return self.fields
+
+
+class BlockedModule(MockModule):
+    def __init__(self, name):
+        self.module_name = name
+
+    def _generate_patches(self):
+        return {'__getattr__': self.getter}
+
+    def getter(self, key):
+        """ If anything asks, we prevent the module. Except for __file__. """
+        # Needed to support coverage - it's okay to ask who I am.
+        if key == '__file__':
+            return self.module_name
+        else:
+            self.prevent_module()
+
+    def prevent_module(self, *args, **kwargs):
+        """
+
+        Args:
+            **kwargs:
+        """
+        raise SandboxPreventModule(f"You cannot import `{self.module_name}` from student code.")
+
+
+class MockPedal(BlockedModule):
+    """ TODO: Deprecated? """
+    module_name = "pedal"
+
+
+def generic_function_capture(self, function_name):
+    def _call(*args, **kwargs):
+        """ This function does nothing. """
+        # TODO: Capture name; does this need to be a decorated function?
+        self._unknown_calls.append((function_name, args, kwargs))
+    return _call
+
+
+class MethodExposer:
+    def __init__(self):
+        self.tracked_functions = {}
+
+    def __call__(self, function):
+        self.tracked_functions[function.__name__] = function
+        return function
+
+    def add_with_name(self, function, name):
+        self.tracked_functions[name] = function
+        return function
+
+
+class MockModuleExposing(MockModule):
+    expose: MethodExposer
+    UNKNOWN_FUNCTIONS: list
+
+    def get_submodules(self):
+        return {}
+
+    def _generate_patches(self):
+        # Use function descriptor to get a bound version of each method
+        fields = {n: f.__get__(self) for n, f in self.expose.tracked_functions.items()}
+        fields.update({
+            name: generic_function_capture(self, name)
+            for name in self.UNKNOWN_FUNCTIONS
+        })
+        fields.update(self.get_submodules())
+        return fields
+
+
+from pedal.sandbox.library import *
```

### Comparing `pedal-2.6.1/pedal/sandbox/result.py` & `pedal-2.6.2/pedal/sandbox/result.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/sandbox/sandbox.py` & `pedal-2.6.2/pedal/sandbox/sandbox.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,999 +1,999 @@
-"""
-File containing the Sandbox class.
-
-TODO: Handle sys.argv
-
-"""
-
-import sys
-import io
-import types
-from itertools import zip_longest
-from unittest.mock import patch
-
-from pedal.core.feedback_category import FeedbackCategory
-from pedal.core.report import MAIN_REPORT
-from pedal.sandbox.mocked import PrintingStringIO
-from pedal.utilities.exceptions import ExpandedTraceback, improve_builtin_exceptions
-from pedal.sandbox.data import SandboxVariable, SandboxContextKind, \
-    SandboxContext, SandboxModules
-from pedal.sandbox import mocked
-from pedal.sandbox.constants import TOOL_NAME
-from pedal.sandbox.feedbacks import runtime_error, EXCEPTION_FF_MAP
-from pedal.sandbox.exceptions import SandboxHasNoFunction, SandboxHasNoVariable
-from pedal.sandbox.timeout import timeout
-from pedal.sandbox.result import SandboxResult
-from pedal.sandbox.tracer import TRACER_STYLES
-
-
-class Sandbox:
-    """
-    Args:
-        report (:py:class:`~pedal.core.report.Report`): The report that this
-            Sandbox is attached to.
-
-    Attributes:
-        data (dict[str, Any]): The namespace that the context are occurring in.
-            Note that this is mutable.
-        result: TODO
-        output (list[str]): The list of strings that have been printed to the
-            console by :py:func:`print`. Note that line endings have been removed
-            using :py:func:`string.rstrip`.
-        inputs (list[str]): The list of strings that will be passed to
-            :py:func:`input`.
-        raw_output (str): A concatenated string of all the text that was printed
-            to console. No changes have been made to the text.
-        exception (Exception or None): The exception that occurred during the
-            most recent execution, or None if nothing happened.
-        feedback: TODO
-        modules.plots: TODO
-        modules.turtles: TODO
-        target: TODO
-        allowed_time (int): How long to allow before stopping execution.
-        tracer_style (str): TODO
-        _context (list[SandboxContext]): The history of executions made in
-            this sandbox.
-        _next_context_id (int): The ID of the next execution context.
-        _current_patches (list[Patch]): A stack of patches that are currently
-            being used. This allows recursive patching behavior.
-        MAXIMUM_TEMPORARY_LENGTH (int): How long to allow arguments to be before
-            turning them into temporary variables.
-    """
-
-    MAXIMUM_TEMPORARY_LENGTH = 200
-    MAXIMUM_INPUTS = 100000
-
-    def __init__(self, report=MAIN_REPORT):
-        self.report = report
-        # Namespace
-        self.data = {}
-        self.result = None
-        self.exception = None
-        self.feedback = None
-        # Contextualization
-        self._context = []
-        self._current_context = None
-        self._next_context_id = 0
-        self._context_group_start = []
-        # Patching
-        self._current_patches = []
-        self._current_stdout = []
-        # Temporary Variables
-        self._temporary_variables = set()
-        self._backup_variables = {}
-        # Modules
-        self._module_overrides = {}
-        self.modules = SandboxModules()
-        self.clear_mocks()
-        self.clear_data()
-        # Inputs
-        self.inputs = []
-        # Outputs
-        self.raw_output = ""
-        self.output = []
-        # Target
-        self.target = None
-
-        # Proxying results
-        self.result_proxy_class = SandboxResult
-        # Show the full traceback
-        self.full_traceback = False
-        # Use threading?
-        self.threaded = False
-        self.allowed_time = 3
-        # Tracer Styles
-        self.tracer_style = 'none'
-
-    ############################################################################
-    # Execution (run/call/eval)
-
-    def _import(self, code, module_name, filename, threaded, **meta):
-        """
-        Import the code as a new module. Requires prior `_execute` of some
-        manner to have already started (e.g., a `call`, `run`, or `evaluate`).
-        This does NOT reset the context, setup output capturing, or handle exceptions.
-        Instead, it relies on the existing infrastructure to do so.
-
-        Args:
-            code:
-            module_name:
-            threaded:
-            **meta:
-
-        Returns:
-
-        """
-        if threaded:
-            return timeout(self.allowed_time, self._import, code, module_name, filename, False, **meta)
-        # TODO: Skulpt doesn't support `module.__dict__` manipulation,
-        #   but once it does we don't need to manually copy over the attrs afterwards
-        imported_module = types.ModuleType(module_name)
-        # Patch the builtins using the same rules as `execute`
-        #    EXCEPT only the builtins, not the other stuff?
-        imported_module_data = {}
-        self._reset_builtins(imported_module_data)
-        builtins = self._module_overrides.get('__builtins__', {})
-        self._mock_builtins(imported_module_data, builtins)
-        # Compile and execute code
-        compiled_code = compile(code, filename, 'exec')
-        with self.trace.as_filename(filename, code):
-            exec(compiled_code, imported_module_data)
-        # Copy over data to module
-        for key, value in imported_module_data.items():
-            setattr(imported_module, key, value)
-        # And get them back the module
-        return imported_module
-
-    def _execute_with_timeout(self, code, filename, kind, **meta):
-        """
-        Execute the given code, but stop after `self.allowed_time`.
-        Args:
-            code (str):
-            filename (str):
-            kind (:py:class:`pedal.sandbox.sandbox_mixins.SandboxContextKind`):
-
-        Returns:
-            :py:class:`pedal.sandbox.sandbox.Sandbox`
-        """
-        try:
-            return timeout(self.allowed_time, self._execute,
-                           code, filename, kind, False, **meta)
-        except TimeoutError as timeout_exception:
-            self._stop_patches()
-            self._capture_exception(timeout_exception, sys.exc_info(),
-                                    code, filename)
-            return self
-
-    def _execute(self, code, filename, kind, threaded, **meta):
-        # Handle any threading if necessary
-        if threaded:
-            return self._execute_with_timeout(code, filename, kind, **meta)
-
-        self.clear_exception()
-
-        context = SandboxContext(self._next_context_id, code, filename, kind,
-                                 self.target, [], "",
-                                 self.exception, self.report.submission, **meta)
-        self._context.append(context)
-
-        # Patch in dangerous built-ins
-        # Override builtins and mock stuff out
-        self._start_mocking(context)
-        self.data['__name__'] = "__main__"
-        try:
-            # TODO: Support CaitNode and Ast (needs skulpt to support compile better)
-            compiled_code = compile(code, filename, 'exec')
-            with self.trace.as_filename(filename, code):
-                exec(compiled_code, self.data)
-        except Exception as user_exception:
-            self._stop_mocking(context)
-            self._capture_exception(user_exception, sys.exc_info(),
-                                    code, filename)
-        # NOTE: https://docs.python.org/3/library/exceptions.html#SystemExit
-        # This exception does not inherit from Exception and has to be caught separately
-        except SystemExit as system_exit:
-            self._stop_mocking(context)
-            self._capture_exception(system_exit, sys.exc_info(),
-                                    code, filename)
-        else:
-            self._stop_mocking(context)
-
-        self._next_context_id += 1
-        return self
-
-    def run(self, code=None, filename=None, inputs=None, threaded=None,
-            after=None, before=None, real_io=False):
-        """
-        If both ``code`` and ``filename`` are None, then the submission's
-        main file will be executed. If ``code`` is given but ``filename`` is
-        not, then it is assumed to be instructor code.
-
-        TODO: This should actually return the ExecutionContext that was generated, right?
-            But the user should be able to treat that as if it were the Sandbox...
-
-        Args:
-            real_io: If True, makes print and input actually write to stdout.
-            code (str or :py:class:`~pedal.cait.cait_node.CaitNode` or None):
-                The code to execute.
-            filename (str or None): The filename to use for this code.
-            inputs (list[str]): Optional inputs to be passed to
-                :py:func:`~pedal.sandbox.Sandbox.set_input`.
-            threaded (bool): Whether or not to run this code in a threaded
-                environment, which allows for timeouts.
-            after (str): Code to run after this code (without a filename).
-            before (str): Code to run before this code (without a filename).
-
-
-        Returns:
-            Sandbox: This sandbox instance.
-        """
-        if real_io:
-            self.allow_function('print')
-            self.set_input(input)
-        if threaded is None:
-            threaded = self.threaded
-        if code is None:
-            if filename is None:
-                filename = self.report.submission.main_file
-            code = self.report.submission.files[filename]
-        elif filename is None:
-            filename = self.report.submission.instructor_file
-        if inputs is not None:
-            self.set_input(inputs)
-        if before is not None:
-            self._execute(before, filename, SandboxContextKind.RUN, threaded)
-        self.target = None
-        self._execute(code, filename, SandboxContextKind.RUN, threaded)
-        if after is not None:
-            self._execute(after, filename, SandboxContextKind.RUN, threaded)
-        if real_io:
-            self.clear_mocked_function('print')
-            self.clear_input()
-        return self
-
-    def call(self, function, *args, target="_", threaded=None,
-             inputs=None, function_kwargs=None,
-             args_locals=None, kwargs_locals=None, **kwargs):
-        """
-        Execute the given function from the student's namespace.
-
-        The ``args_locals`` and ``kwargs_locals`` values allow you to
-        use student's local variables as arguments, instead of literal values.
-        They actually support any arbitrary Python code, it will be injected
-        without modification.
-
-        Args:
-            function (str): The name of the function to call.
-            *args (Any): Any number of positional arguments to be passed to
-                the called function.
-            target (str): The variable to assign the result of this call to.
-                Defaults to ``"_"``.
-            threaded (bool): Whether or not to run this code in a threaded
-                environment, which allows for timeouts.
-            inputs (str or list[str]):
-            function_kwargs (dict[str, Any]): Additional keyword arguments
-                that could not be passed in directly via ``**kwargs`` (perhaps
-                because they conflict with an existing parameter like
-                ``target``).
-            args_locals (list[str]): A list of names (or any valid Python
-                expression) that will be passed as positional arguments to
-                the function (as opposed to actual values). If any value is
-                None (or if the list is too short), then the corresponding
-                position argument from ``*args`` will be used instead.
-            kwargs_locals (dict[str, str]): A dictionary of keyword argument
-                names mapped to local names (or any valid Python expression),
-                that will be used as keyword parameters similar to
-                ``args_locals``.
-            **kwargs (): Additional keyword arguments passed to the called
-                function.
-
-        Returns:
-            Exception or :py:class:`~pedal.sandbox.sandbox.SandboxResult`: The
-                result of calling the function will be returned, proxied behind
-                a SandboxResult (which attempts to perfectly emulate that
-                value). If the function call failed, the exception will be
-                returned instead.
-        """
-        if threaded is None:
-            threaded = self.threaded
-        # Confirm that the function_name exists
-        if function not in self.functions:
-            if function not in self.data:
-                self.exception = SandboxHasNoVariable(
-                    "The function {function} does not exist.".format(function=function)
-                )
-            else:
-                self.exception = SandboxHasNoFunction(
-                    "The variable {function} is not a function.".format(function=function)
-                )
-            return self.exception
-        # Handle convenience setup
-        if inputs is not None:
-            self.set_input(inputs)
-        if function_kwargs is not None:
-            kwargs.update(function_kwargs)
-        if args_locals is None:
-            args_locals = []
-        if kwargs_locals is None:
-            kwargs_locals = []
-        # Make the call and evaluate it
-        self.target = target
-        actual, student, arguments = self._construct_call(function, args, kwargs,
-                                                          args_locals, kwargs_locals,
-                                                          target)
-        context_id = self._next_context_id
-
-        self._execute(actual, self.report.submission.instructor_file,
-                      SandboxContextKind.CALL, threaded,
-                      called=function, args=arguments)
-        self._purge_temporaries()
-        return self._handle_result(target, context_id)
-
-    def evaluate(self, code, target="_", threaded=None):
-        """
-        Evaluates the given code and assigns the result to the given target.
-        Will cause an error if ``code`` is not a valid expression.
-
-        # TODO: Clean up syntax error.
-
-        Args:
-            code (str or :py:class:`~pedal.cait.cait_node.CaitNode`):
-                The code to execute. If a CaitNode, then that will be executed
-                directly instead of being compiled.
-            target (str): The name of the variable to assign the result to.
-                Note that the result is also returned by this function.
-            threaded (bool): Whether or not to run this code in a threaded
-                environment, which allows for timeouts.
-
-        Returns:
-            Exception or :py:class:`~pedal.sandbox.sandbox.SandboxResult`: The
-                result of evaluating the code will be returned, proxied behind
-                a SandboxResult (which attempts to perfectly emulate that
-                value). If the function call failed, the exception will be
-                returned instead.
-        """
-        if threaded is None:
-            threaded = self.threaded
-        self.target = target
-        code = f"{target} = {code}"
-        context_id = self._next_context_id
-        self._execute(code, self.report.submission.instructor_file,
-                      SandboxContextKind.EVAL, threaded=threaded)
-        return self._handle_result(target, context_id)
-
-    def _handle_result(self, target, context_id):
-        """ Determine the appropriate return value (either an exception or the
-        value stored in target. Also updates self.result. """
-        if self.exception is None:
-            self.result = self.data[target]
-            if self.result_proxy_class is not None:
-                self.result = self.result_proxy_class(self.result,
-                                                      context_id=context_id,
-                                                      sandbox=self)
-            return self.result
-        else:
-            if self.result_proxy_class is not None:
-                self.exception = self.result_proxy_class(self.exception,
-                                                         context_id=context_id,
-                                                         sandbox=self)
-            return self.exception
-
-    ############################################################################
-    # Context (history of executions)
-
-    def get_context(self, context_id: int = None):
-        """
-        Retrieve the most recent contexts.
-
-        Returns:
-            list[:py:class:`pedal.sandbox.sandbox_mixins.SandboxContext`]: The
-                most recent execution, or executions if currently in a group.
-
-        """
-        # TODO: Test off-by-one-errors
-        if context_id is None:
-            if not self._context_group_start:
-                return self._context[-1:]
-            else:
-                return self._context[self._context_group_start[-1]:]
-        else:
-            if not self._context_group_start:
-                return [self._context[context_id]]
-            else:
-                for past_context_group_starts in self._context_group_start[::-1]:
-                    if past_context_group_starts < context_id + 1:
-                        return self._context[past_context_group_starts:context_id + 1]
-                return self._context[:context_id + 1]
-
-    def _guess_context(self, target_name):
-        """
-        Tries to figure out the best context for the given target_name, by
-        first checking whether the target was ever used in a CALL or EVAL.
-        If it fails to find it, then it uses the most recent RUN. Otherwise,
-        it just returns None.
-
-        Returns:
-            :py:class:`pedal.sandbox.data.SandboxContext` or None: The found
-                context, or None.
-        """
-        # Was it a target for a CALL or EVAL?
-        for context in self._context[::-1]:
-            if context.kind in (SandboxContextKind.EVAL, SandboxContextKind.CALL):
-                if context.target == target_name:
-                    return context
-        # Just get the last run
-        for context in self._context[::-1]:
-            if context.kind == SandboxContextKind.RUN:
-                return context
-        # Okay just give up
-        return None
-
-    def start_grouping_context(self):
-        """ Any subsequent executions will be grouped. """
-        self._context_group_start.append(self._next_context_id)
-
-    def stop_grouping_context(self):
-        """ Stop grouping subsequent executions. """
-        return self._context_group_start.pop()
-
-    def clear_context(self):
-        """ Removes the history of any previous executions. """
-        self._context_group_start.clear()
-        self._context.clear()
-
-    ############################################################################
-    # Tracing
-    def _set_tracer_style(self, tracer_style):
-        if tracer_style is None:
-            tracer_style = 'none'
-        self._tracer_style = tracer_style.lower()
-        self.trace = TRACER_STYLES[tracer_style.lower()]()
-
-    def _get_tracer_style(self):
-        return self._tracer_style
-
-    tracer_style = property(_get_tracer_style, _set_tracer_style)
-
-    def clear_tracer(self):
-        """ Stop tracing in this sandbox. """
-        self.tracer_style = 'none'
-
-    ############################################################################
-    # Exception Handling
-
-    def _capture_exception(self, exception, exc_info, code, filename):
-        self.exception = improve_builtin_exceptions(exception)
-        # Load in any extra data
-        context = self.get_context()
-        line_offsets = {}
-        show_filenames = {filename} - {self.report.submission.instructor_file}
-        hide_filenames = {filename}
-        files = self.report.submission.get_files_lines()
-        if filename not in files:
-            files[filename] = code.split("\n")
-        if self.report.submission is not None:
-            lines = self.report.submission.get_lines()
-            show_filenames.update(self.report.submission.files.keys())
-            line_offsets = self.report.submission.line_offsets
-        else:
-            lines = code.split("\n")
-        # Create a better traceback
-        traceback = ExpandedTraceback(self.exception, exc_info,
-                                      self.full_traceback,
-                                      hide_filenames,
-                                      line_offsets,
-                                      show_filenames,
-                                      lines, files)
-        if filename == self.report.submission.instructor_file:
-            priority = FeedbackCategory.SPECIFICATION
-        else:
-            priority = FeedbackCategory.RUNTIME
-
-        runtime_error_function = EXCEPTION_FF_MAP.get(type(self.exception),
-                                                      runtime_error)
-        self.feedback = runtime_error_function(exception=self.exception, context=[context],
-                                               traceback=traceback, location=traceback.line_number,
-                                               report=self.report, priority=priority)
-        self.exception.feedback = self.feedback
-        return False
-
-    def clear_exception(self):
-        """ Removes the latest exception information """
-        self.exception = None
-        self.feedback = None
-
-    ############################################################################
-    # Patching and Mocking
-
-    # TODO: Need to make this cover the `builtins` module, and look into best practices
-    #   for modern Python mocking, to prevent evil access.
-
-    def _mock_builtins(self, data: dict, builtins: dict):
-        builtins = builtins
-        for name, value in builtins.items():
-            if value is True:
-                data['__builtins__'][name] = mocked.ORIGINAL_BUILTINS[name]
-                data[name] = mocked.ORIGINAL_BUILTINS[name]
-            elif value is False:
-                data['__builtins__'][name] = mocked.disabled_builtin(name)
-                data[name] = mocked.disabled_builtin(name)
-            else:
-                data['__builtins__'][name] = value
-                data[name] = value
-
-    def _start_mocking(self, context: SandboxContext):
-        """ Mock input, output, builtins, and modules """
-        # Handle input tracking
-        self.mock_function('input', self._track_inputs(context.inputs))
-        # Override builtin functions
-        self._reset_builtins(self.data)
-        builtins = self._module_overrides.pop('__builtins__', {})
-        self._mock_builtins(self.data, builtins)
-        # Override sys modules
-        overridden_modules = sys.modules.copy()
-        for name, value in self._module_overrides.items():
-            if value is not True:
-                overridden_modules[name] = value
-        self._module_overrides['__builtins__'] = builtins
-        # Handle allowing *actual* printing to the real stdout console
-        if self._module_overrides['__builtins__'].get('print') is not True:
-            self._current_stdout.append(io.StringIO())
-        else:
-            self._current_stdout.append(PrintingStringIO())
-        # And do the patches
-        self._start_patches(
-            patch.dict('sys.modules', overridden_modules),
-            patch('sys.stdout', self._current_stdout[-1]),
-            patch('time.sleep', return_value=None),
-        )
-
-    def _stop_mocking(self, context: SandboxContext):
-        """ Turn off any patches, store output """
-        self._stop_patches()
-        current_stdout = self._current_stdout.pop()
-        self.append_output(current_stdout.getvalue(), context)
-
-    # Patching Functionality
-    def _start_patches(self, *patches):
-        """ Helper function to start and keep track of multiple patches """
-        self._current_patches.append(patches)
-        for a_patch in patches:
-            a_patch.start()
-
-    def _stop_patches(self):
-        """ Helper function to end any tracked patches """
-        if not self._current_patches:
-            return
-        patches = self._current_patches.pop()
-        for a_patch in patches:
-            a_patch.stop()
-
-    def clear_mocks(self, reset_default_mocks=True):
-        """
-        Removes any module or builtin overrides currently in effect.
-
-        Args:
-            reset_default_mocks (bool): If True, also resets the default mocks (e.g., `open`, `__import__`).
-        """
-        self._module_overrides.clear()
-        self.modules.clear()
-        if reset_default_mocks:
-            self.reset_default_overrides()
-
-    def reset_default_overrides(self):
-        """
-        Resets the list of blocked functions and modules to its starting
-        state. This blocks ``compile``, ``eval``, ``exec``, ``globals``,
-        and provides mocked versions of ``open`` and ``import`` that are
-        more restricted. It also blocks the ``pedal`` module.
-        """
-        self._module_overrides['__builtins__'] = {}
-        self.block_function('compile')
-        self.block_function('eval')
-        self.block_function('exec')
-        self.block_function('globals')
-        self.block_function('exit')
-        self.mock_function('open', mocked.create_open_function(self.report))
-        self.mock_function('__import__', mocked.create_import_function(self.report, self))
-        self.block_module('pedal')
-        self.mock_module('turtle', mocked.MockTurtle(), 'turtles')
-        self.mock_module('matplotlib.pyplot', mocked.MockPlt(), 'plotting')
-        self.mock_module('designer', mocked.MockDesigner(), 'designer')
-        #self.mock_module('drafter', mocked.MockDrafter(), 'drafter')
-        self.mock_module('microbit', mocked.MockMicrobit(), 'microbit')
-
-    def mock_function(self, function_name, new_version):
-        self._module_overrides['__builtins__'][function_name] = new_version
-
-    def allow_function(self, function_name):
-        self._module_overrides['__builtins__'][function_name] = True
-
-    def block_function(self, function_name):
-        self._module_overrides['__builtins__'][function_name] = False
-
-    def clear_mocked_function(self, function_name):
-        """
-        Removes the mocking associated with the given function name.
-
-        Args:
-            function_name (str): The name of the function to be mocked.
-        """
-        if function_name in self._module_overrides['__builtins__']:
-            del self._module_overrides['__builtins__'][function_name]
-
-    def allow_module(self, module_name):
-        """
-
-        Args:
-            module_name (str):
-
-        Returns:
-
-        """
-        self._module_overrides[module_name] = True
-        return self
-
-    def mock_module(self, module_name, new_version, friendly_name=None):
-        """ Create a mocked version of this module. """
-        if friendly_name is None:
-            friendly_name = module_name
-        mocked_modules = self.modules.new_module(new_version, module_name, friendly_name)
-        for name, mocked_version in mocked_modules.items():
-            if name not in self._module_overrides or not self._module_overrides[name]:
-                self._module_overrides[name] = mocked_version
-        return self
-
-    def block_module(self, module_name, friendly_name=None):
-        """
-        Prevent the module from being loaded in student code.
-        Also unloads the module if it has been imported previously by
-        destroying the variable in the current student `data`.
-
-        Args:
-            module_name (str): The name of the module to prevent, as it would
-                be used by import (e.g., ``"matplotlib.pyplot"``).
-            friendly_name (str): A more human-readable name for the module.
-                When accessing the module from the Sandbox, this will be the name
-                to use.
-        Returns:
-            Sandbox: This sandbox.
-        """
-        if friendly_name is None:
-            friendly_name = module_name
-        mocked_modules = self.modules.new_module(mocked.BlockedModule(module_name), module_name, friendly_name)
-        for name, mocked_version in mocked_modules.items():
-            if name not in self._module_overrides or self._module_overrides[name] is True:
-                self._module_overrides[name] = mocked_version
-            if name in self.data:
-                del self.data[name]
-        # self._module_overrides[module_name] = mocked.BlockedModule(module_name)
-        return self
-
-    ############################################################################
-    # Code generation
-
-    def _construct_call(self, function, args, kwargs, args_locals, kwargs_locals,
-                        target):
-        """ Turn the given strings into an actual function call string. """
-        str_args = [arg_name if arg_name is not None else
-                    self._make_temporary('arg', str(index), arg_value)
-                    for index, (arg_value, arg_name)
-                    in enumerate(zip_longest(args, args_locals))]
-        str_kwargs = ["{}={}".format(key,
-                                     self._make_temporary('kwarg', key, value))
-                      if key not in kwargs_locals else
-                      kwargs_locals[key]
-                      for key, value in kwargs.items()]
-        arguments = ", ".join(str_args + str_kwargs)
-        call = f"{function}({arguments})"
-        if target is None:
-            actual = call
-        else:
-            actual = f"{target} = {call}"
-        student_call = call if target == "_" else actual
-        return actual, student_call, arguments
-
-    def _purge_temporaries(self):
-        """
-        Delete any variables in the namespace that have been made as
-        temporaries. This happens automatically after you execute code.
-        """
-        for key in self._temporary_variables:
-            if key in self._backup_variables:
-                self.data[key] = self._backup_variables[key]
-            else:
-                del self.data[key]
-        self._temporary_variables.clear()
-
-    def _make_temporary(self, category, name, value):
-        """
-        Create a temporary variable in the namespace for the given
-        category/name. This is used to load arguments into the namespace to
-        be used in function calls. Temporaries are only created if the value's
-        repr length is too long, as defined by _is_long_value.
-
-        Args:
-            category (str): A categorical division for the temporary variable
-                that can help keep the namespace distinctive - there are a
-                few different kinds of categories (e.g., for regular positional
-                args, star args, kwargs).
-            name (str): A distinctive ID for this variable. The final variable
-                name will be "_temporary_<category>_<name>".
-            value: The value for this argument.
-        Returns:
-            str: The new name for the temporary variable.
-        """
-        if isinstance(value, SandboxVariable):
-            return value.name
-        if len(repr(value)) <= self.MAXIMUM_TEMPORARY_LENGTH:
-            return repr(value)
-        key = '_temporary_{}_{}'.format(category, name)
-        if key in self.data:
-            self._backup_variables[key] = self.data[key]
-        self._temporary_variables.add(key)
-        self.data[key] = value
-        return key
-
-    def make_safe_variable(self, name):
-        """
-        Tries to construct a safe variable name in the current namespace, based
-        off the given one. This is accomplished by appending a "_" and a number
-        of increasing value until no comparable name exists in the namespace.
-        This is particularly useful when you want to create a variable name to
-        assign to, but you are concerned that the user might have a variable
-        with that name already, which their code relies on.
-
-        Args:
-            name (str): A desired target name.
-        Returns:
-            str: A safe target name, based off the given one.
-        """
-        current_addition = ""
-        attempt_index = 2
-        while name + current_addition in self.data:
-            current_addition = "_{}".format(attempt_index)
-            attempt_index += 1
-        return name + current_addition
-
-    ############################################################################
-    # Data Namespace Management
-
-    def clear_data(self):
-        # Temporary data
-        self.data.clear()
-        self._temporary_variables.clear()
-        self._backup_variables.clear()
-        self._reset_builtins(self.data)
-
-    @staticmethod
-    def _reset_builtins(data: dict):
-        """
-        Replace all the existing given `data` with the builtin mocked data.
-        Args:
-            data:
-
-        Returns:
-
-        """
-        data['__builtins__'] = {}
-        for name, value in mocked._default_builtins.items():
-            data['__builtins__'][name] = value
-
-    def set_student_data(self, new_data):
-        """
-        Overwrites the existing student data with the keys and values from
-        the ``new_data``. This copies the data over, but does not modify the
-        reference to ``data``'s dictionary.
-
-        Args:
-            new_data (dict[str, Any]): The new data.
-
-        Returns:
-
-        """
-        self.clear_data()
-        for key, value in new_data.items():
-            self.data[key] = value
-
-    def get_names_by_type(self, type, exclude_builtins=True):
-        """
-
-        Args:
-            type:
-            exclude_builtins:
-
-        Returns:
-
-        """
-        result = []
-        for name, value in self.data.items():
-            if isinstance(value, type):
-                if exclude_builtins and name.startswith('__'):
-                    continue
-                result.append(name)
-        return result
-
-    def get_values_by_type(self, type, exclude_builtins=True):
-        """
-
-        Args:
-            type:
-            exclude_builtins:
-
-        Returns:
-
-        """
-        names = self.get_names_by_type(type, exclude_builtins)
-        return [self.data[name] for name in names]
-
-    def get_variables_by_type(self, type, exclude_builtins=True):
-        """
-
-        Args:
-            type:
-            exclude_builtins:
-
-        Returns:
-
-        """
-        names = self.get_names_by_type(type, exclude_builtins)
-        return [(name, self.data[name]) for name in names]
-
-    @property
-    def functions(self):
-        """
-        Retrieve a list of all the callable names in the students' namespace.
-        In other words, get a list of all the functions the student defined.
-
-        Returns:
-            list of callables
-        """
-        return {k: v for k, v in self.data.items() if callable(v)}
-
-    @property
-    def var(self):
-        """
-
-        Returns:
-
-        """
-        return {k: SandboxVariable(k, v) for k, v in self.data.items()}
-
-    def get_function(self, by_name):
-        """
-        Creates an executable function from the given name, based
-        on the student's namespace. This will be executed using the call
-        method.
-        """
-        return lambda *args, **kwargs: self.call(by_name, *args, **kwargs)
-
-    def __getitem__(self, item):
-        value, exception = None, None
-        try:
-            value = self.data[item]
-        except KeyError:
-            exception = NameError(f"NameError: name '{item}' is not defined")
-        filename = self.report.submission.instructor_file
-        context_id = self._next_context_id
-        best_context = self._guess_context(item)
-        if best_context is None:
-            context = SandboxContext(context_id, str(item), filename,
-                                     SandboxContextKind.GETITEM, item, [], "",
-                                     exception, self.report.submission)
-        else:
-            context = best_context.clone(context_id)
-            context.target = str(item)
-            context.exception = exception
-        self._context.append(context)
-        self._next_context_id += 1
-
-        if self.result_proxy_class is not None:
-            return self.result_proxy_class(value, context_id=context_id,
-                                           sandbox=self)
-        return value
-
-    ############################################################################
-    # Useful Dunders
-
-    # def __repr__(self):
-    #    return "Sandbox({})".format()
-
-    def __str__(self):
-        return "Sandbox(contexts={context_count})".format(context_count=len(self._context))
-
-    ############################################################################
-    # Input Handling
-
-    def clear_input(self):
-        """ Removes any inputs queued. """
-        self.set_input(None)
-        return self
-
-    def set_input(self, inputs, clear=True):
-        """
-        Queues the given value as the next arguments to the `input` function.
-        """
-        if inputs is None:
-            self.inputs = []
-        if clear:
-            self.inputs.clear()
-        if isinstance(inputs, str):
-            self.inputs.append(inputs)
-        elif isinstance(inputs, (int, float, bool)):
-            self.inputs.append(str(inputs))
-        elif isinstance(inputs, (list, tuple)):
-            self.inputs.extend([str(value) for value in inputs])
-        elif inputs is not None:
-            self.inputs = inputs
-        return self
-
-    def _track_inputs(self, context_inputs):
-        """
-        Wraps an input function with a tracker.
-        """
-        self._called_inputs = 0
-
-        def _input_tracker(*args, **kwargs):
-            if args:
-                prompt = args[0]
-            else:
-                prompt = ""
-            if callable(self.inputs):
-                value_entered = self.inputs(prompt)
-            elif self.inputs:
-                print(prompt)
-                value_entered = self.inputs.pop(0)
-            else:
-                # TODO: Make this smarter, more elegant in choosing IF we should repeat 0
-                print(prompt)
-                value_entered = '0'
-            self._context[-1].inputs.append(value_entered)
-            self._called_inputs += 1
-            if self.MAXIMUM_INPUTS is not None:
-                if self.MAXIMUM_INPUTS <= self._called_inputs:
-                    raise IOError(
-                        f"Asked for user input too many times ({self._called_inputs} times). Perhaps you have an infinite loop?")
-            # context_inputs.append(value_entered)
-            return value_entered
-
-        return _input_tracker
-
-    ############################################################################
-    # Output Handling
-
-    def clear_output(self):
-        """ Remove any output currently attached to this sandbox. """
-        # Update outputs
-        self.raw_output = ""
-        self.output.clear()
-        return self
-
-    def append_output(self, raw_output, context):
-        """
-        Adds the string of `raw_output` to the current `raw_output` attribute.
-        The added string will be split on newlines and rstripped to append
-        to the `output` attribute.
-
-        Args:
-            raw_output (str): The new raw_output for the sandbox. To compute
-                the `output` attribute, the system splits and rstrips at
-                newlines.
-            context (:py:class:`pedal.sandbox.data.SandboxContext`): The
-                currently executing context, where this output will be recorded.
-        """
-        self.raw_output += raw_output
-        context.output = raw_output
-        if self.raw_output:
-            lines = raw_output.rstrip().split("\n")
-            lines = [line.rstrip() for line in lines]
-            self.output.extend(lines)
-
-    def clear(self):
-        """ Removes any existing data in this sandbox. """
-        self.clear_data()
-        self.clear_context()
-        self.clear_mocks()
-        self.clear_exception()
-        self.clear_input()
-        self.clear_output()
-        self.clear_tracer()
+"""
+File containing the Sandbox class.
+
+TODO: Handle sys.argv
+
+"""
+
+import sys
+import io
+import types
+from itertools import zip_longest
+from unittest.mock import patch
+
+from pedal.core.feedback_category import FeedbackCategory
+from pedal.core.report import MAIN_REPORT
+from pedal.sandbox.mocked import PrintingStringIO
+from pedal.utilities.exceptions import ExpandedTraceback, improve_builtin_exceptions
+from pedal.sandbox.data import SandboxVariable, SandboxContextKind, \
+    SandboxContext, SandboxModules
+from pedal.sandbox import mocked
+from pedal.sandbox.constants import TOOL_NAME
+from pedal.sandbox.feedbacks import runtime_error, EXCEPTION_FF_MAP
+from pedal.sandbox.exceptions import SandboxHasNoFunction, SandboxHasNoVariable
+from pedal.sandbox.timeout import timeout
+from pedal.sandbox.result import SandboxResult
+from pedal.sandbox.tracer import TRACER_STYLES
+
+
+class Sandbox:
+    """
+    Args:
+        report (:py:class:`~pedal.core.report.Report`): The report that this
+            Sandbox is attached to.
+
+    Attributes:
+        data (dict[str, Any]): The namespace that the context are occurring in.
+            Note that this is mutable.
+        result: TODO
+        output (list[str]): The list of strings that have been printed to the
+            console by :py:func:`print`. Note that line endings have been removed
+            using :py:func:`string.rstrip`.
+        inputs (list[str]): The list of strings that will be passed to
+            :py:func:`input`.
+        raw_output (str): A concatenated string of all the text that was printed
+            to console. No changes have been made to the text.
+        exception (Exception or None): The exception that occurred during the
+            most recent execution, or None if nothing happened.
+        feedback: TODO
+        modules.plots: TODO
+        modules.turtles: TODO
+        target: TODO
+        allowed_time (int): How long to allow before stopping execution.
+        tracer_style (str): TODO
+        _context (list[SandboxContext]): The history of executions made in
+            this sandbox.
+        _next_context_id (int): The ID of the next execution context.
+        _current_patches (list[Patch]): A stack of patches that are currently
+            being used. This allows recursive patching behavior.
+        MAXIMUM_TEMPORARY_LENGTH (int): How long to allow arguments to be before
+            turning them into temporary variables.
+    """
+
+    MAXIMUM_TEMPORARY_LENGTH = 200
+    MAXIMUM_INPUTS = 100000
+
+    def __init__(self, report=MAIN_REPORT):
+        self.report = report
+        # Namespace
+        self.data = {}
+        self.result = None
+        self.exception = None
+        self.feedback = None
+        # Contextualization
+        self._context = []
+        self._current_context = None
+        self._next_context_id = 0
+        self._context_group_start = []
+        # Patching
+        self._current_patches = []
+        self._current_stdout = []
+        # Temporary Variables
+        self._temporary_variables = set()
+        self._backup_variables = {}
+        # Modules
+        self._module_overrides = {}
+        self.modules = SandboxModules()
+        self.clear_mocks()
+        self.clear_data()
+        # Inputs
+        self.inputs = []
+        # Outputs
+        self.raw_output = ""
+        self.output = []
+        # Target
+        self.target = None
+
+        # Proxying results
+        self.result_proxy_class = SandboxResult
+        # Show the full traceback
+        self.full_traceback = False
+        # Use threading?
+        self.threaded = False
+        self.allowed_time = 3
+        # Tracer Styles
+        self.tracer_style = 'none'
+
+    ############################################################################
+    # Execution (run/call/eval)
+
+    def _import(self, code, module_name, filename, threaded, **meta):
+        """
+        Import the code as a new module. Requires prior `_execute` of some
+        manner to have already started (e.g., a `call`, `run`, or `evaluate`).
+        This does NOT reset the context, setup output capturing, or handle exceptions.
+        Instead, it relies on the existing infrastructure to do so.
+
+        Args:
+            code:
+            module_name:
+            threaded:
+            **meta:
+
+        Returns:
+
+        """
+        if threaded:
+            return timeout(self.allowed_time, self._import, code, module_name, filename, False, **meta)
+        # TODO: Skulpt doesn't support `module.__dict__` manipulation,
+        #   but once it does we don't need to manually copy over the attrs afterwards
+        imported_module = types.ModuleType(module_name)
+        # Patch the builtins using the same rules as `execute`
+        #    EXCEPT only the builtins, not the other stuff?
+        imported_module_data = {}
+        self._reset_builtins(imported_module_data)
+        builtins = self._module_overrides.get('__builtins__', {})
+        self._mock_builtins(imported_module_data, builtins)
+        # Compile and execute code
+        compiled_code = compile(code, filename, 'exec')
+        with self.trace.as_filename(filename, code):
+            exec(compiled_code, imported_module_data)
+        # Copy over data to module
+        for key, value in imported_module_data.items():
+            setattr(imported_module, key, value)
+        # And get them back the module
+        return imported_module
+
+    def _execute_with_timeout(self, code, filename, kind, **meta):
+        """
+        Execute the given code, but stop after `self.allowed_time`.
+        Args:
+            code (str):
+            filename (str):
+            kind (:py:class:`pedal.sandbox.sandbox_mixins.SandboxContextKind`):
+
+        Returns:
+            :py:class:`pedal.sandbox.sandbox.Sandbox`
+        """
+        try:
+            return timeout(self.allowed_time, self._execute,
+                           code, filename, kind, False, **meta)
+        except TimeoutError as timeout_exception:
+            self._stop_patches()
+            self._capture_exception(timeout_exception, sys.exc_info(),
+                                    code, filename)
+            return self
+
+    def _execute(self, code, filename, kind, threaded, **meta):
+        # Handle any threading if necessary
+        if threaded:
+            return self._execute_with_timeout(code, filename, kind, **meta)
+
+        self.clear_exception()
+
+        context = SandboxContext(self._next_context_id, code, filename, kind,
+                                 self.target, [], "",
+                                 self.exception, self.report.submission, **meta)
+        self._context.append(context)
+
+        # Patch in dangerous built-ins
+        # Override builtins and mock stuff out
+        self._start_mocking(context)
+        self.data['__name__'] = "__main__"
+        try:
+            # TODO: Support CaitNode and Ast (needs skulpt to support compile better)
+            compiled_code = compile(code, filename, 'exec')
+            with self.trace.as_filename(filename, code):
+                exec(compiled_code, self.data)
+        except Exception as user_exception:
+            self._stop_mocking(context)
+            self._capture_exception(user_exception, sys.exc_info(),
+                                    code, filename)
+        # NOTE: https://docs.python.org/3/library/exceptions.html#SystemExit
+        # This exception does not inherit from Exception and has to be caught separately
+        except SystemExit as system_exit:
+            self._stop_mocking(context)
+            self._capture_exception(system_exit, sys.exc_info(),
+                                    code, filename)
+        else:
+            self._stop_mocking(context)
+
+        self._next_context_id += 1
+        return self
+
+    def run(self, code=None, filename=None, inputs=None, threaded=None,
+            after=None, before=None, real_io=False):
+        """
+        If both ``code`` and ``filename`` are None, then the submission's
+        main file will be executed. If ``code`` is given but ``filename`` is
+        not, then it is assumed to be instructor code.
+
+        TODO: This should actually return the ExecutionContext that was generated, right?
+            But the user should be able to treat that as if it were the Sandbox...
+
+        Args:
+            real_io: If True, makes print and input actually write to stdout.
+            code (str or :py:class:`~pedal.cait.cait_node.CaitNode` or None):
+                The code to execute.
+            filename (str or None): The filename to use for this code.
+            inputs (list[str]): Optional inputs to be passed to
+                :py:func:`~pedal.sandbox.Sandbox.set_input`.
+            threaded (bool): Whether or not to run this code in a threaded
+                environment, which allows for timeouts.
+            after (str): Code to run after this code (without a filename).
+            before (str): Code to run before this code (without a filename).
+
+
+        Returns:
+            Sandbox: This sandbox instance.
+        """
+        if real_io:
+            self.allow_function('print')
+            self.set_input(input)
+        if threaded is None:
+            threaded = self.threaded
+        if code is None:
+            if filename is None:
+                filename = self.report.submission.main_file
+            code = self.report.submission.files[filename]
+        elif filename is None:
+            filename = self.report.submission.instructor_file
+        if inputs is not None:
+            self.set_input(inputs)
+        if before is not None:
+            self._execute(before, filename, SandboxContextKind.RUN, threaded)
+        self.target = None
+        self._execute(code, filename, SandboxContextKind.RUN, threaded)
+        if after is not None:
+            self._execute(after, filename, SandboxContextKind.RUN, threaded)
+        if real_io:
+            self.clear_mocked_function('print')
+            self.clear_input()
+        return self
+
+    def call(self, function, *args, target="_", threaded=None,
+             inputs=None, function_kwargs=None,
+             args_locals=None, kwargs_locals=None, **kwargs):
+        """
+        Execute the given function from the student's namespace.
+
+        The ``args_locals`` and ``kwargs_locals`` values allow you to
+        use student's local variables as arguments, instead of literal values.
+        They actually support any arbitrary Python code, it will be injected
+        without modification.
+
+        Args:
+            function (str): The name of the function to call.
+            *args (Any): Any number of positional arguments to be passed to
+                the called function.
+            target (str): The variable to assign the result of this call to.
+                Defaults to ``"_"``.
+            threaded (bool): Whether or not to run this code in a threaded
+                environment, which allows for timeouts.
+            inputs (str or list[str]):
+            function_kwargs (dict[str, Any]): Additional keyword arguments
+                that could not be passed in directly via ``**kwargs`` (perhaps
+                because they conflict with an existing parameter like
+                ``target``).
+            args_locals (list[str]): A list of names (or any valid Python
+                expression) that will be passed as positional arguments to
+                the function (as opposed to actual values). If any value is
+                None (or if the list is too short), then the corresponding
+                position argument from ``*args`` will be used instead.
+            kwargs_locals (dict[str, str]): A dictionary of keyword argument
+                names mapped to local names (or any valid Python expression),
+                that will be used as keyword parameters similar to
+                ``args_locals``.
+            **kwargs (): Additional keyword arguments passed to the called
+                function.
+
+        Returns:
+            Exception or :py:class:`~pedal.sandbox.sandbox.SandboxResult`: The
+                result of calling the function will be returned, proxied behind
+                a SandboxResult (which attempts to perfectly emulate that
+                value). If the function call failed, the exception will be
+                returned instead.
+        """
+        if threaded is None:
+            threaded = self.threaded
+        # Confirm that the function_name exists
+        if function not in self.functions:
+            if function not in self.data:
+                self.exception = SandboxHasNoVariable(
+                    "The function {function} does not exist.".format(function=function)
+                )
+            else:
+                self.exception = SandboxHasNoFunction(
+                    "The variable {function} is not a function.".format(function=function)
+                )
+            return self.exception
+        # Handle convenience setup
+        if inputs is not None:
+            self.set_input(inputs)
+        if function_kwargs is not None:
+            kwargs.update(function_kwargs)
+        if args_locals is None:
+            args_locals = []
+        if kwargs_locals is None:
+            kwargs_locals = []
+        # Make the call and evaluate it
+        self.target = target
+        actual, student, arguments = self._construct_call(function, args, kwargs,
+                                                          args_locals, kwargs_locals,
+                                                          target)
+        context_id = self._next_context_id
+
+        self._execute(actual, self.report.submission.instructor_file,
+                      SandboxContextKind.CALL, threaded,
+                      called=function, args=arguments)
+        self._purge_temporaries()
+        return self._handle_result(target, context_id)
+
+    def evaluate(self, code, target="_", threaded=None):
+        """
+        Evaluates the given code and assigns the result to the given target.
+        Will cause an error if ``code`` is not a valid expression.
+
+        # TODO: Clean up syntax error.
+
+        Args:
+            code (str or :py:class:`~pedal.cait.cait_node.CaitNode`):
+                The code to execute. If a CaitNode, then that will be executed
+                directly instead of being compiled.
+            target (str): The name of the variable to assign the result to.
+                Note that the result is also returned by this function.
+            threaded (bool): Whether or not to run this code in a threaded
+                environment, which allows for timeouts.
+
+        Returns:
+            Exception or :py:class:`~pedal.sandbox.sandbox.SandboxResult`: The
+                result of evaluating the code will be returned, proxied behind
+                a SandboxResult (which attempts to perfectly emulate that
+                value). If the function call failed, the exception will be
+                returned instead.
+        """
+        if threaded is None:
+            threaded = self.threaded
+        self.target = target
+        code = f"{target} = {code}"
+        context_id = self._next_context_id
+        self._execute(code, self.report.submission.instructor_file,
+                      SandboxContextKind.EVAL, threaded=threaded)
+        return self._handle_result(target, context_id)
+
+    def _handle_result(self, target, context_id):
+        """ Determine the appropriate return value (either an exception or the
+        value stored in target. Also updates self.result. """
+        if self.exception is None:
+            self.result = self.data[target]
+            if self.result_proxy_class is not None:
+                self.result = self.result_proxy_class(self.result,
+                                                      context_id=context_id,
+                                                      sandbox=self)
+            return self.result
+        else:
+            if self.result_proxy_class is not None:
+                self.exception = self.result_proxy_class(self.exception,
+                                                         context_id=context_id,
+                                                         sandbox=self)
+            return self.exception
+
+    ############################################################################
+    # Context (history of executions)
+
+    def get_context(self, context_id: int = None):
+        """
+        Retrieve the most recent contexts.
+
+        Returns:
+            list[:py:class:`pedal.sandbox.sandbox_mixins.SandboxContext`]: The
+                most recent execution, or executions if currently in a group.
+
+        """
+        # TODO: Test off-by-one-errors
+        if context_id is None:
+            if not self._context_group_start:
+                return self._context[-1:]
+            else:
+                return self._context[self._context_group_start[-1]:]
+        else:
+            if not self._context_group_start:
+                return [self._context[context_id]]
+            else:
+                for past_context_group_starts in self._context_group_start[::-1]:
+                    if past_context_group_starts < context_id + 1:
+                        return self._context[past_context_group_starts:context_id + 1]
+                return self._context[:context_id + 1]
+
+    def _guess_context(self, target_name):
+        """
+        Tries to figure out the best context for the given target_name, by
+        first checking whether the target was ever used in a CALL or EVAL.
+        If it fails to find it, then it uses the most recent RUN. Otherwise,
+        it just returns None.
+
+        Returns:
+            :py:class:`pedal.sandbox.data.SandboxContext` or None: The found
+                context, or None.
+        """
+        # Was it a target for a CALL or EVAL?
+        for context in self._context[::-1]:
+            if context.kind in (SandboxContextKind.EVAL, SandboxContextKind.CALL):
+                if context.target == target_name:
+                    return context
+        # Just get the last run
+        for context in self._context[::-1]:
+            if context.kind == SandboxContextKind.RUN:
+                return context
+        # Okay just give up
+        return None
+
+    def start_grouping_context(self):
+        """ Any subsequent executions will be grouped. """
+        self._context_group_start.append(self._next_context_id)
+
+    def stop_grouping_context(self):
+        """ Stop grouping subsequent executions. """
+        return self._context_group_start.pop()
+
+    def clear_context(self):
+        """ Removes the history of any previous executions. """
+        self._context_group_start.clear()
+        self._context.clear()
+
+    ############################################################################
+    # Tracing
+    def _set_tracer_style(self, tracer_style):
+        if tracer_style is None:
+            tracer_style = 'none'
+        self._tracer_style = tracer_style.lower()
+        self.trace = TRACER_STYLES[tracer_style.lower()]()
+
+    def _get_tracer_style(self):
+        return self._tracer_style
+
+    tracer_style = property(_get_tracer_style, _set_tracer_style)
+
+    def clear_tracer(self):
+        """ Stop tracing in this sandbox. """
+        self.tracer_style = 'none'
+
+    ############################################################################
+    # Exception Handling
+
+    def _capture_exception(self, exception, exc_info, code, filename):
+        self.exception = improve_builtin_exceptions(exception)
+        # Load in any extra data
+        context = self.get_context()
+        line_offsets = {}
+        show_filenames = {filename} - {self.report.submission.instructor_file}
+        hide_filenames = {filename}
+        files = self.report.submission.get_files_lines()
+        if filename not in files:
+            files[filename] = code.split("\n")
+        if self.report.submission is not None:
+            lines = self.report.submission.get_lines()
+            show_filenames.update(self.report.submission.files.keys())
+            line_offsets = self.report.submission.line_offsets
+        else:
+            lines = code.split("\n")
+        # Create a better traceback
+        traceback = ExpandedTraceback(self.exception, exc_info,
+                                      self.full_traceback,
+                                      hide_filenames,
+                                      line_offsets,
+                                      show_filenames,
+                                      lines, files)
+        if filename == self.report.submission.instructor_file:
+            priority = FeedbackCategory.SPECIFICATION
+        else:
+            priority = FeedbackCategory.RUNTIME
+
+        runtime_error_function = EXCEPTION_FF_MAP.get(type(self.exception),
+                                                      runtime_error)
+        self.feedback = runtime_error_function(exception=self.exception, context=[context],
+                                               traceback=traceback, location=traceback.line_number,
+                                               report=self.report, priority=priority)
+        self.exception.feedback = self.feedback
+        return False
+
+    def clear_exception(self):
+        """ Removes the latest exception information """
+        self.exception = None
+        self.feedback = None
+
+    ############################################################################
+    # Patching and Mocking
+
+    # TODO: Need to make this cover the `builtins` module, and look into best practices
+    #   for modern Python mocking, to prevent evil access.
+
+    def _mock_builtins(self, data: dict, builtins: dict):
+        builtins = builtins
+        for name, value in builtins.items():
+            if value is True:
+                data['__builtins__'][name] = mocked.ORIGINAL_BUILTINS[name]
+                data[name] = mocked.ORIGINAL_BUILTINS[name]
+            elif value is False:
+                data['__builtins__'][name] = mocked.disabled_builtin(name)
+                data[name] = mocked.disabled_builtin(name)
+            else:
+                data['__builtins__'][name] = value
+                data[name] = value
+
+    def _start_mocking(self, context: SandboxContext):
+        """ Mock input, output, builtins, and modules """
+        # Handle input tracking
+        self.mock_function('input', self._track_inputs(context.inputs))
+        # Override builtin functions
+        self._reset_builtins(self.data)
+        builtins = self._module_overrides.pop('__builtins__', {})
+        self._mock_builtins(self.data, builtins)
+        # Override sys modules
+        overridden_modules = sys.modules.copy()
+        for name, value in self._module_overrides.items():
+            if value is not True:
+                overridden_modules[name] = value
+        self._module_overrides['__builtins__'] = builtins
+        # Handle allowing *actual* printing to the real stdout console
+        if self._module_overrides['__builtins__'].get('print') is not True:
+            self._current_stdout.append(io.StringIO())
+        else:
+            self._current_stdout.append(PrintingStringIO())
+        # And do the patches
+        self._start_patches(
+            patch.dict('sys.modules', overridden_modules),
+            patch('sys.stdout', self._current_stdout[-1]),
+            patch('time.sleep', return_value=None),
+        )
+
+    def _stop_mocking(self, context: SandboxContext):
+        """ Turn off any patches, store output """
+        self._stop_patches()
+        current_stdout = self._current_stdout.pop()
+        self.append_output(current_stdout.getvalue(), context)
+
+    # Patching Functionality
+    def _start_patches(self, *patches):
+        """ Helper function to start and keep track of multiple patches """
+        self._current_patches.append(patches)
+        for a_patch in patches:
+            a_patch.start()
+
+    def _stop_patches(self):
+        """ Helper function to end any tracked patches """
+        if not self._current_patches:
+            return
+        patches = self._current_patches.pop()
+        for a_patch in patches:
+            a_patch.stop()
+
+    def clear_mocks(self, reset_default_mocks=True):
+        """
+        Removes any module or builtin overrides currently in effect.
+
+        Args:
+            reset_default_mocks (bool): If True, also resets the default mocks (e.g., `open`, `__import__`).
+        """
+        self._module_overrides.clear()
+        self.modules.clear()
+        if reset_default_mocks:
+            self.reset_default_overrides()
+
+    def reset_default_overrides(self):
+        """
+        Resets the list of blocked functions and modules to its starting
+        state. This blocks ``compile``, ``eval``, ``exec``, ``globals``,
+        and provides mocked versions of ``open`` and ``import`` that are
+        more restricted. It also blocks the ``pedal`` module.
+        """
+        self._module_overrides['__builtins__'] = {}
+        self.block_function('compile')
+        self.block_function('eval')
+        self.block_function('exec')
+        self.block_function('globals')
+        self.block_function('exit')
+        self.mock_function('open', mocked.create_open_function(self.report))
+        self.mock_function('__import__', mocked.create_import_function(self.report, self))
+        self.block_module('pedal')
+        self.mock_module('turtle', mocked.MockTurtle(), 'turtles')
+        self.mock_module('matplotlib.pyplot', mocked.MockPlt(), 'plotting')
+        self.mock_module('designer', mocked.MockDesigner(), 'designer')
+        self.mock_module('drafter', mocked.MockDrafter(), 'drafter')
+        self.mock_module('microbit', mocked.MockMicrobit(), 'microbit')
+
+    def mock_function(self, function_name, new_version):
+        self._module_overrides['__builtins__'][function_name] = new_version
+
+    def allow_function(self, function_name):
+        self._module_overrides['__builtins__'][function_name] = True
+
+    def block_function(self, function_name):
+        self._module_overrides['__builtins__'][function_name] = False
+
+    def clear_mocked_function(self, function_name):
+        """
+        Removes the mocking associated with the given function name.
+
+        Args:
+            function_name (str): The name of the function to be mocked.
+        """
+        if function_name in self._module_overrides['__builtins__']:
+            del self._module_overrides['__builtins__'][function_name]
+
+    def allow_module(self, module_name):
+        """
+
+        Args:
+            module_name (str):
+
+        Returns:
+
+        """
+        self._module_overrides[module_name] = True
+        return self
+
+    def mock_module(self, module_name, new_version, friendly_name=None):
+        """ Create a mocked version of this module. """
+        if friendly_name is None:
+            friendly_name = module_name
+        mocked_modules = self.modules.new_module(new_version, module_name, friendly_name)
+        for name, mocked_version in mocked_modules.items():
+            if name not in self._module_overrides or not self._module_overrides[name]:
+                self._module_overrides[name] = mocked_version
+        return self
+
+    def block_module(self, module_name, friendly_name=None):
+        """
+        Prevent the module from being loaded in student code.
+        Also unloads the module if it has been imported previously by
+        destroying the variable in the current student `data`.
+
+        Args:
+            module_name (str): The name of the module to prevent, as it would
+                be used by import (e.g., ``"matplotlib.pyplot"``).
+            friendly_name (str): A more human-readable name for the module.
+                When accessing the module from the Sandbox, this will be the name
+                to use.
+        Returns:
+            Sandbox: This sandbox.
+        """
+        if friendly_name is None:
+            friendly_name = module_name
+        mocked_modules = self.modules.new_module(mocked.BlockedModule(module_name), module_name, friendly_name)
+        for name, mocked_version in mocked_modules.items():
+            if name not in self._module_overrides or self._module_overrides[name] is True:
+                self._module_overrides[name] = mocked_version
+            if name in self.data:
+                del self.data[name]
+        # self._module_overrides[module_name] = mocked.BlockedModule(module_name)
+        return self
+
+    ############################################################################
+    # Code generation
+
+    def _construct_call(self, function, args, kwargs, args_locals, kwargs_locals,
+                        target):
+        """ Turn the given strings into an actual function call string. """
+        str_args = [arg_name if arg_name is not None else
+                    self._make_temporary('arg', str(index), arg_value)
+                    for index, (arg_value, arg_name)
+                    in enumerate(zip_longest(args, args_locals))]
+        str_kwargs = ["{}={}".format(key,
+                                     self._make_temporary('kwarg', key, value))
+                      if key not in kwargs_locals else
+                      kwargs_locals[key]
+                      for key, value in kwargs.items()]
+        arguments = ", ".join(str_args + str_kwargs)
+        call = f"{function}({arguments})"
+        if target is None:
+            actual = call
+        else:
+            actual = f"{target} = {call}"
+        student_call = call if target == "_" else actual
+        return actual, student_call, arguments
+
+    def _purge_temporaries(self):
+        """
+        Delete any variables in the namespace that have been made as
+        temporaries. This happens automatically after you execute code.
+        """
+        for key in self._temporary_variables:
+            if key in self._backup_variables:
+                self.data[key] = self._backup_variables[key]
+            else:
+                del self.data[key]
+        self._temporary_variables.clear()
+
+    def _make_temporary(self, category, name, value):
+        """
+        Create a temporary variable in the namespace for the given
+        category/name. This is used to load arguments into the namespace to
+        be used in function calls. Temporaries are only created if the value's
+        repr length is too long, as defined by _is_long_value.
+
+        Args:
+            category (str): A categorical division for the temporary variable
+                that can help keep the namespace distinctive - there are a
+                few different kinds of categories (e.g., for regular positional
+                args, star args, kwargs).
+            name (str): A distinctive ID for this variable. The final variable
+                name will be "_temporary_<category>_<name>".
+            value: The value for this argument.
+        Returns:
+            str: The new name for the temporary variable.
+        """
+        if isinstance(value, SandboxVariable):
+            return value.name
+        if len(repr(value)) <= self.MAXIMUM_TEMPORARY_LENGTH:
+            return repr(value)
+        key = '_temporary_{}_{}'.format(category, name)
+        if key in self.data:
+            self._backup_variables[key] = self.data[key]
+        self._temporary_variables.add(key)
+        self.data[key] = value
+        return key
+
+    def make_safe_variable(self, name):
+        """
+        Tries to construct a safe variable name in the current namespace, based
+        off the given one. This is accomplished by appending a "_" and a number
+        of increasing value until no comparable name exists in the namespace.
+        This is particularly useful when you want to create a variable name to
+        assign to, but you are concerned that the user might have a variable
+        with that name already, which their code relies on.
+
+        Args:
+            name (str): A desired target name.
+        Returns:
+            str: A safe target name, based off the given one.
+        """
+        current_addition = ""
+        attempt_index = 2
+        while name + current_addition in self.data:
+            current_addition = "_{}".format(attempt_index)
+            attempt_index += 1
+        return name + current_addition
+
+    ############################################################################
+    # Data Namespace Management
+
+    def clear_data(self):
+        # Temporary data
+        self.data.clear()
+        self._temporary_variables.clear()
+        self._backup_variables.clear()
+        self._reset_builtins(self.data)
+
+    @staticmethod
+    def _reset_builtins(data: dict):
+        """
+        Replace all the existing given `data` with the builtin mocked data.
+        Args:
+            data:
+
+        Returns:
+
+        """
+        data['__builtins__'] = {}
+        for name, value in mocked._default_builtins.items():
+            data['__builtins__'][name] = value
+
+    def set_student_data(self, new_data):
+        """
+        Overwrites the existing student data with the keys and values from
+        the ``new_data``. This copies the data over, but does not modify the
+        reference to ``data``'s dictionary.
+
+        Args:
+            new_data (dict[str, Any]): The new data.
+
+        Returns:
+
+        """
+        self.clear_data()
+        for key, value in new_data.items():
+            self.data[key] = value
+
+    def get_names_by_type(self, type, exclude_builtins=True):
+        """
+
+        Args:
+            type:
+            exclude_builtins:
+
+        Returns:
+
+        """
+        result = []
+        for name, value in self.data.items():
+            if isinstance(value, type):
+                if exclude_builtins and name.startswith('__'):
+                    continue
+                result.append(name)
+        return result
+
+    def get_values_by_type(self, type, exclude_builtins=True):
+        """
+
+        Args:
+            type:
+            exclude_builtins:
+
+        Returns:
+
+        """
+        names = self.get_names_by_type(type, exclude_builtins)
+        return [self.data[name] for name in names]
+
+    def get_variables_by_type(self, type, exclude_builtins=True):
+        """
+
+        Args:
+            type:
+            exclude_builtins:
+
+        Returns:
+
+        """
+        names = self.get_names_by_type(type, exclude_builtins)
+        return [(name, self.data[name]) for name in names]
+
+    @property
+    def functions(self):
+        """
+        Retrieve a list of all the callable names in the students' namespace.
+        In other words, get a list of all the functions the student defined.
+
+        Returns:
+            list of callables
+        """
+        return {k: v for k, v in self.data.items() if callable(v)}
+
+    @property
+    def var(self):
+        """
+
+        Returns:
+
+        """
+        return {k: SandboxVariable(k, v) for k, v in self.data.items()}
+
+    def get_function(self, by_name):
+        """
+        Creates an executable function from the given name, based
+        on the student's namespace. This will be executed using the call
+        method.
+        """
+        return lambda *args, **kwargs: self.call(by_name, *args, **kwargs)
+
+    def __getitem__(self, item):
+        value, exception = None, None
+        try:
+            value = self.data[item]
+        except KeyError:
+            exception = NameError(f"NameError: name '{item}' is not defined")
+        filename = self.report.submission.instructor_file
+        context_id = self._next_context_id
+        best_context = self._guess_context(item)
+        if best_context is None:
+            context = SandboxContext(context_id, str(item), filename,
+                                     SandboxContextKind.GETITEM, item, [], "",
+                                     exception, self.report.submission)
+        else:
+            context = best_context.clone(context_id)
+            context.target = str(item)
+            context.exception = exception
+        self._context.append(context)
+        self._next_context_id += 1
+
+        if self.result_proxy_class is not None:
+            return self.result_proxy_class(value, context_id=context_id,
+                                           sandbox=self)
+        return value
+
+    ############################################################################
+    # Useful Dunders
+
+    # def __repr__(self):
+    #    return "Sandbox({})".format()
+
+    def __str__(self):
+        return "Sandbox(contexts={context_count})".format(context_count=len(self._context))
+
+    ############################################################################
+    # Input Handling
+
+    def clear_input(self):
+        """ Removes any inputs queued. """
+        self.set_input(None)
+        return self
+
+    def set_input(self, inputs, clear=True):
+        """
+        Queues the given value as the next arguments to the `input` function.
+        """
+        if inputs is None:
+            self.inputs = []
+        if clear:
+            self.inputs.clear()
+        if isinstance(inputs, str):
+            self.inputs.append(inputs)
+        elif isinstance(inputs, (int, float, bool)):
+            self.inputs.append(str(inputs))
+        elif isinstance(inputs, (list, tuple)):
+            self.inputs.extend([str(value) for value in inputs])
+        elif inputs is not None:
+            self.inputs = inputs
+        return self
+
+    def _track_inputs(self, context_inputs):
+        """
+        Wraps an input function with a tracker.
+        """
+        self._called_inputs = 0
+
+        def _input_tracker(*args, **kwargs):
+            if args:
+                prompt = args[0]
+            else:
+                prompt = ""
+            if callable(self.inputs):
+                value_entered = self.inputs(prompt)
+            elif self.inputs:
+                print(prompt)
+                value_entered = self.inputs.pop(0)
+            else:
+                # TODO: Make this smarter, more elegant in choosing IF we should repeat 0
+                print(prompt)
+                value_entered = '0'
+            self._context[-1].inputs.append(value_entered)
+            self._called_inputs += 1
+            if self.MAXIMUM_INPUTS is not None:
+                if self.MAXIMUM_INPUTS <= self._called_inputs:
+                    raise IOError(
+                        f"Asked for user input too many times ({self._called_inputs} times). Perhaps you have an infinite loop?")
+            # context_inputs.append(value_entered)
+            return value_entered
+
+        return _input_tracker
+
+    ############################################################################
+    # Output Handling
+
+    def clear_output(self):
+        """ Remove any output currently attached to this sandbox. """
+        # Update outputs
+        self.raw_output = ""
+        self.output.clear()
+        return self
+
+    def append_output(self, raw_output, context):
+        """
+        Adds the string of `raw_output` to the current `raw_output` attribute.
+        The added string will be split on newlines and rstripped to append
+        to the `output` attribute.
+
+        Args:
+            raw_output (str): The new raw_output for the sandbox. To compute
+                the `output` attribute, the system splits and rstrips at
+                newlines.
+            context (:py:class:`pedal.sandbox.data.SandboxContext`): The
+                currently executing context, where this output will be recorded.
+        """
+        self.raw_output += raw_output
+        context.output = raw_output
+        if self.raw_output:
+            lines = raw_output.rstrip().split("\n")
+            lines = [line.rstrip() for line in lines]
+            self.output.extend(lines)
+
+    def clear(self):
+        """ Removes any existing data in this sandbox. """
+        self.clear_data()
+        self.clear_context()
+        self.clear_mocks()
+        self.clear_exception()
+        self.clear_input()
+        self.clear_output()
+        self.clear_tracer()
```

### Comparing `pedal-2.6.1/pedal/sandbox/timeout.py` & `pedal-2.6.2/pedal/sandbox/timeout.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/sandbox/tracer.py` & `pedal-2.6.2/pedal/sandbox/tracer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/source/__init__.py` & `pedal-2.6.2/pedal/source/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/source/feedbacks.py` & `pedal-2.6.2/pedal/source/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/source/sections.py` & `pedal-2.6.2/pedal/source/sections.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/source/source.py` & `pedal-2.6.2/pedal/source/source.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/tifa/__init__.py` & `pedal-2.6.2/pedal/tifa/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/tifa/commands.py` & `pedal-2.6.2/pedal/tifa/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/tifa/contexts.py` & `pedal-2.6.2/pedal/tifa/contexts.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/tifa/feedbacks.py` & `pedal-2.6.2/pedal/tifa/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/tifa/identifier.py` & `pedal-2.6.2/pedal/tifa/identifier.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/tifa/settings.py` & `pedal-2.6.2/pedal/tifa/settings.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/tifa/state.py` & `pedal-2.6.2/pedal/tifa/state.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/tifa/tifa_core.py` & `pedal-2.6.2/pedal/tifa/tifa_core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/tifa/tifa_visitor.py` & `pedal-2.6.2/pedal/tifa/tifa_visitor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1175 +1,1176 @@
-
-"""
-Main TIFA visitor-based algorithm here.
-
-TODO: JoinedStr
-"""
-
-import ast
-# TODO: FileType, DayType, TimeType,
-from pedal.core.commands import system_error
-from pedal.tifa.tifa_core import TifaCore, TifaAnalysis
-from pedal.types.new_types import (Type, AnyType, ImpossibleType, FunctionType, GeneratorType,
-                                   IntType, FloatType, BoolType, TupleType,
-                                   ListType, StrType, SetType, DictType,
-                                   ClassType, InstanceType, BuiltinConstructorType, NumType, NoneType,
-                                   LiteralValue, LiteralInt, LiteralFloat, LiteralStr, LiteralBool,
-                                   TypeUnion, widen_type, widest_type)
-from pedal.types.new_types import is_subtype, specify_subtype
-from pedal.types.normalize import get_pedal_type_from_value
-from pedal.types.builtin import get_builtin_name
-from pedal.types.operations import (VALID_UNARYOP_TYPES, apply_binary_operation, apply_unary_operation)
-from pedal.tifa.constants import TOOL_NAME
-from pedal.tifa.contexts import NewPath, NewScope
-from pedal.tifa.feedbacks import (action_after_return, return_outside_function,
-                                  write_out_of_scope, unconnected_blocks,
-                                  iteration_problem, not_a_function,
-                                  initialization_problem, unused_variable,
-                                  overwritten_variable, iterating_over_non_list,
-                                  iterating_over_empty_list, incompatible_types,
-                                  parameter_type_mismatch, read_out_of_scope,
-                                  type_changes, unnecessary_second_branch,
-                                  recursive_call, multiple_return_types,
-                                  possible_initialization_problem,
-                                  incorrect_arity, else_on_loop_body,
-                                  module_not_found, nested_function_definition,
-                                  unused_returned_value, invalid_indexing,
-                                  attribute_type_change)
-from pedal.utilities.system import IS_AT_LEAST_PYTHON_38, IS_SKULPT
-
-
-class Tifa(TifaCore, ast.NodeVisitor):
-    """
-    TIFA subclass for traversing an AST and finding common issues.
-    You can instantiate this class, manipulate settings, and then process
-    some code or AST.
-    """
-
-    def process_code(self, code, filename=None, reset=True):
-        """
-        Processes the AST of the given source code to generate a report.
-
-        Args:
-            code (str): The Python source code
-            filename (str): The filename of the source code (defaults to
-                the submissions' main file).
-            reset (bool): Whether or not to reset the results from the
-                previous analysis before running this one.
-        Returns:
-            Report: The successful or successful report object
-        """
-        if reset or self.analysis is None:
-            self.analysis = TifaAnalysis()
-        filename = filename or (self.report.submission.main_file if self.report.submission else 'student.py')
-        self.line_offset = self.report.submission.line_offsets.get(filename, 0) if self.report.submission else 0
-
-        # Attempt parsing - might fail!
-        try:
-            ast_tree = ast.parse(code, filename)
-        except Exception as error:
-            self.analysis.fail(error)
-            system_error(TOOL_NAME, "Could not parse code: " + str(error),
-                         report=self.report)
-            return self.analysis
-        # Attempt processing code - might fail!
-        try:
-            self.process_ast(ast_tree)
-        except Exception as error:
-            self.analysis.fail(error)
-            system_error(TOOL_NAME, message="Successfully parsed but could not "
-                                    "process AST: " + str(error),
-                         report=self.report)
-        # Return whatever we got
-        return self.analysis
-
-    def process_ast(self, ast_tree):
-        """
-        Given an AST, actually performs the type and flow analyses to return a
-        report.
-
-        Args:
-            ast_tree (AST): The AST object
-        """
-        self.reset()
-        # Traverse every node
-        self.visit(ast_tree)
-
-        # Update analysis, finish out the current scope.
-        self.analysis.variables = self.name_map
-        self._finish_scope()
-
-        # Collect top level variables
-        self._collect_top_level_variables()
-
-        return self.analysis
-
-    def visit(self, node):
-        """
-        Process this node by calling its appropriate visit_*
-
-        Args:
-            node (AST): The node to visit
-        Returns:
-            Type: The type calculated during the visit.
-        """
-        # Start processing the node
-        self.node_chain.append(node)
-        self.ast_id += 1
-
-        # Actions after return?
-        if len(self.scope_chain) > 1:
-            return_state = self.find_variable_scope("*return")
-            if return_state.exists and return_state.in_scope:
-                if return_state.state.set == "yes":
-                    self._issue(action_after_return(self.locate(),
-                                                    report=self.report))
-
-        # No? All good, let's enter the node
-        self.final_node = node
-        result = ast.NodeVisitor.visit(self, node)
-        # If a node failed to return something, return the UNKNOWN TYPE
-        if result is None:
-            result = AnyType()
-        self.analysis.node_types[node] = result
-
-        # Pop the node out of the chain
-        self.ast_id -= 1
-        self.node_chain.pop()
-
-        return result
-
-    def _visit_nodes(self, nodes):
-        """
-        Visit all the nodes in the given list.
-
-        Args:
-            nodes (list): A list of values, of which any AST nodes will be
-                          visited.
-        """
-        for node in nodes:
-            if isinstance(node, ast.AST):
-                self.visit(node)
-
-    def _visit_collection_loop(self, node):
-        was_empty = False
-        # Handle the iteration list
-        iter_list = node.iter
-        iter_list_name = None
-        if isinstance(iter_list, ast.Name):
-            iter_list_name = iter_list.id
-            if iter_list_name == "___":
-                self._issue(unconnected_blocks(self.locate(iter_list), report=self.report))
-            state = self.iterate_variable(iter_list_name, self.locate(iter_list))
-            iter_type = state.type
-        else:
-            iter_type = self.visit(iter_list)
-
-        if iter_type.is_empty:
-            # TODO: It should check if its ONLY ever iterating over an empty list.
-            # For now, only reports if we are NOT in a function
-            was_empty = True
-            if len(self.scope_chain) == 1:
-                self._issue(iterating_over_empty_list(self.locate(iter_list), iter_list_name))
-
-        iter_subtype = iter_type.iterate()
-        if isinstance(iter_subtype, ImpossibleType):
-            self._issue(iterating_over_non_list(self.locate(iter_list), iter_list_name, report=self.report))
-
-
-        # Handle the iteration variable
-        self.assign_target(node.target, iter_subtype, store_with_read=True)
-
-        # Check that the iteration list and variable are distinct
-        if isinstance(node.target, ast.Name) and node.target.id == iter_list_name:
-            self._issue(iteration_problem(self.locate(node.target), node.target.id))
-
-        return was_empty
-
-    def break_starred(self, elements):
-        leading, starred, trailing = [], [], []
-        all_elements = iter(elements)
-        for elt in all_elements:
-            if isinstance(elt, ast.Starred):
-                starred.append(elt)
-                break
-            else:
-                leading.append(elt)
-        else:
-            return leading, starred, trailing
-        for elt in all_elements:
-            trailing.append(elt)
-        return leading, starred, trailing
-
-    # TODO: Properly handle assignments with subscripts
-    def assign_target(self, target, target_type, operation=None, store_with_read=False):
-        """
-        Assign the type to the target, handling all kinds of assignment
-        statements, including Names, Tuples/Lists, Subscripts, and
-        Attributes.
-
-        Args:
-            target (ast.AST): The target AST Node.
-            target_type (Type): The new TIFA type.
-            operation (None | ast.op): The AugAssign operation, if there is one
-            store_with_read: Whether to store the variable as a read variable, or just a write variable.
-
-        Returns:
-
-        """
-        if isinstance(target, ast.Name):
-            original_value_type = self.visit(target)
-            if operation:
-                new_target_type = apply_binary_operation(operation, original_value_type, target_type)
-                if isinstance(new_target_type, ImpossibleType):
-                    self._issue(incompatible_types(self.locate(), operation, original_value_type, target_type, report=self.report))
-            else:
-                new_target_type = target_type
-            if store_with_read:
-                self.store_read_variable(target.id, new_target_type)
-            else:
-                self.store_variable(target.id, new_target_type)
-        elif isinstance(target, (ast.Tuple, ast.List)):
-            original_type = self.visit(target)
-            leading, starred, trailing = self.break_starred(target.elts)
-            tt, ot = target_type.break_apart(), original_type.break_apart()
-            for elt, elt_type, old_type in zip(leading, tt, ot):
-                self.assign_target(elt, elt_type)
-            if starred:
-                # TODO: Handle starred node's type changes
-                # if not is_subtype(target_type, old_type):
-                    # self._issue(type_changes(self.locate(), 'an element of NODE', old_type.singular_name, elt_type.singular_name))
-                self.assign_target(starred[0], target_type)
-                for elt, elt_type, old_type in zip(trailing, tt, ot):
-                    # BUG: Any trailing elements will be incorrectly offset, so won't work with finite length stuff
-                    self.assign_target(elt, elt_type)
-        elif isinstance(target, ast.Subscript):
-            original_value_type = self.visit(target.value)
-            origin = self.identify_caller(target.value)
-            original_indexing_type = self.visit(target.slice)
-            original_type = original_value_type.index(original_indexing_type)
-            if operation:
-                new_target_type = apply_binary_operation(operation, original_type, target_type)
-                if isinstance(new_target_type, ImpossibleType):
-                    self._issue(incompatible_types(self.locate(), operation, original_type, target_type, report=self.report))
-            else:
-                new_target_type = target_type
-            original_type.set_index(original_indexing_type, new_target_type)
-            if origin:
-                origin_type = self.load_variable(origin)
-                self.store_variable(origin, origin_type.type)
-        elif isinstance(target, ast.Attribute):
-            original_type = self.visit(target.value)
-            origin = self.identify_caller(target.value)
-            if operation:
-                new_target_type = apply_binary_operation(operation, original_type, target_type)
-                if isinstance(new_target_type, ImpossibleType):
-                    self._issue(incompatible_types(self.locate(), operation, original_type, target_type, report=self.report))
-            else:
-                new_target_type = target_type
-            assigned_type = original_type.add_attr(target.attr, new_target_type)
-            if isinstance(assigned_type, ImpossibleType):
-                self._issue(attribute_type_change(self.locate(), target.attr, original_type, new_target_type, report=self.report))
-            if origin:
-                origin_type = self.load_variable(origin)
-                if origin_type:
-                    self.store_variable(origin, origin_type.type)
-
-    def visit_AnnAssign(self, node):
-        """
-
-        Args:
-            node (ast.AnnAssign):
-
-        Returns:
-
-        """
-        # Name, Attribute, or SubScript
-        target = node.target
-        # Type
-        annotation = node.annotation
-        annotation_type = self.evaluate_type(annotation)
-        was_class_attribute = False
-        # Optional assigned value
-        value = node.value
-        # 0 or 1, with 1 indicating pure names (not expressions)
-        simple = node.simple
-
-        # If it's a class attribute, then build up the type!
-        if simple:
-            current_scope = self.scope_chain[0]
-            if current_scope in self.class_scopes:
-                self.class_scopes[current_scope].add_attr(target.id, annotation)
-                was_class_attribute = True
-        # TODO: Allow setting for optional type coercion, or throw error
-        if value:
-            self.visit(value)
-            # self.assign_target(target, self.visit(value))
-        # Make local variable either way
-        self.assign_target(target, annotation_type, store_with_read=was_class_attribute)
-
-    def visit_Assign(self, node):
-        """
-        Simple assignment statement:
-        __targets__ = __value__
-
-        Args:
-            node (ast.Assign): An Assign node
-        Returns:
-            None
-        """
-        # Handle value
-        value_type = self.visit(node.value)
-        # Apply value to all targets
-        for target in node.targets:
-            self.assign_target(target, value_type)
-
-    def visit_AugAssign(self, node):
-        """
-
-        Args:
-            node (ast.AugAssign):
-
-        Returns:
-
-        """
-        # Handle value
-        right = self.visit(node.value)
-        if isinstance(node.target, ast.Name):
-            self.load_variable(self.identify_caller(node.target))
-        self.assign_target(node.target, right, node.op)
-
-    def visit_Attribute(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        # Handle value
-        value_type = self.visit(node.value)
-        self.check_common_bad_lookups(value_type, node.attr, node.value)
-        # Handle attr
-        result = value_type.get_attr(node.attr)
-        # Set up self if this was a function (because now it's a method!)
-        # TODO: Handle static/class functions differently I guess?
-        if isinstance(result, FunctionType):
-            result = result.as_method(value_type)
-        return result
-
-    def visit_BinOp(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        # Handle left and right
-        left = self.visit(node.left)
-        right = self.visit(node.right)
-        operation = node.op
-
-        new_target_type = apply_binary_operation(operation, left, right)
-        if isinstance(new_target_type, ImpossibleType):
-            self._issue(incompatible_types(self.locate(), operation, left, right, report=self.report))
-        return new_target_type
-
-    def visit_Bool(self, node):
-        """
-        Visit a constant boolean value.
-
-        Args:
-            node (ast.AST): The boolean value Node.
-
-        Returns:
-            Type: A Bool type.
-        """
-        return BoolType()
-
-    def visit_BoolOp(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        # Handle left and right
-        values = [self.visit(value) for value in node.values]
-        # Handle operation
-        # Actually, the operations are always the same behavior!
-        # Handle truthiness
-        if self.get_setting('truthiness_returns_booleans'):
-            return BoolType()
-        elif not values:
-            return ImpossibleType()
-        # All same type? Then return the first one!
-        elif all(is_subtype(values[0], other) for other in values[1:]):
-            return values[0]
-        # Oh no, type union is necessary!
-        else:
-            return TypeUnion(values)
-
-    def load_root_variable(self, node, position=None):
-        root_name = self.identify_caller(node)
-        if root_name is not None:
-            variable = self.find_variable_scope(root_name)
-            if variable.exists:
-                return variable.state
-        return None
-
-    def visit_Call(self, node):
-        # Handle func part
-        function_type = self.visit(node.func)
-        # TODO: Need to grab the actual type in some situations
-        original_callee = self.load_root_variable(node)
-
-        # Handle args
-        arguments = [self.visit(arg) for arg in node.args] if node.args else []
-        keywords = [(kwarg.arg, self.visit(kwarg.value))
-                    for kwarg in node.keywords] if node.keywords else {}
-
-        # Check special common mistakes
-
-        if isinstance(function_type, BuiltinConstructorType):
-            constructor = function_type.definition
-            return constructor(self, function_type, original_callee,
-                               arguments, keywords, self.locate())
-        if isinstance(function_type, FunctionType):
-            # Test if we have called this definition before
-            if function_type.definition not in self.definition_chain:
-                self.definition_chain.append(function_type.definition)
-                # Function invocation
-                result = function_type.definition(self, function_type, original_callee,
-                                                  arguments, keywords, self.locate())
-                self.definition_chain.pop()
-                return result
-            else:
-                self._issue(recursive_call(self.locate(), original_callee, report=self.report))
-        elif isinstance(function_type, ClassType):
-            constructor = function_type.get_constructor().definition
-            self.definition_chain.append(constructor)
-            new_instance = constructor(self, constructor, original_callee, arguments, keywords, self.locate())
-            self.definition_chain.pop()
-            if '__init__' in function_type.fields:
-                initializer = function_type.fields['__init__'].as_method(new_instance)
-                if isinstance(initializer, FunctionType):
-                    self.definition_chain.append(initializer)
-                    initializer.definition(self, initializer, new_instance, [new_instance] + arguments, keywords, self.locate())
-                    self.definition_chain.pop()
-            return new_instance
-        elif isinstance(function_type, (IntType, FloatType, NumType, ListType,
-                                        DictType, SetType, TupleType, InstanceType,
-                                        StrType, BoolType, NoneType, LiteralValue)):
-            if original_callee is None:
-                self._issue(not_a_function(self.locate(), "a value", function_type, report=self.report))
-            else:
-                self._issue(not_a_function(self.locate(), original_callee.name, function_type, report=self.report))
-            return ImpossibleType()
-        return AnyType()
-
-    def visit_ClassDef(self, node):
-        """
-
-        Args:
-            node:
-        """
-        class_name = node.name
-        parents = [self.visit(base) for base in node.bases]
-        new_class_type = ClassType(class_name, {}, parents)
-        self.store_variable(class_name, new_class_type)
-        definitions_scope = self.scope_chain[:]
-        class_scope = NewScope(self, definitions_scope, class_type=new_class_type)
-        # TODO: Handle metaclass... somehow?
-        #self._visit_nodes(node.keywords)
-        with class_scope:
-            self._visit_nodes(node.body)
-        new_class_type = self.apply_decorators(class_name, new_class_type, node.decorator_list)
-        return new_class_type
-
-    def apply_decorators(self, new_name, new_type, decorators):
-        for decorator in reversed(decorators):
-            old_type = self.load_variable(new_name)
-            decorator_type = self.visit(decorator)
-            original_callee = self.load_root_variable(decorator)
-            new_type = decorator_type.definition(self, decorator_type, original_callee,
-                                                 [new_type], {}, self.locate())
-            self.store_variable(new_name, new_type)
-        return new_type
-
-    def visit_Compare(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        # Handle left and right
-        left = self.visit(node.left)
-        comparators = [self.visit(compare) for compare in node.comparators]
-
-        # Handle ops
-        for op, right in zip(node.ops, comparators):
-            if isinstance(op, (ast.Eq, ast.NotEq, ast.Is, ast.IsNot)):
-                continue
-            elif isinstance(op, (ast.Lt, ast.LtE, ast.GtE, ast.Gt)):
-                if type(right) in left.orderable:
-                    continue
-            elif isinstance(op, (ast.In, ast.NotIn)):
-                if right.allows_membership(left):
-                    continue
-            self._issue(incompatible_types(self.locate(), op, left, right, report=self.report))
-        return BoolType()
-
-    def visit_comprehension(self, node):
-        """
-
-        Args:
-            node:
-        """
-        self.fill_in_location(node, self.node_chain[-2])
-        self._visit_collection_loop(node)
-        # Handle ifs, unless they're blank (None in Skulpt :)
-        if node.ifs:
-            self.visit_statements(node.ifs)
-
-    def fill_in_location(self, node, source_node):
-        node.lineno = source_node.lineno
-        node.col_offset = source_node.col_offset
-        if IS_AT_LEAST_PYTHON_38:
-            node.end_lineno = source_node.end_lineno
-            node.end_col_offset = source_node.end_col_offset
-        else:
-            node.end_lineno = source_node.lineno
-            node.end_col_offset = source_node.col_offset
-
-    def visit_Dict(self, node):
-        """
-        Three types of dictionaries
-        - empty
-        - uniform type
-        - record
-        TODO: Handle records appropriately
-        """
-        items = [(self.visit(key), self.visit(value))
-                 for key, value in zip(node.keys, node.values) if key is not None]
-        # Unpack starred dictionaries
-        for key, value in zip(node.keys, node.values):
-            if key is None:
-                value_type = self.visit(value)
-                if isinstance(value_type, DictType):
-                    items.extend([
-                        (k, v) for k, v in value_type.element_types
-                    ])
-        # Empty dictionary
-        if not items:
-            return DictType([])
-        # All literal keys
-        if all(isinstance(k, LiteralValue) for k, _ in items):
-            return DictType([(k, v) for k, v in items])
-        # Find if all matched type
-        first_key = widest_type([key for key, value in items])
-        first_value = widest_type([value for key, value in items])
-        if first_key is not None and first_value is not None:
-            return DictType([(first_key, first_value)])
-        else:
-            # Resort to just matching the types?
-            return DictType([(k, v) for k, v in items])
-
-    def visit_DictComp(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        generator_scope = NewScope(self, self.scope_chain[:])
-        with generator_scope:
-            self._visit_nodes(node.generators)
-            keys = self.visit(node.key)
-            values = self.visit(node.value)
-            return DictType([(keys, values)])
-
-    def visit_Expr(self, node):
-        """
-        Any expression being used as a statement.
-
-        Args:
-            node (AST): An Expr node
-
-        Returns:
-
-        """
-        value = self.visit(node.value)
-        if isinstance(node.value, ast.Call) and not isinstance(value, NoneType):
-            # TODO: Helper function to get name with title ("append method")
-            if isinstance(node.value.func, ast.Name):
-                call_type = 'function'
-            else:
-                call_type = 'method'
-            name = self.identify_caller(node.value)
-            self._issue(unused_returned_value(self.locate(), name,
-                                              call_type, value))
-
-    def visit_For(self, node):
-        """
-
-        Args:
-            node:
-        """
-        was_empty = self._visit_collection_loop(node)
-        # Handle the bodies
-        # if not was_empty:
-        # this_path_id = self.path_chain[0]
-        # non_empty_path = NewPath(self, this_path_id, "f")
-        # with non_empty_path:
-        self.visit_statements(node.body)
-        self.visit_statements(node.orelse)
-
-    def visit_FunctionDef(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        function_name = node.name
-        position = self.locate()
-        definitions_scope = self.scope_chain[:]
-        definition = self.make_function(function_name, definitions_scope, position, node)
-        function = FunctionType(function_name, definition=definition)
-        self.store_variable(function_name, function)
-
-        if len(self.node_chain) > 2:
-            self._issue(nested_function_definition(self.locate(), function_name))
-
-        return self.apply_decorators(function_name, function, node.decorator_list)
-
-    def make_function(self, function_name, definitions_scope, position, node):
-        is_lambda = function_name is None
-
-        class SkipType:
-            pass
-        # Pull apart args into a coherent set of data PRIOR to execution
-        args = node.args
-        pos_parameters = args.posonlyargs + args.args if IS_AT_LEAST_PYTHON_38 and not IS_SKULPT else args.args
-        none_padding = [SkipType] * (len(pos_parameters) - len(args.defaults))
-        pos_defaults = none_padding + [self.visit(d) for d in args.defaults]
-        kwarg_parameter = args.kwarg
-        vararg_parameter = args.vararg
-
-        # TODO: Finish kwargs
-        named_parameters = args.kwonlyargs
-        named_defaults = [self.visit(d) if d is not None else AnyType() for d in args.kw_defaults]
-        expected_returns = self.evaluate_type(node.returns) if not is_lambda and node.returns else None
-
-        def definition(tifa, function, callee_name, arguments, named_arguments, call_position):
-            function_scope = NewScope(self, definitions_scope)
-            with function_scope:
-                # Process arguments
-                if len(arguments) + len(named_arguments) != len(pos_parameters) and not vararg_parameter:
-                    self._issue(incorrect_arity(self.locate(), function_name,
-                                                len(pos_parameters), len(arguments), report=self.report))
-                for parameter, default, argument in zip(pos_parameters, pos_defaults, arguments):
-                    parameter_name = parameter.arg
-                    if parameter.annotation:
-                        annotation = self.evaluate_type(parameter.annotation)
-                        if is_subtype(argument, annotation):
-                            specify_subtype(annotation, argument)
-                        else:
-                            self._issue(parameter_type_mismatch(self.locate(), parameter_name,
-                                                                annotation, argument))
-                    elif default is not SkipType:
-                        if is_subtype(argument, default):
-                            specify_subtype(default, argument)
-                        else:
-                            self._issue(parameter_type_mismatch(self.locate(), parameter_name,
-                                                                default, argument))
-                    if argument is not None:
-                        argument_type = argument.clone_mutably()
-                        self.create_variable(parameter_name, argument_type, position)
-                # Too many arguments
-                if len(pos_parameters) < len(arguments):
-                    if vararg_parameter:
-                        the_rest = arguments[len(pos_parameters):]
-                        self.create_variable(vararg_parameter.arg, TupleType(the_rest), position)
-                # Not enough arguments
-                if len(pos_parameters) > len(arguments):
-                    for parameter in pos_parameters[len(arguments):]:
-                        if parameter.annotation:
-                            annotation = self.evaluate_type(parameter.annotation)
-                        else:
-                            annotation = AnyType()
-                        self.create_variable(parameter.arg, annotation, position)
-                if is_lambda:
-                    return self.visit(node.body)
-
-                self.visit_statements(node.body)
-                return_state = self.find_variable_scope("*return")
-                return_value = NoneType()
-                # TODO: Figure out if we are not returning something when we should
-                # If the pseudo variable exists, we load it and get its type
-                if return_state.exists and return_state.in_scope:
-                    return_state = self.load_variable("*return", call_position)
-                    return_value = return_state.type
-                    if expected_returns:
-                        if not is_subtype(return_value, expected_returns):
-                            self._issue(multiple_return_types(return_state.position,
-                                                              expected_returns.singular_name,
-                                                              return_value.singular_name,
-                                                              report=self.report))
-            return return_value
-        return definition
-
-    def evaluate_type(self, node):
-        string_literal = False
-        if isinstance(node, ast.Str):
-            string_literal = node.s
-        elif isinstance(node, ast.Constant) and isinstance(node.value, str):
-            string_literal = node.value
-        if string_literal is not False:
-            if self.get_setting('evaluate_string_literal_types'):
-                # TODO: Handle string literal types properly!
-                pass
-            else:
-                return LiteralStr(string_literal)
-        elif isinstance(node, ast.List):
-            if node.elts:
-                return ListType(False, self.evaluate_type(node.elts[0]))
-            else:
-                return ListType(True)
-        elif isinstance(node, ast.Set) and node.elts:
-            return TypeUnion([self.evaluate_type(e) for e in node.elts])
-        elif isinstance(node, ast.Tuple) and node.elts:
-            return TupleType([self.evaluate_type(e) for e in node.elts])
-        elif isinstance(node, ast.Dict):
-            if node.keys and node.values:
-                return DictType([(self.evaluate_type(k), self.evaluate_type(v))
-                                 for k, v in zip(node.keys, node.values)])
-            else:
-                return DictType([])
-        else:
-            evaluated = self.visit(node)
-            return evaluated.as_type(self, self.locate(node))
-
-    def visit_GeneratorExp(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        generator_scope = NewScope(self, self.scope_chain[:])
-        with generator_scope:
-            self._visit_nodes(node.generators)
-            return GeneratorType(False, self.visit(node.elt))
-
-    def visit_If(self, node):
-        """
-
-        Args:
-            node:
-        """
-        # Visit the conditional
-        self.visit(node.test)
-
-        if len(node.orelse) == 1 and isinstance(node.orelse[0], ast.Pass):
-            self._issue(unnecessary_second_branch(self.locate()))
-        elif len(node.body) == 1 and isinstance(node.body[0], ast.Pass):
-            if node.orelse:
-                self._issue(unnecessary_second_branch(self.locate()))
-
-        # Visit the bodies
-        this_path_id = self.path_chain[0]
-        if_path = NewPath(self, this_path_id, "i")
-        with if_path:
-            for statement in node.body:
-                self.visit(statement)
-        else_path = NewPath(self, this_path_id, "e")
-        with else_path:
-            for statement in node.orelse:
-                self.visit(statement)
-
-        # TODO: Unconditional return
-
-        # Combine two paths into one
-        # Check for any names that are on the IF path
-        self.merge_paths(this_path_id, if_path.id, else_path.id)
-
-    def visit_IfExp(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        # Visit the conditional
-        self.visit(node.test)
-
-        # Visit the body
-        body = self.visit(node.body)
-
-        # Visit the orelse
-        orelse = self.visit(node.orelse)
-
-        if is_subtype(body, orelse):
-            return body
-
-        # TODO: Union type?
-        return TypeUnion([body, orelse])
-
-    def visit_Import(self, node):
-        """
-
-        Args:
-            node:
-        """
-        # Handle names
-        for alias in node.names:
-            asname = alias.asname or alias.name
-            module_type = self.load_module(alias.name)
-            self.store_variable(asname, module_type)
-
-    def visit_ImportFrom(self, node):
-        """
-
-        Args:
-            node:
-        """
-        # Handle names
-        for alias in node.names:
-            if alias.name == '*':
-                module_type = self.load_module(node.module)
-                for field, value in module_type.fields.items():
-                    self.store_read_variable(field, value)
-            else:
-                if node.module is None:
-                    asname = alias.asname or alias.name
-                    module_type = self.load_module(alias.name)
-                else:
-                    module_name = node.module
-                    asname = alias.asname or alias.name
-                    module_type = self.load_module(module_name)
-                name_type = module_type.get_attr(alias.name)
-                self.store_variable(asname, name_type)
-
-    def visit_Lambda(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        position = self.locate()
-        definitions_scope = self.scope_chain[:]
-        definition = self.make_function(None, definitions_scope, position, node)
-        return FunctionType("*lambda", definition=definition)
-
-    def visit_List(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        if not node.elts:
-            return ListType(True)
-
-        # All literal keys
-        elements = [self.visit(v) for v in node.elts]
-        if all(isinstance(v, LiteralValue) for v in elements):
-            # TODO: Allow type union instead?
-            return ListType(False, elements[0].promote())
-        # Find if all matched type
-        first_value = widest_type(elements)
-        if first_value is not None:
-            return ListType(False, first_value)
-        else:
-            # Resort to just matching the types?
-            return ListType(False, TypeUnion(elements))
-
-    def visit_ListComp(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        # TODO: Handle comprehension scope
-        generator_scope = NewScope(self, self.scope_chain[:])
-        with generator_scope:
-            self._visit_nodes(node.generators)
-            return ListType(False, self.visit(node.elt))
-
-    def visit_NameConstant(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        value = node.value
-        if isinstance(value, bool):
-            return LiteralBool(value)
-        else:
-            return NoneType()
-
-    def visit_Name(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        name = node.id
-        if name == "___":
-            self._issue(unconnected_blocks(self.locate()))
-        if isinstance(node.ctx, ast.Load):
-            if name == "True" or name == "False":
-                return LiteralBool(name == "True")
-            elif name == "None":
-                return NoneType()
-            else:
-                variable = self.find_variable_scope(name)
-                builtin = get_builtin_name(name)
-                if not variable.exists and builtin:
-                    return builtin
-                else:
-                    state = self.load_variable(name)
-                    return state.type
-        else:
-            variable = self.find_variable_scope(name)
-            if variable.exists:
-                return variable.state.type
-            else:
-                return AnyType()
-
-    def visit_Num(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        return LiteralInt(node.n) if isinstance(node.n, int) else LiteralFloat(node.n)
-
-    def visit_Constant(self, node) -> Type:
-        """ Handle new 3.8's Constant node """
-        return get_pedal_type_from_value(node.value, self.evaluate_type)
-
-    def visit_Return(self, node):
-        """
-
-        Args:
-            node:
-        """
-        if len(self.scope_chain) == 1:
-            self._issue(return_outside_function(self.locate(), report=self.report))
-        # TODO: Unconditional return inside loop
-        if node.value is not None:
-            self.return_variable(self.visit(node.value))
-        else:
-            self.return_variable(NoneType())
-
-    def visit_Set(self, node):
-        # Fun fact, it's impossible to make a literal empty set
-        if not node.elts:
-            return SetType(True)
-
-        # All literal keys
-        elements = [self.visit(v) for v in node.elts]
-        if all(isinstance(v, LiteralValue) for v in elements):
-            # TODO: Allow type union instead?
-            return SetType(False, elements[0].promote())
-        # Find if all matched type
-        first_value = widest_type(elements)
-        if first_value is not None:
-            return SetType(False, first_value)
-        else:
-            # Resort to just matching the types?
-            return SetType(False, TypeUnion(elements))
-
-    def visit_SetComp(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        # TODO: Handle comprehension scope
-        generator_scope = NewScope(self, self.scope_chain[:])
-        with generator_scope:
-            self._visit_nodes(node.generators)
-            return SetType(False, self.visit(node.elt))
-
-    def visit_statements(self, nodes):
-        """
-
-        Args:
-            nodes:
-
-        Returns:
-
-        """
-        # TODO: Check for pass in the middle of a series of statement
-        if any(isinstance(node, ast.Pass) for node in nodes):
-            pass
-        return [self.visit(statement) for statement in nodes]
-
-    def visit_Str(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        return LiteralStr(node.s)
-
-    def visit_JoinedStr(self, node):
-        values = [self.visit(expr) for expr in node.values]
-        # The result will be all StrType
-        return StrType(is_empty=all(isinstance(n, (StrType, LiteralStr)) and n.is_empty
-                                    for n in values))
-
-    def visit_FormattedValue(self, node):
-        value = self.visit(node.value)
-        if isinstance(value, StrType):
-            return value
-        else:
-            return StrType(is_empty=False)
-
-    def visit_Subscript(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        # Handle value
-        value_type = self.visit(node.value)
-        slice_type = self.visit(node.slice)
-        result = value_type.index(slice_type)
-        if isinstance(result, ImpossibleType):
-            self._issue(invalid_indexing(self.locate(), value_type, slice_type))
-        if isinstance(node.slice, ast.Slice):
-            return value_type.shallow_clone()
-        else:
-            return result
-
-    def visit_Slice(self, node):
-        """ Handles a slice by visiting its components; cannot return a value
-        because the slice is always the same type as its value, which is
-        not available on the Slice node itself. """
-        if node.lower is not None:
-            self.visit(node.lower)
-        if node.upper is not None:
-            self.visit(node.upper)
-        if node.step is not None:
-            self.visit(node.step)
-
-    def visit_Index(self, node):
-        return self.visit(node.value)
-
-    def visit_ExtSlice(self, node):
-        return TupleType([self.visit(d) for d in node.dims])
-
-    def visit_Starred(self, node):
-        return self.visit(node.value).break_apart()
-
-    def visit_Tuple(self, node) -> TupleType:
-        # Fun fact, it's impossible to make a literal empty set
-        if not node.elts:
-            return TupleType(True)
-
-        # All literal keys
-        return TupleType([self.visit(v) for v in node.elts])
-
-    def visit_UnaryOp(self, node):
-        """
-
-        Args:
-            node:
-
-        Returns:
-
-        """
-        # Handle operand
-        operand_type = self.visit(node.operand)
-        return apply_unary_operation(node.op, operand_type)
-
-    def visit_While(self, node):
-        """
-
-        Args:
-            node:
-        """
-        # Visit conditional
-        self.visit(node.test)
-
-        # Visit the bodies
-        this_path_id = self.path_id
-        # One path is that we never enter the body
-        empty_path = NewPath(self, this_path_id, "e")
-        with empty_path:
-            pass
-        # Another path is that we loop through the body and check the test again
-        body_path = NewPath(self, this_path_id, "w")
-        with body_path:
-            for statement in node.body:
-                self.visit(statement)
-            # Revisit conditional
-            self.visit(node.test)
-        # If there's else bodies (WEIRD) then we should check them afterwards
-        if node.orelse:
-            self._issue(else_on_loop_body(self.locate()))
-            for statement in node.orelse:
-                self.visit(statement)
-
-        # Combine two paths into one
-        # Check for any names that are on the IF path
-        self.merge_paths(this_path_id, body_path.id, empty_path.id)
-
-    def visit_With(self, node):
-        """
-
-        Args:
-            node:
-        """
-        for item in node.items:
-            type_value = self.visit(item.context_expr)
-            if item.optional_vars is not None:
-                self.assign_target(item.optional_vars, type_value)
-        # Handle the bodies
-        self.visit_statements(node.body)
+
+"""
+Main TIFA visitor-based algorithm here.
+
+TODO: JoinedStr
+"""
+
+import ast
+# TODO: FileType, DayType, TimeType,
+from pedal.core.commands import system_error
+from pedal.tifa.tifa_core import TifaCore, TifaAnalysis
+from pedal.types.new_types import (Type, AnyType, ImpossibleType, FunctionType, GeneratorType,
+                                   IntType, FloatType, BoolType, TupleType,
+                                   ListType, StrType, SetType, DictType,
+                                   ClassType, InstanceType, BuiltinConstructorType, NumType, NoneType,
+                                   LiteralValue, LiteralInt, LiteralFloat, LiteralStr, LiteralBool,
+                                   TypeUnion, widen_type, widest_type)
+from pedal.types.new_types import is_subtype, specify_subtype
+from pedal.types.normalize import get_pedal_type_from_value
+from pedal.types.builtin import get_builtin_name
+from pedal.types.operations import (VALID_UNARYOP_TYPES, apply_binary_operation, apply_unary_operation)
+from pedal.tifa.constants import TOOL_NAME
+from pedal.tifa.contexts import NewPath, NewScope
+from pedal.tifa.feedbacks import (action_after_return, return_outside_function,
+                                  write_out_of_scope, unconnected_blocks,
+                                  iteration_problem, not_a_function,
+                                  initialization_problem, unused_variable,
+                                  overwritten_variable, iterating_over_non_list,
+                                  iterating_over_empty_list, incompatible_types,
+                                  parameter_type_mismatch, read_out_of_scope,
+                                  type_changes, unnecessary_second_branch,
+                                  recursive_call, multiple_return_types,
+                                  possible_initialization_problem,
+                                  incorrect_arity, else_on_loop_body,
+                                  module_not_found, nested_function_definition,
+                                  unused_returned_value, invalid_indexing,
+                                  attribute_type_change)
+from pedal.utilities.system import IS_AT_LEAST_PYTHON_38, IS_SKULPT
+
+
+class Tifa(TifaCore, ast.NodeVisitor):
+    """
+    TIFA subclass for traversing an AST and finding common issues.
+    You can instantiate this class, manipulate settings, and then process
+    some code or AST.
+    """
+
+    def process_code(self, code, filename=None, reset=True):
+        """
+        Processes the AST of the given source code to generate a report.
+
+        Args:
+            code (str): The Python source code
+            filename (str): The filename of the source code (defaults to
+                the submissions' main file).
+            reset (bool): Whether or not to reset the results from the
+                previous analysis before running this one.
+        Returns:
+            Report: The successful or successful report object
+        """
+        if reset or self.analysis is None:
+            self.analysis = TifaAnalysis()
+        filename = filename or (self.report.submission.main_file if self.report.submission else 'student.py')
+        self.line_offset = self.report.submission.line_offsets.get(filename, 0) if self.report.submission else 0
+
+        # Attempt parsing - might fail!
+        try:
+            ast_tree = ast.parse(code, filename)
+        except Exception as error:
+            self.analysis.fail(error)
+            system_error(TOOL_NAME, "Could not parse code: " + str(error),
+                         report=self.report)
+            return self.analysis
+        # Attempt processing code - might fail!
+        try:
+            self.process_ast(ast_tree)
+        except Exception as error:
+            self.analysis.fail(error)
+            system_error(TOOL_NAME, message="Successfully parsed but could not "
+                                    "process AST: " + str(error),
+                         report=self.report)
+        # Return whatever we got
+        return self.analysis
+
+    def process_ast(self, ast_tree):
+        """
+        Given an AST, actually performs the type and flow analyses to return a
+        report.
+
+        Args:
+            ast_tree (AST): The AST object
+        """
+        self.reset()
+        # Traverse every node
+        self.visit(ast_tree)
+
+        # Update analysis, finish out the current scope.
+        self.analysis.variables = self.name_map
+        self._finish_scope()
+
+        # Collect top level variables
+        self._collect_top_level_variables()
+
+        return self.analysis
+
+    def visit(self, node):
+        """
+        Process this node by calling its appropriate visit_*
+
+        Args:
+            node (AST): The node to visit
+        Returns:
+            Type: The type calculated during the visit.
+        """
+        # Start processing the node
+        self.node_chain.append(node)
+        self.ast_id += 1
+
+        # Actions after return?
+        if len(self.scope_chain) > 1:
+            return_state = self.find_variable_scope("*return")
+            if return_state.exists and return_state.in_scope:
+                if return_state.state.set == "yes":
+                    self._issue(action_after_return(self.locate(),
+                                                    report=self.report))
+
+        # No? All good, let's enter the node
+        self.final_node = node
+        result = ast.NodeVisitor.visit(self, node)
+        # If a node failed to return something, return the UNKNOWN TYPE
+        if result is None:
+            result = AnyType()
+        self.analysis.node_types[node] = result
+
+        # Pop the node out of the chain
+        self.ast_id -= 1
+        self.node_chain.pop()
+
+        return result
+
+    def _visit_nodes(self, nodes):
+        """
+        Visit all the nodes in the given list.
+
+        Args:
+            nodes (list): A list of values, of which any AST nodes will be
+                          visited.
+        """
+        for node in nodes:
+            if isinstance(node, ast.AST):
+                self.visit(node)
+
+    def _visit_collection_loop(self, node):
+        was_empty = False
+        # Handle the iteration list
+        iter_list = node.iter
+        iter_list_name = None
+        if isinstance(iter_list, ast.Name):
+            iter_list_name = iter_list.id
+            if iter_list_name == "___":
+                self._issue(unconnected_blocks(self.locate(iter_list), report=self.report))
+            state = self.iterate_variable(iter_list_name, self.locate(iter_list))
+            iter_type = state.type
+        else:
+            iter_type = self.visit(iter_list)
+
+        if iter_type.is_empty:
+            # TODO: It should check if its ONLY ever iterating over an empty list.
+            # For now, only reports if we are NOT in a function
+            was_empty = True
+            if len(self.scope_chain) == 1:
+                self._issue(iterating_over_empty_list(self.locate(iter_list), iter_list_name))
+
+        iter_subtype = iter_type.iterate()
+        if isinstance(iter_subtype, ImpossibleType):
+            self._issue(iterating_over_non_list(self.locate(iter_list), iter_list_name, report=self.report))
+
+
+        # Handle the iteration variable
+        self.assign_target(node.target, iter_subtype, store_with_read=True)
+
+        # Check that the iteration list and variable are distinct
+        if isinstance(node.target, ast.Name) and node.target.id == iter_list_name:
+            self._issue(iteration_problem(self.locate(node.target), node.target.id))
+
+        return was_empty
+
+    def break_starred(self, elements):
+        leading, starred, trailing = [], [], []
+        all_elements = iter(elements)
+        for elt in all_elements:
+            if isinstance(elt, ast.Starred):
+                starred.append(elt)
+                break
+            else:
+                leading.append(elt)
+        else:
+            return leading, starred, trailing
+        for elt in all_elements:
+            trailing.append(elt)
+        return leading, starred, trailing
+
+    # TODO: Properly handle assignments with subscripts
+    def assign_target(self, target, target_type, operation=None, store_with_read=False):
+        """
+        Assign the type to the target, handling all kinds of assignment
+        statements, including Names, Tuples/Lists, Subscripts, and
+        Attributes.
+
+        Args:
+            target (ast.AST): The target AST Node.
+            target_type (Type): The new TIFA type.
+            operation (None | ast.op): The AugAssign operation, if there is one
+            store_with_read: Whether to store the variable as a read variable, or just a write variable.
+
+        Returns:
+
+        """
+        if isinstance(target, ast.Name):
+            original_value_type = self.visit(target)
+            if operation:
+                new_target_type = apply_binary_operation(operation, original_value_type, target_type)
+                if isinstance(new_target_type, ImpossibleType):
+                    self._issue(incompatible_types(self.locate(), operation, original_value_type, target_type, report=self.report))
+            else:
+                new_target_type = target_type
+            if store_with_read:
+                self.store_read_variable(target.id, new_target_type)
+            else:
+                self.store_variable(target.id, new_target_type)
+        elif isinstance(target, (ast.Tuple, ast.List)):
+            original_type = self.visit(target)
+            leading, starred, trailing = self.break_starred(target.elts)
+            tt, ot = target_type.break_apart(), original_type.break_apart()
+            for elt, elt_type, old_type in zip(leading, tt, ot):
+                self.assign_target(elt, elt_type)
+            if starred:
+                # TODO: Handle starred node's type changes
+                # if not is_subtype(target_type, old_type):
+                    # self._issue(type_changes(self.locate(), 'an element of NODE', old_type.singular_name, elt_type.singular_name))
+                self.assign_target(starred[0], target_type)
+                for elt, elt_type, old_type in zip(trailing, tt, ot):
+                    # BUG: Any trailing elements will be incorrectly offset, so won't work with finite length stuff
+                    self.assign_target(elt, elt_type)
+        elif isinstance(target, ast.Subscript):
+            original_value_type = self.visit(target.value)
+            origin = self.identify_caller(target.value)
+            original_indexing_type = self.visit(target.slice)
+            original_type = original_value_type.index(original_indexing_type)
+            if operation:
+                new_target_type = apply_binary_operation(operation, original_type, target_type)
+                if isinstance(new_target_type, ImpossibleType):
+                    self._issue(incompatible_types(self.locate(), operation, original_type, target_type, report=self.report))
+            else:
+                new_target_type = target_type
+            original_type.set_index(original_indexing_type, new_target_type)
+            if origin:
+                origin_type = self.load_variable(origin)
+                self.store_variable(origin, origin_type.type)
+        elif isinstance(target, ast.Attribute):
+            original_type = self.visit(target.value)
+            origin = self.identify_caller(target.value)
+            if operation:
+                original_type_field = original_type.get_attr(target.attr)
+                new_target_type = apply_binary_operation(operation, original_type_field, target_type)
+                if isinstance(new_target_type, ImpossibleType):
+                    self._issue(incompatible_types(self.locate(), operation, original_type, target_type, report=self.report))
+            else:
+                new_target_type = target_type
+            assigned_type = original_type.add_attr(target.attr, new_target_type)
+            if isinstance(assigned_type, ImpossibleType):
+                self._issue(attribute_type_change(self.locate(), target.attr, original_type, new_target_type, report=self.report))
+            if origin:
+                origin_type = self.load_variable(origin)
+                if origin_type:
+                    self.store_variable(origin, origin_type.type)
+
+    def visit_AnnAssign(self, node):
+        """
+
+        Args:
+            node (ast.AnnAssign):
+
+        Returns:
+
+        """
+        # Name, Attribute, or SubScript
+        target = node.target
+        # Type
+        annotation = node.annotation
+        annotation_type = self.evaluate_type(annotation)
+        was_class_attribute = False
+        # Optional assigned value
+        value = node.value
+        # 0 or 1, with 1 indicating pure names (not expressions)
+        simple = node.simple
+
+        # If it's a class attribute, then build up the type!
+        if simple:
+            current_scope = self.scope_chain[0]
+            if current_scope in self.class_scopes:
+                self.class_scopes[current_scope].add_attr(target.id, annotation)
+                was_class_attribute = True
+        # TODO: Allow setting for optional type coercion, or throw error
+        if value:
+            self.visit(value)
+            # self.assign_target(target, self.visit(value))
+        # Make local variable either way
+        self.assign_target(target, annotation_type, store_with_read=was_class_attribute)
+
+    def visit_Assign(self, node):
+        """
+        Simple assignment statement:
+        __targets__ = __value__
+
+        Args:
+            node (ast.Assign): An Assign node
+        Returns:
+            None
+        """
+        # Handle value
+        value_type = self.visit(node.value)
+        # Apply value to all targets
+        for target in node.targets:
+            self.assign_target(target, value_type)
+
+    def visit_AugAssign(self, node):
+        """
+
+        Args:
+            node (ast.AugAssign):
+
+        Returns:
+
+        """
+        # Handle value
+        right = self.visit(node.value)
+        if isinstance(node.target, ast.Name):
+            self.load_variable(self.identify_caller(node.target))
+        self.assign_target(node.target, right, node.op)
+
+    def visit_Attribute(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        # Handle value
+        value_type = self.visit(node.value)
+        self.check_common_bad_lookups(value_type, node.attr, node.value)
+        # Handle attr
+        result = value_type.get_attr(node.attr)
+        # Set up self if this was a function (because now it's a method!)
+        # TODO: Handle static/class functions differently I guess?
+        if isinstance(result, FunctionType):
+            result = result.as_method(value_type)
+        return result
+
+    def visit_BinOp(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        # Handle left and right
+        left = self.visit(node.left)
+        right = self.visit(node.right)
+        operation = node.op
+
+        new_target_type = apply_binary_operation(operation, left, right)
+        if isinstance(new_target_type, ImpossibleType):
+            self._issue(incompatible_types(self.locate(), operation, left, right, report=self.report))
+        return new_target_type
+
+    def visit_Bool(self, node):
+        """
+        Visit a constant boolean value.
+
+        Args:
+            node (ast.AST): The boolean value Node.
+
+        Returns:
+            Type: A Bool type.
+        """
+        return BoolType()
+
+    def visit_BoolOp(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        # Handle left and right
+        values = [self.visit(value) for value in node.values]
+        # Handle operation
+        # Actually, the operations are always the same behavior!
+        # Handle truthiness
+        if self.get_setting('truthiness_returns_booleans'):
+            return BoolType()
+        elif not values:
+            return ImpossibleType()
+        # All same type? Then return the first one!
+        elif all(is_subtype(values[0], other) for other in values[1:]):
+            return values[0]
+        # Oh no, type union is necessary!
+        else:
+            return TypeUnion(values)
+
+    def load_root_variable(self, node, position=None):
+        root_name = self.identify_caller(node)
+        if root_name is not None:
+            variable = self.find_variable_scope(root_name)
+            if variable.exists:
+                return variable.state
+        return None
+
+    def visit_Call(self, node):
+        # Handle func part
+        function_type = self.visit(node.func)
+        # TODO: Need to grab the actual type in some situations
+        original_callee = self.load_root_variable(node)
+
+        # Handle args
+        arguments = [self.visit(arg) for arg in node.args] if node.args else []
+        keywords = [(kwarg.arg, self.visit(kwarg.value))
+                    for kwarg in node.keywords] if node.keywords else {}
+
+        # Check special common mistakes
+
+        if isinstance(function_type, BuiltinConstructorType):
+            constructor = function_type.definition
+            return constructor(self, function_type, original_callee,
+                               arguments, keywords, self.locate())
+        if isinstance(function_type, FunctionType):
+            # Test if we have called this definition before
+            if function_type.definition not in self.definition_chain:
+                self.definition_chain.append(function_type.definition)
+                # Function invocation
+                result = function_type.definition(self, function_type, original_callee,
+                                                  arguments, keywords, self.locate())
+                self.definition_chain.pop()
+                return result
+            else:
+                self._issue(recursive_call(self.locate(), original_callee, report=self.report))
+        elif isinstance(function_type, ClassType):
+            constructor = function_type.get_constructor().definition
+            self.definition_chain.append(constructor)
+            new_instance = constructor(self, constructor, original_callee, arguments, keywords, self.locate())
+            self.definition_chain.pop()
+            if '__init__' in function_type.fields:
+                initializer = function_type.fields['__init__'].as_method(new_instance)
+                if isinstance(initializer, FunctionType):
+                    self.definition_chain.append(initializer)
+                    initializer.definition(self, initializer, new_instance, [new_instance] + arguments, keywords, self.locate())
+                    self.definition_chain.pop()
+            return new_instance
+        elif isinstance(function_type, (IntType, FloatType, NumType, ListType,
+                                        DictType, SetType, TupleType, InstanceType,
+                                        StrType, BoolType, NoneType, LiteralValue)):
+            if original_callee is None:
+                self._issue(not_a_function(self.locate(), "a value", function_type, report=self.report))
+            else:
+                self._issue(not_a_function(self.locate(), original_callee.name, function_type, report=self.report))
+            return ImpossibleType()
+        return AnyType()
+
+    def visit_ClassDef(self, node):
+        """
+
+        Args:
+            node:
+        """
+        class_name = node.name
+        parents = [self.visit(base) for base in node.bases]
+        new_class_type = ClassType(class_name, {}, parents)
+        self.store_variable(class_name, new_class_type)
+        definitions_scope = self.scope_chain[:]
+        class_scope = NewScope(self, definitions_scope, class_type=new_class_type)
+        # TODO: Handle metaclass... somehow?
+        #self._visit_nodes(node.keywords)
+        with class_scope:
+            self._visit_nodes(node.body)
+        new_class_type = self.apply_decorators(class_name, new_class_type, node.decorator_list)
+        return new_class_type
+
+    def apply_decorators(self, new_name, new_type, decorators):
+        for decorator in reversed(decorators):
+            old_type = self.load_variable(new_name)
+            decorator_type = self.visit(decorator)
+            original_callee = self.load_root_variable(decorator)
+            new_type = decorator_type.definition(self, decorator_type, original_callee,
+                                                 [new_type], {}, self.locate())
+            self.store_variable(new_name, new_type)
+        return new_type
+
+    def visit_Compare(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        # Handle left and right
+        left = self.visit(node.left)
+        comparators = [self.visit(compare) for compare in node.comparators]
+
+        # Handle ops
+        for op, right in zip(node.ops, comparators):
+            if isinstance(op, (ast.Eq, ast.NotEq, ast.Is, ast.IsNot)):
+                continue
+            elif isinstance(op, (ast.Lt, ast.LtE, ast.GtE, ast.Gt)):
+                if type(right) in left.orderable:
+                    continue
+            elif isinstance(op, (ast.In, ast.NotIn)):
+                if right.allows_membership(left):
+                    continue
+            self._issue(incompatible_types(self.locate(), op, left, right, report=self.report))
+        return BoolType()
+
+    def visit_comprehension(self, node):
+        """
+
+        Args:
+            node:
+        """
+        self.fill_in_location(node, self.node_chain[-2])
+        self._visit_collection_loop(node)
+        # Handle ifs, unless they're blank (None in Skulpt :)
+        if node.ifs:
+            self.visit_statements(node.ifs)
+
+    def fill_in_location(self, node, source_node):
+        node.lineno = source_node.lineno
+        node.col_offset = source_node.col_offset
+        if IS_AT_LEAST_PYTHON_38:
+            node.end_lineno = source_node.end_lineno
+            node.end_col_offset = source_node.end_col_offset
+        else:
+            node.end_lineno = source_node.lineno
+            node.end_col_offset = source_node.col_offset
+
+    def visit_Dict(self, node):
+        """
+        Three types of dictionaries
+        - empty
+        - uniform type
+        - record
+        TODO: Handle records appropriately
+        """
+        items = [(self.visit(key), self.visit(value))
+                 for key, value in zip(node.keys, node.values) if key is not None]
+        # Unpack starred dictionaries
+        for key, value in zip(node.keys, node.values):
+            if key is None:
+                value_type = self.visit(value)
+                if isinstance(value_type, DictType):
+                    items.extend([
+                        (k, v) for k, v in value_type.element_types
+                    ])
+        # Empty dictionary
+        if not items:
+            return DictType([])
+        # All literal keys
+        if all(isinstance(k, LiteralValue) for k, _ in items):
+            return DictType([(k, v) for k, v in items])
+        # Find if all matched type
+        first_key = widest_type([key for key, value in items])
+        first_value = widest_type([value for key, value in items])
+        if first_key is not None and first_value is not None:
+            return DictType([(first_key, first_value)])
+        else:
+            # Resort to just matching the types?
+            return DictType([(k, v) for k, v in items])
+
+    def visit_DictComp(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        generator_scope = NewScope(self, self.scope_chain[:])
+        with generator_scope:
+            self._visit_nodes(node.generators)
+            keys = self.visit(node.key)
+            values = self.visit(node.value)
+            return DictType([(keys, values)])
+
+    def visit_Expr(self, node):
+        """
+        Any expression being used as a statement.
+
+        Args:
+            node (AST): An Expr node
+
+        Returns:
+
+        """
+        value = self.visit(node.value)
+        if isinstance(node.value, ast.Call) and not isinstance(value, NoneType):
+            # TODO: Helper function to get name with title ("append method")
+            if isinstance(node.value.func, ast.Name):
+                call_type = 'function'
+            else:
+                call_type = 'method'
+            name = self.identify_caller(node.value)
+            self._issue(unused_returned_value(self.locate(), name,
+                                              call_type, value))
+
+    def visit_For(self, node):
+        """
+
+        Args:
+            node:
+        """
+        was_empty = self._visit_collection_loop(node)
+        # Handle the bodies
+        # if not was_empty:
+        # this_path_id = self.path_chain[0]
+        # non_empty_path = NewPath(self, this_path_id, "f")
+        # with non_empty_path:
+        self.visit_statements(node.body)
+        self.visit_statements(node.orelse)
+
+    def visit_FunctionDef(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        function_name = node.name
+        position = self.locate()
+        definitions_scope = self.scope_chain[:]
+        definition = self.make_function(function_name, definitions_scope, position, node)
+        function = FunctionType(function_name, definition=definition)
+        self.store_variable(function_name, function)
+
+        if len(self.node_chain) > 2:
+            self._issue(nested_function_definition(self.locate(), function_name))
+
+        return self.apply_decorators(function_name, function, node.decorator_list)
+
+    def make_function(self, function_name, definitions_scope, position, node):
+        is_lambda = function_name is None
+
+        class SkipType:
+            pass
+        # Pull apart args into a coherent set of data PRIOR to execution
+        args = node.args
+        pos_parameters = args.posonlyargs + args.args if IS_AT_LEAST_PYTHON_38 and not IS_SKULPT else args.args
+        none_padding = [SkipType] * (len(pos_parameters) - len(args.defaults))
+        pos_defaults = none_padding + [self.visit(d) for d in args.defaults]
+        kwarg_parameter = args.kwarg
+        vararg_parameter = args.vararg
+
+        # TODO: Finish kwargs
+        named_parameters = args.kwonlyargs
+        named_defaults = [self.visit(d) if d is not None else AnyType() for d in args.kw_defaults]
+        expected_returns = self.evaluate_type(node.returns) if not is_lambda and node.returns else None
+
+        def definition(tifa, function, callee_name, arguments, named_arguments, call_position):
+            function_scope = NewScope(self, definitions_scope)
+            with function_scope:
+                # Process arguments
+                if len(arguments) + len(named_arguments) != len(pos_parameters) and not vararg_parameter:
+                    self._issue(incorrect_arity(self.locate(), function_name,
+                                                len(pos_parameters), len(arguments), report=self.report))
+                for parameter, default, argument in zip(pos_parameters, pos_defaults, arguments):
+                    parameter_name = parameter.arg
+                    if parameter.annotation:
+                        annotation = self.evaluate_type(parameter.annotation)
+                        if is_subtype(argument, annotation):
+                            specify_subtype(annotation, argument)
+                        else:
+                            self._issue(parameter_type_mismatch(self.locate(), parameter_name,
+                                                                annotation, argument))
+                    elif default is not SkipType:
+                        if is_subtype(argument, default):
+                            specify_subtype(default, argument)
+                        else:
+                            self._issue(parameter_type_mismatch(self.locate(), parameter_name,
+                                                                default, argument))
+                    if argument is not None:
+                        argument_type = argument.clone_mutably()
+                        self.create_variable(parameter_name, argument_type, position)
+                # Too many arguments
+                if len(pos_parameters) < len(arguments):
+                    if vararg_parameter:
+                        the_rest = arguments[len(pos_parameters):]
+                        self.create_variable(vararg_parameter.arg, TupleType(the_rest), position)
+                # Not enough arguments
+                if len(pos_parameters) > len(arguments):
+                    for parameter in pos_parameters[len(arguments):]:
+                        if parameter.annotation:
+                            annotation = self.evaluate_type(parameter.annotation)
+                        else:
+                            annotation = AnyType()
+                        self.create_variable(parameter.arg, annotation, position)
+                if is_lambda:
+                    return self.visit(node.body)
+
+                self.visit_statements(node.body)
+                return_state = self.find_variable_scope("*return")
+                return_value = NoneType()
+                # TODO: Figure out if we are not returning something when we should
+                # If the pseudo variable exists, we load it and get its type
+                if return_state.exists and return_state.in_scope:
+                    return_state = self.load_variable("*return", call_position)
+                    return_value = return_state.type
+                    if expected_returns:
+                        if not is_subtype(return_value, expected_returns):
+                            self._issue(multiple_return_types(return_state.position,
+                                                              expected_returns.singular_name,
+                                                              return_value.singular_name,
+                                                              report=self.report))
+            return return_value
+        return definition
+
+    def evaluate_type(self, node):
+        string_literal = False
+        if isinstance(node, ast.Str):
+            string_literal = node.s
+        elif isinstance(node, ast.Constant) and isinstance(node.value, str):
+            string_literal = node.value
+        if string_literal is not False:
+            if self.get_setting('evaluate_string_literal_types'):
+                # TODO: Handle string literal types properly!
+                pass
+            else:
+                return LiteralStr(string_literal)
+        elif isinstance(node, ast.List):
+            if node.elts:
+                return ListType(False, self.evaluate_type(node.elts[0]))
+            else:
+                return ListType(True)
+        elif isinstance(node, ast.Set) and node.elts:
+            return TypeUnion([self.evaluate_type(e) for e in node.elts])
+        elif isinstance(node, ast.Tuple) and node.elts:
+            return TupleType([self.evaluate_type(e) for e in node.elts])
+        elif isinstance(node, ast.Dict):
+            if node.keys and node.values:
+                return DictType([(self.evaluate_type(k), self.evaluate_type(v))
+                                 for k, v in zip(node.keys, node.values)])
+            else:
+                return DictType([])
+        else:
+            evaluated = self.visit(node)
+            return evaluated.as_type(self, self.locate(node))
+
+    def visit_GeneratorExp(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        generator_scope = NewScope(self, self.scope_chain[:])
+        with generator_scope:
+            self._visit_nodes(node.generators)
+            return GeneratorType(False, self.visit(node.elt))
+
+    def visit_If(self, node):
+        """
+
+        Args:
+            node:
+        """
+        # Visit the conditional
+        self.visit(node.test)
+
+        if len(node.orelse) == 1 and isinstance(node.orelse[0], ast.Pass):
+            self._issue(unnecessary_second_branch(self.locate()))
+        elif len(node.body) == 1 and isinstance(node.body[0], ast.Pass):
+            if node.orelse:
+                self._issue(unnecessary_second_branch(self.locate()))
+
+        # Visit the bodies
+        this_path_id = self.path_chain[0]
+        if_path = NewPath(self, this_path_id, "i")
+        with if_path:
+            for statement in node.body:
+                self.visit(statement)
+        else_path = NewPath(self, this_path_id, "e")
+        with else_path:
+            for statement in node.orelse:
+                self.visit(statement)
+
+        # TODO: Unconditional return
+
+        # Combine two paths into one
+        # Check for any names that are on the IF path
+        self.merge_paths(this_path_id, if_path.id, else_path.id)
+
+    def visit_IfExp(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        # Visit the conditional
+        self.visit(node.test)
+
+        # Visit the body
+        body = self.visit(node.body)
+
+        # Visit the orelse
+        orelse = self.visit(node.orelse)
+
+        if is_subtype(body, orelse):
+            return body
+
+        # TODO: Union type?
+        return TypeUnion([body, orelse])
+
+    def visit_Import(self, node):
+        """
+
+        Args:
+            node:
+        """
+        # Handle names
+        for alias in node.names:
+            asname = alias.asname or alias.name
+            module_type = self.load_module(alias.name)
+            self.store_variable(asname, module_type)
+
+    def visit_ImportFrom(self, node):
+        """
+
+        Args:
+            node:
+        """
+        # Handle names
+        for alias in node.names:
+            if alias.name == '*':
+                module_type = self.load_module(node.module)
+                for field, value in module_type.fields.items():
+                    self.store_read_variable(field, value)
+            else:
+                if node.module is None:
+                    asname = alias.asname or alias.name
+                    module_type = self.load_module(alias.name)
+                else:
+                    module_name = node.module
+                    asname = alias.asname or alias.name
+                    module_type = self.load_module(module_name)
+                name_type = module_type.get_attr(alias.name)
+                self.store_variable(asname, name_type)
+
+    def visit_Lambda(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        position = self.locate()
+        definitions_scope = self.scope_chain[:]
+        definition = self.make_function(None, definitions_scope, position, node)
+        return FunctionType("*lambda", definition=definition)
+
+    def visit_List(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        if not node.elts:
+            return ListType(True)
+
+        # All literal keys
+        elements = [self.visit(v) for v in node.elts]
+        if all(isinstance(v, LiteralValue) for v in elements):
+            # TODO: Allow type union instead?
+            return ListType(False, elements[0].promote())
+        # Find if all matched type
+        first_value = widest_type(elements)
+        if first_value is not None:
+            return ListType(False, first_value)
+        else:
+            # Resort to just matching the types?
+            return ListType(False, TypeUnion(elements))
+
+    def visit_ListComp(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        # TODO: Handle comprehension scope
+        generator_scope = NewScope(self, self.scope_chain[:])
+        with generator_scope:
+            self._visit_nodes(node.generators)
+            return ListType(False, self.visit(node.elt))
+
+    def visit_NameConstant(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        value = node.value
+        if isinstance(value, bool):
+            return LiteralBool(value)
+        else:
+            return NoneType()
+
+    def visit_Name(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        name = node.id
+        if name == "___":
+            self._issue(unconnected_blocks(self.locate()))
+        if isinstance(node.ctx, ast.Load):
+            if name == "True" or name == "False":
+                return LiteralBool(name == "True")
+            elif name == "None":
+                return NoneType()
+            else:
+                variable = self.find_variable_scope(name)
+                builtin = get_builtin_name(name)
+                if not variable.exists and builtin:
+                    return builtin
+                else:
+                    state = self.load_variable(name)
+                    return state.type
+        else:
+            variable = self.find_variable_scope(name)
+            if variable.exists:
+                return variable.state.type
+            else:
+                return AnyType()
+
+    def visit_Num(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        return LiteralInt(node.n) if isinstance(node.n, int) else LiteralFloat(node.n)
+
+    def visit_Constant(self, node) -> Type:
+        """ Handle new 3.8's Constant node """
+        return get_pedal_type_from_value(node.value, self.evaluate_type)
+
+    def visit_Return(self, node):
+        """
+
+        Args:
+            node:
+        """
+        if len(self.scope_chain) == 1:
+            self._issue(return_outside_function(self.locate(), report=self.report))
+        # TODO: Unconditional return inside loop
+        if node.value is not None:
+            self.return_variable(self.visit(node.value))
+        else:
+            self.return_variable(NoneType())
+
+    def visit_Set(self, node):
+        # Fun fact, it's impossible to make a literal empty set
+        if not node.elts:
+            return SetType(True)
+
+        # All literal keys
+        elements = [self.visit(v) for v in node.elts]
+        if all(isinstance(v, LiteralValue) for v in elements):
+            # TODO: Allow type union instead?
+            return SetType(False, elements[0].promote())
+        # Find if all matched type
+        first_value = widest_type(elements)
+        if first_value is not None:
+            return SetType(False, first_value)
+        else:
+            # Resort to just matching the types?
+            return SetType(False, TypeUnion(elements))
+
+    def visit_SetComp(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        # TODO: Handle comprehension scope
+        generator_scope = NewScope(self, self.scope_chain[:])
+        with generator_scope:
+            self._visit_nodes(node.generators)
+            return SetType(False, self.visit(node.elt))
+
+    def visit_statements(self, nodes):
+        """
+
+        Args:
+            nodes:
+
+        Returns:
+
+        """
+        # TODO: Check for pass in the middle of a series of statement
+        if any(isinstance(node, ast.Pass) for node in nodes):
+            pass
+        return [self.visit(statement) for statement in nodes]
+
+    def visit_Str(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        return LiteralStr(node.s)
+
+    def visit_JoinedStr(self, node):
+        values = [self.visit(expr) for expr in node.values]
+        # The result will be all StrType
+        return StrType(is_empty=all(isinstance(n, (StrType, LiteralStr)) and n.is_empty
+                                    for n in values))
+
+    def visit_FormattedValue(self, node):
+        value = self.visit(node.value)
+        if isinstance(value, StrType):
+            return value
+        else:
+            return StrType(is_empty=False)
+
+    def visit_Subscript(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        # Handle value
+        value_type = self.visit(node.value)
+        slice_type = self.visit(node.slice)
+        result = value_type.index(slice_type)
+        if isinstance(result, ImpossibleType):
+            self._issue(invalid_indexing(self.locate(), value_type, slice_type))
+        if isinstance(node.slice, ast.Slice):
+            return value_type.shallow_clone()
+        else:
+            return result
+
+    def visit_Slice(self, node):
+        """ Handles a slice by visiting its components; cannot return a value
+        because the slice is always the same type as its value, which is
+        not available on the Slice node itself. """
+        if node.lower is not None:
+            self.visit(node.lower)
+        if node.upper is not None:
+            self.visit(node.upper)
+        if node.step is not None:
+            self.visit(node.step)
+
+    def visit_Index(self, node):
+        return self.visit(node.value)
+
+    def visit_ExtSlice(self, node):
+        return TupleType([self.visit(d) for d in node.dims])
+
+    def visit_Starred(self, node):
+        return self.visit(node.value).break_apart()
+
+    def visit_Tuple(self, node) -> TupleType:
+        # Fun fact, it's impossible to make a literal empty set
+        if not node.elts:
+            return TupleType(True)
+
+        # All literal keys
+        return TupleType([self.visit(v) for v in node.elts])
+
+    def visit_UnaryOp(self, node):
+        """
+
+        Args:
+            node:
+
+        Returns:
+
+        """
+        # Handle operand
+        operand_type = self.visit(node.operand)
+        return apply_unary_operation(node.op, operand_type)
+
+    def visit_While(self, node):
+        """
+
+        Args:
+            node:
+        """
+        # Visit conditional
+        self.visit(node.test)
+
+        # Visit the bodies
+        this_path_id = self.path_id
+        # One path is that we never enter the body
+        empty_path = NewPath(self, this_path_id, "e")
+        with empty_path:
+            pass
+        # Another path is that we loop through the body and check the test again
+        body_path = NewPath(self, this_path_id, "w")
+        with body_path:
+            for statement in node.body:
+                self.visit(statement)
+            # Revisit conditional
+            self.visit(node.test)
+        # If there's else bodies (WEIRD) then we should check them afterwards
+        if node.orelse:
+            self._issue(else_on_loop_body(self.locate()))
+            for statement in node.orelse:
+                self.visit(statement)
+
+        # Combine two paths into one
+        # Check for any names that are on the IF path
+        self.merge_paths(this_path_id, body_path.id, empty_path.id)
+
+    def visit_With(self, node):
+        """
+
+        Args:
+            node:
+        """
+        for item in node.items:
+            type_value = self.visit(item.context_expr)
+            if item.optional_vars is not None:
+                self.assign_target(item.optional_vars, type_value)
+        # Handle the bodies
+        self.visit_statements(node.body)
```

### Comparing `pedal-2.6.1/pedal/types/builtin.py` & `pedal-2.6.2/pedal/types/builtin.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/types/library/cs1_curriculum.py` & `pedal-2.6.2/pedal/types/library/cs1_curriculum.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/types/library/designer.py` & `pedal-2.6.2/pedal/types/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/types/library/drafter.py` & `pedal-2.6.2/pedal/types/library/drafter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from pedal.types.new_types import ModuleType, FunctionType, void_function, ClassType, \
     InstanceType, bool_function, int_function, str_function, register_builtin_module, AnyType, ListType
 
 # TODO: route, Button, ...
 
 _VOID_FUNCTIONS = ['start_server', 'show_debug_information', 'hide_debug_information']
-_COMPONENT_FUNCTIONS = ["Image", "Link", "TextBox", "TextArea", "SelectBox",
-                        "CheckBox", "LineBreak", "HorizontalRule", "Button",
-                        "NumberedList", "BulletedList", "Header", "Table"]
+_COMPONENT_FUNCTIONS = ['BulletedList', 'Button', 'CheckBox',
+                        'Header', 'HorizontalRule', 'Image', 'LineBreak', 'Link', 'LinkContent',
+                        'NumberedList', 'PageContent', 'SelectBox',
+                        'SubmitButton', 'Table', 'Text', 'TextArea', 'TextBox', 'Span', 'Argument']
 _IDENTITY_FUNCTIONS = ["route"]
 
 
 def build_drafter_module():
     _PageObject = ClassType('Page', {
         'state': AnyType(),
         'content': ListType(AnyType())
```

### Comparing `pedal-2.6.1/pedal/types/library/matplotlib.py` & `pedal-2.6.2/pedal/types/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/types/library/microbit.py` & `pedal-2.6.2/pedal/types/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/types/new_types.py` & `pedal-2.6.2/pedal/types/new_types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/types/normalize.py` & `pedal-2.6.2/pedal/types/normalize.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/types/operations.py` & `pedal-2.6.2/pedal/types/operations.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/utilities/__init__.py` & `pedal-2.6.2/pedal/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/utilities/ast_tools.py` & `pedal-2.6.2/pedal/utilities/ast_tools.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/utilities/comparisons.py` & `pedal-2.6.2/pedal/utilities/comparisons.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/utilities/dictionaries.py` & `pedal-2.6.2/pedal/utilities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/utilities/exceptions.py` & `pedal-2.6.2/pedal/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/utilities/files.py` & `pedal-2.6.2/pedal/utilities/files.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/utilities/operators.py` & `pedal-2.6.2/pedal/utilities/operators.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/utilities/progsnap.py` & `pedal-2.6.2/pedal/utilities/progsnap.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/utilities/sorting.py` & `pedal-2.6.2/pedal/utilities/sorting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/utilities/text.py` & `pedal-2.6.2/pedal/utilities/text.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/pedal/utilities/types.py` & `pedal-2.6.2/pedal/utilities/types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/setup.py` & `pedal-2.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='pedal',
-    version='2.6.1',
+    version='2.6.2',
     python_requires='>=3.7',
     author='acbart,lukesg08',
     author_email='acbart@udel.edu',
     description='Tools to provide feedback on student code.',
     keywords='feedback education teaching program analysis tifa cait sandbox pedal grading grader grade',
     packages=['pedal', 'pedal.core', 'pedal.utilities', 'pedal.environments',
               'pedal.resolvers', 'pedal.command_line',
```

### Comparing `pedal-2.6.1/tests/test_assertion_dataclasses.py` & `pedal-2.6.2/tests/test_assertion_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_assertion_functions.py` & `pedal-2.6.2/tests/test_assertion_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 Line 3 of file answer.py in make_polite
         return ", please"+make_polite
 """ + ('               ^^^^^^^^^^^^^^^^^^^^^^\n' if IS_AT_LEAST_PYTHON_311 else "") + """
 Type errors occur when you use an operator or function on the wrong type of value. For example, using `+` to add to a list (instead of `.append`), or dividing a string by a number.
 
 Suggestion: To fix a type error, you should trace through your code. Make sure each expression has the type you expect it to have.""")
 
+    @unittest.skip("Temporarily disabled while we fix skulpt's context manager")
     def test_unit_test_with_style(self):
         with Execution("""
 def add(a, b):
     return a - b""", run_tifa=False) as e:
             with unit_test('add'):
                 assert_equal(call('add', 1, 2), 3)
                 assert_equal(call('add', 0, 0), 0)
```

### Comparing `pedal-2.6.1/tests/test_assertion_static.py` & `pedal-2.6.2/tests/test_assertion_static.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_assertions_runtime.py` & `pedal-2.6.2/tests/test_assertions_runtime.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_cait.py` & `pedal-2.6.2/tests/test_cait.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_cait_node.py` & `pedal-2.6.2/tests/test_cait_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_drafter.py` & `pedal-2.6.2/tests/test_drafter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from textwrap import dedent
 
 from pedal.assertions.feedbacks import assert_group
 from pedal.assertions.runtime import *
 from pedal.sandbox.commands import call, start_trace, get_sandbox, evaluate, CommandBlock, run
 from tests.execution_helper import Execution, ExecutionTestCase, SUCCESS_MESSAGE
-from pedal.sandbox.library.drafter import MockDrafter
+from pedal.sandbox.library.drafter_library import MockDrafter
 import unittest
 
 
 @unittest.skip
 class TestAssertions(ExecutionTestCase):
 
     def test_basic_mocking(self):
```

### Comparing `pedal-2.6.1/tests/test_environment_nbgrader.py` & `pedal-2.6.2/tests/test_environment_nbgrader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_environment_terminal.py` & `pedal-2.6.2/tests/test_environment_terminal.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,135 +26,135 @@
 
     def test_correct(self):
         with io.StringIO() as f, redirect_stdout(f):
             terminal = setup_environment(main_code="""1+2""")
             terminal.resolve()
             clear_report()
             self.checkFeedback(f.getvalue(), '''
-[;7mYOUR CODE[0;0m We ran your code. Here's the output:
+[;7m YOUR CODE [0;0m We ran your code. Here's the output:
 
 
-[;7mFEEDBACK[0;0m Based on your code, here are some tips and recommendations:
+[;7m FEEDBACK [0;0m Based on your code, here are some tips and recommendations:
 
 [1;92m✓[0;0m️  Your code ran successfully.
 
 Great work! Based on your code submitted, there are no other recommendations available. You can proceed to the next page by using the “Next” button in your lesson.
 ''')
 
     def test_empty_source(self):
         with io.StringIO() as f, redirect_stdout(f):
             terminal = setup_environment(main_code="")
             terminal.resolve()
             clear_report()
             self.checkFeedback(f.getvalue(), '''
-[;7mYOUR CODE[0;0m We ran your code. Here's the output:
+[;7m YOUR CODE [0;0m We ran your code. Here's the output:
 
 
-[;7mFEEDBACK[0;0m Based on your code, here are some tips and recommendations:
+[;7m FEEDBACK [0;0m Based on your code, here are some tips and recommendations:
 
 [1;91m✗[0;0m  No Source Code
 
 Source code file is blank.
 ''')
 
     def test_syntax_error(self):
         with io.StringIO() as f, redirect_stdout(f):
             terminal = setup_environment(main_code="""1 1 2 3""")
             terminal.resolve()
             clear_report()
             self.checkFeedback(f.getvalue(), '''
-[;7mYOUR CODE[0;0m We ran your code. Here's the output:
+[;7m YOUR CODE [0;0m We ran your code. Here's the output:
 
 
-[;7mFEEDBACK[0;0m Based on your code, here are some tips and recommendations:
+[;7m FEEDBACK [0;0m Based on your code, here are some tips and recommendations:
 
 [1;91m✗[0;0m  Syntax Error
 
 Bad syntax on line [4m1[0;0m.
 Suggestion: Check line [4m1[0;0m, the line before it, and the line after it. Ignore blank lines.
 
-[;7mTERMINAL OUTPUT[0;0m For reference, here is the original Python error:
+[;7m TERMINAL OUTPUT [0;0m For reference, here is the original Python error:
 
 Line [4m1[0;0m of file [4manswer.py[0;0m
     1 1 2 3
 ''' + ('      ^\n' if IS_AT_LEAST_PYTHON_311 else "") + '''
 SyntaxError: Invalid syntax.
 ''')
 
     def test_tifa_feedback(self):
         with io.StringIO() as f, redirect_stdout(f):
             terminal = setup_environment(main_code="""1+''""")
             terminal.resolve()
             clear_report()
             self.checkFeedback(f.getvalue(), '''
-[;7mYOUR CODE[0;0m We ran your code. Here's the output:
+[;7m YOUR CODE [0;0m We ran your code. Here's the output:
 
 
-[;7mFEEDBACK[0;0m Based on your code, here are some tips and recommendations:
+[;7m FEEDBACK [0;0m Based on your code, here are some tips and recommendations:
 
 [1;91m✗[0;0m  Incompatible types
 
 You used an addition operation with an integer and a string on line [4m1[0;0m. But you can't do that with that operator. Make sure both sides of the operator are the right type.
 
-[;7mTERMINAL OUTPUT[0;0m For reference, here is the original Python error:
+[;7m TERMINAL OUTPUT [0;0m For reference, here is the original Python error:
 
 Line [4m1[0;0m of file [4manswer.py[0;0m
     1+''
 ''' + ('    ^^^^\n' if IS_AT_LEAST_PYTHON_311 else "") + '''
 TypeError: Unsupported operand type(s) for +: 'int' and 'str'
     ''')
 
     def test_runtime_feedback(self):
         with io.StringIO() as f, redirect_stdout(f):
             terminal = setup_environment(main_code="""import json\njson.loads('1')+''""")
             terminal.resolve()
             clear_report()
             self.checkFeedback(f.getvalue(), '''
-[;7mYOUR CODE[0;0m We ran your code. Here's the output:
+[;7m YOUR CODE [0;0m We ran your code. Here's the output:
 
 
-[;7mFEEDBACK[0;0m Based on your code, here are some tips and recommendations:
+[;7m FEEDBACK [0;0m Based on your code, here are some tips and recommendations:
 
 [1;91m✗[0;0m  Type Error
 
 I ran your code.
 
 A TypeError occurred:
 
     Unsupported operand type(s) for +: 'int' and 'str'
 
 Type errors occur when you use an operator or function on the wrong type of value. For example, using `+` to add to a list (instead of `.append`), or dividing a string by a number.
 
 Suggestion: To fix a type error, you should trace through your code. Make sure each expression has the type you expect it to have.
 
-[;7mTERMINAL OUTPUT[0;0m For reference, here is the original Python error:
+[;7m TERMINAL OUTPUT [0;0m For reference, here is the original Python error:
 
 Line [4m2[0;0m of file [4manswer.py[0;0m
     json.loads('1')+''
 ''' + ('    ^^^^^^^^^^^^^^^^^^\n' if IS_AT_LEAST_PYTHON_311 else "") + '''
 TypeError: Unsupported operand type(s) for +: 'int' and 'str'
 ''')
 
     def test_explain(self):
         with io.StringIO() as f, redirect_stdout(f):
             terminal = setup_environment(main_code="""import json\njson.loads('1')+''""")
             explain("You should not be using the JSON library at all.")
             terminal.resolve()
             clear_report()
             self.checkFeedback(f.getvalue(), '''
-[;7mYOUR CODE[0;0m We ran your code. Here's the output:
+[;7m YOUR CODE [0;0m We ran your code. Here's the output:
 
 
-[;7mFEEDBACK[0;0m Based on your code, here are some tips and recommendations:
+[;7m FEEDBACK [0;0m Based on your code, here are some tips and recommendations:
 
 [1;91m✗[0;0m  Instructor Feedback
 
 You should not be using the JSON library at all.
 
-[;7mTERMINAL OUTPUT[0;0m For reference, here is the original Python error:
+[;7m TERMINAL OUTPUT [0;0m For reference, here is the original Python error:
 
 Line [4m2[0;0m of file [4manswer.py[0;0m
     json.loads('1')+''
 ''' + ('    ^^^^^^^^^^^^^^^^^^\n' if IS_AT_LEAST_PYTHON_311 else "") + '''
 TypeError: Unsupported operand type(s) for +: 'int' and 'str'
 ''')
 
@@ -162,32 +162,32 @@
     def test_call_assertion(self):
         with io.StringIO() as f, redirect_stdout(f):
             terminal = setup_environment(main_code="""def x(): return 1+''\nx""")
             assert_equal(call('x'), 5)
             terminal.resolve()
             clear_report()
             self.checkFeedback(f.getvalue(), '''
-[;7mYOUR CODE[0;0m We ran your code. Here's the output:
+[;7m YOUR CODE [0;0m We ran your code. Here's the output:
 
 
-[;7mFEEDBACK[0;0m Based on your code, here are some tips and recommendations:
+[;7m FEEDBACK [0;0m Based on your code, here are some tips and recommendations:
 
 [1;91m✗[0;0m  Type Error
 
 I ran the code:
     x()
 
 A TypeError occurred:
 
     Unsupported operand type(s) for +: 'int' and 'str'
 
 Type errors occur when you use an operator or function on the wrong type of value. For example, using `+` to add to a list (instead of `.append`), or dividing a string by a number.
 
 Suggestion: To fix a type error, you should trace through your code. Make sure each expression has the type you expect it to have.
 
-[;7mTERMINAL OUTPUT[0;0m For reference, here is the original Python error:
+[;7m TERMINAL OUTPUT [0;0m For reference, here is the original Python error:
 
 Line [4m1[0;0m of file [4manswer.py[0;0m in x
     def x(): return 1+''
 ''' + ('                    ^^^^\n' if IS_AT_LEAST_PYTHON_311 else "") + '''
 TypeError: Unsupported operand type(s) for +: 'int' and 'str'
 ''')
```

### Comparing `pedal-2.6.1/tests/test_formatter.py` & `pedal-2.6.2/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_loader.py` & `pedal-2.6.2/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_microbits.py` & `pedal-2.6.2/tests/test_microbits.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_plots.py` & `pedal-2.6.2/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_questions.py` & `pedal-2.6.2/tests/test_questions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_report.py` & `pedal-2.6.2/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_sandbox.py` & `pedal-2.6.2/tests/test_sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_sneks_functions.py` & `pedal-2.6.2/tests/test_sneks_functions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_source.py` & `pedal-2.6.2/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_testing_libraries.py` & `pedal-2.6.2/tests/test_testing_libraries.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_tifa.py` & `pedal-2.6.2/tests/test_tifa.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1228 +1,1247 @@
-import traceback
-import unittest
-import os
-import sys
-from textwrap import dedent
-from pprint import pprint
-from dataclasses import dataclass
-
-sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
-import pedal.tifa
-import pedal.types.new_types as defs
-import pedal.types.normalize as normalize
-from pedal import contextualize_report, Submission, evaluate
-from pedal.tifa import tifa_provide_module_type
-
-unit_tests = {
-    # Source Code, Shouldn't catch this, Should catch this
-    'builtin_True': ['print(True)', ['initialization_problem'], []],
-    'unread_variable': ['a = 0', [], ['unused_variable']],
-    'undefined_variable': ['print(a)', [], ['initialization_problem']],
-    'defined_read_variable': ['a = 0\nprint(a)', ['initialization_problem'], []],
-    'overwritten_variable': ['a = 0\na = 5', [], ['overwritten_variable']],
-    'unread_variables': ['a = 0\nb = 5', ['overwritten_variable'], ['unused_variable']],
-    'wrwr_variable': ['a = [1]\nprint(a)\na = [1]\nprint(a)', [], []],
-    # unconnected_blocks
-    'unconnected_assign': ['a = ___', [], ['unconnected_blocks']],
-    'unconnected_print': ['print(___)', [], ['unconnected_blocks']],
-
-    'literal_in_call': ['print("dog" in input("test"))', [], []],
-    'wrong_method_for_type': ['[].replace(",","")', [], []],
-
-    "check_true_argument_in_function_call":
-        ['def is_true(x:bool)->bool:\n return x\nis_true(True)', 'parameter_type_mismatch', ''],
-
-    # Double call
-    'double_call': ['def x(a):\n    return a\nx(5)\nx(3)', ['read_out_of_scope'], []],
-
-    # Chained functions
-    'chained_functions': ['def x():\n    return 0\ndef y():\n    x()\ny()',
-                          ['read_out_of_scope', 'initialization_problem'], []],
-
-    # String indexing and slicing
-    'string_indexing_slicing': ['("a"[0] + ""[:])[:][0]', ['incompatible_types'], []],
-    # List indexing and slicing
-    'list_indexing_slicing': ['([0][0] + [1,2,3][:][2])', ['incompatible_types'], []],
-
-    'returned_string':
-        [
-            'def pluralize(a_word):\n    return a_word+"s"\nnoun = pluralize("Dog")\nprint(noun + " can pet other " + noun)',
-            ['incompatible_types'], []],
-    'update_without_read':
-        ['a = 0\na+= 1', ['initialization_problem'], ['unused_variable']],
-    'update_and_read':
-        ['a = 0\na+= 1\nprint(a)', ['initialization_problem', 'unused_variable'], []],
-    'iterate_through_non_existing_list':
-        ['for x in y:\n\tpass', ['unused_variable'], ['initialization_problem']],
-    'iterate_through_list':
-        ['y = [1,2,3]\nfor x in y:\n\tpass', ['unused_variable', 'initialization_problem'], []],
-    'iterate_through_empty_list':
-        ['y = []\nfor x in y:\n\tpass', ['unused_variable', 'initialization_problem'], ['iterating_over_empty_list']],
-    'double_iterate_through_strings':
-        ['ss = ["Testing", "Here"]\nfor a in ss:\n    print(a)\nfor b in a:\n    print(b)',
-         ['iterating_over_non_list', 'iterating_over_empty_list'], []],
-    'iterate_through_number':
-        ['y = 5\nfor x in y:\n\tpass', ['unused_variable', 'initialization_problem'], ['iterating_over_non_list']],
-    'iterate_over_iteration_variable':
-        ['y = [1,2,3]\nfor y in y:\n\tpass', [], ['iteration_problem']],
-    'type_change':
-        ['a = 0\nprint(a)\na="T"\nprint(a)', [], ['type_changes']],
-    'defined_in_if_root_but_not_other':
-        ['if True:\n\ta = 0\nprint(a)', [], ['possible_initialization_problem']],
-    'defined_in_both_branches':
-        ['if True:\n\ta = 0\nelse:\n\ta = 1\nprint(a)', ['possible_initialization_problem'], []],
-    'defined_in_else_root_but_not_other':
-        ['if True:\n\tpass\nelse:\n\ta = 1\nprint(a)', [], ['possible_initialization_problem']],
-    'defined_in_if_branch_but_others':
-        ['if True:\n\tif False:\n\t\ta = 0\nprint(a)', [], ['possible_initialization_problem']],
-    'defined_before_if_branch_but_not_others':
-        ['if True:\n\ta = 0\nif False:\t\tpass\nprint(a)', [], ['possible_initialization_problem']],
-    'defined_after_if_branch_but_not_others':
-        ['if True:\n\tif False:\n\t\tpass\n\ta = 0\nprint(a)', [], ['possible_initialization_problem']],
-    'defined_within_both_if_branches_but_not_others':
-        ['if True:\n\tif False:\n\t\ta=0\n\telse:\n\t\ta = 0\nprint(a)', [], ['possible_initialization_problem']],
-    'defined_in_all_branches':
-        ['if True:\n\tif False:\n\t\ta=0\n\telse:\n\t\ta = 0\nelse:\n\ta=3\nprint(a)',
-         ['possible_initialization_problem'], []],
-    'read_in_if_branch_but_unset':
-        ['if True:\n\tprint(a)', [], ['initialization_problem']],
-    'read_in_else_branch_but_unset':
-        ['if True:\n\tpass\nelse:\n\tprint(a)', [], ['initialization_problem']],
-    'read_in_both_branches_but_unset':
-        ['if True:\n\tprint(a)\nelse:\n\tprint(a)', [], ['initialization_problem']],
-    'overwritten_in_both_branches':
-        ['a = 0\nif True:\n\ta = 0\nelse:\n\ta = 1', [], ['overwritten_variable']],
-    'overwritten_in_one_branch':
-        ['a = 0\nif True:\n\tpass\nelse:\n\ta = 1', ['overwritten_variable'], []],
-    'overwritten_in_inner_branch':
-        ['a = 0\nif True:\n\tif False:\n\t\ta = 0\nelse:\n\ta = 1', ['overwritten_variable'], []],
-    'overwritten_in_all_branch':
-        ['a = 0\nif True:\n\tif False:\n\t\ta = 0\n\telse:\n\t\ta = 2\nelse:\n\ta = 1', [], ['overwritten_variable']],
-    'overwritten_in_all_branches2':
-        ['a = 0\nif True:\n\tprint(a)\n\tif False:\n\t\ta = 0\n\telse:\n\t\ta = 2\nelse:\n\ta = 1',
-         ['overwritten_variable'], []],
-
-    # TODO: This test case still fails! Investigate why, it's something quite complex.
-    'take_pattern':
-        ['def take(l):\n'
-         ' t=True\n'
-         ' r=[]\n'
-         ' for i in l:\n'
-         '  if i==".":\n'
-         '    t=False\n'
-         '  elif t:\n'
-         '    r.append(i)\n'
-         ' return r\n'
-         'take([1,2,3, ".", 5, 6])', ['unused_variable', 'possible_initialization_problem', 'initialization_problem'], []],
-
-    # TODO: This test case still fails! Investigate why, it's something quite complex.
-    'possibly_overwritten_in_elif_branch':
-        ['highest = 0\nfor score in [1,2]:\n    if False:\n        pass\n    elif False:\n        pass\n    else:\n        highest = 0\nhighest',
-         ['possible_initialization_problem'], []],
-
-    'andy_overwritten_in_elif_branch':
-    ['from rates import bill_small,bill_medium,bill_large\n# do not delete the above line\nfrom cisc106 import assert_equal\n\ndef total_bill(data,base):\n    ''\n    if data < 100:\n        bill= bill_small(data,base)\n        return bill\n    elif data <= 1000 and data>100:\n        return bill_medium(data,base)\n    elif data > 1000:\n        bill = bill_large(data,base)\n        return float(bill)\n\nassert_equal(total_bill(30,80.),80.)\nassert_equal(total_bill(150,80.),95.5)\nassert_equal(total_bill(3000,80.0),160.)',
-     ['possible_initialization_problem'], []],
-
-    # Iterating over the result of a builtin
-    'print_range':
-        ['x = range(100)\nprint(x)', ['iterating_over_non_list'], []],
-    'iterate_range':
-        ['x = range(100)\nfor y in x:\n    print(y)', ['iterating_over_non_list'], []],
-    'iterate_over_ranges_atomic_subtype':
-        ['x = range(100)\nfor y in x:\n    pass\nfor z in y:\n    print(z)', [], ['iterating_over_non_list']],
-    'iterate_over_split':
-        ['for x in "a,b,c".split(","):\n  x+""', ['iterating_over_non_list', 'iterating_over_empty_list'], []],
-    'iterate_over_string_upper':
-        ['for l in "abc".upper():\n  l+""', ['iterating_over_non_list', 'iterating_over_empty_list'], []],
-
-    # incompatible_types
-    'add_int_str':
-        ['a = 5 + "ERROR"', [], ['incompatible_types']],
-    'multiply_str_int':
-        ['a = "ERROR" * 5', ['incompatible_types'], []],
-    'unary_and_sub_int_int':
-        ['-(5)+0', ['incompatible_types'], []],
-    'simple_unary_op':
-        ['+1', ['incompatible_types'], []],
-    'unary_compare':
-        ['-1 < 5', ['incompatible_types'], []],
-    'iadd_int_int':
-        ['a=0\na+=5\na', ['incompatible_types', 'unused_variable', 'initialization_problem', 'overwritten_variable'],
-         []],
-    'iadd_str_int':
-        ['a=""\na+=5\na', ['unused_variable', 'initialization_problem', 'overwritten_variable'],
-         ['incompatible_types']],
-    'iadd_undefined':
-        ['a+=5\na', ['unused_variable', 'overwritten_variable'], ['initialization_problem']],
-    'iadd_unread':
-        ['a=0\na+=5', ['initialization_problem', 'overwritten_variable'], ['unused_variable']],
-    'string_in_string':
-        ['"" in ""', ['incompatible_types'], []],
-    "string_in_tuple_str":
-        ['"" in ("", "")', ['incompatible_types'], []],
-    "string_in_int":
-            ['"" in 5', [], ['incompatible_types']],
-    "string_in_tuple_int":
-        ['"" in (5, 4)', [], ['incompatible_types']],
-    "string_var_in_tuple_strings":
-        ['food = "fruitless"\nfood in ("apple", "banana")', ['incompatible_types'], []],
-    "iter_string_var_in_tuple_string":
-        ['x = [""]\nfor y in x:\n y in ("", "")', ['incompatible_types'], [] ],
-    "iter_int_var_in_tuple_int":
-        ['x = [5]\nfor y in x:\n y in (3,)', ['incompatible_types'], [] ],
-    "iter_int_var_in_tuple_string":
-        ['x = [4]\nfor y in x:\n y in ("", "")', [], ['incompatible_types'] ],
-
-    # Lambda
-    'lambda_add':
-        ['a = lambda: 0\nb=a()\nb+5', ['incompatible_types'], []],
-
-    # Handle function definitions
-    'uncalled_function':
-        ['def named(x):\n\tprint(x)\n', ['initialization_problem'], ['unused_variable']],
-    'called_int_function':
-        ['def int_func(x):\n\treturn 5\nint_func(10)', [], []],
-    'called_constant_function':
-        ['def x():\n    return 4\nx()', ['unused_variable'], []],
-    'overwritten_parameter':
-        ['def x(v):\n  v = 0\n  return v\nx()', [], ['overwritten_variable']],
-    'overwritten_variable_in_function':
-        ['def x():\n  v = 0\n  v = 7\n  return v\nx()', [], ['overwritten_variable']],
-    # Actions after returning
-    'return_after_return':
-        ['def x():\n    return 5\n    return 4\nx()', [], ['action_after_return']],
-    'action_after_return_on_both_branches':
-        ['def x():\n  if True:\n    return 4\n  else:\n    return 3\n  a = 0\n  print(a)\nx()', [],
-         ['action_after_return']],
-    # Function with subtypes
-    'function_with_subtypes_add_int_list_int':
-        ['def add_first(a_list):\n    for element in a_list:\n        return element + 5\nprint(add_first([1]))',
-         ['incompatible_types'], []],
-    'function_with_subtypes_add_int_list_str':
-        ['def add_first(a_list):\n    for element in a_list:\n        return element + 5\nprint(add_first(["1"]))', [],
-         ['incompatible_types']],
-    'function_with_subtypes_add_int_primitive_int':
-        ['def add_first(a_list):\n    for element in a_list:\n        return element + 5\nprint(add_first(1))', [],
-         ['iterating_over_non_list']],
-    'function_with_subtypes_add_int_primitive_str':
-        ['def add_first(a_list):\n    for element in a_list:\n        return element + 5\nprint(add_first("1"))', [],
-         ['incompatible_types']],
-    # Out of scope
-    'read_out_of_scope':
-        ['def x(parameter):\n    return parameter\nx(0)\nparameter', [], ['read_out_of_scope']],
-    'read_inside_of_scope':
-        ['def x(parameter):\n    return parameter\nx(0)', ['read_out_of_scope'], []],
-    'read_not_out_of_scope':
-        ['def x():\n    if 1:\n        y=0\n    else:\n        y=1\n    y\nx()\nx()', ['read_out_of_scope'], []],
-
-    # Function with annotations
-    'annotated_parameters_correct':
-        ['def x(n: int):\n    1+n\nx(5)', ['parameter_type_mismatch', 'incompatible_types'], []],
-    'annotated_parameters_wrong_argument':
-        ['def x(n: int):\n    1+n\nx("5")', [], ['parameter_type_mismatch']],
-    'annotated_parameters_wrong_parameter':
-        ['def x(n: int):\n    "1"+n\nx(5)', [], ['incompatible_types']],
-    'annotated_parameters_append_list':
-        ['def x(l: list):\n    l.append(1)\nx([])', ['parameter_type_mismatch', 'incompatible_types'], []],
-    'annotated_returns_int':
-        ['def x()->int:\n    return "Wrong"\nx()', [], ['multiple_return_types']],
-    'annotated_returns_list_int':
-        ['def x()->[int]:\n    return [1,2,3]\nx().append(4)', ['multiple_return_types', 'incompatible_types'], []],
-
-    'append_to_empty_list':
-        ['a = []\na.append(1)\nprint(a)', ['initialization_problem', 'unused_variable'], []],
-    'append_to_non_empty_list':
-        ['a = [1]\na.append(1)\nprint(a)', ['initialization_problem', 'unused_variable'], []],
-    'append_to_undefined':
-        ['a.append(1)\nprint(a)', ['unused_variable'], ['initialization_problem']],
-    'append_to_unread':
-        ['a=[]\na.append(1)', ['initialization_problem'], ['unused_variable']],
-    'append_to_number':
-        ['a=1\na.append(1)\nprint(a)', [], ['append_to_non_list']],
-
-    'append_and_index':
-        ['x=[]\nx.append(1)\nx[0]+1', ['incompatible_types'], []],
-    'indexing_used':
-        ['mag1 = 0\nmercalli = [0]\nmag1 = mercalli[mag1]\nmag1',
-         ['initialization_problem', 'unused_variable', 'overwritten_variable'], []],
-
-    'created_list_but_unread':
-        ['old = [1,2,3]\nnew=[]\nfor x in old:\n\tnew.append(x)', [], ['unused_variable']],
-    'created_list_but_undefined':
-        ['old = [1,2,3]\nfor x in old:\n\tnew.append(x)\nprint(new)', [], ['initialization_problem']],
-
-    'builtin_float_converter':
-        ['a = float(5)\nb = "test"\nprint(a+b)', [], ['incompatible_types']],
-
-    # Double iteration
-    'iterate_over_list_of_tuples':
-        ['for x,y in [(1,2), (3,4)]:\n    x, y', ['initialization_problem'], []],
-    'iterate_over_items':
-        ['record = {"A": 5, "B": 6}\nfor x,y in record.items():\n    x, y', ['initialization_problem'], []],
-    'iterate_over_items_add':
-        ['record = {"A": 5, "B": 6}\nfor x,y in record.items():\n    x+"", y+0',
-         ['initialization_problem', "incompatible_types"], []],
-
-    # Tuple, Multiple Assignment
-    'multiple_assignment': ['a,b = 1,2\n1+a\nb', ['incompatible_types'], []],
-    'tuple_index': ['tuple_box = (6, 8, 4)\nprint(tuple_box[0])', [], []],
-
-    # Sets
-    'set_creation': ['a = set([1,2,3])\nprint(a)', ['initialization_problem'], []],
-    'set_addition': ['a = {"dog"}\na+"cat"', [], ['incompatible_types']],
-    'set_union_good': ['a = {"dog"}\na|{"cat"}', ['incompatible_types'], []],
-    'set_union_bad': ['a = {"dog"}\na|"cat"', [], ['incompatible_types']],
-
-    # Dictionaries
-    'set_key_in_dict': ['a = {}\na[1] = 0', [], []],
-    'use_key_in_dict': ['a = {"x": 5, "y": "T"}\na["x"]+5', ['incompatible_types'], []],
-    'use_key_in_lod': ['x=[{"a": 0, "b": True}, {"a": 1, "b": False}]\ny=x[0]\nz=y["a"]+0', ['incompatible_types'], []],
-    'use_chained_key_in_lod': ['x=[{"a": 0, "b": True}, {"a": 1, "b": False}]\nnot x[1]["b"]', ['incompatible_types'],
-                               []],
-    'iterate_over_lod': ['ls=[{"a": 0, "b": True}, {"a": 1, "b": False}]\nfor x in ls:\n    x["a"]+0',
-                         ['incompatible_types'], []],
-    # TODO: Add stronger assertion this one, it shouldn't be a good one
-    'incorrect_dict_iteration': ['dict = {"T": "V"}\nfor key,value in dict:\n    print(key)', [], []],
-    'incorrect_dict_iteration2': ['dict = {"T": 0}\nfor i in dict:\n print(i, dict[i])', [], []],
-
-    # Record type
-    'record_type_simple': [
-        ('Dog = {"Name": str, "Age": int, "Fluffy": bool}\n'
-         'def do_stuff(a_dog: Dog) -> Dog:\n'
-         '    a_dog["Name"]+""\n'
-         '    a_dog["Age"] = a_dog["Age"]+5\n'
-         '    return a_dog\n'
-         'ada = {"Name": "Ada", "Age": 2, "Fluffy": True}\n'
-         'do_stuff(ada)["Name"] + ""'
-         ), ['incompatible_types'], []
-    ],
-    'dict_with_setter': [
-        ('person1={"Name": "Babbage", "Age": 3}\n'
-            'def make_older(a_dog: dict) -> int:\n'
-            '    a_dog["Age"]+=1\n'
-            '    return a_dog["Age"]\n'
-            'make_older(person1) + 0'), ['incompatible_types', 'type_changes'], []
-    ],
-    'function_returns_typed_dict': [
-        ('def count_words(words: str) -> {str: int}:\n'
-         '  counts = {}\n'
-         '  for word in words.split(","):\n'
-         '    if word not in counts:\n'
-         '      counts[word] = 0\n'
-         '    counts[word] += 1\n'
-         '  return counts\n'
-         'count_words("alpha,alpha,beta,alpha")'), ['multiple_return_types'], []
-    ],
-    'record_type_in_list': [
-        ('Test = {"a": str}\n'
-         'def x(y: [Test]):\n'
-         '  return y[0]["a"]\n'
-         'x([{"a": "apple"}])'),
-         ['Parameter Type Mismatch'], []
-    ],
-
-    # While
-    'while_until_input': [
-        'user = input("Give a word.")\nwhile user:\n    print(user)\n    user = input("Give another word.")',
-        ['unused_variable'], []],
-
-    # With
-    'with_open':
-        ['with open("A") as a:\n    print(a)', ['initialization_problem'], []],
-
-    # List comprehensions
-    'list_comprehension':
-        ['a = [5 for x in range(100)]\nfor i in a:\n    5+i', ['iterating_over_non_list', 'incompatible_types'], []],
-
-    # return_outside_function
-    'no_return_outside_function':
-        ['def x():\n    return 5\nx()', ['return_outside_function'], []],
-    'return_outside_function':
-        ['def x():\n    pass\nreturn 5\nx()', [], ['return_outside_function']],
-
-    # Classes
-    'class_definition':
-        [
-            'class A:\n    y = 0\n    def __init__(self, x):\n        self.x = 0\n        self.test()\n    def test(self):\n        self.x = 5\nA()',
-            [], []],
-    'instance_assignment':
-        ['class A:\n pass\na = A()\na.b = 0\nb', [], ['initialization_problem']],
-    'instance_assignment_alt':
-        ['class A:\n pass\na = A()\na.b = 0\na.b', ['initialization_problem'], []],
-    'constructor_assignment':
-        ['class A:\n def __init__(self):\n  self.x=0\na=A()\na.x+""', [], ['incompatible_types']],
-    'parameterized_constructor_assignment':
-        [dedent("""
-                class A:
-                    def __init__(self, f):
-                        self.y = f
-                a = A(7)
-                a.y + ''"""), [], ['incompatible_types']],
-    'complex_destructuring':
-        [dedent("""
-                class Player:
-                    def __init__(self):
-                        self.health = 100
-                class World:
-                    def __init__(self):
-                        self.p = Player()
-                w = World()
-                w.p.health, w.p = (5, Player())
-                """), ['incompatible_types'], []],
-    'class_type_promotion':
-        [dedent("""
-                class Enemy:
-                    def __init__(self):
-                        self.health = 0
-                class Player:
-                    def __init__(self):
-                        self.enemies = []
-                class World:
-                    def __init__(self):
-                        self.p = Player()
-                w = World()
-                w.p.enemies.append(Enemy())
-                w.p.enemies[0].health + 100
-                """), ['incompatible_types'], []],
-
-    # Mutable Types
-    'mutable_list_in_function':
-        ['def t():\n    x = []\n    x.append(1)\n    return x\nfor x in t():\n    x + 1', ['incompatible_types'], []],
-    # Importing
-    'import_matplotlib':
-        ['import matplotlib.pyplot as plt\nplt.hist([1,2,3])\nplt.show()', ['initialization_problem'], []],
-    'import_random':
-        ['from random import randint\na=randint(1,2)\n1+a', ['initialization_problem', 'incompatible_types'], []],
-
-    'import_state_demographics':
-        [
-            "import state_demographics\n\n\nincome_list = state_demographics.get(\"Per Capita Income\",\"(None)\",'')\nfilter_income = []\nfor income in income_list:\n    if income > 28000:\n        income_list.append(filter_income)\nprint(filter_income)\n",
-            [], []],
-    'import_state_demographics2':
-        [
-            "import state_demographics\n\n\nincome_list = state_demographics.get(\"Per Capita Income\",\"(None)\",'')\nnew_income_list = 0\nfor income in income_list:\n    if income > 28000:\n        new_income_list = new_income_list + 1\nprint(new_income_list)\n",
-            [], []],
-    'filter_pattern':
-        ['l = []\nfor x in l:\n    if x > 0:\n        x', [], []],
-    'append_iter_var_to_list':
-        ['x = []\nx.append(x)\nx', [], []],
-    'append_multiple_types':
-        ['x = []\nx.append(7)\nx.append("F")\nx', [], ['type_change_append']],
-    'bad_append_iter_var_to_list':
-        ['x = []\nx.append(x)\nx.append(7)\nx', [], ['type_change_append']],
-    'function_with_parameter':
-        ['def x(y):\n    y\nx()', [], []],
-    'function_returns_None':
-        ['def x():\n    return\nx()', [], []],
-    'mutually_recursive_call':
-        ['def y():\n    x()\ndef x():\n    y()\nx()', [], ['recursive_call']],
-    'recursive_call':
-        ['def x():\n    x()\nx()', [], ['recursive_call']],
-    'overwritten_double_nested_branch':
-        ['b= 0\nif True:\n    if True:\n        b=0\nb', ['possible_initialization_problem'], []],
-    # Overwritten in one branches
-    'overwritten_in_one_branch_alt':
-        ['a = 0\nif True:\n\ta = 1\na', ['possible_initialization_problem'], []],
-    'filter_pattern2':
-        ["t = 0\nfor x in []:\n    if x:\n        t = t + 1\nprint(t)", ['possible_initialization_problem'], []],
-    'read_out_scope2':
-        ["x = ''\ndef y():\n    return x\ny()", ['unused_variable'], []],
-
-    'read_out_scope_double_branch':
-        ["def x():\n  if True:\n    y=0\n  else:\n    y=1\n  y\nx()",
-         ['unused_variable', 'read_out_of_scope'], []],
-
-    # Calling functions from within functions
-    'call_function_within_function':
-        ['def z():\n     return b\ndef y():\n    b = 0\n    z()\n    return b\ndef x():\n    y()\nx()',
-         ['unused_variable'], ['read_out_of_scope']],
-
-    # While loop with possibly unused body
-    'while_body_and_conditional_uses_variable':
-        ['a = 10\nwhile a:\n    a -= 1', ['unused_variable'], []],
-    'while_body_uses_variable':
-        ['a = 10\nwhile True:\n    a -= 1', [], ['unused_variable']],
-    'while_body_possibly_defines_variable':
-        ['while True:\n    a=0\na', [], ['possible_initialization_problem']],
-    'while_body_defined_variable':
-        ['a=0\nwhile True:\n    a=0\na', ['possible_initialization_problem'], []],
-
-    # Generators
-    'add_list_to_list_comprehension':
-        ['[1]+[a for a in [1,2,3]]', ['unused_variable', "incompatible_types"], []],
-    'add_set_to_set_comprehension':
-        ['{4}+{a for a in [1,2,3]}', ['unused_variable'], ["incompatible_types"]],
-    'union_set_to_set_comprehension':
-        ['{4}|{a for a in [1,2,3]}', ['unused_variable', "incompatible_types"], []],
-    'int_membership_in_dictionary':
-        ['3 in {a:a for a in [1,2,3]}', ['unused_variable', "incompatible_types"], []],
-    'int_membership_in_comprehension':
-        ['4 in (a for a in [1,2,3])', ['unused_variable', "incompatible_types"], []],
-
-    'prevent_empty_iteration_in_appended_list':
-        ['eles = [1,2,3]\nx = []\nfor ele in eles:\n    x.append(ele)\nfor e2 in x:\n    e2+1',
-         ['iterating_over_empty_list'], []],
-
-    'prevent_empty_iteration_dict':
-        ['x={"A":5}\nfor y in x:\n y', ['iterating_over_empty_list'], []],
-    
-    # Slices
-    'function_call_in_slice':
-        ['def x(): return 2\n"TEST"[:x()]', ['unused_variable'], []],
-
-    # Built-in modules
-    'import_string_letters':
-        ['import string\nstring.letters+""', ['incompatible_types'], []],
-
-    # Nested function definitions
-    'function_nested_inside_if':
-        ['if False:\n  def x():\n    pass', [], ['nested_function_definition']],
-    'function_toplevel':
-        ['def x():\n  if False:\n    pass', ['nested_function_definition'], []],
-    'no_function_whatsoever':
-        ['if False:\n  pass', ['nested_function_definition'], []],
-    'unused_result_function':
-        ['abs(-5)', [], ['unused_returned_value']],
-    'unused_result_method':
-        ['"".strip()', [], ['unused_returned_value']],
-    'unused_result_custom_function':
-        ['def x(): return 7\nx()', [], ['unused_returned_value']],
-    'used_result_custom_function':
-        ['def x(): return 7\nprint(x())', ['unused_returned_value'], []],
-    'used_result_function':
-        ['print(abs(-5))', ['unused_returned_value'], []],
-
-    # Reused variable in outer scope
-    'function_reused_outer_variable_write':
-        ['def y(b): return b+"!"\ndef x(a): return y(a)+"?"\na="Hi"\nx(a)',
-         ['write_out_of_scope'], []],
-
-    # Dictionary stuff
-    'dictionary_literal_key_access_int':
-        ['person = {"Name": "Charles", "Age": 4}\nperson["Age"] + 1',
-         ['incompatible_types'], []],
-    'dictionary_literal_key_access_int_bad':
-        ['person = {"Name": "Charles", "Age": 4}\nperson["Age"] + "1"',
-         [], ['incompatible_types']],
-    'dictionary_literal_key_access_str':
-        ['person = {"Name": "Charles", "Age": 4}\nperson["Name"] + 1',
-         [], ['incompatible_types']],
-    'dictionary_literal_key_access_str_bad':
-        ['person = {"Name": "Charles", "Age": 4}\nperson["Name"] + "1"',
-         ['incompatible_types'], []],
-
-    # Enumerate
-    'enumerate_function_in_function':
-        ['def do_it(data):\n    v = 0\n    for i, _ in enumerate(data):\n        v += i\n    return v\ndo_it("ab")',
-         ['unused_variable'], []]
-}
-
-
-class TestCode(unittest.TestCase):
-    pass
-
-
-SILENCE_EXCEPT = 'enumerate_function_in_function' # 'possibly_overwritten_in_elif_branch' # None  # 'read_not_out_of_scope'
-
-
-def make_tester(internal_name, code, nones, somes):
-    def test_code(self):
-        contextualize_report(code)
-        tifa = pedal.tifa.Tifa()
-        try:
-            result = tifa.process_code(code)
-        except Exception as e:
-            raise type(e)(str(e) +
-                          ' in code:\n%s' % code)
-        if not result.success:
-            traceback.print_tb(result.error.__traceback__)
-            #self.fail("Error message in\n" + code + "\n" +
-            #          str(result.error))
-            self.fail(f"Error occurred: {str(result.error)}\nName: {internal_name}\n----\n{code}\n----\n")
-        for none in nones:
-            if result.issues.get(none, []):
-                print("")
-                pprint(result.variables)
-                self.fail(f"Incorrectly detected `{none}`\nName: {internal_name}\n----\n{code}\n----\n")
-        for some in somes:
-            if not result.issues.get(some, []):
-                self.fail(f"Failed to detect `{some}`\nName: {internal_name}\n----\n{code}\n----\n")
-    test_code.__name__ = "test_code_"+str(internal_name)
-    return test_code
-
-
-for name, (code, nones, somes) in unit_tests.items():
-    if SILENCE_EXCEPT in (None, "None") or SILENCE_EXCEPT == name:
-        setattr(TestCode, 'test_code_{}'.format(name), make_tester(name, code, nones, somes))
-
-
-class TestVariables(unittest.TestCase):
-    def test_type_comparisons(self):
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code('my_int=0\nmy_str="A"\nmy_list=[1,2,3]')
-        variables = result.top_level_variables
-        self.assertEqual(len(variables), 3)
-        # Integer variable
-        my_int = variables['my_int'].type
-        self.assertTrue(my_int.is_equal('num'))
-        self.assertTrue(my_int.is_equal('NumType'))
-        self.assertTrue(my_int.is_equal(int))
-        self.assertFalse(my_int.is_equal(float))
-        self.assertFalse(my_int.is_equal(str))
-        # String variable
-        my_str = variables['my_str'].type
-        self.assertTrue(my_str.is_equal('str'))
-        self.assertTrue(my_str.is_equal('StrType'))
-        self.assertTrue(my_str.is_equal(str))
-        # List variable
-        my_list = variables['my_list'].type
-        self.assertTrue(my_list.is_equal('list'))
-        self.assertTrue(my_list.is_equal('ListType'))
-        self.assertTrue(my_list.is_equal(list))
-        # List subtype
-        self.assertTrue(my_list.element_type.is_equal(int))
-        self.assertTrue(my_list.element_type.is_equal('num'))
-        self.assertFalse(my_list.element_type.is_equal(float))
-        self.assertTrue(my_list.element_type.is_equal('NumType'))
-
-    def test_variable_def_use(self):
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code('a=0\nb=0\nb\nc')
-        issues = result.issues
-        # Unused variables
-        self.assertEqual(len(issues['unused_variable']), 1)
-        unused_variables = [i.fields['name'] for i in issues['unused_variable']]
-        self.assertIn('a', unused_variables)
-        self.assertNotIn('b', unused_variables)
-        self.assertNotIn('c', unused_variables)
-        # Uninitalized variables
-        self.assertEqual(len(issues['initialization_problem']), 1)
-        unset_variables = [i.fields['name'] for i in issues['initialization_problem']]
-        self.assertNotIn('a', unset_variables)
-        self.assertNotIn('b', unset_variables)
-        self.assertIn('c', unset_variables)
-
-    def test_weirdness_used_function(self):
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code('def a(x):\n    return x\na(1)')
-        self.assertTrue(result.success)
-
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code('def a(x):\n    return x\n')
-        issues = result.issues
-        self.assertEqual(issues['unused_variable'][0].message,
-                         "The function a was "
-                         "given a definition on line 1, but was never used "
-                         "after that.")
-
-    def test_bad_parameter_found(self):
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code('def a(x: int):\n    return x\na("hello")')
-        issues = result.issues
-        self.assertEqual(issues['parameter_type_mismatch'][0].message,
-                         "You defined the parameter x as an integer. However, the argument passed to that parameter on line 3 was a string. The formal parameter type must match the argument's type.")
-
-    def test_bad_parameter_found_complex(self):
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code('def a(x: list[int]):\n    return x\na(5)')
-        issues = result.issues
-        self.assertEqual(issues['parameter_type_mismatch'][0].message,
-                         "You defined the parameter x as a list of integers. However, the argument passed to that parameter on line 3 was an integer. The formal parameter type must match the argument's type.")
-
-    def test_weirdness_tate_import_example(self):
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(dedent('''
-        import tate
-        art = tate.get_artwork()
-        h = [a['dimensions']['height'] for a in art if a['artist']['birth']['year'] > 1000]
-        b = [a['artist']['birth']['year'] for a in art 
-             if a['artist']['birth']['year'] > 1000]
-        import matplotlib.pyplot as plt
-        plt.scatter(b, h, alpha=.1)
-        plt.show()'''))
-        self.assertTrue(result.success)
-
-    '''
-    def test_tifa_graceful_errors(self):
-        student_code = '1 + "Banana"'
-        set_source(student_code)
-        exception = commands.run_student()
-        self.assertIsNotNone(exception)'''
-
-    def test_json_types(self):
-        t = normalize.get_pedal_type_from_json({'type': 'NumType'})
-        self.assertIsInstance(t, defs.NumType)
-        t = normalize.get_pedal_type_from_json({'type': 'StrType'})
-        self.assertIsInstance(t, defs.StrType)
-        t = normalize.get_pedal_type_from_json({'type': 'BoolType'})
-        self.assertIsInstance(t, defs.BoolType)
-        t = normalize.get_pedal_type_from_json({'type': 'NoneType'})
-        self.assertIsInstance(t, defs.NoneType)
-        t = normalize.get_pedal_type_from_json({'type': 'ListType',
-                                 'subtype': {'type': 'NumType'}})
-        self.assertIsInstance(t, defs.ListType)
-        self.assertIsInstance(t.element_type, defs.NumType)
-
-        l1 = {'type': 'LiteralStr', 'value': 'First'}
-        l2 = {'type': 'LiteralStr', 'value': 'Second'}
-        v1, v2 = {'type': 'StrType'}, {'type': 'NumType'}
-        t = normalize.get_pedal_type_from_json({'type': 'DictType', 'literals': [l1, l2],
-                                 'values': [v1, v2]})
-        self.assertIsInstance(t, defs.DictType)
-        self.assertIsInstance(t.element_types, list)
-        self.assertEqual(len(t.element_types), 2)
-        self.assertIsInstance(t.element_types[0][0], defs.LiteralStr)
-        self.assertEqual(t.element_types[0][0].value, 'First')
-        self.assertIsInstance(t.element_types[1][0], defs.LiteralStr)
-        self.assertEqual(t.element_types[1][0].value, 'Second')
-        self.assertIsInstance(t.element_types, list)
-        self.assertEqual(len(t.element_types), 2)
-        self.assertIsInstance(t.element_types[0][1], defs.StrType)
-        self.assertIsInstance(t.element_types[1][1], defs.NumType)
-
-        # Try to parse the Broadway type definition
-        complex_type = {"type": "ModuleType",
-                        "fields": {
-                            'get': {"type": "ListType", "empty": False,
-                                    "subtype": {"type": "NumType"}},
-
-                            'get_shows':
-                                {"type": "ListType", "subtype":
-                                    {"type": "DictType", "literals": [{"type": "LiteralStr", "value": 'Statistics'},
-                                                                      {"type": "LiteralStr", "value": 'Show'},
-                                                                      {"type": "LiteralStr", "value": 'Date'}],
-                                     "values": [
-                                         {"type": "DictType", "literals": [{"type": "LiteralStr", "value": 'Capacity'},
-                                                                           {"type": "LiteralStr",
-                                                                            "value": 'Attendance'},
-                                                                           {"type": "LiteralStr",
-                                                                            "value": 'Performances'},
-                                                                           {"type": "LiteralStr", "value": 'Gross'},
-                                                                           {"type": "LiteralStr",
-                                                                            "value": 'Gross Potential'}], "values": [
-                                             {"type": "NumType"},
-                                             {"type": "NumType"},
-                                             {"type": "NumType"},
-                                             {"type": "NumType"},
-                                             {"type": "NumType"}]},
-                                         {"type": "DictType", "literals": [{"type": "LiteralStr", "value": 'Type'},
-                                                                           {"type": "LiteralStr", "value": 'Theatre'},
-                                                                           {"type": "LiteralStr", "value": 'Name'}],
-                                          "values": [
-                                              {"type": "StrType"},
-                                              {"type": "StrType"},
-                                              {"type": "StrType"}]},
-                                         {"type": "DictType", "literals": [{"type": "LiteralStr", "value": 'Day'},
-                                                                           {"type": "LiteralStr", "value": 'Month'},
-                                                                           {"type": "LiteralStr", "value": 'Year'},
-                                                                           {"type": "LiteralStr", "value": 'Full'}],
-                                          "values": [
-                                              {"type": "NumType"},
-                                              {"type": "NumType"},
-                                              {"type": "NumType"},
-                                              {"type": "StrType"}]}]}},
-
-                        }}
-        normalize.get_pedal_type_from_json(complex_type)
-
-    def test_custom_module_import_weather(self):
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code('import weather\n' +
-                          'rs = weather.get_weather()\n' +
-                          'for r in rs:\n' +
-                          '  0+r["Data"]["Precipitation"]',
-                                   filename='student.py')
-        self.assertTrue(result.success)
-        self.assertNotIn('module_not_found', result.issues)
-
-    def test_custom_module_import_police(self):
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code('import police_shootings\n'
-                          'rs = police_shootings.get_shootings()\n'
-                          'for r in rs:\n'
-                          '  x=0+r["Person.Age"]\n'
-                          'x', filename='student.py')
-        self.assertTrue(defs.is_subtype(result.top_level_variables['x'].type, defs.NumType()))
-        self.assertTrue(result.success)
-        self.assertNotIn('module_not_found', result.issues)
-
-    def test_custom_module_import_babbages(self):
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code('import babbages\n'
-                          'print(babbages)', filename='student.py')
-        self.assertIn('module_not_found', result.issues)
-
-    def test_custom_module_import_broadway(self):
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(dedent("""
-            import broadway
-            report_list = broadway.get_shows()
-            total= 0
-            for broadway in report_list:
-                if broadway ["Show"]["Type"] == "Musical":
-                    total = total + 1
-            print(total)"""), filename='student.py')
-        self.assertTrue(result.success)
-        self.assertNotIn('module_not_found', result.issues)
-
-    def test_get_types(self):
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code('a=0\na="Hello"\na=[1,2,3]\na=1')
-        a = result.top_level_variables['a']
-        self.assertTrue(a.was_type('num'))
-        self.assertTrue(a.was_type(int))
-        self.assertTrue(a.was_type('NumType'))
-        self.assertTrue(a.was_type(defs.NumType))
-        self.assertFalse(a.was_type(bool))
-        self.assertFalse(a.was_type(defs.DictType))
-        self.assertTrue(a.was_type('ListType'))
-
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code('credits=[1,2,3,4]\nfor credit in credits:\n  print(credit)')
-        credit = result.top_level_variables['credit']
-        self.assertFalse(credit.was_type(list))
-        self.assertTrue(credit.was_type(int))
-
-    def test_dict_iteration(self):
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code('dict = {"T": 0}\nfor i in dict:\n    print(i, dict[i])')
-        self.assertTrue(result.success)
-
-    def test_classes(self):
-        program = 'class A:\n def __init__(self):\n  self.x=0\na=A()\na.x+""'
-        # print(indent(program, '    '))
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program)
-        # self.assertTrue(tifa.report['tifa']['success'])
-        # pprint(tifa.report['tifa'])
-        # print(tifa.report['tifa']['top_level_variables']['a'].type.parent.fields)
-        self.assertFalse(result.error)
-
-        program = dedent("""
-                class Enemy:
-                    def __init__(self):
-                        self.health = 0
-                class Player:
-                    def __init__(self):
-                        self.enemies = []
-                class World:
-                    def __init__(self):
-                        self.p = Player()
-                w = World()
-                w.p.enemies.append(Enemy())
-                w.p.enemies[0].health + 100
-                """)
-        tifa = pedal.tifa.Tifa()
-        tifa.process_code(program)
-        # pprint(tifa.report['tifa'])
-    
-    def test_locations(self):
-        program = dedent("""
-                a = 0
-                "Ignore"
-                "This"
-                "Line"
-                def unnecessary():
-                    pass
-                unnecessary
-                """)
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program)
-        self.assertEqual(result.issues['unused_variable'][0].location.line, 2)
-
-
-    def test_weird_indexing_behavior(self):
-        program = dedent("""
-        movie_list = [{'Title':'Iron Man', 'Release Date':'May 2, 2008','Budget':'140','Running Time':'126'},
-              {'Title':'Iron Man 2', 'Release Date':'May 7, 2010','Budget':'200', 'Running Time':'125'},
-              {'Title':'Iron Man 3', 'Release Date':'May 3, 2013','Budget':'200', 'Running Time':'130'}]
-        total=0
-        for title in movie_list:
-            total=total + 'title'['Running Time']
-        print(total)
-        """)
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program)
-        #self.assertNotIn('incompatible_types', result.issues)
-        self.assertIn('invalid_indexing', result.issues)
-
-    def test_not_finding_unused_return_value(self):
-        program = dedent("""
-            #import classics
-            import matplotlib.pyplot as plt
-            book_downloads = []
-            #report_list = classics.get_books(test=True)
-            report_list = [{'bibliography': {'type': 'Text'},
-                            'metadata': {'downloads': 0}}]
-            for report in report_list:
-                if report["bibliography"]["type"] == "Text":
-                    book_downloads.append(report["metadata"]["downloads"])
-            plt.hist(book_downloads)
-            plt.ylabel("Number of Books")
-            plt.xlabel("downloads")
-            plt.title("Spreads of Book Downloads")
-            plt.show()
-        """)
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program, filename="student.py")
-        self.assertNotIn('unused_returned_value', result.issues)
-        self.assertFalse(result.issues)
-
-    @unittest.skip("Currently broken, need to increase sophistication of typeddict support")
-    def test_typedict_book(self):
-        program = dedent("""
-            from cisc108 import *
-            class Book(TypedDict):
-                title: str
-                pages: int
-                hardcover: bool
-            
-            def page_count(a_book: Book) -> int:
-                return a_book['pages']
-                
-            hp = {'title': 'Harry Potter',
-                  'pages': 300,
-                  'hardcover': false}
-            
-            assert_equal(page_count(hp), 300)
-        """)
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program, filename="student.py")
-        self.assertFalse(result.issues)
-
-    def test_unnecessary_second_branch(self):
-        program = dedent("""# Remember to initialize the variables!
-age = 20
-has_license = True
-# Keep this If/else structure unchanged, but
-# fill in the blanks with the code above
-if has_license == True:
-    if age >= 21:
-        print("Can drink")
-        if age < 1000:
-            pass
-        else:
-            print("Too old")
-            
-    else:
-        print("Too young")
-        
-else:
-    print("Doesn't have a license")""")
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program, filename="student.py")
-        self.assertTrue(result.issues)
-
-    def test_complex_record_type(self):
-        program = dedent("""
-Test = {"a": str}
-
-def x(y: [Test]):
-    return y[0]['a']
-
-print(x([{"a": "apple"}]))""")
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program, filename="student.py")
-        self.assertFalse(result.issues)
-
-    def test_new_class_record_type(self):
-        program = dedent("""
-        from dataclasses import dataclass
-        
-        @dataclass
-        class Dog:
-            name: str
-            age: int
-            fuzzy: bool
-            
-        def is_fuzzy(a_dog: Dog) -> bool:
-            return a_dog.fuzzy
-            
-        ada = Dog('Ada Bart', 4, True)
-        print(ada.name)
-        
-        print(is_fuzzy(ada))
-        """)
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program, filename="student.py")
-        self.assertFalse(result.issues)
-
-    def test_new_class_record_type_bad_instance(self):
-        program = dedent("""
-        class Dog(record):
-            name: str
-            age: int
-            fuzzy: bool
-
-        def is_fuzzy(a_dog: Dog) -> bool:
-            return a_dog.fuzzy
-
-        ada = Dog('Ada Bart', 4)
-        print(ada.name)
-
-        print(is_fuzzy(ada))
-        """)
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program, filename="student.py")
-        self.assertTrue(result.issues)
-
-    def test_dataclass_mistake(self):
-        program = dedent("""
-        from dataclasses import dataclass
-        
-        @dataclass
-        class Dog:
-            name: str
-            age: int
-            fuzzy: bool
-            
-        @dataclass
-        class Cat:
-            name: str
-            age: int
-            fuzzy: bool
-
-        def is_fuzzy(a_dog: Dog) -> bool:
-            return a_dog.fuzzy
-
-        ada = Dog('Ada Bart', 4, True)
-        print(ada.name)
-
-        print(is_fuzzy(ada))
-        
-        adacat = Cat("Ada Bart", 4, True)
-        print(is_fuzzy(adacat))
-        """)
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program, filename="student.py")
-        self.assertIsNone(result.error)
-        self.assertTrue(result.issues)
-
-    def test_dataclass_mistake_lists(self):
-        program = dedent("""
-        from dataclasses import dataclass
-
-        @dataclass
-        class Dog:
-            name: str
-            age: int
-            fuzzy: bool
-
-        @dataclass
-        class Cat:
-            name: str
-            age: int
-            fuzzy: bool
-
-        def all_fuzzy(dogs: list[Dog]) -> bool:
-            return all(a_dog.fuzzy for a_dog in dogs)
-
-        ada = Dog('Ada Bart', 4, True)
-        print(ada.name)
-
-        print(all_fuzzy([ada]))
-
-        adacat = Cat("Ada Bart", 4, True)
-        print(all_fuzzy([adacat]))
-        """)
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program, filename="student.py")
-        self.assertIsNone(result.error)
-        self.assertTrue(result.issues)
-        self.assertEqual("You defined the parameter dogs as a list of Dog. "
-                         "However, the argument passed to that parameter on line 25 was a list of Cat. "
-                         "The formal parameter type must match the argument's type.",
-                         result.issues['parameter_type_mismatch'][0].message)
-
-    def test_dataclass_bad_constructor_call_order(self):
-        program = dedent("""
-        from dataclasses import dataclass
-
-        @dataclass
-        class Dog:
-            name: str
-            age: int
-            fuzzy: bool
-        
-        ada = Dog('Ada Bart', True, 4)
-        print(ada.name)
-        """)
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program, filename="student.py")
-        self.assertIsNone(result.error)
-        self.assertTrue(result.issues)
-        self.assertEqual("You defined the field age as an integer. However, the argument passed to that field's "
-                         "parameter in the constructor function on line 10 was a boolean. The formal field type "
-                         "must match the argument's type.",
-                         result.issues['field_type_mismatch'][0].message)
-
-    def test_dataclass_bad_constructor_call_arity(self):
-        program = dedent("""
-        from dataclasses import dataclass
-
-        @dataclass
-        class Dog:
-            name: str
-            age: int
-            fuzzy: bool
-
-        ada = Dog('Ada Bart', 4)
-        print(ada.name)
-        """)
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program, filename="student.py")
-        self.assertIsNone(result.error)
-        self.assertTrue(result.issues)
-        self.assertEqual("The constructor function Dog was given the wrong number of arguments. You should have "
-                         "had 3 arguments, but instead you had 2 arguments.",
-                         result.issues['incorrect_arity'][0].message)
-
-    def test_dataclass_bad_constructor_call_extra(self):
-        program = dedent("""
-        from dataclasses import dataclass
-
-        @dataclass
-        class Dog:
-            name: str
-            age: int
-            fuzzy: bool
-
-        ada = Dog('Ada Bart', 4, True, "is cute!")
-        print(ada.name)
-        """)
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(program, filename="student.py")
-        self.assertIsNone(result.error)
-        self.assertTrue(result.issues)
-        self.assertEqual("The constructor function Dog was given the wrong number of arguments. You should have "
-                         "had 3 arguments, but instead you had 4 arguments.",
-                         result.issues['incorrect_arity'][0].message)
-
-    def test_import_second_file(self):
-        main_program = dedent("""
-        import monsters
-        
-        monsters.number + ""
-        """)
-        monster_file = dedent("""number = 7\nalpha = 'test'""")
-        contextualize_report(Submission(files={'student.py': main_program, 'monsters.py': monster_file}))
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(main_program, filename="student.py")
-        self.assertIsNone(result.error)
-        self.assertTrue(result.issues)
-        self.assertEqual("You used an addition operation with an integer and a string on line 4. But you can't do that with that operator. Make sure both sides of the operator are the right type.",
-                         result.issues['incompatible_types'][0].message)
-        self.assertEqual(len(result.issues.get('unused_variable', [])), 0)
-
-    def test_import_second_file_successful(self):
-        main_program = dedent("""
-        from monsters import Monster, dracula
-
-        dracula.name + ""
-        print(Monster("Wolfman"))
-        """)
-        monster_file = dedent("""
-        from dataclasses import dataclass
-        @dataclass
-        class Monster:
-            name: str
-        dracula = Monster('Dracula')""")
-        contextualize_report(Submission(files={'student.py': main_program, 'monsters.py': monster_file}))
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(main_program, filename="student.py")
-        self.assertIsNone(result.error)
-        self.assertFalse(result.issues)
-
-    def test_provide_import_type_definitions(self):
-        main_program = dedent("""
-        import monsters
-
-        monsters.number + ""
-        """)
-        tifa = pedal.tifa.Tifa()
-        tifa_provide_module_type('monsters', {'number': normalize.normalize_type('int')})
-        result = tifa.process_code(main_program, filename="student.py")
-        self.assertIsNone(result.error)
-        self.assertTrue(result.issues)
-        self.assertEqual(
-            "You used an addition operation with an integer and a string on line 4. But you can't do that with that operator. Make sure both sides of the operator are the right type.",
-            result.issues['incompatible_types'][0].message)
-
-    @unittest.skip
-    def test_provide_module_definitions(self):
-        main_program = dedent("""
-        from monsters import dracula
-
-        dracula.age + ""
-        """)
-        tifa = pedal.tifa.Tifa()
-        import tests.test_files.monsters as monsters
-        tifa_provide_module_type('monsters', normalize.normalize_type(monsters))
-        result = tifa.process_code(main_program, filename="student.py")
-        if result.error is not None:
-            raise result.error
-        self.assertIsNone(result.error)
-        self.assertTrue(result.issues)
-        self.assertEqual(
-            "You used an addition operation with an integer and a string on line 4. But you can't do that with that operator. Make sure both sides of the operator are the right type.",
-            result.issues['incompatible_types'][0].message)
-
-    def test_weird_return_control_flow(self):
-        main_program = dedent("""
-        from dataclasses import dataclass
-        
-        @dataclass
-        class Media:
-            name: str
-            kind: str
-            duration: int
-        
-        def longest(media: list[Media]) -> str:
-            movies_only = [i for i in media if i.kind == 'movie']
-            if not movies_only:
-                return 'no movies'
-            key = lambda movie: movie.duration
-            return max(movies_only, key=key).name
-        
-        print(longest([Media("Snoopy", "movie", 5)]))
-        print(longest([]))
-        """)
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(main_program, filename="student.py")
-        if result.error:
-            raise result.error
-        self.assertIsNone(result.error)
-        self.assertFalse(result.issues)
-
-    def test_weird_increment_set_list(self):
-        main_program = dedent("""from dataclasses import dataclass
-
-@dataclass
-class Forecast:
-    reports: list[int]
-    
-def rainfall(weather: list[Forecast]) -> list[int]:
-    reports = []
-    for a_weather in weather:
-        reports += a_weather.reports
-    return reports
-
-def total_rainfall(forecast: list[Forecast]) -> int:
-    total = 0
-    reports = rainfall(forecast)
-    for measurement in reports:
-        total += measurement
-    return total
-
-forecast1 = [Forecast([1,2,3])]
-5+total_rainfall(forecast1)""")
-        tifa = pedal.tifa.Tifa()
-        result = tifa.process_code(main_program, filename="student.py")
-        if result.error:
-            raise result.error
-        self.assertIsNone(result.error)
-        self.assertFalse(result.issues)
-
-if __name__ == '__main__':
-    unittest.main(buffer=False)
+import traceback
+import unittest
+import os
+import sys
+from textwrap import dedent
+from pprint import pprint
+from dataclasses import dataclass
+
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+import pedal.tifa
+import pedal.types.new_types as defs
+import pedal.types.normalize as normalize
+from pedal import contextualize_report, Submission, evaluate
+from pedal.tifa import tifa_provide_module_type
+
+unit_tests = {
+    'add_assign_inside_dataclass_function':
+        ['from dataclasses import dataclass\n@dataclass\nclass X:\n    y: int = 0\ndef inc(z: X):\n    z.y += 1\ninc(X(0))',
+            ['incompatible_types'], []],
+    'assign_inside_dataclass_function':
+        ['from dataclasses import dataclass\n@dataclass\nclass X:\n    y: int = 0\ndef inc(z: X):\n    z.y = 1\ninc(X(0))',
+            ['incompatible_types'], []],
+
+
+    # Function decorator
+    'function_decorator':
+        ['def dec(f):\n    return f\n@dec\ndef x(a: int):\n    return a\nx()', ['unused_variable'], []],
+    'fancy_drafter_route':
+        ['from bakery import assert_equal\nfrom drafter import *\nfrom dataclasses import dataclass\n\n@dataclass\nclass State:\n    cookies: int\n\n@route\ndef cookie(state: State) -> Page:\n    state.cookies += 1\n    return Page(state, [])\n\nassert_equal(\n    cookie(State(cookies=100)),\n    Page(\n        state=State(cookies=101),\n        content=[],\n    ),\n)\n\n#start_server(State(0))\n',
+            ['incompatible_types'], []],
+    'drafter_route':
+        ['from drafter import *\nfrom dataclasses import dataclass\n@dataclass\nclass State: pass\n@route\ndef index(state: State) -> Page:\n    return Page()\nindex(State())',
+            ['initialization_problem'], []],
+
+
+    # Source Code, Shouldn't catch this, Should catch this
+    'builtin_True': ['print(True)', ['initialization_problem'], []],
+    'unread_variable': ['a = 0', [], ['unused_variable']],
+    'undefined_variable': ['print(a)', [], ['initialization_problem']],
+    'defined_read_variable': ['a = 0\nprint(a)', ['initialization_problem'], []],
+    'overwritten_variable': ['a = 0\na = 5', [], ['overwritten_variable']],
+    'unread_variables': ['a = 0\nb = 5', ['overwritten_variable'], ['unused_variable']],
+    'wrwr_variable': ['a = [1]\nprint(a)\na = [1]\nprint(a)', [], []],
+    # unconnected_blocks
+    'unconnected_assign': ['a = ___', [], ['unconnected_blocks']],
+    'unconnected_print': ['print(___)', [], ['unconnected_blocks']],
+
+    'literal_in_call': ['print("dog" in input("test"))', [], []],
+    'wrong_method_for_type': ['[].replace(",","")', [], []],
+
+    "check_true_argument_in_function_call":
+        ['def is_true(x:bool)->bool:\n return x\nis_true(True)', 'parameter_type_mismatch', ''],
+
+    # Double call
+    'double_call': ['def x(a):\n    return a\nx(5)\nx(3)', ['read_out_of_scope'], []],
+
+    # Chained functions
+    'chained_functions': ['def x():\n    return 0\ndef y():\n    x()\ny()',
+                          ['read_out_of_scope', 'initialization_problem'], []],
+
+    # String indexing and slicing
+    'string_indexing_slicing': ['("a"[0] + ""[:])[:][0]', ['incompatible_types'], []],
+    # List indexing and slicing
+    'list_indexing_slicing': ['([0][0] + [1,2,3][:][2])', ['incompatible_types'], []],
+
+    'returned_string':
+        [
+            'def pluralize(a_word):\n    return a_word+"s"\nnoun = pluralize("Dog")\nprint(noun + " can pet other " + noun)',
+            ['incompatible_types'], []],
+    'update_without_read':
+        ['a = 0\na+= 1', ['initialization_problem'], ['unused_variable']],
+    'update_and_read':
+        ['a = 0\na+= 1\nprint(a)', ['initialization_problem', 'unused_variable'], []],
+    'iterate_through_non_existing_list':
+        ['for x in y:\n\tpass', ['unused_variable'], ['initialization_problem']],
+    'iterate_through_list':
+        ['y = [1,2,3]\nfor x in y:\n\tpass', ['unused_variable', 'initialization_problem'], []],
+    'iterate_through_empty_list':
+        ['y = []\nfor x in y:\n\tpass', ['unused_variable', 'initialization_problem'], ['iterating_over_empty_list']],
+    'double_iterate_through_strings':
+        ['ss = ["Testing", "Here"]\nfor a in ss:\n    print(a)\nfor b in a:\n    print(b)',
+         ['iterating_over_non_list', 'iterating_over_empty_list'], []],
+    'iterate_through_number':
+        ['y = 5\nfor x in y:\n\tpass', ['unused_variable', 'initialization_problem'], ['iterating_over_non_list']],
+    'iterate_over_iteration_variable':
+        ['y = [1,2,3]\nfor y in y:\n\tpass', [], ['iteration_problem']],
+    'type_change':
+        ['a = 0\nprint(a)\na="T"\nprint(a)', [], ['type_changes']],
+    'defined_in_if_root_but_not_other':
+        ['if True:\n\ta = 0\nprint(a)', [], ['possible_initialization_problem']],
+    'defined_in_both_branches':
+        ['if True:\n\ta = 0\nelse:\n\ta = 1\nprint(a)', ['possible_initialization_problem'], []],
+    'defined_in_else_root_but_not_other':
+        ['if True:\n\tpass\nelse:\n\ta = 1\nprint(a)', [], ['possible_initialization_problem']],
+    'defined_in_if_branch_but_others':
+        ['if True:\n\tif False:\n\t\ta = 0\nprint(a)', [], ['possible_initialization_problem']],
+    'defined_before_if_branch_but_not_others':
+        ['if True:\n\ta = 0\nif False:\t\tpass\nprint(a)', [], ['possible_initialization_problem']],
+    'defined_after_if_branch_but_not_others':
+        ['if True:\n\tif False:\n\t\tpass\n\ta = 0\nprint(a)', [], ['possible_initialization_problem']],
+    'defined_within_both_if_branches_but_not_others':
+        ['if True:\n\tif False:\n\t\ta=0\n\telse:\n\t\ta = 0\nprint(a)', [], ['possible_initialization_problem']],
+    'defined_in_all_branches':
+        ['if True:\n\tif False:\n\t\ta=0\n\telse:\n\t\ta = 0\nelse:\n\ta=3\nprint(a)',
+         ['possible_initialization_problem'], []],
+    'read_in_if_branch_but_unset':
+        ['if True:\n\tprint(a)', [], ['initialization_problem']],
+    'read_in_else_branch_but_unset':
+        ['if True:\n\tpass\nelse:\n\tprint(a)', [], ['initialization_problem']],
+    'read_in_both_branches_but_unset':
+        ['if True:\n\tprint(a)\nelse:\n\tprint(a)', [], ['initialization_problem']],
+    'overwritten_in_both_branches':
+        ['a = 0\nif True:\n\ta = 0\nelse:\n\ta = 1', [], ['overwritten_variable']],
+    'overwritten_in_one_branch':
+        ['a = 0\nif True:\n\tpass\nelse:\n\ta = 1', ['overwritten_variable'], []],
+    'overwritten_in_inner_branch':
+        ['a = 0\nif True:\n\tif False:\n\t\ta = 0\nelse:\n\ta = 1', ['overwritten_variable'], []],
+    'overwritten_in_all_branch':
+        ['a = 0\nif True:\n\tif False:\n\t\ta = 0\n\telse:\n\t\ta = 2\nelse:\n\ta = 1', [], ['overwritten_variable']],
+    'overwritten_in_all_branches2':
+        ['a = 0\nif True:\n\tprint(a)\n\tif False:\n\t\ta = 0\n\telse:\n\t\ta = 2\nelse:\n\ta = 1',
+         ['overwritten_variable'], []],
+
+    # TODO: This test case still fails! Investigate why, it's something quite complex.
+    'take_pattern':
+        ['def take(l):\n'
+         ' t=True\n'
+         ' r=[]\n'
+         ' for i in l:\n'
+         '  if i==".":\n'
+         '    t=False\n'
+         '  elif t:\n'
+         '    r.append(i)\n'
+         ' return r\n'
+         'take([1,2,3, ".", 5, 6])', ['unused_variable', 'possible_initialization_problem', 'initialization_problem'], []],
+
+    # TODO: This test case still fails! Investigate why, it's something quite complex.
+    'possibly_overwritten_in_elif_branch':
+        ['highest = 0\nfor score in [1,2]:\n    if False:\n        pass\n    elif False:\n        pass\n    else:\n        highest = 0\nhighest',
+         ['possible_initialization_problem'], []],
+
+    'andy_overwritten_in_elif_branch':
+    ['from rates import bill_small,bill_medium,bill_large\n# do not delete the above line\nfrom cisc106 import assert_equal\n\ndef total_bill(data,base):\n    ''\n    if data < 100:\n        bill= bill_small(data,base)\n        return bill\n    elif data <= 1000 and data>100:\n        return bill_medium(data,base)\n    elif data > 1000:\n        bill = bill_large(data,base)\n        return float(bill)\n\nassert_equal(total_bill(30,80.),80.)\nassert_equal(total_bill(150,80.),95.5)\nassert_equal(total_bill(3000,80.0),160.)',
+     ['possible_initialization_problem'], []],
+
+    # Iterating over the result of a builtin
+    'print_range':
+        ['x = range(100)\nprint(x)', ['iterating_over_non_list'], []],
+    'iterate_range':
+        ['x = range(100)\nfor y in x:\n    print(y)', ['iterating_over_non_list'], []],
+    'iterate_over_ranges_atomic_subtype':
+        ['x = range(100)\nfor y in x:\n    pass\nfor z in y:\n    print(z)', [], ['iterating_over_non_list']],
+    'iterate_over_split':
+        ['for x in "a,b,c".split(","):\n  x+""', ['iterating_over_non_list', 'iterating_over_empty_list'], []],
+    'iterate_over_string_upper':
+        ['for l in "abc".upper():\n  l+""', ['iterating_over_non_list', 'iterating_over_empty_list'], []],
+
+    # incompatible_types
+    'add_int_str':
+        ['a = 5 + "ERROR"', [], ['incompatible_types']],
+    'multiply_str_int':
+        ['a = "ERROR" * 5', ['incompatible_types'], []],
+    'unary_and_sub_int_int':
+        ['-(5)+0', ['incompatible_types'], []],
+    'simple_unary_op':
+        ['+1', ['incompatible_types'], []],
+    'unary_compare':
+        ['-1 < 5', ['incompatible_types'], []],
+    'iadd_int_int':
+        ['a=0\na+=5\na', ['incompatible_types', 'unused_variable', 'initialization_problem', 'overwritten_variable'],
+         []],
+    'iadd_str_int':
+        ['a=""\na+=5\na', ['unused_variable', 'initialization_problem', 'overwritten_variable'],
+         ['incompatible_types']],
+    'iadd_undefined':
+        ['a+=5\na', ['unused_variable', 'overwritten_variable'], ['initialization_problem']],
+    'iadd_unread':
+        ['a=0\na+=5', ['initialization_problem', 'overwritten_variable'], ['unused_variable']],
+    'string_in_string':
+        ['"" in ""', ['incompatible_types'], []],
+    "string_in_tuple_str":
+        ['"" in ("", "")', ['incompatible_types'], []],
+    "string_in_int":
+            ['"" in 5', [], ['incompatible_types']],
+    "string_in_tuple_int":
+        ['"" in (5, 4)', [], ['incompatible_types']],
+    "string_var_in_tuple_strings":
+        ['food = "fruitless"\nfood in ("apple", "banana")', ['incompatible_types'], []],
+    "iter_string_var_in_tuple_string":
+        ['x = [""]\nfor y in x:\n y in ("", "")', ['incompatible_types'], [] ],
+    "iter_int_var_in_tuple_int":
+        ['x = [5]\nfor y in x:\n y in (3,)', ['incompatible_types'], [] ],
+    "iter_int_var_in_tuple_string":
+        ['x = [4]\nfor y in x:\n y in ("", "")', [], ['incompatible_types'] ],
+
+    # Lambda
+    'lambda_add':
+        ['a = lambda: 0\nb=a()\nb+5', ['incompatible_types'], []],
+
+    # Handle function definitions
+    'uncalled_function':
+        ['def named(x):\n\tprint(x)\n', ['initialization_problem'], ['unused_variable']],
+    'called_int_function':
+        ['def int_func(x):\n\treturn 5\nint_func(10)', [], []],
+    'called_constant_function':
+        ['def x():\n    return 4\nx()', ['unused_variable'], []],
+    'overwritten_parameter':
+        ['def x(v):\n  v = 0\n  return v\nx()', [], ['overwritten_variable']],
+    'overwritten_variable_in_function':
+        ['def x():\n  v = 0\n  v = 7\n  return v\nx()', [], ['overwritten_variable']],
+    # Actions after returning
+    'return_after_return':
+        ['def x():\n    return 5\n    return 4\nx()', [], ['action_after_return']],
+    'action_after_return_on_both_branches':
+        ['def x():\n  if True:\n    return 4\n  else:\n    return 3\n  a = 0\n  print(a)\nx()', [],
+         ['action_after_return']],
+    # Function with subtypes
+    'function_with_subtypes_add_int_list_int':
+        ['def add_first(a_list):\n    for element in a_list:\n        return element + 5\nprint(add_first([1]))',
+         ['incompatible_types'], []],
+    'function_with_subtypes_add_int_list_str':
+        ['def add_first(a_list):\n    for element in a_list:\n        return element + 5\nprint(add_first(["1"]))', [],
+         ['incompatible_types']],
+    'function_with_subtypes_add_int_primitive_int':
+        ['def add_first(a_list):\n    for element in a_list:\n        return element + 5\nprint(add_first(1))', [],
+         ['iterating_over_non_list']],
+    'function_with_subtypes_add_int_primitive_str':
+        ['def add_first(a_list):\n    for element in a_list:\n        return element + 5\nprint(add_first("1"))', [],
+         ['incompatible_types']],
+    # Out of scope
+    'read_out_of_scope':
+        ['def x(parameter):\n    return parameter\nx(0)\nparameter', [], ['read_out_of_scope']],
+    'read_inside_of_scope':
+        ['def x(parameter):\n    return parameter\nx(0)', ['read_out_of_scope'], []],
+    'read_not_out_of_scope':
+        ['def x():\n    if 1:\n        y=0\n    else:\n        y=1\n    y\nx()\nx()', ['read_out_of_scope'], []],
+
+    # Function with annotations
+    'annotated_parameters_correct':
+        ['def x(n: int):\n    1+n\nx(5)', ['parameter_type_mismatch', 'incompatible_types'], []],
+    'annotated_parameters_wrong_argument':
+        ['def x(n: int):\n    1+n\nx("5")', [], ['parameter_type_mismatch']],
+    'annotated_parameters_wrong_parameter':
+        ['def x(n: int):\n    "1"+n\nx(5)', [], ['incompatible_types']],
+    'annotated_parameters_append_list':
+        ['def x(l: list):\n    l.append(1)\nx([])', ['parameter_type_mismatch', 'incompatible_types'], []],
+    'annotated_returns_int':
+        ['def x()->int:\n    return "Wrong"\nx()', [], ['multiple_return_types']],
+    'annotated_returns_list_int':
+        ['def x()->[int]:\n    return [1,2,3]\nx().append(4)', ['multiple_return_types', 'incompatible_types'], []],
+
+    'append_to_empty_list':
+        ['a = []\na.append(1)\nprint(a)', ['initialization_problem', 'unused_variable'], []],
+    'append_to_non_empty_list':
+        ['a = [1]\na.append(1)\nprint(a)', ['initialization_problem', 'unused_variable'], []],
+    'append_to_undefined':
+        ['a.append(1)\nprint(a)', ['unused_variable'], ['initialization_problem']],
+    'append_to_unread':
+        ['a=[]\na.append(1)', ['initialization_problem'], ['unused_variable']],
+    'append_to_number':
+        ['a=1\na.append(1)\nprint(a)', [], ['append_to_non_list']],
+
+    'append_and_index':
+        ['x=[]\nx.append(1)\nx[0]+1', ['incompatible_types'], []],
+    'indexing_used':
+        ['mag1 = 0\nmercalli = [0]\nmag1 = mercalli[mag1]\nmag1',
+         ['initialization_problem', 'unused_variable', 'overwritten_variable'], []],
+
+    'created_list_but_unread':
+        ['old = [1,2,3]\nnew=[]\nfor x in old:\n\tnew.append(x)', [], ['unused_variable']],
+    'created_list_but_undefined':
+        ['old = [1,2,3]\nfor x in old:\n\tnew.append(x)\nprint(new)', [], ['initialization_problem']],
+
+    'builtin_float_converter':
+        ['a = float(5)\nb = "test"\nprint(a+b)', [], ['incompatible_types']],
+
+    # Double iteration
+    'iterate_over_list_of_tuples':
+        ['for x,y in [(1,2), (3,4)]:\n    x, y', ['initialization_problem'], []],
+    'iterate_over_items':
+        ['record = {"A": 5, "B": 6}\nfor x,y in record.items():\n    x, y', ['initialization_problem'], []],
+    'iterate_over_items_add':
+        ['record = {"A": 5, "B": 6}\nfor x,y in record.items():\n    x+"", y+0',
+         ['initialization_problem', "incompatible_types"], []],
+
+    # Tuple, Multiple Assignment
+    'multiple_assignment': ['a,b = 1,2\n1+a\nb', ['incompatible_types'], []],
+    'tuple_index': ['tuple_box = (6, 8, 4)\nprint(tuple_box[0])', [], []],
+
+    # Sets
+    'set_creation': ['a = set([1,2,3])\nprint(a)', ['initialization_problem'], []],
+    'set_addition': ['a = {"dog"}\na+"cat"', [], ['incompatible_types']],
+    'set_union_good': ['a = {"dog"}\na|{"cat"}', ['incompatible_types'], []],
+    'set_union_bad': ['a = {"dog"}\na|"cat"', [], ['incompatible_types']],
+
+    # Dictionaries
+    'set_key_in_dict': ['a = {}\na[1] = 0', [], []],
+    'use_key_in_dict': ['a = {"x": 5, "y": "T"}\na["x"]+5', ['incompatible_types'], []],
+    'use_key_in_lod': ['x=[{"a": 0, "b": True}, {"a": 1, "b": False}]\ny=x[0]\nz=y["a"]+0', ['incompatible_types'], []],
+    'use_chained_key_in_lod': ['x=[{"a": 0, "b": True}, {"a": 1, "b": False}]\nnot x[1]["b"]', ['incompatible_types'],
+                               []],
+    'iterate_over_lod': ['ls=[{"a": 0, "b": True}, {"a": 1, "b": False}]\nfor x in ls:\n    x["a"]+0',
+                         ['incompatible_types'], []],
+    # TODO: Add stronger assertion this one, it shouldn't be a good one
+    'incorrect_dict_iteration': ['dict = {"T": "V"}\nfor key,value in dict:\n    print(key)', [], []],
+    'incorrect_dict_iteration2': ['dict = {"T": 0}\nfor i in dict:\n print(i, dict[i])', [], []],
+
+    # Record type
+    'record_type_simple': [
+        ('Dog = {"Name": str, "Age": int, "Fluffy": bool}\n'
+         'def do_stuff(a_dog: Dog) -> Dog:\n'
+         '    a_dog["Name"]+""\n'
+         '    a_dog["Age"] = a_dog["Age"]+5\n'
+         '    return a_dog\n'
+         'ada = {"Name": "Ada", "Age": 2, "Fluffy": True}\n'
+         'do_stuff(ada)["Name"] + ""'
+         ), ['incompatible_types'], []
+    ],
+    'dict_with_setter': [
+        ('person1={"Name": "Babbage", "Age": 3}\n'
+            'def make_older(a_dog: dict) -> int:\n'
+            '    a_dog["Age"]+=1\n'
+            '    return a_dog["Age"]\n'
+            'make_older(person1) + 0'), ['incompatible_types', 'type_changes'], []
+    ],
+    'function_returns_typed_dict': [
+        ('def count_words(words: str) -> {str: int}:\n'
+         '  counts = {}\n'
+         '  for word in words.split(","):\n'
+         '    if word not in counts:\n'
+         '      counts[word] = 0\n'
+         '    counts[word] += 1\n'
+         '  return counts\n'
+         'count_words("alpha,alpha,beta,alpha")'), ['multiple_return_types'], []
+    ],
+    'record_type_in_list': [
+        ('Test = {"a": str}\n'
+         'def x(y: [Test]):\n'
+         '  return y[0]["a"]\n'
+         'x([{"a": "apple"}])'),
+         ['Parameter Type Mismatch'], []
+    ],
+
+    # While
+    'while_until_input': [
+        'user = input("Give a word.")\nwhile user:\n    print(user)\n    user = input("Give another word.")',
+        ['unused_variable'], []],
+
+    # With
+    'with_open':
+        ['with open("A") as a:\n    print(a)', ['initialization_problem'], []],
+
+    # List comprehensions
+    'list_comprehension':
+        ['a = [5 for x in range(100)]\nfor i in a:\n    5+i', ['iterating_over_non_list', 'incompatible_types'], []],
+
+    # return_outside_function
+    'no_return_outside_function':
+        ['def x():\n    return 5\nx()', ['return_outside_function'], []],
+    'return_outside_function':
+        ['def x():\n    pass\nreturn 5\nx()', [], ['return_outside_function']],
+
+    # Classes
+    'class_definition':
+        [
+            'class A:\n    y = 0\n    def __init__(self, x):\n        self.x = 0\n        self.test()\n    def test(self):\n        self.x = 5\nA()',
+            [], []],
+    'instance_assignment':
+        ['class A:\n pass\na = A()\na.b = 0\nb', [], ['initialization_problem']],
+    'instance_assignment_alt':
+        ['class A:\n pass\na = A()\na.b = 0\na.b', ['initialization_problem'], []],
+    'constructor_assignment':
+        ['class A:\n def __init__(self):\n  self.x=0\na=A()\na.x+""', [], ['incompatible_types']],
+    'parameterized_constructor_assignment':
+        [dedent("""
+                class A:
+                    def __init__(self, f):
+                        self.y = f
+                a = A(7)
+                a.y + ''"""), [], ['incompatible_types']],
+    'complex_destructuring':
+        [dedent("""
+                class Player:
+                    def __init__(self):
+                        self.health = 100
+                class World:
+                    def __init__(self):
+                        self.p = Player()
+                w = World()
+                w.p.health, w.p = (5, Player())
+                """), ['incompatible_types'], []],
+    'class_type_promotion':
+        [dedent("""
+                class Enemy:
+                    def __init__(self):
+                        self.health = 0
+                class Player:
+                    def __init__(self):
+                        self.enemies = []
+                class World:
+                    def __init__(self):
+                        self.p = Player()
+                w = World()
+                w.p.enemies.append(Enemy())
+                w.p.enemies[0].health + 100
+                """), ['incompatible_types'], []],
+
+    # Mutable Types
+    'mutable_list_in_function':
+        ['def t():\n    x = []\n    x.append(1)\n    return x\nfor x in t():\n    x + 1', ['incompatible_types'], []],
+    # Importing
+    'import_matplotlib':
+        ['import matplotlib.pyplot as plt\nplt.hist([1,2,3])\nplt.show()', ['initialization_problem'], []],
+    'import_random':
+        ['from random import randint\na=randint(1,2)\n1+a', ['initialization_problem', 'incompatible_types'], []],
+
+    'import_state_demographics':
+        [
+            "import state_demographics\n\n\nincome_list = state_demographics.get(\"Per Capita Income\",\"(None)\",'')\nfilter_income = []\nfor income in income_list:\n    if income > 28000:\n        income_list.append(filter_income)\nprint(filter_income)\n",
+            [], []],
+    'import_state_demographics2':
+        [
+            "import state_demographics\n\n\nincome_list = state_demographics.get(\"Per Capita Income\",\"(None)\",'')\nnew_income_list = 0\nfor income in income_list:\n    if income > 28000:\n        new_income_list = new_income_list + 1\nprint(new_income_list)\n",
+            [], []],
+    'filter_pattern':
+        ['l = []\nfor x in l:\n    if x > 0:\n        x', [], []],
+    'append_iter_var_to_list':
+        ['x = []\nx.append(x)\nx', [], []],
+    'append_multiple_types':
+        ['x = []\nx.append(7)\nx.append("F")\nx', [], ['type_change_append']],
+    'bad_append_iter_var_to_list':
+        ['x = []\nx.append(x)\nx.append(7)\nx', [], ['type_change_append']],
+    'function_with_parameter':
+        ['def x(y):\n    y\nx()', [], []],
+    'function_returns_None':
+        ['def x():\n    return\nx()', [], []],
+    'mutually_recursive_call':
+        ['def y():\n    x()\ndef x():\n    y()\nx()', [], ['recursive_call']],
+    'recursive_call':
+        ['def x():\n    x()\nx()', [], ['recursive_call']],
+    'overwritten_double_nested_branch':
+        ['b= 0\nif True:\n    if True:\n        b=0\nb', ['possible_initialization_problem'], []],
+    # Overwritten in one branches
+    'overwritten_in_one_branch_alt':
+        ['a = 0\nif True:\n\ta = 1\na', ['possible_initialization_problem'], []],
+    'filter_pattern2':
+        ["t = 0\nfor x in []:\n    if x:\n        t = t + 1\nprint(t)", ['possible_initialization_problem'], []],
+    'read_out_scope2':
+        ["x = ''\ndef y():\n    return x\ny()", ['unused_variable'], []],
+
+    'read_out_scope_double_branch':
+        ["def x():\n  if True:\n    y=0\n  else:\n    y=1\n  y\nx()",
+         ['unused_variable', 'read_out_of_scope'], []],
+
+    # Calling functions from within functions
+    'call_function_within_function':
+        ['def z():\n     return b\ndef y():\n    b = 0\n    z()\n    return b\ndef x():\n    y()\nx()',
+         ['unused_variable'], ['read_out_of_scope']],
+
+    # While loop with possibly unused body
+    'while_body_and_conditional_uses_variable':
+        ['a = 10\nwhile a:\n    a -= 1', ['unused_variable'], []],
+    'while_body_uses_variable':
+        ['a = 10\nwhile True:\n    a -= 1', [], ['unused_variable']],
+    'while_body_possibly_defines_variable':
+        ['while True:\n    a=0\na', [], ['possible_initialization_problem']],
+    'while_body_defined_variable':
+        ['a=0\nwhile True:\n    a=0\na', ['possible_initialization_problem'], []],
+
+    # Generators
+    'add_list_to_list_comprehension':
+        ['[1]+[a for a in [1,2,3]]', ['unused_variable', "incompatible_types"], []],
+    'add_set_to_set_comprehension':
+        ['{4}+{a for a in [1,2,3]}', ['unused_variable'], ["incompatible_types"]],
+    'union_set_to_set_comprehension':
+        ['{4}|{a for a in [1,2,3]}', ['unused_variable', "incompatible_types"], []],
+    'int_membership_in_dictionary':
+        ['3 in {a:a for a in [1,2,3]}', ['unused_variable', "incompatible_types"], []],
+    'int_membership_in_comprehension':
+        ['4 in (a for a in [1,2,3])', ['unused_variable', "incompatible_types"], []],
+
+    'prevent_empty_iteration_in_appended_list':
+        ['eles = [1,2,3]\nx = []\nfor ele in eles:\n    x.append(ele)\nfor e2 in x:\n    e2+1',
+         ['iterating_over_empty_list'], []],
+
+    'prevent_empty_iteration_dict':
+        ['x={"A":5}\nfor y in x:\n y', ['iterating_over_empty_list'], []],
+    
+    # Slices
+    'function_call_in_slice':
+        ['def x(): return 2\n"TEST"[:x()]', ['unused_variable'], []],
+
+    # Built-in modules
+    'import_string_letters':
+        ['import string\nstring.letters+""', ['incompatible_types'], []],
+
+    # Nested function definitions
+    'function_nested_inside_if':
+        ['if False:\n  def x():\n    pass', [], ['nested_function_definition']],
+    'function_toplevel':
+        ['def x():\n  if False:\n    pass', ['nested_function_definition'], []],
+    'no_function_whatsoever':
+        ['if False:\n  pass', ['nested_function_definition'], []],
+    'unused_result_function':
+        ['abs(-5)', [], ['unused_returned_value']],
+    'unused_result_method':
+        ['"".strip()', [], ['unused_returned_value']],
+    'unused_result_custom_function':
+        ['def x(): return 7\nx()', [], ['unused_returned_value']],
+    'used_result_custom_function':
+        ['def x(): return 7\nprint(x())', ['unused_returned_value'], []],
+    'used_result_function':
+        ['print(abs(-5))', ['unused_returned_value'], []],
+
+    # Reused variable in outer scope
+    'function_reused_outer_variable_write':
+        ['def y(b): return b+"!"\ndef x(a): return y(a)+"?"\na="Hi"\nx(a)',
+         ['write_out_of_scope'], []],
+
+    # Dictionary stuff
+    'dictionary_literal_key_access_int':
+        ['person = {"Name": "Charles", "Age": 4}\nperson["Age"] + 1',
+         ['incompatible_types'], []],
+    'dictionary_literal_key_access_int_bad':
+        ['person = {"Name": "Charles", "Age": 4}\nperson["Age"] + "1"',
+         [], ['incompatible_types']],
+    'dictionary_literal_key_access_str':
+        ['person = {"Name": "Charles", "Age": 4}\nperson["Name"] + 1',
+         [], ['incompatible_types']],
+    'dictionary_literal_key_access_str_bad':
+        ['person = {"Name": "Charles", "Age": 4}\nperson["Name"] + "1"',
+         ['incompatible_types'], []],
+
+    # Enumerate
+    'enumerate_function_in_function':
+        ['def do_it(data):\n    v = 0\n    for i, _ in enumerate(data):\n        v += i\n    return v\ndo_it("ab")',
+         ['unused_variable'], []],
+}
+
+
+class TestCode(unittest.TestCase):
+    pass
+
+
+SILENCE_EXCEPT = None #'add_assign_inside_dataclass_function' # 'possibly_overwritten_in_elif_branch' # None  # 'read_not_out_of_scope'
+
+
+def make_tester(internal_name, code, nones, somes):
+    def test_code(self):
+        contextualize_report(code)
+        tifa = pedal.tifa.Tifa()
+        try:
+            result = tifa.process_code(code)
+        except Exception as e:
+            raise type(e)(str(e) +
+                          ' in code:\n%s' % code)
+        if not result.success:
+            traceback.print_tb(result.error.__traceback__)
+            #self.fail("Error message in\n" + code + "\n" +
+            #          str(result.error))
+            self.fail(f"Error occurred: {str(result.error)}\nName: {internal_name}\n----\n{code}\n----\n")
+        for none in nones:
+            if result.issues.get(none, []):
+                print("")
+                pprint(result.variables)
+                self.fail(f"Incorrectly detected `{none}`\nName: {internal_name}\n----\n{code}\n----\n")
+        for some in somes:
+            if not result.issues.get(some, []):
+                self.fail(f"Failed to detect `{some}`\nName: {internal_name}\n----\n{code}\n----\n")
+    test_code.__name__ = "test_code_"+str(internal_name)
+    return test_code
+
+
+for name, (code, nones, somes) in unit_tests.items():
+    if SILENCE_EXCEPT in (None, "None") or SILENCE_EXCEPT == name:
+        setattr(TestCode, 'test_code_{}'.format(name), make_tester(name, code, nones, somes))
+
+
+class TestVariables(unittest.TestCase):
+    def test_type_comparisons(self):
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code('my_int=0\nmy_str="A"\nmy_list=[1,2,3]')
+        variables = result.top_level_variables
+        self.assertEqual(len(variables), 3)
+        # Integer variable
+        my_int = variables['my_int'].type
+        self.assertTrue(my_int.is_equal('num'))
+        self.assertTrue(my_int.is_equal('NumType'))
+        self.assertTrue(my_int.is_equal(int))
+        self.assertFalse(my_int.is_equal(float))
+        self.assertFalse(my_int.is_equal(str))
+        # String variable
+        my_str = variables['my_str'].type
+        self.assertTrue(my_str.is_equal('str'))
+        self.assertTrue(my_str.is_equal('StrType'))
+        self.assertTrue(my_str.is_equal(str))
+        # List variable
+        my_list = variables['my_list'].type
+        self.assertTrue(my_list.is_equal('list'))
+        self.assertTrue(my_list.is_equal('ListType'))
+        self.assertTrue(my_list.is_equal(list))
+        # List subtype
+        self.assertTrue(my_list.element_type.is_equal(int))
+        self.assertTrue(my_list.element_type.is_equal('num'))
+        self.assertFalse(my_list.element_type.is_equal(float))
+        self.assertTrue(my_list.element_type.is_equal('NumType'))
+
+    def test_variable_def_use(self):
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code('a=0\nb=0\nb\nc')
+        issues = result.issues
+        # Unused variables
+        self.assertEqual(len(issues['unused_variable']), 1)
+        unused_variables = [i.fields['name'] for i in issues['unused_variable']]
+        self.assertIn('a', unused_variables)
+        self.assertNotIn('b', unused_variables)
+        self.assertNotIn('c', unused_variables)
+        # Uninitalized variables
+        self.assertEqual(len(issues['initialization_problem']), 1)
+        unset_variables = [i.fields['name'] for i in issues['initialization_problem']]
+        self.assertNotIn('a', unset_variables)
+        self.assertNotIn('b', unset_variables)
+        self.assertIn('c', unset_variables)
+
+    def test_weirdness_used_function(self):
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code('def a(x):\n    return x\na(1)')
+        self.assertTrue(result.success)
+
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code('def a(x):\n    return x\n')
+        issues = result.issues
+        self.assertEqual(issues['unused_variable'][0].message,
+                         "The function a was "
+                         "given a definition on line 1, but was never used "
+                         "after that.")
+
+    def test_bad_parameter_found(self):
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code('def a(x: int):\n    return x\na("hello")')
+        issues = result.issues
+        self.assertEqual(issues['parameter_type_mismatch'][0].message,
+                         "You defined the parameter x as an integer. However, the argument passed to that parameter on line 3 was a string. The formal parameter type must match the argument's type.")
+
+    def test_bad_parameter_found_complex(self):
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code('def a(x: list[int]):\n    return x\na(5)')
+        issues = result.issues
+        self.assertEqual(issues['parameter_type_mismatch'][0].message,
+                         "You defined the parameter x as a list of integers. However, the argument passed to that parameter on line 3 was an integer. The formal parameter type must match the argument's type.")
+
+    def test_weirdness_tate_import_example(self):
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(dedent('''
+        import tate
+        art = tate.get_artwork()
+        h = [a['dimensions']['height'] for a in art if a['artist']['birth']['year'] > 1000]
+        b = [a['artist']['birth']['year'] for a in art 
+             if a['artist']['birth']['year'] > 1000]
+        import matplotlib.pyplot as plt
+        plt.scatter(b, h, alpha=.1)
+        plt.show()'''))
+        self.assertTrue(result.success)
+
+    '''
+    def test_tifa_graceful_errors(self):
+        student_code = '1 + "Banana"'
+        set_source(student_code)
+        exception = commands.run_student()
+        self.assertIsNotNone(exception)'''
+
+    def test_json_types(self):
+        t = normalize.get_pedal_type_from_json({'type': 'NumType'})
+        self.assertIsInstance(t, defs.NumType)
+        t = normalize.get_pedal_type_from_json({'type': 'StrType'})
+        self.assertIsInstance(t, defs.StrType)
+        t = normalize.get_pedal_type_from_json({'type': 'BoolType'})
+        self.assertIsInstance(t, defs.BoolType)
+        t = normalize.get_pedal_type_from_json({'type': 'NoneType'})
+        self.assertIsInstance(t, defs.NoneType)
+        t = normalize.get_pedal_type_from_json({'type': 'ListType',
+                                 'subtype': {'type': 'NumType'}})
+        self.assertIsInstance(t, defs.ListType)
+        self.assertIsInstance(t.element_type, defs.NumType)
+
+        l1 = {'type': 'LiteralStr', 'value': 'First'}
+        l2 = {'type': 'LiteralStr', 'value': 'Second'}
+        v1, v2 = {'type': 'StrType'}, {'type': 'NumType'}
+        t = normalize.get_pedal_type_from_json({'type': 'DictType', 'literals': [l1, l2],
+                                 'values': [v1, v2]})
+        self.assertIsInstance(t, defs.DictType)
+        self.assertIsInstance(t.element_types, list)
+        self.assertEqual(len(t.element_types), 2)
+        self.assertIsInstance(t.element_types[0][0], defs.LiteralStr)
+        self.assertEqual(t.element_types[0][0].value, 'First')
+        self.assertIsInstance(t.element_types[1][0], defs.LiteralStr)
+        self.assertEqual(t.element_types[1][0].value, 'Second')
+        self.assertIsInstance(t.element_types, list)
+        self.assertEqual(len(t.element_types), 2)
+        self.assertIsInstance(t.element_types[0][1], defs.StrType)
+        self.assertIsInstance(t.element_types[1][1], defs.NumType)
+
+        # Try to parse the Broadway type definition
+        complex_type = {"type": "ModuleType",
+                        "fields": {
+                            'get': {"type": "ListType", "empty": False,
+                                    "subtype": {"type": "NumType"}},
+
+                            'get_shows':
+                                {"type": "ListType", "subtype":
+                                    {"type": "DictType", "literals": [{"type": "LiteralStr", "value": 'Statistics'},
+                                                                      {"type": "LiteralStr", "value": 'Show'},
+                                                                      {"type": "LiteralStr", "value": 'Date'}],
+                                     "values": [
+                                         {"type": "DictType", "literals": [{"type": "LiteralStr", "value": 'Capacity'},
+                                                                           {"type": "LiteralStr",
+                                                                            "value": 'Attendance'},
+                                                                           {"type": "LiteralStr",
+                                                                            "value": 'Performances'},
+                                                                           {"type": "LiteralStr", "value": 'Gross'},
+                                                                           {"type": "LiteralStr",
+                                                                            "value": 'Gross Potential'}], "values": [
+                                             {"type": "NumType"},
+                                             {"type": "NumType"},
+                                             {"type": "NumType"},
+                                             {"type": "NumType"},
+                                             {"type": "NumType"}]},
+                                         {"type": "DictType", "literals": [{"type": "LiteralStr", "value": 'Type'},
+                                                                           {"type": "LiteralStr", "value": 'Theatre'},
+                                                                           {"type": "LiteralStr", "value": 'Name'}],
+                                          "values": [
+                                              {"type": "StrType"},
+                                              {"type": "StrType"},
+                                              {"type": "StrType"}]},
+                                         {"type": "DictType", "literals": [{"type": "LiteralStr", "value": 'Day'},
+                                                                           {"type": "LiteralStr", "value": 'Month'},
+                                                                           {"type": "LiteralStr", "value": 'Year'},
+                                                                           {"type": "LiteralStr", "value": 'Full'}],
+                                          "values": [
+                                              {"type": "NumType"},
+                                              {"type": "NumType"},
+                                              {"type": "NumType"},
+                                              {"type": "StrType"}]}]}},
+
+                        }}
+        normalize.get_pedal_type_from_json(complex_type)
+
+    def test_custom_module_import_weather(self):
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code('import weather\n' +
+                          'rs = weather.get_weather()\n' +
+                          'for r in rs:\n' +
+                          '  0+r["Data"]["Precipitation"]',
+                                   filename='student.py')
+        self.assertTrue(result.success)
+        self.assertNotIn('module_not_found', result.issues)
+
+    def test_custom_module_import_police(self):
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code('import police_shootings\n'
+                          'rs = police_shootings.get_shootings()\n'
+                          'for r in rs:\n'
+                          '  x=0+r["Person.Age"]\n'
+                          'x', filename='student.py')
+        self.assertTrue(defs.is_subtype(result.top_level_variables['x'].type, defs.NumType()))
+        self.assertTrue(result.success)
+        self.assertNotIn('module_not_found', result.issues)
+
+    def test_custom_module_import_babbages(self):
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code('import babbages\n'
+                          'print(babbages)', filename='student.py')
+        self.assertIn('module_not_found', result.issues)
+
+    def test_custom_module_import_broadway(self):
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(dedent("""
+            import broadway
+            report_list = broadway.get_shows()
+            total= 0
+            for broadway in report_list:
+                if broadway ["Show"]["Type"] == "Musical":
+                    total = total + 1
+            print(total)"""), filename='student.py')
+        self.assertTrue(result.success)
+        self.assertNotIn('module_not_found', result.issues)
+
+    def test_get_types(self):
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code('a=0\na="Hello"\na=[1,2,3]\na=1')
+        a = result.top_level_variables['a']
+        self.assertTrue(a.was_type('num'))
+        self.assertTrue(a.was_type(int))
+        self.assertTrue(a.was_type('NumType'))
+        self.assertTrue(a.was_type(defs.NumType))
+        self.assertFalse(a.was_type(bool))
+        self.assertFalse(a.was_type(defs.DictType))
+        self.assertTrue(a.was_type('ListType'))
+
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code('credits=[1,2,3,4]\nfor credit in credits:\n  print(credit)')
+        credit = result.top_level_variables['credit']
+        self.assertFalse(credit.was_type(list))
+        self.assertTrue(credit.was_type(int))
+
+    def test_dict_iteration(self):
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code('dict = {"T": 0}\nfor i in dict:\n    print(i, dict[i])')
+        self.assertTrue(result.success)
+
+    def test_classes(self):
+        program = 'class A:\n def __init__(self):\n  self.x=0\na=A()\na.x+""'
+        # print(indent(program, '    '))
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program)
+        # self.assertTrue(tifa.report['tifa']['success'])
+        # pprint(tifa.report['tifa'])
+        # print(tifa.report['tifa']['top_level_variables']['a'].type.parent.fields)
+        self.assertFalse(result.error)
+
+        program = dedent("""
+                class Enemy:
+                    def __init__(self):
+                        self.health = 0
+                class Player:
+                    def __init__(self):
+                        self.enemies = []
+                class World:
+                    def __init__(self):
+                        self.p = Player()
+                w = World()
+                w.p.enemies.append(Enemy())
+                w.p.enemies[0].health + 100
+                """)
+        tifa = pedal.tifa.Tifa()
+        tifa.process_code(program)
+        # pprint(tifa.report['tifa'])
+    
+    def test_locations(self):
+        program = dedent("""
+                a = 0
+                "Ignore"
+                "This"
+                "Line"
+                def unnecessary():
+                    pass
+                unnecessary
+                """)
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program)
+        self.assertEqual(result.issues['unused_variable'][0].location.line, 2)
+
+
+    def test_weird_indexing_behavior(self):
+        program = dedent("""
+        movie_list = [{'Title':'Iron Man', 'Release Date':'May 2, 2008','Budget':'140','Running Time':'126'},
+              {'Title':'Iron Man 2', 'Release Date':'May 7, 2010','Budget':'200', 'Running Time':'125'},
+              {'Title':'Iron Man 3', 'Release Date':'May 3, 2013','Budget':'200', 'Running Time':'130'}]
+        total=0
+        for title in movie_list:
+            total=total + 'title'['Running Time']
+        print(total)
+        """)
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program)
+        #self.assertNotIn('incompatible_types', result.issues)
+        self.assertIn('invalid_indexing', result.issues)
+
+    def test_not_finding_unused_return_value(self):
+        program = dedent("""
+            #import classics
+            import matplotlib.pyplot as plt
+            book_downloads = []
+            #report_list = classics.get_books(test=True)
+            report_list = [{'bibliography': {'type': 'Text'},
+                            'metadata': {'downloads': 0}}]
+            for report in report_list:
+                if report["bibliography"]["type"] == "Text":
+                    book_downloads.append(report["metadata"]["downloads"])
+            plt.hist(book_downloads)
+            plt.ylabel("Number of Books")
+            plt.xlabel("downloads")
+            plt.title("Spreads of Book Downloads")
+            plt.show()
+        """)
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program, filename="student.py")
+        self.assertNotIn('unused_returned_value', result.issues)
+        self.assertFalse(result.issues)
+
+    @unittest.skip("Currently broken, need to increase sophistication of typeddict support")
+    def test_typedict_book(self):
+        program = dedent("""
+            from cisc108 import *
+            class Book(TypedDict):
+                title: str
+                pages: int
+                hardcover: bool
+            
+            def page_count(a_book: Book) -> int:
+                return a_book['pages']
+                
+            hp = {'title': 'Harry Potter',
+                  'pages': 300,
+                  'hardcover': false}
+            
+            assert_equal(page_count(hp), 300)
+        """)
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program, filename="student.py")
+        self.assertFalse(result.issues)
+
+    def test_unnecessary_second_branch(self):
+        program = dedent("""# Remember to initialize the variables!
+age = 20
+has_license = True
+# Keep this If/else structure unchanged, but
+# fill in the blanks with the code above
+if has_license == True:
+    if age >= 21:
+        print("Can drink")
+        if age < 1000:
+            pass
+        else:
+            print("Too old")
+            
+    else:
+        print("Too young")
+        
+else:
+    print("Doesn't have a license")""")
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program, filename="student.py")
+        self.assertTrue(result.issues)
+
+    def test_complex_record_type(self):
+        program = dedent("""
+Test = {"a": str}
+
+def x(y: [Test]):
+    return y[0]['a']
+
+print(x([{"a": "apple"}]))""")
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program, filename="student.py")
+        self.assertFalse(result.issues)
+
+    def test_new_class_record_type(self):
+        program = dedent("""
+        from dataclasses import dataclass
+        
+        @dataclass
+        class Dog:
+            name: str
+            age: int
+            fuzzy: bool
+            
+        def is_fuzzy(a_dog: Dog) -> bool:
+            return a_dog.fuzzy
+            
+        ada = Dog('Ada Bart', 4, True)
+        print(ada.name)
+        
+        print(is_fuzzy(ada))
+        """)
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program, filename="student.py")
+        self.assertFalse(result.issues)
+
+    def test_new_class_record_type_bad_instance(self):
+        program = dedent("""
+        class Dog(record):
+            name: str
+            age: int
+            fuzzy: bool
+
+        def is_fuzzy(a_dog: Dog) -> bool:
+            return a_dog.fuzzy
+
+        ada = Dog('Ada Bart', 4)
+        print(ada.name)
+
+        print(is_fuzzy(ada))
+        """)
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program, filename="student.py")
+        self.assertTrue(result.issues)
+
+    def test_dataclass_mistake(self):
+        program = dedent("""
+        from dataclasses import dataclass
+        
+        @dataclass
+        class Dog:
+            name: str
+            age: int
+            fuzzy: bool
+            
+        @dataclass
+        class Cat:
+            name: str
+            age: int
+            fuzzy: bool
+
+        def is_fuzzy(a_dog: Dog) -> bool:
+            return a_dog.fuzzy
+
+        ada = Dog('Ada Bart', 4, True)
+        print(ada.name)
+
+        print(is_fuzzy(ada))
+        
+        adacat = Cat("Ada Bart", 4, True)
+        print(is_fuzzy(adacat))
+        """)
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program, filename="student.py")
+        self.assertIsNone(result.error)
+        self.assertTrue(result.issues)
+
+    def test_dataclass_mistake_lists(self):
+        program = dedent("""
+        from dataclasses import dataclass
+
+        @dataclass
+        class Dog:
+            name: str
+            age: int
+            fuzzy: bool
+
+        @dataclass
+        class Cat:
+            name: str
+            age: int
+            fuzzy: bool
+
+        def all_fuzzy(dogs: list[Dog]) -> bool:
+            return all(a_dog.fuzzy for a_dog in dogs)
+
+        ada = Dog('Ada Bart', 4, True)
+        print(ada.name)
+
+        print(all_fuzzy([ada]))
+
+        adacat = Cat("Ada Bart", 4, True)
+        print(all_fuzzy([adacat]))
+        """)
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program, filename="student.py")
+        self.assertIsNone(result.error)
+        self.assertTrue(result.issues)
+        self.assertEqual("You defined the parameter dogs as a list of Dog. "
+                         "However, the argument passed to that parameter on line 25 was a list of Cat. "
+                         "The formal parameter type must match the argument's type.",
+                         result.issues['parameter_type_mismatch'][0].message)
+
+    def test_dataclass_bad_constructor_call_order(self):
+        program = dedent("""
+        from dataclasses import dataclass
+
+        @dataclass
+        class Dog:
+            name: str
+            age: int
+            fuzzy: bool
+        
+        ada = Dog('Ada Bart', True, 4)
+        print(ada.name)
+        """)
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program, filename="student.py")
+        self.assertIsNone(result.error)
+        self.assertTrue(result.issues)
+        self.assertEqual("You defined the field age as an integer. However, the argument passed to that field's "
+                         "parameter in the constructor function on line 10 was a boolean. The formal field type "
+                         "must match the argument's type.",
+                         result.issues['field_type_mismatch'][0].message)
+
+    def test_dataclass_bad_constructor_call_arity(self):
+        program = dedent("""
+        from dataclasses import dataclass
+
+        @dataclass
+        class Dog:
+            name: str
+            age: int
+            fuzzy: bool
+
+        ada = Dog('Ada Bart', 4)
+        print(ada.name)
+        """)
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program, filename="student.py")
+        self.assertIsNone(result.error)
+        self.assertTrue(result.issues)
+        self.assertEqual("The constructor function Dog was given the wrong number of arguments. You should have "
+                         "had 3 arguments, but instead you had 2 arguments.",
+                         result.issues['incorrect_arity'][0].message)
+
+    def test_dataclass_bad_constructor_call_extra(self):
+        program = dedent("""
+        from dataclasses import dataclass
+
+        @dataclass
+        class Dog:
+            name: str
+            age: int
+            fuzzy: bool
+
+        ada = Dog('Ada Bart', 4, True, "is cute!")
+        print(ada.name)
+        """)
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(program, filename="student.py")
+        self.assertIsNone(result.error)
+        self.assertTrue(result.issues)
+        self.assertEqual("The constructor function Dog was given the wrong number of arguments. You should have "
+                         "had 3 arguments, but instead you had 4 arguments.",
+                         result.issues['incorrect_arity'][0].message)
+
+    def test_import_second_file(self):
+        main_program = dedent("""
+        import monsters
+        
+        monsters.number + ""
+        """)
+        monster_file = dedent("""number = 7\nalpha = 'test'""")
+        contextualize_report(Submission(files={'student.py': main_program, 'monsters.py': monster_file}))
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(main_program, filename="student.py")
+        self.assertIsNone(result.error)
+        self.assertTrue(result.issues)
+        self.assertEqual("You used an addition operation with an integer and a string on line 4. But you can't do that with that operator. Make sure both sides of the operator are the right type.",
+                         result.issues['incompatible_types'][0].message)
+        self.assertEqual(len(result.issues.get('unused_variable', [])), 0)
+
+    def test_import_second_file_successful(self):
+        main_program = dedent("""
+        from monsters import Monster, dracula
+
+        dracula.name + ""
+        print(Monster("Wolfman"))
+        """)
+        monster_file = dedent("""
+        from dataclasses import dataclass
+        @dataclass
+        class Monster:
+            name: str
+        dracula = Monster('Dracula')""")
+        contextualize_report(Submission(files={'student.py': main_program, 'monsters.py': monster_file}))
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(main_program, filename="student.py")
+        self.assertIsNone(result.error)
+        self.assertFalse(result.issues)
+
+    def test_provide_import_type_definitions(self):
+        main_program = dedent("""
+        import monsters
+
+        monsters.number + ""
+        """)
+        tifa = pedal.tifa.Tifa()
+        tifa_provide_module_type('monsters', {'number': normalize.normalize_type('int')})
+        result = tifa.process_code(main_program, filename="student.py")
+        self.assertIsNone(result.error)
+        self.assertTrue(result.issues)
+        self.assertEqual(
+            "You used an addition operation with an integer and a string on line 4. But you can't do that with that operator. Make sure both sides of the operator are the right type.",
+            result.issues['incompatible_types'][0].message)
+
+    @unittest.skip
+    def test_provide_module_definitions(self):
+        main_program = dedent("""
+        from monsters import dracula
+
+        dracula.age + ""
+        """)
+        tifa = pedal.tifa.Tifa()
+        import tests.test_files.monsters as monsters
+        tifa_provide_module_type('monsters', normalize.normalize_type(monsters))
+        result = tifa.process_code(main_program, filename="student.py")
+        if result.error is not None:
+            raise result.error
+        self.assertIsNone(result.error)
+        self.assertTrue(result.issues)
+        self.assertEqual(
+            "You used an addition operation with an integer and a string on line 4. But you can't do that with that operator. Make sure both sides of the operator are the right type.",
+            result.issues['incompatible_types'][0].message)
+
+    def test_weird_return_control_flow(self):
+        main_program = dedent("""
+        from dataclasses import dataclass
+        
+        @dataclass
+        class Media:
+            name: str
+            kind: str
+            duration: int
+        
+        def longest(media: list[Media]) -> str:
+            movies_only = [i for i in media if i.kind == 'movie']
+            if not movies_only:
+                return 'no movies'
+            key = lambda movie: movie.duration
+            return max(movies_only, key=key).name
+        
+        print(longest([Media("Snoopy", "movie", 5)]))
+        print(longest([]))
+        """)
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(main_program, filename="student.py")
+        if result.error:
+            raise result.error
+        self.assertIsNone(result.error)
+        self.assertFalse(result.issues)
+
+    def test_weird_increment_set_list(self):
+        main_program = dedent("""from dataclasses import dataclass
+
+@dataclass
+class Forecast:
+    reports: list[int]
+    
+def rainfall(weather: list[Forecast]) -> list[int]:
+    reports = []
+    for a_weather in weather:
+        reports += a_weather.reports
+    return reports
+
+def total_rainfall(forecast: list[Forecast]) -> int:
+    total = 0
+    reports = rainfall(forecast)
+    for measurement in reports:
+        total += measurement
+    return total
+
+forecast1 = [Forecast([1,2,3])]
+5+total_rainfall(forecast1)""")
+        tifa = pedal.tifa.Tifa()
+        result = tifa.process_code(main_program, filename="student.py")
+        if result.error:
+            raise result.error
+        self.assertIsNone(result.error)
+        self.assertFalse(result.issues)
+
+if __name__ == '__main__':
+    unittest.main(buffer=False)
```

### Comparing `pedal-2.6.1/tests/test_toolkit.py` & `pedal-2.6.2/tests/test_toolkit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_types.py` & `pedal-2.6.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_user_feedback.py` & `pedal-2.6.2/tests/test_user_feedback.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_utilities_progsnap.py` & `pedal-2.6.2/tests/test_utilities_progsnap.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_utilities_sorting.py` & `pedal-2.6.2/tests/test_utilities_sorting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_vpl.py` & `pedal-2.6.2/tests/test_vpl.py`

 * *Files identical despite different names*

### Comparing `pedal-2.6.1/tests/test_wheatchaff_game.py` & `pedal-2.6.2/tests/test_wheatchaff_game.py`

 * *Files identical despite different names*

