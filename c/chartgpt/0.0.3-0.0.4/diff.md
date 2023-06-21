# Comparing `tmp/chartgpt-0.0.3.tar.gz` & `tmp/chartgpt-0.0.4.tar.gz`

## Comparing `chartgpt-0.0.3.tar` & `chartgpt-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 chartgpt-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 chartgpt-0.0.3/mkdocs.yml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 chartgpt-0.0.3/requirements.txt
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 chartgpt-0.0.3/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 chartgpt-0.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/__init__.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/__main__.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/chartgpt.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/constants.py
--rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/llm.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/prompts/base.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 chartgpt-0.0.3/chartgpt/prompts/generate_python_code.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 chartgpt-0.0.3/docs/api-generated.md
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 chartgpt-0.0.3/docs/index.md
--rw-r--r--   0        0        0   925601 2020-02-02 00:00:00.000000 chartgpt-0.0.3/docs/assets/dash.png
--rw-r--r--   0        0        0   746570 2020-02-02 00:00:00.000000 chartgpt-0.0.3/docs/assets/notebook.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chartgpt-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 chartgpt-0.0.3/tests/test_run_code.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 chartgpt-0.0.3/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.3/LICENSE
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 chartgpt-0.0.3/README.md
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 chartgpt-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 chartgpt-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 chartgpt-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 chartgpt-0.0.4/mkdocs.yml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 chartgpt-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 chartgpt-0.0.4/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 chartgpt-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/__init__.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/__main__.py
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/chartgpt.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/constants.py
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/llm.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/prompts/base.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 chartgpt-0.0.4/chartgpt/prompts/generate_python_code.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 chartgpt-0.0.4/docs/api-generated.md
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 chartgpt-0.0.4/docs/index.md
+-rw-r--r--   0        0        0    80099 2020-02-02 00:00:00.000000 chartgpt-0.0.4/docs/assets/chart.png
+-rw-r--r--   0        0        0   925601 2020-02-02 00:00:00.000000 chartgpt-0.0.4/docs/assets/dash.png
+-rw-r--r--   0        0        0   746570 2020-02-02 00:00:00.000000 chartgpt-0.0.4/docs/assets/notebook.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chartgpt-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 chartgpt-0.0.4/tests/test_run_code.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 chartgpt-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 chartgpt-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 chartgpt-0.0.4/README.md
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 chartgpt-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 chartgpt-0.0.4/PKG-INFO
```

### Comparing `chartgpt-0.0.3/.pre-commit-config.yaml` & `chartgpt-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.3/mkdocs.yml` & `chartgpt-0.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.3/.devcontainer/devcontainer.json` & `chartgpt-0.0.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.3/.github/workflows/publish.yml` & `chartgpt-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.3/.github/workflows/test.yml` & `chartgpt-0.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.3/chartgpt/chartgpt.py` & `chartgpt-0.0.4/chartgpt/chartgpt.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             llm (Optional[str], optional): _description_. Defaults to "openai".
             conversational (bool, optional): _description_. Defaults to True.
             verbose (bool, optional): _description_. Defaults to False.
         """
         self.llm = LLM(api_key=api_key, **kwargs)
         self.fig = None
         self.last_run_code = None
+        self.variables_payload = {}
 
     def load(self, df: pd.DataFrame) -> None:
         """Load a DataFrame.
 
         Args:
             df (pd.DataFrame): A DataFrame.
 
@@ -42,44 +43,41 @@
         """
         self.df = df
         self.df_columns = df.columns
 
     def plot(
         self, prompt: str, show_code=False, debug=False, return_fig=False
     ) -> Figure:
-        """Run the model on a prompt.
+        """Generate a plot based on the prompt.
 
         Args:
             prompt (Optional[str]): _description_
             show_code (bool, optional): Print the code generated by the model. \
                 Defaults to False.
             debug (bool, optional): _description_. Defaults to False.
 
         Returns:
             str: _description_
         """
 
-        self._original_instructions = {
-            "question": prompt,
-            "df_columns": self.df_columns,
-        }
-
         if debug:
             code = """
-import plotly.express as px
+import plotly.graph_objects as go
 
-fig = px.bar(df, x="State", y="Population")
+fig = go.Figure
 fig"""
         else:
-            code = self.llm.generate_code(
-                GeneratePythonCodePrompt(
-                    df_columns=self.df_columns,
-                ),
-                prompt,
-            )
+            self.variables_payload = {
+                "question": prompt,
+                "df_columns": self.df_columns,
+                "user_prompt": prompt,
+            }
+            instructions = str(GeneratePythonCodePrompt(**self.variables_payload))
+
+            code = self.llm.generate_code(instructions)
 
         fig = self.run_code(
             code,
             self.df,
         )
 
         self.last_run_code = code
```

### Comparing `chartgpt-0.0.3/chartgpt/constants.py` & `chartgpt-0.0.4/chartgpt/constants.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.3/chartgpt/llm.py` & `chartgpt-0.0.4/chartgpt/llm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import re
 from typing import Any, Dict
 
 import openai
 
 from .constants import END_CODE_TAG, START_CODE_TAG
-from .prompts.base import Prompt
 
 
 class LLM:
     """LLM class for generating code from a prompt.
 
     Args:
         model_name (str, optional): Model name. Defaults to "text-davinci-003".
@@ -25,34 +24,38 @@
 
     Returns:
         str: Generated code
     """
 
     def __init__(
         self,
-        model_name: str = "text-davinci-003",
+        model_name: str = None,
         temperature: int = 0.2,
         max_tokens: int = 1000,
         top_p: int = 1,
         frequency_penalty: int = 0,
         presence_penalty: int = 0,
+        chat: bool = True,
         api_key: str = None,
     ):
-        self.model_name = model_name
+        self.model_name = model_name or "gpt-3.5-turbo" if chat else "text-davinci-003"
         self.temperature = temperature
         self.max_tokens = max_tokens
         self.top_p = top_p
         self.frequency_penalty = frequency_penalty
         self.presence_penalty = presence_penalty
+        self.chat = chat
 
         self.api_key = api_key or os.getenv("OPENAI_API_KEY") or None
         if self.api_key is None:
             raise ValueError("Please provide an OpenAI API key")
         openai.api_key = self.api_key
 
+        self.messages = []
+
     def _extract_code(self, response: str, separator: str = "```") -> str:
         """
         Extract the code from the response.
 
         Args:
             response (str): Response
             separator (str, optional): Separator. Defaults to "```".
@@ -67,27 +70,33 @@
             re.DOTALL,
         )
         if match:
             code = match.group(1).strip()
         if len(code.split(separator)) > 1:
             code = code.split(separator)[1]
 
+        if self.chat:
+            code = code.replace("python", "")
+
         if "fig.show()" in code:
             code = code.replace("fig.show()", "fig")
 
         return code
 
-    def generate_code(self, instruction: Prompt, prompt: str) -> str:
+    def generate_code(self, instructions: str) -> str:
         """
         Generate the code based on the instruction and the given prompt.
 
         Returns:
             str: Code
         """
-        return self._extract_code(self.completion(str(instruction) + prompt))
+        if self.chat:
+            return self._extract_code(self.chat_completion(instructions))
+        else:
+            return self._extract_code(self.completion(instructions))
 
     @property
     def _default_params(self) -> Dict[str, Any]:
         """
         Get the default parameters for calling OpenAI API
 
         Returns (Dict): A dict of OpenAi API parameters
@@ -114,7 +123,38 @@
             str: LLM response
         """
         params = {**self._default_params, "prompt": prompt}
 
         response = openai.Completion.create(**params)
 
         return response["choices"][0]["text"]
+
+    def chat_completion(self, value: str) -> str:
+        """
+        Query the chat completion API
+
+        Args:
+            value (str): Prompt
+
+        Returns:
+            str: LLM response
+        """
+        params = {
+            **self._default_params,
+            "messages": [
+                {
+                    "role": "system",
+                    "content": value,
+                }
+            ],
+        }
+
+        response = openai.ChatCompletion.create(**params)
+        message = response["choices"][0]["message"]["content"]
+
+        self.add_history(value, message)
+        return message
+
+    def add_history(self, user_message, bot_message):
+        self.messages.append({"role": "system", "content": bot_message})
+        self.messages.append({"role": "human", "content": user_message})
+        return None
```

### Comparing `chartgpt-0.0.3/chartgpt/prompts/base.py` & `chartgpt-0.0.4/chartgpt/prompts/base.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.3/chartgpt/prompts/generate_python_code.py` & `chartgpt-0.0.4/chartgpt/prompts/generate_python_code.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 You are ChartGPT, a data scientist working at a startup. You are asked to analyze a \
 dataset and create a chart.
 Today is {today_date}.
 You are given a dataset `df` with the following columns: {df_columns}.
 
 When asked about the data, your response must include a python code that uses the \
 library Plotly to make a chart using the dataframe `df`. If necessary, you can filter \
-the dataframe `df`. If the question in complex, feel free to use Plotly Graph Objects \
-instead of Plotly Express.
+the dataframe `df`. You can use any chart type you want.
 Using the provided dataframe, df, return the python code and make sure to prefix the \
 requested python code with {START_CODE_TAG} exactly and suffix the code with \
 {END_CODE_TAG} exactly to get the answer to the following question:
 """
 
     def __init__(self, **kwargs):
         super().__init__(
```

### Comparing `chartgpt-0.0.3/docs/assets/dash.png` & `chartgpt-0.0.4/docs/assets/dash.png`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.3/docs/assets/notebook.png` & `chartgpt-0.0.4/docs/assets/notebook.png`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.3/tests/test_run_code.py` & `chartgpt-0.0.4/tests/test_run_code.py`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.3/LICENSE` & `chartgpt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chartgpt-0.0.3/README.md` & `chartgpt-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 pip install chartgpt
 ```
 
 ## Example Usage 🎉
 
 ### Jupyter Notebook 📔
 
-![ChartGPT in a Jupyter notebook](docs/assets/notebook.png)
-
 ```python
 import chartgpt as cg
 
 df = pd.read_csv('data.csv')
 chart = cg.Chart(df, api_key="YOUR_API_KEY")
-chart.plot("Ask any question you want!")
+chart.plot("Pop vs. State")
 ```
 
+![ChartGPT in a Jupyter notebook](docs/assets/chart.png)
+
+Generated graph after inputting 'Pop vs. State'
+
 ### Dash App 🚀
 
 ![ChartGPT in a Dash app](docs/assets/dash.png)
 
 See Dash example [here](https://colab.research.google.com/drive/1KvXzl8W_WfmS-_VSG12A9eyT2YAHL1HE?usp=sharing).
 
 ## Documentation 📚
```

### Comparing `chartgpt-0.0.3/pyproject.toml` & `chartgpt-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chartgpt"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Elie Brosset", email="eliebrosset@gmail.com" },
 ]
 description = "ChartGPT is a library for generating charts from text"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `chartgpt-0.0.3/PKG-INFO` & `chartgpt-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartgpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: ChartGPT is a library for generating charts from text
 Project-URL: Homepage, https://github.com/chatgpt/chart
 Author-email: Elie Brosset <eliebrosset@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -61,24 +61,26 @@
 pip install chartgpt
 ```
 
 ## Example Usage 🎉
 
 ### Jupyter Notebook 📔
 
-![ChartGPT in a Jupyter notebook](docs/assets/notebook.png)
-
 ```python
 import chartgpt as cg
 
 df = pd.read_csv('data.csv')
 chart = cg.Chart(df, api_key="YOUR_API_KEY")
-chart.plot("Ask any question you want!")
+chart.plot("Pop vs. State")
 ```
 
+![ChartGPT in a Jupyter notebook](docs/assets/chart.png)
+
+Generated graph after inputting 'Pop vs. State'
+
 ### Dash App 🚀
 
 ![ChartGPT in a Dash app](docs/assets/dash.png)
 
 See Dash example [here](https://colab.research.google.com/drive/1KvXzl8W_WfmS-_VSG12A9eyT2YAHL1HE?usp=sharing).
 
 ## Documentation 📚
```

