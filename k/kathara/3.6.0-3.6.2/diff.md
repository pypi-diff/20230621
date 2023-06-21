# Comparing `tmp/kathara-3.6.0.tar.gz` & `tmp/kathara-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kathara-3.6.0.tar", last modified: Mon May 22 09:27:57 2023, max compression
+gzip compressed data, was "kathara-3.6.2.tar", last modified: Wed Jun 21 14:21:36 2023, max compression
```

## Comparing `kathara-3.6.0.tar` & `kathara-3.6.2.tar`

### file list

```diff
@@ -1,215 +1,413 @@
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.237546 kathara-3.6.0/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    35141 2022-09-29 09:36:59.000000 kathara-3.6.0/LICENSE
--rw-rw-r--   0 tommaso   (1001) tommaso   (1001)    50225 2023-05-22 09:27:57.237546 kathara-3.6.0/PKG-INFO
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     8365 2023-01-31 11:35:52.000000 kathara-3.6.0/README.md
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1986 2023-05-22 08:35:38.000000 kathara-3.6.0/pyproject.toml
--rw-rw-r--   0 tommaso   (1001) tommaso   (1001)      723 2023-05-22 09:27:57.237546 kathara-3.6.0/setup.cfg
--rw-rw-r--   0 tommaso   (1001) tommaso   (1001)     1679 2023-05-22 08:35:38.000000 kathara-3.6.0/setup.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.213546 kathara-3.6.0/src/
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.213546 kathara-3.6.0/src/Kathara/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.213546 kathara-3.6.0/src/Kathara/auth/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1650 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/auth/PrivilegeHandler.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/auth/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.213546 kathara-3.6.0/src/Kathara/cli/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.217546 kathara-3.6.0/src/Kathara/cli/command/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2240 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/CheckCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2521 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/ConnectCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3068 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/cli/command/ExecCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1972 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/LcleanCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3010 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/LconfigCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     4632 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/LinfoCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2575 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/ListCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     4324 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/LrestartCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     8237 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/LstartCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     4512 2023-02-08 10:14:37.000000 kathara-3.6.0/src/Kathara/cli/command/LtestCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      350 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/command/SettingsCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1253 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/VcleanCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2698 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/VconfigCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     6964 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/VstartCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2217 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/command/WipeCommand.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/command/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.217546 kathara-3.6.0/src/Kathara/cli/ui/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.217546 kathara-3.6.0/src/Kathara/cli/ui/event/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1313 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/event/HandleProgressBar.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      694 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/event/OpenMachineTerminal.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1058 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/event/UpdateDockerImage.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/event/__init__.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2402 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/event/register.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/cli/ui/setting/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    21225 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/ui/setting/CommonOptionsHandler.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    13071 2023-02-08 10:14:16.000000 kathara-3.6.0/src/Kathara/cli/ui/setting/DockerOptionsHandler.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     8908 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1483 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/setting/SettingsMenuFactory.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/setting/__init__.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3828 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/cli/ui/setting/utils.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     5981 2023-02-08 10:14:37.000000 kathara-3.6.0/src/Kathara/cli/ui/utils.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      623 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/decorators.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/event/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2832 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/event/EventDispatcher.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/event/__init__.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3718 2022-12-22 11:19:53.000000 kathara-3.6.0/src/Kathara/exceptions.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/cli/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      741 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/foundation/cli/CliArgs.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/cli/command/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      595 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/command/Command.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      205 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/command/CommandFactory.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/command/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/cli/ui/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/ui/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/cli/ui/setting/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1023 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      233 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/ui/setting/OptionsHandlerFactory.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/cli/ui/setting/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/factory/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1010 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/factory/Factory.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/factory/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/manager/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    17939 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/foundation/manager/IManager.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      213 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/ManagerFactory.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.221546 kathara-3.6.0/src/Kathara/foundation/manager/stats/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      681 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/stats/ILinkStats.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      674 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/stats/IMachineStats.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/stats/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/foundation/manager/terminal/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2095 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/terminal/Terminal.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/terminal/__init__.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1178 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/manager/terminal/terminal_utils.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/foundation/model/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    11264 2023-05-17 10:04:03.000000 kathara-3.6.0/src/Kathara/foundation/model/FilesystemMixin.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2023-02-08 10:14:37.000000 kathara-3.6.0/src/Kathara/foundation/model/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/foundation/setting/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      749 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/setting/SettingsAddon.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      228 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/setting/SettingsAddonFactory.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/setting/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/foundation/test/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1662 2023-02-08 10:14:37.000000 kathara-3.6.0/src/Kathara/foundation/test/Test.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/foundation/test/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    18970 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/manager/Kathara.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/docker/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     7128 2023-03-29 09:31:09.000000 kathara-3.6.0/src/Kathara/manager/docker/DockerImage.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    13831 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/manager/docker/DockerLink.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    36212 2023-05-17 10:04:03.000000 kathara-3.6.0/src/Kathara/manager/docker/DockerMachine.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    31189 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/manager/docker/DockerManager.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3606 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/manager/docker/DockerPlugin.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/docker/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/docker/stats/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3383 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/docker/stats/DockerLinkStats.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     5220 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/docker/stats/DockerMachineStats.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/docker/stats/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/docker/terminal/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2205 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1157 2023-04-03 14:17:45.000000 kathara-3.6.0/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/docker/terminal/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/kubernetes/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1924 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesConfig.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     4252 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesConfigMap.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    14270 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesLink.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    34972 2023-05-17 10:04:03.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesMachine.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    30101 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesManager.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     4366 2022-12-22 11:19:53.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesNamespace.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/kubernetes/stats/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2144 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3444 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/stats/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/manager/kubernetes/terminal/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2418 2022-12-15 11:28:14.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/manager/kubernetes/terminal/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.225546 kathara-3.6.0/src/Kathara/model/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1975 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/model/ExternalLink.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    14008 2023-03-29 09:31:09.000000 kathara-3.6.0/src/Kathara/model/Lab.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1252 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/model/Link.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    24708 2023-05-17 10:04:03.000000 kathara-3.6.0/src/Kathara/model/Machine.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/model/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/os/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     5402 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/os/Networking.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/os/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/parser/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/parser/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/parser/netkit/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2657 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/parser/netkit/DepParser.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2665 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/parser/netkit/ExtParser.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1146 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/parser/netkit/FolderParser.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3433 2023-05-09 11:16:07.000000 kathara-3.6.0/src/Kathara/parser/netkit/LabParser.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      903 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/parser/netkit/OptionParser.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/parser/netkit/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/setting/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    11573 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/setting/Setting.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/setting/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/setting/addon/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1116 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/setting/addon/DockerSettingsAddon.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      906 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/setting/addon/KubernetesSettingsAddon.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/setting/addon/__init__.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1404 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/strings.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/test/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     5449 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/test/BuiltinTest.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     4534 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/test/UserTest.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/test/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/trdparty/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.229546 kathara-3.6.0/src/Kathara/trdparty/consolemenu/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      519 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/__init__.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    15168 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/console_menu.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      850 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/__init__.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    14430 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_borders.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1502 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_margins.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1445 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_padding.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3760 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_style.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      385 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/__init__.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1335 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/command_item.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      803 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/external_item.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1353 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/function_item.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      595 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/selection_item.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1596 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/submenu_item.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    13445 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/menu_component.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    11425 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/menu_formatter.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     3281 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/multiselect_menu.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)    12321 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/prompt_utils.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1805 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/screen.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2772 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/selection_menu.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/__init__.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      765 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/base.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1009 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/regex.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      558 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/url.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)       22 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/consolemenu/version.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/curses/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/curses/__init__.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1352 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/curses/curses.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/depgen/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/depgen/__init__.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2992 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/depgen/depgen.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/libtmux/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/trdparty/libtmux/__init__.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     2738 2023-03-29 09:31:09.000000 kathara-3.6.0/src/Kathara/trdparty/libtmux/tmux.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.233546 kathara-3.6.0/src/Kathara/trdparty/strtobool/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2023-01-31 11:35:52.000000 kathara-3.6.0/src/Kathara/trdparty/strtobool/__init__.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      692 2023-01-31 11:35:52.000000 kathara-3.6.0/src/Kathara/trdparty/strtobool/strtobool.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     9659 2023-04-26 09:34:00.000000 kathara-3.6.0/src/Kathara/utils.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.237546 kathara-3.6.0/src/Kathara/validator/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      599 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/validator/ImageValidator.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      457 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/validator/TerminalValidator.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/validator/__init__.py
--rw-rw-r--   0 tommaso   (1001) tommaso   (1001)      308 2023-05-22 08:35:38.000000 kathara-3.6.0/src/Kathara/version.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.237546 kathara-3.6.0/src/Kathara/webhooks/
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)     1318 2022-10-27 08:44:22.000000 kathara-3.6.0/src/Kathara/webhooks/DockerHubApi.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)      795 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/webhooks/GitHubApi.py
--rw-r--r--   0 tommaso   (1001) tommaso   (1001)        0 2022-09-29 09:36:59.000000 kathara-3.6.0/src/Kathara/webhooks/__init__.py
-drwxrwxr-x   0 tommaso   (1001) tommaso   (1001)        0 2023-05-22 09:27:57.237546 kathara-3.6.0/src/kathara.egg-info/
--rw-rw-r--   0 tommaso   (1001) tommaso   (1001)    50225 2023-05-22 09:27:57.000000 kathara-3.6.0/src/kathara.egg-info/PKG-INFO
--rw-rw-r--   0 tommaso   (1001) tommaso   (1001)     6929 2023-05-22 09:27:57.000000 kathara-3.6.0/src/kathara.egg-info/SOURCES.txt
--rw-rw-r--   0 tommaso   (1001) tommaso   (1001)        1 2023-05-22 09:27:57.000000 kathara-3.6.0/src/kathara.egg-info/dependency_links.txt
--rw-rw-r--   0 tommaso   (1001) tommaso   (1001)      463 2023-05-22 09:27:57.000000 kathara-3.6.0/src/kathara.egg-info/requires.txt
--rw-rw-r--   0 tommaso   (1001) tommaso   (1001)       16 2023-05-22 09:27:57.000000 kathara-3.6.0/src/kathara.egg-info/top_level.txt
--rwxrwxrwx   0 tommaso   (1001) tommaso   (1001)     4027 2022-10-27 08:44:22.000000 kathara-3.6.0/src/kathara.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/.github/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      527 2022-07-26 14:39:39.000000 kathara-3.6.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      560 2022-07-26 14:39:39.000000 kathara-3.6.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      510 2022-07-26 14:39:39.000000 kathara-3.6.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1435 2023-05-19 15:22:33.000000 kathara-3.6.2/.gitignore
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3351 2022-07-26 14:39:39.000000 kathara-3.6.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1514 2022-07-26 14:39:39.000000 kathara-3.6.2/CONTRIBUTING.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    35141 2022-07-26 14:39:39.000000 kathara-3.6.2/LICENSE
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)    50225 2023-06-21 14:21:36.783736 kathara-3.6.2/PKG-INFO
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8365 2023-01-17 11:29:05.000000 kathara-3.6.2/README.md
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/docs/
+-rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     1413 2022-07-26 14:39:39.000000 kathara-3.6.2/docs/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1161 2022-09-09 09:29:44.000000 kathara-3.6.2/docs/footer.txt
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1307 2022-07-26 14:39:39.000000 kathara-3.6.2/docs/index.txt
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      985 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-check.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1638 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-connect.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1622 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-exec.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3267 2022-09-02 15:11:08.000000 kathara-3.6.2/docs/kathara-lab-dirs.7.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4449 2022-09-02 15:11:08.000000 kathara-3.6.2/docs/kathara-lab.conf.5.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      658 2022-09-02 15:11:08.000000 kathara-3.6.2/docs/kathara-lab.dep.5.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1820 2022-09-02 15:11:08.000000 kathara-3.6.2/docs/kathara-lab.ext.5.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1108 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-lclean.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2214 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-lconfig.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1985 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-linfo.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1417 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-list.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4210 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-lrestart.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5303 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-lstart.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5417 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-ltest.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      524 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-settings.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      567 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-vclean.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1638 2022-09-02 15:11:08.000000 kathara-3.6.2/docs/kathara-vconfig.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7226 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-vstart.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1163 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-wipe.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3313 2022-09-09 09:29:44.000000 kathara-3.6.2/docs/kathara.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     6196 2022-09-02 15:11:08.000000 kathara-3.6.2/docs/kathara.conf.5.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1986 2023-06-18 15:50:16.000000 kathara-3.6.2/pyproject.toml
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.747736 kathara-3.6.2/scripts/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Deb/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Deb/Docker-Linux-Build/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      841 2023-05-17 13:20:12.000000 kathara-3.6.2/scripts/Linux-Deb/Docker-Linux-Build/Dockerfile_template
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      168 2023-05-18 10:29:39.000000 kathara-3.6.2/scripts/Linux-Deb/Docker-Linux-Build/dput.cf
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)     6087 2023-06-21 13:32:12.000000 kathara-3.6.2/scripts/Linux-Deb/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1340 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/README.md
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Deb/debian/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      354 2023-06-21 13:41:59.000000 kathara-3.6.2/scripts/Linux-Deb/debian/changelog
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        3 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/compat
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      871 2023-04-27 14:28:28.000000 kathara-3.6.2/scripts/Linux-Deb/debian/control
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1042 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/copyright
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       24 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/kathara.dirs
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       40 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/kathara.links
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      344 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/kathara.lintian-overrides
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      157 2023-05-18 09:09:00.000000 kathara-3.6.2/scripts/Linux-Deb/debian/kathara.postinst
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       88 2023-05-18 09:08:56.000000 kathara-3.6.2/scripts/Linux-Deb/debian/kathara.prerm
+-rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     1379 2023-05-24 09:06:02.000000 kathara-3.6.2/scripts/Linux-Deb/debian/rules
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Deb/debian/source/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       12 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/source/format
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       33 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/source/lintian-overrides
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Pkg/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Pkg/Docker-Linux-Build/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      691 2023-05-24 09:06:38.000000 kathara-3.6.2/scripts/Linux-Pkg/Docker-Linux-Build/Dockerfile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2694 2023-06-18 17:19:35.000000 kathara-3.6.2/scripts/Linux-Pkg/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1283 2023-06-18 17:20:44.000000 kathara-3.6.2/scripts/Linux-Pkg/README.md
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Pkg/pkginfo/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3067 2023-06-18 17:18:39.000000 kathara-3.6.2/scripts/Linux-Pkg/pkginfo/PKGBUILD
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      262 2023-06-18 15:50:16.000000 kathara-3.6.2/scripts/Linux-Pkg/pkginfo/kathara.changelog
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      235 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Pkg/pkginfo/kathara.install
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Rpm/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Rpm/Docker-Linux-Build/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      383 2023-01-04 12:29:14.000000 kathara-3.6.2/scripts/Linux-Rpm/Docker-Linux-Build/Dockerfile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2008 2023-06-18 15:50:16.000000 kathara-3.6.2/scripts/Linux-Rpm/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      538 2023-05-24 09:06:02.000000 kathara-3.6.2/scripts/Linux-Rpm/README.md
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Rpm/rpm/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3041 2023-06-18 15:50:16.000000 kathara-3.6.2/scripts/Linux-Rpm/rpm/kathara.spec
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/OSX/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4476 2023-06-18 15:50:16.000000 kathara-3.6.2/scripts/OSX/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2429 2022-09-09 09:29:44.000000 kathara-3.6.2/scripts/OSX/README.md
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/OSX/darwin/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1501 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/darwin/Distribution
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/OSX/darwin/Resources/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    59811 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/darwin/Resources/banner.png
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1926 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/darwin/Resources/conclusion.html
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1240 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/darwin/Resources/welcome.html
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/OSX/darwin/scripts/
+-rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)      393 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/darwin/scripts/postinstall
+-rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     1527 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/darwin/uninstall.sh
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2836 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/kathara.spec
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/Windows/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/Windows/Assets/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    32988 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Windows/Assets/app_icon.ico
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1580 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Windows/Assets/environment.iss
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2844 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Windows/Assets/kathara.spec
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      707 2022-09-09 09:29:44.000000 kathara-3.6.2/scripts/Windows/README.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      761 2023-05-24 09:06:02.000000 kathara-3.6.2/scripts/Windows/WindowsBuild.bat
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2288 2023-06-18 15:50:16.000000 kathara-3.6.2/scripts/Windows/installer.iss
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/autocompletion/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3034 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/autocompletion/generate_autocompletion.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      120 2023-05-24 09:06:02.000000 kathara-3.6.2/scripts/autocompletion/requirements.txt
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/pip-package/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      291 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/pip-package/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      387 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/pip-package/README.md
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/pydoc/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1142 2022-12-28 11:38:10.000000 kathara-3.6.2/scripts/pydoc/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      194 2022-09-26 11:15:29.000000 kathara-3.6.2/scripts/pydoc/README.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      706 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/pydoc/generate_doc.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      723 2023-06-21 14:21:36.783736 kathara-3.6.2/setup.cfg
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1679 2023-06-18 15:50:16.000000 kathara-3.6.2/setup.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/src/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/src/Kathara/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/src/Kathara/auth/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1650 2022-09-02 15:11:08.000000 kathara-3.6.2/src/Kathara/auth/PrivilegeHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/auth/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/src/Kathara/cli/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/cli/command/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2240 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/CheckCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2521 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/ConnectCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3068 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/ExecCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1972 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/LcleanCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3010 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/LconfigCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4632 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/LinfoCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2575 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/ListCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4324 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/LrestartCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8237 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/LstartCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4512 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/LtestCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      350 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/command/SettingsCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1253 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/VcleanCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2698 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/VconfigCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     6964 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/VstartCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2217 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/WipeCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/command/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/cli/ui/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/cli/ui/event/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1313 2022-11-02 11:57:09.000000 kathara-3.6.2/src/Kathara/cli/ui/event/HandleProgressBar.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      694 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/event/OpenMachineTerminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1058 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/event/UpdateDockerImage.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/event/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2402 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/event/register.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/cli/ui/setting/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    21159 2023-06-16 09:17:57.000000 kathara-3.6.2/src/Kathara/cli/ui/setting/CommonOptionsHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13071 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/ui/setting/DockerOptionsHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8908 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1483 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/setting/SettingsMenuFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/setting/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3828 2022-08-26 10:08:06.000000 kathara-3.6.2/src/Kathara/cli/ui/setting/utils.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5981 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/ui/utils.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      623 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/decorators.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/event/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2832 2022-09-02 16:43:02.000000 kathara-3.6.2/src/Kathara/event/EventDispatcher.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/event/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3718 2023-05-16 16:24:29.000000 kathara-3.6.2/src/Kathara/exceptions.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/cli/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      741 2022-09-02 15:11:08.000000 kathara-3.6.2/src/Kathara/foundation/cli/CliArgs.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/cli/command/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      595 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/command/Command.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      205 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/command/CommandFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/command/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/cli/ui/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/ui/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/cli/ui/setting/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1023 2022-09-02 15:11:08.000000 kathara-3.6.2/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      233 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/ui/setting/OptionsHandlerFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/ui/setting/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/factory/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1010 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/factory/Factory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/factory/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/manager/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    17939 2023-05-09 13:30:55.000000 kathara-3.6.2/src/Kathara/foundation/manager/IManager.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      213 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/ManagerFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/manager/stats/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      681 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/stats/ILinkStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      674 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/stats/IMachineStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/stats/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/manager/terminal/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2095 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/terminal/Terminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/terminal/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1178 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/terminal/terminal_utils.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/foundation/model/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11374 2023-06-16 09:17:54.000000 kathara-3.6.2/src/Kathara/foundation/model/FilesystemMixin.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/foundation/model/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/foundation/setting/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      749 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/setting/SettingsAddon.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      228 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/setting/SettingsAddonFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/setting/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/foundation/test/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1662 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/foundation/test/Test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/test/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    18970 2023-05-09 13:30:55.000000 kathara-3.6.2/src/Kathara/manager/Kathara.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/docker/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7128 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/manager/docker/DockerImage.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13831 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/manager/docker/DockerLink.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    36272 2023-06-16 09:17:57.000000 kathara-3.6.2/src/Kathara/manager/docker/DockerMachine.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    31189 2023-05-09 13:30:55.000000 kathara-3.6.2/src/Kathara/manager/docker/DockerManager.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3606 2022-09-02 16:24:37.000000 kathara-3.6.2/src/Kathara/manager/docker/DockerPlugin.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/docker/stats/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3383 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/stats/DockerLinkStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5220 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/stats/DockerMachineStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/stats/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/docker/terminal/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2205 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1157 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/terminal/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/kubernetes/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1924 2022-09-02 17:03:11.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesConfig.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4252 2022-09-09 09:29:44.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesConfigMap.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    14270 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesLink.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    34969 2023-06-16 09:17:54.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesMachine.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    30101 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesManager.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4366 2022-12-22 14:55:44.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesNamespace.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/kubernetes/stats/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2144 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3444 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/stats/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/kubernetes/terminal/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2418 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/terminal/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/model/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1975 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/model/ExternalLink.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    14058 2023-06-16 09:17:54.000000 kathara-3.6.2/src/Kathara/model/Lab.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1252 2022-08-26 10:08:06.000000 kathara-3.6.2/src/Kathara/model/Link.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    25351 2023-06-16 09:17:57.000000 kathara-3.6.2/src/Kathara/model/Machine.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-05-29 14:35:19.000000 kathara-3.6.2/src/Kathara/model/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/os/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5402 2022-09-02 17:03:11.000000 kathara-3.6.2/src/Kathara/os/Networking.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/os/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/parser/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/parser/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/parser/netkit/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2657 2022-09-09 09:29:44.000000 kathara-3.6.2/src/Kathara/parser/netkit/DepParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2665 2022-09-09 09:29:44.000000 kathara-3.6.2/src/Kathara/parser/netkit/ExtParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1146 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/parser/netkit/FolderParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3436 2023-06-16 09:17:54.000000 kathara-3.6.2/src/Kathara/parser/netkit/LabParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      903 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/parser/netkit/OptionParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/parser/netkit/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/setting/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11573 2023-06-18 15:50:16.000000 kathara-3.6.2/src/Kathara/setting/Setting.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/setting/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/setting/addon/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1116 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/setting/addon/DockerSettingsAddon.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      906 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/setting/addon/KubernetesSettingsAddon.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/setting/addon/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1404 2022-09-02 15:11:08.000000 kathara-3.6.2/src/Kathara/strings.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/test/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5449 2022-09-09 09:29:44.000000 kathara-3.6.2/src/Kathara/test/BuiltinTest.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4534 2022-09-09 09:29:44.000000 kathara-3.6.2/src/Kathara/test/UserTest.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/test/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/trdparty/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/trdparty/consolemenu/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      519 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    15168 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/console_menu.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      850 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    14430 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_borders.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1502 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_margins.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1445 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_padding.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3760 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_style.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      385 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1335 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/command_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      803 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/external_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1353 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/function_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      595 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/selection_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1596 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/submenu_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13445 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/menu_component.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11425 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/menu_formatter.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3281 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/multiselect_menu.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    12321 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/prompt_utils.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1805 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/screen.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2772 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/selection_menu.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      765 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/base.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1009 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/regex.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      558 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/url.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       22 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/version.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/Kathara/trdparty/curses/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/curses/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1352 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/curses/curses.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/Kathara/trdparty/depgen/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/depgen/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2992 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/depgen/depgen.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/Kathara/trdparty/libtmux/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/libtmux/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2738 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/trdparty/libtmux/tmux.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/Kathara/trdparty/strtobool/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/trdparty/strtobool/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      692 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/trdparty/strtobool/strtobool.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     9659 2023-05-29 14:28:12.000000 kathara-3.6.2/src/Kathara/utils.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/Kathara/validator/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      599 2022-09-02 15:11:08.000000 kathara-3.6.2/src/Kathara/validator/ImageValidator.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      457 2022-09-02 15:11:08.000000 kathara-3.6.2/src/Kathara/validator/TerminalValidator.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/validator/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      308 2023-06-18 15:50:16.000000 kathara-3.6.2/src/Kathara/version.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/Kathara/webhooks/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3461 2023-06-18 15:50:16.000000 kathara-3.6.2/src/Kathara/webhooks/DockerHubApi.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      795 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/webhooks/GitHubApi.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/webhooks/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/kathara.egg-info/
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)    50225 2023-06-21 14:21:36.000000 kathara-3.6.2/src/kathara.egg-info/PKG-INFO
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)    11859 2023-06-21 14:21:36.000000 kathara-3.6.2/src/kathara.egg-info/SOURCES.txt
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)        1 2023-06-21 14:21:36.000000 kathara-3.6.2/src/kathara.egg-info/dependency_links.txt
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)      463 2023-06-21 14:21:36.000000 kathara-3.6.2/src/kathara.egg-info/requires.txt
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)       16 2023-06-21 14:21:36.000000 kathara-3.6.2/src/kathara.egg-info/top_level.txt
+-rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     4027 2022-09-09 09:29:44.000000 kathara-3.6.2/src/kathara.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      444 2023-05-24 09:06:02.000000 kathara-3.6.2/src/requirements.txt
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.747736 kathara-3.6.2/tests/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/tests/cli/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4997 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/connect_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7588 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/exec_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3025 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/lclean_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7356 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/lconfig_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7011 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/linfo_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8275 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/list_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1855 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/lrestart_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    27515 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/lstart_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      632 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/vclean_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1285 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/vconfig_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    32948 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/vstart_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4157 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/wipe_command_test.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/tests/manager/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/manager/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/tests/manager/docker/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/manager/docker/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11289 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/manager/docker/docker_image_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13862 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/manager/docker/docker_link_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    36139 2022-12-22 14:55:44.000000 kathara-3.6.2/tests/manager/docker/docker_machine_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    46614 2023-06-16 09:17:54.000000 kathara-3.6.2/tests/manager/docker/docker_manager_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     6072 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/manager/docker/docker_plugin_test.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/manager/kubernetes/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/manager/kubernetes/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    19509 2022-12-22 14:55:44.000000 kathara-3.6.2/tests/manager/kubernetes/kubernetes_link_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    30115 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/manager/kubernetes/kubernetes_machine_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    35405 2023-06-16 09:17:54.000000 kathara-3.6.2/tests/manager/kubernetes/kubernetes_manager_test.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/model/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1422 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/model/external_link_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    16555 2023-06-16 09:17:54.000000 kathara-3.6.2/tests/model/filesystem_mixin_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    12130 2023-06-16 09:17:54.000000 kathara-3.6.2/tests/model/lab_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    10461 2023-06-16 09:17:54.000000 kathara-3.6.2/tests/model/machine_test.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      779 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/dep_parser_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      881 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/ext_parser_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      669 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/folder_parser_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2987 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/parser/lab_parser_test.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labconf/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/inline_comment/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       43 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/parser/labconf/inline_comment/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/inline_comment_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       42 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/parser/labconf/inline_comment_error/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/one_device/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      177 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labconf/one_device/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/one_device_interface_name_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       76 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labconf/one_device_interface_name_error/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/one_device_lab_description/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      303 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labconf/one_device_lab_description/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/one_device_same_collision_domain_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       21 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labconf/one_device_same_collision_domain_error/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/one_device_shared_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       14 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labconf/one_device_shared_error/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/two_devices_one_cd/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      131 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labconf/two_devices_one_cd/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/unclosed_quotes/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        9 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/parser/labconf/unclosed_quotes/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/unmatched_quotes/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       10 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/parser/labconf/unmatched_quotes/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labdep/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labdep/comments_empty_lines/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       66 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labdep/comments_empty_lines/lab.dep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labdep/devices_loop/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       26 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labdep/devices_loop/lab.dep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labdep/syntax_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       24 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labdep/syntax_error/lab.dep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labdep/three_devices_dependencies/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       21 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labdep/three_devices_dependencies/lab.dep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labext/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labext/syntax_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       65 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/labext/syntax_error/lab.conf
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       23 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/labext/syntax_error/lab.ext
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labext/two_devices/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       65 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labext/two_devices/lab.conf
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       36 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labext/two_devices/lab.ext
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labext/value_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       65 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/labext/value_error/lab.conf
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       17 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/labext/value_error/lab.ext
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labfolder/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/pc1/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/pc1/.gitkeep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/pc2/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/pc2/.gitkeep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/shared/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/shared/.gitkeep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labfolder/one_device/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labfolder/one_device/pc1/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labfolder/one_device/pc1/.gitkeep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labfolder/two_devices/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labfolder/two_devices/pc1/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labfolder/two_devices/pc1/.gitkeep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labfolder/two_devices/pc2/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labfolder/two_devices/pc2/.gitkeep
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      681 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/option_parser_test.py
```

### Comparing `kathara-3.6.0/LICENSE` & `kathara-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/PKG-INFO` & `kathara-3.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kathara
-Version: 3.6.0
+Version: 3.6.2
 Summary: A lightweight container-based emulation system.
 Home-page: https://www.kathara.org
-Download-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.6.0.tar.gz
+Download-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.6.2.tar.gz
 Author: Kathara Framework
 Author-email: Kathara Framework <contact@kathara.org>
 Maintainer-email: Tommaso Caiazzi <contact@kathara.org>, Mariano Scazzariello <contact@kathara.org>, Lorenzo Ariemma <contact@kathara.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `kathara-3.6.0/README.md` & `kathara-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/pyproject.toml` & `kathara-3.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kathara"
-version = "3.6.0"
+version = "3.6.2"
 description = "A lightweight container-based emulation system."
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 keywords = ["NETWORK-EMULATION", "CONTAINERS", "NFV"]
 authors = [
     { name = "Kathara Framework", email = "contact@kathara.org" } # Optional
```

### Comparing `kathara-3.6.0/setup.cfg` & `kathara-3.6.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kathara
-version = 3.6.0
+version = 3.6.2
 author = Kathara Framework
 author_email = contact@kathara.org
 description = A lightweight container based emulation system
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = www.kathara.org
 project_urls =
```

### Comparing `kathara-3.6.0/setup.py` & `kathara-3.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from setuptools import find_packages
 
 setup(
     name='kathara',
     package_dir={'': 'src'},
     packages=find_packages('src'),
     py_modules=['kathara'],
-    version='3.6.0',
+    version='3.6.2',
     license='gpl-3.0',
     description='A lightweight container based emulation system.',
     author='Kathara Framework',
     author_email='contact@kathara.org',
     url='https://www.kathara.org',
-    download_url='https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.6.0.tar.gz',
+    download_url='https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.6.2.tar.gz',
     keywords=['NETWORK-EMULATION', 'CONTAINERS', 'NFV'],
     install_requires=[
         "binaryornot>=0.4.4",
         "docker>=6.0.1",
         "kubernetes>=23.3.0",
         "requests>=2.22.0",
         "coloredlogs>=10.0",
```

### Comparing `kathara-3.6.0/src/Kathara/auth/PrivilegeHandler.py` & `kathara-3.6.2/src/Kathara/auth/PrivilegeHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/CheckCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/CheckCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/ConnectCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/ConnectCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/ExecCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/ExecCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/LcleanCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/LcleanCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/LconfigCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/LconfigCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/LinfoCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/LinfoCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/ListCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/ListCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/LrestartCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/LrestartCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/LstartCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/LstartCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/LtestCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/LtestCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/VcleanCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/VcleanCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/VconfigCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/VconfigCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/VstartCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/VstartCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/command/WipeCommand.py` & `kathara-3.6.2/src/Kathara/cli/command/WipeCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/ui/event/HandleProgressBar.py` & `kathara-3.6.2/src/Kathara/cli/ui/event/HandleProgressBar.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/ui/event/OpenMachineTerminal.py` & `kathara-3.6.2/src/Kathara/cli/ui/event/OpenMachineTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/ui/event/UpdateDockerImage.py` & `kathara-3.6.2/src/Kathara/cli/ui/event/UpdateDockerImage.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/ui/event/register.py` & `kathara-3.6.2/src/Kathara/cli/ui/event/register.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/ui/setting/CommonOptionsHandler.py` & `kathara-3.6.2/src/Kathara/cli/ui/setting/CommonOptionsHandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from . import utils as setting_utils
-from ....webhooks.DockerHubApi import DockerHubApi
 from ....exceptions import HTTPConnectionError
 from ....foundation.cli.ui.setting.OptionsHandler import OptionsHandler
 from ....manager.Kathara import Kathara
 from ....setting.Setting import Setting, DEFAULTS, AVAILABLE_DEBUG_LEVELS
 from ....trdparty.consolemenu import *
 from ....trdparty.consolemenu.items import *
 from ....trdparty.consolemenu.validators.regex import RegexValidator
 from ....utils import exec_by_platform
 from ....validator.ImageValidator import ImageValidator
 from ....validator.TerminalValidator import TerminalValidator
+from ....webhooks.DockerHubApi import DockerHubApi
 
 SHELLS_HINT = ["/bin/bash", "/bin/sh", "/bin/ash", "/bin/ksh", "/bin/zsh", "/bin/fish", "/bin/csh", "/bin/tcsh"]
 TERMINALS_OSX = ["Terminal", "iTerm"]
 
 
 class CommonOptionsHandler(OptionsHandler):
     def add_items(self, current_menu: ConsoleMenu, menu_formatter: MenuFormatBuilder) -> None:
@@ -48,17 +48,15 @@
                                           prologue_text="""Default Docker image when you start a network scenario or """
                                                         """a single Kathara device.
                                                         Default is `%s`.""" % DEFAULTS['image'],
                                           formatter=menu_formatter
                                           )
 
         try:
-            for image in DockerHubApi.get_images():
-                image_name = "%s/%s" % (image['namespace'], image['name'])
-
+            for image_name in DockerHubApi.get_tagged_images():
                 select_image_menu.append_item(FunctionItem(text=image_name,
                                                            function=setting_utils.update_setting_value,
                                                            args=['image', image_name],
                                                            should_exit=True
                                                            )
                                               )
         except HTTPConnectionError:
```

### Comparing `kathara-3.6.0/src/Kathara/cli/ui/setting/DockerOptionsHandler.py` & `kathara-3.6.2/src/Kathara/cli/ui/setting/DockerOptionsHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py` & `kathara-3.6.2/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/ui/setting/SettingsMenuFactory.py` & `kathara-3.6.2/src/Kathara/cli/ui/setting/SettingsMenuFactory.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/ui/setting/utils.py` & `kathara-3.6.2/src/Kathara/cli/ui/setting/utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/cli/ui/utils.py` & `kathara-3.6.2/src/Kathara/cli/ui/utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/decorators.py` & `kathara-3.6.2/src/Kathara/decorators.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/event/EventDispatcher.py` & `kathara-3.6.2/src/Kathara/event/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/exceptions.py` & `kathara-3.6.2/src/Kathara/exceptions.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/foundation/cli/CliArgs.py` & `kathara-3.6.2/src/Kathara/foundation/cli/CliArgs.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/foundation/cli/command/Command.py` & `kathara-3.6.2/src/Kathara/foundation/cli/command/Command.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py` & `kathara-3.6.2/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/foundation/factory/Factory.py` & `kathara-3.6.2/src/Kathara/foundation/factory/Factory.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/foundation/manager/IManager.py` & `kathara-3.6.2/src/Kathara/foundation/manager/IManager.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/foundation/manager/stats/ILinkStats.py` & `kathara-3.6.2/src/Kathara/foundation/manager/stats/ILinkStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/foundation/manager/stats/IMachineStats.py` & `kathara-3.6.2/src/Kathara/foundation/manager/stats/IMachineStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/foundation/manager/terminal/Terminal.py` & `kathara-3.6.2/src/Kathara/foundation/manager/terminal/Terminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/foundation/manager/terminal/terminal_utils.py` & `kathara-3.6.2/src/Kathara/foundation/manager/terminal/terminal_utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/foundation/model/FilesystemMixin.py` & `kathara-3.6.2/src/Kathara/foundation/model/FilesystemMixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,19 +201,18 @@
             file_lines = file.readlines()
             file.seek(0)
             file.truncate()
             new_lines = []
             for line in file_lines:
                 if searched_line.strip() == line.strip():
                     if not first_occurrence or (first_occurrence and n_added == 0):
-                        new_lines.append(line_to_add)
+                        new_lines.append(line_to_add + '\n')
                         n_added += 1
-                new_lines.append(line.strip())
-
-            file.writelines(s + '\n' for s in new_lines)
+                new_lines.append(line.replace("\n\r", "\n").replace("\r\n", "\n"))
+            file.writelines(new_lines)
 
         return n_added
 
     def write_line_after(self, file_path: str, line_to_add: str, searched_line: str, first_occurrence: bool = False) \
             -> int:
         """Write a new line after a specific line in a file.
 
@@ -238,21 +237,21 @@
         n_added = 0
         with self.fs.open(file_path, "r+") as file:
             file_lines = file.readlines()
             file.seek(0)
             file.truncate()
             new_lines = []
             for line in file_lines:
-                new_lines.append(line.strip())
+                new_lines.append(line.replace("\n\r", "\n").replace("\r\n", "\n"))
                 if searched_line.strip() == line.strip():
                     if not first_occurrence or (first_occurrence and n_added == 0):
-                        new_lines.append(line_to_add)
+                        new_lines.append(("\n" if not line.endswith("\n") else "") + line_to_add + '\n')
                         n_added += 1
 
-            file.writelines(s + '\n' for s in new_lines)
+            file.writelines(new_lines)
 
         return n_added
 
     def delete_line(self, file_path: str, line_to_delete: str, first_occurrence: bool = False) -> int:
         """Delete a specified line in a file.
 
         Args:
@@ -280,12 +279,12 @@
             new_lines = []
             for line in file_lines:
                 if line_to_delete.strip() == line.strip():
                     if not first_occurrence or (first_occurrence and n_deleted == 0):
                         n_deleted += 1
                         continue
 
-                new_lines.append(line.strip())
+                new_lines.append(line.replace("\n\r", "\n").replace("\r\n", "\n"))
 
-            file.writelines(s + '\n' for s in new_lines)
+            file.writelines(new_lines)
 
         return n_deleted
```

### Comparing `kathara-3.6.0/src/Kathara/foundation/setting/SettingsAddon.py` & `kathara-3.6.2/src/Kathara/foundation/setting/SettingsAddon.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/foundation/test/Test.py` & `kathara-3.6.2/src/Kathara/foundation/test/Test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/Kathara.py` & `kathara-3.6.2/src/Kathara/manager/Kathara.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/docker/DockerImage.py` & `kathara-3.6.2/src/Kathara/manager/docker/DockerImage.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/docker/DockerLink.py` & `kathara-3.6.2/src/Kathara/manager/docker/DockerLink.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/docker/DockerMachine.py` & `kathara-3.6.2/src/Kathara/manager/docker/DockerMachine.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,18 +194,18 @@
             for (host_port, protocol), guest_port in ports_info.items():
                 ports['%d/%s' % (guest_port, protocol)] = host_port
 
         # Get the general options into a local variable (just to avoid accessing the lab object every time)
         options = machine.lab.general_options
 
         # If bridged is required in command line but not defined in machine meta, add it.
-        if "bridged" in options and not machine.meta['bridged']:
+        if "bridged" in options and not machine.is_bridged():
             machine.add_meta("bridged", True)
 
-        if ports and not machine.meta['bridged']:
+        if ports and not machine.is_bridged():
             logging.warning(
                 "To expose ports of device `%s` on the host, "
                 "you have to specify the `bridged` option on that device." % machine.name
             )
 
         # If any exec command is passed in command line, add it.
         if "exec" in options:
@@ -215,15 +215,15 @@
         # This should be used in container create function
         first_network = None
         if machine.interfaces:
             first_network = machine.interfaces[0].api_object
 
         # If no interfaces are declared in machine, but bridged mode is required, get bridge as first link.
         # Flag that bridged is already connected (because there's another check in `start`).
-        if first_network is None and machine.meta['bridged']:
+        if first_network is None and machine.is_bridged():
             first_network = machine.lab.get_or_new_link(BRIDGE_LINK_NAME).api_object
             machine.add_meta("bridge_connected", True)
 
         # Sysctl params to pass to the container creation
         sysctl_parameters = {RP_FILTER_NAMESPACE % x: 0 for x in ["all", "default", "lo"]}
 
         if first_network:
@@ -307,14 +307,15 @@
         Returns:
             None
 
         Raises:
             DockerPluginError: If Kathara has been left in an inconsistent state.
             APIError: If the Docker APIs return an error.
         """
+        machine.api_object.reload()
         attached_networks = machine.api_object.attrs["NetworkSettings"]["Networks"]
 
         if link.api_object.name not in attached_networks:
             try:
                 link.api_object.connect(machine.api_object)
             except APIError as e:
                 if e.response.status_code == 500 and \
@@ -331,14 +332,15 @@
         Args:
             machine (Kathara.model.Machine): A Kathara device.
             link (Kathara.model.Link): A Kathara collision domain object.
 
         Returns:
             None
         """
+        machine.api_object.reload()
         attached_networks = machine.api_object.attrs["NetworkSettings"]["Networks"]
 
         if link.api_object.name in attached_networks:
             link.api_object.disconnect(machine.api_object)
 
     def start(self, machine: Machine) -> None:
         """Start the Docker container representing the device.
@@ -385,15 +387,15 @@
                         ("network does not exist" in e.explanation or "endpoint does not exist" in e.explanation):
                     raise DockerPluginError(
                         "Kathara has been left in an inconsistent state! Please run `kathara wipe`.")
                 else:
                     raise e
 
         # Bridged connection required but not added in `deploy` method.
-        if "bridge_connected" not in machine.meta and machine.meta['bridged']:
+        if "bridge_connected" not in machine.meta and machine.is_bridged():
             bridge_link = machine.lab.get_or_new_link(BRIDGE_LINK_NAME).api_object
             bridge_link.connect(machine.api_object)
 
         # Append executed machine startup commands inside the /var/log/startup.log file
         if machine.meta['startup_commands']:
             new_commands = []
             for command in machine.meta['startup_commands']:
```

### Comparing `kathara-3.6.0/src/Kathara/manager/docker/DockerManager.py` & `kathara-3.6.2/src/Kathara/manager/docker/DockerManager.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/docker/DockerPlugin.py` & `kathara-3.6.2/src/Kathara/manager/docker/DockerPlugin.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/docker/stats/DockerLinkStats.py` & `kathara-3.6.2/src/Kathara/manager/docker/stats/DockerLinkStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/docker/stats/DockerMachineStats.py` & `kathara-3.6.2/src/Kathara/manager/docker/stats/DockerMachineStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py` & `kathara-3.6.2/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py` & `kathara-3.6.2/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesConfig.py` & `kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesConfig.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesConfigMap.py` & `kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesConfigMap.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesLink.py` & `kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesLink.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesMachine.py` & `kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesMachine.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
         """
         logging.debug("Creating device `%s`..." % machine.name)
 
         # Get the general options into a local variable (just to avoid accessing the lab object every time)
         options = machine.lab.general_options
 
         # If bridged is defined for the device, throw a warning.
-        if "bridged" in options or machine.meta['bridged']:
+        if "bridged" in options or machine.is_bridged():
             logging.warning('Bridged option is not supported on Megalos. It will be ignored.')
 
         # If any exec command is passed in command line, add it.
         if "exec" in options:
             machine.add_meta("exec", options["exec"])
 
         # Sysctl params to pass to the container creation
```

### Comparing `kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesManager.py` & `kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesManager.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/kubernetes/KubernetesNamespace.py` & `kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesNamespace.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py` & `kathara-3.6.2/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py` & `kathara-3.6.2/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py` & `kathara-3.6.2/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/model/ExternalLink.py` & `kathara-3.6.2/src/Kathara/model/ExternalLink.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/model/Lab.py` & `kathara-3.6.2/src/Kathara/model/Lab.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from . import Machine as MachinePackage
 from .ExternalLink import ExternalLink
 from .Link import Link
 from .. import utils
 from ..exceptions import LinkNotFoundError, MachineNotFoundError, MachineAlreadyExistsError, LinkAlreadyExistsError
 from ..foundation.model.FilesystemMixin import FilesystemMixin
 
+LAB_METADATA: List[str] = ["LAB_NAME", "LAB_DESCRIPTION", "LAB_VERSION", "LAB_AUTHOR", "LAB_EMAIL", "LAB_WEB"]
+
 
 class Lab(FilesystemMixin):
     """A Kathara network scenario, containing information about devices and collision domains.
 
     Attributes:
         name (str): The name of the network scenario.
         description (str): A short description of the network scenario.
@@ -100,33 +102,31 @@
         machine = self.get_or_new_machine(machine_name)
         link = self.get_or_new_link(link_name)
 
         machine.add_interface(link, number=machine_iface_number)
 
         return machine, link
 
-    def assign_meta_to_machine(self, machine_name: str, meta_name: str, meta_value: str) -> 'MachinePackage.Machine':
+    def assign_meta_to_machine(self, machine_name: str, meta_name: str, meta_value: str) -> Optional[Any]:
         """Assign meta information to the specified device.
 
         Args:
             machine_name (str): The name of the device.
             meta_name (str): The name of the meta property.
             meta_value (str): The value of the meta property.
 
         Returns:
-            Kathara.model.Machine: The Kathara device specified by the name.
+            Optional[Any]: Previous value if meta was already assigned, None otherwise.
 
         Raises:
             MachineOptionError: If invalid values are specified for meta properties.
         """
         machine = self.get_or_new_machine(machine_name)
 
-        machine.add_meta(meta_name, meta_value)
-
-        return machine
+        return machine.add_meta(meta_name, meta_value)
 
     def attach_external_links(self, external_links: Dict[str, List[ExternalLink]]) -> None:
         """Attach external collision domains to the network scenario.
 
         Args:
             external_links (Dict[Kathara.model.Link, List[Kathara.model.ExternalLink]]): Keys are Link objects,
             values are ExternalLink objects.
@@ -220,15 +220,15 @@
         Returns:
             Kathara.model.Machine: A Kathara device.
 
         Raises:
             MachineAlreadyExistsError: If the device is already in the network scenario.
         """
         if name in self.machines:
-            raise MachineAlreadyExistsError(f"Device {name} already in the network scenario.")
+            raise MachineAlreadyExistsError(name)
 
         self.machines[name] = MachinePackage.Machine(self, name, **kwargs)
 
         return self.machines[name]
 
     def get_or_new_machine(self, name: str, **kwargs: Dict[str, Any]) -> 'MachinePackage.Machine':
         """Get the specified device. If it not exists, create and add it to the devices list.
```

### Comparing `kathara-3.6.0/src/Kathara/model/Link.py` & `kathara-3.6.2/src/Kathara/model/Link.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/model/Machine.py` & `kathara-3.6.2/src/Kathara/model/Machine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import collections
 import logging
 import re
-import tempfile
 from io import BytesIO
 from typing import Dict, Any, Tuple, Optional, List, OrderedDict, TextIO, Union, BinaryIO
 
 # noinspection PyUnresolvedReferences
 from fs._bulk import Copier
 from fs.base import FS
 from fs.copy import copy_fs, copy_file
@@ -61,19 +60,18 @@
 
         self.lab: LabPackage.Lab = lab
         self.name: str = name
 
         self.interfaces: OrderedDict[int, Link] = collections.OrderedDict()
 
         self.meta: Dict[str, Any] = {
+            'startup_commands': [],
             'sysctls': {},
             'envs': {},
-            'bridged': False,
             'ports': {},
-            'startup_commands': []
         }
 
         self.api_object: Any = None
 
         self.fs: FS = self.lab.fs.opendir(self.name) \
             if self.lab.fs.exists(self.name) and self.lab.fs.isdir(self.name) else None
 
@@ -125,64 +123,69 @@
             )
 
         self.interfaces = collections.OrderedDict(
             map(lambda x: x if x[1] is not None and x[1].name != link.name else (x[0], None), self.interfaces.items())
         )
         link.machines.pop(self.name)
 
-    def add_meta(self, name: str, value: Any) -> None:
+    def add_meta(self, name: str, value: Any) -> Optional[Any]:
         """Add a meta property to the device.
 
         Args:
             name (str): The name of the property.
             value (Any): The value of the property.
 
         Returns:
-            None
+            Optional[Any]: Previous value if meta was already assigned, None otherwise.
 
         Raises:
             MachineOptionError: If the specified value is not valid for the specified property.
         """
         if name == "exec":
             self.meta['startup_commands'].append(value)
-            return
+            return None
 
         if name == "bridged":
+            old_value = self.meta[name] if name in self.meta else None
             self.meta[name] = strtobool(str(value))
-            return
+            return old_value
 
         if name == "sysctl":
-            matches = re.search(r"^(?P<key>net\.(\w+\.)+\w+)=(?P<value>\w+)$", value)
+            matches = re.search(r"^(?P<key>net\.([\w-]+\.)+[\w-]+)=(?P<value>\w+)$", value)
 
             # Check for valid kv-pair
             if matches:
                 key = matches.group("key").strip()
                 val = matches.group("value").strip()
 
+                old_value = self.meta['sysctls'][key] if key in self.meta['sysctls'] else None
+
                 # Convert to int if possible
                 self.meta['sysctls'][key] = int(val) if val.isdigit() else val
             else:
                 raise MachineOptionError(
                     "Invalid sysctl value (`%s`) on `%s`, missing `=` or value not in `net.` namespace."
                     % (value, self.name)
                 )
-            return
+            return old_value
 
         if name == "env":
             matches = re.search(r"^(?P<key>\w+)=(?P<value>\S+)$", value)
 
             # Check for valid kv-pair
             if matches:
                 key = matches.group("key").strip()
                 val = matches.group("value").strip()
 
+                old_value = self.meta['envs'][key] if key in self.meta['envs'] else None
+
                 self.meta['envs'][key] = val
             else:
                 raise MachineOptionError("Invalid env value (`%s`) on `%s`." % (value, self.name))
-            return
+            return old_value
 
         if name == "port":
             if '/' in value:
                 (ports, protocol) = value.split('/')
             else:
                 (ports, protocol) = value, 'tcp'
 
@@ -192,20 +195,66 @@
                 (host_port, guest_port) = ports.split(':')
 
             protocol = protocol.lower()
             if protocol not in ['tcp', 'udp', 'sctp']:
                 raise MachineOptionError("Port protocol value not valid on `%s`." % self.name)
 
             try:
-                self.meta['ports'][(int(host_port), protocol)] = int(guest_port)
+                key_tuple = (int(host_port), protocol)
+
+                old_value = self.meta['ports'][key_tuple] if key_tuple in self.meta['ports'] else None
+
+                self.meta['ports'][key_tuple] = int(guest_port)
             except ValueError:
                 raise MachineOptionError("Port value not valid on `%s`." % self.name)
-            return
+            return old_value
 
+        old_value = self.meta[name] if name in self.meta else None
         self.meta[name] = value
+        return old_value
+
+    def update_meta(self, args: Dict[str, Any]) -> None:
+        """Update the device metas from a dict.
+
+        Args:
+            args (Dict[str, Any]): Keys are the meta properties names, values are the updated meta properties values.
+
+        Returns:
+            None
+        """
+        if 'exec_commands' in args and args['exec_commands'] is not None:
+            for command in args['exec_commands']:
+                self.add_meta("exec", command)
+
+        if 'mem' in args and args['mem'] is not None:
+            self.add_meta("mem", args['mem'])
+
+        if 'cpus' in args and args['cpus'] is not None:
+            self.add_meta("cpus", args['cpus'])
+
+        if 'image' in args and args['image'] is not None:
+            self.add_meta("image", args['image'])
+
+        if 'bridged' in args and args['bridged'] is not None and args['bridged']:
+            self.add_meta("bridged", True)
+
+        if 'ports' in args and args['ports'] is not None:
+            for port in args['ports']:
+                self.add_meta("port", port)
+
+        if 'num_terms' in args and args['num_terms'] is not None:
+            self.add_meta('num_terms', args['num_terms'])
+
+        if 'sysctls' in args and args['sysctls'] is not None:
+            for sysctl in args['sysctls']:
+                self.add_meta("sysctl", sysctl)
+
+        if 'envs' in args and args['envs'] is not None:
+            for envs in args['envs']:
+                self.add_meta("env", envs)
 
     def check(self) -> None:
         """Sort interfaces and check if there are missing interface numbers.
 
         Returns:
             None
 
@@ -257,14 +306,57 @@
         if not is_empty:
             file.seek(0)
             return file.read()
 
         # If no machine files are found, return None.
         return None
 
+    def get_startup_commands(self) -> List[str]:
+        """Get the additional device startup commands.
+
+        Returns:
+            List[str]: The list containing the additional commands.
+        """
+        return self.meta['startup_commands']
+
+    def is_bridged(self) -> bool:
+        """Return True if the device is bridged, else return False.
+
+        Returns:
+            bool: True if the device is bridged, else False.
+        """
+        if "bridged" not in self.meta:
+            return False
+
+        return self.meta['bridged']
+
+    def get_sysctls(self) -> Dict[str, Union[int, str]]:
+        """Get the sysctls specified for the device.
+
+        Returns:
+            Dict[str, Union[int, str]]: Keys contain the sysctls to set, values are the values to apply.
+        """
+        return self.meta['sysctls']
+
+    def get_envs(self) -> Dict[str, Union[int, str]]:
+        """Get the environment variables specified for the device.
+
+        Returns:
+            Dict[str, Union[int, str]]: Keys are environment variables to set, values are the values to apply.
+        """
+        return self.meta['envs'] if self.meta['envs'] else {}
+
+    def get_ports(self) -> Dict[Tuple[int, str], int]:
+        """Get the port mapping of the device.
+
+        Returns:
+            Dict[(int, str), int]: Keys are pairs (host port, protocol), values specifies the guest port.
+        """
+        return self.meta['ports']
+
     def get_image(self) -> str:
         """Get the image of the device, if defined in options or device meta. If not, use default one.
 
         Returns:
             str: The name of the device image.
         """
         return self.lab.general_options["image"] if "image" in self.lab.general_options else \
@@ -321,54 +413,22 @@
             try:
                 return int(float(self.meta["cpus"]) * multiplier)
             except ValueError:
                 raise MachineOptionError("CPU value not valid on `%s`." % self.name)
 
         return None
 
-    def get_ports(self) -> Dict[Tuple[int, str], int]:
-        """Get the port mapping of the device.
-
-        Returns:
-            Dict[(int, str), int]: Keys are pairs (host port, protocol), values specifies the guest port.
-        """
-        return self.meta['ports']
-
-    def get_sysctls(self) -> Dict[str, Union[int, str]]:
-        """Get the sysctls specified for the device.
-
-        Returns:
-            Dict[str, Union[int, str]]: Keys contain the sysctls to set, values are the values to apply.
-        """
-        return self.meta['sysctls']
-
     def get_shell(self) -> str:
         """Get the custom shell specified for the device.
 
         Returns:
             str: The path of the custom shell specified for connecting to the device.
         """
         return self.meta['shell'] if 'shell' in self.meta else Setting.get_instance().device_shell
 
-    def get_envs(self) -> Dict[str, Union[int, str]]:
-        """Get the environment variables specified for the device.
-
-        Returns:
-            Dict[str, Union[int, str]]: Keys are environment variables to set, values are the values to apply.
-        """
-        return self.meta['envs'] if self.meta['envs'] else {}
-
-    def is_bridged(self) -> bool:
-        """Return True if the device is bridged, else return False.
-
-        Returns:
-            bool: True if the device is bridged, else False.
-        """
-        return self.meta['bridged']
-
     def get_num_terms(self) -> int:
         """Get the number of terminals to be opened for the device.
 
         Returns:
             int: The number of terminals to be opened.
 
         Raises:
@@ -402,62 +462,14 @@
         """
         try:
             return strtobool(self.lab.general_options["ipv6"]) if "ipv6" in self.lab.general_options else \
                 strtobool(self.meta["ipv6"]) if "ipv6" in self.meta else Setting.get_instance().enable_ipv6
         except ValueError:
             raise MachineOptionError("IPv6 value not valid on `%s`." % self.name)
 
-    def get_startup_commands(self) -> List[str]:
-        """Get the additional device startup commands.
-
-        Returns:
-            List[str]: The list containing the additional commands.
-        """
-        return self.meta['startup_commands']
-
-    def update_meta(self, args: Dict[str, Any]) -> None:
-        """Update the device metas from a dict.
-
-        Args:
-            args (Dict[str, Any]): Keys are the meta properties names, values are the updated meta properties values.
-
-        Returns:
-            None
-        """
-        if 'exec_commands' in args and args['exec_commands'] is not None:
-            for command in args['exec_commands']:
-                self.add_meta("exec", command)
-
-        if 'mem' in args and args['mem'] is not None:
-            self.add_meta("mem", args['mem'])
-
-        if 'cpus' in args and args['cpus'] is not None:
-            self.add_meta("cpus", args['cpus'])
-
-        if 'image' in args and args['image'] is not None:
-            self.add_meta("image", args['image'])
-
-        if 'bridged' in args and args['bridged'] is not None and args['bridged']:
-            self.add_meta("bridged", True)
-
-        if 'ports' in args and args['ports'] is not None:
-            for port in args['ports']:
-                self.add_meta("port", port)
-
-        if 'num_terms' in args and args['num_terms'] is not None:
-            self.add_meta('num_terms', args['num_terms'])
-
-        if 'sysctls' in args and args['sysctls'] is not None:
-            for sysctl in args['sysctls']:
-                self.add_meta("sysctl", sysctl)
-
-        if 'envs' in args and args['envs'] is not None:
-            for envs in args['envs']:
-                self.add_meta("env", envs)
-
     # Override FilesystemMixin methods to handle the condition if we want to add a file but self.fs is not set
     # In this case, we create the machine directory and assign it to self.fs before calling the actual method
     def create_file_from_string(self, content: str, dst_path: str) -> None:
         """Create a file from a string in the device fs. If fs is None, create it in the network scenario.
 
         Args:
             content (str): The string representing the content of the file to create.
```

### Comparing `kathara-3.6.0/src/Kathara/os/Networking.py` & `kathara-3.6.2/src/Kathara/os/Networking.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/parser/netkit/DepParser.py` & `kathara-3.6.2/src/Kathara/parser/netkit/DepParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/parser/netkit/ExtParser.py` & `kathara-3.6.2/src/Kathara/parser/netkit/ExtParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/parser/netkit/FolderParser.py` & `kathara-3.6.2/src/Kathara/parser/netkit/FolderParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/parser/netkit/LabParser.py` & `kathara-3.6.2/src/Kathara/parser/netkit/LabParser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import logging
 import mmap
 import os
 import re
 
-from ...model.Lab import Lab
+from ...model.Lab import Lab, LAB_METADATA
 from ...utils import RESERVED_MACHINE_NAMES
 
 
 class LabParser(object):
     """Class responsible for parsing the lab.conf file."""
 
     @staticmethod
@@ -60,25 +61,23 @@
                     if re.search(r"^\w+$", value):
                         lab.connect_machine_to_link(key, value, machine_iface_number=interface_number)
                     else:
                         raise SyntaxError(f"In lab.conf - Line {line_number}: "
                                           f"Collision domain `{value}` contains non-alphanumeric characters.")
                 except ValueError:
                     # Not an interface, add it to the machine metas.
-                    lab.assign_meta_to_machine(key, arg, value)
+                    if lab.assign_meta_to_machine(key, arg, value) is not None:
+                        logging.warning(f"In lab.conf - Line {line_number}: "
+                                        f"Device `{key}` already has a value assigned to meta `{arg}`. "
+                                        f"Previous value has been overwritten with `{value}`.")
             else:
                 if not line.startswith('#') and \
                         line.strip():
-                    if not line.startswith("LAB_NAME=") and \
-                            not line.startswith("LAB_DESCRIPTION=") and \
-                            not line.startswith("LAB_VERSION=") and \
-                            not line.startswith("LAB_AUTHOR=") and \
-                            not line.startswith("LAB_EMAIL=") and \
-                            not line.startswith("LAB_WEB="):
-                        raise SyntaxError(f"In lab.conf - Line {line_number}: `{line}`")
+                    if not any([line.startswith(f"{x}=") for x in LAB_METADATA]):
+                        raise SyntaxError(f"In lab.conf - Line {line_number}: `{line}`.")
                     else:
                         (key, value) = line.split("=")
                         key = key.replace("LAB_", "").lower()
                         setattr(lab, key, value.replace('"', '').replace("'", '').strip())
 
             line_number += 1
             line = lab_mem_file.readline().decode('utf-8')
```

### Comparing `kathara-3.6.0/src/Kathara/parser/netkit/OptionParser.py` & `kathara-3.6.2/src/Kathara/parser/netkit/OptionParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/setting/Setting.py` & `kathara-3.6.2/src/Kathara/setting/Setting.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/setting/addon/DockerSettingsAddon.py` & `kathara-3.6.2/src/Kathara/setting/addon/DockerSettingsAddon.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/setting/addon/KubernetesSettingsAddon.py` & `kathara-3.6.2/src/Kathara/setting/addon/KubernetesSettingsAddon.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/strings.py` & `kathara-3.6.2/src/Kathara/strings.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/test/BuiltinTest.py` & `kathara-3.6.2/src/Kathara/test/BuiltinTest.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/test/UserTest.py` & `kathara-3.6.2/src/Kathara/test/UserTest.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/__init__.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/__init__.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/console_menu.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/console_menu.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/__init__.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/__init__.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_borders.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_borders.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_margins.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_margins.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_padding.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_padding.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/format/menu_style.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_style.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/command_item.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/command_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/external_item.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/external_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/function_item.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/function_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/selection_item.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/selection_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/items/submenu_item.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/submenu_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/menu_component.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/menu_component.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/menu_formatter.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/menu_formatter.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/multiselect_menu.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/multiselect_menu.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/prompt_utils.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/screen.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/screen.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/selection_menu.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/selection_menu.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/base.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/base.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/regex.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/regex.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/consolemenu/validators/url.py` & `kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/url.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/curses/curses.py` & `kathara-3.6.2/src/Kathara/trdparty/curses/curses.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/depgen/depgen.py` & `kathara-3.6.2/src/Kathara/trdparty/depgen/depgen.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/libtmux/tmux.py` & `kathara-3.6.2/src/Kathara/trdparty/libtmux/tmux.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/trdparty/strtobool/strtobool.py` & `kathara-3.6.2/src/Kathara/trdparty/strtobool/strtobool.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/utils.py` & `kathara-3.6.2/src/Kathara/utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/validator/ImageValidator.py` & `kathara-3.6.2/src/Kathara/validator/ImageValidator.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/Kathara/webhooks/GitHubApi.py` & `kathara-3.6.2/src/Kathara/webhooks/GitHubApi.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.0/src/kathara.egg-info/PKG-INFO` & `kathara-3.6.2/src/kathara.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kathara
-Version: 3.6.0
+Version: 3.6.2
 Summary: A lightweight container-based emulation system.
 Home-page: https://www.kathara.org
-Download-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.6.0.tar.gz
+Download-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.6.2.tar.gz
 Author: Kathara Framework
 Author-email: Kathara Framework <contact@kathara.org>
 Maintainer-email: Tommaso Caiazzi <contact@kathara.org>, Mariano Scazzariello <contact@kathara.org>, Lorenzo Ariemma <contact@kathara.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `kathara-3.6.0/src/kathara.py` & `kathara-3.6.2/src/kathara.py`

 * *Files identical despite different names*

