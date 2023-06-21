# Comparing `tmp/gpt-term-1.1.4.tar.gz` & `tmp/gpt-term-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-term-1.1.4.tar", last modified: Wed Jun 14 16:08:21 2023, max compression
+gzip compressed data, was "gpt-term-1.2.0.tar", last modified: Wed Jun 21 08:04:38 2023, max compression
```

## Comparing `gpt-term-1.1.4.tar` & `gpt-term-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:08:21.680472 gpt-term-1.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:08:21.664472 gpt-term-1.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:08:21.668472 gpt-term-1.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-14 16:07:52.000000 gpt-term-1.1.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-14 16:07:52.000000 gpt-term-1.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-14 16:07:52.000000 gpt-term-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-06-14 16:08:21.676473 gpt-term-1.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:08:21.668472 gpt-term-1.1.4/README.assets/
--rw-r--r--   0 runner    (1001) docker     (123)   297411 2023-06-14 16:07:52.000000 gpt-term-1.1.4/README.assets/image-20230303233352970.png
--rw-r--r--   0 runner    (1001) docker     (123)  3707698 2023-06-14 16:07:52.000000 gpt-term-1.1.4/README.assets/small.gif
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-06-14 16:07:52.000000 gpt-term-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-06-14 16:07:52.000000 gpt-term-1.1.4/README.zh-CN.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-06-14 16:07:52.000000 gpt-term-1.1.4/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:08:21.672472 gpt-term-1.1.4/gpt_term/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 16:07:52.000000 gpt-term-1.1.4/gpt_term/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 16:07:52.000000 gpt-term-1.1.4/gpt_term/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 16:08:21.000000 gpt-term-1.1.4/gpt_term/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-14 16:07:52.000000 gpt-term-1.1.4/gpt_term/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:08:21.676473 gpt-term-1.1.4/gpt_term/locale/
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-06-14 16:07:52.000000 gpt-term-1.1.4/gpt_term/locale/gpt_term.de.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-06-14 16:07:52.000000 gpt-term-1.1.4/gpt_term/locale/gpt_term.en.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-06-14 16:07:52.000000 gpt-term-1.1.4/gpt_term/locale/gpt_term.jp.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-14 16:07:52.000000 gpt-term-1.1.4/gpt_term/locale/gpt_term.zh_CN.yml
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-14 16:07:52.000000 gpt-term-1.1.4/gpt_term/locale.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48560 2023-06-14 16:07:52.000000 gpt-term-1.1.4/gpt_term/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:08:21.676473 gpt-term-1.1.4/gpt_term.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-06-14 16:08:21.000000 gpt-term-1.1.4/gpt_term.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-14 16:08:21.000000 gpt-term-1.1.4/gpt_term.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:08:21.000000 gpt-term-1.1.4/gpt_term.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-14 16:08:21.000000 gpt-term-1.1.4/gpt_term.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-14 16:08:21.000000 gpt-term-1.1.4/gpt_term.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 16:08:21.000000 gpt-term-1.1.4/gpt_term.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-14 16:07:52.000000 gpt-term-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-14 16:07:52.000000 gpt-term-1.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:08:21.680472 gpt-term-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:04:38.707402 gpt-term-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:04:38.699402 gpt-term-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:04:38.699402 gpt-term-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 08:04:27.000000 gpt-term-1.2.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-21 08:04:27.000000 gpt-term-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 08:04:27.000000 gpt-term-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-06-21 08:04:38.707402 gpt-term-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:04:38.699402 gpt-term-1.2.0/README.assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   297411 2023-06-21 08:04:27.000000 gpt-term-1.2.0/README.assets/image-20230303233352970.png
+-rw-r--r--   0 runner    (1001) docker     (123)  3707698 2023-06-21 08:04:27.000000 gpt-term-1.2.0/README.assets/small.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-06-21 08:04:27.000000 gpt-term-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-06-21 08:04:27.000000 gpt-term-1.2.0/README.zh-CN.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-06-21 08:04:27.000000 gpt-term-1.2.0/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:04:38.703402 gpt-term-1.2.0/gpt_term/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-21 08:04:27.000000 gpt-term-1.2.0/gpt_term/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-21 08:04:27.000000 gpt-term-1.2.0/gpt_term/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 08:04:38.000000 gpt-term-1.2.0/gpt_term/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-21 08:04:27.000000 gpt-term-1.2.0/gpt_term/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:04:38.707402 gpt-term-1.2.0/gpt_term/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-06-21 08:04:27.000000 gpt-term-1.2.0/gpt_term/locale/gpt_term.de.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-06-21 08:04:27.000000 gpt-term-1.2.0/gpt_term/locale/gpt_term.en.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-06-21 08:04:27.000000 gpt-term-1.2.0/gpt_term/locale/gpt_term.jp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-06-21 08:04:27.000000 gpt-term-1.2.0/gpt_term/locale/gpt_term.zh_CN.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-21 08:04:27.000000 gpt-term-1.2.0/gpt_term/locale.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49394 2023-06-21 08:04:27.000000 gpt-term-1.2.0/gpt_term/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:04:38.707402 gpt-term-1.2.0/gpt_term.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-06-21 08:04:38.000000 gpt-term-1.2.0/gpt_term.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-21 08:04:38.000000 gpt-term-1.2.0/gpt_term.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:04:38.000000 gpt-term-1.2.0/gpt_term.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 08:04:38.000000 gpt-term-1.2.0/gpt_term.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 08:04:38.000000 gpt-term-1.2.0/gpt_term.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 08:04:38.000000 gpt-term-1.2.0/gpt_term.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-21 08:04:27.000000 gpt-term-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 08:04:27.000000 gpt-term-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 08:04:38.707402 gpt-term-1.2.0/setup.cfg
```

### Comparing `gpt-term-1.1.4/.github/workflows/pypi-publish.yml` & `gpt-term-1.2.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.4/LICENSE` & `gpt-term-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.4/PKG-INFO` & `gpt-term-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.1.4
+Version: 1.2.0
 Summary: Chat with GPT in Terminal
 Author: xiaoxx970, Ace-Radom
 License: MIT License
         
         Copyright (c) 2023 xiaoxx970
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,36 +59,51 @@
 
 [GPTerm implemented in C/C++](https://github.com/Ace-Radom/cGPTerm) by @Ace-Radom
 
 [gpt-term that can call POE API](https://github.com/Lemon-2333/chatgpt-in-terminal-Poe-Api) by @Lemon-2333
 
 ## Changelog
 
-### 2023-05-20
+### 2023-06-21
 
-- Added host configuration support, which is very useful when using self-built API reverse proxy server ([#49](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/49)), you can now use `gpt-term --set-host HOST` to configure host, the default is https://api.openai.com
+- Added direct query mode, now you can run `gpt-term` with the content of the question as a parameter to conduct a single question and answer
 
-### 2023-05-18
+  ```sh
+  gpt-term "What's the weather like today?"
+  ```
 
-- Added multi-language support: English, Chinese, Japanese, German, follow the system language by default, now you can use `/lang` to switch languages
+  The answer will be printed directly, or piped into a variable
+
+  ```sh
+  gpt-term "What's the weather like today" | read answer
+  echo $answer
+  ```
 
 <details>
   <summary>More Change log</summary>
 
+### 2023-05-20
+
+- Added host configuration support, which is very useful when using self-built API reverse proxy server ([#49](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/49)), you can now use `gpt-term --set-host HOST` to configure host, the default is https://api.openai.com
+
+### 2023-05-18
+
+- Added multi-language support: English, Chinese, Japanese, German, follow the system language by default, now you can use `/lang` to switch languages
 ### 2023-05-11
 
 - Find the command the user most likely intended to enter when typing an unrecognized command
 
 ### 2023-05-05
 
 - Add `/rand` command to set temperature parameter
 
 - Add overflow mode switch for `/stream` command, now you can run command `/stream visible` to switch to always visible mode. In this mode, the content that exceeds the screen will be scrolled up, and the new content will be output until it is completed
 
 ### 2023-04-23
+
 Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
 
 ### 2023-04-15
 
 - Added the ability to create a line break in single-line mode using `Esc` + `Enter`
 
 ### 2023-04-13
@@ -175,14 +190,20 @@
 
 Or:
 
 ```shell
 python3 -m gpt_term
 ```
 
+Quick query:
+
+```sh
+gpt-term "What's the weather like today?"
+```
+
 When entering a question in single-line mode, use `Esc` + `Enter` to start a new line, and use `Enter` to submit the question.
 
 Here are some common shortcut keys (also shortcut keys for the shell):
 
 - `Ctrl+_`:	Undo
 - `Ctrl+L`: Clear screen, equivalent to `clear` command in shell
 - `Ctrl+C`: Stop the current answer or cancel the current input
```

### Comparing `gpt-term-1.1.4/README.assets/image-20230303233352970.png` & `gpt-term-1.2.0/README.assets/image-20230303233352970.png`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.4/README.assets/small.gif` & `gpt-term-1.2.0/README.assets/small.gif`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.4/README.md` & `gpt-term-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,36 +23,51 @@
 
 [GPTerm implemented in C/C++](https://github.com/Ace-Radom/cGPTerm) by @Ace-Radom
 
 [gpt-term that can call POE API](https://github.com/Lemon-2333/chatgpt-in-terminal-Poe-Api) by @Lemon-2333
 
 ## Changelog
 
-### 2023-05-20
+### 2023-06-21
 
-- Added host configuration support, which is very useful when using self-built API reverse proxy server ([#49](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/49)), you can now use `gpt-term --set-host HOST` to configure host, the default is https://api.openai.com
+- Added direct query mode, now you can run `gpt-term` with the content of the question as a parameter to conduct a single question and answer
 
-### 2023-05-18
+  ```sh
+  gpt-term "What's the weather like today?"
+  ```
 
-- Added multi-language support: English, Chinese, Japanese, German, follow the system language by default, now you can use `/lang` to switch languages
+  The answer will be printed directly, or piped into a variable
+
+  ```sh
+  gpt-term "What's the weather like today" | read answer
+  echo $answer
+  ```
 
 <details>
   <summary>More Change log</summary>
 
+### 2023-05-20
+
+- Added host configuration support, which is very useful when using self-built API reverse proxy server ([#49](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/49)), you can now use `gpt-term --set-host HOST` to configure host, the default is https://api.openai.com
+
+### 2023-05-18
+
+- Added multi-language support: English, Chinese, Japanese, German, follow the system language by default, now you can use `/lang` to switch languages
 ### 2023-05-11
 
 - Find the command the user most likely intended to enter when typing an unrecognized command
 
 ### 2023-05-05
 
 - Add `/rand` command to set temperature parameter
 
 - Add overflow mode switch for `/stream` command, now you can run command `/stream visible` to switch to always visible mode. In this mode, the content that exceeds the screen will be scrolled up, and the new content will be output until it is completed
 
 ### 2023-04-23
+
 Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
 
 ### 2023-04-15
 
 - Added the ability to create a line break in single-line mode using `Esc` + `Enter`
 
 ### 2023-04-13
@@ -139,14 +154,20 @@
 
 Or:
 
 ```shell
 python3 -m gpt_term
 ```
 
+Quick query:
+
+```sh
+gpt-term "What's the weather like today?"
+```
+
 When entering a question in single-line mode, use `Esc` + `Enter` to start a new line, and use `Enter` to submit the question.
 
 Here are some common shortcut keys (also shortcut keys for the shell):
 
 - `Ctrl+_`:	Undo
 - `Ctrl+L`: Clear screen, equivalent to `clear` command in shell
 - `Ctrl+C`: Stop the current answer or cancel the current input
```

### Comparing `gpt-term-1.1.4/README.zh-CN.md` & `gpt-term-1.2.0/README.zh-CN.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,40 @@
 
 [C/C++实现的GPTerm](https://github.com/Ace-Radom/cGPTerm) by @Ace-Radom
 
 [可以调用 POE API 的 gpt-term](https://github.com/Lemon-2333/chatgpt-in-terminal-Poe-Api) by @Lemon-2333
 
 ## 更新记录
 
+### 2023-06-21
+
+- 新增直接询问模式，现在你可以运行 `gpt-term` 加上要提问的内容作为参数来进行单次提问和回答
+
+  ```sh
+  gpt-term 今天天气怎么样
+  ```
+
+  回答将直接被打印，或者使用管道存放于变量中
+
+  ```sh
+  gpt-term 今天天气怎么样 | read answer
+  echo $answer
+  ```
+
+<details>
+  <summary>更多 Change log</summary>
+
 ### 2023-05-20
 
 - 新增 host 配置项支持，在使用自建 API 反向代理服务器的时候很有用([#49](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/49))，你现在可以使用 `gpt-term --set-host HOST` 来配置 host，默认为 https://api.openai.com。
 
 ### 2023-05-18
 
 - 新增多语言支持：英语、中文、日语、德语，默认跟随系统语言，现在可以使用 `/lang` 来切换语言
 
-<details>
-  <summary>更多 Change log</summary>
-
 ### 2023-05-11
 
 - 在输入未被识别的命令时查找用户最可能想输入的命令
 
 ### 2023-05-05
 
 - 添加`/rand`命令设置temperature参数
@@ -142,14 +157,20 @@
 
 或者：
 
 ```shell
 python3 -m gpt_term
 ```
 
+单次提问：
+
+```sh
+gpt-term 今天天气怎么样
+```
+
 在默认的单行模式下输入提问时，使用 `Esc` + `Enter` 换行，`Enter` 提交
 
 以下是一些常见的快捷键（同时也是shell的快捷键）：
 
 - `Ctrl+_`: 撤消
 - `Ctrl+L`: 清屏，相当于shell中的`clear`命令
 - `Ctrl+C`: 停止当前回答或取消当前输入
```

### Comparing `gpt-term-1.1.4/gpt_term/config.ini` & `gpt-term-1.2.0/gpt_term/config.ini`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.4/gpt_term/locale/gpt_term.de.yml` & `gpt-term-1.2.0/gpt_term/locale/gpt_term.de.yml`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
   help_set_host: "API Host einstellen (wird normalerweise zur Konfiguration des Proxys verwendet)"
   help_set_key: "API-Schlüssel für OpenAI einstellen"
   help_set_timeout: "Maximale Wartezeit für API-Anfragen einstellen"
   help_set_gentitle: "Festlegen, ob automatisch ein Titel für den Chat generiert werden soll"
   help_set_lang: "Sprache einstellen"
   help_set_saveperfix: "Speicherperfix für die Chatverlaufsdatei einstellen"
   help_set_loglevel: "Log-Stufe einstellen:"
+  help_direct_query: "Frag GPT direkt an"
   #
   help_use_help: "Verwenden `[deep_sky_blue3]/help[/]`, um alle verfügbaren Slash-Befehle zu sehen"
   help_uncommand: "Unerkannter Slash-Befehl `[bold red]%{command}[/]`"
   help_mean_command: "Meinst Du `[deep_sky_blue3]%{most_similar_command}[/]`?"
   help_text: |
     [bold]Verfügbare Befehle:[/]
       /raw                     - Rohmode umschalten (zeigt den Rohtext der ChatGPT-Antwort an)
@@ -147,8 +148,8 @@
       /timeout \[new_timeout]   - Ändern der API Zeitüberschreitung
       /undo                    - Löschen der letzten Frage und Entfernen ihrer Antwort
       /delete (first)          - Löschen der ersten Unterhaltung im aktuellen Chat
       /delete all              -  Löschen aller Nachrichten und Unterhaltungen im aktuellen Chat
       /version                 - Zeigen der Lokal- und der Fernersion von gpt-term an
       /lang \[new_language]     - Sprache umschalten
       /help                    - Zeigen dieser Hilfemeldung an
-      /exit                    - Beenden der Anwendung
+      /exit                    - Beenden der Anwendung
```

### Comparing `gpt-term-1.1.4/gpt_term/locale/gpt_term.en.yml` & `gpt-term-1.2.0/gpt_term/locale/gpt_term.en.yml`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
   help_set_host: "Set the API Host to use (usually used to configure proxy)"
   help_set_key: "Set API key for OpenAI"
   help_set_timeout: "Set maximum waiting time for API requests"
   help_set_gentitle: "Set whether to automatically generate a title for chat"
   help_set_lang: "Set language"
   help_set_saveperfix: "Set chat history file's save perfix"
   help_set_loglevel: "Set log level:"
+  help_direct_query: "The direct query to GPT"
   #
   help_use_help: "Use `[deep_sky_blue3]/help[/]` to see all available slash commands"
   help_uncommand: "Unrecognized Slash Command `[bold red]%{command}[/]`"
   help_mean_command: "Do you mean `[deep_sky_blue3]%{most_similar_command}[/]`?"
   help_text: |
     [bold]Available commands:[/]
       /raw                     - Toggle raw mode (showing raw text of ChatGPT's reply)
```

### Comparing `gpt-term-1.1.4/gpt_term/locale/gpt_term.jp.yml` & `gpt-term-1.2.0/gpt_term/locale/gpt_term.jp.yml`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
   help_set_host: "使用するAPIホストを設定する（通常、プロキシを設定するために使用します。）"
   help_set_key: "OpenAIのAPIキーを設定する"
   help_set_timeout: "APIリクエストの最大待ち時間を設定する"
   help_set_gentitle: "チャットのタイトルを自動生成するかどうかを設定する"
   help_set_lang: "言語を設定する"
   help_set_saveperfix: "チャット履歴ファイルの保存プレフィックスを設定する"
   help_set_loglevel: "ログレベルを設定する:"
+  help_direct_query: "GPT への直接クエリ"
   #
   help_use_help: "`[deep_sky_blue3]/help[/]`を使用して利用可能なスラッシュコマンドをすべて表示します"
   help_uncommand: "未知のスラッシュコマンド `[bold red]%{command}[/]`"
   help_mean_command: "`[deep_sky_blue3]%{most_similar_command}[/]`を意味しますか？"
   help_text: |
     [bold]利用可能なコマンド：[/]
       /raw                     - ローモードを切り替える（ChatGPTの応答の生のテキストを表示する）
```

### Comparing `gpt-term-1.1.4/gpt_term/locale/gpt_term.zh_CN.yml` & `gpt-term-1.2.0/gpt_term/locale/gpt_term.zh_CN.yml`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
   help_set_host: "设置API Host地址（这通常被用来配置代理）"
   help_set_key: "设置OpenAI的API密钥"
   help_set_timeout: "设置API请求的最大等待时间"
   help_set_gentitle: "设置是否自动生成聊天标题"
   help_set_lang: "设置语言"
   help_set_saveperfix: "设置聊天历史记录文件的保存前缀"
   help_set_loglevel: "设置日志级别: "
+  help_direct_query: "直接向GPT提问的内容"
   #
   help_use_help: "使用 `[deep_sky_blue3]/help[/]` 查看所有可用命令"
   help_uncommand: "无法识别命令 `[bold red]%{command}[/]`"
   help_mean_command: "您是否指的是 `[deep_sky_blue3]%{most_similar_command}[/]`?"
   help_text: |
     [bold]可用命令: [/]
       /raw                     - 切换原始模式 (显示 ChatGPT 回复的原始文本)
```

### Comparing `gpt-term-1.1.4/gpt_term/main.py` & `gpt-term-1.2.0/gpt_term/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,16 +156,14 @@
         except requests.exceptions.RequestException as e:
             console.print(_("gpt_term.Error_message",error_msg=str(e)))
             log.exception(e)
             return None
 
     def send_request_silent(self, data):
         # this is a silent sub function, for sending request without outputs (silently)
-        # it SHOULD NOT be triggered or used by not-silent functions
-        # it is only used by gen_title_silent now
         try:
             response = requests.post(
                 self.endpoint, headers=self.headers, data=json.dumps(data), timeout=self.timeout)
             # match 4xx error codes
             if response.status_code // 100 == 4:
                 error_msg = response.json()['error']['message']
                 log.error(error_msg)
@@ -239,14 +237,27 @@
         del self.messages[1:]
         self.title = None
         # recount current tokens
         self.current_tokens = count_token(self.messages)
         os.system('cls' if os.name == 'nt' else 'clear')
         console.print(_('gpt_term.delete_all'))
 
+    def handle_simple(self, message: str):
+        self.messages.append({"role": "user", "content": message})
+        data = {
+            "model": self.model,
+            "messages": self.messages,
+            "temperature": self.temperature
+        }
+        response = self.send_request_silent(data)
+        if response:
+            response_json = response.json()
+            log.debug(f"Response: {response_json}")
+            print(response_json["choices"][0]["message"]["content"])
+
     def handle(self, message: str):
         try:
             self.messages.append({"role": "user", "content": message})
             data = {
                 "model": self.model,
                 "messages": self.messages,
                 "stream": ChatMode.stream_mode,
@@ -1066,14 +1077,16 @@
     parser.add_argument('--set-apikey', metavar='KEY', type=str, help=_("gpt_term.help_set_key"))
     parser.add_argument('--set-timeout', metavar='SEC', type=int, help=_("gpt_term.help_set_timeout"))
     parser.add_argument('--set-gentitle', metavar='BOOL', type=str, help=_("gpt_term.help_set_gentitle"))
     ## 新添加的选项：--set-lang
     parser.add_argument('--set-lang', type=str, choices=['en', 'zh_CN', 'jp', 'de'], help=_("gpt_term.help_set_lang"))
     parser.add_argument('--set-saveperfix', metavar='PERFIX', type=str, help=_("gpt_term.help_set_saveperfix"))
     parser.add_argument('--set-loglevel', metavar='LEVEL', type=str, help=_("gpt_term.help_set_loglevel")+'DEBUG, INFO, WARNING, ERROR, CRITICAL')
+    # Query without parameter
+    parser.add_argument("query", nargs="*", help=_("gpt_term.help_direct_query"))
     # setting args
     args = parser.parse_args()
 
     set_config_by_args(args, config_ini)
 
     if args.lang:
         _=set_lang(args.lang)
@@ -1111,16 +1124,14 @@
         if confirm(_("gpt_term.save_api_key"), suffix=" (y/N) "):
             config["OPENAI_API_KEY"] = api_key
             write_config(config_ini)
 
     api_key_log = api_key[:3] + '*' * (len(api_key) - 7) + api_key[-4:]
     log.debug(f"Loaded API Key: {api_key_log}")
 
-    console.print(_("gpt_term.welcome"))
-
     api_timeout = config.getfloat("OPENAI_API_TIMEOUT", 30)
     log.debug(f"API Timeout set to {api_timeout}")
 
     chat_save_perfix = config.get("CHAT_SAVE_PERFIX", "./chat_history_")
 
     chat_gpt = ChatGPT(api_key, api_timeout)
     
@@ -1156,14 +1167,26 @@
             chat_gpt.messages = chat_history
             for message in chat_gpt.messages:
                 print_message(message)
             chat_gpt.current_tokens = count_token(chat_gpt.messages)
             log.info(f"Chat history successfully loaded from: {args.load}")
             console.print(
                 _("gpt_term.load_chat_history",load=args.load), highlight=False)
+            
+    if args.query:
+        query_text = " ".join(args.query)
+        log.info(f"> {query_text}")
+        is_stdout_tty = os.isatty(sys.stdout.fileno())
+        if is_stdout_tty:
+            chat_gpt.handle(query_text)
+        else:  # Running in pipe/stream mode
+            chat_gpt.handle_simple(query_text)
+        return
+    else:
+        console.print(_("gpt_term.welcome"))
 
     session = PromptSession()
 
     # 绑定回车事件，达到自定义多行模式的效果
     key_bindings = create_key_bindings()
 
     while True:
```

### Comparing `gpt-term-1.1.4/gpt_term.egg-info/PKG-INFO` & `gpt-term-1.2.0/gpt_term.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-term
-Version: 1.1.4
+Version: 1.2.0
 Summary: Chat with GPT in Terminal
 Author: xiaoxx970, Ace-Radom
 License: MIT License
         
         Copyright (c) 2023 xiaoxx970
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,36 +59,51 @@
 
 [GPTerm implemented in C/C++](https://github.com/Ace-Radom/cGPTerm) by @Ace-Radom
 
 [gpt-term that can call POE API](https://github.com/Lemon-2333/chatgpt-in-terminal-Poe-Api) by @Lemon-2333
 
 ## Changelog
 
-### 2023-05-20
+### 2023-06-21
 
-- Added host configuration support, which is very useful when using self-built API reverse proxy server ([#49](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/49)), you can now use `gpt-term --set-host HOST` to configure host, the default is https://api.openai.com
+- Added direct query mode, now you can run `gpt-term` with the content of the question as a parameter to conduct a single question and answer
 
-### 2023-05-18
+  ```sh
+  gpt-term "What's the weather like today?"
+  ```
 
-- Added multi-language support: English, Chinese, Japanese, German, follow the system language by default, now you can use `/lang` to switch languages
+  The answer will be printed directly, or piped into a variable
+
+  ```sh
+  gpt-term "What's the weather like today" | read answer
+  echo $answer
+  ```
 
 <details>
   <summary>More Change log</summary>
 
+### 2023-05-20
+
+- Added host configuration support, which is very useful when using self-built API reverse proxy server ([#49](https://github.com/xiaoxx970/chatgpt-in-terminal/issues/49)), you can now use `gpt-term --set-host HOST` to configure host, the default is https://api.openai.com
+
+### 2023-05-18
+
+- Added multi-language support: English, Chinese, Japanese, German, follow the system language by default, now you can use `/lang` to switch languages
 ### 2023-05-11
 
 - Find the command the user most likely intended to enter when typing an unrecognized command
 
 ### 2023-05-05
 
 - Add `/rand` command to set temperature parameter
 
 - Add overflow mode switch for `/stream` command, now you can run command `/stream visible` to switch to always visible mode. In this mode, the content that exceeds the screen will be scrolled up, and the new content will be output until it is completed
 
 ### 2023-04-23
+
 Released `gpt-term` on [Pypi](https://pypi.org/project/gpt-term/), started version control. No need to clone the project locally anymore, simply use the `pip` command to install gpt-term.
 
 ### 2023-04-15
 
 - Added the ability to create a line break in single-line mode using `Esc` + `Enter`
 
 ### 2023-04-13
@@ -175,14 +190,20 @@
 
 Or:
 
 ```shell
 python3 -m gpt_term
 ```
 
+Quick query:
+
+```sh
+gpt-term "What's the weather like today?"
+```
+
 When entering a question in single-line mode, use `Esc` + `Enter` to start a new line, and use `Enter` to submit the question.
 
 Here are some common shortcut keys (also shortcut keys for the shell):
 
 - `Ctrl+_`:	Undo
 - `Ctrl+L`: Clear screen, equivalent to `clear` command in shell
 - `Ctrl+C`: Stop the current answer or cancel the current input
```

### Comparing `gpt-term-1.1.4/gpt_term.egg-info/SOURCES.txt` & `gpt-term-1.2.0/gpt_term.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-term-1.1.4/pyproject.toml` & `gpt-term-1.2.0/pyproject.toml`

 * *Files identical despite different names*

