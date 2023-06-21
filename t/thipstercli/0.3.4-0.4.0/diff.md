# Comparing `tmp/thipstercli-0.3.4.tar.gz` & `tmp/thipstercli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipstercli-0.3.4.tar", last modified: Wed Jun 21 12:53:46 2023, max compression
+gzip compressed data, was "thipstercli-0.4.0.tar", last modified: Wed Jun 21 13:13:20 2023, max compression
```

## Comparing `thipstercli-0.3.4.tar` & `thipstercli-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:53:46.815290 thipstercli-0.3.4/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-21 12:53:43.000000 thipstercli-0.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 12:53:46.815290 thipstercli-0.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4516 2023-06-21 12:53:43.000000 thipstercli-0.3.4/README.md
--rw-r--r--   0 root         (0) root         (0)     1361 2023-06-21 12:53:43.000000 thipstercli-0.3.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 12:53:46.819290 thipstercli-0.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1823 2023-06-21 12:53:43.000000 thipstercli-0.3.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:53:46.815290 thipstercli-0.3.4/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 12:53:43.000000 thipstercli-0.3.4/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-06-21 12:53:43.000000 thipstercli-0.3.4/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3847 2023-06-21 12:53:43.000000 thipstercli-0.3.4/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     3137 2023-06-21 12:53:43.000000 thipstercli-0.3.4/tests/test_providers.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-06-21 12:53:43.000000 thipstercli-0.3.4/tests/test_repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:53:46.815290 thipstercli-0.3.4/thipstercli/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6108 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/cli.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/config.py
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/constants.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/display.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/helpers.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/providers.py
--rw-r--r--   0 root         (0) root         (0)     3438 2023-06-21 12:53:43.000000 thipstercli-0.3.4/thipstercli/repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:53:46.815290 thipstercli-0.3.4/thipstercli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 12:53:46.000000 thipstercli-0.3.4/thipstercli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      567 2023-06-21 12:53:46.000000 thipstercli-0.3.4/thipstercli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 12:53:46.000000 thipstercli-0.3.4/thipstercli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-21 12:53:46.000000 thipstercli-0.3.4/thipstercli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      265 2023-06-21 12:53:46.000000 thipstercli-0.3.4/thipstercli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 12:53:46.000000 thipstercli-0.3.4/thipstercli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:13:20.122813 thipstercli-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-21 13:13:16.000000 thipstercli-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 13:13:20.122813 thipstercli-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-06-21 13:13:16.000000 thipstercli-0.4.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-06-21 13:13:16.000000 thipstercli-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 13:13:20.122813 thipstercli-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-06-21 13:13:16.000000 thipstercli-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:13:20.118812 thipstercli-0.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 13:13:16.000000 thipstercli-0.4.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-21 13:13:16.000000 thipstercli-0.4.0/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-06-21 13:13:16.000000 thipstercli-0.4.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-06-21 13:13:16.000000 thipstercli-0.4.0/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-06-21 13:13:16.000000 thipstercli-0.4.0/tests/test_providers.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-21 13:13:16.000000 thipstercli-0.4.0/tests/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:13:20.118812 thipstercli-0.4.0/thipstercli/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6293 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:13:20.122813 thipstercli-0.4.0/thipstercli/commands/
+-rw-r--r--   0 root         (0) root         (0)      131 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8194 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/commands/info.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/commands/providers.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/commands/repository.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/config.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/display.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-06-21 13:13:16.000000 thipstercli-0.4.0/thipstercli/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:13:20.122813 thipstercli-0.4.0/thipstercli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-21 13:13:20.000000 thipstercli-0.4.0/thipstercli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      666 2023-06-21 13:13:20.000000 thipstercli-0.4.0/thipstercli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:13:20.000000 thipstercli-0.4.0/thipstercli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-21 13:13:20.000000 thipstercli-0.4.0/thipstercli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-21 13:13:20.000000 thipstercli-0.4.0/thipstercli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 13:13:20.000000 thipstercli-0.4.0/thipstercli.egg-info/top_level.txt
```

### Comparing `thipstercli-0.3.4/LICENSE` & `thipstercli-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.4/PKG-INFO` & `thipstercli-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.3.4
+Version: 0.4.0
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.3.4 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.4.0 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.3.4/README.md` & `thipstercli-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.4/pyproject.toml` & `thipstercli-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.4/setup.py` & `thipstercli-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('.').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.3.4'
+__version__ = '0.4.0'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as f:
     long_description = f.read()
```

### Comparing `thipstercli-0.3.4/tests/conftest.py` & `thipstercli-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.4/tests/test_cli.py` & `thipstercli-0.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.4/tests/test_providers.py` & `thipstercli-0.4.0/tests/test_providers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Test the providers.py module."""
 import pytest
 from typer.testing import CliRunner
 
+from thipstercli.commands.providers import check_provider_exists, providers_app
 from thipstercli.config import init_parameters, state
 from thipstercli.helpers import get_auth_provider_class
-from thipstercli.providers import check_provider_exists, provider_app
 
 from .conftest import get_config_file
 
 runner = CliRunner(mix_stderr=False)
 
 providers = [
     'google',
@@ -21,54 +21,54 @@
     create_config_file.write_text("""{"auth_provider": "notfound"}""")
     init_parameters()
     yield
 
 
 def test_list_providers():
     """Test the list command."""
-    result = runner.invoke(provider_app, ['list'])
+    result = runner.invoke(providers_app, ['list'])
     assert result.exit_code == 0
     for provider in providers:
         assert provider in result.stdout.lower()
 
 
 def test_info_provider():
     """Test the info command for 'google'."""
-    result = runner.invoke(provider_app, ['info', 'google'])
+    result = runner.invoke(providers_app, ['info', 'google'])
     assert result.exit_code == 0
     assert 'google' in result.stdout.lower()
     assert 'gcloud' in result.stdout.lower()
 
 
 def test_info_provider_not_found():
     """Test the info command for wrong provider 'notfound'."""
-    result = runner.invoke(provider_app, ['info', 'notfound'])
+    result = runner.invoke(providers_app, ['info', 'notfound'])
     assert result.exit_code == 1
     assert 'provider notfound not found.' in result.stdout.lower()
 
 
 def test_set_provider():
     """Test the set command for 'google'."""
-    result = runner.invoke(provider_app, ['set', 'google'])
+    result = runner.invoke(providers_app, ['set', 'google'])
     assert result.exit_code == 0
     assert 'google' in result.stdout.lower()
     assert 'provider set to' in result.stdout.lower()
 
 
 def test_set_provider_not_found():
     """Test the set command for wrong provider 'notfound'."""
-    result = runner.invoke(provider_app, ['set', 'notfound'])
+    result = runner.invoke(providers_app, ['set', 'notfound'])
     assert result.exit_code == 1
     assert 'provider notfound not found.' in result.stdout.lower()
 
 
 def test_display_provider(config_file):
     """Test the display command for the 'google' provider set in the config file."""
     _ = config_file
-    result = runner.invoke(provider_app, ['display'])
+    result = runner.invoke(providers_app, ['display'])
     assert result.exit_code == 0
     assert 'provider set to' in result.stdout.lower()
     assert 'google' in result.stdout.lower()
 
 
 def test_get_provider_class():
     """Test the get_auth_provider_class function."""
@@ -81,16 +81,16 @@
     provider = check_provider_exists('google')
     assert provider == 'google'
 
 
 def test_set_provider_config_file(config_file_wrong_provider):
     """Test if the set command sets the provider in the config file."""
     _ = config_file_wrong_provider
-    runner.invoke(provider_app, ['set', 'google'])
+    runner.invoke(providers_app, ['set', 'google'])
     assert get_config_file().get('auth_provider') == 'google'
 
 
 def test_wrong_provider_config_file(config_file_wrong_provider):
     """Test the behavior of the app when the config file has a wrong provider."""
     _ = config_file_wrong_provider
-    runner.invoke(provider_app, ['--help'])
+    runner.invoke(providers_app, ['--help'])
     assert state.get('auth_provider') is None
```

### Comparing `thipstercli-0.3.4/tests/test_repository.py` & `thipstercli-0.4.0/tests/test_repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import pytest
 from typer import get_app_dir
 from typer.testing import CliRunner
 
 import thipstercli.constants as constants
 from tests.conftest import get_config_file
-from thipstercli.repository import repository_app
+from thipstercli.commands.repository import repository_app
 
 runner = CliRunner(mix_stderr=False)
 
 
 @pytest.fixture
 def create_models_directory():
     """Create the model subdirectory if needed."""
```

### Comparing `thipstercli-0.3.4/thipstercli/cli.py` & `thipstercli-0.4.0/thipstercli/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """THipster CLI."""
+import importlib
+import os
 from pathlib import Path
 
 import typer
 from rich import print
 from thipster import Engine as ThipsterEngine
 from thipster.auth import Google
 from thipster.engine.exceptions import THipsterError
 from thipster.parser import ParserFactory
 from thipster.repository import GithubRepo, LocalRepo
 from thipster.terraform import Terraform
 
 import thipstercli.constants as constants
-from thipstercli import providers, repository
+from thipstercli.commands import providers, repository
 from thipstercli.config import app_dir, init_parameters, state
 from thipstercli.display import (
     error,
     print_if_verbose,
     print_package_version,
     print_start_if_verbose,
     print_success_if_verbose,
@@ -24,16 +26,22 @@
 init_parameters()
 
 main_app = typer.Typer(
     name=state.get(
         'app_name', constants.APP_NAME,
     ), no_args_is_help=True,
 )
-main_app.add_typer(providers.provider_app, name='providers')
-main_app.add_typer(repository.repository_app, name='repository')
+
+module = importlib.import_module('thipstercli.commands')
+for command in os.scandir(Path(module.__file__).parent):
+    if command.name.startswith('__'):
+        continue
+    command = command.name[:-3]
+
+    main_app.add_typer(getattr(module, f'{command}_app'), name=command)
 
 
 @main_app.callback()
 def _callback(
     verbose: bool = typer.Option(
         state.get('verbose', constants.VERBOSE),
         '--verbose', '-v',
```

### Comparing `thipstercli-0.3.4/thipstercli/config.py` & `thipstercli-0.4.0/thipstercli/config.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.4/thipstercli/display.py` & `thipstercli-0.4.0/thipstercli/display.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.4/thipstercli/helpers.py` & `thipstercli-0.4.0/thipstercli/helpers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.3.4/thipstercli/providers.py` & `thipstercli-0.4.0/thipstercli/commands/providers.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,56 +6,56 @@
 from thipstercli.config import state, update_config_file
 from thipstercli.helpers import (
     check_thipster_module_exists,
     get_auth_provider_class,
     get_thipster_module_class_list,
 )
 
-provider_app = typer.Typer(no_args_is_help=True)
+providers_app = typer.Typer(no_args_is_help=True)
 
 
-@provider_app.callback()
+@providers_app.callback()
 def _callback():
     """Manage authentification providers."""
 
 
-@provider_app.command('list')
+@providers_app.command('list')
 def _list():
     """List all the supported providers."""
     state['providers'] = get_thipster_module_class_list('auth')
     provider_display = ''
     for provider in state['providers']:
         provider_display += f'[green]{provider[:-3]}[/green]\n'
     print(Panel(provider_display, title='Providers'))
     __more_info_provider()
 
 
-@provider_app.command('info')
+@providers_app.command('info')
 def info(provider: str):
     """Get information about a provider."""
     provider = check_provider_exists(provider)
 
     provider_class = get_auth_provider_class(provider)
     print(Panel(provider_class.__doc__, title=provider))
 
 
-@provider_app.command('set')
+@providers_app.command('set')
 def set_auth_provider(provider: str):
     """Set the provider to use for the auth."""
     provider = check_provider_exists(provider)
 
     update_config_file(
         {'auth_provider': provider},
     )
 
     print(f'Provider set to [green]{provider}[/green]')
     __more_info_provider()
 
 
-@provider_app.command('display')
+@providers_app.command('display')
 def display():
     """Display the current provider."""
     if not state.get('auth_provider', None):
         print('No provider set.\nPlease use [bold]thipster providers set <provider>\
 [/bold] to set a provider')
         return
     print(f"Provider set to [green]{state['auth_provider']}[/green]")
@@ -76,8 +76,8 @@
     print(
         Panel('For more information about a provider, run: thipster providers info \
 <provider>'),
     ) if state.get('verbose') else None
 
 
 if __name__ == '__main__':
-    provider_app()
+    providers_app()
```

### Comparing `thipstercli-0.3.4/thipstercli/repository.py` & `thipstercli-0.4.0/thipstercli/commands/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from typing import Annotated
 
 import typer
 from git import Repo
 from rich import print
 from rich.panel import Panel
 
-from .config import app_dir, state, update_config_file
-from .constants import LOCAL_MODELS_REPOSITORY_PATH
-from .display import error, warn
+from thipstercli.config import app_dir, state, update_config_file
+from thipstercli.constants import LOCAL_MODELS_REPOSITORY_PATH
+from thipstercli.display import error, warn
 
 repository_app = typer.Typer(no_args_is_help=True)
 
 
 @repository_app.callback()
 def main():
     """Manage locally installed THipster repositories."""
```

### Comparing `thipstercli-0.3.4/thipstercli.egg-info/PKG-INFO` & `thipstercli-0.4.0/thipstercli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.3.4
+Version: 0.4.0
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.3.4 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.4.0 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.3.4/thipstercli.egg-info/SOURCES.txt` & `thipstercli-0.4.0/thipstercli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 tests/__init__.py
 tests/conftest.py
 tests/test_cli.py
+tests/test_info.py
 tests/test_providers.py
 tests/test_repository.py
 thipstercli/__init__.py
 thipstercli/__main__.py
 thipstercli/cli.py
 thipstercli/config.py
 thipstercli/constants.py
 thipstercli/display.py
 thipstercli/helpers.py
-thipstercli/providers.py
-thipstercli/repository.py
 thipstercli.egg-info/PKG-INFO
 thipstercli.egg-info/SOURCES.txt
 thipstercli.egg-info/dependency_links.txt
 thipstercli.egg-info/entry_points.txt
 thipstercli.egg-info/requires.txt
-thipstercli.egg-info/top_level.txt
+thipstercli.egg-info/top_level.txt
+thipstercli/commands/__init__.py
+thipstercli/commands/info.py
+thipstercli/commands/providers.py
+thipstercli/commands/repository.py
```

