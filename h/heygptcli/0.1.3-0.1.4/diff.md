# Comparing `tmp/heygptcli-0.1.3.tar.gz` & `tmp/heygptcli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heygptcli-0.1.3.tar", max compression
+gzip compressed data, was "heygptcli-0.1.4.tar", max compression
```

## Comparing `heygptcli-0.1.3.tar` & `heygptcli-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       87 2023-06-20 17:30:39.875805 heygptcli-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-20 17:30:39.875805 heygptcli-0.1.3/heygpt/__init__.py
--rw-r--r--   0        0        0      717 2023-06-20 17:30:39.875805 heygptcli-0.1.3/heygpt/api.py
--rwxr-xr-x   0        0        0     5048 2023-06-20 17:30:39.879805 heygptcli-0.1.3/heygpt/cli.py
--rw-r--r--   0        0        0     2249 2023-06-20 17:30:39.879805 heygptcli-0.1.3/heygpt/constant.py
--rw-r--r--   0        0        0     3440 2023-06-20 17:30:39.879805 heygptcli-0.1.3/heygpt/core.py
--rw-r--r--   0        0        0     1897 2023-06-20 17:30:39.879805 heygptcli-0.1.3/heygpt/serve.py
--rw-r--r--   0        0        0      153 2023-06-20 17:30:39.879805 heygptcli-0.1.3/heygpt/serve_prompts.py
--rw-r--r--   0        0        0      849 2023-06-20 17:30:39.879805 heygptcli-0.1.3/heygpt/utils.py
--rw-r--r--   0        0        0      677 2023-06-20 17:30:39.879805 heygptcli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 heygptcli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-21 13:32:50.445042 heygptcli-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/__init__.py
+-rw-r--r--   0        0        0      774 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/api.py
+-rwxr-xr-x   0        0        0     5292 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/cli.py
+-rw-r--r--   0        0        0     2249 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/constant.py
+-rw-r--r--   0        0        0     3519 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/core.py
+-rw-r--r--   0        0        0     1984 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/serve.py
+-rw-r--r--   0        0        0      153 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/serve_prompts.py
+-rw-r--r--   0        0        0      849 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/utils.py
+-rw-r--r--   0        0        0      677 2023-06-21 13:32:50.445042 heygptcli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 heygptcli-0.1.4/PKG-INFO
```

### Comparing `heygptcli-0.1.3/heygpt/api.py` & `heygptcli-0.1.4/heygpt/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,18 @@
     allow_credentials=True,
     allow_methods=["GET", "POST", "PUT", "DELETE"],
     allow_headers=["*"],
 )
 
 
 @app.post("/gpt")
-async def gpt(msg: PromptInput):
-    return completion_openai_gpt(command=msg.prompt.Command, text=f"""{msg.text}""")
+async def gpt(msg: PromptInput, model: str = "gpt-3.5-turbo"):
+    return completion_openai_gpt(
+        command=msg.prompt.Command, text=f"""{msg.text}""", model=model
+    )
 
 
 @app.get("/prompt-items")
 async def prompt_items():
     return prompts
```

### Comparing `heygptcli-0.1.3/heygpt/cli.py` & `heygptcli-0.1.4/heygpt/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     wisper,
     print_md,
     ask_prompt_input,
 )
 
 app = typer.Typer(
     help="""
-HeyGPT CLI\n\nA simple command line tool to generate text using OpenAI GPT-3 or Bard base on ready made templated promts.
+HeyGPT CLI\n\nA simple command line tool to generate text using OpenAI GPT or Bard base on ready made templated promts.
 \n\n\nFor debug logs use: `export LOG_LEVEL=DEBUG` or `set LOG_LEVEL=DEBUG` on windows."""
 )
 
 
 @app.command(help="Ask query or task to gpt using prompt templates")
 def ask(
     bard: bool = typer.Option(
@@ -44,15 +44,21 @@
     save: str = typer.Option(
         "", "--output", "-o", help="save output to file availabe formats: md"
     ),
     model: str = typer.Option(
         openai_model,
         "--model",
         "-m",
-        help="OpenAI model name. info: https://platform.openai.com/docs/models/gpt-3",
+        help="OpenAI model name. info: https://platform.openai.com/docs/models/",
+    ),
+    temperature: float = typer.Option(
+        0.5,
+        "--temperature",
+        "-t",
+        help="temperature value for openai, more temperature more randomness",
     ),
 ):
     tags: str = " #".join(tag)
     command: str = ""
 
     # print(tags)
     # return
@@ -94,15 +100,19 @@
         text = Prompt.ask("[blue]Enter text")
 
     # log.debug(text)
     if bard:
         content = completion_bard(command=command, text=text, _print=True)
     else:
         completion = completion_openai_gpt(
-            command=command, text=text, model=model, _print=True
+            command=command,
+            text=text,
+            model=model,
+            _print=True,
+            temperature=temperature,
         )
         content = completion
 
     # typer.echo("\n---------- output ----------\n")
 
     if save != "":
         with open(f"{save}", "w") as f:
```

### Comparing `heygptcli-0.1.3/heygpt/constant.py` & `heygptcli-0.1.4/heygpt/constant.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.3/heygpt/core.py` & `heygptcli-0.1.4/heygpt/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 def ask_prompt_input(items: list, title="Select item"):
     completer = FuzzyWordCompleter(items)
     text = prompt(f"{title}: ", completer=completer, complete_while_typing=True)
     return text
 
 
 def completion_openai_gpt(
-    text: str = None, command: str = "", model=openai_model, _print=False
+    text: str = None,
+    command: str = "",
+    model=openai_model,
+    _print=False,
+    temperature=0.7,
 ):
     """
     ref: https://docs.openai.com/api-reference/completions/create
     """
     out = ""
     log.debug(f"model: {model}")
 
@@ -48,14 +52,15 @@
     else:
         _command = text
 
     if "gpt-3" in model:
         completion = openai.ChatCompletion.create(
             model=model,
             stream=True,
+            temperature=temperature,
             messages=[
                 {
                     "role": "system",
                     "content": "Output has to be in markdown supported format",
                 },
                 {"role": "user", "content": _command},
             ],
@@ -68,15 +73,15 @@
             out += c
             if _print:
                 console.print(c, end="", markup=True)
     else:
         completion = openai.Completion.create(
             model=model,
             prompt=_command,
-            temperature=0.9,
+            temperature=temperature,
             max_tokens=1000,
             stream=True,
             top_p=1,
         )
         for chunk in completion:
             c = chunk["choices"][0]["text"]
             out += c
```

### Comparing `heygptcli-0.1.3/heygpt/serve.py` & `heygptcli-0.1.4/heygpt/serve.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 
 st.set_page_config(
     page_title="HeyGPT",
     page_icon=":shark:",
     layout="wide",
     initial_sidebar_state="collapsed",
 )
-st.write("<h5 style='text-align: center'>HeyGPT</h5><br>", unsafe_allow_html=True)
 
 col1, col2, col3 = st.columns([2, 5, 1])
 
 with st.container():
     col4, col5, col6 = st.columns([2, 5, 1])
-    with col5:
+    with col2:
         ask = st.text_area("**Input**:", height=80)
         print_prompt = st.empty()
-    with col6:
+    with col3:
         st.write("<br><br><br>", unsafe_allow_html=True)
         submit = st.button("Submit")
 
 
 with col1:
-    use_bard = st.checkbox("Ask Bard", value=False)
+    _options = {"GPT": "gpt-3.5-turbo", "Davinci": "text-davinci-003", "Bard": "bard"}
+    use_model = st.radio("**Model**", options=_options.keys())
     prompt = st.radio(
         label="**Promots**", options=["None"] + list(prompts_title.keys())
     )
 
 
 with st.container():
     content = ""
@@ -45,16 +45,18 @@
         if prompt != "None":
             _selected_prompt = prompts_title[prompt]
             print_prompt.write(f"**Selected**: {_selected_prompt}")
         else:
             _selected_prompt = ""
 
         if submit:
-            if not use_bard:
-                completion = completion_openai_gpt(command=_selected_prompt, text=ask)
+            if use_model != "Bard":
+                completion = completion_openai_gpt(
+                    command=_selected_prompt, text=ask, model=_options[use_model]
+                )
             else:
                 completion = completion_bard(command=_selected_prompt, text=ask)
             content = completion
             st.markdown(content)
 
     with col3:
         if content != "":
```

### Comparing `heygptcli-0.1.3/heygpt/utils.py` & `heygptcli-0.1.4/heygpt/utils.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.3/pyproject.toml` & `heygptcli-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heygptcli"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Rishang <rishang@localhost.com>"]
 readme = "README.md"
 packages = [
   { include = "heygpt" }
 ]
```

### Comparing `heygptcli-0.1.3/PKG-INFO` & `heygptcli-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heygptcli
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Rishang
 Author-email: rishang@localhost.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

