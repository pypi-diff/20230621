# Comparing `tmp/corallium-0.2.2.tar.gz` & `tmp/corallium-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corallium-0.2.2.tar", max compression
+gzip compressed data, was "corallium-0.3.0.tar", max compression
```

## Comparing `corallium-0.2.2.tar` & `corallium-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1066 2023-04-08 17:23:14.679517 corallium-0.2.2/LICENSE
--rw-r--r--   0        0        0      505 2023-05-17 00:04:47.972377 corallium-0.2.2/corallium/__init__.py
--rw-r--r--   0        0        0     8688 2023-04-22 15:33:16.021263 corallium-0.2.2/corallium/file_helpers.py
--rw-r--r--   0        0        0     3671 2023-02-25 15:48:42.282044 corallium-0.2.2/corallium/log.py
--rw-r--r--   0        0        0        0 2023-02-23 12:18:48.616595 corallium-0.2.2/corallium/loggers/__init__.py
--rw-r--r--   0        0        0      526 2023-04-22 04:53:47.931473 corallium-0.2.2/corallium/loggers/plain_printer.py
--rw-r--r--   0        0        0     2106 2023-05-16 23:56:42.625392 corallium-0.2.2/corallium/loggers/rich_printer.py
--rw-r--r--   0        0        0      274 2023-04-22 04:52:34.549543 corallium-0.2.2/corallium/loggers/structlog_logger/__init__.py
--rw-r--r--   0        0        0      758 2023-04-22 04:57:25.576582 corallium-0.2.2/corallium/loggers/structlog_logger/_structlog_logger.py
--rw-r--r--   0        0        0     2122 2023-02-25 16:07:54.214330 corallium-0.2.2/corallium/loggers/styles.py
--rw-r--r--   0        0        0     4486 2023-04-22 05:00:46.991583 corallium-0.2.2/corallium/pretty_process.py
--rw-r--r--   0        0        0     2493 2023-04-22 07:02:25.379564 corallium-0.2.2/corallium/shell.py
--rw-r--r--   0        0        0      192 2023-02-22 03:38:37.960591 corallium-0.2.2/corallium/tomllib.py
--rw-r--r--   0        0        0     2833 2023-05-17 00:04:53.524551 corallium-0.2.2/docs/README.md
--rw-r--r--   0        0        0     1586 2023-05-17 00:04:47.987207 corallium-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 corallium-0.2.2/setup.py
--rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 corallium-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-17 13:14:14.921090 corallium-0.3.0/LICENSE
+-rw-r--r--   0        0        0      505 2023-06-21 12:44:03.816629 corallium-0.3.0/corallium/__init__.py
+-rw-r--r--   0        0        0     8688 2023-06-21 12:24:23.679622 corallium-0.3.0/corallium/file_helpers.py
+-rw-r--r--   0        0        0     3671 2023-02-25 15:48:42.282044 corallium-0.3.0/corallium/log.py
+-rw-r--r--   0        0        0        0 2023-02-23 12:18:48.616595 corallium-0.3.0/corallium/loggers/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-21 07:55:37.168870 corallium-0.3.0/corallium/loggers/plain_printer.py
+-rw-r--r--   0        0        0     2106 2023-06-17 12:08:58.798315 corallium-0.3.0/corallium/loggers/rich_printer.py
+-rw-r--r--   0        0        0      274 2023-04-22 04:52:34.549543 corallium-0.3.0/corallium/loggers/structlog_logger/__init__.py
+-rw-r--r--   0        0        0      758 2023-04-22 04:57:25.576582 corallium-0.3.0/corallium/loggers/structlog_logger/_structlog_logger.py
+-rw-r--r--   0        0        0     2122 2023-02-25 16:07:54.214330 corallium-0.3.0/corallium/loggers/styles.py
+-rw-r--r--   0        0        0     4486 2023-06-17 12:19:52.231514 corallium-0.3.0/corallium/pretty_process.py
+-rw-r--r--   0        0        0     3734 2023-06-21 12:24:37.948419 corallium-0.3.0/corallium/shell.py
+-rw-r--r--   0        0        0      192 2023-02-22 03:38:37.960591 corallium-0.3.0/corallium/tomllib.py
+-rw-r--r--   0        0        0     2833 2023-06-21 12:44:08.312628 corallium-0.3.0/docs/README.md
+-rw-r--r--   0        0        0     1618 2023-06-21 12:44:03.827256 corallium-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3970 1970-01-01 00:00:00.000000 corallium-0.3.0/PKG-INFO
```

### Comparing `corallium-0.2.2/LICENSE` & `corallium-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corallium-0.2.2/corallium/file_helpers.py` & `corallium-0.3.0/corallium/file_helpers.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.2/corallium/log.py` & `corallium-0.3.0/corallium/log.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.2/corallium/loggers/rich_printer.py` & `corallium-0.3.0/corallium/loggers/rich_printer.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,12 +54,12 @@
         new_text.append(f': {line}', style=_styles.value_own_line)
         _console.print(new_text)
 
     if _this_level == logging.CRITICAL:
         term_width, _height = shutil.get_terminal_size((100, 50))
         _console.print_exception(
             extra_lines=1,
-            max_frames=5,
+            max_frames=6,
             show_locals=False,
             width=term_width,
         )
         # > or 'from rich.traceback import install; install(show_locals=True)'
```

### Comparing `corallium-0.2.2/corallium/loggers/structlog_logger/_structlog_logger.py` & `corallium-0.3.0/corallium/loggers/structlog_logger/_structlog_logger.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.2/corallium/loggers/styles.py` & `corallium-0.3.0/corallium/loggers/styles.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.2/corallium/pretty_process.py` & `corallium-0.3.0/corallium/pretty_process.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.2/corallium/shell.py` & `corallium-0.3.0/corallium/shell.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Run shell commands."""
 
+import asyncio
 import subprocess  # noqa: S404  # nosec
 import sys
 from io import BufferedReader
 from pathlib import Path
 from time import time
 
 from beartype import beartype
@@ -12,15 +13,15 @@
 from .log import logger
 
 
 @beartype
 def capture_shell(
     cmd: str, *, timeout: int = 120, cwd: Optional[Path] = None, printer: Optional[Callable[[str], None]] = None,
 ) -> str:
-    """Run shell command and return the output.
+    """Run shell command, return the output, and optionally print in real time.
 
     Inspired by: https://stackoverflow.com/a/38745040/3219667
 
     Args:
         cmd: shell command
         timeout: process timeout. Defaults to 2 minutes
         cwd: optional path for shell execution
@@ -57,17 +58,54 @@
 
     output = ''.join(lines)  # type: ignore[arg-type]
     if return_code != 0:
         raise subprocess.CalledProcessError(returncode=return_code or 404, cmd=cmd, output=output)
     return output
 
 
+async def _capture_shell_async(cmd: str, *, cwd: Optional[Path] = None) -> str:
+    proc = await asyncio.create_subprocess_shell(  # noqa: DUO116  # nosec  # nosemgrep
+        cmd, cwd=cwd,
+        stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
+        shell=True,  # noqa: S604
+    )
+
+    stdout, _stderr = await proc.communicate()
+    output = stdout.decode().strip()
+    if proc.returncode != 0:
+        raise subprocess.CalledProcessError(returncode=proc.returncode or 404, cmd=cmd, output=output)
+    return output
+
+
+async def capture_shell_async(cmd: str, *, timeout: int = 120, cwd: Optional[Path] = None) -> str:
+    """Run a shell command asynchronously and return the output.
+
+    ```py
+    print(asyncio.run(capture_shell_async('ls ~/.config')))
+    ```
+
+    Args:
+        cmd: shell command
+        timeout: process timeout. Defaults to 2 minutes
+        cwd: optional path for shell execution
+
+    Returns:
+        str: stripped output
+
+    Raises:
+        CalledProcessError: if return code is non-zero
+
+    """
+    logger.debug('Running', cmd=cmd, timeout=timeout, cwd=cwd)
+    return await asyncio.wait_for(_capture_shell_async(cmd=cmd, cwd=cwd), timeout=timeout)
+
+
 @beartype
 def run_shell(cmd: str, *, timeout: int = 120, cwd: Optional[Path] = None) -> None:
-    """Run shell command with buffering output.
+    """Run a shell command without capturing the output.
 
     Args:
         cmd: shell command
         timeout: process timeout. Defaults to 2 minutes
         cwd: optional path for shell execution
 
     Raises:
```

### Comparing `corallium-0.2.2/docs/README.md` & `corallium-0.3.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `corallium-0.2.2/pyproject.toml` & `corallium-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "0.2.2"
+version = "0.3.0"
 version_files = ["corallium/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
 ] # https://pypi.org/classifiers/
-description = "Shared functionality for calcipy-ecosystem"
+description = "Shared functionality for the calcipy-ecosystem"
 documentation = "https://corallium.kyleking.me"
 include = ["LICENSE"]
 keywords = []
 license = "MIT"
 maintainers = []
 name = "corallium"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/corallium"
-version = "0.2.2"
+version = "0.3.0"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
 beartype = ">=0.12.0"
 pydantic = ">=1.10.4"
 rich = ">=12.6.0"
 tomli = {markers = "python_version < '3.11'", version = ">=2.0.1"}
 
 [tool.poetry.group.dev.dependencies]
 calcipy = {extras = ["doc", "lint", "nox", "stale", "tags", "test", "types"], version = ">=1.2.4"}
+pytest-asyncio = ">=0.21.0"
 pytest-structlog = ">=0.6" # Provides pytest fixture 'log'
 pytest-subprocess = ">=1.4.1"
 structlog = ">=22.3.0"
 types-pyyaml = ">=6.0.12.8"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/kyleking/corallium/issues"
```

### Comparing `corallium-0.2.2/setup.py` & `corallium-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,94 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: corallium
+Version: 0.3.0
+Summary: Shared functionality for the calcipy-ecosystem
+Home-page: https://github.com/kyleking/corallium
+License: MIT
+Author: Kyle King
+Author-email: dev.act.kyle@gmail.com
+Requires-Python: >=3.8.12,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: beartype (>=0.12.0)
+Requires-Dist: pydantic (>=1.10.4)
+Requires-Dist: rich (>=12.6.0)
+Requires-Dist: tomli (>=2.0.1) ; python_version < "3.11"
+Project-URL: Bug Tracker, https://github.com/kyleking/corallium/issues
+Project-URL: Changelog, https://github.com/kyleking/corallium/blob/main/docs/docs/CHANGELOG.md
+Project-URL: Documentation, https://corallium.kyleking.me
+Project-URL: Repository, https://github.com/kyleking/corallium
+Description-Content-Type: text/markdown
 
-packages = \
-['corallium', 'corallium.loggers', 'corallium.loggers.structlog_logger']
+# corallium
 
-package_data = \
-{'': ['*']}
+Shared functionality for the calcipy-ecosystem.
 
-install_requires = \
-['beartype>=0.12.0', 'pydantic>=1.10.4', 'rich>=12.6.0']
-
-extras_require = \
-{':python_version < "3.11"': ['tomli>=2.0.1']}
-
-setup_kwargs = {
-    'name': 'corallium',
-    'version': '0.2.2',
-    'description': 'Shared functionality for calcipy-ecosystem',
-    'long_description': '# corallium\n\nShared functionality for the calcipy-ecosystem.\n\n## Installation\n\n1. `poetry add corallium`\n\n1. Take advantage of the logger or other common functionality\n\n    ```sh\n    form corallium.log import logger\n\n    logger.info(\'Hello!\')\n    ```\n\n## Usage\n\n<!-- < TODO: Show an example (screenshots, terminal recording, etc.) >\n\n- **log**: TBD\n- **pretty_process**: TBD\n- **shell**: TBD\n- **file_helpers**: TBD\n- **tomllib**: This is a lightweight wrapper to backport `tomli` in place of `tomllib` until we can use Python >3.11. Use with `from corallium.tomllib import tomllib`\n- **dot_dict**: has one function `ddict`, which is a light-weight wrapper around whatever is the most [maintained dotted-dictionary package in Python](https://pypi.org/search/?q=dot+accessible+dictionary&o=). Dotted dictionaries can sometimes improve code readability, but they aren\'t a one-size fits all solution. Sometimes `attr.s` or `dataclass` are more appropriate.\n    - The benefit of this wrapper is a stable interface that can be replaced with better internal implementations, such [Bunch](https://pypi.org/project/bunch/), [Chunk](https://pypi.org/project/chunk/), [Munch](https://pypi.org/project/munch/), [flexible-dotdict](https://pypi.org/project/flexible-dotdict/), [classy-json](https://pypi.org/project/classy-json/), and now [Python-Box](https://pypi.org/project/python-box/)\n -->\n\nFor more example code, see the [scripts] directory or the [tests].\n\n## Project Status\n\nSee the `Open Issues` and/or the [CODE_TAG_SUMMARY]. For release history, see the [CHANGELOG].\n\n## Contributing\n\nWe welcome pull requests! For your pull request to be accepted smoothly, we suggest that you first open a GitHub issue to discuss your idea. For resources on getting started with the code base, see the below documentation:\n\n- [DEVELOPER_GUIDE]\n- [STYLE_GUIDE]\n\n## Code of Conduct\n\nWe follow the [Contributor Covenant Code of Conduct][contributor-covenant].\n\n### Open Source Status\n\nWe try to reasonably meet most aspects of the "OpenSSF scorecard" from [Open Source Insights](https://deps.dev/pypi/corallium)\n\n## Responsible Disclosure\n\nIf you have any security issue to report, please contact the project maintainers privately. You can reach us at [dev.act.kyle@gmail.com](mailto:dev.act.kyle@gmail.com).\n\n## License\n\n[LICENSE]\n\n[changelog]: https://corallium.kyleking.me/docs/CHANGELOG\n[code_tag_summary]: https://corallium.kyleking.me/docs/CODE_TAG_SUMMARY\n[contributor-covenant]: https://www.contributor-covenant.org\n[developer_guide]: https://corallium.kyleking.me/docs/DEVELOPER_GUIDE\n[license]: https://github.com/kyleking/corallium/blob/main/LICENSE\n[scripts]: https://github.com/kyleking/corallium/blob/main/scripts\n[style_guide]: https://corallium.kyleking.me/docs/STYLE_GUIDE\n[tests]: https://github.com/kyleking/corallium/blob/main/tests\n',
-    'author': 'Kyle King',
-    'author_email': 'dev.act.kyle@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/kyleking/corallium',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8.12,<4.0.0',
-}
+## Installation
 
+1. `poetry add corallium`
+
+1. Take advantage of the logger or other common functionality
+
+    ```sh
+    form corallium.log import logger
+
+    logger.info('Hello!')
+    ```
+
+## Usage
+
+<!-- < TODO: Show an example (screenshots, terminal recording, etc.) >
+
+- **log**: TBD
+- **pretty_process**: TBD
+- **shell**: TBD
+- **file_helpers**: TBD
+- **tomllib**: This is a lightweight wrapper to backport `tomli` in place of `tomllib` until we can use Python >3.11. Use with `from corallium.tomllib import tomllib`
+- **dot_dict**: has one function `ddict`, which is a light-weight wrapper around whatever is the most [maintained dotted-dictionary package in Python](https://pypi.org/search/?q=dot+accessible+dictionary&o=). Dotted dictionaries can sometimes improve code readability, but they aren't a one-size fits all solution. Sometimes `attr.s` or `dataclass` are more appropriate.
+    - The benefit of this wrapper is a stable interface that can be replaced with better internal implementations, such [Bunch](https://pypi.org/project/bunch/), [Chunk](https://pypi.org/project/chunk/), [Munch](https://pypi.org/project/munch/), [flexible-dotdict](https://pypi.org/project/flexible-dotdict/), [classy-json](https://pypi.org/project/classy-json/), and now [Python-Box](https://pypi.org/project/python-box/)
+ -->
+
+For more example code, see the [scripts] directory or the [tests].
+
+## Project Status
+
+See the `Open Issues` and/or the [CODE_TAG_SUMMARY]. For release history, see the [CHANGELOG].
+
+## Contributing
+
+We welcome pull requests! For your pull request to be accepted smoothly, we suggest that you first open a GitHub issue to discuss your idea. For resources on getting started with the code base, see the below documentation:
+
+- [DEVELOPER_GUIDE]
+- [STYLE_GUIDE]
+
+## Code of Conduct
+
+We follow the [Contributor Covenant Code of Conduct][contributor-covenant].
+
+### Open Source Status
+
+We try to reasonably meet most aspects of the "OpenSSF scorecard" from [Open Source Insights](https://deps.dev/pypi/corallium)
+
+## Responsible Disclosure
+
+If you have any security issue to report, please contact the project maintainers privately. You can reach us at [dev.act.kyle@gmail.com](mailto:dev.act.kyle@gmail.com).
+
+## License
+
+[LICENSE]
+
+[changelog]: https://corallium.kyleking.me/docs/CHANGELOG
+[code_tag_summary]: https://corallium.kyleking.me/docs/CODE_TAG_SUMMARY
+[contributor-covenant]: https://www.contributor-covenant.org
+[developer_guide]: https://corallium.kyleking.me/docs/DEVELOPER_GUIDE
+[license]: https://github.com/kyleking/corallium/blob/main/LICENSE
+[scripts]: https://github.com/kyleking/corallium/blob/main/scripts
+[style_guide]: https://corallium.kyleking.me/docs/STYLE_GUIDE
+[tests]: https://github.com/kyleking/corallium/blob/main/tests
 
-setup(**setup_kwargs)
```

