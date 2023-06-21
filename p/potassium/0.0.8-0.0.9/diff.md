# Comparing `tmp/potassium-0.0.8.tar.gz` & `tmp/potassium-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potassium-0.0.8.tar", last modified: Sun Mar 26 02:52:22 2023, max compression
+gzip compressed data, was "potassium-0.0.9.tar", last modified: Thu May 25 22:30:00 2023, max compression
```

## Comparing `potassium-0.0.8.tar` & `potassium-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-26 02:52:22.943730 potassium-0.0.8/
--rw-r--r--   0 erik       (501) staff       (20)    11357 2023-03-01 00:40:07.000000 potassium-0.0.8/LICENSE
--rw-r--r--   0 erik       (501) staff       (20)     6384 2023-03-26 02:52:22.943571 potassium-0.0.8/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     5718 2023-03-26 02:49:27.000000 potassium-0.0.8/README.md
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-26 02:52:22.942622 potassium-0.0.8/potassium/
--rw-r--r--   0 erik       (501) staff       (20)       45 2023-03-24 22:28:08.000000 potassium-0.0.8/potassium/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)      221 2023-03-24 22:28:08.000000 potassium-0.0.8/potassium/hooks.py
--rw-r--r--   0 erik       (501) staff       (20)     3839 2023-03-26 02:47:22.000000 potassium-0.0.8/potassium/potassium.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-26 02:52:22.943338 potassium-0.0.8/potassium.egg-info/
--rw-r--r--   0 erik       (501) staff       (20)     6384 2023-03-26 02:52:22.000000 potassium-0.0.8/potassium.egg-info/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)      254 2023-03-26 02:52:22.000000 potassium-0.0.8/potassium.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2023-03-26 02:52:22.000000 potassium-0.0.8/potassium.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (501) staff       (20)       25 2023-03-26 02:52:22.000000 potassium-0.0.8/potassium.egg-info/requires.txt
--rw-r--r--   0 erik       (501) staff       (20)       10 2023-03-26 02:52:22.000000 potassium-0.0.8/potassium.egg-info/top_level.txt
--rw-r--r--   0 erik       (501) staff       (20)       38 2023-03-26 02:52:22.943793 potassium-0.0.8/setup.cfg
--rw-r--r--   0 erik       (501) staff       (20)     1241 2023-03-26 02:49:09.000000 potassium-0.0.8/setup.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-05-25 22:30:00.474604 potassium-0.0.9/
+-rw-r--r--   0 erik       (501) staff       (20)    11357 2023-04-24 01:09:41.000000 potassium-0.0.9/LICENSE
+-rw-r--r--   0 erik       (501) staff       (20)     7939 2023-05-25 22:30:00.474489 potassium-0.0.9/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)     7273 2023-05-12 03:11:03.000000 potassium-0.0.9/README.md
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-05-25 22:30:00.473780 potassium-0.0.9/potassium/
+-rw-r--r--   0 erik       (501) staff       (20)       83 2023-04-28 20:13:33.000000 potassium-0.0.9/potassium/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)      221 2023-04-24 01:09:41.000000 potassium-0.0.9/potassium/hooks.py
+-rw-r--r--   0 erik       (501) staff       (20)     6946 2023-05-25 22:13:36.000000 potassium-0.0.9/potassium/potassium.py
+-rw-r--r--   0 erik       (501) staff       (20)     4063 2023-04-28 21:55:56.000000 potassium-0.0.9/potassium/store.py
+-rw-r--r--   0 erik       (501) staff       (20)     1305 2023-04-28 21:46:28.000000 potassium-0.0.9/potassium/store_test.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-05-25 22:30:00.474332 potassium-0.0.9/potassium.egg-info/
+-rw-r--r--   0 erik       (501) staff       (20)     7939 2023-05-25 22:30:00.000000 potassium-0.0.9/potassium.egg-info/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)      297 2023-05-25 22:30:00.000000 potassium-0.0.9/potassium.egg-info/SOURCES.txt
+-rw-r--r--   0 erik       (501) staff       (20)        1 2023-05-25 22:30:00.000000 potassium-0.0.9/potassium.egg-info/dependency_links.txt
+-rw-r--r--   0 erik       (501) staff       (20)       31 2023-05-25 22:30:00.000000 potassium-0.0.9/potassium.egg-info/requires.txt
+-rw-r--r--   0 erik       (501) staff       (20)       10 2023-05-25 22:30:00.000000 potassium-0.0.9/potassium.egg-info/top_level.txt
+-rw-r--r--   0 erik       (501) staff       (20)       38 2023-05-25 22:30:00.474636 potassium-0.0.9/setup.cfg
+-rw-r--r--   0 erik       (501) staff       (20)     1258 2023-05-25 22:27:50.000000 potassium-0.0.9/setup.py
```

### Comparing `potassium-0.0.8/LICENSE` & `potassium-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `potassium-0.0.8/PKG-INFO` & `potassium-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: potassium
-Version: 0.0.8
-Summary: The potassium package is a flask-like HTTP server for serving large AI models
-Home-page: https://www.banana.dev
-Author: Erik Dunteman
-Author-email: erik@banana.dev
-License: Apache License 2.0
-Keywords: Banana server,HTTP server,Banana,Framework
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Potassium
 
 ![Potassium (1)](https://user-images.githubusercontent.com/44653944/222016748-ca2c6905-8fd5-4ee5-a68e-7aed48f23436.png)
 
 [Potassium](https://github.com/bananaml/potassium) is an open source web framework, built to tackle the unique challenges of serving custom models in production.
 
 The goal of this project is to:
@@ -29,16 +11,15 @@
 - Provide a set of primitives common in ML serving, such as:
     - POST request handlers
     - Websocket / streaming connections
     - Async handlers w/ webhooks
 - Maintain a standard interface, to allow the code and models to compile to specialized hardware (ideally on [Banana Serverless GPUs](https://banana.dev) 😉)
 
 ### Stability Notes:
-- This is a v0 release using SemVer, and is not stable; the interface may change at any time. Be sure to lock your versions!
-- If deploying to Banana, Potassium apps currently won't receive [fast boot optimizations](https://docs.banana.dev/banana-docs/core-concepts/build-system). This will be added within a few days.
+Potassium uses Semantic Versioning, in that major versions imply breaking changes, and v0 implies instability even between minor/patch versions. Be sure to lock your versions, as we're still in v0!
 
 ---
 
 ## Quickstart: Serving a Huggingface BERT model
 
 The fastest way to get up and running is to use the [Banana CLI](https://github.com/bananaml/banana-cli), which downloads and runs your first model.
 
@@ -176,15 +157,15 @@
 There may only be one `@app.init` function.
 
 ---
 
 ## @app.handler()
 
 ```python
-@app.handler("/")
+@app.handler("/", gpu=True)
 def handler(context: dict, request: Request) -> Response:
     
     prompt = request.json.get("prompt")
     model = context.get("model")
     outputs = model(prompt)
 
     return Response(
@@ -192,39 +173,82 @@
         status=200
     )
 ```
 
 The `@app.handler` decorated function runs for every http call, and is used to run inference or training workloads against your model(s).
 
 You may configure as many `@app.handler` functions as you'd like, with unique API routes.
-Note: Banana serverless currently only supports handlers at the root "/"
+
+The `gpu=True` argument allows the handler to access the prewarmed context value, and runs the handler as blocking. While the handler is running, potassium will reject any other `gpu=True` handlers with a 423 Locked error, to ensure that there are no multithreading issues with CUDA. If set to `false`, the handler may be called at any time, but the context provided will be `None`. `gpu` defaults to `True`.
 
 ---
 
-## @app.async_handler(path="/async")
+## @app.background(path="/background", gpu=True)
 
 ```python
-@app.async_handler("/async")
+@app.background("/background")
 def handler(context: dict, request: Request) -> Response:
 
     prompt = request.json.get("prompt")
     model = context.get("model")
     outputs = model(prompt)
 
     send_webhook(url="http://localhost:8001", json={"outputs": outputs})
 
     return
 ```
 
-The `@app.async_handler()` decorated function runs a nonblocking job in the background, for tasks where results aren't expected to return clientside. It's on you to forward the data to wherever you please. Potassium supplies a `send_webhook()` helper function for POSTing data onward to a url, or you may add your own custom upload/pipeline code.
+The `@app.background()` decorated function runs a nonblocking job in the background, for tasks where results aren't expected to return clientside. It's on you to forward the data to wherever you please. Potassium supplies a `send_webhook()` helper function for POSTing data onward to a url, or you may add your own custom upload/pipeline code.
 
 When invoked, the client immediately returns a `{"success": true}` message.
 
-You may configure as many `@app.async_handler` functions as you'd like, with unique API routes.
-Note: Banana serverless isn't perfectly stable running async_handler. You can use it, but concurrency may be weird.
+You may configure as many `@app.background` functions as you'd like, with unique API routes.
 
+The `gpu=True` argument allows the background handler to access the prewarmed context value, and runs the child background thread as blocking. While the child thread is running, potassium will reject any other `gpu=True` handlers with a 423 Locked error, to ensure that there are no multithreading issues with CUDA. If set to `false`, the handler may be called at any time, but the context provided will be `None`. `gpu` defaults to `True`.
 
 ---
 
 ## app.serve()
 
 `app.serve` runs the server, and is a blocking operation.
+
+
+---
+
+# Store
+Potassium includes a key-value storage primative, to help users persist data between calls. This is often used to implement patterns such as an async-worker queue where one background task runs inference and saves the result to the Store, with another handler set to `gpu=False` built to fetch the result.
+
+Example usage: your own Redis backend (encouraged)
+```
+from potassium.store import Store, RedisConfig
+
+store = Store(
+    backend="redis",
+    config = RedisConfig(
+        host = "localhost",
+        port = 6379
+    )
+)
+
+# in one handler
+store.set("key", "value", ttl=60)
+
+# in another handler
+value = store.get("key")
+```
+
+Example usage: using local storage 
+- Note: not encouraged on Banana serverless or multi-replica environments, as data is stored only on the single replica
+```
+from potassium.store import Store, RedisConfig
+
+store = Store(
+    backend="local"
+)
+
+# in one handler
+store.set("key", "value", ttl=60)
+
+# in another handler
+value = store.get("key")
+```
+
```

### Comparing `potassium-0.0.8/README.md` & `potassium-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: potassium
+Version: 0.0.9
+Summary: The potassium package is a flask-like HTTP server for serving large AI models
+Home-page: https://www.banana.dev
+Author: Erik Dunteman
+Author-email: erik@banana.dev
+License: Apache License 2.0
+Keywords: Banana server,HTTP server,Banana,Framework
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Potassium
 
 ![Potassium (1)](https://user-images.githubusercontent.com/44653944/222016748-ca2c6905-8fd5-4ee5-a68e-7aed48f23436.png)
 
 [Potassium](https://github.com/bananaml/potassium) is an open source web framework, built to tackle the unique challenges of serving custom models in production.
 
 The goal of this project is to:
@@ -11,16 +29,15 @@
 - Provide a set of primitives common in ML serving, such as:
     - POST request handlers
     - Websocket / streaming connections
     - Async handlers w/ webhooks
 - Maintain a standard interface, to allow the code and models to compile to specialized hardware (ideally on [Banana Serverless GPUs](https://banana.dev) 😉)
 
 ### Stability Notes:
-- This is a v0 release using SemVer, and is not stable; the interface may change at any time. Be sure to lock your versions!
-- If deploying to Banana, Potassium apps currently won't receive [fast boot optimizations](https://docs.banana.dev/banana-docs/core-concepts/build-system). This will be added within a few days.
+Potassium uses Semantic Versioning, in that major versions imply breaking changes, and v0 implies instability even between minor/patch versions. Be sure to lock your versions, as we're still in v0!
 
 ---
 
 ## Quickstart: Serving a Huggingface BERT model
 
 The fastest way to get up and running is to use the [Banana CLI](https://github.com/bananaml/banana-cli), which downloads and runs your first model.
 
@@ -158,15 +175,15 @@
 There may only be one `@app.init` function.
 
 ---
 
 ## @app.handler()
 
 ```python
-@app.handler("/")
+@app.handler("/", gpu=True)
 def handler(context: dict, request: Request) -> Response:
     
     prompt = request.json.get("prompt")
     model = context.get("model")
     outputs = model(prompt)
 
     return Response(
@@ -174,39 +191,82 @@
         status=200
     )
 ```
 
 The `@app.handler` decorated function runs for every http call, and is used to run inference or training workloads against your model(s).
 
 You may configure as many `@app.handler` functions as you'd like, with unique API routes.
-Note: Banana serverless currently only supports handlers at the root "/"
+
+The `gpu=True` argument allows the handler to access the prewarmed context value, and runs the handler as blocking. While the handler is running, potassium will reject any other `gpu=True` handlers with a 423 Locked error, to ensure that there are no multithreading issues with CUDA. If set to `false`, the handler may be called at any time, but the context provided will be `None`. `gpu` defaults to `True`.
 
 ---
 
-## @app.async_handler(path="/async")
+## @app.background(path="/background", gpu=True)
 
 ```python
-@app.async_handler("/async")
+@app.background("/background")
 def handler(context: dict, request: Request) -> Response:
 
     prompt = request.json.get("prompt")
     model = context.get("model")
     outputs = model(prompt)
 
     send_webhook(url="http://localhost:8001", json={"outputs": outputs})
 
     return
 ```
 
-The `@app.async_handler()` decorated function runs a nonblocking job in the background, for tasks where results aren't expected to return clientside. It's on you to forward the data to wherever you please. Potassium supplies a `send_webhook()` helper function for POSTing data onward to a url, or you may add your own custom upload/pipeline code.
+The `@app.background()` decorated function runs a nonblocking job in the background, for tasks where results aren't expected to return clientside. It's on you to forward the data to wherever you please. Potassium supplies a `send_webhook()` helper function for POSTing data onward to a url, or you may add your own custom upload/pipeline code.
 
 When invoked, the client immediately returns a `{"success": true}` message.
 
-You may configure as many `@app.async_handler` functions as you'd like, with unique API routes.
-Note: Banana serverless isn't perfectly stable running async_handler. You can use it, but concurrency may be weird.
+You may configure as many `@app.background` functions as you'd like, with unique API routes.
 
+The `gpu=True` argument allows the background handler to access the prewarmed context value, and runs the child background thread as blocking. While the child thread is running, potassium will reject any other `gpu=True` handlers with a 423 Locked error, to ensure that there are no multithreading issues with CUDA. If set to `false`, the handler may be called at any time, but the context provided will be `None`. `gpu` defaults to `True`.
 
 ---
 
 ## app.serve()
 
 `app.serve` runs the server, and is a blocking operation.
+
+
+---
+
+# Store
+Potassium includes a key-value storage primative, to help users persist data between calls. This is often used to implement patterns such as an async-worker queue where one background task runs inference and saves the result to the Store, with another handler set to `gpu=False` built to fetch the result.
+
+Example usage: your own Redis backend (encouraged)
+```
+from potassium.store import Store, RedisConfig
+
+store = Store(
+    backend="redis",
+    config = RedisConfig(
+        host = "localhost",
+        port = 6379
+    )
+)
+
+# in one handler
+store.set("key", "value", ttl=60)
+
+# in another handler
+value = store.get("key")
+```
+
+Example usage: using local storage 
+- Note: not encouraged on Banana serverless or multi-replica environments, as data is stored only on the single replica
+```
+from potassium.store import Store, RedisConfig
+
+store = Store(
+    backend="local"
+)
+
+# in one handler
+store.set("key", "value", ttl=60)
+
+# in another handler
+value = store.get("key")
+```
+
```

### Comparing `potassium-0.0.8/potassium.egg-info/PKG-INFO` & `potassium-0.0.9/potassium.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potassium
-Version: 0.0.8
+Version: 0.0.9
 Summary: The potassium package is a flask-like HTTP server for serving large AI models
 Home-page: https://www.banana.dev
 Author: Erik Dunteman
 Author-email: erik@banana.dev
 License: Apache License 2.0
 Keywords: Banana server,HTTP server,Banana,Framework
 Classifier: Development Status :: 3 - Alpha
@@ -29,16 +29,15 @@
 - Provide a set of primitives common in ML serving, such as:
     - POST request handlers
     - Websocket / streaming connections
     - Async handlers w/ webhooks
 - Maintain a standard interface, to allow the code and models to compile to specialized hardware (ideally on [Banana Serverless GPUs](https://banana.dev) 😉)
 
 ### Stability Notes:
-- This is a v0 release using SemVer, and is not stable; the interface may change at any time. Be sure to lock your versions!
-- If deploying to Banana, Potassium apps currently won't receive [fast boot optimizations](https://docs.banana.dev/banana-docs/core-concepts/build-system). This will be added within a few days.
+Potassium uses Semantic Versioning, in that major versions imply breaking changes, and v0 implies instability even between minor/patch versions. Be sure to lock your versions, as we're still in v0!
 
 ---
 
 ## Quickstart: Serving a Huggingface BERT model
 
 The fastest way to get up and running is to use the [Banana CLI](https://github.com/bananaml/banana-cli), which downloads and runs your first model.
 
@@ -176,15 +175,15 @@
 There may only be one `@app.init` function.
 
 ---
 
 ## @app.handler()
 
 ```python
-@app.handler("/")
+@app.handler("/", gpu=True)
 def handler(context: dict, request: Request) -> Response:
     
     prompt = request.json.get("prompt")
     model = context.get("model")
     outputs = model(prompt)
 
     return Response(
@@ -192,39 +191,82 @@
         status=200
     )
 ```
 
 The `@app.handler` decorated function runs for every http call, and is used to run inference or training workloads against your model(s).
 
 You may configure as many `@app.handler` functions as you'd like, with unique API routes.
-Note: Banana serverless currently only supports handlers at the root "/"
+
+The `gpu=True` argument allows the handler to access the prewarmed context value, and runs the handler as blocking. While the handler is running, potassium will reject any other `gpu=True` handlers with a 423 Locked error, to ensure that there are no multithreading issues with CUDA. If set to `false`, the handler may be called at any time, but the context provided will be `None`. `gpu` defaults to `True`.
 
 ---
 
-## @app.async_handler(path="/async")
+## @app.background(path="/background", gpu=True)
 
 ```python
-@app.async_handler("/async")
+@app.background("/background")
 def handler(context: dict, request: Request) -> Response:
 
     prompt = request.json.get("prompt")
     model = context.get("model")
     outputs = model(prompt)
 
     send_webhook(url="http://localhost:8001", json={"outputs": outputs})
 
     return
 ```
 
-The `@app.async_handler()` decorated function runs a nonblocking job in the background, for tasks where results aren't expected to return clientside. It's on you to forward the data to wherever you please. Potassium supplies a `send_webhook()` helper function for POSTing data onward to a url, or you may add your own custom upload/pipeline code.
+The `@app.background()` decorated function runs a nonblocking job in the background, for tasks where results aren't expected to return clientside. It's on you to forward the data to wherever you please. Potassium supplies a `send_webhook()` helper function for POSTing data onward to a url, or you may add your own custom upload/pipeline code.
 
 When invoked, the client immediately returns a `{"success": true}` message.
 
-You may configure as many `@app.async_handler` functions as you'd like, with unique API routes.
-Note: Banana serverless isn't perfectly stable running async_handler. You can use it, but concurrency may be weird.
+You may configure as many `@app.background` functions as you'd like, with unique API routes.
 
+The `gpu=True` argument allows the background handler to access the prewarmed context value, and runs the child background thread as blocking. While the child thread is running, potassium will reject any other `gpu=True` handlers with a 423 Locked error, to ensure that there are no multithreading issues with CUDA. If set to `false`, the handler may be called at any time, but the context provided will be `None`. `gpu` defaults to `True`.
 
 ---
 
 ## app.serve()
 
 `app.serve` runs the server, and is a blocking operation.
+
+
+---
+
+# Store
+Potassium includes a key-value storage primative, to help users persist data between calls. This is often used to implement patterns such as an async-worker queue where one background task runs inference and saves the result to the Store, with another handler set to `gpu=False` built to fetch the result.
+
+Example usage: your own Redis backend (encouraged)
+```
+from potassium.store import Store, RedisConfig
+
+store = Store(
+    backend="redis",
+    config = RedisConfig(
+        host = "localhost",
+        port = 6379
+    )
+)
+
+# in one handler
+store.set("key", "value", ttl=60)
+
+# in another handler
+value = store.get("key")
+```
+
+Example usage: using local storage 
+- Note: not encouraged on Banana serverless or multi-replica environments, as data is stored only on the single replica
+```
+from potassium.store import Store, RedisConfig
+
+store = Store(
+    backend="local"
+)
+
+# in one handler
+store.set("key", "value", ttl=60)
+
+# in another handler
+value = store.get("key")
+```
+
```

### Comparing `potassium-0.0.8/setup.py` & `potassium-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='potassium',
     packages=['potassium'],
-    version='0.0.8',
+    version='0.0.9',
     license='Apache License 2.0',
     # Give a short description about your library
     description='The potassium package is a flask-like HTTP server for serving large AI models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Erik Dunteman',
     author_email='erik@banana.dev',
     url='https://www.banana.dev',
     keywords=['Banana server', 'HTTP server', 'Banana', 'Framework'],
     setup_requires=['wheel'],
     install_requires=[
         "Flask",
         "requests",
-        "termcolor"
+        "termcolor",
+        "redis"
     ],
     classifiers=[
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
```

