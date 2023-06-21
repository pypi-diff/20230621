# Comparing `tmp/yls-1.3.3.tar.gz` & `tmp/yls-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yls-1.3.3.tar", max compression
+gzip compressed data, was "yls-1.3.4.tar", max compression
```

## Comparing `yls-1.3.3.tar` & `yls-1.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1082 2022-10-06 11:41:51.329876 yls-1.3.3/LICENSE
--rw-r--r--   0        0        0     1772 2022-10-06 11:41:51.329876 yls-1.3.3/LICENSE-THIRD-PARTY
--rw-r--r--   0        0        0     1844 2022-10-06 11:41:51.329876 yls-1.3.3/README.md
--rw-r--r--   0        0        0     2178 2023-03-29 10:29:12.226485 yls-1.3.3/pyproject.toml
--rw-r--r--   0        0        0       55 2022-10-06 11:41:51.365879 yls-1.3.3/yls/__init__.py
--rw-r--r--   0        0        0     4707 2023-02-02 12:50:09.230260 yls-1.3.3/yls/code_actions.py
--rw-r--r--   0        0        0     8512 2023-02-02 12:50:09.234260 yls-1.3.3/yls/completer.py
--rw-r--r--   0        0        0    14959 2023-02-02 12:50:09.234260 yls-1.3.3/yls/completion.py
--rw-r--r--   0        0        0     4294 2023-01-10 10:21:10.292138 yls-1.3.3/yls/debugger.py
--rw-r--r--   0        0        0     3070 2023-02-02 12:50:09.234260 yls-1.3.3/yls/hookspecs.py
--rw-r--r--   0        0        0     7284 2023-02-02 12:50:09.238260 yls-1.3.3/yls/hover.py
--rw-r--r--   0        0        0      101 2022-10-06 11:41:51.369880 yls-1.3.3/yls/icons.py
--rw-r--r--   0        0        0     2235 2023-02-02 12:50:09.238260 yls-1.3.3/yls/linting.py
--rw-r--r--   0        0        0     2953 2023-02-02 12:50:09.238260 yls-1.3.3/yls/plugin_manager_provider.py
--rw-r--r--   0        0        0        0 2022-10-06 11:41:51.369880 yls-1.3.3/yls/py.typed
--rw-r--r--   0        0        0    25145 2023-03-28 09:50:42.489622 yls-1.3.3/yls/server.py
--rw-r--r--   0        0        0     3682 2023-02-02 12:50:09.242260 yls-1.3.3/yls/strings.py
--rw-r--r--   0        0        0    27207 2023-02-05 12:51:18.780281 yls-1.3.3/yls/utils.py
--rw-r--r--   0        0        0       22 2023-03-29 10:29:07.722427 yls-1.3.3/yls/version.py
--rw-r--r--   0        0        0      566 2023-02-05 12:51:18.780281 yls-1.3.3/yls/yaramod_provider.py
--rw-r--r--   0        0        0     2594 1970-01-01 00:00:00.000000 yls-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-10-06 11:41:51.329876 yls-1.3.4/LICENSE
+-rw-r--r--   0        0        0     1772 2022-10-06 11:41:51.329876 yls-1.3.4/LICENSE-THIRD-PARTY
+-rw-r--r--   0        0        0     1873 2023-06-19 08:57:10.220386 yls-1.3.4/README.md
+-rw-r--r--   0        0        0     2202 2023-06-21 11:24:54.210534 yls-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0       55 2022-10-06 11:41:51.365879 yls-1.3.4/yls/__init__.py
+-rw-r--r--   0        0        0     4707 2023-03-31 16:56:48.415084 yls-1.3.4/yls/code_actions.py
+-rw-r--r--   0        0        0     8512 2023-04-03 12:54:48.417380 yls-1.3.4/yls/completer.py
+-rw-r--r--   0        0        0    14959 2023-03-31 16:56:48.419083 yls-1.3.4/yls/completion.py
+-rw-r--r--   0        0        0     4294 2023-03-31 16:56:48.419083 yls-1.3.4/yls/debugger.py
+-rw-r--r--   0        0        0     3070 2023-03-31 16:56:48.423082 yls-1.3.4/yls/hookspecs.py
+-rw-r--r--   0        0        0     7284 2023-03-31 16:56:48.423082 yls-1.3.4/yls/hover.py
+-rw-r--r--   0        0        0      101 2022-10-06 11:41:51.369880 yls-1.3.4/yls/icons.py
+-rw-r--r--   0        0        0     2235 2023-03-31 16:56:48.423082 yls-1.3.4/yls/linting.py
+-rw-r--r--   0        0        0     2953 2023-03-31 16:56:48.423082 yls-1.3.4/yls/plugin_manager_provider.py
+-rw-r--r--   0        0        0        0 2022-10-06 11:41:51.369880 yls-1.3.4/yls/py.typed
+-rw-r--r--   0        0        0    22767 2023-05-18 14:43:20.650272 yls-1.3.4/yls/server.py
+-rw-r--r--   0        0        0     3682 2023-03-31 16:56:48.427081 yls-1.3.4/yls/strings.py
+-rw-r--r--   0        0        0    27207 2023-06-21 09:50:47.849574 yls-1.3.4/yls/utils.py
+-rw-r--r--   0        0        0       22 2023-06-21 11:24:49.338504 yls-1.3.4/yls/version.py
+-rw-r--r--   0        0        0      566 2023-03-31 16:56:48.427081 yls-1.3.4/yls/yaramod_provider.py
+-rw-r--r--   0        0        0     2623 1970-01-01 00:00:00.000000 yls-1.3.4/PKG-INFO
```

### Comparing `yls-1.3.3/LICENSE` & `yls-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yls-1.3.3/LICENSE-THIRD-PARTY` & `yls-1.3.4/LICENSE-THIRD-PARTY`

 * *Files identical despite different names*

### Comparing `yls-1.3.3/README.md` & `yls-1.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - Code completion of all available modules (including function parameters)
 - Function documentation for hovers and code completion
 - Opinionated code formatting
 - Signature help
 - Linting
 - Go-to definition and references
 - Symbol highlighting under the cursor
-- Debugging? Stay tuned...
+- Debugging using [yari](https://github.com/avast/yari)
 - ...
 
 ![Showcase](https://github.com/avast/yls/raw/master/docs/assets/yls.png)
 
 For more information, check out:
 - [Blog post](https://engineering.avast.io/yls-first-step-towards-yara-development-environment/)
 - [Wiki](https://www.github.com/avast/yls/wiki)
```

### Comparing `yls-1.3.3/pyproject.toml` & `yls-1.3.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yls"
-version = "1.3.3"
+version = "1.3.4"
 description = "YARA Language Server"
 authors = ["Matej Kašťák <matej.kastak@avast.com>"]
 maintainers = ["Matej Kašťák <matej.kastak@avast.com>"]
 readme = "README.md"
 license = "MIT"
 include = ["py.typed", "LICENSE", "LICENSE-THIRD-PARTY"]
 
@@ -54,16 +54,16 @@
 test = "pytest -vvv --mypy --black --pylint --pylint-rcfile=pyproject.toml --cov=yls --cov-report=term-missing -l ./yls ./tests"
 
 [tool.poetry.scripts]
 yls = 'yls.server:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-pygls = "^1.0.0"
-yaramod = "^3.19.1"
+pygls = "^1.0.1"
+yaramod = "^3.20.1"
 yari-py = "^0.1.6"
 pluggy = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
@@ -97,9 +97,10 @@
     missing-class-docstring,
     missing-function-docstring,
     missing-module-docstring,
     no-else-return,
     redefined-outer-name,
     too-few-public-methods,
     too-many-arguments,
-    too-many-return-statements
+    too-many-return-statements,
+    wrong-import-order
     """
```

### Comparing `yls-1.3.3/yls/code_actions.py` & `yls-1.3.4/yls/code_actions.py`

 * *Files identical despite different names*

### Comparing `yls-1.3.3/yls/completer.py` & `yls-1.3.4/yls/completer.py`

 * *Files identical despite different names*

### Comparing `yls-1.3.3/yls/completion.py` & `yls-1.3.4/yls/completion.py`

 * *Files identical despite different names*

### Comparing `yls-1.3.3/yls/debugger.py` & `yls-1.3.4/yls/debugger.py`

 * *Files identical despite different names*

### Comparing `yls-1.3.3/yls/hookspecs.py` & `yls-1.3.4/yls/hookspecs.py`

 * *Files identical despite different names*

### Comparing `yls-1.3.3/yls/hover.py` & `yls-1.3.4/yls/hover.py`

 * *Files identical despite different names*

### Comparing `yls-1.3.3/yls/linting.py` & `yls-1.3.4/yls/linting.py`

 * *Files identical despite different names*

### Comparing `yls-1.3.3/yls/plugin_manager_provider.py` & `yls-1.3.4/yls/plugin_manager_provider.py`

 * *Files identical despite different names*

### Comparing `yls-1.3.3/yls/server.py` & `yls-1.3.4/yls/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from lsprotocol.types import TEXT_DOCUMENT_DID_SAVE
 from lsprotocol.types import TEXT_DOCUMENT_DOCUMENT_HIGHLIGHT
 from lsprotocol.types import TEXT_DOCUMENT_DOCUMENT_SYMBOL
 from lsprotocol.types import TEXT_DOCUMENT_FORMATTING
 from lsprotocol.types import TEXT_DOCUMENT_HOVER
 from lsprotocol.types import TEXT_DOCUMENT_REFERENCES
 from lsprotocol.types import TEXT_DOCUMENT_SIGNATURE_HELP
-from lsprotocol.types import WORKSPACE_DID_CHANGE_CONFIGURATION
 from pygls.server import LanguageServer
 from pygls.uris import from_fs_path
 
 from yls import code_actions
 from yls import icons
 from yls import linting
 from yls import utils
@@ -93,41 +92,14 @@
         commands_to_register = utils.flatten_list(
             PluginManagerProvider.instance().hook.yls_supported_commands(ls=self)
         )
         for command in commands_to_register:
             func = functools.partial(command_wrapper, command)
             self.command(command)(func)
 
-    def did_change_configuration(self) -> None:
-        """Server changed the configuration.
-
-        This function will fetch the latest configuration and set the YLS state accordingly.
-        """
-
-        def _config_callback(config: Any) -> None:
-            try:
-                conf = config[0]
-                log.debug(f"[did_change_configuration] yls configuration is: {config[0]}")
-                self.debug_hover = conf.debug.hover
-
-            except Exception as e:  # pylint: disable=broad-except
-                log.error(f"[did_change_configuration] Error occurred: {e}")
-
-        # Request the configuration from the client for "yls"
-        # FIXME: There seems to be a bug in `get_configuration` that expects a
-        # wrong type. It should be already fixed in the
-        # https://github.com/openlawlibrary/pygls/pull/310, after pygls
-        # releases a new version we can remove the `# type: ignore`
-        self.get_configuration(
-            lsp_types.WorkspaceConfigurationParams(  # type: ignore
-                items=[lsp_types.ConfigurationItem(scope_uri="", section="yls")]
-            ),
-            _config_callback,
-        )
-
     def get_current_rule(
         self, uri: str, position: lsp_types.Position, yara_file: yaramod.YaraFile | None = None
     ) -> yaramod.Rule | None:
         """Get the last defined rule for given cursor position."""
         doc_path = pathlib.Path(self.workspace.get_document(uri).path)
         log.debug(f"[GET_CURRENT_RULE] Position={position}, Document={doc_path}")
 
@@ -187,50 +159,19 @@
         self.show_message(msg, lsp_types.MessageType.Error)
 
 
 # The main YLS Server instance
 SERVER = YaraLanguageServer("yara-language-server", f"v{__version__}")
 
 
-@SERVER.feature(WORKSPACE_DID_CHANGE_CONFIGURATION)
-def did_change_configuration(ls: YaraLanguageServer, _params: Any) -> None:
-    """Configuration was changed.
-
-    This notification is somehow not being triggered. See `set_traceback` comment.
-    """
-    utils.log_command(WORKSPACE_DID_CHANGE_CONFIGURATION)
-    log.debug("[DID_CHANGE_CONFIGURATION] Configuration was changed")
-    ls.did_change_configuration()
-
-
-@SERVER.feature("$/setTraceNotification")
-def set_traceback(ls: YaraLanguageServer, params: Any) -> None:
-    """Set traceback notification.
-
-    This feature is declared manually because the pygls does not support it yet.
-    It is proposed in the 3.16 version. Params include `TraceValue` which can be
-    one of `{'off', 'message', 'verbose'}`.
-
-    Based on tests it looks like this is send in the event of configuration change
-    instead of WORKSPACE_DID_CHANGE_CONFIGURATION.
-    """
-    log.debug(
-        "[SET_TRACE_NOTIFICATION] Received setTraceNotification, "
-        "this could mean that the configuration was changed."
-    )
-    log.debug(params)
-    ls.did_change_configuration()
-
-
 @SERVER.feature(INITIALIZED)
-def initiliazed(ls: YaraLanguageServer, _params: Any) -> None:
+def initiliazed(_ls: YaraLanguageServer, _params: Any) -> None:
     """Connection is initialized."""
     utils.log_command(INITIALIZED)
     log.debug("[INITIALIZED] Connection was established")
-    ls.did_change_configuration()
     # NOTE: In the future we can parse all files in the workspace
 
 
 @SERVER.feature(TEXT_DOCUMENT_COMPLETION, lsp_types.CompletionOptions(trigger_characters=["."]))
 def completion(
     ls: YaraLanguageServer, params: lsp_types.CompletionParams
 ) -> lsp_types.CompletionList:
```

### Comparing `yls-1.3.3/yls/strings.py` & `yls-1.3.4/yls/strings.py`

 * *Files identical despite different names*

### Comparing `yls-1.3.3/yls/utils.py` & `yls-1.3.4/yls/utils.py`

 * *Files identical despite different names*

### Comparing `yls-1.3.3/yls/yaramod_provider.py` & `yls-1.3.4/yls/yaramod_provider.py`

 * *Files identical despite different names*

### Comparing `yls-1.3.3/PKG-INFO` & `yls-1.3.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: yls
-Version: 1.3.3
+Version: 1.3.4
 Summary: YARA Language Server
 License: MIT
 Author: Matej Kašťák
 Author-email: matej.kastak@avast.com
 Maintainer: Matej Kašťák
 Maintainer-email: matej.kastak@avast.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pluggy (>=1.0.0,<2.0.0)
-Requires-Dist: pygls (>=1.0.0,<2.0.0)
-Requires-Dist: yaramod (>=3.19.1,<4.0.0)
+Requires-Dist: pygls (>=1.0.1,<2.0.0)
+Requires-Dist: yaramod (>=3.20.1,<4.0.0)
 Requires-Dist: yari-py (>=0.1.6,<0.2.0)
 Description-Content-Type: text/markdown
 
 # YLS
 
 ![PyPI](https://img.shields.io/pypi/v/yls?label=yls)
 ![Visual Studio Marketplace Version](https://img.shields.io/visual-studio-marketplace/v/avast-threatlabs-yara.vscode-yls?label=vscode)
@@ -32,15 +32,15 @@
 - Code completion of all available modules (including function parameters)
 - Function documentation for hovers and code completion
 - Opinionated code formatting
 - Signature help
 - Linting
 - Go-to definition and references
 - Symbol highlighting under the cursor
-- Debugging? Stay tuned...
+- Debugging using [yari](https://github.com/avast/yari)
 - ...
 
 ![Showcase](https://github.com/avast/yls/raw/master/docs/assets/yls.png)
 
 For more information, check out:
 - [Blog post](https://engineering.avast.io/yls-first-step-towards-yara-development-environment/)
 - [Wiki](https://www.github.com/avast/yls/wiki)
```

