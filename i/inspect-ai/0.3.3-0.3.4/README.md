# Comparing `tmp/inspect_ai-0.3.3.tar.gz` & `tmp/inspect_ai-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspect_ai-0.3.3.tar", last modified: Sun Apr 28 20:45:31 2024, max compression
+gzip compressed data, was "inspect_ai-0.3.4.tar", last modified: Wed May  1 18:12:02 2024, max compression
```

## Comparing `inspect_ai-0.3.3.tar` & `inspect_ai-0.3.4.tar`

### file list

```diff
@@ -1,367 +1,368 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.204771 inspect_ai-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.144770 inspect_ai-0.3.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.144770 inspect_ai-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.144770 inspect_ai-0.3.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-28 20:45:31.204771 inspect_ai-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.144770 inspect_ai-0.3.3/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/arc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.144770 inspect_ai-0.3.3/benchmarks/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/datasets/math_test.csv
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/datasets/mmlu.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/gpqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/gsm8k.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/hellaswag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/mathematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/benchmarks/mmlu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.148770 inspect_ai-0.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.152770 inspect_ai-0.3.3/docs/_examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/arc.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/biology_qa.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/footer.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/gsm8k.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/hellaswag.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/mathematics.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/popularity.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/security_guide.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/theory_of_mind.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_examples/tool_use.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.152770 inspect_ai-0.3.3/docs/_format/
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_format/pre-render.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/_variables.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/datasets.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/eval-logs.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/eval-suites.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10197 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/eval-tuning.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    35808 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/examples.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.160770 inspect_ai-0.3.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   170128 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/aisi-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68030 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/eval-log.png
--rw-r--r--   0 runner    (1001) docker     (127)   314093 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-answers.png
--rw-r--r--   0 runner    (1001) docker     (127)   280184 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-filter.png
--rw-r--r--   0 runner    (1001) docker     (127)   284131 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-history.png
--rw-r--r--   0 runner    (1001) docker     (127)   413188 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-home.png
--rw-r--r--   0 runner    (1001) docker     (127)   241738 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-info.png
--rw-r--r--   0 runner    (1001) docker     (127)   143202 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-logging-console.png
--rw-r--r--   0 runner    (1001) docker     (127)   155304 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-logging.png
--rw-r--r--   0 runner    (1001) docker     (127)   373146 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-main.png
--rw-r--r--   0 runner    (1001) docker     (127)   321793 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-messages.png
--rw-r--r--   0 runner    (1001) docker     (127)   165394 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-metadata.png
--rw-r--r--   0 runner    (1001) docker     (127)   272733 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-scoring.png
--rw-r--r--   0 runner    (1001) docker     (127)   274383 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/inspect-view-sort.png
--rw-r--r--   0 runner    (1001) docker     (127)    68787 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/popularity.png
--rw-r--r--   0 runner    (1001) docker     (127)    54252 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/rate-limit.png
--rw-r--r--   0 runner    (1001) docker     (127)    48461 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/images/running-theory.png
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/log-viewer.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/models.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/scorers.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/solvers.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/theme.scss
--rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/tools.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    12352 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/docs/workflow.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.160770 inspect_ai-0.3.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.136770 inspect_ai-0.3.3/examples/agents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.160770 inspect_ai-0.3.3/examples/agents/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/.env.example
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/inspect_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/wikipedia.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/agents/langchain/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/biology_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/popularity.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/security_guide.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/theory_of_mind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/examples/tool_use.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 20:45:31.204771 inspect_ai-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.136770 inspect_ai-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.160770 inspect_ai-0.3.3/src/inspect_ai/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.164770 inspect_ai-0.3.3/src/inspect_ai/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/score.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_cli/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.164770 inspect_ai-0.3.3/src/inspect_ai/_display/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_display/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_display/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_display/rich.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.164770 inspect_ai-0.3.3/src/inspect_ai/_eval/
--rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/score.py
--rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_eval/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.168770 inspect_ai-0.3.3/src/inspect_ai/_util/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/dotenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/url.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.168770 inspect_ai-0.3.3/src/inspect_ai/_view/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.172770 inspect_ai-0.3.3/src/inspect_ai/_view/www/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/App.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/api.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.172770 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.136770 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.172770 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (127)    85877 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   232903 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.172770 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   176196 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   130764 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.172770 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (127)    80615 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    31629 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/json5.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.176770 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/prism/
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/prism/prism-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/prism/prism.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/prism/prism.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/purify.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    75207 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/showdown.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/log-schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/log.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.176770 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/hooks.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.176770 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/htm/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/htm/htm.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/htm/preact.js
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/htm/preact.mjs
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/preact-hooks.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/preact.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.176770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/App.css
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/Constants.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/Register.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/AnsiDisplay.css
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/Card.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/ChatView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/Dialog.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/EmptyPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/LabeledValue.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/MessageContent.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/MetaDataView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/RenderedContent.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/TabSet.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/ToolButton.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/ansi-output.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/log-reader/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/log-reader/Native-Log-Reader.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/plan/
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/plan/PlanCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/samples/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/samples/SampleGroupSeparator.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/samples/SampleView.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/title/
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/title/TitleBlock.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.180770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/usage/UsageCard.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.184770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/utils/Format.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/utils/Git.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/utils/Path.mjs
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/utils/Type.mjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.184770 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs
--rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/_view/www/tools.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.184770 inspect_ai-0.3.3/src/inspect_ai/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.184770 inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/
--rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/bias_detection.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/biology_qa.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    32773 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/popularity.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/security_guide.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    31831 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.184770 inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/dataset/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.184770 inspect_ai-0.3.3/src/inspect_ai/log/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/log/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/log/_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.188770 inspect_ai-0.3.3/src/inspect_ai/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31676 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.188770 inspect_ai-0.3.3/src/inspect_ai/model/_providers/
--rw-r--r--   0 runner    (1001) docker     (127)    29724 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/azureai.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/bedrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/together.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_providers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/model/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.192771 inspect_ai-0.3.3/src/inspect_ai/scorer/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.192771 inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/std.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/scorer/_scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.192771 inspect_ai-0.3.3/src/inspect_ai/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_critique.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_multiple_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.192771 inspect_ai-0.3.3/src/inspect_ai/solver/_tool/
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_tool/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_tool/tool_def.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_tool/use_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_tool/web_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/solver/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.192771 inspect_ai-0.3.3/src/inspect_ai/util/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.196771 inspect_ai-0.3.3/src/inspect_ai/util/_context/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/util/_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/util/_context/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/util/_context/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/util/_context/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/src/inspect_ai/util/_context/subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/src/inspect_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-28 20:45:31.000000 inspect_ai-0.3.3/src/inspect_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-04-28 20:45:31.000000 inspect_ai-0.3.3/src/inspect_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 20:45:31.000000 inspect_ai-0.3.3/src/inspect_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-28 20:45:31.000000 inspect_ai-0.3.3/src/inspect_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-28 20:45:31.000000 inspect_ai-0.3.3/src/inspect_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 20:45:31.000000 inspect_ai-0.3.3/src/inspect_ai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.196771 inspect_ai-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_cloudlfare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_collapse_user_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_dataset/samples.csv
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_dataset/samples.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_dataset/samples.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_images/
--rw-r--r--   0 runner    (1001) docker     (127)   732622 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_images/images.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_list_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_logprobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_num_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_stop_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/attribs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/multiple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/multiple_dir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/multiple_dir/_decoy/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/multiple_dir/_decoy/testit.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/multiple_dir/_decoy2.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/multiple_dir/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/multiple_dir/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.140770 inspect_ai-0.3.3/tests/test_task_list/recurse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/recurse/.folder3/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/recurse/.folder3/epsilon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/recurse/folder1/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/recurse/folder1/_decoy.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/recurse/folder1/theta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/recurse/folder2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:45:31.200770 inspect_ai-0.3.3/tests/test_task_list/recurse/folder2/.folder3/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/recurse/folder2/.folder3/epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/recurse/folder2/another.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_task_list/recurse/folder2/first.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-28 20:45:25.000000 inspect_ai-0.3.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.080438 inspect_ai-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.024439 inspect_ai-0.3.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.024439 inspect_ai-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.024439 inspect_ai-0.3.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-01 18:12:02.080438 inspect_ai-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.028439 inspect_ai-0.3.4/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/arc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.028439 inspect_ai-0.3.4/benchmarks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/datasets/math_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/datasets/mmlu.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/gpqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/gsm8k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/hellaswag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/mathematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/benchmarks/mmlu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.028439 inspect_ai-0.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.032439 inspect_ai-0.3.4/docs/_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/arc.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/biology_qa.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/footer.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/gsm8k.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/hellaswag.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/mathematics.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/popularity.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/security_guide.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/theory_of_mind.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_examples/tool_use.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.032439 inspect_ai-0.3.4/docs/_format/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_format/pre-render.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/_variables.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/datasets.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/eval-logs.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/eval-suites.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10197 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/eval-tuning.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    35808 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/examples.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.040439 inspect_ai-0.3.4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   170128 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/aisi-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68030 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/eval-log.png
+-rw-r--r--   0 runner    (1001) docker     (127)   314093 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-answers.png
+-rw-r--r--   0 runner    (1001) docker     (127)   280184 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)   284131 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-history.png
+-rw-r--r--   0 runner    (1001) docker     (127)   413188 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-home.png
+-rw-r--r--   0 runner    (1001) docker     (127)   241738 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-info.png
+-rw-r--r--   0 runner    (1001) docker     (127)   143202 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-logging-console.png
+-rw-r--r--   0 runner    (1001) docker     (127)   155304 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-logging.png
+-rw-r--r--   0 runner    (1001) docker     (127)   373146 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-main.png
+-rw-r--r--   0 runner    (1001) docker     (127)   321793 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-messages.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165394 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-metadata.png
+-rw-r--r--   0 runner    (1001) docker     (127)   272733 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-scoring.png
+-rw-r--r--   0 runner    (1001) docker     (127)   274383 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-sort.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90624 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/inspect-view-splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68787 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/popularity.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54252 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/rate-limit.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48461 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/images/running-theory.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/log-viewer.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/models.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/scorers.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/solvers.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/tools.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    12352 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/docs/workflow.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.040439 inspect_ai-0.3.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.020439 inspect_ai-0.3.4/examples/agents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.040439 inspect_ai-0.3.4/examples/agents/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/.env.example
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/inspect_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/wikipedia.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/agents/langchain/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/biology_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/popularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/security_guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/theory_of_mind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/examples/tool_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:12:02.080438 inspect_ai-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.020439 inspect_ai-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.040439 inspect_ai-0.3.4/src/inspect_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.044439 inspect_ai-0.3.4/src/inspect_ai/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_cli/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.044439 inspect_ai-0.3.4/src/inspect_ai/_display/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_display/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_display/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_display/rich.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.044439 inspect_ai-0.3.4/src/inspect_ai/_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_eval/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.048439 inspect_ai-0.3.4/src/inspect_ai/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/dotenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.048439 inspect_ai-0.3.4/src/inspect_ai/_view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.048439 inspect_ai-0.3.4/src/inspect_ai/_view/www/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/App.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/api.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.020439 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    85877 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   232903 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   176196 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   130764 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    80615 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31629 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/json5.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/prism-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/prism.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/prism.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/purify.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    75207 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/showdown.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/log-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/log.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/hooks.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/htm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/htm/htm.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/htm/preact.js
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/htm/preact.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/preact-hooks.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/preact.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.052439 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/Constants.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/Register.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.056439 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/AnsiDisplay.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/Card.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ChatView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/CopyButton.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/Dialog.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/EmptyPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/LabeledValue.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/MessageContent.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/MetaDataView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/RenderedContent.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/TabSet.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ToolButton.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ansi-output.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.056439 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/log-reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/log-reader/Native-Log-Reader.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.056439 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.056439 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/plan/PlanCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SampleGroupSeparator.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SampleView.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/title/
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/title/TitleBlock.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/usage/UsageCard.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/utils/Format.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/utils/Git.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/utils/Path.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/utils/Type.mjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/_view/www/tools.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.060438 inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    20756 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/bias_detection.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/biology_qa.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    32773 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/popularity.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/security_guide.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    31831 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.064438 inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/dataset/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.064438 inspect_ai-0.3.4/src/inspect_ai/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/log/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/log/_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.064438 inspect_ai-0.3.4/src/inspect_ai/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31676 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.068439 inspect_ai-0.3.4/src/inspect_ai/model/_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)    29724 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/azureai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/bedrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/together.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_providers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/model/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.068439 inspect_ai-0.3.4/src/inspect_ai/scorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.068439 inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/scorer/_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.068439 inspect_ai-0.3.4/src/inspect_ai/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_critique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_multiple_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.072439 inspect_ai-0.3.4/src/inspect_ai/solver/_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_tool/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_tool/tool_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_tool/use_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_tool/web_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/solver/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.072439 inspect_ai-0.3.4/src/inspect_ai/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.072439 inspect_ai-0.3.4/src/inspect_ai/util/_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/util/_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/util/_context/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/util/_context/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/util/_context/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/src/inspect_ai/util/_context/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.080438 inspect_ai-0.3.4/src/inspect_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-01 18:12:01.000000 inspect_ai-0.3.4/src/inspect_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10841 2024-05-01 18:12:02.000000 inspect_ai-0.3.4/src/inspect_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:12:01.000000 inspect_ai-0.3.4/src/inspect_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 18:12:01.000000 inspect_ai-0.3.4/src/inspect_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-01 18:12:01.000000 inspect_ai-0.3.4/src/inspect_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 18:12:01.000000 inspect_ai-0.3.4/src/inspect_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_cloudlfare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_collapse_user_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_dataset/samples.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_dataset/samples.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_dataset/samples.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_eval_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_images/
+-rw-r--r--   0 runner    (1001) docker     (127)   732622 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_images/images.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_list_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_logprobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_num_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_stop_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_task_list/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/attribs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/multiple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_task_list/multiple_dir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_task_list/multiple_dir/_decoy/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/multiple_dir/_decoy/testit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/multiple_dir/_decoy2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/multiple_dir/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/multiple_dir/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.024439 inspect_ai-0.3.4/tests/test_task_list/recurse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_task_list/recurse/.folder3/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/recurse/.folder3/epsilon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.076439 inspect_ai-0.3.4/tests/test_task_list/recurse/folder1/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/recurse/folder1/_decoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/recurse/folder1/theta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.080438 inspect_ai-0.3.4/tests/test_task_list/recurse/folder2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:12:02.080438 inspect_ai-0.3.4/tests/test_task_list/recurse/folder2/.folder3/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/recurse/folder2/.folder3/epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/recurse/folder2/another.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_task_list/recurse/folder2/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-01 18:11:56.000000 inspect_ai-0.3.4/tests/utils.py
```

### Comparing `inspect_ai-0.3.3/.github/workflows/build.yml` & `inspect_ai-0.3.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/.github/workflows/docs.yml` & `inspect_ai-0.3.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/.github/workflows/pypi.yml` & `inspect_ai-0.3.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/.gitignore` & `inspect_ai-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/.pre-commit-config.yaml` & `inspect_ai-0.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/CHANGELOG.md` & `inspect_ai-0.3.4/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## v0.3.4 (01 May 2024)
+
+- `write_eval_log()` now ignores unserializable objects in metadata fields.
+- `read_eval_log()` now takes a `str` or `FileInfo` (for compatibility w/ list returned from `list_eval_logs()`).
+- Registry name looks are now case sensitive (fixes issue w/ loading tasks w/ mixed case names).
+- Resiliancy to Python syntax errors that occur when enumerating tasks in a directory.
+- Do not throw error if unable to parse or load `.ipynb` file due to lack of dependencies (e.g. `nbformat`).
+- Various additions to log viewer display (log file name, dataset/scorer in listing, filter by complex score types).
+- Improvements to markdown rendering in log viewer (don't render intraword underscores, escape html tags).
+
 ## v0.3.3 (28 April 2024)
 
 - `inspect view` command for viewing eval log files.
 - `Score` now has an optional `answer` field, which denotes the answer text extracted from model output.
 - Accuracy metrics now take an optional `ValueToFloat` function for customizing how textual values mapped to float.
 - Made `model_graded_qa` more flexible with separate `instruction` template and `grade_pattern`, as well providing `partial_credit` as an option.
 - Modify the default templates for `chain_of_thought()` and `self_critique()` to instruct the model to reply with `ANSWER: $ANSWER` at the end on its own line.
```

### Comparing `inspect_ai-0.3.3/LICENSE` & `inspect_ai-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/PKG-INFO` & `inspect_ai-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspect_ai
-Version: 0.3.3
+Version: 0.3.4
 Summary: Framework for large language model evaluations
 Author: UK AI Safety Institute
 License: MIT License
 Project-URL: Documentation, https://UKGovernmentBEIS.github.io/inspect_ai/
 Project-URL: Source Code, https://github.com/UKGovernmentBEIS/inspect_ai
 Project-URL: Issue Tracker, https://github.com/UKGovernmentBEIS/inspect_ai/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `inspect_ai-0.3.3/README.md` & `inspect_ai-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/benchmarks/README.md` & `inspect_ai-0.3.4/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/benchmarks/arc.py` & `inspect_ai-0.3.4/benchmarks/arc.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/benchmarks/gpqa.py` & `inspect_ai-0.3.4/benchmarks/gpqa.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/benchmarks/gsm8k.py` & `inspect_ai-0.3.4/benchmarks/gsm8k.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/benchmarks/hellaswag.py` & `inspect_ai-0.3.4/benchmarks/hellaswag.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/benchmarks/mathematics.py` & `inspect_ai-0.3.4/benchmarks/mathematics.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/benchmarks/mmlu.py` & `inspect_ai-0.3.4/benchmarks/mmlu.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/_examples/arc.qmd` & `inspect_ai-0.3.4/docs/_examples/arc.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/_examples/biology_qa.qmd` & `inspect_ai-0.3.4/docs/_examples/biology_qa.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/_examples/footer.qmd` & `inspect_ai-0.3.4/docs/_examples/footer.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/_examples/gsm8k.qmd` & `inspect_ai-0.3.4/docs/_examples/gsm8k.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/_examples/hellaswag.qmd` & `inspect_ai-0.3.4/docs/_examples/hellaswag.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/_examples/index.qmd` & `inspect_ai-0.3.4/docs/_examples/index.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/_examples/mathematics.qmd` & `inspect_ai-0.3.4/docs/_examples/mathematics.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/_examples/popularity.qmd` & `inspect_ai-0.3.4/docs/_examples/popularity.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/_examples/security_guide.qmd` & `inspect_ai-0.3.4/docs/_examples/security_guide.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/_examples/theory_of_mind.qmd` & `inspect_ai-0.3.4/docs/_examples/theory_of_mind.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/_examples/tool_use.qmd` & `inspect_ai-0.3.4/docs/_examples/tool_use.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/_quarto.yml` & `inspect_ai-0.3.4/docs/_quarto.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 project:
    type: book
    pre-render:
       -  _format/pre-render.sh
   
 book:
    title: "Inspect"
-   subtitle: "A framework for large language model evaluations"
+   subtitle: "An open-source framework for large language model evaluations"
    page-navigation: true
    repo-url: https://github.com/UKGovernmentBEIS/inspect_ai
    site-url: https://UKGovernmentBEIS.github.io/inspect_ai/
    repo-actions: [issue]
    downloads: [pdf, epub, docx]
    twitter-card:
-      description: "A framework for large language model evaluations"
+      description: "Open-source framework for large language model evaluations"
    open-graph: 
-      description: "A framework for large language model evaluations"
+      description: "Open-source framework for large language model evaluations"
    sidebar:
       header: >
          [![](images/aisi-logo.png)](https://www.gov.uk/government/organisations/ai-safety-institute)
 
    page-footer: 
       left: 
          - text: UK AI Safety Institute
```

### Comparing `inspect_ai-0.3.3/docs/datasets.qmd` & `inspect_ai-0.3.4/docs/datasets.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/eval-logs.qmd` & `inspect_ai-0.3.4/docs/eval-logs.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/eval-suites.qmd` & `inspect_ai-0.3.4/docs/eval-suites.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/eval-tuning.qmd` & `inspect_ai-0.3.4/docs/eval-tuning.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/examples.qmd` & `inspect_ai-0.3.4/docs/examples.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/aisi-logo.png` & `inspect_ai-0.3.4/docs/images/aisi-logo.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/eval-log.png` & `inspect_ai-0.3.4/docs/images/eval-log.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/inspect-view-answers.png` & `inspect_ai-0.3.4/docs/images/inspect-view-answers.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/inspect-view-filter.png` & `inspect_ai-0.3.4/docs/images/inspect-view-filter.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/inspect-view-history.png` & `inspect_ai-0.3.4/docs/images/inspect-view-history.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/inspect-view-home.png` & `inspect_ai-0.3.4/docs/images/inspect-view-home.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/inspect-view-info.png` & `inspect_ai-0.3.4/docs/images/inspect-view-info.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/inspect-view-logging-console.png` & `inspect_ai-0.3.4/docs/images/inspect-view-logging-console.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/inspect-view-logging.png` & `inspect_ai-0.3.4/docs/images/inspect-view-logging.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/inspect-view-main.png` & `inspect_ai-0.3.4/docs/images/inspect-view-main.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/inspect-view-messages.png` & `inspect_ai-0.3.4/docs/images/inspect-view-messages.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/inspect-view-metadata.png` & `inspect_ai-0.3.4/docs/images/inspect-view-metadata.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/inspect-view-scoring.png` & `inspect_ai-0.3.4/docs/images/inspect-view-scoring.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/inspect-view-sort.png` & `inspect_ai-0.3.4/docs/images/inspect-view-sort.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/popularity.png` & `inspect_ai-0.3.4/docs/images/popularity.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/rate-limit.png` & `inspect_ai-0.3.4/docs/images/rate-limit.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/images/running-theory.png` & `inspect_ai-0.3.4/docs/images/running-theory.png`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/index.qmd` & `inspect_ai-0.3.4/docs/index.qmd`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+---
+toc: false
+---
+
+::: {layout=[45,55] .splash}
+
+- Easy creation of simple benchmark-style evaluations.
+
+- Scale up to more sophsisticated evals with multi-turn dialog, agent scaffolds and model grading.
+
+- Interactive workflows for researchers; production workflows for larger evaluation suites. 
+
+- Adapt and extend the framework with custom Python components.
+
+![](images/inspect-view-splash.png){.lightbox .border}
+
+:::
+
 ## Welcome
 
 Welcome to Inspect, a framework for large language model evaluations created by the [UK AI Safety Institute](https://www.gov.uk/government/organisations/ai-safety-institute).
 
 Inspect provides many built-in components, including facilities for prompt engineering, tool usage, multi-turn dialog, and model graded evaluations. Extensions to Inspect (e.g. to support new elicitation and scoring techniques) can be provided by other Python packages.
 
 We'll walk through a fairly trivial "Hello, Inspect" example below. Read on to learn the basics, then read the documentation on [Workflow](#sec-workflow), [Solvers](#sec-solvers), [Tools](#sec-tools), [Scorers](#sec-scorers), [Datasets](#sec-datasets), and [Models](#sec-models) to learn how to create more advanced evaluations.
```

### Comparing `inspect_ai-0.3.3/docs/log-viewer.qmd` & `inspect_ai-0.3.4/docs/log-viewer.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/models.qmd` & `inspect_ai-0.3.4/docs/models.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/scorers.qmd` & `inspect_ai-0.3.4/docs/scorers.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/solvers.qmd` & `inspect_ai-0.3.4/docs/solvers.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/tools.qmd` & `inspect_ai-0.3.4/docs/tools.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/docs/workflow.qmd` & `inspect_ai-0.3.4/docs/workflow.qmd`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/examples/agents/langchain/README.md` & `inspect_ai-0.3.4/examples/agents/langchain/README.md`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/examples/agents/langchain/inspect_langchain.py` & `inspect_ai-0.3.4/examples/agents/langchain/inspect_langchain.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/examples/agents/langchain/wikipedia.jsonl` & `inspect_ai-0.3.4/examples/agents/langchain/wikipedia.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/examples/agents/langchain/wikipedia.py` & `inspect_ai-0.3.4/examples/agents/langchain/wikipedia.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/examples/biology_qa.py` & `inspect_ai-0.3.4/examples/biology_qa.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/examples/popularity.py` & `inspect_ai-0.3.4/examples/popularity.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/examples/security_guide.py` & `inspect_ai-0.3.4/examples/security_guide.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/examples/theory_of_mind.py` & `inspect_ai-0.3.4/examples/theory_of_mind.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/examples/tool_use.py` & `inspect_ai-0.3.4/examples/tool_use.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/pyproject.toml` & `inspect_ai-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/__init__.py` & `inspect_ai-0.3.4/src/inspect_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_cli/common.py` & `inspect_ai-0.3.4/src/inspect_ai/_cli/common.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_cli/eval.py` & `inspect_ai-0.3.4/src/inspect_ai/_cli/eval.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_cli/info.py` & `inspect_ai-0.3.4/src/inspect_ai/_cli/info.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_cli/list.py` & `inspect_ai-0.3.4/src/inspect_ai/_cli/list.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_cli/main.py` & `inspect_ai-0.3.4/src/inspect_ai/_cli/main.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_cli/score.py` & `inspect_ai-0.3.4/src/inspect_ai/_cli/score.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_cli/util.py` & `inspect_ai-0.3.4/src/inspect_ai/_cli/util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_cli/view.py` & `inspect_ai-0.3.4/src/inspect_ai/_cli/view.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_display/_display.py` & `inspect_ai-0.3.4/src/inspect_ai/_display/_display.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_display/logger.py` & `inspect_ai-0.3.4/src/inspect_ai/_display/logger.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_display/rich.py` & `inspect_ai-0.3.4/src/inspect_ai/_display/rich.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_eval/eval.py` & `inspect_ai-0.3.4/src/inspect_ai/_eval/eval.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_eval/images.py` & `inspect_ai-0.3.4/src/inspect_ai/_eval/images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_eval/list.py` & `inspect_ai-0.3.4/src/inspect_ai/_eval/list.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from importlib.util import module_from_spec, spec_from_loader
 from logging import getLogger
 from pathlib import Path
 from types import ModuleType
 from typing import Any, Callable
 
 from inspect_ai._util.dotenv import dotenv_environ
-from inspect_ai._util.error import exception_message, pip_dependency_error
+from inspect_ai._util.error import exception_message
 from inspect_ai._util.file import file
 from inspect_ai._util.path import chdir_python
 from inspect_ai._util.registry import RegistryInfo, is_registry_object, registry_info
 from inspect_ai.model import ModelName
 
 from .registry import task_create
 from .task import TASK_FILE_ATTR, TASK_RUN_DIR_ATTR, Task, TaskInfo
@@ -227,17 +227,15 @@
         loader.exec_module(module)
         return module
 
     elif task_path.suffix == ".ipynb":
         try:
             from inspect_ai._util.notebook import NotebookLoader
         except ImportError:
-            raise pip_dependency_error(
-                "Loading tasks from notebooks", ["ipython", "nbformat"]
-            )
+            return None
 
         # bail if the code doesn't have a task
         def exec_filter(cells: list[str]) -> bool:
             code = "\n\n".join(cells)
             return code_has_task(code)
 
         notebook_loader = NotebookLoader(exec_filter)
@@ -246,64 +244,71 @@
     else:
         raise ModuleNotFoundError(
             f"Invalid extension for task file: {task_path.suffix}"
         )
 
 
 def code_has_task(code: str) -> bool:
-    tree = ast.parse(code)
-    for node in ast.iter_child_nodes(tree):
-        if isinstance(node, ast.FunctionDef):
-            for decorator in node.decorator_list:
-                if isinstance(decorator, ast.Name):
-                    if str(decorator.id) == "task":
-                        return True
-                elif isinstance(decorator, ast.Call):
-                    if isinstance(decorator.func, ast.Name):
-                        if str(decorator.func.id) == "task":
+    try:
+        tree = ast.parse(code)
+        for node in ast.iter_child_nodes(tree):
+            if isinstance(node, ast.FunctionDef):
+                for decorator in node.decorator_list:
+                    if isinstance(decorator, ast.Name):
+                        if str(decorator.id) == "task":
                             return True
+                    elif isinstance(decorator, ast.Call):
+                        if isinstance(decorator.func, ast.Name):
+                            if str(decorator.func.id) == "task":
+                                return True
+    except SyntaxError:
+        pass
+
     return False
 
 
 def parse_tasks(path: Path, root_dir: Path, absolute: bool) -> list[TaskInfo]:
     # read code from python source file
     if path.suffix.lower() == ".py":
         with file(path.as_posix(), "r", encoding="utf-8") as f:
             code = f.read()
 
     # read code from notebook
     elif path.suffix.lower() == ".ipynb":
         try:
             from inspect_ai._util.notebook import read_notebook_code
         except ImportError:
-            raise pip_dependency_error(
-                "Parsing tasks from notebooks", ["ipython", "nbformat"]
-            )
+            return []
+
         code = read_notebook_code(path)
 
     # unsupported file type
     else:
         raise ModuleNotFoundError(f"Invalid extension for task file: {path.suffix}")
 
     # parse the top level tasks out of the code
     tasks: list[TaskInfo] = []
-    tree = ast.parse(code)
-    for node in ast.iter_child_nodes(tree):
-        if isinstance(node, ast.FunctionDef):
-            for decorator in node.decorator_list:
-                result = parse_decorator(node, decorator)
-                if result:
-                    name, attribs = result
-                    tasks.append(
-                        TaskInfo(
-                            file=task_path(path, root_dir, absolute),
-                            name=name,
-                            attribs=attribs,
+    try:
+        tree = ast.parse(code)
+        for node in ast.iter_child_nodes(tree):
+            if isinstance(node, ast.FunctionDef):
+                for decorator in node.decorator_list:
+                    result = parse_decorator(node, decorator)
+                    if result:
+                        name, attribs = result
+                        tasks.append(
+                            TaskInfo(
+                                file=task_path(path, root_dir, absolute),
+                                name=name,
+                                attribs=attribs,
+                            )
                         )
-                    )
+    except SyntaxError:
+        pass
+
     return tasks
 
 
 def parse_decorator(
     node: ast.FunctionDef, decorator: ast.expr
 ) -> tuple[str, dict[str, Any]] | None:
     if isinstance(decorator, ast.Name):
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_eval/loader.py` & `inspect_ai-0.3.4/src/inspect_ai/_eval/loader.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_eval/log.py` & `inspect_ai-0.3.4/src/inspect_ai/_eval/log.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_eval/registry.py` & `inspect_ai-0.3.4/src/inspect_ai/_eval/registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_eval/score.py` & `inspect_ai-0.3.4/src/inspect_ai/_eval/score.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_eval/task.py` & `inspect_ai-0.3.4/src/inspect_ai/_eval/task.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_util/dotenv.py` & `inspect_ai-0.3.4/src/inspect_ai/_util/dotenv.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_util/error.py` & `inspect_ai-0.3.4/src/inspect_ai/_util/error.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_util/file.py` & `inspect_ai-0.3.4/src/inspect_ai/_util/file.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_util/git.py` & `inspect_ai-0.3.4/src/inspect_ai/_util/git.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_util/http.py` & `inspect_ai-0.3.4/src/inspect_ai/_util/http.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_util/images.py` & `inspect_ai-0.3.4/src/inspect_ai/_util/images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_util/json.py` & `inspect_ai-0.3.4/src/inspect_ai/_util/json.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_util/notebook.py` & `inspect_ai-0.3.4/src/inspect_ai/_util/notebook.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import sys
 import types
 from pathlib import Path
 from typing import Callable
 
 from IPython import get_ipython  # type: ignore
 from IPython.core.interactiveshell import InteractiveShell
-from nbformat import read
+from nbformat import NBFormatError, ValidationError, read
+from nbformat.reader import NotJSONError
 
 # from https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Importing%20Notebooks.html
 
 
 class NotebookLoader(object):
     """Module Loader for Jupyter Notebooks"""
 
@@ -60,17 +61,24 @@
 
             return mod
         finally:
             self.shell.user_ns = save_user_ns
 
 
 def read_notebook_code(path: Path) -> str:
-    # load the notebook object
-    with io.open(path, "r", encoding="utf-8") as f:
-        nb = read(f, 4)  # type: ignore
+    try:
+        # load the notebook object
+        with io.open(path, "r", encoding="utf-8") as f:
+            nb = read(f, 4)  # type: ignore
+    except NotJSONError:
+        return ""
+    except ValidationError:
+        return ""
+    except NBFormatError:
+        return ""
 
     # for dealing w/ magics
     shell = InteractiveShell.instance()
 
     # get the code
     lines: list[str] = []
     for cell in nb.cells:
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_util/path.py` & `inspect_ai-0.3.4/src/inspect_ai/_util/path.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_util/platform.py` & `inspect_ai-0.3.4/src/inspect_ai/_util/platform.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_util/registry.py` & `inspect_ai-0.3.4/src/inspect_ai/_util/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 def registry_name(o: object, name: str) -> str:
     r"""Compute the registry name of an object.
 
     This function checks whether the passsed object is in a package,
     and if it is, preprends the package name as a namespace
     """
     package = get_package_name(o)
-    return (f"{package}/{name}" if package else name).lower()
+    return f"{package}/{name}" if package else name
 
 
 def registry_lookup(type: RegistryType, name: str) -> object | None:
     r"""Lookup an object in the registry by type and name.
 
     Objects that defined in inspect extension packages (i.e. not
     directly within the core inspect_ai package) must be namespaced
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_util/retry.py` & `inspect_ai-0.3.4/src/inspect_ai/_util/retry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_util/url.py` & `inspect_ai-0.3.4/src/inspect_ai/_util/url.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/schema.py` & `inspect_ai-0.3.4/src/inspect_ai/_view/schema.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/view.py` & `inspect_ai-0.3.4/src/inspect_ai/_view/view.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/App.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/App.mjs`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import { client_events, eval_logs } from "api";
 
 import "./src/Register.mjs";
 
 import { icons } from "./src/Constants.mjs";
 import { WorkSpace } from "./src/workspace/WorkSpace.mjs";
 import { eval_log } from "./api.mjs";
+import { CopyButton } from "./src/components/CopyButton.mjs";
 
 export function App() {
   const [selected, setSelected] = useState(0);
   const [logs, setLogs] = useState({ log_dir: "", files: [] });
   const [logHeaders, setLogHeaders] = useState({});
   const [offcanvas, setOffcanvas] = useState(false);
 
@@ -85,15 +86,15 @@
   // Configure an app envelope specific to the current state
   // if there are no log files, then don't show sidebar
   const fullScreen = logs.files.length === 1 && !logs.log_dir;
 
   const appEnvelope = fullScreen
     ? ""
     : html`
-        <${Header} logs=${logs} offcanvas=${offcanvas} />
+        <${Header} logs=${logs} selected=${selected} offcanvas=${offcanvas} />
         <${Sidebar}
           logs=${logs}
           logHeaders=${logHeaders}
           offcanvas=${offcanvas}
           selected=${selected}
           onSelected=${(index) => {
             setSelected(index);
@@ -119,14 +120,22 @@
     </div>
   `;
 }
 
 const Header = (props) => {
   const toggleOffCanClass = props.offcanvas ? "" : " d-md-none";
   const gearOffCanClass = props.offcanvas ? "" : " d-md-inline";
+
+  const logFiles = props.logs.files || [];
+  const logSelected = props.selected || 0;
+  const logUri = logFiles.length > logSelected ? logFiles[logSelected].name : "";
+  const logName =logUri.split('/').pop();
+  
+
+
   return html`
     <nav class="navbar sticky-top shadow-sm" style=${{ flexWrap: "nowrap" }}>
       <div class="container-fluid">
         <span
           class="navbar-brand mb-0"
           style=${{ display: "flex", alignItems: "center" }}
         >
@@ -148,27 +157,27 @@
           </button>
           <i
             class="${icons.inspect} d-none ${gearOffCanClass}"
             style=${{ marginRight: "0.3rem" }}
           ></i>
           <span> Inspect View </span>
         </span>
-        <span
+        <div
           class="navbar-text"
           style=${{
             paddingTop: "0.3rem",
             paddingBottom: 0,
-            fontSize: "1rem",
+            fontSize: "0.8rem",
             whiteSpace: "nowrap",
             textOverflow: "ellipsis",
             overflow: "hidden",
           }}
         >
-          ${props.logs.log_dir}
-        </span>
+          ${logName}<${CopyButton} value=${logUri}/>
+        </div>
       </div>
     </nav>
   `;
 };
 
 const Sidebar = (props) => {
   const btnOffCanClass = props.offcanvas ? "" : " d-md-none";
@@ -214,14 +223,17 @@
           const time = new Date(file.mtime);
           const logHeader = logHeaders[file.name];
           const hyperparameters = logHeader ? {
             ...logHeader.plan?.config,
             ...logHeader.eval?.task_args,
           } : undefined;
 
+          const model = logHeader?.eval?.model;
+          const dataset = logHeader?.eval?.dataset;
+          const scorer = logHeader?.results?.scorer?.name;
           
           return html`
             <li
               class="list-group-item list-group-item-action${active}"
               onclick=${() => props.onSelected(index)}
               style=${{ fontSize: "0.8rem" }}
             >
@@ -231,33 +243,29 @@
                   flexDirection: "row",
                   justifyContent: "space-between",
                 }}
               >
                 <div>
                   <div
                     style=${{
-                      fontSize: "1.4em",
+                      fontSize: "1.5em",
                       fontWeight: "600",
                     }}
                   >
                     ${logHeader?.eval?.task || file.task}
                   </div>
                   <small class="mb-1 text-muted">
                     ${time.toDateString()}
                     ${time.toLocaleTimeString([], {
                       hour: "2-digit",
                       minute: "2-digit",
                     })}
                   </small>
 
-                  ${logHeader?.eval?.model
-                    ? html` <div>
-                        <small> ${logHeader?.eval.model} </small>
-                      </div>`
-                    : ""}
+                  ${model ? html` <div><small class="mb-1 text-muted">${model}</small></div>`: ""}
                 </div>
                 ${logHeader?.results?.metrics
                   ? html`<div style=${{display: "flex", flexDirection: "row", flexWrap: "wrap", justifyContent: "flex-end" }}>
                           
                       ${Object.keys(logHeader?.results.metrics).map(
                         (metric) => {
                           return html`
@@ -270,33 +278,37 @@
                               }}
                             >
                               <div
                                 style=${{ fontWeight: 300 }}
                               >
                                 ${logHeader?.results.metrics[metric].name}
                                 </div>
-                              <div style=${{fontWeight: 600, fontSize: "1.4em"}}>
+                              <div style=${{fontWeight: 600, fontSize: "1.5em"}}>
                                 ${formatPrettyDecimal(
                                   logHeader?.results.metrics[metric].value
                                 )}
                               </div>
                             </div>
                           `;
                         }
                       )}
                     </div>`
                   : logHeader?.status === "error" ? html`<div style=${{color: "var(--bs-danger)"}}>Eval Error</div>` : ""}
               </div>
-              <small style=${{ marginTop: "0.4em" }}>
+              <div style=${{ marginTop: "0.4em" }}>
+              <small class="mb-1 text-muted">
               ${
                 hyperparameters ? Object.keys((hyperparameters)).map((key) => {
                   return `${key}: ${hyperparameters[key]}`
                 }).join(", ") : ""
               } 
               </small>
+              </div>
+              ${dataset || scorer ? html`<div style=${{display: "flex", justifyContent: "space-between", marginTop: "0.5em" }}><span>dataset: ${dataset.name || "(samples)"}</span><span>scorer: ${scorer}</span></div>` : ""}
+
             </li>
           `;
         })}
       </ul>
     </div>
   `;
 };
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/api.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/api.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/favicon.svg` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/favicon.svg`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/index.html` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -51,12 +51,12 @@
     <script src="./libs/prism/prism.min.js"></script>
     <script src="./libs/clipboard.min.js"></script>
     <script src="./libs/json5.min.js"></script>
     <script src="./libs/purify.min.js"></script>
     <script src="./libs/showdown.min.js"></script>
     <script>
       window.document.addEventListener("DOMContentLoaded", function (_event) {
-        new ClipboardJS(".clipboard-button");
+        new ClipboardJS(".clipboard-button,.copy-button");
       });
     </script>
   </body>
 </html>
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/clipboard.min.js` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/json5.min.js` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/json5.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/prism/prism-dark.css` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/prism-dark.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/prism/prism.min.css` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/prism.min.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/prism/prism.min.js` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/prism/prism.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/purify.min.js` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/purify.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/libs/showdown.min.js` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/libs/showdown.min.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/log-schema.json` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/log-schema.json`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/log.d.ts` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/log.d.ts`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/hooks.js` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/hooks.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/htm/htm.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/htm/htm.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/preact/preact.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/preact/preact.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/App.css` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/App.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/Constants.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/Constants.mjs`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     right: "bi bi-arrow-right",
     down: "bi bi-arrow-down",
   },
   "collapse-all": "bi bi-arrows-collapse",
   "close": "bi bi-x",
   config: "bi bi-gear",
   confirm: "bi bi-check",
-  copy: "bi bi-clipboard",
+  copy: "bi bi-copy",
 
   epoch: (epoch) => {
     return `bi bi-${epoch}-circle`;
   },
   error: "bi bi-exclamation-circle",
   "expand-all": "bi bi-arrows-expand",
   inspect: "bi bi-gear",
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/AnsiDisplay.css` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/AnsiDisplay.css`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/Card.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/Card.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/ChatView.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ChatView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/Dialog.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/Dialog.mjs`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
       class="modal fade ${classes}"
       id="${id}"
       tabindex="-1"
       aria-hidden="true"
       styles=${{ ...styles }}
     >
       <div
-        class="modal-dialog ${centered
+        class="modal-dialog modal-lg ${centered
           ? "modal-dialog-centered"
           : ""} ${scrollable ? "modal-dialog-scrollable" : ""}"
       >
         <div class="modal-content">
           <div class="modal-header">
             <h5 class="modal-title">${title}</h5>
             <button
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ErrorPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/LabeledValue.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/LabeledValue.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/LoadingScreen.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import { html } from "htm/preact";
 
 showdown.setOption('simpleLineBreaks', true);
+showdown.setOption('literalMidWordUnderscores', true);
 const converter = new showdown.Converter();
 
 
 export const MarkdownDiv = (props) => {
   const { markdown, style } = props;
+  
+  // Escape all HTML tags
+  const escaped = DOMPurify.sanitize(markdown, { ALLOWED_TAGS: []});
 
   // Pre-render any text that isn't handled by markdown
-  const preRenderedMarkdown = preRenderAlphaLists(markdown);
+  const preRendered = preRenderAlphaLists(escaped);
+  const renderedHtml = converter.makeHtml(preRendered);
 
-  // Render the markdown and sanitize the output
-  const dirtyHtml = converter.makeHtml(preRenderedMarkdown);
-  const cleanHtml = DOMPurify.sanitize(dirtyHtml);
-  
   // Return the rendered markdown
-  const markup = { __html: cleanHtml };
+  const markup = { __html: renderedHtml };
   return html`<div dangerouslySetInnerHTML=${markup} style=${style} class="${props.class ? props.class : ''} markdown-content" />`;
 };
 
 
 // Special handling for ordered lists that look like
 // multiple choice (e.g. a), b), c), d) etc..)
 const kLetterListPattern = /^([a-zA-Z][\)\.]\s.*?)$/gm;
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/MessageContent.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/MessageContent.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/MetaDataView.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/MetaDataView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/RenderedContent.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/RenderedContent.mjs`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,15 @@
             centered=true
             scrollable=true
             style=${{
               fontSize: "0.8em",
               maxWidth: "650px",
             }}
           >
-            <pre><code class="sourceCode" dangerouslySetInnerHTML="${{
+            <pre><code class="sourceCode" style=${{ whiteSpace: "pre-wrap" }} dangerouslySetInnerHTML="${{
               __html: DOMPurify.sanitize(highlightedHtml),
             }}">
             </code></pre>
           </${DialogAfterBody}>`,
       };
     },
   },
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/TabSet.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/TabSet.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/components/ansi-output.js` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/components/ansi-output.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/log-reader/Log-Reader.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/log-reader/Open-AI-Log-Reader.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/logging/LoggingPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/plan/PlanCard.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/plan/PlanCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SampleScoreView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/samples/SampleView.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SampleView.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/samples/SamplesCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/title/TitleBlock.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/title/TitleBlock.mjs`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import { html } from "htm/preact";
 
 import { icons } from "../Constants.mjs";
 import { LabeledValue } from "../components/LabeledValue.mjs";
-import { formatPrettyDecimal } from "../utils/Format.mjs";
+import { formatPrettyDecimal, formatDataset } from "../utils/Format.mjs";
 
 export const TitleBlock = ({
   title,
   subtitle,
   tertiaryTitle,
   log,
   metrics,
@@ -156,28 +156,20 @@
 };
 
 const DatasetSummary = ({ dataset, samples, epochs, style }) => {
   if (!dataset) {
     return "";
   }
 
-  const sampleCount = epochs > 0 ? samples.length / epochs : samples;
-  console
-
   return html`
     <div style=${style}>
       ${dataset.name}${samples?.length
-        ? html` <span
-            style=${{ fontSize: "0.9em" }}
-          >
-            ${dataset.name ? "— " : ""}${sampleCount + " "}${epochs > 1
-              ? `x ${epochs} `
-              : ""}
-            ${samples.length === 1 ? "sample" : "samples"}</span
-          >`
+        ? html` <span style=${{ fontSize: "0.9em" }}>
+          ${formatDataset(dataset.name, samples.length, epochs)}
+          </span>`
         : ""}
     </div>
   `;
 };
 
 const ScorerSummary = ({ scorer }) => {
   if (!scorer) {
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/usage/ModelTokenTable.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/usage/UsageCard.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/usage/UsageCard.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/utils/Format.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/utils/Format.mjs`

 * *Files 18% similar despite different names*

```diff
@@ -46,14 +46,19 @@
       }  
     }
   } else {
     return undefined;
   }
 };
 
+export const formatDataset = (name, samples, epochs) => {
+  const perEpochSamples = epochs > 0 ? samples / epochs : samples;
+  return `${name ? "— " : ""}${perEpochSamples + " "}${epochs > 1 ? `x ${epochs} ` : ""}${samples === 1 ? "sample" : "samples"}`;
+}
+
 export const userPromptForSample = (sample) => {
   if (sample) {
     if (typeof (sample.input) == "string") {
       return sample.input.trim();
     } else if (Array.isArray(sample.input)) {
       const userPrompt = sample.input.find(message => message.role == "user");
       if (userPrompt) {
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/EpochFilter.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/SampleFilter.mjs`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import { html } from "htm/preact";
 import { isNumeric } from "../utils/Type.mjs";
 
 import {
   kScoreTypeCategorical,
   kScoreTypeNumeric,
+  kScoreTypeObject,
   kScoreTypePassFail,
 } from "./SamplesDescriptor.mjs";
 
 export const SampleFilter = ({ descriptor, filter, filterChanged }) => {
   const filterCategory = (e) => {
     const val = e.currentTarget.value;
     if (val === "all") {
@@ -17,14 +18,16 @@
       });
     } else {
       filterChanged({
         value: val,
         filterFn: (sample, value) => {
           if (typeof sample.score.value === "string") {
             return sample.score.value.toLowerCase() === value?.toLowerCase();
+          } else if (typeof sample.score.value === "object") {
+            return JSON.stringify(sample.score.value) == value;
           } else {
             return sample.score.value === value;
           }
         },
       });
     }
   };
@@ -72,14 +75,33 @@
           value=${filter.value}
           placeholder="Filter Samples (score)"
           onInput=${filterInput}
         />
       `;
     }
 
+    case kScoreTypeObject: {
+      if (!descriptor.scoreDescriptor.categories) {
+        return  "";
+      }
+      const options = [{ text: "All", value: "all" }];
+      options.push(
+        ...descriptor.scoreDescriptor.categories.map((cat) => {
+          return { text: cat.text, value: cat.value};
+        })
+      );
+
+
+      
+      return html`<${SelectFilter}
+        options=${options}
+        filterFn=${filterCategory}
+      />`;
+    }
+
     default: {
       return undefined;
     }
   }
 };
 
 const SelectFilter = ({ options, filterFn }) => {
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/SamplesDescriptor.mjs`

 * *Files 2% similar despite different names*

```diff
@@ -112,16 +112,30 @@
         };
       }
     },
   },
   {
     describe: (values, types) => {
       if (types.length !== 0 && types[0] === "object") {
+
+        const buckets = values.map((val) => { return JSON.stringify(val); });
+        const vals = new Set(buckets);
+        let categories = undefined;
+        if (vals.size < 10) {
+          categories = Array.from(vals).map((val) => {
+            return {
+              val,
+              text: val
+            }
+          });
+        }
+
         return {
           scoreType: kScoreTypeObject,
+          categories,
           render: (score) => {
             if (score === null) {
               return "[null]";
             }
 
             const scores = [];
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/SortFilter.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/TaskErrorPanel.mjs`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/src/workspace/WorkSpace.mjs`

 * *Files 0% similar despite different names*

```diff
@@ -361,18 +361,14 @@
           iconEl.className = oldIconClz;
         }, 1250);
       }
     },
     [state]
   );
 
-  const selectTab = (event) => {
-    const id = event.currentTarget.id;
-    setSelectedTab(state, id);
-  };
 
   /**
    *
    * @param {import('../../log.d.ts').EvalLog} log
    */
   const showLog = (log) => {
     if (log.contents) {
@@ -439,22 +435,28 @@
         const tools = tab.tools(state);
         return tools;
       } else {
         return "";
       }
     });
 
+    const selectTab = (event) => {
+      const id = event.currentTarget.id;
+      setSelectedTab(state, id);
+    };
+    
   return html`<${WorkspaceDisplay}
     divRef=${divRef}
     tabs=${tabs}
     tabTools=${tabTools}
     state=${state}
     fullScreen=${props.fullScreen}
     offcanvas=${props.offcanvas}
     context=${context}
+    selectTab=${selectTab}
     afterBodyElements=${afterBodyElements}
   />`;
 };
 
 const WorkspaceDisplay = ({
   state,
   tabs,
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/_view/www/tools.js` & `inspect_ai-0.3.4/src/inspect_ai/_view/www/tools.js`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/dataset/__init__.py` & `inspect_ai-0.3.4/src/inspect_ai/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/dataset/_dataset.py` & `inspect_ai-0.3.4/src/inspect_ai/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/bias_detection.jsonl` & `inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/bias_detection.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/biology_qa.jsonl` & `inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/biology_qa.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/popularity.jsonl` & `inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/popularity.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/security_guide.jsonl` & `inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/security_guide.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl` & `inspect_ai-0.3.4/src/inspect_ai/dataset/_examples/theory_of_mind.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/csv.py` & `inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/csv.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/example.py` & `inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/example.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/file.py` & `inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/file.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/hf.py` & `inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/hf.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/dataset/_sources/json.py` & `inspect_ai-0.3.4/src/inspect_ai/dataset/_sources/json.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/dataset/_util.py` & `inspect_ai-0.3.4/src/inspect_ai/dataset/_util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/log/__init__.py` & `inspect_ai-0.3.4/src/inspect_ai/log/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/log/_file.py` & `inspect_ai-0.3.4/src/inspect_ai/log/_file.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import re
 from pathlib import Path
 from typing import Any, Callable, cast
 from urllib.parse import urlparse
 
 import json_stream  # type: ignore
 from pydantic import BaseModel, Field
+from pydantic_core import to_json
 
 from inspect_ai._util.file import FileInfo, file, filesystem
 
 from ._log import (
     EvalError,
     EvalLog,
     EvalPlan,
@@ -77,41 +78,49 @@
             for log in eval_logs
             if filter(read_eval_log(log.name, header_only=True))
         ]
     else:
         return eval_logs
 
 
-def write_eval_log(log: EvalLog, log_file: str) -> None:
+def write_eval_log(log: EvalLog, log_file: str | FileInfo) -> None:
     """Write an evaluation log.
 
     Args:
        log (EvalLog): Evaluation log to write.
-       log_file (str): Location to write log to.
+       log_file (str | FileInfo): Location to write log to.
 
     """
+    log_file = log_file if isinstance(log_file, str) else log_file.name
     with file(log_file, "w") as f:
         f.write(eval_log_json(log))
 
 
 def eval_log_json(log: EvalLog) -> str:
-    return log.model_dump_json(exclude_none=True, exclude_defaults=False, indent=2)
+    # serialize to json (ignore values that are unserializable)
+    # these values often result from solvers using metadata to
+    # pass around 'live' objects -- this is fine to do and we
+    # don't want to prevent it at the serialization level
+    return to_json(
+        value=log, indent=2, exclude_none=True, fallback=lambda _x: None
+    ).decode()
 
 
-def read_eval_log(log_file: str, header_only: bool = False) -> EvalLog:
+def read_eval_log(log_file: str | FileInfo, header_only: bool = False) -> EvalLog:
     """Read an evaluation log.
 
     Args:
-       log_file (str): Log file to read.
+       log_file (str | FileInfo): Log file to read.
        header_only (bool): Read only the header (i.e. exclude
          the "samples" and "logging" fields). Defaults to False.
 
     Returns:
        EvalLog object read from file.
     """
+    log_file = log_file if isinstance(log_file, str) else log_file.name
     with file(log_file, "r") as f:
         # header-only uses json-stream
         if header_only:
             data = json_stream.load(f, persistent=True)
 
             def read_field(field: str) -> Any:
                 if field in data.keys():
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/log/_log.py` & `inspect_ai-0.3.4/src/inspect_ai/log/_log.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/__init__.py` & `inspect_ai-0.3.4/src/inspect_ai/model/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_model.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_model.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_providers/anthropic.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_providers/azureai.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_providers/azureai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_providers/bedrock.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_providers/bedrock.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_providers/cloudflare.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_providers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_providers/google.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_providers/google.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_providers/hf.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_providers/hf.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_providers/mistral.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_providers/mistral.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_providers/openai.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_providers/openai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_providers/providers.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_providers/providers.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_providers/together.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_providers/together.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_providers/util.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_providers/util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_registry.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_tool.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_tool.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/model/_util.py` & `inspect_ai-0.3.4/src/inspect_ai/model/_util.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/scorer/__init__.py` & `inspect_ai-0.3.4/src/inspect_ai/scorer/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/scorer/_answer.py` & `inspect_ai-0.3.4/src/inspect_ai/scorer/_answer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/scorer/_common.py` & `inspect_ai-0.3.4/src/inspect_ai/scorer/_common.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/scorer/_match.py` & `inspect_ai-0.3.4/src/inspect_ai/scorer/_match.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/scorer/_metric.py` & `inspect_ai-0.3.4/src/inspect_ai/scorer/_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,16 +154,15 @@
     Args:
         scores (list[dict]): List of scores.
 
     Returns:
         Metric value
     """
 
-    def __call__(self, scores: list[Score]) -> int | float:
-        ...
+    def __call__(self, scores: list[Score]) -> int | float: ...
 
 
 MetricType = TypeVar("MetricType", Callable[..., Metric], type[Metric])
 r"""Metric type.
 Valid metric types include:
  - Functions that return a Metric
  - Classes derivied from Metric
@@ -178,15 +177,15 @@
             Function that returns a Metric or class
             deriving fromMetric
         name (str): Name of metric (Optional, defaults to object name)
 
     Returns:
         Metric type with registry attributes.
     """
-    metric_name = (name if name else getattr(metric, "__name__")).lower()
+    metric_name = name if name else getattr(metric, "__name__")
     registry_add(metric, RegistryInfo(type="metric", name=metric_name))
     return metric
 
 
 def metric_create(name: str, **kwargs: Any) -> Metric:
     r"""Create a Metric based on its registered name.
 
@@ -200,27 +199,24 @@
     Returns:
         Metric with registry info attribute
     """
     return cast(Metric, registry_create("metric", name, **kwargs))
 
 
 @overload
-def metric(name: str) -> Callable[..., MetricType]:
-    ...
+def metric(name: str) -> Callable[..., MetricType]: ...
 
 
 @overload
 # type: ignore
-def metric(name: Callable[..., Metric]) -> Callable[..., Metric]:
-    ...
+def metric(name: Callable[..., Metric]) -> Callable[..., Metric]: ...
 
 
 @overload
-def metric(name: type[Metric]) -> type[Metric]:
-    ...
+def metric(name: type[Metric]) -> type[Metric]: ...
 
 
 def metric(name: str | MetricType) -> Callable[..., MetricType] | MetricType:
     r"""Decorator for registering metrics.
 
     Args:
         name: (str | MetricType):
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/accuracy.py` & `inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/mean.py` & `inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/mean.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/scorer/_metrics/std.py` & `inspect_ai-0.3.4/src/inspect_ai/scorer/_metrics/std.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/scorer/_model.py` & `inspect_ai-0.3.4/src/inspect_ai/scorer/_model.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/scorer/_pattern.py` & `inspect_ai-0.3.4/src/inspect_ai/scorer/_pattern.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/scorer/_scorer.py` & `inspect_ai-0.3.4/src/inspect_ai/scorer/_scorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,18 @@
     `text` property to access the value as a single string.
     """
 
     def __init__(self, target: str | list[str]) -> None:
         self.target = target if isinstance(target, list) else [target]
 
     @overload
-    def __getitem__(self, index: int) -> str:
-        ...
+    def __getitem__(self, index: int) -> str: ...
 
     @overload
-    def __getitem__(self, index: slice) -> Sequence[str]:
-        ...
+    def __getitem__(self, index: slice) -> Sequence[str]: ...
 
     def __getitem__(self, index: Union[int, slice]) -> Union[str, Sequence[str]]:
         return self.target[index]
 
     def __len__(self) -> int:
         return len(self.target)
 
@@ -60,16 +58,15 @@
     dictionary with scoring outcomes and context.
 
     Args:
         state (TaskState): Task state
         target (Target): Ideal target for the output.
     """
 
-    async def __call__(self, state: TaskState, target: Target) -> Score:
-        ...
+    async def __call__(self, state: TaskState, target: Target) -> Score: ...
 
 
 ScorerType = TypeVar("ScorerType", Callable[..., Scorer], type[Scorer])
 r"""Scorer type.
 
 Valid scorer types include:
  - Functions that return a Scorer
@@ -85,15 +82,15 @@
             Scorer, function that returns a Scorer, or class
             deriving from the Scorer protocol.
         name (str): Name of scorer (Optional, defaults to object name)
 
     Returns:
         Scorer with registry attributes.
     """
-    scorer_name = (name if name else getattr(scorer, "__name__")).lower()
+    scorer_name = name if name else getattr(scorer, "__name__")
     registry_add(scorer, RegistryInfo(type="scorer", name=scorer_name))
     return scorer
 
 
 def scorer_create(name: str, **kwargs: Any) -> Scorer:
     r"""Create a Scorer based on its registered name.
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/solver/__init__.py` & `inspect_ai-0.3.4/src/inspect_ai/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/solver/_critique.py` & `inspect_ai-0.3.4/src/inspect_ai/solver/_critique.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/solver/_multiple_choice.py` & `inspect_ai-0.3.4/src/inspect_ai/solver/_multiple_choice.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/solver/_plan.py` & `inspect_ai-0.3.4/src/inspect_ai/solver/_plan.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/solver/_prompt.py` & `inspect_ai-0.3.4/src/inspect_ai/solver/_prompt.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/solver/_solver.py` & `inspect_ai-0.3.4/src/inspect_ai/solver/_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,16 +129,15 @@
 
     Returns:
        Updated TaskState.
     """
 
     async def __call__(
         self, state: TaskState, **kwargs: Unpack[GenerateConfigArgs]
-    ) -> TaskState:
-        ...
+    ) -> TaskState: ...
 
 
 @runtime_checkable
 class Solver(Protocol):
     r"""Contribute to solving an evaluation task.
 
     Contribute to the solution of a task by transforming a TaskState
@@ -156,16 +155,15 @@
         Updated TaskState.
     """
 
     async def __call__(
         self,
         state: TaskState,
         generate: Generate,
-    ) -> TaskState:
-        ...
+    ) -> TaskState: ...
 
 
 SolverType = TypeVar("SolverType", Callable[..., Solver], type[Solver])
 r"""Solver type.
 
 Valid solver types include:
  - Functions that return a Solver
@@ -180,15 +178,15 @@
         solver (SolverType):
             Function that returns a Solver or class derived Solver.
         name (str): Name of solver (Optional, defaults to object name)
 
     Returns:
         Solver with registry attributes.
     """
-    solver_name = (name if name else getattr(solver, "__name__")).lower()
+    solver_name = name if name else getattr(solver, "__name__")
     registry_add(solver, RegistryInfo(type="solver", name=solver_name))
     return solver
 
 
 def solver_create(name: str, **kwargs: Any) -> Solver:
     r"""Create a Solver based on its registered name.
 
@@ -199,27 +197,24 @@
     Returns:
         Solver with registry info attribute
     """
     return cast(Solver, registry_create("solver", name, **kwargs))
 
 
 @overload
-def solver(name: str) -> Callable[..., SolverType]:
-    ...
+def solver(name: str) -> Callable[..., SolverType]: ...
 
 
 @overload
 # type: ignore
-def solver(name: Callable[..., Solver]) -> Callable[..., Solver]:
-    ...
+def solver(name: Callable[..., Solver]) -> Callable[..., Solver]: ...
 
 
 @overload
-def solver(name: type[Solver]) -> type[Solver]:
-    ...
+def solver(name: type[Solver]) -> type[Solver]: ...
 
 
 def solver(name: str | SolverType) -> Callable[..., SolverType] | SolverType:
     r"""Decorator for registering solvers.
 
     Args:
         name: (str | SolverType):
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai/solver/_tool/tool.py` & `inspect_ai-0.3.4/src/inspect_ai/solver/_tool/tool.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/solver/_tool/tool_def.py` & `inspect_ai-0.3.4/src/inspect_ai/solver/_tool/tool_def.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/solver/_tool/use_tools.py` & `inspect_ai-0.3.4/src/inspect_ai/solver/_tool/use_tools.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/solver/_tool/web_search.py` & `inspect_ai-0.3.4/src/inspect_ai/solver/_tool/web_search.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/util/_context/concurrency.py` & `inspect_ai-0.3.4/src/inspect_ai/util/_context/concurrency.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/util/_context/logger.py` & `inspect_ai-0.3.4/src/inspect_ai/util/_context/logger.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/util/_context/resource.py` & `inspect_ai-0.3.4/src/inspect_ai/util/_context/resource.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai/util/_context/subprocess.py` & `inspect_ai-0.3.4/src/inspect_ai/util/_context/subprocess.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/src/inspect_ai.egg-info/PKG-INFO` & `inspect_ai-0.3.4/src/inspect_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspect_ai
-Version: 0.3.3
+Version: 0.3.4
 Summary: Framework for large language model evaluations
 Author: UK AI Safety Institute
 License: MIT License
 Project-URL: Documentation, https://UKGovernmentBEIS.github.io/inspect_ai/
 Project-URL: Source Code, https://github.com/UKGovernmentBEIS/inspect_ai
 Project-URL: Issue Tracker, https://github.com/UKGovernmentBEIS/inspect_ai/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai.egg-info/SOURCES.txt` & `inspect_ai-0.3.4/src/inspect_ai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 docs/images/inspect-view-logging-console.png
 docs/images/inspect-view-logging.png
 docs/images/inspect-view-main.png
 docs/images/inspect-view-messages.png
 docs/images/inspect-view-metadata.png
 docs/images/inspect-view-scoring.png
 docs/images/inspect-view-sort.png
+docs/images/inspect-view-splash.png
 docs/images/popularity.png
 docs/images/rate-limit.png
 docs/images/running-theory.png
 examples/biology_qa.py
 examples/popularity.py
 examples/security_guide.py
 examples/theory_of_mind.py
@@ -135,16 +136,14 @@
 src/inspect_ai/_view/www/.gitignore
 src/inspect_ai/_view/www/App.mjs
 src/inspect_ai/_view/www/api.mjs
 src/inspect_ai/_view/www/favicon.svg
 src/inspect_ai/_view/www/index.html
 src/inspect_ai/_view/www/log-schema.json
 src/inspect_ai/_view/www/log.d.ts
-src/inspect_ai/_view/www/package-lock.json
-src/inspect_ai/_view/www/package.json
 src/inspect_ai/_view/www/tools.js
 src/inspect_ai/_view/www/libs/clipboard.min.js
 src/inspect_ai/_view/www/libs/json5.min.js
 src/inspect_ai/_view/www/libs/purify.min.js
 src/inspect_ai/_view/www/libs/showdown.min.js
 src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap-icons.min.css
 src/inspect_ai/_view/www/libs/bootstrap/css/bootstrap.min.css
@@ -164,14 +163,15 @@
 src/inspect_ai/_view/www/src/Constants.mjs
 src/inspect_ai/_view/www/src/Register.mjs
 src/inspect_ai/_view/www/src/components/AnsiDisplay.css
 src/inspect_ai/_view/www/src/components/AnsiDisplay.mjs
 src/inspect_ai/_view/www/src/components/AppErrorBoundary.mjs
 src/inspect_ai/_view/www/src/components/Card.mjs
 src/inspect_ai/_view/www/src/components/ChatView.mjs
+src/inspect_ai/_view/www/src/components/CopyButton.mjs
 src/inspect_ai/_view/www/src/components/Dialog.mjs
 src/inspect_ai/_view/www/src/components/EmptyPanel.mjs
 src/inspect_ai/_view/www/src/components/ErrorPanel.mjs
 src/inspect_ai/_view/www/src/components/LabeledValue.mjs
 src/inspect_ai/_view/www/src/components/LoadingScreen.mjs
 src/inspect_ai/_view/www/src/components/MarkdownDiv.mjs
 src/inspect_ai/_view/www/src/components/MessageContent.mjs
@@ -263,14 +263,15 @@
 src/inspect_ai/util/_context/logger.py
 src/inspect_ai/util/_context/resource.py
 src/inspect_ai/util/_context/subprocess.py
 tests/test_anthropic.py
 tests/test_cloudlfare.py
 tests/test_collapse_user_message.py
 tests/test_dataset.py
+tests/test_eval_log.py
 tests/test_examples.py
 tests/test_images.py
 tests/test_list_task.py
 tests/test_logprobs.py
 tests/test_metric.py
 tests/test_num_choices.py
 tests/test_openai.py
```

### Comparing `inspect_ai-0.3.3/src/inspect_ai.egg-info/requires.txt` & `inspect_ai-0.3.4/src/inspect_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_anthropic.py` & `inspect_ai-0.3.4/tests/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_collapse_user_message.py` & `inspect_ai-0.3.4/tests/test_collapse_user_message.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_dataset.py` & `inspect_ai-0.3.4/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_images/images.jsonl` & `inspect_ai-0.3.4/tests/test_images/images.jsonl`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_images.py` & `inspect_ai-0.3.4/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_list_task.py` & `inspect_ai-0.3.4/tests/test_list_task.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_logprobs.py` & `inspect_ai-0.3.4/tests/test_logprobs.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_metric.py` & `inspect_ai-0.3.4/tests/test_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,29 +47,29 @@
     def __call__(self, scores: list[Score]) -> int | float:
         return 1
 
 
 def test_metric_registry() -> None:
     registry_assert(accuracy1, "accuracy1")
     registry_assert(acc_fn, "accuracy2")
-    registry_assert(Accuracy3, "accuracy3")
+    registry_assert(Accuracy3, "Accuracy3")
     registry_assert(AccuracyNamedCls, "accuracy4")
 
 
 def test_metric_call() -> None:
     registry_assert(accuracy1(), "accuracy1")
     registry_assert(acc_fn(), "accuracy2")
-    registry_assert(Accuracy3(), "accuracy3")
+    registry_assert(Accuracy3(), "Accuracy3")
     registry_assert(AccuracyNamedCls(), "accuracy4")
 
 
 def test_metric_create() -> None:
     metric_create_assert("accuracy1", correct="C")
     metric_create_assert("accuracy1", correct="C")
-    metric_create_assert("accuracy3", correct="C")
+    metric_create_assert("Accuracy3", correct="C")
     metric_create_assert("accuracy4", correct="C")
 
 
 def test_inspect_metrics() -> None:
     registry_assert(accuracy, f"{PKG_NAME}/accuracy")
     registry_assert(accuracy(), f"{PKG_NAME}/accuracy")
 
@@ -80,15 +80,15 @@
     def check_log(log):
         assert log.results and (
             list(log.results.metrics.keys())
             == [
                 "accuracy",
                 "bootstrap_std",
                 "accuracy1",
-                "accuracy3",
+                "Accuracy3",
             ]
         )
 
     task = Task(
         dataset=[Sample(input="What is 1 + 1?", target=["2", "2.0", "Two"])],
         scorer=match(),
         metrics=[accuracy(), accuracy1(), Accuracy3()],
```

### Comparing `inspect_ai-0.3.3/tests/test_num_choices.py` & `inspect_ai-0.3.4/tests/test_num_choices.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_openai.py` & `inspect_ai-0.3.4/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_plan.py` & `inspect_ai-0.3.4/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_registry.py` & `inspect_ai-0.3.4/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_retry.py` & `inspect_ai-0.3.4/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_scorer.py` & `inspect_ai-0.3.4/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_solver.py` & `inspect_ai-0.3.4/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_stop_reason.py` & `inspect_ai-0.3.4/tests/test_stop_reason.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_subprocess.py` & `inspect_ai-0.3.4/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/test_tools.py` & `inspect_ai-0.3.4/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `inspect_ai-0.3.3/tests/utils.py` & `inspect_ai-0.3.4/tests/utils.py`

 * *Files identical despite different names*

