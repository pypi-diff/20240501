# Comparing `tmp/pyodide_mkdocs_theme-0.6.1.tar.gz` & `tmp/pyodide_mkdocs_theme-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-0.6.1.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-0.7.0.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-0.6.1.tar` & `pyodide_mkdocs_theme-0.7.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.6.1/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.6.1/README.md
--rw-r--r--   0        0        0     1347 2024-04-29 14:09:17.377380 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     2244 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-04-29 14:09:17.421381 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0     1178 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
--rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     4996 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
--rw-r--r--   0        0        0    22407 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
--rw-r--r--   0        0        0    16081 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
--rw-r--r--   0        0        0      689 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6043 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0     3861 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11723 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0    13163 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/messages.py
--rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4485 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0    12267 2024-04-27 23:06:40.767927 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11736 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0     6420 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
--rw-r--r--   0        0        0     1603 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0    10204 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
--rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     8198 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0      374 2024-04-28 09:15:25.683143 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     6909 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/__init__.py
--rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/custom_lang.py
--rw-r--r--   0        0        0     3979 2024-04-29 14:09:17.373380 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/custom_lang_src.py
--rw-r--r--   0        0        0     5565 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     5387 2024-04-29 14:05:12.654065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0     7420 2024-04-29 14:05:12.654065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1702 2024-04-29 14:05:12.654065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4320 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
--rw-r--r--   0        0        0     4361 2024-04-29 14:05:12.654065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
--rw-r--r--   0        0        0     6642 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     1924 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     9831 2024-04-29 14:05:12.658065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
--rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
--rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
--rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
--rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
--rw-r--r--   0        0        0     6753 2024-04-29 14:05:12.658065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
--rw-r--r--   0        0        0    16617 2024-04-29 14:05:12.658065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
--rw-r--r--   0        0        0    11246 2024-04-29 14:05:12.658065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
--rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
--rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
--rw-r--r--   0        0        0     9195 2024-04-29 14:05:12.658065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
--rw-r--r--   0        0        0     3740 2024-04-26 21:34:38.171571 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
--rw-r--r--   0        0        0     1651 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
--rw-r--r--   0        0        0     5379 2024-04-26 21:34:38.171571 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
--rw-r--r--   0        0        0     4201 2024-04-29 14:05:12.658065 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
--rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
--rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
--rw-r--r--   0        0        0     3774 2024-04-14 12:10:19.820826 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
--rw-r--r--   0        0        0    12716 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
--rw-r--r--   0        0        0     1761 2024-04-29 14:09:14.657299 pyodide_mkdocs_theme-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.7.0/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.7.0/README.md
+-rw-r--r--   0        0        0     1347 2024-05-01 19:58:31.756073 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     2244 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-05-01 19:58:31.792074 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
+-rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     4979 2024-05-01 19:57:26.306151 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
+-rw-r--r--   0        0        0    24750 2024-05-01 19:57:26.306151 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
+-rw-r--r--   0        0        0    15749 2024-05-01 19:57:26.306151 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
+-rw-r--r--   0        0        0      689 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6043 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0     3861 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11723 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0    13163 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     7120 2024-05-01 19:57:26.306151 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0     4483 2024-05-01 19:57:26.310151 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4485 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0    13652 2024-05-01 19:57:26.310151 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11739 2024-05-01 19:57:26.310151 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0     6663 2024-05-01 19:57:26.310151 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
+-rw-r--r--   0        0        0     1603 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0    10204 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
+-rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     8198 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0      374 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     6933 2024-05-01 19:57:26.310151 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/scripts/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/scripts/custom_lang.py
+-rw-r--r--   0        0        0     3979 2024-05-01 19:58:31.756073 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/scripts/custom_lang_src.py
+-rw-r--r--   0        0        0     5565 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     5496 2024-05-01 19:57:26.310151 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0     7420 2024-05-01 08:58:57.928287 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1702 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4435 2024-05-01 19:57:26.310151 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
+-rw-r--r--   0        0        0     4361 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
+-rw-r--r--   0        0        0     6642 2024-04-26 21:34:38.167571 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     1924 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     9885 2024-05-01 19:57:26.310151 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
+-rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
+-rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
+-rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
+-rw-r--r--   0        0        0     7613 2024-05-01 19:57:26.310151 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
+-rw-r--r--   0        0        0    16617 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
+-rw-r--r--   0        0        0    11246 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
+-rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
+-rw-r--r--   0        0        0     9195 2024-04-29 14:09:33.377858 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
+-rw-r--r--   0        0        0     3740 2024-04-26 21:34:38.171571 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
+-rw-r--r--   0        0        0     1651 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
+-rw-r--r--   0        0        0     5379 2024-04-26 21:34:38.171571 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
+-rw-r--r--   0        0        0     4201 2024-04-29 14:09:33.377858 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
+-rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
+-rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
+-rw-r--r--   0        0        0     3774 2024-04-14 12:10:19.820826 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
+-rw-r--r--   0        0        0    12716 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
+-rw-r--r--   0        0        0     1761 2024-05-01 19:58:27.991963 pyodide_mkdocs_theme-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.7.0/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-0.6.1/LICENSE` & `pyodide_mkdocs_theme-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/README.md` & `pyodide_mkdocs_theme-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/deprecation.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     Insert the given section from the python file.
     Note: To use only on python scripts holding all the sections for the IDE macros. For regular
           files, use the `py` macro or regular code fences with file inclusions (for performances
           reasons).
     """
     @wraps(section)
     def _section(py_name:str, section_name:ScriptSection, ID:Optional[int]=None):
-        file_data = IdeFilesExtractor(env, py_name, ID, skip_check=True)
+        file_data = IdeFilesExtractor(env, py_name, ID)
         content = file_data.get_section(section_name)
 
         id_pattern = "" if ID is None else rf",\s*ID\s*=\s*{ ID }\b\s*"
         macro_pattern = rf"""['"]{ py_name }['"]\s*,\s*['"]{ section_name }['"]{ id_pattern }"""
         ide_jinja_reg = re.compile( rf"section\(\s*{ macro_pattern }" )
         indent = env.get_indent_in_current_page(ide_jinja_reg)
         out = build_code_fence(content, indent, lang='python')
```

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 from math import inf
 
 from mkdocs.exceptions import BuildError
 
 from pyodide_mkdocs_theme.pyodide_macros.messages import Tip
 
 from ... import html_builder as Html
+from ...pyodide_logger import logger
 from ...tools_and_constants import HtmlClass, Prefix, ScriptKind
 from ...pages_and_ides_configs import IdeConfigKey
-from ...parsing import build_code_fence
+from ...parsing import build_code_fence, items_comma_joiner
 from ...paths_utils import convert_url_to_utf8, to_uri
 from ...plugin.maestro_IDE import MaestroIDE
 
 from .ide_files_data import IdeFilesExtractor
 
 
 
@@ -160,14 +161,18 @@
     @property               # pylint: disable-next=all
     def has_secrets(self):  return self.files_data.has_secrets
     @property               # pylint: disable-next=all
     def has_rem(self):      return self.files_data.has_rem
     @property               # pylint: disable-next=all
     def has_vis_rem(self):  return self.files_data.has_vis_rem
 
+    @property               # pylint: disable-next=all
+    def has_any_corr_rem(self):
+        return self.has_corr or self.has_rem or self.has_vis_rem
+
 
 
     def __post_init__(self):
 
         to_globals_if_none = (
             ('max_attempts', 'max_attempts_before_corr_available'),
             ('max_size',     'default_ide_height_lines'),
@@ -175,61 +180,62 @@
         for prop,conf_prop in to_globals_if_none:
             if getattr(self, prop) is None:
                 def_val = getattr(self.my_env, conf_prop)
                 setattr(self, prop, def_val)
 
         self.files_data = IdeFilesExtractor(self.my_env, self.py_name, self.id)
 
+        # Extract max number of attempts from file or macro argument, clean up the file if needed,
+        # then pick the correct number of attempts and set it in the global structure.
+        # Also defines self.ide_content.
+        max_attempts = self._define_max_attempts_symbols_and_value()
+
+        self._validate_config(max_attempts)
+
+
         if 0 <= self.rec_limit < self.my_env.MIN_RECURSION_LIMIT:
-            with_id = f' (ID={ self.id })' if self.id is not None else ''
             raise BuildError(
-                f"The recursion limit for {self.my_env.page.file.src_uri}:{self.py_name}"
-                f"{with_id} is set too low and may causes runtime troubles. Please set it to "
-                f"at least { self.my_env.MIN_RECURSION_LIMIT }."
+                f"The recursion limit for {self} is set too low and may causes runtime troubles. "
+                f"Please set it to at least { self.my_env.MIN_RECURSION_LIMIT }."
             )
 
         if self.id is not None and not isinstance(self.id, int):
-            raise BuildError(f'The ID argument should be an integer, but was: {self.id!r}')
+            raise BuildError(f'The ID argument should be an integer, for {self}')
 
 
         # Extract python content and compute editor name:
         exo_py: Optional[Path] = self.files_data.exo_py
         id_ide: str = self._generate_id_ide(exo_py)
         self.editor_name = f"{ Prefix.editor_ }{ id_ide }"
 
 
-        # Extract max number of attempts from file or macro argument, clean up the file if needed,
-        # then pick the correct number of attempts and set it in the global structure.
-        # Also defines self.ide_content.
-        max_attempts = self._define_max_attempts_symbols_and_value()
-
-
         # Compute all code exclusions and white list of imports:
         white_list = self._compute_exclusions_and_white_list("white_list")
         excluded = self._compute_exclusions_and_white_list("excluded")
-        excluded_methods = [ meth for meth in excluded if meth.startswith('.') ]
-        excluded = [ no_meth for no_meth in excluded if not no_meth.startswith('.') ]
+        excluded_methods = [ meth for meth in excluded if     meth.startswith('.') ]
+        excluded =         [ meth for meth in excluded if not meth.startswith('.') ]
 
 
         # Search the indentation level for the current IDE:
         is_v = self.mode.strip('_')
         quotes = """['"]"""
         script_pattern = "" if not self.py_name else f"{quotes}{ self.py_name }{quotes}"
         id_pattern = r'(?!.*?ID\s*=)' if self.id is None else rf".*?ID\s*=\s*{ self.id }\b"
 
         ide_jinja_reg = re.compile( rf"IDE{ is_v }\(\s*{ script_pattern }{ id_pattern }" )
         self.indentation = self.my_env.get_indent_in_current_page(ide_jinja_reg)
 
 
 
         to_register: List[Tuple[IdeConfigKey,Any]] = [
-            ('hdr_content',         self.files_data.hdr),
+            ('env_content',         self.files_data.env_content),
             ('user_content',        self.files_data.user_content),
             ('public_tests',        self.files_data.public_tests),
             ('secret_tests',        self.files_data.secret_tests),
+            ('post_content',        self.files_data.post_content),
             ('corr_rem_config',     self.files_data.corr_rem_bit_mask),
             ('attempts_left',       max_attempts),
             ("excluded",            excluded),
             ("excluded_methods",    excluded_methods),
             ("white_list",          white_list),
             ("auto_log_assert",     self.auto_log_assert),
             ("rec_limit",           self.rec_limit),
@@ -238,14 +244,93 @@
             self.my_env.set_current_page_js_data(self.editor_name, field, value)
 
 
 
     #-----------------------------------------------------------------------------
 
 
+    def __str__(self):
+        with_id = '' if self.id is None else f', ID={self.id}'
+        return f"IDE('{self.py_name}'{with_id}), in file {self.my_env.page.file.src_uri}"
+
+
+    def _define_max_attempts_symbols_and_value(self):
+        """
+        Any MAX value defined in the file takes precedence, because it's not possible to know
+        if the value coming from the macro is the default one or not.
+        """
+        max_ide = str(self.max_attempts)        # from macro call
+
+        # If something about MAX in the file, it has precedence (if exists -> legacy...)
+        max_from_file = self.files_data.file_max_attempts
+        if max_from_file != "":
+            max_ide = max_from_file
+
+        is_inf = max_ide in ("+", "1000")     # 1000: legacy...
+
+        # If ever there are neither correction nor remark, or if no tests, use also inf:
+        is_inf = is_inf or not self.has_any_corr_rem or not self.has_secrets
+
+        self.max_attempts_symbol = self.INFINITY_SYMBOL if is_inf else str(max_ide)
+
+        max_attempts = inf if is_inf else int(max_ide)
+        return max_attempts
+
+
+
+    def _validate_config(self, max_attempts: Union[int,float]):
+        msg: Optional[Tuple[str,str]] = None
+
+        if (self.my_env.forbid_secrets_without_corr_or_REMs
+            and self.has_secrets and not self.has_any_corr_rem
+        ):
+            msg = (
+                "A `secrets` section exist but there are no `corr` section, REM or VIS_REM file.",
+                "forbid_secrets_without_corr_or_REMs"
+            )
+
+        elements = [*filter(bool,(
+            "a correction"   * (not self.has_corr),
+            "a REM file"     * (not self.has_rem),
+            "a VIS_REM file" * (not self.has_vis_rem),
+        ))]
+        elt_msg = items_comma_joiner(elements, 'and')
+        single  = len(elements)==1
+        elt_msg = f"{ elt_msg } exist{ 's' * (single)}".capitalize()
+
+        if (self.my_env.forbid_hidden_corr_and_REMs_without_secrets
+            and self.has_any_corr_rem and not self.has_secrets
+        ):
+            msg = (
+                f"{ elt_msg }, but there is no `secrets` section.",
+                'forbid_hidden_corr_and_REMs_without_secrets'
+            )
+
+        if (self.my_env.forbid_corr_and_REMs_with_infinite_attempts
+            and max_attempts==inf and self.has_any_corr_rem
+        ):
+            subject = "it" if single else "they"
+            msg = (
+                f"{ elt_msg }, but {subject} will never be visible because the number of "
+                "attempts is set to infinity.",
+                'forbid_corr_and_REMs_with_infinite_attempts'
+            )
+
+        if msg:
+            msg, opt = msg
+            msg = (
+                f"Invalid configuration\n    {self}:\n    {msg}\n    You can deactivate this "
+                f"check by setting plugins.pyodide_macros.build.{opt} to false in `mkdocs.yml`."
+            )
+            if self.my_env._dev_mode:       # pylint: disable=protected-access
+                logger.error("DEV_MODE (expected x2) - " + msg)
+            else:
+                raise BuildError(msg)
+
+
 
     def _compute_exclusions_and_white_list(self, prop:str):
         """
         Convert a string argument (exclusions or white list) tot he equivalent list of data.
         """
         rule = (getattr(self, prop) or "").strip(' ;,')       # (never allow None)
         lst = re.split(r'[ ;,]+', rule) if rule else []
@@ -284,46 +369,21 @@
 
         id_ide = hashlib.sha1(path.encode("utf-8")).hexdigest()
 
         if not self.my_env.register_if_unique(id_ide):
             raise BuildError(
                 "The same editor ID got generated twice. If you are trying to use the same set"
                 "of files for different IDEs, use the ID argument to disambiguate their id.\n"
-               f"  Problematic file:  { py_path }\n"
-               f"  Possible solution: { '{{' } IDE(\"{ self.py_name }\", ID=2) { '}}' }"
+               f"  Problematic call:  { self }\n"
+               f"  Possible solution: add the ID:int keyword argument or change its value"
             )
         return id_ide
 
 
 
-    def _define_max_attempts_symbols_and_value(self):
-        """
-        Any MAX value defined in the file takes precedence, because it's not possible to know
-        if the value coming from the macro is the default one or not.
-        """
-        max_ide = str(self.max_attempts)        # from macro call
-
-        # If something about MAX in the file, it has precedence (if exists -> legacy...)
-        max_from_file = self.files_data.file_max_attempts
-        if max_from_file != "":
-            max_ide = max_from_file
-
-        is_inf = max_ide in ("+", "1000")     # 1000: legacy...
-
-        # If ever there are neither correction nor remark, or if no tests, use also inf:
-        is_inf = is_inf or not (self.has_corr or self.has_rem) or not self.has_secrets
-
-        self.max_attempts_symbol = self.INFINITY_SYMBOL if is_inf else str(max_ide)
-
-        max_attempts = inf if is_inf else int(max_ide)
-        return max_attempts
-
-
-
-
 
     #-----------------------------------------------------------------------------
 
 
 
 
     def make_ide(self) -> str:
```

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,49 +105,57 @@
 
 
     corr_rem_bit_mask: int = 0
     """ Bit mask giving the configuration for correction and/or remark data
         mask&1 represent the presence of correction, mask&2 is for REM.
     """
 
-    hdr: str = ""
-    """ Python header code content """
+    env_content: str = ""
+    """ Python header code content (run async) """
 
     user_content:str = ""
     """ Python user code (only) """
 
     corr_content: str = ""
     """ Python solution code """
 
     public_tests: str = ""
     """ Public tests (only) """
 
     secret_tests:str = ""
     """ Code for the private tests """
 
+    post_content: str = ""
+    """ Code for post executions (teardown / run async).
+        Always run, even in case of failures in users or tests code, but NOT if an error
+        occurred in the ENV section.
+    """
+
+
 
     #------------------------------------------------------------
 
-    skip_check: bool = False
-    """
-    If True, the sanity check about the presence of secret tests vs corr&REM, and the
-    python code checks will be skipped.
-    """
+    # skip_check: bool = False
+    # """
+    # If True, the sanity check about the presence of secret tests vs corr&REM, and the
+    # python code checks will be skipped.
+    # """
 
 
     SECTION_TOKEN: ClassVar[re.Pattern] = re.compile(
         r'^(# *-+ *PYODIDE *: *\w+ *-+ *#)$', flags=re.MULTILINE
     )
 
     SECTION_TO_PROP: ClassVar[Dict[str,str]] = {
-        ScriptSection.hdr:     "hdr",
+        ScriptSection.env:     "env_content",
         ScriptSection.user:    "user_content",
         ScriptSection.corr:    "corr_content",
         ScriptSection.tests:   "public_tests",
         ScriptSection.secrets: "secret_tests",
+        ScriptSection.post:    "post_content",
     }
 
 
     @property
     def has_corr(self):
         return bool(self.corr_content)
     @property
@@ -176,37 +184,18 @@
 
         # Extract everything:
         if self.SECTION_TOKEN.search(script_content):
             self.extract_multi_sections(script_content)
         else:
             self.extract_multi_files(script_content)
 
-
         self.corr_rem_bit_mask = self.has_corr + self.has_rem * 2
 
-        # Sanity check:
-        has_hidden_stuff = self.has_corr or self.has_rem or self.has_vis_rem
-        if not self.skip_check and not self.has_secrets and has_hidden_stuff:
-            opn,clos = '{{','}}'
-            maybe_id = "" if self.id is None else f", ID={ self.id }"
-            location = self.env.page.file.src_uri
-            test_file = self.py_name + SiblingFile.test
-            msg = (
-                f'An invalid configuration of files has been found for {opn} IDE("'
-                f'{self.py_name}"{ maybe_id }, ...) {clos} in the page { location }: '
-                f'a correction or remark file exists but there is no { test_file } file.'
-            )
-            if self.env._dev_mode:
-                logger.error('EXPECTED (1x) - ' + msg)
-            else:
-                raise BuildError(msg)
-
-
-        if not self.skip_check and self.env.check_python_files:
-            self.check_python()
+        # if not self.skip_check and self.env.check_python_files:
+        #     self.check_python()
 
         # self._fuuuuuusion()
         # self._cleanup_tests()
 
 
 
     def get_path_and_existence(self, tail:str):
@@ -321,15 +310,15 @@
             script = script_content
             first_line, script = script.split("\n", 1) if "\n" in script else (script,'')
 
             script_content = script.strip()
             self.file_max_attempts = first_line.split("=")[1].strip()
 
         (
-            self.hdr, self.user_content, self.public_tests,
+            self.env_content, self.user_content, self.public_tests,
         ) = self.env.get_hdr_and_public_contents_from(script_content)
 
         (
             (self.test_rel_path, self.secret_tests),
             (self.corr_rel_path, self.corr_content),
             (self.rem_rel_path,  _),
             (self.vis_rem_rel_path,  _),
@@ -349,34 +338,35 @@
 
     def check_python(self):
         """
         * hdr + corr + public + secret => pass
         * hdr + user + public => doesn't pass
         * hdr + user + secret => doesn't pass
         """
+        raise ValueError("The build.check_python_files option has been disabled.")
         if not self.py_name: # or self.id is not None:
             # skip: nothing to check
             return
 
         src    = get_sibling_of_current_page(self.env, self.py_name, tail='.py')
         target = Path('___XXX_check_python.py')
         target.touch(exist_ok=True)
 
         to_check = [
             (
                 "Correction code should have passed", True, bool(self.corr_content and self.secret_tests),
-                [self.hdr, self.corr_content, self.public_tests, self.secret_tests],
+                [self.env_content, self.corr_content, self.public_tests, self.secret_tests],
             ),
             (
                 "Initial solution should fail public tests", False, True,
-                [self.hdr, self.user_content, self.public_tests],
+                [self.env_content, self.user_content, self.public_tests],
             ),
             (
                 "Initial solution should fail public + secret tests", False, bool(self.secret_tests),
-                [self.hdr, self.user_content, self.public_tests, self.secret_tests],
+                [self.env_content, self.user_content, self.public_tests, self.secret_tests],
             ),
         ]
         try:
             for msg, does_run, todo, sections in to_check:
 
                 if not todo: continue
 
@@ -414,53 +404,53 @@
 
     #--------------------------------------------------------------------------
     #        PYTHON FILES MANAGEMENT IN BATCHES (used on CodEx only)
     #--------------------------------------------------------------------------
 
 
 
-    def _fuuuuuusion(self):
-        src = get_sibling_of_current_page(self.env, self.py_name, tail=SiblingFile.exo)
-        if not src:
-            return
-        alter = 'fusion_tmp' / src.relative_to(self.env.docs_dir_path)
-        # print(alter)
-        self.__create_merged_file(alter)
-
-
-    def _cleanup_tests(self):
-        target_prop = 'corr_content'
-        content_to_cleanup:str = getattr(self, target_prop)
-        if self.public_tests and self.public_tests in content_to_cleanup:
-            cuts = [*map(str.strip, content_to_cleanup.split(self.public_tests))]
-            print(f"TESTS - {self.exo_py} : n_parts={ len(cuts) }") # | { cuts[0].strip() }")
-            assert len(cuts)==2
-
-            start,end = cuts
-            start = re.sub(r'(?i)# *tests?$', '', start, flags=re.MULTILINE).strip()
-            setattr(self, target_prop, start+"\n"+end)
-
-            src = get_sibling_of_current_page(self.env, self.py_name, tail=SiblingFile.exo)
-            alter = 'fusion_tmp' / src.relative_to(self.env.docs_dir_path)
-            self.__create_merged_file(alter)
-
+    # def _fuuuuuusion(self):
+    #     src = get_sibling_of_current_page(self.env, self.py_name, tail=SiblingFile.exo)
+    #     if not src:
+    #         return
+    #     alter = 'fusion_tmp' / src.relative_to(self.env.docs_dir_path)
+    #     # print(alter)
+    #     self.__create_merged_file(alter)
+
+
+    # def _cleanup_tests(self):
+    #     target_prop = 'corr_content'
+    #     content_to_cleanup:str = getattr(self, target_prop)
+    #     if self.public_tests and self.public_tests in content_to_cleanup:
+    #         cuts = [*map(str.strip, content_to_cleanup.split(self.public_tests))]
+    #         print(f"TESTS - {self.exo_py} : n_parts={ len(cuts) }") # | { cuts[0].strip() }")
+    #         assert len(cuts)==2
+
+    #         start,end = cuts
+    #         start = re.sub(r'(?i)# *tests?$', '', start, flags=re.MULTILINE).strip()
+    #         setattr(self, target_prop, start+"\n"+end)
+
+    #         src = get_sibling_of_current_page(self.env, self.py_name, tail=SiblingFile.exo)
+    #         alter = 'fusion_tmp' / src.relative_to(self.env.docs_dir_path)
+    #         self.__create_merged_file(alter)
 
 
-    def __create_merged_file(self, merge_file:Path):
-        order = [
-            (section, getattr(self, self.SECTION_TO_PROP[section]))
-                 for section in [
-                                    ScriptSection.hdr,
-                                    ScriptSection.user,
-                                    ScriptSection.corr,
-                                    ScriptSection.tests,
-                                    ScriptSection.secrets,
-                                ]]
-        merged = ''.join(
-            f"\n\n\n# --------- PYODIDE:{ section } --------- #\n\n{ content }"
-                for section,content in order
-                if content
-        )
 
-        merge_file.parent.mkdir(parents=True, exist_ok=True)
-        merge_file.touch(exist_ok=True)
-        merge_file.write_text(merged, encoding='utf-8')
+    # def __create_merged_file(self, merge_file:Path):
+    #     order = [
+    #         (section, getattr(self, self.SECTION_TO_PROP[section]))
+    #              for section in [
+    #                                 ScriptSection.env,
+    #                                 ScriptSection.user,
+    #                                 ScriptSection.corr,
+    #                                 ScriptSection.tests,
+    #                                 ScriptSection.secrets,
+    #                             ]]
+    #     merged = ''.join(
+    #         f"\n\n\n# --------- PYODIDE:{ section } --------- #\n\n{ content }"
+    #             for section,content in order
+    #             if content
+    #     )
+
+    #     merge_file.parent.mkdir(parents=True, exist_ok=True)
+    #     merge_file.touch(exist_ok=True)
+    #     merge_file.write_text(merged, encoding='utf-8')
```

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/messages.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/messages.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
-
-"""
-Define a class the can be passed to all macro functions, holding all the necessary data
-"""
 # pylint: disable=multiple-statements
 
 
 import json
 from typing import Any, Dict, List, Literal, Set, Tuple, Type, TYPE_CHECKING
 from dataclasses import dataclass
 from math import inf
@@ -44,17 +40,18 @@
 # Automatically updated from IdeConfig code, through build_tools:
 IdeConfigKey = Literal[
     'attempts_left',
     'auto_log_assert',
     'corr_content',
     'corr_rem_config',
     'encrypted',
+    'env_content',
     'excluded',
     'excluded_methods',
-    'hdr_content',
+    'post_content',
     'public_tests',
     'rec_limit',
     'secret_tests',
     'user_content',
     'white_list',
 ]
 
@@ -67,19 +64,20 @@
     Configuration of one IDE in one page of the documentation. Convertible to JS, to define the
     global variable specific to each page.
     """
 
     # BUILD_TOOL_TOKEN
     attempts_left: int = 0      # Not overwriting this means there is no counter displayed
     auto_log_assert: bool=None  # If None, use the global setting, CONFIG.showAssertionCodeOnFailedTest
-    hdr_content: str = ""       # HDR part of "exo.py"
+    env_content: str = ""       # HDR part of "exo.py"
     user_content: str = ""      # Non-HDR part of "exo.py" (initial code)
     corr_content: str = ""      # content of "exo_corr.py"
     public_tests: str = ""      # test part of "exo.py" (initial code)
     secret_tests: str = ""      # Content of "exo_test.py" (private tests)
+    post_content: str = ""      # Content to run after executions are done
     corr_rem_config: int = 0    # Bit mask:   has_corr=corr_rem_config&1 ; has_rem=corr_rem_config&2
     encrypted: bool = True      # Tells if the html content is still encrypted or not
     rec_limit: int = -1         # recursion depth to use at runtime, if defined (-1 otherwise).
     excluded: List[str]=None    # List of forbidden instructions (functions or packages)
     excluded_methods: List[str]=None # List of forbidden methods accesses
     white_list: List[str]=None  # White list of packages to preload at runtime
     # BUILD_TOOL_TOKEN
@@ -176,19 +174,23 @@
             )
 
 
     def set(self, editor_name:str, prop:IdeConfigKey, value:Any):
         """ Register an IDE configuration property, creating the IdeConfig on the fly,
             if it doesn't exist yet.
         """
-        if self.env._dev_mode and prop not in IdeConfig.__annotations__:    # pylint: disable=no-member
+        if self.env._dev_mode and prop not in IdeConfig.__annotations__:    # pylint: disable=no-member, protected-access
             msg = f'{prop!r} is not a valide attribut of { IdeConfig.__name__ } class'
             raise AttributeError(msg)
 
         if editor_name not in self:
             self[editor_name] = IdeConfig()
 
         setattr(self[editor_name], prop, value)
 
 
     def update_kinds(self , kinds:Tuple[ScriptKind]):
+        """
+        Register a kind of "need" (things to insert in the bottom of the content age, as css or
+        scripts) for the current page.
+        """
         self.needs.update(kinds)
```

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 import re
+from typing import List
 from mkdocs.exceptions import BuildError
 
 
 
 
 def replace_chunk(source:str, start:str, end:str, repl:str, *, at=0, keep_limiters=False):
     """ Given a @source and two delimiters/tokens, @start and @end, find those two tokens in
@@ -78,14 +79,21 @@
     """ Applique c ^ 43960 à chaque caractère de text (43960 = 0b1010101010101010) and send that
         as dot joined integers (needed to allow JS to decode emojis "the way python sees them")
         (...sort of...)
     """
     return ".".join( f"{ ord(c) ^ key :0>5}" for c in text )
 
 
+def items_comma_joiner(lst:List[str], join:str):
+    elements = lst[:]
+    if len(elements)>1:
+        last = elements.pop()
+        elements[-1] += f" {join} {last}"
+    elements = ', '.join(elements)
+    return elements
 
 
 def build_code_fence(
     content:str,
     indent:str="",
     line_nums=1,
     lang:str='python',
```

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,14 +100,17 @@
     max_attempts_before_corr_available = C.Type(int, default=5)
     """
     Global setting for all IDE in the documentation: max number of tries a user can do before
     correction and remarks become available (reminder: they are in a collapsed details/admonition,
     requiring the user to click to reveal the content. This way, they can still try to get the code
     right without actually seeing the solution, before actually giving up).
 
+    NOTE: using 1000 will result in an infinite number of attempts (ie. corr and REMs contents will
+    never become available if any).
+
     This behavior is global, but can be overridden on a "per IDE" base, using the `MAX` optional
     argument.
     """
 
     decrease_attempts_on_user_code_failure = C.Type(bool, default=True)
     """
     If true, any failure when running the user code during a validation will decrease the number
@@ -162,91 +165,121 @@
         If ever something unexpected is found, the build will be aborted, because no guarantee
         can be given about the correctness of the build in such a situation.
 
         In case of minor changes, this option will allow the build, but use it "at your own risks".
     """
 
 
-
     skip_py_md_paths_names_validation = C.Type(bool, default=False)
     """
     By default, the path names of all the `.py` and `.md` files present in the docs_dir are
     checked so that they do not contain any character other than letters, digits, dot or dash.
     This ensures that the macros related to IDEs will work properly.
 
     If unwanted characters are found, a BuildError is raised, but this verification can be turned
     off by setting this flag to True. Use it at your own risks.
     """
 
 
 
-    check_python_files = C.Type(bool, default=False)
-    """
-    If True, the different sections of the python files will be tested against each others during
-    the build and provide feedback in the console.
-
-    Unless the `soft_check` option is used, a BuildError will be raised if something considered
-    wrong happens. See the documentation for more details.
-
-    Warning:
-        - This is totally independent from the pyodide environment. For example, it won't
-          give any warning if a forbidden function is used in the tests (which will fail
-          on the website).
-        - These verifications __considerably increase the build time__ (expect something
-          around x10).
-    """
-
-    soft_check = C.Type(bool, default=True)
-    """
-    If True and `check_python_files` is also True, the python sections are verified, but the
-    build won't be interrupted if something wrong or suspicious is discovered: a message will
-    instead be displayed in the console.
-    """
-
-
-
     load_yaml_encoding = C.Type(str, default='utf-8')
     """
     Encoding to use when loading yaml data with the original MacrosPlugin functionalities :
 
     The original method doesn't use any encoding argument, which can lead to different behaviors
     between Windows and Linux (typically: during a pipeline!).
     """
 
 
+
     macros_with_indents = C.ListOfItems(C.Type(str), default=[])
     """
     Allow to register external macros, as a list of strings, that will need to insert properly
     indented multiline contents in the page.
 
     This is relying on `PyodideMacrosPlugin.get_indent` logistic.
     """
 
 
+
     bypass_indent_errors = C.Type(bool, default=False)
     """
     If True, all errors raised when trying to find what is the indentation level of a macro call
     are bypassed and a message is instead printed to the console.
 
     The purpose of this option is _not_ to deactivate the securities, but to allow gathering info
     about all the indentation problems at once: the resulting markdown content will most likely be
     incorrect and be rendered with unexpected results.
     """
 
 
+
     encrypt_corrections_and_rems = C.Type(bool, default=True)
     """
     If True, the html div under IDEs containing correction and remarks will be encrypted at build
     time.
 
     Passing this to False can be useful during development, but value should _ALWAYS_ be set
     to true on the deployed website: keep in mind the search engine can otherwise make surface
     contents from corrections and remarks as suggestions when the user is using the search bar.
     """
 
+    forbid_secrets_without_corr_or_REMs = C.Type(bool, default=True)
+    """
+    By default, this situation is considered invalid and `BuildError` will be raised.
+    If this is the desired behavior, set this option to false.
+    """
+
+    forbid_hidden_corr_and_REMs_without_secrets = C.Type(bool, default=True)
+    """
+    When building IDEs, the validation button will appear only when a `secrets` section exist.
+    If none is given while a corr section or REM files exist, their content will never be available
+    to the user because of the lack of validation button in the interface.
+
+    By default, this situation is considered invalid and `BuildError` will be raised.
+    If this is the desired behavior, set this option to false.
+    """
+
+    forbid_corr_and_REMs_with_infinite_attempts = C.Type(bool, default=True)
+    """
+    When building IDEs, if a `corr` section, a REM file or a VIS_REM file exist while the number
+    of attempts is infinite, that content will never become accessible to the user, unless they
+    pass the tests.
+
+    By default, this situation is considered invalid and `BuildError` will be raised.
+    If this is the desired behavior, set this option to false.
+    """
+
+
+    # check_python_files = C.Type(bool, default=False)
+    # """
+    # If True, the different sections of the python files will be tested against each others during
+    # the build and provide feedback in the console.
+
+    # Unless the `soft_check` option is used, a BuildError will be raised if something considered
+    # wrong happens. See the documentation for more details.
+
+    # Warning:
+    #     - This is totally independent from the pyodide environment. For example, it won't
+    #       give any warning if a forbidden function is used in the tests (which will fail
+    #       on the website).
+    #     - These verifications __considerably increase the build time__ (expect something
+    #       around x10).
+    # """
+
+    # soft_check = C.Type(bool, default=True)
+    # """
+    # If True and `check_python_files` is also True, the python sections are verified, but the
+    # build won't be interrupted if something wrong or suspicious is discovered: a message will
+    # instead be displayed in the console.
+    # """
+
+
+
+
 
 
 class QcmsConfig(Config):
     """ Options specific to the QCMs or QCSs"""
 
     hide = C.Type(bool, default=False)
     """
```

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             content = opt_path_or_content
         else:
             if opt_path_or_content is None or not opt_path_or_content.is_file():
                 return '','',''
             content = opt_path_or_content.read_text(encoding="utf-8")
 
         lst = self.HDR_PATTERN.split(content)
-        # If HDR tokens are present, split will return an empty string as first element, hence:
+        # NOTE: If HDR tokens are present, split will return an empty string as first element, so:
         #   - len == 1 : [content]
         #   - len == 3 : ['', hdr, content]
 
         if len(lst) not in (1,3):
             raise BuildError(
                 f"Wrong number of HDR/ENV tokens (found { len(lst)-1 }) in:\n"
                 f"{opt_path_or_content!s}"
```

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,20 +55,23 @@
 
     Note that, for the ConfigExtractor for to properly work, the class hierarchy has to
     extend MacrosPlugin at some point.
     """
 
     ignore_macros_plugin_diffs:              bool = ConfigExtractor('build')
     skip_py_md_paths_names_validation:       bool = ConfigExtractor('build')
-    check_python_files:                      bool = ConfigExtractor('build')
-    soft_check:                              bool = ConfigExtractor('build')
     load_yaml_encoding:                      str  = ConfigExtractor('build')
+    macros_with_indents:                List[str] = ConfigExtractor('build')
     bypass_indent_errors:                    bool = ConfigExtractor('build')
     encrypt_corrections_and_rems:            bool = ConfigExtractor('build')
-    macros_with_indents:                List[str] = ConfigExtractor('build')
+    forbid_secrets_without_corr_or_REMs:     bool = ConfigExtractor('build')
+    forbid_hidden_corr_and_REMs_without_secrets: bool = ConfigExtractor('build')
+    forbid_corr_and_REMs_with_infinite_attempts: bool = ConfigExtractor('build')
+    # check_python_files:                      bool = ConfigExtractor('build')
+    # soft_check:                              bool = ConfigExtractor('build')
 
     show_assertion_code_on_failed_test:      bool = ConfigExtractor("ides")
     max_attempts_before_corr_available:      bool = ConfigExtractor("ides")
     decrease_attempts_on_user_code_failure:  bool = ConfigExtractor("ides")
     default_ide_height_lines:       Optional[int] = ConfigExtractor("ides")
     deactivate_stdout_for_secrets: Optional[bool] = ConfigExtractor("ides")
     show_only_assertion_errors_for_secrets: Optional[bool] = ConfigExtractor("ides")
```

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,19 +186,20 @@
     vis_rem = '_VIS_REM.md'
 
 
 
 
 class ScriptSection:
     """ Name of each possible section used in a "monolithic" python file """
-    hdr = AutoDescriptor("env")
+    env = AutoDescriptor()
     user = AutoDescriptor("code")
     corr = AutoDescriptor()
     tests = AutoDescriptor()
     secrets = AutoDescriptor()
+    post  = AutoDescriptor()
```

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/__init__.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/custom_lang.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/scripts/custom_lang.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/custom_lang_src.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/scripts/custom_lang_src.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/__init__.py` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -30,20 +30,21 @@
 
     /*
     The following values are passed from python to JS through the main.html,
     once this script got loaded */
     //CONFIG_DUMP
     ignoreMacrosPluginDiffs: null,
     skipPyMdPathsNamesValidation: null,
-    checkPythonFiles: null,
-    softCheck: null,
     loadYamlEncoding: null,
+    macrosWithIndents: null,
     bypassIndentErrors: null,
     encryptCorrectionsAndRems: null,
-    macrosWithIndents: null,
+    forbidSecretsWithoutCorrOr_REMs: null,
+    forbidHiddenCorrAnd_REMsWithoutSecrets: null,
+    forbidCorrAnd_REMsWithInfiniteAttempts: null,
     showAssertionCodeOnFailedTest: null,
     maxAttemptsBeforeCorrAvailable: null,
     decreaseAttemptsOnUserCodeFailure: null,
     defaultIdeHeightLines: null,
     deactivateStdoutForSecrets: null,
     showOnlyAssertionErrorsForSecrets: null,
     hide: null,
@@ -136,17 +137,17 @@
 
 
     cutFeedback: true,
 
     COMMENTED_PATTERN: /(^\s*)(\S)(.?)/,
     // HDR_TOKEN_PATTERN:   /#\s*-[\s-]*HDR\s*-[\s-]*#/i,           // not used anymore
 
-    MODULE_REG: /File "<(env|exec|console)>", line (\d+)($|, in (?!await_fut))/,
-    TRACE_REG: /  File "<(env|exec|console)>"/,
-    TRACE_NUM_LINE: /File "<(?:env|exec|console)>", line (\d+)/,
+    MODULE_REG: /File "<(env|post|exec|console)>", line (\d+)($|, in (?!await_fut))/,
+    TRACE_REG: /  File "<(env|post|exec|console)>"/,
+    TRACE_NUM_LINE: /File "<(?:env|post|exec|console)>", line (\d+)/,
 
     ACE_COLOR_THEME: {
         customTheme: undefined,
         customThemeDefaultKey: "",
         aceStyle: undefined,
     },
```

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -24,19 +24,20 @@
 Inserted on the fly in each page needing IDEs (done by the macros_ide).
 The structure of this object is the following:
 
 var PAGE_IDES_CONFIG = {
     "editor_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx: {
         attempts_left: int = 0      # Not overwriting this means there is no counter displayed
         auto_log_assert: bool=None  # If None, use the global setting, CONFIG.showAssertionCodeOnFailedTest
-        hdr_content: str = ""       # HDR part of "exo.py"
+        env_content: str = ""       # HDR part of "exo.py"
         user_content: str = ""      # Non-HDR part of "exo.py" (initial code)
         corr_content: str = ""      # content of "exo_corr.py"
         public_tests: str = ""      # test part of "exo.py" (initial code)
         secret_tests: str = ""      # Content of "exo_test.py" (private tests)
+        post_content: str = ""      # Content to run after executions are done
         corr_rem_config: int = 0    # Bit mask:   has_corr=corr_rem_config&1 ; has_rem=corr_rem_config&2
         encrypted: bool = True      # Tells if the html content is still encrypted or not
         rec_limit: int = -1         # recursion depth to use at runtime, if defined (-1 otherwise).
         excluded: List[str]=None    # List of forbidden instructions (functions or packages)
         excluded_methods: List[str]=None # List of forbidden methods accesses
         white_list: List[str]=None  # White list of packages to preload at runtime
     }
@@ -50,15 +51,16 @@
 
     attemptsLeft: "attempts_left",
     autoLogAssert: "auto_log_assert",
     corrRemMask: "corr_rem_config",
     encrypted: "encrypted",
     excluded: "excluded",
     excludedMethods: "excluded_methods",
-    hdrContent: "hdr_content",
+    envContent: "env_content",
+    postContent: "post_content",
     publicTests: "public_tests",
     recLimit: "rec_limit",
     secretTests: "secret_tests",
     userContent: "user_content",
     whiteList: "white_list",
 }
```

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/main.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -31,15 +31,15 @@
 
     let [code, terminal, options] = await setupRuntimeAndTerminal(editorName);
     let stdErr = ""
 
     try {
         stdErr = await runPythonCodeWithOptions(code, terminal, options, true)
     } finally {
-        tearDownRuntimeAndTerminal(terminal, stdErr)
+        await tearDownRuntimeAndTerminal(editorName, options, terminal, stdErr)
     }
     $.terminal.active().focus()
 
 }, 'play')
 
 
 
@@ -96,15 +96,15 @@
             const nAttemptsLeft = updateIdeCounter(editorName)
             if (unhideSolutionAndRem(editorName, nAttemptsLeft, false)) {
                 finalMsg = enhanceFailureMsg(editorName, stdErr)
             }
         }
 
     } finally {
-        tearDownRuntimeAndTerminal(terminal, stdErr, finalMsg)
+        await tearDownRuntimeAndTerminal(editorName, options, terminal, stdErr, finalMsg)
     }
     $.terminal.active().focus()
 
 }, 'validate')
```

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -16,69 +16,41 @@
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 */
 
 
 
 
-/**Extract the content of the header code for the given editorName, and run its content
- * into pyodide environment.
- * */
-async function runHdrContent(editorName, options, terminal) {
-    const headerContent = securedExtraction(editorName, CONFIG.ideProp.hdrContent)
-    if (headerContent) {
-        await installAndImportMissingModules(headerContent, options, terminal)
-        await pyodide.runPythonAsync(headerContent, {
-            filename: '<env>'
-        })
-    }
-}
-
-
 /**Prepare the runtime python environment:
  *  - Save the current code in the editor to LocaleStorage
  *  - Refresh the basic functionalities
  *  - Refresh any HDR content in the environment
  *  - Refresh any exclusion logistic, by defining extra functions in the environment
  *  - Returns the modified code, with the active terminal
  */
 async function setupRuntimeAndTerminal(editorName) {
 
     // Extract the user's full code (possibly with public tests):
     let aceCode = await ace.edit(editorName).getSession().getValue();
 
     // save before anything else, in case an error occur somewhere...
     _save(editorName, aceCode)
+    storeUserCodeInPython(aceCode)
 
 
     // Build the default configuration options to use to run the user's code:
     const options = buildOptionsForPyodideRun(editorName)
     const terminal = await setupOrGetTerminalAndPyEnv("term_" + editorName, true);
 
     terminal.pause() // Pause is to avoid ">>>" showing up during executions
     terminal.clear() // Erase previous content
     terminal.echo(CONFIG.lang.runScript.msg) // tell the user it started to run
     await sleep() // Make sure the change is noticeable
 
-    let stdErr = '',
-        gotErr
-    setupStdIO()
-    try {
-        await runHdrContent(editorName, options, terminal)
-    } catch (err) {
-        gotErr = err
-        stdErr = generateErrorLog(err, "", false, false)
-    } finally {
-        let someMsg = getFullStdIO() + stdErr
-        if (someMsg) terminal.echo(someMsg)
-    }
-    if (gotErr) {
-        terminal.resume()
-        throw gotErr // Reraise, stopping executions if error
-    }
+    await runEnvironmentAsync(editorName, options, terminal, 'env')
 
     return [aceCode, terminal, options]
 }
 
 
 
 /**Actions performed once all the running code steps have been completed.
@@ -86,25 +58,78 @@
  * This function MUST be always executed, whatever happened before, even for JS errors,
  * otherwise the terminal would stay locked. So its call must be in a try/finally clause.
  *
  * @terminal :   the currently "active" (paused) terminal.
  * @stdErr :     message that got already displayed in the terminal, or empty string id no error.
  * @successMsg : only used for validation tests. If they succeeded, this string won't be empty.
  * */
-function tearDownRuntimeAndTerminal(terminal, stdErr, finalMsg = "") {
+async function tearDownRuntimeAndTerminal(editorName, options, terminal, stdErr, finalMsg = "") {
     jsLogger("[Teardown] -", JSON.stringify(stdErr))
 
+    await runEnvironmentAsync(editorName, options, terminal, 'post')
+
     if (!stdErr || finalMsg) {
         terminal.echo(finalMsg || CONFIG.lang.successMsg.msg)
     }
-    terminal.resume()
+    globalTearDown(terminal)
+}
+
+
+
+function storeUserCodeInPython(code) {
+    // The double quotes are all escaped to make sure no multiline string will cause troubles
+    const escapedCode = code.replace(/"/g, '\\"')
+    pyodide.runPython(`__builtins__.__USER_CODE__ = """${ escapedCode }"""`)
 }
 
 
 
+/**Extract the content of the an environment code for the given editorName, and run its content
+ * into pyodide environment.
+ * */
+async function runEnvironmentAsync(editorName, options, terminal, name) {
+    const prop = `${name}Content`
+
+    let gotErr, stdErr = ''
+    setupStdIO()
+    try {
+        const content = securedExtraction(editorName, CONFIG.ideProp[prop])
+        if (content) {
+            // make sure packages are installed
+            await installAndImportMissingModules(content, options, terminal)
+
+            // run env/post content
+            await pyodide.runPythonAsync(content, {
+                filename: `<${name}>`
+            })
+        }
+
+        // If an error occurred, give feedback in the console, with stdout teardown on the way,
+        // then stop everything :
+    } catch (err) {
+        gotErr = err
+        stdErr = generateErrorLog(err, "", false, false)
+    } finally {
+        let someMsg = getFullStdIO() + stdErr
+        if (someMsg) terminal.echo(someMsg)
+    }
+    if (gotErr) {
+        globalTearDown(terminal) // May occur in env section!
+        throw gotErr // Reraise, stopping executions if error
+    }
+}
+
+
+/**Generic teardown operations UNRELATED to pyodide (hence, JS or DOM related).
+ * */
+function globalTearDown(terminal) {
+    terminal.resume()
+}
+
+
 
 
 
 /**Applique c ^ key à chaque nombre de text
  * (Nota: 43960 = 0b1010101010101010)
  * */
 const decrypt_string = (text, key = 43960) => {
```

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js` & `pyodide_mkdocs_theme-0.7.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.6.1/pyproject.toml` & `pyodide_mkdocs_theme-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "0.6.1"
+version = "0.7.0"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
```

### Comparing `pyodide_mkdocs_theme-0.6.1/PKG-INFO` & `pyodide_mkdocs_theme-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 0.6.1
+Version: 0.7.0
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

