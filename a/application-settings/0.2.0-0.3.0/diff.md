# Comparing `tmp/application_settings-0.2.0.tar.gz` & `tmp/application_settings-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "application_settings-0.2.0.tar", max compression
+gzip compressed data, was "application_settings-0.3.0.tar", max compression
```

## Comparing `application_settings-0.2.0.tar` & `application_settings-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,22 @@
--rw-r--r--   0        0        0     1024 2023-03-19 20:52:11.085558 application_settings-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1141 2023-03-12 20:42:18.008107 application_settings-0.2.0/LICENSE
--rw-r--r--   0        0        0     3911 2023-03-19 20:48:37.336181 application_settings-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2847 2023-03-19 20:51:54.576438 application_settings-0.2.0/README.md
--rw-r--r--   0        0        0      634 2023-03-19 20:48:37.336181 application_settings-0.2.0/src/application_settings/__init__.py
--rw-r--r--   0        0        0     1030 2023-03-19 20:48:37.339165 application_settings-0.2.0/src/application_settings/configuring_base.py
--rw-r--r--   0        0        0     8791 2023-03-19 20:48:37.340288 application_settings-0.2.0/src/application_settings/container_base.py
--rw-r--r--   0        0        0       49 2023-03-12 20:42:18.042930 application_settings-0.2.0/src/application_settings/py.typed
--rw-r--r--   0        0        0      748 2023-03-19 20:48:37.342091 application_settings-0.2.0/src/application_settings/settings_base.py
--rw-r--r--   0        0        0      510 2023-03-19 20:48:37.342309 application_settings-0.2.0/src/application_settings/type_notation_helper.py
--rw-r--r--   0        0        0        0 2023-03-12 20:42:18.050944 application_settings-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     8356 2023-03-19 20:48:37.345170 application_settings-0.2.0/tests/test_config.py
--rw-r--r--   0        0        0     4580 2023-03-19 20:48:37.345521 application_settings-0.2.0/tests/test_settings.py
--rw-r--r--   0        0        0     3802 1970-01-01 00:00:00.000000 application_settings-0.2.0/setup.py
--rw-r--r--   0        0        0     4144 1970-01-01 00:00:00.000000 application_settings-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2491 2023-06-21 18:14:52.102528 application_settings-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      198 2023-06-18 19:26:50.645813 application_settings-0.3.0/examples/Quick_start/config.toml
+-rw-r--r--   0        0        0     2927 2023-06-18 19:26:50.645813 application_settings-0.3.0/examples/Quick_start/example_configuring.py
+-rw-r--r--   0        0        0     2995 2023-06-18 19:58:54.362331 application_settings-0.3.0/examples/Quick_start/example_settings.py
+-rw-r--r--   0        0        0       52 2023-06-18 19:26:50.655146 application_settings-0.3.0/examples/Quick_start/settings.json
+-rw-r--r--   0        0        0     1141 2023-05-30 19:59:15.162814 application_settings-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5297 2023-06-18 19:58:54.266122 application_settings-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2912 2023-06-21 18:16:32.945163 application_settings-0.3.0/README.md
+-rw-r--r--   0        0        0      989 2023-06-18 19:58:54.370331 application_settings-0.3.0/src/application_settings/__init__.py
+-rw-r--r--   0        0        0     1415 2023-06-20 19:53:57.488717 application_settings-0.3.0/src/application_settings/configuring_base.py
+-rw-r--r--   0        0        0     6203 2023-06-20 19:53:57.496022 application_settings-0.3.0/src/application_settings/container_base.py
+-rw-r--r--   0        0        0     3072 2023-06-20 19:53:57.496022 application_settings-0.3.0/src/application_settings/container_section_base.py
+-rw-r--r--   0        0        0     3789 2023-06-20 20:00:06.394710 application_settings-0.3.0/src/application_settings/convenience.py
+-rw-r--r--   0        0        0       49 2023-05-30 19:59:15.224540 application_settings-0.3.0/src/application_settings/py.typed
+-rw-r--r--   0        0        0     1084 2023-06-20 19:53:57.496022 application_settings-0.3.0/src/application_settings/settings_base.py
+-rw-r--r--   0        0        0      524 2023-06-20 19:53:57.496022 application_settings-0.3.0/src/application_settings/type_notation_helper.py
+-rw-r--r--   0        0        0        0 2023-05-30 19:59:15.224540 application_settings-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0    11396 2023-06-20 18:54:19.025427 application_settings-0.3.0/tests/test_config.py
+-rw-r--r--   0        0        0     8080 2023-06-18 19:58:54.370331 application_settings-0.3.0/tests/test_settings.py
+-rw-r--r--   0        0        0      206 2023-06-18 19:26:50.687562 application_settings-0.3.0/tests/test_version.py
+-rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 application_settings-0.3.0/setup.py
+-rw-r--r--   0        0        0     4284 1970-01-01 00:00:00.000000 application_settings-0.3.0/PKG-INFO
```

### Comparing `application_settings-0.2.0/LICENSE` & `application_settings-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `application_settings-0.2.0/pyproject.toml` & `application_settings-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "application_settings"
-version = "0.2.0"
+version = "0.3.0"
 description = "For providing a python application with configuration and/or settings"
 authors = ["Stockwatchdevs <stockwatchdevs@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/StockwatchDev/application_settings"
 repository = "https://github.com/StockwatchDev/application_settings"
 keywords = ["configuration", "settings", "dataclass", "pydantic", "toml"]
@@ -21,36 +21,39 @@
     "Typing :: Typed",
 ]
 include = [
     { path = "CHANGELOG.md" },
     { path = "LICENSE" },
     { path = "README.md" },
     { path = "tests", format = "sdist" },
+    { path = "examples", format = "sdist" },
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pathvalidate = "^2.5"
+pathvalidate = ">=2.5,<4.0"
 pydantic = "^1.10"
 tomli = { version = "^2.0", python = "<3.11" }
 tomli-w = "^1.0"
+typing-extensions = { version = "^4.5.0", python = "<3.11" }
 
 [tool.poetry.group.testing]
 optional = true
 
 [tool.poetry.group.testing.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.0"
 
 [tool.poetry.group.typing]
 optional = true
 
 [tool.poetry.group.typing.dependencies]
-mypy = ">=0.942"
+mypy = "^1.1"
+lxml = "^4.9"
 
 [tool.poetry.group.style]
 optional = true
 
 [tool.poetry.group.style.dependencies]
 black = ">=22.10,<24.0"
 isort = "^5.12"
@@ -58,14 +61,20 @@
 
 [tool.poetry.group.testrunner]
 optional = true
 
 [tool.poetry.group.testrunner.dependencies]
 tox = "^4.4"
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+portray = "^1.8"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
@@ -118,22 +127,66 @@
 
 [tool.pylint.typing]
 runtime-typing = false
 
 [tool.pylint.similarities]
 ignore-imports = "yes"
 
+[tool.portray.mkdocs]
+markdown_extensions = [
+    "pymdownx.highlight",
+    "pymdownx.superfences",
+    "pymdownx.tabbed",
+]
+
+[[tool.portray.extra_markdown_extensions]]
+[tool.portray.extra_markdown_extensions."pymdownx.tabbed"]
+alternate_style = true
+
+[tool.portray.mkdocs.theme]
+name = "material"
+palette = { scheme = "slate", primary = "blue" }
+
+[[tool.portray.mkdocs.nav]]
+Home = "README.md"
+
+[[tool.portray.mkdocs.nav]]
+"Quick start" = "docs/Quick_start.md"
+
+[[tool.portray.mkdocs.nav]]
+[[tool.portray.mkdocs.nav.Usage]]
+"1. Installation" = "docs/1-Installation.md"
+
+[[tool.portray.mkdocs.nav.Usage]]
+"2. Defining parameters" = "docs/2-Defining_parameters.md"
+
+[[tool.portray.mkdocs.nav.Usage]]
+"3. Files and file location" = "docs/3-Files.md"
+
+[[tool.portray.mkdocs.nav.Usage]]
+"4. Using parameters" = "docs/4-Using_parameters.md"
+
+[[tool.portray.mkdocs.nav.Usage]]
+"5. Usage in a library package" = "docs/5-Usage_in_a_library_package.md"
+
+[[tool.portray.mkdocs.nav.Usage]]
+"6. Handling deviations" = "docs/6-Handling_deviations.md"
+
+[[tool.portray.mkdocs.nav]]
+Changelog = "CHANGELOG.md"
+
+
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = true
 envlist =
     py{39,310,311}
     style
-    typing
+    py{39,310,311}-typing
 
 [testenv]
 allowlist_externals = poetry
 commands_pre =
     poetry install --no-root --with testing -v
 commands =
     poetry run pytest --cov-report xml:coverage.xml --cov-report term-missing --cov=application_settings tests/ --import-mode importlib
@@ -141,16 +194,16 @@
 [testenv:style]
 skip_install = true
 commands_pre =
     poetry install --with style -v
 commands =
     poetry run python -m black --check ./src
     poetry run isort --check --diff ./src
-    poetry run pylint --recursive=y ./src
+    poetry run pylint ./src
 
-[testenv:typing]
+[testenv:py{39,310,311}-typing]
 skip_install = true
 commands_pre =
     poetry install --with typing -v
 commands =
     poetry run mypy ./src
 """
```

### Comparing `application_settings-0.2.0/README.md` & `application_settings-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# application_settings
+# application_settings - version 0.3.0
 
 [![pypi](https://img.shields.io/pypi/v/application-settings.svg)](https://pypi.python.org/pypi/application-settings)
 [![versions](https://img.shields.io/pypi/pyversions/application-settings.svg)](https://github.com/StockwatchDev/application_settings)
-[![Build Status](https://github.com/StockwatchDev/application_settings/actions/workflows/application_settings-tests.yml/badge.svg?branch=develop)](https://github.com/StockwatchDev/application_settings/actions)
+[![Build Status](https://github.com/StockwatchDev/application_settings/actions/workflows/merge_checks.yml/badge.svg?branch=develop)](https://github.com/StockwatchDev/application_settings/actions)
 [![codecov](https://codecov.io/gh/StockwatchDev/application_settings/branch/develop/graph/badge.svg)](https://app.codecov.io/gh/StockwatchDev/application_settings)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 "You write the dataclasses to define parameters for configuration and settings, 
 application\_settings takes care of the logic."
 
 ## What and why
 
-Application\_settings is a package for providing a python application with parameters for
-configuration and settings. It uses [toml](https://toml.io/en/) or 
+Application\_settings is a package for providing a python application or library with
+parameters for configuration and settings. It uses [toml](https://toml.io/en/) or 
 [json](https://www.json.org/) files that are parsed
 into dataclasses. This brings some benefits:
 
-- Minimal work for the application designer
+- Minimal work for the developer of the application / library
 - Parameters are typed, which allows for improved static code analyses.
 - IDEs will provide helpful hints and completion when using the parameters.
 - More control over what happens when a file contains mistakes
   (by leveraging the power of [pydantic](https://docs.pydantic.dev/)).
 - Possibility to specify defaults when no file is found or entries are missing.
 - Configuration parameters are read-only (i.e., changed by editing the config file); we
   recommend (and support) the use of `toml` for this, which is a human-oriented,
   flexible, standardardized and not overly complex format.
 - Settings parameters are read-write (i.e., mostly changed via the UI of the
   application); we recommend (and support) use `json` for this, an established
   standardized machine-oriented format.
 
-Parsing is done once during first access and the resulting set of parameters is stored
-as a singleton.
+Parsing is done once before or during first access and the resulting set of parameters is
+stored as a singleton.
 
 Interested? Then have a look at our
-[quick start](https://stockwatchdev.github.io/application_settings/0.2.0/docs/Quick_start/).
+[quick start](https://stockwatchdev.github.io/application_settings/0.3.0/docs/Quick_start/).
 
-[//]: # (Change link to published quick start)
+[//]: # (Change version in header and link to published quick start)
 
 ## License
 
-This project is licensed under the terms of the MIT license.
+This project is licensed under the terms of the MIT license.
```

### Comparing `application_settings-0.2.0/src/application_settings/configuring_base.py` & `application_settings-0.3.0/src/application_settings/configuring_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 """Module for handling configuration."""
 from typing import Any, TypeVar
 
 from pydantic.dataclasses import dataclass
 
-from .container_base import ContainerBase, ContainerSectionBase, ContainerTypeStr
+from application_settings.container_base import ContainerBase, FileFormat
+from application_settings.container_section_base import (
+    ContainerSectionBase,
+    SectionTypeStr,
+)
 
 ConfigT = TypeVar("ConfigT", bound="ConfigBase")
-ConfigSectionT = TypeVar("ConfigSectionT", bound="ConfigSectionBase")
+ConfigT.__doc__ = "Represents ConfigBase and all subclasses"
 
 
 @dataclass(frozen=True)
 class ConfigSectionBase(ContainerSectionBase):
     """Base class for all ConfigSection classes (so that we can bound a TypeVar)"""
 
+    @classmethod
+    def kind_string(cls) -> SectionTypeStr:
+        "Return 'Config'"
+        return "Config"
+
 
 @dataclass(frozen=True)
 class ConfigBase(ContainerBase):
     """Base class for main Config class"""
 
     @classmethod
-    def kind_string(cls: type[ConfigT]) -> ContainerTypeStr:
+    def kind_string(cls) -> SectionTypeStr:
         "Return 'Config'"
         return "Config"
 
-    def update(self: ConfigT, changes: dict[str, dict[str, Any]]) -> ConfigT:
+    @classmethod
+    def default_file_format(cls) -> FileFormat:
+        "Return the default file format"
+        return FileFormat.TOML
+
+    @classmethod
+    def update(
+        cls: type["ConfigBase"], changes: dict[str, dict[str, Any]]
+    ) -> "ConfigBase":
         "Update and save the settings with data specified in changes; not meant for config"
         raise TypeError(
             "Configs should not be updated runtime; consider converting to settings."
         )
```

### Comparing `application_settings-0.2.0/src/application_settings/settings_base.py` & `application_settings-0.3.0/src/application_settings/settings_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 """Module for handling settings."""
 from typing import TypeVar
 
 from pydantic.dataclasses import dataclass
 
-from .container_base import ContainerBase, ContainerSectionBase, ContainerTypeStr
+from application_settings.container_base import ContainerBase, FileFormat
+from application_settings.container_section_base import (
+    ContainerSectionBase,
+    SectionTypeStr,
+)
 
 SettingsT = TypeVar("SettingsT", bound="SettingsBase")
-SettingsSectionT = TypeVar("SettingsSectionT", bound="SettingsSectionBase")
+SettingsT.__doc__ = "Represents SettingsBase and all subclasses"
 
 
 @dataclass(frozen=True)
 class SettingsSectionBase(ContainerSectionBase):
     """Base class for all SettingsSection classes (so that we can bound a TypeVar)"""
 
+    @classmethod
+    def kind_string(cls) -> SectionTypeStr:
+        "Return 'Settings'"
+        return "Settings"
+
 
 @dataclass(frozen=True)
 class SettingsBase(ContainerBase):
     """Base class for main Settings class"""
 
     @classmethod
-    def kind_string(cls: type[SettingsT]) -> ContainerTypeStr:
+    def kind_string(cls) -> SectionTypeStr:
         "Return 'Settings'"
         return "Settings"
+
+    @classmethod
+    def default_file_format(cls) -> FileFormat:
+        "Return the default file format"
+        return FileFormat.JSON
```

### Comparing `application_settings-0.2.0/tests/test_config.py` & `application_settings-0.3.0/tests/test_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,130 @@
 # pylint: disable=missing-module-docstring
 # pylint: disable=missing-function-docstring
-# pylint: disable=consider-alternative-union-syntax
 # pylint: disable=redefined-outer-name
 import json
 import sys
 from pathlib import Path
 from typing import Any
 
 import pytest
 import tomli_w
 from pydantic import ValidationError
 from pydantic.dataclasses import dataclass
 
-from application_settings import ConfigBase, ConfigSectionBase, PathOpt, __version__
+from application_settings import (
+    ConfigBase,
+    ConfigSectionBase,
+    PathOpt,
+    __version__,
+    config_filepath_from_cli,
+)
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
 
 
 @dataclass(frozen=True)
+class AnExampleConfigSubSection(ConfigSectionBase):
+    """Example of a Config subsection"""
+
+    field3: tuple[int, str] = (3, "yes")
+
+
+@dataclass(frozen=True)
 class AnExample1ConfigSection(ConfigSectionBase):
     """Example 1 of a Config section"""
 
     field1: str = "field1"
     field2: int = 2
+    subsec: AnExampleConfigSubSection = AnExampleConfigSubSection()
 
 
 @dataclass(frozen=True)
 class AnExample1Config(ConfigBase):
     """Example Config"""
 
+    field0: float = 2.2
     section1: AnExample1ConfigSection = AnExample1ConfigSection()
 
 
+@dataclass(frozen=True)
+class Config(ConfigBase):
+    """Config class def"""
+
+
 @pytest.fixture(scope="session")
 def toml_file(tmp_path_factory: pytest.TempPathFactory) -> Path:
     file_path = (
         tmp_path_factory.mktemp(AnExample1Config.default_foldername())
         / AnExample1Config.default_filename()
     )
     with file_path.open(mode="wb") as fptr:
-        tomli_w.dump({"section1": {"field1": "f1", "field2": 22}}, fptr)
+        tomli_w.dump(
+            {
+                "field0": 33.33,
+                "section1": {
+                    "field1": "f1",
+                    "field2": 22,
+                    "subsec": {"field3": (-3, "no")},
+                },
+            },
+            fptr,
+        )
     return file_path
 
 
 @pytest.fixture(scope="session")
 def json_file(tmp_path_factory: pytest.TempPathFactory) -> Path:
     file_path = tmp_path_factory.mktemp(
         AnExample1Config.default_foldername()
     ) / AnExample1Config.default_filename().replace("toml", "json")
     with file_path.open(mode="w") as fptr:
-        json.dump({"section1": {"field1": "f2", "field2": 33}}, fptr)
+        json.dump(
+            {
+                "section1": {
+                    "field1": "f2",
+                    "field2": 33,
+                    "subsec": {"field3": (-4, "maybe")},
+                }
+            },
+            fptr,
+        )
     return file_path
 
 
 @pytest.fixture(scope="session")
 def ini_file(tmp_path_factory: pytest.TempPathFactory) -> Path:
     file_path = tmp_path_factory.mktemp(
         AnExample1Config.default_foldername()
     ) / AnExample1Config.default_filename().replace("toml", "ini")
     with file_path.open(mode="w") as fptr:
         fptr.write("inifile")
     return file_path
 
 
-def test_version() -> None:
-    assert __version__ == "0.2.0"
+def test_kind_string() -> None:
+    assert AnExample1ConfigSection.kind_string() == "Config"
+
+
+def test_section_singleton(capfd: pytest.CaptureFixture[str]) -> None:
+    assert AnExample1ConfigSection.get().field1 == "field1"
+    captured = capfd.readouterr()
+    assert " accessed before data has been set by the application." in captured.out
 
 
 def test_paths(toml_file: Path) -> None:
     # default_filepath:
+    if the_path := Config.default_filepath():
+        assert the_path.parts[-2] == ".config"
+    else:
+        assert False
+
     if the_path := AnExample1Config.default_filepath():
         assert the_path.parts[-1] == "config.toml"
         assert the_path.parts[-2] == ".an_example1"
     else:
         assert False
 
     # filepath:
@@ -90,96 +139,137 @@
 
     # reset to default:
     AnExample1Config.set_filepath("")
     assert AnExample1Config.filepath() == the_path
 
     # raising of FileNotFoundError:
     with pytest.raises(FileNotFoundError):
-        _ = AnExample1Config.get().section1.field1
+        AnExample1Config.load(throw_if_file_not_found=True)
 
+    AnExample1Config.set_filepath(
+        str(Path.home() / "ProgramData" / "test" / "config.toml")
+    )
     # raising in case of invalid path:
     with pytest.raises(ValueError):
         AnExample1Config.set_filepath('fi:\0\\l*e/p"a?t>h|.t<xt')
 
 
+def test_config_cmdline(monkeypatch: pytest.MonkeyPatch) -> None:
+    # test without commandline arguments
+    # - this works, but not together with the last 4 lines
+    # monkeypatch.setattr(sys, "argv", ["bla"])
+    # config_filepath_from_cli(Config, short_option="-k")
+    # assert Config.filepath() == Config.default_filepath()
+    some_path = Path.home() / "ProgramData" / "test" / "config.toml"
+    monkeypatch.setattr(sys, "argv", ["bla", "-k", str(some_path)])
+    config_filepath_from_cli(AnExample1Config, short_option="-k")
+    assert str(AnExample1Config.filepath()) == str(some_path)
+
+
 def test_get_defaults(
     monkeypatch: pytest.MonkeyPatch, capfd: pytest.CaptureFixture[str]
 ) -> None:
     def mock_default_filepath() -> PathOpt:
         return None
 
     monkeypatch.setattr(AnExample1Config, "default_filepath", mock_default_filepath)
-    AnExample1Config.set_filepath("")
-    assert AnExample1Config.get(reload=True).section1.field1 == "field1"
+    AnExample1Config.set_filepath("", load=True)
+    assert AnExample1Config.get().section1.field1 == "field1"
+    AnExample1Config.set_filepath("", load=True)
     assert AnExample1Config.get().section1.field2 == 2
+    assert AnExample1Config.get().section1.subsec.field3[1] == "yes"
     captured = capfd.readouterr()
     assert (
-        "No path specified for config file; trying with defaults, but this may not work."
+        "Path None not valid for config file. Trying with defaults, but this may not work."
         in captured.out
     )
+    # raising of FileNotFoundError:
+    with pytest.raises(FileNotFoundError):
+        AnExample1Config.load(throw_if_file_not_found=True)
+
+
+def test_set_filepath_after_get(
+    toml_file: Path, capfd: pytest.CaptureFixture[str]
+) -> None:
+    AnExample1Config.set_filepath(toml_file, load=True)
+    assert AnExample1Config.get().section1.field1 == "f1"
+    assert AnExample1Config.get().section1.subsec.field3[1] == "no"
+    # test if the subsection singleton is properly registered
+    assert AnExampleConfigSubSection.get().field3[1] == "no"
+    AnExample1Config.set_filepath("", load=False)
+    captured = capfd.readouterr()
+    assert "file is not loaded into the Config." in captured.out
 
 
 def test_get(monkeypatch: pytest.MonkeyPatch, toml_file: Path) -> None:
     AnExample1Config.set_filepath(toml_file)
-    assert AnExample1Config.get(reload=True).section1.field1 == "f1"
+    AnExample1Config.load()
+    assert AnExample1Config.get().field0 == 33.33
+    assert AnExample1Config.get().section1.field1 == "f1"
     assert AnExample1Config.get().section1.field2 == 22
 
     # test that by default it is not reloaded
     def mock_tomllib_load(
         fptr: Any,  # pylint: disable=unused-argument
     ) -> dict[str, dict[str, Any]]:
         return {"section1": {"field1": "f1", "field2": 222}}
 
     monkeypatch.setattr(tomllib, "load", mock_tomllib_load)
     assert AnExample1Config.get().section1.field2 == 22
 
     # and now test reload
-    assert AnExample1Config.get(reload=True).section1.field2 == 222
+    AnExample1Config.load()
+    assert AnExample1Config.get().field0 == 2.2
+    assert AnExample1Config.get().section1.field2 == 222
 
 
 def test_get_json(json_file: Path) -> None:
     AnExample1Config.set_filepath(json_file)
-    assert AnExample1Config.get(reload=True).section1.field1 == "f2"
+    AnExample1Config.load()
+    assert AnExample1Config.get().section1.field1 == "f2"
     assert AnExample1Config.get().section1.field2 == 33
 
 
 def test_get_ini(ini_file: Path, capfd: pytest.CaptureFixture[str]) -> None:
     AnExample1Config.set_filepath(ini_file)
-    assert AnExample1Config.get(reload=True).section1.field1 == "field1"
+    AnExample1Config.load()
+    assert AnExample1Config.get().section1.field1 == "field1"
     assert AnExample1Config.get().section1.field2 == 2
     captured = capfd.readouterr()
     assert "Unknown file format ini given in" in captured.out
 
 
 def test_type_coercion(monkeypatch: pytest.MonkeyPatch, toml_file: Path) -> None:
     def mock_tomllib_load(
         fptr: Any,  # pylint: disable=unused-argument
     ) -> dict[str, dict[str, Any]]:
         return {"section1": {"field1": True, "field2": "22"}}
 
     monkeypatch.setattr(tomllib, "load", mock_tomllib_load)
     AnExample1Config.set_filepath(toml_file)
-    test_config = AnExample1Config.get(reload=True)
+    AnExample1Config.load()
+    test_config = AnExample1Config.get()
     assert isinstance(test_config.section1.field1, str)
     assert test_config.section1.field1 == "True"
     assert isinstance(test_config.section1.field2, int)
     assert test_config.section1.field2 == 22
 
 
 def test_wrong_type(monkeypatch: pytest.MonkeyPatch, toml_file: Path) -> None:
     def mock_tomllib_load(
         fptr: Any,  # pylint: disable=unused-argument
     ) -> dict[str, dict[str, Any]]:
-        return {"section1": {"field1": ("f1", 22), "field2": None}}  # type: ignore
+        return {"section1": {"field1": ("f1", 22), "field2": None}}
 
     monkeypatch.setattr(tomllib, "load", mock_tomllib_load)
 
     AnExample1Config.set_filepath(toml_file)
     with pytest.raises(ValidationError) as excinfo:
-        _ = AnExample1Config.get(reload=True)
+        AnExample1Config.load()
+        _ = AnExample1Config.get()
     assert "2 validation errors" in str(excinfo.value)
     assert "str type expected" in str(excinfo.value)
     assert "none is not an allowed value" in str(excinfo.value)
 
 
 def test_missing_extra_attributes(
     monkeypatch: pytest.MonkeyPatch, toml_file: Path
@@ -188,15 +278,16 @@
         fptr: Any,  # pylint: disable=unused-argument
     ) -> dict[str, dict[str, Any]]:
         return {"section1": {"field1": "f1", "field3": 22}}
 
     monkeypatch.setattr(tomllib, "load", mock_tomllib_load)
 
     AnExample1Config.set_filepath(toml_file)
-    test_config = AnExample1Config.get(reload=True)
+    AnExample1Config.load()
+    test_config = AnExample1Config.get()
     assert test_config.section1.field2 == 2
     with pytest.raises(AttributeError):
         assert test_config.section1.field3 == 22  # type: ignore[attr-defined]
 
 
 @dataclass(frozen=True)
 class Example2aConfigSection(ConfigSectionBase):
@@ -222,28 +313,31 @@
     section2: Example2bConfigSection = Example2bConfigSection()
 
 
 def test_attributes_no_default(
     monkeypatch: pytest.MonkeyPatch, toml_file: Path
 ) -> None:
     Example2Config.set_filepath(toml_file)
-    with pytest.raises(TypeError):
-        _ = Example2Config.get(reload=True)
+    with pytest.raises(ValidationError):
+        AnExample1Config.load()
+        _ = Example2Config.get()
 
     def mock_tomllib_load2(
         fptr: Any,  # pylint: disable=unused-argument
     ) -> dict[str, dict[str, float]]:
         return {"section1": {"field3": 1.1}}
 
     monkeypatch.setattr(tomllib, "load", mock_tomllib_load2)
 
-    test_config = Example2Config.get(reload=True)
+    AnExample1Config.load()
+    test_config = Example2Config.get()
     assert test_config.section1.field3 == 1.1
     assert test_config.section1.field4 == 0.5
     assert test_config.section2.field1 == "field1"
 
 
 def test_update() -> None:
     with pytest.raises(TypeError):
+        # a Config cannot be updated
         _ = AnExample1Config.get().update(
             {"section1": {"setting1": "new s1", "setting2": 222}}
         )
```

### Comparing `application_settings-0.2.0/setup.py` & `application_settings-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 packages = \
 ['application_settings']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pathvalidate>=2.5,<3.0', 'pydantic>=1.10,<2.0', 'tomli-w>=1.0,<2.0']
+['pathvalidate>=2.5,<4.0', 'pydantic>=1.10,<2.0', 'tomli-w>=1.0,<2.0']
 
 extras_require = \
-{':python_version < "3.11"': ['tomli>=2.0,<3.0']}
+{':python_version < "3.11"': ['tomli>=2.0,<3.0',
+                              'typing-extensions>=4.5.0,<5.0.0']}
 
 setup_kwargs = {
     'name': 'application-settings',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'For providing a python application with configuration and/or settings',
-    'long_description': '# application_settings\n\n[![pypi](https://img.shields.io/pypi/v/application-settings.svg)](https://pypi.python.org/pypi/application-settings)\n[![versions](https://img.shields.io/pypi/pyversions/application-settings.svg)](https://github.com/StockwatchDev/application_settings)\n[![Build Status](https://github.com/StockwatchDev/application_settings/actions/workflows/application_settings-tests.yml/badge.svg?branch=develop)](https://github.com/StockwatchDev/application_settings/actions)\n[![codecov](https://codecov.io/gh/StockwatchDev/application_settings/branch/develop/graph/badge.svg)](https://app.codecov.io/gh/StockwatchDev/application_settings)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\n"You write the dataclasses to define parameters for configuration and settings, \napplication\\_settings takes care of the logic."\n\n## What and why\n\nApplication\\_settings is a package for providing a python application with parameters for\nconfiguration and settings. It uses [toml](https://toml.io/en/) or \n[json](https://www.json.org/) files that are parsed\ninto dataclasses. This brings some benefits:\n\n- Minimal work for the application designer\n- Parameters are typed, which allows for improved static code analyses.\n- IDEs will provide helpful hints and completion when using the parameters.\n- More control over what happens when a file contains mistakes\n  (by leveraging the power of [pydantic](https://docs.pydantic.dev/)).\n- Possibility to specify defaults when no file is found or entries are missing.\n- Configuration parameters are read-only (i.e., changed by editing the config file); we\n  recommend (and support) the use of `toml` for this, which is a human-oriented,\n  flexible, standardardized and not overly complex format.\n- Settings parameters are read-write (i.e., mostly changed via the UI of the\n  application); we recommend (and support) use `json` for this, an established\n  standardized machine-oriented format.\n\nParsing is done once during first access and the resulting set of parameters is stored\nas a singleton.\n\nInterested? Then have a look at our\n[quick start](https://stockwatchdev.github.io/application_settings/0.2.0/docs/Quick_start/).\n\n[//]: # (Change link to published quick start)\n\n## License\n\nThis project is licensed under the terms of the MIT license.',
+    'long_description': '# application_settings - version 0.3.0\n\n[![pypi](https://img.shields.io/pypi/v/application-settings.svg)](https://pypi.python.org/pypi/application-settings)\n[![versions](https://img.shields.io/pypi/pyversions/application-settings.svg)](https://github.com/StockwatchDev/application_settings)\n[![Build Status](https://github.com/StockwatchDev/application_settings/actions/workflows/merge_checks.yml/badge.svg?branch=develop)](https://github.com/StockwatchDev/application_settings/actions)\n[![codecov](https://codecov.io/gh/StockwatchDev/application_settings/branch/develop/graph/badge.svg)](https://app.codecov.io/gh/StockwatchDev/application_settings)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\n"You write the dataclasses to define parameters for configuration and settings, \napplication\\_settings takes care of the logic."\n\n## What and why\n\nApplication\\_settings is a package for providing a python application or library with\nparameters for configuration and settings. It uses [toml](https://toml.io/en/) or \n[json](https://www.json.org/) files that are parsed\ninto dataclasses. This brings some benefits:\n\n- Minimal work for the developer of the application / library\n- Parameters are typed, which allows for improved static code analyses.\n- IDEs will provide helpful hints and completion when using the parameters.\n- More control over what happens when a file contains mistakes\n  (by leveraging the power of [pydantic](https://docs.pydantic.dev/)).\n- Possibility to specify defaults when no file is found or entries are missing.\n- Configuration parameters are read-only (i.e., changed by editing the config file); we\n  recommend (and support) the use of `toml` for this, which is a human-oriented,\n  flexible, standardardized and not overly complex format.\n- Settings parameters are read-write (i.e., mostly changed via the UI of the\n  application); we recommend (and support) use `json` for this, an established\n  standardized machine-oriented format.\n\nParsing is done once before or during first access and the resulting set of parameters is\nstored as a singleton.\n\nInterested? Then have a look at our\n[quick start](https://stockwatchdev.github.io/application_settings/0.3.0/docs/Quick_start/).\n\n[//]: # (Change version in header and link to published quick start)\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
     'author': 'Stockwatchdevs',
     'author_email': 'stockwatchdevs@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/StockwatchDev/application_settings',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `application_settings-0.2.0/PKG-INFO` & `application_settings-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: application-settings
-Version: 0.2.0
+Version: 0.3.0
 Summary: For providing a python application with configuration and/or settings
 Home-page: https://github.com/StockwatchDev/application_settings
 License: MIT
 Keywords: configuration,settings,dataclass,pydantic,toml
 Author: Stockwatchdevs
 Author-email: stockwatchdevs@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -18,60 +18,62 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: pathvalidate (>=2.5,<3.0)
+Requires-Dist: pathvalidate (>=2.5,<4.0)
 Requires-Dist: pydantic (>=1.10,<2.0)
 Requires-Dist: tomli (>=2.0,<3.0) ; python_version < "3.11"
 Requires-Dist: tomli-w (>=1.0,<2.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version < "3.11"
 Project-URL: Repository, https://github.com/StockwatchDev/application_settings
 Description-Content-Type: text/markdown
 
-# application_settings
+# application_settings - version 0.3.0
 
 [![pypi](https://img.shields.io/pypi/v/application-settings.svg)](https://pypi.python.org/pypi/application-settings)
 [![versions](https://img.shields.io/pypi/pyversions/application-settings.svg)](https://github.com/StockwatchDev/application_settings)
-[![Build Status](https://github.com/StockwatchDev/application_settings/actions/workflows/application_settings-tests.yml/badge.svg?branch=develop)](https://github.com/StockwatchDev/application_settings/actions)
+[![Build Status](https://github.com/StockwatchDev/application_settings/actions/workflows/merge_checks.yml/badge.svg?branch=develop)](https://github.com/StockwatchDev/application_settings/actions)
 [![codecov](https://codecov.io/gh/StockwatchDev/application_settings/branch/develop/graph/badge.svg)](https://app.codecov.io/gh/StockwatchDev/application_settings)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 "You write the dataclasses to define parameters for configuration and settings, 
 application\_settings takes care of the logic."
 
 ## What and why
 
-Application\_settings is a package for providing a python application with parameters for
-configuration and settings. It uses [toml](https://toml.io/en/) or 
+Application\_settings is a package for providing a python application or library with
+parameters for configuration and settings. It uses [toml](https://toml.io/en/) or 
 [json](https://www.json.org/) files that are parsed
 into dataclasses. This brings some benefits:
 
-- Minimal work for the application designer
+- Minimal work for the developer of the application / library
 - Parameters are typed, which allows for improved static code analyses.
 - IDEs will provide helpful hints and completion when using the parameters.
 - More control over what happens when a file contains mistakes
   (by leveraging the power of [pydantic](https://docs.pydantic.dev/)).
 - Possibility to specify defaults when no file is found or entries are missing.
 - Configuration parameters are read-only (i.e., changed by editing the config file); we
   recommend (and support) the use of `toml` for this, which is a human-oriented,
   flexible, standardardized and not overly complex format.
 - Settings parameters are read-write (i.e., mostly changed via the UI of the
   application); we recommend (and support) use `json` for this, an established
   standardized machine-oriented format.
 
-Parsing is done once during first access and the resulting set of parameters is stored
-as a singleton.
+Parsing is done once before or during first access and the resulting set of parameters is
+stored as a singleton.
 
 Interested? Then have a look at our
-[quick start](https://stockwatchdev.github.io/application_settings/0.2.0/docs/Quick_start/).
+[quick start](https://stockwatchdev.github.io/application_settings/0.3.0/docs/Quick_start/).
 
-[//]: # (Change link to published quick start)
+[//]: # (Change version in header and link to published quick start)
 
 ## License
 
 This project is licensed under the terms of the MIT license.
+
```

