# Comparing `tmp/starception-1.0.1.tar.gz` & `tmp/starception-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starception-1.0.1.tar", max compression
+gzip compressed data, was "starception-1.2.1.tar", max compression
```

## Comparing `starception-1.0.1.tar` & `starception-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,21 @@
--rw-r--r--   0        0        0     1074 2022-11-11 12:55:25.522223 starception-1.0.1/LICENSE
--rw-r--r--   0        0        0     4890 2022-11-11 12:55:25.522223 starception-1.0.1/README.md
--rw-r--r--   0        0        0     2864 2022-11-11 12:55:25.526223 starception-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      312 2022-11-11 12:55:25.526223 starception-1.0.1/starception/__init__.py
--rw-r--r--   0        0        0     9374 2022-11-11 12:55:25.526223 starception-1.0.1/starception/exception_handler.py
--rw-r--r--   0        0        0     2240 2022-11-11 12:55:25.526223 starception-1.0.1/starception/middleware.py
--rw-r--r--   0        0        0        0 2022-11-11 12:55:25.526223 starception-1.0.1/starception/py.typed
--rw-r--r--   0        0        0     4850 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/code_dark.css
--rw-r--r--   0        0        0     3303 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/code_light.css
--rw-r--r--   0        0        0     1519 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/code_snippet.html
--rw-r--r--   0        0        0      565 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/dark.css
--rw-r--r--   0        0        0      910 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/frame_line.html
--rw-r--r--   0        0        0      322 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/icon_google.svg
--rw-r--r--   0        0        0      362 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/icon_moon.svg
--rw-r--r--   0        0        0      555 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/icon_stackoverflow.svg
--rw-r--r--   0        0        0      418 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/icon_sun.svg
--rw-r--r--   0        0        0      548 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/icon_sun_moon.svg
--rw-r--r--   0        0        0     4721 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/index.html
--rw-r--r--   0        0        0      480 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/lib.html
--rw-r--r--   0        0        0     4591 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/scripts.js
--rw-r--r--   0        0        0     7145 2022-11-11 12:55:25.526223 starception-1.0.1/starception/templates/styles.css
--rw-r--r--   0        0        0     5898 1970-01-01 00:00:00.000000 starception-1.0.1/setup.py
--rw-r--r--   0        0        0     6419 1970-01-01 00:00:00.000000 starception-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-21 18:30:29.298027 starception-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3590 2023-06-21 18:30:29.298027 starception-1.2.1/README.md
+-rw-r--r--   0        0        0     2861 2023-06-21 18:30:29.302027 starception-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      226 2023-06-21 18:30:29.302027 starception-1.2.1/starception/__init__.py
+-rw-r--r--   0        0        0     9779 2023-06-21 18:30:29.302027 starception-1.2.1/starception/exception_handler.py
+-rw-r--r--   0        0        0        0 2023-06-21 18:30:29.302027 starception-1.2.1/starception/py.typed
+-rw-r--r--   0        0        0     4850 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/code_dark.css
+-rw-r--r--   0        0        0     3303 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/code_light.css
+-rw-r--r--   0        0        0     1519 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/code_snippet.html
+-rw-r--r--   0        0        0      565 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/dark.css
+-rw-r--r--   0        0        0      910 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/frame_line.html
+-rw-r--r--   0        0        0      322 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/icon_google.svg
+-rw-r--r--   0        0        0      362 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/icon_moon.svg
+-rw-r--r--   0        0        0      555 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/icon_stackoverflow.svg
+-rw-r--r--   0        0        0      418 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/icon_sun.svg
+-rw-r--r--   0        0        0      548 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/icon_sun_moon.svg
+-rw-r--r--   0        0        0     4935 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/index.html
+-rw-r--r--   0        0        0      489 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/lib.html
+-rw-r--r--   0        0        0     4608 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/scripts.js
+-rw-r--r--   0        0        0     7295 2023-06-21 18:30:29.302027 starception-1.2.1/starception/templates/styles.css
+-rw-r--r--   0        0        0     4786 1970-01-01 00:00:00.000000 starception-1.2.1/PKG-INFO
```

### Comparing `starception-1.0.1/LICENSE` & `starception-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starception-1.0.1/README.md` & `starception-1.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,42 @@
+Metadata-Version: 2.1
+Name: starception
+Version: 1.2.1
+Summary: Beautiful debugging page for Starlette apps.
+Home-page: https://github.com/alex-oleshkevich/starception
+License: MIT
+Author: Alex Oleshkevich
+Author-email: alex.oleshkevich@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Provides-Extra: highlight
+Requires-Dist: Jinja2 (>=3,<4)
+Requires-Dist: MarkupSafe (>=2,<3)
+Requires-Dist: typing_extensions (>=4.4,<5.0)
+Project-URL: Documentation, https://github.com/alex-oleshkevich/starception
+Project-URL: Repository, https://github.com/alex-oleshkevich/starception
+Description-Content-Type: text/markdown
+
 # Starception
 
 Beautiful exception page for Starlette and FastAPI apps.
 
 ![PyPI](https://img.shields.io/pypi/v/starception)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/alex-oleshkevich/starception/Lint%20and%20test)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/alex-oleshkevich/starception/lint_and_test.yml?branch=master)
 ![GitHub](https://img.shields.io/github/license/alex-oleshkevich/starception)
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/starception)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/starception)
 ![GitHub Release Date](https://img.shields.io/github/release-date/alex-oleshkevich/starception)
 
 ## Installation
 
@@ -51,89 +80,34 @@
 * platform information
 * environment variables
 * syntax highlight
 * open paths in editor (vscode only)
 * exception chains
 * dark theme
 
-The middleware will automatically mask any value which key contains `key`, `secret`, `token`, `password`.
+Starception automatically masks any value which key contains `key`, `secret`, `token`, `password`.
 
 ## Quick start
 
 See example application in [examples/](examples/) directory of this repository.
 
 ## Usage
 
-Starception will work only in debug mode so don't forget to set `debug=True` for local development.
-
-### Monkey patching Starlette
+Starception will work only in debug mode so don't forget to set `Starlette.debug=True`.
 
 To replace built-in debug exception handler call `install_error_handler` before you create Starlette instance.
-> Currently, this is a recommended approach.
 
 ```python
 from starception import install_error_handler
 from starlette.applications import Starlette
 
 install_error_handler()
 app = Starlette()
 ```
 
-### Using middleware
-
-To render a beautiful exception page you need to install a `StarceptionMiddleware` middleware to your application.
-
-
-> Note, to catch as many exceptions as possible the middleware has to be the first one in the stack.
-
-```python
-import typing
-
-from starlette.applications import Starlette
-from starlette.middleware import Middleware
-from starlette.requests import Request
-from starlette.routing import Route
-
-from starception import StarceptionMiddleware
-
-
-async def index_view(request: Request) -> typing.NoReturn:
-    raise TypeError('Oops, something really went wrong...')
-
-
-app = Starlette(
-    debug=True,
-    routes=[Route('/', index_view)],
-    middleware=[
-        Middleware(StarceptionMiddleware),
-        # other middleware go here
-    ],
-)
-```
-
-### Integration with FastAPI
-
-Attach `StarceptionMiddleware` middleware to your FastAPI application:
-
-```python
-import typing
-
-from fastapi import FastAPI, Request
-
-from starception import StarceptionMiddleware
-
-app = FastAPI(debug=True)
-app.add_middleware(StarceptionMiddleware)  # must be the first one!
-
-
-@app.route('/')
-async def index_view(request: Request) -> typing.NoReturn:
-    raise TypeError('Oops, something really went wrong...')
-```
-
 ### Integration with other frameworks
 
 `starception` exports `starception.exception_handler(request, exc)` function, which you can use in your
 framework.
 But keep in mind, Starlette will [not call](https://github.com/encode/starlette/issues/1802) any custom exception
 handler
 in debug mode (it always uses built-in one).
@@ -191,7 +165,8 @@
 set_editor('vscode')
 ```
 
 ## Credentials
 
 * Look and feel inspired by [Phoenix Framework](https://www.phoenixframework.org/).
 * Icons by [Tabler Icons](https://tabler-icons.io/).
+
```

### Comparing `starception-1.0.1/pyproject.toml` & `starception-1.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 [tool.poetry]
 name = "starception"
 description = "Beautiful debugging page for Starlette apps."
-version = "1.0.1"
+version = "1.2.1"
 authors = ["Alex Oleshkevich <alex.oleshkevich@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/alex-oleshkevich/starception"
 repository = "https://github.com/alex-oleshkevich/starception"
 documentation = "https://github.com/alex-oleshkevich/starception"
 keywords = []
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.7",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-starlette = "^0"
+python = "^3.8"
 MarkupSafe = "^2"
 Jinja2 = "^3"
 typing_extensions = "^4.4"
 
 [tool.poetry.group.dev.dependencies]
+starlette = "*"
 pytest = "^7.2"
 pytest-asyncio = "^0.18.0"
 pytest-cov = "^4.0"
 black = "^22.6.0"
-mypy = "^v0.971"
+mypy = "^1.4"
 flake8 = "^4.0.1"
 uvicorn = "^0.18.2"
 fastapi = "^0.79.0"
 requests = "^2.28.1"
 pygments = { optional = true, version = "^2.13" }
 
 [tool.poetry.extras]
```

### Comparing `starception-1.0.1/starception/exception_handler.py` & `starception-1.2.1/starception/exception_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     return template.format(path=path, lineno=lineno)
 
 
 def install_error_handler(editor: str = '') -> None:
     """
     Replace Starlette debug exception handler in-place.
 
-    May be, someday, we won't need it.
-    See https://github.com/encode/starlette/discussions/1867
+    May be, someday, we won't need it. See
+    https://github.com/encode/starlette/discussions/1867
     """
     set_editor(editor)
 
     def bound_handler(self: ServerErrorMiddleware, request: Request, exc: Exception) -> Response:
         return exception_handler(request, exc)
 
     setattr(ServerErrorMiddleware, 'debug_response', bound_handler)
@@ -178,18 +178,26 @@
         if lexer:
             return highlight(value, lexer, HtmlFormatter(nowrap=True))  # type: ignore
         return value
     except ImportError:
         return markupsafe.escape(value)
 
 
+def save_str(value: typing.Any) -> str:
+    try:
+        return str(value)
+    except Exception as ex:
+        return Markup(f'<span class="text-error">ERROR</span>: {html.escape(str(ex))}')
+
+
 jinja = jinja2.Environment(loader=jinja2.PackageLoader(__name__))
 jinja.filters.update(
     {
         'symbol': get_symbol,
+        'save_str': save_str,
         'frame_id': frame_id,
         'is_vendor': is_vendor,
         'highlight': highlight,
         'to_ide_link': to_ide_link,
         'mask_secrets': mask_secrets,
         'package_dir': get_package_dir,
         'package_name': get_package_name,
@@ -216,35 +224,38 @@
 
 @dataclasses.dataclass
 class StackItem:
     exc: Exception
     frames: typing.List[inspect.FrameInfo]
     has_vendor_frames: bool
     solution: str
+    notes: typing.List[str]
 
 
 def generate_html(request: Request, exc: Exception, limit: int = 15) -> str:
     traceback_obj = traceback.TracebackException.from_exception(exc, capture_locals=True)
     frames = inspect.getinnerframes(exc.__traceback__, limit) if exc.__traceback__ else []
     stack = [
         StackItem(
             exc=exc,
             solution=getattr(exc, 'solution', ''),
+            notes=getattr(exc, '__notes__', []),
             frames=frames,
             has_vendor_frames=any(is_vendor(f) for f in frames),
         )
     ]
     exception = exc
     cause = getattr(exception, '__cause__')
     while cause:
         frames = inspect.getinnerframes(cause.__traceback__, limit) if cause.__traceback__ else []
         stack.append(
             StackItem(
                 exc=cause,
                 solution=getattr(cause, 'solution', ''),
+                notes=getattr(exc, '__notes__', []),
                 frames=frames,
                 has_vendor_frames=any(is_vendor(f) for f in frames),
             )
         )
         cause = getattr(cause, '__cause__')
 
     template = jinja.get_template('index.html')
@@ -287,14 +298,15 @@
                 "Python version": sys.version,
                 "Platform": sys.platform,
                 "Python": sys.executable,
                 "Paths": Markup("<br>".join(sys.path)),
             },
             'environment': os.environ,
             'solution': getattr(exc, 'solution', None),
+            'notes': getattr(exc, '__notes__', []),
         }
     )
 
 
 def _get_session_info(request: Request) -> typing.Dict[str, typing.Any]:
     try:
         return dict(request.session if 'session' in request.scope else {})
```

### Comparing `starception-1.0.1/starception/templates/code_dark.css` & `starception-1.2.1/starception/templates/code_dark.css`

 * *Files identical despite different names*

### Comparing `starception-1.0.1/starception/templates/code_light.css` & `starception-1.2.1/starception/templates/code_light.css`

 * *Files identical despite different names*

### Comparing `starception-1.0.1/starception/templates/code_snippet.html` & `starception-1.2.1/starception/templates/code_snippet.html`

 * *Files identical despite different names*

### Comparing `starception-1.0.1/starception/templates/dark.css` & `starception-1.2.1/starception/templates/dark.css`

 * *Files identical despite different names*

### Comparing `starception-1.0.1/starception/templates/frame_line.html` & `starception-1.2.1/starception/templates/frame_line.html`

 * *Files identical despite different names*

### Comparing `starception-1.0.1/starception/templates/icon_stackoverflow.svg` & `starception-1.2.1/starception/templates/icon_stackoverflow.svg`

 * *Files identical despite different names*

### Comparing `starception-1.0.1/starception/templates/icon_sun_moon.svg` & `starception-1.2.1/starception/templates/icon_sun_moon.svg`

 * *Files identical despite different names*

### Comparing `starception-1.0.1/starception/templates/index.html` & `starception-1.2.1/starception/templates/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -18,25 +18,14 @@
             <div>
                 <strong class="exception-class">{{ exception_class }}</strong>
                 at {{ request_method }} {{ request_path }}
             </div>
             <div class="exception text-red">{{ error_message|e }}</div>
         </div>
         <div class="flex-center">
-            <div class="search-links">
-                <a target="_blank" href="https://www.google.com/search?q={{ search_query }}">
-                    {% include 'icon_google.svg' %}
-                    <span>Google</span>
-                </a>
-                <a target="_blank" href="https://www.stackoverflow.com/search?q={{ search_query }}">
-                    {% include 'icon_stackoverflow.svg' %}
-                    <span>Stack Overflow</span>
-                </a>
-            </div>
-
             <!-- auto -> dark -> light -> auto -->
             <button data-theme-toggle>
                 <div data-force-theme="light" title="Force light theme">
                     {% include 'icon_sun.svg' %}
                 </div>
                 <div data-force-theme="auto" class="flex-center" title="Use system theme">
                     {% include 'icon_sun_moon.svg' %}
@@ -44,16 +33,25 @@
                 </div>
                 <div data-force-theme="dark" title="Force dark theme">
                     {% include 'icon_moon.svg' %}
                 </div>
             </button>
         </div>
     </div>
-    {% if solution %}
-        <div class="solution">Hint: {{ solution }}</div>
+    {% if solution or notes %}
+        <div class="solution">
+            <ul>
+                {% if solution %}
+                    <li>{{ solution }}</li>
+                {% endif %}
+                {% for note in notes %}
+                    <li>{{ note }}</li>
+                {% endfor %}
+            </ul>
+        </div>
     {% endif %}
 </header>
 <main>
     <!-- exception block -->
     {% for stack_item in stack %}
         {% set stackloop = loop %}
         <div data-stack-root="{{ stackloop.loop0 }}">
@@ -63,17 +61,26 @@
                     <div>
                         <div class="exception text-red">{{ stack_item.exc|e }}</div>
                     </div>
                 </header>
             {% endif %}
             <div data-trace-target {% if loop.index0 > 0 %} class="collapsed"{% endif %}>
                 {% if loop.index0 > 0 %}
-                    {% if stack_item.solution %}
+                    {% if stack_item.solution or stack_item.notes %}
                         <div style="padding: 0 48px">
-                            <div class="solution" style="margin-top: 8px">Hint: {{ stack_item.solution }}</div>
+                            <div class="solution" style="margin-top: 8px">
+                                <ul>
+                                    {% if stack_item.solution %}
+                                        <li>{{ stack_item.solution }}</li>
+                                    {% endif %}
+                                    {% for note in stack_item.notes %}
+                                        <li>{{ note }}</li>
+                                    {% endfor %}
+                                </ul>
+                            </div>
                         </div>
                     {% endif %}
                 {% endif %}
                 <section class="trace">
                     {% for frame in stack_item.frames|reverse %}
                         {% with frame=frame, is_current=loop.first %}
                             {% include 'code_snippet.html' %}
```

#### html2text {}

```diff
@@ -1,25 +1,31 @@
 {% import 'lib.html' as lib %}
 {{ exception_class }} at {{ request_method }} {{ request_path }}
 {{ error_message|e }}
-{%_include_'icon_google.svg'_%}_Google {%_include_'icon_stackoverflow.svg'_%}
-Stack_Overflow
 
 {% include 'icon_sun.svg' %}
 {% include 'icon_sun_moon.svg' %} Auto
 {% include 'icon_moon.svg' %}
-{% if solution %}
-Hint: {{ solution }}
+{% if solution or notes %}
+    * {% if solution %}
+    * {{ solution }}
+    * {% endif %} {% for note in notes %}
+    * {{ note }}
+    * {% endfor %}
 {% endif %}    {% for stack_item in stack %} {% set stackloop = loop %}
 {% if loop.index0 > 0 %}  Caused by
 {{ stack_item.exc|e }}
  {% endif %}
 % if loop.index0 > 0 %} class="collapsed"{% endif %}> {% if loop.index0 > 0 %}
-{% if stack_item.solution %}
-Hint: {{ stack_item.solution }}
+{% if stack_item.solution or stack_item.notes %}
+    * {% if stack_item.solution %}
+    * {{ stack_item.solution }}
+    * {% endif %} {% for note in stack_item.notes %}
+    * {{ note }}
+    * {% endfor %}
 {% endif %} {% endif %}  {% for frame in stack_item.frames|reverse %} {% with
 frame=frame, is_current=loop.first %} {% include 'code_snippet.html' %} {%
 endwith %} {% endfor %}
 {% if stack_item.has_vendor_frames %}
  * Hide vendor frames
 {% endif %} {% for frame in stack_item.frames|reverse %} {% with frame=frame,
 is_current=loop.first %} {% include 'frame_line.html' %} {% endwith %} {%
```

### Comparing `starception-1.0.1/starception/templates/scripts.js` & `starception-1.2.1/starception/templates/scripts.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -132,19 +132,21 @@
 
 /**
  * Bind exception block features.
  * @param {HTMLElement} el
  */
 function bindStackBlock(el) {
     restoreColorTheme();
-    bindThemeToggle();
     bindVendorFramesToggle(el);
     bindExceptionBlocks(el);
     bindCodeSnippets(el);
     bindSecretsReveal();
 }
 
 function bindStackBlocks() {
     document.querySelectorAll('[data-stack-root]').forEach(bindStackBlock);
 }
 
-document.addEventListener('DOMContentLoaded', bindStackBlocks);
+document.addEventListener('DOMContentLoaded', () => {
+    bindThemeToggle();
+    bindStackBlocks();
+});
```

### Comparing `starception-1.0.1/starception/templates/styles.css` & `starception-1.2.1/starception/templates/styles.css`

 * *Files 1% similar despite different names*

```diff
@@ -372,7 +372,21 @@
     width: 20px;
     height: 20px;
 }
 
 .search-links a:hover {
     text-decoration: underline;
 }
+
+.text-error {
+    color: var(--red);
+}
+
+.solution ul {
+    margin: 0;
+    padding: 0;
+}
+
+.solution ul li {
+    margin: 0 0 0 20px;
+    padding: 0;
+}
```

