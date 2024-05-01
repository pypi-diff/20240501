# Comparing `tmp/kathara-3.7.4.tar.gz` & `tmp/kathara-3.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kathara-3.7.4.tar", last modified: Wed Mar 27 16:34:42 2024, max compression
+gzip compressed data, was "kathara-3.7.5.tar", last modified: Wed May  1 13:04:59 2024, max compression
```

## Comparing `kathara-3.7.4.tar` & `kathara-3.7.5.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.162779 kathara-3.7.4/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    35141 2023-12-20 16:03:43.000000 kathara-3.7.4/LICENSE
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    51434 2024-03-27 16:34:42.162779 kathara-3.7.4/PKG-INFO
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8999 2024-01-30 16:39:45.000000 kathara-3.7.4/README.md
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1811 2024-03-27 16:34:08.000000 kathara-3.7.4/pyproject.toml
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      730 2024-03-27 16:34:42.162779 kathara-3.7.4/setup.cfg
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1562 2024-03-27 16:34:08.000000 kathara-3.7.4/setup.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.092779 kathara-3.7.4/src/
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.092779 kathara-3.7.4/src/Kathara/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.102779 kathara-3.7.4/src/Kathara/auth/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2398 2023-12-28 15:09:31.000000 kathara-3.7.4/src/Kathara/auth/PrivilegeHandler.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/auth/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.102779 kathara-3.7.4/src/Kathara/cli/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/cli/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.102779 kathara-3.7.4/src/Kathara/cli/command/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2736 2024-02-01 11:32:57.000000 kathara-3.7.4/src/Kathara/cli/command/CheckCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2498 2024-02-01 11:32:57.000000 kathara-3.7.4/src/Kathara/cli/command/ConnectCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3665 2024-02-07 10:18:30.000000 kathara-3.7.4/src/Kathara/cli/command/ExecCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1897 2024-01-31 16:39:33.000000 kathara-3.7.4/src/Kathara/cli/command/LcleanCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3296 2024-01-31 16:39:33.000000 kathara-3.7.4/src/Kathara/cli/command/LconfigCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5473 2024-02-07 18:30:28.000000 kathara-3.7.4/src/Kathara/cli/command/LinfoCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2785 2024-02-01 11:32:57.000000 kathara-3.7.4/src/Kathara/cli/command/ListCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4343 2024-02-28 16:38:46.000000 kathara-3.7.4/src/Kathara/cli/command/LrestartCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8513 2024-03-07 16:57:10.000000 kathara-3.7.4/src/Kathara/cli/command/LstartCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4731 2024-01-31 16:39:33.000000 kathara-3.7.4/src/Kathara/cli/command/LtestCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      350 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/cli/command/SettingsCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1339 2024-01-31 16:39:33.000000 kathara-3.7.4/src/Kathara/cli/command/VcleanCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3073 2024-02-07 18:14:55.000000 kathara-3.7.4/src/Kathara/cli/command/VconfigCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7321 2024-02-05 13:22:31.000000 kathara-3.7.4/src/Kathara/cli/command/VstartCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2076 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/cli/command/WipeCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/cli/command/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.102779 kathara-3.7.4/src/Kathara/cli/ui/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/cli/ui/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.112779 kathara-3.7.4/src/Kathara/cli/ui/event/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3466 2024-01-30 16:39:45.000000 kathara-3.7.4/src/Kathara/cli/ui/event/HandleDockerImagePull.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1204 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/cli/ui/event/HandleMachineTerminal.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2005 2024-01-30 16:39:45.000000 kathara-3.7.4/src/Kathara/cli/ui/event/HandleProgressBar.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1058 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/cli/ui/event/UpdateDockerImage.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/cli/ui/event/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4677 2024-01-30 16:39:45.000000 kathara-3.7.4/src/Kathara/cli/ui/event/register.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.112779 kathara-3.7.4/src/Kathara/cli/ui/setting/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    16110 2024-03-07 16:57:10.000000 kathara-3.7.4/src/Kathara/cli/ui/setting/CommonOptionsHandler.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11580 2023-12-28 15:09:31.000000 kathara-3.7.4/src/Kathara/cli/ui/setting/DockerOptionsHandler.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     6410 2023-12-28 15:09:31.000000 kathara-3.7.4/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1499 2023-12-28 15:09:31.000000 kathara-3.7.4/src/Kathara/cli/ui/setting/SettingsMenuFactory.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/cli/ui/setting/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4252 2023-12-28 15:09:31.000000 kathara-3.7.4/src/Kathara/cli/ui/setting/utils.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7696 2024-03-07 16:57:10.000000 kathara-3.7.4/src/Kathara/cli/ui/utils.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      623 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/decorators.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.112779 kathara-3.7.4/src/Kathara/event/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3328 2024-02-01 16:18:27.000000 kathara-3.7.4/src/Kathara/event/EventDispatcher.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/event/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4227 2024-03-27 16:34:08.000000 kathara-3.7.4/src/Kathara/exceptions.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.112779 kathara-3.7.4/src/Kathara/foundation/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.112779 kathara-3.7.4/src/Kathara/foundation/cli/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      741 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/cli/CliArgs.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/cli/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.112779 kathara-3.7.4/src/Kathara/foundation/cli/command/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1102 2024-02-01 11:32:57.000000 kathara-3.7.4/src/Kathara/foundation/cli/command/Command.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      205 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/cli/command/CommandFactory.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/cli/command/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.112779 kathara-3.7.4/src/Kathara/foundation/cli/ui/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/cli/ui/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.112779 kathara-3.7.4/src/Kathara/foundation/cli/ui/setting/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1023 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      233 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/cli/ui/setting/OptionsHandlerFactory.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/cli/ui/setting/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.112779 kathara-3.7.4/src/Kathara/foundation/factory/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1010 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/factory/Factory.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/factory/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.112779 kathara-3.7.4/src/Kathara/foundation/manager/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    27782 2024-02-07 12:09:50.000000 kathara-3.7.4/src/Kathara/foundation/manager/IManager.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      213 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/manager/ManagerFactory.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/manager/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.122779 kathara-3.7.4/src/Kathara/foundation/manager/stats/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      681 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/manager/stats/ILinkStats.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      674 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/manager/stats/IMachineStats.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/manager/stats/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.122779 kathara-3.7.4/src/Kathara/foundation/manager/terminal/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2095 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/manager/terminal/Terminal.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/manager/terminal/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1178 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/manager/terminal/terminal_utils.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.122779 kathara-3.7.4/src/Kathara/foundation/model/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    12035 2024-03-07 16:57:10.000000 kathara-3.7.4/src/Kathara/foundation/model/FilesystemMixin.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/model/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.122779 kathara-3.7.4/src/Kathara/foundation/setting/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      749 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/setting/SettingsAddon.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      228 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/setting/SettingsAddonFactory.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/setting/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.122779 kathara-3.7.4/src/Kathara/foundation/test/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1929 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/test/Test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/foundation/test/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.122779 kathara-3.7.4/src/Kathara/manager/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    29788 2024-03-07 16:57:10.000000 kathara-3.7.4/src/Kathara/manager/Kathara.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.122779 kathara-3.7.4/src/Kathara/manager/docker/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7953 2024-01-30 16:39:45.000000 kathara-3.7.4/src/Kathara/manager/docker/DockerImage.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    16840 2024-03-07 16:57:10.000000 kathara-3.7.4/src/Kathara/manager/docker/DockerLink.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    44535 2024-03-27 16:34:08.000000 kathara-3.7.4/src/Kathara/manager/docker/DockerMachine.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    46200 2024-03-27 16:34:08.000000 kathara-3.7.4/src/Kathara/manager/docker/DockerManager.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7007 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/docker/DockerPlugin.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/docker/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.122779 kathara-3.7.4/src/Kathara/manager/docker/stats/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3514 2024-01-31 16:39:33.000000 kathara-3.7.4/src/Kathara/manager/docker/stats/DockerLinkStats.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5392 2024-01-31 16:39:33.000000 kathara-3.7.4/src/Kathara/manager/docker/stats/DockerMachineStats.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/docker/stats/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.122779 kathara-3.7.4/src/Kathara/manager/docker/terminal/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2205 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1157 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/docker/terminal/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.132779 kathara-3.7.4/src/Kathara/manager/kubernetes/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1924 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/kubernetes/KubernetesConfig.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4252 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/kubernetes/KubernetesConfigMap.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    14235 2024-01-31 16:39:33.000000 kathara-3.7.4/src/Kathara/manager/kubernetes/KubernetesLink.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    39334 2024-03-27 16:34:08.000000 kathara-3.7.4/src/Kathara/manager/kubernetes/KubernetesMachine.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    41853 2024-03-07 16:57:10.000000 kathara-3.7.4/src/Kathara/manager/kubernetes/KubernetesManager.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4366 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/kubernetes/KubernetesNamespace.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/kubernetes/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.132779 kathara-3.7.4/src/Kathara/manager/kubernetes/stats/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2144 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3444 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/kubernetes/stats/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.132779 kathara-3.7.4/src/Kathara/manager/kubernetes/terminal/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2418 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/manager/kubernetes/terminal/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.132779 kathara-3.7.4/src/Kathara/model/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1975 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/model/ExternalLink.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1421 2023-12-28 15:09:31.000000 kathara-3.7.4/src/Kathara/model/Interface.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    18091 2024-03-11 14:51:48.000000 kathara-3.7.4/src/Kathara/model/Lab.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1252 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/model/Link.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    27150 2024-03-07 16:57:10.000000 kathara-3.7.4/src/Kathara/model/Machine.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/model/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.132779 kathara-3.7.4/src/Kathara/os/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7556 2024-03-27 16:34:08.000000 kathara-3.7.4/src/Kathara/os/Networking.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/os/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.132779 kathara-3.7.4/src/Kathara/parser/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/parser/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.142779 kathara-3.7.4/src/Kathara/parser/netkit/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2658 2023-12-28 15:09:31.000000 kathara-3.7.4/src/Kathara/parser/netkit/DepParser.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2665 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/parser/netkit/ExtParser.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1146 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/parser/netkit/FolderParser.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4003 2024-01-08 16:37:41.000000 kathara-3.7.4/src/Kathara/parser/netkit/LabParser.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      903 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/parser/netkit/OptionParser.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/parser/netkit/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.142779 kathara-3.7.4/src/Kathara/setting/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11571 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/setting/Setting.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/setting/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.142779 kathara-3.7.4/src/Kathara/setting/addon/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1445 2023-12-28 15:09:31.000000 kathara-3.7.4/src/Kathara/setting/addon/DockerSettingsAddon.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      906 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/setting/addon/KubernetesSettingsAddon.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/setting/addon/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1426 2024-01-31 16:39:33.000000 kathara-3.7.4/src/Kathara/strings.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.142779 kathara-3.7.4/src/Kathara/test/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5449 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/test/BuiltinTest.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4534 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/test/UserTest.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/test/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.142779 kathara-3.7.4/src/Kathara/trdparty/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.142779 kathara-3.7.4/src/Kathara/trdparty/consolemenu/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      519 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    15168 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/console_menu.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.152779 kathara-3.7.4/src/Kathara/trdparty/consolemenu/format/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      850 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/format/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    14430 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/format/menu_borders.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1502 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/format/menu_margins.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1445 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/format/menu_padding.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3760 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/format/menu_style.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.152779 kathara-3.7.4/src/Kathara/trdparty/consolemenu/items/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      385 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/items/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1335 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/items/command_item.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      803 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/items/external_item.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1353 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/items/function_item.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      595 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/items/selection_item.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1596 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/items/submenu_item.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13445 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/menu_component.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11425 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/menu_formatter.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3281 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/multiselect_menu.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    12321 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/prompt_utils.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1805 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/screen.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2772 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/selection_menu.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.152779 kathara-3.7.4/src/Kathara/trdparty/consolemenu/validators/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/validators/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      765 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/validators/base.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1009 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/validators/regex.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      558 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/validators/url.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       22 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/consolemenu/version.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.152779 kathara-3.7.4/src/Kathara/trdparty/depgen/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/depgen/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2992 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/depgen/depgen.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.152779 kathara-3.7.4/src/Kathara/trdparty/libtmux/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/libtmux/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2738 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/libtmux/tmux.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.152779 kathara-3.7.4/src/Kathara/trdparty/nsenter/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/nsenter/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5895 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/nsenter/nsenter.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.152779 kathara-3.7.4/src/Kathara/trdparty/strtobool/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/strtobool/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      692 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/trdparty/strtobool/strtobool.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      889 2023-12-28 15:09:31.000000 kathara-3.7.4/src/Kathara/types.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    10514 2024-03-27 16:34:08.000000 kathara-3.7.4/src/Kathara/utils.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.152779 kathara-3.7.4/src/Kathara/validator/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      599 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/validator/ImageValidator.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      457 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/validator/TerminalValidator.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/validator/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      308 2024-03-27 16:34:08.000000 kathara-3.7.4/src/Kathara/version.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.152779 kathara-3.7.4/src/Kathara/webhooks/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3470 2024-01-30 16:39:45.000000 kathara-3.7.4/src/Kathara/webhooks/DockerHubApi.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      795 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/webhooks/GitHubApi.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.4/src/Kathara/webhooks/__init__.py
-drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-03-27 16:34:42.152779 kathara-3.7.4/src/kathara.egg-info/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    51434 2024-03-27 16:34:42.000000 kathara-3.7.4/src/kathara.egg-info/PKG-INFO
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7036 2024-03-27 16:34:42.000000 kathara-3.7.4/src/kathara.egg-info/SOURCES.txt
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        1 2024-03-27 16:34:42.000000 kathara-3.7.4/src/kathara.egg-info/dependency_links.txt
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      337 2024-03-27 16:34:42.000000 kathara-3.7.4/src/kathara.egg-info/requires.txt
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       16 2024-03-27 16:34:42.000000 kathara-3.7.4/src/kathara.egg-info/top_level.txt
--rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     4445 2024-02-05 13:17:40.000000 kathara-3.7.4/src/kathara.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.103128 kathara-3.7.5/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    35141 2023-12-20 16:03:43.000000 kathara-3.7.5/LICENSE
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    51374 2024-05-01 13:04:59.103128 kathara-3.7.5/PKG-INFO
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8939 2024-04-18 10:27:34.000000 kathara-3.7.5/README.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1811 2024-05-01 13:04:22.000000 kathara-3.7.5/pyproject.toml
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      730 2024-05-01 13:04:59.103128 kathara-3.7.5/setup.cfg
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1562 2024-05-01 13:04:22.000000 kathara-3.7.5/setup.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.053126 kathara-3.7.5/src/
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.053126 kathara-3.7.5/src/Kathara/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.053126 kathara-3.7.5/src/Kathara/auth/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2398 2023-12-28 15:09:31.000000 kathara-3.7.5/src/Kathara/auth/PrivilegeHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/auth/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.053126 kathara-3.7.5/src/Kathara/cli/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/cli/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.063127 kathara-3.7.5/src/Kathara/cli/command/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2736 2024-02-01 11:32:57.000000 kathara-3.7.5/src/Kathara/cli/command/CheckCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2498 2024-02-01 11:32:57.000000 kathara-3.7.5/src/Kathara/cli/command/ConnectCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3665 2024-02-07 10:18:30.000000 kathara-3.7.5/src/Kathara/cli/command/ExecCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1897 2024-01-31 16:39:33.000000 kathara-3.7.5/src/Kathara/cli/command/LcleanCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3296 2024-01-31 16:39:33.000000 kathara-3.7.5/src/Kathara/cli/command/LconfigCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5473 2024-02-07 18:30:28.000000 kathara-3.7.5/src/Kathara/cli/command/LinfoCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2785 2024-02-01 11:32:57.000000 kathara-3.7.5/src/Kathara/cli/command/ListCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4343 2024-02-28 16:38:46.000000 kathara-3.7.5/src/Kathara/cli/command/LrestartCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8513 2024-03-07 16:57:10.000000 kathara-3.7.5/src/Kathara/cli/command/LstartCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4731 2024-01-31 16:39:33.000000 kathara-3.7.5/src/Kathara/cli/command/LtestCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      350 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/cli/command/SettingsCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1339 2024-01-31 16:39:33.000000 kathara-3.7.5/src/Kathara/cli/command/VcleanCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3073 2024-02-07 18:14:55.000000 kathara-3.7.5/src/Kathara/cli/command/VconfigCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7321 2024-02-05 13:22:31.000000 kathara-3.7.5/src/Kathara/cli/command/VstartCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2076 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/cli/command/WipeCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/cli/command/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.063127 kathara-3.7.5/src/Kathara/cli/ui/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/cli/ui/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.063127 kathara-3.7.5/src/Kathara/cli/ui/event/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3466 2024-01-30 16:39:45.000000 kathara-3.7.5/src/Kathara/cli/ui/event/HandleDockerImagePull.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1204 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/cli/ui/event/HandleMachineTerminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2005 2024-01-30 16:39:45.000000 kathara-3.7.5/src/Kathara/cli/ui/event/HandleProgressBar.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1058 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/cli/ui/event/UpdateDockerImage.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/cli/ui/event/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4677 2024-01-30 16:39:45.000000 kathara-3.7.5/src/Kathara/cli/ui/event/register.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.063127 kathara-3.7.5/src/Kathara/cli/ui/setting/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    16110 2024-03-07 16:57:10.000000 kathara-3.7.5/src/Kathara/cli/ui/setting/CommonOptionsHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11580 2023-12-28 15:09:31.000000 kathara-3.7.5/src/Kathara/cli/ui/setting/DockerOptionsHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     6410 2023-12-28 15:09:31.000000 kathara-3.7.5/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1499 2023-12-28 15:09:31.000000 kathara-3.7.5/src/Kathara/cli/ui/setting/SettingsMenuFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/cli/ui/setting/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4252 2023-12-28 15:09:31.000000 kathara-3.7.5/src/Kathara/cli/ui/setting/utils.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7696 2024-03-07 16:57:10.000000 kathara-3.7.5/src/Kathara/cli/ui/utils.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      623 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/decorators.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.063127 kathara-3.7.5/src/Kathara/event/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3328 2024-02-01 16:18:27.000000 kathara-3.7.5/src/Kathara/event/EventDispatcher.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/event/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4227 2024-03-27 16:34:08.000000 kathara-3.7.5/src/Kathara/exceptions.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.063127 kathara-3.7.5/src/Kathara/foundation/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.063127 kathara-3.7.5/src/Kathara/foundation/cli/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      741 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/cli/CliArgs.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/cli/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.063127 kathara-3.7.5/src/Kathara/foundation/cli/command/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1102 2024-02-01 11:32:57.000000 kathara-3.7.5/src/Kathara/foundation/cli/command/Command.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      205 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/cli/command/CommandFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/cli/command/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.063127 kathara-3.7.5/src/Kathara/foundation/cli/ui/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/cli/ui/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.073127 kathara-3.7.5/src/Kathara/foundation/cli/ui/setting/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1023 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      233 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/cli/ui/setting/OptionsHandlerFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/cli/ui/setting/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.073127 kathara-3.7.5/src/Kathara/foundation/factory/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1010 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/factory/Factory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/factory/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.073127 kathara-3.7.5/src/Kathara/foundation/manager/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    27782 2024-02-07 12:09:50.000000 kathara-3.7.5/src/Kathara/foundation/manager/IManager.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      213 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/manager/ManagerFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/manager/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.073127 kathara-3.7.5/src/Kathara/foundation/manager/stats/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      681 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/manager/stats/ILinkStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      674 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/manager/stats/IMachineStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/manager/stats/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.073127 kathara-3.7.5/src/Kathara/foundation/manager/terminal/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2095 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/manager/terminal/Terminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/manager/terminal/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1178 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/manager/terminal/terminal_utils.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.073127 kathara-3.7.5/src/Kathara/foundation/model/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    12035 2024-03-07 16:57:10.000000 kathara-3.7.5/src/Kathara/foundation/model/FilesystemMixin.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/model/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.073127 kathara-3.7.5/src/Kathara/foundation/setting/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      749 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/setting/SettingsAddon.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      228 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/setting/SettingsAddonFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/setting/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.073127 kathara-3.7.5/src/Kathara/foundation/test/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1929 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/test/Test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/foundation/test/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.073127 kathara-3.7.5/src/Kathara/manager/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    29788 2024-03-07 16:57:10.000000 kathara-3.7.5/src/Kathara/manager/Kathara.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.073127 kathara-3.7.5/src/Kathara/manager/docker/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7953 2024-01-30 16:39:45.000000 kathara-3.7.5/src/Kathara/manager/docker/DockerImage.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    16840 2024-03-07 16:57:10.000000 kathara-3.7.5/src/Kathara/manager/docker/DockerLink.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    44394 2024-05-01 13:04:22.000000 kathara-3.7.5/src/Kathara/manager/docker/DockerMachine.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    46641 2024-05-01 13:04:22.000000 kathara-3.7.5/src/Kathara/manager/docker/DockerManager.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7007 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/docker/DockerPlugin.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/docker/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.083127 kathara-3.7.5/src/Kathara/manager/docker/stats/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3514 2024-01-31 16:39:33.000000 kathara-3.7.5/src/Kathara/manager/docker/stats/DockerLinkStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5392 2024-01-31 16:39:33.000000 kathara-3.7.5/src/Kathara/manager/docker/stats/DockerMachineStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/docker/stats/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.083127 kathara-3.7.5/src/Kathara/manager/docker/terminal/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2205 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1157 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/docker/terminal/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.083127 kathara-3.7.5/src/Kathara/manager/kubernetes/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1924 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/kubernetes/KubernetesConfig.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4252 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/kubernetes/KubernetesConfigMap.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    14235 2024-01-31 16:39:33.000000 kathara-3.7.5/src/Kathara/manager/kubernetes/KubernetesLink.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    39334 2024-03-27 16:34:08.000000 kathara-3.7.5/src/Kathara/manager/kubernetes/KubernetesMachine.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    41853 2024-03-07 16:57:10.000000 kathara-3.7.5/src/Kathara/manager/kubernetes/KubernetesManager.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4366 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/kubernetes/KubernetesNamespace.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/kubernetes/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.083127 kathara-3.7.5/src/Kathara/manager/kubernetes/stats/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2144 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3444 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/kubernetes/stats/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.083127 kathara-3.7.5/src/Kathara/manager/kubernetes/terminal/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2418 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/manager/kubernetes/terminal/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.083127 kathara-3.7.5/src/Kathara/model/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1975 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/model/ExternalLink.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1421 2023-12-28 15:09:31.000000 kathara-3.7.5/src/Kathara/model/Interface.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    18091 2024-04-19 12:30:29.000000 kathara-3.7.5/src/Kathara/model/Lab.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1252 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/model/Link.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    27150 2024-03-07 16:57:10.000000 kathara-3.7.5/src/Kathara/model/Machine.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/model/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.083127 kathara-3.7.5/src/Kathara/os/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7556 2024-03-27 16:34:08.000000 kathara-3.7.5/src/Kathara/os/Networking.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/os/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.083127 kathara-3.7.5/src/Kathara/parser/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/parser/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.083127 kathara-3.7.5/src/Kathara/parser/netkit/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2658 2023-12-28 15:09:31.000000 kathara-3.7.5/src/Kathara/parser/netkit/DepParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2665 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/parser/netkit/ExtParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1146 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/parser/netkit/FolderParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4003 2024-01-08 16:37:41.000000 kathara-3.7.5/src/Kathara/parser/netkit/LabParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      903 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/parser/netkit/OptionParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/parser/netkit/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.093128 kathara-3.7.5/src/Kathara/setting/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11571 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/setting/Setting.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/setting/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.093128 kathara-3.7.5/src/Kathara/setting/addon/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1445 2023-12-28 15:09:31.000000 kathara-3.7.5/src/Kathara/setting/addon/DockerSettingsAddon.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      906 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/setting/addon/KubernetesSettingsAddon.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/setting/addon/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1426 2024-01-31 16:39:33.000000 kathara-3.7.5/src/Kathara/strings.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.093128 kathara-3.7.5/src/Kathara/test/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5449 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/test/BuiltinTest.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4534 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/test/UserTest.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/test/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.093128 kathara-3.7.5/src/Kathara/trdparty/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.093128 kathara-3.7.5/src/Kathara/trdparty/consolemenu/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      519 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    15168 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/console_menu.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.093128 kathara-3.7.5/src/Kathara/trdparty/consolemenu/format/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      850 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/format/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    14430 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/format/menu_borders.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1502 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/format/menu_margins.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1445 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/format/menu_padding.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3760 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/format/menu_style.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.103128 kathara-3.7.5/src/Kathara/trdparty/consolemenu/items/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      385 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/items/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1335 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/items/command_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      803 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/items/external_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1353 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/items/function_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      595 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/items/selection_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1596 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/items/submenu_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13445 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/menu_component.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11425 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/menu_formatter.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3281 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/multiselect_menu.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    12321 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/prompt_utils.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1805 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/screen.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2772 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/selection_menu.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.103128 kathara-3.7.5/src/Kathara/trdparty/consolemenu/validators/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/validators/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      765 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/validators/base.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1009 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/validators/regex.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      558 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/validators/url.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       22 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/consolemenu/version.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.103128 kathara-3.7.5/src/Kathara/trdparty/depgen/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/depgen/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2992 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/depgen/depgen.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.103128 kathara-3.7.5/src/Kathara/trdparty/libtmux/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/libtmux/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2738 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/libtmux/tmux.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.103128 kathara-3.7.5/src/Kathara/trdparty/nsenter/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/nsenter/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5895 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/nsenter/nsenter.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.103128 kathara-3.7.5/src/Kathara/trdparty/strtobool/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/strtobool/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      692 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/trdparty/strtobool/strtobool.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      889 2023-12-28 15:09:31.000000 kathara-3.7.5/src/Kathara/types.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    10514 2024-03-27 16:34:08.000000 kathara-3.7.5/src/Kathara/utils.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.103128 kathara-3.7.5/src/Kathara/validator/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      599 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/validator/ImageValidator.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      457 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/validator/TerminalValidator.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/validator/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      308 2024-05-01 13:04:22.000000 kathara-3.7.5/src/Kathara/version.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.103128 kathara-3.7.5/src/Kathara/webhooks/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3470 2024-01-30 16:39:45.000000 kathara-3.7.5/src/Kathara/webhooks/DockerHubApi.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      795 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/webhooks/GitHubApi.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-12-20 16:03:43.000000 kathara-3.7.5/src/Kathara/webhooks/__init__.py
+drwxr-xr-x   0 tommaso   (1000) tommaso   (1000)        0 2024-05-01 13:04:59.103128 kathara-3.7.5/src/kathara.egg-info/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    51374 2024-05-01 13:04:59.000000 kathara-3.7.5/src/kathara.egg-info/PKG-INFO
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7036 2024-05-01 13:04:59.000000 kathara-3.7.5/src/kathara.egg-info/SOURCES.txt
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        1 2024-05-01 13:04:59.000000 kathara-3.7.5/src/kathara.egg-info/dependency_links.txt
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      337 2024-05-01 13:04:59.000000 kathara-3.7.5/src/kathara.egg-info/requires.txt
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       16 2024-05-01 13:04:59.000000 kathara-3.7.5/src/kathara.egg-info/top_level.txt
+-rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     4445 2024-02-05 13:17:40.000000 kathara-3.7.5/src/kathara.py
```

### Comparing `kathara-3.7.4/LICENSE` & `kathara-3.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/PKG-INFO` & `kathara-3.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kathara
-Version: 3.7.4
+Version: 3.7.5
 Summary: A lightweight container-based network emulation tool.
 Home-page: https://www.kathara.org
-Download-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.7.4.tar.gz
+Download-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.7.5.tar.gz
 Author: Kathara Framework
 Author-email: Kathara Framework <contact@kathara.org>
 Maintainer-email: Tommaso Caiazzi <contact@kathara.org>, Mariano Scazzariello <contact@kathara.org>, Lorenzo Ariemma <contact@kathara.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -806,16 +806,14 @@
 
 - [Netkit Lab Generator](https://github.com/KatharaFramework/Netkit-Lab-Generator), a GUI that allows the easy creation of a network scenario configuration and the visualization of its network topology.
 - [VFTGen](https://github.com/KatharaFramework/VFTGen), a tool that allows to create three levels Fat Tree topologies (single-plane or multi-planes) and automatically configure them to run on Kathará.
 - [Tacatá](https://github.com/damiano-massarelli/Tacata), a lightweight Python script which creates Netkit and Kathará labs using an enriched version of the lab.conf file with a simple syntax.
 - [net-vis](https://github.com/Friscobuffo/net-vis-localhost), a tool that parses (and generates) the `lab.conf` file and all the `.startup` files to visualize the network.
 - [kathara-lab-starter](https://github.com/BuonHobo/kathara-lab-starter), an easy and extensible tool to get a kathara lab started.  Utilizing JSON input files, it accelerates setup, while minimizing configuration redundancies.
 
-Being based on Netkit, all the previous tools still work. 
-
 ## Success Stories
 As far as we know, Kathará is currently being used in many [courses and projects](https://www.kathara.org/stories.html). 
  
 We encourage you to tell us your story! 
 
 We are also collecting network scenarios from the community. If you want to be added to the [list](https://github.com/KatharaFramework/Kathara-Labs/tree/main/community-labs), please contact us!
```

### Comparing `kathara-3.7.4/README.md` & `kathara-3.7.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,14 @@
 
 - [Netkit Lab Generator](https://github.com/KatharaFramework/Netkit-Lab-Generator), a GUI that allows the easy creation of a network scenario configuration and the visualization of its network topology.
 - [VFTGen](https://github.com/KatharaFramework/VFTGen), a tool that allows to create three levels Fat Tree topologies (single-plane or multi-planes) and automatically configure them to run on Kathará.
 - [Tacatá](https://github.com/damiano-massarelli/Tacata), a lightweight Python script which creates Netkit and Kathará labs using an enriched version of the lab.conf file with a simple syntax.
 - [net-vis](https://github.com/Friscobuffo/net-vis-localhost), a tool that parses (and generates) the `lab.conf` file and all the `.startup` files to visualize the network.
 - [kathara-lab-starter](https://github.com/BuonHobo/kathara-lab-starter), an easy and extensible tool to get a kathara lab started.  Utilizing JSON input files, it accelerates setup, while minimizing configuration redundancies.
 
-Being based on Netkit, all the previous tools still work. 
-
 ## Success Stories
 As far as we know, Kathará is currently being used in many [courses and projects](https://www.kathara.org/stories.html). 
  
 We encourage you to tell us your story! 
 
 We are also collecting network scenarios from the community. If you want to be added to the [list](https://github.com/KatharaFramework/Kathara-Labs/tree/main/community-labs), please contact us!
```

#### html2text {}

```diff
@@ -80,17 +80,16 @@
 (https://github.com/damiano-massarelli/Tacata), a lightweight Python script
 which creates Netkit and KatharÃ¡ labs using an enriched version of the
 lab.conf file with a simple syntax. - [net-vis](https://github.com/Friscobuffo/
 net-vis-localhost), a tool that parses (and generates) the `lab.conf` file and
 all the `.startup` files to visualize the network. - [kathara-lab-starter]
 (https://github.com/BuonHobo/kathara-lab-starter), an easy and extensible tool
 to get a kathara lab started. Utilizing JSON input files, it accelerates setup,
-while minimizing configuration redundancies. Being based on Netkit, all the
-previous tools still work. ## Success Stories As far as we know, KatharÃ¡ is
-currently being used in many [courses and projects](https://www.kathara.org/
-stories.html). We encourage you to tell us your story! We are also collecting
-network scenarios from the community. If you want to be added to the [list]
-(https://github.com/KatharaFramework/Kathara-Labs/tree/main/community-labs),
-please contact us! ## Join Us KatharÃ¡ is an open source project. Feel free to
-download the code, play with it, and submit feature requests, notify bugs, or
-open pull requests! Thanks to everyone who has contributed to the development
-of KatharÃ¡!
+while minimizing configuration redundancies. ## Success Stories As far as we
+know, KatharÃ¡ is currently being used in many [courses and projects](https://
+www.kathara.org/stories.html). We encourage you to tell us your story! We are
+also collecting network scenarios from the community. If you want to be added
+to the [list](https://github.com/KatharaFramework/Kathara-Labs/tree/main/
+community-labs), please contact us! ## Join Us KatharÃ¡ is an open source
+project. Feel free to download the code, play with it, and submit feature
+requests, notify bugs, or open pull requests! Thanks to everyone who has
+contributed to the development of KatharÃ¡!
```

### Comparing `kathara-3.7.4/pyproject.toml` & `kathara-3.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kathara"
-version = "3.7.4"
+version = "3.7.5"
 description = "A lightweight container-based network emulation tool."
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 keywords = ["NETWORK-EMULATION", "CONTAINERS", "NFV"]
 authors = [
     { name = "Kathara Framework", email = "contact@kathara.org" }
```

### Comparing `kathara-3.7.4/setup.cfg` & `kathara-3.7.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kathara
-version = 3.7.4
+version = 3.7.5
 author = Kathara Framework
 author_email = contact@kathara.org
 description = A lightweight container-based network emulation tool.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = www.kathara.org
 project_urls =
```

### Comparing `kathara-3.7.4/setup.py` & `kathara-3.7.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from setuptools import find_packages
 
 setup(
     name='kathara',
     package_dir={'': 'src'},
     packages=find_packages('src'),
     py_modules=['kathara'],
-    version='3.7.4',
+    version='3.7.5',
     license='gpl-3.0',
     description='A lightweight container-based network emulation tool.',
     author='Kathara Framework',
     author_email='contact@kathara.org',
     url='https://www.kathara.org',
-    download_url='https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.7.4.tar.gz',
+    download_url='https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.7.5.tar.gz',
     keywords=['NETWORK-EMULATION', 'CONTAINERS', 'NFV'],
     install_requires=[
         "binaryornot>=0.4.4",
         "docker>=7.0.0",
         "kubernetes>=23.3.0",
         "requests>=2.22.0",
         "slug>=2.0",
```

### Comparing `kathara-3.7.4/src/Kathara/auth/PrivilegeHandler.py` & `kathara-3.7.5/src/Kathara/auth/PrivilegeHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/CheckCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/CheckCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/ConnectCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/ConnectCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/ExecCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/ExecCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/LcleanCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/LcleanCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/LconfigCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/LconfigCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/LinfoCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/LinfoCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/ListCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/ListCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/LrestartCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/LrestartCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/LstartCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/LstartCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/LtestCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/LtestCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/VcleanCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/VcleanCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/VconfigCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/VconfigCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/VstartCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/VstartCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/command/WipeCommand.py` & `kathara-3.7.5/src/Kathara/cli/command/WipeCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/ui/event/HandleDockerImagePull.py` & `kathara-3.7.5/src/Kathara/cli/ui/event/HandleDockerImagePull.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/ui/event/HandleMachineTerminal.py` & `kathara-3.7.5/src/Kathara/cli/ui/event/HandleMachineTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/ui/event/HandleProgressBar.py` & `kathara-3.7.5/src/Kathara/cli/ui/event/HandleProgressBar.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/ui/event/UpdateDockerImage.py` & `kathara-3.7.5/src/Kathara/cli/ui/event/UpdateDockerImage.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/ui/event/register.py` & `kathara-3.7.5/src/Kathara/cli/ui/event/register.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/ui/setting/CommonOptionsHandler.py` & `kathara-3.7.5/src/Kathara/cli/ui/setting/CommonOptionsHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/ui/setting/DockerOptionsHandler.py` & `kathara-3.7.5/src/Kathara/cli/ui/setting/DockerOptionsHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py` & `kathara-3.7.5/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/ui/setting/SettingsMenuFactory.py` & `kathara-3.7.5/src/Kathara/cli/ui/setting/SettingsMenuFactory.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/ui/setting/utils.py` & `kathara-3.7.5/src/Kathara/cli/ui/setting/utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/cli/ui/utils.py` & `kathara-3.7.5/src/Kathara/cli/ui/utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/decorators.py` & `kathara-3.7.5/src/Kathara/decorators.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/event/EventDispatcher.py` & `kathara-3.7.5/src/Kathara/event/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/exceptions.py` & `kathara-3.7.5/src/Kathara/exceptions.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/foundation/cli/CliArgs.py` & `kathara-3.7.5/src/Kathara/foundation/cli/CliArgs.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/foundation/cli/command/Command.py` & `kathara-3.7.5/src/Kathara/foundation/cli/command/Command.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py` & `kathara-3.7.5/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/foundation/factory/Factory.py` & `kathara-3.7.5/src/Kathara/foundation/factory/Factory.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/foundation/manager/IManager.py` & `kathara-3.7.5/src/Kathara/foundation/manager/IManager.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/foundation/manager/stats/ILinkStats.py` & `kathara-3.7.5/src/Kathara/foundation/manager/stats/ILinkStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/foundation/manager/stats/IMachineStats.py` & `kathara-3.7.5/src/Kathara/foundation/manager/stats/IMachineStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/foundation/manager/terminal/Terminal.py` & `kathara-3.7.5/src/Kathara/foundation/manager/terminal/Terminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/foundation/manager/terminal/terminal_utils.py` & `kathara-3.7.5/src/Kathara/foundation/manager/terminal/terminal_utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/foundation/model/FilesystemMixin.py` & `kathara-3.7.5/src/Kathara/foundation/model/FilesystemMixin.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/foundation/setting/SettingsAddon.py` & `kathara-3.7.5/src/Kathara/foundation/setting/SettingsAddon.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/foundation/test/Test.py` & `kathara-3.7.5/src/Kathara/foundation/test/Test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/Kathara.py` & `kathara-3.7.5/src/Kathara/manager/Kathara.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/docker/DockerImage.py` & `kathara-3.7.5/src/Kathara/manager/docker/DockerImage.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/docker/DockerLink.py` & `kathara-3.7.5/src/Kathara/manager/docker/DockerLink.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/docker/DockerMachine.py` & `kathara-3.7.5/src/Kathara/manager/docker/DockerMachine.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from multiprocessing.dummy import Pool
 from typing import List, Dict, Generator, Optional, Set, Tuple, Union, Any
 
 import chardet
 import docker.models.containers
 from docker import DockerClient
 from docker.errors import APIError
+from docker.utils import version_lt
 
 from .DockerImage import DockerImage
 from .stats.DockerMachineStats import DockerMachineStats
 from ... import utils
 from ...event.EventDispatcher import EventDispatcher
 from ...exceptions import MountDeniedError, MachineAlreadyExistsError, DockerPluginError, \
     MachineBinaryError, MachineNotRunningError, PrivilegeError
@@ -97,19 +98,19 @@
     # Give execute permissions to the file and execute it
     "chmod u+x /hostlab/shared.shutdown; /hostlab/shared.shutdown; fi"
 ]
 
 
 class DockerMachine(object):
     """The class responsible for deploying Kathara devices as Docker container and interact with them."""
-    __slots__ = ['client', 'docker_image']
+    __slots__ = ['client', '_engine_version', 'docker_image']
 
     def __init__(self, client: DockerClient, docker_image: DockerImage) -> None:
         self.client: DockerClient = client
-
+        self._engine_version: str = client.version()['Version']
         self.docker_image: DockerImage = docker_image
 
     def deploy_machines(self, lab: Lab, selected_machines: Set[str] = None) -> None:
         """Deploy all the network scenario devices as Docker containers.
 
         Args:
             lab (Kathara.model.Lab.Lab): A Kathara network scenario.
@@ -238,23 +239,16 @@
         # Sysctl params to pass to the container creation
         sysctl_parameters = {RP_FILTER_NAMESPACE % x: 0 for x in ["all", "default", "lo"]}
         sysctl_parameters["net.ipv4.ip_forward"] = 1
         sysctl_parameters["net.ipv4.icmp_ratelimit"] = 0
 
         sysctl_first_interface = {}
         if first_machine_iface:
-            def sysctl_linux():
-                if utils.is_wsl_platform():
-                    return {RP_FILTER_NAMESPACE % "eth0": 0}
-                return {}
-
-            def sysctl_windows():
-                return {RP_FILTER_NAMESPACE % "eth0": 0}
-
-            sysctl_first_interface = utils.exec_by_platform(sysctl_linux, sysctl_windows, lambda: {})
+            if version_lt(self._engine_version, "26.0.0"):
+                sysctl_first_interface = {RP_FILTER_NAMESPACE % "eth0": 0}
 
         if machine.is_ipv6_enabled():
             sysctl_parameters["net.ipv6.conf.all.forwarding"] = 1
             sysctl_parameters["net.ipv6.conf.all.accept_ra"] = 0
             sysctl_parameters["net.ipv6.icmp.ratelimit"] = 0
             sysctl_parameters["net.ipv6.conf.default.disable_ipv6"] = 0
             sysctl_parameters["net.ipv6.conf.all.disable_ipv6"] = 0
@@ -341,15 +335,14 @@
         Returns:
             None
 
         Raises:
             DockerPluginError: If Kathara has been left in an inconsistent state.
             APIError: If the Docker APIs return an error.
         """
-        machine.api_object.reload()
         attached_networks = machine.api_object.attrs["NetworkSettings"]["Networks"]
 
         if interface.link.api_object.name not in attached_networks:
             try:
                 driver_opt = {'kathara.mac_addr': interface.mac_address} if interface.mac_address else None
 
                 interface.link.api_object.connect(
@@ -371,15 +364,14 @@
         Args:
             machine (Kathara.model.Machine): A Kathara device.
             link (Kathara.model.Link): A Kathara collision domain object.
 
         Returns:
             None
         """
-        machine.api_object.reload()
         attached_networks = machine.api_object.attrs["NetworkSettings"]["Networks"]
 
         if link.api_object.name in attached_networks:
             link.api_object.disconnect(machine.api_object)
 
     def start(self, machine: Machine) -> None:
         """Start the Docker container representing the device.
@@ -468,14 +460,16 @@
 
             logging.warning(f"Shell `{e.binary}` not found in "
                             f"image `{machine.get_image()}` of device `{machine.name}`. "
                             f"Startup commands will not be executed and terminal will not open. "
                             f"Please specify a valid shell for this device."
                             )
 
+        machine.api_object.reload()
+
     def undeploy(self, lab_hash: str, selected_machines: Set[str] = None) -> None:
         """Undeploy the devices contained in the network scenario defined by the lab_hash.
 
         If a set of selected_machines is specified, undeploy only the specified devices.
 
         Args:
             lab_hash (str): The hash of the network scenario to undeploy.
```

### Comparing `kathara-3.7.4/src/Kathara/manager/docker/DockerManager.py` & `kathara-3.7.5/src/Kathara/manager/docker/DockerManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         self.docker_link.deploy_links(lab, selected_links=selected_links)
 
         # Deploy all lab machines.
         self.docker_machine.deploy_machines(lab, selected_machines=selected_machines)
 
     @privileged
     def connect_machine_to_link(self, machine: Machine, link: Link, mac_address: Optional[str] = None) -> None:
-        """Create a new interface and connect a Kathara device to a collision domain.
+        """Create a new interface on a running Kathara device and connect it to a collision domain.
 
         Args:
             machine (Kathara.model.Machine): A Kathara machine object.
             link (Kathara.model.Link): A Kathara collision domain object.
             mac_address (Optional[str]): The MAC address to assign to the interface.
 
         Returns:
@@ -170,15 +170,19 @@
             MachineNotRunningError: If the specified device is not running.
             LabNotFoundError: If the collision domain is not associated to any network scenario.
             MachineCollisionDomainConflictError: If the device is already connected to the collision domain.
         """
         if not machine.lab:
             raise LabNotFoundError("Device `%s` is not associated to a network scenario." % machine.name)
 
-        if not machine.api_object or machine.api_object.status != "running":
+        if not machine.api_object:
+            raise MachineNotRunningError(machine.name)
+
+        machine.api_object.reload()
+        if machine.api_object.status != "running":
             raise MachineNotRunningError(machine.name)
 
         if not link.lab:
             raise LabNotFoundError(f"Collision domain `{link.name}` is not associated to a network scenario.")
 
         if machine.name in link.machines:
             raise MachineCollisionDomainError(
@@ -188,31 +192,39 @@
         interface = machine.add_interface(link, mac_address=mac_address)
 
         self.deploy_link(link)
         self.docker_machine.connect_interface(machine, interface)
 
     @privileged
     def disconnect_machine_from_link(self, machine: Machine, link: Link) -> None:
-        """Disconnect a Kathara device from a collision domain.
+        """Disconnect a running Kathara device from a collision domain.
 
         Args:
             machine (Kathara.model.Machine): A Kathara machine object.
-            link (Kathara.model.Link): The Kathara collision domain from which disconnect the device.
+            link (Kathara.model.Link): The Kathara collision domain from which disconnect the running device.
 
         Returns:
             None
 
         Raises:
             LabNotFoundError: If the device specified is not associated to any network scenario.
+            MachineNotRunningError: If the specified device is not running.
             LabNotFoundError: If the collision domain is not associated to any network scenario.
             MachineCollisionDomainConflictError: If the device is not connected to the collision domain.
         """
         if not machine.lab:
             raise LabNotFoundError(f"Device `{machine.name}` is not associated to a network scenario.")
 
+        if not machine.api_object:
+            raise MachineNotRunningError(machine.name)
+
+        machine.api_object.reload()
+        if machine.api_object.status != "running":
+            raise MachineNotRunningError(machine.name)
+
         if not link.lab:
             raise LabNotFoundError(f"Collision domain `{link.name}` is not associated to a network scenario.")
 
         if machine.name not in link.machines:
             raise MachineCollisionDomainError(
                 f"Device `{machine.name}` is not connected to collision domain `{link.name}`."
             )
```

### Comparing `kathara-3.7.4/src/Kathara/manager/docker/DockerPlugin.py` & `kathara-3.7.5/src/Kathara/manager/docker/DockerPlugin.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/docker/stats/DockerLinkStats.py` & `kathara-3.7.5/src/Kathara/manager/docker/stats/DockerLinkStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/docker/stats/DockerMachineStats.py` & `kathara-3.7.5/src/Kathara/manager/docker/stats/DockerMachineStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py` & `kathara-3.7.5/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py` & `kathara-3.7.5/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/kubernetes/KubernetesConfig.py` & `kathara-3.7.5/src/Kathara/manager/kubernetes/KubernetesConfig.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/kubernetes/KubernetesConfigMap.py` & `kathara-3.7.5/src/Kathara/manager/kubernetes/KubernetesConfigMap.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/kubernetes/KubernetesLink.py` & `kathara-3.7.5/src/Kathara/manager/kubernetes/KubernetesLink.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/kubernetes/KubernetesMachine.py` & `kathara-3.7.5/src/Kathara/manager/kubernetes/KubernetesMachine.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/kubernetes/KubernetesManager.py` & `kathara-3.7.5/src/Kathara/manager/kubernetes/KubernetesManager.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/kubernetes/KubernetesNamespace.py` & `kathara-3.7.5/src/Kathara/manager/kubernetes/KubernetesNamespace.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py` & `kathara-3.7.5/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py` & `kathara-3.7.5/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py` & `kathara-3.7.5/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/model/ExternalLink.py` & `kathara-3.7.5/src/Kathara/model/ExternalLink.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/model/Interface.py` & `kathara-3.7.5/src/Kathara/model/Interface.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/model/Lab.py` & `kathara-3.7.5/src/Kathara/model/Lab.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/model/Link.py` & `kathara-3.7.5/src/Kathara/model/Link.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/model/Machine.py` & `kathara-3.7.5/src/Kathara/model/Machine.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/os/Networking.py` & `kathara-3.7.5/src/Kathara/os/Networking.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/parser/netkit/DepParser.py` & `kathara-3.7.5/src/Kathara/parser/netkit/DepParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/parser/netkit/ExtParser.py` & `kathara-3.7.5/src/Kathara/parser/netkit/ExtParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/parser/netkit/FolderParser.py` & `kathara-3.7.5/src/Kathara/parser/netkit/FolderParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/parser/netkit/LabParser.py` & `kathara-3.7.5/src/Kathara/parser/netkit/LabParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/parser/netkit/OptionParser.py` & `kathara-3.7.5/src/Kathara/parser/netkit/OptionParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/setting/Setting.py` & `kathara-3.7.5/src/Kathara/setting/Setting.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/setting/addon/DockerSettingsAddon.py` & `kathara-3.7.5/src/Kathara/setting/addon/DockerSettingsAddon.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/setting/addon/KubernetesSettingsAddon.py` & `kathara-3.7.5/src/Kathara/setting/addon/KubernetesSettingsAddon.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/strings.py` & `kathara-3.7.5/src/Kathara/strings.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/test/BuiltinTest.py` & `kathara-3.7.5/src/Kathara/test/BuiltinTest.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/test/UserTest.py` & `kathara-3.7.5/src/Kathara/test/UserTest.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/__init__.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/__init__.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/console_menu.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/console_menu.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/format/__init__.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/format/__init__.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/format/menu_borders.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/format/menu_borders.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/format/menu_margins.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/format/menu_margins.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/format/menu_padding.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/format/menu_padding.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/format/menu_style.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/format/menu_style.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/items/command_item.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/items/command_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/items/external_item.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/items/external_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/items/function_item.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/items/function_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/items/selection_item.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/items/selection_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/items/submenu_item.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/items/submenu_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/menu_component.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/menu_component.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/menu_formatter.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/menu_formatter.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/multiselect_menu.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/multiselect_menu.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/prompt_utils.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/screen.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/screen.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/selection_menu.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/selection_menu.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/validators/base.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/validators/base.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/validators/regex.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/validators/regex.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/consolemenu/validators/url.py` & `kathara-3.7.5/src/Kathara/trdparty/consolemenu/validators/url.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/depgen/depgen.py` & `kathara-3.7.5/src/Kathara/trdparty/depgen/depgen.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/libtmux/tmux.py` & `kathara-3.7.5/src/Kathara/trdparty/libtmux/tmux.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/nsenter/nsenter.py` & `kathara-3.7.5/src/Kathara/trdparty/nsenter/nsenter.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/trdparty/strtobool/strtobool.py` & `kathara-3.7.5/src/Kathara/trdparty/strtobool/strtobool.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/types.py` & `kathara-3.7.5/src/Kathara/types.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/utils.py` & `kathara-3.7.5/src/Kathara/utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/validator/ImageValidator.py` & `kathara-3.7.5/src/Kathara/validator/ImageValidator.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/webhooks/DockerHubApi.py` & `kathara-3.7.5/src/Kathara/webhooks/DockerHubApi.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/Kathara/webhooks/GitHubApi.py` & `kathara-3.7.5/src/Kathara/webhooks/GitHubApi.py`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/kathara.egg-info/PKG-INFO` & `kathara-3.7.5/src/kathara.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kathara
-Version: 3.7.4
+Version: 3.7.5
 Summary: A lightweight container-based network emulation tool.
 Home-page: https://www.kathara.org
-Download-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.7.4.tar.gz
+Download-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.7.5.tar.gz
 Author: Kathara Framework
 Author-email: Kathara Framework <contact@kathara.org>
 Maintainer-email: Tommaso Caiazzi <contact@kathara.org>, Mariano Scazzariello <contact@kathara.org>, Lorenzo Ariemma <contact@kathara.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -806,16 +806,14 @@
 
 - [Netkit Lab Generator](https://github.com/KatharaFramework/Netkit-Lab-Generator), a GUI that allows the easy creation of a network scenario configuration and the visualization of its network topology.
 - [VFTGen](https://github.com/KatharaFramework/VFTGen), a tool that allows to create three levels Fat Tree topologies (single-plane or multi-planes) and automatically configure them to run on Kathará.
 - [Tacatá](https://github.com/damiano-massarelli/Tacata), a lightweight Python script which creates Netkit and Kathará labs using an enriched version of the lab.conf file with a simple syntax.
 - [net-vis](https://github.com/Friscobuffo/net-vis-localhost), a tool that parses (and generates) the `lab.conf` file and all the `.startup` files to visualize the network.
 - [kathara-lab-starter](https://github.com/BuonHobo/kathara-lab-starter), an easy and extensible tool to get a kathara lab started.  Utilizing JSON input files, it accelerates setup, while minimizing configuration redundancies.
 
-Being based on Netkit, all the previous tools still work. 
-
 ## Success Stories
 As far as we know, Kathará is currently being used in many [courses and projects](https://www.kathara.org/stories.html). 
  
 We encourage you to tell us your story! 
 
 We are also collecting network scenarios from the community. If you want to be added to the [list](https://github.com/KatharaFramework/Kathara-Labs/tree/main/community-labs), please contact us!
```

### Comparing `kathara-3.7.4/src/kathara.egg-info/SOURCES.txt` & `kathara-3.7.5/src/kathara.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kathara-3.7.4/src/kathara.py` & `kathara-3.7.5/src/kathara.py`

 * *Files identical despite different names*

