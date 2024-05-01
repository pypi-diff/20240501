# Comparing `tmp/langfun-0.0.2.dev20240429.tar.gz` & `tmp/langfun-0.0.2.dev20240430.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240429.tar", last modified: Mon Apr 29 08:04:33 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240430.tar", last modified: Tue Apr 30 08:03:45 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240429.tar` & `langfun-0.0.2.dev20240430.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:33.229938 langfun-0.0.2.dev20240429/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-29 08:04:33.229938 langfun-0.0.2.dev20240429/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:33.205938 langfun-0.0.2.dev20240429/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:33.213938 langfun-0.0.2.dev20240429/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:33.213938 langfun-0.0.2.dev20240429/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:33.213938 langfun-0.0.2.dev20240429/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:33.217938 langfun-0.0.2.dev20240429/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    60264 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22512 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20052 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:33.217938 langfun-0.0.2.dev20240429/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:33.221938 langfun-0.0.2.dev20240429/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14841 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/llms/openai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:33.221938 langfun-0.0.2.dev20240429/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:33.221938 langfun-0.0.2.dev20240429/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:33.225938 langfun-0.0.2.dev20240429/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:33.225938 langfun-0.0.2.dev20240429/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:33.225938 langfun-0.0.2.dev20240429/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-29 08:04:33.000000 langfun-0.0.2.dev20240429/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-29 08:04:33.000000 langfun-0.0.2.dev20240429/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:04:33.000000 langfun-0.0.2.dev20240429/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-29 08:04:33.000000 langfun-0.0.2.dev20240429/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 08:04:33.000000 langfun-0.0.2.dev20240429/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 08:04:33.229938 langfun-0.0.2.dev20240429/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-29 08:04:14.000000 langfun-0.0.2.dev20240429/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.668526 langfun-0.0.2.dev20240430/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-30 08:03:45.668526 langfun-0.0.2.dev20240430/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.648526 langfun-0.0.2.dev20240430/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.656526 langfun-0.0.2.dev20240430/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.656526 langfun-0.0.2.dev20240430/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.656526 langfun-0.0.2.dev20240430/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.656526 langfun-0.0.2.dev20240430/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68405 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24081 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20052 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.660526 langfun-0.0.2.dev20240430/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.660526 langfun-0.0.2.dev20240430/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/openai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.660526 langfun-0.0.2.dev20240430/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.660526 langfun-0.0.2.dev20240430/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.664526 langfun-0.0.2.dev20240430/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.664526 langfun-0.0.2.dev20240430/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.668526 langfun-0.0.2.dev20240430/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-30 08:03:45.000000 langfun-0.0.2.dev20240430/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-30 08:03:45.000000 langfun-0.0.2.dev20240430/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:03:45.000000 langfun-0.0.2.dev20240430/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-30 08:03:45.000000 langfun-0.0.2.dev20240430/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 08:03:45.000000 langfun-0.0.2.dev20240430/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 08:03:45.668526 langfun-0.0.2.dev20240430/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/setup.py
```

### Comparing `langfun-0.0.2.dev20240429/LICENSE` & `langfun-0.0.2.dev20240430/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/PKG-INFO` & `langfun-0.0.2.dev20240430/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240429
+Version: 0.0.2.dev20240430
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240429/README.md` & `langfun-0.0.2.dev20240430/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/__init__.py` & `langfun-0.0.2.dev20240430/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/__init__.py` & `langfun-0.0.2.dev20240430/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240430/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/component.py` & `langfun-0.0.2.dev20240430/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/component_test.py` & `langfun-0.0.2.dev20240430/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240430/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240430/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/console.py` & `langfun-0.0.2.dev20240430/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/console_test.py` & `langfun-0.0.2.dev20240430/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240430/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240430/langfun/core/eval/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """Base classes for langfun evaluation."""
 
 import abc
 import collections
 import dataclasses
 import functools
 import hashlib
+import html
 import inspect
 import io
 import os
 import re
 import threading
 import time
 from typing import Annotated, Any, Callable, Iterator, Literal, Optional, Sequence, Type, Union
@@ -36,15 +37,16 @@
 
 
 class Evaluable(lf.Component):
   """Base class for evaluation and suite."""
 
   EXPERIMENT_JSON = 'experiment.json'
   RESULT_JSON = 'result.json'
-  FAILURES_JSON = 'failures.json'
+  OOP_FAILURES_JSON = 'oop_failures.json'
+  NON_OOP_FAILURES_JSON = 'non_oop_failures.json'
   INDEX_HTML = 'index.html'
   SUMMARY_HTML = 'summary.html'
 
   root_dir: Annotated[
       str | None,
       (
           'The root directory for all evaluables under an evaluation suite'
@@ -354,15 +356,15 @@
           # Save results for non-leaf nodes.
           lf.concurrent.ProgressBar.update(
               overview_bar,
               postfix='SAVING RESULTS...',
               color='yellow')
 
           for node in self.nonleaf_nodes:
-            node._result = {c.id: c.result for c in node.children}  # pylint: disable=protected-access
+            node._result = {c.id: c.result for c in node.leaf_nodes}  # pylint: disable=protected-access
             if should_save:
               node.save(result=False, report=False)
 
           if should_save and summary:
             lf.concurrent.ProgressBar.update(
                 overview_bar, postfix='FINALIZING SUMMARY...'
             )
@@ -536,21 +538,21 @@
       else:
         text_color = 'black'
 
       s.write(
           f'<div style="color: {text_color}; white-space: pre-wrap;'
           'padding: 10px; border: 1px solid; margin-top: 10px">'
       )
-      s.write(m.get('formatted_text', m.text))
+      s.write(html.escape(m.get('formatted_text', m.text)))
       if m.result is not None:
         s.write(
             '<div style="color: magenta; white-space: pre-wrap;'
             'padding: 10px; border: 1px solid; margin: 10px">'
         )
-        s.write(pg.format(m.result))
+        s.write(html.escape(pg.format(m.result)))
         s.write('</div>')
       if 'usage' in m.metadata:
         s.write(
             '<div style="background-color: #EEEEEE; color: black; '
             'white-space: pre-wrap; padding: 10px; border: 0px solid; '
             'margin: 10px">'
             f'prompt: {m.usage.prompt_tokens} tokens, '
@@ -749,18 +751,20 @@
 
   max_workers: Annotated[
       int, 'Max workers to run the evaluation in parallel.'
   ] = 32
 
   # Constants.
   CACHE_JSON = 'cache.json'
-  FAILURES_HTML = 'failures.html'
+  OOP_FAILURES_HTML = 'oop_failures.html'
+  NON_OOP_FAILURES_HTML = 'non_oop_failures.html'
 
   @functools.cached_property
   def hash(self) -> str:
+    """Returns the semantic-based hash of the evaluation."""
     if self.is_deterministic:
       identity = pg.format(self._identifiers(), compact=True)
     else:
       identity = ' '.join(sorted([c.hash for c in self.children]))
     return hashlib.md5(identity.encode()).hexdigest()[:8]
 
   def _identifiers(self) -> dict[str, Any]:
@@ -801,31 +805,84 @@
     return self._num_completed
 
   @property
   def complete_rate(self) -> float:
     """Returns the complete rate."""
     return self.num_completed / self.num_examples
 
+  #
+  # Properties on failures.
+  #
+
   @property
   def failures(self) -> list[tuple[Any, Exception]]:
     """Returns the failed examples and their errors."""
     return self._failures
 
   @property
   def num_failures(self) -> int:
     """Returns the number of failed examples."""
     return len(self.failures)
 
+  @functools.cached_property
+  def failure_breakdown(self) -> dict[str, int]:
+    """Returns the breakdown of failures."""
+    breakdown = collections.defaultdict(int)
+    for _, error in self.failures:
+      breakdown[_error_key(error)] += 1
+    sorted_items = sorted(breakdown.items(), key=lambda x: x[1], reverse=True)
+    return pg.Dict({x[0]: x[1] for x in sorted_items})
+
   @property
   def failure_rate(self) -> float:
     """Returns the failure rate in range [0, 1]."""
     if self.num_completed == 0:
       return 0.0
     return self.num_failures / self.num_completed
 
+  @functools.cached_property
+  def oop_failures(self) -> list[tuple[Any, lf_structured.MappingError]]:
+    """Returns the OOP failures."""
+    return [item for item in self.failures
+            if isinstance(item[1], lf_structured.MappingError)]
+
+  @property
+  def num_oop_failures(self) -> int:
+    """Returns the number of OOP failures."""
+    return len(self.oop_failures)
+
+  @property
+  def oop_failure_rate(self) -> float:
+    """Returns the OOP failure rate in range [0, 1]."""
+    if self.num_completed == 0:
+      return 0.0
+    return self.num_oop_failures / self.num_completed
+
+  @functools.cached_property
+  def non_oop_failures(self) -> list[tuple[Any, Exception]]:
+    """Returns the OOP failures."""
+    return [item for item in self.failures
+            if not isinstance(item[1], lf_structured.MappingError)]
+
+  @property
+  def num_non_oop_failures(self) -> int:
+    """Returns the number of non-OOP failures."""
+    return len(self.non_oop_failures)
+
+  @property
+  def non_oop_failure_rate(self) -> float:
+    """Returns the non-OOP failure rate in range [0, 1]."""
+    if self.num_completed == 0:
+      return 0.0
+    return self.num_non_oop_failures / self.num_completed
+
+  #
+  # Properties on usage.
+  #
+
   @property
   def has_usage(self) -> bool:
     """Returns True if token usage is enabled."""
     return self._num_usages > 0
 
   @property
   def average_prompt_tokens(self) -> int:
@@ -972,21 +1029,30 @@
     super()._reset()
     self._failures = []
     self._num_completed = 0
 
     self._total_prompt_tokens = 0
     self._total_completion_tokens = 0
     self._num_usages = 0
+    self.__dict__.pop('oop_failures', None)
+    self.__dict__.pop('non_oop_failures', None)
+
+  @property
+  def oop_failures_link(self) -> str | None:
+    """Returns the link to the OOP failures page."""
+    if self.dir is None:
+      return None
+    return self.link(os.path.join(self.dir, Evaluation.OOP_FAILURES_HTML))
 
   @property
-  def failures_link(self) -> str | None:
-    """Returns the link to the failures page."""
+  def non_oop_failures_link(self) -> str | None:
+    """Returns the link to then non-OOP failures page."""
     if self.dir is None:
       return None
-    return self.link(os.path.join(self.dir, Evaluation.FAILURES_HTML))
+    return self.link(os.path.join(self.dir, Evaluation.NON_OOP_FAILURES_HTML))
 
   def _dryrun(
       self,
       *,
       example: Any,
       debug: bool | lf.LMDebugMode,
       verbose: bool,
@@ -1007,31 +1073,42 @@
     if verbose:
       lf.console.write(
           str(example),
           title='INPUT',
           color='green',
       )
 
-    with lf.use_settings(debug=debug):
-      output_message = copy.process(example, **(self.additional_args or {}))
-      if self.schema is None:
-        output = output_message.text
-      else:
-        output = output_message.result
+    error, output_message = None, None
 
-    if verbose:
+    try:
+      with lf.use_settings(debug=debug):
+        output_message = copy.process(example, **(self.additional_args or {}))
+        if self.schema is None:
+          output = output_message.text
+        else:
+          output = output_message.result
+
+      if verbose:
+        lf.console.write('')
+        lf.console.write(
+            str(output),
+            title='OUTPUT',
+            color='blue',
+        )
+    except lf_structured.MappingError as e:
       lf.console.write('')
       lf.console.write(
-          str(output),
-          title='OUTPUT',
-          color='blue',
+          str(e),
+          title='ERROR',
+          color='red',
       )
+      error = e
 
-    copy.audit(example, output_message, None, dryrun=True)
-    result = copy.summarize()
+    copy.audit(example, output_message, error, dryrun=True)
+    result = copy.finalize()
 
     if verbose:
       lf.console.write('')
       lf.console.write(
           str(result),
           title='RESULT',
           color='magenta',
@@ -1083,15 +1160,15 @@
           self.audit(example, message, error)
       finally:
         # Save cache upon completion or interruption.
         if self.dir and self.cache:
           self.cache.save()
 
     # Summarize result.
-    self._result = self.summarize()
+    self._result = self.finalize()
     if verbose:
       lf.console.write(
           str(self.result),
           title=f'RESULT ON {self.id}',
           color='magenta',
       )
 
@@ -1139,45 +1216,44 @@
           returns_message=True,
           **kwargs,
       )
 
   def _status(self, progress: lf.concurrent.Progress) -> dict[str, Any]:
     return {
         'Model': self.lm.model_id,
-        'Succeeded': f'%.{self.report_precision}f%% (%d/%d)' % (
-            progress.success_rate * 100,
+        'Succeeded': '%s (%d/%d)' % (
+            self._format_rate(progress.success_rate),
             progress.succeeded,
             progress.completed,
         ),
-        'Failed': f'%.{self.report_precision}f%% (%d/%d)' % (
-            progress.failure_rate * 100,
+        'Failed': '%s (%d/%d)' % (
+            self._format_rate(progress.failure_rate),
             progress.failed,
             progress.completed,
         ),
     }
 
   def _completion_status(self, run_status: str) -> str:
     assert self.result is not None
     m = self.result.metrics
     return (
-        f'COMPLETED(%s): Successes=%.{self.report_precision}f%% (%d/%d)'
-        f' Failures=%.{self.report_precision}f%% (%d/%d)'
+        'COMPLETED(%s): Successes=%s(%d/%d) Failures=%s (%d/%d)'
         % (
             run_status,
-            (1 - m.failure_rate) * 100,
+            self._format_rate(1 - m.failure_rate),
             m.total - m.failures,
             m.total,
-            m.failure_rate * 100,
+            self._format_rate(m.failure_rate),
             m.failures,
             m.total,
         )
     )
 
-  def summarize(self) -> pg.Dict:
-    """Summarizes the evaluation result."""
+  def finalize(self) -> pg.Dict:
+    """Finalizes the evaluation result."""
     if self.cache:
       cache_stats = dict(
           use_cache=True,
           num_queries=self.cache.stats.num_queries,
           num_hits=self.cache.stats.num_hits,
           num_updates=self.cache.stats.num_updates,
       )
@@ -1206,72 +1282,125 @@
             schema_fn=str(self.schema_fn),
         ),
         cache_stats=cache_stats,
         metrics=pg.Dict(
             total=self.num_completed,
             failures=self.num_failures,
             failure_rate=self.failure_rate,
+            oop_failures=self.num_oop_failures,
+            oop_failure_rate=self.oop_failure_rate,
+            non_oop_failures=self.num_non_oop_failures,
+            non_oop_failure_rate=self.non_oop_failure_rate,
+            failure_breakdown=self.failure_breakdown,
         ),
         usage=usage,
     )
     return result
 
-  def summarize_html(self) -> str:
+  def summary_card(self) -> str:
+    """Returns summary card in HTML."""
     s = io.StringIO()
     definition = _html_repr(self, compact=False, escape=True)
     s.write('<div><table><tr><td>')
     if self.result is None:
       s.write(
           f'<a target="_blank" title="{definition}" '
           f'href="{self.link(self.dir)}">{self.hash}</a>'
           '</td></tr><tr><td>'
           '<span style="color: gray">(IN-PROGRESS...)</span>'
       )
     else:
       s.write(
           f'<a target="_blank" title="{definition}" '
           f'href="{self.index_link}">{self.hash}</a>'
+          f' &nbsp;[<a href="{self.link(self.dir)}">dir</a>]'
           '</td></tr><tr><td>'
       )
-      self._render_metric(s)
+      self._render_summary_metrics(s)
 
       # Summarize average usage.
       if self.result.usage is not None:
-        self._render_usage(s)
+        self._render_summary_usage(s)
 
     s.write('</td></tr></table></div>')
     return s.getvalue()
 
-  def _render_usage(self, s: io.StringIO) -> None:
+  def _render_summary_usage(self, s: io.StringIO) -> None:
     """Renders usage in HTML."""
     usage = self.result.usage
     total = usage.total_prompt_tokens + usage.total_completion_tokens
     s.write(
         '&nbsp;<a title="'
         f'# of usages: {usage.num_usages}&#013;'
         f'total prompt: {usage.total_prompt_tokens}&#013;'
         f'total response: {usage.total_completion_tokens}&#013;'
         f'avg prompt: {usage.average_prompt_tokens}&#013;'
         f'avg response: {usage.average_completion_tokens}'
         f'" style="color:gray">({total} tokens)</a>'
     )
 
-  def _render_metric(self, s: io.StringIO) -> None:
+  def _render_summary_metrics(self, s: io.StringIO) -> None:
     """Renders metrics in HTML."""
     assert self.result is not None
     m = self.result.metrics
+
+    # OOP failures.
+    oop_failure_title = f'OOP failures ({m.oop_failures}/{m.total})'
+    if m.oop_failures:
+      oop_failure_title += '&#013;'
+      for name, count in m.failure_breakdown.items():
+        if name.startswith('MappingError'):
+          oop_failure_title += '&#013;%s: %s (%d/%d)' % (
+              name.removeprefix('MappingError.'),
+              self._format_rate(count / m.total),
+              count,
+              m.total,
+          )
+
+    extra_style = ''
+    if m.oop_failure_rate > 0.1 and m.oop_failures > 3:
+      extra_style = ';font-weight:bold'
     s.write(
-        '<a title="Failures (%d/%d)" href="%s" style="color:red">%s</a>'
+        '<a title="%s" href="%s" style="color:magenta%s">%s</a>'
         % (
-            m.failures,
-            m.total,
-            self.failures_link,
-            f'%.{self.report_precision}f%% ' % (m.failure_rate * 100),
+            oop_failure_title,
+            self.oop_failures_link,
+            extra_style,
+            self._format_rate(m.oop_failure_rate),
         )
     )
+    s.write(' | ')
+
+    # Non-OOP failures.
+    non_oop_failure_title = f'Non-OOP failures ({m.non_oop_failures}/{m.total})'
+    if m.non_oop_failures:
+      non_oop_failure_title += '&#013;'
+      for name, count in m.failure_breakdown.items():
+        if not name.startswith('MappingError'):
+          non_oop_failure_title += '&#013;%s: %s (%d/%d)' % (
+              name,
+              self._format_rate(count / m.total),
+              count,
+              m.total,
+          )
+
+    extra_style = ';font-weight:bold' if m.non_oop_failures > 0 else ''
+    s.write(
+        '<a title="%s" href="%s" style="color:red%s">%s</a>'
+        % (
+            non_oop_failure_title,
+            self.non_oop_failures_link,
+            extra_style,
+            self._format_rate(m.non_oop_failure_rate),
+        )
+    )
+
+  def _format_rate(self, rate: float) -> str:
+    """Formats a rate."""
+    return f'%.{self.report_precision}f%% ' % (rate * 100)
 
   def audit(
       self,
       example: Any,
       message: lf.Message | None,
       error: Exception | None = None,
       dryrun: bool = False,
@@ -1283,15 +1412,21 @@
       message: The entire message returned by the LM, which could be used to
         trace the LM input, response and parsed structure. If error is raised
         before LLM could return a response, None will be its value.
       error: The exception during processing the example.
       dryrun: Whether or not audition takes place during dryrun.
     """
     if error is not None:
-      self._failures.append((example, str(error)))
+      self._failures.append((example, error))
+
+      # Invalid cache of num_oop_failures.
+      self.__dict__.pop('oop_failures', None)
+      self.__dict__.pop('non_oop_failures', None)
+      self.__dict__.pop('failure_breakdown', None)
+
       if isinstance(error, lf_structured.MappingError):
         message = error.lm_response
     else:
       assert message is not None
       output = message.text if self.schema is None else message.result
       self.audit_processed(example, output, message, dryrun=dryrun)
 
@@ -1329,39 +1464,50 @@
           os.path.join(self.dir, Evaluable.INDEX_HTML),
           file_format='txt',
       )
 
       # Save failures.
       pg.save(
           [
-              pg.Dict(
-                  input=input, error=lf.text_formatting.decolored(str(error))
-              )
-              for input, error in self.failures
+              pg.Dict(input=input, error=_format_error(error))
+              for input, error in self.oop_failures
           ],
-          os.path.join(self.dir, Evaluation.FAILURES_JSON),
+          os.path.join(self.dir, Evaluation.OOP_FAILURES_JSON),
       )
       pg.save(
-          self._html([self._render_result, self._render_failures]),
-          os.path.join(self.dir, Evaluation.FAILURES_HTML),
+          self._html([self._render_result, self._render_oop_failures]),
+          os.path.join(self.dir, Evaluation.OOP_FAILURES_HTML),
+          file_format='txt',
+      )
+      pg.save(
+          [
+              pg.Dict(input=input, error=_format_error(error))
+              for input, error in self.non_oop_failures
+          ],
+          os.path.join(self.dir, Evaluation.NON_OOP_FAILURES_JSON),
+      )
+      pg.save(
+          self._html([self._render_result, self._render_non_oop_failures]),
+          os.path.join(self.dir, Evaluation.NON_OOP_FAILURES_HTML),
           file_format='txt',
       )
 
   def _render_result_header(self, s: io.StringIO) -> None:
     s.write(
         '<td>Method</td>'
         '<td>Inputs</td>'
         '<td>Model</td>'
         '<td>Prompt</td>'
         '<td>Schema</td>'
         '<td>Additional Args</td>'
     )
     if self.result.usage is not None:
       s.write('<td>Usage</td>')
-    s.write('<td>Failures</td>')
+    s.write('<td>OOP Failures</td>')
+    s.write('<td>Non-OOP Failures</td>')
 
   def _render_result_row(self, s: io.StringIO) -> None:
     s.write(
         f'<td style="color:{self._method_color}">{self.method}</td>'
         f'<td style="color:darkgray">{_html_repr(self.inputs)}</td>'
         f'<td style="color:#494a5c">{_html_repr(self.lm)}</td>'
     )
@@ -1381,55 +1527,121 @@
     s.write(
         '<td style="color:purple" '
         f'{_html_repr(self.additional_args, compact=False)}</td>'
     )
     # Usage.
     if self.result.usage is not None:
       s.write('<td>')
-      self._render_usage(s)
+      self._render_summary_usage(s)
       s.write('</td>')
 
-    # Failures.
+    # OOP failures.
     s.write(
-        '<td><span style="color:orange">%s</span>%s</td>'
+        '<td><span style="color:magenta">%s</span>%s</td>'
         % (
-            f'%.{self.report_precision}f%%' % (self.failure_rate * 100),
+            self._format_rate(self.oop_failure_rate),
             '<a href="%s">(%d/%d)</a>'
-            % (self.failures_link, self.num_failures, self.num_completed),
+            % (self.oop_failures_link,
+               self.num_oop_failures,
+               self.num_completed),
+        )
+    )
+    # Non-OOP failures.
+    s.write(
+        '<td><span style="color:red">%s</span>%s</td>'
+        % (
+            self._format_rate(self.non_oop_failure_rate),
+            '<a href="%s">(%d/%d)</a>'
+            % (self.non_oop_failures_link,
+               self.num_non_oop_failures,
+               self.num_completed),
         )
     )
 
   @property
   def _method_color(self) -> str:
     """Returns the color for rendering method."""
     if self.method == 'call':
       return 'gray'
     elif self.method == 'query':
       return 'blue'
     else:
       return 'cyan'
 
-  def _render_failures(self, s: io.StringIO) -> None:
+  def _render_oop_failures(self, s: io.StringIO) -> None:
+    self._render_failures(s, '^MappingError.*', error_color='magenta')
+
+  def _render_non_oop_failures(self, s: io.StringIO) -> None:
+    self._render_failures(s, '^(?!MappingError).*', error_color='red')
+
+  def _render_failures(
+      self, s: io.StringIO, error_regex: str, error_color: str) -> None:
     """Formats the failed cases into html."""
+    # Failure summary.
     s.write(
-        '<h2> Failed Cases </h2>'
+        '<h2> Error Summary </h2>'
         '<div style="white-space:pre">\n'
         '<table style="border:1px solid">'
-        '<tr class="header"><td>No.</td><td>Input</td><td>Error</td></tr>'
+        '<tr class="header"><td>Error type</td><td>Stats</td></tr>'
+    )
+    error_regex = re.compile(error_regex)
+    if self.result.metrics.failure_breakdown:
+      for name, count in self.result.metrics.failure_breakdown.items():
+        if not error_regex.match(name):
+          continue
+
+        link = f'<a href="#{name}">{name}</a>'
+        error_rate = self._format_rate(count / self.result.metrics.total)
+        stats = (f'<span style="color:{error_color}">{error_rate} '
+                 f'({count}/{self.result.metrics.total})</span>')
+        s.write(f'<tr><td>{link}</td><td>{stats})</td></tr>')
+    s.write(
+        '</table></div>'
+        '<h2> Failed Cases </h2>'
+        '<div style="white-space:pre">'
     )
+    # Failure details by error type.
+    failures_by_error = collections.defaultdict(list)
+    for example, error in self.failures:
+      error_name = _error_key(error)
+      if error_regex.match(error_name):
+        failures_by_error[error_name].append((example, error))
 
-    for i, (example, error) in enumerate(self.failures):
-      bgcolor = 'white' if i % 2 == 0 else '#DDDDDD'
-      s.write(f'<tr style="background-color: {bgcolor}"><td>{i + 1}</td>')
-      input_str = pg.format(example, verbose=False)
-      s.write(f'<td style="color:green;white-space:pre-wrap">{input_str}</td>')
-      error_str = lf.text_formatting.decolored(str(error))
-      s.write(f'<td style="color:red;white-space:pre">{error_str}</td>')
-      s.write('</tr>')
-    s.write('</table></div>')
+    for error_key, failures in failures_by_error.items():
+      s.write(
+          f'<h3 id="{error_key}"><a href="#{error_key}">{error_key}</a> '
+          f'(count={len(failures)})</h3>'
+          '<table style="border:1px solid">'
+          '<tr class="header"><td>No.</td><td>Input</td>'
+          '<td>LM invocation</td><td>Error</td></tr>'
+      )
+      for i, (example, error) in enumerate(failures):
+        lm_response = None
+        if isinstance(error, lf.structured.MappingError):
+          lm_response = error.lm_response
+          error = error.cause
+
+        bgcolor = 'white' if i % 2 == 0 else '#DDDDDD'
+        s.write(f'<tr style="background-color: {bgcolor}"><td>{i + 1}</td>')
+        s.write('<td style="color:green;white-space:pre-wrap">')
+        s.write(pg.format(example, verbose=False))
+        s.write('</td><td>')
+        if lm_response is not None:
+          self._render_message(lm_response, s)
+        s.write(f'</td><td style="color:{error_color};white-space:pre">')
+        s.write(_format_error(error))
+        s.write('</td></tr>')
+      s.write('</table>')
+    s.write('</div>')
+
+  @classmethod
+  def visualize(cls, evaluations: list['Evaluation']) -> str | None:
+    """Visualize the a list of evaluations of this task in HTML."""
+    del evaluations
+    return None
 
 
 @pg.functor()
 def inputs_from(path: str | list[str]) -> list[Any]:
   """A functor that returns a list of user-defined objects as eval inputs."""
   if isinstance(path, str):
     return pg.load(path)
@@ -1574,15 +1786,15 @@
           s.write(f'<td style="padding: 5px">{_html_repr(v)}</td>')
 
         for e in row.data:
           s.write('<td style="padding: 5px;">')
           if e is None:
             s.write('<span style="color: gray">N/A<span>')
           else:
-            s.write(e.summarize_html())
+            s.write(e.summary_card())
           s.write('</td>')
         s.write('</tr>')
       s.write('</table>')
       return s.getvalue()
 
     def _repr_html_(self) -> str:
       return self.html()
@@ -1649,21 +1861,30 @@
   def html(self, pivot_field: str | None = None) -> str:
     """Renders the summary in HTML."""
     pivot_field = pivot_field or self.pivot_field
     s = io.StringIO()
     s.write('<html><body>')
     for task in sorted(self.tasks(), key=lambda cls: cls.__name__):
       table_id = task.__name__.lower()
+      evaluations = self.select(task=task).evaluations
+      table = Summary.Table.from_evaluations(evaluations, pivot_field)
       s.write('<div>')
-      s.write(f'<a id="{table_id}"')
-      s.write(f'<h2><a href="#{table_id}">{task.__name__}</a></h2>')
-      s.write('</a>')
-      table = Summary.Table.from_evaluations(
-          self.select(task=task).evaluations, pivot_field
+      s.write(
+          f'<a id="{table_id}" href="#{table_id}">'
+          f'<h2>{task.__name__}</h2></a>'
       )
+
+      # Allow users to plugin visualization code (e.g. matplot) in the summary
+      # page.
+      visual_part = task.visualize(evaluations)
+      if visual_part:
+        s.write(visual_part)
+
+      s.write(f'<h4 style="color:gray">{len(evaluations)} experiments</h4>')
+      s.write('<hr/>')
       s.write(table.html())
       s.write('</div>')
     s.write('</body></html>')
     return s.getvalue()
 
   def _repr_html_(self) -> str:
     return self.html()
@@ -1681,14 +1902,15 @@
       for entry in self.select(task=task).evaluations:
         results.append(
             pg.Dict(
                 id=entry.id,
                 experiment=entry,
                 dir=entry.dir,
                 metrics=entry.result.metrics if entry.result else None,
+                usage=entry.result.usage if entry.result else None,
             )
         )
       task_results[task.__name__] = results
     return task_results
 
   def save(self, file: str, pivot_field: str | None = None) -> None:
     pg.save(self.html(pivot_field), file, file_format='txt')
@@ -1829,14 +2051,29 @@
         filter,
         pivot_field=pivot_field,
         expect_new_dirs=expect_new_dirs,
     )
     return result.join()
 
 
+def _format_error(error: Exception):
+  """Formats an error into a string."""
+  return (f'({error.__class__.__name__}) '
+          + lf.text_formatting.decolored(str(error)))
+
+
+def _error_key(error: Exception) -> str:
+  """Returns the key for an error."""
+  error_names = []
+  while error is not None:
+    error_names.append(error.__class__.__name__)
+    error = getattr(error, 'cause', None)
+  return '.'.join(error_names)
+
+
 def _html_repr(value: Any, compact: bool = True, escape: bool = False) -> str:
   """Formats prompt in HTML."""
   if type(value) is lf.Template:  # pylint: disable=unidiomatic-typecheck
     return repr(value.template_str)
   s = pg.format(
       value, compact=compact, verbose=False, hide_default_values=True)
   if escape:
```

### Comparing `langfun-0.0.2.dev20240429/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240430/langfun/core/eval/base_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -216,15 +216,26 @@
                 prompt_template='{{example.question}}',
                 method='query',
                 schema_fn='answer_schema()',
             ),
             cache_stats=dict(
                 use_cache=True, num_queries=2, num_hits=0, num_updates=2
             ),
-            metrics=dict(total=2, failures=1, failure_rate=0.5),
+            metrics=dict(
+                total=2,
+                failures=1,
+                failure_rate=0.5,
+                oop_failures=1,
+                oop_failure_rate=0.5,
+                non_oop_failures=0,
+                non_oop_failure_rate=0.0,
+                failure_breakdown={
+                    'MappingError.SchemaError.TypeError': 1
+                }
+            ),
             usage=dict(
                 total_prompt_tokens=774,
                 total_completion_tokens=25,
                 num_usages=2,
                 average_prompt_tokens=387,
                 average_completion_tokens=12,
                 average_total_tokens=399,
@@ -232,19 +243,27 @@
         ),
     )
     self.assertTrue(
         os.path.exists(os.path.join(s.dir, base.Evaluation.EXPERIMENT_JSON)))
     self.assertTrue(
         os.path.exists(os.path.join(s.dir, base.Evaluation.RESULT_JSON)))
     self.assertTrue(
+        os.path.exists(os.path.join(s.dir, base.Evaluation.OOP_FAILURES_JSON)))
+    self.assertTrue(
+        os.path.exists(
+            os.path.join(s.dir, base.Evaluation.NON_OOP_FAILURES_JSON)))
+    self.assertTrue(
         os.path.exists(os.path.join(s.dir, base.Evaluation.CACHE_JSON)))
     self.assertTrue(
         os.path.exists(os.path.join(s.dir, base.Evaluation.INDEX_HTML)))
     self.assertTrue(
-        os.path.exists(os.path.join(s.dir, base.Evaluation.FAILURES_HTML)))
+        os.path.exists(os.path.join(s.dir, base.Evaluation.OOP_FAILURES_HTML)))
+    self.assertTrue(
+        os.path.exists(
+            os.path.join(s.dir, base.Evaluation.NON_OOP_FAILURES_HTML)))
     self.assertTrue(
         os.path.exists(os.path.join(s.root_dir, base.Evaluation.SUMMARY_HTML))
     )
     # Check summary JSON.
     summary_json = os.path.join(
         s.root_dir, base.Evaluation.SUMMARY_HTML.replace('.html', '.json')
     )
@@ -270,15 +289,18 @@
     self.assertFalse(
         os.path.exists(os.path.join(s.dir, base.Evaluation.EXPERIMENT_JSON)))
     self.assertFalse(
         os.path.exists(os.path.join(s.dir, base.Evaluation.RESULT_JSON)))
     self.assertFalse(
         os.path.exists(os.path.join(s.dir, base.Evaluation.INDEX_HTML)))
     self.assertFalse(
-        os.path.exists(os.path.join(s.dir, base.Evaluation.FAILURES_HTML)))
+        os.path.exists(os.path.join(s.dir, base.Evaluation.OOP_FAILURES_HTML)))
+    self.assertFalse(
+        os.path.exists(
+            os.path.join(s.dir, base.Evaluation.NON_OOP_FAILURES_HTML)))
 
   def test_load(self):
     lm = fake.StaticResponse('Solution(final_answer=2)')
     s = eval_set('loas_test', 'query', schema_fn=answer_schema(), lm=lm)
     s.run(dryrun=True)
     self.assertIsNotNone(s.result)
 
@@ -308,15 +330,24 @@
                     prompt_template='{{example.question}}',
                     method='query',
                     schema_fn='answer_schema()',
                 ),
                 cache_stats=dict(
                     use_cache=True, num_queries=2, num_hits=0, num_updates=2
                 ),
-                metrics=dict(total=2, failures=0, failure_rate=0.0),
+                metrics=dict(
+                    total=2,
+                    failures=0,
+                    failure_rate=0.0,
+                    oop_failures=0,
+                    oop_failure_rate=0.0,
+                    non_oop_failures=0,
+                    non_oop_failure_rate=0.0,
+                    failure_breakdown={},
+                ),
                 usage=s.children[1].result.usage,
             ),
         },
     )
 
   def test_search_space(self):
     lm = fake.StaticSequence([
@@ -359,30 +390,52 @@
                     prompt_template='{{example.question}}',
                     method='query',
                     schema_fn='answer_schema()',
                 ),
                 cache_stats=dict(
                     use_cache=True, num_queries=2, num_hits=0, num_updates=2
                 ),
-                metrics=dict(total=2, failures=1, failure_rate=0.5),
+                metrics=dict(
+                    total=2,
+                    failures=1,
+                    failure_rate=0.5,
+                    oop_failures=1,
+                    oop_failure_rate=0.5,
+                    non_oop_failures=0,
+                    non_oop_failure_rate=0.0,
+                    failure_breakdown={
+                        'MappingError.SchemaError.TypeError': 1
+                    }
+                ),
                 usage=s.children[0].result.usage,
             ),
             s.children[1].id: dict(
                 experiment_setup=dict(
                     id=s.children[1].id,
                     dir=s.children[1].dir,
                     model='StaticSequence',
                     prompt_template='Hello {{example.question}}',
                     method='query',
                     schema_fn='answer_schema()',
                 ),
                 cache_stats=dict(
                     use_cache=True, num_queries=2, num_hits=0, num_updates=2
                 ),
-                metrics=dict(total=2, failures=1, failure_rate=0.5),
+                metrics=dict(
+                    total=2,
+                    failures=1,
+                    failure_rate=0.5,
+                    oop_failures=1,
+                    oop_failure_rate=0.5,
+                    non_oop_failures=0,
+                    non_oop_failure_rate=0.0,
+                    failure_breakdown={
+                        'MappingError.SchemaError.TypeError': 1
+                    }
+                ),
                 usage=s.children[1].result.usage,
             ),
         },
     )
 
   def test_call(self):
     lm = fake.StaticSequence(['two'])
@@ -471,68 +524,66 @@
         ],
         lm=lm
     )
     # Test for persistent hash.
     self.assertEqual(s.hash, '26e6cc25')
     s.run()
     expected = {
-        s.children[0].id: dict(
+        'Evaluation@0fade07d': dict(
             experiment_setup=dict(
                 id=s.children[0].id,
                 dir=s.children[0].dir,
                 model='StaticSequence',
                 prompt_template='{{example.question}}',
                 method='query',
                 schema_fn='answer_schema()',
             ),
             cache_stats=dict(
                 use_cache=True, num_queries=2, num_hits=0, num_updates=2
             ),
-            metrics=dict(total=2, failures=1, failure_rate=0.5),
+            metrics=dict(
+                total=2,
+                failures=1,
+                failure_rate=0.5,
+                oop_failures=1,
+                oop_failure_rate=0.5,
+                non_oop_failures=0,
+                non_oop_failure_rate=0.0,
+                failure_breakdown={
+                    'MappingError.SchemaError.TypeError': 1
+                }
+            ),
             usage=s.children[0].result.usage,
         ),
-        s.children[1].id: {
-            s.children[1]
-            .children[0]
-            .id: dict(
-                experiment_setup=dict(
-                    id=s.children[1].children[0].id,
-                    dir=s.children[1].children[0].dir,
-                    model='StaticSequence',
-                    prompt_template='{{example.question}}',
-                    method='call',
-                    schema_fn='answer_schema()',
-                ),
-                cache_stats=dict(
-                    use_cache=True, num_queries=4, num_hits=1, num_updates=3
-                ),
-                metrics=dict(total=2, failures=2, failure_rate=1.0),
-                usage=s.children[1].children[0].result.usage,
+        'Evaluation@ae86c703': dict(
+            experiment_setup=dict(
+                id=s.children[1].children[0].id,
+                dir=s.children[1].children[0].dir,
+                model='StaticSequence',
+                prompt_template='{{example.question}}',
+                method='call',
+                schema_fn='answer_schema()',
             ),
-            s.children[1]
-            .children[2]
-            .id: dict(
-                experiment_setup=dict(
-                    id=s.children[1].children[2].id,
-                    dir=s.children[1].children[2].dir,
-                    model='StaticSequence',
-                    prompt_template='{{example.question}}',
-                    method='query',
-                    schema_fn='answer_schema()',
-                ),
-                cache_stats=dict(
-                    use_cache=True,
-                    num_queries=2,
-                    num_hits=0,
-                    num_updates=2,
-                ),
-                metrics=dict(total=2, failures=1, failure_rate=0.5),
-                usage=s.children[1].children[2].result.usage,
+            cache_stats=dict(
+                use_cache=True, num_queries=4, num_hits=1, num_updates=3
             ),
-        },
+            metrics=dict(
+                total=2,
+                failures=2,
+                failure_rate=1.0,
+                oop_failures=2,
+                oop_failure_rate=1.0,
+                non_oop_failures=0,
+                non_oop_failure_rate=0.0,
+                failure_breakdown={
+                    'MappingError.SchemaError.TypeError': 2
+                }
+            ),
+            usage=s.children[1].children[0].result.usage,
+        ),
     }
     self.assertEqual(s.result, expected)
 
 
 class InputsFrom(unittest.TestCase):
   """Tests for inputs_from."""
```

### Comparing `langfun-0.0.2.dev20240429/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240430/langfun/core/eval/matching.py`

 * *Files 10% similar despite different names*

```diff
@@ -115,53 +115,54 @@
     """Matches answer against the groundtruth. Subclasses can override."""
     return pg.eq(answer, groundtruth)
 
   def _status(self, progress: lf.concurrent.Progress) -> dict[str, Any]:
     del progress
     return {
         'Model': self.lm.model_id,
-        'Matches': f'%.{self.report_precision}f%% (%d/%d)' % (
-            self.match_rate * 100,
+        'Matches': '%s (%d/%d)' % (
+            self._format_rate(self.match_rate),
             self.num_matches,
             self.num_completed,
         ),
-        'Mismatches': f'%.{self.report_precision}f%% (%d/%d)' % (
-            self.mismatch_rate * 100,
+        'Mismatches': '%s (%d/%d)' % (
+            self._format_rate(self.mismatch_rate),
             self.num_mismatches,
             self.num_completed,
         ),
-        'Failed': f'%.{self.report_precision}f%% (%d/%d)' % (
-            self.failure_rate * 100,
+        'Failed': '%s (%d/%d)' % (
+            self._format_rate(self.failure_rate),
             self.num_failures,
             self.num_completed,
         ),
     }
 
   def _completion_status(self, run_status: str) -> str:
     assert self.result is not None
     m = self.result.metrics
     return (
-        f'COMPLETED(%s): Matches=%.{self.report_precision}f%% (%d/%d)'
-        f' Mismatches=%.{self.report_precision}f%% (%d/%d)'
-        f' Failures=%.{self.report_precision}f%% (%d/%d)'
+        'COMPLETED(%s):'
+        ' Matches=%s (%d/%d)'
+        ' Mismatches=%s (%d/%d)'
+        ' Failures=%s (%d/%d)'
     ) % (
         run_status,
-        m.match_rate * 100,
+        self._format_rate(m.match_rate),
         m.num_matches,
         m.total,
-        m.mismatch_rate * 100,
+        self._format_rate(m.mismatch_rate),
         m.num_mismatches,
         m.total,
-        m.failure_rate * 100,
+        self._format_rate(m.failure_rate),
         m.failures,
         m.total,
     )
 
-  def summarize(self) -> pg.Dict:
-    result = super().summarize()
+  def finalize(self) -> pg.Dict:
+    result = super().finalize()
     result.metrics.update(
         num_matches=self.num_matches,
         match_rate=self.match_rate,
         num_mismatches=self.num_mismatches,
         mismatch_rate=self.mismatch_rate,
     )
     return result
@@ -214,55 +215,55 @@
     super()._render_result_header(s)
     s.write('<td>Mismatches</td>')
     s.write('<td>Matches</td>')
 
   def _render_result_row(self, s: io.StringIO):
     super()._render_result_row(s)
     s.write(
-        '<td><span style="color:red">%s</span>%s</td>'
+        '<td><span style="color:orange">%s</span>%s</td>'
         % (
-            f'%.{self.report_precision}f%% ' % (self.mismatch_rate * 100),
+            self._format_rate(self.mismatch_rate),
             '<a href="%s">(%d/%d)</a>'
             % (self.mismatches_link, self.num_mismatches, self.num_completed),
         )
     )
     s.write(
         '<td><span style="color:green">%s</span>%s</td>'
         % (
-            f'%.{self.report_precision}f%% ' % (self.match_rate * 100),
+            self._format_rate(self.match_rate),
             '<a href="%s">(%d/%d)</a>'
             % (self.matches_link, self.num_matches, self.num_completed),
         )
     )
 
-  def _render_metric(self, s: io.StringIO) -> None:
+  def _render_summary_metrics(self, s: io.StringIO) -> None:
     """Renders metrics in HTML."""
     assert self.result is not None
     m = self.result.metrics
     s.write(
         '<a title="Matches (%d/%d)" href="%s" style="color:green">%s</a>'
         % (
             m.num_matches,
             m.total,
             self.matches_link,
-            f'%.{self.report_precision}f%% ' % (m.match_rate * 100),
+            self._format_rate(m.match_rate),
         )
     )
     s.write(' | ')
     s.write(
         '<a title="Mismatches (%d/%d)" href="%s" style="color:orange">%s</a>'
         % (
             m.num_mismatches,
             m.total,
             self.mismatches_link,
-            f'%.{self.report_precision}f%% ' % (m.mismatch_rate * 100),
+            self._format_rate(m.mismatch_rate),
         )
     )
     s.write(' | ')
-    super()._render_metric(s)
+    super()._render_summary_metrics(s)
 
   def _render_matches(self, s: io.StringIO) -> None:
     """Formats the matched cases into html."""
     s.write('<h2> Matches (Correct) </h2>')
     s.write('<div style="white-space:pre">\n')
     s.write(
         '<table style="border: 1px solid;">'
```

### Comparing `langfun-0.0.2.dev20240429/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240430/langfun/core/eval/matching_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,21 @@
                 num_hits=1,
                 num_updates=3,
             ),
             metrics=dict(
                 total=4,
                 failures=1,
                 failure_rate=0.25,
+                oop_failures=1,
+                oop_failure_rate=0.25,
+                non_oop_failures=0,
+                non_oop_failure_rate=0.0,
+                failure_breakdown={
+                    'MappingError.SchemaError.TypeError': 1
+                },
                 num_matches=2,
                 match_rate=0.5,
                 num_mismatches=1,
                 mismatch_rate=0.25,
             ),
             usage=s.result.usage,
         ),
@@ -156,30 +163,44 @@
                 s.dir, matching.Matching.MISMATCHES_JSON
             )
         )
     )
     self.assertTrue(
         os.path.exists(
             os.path.join(
-                s.dir, matching.Matching.FAILURES_JSON
+                s.dir, matching.Matching.OOP_FAILURES_JSON
+            )
+        )
+    )
+    self.assertTrue(
+        os.path.exists(
+            os.path.join(
+                s.dir, matching.Matching.NON_OOP_FAILURES_JSON
             )
         )
     )
     self.assertTrue(
         os.path.exists(os.path.join(s.root_dir, matching.Matching.SUMMARY_HTML))
     )
     self.assertTrue(
         os.path.exists(
             os.path.join(s.dir, matching.Matching.INDEX_HTML)
         )
     )
     self.assertTrue(
         os.path.exists(
             os.path.join(
-                s.dir, matching.Matching.FAILURES_HTML
+                s.dir, matching.Matching.OOP_FAILURES_HTML
+            )
+        )
+    )
+    self.assertTrue(
+        os.path.exists(
+            os.path.join(
+                s.dir, matching.Matching.NON_OOP_FAILURES_HTML
             )
         )
     )
     self.assertTrue(
         os.path.exists(
             os.path.join(s.dir, matching.Matching.MATCHES_HTML)
         )
```

### Comparing `langfun-0.0.2.dev20240429/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240430/langfun/core/eval/scoring.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,16 +109,16 @@
         m.num_scored,
         m.total,
         m.failure_rate * 100,
         m.failures,
         m.total,
     )
 
-  def summarize(self) -> pg.Dict:
-    result = super().summarize()
+  def finalize(self) -> pg.Dict:
+    result = super().finalize()
     result.metrics.update(
         num_scored=self.num_scored,
         score_rate=self.score_rate,
         avg_score=self.avg_score,
     )
     return result
 
@@ -164,29 +164,29 @@
         % (
             '%.2f%% ' % (self.score_rate * 100),
             '<a href="%s">(%d/%d)</a>'
             % (self.scored_link, self.num_scored, self.num_completed),
         )
     )
 
-  def _render_metric(self, s: io.StringIO) -> None:
+  def _render_summary_metrics(self, s: io.StringIO) -> None:
     """Renders metrics in HTML."""
     assert self.result is not None
     m = self.result.metrics
     s.write(
         '<a title="Average score (%d/%d)" href="%s" style="color:green">%s</a>'
         % (
             m.num_scored,
             m.total,
             self.scored_link,
             '%.2f%%' % (m.score_rate * 100),
         )
     )
     s.write(' | ')
-    super()._render_metric(s)
+    super()._render_summary_metrics(s)
 
   def _render_scored(self, s: io.StringIO) -> None:
     """Formats the matched cases into html."""
     s.write('<h2> Scored </h2>')
     s.write('<div style="white-space:pre">\n')
     s.write(
         '<table style="border: 1px solid;">'
```

### Comparing `langfun-0.0.2.dev20240429/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240430/langfun/core/eval/scoring_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,19 @@
                 num_hits=0,
                 num_updates=2,
             ),
             metrics=dict(
                 total=2,
                 failures=0,
                 failure_rate=0.0,
+                oop_failures=0,
+                oop_failure_rate=0.0,
+                non_oop_failures=0,
+                non_oop_failure_rate=0.0,
+                failure_breakdown={},
                 num_scored=2,
                 score_rate=1.0,
                 avg_score=0.5,
             ),
             usage=s.result.usage,
         ),
     )
@@ -120,15 +125,20 @@
     self.assertTrue(
         os.path.exists(
             os.path.join(s.dir, scoring.Scoring.RESULT_JSON)
         )
     )
     self.assertTrue(
         os.path.exists(
-            os.path.join(s.dir, scoring.Scoring.FAILURES_JSON)
+            os.path.join(s.dir, scoring.Scoring.OOP_FAILURES_JSON)
+        )
+    )
+    self.assertTrue(
+        os.path.exists(
+            os.path.join(s.dir, scoring.Scoring.NON_OOP_FAILURES_JSON)
         )
     )
     self.assertTrue(
         os.path.exists(
             os.path.join(s.dir, scoring.Scoring.SCORED_JSON)
         )
     )
@@ -139,15 +149,22 @@
         os.path.exists(
             os.path.join(s.dir, scoring.Scoring.INDEX_HTML)
         )
     )
     self.assertTrue(
         os.path.exists(
             os.path.join(
-                s.dir, scoring.Scoring.FAILURES_HTML
+                s.dir, scoring.Scoring.OOP_FAILURES_HTML
+            )
+        )
+    )
+    self.assertTrue(
+        os.path.exists(
+            os.path.join(
+                s.dir, scoring.Scoring.NON_OOP_FAILURES_HTML
             )
         )
     )
     self.assertTrue(
         os.path.exists(
             os.path.join(
                 s.dir, scoring.Scoring.SCORED_HTML
```

### Comparing `langfun-0.0.2.dev20240429/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240430/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240430/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/language_model.py` & `langfun-0.0.2.dev20240430/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240430/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/groq.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/groq_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
     def _open_ai_chat_completion(prompt: lf.Message):
       if self.multimodal:
         content = []
         for chunk in prompt.chunk():
           if isinstance(chunk, str):
             item = dict(type='text', text=chunk)
           elif isinstance(chunk, lf_modalities.Image) and chunk.uri:
-            item = dict(type='image_url', image_url=chunk.uri)
+            item = dict(type='image_url', image_url=dict(url=chunk.uri))
           else:
             raise ValueError(f'Unsupported modality object: {chunk!r}.')
           content.append(item)
       else:
         content = prompt.text
 
       response = openai.ChatCompletion.create(
```

### Comparing `langfun-0.0.2.dev20240429/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240430/langfun/core/llms/openai_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,16 @@
   )
 
 
 def mock_chat_completion_query_vision(messages, *, n=1, **kwargs):
   del kwargs
   choices = []
   urls = [
-      c['image_url'] for c in messages[0]['content'] if c['type'] == 'image_url'
+      c['image_url']['url']
+      for c in messages[0]['content'] if c['type'] == 'image_url'
   ]
   for k in range(n):
     choices.append(pg.Dict(
         message=pg.Dict(
             content=f'Sample {k} for message: {"".join(urls)}'
         ),
         logprobs=None,
```

### Comparing `langfun-0.0.2.dev20240429/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240430/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240430/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240430/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/memory.py` & `langfun-0.0.2.dev20240430/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/message.py` & `langfun-0.0.2.dev20240430/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/message_test.py` & `langfun-0.0.2.dev20240430/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240430/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240430/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240430/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240430/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240430/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240430/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240430/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/modality.py` & `langfun-0.0.2.dev20240430/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240430/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240430/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240430/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/sampling.py` & `langfun-0.0.2.dev20240430/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240430/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240430/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/subscription.py` & `langfun-0.0.2.dev20240430/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240430/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/template.py` & `langfun-0.0.2.dev20240430/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/template_test.py` & `langfun-0.0.2.dev20240430/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240430/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240430/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240430/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240430/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240430/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240430/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240430/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240430/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240430/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240430/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240430/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240430/langfun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240429
+Version: 0.0.2.dev20240430
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240429/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240430/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240429/setup.py` & `langfun-0.0.2.dev20240430/setup.py`

 * *Files identical despite different names*

