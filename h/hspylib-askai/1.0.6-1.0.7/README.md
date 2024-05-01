# Comparing `tmp/hspylib_askai-1.0.6.tar.gz` & `tmp/hspylib_askai-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib_askai-1.0.6.tar", last modified: Wed Apr 24 04:27:39 2024, max compression
+gzip compressed data, was "hspylib_askai-1.0.7.tar", last modified: Wed May  1 20:19:57 2024, max compression
```

## Comparing `hspylib_askai-1.0.6.tar` & `hspylib_askai-1.0.7.tar`

### file list

```diff
@@ -1,82 +1,96 @@
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.485142 hspylib_askai-1.0.6/
--rw-r--r--   0 hugo       (503) staff       (20)       49 2024-04-20 00:03:24.000000 hspylib_askai-1.0.6/MANIFEST.in
--rw-r--r--   0 hugo       (503) staff       (20)     8142 2024-04-24 04:27:39.484640 hspylib_askai-1.0.6/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)     6006 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/README.md
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.462339 hspylib_askai-1.0.6/askai/
--rw-r--r--   0 hugo       (503) staff       (20)        6 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/.version
--rw-r--r--   0 hugo       (503) staff       (20)      799 2024-04-24 00:20:20.000000 hspylib_askai-1.0.6/askai/__classpath__.py
--rw-r--r--   0 hugo       (503) staff       (20)      180 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/__init__.py
--rwxr-xr-x   0 hugo       (503) staff       (20)     4942 2024-04-24 01:19:17.000000 hspylib_askai-1.0.6/askai/__main__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.465034 hspylib_askai-1.0.6/askai/core/
--rw-r--r--   0 hugo       (503) staff       (20)      341 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)    10896 2024-04-24 03:08:59.000000 hspylib_askai-1.0.6/askai/core/askai.py
--rw-r--r--   0 hugo       (503) staff       (20)     3599 2024-04-24 04:21:42.000000 hspylib_askai-1.0.6/askai/core/askai_configs.py
--rw-r--r--   0 hugo       (503) staff       (20)     2384 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/askai_events.py
--rw-r--r--   0 hugo       (503) staff       (20)     5820 2024-04-24 00:40:38.000000 hspylib_askai-1.0.6/askai/core/askai_messages.py
--rw-r--r--   0 hugo       (503) staff       (20)     1989 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/askai_prompt.py
--rw-r--r--   0 hugo       (503) staff       (20)     4280 2024-04-24 04:25:13.000000 hspylib_askai-1.0.6/askai/core/askai_settings.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.467781 hspylib_askai-1.0.6/askai/core/component/
--rw-r--r--   0 hugo       (503) staff       (20)      272 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/component/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     3606 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/component/audio_player.py
--rw-r--r--   0 hugo       (503) staff       (20)     3778 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/component/cache_service.py
--rw-r--r--   0 hugo       (503) staff       (20)     3380 2024-04-24 00:42:59.000000 hspylib_askai-1.0.6/askai/core/component/geo_location.py
--rw-r--r--   0 hugo       (503) staff       (20)     7132 2024-04-24 00:42:59.000000 hspylib_askai-1.0.6/askai/core/component/internet_service.py
--rw-r--r--   0 hugo       (503) staff       (20)     7125 2024-04-24 03:14:31.000000 hspylib_askai-1.0.6/askai/core/component/recorder.py
--rw-r--r--   0 hugo       (503) staff       (20)     5727 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/component/summarizer.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.468894 hspylib_askai-1.0.6/askai/core/engine/
--rw-r--r--   0 hugo       (503) staff       (20)      200 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/engine/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     2438 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/engine/ai_engine.py
--rw-r--r--   0 hugo       (503) staff       (20)     1992 2024-04-24 00:45:20.000000 hspylib_askai-1.0.6/askai/core/engine/engine_factory.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.470636 hspylib_askai-1.0.6/askai/core/engine/openai/
--rw-r--r--   0 hugo       (503) staff       (20)      237 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/engine/openai/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     2304 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/engine/openai/openai_configs.py
--rw-r--r--   0 hugo       (503) staff       (20)     5752 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/engine/openai/openai_engine.py
--rw-r--r--   0 hugo       (503) staff       (20)     2550 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/engine/openai/openai_model.py
--rw-r--r--   0 hugo       (503) staff       (20)     2800 2024-04-24 00:46:00.000000 hspylib_askai-1.0.6/askai/core/engine/openai/temperature.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.471711 hspylib_askai-1.0.6/askai/core/features/
--rw-r--r--   0 hugo       (503) staff       (20)      191 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/features/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     7696 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/actions.py
--rw-r--r--   0 hugo       (503) staff       (20)     6261 2024-04-24 04:21:02.000000 hspylib_askai-1.0.6/askai/core/features/router.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.474241 hspylib_askai-1.0.6/askai/core/features/tools/
--rw-r--r--   0 hugo       (503) staff       (20)      259 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/features/tools/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     4584 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/tools/analysis.py
--rw-r--r--   0 hugo       (503) staff       (20)     2347 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/tools/browser.py
--rw-r--r--   0 hugo       (503) staff       (20)     2535 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/tools/general.py
--rw-r--r--   0 hugo       (503) staff       (20)     2584 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/tools/generation.py
--rw-r--r--   0 hugo       (503) staff       (20)     2564 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/tools/summarization.py
--rw-r--r--   0 hugo       (503) staff       (20)     5140 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/tools/terminal.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.477377 hspylib_askai-1.0.6/askai/core/model/
--rw-r--r--   0 hugo       (503) staff       (20)      307 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/model/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)      774 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/action_plan.py
--rw-r--r--   0 hugo       (503) staff       (20)      666 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/ai_model.py
--rw-r--r--   0 hugo       (503) staff       (20)      646 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/ai_reply.py
--rw-r--r--   0 hugo       (503) staff       (20)      866 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/query_type.py
--rw-r--r--   0 hugo       (503) staff       (20)     1544 2024-04-24 00:46:35.000000 hspylib_askai-1.0.6/askai/core/model/rag_response.py
--rw-r--r--   0 hugo       (503) staff       (20)      851 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/search_result.py
--rw-r--r--   0 hugo       (503) staff       (20)      737 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/summary_result.py
--rw-r--r--   0 hugo       (503) staff       (20)     1445 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/terminal_command.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.480162 hspylib_askai-1.0.6/askai/core/support/
--rw-r--r--   0 hugo       (503) staff       (20)      296 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/support/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     4891 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/support/chat_context.py
--rw-r--r--   0 hugo       (503) staff       (20)     1612 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/support/langchain_support.py
--rw-r--r--   0 hugo       (503) staff       (20)     4397 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/support/object_mapper.py
--rw-r--r--   0 hugo       (503) staff       (20)     4940 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/support/presets.py
--rw-r--r--   0 hugo       (503) staff       (20)     4802 2024-04-24 00:50:03.000000 hspylib_askai-1.0.6/askai/core/support/shared_instances.py
--rw-r--r--   0 hugo       (503) staff       (20)     3338 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/support/text_formatter.py
--rw-r--r--   0 hugo       (503) staff       (20)     7396 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/support/utilities.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.480859 hspylib_askai-1.0.6/askai/exception/
--rw-r--r--   0 hugo       (503) staff       (20)      161 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/exception/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     2177 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/exception/exceptions.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.481813 hspylib_askai-1.0.6/askai/language/
--rw-r--r--   0 hugo       (503) staff       (20)      183 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/language/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     3627 2024-04-24 00:40:09.000000 hspylib_askai-1.0.6/askai/language/argos_translator.py
--rw-r--r--   0 hugo       (503) staff       (20)     9293 2024-04-24 00:40:09.000000 hspylib_askai-1.0.6/askai/language/language.py
--rw-r--r--   0 hugo       (503) staff       (20)      240 2024-04-20 00:03:24.000000 hspylib_askai-1.0.6/askai/welcome.txt
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.483935 hspylib_askai-1.0.6/hspylib_askai.egg-info/
--rw-r--r--   0 hugo       (503) staff       (20)     8142 2024-04-24 04:27:39.000000 hspylib_askai-1.0.6/hspylib_askai.egg-info/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)     2123 2024-04-24 04:27:39.000000 hspylib_askai-1.0.6/hspylib_askai.egg-info/SOURCES.txt
--rw-r--r--   0 hugo       (503) staff       (20)        1 2024-04-24 04:27:39.000000 hspylib_askai-1.0.6/hspylib_askai.egg-info/dependency_links.txt
--rw-r--r--   0 hugo       (503) staff       (20)      685 2024-04-24 04:27:39.000000 hspylib_askai-1.0.6/hspylib_askai.egg-info/requires.txt
--rw-r--r--   0 hugo       (503) staff       (20)       11 2024-04-24 04:27:39.000000 hspylib_askai-1.0.6/hspylib_askai.egg-info/top_level.txt
--rw-r--r--   0 hugo       (503) staff       (20)       38 2024-04-24 04:27:39.485239 hspylib_askai-1.0.6/setup.cfg
--rw-r--r--   0 hugo       (503) staff       (20)     1988 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/setup.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.045637 hspylib_askai-1.0.7/
+-rw-r--r--   0 hugo       (503) staff       (20)       49 2024-04-20 00:03:24.000000 hspylib_askai-1.0.7/MANIFEST.in
+-rw-r--r--   0 hugo       (503) staff       (20)     8044 2024-05-01 20:19:57.045143 hspylib_askai-1.0.7/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)     5877 2024-05-01 20:19:50.000000 hspylib_askai-1.0.7/README.md
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.007725 hspylib_askai-1.0.7/askai/
+-rw-r--r--   0 hugo       (503) staff       (20)        6 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/.version
+-rw-r--r--   0 hugo       (503) staff       (20)      799 2024-04-24 00:20:20.000000 hspylib_askai-1.0.7/askai/__classpath__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      180 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/__init__.py
+-rwxr-xr-x   0 hugo       (503) staff       (20)     5021 2024-04-25 03:51:29.000000 hspylib_askai-1.0.7/askai/__main__.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.011586 hspylib_askai-1.0.7/askai/core/
+-rw-r--r--   0 hugo       (503) staff       (20)      371 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/core/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)    11573 2024-05-01 01:21:32.000000 hspylib_askai-1.0.7/askai/core/askai.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4321 2024-04-29 03:04:58.000000 hspylib_askai-1.0.7/askai/core/askai_configs.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2384 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/askai_events.py
+-rw-r--r--   0 hugo       (503) staff       (20)     6273 2024-05-01 01:21:32.000000 hspylib_askai-1.0.7/askai/core/askai_messages.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1989 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/askai_prompt.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5610 2024-05-01 01:21:32.000000 hspylib_askai-1.0.7/askai/core/askai_settings.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.013158 hspylib_askai-1.0.7/askai/core/commander/
+-rw-r--r--   0 hugo       (503) staff       (20)      182 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/core/commander/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3892 2024-05-01 01:21:32.000000 hspylib_askai-1.0.7/askai/core/commander/commander.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.014639 hspylib_askai-1.0.7/askai/core/commander/commands/
+-rw-r--r--   0 hugo       (503) staff       (20)      197 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/core/commander/commands/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1837 2024-05-01 01:21:32.000000 hspylib_askai-1.0.7/askai/core/commander/commands/settings_cmd.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3798 2024-05-01 01:21:32.000000 hspylib_askai-1.0.7/askai/core/commander/commands/tts_stt_cmd.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.018822 hspylib_askai-1.0.7/askai/core/component/
+-rw-r--r--   0 hugo       (503) staff       (20)      290 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/core/component/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3606 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/component/audio_player.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3997 2024-04-29 03:22:32.000000 hspylib_askai-1.0.7/askai/core/component/cache_service.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3379 2024-04-25 03:51:29.000000 hspylib_askai-1.0.7/askai/core/component/geo_location.py
+-rw-r--r--   0 hugo       (503) staff       (20)     7169 2024-04-25 03:51:29.000000 hspylib_askai-1.0.7/askai/core/component/internet_service.py
+-rw-r--r--   0 hugo       (503) staff       (20)     8932 2024-05-01 01:21:32.000000 hspylib_askai-1.0.7/askai/core/component/recorder.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4990 2024-04-27 03:17:13.000000 hspylib_askai-1.0.7/askai/core/component/scheduler.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5742 2024-04-25 03:51:29.000000 hspylib_askai-1.0.7/askai/core/component/summarizer.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.020482 hspylib_askai-1.0.7/askai/core/engine/
+-rw-r--r--   0 hugo       (503) staff       (20)      200 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/core/engine/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2544 2024-04-29 02:23:21.000000 hspylib_askai-1.0.7/askai/core/engine/ai_engine.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1990 2024-04-25 03:51:29.000000 hspylib_askai-1.0.7/askai/core/engine/engine_factory.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.022837 hspylib_askai-1.0.7/askai/core/engine/openai/
+-rw-r--r--   0 hugo       (503) staff       (20)      237 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/core/engine/openai/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2202 2024-04-29 02:52:14.000000 hspylib_askai-1.0.7/askai/core/engine/openai/openai_configs.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5972 2024-04-29 02:56:30.000000 hspylib_askai-1.0.7/askai/core/engine/openai/openai_engine.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2550 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/engine/openai/openai_model.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2800 2024-04-24 00:46:00.000000 hspylib_askai-1.0.7/askai/core/engine/openai/temperature.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.024260 hspylib_askai-1.0.7/askai/core/features/
+-rw-r--r--   0 hugo       (503) staff       (20)      191 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/core/features/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     7730 2024-05-01 01:21:32.000000 hspylib_askai-1.0.7/askai/core/features/actions.py
+-rw-r--r--   0 hugo       (503) staff       (20)     6843 2024-04-27 03:17:13.000000 hspylib_askai-1.0.7/askai/core/features/router.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.029321 hspylib_askai-1.0.7/askai/core/features/tools/
+-rw-r--r--   0 hugo       (503) staff       (20)      274 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/core/features/tools/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4832 2024-04-25 03:51:28.000000 hspylib_askai-1.0.7/askai/core/features/tools/analysis.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2347 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/features/tools/browser.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2535 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/features/tools/general.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2536 2024-04-25 03:51:29.000000 hspylib_askai-1.0.7/askai/core/features/tools/generation.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2564 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/features/tools/summarization.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5087 2024-04-25 03:51:29.000000 hspylib_askai-1.0.7/askai/core/features/tools/terminal.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2015 2024-05-01 01:21:32.000000 hspylib_askai-1.0.7/askai/core/features/tools/vision.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.033736 hspylib_askai-1.0.7/askai/core/model/
+-rw-r--r--   0 hugo       (503) staff       (20)      288 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/core/model/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      774 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/model/action_plan.py
+-rw-r--r--   0 hugo       (503) staff       (20)      666 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/model/ai_model.py
+-rw-r--r--   0 hugo       (503) staff       (20)      646 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/model/ai_reply.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1544 2024-04-25 03:51:29.000000 hspylib_askai-1.0.7/askai/core/model/rag_response.py
+-rw-r--r--   0 hugo       (503) staff       (20)      851 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/model/search_result.py
+-rw-r--r--   0 hugo       (503) staff       (20)      737 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/model/summary_result.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1093 2024-04-25 03:51:29.000000 hspylib_askai-1.0.7/askai/core/model/terminal_command.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.037987 hspylib_askai-1.0.7/askai/core/support/
+-rw-r--r--   0 hugo       (503) staff       (20)      296 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/core/support/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4891 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/support/chat_context.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1679 2024-04-25 03:51:29.000000 hspylib_askai-1.0.7/askai/core/support/langchain_support.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4397 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/support/object_mapper.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4940 2024-04-24 00:40:30.000000 hspylib_askai-1.0.7/askai/core/support/presets.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4681 2024-04-25 03:51:29.000000 hspylib_askai-1.0.7/askai/core/support/shared_instances.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3463 2024-05-01 01:21:32.000000 hspylib_askai-1.0.7/askai/core/support/text_formatter.py
+-rw-r--r--   0 hugo       (503) staff       (20)     7515 2024-04-27 03:17:13.000000 hspylib_askai-1.0.7/askai/core/support/utilities.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.039709 hspylib_askai-1.0.7/askai/core/tui/
+-rw-r--r--   0 hugo       (503) staff       (20)      212 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/core/tui/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      433 2024-05-01 01:21:32.000000 hspylib_askai-1.0.7/askai/core/tui/app_icons.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2587 2024-05-01 04:13:43.000000 hspylib_askai-1.0.7/askai/core/tui/app_widgets.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5126 2024-05-01 04:41:32.000000 hspylib_askai-1.0.7/askai/core/tui/askai_app.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3063 2024-05-01 04:43:43.000000 hspylib_askai-1.0.7/askai/core/tui/header.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.040483 hspylib_askai-1.0.7/askai/exception/
+-rw-r--r--   0 hugo       (503) staff       (20)      161 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/exception/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2178 2024-04-25 03:51:28.000000 hspylib_askai-1.0.7/askai/exception/exceptions.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.041898 hspylib_askai-1.0.7/askai/language/
+-rw-r--r--   0 hugo       (503) staff       (20)      183 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/askai/language/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3626 2024-04-25 03:51:29.000000 hspylib_askai-1.0.7/askai/language/argos_translator.py
+-rw-r--r--   0 hugo       (503) staff       (20)     9293 2024-04-25 03:51:29.000000 hspylib_askai-1.0.7/askai/language/language.py
+-rw-r--r--   0 hugo       (503) staff       (20)      240 2024-04-20 00:03:24.000000 hspylib_askai-1.0.7/askai/welcome.txt
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-05-01 20:19:57.044460 hspylib_askai-1.0.7/hspylib_askai.egg-info/
+-rw-r--r--   0 hugo       (503) staff       (20)     8044 2024-05-01 20:19:56.000000 hspylib_askai-1.0.7/hspylib_askai.egg-info/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)     2500 2024-05-01 20:19:56.000000 hspylib_askai-1.0.7/hspylib_askai.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo       (503) staff       (20)        1 2024-05-01 20:19:56.000000 hspylib_askai-1.0.7/hspylib_askai.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo       (503) staff       (20)      701 2024-05-01 20:19:56.000000 hspylib_askai-1.0.7/hspylib_askai.egg-info/requires.txt
+-rw-r--r--   0 hugo       (503) staff       (20)       11 2024-05-01 20:19:56.000000 hspylib_askai-1.0.7/hspylib_askai.egg-info/top_level.txt
+-rw-r--r--   0 hugo       (503) staff       (20)       38 2024-05-01 20:19:57.045723 hspylib_askai-1.0.7/setup.cfg
+-rw-r--r--   0 hugo       (503) staff       (20)     1988 2024-05-01 20:19:53.000000 hspylib_askai-1.0.7/setup.py
```

### Comparing `hspylib_askai-1.0.6/PKG-INFO` & `hspylib_askai-1.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-askai
-Version: 1.0.6
+Version: 1.0.7
 Summary: HomeSetup - AskAI
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-askai/
@@ -19,17 +19,17 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Terminals
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: hspylib>=1.12.36
+Requires-Dist: hspylib>=1.12.38
 Requires-Dist: hspylib-clitt>=0.9.122
-Requires-Dist: hspylib-setman>=0.10.34
+Requires-Dist: hspylib-setman>=0.10.35
 Requires-Dist: retry2==0.9.5
 Requires-Dist: pause==0.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: argostranslate==1.9.1
 Requires-Dist: protobuf==4.22.1
 Requires-Dist: torch==2.2.0
 Requires-Dist: stanza==1.1.1
@@ -54,14 +54,15 @@
 Requires-Dist: opentelemetry-api==1.22.0
 Requires-Dist: opentelemetry-sdk==1.22.0
 Requires-Dist: opentelemetry-proto==1.22.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: pytz==2024.1
 Requires-Dist: bs4==0.0.2
 Requires-Dist: fake_useragent==1.5.1
+Requires-Dist: textual==0.58.0
 
 <img src="https://iili.io/J8wvc1n.png" width="64" height="64" align="right" />
 
 # AskAI
 >
 > Unleash the Power of AI in Your Terminal
 
@@ -77,15 +78,15 @@
 
 <img src="https://iili.io/J8wrBSe.png" width="360" height="360" align="right" />
 
 Born from the idea of empowering individuals with disabilities to navigate the digital world effortlessly, AskAI stands as a beacon of accessibility in the realm of computing. It emerges as a revolutionary solution, harnessing the prowess of AI to bridge the gap between users and the terminal interface. With its intuitive design, AskAI welcomes users of all abilities, eliminating the need for extensive familiarity with shells like bash or zsh. Now, individuals with disabilities can effortlessly command their machines, whether it involves listing files and folders, summarizing documents, accessing real-time data, or delving into a myriad of other functions.
 
 At the heart of AskAI lies its innovative integration of Speech-to-Text and Text-to-Speech technologies, offering a seamless experience for both visually and hearing impaired users. Through these cutting-edge features, individuals can interact with their computers using their natural voice, transcending the barriers imposed by traditional input methods. Moreover, AskAI introduces a unique push-to-talk input mechanism, enabling users to issue commands effortlessly, enhancing the fluidity and ease of interaction.
 
-<img src="https://iili.io/J8wiCqQ.png" style="padding-right: 10px" width="238" height="170" align="left" />
+<img src="https://iili.io/J8wiCqQ.png" style="padding-right: 10px" width="270" height="154" align="left" />
 
 Furthermore, AskAI embraces diversity by breaking language barriers, ensuring that no matter the tongue spoken, users can communicate effectively with their systems. Its adaptive language capabilities ensure that commands are understood and executed accurately, regardless of linguistic nuances. By championing inclusivity on all fronts, AskAI redefines the landscape of computing accessibility, empowering individuals with disabilities to navigate the digital realm with confidence and autonomy.
 
 
 > The world speaks many languages. AskAI understands them all.
 
 The see a brief demo about AskAI feature check our asciinema video.
@@ -99,14 +100,16 @@
 - Seamlessly Integrate AI Models (Currently Supporting OpenAI).
 - Activate Speech-to-Text Inputs via Push-to-Talk Keybinding.
 - Control Text-to-Speech Outputs with Adjustable Speed.
 - Enable Assistive Technology for Visually Impaired Terminal Usage.
 - Enjoy a Natural Typewriter Effect Synced with Speaking Text.
 - Automate Offline Language Translations for Enhanced Accessibility.
 - Interactive and Non-Interactive modes.
+- Image captions to provide textual descriptions for visual content.
+- Enhanced accuracy in responses is achieved through the implementation of a Retrieval-Augmented Generation (RAG) system.
 
 ## Installation
 
 ### Requirements
 
 #### Python
 
@@ -120,31 +123,14 @@
   - Ubuntu 16 and higher
   - CentOS 7 and higher
   - Fedora 31 and higher
 
 You may want to install HsPyLib on other OS's and it will probably work, but there are no guarantees that it
 **WILL ACTUALLY WORK**.
 
-#### Python packages
-
-There are some python dependencies, but they will be automatically downloaded when the build runs. The following python packages are required:
-
-- retry
-- pause
-- requests
-- argostranslate
-- soundfile
-- langchain
-- langchain-openai
-- PyAudio
-- SpeechRecognition
-- openai-whisper
-- urllib3
-- openai
-
 #### Applications / Libraries
 
 The following software are required:
 
 - FFMPEG (To allow playing audio and video files from your terminal).
 - PORTAUDIO (To allow microphone recordings).
```

### Comparing `hspylib_askai-1.0.6/README.md` & `hspylib_askai-1.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 <img src="https://iili.io/J8wrBSe.png" width="360" height="360" align="right" />
 
 Born from the idea of empowering individuals with disabilities to navigate the digital world effortlessly, AskAI stands as a beacon of accessibility in the realm of computing. It emerges as a revolutionary solution, harnessing the prowess of AI to bridge the gap between users and the terminal interface. With its intuitive design, AskAI welcomes users of all abilities, eliminating the need for extensive familiarity with shells like bash or zsh. Now, individuals with disabilities can effortlessly command their machines, whether it involves listing files and folders, summarizing documents, accessing real-time data, or delving into a myriad of other functions.
 
 At the heart of AskAI lies its innovative integration of Speech-to-Text and Text-to-Speech technologies, offering a seamless experience for both visually and hearing impaired users. Through these cutting-edge features, individuals can interact with their computers using their natural voice, transcending the barriers imposed by traditional input methods. Moreover, AskAI introduces a unique push-to-talk input mechanism, enabling users to issue commands effortlessly, enhancing the fluidity and ease of interaction.
 
-<img src="https://iili.io/J8wiCqQ.png" style="padding-right: 10px" width="238" height="170" align="left" />
+<img src="https://iili.io/J8wiCqQ.png" style="padding-right: 10px" width="270" height="154" align="left" />
 
 Furthermore, AskAI embraces diversity by breaking language barriers, ensuring that no matter the tongue spoken, users can communicate effectively with their systems. Its adaptive language capabilities ensure that commands are understood and executed accurately, regardless of linguistic nuances. By championing inclusivity on all fronts, AskAI redefines the landscape of computing accessibility, empowering individuals with disabilities to navigate the digital realm with confidence and autonomy.
 
 
 > The world speaks many languages. AskAI understands them all.
 
 The see a brief demo about AskAI feature check our asciinema video.
@@ -38,14 +38,16 @@
 - Seamlessly Integrate AI Models (Currently Supporting OpenAI).
 - Activate Speech-to-Text Inputs via Push-to-Talk Keybinding.
 - Control Text-to-Speech Outputs with Adjustable Speed.
 - Enable Assistive Technology for Visually Impaired Terminal Usage.
 - Enjoy a Natural Typewriter Effect Synced with Speaking Text.
 - Automate Offline Language Translations for Enhanced Accessibility.
 - Interactive and Non-Interactive modes.
+- Image captions to provide textual descriptions for visual content.
+- Enhanced accuracy in responses is achieved through the implementation of a Retrieval-Augmented Generation (RAG) system.
 
 ## Installation
 
 ### Requirements
 
 #### Python
 
@@ -59,31 +61,14 @@
   - Ubuntu 16 and higher
   - CentOS 7 and higher
   - Fedora 31 and higher
 
 You may want to install HsPyLib on other OS's and it will probably work, but there are no guarantees that it
 **WILL ACTUALLY WORK**.
 
-#### Python packages
-
-There are some python dependencies, but they will be automatically downloaded when the build runs. The following python packages are required:
-
-- retry
-- pause
-- requests
-- argostranslate
-- soundfile
-- langchain
-- langchain-openai
-- PyAudio
-- SpeechRecognition
-- openai-whisper
-- urllib3
-- openai
-
 #### Applications / Libraries
 
 The following software are required:
 
 - FFMPEG (To allow playing audio and video files from your terminal).
 - PORTAUDIO (To allow microphone recordings).
```

### Comparing `hspylib_askai-1.0.6/askai/__classpath__.py` & `hspylib_askai-1.0.7/askai/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/__main__.py` & `hspylib_askai-1.0.7/askai/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,46 +9,46 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 
-import logging as log
-import sys
-from textwrap import dedent
-from typing import Any, Optional
-
 from askai.__classpath__ import classpath
 from askai.core.askai import AskAi
 from clitt.core.term.commons import is_a_tty
 from clitt.core.tui.tui_application import TUIApplication
 from hspylib.core.enums.charset import Charset
 from hspylib.core.tools.commons import to_bool
 from hspylib.core.tools.dict_tools import get_or_default
 from hspylib.core.zoned_datetime import now
 from hspylib.modules.application.argparse.parser_action import ParserAction
 from hspylib.modules.application.exit_status import ExitStatus
 from hspylib.modules.application.version import Version
+from textwrap import dedent
+from typing import Any, Optional
+
+import logging as log
+import sys
 
 if not is_a_tty():
     log.getLogger().setLevel(log.ERROR)
 
 
 class Main(TUIApplication):
     """HomeSetup Ask-AI - Unleash the Power of AI in Your Terminal."""
 
     # The welcome message
-    DESCRIPTION = classpath.get_source("welcome.txt").read_text(encoding=Charset.UTF_8.val)
+    DESCRIPTION: str = classpath.get_source("welcome.txt").read_text(encoding=Charset.UTF_8.val)
 
     # Location of the .version file
-    VERSION = Version.load(load_dir=classpath.source_path())
+    VERSION: Version = Version.load(load_dir=classpath.source_path())
 
     # The resources folder
-    RESOURCE_DIR = str(classpath.resource_path())
+    RESOURCE_DIR: str = str(classpath.resource_path())
 
     INSTANCE: "Main"
 
     def __init__(self, app_name: str):
         super().__init__(app_name, self.VERSION, self.DESCRIPTION.format(self.VERSION), resource_dir=self.RESOURCE_DIR)
         self._askai: AskAi
 
@@ -120,15 +120,15 @@
     def _exec_application(self) -> ExitStatus:
         """Execute the application main flow."""
         self._askai.run()
 
         return ExitStatus.SUCCESS
 
     def _get_argument(self, arg_name: str) -> Optional[Any]:
-        """TODO"""
+        """Get a command line argument, converting to the appropriate type."""
         if arg := self.get_arg(arg_name):
             if isinstance(arg, str):
                 return arg
             elif isinstance(arg, list):
                 return get_or_default(arg, 0, "")
             else:
                 raise TypeError("Argument '' has an invalid type: ''", arg, type(arg))
```

### Comparing `hspylib_askai-1.0.6/askai/core/askai.py` & `hspylib_askai-1.0.7/askai/core/askai.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,55 +10,62 @@
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 import logging as log
 import os
+import re
 import sys
 from functools import partial
 from pathlib import Path
 from threading import Thread
 from typing import List, Optional
 
 import nltk
 import pause
 from askai.__classpath__ import classpath
 from askai.core.askai_configs import configs
 from askai.core.askai_events import ASKAI_BUS_NAME, AskAiEvents, REPLY_ERROR_EVENT, REPLY_EVENT
 from askai.core.askai_messages import msg
 from askai.core.askai_prompt import prompt
+from askai.core.commander.commander import askai
 from askai.core.component.audio_player import player
 from askai.core.component.cache_service import cache, CACHE_DIR
 from askai.core.component.geo_location import geo_location
 from askai.core.component.recorder import recorder
+from askai.core.component.scheduler import scheduler
 from askai.core.engine.ai_engine import AIEngine
 from askai.core.engine.openai.temperature import Temperature
 from askai.core.features.router import router
 from askai.core.support.chat_context import ChatContext
 from askai.core.support.langchain_support import lc_llm
 from askai.core.support.shared_instances import shared
 from askai.core.support.utilities import display_text, read_stdin
 from askai.exception.exceptions import ImpossibleQuery, InaccurateResponse, MaxInteractionsReached, TerminatingQuery
+from click import UsageError
 from clitt.core.term.cursor import cursor
 from clitt.core.term.screen import screen
 from clitt.core.term.terminal import terminal
+from hspylib.core.config.path_object import PathObject
 from hspylib.core.enums.charset import Charset
 from hspylib.core.tools.commons import is_debugging, sysout
 from hspylib.core.tools.text_tools import elide_text
 from hspylib.modules.application.exit_status import ExitStatus
 from hspylib.modules.application.version import Version
 from hspylib.modules.eventbus.event import Event
 from langchain_core.prompts import PromptTemplate
 
 
 class AskAi:
     """Responsible for the OpenAI functionalities."""
 
-    SPLASH = classpath.get_resource("splash.txt").read_text(encoding=Charset.UTF_8.val)
+    SPLASH: str = classpath.get_resource("splash.txt").read_text(encoding=Charset.UTF_8.val)
+
+    RE_ASKAI_CMD: str = r'^(?<!\\)/(\w+)( (.*))*$'
 
     @staticmethod
     def _abort():
         """Abort the execution and exit."""
         sys.exit(ExitStatus.FAILED.val)
 
     def __init__(
@@ -84,29 +91,31 @@
         self._get_query_string(interactive, query)
         configs.is_speak = not quiet
         configs.is_debug = is_debugging() or debug
         configs.tempo = tempo
         configs.is_interactive = interactive
 
     def __str__(self) -> str:
-        device_info = f"{recorder.input_device[1].title()}" if recorder.input_device else ""
+        device_info = f"{recorder.input_device[1]}" if recorder.input_device else ""
+        device_info += f", AUTO-SWAP {'ON' if recorder.is_auto_swap else '%RED%OFF'}"
         dtm = f" {geo_location.datetime} "
+        speak_info = str(configs.tempo) + ' @' + shared.engine.configs.tts_voice
         cur_dir = elide_text(str(Path(os.curdir).absolute()), 67, "…")
         return (
             f"%GREEN%"
             f"AskAI v{Version.load(load_dir=classpath.source_path())} %EOL%"
             f"{dtm.center(80, '=')} %EOL%"
             f"     Engine: {self.engine} %EOL%"
             f"   Language: {configs.language} %EOL%"
             f"    WorkDir: {cur_dir} %EOL%"
             f"{'-' * 80} %EOL%"
             f" Microphone: {device_info or '%RED%Undetected'} %GREEN%%EOL%"
             f"  Debugging: {'ON' if self.is_debugging else '%RED%OFF'} %GREEN%%EOL%"
-            f"   Speaking: {'ON, tempo: ' + str(configs.tempo) if self.is_speak else '%RED%OFF'} %GREEN%%EOL%"
-            f"    Caching: {'ON, TTL: ' + configs.ttl if cache.is_cache_enabled() else '%RED%OFF'} %GREEN%%EOL%"
+            f"   Speaking: {'ON, tempo: ' + speak_info if self.is_speak else '%RED%OFF'} %GREEN%%EOL%"
+            f"    Caching: {'ON, TTL: ' + str(configs.ttl) if cache.is_cache_enabled() else '%RED%OFF'} %GREEN%%EOL%"
             f"{'=' * 80}%EOL%%NC%"
         )
 
     @property
     def engine(self) -> AIEngine:
         return self._engine
 
@@ -195,38 +204,37 @@
             if verbose == "normal" or self.is_debugging:
                 if ev.args.erase_last:
                     cursor.erase_line()
                 self.reply(ev.args.message)
 
     def _splash(self) -> None:
         """Display the AskAI splash screen."""
-        splash_interval = 1000
+        splash_interval = 250
+        screen.clear()
+        sysout(f"%GREEN%{self.SPLASH}%NC%")
         while not self._ready:
-            if not self._processing:
-                screen.clear()
-                sysout(f"%GREEN%{self.SPLASH}%NC%")
             pause.milliseconds(splash_interval)
-        pause.milliseconds(splash_interval)
         screen.clear()
 
     def _startup(self) -> None:
         """Initialize the application."""
         askai_bus = AskAiEvents.get_bus(ASKAI_BUS_NAME)
         askai_bus.subscribe(REPLY_EVENT, self._cb_reply_event)
         askai_bus.subscribe(REPLY_ERROR_EVENT, partial(self._cb_reply_event, error=True))
         if self.is_interactive:
             splash_thread: Thread = Thread(daemon=True, target=self._splash)
             splash_thread.start()
             nltk.download("averaged_perceptron_tagger", quiet=True, download_dir=CACHE_DIR)
             cache.set_cache_enable(self.cache_enabled)
             cache.read_query_history()
             player.start_delay()
+            scheduler.start()
+            recorder.setup()
             self._ready = True
             splash_thread.join()
-            recorder.setup()
             display_text(self, markdown=False)
             self.reply(msg.welcome(os.getenv("USER", "you")))
         else:
             recorder.setup()
             player.start_delay()
         log.info("AskAI is ready to use!")
 
@@ -244,43 +252,49 @@
 
     def _ask_and_reply(self, question: str) -> bool:
         """Ask the question and provide the reply.
         :param question: The question to ask to the AI engine.
         """
         status = True
         try:
-            if not (reply := cache.read_reply(question)):
+            if command := re.search(self.RE_ASKAI_CMD, question):
+                args: list[str] = list(filter(
+                    lambda a: a and a != 'None', re.split(r'\s', f"{command.group(1)} {command.group(2)}")
+                ))
+                askai(args, standalone_mode=False)
+            elif not (reply := cache.read_reply(question)):
                 log.debug('Response not found for "%s" in cache. Querying from %s.', question, self.engine.nickname())
                 AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.wait())
                 if output := router.process(question):
                     self.reply(output)
             else:
                 log.debug("Reply found for '%s' in cache.", question)
                 self.reply(reply)
         except (NotImplementedError, ImpossibleQuery) as err:
             self.reply_error(str(err))
         except (MaxInteractionsReached, InaccurateResponse, ValueError) as err:
-            self.reply_error(msg.unprocessable(str(err)))
+            self.reply_error(msg.unprocessable(type(err)))
+        except UsageError as err:
+            self.reply_error(msg.invalid_command(err))
         except TerminatingQuery:
             status = False
 
         return status
 
     def _get_query_string(self, interactive: bool, query_arg: str | list[str]) -> None:
         """Retrieve the proper query string used in the non interactive mode.
         :param interactive: The interactive mode.
         :param query_arg: The query argument provided by the command line.
         """
         query: str = str(" ".join(query_arg) if isinstance(query_arg, list) else query_arg)
         self._question = query
-        dir_name, file_name = os.path.split(self._query_prompt)
+        dir_name, file_name = PathObject.split(self._query_prompt)
         if not interactive:
             stdin_args = read_stdin()
             template = PromptTemplate(
-                input_variables=["context", "question"],
-                template=prompt.read_prompt(file_name, dir_name.replace("~", os.getenv("HOME"))),
+                input_variables=["context", "question"], template=prompt.read_prompt(file_name, dir_name)
             )
             final_prompt = template.format(context=stdin_args, question=self._question)
             self._query_string = final_prompt if query else stdin_args
             self._question = self._question or self._query_string
         else:
             self._query_string = query
```

### Comparing `hspylib_askai-1.0.6/askai/core/askai_configs.py` & `hspylib_askai-1.0.7/askai/core/askai_configs.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,19 +11,20 @@
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 import os
 from shutil import which
 
+from hspylib.core.enums.charset import Charset
+from hspylib.core.metaclass.singleton import Singleton
+
 from askai.__classpath__ import classpath
 from askai.core.askai_settings import settings
 from askai.language.language import Language
-from hspylib.core.enums.charset import Charset
-from hspylib.core.metaclass.singleton import Singleton
 
 
 class AskAiConfigs(metaclass=Singleton):
     """Provides access to AskAI configurations."""
 
     INSTANCE: "AskAiConfigs"
 
@@ -66,19 +67,19 @@
 
     @is_cache.setter
     def is_cache(self, value: bool) -> None:
         settings.put("askai.cache.enabled", value)
 
     @property
     def tempo(self) -> int:
-        return settings.get_int("askai.speech.tempo")
+        return settings.get_int("askai.text.to.speech.tempo")
 
     @tempo.setter
     def tempo(self, value: int) -> None:
-        settings.get_int("askai.speech.tempo", value)
+        settings.get_int("askai.text.to.speech.tempo", value)
 
     @property
     def language(self) -> Language:
         return self._language
 
     @property
     def encoding(self) -> Charset:
@@ -101,20 +102,38 @@
         return settings.get_int("askai.max.router.retries")
 
     @property
     def max_agent_execution_time_seconds(self) -> int:
         return settings.get_int("askai.max.agent.execution.time.seconds")
 
     @property
+    def recorder_phrase_limit_millis(self) -> int:
+        return settings.get_int("askai.recorder.phrase.limit.millis")
+
+    @property
+    def recorder_silence_timeout_millis(self) -> int:
+        return settings.get_int("askai.recorder.silence.timeout.millis")
+
+    @property
+    def recorder_noise_detection_duration_millis(self) -> int:
+        return settings.get_int("askai.recorder.noise.detection.duration.millis")
+
+    @property
+    def recorder_input_device_auto_swap(self) -> bool:
+        return settings.get_bool("askai.recorder.input.device.auto.swap")
+
+    @property
     def recorder_devices(self) -> list[str]:
         return self._recorder_devices
 
     def add_device(self, device_name: str) -> None:
-        self._recorder_devices.append(device_name)
-        settings.put("askai.recorder.devices", ', '.join(self._recorder_devices))
+        if device_name not in self._recorder_devices:
+            self._recorder_devices.insert(0, device_name)
+            settings.put("askai.recorder.devices", ", ".join(self._recorder_devices))
 
     def remove_device(self, device_name: str) -> None:
-        self._recorder_devices.remove(device_name)
-        settings.put("askai.recorder.devices", ', '.join(self._recorder_devices))
+        if device_name in self._recorder_devices:
+            self._recorder_devices.remove(device_name)
+            settings.put("askai.recorder.devices", ", ".join(self._recorder_devices))
 
 
 assert (configs := AskAiConfigs().INSTANCE) is not None
```

### Comparing `hspylib_askai-1.0.6/askai/core/askai_events.py` & `hspylib_askai-1.0.7/askai/core/askai_events.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/askai_messages.py` & `hspylib_askai-1.0.7/askai/core/askai_messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,20 @@
    @created: Fri, 5 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
-from functools import cached_property, lru_cache
-
-from hspylib.core.metaclass.singleton import Singleton
-from hspylib.modules.application.exit_status import ExitStatus
-
 from askai.core.askai_configs import configs
 from askai.language.argos_translator import ArgosTranslator
 from askai.language.language import Language
+from functools import cached_property, lru_cache
+from hspylib.core.metaclass.singleton import Singleton
+from hspylib.modules.application.exit_status import ExitStatus
 
 
 class AskAiMessages(metaclass=Singleton):
     """Provide access to static 'translated' messages."""
 
     INSTANCE: "AskAiMessages"
 
@@ -114,14 +112,22 @@
     def action_plan(self, plan_text: str) -> str:
         return self.translate(f"@ Action plan: `{plan_text}`")
 
     @lru_cache
     def x_reference(self) -> str:
         return self.translate(f"> Looking for **X-References**…")
 
+    @lru_cache
+    def describe_image(self, image_path: str) -> str:
+        return self.translate(f"Describing image: `{image_path}` …")
+
+    @lru_cache
+    def device_switch(self, device_info: str) -> str:
+        return self.translate(f"\nSwitching to Audio Input device: `{device_info}`")
+
     # Warnings and alerts
 
     @lru_cache
     def search_empty(self) -> str:
         return self.translate("The search didn't return an output !")
 
     @lru_cache
@@ -135,14 +141,18 @@
         return self.translate("No query string was provided in non-interactive mode !")
 
     @lru_cache
     def invalid_response(self, response_text: str) -> str:
         return self.translate(f"Invalid query response/type => '{response_text}' !")
 
     @lru_cache
+    def invalid_command(self, response_text: str) -> str:
+        return self.translate(f"Invalid **AskAI** command => '{response_text}' !")
+
+    @lru_cache
     def cmd_no_exist(self, command: str) -> str:
         return self.translate(f"Command `{command}' does not exist !")
 
     @lru_cache
     def cmd_failed(self, cmd_line: str) -> str:
         return self.translate(f"Command `{cmd_line}' failed to execute !")
 
@@ -172,11 +182,11 @@
 
     @lru_cache
     def too_many_actions(self) -> str:
         return self.translate("Failed to complete the request => 'Max chained actions reached' !")
 
     @lru_cache
     def unprocessable(self, reason: str) -> str:
-        return self.translate(f"Sorry, I was unable to process your request => {reason}")
+        return self.translate(f"Sorry, I was unable to process your request => '{reason}'")
 
 
 assert (msg := AskAiMessages().INSTANCE) is not None
```

### Comparing `hspylib_askai-1.0.6/askai/core/askai_prompt.py` & `hspylib_askai-1.0.7/askai/core/askai_prompt.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/askai_settings.py` & `hspylib_askai-1.0.7/askai/core/askai_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,80 +11,112 @@
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 import logging as log
 import os
 import re
+from contextlib import redirect_stdout
+from io import StringIO
+from pathlib import Path
 from typing import Any, Optional
 
-from askai.__classpath__ import classpath
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.tools.commons import to_bool
+from rich.table import Table
 from setman.settings.settings import Settings
 from setman.settings.settings_config import SettingsConfig
 from setman.settings.settings_entry import SettingsEntry
 
+from askai.__classpath__ import classpath
+from askai.core.support.text_formatter import text_formatter
+
+# AskAI config directory.
+ASKAI_DIR: Path = Path(f'{os.getenv("HHS_DIR", os.getenv("ASKAI_DIR", os.getenv("TEMP", "/tmp")))}/askai')
+if not ASKAI_DIR.exists():
+    ASKAI_DIR: Path = classpath.resource_path()
+
+# Make sure the AskAI directory is exported.
+os.environ["ASKAI_DIR"] = str(ASKAI_DIR)
+
 
 class AskAiSettings(metaclass=Singleton):
     """The Setman Settings."""
 
-    INSTANCE: 'AskAiSettings'
-
-    SETTINGS_DIR = f'{os.getenv("HHS_DIR", os.getenv("TEMP", "/tmp"))}'
+    INSTANCE: "AskAiSettings"
 
     RESOURCE_DIR = str(classpath.resource_path())
 
-    _ACTUAL_VERSION: str = '0.0.2'
+    _ACTUAL_VERSION: str = "0.0.5"
 
     def __init__(self) -> None:
-        self._db_file = f"{self.SETTINGS_DIR}/askai/askai.db"
         self._configs = SettingsConfig(self.RESOURCE_DIR, "application.properties")
         self._settings = Settings(self._configs)
         if not self._settings.count() or self.get("askai.settings.version.id") != self._ACTUAL_VERSION:
-            self._defaults()
+            self.defaults()
 
     def __str__(self) -> str:
-        return str(self._settings)
+        return self.search()
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def __getitem__(self, name: str) -> Optional[SettingsEntry]:
         return self._settings.get(name)
 
     def __setitem__(self, name: str, item: Any) -> None:
-        self._settings.put(name, name[:name.find('.')], item)
+        self._settings.put(name, name[: name.find(".")], item)
+
+    @property
+    def settings(self) -> Settings:
+        return self._settings
+
+    def search(self, filters: str | None = None) -> Optional[str]:
+        data = [(s.name, s.value) for s in self._settings.search(filters)]
+        if data:
+            table = Table(title="AskAI - Settings")
+            table.add_column("No.", style="white", no_wrap=True)
+            table.add_column("Name", style="cyan", no_wrap=True)
+            table.add_column("Value", style="green", no_wrap=True)
+            for i, d in enumerate(data):
+                table.add_row(str(i), d[0], d[1])
+            with StringIO() as buf, redirect_stdout(buf):
+                text_formatter.console.print(table)
+                return buf.getvalue()
+        return None
 
-    def _defaults(self) -> None:
+    def defaults(self) -> None:
         """Create the default settings database if they doesn't exist."""
         # AskAI General
         self._settings.clear()
         self._settings.put("askai.settings.version.id", "askai", self._ACTUAL_VERSION)
         self._settings.put("askai.debug.enabled", "askai", False)
         self._settings.put("askai.speak.enabled", "askai", False)
         self._settings.put("askai.cache.enabled", "askai", False)
         self._settings.put("askai.cache.ttl.minutes", "askai", 30)
-        self._settings.put("askai.speech.tempo", "askai", 1)
+        self._settings.put("askai.text.to.speech.tempo", "askai", 1)
         # Router
-        self._settings.put("askai.max.context.size", "askai", 3)
+        self._settings.put("askai.max.context.size", "askai", 5)
         self._settings.put("askai.max.iteractions", "askai", 30)
         self._settings.put("askai.max.router.retries", "askai", 3)
+        self._settings.put("askai.max.agent.execution.time.seconds", "askai", 120)
         # Recorder
         self._settings.put("askai.recorder.devices", "askai", "")
-        self._settings.put("askai.recorder.silence.timeout.millis", "askai", 1500)
-        self._settings.put("askai.recorder.phrase.limit.millis", "askai", 0)
+        self._settings.put("askai.recorder.silence.timeout.millis", "askai", 800)
+        self._settings.put("askai.recorder.phrase.limit.millis", "askai", 10000)
+        self._settings.put("askai.recorder.noise.detection.duration.millis", "askai", 600)
+        self._settings.put("askai.recorder.input.device.auto.swap", "askai", True)
         # OpenAI
         self._settings.put("openai.speech.to.text.model", "openai", "whisper-1")
         self._settings.put("openai.text.to.speech.model", "openai", "tts-1")
         self._settings.put("openai.text.to.speech.voice", "openai", "onyx")
         self._settings.put("openai.text.to.speech.audio.format", "openai", "mp3")
-        log.debug(f"Settings database created at: '{self._db_file}'")
+        log.debug(f"Settings database created !")
 
-    def get(self, key: str, default_value: str | None = '') -> str:
+    def get(self, key: str, default_value: str | None = "") -> str:
         val = self.__getitem__(key)
         return str(val.value) if val else default_value
 
     def put(self, key: str, value: Any) -> None:
         self.__setitem__(key, value)
 
     def get_bool(self, key: str, default_value: bool | None = False) -> bool:
@@ -99,15 +131,15 @@
     def get_float(self, key: str, default_value: float | None = 0.0) -> float:
         try:
             return float(self.get(key) or default_value)
         except ValueError:
             return 0
 
     def get_list(self, key: str, default_value: list | None = None) -> list:
-        str_val: str = self.get(key) or ''
+        str_val: str = self.get(key) or ""
         val: list | None = None
         if str_val:
-            val: list = re.split(r'[;,|]', str_val)
+            val: list = re.split(r"[;,|]", str_val)
         return val or default_value or []
 
 
 assert (settings := AskAiSettings().INSTANCE) is not None
```

### Comparing `hspylib_askai-1.0.6/askai/core/component/audio_player.py` & `hspylib_askai-1.0.7/askai/core/component/audio_player.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/component/cache_service.py` & `hspylib_askai-1.0.7/askai/core/component/cache_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,37 +8,44 @@
    @created: Tue, 16 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
-from askai.core.support.utilities import hash_text
+from pathlib import Path
+from typing import Optional, Tuple
+
 from clitt.core.tui.line_input.keyboard_input import KeyboardInput
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.tools.commons import file_is_not_empty
 from hspylib.modules.cache.ttl_cache import TTLCache
-from pathlib import Path
-from typing import List, Optional, Tuple
 
-import os
+from askai.core.askai_settings import ASKAI_DIR
+from askai.core.support.utilities import hash_text
+
+# AskAI cache root directory.
+CACHE_DIR: Path = Path(f"{ASKAI_DIR}/cache")
 
-CACHE_DIR: Path = Path(f'{os.getenv("HHS_DIR", os.getenv("TEMP", "/tmp"))}/askai/cache')
+# Settings directory.
+SETTINGS_DIR: Path = Path(str(ASKAI_DIR) + "/settings")
+if not SETTINGS_DIR.exists():
+    SETTINGS_DIR.mkdir(parents=True, exist_ok=True)
 
-# Transcribed audio directory.
+# Transcribed audio cache directory.
 AUDIO_DIR: Path = Path(str(CACHE_DIR) + "/audio")
 if not AUDIO_DIR.exists():
     AUDIO_DIR.mkdir(parents=True, exist_ok=True)
 
-# Voice recordings directory.
+# Voice recordings cache directory.
 REC_DIR: Path = Path(str(CACHE_DIR) + "/recordings")
 if not REC_DIR.exists():
     REC_DIR.mkdir(parents=True, exist_ok=True)
 
-# Transcribed audio directory.
+# Transcribed audio cache directory.
 PERSIST_DIR: Path = Path(str(CACHE_DIR) + "/chroma")
 if not PERSIST_DIR.exists():
     PERSIST_DIR.mkdir(parents=True, exist_ok=True)
 
 
 class CacheService(metaclass=Singleton):
     """Provide a cache service for previously used queries, audio generation, etc..."""
@@ -84,29 +91,28 @@
         cls._TTL_CACHE.save(key, reply)
 
     @classmethod
     def read_query_history(cls) -> None:
         """Read the input queries from TTL cache."""
         hist_str: str = cls._TTL_CACHE.read(cls.ASKAI_INPUT_CACHE_KEY)
         if hist_str:
-            hist: List[str] = hist_str.split(",")
-            hist.reverse()
-            KeyboardInput.preload_history(hist)
+            KeyboardInput.preload_history(hist_str.split(","))
 
     @classmethod
     def save_query_history(cls) -> None:
         """Save the line input queries into the TTL cache."""
         hist = KeyboardInput.history()
         cls._TTL_CACHE.save(cls.ASKAI_INPUT_CACHE_KEY, ",".join(hist))
 
     @classmethod
-    def get_audio_file(cls, text: str, audio_format: str = "mp3") -> Tuple[str, bool]:
+    def get_audio_file(cls, text: str, voice: str = "onyx", audio_format: str = "mp3") -> Tuple[str, bool]:
         """Retrieve the audio file path and whether it exists or not.
         :param text: Text to be cached. This is the text that the audio is speaking.
+        :param voice: The voice used.
         :param audio_format: The audio format used.
         """
-        key = text.strip().lower()
+        key = f"{text.strip().lower()}-{hash_text(voice)}"
         audio_file_path = f"{str(AUDIO_DIR)}/askai-{hash_text(key)}.{audio_format}"
         return audio_file_path, file_is_not_empty(audio_file_path)
 
 
 assert (cache := CacheService().INSTANCE) is not None
```

### Comparing `hspylib_askai-1.0.6/askai/core/component/geo_location.py` & `hspylib_askai-1.0.7/askai/core/component/geo_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,26 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 
-import json
-import logging as log
+from askai.core.askai_configs import configs
 from datetime import datetime
-from json import JSONDecodeError
-from textwrap import dedent
-
-import pytz
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.namespace import Namespace
 from hspylib.modules.fetch import fetch
+from json import JSONDecodeError
 from requests.exceptions import ConnectionError
+from textwrap import dedent
 
-from askai.core.askai_configs import configs
+import json
+import logging as log
+import pytz
 
 
 class GeoLocation(metaclass=Singleton):
     """TODO"""
 
     INSTANCE: "GeoLocation"
```

### Comparing `hspylib_askai-1.0.6/askai/core/component/internet_service.py` & `hspylib_askai-1.0.7/askai/core/component/internet_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,43 +8,42 @@
    @created: Sun, 10 Mar 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
-import logging as log
-import re
+from askai.core.askai_events import AskAiEvents
+from askai.core.askai_messages import msg
+from askai.core.askai_prompt import prompt
+from askai.core.component.geo_location import geo_location
+from askai.core.component.summarizer import summarizer
+from askai.core.engine.openai.temperature import Temperature
+from askai.core.model.search_result import SearchResult
+from askai.core.support.langchain_support import lc_llm
+from askai.core.support.shared_instances import shared
 from functools import lru_cache
-from typing import List
-
-import bs4
 from googleapiclient.errors import HttpError
 from hspylib.core.metaclass.singleton import Singleton
 from langchain.chains.combine_documents import create_stuff_documents_chain
 from langchain_community.document_loaders.web_base import WebBaseLoader
 from langchain_community.utilities import GoogleSearchAPIWrapper
 from langchain_community.vectorstores.chroma import Chroma
 from langchain_core.documents import Document
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.prompts import ChatPromptTemplate, PromptTemplate
 from langchain_core.runnables import RunnablePassthrough
 from langchain_core.runnables.utils import Output
 from langchain_core.tools import Tool
 from langchain_text_splitters import RecursiveCharacterTextSplitter
+from typing import List
 
-from askai.core.askai_events import AskAiEvents
-from askai.core.askai_messages import msg
-from askai.core.askai_prompt import prompt
-from askai.core.component.geo_location import geo_location
-from askai.core.component.summarizer import summarizer
-from askai.core.engine.openai.temperature import Temperature
-from askai.core.model.search_result import SearchResult
-from askai.core.support.langchain_support import lc_llm
-from askai.core.support.shared_instances import shared
+import bs4
+import logging as log
+import re
 
 
 class InternetService(metaclass=Singleton):
     """Provide a internet search service to complete queries that require realtime data."""
 
     INSTANCE: "InternetService"
 
@@ -112,15 +111,17 @@
                 web_paths=search.sites,
                 bs_kwargs=dict(parse_only=bs4.SoupStrainer(["article", "span", "div", "h1", "h2", "h3"])),
             )
             if (page_content := loader.load()) and len(page_content) > 0:
                 splits: List[Document] = summarizer.text_splitter.split_documents(page_content)
                 v_store = Chroma.from_documents(splits, lc_llm.create_embeddings())
                 retriever = v_store.as_retriever()
-                scrap_prompt = PromptTemplate(input_variables=["context", "question"], template=prompt.read_prompt("qstring"))
+                scrap_prompt = PromptTemplate(
+                    input_variables=["context", "question"], template=prompt.read_prompt("qstring")
+                )
 
                 def format_docs(docs):
                     return "\n\n".join(doc.page_content for doc in docs)
 
                 rag_chain = (
                     {"context": retriever | format_docs, "question": RunnablePassthrough()}
                     | scrap_prompt
```

### Comparing `hspylib_askai-1.0.6/askai/core/component/recorder.py` & `hspylib_askai-1.0.7/askai/core/component/recorder.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,91 +8,133 @@
    @created: Wed, 22 Feb 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
+
 import logging as log
+import operator
 from pathlib import Path
-from typing import Callable, List, Optional, Tuple
+from typing import Callable, Optional, Tuple
 
 import pause
-from askai.core.askai_configs import configs
-from askai.core.askai_events import AskAiEvents
-from askai.core.askai_messages import msg
-from askai.core.component.cache_service import REC_DIR
-from askai.core.support.utilities import display_text
-from askai.exception.exceptions import IntelligibleAudioError, InvalidInputDevice, InvalidRecognitionApiError
-from askai.language.language import Language
 from clitt.core.term.cursor import cursor
 from clitt.core.tui.mselect.mselect import mselect
 from hspylib.core.enums.enumeration import Enumeration
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.zoned_datetime import now_ms
 from speech_recognition import AudioData, Microphone, Recognizer, RequestError, UnknownValueError, WaitTimeoutError
 
+from askai.core.askai_configs import configs
+from askai.core.askai_events import AskAiEvents
+from askai.core.askai_messages import msg
+from askai.core.component.cache_service import REC_DIR
+from askai.core.component.scheduler import Scheduler
+from askai.core.support.utilities import display_text, seconds
+from askai.exception.exceptions import IntelligibleAudioError, InvalidInputDevice, InvalidRecognitionApiError
+from askai.language.language import Language
+
 
 class Recorder(metaclass=Singleton):
     """Provide an interface to record voice using the microphone device."""
 
     INSTANCE: "Recorder"
 
     class RecognitionApi(Enumeration):
         # fmt: off
         OPEN_AI = 'recognize_whisper'
         GOOGLE = 'recognize_google'
         # fmt: on
 
     @classmethod
-    def get_device_list(cls) -> List[Tuple[int, str]]:
+    def get_device_list(cls) -> list[Tuple[int, str]]:
         """Return a list of available devices."""
         devices = []
         for index, name in enumerate(Microphone.list_microphone_names()):
             devices.append((index, name))
         return devices
 
     def __init__(self):
         self._rec: Recognizer = Recognizer()
         self._devices: list[tuple[int, str]] = []
         self._device_index = None
         self._input_device = None
-        self._rec_phrase_limit_s = 10
-        self._rec_wait_timeout_s = 0.8
+        self._old_device = None
 
     def setup(self) -> None:
         """Setup the recorder."""
         self._devices = self.get_device_list()
         log.debug("Available audio devices:\n%s", "\n".join([f"{d[0]} - {d[1]}" for d in self._devices]))
         self._device_index = self._select_device()
         self._input_device = self._devices[self._device_index] if self._device_index is not None else None
 
+    @staticmethod
+    @Scheduler.every(2000, 10000)
+    def __device_watcher() -> None:
+        """Watch for device changes and swap if a new input device is found."""
+        if recorder.is_auto_swap and recorder.devices:
+            new_list = recorder.get_device_list()
+            new_list.sort(key=operator.itemgetter(1))
+            if len(recorder.devices) < len(new_list):
+                new_devices = [d for d in new_list if d not in recorder.devices]
+                for device in new_devices:
+                    if recorder.test_device(device[0]):
+                        log.info(msg.device_switch(str(device)))
+                        AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.device_switch(str(device)), erase_last=True)
+                        recorder._input_device = device[0]
+                        configs.add_device(device[1])
+                        break
+            elif len(recorder.devices) > len(new_list):
+                for device in recorder.devices:
+                    if recorder.test_device(device[0]):
+                        log.info(msg.device_switch(str(device)))
+                        AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.device_switch(str(device)), erase_last=True)
+                        recorder._input_device = device[0]
+                        break
+            recorder.devices = new_list
+
     @property
-    def devices(self) -> List[Tuple[int, str]]:
+    def devices(self) -> list[Tuple[int, str]]:
+        """TODO"""
         return self._devices if self._devices else []
 
+    @devices.setter
+    def devices(self, value: list[Tuple[int, str]]) -> None:
+        self._devices = value
+
     @property
     def input_device(self) -> Optional[Tuple[int, str]]:
+        """TODO"""
         return self._input_device if self._input_device else None
 
+    @property
+    def is_auto_swap(self) -> bool:
+        """TODO"""
+        return configs.recorder_input_device_auto_swap
+
     def listen(
-        self, recognition_api: RecognitionApi = RecognitionApi.OPEN_AI, language: Language = Language.EN_US
+        self,
+        recognition_api: RecognitionApi = RecognitionApi.OPEN_AI,
+        language: Language = Language.EN_US
     ) -> Tuple[Path, Optional[str]]:
-        """Listen to the microphone, save the AudioData as a wav file and then, transcribe the speech.
+        """listen to the microphone, save the AudioData as a wav file and then, transcribe the speech.
         :param recognition_api: the API to be used to recognize the speech.
         :param language: the spoken language.
         """
         audio_path = Path(f"{REC_DIR}/askai-stt-{now_ms()}.wav")
         with Microphone(device_index=self._device_index) as source:
             try:
                 self._detect_noise()
                 AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.listening())
                 audio: AudioData = self._rec.listen(
-                    source, phrase_time_limit=self._rec_phrase_limit_s, timeout=self._rec_wait_timeout_s
-                )
+                    source,
+                    phrase_time_limit=seconds(configs.recorder_phrase_limit_millis),
+                    timeout=seconds(configs.recorder_silence_timeout_millis))
                 AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.transcribing(), erase_last=True)
                 with open(audio_path, "wb") as f_rec:
                     f_rec.write(audio.get_wav_data())
                     log.debug("Voice recorded and saved as %s", audio_path)
                 if api := getattr(self._rec, recognition_api.value):
                     log.debug("Recognizing voice using %s", recognition_api)
                     assert isinstance(api, Callable)
@@ -108,65 +150,63 @@
             except UnknownValueError as err:
                 raise IntelligibleAudioError(str(err)) from err
             except RequestError as err:
                 raise InvalidRecognitionApiError(str(err)) from err
 
         return audio_path, stt_text
 
-    def _detect_noise(self, interval: float = 0.8) -> None:
-        """Detect and adjust the background noise level.
-        :param interval: the interval in seconds of the noise detection.
+    def test_device(self, idx: int) -> bool:
+        """Test whether the input device specified by index can be used as an STT input.
+        :param idx: The index of the device to be tested.
         """
+        log.debug(f"Testing audio input device at index: '%d'", idx)
+        test_timeout, test_phrase_limit = 0.5, 0.5
+        try:
+            with Microphone(device_index=idx) as source:
+                self._rec.listen(source, timeout=test_timeout, phrase_time_limit=test_phrase_limit)
+                return True
+        except WaitTimeoutError:
+            log.info(f"Device at index: '%d' is functional!", idx)
+            return True
+        except (AssertionError, AttributeError):
+            log.warning(f"Device at index: '%d' is non functional!", idx)
+
+        return False
+
+    def _detect_noise(self) -> None:
+        """Detect and adjust the background noise level."""
         with Microphone() as source:
             try:
                 log.debug("Adjusting noise levels…")
-                self._rec.adjust_for_ambient_noise(source, duration=interval)
+                duration = seconds(configs.recorder_noise_detection_duration_millis)
+                self._rec.adjust_for_ambient_noise(source, duration=duration)
             except UnknownValueError as err:
                 raise IntelligibleAudioError(f"Unable to detect noise => {str(err)}") from err
 
     def _select_device(self) -> Optional[int]:
         """Select device for recording."""
         done = False
-        available: List[str] = list(
-            filter(lambda d: d, map(str.strip, configs.recorder_devices))
-        )
+        available: list[str] = list(filter(lambda d: d, map(str.strip, configs.recorder_devices)))
         while not done:
             if available:
-                for idx, device in self.devices:
-                    if device in available and self._test_device(idx):
+                for idx, device in reversed(self.devices):
+                    if device in available and self.test_device(idx):
                         return idx
             # Choose device from list
             idx_device: Tuple[int, str] = mselect(
                 self.devices, f"{'-=' * 40}%EOL%AskAI::Select the Input device%EOL%{'=-' * 40}%EOL%"
             )
             if not idx_device:
                 break
-            elif self._test_device(idx_device[0]):
+            elif self.test_device(idx_device[0]):
                 available.append(idx_device[1])
                 configs.add_device(idx_device[1])
                 return idx_device[0]
 
             display_text(f"%HOM%%ED2%Error:{idx_device[1]} does not support INPUTS !%NC%")
             self._devices.remove(idx_device)
             pause.seconds(2)
 
         return None
 
-    def _test_device(self, idx: int) -> bool:
-        """Test whether the input device specified by index can be used as an STT input.
-        :param idx: The index of the device to be tested.
-        """
-        log.debug(f"Testing input device at index: %d", idx)
-        try:
-            with Microphone(device_index=idx) as source:
-                self._rec.listen(source, timeout=0.5, phrase_time_limit=0.5)
-                return True
-        except WaitTimeoutError:
-            log.info(f"Device: at index %d is functional!", idx)
-            return True
-        except (AssertionError, AttributeError):
-            log.error(f"Device: at index %d is non functional!", idx)
-
-        return False
-
 
 assert (recorder := Recorder().INSTANCE) is not None
```

### Comparing `hspylib_askai-1.0.6/askai/core/component/summarizer.py` & `hspylib_askai-1.0.7/askai/core/component/summarizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 from askai.core.askai_messages import msg
 from askai.core.component.cache_service import PERSIST_DIR
 from askai.core.model.summary_result import SummaryResult
 from askai.core.support.langchain_support import lc_llm
 from askai.core.support.utilities import hash_text
 from askai.exception.exceptions import DocumentsNotFound
 from functools import lru_cache
+from hspylib.core.config.path_object import PathObject
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.tools.text_tools import ensure_endswith
 from langchain.chains import RetrievalQA
 from langchain_community.document_loaders import DirectoryLoader
 from langchain_community.vectorstores.chroma import Chroma
 from langchain_core.documents import Document
 from langchain_text_splitters import RecursiveCharacterTextSplitter, TextSplitter
 from pathlib import Path
 from typing import List, Optional, Tuple
 
 import logging as log
-import os
 
 
 class Summarizer(metaclass=Singleton):
     """Provide a summarization service to complete queries that require summarization."""
 
     INSTANCE: "Summarizer"
 
@@ -92,15 +92,15 @@
 
     @lru_cache
     def generate(self, folder: str | Path, glob: str) -> bool:
         """Generate a summarization of the folder contents.
         :param folder: The base folder of the summarization.
         :param glob: The glob pattern or file of the summarization.
         """
-        self._folder: str = str(folder).replace("~", os.getenv("HOME")).strip()
+        self._folder = str(PathObject.of(folder))
         self._glob: str = glob.strip()
         AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.summarizing(self.sum_path))
         embeddings = lc_llm.create_embeddings()
 
         try:
             if self.persist_dir.exists():
                 log.info("Recovering vector store from: '%s'", self.persist_dir)
```

### Comparing `hspylib_askai-1.0.6/askai/core/engine/ai_engine.py` & `hspylib_askai-1.0.7/askai/core/engine/ai_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,20 @@
    @created: Fri, 5 May 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
+from typing import Any, List, Optional, Protocol
+
+from langchain_core.language_models import BaseChatModel, BaseLLM
+
 from askai.core.model.ai_model import AIModel
 from askai.core.model.ai_reply import AIReply
-from langchain_core.language_models import BaseChatModel, BaseLLM
-from typing import Any, List, Optional, Protocol
 
 
 class AIEngine(Protocol):
     """Provide an interface for AI engines."""
 
     def lc_model(self, temperature: float, top_p: float) -> BaseLLM:
         """Create a LangChain AI model instance.
@@ -72,7 +74,10 @@
         :param prefix: The prefix of the streamed text.
         """
         ...
 
     def speech_to_text(self) -> Optional[str]:
         """Transcribes audio input from the microphone into the text input language."""
         ...
+
+    def voices(self) -> list[str]:
+        """Return the available model voices for speech to text."""
```

### Comparing `hspylib_askai-1.0.6/askai/core/engine/engine_factory.py` & `hspylib_askai-1.0.7/askai/core/engine/engine_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,23 +9,21 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 
-from typing import List
-
-from hspylib.core.metaclass.singleton import Singleton
-from hspylib.core.preconditions import check_not_none
-
 from askai.core.engine.ai_engine import AIEngine
 from askai.core.engine.openai.openai_engine import OpenAIEngine
 from askai.core.engine.openai.openai_model import OpenAIModel
 from askai.exception.exceptions import NoSuchEngineError
+from hspylib.core.metaclass.singleton import Singleton
+from hspylib.core.preconditions import check_not_none
+from typing import List
 
 
 class EngineFactory(metaclass=Singleton):
     """TODO"""
 
     INSTANCE: "EngineFactory"
```

### Comparing `hspylib_askai-1.0.6/askai/core/engine/openai/openai_configs.py` & `hspylib_askai-1.0.7/askai/core/engine/openai/openai_configs.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,36 +8,37 @@
    @created: Fri, 12 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
+from typing import Literal
+
+from hspylib.core.metaclass.singleton import Singleton
+
 from askai.__classpath__ import classpath
 from askai.core.askai_configs import AskAiConfigs
-from hspylib.core.config.app_config import AppConfigs
-from hspylib.core.metaclass.singleton import Singleton
-from typing import Literal
+from askai.core.askai_settings import settings
 
 
 class OpenAiConfigs(AskAiConfigs, metaclass=Singleton):
     """Provides access to OpenAI configurations."""
 
     INSTANCE: "OpenAiConfigs"
 
     # The resources folder
     RESOURCE_DIR = str(classpath.resource_path())
 
     def __init__(self):
         super().__init__()
-        self._configs = AppConfigs.INSTANCE or AppConfigs(self.RESOURCE_DIR)
-        self._stt_model = self._configs.get("openai.speech-to-text.model")
-        self._tts_model = self._configs.get("openai.text-to-speech.model")
-        self._tts_voice = self._configs.get("openai.text-to-speech.voice")
-        self._tts_format = self._configs.get("openai.text-to-speech.audio.format")
+        self._stt_model = settings.get("openai.speech.to.text.model")
+        self._tts_model = settings.get("openai.text.to.speech.model")
+        self._tts_voice = settings.get("openai.text.to.speech.voice")
+        self._tts_format = settings.get("openai.text.to.speech.audio.format")
 
     @property
     def stt_model(self) -> Literal["whisper-1"]:
         return self._stt_model
 
     @stt_model.setter
     def stt_model(self, value: Literal["whisper-1"]) -> None:
```

### Comparing `hspylib_askai-1.0.6/askai/core/engine/openai/openai_engine.py` & `hspylib_askai-1.0.7/askai/core/engine/openai/openai_engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,33 +9,34 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 
+import logging as log
+import os
+from threading import Thread
+from typing import List, Optional
+
+import langchain_openai
+import pause
+from hspylib.core.preconditions import check_not_none
+from langchain_core.embeddings import Embeddings
+from langchain_core.language_models import BaseChatModel, BaseLLM
+from openai import APIError, OpenAI
+
 from askai.core.component.audio_player import AudioPlayer
 from askai.core.component.cache_service import CacheService
 from askai.core.component.recorder import Recorder
 from askai.core.engine.openai.openai_configs import OpenAiConfigs
 from askai.core.engine.openai.openai_model import OpenAIModel
 from askai.core.model.ai_model import AIModel
 from askai.core.model.ai_reply import AIReply
 from askai.core.support.utilities import stream_text
-from hspylib.core.preconditions import check_not_none
-from langchain_core.embeddings import Embeddings
-from langchain_core.language_models import BaseChatModel, BaseLLM
-from openai import APIError, OpenAI
-from threading import Thread
-from typing import List, Optional
-
-import langchain_openai
-import logging as log
-import os
-import pause
 
 
 class OpenAIEngine:
     """Provide a base class for OpenAI features. Implements the prototype AIEngine."""
 
     def __init__(self, model: AIModel = OpenAIModel.GPT_3_5_TURBO):
         super().__init__()
@@ -51,14 +52,21 @@
     def url(self) -> str:
         return "https://api.openai.com/v1/chat/completions"
 
     @property
     def client(self) -> OpenAI:
         return self._client
 
+    @property
+    def configs(self) -> OpenAiConfigs:
+        return self._configs
+
+    def voices(self) -> list[str]:
+        return ["alloy", "echo", "fable", "onyx", "nova", "shimmer"]
+
     def lc_model(self, temperature: float = 0.0, top_p: float = 0.0) -> BaseLLM:
         """Create a LangChain OpenAI llm model instance."""
         return langchain_openai.OpenAI(openai_api_key=self._api_key, temperature=temperature, top_p=top_p)
 
     def lc_chat_model(self, temperature: float = 0.0) -> BaseChatModel:
         """Create a LangChain OpenAI llm chat model instance."""
         return langchain_openai.ChatOpenAI(openai_api_key=self._api_key, temperature=temperature)
@@ -93,30 +101,32 @@
         :param temperature: The model engine temperature.
         :param top_p: The model engine top_p.
         """
         try:
             check_not_none(chat_context)
             log.debug(f"Generating AI answer")
             response = self.client.chat.completions.create(
-                model=self.ai_model_name(), messages=chat_context, temperature=temperature, top_p=top_p
+                model=self.ai_model_name(), messages=chat_context,
+                temperature=temperature, top_p=top_p
             )
             reply = AIReply(response.choices[0].message.content, True)
             log.debug("Response received from LLM: %s", str(reply))
         except APIError as error:
             body: dict = error.body or {"message": "Message not provided"}
             reply = AIReply(f"%RED%{error.__class__.__name__} => {body['message']}%NC%", False)
 
         return reply
 
     def text_to_speech(self, text: str, prefix: str = "") -> None:
         """Text-T0-Speech the provided text.
         :param text: The text to speech.
         :param prefix: The prefix of the streamed text.
         """
-        speech_file_path, file_exists = CacheService.get_audio_file(text, self._configs.tts_format)
+        speech_file_path, file_exists = CacheService.get_audio_file(
+            text, self._configs.tts_voice, self._configs.tts_format)
         if not file_exists:
             log.debug(f'Audio file "%s" not found in cache. Generating from %s.', self.nickname(), speech_file_path)
             response = self.client.audio.speech.create(
                 input=text,
                 model=self._configs.tts_model,
                 voice=self._configs.tts_voice,
                 response_format=self._configs.tts_format,
@@ -131,10 +141,10 @@
         speak_thread.start()
         pause.seconds(AudioPlayer.INSTANCE.start_delay())
         stream_text(text, prefix)
         speak_thread.join()  # Block until the speech has finished.
 
     def speech_to_text(self) -> Optional[str]:
         """Transcribes audio input from the microphone into the text input language."""
-        _, text = Recorder.INSTANCE.listen(Recorder.RecognitionApi.OPEN_AI, self._configs.language)
+        _, text = Recorder.INSTANCE.listen(language=self._configs.language)
         log.debug(f"Audio transcribed to: {text}")
         return text.strip()
```

### Comparing `hspylib_askai-1.0.6/askai/core/engine/openai/openai_model.py` & `hspylib_askai-1.0.7/askai/core/engine/openai/openai_model.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/engine/openai/temperature.py` & `hspylib_askai-1.0.7/askai/core/engine/openai/temperature.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/features/actions.py` & `hspylib_askai-1.0.7/askai/core/features/actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from askai.core.askai_messages import msg
 from askai.core.features.tools.analysis import check_output
 from askai.core.features.tools.browser import browse
 from askai.core.features.tools.general import display_tool
 from askai.core.features.tools.generation import generate_content
 from askai.core.features.tools.summarization import summarize
 from askai.core.features.tools.terminal import execute_command, list_contents, open_command
+from askai.core.features.tools.vision import image_captioner
 from askai.exception.exceptions import TerminatingQuery
 from clitt.core.tui.line_input.line_input import line_input
 from functools import lru_cache
 from hspylib.core.metaclass.singleton import Singleton
 from langchain_core.tools import BaseTool, StructuredTool
 from textwrap import dedent
 from typing import Any, Callable
@@ -32,15 +33,15 @@
 
 
 class Actions(metaclass=Singleton):
     """This class provides the AskAI available actions."""
 
     INSTANCE: "Actions"
 
-    RESERVED: list[str] = ["invoke", "enlist"]
+    RESERVED: list[str] = ["agent_tools"]
 
     def __init__(self):
         """TODO"""
         self._all = dict(
             filter(
                 lambda pair: pair[0] not in self.RESERVED and not pair[0].startswith("_"),
                 {n: fn for n, fn in inspect.getmembers(self, predicate=inspect.ismethod)}.items(),
@@ -57,18 +58,15 @@
         confirm_msg = msg.access_grant()
         if (resp := line_input(confirm_msg).lower()) not in ("yes", "y"):
             raise ValueError(f"Terminal command execution was not approved '{resp}' !")
         self._approved = True
 
         return self._approved
 
-    def _create_agent_tool(
-        self,
-        fn: Callable,
-    ) -> BaseTool:
+    def _create_agent_tool(self, fn: Callable) -> BaseTool:
         """Create the LangChain agent tool."""
 
         def arun(*args) -> Any:
             raise NotImplementedError("This tool does not support async")
 
         tool = StructuredTool.from_function(
             fn,
@@ -78,57 +76,57 @@
         )
 
         return tool
 
     def browse(self, search_query: str) -> str:
         """
         Name: 'browse'
-        Description: Use this tool to stay updated on the latest news and current events, particularly when you need real-time information quickly. This tool is ideal for acquiring fresh data.
+        Description: Use this tool to browse the internet or to stay informed about the latest news and current events, especially when you require up-to-date information quickly. It is especially effective for accessing the most recent data available online.
         Usage: 'browse(search_query)'
           input `search_query`: The web search query in string format.
         """
         return browse(search_query)
 
     def check_output(self, question: str) -> str:
         """
         Name: 'check_output'
-        Description: Use this tool for analyzing or checking outputs, examining files and folders and lists as well as examining any content.
+        Description: Use this tool to analyze tool outputs, examine file structures, and assess textual content such as reminders and appointments. The use of terminal commands is prohibited.
         Usage: `check_output(question)`
           input `question`: The query about the output.
         """
         return check_output(question)
 
-    def describe_image(self, image_path: str) -> str:
+    def image_captioner(self, image_path: str) -> str:
         """
-        Name: 'describe_image'
-        Description: Use this tool to open and analyze of visual content in a single image file.
-        Usage: describe_image(image_path)
+        Name: 'image_captioner'
+        Description: Use this tool to analyze visual content of a single image file.
+        Usage: image_captioner(image_path)
           input `image_path`: The file path of the image to be analyzed.
         """
-        return str(NotImplementedError("Tool 'describe_image' is not yet implemented !"))
+        return image_captioner(image_path)
 
     def generate_content(self, instructions: str, mime_type: str, path_name: str) -> str:
         """
         Name: 'generate_content'
         Description: This tool is specifically designed for tasks that require generating (creating) content such as, code, text, image, and others.
         Usage: generate_content(instructions, mime_type, path_name)
           input `instructions`: These are the instructions for generating content (not the content itself).
           input `mime_type`: This is the content type (use MIME types).
           input `path_name`: This is the directory path where you want to save the generated content. This parameter is optional and should be included only if you wish to save files directly to your disk. If not specified, the content will not be saved.
         """
         return generate_content(instructions, mime_type, path_name)
 
-    def final_answer(self, answer: list[str] | str) -> str:
+    def display_tool(self, answer: list[str] | str) -> str:
         """
-        Name: 'final_answer'
-        Description: Use this tool as your final tool to provide your final answer. Join all messages to the user together in only one call as you can input a list of texts do be displayed.
+        Name: 'display_tool'
+        Description: Use this tool to provide general conversation responses, to display text or to output your final answer.
         Usage: 'final_answer(text, ...repeat N times)'
           input `texts`: The comma separated list of texts to be displayed.
         """
-        return display_tool(*answer if isinstance(answer, list) else answer)
+        return display_tool(*(answer if isinstance(answer, list) else [answer]))
 
     def list_tool(self, folder: str) -> str:
         """
         Name: 'list_tool'
         Description: This tool is designed for retrieving and displaying the contents of a specified folder. It is useful for quickly assessing the files and subdirectories within any directory.
         Usage: 'list_tool(folder)'
           input `folder`: A string representing the name of the directory whose contents you wish to list.
```

### Comparing `hspylib_askai-1.0.6/askai/core/features/router.py` & `hspylib_askai-1.0.7/askai/core/features/router.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,65 +9,79 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 
-import logging as log
-from types import SimpleNamespace
-from typing import Any, Optional, TypeAlias, Type
-
 from askai.core.askai_configs import configs
 from askai.core.askai_events import AskAiEvents
 from askai.core.askai_messages import msg
 from askai.core.askai_prompt import prompt
 from askai.core.engine.openai.temperature import Temperature
 from askai.core.features.actions import features
 from askai.core.features.tools.analysis import assert_accuracy
 from askai.core.features.tools.general import final_answer
 from askai.core.model.action_plan import ActionPlan
 from askai.core.support.langchain_support import lc_llm
 from askai.core.support.object_mapper import object_mapper
 from askai.core.support.shared_instances import shared
 from askai.exception.exceptions import InaccurateResponse
+from hspylib.core.exception.exceptions import InvalidArgumentError
 from hspylib.core.metaclass.singleton import Singleton
+from hspylib.core.preconditions import check_argument
 from langchain.agents import AgentExecutor, create_structured_chat_agent
 from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder, PromptTemplate
 from retry import retry
+from textwrap import dedent
+from types import SimpleNamespace
+from typing import Any, Optional, Type, TypeAlias
+
+import logging as log
+import PIL
 
 AgentResponse: TypeAlias = dict[str, Any]
 
 
 class Router(metaclass=Singleton):
     """Class to provide a divide and conquer set of actions to fulfill an objective. This is responsible for the
     orchestration and execution of the actions."""
 
     INSTANCE: "Router"
 
-    HUMAN_PROMPT: str = "{input}\n (reminder to respond in a JSON blob no matter what)"
+    HUMAN_PROMPT: str = dedent(
+        """
+    Answer my question in the end.\n(reminder to respond in a JSON blob no matter what)\nQuestion: '{input}'
+    """
+    )
 
     # Allow the router to retry on the errors bellow.
     RETRIABLE_ERRORS: tuple[Type[Exception], ...] = (
-        InaccurateResponse, ValueError, AttributeError
+        InaccurateResponse,
+        ValueError,
+        AttributeError,
+        InvalidArgumentError,
+        PIL.UnidentifiedImageError,
     )
 
     @staticmethod
     def _wrap_answer(question: str, category: str, response: str) -> str:
         """Provide a final answer to the user.
         :param question: The user question.
         :param response: The AI response.
         """
         match category.lower(), configs.is_speak:
-            case "chat", False:
-                return final_answer(question, context=response)
-            case "file system", True:
-                return final_answer(question, persona_prompt='stt', context=response)
-            case _:
-                return response
+            case "general chat" | "image caption", _:
+                response = final_answer(question, context=response)
+            case "file management", True:
+                response = final_answer(question, persona_prompt="stt", context=response)
+            case "technical assistance", _:
+                response = final_answer(question, persona_prompt="stt", context=response)
+
+        return response
 
     def __init__(self):
         self._approved = False
 
     @property
     def router_template(self) -> ChatPromptTemplate:
         """Retrieve the Router Template."""
@@ -97,47 +111,49 @@
             runnable = self.router_template | lc_llm.create_chat_model(Temperature.COLDEST.temp)
             if response := runnable.invoke({"input": query}):
                 log.info("Router::[RESPONSE] Received from AI: \n%s.", str(response))
                 plan: ActionPlan = object_mapper.of_json(response.content, ActionPlan)
                 if not isinstance(plan, ActionPlan):
                     return f"Error: AI responded an invalid JSON object -> {str(plan)}"
                 AskAiEvents.ASKAI_BUS.events.reply.emit(
-                    message=msg.action_plan(f"[{plan.category}] `{plan.reasoning}`"),
-                    verbosity="debug")
+                    message=msg.action_plan(f"[{plan.category}] `{plan.reasoning}`"), verbosity="debug"
+                )
                 output = self._route(query, plan)
             else:
                 output = response
             return output
 
         return _process_wrapper()
 
     def _route(self, query: str, action_plan: ActionPlan) -> str:
         """Route the actions to the proper function invocations.
         :param query: The user query to complete.
         :param action_plan: The action plan to resolve the request.
         """
-        last_response: str = ''
+        last_response: str = ""
         actions: list[SimpleNamespace] = action_plan.plan
+        check_argument(all(isinstance(act, SimpleNamespace) for act in actions), "Invalid action format")
         for action in actions:
-            task = ', '.join([f"{k.title()}: {v}" for k, v in vars(action).items()])
+            task = ", ".join([f"{k.title()}: {v}" for k, v in vars(action).items()])
             AskAiEvents.ASKAI_BUS.events.reply.emit(message=f"> `{task}`", verbosity="debug")
             llm = lc_llm.create_chat_model(Temperature.COLDEST.temp)
             chat_memory = shared.create_chat_memory()
             lc_agent = create_structured_chat_agent(llm, features.agent_tools(), self.agent_template)
             agent = AgentExecutor(
-                agent=lc_agent, tools=features.agent_tools(),
+                agent=lc_agent,
+                tools=features.agent_tools(),
                 max_iteraction=configs.max_router_retries,
                 memory=chat_memory,
                 max_execution_time=configs.max_agent_execution_time_seconds,
                 handle_parsing_errors=True,
                 return_only_outputs=True,
                 early_stopping_method=True,
                 verbose=configs.is_debug,
             )
-            if (response := agent.invoke({"input": task})) and (output := response['output']):
+            if (response := agent.invoke({"input": task})) and (output := response["output"]):
                 log.info("Router::[RESPONSE] Received from AI: \n%s.", output)
                 last_response = output
                 assert_accuracy(action.action, output)
                 continue
             raise InaccurateResponse("AI provided AN EMPTY response")
 
         return self._wrap_answer(query, action_plan.category, msg.translate(last_response))
```

### Comparing `hspylib_askai-1.0.6/askai/core/features/tools/analysis.py` & `hspylib_askai-1.0.7/askai/core/features/tools/analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 def assert_accuracy(question: str, ai_response: str) -> None:
     """Function responsible for asserting that the question was properly answered.
     :param question: The user question.
     :param ai_response: The AI response to be analysed.
     """
-    issues_prompt = PromptTemplate(input_variables=['problems'], template=prompt.read_prompt("assert"))
+    issues_prompt = PromptTemplate(input_variables=["problems"], template=prompt.read_prompt("assert"))
     if ai_response in msg.accurate_responses:
         return
     elif not ai_response:
         problems = issues_prompt.format(problems="AI provided AN <EMPTY> response")
         raise InaccurateResponse(problems)
 
     assert_template = PromptTemplate(input_variables=["response", "input"], template=prompt.read_prompt("ryg-rag"))
@@ -56,45 +56,47 @@
                 problems = issues_prompt.format(problems=RagResponse.strip_code(output))
                 raise InaccurateResponse(problems)
             return
 
     raise InaccurateResponse(f"AI Assistant didn't respond accurately => '{response.content}'")
 
 
-def replace_x_refs(question: str, context: str) -> str:
+def resolve_x_refs(ref_name: str, context: str | None) -> str:
     """Replace all cross references by their actual values.
-    :param question: The original useer question.
+    :param ref_name: The cross-reference or variable name.
     :param context: The context to analyze the references.
     """
-    template = PromptTemplate(
-        input_variables=["history", "question"], template=prompt.read_prompt("x-references")
-    )
-    final_prompt = template.format(history=context, question=question)
-    log.info("X-REFS::[QUESTION] %s => CTX: '%s'", question, context)
-    llm = lc_llm.create_chat_model(Temperature.DATA_ANALYSIS.temp)
-    AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.x_reference(), verbosity="debug")
+    output = ref_name
+    if context or (context := str(shared.context.flat("HISTORY"))):
+        template = PromptTemplate(input_variables=["history", "pathname"], template=prompt.read_prompt("x-references"))
+        final_prompt = template.format(history=context, pathname=ref_name)
+        log.info("X-REFS::[QUESTION] %s => CTX: '%s'", ref_name, context)
+        llm = lc_llm.create_chat_model(Temperature.DATA_ANALYSIS.temp)
+        AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.x_reference(), verbosity="debug")
+
+        if (result := llm.invoke(final_prompt).content.strip()) and shared.UNCERTAIN_ID not in result:
+            output = result
 
-    return llm.invoke(final_prompt).content.strip()
+    return output
 
 
 def check_output(question: str, context: str | None = None) -> str:
     """Handle 'Text analysis', invoking: analyze(question: str). Analyze the context and answer the question.
     :param question: The question about the content to be analyzed.
     :param context: The context of the question.
     """
     output = None
-    if not context:
-        context = str(shared.context.flat("HISTORY"))
-    log.info("Analysis::[QUESTION] '%s'  context=%s", question, context)
-    llm = lc_llm.create_chat_model(Temperature.DATA_ANALYSIS.temp)
-    template = PromptTemplate(input_variables=["context", "question"], template=prompt.read_prompt("analysis"))
-    final_prompt = template.format(context=context, question=question)
-    response: AIMessage = llm.invoke(final_prompt)
-    AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.analysis(response.content), verbosity="debug")
-
-    if response and (output := response.content):
-        shared.context.push("HISTORY", question)
-        shared.context.push("HISTORY", output, "assistant")
-        AskAiEvents.ASKAI_BUS.events.reply.emit(message=output, verbosity="debug")
-        output = text_formatter.ensure_ln(output)
+    if context or (context := str(shared.context.flat("HISTORY"))):
+        log.info("Analysis::[QUESTION] '%s'  context=%s", question, context)
+        llm = lc_llm.create_chat_model(Temperature.DATA_ANALYSIS.temp)
+        template = PromptTemplate(input_variables=["context", "question"], template=prompt.read_prompt("analysis"))
+        final_prompt = template.format(context=context, question=question)
+        response: AIMessage = llm.invoke(final_prompt)
+        AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.analysis(response.content), verbosity="debug")
+
+        if response and (output := response.content):
+            shared.context.push("HISTORY", question)
+            shared.context.push("HISTORY", output, "assistant")
+            AskAiEvents.ASKAI_BUS.events.reply.emit(message=output, verbosity="debug")
+            output = text_formatter.ensure_ln(output)
 
     return output or msg.translate("Sorry, I don't know.")
```

### Comparing `hspylib_askai-1.0.6/askai/core/features/tools/browser.py` & `hspylib_askai-1.0.7/askai/core/features/tools/browser.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/features/tools/general.py` & `hspylib_askai-1.0.7/askai/core/features/tools/general.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/features/tools/generation.py` & `hspylib_askai-1.0.7/askai/core/features/tools/generation.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,45 +16,44 @@
 from askai.core.askai_messages import msg
 from askai.core.askai_prompt import prompt
 from askai.core.component.cache_service import cache
 from askai.core.engine.openai.temperature import Temperature
 from askai.core.support.langchain_support import lc_llm
 from askai.core.support.shared_instances import shared
 from askai.core.support.utilities import extract_codeblock
+from hspylib.core.config.path_object import PathObject
 from hspylib.core.preconditions import check_not_none
 from langchain_core.messages import AIMessage
 from langchain_core.prompts import PromptTemplate
-from os.path import basename, dirname
 from pathlib import Path
 
 import logging as log
-import os
 
 
-def generate_content(description: str, mime_type: str, pathname: str | None) -> str:
+def generate_content(description: str, mime_type: str, path_name: str | None) -> str:
     """Generate content using the AI. It's a general function now, but ican be specialized afterwards.
     :param description: The description to use to generate the content.
     :param mime_type: The content type and format using MIME types.
-    :param pathname: The directory path where you want to save the generated content.
+    :param path_name: The directory path where you want to save the generated content.
     """
-    check_not_none((description, mime_type, pathname))
+    check_not_none((description, mime_type, path_name))
     template = PromptTemplate(input_variables=["mime_type", "input"], template=prompt.read_prompt("generator"))
     final_prompt = template.format(mime_type=mime_type, input=description)
 
-    log.info("GENERATE::[PROMPT] '%s'  Type: '%s'  Path: '%s'", description, mime_type, pathname)
+    log.info("GENERATE::[PROMPT] '%s'  Type: '%s'  Path: '%s'", description, mime_type, path_name)
     llm = lc_llm.create_chat_model(temperature=Temperature.CODE_GENERATION.temp)
     response: AIMessage = llm.invoke(final_prompt)
 
     if response and (output := response.content):
         shared.context.push("HISTORY", output, "assistant")
-        if pathname:
-            base_dir = Path(dirname(pathname.replace("~", os.getenv("HOME"))))
-            filename = basename(pathname)
-            if base_dir.is_dir() and base_dir.exists():
-                with open(f"{base_dir}/{filename}", "w") as f_path_name:
+        if path_name:
+            path_obj = PathObject.of(path_name)
+            base_dir = path_obj.abs_dir
+            if Path(base_dir).exists:
+                with open(path_obj.join(), "w") as f_path_name:
                     _, content = extract_codeblock(output)
                     f_path_name.write(content)
         cache.save_reply(prompt, output)
     else:
         output = msg.translate("Sorry, I don't know.")
 
     return output or msg.translate("Sorry, the prompt produced no content!")
```

### Comparing `hspylib_askai-1.0.6/askai/core/features/tools/summarization.py` & `hspylib_askai-1.0.7/askai/core/features/tools/summarization.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/features/tools/terminal.py` & `hspylib_askai-1.0.7/askai/core/features/tools/terminal.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,74 +11,73 @@
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 
 from askai.core.askai_events import AskAiEvents
 from askai.core.askai_messages import msg
-from askai.core.features.tools.analysis import replace_x_refs
+from askai.core.features.tools.analysis import resolve_x_refs
 from askai.core.support.shared_instances import shared
 from askai.core.support.utilities import extract_path, media_type_of
 from clitt.core.term.terminal import Terminal
 from functools import partial
+from hspylib.core.config.path_object import PathObject
 from hspylib.modules.application.exit_status import ExitStatus
 from os.path import expandvars
-from pathlib import Path
 from shutil import which
 from typing import Tuple
 
 import logging as log
 import os
 
 
 def list_contents(folder: str) -> str:
     """List the contents of a folder.
     :param folder: The folder to list contents from.
     """
-    posix_path = Path(f"{folder.replace('~', os.getenv('HOME'))}")
-    if posix_path.exists() and posix_path.is_dir():
-        status, output = _execute_bash(f"ls -lht {folder} 2>/dev/null | sort -k9,9")
+    path_obj = PathObject.of(folder)
+    if path_obj.exists and path_obj.is_dir:
+        status, output = _execute_bash(f"ls -lLht {folder} 2>/dev/null | sort -k9,9")
         if status:
             if not output:
                 return f"Folder {folder} is empty!"
             return f"Showing the contents of `{folder}`: \n{output}"
 
     return f"Error: Could not list folder '{folder}'!"
 
 
-def open_command(pathname: str) -> str:
+def open_command(path_name: str) -> str:
     """Open the specified path, regardless if it's a file, folder or application.
-    :param pathname: The file path to open.
+    :param path_name: The file path to open.
     """
-    posix_path = Path(f"{pathname.replace('~', os.getenv('HOME'))}")
-
-    if not posix_path.exists():
+    posix_path = PathObject.of(path_name)
+    if not posix_path.exists:
         # Attempt to resolve cross-references
         if history := str(shared.context.flat("HISTORY") or ""):
-            if x_referenced := replace_x_refs(pathname, history):
-                x_referenced = Path(f"{x_referenced.replace('~', os.getenv('HOME'))}")
-                posix_path = x_referenced if x_referenced.exists() else posix_path
+            if x_referenced := resolve_x_refs(path_name, history):
+                x_referenced = PathObject.of(x_referenced)
+                posix_path = str(x_referenced) if x_referenced.exists else posix_path
 
-    if posix_path.exists():
+    if posix_path.exists:
         # find the best app to open the file.
-        pathname: str = str(posix_path)
-        match media_type_of(pathname):
+        path_name: str = str(posix_path)
+        match media_type_of(path_name):
             case ("audio", _) | ("video", _):
-                fn_open = partial(_execute_bash, f"ffplay -v 0 -autoexit {pathname} &>/dev/null")
+                fn_open = partial(_execute_bash, f"ffplay -v 0 -autoexit {path_name} &>/dev/null")
             case ("text", _):
-                fn_open = partial(_execute_bash, f'echo "File \\`{pathname}\\`: \n" && cat {pathname}')
+                fn_open = partial(_execute_bash, f'echo "File \\`{path_name}\\`: \n" && cat {path_name}')
             case _:
-                fn_open = partial(_execute_bash, f"open {pathname} 2>/dev/null")
+                fn_open = partial(_execute_bash, f"open {path_name} 2>/dev/null")
         status, output = fn_open()
         if status:
             if not output:
-                return f"`{pathname}` was successfully opened!"
+                return f"`{path_name}` was successfully opened!"
             return output
 
-    return f"Error: Could not open '{pathname}'!"
+    return f"Error: Could not open '{path_name}'!"
 
 
 def execute_command(shell: str, command: str) -> str:
     """Execute a terminal command using the specified language.
     :param shell: The shell type to be used.
     :param command: The command line to be executed.
     """
```

### Comparing `hspylib_askai-1.0.6/askai/core/model/action_plan.py` & `hspylib_askai-1.0.7/askai/core/model/action_plan.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/model/ai_model.py` & `hspylib_askai-1.0.7/askai/core/model/ai_model.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/model/ai_reply.py` & `hspylib_askai-1.0.7/askai/core/model/ai_reply.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/model/rag_response.py` & `hspylib_askai-1.0.7/askai/core/model/rag_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 
-import re
-
 from hspylib.core.enums.enumeration import Enumeration
 
+import re
+
 
 class RagResponse(Enumeration):
     """TODO"""
 
     # fmt: off
 
     GOOD        = 'Green'
@@ -41,15 +41,15 @@
 
     @property
     def is_good(self) -> bool:
         return self == self.GOOD
 
     @classmethod
     def matches(cls, output: str) -> re.Match:
-        return re.search(cls._re(), output.replace('\n', ' '), re.IGNORECASE)
+        return re.search(cls._re(), output.replace("\n", " "), re.IGNORECASE)
 
     @classmethod
     def _re(cls) -> str:
         return rf"(^{'|'.join(cls.values())})[:,-]\s*(.+)"
 
     @classmethod
     def strip_code(cls, message: str) -> str:
```

### Comparing `hspylib_askai-1.0.6/askai/core/model/search_result.py` & `hspylib_askai-1.0.7/askai/core/model/search_result.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/model/summary_result.py` & `hspylib_askai-1.0.7/askai/core/model/summary_result.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/model/terminal_command.py` & `hspylib_askai-1.0.7/askai/core/model/terminal_command.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,20 +6,18 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 
-from dataclasses import dataclass
 from functools import lru_cache
 from os.path import basename
 from typing import Literal, TypeAlias
 
-import json
 import os
 import platform
 
 SupportedPlatforms: TypeAlias = Literal["linux", "windows", "darwin"] | None
 
 SupportedShells: TypeAlias = Literal["bash", "csh", "dash", "ksh", "tcsh", "zsh", "sh"] | None
 
@@ -35,20 +33,7 @@
     shell = basename(os.getenv("SHELL", "bash")).lower()
     return shell if shell and shell in ["bash", "csh", "dash", "ksh", "tcsh", "zsh", "sh"] else None
 
 
 @lru_cache
 def get_user() -> str:
     return os.getenv("USER", "user")
-
-
-@dataclass
-class TerminalCommand:
-    """Keep track of the executed terminal commands."""
-
-    cmd_line: str
-    cmd_out: str
-    os: SupportedPlatforms = get_os()
-    shell: SupportedShells = get_shell()
-
-    def __str__(self):
-        return json.dumps(self.__dict__, default=lambda obj: obj.__dict__)
```

### Comparing `hspylib_askai-1.0.6/askai/core/support/chat_context.py` & `hspylib_askai-1.0.7/askai/core/support/chat_context.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/support/langchain_support.py` & `hspylib_askai-1.0.7/askai/core/support/langchain_support.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 def load_document(loader_type: Type, url: str | List[str]) -> List[Document]:
     """TODO"""
     return loader_type(url).load()
 
 
 class LangChainSupport(metaclass=Singleton):
-    """TODO"""
+    """Helper class to support the use of langchain framework."""
 
-    INSTANCE: ""
+    INSTANCE: "LangChainSupport"
 
     @staticmethod
     @lru_cache
     def create_model(temperature: float = 0.0, top_p: float = 0.0) -> Any:
         """TODO"""
         check_not_none(shared.engine, "AI Engine was not created yet!")
         return shared.engine.lc_model(temperature, top_p)
```

### Comparing `hspylib_askai-1.0.6/askai/core/support/object_mapper.py` & `hspylib_askai-1.0.7/askai/core/support/object_mapper.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/support/presets.py` & `hspylib_askai-1.0.7/askai/core/support/presets.py`

 * *Files identical despite different names*

### Comparing `hspylib_askai-1.0.6/askai/core/support/shared_instances.py` & `hspylib_askai-1.0.7/askai/core/support/shared_instances.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,44 +9,39 @@
     @author: "<B>H</B>ugo <B>S</B>aporetti <B>J</B>unior")"
       @site: "https://github.com/yorevs/askai")
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 
-from functools import lru_cache
-from typing import Optional
-
+from askai.core.askai_configs import configs
+from askai.core.askai_prompt import prompt
+from askai.core.engine.ai_engine import AIEngine
+from askai.core.engine.engine_factory import EngineFactory
+from askai.core.support.chat_context import ChatContext
+from askai.core.support.utilities import display_text
 from clitt.core.term.terminal import terminal
 from clitt.core.tui.line_input.line_input import line_input
+from functools import lru_cache
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.preconditions import check_state
 from hspylib.modules.cli.keyboard import Keyboard
 from langchain.memory import ConversationBufferWindowMemory
 from langchain.memory.chat_memory import BaseChatMemory
-
-from askai.core.askai_configs import configs
-from askai.core.askai_prompt import prompt
-from askai.core.engine.ai_engine import AIEngine
-from askai.core.engine.engine_factory import EngineFactory
-from askai.core.support.chat_context import ChatContext
-from askai.core.support.utilities import display_text
+from typing import Optional
 
 
 class SharedInstances(metaclass=Singleton):
     """Provides access to shared instances."""
 
     INSTANCE: "SharedInstances"
 
     # This is the uuid used in the prompts to indicate that the AI does not know the answer.
     UNCERTAIN_ID: str = "bde6f44d-c1a0-4b0c-bd74-8278e468e50c"
 
-    # This is the uuid used in the prompts to indicate that the response is negative.
-    NEGATIVE_ID: str = "1b11b759-e50e-44de-b5b2-4879354fd9cf"
-
     def __init__(self) -> None:
         self._engine: AIEngine | None = None
         self._context: ChatContext | None = None
         self._memory: BaseChatMemory | None = None
         self._idiom: str = configs.language.idiom
         self._max_context_size: int = configs.max_context_size
         self._max_iteractions: int = configs.max_iteractions
@@ -101,15 +96,17 @@
             self._context = ChatContext(token_limit, self.max_context_size)
         return self._context
 
     @lru_cache
     def create_chat_memory(self) -> BaseChatMemory:
         """TODO"""
         if self._memory is None:
-            self._memory = ConversationBufferWindowMemory(memory_key="chat_history", k=self.max_context_size, return_messages=True)
+            self._memory = ConversationBufferWindowMemory(
+                memory_key="chat_history", k=self.max_context_size, return_messages=True
+            )
         return self._memory
 
     def input_text(self, input_prompt: str) -> Optional[str]:
         """Prompt for user input.
         :param input_prompt: The prompt to display to the user.
         """
         ret = None
```

### Comparing `hspylib_askai-1.0.6/askai/core/support/text_formatter.py` & `hspylib_askai-1.0.7/askai/core/support/text_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 
+import os
+import re
+from textwrap import dedent
+from typing import Any
+
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.tools.text_tools import ensure_endswith, ensure_startswith
 from hspylib.modules.cli.vt100.vt_code import VtCode
 from hspylib.modules.cli.vt100.vt_color import VtColor
 from rich.console import Console
 from rich.markdown import Markdown
 from rich.text import Text
-from textwrap import dedent
-from typing import Any
-
-import os
-import re
 
 
 class TextFormatter(metaclass=Singleton):
     """TODO"""
 
     INSTANCE: "TextFormatter"
 
@@ -83,9 +83,13 @@
         self.console.print(Markdown(colorized))
 
     def display_text(self, text: str) -> None:
         """TODO"""
         colorized: str = VtColor.colorize(VtCode.decode(self.beautify(text)))
         self.console.print(Text.from_ansi(colorized))
 
+    def cmd_print(self, text: str):
+        """TODO"""
+        self.display_markdown(f"%ORANGE%  Commander%NC%: {text}")
+
 
 assert (text_formatter := TextFormatter().INSTANCE) is not None
```

### Comparing `hspylib_askai-1.0.6/askai/core/support/utilities.py` & `hspylib_askai-1.0.7/askai/core/support/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,7 +179,12 @@
     mimetypes.init()
     mtype, _ = mimetypes.guess_type(basename(pathname))
 
     if mtype is not None:
         return tuple(mtype.split("/"))
 
     return None
+
+
+def seconds(millis: int) -> float:
+    """Return the amount of second from milliseconds."""
+    return millis / 1000
```

### Comparing `hspylib_askai-1.0.6/askai/exception/exceptions.py` & `hspylib_askai-1.0.7/askai/exception/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,9 +67,10 @@
 class ImpossibleQuery(HSBaseException):
     """Raised when tracing or executing an action plan is/was not possible."""
 
 
 class TerminatingQuery(HSBaseException):
     """Raised when received a terminating question."""
 
+
 class InvalidStructuredResponse(HSBaseException):
     """Raised when received an invalid structured response."""
```

### Comparing `hspylib_askai-1.0.6/askai/language/argos_translator.py` & `hspylib_askai-1.0.7/askai/language/argos_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,24 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 
-import logging as log
-import os
-import sys
-from functools import lru_cache
-from typing import Optional
-
 from argostranslate import package, translate
 from argostranslate.translate import ITranslation
-
 from askai.exception.exceptions import TranslationPackageError
 from askai.language.language import Language
+from functools import lru_cache
+from typing import Optional
+
+import logging as log
+import os
+import sys
 
 
 class ArgosTranslator:
     """Provides a multilingual offline translation engine.
     Language packages are downloaded at: ~/.local/share/argos-translate/packages
     """
```

### Comparing `hspylib_askai-1.0.6/askai/language/language.py` & `hspylib_askai-1.0.7/askai/language/language.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior
       @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright (c) 2024, HomeSetup
 """
 
-import re
-from typing import Tuple
-
 from hspylib.core.enums.charset import Charset
 from hspylib.core.enums.enumeration import Enumeration
 from hspylib.core.tools.dict_tools import get_or_default
+from typing import Tuple
+
+import re
 
 
 class Language(Enumeration):
     """Enumeration to wrap all standard languages.
     Ref:. https://docs.oracle.com/cd/E23824_01/html/E26033/glset.html
     """
```

### Comparing `hspylib_askai-1.0.6/hspylib_askai.egg-info/PKG-INFO` & `hspylib_askai-1.0.7/hspylib_askai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-askai
-Version: 1.0.6
+Version: 1.0.7
 Summary: HomeSetup - AskAI
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-askai/
@@ -19,17 +19,17 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Terminals
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: hspylib>=1.12.36
+Requires-Dist: hspylib>=1.12.38
 Requires-Dist: hspylib-clitt>=0.9.122
-Requires-Dist: hspylib-setman>=0.10.34
+Requires-Dist: hspylib-setman>=0.10.35
 Requires-Dist: retry2==0.9.5
 Requires-Dist: pause==0.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: argostranslate==1.9.1
 Requires-Dist: protobuf==4.22.1
 Requires-Dist: torch==2.2.0
 Requires-Dist: stanza==1.1.1
@@ -54,14 +54,15 @@
 Requires-Dist: opentelemetry-api==1.22.0
 Requires-Dist: opentelemetry-sdk==1.22.0
 Requires-Dist: opentelemetry-proto==1.22.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: pytz==2024.1
 Requires-Dist: bs4==0.0.2
 Requires-Dist: fake_useragent==1.5.1
+Requires-Dist: textual==0.58.0
 
 <img src="https://iili.io/J8wvc1n.png" width="64" height="64" align="right" />
 
 # AskAI
 >
 > Unleash the Power of AI in Your Terminal
 
@@ -77,15 +78,15 @@
 
 <img src="https://iili.io/J8wrBSe.png" width="360" height="360" align="right" />
 
 Born from the idea of empowering individuals with disabilities to navigate the digital world effortlessly, AskAI stands as a beacon of accessibility in the realm of computing. It emerges as a revolutionary solution, harnessing the prowess of AI to bridge the gap between users and the terminal interface. With its intuitive design, AskAI welcomes users of all abilities, eliminating the need for extensive familiarity with shells like bash or zsh. Now, individuals with disabilities can effortlessly command their machines, whether it involves listing files and folders, summarizing documents, accessing real-time data, or delving into a myriad of other functions.
 
 At the heart of AskAI lies its innovative integration of Speech-to-Text and Text-to-Speech technologies, offering a seamless experience for both visually and hearing impaired users. Through these cutting-edge features, individuals can interact with their computers using their natural voice, transcending the barriers imposed by traditional input methods. Moreover, AskAI introduces a unique push-to-talk input mechanism, enabling users to issue commands effortlessly, enhancing the fluidity and ease of interaction.
 
-<img src="https://iili.io/J8wiCqQ.png" style="padding-right: 10px" width="238" height="170" align="left" />
+<img src="https://iili.io/J8wiCqQ.png" style="padding-right: 10px" width="270" height="154" align="left" />
 
 Furthermore, AskAI embraces diversity by breaking language barriers, ensuring that no matter the tongue spoken, users can communicate effectively with their systems. Its adaptive language capabilities ensure that commands are understood and executed accurately, regardless of linguistic nuances. By championing inclusivity on all fronts, AskAI redefines the landscape of computing accessibility, empowering individuals with disabilities to navigate the digital realm with confidence and autonomy.
 
 
 > The world speaks many languages. AskAI understands them all.
 
 The see a brief demo about AskAI feature check our asciinema video.
@@ -99,14 +100,16 @@
 - Seamlessly Integrate AI Models (Currently Supporting OpenAI).
 - Activate Speech-to-Text Inputs via Push-to-Talk Keybinding.
 - Control Text-to-Speech Outputs with Adjustable Speed.
 - Enable Assistive Technology for Visually Impaired Terminal Usage.
 - Enjoy a Natural Typewriter Effect Synced with Speaking Text.
 - Automate Offline Language Translations for Enhanced Accessibility.
 - Interactive and Non-Interactive modes.
+- Image captions to provide textual descriptions for visual content.
+- Enhanced accuracy in responses is achieved through the implementation of a Retrieval-Augmented Generation (RAG) system.
 
 ## Installation
 
 ### Requirements
 
 #### Python
 
@@ -120,31 +123,14 @@
   - Ubuntu 16 and higher
   - CentOS 7 and higher
   - Fedora 31 and higher
 
 You may want to install HsPyLib on other OS's and it will probably work, but there are no guarantees that it
 **WILL ACTUALLY WORK**.
 
-#### Python packages
-
-There are some python dependencies, but they will be automatically downloaded when the build runs. The following python packages are required:
-
-- retry
-- pause
-- requests
-- argostranslate
-- soundfile
-- langchain
-- langchain-openai
-- PyAudio
-- SpeechRecognition
-- openai-whisper
-- urllib3
-- openai
-
 #### Applications / Libraries
 
 The following software are required:
 
 - FFMPEG (To allow playing audio and video files from your terminal).
 - PORTAUDIO (To allow microphone recordings).
```

### Comparing `hspylib_askai-1.0.6/hspylib_askai.egg-info/SOURCES.txt` & `hspylib_askai-1.0.7/hspylib_askai.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,26 @@
 askai/core/__init__.py
 askai/core/askai.py
 askai/core/askai_configs.py
 askai/core/askai_events.py
 askai/core/askai_messages.py
 askai/core/askai_prompt.py
 askai/core/askai_settings.py
+askai/core/commander/__init__.py
+askai/core/commander/commander.py
+askai/core/commander/commands/__init__.py
+askai/core/commander/commands/settings_cmd.py
+askai/core/commander/commands/tts_stt_cmd.py
 askai/core/component/__init__.py
 askai/core/component/audio_player.py
 askai/core/component/cache_service.py
 askai/core/component/geo_location.py
 askai/core/component/internet_service.py
 askai/core/component/recorder.py
+askai/core/component/scheduler.py
 askai/core/component/summarizer.py
 askai/core/engine/__init__.py
 askai/core/engine/ai_engine.py
 askai/core/engine/engine_factory.py
 askai/core/engine/openai/__init__.py
 askai/core/engine/openai/openai_configs.py
 askai/core/engine/openai/openai_engine.py
@@ -34,31 +40,36 @@
 askai/core/features/tools/__init__.py
 askai/core/features/tools/analysis.py
 askai/core/features/tools/browser.py
 askai/core/features/tools/general.py
 askai/core/features/tools/generation.py
 askai/core/features/tools/summarization.py
 askai/core/features/tools/terminal.py
+askai/core/features/tools/vision.py
 askai/core/model/__init__.py
 askai/core/model/action_plan.py
 askai/core/model/ai_model.py
 askai/core/model/ai_reply.py
-askai/core/model/query_type.py
 askai/core/model/rag_response.py
 askai/core/model/search_result.py
 askai/core/model/summary_result.py
 askai/core/model/terminal_command.py
 askai/core/support/__init__.py
 askai/core/support/chat_context.py
 askai/core/support/langchain_support.py
 askai/core/support/object_mapper.py
 askai/core/support/presets.py
 askai/core/support/shared_instances.py
 askai/core/support/text_formatter.py
 askai/core/support/utilities.py
+askai/core/tui/__init__.py
+askai/core/tui/app_icons.py
+askai/core/tui/app_widgets.py
+askai/core/tui/askai_app.py
+askai/core/tui/header.py
 askai/exception/__init__.py
 askai/exception/exceptions.py
 askai/language/__init__.py
 askai/language/argos_translator.py
 askai/language/language.py
 hspylib_askai.egg-info/PKG-INFO
 hspylib_askai.egg-info/SOURCES.txt
```

### Comparing `hspylib_askai-1.0.6/hspylib_askai.egg-info/requires.txt` & `hspylib_askai-1.0.7/hspylib_askai.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-hspylib>=1.12.36
+hspylib>=1.12.38
 hspylib-clitt>=0.9.122
-hspylib-setman>=0.10.34
+hspylib-setman>=0.10.35
 retry2==0.9.5
 pause==0.3
 requests==2.31.0
 argostranslate==1.9.1
 protobuf==4.22.1
 torch==2.2.0
 stanza==1.1.1
@@ -29,7 +29,8 @@
 opentelemetry-api==1.22.0
 opentelemetry-sdk==1.22.0
 opentelemetry-proto==1.22.0
 rich==13.7.1
 pytz==2024.1
 bs4==0.0.2
 fake_useragent==1.5.1
+textual==0.58.0
```

### Comparing `hspylib_askai-1.0.6/setup.py` & `hspylib_askai-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 # The package requirements
 REQUIREMENTS = list(filter(None, (HERE / "requirements.txt").read_text().splitlines()))
 
 # This call to setup() does all the work
 setuptools.setup(
     name="hspylib-askai",
-    version="1.0.6",
+    version="1.0.7",
     description="HomeSetup - AskAI",
     author="Hugo Saporetti Junior",
     author_email="yorevs@hotmail.com",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/yorevs/hspylib",
     project_urls={"GitHub": "https://github.com/yorevs/hspylib", "PyPi": "https://pypi.org/project/hspylib-askai/"},
```

