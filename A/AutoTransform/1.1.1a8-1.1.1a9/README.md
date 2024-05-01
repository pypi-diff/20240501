# Comparing `tmp/AutoTransform-1.1.1a8.tar.gz` & `tmp/AutoTransform-1.1.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoTransform-1.1.1a8.tar", last modified: Thu Aug 24 21:04:19 2023, max compression
+gzip compressed data, was "AutoTransform-1.1.1a9.tar", last modified: Wed Oct  4 22:55:42 2023, max compression
```

## Comparing `AutoTransform-1.1.1a8.tar` & `AutoTransform-1.1.1a9.tar`

### file list

```diff
@@ -1,181 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.519957 AutoTransform-1.1.1a8/
--rw-r--r--   0 runner    (1001) docker     (999)     3699 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/BEST_PRACTICES.md
--rw-r--r--   0 runner    (1001) docker     (999)     7437 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/COMPONENTS.md
--rw-r--r--   0 runner    (1001) docker     (999)     2978 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (999)     4541 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/CUSTOM_DEPLOYMENT.md
--rw-r--r--   0 runner    (1001) docker     (999)     1081 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     1671 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/MANAGE_CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (999)      142 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     5484 2023-08-24 21:04:19.519957 AutoTransform-1.1.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     4698 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/README.md
--rw-r--r--   0 runner    (1001) docker     (999)     3864 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/SCHEDULED_RUNS.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.499957 AutoTransform-1.1.1a8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.499957 AutoTransform-1.1.1a8/examples/docker/
--rw-r--r--   0 runner    (1001) docker     (999)      182 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/examples/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (999)      979 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/examples/docker/docker_autotransform.sh
--rwxr-xr-x   0 runner    (1001) docker     (999)      993 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/examples/docker/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (999)      895 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/examples/manager.json
--rw-r--r--   0 runner    (1001) docker     (999)       28 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/examples/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)      278 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/examples/scheduler.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.499957 AutoTransform-1.1.1a8/examples/schemas/
--rw-r--r--   0 runner    (1001) docker     (999)      903 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/examples/schemas/black_format.json
--rw-r--r--   0 runner    (1001) docker     (999)       93 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/examples/schemas/schema_map.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.503957 AutoTransform-1.1.1a8/examples/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)      880 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/examples/workflows/autotransform.manage.yml
--rw-r--r--   0 runner    (1001) docker     (999)     2048 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/examples/workflows/autotransform.run.yml
--rw-r--r--   0 runner    (1001) docker     (999)      890 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/examples/workflows/autotransform.schedule.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1489 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/examples/workflows/autotransform.update.yml
--rw-r--r--   0 runner    (1001) docker     (999)      103 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-24 21:04:19.519957 AutoTransform-1.1.1a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     2861 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.495957 AutoTransform-1.1.1a8/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.495957 AutoTransform-1.1.1a8/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.503957 AutoTransform-1.1.1a8/src/python/AutoTransform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     5484 2023-08-24 21:04:19.000000 AutoTransform-1.1.1a8/src/python/AutoTransform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     6276 2023-08-24 21:04:19.000000 AutoTransform-1.1.1a8/src/python/AutoTransform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-24 21:04:19.000000 AutoTransform-1.1.1a8/src/python/AutoTransform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      255 2023-08-24 21:04:19.000000 AutoTransform-1.1.1a8/src/python/AutoTransform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      168 2023-08-24 21:04:19.000000 AutoTransform-1.1.1a8/src/python/AutoTransform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       14 2023-08-24 21:04:19.000000 AutoTransform-1.1.1a8/src/python/AutoTransform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.503957 AutoTransform-1.1.1a8/src/python/autotransform/
--rw-r--r--   0 runner    (1001) docker     (999)      627 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.503957 AutoTransform-1.1.1a8/src/python/autotransform/batcher/
--rw-r--r--   0 runner    (1001) docker     (999)      467 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/batcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2793 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/batcher/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     2856 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/batcher/chunk.py
--rw-r--r--   0 runner    (1001) docker     (999)     7144 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/batcher/codeowners.py
--rw-r--r--   0 runner    (1001) docker     (999)     2408 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/batcher/directory.py
--rw-r--r--   0 runner    (1001) docker     (999)     2839 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/batcher/extradata.py
--rw-r--r--   0 runner    (1001) docker     (999)     2789 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/batcher/regex.py
--rw-r--r--   0 runner    (1001) docker     (999)     1966 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/batcher/single.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.503957 AutoTransform-1.1.1a8/src/python/autotransform/change/
--rw-r--r--   0 runner    (1001) docker     (999)      488 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/change/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6558 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/change/base.py
--rw-r--r--   0 runner    (1001) docker     (999)    10075 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/change/github.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.503957 AutoTransform-1.1.1a8/src/python/autotransform/command/
--rw-r--r--   0 runner    (1001) docker     (999)      532 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1778 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/command/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     5972 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/command/script.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.503957 AutoTransform-1.1.1a8/src/python/autotransform/config/
--rw-r--r--   0 runner    (1001) docker     (999)     3816 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    21443 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/config/config.py
--rw-r--r--   0 runner    (1001) docker     (999)     1804 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/config/default.py
--rw-r--r--   0 runner    (1001) docker     (999)     2895 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/config/environment.py
--rw-r--r--   0 runner    (1001) docker     (999)      977 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/config/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.507957 AutoTransform-1.1.1a8/src/python/autotransform/event/
--rw-r--r--   0 runner    (1001) docker     (999)      762 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1833 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/event/action.py
--rw-r--r--   0 runner    (1001) docker     (999)     2846 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/event/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     1757 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/event/debug.py
--rw-r--r--   0 runner    (1001) docker     (999)     4041 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/event/handler.py
--rw-r--r--   0 runner    (1001) docker     (999)      581 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/event/logginglevel.py
--rw-r--r--   0 runner    (1001) docker     (999)     1701 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/event/remoterun.py
--rw-r--r--   0 runner    (1001) docker     (999)     1679 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/event/run.py
--rw-r--r--   0 runner    (1001) docker     (999)     1734 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/event/schedulerun.py
--rw-r--r--   0 runner    (1001) docker     (999)      623 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/event/type.py
--rw-r--r--   0 runner    (1001) docker     (999)     1715 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/event/update.py
--rw-r--r--   0 runner    (1001) docker     (999)     1752 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/event/verbose.py
--rw-r--r--   0 runner    (1001) docker     (999)     1777 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/event/warning.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.507957 AutoTransform-1.1.1a8/src/python/autotransform/filter/
--rw-r--r--   0 runner    (1001) docker     (999)      432 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2405 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/filter/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (999)     4288 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/filter/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     2415 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/filter/codeowners.py
--rw-r--r--   0 runner    (1001) docker     (999)     1151 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/filter/key_hash_shard.py
--rw-r--r--   0 runner    (1001) docker     (999)     2156 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/filter/regex.py
--rw-r--r--   0 runner    (1001) docker     (999)     4401 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/filter/script.py
--rw-r--r--   0 runner    (1001) docker     (999)     1508 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/filter/shard.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.507957 AutoTransform-1.1.1a8/src/python/autotransform/input/
--rw-r--r--   0 runner    (1001) docker     (999)      490 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2562 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/input/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     2462 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/input/directory.py
--rw-r--r--   0 runner    (1001) docker     (999)     1070 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/input/empty.py
--rw-r--r--   0 runner    (1001) docker     (999)     1570 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/input/gitgrep.py
--rw-r--r--   0 runner    (1001) docker     (999)     2703 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/input/inline.py
--rw-r--r--   0 runner    (1001) docker     (999)     3307 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/input/script.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.507957 AutoTransform-1.1.1a8/src/python/autotransform/item/
--rw-r--r--   0 runner    (1001) docker     (999)      450 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1567 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/item/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     1336 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/item/file.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.511957 AutoTransform-1.1.1a8/src/python/autotransform/repo/
--rw-r--r--   0 runner    (1001) docker     (999)      423 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3869 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/repo/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     7282 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/repo/git.py
--rw-r--r--   0 runner    (1001) docker     (999)     9108 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/repo/github.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.511957 AutoTransform-1.1.1a8/src/python/autotransform/runner/
--rw-r--r--   0 runner    (1001) docker     (999)      437 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2195 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/runner/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     6878 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/runner/github.py
--rw-r--r--   0 runner    (1001) docker     (999)     6379 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/runner/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (999)     1296 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/runner/local.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.511957 AutoTransform-1.1.1a8/src/python/autotransform/schema/
--rw-r--r--   0 runner    (1001) docker     (999)      749 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4295 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/schema/builder.py
--rw-r--r--   0 runner    (1001) docker     (999)     4826 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/schema/config.py
--rw-r--r--   0 runner    (1001) docker     (999)    15487 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/schema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.511957 AutoTransform-1.1.1a8/src/python/autotransform/scripts/
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.511957 AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/
--rw-r--r--   0 runner    (1001) docker     (999)      333 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    12182 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/initialize.py
--rw-r--r--   0 runner    (1001) docker     (999)     3159 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/manage.py
--rw-r--r--   0 runner    (1001) docker     (999)     7073 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (999)     3750 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/schedule.py
--rw-r--r--   0 runner    (1001) docker     (999)    13430 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (999)     5301 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (999)     2264 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/scripts/main.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.511957 AutoTransform-1.1.1a8/src/python/autotransform/scripts/migrations/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/scripts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4619 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/scripts/migrations/p1_0_1.py
--rw-r--r--   0 runner    (1001) docker     (999)     3259 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/scripts/migrations/p1_0_3.py
--rw-r--r--   0 runner    (1001) docker     (999)     2901 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/scripts/migrations/p1_0_5.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.511957 AutoTransform-1.1.1a8/src/python/autotransform/step/
--rw-r--r--   0 runner    (1001) docker     (999)      480 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.515957 AutoTransform-1.1.1a8/src/python/autotransform/step/action/
--rw-r--r--   0 runner    (1001) docker     (999)      415 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3360 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/action/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     1558 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/action/comments.py
--rw-r--r--   0 runner    (1001) docker     (999)     2843 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/action/labels.py
--rw-r--r--   0 runner    (1001) docker     (999)     2573 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/action/request.py
--rw-r--r--   0 runner    (1001) docker     (999)     4614 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/action/reviewers.py
--rw-r--r--   0 runner    (1001) docker     (999)     2787 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/action/source.py
--rw-r--r--   0 runner    (1001) docker     (999)     1998 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/base.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.515957 AutoTransform-1.1.1a8/src/python/autotransform/step/condition/
--rw-r--r--   0 runner    (1001) docker     (999)      427 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/condition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2513 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/condition/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (999)    11990 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/condition/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     2651 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/condition/comparison.py
--rw-r--r--   0 runner    (1001) docker     (999)     1519 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/condition/created.py
--rw-r--r--   0 runner    (1001) docker     (999)     1391 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/condition/labels.py
--rw-r--r--   0 runner    (1001) docker     (999)     3671 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/condition/request.py
--rw-r--r--   0 runner    (1001) docker     (999)     2257 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/condition/reviewers.py
--rw-r--r--   0 runner    (1001) docker     (999)     1467 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/condition/schema.py
--rw-r--r--   0 runner    (1001) docker     (999)     4084 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/condition/state.py
--rw-r--r--   0 runner    (1001) docker     (999)     1550 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/condition/updated.py
--rw-r--r--   0 runner    (1001) docker     (999)     3463 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/step/conditional.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.515957 AutoTransform-1.1.1a8/src/python/autotransform/transformer/
--rw-r--r--   0 runner    (1001) docker     (999)      375 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2574 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/transformer/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     2559 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/transformer/jscodeshift.py
--rw-r--r--   0 runner    (1001) docker     (999)     3662 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/transformer/libcst.py
--rw-r--r--   0 runner    (1001) docker     (999)    11395 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/transformer/openai.py
--rw-r--r--   0 runner    (1001) docker     (999)     1617 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/transformer/regex.py
--rw-r--r--   0 runner    (1001) docker     (999)     5359 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/transformer/script.py
--rw-r--r--   0 runner    (1001) docker     (999)     1149 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/transformer/single.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.519957 AutoTransform-1.1.1a8/src/python/autotransform/util/
--rw-r--r--   0 runner    (1001) docker     (999)      334 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2985 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/util/cachedfile.py
--rw-r--r--   0 runner    (1001) docker     (999)    15661 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/util/component.py
--rw-r--r--   0 runner    (1001) docker     (999)     8670 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/util/console.py
--rw-r--r--   0 runner    (1001) docker     (999)      600 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/util/enums.py
--rw-r--r--   0 runner    (1001) docker     (999)     3421 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/util/functions.py
--rw-r--r--   0 runner    (1001) docker     (999)    18520 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/util/github.py
--rw-r--r--   0 runner    (1001) docker     (999)     8931 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/util/manager.py
--rw-r--r--   0 runner    (1001) docker     (999)     1928 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/util/package.py
--rw-r--r--   0 runner    (1001) docker     (999)     5725 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/util/request.py
--rw-r--r--   0 runner    (1001) docker     (999)    16845 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/util/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (999)     5689 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/util/schema_map.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:04:19.519957 AutoTransform-1.1.1a8/src/python/autotransform/validator/
--rw-r--r--   0 runner    (1001) docker     (999)      483 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4321 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/validator/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     7186 2023-08-24 21:03:07.000000 AutoTransform-1.1.1a8/src/python/autotransform/validator/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.312437 AutoTransform-1.1.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/BEST_PRACTICES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/COMPONENTS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/CUSTOM_DEPLOYMENT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/MANAGE_CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2023-10-04 22:55:42.312437 AutoTransform-1.1.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/SCHEDULED_RUNS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.264437 AutoTransform-1.1.1a9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.264437 AutoTransform-1.1.1a9/examples/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/examples/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      979 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/examples/docker/docker_autotransform.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      993 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/examples/docker/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/examples/manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/examples/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/examples/scheduler.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.264437 AutoTransform-1.1.1a9/examples/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/examples/schemas/black_format.json
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/examples/schemas/schema_map.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.264437 AutoTransform-1.1.1a9/examples/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/examples/workflows/autotransform.manage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/examples/workflows/autotransform.run.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/examples/workflows/autotransform.schedule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/examples/workflows/autotransform.update.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-04 22:55:42.312437 AutoTransform-1.1.1a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.252437 AutoTransform-1.1.1a9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.252437 AutoTransform-1.1.1a9/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.268437 AutoTransform-1.1.1a9/src/python/AutoTransform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2023-10-04 22:55:42.000000 AutoTransform-1.1.1a9/src/python/AutoTransform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2023-10-04 22:55:42.000000 AutoTransform-1.1.1a9/src/python/AutoTransform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 22:55:42.000000 AutoTransform-1.1.1a9/src/python/AutoTransform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-04 22:55:42.000000 AutoTransform-1.1.1a9/src/python/AutoTransform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2023-10-04 22:55:42.000000 AutoTransform-1.1.1a9/src/python/AutoTransform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-04 22:55:42.000000 AutoTransform-1.1.1a9/src/python/AutoTransform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.268437 AutoTransform-1.1.1a9/src/python/autotransform/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.272437 AutoTransform-1.1.1a9/src/python/autotransform/batcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/batcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/batcher/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/batcher/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/batcher/codeowners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/batcher/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/batcher/extradata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/batcher/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/batcher/single.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.272437 AutoTransform-1.1.1a9/src/python/autotransform/change/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/change/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/change/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10008 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/change/github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.272437 AutoTransform-1.1.1a9/src/python/autotransform/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/command/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/command/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.276437 AutoTransform-1.1.1a9/src/python/autotransform/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21463 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/config/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/config/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/config/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.280437 AutoTransform-1.1.1a9/src/python/autotransform/event/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/logginglevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/remoterun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/schedulerun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/event/warning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.284437 AutoTransform-1.1.1a9/src/python/autotransform/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/filter/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/filter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/filter/codeowners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/filter/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/filter/key_hash_shard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/filter/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/filter/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/filter/shard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.284437 AutoTransform-1.1.1a9/src/python/autotransform/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/input/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/input/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/input/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/input/gitgrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/input/inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/input/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/input/target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.288437 AutoTransform-1.1.1a9/src/python/autotransform/item/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/item/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/item/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.288437 AutoTransform-1.1.1a9/src/python/autotransform/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/model/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.292437 AutoTransform-1.1.1a9/src/python/autotransform/repo/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/repo/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/repo/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9108 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/repo/github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.296437 AutoTransform-1.1.1a9/src/python/autotransform/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/runner/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/runner/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/runner/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/runner/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.296437 AutoTransform-1.1.1a9/src/python/autotransform/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/schema/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/schema/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16005 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/schema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.296437 AutoTransform-1.1.1a9/src/python/autotransform/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.300437 AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12182 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13430 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/scripts/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.300437 AutoTransform-1.1.1a9/src/python/autotransform/scripts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/scripts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/scripts/migrations/p1_0_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/scripts/migrations/p1_0_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/scripts/migrations/p1_0_5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.300437 AutoTransform-1.1.1a9/src/python/autotransform/step/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.300437 AutoTransform-1.1.1a9/src/python/autotransform/step/action/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/action/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/action/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/action/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/action/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/action/reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/action/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.304437 AutoTransform-1.1.1a9/src/python/autotransform/step/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/condition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/condition/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11919 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/condition/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/condition/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/condition/created.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/condition/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/condition/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/condition/reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/condition/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/condition/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/condition/updated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/step/conditional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.308437 AutoTransform-1.1.1a9/src/python/autotransform/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/transformer/aimodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/transformer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/transformer/jscodeshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/transformer/libcst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/transformer/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/transformer/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/transformer/single.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.308437 AutoTransform-1.1.1a9/src/python/autotransform/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/util/cachedfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15661 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/util/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/util/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/util/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/util/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18520 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/util/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/util/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/util/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16810 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/util/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/util/schema_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 22:55:42.312437 AutoTransform-1.1.1a9/src/python/autotransform/validator/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2023-10-04 22:53:42.000000 AutoTransform-1.1.1a9/src/python/autotransform/validator/script.py
```

### Comparing `AutoTransform-1.1.1a8/BEST_PRACTICES.md` & `AutoTransform-1.1.1a9/BEST_PRACTICES.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/COMPONENTS.md` & `AutoTransform-1.1.1a9/COMPONENTS.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/CONTRIBUTING.md` & `AutoTransform-1.1.1a9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/CUSTOM_DEPLOYMENT.md` & `AutoTransform-1.1.1a9/CUSTOM_DEPLOYMENT.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/LICENSE` & `AutoTransform-1.1.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/MANAGE_CHANGES.md` & `AutoTransform-1.1.1a9/MANAGE_CHANGES.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/PKG-INFO` & `AutoTransform-1.1.1a9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: AutoTransform
-Version: 1.1.1a8
-Summary: A component based framework for designing automated code modification
-Home-page: https://github.com/nathro/AutoTransform
-Author: Nathan Rockenbach
-Author-email: nathro.software@gmail.com
-Project-URL: Source, https://github.com/nathro/AutoTransform/
-Project-URL: Bug Tracker, https://github.com/nathro/AutoTransform/issues
-Keywords: codemod,automation,code change,codeshift,transformation,maintain
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # **Overview**
 
 Full documentation available [here](https://autotransform.readthedocs.io)
 Check out our [tutorial videos](https://www.youtube.com/watch?v=JGtzxWqa6s0&list=PLw32rS7srmZYUV3VfE114ZLYqHzQc9wY9)
 
 ## **Installing**
 
@@ -73,8 +54,8 @@
 
 ### **Run Time Logging**
 
 In addition to static typing, a codemod could instrument untyped functions or other code to log types at run time. These logs could then be fed into the codemod to add types to code that can’t be inferred but can be determined at run time. This codemod could additionally be written to only instrument a small part of the codebase at a given time, preventing excessive resource utilization.
 
 ### **The Whole Versus the Sum of the Parts**
 
-Each codemod that can change code can benefit from all other codemods. As run time logging adds types, static inference can make better changes. Dead code removal can clean up untyped code. The layered passes, and building on top of the changes of each codemod, can produce significantly greater wins.
+Each codemod that can change code can benefit from all other codemods. As run time logging adds types, static inference can make better changes. Dead code removal can clean up untyped code. The layered passes, and building on top of the changes of each codemod, can produce significantly greater wins.
```

### Comparing `AutoTransform-1.1.1a8/README.md` & `AutoTransform-1.1.1a9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: AutoTransform
+Version: 1.1.1a9
+Summary: A component based framework for designing automated code modification
+Home-page: https://github.com/nathro/AutoTransform
+Author: Nathan Rockenbach
+Author-email: nathro.software@gmail.com
+Project-URL: Source, https://github.com/nathro/AutoTransform/
+Project-URL: Bug Tracker, https://github.com/nathro/AutoTransform/issues
+Keywords: codemod,automation,code change,codeshift,transformation,maintain
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: GitPython==3.1.32
+Requires-Dist: ghapi==1.0.3
+Requires-Dist: typing-extensions==4.4.0
+Requires-Dist: colorama==0.4.6
+Requires-Dist: pytz==2022.7.1
+Requires-Dist: pydantic==1.10.4
+Requires-Dist: libcst==0.4.9
+Requires-Dist: requests==2.31.0
+Requires-Dist: codeowners==0.6.0
+Requires-Dist: openai==0.27.8
+
 # **Overview**
 
 Full documentation available [here](https://autotransform.readthedocs.io)
 Check out our [tutorial videos](https://www.youtube.com/watch?v=JGtzxWqa6s0&list=PLw32rS7srmZYUV3VfE114ZLYqHzQc9wY9)
 
 ## **Installing**
 
@@ -54,8 +83,8 @@
 
 ### **Run Time Logging**
 
 In addition to static typing, a codemod could instrument untyped functions or other code to log types at run time. These logs could then be fed into the codemod to add types to code that can’t be inferred but can be determined at run time. This codemod could additionally be written to only instrument a small part of the codebase at a given time, preventing excessive resource utilization.
 
 ### **The Whole Versus the Sum of the Parts**
 
-Each codemod that can change code can benefit from all other codemods. As run time logging adds types, static inference can make better changes. Dead code removal can clean up untyped code. The layered passes, and building on top of the changes of each codemod, can produce significantly greater wins.
+Each codemod that can change code can benefit from all other codemods. As run time logging adds types, static inference can make better changes. Dead code removal can clean up untyped code. The layered passes, and building on top of the changes of each codemod, can produce significantly greater wins.
```

### Comparing `AutoTransform-1.1.1a8/SCHEDULED_RUNS.md` & `AutoTransform-1.1.1a9/SCHEDULED_RUNS.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/examples/docker/docker_autotransform.sh` & `AutoTransform-1.1.1a9/examples/docker/docker_autotransform.sh`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/examples/docker/entrypoint.sh` & `AutoTransform-1.1.1a9/examples/docker/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/examples/manager.json` & `AutoTransform-1.1.1a9/examples/manager.json`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/examples/schemas/black_format.json` & `AutoTransform-1.1.1a9/examples/schemas/black_format.json`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/examples/workflows/autotransform.manage.yml` & `AutoTransform-1.1.1a9/examples/workflows/autotransform.manage.yml`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/examples/workflows/autotransform.run.yml` & `AutoTransform-1.1.1a9/examples/workflows/autotransform.run.yml`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/examples/workflows/autotransform.schedule.yml` & `AutoTransform-1.1.1a9/examples/workflows/autotransform.schedule.yml`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/examples/workflows/autotransform.update.yml` & `AutoTransform-1.1.1a9/examples/workflows/autotransform.update.yml`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/setup.py` & `AutoTransform-1.1.1a9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         data_files.append((f"autotransform-{path}", [os.path.join(path, file) for file in files]))
 
     return data_files
 
 
 setuptools.setup(
     name="AutoTransform",
-    version="1.1.1a8",
+    version="1.1.1a9",
     author="Nathan Rockenbach",
     author_email="nathro.software@gmail.com",
     description="A component based framework for designing automated code modification",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nathro/AutoTransform",
     project_urls={
```

### Comparing `AutoTransform-1.1.1a8/src/python/AutoTransform.egg-info/PKG-INFO` & `AutoTransform-1.1.1a9/src/python/AutoTransform.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoTransform
-Version: 1.1.1a8
+Version: 1.1.1a9
 Summary: A component based framework for designing automated code modification
 Home-page: https://github.com/nathro/AutoTransform
 Author: Nathan Rockenbach
 Author-email: nathro.software@gmail.com
 Project-URL: Source, https://github.com/nathro/AutoTransform/
 Project-URL: Bug Tracker, https://github.com/nathro/AutoTransform/issues
 Keywords: codemod,automation,code change,codeshift,transformation,maintain
@@ -12,14 +12,24 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: GitPython==3.1.32
+Requires-Dist: ghapi==1.0.3
+Requires-Dist: typing-extensions==4.4.0
+Requires-Dist: colorama==0.4.6
+Requires-Dist: pytz==2022.7.1
+Requires-Dist: pydantic==1.10.4
+Requires-Dist: libcst==0.4.9
+Requires-Dist: requests==2.31.0
+Requires-Dist: codeowners==0.6.0
+Requires-Dist: openai==0.27.8
 
 # **Overview**
 
 Full documentation available [here](https://autotransform.readthedocs.io)
 Check out our [tutorial videos](https://www.youtube.com/watch?v=JGtzxWqa6s0&list=PLw32rS7srmZYUV3VfE114ZLYqHzQc9wY9)
 
 ## **Installing**
```

### Comparing `AutoTransform-1.1.1a8/src/python/AutoTransform.egg-info/SOURCES.txt` & `AutoTransform-1.1.1a9/src/python/AutoTransform.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -49,39 +49,46 @@
 src/python/autotransform/config/fetcher.py
 src/python/autotransform/event/__init__.py
 src/python/autotransform/event/action.py
 src/python/autotransform/event/base.py
 src/python/autotransform/event/debug.py
 src/python/autotransform/event/handler.py
 src/python/autotransform/event/logginglevel.py
+src/python/autotransform/event/model.py
 src/python/autotransform/event/remoterun.py
 src/python/autotransform/event/run.py
 src/python/autotransform/event/schedulerun.py
+src/python/autotransform/event/script.py
 src/python/autotransform/event/type.py
 src/python/autotransform/event/update.py
 src/python/autotransform/event/verbose.py
 src/python/autotransform/event/warning.py
 src/python/autotransform/filter/__init__.py
 src/python/autotransform/filter/aggregate.py
 src/python/autotransform/filter/base.py
 src/python/autotransform/filter/codeowners.py
+src/python/autotransform/filter/file.py
 src/python/autotransform/filter/key_hash_shard.py
 src/python/autotransform/filter/regex.py
 src/python/autotransform/filter/script.py
 src/python/autotransform/filter/shard.py
 src/python/autotransform/input/__init__.py
 src/python/autotransform/input/base.py
 src/python/autotransform/input/directory.py
 src/python/autotransform/input/empty.py
 src/python/autotransform/input/gitgrep.py
 src/python/autotransform/input/inline.py
 src/python/autotransform/input/script.py
+src/python/autotransform/input/target.py
 src/python/autotransform/item/__init__.py
 src/python/autotransform/item/base.py
 src/python/autotransform/item/file.py
+src/python/autotransform/model/__init__.py
+src/python/autotransform/model/base.py
+src/python/autotransform/model/openai.py
 src/python/autotransform/repo/__init__.py
 src/python/autotransform/repo/base.py
 src/python/autotransform/repo/git.py
 src/python/autotransform/repo/github.py
 src/python/autotransform/runner/__init__.py
 src/python/autotransform/runner/base.py
 src/python/autotransform/runner/github.py
@@ -122,18 +129,18 @@
 src/python/autotransform/step/condition/labels.py
 src/python/autotransform/step/condition/request.py
 src/python/autotransform/step/condition/reviewers.py
 src/python/autotransform/step/condition/schema.py
 src/python/autotransform/step/condition/state.py
 src/python/autotransform/step/condition/updated.py
 src/python/autotransform/transformer/__init__.py
+src/python/autotransform/transformer/aimodel.py
 src/python/autotransform/transformer/base.py
 src/python/autotransform/transformer/jscodeshift.py
 src/python/autotransform/transformer/libcst.py
-src/python/autotransform/transformer/openai.py
 src/python/autotransform/transformer/regex.py
 src/python/autotransform/transformer/script.py
 src/python/autotransform/transformer/single.py
 src/python/autotransform/util/__init__.py
 src/python/autotransform/util/cachedfile.py
 src/python/autotransform/util/component.py
 src/python/autotransform/util/console.py
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/__init__.py` & `AutoTransform-1.1.1a9/src/python/autotransform/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/batcher/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/batcher/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/batcher/chunk.py` & `AutoTransform-1.1.1a9/src/python/autotransform/batcher/chunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,14 @@
         if self.max_chunks is not None and len(items) / chunk_size > self.max_chunks:
             chunk_size = ceil(len(items) / self.max_chunks)
 
         # Create Batches
         item_chunks = [items[i : i + chunk_size] for i in range(0, len(items), chunk_size)]
         item_batches: List[Batch] = []
         for idx, item_chunk in enumerate(item_chunks, start=1):
-            title = f"[{idx}/{len(item_chunks)}] " + self.title
+            title = f"[{idx}/{len(item_chunks)}] {self.title}"
             batch: Batch = {"items": item_chunk, "title": title}
             if self.metadata is not None:
                 # Deepcopy metadata to ensure mutations don't apply to all Batches
                 batch["metadata"] = deepcopy(self.metadata)
             item_batches.append(batch)
         return item_batches
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/batcher/directory.py` & `AutoTransform-1.1.1a9/src/python/autotransform/batcher/directory.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for the DirectoryBatcher."""
 
-from __future__ import annotations
-
+from collections import defaultdict
 import pathlib
 from copy import deepcopy
 from typing import Any, ClassVar, Dict, List, Optional, Sequence
 
 from autotransform.batcher.base import Batch, Batcher, BatcherName
 from autotransform.item.base import Item
 from autotransform.item.file import FileItem
@@ -43,25 +42,23 @@
             items (Sequence[Item]): The filtered Items to separate.
 
         Returns:
             List[Batch]: A list containing a Batch for each directory containing files.
         """
 
         # Get a mapping from directory to items within that directory
-        item_map: Dict[str, List[FileItem]] = {}
+        item_map: Dict[str, List[FileItem]] = defaultdict(list)
         for item in items:
             assert isinstance(item, FileItem)
             directory = str(pathlib.Path(item.get_path()).parent).replace("\\", "/")
-            if directory not in item_map:
-                item_map[directory] = []
             item_map[directory].append(item)
 
         # Create Batches
         batches: List[Batch] = [
-            {"items": batch_items, "title": self.prefix + ": " + directory}
+            {"items": batch_items, "title": f"{self.prefix}: {directory}"}
             for directory, batch_items in item_map.items()
         ]
 
         if self.metadata is not None:
             for batch in batches:
                 # Deepcopy metadata to ensure mutations don't apply to all Batches
                 batch["metadata"] = deepcopy(self.metadata)
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/batcher/extradata.py` & `AutoTransform-1.1.1a9/src/python/autotransform/batcher/extradata.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for the ExtraDataBatcher."""
 
-from __future__ import annotations
-
-from copy import deepcopy
+from collections import defaultdict
 from typing import Any, ClassVar, Dict, List, Sequence
 
 from pydantic import Field
 
 from autotransform.batcher.base import Batch, Batcher, BatcherName
 from autotransform.item.base import Item
 
@@ -42,37 +40,30 @@
         Args:
             items (Sequence[Item]): The filtered Items to separate.
 
         Returns:
             List[Batch]: A list of Batches grouped by the extra_data of the Items.
         """
 
-        groups: Dict[str, List[Item]] = {}
+        groups: Dict[str, List[Item]] = defaultdict(list)
         for item in items:
             extra_data = item.extra_data or {}
             group_by_val = extra_data[self.group_by]
             assert isinstance(group_by_val, str), "Group by values must be strings"
-            if group_by_val in groups:
-                groups[group_by_val].append(item)
-            else:
-                groups[group_by_val] = [item]
+            groups[group_by_val].append(item)
 
         batches: List[Batch] = []
         for group_title, group_items in groups.items():
             batch: Batch = {"items": group_items, "title": group_title}
             if self.metadata_keys:
-                metadata: Dict[str, List[Any]] = {}
-                for key in self.metadata_keys:
-                    metadata[key] = []
+                metadata: Dict[str, List[Any]] = {key: [] for key in self.metadata_keys}
                 for item in group_items:
                     extra_data = item.extra_data or {}
                     for key in self.metadata_keys:
                         val = extra_data.get(key)
                         if isinstance(val, list):
-                            metadata[key].extend(deepcopy(val))
+                            metadata[key].extend(val)
                         elif val is not None:
-                            metadata[key].append(deepcopy(val))
-                for key in self.metadata_keys:
-                    metadata[key] = list(set(metadata[key]))
-                batch["metadata"] = metadata
+                            metadata[key].append(val)
+                batch["metadata"] = {key: list(set(values)) for key, values in metadata.items()}
             batches.append(batch)
         return batches
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/batcher/regex.py` & `AutoTransform-1.1.1a9/src/python/autotransform/batcher/regex.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # @black_format
 
 """The implementation for the RegexBatcher."""
 
 from __future__ import annotations
 
 import re
+from collections import defaultdict
 from typing import Any, ClassVar, Dict, List, Sequence
 
 from pydantic import Field
 
 from autotransform.batcher.base import Batch, Batcher, BatcherName
 from autotransform.item.base import Item
 from autotransform.item.file import FileItem
@@ -42,36 +43,31 @@
         Args:
             items (Sequence[Item]): The filtered Items to separate.
 
         Returns:
             List[Batch]: A list of Batches grouped by the extra_data of the Items.
         """
 
-        groups: Dict[str, List[FileItem]] = {}
+        groups: Dict[str, List[FileItem]] = defaultdict(list)
         for item in items:
             assert isinstance(item, FileItem)
-            match = re.match(item.get_content(), self.group_by)
+            match = re.match(self.group_by, item.get_content())
             assert match is not None, "Must have value to use for grouping"
             group_by_val = match.group(1)
-            if group_by_val in groups:
-                groups[group_by_val].append(item)
-            else:
-                groups[group_by_val] = [item]
+            groups[group_by_val].append(item)
 
         batches: List[Batch] = []
         for group_title, group_items in groups.items():
             batch: Batch = {"items": group_items, "title": group_title}
             if self.metadata_keys:
-                metadata: Dict[str, List[Any]] = {}
-                for key in self.metadata_keys:
-                    metadata[key] = []
+                metadata: Dict[str, List[Any]] = defaultdict(list)
                 for item in group_items:
                     file_content = item.get_content()
                     for key, regex in self.metadata_keys.items():
-                        match = re.match(file_content, regex)
+                        match = re.match(regex, file_content)
                         if match:
                             metadata[key].append(match.group(1))
-                for key in self.metadata_keys:
+                for key in metadata:
                     metadata[key] = list(set(metadata[key]))
                 batch["metadata"] = metadata
             batches.append(batch)
         return batches
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/batcher/single.py` & `AutoTransform-1.1.1a9/src/python/autotransform/batcher/single.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             items (Sequence[Item]): The filtered Items to separate.
 
         Returns:
             List[Batch]: A list containing a single Batch for all Items.
         """
 
         # Skip if empty when setting is enabled
-        if self.skip_empty_batch and len(items) == 0:
+        if self.skip_empty_batch and not items:
             return []
 
         # Create Batch
         batch: Batch = {
             "items": items,
             "title": self.title,
         }
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/change/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/change/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/change/github.py` & `AutoTransform-1.1.1a9/src/python/autotransform/change/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,71 @@
         name (ClassVar[ChangeName]): The name of the Component.
     """
 
     full_github_name: str
     pull_number: int
     name: ClassVar[ChangeName] = ChangeName.GITHUB
 
+    @cached_property
+    def _pull_request(self) -> PullRequest:
+        """Gets the Pull Request.
+
+        Returns:
+            PullRequest: The Pull Request.
+        """
+
+        return GithubUtils.get(self.full_github_name).get_pull_request(self.pull_number)
+
+    @cached_property
+    def _automation_data(self) -> Tuple[AutoTransformSchema, Batch]:
+        """Loads the Schema and Batch data for the GithubChange as a cached property.
+
+        Returns:
+            Tuple[AutoTransformSchema, Batch]: The Schema and Batch contained
+                in the PullRequest's Body.
+        """
+
+        gist_match = re.search("<<<Automation Info Gist: (.*)>>>", self._pull_request.body)
+        if gist_match:
+            gist_ids = gist_match.groups()[0].split("/")
+            gist = GithubUtils.get(self.full_github_name).get_gist(gist_ids[0])
+            schema_data = gist.get_file_content("schema") or ""
+            batch = json.loads(gist.get_file_content("batch") or "")
+            assert isinstance(batch["items"], List)
+            for i in range(1, len(gist_ids)):
+                gist = GithubUtils.get(self.full_github_name).get_gist(gist_ids[i])
+                items = json.loads(gist.get_file_content("items") or "[]")
+                assert isinstance(items, List)
+                batch["items"].extend(items)
+        else:
+            cur_line_placement = None
+            data_lines: Dict[str, List[str]] = {"schema": [], "batch": []}
+            for line in self._pull_request.body.splitlines():
+                if line == GithubUtils.BEGIN_SCHEMA:
+                    cur_line_placement = "schema"
+                elif line == GithubUtils.END_SCHEMA:
+                    cur_line_placement = None
+                elif line == GithubUtils.BEGIN_BATCH:
+                    cur_line_placement = "batch"
+                elif line == GithubUtils.END_BATCH:
+                    cur_line_placement = None
+                elif cur_line_placement is not None:
+                    data_lines[cur_line_placement].append(line)
+            schema_data = "\n".join(data_lines["schema"])
+            batch = json.loads("\n".join(data_lines["batch"]))
+
+        schema = AutoTransformSchema.from_data(json.loads(schema_data))
+        items = [item_factory.get_instance(item) for item in batch["items"]]
+        batch = {
+            "items": items,
+            "metadata": batch["metadata"],
+            "title": str(batch["title"]),
+        }
+        return (schema, batch)
+
     def get_batch(self) -> Batch:
         """Gets the Batch that was used to produce the Change.
 
         Returns:
             Batch: The Batch used to produce the Change.
         """
 
@@ -91,23 +148,14 @@
 
         Returns:
             ChangeState: The mergeable state of the Change.
         """
 
         return self._pull_request.get_mergeable_state()
 
-    def get_review_state(self) -> ReviewState:
-        """Gets the current review state of the Change.
-
-        Returns:
-            ReviewState: The current review state of the Change.
-        """
-
-        return self._review_state
-
     @cached_property
     def _review_state(self) -> ReviewState:
         """The current review state of the Change as a cached property.
 
         Returns:
             ReviewState: The current review state of the Change.
         """
@@ -115,22 +163,22 @@
         review_state = self._pull_request.get_review_state()
         if review_state == "APPROVED":
             return ReviewState.APPROVED
         if review_state == "CHANGES_REQUESTED":
             return ReviewState.CHANGES_REQUESTED
         return ReviewState.NEEDS_REVIEW
 
-    def get_test_state(self) -> TestState:
-        """Gets the current test state of the Change.
+    def get_review_state(self) -> ReviewState:
+        """Gets the current review state of the Change.
 
         Returns:
-            TestState: The current test state of the Change.
+            ReviewState: The current review state of the Change.
         """
 
-        return self._test_state
+        return self._review_state
 
     @cached_property
     def _test_state(self) -> TestState:
         """The current test state of the Change as a cached property.
 
         Returns:
             TestState: The current test state of the Change.
@@ -139,14 +187,23 @@
         state = self._pull_request.get_test_state()
         if state == "pending":
             return TestState.PENDING
         if state in ["success", "neutral"]:
             return TestState.SUCCESS
         return TestState.FAILURE
 
+    def get_test_state(self) -> TestState:
+        """Gets the current test state of the Change.
+
+        Returns:
+            TestState: The current test state of the Change.
+        """
+
+        return self._test_state
+
     def get_labels(self) -> List[str]:
         """Gets all labels for a Change.
 
         Returns:
             List[str]: The list of labels.
         """
 
@@ -191,17 +248,15 @@
     def abandon(self) -> bool:
         """Close the Pull Request and delete the associated branch.
 
         Returns:
             bool: Whether the abandon was completed successfully.
         """
 
-        if not self._pull_request.close():
-            return False
-        return self._pull_request.delete_branch()
+        return self._pull_request.close() and self._pull_request.delete_branch()
 
     def add_labels(self, labels: List[str]) -> bool:
         """Adds labels to an outstanding Change.
 
         Args:
             labels (List[str]): The labels to add.
 
@@ -242,80 +297,21 @@
     def merge(self) -> bool:
         """Merges the Pull Request and deletes the branch.
 
         Returns:
             bool: Whether the merge was completed successfully.
         """
 
-        if not self._pull_request.merge():
-            return False
-        return self._pull_request.delete_branch()
+        return self._pull_request.merge() and self._pull_request.delete_branch()
 
     def remove_label(self, label: str) -> bool:
         """Removes a label from an outstanding Change.
 
         Args:
             label (str): The label to remove.
 
         Returns:
             bool: Whether the label was removed successfully.
         """
 
         self._pull_request.remove_label(label)
         return True
-
-    @property
-    def _pull_request(self) -> PullRequest:
-        """Gets the Pull Request.
-
-        Returns:
-            PullRequest: The Pull Request.
-        """
-
-        return GithubUtils.get(self.full_github_name).get_pull_request(self.pull_number)
-
-    @cached_property
-    def _automation_data(self) -> Tuple[AutoTransformSchema, Batch]:
-        """Loads the Schema and Batch data for the GithubChange as a cached property.
-
-        Returns:
-            Tuple[AutoTransformSchema, Batch]: The Schema and Batch contained
-                in the PullRequest's Body.
-        """
-
-        gist_match = re.search("<<<Automation Info Gist: (.*)>>>", self._pull_request.body)
-        if gist_match:
-            gist_ids = gist_match.groups()[0].split("/")
-            gist = GithubUtils.get(self.full_github_name).get_gist(gist_ids[0])
-            schema_data = gist.get_file_content("schema") or ""
-            batch = json.loads(gist.get_file_content("batch") or "")
-            assert isinstance(batch["items"], List)
-            for i in range(1, len(gist_ids)):
-                gist = GithubUtils.get(self.full_github_name).get_gist(gist_ids[i])
-                items = json.loads(gist.get_file_content("items") or "[]")
-                assert isinstance(items, List)
-                batch["items"].extend(items)
-        else:
-            cur_line_placement = None
-            data_lines: Dict[str, List[str]] = {"schema": [], "batch": []}
-            for line in self._pull_request.body.splitlines():
-                if line == GithubUtils.BEGIN_SCHEMA:
-                    cur_line_placement = "schema"
-                elif line == GithubUtils.END_SCHEMA:
-                    cur_line_placement = None
-                elif line == GithubUtils.BEGIN_BATCH:
-                    cur_line_placement = "batch"
-                elif line == GithubUtils.END_BATCH:
-                    cur_line_placement = None
-                elif cur_line_placement is not None:
-                    data_lines[cur_line_placement].append(line)
-            schema_data = "\n".join(data_lines["schema"])
-            batch = json.loads("\n".join(data_lines["batch"]))
-
-        schema = AutoTransformSchema.from_data(json.loads(schema_data))
-        items = [item_factory.get_instance(item) for item in batch["items"]]
-        batch = {
-            "items": items,
-            "metadata": batch["metadata"],
-            "title": str(batch["title"]),
-        }
-        return (schema, batch)
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/command/__init__.py` & `AutoTransform-1.1.1a9/src/python/autotransform/command/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/command/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/command/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/command/script.py` & `AutoTransform-1.1.1a9/src/python/autotransform/command/script.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,36 +12,38 @@
 from __future__ import annotations
 
 from typing import Any, ClassVar, List, Mapping, Optional, Sequence
 
 import autotransform.schema
 from autotransform.batcher.base import Batch
 from autotransform.command.base import Command, CommandName
-from autotransform.event.handler import EventHandler
-from autotransform.event.verbose import VerboseEvent
 from autotransform.item.base import Item
 from autotransform.item.file import FileItem
 from autotransform.util.functions import run_cmd_on_items
 
 
 class ScriptCommand(Command):
     """Runs a script with the supplied arguments to perform a command. If the per_item flag is
     set, the script will be invoked on each Item. If run_on_changes is set to True, the script
     will replace the Batch Items with FileItems for each changed file. Sentinel values can be
     used in args to provide custom arguments for a run.
     The available sentinel values for args are:
-        <<KEY>>: A json encoded list of the Items for a Batch. If the per_item flag is set
-            this will simply be the key of an Item.
+        <<KEY>>: A list of the Items for a Batch. If the per_item flag is set this will simply
+            be the key of an Item.
         <<EXTRA_DATA>>: A JSON encoded mapping from Item key to that Item's extra_data. If the
             per_item flag is set, this will simply be a JSON encoding of the Item's extra_data.
             If extra_data is not present for an item, it is treated as an empty Dict.
         <<METADATA>>: A JSON encoded version of the Batch's metadata.
     _FILE can be appended to any of these (i.e. <<KEY_FILE>>) and the arg will instead be replaced
      with a path to a file containing the value.
 
+    Additionally, <<EXTRA_DATA/some_key>> can be used as a sentinel value to get a list of all the
+    values from extra_data for each item with that key. Values will be converted to strings and
+    returned as a list.
+
     Attributes:
         args (List[str]): The arguments to supply to the script.
         script (str): The script to run.
         per_item (bool, optional): Whether to run the script on each item. Defaults to False.
         run_on_changes (bool, optional): Whether to replace the Items in the batch with
             FileItems for the changed files. Defaults to False.
         run_pre_validation (bool, optional): Whether to run the command before validation is done.
@@ -62,87 +64,67 @@
         on the entire Batch, based on the per_item flag.
 
         Args:
             batch (Batch): The transformed Batch to run against.
             _transform_data (Optional[Mapping[str, Any]]): Data from the transformation. Unused.
         """
 
-        if not self.per_item:
-            self._run_batch(batch)
+        items = self._get_items(batch)
+
+        if self.per_item:
+            for item in items:
+                self._run_single(item, batch.get("metadata", None))
             return
+
+        self._run_batch(batch, items)
+
+    def _get_items(self, batch: Batch) -> Sequence[Item]:
+        """Get items based on the run_on_changes flag.
+
+        Args:
+            batch (Batch): The transformed Batch to run against.
+
+        Returns:
+            Sequence[Item]: The sequence of items to be processed.
+        """
         if self.run_on_changes:
             current_schema = autotransform.schema.current
             assert current_schema is not None
             repo = current_schema.repo
             assert repo is not None
-            items: Sequence[Item] = [FileItem(key=file) for file in repo.get_changed_files(batch)]
-        else:
-            items = batch["items"]
+            return [FileItem(key=file) for file in repo.get_changed_files(batch)]
 
-        for item in items:
-            self._run_single(item, batch.get("metadata", None))
+        return batch["items"]
 
     def _run_single(self, item: Item, batch_metadata: Optional[Mapping[str, Any]]) -> None:
         """Executes a simple script to run a command on a single Item.
 
         Args:
             item (Item): The Item that will be validated.
             batch_metadata (Optional[Mapping[str, Any]]): The metadata of the Batch containing the
                 Item.
         """
+        self._run_script([item], batch_metadata or {})
 
-        event_handler = EventHandler.get()
-
-        # Get Command
-        cmd = [self.script]
-        cmd.extend(self.args)
-
-        proc = run_cmd_on_items(cmd, [item], batch_metadata or {})
-
-        # Handle output
-        if proc.stdout.strip() != "":
-            event_handler.handle(VerboseEvent({"message": f"STDOUT:\n{proc.stdout.strip()}"}))
-        else:
-            event_handler.handle(VerboseEvent({"message": "No STDOUT"}))
-        if proc.stderr.strip() != "":
-            event_handler.handle(VerboseEvent({"message": f"STDERR:\n{proc.stderr.strip()}"}))
-        else:
-            event_handler.handle(VerboseEvent({"message": "No STDERR"}))
-        proc.check_returncode()
-
-    def _run_batch(self, batch: Batch) -> None:
+    def _run_batch(self, batch: Batch, items: Sequence[Item]) -> None:
         """Executes a simple script against the given Batch.
 
         Args:
             batch (Batch): The batch that will be run against.
+            items (Sequence[Item]): The sequence of items to be processed.
         """
+        self._run_script(items, batch.get("metadata", {}))
 
-        event_handler = EventHandler.get()
+    def _run_script(self, items: Sequence[Item], metadata: Mapping[str, Any]) -> None:
+        """Executes a simple script against the given items.
 
-        # Get items
-        if self.run_on_changes:
-            current_schema = autotransform.schema.current
-            assert current_schema is not None
-            repo = current_schema.repo
-            assert repo is not None
-            items: Sequence[Item] = [FileItem(key=file) for file in repo.get_changed_files(batch)]
-            if len(items) == 0:
-                return
-        else:
-            items = batch["items"]
+        Args:
+            items (Sequence[Item]): The sequence of items to be processed.
+            metadata (Mapping[str, Any]): The metadata of the Batch containing the items.
+        """
 
         # Get Command
         cmd = [self.script]
         cmd.extend(self.args)
 
-        proc = run_cmd_on_items(cmd, items, batch.get("metadata", {}))
-
-        # Handle output
-        if proc.stdout.strip() != "":
-            event_handler.handle(VerboseEvent({"message": f"STDOUT:\n{proc.stdout.strip()}"}))
-        else:
-            event_handler.handle(VerboseEvent({"message": "No STDOUT"}))
-        if proc.stderr.strip() != "":
-            event_handler.handle(VerboseEvent({"message": f"STDERR:\n{proc.stderr.strip()}"}))
-        else:
-            event_handler.handle(VerboseEvent({"message": "No STDERR"}))
+        proc = run_cmd_on_items(cmd, items, metadata)
         proc.check_returncode()
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/config/__init__.py` & `AutoTransform-1.1.1a9/src/python/autotransform/config/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/config/config.py` & `AutoTransform-1.1.1a9/src/python/autotransform/config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,15 +548,16 @@
                 component_directory=Config.get_component_directory_from_console(
                     prev_config=prev_config, simple=simple
                 ),
                 local_runner=Config.get_local_runner_from_console(
                     prev_config=prev_config, simple=simple
                 ),
                 open_ai_api_key=Config.get_open_ai_api_key_from_console(
-                    prev_config=prev_config, simple=simple,
+                    prev_config=prev_config,
+                    simple=simple,
                 ),
                 remote_runner=Config.get_remote_runner_from_console(
                     prev_config=prev_config, use_github=github, use_jenkins=jenkins, simple=simple
                 ),
                 repo_override=Config.get_repo_override_from_console(
                     prev_config=prev_config, simple=simple
                 ),
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/config/default.py` & `AutoTransform-1.1.1a9/src/python/autotransform/config/default.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/config/environment.py` & `AutoTransform-1.1.1a9/src/python/autotransform/config/environment.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/config/fetcher.py` & `AutoTransform-1.1.1a9/src/python/autotransform/config/fetcher.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/event/__init__.py` & `AutoTransform-1.1.1a9/src/python/autotransform/event/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/event/action.py` & `AutoTransform-1.1.1a9/src/python/autotransform/event/action.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/event/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/event/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/event/debug.py` & `AutoTransform-1.1.1a9/src/python/autotransform/event/debug.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/event/handler.py` & `AutoTransform-1.1.1a9/src/python/autotransform/event/handler.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/event/logginglevel.py` & `AutoTransform-1.1.1a9/src/python/autotransform/event/logginglevel.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/event/remoterun.py` & `AutoTransform-1.1.1a9/src/python/autotransform/event/remoterun.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/event/run.py` & `AutoTransform-1.1.1a9/src/python/autotransform/event/schedulerun.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,47 +3,46 @@
 #
 # Licensed under the MIT License <http://opensource.org/licenses/MIT>
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
-"""The ScriptRunEvent is triggered whenever an AutoTransform script is run and provides
-information on the run.
+"""The ScheduleRunEvent is triggered whenever an AutoTransformSchema is scheduled to be run
+by the schedule command of the AutoTransform script.
 """
 
-from typing import Dict, TypedDict
+from typing import TypedDict
 
 from autotransform.event.base import Event
 from autotransform.event.logginglevel import LoggingLevel
 from autotransform.event.type import EventType
 
 
-class ScriptRunEventData(TypedDict):
-    """The data for a ScriptRunEvent. Contains the information that will be
+class ScheduleRunEventData(TypedDict):
+    """The data for a ScheduleRunEvent. Contains the information that will be
     logged when the event is triggered."""
 
-    args: Dict[str, str]
-    script: str
+    schema_name: str
 
 
-class ScriptRunEvent(Event[ScriptRunEventData]):
-    """A ScriptRunEvent is triggered whenever an AutoTransform script is run. Logs details
-    of the run.
+class ScheduleRunEvent(Event[ScheduleRunEventData]):
+    """A ScheduleRunEvent is triggered whenever an AutoTransformSchema is scheduled to be
+    run by the schedule command and logs the schedule.
     """
 
     @staticmethod
     def get_type() -> EventType:
         """Used to represent the type of Event, output to logs.
 
         Returns:
             EventType: The unique type associated with this Event.
         """
 
-        return EventType.SCRIPT_RUN
+        return EventType.SCHEDULE_RUN
 
     @staticmethod
     def get_logging_level() -> LoggingLevel:
         """The logging level for events of this type.
 
         Returns:
             LoggingLevel: The logging detail required to log this event.
@@ -54,8 +53,8 @@
     def _get_message(self) -> str:
         """Gets a message representing the details of the event.
 
         Returns:
             str: The message for the event.
         """
 
-        return f"Running script command {self.data['script']}"
+        return f"Scheduling run of {self.data['schema_name']}"
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/event/schedulerun.py` & `AutoTransform-1.1.1a9/src/python/autotransform/event/run.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,46 +3,47 @@
 #
 # Licensed under the MIT License <http://opensource.org/licenses/MIT>
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
-"""The ScheduleRunEvent is triggered whenever an AutoTransformSchema is scheduled to be run
-by the schedule command of the AutoTransform script.
+"""The RunEvent is triggered whenever an AutoTransform script is run and provides
+information on the run.
 """
 
-from typing import TypedDict
+from typing import Dict, TypedDict
 
 from autotransform.event.base import Event
 from autotransform.event.logginglevel import LoggingLevel
 from autotransform.event.type import EventType
 
 
-class ScheduleRunEventData(TypedDict):
-    """The data for a ScheduleRunEvent. Contains the information that will be
+class RunEventData(TypedDict):
+    """The data for a RunEvent. Contains the information that will be
     logged when the event is triggered."""
 
-    schema_name: str
+    args: Dict[str, str]
+    mode: str
 
 
-class ScheduleRunEvent(Event[ScheduleRunEventData]):
-    """A ScheduleRunEvent is triggered whenever an AutoTransformSchema is scheduled to be
-    run by the schedule command and logs the schedule.
+class RunEvent(Event[RunEventData]):
+    """A RunEvent is triggered whenever the AutoTransform script is run. Logs details
+    of the run.
     """
 
     @staticmethod
     def get_type() -> EventType:
         """Used to represent the type of Event, output to logs.
 
         Returns:
             EventType: The unique type associated with this Event.
         """
 
-        return EventType.SCHEDULE_RUN
+        return EventType.RUN
 
     @staticmethod
     def get_logging_level() -> LoggingLevel:
         """The logging level for events of this type.
 
         Returns:
             LoggingLevel: The logging detail required to log this event.
@@ -53,8 +54,8 @@
     def _get_message(self) -> str:
         """Gets a message representing the details of the event.
 
         Returns:
             str: The message for the event.
         """
 
-        return f"Scheduling run of {self.data['schema_name']}"
+        return f"{self.data['mode']}"
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/event/update.py` & `AutoTransform-1.1.1a9/src/python/autotransform/event/update.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/event/verbose.py` & `AutoTransform-1.1.1a9/src/python/autotransform/event/verbose.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/event/warning.py` & `AutoTransform-1.1.1a9/src/python/autotransform/event/warning.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/filter/aggregate.py` & `AutoTransform-1.1.1a9/src/python/autotransform/filter/aggregate.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/filter/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/filter/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 
 class FilterName(str, Enum):
     """A simple enum for mapping."""
 
     AGGREGATE = "aggregate"
     CODEOWNERS = "codeowners"
+    FILE_EXISTS = "file_exists"
     REGEX = "regex"
     REGEX_FILE_CONTENT = "regex_file_content"
     SCRIPT = "script"
 
     # Shard Filters
     KEY_HASH_SHARD = "key_hash_shard"
 
@@ -97,15 +98,14 @@
         Args:
             items (Sequence[Item]): The Items to validate.
         """
 
         if self._valid_keys is None:
             self._valid_keys = self._get_valid_keys(items)
 
-
     def _is_valid(self, item: Item) -> bool:
         """Check whether an Item is valid based on the Filter. Does not handle inversion.
 
         Args:
             item (Item): The Item to check.
 
         Returns:
@@ -119,14 +119,17 @@
     {
         FilterName.AGGREGATE: ComponentImport(
             class_name="AggregateFilter", module="autotransform.filter.aggregate"
         ),
         FilterName.CODEOWNERS: ComponentImport(
             class_name="CodeownersFilter", module="autotransform.filter.codeowners"
         ),
+        FilterName.FILE_EXISTS: ComponentImport(
+            class_name="FileExistsFilter", module="autotransform.filter.file"
+        ),
         FilterName.REGEX: ComponentImport(
             class_name="RegexFilter", module="autotransform.filter.regex"
         ),
         FilterName.REGEX_FILE_CONTENT: ComponentImport(
             class_name="RegexFileContentFilter", module="autotransform.filter.regex"
         ),
         FilterName.SCRIPT: ComponentImport(
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/filter/key_hash_shard.py` & `AutoTransform-1.1.1a9/src/python/autotransform/filter/key_hash_shard.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for the KeyHashShardFilter."""
 
-from __future__ import annotations
-
 from hashlib import md5
 from typing import ClassVar
 
 from autotransform.filter.base import FilterName
 from autotransform.filter.shard import ShardFilter
 from autotransform.item.base import Item
 
@@ -34,8 +32,13 @@
         Args:
             item (Item): The Item to produce a shard number for.
 
         Returns:
             int: The shard number for the Item.
         """
 
-        return int(md5(item.key.encode("UTF-8")).hexdigest(), 16) % self.num_shards
+        # Ensure the key is encoded in UTF-8 before hashing
+        encoded_key = item.key.encode("UTF-8")
+        hashed_key = md5(encoded_key).hexdigest()
+
+        # Convert the hexadecimal hash to an integer and return the shard number
+        return int(hashed_key, 16) % self.num_shards
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/filter/regex.py` & `AutoTransform-1.1.1a9/src/python/autotransform/filter/regex.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for regex based filters, including RegexFilter and FileContentRegexFilter."""
 
-from __future__ import annotations
-
 import re
 from typing import ClassVar
 
 from autotransform.filter.base import Filter, FilterName
 from autotransform.item.base import Item
 from autotransform.item.file import FileItem
 
@@ -25,48 +23,47 @@
 
     Attributes:
         pattern (str): The pattern to use when checking the Item's key.
         name (ClassVar[FilterName]): The name of the component.
     """
 
     pattern: str
-
     name: ClassVar[FilterName] = FilterName.REGEX
 
     def _is_valid(self, item: Item) -> bool:
         """Check whether the key contains the pattern.
 
         Args:
             item (Item): The Item to check.
 
         Returns:
             bool: Returns True if the pattern is found within the key.
         """
 
-        return re.search(self.pattern, item.key) is not None
+        return bool(re.search(self.pattern, item.key))
 
 
 class RegexFileContentFilter(Filter):
     """A Filter which only passes FileItems where the file's content contains a match to the
     provided regex pattern. Uses re.search rather than re.match.
 
     Attributes:
         pattern (str): The pattern to use when checking the FileItem's content
         name (ClassVar[FilterName]): The name of the component.
     """
 
     pattern: str
-
     name: ClassVar[FilterName] = FilterName.REGEX_FILE_CONTENT
 
     def _is_valid(self, item: Item) -> bool:
         """Check whether the contents of the file contains the pattern.
 
         Args:
             item (Item): The Item to check.
 
         Returns:
             bool: Returns True if the pattern is found within the file's content.
         """
 
-        assert isinstance(item, FileItem)
-        return re.search(self.pattern, item.get_content()) is not None
+        if not isinstance(item, FileItem):
+            return False
+        return bool(re.search(self.pattern, item.get_content()))
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/filter/script.py` & `AutoTransform-1.1.1a9/src/python/autotransform/filter/script.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,23 +8,20 @@
 # @black_format
 
 """The implementation for script based Filters."""
 
 from __future__ import annotations
 
 import json
-import subprocess
 from tempfile import NamedTemporaryFile as TmpFile
 from typing import ClassVar, List, Optional, Sequence, Set
 
-from autotransform.event.handler import EventHandler
-from autotransform.event.verbose import VerboseEvent
 from autotransform.filter.base import BulkFilter, FilterName
 from autotransform.item.base import Item
-from autotransform.util.functions import replace_script_args
+from autotransform.util.functions import replace_script_args, run_cmd
 
 
 class ScriptFilter(BulkFilter):
     """A Filter that uses a script to validate Items.
 
     Attributes:
         args (List[str]): The arguments to supply to the script.
@@ -54,16 +51,14 @@
         Args:
             items (Sequence[Item]): The Items to check for valid items.
 
         Returns:
             Set[str]: The keys of the valid Items.
         """
 
-        event_handler = EventHandler.get()
-
         # Get Command
         cmd = [self.script]
         cmd.extend(self.args)
 
         chunk_size = self.chunk_size or len(items)
         item_chunks = [items[i : i + chunk_size] for i in range(0, len(items), chunk_size)]
 
@@ -76,37 +71,17 @@
                     "<<RESULT_FILE>>": [res_file.name],
                     "<<ITEM_FILE>>": [item_file.name],
                 }
                 uses_result_file = "<<RESULT_FILE>>" in cmd
                 replaced_cmd = replace_script_args(cmd, arg_replacements)
 
                 # Run script
-                event_handler.handle(VerboseEvent({"message": f"Running command: {replaced_cmd}"}))
-                proc = subprocess.run(
-                    replaced_cmd,
-                    capture_output=True,
-                    encoding="utf-8",
-                    check=False,
-                    timeout=self.timeout,
-                )
-
-                if proc.stdout.strip() != "" and uses_result_file:
-                    event_handler.handle(
-                        VerboseEvent({"message": f"STDOUT:\n{proc.stdout.strip()}"}),
-                    )
-                elif uses_result_file:
-                    event_handler.handle(VerboseEvent({"message": "No STDOUT"}))
-
-                if proc.stderr.strip() != "":
-                    event_handler.handle(
-                        VerboseEvent({"message": f"STDERR:\n{proc.stderr.strip()}"}),
-                    )
-                else:
-                    event_handler.handle(VerboseEvent({"message": "No STDERR"}))
+                proc = run_cmd(replaced_cmd, self.timeout)
                 proc.check_returncode()
+
                 if uses_result_file:
                     with open(res_file.name, encoding="utf-8") as results:
                         key_data = json.loads(results.read())
                 else:
                     key_data = json.loads(proc.stdout.strip())
                 valid_keys = valid_keys.union(set(key_data))
         return valid_keys
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/filter/shard.py` & `AutoTransform-1.1.1a9/src/python/autotransform/filter/shard.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/input/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/input/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     DIRECTORY = "directory"
     EMPTY = "empty"
     GIT_GREP = "git_grep"
     INLINE = "inline"
     INLINE_FILE = "inline_file"
     INLINE_GENERIC = "inline_generic"
     SCRIPT = "script"
+    TARGET = "target"
 
 
 class Input(NamedComponent):
     """The base for Input components. Used by AutoTransform to get Items that
     represent potentially transformable units for a Schema. Usually returns files but
     any Item can be returned as long as Schema components work with it.
 
@@ -71,11 +72,14 @@
         ),
         InputName.INLINE_GENERIC: ComponentImport(
             class_name="InlineGenericInput", module="autotransform.input.inline"
         ),
         InputName.SCRIPT: ComponentImport(
             class_name="ScriptInput", module="autotransform.input.script"
         ),
+        InputName.TARGET: ComponentImport(
+            class_name="TargetInput", module="autotransform.input.target"
+        ),
     },
     Input,  # type: ignore [type-abstract]
     "input.json",
 )
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/input/directory.py` & `AutoTransform-1.1.1a9/src/python/autotransform/input/directory.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/input/empty.py` & `AutoTransform-1.1.1a9/src/python/autotransform/input/empty.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/input/gitgrep.py` & `AutoTransform-1.1.1a9/src/python/autotransform/input/gitgrep.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/input/inline.py` & `AutoTransform-1.1.1a9/src/python/autotransform/input/inline.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/item/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/item/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/item/file.py` & `AutoTransform-1.1.1a9/src/python/autotransform/item/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,8 +46,15 @@
     def write_content(self, content: str) -> None:
         """Writes new content to the file.
 
         Args:
             content (str): The new content for the File.
         """
 
-        CachedFile(self.get_path()).write_content(content)
+        path = (self.extra_data or {}).get("target_path", self.get_path())
+        CachedFile(path).write_content(content)
+
+    def revert(self) -> None:
+        """Reverts all changes to the file."""
+
+        path = (self.extra_data or {}).get("target_path", self.get_path())
+        CachedFile(path).revert()
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/repo/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/repo/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The base class and associated classes for Repo components."""
 
-from __future__ import annotations
-
 from abc import abstractmethod
 from enum import Enum
 from typing import Any, ClassVar, List, Mapping, Optional, Sequence
 
 from autotransform.batcher.base import Batch
 from autotransform.change.base import Change
 from autotransform.util.component import ComponentFactory, ComponentImport, NamedComponent
@@ -54,15 +52,15 @@
         Args:
             batch (Batch): The Batch that was used for the transformation.
 
         Returns:
             bool: Returns True if there are any changes to the codebase.
         """
 
-        return len(self.get_changed_files(batch)) > 0
+        return bool(self.get_changed_files(batch))
 
     @abstractmethod
     def has_outstanding_change(self, batch: Batch) -> bool:
         """Checks the state of the repo to see whether an outstanding Change
         for the Batch exists.
 
         Args:
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/repo/git.py` & `AutoTransform-1.1.1a9/src/python/autotransform/repo/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for the GitRepo."""
 
-from __future__ import annotations
-
 import re
 import subprocess
 from functools import cached_property
 from typing import Any, ClassVar, List, Mapping, Optional, Sequence
 
 from git import Head
 from git import Repo as GitPython
@@ -49,19 +47,18 @@
         Args:
             status (str): The result of git status -s --untracked-files
 
         Returns:
             List[str]: The changed files.
         """
 
-        if status.strip() == "":
-            return []
         return [
             re.sub(r"^(?:\?\?|M|A|D)", "", line.strip()).strip()
             for line in status.strip().split("\n")
+            if line.strip()
         ]
 
     @staticmethod
     def get_branch_name(title: str) -> str:
         """Gets a unique name for a git branch using the title from the Batch.
 
         Args:
@@ -70,18 +67,19 @@
         Returns:
             str: The name of the branch for this change.
         """
 
         # Handle titles of the format "[1/2] foo" that can come from chunk batching
         fixed_title = re.sub(r"\[(\d+)/(\d+)\]", r"\1_\2", title)
 
-        if autotransform.schema.current is not None:
-            schema_name = f"{autotransform.schema.current.config.schema_name}/"
-        else:
-            schema_name = ""
+        schema_name = (
+            f"{autotransform.schema.current.config.schema_name}/"
+            if autotransform.schema.current
+            else ""
+        )
 
         branch_name = f"{GitRepo.BRANCH_NAME_PREFIX}/{schema_name}{fixed_title}"
         # Replace bad characters
         substring_replacements = {
             "/": "__",
             ":": "-",
             "^": "",
@@ -104,20 +102,20 @@
             title (str): The title of the change.
 
         Returns:
             str: The commit message for this change.
         """
 
         # Add a blank space before prefixes
-        if not title.startswith("["):
-            title = f" {title}"
-        if autotransform.schema.current is not None:
-            schema_name = f"[{autotransform.schema.current.config.schema_name}]"
-        else:
-            schema_name = ""
+        title = f" {title}" if not title.startswith("[") else title
+        schema_name = (
+            f"[{autotransform.schema.current.config.schema_name}]"
+            if autotransform.schema.current
+            else ""
+        )
         return f"{GitRepo.COMMIT_MESSAGE_PREFIX}{schema_name}{title}"
 
     @cached_property
     def _local_repo(self) -> GitPython:
         """Returns a cached instance of the local repo
 
         Returns:
@@ -191,18 +189,15 @@
         """Creates a new branch for all changes, stages them, and commits them.
 
         Args:
             title (str): The title of the Batch being commited.
             update(bool): Whether to update an existing change.
         """
 
-        if update:
-            self._local_repo.git.checkout("-B", GitRepo.get_branch_name(title))
-        else:
-            self._local_repo.git.checkout("-b", GitRepo.get_branch_name(title))
+        self._local_repo.git.checkout("-B" if update else "-b", GitRepo.get_branch_name(title))
         self._local_repo.git.add(all=True)
         self._local_repo.index.commit(GitRepo.get_commit_message(title))
 
     def clean(self, _batch: Batch) -> None:
         """Performs `git reset --hard` to remove any changes.
 
         Args:
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/repo/github.py` & `AutoTransform-1.1.1a9/src/python/autotransform/repo/github.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/runner/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/runner/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/runner/github.py` & `AutoTransform-1.1.1a9/src/python/autotransform/runner/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from __future__ import annotations
 
 import json
 from typing import Any, ClassVar, Dict, Optional
 
 from autotransform.change.base import Change
+from autotransform.config import get_config
 from autotransform.event.debug import DebugEvent
 from autotransform.event.handler import EventHandler
 from autotransform.event.remoterun import RemoteRunEvent
 from autotransform.event.update import RemoteUpdateEvent
 from autotransform.event.verbose import VerboseEvent
 from autotransform.filter.shard import ShardFilter
 from autotransform.repo.github import GithubRepo
@@ -135,27 +136,27 @@
             schema (AutoTransformSchema): The Schema that is involved with the dispatch.
             inputs (Dict[str, Any]): The inputs for the dispatch.
 
         Returns:
             str: The URL for the workflow run.
         """
 
+        repo = get_config().repo_override or schema.repo
+
         if self.repo_name is not None:
             repo_name = self.repo_name
         else:
-            repo = schema.repo
             assert isinstance(
                 repo, GithubRepo
             ), "GithubRunner can only run using schemas that have Github repos"
             repo_name = repo.full_github_name
 
         if self.repo_ref is not None:
             repo_ref = self.repo_ref
         else:
-            repo = schema.repo
             assert isinstance(
                 repo, GithubRepo
             ), "GithubRunner can only run using schemas that have Github repos"
             repo_ref = repo.base_branch
 
         # Allow controlling the target repo with the Runner
         if self.target_repo_name is not None:
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/runner/jenkins.py` & `AutoTransform-1.1.1a9/src/python/autotransform/runner/jenkins.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/schema/__init__.py` & `AutoTransform-1.1.1a9/src/python/autotransform/schema/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 
 # @black_format
 
 """Schemas are the heart of AutoTransform. They contain all necesary components and configuration
 to deploy a change.
 """
 
-# pylint: disable=invalid-name
-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional
 
 if TYPE_CHECKING:
     from autotransform.schema.schema import AutoTransformSchema
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/schema/builder.py` & `AutoTransform-1.1.1a9/src/python/autotransform/schema/builder.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/schema/config.py` & `AutoTransform-1.1.1a9/src/python/autotransform/schema/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,24 @@
 
 """A set of configuration options for a schema."""
 
 from __future__ import annotations
 
 from typing import List, Optional, Type
 
-from pydantic import Field, validator
-
 from autotransform.util.component import ComponentModel
 from autotransform.util.console import (
     choose_option,
     choose_options_from_list,
     choose_yes_or_no,
     get_str,
     input_int,
 )
 from autotransform.validator.base import ValidationResultLevel
+from pydantic import Field, validator
 
 
 class SchemaConfig(ComponentModel):  # pylint: disable=too-few-public-methods
     """An object containing all configuration information for a Schema.
 
     Attributes:
         schema_name (str): The unique name of the schema.
@@ -40,15 +39,14 @@
     """
 
     schema_name: str
     allowed_validation_level: ValidationResultLevel = ValidationResultLevel.NONE
     max_submissions: Optional[int] = None
     owners: List[str] = Field(default_factory=list)
 
-    # pylint: disable=invalid-name
     @validator("max_submissions")
     @classmethod
     def max_submissions_is_positive(cls: Type[SchemaConfig], v: Optional[int]) -> Optional[int]:
         """Validates that max submissions is positive.
 
         Args:
             cls (Type[SchemaConfig]): The Config class.
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/schema/schema.py` & `AutoTransform-1.1.1a9/src/python/autotransform/schema/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,25 +67,24 @@
     config: SchemaConfig
 
     filters: List[Filter] = Field(default_factory=list)
     validators: List[Validator] = Field(default_factory=list)
     commands: List[Command] = Field(default_factory=list)
     repo: Optional[Repo] = None
 
-    def get_batches(self) -> List[Batch]:
-        """Runs the Input to get eligible Items, filters them, then batches them.
+    def get_items(self) -> List[Item]:
+        """Runs the Input to get eligible Items and filters them.
         Note: this function is not thread safe.
 
         Returns:
-            List[Batch]: The Batches for the change
+            List[Item]: The valid Items for the Schema.
         """
 
         autotransform.schema.current = self
         event_handler = EventHandler.get()
-        event_handler.handle(VerboseEvent({"message": "Begin get_batches"}))
 
         # Get Items
         event_handler.handle(VerboseEvent({"message": "Begin get_items"}))
         all_items = self.input.get_items()
         item_str = "\n".join([f"{item!r}," for item in all_items])
         event_handler.handle(VerboseEvent({"message": f"Num Items: {len(all_items)}"}))
         event_handler.handle(DebugEvent({"message": f"Items: [\n{item_str}\n]"}))
@@ -109,17 +108,35 @@
         if valid_items:
             valid_item_str = "\n".join([f"{item!r}," for item in valid_items])
             event_handler.handle(VerboseEvent({"message": f"Num Valid Items: {len(valid_items)}"}))
             event_handler.handle(DebugEvent({"message": f"Valid items: [\n{valid_item_str}\n]"}))
         else:
             event_handler.handle(VerboseEvent({"message": "No valid items."}))
 
+        autotransform.schema.current = None
+        return valid_items
+
+    def get_batches(self, items: List[Item]) -> List[Batch]:
+        """Runs the Input to get eligible Items, filters them, then batches them.
+        Note: this function is not thread safe.
+
+        Args:
+            items (List[Item]): The Items to batch.
+
+        Returns:
+            List[Batch]: The Batches for the change
+        """
+
+        autotransform.schema.current = self
+        event_handler = EventHandler.get()
+        event_handler.handle(VerboseEvent({"message": "Begin get_batches"}))
+
         # Batch Items
         event_handler.handle(VerboseEvent({"message": "Begin batching"}))
-        batches = self.batcher.batch(valid_items)
+        batches = self.batcher.batch(items)
         encodable_batches = [
             {"items": [item.bundle() for item in batch["items"]], "metadata": batch["metadata"]}
             for batch in batches
         ]
         event_handler.handle(VerboseEvent({"message": f"Num Batches: {len(batches)}"}))
         event_handler.handle(DebugEvent({"message": f"Batches: {json.dumps(encodable_batches)}"}))
         autotransform.schema.current = None
@@ -219,15 +236,16 @@
         return submitted
 
     def run(self):
         """Fully run a given Schema including getting and executing all Batches.
         Note: this function is not thread safe."""
 
         autotransform.schema.current = self
-        batches = self.get_batches()
+        items = self.get_items()
+        batches = self.get_batches(items)
         num_submissions = 0
         for batch in batches:
             if (
                 self.config.max_submissions is not None
                 and num_submissions >= self.config.max_submissions
             ):
                 EventHandler.get().handle(
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/initialize.py` & `AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/initialize.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/manage.py` & `AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """The manage command is used to manage outstanding Changes for AutoTransform."""
 
 from argparse import ArgumentParser, Namespace
 
 from autotransform.config import get_repo_config_relative_path
 from autotransform.event.handler import EventHandler
 from autotransform.event.logginglevel import LoggingLevel
-from autotransform.event.run import ScriptRunEvent
+from autotransform.event.run import RunEvent
 from autotransform.event.verbose import VerboseEvent
 from autotransform.util.manager import Manager
 
 
 def add_args(parser: ArgumentParser) -> None:
     """Adds the args to a subparser that are required to manage outstanding changes.
 
@@ -90,11 +90,11 @@
 
     manager_file = args.path
     if manager_file is None:
         manager_file = f"{get_repo_config_relative_path()}/manager.json"
     event_args = {"manager_file": manager_file}
     manager = Manager.read(manager_file)
     event_args["manager"] = manager
-    event_handler.handle(ScriptRunEvent({"script": "manage", "args": event_args}))
+    event_handler.handle(RunEvent({"mode": "manage", "args": event_args}))
 
     event_handler.handle(VerboseEvent({"message": f"Running manager: {manager!r}"}))
     manager.run(args.run_local)
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/run.py` & `AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import os
 from argparse import ArgumentParser, Namespace
 
 from autotransform.config import get_config
 from autotransform.event.debug import DebugEvent
 from autotransform.event.handler import EventHandler
 from autotransform.event.logginglevel import LoggingLevel
-from autotransform.event.run import ScriptRunEvent
+from autotransform.event.run import RunEvent
 from autotransform.event.verbose import VerboseEvent
 from autotransform.filter.base import FACTORY as filter_factory
 from autotransform.runner.base import Runner
 from autotransform.runner.local import LocalRunner
 from autotransform.schema.builder import FACTORY as schema_builder_factory
 from autotransform.schema.schema import AutoTransformSchema
 from autotransform.util.schema_map import SchemaMap
@@ -207,9 +207,9 @@
         event_handler.handle(VerboseEvent({"message": "Running remote"}))
         event_args["remote"] = True
         config_runner = get_config().remote_runner
         assert config_runner is not None
         runner = config_runner
 
     event_args["runner"] = runner
-    event_handler.handle(ScriptRunEvent({"script": "run", "args": event_args}))
+    event_handler.handle(RunEvent({"mode": "run", "args": event_args}))
     runner.run(schema)
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/schedule.py` & `AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/schedule.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import time
 from argparse import ArgumentParser, Namespace
 
 from autotransform.config import get_config, get_repo_config_relative_path
 from autotransform.event.handler import EventHandler
 from autotransform.event.logginglevel import LoggingLevel
-from autotransform.event.run import ScriptRunEvent
+from autotransform.event.run import RunEvent
 from autotransform.event.verbose import VerboseEvent
 from autotransform.runner.local import LocalRunner
 from autotransform.util.scheduler import Scheduler
 
 
 def add_args(parser: ArgumentParser) -> None:
     """Adds the args to a subparser that are required to schedule runs.
@@ -104,15 +104,15 @@
     # Get Scheduler
     schedule_file = args.path
     if schedule_file is None:
         schedule_file = f"{get_repo_config_relative_path()}/scheduler.json"
     event_args = {"scheduler_file": schedule_file}
     scheduler = Scheduler.read(schedule_file)
     event_args["scheduler"] = scheduler
-    event_handler.handle(ScriptRunEvent({"script": "schedule", "args": event_args}))
+    event_handler.handle(RunEvent({"mode": "schedule", "args": event_args}))
 
     event_handler.get().handle(VerboseEvent({"message": f"Running scheduler: {scheduler!r}"}))
     if args.run_local:
         runner = get_config().local_runner
     else:
         runner = get_config().remote_runner
     scheduler.run(start_time, runner or LocalRunner())
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/settings.py` & `AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/settings.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/scripts/commands/update.py` & `AutoTransform-1.1.1a9/src/python/autotransform/scripts/commands/update.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from argparse import ArgumentParser, Namespace
 
 from autotransform.change.base import FACTORY as change_factory
 from autotransform.config import get_config
 from autotransform.event.debug import DebugEvent
 from autotransform.event.handler import EventHandler
 from autotransform.event.logginglevel import LoggingLevel
-from autotransform.event.run import ScriptRunEvent
+from autotransform.event.run import RunEvent
 from autotransform.event.verbose import VerboseEvent
 from autotransform.runner.base import Runner
 from autotransform.runner.local import LocalRunner
 
 
 def add_args(parser: ArgumentParser) -> None:
     """Adds the args to a subparser that are required to update a change.
@@ -152,9 +152,9 @@
         event_handler.handle(VerboseEvent({"message": "Running remote"}))
         event_args["remote"] = True
         config_runner = get_config().remote_runner
         assert config_runner is not None
         runner = config_runner
 
     event_args["runner"] = json.dumps(runner.bundle())
-    event_handler.handle(ScriptRunEvent({"script": "update", "args": event_args}))
+    event_handler.handle(RunEvent({"mode": "update", "args": event_args}))
     runner.update(change)
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/scripts/migrations/p1_0_1.py` & `AutoTransform-1.1.1a9/src/python/autotransform/scripts/migrations/p1_0_1.py`

 * *Files 24% similar despite different names*

```diff
@@ -43,22 +43,19 @@
 
 
 def main():
     """Migrate the Manager for 1.0.0 -> 1.0.1."""
 
     parser = get_arg_parser()
     args = parser.parse_args()
-    file_path = args.path
-    if file_path is None:
-        file_path = f"{get_repo_config_relative_path()}/manager.json"
+    file_path = args.path or f"{get_repo_config_relative_path()}/manager.json"
 
     with open(file_path, "r", encoding="UTF-8") as manager_file:
-        manager_json = manager_file.read()
+        manager_data = json.load(manager_file)
 
-    manager_data = json.loads(manager_json)
     update_manager_data(manager_data)
     manager = Manager.from_data(manager_data)
     manager.write(file_path)
 
 
 def update_manager_data(manager_data: Dict[str, Any]) -> None:
     """Updates the Manager data for the new format.
@@ -76,65 +73,60 @@
 
     Args:
         step_data (Dict[str, Any]): The Step data to update.
     """
 
     if step_data["name"] == "conditional":
         if "actions" not in step_data:
-            step_data["actions"] = [{"name": step_data["action"]}]
-            del step_data["action"]
+            step_data["actions"] = [{"name": step_data.pop("action")}]
         update_condition_data(step_data["condition"])
 
 
 def update_condition_data(condition_data: Dict[str, Any]) -> None:
     """Updates the Condition data to the new format.
 
     Args:
         condition_data (Dict[str, Any]): The Condition data to update.
     """
 
     if condition_data["name"] == ConditionName.AGGREGATE:
         for sub_condition in condition_data["conditions"]:
             update_condition_data(sub_condition)
 
-    if condition_data["name"] == ConditionName.CHANGE_STATE and "value" not in condition_data:
-        condition_data["value"] = condition_data["state"]
-        del condition_data["state"]
-
-    if condition_data["name"] == ConditionName.CREATED_AGO and "value" not in condition_data:
-        condition_data["value"] = condition_data["time"]
-        del condition_data["time"]
-
-    if condition_data["name"] == ConditionName.SCHEMA_NAME and "value" not in condition_data:
-        condition_data["value"] = condition_data["schema_name"]
-        del condition_data["schema_name"]
-
-    if condition_data["name"] == ConditionName.UPDATED_AGO and "value" not in condition_data:
-        condition_data["value"] = condition_data["time"]
-        del condition_data["time"]
+    condition_value_mapping = {
+        ConditionName.CHANGE_STATE: "state",
+        ConditionName.CREATED_AGO: "time",
+        ConditionName.SCHEMA_NAME: "schema_name",
+        ConditionName.UPDATED_AGO: "time",
+    }
+
+    if condition_data["name"] in condition_value_mapping and "value" not in condition_data:
+        condition_data["value"] = condition_data.pop(
+            condition_value_mapping[condition_data["name"]]
+        )
 
     update_comparison(condition_data)
 
 
 def update_comparison(condition_data: Dict[str, Any]) -> None:
     """Updates the comparison value.
 
     Args:
         condition_data (Dict[str, Any]): The Condition data to update
     """
+    comparison_mapping = {
+        "eq": ComparisonType.EQUAL,
+        "neq": ComparisonType.NOT_EQUAL,
+        "gt": ComparisonType.GREATER_THAN,
+        "gte": ComparisonType.GREATER_THAN_OR_EQUAL,
+        "lt": ComparisonType.LESS_THAN,
+        "lte": ComparisonType.LESS_THAN_OR_EQUAL,
+    }
+
     if "comparison" in condition_data:
-        if condition_data["comparison"] == "eq":
-            condition_data["comparison"] = ComparisonType.EQUAL
-        if condition_data["comparison"] == "neq":
-            condition_data["comparison"] = ComparisonType.NOT_EQUAL
-        if condition_data["comparison"] == "gt":
-            condition_data["comparison"] = ComparisonType.GREATER_THAN
-        if condition_data["comparison"] == "gte":
-            condition_data["comparison"] = ComparisonType.GREATER_THAN_OR_EQUAL
-        if condition_data["comparison"] == "lt":
-            condition_data["comparison"] = ComparisonType.LESS_THAN
-        if condition_data["comparison"] == "lte":
-            condition_data["comparison"] = ComparisonType.LESS_THAN_OR_EQUAL
+        condition_data["comparison"] = comparison_mapping.get(
+            condition_data["comparison"], condition_data["comparison"]
+        )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/scripts/migrations/p1_0_3.py` & `AutoTransform-1.1.1a9/src/python/autotransform/scripts/migrations/p1_0_3.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,29 +40,37 @@
         type=str,
         help="A file path to the JSON encoded file, only use if file is in a non-usual place.",
     )
 
     return parser
 
 
+def load_json_file(file_path: str) -> Dict[str, Any]:
+    """Load JSON data from a file.
+
+    Args:
+        file_path (str): The path to the JSON file.
+
+    Returns:
+        Dict[str, Any]: The loaded JSON data.
+    """
+    with open(file_path, "r", encoding="UTF-8") as json_file:
+        return json.loads(json_file.read())
+
+
 def main() -> None:
     """Migrate Scheduler and Schema map for 1.0.2 -> 1.0.3."""
 
     parser = get_arg_parser()
     args = parser.parse_args()
 
     # Get existing Scheduler data
-    file_path = args.path
-    if file_path is None:
-        file_path = f"{get_repo_config_relative_path()}/scheduler.json"
-
-    with open(file_path, "r", encoding="UTF-8") as scheduler_file:
-        scheduler_json = scheduler_file.read()
+    file_path = args.path or f"{get_repo_config_relative_path()}/scheduler.json"
 
-    scheduler_data = json.loads(scheduler_json)
+    scheduler_data = load_json_file(file_path)
 
     schema_map = SchemaMap.get()
     update_scheduler_data(scheduler_data, schema_map)
 
     scheduler = Scheduler.from_data(scheduler_data)
     scheduler.write(file_path)
     schema_map.write()
@@ -83,16 +91,15 @@
         if schema_type is None:
             continue
         schema_type = SchemaType(schema_type)
         schema_target = schema_data["target"]
         if schema_type == SchemaType.BUILDER:
             schema = schema_builder_factory.get_instance({"name": schema_target}).build()
         else:
-            with open(schema_target, "r", encoding="UTF-8") as schema_file:
-                schema = AutoTransformSchema.from_data(json.loads(schema_file.read()))
+            schema = AutoTransformSchema.from_data(load_json_file(schema_target))
         schema_name = schema.config.schema_name
         del schema_data["target"]
         del schema_data["type"]
         schema_data["schema_name"] = schema_name
         if schema_name not in schema_map:
             schema_map.add_schema(schema_name, schema_type, schema_target)
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/scripts/migrations/p1_0_5.py` & `AutoTransform-1.1.1a9/src/python/autotransform/scripts/migrations/p1_0_5.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # @black_format
 
 """A script to perform a migration of a Manager JSON file from 1.0.3 to 1.0.5."""
 
 import json
 from argparse import ArgumentParser
-from typing import Any, Dict, List
+from typing import Any, Dict
 
 from autotransform.config import get_repo_config_relative_path
 from autotransform.step.condition.base import ConditionName
 from autotransform.util.manager import Manager
 
 
 def get_arg_parser() -> ArgumentParser:
@@ -42,65 +42,62 @@
 
 
 def main():
     """Migrate the Manager for 1.0.3 -> 1.0.5."""
 
     parser = get_arg_parser()
     args = parser.parse_args()
-    file_path = args.path
-    if file_path is None:
-        file_path = f"{get_repo_config_relative_path()}/manager.json"
+    file_path = args.path or f"{get_repo_config_relative_path()}/manager.json"
 
     with open(file_path, "r", encoding="UTF-8") as manager_file:
-        manager_json = manager_file.read()
+        manager_data = json.load(manager_file)
 
-    manager_data = json.loads(manager_json)
     update_manager_data(manager_data)
     manager = Manager.from_data(manager_data)
     manager.write(file_path)
 
 
 def update_manager_data(manager_data: Dict[str, Any]) -> None:
     """Updates the Manager data for the new format.
 
     Args:
         manager_data (Dict[str, Any]): The Manager data to update
     """
 
-    for step in manager_data["steps"]:
+    for step in manager_data.get("steps", []):
         update_step_data(step)
 
 
 def update_step_data(step_data: Dict[str, Any]) -> None:
     """Updates the Step data to the new format.
 
     Args:
         step_data (Dict[str, Any]): The Step data to update.
     """
 
-    if step_data["name"] == "conditional":
-        update_condition_data(step_data["condition"])
+    if step_data.get("name") == "conditional":
+        update_condition_data(step_data.get("condition", {}))
 
 
 def update_condition_data(condition_data: Dict[str, Any]) -> None:
     """Updates the Condition data to the new format.
 
     Args:
         condition_data (Dict[str, Any]): The Condition data to update.
     """
 
-    if condition_data["name"] != ConditionName.CHANGE_STATE:
+    if condition_data.get("name") != ConditionName.CHANGE_STATE:
         return
 
-    if isinstance(condition_data["value"], str) and condition_data["value"] in [
+    if isinstance(condition_data.get("value"), str) and condition_data["value"] in [
         "approved",
         "changes_requested",
     ]:
         condition_data["name"] = ConditionName.REVIEW_STATE
         return
 
-    if isinstance(condition_data["value"], List):
+    if isinstance(condition_data.get("value"), list):
         print("Can not migrate in/not_in comparisons for conditions")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/action/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/action/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/action/comments.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/action/comments.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,33 +7,31 @@
 
 # @black_format
 
 """All Actions associated with a Change's comments."""
 
 from typing import ClassVar
 
-from pydantic import validator
-
 from autotransform.change.base import Change
 from autotransform.step.action.base import Action, ActionName
+from pydantic import validator
 
 
 class CommentAction(Action):
     """Adds a comment to an existing Change.
 
     Attributes:
         body(str): The body of the comment.
         name (ClassVar[ActionName]): The name of the component.
     """
 
     body: str
 
     name: ClassVar[ActionName] = ActionName.COMMENT
 
-    # pylint: disable=invalid-name
     @validator("body")
     @classmethod
     def body_must_be_non_empty(cls, v: str) -> str:
         """Validates the body is not empty.
 
         Args:
             v (str): The body of the comment.
@@ -41,15 +39,15 @@
         Raises:
             ValueError: Raises an error when the body is empty.
 
         Returns:
             str: The unmodified body of the comment.
         """
 
-        if v == "":
+        if not v.strip():
             raise ValueError("Comment body must be non-empty")
         return v
 
     def run(self, change: Change) -> bool:
         """Adds a comment to the specified Change.
 
         Args:
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/action/labels.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/action/labels.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,33 +7,31 @@
 
 # @black_format
 
 """All Actions associated with a Change's labels."""
 
 from typing import ClassVar, List
 
-from pydantic import validator
-
 from autotransform.change.base import Change
 from autotransform.step.action.base import Action, ActionName
+from pydantic import validator
 
 
 class AddLabelsAction(Action):
     """Adds labels to an existing Change.
 
     Attributes:
         labels(List[str]): The list of labels to add.
         name (ClassVar[ActionName]): The name of the component.
     """
 
     labels: List[str]
 
     name: ClassVar[ActionName] = ActionName.ADD_LABELS
 
-    # pylint: disable=invalid-name
     @validator("labels")
     @classmethod
     def labels_must_be_non_empty(cls, v: List[str]) -> List[str]:
         """Validates the labels are not empty.
 
         Args:
             v (List[str]): The labels to add to the Change.
@@ -43,15 +41,15 @@
 
         Returns:
             List[str]: The unmodified labels to add.
         """
 
         if not v:
             raise ValueError("At least 1 label must be provided")
-        if any(label == "" for label in v):
+        if any(not label for label in v):
             raise ValueError("Labels must be non-empty strings")
         return v
 
     def run(self, change: Change) -> bool:
         """Adds labels to the specified Change.
 
         Args:
@@ -72,15 +70,14 @@
         name (ClassVar[ActionName]): The name of the component.
     """
 
     label: str
 
     name: ClassVar[ActionName] = ActionName.REMOVE_LABEL
 
-    # pylint: disable=invalid-name
     @validator("label")
     @classmethod
     def label_must_be_non_empty(cls, v: str) -> str:
         """Validates the label is not empty.
 
         Args:
             v (str): The label to remove.
@@ -88,15 +85,15 @@
         Raises:
             ValueError: Raises an error when the label is empty.
 
         Returns:
             str: The unmodified label of the comment.
         """
 
-        if v == "":
+        if not v:
             raise ValueError("Label to remove must be non-empty")
         return v
 
     def run(self, change: Change) -> bool:
         """Removes labels from the specified Change.
 
         Args:
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/action/request.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/action/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,25 +55,23 @@
         return RequestHandler(
             url=self.url,
             data=self.data,
             headers=self.headers,
             params=self.params,
             log_response=self.log_response,
             post=self.post,
-            constant_replacers={"env": lambda var: str(os.getenv(var) or "")},
+            constant_replacers={"env": lambda var: os.getenv(var, "")},
         )
 
     def run(self, change: Change) -> bool:
         """Performs a REST API request for a Change.
 
         Args:
             change (Change): The Change to perform the request on.
 
         Returns:
             bool: Whether the request returned a non-error response.
         """
 
-        response = self._handler.get_response(
-            {"change": lambda name: str(getattr(change, name) or "")}
-        )
+        response = self._handler.get_response({"change": lambda name: getattr(change, name, "")})
 
         return response.ok
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/action/reviewers.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/action/reviewers.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 
 # @black_format
 
 """All Actions associated with a Change's reviewers."""
 
 from typing import Any, ClassVar, Dict, List
 
-from pydantic import Field, root_validator, validator
-
 from autotransform.change.base import Change
 from autotransform.step.action.base import Action, ActionName
+from pydantic import Field, root_validator, validator
 
 
 class AddReviewersAction(Action):
     """Adds reviewers to an existing Change.
 
     Attributes:
         reviewers(optional, List[str]): The list of reviewers to add. Defaults to [].
@@ -27,18 +26,17 @@
     """
 
     reviewers: List[str] = Field(default_factory=list)
     team_reviewers: List[str] = Field(default_factory=list)
 
     name: ClassVar[ActionName] = ActionName.ADD_REVIEWERS
 
-    # pylint: disable=invalid-name
     @validator("reviewers")
     @classmethod
-    def labels_must_be_non_empty(cls, v: List[str]) -> List[str]:
+    def reviewers_must_be_non_empty(cls, v: List[str]) -> List[str]:
         """Validates the reviewers are not empty strings.
 
         Args:
             v (List[str]): The reviewers to add to the Change.
 
         Raises:
             ValueError: Raises an error if a reviewer is an empty string.
@@ -47,15 +45,14 @@
             List[str]: The unmodified reviewers to add.
         """
 
         if any(reviewer == "" for reviewer in v):
             raise ValueError("Reviewers must be non-empty strings")
         return v
 
-    # pylint: disable=invalid-name
     @validator("team_reviewers")
     @classmethod
     def team_reviewers_must_be_non_empty(cls, v: List[str]) -> List[str]:
         """Validates the team reviewers are not empty strings.
 
         Args:
             v (List[str]): The team reviewers to add to the Change.
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/action/source.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/action/source.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/condition/aggregate.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/condition/aggregate.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for the AggregateCondition."""
 
-from __future__ import annotations
-
 from typing import Any, ClassVar, Dict, List, Type
 
 from autotransform.change.base import Change
 from autotransform.step.condition.base import FACTORY as condition_factory
 from autotransform.step.condition.base import Condition, ConditionName
 from autotransform.util.enums import AggregatorType
 
@@ -40,33 +38,28 @@
         Args:
             change (Change): The Change the Condition is checking.
 
         Returns:
             bool: Whether the Change passes the Condition.
         """
 
-        if self.aggregator == AggregatorType.ALL:
-            return all(condition.check(change) for condition in self.conditions)
-
-        if self.aggregator == AggregatorType.ANY:
-            return any(condition.check(change) for condition in self.conditions)
-
-        raise ValueError(f"Unknown aggregator type {self.aggregator}")
+        aggregator_check = all if self.aggregator == AggregatorType.ALL else any
+        return aggregator_check(condition.check(change) for condition in self.conditions)
 
     @classmethod
-    def from_data(cls: Type[AggregateCondition], data: Dict[str, Any]) -> AggregateCondition:
+    def from_data(cls: Type["AggregateCondition"], data: Dict[str, Any]) -> "AggregateCondition":
         """Produces an instance of the component from decoded data.
 
         Args:
             data (Dict[str, Any]): The JSON decoded data.
 
         Returns:
             AggregateCondition: An instance of the component.
         """
 
         aggregator = (
-            data["aggregator"]
-            if isinstance(data["aggregator"], AggregatorType)
-            else AggregatorType(data["aggregator"])
+            AggregatorType(data["aggregator"])
+            if isinstance(data["aggregator"], str)
+            else data["aggregator"]
         )
         conditions = [condition_factory.get_instance(condition) for condition in data["conditions"]]
         return cls(aggregator=aggregator, conditions=conditions)
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/condition/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/condition/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Any, ClassVar, Dict, Generic, List, Optional, Set, Type, TypeVar
 
-from pydantic import root_validator, validator
-
 from autotransform.change.base import Change
 from autotransform.step.condition.comparison import ComparisonType, compare
 from autotransform.util.component import ComponentFactory, ComponentImport, NamedComponent
+from pydantic import root_validator, validator
 
 
 class ConditionName(str, Enum):
     """A simple enum for mapping."""
 
     AGGREGATE = "aggregate"
     CHANGE_STATE = "change_state"
@@ -145,15 +144,14 @@
         if comparison not in [ComparisonType.IN, ComparisonType.NOT_IN] and isinstance(
             values["value"], List
         ):
             raise ValueError(f"Can not perform comparison {comparison} when value is a list.")
 
         return values
 
-    # pylint: disable=invalid-name
     @validator("comparison")
     @classmethod
     def comparison_type_is_valid(
         cls: Type[ComparisonCondition], v: ComparisonType
     ) -> ComparisonType:
         """Validates the condition can perform the specified comparison.
 
@@ -286,15 +284,14 @@
         return {
             ComparisonType.CONTAINS,
             ComparisonType.NOT_CONTAINS,
             ComparisonType.EMPTY,
             ComparisonType.NOT_EMPTY,
         }
 
-    # pylint: disable=invalid-name
     @validator("comparison")
     @classmethod
     def comparison_type_is_valid(
         cls: Type[ListComparisonCondition], v: ComparisonType
     ) -> ComparisonType:
         """Validates the condition can perform the specified comparison.
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/condition/comparison.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/condition/comparison.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/condition/created.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/condition/created.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,36 +5,34 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for the CreatedAgoCondition."""
 
-from __future__ import annotations
+from typing import ClassVar, List, Union
 
 import time
-from typing import ClassVar, List
-
 from autotransform.change.base import Change
 from autotransform.step.condition.base import ConditionName, SortableComparisonCondition
 from autotransform.step.condition.comparison import ComparisonType
 
 
 class CreatedAgoCondition(SortableComparisonCondition[int]):
     """A condition which checks how long ago a Change was created against the supplied time, all
     in seconds, using the supplied comparison.
 
     Attributes:
         comparison (ComparisonType): The type of comparison to perform.
-        value (int | List[int]): The number of seconds to compare against.
+        value (Union[int, List[int]]): The number of seconds to compare against.
         name (ClassVar[ConditionName]): The name of the Component.
     """
 
     comparison: ComparisonType
-    value: int | List[int]
+    value: Union[int, List[int]]
 
     name: ClassVar[ConditionName] = ConditionName.CREATED_AGO
 
     def get_val_from_change(self, change: Change) -> int:
         """Gets how long ago the Change was created.
 
         Args:
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/condition/labels.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/condition/labels.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for Conditions based on labels."""
 
-from __future__ import annotations
-
 from typing import ClassVar, List, Optional
 
 from autotransform.change.base import Change
 from autotransform.step.condition.base import ConditionName, ListComparisonCondition
 from autotransform.step.condition.comparison import ComparisonType
 
 
 class LabelsCondition(ListComparisonCondition[str]):
     """A condition which checks the labels for a Change.
 
     Attributes:
         comparison (ComparisonType): The type of comparison to perform.
-        value (optional, Optional[str]): The label to check for. Defaults to None.
+        value (Optional[str], optional): The label to check for. Defaults to None.
         name (ClassVar[ConditionName]): The name of the Component.
     """
 
     comparison: ComparisonType
     value: Optional[str] = None
 
     name: ClassVar[ConditionName] = ConditionName.LABELS
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/condition/request.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/condition/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,32 +68,30 @@
         return RequestHandler(
             url=self.url,
             data=self.data,
             headers=self.headers,
             params=self.params,
             log_response=self.log_response,
             post=self.post,
-            constant_replacers={"env": lambda var: str(os.getenv(var) or "")},
+            constant_replacers={"env": lambda var: os.getenv(var, "")},
         )
 
     def get_val_from_change(self, change: Change) -> str:
         """Gets the existing value to compare against from the Change.
 
         Args:
             change (Change): The Change the Condition is checking.
 
         Returns:
             str: The value from the Change to compare against.
         """
 
-        response = self._handler.get_response(
-            ({"change": lambda name: str(getattr(change, name) or "")})
-        )
+        response = self._handler.get_response(({"change": lambda name: getattr(change, name, "")}))
 
         if not self.response_field:
             return response.text
 
         result = response.json()
         for field_name in self.response_field.split("//"):
-            result = result[field_name]
+            result = result.get(field_name)
 
         return str(result)
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/condition/reviewers.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/condition/reviewers.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for Conditions based on reviewers."""
 
-from __future__ import annotations
-
 from typing import ClassVar, List, Optional
 
 from autotransform.change.base import Change
 from autotransform.step.condition.base import ConditionName, ListComparisonCondition
 from autotransform.step.condition.comparison import ComparisonType
 
 
@@ -25,48 +23,44 @@
         comparison (ComparisonType): The type of comparison to perform.
         value (optional, Optional[str]): The reviewer to check for. Defaults to None.
         name (ClassVar[ConditionName]): The name of the Component.
     """
 
     comparison: ComparisonType
     value: Optional[str] = None
-
     name: ClassVar[ConditionName] = ConditionName.REVIEWERS
 
     def get_val_from_change(self, change: Change) -> List[str]:
         """Gets the reviewers from the Change.
 
         Args:
             change (Change): The Change the Condition is checking.
 
         Returns:
             List[str]: The reviewers of the Change.
         """
-
         return change.get_reviewers()
 
 
 class TeamReviewersCondition(ListComparisonCondition[str]):
     """A condition which checks the team reviewers for a Change.
 
     Attributes:
         comparison (ComparisonType): The type of comparison to perform.
         value (optional, Optional[str]): The team reviewer to check for. Defaults to None.
         name (ClassVar[ConditionName]): The name of the Component.
     """
 
     comparison: ComparisonType
     value: Optional[str] = None
-
     name: ClassVar[ConditionName] = ConditionName.TEAM_REVIEWERS
 
     def get_val_from_change(self, change: Change) -> List[str]:
         """Gets the team reviewers from the Change.
 
         Args:
             change (Change): The Change the Condition is checking.
 
         Returns:
             List[str]: The team reviewers of the Change.
         """
-
         return change.get_team_reviewers()
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/condition/schema.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/condition/schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,35 +5,33 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for the SchemaNameCondition."""
 
-from __future__ import annotations
-
-from typing import ClassVar, List
+from typing import ClassVar, List, Union
 
 from autotransform.change.base import Change
 from autotransform.step.condition.base import ComparisonCondition, ConditionName
 from autotransform.step.condition.comparison import ComparisonType
 
 
 class SchemaNameCondition(ComparisonCondition[str]):
     """A condition which checks the name of the Schema that produced a change against the supplied
     name, using the supplied comparison.
 
     Attributes:
         comparison (ComparisonType): The type of comparison to perform.
-        value (str | List[str]): The schema name(s) to compare against.
+        value (Union[str, List[str]]): The schema name(s) to compare against.
         name (ClassVar[ConditionName]): The name of the Component.
     """
 
     comparison: ComparisonType
-    value: str | List[str]
+    value: Union[str, List[str]]
 
     name: ClassVar[ConditionName] = ConditionName.SCHEMA_NAME
 
     def get_val_from_change(self, change: Change) -> str:
         """Gets the Schema name from the Change.
 
         Args:
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/condition/state.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/condition/state.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,33 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for the ChangeStateCondition."""
 
-from __future__ import annotations
-
-from typing import ClassVar, List
+from typing import ClassVar, List, Union
 
 from autotransform.change.base import Change, ChangeState, ReviewState, TestState
 from autotransform.step.condition.base import ComparisonCondition, ConditionName
 from autotransform.step.condition.comparison import ComparisonType
 
 
 class ChangeStateCondition(ComparisonCondition[ChangeState]):
     """A condition which checks the ChangeState against the state supplied using the supplied
     comparison.
 
     Attributes:
         comparison (ComparisonType): The type of comparison to perform.
-        value (ChangeState | List[ChangeState]): The state(s) to compare against.
+        value (Union[ChangeState, List[ChangeState]]): The state(s) to compare against.
         name (ClassVar[ConditionName]): The name of the Component.
     """
 
     comparison: ComparisonType
-    value: ChangeState | List[ChangeState]
+    value: Union[ChangeState, List[ChangeState]]
 
     name: ClassVar[ConditionName] = ConditionName.CHANGE_STATE
 
     def get_val_from_change(self, change: Change) -> ChangeState:
         """Gets the state from the Change.
 
         Args:
@@ -48,20 +46,20 @@
 
 class MergeableStateCondition(ComparisonCondition[str]):
     """A condition which checks the mergeable state against the state supplied using the supplied
     comparison.
 
     Attributes:
         comparison (ComparisonType): The type of comparison to perform.
-        value (str | List[str]): The state(s) to compare against.
+        value (Union[str, List[str]]): The state(s) to compare against.
         name (ClassVar[ConditionName]): The name of the Component.
     """
 
     comparison: ComparisonType
-    value: str | List[str]
+    value: Union[str, List[str]]
 
     name: ClassVar[ConditionName] = ConditionName.MERGEABLE_STATE
 
     def get_val_from_change(self, change: Change) -> str:
         """Gets the mergeable state from the Change.
 
         Args:
@@ -76,20 +74,20 @@
 
 class ReviewStateCondition(ComparisonCondition[ReviewState]):
     """A condition which checks the ReviewState against the state supplied using the supplied
     comparison.
 
     Attributes:
         comparison (ComparisonType): The type of comparison to perform.
-        value (ReviewState | List[ReviewState]): The state(s) to compare against.
+        value (Union[ReviewState, List[ReviewState]]): The state(s) to compare against.
         name (ClassVar[ConditionName]): The name of the Component.
     """
 
     comparison: ComparisonType
-    value: ReviewState | List[ReviewState]
+    value: Union[ReviewState, List[ReviewState]]
 
     name: ClassVar[ConditionName] = ConditionName.REVIEW_STATE
 
     def get_val_from_change(self, change: Change) -> ReviewState:
         """Gets the review state from the Change.
 
         Args:
@@ -104,20 +102,20 @@
 
 class TestStateCondition(ComparisonCondition[TestState]):
     """A condition which checks the TestState against the state supplied using the supplied
     comparison.
 
     Attributes:
         comparison (ComparisonType): The type of comparison to perform.
-        value (TestState | List[TestState]): The state(s) to compare against.
+        value (Union[TestState, List[TestState]]): The state(s) to compare against.
         name (ClassVar[ConditionName]): The name of the Component.
     """
 
     comparison: ComparisonType
-    value: TestState | List[TestState]
+    value: Union[TestState, List[TestState]]
 
     name: ClassVar[ConditionName] = ConditionName.TEST_STATE
 
     def get_val_from_change(self, change: Change) -> TestState:
         """Gets the state from the Change.
 
         Args:
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/condition/updated.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/condition/updated.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,43 +5,41 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for all conditions handling when a Change was updated."""
 
-from __future__ import annotations
-
-import time
-from typing import ClassVar, List
+from typing import ClassVar, List, Union
 
 from autotransform.change.base import Change
 from autotransform.step.condition.base import ConditionName, SortableComparisonCondition
 from autotransform.step.condition.comparison import ComparisonType
+from time import time as current_time
 
 
 class UpdatedAgoCondition(SortableComparisonCondition[int]):
     """A condition which checks how long ago a Change was updated against the supplied time, all
     in seconds, using the supplied comparison.
 
     Attributes:
         comparison (ComparisonType): The type of comparison to perform.
-        value (int | List[int]): The number of seconds to compare against.
+        value (Union[int, List[int]]): The number of seconds to compare against.
         name (ClassVar[ConditionName]): The name of the Component.
     """
 
     comparison: ComparisonType
-    value: int | List[int]
+    value: Union[int, List[int]]
 
     name: ClassVar[ConditionName] = ConditionName.UPDATED_AGO
 
     def get_val_from_change(self, change: Change) -> int:
         """Gets how long ago the Change was updated.
 
         Args:
             change (Change): The Change the Condition is checking.
 
         Returns:
             int: How long ago the Change was updated.
         """
 
-        return int(time.time() - change.get_last_updated_timestamp())
+        return int(current_time() - change.get_last_updated_timestamp())
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/step/conditional.py` & `AutoTransform-1.1.1a9/src/python/autotransform/step/conditional.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/transformer/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/transformer/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 TResult = TypeVar("TResult", bound=Optional[Mapping[str, Any]])
 
 
 class TransformerName(str, Enum):
     """A simple enum for mapping."""
 
+    AI_MODEL = "ai_model"
     JSCODESHIFT = "jscodeshift"
     LIBCST = "libcst"
-    OPEN_AI = "open_ai"
     REGEX = "regex"
     SCRIPT = "script"
 
 
 class Transformer(Generic[TResult], NamedComponent):
     """The base for Transformer components. Transformers are used to execute changes to a codebase.
     A Transformer takes in a Batch and then executes all changes associated with the Batch.
@@ -50,23 +50,23 @@
         Args:
             batch (Batch): The Batch that will be transformed.
         """
 
 
 FACTORY = ComponentFactory(
     {
+        TransformerName.AI_MODEL: ComponentImport(
+            class_name="AIModelTransformer", module="autotransform.transformer.aimodel"
+        ),
         TransformerName.JSCODESHIFT: ComponentImport(
             class_name="JSCodeshiftTransformer", module="autotransform.transformer.jscodeshift"
         ),
         TransformerName.LIBCST: ComponentImport(
             class_name="LibCSTTransformer", module="autotransform.transformer.libcst"
         ),
-        TransformerName.OPEN_AI: ComponentImport(
-            class_name="OpenAITransformer", module="autotransform.transformer.openai"
-        ),
         TransformerName.REGEX: ComponentImport(
             class_name="RegexTransformer", module="autotransform.transformer.regex"
         ),
         TransformerName.SCRIPT: ComponentImport(
             class_name="ScriptTransformer", module="autotransform.transformer.script"
         ),
     },
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/transformer/jscodeshift.py` & `AutoTransform-1.1.1a9/src/python/autotransform/transformer/jscodeshift.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,69 +5,68 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for the JSCodeshiftTransformer. See https://github.com/facebook/jscodeshift"""
 
-from __future__ import annotations
+from typing import ClassVar, List
 
 import subprocess
-from typing import ClassVar, List
+from pydantic import Field
 
 from autotransform.event.handler import EventHandler
 from autotransform.event.verbose import VerboseEvent
 from autotransform.item.base import Item
 from autotransform.item.file import FileItem
 from autotransform.transformer.base import TransformerName
 from autotransform.transformer.single import SingleTransformer
-from pydantic import Field
 
 
 class JSCodeshiftTransformer(SingleTransformer):
     """A Transformer that makes changes using JSCodeshift.
 
     Attributes:
         js_transform (str): The JSCodeshift transform to execute.
         args (optional, List[str]): The arguments to supply to the transformation. Defaults to [].
         timeout (optional, int): The timeout for an individual run.
         name (ClassVar[TransformerName]): The name of the component.
     """
 
     js_transform: str
-
     args: List[str] = Field(default_factory=list)
     timeout: int = 600
-
     name: ClassVar[TransformerName] = TransformerName.JSCODESHIFT
 
     def _transform_item(self, item: Item) -> None:
         """Run the supplied JSCodeshift transform against the file.
 
         Args:
             item (Item): The file that will be transformed.
         """
 
         assert isinstance(item, FileItem)
         event_handler = EventHandler.get()
 
-        cmd = ["jscodeshift", "-t", self.js_transform, item.get_path()]
-        cmd.extend(self.args)
+        cmd = ["jscodeshift", "-t", self.js_transform, item.get_path(), *self.args]
 
         # Run JSCodeshift
         event_handler.handle(VerboseEvent({"message": f"Running command: {cmd}"}))
         proc = subprocess.run(
             cmd,
             capture_output=True,
             encoding="utf-8",
             check=False,
             timeout=self.timeout,
         )
-        if proc.stdout.strip() != "":
-            event_handler.handle(VerboseEvent({"message": f"STDOUT:\n{proc.stdout.strip()}"}))
-        else:
-            event_handler.handle(VerboseEvent({"message": "No STDOUT"}))
-        if proc.stderr.strip() != "":
-            event_handler.handle(VerboseEvent({"message": f"STDERR:\n{proc.stderr.strip()}"}))
-        else:
-            event_handler.handle(VerboseEvent({"message": "No STDERR"}))
+
+        stdout = proc.stdout.strip()
+        stderr = proc.stderr.strip()
+
+        event_handler.handle(
+            VerboseEvent({"message": f"STDOUT:\n{stdout}" if stdout else "No STDOUT"})
+        )
+        event_handler.handle(
+            VerboseEvent({"message": f"STDERR:\n{stderr}" if stderr else "No STDERR"})
+        )
+
         proc.check_returncode()
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/transformer/libcst.py` & `AutoTransform-1.1.1a9/src/python/autotransform/transformer/libcst.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,57 +42,67 @@
         command_name (str): The name of the class for the CodemodCommand.
         command_args (optional, Dict[str, Any]): Arguments for the CodemodCommand. Defaults to {}.
         name (ClassVar[TransformerName]): The name of the component.
     """
 
     command_module: str
     command_name: str
-
     command_args: Dict[str, Any] = Field(default_factory=dict)
-
     name: ClassVar[TransformerName] = TransformerName.LIBCST
 
     def _transform_item(self, item: Item) -> None:
         """Run the supplied CodemodCommand against a FileItem.
 
         Args:
             item (Item): The file that will be transformed.
         """
 
-        assert isinstance(item, FileItem)
+        if not isinstance(item, FileItem):
+            raise TypeError("Item must be an instance of FileItem")
+
         event_handler = EventHandler.get()
         event_handler.handle(DebugEvent({"message": f"Performing transform on {item.get_path()}"}))
         res = transform_module(self._command, item.get_content())
+
         for message in res.warning_messages:
             event_handler.handle(WarningEvent({"message": f"Warning: {message}"}))
+
         if isinstance(res, TransformSuccess):
             event_handler.handle(DebugEvent({"message": "Transform success"}))
             item.write_content(res.code)
-        if isinstance(res, TransformSkip):
+        elif isinstance(res, TransformSkip):
             event_handler.handle(
                 DebugEvent(
                     {"message": f"Transform skipped ({res.skip_reason}): {res.skip_description}"}
                 )
             )
-        if isinstance(res, TransformFailure):
+        elif isinstance(res, TransformFailure):
             event_handler.handle(
                 WarningEvent({"message": f"Transform failed: {res.error}\n{res.traceback_str}"})
             )
-        if isinstance(res, TransformExit):
+        elif isinstance(res, TransformExit):
             event_handler.handle(DebugEvent({"message": "Transform exited from user interupt"}))
 
     @cached_property
     def _command(self) -> CodemodCommand:
         """Gets an instance of the command and caches it.
 
         Returns:
             CodemodCommand: An instance of the command to run.
         """
 
         module = importlib.import_module(self.command_module)
-        assert hasattr(module, self.command_name)
+
+        if not hasattr(module, self.command_name):
+            raise AttributeError(
+                f"Module {self.command_module} does not have attribute {self.command_name}"
+            )
+
         command_class = getattr(module, self.command_name)
-        assert isinstance(command_class, type), "Command is not a class"
-        assert issubclass(
-            command_class, CodemodCommand
-        ), "Component must be a subclass of CodemodCommand"
+
+        if not isinstance(command_class, type):
+            raise TypeError("Command is not a class")
+
+        if not issubclass(command_class, CodemodCommand):
+            raise TypeError("Component must be a subclass of CodemodCommand")
+
         return command_class(CodemodContext(), **self.command_args)
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/transformer/openai.py` & `AutoTransform-1.1.1a9/src/python/autotransform/model/openai.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,113 +3,74 @@
 #
 # Licensed under the MIT License <http://opensource.org/licenses/MIT>
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
-"""The implementation for the OpenAITransformer."""
+"""The implementation for the OpenAIModel."""
 
-from __future__ import annotations
-
-from time import sleep
-from typing import Any, ClassVar, Dict, List, Optional, Type
+from copy import deepcopy
+from typing import ClassVar, Dict, List, Optional, Sequence, Tuple
 
 import openai  # pylint: disable=import-error
-from autotransform.batcher.base import Batch
-from autotransform.command.base import FACTORY as command_factory
-from autotransform.command.base import Command
 from autotransform.config import get_config
 from autotransform.event.handler import EventHandler
-from autotransform.event.verbose import VerboseEvent
-from autotransform.item.base import Item
+from autotransform.event.model import AIModelCompletionEvent
 from autotransform.item.file import FileItem
-from autotransform.transformer.base import TransformerName
-from autotransform.transformer.single import SingleTransformer
-from autotransform.validator.base import FACTORY as validator_factory
-from autotransform.validator.base import ValidationResultLevel, Validator
-from pydantic import Field, validator
+from autotransform.model.base import Model, ModelName
+from autotransform.validator.base import ValidationResult
+from pydantic import validator  # pylint: disable=import-error
 
 
-class OpenAITransformer(SingleTransformer):
-    """A transformer which uses OpenAI models to perform a completion to generate code.
+class OpenAIModel(Model[List[Dict[str, str]]]):
+    """The base for Model components. Used by AutoTransform to interact with AI models
+    such as LLMs.
 
     Attributes:
-        prompt (str): The prompt to use for completition. Uses sentry values to replace
-            values in the prompt.
-            <<FILE_PATH>> - Replaced with the path of the file being transformed.
-            <<FILE_CONTENT>> - Replaced with the content of the file being transformed.
-        commands (optional, List[Command]): A set of commands to use on transformed files
-            before validation. Useful for correcting things like formatting. Defaults to an
-            empty list.
-        max_completion_attempts (optional, int): The maximum number of times to try the OpenAI
-            API. Defaults to 3.
-        max_validation_attempts (optional, int): The maximum number of times to validate
-            completitions. Defaults to 3.
-        model (optional, str): The model to use for completition. Defaults to gpt-3.5-turbo.
+        prompts (List[str]): The prompts to use for completition. Only the response from the last
+            prompt in the list will be used for code extraction. Previous prompts can be leveraged
+            to provide a path for the model to produce better results, i.e. for test generation.
+            Uses sentry values to replace values in the prompt.
+                <<FILE_PATH>> - Replaced with the path of the file being transformed.
+                <<FILE_CONTENT>> - Replaced with the content of the file being transformed.
+
+        model_name (optional, str): The model to use for completition. Defaults to gpt-3.5-turbo.
         system_message (optional, Optional[str]): The system message to use. Defaults to None.
         temperature (optional, float): The temperature to use to control the quality of outputs.
             Defaults to 0.4.
-        validators (optional, List[Validator]): A set of validators to use to provide feedback to
-            the LLM with issues it may have produced. Defaults to an empty list.
-        name (ClassVar[TransformerName]): The name of the component.
+        name (ClassVar[ModelName]): The name of the Component.
     """
 
-    prompt: str
-    commands: List[Command] = Field(default_factory=list)
-    max_completion_attempts: int = 3
-    max_validation_attempts: int = 3
-    model: str = "gpt-3.5-turbo"
+    prompts: List[str]
+    model_name: str = "gpt-3.5-turbo"
     system_message: Optional[str] = None
     temperature: float = 0.4
-    validators: List[Validator] = Field(default_factory=list)
-
-    name: ClassVar[TransformerName] = TransformerName.OPEN_AI
-
-    # pylint: disable=invalid-name
-    @validator("max_completion_attempts")
-    @classmethod
-    def max_completion_attempts_must_be_positive(cls, v: int) -> int:
-        """Validates the max_completion_attempts is a positive number.
-
-        Args:
-            v (int): The maximum number of completion attempts for the OpenAI API.
 
-        Raises:
-            ValueError: Raises an error when the max_completion_attempts is not positive.
-
-        Returns:
-            int: The unmodified max_completion_attempts.
-        """
+    name: ClassVar[ModelName] = ModelName.OPEN_AI
 
-        if v < 1:
-            raise ValueError("The max completion attempts must be at least 1")
-        return v
-
-    # pylint: disable=invalid-name
-    @validator("max_validation_attempts")
+    @validator("prompts")
     @classmethod
-    def max_validation_attempts_must_be_positive(cls, v: int) -> int:
-        """Validates the max_validation_attempts is a positive number.
+    def prompts_must_contain_at_least_one_item(cls, v: List[str]) -> List[str]:
+        """Validates there is at least one prompt in the list.
 
         Args:
-            v (int): The maximum number of validation attempts for completion.
+            v (List[str]): The prompts to send to the model.
 
         Raises:
-            ValueError: Raises an error when the max_validation_attempts is not positive.
+            ValueError: Raises an error when the prompts contains no items.
 
         Returns:
-            int: The unmodified max_validation_attempts.
+            int: The unmodified temperature.
         """
 
-        if v < 1:
-            raise ValueError("The max validation attempts must be at least 1")
+        if not v:
+            raise ValueError("At least one prompt must be included in the list")
         return v
 
-    # pylint: disable=invalid-name
     @validator("temperature")
     @classmethod
     def temperature_must_be_valid(cls, v: float) -> float:
         """Validates the temperature is between 0 and 1.
 
         Args:
             v (float): The temperature to use for model completion.
@@ -117,132 +78,127 @@
         Raises:
             ValueError: Raises an error when the temperature is not in the valid range.
 
         Returns:
             int: The unmodified temperature.
         """
 
-        if v >= 1.0 or v <= 0.0:
+        if not 0.0 < v < 1.0:
             raise ValueError("The temperature must be between 0.0 and 1.0")
         return v
 
-    def _transform_item(self, item: Item) -> None:
-        """Replaces a file with the completition results from an OpenAI completition.
+    def get_result_for_item(self, item: FileItem) -> Tuple[str, List[Dict[str, str]]]:
+        """Gets a completion for a FileItem, usually used to find new file content.
 
         Args:
-            item (Item): The file that will be transformed.
-        """
-
-        if openai.api_key is None:
-            openai.api_key = get_config().open_ai_api_key
+            item (FileItem): The FileItem to get the result for.
 
-        assert isinstance(item, FileItem)
+        Returns:
+            Tuple[str, List[Dict[str, str]]]: The result for the Item along with previous
+                messages.
+        """
 
-        event_handler = EventHandler.get()
-        original_content = item.get_content()
-        batch: Batch = {"title": "test", "items": [item]}
+        openai.api_key = openai.api_key or get_config().open_ai_api_key
 
-        # Set up messages for prompt
+        # Set up messages for prompts
         messages = []
         if self.system_message:
             messages.append({"role": "system", "content": self.system_message})
-        messages.append(
-            {
-                "role": "user",
-                "content": self._replace_sentinel_values(self.prompt, item),
-            }
-        )
+        completion_result = ""
 
-        completion_success = False
-        for _ in range(self.max_validation_attempts):
-            # Get completion
-            chat_completion = None
-            for i in range(self.max_completion_attempts):
-                try:
-                    chat_completion = openai.ChatCompletion.create(
-                        model=self.model,
-                        messages=messages,
-                        temperature=self.temperature,
-                    )
-                    break
-                except Exception as e:  # pylint: disable=broad-exception-caught
-                    chat_completion = None
-                    sleep(min(4 ** (i+1), 60))
-                    event_handler.handle(
-                        VerboseEvent({"message": f"API Failure on {item.get_path()}: {e}"}),
-                    )
-
-            if chat_completion is None:
-                item.write_content(original_content)
-                return
-
-            # Log completion information
-            token_usage = (
-                f"Prompt: {chat_completion.usage.prompt_tokens}"
-                + f" - Completition: {chat_completion.usage.completion_tokens}"
-            )
-            event_handler.handle(VerboseEvent({"message": token_usage}))
-            completition_result = chat_completion.choices[0].message.content
-            message = f"The completion result for {item.get_path()}:\n\n{completition_result}"
-            event_handler.handle(VerboseEvent({"message": message}))
-
-            # Update File
-            item.write_content(self._extract_code_from_completion(completition_result))
-
-            # Run commands to fix file
-            for command in self.commands:
-                try:
-                    command.run(batch, None)
-                except Exception:  # pylint: disable=broad-exception-caught
-                    event_handler.handle(
-                        VerboseEvent({"message": f"Failed to run command {command}"})
-                    )
-
-            # Run validators to identify issues with completion
-            failures = []
-            for completion_validator in self.validators:
-                validation_result = completion_validator.check(batch, None)
-                if validation_result.level != ValidationResultLevel.NONE:
-                    failures.append(str(validation_result.message))
-
-            # Check if another completion is required
-            completion_success = not failures
-            if completion_success:
-                break
-
-            # Add messages for handling failures for next completion
-            messages.append({"role": "assistant", "content": completition_result})
-            failure_message = "\n".join(failures)
+        for prompt in self.prompts:
             messages.append(
                 {
                     "role": "user",
-                    "content": f"The following errors were found\n{failure_message}"
-                    + "provide the file with fixes for these errors.",
-                },
+                    "content": self._replace_sentinel_values(prompt, item),
+                }
+            )
+            chat_completion = openai.ChatCompletion.create(
+                model=self.model_name,
+                messages=messages,
+                temperature=self.temperature,
             )
+            completion_result = chat_completion.choices[0].message.content
+            messages.append({"role": "assistant", "content": completion_result})
 
-        # If we had validation failures on our last run, just use the original content
-        if not completion_success:
-            event_handler.handle(
-                VerboseEvent({"message": "Completion failed, using original content"})
+            EventHandler.get().handle(
+                AIModelCompletionEvent(
+                    {
+                        "input_tokens": chat_completion.usage.prompt_tokens,
+                        "output_tokens": chat_completion.usage.completion_tokens,
+                        "completion": chat_completion.choices[0].message.content,
+                    }
+                )
             )
-            item.write_content(original_content)
+
+        return (self._extract_code_from_completion(completion_result), messages)
+
+    def get_result_with_validation(
+        self,
+        item: FileItem,
+        result_data: List[Dict[str, str]],
+        validation_failures: Sequence[ValidationResult],
+    ) -> Tuple[str, List[Dict[str, str]]]:
+        """Gets a new result based on ValidationResult issues.
+
+        Args:
+            item (FileItem): The FileItem to get the result for.
+            result_data (List[Dict[str, str]]): The previously returned result data.
+            validation_failures (Sequence[ValidationResult]): The validation failures.
+
+        Returns:
+            Tuple[str, TResultData]: The result for the failures along with any information needed
+                for future completions.
+        """
+
+        messages = deepcopy(result_data)
+        failure_message = "\n".join(
+            str(validation_result.message) for validation_result in validation_failures
+        )
+        messages.append(
+            {
+                "role": "user",
+                "content": f"The following errors were found\n{failure_message}\n\n"
+                + "Provide the file with fixes for these errors.",
+            },
+        )
+
+        chat_completion = openai.ChatCompletion.create(
+            model=self.model_name,
+            messages=messages,
+            temperature=self.temperature,
+        )
+
+        completion_result = chat_completion.choices[0].message.content
+        messages.append({"role": "assistant", "content": completion_result})
+
+        EventHandler.get().handle(
+            AIModelCompletionEvent(
+                {
+                    "input_tokens": chat_completion.usage.prompt_tokens,
+                    "output_tokens": chat_completion.usage.completion_tokens,
+                    "completion": chat_completion.choices[0].message.content,
+                }
+            )
+        )
+        return (self._extract_code_from_completion(completion_result), messages)
 
     def _replace_sentinel_values(self, prompt: str, item: FileItem) -> str:
-        """Replaces sentinel values in a prompt
+        """Replaces sentinel values in a prompt.
 
         Args:
             prompt (str): The prompt with potential sentinel values to replace.
             item (FileItem): The Item to use for replacing sentinel values.
 
         Returns:
             str: The prompt with sentinel values replaced.
         """
-        new_prompt = prompt.replace("<<FILE_PATH>>", item.get_path())
-        return new_prompt.replace("<<FILE_CONTENT>>", item.get_content())
+        return prompt.replace("<<FILE_PATH>>", item.get_path()).replace(
+            "<<FILE_CONTENT>>", item.get_content()
+        )
 
     def _extract_code_from_completion(self, result: str) -> str:
         """Extracts code from the result of an OpenAI completition.
 
         Args:
             result (str): The completition result.
 
@@ -263,34 +219,7 @@
                 code_lines.append(line)
         # Hit when no formatting is present or only trailing backticks
         if not in_code or not code_lines:
             code = result.removesuffix("```")
         else:
             code = "\n".join(code_lines)
         return code
-
-    @classmethod
-    def from_data(cls: Type[OpenAITransformer], data: Dict[str, Any]) -> OpenAITransformer:
-        """Produces an instance of the component from decoded data.
-
-        Args:
-            data (Mapping[str, Any]): The JSON decoded data.
-
-        Returns:
-            OpenAITransformer: An instance of the component.
-        """
-
-        prompt = data["prompt"]
-        commands = [command_factory.get_instance(c) for c in data.get("commands", [])]
-        model = data.get("model", "gpt-3.5-turbo")
-        system_message = data.get("system_message", None)
-        temperature = data.get("temperature", 0.4)
-        validators = [validator_factory.get_instance(v) for v in data.get("validators", [])]
-
-        return cls(
-            prompt=prompt,
-            commands=commands,
-            model=model,
-            system_message=system_message,
-            temperature=temperature,
-            validators=validators,
-        )
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/transformer/regex.py` & `AutoTransform-1.1.1a9/src/python/autotransform/transformer/regex.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """The implementation for the RegexTransformer."""
 
-from __future__ import annotations
-
 import re
 from typing import ClassVar
 
 from autotransform.item.base import Item
 from autotransform.item.file import FileItem
 from autotransform.transformer.base import TransformerName
 from autotransform.transformer.single import SingleTransformer
@@ -39,13 +37,13 @@
     def _transform_item(self, item: Item) -> None:
         """Replaces all instances of a pattern in the file with the replacement string.
 
         Args:
             item (Item): The file that will be transformed.
         """
 
-        # pylint: disable=unspecified-encoding
+        if not isinstance(item, FileItem):
+            raise TypeError(f"Expected instance of type 'FileItem', got '{type(item).__name__}'")
 
-        assert isinstance(item, FileItem)
         content = item.get_content()
         new_content = re.sub(self.pattern, self.replacement, content)
         item.write_content(new_content)
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/transformer/script.py` & `AutoTransform-1.1.1a9/src/python/autotransform/transformer/script.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,34 +10,38 @@
 """The implementation for the ScriptTransformer."""
 
 from __future__ import annotations
 
 from typing import Any, ClassVar, Dict, List, Optional
 
 from autotransform.batcher.base import Batch
-from autotransform.event.handler import EventHandler
-from autotransform.event.verbose import VerboseEvent
 from autotransform.transformer.base import Transformer, TransformerName
 from autotransform.util.functions import run_cmd_on_items
 from pydantic import root_validator, validator
 
 
 class ScriptTransformer(Transformer[None]):
     """A Transformer that makes changes using an invoked script. Sentinel values can be
     used in args to provide custom arguments for a run.
     The available sentinel values for args are:
-        <<KEY>>: A json encoded list of the Items for a Batch. If the per_item flag is set
-            this will simply be the key of an Item.
+        <<KEY>>: A list of the Items for a Batch. If the per_item flag is set this will simply
+            be the key of an Item.
+        <<TARGET_PATH>>: A list of target_path extra_data field for a Batch. If the per_item flag
+            is set this will simply be the target_path of an Item.
         <<EXTRA_DATA>>: A JSON encoded mapping from Item key to that Item's extra_data. If the
             per_item flag is set, this will simply be a JSON encoding of the Item's extra_data.
             If extra_data is not present for an item, it is treated as an empty Dict.
         <<METADATA>>: A JSON encoded version of the Batch's metadata.
     _FILE can be appended to any of these (i.e. <<KEY_FILE>>) and the arg will instead be replaced
      with a path to a file containing the value.
 
+    Additionally, <<EXTRA_DATA/some_key>> can be used as a sentinel value to get a list of all the
+    values from extra_data for each item with that key. Values will be converted to strings and
+    returned as a list.
+
     Attributes:
         args (List[str]): The arguments to supply to the script.
         script (str): The script to run.
         timeout (int): The timeout to use for the script process.
         chunk_size (Optional[int], optional): The size of chunks to operate on. None indicates no
             chunking. Defaults to None.
         name (ClassVar[TransformerName]): The name of the Component.
@@ -46,15 +50,14 @@
     args: List[str]
     script: str
     timeout: int
     chunk_size: Optional[int] = None
 
     name: ClassVar[TransformerName] = TransformerName.SCRIPT
 
-    # pylint: disable=invalid-name
     @validator("chunk_size")
     @classmethod
     def chunk_size_must_be_positive(cls, v: Optional[int]) -> Optional[int]:
         """Validates that chunk
 
         Args:
             v (Optional[int]): The chunk_size that was set.
@@ -85,15 +88,14 @@
             Mapping[str, Any]: The fixed values.
         """
 
         if "per_item" in values and values["per_item"]:
             if "chunk_size" in values and values["chunk_size"] != 1:
                 raise ValueError("Per item can not be specified with a chunk size that is not 1")
             values["chunk_size"] = 1
-            return values
         return values
 
     def transform(self, batch: Batch) -> None:
         """Executes a simple script to transform the given Batch. Sentinel values can be
         used in args to provide custom arguments for a run.
         The available sentinel values for args are:
             <<KEY>>: A json encoded list of the Items for a Batch.
@@ -103,31 +105,20 @@
         _FILE can be appended to any of these (i.e. <<KEY_FILE>>) and the arg will instead be
         replaced with a path to a file containing the value.
 
         Args:
             batch (Batch): The batch that will be transformed.
         """
 
-        event_handler = EventHandler.get()
-
         metadata = batch.get("metadata", {})
         items = batch["items"]
         num_items = max(len(items), 1)
         chunk_size = self.chunk_size or num_items
 
         # Get Command
         for i in range(0, num_items, chunk_size):
             chunk_items = items[i : i + chunk_size]
             cmd = [self.script]
             cmd.extend(self.args)
 
             proc = run_cmd_on_items(cmd, chunk_items, metadata, timeout=self.timeout)
-
-            if proc.stdout.strip() != "":
-                event_handler.handle(VerboseEvent({"message": f"STDOUT:\n{proc.stdout.strip()}"}))
-            else:
-                event_handler.handle(VerboseEvent({"message": "No STDOUT"}))
-            if proc.stderr.strip() != "":
-                event_handler.handle(VerboseEvent({"message": f"STDERR:\n{proc.stderr.strip()}"}))
-            else:
-                event_handler.handle(VerboseEvent({"message": "No STDERR"}))
             proc.check_returncode()
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/transformer/single.py` & `AutoTransform-1.1.1a9/src/python/autotransform/transformer/single.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
 """An interface for Transformers that operate on single Items with no metadata needs."""
 
-
-from abc import abstractmethod
+from abc import ABC, abstractmethod
+from typing import Sequence
 
 from autotransform.batcher.base import Batch
 from autotransform.item.base import Item
 from autotransform.transformer.base import Transformer
 
 
-class SingleTransformer(Transformer[None]):
+class SingleTransformer(Transformer[None], ABC):
     """A simple interface for writing a Transformer that operates on an individual Item level."""
 
     @abstractmethod
     def _transform_item(self, item: Item) -> None:
         """Executes a transformation on a single Item.
 
         Args:
@@ -31,9 +31,10 @@
     def transform(self, batch: Batch) -> None:
         """Splits out all Items to be transformed.
 
         Args:
             batch (Batch): The Batch being transformed.
         """
 
-        for item in batch["items"]:
+        items: Sequence[Item] = batch.get("items", [])
+        for item in items:
             self._transform_item(item)
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/util/cachedfile.py` & `AutoTransform-1.1.1a9/src/python/autotransform/util/cachedfile.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 # @black_format
 
 """CachedFile is a utility class used by AutoTransform to cache file content on read/write to
 reduce excessive file reads and speed up processing. The FILE_CACHE variable stores cached
 file contents, while a CachedFile object is used to interact with the cache. All writes
 should go through the CachedFile object to ensure the cache is properly updated."""
 
-from typing import Dict
+from pathlib import Path
+from typing import Dict, Optional
 
 FILE_CACHE: Dict[str, str] = {}
+ORIGINAL_FILE_CACHE: Dict[str, Optional[str]] = {}
 
 
 class CachedFile:
 
     """A wrapper that allows accessing cached file contents. Content is stored in the
     FILE_CACHE variable. Writing files outside the CachedFile write method can lead to
     invalid cache data.
@@ -75,23 +77,39 @@
 
         Args:
             path (str): The path to write the file content to.
             content (str): The content to write to the file.
         """
 
         # pylint: disable=unspecified-encoding
-
+        directory = Path(path).parent
+        if not directory.exists():
+            directory.mkdir(parents=True)
         with open(path, "w") as file:
             file.write(content)
             file.flush()
 
     def write_content(self, new_content: str) -> None:
         """Updates the content of a cached file, including writing the file.
 
         Args:
             new_content (str): The content to put in the file.
         """
 
         # pylint: disable=unspecified-encoding
 
+        if self.path not in ORIGINAL_FILE_CACHE:
+            ORIGINAL_FILE_CACHE[self.path] = (
+                self._read(self.path) if Path(self.path).exists() else None
+            )
         self._write(self.path, new_content)
         FILE_CACHE[self.path] = new_content
+
+    def revert(self) -> None:
+        """Reverts the content of a file to its original content."""
+
+        if self.path in ORIGINAL_FILE_CACHE:
+            original_content = ORIGINAL_FILE_CACHE[self.path]
+            if original_content is None:
+                Path(self.path).unlink(missing_ok=True)
+            else:
+                self.write_content(original_content)
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/util/component.py` & `AutoTransform-1.1.1a9/src/python/autotransform/util/component.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/util/console.py` & `AutoTransform-1.1.1a9/src/python/autotransform/util/console.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/util/enums.py` & `AutoTransform-1.1.1a9/src/python/autotransform/util/enums.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/util/functions.py` & `AutoTransform-1.1.1a9/src/python/autotransform/util/functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 
 # @black_format
 
 """Utility functions used by multiple components."""
 
 import json
 import os
+import re
 import subprocess
 from tempfile import NamedTemporaryFile as TmpFile
 from typing import Any, Dict, List, Mapping, Optional, Sequence
 
 from autotransform.event.handler import EventHandler
-from autotransform.event.verbose import VerboseEvent
+from autotransform.event.script import ScriptErrEvent, ScriptOutEvent, ScriptRunEvent
 from autotransform.item.base import Item
 
 
 def run_cmd_on_items(
     cmd: List[str],
     items: Sequence[Item],
     batch_metadata: Mapping[str, Any],
@@ -34,22 +35,29 @@
         batch_metadata (Mapping[str, Any]): The metadata for the batch.
         timeout (optional, Optional[int]): A timeout for the subprocess run. Defaults to None.
 
     Returns:
         subprocess.CompletedProcess: The completed process run.
     """
 
-    event_handler = EventHandler.get()
     item_keys = [item.key for item in items]
     extra_data = {item.key: item.extra_data for item in items if item.extra_data is not None}
+
     arg_replacements = {
         "<<KEY>>": item_keys,
         "<<EXTRA_DATA>>": [json.dumps(extra_data)],
         "<<METADATA>>": [json.dumps(batch_metadata)],
     }
+    for arg in cmd:
+        m = re.match(r"^<<EXTRA_DATA\/(.*)>>$", arg)
+        if m is not None and len(m.groups()) == 1:
+            key = m.groups()[0]
+            arg_replacements[f"<<EXTRA_DATA/{key}>>"] = [
+                str(val.get(key)) for val in extra_data.values() if val.get(key) is not None
+            ]
 
     with TmpFile(mode="w+") as inp, TmpFile(mode="w+") as meta, TmpFile(mode="w+") as extra:
         # Make key file
         json.dump(item_keys, inp)
         inp.flush()
         arg_replacements["<<KEY_FILE>>"] = [inp.name]
 
@@ -62,19 +70,15 @@
         json.dump(batch_metadata, meta)
         meta.flush()
         arg_replacements["<<METADATA_FILE>>"] = [meta.name]
 
         # Create command
         replaced_cmd = replace_script_args(cmd, arg_replacements)
 
-        # Run script
-        event_handler.handle(VerboseEvent({"message": f"Running command: {replaced_cmd}"}))
-        return subprocess.run(
-            replaced_cmd, capture_output=True, encoding="utf-8", check=False, timeout=timeout
-        )
+        return run_cmd(replaced_cmd, timeout)
 
 
 def replace_script_args(args: List[str], replacements: Dict[str, List[str]]) -> List[str]:
     """Replaces arguments in a list with replacements that are supplied.
 
     Args:
         args (List[str]): The argument list.
@@ -96,7 +100,34 @@
         if arg in replacements:
             replaced_args.extend(replacements[arg])
         elif arg in env_replacements:
             replaced_args.extend(env_replacements[arg])
         else:
             replaced_args.append(arg)
     return replaced_args
+
+
+def run_cmd(cmd: List[str], timeout: Optional[int] = None) -> subprocess.CompletedProcess:
+    """Run a script
+
+    Args:
+        cmd (List[str]): The command to run.
+        timeout (optional, Optional[int]): A timeout for the subprocess run. Defaults to None.
+
+    Returns:
+        subprocess.CompletedProcess: The completed process run.
+    """
+
+    event_handler = EventHandler.get()
+
+    event_handler.handle(ScriptRunEvent({"command": cmd}))
+    proc = subprocess.run(cmd, capture_output=True, encoding="utf-8", check=False, timeout=timeout)
+
+    stdout = proc.stdout.strip()
+    if stdout:
+        event_handler.handle(ScriptOutEvent({"stdout": f"STDOUT:\n{stdout}"}))
+
+    stderr = proc.stderr.strip()
+    if stderr:
+        event_handler.handle(ScriptErrEvent({"stderr": f"STDERR:\n{stderr}"}))
+
+    return proc
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/util/github.py` & `AutoTransform-1.1.1a9/src/python/autotransform/util/github.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/util/manager.py` & `AutoTransform-1.1.1a9/src/python/autotransform/util/manager.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/util/package.py` & `AutoTransform-1.1.1a9/src/python/autotransform/util/package.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/util/request.py` & `AutoTransform-1.1.1a9/src/python/autotransform/util/request.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/util/scheduler.py` & `AutoTransform-1.1.1a9/src/python/autotransform/util/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,14 @@
     """
 
     schema_name: str
     schedule: SchemaScheduleSettings
 
     max_submissions: Optional[int] = None
 
-    # pylint: disable=invalid-name
     @validator("max_submissions")
     @classmethod
     def max_submissions_is_positive(cls: Type[ScheduledSchema], v: Optional[int]) -> Optional[int]:
         """Validates that max submissions is positive.
 
         Args:
             cls (Type[ScheduledSchema]): The ScheduledSchema class.
```

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/util/schema_map.py` & `AutoTransform-1.1.1a9/src/python/autotransform/util/schema_map.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/validator/base.py` & `AutoTransform-1.1.1a9/src/python/autotransform/validator/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a8/src/python/autotransform/validator/script.py` & `AutoTransform-1.1.1a9/src/python/autotransform/validator/script.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 
 from __future__ import annotations
 
 from typing import Any, ClassVar, List, Mapping, Optional, Sequence
 
 import autotransform.schema
 from autotransform.batcher.base import Batch
-from autotransform.event.handler import EventHandler
-from autotransform.event.verbose import VerboseEvent
 from autotransform.item.base import Item
 from autotransform.item.file import FileItem
 from autotransform.util.functions import run_cmd_on_items
 from autotransform.validator.base import (
     ValidationResult,
     ValidationResultLevel,
     Validator,
@@ -31,23 +29,27 @@
 class ScriptValidator(Validator):
     """Runs a script with the supplied arguments to perform validation. If the per_item flag is
     set to True, the script will be invoked on each Item. If run_on_changes is set to True, the
     script will replace the Batch Items with FileItems for each changed file. The failure_level
     indicates the result level if the script returns a non-zero exit code. Sentinel values can
     be used in args to provide custom arguments for a run.
     The available sentinel values for args are:
-        <<KEY>>: A json encoded list of the Items for a Batch. If the per_item flag is set
-            this will simply be the key of an Item.
+        <<KEY>>: A list of the Items for a Batch. If the per_item flag is set this will simply
+            be the key of an Item.
         <<EXTRA_DATA>>: A JSON encoded mapping from Item key to that Item's extra_data. If the
             per_item flag is set, this will simply be a JSON encoding of the Item's extra_data.
             If extra_data is not present for an item, it is treated as an empty Dict.
         <<METADATA>>: A JSON encoded version of the Batch's metadata.
     _FILE can be appended to any of these (i.e. <<KEY_FILE>>) and the arg will instead be replaced
      with a path to a file containing the value.
 
+    Additionally, <<EXTRA_DATA/some_key>> can be used as a sentinel value to get a list of all the
+    values from extra_data for each item with that key. Values will be converted to strings and
+    returned as a list.
+
     Attributes:
         args (List[str]): The arguments to supply to the script.
         script (str): The script to run.
         failure_level (ValidationResultLevel, optional): The result level to use if validation
             fails. Defaults to ValidationResultLevel.ERROR.
         per_item (bool, optional): Whether to run the script on each item. Defaults to False.
         run_on_changes (bool, optional): Whether to replace the Items in the batch with
@@ -100,47 +102,35 @@
 
         Args:
             item (Item): The Item that will be validated.
             batch_metadata (Optional[Mapping[str, Any]]): The metadata of the Batch containing the
                 Item.
         """
 
-        event_handler = EventHandler.get()
-
         # Get Command
         cmd = [self.script]
         cmd.extend(self.args)
 
         proc = run_cmd_on_items(cmd, [item], batch_metadata or {})
 
         # Handle output
         level = self.failure_level if proc.returncode != 0 else ValidationResultLevel.NONE
-        if proc.stdout.strip() != "":
-            event_handler.handle(VerboseEvent({"message": f"STDOUT:\n{proc.stdout.strip()}"}))
-        else:
-            event_handler.handle(VerboseEvent({"message": "No STDOUT"}))
-        if proc.stderr.strip() != "":
-            event_handler.handle(VerboseEvent({"message": f"STDERR:\n{proc.stderr.strip()}"}))
-        else:
-            event_handler.handle(VerboseEvent({"message": "No STDERR"}))
         return ValidationResult(
             level=level,
             message=f"[{cmd}]\nSTDOUT:\n{proc.stdout.strip()}\nSTDERR:\n{proc.stderr.strip()}",
             validator=self,
         )
 
     def _check_batch(self, batch: Batch) -> ValidationResult:
         """Executes a simple script to validate the given Batch.
 
         Args:
             batch (Batch): The batch that will be validated.
         """
 
-        event_handler = EventHandler.get()
-
         cmd = [self.script]
 
         # Get items
         if self.run_on_changes:
             current_schema = autotransform.schema.current
             assert current_schema is not None
             repo = current_schema.repo
@@ -153,20 +143,12 @@
         cmd = [self.script]
         cmd.extend(self.args)
 
         proc = run_cmd_on_items(cmd, items, batch.get("metadata", {}))
 
         # Handle output
         level = self.failure_level if proc.returncode != 0 else ValidationResultLevel.NONE
-        if proc.stdout.strip() != "":
-            event_handler.handle(VerboseEvent({"message": f"STDOUT:\n{proc.stdout.strip()}"}))
-        else:
-            event_handler.handle(VerboseEvent({"message": "No STDOUT"}))
-        if proc.stderr.strip() != "":
-            event_handler.handle(VerboseEvent({"message": f"STDERR:\n{proc.stderr.strip()}"}))
-        else:
-            event_handler.handle(VerboseEvent({"message": "No STDERR"}))
         return ValidationResult(
             level=level,
             message=f"[{cmd}]\nSTDOUT:\n{proc.stdout.strip()}\nSTDERR:\n{proc.stderr.strip()}",
             validator=self,
         )
```

