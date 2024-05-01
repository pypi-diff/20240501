# Comparing `tmp/pygpt_net-2.2.6.tar.gz` & `tmp/pygpt_net-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygpt_net-2.2.6.tar", max compression
+gzip compressed data, was "pygpt_net-2.2.7.tar", max compression
```

## Comparing `pygpt_net-2.2.6.tar` & `pygpt_net-2.2.7.tar`

### file list

```diff
@@ -1,845 +1,855 @@
--rwxr-xr-x   0        0        0    58625 2024-04-30 16:41:29.967889 pygpt_net-2.2.6/CHANGELOG.md
--rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.2.6/LICENSE
--rwxr-xr-x   0        0        0   133047 2024-04-30 16:41:29.967889 pygpt_net-2.2.6/README.md
--rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.2.6/icon.png
--rw-r--r--   0        0        0     2979 2024-04-30 16:41:29.971889 pygpt_net-2.2.6/pyproject.toml
--rwxr-xr-x   0        0        0    57597 2024-04-30 16:41:29.971889 pygpt_net-2.2.6/src/pygpt_net/CHANGELOG.txt
--rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.2.6/src/pygpt_net/LICENSE
--rwxr-xr-x   0        0        0     1024 2024-04-30 16:41:29.971889 pygpt_net-2.2.6/src/pygpt_net/__init__.py
--rwxr-xr-x   0        0        0    14345 2024-04-17 01:35:30.422055 pygpt_net-2.2.6/src/pygpt_net/app.py
--rwxr-xr-x   0        0        0    15485 2024-04-30 02:35:43.578880 pygpt_net-2.2.6/src/pygpt_net/config.py
--rwxr-xr-x   0        0        0     3601 2024-04-29 05:51:11.636212 pygpt_net-2.2.6/src/pygpt_net/container.py
--rwxr-xr-x   0        0        0     5164 2024-04-29 05:51:11.636212 pygpt_net-2.2.6/src/pygpt_net/controller/__init__.py
--rw-r--r--   0        0        0     4662 2024-02-25 05:32:34.229344 pygpt_net-2.2.6/src/pygpt_net/controller/agent/__init__.py
--rw-r--r--   0        0        0     6829 2024-03-17 13:18:45.622350 pygpt_net-2.2.6/src/pygpt_net/controller/agent/flow.py
--rw-r--r--   0        0        0     9877 2024-04-29 15:13:32.571516 pygpt_net-2.2.6/src/pygpt_net/controller/assistant/__init__.py
--rw-r--r--   0        0        0    20310 2024-04-30 16:41:29.971889 pygpt_net-2.2.6/src/pygpt_net/controller/assistant/batch.py
--rw-r--r--   0        0        0    13203 2024-04-27 14:05:11.727541 pygpt_net-2.2.6/src/pygpt_net/controller/assistant/editor.py
--rw-r--r--   0        0        0    14434 2024-04-30 02:35:43.578880 pygpt_net-2.2.6/src/pygpt_net/controller/assistant/files.py
--rwxr-xr-x   0        0        0    15545 2024-04-30 02:35:43.578880 pygpt_net-2.2.6/src/pygpt_net/controller/assistant/store.py
--rw-r--r--   0        0        0    17631 2024-04-29 05:51:11.636212 pygpt_net-2.2.6/src/pygpt_net/controller/assistant/threads.py
--rwxr-xr-x   0        0        0    15524 2024-04-30 02:35:43.578880 pygpt_net-2.2.6/src/pygpt_net/controller/attachment.py
--rw-r--r--   0        0        0     5972 2024-03-20 16:01:43.275339 pygpt_net-2.2.6/src/pygpt_net/controller/audio/__init__.py
--rw-r--r--   0        0        0     3922 2024-04-29 05:51:11.636212 pygpt_net-2.2.6/src/pygpt_net/controller/calendar/__init__.py
--rw-r--r--   0        0        0     8585 2024-04-11 03:43:59.058733 pygpt_net-2.2.6/src/pygpt_net/controller/calendar/note.py
--rwxr-xr-x   0        0        0    12681 2024-04-30 16:41:29.971889 pygpt_net-2.2.6/src/pygpt_net/controller/camera.py
--rw-r--r--   0        0        0     1628 2024-04-29 05:51:11.636212 pygpt_net-2.2.6/src/pygpt_net/controller/chat/__init__.py
--rwxr-xr-x   0        0        0    11529 2024-04-29 05:51:11.636212 pygpt_net-2.2.6/src/pygpt_net/controller/chat/common.py
--rw-r--r--   0        0        0     2156 2024-04-30 02:35:43.578880 pygpt_net-2.2.6/src/pygpt_net/controller/chat/files.py
--rwxr-xr-x   0        0        0     6457 2024-04-30 16:41:29.971889 pygpt_net-2.2.6/src/pygpt_net/controller/chat/image.py
--rwxr-xr-x   0        0        0     9801 2024-04-29 02:23:54.221168 pygpt_net-2.2.6/src/pygpt_net/controller/chat/input.py
--rwxr-xr-x   0        0        0    10189 2024-04-26 21:55:50.675598 pygpt_net-2.2.6/src/pygpt_net/controller/chat/output.py
--rwxr-xr-x   0        0        0     9610 2024-04-25 00:06:58.371551 pygpt_net-2.2.6/src/pygpt_net/controller/chat/render.py
--rw-r--r--   0        0        0    12507 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/controller/chat/text.py
--rw-r--r--   0        0        0     3382 2024-04-11 20:50:24.189030 pygpt_net-2.2.6/src/pygpt_net/controller/chat/vision.py
--rw-r--r--   0        0        0     5292 2024-03-26 17:12:51.286309 pygpt_net-2.2.6/src/pygpt_net/controller/command.py
--rw-r--r--   0        0        0     4485 2024-04-26 21:55:50.675598 pygpt_net-2.2.6/src/pygpt_net/controller/config/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.6/src/pygpt_net/controller/config/field/__init__.py
--rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.2.6/src/pygpt_net/controller/config/field/checkbox.py
--rw-r--r--   0        0        0     4863 2024-03-12 06:49:17.164785 pygpt_net-2.2.6/src/pygpt_net/controller/config/field/cmd.py
--rw-r--r--   0        0        0     3237 2024-04-27 14:05:11.727541 pygpt_net-2.2.6/src/pygpt_net/controller/config/field/combo.py
--rw-r--r--   0        0        0     6657 2024-03-12 06:49:17.164785 pygpt_net-2.2.6/src/pygpt_net/controller/config/field/dictionary.py
--rw-r--r--   0        0        0     3556 2024-03-15 15:31:21.786121 pygpt_net-2.2.6/src/pygpt_net/controller/config/field/input.py
--rw-r--r--   0        0        0     4580 2024-04-21 01:33:54.239765 pygpt_net-2.2.6/src/pygpt_net/controller/config/field/slider.py
--rw-r--r--   0        0        0     2337 2024-04-22 21:31:19.988317 pygpt_net-2.2.6/src/pygpt_net/controller/config/field/textarea.py
--rw-r--r--   0        0        0     7245 2024-04-24 02:39:32.054775 pygpt_net-2.2.6/src/pygpt_net/controller/config/placeholder.py
--rw-r--r--   0        0        0    29541 2024-04-29 05:51:11.636212 pygpt_net-2.2.6/src/pygpt_net/controller/ctx/__init__.py
--rw-r--r--   0        0        0     5434 2024-04-10 01:07:30.184635 pygpt_net-2.2.6/src/pygpt_net/controller/ctx/common.py
--rwxr-xr-x   0        0        0     7477 2024-04-29 04:57:38.321533 pygpt_net-2.2.6/src/pygpt_net/controller/ctx/extra.py
--rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.2.6/src/pygpt_net/controller/ctx/summarizer.py
--rw-r--r--   0        0        0     7732 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/controller/debug/__init__.py
--rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.2.6/src/pygpt_net/controller/dialogs/__init__.py
--rwxr-xr-x   0        0        0    13546 2024-04-30 02:35:43.578880 pygpt_net-2.2.6/src/pygpt_net/controller/dialogs/confirm.py
--rw-r--r--   0        0        0     5634 2024-03-07 01:04:26.437955 pygpt_net-2.2.6/src/pygpt_net/controller/dialogs/debug.py
--rwxr-xr-x   0        0        0     2582 2024-04-19 00:32:20.498428 pygpt_net-2.2.6/src/pygpt_net/controller/dialogs/info.py
--rwxr-xr-x   0        0        0    15699 2024-04-30 02:35:43.578880 pygpt_net-2.2.6/src/pygpt_net/controller/files.py
--rwxr-xr-x   0        0        0     4874 2024-04-21 01:33:54.239765 pygpt_net-2.2.6/src/pygpt_net/controller/finder.py
--rwxr-xr-x   0        0        0     7090 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/controller/idx/__init__.py
--rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.2.6/src/pygpt_net/controller/idx/common.py
--rwxr-xr-x   0        0        0    21150 2024-04-17 04:14:11.980074 pygpt_net-2.2.6/src/pygpt_net/controller/idx/indexer.py
--rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.2.6/src/pygpt_net/controller/idx/settings.py
--rw-r--r--   0        0        0     3289 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/controller/lang/__init__.py
--rw-r--r--   0        0        0     5080 2024-04-27 14:05:11.727541 pygpt_net-2.2.6/src/pygpt_net/controller/lang/custom.py
--rw-r--r--   0        0        0    20222 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/controller/lang/mapping.py
--rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.2.6/src/pygpt_net/controller/lang/plugins.py
--rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.2.6/src/pygpt_net/controller/lang/settings.py
--rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.2.6/src/pygpt_net/controller/launcher.py
--rwxr-xr-x   0        0        0    11297 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/controller/layout.py
--rw-r--r--   0        0        0     6521 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/controller/mode.py
--rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.2.6/src/pygpt_net/controller/model/__init__.py
--rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.2.6/src/pygpt_net/controller/model/editor.py
--rwxr-xr-x   0        0        0    11795 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/controller/notepad.py
--rw-r--r--   0        0        0     2572 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/controller/painter/__init__.py
--rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.2.6/src/pygpt_net/controller/painter/capture.py
--rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.2.6/src/pygpt_net/controller/painter/common.py
--rw-r--r--   0        0        0    14232 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/controller/plugins/__init__.py
--rw-r--r--   0        0        0    11914 2024-03-07 01:04:26.441956 pygpt_net-2.2.6/src/pygpt_net/controller/plugins/presets.py
--rw-r--r--   0        0        0     6040 2024-04-10 03:33:51.491189 pygpt_net-2.2.6/src/pygpt_net/controller/plugins/settings.py
--rwxr-xr-x   0        0        0    15949 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/controller/presets/__init__.py
--rwxr-xr-x   0        0        0    14997 2024-04-22 22:35:26.800429 pygpt_net-2.2.6/src/pygpt_net/controller/presets/editor.py
--rw-r--r--   0        0        0     7684 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/controller/settings/__init__.py
--rwxr-xr-x   0        0        0    14833 2024-04-24 02:39:32.054775 pygpt_net-2.2.6/src/pygpt_net/controller/settings/editor.py
--rw-r--r--   0        0        0    20965 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/controller/settings/profile.py
--rwxr-xr-x   0        0        0     8597 2024-04-14 16:40:07.849541 pygpt_net-2.2.6/src/pygpt_net/controller/settings/workdir.py
--rwxr-xr-x   0        0        0     6100 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/controller/theme/__init__.py
--rwxr-xr-x   0        0        0     5437 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/controller/theme/common.py
--rw-r--r--   0        0        0     5085 2024-04-24 23:37:32.612565 pygpt_net-2.2.6/src/pygpt_net/controller/theme/markdown.py
--rw-r--r--   0        0        0     4631 2024-04-24 02:39:32.054775 pygpt_net-2.2.6/src/pygpt_net/controller/theme/menu.py
--rw-r--r--   0        0        0     5028 2024-04-24 23:37:32.612565 pygpt_net-2.2.6/src/pygpt_net/controller/theme/nodes.py
--rw-r--r--   0        0        0     6093 2024-04-11 03:43:59.058733 pygpt_net-2.2.6/src/pygpt_net/controller/ui/__init__.py
--rw-r--r--   0        0        0     5156 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/controller/ui/mode.py
--rw-r--r--   0        0        0     2378 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/controller/ui/vision.py
--rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.2.6/src/pygpt_net/core/__init__.py
--rw-r--r--   0        0        0     4330 2024-04-26 21:55:50.675598 pygpt_net-2.2.6/src/pygpt_net/core/assistants/__init__.py
--rw-r--r--   0        0        0     9796 2024-04-30 02:35:43.578880 pygpt_net-2.2.6/src/pygpt_net/core/assistants/files.py
--rw-r--r--   0        0        0     7990 2024-04-30 02:35:43.578880 pygpt_net-2.2.6/src/pygpt_net/core/assistants/store.py
--rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.2.6/src/pygpt_net/core/attachments.py
--rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.2.6/src/pygpt_net/core/audio.py
--rw-r--r--   0        0        0     7404 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/core/bridge.py
--rw-r--r--   0        0        0     6634 2024-03-12 06:49:17.164785 pygpt_net-2.2.6/src/pygpt_net/core/calendar/__init__.py
--rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.2.6/src/pygpt_net/core/camera.py
--rw-r--r--   0        0        0     3240 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/core/chain/__init__.py
--rw-r--r--   0        0        0     4807 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/core/chain/chat.py
--rw-r--r--   0        0        0     5261 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/core/chain/completion.py
--rwxr-xr-x   0        0        0    10217 2024-03-17 14:26:02.923314 pygpt_net-2.2.6/src/pygpt_net/core/command.py
--rwxr-xr-x   0        0        0    32838 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/core/ctx/__init__.py
--rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.2.6/src/pygpt_net/core/ctx/idx.py
--rw-r--r--   0        0        0    15901 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/core/db/__init__.py
--rw-r--r--   0        0        0     8884 2024-04-17 01:35:30.422055 pygpt_net-2.2.6/src/pygpt_net/core/db/viewer.py
--rwxr-xr-x   0        0        0     9240 2024-03-26 17:12:51.290309 pygpt_net-2.2.6/src/pygpt_net/core/debug/__init__.py
--rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.2.6/src/pygpt_net/core/debug/agent.py
--rwxr-xr-x   0        0        0     2532 2024-04-26 21:55:50.675598 pygpt_net-2.2.6/src/pygpt_net/core/debug/assistants.py
--rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.2.6/src/pygpt_net/core/debug/attachments.py
--rwxr-xr-x   0        0        0     2305 2024-04-10 01:07:30.184635 pygpt_net-2.2.6/src/pygpt_net/core/debug/config.py
--rwxr-xr-x   0        0        0     3543 2024-04-14 04:42:08.288289 pygpt_net-2.2.6/src/pygpt_net/core/debug/context.py
--rw-r--r--   0        0        0      776 2024-03-07 01:04:26.441956 pygpt_net-2.2.6/src/pygpt_net/core/debug/db.py
--rw-r--r--   0        0        0     5194 2024-03-12 06:49:17.164785 pygpt_net-2.2.6/src/pygpt_net/core/debug/indexes.py
--rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.2.6/src/pygpt_net/core/debug/models.py
--rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.2.6/src/pygpt_net/core/debug/plugins.py
--rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.2.6/src/pygpt_net/core/debug/presets.py
--rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.2.6/src/pygpt_net/core/debug/ui.py
--rwxr-xr-x   0        0        0     9012 2024-03-26 17:12:51.290309 pygpt_net-2.2.6/src/pygpt_net/core/dispatcher.py
--rwxr-xr-x   0        0        0    15252 2024-04-29 10:51:04.365787 pygpt_net-2.2.6/src/pygpt_net/core/filesystem/__init__.py
--rw-r--r--   0        0        0     4074 2024-03-26 17:12:51.290309 pygpt_net-2.2.6/src/pygpt_net/core/filesystem/actions.py
--rw-r--r--   0        0        0     4123 2024-04-22 03:13:23.727782 pygpt_net-2.2.6/src/pygpt_net/core/filesystem/editor.py
--rw-r--r--   0        0        0     3385 2024-03-19 09:04:41.050928 pygpt_net-2.2.6/src/pygpt_net/core/filesystem/types.py
--rw-r--r--   0        0        0     2753 2024-04-21 01:33:54.243764 pygpt_net-2.2.6/src/pygpt_net/core/filesystem/url.py
--rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/core/history.py
--rwxr-xr-x   0        0        0    17238 2024-04-17 01:35:30.422055 pygpt_net-2.2.6/src/pygpt_net/core/idx/__init__.py
--rwxr-xr-x   0        0        0    12966 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/core/idx/chat.py
--rw-r--r--   0        0        0     2226 2024-02-28 03:58:59.309445 pygpt_net-2.2.6/src/pygpt_net/core/idx/context.py
--rwxr-xr-x   0        0        0    31850 2024-04-17 01:35:30.422055 pygpt_net-2.2.6/src/pygpt_net/core/idx/indexing.py
--rw-r--r--   0        0        0     4016 2024-04-26 23:49:43.379197 pygpt_net-2.2.6/src/pygpt_net/core/idx/llm.py
--rw-r--r--   0        0        0     5304 2024-04-17 01:35:30.422055 pygpt_net-2.2.6/src/pygpt_net/core/idx/metadata.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.2.6/src/pygpt_net/core/idx/types/__init__.py
--rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.2.6/src/pygpt_net/core/idx/types/ctx.py
--rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.2.6/src/pygpt_net/core/idx/types/external.py
--rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.2.6/src/pygpt_net/core/idx/types/files.py
--rwxr-xr-x   0        0        0     3774 2024-04-17 04:14:11.980074 pygpt_net-2.2.6/src/pygpt_net/core/idx/worker.py
--rwxr-xr-x   0        0        0     3288 2024-03-17 13:18:45.634349 pygpt_net-2.2.6/src/pygpt_net/core/image.py
--rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.2.6/src/pygpt_net/core/info.py
--rw-r--r--   0        0        0     2040 2024-03-25 10:26:39.426403 pygpt_net-2.2.6/src/pygpt_net/core/installer.py
--rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.2.6/src/pygpt_net/core/llm/__init__.py
--rwxr-xr-x   0        0        0     5112 2024-04-11 16:41:32.664297 pygpt_net-2.2.6/src/pygpt_net/core/locale.py
--rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.2.6/src/pygpt_net/core/models.py
--rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/core/modes.py
--rwxr-xr-x   0        0        0     3378 2024-04-10 01:07:30.184635 pygpt_net-2.2.6/src/pygpt_net/core/notepad.py
--rwxr-xr-x   0        0        0     4395 2024-03-09 21:41:28.185853 pygpt_net-2.2.6/src/pygpt_net/core/platforms.py
--rwxr-xr-x   0        0        0    14828 2024-04-28 08:05:35.578680 pygpt_net-2.2.6/src/pygpt_net/core/plugins.py
--rw-r--r--   0        0        0     9279 2024-03-17 13:18:45.634349 pygpt_net-2.2.6/src/pygpt_net/core/presets.py
--rw-r--r--   0        0        0     7650 2024-04-10 01:07:30.184635 pygpt_net-2.2.6/src/pygpt_net/core/profile.py
--rw-r--r--   0        0        0     2427 2024-04-22 22:35:26.800429 pygpt_net-2.2.6/src/pygpt_net/core/prompt/__init__.py
--rw-r--r--   0        0        0     2798 2024-04-22 22:35:26.800429 pygpt_net-2.2.6/src/pygpt_net/core/prompt/template.py
--rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.2.6/src/pygpt_net/core/render/__init__.py
--rw-r--r--   0        0        0     5024 2024-04-24 23:37:32.612565 pygpt_net-2.2.6/src/pygpt_net/core/render/base.py
--rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.243764 pygpt_net-2.2.6/src/pygpt_net/core/render/markdown/__init__.py
--rwxr-xr-x   0        0        0     5450 2024-04-22 05:35:04.663179 pygpt_net-2.2.6/src/pygpt_net/core/render/markdown/parser.py
--rwxr-xr-x   0        0        0    23291 2024-04-24 23:37:32.612565 pygpt_net-2.2.6/src/pygpt_net/core/render/markdown/renderer.py
--rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.2.6/src/pygpt_net/core/render/plain/__init__.py
--rw-r--r--   0        0        0    15716 2024-04-21 01:33:54.243764 pygpt_net-2.2.6/src/pygpt_net/core/render/plain/renderer.py
--rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.000000 pygpt_net-2.2.6/src/pygpt_net/core/render/web/__init__.py
--rwxr-xr-x   0        0        0     8564 2024-04-28 06:16:26.324027 pygpt_net-2.2.6/src/pygpt_net/core/render/web/parser.py
--rwxr-xr-x   0        0        0    42853 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/core/render/web/renderer.py
--rwxr-xr-x   0        0        0     7512 2024-04-24 23:37:32.612565 pygpt_net-2.2.6/src/pygpt_net/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-21 01:33:54.243764 pygpt_net-2.2.6/src/pygpt_net/core/text/__init__.py
--rwxr-xr-x   0        0        0     6566 2024-04-21 01:33:54.243764 pygpt_net-2.2.6/src/pygpt_net/core/text/finder.py
--rw-r--r--   0        0        0     2250 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/core/text/utils.py
--rw-r--r--   0        0        0     6487 2024-04-21 01:33:54.243764 pygpt_net-2.2.6/src/pygpt_net/core/text/web_finder.py
--rwxr-xr-x   0        0        0    14462 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/core/tokens.py
--rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.2.6/src/pygpt_net/core/updater/__init__.py
--rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.2.6/src/pygpt_net/core/web.py
--rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.2.6/src/pygpt_net/core/worker.py
--rwxr-xr-x   0        0        0    10603 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/data/config/config.json
--rwxr-xr-x   0        0        0    20313 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/data/config/models.json
--rw-r--r--   0        0        0     1440 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/data/config/modes.json
--rwxr-xr-x   0        0        0      459 2024-01-13 13:04:53.113674 pygpt_net-2.2.6/src/pygpt_net/data/config/presets/batman_and_joker.json
--rw-r--r--   0        0        0     2702 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/config/presets/current.agent.json
--rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/config/presets/current.assistant.json
--rwxr-xr-x   0        0        0      396 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/config/presets/current.chat.json
--rwxr-xr-x   0        0        0      385 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/config/presets/current.completion.json
--rwxr-xr-x   0        0        0      368 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/config/presets/current.img.json
--rwxr-xr-x   0        0        0      382 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/config/presets/current.langchain.json
--rw-r--r--   0        0        0      368 2024-03-03 02:59:46.037803 pygpt_net-2.2.6/src/pygpt_net/data/config/presets/current.llama_index.json
--rwxr-xr-x   0        0        0      392 2024-03-03 03:52:54.350656 pygpt_net-2.2.6/src/pygpt_net/data/config/presets/current.vision.json
--rwxr-xr-x   0        0        0      501 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/config/presets/dalle_white_cat.json
--rwxr-xr-x   0        0        0    32497 2024-04-29 05:51:11.640212 pygpt_net-2.2.6/src/pygpt_net/data/config/settings.json
--rw-r--r--   0        0        0      804 2024-03-17 13:18:45.634349 pygpt_net-2.2.6/src/pygpt_net/data/config/settings_section.json
--rwxr-xr-x   0        0        0      664 2024-03-18 04:54:07.000000 pygpt_net-2.2.6/src/pygpt_net/data/css/fix_windows.css
--rwxr-xr-x   0        0        0     1122 2024-04-19 00:29:50.000000 pygpt_net-2.2.6/src/pygpt_net/data/css/markdown.css
--rwxr-xr-x   0        0        0      730 2024-04-19 00:29:50.000000 pygpt_net-2.2.6/src/pygpt_net/data/css/markdown.dark.css
--rwxr-xr-x   0        0        0      833 2024-04-19 00:29:50.000000 pygpt_net-2.2.6/src/pygpt_net/data/css/markdown.light.css
--rwxr-xr-x   0        0        0      400 2024-04-20 05:54:38.000000 pygpt_net-2.2.6/src/pygpt_net/data/css/style.css
--rwxr-xr-x   0        0        0      729 2024-04-21 01:33:54.243764 pygpt_net-2.2.6/src/pygpt_net/data/css/style.dark.css
--rwxr-xr-x   0        0        0     1726 2024-04-20 05:55:02.000000 pygpt_net-2.2.6/src/pygpt_net/data/css/style.light.css
--rwxr-xr-x   0        0        0     3407 2024-04-24 23:37:32.612565 pygpt_net-2.2.6/src/pygpt_net/data/css/web.css
--rwxr-xr-x   0        0        0     1260 2024-04-25 03:37:50.192528 pygpt_net-2.2.6/src/pygpt_net/data/css/web.dark.css
--rwxr-xr-x   0        0        0     1235 2024-04-25 03:07:07.934949 pygpt_net-2.2.6/src/pygpt_net/data/css/web.light.css
--rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
--rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
--rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
--rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
--rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
--rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
--rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
--rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
--rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
--rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
--rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/OFL.txt
--rw-r--r--   0        0        0    77432 2024-04-08 04:19:15.417912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf
--rw-r--r--   0        0        0    82112 2024-04-08 04:19:15.417912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf
--rw-r--r--   0        0        0    81240 2024-04-08 04:19:15.417912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf
--rw-r--r--   0        0        0    75476 2024-04-08 04:19:15.421912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf
--rw-r--r--   0        0        0    75000 2024-04-08 04:19:15.421912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf
--rw-r--r--   0        0        0    77804 2024-04-08 04:19:15.421912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf
--rw-r--r--   0        0        0    76752 2024-04-08 04:19:15.421912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf
--rw-r--r--   0        0        0    74248 2024-04-08 04:19:15.421912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf
--rw-r--r--   0        0        0    74120 2024-04-08 04:19:15.421912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf
--rw-r--r--   0        0        0    79236 2024-04-08 04:19:15.421912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf
--rw-r--r--   0        0        0    78488 2024-04-08 04:19:15.425912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf
--rw-r--r--   0        0        0    73232 2024-04-08 04:19:15.425912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf
--rw-r--r--   0        0        0    88992 2024-04-08 04:19:15.425912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf
--rw-r--r--   0        0        0    94348 2024-04-08 04:19:15.425912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf
--rw-r--r--   0        0        0    93720 2024-04-08 04:19:15.425912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf
--rw-r--r--   0        0        0    88668 2024-04-08 04:19:15.429912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf
--rw-r--r--   0        0        0    79280 2024-04-08 04:19:15.429912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf
--rw-r--r--   0        0        0    85648 2024-04-08 04:19:15.429912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf
--rw-r--r--   0        0        0    85824 2024-04-08 04:19:15.429912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf
--rw-r--r--   0        0        0    80200 2024-04-08 04:19:15.429912 pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf
--rwxr-xr-x   0        0        0     4352 2024-03-18 04:54:07.633826 pygpt_net-2.2.6/src/pygpt_net/data/fonts/SpaceMono/OFL.txt
--rwxr-xr-x   0        0        0    86636 2024-03-18 04:54:07.633826 pygpt_net-2.2.6/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf
--rwxr-xr-x   0        0        0    95292 2024-03-18 04:54:07.633826 pygpt_net-2.2.6/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
--rwxr-xr-x   0        0        0   103524 2024-03-18 04:54:07.633826 pygpt_net-2.2.6/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf
--rwxr-xr-x   0        0        0    90904 2024-03-18 04:54:07.637826 pygpt_net-2.2.6/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf
--rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.2.6/src/pygpt_net/data/icon.ico
--rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.2.6/src/pygpt_net/data/icon.png
--rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.2.6/src/pygpt_net/data/icon_tray_busy.ico
--rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.2.6/src/pygpt_net/data/icon_tray_error.ico
--rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.2.6/src/pygpt_net/data/icon_tray_idle.ico
--rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/abc.svg
--rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/add.svg
--rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/add_circle.svg
--rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/add_folder.svg
--rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/add_library.svg
--rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/alarm.svg
--rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/apps.svg
--rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/asterisk.svg
--rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/attachment.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/attachments.svg
--rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/back.svg
--rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/backspace.svg
--rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/block.svg
--rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/bookmark.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/brush.svg
--rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/build.svg
--rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/calendar.svg
--rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/camera.svg
--rw-r--r--   0        0        0      987 2024-03-09 21:41:28.185853 pygpt_net-2.2.6/src/pygpt_net/data/icons/chat/audio.png
--rw-r--r--   0        0        0      798 2024-03-09 21:41:28.185853 pygpt_net-2.2.6/src/pygpt_net/data/icons/chat/copy.png
--rw-r--r--   0        0        0      737 2024-03-09 21:41:28.185853 pygpt_net-2.2.6/src/pygpt_net/data/icons/chat/delete.png
--rw-r--r--   0        0        0      837 2024-03-09 21:41:28.185853 pygpt_net-2.2.6/src/pygpt_net/data/icons/chat/edit.png
--rw-r--r--   0        0        0      715 2024-03-10 08:19:22.357281 pygpt_net-2.2.6/src/pygpt_net/data/icons/chat/join.png
--rw-r--r--   0        0        0      956 2024-03-09 21:41:28.185853 pygpt_net-2.2.6/src/pygpt_net/data/icons/chat/reload.png
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/chat.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/check.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/check_circle.svg
--rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/checklist.svg
--rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/circle.svg
--rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/clear.svg
--rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/clock.svg
--rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/close.svg
--rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/close_circle.svg
--rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/code.svg
--rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/computer.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/copy.svg
--rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/crop.svg
--rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/cut.svg
--rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.2.6/src/pygpt_net/data/icons/db.svg
--rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/delete.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/done.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/download.svg
--rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/draft.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/drag.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/edit.svg
--rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/emergency.svg
--rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/equalizer.svg
--rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/error.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/event_available.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/expand.svg
--rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/fast_forward.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/fast_rewind.svg
--rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/favorite.svg
--rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/folder.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/folder_filled.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/forward.svg
--rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/full.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/fullscreen.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/grid.svg
--rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/hearing.svg
--rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/help.svg
--rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/history.svg
--rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/home.svg
--rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/home_filled.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/image.svg
--rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/info.svg
--rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/input.svg
--rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/key.svg
--rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/keyboard.svg
--rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/language.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/list.svg
--rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/lock.svg
--rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/logout.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/map.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/memory.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/menu.svg
--rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/mic.svg
--rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/mic_off.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/more_horizontal.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/mute.svg
--rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/open_tab.svg
--rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/palette.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/paste.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/pause.svg
--rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/pause_circle.svg
--rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/photos.svg
--rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/pin.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/play.svg
--rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/play_pause.svg
--rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/playlist_add.svg
--rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/power.svg
--rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/print.svg
--rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/public_filled.svg
--rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.2.6/src/pygpt_net/data/icons/redo.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/reload.svg
--rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/repeat.svg
--rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/replay.svg
--rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/resize.svg
--rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/robot.svg
--rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/router.svg
--rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/save.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/schedule.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/screenshot.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/search.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/security.svg
--rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/sensors.svg
--rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/settings.svg
--rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/settings_filled.svg
--rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/share.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/shedule.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/sort.svg
--rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/stack.svg
--rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/stacks.svg
--rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.2.6/src/pygpt_net/data/icons/star.svg
--rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/stop.svg
--rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/stop_circle.svg
--rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/sync.svg
--rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/tag.svg
--rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/task.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/terminal.svg
--rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/text.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/textfile.svg
--rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/timer.svg
--rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/today.svg
--rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/tune.svg
--rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/undo.svg
--rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/update.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/updater.svg
--rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/upload.svg
--rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/video.svg
--rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/view.svg
--rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/voice.svg
--rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/volume.svg
--rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/warning.svg
--rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/webcam.svg
--rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.2.6/src/pygpt_net/data/icons/webcam_off.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/width.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/window.svg
--rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/work.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/zoom_in.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.2.6/src/pygpt_net/data/icons/zoom_out.svg
--rwxr-xr-x   0        0        0    46483 2024-04-29 15:13:32.575517 pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.de.ini
--rwxr-xr-x   0        0        0    54728 2024-04-29 15:13:32.575517 pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.en.ini
--rwxr-xr-x   0        0        0    46620 2024-04-29 15:13:32.575517 pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.es.ini
--rwxr-xr-x   0        0        0    48330 2024-04-29 15:13:32.575517 pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.fr.ini
--rwxr-xr-x   0        0        0    45664 2024-04-29 15:13:32.575517 pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.it.ini
--rwxr-xr-x   0        0        0    45600 2024-04-29 15:13:32.575517 pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.pl.ini
--rwxr-xr-x   0        0        0    64199 2024-04-29 15:13:32.575517 pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.uk.ini
--rwxr-xr-x   0        0        0    49212 2024-04-29 15:13:32.575517 pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.zh.ini
--rwxr-xr-x   0        0        0     1477 2024-03-12 06:49:17.164785 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.agent.en.ini
--rwxr-xr-x   0        0        0     1394 2024-03-12 06:49:17.164785 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.agent.pl.ini
--rwxr-xr-x   0        0        0     5371 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.audio_input.en.ini
--rwxr-xr-x   0        0        0     5129 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
--rwxr-xr-x   0        0        0     1721 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.audio_output.en.ini
--rwxr-xr-x   0        0        0     1395 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
--rw-r--r--   0        0        0      622 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
--rw-r--r--   0        0        0      853 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
--rwxr-xr-x   0        0        0     2365 2024-03-19 03:42:00.618910 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
--rwxr-xr-x   0        0        0     1614 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
--rwxr-xr-x   0        0        0      455 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
--rwxr-xr-x   0        0        0      528 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
--rwxr-xr-x   0        0        0     4234 2024-03-13 17:35:47.179523 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
--rwxr-xr-x   0        0        0     3584 2024-03-13 17:35:47.179523 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
--rw-r--r--   0        0        0     2280 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
--rw-r--r--   0        0        0     2765 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
--rw-r--r--   0        0        0     1042 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
--rw-r--r--   0        0        0     1511 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
--rwxr-xr-x   0        0        0     4840 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
--rwxr-xr-x   0        0        0     4660 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
--rw-r--r--   0        0        0      758 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.crontab.en.ini
--rw-r--r--   0        0        0      871 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.crontab.pl.ini
--rw-r--r--   0        0        0      338 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
--rw-r--r--   0        0        0      474 2024-03-12 03:34:38.663323 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
--rwxr-xr-x   0        0        0     1970 2024-03-13 17:35:47.179523 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
--rwxr-xr-x   0        0        0     1180 2024-03-13 17:35:47.179523 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
--rw-r--r--   0        0        0      396 2024-03-17 13:18:45.662349 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
--rw-r--r--   0        0        0      427 2024-03-17 13:18:45.662349 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
--rw-r--r--   0        0        0     1393 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
--rw-r--r--   0        0        0     1426 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
--rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.real_time.en.ini
--rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.real_time.pl.ini
--rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.2.6/src/pygpt_net/data/logo.png
--rw-r--r--   0        0        0    83051 2024-04-22 22:35:26.800429 pygpt_net-2.2.6/src/pygpt_net/data/prompts.csv
--rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.2.6/src/pygpt_net/data/win32/README.rtf
--rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.2.6/src/pygpt_net/data/win32/USER-LICENSE.rtf
--rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.2.6/src/pygpt_net/data/win32/pygpt.aip
--rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.2.6/src/pygpt_net/data/win32/qt.conf
--rw-r--r--   0        0        0    21736 2024-03-02 20:04:01.386329 pygpt_net-2.2.6/src/pygpt_net/icons.qrc
--rw-r--r--   0        0        0    90430 2024-03-02 20:05:43.048414 pygpt_net-2.2.6/src/pygpt_net/icons_rc.py
--rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.2.6/src/pygpt_net/item/__init__.py
--rw-r--r--   0        0        0     9587 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/item/assistant.py
--rw-r--r--   0        0        0     2110 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/item/attachment.py
--rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.2.6/src/pygpt_net/item/calendar_note.py
--rw-r--r--   0        0        0    11499 2024-04-29 05:51:11.644212 pygpt_net-2.2.6/src/pygpt_net/item/ctx.py
--rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.2.6/src/pygpt_net/item/index.py
--rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.2.6/src/pygpt_net/item/mode.py
--rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.2.6/src/pygpt_net/item/model.py
--rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.2.6/src/pygpt_net/item/notepad.py
--rw-r--r--   0        0        0     4052 2024-02-15 05:07:04.122540 pygpt_net-2.2.6/src/pygpt_net/item/preset.py
--rwxr-xr-x   0        0        0     7995 2024-04-21 18:06:27.128064 pygpt_net-2.2.6/src/pygpt_net/launcher.py
--rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.2.6/src/pygpt_net/migrations/Version20231227152900.py
--rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.2.6/src/pygpt_net/migrations/Version20231230095000.py
--rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.2.6/src/pygpt_net/migrations/Version20231231230000.py
--rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240106060000.py
--rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240107060000.py
--rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240222160000.py
--rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240223050000.py
--rw-r--r--   0        0        0      847 2024-03-03 22:43:17.403437 pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240303190000.py
--rw-r--r--   0        0        0     1110 2024-04-10 01:07:30.188635 pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240408180000.py
--rw-r--r--   0        0        0     1745 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240426050000.py
--rw-r--r--   0        0        0     1862 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/migrations/__init__.py
--rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.2.6/src/pygpt_net/migrations/base.py
--rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.6/src/pygpt_net/plugin/__init__.py
--rwxr-xr-x   0        0        0    15161 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/plugin/agent/__init__.py
--rwxr-xr-x   0        0        0    23567 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/plugin/audio_input/__init__.py
--rw-r--r--   0        0        0     4669 2024-04-24 23:37:32.612565 pygpt_net-2.2.6/src/pygpt_net/plugin/audio_input/simple.py
--rwxr-xr-x   0        0        0    10466 2024-03-19 09:04:41.054930 pygpt_net-2.2.6/src/pygpt_net/plugin/audio_input/worker.py
--rwxr-xr-x   0        0        0     6940 2024-03-10 10:31:05.897000 pygpt_net-2.2.6/src/pygpt_net/plugin/audio_output/__init__.py
--rw-r--r--   0        0        0     1806 2024-03-10 10:31:05.897000 pygpt_net-2.2.6/src/pygpt_net/plugin/audio_output/worker.py
--rwxr-xr-x   0        0        0    12704 2024-03-18 04:54:07.637826 pygpt_net-2.2.6/src/pygpt_net/plugin/base.py
--rwxr-xr-x   0        0        0    11734 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_api/__init__.py
--rw-r--r--   0        0        0     6243 2024-03-16 12:28:31.211383 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_api/worker.py
--rwxr-xr-x   0        0        0     9571 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
--rw-r--r--   0        0        0    14580 2024-04-28 01:03:40.864507 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
--rw-r--r--   0        0        0     8841 2024-04-28 01:03:50.072481 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
--rwxr-xr-x   0        0        0     5875 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_custom/__init__.py
--rw-r--r--   0        0        0     4507 2024-03-16 12:28:31.211383 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_custom/worker.py
--rwxr-xr-x   0        0        0    17031 2024-04-25 01:16:54.112014 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_files/__init__.py
--rwxr-xr-x   0        0        0    37969 2024-04-25 01:16:54.112014 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_files/worker.py
--rwxr-xr-x   0        0        0    20404 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_history/__init__.py
--rw-r--r--   0        0        0     6768 2024-04-30 16:41:29.975888 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_history/worker.py
--rwxr-xr-x   0        0        0     6124 2024-03-16 12:28:31.211383 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_serial/__init__.py
--rw-r--r--   0        0        0     8562 2024-03-16 12:28:31.211383 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_serial/worker.py
--rwxr-xr-x   0        0        0    21060 2024-03-17 14:26:02.923314 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_web/__init__.py
--rwxr-xr-x   0        0        0    12772 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_web/websearch.py
--rw-r--r--   0        0        0    10794 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_web/worker.py
--rwxr-xr-x   0        0        0     8163 2024-03-15 15:31:21.786121 pygpt_net-2.2.6/src/pygpt_net/plugin/crontab/__init__.py
--rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.2.6/src/pygpt_net/plugin/extra_prompt/__init__.py
--rwxr-xr-x   0        0        0    14776 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/plugin/idx_llama_index/__init__.py
--rw-r--r--   0        0        0     2825 2024-03-16 16:19:22.432875 pygpt_net-2.2.6/src/pygpt_net/plugin/idx_llama_index/worker.py
--rwxr-xr-x   0        0        0     6579 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/plugin/openai_dalle/__init__.py
--rwxr-xr-x   0        0        0    11659 2024-04-11 20:50:24.193030 pygpt_net-2.2.6/src/pygpt_net/plugin/openai_vision/__init__.py
--rwxr-xr-x   0        0        0     3865 2024-03-17 13:18:45.662349 pygpt_net-2.2.6/src/pygpt_net/plugin/real_time/__init__.py
--rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.6/src/pygpt_net/provider/__init__.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.2.6/src/pygpt_net/provider/audio_input/__init__.py
--rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.2.6/src/pygpt_net/provider/audio_input/base.py
--rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.2.6/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
--rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.2.6/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
--rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.2.6/src/pygpt_net/provider/audio_input/google_speech_recognition.py
--rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.2.6/src/pygpt_net/provider/audio_input/openai_whisper.py
--rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.2.6/src/pygpt_net/provider/audio_input/openai_whisper_local.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.6/src/pygpt_net/provider/audio_output/__init__.py
--rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.2.6/src/pygpt_net/provider/audio_output/base.py
--rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.2.6/src/pygpt_net/provider/audio_output/eleven_labs.py
--rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.2.6/src/pygpt_net/provider/audio_output/google_tts.py
--rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.2.6/src/pygpt_net/provider/audio_output/ms_azure_tts.py
--rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.2.6/src/pygpt_net/provider/audio_output/openai_tts.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/provider/core/__init__.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant/__init__.py
--rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant/base.py
--rw-r--r--   0        0        0     6399 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant/json_file.py
--rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_file/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_file/base.py
--rw-r--r--   0        0        0     5363 2024-04-29 15:13:32.575517 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py
--rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py
--rw-r--r--   0        0        0    10845 2024-04-29 15:13:32.575517 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py
--rw-r--r--   0        0        0     1796 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py
--rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_store/__init__.py
--rw-r--r--   0        0        0     1314 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_store/base.py
--rw-r--r--   0        0        0     3557 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py
--rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py
--rw-r--r--   0        0        0     7438 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py
--rw-r--r--   0        0        0     2120 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py
--rw-r--r--   0        0        0     4377 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_store/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/provider/core/attachment/__init__.py
--rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/provider/core/attachment/base.py
--rw-r--r--   0        0        0     5404 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/provider/core/attachment/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/provider/core/calendar/__init__.py
--rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/provider/core/calendar/base.py
--rw-r--r--   0        0        0     3953 2024-03-08 00:36:17.343108 pygpt_net-2.2.6/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
--rw-r--r--   0        0        0    11113 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/provider/core/config/__init__.py
--rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/provider/core/config/base.py
--rwxr-xr-x   0        0        0     5017 2024-04-11 01:27:21.134184 pygpt_net-2.2.6/src/pygpt_net/provider/core/config/json_file.py
--rwxr-xr-x   0        0        0    75723 2024-04-29 05:51:11.644212 pygpt_net-2.2.6/src/pygpt_net/provider/core/config/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/provider/core/ctx/__init__.py
--rw-r--r--   0        0        0     2577 2024-04-17 05:13:33.075416 pygpt_net-2.2.6/src/pygpt_net/provider/core/ctx/base.py
--rw-r--r--   0        0        0     9171 2024-04-17 05:13:33.075416 pygpt_net-2.2.6/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
--rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.2.6/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
--rw-r--r--   0        0        0    31650 2024-04-17 05:13:33.075416 pygpt_net-2.2.6/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
--rw-r--r--   0        0        0     7644 2024-04-10 01:07:30.188635 pygpt_net-2.2.6/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
--rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/ctx/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/history/__init__.py
--rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/history/base.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/history/patch.py
--rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/history/txt_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/index/__init__.py
--rw-r--r--   0        0        0     2875 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/provider/core/index/base.py
--rw-r--r--   0        0        0     8502 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.2.6/src/pygpt_net/provider/core/index/db_sqlite/patch.py
--rw-r--r--   0        0        0    17470 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/provider/core/index/db_sqlite/storage.py
--rw-r--r--   0        0        0      934 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/provider/core/index/db_sqlite/utils.py
--rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.2.6/src/pygpt_net/provider/core/index/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/index/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/mode/__init__.py
--rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/mode/base.py
--rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/mode/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/mode/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/model/__init__.py
--rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/model/base.py
--rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/model/json_file.py
--rw-r--r--   0        0        0     9946 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/provider/core/model/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/notepad/__init__.py
--rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/notepad/base.py
--rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
--rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
--rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/notepad/json_file.py
--rw-r--r--   0        0        0      488 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/provider/core/plugin_preset/__init__.py
--rw-r--r--   0        0        0      987 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/provider/core/plugin_preset/base.py
--rwxr-xr-x   0        0        0     3198 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/provider/core/plugin_preset/json_file.py
--rwxr-xr-x   0        0        0     1766 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/provider/core/plugin_preset/patch.py
--rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/preset/__init__.py
--rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.2.6/src/pygpt_net/provider/core/preset/base.py
--rwxr-xr-x   0        0        0     7887 2024-02-15 05:07:04.122540 pygpt_net-2.2.6/src/pygpt_net/provider/core/preset/json_file.py
--rw-r--r--   0        0        0     3166 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/core/preset/patch.py
--rw-r--r--   0        0        0     7390 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/provider/gpt/__init__.py
--rw-r--r--   0        0        0    13637 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/provider/gpt/assistants.py
--rw-r--r--   0        0        0     6356 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/provider/gpt/chat.py
--rw-r--r--   0        0        0     5579 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/provider/gpt/completion.py
--rw-r--r--   0        0        0     8255 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/provider/gpt/image.py
--rw-r--r--   0        0        0    16810 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/provider/gpt/store.py
--rw-r--r--   0        0        0     2072 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/provider/gpt/summarizer.py
--rw-r--r--   0        0        0     8004 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/provider/gpt/vision.py
--rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.2.6/src/pygpt_net/provider/gpt/worker/__init__.py
--rw-r--r--   0        0        0    20403 2024-04-30 02:35:43.578880 pygpt_net-2.2.6/src/pygpt_net/provider/gpt/worker/assistants.py
--rw-r--r--   0        0        0    15467 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/provider/gpt/worker/importer.py
--rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.6/src/pygpt_net/provider/llms/__init__.py
--rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.2.6/src/pygpt_net/provider/llms/anthropic.py
--rwxr-xr-x   0        0        0     2800 2024-03-13 15:08:01.569797 pygpt_net-2.2.6/src/pygpt_net/provider/llms/azure_openai.py
--rw-r--r--   0        0        0     3940 2024-03-15 15:31:21.790122 pygpt_net-2.2.6/src/pygpt_net/provider/llms/base.py
--rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.2.6/src/pygpt_net/provider/llms/hugging_face.py
--rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.2.6/src/pygpt_net/provider/llms/llama.py
--rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.2.6/src/pygpt_net/provider/llms/ollama.py
--rwxr-xr-x   0        0        0     2727 2024-03-13 15:08:01.569797 pygpt_net-2.2.6/src/pygpt_net/provider/llms/openai.py
--rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/__init__.py
--rw-r--r--   0        0        0     2515 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/base.py
--rw-r--r--   0        0        0     1258 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_csv.py
--rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_docx.py
--rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_epub.py
--rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_excel.py
--rw-r--r--   0        0        0     1268 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_html.py
--rw-r--r--   0        0        0     1923 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_image_vision.py
--rw-r--r--   0        0        0     1284 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_ipynb.py
--rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_json.py
--rw-r--r--   0        0        0     1292 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_markdown.py
--rw-r--r--   0        0        0     1214 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_pdf.py
--rw-r--r--   0        0        0     1832 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_video_audio.py
--rw-r--r--   0        0        0     1196 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_xml.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
--rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
--rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/database/__init__.py
--rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/database/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/github/__init__.py
--rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/github/issues.py
--rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/github/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/google/__init__.py
--rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/google/calendar.py
--rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/google/docs.py
--rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/google/gmail.py
--rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/google/keep.py
--rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/google/sheets.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
--rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/image_vision/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/json/__init__.py
--rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/json/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
--rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
--rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
--rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/video_audio/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
--rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/web_page/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/yt/__init__.py
--rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/yt/base.py
--rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/yt/utils.py
--rw-r--r--   0        0        0     3626 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_bitbucket.py
--rw-r--r--   0        0        0     2580 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
--rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_database.py
--rw-r--r--   0        0        0     3832 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_github_issues.py
--rw-r--r--   0        0        0     4377 2024-04-17 01:35:30.426055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_github_repo.py
--rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_google_calendar.py
--rw-r--r--   0        0        0     2480 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_google_docs.py
--rw-r--r--   0        0        0     3582 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_google_drive.py
--rw-r--r--   0        0        0     2710 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_google_gmail.py
--rw-r--r--   0        0        0     2412 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_google_keep.py
--rw-r--r--   0        0        0     2590 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_google_sheets.py
--rw-r--r--   0        0        0     4004 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
--rw-r--r--   0        0        0     1572 2024-03-12 06:49:17.168786 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_page.py
--rw-r--r--   0        0        0     1584 2024-03-12 06:49:17.172787 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_rss.py
--rw-r--r--   0        0        0     1853 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_sitemap.py
--rw-r--r--   0        0        0     2831 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_twitter.py
--rw-r--r--   0        0        0     1617 2024-03-12 06:49:17.172787 pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_yt.py
--rw-r--r--   0        0        0     5976 2024-03-08 22:55:56.889343 pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/__init__.py
--rw-r--r--   0        0        0     3791 2024-03-11 03:15:21.875594 pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/base.py
--rwxr-xr-x   0        0        0     3036 2024-03-11 03:15:21.875594 pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/chroma.py
--rw-r--r--   0        0        0     3016 2024-03-11 03:15:21.875594 pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/elasticsearch.py
--rw-r--r--   0        0        0     5041 2024-03-11 03:15:21.875594 pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/pinecode.py
--rw-r--r--   0        0        0     3047 2024-03-11 03:15:21.875594 pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/redis.py
--rw-r--r--   0        0        0     2455 2024-03-11 03:15:21.875594 pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/simple.py
--rw-r--r--   0        0        0     4322 2024-03-11 03:15:21.875594 pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/temp.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.6/src/pygpt_net/provider/web/__init__.py
--rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.2.6/src/pygpt_net/provider/web/base.py
--rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.2.6/src/pygpt_net/provider/web/google_custom_search.py
--rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.2.6/src/pygpt_net/provider/web/microsoft_bing.py
--rw-r--r--   0        0        0     3917 2024-04-19 00:32:20.498428 pygpt_net-2.2.6/src/pygpt_net/tools/__init__.py
--rwxr-xr-x   0        0        0     9791 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/tools/audio_transcriber/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/tools/audio_transcriber/ui/__init__.py
--rw-r--r--   0        0        0     5666 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py
--rw-r--r--   0        0        0     2116 2024-04-19 00:32:20.498428 pygpt_net-2.2.6/src/pygpt_net/tools/base.py
--rwxr-xr-x   0        0        0    11427 2024-04-19 00:32:20.498428 pygpt_net-2.2.6/src/pygpt_net/tools/code_interpreter/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/tools/code_interpreter/ui/__init__.py
--rw-r--r--   0        0        0     6622 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/tools/code_interpreter/ui/dialogs.py
--rw-r--r--   0        0        0     3518 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/tools/code_interpreter/ui/widgets.py
--rwxr-xr-x   0        0        0     9063 2024-04-14 16:40:07.849541 pygpt_net-2.2.6/src/pygpt_net/tools/image_viewer/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/tools/image_viewer/ui/__init__.py
--rw-r--r--   0        0        0     4962 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/tools/image_viewer/ui/dialogs.py
--rwxr-xr-x   0        0        0    18833 2024-04-19 00:32:20.498428 pygpt_net-2.2.6/src/pygpt_net/tools/indexer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/tools/indexer/ui/__init__.py
--rw-r--r--   0        0        0     1438 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/tools/indexer/ui/browse.py
--rw-r--r--   0        0        0     4355 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/tools/indexer/ui/ctx.py
--rw-r--r--   0        0        0     7985 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/tools/indexer/ui/dialogs.py
--rw-r--r--   0        0        0     4034 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/tools/indexer/ui/files.py
--rw-r--r--   0        0        0    10477 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/tools/indexer/ui/web.py
--rw-r--r--   0        0        0     3562 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/tools/indexer/ui/widgets.py
--rwxr-xr-x   0        0        0     6028 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/tools/media_player/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/tools/media_player/ui/__init__.py
--rw-r--r--   0        0        0     3590 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/tools/media_player/ui/dialogs.py
--rw-r--r--   0        0        0    15702 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/tools/media_player/ui/widgets.py
--rw-r--r--   0        0        0     8018 2024-04-14 16:40:07.849541 pygpt_net-2.2.6/src/pygpt_net/tools/text_editor/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/tools/text_editor/ui/__init__.py
--rw-r--r--   0        0        0     2906 2024-04-11 00:43:06.922864 pygpt_net-2.2.6/src/pygpt_net/tools/text_editor/ui/dialogs.py
--rw-r--r--   0        0        0     2754 2024-04-11 03:43:59.058733 pygpt_net-2.2.6/src/pygpt_net/tools/text_editor/ui/widgets.py
--rwxr-xr-x   0        0        0     6639 2024-04-10 01:07:30.188635 pygpt_net-2.2.6/src/pygpt_net/ui/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.6/src/pygpt_net/ui/base/__init__.py
--rw-r--r--   0        0        0     9209 2024-03-11 07:32:25.337990 pygpt_net-2.2.6/src/pygpt_net/ui/base/config_dialog.py
--rw-r--r--   0        0        0     3430 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/ui/base/context_menu.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/__init__.py
--rwxr-xr-x   0        0        0     5730 2024-04-11 20:50:24.193030 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/about.py
--rwxr-xr-x   0        0        0     5140 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/applog.py
--rwxr-xr-x   0        0        0     6480 2024-04-28 06:16:26.324027 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/assistant.py
--rw-r--r--   0        0        0    22532 2024-04-30 02:35:43.578880 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/assistant_store.py
--rwxr-xr-x   0        0        0     1765 2024-03-18 02:45:45.661442 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/changelog.py
--rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/create.py
--rw-r--r--   0        0        0    18520 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/db.py
--rwxr-xr-x   0        0        0     1864 2024-03-18 04:54:07.637826 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/debug.py
--rw-r--r--   0        0        0     5835 2024-03-12 06:49:17.172787 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/dictionary.py
--rwxr-xr-x   0        0        0     2926 2024-04-10 01:07:30.188635 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/editor.py
--rw-r--r--   0        0        0      957 2024-04-08 04:19:15.433912 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/find.py
--rwxr-xr-x   0        0        0     2876 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/image.py
--rwxr-xr-x   0        0        0     2272 2024-03-18 02:45:42.817463 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/license.py
--rwxr-xr-x   0        0        0     1823 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/logger.py
--rw-r--r--   0        0        0    13166 2024-03-10 12:05:00.639613 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/models.py
--rwxr-xr-x   0        0        0    20679 2024-03-12 06:49:17.172787 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/plugins.py
--rwxr-xr-x   0        0        0     6644 2024-02-15 05:07:04.122540 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/preset.py
--rw-r--r--   0        0        0     3796 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/preset_plugins.py
--rw-r--r--   0        0        0     4105 2024-04-10 01:07:30.188635 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/profile.py
--rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/rename.py
--rwxr-xr-x   0        0        0    15113 2024-03-10 12:05:00.639613 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/settings.py
--rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/snap.py
--rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/start.py
--rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/update.py
--rw-r--r--   0        0        0     4275 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/ui/dialog/workdir.py
--rwxr-xr-x   0        0        0     9009 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/ui/dialogs.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.6/src/pygpt_net/ui/layout/__init__.py
--rwxr-xr-x   0        0        0     1535 2024-04-09 20:34:52.308546 pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/__init__.py
--rwxr-xr-x   0        0        0     5518 2024-04-14 20:50:29.556142 pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/attachments.py
--rwxr-xr-x   0        0        0     5280 2024-04-29 15:13:32.575517 pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
--rw-r--r--   0        0        0     5996 2024-04-10 01:07:30.188635 pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/calendar.py
--rwxr-xr-x   0        0        0     9885 2024-04-09 20:35:55.668463 pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/input.py
--rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/markdown.py
--rwxr-xr-x   0        0        0    10452 2024-04-21 18:06:27.128064 pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/output.py
--rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/painter.py
--rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.2.6/src/pygpt_net/ui/layout/ctx/__init__.py
--rwxr-xr-x   0        0        0     6648 2024-04-21 19:42:04.971470 pygpt_net-2.2.6/src/pygpt_net/ui/layout/ctx/ctx_list.py
--rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.2.6/src/pygpt_net/ui/layout/ctx/search_input.py
--rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.2.6/src/pygpt_net/ui/layout/ctx/video.py
--rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.2.6/src/pygpt_net/ui/layout/status.py
--rwxr-xr-x   0        0        0     3477 2024-04-27 14:05:11.727541 pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/__init__.py
--rw-r--r--   0        0        0     2378 2024-01-30 17:23:19.901578 pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/agent.py
--rwxr-xr-x   0        0        0     4436 2024-04-30 02:35:43.578880 pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/assistants.py
--rwxr-xr-x   0        0        0     4254 2024-02-29 03:07:51.278132 pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/footer.py
--rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/image.py
--rw-r--r--   0        0        0     7007 2024-04-30 16:41:29.979888 pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/indexes.py
--rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/mode.py
--rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/model.py
--rwxr-xr-x   0        0        0     4125 2024-03-15 15:31:21.790122 pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/presets.py
--rwxr-xr-x   0        0        0     3242 2024-03-15 15:31:21.790122 pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/prompt.py
--rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/vision.py
--rw-r--r--   0        0        0     9644 2024-04-29 05:51:11.644212 pygpt_net-2.2.6/src/pygpt_net/ui/main.py
--rw-r--r--   0        0        0     1784 2024-03-26 17:12:51.294309 pygpt_net-2.2.6/src/pygpt_net/ui/menu/__init__.py
--rw-r--r--   0        0        0     5067 2024-04-19 00:32:20.498428 pygpt_net-2.2.6/src/pygpt_net/ui/menu/about.py
--rw-r--r--   0        0        0     1655 2024-03-20 16:01:43.283339 pygpt_net-2.2.6/src/pygpt_net/ui/menu/audio.py
--rw-r--r--   0        0        0     7870 2024-04-21 01:33:54.247764 pygpt_net-2.2.6/src/pygpt_net/ui/menu/config.py
--rw-r--r--   0        0        0     5185 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/ui/menu/debug.py
--rw-r--r--   0        0        0     3356 2024-04-17 05:13:33.075416 pygpt_net-2.2.6/src/pygpt_net/ui/menu/file.py
--rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.2.6/src/pygpt_net/ui/menu/lang.py
--rw-r--r--   0        0        0     2880 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/ui/menu/plugins.py
--rwxr-xr-x   0        0        0     3440 2024-04-24 23:37:32.616565 pygpt_net-2.2.6/src/pygpt_net/ui/menu/theme.py
--rw-r--r--   0        0        0     1134 2024-03-26 17:12:51.298308 pygpt_net-2.2.6/src/pygpt_net/ui/menu/tools.py
--rw-r--r--   0        0        0     2026 2024-03-20 16:01:43.283339 pygpt_net-2.2.6/src/pygpt_net/ui/menu/video.py
--rw-r--r--   0        0        0     6711 2024-04-14 20:50:29.556142 pygpt_net-2.2.6/src/pygpt_net/ui/tray.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.6/src/pygpt_net/ui/widget/__init__.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.6/src/pygpt_net/ui/widget/audio/__init__.py
--rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.2.6/src/pygpt_net/ui/widget/audio/input.py
--rw-r--r--   0        0        0     2198 2024-02-29 03:07:51.278132 pygpt_net-2.2.6/src/pygpt_net/ui/widget/audio/input_button.py
--rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.2.6/src/pygpt_net/ui/widget/audio/output.py
--rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.2.6/src/pygpt_net/ui/widget/calendar/__init__.py
--rw-r--r--   0        0        0     8120 2024-04-27 07:58:32.754704 pygpt_net-2.2.6/src/pygpt_net/ui/widget/calendar/select.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/__init__.py
--rwxr-xr-x   0        0        0     1429 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/alert.py
--rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/applog.py
--rw-r--r--   0        0        0     1712 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/assistant_store.py
--rw-r--r--   0        0        0      551 2024-03-26 17:12:51.298308 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/audio.py
--rwxr-xr-x   0        0        0     3802 2024-04-11 03:43:59.058733 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/base.py
--rwxr-xr-x   0        0        0     2302 2024-04-12 10:08:45.275113 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/confirm.py
--rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/create.py
--rw-r--r--   0        0        0     1585 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/db.py
--rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/debug.py
--rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/editor.py
--rwxr-xr-x   0        0        0     6185 2024-04-14 16:40:07.849541 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/editor_file.py
--rw-r--r--   0        0        0     3242 2024-04-11 03:43:59.058733 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/find.py
--rwxr-xr-x   0        0        0      816 2024-03-26 17:12:51.298308 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/image.py
--rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/info.py
--rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/license.py
--rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/logger.py
--rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/model.py
--rw-r--r--   0        0        0     1694 2024-04-10 01:07:30.188635 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/preset_plugins.py
--rw-r--r--   0        0        0     6686 2024-04-19 00:32:20.502428 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/profile.py
--rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/rename.py
--rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/settings.py
--rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/settings_plugin.py
--rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/snap.py
--rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/update.py
--rw-r--r--   0        0        0     1523 2024-03-26 17:12:51.298308 pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/workdir.py
--rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.2.6/src/pygpt_net/ui/widget/draw/__init__.py
--rw-r--r--   0        0        0    10903 2024-04-12 07:23:35.946682 pygpt_net-2.2.6/src/pygpt_net/ui/widget/draw/painter.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.6/src/pygpt_net/ui/widget/element/__init__.py
--rw-r--r--   0        0        0     4173 2024-04-29 15:13:32.575517 pygpt_net-2.2.6/src/pygpt_net/ui/widget/element/button.py
--rw-r--r--   0        0        0     2532 2024-03-07 01:04:26.445956 pygpt_net-2.2.6/src/pygpt_net/ui/widget/element/checkbox.py
--rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.2.6/src/pygpt_net/ui/widget/element/group.py
--rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.2.6/src/pygpt_net/ui/widget/element/labels.py
--rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.2.6/src/pygpt_net/ui/widget/filesystem/__init__.py
--rwxr-xr-x   0        0        0    22934 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/ui/widget/filesystem/explorer.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.6/src/pygpt_net/ui/widget/image/__init__.py
--rwxr-xr-x   0        0        0     3797 2024-03-26 17:12:51.298308 pygpt_net-2.2.6/src/pygpt_net/ui/widget/image/display.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/__init__.py
--rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/assistant.py
--rw-r--r--   0        0        0     3715 2024-04-29 15:13:32.575517 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/assistant_store.py
--rwxr-xr-x   0        0        0     7055 2024-04-14 20:50:29.556142 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/attachment.py
--rwxr-xr-x   0        0        0     2446 2024-04-10 01:07:30.188635 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/base.py
--rwxr-xr-x   0        0        0    17502 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/context.py
--rw-r--r--   0        0        0     5861 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/db.py
--rw-r--r--   0        0        0     3658 2024-03-07 01:04:26.449956 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/debug.py
--rw-r--r--   0        0        0     4818 2024-04-17 01:35:30.430055 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/index.py
--rw-r--r--   0        0        0     6794 2024-04-27 14:05:11.727541 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/index_combo.py
--rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/mode.py
--rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/model.py
--rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/model_editor.py
--rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/plugin.py
--rwxr-xr-x   0        0        0     4071 2024-02-01 01:48:09.378583 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/preset.py
--rw-r--r--   0        0        0     3899 2024-03-07 01:04:26.449956 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/preset_plugins.py
--rw-r--r--   0        0        0     4432 2024-04-10 01:07:30.192635 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/profile.py
--rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/settings.py
--rwxr-xr-x   0        0        0     4382 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/uploaded.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/__init__.py
--rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/checkbox.py
--rw-r--r--   0        0        0     5503 2024-03-12 06:49:17.172787 pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/cmd.py
--rw-r--r--   0        0        0     3592 2024-04-27 10:44:46.049374 pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/combo.py
--rwxr-xr-x   0        0        0    12672 2024-03-11 03:15:21.879593 pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/dictionary.py
--rwxr-xr-x   0        0        0     9304 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/input.py
--rw-r--r--   0        0        0     2601 2024-04-22 22:35:26.800429 pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/prompt.py
--rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/slider.py
--rwxr-xr-x   0        0        0     2684 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/textarea.py
--rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.2.6/src/pygpt_net/ui/widget/tabs/Input.py
--rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.2.6/src/pygpt_net/ui/widget/tabs/__init__.py
--rw-r--r--   0        0        0     2814 2024-04-10 01:07:30.192635 pygpt_net-2.2.6/src/pygpt_net/ui/widget/tabs/output.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/__init__.py
--rw-r--r--   0        0        0     5098 2024-04-21 01:33:54.247764 pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/calendar_note.py
--rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/create.py
--rw-r--r--   0        0        0     5450 2024-04-21 01:33:54.247764 pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/editor.py
--rw-r--r--   0        0        0     1543 2024-04-11 03:43:59.058733 pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/find.py
--rwxr-xr-x   0        0        0     6059 2024-04-22 22:35:26.800429 pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/input.py
--rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/name.py
--rwxr-xr-x   0        0        0     6583 2024-04-21 01:33:54.247764 pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/notepad.py
--rwxr-xr-x   0        0        0     5086 2024-04-23 23:11:13.260159 pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/output.py
--rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/rename.py
--rwxr-xr-x   0        0        0     1833 2024-04-12 10:08:45.275113 pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/search_input.py
--rwxr-xr-x   0        0        0    10060 2024-04-27 14:05:11.727541 pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/web.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.6/src/pygpt_net/ui/widget/vision/__init__.py
--rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.2.6/src/pygpt_net/ui/widget/vision/camera.py
--rwxr-xr-x   0        0        0     5470 2024-04-26 21:55:50.679597 pygpt_net-2.2.6/src/pygpt_net/utils.py
--rw-r--r--   0        0        0   136763 1970-01-01 00:00:00.000000 pygpt_net-2.2.6/PKG-INFO
+-rwxr-xr-x   0        0        0    59167 2024-05-01 18:08:40.466948 pygpt_net-2.2.7/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.2.7/LICENSE
+-rwxr-xr-x   0        0        0   136279 2024-05-01 18:08:40.466948 pygpt_net-2.2.7/README.md
+-rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.2.7/icon.png
+-rw-r--r--   0        0        0     2979 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/pyproject.toml
+-rwxr-xr-x   0        0        0    58137 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/CHANGELOG.txt
+-rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.2.7/src/pygpt_net/LICENSE
+-rwxr-xr-x   0        0        0     1024 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/__init__.py
+-rwxr-xr-x   0        0        0    14447 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/app.py
+-rwxr-xr-x   0        0        0    15485 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/config.py
+-rwxr-xr-x   0        0        0     3683 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/container.py
+-rwxr-xr-x   0        0        0     5164 2024-04-29 05:51:11.636212 pygpt_net-2.2.7/src/pygpt_net/controller/__init__.py
+-rw-r--r--   0        0        0     4730 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/agent/__init__.py
+-rw-r--r--   0        0        0     1408 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/agent/experts.py
+-rw-r--r--   0        0        0     6829 2024-03-17 13:18:45.622350 pygpt_net-2.2.7/src/pygpt_net/controller/agent/flow.py
+-rw-r--r--   0        0        0     9877 2024-04-29 15:13:32.571516 pygpt_net-2.2.7/src/pygpt_net/controller/assistant/__init__.py
+-rw-r--r--   0        0        0    20310 2024-04-30 16:41:29.971889 pygpt_net-2.2.7/src/pygpt_net/controller/assistant/batch.py
+-rw-r--r--   0        0        0    13203 2024-04-27 14:05:11.727541 pygpt_net-2.2.7/src/pygpt_net/controller/assistant/editor.py
+-rw-r--r--   0        0        0    14434 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/controller/assistant/files.py
+-rwxr-xr-x   0        0        0    15545 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/controller/assistant/store.py
+-rw-r--r--   0        0        0    17631 2024-04-29 05:51:11.636212 pygpt_net-2.2.7/src/pygpt_net/controller/assistant/threads.py
+-rwxr-xr-x   0        0        0    15524 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/controller/attachment.py
+-rw-r--r--   0        0        0     5972 2024-03-20 16:01:43.275339 pygpt_net-2.2.7/src/pygpt_net/controller/audio/__init__.py
+-rw-r--r--   0        0        0     3922 2024-04-29 05:51:11.636212 pygpt_net-2.2.7/src/pygpt_net/controller/calendar/__init__.py
+-rw-r--r--   0        0        0     8585 2024-04-11 03:43:59.058733 pygpt_net-2.2.7/src/pygpt_net/controller/calendar/note.py
+-rwxr-xr-x   0        0        0    12681 2024-04-30 16:41:29.971889 pygpt_net-2.2.7/src/pygpt_net/controller/camera.py
+-rw-r--r--   0        0        0     1628 2024-04-29 05:51:11.636212 pygpt_net-2.2.7/src/pygpt_net/controller/chat/__init__.py
+-rwxr-xr-x   0        0        0    11581 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/chat/common.py
+-rw-r--r--   0        0        0     2156 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/controller/chat/files.py
+-rwxr-xr-x   0        0        0     6533 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/chat/image.py
+-rwxr-xr-x   0        0        0    10399 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/chat/input.py
+-rwxr-xr-x   0        0        0    11382 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/chat/output.py
+-rwxr-xr-x   0        0        0     9610 2024-04-25 00:06:58.371551 pygpt_net-2.2.7/src/pygpt_net/controller/chat/render.py
+-rw-r--r--   0        0        0    12683 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/chat/text.py
+-rw-r--r--   0        0        0     3382 2024-04-11 20:50:24.189030 pygpt_net-2.2.7/src/pygpt_net/controller/chat/vision.py
+-rw-r--r--   0        0        0     5292 2024-03-26 17:12:51.286309 pygpt_net-2.2.7/src/pygpt_net/controller/command.py
+-rw-r--r--   0        0        0     4485 2024-04-26 21:55:50.675598 pygpt_net-2.2.7/src/pygpt_net/controller/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/__init__.py
+-rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/checkbox.py
+-rw-r--r--   0        0        0     4863 2024-03-12 06:49:17.164785 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/cmd.py
+-rw-r--r--   0        0        0     3237 2024-04-27 14:05:11.727541 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/combo.py
+-rw-r--r--   0        0        0     6657 2024-03-12 06:49:17.164785 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/dictionary.py
+-rw-r--r--   0        0        0     3556 2024-03-15 15:31:21.786121 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/input.py
+-rw-r--r--   0        0        0     4580 2024-04-21 01:33:54.239765 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/slider.py
+-rw-r--r--   0        0        0     2337 2024-04-22 21:31:19.988317 pygpt_net-2.2.7/src/pygpt_net/controller/config/field/textarea.py
+-rw-r--r--   0        0        0     7255 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/config/placeholder.py
+-rw-r--r--   0        0        0    29541 2024-04-29 05:51:11.636212 pygpt_net-2.2.7/src/pygpt_net/controller/ctx/__init__.py
+-rw-r--r--   0        0        0     5434 2024-04-10 01:07:30.184635 pygpt_net-2.2.7/src/pygpt_net/controller/ctx/common.py
+-rwxr-xr-x   0        0        0     7477 2024-04-29 04:57:38.321533 pygpt_net-2.2.7/src/pygpt_net/controller/ctx/extra.py
+-rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.2.7/src/pygpt_net/controller/ctx/summarizer.py
+-rw-r--r--   0        0        0     7732 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/debug/__init__.py
+-rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/__init__.py
+-rwxr-xr-x   0        0        0    13546 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/confirm.py
+-rw-r--r--   0        0        0     5634 2024-03-07 01:04:26.437955 pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/debug.py
+-rwxr-xr-x   0        0        0     2582 2024-04-19 00:32:20.498428 pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/info.py
+-rwxr-xr-x   0        0        0    15699 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/controller/files.py
+-rwxr-xr-x   0        0        0     4874 2024-04-21 01:33:54.239765 pygpt_net-2.2.7/src/pygpt_net/controller/finder.py
+-rwxr-xr-x   0        0        0     7090 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/idx/__init__.py
+-rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.2.7/src/pygpt_net/controller/idx/common.py
+-rwxr-xr-x   0        0        0    21150 2024-04-17 04:14:11.980074 pygpt_net-2.2.7/src/pygpt_net/controller/idx/indexer.py
+-rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.2.7/src/pygpt_net/controller/idx/settings.py
+-rw-r--r--   0        0        0     3289 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/lang/__init__.py
+-rw-r--r--   0        0        0     5080 2024-04-27 14:05:11.727541 pygpt_net-2.2.7/src/pygpt_net/controller/lang/custom.py
+-rw-r--r--   0        0        0    20222 2024-04-30 16:41:29.975888 pygpt_net-2.2.7/src/pygpt_net/controller/lang/mapping.py
+-rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.2.7/src/pygpt_net/controller/lang/plugins.py
+-rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.2.7/src/pygpt_net/controller/lang/settings.py
+-rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.2.7/src/pygpt_net/controller/launcher.py
+-rwxr-xr-x   0        0        0    11297 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/layout.py
+-rw-r--r--   0        0        0     6521 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/mode.py
+-rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.2.7/src/pygpt_net/controller/model/__init__.py
+-rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.2.7/src/pygpt_net/controller/model/editor.py
+-rwxr-xr-x   0        0        0    11795 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/notepad.py
+-rw-r--r--   0        0        0     2572 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/painter/__init__.py
+-rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.2.7/src/pygpt_net/controller/painter/capture.py
+-rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.2.7/src/pygpt_net/controller/painter/common.py
+-rw-r--r--   0        0        0    14232 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/plugins/__init__.py
+-rw-r--r--   0        0        0    11914 2024-03-07 01:04:26.441956 pygpt_net-2.2.7/src/pygpt_net/controller/plugins/presets.py
+-rw-r--r--   0        0        0     6040 2024-04-10 03:33:51.491189 pygpt_net-2.2.7/src/pygpt_net/controller/plugins/settings.py
+-rwxr-xr-x   0        0        0    17127 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/presets/__init__.py
+-rwxr-xr-x   0        0        0    16058 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/presets/editor.py
+-rw-r--r--   0        0        0     4937 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/presets/experts.py
+-rw-r--r--   0        0        0     7684 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/settings/__init__.py
+-rwxr-xr-x   0        0        0    14833 2024-04-24 02:39:32.054775 pygpt_net-2.2.7/src/pygpt_net/controller/settings/editor.py
+-rw-r--r--   0        0        0    20965 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/controller/settings/profile.py
+-rwxr-xr-x   0        0        0     8597 2024-04-14 16:40:07.849541 pygpt_net-2.2.7/src/pygpt_net/controller/settings/workdir.py
+-rwxr-xr-x   0        0        0     6308 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/theme/__init__.py
+-rwxr-xr-x   0        0        0     5437 2024-04-30 16:41:29.975888 pygpt_net-2.2.7/src/pygpt_net/controller/theme/common.py
+-rw-r--r--   0        0        0     5085 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/controller/theme/markdown.py
+-rw-r--r--   0        0        0     4631 2024-04-24 02:39:32.054775 pygpt_net-2.2.7/src/pygpt_net/controller/theme/menu.py
+-rw-r--r--   0        0        0     5028 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/controller/theme/nodes.py
+-rw-r--r--   0        0        0     6093 2024-04-11 03:43:59.058733 pygpt_net-2.2.7/src/pygpt_net/controller/ui/__init__.py
+-rw-r--r--   0        0        0     6663 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/controller/ui/mode.py
+-rw-r--r--   0        0        0     2378 2024-04-30 16:41:29.975888 pygpt_net-2.2.7/src/pygpt_net/controller/ui/vision.py
+-rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.2.7/src/pygpt_net/core/__init__.py
+-rw-r--r--   0        0        0     4330 2024-04-26 21:55:50.675598 pygpt_net-2.2.7/src/pygpt_net/core/assistants/__init__.py
+-rw-r--r--   0        0        0     9796 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/core/assistants/files.py
+-rw-r--r--   0        0        0     7990 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/core/assistants/store.py
+-rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.2.7/src/pygpt_net/core/attachments.py
+-rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.2.7/src/pygpt_net/core/audio.py
+-rw-r--r--   0        0        0     7490 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/core/bridge.py
+-rw-r--r--   0        0        0     6634 2024-03-12 06:49:17.164785 pygpt_net-2.2.7/src/pygpt_net/core/calendar/__init__.py
+-rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.2.7/src/pygpt_net/core/camera.py
+-rw-r--r--   0        0        0     3330 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/core/chain/__init__.py
+-rw-r--r--   0        0        0     4988 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/core/chain/chat.py
+-rw-r--r--   0        0        0     5413 2024-05-01 18:08:40.474948 pygpt_net-2.2.7/src/pygpt_net/core/chain/completion.py
+-rwxr-xr-x   0        0        0    10217 2024-03-17 14:26:02.923314 pygpt_net-2.2.7/src/pygpt_net/core/command.py
+-rwxr-xr-x   0        0        0    34627 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/ctx/__init__.py
+-rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.2.7/src/pygpt_net/core/ctx/idx.py
+-rw-r--r--   0        0        0    15975 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/db/__init__.py
+-rw-r--r--   0        0        0     8884 2024-04-17 01:35:30.422055 pygpt_net-2.2.7/src/pygpt_net/core/db/viewer.py
+-rwxr-xr-x   0        0        0     9240 2024-03-26 17:12:51.290309 pygpt_net-2.2.7/src/pygpt_net/core/debug/__init__.py
+-rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.2.7/src/pygpt_net/core/debug/agent.py
+-rwxr-xr-x   0        0        0     2532 2024-04-26 21:55:50.675598 pygpt_net-2.2.7/src/pygpt_net/core/debug/assistants.py
+-rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.2.7/src/pygpt_net/core/debug/attachments.py
+-rwxr-xr-x   0        0        0     2305 2024-04-10 01:07:30.184635 pygpt_net-2.2.7/src/pygpt_net/core/debug/config.py
+-rwxr-xr-x   0        0        0     3543 2024-04-14 04:42:08.288289 pygpt_net-2.2.7/src/pygpt_net/core/debug/context.py
+-rw-r--r--   0        0        0      776 2024-03-07 01:04:26.441956 pygpt_net-2.2.7/src/pygpt_net/core/debug/db.py
+-rw-r--r--   0        0        0     5194 2024-03-12 06:49:17.164785 pygpt_net-2.2.7/src/pygpt_net/core/debug/indexes.py
+-rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.2.7/src/pygpt_net/core/debug/models.py
+-rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.2.7/src/pygpt_net/core/debug/plugins.py
+-rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.2.7/src/pygpt_net/core/debug/presets.py
+-rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.2.7/src/pygpt_net/core/debug/ui.py
+-rwxr-xr-x   0        0        0     9307 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/dispatcher.py
+-rw-r--r--   0        0        0     9117 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/experts/__init__.py
+-rwxr-xr-x   0        0        0    15252 2024-04-29 10:51:04.365787 pygpt_net-2.2.7/src/pygpt_net/core/filesystem/__init__.py
+-rw-r--r--   0        0        0     4074 2024-03-26 17:12:51.290309 pygpt_net-2.2.7/src/pygpt_net/core/filesystem/actions.py
+-rw-r--r--   0        0        0     4123 2024-04-22 03:13:23.727782 pygpt_net-2.2.7/src/pygpt_net/core/filesystem/editor.py
+-rw-r--r--   0        0        0     3385 2024-03-19 09:04:41.050928 pygpt_net-2.2.7/src/pygpt_net/core/filesystem/types.py
+-rw-r--r--   0        0        0     2753 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/core/filesystem/url.py
+-rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/core/history.py
+-rwxr-xr-x   0        0        0    17238 2024-04-17 01:35:30.422055 pygpt_net-2.2.7/src/pygpt_net/core/idx/__init__.py
+-rwxr-xr-x   0        0        0    13030 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/idx/chat.py
+-rw-r--r--   0        0        0     2443 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/idx/context.py
+-rwxr-xr-x   0        0        0    31850 2024-04-17 01:35:30.422055 pygpt_net-2.2.7/src/pygpt_net/core/idx/indexing.py
+-rw-r--r--   0        0        0     4016 2024-04-26 23:49:43.379197 pygpt_net-2.2.7/src/pygpt_net/core/idx/llm.py
+-rw-r--r--   0        0        0     5304 2024-04-17 01:35:30.422055 pygpt_net-2.2.7/src/pygpt_net/core/idx/metadata.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.2.7/src/pygpt_net/core/idx/types/__init__.py
+-rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.2.7/src/pygpt_net/core/idx/types/ctx.py
+-rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.2.7/src/pygpt_net/core/idx/types/external.py
+-rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/core/idx/types/files.py
+-rwxr-xr-x   0        0        0     3774 2024-04-17 04:14:11.980074 pygpt_net-2.2.7/src/pygpt_net/core/idx/worker.py
+-rwxr-xr-x   0        0        0     3288 2024-03-17 13:18:45.634349 pygpt_net-2.2.7/src/pygpt_net/core/image.py
+-rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.2.7/src/pygpt_net/core/info.py
+-rw-r--r--   0        0        0     2040 2024-03-25 10:26:39.426403 pygpt_net-2.2.7/src/pygpt_net/core/installer.py
+-rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.2.7/src/pygpt_net/core/llm/__init__.py
+-rwxr-xr-x   0        0        0     5112 2024-04-11 16:41:32.664297 pygpt_net-2.2.7/src/pygpt_net/core/locale.py
+-rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/core/models.py
+-rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/core/modes.py
+-rwxr-xr-x   0        0        0     3378 2024-04-10 01:07:30.184635 pygpt_net-2.2.7/src/pygpt_net/core/notepad.py
+-rwxr-xr-x   0        0        0     4395 2024-03-09 21:41:28.185853 pygpt_net-2.2.7/src/pygpt_net/core/platforms.py
+-rwxr-xr-x   0        0        0    14828 2024-04-28 08:05:35.578680 pygpt_net-2.2.7/src/pygpt_net/core/plugins.py
+-rw-r--r--   0        0        0    12366 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/presets.py
+-rw-r--r--   0        0        0     7650 2024-04-10 01:07:30.184635 pygpt_net-2.2.7/src/pygpt_net/core/profile.py
+-rw-r--r--   0        0        0     4529 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/prompt/__init__.py
+-rw-r--r--   0        0        0     2798 2024-04-22 22:35:26.800429 pygpt_net-2.2.7/src/pygpt_net/core/prompt/template.py
+-rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.2.7/src/pygpt_net/core/render/__init__.py
+-rw-r--r--   0        0        0     5024 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/core/render/base.py
+-rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/core/render/markdown/__init__.py
+-rwxr-xr-x   0        0        0     5450 2024-04-22 05:35:04.663179 pygpt_net-2.2.7/src/pygpt_net/core/render/markdown/parser.py
+-rwxr-xr-x   0        0        0    23291 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/core/render/markdown/renderer.py
+-rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.2.7/src/pygpt_net/core/render/plain/__init__.py
+-rw-r--r--   0        0        0    15716 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/core/render/plain/renderer.py
+-rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.000000 pygpt_net-2.2.7/src/pygpt_net/core/render/web/__init__.py
+-rwxr-xr-x   0        0        0     8564 2024-04-28 06:16:26.324027 pygpt_net-2.2.7/src/pygpt_net/core/render/web/parser.py
+-rwxr-xr-x   0        0        0    43236 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/render/web/renderer.py
+-rwxr-xr-x   0        0        0     7512 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/core/text/__init__.py
+-rwxr-xr-x   0        0        0     6566 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/core/text/finder.py
+-rw-r--r--   0        0        0     2250 2024-04-29 05:51:11.640212 pygpt_net-2.2.7/src/pygpt_net/core/text/utils.py
+-rw-r--r--   0        0        0     6487 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/core/text/web_finder.py
+-rwxr-xr-x   0        0        0    14472 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/core/tokens.py
+-rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.2.7/src/pygpt_net/core/updater/__init__.py
+-rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.2.7/src/pygpt_net/core/web.py
+-rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.2.7/src/pygpt_net/core/worker.py
+-rwxr-xr-x   0        0        0    14457 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/config.json
+-rwxr-xr-x   0        0        0    20573 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/models.json
+-rw-r--r--   0        0        0     1595 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/modes.json
+-rwxr-xr-x   0        0        0      528 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/batman_and_joker.json
+-rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.agent.json
+-rwxr-xr-x   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.assistant.json
+-rwxr-xr-x   0        0        0      447 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.chat.json
+-rwxr-xr-x   0        0        0      436 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.completion.json
+-rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.expert.json
+-rwxr-xr-x   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.img.json
+-rwxr-xr-x   0        0        0      433 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.langchain.json
+-rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.llama_index.json
+-rwxr-xr-x   0        0        0      447 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/current.vision.json
+-rwxr-xr-x   0        0        0      552 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/dalle_white_cat.json
+-rw-r--r--   0        0        0      474 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/joke_agent.json
+-rw-r--r--   0        0        0      683 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/presets/joke_expert.json
+-rwxr-xr-x   0        0        0    33579 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/config/settings.json
+-rw-r--r--   0        0        0      804 2024-03-17 13:18:45.634349 pygpt_net-2.2.7/src/pygpt_net/data/config/settings_section.json
+-rwxr-xr-x   0        0        0      664 2024-03-18 04:54:07.000000 pygpt_net-2.2.7/src/pygpt_net/data/css/fix_windows.css
+-rwxr-xr-x   0        0        0     1122 2024-04-19 00:29:50.000000 pygpt_net-2.2.7/src/pygpt_net/data/css/markdown.css
+-rwxr-xr-x   0        0        0      730 2024-04-19 00:29:50.000000 pygpt_net-2.2.7/src/pygpt_net/data/css/markdown.dark.css
+-rwxr-xr-x   0        0        0      833 2024-04-19 00:29:50.000000 pygpt_net-2.2.7/src/pygpt_net/data/css/markdown.light.css
+-rwxr-xr-x   0        0        0      400 2024-04-20 05:54:38.000000 pygpt_net-2.2.7/src/pygpt_net/data/css/style.css
+-rwxr-xr-x   0        0        0      729 2024-04-21 01:33:54.243764 pygpt_net-2.2.7/src/pygpt_net/data/css/style.dark.css
+-rwxr-xr-x   0        0        0     1726 2024-04-20 05:55:02.000000 pygpt_net-2.2.7/src/pygpt_net/data/css/style.light.css
+-rwxr-xr-x   0        0        0     3407 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/data/css/web.css
+-rwxr-xr-x   0        0        0     1260 2024-04-25 03:37:50.192528 pygpt_net-2.2.7/src/pygpt_net/data/css/web.dark.css
+-rwxr-xr-x   0        0        0     1235 2024-04-25 03:07:07.934949 pygpt_net-2.2.7/src/pygpt_net/data/css/web.light.css
+-rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
+-rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
+-rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
+-rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
+-rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
+-rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
+-rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
+-rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
+-rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
+-rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
+-rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/OFL.txt
+-rw-r--r--   0        0        0    77432 2024-04-08 04:19:15.417912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf
+-rw-r--r--   0        0        0    82112 2024-04-08 04:19:15.417912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf
+-rw-r--r--   0        0        0    81240 2024-04-08 04:19:15.417912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf
+-rw-r--r--   0        0        0    75476 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf
+-rw-r--r--   0        0        0    75000 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf
+-rw-r--r--   0        0        0    77804 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf
+-rw-r--r--   0        0        0    76752 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf
+-rw-r--r--   0        0        0    74248 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf
+-rw-r--r--   0        0        0    74120 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf
+-rw-r--r--   0        0        0    79236 2024-04-08 04:19:15.421912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf
+-rw-r--r--   0        0        0    78488 2024-04-08 04:19:15.425912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf
+-rw-r--r--   0        0        0    73232 2024-04-08 04:19:15.425912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf
+-rw-r--r--   0        0        0    88992 2024-04-08 04:19:15.425912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf
+-rw-r--r--   0        0        0    94348 2024-04-08 04:19:15.425912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf
+-rw-r--r--   0        0        0    93720 2024-04-08 04:19:15.425912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf
+-rw-r--r--   0        0        0    88668 2024-04-08 04:19:15.429912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf
+-rw-r--r--   0        0        0    79280 2024-04-08 04:19:15.429912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf
+-rw-r--r--   0        0        0    85648 2024-04-08 04:19:15.429912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf
+-rw-r--r--   0        0        0    85824 2024-04-08 04:19:15.429912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf
+-rw-r--r--   0        0        0    80200 2024-04-08 04:19:15.429912 pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf
+-rwxr-xr-x   0        0        0     4352 2024-03-18 04:54:07.633826 pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/OFL.txt
+-rwxr-xr-x   0        0        0    86636 2024-03-18 04:54:07.633826 pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf
+-rwxr-xr-x   0        0        0    95292 2024-03-18 04:54:07.633826 pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
+-rwxr-xr-x   0        0        0   103524 2024-03-18 04:54:07.633826 pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf
+-rwxr-xr-x   0        0        0    90904 2024-03-18 04:54:07.637826 pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf
+-rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.2.7/src/pygpt_net/data/icon.ico
+-rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.2.7/src/pygpt_net/data/icon.png
+-rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.2.7/src/pygpt_net/data/icon_tray_busy.ico
+-rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.2.7/src/pygpt_net/data/icon_tray_error.ico
+-rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.2.7/src/pygpt_net/data/icon_tray_idle.ico
+-rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/abc.svg
+-rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/add.svg
+-rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/add_circle.svg
+-rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/add_folder.svg
+-rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/add_library.svg
+-rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/alarm.svg
+-rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/apps.svg
+-rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/asterisk.svg
+-rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/attachment.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/attachments.svg
+-rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/back.svg
+-rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/backspace.svg
+-rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/block.svg
+-rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/bookmark.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/brush.svg
+-rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/build.svg
+-rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/calendar.svg
+-rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/camera.svg
+-rw-r--r--   0        0        0      987 2024-03-09 21:41:28.185853 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/audio.png
+-rw-r--r--   0        0        0      798 2024-03-09 21:41:28.185853 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/copy.png
+-rw-r--r--   0        0        0      737 2024-03-09 21:41:28.185853 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/delete.png
+-rw-r--r--   0        0        0      837 2024-03-09 21:41:28.185853 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/edit.png
+-rw-r--r--   0        0        0      715 2024-03-10 08:19:22.357281 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/join.png
+-rw-r--r--   0        0        0      956 2024-03-09 21:41:28.185853 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/reload.png
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/chat.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/check.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/check_circle.svg
+-rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/checklist.svg
+-rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/circle.svg
+-rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/clear.svg
+-rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/clock.svg
+-rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/close.svg
+-rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/close_circle.svg
+-rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/code.svg
+-rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/computer.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/copy.svg
+-rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/crop.svg
+-rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/cut.svg
+-rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.2.7/src/pygpt_net/data/icons/db.svg
+-rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/delete.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/done.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/download.svg
+-rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/draft.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/drag.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/edit.svg
+-rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/emergency.svg
+-rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/equalizer.svg
+-rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/error.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/event_available.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/expand.svg
+-rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/fast_forward.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/fast_rewind.svg
+-rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/favorite.svg
+-rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/folder.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/folder_filled.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/forward.svg
+-rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/full.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/fullscreen.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/grid.svg
+-rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/hearing.svg
+-rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/help.svg
+-rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/history.svg
+-rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/home.svg
+-rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/home_filled.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/image.svg
+-rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/info.svg
+-rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/input.svg
+-rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/key.svg
+-rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/keyboard.svg
+-rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/language.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/list.svg
+-rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/lock.svg
+-rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/logout.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/map.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/memory.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/menu.svg
+-rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/mic.svg
+-rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/mic_off.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/more_horizontal.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/mute.svg
+-rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/open_tab.svg
+-rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/palette.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/paste.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/pause.svg
+-rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/pause_circle.svg
+-rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/photos.svg
+-rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/pin.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/play.svg
+-rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/play_pause.svg
+-rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/playlist_add.svg
+-rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/power.svg
+-rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/print.svg
+-rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/public_filled.svg
+-rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.2.7/src/pygpt_net/data/icons/redo.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/reload.svg
+-rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/repeat.svg
+-rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/replay.svg
+-rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/resize.svg
+-rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/robot.svg
+-rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/router.svg
+-rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/save.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/schedule.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/screenshot.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/search.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/security.svg
+-rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/sensors.svg
+-rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/settings.svg
+-rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/settings_filled.svg
+-rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/share.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/shedule.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/sort.svg
+-rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/stack.svg
+-rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/stacks.svg
+-rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.2.7/src/pygpt_net/data/icons/star.svg
+-rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/stop.svg
+-rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/stop_circle.svg
+-rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/sync.svg
+-rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/tag.svg
+-rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/task.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/terminal.svg
+-rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/text.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/textfile.svg
+-rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/timer.svg
+-rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/today.svg
+-rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/tune.svg
+-rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/undo.svg
+-rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/update.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/updater.svg
+-rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/upload.svg
+-rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/video.svg
+-rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/view.svg
+-rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/voice.svg
+-rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/volume.svg
+-rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/warning.svg
+-rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/webcam.svg
+-rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.2.7/src/pygpt_net/data/icons/webcam_off.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/width.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/window.svg
+-rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/work.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/zoom_in.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.2.7/src/pygpt_net/data/icons/zoom_out.svg
+-rwxr-xr-x   0        0        0    47611 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.de.ini
+-rwxr-xr-x   0        0        0    55722 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.en.ini
+-rwxr-xr-x   0        0        0    47738 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.es.ini
+-rwxr-xr-x   0        0        0    49440 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.fr.ini
+-rwxr-xr-x   0        0        0    46777 2024-05-01 18:08:40.478948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.it.ini
+-rwxr-xr-x   0        0        0    46707 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.pl.ini
+-rwxr-xr-x   0        0        0    65739 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.uk.ini
+-rwxr-xr-x   0        0        0    50133 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.zh.ini
+-rwxr-xr-x   0        0        0     1477 2024-03-12 06:49:17.164785 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.agent.en.ini
+-rwxr-xr-x   0        0        0     1394 2024-03-12 06:49:17.164785 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.agent.pl.ini
+-rwxr-xr-x   0        0        0     5371 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_input.en.ini
+-rwxr-xr-x   0        0        0     5129 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
+-rwxr-xr-x   0        0        0     1721 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_output.en.ini
+-rwxr-xr-x   0        0        0     1395 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
+-rw-r--r--   0        0        0      622 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
+-rw-r--r--   0        0        0      853 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
+-rwxr-xr-x   0        0        0     2365 2024-03-19 03:42:00.618910 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
+-rwxr-xr-x   0        0        0     1614 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
+-rwxr-xr-x   0        0        0      455 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
+-rwxr-xr-x   0        0        0      528 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
+-rwxr-xr-x   0        0        0     4234 2024-03-13 17:35:47.179523 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
+-rwxr-xr-x   0        0        0     3584 2024-03-13 17:35:47.179523 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
+-rw-r--r--   0        0        0     2280 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
+-rw-r--r--   0        0        0     2765 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
+-rw-r--r--   0        0        0     1042 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
+-rw-r--r--   0        0        0     1511 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
+-rwxr-xr-x   0        0        0     4840 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
+-rwxr-xr-x   0        0        0     4660 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
+-rw-r--r--   0        0        0      758 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.crontab.en.ini
+-rw-r--r--   0        0        0      871 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.crontab.pl.ini
+-rw-r--r--   0        0        0       99 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.experts.en.ini
+-rw-r--r--   0        0        0      338 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
+-rw-r--r--   0        0        0      474 2024-03-12 03:34:38.663323 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
+-rwxr-xr-x   0        0        0     1970 2024-03-13 17:35:47.179523 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
+-rwxr-xr-x   0        0        0     1180 2024-03-13 17:35:47.179523 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
+-rw-r--r--   0        0        0      396 2024-03-17 13:18:45.662349 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
+-rw-r--r--   0        0        0      427 2024-03-17 13:18:45.662349 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
+-rw-r--r--   0        0        0     1393 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
+-rw-r--r--   0        0        0     1426 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
+-rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.real_time.en.ini
+-rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.real_time.pl.ini
+-rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.2.7/src/pygpt_net/data/logo.png
+-rw-r--r--   0        0        0    83051 2024-04-22 22:35:26.800429 pygpt_net-2.2.7/src/pygpt_net/data/prompts.csv
+-rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.2.7/src/pygpt_net/data/win32/README.rtf
+-rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.2.7/src/pygpt_net/data/win32/USER-LICENSE.rtf
+-rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.2.7/src/pygpt_net/data/win32/pygpt.aip
+-rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.2.7/src/pygpt_net/data/win32/qt.conf
+-rw-r--r--   0        0        0    21736 2024-03-02 20:04:01.386329 pygpt_net-2.2.7/src/pygpt_net/icons.qrc
+-rw-r--r--   0        0        0    90430 2024-03-02 20:05:43.048414 pygpt_net-2.2.7/src/pygpt_net/icons_rc.py
+-rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.2.7/src/pygpt_net/item/__init__.py
+-rw-r--r--   0        0        0     9587 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/item/assistant.py
+-rw-r--r--   0        0        0     2110 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/item/attachment.py
+-rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/item/calendar_note.py
+-rw-r--r--   0        0        0    12376 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/item/ctx.py
+-rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/item/index.py
+-rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.2.7/src/pygpt_net/item/mode.py
+-rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/item/model.py
+-rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/item/notepad.py
+-rw-r--r--   0        0        0     4680 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/item/preset.py
+-rwxr-xr-x   0        0        0     7995 2024-04-21 18:06:27.128064 pygpt_net-2.2.7/src/pygpt_net/launcher.py
+-rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20231227152900.py
+-rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20231230095000.py
+-rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20231231230000.py
+-rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240106060000.py
+-rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240107060000.py
+-rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240222160000.py
+-rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240223050000.py
+-rw-r--r--   0        0        0      847 2024-03-03 22:43:17.403437 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240303190000.py
+-rw-r--r--   0        0        0     1110 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240408180000.py
+-rw-r--r--   0        0        0     1745 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240426050000.py
+-rw-r--r--   0        0        0     1052 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240501030000.py
+-rw-r--r--   0        0        0     1974 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/migrations/__init__.py
+-rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.2.7/src/pygpt_net/migrations/base.py
+-rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.7/src/pygpt_net/plugin/__init__.py
+-rwxr-xr-x   0        0        0    15161 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/plugin/agent/__init__.py
+-rwxr-xr-x   0        0        0    23567 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/plugin/audio_input/__init__.py
+-rw-r--r--   0        0        0     4669 2024-04-24 23:37:32.612565 pygpt_net-2.2.7/src/pygpt_net/plugin/audio_input/simple.py
+-rwxr-xr-x   0        0        0    10466 2024-03-19 09:04:41.054930 pygpt_net-2.2.7/src/pygpt_net/plugin/audio_input/worker.py
+-rwxr-xr-x   0        0        0     6940 2024-03-10 10:31:05.897000 pygpt_net-2.2.7/src/pygpt_net/plugin/audio_output/__init__.py
+-rw-r--r--   0        0        0     1806 2024-03-10 10:31:05.897000 pygpt_net-2.2.7/src/pygpt_net/plugin/audio_output/worker.py
+-rwxr-xr-x   0        0        0    12704 2024-03-18 04:54:07.637826 pygpt_net-2.2.7/src/pygpt_net/plugin/base.py
+-rwxr-xr-x   0        0        0    11734 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_api/__init__.py
+-rw-r--r--   0        0        0     6243 2024-03-16 12:28:31.211383 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_api/worker.py
+-rwxr-xr-x   0        0        0     9571 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    14580 2024-04-28 01:03:40.864507 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
+-rw-r--r--   0        0        0     8841 2024-04-28 01:03:50.072481 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
+-rwxr-xr-x   0        0        0     5875 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_custom/__init__.py
+-rw-r--r--   0        0        0     4507 2024-03-16 12:28:31.211383 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_custom/worker.py
+-rwxr-xr-x   0        0        0    17031 2024-04-25 01:16:54.112014 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_files/__init__.py
+-rwxr-xr-x   0        0        0    37969 2024-04-25 01:16:54.112014 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_files/worker.py
+-rwxr-xr-x   0        0        0    20404 2024-04-30 16:41:29.975888 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_history/__init__.py
+-rw-r--r--   0        0        0     6768 2024-04-30 16:41:29.975888 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_history/worker.py
+-rwxr-xr-x   0        0        0     6124 2024-03-16 12:28:31.211383 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_serial/__init__.py
+-rw-r--r--   0        0        0     8562 2024-03-16 12:28:31.211383 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_serial/worker.py
+-rwxr-xr-x   0        0        0    21060 2024-03-17 14:26:02.923314 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_web/__init__.py
+-rwxr-xr-x   0        0        0    12772 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_web/websearch.py
+-rw-r--r--   0        0        0    10794 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_web/worker.py
+-rwxr-xr-x   0        0        0     8163 2024-03-15 15:31:21.786121 pygpt_net-2.2.7/src/pygpt_net/plugin/crontab/__init__.py
+-rwxr-xr-x   0        0        0     2455 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/plugin/experts/__init__.py
+-rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.2.7/src/pygpt_net/plugin/extra_prompt/__init__.py
+-rwxr-xr-x   0        0        0    14776 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/plugin/idx_llama_index/__init__.py
+-rw-r--r--   0        0        0     2825 2024-03-16 16:19:22.432875 pygpt_net-2.2.7/src/pygpt_net/plugin/idx_llama_index/worker.py
+-rwxr-xr-x   0        0        0     6579 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/plugin/openai_dalle/__init__.py
+-rwxr-xr-x   0        0        0    11659 2024-04-11 20:50:24.193030 pygpt_net-2.2.7/src/pygpt_net/plugin/openai_vision/__init__.py
+-rwxr-xr-x   0        0        0     3865 2024-03-17 13:18:45.662349 pygpt_net-2.2.7/src/pygpt_net/plugin/real_time/__init__.py
+-rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.7/src/pygpt_net/provider/__init__.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/__init__.py
+-rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/base.py
+-rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
+-rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
+-rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/google_speech_recognition.py
+-rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/openai_whisper.py
+-rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/openai_whisper_local.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/__init__.py
+-rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/base.py
+-rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/eleven_labs.py
+-rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/google_tts.py
+-rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/ms_azure_tts.py
+-rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/openai_tts.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/__init__.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant/__init__.py
+-rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant/base.py
+-rw-r--r--   0        0        0     6399 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant/json_file.py
+-rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/base.py
+-rw-r--r--   0        0        0     5363 2024-04-29 15:13:32.575517 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py
+-rw-r--r--   0        0        0    10845 2024-04-29 15:13:32.575517 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py
+-rw-r--r--   0        0        0     1796 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py
+-rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/__init__.py
+-rw-r--r--   0        0        0     1314 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/base.py
+-rw-r--r--   0        0        0     3557 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py
+-rw-r--r--   0        0        0     7438 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py
+-rw-r--r--   0        0        0     2120 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py
+-rw-r--r--   0        0        0     4377 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/attachment/__init__.py
+-rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/attachment/base.py
+-rw-r--r--   0        0        0     5404 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/provider/core/attachment/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/__init__.py
+-rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/base.py
+-rw-r--r--   0        0        0     3953 2024-03-08 00:36:17.343108 pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
+-rw-r--r--   0        0        0    11113 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/config/__init__.py
+-rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/config/base.py
+-rwxr-xr-x   0        0        0     5017 2024-04-11 01:27:21.134184 pygpt_net-2.2.7/src/pygpt_net/provider/core/config/json_file.py
+-rwxr-xr-x   0        0        0    76707 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/core/config/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/__init__.py
+-rw-r--r--   0        0        0     2577 2024-04-17 05:13:33.075416 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/base.py
+-rw-r--r--   0        0        0     9648 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
+-rw-r--r--   0        0        0    33381 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
+-rw-r--r--   0        0        0     7644 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
+-rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/history/__init__.py
+-rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/history/base.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/history/patch.py
+-rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/history/txt_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/__init__.py
+-rw-r--r--   0        0        0     2875 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/base.py
+-rw-r--r--   0        0        0     8502 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/patch.py
+-rw-r--r--   0        0        0    17470 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/storage.py
+-rw-r--r--   0        0        0      934 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/utils.py
+-rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/index/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/__init__.py
+-rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/base.py
+-rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/model/__init__.py
+-rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/model/base.py
+-rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/model/json_file.py
+-rw-r--r--   0        0        0    10462 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/core/model/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/__init__.py
+-rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/base.py
+-rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
+-rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
+-rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/json_file.py
+-rw-r--r--   0        0        0      488 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/__init__.py
+-rw-r--r--   0        0        0      987 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/base.py
+-rwxr-xr-x   0        0        0     3198 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/json_file.py
+-rwxr-xr-x   0        0        0     1766 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/patch.py
+-rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/__init__.py
+-rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/base.py
+-rwxr-xr-x   0        0        0     8307 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/json_file.py
+-rw-r--r--   0        0        0     4651 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/patch.py
+-rw-r--r--   0        0        0     7297 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/__init__.py
+-rw-r--r--   0        0        0    13637 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/assistants.py
+-rw-r--r--   0        0        0     7034 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/chat.py
+-rw-r--r--   0        0        0     5876 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/completion.py
+-rw-r--r--   0        0        0     8255 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/image.py
+-rw-r--r--   0        0        0    16810 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/store.py
+-rw-r--r--   0        0        0     2072 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/summarizer.py
+-rw-r--r--   0        0        0     8266 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/vision.py
+-rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/worker/__init__.py
+-rw-r--r--   0        0        0    20403 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/worker/assistants.py
+-rw-r--r--   0        0        0    15467 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/provider/gpt/worker/importer.py
+-rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/provider/llms/__init__.py
+-rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/provider/llms/anthropic.py
+-rwxr-xr-x   0        0        0     2800 2024-03-13 15:08:01.569797 pygpt_net-2.2.7/src/pygpt_net/provider/llms/azure_openai.py
+-rw-r--r--   0        0        0     3940 2024-03-15 15:31:21.790122 pygpt_net-2.2.7/src/pygpt_net/provider/llms/base.py
+-rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/provider/llms/hugging_face.py
+-rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/provider/llms/llama.py
+-rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/provider/llms/ollama.py
+-rwxr-xr-x   0        0        0     2727 2024-03-13 15:08:01.569797 pygpt_net-2.2.7/src/pygpt_net/provider/llms/openai.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/__init__.py
+-rw-r--r--   0        0        0     2515 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/base.py
+-rw-r--r--   0        0        0     1258 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_csv.py
+-rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_docx.py
+-rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_epub.py
+-rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_excel.py
+-rw-r--r--   0        0        0     1268 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_html.py
+-rw-r--r--   0        0        0     1923 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_image_vision.py
+-rw-r--r--   0        0        0     1284 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_ipynb.py
+-rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_json.py
+-rw-r--r--   0        0        0     1292 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_markdown.py
+-rw-r--r--   0        0        0     1214 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_pdf.py
+-rw-r--r--   0        0        0     1832 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_video_audio.py
+-rw-r--r--   0        0        0     1196 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_xml.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
+-rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
+-rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/database/__init__.py
+-rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/database/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/github/__init__.py
+-rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/github/issues.py
+-rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/github/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/__init__.py
+-rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/calendar.py
+-rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/docs.py
+-rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/gmail.py
+-rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/keep.py
+-rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/sheets.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
+-rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/image_vision/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/json/__init__.py
+-rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/json/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
+-rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
+-rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
+-rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/video_audio/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
+-rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/web_page/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/yt/__init__.py
+-rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/yt/base.py
+-rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/yt/utils.py
+-rw-r--r--   0        0        0     3626 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_bitbucket.py
+-rw-r--r--   0        0        0     2580 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
+-rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_database.py
+-rw-r--r--   0        0        0     3832 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_github_issues.py
+-rw-r--r--   0        0        0     4377 2024-04-17 01:35:30.426055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_github_repo.py
+-rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_calendar.py
+-rw-r--r--   0        0        0     2480 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_docs.py
+-rw-r--r--   0        0        0     3582 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_drive.py
+-rw-r--r--   0        0        0     2710 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_gmail.py
+-rw-r--r--   0        0        0     2412 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_keep.py
+-rw-r--r--   0        0        0     2590 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_sheets.py
+-rw-r--r--   0        0        0     4004 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
+-rw-r--r--   0        0        0     1572 2024-03-12 06:49:17.168786 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_page.py
+-rw-r--r--   0        0        0     1584 2024-03-12 06:49:17.172787 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_rss.py
+-rw-r--r--   0        0        0     1853 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_sitemap.py
+-rw-r--r--   0        0        0     2831 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_twitter.py
+-rw-r--r--   0        0        0     1617 2024-03-12 06:49:17.172787 pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_yt.py
+-rw-r--r--   0        0        0     5976 2024-03-08 22:55:56.889343 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/__init__.py
+-rw-r--r--   0        0        0     3791 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/base.py
+-rwxr-xr-x   0        0        0     3036 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/chroma.py
+-rw-r--r--   0        0        0     3016 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/elasticsearch.py
+-rw-r--r--   0        0        0     5041 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/pinecode.py
+-rw-r--r--   0        0        0     3047 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/redis.py
+-rw-r--r--   0        0        0     2455 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/simple.py
+-rw-r--r--   0        0        0     4322 2024-03-11 03:15:21.875594 pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/temp.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.7/src/pygpt_net/provider/web/__init__.py
+-rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.2.7/src/pygpt_net/provider/web/base.py
+-rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.2.7/src/pygpt_net/provider/web/google_custom_search.py
+-rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.2.7/src/pygpt_net/provider/web/microsoft_bing.py
+-rw-r--r--   0        0        0     3917 2024-04-19 00:32:20.498428 pygpt_net-2.2.7/src/pygpt_net/tools/__init__.py
+-rwxr-xr-x   0        0        0     9791 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/audio_transcriber/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/audio_transcriber/ui/__init__.py
+-rw-r--r--   0        0        0     5666 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py
+-rw-r--r--   0        0        0     2116 2024-04-19 00:32:20.498428 pygpt_net-2.2.7/src/pygpt_net/tools/base.py
+-rwxr-xr-x   0        0        0    11427 2024-04-19 00:32:20.498428 pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/ui/__init__.py
+-rw-r--r--   0        0        0     6622 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/ui/dialogs.py
+-rw-r--r--   0        0        0     3518 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/ui/widgets.py
+-rwxr-xr-x   0        0        0     9063 2024-04-14 16:40:07.849541 pygpt_net-2.2.7/src/pygpt_net/tools/image_viewer/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/image_viewer/ui/__init__.py
+-rw-r--r--   0        0        0     4962 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/image_viewer/ui/dialogs.py
+-rwxr-xr-x   0        0        0    18833 2024-04-19 00:32:20.498428 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/__init__.py
+-rw-r--r--   0        0        0     1438 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/browse.py
+-rw-r--r--   0        0        0     4355 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/ctx.py
+-rw-r--r--   0        0        0     7985 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/dialogs.py
+-rw-r--r--   0        0        0     4034 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/files.py
+-rw-r--r--   0        0        0    10477 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/web.py
+-rw-r--r--   0        0        0     3562 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/widgets.py
+-rwxr-xr-x   0        0        0     6028 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/media_player/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/media_player/ui/__init__.py
+-rw-r--r--   0        0        0     3590 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/media_player/ui/dialogs.py
+-rw-r--r--   0        0        0    15702 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/media_player/ui/widgets.py
+-rw-r--r--   0        0        0     8018 2024-04-14 16:40:07.849541 pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/ui/__init__.py
+-rw-r--r--   0        0        0     2906 2024-04-11 00:43:06.922864 pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/ui/dialogs.py
+-rw-r--r--   0        0        0     2754 2024-04-11 03:43:59.058733 pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/ui/widgets.py
+-rwxr-xr-x   0        0        0     6639 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/ui/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.7/src/pygpt_net/ui/base/__init__.py
+-rw-r--r--   0        0        0     9209 2024-03-11 07:32:25.337990 pygpt_net-2.2.7/src/pygpt_net/ui/base/config_dialog.py
+-rw-r--r--   0        0        0     3430 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/ui/base/context_menu.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/__init__.py
+-rwxr-xr-x   0        0        0     5730 2024-04-11 20:50:24.193030 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/about.py
+-rwxr-xr-x   0        0        0     5140 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/applog.py
+-rwxr-xr-x   0        0        0     6480 2024-04-28 06:16:26.324027 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/assistant.py
+-rw-r--r--   0        0        0    22532 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/assistant_store.py
+-rwxr-xr-x   0        0        0     1765 2024-03-18 02:45:45.661442 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/changelog.py
+-rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/create.py
+-rw-r--r--   0        0        0    18520 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/db.py
+-rwxr-xr-x   0        0        0     1864 2024-03-18 04:54:07.637826 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/debug.py
+-rw-r--r--   0        0        0     5835 2024-03-12 06:49:17.172787 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/dictionary.py
+-rwxr-xr-x   0        0        0     2926 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/editor.py
+-rw-r--r--   0        0        0      957 2024-04-08 04:19:15.433912 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/find.py
+-rwxr-xr-x   0        0        0     2876 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/image.py
+-rwxr-xr-x   0        0        0     2272 2024-03-18 02:45:42.817463 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/license.py
+-rwxr-xr-x   0        0        0     1823 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/logger.py
+-rw-r--r--   0        0        0    13166 2024-03-10 12:05:00.639613 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/models.py
+-rwxr-xr-x   0        0        0    20679 2024-03-12 06:49:17.172787 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/plugins.py
+-rwxr-xr-x   0        0        0     7391 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/preset.py
+-rw-r--r--   0        0        0     3796 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/preset_plugins.py
+-rw-r--r--   0        0        0     4105 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/profile.py
+-rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/rename.py
+-rwxr-xr-x   0        0        0    15113 2024-03-10 12:05:00.639613 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/settings.py
+-rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/snap.py
+-rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/start.py
+-rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/update.py
+-rw-r--r--   0        0        0     4275 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/ui/dialog/workdir.py
+-rwxr-xr-x   0        0        0     9009 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/ui/dialogs.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/layout/__init__.py
+-rwxr-xr-x   0        0        0     1535 2024-04-09 20:34:52.308546 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/__init__.py
+-rwxr-xr-x   0        0        0     5518 2024-04-14 20:50:29.556142 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/attachments.py
+-rwxr-xr-x   0        0        0     5280 2024-04-29 15:13:32.575517 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
+-rw-r--r--   0        0        0     5996 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/calendar.py
+-rwxr-xr-x   0        0        0     9885 2024-04-09 20:35:55.668463 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/input.py
+-rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/markdown.py
+-rwxr-xr-x   0        0        0    10452 2024-04-21 18:06:27.128064 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/output.py
+-rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/painter.py
+-rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/__init__.py
+-rwxr-xr-x   0        0        0     6648 2024-04-21 19:42:04.971470 pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/ctx_list.py
+-rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/search_input.py
+-rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/video.py
+-rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.2.7/src/pygpt_net/ui/layout/status.py
+-rwxr-xr-x   0        0        0     3477 2024-04-27 14:05:11.727541 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/__init__.py
+-rw-r--r--   0        0        0     2378 2024-01-30 17:23:19.901578 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/agent.py
+-rwxr-xr-x   0        0        0     4436 2024-04-30 02:35:43.578880 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/assistants.py
+-rwxr-xr-x   0        0        0     4254 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/footer.py
+-rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/image.py
+-rw-r--r--   0        0        0     7007 2024-04-30 16:41:29.979888 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/indexes.py
+-rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/mode.py
+-rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/model.py
+-rwxr-xr-x   0        0        0     5109 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/presets.py
+-rwxr-xr-x   0        0        0     3242 2024-03-15 15:31:21.790122 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/prompt.py
+-rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/vision.py
+-rw-r--r--   0        0        0     9644 2024-04-29 05:51:11.644212 pygpt_net-2.2.7/src/pygpt_net/ui/main.py
+-rw-r--r--   0        0        0     1784 2024-03-26 17:12:51.294309 pygpt_net-2.2.7/src/pygpt_net/ui/menu/__init__.py
+-rw-r--r--   0        0        0     5067 2024-04-19 00:32:20.498428 pygpt_net-2.2.7/src/pygpt_net/ui/menu/about.py
+-rw-r--r--   0        0        0     1655 2024-03-20 16:01:43.283339 pygpt_net-2.2.7/src/pygpt_net/ui/menu/audio.py
+-rw-r--r--   0        0        0     7870 2024-04-21 01:33:54.247764 pygpt_net-2.2.7/src/pygpt_net/ui/menu/config.py
+-rw-r--r--   0        0        0     5185 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/ui/menu/debug.py
+-rw-r--r--   0        0        0     3356 2024-04-17 05:13:33.075416 pygpt_net-2.2.7/src/pygpt_net/ui/menu/file.py
+-rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/ui/menu/lang.py
+-rw-r--r--   0        0        0     2880 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/ui/menu/plugins.py
+-rwxr-xr-x   0        0        0     3440 2024-04-24 23:37:32.616565 pygpt_net-2.2.7/src/pygpt_net/ui/menu/theme.py
+-rw-r--r--   0        0        0     1134 2024-03-26 17:12:51.298308 pygpt_net-2.2.7/src/pygpt_net/ui/menu/tools.py
+-rw-r--r--   0        0        0     2026 2024-03-20 16:01:43.283339 pygpt_net-2.2.7/src/pygpt_net/ui/menu/video.py
+-rw-r--r--   0        0        0     6711 2024-04-14 20:50:29.556142 pygpt_net-2.2.7/src/pygpt_net/ui/tray.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.7/src/pygpt_net/ui/widget/__init__.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/__init__.py
+-rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/input.py
+-rw-r--r--   0        0        0     2198 2024-02-29 03:07:51.278132 pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/input_button.py
+-rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/output.py
+-rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.2.7/src/pygpt_net/ui/widget/calendar/__init__.py
+-rw-r--r--   0        0        0     8120 2024-04-27 07:58:32.754704 pygpt_net-2.2.7/src/pygpt_net/ui/widget/calendar/select.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/__init__.py
+-rwxr-xr-x   0        0        0     1429 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/alert.py
+-rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/applog.py
+-rw-r--r--   0        0        0     1712 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/assistant_store.py
+-rw-r--r--   0        0        0      551 2024-03-26 17:12:51.298308 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/audio.py
+-rwxr-xr-x   0        0        0     3802 2024-04-11 03:43:59.058733 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/base.py
+-rwxr-xr-x   0        0        0     2302 2024-04-12 10:08:45.275113 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/confirm.py
+-rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/create.py
+-rw-r--r--   0        0        0     1585 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/db.py
+-rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/debug.py
+-rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/editor.py
+-rwxr-xr-x   0        0        0     6185 2024-04-14 16:40:07.849541 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/editor_file.py
+-rw-r--r--   0        0        0     3242 2024-04-11 03:43:59.058733 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/find.py
+-rwxr-xr-x   0        0        0      816 2024-03-26 17:12:51.298308 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/image.py
+-rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/info.py
+-rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/license.py
+-rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/logger.py
+-rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/model.py
+-rw-r--r--   0        0        0     1694 2024-04-10 01:07:30.188635 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/preset_plugins.py
+-rw-r--r--   0        0        0     6686 2024-04-19 00:32:20.502428 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/profile.py
+-rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/rename.py
+-rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/settings.py
+-rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/settings_plugin.py
+-rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/snap.py
+-rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/update.py
+-rw-r--r--   0        0        0     1523 2024-03-26 17:12:51.298308 pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/workdir.py
+-rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.2.7/src/pygpt_net/ui/widget/draw/__init__.py
+-rw-r--r--   0        0        0    10903 2024-04-12 07:23:35.946682 pygpt_net-2.2.7/src/pygpt_net/ui/widget/draw/painter.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/__init__.py
+-rw-r--r--   0        0        0     4173 2024-04-29 15:13:32.575517 pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/button.py
+-rw-r--r--   0        0        0     2532 2024-03-07 01:04:26.445956 pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/checkbox.py
+-rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/group.py
+-rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/labels.py
+-rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/filesystem/__init__.py
+-rwxr-xr-x   0        0        0    22934 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/ui/widget/filesystem/explorer.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/image/__init__.py
+-rwxr-xr-x   0        0        0     3797 2024-03-26 17:12:51.298308 pygpt_net-2.2.7/src/pygpt_net/ui/widget/image/display.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/__init__.py
+-rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/assistant.py
+-rw-r--r--   0        0        0     3715 2024-04-29 15:13:32.575517 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/assistant_store.py
+-rwxr-xr-x   0        0        0     7055 2024-04-14 20:50:29.556142 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/attachment.py
+-rwxr-xr-x   0        0        0     2435 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/base.py
+-rwxr-xr-x   0        0        0    17502 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/context.py
+-rw-r--r--   0        0        0     5861 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/db.py
+-rw-r--r--   0        0        0     3658 2024-03-07 01:04:26.449956 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/debug.py
+-rw-r--r--   0        0        0     5739 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/experts.py
+-rw-r--r--   0        0        0     4818 2024-04-17 01:35:30.430055 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/index.py
+-rw-r--r--   0        0        0     6794 2024-04-27 14:05:11.727541 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/index_combo.py
+-rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/mode.py
+-rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/model.py
+-rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/model_editor.py
+-rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/plugin.py
+-rwxr-xr-x   0        0        0     5655 2024-05-01 18:08:40.482948 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/preset.py
+-rw-r--r--   0        0        0     3899 2024-03-07 01:04:26.449956 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/preset_plugins.py
+-rw-r--r--   0        0        0     4432 2024-04-10 01:07:30.192635 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/profile.py
+-rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/settings.py
+-rwxr-xr-x   0        0        0     4382 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/uploaded.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/__init__.py
+-rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/checkbox.py
+-rw-r--r--   0        0        0     5503 2024-03-12 06:49:17.172787 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/cmd.py
+-rw-r--r--   0        0        0     3592 2024-04-27 10:44:46.049374 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/combo.py
+-rwxr-xr-x   0        0        0    12672 2024-03-11 03:15:21.879593 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/dictionary.py
+-rwxr-xr-x   0        0        0     9304 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/input.py
+-rw-r--r--   0        0        0     2601 2024-04-22 22:35:26.800429 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/prompt.py
+-rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/slider.py
+-rwxr-xr-x   0        0        0     2684 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/textarea.py
+-rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.2.7/src/pygpt_net/ui/widget/tabs/Input.py
+-rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.2.7/src/pygpt_net/ui/widget/tabs/__init__.py
+-rw-r--r--   0        0        0     2814 2024-04-10 01:07:30.192635 pygpt_net-2.2.7/src/pygpt_net/ui/widget/tabs/output.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/__init__.py
+-rw-r--r--   0        0        0     5098 2024-04-21 01:33:54.247764 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/calendar_note.py
+-rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/create.py
+-rw-r--r--   0        0        0     5450 2024-04-21 01:33:54.247764 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/editor.py
+-rw-r--r--   0        0        0     1543 2024-04-11 03:43:59.058733 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/find.py
+-rwxr-xr-x   0        0        0     6059 2024-04-22 22:35:26.800429 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/input.py
+-rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/name.py
+-rwxr-xr-x   0        0        0     6583 2024-04-21 01:33:54.247764 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/notepad.py
+-rwxr-xr-x   0        0        0     5086 2024-04-23 23:11:13.260159 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/output.py
+-rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/rename.py
+-rwxr-xr-x   0        0        0     1833 2024-04-12 10:08:45.275113 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/search_input.py
+-rwxr-xr-x   0        0        0    10060 2024-04-27 14:05:11.727541 pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/web.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/vision/__init__.py
+-rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.2.7/src/pygpt_net/ui/widget/vision/camera.py
+-rwxr-xr-x   0        0        0     5470 2024-04-26 21:55:50.679597 pygpt_net-2.2.7/src/pygpt_net/utils.py
+-rw-r--r--   0        0        0   139995 1970-01-01 00:00:00.000000 pygpt_net-2.2.7/PKG-INFO
```

### Comparing `pygpt_net-2.2.6/CHANGELOG.md` & `pygpt_net-2.2.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # CHANGELOG
 
+# 2.2.7 (2024-05-01)
+
+- A new experimental work mode has been added: 'Experts', which allows the creation of separate background instances with their own instructions that can be consulted for help. See the documentation: 'Work Modes / Experts'.
+- Added a new plugin: 'Experts (inline)`.
+- Improved the Agent mode by adding the ability to configure and invoke defined Experts.
+- Improved the prompts that control the autonomous mode.
+- The main prompt controlling the agents has been moved from presets to the application's settings window.
+
 # 2.2.6 (2024-04-30)
 
 - Added a new model: 'gpt-4-turbo'.
 - Vision integrated into Chat mode, without any plugins, if the model supports Vision - currently available for: 'gpt-4-turbo' and 'gpt-4-turbo-2024-04-09'.
 - Store importer connected with Logger.
 - Fixed: issue with batch unassigning remote files from vector stores.
```

### Comparing `pygpt_net-2.2.6/LICENSE` & `pygpt_net-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/README.md` & `pygpt_net-2.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PyGPT - Desktop AI Assistant
 
 [![pygpt](https://snapcraft.io/pygpt/badge.svg)](https://snapcraft.io/pygpt)
 
-Release: **2.2.6** | build: **2024.04.30** | Python: **>=3.10, <3.12**
+Release: **2.2.7** | build: **2024.05.01** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -32,15 +32,15 @@
 
 You can download compiled 64-bit versions for Windows and Linux here: https://pygpt.net/#download
 
 ## Features
 
 - Desktop AI Assistant for `Linux`, `Windows` and `Mac`, written in Python.
 - Works similarly to `ChatGPT`, but locally (on a desktop computer).
-- 8 modes of operation: Chat, Vision, Completion, Assistant, Image generation, Langchain, Chat with files and Agent (autonomous).
+- 9 modes of operation: Chat, Vision, Completion, Assistant, Image generation, Langchain, Chat with files, Experts and Agent (autonomous).
 - Supports multiple models: `GPT-4`, `GPT-3.5`, and any model accessible through `Langchain`.
 - Handles and stores the full context of conversations (short-term memory).
 - Real-time video camera capture in Vision mode.
 - Internet access via `Google` and `Microsoft Bing`.
 - Speech synthesis via `Microsoft Azure`, `Google`, `Eleven Labs` and `OpenAI` Text-To-Speech services.
 - Speech recognition via `OpenAI Whisper`, `Google`, `Google Cloud` and `Microsoft Bing`.
 - Image analysis via `GPT-4 Vision`.
@@ -788,17 +788,17 @@
 **Twitter/X posts**  (web_twitter)
 
 - `bearer_token` - str, default: `None`
 - `num_tweets` - int, default: `100`
 
 ##  Agent (autonomous) 
 
-This mode is experimental.
+**This mode is experimental.**
 
-**WARNING: Please use this mode with caution!** - autonomous mode, when connected with other plugins, may produce unexpected results!
+**WARNING: Please use this mode with caution** - autonomous mode, when connected with other plugins, may produce unexpected results!
 
 The mode activates autonomous mode, where AI begins a conversation with itself. 
 You can set this loop to run for any number of iterations. Throughout this sequence, the model will engage
 in self-dialogue, answering his own questions and comments, in order to find the best possible solution, subjecting previously generated steps to criticism.
 
 ![v2_agent_toolbox](https://github.com/szczyglis-dev/py-gpt/assets/61396542/a0ae5d13-942e-4a18-9c53-33e7ad1886ff)
 
@@ -826,14 +826,47 @@
 If you want to use the Llama-index mode when running the agent, you can also specify which index `Llama-index` should use with the option:
 
 ```Settings / Agent (autonomous) / Index to use```
 
 ![v2_agent_settings](https://github.com/szczyglis-dev/py-gpt/assets/61396542/c577d219-eb25-4f0e-9ea5-adf20a6b6b81)
 
 
+##  Experts (co-op, co-operation mode)
+
+Added in version 2.2.7 (2024-05-01).
+
+**This mode is experimental.**
+
+Expert mode allows for the creation of experts (using presets) and then consulting them during a conversation. In this mode, a primary base context is created for conducting the conversation. From within this context, the model can make requests to an expert to perform a task and return the results to the main thread. When an expert is called in the background, a separate context is created for them with their own memory. This means that each expert, during the life of one main context, also has access to their own memory via their separate, isolated context.
+
+**In simple terms - you can imagine an expert as a separate, additional instance of the model running in the background, which can be called at any moment for assistance, with its own context and memory, as well as its own specialized instructions in a given subject.**
+
+Experts do not share contexts with one another, and the only point of contact between them is the main conversation thread. In this main thread, the model acts as a manager of experts, who can exchange data between them as needed.
+
+An expert is selected based on the name in the presets; for example, naming your expert as: ID = python_expert, name = "Python programmer" will create an expert whom the model will attempt to invoke for matters related to Python programming. You can also manually request to refer to a given expert:
+
+```bash
+Call the Python expert to generate some code.
+```
+
+Experts can be activated or deactivated - to enable or disable use RMB context menu to select the `Enable/Disable` options from the presets list. Only enabled experts are available to use in the thread.
+
+Experts can also be used in `Agent (autonomous)` mode - by creating a new agent using a preset. Simply move the appropriate experts to the active list to automatically make them available for use by the agent.
+
+You can also use experts in "inline" mode - by activating the `Experts (inline)` plugin. This allows for the use of experts in any mode, such as normal chat.
+
+Expert mode, like agent mode, is a "virtual" mode - you need to select a target mode of operation for it, which can be done in the settings at `Settings / Agent (autonomous) / Sub-mode for experts`.
+
+You can also ask for a list of active experts at any time:
+
+```bash
+Give me a list of active experts.
+```
+
+
 # Files and attachments
 
 ## Input attachments (upload)
 
 **PyGPT** makes it simple for users to upload files to the server and send them to the model for tasks like analysis, similar to attaching files in `ChatGPT`. There's a separate `Files` tab next to the text input area specifically for managing file uploads. Users can opt to have files automatically deleted after each upload or keep them on the list for repeated use.
 
 ![v2_file_input](https://github.com/szczyglis-dev/py-gpt/assets/61396542/bd3d9840-2bc4-4ba8-a603-69724f9eb620)
@@ -2763,18 +2796,22 @@
 
 - `Command execute: extra footer (Assistant mode only)`: PAdditional instructions to separate local commands from the remote environment that is already configured in the Assistants.
 
 - `Context: auto-summary (system prompt)`: System prompt for context auto-summary.
 
 - `Context: auto-summary (user message)`: User message for context auto-summary. Placeholders: {input}, {output}
 
-- `Agent: continue`: Prompt sent to automatically continue the conversation. Default: `continue...`
+- `Agent: system instruction`: Prompt to instruct how to handle autonomous mode.
+
+- `Agent: continue`: Prompt sent to automatically continue the conversation.
 
 - `Agent: goal update`: Prompt to instruct how to update current goal status.
 
+- `Experts: Master prompt`: Prompt to instruct how to handle experts.
+
 - `DALL-E: image generate`: Prompt for generating prompts for DALL-E (if raw-mode is disabled).
 
 **Images**
 
 - `DALL-E Image size`: The resolution of the generated images (DALL-E). Default: 1792x1024.
 
 - `DALL-E Image quality`: The image quality of the generated images (DALL-E). Default: standard.
@@ -2833,14 +2870,16 @@
 
 - `DB (ALL), DB (UPDATE), FILES (ALL)`: Index the data – batch indexing is available here.
 
 **Agent (autonomous)**
 
 - `Sub-mode to use`: Sub-mode to use in Agent mode (chat, completion, langchain, llama_index, etc.). Default: chat.
 
+- `Sub-mode for experts`: Sub-mode to use in Experts mode (chat, completion, langchain, llama_index, etc.). Default: chat.
+
 - `Index to use`: Only if sub-mode is llama_index (Chat with files), choose the index to use in Agent mode.
 
 - `Display a tray notification when the goal is achieved.`: If enabled, a notification will be displayed after goal achieved / finished run.
 
 **Updates**
 
 - `Check for updates on start`: Enables checking for updates on start. Default: True.
@@ -3056,14 +3095,22 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+**2.2.7 (2024-05-01)**
+
+- A new experimental work mode has been added: 'Experts', which allows the creation of separate background instances with their own instructions that can be consulted for help. See the documentation: 'Work Modes / Experts'.
+- Added a new plugin: 'Experts (inline)`.
+- Improved the Agent mode by adding the ability to configure and invoke defined Experts.
+- Improved the prompts that control the autonomous mode.
+- The main prompt controlling the agents has been moved from presets to the application's settings window.
+
 **2.2.6 (2024-04-30)**
 
 - Added a new model: 'gpt-4-turbo'.
 - Vision integrated into Chat mode, without any plugins, if the model supports Vision - currently available for: 'gpt-4-turbo' and 'gpt-4-turbo-2024-04-09'.
 - Store importer connected with Logger.
 - Fixed: issue with batch unassigning remote files from vector stores.
```

### Comparing `pygpt_net-2.2.6/icon.png` & `pygpt_net-2.2.7/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/pyproject.toml` & `pygpt_net-2.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygpt-net"
-version = "2.2.6"
+version = "2.2.7"
 description = "Desktop AI Assistant powered by GPT-4, GPT-4V, GPT-3.5, DALL-E 3, Langchain LLMs, Llama-index, Whisper with chatbot, assistant, text completion, vision and image generation, internet access, chat with files, commands and code execution, file upload and download and more"
 authors = ["Marcin Szczyglinski <info@pygpt.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/szczyglis-dev/py-gpt"
 repository = "https://github.com/szczyglis-dev/py-gpt"
 documentation = "https://pygpt.readthedocs.io/"
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/CHANGELOG.txt` & `pygpt_net-2.2.7/src/pygpt_net/CHANGELOG.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+2.2.7 (2024-05-01)
+
+- A new experimental work mode has been added: 'Experts', which allows the creation of separate background instances with their own instructions that can be consulted for help. See the documentation: 'Work Modes / Experts'.
+- Added a new plugin: 'Experts (inline)`.
+- Improved the Agent mode by adding the ability to configure and invoke defined Experts.
+- Improved the prompts that control the autonomous mode.
+- The main prompt controlling the agents has been moved from presets to the application's settings window.
+
 2.2.6 (2024-04-30)
 
 - Added a new model: 'gpt-4-turbo'.
 - Vision integrated into Chat mode, without any plugins, if the model supports Vision - currently available for: 'gpt-4-turbo' and 'gpt-4-turbo-2024-04-09'.
 - Store importer connected with Logger.
 - Fixed: issue with batch unassigning remote files from vector stores.
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/LICENSE` & `pygpt_net-2.2.7/src/pygpt_net/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 18:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 __author__ = "Marcin Szczygliński"
 __copyright__ = "Copyright 2024, Marcin Szczygliński"
 __credits__ = ["Marcin Szczygliński"]
 __license__ = "MIT"
-__version__ = "2.2.6"
-__build__ = "2024.04.30"
+__version__ = "2.2.7"
+__build__ = "2024.05.01"
 __maintainer__ = "Marcin Szczygliński"
 __github__ = "https://github.com/szczyglis-dev/py-gpt"
 __website__ = "https://pygpt.net"
 __pypi__ = "https://pypi.org/project/pygpt-net"
 __snap__ = "https://snapcraft.io/pygpt"
 __donate__ = "https://pygpt.net/#donate"
 __documentation__ = "https://pygpt.readthedocs.io"
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/app.py` & `pygpt_net-2.2.7/src/pygpt_net/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.17 01:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 from pygpt_net.launcher import Launcher
 
 # plugins
 from pygpt_net.plugin.audio_output import Plugin as AudioOutputPlugin
 from pygpt_net.plugin.audio_input import Plugin as AudioInputPlugin
@@ -19,14 +19,15 @@
 from pygpt_net.plugin.cmd_custom import Plugin as CmdCustomCommandPlugin
 from pygpt_net.plugin.cmd_files import Plugin as CmdFilesPlugin
 from pygpt_net.plugin.cmd_history import Plugin as CtxHistoryPlugin
 from pygpt_net.plugin.cmd_serial import Plugin as CmdSerialPlugin
 from pygpt_net.plugin.cmd_web import Plugin as CmdWebPlugin
 from pygpt_net.plugin.crontab import Plugin as CrontabPlugin
 from pygpt_net.plugin.extra_prompt import Plugin as ExtraPromptPlugin
+from pygpt_net.plugin.experts import Plugin as ExpertsPlugin
 from pygpt_net.plugin.idx_llama_index import Plugin as IdxLlamaIndexPlugin
 from pygpt_net.plugin.openai_dalle import Plugin as OpenAIDallePlugin
 from pygpt_net.plugin.openai_vision import Plugin as OpenAIVisionPlugin
 from pygpt_net.plugin.real_time import Plugin as RealTimePlugin
 from pygpt_net.plugin.agent import Plugin as AgentPlugin
 
 # LLM wrapper providers (langchain, llama-index, embeddings)
@@ -279,14 +280,15 @@
     if isinstance(loaders, list):
         for loader in loaders:
             launcher.add_loader(loader)
 
     # register base plugins
     launcher.add_plugin(AgentPlugin())
     launcher.add_plugin(RealTimePlugin())
+    launcher.add_plugin(ExpertsPlugin())
     launcher.add_plugin(ExtraPromptPlugin())
     launcher.add_plugin(AudioInputPlugin())
     launcher.add_plugin(AudioOutputPlugin())
     launcher.add_plugin(CmdWebPlugin())
     launcher.add_plugin(CmdFilesPlugin())
     launcher.add_plugin(CmdCodeInterpreterPlugin())
     launcher.add_plugin(CmdCustomCommandPlugin())
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/config.py` & `pygpt_net-2.2.7/src/pygpt_net/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/container.py` & `pygpt_net-2.2.7/src/pygpt_net/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 07:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 from pygpt_net.config import Config
 from pygpt_net.core.assistants import Assistants
 from pygpt_net.core.attachments import Attachments
 from pygpt_net.core.audio import Audio
 from pygpt_net.core.bridge import Bridge
@@ -18,14 +18,15 @@
 from pygpt_net.core.camera import Camera
 from pygpt_net.core.chain import Chain
 from pygpt_net.core.command import Command
 from pygpt_net.core.ctx import Ctx
 from pygpt_net.core.db import Database
 from pygpt_net.core.debug import Debug
 from pygpt_net.core.dispatcher import Dispatcher
+from pygpt_net.core.experts import Experts
 from pygpt_net.core.idx import Idx
 from pygpt_net.core.installer import Installer
 from pygpt_net.core.filesystem import Filesystem
 from pygpt_net.core.history import History
 from pygpt_net.core.image import Image
 from pygpt_net.core.llm import LLM
 from pygpt_net.core.models import Models
@@ -61,14 +62,15 @@
         self.chain = Chain(window)
         self.command = Command(window)
         self.config = Config(window)
         self.ctx = Ctx(window)
         self.db = Database(window)
         self.debug = Debug(window)
         self.dispatcher = Dispatcher(window)
+        self.experts = Experts(window)
         self.filesystem = Filesystem(window)
         self.gpt = Gpt(window)
         self.history = History(window)
         self.idx = Idx(window)
         self.image = Image(window)
         self.llm = LLM(window)
         self.installer = Installer(window)
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/agent/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/agent/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.02.25 06:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
+from .experts import Experts
 from .flow import Flow
 
 
 class Agent:
     def __init__(self, window=None):
         """
         Agent controller
 
         :param window: Window instance
         """
         self.window = window
+        self.experts = Experts(window)
         self.flow = Flow(window)
         self.options = {
             "agent.iterations": {
                 "type": "int",
                 "slider": True,
                 "label": "agent.iterations",
                 "min": 0,
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/agent/flow.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/agent/flow.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/assistant/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/assistant/batch.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/assistant/batch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/assistant/editor.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/assistant/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/assistant/files.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/assistant/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/assistant/store.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/assistant/store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/assistant/threads.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/assistant/threads.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/attachment.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/audio/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/calendar/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/calendar/note.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/calendar/note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/camera.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/chat/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/chat/common.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/chat/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 07:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import os
 
 from PySide6.QtGui import QTextCursor
 from PySide6.QtWidgets import QFileDialog
 
@@ -195,14 +195,15 @@
         event = Event(Event.FORCE_STOP, {
             "value": True,
         })
         self.window.core.dispatcher.dispatch(event)  # stop event
         event = Event(Event.AUDIO_INPUT_TOGGLE, {
             "value": False,
         })
+        self.window.controller.agent.experts.stop()
         self.window.controller.agent.flow.on_stop()
         self.window.controller.assistant.threads.stop = True
         self.window.controller.assistant.threads.reset()  # reset run and func calls
         self.window.core.dispatcher.dispatch(event)  # stop audio input
         self.window.controller.chat.input.stop = True
         self.window.core.gpt.stop()
         self.unlock_input()
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/chat/files.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/chat/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/chat/image.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/chat/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 from PySide6.QtWidgets import  QApplication
 
 from pygpt_net.core.bridge import BridgeContext
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.core.dispatcher import Event
@@ -25,21 +25,23 @@
         :param window: Window instance
         """
         self.window = window
 
     def send(
             self,
             text: str,
-            prev_ctx: CtxItem = None
+            prev_ctx: CtxItem = None,
+            parent_id: int = None,
     ) -> CtxItem:
         """
         Send prompt for image generate
 
         :param text: prompt for image generation
         :param prev_ctx: previous ctx item
+        :param parent_id: parent ctx id
         :return: ctx item
         """
         num = int(self.window.ui.config['global']['img_variants'].input.text() or 1)
         if num < 1:
             num = 1
         elif num > 4:
             num = 4
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/chat/input.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/chat/input.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.15 10:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 from PySide6.QtWidgets import QApplication
 
 from pygpt_net.core.dispatcher import Event
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.utils import trans
@@ -27,28 +27,31 @@
         self.locked = False
         self.stop = False
         self.generating = False
         self.no_api_key_allowed = [
             "langchain",
             "llama_index",
             "agent",
+            "expert",
         ]
         self.no_ctx_idx_modes = [
             # "img",
             "assistant",
             # "llama_index",
             "agent",
         ]  # assistant is handled in async, agent is handled in agent flow
 
     def send_input(self, force: bool = False):
         """
         Send text from user input (called from UI)
 
         :param force: force send
         """
+        self.window.controller.agent.experts.unlock()  # unlock experts
+
         # check if not in edit mode
         if not force and self.window.controller.ctx.extra.is_editing():
             self.window.controller.ctx.extra.edit_submit()
             return
 
         # get text from input
         text = self.window.ui.nodes['input'].toPlainText().strip()
@@ -89,49 +92,54 @@
 
     def send(
             self,
             text: str = None,
             force: bool = False,
             reply: bool = False,
             internal: bool = False,
-            prev_ctx: CtxItem = None
+            prev_ctx: CtxItem = None,
+            parent_id: int = None,
     ):
         """
         Send input wrapper
 
         :param text: input text
         :param force: force send (ignore input lock)
         :param reply: reply mode (from plugins)
         :param internal: internal call
         :param prev_ctx: previous context (if reply)
+        :param parent_id: parent id (if expert)
         """
         self.execute(
             text=text,
             force=force,
             reply=reply,
             internal=internal,
             prev_ctx=prev_ctx,
+            parent_id=parent_id,
         )
 
     def execute(
             self,
             text: str = None,
             force: bool = False,
             reply: bool = False,
             internal: bool = False,
-            prev_ctx: CtxItem = None
+            prev_ctx: CtxItem = None,
+            parent_id: int = None,
     ):
         """
         Execute send input text to API
 
         :param text: input text
         :param force: force send (ignore input lock)
         :param reply: reply mode (from plugins)
         :param internal: internal call
         :param prev_ctx: previous context (if reply)
+        :param parent_id: parent id (if expert)
         """
         self.window.stateChanged.emit(self.window.STATE_IDLE)
 
         # check if input is not locked
         if self.locked and not force and not internal:
             return
 
@@ -144,15 +152,17 @@
         if mode == 'assistant':
             # check if assistant is selected
             if self.window.core.config.get('assistant') is None \
                     or self.window.core.config.get('assistant') == "":
                 self.window.ui.dialogs.alert(trans('error.assistant_not_selected'))
                 self.generating = False  # unlock
                 return
-        elif mode == 'vision' or self.window.controller.plugins.is_type_enabled('vision'):
+        elif (mode == 'vision'
+              or self.window.controller.plugins.is_type_enabled('vision')
+              or self.window.controller.ui.vision.is_vision_model()):
             # capture frame from camera if auto-capture enabled
             if self.window.controller.camera.is_enabled():
                 if self.window.controller.camera.is_auto():
                     self.window.controller.camera.capture_frame(False)
                     self.log("Captured frame from camera.")  # log
 
         # check if attachment exists, make this here to prevent clearing list on async reply!
@@ -175,15 +185,19 @@
             'mode': mode,
         })
         self.window.core.dispatcher.dispatch(event)
         text = event.data['value']
 
         # check if image captured from camera
         camera_captured = (
-                (mode == 'vision' or self.window.controller.plugins.is_type_enabled('vision'))
+                (
+                        mode == 'vision'
+                        or self.window.controller.plugins.is_type_enabled('vision')
+                        or self.window.controller.ui.vision.is_vision_model()
+                )
                 and self.window.controller.attachment.has(mode)  # check if attachment exists
         )
 
         # allow empty input only for vision modes, otherwise abort
         if len(text.strip()) == 0 and not camera_captured:
             self.generating = False  # unlock as not generating
             return
@@ -214,21 +228,23 @@
         QApplication.processEvents()
 
         # send input to API, return ctx
         if self.window.core.config.get('mode') == 'img':
             ctx = self.window.controller.chat.image.send(
                 text=text,
                 prev_ctx=prev_ctx,
+                parent_id=parent_id,
             )  # image mode
         else:
             ctx = self.window.controller.chat.text.send(
                 text=text,
                 reply=reply,
                 internal=internal,
                 prev_ctx=prev_ctx,
+                parent_id=parent_id,
             )  # text mode: OpenAI, Langchain, Llama, etc.
 
         # clear attachments after send, only if attachments has been provided before send
         if has_attachments:
             if self.window.core.config.get('attachments_send_clear'):
                 self.window.controller.attachment.clear(True)
                 self.window.controller.attachment.update()
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/chat/output.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/chat/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.26 23:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 from PySide6.QtWidgets import QApplication
 
 from pygpt_net.core.dispatcher import Event
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.utils import trans
@@ -232,21 +232,46 @@
             self.window.core.history.append(ctx, "output")
 
         # unlock input if not unlocked before
         self.window.controller.chat.common.unlock_input()  
 
     def handle_cmd(self, ctx: CtxItem):
         """
-        Handle commands
+        Handle commands and expert mentions
 
         :param ctx: CtxItem
         """
         mode = self.window.core.config.get('mode')
-        cmds = self.window.core.command.extract_cmds(ctx.output)  # extract raw commands
+        stream_mode = self.window.core.config.get('stream')
 
+        # extract expert mentions
+        if self.window.controller.agent.experts.enabled():
+            # re-send to master
+            if ctx.sub_reply:
+                self.window.core.ctx.update_item(ctx)
+                self.window.core.experts.reply(ctx)
+            else:
+                # call experts
+                if not ctx.reply:
+                    mentions = self.window.core.experts.extract_mentions(ctx)
+                    if mentions:
+                        self.log("Calling experts...")
+                        self.window.controller.chat.render.end(stream=stream_mode)  # close previous render
+                        for expert_id in mentions:
+                            self.log("Calling: " + expert_id)
+                            ctx.sub_calls += 1
+                            self.window.core.experts.call(
+                                ctx,  # master ctx
+                                expert_id,  # expert id
+                                mentions[expert_id],  # query
+                            )
+                        return  # abort commands if expert call detected
+
+        # extract commands
+        cmds = self.window.core.command.extract_cmds(ctx.output)
         if len(cmds) > 0:
             ctx.cmds = cmds  # append commands to ctx
 
             # agent mode
             if mode == 'agent':
                 commands = self.window.controller.plugins.from_commands(cmds)  # pack to execution list
                 self.window.controller.agent.flow.on_cmd(
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/chat/render.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/chat/render.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/chat/text.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/chat/text.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 from PySide6.QtWidgets import QApplication
 
 from pygpt_net.core.bridge import BridgeContext
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.core.dispatcher import Event
@@ -27,23 +27,25 @@
         self.window = window
 
     def send(
             self,
             text: str,
             reply: bool = False,
             internal: bool = False,
-            prev_ctx: CtxItem = None
+            prev_ctx: CtxItem = None,
+            parent_id: str = None,
     ) -> CtxItem:
         """
         Send text message
 
         :param text: text to send
         :param reply: reply from plugins
         :param internal: internal call
         :param prev_ctx: previous context item (if reply)
+        :param parent_id: parent context id
         :return: context item
         """
         self.window.ui.status(trans('status.sending'))
         is_ctx_debug = self.window.core.config.get("log.ctx")
 
         # event: username prepare
         event = Event(Event.USER_NAME, {
@@ -59,27 +61,39 @@
         self.window.core.dispatcher.dispatch(event)
         ai_name = event.data['value']
 
         # get mode
         mode = self.window.core.config.get('mode')
         model = self.window.core.config.get('model')
         model_data = self.window.core.models.get(model)
+        base_mode = mode  # store parent mode
 
         # create ctx item
         ctx = CtxItem()
         ctx.meta_id = self.window.core.ctx.current
         ctx.internal = internal
         ctx.current = True  # mark as current context item
         ctx.mode = mode  # store current selected mode (not inline changed)
         ctx.model = model  # store model list key, not real model id
         ctx.set_input(text, user_name)
         ctx.set_output(None, ai_name)
         ctx.prev_ctx = prev_ctx  # store previous context item if exists
 
-        self.window.core.ctx.last_item = ctx  # store last item
+        # if prev ctx is not empty
+        if prev_ctx is not None:
+            ctx.input_name = prev_ctx.input_name
+
+        # if reply from expert command
+        if parent_id is not None:
+            ctx.meta_id = parent_id
+            ctx.sub_reply = True  # mark as sub reply
+            ctx.input_name = prev_ctx.input_name
+            ctx.output_name = prev_ctx.output_name
+        else:
+            self.window.core.ctx.last_item = ctx  # store last item
 
         # store thread id, assistant id and pass to gpt wrapper
         if mode == 'assistant':
             self.window.controller.assistant.prepare()  # create new thread if not exists
             ctx.thread = self.window.core.config.get('assistant_thread')
 
         # upload assistant attachments (only assistant mode here)
@@ -89,14 +103,15 @@
             self.window.ui.status(trans('status.sending'))
             self.log("Uploaded attachments (Assistant): {}".format(len(attachments)))
 
         # store history (input)
         if self.window.core.config.get('store_history'):
             self.window.core.history.append(ctx, "input")        
 
+        # log
         if is_ctx_debug:
             self.log("Context: INPUT: {}".format(ctx))
         else:
             self.log("Context: INPUT.")
 
         # agent mode
         if mode == 'agent':
@@ -105,14 +120,30 @@
         # event: context before
         event = Event(Event.CTX_BEFORE)
         event.ctx = ctx
         self.window.core.dispatcher.dispatch(event)
 
         # event: prepare prompt (replace system prompt)
         sys_prompt = self.window.core.config.get('prompt')
+
+        # agent mode
+        if self.window.controller.agent.experts.enabled():
+            prev_prompt = sys_prompt
+            sys_prompt = self.window.core.prompt.get("agent.instruction")
+            if prev_prompt is not None and prev_prompt.strip() != "":
+                sys_prompt = sys_prompt + "\n\n" + prev_prompt  # append previous prompt
+
+        # expert or agent mode
+        if self.window.controller.agent.experts.enabled() and parent_id is None:  # master expert has special prompt
+            if self.window.controller.agent.enabled():  # if agent then leave agent prompt
+                sys_prompt += "\n\n" + self.window.core.experts.get_prompt()  # both, agent + experts
+            else:
+                sys_prompt = self.window.core.experts.get_prompt()
+                mode = "chat"  # change mode to chat for expert
+
         sys_prompt_raw = sys_prompt  # store raw prompt
         event = Event(Event.PRE_PROMPT, {
             'mode': mode,
             'value': sys_prompt,
         })
         self.window.core.dispatcher.dispatch(event)
         sys_prompt = event.data['value']
@@ -121,52 +152,21 @@
         if mode == 'agent':
             sys_prompt = self.window.controller.agent.flow.on_system_prompt(
                 sys_prompt,
                 append_prompt=None,  # sys prompt from preset is used here
                 auto_stop=self.window.core.config.get('agent.auto_stop'),
             )
 
-        # event: system prompt (append to system prompt)
-        event = Event(Event.SYSTEM_PROMPT, {
-            'mode': mode,
-            'value': sys_prompt,
-        })
-        self.window.core.dispatcher.dispatch(event)
-        sys_prompt = event.data['value']
-
-        # event: post prompt (post-handle system prompt)
-        event = Event(Event.POST_PROMPT, {
-            'mode': mode,
-            'reply': reply,
-            'internal': internal,
-            'value': sys_prompt,
-        })
-        event.ctx = ctx
-        self.window.core.dispatcher.dispatch(event)
-        sys_prompt = event.data['value']
-
-        # event: command syntax apply (if commands enabled or inline plugin then append commands prompt)
-        if self.window.core.config.get('cmd') or self.window.controller.plugins.is_type_enabled("cmd.inline"):
-            data = {
-                'mode': mode,
-                'prompt': sys_prompt,
-                'syntax': [],
-                'cmd': [],
-            }
-            # full execute cmd syntax
-            if self.window.core.config.get('cmd'):
-                event = Event(Event.CMD_SYNTAX, data)
-                self.window.core.dispatcher.dispatch(event)
-                sys_prompt = self.window.core.command.append_syntax(event.data)
-
-            # inline cmd syntax only
-            elif self.window.controller.plugins.is_type_enabled("cmd.inline"):
-                event = Event(Event.CMD_SYNTAX_INLINE, data)
-                self.window.core.dispatcher.dispatch(event)
-                sys_prompt = self.window.core.command.append_syntax(event.data)
+        sys_prompt = self.window.core.prompt.prepare_sys_prompt(
+            mode,
+            sys_prompt,
+            ctx,
+            reply,
+            internal,
+        )
 
         self.log("Appending input to chat window...")
 
         # stream mode
         stream_mode = self.window.core.config.get('stream')
 
         # render: begin
@@ -175,24 +175,24 @@
         # append text from input to chat window
         self.window.controller.chat.render.append_input(ctx)
         self.window.ui.nodes['output'].update()
         QApplication.processEvents()
 
         # add ctx to DB here and only update it after response,
         # MUST BE REMOVED NEXT AS FIRST MSG (LAST ON LIST)
-        self.window.core.ctx.add(ctx)
+        self.window.core.ctx.add(ctx, parent_id=parent_id)
 
         # update ctx list, but not reload all to prevent focus out on lists
         self.window.controller.ctx.update(
             reload=True,
             all=False,
         )
 
         # process events to update UI
-        #QApplication.processEvents()
+        # QApplication.processEvents()
 
         # get external functions (if preset is chosen and functions are defined)
         functions = self.window.controller.presets.get_current_functions()
 
         # assistant only
         tools_outputs = []
         if mode == 'assistant':
@@ -207,23 +207,25 @@
         try:
             # make API call
             try:
                 self.window.controller.chat.common.lock_input()  # lock input
                 max_tokens = self.window.core.config.get('max_output_tokens')  # max output tokens
                 files = self.window.core.attachments.get_all(mode)  # get attachments
                 file_ids = self.window.controller.files.uploaded_ids  # uploaded files IDs
+                history = self.window.core.ctx.all(meta_id=parent_id)  # get all history
                 num_files = len(files)
                 if num_files > 0:
                     self.log("Attachments ({}): {}".format(mode, num_files))
 
                 # make call
                 bridge_context = BridgeContext(
                     ctx=ctx,
+                    history=history,
                     mode=mode,
-                    parent_mode=mode,
+                    parent_mode=base_mode,
                     model=model_data,
                     system_prompt=sys_prompt,
                     system_prompt_raw=sys_prompt_raw,
                     prompt=text,
                     stream=stream_mode,
                     attachments=files,
                     file_ids=file_ids,
@@ -284,15 +286,16 @@
         if mode != "assistant":
             ctx.clear_reply()  # reset results
             self.window.controller.chat.output.handle_cmd(ctx)
             ctx.from_previous()  # append previous result again before save
             self.window.core.ctx.update_item(ctx)  # update ctx in DB
 
         # render: end
-        self.window.controller.chat.render.end(stream=stream_mode)
+        if ctx.sub_calls == 0:  # if no experts called
+            self.window.controller.chat.render.end(stream=stream_mode)
 
         # don't unlock input and leave stop btn if assistant mode or if agent/autonomous is enabled
         # send btn will be unlocked in agent mode on stop
         if mode != "assistant" and not self.window.controller.agent.enabled():
             self.window.controller.chat.common.unlock_input()  # unlock input if not assistant and agent mode
 
         # handle ctx name (generate title from summary if not initialized)
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/chat/vision.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/chat/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/command.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/command.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/config/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/config/field/checkbox.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/config/field/cmd.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/cmd.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/config/field/combo.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/config/field/dictionary.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/config/field/input.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/config/field/slider.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/config/field/textarea.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/config/field/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/config/placeholder.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/config/placeholder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.24 02:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 from pygments.styles import get_all_styles
 
 class Placeholder:
     def __init__(self, window=None):
         """
@@ -196,15 +196,15 @@
 
     def get_agent_modes(self) -> list:
         """
         Get modes placeholders list
 
         :return: Models placeholders list
         """
-        modes = ["chat", "completion", "vision", "langchain", "llama_index"]
+        modes = ["chat", "completion", "vision", "langchain", "llama_index", "expert"]
         data = []
         for id in modes:
             data.append({id: id})  # TODO: name
         return data
 
     def get_idx(self) -> list:
         """
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/ctx/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/ctx/common.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/ctx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/ctx/extra.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/ctx/extra.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/ctx/summarizer.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/ctx/summarizer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/debug/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/dialogs/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/dialogs/confirm.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/dialogs/debug.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/dialogs/info.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/dialogs/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/files.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/finder.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/idx/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/idx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/idx/common.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/idx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/idx/indexer.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/idx/indexer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/idx/settings.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/idx/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/lang/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/lang/custom.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/lang/custom.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/lang/mapping.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/lang/mapping.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/lang/plugins.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/lang/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/lang/settings.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/lang/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/launcher.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/layout.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/layout.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/mode.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/model/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/model/editor.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/model/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/notepad.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/painter/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/painter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/painter/capture.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/painter/capture.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/painter/common.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/painter/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/plugins/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/plugins/presets.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/plugins/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/plugins/settings.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/plugins/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/presets/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/presets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 07:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import re
 
 from PySide6.QtGui import QTextCursor
 
 from pygpt_net.controller.presets.editor import Editor
@@ -139,15 +139,14 @@
     def select_default(self):
         """Set default preset"""
         preset_id = self.window.core.config.get('preset')
 
         # if preset is not set, set default
         if preset_id is None or preset_id == "":
             mode = self.window.core.config.get('mode')
-
             # set previously selected preset
             current = self.window.core.config.get('current_preset')  # dict of modes, preset per mode
             if mode in current and \
                     current[mode] is not None and \
                     current[mode] != "" and \
                     current[mode] in self.window.core.presets.get_by_mode(mode):
                 self.window.core.config.set('preset', current[mode])
@@ -259,15 +258,15 @@
         self.update_list()  # update presets list only
         self.select_current()  # select current preset on list
 
     def update_list(self):
         """Update presets list"""
         mode = self.window.core.config.get('mode')
         items = self.window.core.presets.get_by_mode(mode)
-        self.window.ui.toolbox.presets.update(items)
+        self.window.ui.toolbox.presets.update_presets(items)
 
     def reset(self):
         """Reset preset data"""
         self.window.ui.nodes['preset.prompt'].setPlainText("")
         # self.window.ui.nodes['preset.ai_name'].setText("")
         # self.window.ui.nodes['preset.user_name'].setText("")
 
@@ -296,14 +295,42 @@
                     new_id = self.window.core.presets.duplicate(preset)
                     self.window.core.config.set('preset', new_id)
                     self.refresh()
                     idx = self.window.core.presets.get_idx_by_id(mode, new_id)
                     self.editor.edit(idx)
                     self.window.ui.status(trans('status.preset.duplicated'))
 
+    def enable(self, idx: int = None):
+        """
+        Enable preset
+
+        :param idx: preset index (row index)
+        """
+        if idx is not None:
+            mode = self.window.core.config.get('mode')
+            preset_id = self.window.core.presets.get_by_idx(idx, mode)
+            if preset_id is not None and preset_id != "":
+                if preset_id in self.window.core.presets.items:
+                    self.window.core.presets.enable(preset_id)
+                    self.refresh()
+
+    def disable(self, idx: int = None):
+        """
+        Disable preset
+
+        :param idx: preset index (row index)
+        """
+        if idx is not None:
+            mode = self.window.core.config.get('mode')
+            preset_id = self.window.core.presets.get_by_idx(idx, mode)
+            if preset_id is not None and preset_id != "":
+                if preset_id in self.window.core.presets.items:
+                    self.window.core.presets.disable(preset_id)
+                    self.refresh()
+
     def clear(self, force: bool = False):
         """
         Clear preset data
 
         :param force: force clear data
         """
         preset = self.window.core.config.get('preset')
@@ -374,26 +401,30 @@
             self.window.ui.dialogs.confirm(
                 type='preset_restore',
                 id='',
                 msg=trans('confirm.preset.restore'),
             )
             return
         mode = self.window.core.config.get('mode')
+        if mode == "agent":
+            mode = "expert"  # shared presets
         self.window.core.presets.restore(mode)
         self.refresh()
 
     def is_current(self, idx: int = None) -> bool:
         """
         Check if preset is current
 
         :param idx: preset index (row index)
         :return: True if current
         """
         if idx is not None:
             mode = self.window.core.config.get('mode')
+            if mode == "agent":
+                mode = "expert"  # shared presets
             preset_id = self.window.core.presets.get_by_idx(idx, mode)
             if preset_id is not None and preset_id != "":
                 if preset_id == "current." + mode:
                     return True
         return False
 
     def validate_filename(self, value: str) -> str:
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/presets/editor.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/presets/editor.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,32 +2,34 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.22 23:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import datetime
 import os
 
 from pygpt_net.item.preset import PresetItem
 from pygpt_net.utils import trans
+from .experts import Experts
 
 
 class Editor:
     def __init__(self, window=None):
         """
         Presets editor controller
 
         :param window: Window instance
         """
         self.window = window
+        self.experts = Experts(window)
         self.options = {
             "filename": {
                 "type": "text",
                 "label": "preset.filename",
             },
             "name": {
                 "type": "text",
@@ -57,14 +59,18 @@
                 "type": "bool",
                 "label": "preset.vision",
             },
             "langchain": {
                 "type": "bool",
                 "label": "preset.langchain",
             },
+            "expert": {
+                "type": "bool",
+                "label": "preset.expert",
+            },
             "agent": {
                 "type": "bool",
                 "label": "preset.agent",
             },
             # "assistant": {
             # "type": "bool",
             # "label": "preset.assistant",
@@ -105,14 +111,15 @@
                     "urls": {
                         "Help": "https://platform.openai.com/docs/guides/function-calling",
                     },
                 },
             },
         }
         self.id = "preset"
+        self.current = None
 
     def get_options(self) -> dict:
         """
         Get preset options
 
         :return: preset options
         """
@@ -179,14 +186,15 @@
         data.name = ""
         data.filename = ""
 
         if id is not None and id != "":
             if id in self.window.core.presets.items:
                 data = self.window.core.presets.items[id]
                 data.filename = id
+                self.current = data.uuid
 
         if data.name is None:
             data.name = ""
         if data.ai_name is None:
             data.ai_name = ""
         if data.user_name is None:
             data.user_name = ""
@@ -208,14 +216,16 @@
                 data.vision = True
             elif mode == "langchain":
                 data.langchain = True
             # elif mode == "'"assistant':
                 # data.assistant = True
             elif mode == "llama_index":
                 data.llama_index = True
+            elif mode == "expert":
+                data.expert = True
             elif mode == "agent":
                 data.agent = True
 
         options = {}
         data_dict = data.to_dict()
         for key in self.options:
             options[key] = self.options[key]
@@ -223,14 +233,17 @@
 
         # load options
         self.window.controller.config.load_options(
             self.id,
             options,
         )
 
+        # update experts list, after ID loaded
+        self.experts.update_list()
+
         # restore functions
         if data.has_functions():
             functions = data.get_functions()
             values = []
             for function in functions:
                 values.append(
                     {
@@ -244,26 +257,28 @@
         else:
             self.window.ui.config[self.id]['tool.function'].items = []
             self.window.ui.config[self.id]['tool.function'].model.updateData([])
 
         # set focus to name field
         self.window.ui.config[self.id]['name'].setFocus()
 
-    def save(self, force: bool = False):
+    def save(self, force: bool = False, close: bool = True):
         """
         Save ore create preset
 
         :param force: force overwrite file
+        :param close: close dialog
         """
         id = self.window.controller.config.get_value(
             parent_id=self.id,
             key="filename",
             option=self.options["filename"],
         )
         mode = self.window.core.config.get("mode")
+        modes = ["chat", "completion", "img", "vision", "langchain", "llama_index", "expert"]
 
         # disallow editing default preset
         if id == "current." + mode:
             self.window.ui.dialogs.alert("Reserved ID. Please use another ID.")
             return
 
         if id is None or id == "":
@@ -286,55 +301,70 @@
             )
             if os.path.exists(path) and not force:
                 id = id + '_' + datetime.datetime.now().strftime('%Y%m%d%H%M%S')
 
         # validate filename
         id = self.window.controller.presets.validate_filename(id)
         if id not in self.window.core.presets.items:
-            self.window.core.presets.items[id] = PresetItem()
+            self.window.core.presets.items[id] = self.window.core.presets.build()
         elif not force:
             self.window.ui.dialogs.confirm(
                 type='preset_exists',
                 id=id,
                 msg=trans('confirm.preset.overwrite'),
             )
             return
 
         # check if at least one mode is selected
-        modes = ["chat", "completion", "img", "vision", "langchain", "agent", "llama_index"]
         is_mode = False
-        for mode in modes:
+        for check in modes:
             if self.window.controller.config.get_value(
                 parent_id=self.id,
-                key=mode,
-                option=self.options[mode],
+                key=check,
+                option=self.options[check],
             ):
                 is_mode = True
                 break
-        if not is_mode:
+        if mode != "agent" and not is_mode:
             self.window.ui.dialogs.alert(
                 trans('alert.preset.no_chat_completion')
             )
             return
 
         # assign data from fields to preset object in items
         self.assign_data(id)
 
+        # if agent, assign experts and select only agent mode
+        if self.window.core.config.get('mode') == 'agent':
+            self.window.core.presets.items[id].mode = ["agent"]
+
         # apply changes to current active preset
         current = self.window.core.config.get('preset')
         if current is not None and current == id:
             self.to_current(self.window.core.presets.items[id])
             self.window.core.config.save()
 
+        # update current uuid
+        self.current = self.window.core.presets.items[id].uuid
+
         # save
         self.window.core.presets.save(id)
         self.window.controller.presets.refresh()
 
         # close dialog
-        self.window.ui.dialogs.close('editor.preset.presets')
+        if close:
+            self.window.ui.dialogs.close('editor.preset.presets')
+        else:
+            # update ID in field
+            self.window.controller.config.apply_value(
+                parent_id=self.id,
+                key="filename",
+                option=self.options["filename"],
+                value=id,
+            )
         self.window.ui.status(trans('status.preset.saved'))
 
         # sort by name
         self.window.core.presets.sort_by_name()
 
         # switch to editing preset
         self.window.controller.presets.set(mode, id)
@@ -349,15 +379,14 @@
         :param id: preset id (filename)
         """
         data_dict = {}
         for key in self.options:
             # assigned separately
             if key == "tool.function":
                 continue
-
             data_dict[key] = self.window.controller.config.get_value(
                 parent_id=self.id,
                 key=key,
                 option=self.options[key],
             )
         if data_dict['name'] is None or data_dict['name'] == "":
             data_dict['name'] = id + " " + trans('preset.untitled')
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/settings/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/settings/editor.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/settings/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/settings/profile.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/settings/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/settings/workdir.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/settings/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/theme/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/theme/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,19 @@
         """
         self.window.core.config.set("render.code_syntax", name)
         self.window.core.config.save()
         self.window.controller.chat.render.on_theme_change()
         if update_menu:
             self.menu.update_syntax()
 
+    def update_syntax(self):
+        """Update syntax menu"""
+        curr = self.window.core.config.get('render.code_syntax')
+        self.toggle_syntax(curr, update_menu=True)
+
     def reload(self, force: bool = True):
         """
         Reload current theme
 
         :param force: force theme change (manual trigger)
         """
         current = self.window.core.config.get('theme')
@@ -171,7 +176,8 @@
         :return: CSS style for element
         """
         return self.common.get_style(element)
 
     def reload_all(self):
         """Reload all"""
         self.setup()
+        self.update_syntax()
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/theme/common.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/theme/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/theme/markdown.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/theme/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/theme/menu.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/theme/menu.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/theme/nodes.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/theme/nodes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/ui/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/ui/mode.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/presets.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,161 +1,131 @@
-# !/usr/bin/env python3
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
-from pygpt_net.core.dispatcher import Event
+from PySide6 import QtCore
+from PySide6.QtGui import QStandardItemModel, Qt
+from PySide6.QtWidgets import QVBoxLayout, QLabel, QHBoxLayout, QPushButton, QSplitter, QWidget
 
+from pygpt_net.ui.widget.element.labels import HelpLabel, TitleLabel
+from pygpt_net.ui.widget.lists.preset import PresetList
+from pygpt_net.ui.layout.toolbox.footer import Footer
+from pygpt_net.utils import trans
 
-class Mode:
+
+class Presets:
     def __init__(self, window=None):
         """
-        UI mode switch controller
+        Toolbox UI
 
         :param window: Window instance
         """
         self.window = window
+        self.footer = Footer(window)
+        self.id = 'preset.presets'
+
+    def setup(self) -> QSplitter:
+        """
+        Setup presets
+
+        :return: QSplitter
+        """
+        presets = self.setup_presets()
 
-    def update(self):
-        """Update mode, model, preset and rest of the toolbox"""
+        self.window.ui.models['preset.presets'] = self.create_model(self.window)
+        self.window.ui.nodes['preset.presets'].setModel(self.window.ui.models['preset.presets'])
 
-        mode = self.window.core.config.data['mode']
+        self.window.ui.nodes['presets.widget'] = QWidget()
+        self.window.ui.nodes['presets.widget'].setLayout(presets)
+        self.window.ui.nodes['presets.widget'].setMinimumHeight(150)
+
+        return self.window.ui.nodes['presets.widget']
+
+    def setup_presets(self) -> QVBoxLayout:
+        """
+        Setup list
+
+        :return: QVBoxLayout
+        """
+        self.window.ui.nodes['preset.presets.new'] = QPushButton(trans('preset.new'))
+        self.window.ui.nodes['preset.presets.new'].clicked.connect(
+            lambda: self.window.controller.presets.editor.edit()
+        )
+
+        self.window.ui.nodes['preset.presets.label'] = TitleLabel(trans("toolbox.presets.label"))
+        self.window.ui.nodes['preset.agents.label'] = TitleLabel(trans("toolbox.agents.label"))
+        self.window.ui.nodes['preset.experts.label'] = TitleLabel(trans("toolbox.experts.label"))
+        self.window.ui.nodes['preset.presets.label'].setVisible(False)
+        self.window.ui.nodes['preset.agents.label'].setVisible(False)
+        self.window.ui.nodes['preset.experts.label'].setVisible(False)
+
+        header = QHBoxLayout()
+        header.addWidget(self.window.ui.nodes['preset.presets.label'])
+        header.addWidget(self.window.ui.nodes['preset.agents.label'])
+        header.addWidget(self.window.ui.nodes['preset.experts.label'])
+        header.addWidget(self.window.ui.nodes['preset.presets.new'], alignment=Qt.AlignRight)
+        header.setContentsMargins(0, 0, 0, 0)
+
+        header_widget = QWidget()
+        header_widget.setLayout(header)
+
+        self.window.ui.nodes[self.id] = PresetList(self.window, self.id)
+        self.window.ui.nodes[self.id].selection_locked = self.window.controller.presets.preset_change_locked
+
+        self.window.ui.nodes['tip.toolbox.presets'] = HelpLabel(trans('tip.toolbox.presets'), self.window)
+
+        layout = QVBoxLayout()
+        layout.addWidget(header_widget)
+        layout.addWidget(self.window.ui.nodes[self.id])
+        layout.addWidget(self.window.ui.nodes['tip.toolbox.presets'])
+
+        self.window.ui.models[self.id] = self.create_model(self.window)
+        self.window.ui.nodes[self.id].setModel(self.window.ui.models[self.id])
+
+        return layout
+
+    def create_model(self, parent) -> QStandardItemModel:
+        """
+        Create list model
+        :param parent: parent widget
+        :return: QStandardItemModel
+        """
+        return QStandardItemModel(0, 1, parent)
+
+    def update_presets(self, data):
+        """
+        Update presets list
+
+        :param data: Data to update
+        """
+        mode = self.window.core.config.get('mode')
 
-        # presets
-        if mode != "assistant":
-            self.window.ui.nodes['presets.widget'].setVisible(True)
-        else:
-            self.window.ui.nodes['presets.widget'].setVisible(False)
-
-        # presets: clear
-        if mode in ["img", "llama_index", "assistant"]:
-            self.window.ui.nodes['preset.clear'].setVisible(False)
-        else:
-            self.window.ui.nodes['preset.clear'].setVisible(True)
-
-        # presets: use
-        if mode == 'img':
-            self.window.ui.nodes['preset.use'].setVisible(True)
-        else:
-            self.window.ui.nodes['preset.use'].setVisible(False)
-
-        # img options
-        if mode == "img":
-            self.window.ui.nodes['dalle.options'].setVisible(True)
-        else:
-            self.window.ui.nodes['dalle.options'].setVisible(False)
-
-        # agent options
-        if mode == "agent":
-            self.window.ui.nodes['agent.options'].setVisible(True)
-        else:
-            self.window.ui.nodes['agent.options'].setVisible(False)
-
-        # assistants list
-        if mode == "assistant":
-            self.window.ui.nodes['assistants.widget'].setVisible(True)
-        else:
-            self.window.ui.nodes['assistants.widget'].setVisible(False)
-
-        # indexes list
-        if mode == "llama_index":
-            # self.window.ui.nodes['indexes.widget'].setVisible(True)
-            self.window.ui.nodes['idx.options'].setVisible(True)
-        else:
-            # self.window.ui.nodes['indexes.widget'].setVisible(False)
-            self.window.ui.nodes['idx.options'].setVisible(False)
-
-        # stream mode
-        if mode in ["img"]:
-            self.window.ui.nodes['input.stream'].setVisible(False)
-        else:
-            self.window.ui.nodes['input.stream'].setVisible(True)
-
-        # vision
-        show = self.is_vision(mode)
-        self.window.ui.menu['menu.video'].menuAction().setVisible(show)
-        self.window.ui.nodes['icon.video.capture'].setVisible(show)
-        # self.window.ui.nodes['vision.capture.options'].setVisible(show)
-        self.window.ui.nodes['attachments.capture_clear'].setVisible(show)
-
-        # attachments
-        show = self.are_attachments(mode)
-        self.window.ui.tabs['input'].setTabVisible(1, show)  # attachments
-
-        # uploaded files
-        if mode == "assistant":
-            self.window.ui.tabs['input'].setTabVisible(2, True)
-        else:
-            self.window.ui.tabs['input'].setTabVisible(2, False)
-
-        # toggle chat footer
-        if not self.is_chat_tab():
-            self.hide_chat_footer()
-        else:
-            self.show_chat_footer()
-
-    def is_vision(self, mode: str) -> bool:
-        """
-        Check if vision is allowed
-
-        :param mode: current mode
-        """
-        if mode == "vision":
-            return True
-
-        allowed = self.window.controller.painter.is_active()
-        if allowed:
-            return True
-
-        if mode in ["img", "assistant"]:
-            return False
-
-        if self.window.controller.ui.vision.is_vision_model():
-            return True
-
-        # event: UI: vision
-        value = False
-        event = Event(Event.UI_VISION, {
-            'mode': mode,
-            'value': value,
-        })
-        self.window.core.dispatcher.dispatch(event)
-        return event.data['value']
-
-    def are_attachments(self, mode: str) -> bool:
-        """Check if attachments are allowed"""
-        if mode in ["vision", "assistant"]:
-            return True
-
-        if mode == "img":
-            return False
-
-        if self.window.controller.ui.vision.is_vision_model():
-            return True
-
-        # event: UI: attachments
-        value = False
-        event = Event(Event.UI_ATTACHMENTS, {
-            'mode': mode,
-            'value': value,
-        })
-        self.window.core.dispatcher.dispatch(event)
-        return event.data['value']
-
-    def is_chat_tab(self) -> bool:
-        """Check if current tab is chat"""
-        return self.window.controller.ui.current_tab == self.window.controller.ui.tab_idx['chat']
-
-    def show_chat_footer(self):
-        """Show chat footer"""
-        self.window.ui.nodes['chat.footer'].setVisible(True)
-
-    def hide_chat_footer(self):
-        """Hide chat footer"""
-        self.window.ui.nodes['chat.footer'].setVisible(False)
+        # store previous selection
+        self.window.ui.nodes[self.id].backup_selection()
+        self.window.ui.models[self.id].removeRows(0, self.window.ui.models[self.id].rowCount())
+        i = 0
+        for n in data:
+            self.window.ui.models[self.id].insertRow(i)
+            name = data[n].name
+
+            # show disabled in expert mode
+            if mode == "expert" and not n.startswith("current.") and data[n].enabled:
+                name = "[x] " + name
+            elif mode =="agent":
+                num_experts = len(data[n].experts)
+                if num_experts > 0:
+                    name = name + " (" + str(num_experts) + " experts)"
+
+            index = self.window.ui.models[self.id].index(i, 0)
+            self.window.ui.models[self.id].setData(index, n, QtCore.Qt.ToolTipRole)
+            self.window.ui.models[self.id].setData(self.window.ui.models[self.id].index(i, 0), name)
+            i += 1
 
+        # restore previous selection
+        self.window.ui.nodes[self.id].restore_selection()
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/controller/ui/vision.py` & `pygpt_net-2.2.7/src/pygpt_net/controller/ui/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/assistants/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/core/assistants/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/assistants/files.py` & `pygpt_net-2.2.7/src/pygpt_net/core/assistants/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/assistants/store.py` & `pygpt_net-2.2.7/src/pygpt_net/core/assistants/store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/attachments.py` & `pygpt_net-2.2.7/src/pygpt_net/core/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/audio.py` & `pygpt_net-2.2.7/src/pygpt_net/core/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/bridge.py` & `pygpt_net-2.2.7/src/pygpt_net/core/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 03:00:00                  #
 # ================================================== #
 
 import time
 from datetime import datetime, timedelta
 
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.item.model import ModelItem
@@ -20,14 +20,15 @@
     def __init__(self, **kwargs):
         """
         Bridge context
 
         :param kwargs: keyword arguments
         """
         self.ctx = kwargs.get("ctx", CtxItem())
+        self.history = kwargs.get("history", [])
         self.mode = kwargs.get("mode", None)
         self.parent_mode = kwargs.get("parent_mode", None)  # real mode (global)
         self.model = kwargs.get("model", None)  # model instance, not model name
         self.temperature = kwargs.get("temperature", 1.0)
         self.prompt = kwargs.get("prompt", "")
         self.system_prompt = kwargs.get("system_prompt", "")
         self.system_prompt_raw = kwargs.get("system_prompt_raw", "")  # without plugins addons
@@ -52,14 +53,15 @@
         """
         Return as dictionary
 
         :return: dictionary
         """
         return {
             "ctx": self.ctx,  # "ctx": self.ctx.dump() ??
+            "history": self.history,
             "mode": self.mode,
             "parent_mode": self.parent_mode,
             "model": self.model,
             "temperature": self.temperature,
             "prompt": self.prompt,
             "system_prompt": self.system_prompt,
             "system_prompt_raw": self.system_prompt_raw,
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/calendar/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/core/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/camera.py` & `pygpt_net-2.2.7/src/pygpt_net/core/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/chain/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/core/chain/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 03:00:00                  #
 # ================================================== #
 
 from pygpt_net.core.bridge import BridgeContext
 from pygpt_net.item.ctx import CtxItem
 from .chat import Chat
 from .completion import Completion
 
@@ -57,24 +57,26 @@
 
         try:
             if sub_mode == 'chat':
                 response = self.chat.send(
                     prompt=prompt,
                     system_prompt=system_prompt,
                     model=model,
+                    history=context.history,
                     stream=stream,
                     ai_name=ai_name,
                     user_name=user_name,
                 )
                 used_tokens = self.chat.get_used_tokens()
             elif sub_mode == 'completion':
                 response = self.completion.send(
                     prompt=prompt,
                     system_prompt=system_prompt,
                     model=model,
+                    history=context.history,
                     stream=stream,
                     ai_name=ai_name,
                     user_name=user_name,
                 )
                 used_tokens = self.completion.get_used_tokens()
 
         except Exception as e:
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/chain/chat.py` & `pygpt_net-2.2.7/src/pygpt_net/core/chain/chat.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 03:00:00                  #
 # ================================================== #
 
 from langchain.schema import SystemMessage, HumanMessage, AIMessage
 
 from pygpt_net.item.model import ModelItem
 
 
@@ -25,24 +25,26 @@
         self.input_tokens = 0
 
     def send(
             self,
             prompt: str,
             system_prompt: str,
             model: ModelItem,
+            history: list = None,
             stream: bool = False,
             ai_name: str = None,
             user_name: str = None
     ):
         """
         Chat with LLM
 
         :param prompt: user prompt
         :param system_prompt: system prompt
         :param model: model item
+        :param history: history
         :param stream: stream mode
         :param ai_name: AI name
         :param user_name: username
         :return: LLM response
         """
         llm = None
         if 'provider' in model.langchain:
@@ -69,36 +71,39 @@
         if llm is None:
             raise Exception("Invalid LLM")
 
         messages = self.build(
             prompt=prompt,
             system_prompt=system_prompt,
             model=model,
+            history=history,
             ai_name=ai_name,
             user_name=user_name,
         )
         if stream:
             return llm.stream(messages)
         else:
             return llm.invoke(messages)
 
     def build(
             self,
             prompt: str,
             system_prompt: str,
             model: ModelItem,
+            history: list = None,
             ai_name: str = None,
             user_name: str = None
     ) -> list:
         """
         Build chat messages list
 
         :param prompt: user prompt
         :param system_prompt: system prompt
         :param model: model item
+        :param history: history
         :param ai_name: AI name
         :param user_name: username
         :return: list of messages
         """
         messages = []
 
         # tokens
@@ -117,15 +122,16 @@
 
         # append initial (system) message
         if system_prompt is not None and system_prompt != "":
             messages.append(SystemMessage(content=system_prompt))
 
         # append messages from context (memory)
         if self.window.core.config.get('use_context'):
-            items = self.window.core.ctx.get_prompt_items(
+            items = self.window.core.ctx.get_history(
+                history,
                 model.id,
                 "langchain",
                 used_tokens,
                 max_ctx_tokens,
             )
             for item in items:
                 # input
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/chain/completion.py` & `pygpt_net-2.2.7/src/pygpt_net/core/chain/completion.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 03:00:00                  #
 # ================================================== #
 
 from pygpt_net.item.model import ModelItem
 
 
 class Completion:
     def __init__(self, window=None):
@@ -23,24 +23,26 @@
         self.input_tokens = 0
 
     def send(
             self,
             prompt: str,
             system_prompt: str,
             model: ModelItem,
+            history: list = None,
             stream: bool = False,
             ai_name: str = None,
             user_name: str = None
     ):
         """
         Chat with LLM
 
         :param prompt: user prompt
         :param system_prompt: system prompt
         :param model: model item
+        :param history: history
         :param stream: stream mode
         :param ai_name: AI name
         :param user_name: username
         :return: LLM response
         """
         llm = None
         if 'provider' in model.langchain:
@@ -79,23 +81,25 @@
             return llm.invoke(message)
 
     def build(
             self,
             prompt: str,
             system_prompt: str,
             model: ModelItem,
+            history: list = None,
             ai_name: str = None,
             user_name: str = None
     ) -> str:
         """
         Build completion string
 
         :param prompt: user prompt
         :param system_prompt: system prompt
         :param model: model item
+        :param history: history
         :param ai_name: AI name
         :param user_name: username
         :return: message string (parsed with context)
         """
         message = ""
 
         # tokens config
@@ -112,15 +116,16 @@
         # input tokens: reset
         self.reset_tokens()
 
         if system_prompt is not None and system_prompt != "":
             message += system_prompt
 
         if self.window.core.config.get('use_context'):
-            items = self.window.core.ctx.get_prompt_items(
+            items = self.window.core.ctx.get_history(
+                history,
                 model.id,
                 "langchain",
                 used_tokens,
                 max_ctx_tokens,
             )
             for item in items:
                 if item.input_name is not None \
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/command.py` & `pygpt_net-2.2.7/src/pygpt_net/core/command.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/ctx/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/core/ctx/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.17 07:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import copy
 import datetime
 import uuid
 
 from packaging.version import Version
@@ -50,22 +50,23 @@
         self.search_string = None  # search string
         self.groups = {}  # groups
         self.filters = {}  # search filters
         self.filters_labels = []  # search labels
         self.current_cmd = []  # current commands
         self.current_cmd_schema = "" # current commands schema
         self.allowed_modes = {
-            'chat': ["chat", "completion", "img", "langchain", "vision", "assistant", "llama_index", "agent"],
-            'completion': ["chat", "completion", "img", "langchain", "vision", "assistant", "llama_index", "agent"],
+            'chat': ["chat", "completion", "img", "langchain", "vision", "assistant", "llama_index", "agent", "expert"],
+            'completion': ["chat", "completion", "img", "langchain", "vision", "assistant", "llama_index", "agent", "expert"],
             'img': ["img"],
-            'langchain': ["chat", "completion", "img", "langchain", "vision", "assistant", "llama_index", "agent"],
-            'vision': ["chat", "completion", "img", "langchain", "vision", "assistant", "llama_index", "agent"],
+            'langchain': ["chat", "completion", "img", "langchain", "vision", "assistant", "llama_index", "agent", "expert"],
+            'vision': ["chat", "completion", "img", "langchain", "vision", "assistant", "llama_index", "agent", "expert"],
             'assistant': ["assistant"],
-            'llama_index': ["chat", "completion", "img", "langchain", "vision", "assistant", "llama_index", "agent"],
-            'agent': ["chat", "completion", "img", "langchain", "vision", "assistant", "llama_index", "agent"],
+            'llama_index': ["chat", "completion", "img", "langchain", "vision", "assistant", "llama_index", "agent", "expert"],
+            'agent': ["chat", "completion", "img", "langchain", "vision", "assistant", "llama_index", "agent", "expert"],
+            'expert': ["chat", "completion", "img", "langchain", "vision", "assistant", "llama_index", "agent", "expert"],
         }
         self.current_sys_prompt = ""
         self.groups_loaded = False
 
     def install(self):
         """Install provider data"""
         self.provider.install()
@@ -173,32 +174,53 @@
         meta = self.build()
         if group_id is not None:
             meta.group_id = group_id
         id = self.provider.create(meta)
         meta.id = id
         return meta
 
-    def add(self, item: CtxItem):
+    def add(self, item: CtxItem, parent_id: int = None):
         """
         Add CtxItem to contexts and saves context
 
         :param item: CtxItem to append
+        :param parent_id: parent id
         """
+        # custom parent
+        if parent_id is not None:
+            self.add_to_meta(item, parent_id)
+            return
+
+        # to current
         self.items.append(item)  # add CtxItem to context items
 
         # append in provider
         if self.current is not None:
             if self.current not in self.meta:
                 self.load_tmp_meta(self.current)
             if self.current in self.meta:
                 meta = self.meta[self.current]
                 result = self.provider.append_item(meta, item)
                 if not result:
                     self.store()  # if not stored, e.g. in JSON file provider, then store whole ctx (save all)
 
+    def add_to_meta(self, item: CtxItem, meta_id: int = None):
+        """
+        Add CtxItem to custom meta
+
+        :param item: CtxItem to append
+        :param meta_id: meta id
+        """
+        if meta_id in self.meta:
+            meta = self.meta[meta_id]
+        else:
+            meta = self.provider.get_meta_by_id(meta_id)
+        if meta is not None:
+            self.provider.append_item(meta, item)
+
     def update_item(self, item: CtxItem):
         """
         Update CtxItem in context
 
         :param item: CtxItem to update
         """
         self.provider.update_item(item)
@@ -452,21 +474,25 @@
         :return: ctx meta count
         """
         extra = 0
         if self.tmp_meta is not None:
             extra = 1  # prevent create new if tmp meta exists
         return len(self.meta) + extra
 
-    def all(self) -> list:
+    def all(self, meta_id: int = None) -> list:
         """
-        Return ctx items
+        Return ctx items (current or by meta_id if provided)
 
+        :param meta_id: meta id
         :return: ctx items
         """
-        return self.items
+        if meta_id is None:
+            return self.items
+        else:
+            return self.load(meta_id)
 
     def remove(self, id: int):
         """
         Delete ctx by id
 
         :param id: ctx id
         """
@@ -546,14 +572,36 @@
         self.status = status
         if self.current is None:
             return
         if self.current in self.meta:
             self.meta[self.current].status = self.status
             self.save(self.current)
 
+    def get_or_create_slave_meta(self, master_ctx: CtxItem, preset_id: str) -> CtxMeta:
+        """
+        Get or create slave meta
+
+        :param master_ctx: master context
+        :param preset_id: preset ID
+        :return: slave meta
+        """
+        slaves = self.provider.get_meta_by_root_id_and_preset_id(
+            master_ctx.meta_id,
+            preset_id,
+        )
+        if len(slaves) > 0:
+            return list(slaves.values())[0]
+        slave = self.build()
+        slave.root_id = master_ctx.meta_id
+        slave.parent_id = master_ctx.meta_id
+        slave.preset = preset_id
+        id = self.provider.create(slave)
+        slave.id = id
+        return slave
+
     def count_history(
             self,
             history_items: list,
             model: str,
             mode: str,
             used_tokens: int = 100,
             max_tokens: int = 1000
@@ -915,15 +963,15 @@
                 "mode": "IN",
                 "value": self.filters_labels,  # append label colors
             }
         return filters
 
     def load(self, id: int) -> list:
         """
-        Load ctx data from provider
+        Load ctx items from provider
 
         :param id: ctx id
         :return: ctx items list
         """
         return self.provider.load(id)
 
     def load_groups(self):
@@ -1106,14 +1154,16 @@
         prev_ctx.urls = copy.deepcopy(ctx.urls)
         prev_ctx.images = copy.deepcopy(ctx.images)
         prev_ctx.files = copy.deepcopy(ctx.files)
         prev_ctx.attachments = copy.deepcopy(ctx.attachments)
         prev_ctx.results = copy.deepcopy(ctx.results)
         prev_ctx.index_meta = copy.deepcopy(ctx.index_meta)
         prev_ctx.doc_ids = copy.deepcopy(ctx.doc_ids)
+        prev_ctx.input_name = copy.deepcopy(ctx.input_name)
+        prev_ctx.output_name = copy.deepcopy(ctx.output_name)
 
         ctx.clear_reply()  # clear current reply result
         ctx.from_previous()  # get result from previous if exists
         return prev_ctx
 
     def dump(self, ctx: CtxItem) -> str:
         """
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/ctx/idx.py` & `pygpt_net-2.2.7/src/pygpt_net/core/ctx/idx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/db/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/core/db/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 07:00:00                  #
+# Updated Date: 2024.05.01 03:00:00                  #
 # ================================================== #
 
 import os
 import shutil
 import time
 
 from sqlalchemy import create_engine, text
@@ -100,14 +100,17 @@
             'is_deleted',
             'is_important',
             'is_archived',
             'label',
             'indexes_json',
             'external_id',
             'group_id',
+            'root_id',
+            'parent_id',
+            'owner_uuid',
             'uuid',
         ]
         columns["ctx_group"] = [
             'id',
             'name',
             'updated_ts',
             'created_ts',
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/db/viewer.py` & `pygpt_net-2.2.7/src/pygpt_net/core/db/viewer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/debug/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/core/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/debug/agent.py` & `pygpt_net-2.2.7/src/pygpt_net/core/debug/agent.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/debug/assistants.py` & `pygpt_net-2.2.7/src/pygpt_net/core/debug/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/debug/attachments.py` & `pygpt_net-2.2.7/src/pygpt_net/core/debug/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/debug/config.py` & `pygpt_net-2.2.7/src/pygpt_net/core/debug/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/debug/context.py` & `pygpt_net-2.2.7/src/pygpt_net/core/debug/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/debug/db.py` & `pygpt_net-2.2.7/src/pygpt_net/core/debug/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/debug/indexes.py` & `pygpt_net-2.2.7/src/pygpt_net/core/debug/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/debug/models.py` & `pygpt_net-2.2.7/src/pygpt_net/core/debug/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/debug/plugins.py` & `pygpt_net-2.2.7/src/pygpt_net/core/debug/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/debug/presets.py` & `pygpt_net-2.2.7/src/pygpt_net/core/debug/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/debug/ui.py` & `pygpt_net-2.2.7/src/pygpt_net/core/debug/ui.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/dispatcher.py` & `pygpt_net-2.2.7/src/pygpt_net/core/dispatcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.02.25 12:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import json
 
 from PySide6.QtWidgets import QApplication
 
 from pygpt_net.item.ctx import CtxItem
@@ -146,19 +146,21 @@
     def async_allowed(self, ctx: CtxItem) -> bool:
         """
         Check if async execution are allowed
 
         :param ctx: context item
         :return: True if async commands are allowed
         """
-        disallowed_modes = ["assistant", "agent"]
+        disallowed_modes = ["assistant", "agent", "expert"]
         if ctx.internal:
             return False
         if self.window.core.config.get("mode") in disallowed_modes:
             return False
+        if self.window.controller.agent.enabled() or self.window.controller.agent.experts.enabled():
+            return False
         if len(ctx.cmds) > 1:  # if multiple commands then run synchronously
             return False
         return True
 
     def dispatch(
             self,
             event: Event,
@@ -258,20 +260,25 @@
         data = json.dumps(results)
         if len(self.reply_stack) < 2 and self.reply_ctx.extra_ctx and self.window.core.config.get("ctx.use_extra"):
             data = self.reply_ctx.extra_ctx  # if extra content is set, use it as data to send
 
         prev_ctx = self.window.core.ctx.as_previous(self.reply_ctx)  # copy result to previous ctx and clear current ctx
         self.window.core.ctx.update_item(self.reply_ctx)  # update context in db
         self.window.ui.status('...')
+
+        parent_id = None
+        if self.reply_ctx.sub_call:
+            parent_id = self.reply_ctx.meta_id  # slave meta id
         self.window.controller.chat.input.send(
             text=data,
             force=True,
             reply=True,
             internal=self.reply_ctx.internal,
             prev_ctx=prev_ctx,
+            parent_id=parent_id,
         )
         self.clear_reply_stack()
 
     def clear_reply_stack(self):
         """Clear reply stack"""
         self.window.core.debug.info("Reply stack (clear)...")
         self.reply_ctx = None
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/filesystem/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/core/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/filesystem/actions.py` & `pygpt_net-2.2.7/src/pygpt_net/core/filesystem/actions.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/filesystem/editor.py` & `pygpt_net-2.2.7/src/pygpt_net/core/filesystem/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/filesystem/types.py` & `pygpt_net-2.2.7/src/pygpt_net/core/filesystem/types.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/filesystem/url.py` & `pygpt_net-2.2.7/src/pygpt_net/core/filesystem/url.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/history.py` & `pygpt_net-2.2.7/src/pygpt_net/core/history.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/idx/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/core/idx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/idx/chat.py` & `pygpt_net-2.2.7/src/pygpt_net/core/idx/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 03:00:00                  #
 # ================================================== #
 
 import json
 
 from llama_index.core.llms import ChatMessage, MessageRole
 from llama_index.core.prompts import ChatPromptTemplate
 from llama_index.core.memory import ChatMemoryBuffer
@@ -173,15 +173,19 @@
         if not self.storage.exists(idx):
             raise Exception("Index not prepared")
 
         service_context = self.window.core.idx.llm.get_service_context(model=model)
         index = self.storage.get(idx, service_context=service_context)  # get index
 
         # append context from DB
-        history = self.context.get_messages(ctx.input, system_prompt)
+        history = self.context.get_messages(
+            ctx.input,
+            system_prompt,
+            context.history,
+        )
         memory = self.get_memory_buffer(history, service_context.llm)
         input_tokens = self.window.core.tokens.from_llama_messages(
             query,
             history,
             model.id,
         )
         chat_engine = index.as_chat_engine(
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/idx/context.py` & `pygpt_net-2.2.7/src/pygpt_net/core/idx/context.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,35 +2,41 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.02.27 22:00:00                  #
+# Updated Date: 2024.05.01 03:00:00                  #
 # ================================================== #
 
 from llama_index.core.llms import ChatMessage, MessageRole
 
 
 class Context:
     def __init__(self, window=None):
         """
         Context core
 
         :param window: Window instance
         """
         self.window = window
 
-    def get_messages(self, input_prompt, system_prompt):
+    def get_messages(
+            self,
+            input_prompt: str,
+            system_prompt: str,
+            history: list = None
+    ):
         """
         Get messages from db
 
         :param input_prompt: input prompt
         :param system_prompt: system prompt
+        :param history: history
         :return: Messages
         """
         messages = []
 
         # tokens config
         model = self.window.core.config.get('model')
         model_id = self.window.core.models.get_id(model)
@@ -41,15 +47,21 @@
         model_ctx = self.window.core.models.get_num_ctx(model_id)
 
         # fit to max model tokens
         if max_tokens > model_ctx:
             max_tokens = model_ctx
 
         if self.window.core.config.get('use_context'):
-            items = self.window.core.ctx.get_prompt_items(model_id, mode, used_tokens, max_tokens)
+            items = self.window.core.ctx.get_history(
+                history,
+                model_id,
+                mode,
+                used_tokens,
+                max_tokens,
+            )
             for item in items:
                 # input
                 if item.input is not None and item.input != "":
                     messages.append(ChatMessage(
                         role=MessageRole.USER,
                         content=item.input
                     ))
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/idx/indexing.py` & `pygpt_net-2.2.7/src/pygpt_net/core/idx/indexing.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/idx/llm.py` & `pygpt_net-2.2.7/src/pygpt_net/core/idx/llm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/idx/metadata.py` & `pygpt_net-2.2.7/src/pygpt_net/core/idx/metadata.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/idx/types/ctx.py` & `pygpt_net-2.2.7/src/pygpt_net/core/idx/types/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/idx/types/external.py` & `pygpt_net-2.2.7/src/pygpt_net/core/idx/types/external.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/idx/types/files.py` & `pygpt_net-2.2.7/src/pygpt_net/core/idx/types/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/idx/worker.py` & `pygpt_net-2.2.7/src/pygpt_net/core/idx/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/image.py` & `pygpt_net-2.2.7/src/pygpt_net/core/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/info.py` & `pygpt_net-2.2.7/src/pygpt_net/core/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/installer.py` & `pygpt_net-2.2.7/src/pygpt_net/core/installer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/llm/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/core/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/locale.py` & `pygpt_net-2.2.7/src/pygpt_net/core/locale.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/models.py` & `pygpt_net-2.2.7/src/pygpt_net/core/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/modes.py` & `pygpt_net-2.2.7/src/pygpt_net/core/modes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/notepad.py` & `pygpt_net-2.2.7/src/pygpt_net/core/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/platforms.py` & `pygpt_net-2.2.7/src/pygpt_net/core/platforms.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/plugins.py` & `pygpt_net-2.2.7/src/pygpt_net/core/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/presets.py` & `pygpt_net-2.2.7/src/pygpt_net/core/presets.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.17 13:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import copy
+import uuid
 
 from packaging.version import Version
 from pygpt_net.item.preset import PresetItem
 from pygpt_net.provider.core.preset.json_file import JsonFileProvider
 
 
 class Presets:
@@ -38,37 +39,41 @@
 
     def build(self) -> PresetItem:
         """
         Build empty preset
 
         :return: empty preset
         """
-        return PresetItem()
+        preset = PresetItem()
+        preset.uuid = str(uuid.uuid4())
+        return preset
 
     def append_current(self):
         """Append current presets"""
         # create empty presets
         curr_chat = self.build()
         curr_completion = self.build()
         curr_img = self.build()
         curr_vision = self.build()
         curr_langchain = self.build()
         curr_assistant = self.build()
         curr_llama = self.build()
         curr_agent = self.build()
+        curr_expert = self.build()
 
         # prepare ids
         id_chat = 'current.chat'
         id_completion = 'current.completion'
         id_img = 'current.img'
         id_vision = 'current.vision'
         id_langchain = 'current.langchain'
         id_assistant = 'current.assistant'
         id_llama = 'current.llama_index'
         id_agent = 'current.agent'
+        id_expert = 'current.expert'
 
         # set default initial prompt for chat mode
         curr_chat.prompt = self.window.core.prompt.get('default')
 
         # get data from presets if exists
         if id_chat in self.items:
             curr_chat = self.items[id_chat]
@@ -82,59 +87,93 @@
             curr_langchain = self.items[id_langchain]
         if id_assistant in self.items:
             curr_assistant = self.items[id_assistant]
         if id_llama in self.items:
             curr_llama = self.items[id_llama]
         if id_agent in self.items:
             curr_agent = self.items[id_agent]
+        if id_expert in self.items:
+            curr_expert = self.items[id_expert]
 
         # allow usage in specific mode
         curr_chat.chat = True
         curr_completion.completion = True
         curr_img.img = True
         curr_vision.vision = True
         curr_langchain.langchain = True
         curr_assistant.assistant = True
         curr_llama.llama_index = True
         curr_agent.agent = True
+        curr_expert.expert = True
 
         # always apply default name
         curr_chat.name = '*'
         curr_completion.name = '*'
         curr_img.name = '*'
         curr_vision.name = '*'
         curr_langchain.name = '*'
         curr_assistant.name = '*'
         curr_llama.name = '*'
         curr_agent.name = '*'
+        curr_expert.name = '*'
 
         # append at first position
         self.items = {
             id_chat: curr_chat,
             id_completion: curr_completion,
             id_img: curr_img,
             id_vision: curr_vision,
             id_langchain: curr_langchain,
             id_assistant: curr_assistant,
             id_llama: curr_llama,
             id_agent: curr_agent,
+            id_expert: curr_expert,
             **self.items
         }
 
     def exists(self, id: str) -> bool:
         """
         Check if preset exists
 
         :param id: preset id
         :return: True if exists
         """
         if id in self.items:
             return True
         return False
 
+    def exists_uuid(self, uuid: str) -> bool:
+        """
+        Check if preset exists
+
+        :param uuid: preset uuid
+        :return: True if exists
+        """
+        for id in self.items:
+            if self.items[id].uuid == uuid:
+                return True
+        return False
+
+    def enable(self, id: str):
+        """
+        Enable preset
+
+        :param id: preset id
+        """
+        if id in self.items:
+            self.items[id].enabled = True
+    def disable(self, id: str):
+        """
+        Disable preset
+
+        :param id: preset id
+        """
+        if id in self.items:
+            self.items[id].enabled = False
+
     def get_first_mode(self, id: str) -> str or None:
         """
         Return first mode for preset
 
         :param id: preset id
         :return: mode name
         """
@@ -151,14 +190,16 @@
             return 'langchain'
         if preset.assistant:
             return 'assistant'
         if preset.llama_index:
             return 'llama_index'
         if preset.agent:
             return 'agent'
+        if preset.expert:
+            return 'expert'
         return None
 
     def has(self, mode: str, id: str) -> bool:
         """
         Check if preset for mode exists
 
         :param mode: mode name
@@ -177,14 +218,39 @@
         :param idx: index
         :param mode: mode
         :return: preset id
         """
         presets = self.get_by_mode(mode)
         return list(presets.keys())[idx]
 
+    def get_by_id(self, mode: str, id: str) -> PresetItem or None:
+        """
+        Return preset by id
+
+        :param mode: mode name
+        :param id: preset id
+        :return: preset item
+        """
+        presets = self.get_by_mode(mode)
+        if id in presets:
+            return presets[id]
+        return None
+
+    def get_by_uuid(self, uuid: str) -> PresetItem or None:
+        """
+        Return preset by UUID
+
+        :param uuid: preset UUID
+        :return: preset item
+        """
+        for id in self.items:
+            if self.items[id].uuid == uuid:
+                return self.items[id]
+        return None
+
     def get_by_mode(self, mode: str) -> dict:
         """
         Return presets for mode
 
         :param mode: mode name
         :return: presets dict for mode
         """
@@ -193,15 +259,16 @@
             if (mode == 'chat' and self.items[id].chat) \
                     or (mode == 'completion' and self.items[id].completion) \
                     or (mode == 'img' and self.items[id].img) \
                     or (mode == 'vision' and self.items[id].vision) \
                     or (mode == 'langchain' and self.items[id].langchain) \
                     or (mode == 'assistant' and self.items[id].assistant) \
                     or (mode == 'llama_index' and self.items[id].llama_index) \
-                    or (mode == 'agent' and self.items[id].agent):
+                    or (mode == 'agent' and self.items[id].agent) \
+                    or (mode == 'expert' and self.items[id].expert):
                 presets[id] = self.items[id]
         return presets
 
     def get_idx_by_id(self, mode: str, id: str) -> int:
         """
         Return preset index
 
@@ -252,14 +319,15 @@
         :param id: preset id
         :return: duplicated preset ID
         """
         prev_id = id
         id, name = self.get_duplicate_name(id)
         self.items[id] = copy.deepcopy(self.items[prev_id])
         self.items[id].name = name
+        self.items[id].filename = id
         self.sort_by_name()
         return id
 
     def remove(self, id: str, remove_file: bool = True):
         """
         Delete preset
 
@@ -307,26 +375,66 @@
     def load_base(self):
         """Load base presets"""
         return self.provider.load_base()
 
     def load(self):
         """Load presets templates"""
         self.items = self.provider.load()
+        self.patch_uuids()
 
         # sort presets
         self.sort_by_name()
         self.append_current()
 
     def save(self, id: str):
         """
         Save preset
 
         :param id: preset id
         """
         if id not in self.items:
             return
-
         self.provider.save(id, self.items[id])
 
     def save_all(self):
         """Save all presets"""
         self.provider.save_all(self.items)
+
+    def add_expert(self, agent_uuid: str, expert_uuid: str):
+        """
+        Add expert to agent
+
+        :param agent_uuid: agent uuid
+        :param expert_uuid: expert uuid
+        """
+        agent = self.get_by_uuid(agent_uuid)
+        if agent is None:
+            return
+        if expert_uuid not in agent.experts:
+            agent.experts.append(expert_uuid)
+        self.save(agent.filename)
+
+    def remove_expert(self, agent_uuid: str, expert_uuid: str):
+        """
+        Remove expert from agent
+        :param agent_uuid: agent uuid
+        :param expert_uuid: expert uuid
+        """
+        agent = self.get_by_uuid(agent_uuid)
+        if agent is None:
+            return
+        if expert_uuid in agent.experts:
+            agent.experts.remove(expert_uuid)
+        self.save(agent.filename)
+
+    def patch_uuids(self):
+        """Patch UUIDs for all presets"""
+        patched = False
+        for id in self.items:
+            if self.items[id].uuid is None:
+                self.items[id].uuid = str(uuid.uuid4())
+                patched = True
+            if self.items[id].filename is None or self.items[id].filename == "":
+                self.items[id].filename = id
+                patched = True
+        if patched:
+            self.save_all()
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/profile.py` & `pygpt_net-2.2.7/src/pygpt_net/core/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/prompt/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/core/prompt/template.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,68 +5,87 @@
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
 # Updated Date: 2024.04.22 23:00:00                  #
 # ================================================== #
 
-from pygpt_net.core.dispatcher import Event
+import os
+import csv
 
-from .template import Template
+from PySide6.QtGui import QAction
+from pygpt_net.utils import trans
 
 
-class Prompt:
+class Template:
     def __init__(self, window=None):
         """
-        Prompt core
+        Prompt templates
 
         :param window: Window instance
         """
         self.window = window
-        self.template = Template(window)
+        self.prompts = {}
+        self.loaded = False
 
-    def get(self, prompt: str) -> str:
+    def init(self):
+        """Init prompt templates"""
+        self.load()
+
+    def load(self):
+        """Load prompt templates"""
+        if self.loaded:
+            return
+        try:
+            self.load_from_csv()
+        except Exception as e:
+            self.window.core.debug.log(e)
+        self.loaded = True
+
+    def load_from_csv(self):
+        """Load prompt templates from CSV"""
+        # CSV file is given from: https://github.com/f/awesome-chatgpt-prompts
+        path = os.path.join(self.window.core.config.get_app_path(), "data", "prompts.csv")
+        self.prompts = {}
+        i = 0
+        with open(path, newline='', encoding='utf-8') as f:
+            data = csv.reader(f, delimiter=',')
+            for row in data:
+                if i == 0:
+                    i += 1
+                    continue
+                self.prompts[i] = {
+                    "name": row[0],
+                    "prompt": row[1]
+                }
+                i += 1
+        # sort by name
+        self.prompts = dict(sorted(self.prompts.items(), key=lambda item: item[1]['name']))
+
+    def to_menu_options(self, menu, parent: str = "global"):
+        """Convert prompts to menu options"""
+        self.init()
+        menu.addSeparator()
+        submenu = menu.addMenu(trans("preset.prompt.paste_template"))
+        for key, value in self.prompts.items():
+            action = QAction(value['name'], menu)
+            action.triggered.connect(lambda checked=False, key=key: self.window.controller.presets.paste_prompt(key, parent))
+            action.setToolTip(value['prompt'])
+            submenu.addAction(action)
+
+    def get_by_id(self, id: int) -> dict or None:
+        """
+        Get prompt by id
+
+        :param id: Prompt ID
         """
-        Get prompt content
+        self.init()
+        return self.prompts.get(id, None)
 
-        :param prompt: id of the prompt
-        :return: text content
+    def get_all(self) -> dict:
         """
-        key = "prompt." + prompt
-        if self.window.core.config.has(key):
-            return str(self.window.core.config.get(key))
-        return ""
-
-    def build_final_system_prompt(self, prompt: str) -> str:
-        # tmp dispatch event: system prompt
-        event = Event(Event.SYSTEM_PROMPT, {
-            'mode': self.window.core.config.get('mode'),
-            'value': prompt,
-            'silent': True,
-        })
-        self.window.core.dispatcher.dispatch(event)
-        prompt = event.data['value']
-
-        if self.window.core.config.get('cmd') or self.window.controller.plugins.is_type_enabled("cmd.inline"):
-
-            # cmd syntax tokens
-            data = {
-                'prompt': prompt,
-                'silent': True,
-                'syntax': [],
-                'cmd': [],
-            }
-
-            # tmp dispatch event: command syntax apply
-            # full execute cmd syntax
-            if self.window.core.config.get('cmd'):
-                event = Event(Event.CMD_SYNTAX, data)
-                self.window.core.dispatcher.dispatch(event)
-                prompt = self.window.core.command.append_syntax(event.data)
-
-            # inline cmd syntax only
-            elif self.window.controller.plugins.is_type_enabled("cmd.inline"):
-                event = Event(Event.CMD_SYNTAX_INLINE, data)
-                self.window.core.dispatcher.dispatch(event)
-                prompt = self.window.core.command.append_syntax(event.data)
+        Get all prompt templates
 
-        return prompt
+        :return: Prompt templates
+        """
+        self.init()
+        return self.prompts
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/prompt/template.py` & `pygpt_net-2.2.7/src/pygpt_net/item/attachment.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,90 +2,78 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.22 23:00:00                  #
+# Updated Date: 2024.04.26 23:00:00                  #
 # ================================================== #
 
-import os
-import csv
+import json
 
-from PySide6.QtGui import QAction
-from pygpt_net.utils import trans
 
-
-class Template:
-    def __init__(self, window=None):
+class AttachmentItem:
+    def __init__(self):
+        """
+        Attachment item
         """
-        Prompt templates
+        self.name = None
+        self.id = None
+        self.path = None
+        self.remote = None
+        self.vector_store_ids = []
+        self.size = 0
+        self.send = False
 
-        :param window: Window instance
+    def serialize(self) -> dict:
         """
-        self.window = window
-        self.prompts = {}
-        self.loaded = False
+        Serialize item to dict
 
-    def init(self):
-        """Init prompt templates"""
-        self.load()
+        :return: serialized item
+        """
+        return {
+            'id': self.id,
+            'name': self.name,
+            'path': self.path,
+            'size': self.size,
+            'remote': self.remote,
+            'vector_store_ids': self.vector_store_ids,
+            'send': self.send
+        }
 
-    def load(self):
-        """Load prompt templates"""
-        if self.loaded:
-            return
-        try:
-            self.load_from_csv()
-        except Exception as e:
-            self.window.core.debug.log(e)
-        self.loaded = True
+    def deserialize(self, data: dict):
+        """
+        Deserialize item from dict
 
-    def load_from_csv(self):
-        """Load prompt templates from CSV"""
-        # CSV file is given from: https://github.com/f/awesome-chatgpt-prompts
-        path = os.path.join(self.window.core.config.get_app_path(), "data", "prompts.csv")
-        self.prompts = {}
-        i = 0
-        with open(path, newline='', encoding='utf-8') as f:
-            data = csv.reader(f, delimiter=',')
-            for row in data:
-                if i == 0:
-                    i += 1
-                    continue
-                self.prompts[i] = {
-                    "name": row[0],
-                    "prompt": row[1]
-                }
-                i += 1
-        # sort by name
-        self.prompts = dict(sorted(self.prompts.items(), key=lambda item: item[1]['name']))
-
-    def to_menu_options(self, menu, parent: str = "global"):
-        """Convert prompts to menu options"""
-        self.init()
-        menu.addSeparator()
-        submenu = menu.addMenu(trans("preset.prompt.paste_template"))
-        for key, value in self.prompts.items():
-            action = QAction(value['name'], menu)
-            action.triggered.connect(lambda checked=False, key=key: self.window.controller.presets.paste_prompt(key, parent))
-            action.setToolTip(value['prompt'])
-            submenu.addAction(action)
-
-    def get_by_id(self, id: int) -> dict or None:
-        """
-        Get prompt by id
-
-        :param id: Prompt ID
-        """
-        self.init()
-        return self.prompts.get(id, None)
+        :param data: serialized item
+        """
+        if 'id' in data:
+            self.id = data['id']
+        if 'name' in data:
+            self.name = data['name']
+        if 'path' in data:
+            self.path = data['path']
+        if 'size' in data:
+            self.size = data['size']
+        if 'remote_id' in data:
+            self.remote = data['remote']
+        if 'vector_store_ids' in data:
+            self.vector_store_ids = data['vector_store_ids']
+        if 'send' in data:
+            self.send = data['send']
 
-    def get_all(self) -> dict:
+    def dump(self) -> str:
         """
-        Get all prompt templates
+        Dump item to string
 
-        :return: Prompt templates
+        :return: serialized item
         """
-        self.init()
-        return self.prompts
+        try:
+            return json.dumps(self.serialize())
+        except Exception as e:
+            pass
+        return ""
+
+    def __str__(self):
+        """To string"""
+        return self.dump()
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/render/base.py` & `pygpt_net-2.2.7/src/pygpt_net/core/render/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/render/markdown/parser.py` & `pygpt_net-2.2.7/src/pygpt_net/core/render/markdown/parser.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/render/markdown/renderer.py` & `pygpt_net-2.2.7/src/pygpt_net/core/render/markdown/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/render/plain/renderer.py` & `pygpt_net-2.2.7/src/pygpt_net/core/render/plain/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/render/web/parser.py` & `pygpt_net-2.2.7/src/pygpt_net/core/render/web/parser.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/render/web/renderer.py` & `pygpt_net-2.2.7/src/pygpt_net/core/render/web/renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import json
 import os
 import re
 import html
 import time
@@ -63,21 +63,27 @@
         """
         if not self.initialized:
             self.flush()
             self.initialized = True
         else:
             self.clear_chunks()
 
+    def reset_names(self):
+        """Reset names"""
+        self.name_user = trans("chat.name.user")
+        self.name_bot = trans("chat.name.bot")
+
     def begin(self, stream: bool = False):
         """
         Render begin
 
         :param stream: True if it is a stream
         """
         self.init()
+        self.reset_names()
 
     def end(self, stream: bool = False):
         """
         Render end
 
         :param stream: True if it is a stream
         """
@@ -118,16 +124,15 @@
         self.item = None
         self.html = ""
         self.clear_nodes()
         self.clear_chunks()
         self.images_appended = []
         self.urls_appended = []
         self.get_output_node().reset_current_content()
-        self.name_user = trans("chat.name.user")
-        self.name_bot = trans("chat.name.bot")
+        self.reset_names()
 
     def reload(self):
         """Reload output, called externally only on theme change to redraw content"""
         self.window.controller.ctx.refresh_output()  # if clear all and appends all items again
 
     def update_names(self, item: CtxItem):
         """
@@ -189,15 +194,16 @@
         if item.input.strip().startswith("[") and item.input.strip().endswith("]"):
             is_cmd = True
 
         # hidden internal call
         if item.internal \
                 and not is_cmd \
                 and not item.first \
-                and not item.input.strip().startswith("user: "):
+                and not item.input.strip().startswith("user: ")\
+                and not item.input.strip().startswith("@"):  # expert says:
             if flush:
                 content = self.prepare_node('>>>', self.NODE_INPUT, item)
                 self.append_chunk_input(item, content, True)
             else:
                 self.append_node('>>>', self.NODE_INPUT, item)
             return
         else:
@@ -272,15 +278,16 @@
 
         :param item: context item
         :param text_chunk: text chunk
         :param begin: if it is the beginning of the text
         """
         if text_chunk is None or text_chunk == "":
             return
-
+        if item.hidden:
+            return
         self.clear_chunks_input()
         chunk = self.format_chunk(text_chunk)
         escaped_chunk = json.dumps(chunk)
         try:
             self.get_output_node().page().runJavaScript(f"appendToInput({escaped_chunk});")
         except Exception as e:
             pass
@@ -315,15 +322,18 @@
         :param item: CtxItem instance
         :return: prepared HTML
         """
         id = "msg-user-" + str(item.id) if item is not None else ""
         content = self.append_timestamp(self.format_user_text(html), item, type=self.NODE_INPUT)
         html = "<p>" + content + "</p>"
         html = self.post_format_text(html)
-        html = '<div class="msg-box msg-user" id="{}"><div class="name-header name-user">{}</div><div class="msg">'.format(id, self.name_user) + html + "</div></div>"
+        name = self.name_user
+        if item.internal and not item.input.startswith("user: "):
+            name = "System"
+        html = '<div class="msg-box msg-user" id="{}"><div class="name-header name-user">{}</div><div class="msg">'.format(id, name) + html + "</div></div>"
         return html
 
     def prepare_node_output(self, html: str, item: CtxItem = None) -> str:
         """
         Prepare output node
 
         :param html: html text
@@ -344,14 +354,16 @@
         """
         Append and format raw text to output
 
         :param html: text to append
         :param type: type of message
         :param item: CtxItem instance
         """
+        if item.hidden:
+            return
         self.append(self.prepare_node(html, type, item))
 
     def clear_chunks_output(self):
         """Clear chunks from output"""
         if not self.loaded:
             js = "var element = document.getElementById('_append_output_');"
             js += "if (element) { element.innerHTML = ''; }"
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/settings.py` & `pygpt_net-2.2.7/src/pygpt_net/core/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/text/finder.py` & `pygpt_net-2.2.7/src/pygpt_net/core/text/finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/text/utils.py` & `pygpt_net-2.2.7/src/pygpt_net/core/text/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/text/web_finder.py` & `pygpt_net-2.2.7/src/pygpt_net/core/text/web_finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/tokens.py` & `pygpt_net-2.2.7/src/pygpt_net/core/tokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import tiktoken
 
 from pygpt_net.item.ctx import CtxItem
 
-CHAT_MODES = ["chat", "vision", "langchain", "assistant", "llama_index", "agent"]
+CHAT_MODES = ["chat", "vision", "langchain", "assistant", "llama_index", "agent", "expert"]
 
 
 class Tokens:
     def __init__(self, window=None):
         """
         Tokens core
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/updater/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/core/updater/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/web.py` & `pygpt_net-2.2.7/src/pygpt_net/core/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/core/worker.py` & `pygpt_net-2.2.7/src/pygpt_net/core/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/config/models.json` & `pygpt_net-2.2.7/src/pygpt_net/data/config/models.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.874077912414966%*

 * *Differences: {"'__meta__'": "{'version': '2.2.7', 'app.version': '2.2.7', 'updated_at': '2024-05-01T00:00:00'}",*

 * * "'items'": "{'gpt-3.5-turbo': {'mode': {insert: [(5, 'expert')]}}, 'gpt-3.5-turbo-1106': {'mode': "*

 * *            "{insert: [(4, 'expert')]}}, 'gpt-3.5-turbo-16k': {'mode': {insert: [(5, 'expert')]}}, "*

 * *            "'gpt-4': {'mode': {insert: [(5, 'expert')]}}, 'gpt-4-1106-preview': {'mode': {insert: "*

 * *            "[(5, 'expert')]}}, 'gpt-4-0125-preview': {'mode': {insert: [(5, 'expert')]}}, "*

 * *            "'gp […]*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.6",
-        "updated_at": "2024-04-30T00:00:00",
-        "version": "2.2.6"
+        "app.version": "2.2.7",
+        "updated_at": "2024-05-01T00:00:00",
+        "version": "2.2.7"
     },
     "items": {
         "dall-e-2": {
             "ctx": 0,
             "default": false,
             "id": "dall-e-2",
             "langchain": {
@@ -100,15 +100,16 @@
                 "provider": "openai"
             },
             "mode": [
                 "chat",
                 "assistant",
                 "langchain",
                 "llama_index",
-                "agent"
+                "agent",
+                "expert"
             ],
             "name": "gpt-3.5-turbo",
             "tokens": 4096
         },
         "gpt-3.5-turbo-1106": {
             "ctx": 16385,
             "default": false,
@@ -142,15 +143,16 @@
                 "mode": [],
                 "provider": null
             },
             "mode": [
                 "chat",
                 "assistant",
                 "langchain",
-                "agent"
+                "agent",
+                "expert"
             ],
             "name": "gpt-3.5-turbo-1106",
             "tokens": 4096
         },
         "gpt-3.5-turbo-16k": {
             "ctx": 16385,
             "default": false,
@@ -202,15 +204,16 @@
                 "provider": "openai"
             },
             "mode": [
                 "chat",
                 "assistant",
                 "langchain",
                 "llama_index",
-                "agent"
+                "agent",
+                "expert"
             ],
             "name": "gpt-3.5-turbo-16k",
             "tokens": 4096
         },
         "gpt-3.5-turbo-instruct": {
             "ctx": 4096,
             "default": false,
@@ -302,15 +305,16 @@
                 "provider": "openai"
             },
             "mode": [
                 "chat",
                 "assistant",
                 "langchain",
                 "llama_index",
-                "agent"
+                "agent",
+                "expert"
             ],
             "name": "gpt-4",
             "tokens": 4096
         },
         "gpt-4-0125-preview": {
             "ctx": 128000,
             "default": false,
@@ -362,15 +366,16 @@
                 "provider": "openai"
             },
             "mode": [
                 "chat",
                 "assistant",
                 "langchain",
                 "llama_index",
-                "agent"
+                "agent",
+                "expert"
             ],
             "name": "gpt-4-0125-preview",
             "tokens": 4096
         },
         "gpt-4-1106-preview": {
             "ctx": 128000,
             "default": false,
@@ -422,15 +427,16 @@
                 "provider": "openai"
             },
             "mode": [
                 "chat",
                 "assistant",
                 "langchain",
                 "llama_index",
-                "agent"
+                "agent",
+                "expert"
             ],
             "name": "gpt-4-1106-preview",
             "tokens": 4096
         },
         "gpt-4-32k": {
             "ctx": 32768,
             "default": false,
@@ -482,15 +488,16 @@
                 "provider": "openai"
             },
             "mode": [
                 "chat",
                 "assistant",
                 "langchain",
                 "llama_index",
-                "agent"
+                "agent",
+                "expert"
             ],
             "name": "gpt-4-32k",
             "tokens": 4096
         },
         "gpt-4-turbo": {
             "ctx": 128000,
             "default": false,
@@ -543,15 +550,16 @@
             },
             "mode": [
                 "chat",
                 "assistant",
                 "langchain",
                 "llama_index",
                 "vision",
-                "agent"
+                "agent",
+                "expert"
             ],
             "name": "gpt-4-turbo",
             "tokens": 4096
         },
         "gpt-4-turbo-2024-04-09": {
             "ctx": 128000,
             "default": false,
@@ -604,15 +612,16 @@
             },
             "mode": [
                 "chat",
                 "assistant",
                 "langchain",
                 "llama_index",
                 "vision",
-                "agent"
+                "agent",
+                "expert"
             ],
             "name": "gpt-4-turbo-2024-04-09",
             "tokens": 4096
         },
         "gpt-4-turbo-preview": {
             "ctx": 128000,
             "default": false,
@@ -664,15 +673,16 @@
                 "provider": "openai"
             },
             "mode": [
                 "chat",
                 "assistant",
                 "langchain",
                 "llama_index",
-                "agent"
+                "agent",
+                "expert"
             ],
             "name": "gpt-4-turbo-preview",
             "tokens": 4096
         },
         "gpt-4-vision-preview": {
             "ctx": 128000,
             "default": false,
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/config/modes.json` & `pygpt_net-2.2.7/src/pygpt_net/data/config/modes.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8472222222222222%*

 * *Differences: {"'__meta__'": "{'version': '2.2.7', 'app.version': '2.2.7', 'updated_at': '2024-05-01T00:00:00'}",*

 * * "'items'": "{'expert': OrderedDict([('id', 'expert'), ('name', 'Experts'), ('label', "*

 * *            "'mode.expert'), ('default', False)])}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.6",
-        "updated_at": "2024-04-30T00:00:00",
-        "version": "2.2.6"
+        "app.version": "2.2.7",
+        "updated_at": "2024-05-01T00:00:00",
+        "version": "2.2.7"
     },
     "items": {
         "agent": {
             "default": false,
             "id": "agent",
             "label": "mode.agent",
             "name": "Agent (autonomous)"
@@ -25,14 +25,20 @@
         },
         "completion": {
             "default": false,
             "id": "completion",
             "label": "mode.completion",
             "name": "completion"
         },
+        "expert": {
+            "default": false,
+            "id": "expert",
+            "label": "mode.expert",
+            "name": "Experts"
+        },
         "img": {
             "default": false,
             "id": "img",
             "label": "mode.img",
             "name": "img"
         },
         "langchain": {
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/config/settings.json` & `pygpt_net-2.2.7/src/pygpt_net/data/config/settings.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.968421052631579%*

 * *Differences: {"'experts.mode'": "OrderedDict([('section', 'agent'), ('type', 'combo'), ('use', 'agent_modes'), "*

 * *                   "('slider', False), ('label', 'settings.experts.mode'), ('description', "*

 * *                   "'settings.experts.mode.desc'), ('value', 'chat'), ('min', None), ('max', "*

 * *                   "None), ('multiplier', None), ('step', None), ('advanced', False)])",*

 * * "'prompt.agent.instruction'": "OrderedDict([('section', 'prompts'), ('type', 'textarea'), "*

 * *                               "('slider', […]*

```diff
@@ -217,14 +217,28 @@
         "multiplier": null,
         "section": "files",
         "slider": false,
         "step": null,
         "type": "text",
         "value": "download"
     },
+    "experts.mode": {
+        "advanced": false,
+        "description": "settings.experts.mode.desc",
+        "label": "settings.experts.mode",
+        "max": null,
+        "min": null,
+        "multiplier": null,
+        "section": "agent",
+        "slider": false,
+        "step": null,
+        "type": "combo",
+        "use": "agent_modes",
+        "value": "chat"
+    },
     "font_size": {
         "advanced": false,
         "description": "settings.font_size.tip",
         "label": "settings.font_size",
         "max": 42,
         "min": 8,
         "multiplier": 1,
@@ -948,14 +962,27 @@
         "multiplier": 1,
         "section": "prompts",
         "slider": false,
         "step": 1,
         "type": "textarea",
         "value": ""
     },
+    "prompt.agent.instruction": {
+        "advanced": false,
+        "description": "settings.prompt.agent.instruction.desc",
+        "label": "settings.prompt.agent.instruction",
+        "max": 0,
+        "min": 0,
+        "multiplier": 1,
+        "section": "prompts",
+        "slider": false,
+        "step": 1,
+        "type": "textarea",
+        "value": ""
+    },
     "prompt.cmd": {
         "advanced": false,
         "description": "settings.prompt.cmd.desc",
         "label": "settings.prompt.cmd",
         "max": null,
         "min": null,
         "multiplier": null,
@@ -1011,14 +1038,27 @@
         "multiplier": null,
         "section": "prompts",
         "slider": false,
         "step": null,
         "type": "textarea",
         "value": ""
     },
+    "prompt.expert": {
+        "advanced": false,
+        "description": "settings.prompt.expert.desc",
+        "label": "settings.prompt.expert",
+        "max": 0,
+        "min": 0,
+        "multiplier": 1,
+        "section": "prompts",
+        "slider": false,
+        "step": 1,
+        "type": "textarea",
+        "value": ""
+    },
     "prompt.img": {
         "advanced": false,
         "description": "settings.prompt.img.desc",
         "label": "settings.prompt.img",
         "max": null,
         "min": null,
         "multiplier": null,
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/config/settings_section.json` & `pygpt_net-2.2.7/src/pygpt_net/data/config/settings_section.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/css/fix_windows.css` & `pygpt_net-2.2.7/src/pygpt_net/data/css/fix_windows.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/css/markdown.css` & `pygpt_net-2.2.7/src/pygpt_net/data/css/markdown.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/css/markdown.dark.css` & `pygpt_net-2.2.7/src/pygpt_net/data/css/markdown.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/css/markdown.light.css` & `pygpt_net-2.2.7/src/pygpt_net/data/css/markdown.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/css/style.dark.css` & `pygpt_net-2.2.7/src/pygpt_net/data/css/style.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/css/style.light.css` & `pygpt_net-2.2.7/src/pygpt_net/data/css/style.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/css/web.css` & `pygpt_net-2.2.7/src/pygpt_net/data/css/web.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/css/web.dark.css` & `pygpt_net-2.2.7/src/pygpt_net/data/css/web.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/css/web.light.css` & `pygpt_net-2.2.7/src/pygpt_net/data/css/web.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/Lato/OFL.txt` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/SpaceMono/OFL.txt` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/OFL.txt`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf` & `pygpt_net-2.2.7/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icon.ico` & `pygpt_net-2.2.7/src/pygpt_net/data/icon.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icon.png` & `pygpt_net-2.2.7/src/pygpt_net/data/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icon_tray_busy.ico` & `pygpt_net-2.2.7/src/pygpt_net/data/icon_tray_busy.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icon_tray_error.ico` & `pygpt_net-2.2.7/src/pygpt_net/data/icon_tray_error.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icon_tray_idle.ico` & `pygpt_net-2.2.7/src/pygpt_net/data/icon_tray_idle.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/abc.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/abc.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/alarm.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/alarm.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/apps.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/apps.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/build.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/build.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/calendar.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/calendar.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/chat/audio.png` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/audio.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/chat/copy.png` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/copy.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/chat/delete.png` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/delete.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/chat/edit.png` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/edit.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/chat/join.png` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/join.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/chat/reload.png` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/chat/reload.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/cut.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/cut.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/db.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/db.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/error.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/error.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/hearing.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/hearing.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/help.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/help.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/info.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/info.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/key.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/key.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/keyboard.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/keyboard.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/language.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/language.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/palette.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/palette.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/public_filled.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/public_filled.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/robot.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/router.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/router.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/sensors.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/sensors.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/settings.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/share.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/share.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/view.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/view.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/icons/voice.svg` & `pygpt_net-2.2.7/src/pygpt_net/data/icons/voice.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.de.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.de.ini`

 * *Files 1% similar despite different names*

```diff
@@ -478,14 +478,16 @@
 menu.video = Video
 menu.video.capture = Eingang: kamera
 menu.video.capture.auto = Automatische Bildaufnahme
 mode.agent = Agent (autonom)
 mode.assistant = Assistent
 mode.chat = Chat
 mode.completion = Vervollständigung
+mode.expert = Experten (Kooperation)
+mode.expert.tooltip = Experten zum Hintergrund rufen
 mode.img = Bild (DALL-E)
 mode.langchain = Langchain
 mode.vision = Vision
 mode.llama_index = Chat mit Dateien
 mode.agent.tooltip = Autonome Agenten
 mode.assistant.tooltip = Chat mittels Assistants API
 mode.chat.tooltip = Chatmodus (Standard)
@@ -515,27 +517,33 @@
 painter.btn.clear = Löschen
 painter.capture.name.prefix = Zeichnung von
 painter.capture.manual.captured.success = Bild erfasst:
 plugin.tab.general = Allgemein
 preset.action.delete = Löschen
 preset.action.duplicate = Duplizieren
 preset.action.edit = Bearbeiten
+preset.action.enable = Aktivieren
+preset.action.disable = Deaktivieren
 preset.ai_name = KI-Name
 preset.assistant = Assistent
 preset.chat = Chat
 preset.clear = Löschen
 preset.completion = Vervollständigung
+preset.expert = Experten
+preset.experts.available.label = Verfügbare Experten
+preset.experts.selected.label = Zugewiesene Experten (dieser Agent)
 preset.filename = ID (Dateiname)
 preset.img = Bild
 preset.langchain = Langchain
 preset.llama_index = Chat mit Dateien
 preset.name = Voreinstellungsname
 preset.new = Erstellen
 preset.prompt = Systemaufforderung
 preset.prompt.paste_template: Aus Vorlage einfügen...
+preset.prompt.agent = Agentensystemaufforderung (zusätzlich), Basissinstruktion ist definiert in: Konfigurieren -> Aufforderungen -> Agent: Systeminstruktion
 preset.temperature = Temperatur
 preset.untitled = (unbetitelt)
 preset.use = Verwenden
 preset.user_name = Benutzername
 preset.vision = Vision
 profile.current.suffix = (aktuell)
 screenshot.capture.name.prefix = Screenshot von
@@ -566,14 +574,16 @@
 settings.ctx.sources = Zeige Llama-Indexquellen
 settings.ctx.sources.desc = Falls aktiviert, werden die genutzten Quellen in der Antwort angezeigt (falls verfügbar, funktioniert nicht im gestreamten Chat)
 settings.defaults.app.confirm = Werksseitige App-Einstellungen laden?
 settings.defaults.user.confirm = Aktuelle Änderungen rückgängig machen?
 settings.download.dir = Verzeichnis für Dateidownloads
 settings.download.dir.desc = Unterordner für heruntergeladene Dateien, z.B. im Assistentenmodus, innerhalb von "data"
 settings.dict.delete.confirm = Eintrag aus der Liste entfernen?
+settings.experts.mode = Untermodus für Experten
+settings.experts.mode.desc = Untermodus, der für Experten verwendet wird (Chat, Vervollständigung, Langkette, Llama_Index, usw.)
 settings.font_size.tip = Tipp: Sie können die Schriftgröße ändern, indem Sie STRG + Mausrad verwenden
 settings.font_size = Schriftgröße (Chat-Text, Notizblöcke)
 settings.font_size.ctx = Schriftgröße (Kontextliste)
 settings.font_size.input = Schriftgröße (Eingabe)
 settings.font_size.toolbox = Schriftgröße (Werkzeugkasten)
 settings.frequency_penalty = Frequenzstrafe
 settings.img_prompt_model = DALL-E: Modell zur Prompterzeugung
@@ -618,22 +628,26 @@
 settings.notepad.num = Anzahl der Notizblöcke
 settings.organization_key = OpenAI ORGANISATIONSKEY
 settings.presence_penalty = Anwesenheitsstrafe
 settings.prompt.agent.continue = Agent: fortsetzen
 settings.prompt.agent.continue.desc = Aufforderung zur automatischen Fortsetzung des Gesprächs
 settings.prompt.agent.goal = Agent: Zielaktualisierung
 settings.prompt.agent.goal.desc = Anweisung zur Aktualisierung des aktuellen Zielstatus
+settings.prompt.agent.instruction = Agent: Systeminstruktion
+settings.prompt.agent.instruction.desc = Aufforderung zur Anleitung, wie man den autonomen Modus handhabt
 settings.prompt.cmd = Befehlsausführung: Anweisung
 settings.prompt.cmd.desc = Platzhalter: {schema}, {extra}
 settings.prompt.cmd.extra = Befehlsausführung: zusätzliches Nachwort (Nicht-Assistent-Modi)
 settings.prompt.cmd.extra.assistants = Befehlsausführung: zusätzliches Nachwort (nur im Assistentenmodus)
 settings.prompt.cmd.extra.assistants.desc = Zusätzliche Anweisungen zur Trennung lokaler Befehle von der bereits konfigurierten entfernten Umgebung in den Assistenten.
 settings.prompt.ctx.auto_summary.system = Kontext: Auto-Zusammenfassung (Systemaufforderung)
 settings.prompt.ctx.auto_summary.user = Kontext: Auto-Zusammenfassung (Benutzernachricht)
 settings.prompt.ctx.auto_summary.user.desc = Platzhalter: {input}, {output}
+settings.prompt.expert = Experte: Masteraufforderung
+settings.prompt.expert.desc = Anweisung (Systemaufforderung) für den Master-Experten, wie man Sklavenexperten handhabt. Anweisungen für Sklavenexperten werden aus ihren Voreinstellungen gegeben.
 settings.prompt.img = DALL-E: Bildgenerierung
 settings.prompt.img.desc = Aufforderung zur Erzeugung von Anweisungen für DALL-E (falls Rohmodus deaktiviert ist). Nur im Bildmodus.
 settings.render.code_syntax = Stil der Syntaxhervorhebung für Code
 settings.render.plain = Markdown-Formatierung in der Ausgabe deaktivieren (RAW-Textmodus)
 settings.restart.required = Ein Neustart der Anwendung ist notwendig, damit die Änderungen für diese Option übernommen werden.
 settings.section.agent = Agent (autonom)
 settings.section.files = Dateien und Anhänge
@@ -746,14 +760,16 @@
 tool.indexer.tab.web.help = Hilfe
 tool.indexer.tab.web.loader = Datenlader
 tool.indexer.tab.web.source = Datenquelle
 tool.indexer.tab.web.tip = Wählen Sie einen Datenlader aus und definieren Sie die Laderparameter, um externe Daten aus dem Web einzubetten.
 tool.indexer.title = Indexierer
 toolbox.agent.auto_stop.label = Automatischer Stopp
 toolbox.agent.iterations.label = Durchlaufschritte (Iterationen, 0 = unendlich)
+toolbox.agents.label = Agenten
+toolbox.experts.label = Experten
 toolbox.assistants.label = Assistenten
 toolbox.indexes.label = Indizes
 toolbox.img_variants.label = Anzahl der zu generierenden Bildvarianten
 toolbox.mode.label = Modus
 toolbox.model.label = Modell
 toolbox.name.ai = KI-Name
 toolbox.name.user = Benutzername
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.en.ini`

 * *Files 3% similar despite different names*

```diff
@@ -585,14 +585,16 @@
 menu.video = Video
 menu.video.capture = Input: camera
 menu.video.capture.auto = Auto capture
 mode.agent = Agent (autonomous)
 mode.assistant = Assistant
 mode.chat = Chat
 mode.completion = Completion
+mode.expert = Experts (co-op)
+mode.expert.tooltip = Experts to call in background
 mode.img = Image (DALL-E)
 mode.langchain = Langchain
 mode.llama_index = Chat with files
 mode.vision = Vision
 mode.agent.tooltip = Autonomous agents
 mode.assistant.tooltip = Chat using Assistants API
 mode.chat.tooltip = Chat mode (default)
@@ -647,27 +649,33 @@
 painter.btn.clear = Clear
 painter.capture.name.prefix = Drawing from
 painter.capture.manual.captured.success = Image captured:
 plugin.tab.general = General
 preset.action.delete = Delete
 preset.action.duplicate = Duplicate
 preset.action.edit = Edit
+preset.action.enable = Enable
+preset.action.disable = Disable
 preset.agent = Agent
 preset.ai_name = AI name
 preset.assistant = Assistant
 preset.chat = Chat
 preset.clear = Clear
 preset.completion = Completion
+preset.expert = Experts
+preset.experts.available.label = Available experts
+preset.experts.selected.label = Assigned experts (this agent)
 preset.filename = ID (filename)
 preset.img = Image
 preset.langchain = Langchain
 preset.llama_index = Chat with files
 preset.name = Preset Name
 preset.new = Create
 preset.prompt = System prompt
+preset.prompt.agent = Agent system prompt (additional), base instruction is defined in: Config -> Prompts -> Agent: system instruction
 preset.prompt.paste_template = Paste from template...
 preset.temperature = Temperature
 preset.tool.function = Functions
 preset.untitled = (untitled)
 preset.use = Use
 preset.user_name = User name
 preset.vision = Vision
@@ -712,14 +720,16 @@
 settings.ctx.use_extra.desc = If enabled, plain text output (if available) from command results will be displayed alongside the JSON output.
 settings.developer.debug = Show debug menu
 settings.defaults.app.confirm = Load factory app settings?
 settings.defaults.user.confirm = Undo current changes?
 settings.dict.delete.confirm = Remove item from list?
 settings.download.dir = Directory for file downloads
 settings.download.dir.desc = Subdirectory for downloaded files, e.g. in Assistants mode, inside "data"
+settings.experts.mode = Sub-mode for experts
+settings.experts.mode.desc = Sub-mode to use for Experts (chat, completion, langchain, llama_index, etc.)
 settings.font_size.tip = Tip: You can change the font size using CTRL + Mouse Wheel
 settings.font_size = Font size (chat plain-text, notepads)
 settings.font_size.ctx = Font size (ctx list)
 settings.font_size.input = Font size (input)
 settings.font_size.toolbox = Font size (toolbox)
 settings.frequency_penalty = Frequency Penalty
 settings.img_prompt_model = DALL-E: prompt generation model
@@ -782,22 +792,26 @@
 settings.notepad.num = Number of notepads
 settings.organization_key = OpenAI ORGANIZATION KEY
 settings.presence_penalty = Presence Penalty
 settings.prompt.agent.continue = Agent: continue
 settings.prompt.agent.continue.desc = Prompt sent to automatically continue the conversation
 settings.prompt.agent.goal = Agent: goal update
 settings.prompt.agent.goal.desc = Prompt to instruct how to update current goal status
+settings.prompt.agent.instruction = Agent: system instruction
+settings.prompt.agent.instruction.desc = Prompt to instruct how to handle autonomous mode
 settings.prompt.cmd = Command execute: instruction
 settings.prompt.cmd.desc = Placeholders: {schema}, {extra}
 settings.prompt.cmd.extra = Command execute: extra footer (non-Assistant modes)
 settings.prompt.cmd.extra.assistants = Command execute: extra footer (Assistant mode only)
 settings.prompt.cmd.extra.assistants.desc = Additional instructions to separate local commands from the remote environment that is already configured in the Assistants.
 settings.prompt.ctx.auto_summary.system = Context: auto-summary (system prompt)
 settings.prompt.ctx.auto_summary.user = Context: auto-summary (user message)
 settings.prompt.ctx.auto_summary.user.desc = Placeholders: {input}, {output}
+settings.prompt.expert = Expert: Master prompt
+settings.prompt.expert.desc = Instruction (system prompt) for Master expert how to handle slave experts. Instructions for slave experts are given from their presets.
 settings.prompt.img = DALL-E: image generate
 settings.prompt.img.desc = Prompt for generating prompts for DALL-E (if raw-mode is disabled). Image mode only.
 settings.render.engine = Rendering engine
 settings.render.open_gl = OpenGL hardware acceleration
 settings.render.web.only.desc = WebEngine / Chromium rendering engine only
 settings.render.code_syntax = Code syntax highlight
 settings.render.plain = Disable markdown formatting in output (RAW plain text mode)
@@ -924,15 +938,17 @@
 tool.indexer.tab.web.help = Help
 tool.indexer.tab.web.loader = Loader
 tool.indexer.tab.web.source = Data source
 tool.indexer.tab.web.tip = Select a data loader and define the loader parameters to embed external data from the web.
 tool.indexer.title = Indexer
 toolbox.agent.auto_stop.label = Auto-stop
 toolbox.agent.iterations.label = Run steps (iterations, 0 = infinity)
+toolbox.agents.label = Agents
 toolbox.assistants.label = Assistants
+toolbox.experts.label = Experts
 toolbox.indexes.label = Indexes
 toolbox.img_variants.label = Number of image variants to generate
 toolbox.llama_index.label = Llama-index
 toolbox.mode.label = Mode
 toolbox.model.label = Model
 toolbox.name.ai = AI Name
 toolbox.name.user = User Name
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.es.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.es.ini`

 * *Files 1% similar despite different names*

```diff
@@ -475,14 +475,16 @@
 menu.tray.screenshot = Preguntar con captura de pantalla...
 menu.tray.scheduled = Trabajos programados
 menu.video = Vídeo
 menu.video.capture = Entrada: cámara
 menu.video.capture.auto = Captura automática
 mode.agent = Agente (autónomo)
 mode.assistant = Asistente
+mode.expert = Expertos (cooperación)
+mode.expert.tooltip = Llamar a expertos en segundo plano
 mode.chat = Chat
 mode.completion = Finalización
 mode.img = Imagen (DALL-E)
 mode.langchain = Langchain
 mode.vision = Visión
 mode.llama_index = Chat con archivos
 mode.agent.tooltip = Agentes autónomos
@@ -514,19 +516,25 @@
 painter.btn.clear = Limpiar
 painter.capture.name.prefix = Dibujo de
 painter.capture.manual.captured.success = Imagen capturada:
 plugin.tab.general = General
 preset.action.delete = Eliminar
 preset.action.duplicate = Duplicar
 preset.action.edit = Editar
+preset.action.enable = Habilitar
+preset.action.disable = Deshabilitar
 preset.ai_name = Nombre de la IA
 preset.assistant = Asistente
 preset.chat = Chat
 preset.clear = Limpiar
 preset.completion = Finalización
+preset.expert = Expertos
+preset.experts.available.label = Expertos disponibles
+preset.experts.selected.label = Expertos asignados (este agente)
+preset.prompt.agent = Prompt del sistema del agente (adicional), la instrucción base está definida en: Configuración -> Prompts -> Agente: instrucción del sistema
 preset.filename = ID (nombre del archivo)
 preset.img = Imagen
 preset.langchain = Langchain
 preset.llama_index = Chat con archivos
 preset.name = Nombre del ajuste preestablecido
 preset.new = Crear
 preset.prompt = Indicación del sistema
@@ -565,14 +573,16 @@
 settings.ctx.sources = Mostrar fuentes del índice Llama
 settings.ctx.sources.desc = Si está habilitado, las fuentes utilizadas se mostrarán en la respuesta (si están disponibles, no funcionará en el chat en vivo)
 settings.defaults.app.confirm = ¿Cargar ajustes predeterminados de la aplicación?
 settings.defaults.user.confirm = ¿Deshacer cambios actuales?
 settings.dict.delete.confirm = ¿Eliminar elemento de la lista?
 settings.download.dir = Directorio para descargas de archivos
 settings.download.dir.desc = Subdirectorio para archivos descargados, por ejemplo, en modo Asistentes, dentro de "data"
+settings.experts.mode = Submodo para expertos
+settings.experts.mode.desc = Submodo a utilizar para Expertos (chat, completado, langchain, índice de llama, etc.)
 settings.font_size.tip = Consejo: Puedes cambiar el tamaño de la fuente usando CTRL + Rueda del ratón
 settings.font_size = Tamaño de fuente (texto plano de chat, bloc de notas)
 settings.font_size.ctx = Tamaño de fuente (lista ctx)
 settings.font_size.input = Tamaño de fuente (entrada)
 settings.font_size.toolbox = Tamaño de fuente (caja de herramientas)
 settings.frequency_penalty = Penalización de frecuencia
 settings.img_prompt_model = DALL-E: modelo de generación de indicaciones
@@ -618,22 +628,26 @@
 settings.notepad.num = Número de bloc de notas
 settings.organization_key = Clave de organización de OpenAI
 settings.presence_penalty = Penalización de presencia
 settings.prompt.agent.continue = Agente: continuar
 settings.prompt.agent.continue.desc = Mensaje enviado para continuar automáticamente la conversación
 settings.prompt.agent.goal = Agente: actualización de objetivo
 settings.prompt.agent.goal.desc = Mensaje para instruir cómo actualizar el estado actual del objetivo
+settings.prompt.agent.instruction = Agente: instrucción del sistema
+settings.prompt.agent.instruction.desc = Prompt para instruir cómo manejar el modo autónomo
 settings.prompt.cmd = Ejecutar comando: instrucción
 settings.prompt.cmd.desc = Marcadores de posición: {schema}, {extra}
 settings.prompt.cmd.extra = Ejecutar comando: pie de página extra (modos no asistente)
 settings.prompt.cmd.extra.assistants = Ejecutar comando: pie de página extra (solo modo asistente)
 settings.prompt.cmd.extra.assistants.desc = Instrucciones adicionales para separar los comandos locales del entorno remoto que ya está configurado en los Asistentes.
 settings.prompt.ctx.auto_summary.system = Contexto: resumen automático (prompt del sistema)
 settings.prompt.ctx.auto_summary.user = Contexto: resumen automático (mensaje del usuario)
 settings.prompt.ctx.auto_summary.user.desc = Marcadores de posición: {input}, {output}
+settings.prompt.expert = Experto: Master prompt
+settings.prompt.expert.desc = Instrucción (prompt del sistema) para el experto Master cómo manejar a los expertos subordinados. Las instrucciones para los expertos subordinados se dan desde sus presets.
 settings.prompt.img = DALL-E: generación de imagen
 settings.prompt.img.desc = Mensaje para generar comandos para DALL-E (si el modo crudo está desactivado). Solo modo de imagen.
 settings.render.code_syntax = Estilo de resaltado de sintaxis de código
 settings.render.plain = Desactivar el formato markdown en la salida (modo de texto plano RAW)
 settings.restart.required = Es necesario reiniciar la aplicación para que los cambios en esta opción se apliquen.
 settings.section.agent = Agente (autónomo)
 settings.section.files = Archivos y adjuntos
@@ -746,14 +760,16 @@
 tool.indexer.tab.web.help = Ayuda
 tool.indexer.tab.web.loader = Cargador
 tool.indexer.tab.web.source = Fuente de datos
 tool.indexer.tab.web.tip = Seleccione un cargador de datos y defina los parámetros del cargador para incrustar datos externos de la web.
 tool.indexer.title = Indexador
 toolbox.agent.auto_stop.label = Auto-parada
 toolbox.agent.iterations.label = Pasos de ejecución (iteraciones, 0 = infinito)
+toolbox.agents.label = Agentes
+toolbox.experts.label = Expertos
 toolbox.assistants.label = Asistentes
 toolbox.indexes.label = Índices
 toolbox.img_variants.label = Número de variantes de imagen a generar
 toolbox.mode.label = Modo
 toolbox.model.label = Modelo
 toolbox.name.ai = Nombre de la IA
 toolbox.name.user = Nombre de usuario
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.fr.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.fr.ini`

 * *Files 2% similar despite different names*

```diff
@@ -483,14 +483,16 @@
 mode.chat = Chat
 mode.completion = Complétion
 mode.img = Image (DALL-E)
 mode.langchain = Langchain
 mode.vision = Vision
 mode.llama_index = Chat avec fichiers
 mode.agent.tooltip = Agents autonomes
+mode.expert = Experts (co-opération)
+mode.expert.tooltip = Appeler des experts en arrière-plan
 mode.assistant.tooltip = Discuter via l'API des Assistants
 mode.chat.tooltip = Mode chat (par défaut)
 mode.completion.tooltip = Mode de complétion
 mode.img.tooltip = Génération d'image avec DALL-E
 mode.langchain.tooltip = Discussion avec les modèles fournis par Langchain
 mode.llama_index.tooltip = Discussion avec un contexte supplémentaire fourni par Llama-index
 mode.vision.tooltip = Analyse d'image avec GPT-4 Vision
@@ -514,27 +516,33 @@
 painter.btn.clear = Effacer
 painter.capture.name.prefix = Dessin de
 painter.capture.manual.captured.success = Image capturée:
 plugin.tab.general = Général
 preset.action.delete = Supprimer
 preset.action.duplicate = Dupliquer
 preset.action.edit = Modifier
+preset.action.enable = Activer
+preset.action.disable = Désactiver
 preset.ai_name = Nom de l'IA
 preset.assistant = Assistant
 preset.chat = Chat
 preset.clear = Effacer
 preset.completion = Complétion
+preset.expert = Experts
+preset.experts.available.label = Experts disponibles
+preset.experts.selected.label = Experts assignés (cet agent)
 preset.filename = ID (nom de fichier)
 preset.img = Image
 preset.langchain = Langchain
 preset.llama_index = Chat avec fichiers
 preset.name = Nom du préréglage
 preset.new = Créer
 preset.prompt = Invite du système
 preset.prompt.paste_template: Coller à partir du modèle...
+preset.prompt.agent = Prompt système d'agent (complémentaire), l'instruction de base est définie dans : Configuration -> Prompts -> Agent : instruction système
 preset.temperature = Température
 preset.untitled = (sans titre)
 preset.use = Utiliser
 preset.user_name = Nom de l'utilisateur
 preset.vision = Vision
 profile.current.suffix = (actuel)
 screenshot.capture.name.prefix = Capture d'écran de
@@ -565,14 +573,16 @@
 settings.ctx.sources = Afficher les sources de l'index Llama
 settings.ctx.sources.desc = Si activé, les sources utilisées seront affichées dans la réponse (si disponibles, cela ne fonctionnera pas dans le chat en continu)
 settings.defaults.app.confirm = Charger les réglages par défaut de l'application ?
 settings.defaults.user.confirm = Annuler les modifications actuelles ?
 settings.dict.delete.confirm = Supprimer l'élément de la liste ?
 settings.download.dir = Répertoire pour les téléchargements de fichiers
 settings.download.dir.desc = Sous-répertoire pour les fichiers téléchargés, par exemple en mode Assistants, à l'intérieur de "data"
+settings.experts.mode = Sous-mode pour les experts
+settings.experts.mode.desc = Sous-mode utilisé pour les Experts (chat, complétion, langchain, llama_index, etc.)
 settings.font_size.tip = Astuce : Vous pouvez changer la taille de la police en utilisant CTRL + Molette de la souris
 settings.font_size = Taille de police (texte brut de chat, blocs-notes)
 settings.font_size.ctx = Taille de police (liste ctx)
 settings.font_size.input = Taille de police (entrée)
 settings.font_size.toolbox = Taille de police (boîte à outils)
 settings.frequency_penalty = Pénalité de fréquence
 settings.img_prompt_model = DALL-E : modèle de génération d'invite
@@ -618,22 +628,26 @@
 settings.notepad.num = Nombre de blocs-notes
 settings.organization_key = Clé d'organisation OpenAI
 settings.presence_penalty = Pénalité de présence
 settings.prompt.agent.continue = Agent : continuer
 settings.prompt.agent.continue.desc = Prompt envoyé pour continuer automatiquement la conversation
 settings.prompt.agent.goal = Agent : mise à jour de l'objectif
 settings.prompt.agent.goal.desc = Prompt pour indiquer comment mettre à jour le statut de l'objectif actuel
+settings.prompt.agent.instruction = Agent : instruction système
+settings.prompt.agent.instruction.desc = Prompt pour instruire comment gérer le mode autonome
 settings.prompt.cmd = Exécuter une commande: instruction
 settings.prompt.cmd.desc = Espaces réservés: {schema}, {extra}
 settings.prompt.cmd.extra = Exécuter une commande: pied de page supplémentaire (modes non-Assistant)
 settings.prompt.cmd.extra.assistants = Exécuter une commande: pied de page supplémentaire (mode Assistant uniquement)
 settings.prompt.cmd.extra.assistants.desc = Instructions supplémentaires pour séparer les commandes locales de l'environnement à distance qui est déjà configuré dans les Assistants.
 settings.prompt.ctx.auto_summary.system = Contexte: résumé automatique (prompt système)
 settings.prompt.ctx.auto_summary.user = Contexte: résumé automatique (message utilisateur)
 settings.prompt.ctx.auto_summary.user.desc = Espaces réservés: {input}, {output}
+settings.prompt.expert = Expert : Master prompt
+settings.prompt.expert.desc = Instruction (prompt système) pour l'expert Master sur comment gérer les experts esclaves. Les instructions pour les experts esclaves sont données à partir de leurs presets.
 settings.prompt.img = DALL-E: génération d'image
 settings.prompt.img.desc = Prompt pour générer des commandes pour DALL-E (si le mode brut est désactivé). Mode image uniquement.
 settings.render.code_syntax = Style de mise en évidence de la syntaxe du code
 settings.render.plain = Désactiver le formatage markdown dans la sortie (mode texte brut RAW)
 settings.restart.required = Un redémarrage de l'application est requis pour que les modifications de cette option soient appliquées.
 settings.section.agent = Agent (autonome)
 settings.section.files = Fichiers et pièces jointes
@@ -746,14 +760,16 @@
 tool.indexer.tab.web.help = Aide
 tool.indexer.tab.web.loader = Chargeur de données
 tool.indexer.tab.web.source = Source de données
 tool.indexer.tab.web.tip = Sélectionnez un chargeur de données et définissez les paramètres du chargeur pour intégrer des données externes provenant du web.
 tool.indexer.title = Indexeur
 toolbox.agent.auto_stop.label = Arrêt automatique
 toolbox.agent.iterations.label = Nombre de pas (itérations, 0 = infini)
+toolbox.agents.label = Agents
+toolbox.experts.label = Experts
 toolbox.assistants.label = Assistants
 toolbox.indexes.label = Index
 toolbox.img_variants.label = Nombre de variantes d'image à générer
 toolbox.mode.label = Mode
 toolbox.model.label = Modèle
 toolbox.name.ai = Nom de l'IA
 toolbox.name.user = Nom de l'utilisateur
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.it.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.it.ini`

 * *Files 1% similar despite different names*

```diff
@@ -478,14 +478,16 @@
 menu.video = Video
 menu.video.capture = Ingresso: fotocamera
 menu.video.capture.auto = Cattura automatica
 mode.agent = Agente (autonomo)
 mode.assistant = Assistente
 mode.chat = Chat
 mode.completion = Completamento
+mode.expert = Esperti (cooperazione)
+mode.expert.tooltip = Chiamare esperti in background
 mode.img = Immagine (DALL-E)
 mode.langchain = Langchain
 mode.vision = Vision
 mode.llama_index = Chat con file
 mode.agent.tooltip = Agenti autonomi
 mode.assistant.tooltip = Chattare utilizzando l'API degli Assistenti
 mode.chat.tooltip = Modalità chat (predefinita)
@@ -514,28 +516,34 @@
 painter.btn.camera.capture = Dalla fotocamera
 painter.btn.clear = Pulire
 painter.capture.name.prefix = Disegno da
 painter.capture.manual.captured.success = Immagine catturata:
 plugin.tab.general = Generale
 preset.action.delete = Elimina
 preset.action.duplicate = Duplica
+preset.action.enable = Abilitare
+preset.action.disable = Disabilitare
 preset.action.edit = Modifica
 preset.ai_name = Nome dell'AI
 preset.assistant = Assistente
 preset.chat = Chat
 preset.clear = Pulisci
 preset.completion = Completamento
+preset.expert = Esperti
+preset.experts.available.label = Esperti disponibili
+preset.experts.selected.label = Esperti assegnati (questo agente)
 preset.filename = ID (nome del file)
 preset.img = Immagine
 preset.langchain = Langchain
 preset.llama_index = Chat con file
 preset.name = Nome del preset
 preset.new = Crea
 preset.prompt = Prompt del sistema
 preset.prompt.paste_template: Incolla dal modello...
+preset.prompt.agent = Prompt del sistema dell'agente (aggiuntivo), l'istruzione di base è definita in: Config -> Prompts -> Agente: istruzione di sistema
 preset.temperature = Temperatura
 preset.untitled = (senza titolo)
 preset.use = Usa
 preset.user_name = Nome dell'utente
 preset.vision = Visione
 profile.current.suffix = (corrente)
 screenshot.capture.name.prefix = Screenshot da
@@ -566,14 +574,16 @@
 settings.ctx.sources = Mostra le fonti dell'indice Llama
 settings.ctx.sources.desc = Se abilitato, le fonti utilizzate saranno mostrate nella risposta (se disponibili, non funzionerà nella chat in streaming)
 settings.defaults.app.confirm = Caricare le impostazioni predefinite dell'applicazione?
 settings.defaults.user.confirm = Annullare le modifiche correnti?
 settings.dict.delete.confirm = Rimuovere l'elemento dall'elenco?
 settings.download.dir = Directory per il download dei file
 settings.download.dir.desc = Sottodirectory per i file scaricati, ad esempio in modalità Assistenti, all'interno di "data"
+settings.experts.mode = Sottomodalità per esperti
+settings.experts.mode.desc = Sottomodalità da utilizzare per gli Esperti (chat, completamento, langchain, indice di llama, ecc.)
 settings.font_size.tip = Suggerimento: Puoi cambiare la dimensione del carattere usando CTRL + Rotellina del mouse
 settings.font_size = Dimensione del carattere (testo semplice della chat, blocchi appunti)
 settings.font_size.ctx = Dimensione del carattere (lista dei contesti)
 settings.font_size.input = Dimensione del carattere (input)
 settings.font_size.toolbox = Dimensione del carattere (toolbox)
 settings.frequency_penalty = Penale di frequenza
 settings.img_prompt_model = DALL-E: modello di generazione del prompt
@@ -619,22 +629,26 @@
 settings.notepad.num = Numero di blocchi note
 settings.organization_key = OpenAI ORGANIZATION KEY
 settings.presence_penalty = Penale di presenza
 settings.prompt.agent.continue = Agente: continua
 settings.prompt.agent.continue.desc = Prompt inviato per continuare automaticamente la conversazione
 settings.prompt.agent.goal = Agente: aggiornamento dell'obiettivo
 settings.prompt.agent.goal.desc = Prompt per istruire come aggiornare lo stato dell'obiettivo corrente
+settings.prompt.agent.instruction = Agente: istruzione di sistema
+settings.prompt.agent.instruction.desc = Prompt per istruire come gestire la modalità autonoma
 settings.prompt.cmd = Esegui comando: istruzione
 settings.prompt.cmd.desc = Placeholder: {schema}, {extra}
 settings.prompt.cmd.extra = Esegui comando: piè di pagina extra (modalità non assistente)
 settings.prompt.cmd.extra.assistants = Esegui comando: piè di pagina extra (solo modalità assistente)
 settings.prompt.cmd.extra.assistants.desc = Istruzioni aggiuntive per separare i comandi locali dall'ambiente remoto già configurato negli Assistenti.
 settings.prompt.ctx.auto_summary.system = Contesto: auto-riassunto (prompt del sistema)
 settings.prompt.ctx.auto_summary.user = Contesto: auto-riassunto (messaggio dell'utente)
 settings.prompt.ctx.auto_summary.user.desc = Placeholder: {input}, {output}
+settings.prompt.expert = Esperto: Master prompt
+settings.prompt.expert.desc = Istruzione (prompt del sistema) per l'esperto Master su come gestire gli esperti subalterni. Le istruzioni per gli esperti subalterni sono date dalle loro preimpostazioni.
 settings.prompt.img = DALL-E: generazione immagine
 settings.prompt.img.desc = Prompt per generare comandi per DALL-E (se la modalità grezza è disabilitata). Solo modalità immagine.
 settings.render.code_syntax = Stile di evidenziazione della sintassi del codice
 settings.restart.required = È necessario riavviare l'applicazione affinché le modifiche a questa opzione siano applicate.
 settings.section.agent = Agente (autonomo)
 settings.section.files = File e allegati
 settings.section.general = Generale
@@ -746,14 +760,16 @@
 tool.indexer.tab.web.help = Aiuto
 tool.indexer.tab.web.loader = Caricatore di dati
 tool.indexer.tab.web.source = Fonte dati
 tool.indexer.tab.web.tip = Seleziona un caricatore di dati e definisci i parametri del caricatore per incorporare dati esterni dal web.
 tool.indexer.title = Indicizzatore
 toolbox.agent.auto_stop.label = Arresto automatico
 toolbox.agent.iterations.label = Passi di esecuzione (iterazioni, 0 = infinito)
+toolbox.agents.label = Agenti
+toolbox.experts.label = Esperti
 toolbox.assistants.label = Assistenti
 toolbox.indexes.label = Indici
 toolbox.img_variants.label = Numero di varianti di immagine da generare
 toolbox.mode.label = Modalità
 toolbox.model.label = Modello
 toolbox.name.ai = Nome AI
 toolbox.name.user = Nome utente
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.pl.ini`

 * *Files 2% similar despite different names*

```diff
@@ -478,14 +478,16 @@
 menu.video = Wideo
 menu.video.capture = Wejście: kamera
 menu.video.capture.auto = Automatyczne przechwytywanie
 mode.agent = Agent (autonomiczny)
 mode.assistant = Asystent
 mode.chat = Czat
 mode.completion = Uzupełnianie
+mode.expert = Eksperci (współpraca)
+mode.expert.tooltip = Eksperci do wezwania w tle
 mode.img = Obraz (DALL-E)
 mode.langchain = Langchain
 mode.vision = Wizja
 mode.llama_index = Czat z plikami
 mode.agent.tooltip = Autonomiczni agenci
 mode.assistant.tooltip = Czat przy użyciu API Asystentów
 mode.chat.tooltip = Tryb czatu (domyślny)
@@ -514,27 +516,33 @@
 painter.btn.camera.capture = Z kamery
 painter.btn.clear = Wyczyść
 painter.capture.name.prefix = Drawing from
 painter.capture.manual.captured.success = Image captured:
 plugin.tab.general = Ogólne
 preset.action.delete = Usuń
 preset.action.duplicate = Duplikuj
+preset.action.enable = Włączyć
+preset.action.disable = Wyłączyć
 preset.action.edit = Edycja
 preset.ai_name = Imię AI
 preset.assistant = Asystent
 preset.chat = Czat (Chat)
 preset.clear = Wyczyść
 preset.completion = Uzupełnianie (Completion)
+preset.expert = Eksperci
+preset.experts.available.label = Dostępni eksperci
+preset.experts.selected.label = Przypisani eksperci (ten agent)
 preset.filename = ID (nazwa pliku)
 preset.img = Obraz (Image / DALL-E)
 preset.langchain = Langchain
 preset.llama_index = Czat z plikami
 preset.name = Nazwa presetu
 preset.new = Utwórz
 preset.prompt = Prompt systemowy
+preset.prompt.agent = Instrukcja systemowa agenta (dodatkowa), podstawowa instrukcja jest zdefiniowana w: Konfiguracja -> Wskazówki -> Agent: systemowa instrukcja
 preset.prompt.paste_template: Wklej z szablonu...
 preset.temperature = Temperatura
 preset.untitled = (bez nazwy)
 preset.use = Użyj
 preset.user_name = Imię użytkownika
 preset.vision = Wizja (Vision)
 profile.current.suffix = (bieżący)
@@ -566,14 +574,16 @@
 settings.ctx.sources = Pokaż źródła indeksu Llama
 settings.ctx.sources.desc = Jeśli opcja jest włączona, wykorzystane źródła będą wyświetlane w odpowiedzi (jeśli dostępne, nie zadziała w czacie z wł. opcją stream)
 settings.defaults.app.confirm = Wczytać fabryczne ustawienia aplikacji?
 settings.defaults.user.confirm = Przywrócić dokonane zmiany?
 settings.dict.delete.confirm = Usunąć pozycję z listy?
 settings.download.dir = Katalog na pliki do pobrania
 settings.download.dir.desc = Podkatalog na pobrane pliki, np. w trybie Asystentów, wewnątrz "data"
+settings.experts.mode = Podtryb dla ekspertów
+settings.experts.mode.desc = Podtryb używany dla Ekspertów (czat, uzupełnianie, langchain, llama_index, itp.)
 settings.font_size.tip = Wskazówka: Możesz zmienić rozmiar czcionki używając CTRL + Rolka myszy
 settings.font_size = Rozmiar czcionki (czat plain-text, notatniki)
 settings.font_size.ctx = Rozmiar czcionki (lista rozmów)
 settings.font_size.input = Rozmiar czcionki (wejście)
 settings.font_size.toolbox = Rozmiar czcionki (narzędzia)
 settings.frequency_penalty = Frequency Penalty
 settings.img_prompt_model = DALL-E: model do generowania promptów
@@ -619,22 +629,26 @@
 settings.notepad.num = Liczba notatników
 settings.organization_key = Klucz ORGANIZACJI OpenAI
 settings.presence_penalty = Presence Penalty
 settings.prompt.agent.continue = Agent: kontynuuj
 settings.prompt.agent.continue.desc = Prompt wysyłany do automatycznego kontynuowania rozmowy
 settings.prompt.agent.goal = Agent: aktualizacja celu
 settings.prompt.agent.goal.desc = Prompt instrukujący jak zaktualizować obecny status celu
+settings.prompt.agent.instruction = Agent: systemowa instrukcja
+settings.prompt.agent.instruction.desc = Wskazówka, jak obsługiwać tryb autonomiczny
 settings.prompt.cmd = Wykonaj polecenie: instrukcja
 settings.prompt.cmd.desc = Placeholdery: {schema}, {extra}
 settings.prompt.cmd.extra = Wykonaj polecenie: dodatkowa stopka (poza trybem Asystenta)
 settings.prompt.cmd.extra.assistants = Wykonaj polecenie: dodatkowa stopka (tryb Asystenta wyłącznie)
 settings.prompt.cmd.extra.assistants.desc = Dodatkowe instrukcje do oddzielenia lokalnych poleceń od zdalnego środowiska, które już jest skonfigurowane w Asystentach.
 settings.prompt.ctx.auto_summary.system = Kontekst: auto-podsumowanie (komunikat systemowy)
 settings.prompt.ctx.auto_summary.user = Kontekst: auto-podsumowanie (wiadomość użytkownika)
 settings.prompt.ctx.auto_summary.user.desc = Placeholdery: {input}, {output}
+settings.prompt.expert = Ekspert: Główna wskazówka
+settings.prompt.expert.desc = Instrukcja (systemowa wskazówka) dla głównego eksperta, jak obsługiwać ekspertów pomocniczych. Instrukcje dla ekspertów pomocniczych są podawane z ich ustawień.
 settings.prompt.img = DALL-E: generowanie obrazu
 settings.prompt.img.desc = Prompt do generowania poleceń dla DALL-E (jeśli surowy tryb jest wyłączony). Tylko tryb obrazu.
 settings.render.code_syntax = Styl podświetlenia składni kodu
 settings.render.plain = Wyłącz formatowanie markdown w wyjściu (tryb plain-text)
 settings.restart.required = Restart aplikacji jest wymagany, aby zmiany dla tej opcji zostały wprowadzone.
 settings.section.agent = Agent (autonomiczny)
 settings.section.files = Pliki i załączniki
@@ -747,14 +761,16 @@
 tool.indexer.tab.web.help = Pomoc
 tool.indexer.tab.web.loader = Ładowarka danych
 tool.indexer.tab.web.source = Źródło danych
 tool.indexer.tab.web.tip = Wybierz ładowarkę danych i zdefiniuj parametry ładowarki, aby osadzić zewnętrzne dane z internetu.
 tool.indexer.title = Indeksator
 toolbox.agent.auto_stop.label = Auto-stop
 toolbox.agent.iterations.label = Liczba kroków (iteracje, 0 = nieskończoność)
+toolbox.agents.label = Agenci
+toolbox.experts.label = Eksperci
 toolbox.assistants.label = Asystenci
 toolbox.indexes.label = Indeksy
 toolbox.img_variants.label = Ilość wariantów obrazów do wygenerowania
 toolbox.mode.label = Tryb
 toolbox.model.label = Model
 toolbox.name.ai = Imię AI
 toolbox.name.user = Imię użytkownika
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.uk.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.uk.ini`

 * *Files 1% similar despite different names*

```diff
@@ -478,14 +478,16 @@
 menu.video = Відео
 menu.video.capture = Вхід: камера
 menu.video.capture.auto = Автоматичне захоплення зображення
 mode.agent = Агент (автономний)
 mode.assistant = Помічник
 mode.chat = Чат
 mode.completion = Завершення
+mode.expert = Експерти (співпраця)
+mode.expert.tooltip = Виклик експертів на задній план
 mode.img = Зображення(DALL-E)
 mode.langchain = Langchain
 mode.vision = Оптика
 mode.llama_index = Чат з файлами
 mode.agent.tooltip = Автономні агенти
 mode.assistant.tooltip = Чат за допомогою API Асистентів
 mode.chat.tooltip = Режим чату (за замовчуванням)
@@ -515,27 +517,33 @@
 painter.btn.clear = Очистити
 painter.capture.name.prefix = Малюнок з
 painter.capture.manual.captured.success = Зображення захоплено:
 plugin.tab.general = Загальне
 preset.action.delete = Видалити
 preset.action.duplicate = Дублювати
 preset.action.edit = Редагувати
+preset.action.enable = Увімкнути
+preset.action.disable = Вимкнути
 preset.ai_name = Ім'я AI
 preset.assistant = Помічник
 preset.chat = Чат
 preset.clear = Очистити
 preset.completion = Завершення
+preset.expert = Експерти
+preset.experts.available.label = Доступні експерти
+preset.experts.selected.label = Призначені експерти (цей агент)
 preset.filename = ID (ім'я файлу)
 preset.img = Зображення
 preset.langchain = Langchain
 preset.llama_index = Чат з файлами
 preset.name = Ім'я пресета
 preset.new = Створити
 preset.prompt = Системний запит
 preset.prompt.paste_template: Вставити з шаблону...
+preset.prompt.agent = Системний запит агента (додатково), базова інструкція визначена в: Налаштування -> Запити -> Агент: системна інструкція
 preset.temperature = Температура
 preset.untitled = (без назви)
 preset.use = Використовувати
 preset.user_name = Ім'я користувача
 preset.vision = Оптика
 profile.current.suffix = (поточний)
 screenshot.capture.name.prefix = Скріншот з
@@ -566,14 +574,16 @@
 settings.ctx.sources = Показати джерела індексу Llama
 settings.ctx.sources.desc = Якщо включено, використані джерела будуть відображатися в відповіді (якщо доступно, не працюватиме в потоковому чаті)
 settings.defaults.app.confirm = Завантажити заводські налаштування додатку?
 settings.defaults.user.confirm = Відмінити поточні зміни?
 settings.dict.delete.confirm = Видалити елемент зі списку?
 settings.download.dir = Директорія для завантаження файлів
 settings.download.dir.desc = Піддиректорія для завантажених файлів, наприклад, у режимі помічників, всередині "data"
+settings.experts.mode = Підпрограма для експертів
+settings.experts.mode.desc = Підпрограма для використання експертами (чат, завершення, langchain, llama_index тощо)
 settings.font_size.tip = Підказка: Ви можете змінити розмір шрифту, використовуючи CTRL + Колесо миші
 settings.font_size = Розмір шрифту (звичайний текст чату, блокноти)
 settings.font_size.ctx = Розмір шрифту (список ctx)
 settings.font_size.input = Розмір шрифту (введення)
 settings.font_size.toolbox = Розмір шрифту (панель інструментів)
 settings.frequency_penalty = Частотний штраф
 settings.img_prompt_model = DALL-E: модель генерації запиту
@@ -619,23 +629,27 @@
 settings.notepad.num = Кількість блокнотів
 settings.organization_key = OpenAI ORGANIZATION KEY
 settings.presence_penalty = Штраф за наявність
 settings.prompt.agent.continue = Агент: продовжити
 settings.prompt.agent.continue.desc = Підказка, що надсилається для автоматичного продовження розмови
 settings.prompt.agent.goal = Агент: оновлення цілі
 settings.prompt.agent.goal.desc = Підказка, яка інструктує, як оновити поточний статус цілі
+settings.prompt.agent.instruction = Агент: системна інструкція
+settings.prompt.agent.instruction.desc = Запит для інструкції, як обробляти автономний режим
 settings.prompt.cmd = Виконання команди: інструкція
 settings.prompt.cmd.desc = Заповнювачі: {schema}, {extra}
 settings.prompt.cmd.extra = Виконання команди: додатковий низ (режими без Асистента)
 settings.prompt.cmd.extra.assistants = Виконання команди: додатковий низ (тільки режим Асистента)
 settings.prompt.cmd.extra.assistants.desc = Додаткові інструкції для відокремлення локальних команд від віддаленого середовища, яке вже налаштоване в Асистентах.
 settings.prompt.ctx.auto_summary.system = Контекст: авто-резюме (системний запит)
 settings.prompt.ctx.auto_summary.user = Контекст: авто-резюме (повідомлення користувача)
 settings.prompt.ctx.auto_summary.user.desc = Заповнювачі: {input}, {output}
 settings.prompt.img = DALL-E: генерація зображення
+settings.prompt.expert = Експерт: Основний запит
+settings.prompt.expert.desc = Інструкція (системний запит) для ведучого експерта, як керувати підеекспертами. Інструкції для підеекспертів даються з їхніх налаштувань.
 settings.prompt.img.desc = Підказка для генерації команддля DALL-E (якщо вимкнено сирівний режим). Тільки режим зображення.
 settings.render.code_syntax = Стиль підсвічування синтаксису коду
 settings.render.plain = Вимкнути форматування markdown у виводі (режим простого тексту RAW)
 settings.restart.required = Для внесення змін у цю опцію необхідно перезапустити програму.
 settings.section.agent = Агент (автономний)
 settings.section.files = Файли та вкладення
 settings.section.general = Загальні
@@ -747,14 +761,16 @@
 tool.indexer.tab.web.help = Допомога
 tool.indexer.tab.web.loader = Завантажувач даних
 tool.indexer.tab.web.source = Джерело даних
 tool.indexer.tab.web.tip = Виберіть завантажувач даних та визначте параметри завантажувача для вбудовування зовнішніх даних з вебу.
 tool.indexer.title = Індексатор
 toolbox.agent.auto_stop.label = Авто-стоп
 toolbox.agent.iterations.label = Кількість кроків (ітерації, 0 = нескінченність)
+toolbox.agents.label = Агенти
+toolbox.experts.label = Експерти
 toolbox.assistants.label = Помічники
 toolbox.indexes.label = Індекси
 toolbox.img_variants.label = Кількість варіантів зображень для генерації
 toolbox.mode.label = Режим
 toolbox.model.label = Модель
 toolbox.name.ai = Ім'я AI
 toolbox.name.user = Ім'я користувача
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/locale.zh.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/locale.zh.ini`

 * *Files 2% similar despite different names*

```diff
@@ -553,14 +553,16 @@
 menu.video = 視頻
 menu.video.capture = 輸入：相機
 menu.video.capture.auto = 自動捕捉
 mode.agent = 代理（自主）
 mode.assistant = 助手
 mode.chat = 聊天模式
 mode.completion = 完成模式
+mode.expert = 专家 (合作)
+mode.expert.tooltip = 背景中呼叫专家
 mode.img = 圖像（DALL-E）
 mode.langchain = Langchain模式
 mode.llama_index = 文件聊天模式
 mode.vision = 視覺模式
 mode.agent.tooltip = 自主代理
 mode.assistant.tooltip = 使用助手API進行聊天
 mode.chat.tooltip = 聊天模式（預設）
@@ -615,28 +617,34 @@
 painter.btn.clear= 清除
 painter.capture.name.prefix= 從繪畫捕獲的圖像
 painter.capture.manual.captured.success= 圖像捕獲：
 plugin.tab.general= 一般設置
 preset.action.delete= 刪除
 preset.action.duplicate= 複製
 preset.action.edit= 編輯
+preset.action.enable = 启用
+preset.action.disable = 禁用
 preset.agent= 代理模式预设参数设置
 preset.ai_name = AI名稱
 preset.assistant = 助手
 preset.chat = 聊天
 preset.clear = 清除
 preset.completion = 完成
+preset.expert = 专家团
+preset.experts.available.label = 可用专家
+preset.experts.selected.label = 分配专家 (该代理)
 preset.filename = ID（文件名）
 preset.img = 圖像
 preset.langchain = Langchain
 preset.llama_index = 文件聊天
 preset.name = 預設名稱
 preset.new = 創建
 preset.prompt = 系統提示
 preset.prompt.paste_template: 从模板粘贴...
+preset.prompt.agent = 代理系统提示（附加），基本指令定义在：配置 -> 提示 -> 代理：系统指令
 preset.temperature = 溫度
 preset.tool.function = 函數
 preset.untitled = （無標題）
 preset.use = 使用
 preset.user_name = 用戶名稱
 preset.vision = 視覺
 profile.current.suffix = （当前）
@@ -663,14 +671,16 @@
 settings.ctx.convert_lists = 将列表转换为段落
 settings.ctx.copy_code = 在代码块中显示“复制到剪贴板”
 settings.ctx.records.limit = 上下文列表中的最後上下文限制（0=無限制）
 settings.ctx.search_content = 也在對話內容中搜索，而不僅僅是標題中搜索
 settings.ctx.search.desc = 啟用在上下文項目內容中進行搜索的功能
 settings.ctx.sources = 显示Llama索引源
 settings.ctx.sources.desc = 如果启用，使用的源将在回应中显示（如果可用，不适用于流式聊天）
+settings.experts.mode = 专家子模式
+settings.experts.mode.desc = 用于专家的子模式（聊天、完成、语言链、llama_index等）
 settings.developer.debug= 顯示調試菜單
 settings.defaults.app.confirm= 加載工廠應用設置？
 settings.defaults.user.confirm= 撤銷當前更改？
 settings.dict.delete.confirm= 從列表中移除項目？
 settings.download.dir= 文件下載目錄
 settings.download.dir.desc= 下載文件的子目錄，例如在助手模式下，在"data"內部
 settings.font_size.tip= 提示：您可以使用CTRL + 滑鼠滾輪更改字體大小
@@ -729,22 +739,26 @@
 settings.notepad.num = 記事本數量
 settings.organization_key = OpenAI組織密鑰
 settings.presence_penalty = 存在處罰
 settings.prompt.agent.continue = 代理：继续
 settings.prompt.agent.continue.desc = 发送提示以自动继续对话
 settings.prompt.agent.goal = 代理：目标更新
 settings.prompt.agent.goal.desc = 指令提示如何更新当前目标状态
+settings.prompt.agent.instruction = 代理：系统指令
+settings.prompt.agent.instruction.desc = 提示如何处理自主模式的指令
 settings.prompt.cmd = 命令执行：指令
 settings.prompt.cmd.desc = 占位符：{schema}, {extra}
 settings.prompt.cmd.extra = 命令执行：额外页脚（非助理模式）
 settings.prompt.cmd.extra.assistants = 命令执行：额外页脚（仅助理模式）
 settings.prompt.cmd.extra.assistants.desc = 额外指令用于区分本地命令与已在助理中配置的远程环境。
 settings.prompt.ctx.auto_summary.system = 上下文：自动摘要（系统提示）
 settings.prompt.ctx.auto_summary.user = 上下文：自动摘要（用户信息）
 settings.prompt.ctx.auto_summary.user.desc = 占位符：{input}, {output}
+settings.prompt.expert = 专家：主提示
+settings.prompt.expert.desc = 对主专家如何处理奴隶专家的指令（系统提示）。奴隶专家的指令根据他们的预设给出。
 settings.prompt.img = DALL-E：生成图像
 settings.prompt.img.desc = 提示用于生成DALL-E的命令（如果原始模式被禁用）。仅图像模式。
 settings.render.code_syntax = 代码语法高亮样式
 settings.render.plain = 在輸出中禁用markdown格式化（RAW純文本模式）
 settings.restart.required = 此選項生效需要重新啟動應用程序。
 settings.section.agent = 代理（自主）
 settings.section.files = 文件和附件
@@ -864,14 +878,16 @@
 tool.indexer.tab.web.loader = 数据加载器
 tool.indexer.tab.web.source = 数据来源
 tool.indexer.tab.web.tip = 选择数据加载器并定义加载器参数，以便嵌入来自网络的外部数据。
 tool.indexer.title = 索引器
 toolbox.agent.auto_stop.label = 自動停止
 toolbox.agent.iterations.label = 運行步驟（迭代次數，0=無限）
 toolbox.assistants.label = 助手
+toolbox.agents.label = 代办
+toolbox.experts.label = 专家
 toolbox.indexes.label = 索引
 toolbox.img_variants.label = 生成圖像變體的數量
 toolbox.llama_index.label = Llama-index
 toolbox.mode.label = 模式
 toolbox.model.label = 模型
 toolbox.name.ai = AI名稱
 toolbox.name.user = 用戶名稱
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.agent.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.agent.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.agent.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.agent.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.audio_input.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_input.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.audio_input.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_input.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.audio_output.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_output.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.audio_output.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.audio_output.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_api.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_api.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_files.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_files.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_history.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_history.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_web.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_web.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.crontab.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.crontab.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.crontab.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.crontab.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.openai_vision.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.openai_vision.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.real_time.en.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.real_time.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/locale/plugin.real_time.pl.ini` & `pygpt_net-2.2.7/src/pygpt_net/data/locale/plugin.real_time.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/logo.png` & `pygpt_net-2.2.7/src/pygpt_net/data/logo.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/prompts.csv` & `pygpt_net-2.2.7/src/pygpt_net/data/prompts.csv`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/win32/README.rtf` & `pygpt_net-2.2.7/src/pygpt_net/data/win32/README.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/win32/USER-LICENSE.rtf` & `pygpt_net-2.2.7/src/pygpt_net/data/win32/USER-LICENSE.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/data/win32/pygpt.aip` & `pygpt_net-2.2.7/src/pygpt_net/data/win32/pygpt.aip`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/icons.qrc` & `pygpt_net-2.2.7/src/pygpt_net/icons.qrc`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/icons_rc.py` & `pygpt_net-2.2.7/src/pygpt_net/icons_rc.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/item/assistant.py` & `pygpt_net-2.2.7/src/pygpt_net/item/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/item/attachment.py` & `pygpt_net-2.2.7/src/pygpt_net/item/index.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,75 +2,64 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.26 23:00:00                  #
+# Updated Date: 2024.01.27 17:00:00                  #
 # ================================================== #
 
 import json
 
 
-class AttachmentItem:
+class IndexItem:
     def __init__(self):
         """
-        Attachment item
+        Index item
         """
-        self.name = None
         self.id = None
-        self.path = None
-        self.remote = None
-        self.vector_store_ids = []
-        self.size = 0
-        self.send = False
+        self.name = None
+        self.store = None
+        self.items = {}
 
     def serialize(self) -> dict:
         """
         Serialize item to dict
 
         :return: serialized item
         """
         return {
             'id': self.id,
             'name': self.name,
-            'path': self.path,
-            'size': self.size,
-            'remote': self.remote,
-            'vector_store_ids': self.vector_store_ids,
-            'send': self.send
+            'store': self.store,
+            'items': self.items,
         }
 
     def deserialize(self, data: dict):
         """
         Deserialize item from dict
 
         :param data: serialized item
         """
         if 'id' in data:
             self.id = data['id']
         if 'name' in data:
             self.name = data['name']
-        if 'path' in data:
-            self.path = data['path']
-        if 'size' in data:
-            self.size = data['size']
-        if 'remote_id' in data:
-            self.remote = data['remote']
-        if 'vector_store_ids' in data:
-            self.vector_store_ids = data['vector_store_ids']
-        if 'send' in data:
-            self.send = data['send']
+        if 'store' in data:
+            self.store = data['store']
+        if 'items' in data:
+            self.items = data['items']
 
-    def dump(self) -> str:
+    def dump(self):
         """
         Dump item to string
 
         :return: serialized item
+        :rtype: str
         """
         try:
             return json.dumps(self.serialize())
         except Exception as e:
             pass
         return ""
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/item/calendar_note.py` & `pygpt_net-2.2.7/src/pygpt_net/item/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/item/ctx.py` & `pygpt_net-2.2.7/src/pygpt_net/item/ctx.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.08 21:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import copy
 import datetime
 import json
 import time
 
@@ -55,14 +55,18 @@
         self.idx = 0
         self.first = False
         self.tool_calls = []  # API tool calls
         self.index_meta = {}  # llama-index metadata ctx used
         self.doc_ids = []  # document ids
         self.prev_ctx = None  # previous context (reply output)
         self.stopped = False  # run stopped
+        self.sub_calls = 0  # sub calls count
+        self.sub_call = False  # is sub call
+        self.sub_reply = False  # sub call reply
+        self.hidden = False  # hidden context
 
     def clear_reply(self):
         """Clear current reply output"""
         if self.reply:
             self.urls = []
 
     def from_previous(self):
@@ -150,14 +154,18 @@
             "internal": self.internal,
             "is_vision": self.is_vision,
             "idx": self.idx,
             "first": self.first,
             "tool_calls": self.tool_calls,
             "index_meta": self.index_meta,
             "doc_ids": self.doc_ids,
+            "sub_calls": 0,
+            "sub_call": False,
+            "sub_reply": False,
+            "hidden": False,
         }
 
     def from_dict(self, data: dict):
         """
         Load context item from dict
 
         :param data: dict
@@ -193,14 +201,18 @@
         self.internal = data.get("internal", False)
         self.is_vision = data.get("is_vision", False)
         self.idx = data.get("idx", 0)
         self.first = data.get("first", False)
         self.tool_calls = data.get("tool_calls", [])
         self.index_meta = data.get("index_meta", {})
         self.doc_ids = data.get("doc_ids", [])
+        self.sub_calls = data.get("sub_calls", 0)
+        self.sub_call = data.get("sub_call", False)
+        self.sub_reply = data.get("sub_reply", False)
+        self.hidden = data.get("hidden", False)
 
     def dump(self) -> str:
         """
         Dump context item to JSON string
 
         :return: JSON string
         """
@@ -243,14 +255,17 @@
         self.initialized = False
         self.deleted = False
         self.important = False
         self.archived = False
         self.label = 0  # label color
         self.indexes = {}  # indexes data
         self.group_id = None
+        self.root_id = None
+        self.parent_id = None
+        self.owner_uuid = None
 
     def to_dict(self) -> dict:
         """
         Dump context meta to dict
 
         :return: dict
         """
@@ -276,14 +291,17 @@
             "initialized": self.initialized,
             "deleted": self.deleted,
             "important": self.important,
             "archived": self.archived,
             "label": self.label,
             "indexes": self.indexes,
             "group_id": self.group_id,
+            "root_id": self.root_id,
+            "parent_id": self.parent_id,
+            "owner_uuid": self.owner_uuid,
         }
 
     def from_dict(self, data: dict):
         """
         Load context meta from dict
 
         :param data: dict
@@ -309,14 +327,17 @@
         self.initialized = data.get("initialized", False)
         self.deleted = data.get("deleted", False)
         self.important = data.get("important", False)
         self.archived = data.get("archived", False)
         self.label = data.get("label", 0)
         self.indexes = data.get("indexes", {})
         self.group_id = data.get("group_id", None)
+        self.root_id = data.get("root_id", None)
+        self.parent_id = data.get("parent_id", None)
+        self.owner_uuid = data.get("owner_uuid", None)
 
 class CtxGroup:
     def __init__(self, id=None, name=None):
         """
         Context group
 
         :param id: Group ID
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/item/mode.py` & `pygpt_net-2.2.7/src/pygpt_net/item/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/item/model.py` & `pygpt_net-2.2.7/src/pygpt_net/item/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/item/notepad.py` & `pygpt_net-2.2.7/src/pygpt_net/item/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/item/preset.py` & `pygpt_net-2.2.7/src/pygpt_net/item/preset.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,63 +2,77 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.02.14 16:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import json
+import uuid
 
 
 class PresetItem:
     def __init__(self):
+        self.uuid = None
         self.name = "*"
         self.ai_name = ""
         self.user_name = ""
         self.prompt = ""
         self.chat = False
         self.completion = False
         self.img = False
         self.vision = False
         self.langchain = False
         self.assistant = False
         self.llama_index = False
         self.agent = False
+        self.expert = False
         self.temperature = 1.0
         self.filename = None
         self.model = None
         self.version = None
+        self.experts = []  # agent mode
+        self.enabled = True
         self.tools = {
             "function": [],
         }
 
+    def get_id(self) -> str:
+        return self.filename
+
     def to_dict(self):
         return {
+            "uuid": str(self.uuid),
             "name": self.name,
             "ai_name": self.ai_name,
             "user_name": self.user_name,
             "prompt": self.prompt,
             "chat": self.chat,
             "completion": self.completion,
             "img": self.img,
             "vision": self.vision,
             "langchain": self.langchain,
             "assistant": self.assistant,
             "llama_index": self.llama_index,
             "agent": self.agent,
+            "expert": self.expert,
             "temperature": self.temperature,
             "filename": self.filename,
             "model": self.model,
             "tool.function": self.tools["function"],
+            "experts": self.experts,
+            "enabled": self.enabled,
         }
 
     def from_dict(self, data):
+        if "uuid" in data:
+            self.uuid = uuid.UUID(data["uuid"])
         if "name" in data:
             self.name = data["name"]
         if "ai_name" in data:
             self.ai_name = data["ai_name"]
         if "user_name" in data:
             self.user_name = data["user_name"]
         if "prompt" in data:
@@ -75,22 +89,28 @@
             self.langchain = data["langchain"]
         if "assistant" in data:
             self.assistant = data["assistant"]
         if "llama_index" in data:
             self.llama_index = data["llama_index"]
         if "agent" in data:
             self.agent = data["agent"]
+        if "expert" in data:
+            self.expert = data["expert"]
         if "temperature" in data:
             self.temperature = data["temperature"]
         if "filename" in data:
             self.filename = data["filename"]
         if "model" in data:
             self.model = data["model"]
         if "tool.function" in data:
             self.tools["function"] = data["tool.function"]
+        if "experts" in data:
+            self.experts = data["experts"]
+        if "enabled" in data:
+            self.enabled = data["enabled"]
         return self
 
     def add_function(self, name: str, parameters: str, desc: str):
         """
         Add function to preset
 
         :param name: function name
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/launcher.py` & `pygpt_net-2.2.7/src/pygpt_net/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/migrations/Version20231227152900.py` & `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20231227152900.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/migrations/Version20231230095000.py` & `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20231230095000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/migrations/Version20231231230000.py` & `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20231231230000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240106060000.py` & `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240106060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240107060000.py` & `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240107060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240222160000.py` & `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240222160000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240223050000.py` & `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240223050000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240303190000.py` & `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240303190000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240408180000.py` & `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240408180000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/migrations/Version20240426050000.py` & `pygpt_net-2.2.7/src/pygpt_net/migrations/Version20240426050000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/migrations/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/migrations/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.26 23:00:00                  #
+# Updated Date: 2024.05.01 03:00:00                  #
 # ================================================== #
 
 from .Version20231227152900 import Version20231227152900  # 2.0.59
 from .Version20231230095000 import Version20231230095000  # 2.0.66
 from .Version20231231230000 import Version20231231230000  # 2.0.71
 from .Version20240106060000 import Version20240106060000  # 2.0.84
 from .Version20240107060000 import Version20240107060000  # 2.0.88
 from .Version20240222160000 import Version20240222160000  # 2.0.162
 from .Version20240223050000 import Version20240223050000  # 2.0.163
 from .Version20240303190000 import Version20240303190000  # 2.1.8
 from .Version20240408180000 import Version20240408180000  # 2.1.41
 from .Version20240426050000 import Version20240426050000  # 2.1.79
+from .Version20240501030000 import Version20240501030000  # 2.2.7
 
 class Migrations:
     def __init__(self):
         pass
 
     @staticmethod
     def get_versions() -> list:
@@ -38,8 +39,9 @@
             Version20240106060000(),  # 2.0.84
             Version20240107060000(),  # 2.0.88
             Version20240222160000(),  # 2.0.162
             Version20240223050000(),  # 2.0.163
             Version20240303190000(),  # 2.1.8
             Version20240408180000(),  # 2.1.41
             Version20240426050000(),  # 2.1.79
+            Version20240501030000(),  # 2.2.7
         ]
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/migrations/base.py` & `pygpt_net-2.2.7/src/pygpt_net/migrations/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/agent/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/audio_input/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/audio_input/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/audio_input/simple.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/audio_input/simple.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/audio_input/worker.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/audio_input/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/audio_output/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/audio_output/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/audio_output/worker.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/audio_output/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/base.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_api/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_api/worker.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_api/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_code_interpreter/runner.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_code_interpreter/runner.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_code_interpreter/worker.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_code_interpreter/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_custom/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_custom/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_custom/worker.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_custom/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_files/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_files/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_files/worker.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_files/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_history/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_history/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_history/worker.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_history/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_serial/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_serial/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_serial/worker.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_serial/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_web/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_web/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_web/websearch.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_web/websearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/cmd_web/worker.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/cmd_web/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/crontab/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/crontab/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/extra_prompt/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/extra_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/idx_llama_index/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/idx_llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/idx_llama_index/worker.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/idx_llama_index/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/openai_dalle/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/openai_dalle/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/openai_vision/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/openai_vision/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/plugin/real_time/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/plugin/real_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/audio_input/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/audio_input/bing_speech_recognition.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/bing_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/audio_input/google_speech_recognition.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/google_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/audio_input/openai_whisper.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/openai_whisper.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/audio_input/openai_whisper_local.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/audio_input/openai_whisper_local.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/audio_output/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/audio_output/eleven_labs.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/audio_output/google_tts.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/google_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/audio_output/ms_azure_tts.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/ms_azure_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/audio_output/openai_tts.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/audio_output/openai_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant/json_file.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_file/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_store/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/assistant_store/json_file.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/assistant_store/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/attachment/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/attachment/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/attachment/json_file.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/attachment/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/calendar/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/config/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/config/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/config/json_file.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/config/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/config/patch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/config/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.29 07:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import copy
 import os
 
 from packaging.version import parse as parse_version, Version
 
@@ -1411,14 +1411,31 @@
             # < 2.2.2
             if old < parse_version("2.2.2"):
                 print("Migrating config from < 2.2.2...")
                 if 'app.env' not in data:
                     data["app.env"] = []
                 updated = True
 
+            # < 2.2.7
+            if old < parse_version("2.2.7"):
+                print("Migrating config from < 2.2.7...")
+                if 'prompt.agent.instruction' not in data:
+                    data["prompt.agent.instruction"] = ""
+                if 'prompt.expert' not in data:
+                    data["prompt.expert"] = ""
+                if 'experts.mode' not in data:
+                    data["experts.mode"] = "chat"
+                # from base
+                data["prompt.agent.instruction"] = self.window.core.config.get_base('prompt.agent.instruction')
+                data["prompt.agent.continue"] = self.window.core.config.get_base('prompt.agent.continue')
+                data["prompt.agent.goal"] = self.window.core.config.get_base('prompt.agent.goal')
+                data["prompt.expert"] = self.window.core.config.get_base('prompt.expert')
+                data["prompt.img"] = self.window.core.config.get_base('prompt.img')
+                updated = True
+
         # update file
         migrated = False
         if updated:
             data = dict(sorted(data.items()))
             self.window.core.config.data = data
             self.window.core.config.save()
             migrated = True
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/ctx/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.17 07:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import time
 from uuid import uuid4
 from packaging.version import Version
 
 from pygpt_net.item.ctx import CtxMeta, CtxItem, CtxGroup
@@ -287,14 +287,31 @@
         """
         Return dict of groups
 
         :return: dict of ctx meta
         """
         return self.storage.get_groups()
 
+    def get_meta_by_id(self, id: int) -> CtxMeta or None:
+        """
+        Get meta by ID
+
+        :param id: ctx ID
+        """
+        return self.storage.get_meta_by_id(id)
+
+    def get_meta_by_root_id_and_preset_id(self, root_id: int, preset_id: str):
+        """
+        Get meta by root ID and preset ID
+
+        :param root_id: root ID
+        :param preset_id: preset ID
+        """
+        return self.storage.get_meta_by_root_id_and_preset_id(root_id, preset_id)
+
     def insert_group(self, group: CtxGroup):
         """
         Insert group
 
         :param group: CtxGroup
         """
         return self.storage.insert_group(group)
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.08 21:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 from datetime import datetime
 import re
 import time
 
 from sqlalchemy import text
@@ -58,14 +58,17 @@
         :param append_date_ranges: append date ranges
         :return: where_statement, join_statement, bind_params
         """
         where_clauses = []
         join_clauses = []
         bind_params = {}
 
+        # only base by default
+        where_clauses.append("(m.root_id IS NULL OR m.root_id = 0)")
+
         # search_string
         if search_string:
             date_ranges = search_by_date_string(search_string)
             search_string = re.sub(
                 r'@date\((\d{4}-\d{2}-\d{2})?(,)?(\d{4}-\d{2}-\d{2})?\)',
                 '',
                 search_string.strip(),
@@ -180,14 +183,56 @@
             result = conn.execute(stmt)
             for row in result:
                 meta = CtxMeta()
                 unpack_meta(meta, row._asdict())
                 items[meta.id] = meta
         return items
 
+    def get_meta_by_root_id_and_preset_id(self, root_id: int, preset_id: str) -> dict:
+        """
+        Return dict with indexed CtxMeta objects, indexed by ID
+
+        :return: dict of CtxMeta
+        """
+        stmt_text = f"""
+            SELECT * FROM ctx_meta WHERE root_id = :root_id AND preset_id = :preset_id
+        """
+        stmt = text(stmt_text).bindparams(
+            root_id=root_id,
+            preset_id=preset_id,
+        )
+        items = {}
+        db = self.window.core.db.get_db()
+        with db.connect() as conn:
+            result = conn.execute(stmt)
+            for row in result:
+                meta = CtxMeta()
+                unpack_meta(meta, row._asdict())
+                items[meta.id] = meta
+        return items
+
+    def get_meta_by_id(self, id: int) -> CtxMeta or None:
+        """
+        Return ctx meta by ID
+
+        :return: CtxMeta
+        """
+        stmt = text("""
+            SELECT * FROM ctx_meta WHERE id = :id
+        """).bindparams(id=id)
+        db = self.window.core.db.get_db()
+        with db.connect() as conn:
+            result = conn.execute(stmt)
+            row = result.fetchone()
+            if row:
+                meta = CtxMeta()
+                unpack_meta(meta, row._asdict())
+                return meta
+        return None
+
     def get_items(self, id: int) -> list:
         """
         Return ctx items list by ctx meta ID
 
         :return: list of CtxItem
         """
         stmt = text("""
@@ -307,15 +352,17 @@
                 run_id = :run_id,
                 status = :status,
                 extra = :extra,
                 is_initialized = :is_initialized,
                 is_deleted = :is_deleted,
                 is_important = :is_important,
                 is_archived = :is_archived,
-                label = :label
+                label = :label,
+                root_id = :root_id,
+                parent_id = :parent_id
             WHERE id = :id
         """).bindparams(
             id=meta.id,
             external_id=meta.external_id,
             name=meta.name,
             mode=meta.mode,
             model=meta.model,
@@ -328,14 +375,16 @@
             status=meta.status,
             extra=meta.extra,
             is_initialized=int(meta.initialized),
             is_deleted=int(meta.deleted),
             is_important=int(meta.important),
             is_archived=int(meta.archived),
             label=int(meta.label),
+            root_id=meta.root_id,
+            parent_id=meta.parent_id,
         )
         with db.begin() as conn:
             conn.execute(stmt)
             return True
 
     def update_meta_all(self, meta: CtxMeta, items: list) -> bool:
         """
@@ -542,15 +591,17 @@
                 status,
                 extra,
                 is_initialized,
                 is_deleted,
                 is_important,
                 is_archived,
                 label,
-                group_id
+                group_id,
+                root_id,
+                parent_id
             )
             VALUES 
             (
                 :uuid,
                 :external_id,
                 :created_ts,
                 :updated_ts,
@@ -566,15 +617,17 @@
                 :status,
                 :extra,
                 :is_initialized,
                 :is_deleted,
                 :is_important,
                 :is_archived,
                 :label,
-                :group_id
+                :group_id,
+                :root_id,
+                :parent_id
             )
         """).bindparams(
             uuid=meta.uuid,
             external_id=meta.external_id,
             created_ts=int(meta.created or 0),
             updated_ts=int(meta.updated or 0),
             name=meta.name,
@@ -590,14 +643,16 @@
             extra=meta.extra,
             is_initialized=int(meta.initialized),
             is_deleted=int(meta.deleted),
             is_important=int(meta.important),
             is_archived=int(meta.archived),
             label=int(meta.label),
             group_id=meta.group_id,
+            root_id=meta.root_id,
+            parent_id=meta.parent_id,
         )
         with db.begin() as conn:
             result = conn.execute(stmt)
             meta.id = result.lastrowid
             return meta.id
 
     def insert_item(self, meta: CtxMeta, item: CtxItem) -> int:
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/ctx/json_file.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/ctx/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/history/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/history/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/history/patch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/history/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/history/txt_file.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/history/txt_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/index/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/index/db_sqlite/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/index/db_sqlite/patch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/index/db_sqlite/storage.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/index/db_sqlite/utils.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/index/json_file.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/index/patch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/index/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/mode/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/mode/json_file.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/mode/patch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/mode/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/model/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/model/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/model/json_file.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/model/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/model/patch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/model/patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 16:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 from packaging.version import parse as parse_version, Version
 
 
 class Patch:
     def __init__(self, window=None):
@@ -208,14 +208,25 @@
                 updated = True
 
             if old < parse_version("2.2.6"):
                 print("Migrating models from < 2.2.6...")
                 # add missing gpt-4-turbo
                 updated = True
 
+            # < 2.2.7  <--- add expert mode
+            if old < parse_version("2.2.7"):
+                print("Migrating models from < 2.2.7...")
+                exclude = ["gpt-3.5-turbo-instruct", "gpt-4-vision-preview"]
+                for id in data:
+                    model = data[id]
+                    if model.id.startswith("gpt-") and model.id not in exclude:
+                        if "expert" not in model.mode:
+                            model.mode.append("expert")
+                updated = True
+
         # update file
         if updated:
             data = dict(sorted(data.items()))
             self.window.core.models.items = data
             self.window.core.models.save()
 
             # also patch any missing models
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/notepad/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/notepad/json_file.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/notepad/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/plugin_preset/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/plugin_preset/json_file.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/plugin_preset/patch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/plugin_preset/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/preset/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/preset/json_file.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/json_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -161,40 +161,46 @@
         """
         Serialize item to dict
 
         :param item: item to serialize
         :return: serialized item
         """
         return {
+            'uuid': item.uuid,
             'name': item.name,
             'ai_name': item.ai_name,
             'user_name': item.user_name,
             'prompt': item.prompt,
             'chat': item.chat,
             'completion': item.completion,
             'img': item.img,
             'vision': item.vision,
             'langchain': item.langchain,
             'assistant': item.assistant,
             "llama_index": item.llama_index,
             "agent": item.agent,
+            "expert": item.expert,
             'temperature': item.temperature,
             'filename': item.filename,
             'model': item.model,
             'tools': item.tools,
+            'experts': item.experts,
+            'enabled': item.enabled,
         }
 
     @staticmethod
     def deserialize(data: dict, item: PresetItem):
         """
         Deserialize item from dict
 
         :param data: serialized item
         :param item: item to deserialize
         """
+        if 'uuid' in data:
+            item.uuid = data['uuid']
         if 'name' in data:
             item.name = data['name']
         if 'ai_name' in data:
             item.ai_name = data['ai_name']
         if 'user_name' in data:
             item.user_name = data['user_name']
         if 'prompt' in data:
@@ -211,22 +217,28 @@
             item.langchain = data['langchain']
         if 'assistant' in data:
             item.assistant = data['assistant']
         if 'llama_index' in data:
             item.llama_index = data['llama_index']
         if 'agent' in data:
             item.agent = data['agent']
+        if 'expert' in data:
+            item.expert = data['expert']
         if 'temperature' in data:
             item.temperature = data['temperature']
         if 'filename' in data:
             item.filename = data['filename']
         if 'model' in data:
             item.model = data['model']
         if 'tools' in data:
             item.tools = data['tools']
+        if 'experts' in data:
+            item.experts = data['experts']
+        if 'enabled' in data:
+            item.enabled = data['enabled']
 
         # get version
         if '__meta__' in data and 'version' in data['__meta__']:
             item.version = data['__meta__']['version']
 
     def dump(self, item: PresetItem) -> str:
         """
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/core/preset/patch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/core/preset/patch.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.01.12 10:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import os
 import shutil
 
 from packaging.version import parse as parse_version, Version
 
@@ -24,19 +24,23 @@
         Migrate to current app version
 
         :param version: current app version
         :return: True if migrated
         """
         migrated = False
         is_llama = False
+        is_expert = False
         for k in self.window.core.presets.items:
             data = self.window.core.presets.items[k]
             updated = False
 
             # get version of preset
+            if data.version is None or data.version == "":
+                continue
+
             old = parse_version(data.version)
 
             # check if presets file is older than current app version
             if old < version:
                 # < 2.0.0
                 if old < parse_version("2.0.0"):
                     print("Migrating presets dir from < 2.0.0...")
@@ -60,14 +64,33 @@
                         src = os.path.join(self.window.core.config.get_app_path(), 'data', 'config', 'presets',
                                            'current.llama_index.json')
                         shutil.copyfile(src, dst)
                         updated = True
                         is_llama = True  # prevent multiple copies
                         print("Patched file: {}.".format(dst))
 
+                # < 2.2.7
+                if old < parse_version("2.2.7"):
+                    if not is_expert:
+                        print("Migrating preset files from < 2.2.7...")
+                        dst = os.path.join(self.window.core.config.get_user_dir('presets'), 'current.expert.json')
+                        src = os.path.join(self.window.core.config.get_app_path(), 'data', 'config', 'presets', 'current.expert.json')
+                        shutil.copyfile(src, dst)
+                        print("Patched file: {}.".format(dst))
+                        dst = os.path.join(self.window.core.config.get_user_dir('presets'), 'current.agent.json')
+                        src = os.path.join(self.window.core.config.get_app_path(), 'data', 'config', 'presets', 'current.agent.json')
+                        shutil.copyfile(src, dst)
+                        print("Patched file: {}.".format(dst))
+                        dst = os.path.join(self.window.core.config.get_user_dir('presets'), 'joke_expert.json')
+                        src = os.path.join(self.window.core.config.get_app_path(), 'data', 'config', 'presets', 'joke_expert.json')
+                        shutil.copyfile(src, dst)
+                        print("Patched file: {}.".format(dst))
+                        updated = True
+                        is_expert = True  # prevent multiple copies
+
             # update file
             if updated:
                 self.window.core.presets.load()  # reload presets from patched files
                 self.window.core.presets.save(k)  # re-save presets
                 migrated = True
                 print("Preset {} patched to version {}.".format(k, version))
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/gpt/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 from openai import OpenAI
 
 from pygpt_net.core.bridge import BridgeContext
 
 from .assistants import Assistants
@@ -78,18 +78,14 @@
         # get model id
         model_id = None
         if model is not None:
             model_id = model.id
             if max_tokens > model.tokens:  # check max output tokens
                 max_tokens = model.tokens
 
-        # minimum 1 token is required
-        if max_tokens < 1:
-            max_tokens = 1
-
         response = None
         used_tokens = 0
         context.max_tokens = max_tokens  # update max output tokens
         file_ids = context.file_ids  # uploaded files IDs (assistant mode only)
 
         # completion
         if mode == "completion":
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/gpt/assistants.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/gpt/chat.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/chat.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 import json
+import re
 
 from pygpt_net.core.bridge import BridgeContext
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.item.model import ModelItem
 
 
 class Chat:
@@ -32,15 +33,15 @@
 
         :param context: Bridge context
         :param extra: Extra arguments
         :return: response or stream chunks
         """
         prompt = context.prompt
         stream = context.stream
-        max_tokens = context.max_tokens
+        max_tokens = int(context.max_tokens or 0)
         system_prompt = context.system_prompt
         model = context.model
         functions = context.external_functions
         attachments = context.attachments
 
         ctx = context.ctx
         if ctx is None:
@@ -51,27 +52,29 @@
         client = self.window.core.gpt.get_client()
 
         # build chat messages
         messages = self.build(
             prompt=prompt,
             system_prompt=system_prompt,
             model=model,
+            history=context.history,
             attachments=attachments,
             ai_name=ai_name,
             user_name=user_name,
         )
         msg_tokens = self.window.core.tokens.from_messages(
             messages,
             model.id,
         )
         # check if max tokens not exceeded
-        if msg_tokens + int(max_tokens) > model.ctx:
-            max_tokens = model.ctx - msg_tokens - 1
-            if max_tokens < 1:
-                max_tokens = 1
+        if max_tokens > 0:
+            if msg_tokens + int(max_tokens) > model.ctx:
+                max_tokens = model.ctx - msg_tokens - 1
+                if max_tokens < 0:
+                    max_tokens = 0
 
         # extra API kwargs
         response_kwargs = {}
 
         # tools / functions
         tools = []
         if functions is not None and isinstance(functions, list):
@@ -87,42 +90,45 @@
                             "parameters": params,
                             "description": function['desc'],
                         }
                     }
                 )
         if len(tools) > 0:
             response_kwargs['tools'] = tools
+        if max_tokens > 0:
+            response_kwargs['max_tokens'] = max_tokens
 
         response = client.chat.completions.create(
             messages=messages,
             model=model.id,
-            max_tokens=int(max_tokens),
             temperature=self.window.core.config.get('temperature'),
             top_p=self.window.core.config.get('top_p'),
             frequency_penalty=self.window.core.config.get('frequency_penalty'),
             presence_penalty=self.window.core.config.get('presence_penalty'),
             stream=stream,
             **response_kwargs
         )
         return response
 
     def build(
             self,
             prompt: str,
             system_prompt: str,
             model: ModelItem,
+            history: list = None,
             attachments: dict = None,
             ai_name: str = None,
             user_name: str = None
     ) -> list:
         """
         Build list of chat messages
 
         :param prompt: user prompt
         :param system_prompt: system prompt
+        :param history: history
         :param model: model item
         :param attachments: attachments
         :param ai_name: AI name
         :param user_name: username
         :return: messages list
         """
         messages = []
@@ -150,28 +156,29 @@
 
         # append system prompt
         if system_prompt is not None and system_prompt != "":
             messages.append({"role": "system", "content": system_prompt})
 
         # append messages from context (memory)
         if self.window.core.config.get('use_context'):
-            items = self.window.core.ctx.get_prompt_items(
+            items = self.window.core.ctx.get_history(
+                history,
                 model.id,
                 mode,
                 used_tokens,
                 max_ctx_tokens,
             )
             for item in items:
                 # input
                 if item.input is not None and item.input != "":
-                    messages.append({"role": "system", "name": user_name, "content": item.input})
+                    messages.append({"role": "system", "name": self.sanitize_name(user_name), "content": item.input})
 
                 # output
                 if item.output is not None and item.output != "":
-                    messages.append({"role": "system", "name": ai_name, "content": item.output})
+                    messages.append({"role": "system", "name": self.sanitize_name(ai_name), "content": item.output})
 
         # use vision if available in current model
         content = str(prompt)
         if "vision" in model.mode:
             content = self.window.core.gpt.vision.build_content(prompt, attachments)
 
         # append current prompt
@@ -180,14 +187,28 @@
         # input tokens: update
         self.input_tokens += self.window.core.tokens.from_messages(
             messages,
             model.id,
         )
         return messages
 
+    def sanitize_name(self, name: str) -> str:
+        """
+        Sanitize name
+
+        :param name: name
+        :return: sanitized name
+        """
+        if name is None:
+            return ""
+        # allowed characters: a-z, A-Z, 0-9, _, and -
+        name = name.strip().lower()
+        sanitized_name = re.sub(r'[^a-z0-9_-]', '_', name)
+        return sanitized_name[:64]  # limit to 64 characters
+
     def reset_tokens(self):
         """Reset input tokens counter"""
         self.input_tokens = 0
 
     def get_used_tokens(self) -> int:
         """
         Get input tokens counter
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/gpt/completion.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/completion.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 03:00:00                  #
 # ================================================== #
 
 from pygpt_net.core.bridge import BridgeContext
 from pygpt_net.item.ctx import CtxItem
 from pygpt_net.item.model import ModelItem
 
 
@@ -30,15 +30,15 @@
 
         :param context: Bridge context
         :param extra: Extra arguments
         :return: response or stream chunks
         """
         prompt = context.prompt
         stream = context.stream
-        max_tokens = context.max_tokens
+        max_tokens = int(context.max_tokens or 0)
         system_prompt = context.system_prompt
         model = context.model
         model_id = model.id
 
         ctx = context.ctx
         if ctx is None:
             ctx = CtxItem()  # create empty context
@@ -46,61 +46,70 @@
         ai_name = ctx.output_name  # from ctx
 
         # build prompt message
         message = self.build(
             prompt=prompt,
             system_prompt=system_prompt,
             model=model,
+            history=context.history,
             ai_name=ai_name,
             user_name=user_name,
         )
 
         # check if max tokens not exceeded
         available_tokens = model.ctx - self.input_tokens
-        if available_tokens < max_tokens:
-            max_tokens = available_tokens
+        if max_tokens > 0:
+            if available_tokens < max_tokens:
+                max_tokens = available_tokens
 
         # prepare stop word if user_name is set
         stop = ""
         if user_name is not None and user_name != '':
             stop = [user_name + ':']
 
         client = self.window.core.gpt.get_client()
 
         # fix for deprecated OpenAI davinci models
         if model_id.startswith('text-davinci'):
             model_id = 'gpt-3.5-turbo-instruct'
 
+        # extra API kwargs
+        response_kwargs = {}
+        if max_tokens > 0:
+            response_kwargs['max_tokens'] = max_tokens
+
         response = client.completions.create(
             prompt=message,
             model=model_id,
-            max_tokens=int(max_tokens),
             temperature=self.window.core.config.get('temperature'),
             top_p=self.window.core.config.get('top_p'),
             frequency_penalty=self.window.core.config.get('frequency_penalty'),
             presence_penalty=self.window.core.config.get('presence_penalty'),
             stop=stop,
             stream=stream,
+            **response_kwargs
         )
         return response
 
     def build(
             self,
             prompt: str,
             system_prompt: str,
             model: ModelItem,
+            history: list = None,
             ai_name: str = None,
             user_name: str = None,
     ) -> str:
         """
         Build completion string
 
         :param prompt: user prompt
         :param system_prompt: system prompt
         :param model: model item
+        :param history: history
         :param ai_name: AI name
         :param user_name: username
         :return: message string (parsed with context)
         """
         message = ""
 
         # tokens config
@@ -117,15 +126,16 @@
         # input tokens: reset
         self.reset_tokens()
 
         if system_prompt is not None and system_prompt != "":
             message += system_prompt
 
         if self.window.core.config.get('use_context'):
-            items = self.window.core.ctx.get_prompt_items(
+            items = self.window.core.ctx.get_history(
+                history,
                 model.id,
                 "completion",
                 used_tokens,
                 max_ctx_tokens,
             )
             for item in items:
                 if item.input_name is not None \
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/gpt/image.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/gpt/store.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/gpt/summarizer.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/summarizer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/gpt/vision.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/vision.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.30 15:00:00                  #
+# Updated Date: 2024.05.01 03:00:00                  #
 # ================================================== #
 
 import base64
 import os
 import re
 
 from pygpt_net.core.bridge import BridgeContext
@@ -36,49 +36,57 @@
 
         :param context: Bridge context
         :param extra: Extra arguments
         :return: response or stream chunks
         """
         prompt = context.prompt
         stream = context.stream
-        max_tokens = context.max_tokens
+        max_tokens = int(context.max_tokens or 0)
         system_prompt = context.system_prompt
         attachments = context.attachments
         model = context.model
         model_id = model.id
         client = self.window.core.gpt.get_client()
 
+        # extra API kwargs
+        response_kwargs = {}
+        if max_tokens > 0:
+            response_kwargs['max_tokens'] = max_tokens
+
         # build chat messages
         messages = self.build(
             prompt=prompt,
             system_prompt=system_prompt,
             model=model,
+            history=context.history,
             attachments=attachments,
         )
         response = client.chat.completions.create(
             messages=messages,
             model=model_id,
-            max_tokens=int(max_tokens),
             stream=stream,
+            **response_kwargs
         )
         return response
 
     def build(
             self,
             prompt: str,
             system_prompt: str,
             model: ModelItem,
+            history: list = None,
             attachments: dict = None,
     ) -> list:
         """
         Build chat messages list
 
         :param prompt: user prompt
         :param system_prompt: system prompt
         :param model: model item
+        :param history: history
         :param attachments: attachments
         :return: messages list
         """
         messages = []
 
         # tokens config
         mode = 'vision'
@@ -100,15 +108,16 @@
             messages.append({"role": "system", "content": system_prompt})
         else:
             if system_prompt is not None and system_prompt != "":
                 messages.append({"role": "system", "content": system_prompt})
 
         # append messages from context (memory)
         if self.window.core.config.get('use_context'):
-            items = self.window.core.ctx.get_prompt_items(
+            items = self.window.core.ctx.get_history(
+                history,
                 model.id,
                 mode,
                 used_tokens,
                 max_ctx_tokens,
             )
             for item in items:
                 # input
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/gpt/worker/assistants.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/worker/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/gpt/worker/importer.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/gpt/worker/importer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/llms/anthropic.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/llms/azure_openai.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/llms/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/llms/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/llms/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/llms/hugging_face.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/llms/hugging_face.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/llms/llama.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/llms/llama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/llms/ollama.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/llms/openai.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/llms/openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_csv.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_csv.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_docx.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_docx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_epub.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_epub.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_excel.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_excel.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_html.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_html.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_image_vision.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_image_vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_ipynb.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_ipynb.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_json.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_json.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_markdown.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_pdf.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_pdf.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_video_audio.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_video_audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/file_xml.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/file_xml.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/database/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/database/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/github/issues.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/github/issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/github/repo.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/github/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/google/calendar.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/google/docs.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/google/gmail.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/google/keep.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/google/sheets.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/google/sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/image_vision/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/image_vision/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/json/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/json/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/simple_csv/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/simple_csv/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/video_audio/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/video_audio/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/web_page/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/web_page/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/yt/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/yt/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/hub/yt/utils.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/hub/yt/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_bitbucket.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_bitbucket.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_database.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_database.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_github_issues.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_github_issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_github_repo.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_github_repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_google_calendar.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_google_docs.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_google_drive.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_drive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_google_gmail.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_google_keep.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_google_sheets.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_google_sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_page.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_rss.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_rss.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_sitemap.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_sitemap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_twitter.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_twitter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/loaders/web_yt.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/loaders/web_yt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/chroma.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/elasticsearch.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/pinecode.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/pinecode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/redis.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/redis.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/simple.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/vector_stores/temp.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/vector_stores/temp.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/web/base.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/web/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/web/google_custom_search.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/web/google_custom_search.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/provider/web/microsoft_bing.py` & `pygpt_net-2.2.7/src/pygpt_net/provider/web/microsoft_bing.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/audio_transcriber/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/audio_transcriber/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/base.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/code_interpreter/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/code_interpreter/ui/dialogs.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/code_interpreter/ui/widgets.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/code_interpreter/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/image_viewer/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/image_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/image_viewer/ui/dialogs.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/image_viewer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/indexer/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/indexer/ui/browse.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/browse.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/indexer/ui/ctx.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/indexer/ui/dialogs.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/indexer/ui/files.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/indexer/ui/web.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/indexer/ui/widgets.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/indexer/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/media_player/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/media_player/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/media_player/ui/dialogs.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/media_player/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/media_player/ui/widgets.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/media_player/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/text_editor/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/text_editor/ui/dialogs.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/tools/text_editor/ui/widgets.py` & `pygpt_net-2.2.7/src/pygpt_net/tools/text_editor/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/base/config_dialog.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/base/config_dialog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/base/context_menu.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/base/context_menu.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/about.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/applog.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/assistant.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/assistant_store.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/changelog.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/changelog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/create.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/db.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/debug.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/dictionary.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/editor.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/find.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/image.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/license.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/logger.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/models.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/plugins.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/preset.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/preset.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.02.15 01:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QPushButton, QHBoxLayout, QLabel, QVBoxLayout, QSplitter, QWidget, QSizePolicy
 
 from pygpt_net.ui.base.config_dialog import BaseConfigDialog
 from pygpt_net.ui.widget.dialog.editor import EditorDialog
+from pygpt_net.ui.widget.lists.experts import ExpertsEditor
 from pygpt_net.utils import trans
 
 
 class Preset(BaseConfigDialog):
     def __init__(self, window=None, *args, **kwargs):
         super(Preset, self).__init__(window, *args, **kwargs)
         """
@@ -76,51 +77,67 @@
             elif fields[key]["type"] == 'combo':
                 options[key] = self.add_option(widgets[key], fields[key])
 
         self.window.ui.nodes['preset.tool.function.label'].setVisible(False)  # hide label
 
         rows = QVBoxLayout()
 
-        ignore_keys = ["chat", "completion", "img", "vision", "llama_index", "langchain", "agent", "prompt", "tool.function"]
+        ignore_keys = [
+            "chat",
+            "completion",
+            "img", "vision",
+            "llama_index",
+            "langchain",
+            "agent",
+            "expert",
+            "prompt",
+            "tool.function",
+        ]
 
         options["chat"].setContentsMargins(0, 0, 0, 0)
         options["completion"].setContentsMargins(0, 0, 0, 0)
         options["img"].setContentsMargins(0, 0, 0, 0)
         options["vision"].setContentsMargins(0, 0, 0, 0)
         options["langchain"].setContentsMargins(0, 0, 0, 0)
         options["llama_index"].setContentsMargins(0, 0, 0, 0)
         options["agent"].setContentsMargins(0, 0, 0, 0)
+        options["expert"].setContentsMargins(0, 0, 0, 0)
         options["prompt"].setContentsMargins(0, 0, 0, 0)
         options["tool.function"].setContentsMargins(0, 0, 0, 0)
 
         rows_mode = QVBoxLayout()
         rows_mode.addLayout(options["chat"])
         rows_mode.addLayout(options["completion"])
         rows_mode.addLayout(options["img"])
         rows_mode.addLayout(options["vision"])
         # rows_mode.addLayout(options["assistant"])
         rows_mode.addLayout(options["langchain"])
         rows_mode.addLayout(options["llama_index"])
         rows_mode.addLayout(options["agent"])
+        rows_mode.addLayout(options["expert"])
+
 
         rows_mode.addStretch()
         rows_mode.setContentsMargins(0, 0, 0, 0)
 
-        widget_mode = QWidget()
-        widget_mode.setLayout(rows_mode)
-        widget_mode.setContentsMargins(0, 0, 0, 0)
+        self.window.ui.nodes['preset.editor.modes'] = QWidget()
+        self.window.ui.nodes['preset.editor.modes'].setLayout(rows_mode)
+        self.window.ui.nodes['preset.editor.modes'].setContentsMargins(0, 0, 0, 0)
+        self.window.ui.nodes['preset.editor.modes'].setMaximumWidth(300)
+
+        self.window.ui.nodes['preset.editor.functions'] = QWidget()
+        self.window.ui.nodes['preset.editor.functions'].setLayout(options["tool.function"])
+        self.window.ui.nodes['preset.editor.functions'].setMinimumWidth(400)
+
+        self.window.ui.nodes['preset.editor.experts'] = ExpertsEditor(self.window)
 
         widget_prompt = QWidget()
         widget_prompt.setLayout(options["prompt"])
         widget_prompt.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
 
-        widget_tools = QWidget()
-        widget_tools.setLayout(options["tool.function"])
-        widget_tools.setMinimumWidth(400)
-
         # append widgets options layouts to rows
         for key in options:
             if key in ignore_keys:
                 continue
             options[key].setContentsMargins(0, 0, 0, 0)
             rows.addLayout(options[key])
 
@@ -129,21 +146,20 @@
         rows.addStretch()
         widget_base = QWidget()
         widget_base.setLayout(rows)
 
         # set max width to options
         widget_base.setMinimumWidth(400)
         widget_base.setMaximumWidth(450)
-        widget_mode.setMaximumWidth(300)
 
         main = QHBoxLayout()
         main.addWidget(widget_base)
-
-        main.addWidget(widget_tools)
-        main.addWidget(widget_mode)
+        main.addWidget(self.window.ui.nodes['preset.editor.functions'])
+        main.addWidget(self.window.ui.nodes['preset.editor.modes'])
+        main.addWidget(self.window.ui.nodes['preset.editor.experts'])
         main.setContentsMargins(0, 0, 0, 0)
 
         widget_main = QWidget()
         widget_main.setLayout(main)
 
         self.window.ui.splitters['editor.presets'] = QSplitter(Qt.Vertical)
         self.window.ui.splitters['editor.presets'].addWidget(widget_main)
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/preset_plugins.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/profile.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/rename.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/settings.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/snap.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/start.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/start.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/update.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialog/workdir.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialog/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/dialogs.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/attachments.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/attachments_uploaded.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/attachments_uploaded.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/calendar.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/input.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/markdown.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/output.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/chat/painter.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/chat/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/ctx/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/ctx/ctx_list.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/ctx_list.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/ctx/search_input.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/search_input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/ctx/video.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/ctx/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/status.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/status.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/agent.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/agent.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/assistants.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/footer.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/footer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/image.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/indexes.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/mode.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/model.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/prompt.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/layout/toolbox/vision.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/layout/toolbox/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/main.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/main.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/menu/__init__.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/menu/about.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/menu/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/menu/audio.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/menu/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/menu/config.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/menu/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/menu/debug.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/menu/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/menu/file.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/menu/file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/menu/lang.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/menu/lang.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/menu/plugins.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/menu/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/menu/theme.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/menu/theme.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/menu/tools.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/menu/tools.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/menu/video.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/menu/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/tray.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/tray.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/audio/input.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/audio/input_button.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/input_button.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/audio/output.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/audio/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/calendar/select.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/calendar/select.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/alert.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/alert.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/applog.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/assistant_store.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/audio.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/base.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/confirm.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/create.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/db.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/debug.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/editor.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/editor_file.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/editor_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/find.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/image.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/info.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/license.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/logger.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/model.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/preset_plugins.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/profile.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/rename.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/settings.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/settings_plugin.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/settings_plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/snap.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/update.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/dialog/workdir.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/dialog/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/draw/painter.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/draw/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/element/button.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/button.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/element/checkbox.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/element/group.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/group.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/element/labels.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/element/labels.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/filesystem/explorer.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/filesystem/explorer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/image/display.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/image/display.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/assistant.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/assistant_store.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/attachment.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/base.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.08 21:00:00                  #
+# Updated Date: 2024.05.01 17:00:00                  #
 # ================================================== #
 
 from PySide6.QtCore import QItemSelectionModel
 from PySide6.QtWidgets import QTreeView, QAbstractItemView
 
 
 class BaseList(QTreeView):
@@ -31,15 +31,15 @@
         self.selection_locked = None
         self.selection = None
         self.unlocked = False
         self.clicked.connect(self.click)
         self.header().hide()
 
     def click(self, val):
-        self.window.controller.mode.select(self.id, val.row())
+        self.window.controller.mode.select(self.id)
         self.selection = self.selectionModel().selection()
 
     def lockSelection(self, selected=None, deselected=None):
         if self.selection is not None:
             self.selectionModel().select(self.selection, QItemSelectionModel.Select)
 
     def backup_selection(self):
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/context.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/db.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/debug.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/index.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/index.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/index_combo.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/index_combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/mode.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/model.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/model_editor.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/model_editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/plugin.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/preset.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/preset_plugins.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,127 +2,123 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.02.01 00:00:00                  #
+# Updated Date: 2024.03.06 22:00:00                  #
 # ================================================== #
 
 from PySide6.QtGui import QAction, QIcon
 from PySide6.QtWidgets import QMenu
 
 from pygpt_net.ui.widget.lists.base import BaseList
 from pygpt_net.utils import trans
 import pygpt_net.icons_rc
 
 
-class PresetList(BaseList):
+class PresetPluginsList(BaseList):
     def __init__(self, window=None, id=None):
         """
-        Presets select menu
+        Preset plugins menu (in editor)
 
         :param window: main window
-        :param id: input id
+        :param id: parent id
         """
-        super(PresetList, self).__init__(window)
+        super(PresetPluginsList, self).__init__(window)
         self.window = window
         self.id = id
 
-        self.doubleClicked.connect(self.dblclick)
-
     def click(self, val):
-        self.window.controller.presets.select(val.row())
-        self.selection = self.selectionModel().selection()
-
-    def dblclick(self, val):
-        """
-        Double click event
-
-        :param val: double click event
-        """
-        self.window.controller.presets.editor.edit(val.row())
+        pass
 
     def contextMenuEvent(self, event):
         """
         Context menu event
 
         :param event: context menu event
         """
-        item = self.indexAt(event.pos())
-        idx = item.row()
-
         actions = {}
-        actions['edit'] = QAction(QIcon(":/icons/edit.svg"), trans('preset.action.edit'), self)
-        actions['edit'].triggered.connect(
-            lambda: self.action_edit(event))
-
-        actions['duplicate'] = QAction(QIcon(":/icons/copy.svg"), trans('preset.action.duplicate'), self)
+        actions['use'] = QAction(QIcon(":/icons/check.svg"), trans('action.use'), self)
+        actions['use'].triggered.connect(
+            lambda: self.action_use(event))
+        actions['rename'] = QAction(QIcon(":/icons/edit.svg"), trans('action.rename'), self)
+        actions['rename'].triggered.connect(
+            lambda: self.action_rename(event))
+        actions['duplicate'] = QAction(QIcon(":/icons/copy.svg"), trans('action.duplicate'), self)
         actions['duplicate'].triggered.connect(
             lambda: self.action_duplicate(event))
-
-        if self.window.controller.presets.is_current(idx):
-            actions['restore'] = QAction(QIcon(":/icons/undo.svg"), trans('dialog.editor.btn.defaults'), self)
-            actions['restore'].triggered.connect(
-                lambda: self.action_restore(event))
-        else:
-            actions['delete'] = QAction(QIcon(":/icons/delete.svg"), trans('preset.action.delete'), self)
-            actions['delete'].triggered.connect(
-                lambda: self.action_delete(event))
+        actions['reset'] = QAction(QIcon(":/icons/close.svg"), trans('action.reset'), self)
+        actions['reset'].triggered.connect(
+            lambda: self.action_reset(event))
+        actions['delete'] = QAction(QIcon(":/icons/delete.svg"), trans('action.delete'), self)
+        actions['delete'].triggered.connect(
+            lambda: self.action_delete(event))
 
         menu = QMenu(self)
-        menu.addAction(actions['edit'])
-        if self.window.controller.presets.is_current(idx):
-            actions['edit'].setEnabled(False)
-            menu.addAction(actions['restore'])
-            menu.addAction(actions['duplicate'])
-        else:
-            menu.addAction(actions['duplicate'])
-            menu.addAction(actions['delete'])
+        menu.addAction(actions['use'])
+        menu.addAction(actions['rename'])
+        menu.addAction(actions['duplicate'])
+        menu.addAction(actions['reset'])
+        menu.addAction(actions['delete'])
 
+        item = self.indexAt(event.pos())
+        idx = item.row()
         if idx >= 0:
-            self.window.controller.presets.select(idx)
-            self.selection = self.selectionModel().selection()
-            # self.window.controller.mode.select(self.id, item.row())
             menu.exec_(event.globalPos())
 
-    def action_edit(self, event):
+    def action_use(self, event):
         """
-        Edit action handler
+        Use action handler
 
         :param event: mouse event
         """
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
-            self.window.controller.presets.editor.edit(idx)
+            self.window.controller.plugins.presets.select_by_idx(idx)
 
     def action_duplicate(self, event):
         """
         Duplicate action handler
 
         :param event: mouse event
         """
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
-            self.window.controller.presets.duplicate(idx)
+            self.window.controller.plugins.presets.duplicate_by_idx(idx)
+
+    def action_reset(self, event):
+        """
+        Reset action handler
+
+        :param event: mouse event
+        """
+        item = self.indexAt(event.pos())
+        idx = item.row()
+        if idx >= 0:
+            self.window.controller.plugins.presets.reset_by_idx(idx)
 
     def action_delete(self, event):
         """
         Delete action handler
 
         :param event: mouse event
         """
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
-            self.window.controller.presets.delete(idx)
+            self.window.controller.plugins.presets.delete_by_idx(idx)
 
-    def action_restore(self, event):
+    def action_rename(self, event):
         """
-        Restore action handler
+        Rename action handler
 
         :param event: mouse event
         """
-        self.window.controller.presets.restore()
+        item = self.indexAt(event.pos())
+        idx = item.row()
+        if idx >= 0:
+            self.window.controller.plugins.presets.rename_by_idx(idx)
+
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/preset_plugins.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.03.06 22:00:00                  #
+# Updated Date: 2024.04.09 23:00:00                  #
 # ================================================== #
 
 from PySide6.QtGui import QAction, QIcon
 from PySide6.QtWidgets import QMenu
 
 from pygpt_net.ui.widget.lists.base import BaseList
 from pygpt_net.utils import trans
 import pygpt_net.icons_rc
 
 
-class PresetPluginsList(BaseList):
+class ProfileList(BaseList):
     def __init__(self, window=None, id=None):
         """
-        Preset plugins menu (in editor)
+        Profile menu (in editor)
 
         :param window: main window
         :param id: parent id
         """
-        super(PresetPluginsList, self).__init__(window)
+        super(ProfileList, self).__init__(window)
         self.window = window
         self.id = id
 
     def click(self, val):
         pass
 
     def contextMenuEvent(self, event):
@@ -38,33 +38,39 @@
 
         :param event: context menu event
         """
         actions = {}
         actions['use'] = QAction(QIcon(":/icons/check.svg"), trans('action.use'), self)
         actions['use'].triggered.connect(
             lambda: self.action_use(event))
-        actions['rename'] = QAction(QIcon(":/icons/edit.svg"), trans('action.rename'), self)
-        actions['rename'].triggered.connect(
-            lambda: self.action_rename(event))
+        actions['edit'] = QAction(QIcon(":/icons/edit.svg"), trans('action.edit'), self)
+        actions['edit'].triggered.connect(
+            lambda: self.action_edit(event))
         actions['duplicate'] = QAction(QIcon(":/icons/copy.svg"), trans('action.duplicate'), self)
         actions['duplicate'].triggered.connect(
             lambda: self.action_duplicate(event))
+
+
         actions['reset'] = QAction(QIcon(":/icons/close.svg"), trans('action.reset'), self)
         actions['reset'].triggered.connect(
             lambda: self.action_reset(event))
-        actions['delete'] = QAction(QIcon(":/icons/delete.svg"), trans('action.delete'), self)
+        actions['delete'] = QAction(QIcon(":/icons/delete.svg"), trans('action.profile.delete'), self)
         actions['delete'].triggered.connect(
             lambda: self.action_delete(event))
+        actions['delete_all'] = QAction(QIcon(":/icons/delete.svg"), trans('action.profile.delete_all'), self)
+        actions['delete_all'].triggered.connect(
+            lambda: self.action_delete_all(event))
 
         menu = QMenu(self)
+        menu.addAction(actions['edit'])
         menu.addAction(actions['use'])
-        menu.addAction(actions['rename'])
         menu.addAction(actions['duplicate'])
         menu.addAction(actions['reset'])
         menu.addAction(actions['delete'])
+        menu.addAction(actions['delete_all'])
 
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
             menu.exec_(event.globalPos())
 
     def action_use(self, event):
@@ -72,53 +78,64 @@
         Use action handler
 
         :param event: mouse event
         """
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
-            self.window.controller.plugins.presets.select_by_idx(idx)
+            self.window.controller.settings.profile.select_by_idx(idx)
 
     def action_duplicate(self, event):
         """
         Duplicate action handler
 
         :param event: mouse event
         """
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
-            self.window.controller.plugins.presets.duplicate_by_idx(idx)
+            self.window.controller.settings.profile.duplicate_by_idx(idx)
 
     def action_reset(self, event):
         """
         Reset action handler
 
         :param event: mouse event
         """
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
-            self.window.controller.plugins.presets.reset_by_idx(idx)
+            self.window.controller.settings.profile.reset_by_idx(idx)
 
     def action_delete(self, event):
         """
         Delete action handler
 
         :param event: mouse event
         """
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
-            self.window.controller.plugins.presets.delete_by_idx(idx)
+            self.window.controller.settings.profile.delete_by_idx(idx)
+
+    def action_delete_all(self, event):
+        """
+        Delete all action handler
+
+        :param event: mouse event
+        """
+        item = self.indexAt(event.pos())
+        idx = item.row()
+        if idx >= 0:
+            self.window.controller.settings.profile.delete_all_by_idx(idx)
 
-    def action_rename(self, event):
+    def action_edit(self, event):
         """
-        Rename action handler
+        Edit action handler
 
         :param event: mouse event
         """
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
-            self.window.controller.plugins.presets.rename_by_idx(idx)
+            self.window.controller.settings.profile.edit_by_idx(idx)
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/profile.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/uploaded.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,140 +2,140 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.04.09 23:00:00                  #
+# Updated Date: 2024.04.26 23:00:00                  #
 # ================================================== #
 
-from PySide6.QtGui import QAction, QIcon
+from PySide6.QtGui import QAction, QIcon, QResizeEvent, Qt
 from PySide6.QtWidgets import QMenu
 
 from pygpt_net.ui.widget.lists.base import BaseList
 from pygpt_net.utils import trans
 import pygpt_net.icons_rc
 
 
-class ProfileList(BaseList):
+class UploadedFileList(BaseList):
     def __init__(self, window=None, id=None):
         """
-        Profile menu (in editor)
+        Attachments menu
 
         :param window: main window
-        :param id: parent id
+        :param id: input id
         """
-        super(ProfileList, self).__init__(window)
+        super(UploadedFileList, self).__init__(window)
         self.window = window
         self.id = id
+        self.doubleClicked.connect(self.dblclick)
+        self.setHeaderHidden(False)
+        self.clicked.disconnect(self.click)
+
+        self.header = self.header()
+        self.header.setStretchLastSection(False)
+
+        self.column_proportion = 0.3
+        self.adjustColumnWidths()
+
+    def adjustColumnWidths(self):
+        total_width = self.width()
+        first_column_width = int(total_width * self.column_proportion)
+        self.setColumnWidth(0, first_column_width)
+        for column in range(1, 4):
+            self.setColumnWidth(column, (total_width - first_column_width) // (4 - 1))
+
+    def resizeEvent(self, event: QResizeEvent):
+        super().resizeEvent(event)
+        self.adjustColumnWidths()
+
+    def mousePressEvent(self, event):
+        """
+        Mouse press event
+
+        :param event: mouse event
+        """
+        if event.buttons() == Qt.LeftButton:
+            index = self.indexAt(event.pos())
+            if index.isValid():
+                self.window.controller.assistant.files.select(index.row())
+        super(UploadedFileList, self).mousePressEvent(event)
 
     def click(self, val):
+        """
+        Click event
+
+        :param val: click event
+        """
         pass
 
+    def dblclick(self, val):
+        """
+        Double click event
+
+        :param val: double click event
+        """
+        self.window.controller.assistant.files.select(val.row())
+
     def contextMenuEvent(self, event):
         """
         Context menu event
 
         :param event: context menu event
         """
         actions = {}
-        actions['use'] = QAction(QIcon(":/icons/check.svg"), trans('action.use'), self)
-        actions['use'].triggered.connect(
-            lambda: self.action_use(event))
-        actions['edit'] = QAction(QIcon(":/icons/edit.svg"), trans('action.edit'), self)
-        actions['edit'].triggered.connect(
-            lambda: self.action_edit(event))
-        actions['duplicate'] = QAction(QIcon(":/icons/copy.svg"), trans('action.duplicate'), self)
-        actions['duplicate'].triggered.connect(
-            lambda: self.action_duplicate(event))
+        actions['download'] = QAction(QIcon(":/icons/download.svg"), trans('action.download'), self)
+        actions['download'].triggered.connect(
+            lambda: self.action_download(event))
+
+        actions['rename'] = QAction(QIcon(":/icons/edit.svg"), trans('action.rename'), self)
+        actions['rename'].triggered.connect(
+            lambda: self.action_rename(event))
 
-
-        actions['reset'] = QAction(QIcon(":/icons/close.svg"), trans('action.reset'), self)
-        actions['reset'].triggered.connect(
-            lambda: self.action_reset(event))
-        actions['delete'] = QAction(QIcon(":/icons/delete.svg"), trans('action.profile.delete'), self)
+        actions['delete'] = QAction(QIcon(":/icons/delete.svg"), trans('action.delete'), self)
         actions['delete'].triggered.connect(
             lambda: self.action_delete(event))
-        actions['delete_all'] = QAction(QIcon(":/icons/delete.svg"), trans('action.profile.delete_all'), self)
-        actions['delete_all'].triggered.connect(
-            lambda: self.action_delete_all(event))
 
         menu = QMenu(self)
-        menu.addAction(actions['edit'])
-        menu.addAction(actions['use'])
-        menu.addAction(actions['duplicate'])
-        menu.addAction(actions['reset'])
+        # menu.addAction(actions['download'])  # not allowed for download files with purpose: assistants :(
+        menu.addAction(actions['rename'])
         menu.addAction(actions['delete'])
-        menu.addAction(actions['delete_all'])
 
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
+            self.window.controller.assistant.files.select(item.row())
             menu.exec_(event.globalPos())
 
-    def action_use(self, event):
-        """
-        Use action handler
-
-        :param event: mouse event
-        """
-        item = self.indexAt(event.pos())
-        idx = item.row()
-        if idx >= 0:
-            self.window.controller.settings.profile.select_by_idx(idx)
-
-    def action_duplicate(self, event):
+    def action_rename(self, event):
         """
-        Duplicate action handler
+        Rename action handler
 
         :param event: mouse event
         """
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
-            self.window.controller.settings.profile.duplicate_by_idx(idx)
+            self.window.controller.assistant.files.rename(idx)
 
-    def action_reset(self, event):
+    def action_download(self, event):
         """
-        Reset action handler
+        Download action handler
 
         :param event: mouse event
         """
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
-            self.window.controller.settings.profile.reset_by_idx(idx)
+            self.window.controller.assistant.files.download(idx)
 
     def action_delete(self, event):
         """
         Delete action handler
 
         :param event: mouse event
         """
         item = self.indexAt(event.pos())
         idx = item.row()
         if idx >= 0:
-            self.window.controller.settings.profile.delete_by_idx(idx)
-
-    def action_delete_all(self, event):
-        """
-        Delete all action handler
-
-        :param event: mouse event
-        """
-        item = self.indexAt(event.pos())
-        idx = item.row()
-        if idx >= 0:
-            self.window.controller.settings.profile.delete_all_by_idx(idx)
-
-    def action_edit(self, event):
-        """
-        Edit action handler
-
-        :param event: mouse event
-        """
-        item = self.indexAt(event.pos())
-        idx = item.row()
-        if idx >= 0:
-            self.window.controller.settings.profile.edit_by_idx(idx)
-
+            self.window.controller.assistant.files.delete(idx)
```

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/lists/settings.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/lists/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/checkbox.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/cmd.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/cmd.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/combo.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/dictionary.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/input.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/prompt.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/slider.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/option/textarea.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/option/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/tabs/Input.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/tabs/Input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/tabs/output.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/tabs/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/calendar_note.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/create.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/editor.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/find.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/input.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/name.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/name.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/notepad.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/output.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/rename.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/search_input.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/search_input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/textarea/web.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/textarea/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/ui/widget/vision/camera.py` & `pygpt_net-2.2.7/src/pygpt_net/ui/widget/vision/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/src/pygpt_net/utils.py` & `pygpt_net-2.2.7/src/pygpt_net/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.6/PKG-INFO` & `pygpt_net-2.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygpt-net
-Version: 2.2.6
+Version: 2.2.7
 Summary: Desktop AI Assistant powered by GPT-4, GPT-4V, GPT-3.5, DALL-E 3, Langchain LLMs, Llama-index, Whisper with chatbot, assistant, text completion, vision and image generation, internet access, chat with files, commands and code execution, file upload and download and more
 Home-page: https://github.com/szczyglis-dev/py-gpt
 License: MIT
 Keywords: py_gpt,py-gpt,pygpt,desktop,app,gpt,gpt4,gpt4-v,gpt3.5,gpt-4,gpt-4V,gpt-3.5,tts,whisper,vision,chatgpt,dall-e,chat,chatbot,assistant,text completion,image generation,ai,api,openai,api key,langchain,llama-index,presets,ui,qt,pyside
 Author: Marcin Szczyglinski
 Author-email: info@pygpt.net
 Requires-Python: >=3.10,<3.12
@@ -70,15 +70,15 @@
 Project-URL: Repository, https://github.com/szczyglis-dev/py-gpt
 Description-Content-Type: text/markdown
 
 # PyGPT - Desktop AI Assistant
 
 [![pygpt](https://snapcraft.io/pygpt/badge.svg)](https://snapcraft.io/pygpt)
 
-Release: **2.2.6** | build: **2024.04.30** | Python: **>=3.10, <3.12**
+Release: **2.2.7** | build: **2024.05.01** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -104,15 +104,15 @@
 
 You can download compiled 64-bit versions for Windows and Linux here: https://pygpt.net/#download
 
 ## Features
 
 - Desktop AI Assistant for `Linux`, `Windows` and `Mac`, written in Python.
 - Works similarly to `ChatGPT`, but locally (on a desktop computer).
-- 8 modes of operation: Chat, Vision, Completion, Assistant, Image generation, Langchain, Chat with files and Agent (autonomous).
+- 9 modes of operation: Chat, Vision, Completion, Assistant, Image generation, Langchain, Chat with files, Experts and Agent (autonomous).
 - Supports multiple models: `GPT-4`, `GPT-3.5`, and any model accessible through `Langchain`.
 - Handles and stores the full context of conversations (short-term memory).
 - Real-time video camera capture in Vision mode.
 - Internet access via `Google` and `Microsoft Bing`.
 - Speech synthesis via `Microsoft Azure`, `Google`, `Eleven Labs` and `OpenAI` Text-To-Speech services.
 - Speech recognition via `OpenAI Whisper`, `Google`, `Google Cloud` and `Microsoft Bing`.
 - Image analysis via `GPT-4 Vision`.
@@ -860,17 +860,17 @@
 **Twitter/X posts**  (web_twitter)
 
 - `bearer_token` - str, default: `None`
 - `num_tweets` - int, default: `100`
 
 ##  Agent (autonomous) 
 
-This mode is experimental.
+**This mode is experimental.**
 
-**WARNING: Please use this mode with caution!** - autonomous mode, when connected with other plugins, may produce unexpected results!
+**WARNING: Please use this mode with caution** - autonomous mode, when connected with other plugins, may produce unexpected results!
 
 The mode activates autonomous mode, where AI begins a conversation with itself. 
 You can set this loop to run for any number of iterations. Throughout this sequence, the model will engage
 in self-dialogue, answering his own questions and comments, in order to find the best possible solution, subjecting previously generated steps to criticism.
 
 ![v2_agent_toolbox](https://github.com/szczyglis-dev/py-gpt/assets/61396542/a0ae5d13-942e-4a18-9c53-33e7ad1886ff)
 
@@ -898,14 +898,47 @@
 If you want to use the Llama-index mode when running the agent, you can also specify which index `Llama-index` should use with the option:
 
 ```Settings / Agent (autonomous) / Index to use```
 
 ![v2_agent_settings](https://github.com/szczyglis-dev/py-gpt/assets/61396542/c577d219-eb25-4f0e-9ea5-adf20a6b6b81)
 
 
+##  Experts (co-op, co-operation mode)
+
+Added in version 2.2.7 (2024-05-01).
+
+**This mode is experimental.**
+
+Expert mode allows for the creation of experts (using presets) and then consulting them during a conversation. In this mode, a primary base context is created for conducting the conversation. From within this context, the model can make requests to an expert to perform a task and return the results to the main thread. When an expert is called in the background, a separate context is created for them with their own memory. This means that each expert, during the life of one main context, also has access to their own memory via their separate, isolated context.
+
+**In simple terms - you can imagine an expert as a separate, additional instance of the model running in the background, which can be called at any moment for assistance, with its own context and memory, as well as its own specialized instructions in a given subject.**
+
+Experts do not share contexts with one another, and the only point of contact between them is the main conversation thread. In this main thread, the model acts as a manager of experts, who can exchange data between them as needed.
+
+An expert is selected based on the name in the presets; for example, naming your expert as: ID = python_expert, name = "Python programmer" will create an expert whom the model will attempt to invoke for matters related to Python programming. You can also manually request to refer to a given expert:
+
+```bash
+Call the Python expert to generate some code.
+```
+
+Experts can be activated or deactivated - to enable or disable use RMB context menu to select the `Enable/Disable` options from the presets list. Only enabled experts are available to use in the thread.
+
+Experts can also be used in `Agent (autonomous)` mode - by creating a new agent using a preset. Simply move the appropriate experts to the active list to automatically make them available for use by the agent.
+
+You can also use experts in "inline" mode - by activating the `Experts (inline)` plugin. This allows for the use of experts in any mode, such as normal chat.
+
+Expert mode, like agent mode, is a "virtual" mode - you need to select a target mode of operation for it, which can be done in the settings at `Settings / Agent (autonomous) / Sub-mode for experts`.
+
+You can also ask for a list of active experts at any time:
+
+```bash
+Give me a list of active experts.
+```
+
+
 # Files and attachments
 
 ## Input attachments (upload)
 
 **PyGPT** makes it simple for users to upload files to the server and send them to the model for tasks like analysis, similar to attaching files in `ChatGPT`. There's a separate `Files` tab next to the text input area specifically for managing file uploads. Users can opt to have files automatically deleted after each upload or keep them on the list for repeated use.
 
 ![v2_file_input](https://github.com/szczyglis-dev/py-gpt/assets/61396542/bd3d9840-2bc4-4ba8-a603-69724f9eb620)
@@ -2835,18 +2868,22 @@
 
 - `Command execute: extra footer (Assistant mode only)`: PAdditional instructions to separate local commands from the remote environment that is already configured in the Assistants.
 
 - `Context: auto-summary (system prompt)`: System prompt for context auto-summary.
 
 - `Context: auto-summary (user message)`: User message for context auto-summary. Placeholders: {input}, {output}
 
-- `Agent: continue`: Prompt sent to automatically continue the conversation. Default: `continue...`
+- `Agent: system instruction`: Prompt to instruct how to handle autonomous mode.
+
+- `Agent: continue`: Prompt sent to automatically continue the conversation.
 
 - `Agent: goal update`: Prompt to instruct how to update current goal status.
 
+- `Experts: Master prompt`: Prompt to instruct how to handle experts.
+
 - `DALL-E: image generate`: Prompt for generating prompts for DALL-E (if raw-mode is disabled).
 
 **Images**
 
 - `DALL-E Image size`: The resolution of the generated images (DALL-E). Default: 1792x1024.
 
 - `DALL-E Image quality`: The image quality of the generated images (DALL-E). Default: standard.
@@ -2905,14 +2942,16 @@
 
 - `DB (ALL), DB (UPDATE), FILES (ALL)`: Index the data – batch indexing is available here.
 
 **Agent (autonomous)**
 
 - `Sub-mode to use`: Sub-mode to use in Agent mode (chat, completion, langchain, llama_index, etc.). Default: chat.
 
+- `Sub-mode for experts`: Sub-mode to use in Experts mode (chat, completion, langchain, llama_index, etc.). Default: chat.
+
 - `Index to use`: Only if sub-mode is llama_index (Chat with files), choose the index to use in Agent mode.
 
 - `Display a tray notification when the goal is achieved.`: If enabled, a notification will be displayed after goal achieved / finished run.
 
 **Updates**
 
 - `Check for updates on start`: Enables checking for updates on start. Default: True.
@@ -3128,14 +3167,22 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+**2.2.7 (2024-05-01)**
+
+- A new experimental work mode has been added: 'Experts', which allows the creation of separate background instances with their own instructions that can be consulted for help. See the documentation: 'Work Modes / Experts'.
+- Added a new plugin: 'Experts (inline)`.
+- Improved the Agent mode by adding the ability to configure and invoke defined Experts.
+- Improved the prompts that control the autonomous mode.
+- The main prompt controlling the agents has been moved from presets to the application's settings window.
+
 **2.2.6 (2024-04-30)**
 
 - Added a new model: 'gpt-4-turbo'.
 - Vision integrated into Chat mode, without any plugins, if the model supports Vision - currently available for: 'gpt-4-turbo' and 'gpt-4-turbo-2024-04-09'.
 - Store importer connected with Logger.
 - Fixed: issue with batch unassigning remote files from vector stores.
```

