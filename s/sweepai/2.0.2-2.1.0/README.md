# Comparing `tmp/sweepai-2.0.2.tar.gz` & `tmp/sweepai-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-2.0.2.tar", last modified: Thu Apr 18 19:11:04 2024, max compression
+gzip compressed data, was "sweepai-2.1.0.tar", last modified: Tue Apr 30 23:02:00 2024, max compression
```

## Comparing `sweepai-2.0.2.tar` & `sweepai-2.1.0.tar`

### file list

```diff
@@ -1,138 +1,145 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/
--rw-r--r--   0 root         (0) root         (0)     2615 2024-04-14 06:06:44.000000 sweepai-2.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10788 2024-04-18 19:11:04.181913 sweepai-2.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6058 2024-04-14 06:06:44.000000 sweepai-2.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)     2073 2024-04-18 19:10:54.000000 sweepai-2.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 19:11:04.181913 sweepai-2.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.161913 sweepai-2.0.2/sweepai/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.165913 sweepai-2.0.2/sweepai/agents/
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/agent_utils.py
--rw-r--r--   0 root         (0) root         (0)     4691 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/assistant_functions.py
--rw-r--r--   0 root         (0) root         (0)     3525 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/assistant_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     4052 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/assistant_wrapper_test.py
--rw-r--r--   0 root         (0) root         (0)     2958 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/agents/complete_code.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/agents/complete_code_test.py
--rw-r--r--   0 root         (0) root         (0)     2448 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/distill_issue.py
--rw-r--r--   0 root         (0) root         (0)    43177 2024-04-18 18:59:36.000000 sweepai-2.0.2/sweepai/agents/modify.py
--rw-r--r--   0 root         (0) root         (0)    23096 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/modify_bot.py
--rw-r--r--   0 root         (0) root         (0)     3515 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/modify_file.py
--rw-r--r--   0 root         (0) root         (0)     1357 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/pr_description_bot.py
--rw-r--r--   0 root         (0) root         (0)     3814 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/agents/prune_modify_snippets.py
--rw-r--r--   0 root         (0) root         (0)    52254 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/api.py
--rw-r--r--   0 root         (0) root         (0)      753 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/api_test.py
--rw-r--r--   0 root         (0) root         (0)    13441 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/cli.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/cli_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.165913 sweepai-2.0.2/sweepai/config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12573 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/config/client.py
--rw-r--r--   0 root         (0) root         (0)     9845 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/config/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.169913 sweepai-2.0.2/sweepai/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19734 2024-04-18 17:51:40.000000 sweepai-2.0.2/sweepai/core/chat.py
--rw-r--r--   0 root         (0) root         (0)    49580 2024-04-16 16:51:35.000000 sweepai-2.0.2/sweepai/core/context_pruning.py
--rw-r--r--   0 root         (0) root         (0)    17807 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/entities.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/external_searcher.py
--rw-r--r--   0 root         (0) root         (0)    10786 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/lexical_search.py
--rw-r--r--   0 root         (0) root         (0)     5826 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/post_merge.py
--rw-r--r--   0 root         (0) root         (0)     4345 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/pr_reader.py
--rw-r--r--   0 root         (0) root         (0)    45655 2024-04-18 06:45:17.000000 sweepai-2.0.2/sweepai/core/prompts.py
--rw-r--r--   0 root         (0) root         (0)    33698 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/reflection_utils.py
--rw-r--r--   0 root         (0) root         (0)     5413 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/repo_parsing_utils.py
--rw-r--r--   0 root         (0) root         (0)    34537 2024-04-18 06:40:48.000000 sweepai-2.0.2/sweepai/core/sweep_bot.py
--rw-r--r--   0 root         (0) root         (0)     5758 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/core/update_prompts.py
--rw-r--r--   0 root         (0) root         (0)    10156 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/vector_db.py
--rw-r--r--   0 root         (0) root         (0)       19 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/global_threads.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.173913 sweepai-2.0.2/sweepai/handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15508 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/handlers/create_pr.py
--rw-r--r--   0 root         (0) root         (0)     5670 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/handlers/on_button_click.py
--rw-r--r--   0 root         (0) root         (0)     1569 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/handlers/on_button_click_test.py
--rw-r--r--   0 root         (0) root         (0)     5711 2024-04-18 19:10:06.000000 sweepai-2.0.2/sweepai/handlers/on_check_suite.py
--rw-r--r--   0 root         (0) root         (0)    18999 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/handlers/on_comment.py
--rw-r--r--   0 root         (0) root         (0)     3159 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/handlers/on_jira_ticket.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/handlers/on_merge.py
--rw-r--r--   0 root         (0) root         (0)    13160 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/handlers/on_merge_conflict.py
--rw-r--r--   0 root         (0) root         (0)      722 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/handlers/on_review.py
--rw-r--r--   0 root         (0) root         (0)    79750 2024-04-18 06:40:48.000000 sweepai-2.0.2/sweepai/handlers/on_ticket.py
--rw-r--r--   0 root         (0) root         (0)     5168 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/handlers/pr_utils.py
--rw-r--r--   0 root         (0) root         (0)    10042 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/handlers/stack_pr.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/handlers/stack_pr_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.173913 sweepai-2.0.2/sweepai/logn/
--rw-r--r--   0 root         (0) root         (0)       44 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/logn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7204 2024-04-17 00:16:26.000000 sweepai-2.0.2/sweepai/logn/cache.py
--rw-r--r--   0 root         (0) root         (0)    11758 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/logn/logn.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/logn/trace_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/sweepai/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3235 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/anthropic_client.py
--rw-r--r--   0 root         (0) root         (0)     1980 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/autoimport.py
--rw-r--r--   0 root         (0) root         (0)     3047 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/buttons.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/buttons_test.py
--rw-r--r--   0 root         (0) root         (0)     7850 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/chat_logger.py
--rw-r--r--   0 root         (0) root         (0)     7882 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/code_tree.py
--rw-r--r--   0 root         (0) root         (0)      716 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/code_tree_test.py
--rw-r--r--   0 root         (0) root         (0)      616 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/comment_utils.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/comment_utils_test.py
--rw-r--r--   0 root         (0) root         (0)     6761 2024-04-16 22:36:43.000000 sweepai-2.0.2/sweepai/utils/convert_openai_anthropic.py
--rw-r--r--   0 root         (0) root         (0)    13400 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/diff.py
--rw-r--r--   0 root         (0) root         (0)     2902 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/diff_test.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)      392 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/docker_utils_test.py
--rw-r--r--   0 root         (0) root         (0)     2637 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/event_logger.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/file_utils.py
--rw-r--r--   0 root         (0) root         (0)     7115 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/fuzzy_diff.py
--rw-r--r--   0 root         (0) root         (0)     2709 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/fuzzy_diff_test.py
--rw-r--r--   0 root         (0) root         (0)    24360 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/github_utils.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/github_utils_test.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/hash.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/html_extractor.py
--rw-r--r--   0 root         (0) root         (0)     4955 2024-04-16 18:54:57.000000 sweepai-2.0.2/sweepai/utils/modify_utils.py
--rw-r--r--   0 root         (0) root         (0)     5888 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/multi_query.py
--rw-r--r--   0 root         (0) root         (0)    34644 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/openai_listwise_reranker.py
--rw-r--r--   0 root         (0) root         (0)    11201 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/openai_proxy.py
--rw-r--r--   0 root         (0) root         (0)     4220 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/openai_proxy_test.py
--rw-r--r--   0 root         (0) root         (0)     1422 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/patch_utils.py
--rw-r--r--   0 root         (0) root         (0)     9641 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/progress.py
--rw-r--r--   0 root         (0) root         (0)      384 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/progress_test.py
--rw-r--r--   0 root         (0) root         (0)     7557 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/prompt_constructor.py
--rw-r--r--   0 root         (0) root         (0)      924 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/regex_utils.py
--rw-r--r--   0 root         (0) root         (0)      841 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/safe_pqueue.py
--rw-r--r--   0 root         (0) root         (0)     2022 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/scorer.py
--rw-r--r--   0 root         (0) root         (0)      791 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/scorer_test.py
--rw-r--r--   0 root         (0) root         (0)    13788 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/search_and_replace.py
--rw-r--r--   0 root         (0) root         (0)     2101 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/search_and_replace_test.py
--rw-r--r--   0 root         (0) root         (0)     4991 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/str_utils.py
--rw-r--r--   0 root         (0) root         (0)    17916 2024-04-17 23:25:00.000000 sweepai-2.0.2/sweepai/utils/ticket_utils.py
--rw-r--r--   0 root         (0) root         (0)      606 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/timer.py
--rw-r--r--   0 root         (0) root         (0)     7346 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/tree_utils.py
--rw-r--r--   0 root         (0) root         (0)     2963 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/user_settings.py
--rw-r--r--   0 root         (0) root         (0)    23680 2024-04-16 16:48:05.000000 sweepai-2.0.2/sweepai/utils/utils.py
--rw-r--r--   0 root         (0) root         (0)      586 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/utils_test.py
--rw-r--r--   0 root         (0) root         (0)     3989 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/sweepai/web/
--rw-r--r--   0 root         (0) root         (0)     1864 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/web/event_utils.py
--rw-r--r--   0 root         (0) root         (0)     4588 2024-03-03 05:40:09.000000 sweepai-2.0.2/sweepai/web/events.py
--rw-r--r--   0 root         (0) root         (0)     1945 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/web/health.py
--rw-r--r--   0 root         (0) root         (0)     1655 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/web/health_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/sweepai.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10788 2024-04-18 19:11:04.000000 sweepai-2.0.2/sweepai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3561 2024-04-18 19:11:04.000000 sweepai-2.0.2/sweepai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 19:11:04.000000 sweepai-2.0.2/sweepai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-18 19:11:04.000000 sweepai-2.0.2/sweepai.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      755 2024-04-18 19:11:04.000000 sweepai-2.0.2/sweepai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       93 2024-04-18 19:11:04.000000 sweepai-2.0.2/sweepai.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/tests/
--rw-r--r--   0 root         (0) root         (0)      573 2024-04-14 06:06:44.000000 sweepai-2.0.2/tests/test_gha_extraction.py
--rw-r--r--   0 root         (0) root         (0)      381 2024-04-14 06:06:44.000000 sweepai-2.0.2/tests/test_jira_ticket.py
--rw-r--r--   0 root         (0) root         (0)     3487 2024-04-18 19:10:06.000000 sweepai-2.0.2/tests/test_run_gha.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-02-26 23:28:50.000000 sweepai-2.0.2/tests/test_watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.161913 sweepai-2.0.2/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/vendor/tree-sitter-go/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.161913 sweepai-2.0.2/vendor/tree-sitter-go/bindings/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.161913 sweepai-2.0.2/vendor/tree-sitter-go/bindings/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/vendor/tree-sitter-go/bindings/python/tree_sitter_go/
--rw-r--r--   0 root         (0) root         (0)       85 2024-04-11 22:16:11.000000 sweepai-2.0.2/vendor/tree-sitter-go/bindings/python/tree_sitter_go/__init__.py
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-11 22:16:11.000000 sweepai-2.0.2/vendor/tree-sitter-go/bindings/python/tree_sitter_go/__init__.pyi
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 22:16:11.000000 sweepai-2.0.2/vendor/tree-sitter-go/bindings/python/tree_sitter_go/py.typed
--rw-r--r--   0 root         (0) root         (0)     1503 2024-04-11 22:16:11.000000 sweepai-2.0.2/vendor/tree-sitter-go/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.232103 sweepai-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     2615 2024-04-10 22:25:21.000000 sweepai-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10868 2024-04-30 23:02:00.232103 sweepai-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6058 2024-04-05 22:26:32.000000 sweepai-2.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.208103 sweepai-2.1.0/node_modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.208103 sweepai-2.1.0/node_modules/flatted/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.208103 sweepai-2.1.0/node_modules/flatted/python/
+-rw-r--r--   0 root         (0) root         (0)     3879 2024-04-30 18:30:02.000000 sweepai-2.1.0/node_modules/flatted/python/flatted.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2024-04-30 18:30:02.000000 sweepai-2.1.0/node_modules/flatted/python/test.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2024-04-30 20:53:17.000000 sweepai-2.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 23:02:00.232103 sweepai-2.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.208103 sweepai-2.1.0/sweepai/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.212103 sweepai-2.1.0/sweepai/agents/
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/agents/agent_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4691 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/agents/assistant_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3525 2024-04-14 03:11:57.000000 sweepai-2.1.0/sweepai/agents/assistant_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/agents/assistant_wrapper_test.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/agents/complete_code.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/agents/complete_code_test.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/agents/distill_issue.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2024-04-29 23:55:33.000000 sweepai-2.1.0/sweepai/agents/image_description_bot.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2024-04-20 23:30:39.000000 sweepai-2.1.0/sweepai/agents/issue_cleanup_agent.py
+-rw-r--r--   0 root         (0) root         (0)    82454 2024-04-30 20:53:17.000000 sweepai-2.1.0/sweepai/agents/modify.py
+-rw-r--r--   0 root         (0) root         (0)    23163 2024-04-27 01:24:38.000000 sweepai-2.1.0/sweepai/agents/modify_bot.py
+-rw-r--r--   0 root         (0) root         (0)     3564 2024-04-26 18:59:24.000000 sweepai-2.1.0/sweepai/agents/modify_file.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/agents/pr_description_bot.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/agents/prune_modify_snippets.py
+-rw-r--r--   0 root         (0) root         (0)    43534 2024-04-30 19:27:55.000000 sweepai-2.1.0/sweepai/api.py
+-rw-r--r--   0 root         (0) root         (0)      753 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/api_test.py
+-rw-r--r--   0 root         (0) root         (0)    13653 2024-04-21 21:37:03.000000 sweepai-2.1.0/sweepai/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/cli_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.212103 sweepai-2.1.0/sweepai/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12716 2024-04-26 18:59:24.000000 sweepai-2.1.0/sweepai/config/client.py
+-rw-r--r--   0 root         (0) root         (0)     9973 2024-04-27 01:24:38.000000 sweepai-2.1.0/sweepai/config/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.216103 sweepai-2.1.0/sweepai/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6443 2024-04-29 17:41:13.000000 sweepai-2.1.0/sweepai/core/annotate_code_openai.py
+-rw-r--r--   0 root         (0) root         (0)    22718 2024-04-26 18:59:24.000000 sweepai-2.1.0/sweepai/core/chat.py
+-rw-r--r--   0 root         (0) root         (0)    50143 2024-04-30 02:17:06.000000 sweepai-2.1.0/sweepai/core/context_pruning.py
+-rw-r--r--   0 root         (0) root         (0)    17899 2024-04-27 01:24:38.000000 sweepai-2.1.0/sweepai/core/entities.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/core/external_searcher.py
+-rw-r--r--   0 root         (0) root         (0)    10786 2024-04-04 06:39:36.000000 sweepai-2.1.0/sweepai/core/lexical_search.py
+-rw-r--r--   0 root         (0) root         (0)     7192 2024-04-30 19:27:55.000000 sweepai-2.1.0/sweepai/core/planning_prompts.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/core/post_merge.py
+-rw-r--r--   0 root         (0) root         (0)     4345 2024-04-04 06:39:36.000000 sweepai-2.1.0/sweepai/core/pr_reader.py
+-rw-r--r--   0 root         (0) root         (0)    59204 2024-04-30 19:27:55.000000 sweepai-2.1.0/sweepai/core/prompts.py
+-rw-r--r--   0 root         (0) root         (0)    33618 2024-04-26 18:59:24.000000 sweepai-2.1.0/sweepai/core/reflection_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2024-04-09 21:46:59.000000 sweepai-2.1.0/sweepai/core/repo_parsing_utils.py
+-rw-r--r--   0 root         (0) root         (0)    69875 2024-04-30 19:12:59.000000 sweepai-2.1.0/sweepai/core/sweep_bot.py
+-rw-r--r--   0 root         (0) root         (0)     5758 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/core/update_prompts.py
+-rw-r--r--   0 root         (0) root         (0)    10156 2024-04-26 18:59:24.000000 sweepai-2.1.0/sweepai/core/vector_db.py
+-rw-r--r--   0 root         (0) root         (0)       19 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/global_threads.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.216103 sweepai-2.1.0/sweepai/handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15539 2024-04-26 18:59:24.000000 sweepai-2.1.0/sweepai/handlers/create_pr.py
+-rw-r--r--   0 root         (0) root         (0)     5670 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/handlers/on_button_click.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/handlers/on_button_click_test.py
+-rw-r--r--   0 root         (0) root         (0)     5711 2024-04-20 23:30:39.000000 sweepai-2.1.0/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0 root         (0) root         (0)    19058 2024-04-26 18:59:24.000000 sweepai-2.1.0/sweepai/handlers/on_comment.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2024-04-08 20:37:50.000000 sweepai-2.1.0/sweepai/handlers/on_jira_ticket.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/handlers/on_merge.py
+-rw-r--r--   0 root         (0) root         (0)    13160 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/handlers/on_merge_conflict.py
+-rw-r--r--   0 root         (0) root         (0)      722 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/handlers/on_review.py
+-rw-r--r--   0 root         (0) root         (0)    79206 2024-04-30 22:41:13.000000 sweepai-2.1.0/sweepai/handlers/on_ticket.py
+-rw-r--r--   0 root         (0) root         (0)     4996 2024-04-20 23:30:39.000000 sweepai-2.1.0/sweepai/handlers/pr_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10042 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/handlers/stack_pr.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/handlers/stack_pr_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.220103 sweepai-2.1.0/sweepai/logn/
+-rw-r--r--   0 root         (0) root         (0)       44 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/logn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7428 2024-04-26 18:59:24.000000 sweepai-2.1.0/sweepai/logn/cache.py
+-rw-r--r--   0 root         (0) root         (0)    11758 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/logn/logn.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/logn/trace_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.228103 sweepai-2.1.0/sweepai/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3279 2024-04-26 18:59:24.000000 sweepai-2.1.0/sweepai/utils/anthropic_client.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/autoimport.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/buttons.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/buttons_test.py
+-rw-r--r--   0 root         (0) root         (0)     7850 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/chat_logger.py
+-rw-r--r--   0 root         (0) root         (0)     7881 2024-04-21 21:37:03.000000 sweepai-2.1.0/sweepai/utils/code_tree.py
+-rw-r--r--   0 root         (0) root         (0)      716 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/code_tree_test.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-04-20 23:30:39.000000 sweepai-2.1.0/sweepai/utils/cohere_utils.py
+-rw-r--r--   0 root         (0) root         (0)      616 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/comment_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/comment_utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     6761 2024-04-20 23:30:39.000000 sweepai-2.1.0/sweepai/utils/convert_openai_anthropic.py
+-rw-r--r--   0 root         (0) root         (0)    13860 2024-04-29 23:13:05.000000 sweepai-2.1.0/sweepai/utils/diff.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/diff_test.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)      392 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/docker_utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/event_logger.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/file_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10663 2024-04-30 19:27:55.000000 sweepai-2.1.0/sweepai/utils/fuzzy_diff.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/fuzzy_diff_test.py
+-rw-r--r--   0 root         (0) root         (0)    26741 2024-04-26 18:59:24.000000 sweepai-2.1.0/sweepai/utils/github_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/github_utils_test.py
+-rw-r--r--   0 root         (0) root         (0)      115 2024-04-20 23:30:39.000000 sweepai-2.1.0/sweepai/utils/hash.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/html_extractor.py
+-rw-r--r--   0 root         (0) root         (0)     6976 2024-04-29 23:55:33.000000 sweepai-2.1.0/sweepai/utils/image_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2379 2024-04-30 23:01:24.000000 sweepai-2.1.0/sweepai/utils/issue_validator.py
+-rw-r--r--   0 root         (0) root         (0)     5003 2024-04-29 23:55:33.000000 sweepai-2.1.0/sweepai/utils/modify_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5957 2024-04-27 01:24:38.000000 sweepai-2.1.0/sweepai/utils/multi_query.py
+-rw-r--r--   0 root         (0) root         (0)    34644 2024-04-12 22:10:10.000000 sweepai-2.1.0/sweepai/utils/openai_listwise_reranker.py
+-rw-r--r--   0 root         (0) root         (0)    12124 2024-04-26 18:59:24.000000 sweepai-2.1.0/sweepai/utils/openai_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     4220 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/openai_proxy_test.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/patch_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10739 2024-04-26 18:59:24.000000 sweepai-2.1.0/sweepai/utils/previous_diff_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9641 2024-03-28 21:42:33.000000 sweepai-2.1.0/sweepai/utils/progress.py
+-rw-r--r--   0 root         (0) root         (0)      384 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/progress_test.py
+-rw-r--r--   0 root         (0) root         (0)     7557 2024-04-08 20:37:50.000000 sweepai-2.1.0/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0 root         (0) root         (0)      924 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/regex_utils.py
+-rw-r--r--   0 root         (0) root         (0)      841 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/safe_pqueue.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/scorer.py
+-rw-r--r--   0 root         (0) root         (0)      791 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/scorer_test.py
+-rw-r--r--   0 root         (0) root         (0)    13788 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/search_and_replace.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/search_and_replace_test.py
+-rw-r--r--   0 root         (0) root         (0)     4995 2024-04-22 22:27:37.000000 sweepai-2.1.0/sweepai/utils/str_utils.py
+-rw-r--r--   0 root         (0) root         (0)    18093 2024-04-29 17:41:51.000000 sweepai-2.1.0/sweepai/utils/ticket_utils.py
+-rw-r--r--   0 root         (0) root         (0)      606 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/timer.py
+-rw-r--r--   0 root         (0) root         (0)     7346 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/tree_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/user_settings.py
+-rw-r--r--   0 root         (0) root         (0)    27849 2024-04-30 22:41:13.000000 sweepai-2.1.0/sweepai/utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)      586 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/utils/utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-22 17:25:19.000000 sweepai-2.1.0/sweepai/utils/validate_license.py
+-rw-r--r--   0 root         (0) root         (0)     3989 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.228103 sweepai-2.1.0/sweepai/web/
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-04-08 20:37:50.000000 sweepai-2.1.0/sweepai/web/event_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/web/events.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/web/health.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2024-03-26 02:10:48.000000 sweepai-2.1.0/sweepai/web/health_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.228103 sweepai-2.1.0/sweepai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10868 2024-04-30 23:02:00.000000 sweepai-2.1.0/sweepai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3788 2024-04-30 23:02:00.000000 sweepai-2.1.0/sweepai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 23:02:00.000000 sweepai-2.1.0/sweepai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-30 23:02:00.000000 sweepai-2.1.0/sweepai.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      805 2024-04-30 23:02:00.000000 sweepai-2.1.0/sweepai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2024-04-30 23:02:00.000000 sweepai-2.1.0/sweepai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 23:02:00.228103 sweepai-2.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-04-30 02:17:06.000000 sweepai-2.1.0/tests/test_context_pruning.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-04-26 18:59:24.000000 sweepai-2.1.0/tests/test_get_gha_logs_from_pr.py
+-rw-r--r--   0 root         (0) root         (0)      560 2024-04-30 01:46:06.000000 sweepai-2.1.0/tests/test_gha_extraction.py
+-rw-r--r--   0 root         (0) root         (0)      381 2024-04-08 20:37:50.000000 sweepai-2.1.0/tests/test_jira_ticket.py
+-rw-r--r--   0 root         (0) root         (0)     3487 2024-04-20 23:30:39.000000 sweepai-2.1.0/tests/test_run_gha.py
+-rw-r--r--   0 root         (0) root         (0)      314 2024-03-26 02:10:48.000000 sweepai-2.1.0/tests/test_watch.py
```

### Comparing `sweepai-2.0.2/LICENSE` & `sweepai-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/PKG-INFO` & `sweepai-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 2.0.2
+Version: 2.1.0
 Summary: Sweep fixes GitHub issues
 Author-email: Kevin Lu <kevin@sweep.dev>, William Zeng <william@sweep.dev>, Martin Ye <martin@sweep.dev>
 License: Sweep Enterprise Edition (EE) license (the “EE License”)
         Copyright (c) 2024-present Sweep AI, Inc.
         
         With regard to the Sweep Software:
         
@@ -38,16 +38,18 @@
 Requires-Dist: prometheus-fastapi-instrumentator==7.0.0
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: openai==1.13.3
 Requires-Dist: backoff==2.2.1
 Requires-Dist: pymongo==4.6.3
 Requires-Dist: gitpython==3.1.42
+Requires-Dist: stringzilla==3.8.4
 Requires-Dist: tree-sitter==0.21.0
 Requires-Dist: tree-sitter-python==0.21.0
+Requires-Dist: tree-sitter-javascript==0.21.0
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: rapidfuzz==3.6.2
 Requires-Dist: importmagic==0.1.7
 Requires-Dist: hatchet-sdk==0.18.0
 Requires-Dist: pyflakes==3.2.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: networkx==3.2.1
```

### Comparing `sweepai-2.0.2/README.md` & `sweepai-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/pyproject.toml` & `sweepai-2.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Community = "https://discord.gg/sweep"
 Documentation = "https://docs.sweep.dev"
 Homepage = "https://sweep.dev"
 "Bug Tracker" = "https://github.com/sweepai/sweep/issues"
 
 [project]
 name = "sweepai"
-version = "2.0.2"
+version = "2.1.0"
 description = "Sweep fixes GitHub issues"
 authors = [
     {name = "Kevin Lu", email = "kevin@sweep.dev"},
     {name = "William Zeng", email = "william@sweep.dev"},
     {name = "Martin Ye", email = "martin@sweep.dev"},
 ]
 readme = "README.md"
@@ -43,16 +43,18 @@
   "prometheus-fastapi-instrumentator==7.0.0",
   "pyyaml==6.0.1",
   "python-dotenv==1.0.1",
   "openai==1.13.3",
   "backoff==2.2.1",
   "pymongo==4.6.3",
   "gitpython==3.1.42",
+  "stringzilla==3.8.4",
   "tree-sitter==0.21.0",
   "tree-sitter-python==0.21.0",
+  "tree-sitter-javascript==0.21.0",
   "tree-sitter-languages==1.10.2",
   "rapidfuzz==3.6.2",
   "importmagic==0.1.7",
   "hatchet-sdk==0.18.0",
   "pyflakes==3.2.0",
   "beautifulsoup4==4.12.3",
   "networkx==3.2.1",
```

### Comparing `sweepai-2.0.2/sweepai/agents/agent_utils.py` & `sweepai-2.1.0/sweepai/agents/agent_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/agents/assistant_functions.py` & `sweepai-2.1.0/sweepai/agents/assistant_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/agents/assistant_wrapper.py` & `sweepai-2.1.0/sweepai/agents/assistant_wrapper.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/agents/assistant_wrapper_test.py` & `sweepai-2.1.0/sweepai/agents/assistant_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/agents/complete_code.py` & `sweepai-2.1.0/sweepai/agents/complete_code.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/agents/complete_code_test.py` & `sweepai-2.1.0/sweepai/agents/complete_code_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/agents/distill_issue.py` & `sweepai-2.1.0/sweepai/agents/distill_issue.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/agents/modify_bot.py` & `sweepai-2.1.0/sweepai/agents/modify_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,15 @@
         new_files = modify(
             request=instructions,
             cloned_repo=cloned_repo,
             relevant_filepaths=relevant_filepaths,
             fcrs=fcrs,
             chat_logger=self.chat_logger,
             use_openai=use_openai,
+            previous_modify_files_dict=previous_modify_files_dict,
         )
         if new_files:
             posthog.capture(
                 (
                     self.chat_logger.data["username"]
                     if self.chat_logger is not None
                     else "anonymous"
```

### Comparing `sweepai-2.0.2/sweepai/agents/modify_file.py` & `sweepai-2.1.0/sweepai/agents/modify_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         from sweepai.utils.github_utils import get_installation_id
         organization_name = "sweepai"
         installation_id = get_installation_id(organization_name)
         cloned_repo = ClonedRepo("sweepai/sweep", installation_id, "main")
 
         new_file = modify_file(
             cloned_repo=cloned_repo,
+            request="complete the user request",
             metadata="This repo is Sweep.",
             file_change_requests=[FileChangeRequest(
                 filename="sweepai/api.py",
                 instructions="import math at the top of the file",
                 change_type="modify",
             )],
         )
```

### Comparing `sweepai-2.0.2/sweepai/agents/pr_description_bot.py` & `sweepai-2.1.0/sweepai/agents/pr_description_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/agents/prune_modify_snippets.py` & `sweepai-2.1.0/sweepai/agents/prune_modify_snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/api.py` & `sweepai-2.1.0/sweepai/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,37 +19,33 @@
 )
 from fastapi.responses import HTMLResponse
 from fastapi.security import HTTPAuthorizationCredentials, HTTPBearer
 from fastapi.templating import Jinja2Templates
 from github.Commit import Commit
 
 from sweepai.config.client import (
-    DEFAULT_RULES,
     RESTART_SWEEP_BUTTON,
     REVERT_CHANGED_FILES_TITLE,
-    RULES_LABEL,
     RULES_TITLE,
     SWEEP_BAD_FEEDBACK,
     SWEEP_GOOD_FEEDBACK,
     SweepConfig,
     get_gha_enabled,
-    get_rules,
 )
 from sweepai.config.server import (
     BLACKLISTED_USERS,
     DISABLED_REPOS,
     DISCORD_FEEDBACK_WEBHOOK_URL,
     ENV,
     GHA_AUTOFIX_ENABLED,
     GITHUB_BOT_USERNAME,
     GITHUB_LABEL_COLOR,
     GITHUB_LABEL_DESCRIPTION,
     GITHUB_LABEL_NAME,
     IS_SELF_HOSTED,
-    MERGE_CONFLICT_ENABLED,
 )
 from sweepai.core.entities import PRChangeRequest
 from sweepai.global_threads import global_threads
 from sweepai.handlers.create_pr import (  # type: ignore
     add_config_to_top_repos,
     create_gha_pr,
 )
@@ -57,22 +53,17 @@
 from sweepai.handlers.on_check_suite import (  # type: ignore
     clean_gh_logs,
     download_logs,
     on_check_suite,
 )
 from sweepai.handlers.on_comment import on_comment
 from sweepai.handlers.on_jira_ticket import handle_jira_ticket
-from sweepai.handlers.on_merge import on_merge
-from sweepai.handlers.on_merge_conflict import on_merge_conflict
 from sweepai.handlers.on_ticket import on_ticket
-from sweepai.handlers.pr_utils import make_pr
 from sweepai.handlers.stack_pr import stack_pr
 from sweepai.utils.buttons import (
-    Button,
-    ButtonList,
     check_button_activated,
     check_button_title_match,
 )
 from sweepai.utils.chat_logger import ChatLogger
 from sweepai.utils.event_logger import logger, posthog
 from sweepai.utils.github_utils import CURRENT_USERNAME, get_github_client
 from sweepai.utils.progress import TicketProgress
@@ -237,20 +228,14 @@
         thread.name == key and thread.is_alive() for thread in threading.enumerate()
     ):
         thread = threading.Thread(target=worker, name=key)
         thread.start()
         global_threads.append(thread)
 
 
-def call_on_merge(*args, **kwargs):
-    thread = threading.Thread(target=on_merge, args=args, kwargs=kwargs)
-    thread.start()
-    global_threads.append(thread)
-
-
 @app.get("/health")
 def redirect_to_health():
     return health_check()
 
 
 @app.get("/", response_class=HTMLResponse)
 def home(request: Request):
@@ -499,114 +484,28 @@
                                 pr_number=pr.number,
                                 username=attributor,
                                 repo_full_name=repo.full_name,
                                 installation_id=request.installation.id,
                                 tracking_id=tracking_id,
                                 commit_hash=pr.head.sha,
                             )
-                elif (
-                    request.check_run.check_suite.head_branch == repo.default_branch
-                    and get_gha_enabled(repo)
-                    and GHA_AUTOFIX_ENABLED
-                ):
-                    if request.check_run.conclusion == "failure":
-                        commit = repo.get_commit(request.check_run.head_sha)
-                        attributor = request.sender.login
-                        if attributor.endswith("[bot]"):
-                            attributor = commit.author.login
-                        if attributor.endswith("[bot]"):
-                            return {
-                                "success": False,
-                                "error_message": "The PR was created by a bot, so I won't attempt to fix it.",
-                            }
-                        logs = download_logs(
-                            request.repository.full_name,
-                            request.check_run.run_id,
-                            request.installation.id,
-                        )
-                        logs, user_message = clean_gh_logs(logs)
-                        chat_logger = ChatLogger(
-                            data={
-                                "username": attributor,
-                                "title": "[Sweep GHA Fix] Fix the failing GitHub Actions",
-                            }
-                        )
-                        if chat_logger.use_faster_model() and not IS_SELF_HOSTED:
-                            return {
-                                "success": False,
-                                "error_message": "Disabled for free users",
-                            }
-                        make_pr(
-                            title=f"[Sweep GHA Fix] Fix the failing GitHub Actions on {request.check_run.head_sha[:7]} ({repo.default_branch})",
-                            repo_description=repo.description,
-                            summary=f"The GitHub Actions run failed with the following error logs:\n\n```\n{logs}\n```",
-                            repo_full_name=request_dict["repository"]["full_name"],
-                            installation_id=request_dict["installation"]["id"],
-                            user_token=None,
-                            use_faster_model=chat_logger.use_faster_model(),
-                            username=attributor,
-                            chat_logger=chat_logger,
-                        )
-
             case "pull_request", "opened":
                 _, g = get_github_client(request_dict["installation"]["id"])
                 repo = g.get_repo(request_dict["repository"]["full_name"])
                 pr = repo.get_pull(request_dict["pull_request"]["number"])
                 # if the pr already has a comment from sweep bot do nothing
                 time.sleep(10)
                 if any(
                     comment.user.login == GITHUB_BOT_USERNAME
                     for comment in pr.get_issue_comments()
                 ) or pr.title.startswith("Sweep:"):
                     return {
                         "success": True,
                         "reason": "PR already has a comment from sweep bot",
                     }
-                rule_buttons = []
-                repo_rules = get_rules(repo) or []
-                if repo_rules != [""] and repo_rules != []:
-                    for rule in repo_rules or []:
-                        if rule:
-                            rule_buttons.append(Button(label=f"{RULES_LABEL} {rule}"))
-                    if len(repo_rules) == 0:
-                        for rule in DEFAULT_RULES:
-                            rule_buttons.append(Button(label=f"{RULES_LABEL} {rule}"))
-                if rule_buttons:
-                    rules_buttons_list = ButtonList(
-                        buttons=rule_buttons, title=RULES_TITLE
-                    )
-                    pr.create_issue_comment(rules_buttons_list.serialize() + BOT_SUFFIX)
-
-                if pr.mergeable is False and MERGE_CONFLICT_ENABLED:
-                    attributor = pr.user.login
-                    if attributor.endswith("[bot]"):
-                        attributor = pr.assignee.login
-                    if attributor.endswith("[bot]"):
-                        return {
-                            "success": False,
-                            "error_message": "The PR was created by a bot, so I won't attempt to fix it.",
-                        }
-                    chat_logger = ChatLogger(
-                        data={
-                            "username": attributor,
-                            "title": "[Sweep GHA Fix] Fix the failing GitHub Actions",
-                        }
-                    )
-                    if chat_logger.use_faster_model() and not IS_SELF_HOSTED:
-                        return {
-                            "success": False,
-                            "error_message": "Disabled for free users",
-                        }
-                    on_merge_conflict(
-                        pr_number=pr.number,
-                        username=attributor,
-                        repo_full_name=request_dict["repository"]["full_name"],
-                        installation_id=request_dict["installation"]["id"],
-                        tracking_id=get_hash(),
-                    )
             case "issues", "opened":
                 request = IssueRequest(**request_dict)
                 issue_title_lower = request.issue.title.lower()
                 if (
                     issue_title_lower.startswith("sweep")
                     or "sweep:" in issue_title_lower
                 ):
@@ -1103,77 +1002,11 @@
                             + pr_request.pull_request.deletions,
                             "edited_by_developers": edited_by_developers,
                             "total_lines_in_commit": total_lines_in_commit,
                             "total_lines_edited_by_developer": total_lines_edited_by_developer,
                         },
                     )
                 chat_logger = ChatLogger({"username": merged_by})
-            case "push", None:
-                if event != "pull_request" or request_dict["base"]["merged"] is True:
-                    chat_logger = ChatLogger(
-                        {"username": request_dict["pusher"]["name"]}
-                    )
-                    # on merge
-                    call_on_merge(request_dict, chat_logger)
-                    ref = request_dict["ref"] if "ref" in request_dict else ""
-                    if ref.startswith("refs/heads") and not ref.startswith(
-                        "ref/heads/sweep"
-                    ):
-                        _, g = get_github_client(request_dict["installation"]["id"])
-                        repo = g.get_repo(request_dict["repository"]["full_name"])
-                        if ref[len("refs/heads/") :] == SweepConfig.get_branch(repo):
-                            update_sweep_prs_v2(
-                                request_dict["repository"]["full_name"],
-                                installation_id=request_dict["installation"]["id"],
-                            )
-                    if ref.startswith("refs/heads"):
-                        branch_name = ref[len("refs/heads/") :]
-                        # Check if the branch has an associated PR
-
-                        org_name, repo_name = request_dict["repository"][
-                            "full_name"
-                        ].split("/")
-                        pulls = repo.get_pulls(
-                            state="open",
-                            sort="created",
-                            head=org_name + ":" + branch_name,
-                        )
-                        for pr in pulls:
-                            logger.info(
-                                f"PR associated with branch {branch_name}: #{pr.number} - {pr.title}"
-                            )
-                            if pr.mergeable is False and MERGE_CONFLICT_ENABLED:
-                                attributor = pr.user.login
-                                if attributor.endswith("[bot]"):
-                                    attributor = pr.assignee.login
-                                if attributor.endswith("[bot]"):
-                                    return {
-                                        "success": False,
-                                        "error_message": "The PR was created by a bot, so I won't attempt to fix it.",
-                                    }
-                                chat_logger = ChatLogger(
-                                    data={
-                                        "username": attributor,
-                                        "title": "[Sweep GHA Fix] Fix the failing GitHub Actions",
-                                    }
-                                )
-                                if (
-                                    chat_logger.use_faster_model()
-                                    and not IS_SELF_HOSTED
-                                ):
-                                    return {
-                                        "success": False,
-                                        "error_message": "Disabled for free users",
-                                    }
-                                on_merge_conflict(
-                                    pr_number=pr.number,
-                                    username=pr.user.login,
-                                    repo_full_name=request_dict["repository"][
-                                        "full_name"
-                                    ],
-                                    installation_id=request_dict["installation"]["id"],
-                                    tracking_id=get_hash(),
-                                )
             case "ping", None:
                 return {"message": "pong"}
             case _:
                 return {"error": "Unsupported type"}
```

### Comparing `sweepai-2.0.2/sweepai/api_test.py` & `sweepai-2.1.0/sweepai/api_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/cli.py` & `sweepai-2.1.0/sweepai/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from sweepai.web.events import Account, Installation, IssueRequest
 
 app = typer.Typer(
     name="sweepai", context_settings={"help_option_names": ["-h", "--help"]}
 )
 app_dir = typer.get_app_dir("sweepai")
 config_path = os.path.join(app_dir, "config.json")
+os.environ["CLI"] = "True"
 
 console = Console()
 cprint = console.print
 
 
 def posthog_capture(event_name, properties, *args, **kwargs):
     POSTHOG_DISTINCT_ID = os.environ.get("POSTHOG_DISTINCT_ID")
@@ -40,15 +41,19 @@
 
 
 def load_config():
     if os.path.exists(config_path):
         cprint(f"\nLoading configuration from {config_path}", style="yellow")
         with open(config_path, "r") as f:
             config = json.load(f)
-        os.environ.update(config)
+        for key, value in config.items():
+            try:
+                os.environ[key] = value
+            except Exception as e:
+                cprint(f"Error loading config: {e}, skipping.", style="yellow")
         os.environ["POSTHOG_DISTINCT_ID"] = str(os.environ.get("POSTHOG_DISTINCT_ID", ""))
         # Should contain:
         # GITHUB_PAT
         # OPENAI_API_KEY
         # ANTHROPIC_API_KEY
         # VOYAGE_API_KEY
         # POSTHOG_DISTINCT_ID
@@ -289,15 +294,15 @@
         default=True,
     )
     if enable_telemetry:
         cprint(
             "\nThank you for enabling telemetry. We'll collect anonymous usage statistics to improve the product. You can disable this at any time by rerunning 'sweep init'.",
             style="yellow",
         )
-        POSTHOG_DISTINCT_ID = uuid.getnode()
+        POSTHOG_DISTINCT_ID = str(uuid.getnode())
         posthog.capture(POSTHOG_DISTINCT_ID, "sweep_init", {})
 
     config = {
         "GITHUB_PAT": github_pat,
         "OPENAI_API_KEY": openai_api_key,
         "ANTHROPIC_API_KEY": anthropic_api_key,
         "VOYAGE_API_KEY": voyage_api_key,
```

### Comparing `sweepai-2.0.2/sweepai/cli_test.py` & `sweepai-2.1.0/sweepai/cli_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/config/client.py` & `sweepai-2.1.0/sweepai/config/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,21 @@
     ]
     # cutoff for when we output truncated versions of strings, this is an arbitrary number and can be changed
     truncation_cutoff: int = 20000
     # Image formats
     max_file_limit: int = 60_000
     # github comments
     max_github_comment_body_length: int = 65535
+    # allowed image types for vision
+    allowed_image_types: list[str] = [
+        "jpg",
+        "jpeg",
+        "webp",
+        "png"
+    ]
 
     def to_yaml(self) -> str:
         return yaml.safe_dump(self.dict())
 
     @classmethod
     def from_yaml(cls, yaml_str: str) -> "SweepConfig":
         data = yaml.safe_load(yaml_str)
```

### Comparing `sweepai-2.0.2/sweepai/config/server.py` & `sweepai-2.1.0/sweepai/config/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     MULTI_REGION_CONFIG = [item.split(",") for item in MULTI_REGION_CONFIG.split("\n")]
 
 WHITELISTED_USERS = os.environ.get("WHITELISTED_USERS", None)
 if WHITELISTED_USERS:
     WHITELISTED_USERS = WHITELISTED_USERS.split(",")
     WHITELISTED_USERS.append(GITHUB_BOT_USERNAME)
 
-DEFAULT_GPT4_32K_MODEL = os.environ.get("DEFAULT_GPT4_32K_MODEL", "gpt-4-0125-preview")
+DEFAULT_GPT4_32K_MODEL = os.environ.get("DEFAULT_GPT4_32K_MODEL", "gpt-4-turbo-2024-04-09")
 DEFAULT_GPT35_MODEL = os.environ.get("DEFAULT_GPT35_MODEL", "gpt-3.5-turbo-1106")
 
 RESEND_API_KEY = os.environ.get("RESEND_API_KEY", None)
 LOKI_URL = None
 
 DEBUG = os.environ.get("DEBUG", "false").lower() == "true"
 ENV = "prod" if GITHUB_BOT_USERNAME != TEST_BOT_NAME else "dev"
@@ -244,7 +244,10 @@
 )
 
 DEPLOYMENT_GHA_ENABLED = os.environ.get("DEPLOYMENT_GHA_ENABLED", "true").lower() == "true"
 
 JIRA_USER_NAME = os.environ.get("JIRA_USER_NAME", None)
 JIRA_API_TOKEN = os.environ.get("JIRA_API_TOKEN", None)
 JIRA_URL = os.environ.get("JIRA_URL", None)
+
+LICENSE_KEY = os.environ.get("LICENSE_KEY", None)
+ALTERNATE_AWS = os.environ.get("ALTERNATE_AWS", "none").lower() == "true"
```

### Comparing `sweepai-2.0.2/sweepai/core/chat.py` & `sweepai-2.1.0/sweepai/core/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 import backoff
 from loguru import logger
 from pydantic import BaseModel
 
 from sweepai.agents.agent_utils import ensure_additional_messages_length
 from sweepai.config.client import get_description
 from sweepai.config.server import (
+    ALTERNATE_AWS,
     ANTHROPIC_AVAILABLE,
     AWS_ACCESS_KEY,
     AWS_REGION,
     AWS_SECRET_KEY,
     DEFAULT_GPT4_32K_MODEL,
     PAREA_API_KEY
 )
 from sweepai.core.entities import Message
 from sweepai.core.prompts import repo_description_prefix_prompt, system_message_prompt
 from sweepai.logn.cache import file_cache
 from sweepai.utils.anthropic_client import sanitize_anthropic_messages
 from sweepai.utils.chat_logger import ChatLogger
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import ClonedRepo
+from sweepai.utils.image_utils import create_message_with_images
 from sweepai.utils.openai_proxy import OpenAIProxy
 from sweepai.utils.prompt_constructor import HumanMessagePrompt
 from sweepai.utils.utils import Tiktoken
 from parea import Parea
 
 parea_client = None
 try:
@@ -45,14 +47,16 @@
 OpenAIModel = (
     Literal["gpt-3.5-turbo"]
     | Literal["gpt-3.5-turbo-1106"]
     | Literal["gpt-3.5-turbo-16k"]
     | Literal["gpt-3.5-turbo-16k-0613"]
     | Literal["gpt-4-1106-preview"]
     | Literal["gpt-4-0125-preview"]
+    | Literal["gpt-4-turbo-2024-04-09"]
+    | Literal["gpt-4-turbo"]
 )
 
 AnthropicModel = (
     Literal["claude-3-haiku-20240307"]
     | Literal["claude-3-sonnet-20240229"]
     | Literal["claude-3-opus-20240229"]
 )
@@ -170,14 +174,24 @@
             parameters = tool_call_parameters[tool_name]
             tool_call = { "tool": tool_name, 
                         "arguments": parse_function_call_parameters(tool_call_contents, parameters) 
                         }
             tool_calls.append(tool_call)
     return tool_calls
 
+# go through each message and see if we need to update it to include images or not
+def add_images_to_messages(message_dicts: list[dict[str, str]], images: list[tuple[str, str, str]], use_openai: bool = False):
+    if not images:
+        return message_dicts
+    new_message_dicts = []
+    for message in message_dicts:
+        new_message = create_message_with_images(message, images, use_openai=use_openai)
+        new_message_dicts.append(new_message)
+    return new_message_dicts
+
 class ChatGPT(MessageList):
     prev_message_states: list[list[Message]] = []
     model: ChatModel = DEFAULT_GPT4_32K_MODEL
     chat_logger: ChatLogger | None = None
     human_message: HumanMessagePrompt | None = None
     file_change_paths: list[str] = []
     cloned_repo: ClonedRepo | None = None
@@ -250,26 +264,27 @@
         content: str,
         model: ChatModel | None = None,
         message_key: str | None = None,
         temperature: float | None = None,
         max_tokens: int | None = None,
         stop_sequences: list[str] = [],
     ):
-        self.messages.append(Message(role="user", content=content, key=message_key))
+        self.messages.append(Message(role="user", content=content, key=message_key)) if content else None # supports calling assistant again
         model = model or self.model
         temperature = temperature or self.temperature or default_temperature
+        new_content = self.call_openai(
+            model=model,
+            temperature=temperature,
+            requested_max_tokens=max_tokens,
+            stop_sequences=stop_sequences,
+        )
         self.messages.append(
             Message(
                 role="assistant",
-                content=self.call_openai(
-                    model=model,
-                    temperature=temperature,
-                    requested_max_tokens=max_tokens,
-                    stop_sequences=stop_sequences,
-                ),
+                content=new_content,
                 key=message_key,
             )
         )
         self.prev_message_states.append(self.messages)
         return self.messages[-1].content
 
     @file_cache(ignore_params=["chat_logger", "cloned_repo"])
@@ -328,15 +343,15 @@
                 output = None
                 output = openai_proxy.call_openai(
                     model=model,
                     messages=self.messages_dicts,
                     max_tokens=max_tokens - token_sub,
                     temperature=temperature,
                     stop_sequences=stop_sequences,
-                ).choices[0].message.content
+                )
                 if self.chat_logger is not None:
                     self.chat_logger.add_chat(
                         {
                             "model": model,
                             "messages": self.messages_dicts,
                             "max_tokens": max_tokens - token_sub,
                             "temperature": temperature,
@@ -383,50 +398,56 @@
         assistant_message_content: str = "",
         model: ChatModel = "claude-3-haiku-20240307",
         message_key: str | None = None,
         temperature: float | None = None,
         stop_sequences: list[str] = [],
         max_tokens: int = 4096,
         use_openai: bool = False,
+        verbose: bool = True,
+        images: list[tuple[str, str, str]] | None = None
     ):
         # use openai
         if use_openai:
             OPENAI_API_KEY = os.environ.get("OPENAI_API_KEY")
             assert OPENAI_API_KEY
             self.model = 'gpt-4-turbo'
         else:
             ANTHROPIC_API_KEY = os.environ.get("ANTHROPIC_API_KEY")
             assert ANTHROPIC_API_KEY
             self.model = model
-        self.messages.append(Message(role="user", content=content, key=message_key))
+        if content:
+            self.messages.append(Message(role="user", content=content, key=message_key))
         if assistant_message_content:
             self.messages.append(Message(role="assistant", content=assistant_message_content))
         temperature = temperature or self.temperature or default_temperature
         messages_string = '\n\n'.join([message.content for message in self.messages])
-        logger.debug(f"Calling anthropic with model {model}\nMessages:{messages_string}\nInput:\n{content}")
+        if verbose:
+            logger.debug(f"Calling anthropic with model {model}\nMessages:{messages_string}\nInput:\n{content}")
         system_message = "\n\n".join([message.content for message in self.messages if message.role == "system"])
         content = ""
         e = None
-        NUM_ANTHROPIC_RETRIES = 4
+        NUM_ANTHROPIC_RETRIES = 6
+        use_aws = True
+        hit_content_filtering = False
         for i in range(NUM_ANTHROPIC_RETRIES):
             try:
-                @file_cache(redis=True) # must be in the inner scope because this entire function manages state
+                @file_cache(redis=True, ignore_contents=True) # must be in the inner scope because this entire function manages state
                 def call_anthropic(
                     message_dicts: list[dict[str, str]], 
                     system_message: str = system_message, 
                     model: str = model,
                     use_openai: bool = use_openai,
+                    use_aws: bool = True,
                 ) -> str: # add system message and model to cache
                     if use_openai:
                         client = OpenAI()
                     else:
-                        if ANTHROPIC_AVAILABLE:
+                        if ANTHROPIC_AVAILABLE and use_aws:
                             if "anthropic" not in model:
                                 model = f"anthropic.{model}-v1:0"
-                                self.model = f"anthropic.{self.model}-v1:0"
                             client = AnthropicBedrock(
                                 aws_access_key=AWS_ACCESS_KEY,
                                 aws_secret_key=AWS_SECRET_KEY,
                                 aws_region=AWS_REGION,
                             )
                         else:
                             client = Anthropic(api_key=ANTHROPIC_API_KEY)
@@ -440,22 +461,46 @@
                             model=model,
                             messages=self.messages_dicts,
                             max_tokens=max_tokens,
                             temperature=temperature,
                             stop=stop_sequences,
                         ).choices[0].message.content
                     else:
-                        response = client.messages.create(
-                            model=model,
-                            temperature=temperature,
-                            max_tokens=max_tokens,
-                            messages=message_dicts,
-                            system=system_message,
-                            stop_sequences=stop_sequences,
-                        ).content[0].text
+                        if ANTHROPIC_AVAILABLE and use_aws: # streaming doesn't work with AWS
+                            response = client.messages.create(
+                                model=model,
+                                messages=message_dicts,
+                                max_tokens=max_tokens,
+                                temperature=temperature,
+                                system=system_message,
+                                stop_sequences=stop_sequences,
+                            ).content[0].text
+                        else:
+                            verbose = True
+                            start_time = time.time()
+                            if verbose:
+                                print(f"In queue with model {model}...")
+                            with client.messages.stream(
+                                model=model,
+                                temperature=temperature,
+                                max_tokens=max_tokens,
+                                messages=message_dicts,
+                                system=system_message,  
+                                stop_sequences=stop_sequences,
+                            ) as stream:
+                                if verbose:
+                                    print(f"Started stream in {time.time() - start_time:.2f}s!")
+                                for i, text in enumerate(stream.text_stream):
+                                    if verbose:
+                                        if i == 0:
+                                            print(f"Time to first token: {time.time() - start_time:.2f}s")
+                                        print(text, end="", flush=True)
+                            response = stream.get_final_message().content[0].text
+                            if verbose:
+                                print("Done streaming results!")
                     return response
                 if use_openai:
                     message_dicts = [
                         {
                             "role": message.role,
                             "content": message.content,
                         } for message in self.messages
@@ -465,33 +510,44 @@
                     message_dicts = [
                         {
                             "role": message.role,
                             "content": message.content,
                         } for message in self.messages if message.role != "system"
                     ]
                     message_dicts = sanitize_anthropic_messages(message_dicts)
-                content = call_anthropic(message_dicts, self.messages[0].content, self.model, use_openai=use_openai)
+                # need to modify message dicts if we have images
+                if images:
+                    message_dicts = add_images_to_messages(message_dicts, images, use_openai=use_openai)
+                content = call_anthropic(message_dicts, self.messages[0].content, self.model, use_openai=use_openai, use_aws=use_aws)
                 break
             except BadRequestError as e_:
                 e = e_ # sometimes prompt is too long
-                raise e_
+                if not ALTERNATE_AWS:
+                    raise e_
+                elif hit_content_filtering: # hit it twice, raise error
+                    raise e_
+                else:
+                    hit_content_filtering = True # stop using anthropic
             except Exception as e_:
                 logger.exception(e_)
                 e = e_
-                time.sleep(4 * 2 ** i) # faster debugging
+                time.sleep(4 * 1.75 ** i) # faster debugging
+                if ALTERNATE_AWS: # alternate between aws and anthropic (for load balancing only)
+                    use_aws = not use_aws and not hit_content_filtering
         else:
             raise Exception("Anthropic call failed") from e
         self.messages.append(
             Message(
                 role="assistant",
                 content=content,
                 key=message_key,
             )
         )
-        logger.debug(f'{"Openai" if use_openai else "Anthropic"} response: {self.messages[-1].content}')
+        if verbose:
+            logger.debug(f'{"Openai" if use_openai else "Anthropic"} response: {self.messages[-1].content}')
         self.prev_message_states.append(self.messages)
         return self.messages[-1].content
 
     @property
     def messages_dicts(self):
         # Remove the key from the message object before sending to OpenAI
         cleaned_messages = [message.to_openai() for message in self.messages]
```

### Comparing `sweepai-2.0.2/sweepai/core/context_pruning.py` & `sweepai-2.1.0/sweepai/core/context_pruning.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,14 +168,27 @@
 def escape_ripgrep(text):
     # Special characters to escape
     special_chars = ["(", "{"]
     for s in special_chars:
         text = text.replace(s, "\\" + s)
     return text
 
+def run_ripgrep_command(code_entity, repo_dir):
+    rg_command = [
+        "rg",
+        "-n",
+        "-i",
+        code_entity,
+        repo_dir,
+    ]
+    result = subprocess.run(
+        " ".join(rg_command), text=True, shell=True, capture_output=True
+    )
+    return result.stdout
+
 @staticmethod
 def can_add_snippet(snippet: Snippet, current_snippets: list[Snippet]):
     return (
         len(snippet.xml) + sum([len(snippet.xml) for snippet in current_snippets])
         <= ASSISTANT_MAX_CHARS
     )
 
@@ -185,14 +198,15 @@
     dir_obj: DirectoryTree
     current_top_tree: str
     snippets: list[Snippet]
     snippet_scores: dict[str, float]
     cloned_repo: ClonedRepo
     current_top_snippets: list[Snippet] = field(default_factory=list)
     read_only_snippets: list[Snippet] = field(default_factory=list)
+    test_current_top_snippets: list[Snippet] = field(default_factory=list)
     issue_report_and_plan: str = ""
     import_trees: str = ""
     relevant_file_paths: list[str] = field(
         default_factory=list
     )  # a list of file paths that appear in the user query
 
     @property
@@ -276,19 +290,22 @@
         return highest_scoring_snippet
 
     def add_snippets(self, snippets_to_add: list[Snippet]):
         # self.dir_obj.add_file_paths([snippet.file_path for snippet in snippets_to_add])
         for snippet in snippets_to_add:
             self.current_top_snippets.append(snippet)
 
-    # does the same thing as add_snippets but adds it to the beginning of the list
-    def boost_snippets_to_top(self, snippets_to_boost: list[Snippet]):
+    def boost_snippets_to_top(self, snippets_to_boost: list[Snippet], code_files_in_query: list[str]):
         # self.dir_obj.add_file_paths([snippet.file_path for snippet in snippets_to_boost])
         for snippet in snippets_to_boost:
-            self.current_top_snippets.insert(0, snippet)
+            # get first positions of all snippets that are in the code_files_in_query
+            all_first_in_query_positions = [self.top_snippet_paths.index(file_path) for file_path in code_files_in_query if file_path in self.top_snippet_paths]
+            last_mentioned_result_index = (max(all_first_in_query_positions, default=-1) + 1) if all_first_in_query_positions else 0
+            # insert after the last mentioned result
+            self.current_top_snippets.insert(max(0, last_mentioned_result_index), snippet)
 
     def add_import_trees(self, import_trees: str):
         self.import_trees += "\n" + import_trees
 
     def append_relevant_file_paths(self, relevant_file_paths: str):
         # do not use append, it modifies the list in place and will update it for ALL instances of RepoContextManager
         self.relevant_file_paths = self.relevant_file_paths + [relevant_file_paths]
@@ -515,15 +532,15 @@
         ]
         # if our mentioned code file isnt already in the current_top_snippets we add it
         if file not in current_top_snippet_paths:
             try:
                 code_snippets = [
                     snippet for snippet in rcm.snippets if snippet.file_path == file
                 ]
-                rcm.boost_snippets_to_top(code_snippets)
+                rcm.boost_snippets_to_top(code_snippets, code_files_in_query)
             except Exception as e:
                 logger.error(
                     f"Tried to add code file found in query but recieved error: {e}, skipping and continuing to next one."
                 )
     return rcm
 
 def generate_import_graph_text(graph):
@@ -744,26 +761,16 @@
     output = ""
     current_top_snippets_string = "\n".join(
         list(dict.fromkeys([snippet.file_path for snippet in repo_context_manager.current_top_snippets]))
     )
     if function_name == "code_search":
         code_entity = f'"{function_input["code_entity"]}"'  # handles cases with two words
         code_entity = escape_ripgrep(code_entity) # escape special characters
-        rg_command = [
-            "rg",
-            "-n",
-            "-i",
-            code_entity,
-            repo_context_manager.cloned_repo.repo_dir,
-        ]
         try:
-            result = subprocess.run(
-                " ".join(rg_command), text=True, shell=True, capture_output=True
-            )
-            rg_output = result.stdout
+            rg_output = run_ripgrep_command(code_entity, repo_context_manager.cloned_repo.repo_dir)
             if rg_output:
                 # post process rip grep output to be more condensed
                 rg_output_pretty, file_output_dict, file_to_num_occurrences = post_process_rg_output(
                     repo_context_manager.cloned_repo.repo_dir, SweepConfig(), rg_output
                 )
                 # return results first by occurrences then by alphabetical order
                 non_stored_files = sorted([
```

### Comparing `sweepai-2.0.2/sweepai/core/entities.py` & `sweepai-2.1.0/sweepai/core/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,14 +357,15 @@
     Start and end refer to line numbers
     """
 
     content: str = Field(repr=False)
     start: int
     end: int
     file_path: str
+    score: float = 0.0 # TODO: migrate all usages to use this
 
     def __eq__(self, other):
         if isinstance(other, Snippet):
             return (
                 self.file_path == other.file_path
                 and self.start == other.start
                 and self.end == other.end
@@ -453,14 +454,15 @@
 
     def expand(self, num_lines: int = 25):
         return Snippet(
             content=self.content,
             start=max(self.start - num_lines, 1),
             end=min(self.end + num_lines, self.content.count("\n") + 1),
             file_path=self.file_path,
+            score=self.score,
         )
 
     @property
     def denotation(self):
         return f"{self.file_path}:{self.start}-{self.end}"
```

### Comparing `sweepai-2.0.2/sweepai/core/external_searcher.py` & `sweepai-2.1.0/sweepai/core/external_searcher.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/core/lexical_search.py` & `sweepai-2.1.0/sweepai/core/lexical_search.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/core/post_merge.py` & `sweepai-2.1.0/sweepai/core/post_merge.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/core/pr_reader.py` & `sweepai-2.1.0/sweepai/core/pr_reader.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/core/prompts.py` & `sweepai-2.1.0/sweepai/core/prompts.py`

 * *Files 16% similar despite different names*

```diff
@@ -175,182 +175,361 @@
 
 cot_retrieval_prompt = """
 Gather information to solve the problem. Use "finish" when you feel like you have sufficient information.
 """
 
 files_to_change_abstract_prompt = """Write an abstract minimum plan to address this issue in the least amount of change possible. Try to originate the root causes of this issue. Be clear and concise. 1 paragraph."""
 
-files_to_change_system_prompt = """You are an AI assistant helping an intern update code to resolve a GitHub issue. The user will provide code snippets, a description of the issue, and relevant parts of the codebase.
+files_to_change_system_prompt = """You are an AI assistant helping an intern write code to resolve a GitHub issue. The user will provide code files, a description of the issue, and relevant parts of the codebase.
+Your role is to analyze the issue and codebase, then provide a clear, step-by-step plan the intern can follow to make the necessary code changes to resolve the issue. Reference specific files, functions, variables and code files in your plan. Organize the steps logically and break them into small, manageable tasks.
+Prioritize using existing code and functions to make efficient and maintainable changes. Ensure your suggestions fully resolve the issue.
+
+Take these steps:
+1. Analyze the issue and codebase to understand the problem.
+
+2. Create a detailed plan for the intern to follow, including all necessary changes to resolve the issue.
+    - When modifying code you MUST do the following:
+        - Modify step 1. Copy the original code in <original_code> tags, copying them VERBATIM from the file. Do NOT paraphrase or abbreviate the source code. Placeholder comments like "# existing code" are not permitted.
+        - Modify step 2. Write the new code in <new_code> tags, specifying necessary imports and referencing relevant type definitions, interfaces, and schemas. BE EXACT as this code will replace the mentioned <original_code>.
 
-Your role is to analyze the issue and codebase, then provide a clear, step-by-step plan the intern can follow to make the necessary code changes to resolve the issue. Reference specific files, functions, variables and code snippets in your plan.
-
-Do not write out the full code changes, but rather give detailed natural language instructions and explanations the intern can follow to update the code themselves. Organize the steps logically and break them into small, manageable tasks.
-
-Prioritize using existing code and functions to make efficient and maintainable changes, while minimizing new code. Ensure your suggestions fully resolve the issue."""
+3. List all of the relevant files to reference while making changes, one per line."""
 
+# TODO: 2 paragraphs
+# the current issue analysis is heavily optimized, i'd like to try removing step d though
 files_to_change_prompt = """Your job is to write a high quality, detailed, step-by-step plan for an intern to help resolve a user's GitHub issue.
 
-You will analyze the provided code snippets, repository, and GitHub issue to understand the requested change. Create a step-by-step plan for an intern to fully resolve the user's GitHub issue. The plan should utilize the relevant code snippets and utility modules provided. Give detailed instructions for updating the code logic, as the intern is unfamiliar with the codebase.
+You will analyze the provided code files, repository, and GitHub issue to understand the requested change. Create a step-by-step plan for an intern to fully resolve the user's GitHub issue. The plan should utilize the relevant code files and utility modules provided. Give detailed instructions for updating the code logic, as the intern is unfamiliar with the codebase.
 
 Guidelines:
-- Always include the full file path and reference the provided snippets 
+- Always include the full file path and reference the provided files 
 - Provide clear instructions for updating the code, specifying necessary imports
-- Be specific and direct, using phrases like "add", "change", "remove" instead of vague terms
+- Be specific and direct, using the phrases "add", "replace", and "remove".
 - Reference relevant type definitions, interfaces, and schemas 
-- Avoid line numbers and instead reference code locations using surrounding code or function names
 - Ensure your plan is complete and covers all necessary changes to fully resolve the issue
 - Suggest high-quality, safe, maintainable, efficient and backwards compatible changes
 - Prioritize using existing code and utility methods to minimize writing new code
 - Break the task into small steps, with each <create> or <modify> section for each logical code block worth of change. Use multiple <modify> blocks for the same file if there are multiple distinct changes to make in that file.
+- To remove code, replace it with empty <new_code> tags.
 
 Please use the following XML format for your response:
 
-# Issue Analysis:
+# 1. Issue Analysis:
 <issue_analysis>
-* Identify the root cause of the issue by referencing specific code entities in the relevant files.
-* Outline ALL changes that need to occur for the user's request to be resolved, by referencing provided code snippets, entity names, and necessary files/directories.
-
-List ALL files we should modify to resolve the issue:
-- File path 1: Outline of instructions for modifying the file
-    - First change to make in the file
-    - Second change to make in the file
-- File path 2: Outline of instructions for modifying the file
-    - First change to make in the file
-    - Second change to make in the file
-[additional files as needed]
+a. Identify potential root causes of the issue by referencing specific code entities in the relevant files. Then, select which of the root causes the user is most likely to be interested in resolving based on the current state of the codebase. (1 paragraph)
 
-List ALL relevant read-only utility modules from the provided set and specify where they can be used. These are not files you need to make changes to but files you need to read while making changes in other files, including:
-- Type definitions, interfaces, and schemas
-- Helper functions
-- Frontend components
-- Database services
-- API endpoints
-[additional relevant modules as needed]
-
-* For each <create> or <modify> section in your plan, explain its purpose and how it contributes to resolving the issue.
-[additional analysis as needed]
-</issue_analysis>
+c. Detail ALL of the changes that need to be made to the codebase (excluding tests) to resolve the user request. Reference the provided code files, summaries, entity names, and necessary files/directories. Be complete and precise. (1 paragraph)
 
-Format:
-<issue_analysis>
-Identify the root cause of the issue referencing specific code in the relevant files. Outline ALL changes needed to resolve the user's request, referencing provided code snippets, entity names, and necessary files/directories. 
-
-List ALL files to modify:
-- File path 1: Outline of changes 
-- File path 2: Outline of changes
-[additional files]
-
-List ALL relevant read-only utility modules to reference:
-- Type definitions, interfaces, schemas
-- Helper functions 
-- Frontend components
-- Database services 
-- API endpoints
-[additional modules]
+d. List ALL of the files we should modify to resolve the issue. Reference the provided code files, summaries, entity names, and necessary files/directories. Respond in the following format:
+  - File path 1: Detailed instructions for modifying the file.
+      a. Describe the first change to make in the file.
+      b. Describe the second change to make in the file.
+      c. Continue listing all changes that need to be made. Be complete and precise.
+  - File path 2: Detailed instructions for modifying the file.
+      a. Describe the first change to make in the file.
+      b. Describe the second change to make in the file.
+      c. Continue listing all changes that need to be made. Be complete and precise.
+[additional files as needed]
 
-For each <create> or <modify> in the plan, explain its purpose for resolving the issue.
-[additional analysis]
+e. List ALL relevant read-only utility modules from the provided set and specify where they can be used. These are not files you need to make changes to but files you need to read while making changes in other files, including:
+  - Type definitions, interfaces, and schemas
+  - Helper functions
+  - Frontend components
+  - Database services
+  - API endpoints
+  [additional relevant modules as needed]
 </issue_analysis>
 
+# 2. Plan:
 <plan>  
 <create file="file_path_1">
-Instructions for creating the new file. Reference imports and entity names. Include relevant type definitions, interfaces, schemas.
+Detailed explanation of the contents of the new file. Reference imports and entity names. Include relevant type definitions, interfaces, and schemas.
+
+Then, write the new code in <new_code> tags:
+
+<new_code>
+All the new code required to be added to the file.
+</new_code>
 </create>
 [additional creates]
 
 <modify file="file_path_2"> 
-Instructions for modifying one section of the file. Reference change locations using surrounding code or functions, not line numbers. Include relevant type definitions, interfaces, schemas. Describe code changes without writing code.
+Instructions for modifying one section of the file. 
+
+1. Reference the original code in <original_code> tags, copying them VERBATIM from the file. Do NOT paraphrase or abbreviate the source code. Placeholder comments like "# existing code" are not permitted. This block must NOT be empty.
+
+2. Write the new code in <new_code> tags, specifying necessary imports and referencing relevant type definitions, interfaces, and schemas. BE EXACT as this code will replace the mentioned <original_code>.
+
+If imports are needed, they should be in a separate <modify> block. Use multiple <modify> blocks for the same file to separate distinct changes.
 </modify>
 
 <modify file="file_path_2">
-Instructions for modifying a different section of the same file. Use multiple <modify> blocks for the same file to separate distinct changes.
+Instructions for modifying a different section of the same file. 
+
+1. Reference the original code in <original_code> tags, copying them VERBATIM from the file. Do NOT paraphrase or abbreviate the source code. Placeholder comments like "# existing code" are not permitted. This block must NOT be empty.
+
+2. Write the new code in <new_code> tags, specifying necessary imports and referencing relevant type definitions, interfaces, and schemas. BE EXACT as this code will replace the mentioned <original_code>.
+
+Use multiple <modify> blocks for the same file to separate distinct changes.
 </modify>
 
 [additional modifies as needed, for the same file or different files]
 </plan>
 
+# 3. Relevant Modules:
 <relevant_modules>
 [List of all relevant files to reference while making changes, one per line] 
-</relevant_modules>
+</relevant_modules>""" # + files_to_change_example TODO: test separately
+
+fix_files_to_change_prompt = """You proposed plan a plan. However, your proposed plan has the following errors:
+
+<errors>
+{error_message}
+</errors>
+
+You must resolve these errors before proceeding. Respond in the following format:
+
+<error_resolutions>
+For each error, identify what went wrong and what the fix is. Analyze the contents of the provided file path to find the correct code block that needs to be modified. Update the <original_code> block with the actual code from the file, and then provide the necessary changes in the <new_code> block. Follow the format:
+
+<error_resolution>
+Error #0: Description of the error
+
+You will first think step-by-step about the error, and then either rewrite the instructions with the corrected fix, or drop the task.
+
+<thinking>
+Analyze extremely carefully in great detail what went wrong, including the file path and the specific code block that needs to be modified. If you have failed to copy code verbatim, indicate precisely what is different between the code you provided and the code in the actual file.
+</thinking>
+
+Then, let's resolve the errors in your proposed plan. If you would like patch the corresponding task of the plan, create a modify or create block with an index. The index should be equivalent to the error number of this error_resolution block. Otherwise, if you absolutely cannot resolve the error, drop the task. You must pick exactly ONE of the three options. Follow this format:
+
+Option a: To patch the error as a modify block, follow this format:
+
+<modify file="file_path" index="0">
+Rewritten instructions to resolve the error. Update the original_code and new_code blocks as required, ensuring that the <original_code> block contains the actual code from the file.
+
+Update <original_code> with the necessary changes:
+<original_code>
+The corrected code from the file verbatim. Abbreviating, missing indents, paraphrasing and placeholder code are NOT permitted. It is absolutely critical that the indentation is correct and matches the source code EXACTLY.
+</original_code>
 
-Here's an example of an excellent issue analysis and plan:
+Update <new_code> block with the necessary changes:
+<new_code>
+Updated new code, based on the corrections in <original_code>. Ensure all newly introduced indents and comments are propagated here.
+</new_code>
+</modify>
+
+Option b: To patch a task to create a file instead, create a create block like so:
+
+<create file="file_path">
+Instructions for creating the new file. Reference imports and entity names. Include relevant type definitions, interfaces, and schemas. You may only have one new_code block in this section.
+<new_code>
+All the new code required to be added to the file.
+</new_code>
+</create>
+
+Option c: Otherwise, if you absolutely cannot resolve the error, drop the task like so:
+
+<drop>Index of the task to drop</drop>
+</error_resolution>
+
+[additional <error_resolution> blocks as needed, for the same file or different files]
+</error_resolutions>
+
+Please resolve the errors in your proposed plan."""
+
+test_files_to_change_system_prompt = """You are an AI assistant helping an intern write tests to validate his code that aims to resolve a GitHub issue. The user will provide code files, a description of the issue, and relevant parts of the codebase.
+Your role is to analyze the issue and codebase, then provide a clear, step-by-step plan the intern can follow to make the necessary code changes to resolve the issue. Reference specific files, functions, variables and code files in your plan. Organize the steps logically and break them into small, manageable tasks.
+Prioritize using existing code and functions to make efficient and maintainable changes. Ensure your suggestions fully resolve the issue.
+
+Take these steps:
+1. Analyze the issue and codebase to understand the problem.
+
+2. Create a detailed plan for the intern to follow, including all necessary changes to resolve the issue.
+    - When modifying code you MUST do the following:
+        - Modify step 1. Copy the original code in <original_code> tags, copying them VERBATIM from the file. Do NOT paraphrase or abbreviate the source code. Placeholder comments like "# existing code" are not permitted.
+        - Modify step 2. Write the new code in <new_code> tags, specifying necessary imports and referencing relevant type definitions, interfaces, and schemas. BE EXACT as this code will replace the mentioned <original_code>.
+
+3. List all of the relevant files to reference while making changes, one per line."""
+
+test_files_to_change_prompt = """Now let's add tests to the code changes you made in the previous step. You will need to add or update tests to ensure that the changes you made are correct and do not break existing functionality.
+
+Please use the following XML format for your response:
 
+# 1. Issue Analysis:
 <issue_analysis>
-The root cause of the issue is that the `createPost` method in the `PostService` class (post_service.py) does not validate that the user submitting the post has a non-deleted account. It should check the `user.deleted` property and raise an exception if the user's account is deleted.
+a. Identify the functional changes made and locate the tests for the edited code. Respond in the following format:
 
-To completely resolve the user's request, we need to:
-- Modify the `createPost` method in post_service.py to check if the user's account is deleted before creating the post
-- Add a new exception class `DeletedAccountError` in exceptions.py to raise when a deleted user tries to create a post
-- Update the `create_post` endpoint in app.py to catch the new `DeletedAccountError` and return a 403 error response
-
-Relevant files to modify:
-- src/services/post_service.py
-  - Import the `User` entity and `DeletedAccountError` 
-  - Add validation to check if the user's account is deleted in `createPost`
-  - Raise `DeletedAccountError` if the user's account is deleted
-- src/exceptions.py
-  - Define a new exception class `DeletedAccountError`
-- src/app.py
-  - Import the new `DeletedAccountError`
-  - Catch `DeletedAccountError` in the `create_post` endpoint
-  - Return a 403 error response if `DeletedAccountError` is caught
-
-The relevant utility modules are:
-- `User` entity (src/entities/user.py) - to check if user's account is deleted 
-- `Post` entity (src/entities/post.py) - the entity being created in `createPost`
-
-The <create> and <modify> changes work together to fully handle preventing deleted users from creating posts:
-- The new exception class is created first to be used in the other changes
-- The service method is updated to validate the user and raise the new exception 
-- The API endpoint is updated to catch the new exception and return an appropriate error
+  - File path 1:
+    a. Identify the edited functions and classes.
+    b. Then, locate the tests for this module by checking for the most relevant test that imports the file in the <imports> section.
+    c. List and summarize all tests in each relevant test from step b. Then, identify the most similar tests we can copy with some minor edits. For example, if you need to test a functionality with a specific new feature, you can copy the test of the base functionality. Be as specific as possible. Follow the following format:
+
+First test name, which section it is located in, and which file it is from.
+```
+Copy of test code here
+```
+
+Second test name, which section it is located in, and which file it is from.
+```
+Copy of test code here
+```
+
+    d. Detail all of the tests that need to be added or updated to validate the changes. Reference the provided code files, summaries, entity names, and necessary files/directories. Be complete and precise. Follow the following format:
+      - First place to make a change or create a new test in extreme detail.
+      - Second place to make a change or create a new test in extreme detail.
+
+  - File path 2:
+    a. Identify the edited functions and classes.
+    b. Then, locate the tests for this module by checking for the most relevant test that imports the file in the <imports> section.
+    c. List and summarize all tests in each relevant test from step b. Then, identify the most similar tests we can copy with some minor edits. For example, if you need to test a functionality with a specific new feature, you can copy the test of the base functionality. Be as specific as possible. Follow the following format:
+
+First test name, which section it is located in, and which file it is from.
+```
+Copy of test code here
+```
+
+Second test name, which section it is located in, and which file it is from.
+```
+Copy of test code here
+```
+
+    d. Detail all of the tests that need to be added or updated to validate the changes. Reference the provided code files, summaries, entity names, and necessary files/directories. Be complete and precise. Follow the following format:
+      - First place to make a change or create a new test in extreme detail.
+      - Second place to make a change or create a new test in extreme detail.
+[additional files as needed]
+
+b. List ALL relevant read-only utility modules from the provided set and specify where they can be used. These are not files you need to make changes to but files you need to read while making changes in other tests, including:
+  - Relevant source code that we're testing
+  - Type definitions, interfaces, and schemas
+  - Helper functions
+  - Frontend components
+  - Database services
+  - API endpoints
+[additional relevant modules as needed]
 </issue_analysis>
 
-<plan>
-<create file="src/exceptions.py">
-* Define a new exception class called `DeletedAccountError`
-* Have it inherit from the base `Exception` class
-* Give it a clear error message indicating that a deleted account tried to perform an action
+# 2. Plan:
+<plan>  
+<create file="file_path_1">
+Instructions for creating the new file. Reference imports and entity names. Include relevant type definitions, interfaces, and schemas.
 </create>
+[additional creates]
 
-<modify file="src/services/post_service.py">
-At the top of the file:
-* Import the `User` entity from `src/entities/user.py`
-* Import the `DeletedAccountError` from `src/exceptions.py`
-
-In the `createPost` method of the `PostService` class:
-* After getting the `user` by ID, add an if statement to check:
-  - If `user.deleted` is True, raise a `DeletedAccountError`
-  - Otherwise, continue with creating the post as normal
-</modify>
+<modify file="file_path_2"> 
+One sentence explanation of the change. Instructions for modifying one section of the file.
+
+1. Reference the original code in <original_code> tags, copying them VERBATIM from the file. Do NOT paraphrase or abbreviate the source code. Placeholder comments like "# existing code" are not permitted. This block must NOT be empty.
 
-<modify file="src/services/post_service.py">
-In the `createPost` method of the `PostService` class:
-* After the line that creates the new `post` instance, add:
-  - A call to `self.post_repo.save(post)` to save the new post to the database
-  - A call to `self.logger.info(f"User {{user.id}} created a new post with id {{post.id}}")` to log the post creation
-* Return the newly created `post` instance
+2. Write the new code in <new_code> tags, specifying necessary imports and referencing relevant type definitions, interfaces, and schemas. BE EXACT as this code will replace the mentioned <original_code>.
 </modify>
 
-<modify file="src/app.py">
-At the top of the file: 
-* Import the `DeletedAccountError` from `src/exceptions.py`
-
-In the `create_post` endpoint:
-* Wrap the existing code in a try/except block
-* Catch the `DeletedAccountError` in the except block
-* If caught, return a JSON response with:
-  - A 403 status code
-  - An error message like "Cannot create post with a deleted account"
+<modify file="file_path_2">
+One sentence explanation of the change. Instructions for modifying one section of the file.
+
+1. Reference the original code in <original_code> tags, copying them VERBATIM from the file. Do NOT paraphrase or abbreviate the source code. Placeholder comments like "# existing code" are not permitted. This block must NOT be empty.
+
+2. Write the new code in <new_code> tags, specifying necessary imports and referencing relevant type definitions, interfaces, and schemas. BE EXACT as this code will replace the mentioned <original_code>.
+
+Use multiple <modify> blocks for the same file to separate distinct changes.
 </modify>
+
+[additional modifies as needed, for the same file or different files]
 </plan>
 
+# 3. Relevant Modules:
 <relevant_modules>
-src/entities/user.py
-src/entities/post.py
-</relevant_modules>"""
+[List of all relevant files to reference while making changes, one per line] 
+</relevant_modules>""" # + files_to_change_example TODO: test separately
+
+gha_files_to_change_system_prompt = """You are an AI assistant helping an intern write a plan to fix failing errors in his code. The intern will provide code files, a description of the issue, the error log, relevant parts of the codebase, and the changes he's made. You may only modify code files to resolve the issue.
+
+Your role is to analyze the issue and codebase, then provide a clear, step-by-step plan the intern can follow to make the necessary code changes to fix the errors. Reference specific files, functions, variables and code files in your plan. Organize the steps logically and break them into small, manageable tasks.
+Prioritize using existing code and functions to make efficient and maintainable changes. Ensure your suggestions fully resolve the issue.
+
+Take these steps:
+1. Analyze the issue, errors, codebase and existing changes to understand the problem.
+
+2. Create a detailed plan for the intern to follow, including all necessary changes to resolve the issue.
+    - When modifying code you MUST take the following approach:
+        Step 1. Reference the original code in <original_code> tags, copying them VERBATIM from the file, with correct indentation and whitespace.
+            - Do NOT paraphrase or abbreviate the source code.
+            - Placeholder comments like "# existing code" are not permitted.
+            - Start with a function header.
+        Step 2. Write the new code in <new_code> tags, specifying necessary imports and including relevant type definitions, interfaces, and schemas.
+            - BE EXACT as this code will replace the mentioned <original_code>.
+        Step 3. Determine if this is a change that occurs EXACTLY in other parts of the same file. If so, add a <replace_all>true</replace_all> flag.
+
+3. List all of the relevant files to reference while making changes, one per line."""
+
+gha_files_to_change_prompt = """Your job is to write a high quality, detailed, step-by-step plan for an intern to help resolve the errors in his code while also resolving the GitHub issue.
+
+You will analyze the provided issue, error log, relevant parts of the codebase, and changes he's made to understand the requested change. Create a step-by-step plan for an intern to fully resolve the user's GitHub issue. The plan should utilize the relevant code files and utility modules provided. Give detailed instructions for updating the code logic, as the intern is unfamiliar with the codebase.
+
+Guidelines:
+- Always include the full file path and reference the provided files 
+- Provide clear instructions for updating the code, specifying necessary imports
+- Reference relevant type definitions, interfaces, and schemas 
+- Ensure your plan is complete and covers all necessary changes to fully resolve the issue
+- Suggest high-quality, safe, maintainable, efficient and backwards compatible changes
+- Prioritize using existing code and utility methods to minimize writing new code
+- To remove code, replace it with empty <new_code> tags.
+- Break the task into small steps, with each <create> or <modify> section for each logical code block worth of change. Use multiple <modify> blocks for the same file if there are multiple distinct changes to make in that file. However, if a particular change is repeated exactly across an entire file, use <replace_all>true</replace_all>.
+- Do not make a change that has already been made by the intern.
+
+Please use the following XML format for your response:
+
+# 1. Thinking:
+<thinking>
+a. Summarize what the original GitHub issue is and asks us to do.
+
+b. List ALL the changes made so far in extreme detail. Be absolutely complete. Follow this format:
+    - File path 1:
+        - Description of first diff hunk in extreme detail.
+        - Description of second diff hunk in extreme detail.
+        [additional changes as needed]
+    - File path 2:
+        - Description of first diff hunk in extreme detail.
+        - Description of second diff hunk in extreme detail.
+        [additional changes as needed]
+    [additional files as needed]
+</thinking>
+
+# 2. Plan:
+<plan>  
+List ALL the types of error messages in the error logs and their root causes. Follow this format:
+
+There are a total of X errors in the error logs:
+
+<error_analysis index="1">
+Error message 1: Copy the full error message here VERBOSE, abbreviations, paraphrasing, ellipses, and placeholder comments are not permitted.
+- Count the number of occurrences of this error and list all of the particular tests that raised it.
+- Identify the root cause of the error, i.e. whether the error is due to a missing change in the tests or the source code. Most of the time, the test case has yet to be updated.
+- Explain how to resolve the error in the test case. Be complete and precise.
+- Indicate whether this exact fix is required in multiple places in the same file.
+
+Then, based on the analysis, propose a fix by following the format below. If the error has already been fixed, you can skip this step.
+
+<modify file="file_path"> 
+Instructions for modifying one section of the file. Each block must have exactly one original_code and one new_code block. Do not make a change that has already been made by the intern.
+
+a. Describe the section of code that needs to be modified, i.e. the test case that checks if `foo` == `bar`.
+<original_code>
+Copy the original_code here VERBATIM from the file. Do NOT paraphrase or abbreviate the source code. Placeholder comments like "# existing code" are not permitted. Start with a function header.
+</original_code>
+
+b. Describe the changes that need to be made to the code, i.e. the test case should instead check if `foo` != `baz`.
+<new_code>
+Write the new code in <new_code> tags, specifying necessary imports and referencing relevant type definitions, interfaces, and schemas. BE EXACT as this code will replace the mentioned <original_code>.
+</new_code>
+
+c. (Optional) Identify whether this is a change that needs to be applied exactly in other places of this file. If so, add <replace_all>true</replace_all> to replace all instances of the <original_code> in the file with the <new_code>.
+</modify>
+</error_analysis>
+[additional <error_analysis> blocks as needed, for ALL error messages in the error logs]
+</plan>""" # + files_to_change_example TODO: test separately
 
 plan_selection_prompt = """Critique the pros and cons of each plan based on the following guidelines, prioritizing thoroughness and correctness over potential performance overhead: 
 - Correctness: The code change should fully address the original issue or requirement without introducing new bugs, security vulnerabilities, or performance problems. Follow defensive programming practices, such as avoiding implicit assumptions, validating inputs, and handling edge cases. Consider the potential impact on all relevant data structures and ensure the solution maintains data integrity and consistency. Thoroughness is a top priority. 
 - Backwards Compatibility: When possible, avoid breaking changes to public APIs, data formats, or behaviors that existing code depends on. 
 - Clarity: The code change should be readable, well-structured, and easy for other developers to understand and maintain. Follow existing conventions and style guides, and include documentation and comments for complex or non-obvious logic. 
 - Simplicity: Strive for a solution that is as simple as possible while still being complete and correct. Favor straightforward and easily understandable code. Performance overhead should not be a factor in evaluating simplicity. 
 - Integration: Assess how well the change fits with the overall architecture and design of the system. Avoid tightly coupling components or introducing new dependencies that could complicate future development or deployment. After evaluating the plans against these criteria, select the one that provides the most thorough and correct solution within the specific context and constraints of the project. Prioritize long-term maintainability and architectural integrity.
@@ -370,74 +549,62 @@
 ...
 <modify file="anotherexamplefile.py">
 [More example instructions here]
 </modify>
 [Your explanation of why this plan was chosen and how it aligns with the guidelines and any modications made to this plan]
 </final_plan>"""
 
-context_files_to_change_prompt = """Your job is to write a high quality, detailed, step-by-step plan for an intern to help resolve a user's GitHub issue.
+context_files_to_change_system_prompt = """You are an AI assistant helping an intern plan the resolution to a GitHub issue. Code files, a description of the issue, and relevant parts of the codebase have been provided. List all of the relevant files to reference while making changes, one per line."""
 
-You will analyze the provided code snippets, repository, and GitHub issue to understand the requested change. Create a step-by-step plan for an intern to fully resolve the user's GitHub issue. The plan should utilize the relevant code snippets and utility modules provided. Give detailed instructions for updating the code logic, as the intern is unfamiliar with the codebase.
+context_files_to_change_prompt = """Your job is to write two high quality approaches for an intern to help resolve a user's GitHub issue. 
 
-Guidelines:
-- Always include the full file path and reference the provided snippets 
-- Provide clear instructions for updating the code, specifying necessary imports
-- Be specific and direct, using phrases like "add", "change", "remove" instead of vague terms
-- Reference relevant type definitions, interfaces, and schemas 
-- Avoid line numbers and instead reference code locations using surrounding code or function names
-- Ensure your plan is complete and covers all necessary changes to fully resolve the issue
-- Suggest high-quality, safe, maintainable, efficient and backwards compatible changes
-- Prioritize using existing code and utility methods to minimize writing new code
-- Break the task into small steps, with each <create> or <modify> section for each logical code block worth of change. Use multiple <modify> blocks for the same file if there are multiple distinct changes to make in that file.
+Follow the below steps:
+1. Identify the root cause of the issue by referencing specific code entities in the relevant files. (1 paragraph)
 
-Please use the following XML format for your response:
-
-# Issue Analysis:
-<issue_analysis>
-Identify the root cause of the issue referencing specific code in the relevant files. Outline ALL changes needed to resolve the user's request, referencing provided code snippets, entity names, and necessary files/directories. 
-
-List ALL files to modify:
-- File path 1: Outline of changes 
-- File path 2: Outline of changes
-[additional files]
-
-List ALL relevant read-only utility modules to reference:
-- Type definitions, interfaces, schemas
-- Helper functions 
-- Frontend components
-- Database services 
-- API endpoints
-[additional modules]
-
-For each <create> or <modify> in the plan, explain its purpose for resolving the issue.
-[additional analysis]
-</issue_analysis>
-
-<plan number="#">
-<create file="file_path_1">
-Instructions for creating the new file. Reference imports and entity names. Include relevant type definitions, interfaces, schemas.
-</create>
-[additional creates]
-
-<modify file="file_path_2"> 
-Instructions for modifying one section of the file. Reference change locations using surrounding code or functions, not line numbers. Include relevant type definitions, interfaces, schemas. Describe code changes without writing code.
-</modify>
-
-<modify file="file_path_2">
-Instructions for modifying a different section of the same file. Use multiple <modify> blocks for the same file to separate distinct changes.
-</modify>
+2. Plan two possible solutions to the user's request, prioritizing changes that use different files in the codebase. List them below as follows:
+    - Plan 1: The most likely solution to the issue. Reference the provided code files, summaries, entity names, and necessary files/directories.
+    - Plan 2: The second most likely solution to the issue. Reference the provided code files, summaries, entity names, and necessary files/directories.
+
+3. List all tests that may need to be added or updated to validate the changes given the two approaches. Follow the following format:
+    - Plan 1:
+        - File path 1: Detailed description of functionality we need to test in file path 1
+            a. Identify where the functionality will take place.
+            b. Check the <imports> section to find the most relevant test that imports file path 1 to identify where the existing tests for this are located.
+        - File path 2: Detailed description of functionality we need to test in file path 2
+            a. Identify where the functionality will take place.
+            b. Check the <imports> section to find the most relevant test that imports file path 2 to identify where the existing tests for this are located.
+        [additional files as needed]
+    - Plan 2:
+        - File path 1: Detailed description of functionality we need to test in file path 1
+            a. Identify where the functionality will take place.
+            b. Check the <imports> section to find the most relevant test that imports file path 1 to identify where the existing tests for this are located.
+        - File path 2: Detailed description of functionality we need to test in file path 2
+            a. Identify where the functionality will take place.
+            b. Check the <imports> section to find the most relevant test that imports file path 2 to identify where the existing tests for this are located.
+        [additional files as needed]
+
+4a. List all files, including tests, that may need to be modified to resolve the issue given the two approaches.
+
+- These files must be formatted in <relevant_files> tags like so:
+<relevant_files>
+file_path_1
+file_path_2
+...
+</relevant_files>
 
-[additional modifies as needed, for the same file or different files]
-</plan>
+4b. List all relevant read-only files from the provided set given the two approaches.
 
-<relevant_modules>
-[List of all relevant files to reference while making changes, one per line] 
-</relevant_modules>
+- These files must be formatted in <read_only_files> tags like so:
+<read_only_files>
+file_path_1
+file_path_2
+...
+</read_only_files>
 
-Generate three diverse plans to address the user issue based off of your issue analysis. The best plan will be chosen later."""
+Generate two different plans to address the user issue. The best plan will be chosen later."""
 
 extract_files_to_change_prompt = """\
 # Task:
 Create a plan that resolves the user's query and ONLY the user's query under "Issue Title" and "Issue Description", providing your response in the below format:
 <contextual_request_analysis>
 Review each function of each relevant_snippet and analyze the user request to determine if this change should use the refactor or unit test tools.
 The refactor tool performs code transformations in a single file without making other logical changes. Determine the function(s) that are too long and should have it's individual parts extracted.
```

### Comparing `sweepai-2.0.2/sweepai/core/reflection_utils.py` & `sweepai-2.1.0/sweepai/core/reflection_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,24 +419,21 @@
         content = formatted_problem_statement + formatted_plan + changed_files_section + formatted_patch_and_contents
         if warning_message:
             content += f"The changes also trigger the following warnings:\n<warnings>\n{warning_message}\n</warnings>\n\n"
         content += current_task
         if previous_attempt:
             content += "\n\n" + previous_attempt
         content += "\n\n" + modify_eval_suffix_prompt
-        # if warning_message:
-        #     breakpoint()
         evaluate_response = self.chat_anthropic(
             content=content,
             stop_sequences=["</message_to_contractor>"],
             model=CLAUDE_MODEL,
             message_key="user_request",
         )
         evaluate_response += "</message_to_contractor>" # add the stop sequence back in, if it stopped for another reason we've crashed
-        # breakpoint()
         # update chat_logger_messages in place if they are passed in
         if chat_logger_messages:
             chat_logger_messages.append({"role": "assistant", "content": content})
             chat_logger_messages.append({"role": "user", "content": evaluate_response})
         next_step = None
         feedback = ""
         try:
```

### Comparing `sweepai-2.0.2/sweepai/core/repo_parsing_utils.py` & `sweepai-2.1.0/sweepai/core/repo_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/core/update_prompts.py` & `sweepai-2.1.0/sweepai/core/update_prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/core/vector_db.py` & `sweepai-2.1.0/sweepai/core/vector_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from sweepai.utils.hash import hash_sha256
 from sweepai.utils.openai_proxy import get_embeddings_client
 from sweepai.utils.utils import Tiktoken
 
 # Now uses Voyage AI if available, with asymmetric embedding
 # CACHE_VERSION = "v2.0.04" + "-voyage" if VOYAGE_API_KEY else ""
 suffix = "-voyage-aws" if VOYAGE_API_USE_AWS else "-voyage" if VOYAGE_API_KEY else ""
-CACHE_VERSION = "v2.0.07" + suffix 
+CACHE_VERSION = "v2.0.08" + suffix 
 redis_client: Redis = Redis.from_url(REDIS_URL)  # TODO: add lazy loading
 tiktoken_client = Tiktoken()
 
 
 def cosine_similarity(a, B):
     """
     Updated to handle multi-queries.
```

### Comparing `sweepai-2.0.2/sweepai/handlers/create_pr.py` & `sweepai-2.1.0/sweepai/handlers/create_pr.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,16 @@
             changed_file,
             commit,
             file_change_requests,
         ) in sweep_bot.change_files_in_github_iterator(
             file_change_requests,
             pull_request.branch_name,
             blocked_dirs,
-            additional_messages=additional_messages
+            additional_messages=additional_messages,
+            username=username
         ):
             completed_count += len(new_file_contents or [])
             logger.info(f"Completed {completed_count}/{fcr_count} files")
             yield new_file_contents, changed_file, commit, file_change_requests
         if completed_count == 0 and fcr_count != 0:
             logger.info("No changes made")
             posthog.capture(
```

### Comparing `sweepai-2.0.2/sweepai/handlers/on_button_click.py` & `sweepai-2.1.0/sweepai/handlers/on_button_click.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/handlers/on_button_click_test.py` & `sweepai-2.1.0/sweepai/handlers/on_button_click_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/handlers/on_check_suite.py` & `sweepai-2.1.0/sweepai/handlers/on_check_suite.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/handlers/on_comment.py` & `sweepai-2.1.0/sweepai/handlers/on_comment.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 from sweepai.config.client import get_blocked_dirs, get_documentation_dict
 from sweepai.config.server import (
     DEFAULT_GPT4_32K_MODEL,
     ENV,
     GITHUB_BOT_USERNAME,
     MONGODB_URI,
 )
-from sweepai.core.context_pruning import get_relevant_context
 from sweepai.core.entities import FileChangeRequest, MockPR, NoFilesException
 from sweepai.core.sweep_bot import SweepBot, get_files_to_change, validate_file_change_requests
 from sweepai.handlers.on_review import get_pr_diffs
 from sweepai.utils.chat_logger import ChatLogger
 from sweepai.utils.event_logger import posthog
-from sweepai.utils.github_utils import ClonedRepo, get_github_client
+from sweepai.utils.github_utils import ClonedRepo, get_github_client, sanitize_string_for_github
 from sweepai.utils.progress import TicketProgress
 from sweepai.utils.prompt_constructor import HumanMessageCommentPrompt
 from sweepai.utils.str_utils import BOT_SUFFIX, FASTER_MODEL_MESSAGE
 from sweepai.utils.ticket_utils import fire_and_forget_wrapper, prep_snippets
 
 num_of_snippets_to_query = 30
 total_number_of_snippet_tokens = 15_000
@@ -171,14 +170,15 @@
 
         item_to_react_to = None
         reaction = None
 
         bot_comment = None
 
         def edit_comment(new_comment: str) -> None:
+            new_comment = sanitize_string_for_github(new_comment)
             if bot_comment is not None:
                 bot_comment.edit(new_comment + BOT_SUFFIX)
 
         try:
             # Check if the PR is closed
             if pr.state == "closed":
                 return {"success": True, "message": "PR is closed. No event fired."}
@@ -267,20 +267,14 @@
             else:
                 try:
                     search_query = (comment).strip("\n")
                     formatted_query = (f"{comment}").strip("\n")
                     repo_context_manager = prep_snippets(
                         cloned_repo, search_query, TicketProgress(tracking_id="none")
                     )
-                    repo_context_manager = get_relevant_context(
-                        formatted_query,
-                        repo_context_manager,
-                        TicketProgress(tracking_id="none"),
-                        chat_logger=chat_logger,
-                    )
                     snippets = repo_context_manager.current_top_snippets
                     tree = str(repo_context_manager.dir_obj)
                     cloned_repo = repo_context_manager.cloned_repo
                 except Exception as e:
                     logger.error(traceback.format_exc())
                     raise e
             get_documentation_dict(repo)
@@ -310,28 +304,29 @@
                 human_message=human_message,
                 repo=repo,
                 chat_logger=chat_logger,
                 model=DEFAULT_GPT4_32K_MODEL,
                 cloned_repo=cloned_repo,
             )
         except Exception as e:
-            logger.error(traceback.format_exc())
+            stack_trace = traceback.format_exc()
+            logger.error(stack_trace)
             elapsed_time = time.time() - start_time
             posthog.capture(
                 username,
                 "failed",
                 properties={
                     "error": str(e),
-                    "reason": "Failed to get files",
+                    "reason": f"An error occured! The stack trace is below:\n\n{stack_trace}",
                     "duration": elapsed_time,
                     "tracking_id": tracking_id,
                     **metadata,
                 },
             )
-            edit_comment(ERROR_FORMAT.format(title="Failed to get files"))
+            edit_comment(ERROR_FORMAT.format(title=f"An error occured!\n\nThe exception message is:{str(e)}\n\nThe stack trace is:{stack_trace}"))
             raise e
 
         try:
             logger.info("Fetching files to modify/create...")
             if file_comment:
                 file_change_requests = [
                     FileChangeRequest(
@@ -343,15 +338,16 @@
                 ]
             else:
                 file_change_requests, plan = get_files_to_change(
                     relevant_snippets=repo_context_manager.current_top_snippets,
                     read_only_snippets=repo_context_manager.read_only_snippets,
                     problem_statement=formatted_query,
                     repo_name=repo_name,
-                    pr_diffs=pr_diff_string
+                    pr_diffs=pr_diff_string,
+                    cloned_repo=cloned_repo,
                 )
                 validate_file_change_requests(file_change_requests, repo_context_manager.cloned_repo)
                 file_change_requests = sweep_bot.validate_file_change_requests(
                     file_change_requests, branch=branch_name
                 )
 
             sweep_response = "I couldn't find any relevant files to change."
@@ -402,15 +398,14 @@
 
             if not isinstance(pr, MockPR):
                 if pr.user.login == GITHUB_BOT_USERNAME and pr.title.startswith(
                     "[DRAFT] "
                 ):
                     # Update the PR title to remove the "[DRAFT]" prefix
                     pr.edit(title=pr.title.replace("[DRAFT] ", "", 1))
-
             logger.info("Done!")
         except NoFilesException:
             elapsed_time = time.time() - start_time
             posthog.capture(
                 username,
                 "failed",
                 properties={
@@ -419,27 +414,28 @@
                     "duration": elapsed_time,
                     **metadata,
                 },
             )
             edit_comment(ERROR_FORMAT.format(title="Could not find files to change"))
             return {"success": True, "message": "No files to change."}
         except Exception as e:
-            logger.error(traceback.format_exc())
+            stack_trace = traceback.format_exc()
+            logger.error(stack_trace)
             elapsed_time = time.time() - start_time
             posthog.capture(
                 username,
                 "failed",
                 properties={
                     "error": str(e),
                     "reason": "Failed to make changes",
                     "duration": elapsed_time,
                     **metadata,
                 },
             )
-            edit_comment(ERROR_FORMAT.format(title="Failed to make changes"))
+            edit_comment(ERROR_FORMAT.format(title=f"Failed to make changes:\n\nThe exception message is:{str(e)}\n\nThe stack trace is:{stack_trace}"))
             raise e
 
         # Delete eyes
         if reaction is not None:
             item_to_react_to.delete_reaction(reaction.id)
 
         try:
```

### Comparing `sweepai-2.0.2/sweepai/handlers/on_jira_ticket.py` & `sweepai-2.1.0/sweepai/handlers/on_jira_ticket.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/handlers/on_merge.py` & `sweepai-2.1.0/sweepai/handlers/on_merge.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/handlers/on_merge_conflict.py` & `sweepai-2.1.0/sweepai/handlers/on_merge_conflict.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/handlers/on_review.py` & `sweepai-2.1.0/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/handlers/on_ticket.py` & `sweepai-2.1.0/sweepai/handlers/on_ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,66 +21,64 @@
 from github.Issue import Issue
 from github.PullRequest import PullRequest as GithubPullRequest
 from loguru import logger
 from tabulate import tabulate
 from tqdm import tqdm
 from yamllint import linter
 
+from sweepai.core.sweep_bot import GHA_PROMPT
 from sweepai.agents.pr_description_bot import PRDescriptionBot
+from sweepai.agents.image_description_bot import ImageDescriptionBot
 from sweepai.config.client import (
-    DEFAULT_RULES,
     RESET_FILE,
     RESTART_SWEEP_BUTTON,
     REVERT_CHANGED_FILES_TITLE,
-    RULES_LABEL,
-    RULES_TITLE,
-    SWEEP_BAD_FEEDBACK,
-    SWEEP_GOOD_FEEDBACK,
     SweepConfig,
     get_documentation_dict,
     get_gha_enabled,
-    get_rules,
 )
 from sweepai.config.server import (
     DEPLOYMENT_GHA_ENABLED,
-    DISCORD_FEEDBACK_WEBHOOK_URL,
     ENV,
     GITHUB_LABEL_NAME,
     IS_SELF_HOSTED,
     MONGODB_URI,
     PROGRESS_BASE_URL,
 )
-from sweepai.core.context_pruning import get_relevant_context
 from sweepai.core.entities import (
     AssistantRaisedException,
     FileChangeRequest,
     MaxTokensExceeded,
     NoFilesException,
     PullRequest,
     SandboxResponse,
 )
 from sweepai.core.entities import create_error_logs as entities_create_error_logs
 from sweepai.core.pr_reader import PRReader
-from sweepai.core.sweep_bot import SweepBot, get_files_to_change, validate_file_change_requests
+from sweepai.core.sweep_bot import SweepBot, get_files_to_change, get_files_to_change_for_gha, validate_file_change_requests
 from sweepai.handlers.create_pr import (
     create_config_pr,
     create_pr_changes,
     safe_delete_sweep_branch,
 )
 from sweepai.handlers.on_check_suite import clean_gh_logs
+from sweepai.utils.image_utils import get_image_contents_from_urls, get_image_urls_from_issue
+from sweepai.utils.issue_validator import validate_issue
+from sweepai.utils.validate_license import validate_license
 from sweepai.utils.buttons import Button, ButtonList, create_action_buttons
 from sweepai.utils.chat_logger import ChatLogger
 from sweepai.utils.diff import generate_diff
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import (
     CURRENT_USERNAME,
     ClonedRepo,
     convert_pr_draft_field,
     get_github_client,
     get_token,
+    sanitize_string_for_github,
 )
 from sweepai.utils.progress import (
     AssistantConversation,
     PaymentContext,
     TicketContext,
     TicketProgress,
     TicketProgressStatus,
@@ -164,15 +162,15 @@
 {github_action_log}
 """
 
 
 # Add :eyes: emoji to ticket
 def add_emoji(issue: Issue, comment_id: int = None, reaction_content="eyes"):
     item_to_react_to = issue.get_comment(comment_id) if comment_id else issue
-    item_to_react_to.create_reaction("eyes")
+    item_to_react_to.create_reaction(reaction_content)
 
 
 # If SWEEP_BOT reacted to item_to_react_to with "rocket", then remove it.
 def remove_emoji(issue: Issue, comment_id: int = None, content_to_delete="eyes"):
     item_to_react_to = issue.get_comment(comment_id) if comment_id else issue
     reactions = item_to_react_to.get_reactions()
     for reaction in reactions:
@@ -245,14 +243,19 @@
                             f"{job['name']}/{step['number']}_{step['name']}"
                         )
         else:
             logger.error(
                 "Failed to get jobs for failing github actions, possible a credentials issue"
             )
             return all_logs
+        # make sure jobs in valid
+        if jobs_response.json()['total_count'] == 0:
+            logger.error(f"no jobs for this run: {run}, continuing...")
+            continue
+
         # logs url
         logs_url = run.logs_url
         logs_response = requests.get(
             logs_url,
             headers={
                 "Accept": "application/vnd.github+json",
                 "Authorization": f"Bearer {token}",
@@ -270,15 +273,14 @@
                     logs = zip_file.read(f"{file}.txt").decode("utf-8")
                     logs_prompt = clean_gh_logs(logs)
                     all_logs += logs_prompt + "\n"
         else:
             logger.error(
                 "Failed to get logs for failing github actions, likely a credentials issue"
             )
-            return all_logs
     return all_logs
 
 
 def delete_old_prs(repo: Repository, issue_number: int):
     logger.info("Deleting old PRs...")
     prs = repo.get_pulls(
         state="open",
@@ -432,14 +434,16 @@
     repo_full_name: str,
     repo_description: str,
     installation_id: int,
     comment_id: int = None,
     edited: bool = False,
     tracking_id: str | None = None,
 ):
+    if not os.environ.get("CLI"):
+        assert validate_license(), "License key is invalid or expired. Please contact us at team@sweep.dev to upgrade to an enterprise license."
     with logger.contextualize(
         tracking_id=tracking_id,
     ):
         if tracking_id is None:
             tracking_id = get_hash()
         on_ticket_start_time = time()
         logger.info(f"Starting on_ticket with title {title} and summary {summary}")
@@ -448,15 +452,17 @@
             slow_mode,
             do_map,
             subissues_mode,
             sandbox_mode,
             fast_mode,
             lint_mode,
         ) = strip_sweep(title)
-
+        # fetch images from body of issue
+        image_urls = get_image_urls_from_issue(issue_number, repo_full_name, installation_id)
+        image_contents = get_image_contents_from_urls(image_urls)
         summary = summary or ""
         summary = re.sub(
             "<details (open)?>(\r)?\n<summary>Checklist</summary>.*",
             "",
             summary,
             flags=re.DOTALL,
         ).strip()
@@ -466,15 +472,14 @@
             summary,
             flags=re.DOTALL,
         ).strip()
         summary = re.sub(
             "### Details\n\n_No response_", "", summary, flags=re.DOTALL
         )
         summary = re.sub("\n\n", "\n", summary, flags=re.DOTALL)
-
         repo_name = repo_full_name
         user_token, g = get_github_client(installation_id)
         repo = g.get_repo(repo_full_name)
         current_issue: Issue = repo.get_issue(number=issue_number)
         assignee = current_issue.assignee.login if current_issue.assignee else None
         if assignee is None:
             assignee = current_issue.user.login
@@ -592,14 +597,17 @@
                 )
                 return {"success": False, "reason": "Issue is closed"}
 
             fire_and_forget_wrapper(add_emoji)(current_issue, comment_id)
             fire_and_forget_wrapper(remove_emoji)(
                 current_issue, comment_id, content_to_delete="rocket"
             )
+            fire_and_forget_wrapper(remove_emoji)(
+                current_issue, comment_id, content_to_delete="confused"
+            )
             fire_and_forget_wrapper(current_issue.edit)(body=summary)
 
             replies_text = ""
             summary = summary if summary else ""
 
             fire_and_forget_wrapper(delete_old_prs)(repo, issue_number)
 
@@ -657,14 +665,18 @@
                 )
                 if issue_comment is None:
                     issue_comment = current_issue.create_comment(
                         first_comment + BOT_SUFFIX
                     )
                 else:
                     issue_comment.edit(first_comment + BOT_SUFFIX)
+                fire_and_forget_wrapper(add_emoji)(
+                    current_issue, comment_id, reaction_content="confused"
+                )
+                fire_and_forget_wrapper(remove_emoji)(content_to_delete="eyes")
                 return {"success": False}
             indexing_message = (
                 "I'm searching for relevant snippets in your repository. If this is your first"
                 " time using Sweep, I'm indexing your repository. You can monitor the progress using the progress dashboard"
             )
             first_comment = (
                 f"{get_comment_header(0, g, repo_full_name, user_settings, progress_headers, tracking_id, payment_message_start, user_settings_message)}\n{sep}I am currently looking into this ticket! I"
@@ -700,14 +712,17 @@
                 message: str,
                 index: int,
                 pr_message="",
                 done=False,
                 add_bonus_message=True,
             ):
                 nonlocal current_index, user_token, g, repo, issue_comment, initial_sandbox_response, initial_sandbox_response_file
+                message = sanitize_string_for_github(message)
+                if pr_message:
+                    pr_message = sanitize_string_for_github(pr_message)
                 # -1 = error, -2 = retry
                 # Only update the progress bar if the issue generation errors.
                 errored = index == -1
                 if index >= 0:
                     past_messages[index] = message
                     current_index = index
 
@@ -785,37 +800,39 @@
                     username,
                     "ran_out_of_tickets",
                     properties={
                         **metadata,
                         "duration": round(time() - on_ticket_start_time),
                     },
                 )
+                fire_and_forget_wrapper(add_emoji)(
+                    current_issue, comment_id, reaction_content="confused"
+                )
+                fire_and_forget_wrapper(remove_emoji)(content_to_delete="eyes")
                 return {
                     "success": False,
                     "error_message": "We deprecated supporting GPT 3.5.",
                 }
-
-            if sandbox_mode:
-                handle_sandbox_mode(
-                    title, repo_full_name, repo, ticket_progress, edit_sweep_comment
-                )
-                return {"success": True}
-
-            if len(title + summary) < 20:
-                logger.info("Issue too short")
+            
+            error_message = validate_issue(title + summary)
+            if error_message:
+                logger.warning(f"Validation error: {error_message}")
                 edit_sweep_comment(
                     (
-                        f"Please add more details to your issue. I need at least 20 characters"
-                        f" to generate a plan. Please join our Discord server for support (tracking_id={tracking_id})"
+                        f"The issue was rejected with the following response:\n\n{blockquote(error_message)}"
                     ),
                     -1,
                 )
+                fire_and_forget_wrapper(add_emoji)(
+                    current_issue, comment_id, reaction_content="confused"
+                )
+                fire_and_forget_wrapper(remove_emoji)(content_to_delete="eyes")
                 posthog.capture(
                     username,
-                    "issue_too_short",
+                    "invalid_issue",
                     properties={
                         **metadata,
                         "duration": round(time() - on_ticket_start_time),
                     },
                 )
                 return {"success": True}
 
@@ -832,35 +849,38 @@
                     ),
                     1,
                 )
 
             try:
                 # search/context manager
                 logger.info("Searching for relevant snippets...")
+                if image_contents: # doing it here to avoid editing the original issue
+                    message_summary += ImageDescriptionBot().describe_images(text=title + message_summary, images=image_contents)
                 snippets, tree, _, repo_context_manager = fetch_relevant_files(
                     cloned_repo,
                     title,
                     message_summary,
                     replies_text,
                     username,
                     metadata,
                     on_ticket_start_time,
                     tracking_id,
                     is_paying_user,
                     is_consumer_tier,
                     issue_url,
                     chat_logger,
                     ticket_progress,
+                    images=image_contents
                 )
                 cloned_repo = repo_context_manager.cloned_repo
             except Exception as e:
                 edit_sweep_comment(
                     (
                         "It looks like an issue has occurred around fetching the files."
-                        " Perhaps the repo failed to initialized. If this error persists"
+                        f" The exception was {str(e)}. If this error persists"
                         f" contact team@sweep.dev.\n\n> @{username}, editing this issue description to include more details will automatically make me relaunch. Please join our Discord server for support (tracking_id={tracking_id})"
                     ),
                     -1,
                 )
                 raise Exception("Failed to fetch files") from e
             _user_token, g = get_github_client(installation_id)
             user_token, g, repo = refresh_token()
@@ -873,18 +893,14 @@
             ticket_progress.save()
 
             # Fetch git commit history
             if not repo_description:
                 repo_description = "No description provided."
 
             message_summary += replies_text
-            # removed external search as it provides no real value and only adds noise
-            # external_results = ExternalSearcher.extract_summaries(message_summary)
-            # if external_results:
-            #     message_summary += "\n\n" + external_results
 
             get_documentation_dict(repo)
             docs_results = ""
             sweep_bot = construct_sweep_bot(
                 repo=repo,
                 repo_name=repo_name,
                 issue_url=issue_url,
@@ -933,16 +949,14 @@
             # If sweep.yaml does not exist, then create a new PR that simply creates the sweep.yaml file.
             if not sweep_yml_exists:
                 try:
                     logger.info("Creating sweep.yaml file...")
                     config_pr = create_config_pr(sweep_bot, cloned_repo=cloned_repo)
                     config_pr_url = config_pr.html_url
                     edit_sweep_comment(message="", index=-2)
-                except SystemExit:
-                    raise SystemExit
                 except Exception as e:
                     logger.error(
                         "Failed to create new branch for sweep.yaml file.\n",
                         e,
                         traceback.format_exc(),
                     )
             else:
@@ -971,21 +985,22 @@
                         )
                         if prs_extracted
                         else ""
                     )
                     + (f"\n\n{docs_results}\n\n" if docs_results else ""),
                     1,
                 )
-
                 logger.info("Fetching files to modify/create...")
                 file_change_requests, plan = get_files_to_change(
                     relevant_snippets=repo_context_manager.current_top_snippets,
                     read_only_snippets=repo_context_manager.read_only_snippets,
-                    problem_statement=f"{title}\n\n{summary}",
+                    problem_statement=f"{title}\n\n{message_summary}",
                     repo_name=repo_full_name,
+                    cloned_repo=cloned_repo,
+                    images=image_contents
                 )
                 validate_file_change_requests(file_change_requests, cloned_repo)
                 ticket_progress.planning_progress.file_change_requests = (
                     file_change_requests
                 )
                 ticket_progress.coding_progress.file_change_requests = (
                     file_change_requests
@@ -1098,15 +1113,14 @@
 
                 current_issue = repo.get_issue(number=issue_number)
                 current_issue.edit(
                     body=summary + "\n\n" + condensed_checkboxes_collapsible
                 )
 
                 delete_branch = False
-
                 generator = create_pr_changes(
                     file_change_requests,
                     pull_request,
                     sweep_bot,
                     username,
                     installation_id,
                     issue_number,
@@ -1291,16 +1305,14 @@
                 change_location = f" [`{pr_changes.pr_head}`](https://github.com/{repo_full_name}/commits/{pr_changes.pr_head}).\n\n"
                 review_message = (
                     "Here are my self-reviews of my changes at" + change_location
                 )
 
                 try:
                     fire_and_forget_wrapper(remove_emoji)(content_to_delete="eyes")
-                except SystemExit:
-                    raise SystemExit
                 except Exception:
                     pass
 
                 changes_required, review_message = False, ""
                 if changes_required:
                     edit_sweep_comment(
                         review_message
@@ -1309,64 +1321,23 @@
                     )
                 else:
                     edit_sweep_comment(
                         f"I have finished reviewing the code for completeness. I did not find errors for {change_location}",
                         3,
                     )
 
-                pr_actions_message = (
-                    create_action_buttons(
-                        [
-                            SWEEP_GOOD_FEEDBACK,
-                            SWEEP_BAD_FEEDBACK,
-                        ],
-                        header="### PR Feedback (click)\n",
-                    )
-                    + "\n"
-                    if DISCORD_FEEDBACK_WEBHOOK_URL is not None
-                    else ""
-                )
                 revert_buttons = []
                 for changed_file in set(changed_files):
                     revert_buttons.append(
                         Button(label=f"{RESET_FILE} {changed_file}")
                     )
                 revert_buttons_list = ButtonList(
                     buttons=revert_buttons, title=REVERT_CHANGED_FILES_TITLE
                 )
 
-                rule_buttons = []
-                repo_rules = get_rules(repo) or []
-                if repo_rules != [""] and repo_rules != []:
-                    for rule in repo_rules or []:
-                        if rule:
-                            rule_buttons.append(
-                                Button(label=f"{RULES_LABEL} {rule}")
-                            )
-                    if len(repo_rules) == 0:
-                        for rule in DEFAULT_RULES:
-                            rule_buttons.append(
-                                Button(label=f"{RULES_LABEL} {rule}")
-                            )
-
-                rules_buttons_list = ButtonList(
-                    buttons=rule_buttons, title=RULES_TITLE
-                )
-
-                sandbox_passed = None
-                for file_change_request in file_change_requests:
-                    if file_change_request.change_type == "check":
-                        if (
-                            file_change_request.sandbox_response
-                            and file_change_request.sandbox_response.error_messages
-                        ):
-                            sandbox_passed = False
-                        elif sandbox_passed is None:
-                            sandbox_passed = True
-
                 # delete failing sweep yaml if applicable
                 if sweep_yml_failed:
                     try:
                         repo.delete_file(
                             "sweep.yaml",
                             "Delete failing sweep.yaml",
                             branch=pr_changes.pr_head,
@@ -1374,15 +1345,15 @@
                         )
                     except Exception:
                         pass
 
                 # create draft pr, then convert to regular pr later
                 pr: GithubPullRequest = repo.create_pull(
                     title=pr_changes.title,
-                    body=pr_actions_message + pr_changes.body,
+                    body=pr_changes.body,
                     head=pr_changes.pr_head,
                     base=overrided_branch_name or SweepConfig.get_branch(repo),
                     # removed draft PR
                     draft=False,
                 )
 
                 try:
@@ -1397,18 +1368,14 @@
                 ticket_progress.context.pr_id = pr.number
                 ticket_progress.save()
 
                 if revert_buttons:
                     pr.create_issue_comment(
                         revert_buttons_list.serialize() + BOT_SUFFIX
                     )
-                if rule_buttons:
-                    pr.create_issue_comment(
-                        rules_buttons_list.serialize() + BOT_SUFFIX
-                    )
 
                 # add comments before labelling
                 pr.add_to_labels(GITHUB_LABEL_NAME)
                 current_issue.create_reaction("rocket")
                 heres_pr_message = f'<h1 align="center">🚀 Here\'s the PR! <a href="{pr.html_url}">#{pr.number}</a></h1>'
                 progress_message = f'<div align="center"><b>See Sweep\'s progress at <a href="{PROGRESS_BASE_URL}/issues/{tracking_id}">the progress dashboard</a>!</b></div>'
                 edit_sweep_comment(
@@ -1465,29 +1432,30 @@
                 )
 
                 # poll for github to check when gha are done
                 total_poll_attempts = 0
                 total_edit_attempts = 0
                 SLEEP_DURATION_SECONDS = 15
                 GITHUB_ACTIONS_ENABLED = get_gha_enabled(repo=repo) and DEPLOYMENT_GHA_ENABLED
-                GHA_MAX_EDIT_ATTEMPTS = 1 # max number of times to edit PR
+                GHA_MAX_EDIT_ATTEMPTS = 5 # max number of times to edit PR
+                current_commit = pr.head.sha
                 while True and GITHUB_ACTIONS_ENABLED:
                     logger.info(
                         f"Polling to see if Github Actions have finished... {total_poll_attempts}"
                     )
                     # we wait at most 60 minutes
                     if total_poll_attempts * SLEEP_DURATION_SECONDS // 60 >= 60:
                         break
                     else:
                         # wait one minute between check attempts
                         total_poll_attempts += 1
                         from time import sleep
 
                         sleep(SLEEP_DURATION_SECONDS)
-                    runs = list(repo.get_workflow_runs(branch=pr.head.ref, head_sha=pr.head.sha))
+                    runs = list(repo.get_workflow_runs(branch=pr.head.ref, head_sha=current_commit))
                     # if all runs have succeeded, break
                     if all([run.conclusion == "success" for run in runs]):
                         break
                     # if any of them have failed we retry
                     if any([run.conclusion == "failure" for run in runs]):
                         failed_runs = [
                             run for run in runs if run.conclusion == "failure"
@@ -1504,55 +1472,55 @@
                                 repo_full_name,
                                 installation_id=installation_id,
                                 token=user_token,
                                 repo=repo,
                                 branch=pr.head.ref,
                             )
                             diffs = get_branch_diff_text(repo=repo, branch=pr.head.ref, base_branch=pr.base.ref)
-                            problem_statement = f"{title}\n{summary}\n{replies_text}"
-                            all_information_prompt = f"While trying to address the user request:\n<user_request>\n{problem_statement}\n</user_request>\n{failed_gha_logs}\nThese are the changes that were previously made:\n<diffs>\n{diffs}\n</diffs>\n\nFix the failing logs."
-                            
-                            repo_context_manager = prep_snippets(cloned_repo=cloned_repo, query=(title + summary + replies_text).strip("\n"), ticket_progress=ticket_progress) # need to do this, can use the old query for speed
-                            repo_context_manager = get_relevant_context(
-                                all_information_prompt,
-                                repo_context_manager,
-                                ticket_progress,
-                                chat_logger=chat_logger,
-                                import_graph=None,
-                                num_rollouts=1,
+                            problem_statement = f"{title}\n{message_summary}\n{replies_text}"
+                            all_information_prompt = GHA_PROMPT.format(
+                                problem_statement=problem_statement,
+                                github_actions_logs=failed_gha_logs,
+                                changes_made=diffs,
                             )
+                            
+                            repo_context_manager = prep_snippets(cloned_repo=cloned_repo, query=(title + message_summary + replies_text).strip("\n"), ticket_progress=ticket_progress) # need to do this, can use the old query for speed
                             sweep_bot: SweepBot = construct_sweep_bot(
                                 repo=repo,
                                 repo_name=repo_name,
                                 issue_url=issue_url,
                                 repo_description=repo_description,
                                 title="Fix the following errors to complete the user request.",
                                 message_summary=all_information_prompt,
                                 cloned_repo=cloned_repo,
                                 ticket_progress=ticket_progress,
                                 chat_logger=chat_logger,
                                 snippets=snippets,
                                 tree=tree,
                                 comments=comments,
                             )
-                            file_change_requests, plan = get_files_to_change(
+                            file_change_requests, plan = get_files_to_change_for_gha(
                                 relevant_snippets=repo_context_manager.current_top_snippets,
                                 read_only_snippets=repo_context_manager.read_only_snippets,
                                 problem_statement=all_information_prompt,
-                                repo_name=repo_full_name,
+                                updated_files=new_file_contents,
+                                cloned_repo=cloned_repo,
+                                chat_logger=chat_logger,
                             )
                             validate_file_change_requests(file_change_requests, cloned_repo)
                             previous_modify_files_dict: dict[str, dict[str, str | list[str]]] | None = None
-                            sweep_bot.handle_modify_file_main(
+                            _, commit, _ = sweep_bot.handle_modify_file_main(
                                 branch=pr.head.ref,
                                 assistant_conversation=None,
                                 additional_messages=[],
                                 previous_modify_files_dict=previous_modify_files_dict,
-                                file_change_requests=file_change_requests
+                                file_change_requests=file_change_requests,
+                                username=username
                             )
+                            current_commit = commit.sha
                             pr = repo.get_pull(pr.number) # IMPORTANT: resync PR otherwise you'll fetch old GHA runs
                             total_edit_attempts += 1
                             if total_edit_attempts >= GHA_MAX_EDIT_ATTEMPTS:
                                 logger.info(f"Tried to edit PR {GHA_MAX_EDIT_ATTEMPTS} times, giving up.")
                                 break
                     # if none of the runs have completed we wait and poll github
                     logger.info(
@@ -1611,16 +1579,17 @@
                     str(e) + "\n" + traceback.format_exc(),
                     priority=2,
                 )
                 edit_sweep_comment(
                     (
                         "Sorry, Sweep could not find any appropriate files to edit to address"
                         " this issue. If this is a mistake, please provide more context and Sweep"
-                        f" will retry!\n\n> @{username}, please edit the issue description to"
-                        " include more details about this issue."
+                        f" will retry!\n\n@{username}, please edit the issue description to"
+                        " include more details. You can also ask for help on our community" 
+                        " forum: https://community.sweep.dev/"
                     ),
                     -1,
                 )
                 delete_branch = True
                 raise e
             except openai.BadRequestError as e:
                 ticket_progress.status = TicketProgressStatus.ERROR
@@ -1688,26 +1657,26 @@
 
                 logger.error(traceback.format_exc())
                 logger.error(e)
                 # title and summary are defined elsewhere
                 if len(title + summary) < 60:
                     edit_sweep_comment(
                         (
-                            "I'm sorry, but it looks like an error has occurred due to"
-                            + " a planning failure. Feel free to add more details to the issue description"
-                            + " so Sweep can better address it. Alternatively, reach out to Kevin or William for help at"
-                            + " https://discord.gg/sweep."
+                            "I'm sorry, but it looks like an error occurred due to" 
+                            f" a planning failure. The error message is {str(e)}. Feel free to add more details to the issue description"
+                            " so Sweep can better address it. Alternatively, post on our community forum"
+                            " for assistance: https://community.sweep.dev/"
                         ),
                         -1,
-                    )
+                    )  
                 else:
                     edit_sweep_comment(
                         (
                             "I'm sorry, but it looks like an error has occurred due to"
-                            + " a planning failure. Feel free to add more details to the issue description"
+                            + f" a planning failure. The error message is {str(e)}. Feel free to add more details to the issue description"
                             + " so Sweep can better address it. Alternatively, reach out to Kevin or William for help at"
                             + " https://discord.gg/sweep."
                         ),
                         -1,
                     )
                 log_error(
                     is_paying_user,
@@ -1734,16 +1703,14 @@
                         repo.get_git_ref(
                             f"heads/{pull_request.branch_name}"
                         ).delete()
                     else:
                         raise Exception(
                             f"Branch name {pull_request.branch_name} does not start with sweep/"
                         )
-                except SystemExit:
-                    raise SystemExit
                 except Exception as e:
                     logger.error(e)
                     logger.error(traceback.format_exc())
                     logger.info("Deleted branch", pull_request.branch_name)
         except Exception as e:
             posthog.capture(
                 username,
```

### Comparing `sweepai-2.0.2/sweepai/handlers/pr_utils.py` & `sweepai-2.1.0/sweepai/handlers/pr_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     REVERT_CHANGED_FILES_TITLE,
     SWEEP_BAD_FEEDBACK,
     SWEEP_GOOD_FEEDBACK,
     SweepConfig,
     get_documentation_dict,
 )
 from sweepai.config.server import DISCORD_FEEDBACK_WEBHOOK_URL
-from sweepai.core.context_pruning import get_relevant_context
 from sweepai.core.entities import NoFilesException, SandboxResponse
 from sweepai.core.sweep_bot import SweepBot, get_files_to_change, validate_file_change_requests
 
 # from sandbox.sandbox_utils import Sandbox
 from sweepai.handlers.create_pr import GITHUB_LABEL_NAME, create_pr_changes
 from sweepai.utils.buttons import Button, ButtonList, create_action_buttons
 from sweepai.utils.chat_logger import ChatLogger
@@ -44,19 +43,14 @@
         token=user_token,
         branch=branch_name,
     )
     logger.info("Fetching relevant files...")
     search_query = (title + summary).strip("\n")
     formatted_query = (f"{title.strip()}\n{summary.strip()}").strip("\n")
     repo_context_manager = prep_snippets(cloned_repo, search_query)
-    repo_context_manager = get_relevant_context(
-        formatted_query,
-        repo_context_manager,
-        chat_logger=chat_logger,
-    )
     snippets = repo_context_manager.current_top_snippets
     tree = str(repo_context_manager.dir_obj)
     message_summary = summary
     # removed external search as it provides no real value and only adds noise
     # external_results = ExternalSearcher.extract_summaries(message_summary)
     # if external_results:
     #     message_summary += "\n\n" + external_results
@@ -81,14 +75,15 @@
         cloned_repo=cloned_repo,
     )
     file_change_requests, plan = get_files_to_change(
         relevant_snippets=repo_context_manager.current_top_snippets,
         read_only_snippets=repo_context_manager.read_only_snippets,
         problem_statement=formatted_query,
         repo_name=repo_name,
+        cloned_repo=cloned_repo,
     )
     validate_file_change_requests(file_change_requests, repo_context_manager.cloned_repo)
     file_change_requests = sweep_bot.validate_file_change_requests(
         file_change_requests, branch_name
     )
     pull_request = sweep_bot.generate_pull_request()
     generator = create_pr_changes(
```

### Comparing `sweepai-2.0.2/sweepai/handlers/stack_pr.py` & `sweepai-2.1.0/sweepai/handlers/stack_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/handlers/stack_pr_test.py` & `sweepai-2.1.0/sweepai/handlers/stack_pr_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/logn/cache.py` & `sweepai-2.1.0/sweepai/logn/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,24 +45,24 @@
         return hashlib.md5("unknown".encode()).hexdigest()
 
 
 def hash_code(code):
     return hashlib.md5(code.encode()).hexdigest()
 
 
-def file_cache(ignore_params=[], verbose=False, redis=False):
+def file_cache(ignore_params=[], ignore_contents=False, verbose=False, redis=False):
     """Decorator to cache function output based on its inputs, ignoring specified parameters.
     Ignore parameters are used to avoid caching on non-deterministic inputs, such as timestamps.
     We can also ignore parameters that are slow to serialize/constant across runs, such as large objects.
     """
 
     def decorator(func):
         if DEBUG:
             return func
-        func_source_code_hash = hash_code(inspect.getsource(func))
+        func_source_code_hash = hash_code(inspect.getsource(func)) if not ignore_contents else ""
 
         def wrapper(*args, **kwargs):
             cache_dir = os.environ.get("MOUNT_DIR", "") + "/tmp/file_cache"
             os.makedirs(cache_dir, exist_ok=True)
             result = None
 
             # Convert args to a dictionary based on the function's signature
@@ -81,21 +81,23 @@
                 + recursive_hash(kwargs_clone, ignore_params=ignore_params)
                 + func_source_code_hash
             )
             cache_key = f"{func.__module__}_{func.__name__}_{arg_hash}"
             cache_file = os.path.join(
                 cache_dir, f"{cache_key}.pickle"
             )
+            redis_cache_hit = False
             if redis and redis_client: # only use this for LLM calls
                 try:
                     cached_result = redis_client.get(cache_key)
                     if cached_result:
                         if verbose:
                             print("Used redis cache for function: " + func.__name__)
                         result = pickle.loads(cached_result)
+                        redis_cache_hit = True
                 except Exception:
                     pass
             if result is None:
                 try:
                     # If cache exists, load and return it
                     if os.path.exists(cache_file):
                         if verbose:
@@ -104,29 +106,29 @@
                             result = pickle.load(f)
                 except Exception:
                     logger.info("Unpickling failed")
             # Otherwise, call the function and save its result to the cache
             if result is None:
                 result = func(*args, **kwargs)
             # hydrate both caches in all cases
-            if redis and redis_client: # cache this to redis as well
+            if redis and redis_client and not redis_cache_hit: # cache this to redis as well
                 try:
-                    # Cache the result using the unique cache key
+                    # Cache the result using the unique cache key only if it wasn't a redis cache hit
                     redis_client.set(cache_key, pickle.dumps(result))
                 except Exception as e:
                     if verbose:
                         print(f"Redis caching failed for function: {func.__name__}, Error: {e}")
-            if not isinstance(result, Exception):
+            if isinstance(result, Exception):
+                logger.info(f"Function {func.__name__} returned an exception")
+            elif not os.path.exists(cache_file):
                 try:
                     with open(cache_file, "wb") as f:
                         pickle.dump(result, f)
                 except Exception as e:
                     logger.info(f"Pickling failed: {e}")
-            else:
-                logger.info(f"Function {func.__name__} returned an exception")
             return result
 
         return wrapper
 
     return decorator
```

### Comparing `sweepai-2.0.2/sweepai/logn/logn.py` & `sweepai-2.1.0/sweepai/logn/logn.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/anthropic_client.py` & `sweepai-2.1.0/sweepai/utils/anthropic_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 parea_client = None
 try:
     if PAREA_API_KEY:
         parea_client = Parea(api_key=PAREA_API_KEY)
 except Exception as e:
     logger.info(f"Failed to initialize Parea client: {e}")
 
+# we cannot have two user messages in a row
 def sanitize_anthropic_messages(messages: list[dict[str, str]]):
     new_messages = []
     for message in messages:
         if message["role"] == "system":
             message["role"] = "user"
         if new_messages and new_messages[-1]["role"] == message["role"]:
             new_messages[-1]["content"] += "\n\n" + message["content"].rstrip()
```

### Comparing `sweepai-2.0.2/sweepai/utils/autoimport.py` & `sweepai-2.1.0/sweepai/utils/autoimport.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/buttons.py` & `sweepai-2.1.0/sweepai/utils/buttons.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/buttons_test.py` & `sweepai-2.1.0/sweepai/utils/buttons_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/chat_logger.py` & `sweepai-2.1.0/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/code_tree.py` & `sweepai-2.1.0/sweepai/utils/code_tree.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -215,8 +215,8 @@
     # file_contents = full_code
     # match_start = 16
     # match_end = 20
     code_tree = CodeTree.from_code(file_contents)
     print(code_tree.get_preview())
     print(len(code_tree.get_preview().split("\n")))
     # print(code_tree.get_lines_surrounding(match_start)[0])
-    # print(code_tree.get_lines_surrounding(match_end)[1])
+    # print(code_tree.get_lines_surrounding(match_end)[1])
```

### Comparing `sweepai-2.0.2/sweepai/utils/code_tree_test.py` & `sweepai-2.1.0/sweepai/utils/code_tree_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/comment_utils.py` & `sweepai-2.1.0/sweepai/utils/comment_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/comment_utils_test.py` & `sweepai-2.1.0/sweepai/utils/comment_utils_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/convert_openai_anthropic.py` & `sweepai-2.1.0/sweepai/utils/convert_openai_anthropic.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/diff.py` & `sweepai-2.1.0/sweepai/utils/diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,41 @@
 
 def generate_diff(old_code, new_code, **kwargs):
     if old_code == new_code:
         return ""
     stripped_old_code = old_code.strip()
     stripped_new_code = new_code.strip()
 
+    # Split the code into lines, preserving the line endings
+    old_lines = old_code.splitlines(keepends=True)
+    new_lines = new_code.splitlines(keepends=True)
+
+    # Add a newline character at the end if it's missing
+    if not old_code.endswith("\n"):
+        old_lines.append("\n")
+    if not new_code.endswith("\n"):
+        new_lines.append("\n")
+
     default_kwargs = {"n": 5}
     default_kwargs.update(kwargs)
 
     diff = difflib.unified_diff(
         stripped_old_code.splitlines(keepends=True),
         stripped_new_code.splitlines(keepends=True),
         **kwargs
     )
 
-    diff_text = "".join(diff)
+    diff_result = ""
 
-    return diff_text
+    for line in diff:
+        if not line.endswith("\n"):
+            line += "\n"
+        diff_result += line
 
+    return diff_result
 
 def generate_ndiff(old_code, new_code, **kwargs):
     if old_code == new_code:
         return ""
     stripped_old_code = old_code.strip()
     stripped_new_code = new_code.strip()
```

### Comparing `sweepai-2.0.2/sweepai/utils/diff_test.py` & `sweepai-2.1.0/sweepai/utils/diff_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/docker_utils.py` & `sweepai-2.1.0/sweepai/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/event_logger.py` & `sweepai-2.1.0/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/fuzzy_diff_test.py` & `sweepai-2.1.0/sweepai/utils/fuzzy_diff_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/github_utils.py` & `sweepai-2.1.0/sweepai/utils/github_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import datetime
 import difflib
 import hashlib
 import json
 import os
 import re
 import shutil
@@ -11,20 +12,21 @@
 import traceback
 from dataclasses import dataclass
 from functools import cached_property
 from typing import Any
 
 import git
 import requests
-from github import Github, PullRequest, Repository, InputGitTreeElement
+from github import Github, PullRequest, Repository, InputGitTreeElement, GithubException
 from jwt import encode
 from loguru import logger
 
 from sweepai.config.client import SweepConfig
 from sweepai.config.server import GITHUB_APP_ID, GITHUB_APP_PEM, GITHUB_BOT_USERNAME
+from sweepai.core.entities import FileChangeRequest
 from sweepai.utils.tree_utils import DirectoryTree, remove_all_not_included
 
 MAX_FILE_COUNT = 50
 
 
 def make_valid_string(string: str):
     pattern = r"[^\w./-]+"
@@ -59,15 +61,15 @@
                 raise Exception("Could not get token")
             return obj["token"]
         except SystemExit:
             raise SystemExit
         except Exception:
             time.sleep(timeout)
     raise Exception(
-        "Could not get token, please double check your PRIVATE_KEY and GITHUB_APP_ID in the .env file. Make sure to restart uvicorn after."
+        "Could not get token, please double check your GITHUB_APP_PEM and GITHUB_APP_ID in the .env file. Make sure to restart uvicorn after."
     )
 
 
 def get_app():
     jwt = get_jwt()
     headers = {
         "Accept": "application/vnd.github+json",
@@ -144,28 +146,51 @@
         try:
             obj = response.json()
             return obj["id"]
         except Exception as e:
             logger.error(e)
             logger.error(response.text)
         raise Exception("Could not get installation id, probably not installed")
+    
+# for check if a file exists within a github repo (calls the actual github api)
+def file_exists_in_repo(repo: Repository, filepath: str):
+    try:
+        # Attempt to get the contents of the file
+        repo.get_contents(filepath)
+        return True  # If no exception, the file exists
+    except GithubException:
+        return False  # File does not exist
+    
+def validate_and_sanitize_multi_file_changes(repo: Repository, file_changes: dict[str, str], fcrs: list[FileChangeRequest]):
+    sanitized_file_changes = {}
+    all_file_names = list(file_changes.keys())
+    all_fcr_file_names = set(os.path.normpath(fcr.filename) for fcr in fcrs)
+    file_removed = False
+    # validate each file change
+    for file_name in all_file_names:
+        # file_name must either appear in the repo or in a fcr
+        if os.path.normpath(file_name) in all_fcr_file_names or file_exists_in_repo(repo, os.path.normpath(file_name)):
+            sanitized_file_changes[file_name] = copy.deepcopy(file_changes[file_name])
+        else:
+            file_removed = True
+    return sanitized_file_changes, file_removed
 
 # commits multiple files in a single commit, returns the commit object
 def commit_multi_file_changes(repo: Repository, file_changes: dict[str, str], commit_message: str, branch: str):
     blobs_to_commit = []
     # convert to blob
     for path, content in file_changes.items():
         blob = repo.create_git_blob(content, "utf-8")
         blobs_to_commit.append(InputGitTreeElement(path=os.path.normpath(path), mode="100644", type="blob", sha=blob.sha))
-    latest_commit = repo.get_branch(branch).commit
-    base_tree = latest_commit.commit.tree
+    head_sha = repo.get_branch(branch).commit.sha
+    base_tree = repo.get_git_tree(sha=head_sha)
     # create new git tree
     new_tree = repo.create_git_tree(blobs_to_commit, base_tree=base_tree)
     # commit the changes
-    parent = repo.get_git_commit(latest_commit.sha)
+    parent = repo.get_git_commit(sha=head_sha)
     commit = repo.create_git_commit(
         commit_message,
         new_tree,
         [parent],
     )
     # update ref of branch
     ref = f"heads/{branch}"
@@ -377,15 +402,15 @@
 
     def get_file_contents(self, file_path, ref=None):
         local_path = (
             f"{self.repo_dir}{file_path}"
             if file_path.startswith("/")
             else f"{self.repo_dir}/{file_path}"
         )
-        if os.path.exists(local_path):
+        if os.path.exists(local_path) and os.path.isfile(local_path):
             with open(local_path, "r", encoding="utf-8", errors="replace") as f:
                 contents = f.read()
             return contents
         else:
             raise FileNotFoundError(f"{local_path} does not exist.")
 
     def get_num_files_from_repo(self):
@@ -654,14 +679,35 @@
     # Make the POST request
     response = requests.post(url, headers=headers, data=json.dumps(json_data))
     if response.status_code != 200:
         logger.error(f"Failed to convert PR to {'draft' if is_draft else 'open'}")
         return False
     return True
 
+# makes sure no secrets are in the message
+def sanitize_string_for_github(message: str):
+    GITHUB_APP_PEM = os.environ.get("GITHUB_APP_PEM", "")
+    GITHUB_APP_ID = os.environ.get("GITHUB_APP_ID", "")
+    ANTHROPIC_API_KEY = os.environ.get("ANTHROPIC_API_KEY", "")
+    OPENAI_API_KEY = os.environ.get("OPENAI_API_KEY", "")
+    INSTALLATION_ID = os.environ.get("INSTALLATION_ID", "")
+    GITHUB_PAT = os.environ.get("GITHUB_PAT", "")
+    COHERE_API_KEY = os.environ.get("COHERE_API_KEY", "")
+    LICENSE_KEY = os.environ.get("LICENSE_KEY", "")
+    VOYAGE_API_KEY = os.environ.get("VOYAGE_API_KEY", "")
+    AWS_ACCESS_KEY = os.environ.get("AWS_ACCESS_KEY", "")
+    AWS_SECRET_KEY = os.environ.get("AWS_SECRET_KEY", "")
+    # include all previous env vars in secrets array
+    secrets = [GITHUB_APP_PEM, GITHUB_APP_ID, ANTHROPIC_API_KEY, OPENAI_API_KEY, INSTALLATION_ID, GITHUB_PAT, COHERE_API_KEY, LICENSE_KEY, VOYAGE_API_KEY, AWS_ACCESS_KEY, AWS_SECRET_KEY]
+    secrets = [secret for secret in secrets if secret]
+    for secret in secrets:
+        if secret in message:
+            message = message.replace(secret, "*" * len(secret))
+    return message
+
 
 try:
     g = Github(os.environ.get("GITHUB_PAT"))
     CURRENT_USERNAME = g.get_user().login
 except Exception:
     try:
         slug = get_app()["slug"]
```

### Comparing `sweepai-2.0.2/sweepai/utils/github_utils_test.py` & `sweepai-2.1.0/sweepai/utils/github_utils_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/html_extractor.py` & `sweepai-2.1.0/sweepai/utils/html_extractor.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/modify_utils.py` & `sweepai-2.1.0/sweepai/utils/modify_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,19 +81,19 @@
                         if line.startswith(new_code):
                             return 0, True
                         return len(line)-len(line.lstrip()), True
         return -1, False
                 
     # assume one indent is two spaces and check max 10 indents
     for indent in range(0, 40, 2):
-        new_code_lines = [f"{' ' * indent}{line}" for line in code_lines]
+        new_code_lines = [f"{' ' * indent}{line}" if line.strip() else "" for line in code_lines]
         new_code = "\n".join(new_code_lines)
         if new_code in file_contents:
             return indent, False
     # sometimes llm returns code with trailing whitespace, if we have reached here check again but strip all trailing whitespace
     code_lines = [line.rstrip() for line in code_snippet.split("\n")]
     for indent in range(0, 40, 2):
-        new_code_lines = [f"{' ' * indent}{line}" for line in code_lines]
+        new_code_lines = [f"{' ' * indent}{line}" if line.strip() else "" for line in code_lines]
         new_code = "\n".join(new_code_lines)
         if new_code in file_contents:
             return indent, True
     return -1, False
```

### Comparing `sweepai-2.0.2/sweepai/utils/multi_query.py` & `sweepai-2.1.0/sweepai/utils/multi_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
   - Auth flows, session management, encryption
   - Infrastructure, CI/CD, deployments, config
 - List out any unfamiliar domain terms to search for to better understand schemas, types, relationships between entities, etc. Finding data models is key.
 - Rate limiting, caching and other cross-cutting concerns could be very relevant for issues with scale or performance.
 
 3. Queries
 
-Generate a list of 10 diverse, highly specific, focused "where" queries to use as vector database search queries to find the most relevant code sections to directly resolve the GitHub issue.
+Generate a list of 10 DIVERSE, highly specific, focused "where" queries to use as vector database search queries to find the most relevant code sections to directly resolve the GitHub issue.
 - Reference very specific functions, variables, classes, endpoints, etc. using exact names.
 - Describe the purpose and behavior of the code in detail to differentiate it. 
 - Ask about granular logic within individual functions/methods.
 - Mention adjacent code like schemas, configs, and helpers to establish context.
 - Use verbose natural language that mirrors the terminology in the codebase.
 - Aim for high specificity to pinpoint the most relevant code in a large codebase.
 
@@ -55,17 +55,17 @@
 Exhaustive list of relevant parts of the codebase that could be used in the solution include:
 - [Module, service, function or endpoint 1] 
 - [Module, service, function or endpoint 2]
 - [etc.]
 </solution>
 
 <queries>
-<query>Where is the [extremely specific description of code section 1]?</query>
-<query>Where is the [extremely specific description of code section 2]?</query>
-<query>Where is the [extremely specific description of code section 3]?</query>
+<query>Where is the [EXTREMELY specific description of code section 1]?</query>
+<query>Where is the [EXTREMELY specific description of code section 2]?</query>
+<query>Where is the [EXTREMELY specific description of code section 3]?</query>
 ...
 </queries>
 
 Examples of good queries:
 - Where is the function that compares the user-provided password hash against the stored hash from the database in the user-authentication service?
 - Where is the code that constructs the GraphQL mutation for updating a user's profile information, and what specific fields are being updated?
 - Where are the React components that render the product carousel on the homepage, and what library is being used for the carousel functionality?
@@ -81,23 +81,24 @@
             Message(
                 content=system_message,
                 role="system",
             )
         ],
     )
     stripped_input = input_query.strip('\n')
-    response = chatgpt.chat_anthropic(
-        f"<github_issue>\n{stripped_input}\n</github_issue>", 
-        model="claude-3-opus-20240229"
+    response = chatgpt.chat(
+        content=f"<github_issue>\n{stripped_input}\n</github_issue>",
+        model="gpt-4-turbo-2024-04-09",
+        temperature=0.7, # I bumped this and it improved the benchmarks
     )
     pattern = re.compile(r"<query>(?P<query>.*?)</query>", re.DOTALL)
     queries = []
     for q in pattern.finditer(response):
         query = q.group("query").strip()
         if query:
             queries.append(query)
     logger.debug(f"Generated {len(queries)} queries from the input query.")
     return queries
 
 if __name__ == "__main__":
     input_query = "I am trying to set up payment processing in my app using Stripe, but I keep getting a 400 error when I try to create a payment intent. I have checked the API key and the request body, but I can't figure out what's wrong. Here is the error message I'm getting: 'Invalid request: request parameters are invalid'. I have attached the relevant code snippets below. Can you help me find the part of the code that is causing this error?"
-    generate_multi_queries(input_query)
+    generate_multi_queries(input_query)
```

### Comparing `sweepai-2.0.2/sweepai/utils/openai_listwise_reranker.py` & `sweepai-2.1.0/sweepai/utils/openai_listwise_reranker.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/openai_proxy.py` & `sweepai-2.1.0/sweepai/utils/openai_proxy.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                             response = self.call_azure_api(
                                 model=model,
                                 messages=messages,
                                 tools=tools,
                                 max_tokens=max_tokens,
                                 temperature=temperature,
                             )
-                            return response
+                            return response.choices[0].message.content
                     except RateLimitError as e:
                         logger.exception(f"Rate Limit Error calling Azure: {e}")
                 else:
                     logger.info(
                         f"Calling OpenAI with model {model}."
                     )
                     with Timer():
@@ -125,15 +125,15 @@
                             api_key=api_key,
                             model=model,
                             messages=messages,
                             tools=tools,
                             max_tokens=max_tokens,
                             temperature=temperature,
                         )
-                        return response
+                        return response.choices[0].message.content
                 except (RateLimitError, APITimeoutError, InternalServerError) as e:
                     logger.exception(f"RateLimitError calling {region_url}: {e}")
             raise Exception("No Azure regions available")
         except (RateLimitError, APITimeoutError, InternalServerError) as e:
             try:
                 with Timer():
                     return self.set_openai_default_api_parameters(
@@ -242,27 +242,36 @@
                 model=model,
                 messages=messages,
                 max_tokens=max_tokens,
                 temperature=temperature,
                 timeout=OPENAI_TIMEOUT,
                 seed=SEED,
                 stop=stop_sequences,
+                stream=True,
             )
+            text = ""
+            for chunk in response:
+                new_content = chunk.choices[0].delta.content
+                text += new_content if new_content else ""
+                if new_content:
+                    print(new_content, end="", flush=True)
+            print() # clear the line
+            return text
         else:
             response = client.chat.completions.create(
                 model=model,
                 messages=messages,
                 tools=tools,
                 max_tokens=max_tokens,
                 temperature=temperature,
                 timeout=OPENAI_TIMEOUT,
                 seed=SEED,
                 stop=stop_sequences,
             )
-        return response
+            return response.choices[0].message.content
 
 
 def get_client():
     OPENAI_API_KEY = os.environ.get("OPENAI_API_KEY")
     OPENAI_API_TYPE = os.environ.get("OPENAI_API_TYPE", "openai")
     OPENAI_API_BASE = os.environ.get(
         "OPENAI_API_BASE", None
@@ -320,9 +329,24 @@
         model=model,
         name="Test assistant",
         description="test",
         instructions="Say this is a test",
     )
 
 if __name__ == "__main__":
-    test_openai_proxy()
-    test_get_client()
+    model, client = get_client()
+    response = client.chat.completions.create(
+        model=model,
+        messages=[Message(
+            role="user",
+            content="Say this is a test",
+        ).to_openai()],
+        stream=True,
+    )
+    print("Generating response...", flush=True)
+    text = ""
+    for chunk in response:
+        new_content = chunk.choices[0].delta.content
+        text += new_content if new_content else ""
+        if new_content:
+            print(new_content, end="", flush=True)
+    print()
```

### Comparing `sweepai-2.0.2/sweepai/utils/openai_proxy_test.py` & `sweepai-2.1.0/sweepai/utils/openai_proxy_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/patch_utils.py` & `sweepai-2.1.0/sweepai/utils/patch_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/progress.py` & `sweepai-2.1.0/sweepai/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/prompt_constructor.py` & `sweepai-2.1.0/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/regex_utils.py` & `sweepai-2.1.0/sweepai/utils/regex_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/safe_pqueue.py` & `sweepai-2.1.0/sweepai/utils/safe_pqueue.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/scorer.py` & `sweepai-2.1.0/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/scorer_test.py` & `sweepai-2.1.0/sweepai/utils/scorer_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/search_and_replace.py` & `sweepai-2.1.0/sweepai/utils/search_and_replace.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/search_and_replace_test.py` & `sweepai-2.1.0/sweepai/utils/search_and_replace_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/str_utils.py` & `sweepai-2.1.0/sweepai/utils/str_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 sep = "\n---\n"
 bot_suffix_starring = ""
 bot_suffix = (
     f"\n{sep}\n{UPDATES_MESSAGE}\n\n💡 To recreate the pull request edit the issue"
     " title or description."
 )
 discord_suffix = (
-    "\n<sup>Something wrong? [Let us know](https://discord.gg/sweep).</sup>"
+    "\n<sup>Something wrong? [Let us know](https://community.sweep.dev/).</sup>"
 )
 
 stars_suffix = ""
 
 collapsible_template = """
 <details {opened}>
 <summary>{summary}</summary>
```

### Comparing `sweepai-2.0.2/sweepai/utils/ticket_utils.py` & `sweepai-2.1.0/sweepai/utils/ticket_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from collections import defaultdict
+import copy
 import traceback
 from time import time
 
-import cohere
 from loguru import logger
 from tqdm import tqdm
 import networkx as nx
 
 from sweepai.config.client import SweepConfig, get_blocked_dirs
 from sweepai.config.server import COHERE_API_KEY
 from sweepai.core.context_pruning import RepoContextManager, add_relevant_files_to_top_snippets, build_import_trees, integrate_graph_retrieval
 from sweepai.core.entities import Snippet
 from sweepai.core.lexical_search import (
     compute_vector_search_scores,
     prepare_lexical_search_index,
     search_index,
 )
-from sweepai.core.sweep_bot import get_files_to_change
+from sweepai.core.sweep_bot import context_get_files_to_change
 from sweepai.logn.cache import file_cache
 from sweepai.utils.chat_logger import discord_log_error
+from sweepai.utils.cohere_utils import cohere_rerank_call
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import ClonedRepo
 from sweepai.utils.multi_query import generate_multi_queries
 from sweepai.utils.openai_listwise_reranker import listwise_rerank_snippets
 from sweepai.utils.progress import TicketProgress
+from sweepai.utils.tree_utils import DirectoryTree
 
 """
 Input queries are in natural language so both lexical search 
 and vector search have a heavy bias towards natural language
 files such as tests, docs and localization files. Therefore,
 we add adjustment scores to compensate for this bias.
 """
@@ -49,34 +51,36 @@
     ".json": 0.8,
     ".toml": 0.8,
     ".yaml": 0.8,
     ".yml": 0.8,
     ".1": 0.5, # man pages
     ".spec.ts": 0.6,
     ".spec.js": 0.6,
+    ".test.ts": 0.6,
     ".generated.ts": 0.5,
     ".generated.graphql": 0.5,
     ".generated.js": 0.5,
     "ChangeLog": 0.5,
 }
 
 substring_adjustment = {
     "tests/": 0.5,
-    "test_": 0.5,
+    "test/": 0.5,
+    "/test": 0.5,
     "_test": 0.5,
     "egg-info": 0.5,
     "LICENSE": 0.5,
 }
 
 def apply_adjustment_score(
     snippet: str,
     old_score: float,
 ):
     snippet_score = old_score
-    file_path, *_ = snippet.split(":")
+    file_path, *_ = snippet.rsplit(":", 1)
     file_path = file_path.lower()
     for prefix, adjustment in prefix_adjustment.items():
         if file_path.startswith(prefix):
             snippet_score *= adjustment
             break
     for suffix, adjustment in suffix_adjustment.items():
         if file_path.endswith(suffix):
@@ -163,30 +167,14 @@
     k: int = 15,
 ):
     ranked_snippets_list, snippets, content_to_lexical_score_list = multi_get_top_k_snippets(
         cloned_repo, [query], ticket_progress, k
     )
     return ranked_snippets_list[0], snippets, content_to_lexical_score_list[0]
 
-@file_cache()
-def cohere_rerank_call(
-    query: str,
-    documents: list[str],
-    model='rerank-english-v3.0',
-    **kwargs,
-):
-    # Cohere API call with caching
-    co = cohere.Client(COHERE_API_KEY)
-    return co.rerank(
-        model=model,
-        query=query,
-        documents=documents,
-        **kwargs
-    )
-
 def get_pointwise_reranked_snippet_scores(
     query: str,
     snippets: list[Snippet],
     snippet_scores: dict[str, float],
 ):
     """
     Ranks 1-5 snippets are frozen. They're just passed into Cohere since it helps with reranking. We multiply the scores by 1_000 to make them more significant.
@@ -219,14 +207,18 @@
             sorted_snippets[document.index].denotation,
             document.relevance_score,
         )
 
     for snippet in sorted_snippets[:NUM_SNIPPETS_TO_KEEP]:
         new_snippet_scores[snippet.denotation] = snippet_scores[snippet.denotation] * 1_000
     
+    # override score with Cohere score
+    for snippet in sorted_snippets[:NUM_SNIPPETS_TO_RERANK]:
+        if snippet.denotation in new_snippet_scores:
+            snippet.score = new_snippet_scores[snippet.denotation]
     return new_snippet_scores
 
 def multi_prep_snippets(
     cloned_repo: ClonedRepo,
     queries: list[str],
     ticket_progress: TicketProgress | None = None,
     k: int = 15,
@@ -269,28 +261,29 @@
             key=lambda snippet: content_to_lexical_score[snippet.denotation],
             reverse=True,
         )[:k]
     if ticket_progress:
         ticket_progress.search_progress.retrieved_snippets = ranked_snippets
         ticket_progress.save()
     # you can use snippet.denotation and snippet.get_snippet()
-    if not skip_reranking and not skip_pointwise_reranking:
+    if not skip_reranking and skip_pointwise_reranking:
         ranked_snippets[:NUM_SNIPPETS_TO_RERANK] = listwise_rerank_snippets(queries[0], ranked_snippets[:NUM_SNIPPETS_TO_RERANK])
     snippet_paths = [snippet.file_path for snippet in ranked_snippets]
     prefixes = []
     for snippet_path in snippet_paths:
         snippet_depth = len(snippet_path.split("/"))
         for idx in range(snippet_depth):  # heuristic
             if idx > snippet_depth // 2:
                 prefixes.append("/".join(snippet_path.split("/")[:idx]) + "/")
         prefixes.append(snippet_path)
-    _, dir_obj = cloned_repo.list_directory_tree(
-        included_directories=list(set(prefixes)),
-        included_files=list(set(snippet_paths)),
-    )
+    # _, dir_obj = cloned_repo.list_directory_tree(
+    #     included_directories=list(set(prefixes)),
+    #     included_files=list(set(snippet_paths)),
+    # )
+    dir_obj = DirectoryTree() # init dummy one for now, this shouldn't be used
     repo_context_manager = RepoContextManager(
         dir_obj=dir_obj,
         current_top_tree=str(dir_obj),
         current_top_snippets=ranked_snippets,
         snippets=snippets,
         snippet_scores=content_to_lexical_score,
         cloned_repo=cloned_repo,
@@ -315,71 +308,68 @@
 
 def get_relevant_context(
     query: str,
     repo_context_manager: RepoContextManager,
     seed: int = None,
     import_graph: nx.DiGraph = None,
     chat_logger = None,
+    images = None
 ) -> RepoContextManager:
     logger.info("Seed: " + str(seed))
     repo_context_manager = build_import_trees(
         repo_context_manager,
         import_graph,
     )
     repo_context_manager = add_relevant_files_to_top_snippets(repo_context_manager)
     repo_context_manager.dir_obj.add_relevant_files(
         repo_context_manager.relevant_file_paths
     )
-    fcrs, plan = get_files_to_change(
+    relevant_files, read_only_files = context_get_files_to_change(
         relevant_snippets=repo_context_manager.current_top_snippets,
-        read_only_snippets=repo_context_manager.snippets,
+        read_only_snippets=repo_context_manager.read_only_snippets,
         problem_statement=query,
         repo_name=repo_context_manager.cloned_repo.repo_full_name,
         import_graph=import_graph,
         chat_logger=chat_logger,
         seed=seed,
-        context=True
+        cloned_repo=repo_context_manager.cloned_repo,
+        images=images
     )
+    previous_top_snippets = copy.deepcopy(repo_context_manager.current_top_snippets)
+    previous_read_only_snippets = copy.deepcopy(repo_context_manager.read_only_snippets)
     repo_context_manager.current_top_snippets = []
     repo_context_manager.read_only_snippets = []
-    visited_paths = set()
-    for fcr in fcrs:
-        if fcr.filename in visited_paths:
-            continue
-        visited_paths.add(fcr.filename)
+    for relevant_file in relevant_files:
         try:
-            content = repo_context_manager.cloned_repo.get_file_contents(fcr.filename)
+            content = repo_context_manager.cloned_repo.get_file_contents(relevant_file)
         except FileNotFoundError:
             continue
         snippet = Snippet(
-            file_path=fcr.filename,
+            file_path=relevant_file,
             start=0,
             end=len(content.split("\n")),
             content=content,
         )
         repo_context_manager.current_top_snippets.append(snippet)
-    repo_context_manager.read_only_snippets = []
-    if fcrs:
-        for file_path in fcrs[0].relevant_files:
-            if file_path in visited_paths:
-                continue
-            visited_paths.add(file_path)
-            try:
-                content = repo_context_manager.cloned_repo.get_file_contents(file_path)
-            except FileNotFoundError:
-                continue
-            snippet = Snippet(
-                file_path=file_path,
-                start=0,
-                end=len(content.split("\n")),
-                content=content,
-            )
-            repo_context_manager.read_only_snippets.append(snippet)
-    else:
-        raise Exception("No file change requests created.")
+    for read_only_file in read_only_files:
+        try:
+            content = repo_context_manager.cloned_repo.get_file_contents(read_only_file)
+        except FileNotFoundError:
+            continue
+        snippet = Snippet(
+            file_path=read_only_file,
+            start=0,
+            end=len(content.split("\n")),
+            content=content,
+        )
+        repo_context_manager.read_only_snippets.append(snippet)
+    
+    if not repo_context_manager.current_top_snippets and not repo_context_manager.read_only_snippets:
+        repo_context_manager.current_top_snippets = copy.deepcopy(previous_top_snippets)
+        repo_context_manager.read_only_snippets = copy.deepcopy(previous_read_only_snippets)
     return repo_context_manager
 
 def fetch_relevant_files(
     cloned_repo,
     title,
     summary,
     replies_text,
@@ -388,42 +378,41 @@
     on_ticket_start_time,
     tracking_id,
     is_paying_user,
     is_consumer_tier,
     issue_url,
     chat_logger,
     ticket_progress: TicketProgress,
+    images = None
 ):
     logger.info("Fetching relevant files...")
     try:
         search_query = (title + summary + replies_text).strip("\n")
         replies_text = f"\n{replies_text}" if replies_text else ""
         formatted_query = (f"{title.strip()}\n{summary.strip()}" + replies_text).strip(
             "\n"
         )
         repo_context_manager = prep_snippets(cloned_repo, search_query, ticket_progress)
 
         repo_context_manager, import_graph = integrate_graph_retrieval(search_query, repo_context_manager)
 
-        ticket_progress.search_progress.repo_tree = str(repo_context_manager.dir_obj)
         ticket_progress.save()
         repo_context_manager = get_relevant_context(
             formatted_query,
             repo_context_manager,
             ticket_progress,
             chat_logger=chat_logger,
             import_graph=import_graph,
+            images=images
         )
         snippets = repo_context_manager.current_top_snippets
-        ticket_progress.search_progress.repo_tree = str(repo_context_manager.dir_obj)
         ticket_progress.search_progress.final_snippets = snippets
         ticket_progress.save()
-
-        tree = str(repo_context_manager.dir_obj)
         dir_obj = repo_context_manager.dir_obj
+        tree = str(dir_obj)
     except Exception as e:
         trace = traceback.format_exc()
         logger.exception(f"{trace} (tracking ID: `{tracking_id}`)")
         log_error(
             is_paying_user,
             is_consumer_tier,
             username,
```

### Comparing `sweepai-2.0.2/sweepai/utils/timer.py` & `sweepai-2.1.0/sweepai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/tree_utils.py` & `sweepai-2.1.0/sweepai/utils/tree_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/user_settings.py` & `sweepai-2.1.0/sweepai/utils/user_settings.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/utils/utils.py` & `sweepai-2.1.0/sweepai/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,33 @@
 from typing import Optional
 import uuid
 
 from pylint.lint import Run
 from pylint.reporters.text import TextReporter
 import tiktoken
 from loguru import logger
-from tree_sitter import Node
-from tree_sitter_languages import get_parser
+from tree_sitter import Node, Parser, Language
+from tree_sitter_languages import get_parser as tree_sitter_get_parser
+import tree_sitter_python
+import tree_sitter_javascript
 
 from sweepai.core.entities import Snippet
+from sweepai.logn.cache import file_cache
 from sweepai.utils.fuzzy_diff import patience_fuzzy_additions
 
+def get_parser(language: str):
+    parser = Parser()
+    if language in ("python", "py"):
+        lang = Language(tree_sitter_python.language(), "python")
+    elif language in ("javascript", "js"):
+        lang = Language(tree_sitter_javascript.language(), "javascript")
+    else:
+        return tree_sitter_get_parser(language)
+    parser.set_language(lang)
+    return parser
 
 def non_whitespace_len(s: str) -> int:  # new len function
     return len(re.sub("\s", "", s))
 
 
 def get_line_number(index: int, source_code: str) -> int:
     total_chars = 0
@@ -194,14 +207,45 @@
         end = min(start + line_count, total_lines)
         chunk = "\n".join(lines[start:end])
         chunks.append(chunk)
         start += line_count - overlap
 
     return chunks
 
+def get_new_lint_errors_for_pylint(new_errors: str, old_errors: str) -> str:
+    # Example of error: "main.py:1585:12: W0612: Unused variable 'command' (unused-variable)"
+    additional_errors = patience_fuzzy_additions(old_errors, new_errors).splitlines()
+    old_error_types = []
+    for line in old_errors.splitlines():
+        if line.count(" ") > 2:
+            _file_delimiter, error_type, *_ = line.split(" ")
+            old_error_types.append(error_type)
+    results = []
+    for line in additional_errors:
+        _file_delimiter, error_type, *_ = line.split(" ")
+        if error_type.startswith("E") or old_error_types.count(error_type) < 2: # if there are more than 1 of the same error, we consider it new
+            results.append(line)
+    return "\n".join(results)
+
+def get_new_lint_errors_for_eslint(new_errors: str, old_errors: str) -> str:
+    # Example of error: "main.py:1585:12: W0612: Unused variable 'command' (unused-variable)"
+    additional_errors = patience_fuzzy_additions(old_errors, new_errors).splitlines()
+    old_error_types = []
+    for line in old_errors.splitlines():
+        if line.count(" ") > 2:
+            *_, error_type = line.split(" ")
+            old_error_types.append(error_type)
+    results = []
+    for line in additional_errors:
+        *_, error_type = line.split(" ")
+        if not line.startswith("✖") and old_error_types.count(error_type) < 2: # if there are more than 1 of the same error, we consider it new
+            results.append(line)
+    return "\n".join(results)
+
+
 @dataclass
 class CheckResults:
     # Experimental feature, we'll see how this does.
     # TODO: smart parsing
     parse_error_message: str = ""
     pylint: str = ""
     eslint: str = ""
@@ -210,27 +254,36 @@
         if self.parse_error_message:
             return True
         if other.parse_error_message:
             return False
         return len(self.pylint.splitlines()) > len(other.pylint.splitlines()) or len(self.eslint.splitlines()) > len(other.eslint.splitlines())
     
     def is_worse_than_message(self, other: CheckResults) -> str:
+        if other.parse_error_message:
+            # Previously failing
+            return ""
         if self.parse_error_message:
             return self.parse_error_message
-        if other.parse_error_message:
-            return other.parse_error_message
         if len(self.pylint.splitlines()) > len(other.pylint.splitlines()):
             # return f"The code has the following pylint errors:\n\n{self.pylint}"
+            new_pylint_errors = get_new_lint_errors_for_pylint(self.pylint, other.pylint)
             if not other.pylint:
                 return f"The code has the following pylint errors:\n\n{self.pylint}"
-            return f"The following new pylint errors have appeared:\n\n{patience_fuzzy_additions(other.pylint, self.pylint)}"
+            elif not new_pylint_errors:
+                # All the errors are invalid
+                return ""
+            return f"The following new pylint errors have appeared:\n\n{new_pylint_errors}"
         if len(self.eslint.splitlines()) > len(other.eslint.splitlines()):
+            new_eslint_errors = get_new_lint_errors_for_eslint(self.eslint, other.eslint)
             if not other.eslint:
                 return f"The code has the following eslint errors:\n\n{self.eslint}"
-            return f"The following new eslint errors have appeared:\n\n{patience_fuzzy_additions(other.eslint, self.eslint)}"
+            elif not new_eslint_errors:
+                # All the errors are invalid
+                return ""
+            return f"The following new eslint errors have appeared:\n\n{new_eslint_errors}"
         return ""
 
 def strip_ansi_codes(text: str) -> str:
     # ANSI escape sequences (color codes) are often starting with ESC ([) followed by some numbers and ends with "m".
     ansi_escape = re.compile(r'(\x9B|\x1B\[)[0-?]*[ -\/]*[@-~]')
     return ansi_escape.sub('', text)
 
@@ -337,110 +390,119 @@
         return (False, error_message)
     return True, ""
 
 # Need to add "no-unused-vars": "error"
 # Need to add "import/first": "error"
 
 DEFAULT_ESLINTRC = """{
-  "parser": "@typescript-eslint/parser",
-  "parserOptions": {
-    "ecmaVersion": 2020,
-    "sourceType": "module"
-  },
-  "plugins": [
-    "@typescript-eslint",
-    "import"
-  ],
-  "rules": {
-    "no-undef": "error",
-    "no-const-assign": "error",
-    "no-redeclare": "error",
-    "no-unused-vars": "error",
-    "no-use-before-define": ["error", { "functions": true, "classes": true, "variables": true }],
-    "import/first": "error"
-  },
-  "settings": {
-    "import/resolver": {
-      "typescript": {}
-    }
-  },
-  "extends": [
-    "eslint:recommended",
-    "plugin:@typescript-eslint/recommended",
-    "plugin:import/typescript"
-  ],
-  "overrides": [
-    {
-      "files": ["*.ts", "*.tsx"],
-      "rules": {
-        "no-undef": "off"
+    "parser": "@typescript-eslint/parser",
+    "parserOptions": {
+      "ecmaVersion": 2020,
+      "sourceType": "module",
+      "ecmaFeatures": {
+        "jsx": true
       }
+    },
+    "settings": {
+      "react": {
+        "version": "detect"
+      }
+    },
+    "extends": [
+      "eslint:recommended",
+      "plugin:react/recommended",
+      "plugin:@typescript-eslint/recommended"
+    ],
+    "env": {
+      "browser": true,
+      "es2021": true,
+      "node": true
+    },
+    "plugins": [
+      "react",
+      "@typescript-eslint"
+    ],
+    "rules": {
+        "no-undef": "error",
+        "no-const-assign": "error",
+        "no-redeclare": "error",
+        "no-unused-vars": "error",
+        "no-use-before-define": ["error", { "functions": true, "classes": true, "variables": true }],
+        "import/first": "error"
     }
-  ]
-}"""
+  }
+  """
+
+@file_cache()
+def get_pylint_check_results(file_path: str, code: str) -> CheckResults:
+    logger.debug(f"Running pylint on {file_path}...")
+    file_hash = uuid.uuid4().hex
+    new_file = os.path.join("/tmp", file_hash + "_" + os.path.basename(file_path))
+    stem = os.path.splitext(os.path.basename(file_path))[0]
+    with open(new_file, "w") as f:
+        f.write(code)
+    pylint_output = StringIO()
+    reporter = TextReporter(pylint_output)
+    Run(
+        [
+            new_file,
+            "--disable=C",
+            "--enable=C0413",  # Enable only the check for imports not at the top
+            "--disable=R",
+            "--disable=import-error",
+            "--disable=no-member",
+        ],
+        reporter=reporter,
+        exit=False,
+    )
+    error_message = pylint_output.getvalue().strip()
+    try:
+        os.remove(new_file)
+    except FileNotFoundError:
+        pass
+    succeeded = error_message.startswith("------------------------------------")
+    if error_message:
+        error_message = error_message.replace(new_file, file_path).replace(f"{file_hash}_" + stem, stem)
+        error_message = error_message.split("-----------------------------------", 1)[0].strip()
+        error_message = f"> pylint {file_path}\n\n" + error_message
+    logger.debug("Done running pylint.")
+    return CheckResults(pylint=error_message if not succeeded else "")
 
 def get_check_results(file_path: str, code: str) -> CheckResults:
     is_valid, error_message = check_syntax(file_path, code)
     if not is_valid:
         return CheckResults(parse_error_message=error_message)
-    ext = file_path.split(".")[-1] # noqa
+    ext = file_path.rsplit(".")[-1] # noqa
     if ext == "py":
-        file_hash = uuid.uuid4().hex
-        new_file = os.path.join("/tmp", file_hash + "_" + os.path.basename(file_path))
-        stem = os.path.splitext(os.path.basename(file_path))[0]
         try:
-            with open(new_file, "w") as f:
-                f.write(code)
-            pylint_output = StringIO()
-            reporter = TextReporter(pylint_output)
-            Run(
-                [
-                    new_file,
-                    "--disable=C",
-                    "--enable=C0413",  # Enable only the check for imports not at the top
-                    "--disable=R",
-                    "--disable=import-error",
-                    "--disable=no-member",
-                    "--disable=unused-import" # we have a workaround for this tbh
-                ],
-                reporter=reporter,
-                exit=False,
-            )
-            error_message = pylint_output.getvalue().strip()
-            try:
-                os.remove(new_file)
-            except FileNotFoundError:
-                pass
-            succeeded = error_message.startswith("------------------------------------")
-            if error_message:
-                error_message = error_message.replace(new_file, file_path).replace(f"{file_hash}_" + stem, stem)
-                error_message = error_message.split("-----------------------------------", 1)[0].strip()
-                error_message = f"> pylint {file_path}\n\n" + error_message
-            return CheckResults(pylint=error_message if not succeeded else "")
+            return get_pylint_check_results(file_path, code)
         except Exception as e:
             logger.exception(e)
-    if ext == "ts":
+    elif ext in ["js", "jsx", "ts", "tsx"]:
         # see if eslint is installed
         npx_commands = ["npx", "eslint", "--version"]
         result = subprocess.run(
             " ".join(npx_commands),
             timeout=5,
             capture_output=True,
             text=True,
             shell=True,
         )
+        # Check eslint < v9 and all the plugins exist
         if result.returncode == 0:
-            with TemporaryDirectory() as temp_dir:
-                new_file = os.path.join(temp_dir, "temp.ts")
-                with open(os.path.join(temp_dir, ".eslintrc"), "w") as f:
+            with TemporaryDirectory(dir=os.getcwd()) as temp_dir:
+                file_name = file_path.split(os.path.sep)[-1]
+                new_file = os.path.join(temp_dir, f"{file_name}")
+                config_file = os.path.join(temp_dir, ".eslintrc")
+                with open(config_file, "w") as f:
                     f.write(DEFAULT_ESLINTRC)
                 with open(new_file, "w") as f:
                     f.write(code)
                 try:
-                    eslint_commands = ["npx", "eslint", new_file]
+                    eslint_commands = ["npx", "eslint", new_file, "--config", config_file, "--no-ignore"]
                     result = subprocess.run(
                         " ".join(eslint_commands),
                         capture_output=True,
                         text=True,
                         shell=True,
                         timeout=30,
                     )
@@ -612,46 +674,92 @@
 
 test_code = """
 x = "test"
 
 import numpy
 """
 
+def get_function_name(file_name: str, source_code: str, line_number: int):
+    ext = file_name.split(".")[-1]
+    if ext in extension_to_language:
+        language = extension_to_language[ext]
+    else:
+        return None
+    type_mapping_per_language = {
+        "python": "function_definition",
+        "tsx": "function_declaration",
+        "js": "function_declaration"
+    }
+    function_type_string = type_mapping_per_language.get(language)
+    parser = get_parser(language)
+
+    # Parse the source code
+    tree = parser.parse(bytes(source_code, 'utf8'))
+
+    # Get the root node of the syntax tree
+    root_node = tree.root_node
+
+    # Find the function node that contains the given line number
+    function_node = root_node.descendant_for_point_range((line_number, 0), (line_number, 1))
+
+    max_depth = 25 # Maximum depth to search for the function node
+    while function_node.type != function_type_string:
+        function_node = function_node.parent
+        max_depth -= 1
+        if max_depth == 0 or function_node is None:
+            return None
+
+    # Extract the function name
+    function_name = function_node.child_by_field_name('name').text.decode('utf8')
+
+    return function_name
+
 if __name__ == "__main__":
     # print(check_code("main.tsx", test_code))
     # print(get_check_results("main.py", test_code))
-    code = """import { isPossiblyValidEmail } from '../validation-utils'
-import { PulseValidationException } from '../pulse-exceptions'
-
-export function getEmailDomain (email: string): string {
-  if (!isPossiblyValidEmail(email)) {
-    throw new PulseValidationException(`Email is invalid: ${email}`)
-  }
-  // Emails are tough. An email can contain multiple '@' symbols.
-  // Thankfully, domains cannot contain @, so the domain will be
-  // part after the last @ in the email.
-  // e.g., "steve@macbook"@trilogy.com is a valid email.
-  //
-  const tokens = email.split('@')
-  return tokens[tokens.length - 1].toLowerCase().trim()
-}
-
-export function removeEmailAlias(email: string): string {
-  if (!isPossiblyValidEmail(email)) {
-    throw new PulseValidationException(`Email is invalid: ${email}`)
+    code = """import {
+    Flex,
+    Container,
+    Heading,
+    Stack,
+    Text,
+    Button,
+  } from "@chakra-ui/react";
+  import { tsParticles } from "tsparticles";
+  import { loadConfettiPreset } from "tsparticles-preset-confetti";
+  import { useState } from "react";
+  import logo from "../assets/icon.png";
   
-  }
-  const atIndex = email.lastIndexOf('@')
-  const aliasIndex = email.lastIndexOf('+', atIndex)
-
-  if (aliasIndex > 0) {
-    return email.substring(0, aliasIndex) + email.substring(atIndex)
-  }
+  import ExternalLinkWithText from "./ExternalLinkWithText";
+  import { TypeAnimation } from "react-type-animation";
+  import { FontAwesomeIcon } from '@fortawesome/react-fontawesome';
+  import { faUsers } from '@fortawesome/free-solid-svg-icons';
+  const demo = require("../assets/demo.mp4");
+  
+export default function CallToAction() {
+    const [spin, setSpin] = useState(false);
+    // const canvas = document.getElementById('canvas3d');
+    // const app = new Application(canvas);
+    // app.load('https://prod.spline.design/jzV1MbbHCyCmMG7u/scene.splinecode');
+    return (
+      <Container maxW={"5xl"}>
+      </Container>
+    );
+}
+"""
+   
+if __name__ == "__main__":
+    python_code = """import math
 
-  return email
-  }
+def get_circle_area(radius: float) -> float:
+    return math.pi * radius ** 2
 """
-    new_code = """console.log("hello world")"""
-    check_results = check_valid_typescript("test.ts",new_code)
+    function_name = get_function_name("main.ts", code, 20)
+    print(function_name)
+    function_name = get_function_name("main.py", python_code, 3)
+    print(function_name)
+    # new_code = """console.log("hello world")"""
+    # check_results = check_syntax("test.js", new_code)
+    check_results = get_check_results("test.tsx", code)
     import pdb
     # pylint: disable=no-member
     pdb.set_trace()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sweepai-2.0.2/sweepai/utils/utils_test.py` & `sweepai-2.1.0/sweepai/utils/utils_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/watch.py` & `sweepai-2.1.0/sweepai/watch.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/web/event_utils.py` & `sweepai-2.1.0/sweepai/web/event_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/web/events.py` & `sweepai-2.1.0/sweepai/web/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/web/health.py` & `sweepai-2.1.0/sweepai/web/health.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai/web/health_test.py` & `sweepai-2.1.0/sweepai/web/health_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.2/sweepai.egg-info/PKG-INFO` & `sweepai-2.1.0/sweepai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 2.0.2
+Version: 2.1.0
 Summary: Sweep fixes GitHub issues
 Author-email: Kevin Lu <kevin@sweep.dev>, William Zeng <william@sweep.dev>, Martin Ye <martin@sweep.dev>
 License: Sweep Enterprise Edition (EE) license (the “EE License”)
         Copyright (c) 2024-present Sweep AI, Inc.
         
         With regard to the Sweep Software:
         
@@ -38,16 +38,18 @@
 Requires-Dist: prometheus-fastapi-instrumentator==7.0.0
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: openai==1.13.3
 Requires-Dist: backoff==2.2.1
 Requires-Dist: pymongo==4.6.3
 Requires-Dist: gitpython==3.1.42
+Requires-Dist: stringzilla==3.8.4
 Requires-Dist: tree-sitter==0.21.0
 Requires-Dist: tree-sitter-python==0.21.0
+Requires-Dist: tree-sitter-javascript==0.21.0
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: rapidfuzz==3.6.2
 Requires-Dist: importmagic==0.1.7
 Requires-Dist: hatchet-sdk==0.18.0
 Requires-Dist: pyflakes==3.2.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: networkx==3.2.1
```

### Comparing `sweepai-2.0.2/sweepai.egg-info/SOURCES.txt` & `sweepai-2.1.0/sweepai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
+node_modules/flatted/python/flatted.py
+node_modules/flatted/python/test.py
 sweepai/__init__.py
 sweepai/api.py
 sweepai/api_test.py
 sweepai/cli.py
 sweepai/cli_test.py
 sweepai/global_threads.py
 sweepai/watch.py
@@ -17,28 +19,32 @@
 sweepai/agents/agent_utils.py
 sweepai/agents/assistant_functions.py
 sweepai/agents/assistant_wrapper.py
 sweepai/agents/assistant_wrapper_test.py
 sweepai/agents/complete_code.py
 sweepai/agents/complete_code_test.py
 sweepai/agents/distill_issue.py
+sweepai/agents/image_description_bot.py
+sweepai/agents/issue_cleanup_agent.py
 sweepai/agents/modify.py
 sweepai/agents/modify_bot.py
 sweepai/agents/modify_file.py
 sweepai/agents/pr_description_bot.py
 sweepai/agents/prune_modify_snippets.py
 sweepai/config/__init__.py
 sweepai/config/client.py
 sweepai/config/server.py
 sweepai/core/__init__.py
+sweepai/core/annotate_code_openai.py
 sweepai/core/chat.py
 sweepai/core/context_pruning.py
 sweepai/core/entities.py
 sweepai/core/external_searcher.py
 sweepai/core/lexical_search.py
+sweepai/core/planning_prompts.py
 sweepai/core/post_merge.py
 sweepai/core/pr_reader.py
 sweepai/core/prompts.py
 sweepai/core/reflection_utils.py
 sweepai/core/repo_parsing_utils.py
 sweepai/core/sweep_bot.py
 sweepai/core/update_prompts.py
@@ -65,14 +71,15 @@
 sweepai/utils/anthropic_client.py
 sweepai/utils/autoimport.py
 sweepai/utils/buttons.py
 sweepai/utils/buttons_test.py
 sweepai/utils/chat_logger.py
 sweepai/utils/code_tree.py
 sweepai/utils/code_tree_test.py
+sweepai/utils/cohere_utils.py
 sweepai/utils/comment_utils.py
 sweepai/utils/comment_utils_test.py
 sweepai/utils/convert_openai_anthropic.py
 sweepai/utils/diff.py
 sweepai/utils/diff_test.py
 sweepai/utils/docker_utils.py
 sweepai/utils/docker_utils_test.py
@@ -80,20 +87,23 @@
 sweepai/utils/file_utils.py
 sweepai/utils/fuzzy_diff.py
 sweepai/utils/fuzzy_diff_test.py
 sweepai/utils/github_utils.py
 sweepai/utils/github_utils_test.py
 sweepai/utils/hash.py
 sweepai/utils/html_extractor.py
+sweepai/utils/image_utils.py
+sweepai/utils/issue_validator.py
 sweepai/utils/modify_utils.py
 sweepai/utils/multi_query.py
 sweepai/utils/openai_listwise_reranker.py
 sweepai/utils/openai_proxy.py
 sweepai/utils/openai_proxy_test.py
 sweepai/utils/patch_utils.py
+sweepai/utils/previous_diff_utils.py
 sweepai/utils/progress.py
 sweepai/utils/progress_test.py
 sweepai/utils/prompt_constructor.py
 sweepai/utils/regex_utils.py
 sweepai/utils/safe_pqueue.py
 sweepai/utils/scorer.py
 sweepai/utils/scorer_test.py
@@ -102,19 +112,18 @@
 sweepai/utils/str_utils.py
 sweepai/utils/ticket_utils.py
 sweepai/utils/timer.py
 sweepai/utils/tree_utils.py
 sweepai/utils/user_settings.py
 sweepai/utils/utils.py
 sweepai/utils/utils_test.py
+sweepai/utils/validate_license.py
 sweepai/web/event_utils.py
 sweepai/web/events.py
 sweepai/web/health.py
 sweepai/web/health_test.py
+tests/test_context_pruning.py
+tests/test_get_gha_logs_from_pr.py
 tests/test_gha_extraction.py
 tests/test_jira_ticket.py
 tests/test_run_gha.py
-tests/test_watch.py
-vendor/tree-sitter-go/setup.py
-vendor/tree-sitter-go/bindings/python/tree_sitter_go/__init__.py
-vendor/tree-sitter-go/bindings/python/tree_sitter_go/__init__.pyi
-vendor/tree-sitter-go/bindings/python/tree_sitter_go/py.typed
+tests/test_watch.py
```

### Comparing `sweepai-2.0.2/sweepai.egg-info/requires.txt` & `sweepai-2.1.0/sweepai.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 prometheus-fastapi-instrumentator==7.0.0
 pyyaml==6.0.1
 python-dotenv==1.0.1
 openai==1.13.3
 backoff==2.2.1
 pymongo==4.6.3
 gitpython==3.1.42
+stringzilla==3.8.4
 tree-sitter==0.21.0
 tree-sitter-python==0.21.0
+tree-sitter-javascript==0.21.0
 tree-sitter-languages==1.10.2
 rapidfuzz==3.6.2
 importmagic==0.1.7
 hatchet-sdk==0.18.0
 pyflakes==3.2.0
 beautifulsoup4==4.12.3
 networkx==3.2.1
```

### Comparing `sweepai-2.0.2/tests/test_gha_extraction.py` & `sweepai-2.1.0/tests/test_gha_extraction.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,9 +12,8 @@
         return None
     logs = clean_gh_logs(logs)
     return logs
 
 RUN_ID = 8576903108
 REPO_FULL_NAME = "sweepai/sweep"
 
-logs = test_clean_gh_logs(RUN_ID, INSTALLATION_ID, REPO_FULL_NAME)
-breakpoint()
+logs = test_clean_gh_logs(RUN_ID, INSTALLATION_ID, REPO_FULL_NAME)
```

### Comparing `sweepai-2.0.2/tests/test_run_gha.py` & `sweepai-2.1.0/tests/test_run_gha.py`

 * *Files identical despite different names*

