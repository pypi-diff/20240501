# Comparing `tmp/livekit-agents-0.5.dev3.tar.gz` & `tmp/livekit_agents-0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-agents-0.5.dev3.tar", last modified: Thu Apr 11 23:44:21 2024, max compression
+gzip compressed data, was "livekit_agents-0.6.dev0.tar", last modified: Wed May  1 00:22:19 2024, max compression
```

## Comparing `livekit-agents-0.5.dev3.tar` & `livekit_agents-0.6.dev0.tar`

### file list

```diff
@@ -1,68 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:44:21.717491 livekit-agents-0.5.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-11 23:44:21.717491 livekit-agents-0.5.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:44:21.705491 livekit-agents-0.5.dev3/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:44:21.709491 livekit-agents-0.5.dev3/livekit/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:44:21.709491 livekit-agents-0.5.dev3/livekit/agents/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/aio/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/aio/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/aio/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/aio/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/aio/sleep.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/aio/wait_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/apipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:44:21.713491 livekit-agents-0.5.dev3/livekit/agents/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/cli/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/cli/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/cli/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:44:21.713491 livekit-agents-0.5.dev3/livekit/agents/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/codecs/mp3.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/http_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:44:21.713491 livekit-agents-0.5.dev3/livekit/agents/ipc/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/ipc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/ipc/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/ipc/job_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/ipc/job_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/ipc/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/ipc_enc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/job_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/job_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:44:21.713491 livekit-agents-0.5.dev3/livekit/agents/llm/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/llm/function_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/llm/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:44:21.713491 livekit-agents-0.5.dev3/livekit/agents/stt/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/stt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/stt/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/stt/stt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:44:21.713491 livekit-agents-0.5.dev3/livekit/agents/tokenize/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/tokenize/sentence_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:44:21.713491 livekit-agents-0.5.dev3/livekit/agents/tts/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/tts/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/tts/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/vad.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/voice_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)    15451 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/livekit/agents/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:44:21.717491 livekit-agents-0.5.dev3/livekit_agents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-11 23:44:21.000000 livekit-agents-0.5.dev3/livekit_agents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-11 23:44:21.000000 livekit-agents-0.5.dev3/livekit_agents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:44:21.000000 livekit-agents-0.5.dev3/livekit_agents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-11 23:44:21.000000 livekit-agents-0.5.dev3/livekit_agents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 23:44:21.000000 livekit-agents-0.5.dev3/livekit_agents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:44:21.717491 livekit-agents-0.5.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-11 23:44:17.000000 livekit-agents-0.5.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.621821 livekit_agents-0.6.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.625821 livekit_agents-0.6.dev0/livekit/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.629821 livekit_agents-0.6.dev0/livekit/agents/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/aio/wait_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/apipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.629821 livekit_agents-0.6.dev0/livekit/agents/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/cli/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/cli/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/cli/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.629821 livekit_agents-0.6.dev0/livekit/agents/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/codecs/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/http_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.629821 livekit_agents-0.6.dev0/livekit/agents/ipc/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/ipc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/ipc/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/ipc/job_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/ipc/job_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/ipc/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/ipc_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/job_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/job_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.629821 livekit_agents-0.6.dev0/livekit/agents/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/llm/function_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/llm/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.629821 livekit_agents-0.6.dev0/livekit/agents/stt/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/stt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/stt/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/stt/stt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/livekit/agents/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/tokenize/sentence_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/livekit/agents/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/tts/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/tts/tts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/livekit/agents/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/utils/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/utils/exp_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/utils/moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/livekit/agents/voice_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/voice_assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30779 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/voice_assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/voice_assistant/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16319 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/livekit/agents/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/livekit_agents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-01 00:22:19.000000 livekit_agents-0.6.dev0/livekit_agents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-01 00:22:19.000000 livekit_agents-0.6.dev0/livekit_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:22:19.000000 livekit_agents-0.6.dev0/livekit_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-01 00:22:19.000000 livekit_agents-0.6.dev0/livekit_agents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:22:19.000000 livekit_agents-0.6.dev0/livekit_agents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:22:19.633821 livekit_agents-0.6.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-01 00:22:06.000000 livekit_agents-0.6.dev0/setup.py
```

### Comparing `livekit-agents-0.5.dev3/PKG-INFO` & `livekit_agents-0.6.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.5.dev3
+Version: 0.6.dev0
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: click~=8.1.0
-Requires-Dist: livekit~=0.9
+Requires-Dist: livekit~=0.11
 Requires-Dist: livekit-api~=0.4
 Requires-Dist: livekit-protocol~=0.4
 Requires-Dist: protobuf>=3
 Requires-Dist: types-protobuf<5,>=4
 Requires-Dist: python-json-logger~=2.0
 Requires-Dist: attrs~=23.0
 Requires-Dist: watchfiles~=0.21
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/__init__.py` & `livekit_agents-0.6.dev0/livekit/agents/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from . import aio, codecs, ipc, llm, stt, tokenize, tts, utils, vad
+from . import aio, codecs, ipc, llm, stt, tokenize, tts, utils, vad, voice_assistant
 from .apipe import AsyncPipe  # noqa
 from .ipc.protocol import IPC_MESSAGES, Log, StartJobRequest, StartJobResponse  # noqa
 from .job_context import JobContext
 from .job_request import AutoDisconnect, AutoSubscribe, JobRequest
 from .plugin import Plugin
 from .version import __version__
-from .voice_assistant import VoiceAssistant
 from .worker import Worker, WorkerOptions
 
 __all__ = [
     "__version__",
-    "VoiceAssistant",
     "Worker",
     "WorkerOptions",
     "JobRequest",
     "AutoSubscribe",
     "AutoDisconnect",
     "JobContext",
     "Plugin",
@@ -37,8 +35,9 @@
     "stt",
     "vad",
     "utils",
     "tts",
     "aio",
     "tokenize",
     "llm",
+    "voice_assistant",
 ]
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/aio/channel.py` & `livekit_agents-0.6.dev0/livekit/agents/aio/channel.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/aio/debug.py` & `livekit_agents-0.6.dev0/livekit/agents/aio/debug.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/aio/interval.py` & `livekit_agents-0.6.dev0/livekit/agents/aio/interval.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/aio/select.py` & `livekit_agents-0.6.dev0/livekit/agents/aio/select.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,21 +102,19 @@
                 try:
                     v = t.result()
                     self._q.append(
                         __class__.Completed(
                             selected=g.gen, index=ogi, exc=None, value=v
                         )
                     )
-                except StopAsyncIteration:
-                    self._gens.pop(self._gens.index(g))
-                    self._og.pop(ogi)
-
-                    if self._done():
-                        raise StopAsyncIteration
                 except Exception as e:
+                    if isinstance(e, StopAsyncIteration):
+                        self._gens.pop(self._gens.index(g))
+                        self._og.pop(ogi)
+
                     self._q.append(
                         __class__.Completed(
                             selected=g.gen, index=ogi, exc=e, value=None
                         )
                     )
                 finally:
                     g.next_task = None
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/aio/sleep.py` & `livekit_agents-0.6.dev0/livekit/agents/aio/sleep.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/aio/wait_group.py` & `livekit_agents-0.6.dev0/livekit/agents/aio/wait_group.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/apipe.py` & `livekit_agents-0.6.dev0/livekit/agents/apipe.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/cli/cli.py` & `livekit_agents-0.6.dev0/livekit/agents/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,24 +49,32 @@
 
     cli = click.Group()
 
     @cli.command(
         help="Start the worker in production mode. Use a json logger by default."
     )
     @shared_args
-    def start(log_level: str, url: str, api_key: str, api_secret: str) -> None:
+    @click.option(
+        "--drain-timeout",
+        default=60,
+        help="Time in seconds to wait for jobs to finish before shutting down",
+    )
+    def start(
+        log_level: str, url: str, api_key: str, api_secret: str, drain_timeout: int
+    ) -> None:
         opts.ws_url = url or opts.ws_url
         opts.api_key = api_key or opts.api_key
         opts.api_secret = api_secret or opts.api_secret
         args = protocol.CliArgs(
             opts=opts,
             log_level=log_level,
             production=True,
             asyncio_debug=False,
             watch=False,
+            drain_timeout=drain_timeout,
         )
         run_worker(args)
 
     @cli.command(help="Start the worker in development mode")
     @shared_args
     @click.option(
         "--asyncio-debug/--no-asyncio-debug",
@@ -91,14 +99,15 @@
         opts.api_secret = api_secret or opts.api_secret
         args = protocol.CliArgs(
             opts=opts,
             log_level=log_level,
             production=False,
             asyncio_debug=asyncio_debug,
             watch=watch,
+            drain_timeout=0,
         )
 
         if watch:
             from .watcher import WatchServer
 
             setup_logging(log_level, args.production)
 
@@ -138,17 +147,15 @@
 
         for sig in (signal.SIGINT, signal.SIGTERM):
             loop.add_signal_handler(sig, _signal_handler)
     except NotImplementedError:
         # TODO(theomonnom): add_signal_handler is not implemented on win
         pass
 
-    async def _worker_run(
-        worker: Worker,
-    ) -> None:
+    async def _worker_run(worker: Worker) -> None:
         try:
             await worker.run()
         except Exception:
             logger.exception("worker failed")
 
     watch_client = None
     if args.watch:
@@ -161,14 +168,17 @@
 
     main_task = loop.create_task(_worker_run(worker))
     try:
         loop.run_until_complete(main_task)
     except (Shutdown, KeyboardInterrupt):
         pass
 
+    if args.production:
+        loop.run_until_complete(worker.drain(timeout=args.drain_timeout))
+
     loop.run_until_complete(worker.aclose())
 
     if watch_client:
         loop.run_until_complete(watch_client.aclose())
 
     tasks = asyncio.all_tasks(loop)
     for task in tasks:
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/cli/log.py` & `livekit_agents-0.6.dev0/livekit/agents/cli/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,30 +17,31 @@
         return message + extra_txt
 
 
 def setup_logging(log_level: str, production: bool = True) -> None:
     h = logging.StreamHandler()
 
     if production:
-        ## production mode, json logs
+        # production mode, json logs
         from pythonjsonlogger import jsonlogger
 
         class CustomJsonFormatter(jsonlogger.JsonFormatter):
             def add_fields(self, log_record, record, message_dict):
                 super().add_fields(log_record, record, message_dict)
-                if "taskName" in log_record:
-                    log_record.pop("taskName")
                 log_record["level"] = record.levelname
 
         f = CustomJsonFormatter("%(asctime)s %(level)s %(name)s %(message)s")
         h.setFormatter(f)
     else:
-        ## dev mode, colored logs & show all extra
+        # dev mode, colored logs & show all extra
         import colorlog
 
+        watch_logger = logging.getLogger("watchfiles.main")
+        watch_logger.level = logging.WARN
+
         f = ExtraLogFormatter(
             colorlog.ColoredFormatter(
                 "%(asctime)s %(log_color)s%(levelname)-4s %(bold_white)s %(name)s %(reset)s %(message)s",
                 log_colors={
                     **colorlog.default_log_colors,
                     "DEBUG": "blue",
                 },
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/cli/protocol.py` & `livekit_agents-0.6.dev0/livekit/agents/cli/protocol.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 @define(kw_only=True)
 class CliArgs:
     opts: WorkerOptions
     log_level: str
     production: bool
     asyncio_debug: bool
     watch: bool
+    drain_timeout: int
     cch: ipc_enc.ProcessPipe | None = None  # None when watch is disabled
 
 
 @define(kw_only=True)
 class ActiveJobsRequest:
     MSG_ID: ClassVar[int] = 1
 
@@ -34,30 +35,30 @@
 
 @define(kw_only=True)
 class ActiveJobsResponse:
     MSG_ID: ClassVar[int] = 2
     jobs: list[ActiveJob] = Factory(list)
 
     def write(self, b: io.BytesIO) -> None:
-        b.write(len(self.jobs).to_bytes(4))
+        b.write(len(self.jobs).to_bytes(4, "big"))
         for aj in self.jobs:
             job_s = aj.job.SerializeToString()
-            b.write(len(job_s).to_bytes(4))
+            b.write(len(job_s).to_bytes(4, "big"))
             b.write(job_s)
             accept_s = pickle.dumps(aj.accept_data)
-            b.write(len(accept_s).to_bytes(4))
+            b.write(len(accept_s).to_bytes(4, "big"))
             b.write(accept_s)
 
     def read(self, b: io.BytesIO) -> None:
-        job_count = int.from_bytes(b.read(4))
+        job_count = int.from_bytes(b.read(4), "big")
         for _ in range(job_count):
-            job_len = int.from_bytes(b.read(4))
+            job_len = int.from_bytes(b.read(4), "big")
             job = agent.Job()
             job.ParseFromString(b.read(job_len))
-            accept_len = int.from_bytes(b.read(4))
+            accept_len = int.from_bytes(b.read(4), "big")
             accept_data = pickle.loads(b.read(accept_len))
             self.jobs.append(ActiveJob(job=job, accept_data=accept_data))
 
 
 @define(kw_only=True)
 class ReloadJobsRequest:
     MSG_ID: ClassVar[int] = 3
@@ -71,30 +72,30 @@
 
 @define(kw_only=True)
 class ReloadJobsResponse:
     MSG_ID: ClassVar[int] = 4
     jobs: list[ActiveJob] = Factory(list)
 
     def write(self, b: io.BytesIO) -> None:
-        b.write(len(self.jobs).to_bytes(4))
+        b.write(len(self.jobs).to_bytes(4, "big"))
         for aj in self.jobs:
             job_s = aj.job.SerializeToString()
-            b.write(len(job_s).to_bytes(4))
+            b.write(len(job_s).to_bytes(4, "big"))
             b.write(job_s)
             accept_s = pickle.dumps(aj.accept_data)
-            b.write(len(accept_s).to_bytes(4))
+            b.write(len(accept_s).to_bytes(4, "big"))
             b.write(accept_s)
 
     def read(self, b: io.BytesIO) -> None:
-        job_count = int.from_bytes(b.read(4))
+        job_count = int.from_bytes(b.read(4), "big")
         for _ in range(job_count):
-            job_len = int.from_bytes(b.read(4))
+            job_len = int.from_bytes(b.read(4), "big")
             job = agent.Job()
             job.ParseFromString(b.read(job_len))
-            accept_len = int.from_bytes(b.read(4))
+            accept_len = int.from_bytes(b.read(4), "big")
             accept_data = pickle.loads(b.read(accept_len))
             self.jobs.append(ActiveJob(job=job, accept_data=accept_data))
 
 
 @define(kw_only=True)
 class Reloaded:
     MSG_ID: ClassVar[int] = 5
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/cli/watcher.py` & `livekit_agents-0.6.dev0/livekit/agents/cli/watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
             logger.info(f"Watching {p}")
 
         self._read_thread.start()
         watchfiles.run_process(
             *paths,
             target=self._worker_runner,
             args=(self._args,),
+            watch_filter=watchfiles.filters.PythonFilter(),
             callback=self._on_reload,
         )
 
     def _read_loop(self) -> None:
         try:
             active_jobs = []
             while True:
@@ -129,14 +130,15 @@
             while True:
                 msg = await self._apipe.read()
 
                 if isinstance(msg, protocol.ActiveJobsRequest):
                     jobs = self._worker.active_jobs
                     await self.send(protocol.ActiveJobsResponse(jobs=jobs))
                 elif isinstance(msg, protocol.ReloadJobsResponse):
+                    # TODO(theomonnom): This doesn't wait for the worker to be ready/connected
                     self._worker._reload_jobs(msg.jobs)
                     await self.send(protocol.Reloaded())
 
         except Exception:
             logger.exception("watcher failed")
 
     async def send(self, msg: ipc_enc.Message) -> None:
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/codecs/__init__.py` & `livekit_agents-0.6.dev0/livekit/agents/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/codecs/mp3.py` & `livekit_agents-0.6.dev0/livekit/agents/codecs/mp3.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/http_server.py` & `livekit_agents-0.6.dev0/livekit/agents/http_server.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/ipc/job_main.py` & `livekit_agents-0.6.dev0/livekit/agents/ipc/job_main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import logging
-import os
+import traceback
 
 from livekit import rtc
 
 from .. import aio, apipe, ipc_enc
-from ..job_context import JobContext
+from ..job_context import JobContext, _ShutdownInfo
 from ..job_request import AutoSubscribe
+from ..log import logger
 from ..utils import time_ms
 from . import protocol
 
 
 class LogHandler(logging.Handler):
     """Log handler forwarding logs to the worker process"""
 
     def __init__(self, writer: ipc_enc.ProcessPipeWriter) -> None:
         super().__init__(logging.NOTSET)
         self._writer = writer
 
     def emit(self, record: logging.LogRecord) -> None:
         try:
+            try:
+                msg = record.getMessage()
+            except TypeError:
+                msg = record.msg.format(*record.args)
+
+            if record.exc_info:
+                type, value, tb = record.exc_info
+                msg += "\n" + "".join(traceback.format_exception(type, value, tb))
+
             ipc_enc.write_msg(
                 self._writer,
-                protocol.Log(level=record.levelno, message=record.getMessage()),
+                protocol.Log(
+                    level=record.levelno, logger_name=record.name, message=msg
+                ),
             )
         except Exception as e:
-            print(f"failed to write log: {e}")
+            print(f"failed to log {record.filename}:{record.lineno}, exception '{e}'")
 
 
 async def _start(
     pipe: apipe.AsyncPipe, args: protocol.JobMainArgs, room: rtc.Room
 ) -> None:
     close_tx, close_rx = aio.channel()  # used by the JobContext to signal shutdown
 
@@ -42,64 +54,78 @@
     cnt = room.connect(args.url, args.token, options=opts)
     start_req: protocol.StartJobRequest | None = None
     usertask: asyncio.Task | None = None
     shutting_down = False
 
     async def _start_if_valid():
         nonlocal usertask
-        if start_req and room.isconnected():
 
-            def on_track_published(pub: rtc.RemoteTrackPublication, *_):
+        if not start_req or not room.isconnected():
+            return
+
+        if auto_subscribe == AutoSubscribe.SUBSCRIBE_NONE:
+            return
+
+        @room.on("track_published")
+        def on_track_published(
+            pub: rtc.RemoteTrackPublication, participant: rtc.RemoteParticipant
+        ):
+            if (
+                pub.kind == rtc.TrackKind.KIND_AUDIO
+                and auto_subscribe == AutoSubscribe.AUDIO_ONLY
+            ):
+                pub.set_subscribed(True)
+            elif (
+                pub.kind == rtc.TrackKind.KIND_VIDEO
+                and auto_subscribe == AutoSubscribe.VIDEO_ONLY
+            ):
+                pub.set_subscribed(True)
+
+        for participant in room.participants.values():
+            for track_pub in participant.tracks.values():
                 if (
-                    pub.kind == rtc.TrackKind.KIND_AUDIO
+                    track_pub.kind == rtc.TrackKind.KIND_AUDIO
                     and auto_subscribe == AutoSubscribe.AUDIO_ONLY
                 ):
-                    pub.set_subscribed(True)
+                    track_pub.set_subscribed(True)
                 elif (
-                    pub.kind == rtc.TrackKind.KIND_VIDEO
+                    track_pub.kind == rtc.TrackKind.KIND_VIDEO
                     and auto_subscribe == AutoSubscribe.VIDEO_ONLY
                 ):
-                    pub.set_subscribed(True)
+                    track_pub.set_subscribed(True)
 
-            if auto_subscribe != AutoSubscribe.SUBSCRIBE_NONE:
-                room.on("track_published", on_track_published)
+        ctx = JobContext(close_tx, start_req.job, room)
+        usertask = asyncio.create_task(args.accept_data.entry(ctx))
 
-                for participant in room.participants.values():
-                    for track_pub in participant.tracks.values():
-                        if (
-                            track_pub.kind == rtc.TrackKind.KIND_AUDIO
-                            and auto_subscribe == AutoSubscribe.AUDIO_ONLY
-                        ):
-                            track_pub.set_subscribed(True)
-                        elif (
-                            track_pub.kind == rtc.TrackKind.KIND_VIDEO
-                            and auto_subscribe == AutoSubscribe.VIDEO_ONLY
-                        ):
-                            track_pub.set_subscribed(True)
-            # start the job
-            await pipe.write(protocol.StartJobResponse())
-
-            ctx = JobContext(
-                close_tx,
-                start_req.job,
-                room,
-            )
-            usertask = asyncio.create_task(args.accept_data.entry(ctx))
+        def log_exception(t: asyncio.Task) -> None:
+            if not t.cancelled() and t.exception():
+                logger.error(
+                    f"unhandled exception in the job entry {args.accept_data.entry}",
+                    exc_info=t.exception(),
+                )
+
+        usertask.add_done_callback(log_exception)
+        await pipe.write(protocol.StartJobResponse())
+
+    @room.on("disconnected")
+    def on_disconnected():
+        close_tx.send_nowait(_ShutdownInfo(reason="room disconnected"))
 
     async with contextlib.aclosing(aio.select([pipe, cnt, close_rx])) as select:
         while True:
             s = await select()
             if s.selected is cnt:
                 if s.exc:
-                    await pipe.write(protocol.StartJobResponse(exc=s.exc))
+                    error = "".join(traceback.format_exception_only(type(s.exc), s.exc))
+                    await pipe.write(protocol.StartJobResponse(error=error))
                     break  # failed to connect, break and exit the process
                 await _start_if_valid()
 
             if s.selected is close_rx:
-                await pipe.write(protocol.UserExit())
+                await pipe.write(protocol.UserExit(reason=s.value.reason))
                 break
 
             msg = s.result()
             if isinstance(msg, protocol.ShutdownRequest):
                 shutting_down = True
                 break
             if isinstance(msg, protocol.StartJobRequest):
@@ -107,19 +133,20 @@
                 await _start_if_valid()
             if isinstance(msg, protocol.Ping):
                 last_timestamp = msg.timestamp
                 await pipe.write(
                     protocol.Pong(last_timestamp=last_timestamp, timestamp=time_ms())
                 )
 
-    logging.debug("disconnecting from room")
+    logger.debug("disconnecting from room")
     await room.disconnect()
 
-    if usertask is not None:
-        with contextlib.suppress(asyncio.CancelledError):
+    with contextlib.suppress(Exception):
+        # exceptions are already logged inside the done_callback
+        if usertask is not None:
             await usertask  # type: ignore
 
     if shutting_down:
         await pipe.write(protocol.ShutdownResponse())
 
 
 def _run_job(cch: ipc_enc.ProcessPipe, args: protocol.JobMainArgs) -> None:
@@ -128,17 +155,17 @@
     asyncio.set_event_loop(loop)
 
     logging.root.setLevel(logging.NOTSET)
     # logging.root.propagate = False
     logging.root.addHandler(LogHandler(cch))
 
     # current process pid
-    pid = os.getpid()
-    logging.debug(
-        "process started", extra={"job_id": args.job_id, "url": args.url, "pid": pid}
+    logger.debug(
+        "process started",
+        extra={"url": args.url},
     )
 
     pipe = apipe.AsyncPipe(cch, loop, protocol.IPC_MESSAGES)
     loop.slow_callback_duration = 0.02  # 20ms
     aio.debug.hook_slow_callbacks(0.75)
     loop.set_debug(args.asyncio_debug)
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/ipc/job_process.py` & `livekit_agents-0.6.dev0/livekit/agents/ipc/job_process.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import contextlib
-import multiprocessing
+import logging
+import multiprocessing as mp
 import sys
 import threading
 
 from livekit.protocol import agent
 
 from .. import aio, apipe
 from ..job_request import AcceptData
@@ -21,23 +22,21 @@
         url: str,
         token: str,
         accept_data: AcceptData,
         loop: asyncio.AbstractEventLoop | None = None,
     ) -> None:
         self._loop = loop or asyncio.get_event_loop()
         self._job = job
-        pch, cch = multiprocessing.Pipe(duplex=True)
+        pch, cch = mp.Pipe(duplex=True)
         asyncio_debug = self._loop.get_debug()
         args = (
             cch,
             protocol.JobMainArgs(job.id, url, token, accept_data, asyncio_debug),
         )
-        self._process = multiprocessing.Process(
-            target=_run_job, args=args, daemon=True
-        )  # daemon=True to avoid unresponsive process in production
+        self._process = mp.Process(target=_run_job, args=args)
         self._pipe = apipe.AsyncPipe(
             pch, loop=self._loop, messages=protocol.IPC_MESSAGES
         )
         self._close_future = asyncio.Future()
 
     async def run(self) -> None:
         self._process.start()
@@ -83,49 +82,56 @@
                         extra=self.logging_extra(),
                     )
                     break
 
                 if isinstance(res, protocol.StartJobResponse):
                     start_res = res
                 if isinstance(res, protocol.Log):
-                    logger.log(res.level, res.message, extra=self.logging_extra())
+                    logging.getLogger(res.logger_name).log(
+                        res.level, res.message, extra=self.logging_extra()
+                    )
                 if isinstance(res, protocol.Pong):
                     delay = time_ms() - res.timestamp
                     if delay > consts.HIGH_PING_THRESHOLD * 1000:
                         logger.warning(
                             "job is unresponsive",
                             extra={"delay": delay, **self.logging_extra()},
                         )
 
                     with contextlib.suppress(aio.SleepFinished):
                         pong_timeout.reset()
 
                 if isinstance(res, protocol.UserExit) or isinstance(
                     res, protocol.ShutdownResponse
                 ):
-                    logger.info("job exiting", extra=self.logging_extra())
+                    logger.info(
+                        "job exiting",
+                        extra={"exit": res, **self.logging_extra()},
+                    )
                     break
 
+        await self.join()
+        logger.info("job process closed", extra=self.logging_extra())
+
+    async def join(self) -> None:
         def _join_process():
             try:
                 self._process.join()
             except Exception as e:
                 logger.error(
                     "error joining job process",
                     exc_info=e,
                     extra=self.logging_extra(),
                 )
 
             self._loop.call_soon_threadsafe(self._close_future.set_result, None)
 
+        # TODO: Don't use a thread?
         join_t = threading.Thread(target=_join_process, daemon=True)
         join_t.start()
-        await self._close_future
-
-        logger.info("job process closed", extra=self.logging_extra())
 
     def _sig_kill(self) -> None:
         if not self._process.is_alive():
             return
 
         logger.info("killing job process", extra=self.logging_extra())
         if sys.platform == "win32":
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/ipc/protocol.py` & `livekit_agents-0.6.dev0/livekit/agents/ipc/protocol.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import io
-import pickle
 from typing import ClassVar
 
 from attrs import define
 from livekit.protocol import agent
 
+from .. import ipc_enc
 from ..job_request import AcceptData
 
 
 @define
 class JobMainArgs:
     job_id: str
     url: str
@@ -21,88 +21,75 @@
 
 @define(kw_only=True)
 class StartJobRequest:
     MSG_ID: ClassVar[int] = 0
     job: agent.Job = agent.Job()
 
     def write(self, b: io.BytesIO) -> None:
-        job_s = self.job.SerializeToString()
-        b.write(len(job_s).to_bytes(4))
-        b.write(job_s)
+        ipc_enc._write_bytes(b, self.job.SerializeToString())
 
     def read(self, b: io.BytesIO) -> None:
-        job_len = int.from_bytes(b.read(4))
-        self.job = agent.Job()
-        self.job.ParseFromString(b.read(job_len))
+        self.job.ParseFromString(ipc_enc._read_bytes(b))
 
 
 @define(kw_only=True)
 class StartJobResponse:
     MSG_ID: ClassVar[int] = 1
-    exc: BaseException | None = None
+    error: str = ""
 
     def write(self, b: io.BytesIO) -> None:
-        if self.exc is None:
-            b.write(bytes(4))
-        else:
-            exc_s = pickle.dumps(self.exc)
-            b.write(len(exc_s).to_bytes(4))
-            b.write(pickle.dumps(self.exc))
-
-    def read(self, b: io.BytesIO) -> None:
-        exc_len = int.from_bytes(b.read(4))
-        if exc_len == 0:
-            self.exc = None
-        else:
-            self.exc = pickle.loads(b.read(exc_len))
+        ipc_enc._write_string(b, self.error)
+
+    def read(self, b: io.BytesIO) -> None:
+        self.error = ipc_enc._read_string(b)
 
 
 @define(kw_only=True)
 class Log:
     MSG_ID: ClassVar[int] = 2
     level: int = 0  # logging._Level
+    logger_name: str = ""
     message: str = ""
 
     def write(self, b: io.BytesIO) -> None:
-        b.write(self.level.to_bytes(4))
-        message_s = self.message.encode()
-        b.write(len(message_s).to_bytes(4))
-        b.write(message_s)
+        ipc_enc._write_int(b, self.level)
+        ipc_enc._write_string(b, self.logger_name)
+        ipc_enc._write_string(b, self.message)
 
     def read(self, b: io.BytesIO) -> None:
-        self.level = int.from_bytes(b.read(4))
-        message_len = int.from_bytes(b.read(4))
-        self.message = b.read(message_len).decode()
+        self.level = ipc_enc._read_int(b)
+        self.logger_name = ipc_enc._read_string(b)
+        self.message = ipc_enc._read_string(b)
 
 
 @define(kw_only=True)
 class Ping:
     MSG_ID: ClassVar[int] = 3
     timestamp: int = 0
 
     def write(self, b: io.BytesIO) -> None:
-        b.write(self.timestamp.to_bytes(8))
+        b.write(self.timestamp.to_bytes(8, "big"))
 
     def read(self, b: io.BytesIO) -> None:
-        self.timestamp = int.from_bytes(b.read(8))
+        self.timestamp = int.from_bytes(b.read(8), "big")
 
 
 @define(kw_only=True)
 class Pong:
     MSG_ID: ClassVar[int] = 4
     last_timestamp: int = 0
     timestamp: int = 0
 
     def write(self, b: io.BytesIO) -> None:
-        b.write(self.last_timestamp.to_bytes(8))
-        b.write(self.timestamp.to_bytes(8))
+        ipc_enc._write_long(b, self.last_timestamp)
+        ipc_enc._write_long(b, self.timestamp)
 
     def read(self, b: io.BytesIO) -> None:
-        self.last_timestamp = int.from_bytes(b.read(8))
-        self.timestamp = int.from_bytes(b.read(8))
+        self.last_timestamp = ipc_enc._read_long(b)
+        self.timestamp = ipc_enc._read_long(b)
 
 
 @define(kw_only=True)
 class ShutdownRequest:
     MSG_ID: ClassVar[int] = 5
 
     def write(self, b: io.BytesIO) -> None:
@@ -122,20 +109,21 @@
     def read(self, b: io.BytesIO) -> None:
         pass
 
 
 @define(kw_only=True)
 class UserExit:
     MSG_ID: ClassVar[int] = 7
+    reason: str = ""
 
     def write(self, b: io.BytesIO) -> None:
-        pass
+        ipc_enc._write_string(b, self.reason)
 
     def read(self, b: io.BytesIO) -> None:
-        pass
+        self.reason = ipc_enc._read_string(b)
 
 
 IPC_MESSAGES = {
     StartJobRequest.MSG_ID: StartJobRequest,
     StartJobResponse.MSG_ID: StartJobResponse,
     Log.MSG_ID: Log,
     Ping.MSG_ID: Ping,
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/job_context.py` & `livekit_agents-0.6.dev0/livekit/agents/job_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,27 +10,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from attrs import define
 from livekit import rtc
 from livekit.protocol import agent
 
 from . import aio
 
 
+@define(kw_only=True)
+class _ShutdownInfo:
+    reason: str = ""
+
+
 class JobContext:
     """Context for job, it contains the worker, the room, and the participant.
     You should not create these on your own. They are created by the Worker."""
 
     def __init__(
         self,
-        close_tx: aio.ChanSender[None],
+        close_tx: aio.ChanSender[_ShutdownInfo],
         job: agent.Job,
         room: rtc.Room,
         publisher: rtc.RemoteParticipant | None = None,
     ) -> None:
         self._job = job
         self._room = room
         self._publisher = publisher
@@ -52,9 +58,9 @@
     def publisher(self) -> rtc.RemoteParticipant | None:
         return self._publisher
 
     @property
     def agent(self) -> rtc.LocalParticipant:
         return self._room.local_participant
 
-    def shutdown(self) -> None:
-        self._close_tx.close()
+    def shutdown(self, reason: str = "") -> None:
+        self._close_tx.send_nowait(_ShutdownInfo(reason=reason))
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/job_request.py` & `livekit_agents-0.6.dev0/livekit/agents/job_request.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/llm/__init__.py` & `livekit_agents-0.6.dev0/livekit/agents/llm/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     AIFunction,
     FunctionContext,
     TypeInfo,
     ai_callable,
 )
 from .llm import (
     LLM,
+    CalledFunction,
     ChatChunk,
     ChatContext,
     ChatMessage,
     ChatRole,
     Choice,
     ChoiceDelta,
     LLMStream,
@@ -29,8 +30,9 @@
     "ChatChunk",
     "FunctionContext",
     "ai_callable",
     "TypeInfo",
     "AIFncArg",
     "AIFunction",
     "AIFncMetadata",
+    "CalledFunction",
 ]
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/llm/function_context.py` & `livekit_agents-0.6.dev0/livekit/agents/llm/function_context.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/plugin.py` & `livekit_agents-0.6.dev0/livekit/agents/plugin.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/stt/stream_adapter.py` & `livekit_agents-0.6.dev0/livekit/agents/stt/stream_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import logging
 
 from livekit import rtc
-from livekit.agents import stt
 
 from ..log import logger
 from ..utils import AudioBuffer, merge_frames
 from ..vad import VADEventType, VADStream
 from .stt import (
     STT,
     SpeechEvent,
+    SpeechEventType,
     SpeechStream,
 )
 
 
 class StreamAdapter(STT):
     def __init__(
         self,
         stt: STT,
         vad_stream: VADStream,
     ) -> None:
         super().__init__(streaming_supported=True)
         self._vad = vad_stream
         self._stt = stt
 
+    @property
+    def wrapped_stt(self) -> STT:
+        return self._stt
+
     async def recognize(self, *, buffer: AudioBuffer, language: str | None = None):
         return await self._stt.recognize(
             buffer=buffer,
             language=language,
         )
 
     def stream(
@@ -69,25 +73,25 @@
 
         self._main_task.add_done_callback(log_exception)
 
     async def _run(self) -> None:
         try:
             async for event in self._vad:
                 if event.type == VADEventType.START_OF_SPEECH:
-                    start_event = SpeechEvent(type=stt.SpeechEventType.START_OF_SPEECH)
+                    start_event = SpeechEvent(SpeechEventType.START_OF_SPEECH)
                     self._event_queue.put_nowait(start_event)
                 elif event.type == VADEventType.END_OF_SPEECH:
-                    merged_frames = merge_frames(event.speech)
+                    merged_frames = merge_frames(event.frames)
                     event = await self._stt.recognize(
                         buffer=merged_frames, *self._args, **self._kwargs
                     )
                     self._event_queue.put_nowait(event)
 
                     end_event = SpeechEvent(
-                        type=stt.SpeechEventType.END_OF_SPEECH,
+                        type=SpeechEventType.END_OF_SPEECH,
                         alternatives=[event.alternatives[0]],
                     )
                     self._event_queue.put_nowait(end_event)
         except Exception as e:
             logging.exception(f"stream adapter failed: {e}")
         finally:
             self._event_queue.put_nowait(None)
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/stt/stt.py` & `livekit_agents-0.6.dev0/livekit/agents/stt/stt.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/tokenize/sentence_tokenizer.py` & `livekit_agents-0.6.dev0/livekit/agents/tokenize/sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/tts/stream_adapter.py` & `livekit_agents-0.6.dev0/livekit/agents/tts/stream_adapter.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/tts/tts.py` & `livekit_agents-0.6.dev0/livekit/agents/tts/tts.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         """
         Mark the end of the current segment, this is equivalent to calling
         push_text(None)
         """
         self.push_text(None)
 
     @abstractmethod
-    async def aclose(self, wait: bool = True) -> None:
+    async def aclose(self, *, wait: bool = True) -> None:
         """
         Close the stream, if wait is True, it will wait for the TTS to
         finish synthesizing the audio, otherwise it will close ths stream immediately
         """
         pass
 
     @abstractmethod
@@ -61,16 +61,28 @@
         pass
 
     def __aiter__(self) -> "SynthesizeStream":
         return self
 
 
 class TTS(ABC):
-    def __init__(self, *, streaming_supported: bool) -> None:
+    def __init__(
+        self, *, streaming_supported: bool, sample_rate: int, num_channels: int
+    ) -> None:
         self._streaming_supported = streaming_supported
+        self._sample_rate = sample_rate
+        self._num_channels = num_channels
+
+    @property
+    def sample_rate(self) -> int:
+        return self._sample_rate
+
+    @property
+    def num_channels(self) -> int:
+        return self._num_channels
 
     @abstractmethod
     def synthesize(self, text: str) -> AsyncIterable[SynthesizedAudio]:
         raise NotImplementedError("synthesize is not implemented")
 
     def stream(self) -> SynthesizeStream:
         raise NotImplementedError(
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/utils.py` & `livekit_agents-0.6.dev0/livekit/agents/utils/misc.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.5.dev3/livekit/agents/vad.py` & `livekit_agents-0.6.dev0/livekit/agents/vad.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,40 +4,45 @@
 from typing import List
 
 from livekit import rtc
 
 
 class VADEventType(Enum):
     START_OF_SPEECH = 1
-    SPEAKING = 2
+    INFERENCE_DONE = 2
     END_OF_SPEECH = 3
 
 
 @dataclass
 class VADEvent:
     type: VADEventType
     """type of the event"""
     samples_index: int
     """index of the samples of the event (when the event was fired)"""
     duration: float = 0.0
     """duration of the speech in seconds (only for END_SPEAKING event)"""
-    speech: List[rtc.AudioFrame] = field(default_factory=list)
+    frames: List[rtc.AudioFrame] = field(default_factory=list)
     """list of audio frames of the speech"""
+    probability: float = 0.0
+    """smoothed probability of the speech (only for INFERENCE_DONE event)"""
+    raw_inference_prob: float = 0.0
+    """raw probability of the speech (only for INFERENCE_DONE event)"""
+    inference_duration: float = 0.0
+    """duration of the inference in seconds (only for INFERENCE_DONE event)"""
+    speaking: bool = False
+    """whether speech was detected in the frames"""
 
 
 class VAD(ABC):
-    def __init__(self) -> None:
-        pass
-
     @abstractmethod
     def stream(
         self,
         *,
-        min_speaking_duration: float = 0.5,
-        min_silence_duration: float = 0.5,
+        min_speaking_duration: float = 0.16,
+        min_silence_duration: float = 1.3,
         padding_duration: float = 0.1,
         sample_rate: int = 16000,
         max_buffered_speech: float = 45.0,
     ) -> "VADStream":
         """Returns a VADStream that can be used to push audio frames and receive VAD events
         Args:
           min_speaking_duration: minimum duration of speech to trigger a START_SPEAKING event
@@ -51,17 +56,14 @@
 
           max_buffered_speech: max buffered speech in seconds that we keep until the END_SPEAKING event is triggered
               it is unrecommended to use 0.0 as it may cause OOM if the user doesn't stop speaking"""
         pass
 
 
 class VADStream(ABC):
-    def __init__(self) -> None:
-        pass
-
     @abstractmethod
     def push_frame(self, frame: rtc.AudioFrame) -> None:
         pass
 
     @abstractmethod
     async def aclose(self, *, wait: bool = True) -> None:
         pass
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/version.py` & `livekit_agents-0.6.dev0/livekit/agents/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.5.dev3"
+__version__ = "0.6.dev0"
```

### Comparing `livekit-agents-0.5.dev3/livekit/agents/worker.py` & `livekit_agents-0.6.dev0/livekit/agents/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,29 +35,28 @@
 from .version import __version__
 
 JobRequestFnc = Callable[[JobRequest], Coroutine]
 LoadFnc = Callable[[], float]
 
 
 def cpu_load_fnc() -> float:
-    [m1, m5, m15] = [x / psutil.cpu_count() for x in psutil.getloadavg()]
-    return m1
+    return psutil.cpu_percent() / 100
 
 
 @define(kw_only=True)
 class WorkerPermissions:
     can_publish: bool = True
     can_subscribe: bool = True
     can_publish_data: bool = True
     can_update_metadata: bool = True
     hidden: bool = False
 
 
 # NOTE: this object must be pickle-able
-@define(kw_only=True)
+@define
 class WorkerOptions:
     request_fnc: JobRequestFnc
     load_fnc: LoadFnc = cpu_load_fnc
     load_threshold: float = 0.8
     namespace: str = "default"
     permissions: WorkerPermissions = WorkerPermissions()
     worker_type: agent.JobType = agent.JobType.JT_ROOM
@@ -88,14 +87,15 @@
 
         self._opts = opts
         self._loop = loop or asyncio.get_event_loop()
         self._id = "unregistered"
         self._session = None
         self._closed = False
         self._tasks = set()
+        self._draining = False
         self._pending_assignments: dict[str, asyncio.Future[agent.JobAssignment]] = {}
         self._processes = dict[str, tuple[ipc.JobProcess, ActiveJob]]()
         self._close_future = asyncio.Future(loop=self._loop)
 
         self._chan = aio.Chan[agent.WorkerMessage](32, loop=self._loop)
         # We use the same event loop as the worker (so the health checks are more accurate)
         self._http_server = http_server.HttpServer(
@@ -171,14 +171,42 @@
     def id(self) -> str:
         return self._id
 
     @property
     def active_jobs(self) -> list[ActiveJob]:
         return [active_job for (_, active_job) in self._processes.values()]
 
+    async def drain(self, timeout: int | None = None) -> None:
+        if self._draining:
+            return
+
+        logger.info("draining worker", extra={"id": self.id, "timeout": timeout})
+        self._draining = True
+
+        # exit the queue
+        update = agent.UpdateWorkerStatus(
+            status=(agent.WorkerStatus.WS_FULL),
+        )
+        msg = agent.WorkerMessage(update_worker=update)
+        try:
+            self._chan.send_nowait(msg)
+        except aio.ChanClosed:
+            return
+
+        # wait for all jobs to finish with a final timeout
+        async def _join_jobs():
+            for proc, _ in self._processes.values():
+                await proc.join()
+
+        if timeout:
+            with contextlib.suppress(asyncio.TimeoutError):
+                await asyncio.wait_for(_join_jobs(), timeout)
+        else:
+            await _join_jobs()
+
     async def aclose(self) -> None:
         if self._closed:
             return
 
         logger.info("shutting down worker", extra={"id": self.id})
 
         # shutdown processes before closing the connection to the lkserver
@@ -219,15 +247,15 @@
         async def load_monitor_task():
             interval = aio.interval(consts.LOAD_INTERVAL)
             registered = True
             while True:
                 await interval.tick()
                 load = self._opts.load_fnc()
                 is_full = load >= self._opts.load_threshold
-                should_register = not is_full
+                should_register = not is_full and not self._draining
 
                 update = agent.UpdateWorkerStatus(
                     load=load,
                     status=(
                         agent.WorkerStatus.WS_FULL
                         if is_full
                         else agent.WorkerStatus.WS_AVAILABLE
@@ -297,14 +325,15 @@
                     self._handle_assignment(msg.assignment)
 
         await asyncio.gather(send_task(), recv_task(), load_monitor_task())
 
     def _reload_jobs(self, jobs: list[ActiveJob]):
         for aj in jobs:
             logger.info("reloading job", extra={"job": aj.job})
+
             # reloading jobs doesn't work on third-party workers
             # so it is ok to use the ws_url from the local worker
             # (also create a token with the worker api key)
             url = self._opts.ws_url
 
             jwt = (
                 api.AccessToken(self._opts.api_key, self._opts.api_secret)
```

### Comparing `livekit-agents-0.5.dev3/livekit_agents.egg-info/PKG-INFO` & `livekit_agents-0.6.dev0/livekit_agents.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.5.dev3
+Version: 0.6.dev0
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: click~=8.1.0
-Requires-Dist: livekit~=0.9
+Requires-Dist: livekit~=0.11
 Requires-Dist: livekit-api~=0.4
 Requires-Dist: livekit-protocol~=0.4
 Requires-Dist: protobuf>=3
 Requires-Dist: types-protobuf<5,>=4
 Requires-Dist: python-json-logger~=2.0
 Requires-Dist: attrs~=23.0
 Requires-Dist: watchfiles~=0.21
```

### Comparing `livekit-agents-0.5.dev3/livekit_agents.egg-info/SOURCES.txt` & `livekit_agents-0.6.dev0/livekit_agents.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 livekit/agents/http_server.py
 livekit/agents/ipc_enc.py
 livekit/agents/job_context.py
 livekit/agents/job_request.py
 livekit/agents/log.py
 livekit/agents/plugin.py
 livekit/agents/py.typed
-livekit/agents/utils.py
 livekit/agents/vad.py
 livekit/agents/version.py
-livekit/agents/voice_assistant.py
 livekit/agents/worker.py
 livekit/agents/aio/__init__.py
 livekit/agents/aio/channel.py
 livekit/agents/aio/debug.py
 livekit/agents/aio/interval.py
 livekit/agents/aio/select.py
 livekit/agents/aio/sleep.py
@@ -43,12 +41,20 @@
 livekit/agents/stt/stream_adapter.py
 livekit/agents/stt/stt.py
 livekit/agents/tokenize/__init__.py
 livekit/agents/tokenize/sentence_tokenizer.py
 livekit/agents/tts/__init__.py
 livekit/agents/tts/stream_adapter.py
 livekit/agents/tts/tts.py
+livekit/agents/utils/__init__.py
+livekit/agents/utils/event_emitter.py
+livekit/agents/utils/exp_filter.py
+livekit/agents/utils/misc.py
+livekit/agents/utils/moving_average.py
+livekit/agents/voice_assistant/__init__.py
+livekit/agents/voice_assistant/assistant.py
+livekit/agents/voice_assistant/plotter.py
 livekit_agents.egg-info/PKG-INFO
 livekit_agents.egg-info/SOURCES.txt
 livekit_agents.egg-info/dependency_links.txt
 livekit_agents.egg-info/requires.txt
 livekit_agents.egg-info/top_level.txt
```

### Comparing `livekit-agents-0.5.dev3/setup.py` & `livekit_agents-0.6.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit", "agents", "AI"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
         "click~=8.1.0",
-        "livekit~=0.9",
+        "livekit~=0.11",
         "livekit-api~=0.4",
         "livekit-protocol~=0.4",
         "protobuf>=3",
         "types-protobuf>=4,<5",
         "python-json-logger~=2.0",
         "attrs~=23.0",
         "watchfiles~=0.21",
```

