# Comparing `tmp/gpt-engineer-0.0.3.tar.gz` & `tmp/gpt-engineer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-engineer-0.0.3.tar", last modified: Sun Jun 18 21:33:56 2023, max compression
+gzip compressed data, was "gpt-engineer-0.0.4.tar", last modified: Tue Jun 20 23:17:14 2023, max compression
```

## Comparing `gpt-engineer-0.0.3.tar` & `gpt-engineer-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:33:56.704646 gpt-engineer-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-18 21:33:56.704646 gpt-engineer-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:33:56.700646 gpt-engineer-0.0.3/gpt_engineer/
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/gpt_engineer/ai.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/gpt_engineer/chat_to_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/gpt_engineer/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/gpt_engineer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/gpt_engineer/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:33:56.704646 gpt-engineer-0.0.3/gpt_engineer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-18 21:33:56.000000 gpt-engineer-0.0.3/gpt_engineer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-18 21:33:56.000000 gpt-engineer-0.0.3/gpt_engineer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:33:56.000000 gpt-engineer-0.0.3/gpt_engineer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-18 21:33:56.000000 gpt-engineer-0.0.3/gpt_engineer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-18 21:33:56.000000 gpt-engineer-0.0.3/gpt_engineer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 21:33:56.000000 gpt-engineer-0.0.3/gpt_engineer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 21:33:56.704646 gpt-engineer-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:33:56.704646 gpt-engineer-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/tests/test_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/tests/test_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:17:14.941167 gpt-engineer-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-20 23:17:14.941167 gpt-engineer-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:17:14.941167 gpt-engineer-0.0.4/gpt_engineer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/gpt_engineer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/gpt_engineer/ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/gpt_engineer/chat_to_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/gpt_engineer/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/gpt_engineer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/gpt_engineer/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:17:14.941167 gpt-engineer-0.0.4/gpt_engineer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-20 23:17:14.000000 gpt-engineer-0.0.4/gpt_engineer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-20 23:17:14.000000 gpt-engineer-0.0.4/gpt_engineer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:17:14.000000 gpt-engineer-0.0.4/gpt_engineer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 23:17:14.000000 gpt-engineer-0.0.4/gpt_engineer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 23:17:14.000000 gpt-engineer-0.0.4/gpt_engineer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 23:17:14.000000 gpt-engineer-0.0.4/gpt_engineer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:17:14.941167 gpt-engineer-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:17:14.941167 gpt-engineer-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/tests/test_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/tests/test_chat_to_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/tests/test_db.py
```

### Comparing `gpt-engineer-0.0.3/LICENSE` & `gpt-engineer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.3/PKG-INFO` & `gpt-engineer-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: gpt-engineer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Specify what you want it to build, the AI asks for clarification, and then builds it.
 Project-URL: Homepage, https://github.com/AntonOsika/gpt-engineer
 Project-URL: Bug Tracker, https://github.com/AntonOsika/gpt-engineer/issues
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPT Engineer
+[![Discord Follow](https://dcbadge.vercel.app/api/server/4t5vXHhu?style=flat)](https://discord.gg/4t5vXHhu)
+[![GitHub Repo stars](https://img.shields.io/github/stars/AntonOsika/gpt-engineer?style=social)](https://github.com/AntonOsika/gpt-engineer)
+[![Twitter Follow](https://img.shields.io/twitter/follow/antonosika?style=social)](https://twitter.com/AntonOsika)
+
+
 **Specify what you want it to build, the AI asks for clarification, and then builds it.**
 
 GPT Engineer is made to be easy to adapt, extend, and make your agent learn how you want your code to look. It generates an entire codebase based on a prompt.
 
 [Demo](https://twitter.com/antonosika/status/1667641038104674306) 👶🤖
 
 ## Project philosophy
@@ -50,27 +55,26 @@
   - `cp -r projects/example/ projects/my-new-project`
 - Fill in the `main_prompt` file in your new folder
 - Run: `gpt-engineer projects/my-new-project`
 
 **Results**
 - Check the generated files in `projects/my-new-project/workspace`
 
-### Limitations
-Implementing additional chain of thought prompting, e.g. [Reflexion](https://github.com/noahshinn024/reflexion), should be able to make it more reliable and not miss requested functionality in the main prompt.
-
-Contributors welcome! If you are unsure what to add, check out the ideas listed in the Projects tab in the GitHub repo.
-
 
 ## Features
 You can specify the "identity" of the AI agent by editing the files in the `identity` folder.
 
 Editing the identity, and evolving the `main_prompt`, is currently how you make the agent remember things between projects.
 
 Each step in `steps.py` will have its communication history with GPT4 stored in the logs folder, and can be rerun with `scripts/rerun_edited_message_logs.py`.
 
 ## Contributing
-If you want to contribute, please check out the [projects](https://github.com/AntonOsika/gpt-engineer/projects?query=is%3Aopen) or [issues tab](https://github.com/AntonOsika/gpt-engineer/issues) in the GitHub repo and please read the [contributing document](.github/CONTRIBUTING.md) on how to contribute.
+We are building the open platform for devs to tinker with and build their personal code-generation toolbox.
+
+If you want to contribute, please check out the [roadmap](https://github.com/AntonOsika/gpt-engineer/blob/main/ROADMAP.md), [projects](https://github.com/AntonOsika/gpt-engineer/projects?query=is%3Aopen) or [issues tab](https://github.com/AntonOsika/gpt-engineer/issues) in the GitHub repo. You are welcome to read the [contributing document](.github/CONTRIBUTING.md) and join our [Discord 💬](https://discord.gg/4t5vXHhu).
+
+We are currently looking for more maintainers and community organisers. Email anton.osika@gmail.com if you are interested in an official role.
 
 
-## High resolution example
+## Example
 
 https://github.com/AntonOsika/gpt-engineer/assets/4467025/6e362e45-4a94-4b0d-973d-393a31d92d9b
```

### Comparing `gpt-engineer-0.0.3/README.md` & `gpt-engineer-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 # GPT Engineer
+[![Discord Follow](https://dcbadge.vercel.app/api/server/4t5vXHhu?style=flat)](https://discord.gg/4t5vXHhu)
+[![GitHub Repo stars](https://img.shields.io/github/stars/AntonOsika/gpt-engineer?style=social)](https://github.com/AntonOsika/gpt-engineer)
+[![Twitter Follow](https://img.shields.io/twitter/follow/antonosika?style=social)](https://twitter.com/AntonOsika)
+
+
 **Specify what you want it to build, the AI asks for clarification, and then builds it.**
 
 GPT Engineer is made to be easy to adapt, extend, and make your agent learn how you want your code to look. It generates an entire codebase based on a prompt.
 
 [Demo](https://twitter.com/antonosika/status/1667641038104674306) 👶🤖
 
 ## Project philosophy
@@ -40,27 +45,26 @@
   - `cp -r projects/example/ projects/my-new-project`
 - Fill in the `main_prompt` file in your new folder
 - Run: `gpt-engineer projects/my-new-project`
 
 **Results**
 - Check the generated files in `projects/my-new-project/workspace`
 
-### Limitations
-Implementing additional chain of thought prompting, e.g. [Reflexion](https://github.com/noahshinn024/reflexion), should be able to make it more reliable and not miss requested functionality in the main prompt.
-
-Contributors welcome! If you are unsure what to add, check out the ideas listed in the Projects tab in the GitHub repo.
-
 
 ## Features
 You can specify the "identity" of the AI agent by editing the files in the `identity` folder.
 
 Editing the identity, and evolving the `main_prompt`, is currently how you make the agent remember things between projects.
 
 Each step in `steps.py` will have its communication history with GPT4 stored in the logs folder, and can be rerun with `scripts/rerun_edited_message_logs.py`.
 
 ## Contributing
-If you want to contribute, please check out the [projects](https://github.com/AntonOsika/gpt-engineer/projects?query=is%3Aopen) or [issues tab](https://github.com/AntonOsika/gpt-engineer/issues) in the GitHub repo and please read the [contributing document](.github/CONTRIBUTING.md) on how to contribute.
+We are building the open platform for devs to tinker with and build their personal code-generation toolbox.
+
+If you want to contribute, please check out the [roadmap](https://github.com/AntonOsika/gpt-engineer/blob/main/ROADMAP.md), [projects](https://github.com/AntonOsika/gpt-engineer/projects?query=is%3Aopen) or [issues tab](https://github.com/AntonOsika/gpt-engineer/issues) in the GitHub repo. You are welcome to read the [contributing document](.github/CONTRIBUTING.md) and join our [Discord 💬](https://discord.gg/4t5vXHhu).
+
+We are currently looking for more maintainers and community organisers. Email anton.osika@gmail.com if you are interested in an official role.
 
 
-## High resolution example
+## Example
 
 https://github.com/AntonOsika/gpt-engineer/assets/4467025/6e362e45-4a94-4b0d-973d-393a31d92d9b
```

### Comparing `gpt-engineer-0.0.3/gpt_engineer/ai.py` & `gpt-engineer-0.0.4/gpt_engineer/ai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 
 import openai
 
 logger = logging.getLogger(__name__)
 
 
@@ -35,15 +37,15 @@
         return {"role": "user", "content": msg}
 
     def fassistant(self, msg):
         return {"role": "assistant", "content": msg}
 
     def next(self, messages: list[dict[str, str]], prompt=None):
         if prompt:
-            messages = messages + [{"role": "user", "content": prompt}]
+            messages += [{"role": "user", "content": prompt}]
 
         logger.debug(f"Creating a new chat completion: {messages}")
         response = openai.ChatCompletion.create(
             messages=messages,
             stream=True,
             model=self.model,
             temperature=self.temperature,
@@ -52,10 +54,10 @@
         chat = []
         for chunk in response:
             delta = chunk["choices"][0]["delta"]
             msg = delta.get("content", "")
             print(msg, end="")
             chat.append(msg)
         print()
-        messages = messages + [{"role": "assistant", "content": "".join(chat)}]
+        messages += [{"role": "assistant", "content": "".join(chat)}]
         logger.debug(f"Chat completion finished: {messages}")
         return messages
```

### Comparing `gpt-engineer-0.0.3/gpt_engineer/chat_to_files.py` & `gpt-engineer-0.0.4/gpt_engineer/chat_to_files.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 import re
 
 
 def parse_chat(chat):  # -> List[Tuple[str, str]]:
     # Get all ``` blocks and preceding filenames
-    regex = r"(\S+?)\n```\S+\n(.+?)```"
+    regex = r"(\S+)\n\s*```[^\n]*\n(.+?)```"
     matches = re.finditer(regex, chat, re.DOTALL)
 
     files = []
     for match in matches:
         # Strip the filename of any non-allowed characters and convert / to \
         path = re.sub(r'[<>"|?*]', "", match.group(1))
 
+        # Remove leading and trailing brackets
+        path = re.sub(r"^\[(.*)\]$", r"\1", path)
+
+        # Remove leading and trailing backticks
+        path = re.sub(r"^`(.*)`$", r"\1", path)
+
+        # Remove trailing ]
+        path = re.sub(r"\]$", "", path)
+
         # Get the code
         code = match.group(2)
 
         # Add the file to the list
         files.append((path, code))
 
     # Get all the text before the first ``` block
```

### Comparing `gpt-engineer-0.0.3/gpt_engineer/db.py` & `gpt-engineer-0.0.4/gpt_engineer/db.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,18 @@
         self.path = Path(path).absolute()
 
         self.path.mkdir(parents=True, exist_ok=True)
 
     def __getitem__(self, key):
         full_path = self.path / key
 
-        if full_path.is_file():
-            with full_path.open("r", encoding="utf-8") as f:
-                return f.read()
-        else:
+        if not full_path.is_file():
             raise KeyError(key)
+        with full_path.open("r", encoding="utf-8") as f:
+            return f.read()
 
     def __setitem__(self, key, val):
         full_path = self.path / key
         full_path.parent.mkdir(parents=True, exist_ok=True)
 
         if isinstance(val, str):
             full_path.write_text(val, encoding="utf-8")
```

### Comparing `gpt-engineer-0.0.3/gpt_engineer/main.py` & `gpt-engineer-0.0.4/gpt_engineer/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,42 +3,45 @@
 import os
 import shutil
 
 from pathlib import Path
 
 import typer
 
+from gpt_engineer import steps
 from gpt_engineer.ai import AI
 from gpt_engineer.db import DB, DBs
 from gpt_engineer.steps import STEPS
 
 app = typer.Typer()
 
 
 @app.command()
 def main(
     project_path: str = typer.Argument("example", help="path"),
     delete_existing: bool = typer.Argument(False, help="delete existing files"),
     model: str = "gpt-4",
     temperature: float = 0.1,
-    steps_config: str = "default",
+    steps_config: steps.Config = typer.Option(
+        steps.Config.DEFAULT, "--steps", "-s", help="decide which steps to run"
+    ),
     verbose: bool = typer.Option(False, "--verbose", "-v"),
     run_prefix: str = typer.Option(
         "",
         help=(
             "run prefix, if you want to run multiple variants of the same project and "
             "later compare them"
         ),
     ),
 ):
     logging.basicConfig(level=logging.DEBUG if verbose else logging.INFO)
 
     input_path = Path(project_path).absolute()
-    memory_path = input_path / (run_prefix + "memory")
-    workspace_path = input_path / (run_prefix + "workspace")
+    memory_path = input_path / f"{run_prefix}memory"
+    workspace_path = input_path / f"{run_prefix}workspace"
 
     if delete_existing:
         # Delete files and subdirectories in paths
         shutil.rmtree(memory_path, ignore_errors=True)
         shutil.rmtree(workspace_path, ignore_errors=True)
 
     ai = AI(
```

### Comparing `gpt-engineer-0.0.3/gpt_engineer/steps.py` & `gpt-engineer-0.0.4/gpt_engineer/steps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
 import re
 import subprocess
 
+from enum import Enum
+
 from gpt_engineer.ai import AI
 from gpt_engineer.chat_to_files import to_files
 from gpt_engineer.db import DBs
 
 
 def setup_sys_prompt(dbs):
     return dbs.identity["generate"] + "\nUseful to know:\n" + dbs.identity["philosophy"]
@@ -30,18 +32,18 @@
     while True:
         messages = ai.next(messages, user)
 
         if messages[-1]["content"].strip().lower().startswith("no"):
             break
 
         print()
-        user = input('(answer in text, or "q" to move on)\n')
+        user = input('(answer in text, or "c" to move on)\n')
         print()
 
-        if not user or user == "q":
+        if not user or user == "c":
             break
 
         user += (
             "\n\n"
             "Is anything else unclear? If yes, only answer in the form:\n"
             "{remaining unclear areas} remaining questions.\n"
             "{Next question}\n"
@@ -66,15 +68,15 @@
 
     dbs.memory["specification"] = messages[-1]["content"]
 
     return messages
 
 
 def respec(ai: AI, dbs: DBs):
-    messages = dbs.logs[gen_spec.__name__]
+    messages = json.loads(dbs.logs[gen_spec.__name__])
     messages += [ai.fsystem(dbs.identity["respec"])]
 
     messages = ai.next(messages)
     messages = ai.next(
         messages,
         (
             "Based on the conversation so far, please reiterate the specification for "
@@ -141,18 +143,24 @@
 
     print("Do you want to execute this code?")
     print()
     print(command)
     print()
     print('If yes, press enter. Otherwise, type "no"')
     print()
-    if input() != "":
+    if input() not in ["", "y", "yes"]:
         print("Ok, not executing the code.")
         return []
     print("Executing the code...")
+    print(
+        "\033[92m"  # green color
+        + "Note: If it does not work as expected, please consider running the code'"
+        + " in another way than above."
+        + "\033[0m"
+    )
     print()
     subprocess.run("bash run.sh", shell=True, cwd=dbs.workspace.path)
     return []
 
 
 def gen_entrypoint(ai, dbs):
     messages = ai.start(
@@ -161,14 +169,16 @@
             "the current folder.\n"
             "From this you will answer with code blocks that includes all the necessary "
             "unix terminal commands to "
             "a) install dependencies "
             "b) run all necessary parts of the codebase (in parallell if necessary).\n"
             "Do not install globally. Do not use sudo.\n"
             "Do not explain the code, just give the commands.\n"
+            "Do not use placeholders, use example values (like . for a folder argument) "
+            "if necessary.\n"
         ),
         user="Information about the codebase:\n\n" + dbs.workspace["all_output.txt"],
     )
     print()
 
     regex = r"```\S*\n(.+?)```"
     matches = re.finditer(regex, messages[-1]["content"], re.DOTALL)
@@ -179,15 +189,15 @@
 def use_feedback(ai: AI, dbs: DBs):
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
         ai.fuser(f"Instructions: {dbs.input['main_prompt']}"),
         ai.fassistant(dbs.workspace["all_output.txt"]),
         ai.fsystem(dbs.identity["use_feedback"]),
     ]
-    messages = ai.next(messages, dbs.memory["feedback"])
+    messages = ai.next(messages, dbs.input["feedback"])
     to_files(messages[-1]["content"], dbs.workspace)
     return messages
 
 
 def fix_code(ai: AI, dbs: DBs):
     code_ouput = json.loads(dbs.logs[gen_code.__name__])[-1]["content"]
     messages = [
@@ -197,30 +207,65 @@
         ai.fsystem(dbs.identity["fix_code"]),
     ]
     messages = ai.next(messages, "Please fix any errors in the code above.")
     to_files(messages[-1]["content"], dbs.workspace)
     return messages
 
 
+class Config(str, Enum):
+    DEFAULT = "default"
+    BENCHMARK = "benchmark"
+    SIMPLE = "simple"
+    TDD = "tdd"
+    TDD_PLUS = "tdd+"
+    CLARIFY = "clarify"
+    RESPEC = "respec"
+    EXECUTE_ONLY = "execute_only"
+    USE_FEEDBACK = "use_feedback"
+
+
 # Different configs of what steps to run
 STEPS = {
-    "default": [gen_spec, gen_unit_tests, gen_code, gen_entrypoint, execute_entrypoint],
-    "benchmark": [gen_spec, gen_unit_tests, gen_code, fix_code, gen_entrypoint],
-    "simple": [simple_gen, gen_entrypoint, execute_entrypoint],
-    "clarify": [clarify, gen_clarified_code, gen_entrypoint, execute_entrypoint],
-    "respec": [
+    Config.DEFAULT: [
+        clarify,
+        gen_clarified_code,
+        gen_entrypoint,
+        execute_entrypoint,
+    ],
+    Config.BENCHMARK: [simple_gen, gen_entrypoint],
+    Config.SIMPLE: [simple_gen, gen_entrypoint, execute_entrypoint],
+    Config.TDD: [
+        gen_spec,
+        gen_unit_tests,
+        gen_code,
+        gen_entrypoint,
+        execute_entrypoint,
+    ],
+    Config.TDD_PLUS: [
+        gen_spec,
+        gen_unit_tests,
+        gen_code,
+        fix_code,
+        gen_entrypoint,
+        execute_entrypoint,
+    ],
+    Config.CLARIFY: [
+        clarify,
+        gen_clarified_code,
+        gen_entrypoint,
+        execute_entrypoint,
+    ],
+    Config.RESPEC: [
         gen_spec,
         respec,
         gen_unit_tests,
         gen_code,
         gen_entrypoint,
         execute_entrypoint,
     ],
-    "execute_only": [execute_entrypoint],
-    "use_feedback": [use_feedback],
+    Config.USE_FEEDBACK: [use_feedback, gen_entrypoint, execute_entrypoint],
+    Config.EXECUTE_ONLY: [gen_entrypoint, execute_entrypoint],
 }
 
 # Future steps that can be added:
-# self_reflect_and_improve_files,
-# add_tests
-# run_tests_and_fix_files,
-# improve_based_on_in_file_feedback_comments
+# run_tests_and_fix_files
+# execute_entrypoint_and_fix_files_if_needed
```

### Comparing `gpt-engineer-0.0.3/gpt_engineer.egg-info/PKG-INFO` & `gpt-engineer-0.0.4/gpt_engineer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: gpt-engineer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Specify what you want it to build, the AI asks for clarification, and then builds it.
 Project-URL: Homepage, https://github.com/AntonOsika/gpt-engineer
 Project-URL: Bug Tracker, https://github.com/AntonOsika/gpt-engineer/issues
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPT Engineer
+[![Discord Follow](https://dcbadge.vercel.app/api/server/4t5vXHhu?style=flat)](https://discord.gg/4t5vXHhu)
+[![GitHub Repo stars](https://img.shields.io/github/stars/AntonOsika/gpt-engineer?style=social)](https://github.com/AntonOsika/gpt-engineer)
+[![Twitter Follow](https://img.shields.io/twitter/follow/antonosika?style=social)](https://twitter.com/AntonOsika)
+
+
 **Specify what you want it to build, the AI asks for clarification, and then builds it.**
 
 GPT Engineer is made to be easy to adapt, extend, and make your agent learn how you want your code to look. It generates an entire codebase based on a prompt.
 
 [Demo](https://twitter.com/antonosika/status/1667641038104674306) 👶🤖
 
 ## Project philosophy
@@ -50,27 +55,26 @@
   - `cp -r projects/example/ projects/my-new-project`
 - Fill in the `main_prompt` file in your new folder
 - Run: `gpt-engineer projects/my-new-project`
 
 **Results**
 - Check the generated files in `projects/my-new-project/workspace`
 
-### Limitations
-Implementing additional chain of thought prompting, e.g. [Reflexion](https://github.com/noahshinn024/reflexion), should be able to make it more reliable and not miss requested functionality in the main prompt.
-
-Contributors welcome! If you are unsure what to add, check out the ideas listed in the Projects tab in the GitHub repo.
-
 
 ## Features
 You can specify the "identity" of the AI agent by editing the files in the `identity` folder.
 
 Editing the identity, and evolving the `main_prompt`, is currently how you make the agent remember things between projects.
 
 Each step in `steps.py` will have its communication history with GPT4 stored in the logs folder, and can be rerun with `scripts/rerun_edited_message_logs.py`.
 
 ## Contributing
-If you want to contribute, please check out the [projects](https://github.com/AntonOsika/gpt-engineer/projects?query=is%3Aopen) or [issues tab](https://github.com/AntonOsika/gpt-engineer/issues) in the GitHub repo and please read the [contributing document](.github/CONTRIBUTING.md) on how to contribute.
+We are building the open platform for devs to tinker with and build their personal code-generation toolbox.
+
+If you want to contribute, please check out the [roadmap](https://github.com/AntonOsika/gpt-engineer/blob/main/ROADMAP.md), [projects](https://github.com/AntonOsika/gpt-engineer/projects?query=is%3Aopen) or [issues tab](https://github.com/AntonOsika/gpt-engineer/issues) in the GitHub repo. You are welcome to read the [contributing document](.github/CONTRIBUTING.md) and join our [Discord 💬](https://discord.gg/4t5vXHhu).
+
+We are currently looking for more maintainers and community organisers. Email anton.osika@gmail.com if you are interested in an official role.
 
 
-## High resolution example
+## Example
 
 https://github.com/AntonOsika/gpt-engineer/assets/4467025/6e362e45-4a94-4b0d-973d-393a31d92d9b
```

### Comparing `gpt-engineer-0.0.3/pyproject.toml` & `gpt-engineer-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "gpt-engineer"
-version = "0.0.3"
+version = "0.0.4"
 description = "Specify what you want it to build, the AI asks for clarification, and then builds it."
 readme = "README.md"
 requires-python = ">=3"
 dependencies = [
   'black == 23.3.0',
+  'mypy == 1.3.0',
   'openai == 0.27.8',
+  'pre-commit == 3.3.3',
+  'pytest == 7.3.1',
   'ruff == 0.0.272',
-  'typer == 0.9.0'
+  'termcolor==2.3.0',
+  'typer == 0.9.0',
 ]
 
 [project.scripts]
 gpt-engineer = 'gpt_engineer.main:app'
 
 [tool.setuptools]
 packages = ["gpt_engineer"]
```

