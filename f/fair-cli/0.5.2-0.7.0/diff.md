# Comparing `tmp/fair_cli-0.5.2.tar.gz` & `tmp/fair_cli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_cli-0.5.2.tar", max compression
+gzip compressed data, was "fair_cli-0.7.0.tar", max compression
```

## Comparing `fair_cli-0.5.2.tar` & `fair_cli-0.7.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1888 2023-04-27 13:19:09.272183 fair_cli-0.5.2/CHANGELOG.md
--rw-r--r--   0        0        0     1397 2023-04-27 13:19:09.272183 fair_cli-0.5.2/CITATION.cff
--rw-r--r--   0        0        0     2027 2023-04-27 10:42:03.123818 fair_cli-0.5.2/fair/__init__.py
--rw-r--r--   0        0        0    20683 2023-04-28 23:41:25.182481 fair_cli-0.5.2/fair/cli.py
--rw-r--r--   0        0        0     9462 2023-04-27 13:19:09.276183 fair_cli-0.5.2/fair/common.py
--rw-r--r--   0        0        0    28995 2023-04-28 23:41:25.182481 fair_cli-0.5.2/fair/configuration/__init__.py
--rw-r--r--   0        0        0     3443 2023-04-27 13:19:09.277182 fair_cli-0.5.2/fair/configuration/validation.py
--rw-r--r--   0        0        0     5555 2023-04-27 13:19:09.277182 fair_cli-0.5.2/fair/exceptions.py
--rw-r--r--   0        0        0    10127 2023-04-27 13:19:09.278183 fair_cli-0.5.2/fair/files.txt
--rw-r--r--   0        0        0     4785 2023-04-27 13:19:09.278183 fair_cli-0.5.2/fair/history.py
--rw-r--r--   0        0        0     4139 2023-04-28 23:41:30.085525 fair_cli-0.5.2/fair/identifiers.py
--rw-r--r--   0        0        0     2383 2023-04-27 13:19:09.279183 fair_cli-0.5.2/fair/logging.py
--rw-r--r--   0        0        0     8423 2023-04-27 13:19:09.279183 fair_cli-0.5.2/fair/register.py
--rw-r--r--   0        0        0      168 2023-04-27 13:19:09.280182 fair_cli-0.5.2/fair/registry/__init__.py
--rw-r--r--   0        0        0     1285 2023-04-27 10:42:03.127817 fair_cli-0.5.2/fair/registry/file_formats.json
--rw-r--r--   0        0        0      126 2023-04-27 10:42:03.127817 fair_cli-0.5.2/fair/registry/file_types.py
--rw-r--r--   0        0        0    15642 2023-04-28 23:41:25.183481 fair_cli-0.5.2/fair/registry/requests.py
--rw-r--r--   0        0        0    15251 2023-04-28 23:41:25.183481 fair_cli-0.5.2/fair/registry/server.py
--rw-r--r--   0        0        0    23360 2023-04-28 23:41:25.184481 fair_cli-0.5.2/fair/registry/storage.py
--rw-r--r--   0        0        0    15401 2023-04-28 23:41:25.184481 fair_cli-0.5.2/fair/registry/sync.py
--rw-r--r--   0        0        0     4936 2023-04-27 13:19:09.281183 fair_cli-0.5.2/fair/registry/versioning.py
--rw-r--r--   0        0        0     2396 2023-04-27 13:19:09.282183 fair_cli-0.5.2/fair/run.py
--rw-r--r--   0        0        0    41645 2023-04-28 23:41:25.185481 fair_cli-0.5.2/fair/session.py
--rw-r--r--   0        0        0    15660 2023-04-28 23:41:25.185481 fair_cli-0.5.2/fair/staging.py
--rw-r--r--   0        0        0      515 2023-04-27 10:42:03.130817 fair_cli-0.5.2/fair/templates/__init__.py
--rw-r--r--   0        0        0      301 2023-04-27 10:42:03.131817 fair_cli-0.5.2/fair/templates/config.jinja
--rw-r--r--   0        0        0      139 2023-04-27 10:42:03.131817 fair_cli-0.5.2/fair/templates/hist.jinja
--rw-r--r--   0        0        0     3284 2023-04-27 13:19:09.283182 fair_cli-0.5.2/fair/testing.py
--rw-r--r--   0        0        0    55154 2023-04-27 13:19:09.284183 fair_cli-0.5.2/fair/user_config/__init__.py
--rw-r--r--   0        0        0     5023 2023-04-27 13:19:09.284183 fair_cli-0.5.2/fair/user_config/globbing.py
--rw-r--r--   0        0        0     9510 2023-04-27 13:19:09.285183 fair_cli-0.5.2/fair/user_config/validation.py
--rw-r--r--   0        0        0     5168 2023-04-28 23:41:25.186481 fair_cli-0.5.2/fair/utilities.py
--rw-r--r--   0        0        0     1511 2023-04-27 13:19:09.285183 fair_cli-0.5.2/fair/virtualenv.py
--rw-r--r--   0        0        0     1339 2023-04-27 10:42:03.118817 fair_cli-0.5.2/LICENSE
--rw-r--r--   0        0        0     2463 2023-04-28 23:41:30.085525 fair_cli-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    11631 2023-04-27 13:19:09.272183 fair_cli-0.5.2/README.md
--rw-r--r--   0        0        0    13363 1970-01-01 00:00:00.000000 fair_cli-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1855 2023-06-12 13:03:22.463189 fair_cli-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1358 2023-06-12 13:03:22.463239 fair_cli-0.7.0/CITATION.cff
+-rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.7.0/LICENSE
+-rw-r--r--   0        0        0    11363 2023-06-21 16:01:16.540375 fair_cli-0.7.0/README.md
+-rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.7.0/fair/__init__.py
+-rw-r--r--   0        0        0    22289 2023-06-21 17:23:03.900038 fair_cli-0.7.0/fair/cli.py
+-rw-r--r--   0        0        0     9190 2023-06-21 16:01:16.540403 fair_cli-0.7.0/fair/common.py
+-rw-r--r--   0        0        0    28212 2023-06-21 17:07:31.416628 fair_cli-0.7.0/fair/configuration/__init__.py
+-rw-r--r--   0        0        0     3311 2023-06-12 13:03:22.464979 fair_cli-0.7.0/fair/configuration/validation.py
+-rw-r--r--   0        0        0     5358 2023-06-12 13:03:22.465044 fair_cli-0.7.0/fair/exceptions.py
+-rw-r--r--   0        0        0    10127 2023-06-12 13:03:22.465098 fair_cli-0.7.0/fair/files.txt
+-rw-r--r--   0        0        0     4619 2023-06-12 13:03:22.465161 fair_cli-0.7.0/fair/history.py
+-rw-r--r--   0        0        0     3958 2023-06-12 13:03:22.465230 fair_cli-0.7.0/fair/identifiers.py
+-rw-r--r--   0        0        0     3010 2023-06-14 13:29:24.954224 fair_cli-0.7.0/fair/logging.py
+-rw-r--r--   0        0        0     8206 2023-06-14 13:29:24.954405 fair_cli-0.7.0/fair/register.py
+-rw-r--r--   0        0        0      161 2023-06-12 13:03:22.465449 fair_cli-0.7.0/fair/registry/__init__.py
+-rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.7.0/fair/registry/file_formats.json
+-rw-r--r--   0        0        0      120 2023-06-12 13:03:22.465547 fair_cli-0.7.0/fair/registry/file_types.py
+-rw-r--r--   0        0        0    17278 2023-06-14 13:29:24.954679 fair_cli-0.7.0/fair/registry/requests.py
+-rw-r--r--   0        0        0    14756 2023-06-12 13:03:22.465732 fair_cli-0.7.0/fair/registry/server.py
+-rw-r--r--   0        0        0    23693 2023-06-21 16:05:36.970594 fair_cli-0.7.0/fair/registry/storage.py
+-rw-r--r--   0        0        0    38433 2023-06-14 13:29:24.955335 fair_cli-0.7.0/fair/registry/sync.py
+-rw-r--r--   0        0        0     4752 2023-06-12 13:03:22.466011 fair_cli-0.7.0/fair/registry/versioning.py
+-rw-r--r--   0        0        0     2302 2023-06-12 13:03:22.466108 fair_cli-0.7.0/fair/run.py
+-rw-r--r--   0        0        0    49608 2023-06-21 16:41:58.205044 fair_cli-0.7.0/fair/session.py
+-rw-r--r--   0        0        0    16133 2023-06-14 13:29:24.955867 fair_cli-0.7.0/fair/staging.py
+-rw-r--r--   0        0        0      490 2023-06-12 13:03:22.466460 fair_cli-0.7.0/fair/templates/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.7.0/fair/templates/config.jinja
+-rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.7.0/fair/templates/hist.jinja
+-rw-r--r--   0        0        0     3181 2023-06-12 13:03:22.466610 fair_cli-0.7.0/fair/testing.py
+-rw-r--r--   0        0        0    53662 2023-06-12 13:03:22.466847 fair_cli-0.7.0/fair/user_config/__init__.py
+-rw-r--r--   0        0        0     4830 2023-06-12 13:03:22.466916 fair_cli-0.7.0/fair/user_config/globbing.py
+-rw-r--r--   0        0        0     9187 2023-06-12 13:03:22.466981 fair_cli-0.7.0/fair/user_config/validation.py
+-rw-r--r--   0        0        0     5087 2023-06-14 13:29:24.956007 fair_cli-0.7.0/fair/utilities.py
+-rw-r--r--   0        0        0     1465 2023-06-12 13:03:22.467103 fair_cli-0.7.0/fair/virtualenv.py
+-rw-r--r--   0        0        0     2563 2023-06-21 18:06:06.014133 fair_cli-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    13498 1970-01-01 00:00:00.000000 fair_cli-0.7.0/PKG-INFO
```

### Comparing `fair_cli-0.5.2/CHANGELOG.md` & `fair_cli-0.7.0/CHANGELOG.md`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# Unreleased
-- Fix virtual environment bug in `fair` binaries where `venv` assumes the main executable is `python`.
-- Registration of `author` and `namespace` objects.
-- Allow specification of tag to install registry from during `fair registry install`.
-- Wildcard '*' parsing introduced for data products.
-- Ability to `push` to a registry added.
-- Added `--dirty` option to `fair run` to allow running with uncommitted changes.
-- Added `config.yaml` file validation.
-- Added initialisation from existing registry.
-- Switch to setting port not local URI during initialisation.
-- Added option to specify port on `fair registry start`.
-- Added `cli-config.yaml` file validation during initialisation.
-- Added `fair reset` to list of commands.
-- Add tab completion for staging data products.
-
-# 2021-11-17 [v0.2.3](https://github.com/FAIRDataPipeline/FAIR-CLI/releases/tag/v0.2.3)
-- Move handling of the user `config.yaml` file to a separate class `JobConfiguration`.
-- Added various fixes to improve functionality within Windows.
-- Move registry installation from script execution to internal function which sets up virtual environment etc.
-- Added a test suite to the project.
-- Added additional recognised identifiers for author setup from an organisation GRID and ROR.
-
-# 2021-10-06 [v0.2.2](https://github.com/FAIRDataPipeline/FAIR-CLI/releases/tag/v0.2.2)
-- Update to package metadata for PyPi
-
-# 2021-10-06 [v0.2.1](https://github.com/FAIRDataPipeline/FAIR-CLI/releases/tag/v0.2.1)
-- Automatic starter `config.yaml` generation.
-- Local and Global CLI configurations.
-- Start/stop local registry either explicitly or during synchronisations.
-- Run logs available via git-like interface.
-- Added ability to add/remove files.
-- Repository style handling, acts like another git-like tool per project.
-- Creation of an interface for `fair` using `click`.
+# Unreleased
+- Fix virtual environment bug in `fair` binaries where `venv` assumes the main executable is `python`.
+- Registration of `author` and `namespace` objects.
+- Allow specification of tag to install registry from during `fair registry install`.
+- Wildcard '*' parsing introduced for data products.
+- Ability to `push` to a registry added.
+- Added `--dirty` option to `fair run` to allow running with uncommitted changes.
+- Added `config.yaml` file validation.
+- Added initialisation from existing registry.
+- Switch to setting port not local URI during initialisation.
+- Added option to specify port on `fair registry start`.
+- Added `cli-config.yaml` file validation during initialisation.
+- Added `fair reset` to list of commands.
+- Add tab completion for staging data products.
+
+# 2021-11-17 [v0.2.3](https://github.com/FAIRDataPipeline/FAIR-CLI/releases/tag/v0.2.3)
+- Move handling of the user `config.yaml` file to a separate class `JobConfiguration`.
+- Added various fixes to improve functionality within Windows.
+- Move registry installation from script execution to internal function which sets up virtual environment etc.
+- Added a test suite to the project.
+- Added additional recognised identifiers for author setup from an organisation GRID and ROR.
+
+# 2021-10-06 [v0.2.2](https://github.com/FAIRDataPipeline/FAIR-CLI/releases/tag/v0.2.2)
+- Update to package metadata for PyPi
+
+# 2021-10-06 [v0.2.1](https://github.com/FAIRDataPipeline/FAIR-CLI/releases/tag/v0.2.1)
+- Automatic starter `config.yaml` generation.
+- Local and Global CLI configurations.
+- Start/stop local registry either explicitly or during synchronisations.
+- Run logs available via git-like interface.
+- Added ability to add/remove files.
+- Repository style handling, acts like another git-like tool per project.
+- Creation of an interface for `fair` using `click`.
```

### Comparing `fair_cli-0.5.2/fair/__init__.py` & `fair_cli-0.7.0/fair/__init__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-#!/usr/bin/env python3
-"""
-FAIR Data Pipeline Command Line Interface Tool
-----------------------------------------------
-Contains definitions for the synchronisation tool for communication between
-remote and local FAIR Data Pipeline registries.
-
-License
--------
-
-BSD 2-Clause License
-
-Copyright (c) 2021, Scottish COVID Response Consortium
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-"""
-
-__author__ = "Scottish COVID-19 Response Consortium"
-__credits__ = [
-    "Richard Reeve (University of Glasgow)",
-    "Nathan Cummings (UKAEA)",
-    "Kristian Zarebski (UKAEA)",
-    "Dennis Reddyhoff (University of Sheffield)",
-]
-__license__ = "BSD-2-Clause"
-__status__ = "Development"
-__copyright__ = "Copyright 2021, SCRC"
-
-import logging
-
-logging.basicConfig()
+#!/usr/bin/env python3
+"""
+FAIR Data Pipeline Command Line Interface Tool
+----------------------------------------------
+Contains definitions for the synchronisation tool for communication between
+remote and local FAIR Data Pipeline registries.
+
+License
+-------
+
+BSD 2-Clause License
+
+Copyright (c) 2021, Scottish COVID Response Consortium
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+"""
+
+__author__ = "Scottish COVID-19 Response Consortium"
+__credits__ = [
+    "Richard Reeve (University of Glasgow)",
+    "Nathan Cummings (UKAEA)",
+    "Kristian Zarebski (UKAEA)",
+    "Dennis Reddyhoff (University of Sheffield)",
+]
+__license__ = "BSD-2-Clause"
+__status__ = "Development"
+__copyright__ = "Copyright 2021, SCRC"
+
+import logging
+
+logging.basicConfig()
```

### Comparing `fair_cli-0.5.2/fair/cli.py` & `fair_cli-0.7.0/fair/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,668 +1,744 @@
-#!/usr/bin/env python3
-# flake8: noqa
-# -*- coding: utf-8 -*-
-"""
-Command Line Interface
-======================
-
-Main command line interface setup script for creation of commands used to
-interact with the synchronisation tool.
-"""
-
-__date__ = "2021-06-24"
-
-import glob
-import logging
-import os
-import pathlib
-import sys
-import typing
-
-import click
-import click.shell_completion
-import yaml
-
-import fair.common as fdp_com
-import fair.configuration as fdp_conf
-import fair.exceptions as fdp_exc
-import fair.history as fdp_hist
-import fair.registry.server as fdp_svr
-import fair.run as fdp_run
-import fair.session as fdp_session
-
-__author__ = "Scottish COVID Response Consortium"
-__credits__ = [
-    "Richard Reeve (University of Glasgow)",
-    "Nathan Cummings (UKAEA)",
-    "Kristian Zarebski (UKAEA)",
-    "Dennis Reddyhoff (University of Sheffield)",
-    "Ryan Field (University of Glasgow)",
-]
-__license__ = "BSD-2-Clause"
-__status__ = "Development"
-__copyright__ = "Copyright 2021, FAIR Data Pipeline"
-
-
-def complete_yamls(ctx, param, incomplete):
-    _file_list: typing.List[str] = [
-        str(i) for i in pathlib.Path(os.getcwd()).rglob("*.yaml")
-    ]
-    _file_list += [str(i) for i in pathlib.Path(os.getcwd()).rglob("*.yml")]
-    return [
-        click.shell_completion.CompletionItem(k)
-        for k in _file_list
-        if k.startswith(incomplete)
-    ]
-
-
-def complete_data_products(ctx, param, incomplete) -> typing.List[str]:
-    _staging_file = fdp_com.staging_cache(os.getcwd())
-    if not os.path.exists(_staging_file):
-        return []
-    _staging_data = yaml.safe_load(open(_staging_file))
-    _candidates = list(_staging_data["data_product"].keys())
-    return [
-        click.shell_completion.CompletionItem(c)
-        for c in _candidates
-        if c.startswith(incomplete)
-    ]
-
-
-def complete_jobs(ctx, param, incomplete) -> typing.List[str]:
-    _log_dir = fdp_hist.history_directory(os.getcwd())
-    _job_dir = fdp_com.default_jobs_dir()
-    if not os.path.isdir(_log_dir) or not os.path.isdir(_job_dir):
-        return []
-    _job_dirs = glob.glob(os.path.join(_job_dir, "*"))
-    _jobs = [fdp_run.get_job_hash(jd) for jd in _job_dirs]
-    return [
-        click.shell_completion.CompletionItem(j)
-        for j in _jobs
-        if j.startswith(incomplete)
-    ]
-
-
-@click.group()
-@click.version_option(package_name="fair-cli")
-def cli():
-    """Welcome to FAIR-CLI, the FAIR data pipeline command-line interface."""
-    pass
-
-
-@cli.command()
-@click.option("--verbose/--not-verbose", help="Display URLs", default=False)
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-def status(verbose, debug) -> None:
-    """Get the status of files under staging"""
-    try:
-        with fdp_session.FAIR(
-            os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
-        ) as fair_session:
-            fair_session.status_data_products()
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@cli.command()
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-@click.argument("output", nargs=-1)
-def create(debug, output: str) -> None:
-    """Generate a new FAIR repository user YAML config file"""
-    output = (
-        output[0]
-        if output
-        else os.path.join(os.getcwd(), fdp_com.USER_CONFIG_FILE)
-    )
-    click.echo(f"Generating new user configuration file" f" '{output}'")
-    with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
-        fair_session.make_starter_config(output)
-
-
-@cli.command()
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-def reset(debug: bool) -> None:
-    """Unstage all items marked for staging"""
-    try:
-        with fdp_session.FAIR(
-            os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
-        ) as fair_session:
-            fair_session.reset_staging()
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@cli.command()
-@click.option(
-    "--config",
-    help="Create a starter user config.yaml file during initialisation",
-    default=None,
-)
-@click.option(
-    "--using",
-    help="Initialise the CLI system from an existing CLI global configuration file",
-    default="",
-    shell_complete=complete_yamls,
-)
-@click.option(
-    "--registry",
-    help="Specify registry directory",
-    default=None,
-    show_default=True,
-)
-@click.option(
-    "--ci/--standard",
-    help="Run in testing mode for a CI system",
-    default=False,
-)
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-@click.option(
-    "--export", help="Export the CLI configuration to a file", default=""
-)
-@click.option(
-    "--local/--no-local",
-    help="init without a remote registry - useful for closed systems",
-    default=False,
-)
-def init(
-    config: str,
-    debug: bool,
-    using: str,
-    registry: str,
-    ci: bool,
-    local: bool,
-    export: str = "",
-) -> None:
-    """Initialise repository in current location"""
-    try:
-        with fdp_session.FAIR(
-            os.getcwd(), None, debug=debug, testing=ci, local=local
-        ) as fair_session:
-            _use_dict = {}
-            if using:
-                if not os.path.exists(using):
-                    raise fdp_exc.FileNotFoundError(
-                        f"Cannot load CLI configuration from file '{using}', "
-                        "file does not exist."
-                    )
-                _use_dict = yaml.safe_load(open(using))
-
-            fair_session.initialise(
-                using=_use_dict,
-                registry=registry,
-                export_as=export,
-                local=local,
-            )
-            if config:
-                fair_session.make_starter_config(config)
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@cli.command()
-@click.option(
-    "glob",
-    "--global/--no-global",
-    help="Also delete global FAIR-CLI directories",
-    default=False,
-)
-@click.option(
-    "--yes/--no",
-    help="Deletes the configurations specified without prompt",
-    default=False,
-)
-@click.option(
-    "--data/--no-data",
-    help="Also delete the local data directory",
-    default=False,
-)
-@click.option(
-    "--all/--not-all",
-    help="Remove all FAIR interfaces and registry",
-    default=False,
-)
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-def purge(glob: bool, debug: bool, yes: bool, data: bool, all: bool) -> None:
-    # sourcery skip: avoid-builtin-shadow
-    """Resets the repository deleting all local caches"""
-    _purge = yes
-
-    if all:
-        all = click.confirm(
-            "Are you sure you want to remove all FAIR components from this system?\n"
-            "WARNING: This will also remove your local registry"
-        )
-    else:
-        _purge = click.confirm(
-            "Are you sure you want to reset FAIR tracking, "
-            "this is not reversible?"
-        )
-        if data:
-            data = click.confirm(
-                "Are you sure you want to delete the local data directory?\n"
-                "WARNING: Do not do this if you have a populated local registry"
-            )
-        if not _purge:
-            return
-
-    try:
-        with fdp_session.FAIR(os.getcwd()) as fair_session:
-            fair_session.purge(global_cfg=glob, clear_data=data, clear_all=all)
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@cli.group()
-def registry() -> None:
-    """Commands relating to control of the local registry server"""
-    pass
-
-
-@registry.command()
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-def uninstall(debug: bool):
-    """Uninstall the local registry from the system"""
-    _confirm = click.confirm(
-        "Are you sure you want to remove the local registry and its components?",
-        default=False,
-    )
-    if not _confirm:
-        return
-    try:
-        if debug:
-            logging.getLogger("FAIRDataPipeline").setLevel(logging.DEBUG)
-        fdp_svr.uninstall_registry()
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@registry.command()
-@click.option("--force/--no-force", help="Force a reinstall", default=False)
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-@click.option("--directory", help="Installation location", default=None)
-@click.option(
-    "--version",
-    help="Specify version tag of registry to install, else latest repo tag",
-    default=None,
-)
-def install(debug: bool, force: bool, directory: str, version: str):
-    """Install the local registry on the system"""
-    try:
-        if debug:
-            logging.getLogger("FAIRDataPipeline").setLevel(logging.DEBUG)
-        _version = fdp_svr.install_registry(
-            install_dir=directory, reference=version, force=force
-        )
-        click.echo(f"Installed registry version '{_version}'")
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@registry.command()
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-@click.option("--port", help="port on which to run registry", default=8000)
-@click.option("--address", help="Address on which to run registry", default="127.0.0.1")
-def start(debug: bool, port: int, address: str) -> None:
-    """Start the local registry server"""
-    try:
-        fdp_session.FAIR(
-            os.getcwd(),
-            server_mode=fdp_svr.SwitchMode.USER_START,
-            debug=debug,
-            server_port=port,
-            server_address=address
-        )
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@registry.command()
-@click.option("--force/--no-force", help="Force server stop", default=False)
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-def stop(force: bool, debug: bool) -> None:
-    """Stop the local registry server"""
-    _mode = (
-        fdp_svr.SwitchMode.FORCE_STOP
-        if force
-        else fdp_svr.SwitchMode.USER_STOP
-    )
-    try:
-        fdp_session.FAIR(os.getcwd(), server_mode=_mode, debug=debug)
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@cli.command()
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-def log(debug: bool) -> None:
-    """Show a full job history"""
-    try:
-        fdp_hist.show_history(os.getcwd())
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@cli.command()
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-@click.argument("job_id", shell_complete=complete_jobs)
-def view(job_id: str, debug: bool) -> None:
-    """View log for a given job"""
-    try:
-        fdp_hist.show_job_log(os.getcwd(), job_id)
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@cli.command()
-@click.argument("identifier")
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-@click.option("-j", "--job/--no-job", help="Stage entire job", default=False)
-def unstage(identifier: str, debug: bool, job: bool) -> None:
-    """Remove data products or jobs from staging"""
-    try:
-        with fdp_session.FAIR(
-            os.getcwd(),
-            debug=debug,
-        ) as fair_session:
-            fair_session.change_staging_state(
-                identifier,
-                "job" if job else "data_product",
-                stage=False,
-            )
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@cli.command()
-@click.argument("identifier", shell_complete=complete_data_products)
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-def add(identifier: str, debug: bool) -> None:
-    """Add a data product to staging"""
-    try:
-        with fdp_session.FAIR(
-            os.getcwd(),
-            debug=debug,
-        ) as fair_session:
-            fair_session.change_staging_state(
-                identifier,
-                "data_product",
-            )
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@cli.command()
-@click.argument("job_ids", nargs=-1)
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-@click.option(
-    "--cached/--not-cached",
-    default=False,
-    help="remove from tracking but do not delete from file system",
-)
-def rm(
-    job_ids: typing.List[str], cached: bool = False, debug: bool = False
-) -> None:
-    """Removes jobs from system or just tracking"""
-    pass
-
-
-@cli.command()
-@click.argument("config", nargs=-1)
-@click.option(
-    "--script",
-    help="Specify a shell command to execute, this will be inserted into the working config",
-    default="",
-)
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-@click.option(
-    "--ci/--no-ci",
-    help="Calls run passively without executing any commands for a CI system",
-    default=False,
-)
-@click.option(
-    "--dirty/--clean",
-    help="Allow running with uncommitted changes",
-    default=False,
-)
-@click.option(
-    "--local/--no-local",
-    help="init without a remote registry - useful for closed systems",
-    default=False,
-)
-def run(
-    config: str, script: str, debug: bool, ci: bool, dirty: bool, local: bool
-):
-    """Initialises a job with the option to specify a bash command"""
-    # Allow no config to be specified, if that is the case use default local
-    config = config[0] if config else fdp_com.local_user_config(os.getcwd())
-    try:
-        with fdp_session.FAIR(
-            os.getcwd(),
-            config,
-            debug=debug,
-            server_mode=fdp_svr.SwitchMode.CLI,
-            allow_dirty=dirty,
-            local=local,
-        ) as fair_session:
-            _hash = fair_session.run(
-                script, passive=ci, allow_dirty=dirty, local=local
-            )
-            if ci:
-                click.echo(fdp_run.get_job_dir(_hash))
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@cli.group(invoke_without_command=True)
-@click.option("--verbose/--no-verbose", "-v/")
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-@click.pass_context
-def remote(ctx, verbose: bool = False, debug: bool = False):
-    """List remotes if no additional command is provided"""
-    if not ctx.invoked_subcommand:
-        try:
-            with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
-                fair_session.list_remotes(verbose)
-        except fdp_exc.FAIRCLIException as e:
-            if debug:
-                raise e
-            e.err_print()
-            if e.level.lower() == "error":
-                sys.exit(e.exit_code)
-
-
-@remote.command()
-@click.argument("options", nargs=-1)
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-def add(options: typing.List[str], debug: bool) -> None:
-    """Add a remote registry URL with option to give it a label if multiple
-    remotes may be used.
-
-    Parameters
-    ----------
-    options : typing.List[str]
-        size 1 or 2 list containing either:
-            - label, url
-            - url
-    """
-    _url = options[1] if len(options) > 1 else options[0]
-    _label = options[0] if len(options) > 1 else "origin"
-
-    try:
-        with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
-            fair_session.add_remote(_url, _label)
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@remote.command()
-@click.argument("label")
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-def remove(label: str, debug: bool) -> None:
-    """Removes the specified remote from the remotes list
-
-    Parameters
-    ----------
-    label : str
-        label of remote to remove
-    """
-    try:
-        with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
-            fair_session.remove_remove(label)
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@remote.command()
-@click.argument("label")
-@click.argument("url")
-@click.pass_context
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-def modify(ctx, label: str, url: str, debug: bool) -> None:
-    """Modify a remote address"""
-    try:
-        with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
-            fair_session.modify_remote(label, url)
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@cli.command()
-@click.argument("remote", nargs=-1)
-@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
-@click.option(
-    "--dirty/--clean",
-    help="Allow running with uncommitted changes",
-    default=False,
-)
-def push(remote: str, debug: bool, dirty: bool):
-    """Push data between the local and remote registry"""
-    remote = remote[0] if remote else "origin"
-    try:
-        with fdp_session.FAIR(
-            os.getcwd(),
-            debug=debug,
-            server_mode=fdp_svr.SwitchMode.CLI,
-            allow_dirty=dirty,
-        ) as fair_session:
-            fair_session.push(remote)
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-@cli.group()
-def config():
-    """Configure user information"""
-    pass
-
-
-@config.command(name="user.name")
-@click.argument("user_name")
-def config_user(user_name: str) -> None:
-    fdp_conf.set_user(os.getcwd(), user_name)
-
-
-@config.command(name="user.email")
-@click.argument("user_email")
-def config_email(user_email: str) -> None:
-    fdp_conf.set_email(os.getcwd(), user_email)
-
-
-@cli.command()
-@click.argument("config", nargs=-1)
-@click.option("--debug/--no-debug")
-@click.option(
-    "--local/--no-local",
-    help="init without a remote registry - useful for closed systems",
-    default=False,
-)
-def pull(config: str, debug: bool, local: bool):
-    """Update local registry from remotes and sources"""
-    config = config[0] if config else fdp_com.local_user_config(os.getcwd())
-    try:
-        with fdp_session.FAIR(
-            os.getcwd(),
-            config,
-            server_mode=fdp_svr.SwitchMode.CLI,
-            debug=debug,
-            local=local,
-            allow_dirty=True,
-        ) as fair:
-            fair.pull()
-    except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
-        e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
-
-
-if __name__ in "__main__":
-    cli()
+#!/usr/bin/env python3
+# flake8: noqa
+# -*- coding: utf-8 -*-
+"""
+Command Line Interface
+======================
+
+Main command line interface setup script for creation of commands used to
+interact with the synchronisation tool.
+"""
+
+__date__ = "2021-06-24"
+
+import glob
+import logging
+from multiprocessing import context
+import os
+import pathlib
+import sys
+import typing
+
+import click
+import click.shell_completion
+import yaml
+
+import fair.common as fdp_com
+import fair.configuration as fdp_conf
+import fair.exceptions as fdp_exc
+import fair.history as fdp_hist
+import fair.registry.server as fdp_svr
+import fair.run as fdp_run
+import fair.session as fdp_session
+
+__author__ = "Scottish COVID Response Consortium"
+__credits__ = [
+    "Richard Reeve (University of Glasgow)",
+    "Nathan Cummings (UKAEA)",
+    "Kristian Zarebski (UKAEA)",
+    "Dennis Reddyhoff (University of Sheffield)",
+    "Ryan Field (University of Glasgow)",
+]
+__license__ = "BSD-2-Clause"
+__status__ = "Development"
+__copyright__ = "Copyright 2021, FAIR Data Pipeline"
+
+
+def complete_yamls(ctx, param, incomplete):
+    _file_list: typing.List[str] = [
+        str(i) for i in pathlib.Path(os.getcwd()).rglob("*.yaml")
+    ]
+    _file_list += [str(i) for i in pathlib.Path(os.getcwd()).rglob("*.yml")]
+    return [
+        click.shell_completion.CompletionItem(k)
+        for k in _file_list
+        if k.startswith(incomplete)
+    ]
+
+
+def complete_data_products(ctx, param, incomplete) -> typing.List[str]:
+    _staging_file = fdp_com.staging_cache(os.getcwd())
+    if not os.path.exists(_staging_file):
+        return []
+    _staging_data = yaml.safe_load(open(_staging_file))
+    _candidates = list(_staging_data["data_product"].keys())
+    return [
+        click.shell_completion.CompletionItem(c)
+        for c in _candidates
+        if c.startswith(incomplete)
+    ]
+
+
+def complete_jobs(ctx, param, incomplete) -> typing.List[str]:
+    _log_dir = fdp_hist.history_directory(os.getcwd())
+    _job_dir = fdp_com.default_jobs_dir()
+    if not os.path.isdir(_log_dir) or not os.path.isdir(_job_dir):
+        return []
+    _job_dirs = glob.glob(os.path.join(_job_dir, "*"))
+    _jobs = [fdp_run.get_job_hash(jd) for jd in _job_dirs]
+    return [
+        click.shell_completion.CompletionItem(j)
+        for j in _jobs
+        if j.startswith(incomplete)
+    ]
+
+
+@click.group()
+@click.version_option(package_name="fair-cli")
+@click.pass_context
+def cli(ctx):
+    """Welcome to FAIR-CLI, the FAIR data pipeline command-line interface."""
+    pass
+
+
+@cli.command()
+@click.option("--verbose/--not-verbose", help="Display URLs", default=False)
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+def status(verbose, debug) -> None:
+    """Get the status of files under staging"""
+    try:
+        with fdp_session.FAIR(
+            os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
+        ) as fair_session:
+            fair_session.status_data_products()
+            fair_session.status_code_runs()
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+@cli.group(invoke_without_command=True)
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+@click.option("--remote", help="Show Remote Code Runs", default= "")
+@click.pass_context
+def list(ctx, debug, remote) -> None:
+    """Commands to list data_product(s) and code_run(s)"""
+    if ctx.obj is None:
+        ctx.obj = {}
+    ctx.obj['DEBUG'] = debug
+    ctx.obj['REMOTE'] = remote
+    ctx.invoke(data_products)
+    ctx.invoke(code_runs)
+
+@list.command()
+@click.pass_context
+def data_products(ctx) -> None:
+    debug = ctx.obj['DEBUG']
+    remote = ctx.obj['REMOTE']
+    try:
+        with fdp_session.FAIR(
+            os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
+        ) as fair_session:
+            fair_session.show_all_data_products(remote = remote)
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+@list.command()
+@click.pass_context
+def code_runs(ctx) -> None:
+    debug = ctx.obj['DEBUG']
+    remote = ctx.obj['REMOTE']
+    try:
+        with fdp_session.FAIR(
+            os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
+        ) as fair_session:
+            fair_session.show_all_code_runs(remote = remote)
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+@cli.command()
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+@click.argument("output", nargs=-1)
+def create(debug, output: str) -> None:
+    """Generate a new FAIR repository user YAML config file"""
+    output = (
+        output[0]
+        if output
+        else os.path.join(os.getcwd(), fdp_com.USER_CONFIG_FILE)
+    )
+    click.echo(f"Generating new user configuration file" f" '{output}'")
+    with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
+        fair_session.make_starter_config(output)
+
+
+@cli.command()
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+def reset(debug: bool) -> None:
+    """Unstage all items marked for staging"""
+    try:
+        with fdp_session.FAIR(
+            os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
+        ) as fair_session:
+            fair_session.reset_staging()
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@cli.command()
+@click.option(
+    "--config",
+    help="Create a starter user config.yaml file during initialisation",
+    default=None,
+)
+@click.option(
+    "--using",
+    help="Initialise the CLI system from an existing CLI global configuration file",
+    default="",
+    shell_complete=complete_yamls,
+)
+@click.option(
+    "--registry",
+    help="Specify registry directory",
+    default=None,
+    show_default=True,
+)
+@click.option(
+    "--ci/--standard",
+    help="Run in testing mode for a CI system",
+    default=False,
+)
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+@click.option(
+    "--export", help="Export the CLI configuration to a file", default=""
+)
+@click.option(
+    "--local/--no-local",
+    help="init without a remote registry - useful for closed systems",
+    default=False,
+)
+def init(
+    config: str,
+    debug: bool,
+    using: str,
+    registry: str,
+    ci: bool,
+    local: bool,
+    export: str = "",
+) -> None:
+    """Initialise repository in current location"""
+    try:
+        with fdp_session.FAIR(
+            os.getcwd(), None, debug=debug, testing=ci, local=local
+        ) as fair_session:
+            _use_dict = {}
+            if using:
+                if not os.path.exists(using):
+                    raise fdp_exc.FileNotFoundError(
+                        f"Cannot load CLI configuration from file '{using}', "
+                        "file does not exist."
+                    )
+                _use_dict = yaml.safe_load(open(using))
+
+            fair_session.initialise(
+                using=_use_dict,
+                registry=registry,
+                export_as=export,
+                local=local,
+            )
+            if config:
+                fair_session.make_starter_config(config)
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@cli.command()
+@click.option(
+    "glob",
+    "--global/--no-global",
+    help="Also delete global FAIR-CLI directories",
+    default=False,
+)
+@click.option(
+    "--yes/--no",
+    help="Deletes the configurations specified without prompt",
+    default=False,
+)
+@click.option(
+    "--data/--no-data",
+    help="Also delete the local data directory",
+    default=False,
+)
+@click.option(
+    "--all/--not-all",
+    help="Remove all FAIR interfaces and registry",
+    default=False,
+)
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+def purge(glob: bool, debug: bool, yes: bool, data: bool, all: bool) -> None:
+    # sourcery skip: avoid-builtin-shadow
+    """Resets the repository deleting all local caches"""
+    _purge = yes
+
+    if all:
+        all = click.confirm(
+            "Are you sure you want to remove all FAIR components from this system?\n"
+            "WARNING: This will also remove your local registry"
+        )
+    else:
+        _purge = click.confirm(
+            "Are you sure you want to reset FAIR tracking, "
+            "this is not reversible?"
+        )
+        if data:
+            data = click.confirm(
+                "Are you sure you want to delete the local data directory?\n"
+                "WARNING: Do not do this if you have a populated local registry"
+            )
+        if not _purge:
+            return
+
+    try:
+        with fdp_session.FAIR(os.getcwd()) as fair_session:
+            fair_session.purge(global_cfg=glob, clear_data=data, clear_all=all)
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@cli.group()
+def registry() -> None:
+    """Commands relating to control of the local registry server"""
+    pass
+
+
+@registry.command()
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+def uninstall(debug: bool):
+    """Uninstall the local registry from the system"""
+    _confirm = click.confirm(
+        "Are you sure you want to remove the local registry and its components?",
+        default=False,
+    )
+    if not _confirm:
+        return
+    try:
+        if debug:
+            logging.getLogger("FAIRDataPipeline").setLevel(logging.DEBUG)
+        fdp_svr.uninstall_registry()
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@registry.command()
+@click.option("--force/--no-force", help="Force a reinstall", default=False)
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+@click.option("--directory", help="Installation location", default=None)
+@click.option(
+    "--version",
+    help="Specify version tag of registry to install, else latest repo tag",
+    default=None,
+)
+def install(debug: bool, force: bool, directory: str, version: str):
+    """Install the local registry on the system"""
+    try:
+        if debug:
+            logging.getLogger("FAIRDataPipeline").setLevel(logging.DEBUG)
+        _version = fdp_svr.install_registry(
+            install_dir=directory, reference=version, force=force
+        )
+        click.echo(f"Installed registry version '{_version}'")
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@registry.command()
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+@click.option("--port", help="port on which to run registry", default=8000)
+@click.option("--address", help="Address on which to run registry", default="127.0.0.1")
+def start(debug: bool, port: int, address: str) -> None:
+    """Start the local registry server"""
+    try:
+        fdp_session.FAIR(
+            os.getcwd(),
+            server_mode=fdp_svr.SwitchMode.USER_START,
+            debug=debug,
+            server_port=port,
+            server_address=address
+        )
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@registry.command()
+@click.option("--force/--no-force", help="Force server stop", default=False)
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+def stop(force: bool, debug: bool) -> None:
+    """Stop the local registry server"""
+    _mode = (
+        fdp_svr.SwitchMode.FORCE_STOP
+        if force
+        else fdp_svr.SwitchMode.USER_STOP
+    )
+    try:
+        fdp_session.FAIR(os.getcwd(), server_mode=_mode, debug=debug)
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@registry.command()
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+def status(debug) -> None:
+    try:
+        with fdp_session.FAIR(
+            os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.NO_SERVER
+        ) as fair_session:
+            fair_session.registry_status()
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@cli.command()
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+def log(debug: bool) -> None:
+    """Show a full job history"""
+    try:
+        fdp_hist.show_history(os.getcwd())
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@cli.command()
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+@click.argument("job_id", shell_complete=complete_jobs)
+def view(job_id: str, debug: bool) -> None:
+    """View log for a given job"""
+    try:
+        fdp_hist.show_job_log(os.getcwd(), job_id)
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@cli.command()
+@click.argument("identifier")
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+@click.option("-j", "--job/--no-job", help="Stage entire job", default=False)
+def unstage(identifier: str, debug: bool, job: bool) -> None:
+    """Remove data products or jobs from staging"""
+    try:
+        with fdp_session.FAIR(
+            os.getcwd(),
+            debug=debug,
+        ) as fair_session:
+            fair_session.change_staging_state(
+                identifier,
+                job,
+                stage=False,
+            )
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@cli.command()
+@click.argument("identifier", shell_complete=complete_data_products)
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+def add(identifier: str, debug: bool) -> None:
+    """
+    Add a data product or coderun to staging
+
+    Data Products should be formatted: 
+    <namespace>:<data product name>@v<version>
+    eg:
+    PSU:SEIRS_model/parameters@v1.0.0
+
+    Code Runs should be specified by code run uuid
+
+    Use `fair list` to view Data Products and Code Runs
+    
+    """
+    try:
+        with fdp_session.FAIR(
+            os.getcwd(),
+            debug=debug,
+        ) as fair_session:
+            fair_session.add_to_staging(
+                identifier
+            )
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@cli.command()
+@click.argument("job_ids", nargs=-1)
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+@click.option(
+    "--cached/--not-cached",
+    default=False,
+    help="remove from tracking but do not delete from file system",
+)
+def rm(
+    job_ids: typing.List[str], cached: bool = False, debug: bool = False
+) -> None:
+    """Removes jobs from system or just tracking"""
+    pass
+
+
+@cli.command()
+@click.argument("config", nargs=-1)
+@click.option(
+    "--script",
+    help="Specify a shell command to execute, this will be inserted into the working config",
+    default="",
+)
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+@click.option(
+    "--ci/--no-ci",
+    help="Calls run passively without executing any commands for a CI system",
+    default=False,
+)
+@click.option(
+    "--dirty/--clean",
+    help="Allow running with uncommitted changes",
+    default=False,
+)
+@click.option(
+    "--local/--no-local",
+    help="init without a remote registry - useful for closed systems",
+    default=False,
+)
+def run(
+    config: str, script: str, debug: bool, ci: bool, dirty: bool, local: bool
+):
+    """Initialises a job with the option to specify a bash command"""
+    # Allow no config to be specified, if that is the case use default local
+    config = config[0] if config else fdp_com.local_user_config(os.getcwd())
+    try:
+        with fdp_session.FAIR(
+            os.getcwd(),
+            config,
+            debug=debug,
+            server_mode=fdp_svr.SwitchMode.CLI,
+            allow_dirty=dirty,
+            local=local,
+        ) as fair_session:
+            _hash = fair_session.run(
+                script, passive=ci, allow_dirty=dirty, local=local
+            )
+            if ci:
+                click.echo(fdp_run.get_job_dir(_hash))
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@cli.group(invoke_without_command=True)
+@click.option("--verbose/--no-verbose", "-v/")
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+@click.pass_context
+def remote(ctx, verbose: bool = False, debug: bool = False):
+    """List remotes if no additional command is provided"""
+    if not ctx.invoked_subcommand:
+        try:
+            with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
+                fair_session.list_remotes(verbose)
+        except fdp_exc.FAIRCLIException as e:
+            if debug:
+                raise e
+            e.err_print()
+            if e.level.lower() == "error":
+                sys.exit(e.exit_code)
+
+
+@remote.command()
+@click.argument("options", nargs=-1)
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+def add(options: typing.List[str], debug: bool) -> None:
+    """Add a remote registry URL with option to give it a label if multiple
+    remotes may be used.
+
+    Parameters
+    ----------
+    options : typing.List[str]
+        size 1 or 2 list containing either:
+            - label, url
+            - url
+    """
+    _url = options[1] if len(options) > 1 else options[0]
+    _label = options[0] if len(options) > 1 else "origin"
+
+    try:
+        with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
+            fair_session.add_remote(_url, _label)
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@remote.command()
+@click.argument("label")
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+def remove(label: str, debug: bool) -> None:
+    """Removes the specified remote from the remotes list
+
+    Parameters
+    ----------
+    label : str
+        label of remote to remove
+    """
+    try:
+        with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
+            fair_session.remove_remove(label)
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@remote.command()
+@click.argument("label")
+@click.argument("url")
+@click.pass_context
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+def modify(ctx, label: str, url: str, debug: bool) -> None:
+    """Modify a remote address"""
+    try:
+        with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
+            fair_session.modify_remote(label, url)
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@cli.command()
+@click.argument("remote", nargs=-1)
+@click.option("--debug/--no-debug", help="Run in debug mode", default=False)
+@click.option(
+    "--dirty/--clean",
+    help="Allow running with uncommitted changes",
+    default=False,
+)
+def push(remote: str, debug: bool, dirty: bool):
+    """Push data between the local and remote registry"""
+    remote = remote[0] if remote else "origin"
+    try:
+        with fdp_session.FAIR(
+            os.getcwd(),
+            debug=debug,
+            server_mode=fdp_svr.SwitchMode.CLI,
+            allow_dirty=dirty,
+        ) as fair_session:
+            fair_session.push(remote)
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+@cli.group()
+def config():
+    """Configure user information"""
+    pass
+
+
+@config.command(name="user.name")
+@click.argument("user_name")
+def config_user(user_name: str) -> None:
+    fdp_conf.set_user(os.getcwd(), user_name)
+
+
+@config.command(name="user.email")
+@click.argument("user_email")
+def config_email(user_email: str) -> None:
+    fdp_conf.set_email(os.getcwd(), user_email)
+
+
+@cli.command()
+@click.argument("config", nargs=-1)
+@click.option("--debug/--no-debug")
+@click.option(
+    "--local/--no-local",
+    help="init without a remote registry - useful for closed systems",
+    default=False,
+)
+def pull(config: str, debug: bool, local: bool):
+    """Update local registry from remotes and sources"""
+    config = config[0] if config else fdp_com.local_user_config(os.getcwd())
+    try:
+        with fdp_session.FAIR(
+            os.getcwd(),
+            config,
+            server_mode=fdp_svr.SwitchMode.CLI,
+            debug=debug,
+            local=local,
+            allow_dirty=True,
+        ) as fair:
+            fair.pull()
+    except fdp_exc.FAIRCLIException as e:
+        if debug:
+            raise e
+        e.err_print()
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
+
+
+if __name__ in "__main__":
+    cli(obj={})
```

### Comparing `fair_cli-0.5.2/fair/common.py` & `fair_cli-0.7.0/fair/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,299 +1,299 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-"""
-
-Common Paths
-============
-
-Functions and constant strings related to the location of directories
-and files for executing a CLI session.
-
-
-Contents
-========
-
-Members
--------
-    USER_FAIR_DIR   - user FAIR directory
-    FAIR_CLI_CONFIG - name of the FAIR-CLI configuration file
-    FAIR_FOLDER     - name for FAIR local repository directory
-
-Functions
--------
-    registry_home       - returns the location of the local data registry
-    find_fair_root      - returns the closest '.fair' directory in the upper hierarchy
-    find_git_root       - returns the closest '.git' directory
-    staging_cache       - returns the current repository staging cache directory
-    default_data_dir    - returns the default data store
-    local_fdpconfig     - returns path of FAIR-CLI local repository config
-    local_user_config   - returns the path of the user config in the given folder
-    default_jobs_dir    - returns the default jobs folder
-    global_config_dir   - returns the FAIR-CLI global config directory
-    global_fdpconfig    - returns path of FAIR-CLI global config
-    session_cache_dir   - returns location of session cache folder
-
-"""
-__date__ = "2021-06-28"
-
-import enum
-import os
-import pathlib
-import logging
-import stat
-
-import git
-import yaml
-
-import fair.exceptions as fdp_exc
-
-_logger = logging.getLogger("FAIRDataPipeline.Common")
-
-USER_FAIR_DIR = os.path.join(pathlib.Path.home(), ".fair")
-FAIR_CLI_CONFIG = "cli-config.yaml"
-USER_CONFIG_FILE = "config.yaml"
-FAIR_FOLDER = ".fair"
-JOBS_DIR = "jobs"
-
-FAIR_REGISTRY_REPO = "https://github.com/FAIRDataPipeline/data-registry.git"
-
-DEFAULT_REGISTRY_DOMAIN = "https://data.scrc.uk/"
-REGISTRY_INSTALL_URL = "https://data.scrc.uk/static/localregistry.sh"
-
-DEFAULT_REGISTRY_LOCATION = os.path.join(
-    pathlib.Path().home(), FAIR_FOLDER, "registry"
-)
-
-DEFAULT_LOCAL_REGISTRY_URL = "http://127.0.0.1:8000/api/"
-
-
-class CMD_MODE(enum.Enum):
-    RUN = 1
-    PULL = 2
-    PUSH = 3
-    PASS = 4
-
-
-def registry_home() -> str:
-    if not os.path.exists(global_fdpconfig()):
-        if "FAIR_REGISTRY_DIR" in os.environ:
-            return os.environ["FAIR_REGISTRY_DIR"]
-        else:
-            return DEFAULT_REGISTRY_LOCATION
-    _glob_conf = yaml.safe_load(open(global_fdpconfig()))
-    if not _glob_conf:
-        return DEFAULT_REGISTRY_LOCATION
-    if "registries" not in _glob_conf:
-        raise fdp_exc.CLIConfigurationError(
-            "Expected key 'registries' in global CLI configuration"
-        )
-
-    if "local" not in _glob_conf["registries"]:
-        raise fdp_exc.CLIConfigurationError(
-            "Expected 'local' registry in global CLI configuration registries"
-        )
-
-    if "directory" not in _glob_conf["registries"]["local"]:
-        raise fdp_exc.CLIConfigurationError(
-            "Expected directory of local registry in global CLI configuration"
-        )
-
-    return _glob_conf["registries"]["local"]["directory"]
-
-
-def find_fair_root(start_directory: str = os.getcwd()) -> str:
-    """Locate the .fair folder within the current hierarchy
-
-    Parameters
-    ----------
-
-    start_directory : str, optional
-        starting point for local FAIR folder search
-
-    Returns
-    -------
-    str
-        absolute path of the .fair folder
-    """
-    _current_dir = os.path.abspath(start_directory)
-
-    while _current_dir:
-        # If the home directory has been reached then abort as upper file system
-        # is outside user area, also we do not want to return global FAIR folder
-        if str(_current_dir) == str(pathlib.Path().home()):
-            return ""
-
-        if os.path.exists(os.path.join(_current_dir, FAIR_FOLDER)):
-            return _current_dir
-        _current_dir, _directory = os.path.split(_current_dir)
-
-        # If there is no directory component this means the top of the file
-        # system has been reached
-        if not _directory:
-            return ""
-
-
-def registry_session_port_file(registry_dir: str = None) -> str:
-    """Retrieve the location of the registry session port file
-
-    Parameters
-    ----------
-    registry_dir : str, optional
-        registry directory, by default None
-
-    Returns
-    -------
-    str
-        path to registry port session file
-    """
-    if not registry_dir:
-        registry_dir = registry_home()
-    return os.path.join(registry_dir, "session_port.log")
-
-def registry_session_address_file(registry_dir: str = None) -> str:
-    """Retrieve the location of the registry session port file
-
-    Parameters
-    ----------
-    registry_dir : str, optional
-        registry directory, by default None
-
-    Returns
-    -------
-    str
-        path to registry port session file
-    """
-    if not registry_dir:
-        registry_dir = registry_home()
-    return os.path.join(registry_dir, "session_address.log")
-
-
-def registry_session_port(registry_dir: str = None) -> int:
-    """Retrieve the registry session port
-
-    Unlike 'get_local_port' within the configuration module, this retrieves the
-    port number from the file generated by the registry itself
-
-    Parameters
-    ----------
-    registry_dir : str, optional
-        registry directory, by default None
-
-    Returns
-    -------
-    int
-        current/most recent port used to launch the registry
-    """
-    return int(open(registry_session_port_file(registry_dir)).read().strip())
-
-def registry_session_address(registry_dir: str = None) -> str:
-    """Retrieve the registry session address
-
-    Unlike 'get_local_address' within the configuration module, this retrieves the
-    port number from the file generated by the registry itself
-
-    Parameters
-    ----------
-    registry_dir : str, optional
-        registry directory, by default None
-
-    Returns
-    -------
-    str
-        current/most recent address used to launch the registry
-    """
-    if not os.path.exists(registry_session_address_file(registry_dir)):
-        _logger.warning("Session Address file not found, please make sure your registry is up-to-date")
-        _logger.info("Using 127.0.0.1")
-        return "127.0.0.1"
-
-    _address = open(registry_session_address_file(registry_dir)).read().strip()
-    if _address != "0.0.0.0":
-        return _address
-    else:
-        return "127.0.0.1"
-
-
-def staging_cache(user_loc: str) -> str:
-    """Location of staging cache for the given repository"""
-    return os.path.abspath(
-        os.path.join(find_fair_root(user_loc), FAIR_FOLDER, "staging")
-    )
-
-
-def default_data_dir(location: str = "local") -> str:
-    """Location of the default data store"""
-    if not os.path.exists(global_fdpconfig()):
-        raise fdp_exc.InternalError(
-            f"Failed to read CLI global config file '{global_fdpconfig()}'"
-        )
-    _glob_conf = yaml.safe_load(open(global_fdpconfig()))
-    if "data_store" in _glob_conf["registries"][location]:
-        return _glob_conf["registries"][location]["data_store"]
-    if location == "local":
-        return os.path.join(USER_FAIR_DIR, f"data{os.path.sep}")
-    else:
-        raise fdp_exc.UserConfigError(
-            "Cannot guess remote data store location"
-        )
-
-
-def local_fdpconfig(user_loc: str = os.getcwd()) -> str:
-    """Location of the FAIR-CLI configuration file for the given repository"""
-    return os.path.join(find_fair_root(user_loc), FAIR_FOLDER, FAIR_CLI_CONFIG)
-
-
-def local_user_config(user_loc: str = os.getcwd()) -> str:
-    """Location of the default user configuration file for the given repository"""
-    return os.path.join(find_fair_root(user_loc), USER_CONFIG_FILE)
-
-
-def default_jobs_dir() -> str:
-    """Default location to place job outputs"""
-    return os.path.join(default_data_dir(), JOBS_DIR)
-
-
-def global_config_dir() -> str:
-    """Directory of global CLI configuration"""
-    return os.path.join(USER_FAIR_DIR, "cli")
-
-
-def session_cache_dir() -> str:
-    """Location of run files used to determine if server is being used"""
-    return os.path.join(global_config_dir(), "sessions")
-
-
-def global_fdpconfig() -> str:
-    """Location of global CLI configuration"""
-    return os.path.join(global_config_dir(), FAIR_CLI_CONFIG)
-
-
-def find_git_root(start_directory: str = os.getcwd()) -> str:
-    """Locate the .git folder within the current hierarchy
-
-    Parameters
-    ----------
-
-    start_directory : str, optional
-        starting point for local git folder search
-
-    Returns
-    -------
-    str
-        absolute path of the .git folder
-    """
-    try:
-        _repository = git.Repo(start_directory, search_parent_directories=True)
-    except git.InvalidGitRepositoryError as e:
-        raise fdp_exc.UserConfigError(
-            "Failed to retrieve git repository for current configuration"
-            f" in location '{start_directory}'"
-        ) from e
-
-    return _repository.git.rev_parse("--show-toplevel").strip()
-
-def set_file_permissions(path: str):
-    for root, dirs, files in os.walk(path, topdown=False):
-        for dir in [os.path.join(root,d) for d in dirs]:
-            os.chmod(dir, stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO)
-        for file in [os.path.join(root, f) for f in files]:
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+"""
+
+Common Paths
+============
+
+Functions and constant strings related to the location of directories
+and files for executing a CLI session.
+
+
+Contents
+========
+
+Members
+-------
+    USER_FAIR_DIR   - user FAIR directory
+    FAIR_CLI_CONFIG - name of the FAIR-CLI configuration file
+    FAIR_FOLDER     - name for FAIR local repository directory
+
+Functions
+-------
+    registry_home       - returns the location of the local data registry
+    find_fair_root      - returns the closest '.fair' directory in the upper hierarchy
+    find_git_root       - returns the closest '.git' directory
+    staging_cache       - returns the current repository staging cache directory
+    default_data_dir    - returns the default data store
+    local_fdpconfig     - returns path of FAIR-CLI local repository config
+    local_user_config   - returns the path of the user config in the given folder
+    default_jobs_dir    - returns the default jobs folder
+    global_config_dir   - returns the FAIR-CLI global config directory
+    global_fdpconfig    - returns path of FAIR-CLI global config
+    session_cache_dir   - returns location of session cache folder
+
+"""
+__date__ = "2021-06-28"
+
+import enum
+import os
+import pathlib
+import logging
+import stat
+
+import git
+import yaml
+
+import fair.exceptions as fdp_exc
+
+_logger = logging.getLogger("FAIRDataPipeline.Common")
+
+USER_FAIR_DIR = os.path.join(pathlib.Path.home(), ".fair")
+FAIR_CLI_CONFIG = "cli-config.yaml"
+USER_CONFIG_FILE = "config.yaml"
+FAIR_FOLDER = ".fair"
+JOBS_DIR = "jobs"
+
+FAIR_REGISTRY_REPO = "https://github.com/FAIRDataPipeline/data-registry.git"
+
+DEFAULT_REGISTRY_DOMAIN = "https://data.fairdatapipeline.org/"
+REGISTRY_INSTALL_URL = "https://data.fairdatapipeline.org/static/localregistry.sh"
+
+DEFAULT_REGISTRY_LOCATION = os.path.join(
+    pathlib.Path().home(), FAIR_FOLDER, "registry"
+)
+
+DEFAULT_LOCAL_REGISTRY_URL = "http://127.0.0.1:8000/api/"
+
+
+class CMD_MODE(enum.Enum):
+    RUN = 1
+    PULL = 2
+    PUSH = 3
+    PASS = 4
+
+
+def registry_home() -> str:
+    if not os.path.exists(global_fdpconfig()):
+        if "FAIR_REGISTRY_DIR" in os.environ:
+            return os.environ["FAIR_REGISTRY_DIR"]
+        else:
+            return DEFAULT_REGISTRY_LOCATION
+    _glob_conf = yaml.safe_load(open(global_fdpconfig()))
+    if not _glob_conf:
+        return DEFAULT_REGISTRY_LOCATION
+    if "registries" not in _glob_conf:
+        raise fdp_exc.CLIConfigurationError(
+            "Expected key 'registries' in global CLI configuration"
+        )
+
+    if "local" not in _glob_conf["registries"]:
+        raise fdp_exc.CLIConfigurationError(
+            "Expected 'local' registry in global CLI configuration registries"
+        )
+
+    if "directory" not in _glob_conf["registries"]["local"]:
+        raise fdp_exc.CLIConfigurationError(
+            "Expected directory of local registry in global CLI configuration"
+        )
+
+    return _glob_conf["registries"]["local"]["directory"]
+
+
+def find_fair_root(start_directory: str = os.getcwd()) -> str:
+    """Locate the .fair folder within the current hierarchy
+
+    Parameters
+    ----------
+
+    start_directory : str, optional
+        starting point for local FAIR folder search
+
+    Returns
+    -------
+    str
+        absolute path of the .fair folder
+    """
+    _current_dir = os.path.abspath(start_directory)
+
+    while _current_dir:
+        # If the home directory has been reached then abort as upper file system
+        # is outside user area, also we do not want to return global FAIR folder
+        if str(_current_dir) == str(pathlib.Path().home()):
+            return ""
+
+        if os.path.exists(os.path.join(_current_dir, FAIR_FOLDER)):
+            return _current_dir
+        _current_dir, _directory = os.path.split(_current_dir)
+
+        # If there is no directory component this means the top of the file
+        # system has been reached
+        if not _directory:
+            return ""
+
+
+def registry_session_port_file(registry_dir: str = None) -> str:
+    """Retrieve the location of the registry session port file
+
+    Parameters
+    ----------
+    registry_dir : str, optional
+        registry directory, by default None
+
+    Returns
+    -------
+    str
+        path to registry port session file
+    """
+    if not registry_dir:
+        registry_dir = registry_home()
+    return os.path.join(registry_dir, "session_port.log")
+
+def registry_session_address_file(registry_dir: str = None) -> str:
+    """Retrieve the location of the registry session port file
+
+    Parameters
+    ----------
+    registry_dir : str, optional
+        registry directory, by default None
+
+    Returns
+    -------
+    str
+        path to registry port session file
+    """
+    if not registry_dir:
+        registry_dir = registry_home()
+    return os.path.join(registry_dir, "session_address.log")
+
+
+def registry_session_port(registry_dir: str = None) -> int:
+    """Retrieve the registry session port
+
+    Unlike 'get_local_port' within the configuration module, this retrieves the
+    port number from the file generated by the registry itself
+
+    Parameters
+    ----------
+    registry_dir : str, optional
+        registry directory, by default None
+
+    Returns
+    -------
+    int
+        current/most recent port used to launch the registry
+    """
+    return int(open(registry_session_port_file(registry_dir)).read().strip())
+
+def registry_session_address(registry_dir: str = None) -> str:
+    """Retrieve the registry session address
+
+    Unlike 'get_local_address' within the configuration module, this retrieves the
+    port number from the file generated by the registry itself
+
+    Parameters
+    ----------
+    registry_dir : str, optional
+        registry directory, by default None
+
+    Returns
+    -------
+    str
+        current/most recent address used to launch the registry
+    """
+    if not os.path.exists(registry_session_address_file(registry_dir)):
+        _logger.warning("Session Address file not found, please make sure your registry is up-to-date")
+        _logger.info("Using 127.0.0.1")
+        return "127.0.0.1"
+
+    _address = open(registry_session_address_file(registry_dir)).read().strip()
+    if _address != "0.0.0.0":
+        return _address
+    else:
+        return "127.0.0.1"
+
+
+def staging_cache(user_loc: str) -> str:
+    """Location of staging cache for the given repository"""
+    return os.path.abspath(
+        os.path.join(find_fair_root(user_loc), FAIR_FOLDER, "staging")
+    )
+
+
+def default_data_dir(location: str = "local") -> str:
+    """Location of the default data store"""
+    if not os.path.exists(global_fdpconfig()):
+        raise fdp_exc.InternalError(
+            f"Failed to read CLI global config file '{global_fdpconfig()}'"
+        )
+    _glob_conf = yaml.safe_load(open(global_fdpconfig()))
+    if "data_store" in _glob_conf["registries"][location]:
+        return _glob_conf["registries"][location]["data_store"]
+    if location == "local":
+        return os.path.join(USER_FAIR_DIR, f"data{os.path.sep}")
+    else:
+        raise fdp_exc.UserConfigError(
+            "Cannot guess remote data store location"
+        )
+
+
+def local_fdpconfig(user_loc: str = os.getcwd()) -> str:
+    """Location of the FAIR-CLI configuration file for the given repository"""
+    return os.path.join(find_fair_root(user_loc), FAIR_FOLDER, FAIR_CLI_CONFIG)
+
+
+def local_user_config(user_loc: str = os.getcwd()) -> str:
+    """Location of the default user configuration file for the given repository"""
+    return os.path.join(find_fair_root(user_loc), USER_CONFIG_FILE)
+
+
+def default_jobs_dir() -> str:
+    """Default location to place job outputs"""
+    return os.path.join(default_data_dir(), JOBS_DIR)
+
+
+def global_config_dir() -> str:
+    """Directory of global CLI configuration"""
+    return os.path.join(USER_FAIR_DIR, "cli")
+
+
+def session_cache_dir() -> str:
+    """Location of run files used to determine if server is being used"""
+    return os.path.join(global_config_dir(), "sessions")
+
+
+def global_fdpconfig() -> str:
+    """Location of global CLI configuration"""
+    return os.path.join(global_config_dir(), FAIR_CLI_CONFIG)
+
+
+def find_git_root(start_directory: str = os.getcwd()) -> str:
+    """Locate the .git folder within the current hierarchy
+
+    Parameters
+    ----------
+
+    start_directory : str, optional
+        starting point for local git folder search
+
+    Returns
+    -------
+    str
+        absolute path of the .git folder
+    """
+    try:
+        _repository = git.Repo(start_directory, search_parent_directories=True)
+    except git.InvalidGitRepositoryError as e:
+        raise fdp_exc.UserConfigError(
+            "Failed to retrieve git repository for current configuration"
+            f" in location '{start_directory}'"
+        ) from e
+
+    return _repository.git.rev_parse("--show-toplevel").strip()
+
+def set_file_permissions(path: str):
+    for root, dirs, files in os.walk(path, topdown=False):
+        for dir in [os.path.join(root,d) for d in dirs]:
+            os.chmod(dir, stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO)
+        for file in [os.path.join(root, f) for f in files]:
             os.chmod(file, stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO)
```

### Comparing `fair_cli-0.5.2/fair/configuration/__init__.py` & `fair_cli-0.7.0/fair/configuration/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,879 +1,881 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-"""
-
-Configuration
-=============
-
-Module contains methods relating to configuration of the CLI itself.
-
-Contents
-========
-
-Functions
----------
-
-    read_local_fdpconfig - read the contents of the local CLI config file
-    read_global_fdpconfig - read the contents of the global CLI config file
-    set_email - set the user's email in the configuration
-    set_user - set the user's name in the configuration
-    get_current_user_name - retrieve name of the current user
-    get_current_user_email - retrieve email of the current user
-    get_remote_uri - retrieve URL for the remote registry
-    local_git_repo - retrieve path for the current project Git repository
-    remote_git_repo - retrieve URL for the remote Git repository
-    get_remote_token - retrieve the token for the remote registry
-    get_session_git_remote - get the current git remote label or URL
-    get_current_user_uri - retrieve the full URL identifier for the current user
-    get_current_user_uuid - retrieve the uuid of the current user if specified
-    check_registry_exists - check that the specified local registry directory exists
-    get_local_uri - retrieve the URL of the local registry
-    get_local_port - retrieve the port number of the local registry
-    global_config_query - setup the global configuration using prompts
-    local_config_query - setup the local configuration using prompts
-    write_data_store - retrieve the current write data store
-    input_namespace - retrieve current input namespace
-    output_namespace - retrieve current output namespace
-    is_public - retrieve the current data is_public label
-    read_version - retrieve the current data read version
-    write_version - retrieve the current data write
-    registry_url - retrieves either local or remote registry URL
-    update_metadata - updates the metadata within a use configuration file
-"""
-
-__date__ = "2021-07-02"
-
-import copy
-import logging
-import os
-import pathlib
-import typing
-import uuid
-from urllib.parse import urljoin, urlparse
-
-import click
-import git
-import yaml
-
-import fair.common as fdp_com
-import fair.exceptions as fdp_exc
-import fair.identifiers as fdp_id
-import fair.registry.requests as fdp_req
-import fair.registry.server as fdp_serv
-
-logger = logging.getLogger("FAIRDataPipeline.Configuration")
-
-
-def read_local_fdpconfig(repo_loc: str) -> typing.MutableMapping:
-    """Read contents of repository level FAIR-CLI configurations.
-
-    Parameters
-    ----------
-    repo_loc : str
-        FAIR-CLI repository directory
-
-    Returns
-    -------
-    MutableMapping
-        configurations as a mapping
-    """
-    _local_config: typing.MutableMapping = {}
-
-    # Retrieve the location of this repositories CLI config file
-    _local_config_file_addr = fdp_com.local_fdpconfig(repo_loc)
-    if os.path.exists(_local_config_file_addr):
-        _local_config = yaml.safe_load(open(_local_config_file_addr))
-
-    return _local_config
-
-
-def read_global_fdpconfig() -> typing.MutableMapping:
-    """Read contents of the global FAIR-CLI configurations.
-
-    Returns
-    -------
-    MutableMapping
-        configurations as a mapping
-    """
-    _global_config: typing.MutableMapping = {}
-
-    # Retrieve the location of the global CLI config file
-    _global_config_addr = fdp_com.global_fdpconfig()
-
-    if os.path.exists(_global_config_addr):
-        _global_config = yaml.safe_load(open(_global_config_addr))
-
-    return _global_config
-
-
-def set_email(repo_loc: str, email: str, is_global: bool = False) -> None:
-    """Update the email address for the user
-
-    Parameters
-    ----------
-    repo_loc : str
-        repository directory path
-    email : str
-        new email address to set
-    is_global : bool, optional
-        whether to also override the global settings, by default False
-    """
-    _loc_conf = read_local_fdpconfig(repo_loc)
-    _loc_conf["user"]["email"] = email
-    yaml.dump(_loc_conf, open(fdp_com.local_fdpconfig(repo_loc), "w"))
-    if is_global:
-        _glob_conf = read_global_fdpconfig()
-        _glob_conf["user"]["email"] = email
-        yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), "w"))
-
-
-def set_user(repo_loc: str, name: str, is_global: bool = False) -> None:
-    """Update the name for the user
-
-    Parameters
-    ----------
-    repo_loc : str
-        repository directory path
-    name : str
-        new user full name
-    is_global : bool, optional
-        whether to also override the global settings, by default False
-    """
-    _loc_conf = read_local_fdpconfig(repo_loc)
-    if len(name.split()) > 1:
-        _given_name, _family_name = name.rsplit(" ", 1)
-        _loc_conf["user"]["given_names"] = _given_name.title().strip()
-        _loc_conf["user"]["family_name"] = _family_name.title().strip()
-        if is_global:
-            _glob_conf = read_global_fdpconfig()
-            _glob_conf["user"]["given_names"] = _given_name.title().strip()
-            _glob_conf["user"]["family_name"] = _family_name.title().strip()
-            yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), "w"))
-    else:
-        _loc_conf["user"]["given_names"] = name.title().strip()
-        _loc_conf["user"]["family_name"] = None
-        if is_global:
-            _glob_conf = read_global_fdpconfig()
-            _glob_conf["user"]["given_names"] = name.title().strip()
-            _glob_conf["user"]["family_name"] = None
-            yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), "w"))
-    yaml.dump(_loc_conf, open(fdp_com.local_fdpconfig(repo_loc), "w"))
-    if is_global:
-        _glob_conf = read_global_fdpconfig()
-        _glob_conf["user"]["name"] = name
-        yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), "w"))
-
-
-def get_current_user_name(repo_loc: str) -> typing.Tuple[str]:
-    """Retrieves the name of the current session user as defined in the config
-
-    Returns
-    -------
-    str
-        user name
-    """
-    _local_conf = read_local_fdpconfig(repo_loc)
-
-    if not _local_conf:
-        raise fdp_exc.CLIConfigurationError(
-            "Cannot retrieve current user from empty CLI config"
-        )
-
-    _given = _local_conf["user"]["given_names"]
-    if "family_name" in _local_conf["user"]:
-        _family = _local_conf["user"]["family_name"]
-    else:
-        _family = ""
-    return (_given, _family)
-
-
-def get_current_user_email(repo_loc: str) -> typing.Tuple[str]:
-    """Retrieves the email of the current session user as defined in the config
-
-    Returns
-    -------
-    str
-        user email
-    """
-    _local_conf = read_local_fdpconfig(repo_loc)
-
-    if not _local_conf:
-        raise fdp_exc.CLIConfigurationError(
-            "Cannot retrieve current user from empty CLI config"
-        )
-
-    return _local_conf["user"]["email"]
-
-
-def get_remote_uri(repo_loc: str, remote_label: str = "origin") -> str:
-    """Retrieves the URI of the remote registry
-
-    Parameters
-    ----------
-    repo_locget_remote_token : str
-        local FAIR repository directory
-    remote_label : str, optional
-        label of remote to retrieve, default is 'origin'
-
-    Returns
-    -------
-    str
-        remote URI path
-    """
-    _local_conf = read_local_fdpconfig(repo_loc)
-    return _local_conf["registries"][remote_label]["uri"]
-
-
-def local_git_repo(fair_repo_loc: str) -> str:
-    """Retriget_remote_token root git repository directory"""
-    _local_conf = read_local_fdpconfig(fair_repo_loc)
-
-    try:
-        return _local_conf["git"]["local_repo"]
-    except KeyError as e:
-        raise fdp_exc.CLIConfigurationError(
-            "Expected key 'git:local_repo' in local CLI configuration"
-        ) from e
-
-
-def remote_git_repo(fair_repo_loc: str) -> str:
-    """Retrieves the remote repository git directory
-
-    Parameters
-    ----------
-    fair_repo_loc : str
-        FAIR repository location
-
-    Returns
-    -------
-    str
-        the git repository remote URL
-    """
-
-    _local_conf = read_local_fdpconfig(fair_repo_loc)
-
-    try:
-        return _local_conf["git"]["remote_repo"]
-    except KeyError as e:
-        raise fdp_exc.CLIConfigurationError(
-            "Expected key 'git:remote_repo' in local CLI configuration"
-        ) from e
-
-
-def get_remote_token(
-    repo_dir: str, remote: str = "origin", local: bool = False
-) -> str:
-    _local_config = read_local_fdpconfig(repo_dir)
-    if remote not in _local_config["registries"]:
-        raise fdp_exc.CLIConfigurationError(
-            f"Cannot find remote registry '{remote}' in local CLI configuration"
-        )
-    if "token" not in _local_config["registries"][remote]:
-        raise fdp_exc.CLIConfigurationError(
-            f"Cannot find token for registry '{remote}', no token file provided"
-        )
-    _token_file = _local_config["registries"][remote]["token"]
-    if not _token_file:
-        logger.warning("\n not token file found \n")
-        return None
-    if not local:
-        if not os.path.exists(_token_file):
-            raise fdp_exc.FileNotFoundError(
-                f"Cannot read token for registry '{remote}', token file '{_token_file}'"
-                " does not exist"
-            )
-
-        _token = open(_token_file).read().strip()
-
-        if not _token:
-            raise fdp_exc.CLIConfigurationError(
-                f"Cannot read token from file '{_token_file}', file is empty."
-            )
-
-        return _token
-    return None
-
-
-def get_local_data_store() -> str:
-    """Retrieves the local data store path"""
-    _global_conf = read_global_fdpconfig()
-
-    try:
-        return _global_conf["registries"]["local"]["data_store"]
-    except KeyError as e:
-        raise fdp_exc.CLIConfigurationError(
-            "Expected key 'registries:local:data_store' in global CLI configuration"
-        ) from e
-
-
-def get_session_git_remote(repo_loc: str, url: bool = False) -> str:
-    """Retrieves the local repository git remote
-
-    Parameters
-    ----------
-    repo_loc : str
-        Location of session CLI config
-    url : optional, bool
-        If True return the URL for the remote instead
-
-    Returns
-    -------
-    str
-        the remote label or URL of the git repository
-    """
-    _local_conf = read_local_fdpconfig(repo_loc)
-
-    try:
-        _remote_label = _local_conf["git"]["remote"]
-    except KeyError as e:
-        raise fdp_exc.InternalError(
-            "Failed to retrieve project git repository remote"
-        ) from e
-
-    if not url:
-        return _remote_label
-
-    _repo_root = fdp_com.find_git_root(repo_loc)
-
-    try:
-        return git.Repo(_repo_root).remote(_remote_label).url
-    except ValueError as e:
-        raise fdp_exc.CLIConfigurationError(
-            f"Failed to retrieve URL for git remote '{_remote_label}'"
-        ) from e
-
-
-def get_current_user_uuid(repo_loc: str) -> str:
-    """Retrieves the UUID of the current session user if defined in the config
-
-    Returns
-    -------
-    str
-        user UUID
-    """
-    _local_conf = read_local_fdpconfig(repo_loc)
-    try:
-        _uuid = _local_conf["user"]["uuid"]
-    except KeyError:
-        _uuid = None
-    if not _uuid or _uuid == "None":
-        raise fdp_exc.CLIConfigurationError("No UUID defined.")
-    return _uuid
-
-
-def get_current_user_uri(repo_loc: str) -> str:
-    """Retrieves the URI identifier for the current user
-
-    Returns
-    -------
-    str
-        user URI identifier
-    """
-    _local_conf = read_local_fdpconfig(repo_loc)
-    try:
-        _uri = _local_conf["user"]["uri"]
-    except KeyError:
-        _uri = None
-    if not _uri or _uri == "None":
-        raise fdp_exc.CLIConfigurationError("No user URI identifier defined.")
-    return _uri
-
-
-def check_registry_exists(registry: str = None) -> typing.Optional[str]:
-    """Checks if fair registry is set up on users machine
-
-    Returns
-    -------
-    str
-        registry location if found
-    """
-    if not registry:
-        registry = fdp_com.DEFAULT_REGISTRY_LOCATION
-    if os.path.isdir(registry):
-        return registry
-
-
-def get_local_uri() -> str:
-    """Retrieve the local registry URI"""
-    _global_conf = read_global_fdpconfig()
-
-    if not _global_conf:
-        return fdp_com.DEFAULT_LOCAL_REGISTRY_URL
-
-    try:
-        return _global_conf["registries"]["local"]["uri"]
-    except KeyError as e:
-        raise fdp_exc.CLIConfigurationError(
-            "Expected key 'registries:local:uri' in global CLI configuration"
-        ) from e
-
-
-def set_local_uri(uri: str) -> str:
-    """Sets the local URI
-
-    Parameters
-    ----------
-    uri: str
-        new local URI for the registry
-    """
-    _global_conf = read_global_fdpconfig()
-
-    _global_conf["registries"]["local"]["uri"] = uri
-
-    with open(fdp_com.global_fdpconfig(), "w") as out_f:
-        yaml.dump(_global_conf, out_f)
-
-
-def get_local_port(local_uri: str = None) -> int:
-    """Retrieve the local port from the local URI"""
-    if not local_uri:
-        local_uri = get_local_uri()
-    _port = urlparse(local_uri).port
-    if not _port:
-        raise fdp_exc.InternalError(
-            "Failed to determine port number from local registry URL"
-        )
-    return _port
-
-
-def update_local_port() -> str:
-    """Updates the local port in the global configuration from the session port file"""
-    _current_port = fdp_com.registry_session_port()
-    _current_address = fdp_com.registry_session_address()
-
-    _new_url = f'http://{_current_address}:{_current_port}/api/'
-
-    if os.path.exists(fdp_com.global_fdpconfig()) and read_global_fdpconfig():
-        _glob_conf = read_global_fdpconfig()
-        _glob_conf["registries"]["local"]["uri"] = _new_url
-        with open(fdp_com.global_fdpconfig(), "w") as out_f:
-            yaml.dump(_glob_conf, out_f)
-
-    return _new_url
-
-
-def _handle_orcid(user_orcid: str) -> typing.Tuple[typing.Dict, str]:
-    """Extract the name information from an ORCID selection
-
-    Parameters
-    ----------
-    user_orcid : str
-        ORCID to search
-
-    Returns
-    -------
-    user_info : typing.Dict
-        dictionary of extracted name metadata
-    str
-        default output namespace
-    """
-    _user_info = fdp_id.check_orcid(user_orcid.strip())
-
-    while not _user_info:
-        click.echo("Invalid ORCID given.")
-        user_orcid = click.prompt("ORCID")
-        _user_info = fdp_id.check_orcid(user_orcid.strip())
-
-    _user_info["orcid"] = user_orcid
-
-    click.echo(
-        f"Found entry: {_user_info['given_names']} {_user_info['family_name']}"
-    )
-
-    _def_ospace = "".join(_user_info["given_names"]).lower()
-
-    _def_ospace += _user_info["family_name"].lower().replace(" ", "")
-
-    return _user_info, _def_ospace
-
-
-def _handle_ror(user_ror: str) -> typing.Tuple[typing.Dict, str]:
-    """Extract institution name information from an ROR ID
-
-    Parameters
-    ----------
-    user_ror : str
-        ROR ID for an institution
-
-    Returns
-    -------
-    user_info : typing.Dict
-        dictionary of extracted name metadata
-    str
-        default output namespace
-    """
-    _user_info = fdp_id.check_ror(user_ror.strip())
-
-    while not _user_info:
-        click.echo("Invalid ROR ID given.")
-        user_ror = click.prompt("ROR ID")
-        _user_info = fdp_id.check_ror(user_ror.strip())
-
-    _user_info["ror"] = user_ror
-
-    click.echo(f"Found entry: {_user_info['family_name']} ")
-
-    _def_ospace = _user_info["family_name"].lower().replace(" ", "_")
-
-    return _user_info, _def_ospace
-
-
-def _handle_grid(user_grid: str) -> typing.Tuple[typing.Dict, str]:
-    """Extract institution name information from an GRID ID
-
-    Parameters
-    ----------
-    user_grid : str
-        GRID ID for an institution
-
-    Returns
-    -------
-    user_info : typing.Dict
-        dictionary of extracted name metadata
-    str
-        default output namespace
-    """
-    _user_info = fdp_id.check_grid(user_grid.strip())
-
-    while not _user_info:
-        click.echo("Invalid GRID ID given.")
-        user_grid = click.prompt("GRID ID")
-        _user_info = fdp_id.check_grid(user_grid.strip())
-
-    _user_info["grid"] = user_grid
-
-    click.echo(f"Found entry: {_user_info['family_name']} ")
-
-    _def_ospace = _user_info["family_name"].lower().replace(" ", "_")
-
-    return _user_info, _def_ospace
-
-
-def _handle_uuid() -> typing.Tuple[typing.Dict, str]:
-    """Obtain metadata for user where no ID provided
-
-    Returns
-    -------
-    user_info : typing.Dict
-        dictionary of extracted name metadata
-    str
-        default output namespace
-    """
-    _full_name = click.prompt("Full Name")
-    _def_ospace = ""
-    _user_info = {}
-    if len(_full_name.split()) > 1:
-        _given_name, _family_name = _full_name.split(" ", 1)
-        _def_ospace = _full_name.lower().replace(" ", "")
-        _user_info["given_names"] = _given_name.strip()
-        _user_info["family_name"] = _family_name.strip()
-    else:
-        _def_ospace += _full_name
-        _user_info["given_names"] = _full_name
-        _user_info["family_name"] = None
-
-    return _user_info, _def_ospace
-
-
-def _get_user_info_and_namespaces() -> typing.Dict[str, typing.Dict]:
-    _user_email = click.prompt("Email")
-
-    _invalid_input = True
-
-    while _invalid_input:
-        _id_type = click.prompt(
-            "User ID system (ORCID/ROR/GRID/None)", default="None"
-        )
-
-        if _id_type.upper() == "ORCID":
-            _user_orcid = click.prompt("ORCID")
-            _user_info, _def_ospace = _handle_orcid(_user_orcid)
-            _invalid_input = False
-        elif _id_type.upper() == "ROR":
-            _user_ror = click.prompt("ROR ID")
-            _user_info, _def_ospace = _handle_ror(_user_ror)
-            _invalid_input = False
-        elif _id_type.upper() == "GRID":
-            _user_grid = click.prompt("GRID ID")
-            _user_info, _def_ospace = _handle_grid(_user_grid)
-            _invalid_input = False
-        elif _id_type.upper() == "NONE":
-            _user_info, _def_ospace = _handle_uuid()
-            _user_uuid = str(uuid.uuid4())
-            _user_info["uuid"] = _user_uuid
-            _invalid_input = False
-
-    _user_info["email"] = _user_email
-
-    _def_ospace = _def_ospace.lower().replace(" ", "").strip()
-    _def_ospace = click.prompt("Default output namespace", default=_def_ospace)
-    _def_ispace = click.prompt("Default input namespace", default=_def_ospace)
-
-    _namespaces = {"input": _def_ispace, "output": _def_ospace}
-
-    return {"user": _user_info, "namespaces": _namespaces}
-
-
-def global_config_query(
-    registry: str = None, local: bool = False
-) -> typing.Dict[str, typing.Any]:
-    """Ask user question set for creating global FAIR config"""
-    logger.debug(
-        "Running global configuration query with registry at '%s'", registry
-    )
-    click.echo("Checking for local registry")
-    if not registry and "FAIR_REGISTRY_DIR" in os.environ:
-        registry = os.environ["FAIR_REGISTRY_DIR"]
-    if check_reg := check_registry_exists(registry):
-        registry = check_reg
-        click.echo(f"Local registry found at '{check_reg}'")
-    elif not registry:
-        if _ := click.confirm(
-            "Local registry not found at default location"
-            f"'{fdp_com.DEFAULT_REGISTRY_LOCATION}', "
-            "would you like to specify an existing installation?",
-            default=False,
-        ):
-            _reg_loc = click.prompt("Local registry directory")
-            _manage_script = os.path.join(_reg_loc, "manage.py")
-            while not os.path.exists(_manage_script):
-                click.echo(
-                    f"Error: Location '{_reg_loc}' is not a valid registry installation"
-                )
-                _reg_loc = click.prompt("Local registry directory")
-                _manage_script = os.path.join(_reg_loc, "manage.py")
-        else:
-            registry = fdp_com.DEFAULT_REGISTRY_LOCATION
-            fdp_serv.install_registry(install_dir=registry)
-    else:
-        click.echo(f"Will install registry to '{registry}'")
-        fdp_serv.install_registry(install_dir=registry)
-
-    _local_port: int = click.prompt("Local Registry Port", default="8000")
-    _local_uri = fdp_com.DEFAULT_LOCAL_REGISTRY_URL.replace(
-        ":8000", f":{_local_port}"
-    )
-    if local:
-        _remote_url = "http://127.0.0.1:8000/api/"
-        _rem_key_file = os.path.join(registry, "token")
-        _rem_data_store = os.path.join(os.curdir, "data_store") + os.path.sep
-    else:
-        _default_rem = urljoin(fdp_com.DEFAULT_REGISTRY_DOMAIN, "api/")
-        _remote_url = click.prompt("Remote API URL", default=_default_rem)
-
-        _rem_data_store = click.prompt(
-            "Remote Data Storage Root",
-            default=_remote_url.replace("api", "data"),
-        )
-
-        _rem_key_file = click.prompt(
-            "Remote API Token File",
-        )
-        _rem_key_file = os.path.expandvars(_rem_key_file)
-
-        while (
-            not os.path.exists(_rem_key_file)
-            or not open(_rem_key_file).read().strip()
-        ):
-            click.echo(
-                f"Token file '{_rem_key_file}' does not exist or is empty, "
-                "please provide a valid token file."
-            )
-            _rem_key_file = click.prompt("Remote API Token File")
-            _rem_key_file = os.path.expandvars(_rem_key_file)
-
-    if not fdp_serv.check_server_running():
-        if _ := click.confirm(
-            "Local registry is offline, would you like to start it?",
-            default=False,
-        ):
-            fdp_serv.launch_server(registry_dir=registry)
-
-            # Keep server running by creating user run cache file
-            _cache_addr = os.path.join(fdp_com.session_cache_dir(), "user.run")
-            pathlib.Path(_cache_addr).touch()
-
-        else:
-            click.echo("Temporarily launching server to retrieve API token.")
-            fdp_serv.launch_server(registry_dir=registry)
-            fdp_serv.stop_server(registry_dir=registry, local_uri=_local_uri)
-            try:
-                fdp_req.local_token(registry_dir=registry)
-            except fdp_exc.FileNotFoundError as e:
-                raise fdp_exc.RegistryError(
-                    "Failed to retrieve local API token from registry."
-                ) from e
-
-    _loc_data_store = click.prompt(
-        "Default Data Store",
-        default=os.path.join(fdp_com.USER_FAIR_DIR, "data/"),
-    )
-    if _loc_data_store[-1] != os.path.sep:
-        _loc_data_store += os.path.sep
-
-    _glob_conf_dict = _get_user_info_and_namespaces()
-    _glob_conf_dict["registries"] = {
-        "local": {
-            "uri": _local_uri,
-            "directory": os.path.abspath(registry),
-            "data_store": _loc_data_store,
-            "token": os.path.join(os.path.abspath(registry), "token"),
-        },
-        "origin": {
-            "uri": _remote_url,
-            "token": _rem_key_file,
-            "data_store": _rem_data_store,
-        },
-    }
-
-    return _glob_conf_dict
-
-
-def local_config_query(
-    global_config: typing.Dict[str, typing.Any] = read_global_fdpconfig(),
-    first_time_setup: bool = False,
-    local: bool = False,
-) -> typing.Dict[str, typing.Any]:
-    """Ask user questions to create local user config
-
-    Parameters
-    ----------
-    global_config : Dict[str, Any], optional
-        global configuration dictionary
-    first_time_setup : bool, optional
-        if first time need to setup globals as well, by default False
-
-    Returns
-    -------
-    Dict[str, Any]
-        dictionary of local configurations
-    """
-    # Try extracting global configurations. If any keys do not exist re-run
-    # setup for creation of these, then try again.
-    try:
-        _def_remote = global_config["registries"]["origin"]["uri"]
-        _def_rem_key = global_config["registries"]["origin"]["token"]
-        _def_ospace = global_config["namespaces"]["output"]
-        _def_user = global_config["user"]
-    except KeyError:
-        click.echo(
-            "Error: Failed to read global configuration, re-running global setup."
-        )
-        first_time_setup = True
-        global_config = global_config_query()
-        _def_remote = global_config["registries"]["origin"]["uri"]
-        _def_rem_key = global_config["registries"]["origin"]["token"]
-        _def_ospace = global_config["namespaces"]["output"]
-        _def_user = global_config["user"]
-
-    # Allow the user to continue without an input namespace as some
-    # functionality does not require this.
-    if (
-        "input" not in global_config["namespaces"]
-        or not global_config["namespaces"]
-    ):
-        click.echo(f"Will use '{_def_ospace}' as default input namespace")
-        _def_ispace = _def_ospace
-    else:
-        _def_ispace = global_config["namespaces"]["input"]
-
-    # Try checking to see if the current location is a git repository and
-    # suggesting this as a default
-    try:
-        _git_repo = fdp_com.find_git_root(os.getcwd())
-    except fdp_exc.UserConfigError:
-        _git_repo = None
-
-    _git_repo = click.prompt("Local Git repository", default=_git_repo)
-    _invalid_repo = True
-
-    # Check this is indeed a git repository
-    while _invalid_repo:
-        try:
-            git.Repo(_git_repo)
-            _invalid_repo = False
-        except (git.InvalidGitRepositoryError, git.NoSuchPathError):
-            _invalid_repo = True
-            click.echo(
-                "Invalid directory, location is not the head of a local"
-                " git repository."
-            )
-            _git_repo = click.prompt("Local Git repository")
-
-    # Set the remote to use within git by label, by default 'origin'
-    # check the remote label is valid before proceeding
-    try:
-        git.Repo(_git_repo).remotes["origin"]
-        _def_rem = "origin"
-    except IndexError:
-        _def_rem = None
-
-    _git_remote = click.prompt("Git remote name", default=_def_rem)
-    _invalid_rem = True
-
-    while _invalid_rem and _def_rem:
-        try:
-            git.Repo(_git_repo).remotes[_git_remote]
-            _invalid_rem = False
-        except IndexError:
-            _invalid_rem = True
-            click.echo("Invalid remote name for git repository")
-            _git_remote = click.prompt("Git remote name", default=_def_rem)
-
-    _repo = git.Repo(_git_repo)
-
-    while _git_remote not in _repo.remotes:
-        click.echo(f"Git remote label '{_git_remote}' does not exist")
-        _git_remote = click.prompt("Git remote name")
-
-    _git_remote_repo = _repo.remotes[_git_remote].url
-
-    click.echo(
-        f"Using git repository remote '{_git_remote}': {_git_remote_repo}"
-    )
-
-    # If this is not the first setup it means globals are available so these
-    # can be suggested as defaults during local setup
-    if not first_time_setup or not local:
-        _def_remote = click.prompt("Remote API URL", default=_def_remote)
-        _def_rem_key = click.prompt(
-            "Remote API Token File", default=_def_rem_key
-        )
-        _def_rem_key = os.path.expandvars(_def_rem_key)
-
-        while (
-            not os.path.exists(_def_rem_key)
-            or not open(_def_rem_key).read().strip()
-        ):
-            click.echo(
-                f"Token file '{_def_rem_key}' does not exist or is empty, "
-                "please provide a valid token file."
-            )
-            _def_rem_key = click.prompt("Remote API Token File")
-            _def_rem_key = os.path.expandvars(_def_rem_key)
-        _def_ospace = click.prompt(
-            "Default output namespace", default=_def_ospace
-        )
-        _def_ispace = click.prompt(
-            "Default input namespace", default=_def_ispace
-        )
-
-    _local_config: typing.Dict[str, typing.Any] = {
-        "namespaces": {"output": _def_ospace, "input": _def_ispace},
-        "git": {
-            "remote": _git_remote,
-            "local_repo": _git_repo,
-            "remote_repo": _git_remote_repo,
-        },
-        "registries": copy.deepcopy(global_config["registries"]),
-    }
-
-    # Local registry is a globally defined entity
-    del _local_config["registries"]["local"]
-
-    _local_config["registries"]["origin"]["uri"] = _def_remote
-    _local_config["registries"]["origin"]["token"] = _def_rem_key
-
-    _local_config["user"] = _def_user
-
-    return _local_config
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+"""
+
+Configuration
+=============
+
+Module contains methods relating to configuration of the CLI itself.
+
+Contents
+========
+
+Functions
+---------
+
+    read_local_fdpconfig - read the contents of the local CLI config file
+    read_global_fdpconfig - read the contents of the global CLI config file
+    set_email - set the user's email in the configuration
+    set_user - set the user's name in the configuration
+    get_current_user_name - retrieve name of the current user
+    get_current_user_email - retrieve email of the current user
+    get_remote_uri - retrieve URL for the remote registry
+    local_git_repo - retrieve path for the current project Git repository
+    remote_git_repo - retrieve URL for the remote Git repository
+    get_remote_token - retrieve the token for the remote registry
+    get_session_git_remote - get the current git remote label or URL
+    get_current_user_uri - retrieve the full URL identifier for the current user
+    get_current_user_uuid - retrieve the uuid of the current user if specified
+    check_registry_exists - check that the specified local registry directory exists
+    get_local_uri - retrieve the URL of the local registry
+    get_local_port - retrieve the port number of the local registry
+    global_config_query - setup the global configuration using prompts
+    local_config_query - setup the local configuration using prompts
+    write_data_store - retrieve the current write data store
+    input_namespace - retrieve current input namespace
+    output_namespace - retrieve current output namespace
+    is_public - retrieve the current data is_public label
+    read_version - retrieve the current data read version
+    write_version - retrieve the current data write
+    registry_url - retrieves either local or remote registry URL
+    update_metadata - updates the metadata within a use configuration file
+"""
+
+__date__ = "2021-07-02"
+
+import copy
+import logging
+import os
+import pathlib
+import typing
+import uuid
+from urllib.parse import urljoin, urlparse
+
+import click
+import git
+import yaml
+
+import fair.common as fdp_com
+import fair.exceptions as fdp_exc
+import fair.identifiers as fdp_id
+import fair.registry.requests as fdp_req
+import fair.registry.server as fdp_serv
+
+logger = logging.getLogger("FAIRDataPipeline.Configuration")
+
+
+def read_local_fdpconfig(repo_loc: str) -> typing.MutableMapping:
+    """Read contents of repository level FAIR-CLI configurations.
+
+    Parameters
+    ----------
+    repo_loc : str
+        FAIR-CLI repository directory
+
+    Returns
+    -------
+    MutableMapping
+        configurations as a mapping
+    """
+    _local_config: typing.MutableMapping = {}
+
+    # Retrieve the location of this repositories CLI config file
+    _local_config_file_addr = fdp_com.local_fdpconfig(repo_loc)
+    if os.path.exists(_local_config_file_addr):
+        _local_config = yaml.safe_load(open(_local_config_file_addr))
+
+    return _local_config
+
+
+def read_global_fdpconfig() -> typing.MutableMapping:
+    """Read contents of the global FAIR-CLI configurations.
+
+    Returns
+    -------
+    MutableMapping
+        configurations as a mapping
+    """
+    _global_config: typing.MutableMapping = {}
+
+    # Retrieve the location of the global CLI config file
+    _global_config_addr = fdp_com.global_fdpconfig()
+
+    if os.path.exists(_global_config_addr):
+        _global_config = yaml.safe_load(open(_global_config_addr))
+
+    return _global_config
+
+
+def set_email(repo_loc: str, email: str, is_global: bool = False) -> None:
+    """Update the email address for the user
+
+    Parameters
+    ----------
+    repo_loc : str
+        repository directory path
+    email : str
+        new email address to set
+    is_global : bool, optional
+        whether to also override the global settings, by default False
+    """
+    _loc_conf = read_local_fdpconfig(repo_loc)
+    _loc_conf["user"]["email"] = email
+    yaml.dump(_loc_conf, open(fdp_com.local_fdpconfig(repo_loc), "w"))
+    if is_global:
+        _glob_conf = read_global_fdpconfig()
+        _glob_conf["user"]["email"] = email
+        yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), "w"))
+
+
+def set_user(repo_loc: str, name: str, is_global: bool = False) -> None:
+    """Update the name for the user
+
+    Parameters
+    ----------
+    repo_loc : str
+        repository directory path
+    name : str
+        new user full name
+    is_global : bool, optional
+        whether to also override the global settings, by default False
+    """
+    _loc_conf = read_local_fdpconfig(repo_loc)
+    if len(name.split()) > 1:
+        _given_name, _family_name = name.rsplit(" ", 1)
+        _loc_conf["user"]["given_names"] = _given_name.title().strip()
+        _loc_conf["user"]["family_name"] = _family_name.title().strip()
+        if is_global:
+            _glob_conf = read_global_fdpconfig()
+            _glob_conf["user"]["given_names"] = _given_name.title().strip()
+            _glob_conf["user"]["family_name"] = _family_name.title().strip()
+            yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), "w"))
+    else:
+        _loc_conf["user"]["given_names"] = name.title().strip()
+        _loc_conf["user"]["family_name"] = None
+        if is_global:
+            _glob_conf = read_global_fdpconfig()
+            _glob_conf["user"]["given_names"] = name.title().strip()
+            _glob_conf["user"]["family_name"] = None
+            yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), "w"))
+    yaml.dump(_loc_conf, open(fdp_com.local_fdpconfig(repo_loc), "w"))
+    if is_global:
+        _glob_conf = read_global_fdpconfig()
+        _glob_conf["user"]["name"] = name
+        yaml.dump(_glob_conf, open(fdp_com.global_fdpconfig(), "w"))
+
+
+def get_current_user_name(repo_loc: str) -> typing.Tuple[str]:
+    """Retrieves the name of the current session user as defined in the config
+
+    Returns
+    -------
+    str
+        user name
+    """
+    _local_conf = read_local_fdpconfig(repo_loc)
+
+    if not _local_conf:
+        raise fdp_exc.CLIConfigurationError(
+            "Cannot retrieve current user from empty CLI config"
+        )
+
+    _given = _local_conf["user"]["given_names"]
+    if "family_name" in _local_conf["user"]:
+        _family = _local_conf["user"]["family_name"]
+    else:
+        _family = ""
+    return (_given, _family)
+
+
+def get_current_user_email(repo_loc: str) -> typing.Tuple[str]:
+    """Retrieves the email of the current session user as defined in the config
+
+    Returns
+    -------
+    str
+        user email
+    """
+    _local_conf = read_local_fdpconfig(repo_loc)
+
+    if not _local_conf:
+        raise fdp_exc.CLIConfigurationError(
+            "Cannot retrieve current user from empty CLI config"
+        )
+
+    return _local_conf["user"]["email"]
+
+
+def get_remote_uri(repo_loc: str, remote_label: str = "origin") -> str:
+    """Retrieves the URI of the remote registry
+
+    Parameters
+    ----------
+    repo_loc : str
+        local FAIR repository directory
+    remote_label : str, optional
+        label of remote to retrieve, default is 'origin'
+
+    Returns
+    -------
+    str
+        remote URI path
+    """
+    _local_conf = read_local_fdpconfig(repo_loc)
+    return _local_conf["registries"][remote_label]["uri"]
+
+
+def local_git_repo(fair_repo_loc: str) -> str:
+    """Retriget_remote_token root git repository directory"""
+    _local_conf = read_local_fdpconfig(fair_repo_loc)
+
+    try:
+        return _local_conf["git"]["local_repo"]
+    except KeyError as e:
+        raise fdp_exc.CLIConfigurationError(
+            "Expected key 'git:local_repo' in local CLI configuration"
+        ) from e
+
+
+def remote_git_repo(fair_repo_loc: str) -> str:
+    """Retrieves the remote repository git directory
+
+    Parameters
+    ----------
+    fair_repo_loc : str
+        FAIR repository location
+
+    Returns
+    -------
+    str
+        the git repository remote URL
+    """
+
+    _local_conf = read_local_fdpconfig(fair_repo_loc)
+
+    try:
+        return _local_conf["git"]["remote_repo"]
+    except KeyError as e:
+        raise fdp_exc.CLIConfigurationError(
+            "Expected key 'git:remote_repo' in local CLI configuration"
+        ) from e
+
+
+def get_remote_token(
+    repo_dir: str, remote: str = "origin", local: bool = False
+) -> str:
+    _local_config = read_local_fdpconfig(repo_dir)
+    if remote not in _local_config["registries"]:
+        raise fdp_exc.CLIConfigurationError(
+            f"Cannot find remote registry '{remote}' in local CLI configuration"
+        )
+    if "token" not in _local_config["registries"][remote]:
+        raise fdp_exc.CLIConfigurationError(
+            f"Cannot find token for registry '{remote}', no token file provided"
+        )
+    _token_file = _local_config["registries"][remote]["token"]
+    if not _token_file:
+        logger.warning("\n not token file found \n")
+        return None
+    if not local:
+        if not os.path.exists(_token_file):
+            raise fdp_exc.FileNotFoundError(
+                f"Cannot read token for registry '{remote}', token file '{_token_file}'"
+                " does not exist"
+            )
+
+        _token = open(_token_file).read().strip()
+
+        if not _token:
+            raise fdp_exc.CLIConfigurationError(
+                f"Cannot read token from file '{_token_file}', file is empty."
+            )
+
+        return _token
+    return None
+
+
+def get_local_data_store() -> str:
+    """Retrieves the local data store path"""
+    _global_conf = read_global_fdpconfig()
+
+    try:
+        return _global_conf["registries"]["local"]["data_store"]
+    except KeyError as e:
+        raise fdp_exc.CLIConfigurationError(
+            "Expected key 'registries:local:data_store' in global CLI configuration"
+        ) from e
+
+
+def get_session_git_remote(repo_loc: str, url: bool = False) -> str:
+    """Retrieves the local repository git remote
+
+    Parameters
+    ----------
+    repo_loc : str
+        Location of session CLI config
+    url : optional, bool
+        If True return the URL for the remote instead
+
+    Returns
+    -------
+    str
+        the remote label or URL of the git repository
+    """
+    _local_conf = read_local_fdpconfig(repo_loc)
+
+    try:
+        _remote_label = _local_conf["git"]["remote"]
+    except KeyError as e:
+        raise fdp_exc.InternalError(
+            "Failed to retrieve project git repository remote"
+        ) from e
+
+    if not url:
+        return _remote_label
+
+    _repo_root = fdp_com.find_git_root(repo_loc)
+
+    try:
+        return git.Repo(_repo_root).remote(_remote_label).url
+    except ValueError as e:
+        raise fdp_exc.CLIConfigurationError(
+            f"Failed to retrieve URL for git remote '{_remote_label}'"
+        ) from e
+
+
+def get_current_user_uuid(repo_loc: str) -> str:
+    """Retrieves the UUID of the current session user if defined in the config
+
+    Returns
+    -------
+    str
+        user UUID
+    """
+    _local_conf = read_local_fdpconfig(repo_loc)
+    try:
+        _uuid = _local_conf["user"]["uuid"]
+    except KeyError:
+        _uuid = None
+    if not _uuid or _uuid == "None":
+        raise fdp_exc.CLIConfigurationError("No UUID defined.")
+    return _uuid
+
+
+def get_current_user_uri(repo_loc: str) -> str:
+    """Retrieves the URI identifier for the current user
+
+    Returns
+    -------
+    str
+        user URI identifier
+    """
+    _local_conf = read_local_fdpconfig(repo_loc)
+    try:
+        _uri = _local_conf["user"]["uri"]
+    except KeyError:
+        _uri = None
+    if not _uri or _uri == "None":
+        raise fdp_exc.CLIConfigurationError("No user URI identifier defined.")
+    return _uri
+
+
+def check_registry_exists(registry: str = None) -> typing.Optional[str]:
+    """Checks if fair registry is set up on users machine
+
+    Returns
+    -------
+    str
+        registry location if found
+    """
+    if not registry:
+        registry = fdp_com.DEFAULT_REGISTRY_LOCATION
+    if os.path.isdir(registry):
+        return registry
+
+
+def get_local_uri() -> str:
+    """Retrieve the local registry URI"""
+    _global_conf = read_global_fdpconfig()
+
+    if not _global_conf:
+        return fdp_com.DEFAULT_LOCAL_REGISTRY_URL
+
+    try:
+        return _global_conf["registries"]["local"]["uri"]
+    except KeyError as e:
+        raise fdp_exc.CLIConfigurationError(
+            "Expected key 'registries:local:uri' in global CLI configuration"
+        ) from e
+
+
+def set_local_uri(uri: str) -> str:
+    """Sets the local URI
+
+    Parameters
+    ----------
+    uri: str
+        new local URI for the registry
+    """
+    _global_conf = read_global_fdpconfig()
+
+    _global_conf["registries"]["local"]["uri"] = uri
+
+    with open(fdp_com.global_fdpconfig(), "w") as out_f:
+        yaml.dump(_global_conf, out_f)
+
+
+def get_local_port(local_uri: str = None) -> int:
+    """Retrieve the local port from the local URI"""
+    if not local_uri:
+        local_uri = get_local_uri()
+    _port = urlparse(local_uri).port
+    if not _port:
+        raise fdp_exc.InternalError(
+            "Failed to determine port number from local registry URL"
+        )
+    return _port
+
+
+def update_local_port() -> str:
+    """Updates the local port in the global configuration from the session port file"""
+    _current_port = fdp_com.registry_session_port()
+    _current_address = fdp_com.registry_session_address()
+
+    _new_url = f'http://{_current_address}:{_current_port}/api/'
+
+    if os.path.exists(fdp_com.global_fdpconfig()) and read_global_fdpconfig():
+        _glob_conf = read_global_fdpconfig()
+        _glob_conf["registries"]["local"]["uri"] = _new_url
+        with open(fdp_com.global_fdpconfig(), "w") as out_f:
+            yaml.dump(_glob_conf, out_f)
+
+    return _new_url
+
+
+def _handle_orcid(user_orcid: str) -> typing.Tuple[typing.Dict, str]:
+    """Extract the name information from an ORCID selection
+
+    Parameters
+    ----------
+    user_orcid : str
+        ORCID to search
+
+    Returns
+    -------
+    user_info : typing.Dict
+        dictionary of extracted name metadata
+    str
+        default output namespace
+    """
+    _user_info = fdp_id.check_orcid(user_orcid.strip())
+
+    while not _user_info:
+        click.echo("Invalid ORCID given.")
+        user_orcid = click.prompt("ORCID")
+        _user_info = fdp_id.check_orcid(user_orcid.strip())
+
+    _user_info["orcid"] = user_orcid
+
+    click.echo(
+        f"Found entry: {_user_info['given_names']} {_user_info['family_name']}"
+    )
+
+    _def_ospace = "".join(_user_info["given_names"]).lower()
+
+    _def_ospace += _user_info["family_name"].lower().replace(" ", "")
+
+    return _user_info, _def_ospace
+
+
+def _handle_ror(user_ror: str) -> typing.Tuple[typing.Dict, str]:
+    """Extract institution name information from an ROR ID
+
+    Parameters
+    ----------
+    user_ror : str
+        ROR ID for an institution
+
+    Returns
+    -------
+    user_info : typing.Dict
+        dictionary of extracted name metadata
+    str
+        default output namespace
+    """
+    _user_info = fdp_id.check_ror(user_ror.strip())
+
+    while not _user_info:
+        click.echo("Invalid ROR ID given.")
+        user_ror = click.prompt("ROR ID")
+        _user_info = fdp_id.check_ror(user_ror.strip())
+
+    _user_info["ror"] = user_ror
+
+    click.echo(f"Found entry: {_user_info['family_name']} ")
+
+    _def_ospace = _user_info["family_name"].lower().replace(" ", "_")
+
+    return _user_info, _def_ospace
+
+
+def _handle_grid(user_grid: str) -> typing.Tuple[typing.Dict, str]:
+    """Extract institution name information from an GRID ID
+
+    Parameters
+    ----------
+    user_grid : str
+        GRID ID for an institution
+
+    Returns
+    -------
+    user_info : typing.Dict
+        dictionary of extracted name metadata
+    str
+        default output namespace
+    """
+    _user_info = fdp_id.check_grid(user_grid.strip())
+
+    while not _user_info:
+        click.echo("Invalid GRID ID given.")
+        user_grid = click.prompt("GRID ID")
+        _user_info = fdp_id.check_grid(user_grid.strip())
+
+    _user_info["grid"] = user_grid
+
+    click.echo(f"Found entry: {_user_info['family_name']} ")
+
+    _def_ospace = _user_info["family_name"].lower().replace(" ", "_")
+
+    return _user_info, _def_ospace
+
+
+def _handle_uuid() -> typing.Tuple[typing.Dict, str]:
+    """Obtain metadata for user where no ID provided
+
+    Returns
+    -------
+    user_info : typing.Dict
+        dictionary of extracted name metadata
+    str
+        default output namespace
+    """
+    _full_name = click.prompt("Full Name")
+    _def_ospace = ""
+    _user_info = {}
+    if len(_full_name.split()) > 1:
+        _given_name, _family_name = _full_name.split(" ", 1)
+        _def_ospace = _full_name.lower().replace(" ", "")
+        _user_info["given_names"] = _given_name.strip()
+        _user_info["family_name"] = _family_name.strip()
+    else:
+        _def_ospace += _full_name
+        _user_info["given_names"] = _full_name
+        _user_info["family_name"] = None
+
+    return _user_info, _def_ospace
+
+
+def _get_user_info_and_namespaces() -> typing.Dict[str, typing.Dict]:
+    _user_email = click.prompt("Email")
+
+    _invalid_input = True
+
+    while _invalid_input:
+        _id_type = click.prompt(
+            "User ID system (ORCID/ROR/GRID/None)", default="None"
+        )
+
+        if _id_type.upper() == "ORCID":
+            _user_orcid = click.prompt("ORCID")
+            _user_info, _def_ospace = _handle_orcid(_user_orcid)
+            _invalid_input = False
+        elif _id_type.upper() == "ROR":
+            _user_ror = click.prompt("ROR ID")
+            _user_info, _def_ospace = _handle_ror(_user_ror)
+            _invalid_input = False
+        elif _id_type.upper() == "GRID":
+            _user_grid = click.prompt("GRID ID")
+            _user_info, _def_ospace = _handle_grid(_user_grid)
+            _invalid_input = False
+        elif _id_type.upper() == "NONE":
+            _user_info, _def_ospace = _handle_uuid()
+            _user_uuid = str(uuid.uuid4())
+            _user_info["uuid"] = _user_uuid
+            _invalid_input = False
+
+    _user_info["email"] = _user_email
+
+    _def_ospace = _def_ospace.lower().replace(" ", "").strip()
+    _def_ospace = click.prompt("Default output namespace", default=_def_ospace)
+    _def_ispace = click.prompt("Default input namespace", default=_def_ospace)
+
+    _namespaces = {"input": _def_ispace, "output": _def_ospace}
+
+    return {"user": _user_info, "namespaces": _namespaces}
+
+
+def global_config_query(
+    registry: str = None, local: bool = False
+) -> typing.Dict[str, typing.Any]:
+    """Ask user question set for creating global FAIR config"""
+    logger.debug(
+        "Running global configuration query with registry at '%s'", registry
+    )
+    click.echo("Checking for local registry")
+    if not registry and "FAIR_REGISTRY_DIR" in os.environ:
+        registry = os.environ["FAIR_REGISTRY_DIR"]
+    if check_reg := check_registry_exists(registry):
+        registry = check_reg
+        click.echo(f"Local registry found at '{check_reg}'")
+    elif not registry:
+        if _ := click.confirm(
+            "Local registry not found at default location"
+            f"'{fdp_com.DEFAULT_REGISTRY_LOCATION}', "
+            "would you like to specify an existing installation?",
+            default=False,
+        ):
+            _reg_loc = click.prompt("Local registry directory")
+            _manage_script = os.path.join(_reg_loc, "manage.py")
+            while not os.path.exists(_manage_script):
+                click.echo(
+                    f"Error: Location '{_reg_loc}' is not a valid registry installation"
+                )
+                _reg_loc = click.prompt("Local registry directory")
+                _manage_script = os.path.join(_reg_loc, "manage.py")
+            registry = _reg_loc
+        else:
+            registry = fdp_com.DEFAULT_REGISTRY_LOCATION
+            click.echo(f"Installing registry to '{registry}'")
+            fdp_serv.install_registry(install_dir=registry)
+    else:
+        click.echo(f"Will install registry to '{registry}'")
+        fdp_serv.install_registry(install_dir=registry)
+
+    _local_port: int = click.prompt("Local Registry Port", default="8000")
+    _local_uri = fdp_com.DEFAULT_LOCAL_REGISTRY_URL.replace(
+        ":8000", f":{_local_port}"
+    )
+    if local:
+        _remote_url = "http://127.0.0.1:8000/api/"
+        _rem_key_file = os.path.join(registry, "token")
+        _rem_data_store = os.path.join(os.curdir, "data_store") + os.path.sep
+    else:
+        _default_rem = urljoin(fdp_com.DEFAULT_REGISTRY_DOMAIN, "api/")
+        _remote_url = click.prompt("Remote API URL", default=_default_rem)
+
+        _rem_data_store = click.prompt(
+            "Remote Data Storage Root",
+            default=_remote_url.replace("/api/", "/data/"),
+        )
+
+        _rem_key_file = click.prompt(
+            "Remote API Token File",
+        )
+        _rem_key_file = os.path.expandvars(_rem_key_file)
+
+        while (
+            not os.path.exists(_rem_key_file)
+            or not open(_rem_key_file).read().strip()
+        ):
+            click.echo(
+                f"Token file '{_rem_key_file}' does not exist or is empty, "
+                "please provide a valid token file."
+            )
+            _rem_key_file = click.prompt("Remote API Token File")
+            _rem_key_file = os.path.expandvars(_rem_key_file)
+
+    if not fdp_serv.check_server_running():
+        if _ := click.confirm(
+            "Local registry is offline, would you like to start it?",
+            default=False,
+        ):
+            fdp_serv.launch_server(registry_dir=registry)
+
+            # Keep server running by creating user run cache file
+            _cache_addr = os.path.join(fdp_com.session_cache_dir(), "user.run")
+            pathlib.Path(_cache_addr).touch()
+
+        else:
+            click.echo("Temporarily launching server to retrieve API token.")
+            fdp_serv.launch_server(registry_dir=registry)
+            fdp_serv.stop_server(registry_dir=registry, local_uri=_local_uri)
+            try:
+                fdp_req.local_token(registry_dir=registry)
+            except fdp_exc.FileNotFoundError as e:
+                raise fdp_exc.RegistryError(
+                    "Failed to retrieve local API token from registry."
+                ) from e
+
+    _loc_data_store = click.prompt(
+        "Default Data Store",
+        default=os.path.join(fdp_com.USER_FAIR_DIR, f"data{os.path.sep}"),
+    )
+    if _loc_data_store[-1] != os.path.sep:
+        _loc_data_store += os.path.sep
+
+    _glob_conf_dict = _get_user_info_and_namespaces()
+    _glob_conf_dict["registries"] = {
+        "local": {
+            "uri": _local_uri,
+            "directory": os.path.abspath(registry),
+            "data_store": _loc_data_store,
+            "token": os.path.join(os.path.abspath(registry), "token"),
+        },
+        "origin": {
+            "uri": _remote_url,
+            "token": _rem_key_file,
+            "data_store": _rem_data_store,
+        },
+    }
+
+    return _glob_conf_dict
+
+
+def local_config_query(
+    global_config: typing.Dict[str, typing.Any] = read_global_fdpconfig(),
+    first_time_setup: bool = False,
+    local: bool = False,
+) -> typing.Dict[str, typing.Any]:
+    """Ask user questions to create local user config
+
+    Parameters
+    ----------
+    global_config : Dict[str, Any], optional
+        global configuration dictionary
+    first_time_setup : bool, optional
+        if first time need to setup globals as well, by default False
+
+    Returns
+    -------
+    Dict[str, Any]
+        dictionary of local configurations
+    """
+    # Try extracting global configurations. If any keys do not exist re-run
+    # setup for creation of these, then try again.
+    try:
+        _def_remote = global_config["registries"]["origin"]["uri"]
+        _def_rem_key = global_config["registries"]["origin"]["token"]
+        _def_ospace = global_config["namespaces"]["output"]
+        _def_user = global_config["user"]
+    except KeyError:
+        click.echo(
+            "Error: Failed to read global configuration, re-running global setup."
+        )
+        first_time_setup = True
+        global_config = global_config_query()
+        _def_remote = global_config["registries"]["origin"]["uri"]
+        _def_rem_key = global_config["registries"]["origin"]["token"]
+        _def_ospace = global_config["namespaces"]["output"]
+        _def_user = global_config["user"]
+
+    # Allow the user to continue without an input namespace as some
+    # functionality does not require this.
+    if (
+        "input" not in global_config["namespaces"]
+        or not global_config["namespaces"]
+    ):
+        click.echo(f"Will use '{_def_ospace}' as default input namespace")
+        _def_ispace = _def_ospace
+    else:
+        _def_ispace = global_config["namespaces"]["input"]
+
+    # Try checking to see if the current location is a git repository and
+    # suggesting this as a default
+    try:
+        _git_repo = fdp_com.find_git_root(os.getcwd())
+    except fdp_exc.UserConfigError:
+        _git_repo = None
+
+    _git_repo = click.prompt("Local Git repository", default=_git_repo)
+    _invalid_repo = True
+
+    # Check this is indeed a git repository
+    while _invalid_repo:
+        try:
+            git.Repo(_git_repo)
+            _invalid_repo = False
+        except (git.InvalidGitRepositoryError, git.NoSuchPathError):
+            _invalid_repo = True
+            click.echo(
+                "Invalid directory, location is not the head of a local"
+                " git repository."
+            )
+            _git_repo = click.prompt("Local Git repository")
+
+    # Set the remote to use within git by label, by default 'origin'
+    # check the remote label is valid before proceeding
+    try:
+        git.Repo(_git_repo).remotes["origin"]
+        _def_rem = "origin"
+    except IndexError:
+        _def_rem = None
+
+    _git_remote = click.prompt("Git remote name", default=_def_rem)
+    _invalid_rem = True
+
+    while _invalid_rem and _def_rem:
+        try:
+            git.Repo(_git_repo).remotes[_git_remote]
+            _invalid_rem = False
+        except IndexError:
+            _invalid_rem = True
+            click.echo("Invalid remote name for git repository")
+            _git_remote = click.prompt("Git remote name", default=_def_rem)
+
+    _repo = git.Repo(_git_repo)
+
+    while _git_remote not in _repo.remotes:
+        click.echo(f"Git remote label '{_git_remote}' does not exist")
+        _git_remote = click.prompt("Git remote name")
+
+    _git_remote_repo = _repo.remotes[_git_remote].url
+
+    click.echo(
+        f"Using git repository remote '{_git_remote}': {_git_remote_repo}"
+    )
+
+    # If this is not the first setup it means globals are available so these
+    # can be suggested as defaults during local setup
+    if not first_time_setup or not local:
+        _def_remote = click.prompt("Remote API URL", default=_def_remote)
+        _def_rem_key = click.prompt(
+            "Remote API Token File", default=_def_rem_key
+        )
+        _def_rem_key = os.path.expandvars(_def_rem_key)
+
+        while (
+            not os.path.exists(_def_rem_key)
+            or not open(_def_rem_key).read().strip()
+        ):
+            click.echo(
+                f"Token file '{_def_rem_key}' does not exist or is empty, "
+                "please provide a valid token file."
+            )
+            _def_rem_key = click.prompt("Remote API Token File")
+            _def_rem_key = os.path.expandvars(_def_rem_key)
+        _def_ospace = click.prompt(
+            "Default output namespace", default=_def_ospace
+        )
+        _def_ispace = click.prompt(
+            "Default input namespace", default=_def_ispace
+        )
+
+    _local_config: typing.Dict[str, typing.Any] = {
+        "namespaces": {"output": _def_ospace, "input": _def_ispace},
+        "git": {
+            "remote": _git_remote,
+            "local_repo": _git_repo,
+            "remote_repo": _git_remote_repo,
+        },
+        "registries": copy.deepcopy(global_config["registries"]),
+    }
+
+    # Local registry is a globally defined entity
+    del _local_config["registries"]["local"]
+
+    _local_config["registries"]["origin"]["uri"] = _def_remote
+    _local_config["registries"]["origin"]["token"] = _def_rem_key
+
+    _local_config["user"] = _def_user
+
+    return _local_config
```

### Comparing `fair_cli-0.5.2/fair/configuration/validation.py` & `fair_cli-0.7.0/fair/configuration/validation.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-# sourcery skip: avoid-builtin-shadow
-"""
-CLI Config Validation
-=====================
-
-validation of the CLI configuration files both global and local variants
-
-Contents
-========
-
-Classes
--------
-
-"""
-
-__date__ = "2021-12-07"
-
-import pathlib
-import typing
-
-import pydantic
-
-
-class Git(pydantic.BaseModel):
-    local_repo: pathlib.Path = pydantic.Field(
-        ...,
-        title="local repository",
-        description="Local project git repository",
-    )
-    remote: str = pydantic.Field(
-        ...,
-        title="remote label",
-        description="label of git repository remote to use",
-    )
-    remote_repo: str = pydantic.Field(
-        ...,
-        title="URL of remote repo",
-        description="URL for the given remote repository",
-    )
-
-    class Config:
-        extra = "forbid"
-
-
-class Namespaces(pydantic.BaseModel):
-    input: str = pydantic.Field(
-        ...,
-        title="input namespace",
-        description="namespace label to use for registry inputs",
-    )
-    output: str = pydantic.Field(
-        ...,
-        title="output namespace",
-        description="namespace label to use for registry outputs",
-    )
-
-    class Config:
-        extra = "forbid"
-
-
-class Registry(pydantic.BaseModel):
-    data_store: pathlib.Path = pydantic.Field(
-        ...,
-        title="data store path",
-        description="location of data storage directory for registry",
-    )
-    token: pathlib.Path = pydantic.Field(
-        ...,
-        title="token file path",
-        description="path of file containing token for the registry",
-    )
-    uri: pydantic.AnyHttpUrl = pydantic.Field(
-        ..., title="registry URL", description="URL of the data registry"
-    )
-    directory: typing.Optional[pathlib.Path] = pydantic.Field(
-        None,
-        title="local directory",
-        description="local location of registry on system",
-    )
-
-    class Config:
-        extra = "forbid"
-
-
-class User(pydantic.BaseModel):
-    email: pydantic.EmailStr = pydantic.Field(
-        ..., title="user email", description="email address of the user"
-    )
-    family_name: str = pydantic.Field(
-        ..., title="user surname", description="family name of the user"
-    )
-    given_names: str = pydantic.Field(
-        ..., title="user forenames", description="given names of the user"
-    )
-    orcid: typing.Optional[str] = pydantic.Field(
-        None,
-        title="ORCID for the user",
-        description="The users ORCID if applicable",
-    )
-    uri: typing.Optional[str] = pydantic.Field(
-        None, title="user URI", description="Full URL identifier for the user"
-    )
-    uuid: typing.Optional[pydantic.UUID4] = pydantic.Field(
-        None, title="user UUID", description="The users UUID if applicable"
-    )
-    name: typing.Optional[str] = pydantic.Field(
-        None, title="Full Name", description="Full name for the user"
-    )
-
-    class Config:
-        extra = "forbid"
-
-
-class LocalCLIConfig(pydantic.BaseModel):
-    git: Git
-    namespaces: Namespaces
-    registries: typing.Dict[str, Registry]
-    user: User
-
-    class Config:
-        extra = "forbid"
-
-
-class GlobalCLIConfig(pydantic.BaseModel):
-    namespaces: Namespaces
-    registries: typing.Dict[str, Registry]
-    user: User
-
-    class Config:
-        extra = "forbid"
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+# sourcery skip: avoid-builtin-shadow
+"""
+CLI Config Validation
+=====================
+
+validation of the CLI configuration files both global and local variants
+
+Contents
+========
+
+Classes
+-------
+
+"""
+
+__date__ = "2021-12-07"
+
+import pathlib
+import typing
+
+import pydantic
+
+
+class Git(pydantic.BaseModel):
+    local_repo: pathlib.Path = pydantic.Field(
+        ...,
+        title="local repository",
+        description="Local project git repository",
+    )
+    remote: str = pydantic.Field(
+        ...,
+        title="remote label",
+        description="label of git repository remote to use",
+    )
+    remote_repo: str = pydantic.Field(
+        ...,
+        title="URL of remote repo",
+        description="URL for the given remote repository",
+    )
+
+    class Config:
+        extra = "forbid"
+
+
+class Namespaces(pydantic.BaseModel):
+    input: str = pydantic.Field(
+        ...,
+        title="input namespace",
+        description="namespace label to use for registry inputs",
+    )
+    output: str = pydantic.Field(
+        ...,
+        title="output namespace",
+        description="namespace label to use for registry outputs",
+    )
+
+    class Config:
+        extra = "forbid"
+
+
+class Registry(pydantic.BaseModel):
+    data_store: pathlib.Path = pydantic.Field(
+        ...,
+        title="data store path",
+        description="location of data storage directory for registry",
+    )
+    token: pathlib.Path = pydantic.Field(
+        ...,
+        title="token file path",
+        description="path of file containing token for the registry",
+    )
+    uri: pydantic.AnyHttpUrl = pydantic.Field(
+        ..., title="registry URL", description="URL of the data registry"
+    )
+    directory: typing.Optional[pathlib.Path] = pydantic.Field(
+        None,
+        title="local directory",
+        description="local location of registry on system",
+    )
+
+    class Config:
+        extra = "forbid"
+
+
+class User(pydantic.BaseModel):
+    email: pydantic.EmailStr = pydantic.Field(
+        ..., title="user email", description="email address of the user"
+    )
+    family_name: str = pydantic.Field(
+        ..., title="user surname", description="family name of the user"
+    )
+    given_names: str = pydantic.Field(
+        ..., title="user forenames", description="given names of the user"
+    )
+    orcid: typing.Optional[str] = pydantic.Field(
+        None,
+        title="ORCID for the user",
+        description="The users ORCID if applicable",
+    )
+    uri: typing.Optional[str] = pydantic.Field(
+        None, title="user URI", description="Full URL identifier for the user"
+    )
+    uuid: typing.Optional[pydantic.UUID4] = pydantic.Field(
+        None, title="user UUID", description="The users UUID if applicable"
+    )
+    name: typing.Optional[str] = pydantic.Field(
+        None, title="Full Name", description="Full name for the user"
+    )
+
+    class Config:
+        extra = "forbid"
+
+
+class LocalCLIConfig(pydantic.BaseModel):
+    git: Git
+    namespaces: Namespaces
+    registries: typing.Dict[str, Registry]
+    user: User
+
+    class Config:
+        extra = "forbid"
+
+
+class GlobalCLIConfig(pydantic.BaseModel):
+    namespaces: Namespaces
+    registries: typing.Dict[str, Registry]
+    user: User
+
+    class Config:
+        extra = "forbid"
```

### Comparing `fair_cli-0.5.2/fair/exceptions.py` & `fair_cli-0.7.0/fair/exceptions.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,197 +1,197 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-"""
-FAIR-CLI Exceptions
-===================
-
-Custom exceptions for the command line interface. These are captured during
-command line usage, but provide a means examining scenarios during testing.
-
-
-Contents
-========
-
-Exceptions
-----------
-
-    FAIRCLIException
-    RegistryErrorException
-    CLIConfigurationError
-    KeyPathError
-    UnexpectedRegistryServerState
-    FDPRepositoryError
-    FileNotFoundError
-    InternalError
-    StagingError
-    ValidationError
-"""
-
-__date__ = "2021-06-28"
-
-import json
-import typing
-
-import click
-
-
-class FAIRCLIException(Exception):
-    """Base exception class for all FAIR-CLI exceptions"""
-
-    def __init__(
-        self,
-        msg: str,
-        hint: str = "",
-        level: str = "Error",
-        exit_code: int = 1,
-    ):
-        """Initialises a FAIR-CLI exception type.
-
-        A level can be specified which is a prefix whenever the exception is
-        captured and printed (when used within the CLI itself)
-
-        Parameters
-        ----------
-        msg : str
-            message to display
-        hint : str
-            possible solution to issue raised
-        level : str, optional
-            level descriptor (message prefix), by default "Error"
-        """
-        self.msg = msg
-        self.level = level
-        self.hint = hint
-        self.exit_code = exit_code
-        super().__init__(msg)
-
-    def err_print(self) -> None:
-        _out_msg = f"{f'{self.level}: ' if self.level else ''}{self.msg}"
-        if self.hint:
-            _out_msg += f"\n{self.hint}"
-        click.echo(_out_msg)
-
-
-class RegistryError(FAIRCLIException):
-    """Errors relating to registry setup and usage"""
-
-    def __init__(self, msg: str, hint: str = ""):
-        super().__init__(msg, hint=hint)
-
-
-class CLIConfigurationError(FAIRCLIException):
-    """Errors relating to CLI configuration"""
-
-    def __init__(self, msg, hint="", level="Error"):
-        super().__init__(msg, hint=hint, level=level)
-
-
-class KeyPathError(FAIRCLIException):
-    """Errors relating to key path within a nested mapping"""
-
-    def __init__(self, key, parent_label):
-        _msg = f"Failed to retrieve item at address '{key}' from mapping '{parent_label}', no such address"
-        super().__init__(_msg, level="Error")
-
-
-class UserConfigError(FAIRCLIException):
-    """Errors relating to the user 'config.yaml' file"""
-
-    def __init__(self, msg, hint=""):
-        super().__init__(msg, hint=hint)
-
-
-class UnexpectedRegistryServerState(FAIRCLIException):
-    """Errors relating to server start/stop when already up/down)"""
-
-    def __init__(self, msg, hint=""):
-        super().__init__(msg, hint)
-
-
-class FDPRepositoryError(FAIRCLIException):
-    """Errors relating to FAIR repository"""
-
-    def __init__(self, msg, hint=""):
-        super().__init__(msg, hint=hint)
-
-
-class FileNotFoundError(FAIRCLIException):
-    """Attempt to access a non-existent file"""
-
-    def __init__(self, msg, hint=""):
-        super().__init__(msg, hint=hint)
-
-
-class InternalError(FAIRCLIException):
-    """Errors relating to non-user created issues"""
-
-    def __init__(self, msg):
-        super().__init__(msg, level="InternalError")
-
-
-class CommandExecutionError(FAIRCLIException):
-    """Errors related to execution of submission script commands"""
-
-    def __init__(self, msg, exit_code):
-        super().__init__(msg, exit_code=exit_code)
-
-
-class RegistryAPICallError(FAIRCLIException):
-    """Errors relating to invalid queries to the registry RestAPI"""
-
-    def __init__(self, msg, error_code):
-        self.error_code = error_code
-        _level = "Warning" if self.error_code in [403] else "Error"
-        super().__init__(
-            f"[HTTP {self.error_code}]: {msg}",
-            exit_code=error_code,
-            level=_level,
-        )
-
-
-class ValidationError(FAIRCLIException):
-    """Errors relating to the Pydantic based User Config validation"""
-
-    def __init__(self, info: typing.List[typing.Dict]) -> None:
-        _invalid_data: typing.List[typing.Dict] = []
-
-        for data in json.loads(info):
-            _location = map(str, data["loc"])
-            _location = ":".join(_location)
-            _type = str(data["type"])
-            _msg = str(data["msg"])
-            _invalid_data.append(f"{_location:<50}  {_type:<20}  {_msg:<20}")
-
-        _msg = "User 'config.yaml' file validation failed with:\n"
-        _msg += "\n" + f'{"Location":<50}  {"Type":<20}  {"Message":<20}\n'
-        _msg += "=" * 94 + "\n"
-        _msg += "\n".join(_invalid_data)
-        super().__init__(_msg)
-
-
-class NotImplementedError(FAIRCLIException):
-    """Errors relating to features that have not yet been implemented"""
-
-    def __init__(self, msg, hint="", level="Error"):
-        super().__init__(msg, hint, level=level)
-
-
-class StagingError(FAIRCLIException):
-    """Errors relating to the staging of jobs"""
-
-    def __init__(self, msg):
-        super().__init__(msg)
-
-
-class SynchronisationError(FAIRCLIException):
-    """Errors relating to synchronisation between registries"""
-
-    def __init__(self, msg, error_code):
-        self.error_code = error_code
-        super().__init__(msg, exit_code=error_code)
-
-
-class ImplementationError(FAIRCLIException):
-    """Errors relating to setup via API implementation"""
-
-    def __init__(self, msg):
-        super().__init__(msg)
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+"""
+FAIR-CLI Exceptions
+===================
+
+Custom exceptions for the command line interface. These are captured during
+command line usage, but provide a means examining scenarios during testing.
+
+
+Contents
+========
+
+Exceptions
+----------
+
+    FAIRCLIException
+    RegistryErrorException
+    CLIConfigurationError
+    KeyPathError
+    UnexpectedRegistryServerState
+    FDPRepositoryError
+    FileNotFoundError
+    InternalError
+    StagingError
+    ValidationError
+"""
+
+__date__ = "2021-06-28"
+
+import json
+import typing
+
+import click
+
+
+class FAIRCLIException(Exception):
+    """Base exception class for all FAIR-CLI exceptions"""
+
+    def __init__(
+        self,
+        msg: str,
+        hint: str = "",
+        level: str = "Error",
+        exit_code: int = 1,
+    ):
+        """Initialises a FAIR-CLI exception type.
+
+        A level can be specified which is a prefix whenever the exception is
+        captured and printed (when used within the CLI itself)
+
+        Parameters
+        ----------
+        msg : str
+            message to display
+        hint : str
+            possible solution to issue raised
+        level : str, optional
+            level descriptor (message prefix), by default "Error"
+        """
+        self.msg = msg
+        self.level = level
+        self.hint = hint
+        self.exit_code = exit_code
+        super().__init__(msg)
+
+    def err_print(self) -> None:
+        _out_msg = f"{f'{self.level}: ' if self.level else ''}{self.msg}"
+        if self.hint:
+            _out_msg += f"\n{self.hint}"
+        click.echo(_out_msg)
+
+
+class RegistryError(FAIRCLIException):
+    """Errors relating to registry setup and usage"""
+
+    def __init__(self, msg: str, hint: str = ""):
+        super().__init__(msg, hint=hint)
+
+
+class CLIConfigurationError(FAIRCLIException):
+    """Errors relating to CLI configuration"""
+
+    def __init__(self, msg, hint="", level="Error"):
+        super().__init__(msg, hint=hint, level=level)
+
+
+class KeyPathError(FAIRCLIException):
+    """Errors relating to key path within a nested mapping"""
+
+    def __init__(self, key, parent_label):
+        _msg = f"Failed to retrieve item at address '{key}' from mapping '{parent_label}', no such address"
+        super().__init__(_msg, level="Error")
+
+
+class UserConfigError(FAIRCLIException):
+    """Errors relating to the user 'config.yaml' file"""
+
+    def __init__(self, msg, hint=""):
+        super().__init__(msg, hint=hint)
+
+
+class UnexpectedRegistryServerState(FAIRCLIException):
+    """Errors relating to server start/stop when already up/down)"""
+
+    def __init__(self, msg, hint=""):
+        super().__init__(msg, hint)
+
+
+class FDPRepositoryError(FAIRCLIException):
+    """Errors relating to FAIR repository"""
+
+    def __init__(self, msg, hint=""):
+        super().__init__(msg, hint=hint)
+
+
+class FileNotFoundError(FAIRCLIException):
+    """Attempt to access a non-existent file"""
+
+    def __init__(self, msg, hint=""):
+        super().__init__(msg, hint=hint)
+
+
+class InternalError(FAIRCLIException):
+    """Errors relating to non-user created issues"""
+
+    def __init__(self, msg):
+        super().__init__(msg, level="InternalError")
+
+
+class CommandExecutionError(FAIRCLIException):
+    """Errors related to execution of submission script commands"""
+
+    def __init__(self, msg, exit_code):
+        super().__init__(msg, exit_code=exit_code)
+
+
+class RegistryAPICallError(FAIRCLIException):
+    """Errors relating to invalid queries to the registry RestAPI"""
+
+    def __init__(self, msg, error_code):
+        self.error_code = error_code
+        _level = "Warning" if self.error_code in [403] else "Error"
+        super().__init__(
+            f"[HTTP {self.error_code}]: {msg}",
+            exit_code=error_code,
+            level=_level,
+        )
+
+
+class ValidationError(FAIRCLIException):
+    """Errors relating to the Pydantic based User Config validation"""
+
+    def __init__(self, info: typing.List[typing.Dict]) -> None:
+        _invalid_data: typing.List[typing.Dict] = []
+
+        for data in json.loads(info):
+            _location = map(str, data["loc"])
+            _location = ":".join(_location)
+            _type = str(data["type"])
+            _msg = str(data["msg"])
+            _invalid_data.append(f"{_location:<50}  {_type:<20}  {_msg:<20}")
+
+        _msg = "User 'config.yaml' file validation failed with:\n"
+        _msg += "\n" + f'{"Location":<50}  {"Type":<20}  {"Message":<20}\n'
+        _msg += "=" * 94 + "\n"
+        _msg += "\n".join(_invalid_data)
+        super().__init__(_msg)
+
+
+class NotImplementedError(FAIRCLIException):
+    """Errors relating to features that have not yet been implemented"""
+
+    def __init__(self, msg, hint="", level="Error"):
+        super().__init__(msg, hint, level=level)
+
+
+class StagingError(FAIRCLIException):
+    """Errors relating to the staging of jobs"""
+
+    def __init__(self, msg):
+        super().__init__(msg)
+
+
+class SynchronisationError(FAIRCLIException):
+    """Errors relating to synchronisation between registries"""
+
+    def __init__(self, msg, error_code):
+        self.error_code = error_code
+        super().__init__(msg, exit_code=error_code)
+
+
+class ImplementationError(FAIRCLIException):
+    """Errors relating to setup via API implementation"""
+
+    def __init__(self, msg):
+        super().__init__(msg)
```

### Comparing `fair_cli-0.5.2/fair/files.txt` & `fair_cli-0.7.0/fair/files.txt`

 * *Files identical despite different names*

### Comparing `fair_cli-0.5.2/fair/history.py` & `fair_cli-0.7.0/fair/history.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-"""
-
-Run History
-===========
-
-Methods relating to the summary of jobs commenced within the given FAIR-CLI
-repository. Allowing user to view any stdout from these.
-
-Contents
-========
-
-Functions
----------
-
-    history_directory - returns the current repository logs directory
-"""
-import glob
-import os
-
-import click
-import rich
-
-import fair.common as fdp_com
-import fair.exceptions as fdp_exc
-import fair.run as fdp_run
-import fair.templates as fdp_tpl
-
-
-def history_directory(repo_loc: str) -> str:
-    """Retrieve the directory containing job logs for the specified repository
-
-    Parameters
-    ----------
-    repo_loc : str
-        FAIR-CLI repository path
-
-    Returns
-    -------
-    str
-        location of the job logs directory
-    """
-    return os.path.join(
-        fdp_com.find_fair_root(repo_loc), fdp_com.FAIR_FOLDER, "logs"
-    )
-
-
-def show_job_log(repo_loc: str, job_id: str) -> str:
-    """Show the log from a given job
-
-    Parameters
-    ----------
-    repo_loc : str
-        FAIR-CLI repository path
-    job_id : str
-        SHA identifier for the job
-
-    Returns
-    -------
-    str
-        log file location for the given job
-    """
-    _sorted_time_dirs = sorted(
-        glob.glob(os.path.join(fdp_com.default_jobs_dir(), "*")), reverse=True
-    )
-
-    _log_files = [
-        os.path.join(
-            history_directory(repo_loc), f"job_{os.path.basename(i)}.log"
-        )
-        for i in _sorted_time_dirs
-    ]
-
-    for job_dir, _log_file in zip(_sorted_time_dirs, _log_files):
-        # Use the timestamp directory name for the hash
-        _job_id = fdp_run.get_job_hash(job_dir)
-
-        if _job_id[: len(job_id)] == job_id:
-            with open(_log_file) as f:
-                click.echo(f.read())
-            _jobs_list = os.path.join(job_dir, "coderuns.txt")
-
-            # Check if a code runs file exists for the given job and also
-            # print the list of code_run uuids created in the registry
-            if os.path.exists(_jobs_list):
-                click.echo("Related Code Runs: ")
-                click.echo(
-                    "\t- " + "\n\t- ".join(open(_jobs_list).readlines())
-                )
-
-            return _log_file
-
-    raise fdp_exc.FileNotFoundError(
-        f"Could not find job matching id '{job_id}'"
-    )
-
-
-def show_history(repo_loc: str, length: int = 10) -> None:
-    """Show job history by time sorting log outputs, display metadata
-
-    Parameters
-    ----------
-    repo_loc : str
-        FAIR-CLI repository path
-    length : int, optional
-        max number of entries to display, by default 10
-    """
-
-    _sorted_time_dirs = sorted(
-        glob.glob(os.path.join(fdp_com.default_jobs_dir(), "*")), reverse=True
-    )
-
-    _log_files = [
-        os.path.join(
-            history_directory(repo_loc), f"job_{os.path.basename(i)}.log"
-        )
-        for i in _sorted_time_dirs
-    ]
-
-    # Iterate through the logs printing out the job author
-    for i, (job_dir, _log_file) in enumerate(
-        zip(_sorted_time_dirs, _log_files)
-    ):
-        _job_id = fdp_run.get_job_hash(job_dir)
-        if not os.path.exists(_log_file):
-            raise fdp_exc.FileNotFoundError(
-                f"Cannot open log for job '{_job_id}'"
-            )
-        with open(_log_file) as f:
-            _log_lines = f.readlines()
-            _metadata = []
-            for line in _log_lines:
-                if "------- time taken " in line:
-                    break
-                if " = " in line:
-                    _metadata.append(line)
-        if not _metadata:
-            continue
-        _metadata = [i for i in _metadata if i.strip()]
-        _user_lines = [i for i in _metadata if "Author" in i]
-        if not _user_lines:
-            raise fdp_exc.InternalError(
-                "Failed to retrieve author information from log "
-                f"for job '{_job_id}'"
-            )
-        _date_lines = [i for i in _metadata if "Commenced" in i]
-        if not _date_lines:
-            raise fdp_exc.InternalError(
-                "Failed to retrieve date information from log "
-                f"for job '{_job_id}'"
-            )
-        _date = _date_lines[0].split("=")[1].strip()
-        _user = _user_lines[0].split("=")[1].strip()
-        _name = _user.split("<")[0].strip()
-        _email = _user.replace(_name, "").strip()
-        _meta = {
-            "sha": _job_id,
-            "user": _name,
-            "user_email": _email,
-            "datetime": _date,
-        }
-        rich.print(fdp_tpl.hist_template.render(**_meta))
-
-        if i == length:
-            return
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+"""
+
+Run History
+===========
+
+Methods relating to the summary of jobs commenced within the given FAIR-CLI
+repository. Allowing user to view any stdout from these.
+
+Contents
+========
+
+Functions
+---------
+
+    history_directory - returns the current repository logs directory
+"""
+import glob
+import os
+
+import click
+import rich
+
+import fair.common as fdp_com
+import fair.exceptions as fdp_exc
+import fair.run as fdp_run
+import fair.templates as fdp_tpl
+
+
+def history_directory(repo_loc: str) -> str:
+    """Retrieve the directory containing job logs for the specified repository
+
+    Parameters
+    ----------
+    repo_loc : str
+        FAIR-CLI repository path
+
+    Returns
+    -------
+    str
+        location of the job logs directory
+    """
+    return os.path.join(
+        fdp_com.find_fair_root(repo_loc), fdp_com.FAIR_FOLDER, "logs"
+    )
+
+
+def show_job_log(repo_loc: str, job_id: str) -> str:
+    """Show the log from a given job
+
+    Parameters
+    ----------
+    repo_loc : str
+        FAIR-CLI repository path
+    job_id : str
+        SHA identifier for the job
+
+    Returns
+    -------
+    str
+        log file location for the given job
+    """
+    _sorted_time_dirs = sorted(
+        glob.glob(os.path.join(fdp_com.default_jobs_dir(), "*")), reverse=True
+    )
+
+    _log_files = [
+        os.path.join(
+            history_directory(repo_loc), f"job_{os.path.basename(i)}.log"
+        )
+        for i in _sorted_time_dirs
+    ]
+
+    for job_dir, _log_file in zip(_sorted_time_dirs, _log_files):
+        # Use the timestamp directory name for the hash
+        _job_id = fdp_run.get_job_hash(job_dir)
+
+        if _job_id[: len(job_id)] == job_id:
+            with open(_log_file) as f:
+                click.echo(f.read())
+            _jobs_list = os.path.join(job_dir, "coderuns.txt")
+
+            # Check if a code runs file exists for the given job and also
+            # print the list of code_run uuids created in the registry
+            if os.path.exists(_jobs_list):
+                click.echo("Related Code Runs: ")
+                click.echo(
+                    "\t- " + "\n\t- ".join(open(_jobs_list).readlines())
+                )
+
+            return _log_file
+
+    raise fdp_exc.FileNotFoundError(
+        f"Could not find job matching id '{job_id}'"
+    )
+
+
+def show_history(repo_loc: str, length: int = 10) -> None:
+    """Show job history by time sorting log outputs, display metadata
+
+    Parameters
+    ----------
+    repo_loc : str
+        FAIR-CLI repository path
+    length : int, optional
+        max number of entries to display, by default 10
+    """
+
+    _sorted_time_dirs = sorted(
+        glob.glob(os.path.join(fdp_com.default_jobs_dir(), "*")), reverse=True
+    )
+
+    _log_files = [
+        os.path.join(
+            history_directory(repo_loc), f"job_{os.path.basename(i)}.log"
+        )
+        for i in _sorted_time_dirs
+    ]
+
+    # Iterate through the logs printing out the job author
+    for i, (job_dir, _log_file) in enumerate(
+        zip(_sorted_time_dirs, _log_files)
+    ):
+        _job_id = fdp_run.get_job_hash(job_dir)
+        if not os.path.exists(_log_file):
+            raise fdp_exc.FileNotFoundError(
+                f"Cannot open log for job '{_job_id}'"
+            )
+        with open(_log_file) as f:
+            _log_lines = f.readlines()
+            _metadata = []
+            for line in _log_lines:
+                if "------- time taken " in line:
+                    break
+                if " = " in line:
+                    _metadata.append(line)
+        if not _metadata:
+            continue
+        _metadata = [i for i in _metadata if i.strip()]
+        _user_lines = [i for i in _metadata if "Author" in i]
+        if not _user_lines:
+            raise fdp_exc.InternalError(
+                "Failed to retrieve author information from log "
+                f"for job '{_job_id}'"
+            )
+        _date_lines = [i for i in _metadata if "Commenced" in i]
+        if not _date_lines:
+            raise fdp_exc.InternalError(
+                "Failed to retrieve date information from log "
+                f"for job '{_job_id}'"
+            )
+        _date = _date_lines[0].split("=")[1].strip()
+        _user = _user_lines[0].split("=")[1].strip()
+        _name = _user.split("<")[0].strip()
+        _email = _user.replace(_name, "").strip()
+        _meta = {
+            "sha": _job_id,
+            "user": _name,
+            "user_email": _email,
+            "datetime": _date,
+        }
+        rich.print(fdp_tpl.hist_template.render(**_meta))
+
+        if i == length:
+            return
```

### Comparing `fair_cli-0.5.2/fair/register.py` & `fair_cli-0.7.0/fair/register.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,263 +1,265 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-"""
-
-Register Key Methods
-====================
-
-Substitute/fetch data relating to 'register' entries in the
-`config.yaml` user config
-
-
-Contents
-========
-
-Functions
--------
-
-"""
-
-__date__ = "2021-08-16"
-
-import copy
-import logging
-import os
-import platform
-import shutil
-import typing
-import urllib.parse
-
-import fair.exceptions as fdp_exc
-import fair.registry.requests as fdp_req
-import fair.registry.storage as fdp_store
-import fair.registry.sync as fdp_sync
-import fair.registry.versioning as fdp_ver
-from fair.registry import SEARCH_KEYS
-
-logger = logging.getLogger("FAIRDataPipeline.Register")
-
-
-def convert_key_value_to_id(
-    uri: str, obj_type: str, value: str, token: str
-) -> int:
-    """Converts a config key value to the relevant URL on the local registry
-
-    Parameters
-    ----------
-    uri: str
-        registry endpoint to use for obtaining URL
-    obj_type : str
-        object type
-    value : str
-        search term to use
-    token: str
-        registry access token
-
-    Returns
-    -------
-    int
-        ID on the local registry matching the entry
-    """
-    _params = {SEARCH_KEYS[obj_type]: value}
-    _result = fdp_req.get(uri, obj_type, token, params=_params)
-    if not _result:
-        raise fdp_exc.RegistryError(
-            f"Failed to obtain result for '{obj_type}' with parameters '{_params}'"
-        )
-    return fdp_req.get_obj_id_from_url(_result[0]["url"])
-
-
-# flake8: noqa: C901
-def fetch_registrations(
-    local_uri: str,
-    repo_dir: str,
-    write_data_store: str,
-    user_config_register: typing.Dict,
-) -> typing.Dict:
-    """As part of running 'pull' fetch all items listed under 'register'
-
-    Parameters
-    ----------
-    repo_dir : str
-        FAIR project repository
-    cfg : typing.Dict
-        Dict containing working config
-
-    Returns
-    -------
-    typing.List[str]
-        list of registered object URLs
-    """
-    _expected_keys = [
-        "root",
-        "path",
-        "file_type",
-        "primary",
-        "version",
-        "public",
-    ]
-
-    _stored_objects: typing.List[str] = []
-
-    for entry in user_config_register:
-        for key in _expected_keys:
-            if key not in entry and key not in entry["use"]:
-                raise fdp_exc.UserConfigError(
-                    f"Expected key '{key}' in 'register' item"
-                )
-
-        _identifier: str = entry["identifier"] if "identifier" in entry else ""
-        _unique_name: str = (
-            entry["unique_name"] if "unique_name" in entry else ""
-        )
-
-        _data_product = None
-        _external_object = None
-        _is_present = None
-
-        _search_data = {}
-
-        if "data_product" in entry:
-            _data_product: str = entry["use"]["data_product"]
-        elif "external_object" in entry:
-            _external_object: str = entry["use"]["data_product"]
-
-        if not _external_object and not _data_product:
-            raise fdp_exc.UserConfigError(
-                "Expected either 'data_product' or 'external_object' in 'register' item"
-            )
-
-        elif _external_object and _data_product:
-            raise fdp_exc.UserConfigError(
-                "Only one type may be provided (data_product/external_object)"
-            )
-        elif _external_object:
-            _name = entry["use"]["data_product"]
-            _obj_type = "external_object"
-            # TODO: This doesn't work because of a mismatch with spaces in alternate_identifier, perhaps?
-            if "unique_name" in entry and "alternate_identifier_type" in entry:
-                #                _search_data['alternate_identifier'] = entry['unique_name']
-                _search_data["alternate_identifier_type"] = entry[
-                    "alternate_identifier_type"
-                ]
-            elif "identifier" in entry:
-                _search_data["identifier"] = entry["identifier"]
-            else:
-                raise fdp_exc.UserConfigError(
-                    "Expected either 'identifier', or 'unique_name' and "
-                    f"'alternate_identifier_type' in external object '{_name}'"
-                )
-            try:
-                _data_product_id = convert_key_value_to_id(
-                    local_uri,
-                    "data_product",
-                    entry["use"]["data_product"],
-                    fdp_req.local_token(),
-                )
-                _search_data["data_product"] = _data_product_id
-            except fdp_exc.RegistryError:
-                _is_present = "absent"
-
-        else:
-            _name = entry["use"]["data_product"]
-            _obj_type = "data_product"
-            _search_data = {"name": _name}
-
-        _search_data["version"] = entry["use"]["version"]
-        _namespace = entry["use"]["namespace"]
-
-        if not _identifier and not _unique_name:
-            raise fdp_exc.UserConfigError(
-                "Expected either 'unique_name' or 'identifier' in 'register' item"
-            )
-
-        elif _identifier and _unique_name:
-            raise fdp_exc.UserConfigError(
-                "Only one unique identifier may be provided (doi/unique_name)"
-            )
-
-        if "cache" in entry:
-            _temp_data_file = entry["cache"]
-        else:
-            _local_parsed = urllib.parse.urlparse(local_uri)
-            _local_url = f"{_local_parsed.scheme}://{_local_parsed.netloc}"
-            _temp_data_file = fdp_sync.download_from_registry(
-                _local_url, root=entry["root"], path=entry["path"]
-            )
-
-        # Need to fix the path for Windows
-        if platform.system() == "Windows":
-            _name = _name.replace("/", os.path.sep)
-
-        _local_dir = os.path.join(write_data_store, _namespace, _name)
-
-        # Check if the object is already present on the local registry
-        _is_present = fdp_store.check_if_object_exists(
-            local_uri=local_uri,
-            file_loc=_temp_data_file,
-            token=fdp_req.local_token(),
-            obj_type=_obj_type,
-            search_data=_search_data,
-        )
-
-        # Hash matched version already present
-        if _is_present == "hash_match":
-            logger.debug(
-                "Skipping item '%s' as a hash matched entry is already"
-                " present with this name, deleting temporary data file",
-                _name,
-            )
-            os.remove(_temp_data_file)
-            continue
-
-        # Item found but not hash matched retrieve a version number
-        elif _is_present != "absent":
-            _results = _is_present
-            _user_version = fdp_ver.get_correct_version(
-                results_list=_results,
-                free_write=True,
-                version=entry["use"]["version"],
-            )
-            logger.debug("Found existing results for %s", _results)
-        else:
-            _user_version = fdp_ver.get_correct_version(
-                results_list=None,
-                free_write=True,
-                version=entry["use"]["version"],
-            )
-            logger.debug("No existing results found for %s", _search_data)
-
-        # Create object location directory, ignoring if already present
-        # as multiple version files can exist
-        os.makedirs(_local_dir, exist_ok=True)
-
-        _local_file = os.path.join(
-            _local_dir, f"{_user_version}.{entry['file_type']}"
-        )
-        # Copy the temporary file into the data store
-        # then remove temporary file to save space
-        logger.debug("Saving data file to '%s'", _local_file)
-        shutil.copy(_temp_data_file, _local_file)
-
-        os.remove(_temp_data_file)
-
-        if "public" in entry:
-            _public = entry["public"]
-
-        data = copy.deepcopy(entry)
-
-        data["namespace_name"] = entry["use"]["namespace"]
-
-        _file_url = fdp_store.store_data_file(
-            uri=local_uri,
-            repo_dir=repo_dir,
-            token=fdp_req.local_token(),
-            data=data,
-            local_file=_local_file,
-            write_data_store=write_data_store,
-            public=_public,
-        )
-
-        _stored_objects.append(_file_url)
-
-    return _stored_objects
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+"""
+
+Register Key Methods
+====================
+
+Substitute/fetch data relating to 'register' entries in the
+`config.yaml` user config
+
+
+Contents
+========
+
+Functions
+-------
+
+"""
+
+__date__ = "2021-08-16"
+
+import copy
+import logging
+import os
+import platform
+import shutil
+import typing
+import urllib.parse
+
+import fair.exceptions as fdp_exc
+import fair.registry.requests as fdp_req
+import fair.registry.storage as fdp_store
+import fair.registry.sync as fdp_sync
+import fair.registry.versioning as fdp_ver
+from fair.registry import SEARCH_KEYS
+
+logger = logging.getLogger("FAIRDataPipeline.Register")
+
+
+def convert_key_value_to_id(
+    uri: str, obj_type: str, value: str, token: str
+) -> int:
+    """Converts a config key value to the relevant URL on the local registry
+
+    Parameters
+    ----------
+    uri: str
+        registry endpoint to use for obtaining URL
+    obj_type : str
+        object type
+    value : str
+        search term to use
+    token: str
+        registry access token
+
+    Returns
+    -------
+    int
+        ID on the local registry matching the entry
+    """
+    _params = {SEARCH_KEYS[obj_type]: value}
+    _result = fdp_req.get(uri, obj_type, token, params=_params)
+    if not _result:
+        raise fdp_exc.RegistryError(
+            f"Failed to obtain result for '{obj_type}' with parameters '{_params}'"
+        )
+    return fdp_req.get_obj_id_from_url(_result[0]["url"])
+
+
+# flake8: noqa: C901
+def fetch_registrations(
+    local_uri: str,
+    repo_dir: str,
+    write_data_store: str,
+    user_config_register: typing.Dict,
+) -> typing.Dict:
+    """As part of running 'pull' fetch all items listed under 'register'
+
+    Parameters
+    ----------
+    repo_dir : str
+        FAIR project repository
+    cfg : typing.Dict
+        Dict containing working config
+
+    Returns
+    -------
+    typing.List[str]
+        list of registered object URLs
+    """
+    _expected_keys = [
+        "root",
+        "path",
+        "file_type",
+        "primary",
+        "version",
+        "public",
+    ]
+
+    _stored_objects: typing.List[str] = []
+
+    for entry in user_config_register:
+        for key in _expected_keys:
+            if key not in entry and key not in entry["use"]:
+                raise fdp_exc.UserConfigError(
+                    f"Expected key '{key}' in 'register' item"
+                )
+
+        _identifier: str = entry["identifier"] if "identifier" in entry else ""
+        _unique_name: str = (
+            entry["unique_name"] if "unique_name" in entry else ""
+        )
+
+        _data_product = None
+        _external_object = None
+        _is_present = None
+
+        _search_data = {}
+
+        if "data_product" in entry:
+            _data_product: str = entry["use"]["data_product"]
+        elif "external_object" in entry:
+            _external_object: str = entry["use"]["data_product"]
+
+        if not _external_object and not _data_product:
+            raise fdp_exc.UserConfigError(
+                "Expected either 'data_product' or 'external_object' in 'register' item"
+            )
+
+        elif _external_object and _data_product:
+            raise fdp_exc.UserConfigError(
+                "Only one type may be provided (data_product/external_object)"
+            )
+        elif _external_object:
+            _name = entry["use"]["data_product"]
+            _obj_type = "external_object"
+            # TODO: This doesn't work because of a mismatch with spaces in alternate_identifier, perhaps?
+            if "unique_name" in entry and "alternate_identifier_type" in entry:
+                #                _search_data['alternate_identifier'] = entry['unique_name']
+                _search_data["alternate_identifier_type"] = entry[
+                    "alternate_identifier_type"
+                ]
+            elif "identifier" in entry:
+                _search_data["identifier"] = entry["identifier"]
+            else:
+                raise fdp_exc.UserConfigError(
+                    "Expected either 'identifier', or 'unique_name' and "
+                    f"'alternate_identifier_type' in external object '{_name}'"
+                )
+            try:
+                _data_product_id = convert_key_value_to_id(
+                    local_uri,
+                    "data_product",
+                    entry["use"]["data_product"],
+                    fdp_req.local_token(),
+                )
+                _search_data["data_product"] = _data_product_id
+            except fdp_exc.RegistryError:
+                _is_present = "absent"
+
+        else:
+            _name = entry["use"]["data_product"]
+            _obj_type = "data_product"
+            _search_data = {"name": _name}
+
+        _search_data["version"] = entry["use"]["version"]
+        _namespace = entry["use"]["namespace"]
+
+        if not _identifier and not _unique_name:
+            raise fdp_exc.UserConfigError(
+                "Expected either 'unique_name' or 'identifier' in 'register' item"
+            )
+
+        elif _identifier and _unique_name:
+            raise fdp_exc.UserConfigError(
+                "Only one unique identifier may be provided (doi/unique_name)"
+            )
+
+        if "cache" in entry:
+            _temp_data_file = entry["cache"]
+        else:
+            _local_parsed = urllib.parse.urlparse(local_uri)
+            _local_url = f"{_local_parsed.scheme}://{_local_parsed.netloc}"
+            _temp_data_file = fdp_sync.download_from_registry(
+                _local_url, root=entry["root"], path=entry["path"]
+            )
+
+        # Need to fix the path for Windows
+        if platform.system() == "Windows":
+            _name = _name.replace("/", os.path.sep)
+
+        _local_dir = os.path.join(write_data_store, _namespace, _name)
+
+        # Check if the object is already present on the local registry
+        _is_present = fdp_store.check_if_object_exists(
+            local_uri=local_uri,
+            file_loc=_temp_data_file,
+            token=fdp_req.local_token(),
+            obj_type=_obj_type,
+            search_data=_search_data,
+        )
+
+        # Hash matched version already present
+        if _is_present == "hash_match":
+            logger.debug(
+                "Skipping item '%s' as a hash matched entry is already"
+                " present with this name, deleting temporary data file",
+                _name,
+            )
+            os.remove(_temp_data_file)
+            continue
+
+        # Item found but not hash matched retrieve a version number
+        elif _is_present != "absent":
+            _results = _is_present
+            _user_version = fdp_ver.get_correct_version(
+                results_list=_results,
+                free_write=True,
+                version=entry["use"]["version"],
+            )
+            logger.debug("Found existing results for %s", _results)
+        else:
+            _user_version = fdp_ver.get_correct_version(
+                results_list=None,
+                free_write=True,
+                version=entry["use"]["version"],
+            )
+            logger.debug("No existing results found for %s", _search_data)
+
+        # Create object location directory, ignoring if already present
+        # as multiple version files can exist
+        os.makedirs(_local_dir, exist_ok=True)
+
+        _local_file = os.path.join(
+            _local_dir, f"{_user_version}.{entry['file_type']}"
+        )
+        # Copy the temporary file into the data store
+        # then remove temporary file to save space
+        logger.debug("Saving data file to '%s'", _local_file)
+        shutil.copy(_temp_data_file, _local_file)
+
+        os.remove(_temp_data_file)
+
+        if "public" in entry:
+            _public = entry["public"]
+
+        data = copy.deepcopy(entry)
+
+        data["namespace_name"] = entry["use"]["namespace"]
+
+        logger.info(f"Registering: {_name}")
+
+        _file_url = fdp_store.store_data_file(
+            uri=local_uri,
+            repo_dir=repo_dir,
+            token=fdp_req.local_token(),
+            data=data,
+            local_file=_local_file,
+            write_data_store=write_data_store,
+            public=_public,
+        )
+
+        _stored_objects.append(_file_url)
+
+    return _stored_objects
```

### Comparing `fair_cli-0.5.2/fair/registry/requests.py` & `fair_cli-0.7.0/fair/registry/requests.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,565 +1,627 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-"""
-Registry Requests
-=================
-
-Methods relating to connection with local and remote registries for the purpose
-of synchronisation and push/pull.
-
-Contents
-========
-
-    local_token   - retrieves the local API token
-    post          - post to the registry RestAPI
-    get           - retrieve from the registry RestAPI
-    post_else_get - if an item already exists retrieve it, else create it
-
-"""
-
-__date__ = "2021-07-02"
-
-import copy
-import json
-import logging
-import os
-import shutil
-import tempfile
-import typing
-import urllib.parse
-import urllib.request
-
-import requests
-import simplejson.errors
-
-import fair.common as fdp_com
-import fair.exceptions as fdp_exc
-import fair.utilities as fdp_util
-
-logger = logging.getLogger("FAIRDataPipeline.Requests")
-
-
-def split_api_url(
-    request_url: str, splitter: str = "api"
-) -> typing.Tuple[str]:
-    """Split a request URL into endpoint and path
-
-    Parameters
-    ----------
-    request_url : str
-        URL to be split
-    splitter : str, optional
-        split point, by default 'api'
-
-    Returns
-    -------
-    typing.Tuple[str]
-        endpoint, path
-    """
-    _root, _path = request_url.split(f"{splitter}/")
-    return f"{_root}{splitter}", _path
-
-
-def local_token(registry_dir: str = None) -> str:
-    """Read the local registry token from the relevant file"""
-    registry_dir = registry_dir or fdp_com.registry_home()
-    _local_token_file = os.path.join(registry_dir, "token")
-    if not os.path.exists(_local_token_file):
-        raise fdp_exc.FileNotFoundError(
-            f"Failed to find local registry token, file '{_local_token_file}'"
-            " does not exist.",
-            hint="Try creating the file by manually starting the registry "
-            "by running 'fair registry start'",
-        )
-    _file_lines = open(_local_token_file).readlines()
-
-    if not _file_lines:
-        raise fdp_exc.FileNotFoundError(
-            f"Expected token in file {_local_token_file}, but file is empty"
-        )
-
-    return _file_lines[0].strip()
-
-
-def _access(
-    uri: str,
-    method: str,
-    token: str,
-    obj_path: str = None,
-    response_codes: typing.List[int] = None,
-    headers: typing.Dict[str, typing.Any] = None,
-    params: typing.Dict = None,
-    data: typing.Dict = None,
-):
-    if response_codes is None:
-        response_codes = [201, 200]
-    if not headers:
-        headers: typing.Dict[str, str] = {}
-
-    if not params:
-        params: typing.Dict[str, str] = {}
-
-    if not data:
-        data: typing.Dict[str, str] = {}
-
-    # Make sure we have the right number of '/' in the components
-    _uri = uri
-    _uri = fdp_util.check_trailing_slash(_uri)
-
-    _url = urllib.parse.urljoin(_uri, obj_path) if obj_path else uri
-
-    _url = fdp_util.check_trailing_slash(_url)
-
-    _headers = copy.deepcopy(headers)
-    if token:
-        _headers["Authorization"] = f"token {token}"
-
-    logger.debug("Sending request of type '%s': %s", method, _url)
-
-    try:
-        if method == "get":
-            logger.debug("Query parameters: %s", params)
-            _request = requests.get(_url, headers=_headers, params=params)
-        elif method == "post":
-            logger.debug("Post data: %s", data)
-            _request = requests.post(_url, headers=_headers, data=data)
-        else:
-            _request = getattr(requests, method)(_url, headers=_headers)
-    except requests.exceptions.ConnectionError as e:
-        raise fdp_exc.UnexpectedRegistryServerState(
-            f"Failed to make registry API request '{_url}'",
-            hint="Is this remote correct and the server running?",
-        ) from e
-
-    _info = f"url = {_url}, "
-    _info += f" parameters = {params}," if params else ""
-    _info += f" data = {data}" if data else ""
-
-    # Case of unrecognised object
-    if _request.status_code == 404:
-        raise fdp_exc.RegistryAPICallError(
-            f"Attempt to access an unrecognised resource on registry "
-            f"using method '{method}' and arguments: " + _info,
-            error_code=404,
-        )
-
-    # Case of unrecognised object
-
-    if _request.status_code == 403:
-        raise fdp_exc.RegistryAPICallError(
-            f"Failed to run method '{method}' for url {_url}, request forbidden",
-            error_code=403,
-        )
-    elif _request.status_code == 409:
-        _searchable = obj_path or uri
-        raise fdp_exc.RegistryAPICallError(
-            f"Cannot post object of type '{_searchable}' "
-            f"using method '{method}' as it already exists."
-            f"Arguments:\n" + _info,
-            error_code=409,
-        )
-
-    try:
-        _json_req = _request.json()
-        _result = _json_req["results"] if "results" in _json_req else _json_req
-    except (json.JSONDecodeError, simplejson.errors.JSONDecodeError) as exc:
-        raise fdp_exc.RegistryAPICallError(
-            f"Failed to retrieve JSON data from request to '{_url}'",
-            error_code=_request.status_code,
-        ) from exc
-
-    if _request.status_code not in response_codes:
-        _info = ""
-        if isinstance(_result, dict) and "detail" in _result:
-            _info = _result["detail"]
-        if not _info:
-            _info = _result
-        raise fdp_exc.RegistryAPICallError(
-            f"Request failed with status code {_request.status_code}: {_info}",
-            error_code=_request.status_code,
-        )
-    return _result
-
-
-def post(
-    uri: str,
-    obj_path: str,
-    token: str,
-    data: typing.Dict[str, typing.Any],
-    headers: typing.Dict[str, typing.Any] = None,
-) -> typing.Dict:
-    """Post an object to the registry
-
-    Parameters
-    ----------
-    uri : str
-        endpoint of the registry
-    obj_path : str
-        type of object to post
-    token : str
-        token for accessing the registry
-    data : typing.Dict[str, typing.Any]
-        data for the object
-    headers : typing.Dict[str, typing.Any], optional
-        any additional headers for the request, by default None
-
-    Returns
-    -------
-    typing.Dict
-        resulting data returned from the request
-    """
-    if headers is None:
-        headers = {}
-
-    headers.update({"Content-Type": "application/json"})
-
-    for param, value in data.copy().items():
-        if not value:
-            logger.warning(
-                f"Key in post data '{param}' has no value so will be ignored"
-            )
-            del data[param]
-
-    return _access(
-        uri,
-        "post",
-        token,
-        obj_path,
-        headers=headers,
-        data=json.dumps(data, cls=fdp_util.JSONDateTimeEncoder),
-    )
-
-
-def url_get(url: str, token: str) -> typing.Dict:
-    """Send a URL only request and retrieve results
-
-    Unlike 'get' this method is 'raw' in that there is no validation of
-    components
-
-    Parameters
-    ----------
-    url : str
-        URL to send request to
-    token: str
-        url access token
-
-    Returns
-    -------
-    typing.Dict
-        results dictionary
-    """
-    return _access(url, "get", token)
-
-
-def get(
-    uri: str,
-    obj_path: str,
-    token: str,
-    headers: typing.Dict[str, typing.Any] = None,
-    params: typing.Dict[str, typing.Any] = None,
-) -> typing.Dict:
-    """Retrieve an object from the given registry
-
-    Parameters
-    ----------
-    uri : str
-        endpoint of the registry
-    obj_path : str
-        type of the object to fetch
-    token : str
-        token for accessing the registry
-    headers : typing.Dict[str, typing.Any], optional
-        any additional headers for the request, by default None
-    params : typing.Dict[str, typing.Any], optional
-        search parameters for the object, by default None
-
-    Returns
-    -------
-    typing.Dict
-        returned data for the given request
-    """
-    logger.debug(
-        "Retrieving object of type '%s' from registry at '%s' with parameters: %s",
-        obj_path,
-        uri,
-        params,
-    )
-
-    if not headers:
-        headers = {}
-
-    params = {} if not params else copy.deepcopy(params)
-
-    for param, value in params.copy().items():
-        if not value:
-            logger.warning(
-                f"Key in get parameters '{param}' has no value so will be ignored"
-            )
-            del params[param]
-
-    return _access(
-        uri, "get", token, obj_path=obj_path, headers=headers, params=params
-    )
-
-
-def post_else_get(
-    uri: str,
-    obj_path: str,
-    token: str,
-    data: typing.Dict[str, typing.Any],
-    params: typing.Dict[str, typing.Any] = None,
-) -> str:
-    """Post to the registry if an object does not exist else retrieve URL
-
-    Parameters
-    ----------
-    uri : str
-        endpoint of the registry
-    obj_path : str
-        object type to post
-    token : str
-        token to access registry
-    data : typing.Dict[str, typing.Any]
-        data for the object to be posted
-    params : typing.Dict[str, typing.Any], optional
-        parameters for searching if object exists, by default None
-
-    Returns
-    -------
-    str
-        URL for object either retrieved or posted
-    """
-    if not params:
-        params = {}
-
-    try:
-        logger.debug(
-            "Attempting to post an instance of '%s' to '%s'", obj_path, uri
-        )
-        _loc = post(uri, obj_path, data=data, token=token)
-    except fdp_exc.RegistryAPICallError as e:
-        if e.error_code != 409:
-            raise e
-        logger.debug(e.msg)
-        logger.debug("Object already exists, retrieving entry")
-        _loc = get(uri, obj_path, token, params=params)
-    if isinstance(_loc, list):
-        if not _loc:
-            logger.error(f"Results of URL query empty: {_loc}")
-            try:
-                _full_listing = get(uri, obj_path, token)
-                logger.debug(f"Available {obj_path}s: {_full_listing}")
-            except fdp_exc.RegistryError:
-                logger.debug("No entries of type '{obj_path}' exist")
-            raise fdp_exc.RegistryError(
-                "Expected to receive a URL location from registry post"
-            )
-        _loc = _loc[0]
-    if isinstance(_loc, dict):
-        _loc = _loc["url"]
-    return _loc
-
-def post_upload_url(
-    remote_uri: str,
-    remote_token: str,
-    file_hash: str
-) -> str:
-    _url = urllib.parse.urljoin(remote_uri, "data", file_hash)
-    return post(_url, None, remote_token)
-
-def filter_object_dependencies(
-    uri: str, obj_path: str, token: str, filter: typing.Dict[str, typing.Any]
-) -> typing.List[str]:
-    """Filter dependencies of an API object based on a set of conditions
-
-    Parameters
-    ----------
-    uri : str
-        endpoint of the registry
-    object : str
-        path of object type, e.g. 'code_run'
-    token : str
-        registry access token
-    filter : typing.Dict[str, typing.Any]
-        list of filters to apply to listing
-
-    Returns
-    -------
-    typing.List[str]
-        list of object type paths
-    """
-    logger.debug(
-        "Filtering dependencies for object '%s' and filter '%s'",
-        obj_path,
-        filter,
-    )
-    try:
-        _actions = _access(uri, "options", token, obj_path)["actions"]["POST"]
-    except KeyError:
-        # No 'actions' key means no dependencies
-        return []
-    _fields: typing.List[str] = []
-
-    for name, info in _actions.items():
-        _filter_result: typing.List[bool] = [
-            info[filt] == value
-            for filt, value in filter.items()
-            if filt in info
-        ]
-
-        if all(_filter_result):
-            _fields.append(name)
-
-    return _fields
-
-
-def get_filter_variables(
-    uri: str, obj_path: str, token: str
-) -> typing.List[str]:
-    """Retrieves a list of variables you can filter by for a given object
-
-    Parameters
-    ----------
-    uri : str
-        endpoint of registry
-    obj_path : str
-        type of object
-    token : str
-        registry access token
-
-    Returns
-    -------
-    typing.List[str]
-        list of filterable fields
-    """
-    try:
-        _filters = _access(uri, "options", token, obj_path)["filter_fields"]
-    except KeyError:
-        # No 'filter_fields' key means no filters
-        return []
-    return [*_filters]
-
-
-def get_writable_fields(
-    uri: str, obj_path: str, token: str
-) -> typing.List[str]:
-    """Retrieve a list of writable fields for the given RestAPI object
-
-    Parameters
-    ----------
-    uri : str
-        endpoint of the registry
-    object : str
-        path of object type, e.g. 'code_run'
-    token: str
-        registry access token
-
-    Returns
-    -------
-    typing.List[str]
-        list of object type paths
-    """
-    return filter_object_dependencies(
-        uri, obj_path, token, {"read_only": False}
-    )
-
-
-def download_file(url: str, chunk_size: int = 8192) -> str:
-    """Download a file from a given URL
-
-    Parameters
-    ----------
-    url : str
-        address of remote file
-    chunk_size : int, optional
-        chunk size for download, by default 8192
-
-    Returns
-    -------
-    str
-        path of downloaded temporary file
-    """
-    # Save the data to a temporary file so we can calculate the hash
-    _file, _fname = tempfile.mkstemp()
-
-    try:
-        with urllib.request.urlopen(url) as response, open(
-            _file, "wb"
-        ) as out_file:
-            shutil.copyfileobj(response, out_file)
-    except urllib.error.URLError as e:
-        raise fdp_exc.FAIRCLIException(
-            f"Failed to download file '{url}'"
-            f" due to connection error: {e.reason}"
-        ) from e
-
-    return _fname
-
-
-def get_dependency_listing(uri: str, token: str) -> typing.Dict:
-    """Get complete listing of all objects and their registry based dependencies
-
-    Parameters
-    ----------
-    uri : str
-        endpoint of the registry
-    token : str
-        registry access token
-
-    Returns
-    -------
-    typing.Dict
-        dictionary of object types and their registry based dependencies
-    """
-    _registry_objs = url_get(uri, token)
-
-    return {
-        obj: filter_object_dependencies(
-            uri,
-            obj,
-            token,
-            {"read_only": False, "type": "field", "local": True},
-        )
-        for obj in _registry_objs
-    }
-
-
-def get_obj_id_from_url(object_url: str) -> int:
-    """Retrieves the ID from an object url
-
-    Parameters
-    ----------
-    object_url : str
-        URL for an object on the registry
-
-    Returns
-    -------
-    int
-        integer ID for that object
-    """
-    _url = urllib.parse.urlparse(object_url)
-    return [i for i in _url.path.split("/") if i.strip()][-1]
-
-
-def get_obj_type_from_url(request_url: str, token: str) -> str:
-    """Retrieves the type of object from the given URL
-
-    Parameters
-    ----------
-    request_url : str
-        url to type check
-    token: str
-        token for accessing specified registry
-
-    Returns
-    -------
-    str
-        object type if recognised else empty string
-    """
-    _uri, _ = split_api_url(request_url)
-    for obj_type in sorted(
-        [*url_get(_uri, token=token)], key=len, reverse=True
-    ):
-        if obj_type in request_url:
-            return obj_type
-    return ""
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+"""
+Registry Requests
+=================
+
+Methods relating to connection with local and remote registries for the purpose
+of synchronisation and push/pull.
+
+Contents
+========
+
+    local_token   - retrieves the local API token
+    post          - post to the registry RestAPI
+    get           - retrieve from the registry RestAPI
+    post_else_get - if an item already exists retrieve it, else create it
+
+"""
+
+__date__ = "2021-07-02"
+
+import copy
+import json
+import logging
+import traceback
+import os
+import re
+import shutil
+import tempfile
+import typing
+import platform
+import urllib.parse
+import urllib.request
+
+import requests
+import simplejson.errors
+
+import fair.common as fdp_com
+import fair.exceptions as fdp_exc
+import fair.utilities as fdp_util
+
+import ssl
+from requests.adapters import HTTPAdapter
+from urllib3.poolmanager import PoolManager
+
+logger = logging.getLogger("FAIRDataPipeline.Requests")
+
+
+def split_api_url(
+    request_url: str, splitter: str = "api"
+) -> typing.Tuple[str]:
+    """Split a request URL into endpoint and path
+
+    Parameters
+    ----------
+    request_url : str
+        URL to be split
+    splitter : str, optional
+        split point, by default 'api'
+
+    Returns
+    -------
+    typing.Tuple[str]
+        endpoint, path
+    """
+    _root, _path = request_url.split(f"{splitter}/")
+    return f"{_root}{splitter}", _path
+
+
+def local_token(registry_dir: str = None) -> str:
+    """Read the local registry token from the relevant file"""
+    registry_dir = registry_dir or fdp_com.registry_home()
+    _local_token_file = os.path.join(registry_dir, "token")
+    if not os.path.exists(_local_token_file):
+        raise fdp_exc.FileNotFoundError(
+            f"Failed to find local registry token, file '{_local_token_file}'"
+            " does not exist.",
+            hint="Try creating the file by manually starting the registry "
+            "by running 'fair registry start'",
+        )
+    _file_lines = open(_local_token_file).readlines()
+
+    if not _file_lines:
+        raise fdp_exc.FileNotFoundError(
+            f"Expected token in file {_local_token_file}, but file is empty"
+        )
+
+    return _file_lines[0].strip()
+
+
+def _access(
+    uri: str,
+    method: str,
+    token: str,
+    obj_path: str = None,
+    response_codes: typing.List[int] = None,
+    headers: typing.Dict[str, typing.Any] = None,
+    params: typing.Dict = None,
+    data: typing.Dict = None,
+    files: typing.Dict = None,
+    trailing_slash = True,
+):
+    if response_codes is None:
+        response_codes = [201, 200]
+    if not headers:
+        headers: typing.Dict[str, str] = {}
+
+    if not params:
+        params: typing.Dict[str, str] = {}
+
+    if not data:
+        data: typing.Dict[str, str] = {}
+
+    # Make sure we have the right number of '/' in the components
+    _uri = uri
+    _uri = fdp_util.check_trailing_slash(_uri)
+
+    _url = urllib.parse.urljoin(_uri, obj_path) if obj_path else uri
+
+    if trailing_slash:
+        _url = fdp_util.check_trailing_slash(_url)
+    else:
+        _url = fdp_util.remove_trailing_slash(_url)
+
+    _headers = copy.deepcopy(headers)
+    if token:
+        _headers["Authorization"] = f"token {token}"
+
+    logger.debug("Sending request of type '%s': %s", method, _url)
+
+    try:
+        if method == "get":
+            logger.debug("Query parameters: %s", params)
+            _request = requests.get(_url, headers=_headers, params=params)
+        elif method == "post":
+            logger.debug("Post data: %s", data)
+            _request = requests.post(_url, headers=_headers, data=data)
+        elif method == "patch":
+            logger.debug("Patch data: %s", data)
+            _headers.update({"Content-Type": "application/json"})
+            _request = requests.patch(_url, headers=_headers, data=json.dumps(data))
+        else:
+            _request = getattr(requests, method)(_url, headers=_headers)
+    except requests.exceptions.ConnectionError as e:
+        raise fdp_exc.UnexpectedRegistryServerState(
+            f"Failed to make registry API request '{_url}'",
+            hint="Is this remote correct and the server running?",
+        ) from e
+
+    _info = f"url = {_url}, "
+    _info += f" parameters = {params}," if params else ""
+    _info += f" data = {data}" if data else ""
+
+    # Case of unrecognised object
+    if _request.status_code == 404:
+        raise fdp_exc.RegistryAPICallError(
+            f"Attempt to access an unrecognised resource on registry "
+            f"using method '{method}' and arguments: " + _info,
+            error_code=404,
+        )
+
+    # Case of unrecognised object
+
+    if _request.status_code == 403:
+        raise fdp_exc.RegistryAPICallError(
+            f"Failed to run method '{method}' for url {_url}, request forbidden",
+            error_code=403,
+        )
+    elif _request.status_code == 409:
+        _searchable = obj_path or uri
+        raise fdp_exc.RegistryAPICallError(
+            f"Cannot post object of type '{_searchable}' "
+            f"using method '{method}' as it already exists."
+            f"Arguments:\n" + _info,
+            error_code=409,
+        )
+
+    try:
+        _json_req = _request.json()
+        _result = _json_req["results"] if "results" in _json_req else _json_req
+    except (json.JSONDecodeError, simplejson.errors.JSONDecodeError) as exc:
+        raise fdp_exc.RegistryAPICallError(
+            f"Failed to retrieve JSON data from request to '{_url}'",
+            error_code=_request.status_code,
+        ) from exc
+
+    if _request.status_code not in response_codes:
+        _info = ""
+        if isinstance(_result, dict) and "detail" in _result:
+            _info = _result["detail"]
+        if not _info:
+            _info = _result
+        raise fdp_exc.RegistryAPICallError(
+            f"Request failed with status code {_request.status_code}: {_info}",
+            error_code=_request.status_code,
+        )
+    return _result
+
+
+def post(
+    uri: str,
+    obj_path: str,
+    token: str,
+    data: typing.Dict[str, typing.Any],
+    headers: typing.Dict[str, typing.Any] = None,
+) -> typing.Dict:
+    """Post an object to the registry
+
+    Parameters
+    ----------
+    uri : str
+        endpoint of the registry
+    obj_path : str
+        type of object to post
+    token : str
+        token for accessing the registry
+    data : typing.Dict[str, typing.Any]
+        data for the object
+    headers : typing.Dict[str, typing.Any], optional
+        any additional headers for the request, by default None
+
+    Returns
+    -------
+    typing.Dict
+        resulting data returned from the request
+    """
+    if headers is None:
+        headers = {}
+
+    headers.update({"Content-Type": "application/json"})
+
+    for param, value in data.copy().items():
+        if not value:
+            logger.debug(
+                f"Key in post data '{param}' has no value so will be ignored"
+            )
+            del data[param]
+
+    return _access(
+        uri,
+        "post",
+        token,
+        obj_path,
+        headers=headers,
+        data=json.dumps(data, cls=fdp_util.JSONDateTimeEncoder),
+    )
+
+
+def url_get(url: str, token: str) -> typing.Dict:
+    """Send a URL only request and retrieve results
+
+    Unlike 'get' this method is 'raw' in that there is no validation of
+    components
+
+    Parameters
+    ----------
+    url : str
+        URL to send request to
+    token: str
+        url access token
+
+    Returns
+    -------
+    typing.Dict
+        results dictionary
+    """
+    return _access(url, "get", token)
+
+def get(
+    uri: str,
+    obj_path: str,
+    token: str,
+    headers: typing.Dict[str, typing.Any] = None,
+    params: typing.Dict[str, typing.Any] = None,
+) -> typing.Dict:
+    """Retrieve an object from the given registry
+
+    Parameters
+    ----------
+    uri : str
+        endpoint of the registry
+    obj_path : str
+        type of the object to fetch
+    token : str
+        token for accessing the registry
+    headers : typing.Dict[str, typing.Any], optional
+        any additional headers for the request, by default None
+    params : typing.Dict[str, typing.Any], optional
+        search parameters for the object, by default None
+
+    Returns
+    -------
+    typing.Dict
+        returned data for the given request
+    """
+    logger.debug(
+        "Retrieving object of type '%s' from registry at '%s' with parameters: %s",
+        obj_path,
+        uri,
+        params,
+    )
+
+    if not headers:
+        headers = {}
+
+    params = {} if not params else copy.deepcopy(params)
+
+    for param, value in params.copy().items():
+        if not value:
+            logger.warning(
+                f"Key in get parameters '{param}' has no value so will be ignored"
+            )
+            del params[param]
+
+    return _access(
+        uri, "get", token, obj_path=obj_path, headers=headers, params=params
+    )
+
+
+def post_else_get(
+    uri: str,
+    obj_path: str,
+    token: str,
+    data: typing.Dict[str, typing.Any],
+    params: typing.Dict[str, typing.Any] = None,
+) -> str:
+    """Post to the registry if an object does not exist else retrieve URL
+
+    Parameters
+    ----------
+    uri : str
+        endpoint of the registry
+    obj_path : str
+        object type to post
+    token : str
+        token to access registry
+    data : typing.Dict[str, typing.Any]
+        data for the object to be posted
+    params : typing.Dict[str, typing.Any], optional
+        parameters for searching if object exists, by default None
+
+    Returns
+    -------
+    str
+        URL for object either retrieved or posted
+    """
+    if not params:
+        params = {}
+
+    try:
+        logger.debug(
+            "Attempting to post an instance of '%s' to '%s'", obj_path, uri
+        )
+        _loc = post(uri, obj_path, data=data, token=token)
+    except fdp_exc.RegistryAPICallError as e:
+        if e.error_code != 409:
+            raise e
+        logger.debug(e.msg)
+        logger.debug("Object already exists, retrieving entry")
+        _loc = get(uri, obj_path, token, params=params)
+    if isinstance(_loc, list):
+        if not _loc:
+            logger.error(f"Results of URL query empty: {_loc}")
+            try:
+                _full_listing = get(uri, obj_path, token)
+                logger.debug(f"Available {obj_path}s: {_full_listing}")
+            except fdp_exc.RegistryError:
+                logger.debug("No entries of type '{obj_path}' exist")
+            raise fdp_exc.RegistryError(
+                "Expected to receive a URL location from registry post"
+            )
+        _loc = _loc[0]
+    if isinstance(_loc, dict):
+        _loc = _loc["url"]
+    return _loc
+
+def post_upload_url(
+    remote_uri: str,
+    remote_token: str,
+    file_hash: str
+) -> str:
+    """Function to get a tempory url to upload and object to
+
+    Args:
+        remote_uri (str): Remote registry URL
+        remote_token (str): Remote token
+        file_hash (str): Hash of the file to be uploaded
+
+    Returns:
+        str: A tempory url to upload the object to
+    """
+    _url = urllib.parse.urljoin(remote_uri, "data/")
+    _url = urllib.parse.urljoin(_url, file_hash)
+    return _access(_url, "post", remote_token, trailing_slash= False)
+
+def filter_object_dependencies(
+    uri: str, obj_path: str, token: str, filter: typing.Dict[str, typing.Any]
+) -> typing.List[str]:
+    """Filter dependencies of an API object based on a set of conditions
+
+    Parameters
+    ----------
+    uri : str
+        endpoint of the registry
+    object : str
+        path of object type, e.g. 'code_run'
+    token : str
+        registry access token
+    filter : typing.Dict[str, typing.Any]
+        list of filters to apply to listing
+
+    Returns
+    -------
+    typing.List[str]
+        list of object type paths
+    """
+    logger.debug(
+        "Filtering dependencies for object '%s' and filter '%s'",
+        obj_path,
+        filter,
+    )
+    try:
+        _actions = _access(uri, "options", token, obj_path)["actions"]["POST"]
+    except KeyError:
+        # No 'actions' key means no dependencies
+        return []
+    _fields: typing.List[str] = []
+
+    for name, info in _actions.items():
+        _filter_result: typing.List[bool] = [
+            info[filt] == value
+            for filt, value in filter.items()
+            if filt in info
+        ]
+
+        if all(_filter_result):
+            _fields.append(name)
+
+    return _fields
+
+
+def get_filter_variables(
+    uri: str, obj_path: str, token: str
+) -> typing.List[str]:
+    """Retrieves a list of variables you can filter by for a given object
+
+    Parameters
+    ----------
+    uri : str
+        endpoint of registry
+    obj_path : str
+        type of object
+    token : str
+        registry access token
+
+    Returns
+    -------
+    typing.List[str]
+        list of filterable fields
+    """
+    try:
+        _filters = _access(uri, "options", token, obj_path)["filter_fields"]
+    except KeyError:
+        # No 'filter_fields' key means no filters
+        return []
+    return [*_filters]
+
+
+def get_writable_fields(
+    uri: str, obj_path: str, token: str
+) -> typing.List[str]:
+    """Retrieve a list of writable fields for the given RestAPI object
+
+    Parameters
+    ----------
+    uri : str
+        endpoint of the registry
+    object : str
+        path of object type, e.g. 'code_run'
+    token: str
+        registry access token
+
+    Returns
+    -------
+    typing.List[str]
+        list of object type paths
+    """
+    return filter_object_dependencies(
+        uri, obj_path, token, {"read_only": False}
+    )
+
+def put_file(upload_url: str, file_loc: str) -> bool:
+    """Upload a file to a given url using put
+    Currently forces the use of TLS 1.2
+
+    Args:
+        upload_url (str): URL of where to send the put request to
+        file_loc (str): Location of the file to be uploaded
+
+    Raises:
+        fdp_exc.RegistryError: If the upload fails a RegistryError will be raised
+
+    Returns:
+        bool: Will return True if the upload succeeded.
+    """
+    s = requests.Session()
+    _req = s.put(upload_url, data= open(file_loc,'rb').read())
+    if _req.status_code not in [200, 201]:
+        raise fdp_exc.RegistryError(f"File: {file_loc} could not be uploaded, Registry Returned: {_req.status_code}")
+    return True
+
+def download_file(url: str, chunk_size: int = 8192) -> str:
+    """Download a file from a given URL
+
+    Parameters
+    ----------
+    url : str
+        address of remote file
+    chunk_size : int, optional
+        chunk size for download, by default 8192
+
+    Returns
+    -------
+    str
+        path of downloaded temporary file
+    """
+    # Save the data to a temporary file so we can calculate the hash
+    _file = tempfile.NamedTemporaryFile(delete=False)
+    _fname = _file.name
+
+    # Copy File if local (Windows fix)
+    if "file://" in url and platform.system() == "Windows":
+        _local_fname = url.replace("file://", "")
+        try:
+            shutil.copy2(_local_fname, _fname)
+        except Exception as e:
+            raise fdp_exc.FAIRCLIException(
+                f"Failed to download file '{url}'"
+                f" due to connection error: {traceback.format_exc()}"
+            ) from e
+
+    else:
+        try:
+            with urllib.request.urlopen(url) as response, open(
+                _fname, "wb"
+            ) as out_file:
+                shutil.copyfileobj(response, out_file)
+        except urllib.error.URLError as e:
+            raise fdp_exc.FAIRCLIException(
+                f"Failed to download file '{url}'"
+                f" due to connection error: {e.reason}"
+            ) from e
+
+    return _fname
+
+
+def get_dependency_listing(uri: str, token: str, read_only: bool = False) -> typing.Dict:
+    """Get complete listing of all objects and their registry based dependencies
+
+    Parameters
+    ----------
+    uri : str
+        endpoint of the registry
+    token : str
+        registry access token
+
+    Returns
+    -------
+    typing.Dict
+        dictionary of object types and their registry based dependencies
+    """
+    try:
+        _registry_objs = url_get(uri, token)
+    except:
+        return {[]}
+
+    _rtn =  {
+        obj: filter_object_dependencies(
+            uri,
+            obj,
+            token,
+            {"read_only": read_only, "type": "field", "local": True},
+        )
+        for obj in _registry_objs
+        }
+    return _rtn
+
+
+def get_obj_id_from_url(object_url: str) -> int:
+    """Retrieves the ID from an object url
+
+    Parameters
+    ----------
+    object_url : str
+        URL for an object on the registry
+
+    Returns
+    -------
+    int
+        integer ID for that object
+    """
+    _url = urllib.parse.urlparse(object_url)
+    return [i for i in _url.path.split("/") if i.strip()][-1]
+
+
+def get_obj_type_from_url(request_url: str, token: str) -> str:
+    """Retrieves the type of object from the given URL
+
+    Parameters
+    ----------
+    request_url : str
+        url to type check
+    token: str
+        token for accessing specified registry
+
+    Returns
+    -------
+    str
+        object type if recognised else empty string
+    """
+    _uri, _ = split_api_url(request_url)
+    for obj_type in sorted(
+        [*url_get(_uri, token=token)], key=len, reverse=True
+    ):
+        if obj_type in request_url:
+            return obj_type
+    return ""
```

### Comparing `fair_cli-0.5.2/fair/registry/server.py` & `fair_cli-0.7.0/fair/registry/server.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,496 +1,496 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-"""
-Registry Server Control
-=======================
-
-Contains methods for controlling the starting and stopping of the local
-FAIR Data Pipeline registry via the CLI.
-
-Contents
-========
-
-Functions
----------
-
-    check_server_running - confirm that the server is running locally
-
-"""
-
-__date__ = "2021-06-28"
-
-import enum
-import glob
-import logging
-import os
-import platform
-import shutil
-import subprocess
-import sys
-import typing
-
-import git
-import requests
-import yaml
-
-import fair.common as fdp_com
-import fair.configuration as fdp_conf
-import fair.exceptions as fdp_exc
-import fair.registry.requests as fdp_req
-import fair.registry.storage as fdp_store
-import fair.utilities as fdp_util
-import fair.virtualenv as fdp_env
-
-
-def django_environ(environ: typing.Dict = os.environ):
-    _environ = environ.copy()
-    _environ["DJANGO_SETTINGS_MODULE"] = "drams.local-settings"
-    _environ["DJANGO_SUPERUSER_USERNAME"] = "admin"
-    _environ["DJANGO_SUPERUSER_PASSWORD"] = "admin"
-    return _environ
-
-
-class SwitchMode(enum.Enum):
-    """Server access mode
-
-    The server can be launched either by the user or by the CLI itself. In the
-    latter case it will be shut down after use if no other instances are using it.
-    However if the user manually starts it themselves then the CLI will not
-    alter the state. This class handles all stop/start request possibilities.
-    """
-
-    USER_START = 0
-    USER_STOP = 1
-    CLI = 2
-    FORCE_STOP = 3
-    NO_SERVER = 4
-
-
-def check_server_running(local_uri: str = None) -> bool:
-    """Check the state of server
-
-    Parameters
-    ----------
-    local_uri : str
-        local registyr endpoint
-
-    Returns
-    -------
-    bool
-        whether server is running
-    """
-    logger = logging.getLogger("FAIRDataPipeline.Server")
-
-    if not local_uri:
-        local_uri = fdp_conf.get_local_uri()
-
-    logger.debug("Checking if server is running on '%s'", local_uri)
-
-    try:
-        _status_code = requests.get(local_uri).status_code
-        assert _status_code == 200
-        return True
-    except (requests.exceptions.ConnectionError, AssertionError):
-        return False
-
-
-def launch_server(
-    port: int = 8000, registry_dir: str = None, verbose: bool = False, address: str = "127.0.0.1"
-) -> int:
-    """Start the registry server.
-
-    Parameters
-    ----------
-    verbose : bool, optional
-        show registry start output, by default False
-    """
-    logger = logging.getLogger("FAIRDataPipeline.Server")
-
-    if not registry_dir:
-        registry_dir = fdp_com.registry_home()
-
-    _server_start_script = os.path.join(
-        registry_dir, "scripts", "start_fair_registry"
-    )
-
-    if platform.system() == "Windows":
-        _server_start_script += "_windows.bat"
-
-    if not os.path.exists(_server_start_script):
-        raise fdp_exc.RegistryError(
-            f"Failed to find local registry executable '{_server_start_script}',"
-            " is the FAIR data pipeline properly installed on this system?"
-        )
-
-    _cmd = [_server_start_script, "-p", f"{port}", "-a", f"{address}"]
-
-    os.environ["FAIR_ALLOWED_HOSTS"] = address if not "FAIR_ALLOWED_HOSTS" in os.environ else os.environ["FAIR_ALLOWED_HOSTS"] + f",{address}"
-
-    logger.debug("Launching server with command '%s'", " ".join(_cmd))
-
-    _start = subprocess.Popen(
-        _cmd,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.STDOUT,
-        shell=False,
-    )
-
-    if verbose and platform.system() != "Windows":
-        for c in iter(lambda: _start.stdout.read(1), b""):
-            sys.stdout.buffer.write(c)
-
-    _start.wait()
-
-    local_uri = fdp_conf.update_local_port()
-
-    if not check_server_running(local_uri):
-        raise fdp_exc.RegistryError(
-            "Failed to start local registry, no response from server"
-        )
-
-
-def stop_server(
-    registry_dir: str = None,
-    local_uri: str = None,
-    force: bool = False,
-    verbose: bool = False,
-) -> None:
-    """Stops the FAIR Data Pipeline local server
-
-    Parameters
-    ----------
-    force : bool, optional
-        whether to force server shutdown if it is being used
-    """
-    logger = logging.getLogger("FAIRDataPipeline.Server")
-
-    registry_dir = registry_dir or fdp_com.registry_home()
-    _session_port_file = fdp_com.registry_session_port_file(registry_dir)
-
-    if not os.path.exists(_session_port_file):
-        raise fdp_exc.FileNotFoundError(
-            "Failed to retrieve current session port from file "
-            f"'{_session_port_file}', file does not exist"
-        )
-
-    # If there are no session cache files shut down server
-    _run_files = glob.glob(os.path.join(fdp_com.session_cache_dir(), "*.run"))
-    if not force and _run_files:
-        raise fdp_exc.RegistryError(
-            "Could not stop registry server, processes still running."
-        )
-
-    _server_stop_script = os.path.join(
-        registry_dir, "scripts", "stop_fair_registry"
-    )
-
-    if platform.system() == "Windows":
-        _server_stop_script += "_windows.bat"
-
-    if not os.path.exists(_server_stop_script):
-        raise fdp_exc.RegistryError(
-            f"Failed to find local registry executable '{_server_stop_script}',"
-            " is the FAIR data pipeline properly installed on this system?"
-        )
-
-    logger.debug("Stopping local registry server.")
-
-    _stop = subprocess.Popen(
-        _server_stop_script,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.STDOUT,
-        shell=False,
-    )
-
-    if verbose:
-        for c in iter(lambda: _stop.stdout.read(1), b""):
-            sys.stdout.buffer.write(c)
-
-    _stop.wait()
-
-    if check_server_running(local_uri):
-        raise fdp_exc.RegistryError("Failed to stop registry server.")
-
-
-def rebuild_local(python: str, install_dir: str = None, silent: bool = False):
-    """Rebuild the local Django registry
-
-    Parameters
-    ----------
-    python : str
-        python binary of virtual environment
-    install_dir : str, optional
-        location of registry installation
-    silent : bool, optional
-        run in silent mode, by default False
-    """
-
-    logger = logging.getLogger("FAIRDataPipeline.Server")
-    logger.debug("Rebuilding local registry")
-    if not install_dir:
-        install_dir = fdp_com.DEFAULT_REGISTRY_LOCATION
-
-    _migration_files = glob.glob(
-        os.path.join(install_dir, "*", "migrations", "*.py*")
-    )
-
-    logger.debug("Removing migration files: %s", _migration_files)
-
-    for mf in _migration_files:
-        os.remove(mf)
-
-    _db_file = os.path.join(install_dir, "db.sqlite3")
-
-    logger.debug("Removing SQL database file")
-
-    if os.path.exists(_db_file):
-        os.remove(_db_file)
-
-    _manage = os.path.join(install_dir, "manage.py")
-
-    _sub_cmds = [
-        ("makemigrations", "custom_user"),
-        ("makemigrations", "data_management"),
-        ("migrate",),
-        (
-            "graph_models",
-            "data_management",
-            "--arrow-shape",
-            "crow",
-            "-x",
-            '"BaseModel,DataObject,DataObjectVersion"',
-            "-E",
-            "-o",
-            os.path.join(install_dir, "schema.dot"),
-        ),
-        ("collectstatic", "--noinput"),
-        ("createsuperuser", "--noinput"),
-    ]
-
-    logger.debug("Running Django migration commands as setup")
-
-    for sub in _sub_cmds:
-        subprocess.check_call(
-            [python, _manage, *sub],
-            shell=False,
-            stdout=subprocess.DEVNULL if silent else None,
-            env=django_environ(),
-        )
-
-    if shutil.which("dot"):
-        logger.debug("Creating schema diagram")
-        subprocess.check_call(
-            [
-                shutil.which("dot"),
-                os.path.join(install_dir, "schema.dot"),
-                "-Tsvg",
-                "-o",
-                os.path.join(install_dir, "static", "images", "schema.svg"),
-            ],
-            shell=False,
-            stdout=subprocess.DEVNULL if silent else None,
-        )
-
-
-def install_registry(
-    repository: str = fdp_com.FAIR_REGISTRY_REPO,
-    reference: str = None,
-    install_dir: str = None,
-    silent: bool = False,
-    force: bool = False,
-    venv_dir: str = None,
-) -> str:
-
-    logger = logging.getLogger("FAIRDataPipeline.Server")
-
-    if not install_dir:
-        install_dir = fdp_com.DEFAULT_REGISTRY_LOCATION
-
-    if os.path.exists(install_dir):
-        raise fdp_exc.RegistryError(
-            f"Local registry is already installed in {install_dir}"
-        )
-
-    logger.debug("Installing registry to '%s'", install_dir)
-
-    # In case registry installation occurs before setup
-    os.makedirs(fdp_com.global_config_dir(), exist_ok=True)
-
-    logger.debug("Updating registry path in global CLI configuration")
-    if os.path.exists(fdp_com.global_fdpconfig()):
-        _glob_conf = fdp_util.flatten_dict(fdp_conf.read_global_fdpconfig())
-        _glob_conf["registries.local.directory"] = install_dir
-
-        with open(fdp_com.global_fdpconfig(), "w") as out_conf:
-            yaml.dump(fdp_util.expand_dict(_glob_conf), out_conf)
-
-    if force:
-        logger.debug("Removing existing installation at '%s'", install_dir)
-        if platform.system() == "Windows":
-            fdp_com.set_file_permissions(install_dir)
-        shutil.rmtree(install_dir, ignore_errors=True)
-
-    logger.debug("Creating directories for installation if they do not exist")
-
-    os.makedirs(os.path.dirname(install_dir), exist_ok=True)
-
-    _repo = git.Repo.clone_from(repository, install_dir)
-
-    logger.debug("Retrieving the reference specified from the repository")
-
-    # If no reference is specified, use the latest tag for the registry
-    if not reference:
-        if not _repo.tags:
-            raise fdp_exc.RegistryError(
-                f"Expected tags in local registry repository '{repository}', "
-                "but found none"
-            )
-        _tags = sorted(_repo.tags, key=lambda t: t.commit.committed_datetime)
-        reference = _tags[-1].name
-
-    logger.debug("Using reference '%s' for registry checkout", reference)
-
-    _candidates = [t.name for t in _repo.tags + _repo.heads + _repo.remote().refs]
-
-    if reference not in _candidates:
-        raise fdp_exc.RegistryError(
-            f"No such head or tag '{reference}' in registry repository"
-            f"Candidates are {_candidates}"
-        )
-    else:
-        _repo.git.checkout(reference)
-
-    if not venv_dir:
-        venv_dir = os.path.join(install_dir, "venv")
-
-        _venv = fdp_env.FAIREnv(with_pip=True)
-
-        _venv.create(venv_dir)
-
-    _python_exe = "python.exe" if platform.system() == "Windows" else "python"
-    _binary_loc = "Scripts" if platform.system() == "Windows" else "bin"
-
-    _venv_python = shutil.which(
-        _python_exe, path=os.path.join(venv_dir, _binary_loc)
-    )
-
-    if not _venv_python:
-        raise FileNotFoundError(
-            f"Failed to find binary '{_python_exe}' in location '{venv_dir}"
-        )
-
-    logger.debug("Installing requirements")
-
-    subprocess.check_call(
-        [_venv_python, "-m", "pip", "install", "--upgrade", "pip", "wheel"],
-        shell=False,
-        stdout=subprocess.DEVNULL if silent else None,
-    )
-
-    subprocess.check_call(
-        [_venv_python, "-m", "pip", "install", "whitenoise"],
-        shell=False,
-        stdout=subprocess.DEVNULL if silent else None,
-    )
-
-    _requirements = os.path.join(install_dir, "local-requirements.txt")
-
-    if not os.path.exists(_requirements):
-        raise FileNotFoundError(f"Expected file '{_requirements}'")
-
-    subprocess.check_call(
-        [_venv_python, "-m", "pip", "install", "-r", _requirements],
-        shell=False,
-        stdout=subprocess.DEVNULL if silent else None,
-    )
-
-    rebuild_local(_venv_python, install_dir, silent)
-
-    return reference
-
-
-def uninstall_registry() -> None:
-    """Uninstall the local registry from the default location"""
-    logger = logging.getLogger("FAIRDataPipeline.Server")
-    # First check if the location can be retrieved from a CLI configuration
-    # else check the default install location
-    if os.path.exists(fdp_com.global_fdpconfig()) and os.path.exists(
-        fdp_com.registry_home()
-    ):
-        logger.debug(
-            "Uninstalling registry, removing '%s'", fdp_com.registry_home()
-        )
-        # On windows file permisions need to be set prior to removing the directory
-        if platform.system() == "Windows":
-            fdp_com.set_file_permissions(fdp_com.registry_home())
-        shutil.rmtree(fdp_com.registry_home())
-    elif os.path.exists(fdp_com.DEFAULT_REGISTRY_LOCATION):
-        logger.debug(
-            "Uninstalling registry, removing '%s'",
-            fdp_com.DEFAULT_REGISTRY_LOCATION,
-        )
-        # On windows file permisions need to be set prior to removing the directory
-        if platform.system() == "Windows":
-            fdp_com.set_file_permissions(fdp_com.DEFAULT_REGISTRY_LOCATION)
-        shutil.rmtree(fdp_com.DEFAULT_REGISTRY_LOCATION)
-    else:
-        raise fdp_exc.RegistryError(
-            "Cannot uninstall registry, no local installation identified"
-        )
-
-
-def update_registry_post_setup(
-    repo_dir: str, global_setup: bool = False
-) -> None:
-    """Add user namespace and file types after CLI setup
-
-    Parameters
-    ----------
-    repo_dir : str
-        current FAIR repository location
-    global_setup : bool, optional
-        whether this is the first (global) setup or local for a new repository
-    """
-    logger = logging.getLogger("FAIRDataPipeline.Server")
-
-    logger.debug("Updating registry from latest setup")
-
-    _is_running = check_server_running(fdp_conf.get_local_uri())
-
-    if not _is_running:
-        launch_server()
-
-    if global_setup:
-        logger.debug("Populating file types")
-        fdp_store.populate_file_type(
-            fdp_conf.get_local_uri(), fdp_req.local_token()
-        )
-
-    logger.debug("Adding 'author' and 'UserAuthor' entries if not present")
-    # Add author and UserAuthor
-    _author_url = fdp_store.store_user(
-        repo_dir, fdp_conf.get_local_uri(), fdp_req.local_token()
-    )
-
-    try:
-        _admin_url = fdp_req.get(
-            fdp_conf.get_local_uri(),
-            "users",
-            fdp_req.local_token(),
-            params={"username": "admin"},
-        )[0]["url"]
-    except (KeyError, IndexError) as e:
-        raise fdp_exc.RegistryError(
-            "Failed to retrieve 'admin' user from registry database"
-        ) from e
-
-    fdp_req.post_else_get(
-        fdp_conf.get_local_uri(),
-        "user_author",
-        fdp_req.local_token(),
-        data={"user": _admin_url, "author": _author_url},
-    )
-
-    # Only stop the server if it was not running initially
-    if not _is_running:
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+"""
+Registry Server Control
+=======================
+
+Contains methods for controlling the starting and stopping of the local
+FAIR Data Pipeline registry via the CLI.
+
+Contents
+========
+
+Functions
+---------
+
+    check_server_running - confirm that the server is running locally
+
+"""
+
+__date__ = "2021-06-28"
+
+import enum
+import glob
+import logging
+import os
+import platform
+import shutil
+import subprocess
+import sys
+import typing
+
+import git
+import requests
+import yaml
+
+import fair.common as fdp_com
+import fair.configuration as fdp_conf
+import fair.exceptions as fdp_exc
+import fair.registry.requests as fdp_req
+import fair.registry.storage as fdp_store
+import fair.utilities as fdp_util
+import fair.virtualenv as fdp_env
+
+
+def django_environ(environ: typing.Dict = os.environ):
+    _environ = environ.copy()
+    _environ["DJANGO_SETTINGS_MODULE"] = "drams.local-settings"
+    _environ["DJANGO_SUPERUSER_USERNAME"] = "admin"
+    _environ["DJANGO_SUPERUSER_PASSWORD"] = "admin"
+    return _environ
+
+
+class SwitchMode(enum.Enum):
+    """Server access mode
+
+    The server can be launched either by the user or by the CLI itself. In the
+    latter case it will be shut down after use if no other instances are using it.
+    However if the user manually starts it themselves then the CLI will not
+    alter the state. This class handles all stop/start request possibilities.
+    """
+
+    USER_START = 0
+    USER_STOP = 1
+    CLI = 2
+    FORCE_STOP = 3
+    NO_SERVER = 4
+
+
+def check_server_running(local_uri: str = None) -> bool:
+    """Check the state of server
+
+    Parameters
+    ----------
+    local_uri : str
+        local registyr endpoint
+
+    Returns
+    -------
+    bool
+        whether server is running
+    """
+    logger = logging.getLogger("FAIRDataPipeline.Server")
+
+    if not local_uri:
+        local_uri = fdp_conf.get_local_uri()
+
+    logger.debug("Checking if server is running on '%s'", local_uri)
+
+    try:
+        _status_code = requests.get(local_uri).status_code
+        assert _status_code == 200
+        return True
+    except (requests.exceptions.ConnectionError, AssertionError):
+        return False
+
+
+def launch_server(
+    port: int = 8000, registry_dir: str = None, verbose: bool = False, address: str = "127.0.0.1"
+) -> int:
+    """Start the registry server.
+
+    Parameters
+    ----------
+    verbose : bool, optional
+        show registry start output, by default False
+    """
+    logger = logging.getLogger("FAIRDataPipeline.Server")
+
+    if not registry_dir:
+        registry_dir = fdp_com.registry_home()
+
+    _server_start_script = os.path.join(
+        registry_dir, "scripts", "start_fair_registry"
+    )
+
+    if platform.system() == "Windows":
+        _server_start_script += "_windows.bat"
+
+    if not os.path.exists(_server_start_script):
+        raise fdp_exc.RegistryError(
+            f"Failed to find local registry executable '{_server_start_script}',"
+            " is the FAIR data pipeline properly installed on this system?"
+        )
+
+    _cmd = [_server_start_script, "-p", f"{port}", "-a", f"{address}"]
+
+    os.environ["FAIR_ALLOWED_HOSTS"] = address if not "FAIR_ALLOWED_HOSTS" in os.environ else os.environ["FAIR_ALLOWED_HOSTS"] + f",{address}"
+
+    logger.debug("Launching server with command '%s'", " ".join(_cmd))
+
+    _start = subprocess.Popen(
+        _cmd,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+        shell=False,
+    )
+
+    if verbose and platform.system() != "Windows":
+        for c in iter(lambda: _start.stdout.read(1), b""):
+            sys.stdout.buffer.write(c)
+
+    _start.wait()
+
+    local_uri = fdp_conf.update_local_port()
+
+    if not check_server_running(local_uri):
+        raise fdp_exc.RegistryError(
+            "Failed to start local registry, no response from server"
+        )
+
+
+def stop_server(
+    registry_dir: str = None,
+    local_uri: str = None,
+    force: bool = False,
+    verbose: bool = False,
+) -> None:
+    """Stops the FAIR Data Pipeline local server
+
+    Parameters
+    ----------
+    force : bool, optional
+        whether to force server shutdown if it is being used
+    """
+    logger = logging.getLogger("FAIRDataPipeline.Server")
+
+    registry_dir = registry_dir or fdp_com.registry_home()
+    _session_port_file = fdp_com.registry_session_port_file(registry_dir)
+
+    if not os.path.exists(_session_port_file):
+        raise fdp_exc.FileNotFoundError(
+            "Failed to retrieve current session port from file "
+            f"'{_session_port_file}', file does not exist"
+        )
+
+    # If there are no session cache files shut down server
+    _run_files = glob.glob(os.path.join(fdp_com.session_cache_dir(), "*.run"))
+    if not force and _run_files:
+        raise fdp_exc.RegistryError(
+            "Could not stop registry server, processes still running."
+        )
+
+    _server_stop_script = os.path.join(
+        registry_dir, "scripts", "stop_fair_registry"
+    )
+
+    if platform.system() == "Windows":
+        _server_stop_script += "_windows.bat"
+
+    if not os.path.exists(_server_stop_script):
+        raise fdp_exc.RegistryError(
+            f"Failed to find local registry executable '{_server_stop_script}',"
+            " is the FAIR data pipeline properly installed on this system?"
+        )
+
+    logger.debug("Stopping local registry server.")
+
+    _stop = subprocess.Popen(
+        _server_stop_script,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+        shell=False,
+    )
+
+    if verbose:
+        for c in iter(lambda: _stop.stdout.read(1), b""):
+            sys.stdout.buffer.write(c)
+
+    _stop.wait()
+
+    if check_server_running(local_uri):
+        raise fdp_exc.RegistryError("Failed to stop registry server.")
+
+
+def rebuild_local(python: str, install_dir: str = None, silent: bool = False):
+    """Rebuild the local Django registry
+
+    Parameters
+    ----------
+    python : str
+        python binary of virtual environment
+    install_dir : str, optional
+        location of registry installation
+    silent : bool, optional
+        run in silent mode, by default False
+    """
+
+    logger = logging.getLogger("FAIRDataPipeline.Server")
+    logger.debug("Rebuilding local registry")
+    if not install_dir:
+        install_dir = fdp_com.DEFAULT_REGISTRY_LOCATION
+
+    _migration_files = glob.glob(
+        os.path.join(install_dir, "*", "migrations", "*.py*")
+    )
+
+    logger.debug("Removing migration files: %s", _migration_files)
+
+    for mf in _migration_files:
+        os.remove(mf)
+
+    _db_file = os.path.join(install_dir, "db.sqlite3")
+
+    logger.debug("Removing SQL database file")
+
+    if os.path.exists(_db_file):
+        os.remove(_db_file)
+
+    _manage = os.path.join(install_dir, "manage.py")
+
+    _sub_cmds = [
+        ("makemigrations", "custom_user"),
+        ("makemigrations", "data_management"),
+        ("migrate",),
+        (
+            "graph_models",
+            "data_management",
+            "--arrow-shape",
+            "crow",
+            "-x",
+            '"BaseModel,DataObject,DataObjectVersion"',
+            "-E",
+            "-o",
+            os.path.join(install_dir, "schema.dot"),
+        ),
+        ("collectstatic", "--noinput"),
+        ("createsuperuser", "--noinput"),
+    ]
+
+    logger.debug("Running Django migration commands as setup")
+
+    for sub in _sub_cmds:
+        subprocess.check_call(
+            [python, _manage, *sub],
+            shell=False,
+            stdout=subprocess.DEVNULL if silent else None,
+            env=django_environ(),
+        )
+
+    if shutil.which("dot"):
+        logger.debug("Creating schema diagram")
+        subprocess.check_call(
+            [
+                shutil.which("dot"),
+                os.path.join(install_dir, "schema.dot"),
+                "-Tsvg",
+                "-o",
+                os.path.join(install_dir, "static", "images", "schema.svg"),
+            ],
+            shell=False,
+            stdout=subprocess.DEVNULL if silent else None,
+        )
+
+
+def install_registry(
+    repository: str = fdp_com.FAIR_REGISTRY_REPO,
+    reference: str = None,
+    install_dir: str = None,
+    silent: bool = False,
+    force: bool = False,
+    venv_dir: str = None,
+) -> str:
+
+    logger = logging.getLogger("FAIRDataPipeline.Server")
+
+    if not install_dir:
+        install_dir = fdp_com.DEFAULT_REGISTRY_LOCATION
+
+    if os.path.exists(install_dir):
+        raise fdp_exc.RegistryError(
+            f"Local registry is already installed in {install_dir}"
+        )
+
+    logger.debug("Installing registry to '%s'", install_dir)
+
+    # In case registry installation occurs before setup
+    os.makedirs(fdp_com.global_config_dir(), exist_ok=True)
+
+    logger.debug("Updating registry path in global CLI configuration")
+    if os.path.exists(fdp_com.global_fdpconfig()):
+        _glob_conf = fdp_util.flatten_dict(fdp_conf.read_global_fdpconfig())
+        _glob_conf["registries.local.directory"] = install_dir
+
+        with open(fdp_com.global_fdpconfig(), "w") as out_conf:
+            yaml.dump(fdp_util.expand_dict(_glob_conf), out_conf)
+
+    if force:
+        logger.debug("Removing existing installation at '%s'", install_dir)
+        if platform.system() == "Windows":
+            fdp_com.set_file_permissions(install_dir)
+        shutil.rmtree(install_dir, ignore_errors=True)
+
+    logger.debug("Creating directories for installation if they do not exist")
+
+    os.makedirs(os.path.dirname(install_dir), exist_ok=True)
+
+    _repo = git.Repo.clone_from(repository, install_dir)
+
+    logger.debug("Retrieving the reference specified from the repository")
+
+    # If no reference is specified, use the latest tag for the registry
+    if not reference:
+        if not _repo.tags:
+            raise fdp_exc.RegistryError(
+                f"Expected tags in local registry repository '{repository}', "
+                "but found none"
+            )
+        _tags = sorted(_repo.tags, key=lambda t: t.commit.committed_datetime)
+        reference = _tags[-1].name
+
+    logger.debug("Using reference '%s' for registry checkout", reference)
+
+    _candidates = [t.name for t in _repo.tags + _repo.heads + _repo.remote().refs]
+
+    if reference not in _candidates:
+        raise fdp_exc.RegistryError(
+            f"No such head or tag '{reference}' in registry repository"
+            f"Candidates are {_candidates}"
+        )
+    else:
+        _repo.git.checkout(reference)
+
+    if not venv_dir:
+        venv_dir = os.path.join(install_dir, "venv")
+
+        _venv = fdp_env.FAIREnv(with_pip=True)
+
+        _venv.create(venv_dir)
+
+    _python_exe = "python.exe" if platform.system() == "Windows" else "python"
+    _binary_loc = "Scripts" if platform.system() == "Windows" else "bin"
+
+    _venv_python = shutil.which(
+        _python_exe, path=os.path.join(venv_dir, _binary_loc)
+    )
+
+    if not _venv_python:
+        raise FileNotFoundError(
+            f"Failed to find binary '{_python_exe}' in location '{venv_dir}"
+        )
+
+    logger.debug("Installing requirements")
+
+    subprocess.check_call(
+        [_venv_python, "-m", "pip", "install", "--upgrade", "pip", "wheel"],
+        shell=False,
+        stdout=subprocess.DEVNULL if silent else None,
+    )
+
+    subprocess.check_call(
+        [_venv_python, "-m", "pip", "install", "whitenoise"],
+        shell=False,
+        stdout=subprocess.DEVNULL if silent else None,
+    )
+
+    _requirements = os.path.join(install_dir, "local-requirements.txt")
+
+    if not os.path.exists(_requirements):
+        raise FileNotFoundError(f"Expected file '{_requirements}'")
+
+    subprocess.check_call(
+        [_venv_python, "-m", "pip", "install", "-r", _requirements],
+        shell=False,
+        stdout=subprocess.DEVNULL if silent else None,
+    )
+
+    rebuild_local(_venv_python, install_dir, silent)
+
+    return reference
+
+
+def uninstall_registry() -> None:
+    """Uninstall the local registry from the default location"""
+    logger = logging.getLogger("FAIRDataPipeline.Server")
+    # First check if the location can be retrieved from a CLI configuration
+    # else check the default install location
+    if os.path.exists(fdp_com.global_fdpconfig()) and os.path.exists(
+        fdp_com.registry_home()
+    ):
+        logger.debug(
+            "Uninstalling registry, removing '%s'", fdp_com.registry_home()
+        )
+        # On windows file permisions need to be set prior to removing the directory
+        if platform.system() == "Windows":
+            fdp_com.set_file_permissions(fdp_com.registry_home())
+        shutil.rmtree(fdp_com.registry_home())
+    elif os.path.exists(fdp_com.DEFAULT_REGISTRY_LOCATION):
+        logger.debug(
+            "Uninstalling registry, removing '%s'",
+            fdp_com.DEFAULT_REGISTRY_LOCATION,
+        )
+        # On windows file permisions need to be set prior to removing the directory
+        if platform.system() == "Windows":
+            fdp_com.set_file_permissions(fdp_com.DEFAULT_REGISTRY_LOCATION)
+        shutil.rmtree(fdp_com.DEFAULT_REGISTRY_LOCATION)
+    else:
+        raise fdp_exc.RegistryError(
+            "Cannot uninstall registry, no local installation identified"
+        )
+
+
+def update_registry_post_setup(
+    repo_dir: str, global_setup: bool = False
+) -> None:
+    """Add user namespace and file types after CLI setup
+
+    Parameters
+    ----------
+    repo_dir : str
+        current FAIR repository location
+    global_setup : bool, optional
+        whether this is the first (global) setup or local for a new repository
+    """
+    logger = logging.getLogger("FAIRDataPipeline.Server")
+
+    logger.debug("Updating registry from latest setup")
+
+    _is_running = check_server_running(fdp_conf.get_local_uri())
+
+    if not _is_running:
+        launch_server()
+
+    if global_setup:
+        logger.debug("Populating file types")
+        fdp_store.populate_file_type(
+            fdp_conf.get_local_uri(), fdp_req.local_token()
+        )
+
+    logger.debug("Adding 'author' and 'UserAuthor' entries if not present")
+    # Add author and UserAuthor
+    _author_url = fdp_store.store_user(
+        repo_dir, fdp_conf.get_local_uri(), fdp_req.local_token()
+    )
+
+    try:
+        _admin_url = fdp_req.get(
+            fdp_conf.get_local_uri(),
+            "users",
+            fdp_req.local_token(),
+            params={"username": "admin"},
+        )[0]["url"]
+    except (KeyError, IndexError) as e:
+        raise fdp_exc.RegistryError(
+            "Failed to retrieve 'admin' user from registry database"
+        ) from e
+
+    fdp_req.post_else_get(
+        fdp_conf.get_local_uri(),
+        "user_author",
+        fdp_req.local_token(),
+        data={"user": _admin_url, "author": _author_url},
+    )
+
+    # Only stop the server if it was not running initially
+    if not _is_running:
         stop_server()
```

### Comparing `fair_cli-0.5.2/fair/registry/storage.py` & `fair_cli-0.7.0/fair/registry/storage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,830 +1,862 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-"""
-Registry Storage
-================
-
-Methods that add objects to the data registry.
-
-Contents
-========
-
-Functions
----------
-
-    get_write_storage - retrieve/create root data store
-    store_user - create author entry for the current user
-    populate_file_type - adds entries for standard file types
-    create_file_type - create a file type entry
-    store_working_config - create locations/objects for a working config
-
-"""
-
-__date__ = "2021-07-02"
-
-import hashlib
-import logging
-import os
-import typing
-
-import yaml
-
-import fair.configuration as fdp_conf
-import fair.exceptions as fdp_exc
-import fair.identifiers as fdp_id
-import fair.registry.file_types as fdp_file
-import fair.registry.requests as fdp_req
-import fair.registry.versioning as fdp_ver
-
-logger = logging.getLogger("FAIRDataPipeline.Storage")
-
-
-def get_write_storage(uri: str, write_data_store: str, token: str) -> str:
-    """Construct storage root if it does not exist
-
-    Parameters
-    ----------
-    uri : str
-        end point of the RestAPI
-    write_data_store : str
-        path of the write data store
-    token: str
-        registry access token
-
-    Returns
-    -------
-    str
-        URI of the created/retrieved storage root
-
-    Raises
-    ------
-    fdp_exc.UserConfigError
-        If 'write_data_store' not present in the working config or global config
-    """
-    logger.debug("Constructing a storage root for '%s'", write_data_store)
-
-    # Convert local file path to a valid data store path
-    _write_store_root = f"file://{write_data_store}"
-    if _write_store_root[-1] != os.path.sep:
-        _write_store_root += os.path.sep
-
-    if _search_root := fdp_req.get(
-        uri, "storage_root", token, params={"root": _write_store_root}
-    ):
-        return _search_root[0]["url"]
-
-    _post_data = {"root": _write_store_root, "local": True}
-    _storage_root = fdp_req.post(uri, "storage_root", token, data=_post_data)
-    return _storage_root["url"]
-
-
-def store_author(
-    uri: str, token: str, name: str, identifier: str = None, uuid: str = None
-) -> str:
-    """Creates an Author entry if one does not exist
-
-    Parameters
-    ----------
-    uri : str
-        registry RestAPI endpoint
-    token: str
-        registry access token
-    data: typing.Dict
-        author data to post
-    params: typing.Dict, optional
-        parameters to search if exists already
-
-    Returns
-    -------
-    str
-        URI for created author
-    """
-    _data = {"name": name, "identifier": identifier, "uuid": uuid}
-
-    return fdp_req.post_else_get(uri, "author", token, _data, {"name": name})
-
-
-def store_user(repo_dir: str, uri: str, token: str) -> str:
-    """Creates an Author entry for the user if one does not exist
-
-    Parameters
-    ----------
-    repo_dir: str
-        repository directory
-    token: str
-        registry access token
-    uri : str
-        registry RestAPI endpoint
-
-    Returns
-    -------
-    str
-        URI for created author
-    """
-
-    _user = fdp_conf.get_current_user_name(repo_dir)
-    name = " ".join(_user) if _user[1] else _user[0]
-    _id = None
-    _uuid = None
-
-    logger.debug("Storing user '%s'", name)
-
-    try:
-        _id = fdp_conf.get_current_user_uri(repo_dir)
-    except fdp_exc.CLIConfigurationError:
-        _uuid = fdp_conf.get_current_user_uuid(repo_dir)
-
-    return store_author(uri, token, name, _id, _uuid)
-
-
-def populate_file_type(uri: str, token: str) -> typing.List[typing.Dict]:
-    """Populates file_type table with common file file_types
-
-    Parameters
-    ----------
-    uri: str
-        registry RestAPI end point
-    token: str
-        registry access token
-    """
-    logger.debug("Adding file types to storage")
-
-    _type_objs = []
-
-    for _extension in fdp_file.FILE_TYPES:
-        # Use post_else_get in case some file types exist already
-        _result = create_file_type(uri, _extension, token)
-        _type_objs.append(_result)
-    return _type_objs
-
-
-def create_file_type(uri: str, extension: str, token: str) -> str:
-    """Creates a new file type on the registry
-
-    Parameters
-    ----------
-    uri : str
-        registry RestAPI end point
-    extension : str
-        file extension
-    token: str
-        registry access string
-
-    Returns
-    -------
-    str
-        URI for created file type
-    """
-    _name = fdp_file.FILE_TYPES[extension]
-
-    logger.debug("Adding file type '%s' with extension '%s'", _name, extension)
-
-    return fdp_req.post_else_get(
-        uri,
-        "file_type",
-        token,
-        data={"name": _name, "extension": extension.lower()},
-        params={"extension": extension.lower()},
-    )
-
-
-def store_working_config(
-    repo_dir: str, uri: str, work_cfg_yml: str, token: str
-) -> str:
-    """Construct a storage location and object for the working config
-
-    Parameters
-    ----------
-    repo_dir : str
-        local FAIR repository
-    uri : str
-        RestAPI end point
-    work_cfg_yml : str
-        location of working config yaml
-    token: str
-        registry access token
-
-    Returns
-    -------
-    str
-        new URI for the created object
-
-    Raises
-    ------
-    fair.exceptions.RegistryAPICallError
-        if bad status code returned from the registry
-    """
-    logger.debug("Storing working config on registry")
-
-    _root_store = get_write_storage(uri, work_cfg_yml, token)
-
-    _work_cfg = yaml.safe_load(open(work_cfg_yml))
-    _work_cfg_data_store = _work_cfg["run_metadata"]["write_data_store"]
-    _rel_path = os.path.relpath(work_cfg_yml, _work_cfg_data_store)
-    _time_stamp_dir = os.path.basename(os.path.dirname(work_cfg_yml))
-
-    # Construct hash from config contents and time stamp
-    # NOTE: You can have the same file stored N times for N job runs
-    # hence the use of a timestamp in the hashing
-    _hashable = open(work_cfg_yml).read() + _time_stamp_dir
-
-    _hash = hashlib.sha1(_hashable.encode("utf-8")).hexdigest()
-
-    _storage_loc_data = {
-        "path": _rel_path,
-        "storage_root": _root_store,
-        "public": _work_cfg["run_metadata"].get("public", True),
-        "hash": _hash,
-    }
-
-    try:
-        _post_store_loc = fdp_req.post(
-            uri, "storage_location", token, data=_storage_loc_data
-        )
-    except fdp_exc.RegistryAPICallError as e:
-        if e.error_code != 409:
-            raise e
-        else:
-            raise fdp_exc.RegistryAPICallError(
-                f"Cannot post storage_location '{_rel_path}' with hash '{_hash}', object already exists",
-                error_code=409,
-            ) from e
-
-    _user = store_user(repo_dir, uri, token)
-
-    _yaml_type = create_file_type(uri, "yaml", token)
-
-    _desc = f"Working configuration file for timestamp {_time_stamp_dir}"
-    _object_data = {
-        "description": _desc,
-        "storage_location": _post_store_loc["url"],
-        "file_type": _yaml_type,
-        "authors": [_user],
-    }
-
-    return fdp_req.post_else_get(
-        uri, "object", token, data=_object_data, params={"description": _desc}
-    )
-
-
-def store_working_script(
-    repo_dir: str, uri: str, script_path: str, working_config: str, token: str
-) -> str:
-    """Construct a storage location and object for the CLI run script
-
-    Parameters
-    ----------
-    repo_dir : str
-        local FAIR repository
-    uri : str
-        RestAPI end point
-    script_path : str
-        location of working CLI run script
-    data_store : str
-        data store path
-    token: str
-        registry access token
-
-    Returns
-    -------
-    str
-        new URI for the created object
-
-    Raises
-    ------
-    fair.exceptions.RegistryAPICallError
-        if bad status code returned from the registry
-    """
-    logger.debug("Storing working script on registry")
-
-    _work_cfg = yaml.safe_load(open(working_config))
-    _root_store = get_write_storage(uri, working_config, token)
-    _data_store = _work_cfg["run_metadata"]["write_data_store"]
-
-    _rel_path = os.path.relpath(script_path, _data_store)
-
-    _time_stamp_dir = os.path.basename(os.path.dirname(working_config))
-
-    # Construct hash from config contents and time
-    # NOTE: You can have the same file stored N times for N job runs
-    # hence the use of a timestamp in the hashing
-    _hashable = open(script_path).read() + _time_stamp_dir
-
-    _hash = hashlib.sha1(_hashable.encode("utf-8")).hexdigest()
-
-    _storage_loc_data = {
-        "path": _rel_path,
-        "storage_root": _root_store,
-        "public": _work_cfg["run_metadata"].get("public", True),
-        "hash": _hash,
-    }
-
-    try:
-        _post_store_loc = fdp_req.post(
-            uri, "storage_location", token, data=_storage_loc_data
-        )
-    except fdp_exc.RegistryAPICallError as e:
-        if e.error_code != 409:
-            raise e
-        else:
-            raise fdp_exc.RegistryAPICallError(
-                f"Cannot post storage_location "
-                f"'{_rel_path}' with hash"
-                f" '{_hash}', object already exists",
-                error_code=409,
-            ) from e
-
-    _user = store_user(repo_dir, uri, token)
-
-    _shell_script_type = create_file_type(uri, "sh", token)
-
-    _time_stamp_dir = os.path.basename(os.path.dirname(script_path))
-    _desc = f"Run script for timestamp {_time_stamp_dir}"
-    _object_data = {
-        "description": _desc,
-        "storage_location": _post_store_loc["url"],
-        "file_type": _shell_script_type,
-        "authors": [_user],
-    }
-
-    return fdp_req.post_else_get(
-        uri, "object", token, data=_object_data, params={"description": _desc}
-    )
-
-
-def store_namespace(
-    uri: str, token: str, name: str, full_name: str = None, website: str = None
-) -> str:
-    """Create a namespace on the registry
-
-    Parameters
-    ----------
-    uri : str
-        endpoint of the registry
-    namespace_label : str
-        name of the Namespace
-    token : str
-        registry access token
-    full_name : str, optional
-        full title of the namespace, by default None
-    website : str, optional
-        website relating to this namespace, by default None
-
-    Returns
-    -------
-    str
-        URL of the created namespace
-    """
-    logger.debug("Storing namespace '%s' on registry", name)
-
-    _data = {
-        "name": name,
-        "full_name": full_name,
-        "website": website,
-    }
-
-    return fdp_req.post_else_get(
-        uri, "namespace", token, data=_data, params={"name": name}
-    )
-
-
-def store_data_file(
-    uri: str,
-    repo_dir: str,
-    token: str,
-    data: typing.Dict,
-    local_file: str,
-    write_data_store: str,
-    public: bool,
-) -> None:
-
-    logger.debug("Storing data file '%s' on registry", local_file)
-
-    _root_store = get_write_storage(uri, write_data_store, token)
-
-    _rel_path = os.path.relpath(local_file, write_data_store)
-
-    if "version" not in data["use"]:
-        raise fdp_exc.InternalError(
-            f"Expected version number for '{local_file}' "
-            "registry submission but none found"
-        )
-
-    _post_store_loc = _get_url_from_storage_loc(
-        local_file=local_file,
-        registry_uri=uri,
-        registry_token=token,
-        relative_path=_rel_path,
-        root_store_url=_root_store,
-        is_public=public,
-    )
-
-    _user = store_user(repo_dir, uri, token)
-
-    _file_type = _get_url_from_file_type(
-        data=data,
-        local_file=local_file,
-        registry_uri=uri,
-        registry_token=token,
-    )
-
-    _namespace_url = _get_url_from_namespace(
-        data=data, label=local_file, registry_uri=uri, registry_token=token
-    )
-
-    _obj_url = _get_url_from_object(
-        data=data,
-        registry_uri=uri,
-        registry_token=token,
-        user=_user,
-        storage_loc_url=_post_store_loc,
-        file_type_url=_file_type,
-    )
-
-    _data_prod_url = _get_url_from_data_product(
-        data=data,
-        label=local_file,
-        registry_uri=uri,
-        registry_token=token,
-        namespace_url=_namespace_url,
-        object_url=_obj_url,
-    )
-
-    # If 'data_product' key present finish here and return URL
-    # else this is an external object
-    if "data_product" in data:
-        return _data_prod_url
-
-    return _get_url_from_external_obj(
-        data=data,
-        local_file=local_file,
-        registry_uri=uri,
-        registry_token=token,
-        data_product_url=_data_prod_url,
-    )
-
-
-def _get_url_from_storage_loc(
-    local_file: str,
-    registry_uri: str,
-    registry_token: str,
-    relative_path: str,
-    root_store_url: str,
-    is_public: bool,
-) -> str:
-    _hash = calculate_file_hash(local_file)
-
-    _storage_loc_data = {
-        "path": relative_path,
-        "storage_root": root_store_url,
-        "public": is_public,
-        "hash": _hash,
-    }
-
-    _search_data = {"hash": _hash}
-
-    return fdp_req.post_else_get(
-        registry_uri,
-        "storage_location",
-        registry_token,
-        data=_storage_loc_data,
-        params=_search_data,
-    )
-
-
-def _get_url_from_file_type(
-    data: typing.Dict, local_file: str, registry_uri: str, registry_token: str
-) -> str:
-    if "file_type" in data:
-        _file_type = data["file_type"]
-    else:
-        _file_type = os.path.splitext(local_file)[1]
-
-    return create_file_type(registry_uri, _file_type, registry_token)
-
-
-def _get_url_from_namespace(
-    data: typing.Dict, label: str, registry_uri: str, registry_token: str
-) -> str:
-    # Namespace is read from the source information
-    if "namespace_name" not in data:
-        raise fdp_exc.UserConfigError(
-            f"Expected 'namespace_name' for item '{label}'"
-        )
-
-    _namespace_args = {
-        "name": data["namespace_name"],
-        "full_name": data["namespace_full_name"]
-        if "namespace_full_name" in data
-        else None,
-        "website": data.get("namespace_website", None),
-    }
-
-    return store_namespace(registry_uri, registry_token, **_namespace_args)
-
-
-def _get_url_from_external_obj(
-    data: typing.Dict,
-    local_file: str,
-    registry_uri: str,
-    registry_token: str,
-    data_product_url: str,
-) -> typing.Dict:
-    _expected_ext_obj_keys = ("release_date", "primary", "title")
-
-    for key in _expected_ext_obj_keys:
-        if key not in data:
-            raise fdp_exc.UserConfigError(
-                f"Expected key '{key}' for item '{local_file}'"
-            )
-
-    _external_obj_data = {
-        "data_product": data_product_url,
-        "title": data["title"],
-        "primary_not_supplement": f'{data["primary"]}',
-        "release_date": data["release_date"],
-    }
-    _external_obj_data.update(_get_identifier_from_data(data, local_file))
-
-    return fdp_req.post(
-        registry_uri,
-        "external_object",
-        registry_token,
-        data=_external_obj_data,
-    )
-
-
-def _get_url_from_object(
-    data: typing.Dict,
-    registry_uri: str,
-    registry_token: str,
-    user: str,
-    storage_loc_url: str,
-    file_type_url: str,
-) -> str:
-    _desc = data.get("description", None)
-
-    _object_data = {
-        "description": _desc,
-        "file_type": file_type_url,
-        "storage_location": storage_loc_url,
-        "authors": [user],
-    }
-
-    try:
-        return fdp_req.post(
-            registry_uri, "object", registry_token, data=_object_data
-        )["url"]
-    except fdp_exc.RegistryAPICallError as e:
-        if e.error_code != 409:
-            raise e
-        else:
-            raise fdp_exc.RegistryAPICallError(
-                f"Cannot post object" f"'{_desc}', duplicate already exists",
-                error_code=409,
-            ) from e
-
-    except KeyError as e:
-        raise fdp_exc.InternalError(
-            f"Expected key 'url' in local registry API response"
-            f" for post object '{_desc}'"
-        ) from e
-
-
-def _get_url_from_data_product(
-    data: typing.Dict,
-    label: str,
-    registry_uri: str,
-    registry_token: str,
-    namespace_url: str,
-    object_url: str,
-) -> str:
-    """Retrieve the URL for a given config data product"""
-    # Get the name of the entry
-    if "external_object" in data:
-        _name = data["external_object"]
-    elif "data_product" in data:
-        _name = data["data_product"]
-    else:
-        raise fdp_exc.UserConfigError(
-            f"Failed to determine type while storing item '{label}'"
-            "into registry"
-        )
-
-    if "data_product" in data["use"]:
-        _name = data["use"]["data_product"]
-
-    _data_prod_data = {
-        "namespace": namespace_url,
-        "object": object_url,
-        "version": str(data["use"]["version"]),
-        "name": _name,
-    }
-
-    try:
-        return fdp_req.post(
-            registry_uri, "data_product", registry_token, data=_data_prod_data
-        )["url"]
-    except fdp_exc.RegistryAPICallError as e:
-        if e.error_code != 409:
-            raise e
-        else:
-            raise fdp_exc.RegistryAPICallError(
-                f"Cannot post data_product '{_name}', duplicate already exists",
-                error_code=409,
-            ) from e
-
-    except KeyError as e:
-        raise fdp_exc.InternalError(
-            f"Expected key 'url' in local registry API response"
-            f" for post object '{_name}'"
-        ) from e
-
-
-def _get_identifier_from_data(
-    data: typing.Dict, label: str
-) -> typing.Dict[str, str]:
-    """Retrieve the identifier metadata from the data entry"""
-    _identifier: typing.Dict[str, str] = {}
-
-    if data.get("identifier", None):
-        if not fdp_id.check_id_permitted(data["identifier"]):
-            raise fdp_exc.UserConfigError(
-                "Identifier '"
-                + data["identifier"]
-                + "' is not a valid identifier"
-            )
-        _identifier["identifier"] = data["identifier"]
-    else:
-        try:
-            _identifier["alternate_identifier"] = data["unique_name"]
-        except KeyError as e:
-            raise fdp_exc.UserConfigError(
-                "No identifier/alternate_identifier given for "
-                f"item '{label}'",
-                hint="You must provide either a URL 'identifier', or "
-                "'unique_name' and 'source_name' keys",
-            ) from e
-
-        _identifier["alternate_identifier"] = data.get(
-            "alternate_identifier_type", "local source descriptor"
-        )
-
-    return _identifier
-
-
-def calculate_file_hash(file_name: str, buffer_size: int = 64 * 1024) -> str:
-    """Calculates the hash of a data file
-
-    Parameters
-    ----------
-    file_name : str
-        file to calculate
-
-    Returns
-    -------
-    str
-        SHA1 hash for file
-    """
-    # If the file is large we do not want to hash it in one go
-    _input_hasher = hashlib.sha1()
-
-    with open(file_name, "rb") as in_f:
-        _buffer = in_f.read(buffer_size)
-        while len(_buffer) > 0:
-            _input_hasher.update(_buffer)
-            _buffer = in_f.read(buffer_size)
-
-    return _input_hasher.hexdigest()
-
-
-def get_storage_root_obj_address(
-    remote_uri: str, remote_token: str, address_str: str
-) -> str:
-    """Retrieve the RestAPI URL for a given storage location on the registry
-
-    Parameters
-    ----------
-    remote_uri : str
-        endpoint of remote registry
-    remote_token : str
-        token for accessing remote registry
-    address_str : str
-        path of the storage location
-
-    Returns
-    -------
-    str
-        URL of the RestAPI object representing this address
-    """
-    try:
-        _results = fdp_req.get(
-            remote_uri,
-            "storage_root",
-            params={"root": address_str},
-            token=remote_token,
-        )
-        if not _results:
-            raise AssertionError
-    except (AssertionError, fdp_exc.RegistryAPICallError) as e:
-        raise fdp_exc.RegistryError(
-            f"Cannot find a match for path '{address_str}' "
-            f"from endpoint '{remote_uri}."
-        ) from e
-
-
-def check_match(input_object: str, results_list: typing.List[str]):
-    """Check if an object is already on the registry using a hash
-
-    In order to perform this check the results must be a list of storage
-    locations for a given list of data_products as SHA1 hashes are present
-    for locations only.
-
-    Parameters
-    ----------
-    input_object : str
-        object pending submission to registry
-    results_list : typing.List[str]
-        list of storage_location results matching search query
-    """
-    _hash_list = [res["hash"] for res in results_list]
-    return calculate_file_hash(input_object) in _hash_list
-
-
-def check_if_object_exists(
-    local_uri: str,
-    file_loc: str,
-    obj_type: str,
-    search_data: typing.Dict,
-    token: str,
-) -> str:
-    """Checks if a data product is already present in the registry
-
-    Parameters
-    ----------
-    local_uri : str
-        local registry endpoint
-    file_loc : str
-        path of file on system
-    obj_type : str
-        object type
-    search_data : typing.Dict
-        data for query
-    token : str
-        token for registry
-
-    Returns
-    -------
-    str
-        whether object is present with matching hash, present or absent
-        if present but not hash matched return the latest version identifier
-    """
-    _version = None
-
-    if "version" in search_data:
-        _version = search_data["version"]
-        if "${{" in _version:
-            del search_data["version"]
-
-    # Obtain list of storage_locations for the given data_product
-    _results = fdp_req.get(
-        local_uri, obj_type, params=search_data, token=token
-    )
-
-    try:
-        fdp_ver.get_correct_version(
-            version=_version, results_list=_results, free_write=True
-        )
-    except fdp_exc.UserConfigError:
-        return "absent"
-
-    if not _results:
-        return "absent"
-
-    if obj_type == "external_object":
-        _results = [res["data_product"] for res in _results]
-        _results = [fdp_req.url_get(r, token=token) for r in _results]
-
-    _object_urls = [res["object"] for res in _results]
-
-    _storage_urls = [
-        fdp_req.url_get(obj_url, token=token)["storage_location"]
-        for obj_url in _object_urls
-    ]
-
-    _storage_objs = [
-        fdp_req.url_get(store_url, token=token) for store_url in _storage_urls
-    ]
-
-    return "hash_match" if check_match(file_loc, _storage_objs) else _results
-
-def get_upload_url(
-    file_hash: str,
-    remote_uri: str = None,
-    remote_token: str = None,
-) -> str:
-    if not remote_uri: 
-        remote_uri = fdp_conf.get_remote_token()
-    if not remote_token:
-        remote_token = fdp_conf.get_remote_token()
-    return fdp_req.post_upload_url(remote_uri, remote_token, file_hash)
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+"""
+Registry Storage
+================
+
+Methods that add objects to the data registry.
+
+Contents
+========
+
+Functions
+---------
+
+    get_write_storage - retrieve/create root data store
+    store_user - create author entry for the current user
+    populate_file_type - adds entries for standard file types
+    create_file_type - create a file type entry
+    store_working_config - create locations/objects for a working config
+
+"""
+
+__date__ = "2021-07-02"
+
+import hashlib
+import logging
+import os
+import typing
+
+import yaml
+
+import fair.configuration as fdp_conf
+import fair.exceptions as fdp_exc
+import fair.identifiers as fdp_id
+import fair.registry.file_types as fdp_file
+import fair.registry.requests as fdp_req
+import fair.registry.versioning as fdp_ver
+
+logger = logging.getLogger("FAIRDataPipeline.Storage")
+
+
+def get_write_storage(uri: str, write_data_store: str, token: str) -> str:
+    """Construct storage root if it does not exist
+
+    Parameters
+    ----------
+    uri : str
+        end point of the RestAPI
+    write_data_store : str
+        path of the write data store
+    token: str
+        registry access token
+
+    Returns
+    -------
+    str
+        URI of the created/retrieved storage root
+
+    Raises
+    ------
+    fdp_exc.UserConfigError
+        If 'write_data_store' not present in the working config or global config
+    """
+    logger.debug("Constructing a storage root for '%s'", write_data_store)
+
+    # Convert local file path to a valid data store path
+    _write_store_root = f"file://{write_data_store}"
+    if _write_store_root[-1] != os.path.sep:
+        _write_store_root += os.path.sep
+
+    if _search_root := fdp_req.get(
+        uri, "storage_root", token, params={"root": _write_store_root}
+    ):
+        return _search_root[0]["url"]
+
+    _post_data = {"root": _write_store_root, "local": True}
+    _storage_root = fdp_req.post(uri, "storage_root", token, data=_post_data)
+    return _storage_root["url"]
+
+
+def store_author(
+    uri: str, token: str, name: str, identifier: str = None, uuid: str = None
+) -> str:
+    """Creates an Author entry if one does not exist
+
+    Parameters
+    ----------
+    uri : str
+        registry RestAPI endpoint
+    token: str
+        registry access token
+    data: typing.Dict
+        author data to post
+    params: typing.Dict, optional
+        parameters to search if exists already
+
+    Returns
+    -------
+    str
+        URI for created author
+    """
+    _data = {"name": name, "identifier": identifier, "uuid": uuid}
+
+    return fdp_req.post_else_get(uri, "author", token, _data, {"name": name})
+
+
+def store_user(repo_dir: str, uri: str, token: str) -> str:
+    """Creates an Author entry for the user if one does not exist
+
+    Parameters
+    ----------
+    repo_dir: str
+        repository directory
+    token: str
+        registry access token
+    uri : str
+        registry RestAPI endpoint
+
+    Returns
+    -------
+    str
+        URI for created author
+    """
+
+    _user = fdp_conf.get_current_user_name(repo_dir)
+    name = " ".join(_user) if _user[1] else _user[0]
+    _id = None
+    _uuid = None
+
+    logger.debug("Storing user '%s'", name)
+
+    try:
+        _id = fdp_conf.get_current_user_uri(repo_dir)
+    except fdp_exc.CLIConfigurationError:
+        _uuid = fdp_conf.get_current_user_uuid(repo_dir)
+
+    return store_author(uri, token, name, _id, _uuid)
+
+
+def populate_file_type(uri: str, token: str) -> typing.List[typing.Dict]:
+    """Populates file_type table with common file file_types
+
+    Parameters
+    ----------
+    uri: str
+        registry RestAPI end point
+    token: str
+        registry access token
+    """
+    logger.debug("Adding file types to storage")
+
+    _type_objs = []
+
+    for _extension in fdp_file.FILE_TYPES:
+        # Use post_else_get in case some file types exist already
+        _result = create_file_type(uri, _extension, token)
+        _type_objs.append(_result)
+    return _type_objs
+
+
+def create_file_type(uri: str, extension: str, token: str) -> str:
+    """Creates a new file type on the registry
+
+    Parameters
+    ----------
+    uri : str
+        registry RestAPI end point
+    extension : str
+        file extension
+    token: str
+        registry access string
+
+    Returns
+    -------
+    str
+        URI for created file type
+    """
+    _name = fdp_file.FILE_TYPES[extension]
+
+    logger.debug("Adding file type '%s' with extension '%s'", _name, extension)
+
+    return fdp_req.post_else_get(
+        uri,
+        "file_type",
+        token,
+        data={"name": _name, "extension": extension.lower()},
+        params={"extension": extension.lower()},
+    )
+
+
+def store_working_config(
+    repo_dir: str, uri: str, work_cfg_yml: str, token: str
+) -> str:
+    """Construct a storage location and object for the working config
+
+    Parameters
+    ----------
+    repo_dir : str
+        local FAIR repository
+    uri : str
+        RestAPI end point
+    work_cfg_yml : str
+        location of working config yaml
+    token: str
+        registry access token
+
+    Returns
+    -------
+    str
+        new URI for the created object
+
+    Raises
+    ------
+    fair.exceptions.RegistryAPICallError
+        if bad status code returned from the registry
+    """
+    logger.debug("Storing working config on registry")
+
+    _root_store = get_write_storage(uri, work_cfg_yml, token)
+
+    _work_cfg = yaml.safe_load(open(work_cfg_yml))
+    _work_cfg_data_store = _work_cfg["run_metadata"]["write_data_store"]
+    _rel_path = os.path.relpath(work_cfg_yml, _work_cfg_data_store)
+    _time_stamp_dir = os.path.basename(os.path.dirname(work_cfg_yml))
+
+    # Construct hash from config contents and time stamp
+    # NOTE: You can have the same file stored N times for N job runs
+    # hence the use of a timestamp in the hashing
+    _hashable = open(work_cfg_yml).read() + _time_stamp_dir
+
+    _hash = hashlib.sha1(_hashable.encode("utf-8")).hexdigest()
+
+    _storage_loc_data = {
+        "path": _rel_path,
+        "storage_root": _root_store,
+        "public": _work_cfg["run_metadata"].get("public", True),
+        "hash": _hash,
+    }
+
+    try:
+        _post_store_loc = fdp_req.post(
+            uri, "storage_location", token, data=_storage_loc_data
+        )
+    except fdp_exc.RegistryAPICallError as e:
+        if e.error_code != 409:
+            raise e
+        else:
+            raise fdp_exc.RegistryAPICallError(
+                f"Cannot post storage_location '{_rel_path}' with hash '{_hash}', object already exists",
+                error_code=409,
+            ) from e
+
+    _user = store_user(repo_dir, uri, token)
+
+    _yaml_type = create_file_type(uri, "yaml", token)
+
+    _desc = f"Working configuration file for timestamp {_time_stamp_dir}"
+    _object_data = {
+        "description": _desc,
+        "storage_location": _post_store_loc["url"],
+        "file_type": _yaml_type,
+        "authors": [_user],
+    }
+
+    return fdp_req.post_else_get(
+        uri, "object", token, data=_object_data, params={"description": _desc}
+    )
+
+
+def store_working_script(
+    repo_dir: str, uri: str, script_path: str, working_config: str, token: str
+) -> str:
+    """Construct a storage location and object for the CLI run script
+
+    Parameters
+    ----------
+    repo_dir : str
+        local FAIR repository
+    uri : str
+        RestAPI end point
+    script_path : str
+        location of working CLI run script
+    data_store : str
+        data store path
+    token: str
+        registry access token
+
+    Returns
+    -------
+    str
+        new URI for the created object
+
+    Raises
+    ------
+    fair.exceptions.RegistryAPICallError
+        if bad status code returned from the registry
+    """
+    logger.debug("Storing working script on registry")
+
+    _work_cfg = yaml.safe_load(open(working_config))
+    _root_store = get_write_storage(uri, working_config, token)
+    _data_store = _work_cfg["run_metadata"]["write_data_store"]
+
+    _rel_path = os.path.relpath(script_path, _data_store)
+
+    _time_stamp_dir = os.path.basename(os.path.dirname(working_config))
+
+    # Construct hash from config contents and time
+    # NOTE: You can have the same file stored N times for N job runs
+    # hence the use of a timestamp in the hashing
+    _hashable = open(script_path).read() + _time_stamp_dir
+
+    _hash = hashlib.sha1(_hashable.encode("utf-8")).hexdigest()
+
+    _storage_loc_data = {
+        "path": _rel_path,
+        "storage_root": _root_store,
+        "public": _work_cfg["run_metadata"].get("public", True),
+        "hash": _hash,
+    }
+
+    try:
+        _post_store_loc = fdp_req.post(
+            uri, "storage_location", token, data=_storage_loc_data
+        )
+    except fdp_exc.RegistryAPICallError as e:
+        if e.error_code != 409:
+            raise e
+        else:
+            raise fdp_exc.RegistryAPICallError(
+                f"Cannot post storage_location "
+                f"'{_rel_path}' with hash"
+                f" '{_hash}', object already exists",
+                error_code=409,
+            ) from e
+
+    _user = store_user(repo_dir, uri, token)
+
+    _shell_script_type = create_file_type(uri, "sh", token)
+
+    _time_stamp_dir = os.path.basename(os.path.dirname(script_path))
+    _desc = f"Run script for timestamp {_time_stamp_dir}"
+    _object_data = {
+        "description": _desc,
+        "storage_location": _post_store_loc["url"],
+        "file_type": _shell_script_type,
+        "authors": [_user],
+    }
+
+    return fdp_req.post_else_get(
+        uri, "object", token, data=_object_data, params={"description": _desc}
+    )
+
+
+def store_namespace(
+    uri: str, token: str, name: str, full_name: str = None, website: str = None
+) -> str:
+    """Create a namespace on the registry
+
+    Parameters
+    ----------
+    uri : str
+        endpoint of the registry
+    namespace_label : str
+        name of the Namespace
+    token : str
+        registry access token
+    full_name : str, optional
+        full title of the namespace, by default None
+    website : str, optional
+        website relating to this namespace, by default None
+
+    Returns
+    -------
+    str
+        URL of the created namespace
+    """
+    logger.debug("Storing namespace '%s' on registry", name)
+
+    _data = {
+        "name": name,
+        "full_name": full_name,
+        "website": website,
+    }
+
+    return fdp_req.post_else_get(
+        uri, "namespace", token, data=_data, params={"name": name}
+    )
+
+
+def store_data_file(
+    uri: str,
+    repo_dir: str,
+    token: str,
+    data: typing.Dict,
+    local_file: str,
+    write_data_store: str,
+    public: bool,
+) -> None:
+
+    logger.debug("Storing data file '%s' on registry", local_file)
+
+    _root_store = get_write_storage(uri, write_data_store, token)
+
+    _rel_path = os.path.relpath(local_file, write_data_store)
+
+    if "version" not in data["use"]:
+        raise fdp_exc.InternalError(
+            f"Expected version number for '{local_file}' "
+            "registry submission but none found"
+        )
+
+    _post_store_loc = _get_url_from_storage_loc(
+        local_file=local_file,
+        registry_uri=uri,
+        registry_token=token,
+        relative_path=_rel_path,
+        root_store_url=_root_store,
+        is_public=public,
+    )
+
+    _user = store_user(repo_dir, uri, token)
+
+    _file_type = _get_url_from_file_type(
+        data=data,
+        local_file=local_file,
+        registry_uri=uri,
+        registry_token=token,
+    )
+
+    _namespace_url = _get_url_from_namespace(
+        data=data, label=local_file, registry_uri=uri, registry_token=token
+    )
+
+    _obj_url = _get_url_from_object(
+        data=data,
+        registry_uri=uri,
+        registry_token=token,
+        user=_user,
+        storage_loc_url=_post_store_loc,
+        file_type_url=_file_type,
+    )
+
+    _data_prod_url = _get_url_from_data_product(
+        data=data,
+        label=local_file,
+        registry_uri=uri,
+        registry_token=token,
+        namespace_url=_namespace_url,
+        object_url=_obj_url,
+    )
+
+    # If 'data_product' key present finish here and return URL
+    # else this is an external object
+    if "data_product" in data:
+        return _data_prod_url
+
+    return _get_url_from_external_obj(
+        data=data,
+        local_file=local_file,
+        registry_uri=uri,
+        registry_token=token,
+        data_product_url=_data_prod_url,
+    )
+
+
+def _get_url_from_storage_loc(
+    local_file: str,
+    registry_uri: str,
+    registry_token: str,
+    relative_path: str,
+    root_store_url: str,
+    is_public: bool,
+) -> str:
+    _hash = calculate_file_hash(local_file)
+
+    _storage_loc_data = {
+        "path": relative_path,
+        "storage_root": root_store_url,
+        "public": is_public,
+        "hash": _hash,
+    }
+
+    _search_data = {"hash": _hash}
+
+    return fdp_req.post_else_get(
+        registry_uri,
+        "storage_location",
+        registry_token,
+        data=_storage_loc_data,
+        params=_search_data,
+    )
+
+
+def _get_url_from_file_type(
+    data: typing.Dict, local_file: str, registry_uri: str, registry_token: str
+) -> str:
+    if "file_type" in data:
+        _file_type = data["file_type"]
+    else:
+        _file_type = os.path.splitext(local_file)[1]
+
+    return create_file_type(registry_uri, _file_type, registry_token)
+
+
+def _get_url_from_namespace(
+    data: typing.Dict, label: str, registry_uri: str, registry_token: str
+) -> str:
+    # Namespace is read from the source information
+    if "namespace_name" not in data:
+        raise fdp_exc.UserConfigError(
+            f"Expected 'namespace_name' for item '{label}'"
+        )
+
+    _namespace_args = {
+        "name": data["namespace_name"],
+        "full_name": data["namespace_full_name"]
+        if "namespace_full_name" in data
+        else None,
+        "website": data.get("namespace_website", None),
+    }
+
+    return store_namespace(registry_uri, registry_token, **_namespace_args)
+
+
+def _get_url_from_external_obj(
+    data: typing.Dict,
+    local_file: str,
+    registry_uri: str,
+    registry_token: str,
+    data_product_url: str,
+) -> typing.Dict:
+    _expected_ext_obj_keys = ("release_date", "primary", "title")
+
+    for key in _expected_ext_obj_keys:
+        if key not in data:
+            raise fdp_exc.UserConfigError(
+                f"Expected key '{key}' for item '{local_file}'"
+            )
+
+    _external_obj_data = {
+        "data_product": data_product_url,
+        "title": data["title"],
+        "primary_not_supplement": f'{data["primary"]}',
+        "release_date": data["release_date"],
+    }
+    _external_obj_data.update(_get_identifier_from_data(data, local_file))
+
+    return fdp_req.post(
+        registry_uri,
+        "external_object",
+        registry_token,
+        data=_external_obj_data,
+    )
+
+
+def _get_url_from_object(
+    data: typing.Dict,
+    registry_uri: str,
+    registry_token: str,
+    user: str,
+    storage_loc_url: str,
+    file_type_url: str,
+) -> str:
+    _desc = data.get("description", None)
+
+    _object_data = {
+        "description": _desc,
+        "file_type": file_type_url,
+        "storage_location": storage_loc_url,
+        "authors": [user],
+    }
+
+    try:
+        return fdp_req.post(
+            registry_uri, "object", registry_token, data=_object_data
+        )["url"]
+    except fdp_exc.RegistryAPICallError as e:
+        if e.error_code != 409:
+            raise e
+        else:
+            raise fdp_exc.RegistryAPICallError(
+                f"Cannot post object" f"'{_desc}', duplicate already exists",
+                error_code=409,
+            ) from e
+
+    except KeyError as e:
+        raise fdp_exc.InternalError(
+            f"Expected key 'url' in local registry API response"
+            f" for post object '{_desc}'"
+        ) from e
+
+
+def _get_url_from_data_product(
+    data: typing.Dict,
+    label: str,
+    registry_uri: str,
+    registry_token: str,
+    namespace_url: str,
+    object_url: str,
+) -> str:
+    """Retrieve the URL for a given config data product"""
+    # Get the name of the entry
+    if "external_object" in data:
+        _name = data["external_object"]
+    elif "data_product" in data:
+        _name = data["data_product"]
+    else:
+        raise fdp_exc.UserConfigError(
+            f"Failed to determine type while storing item '{label}'"
+            "into registry"
+        )
+
+    if "data_product" in data["use"]:
+        _name = data["use"]["data_product"]
+
+    _data_prod_data = {
+        "namespace": namespace_url,
+        "object": object_url,
+        "version": str(data["use"]["version"]),
+        "name": _name,
+    }
+
+    try:
+        return fdp_req.post(
+            registry_uri, "data_product", registry_token, data=_data_prod_data
+        )["url"]
+    except fdp_exc.RegistryAPICallError as e:
+        if e.error_code != 409:
+            raise e
+        else:
+            raise fdp_exc.RegistryAPICallError(
+                f"Cannot post data_product '{_name}', duplicate already exists",
+                error_code=409,
+            ) from e
+
+    except KeyError as e:
+        raise fdp_exc.InternalError(
+            f"Expected key 'url' in local registry API response"
+            f" for post object '{_name}'"
+        ) from e
+
+
+def _get_identifier_from_data(
+    data: typing.Dict, label: str
+) -> typing.Dict[str, str]:
+    """Retrieve the identifier metadata from the data entry"""
+    _identifier: typing.Dict[str, str] = {}
+
+    if data.get("identifier", None):
+        if not fdp_id.check_id_permitted(data["identifier"]):
+            raise fdp_exc.UserConfigError(
+                "Identifier '"
+                + data["identifier"]
+                + "' is not a valid identifier"
+            )
+        _identifier["identifier"] = data["identifier"]
+    else:
+        try:
+            _identifier["alternate_identifier"] = data["unique_name"]
+        except KeyError as e:
+            raise fdp_exc.UserConfigError(
+                "No identifier/alternate_identifier given for "
+                f"item '{label}'",
+                hint="You must provide either a URL 'identifier', or "
+                "'unique_name' and 'source_name' keys",
+            ) from e
+
+        _identifier["alternate_identifier"] = data.get(
+            "alternate_identifier_type", "local source descriptor"
+        )
+
+    return _identifier
+
+
+def calculate_file_hash(file_name: str, buffer_size: int = 64 * 1024) -> str:
+    """Calculates the hash of a data file
+
+    Parameters
+    ----------
+    file_name : str
+        file to calculate
+
+    Returns
+    -------
+    str
+        SHA1 hash for file
+    """
+    # If the file is large we do not want to hash it in one go
+    _input_hasher = hashlib.sha1()
+
+    with open(file_name, "rb") as in_f:
+        _buffer = in_f.read(buffer_size)
+        while len(_buffer) > 0:
+            _input_hasher.update(_buffer)
+            _buffer = in_f.read(buffer_size)
+
+    return _input_hasher.hexdigest()
+
+
+def get_storage_root_obj_address(
+    remote_uri: str, remote_token: str, address_str: str
+) -> str:
+    """Retrieve the RestAPI URL for a given storage location on the registry
+
+    Parameters
+    ----------
+    remote_uri : str
+        endpoint of remote registry
+    remote_token : str
+        token for accessing remote registry
+    address_str : str
+        path of the storage location
+
+    Returns
+    -------
+    str
+        URL of the RestAPI object representing this address
+    """
+    try:
+        _results = fdp_req.get(
+            remote_uri,
+            "storage_root",
+            params={"root": address_str},
+            token=remote_token,
+        )
+        if not _results:
+            raise AssertionError
+    except (AssertionError, fdp_exc.RegistryAPICallError) as e:
+        raise fdp_exc.RegistryError(
+            f"Cannot find a match for path '{address_str}' "
+            f"from endpoint '{remote_uri}."
+        ) from e
+
+
+def check_match(input_object: str, results_list: typing.List[str]):
+    """Check if an object is already on the registry using a hash
+
+    In order to perform this check the results must be a list of storage
+    locations for a given list of data_products as SHA1 hashes are present
+    for locations only.
+
+    Parameters
+    ----------
+    input_object : str
+        object pending submission to registry
+    results_list : typing.List[str]
+        list of storage_location results matching search query
+    """
+    _hash_list = [res["hash"] for res in results_list]
+    return calculate_file_hash(input_object) in _hash_list
+
+
+def check_if_object_exists(
+    local_uri: str,
+    file_loc: str,
+    obj_type: str,
+    search_data: typing.Dict,
+    token: str,
+) -> str:
+    """Checks if a data product is already present in the registry
+
+    Parameters
+    ----------
+    local_uri : str
+        local registry endpoint
+    file_loc : str
+        path of file on system
+    obj_type : str
+        object type
+    search_data : typing.Dict
+        data for query
+    token : str
+        token for registry
+
+    Returns
+    -------
+    str
+        whether object is present with matching hash, present or absent
+        if present but not hash matched return the latest version identifier
+    """
+    _version = None
+
+    if "version" in search_data:
+        _version = search_data["version"]
+        if "${{" in _version:
+            del search_data["version"]
+
+    # Obtain list of storage_locations for the given data_product
+    _results = fdp_req.get(
+        local_uri, obj_type, params=search_data, token=token
+    )
+
+    try:
+        fdp_ver.get_correct_version(
+            version=_version, results_list=_results, free_write=True
+        )
+    except fdp_exc.UserConfigError:
+        return "absent"
+
+    if not _results:
+        return "absent"
+
+    if obj_type == "external_object":
+        _results = [res["data_product"] for res in _results]
+        _results = [fdp_req.url_get(r, token=token) for r in _results]
+
+    _object_urls = [res["object"] for res in _results]
+
+    _storage_urls = [
+        fdp_req.url_get(obj_url, token=token)["storage_location"]
+        for obj_url in _object_urls
+    ]
+
+    _storage_objs = [
+        fdp_req.url_get(store_url, token=token) for store_url in _storage_urls
+    ]
+
+    return "hash_match" if check_match(file_loc, _storage_objs) else _results
+
+def get_upload_url(
+    file_loc: str,
+    remote_uri: str = None,
+    remote_token: str = None,
+) -> str:
+    """Wrapper function to get an upload_url for object storage
+
+    Args:
+        file_loc (str): File Location
+        remote_uri (str, optional): Remote Registry URL. Defaults to None.
+        remote_token (str, optional): Remote Registry Token. Defaults to None.
+
+    Returns:
+        str: Ad upload url for object storage
+    """
+    file_hash = calculate_file_hash(file_loc)
+    if not remote_uri: 
+        remote_uri = fdp_conf.get_remote_token()
+    if not remote_token:
+        remote_token = fdp_conf.get_remote_token()
+    return fdp_req.post_upload_url(remote_uri, remote_token, file_hash)['url']
+
+def upload_remote_file(
+    file_loc: str,
+    remote_uri = None,
+    remote_token = None,
+):
+    """Wrapper to upload a file to a remote registry
+
+    Args:
+        file_loc (str): Location of the file
+        remote_uri (_type_, optional): Remote Registry URL. Defaults to None.
+        remote_token (_type_, optional): Remote Registry Token. Defaults to None.
+
+    Raises:
+        fdp_exc.FileNotFoundError: If the file does not exist a FileNotFound error will be raised.
+    """
+    if not os.path.exists(file_loc):
+        raise fdp_exc.FileNotFoundError(f'File: {file_loc} does not exist')
+    _upload_url = get_upload_url(file_loc, remote_uri, remote_token)
+    logger.debug(f"Uploading {file_loc} to URL: {_upload_url}")
+    fdp_req.put_file(_upload_url, file_loc)
```

### Comparing `fair_cli-0.5.2/fair/registry/versioning.py` & `fair_cli-0.7.0/fair/registry/versioning.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-"""
-Versioning
-==========
-
-Methods for handling semantic versioning and parsing version formats
-
-Contents
-========
-
-Functions
----------
-    parse_incrementer - parse version increment format
-
-"""
-
-
-import contextlib
-
-__date__ = "2021-08-05"
-
-import re
-import typing
-
-import semver
-
-import fair.exceptions as fdp_exc
-
-BUMP_FUNCS = {
-    "LATEST": None,
-    "MINOR": "bump_minor",
-    "MAJOR": "bump_major",
-    "PATCH": "bump_patch",
-    "BUILD": "bump_build",
-    "PRERELEASE": "bump_prerelease",
-}
-
-DEFAULT_WRITE_VERSION = "PATCH"
-DEFAULT_READ_VERSION = "LATEST"
-
-
-def parse_incrementer(incrementer: str) -> str:
-    """Convert an incrementer string in a config to the relevant bump function
-
-    Parameters
-    ----------
-        incrementer : str
-            config.yaml variable to describe how version increases are handled
-
-    Returns
-    -------
-        str
-            relevant member method of VersionInfo for 'bumping' the semantic version
-
-    """
-    # Sanity check to confirm all methods are still present in semver module
-    for func in BUMP_FUNCS.values():
-        if func and func not in dir(semver.VersionInfo):
-            raise fdp_exc.InternalError(
-                f"Unrecognised 'semver.VersionInfo' method '{func}'"
-            )
-
-    for component in BUMP_FUNCS:
-        try:
-            if re.findall(r"\$\{\{\s*" + component + r"\s*\}\}", incrementer):
-                return BUMP_FUNCS[component]
-        except TypeError as e:
-            raise fdp_exc.InternalError(
-                f"Failed to parse incrementer '{incrementer}' expected string"
-            ) from e
-
-    raise fdp_exc.UserConfigError(
-        f"Unrecognised version incrementer variable '{incrementer}'"
-    )
-
-
-def undo_incrementer(incrementer: str) -> str:
-    """Convert an incrementer string to just return the latest value
-
-    Parameters
-    ----------
-        incrementer : str
-            config.yaml variable to describe how version increases are handled for register
-
-    Returns
-    -------
-        str
-            correct value for version string for read
-
-    """
-    for component in BUMP_FUNCS:
-        if re.findall(r"\$\{\{\s*" + component + r"\s*\}\}", incrementer):
-            return re.sub(
-                r"\$\{\{\s*" + component + r"\s*\}\}",
-                "${{ LATEST }}",
-                incrementer,
-            )
-
-    return incrementer
-
-
-def get_latest_version(results_list: typing.List = None) -> semver.VersionInfo:
-    if not results_list:
-        return semver.VersionInfo.parse("0.0.0")
-
-    _versions = [
-        semver.VersionInfo.parse(i["version"])
-        for i in results_list
-        if "version" in i
-    ]
-
-    if not _versions:
-        return semver.VersionInfo.parse("0.0.0")
-
-    return max(_versions)
-
-
-def get_correct_version(
-    version: str, results_list: typing.List = None, free_write: bool = True
-) -> semver.VersionInfo:
-
-    # Version is already specified
-    if isinstance(version, semver.VersionInfo):
-        return version
-
-    with contextlib.suppress(ValueError):
-        return semver.VersionInfo.parse(version)
-    _zero = semver.VersionInfo.parse("0.0.0")
-
-    if results_list:
-        _versions = [
-            semver.VersionInfo.parse(i["version"])
-            for i in results_list
-            if "version" in i
-        ]
-    else:
-        _versions = []
-
-    try:
-        _bump_func = parse_incrementer(version)
-        if free_write:
-            _versions.append(_zero)
-
-        if not _versions:
-            raise fdp_exc.InternalError(
-                f"Version parsing failed for version={version}, free_write={free_write}"
-            )
-        _max_ver = max(_versions)
-
-        _new_version = (
-            getattr(_max_ver, _bump_func)() if _bump_func else _max_ver
-        )
-    except fdp_exc.UserConfigError:  # Not a command, try an exact version
-        _new_version = semver.VersionInfo.parse(version)
-
-    if _new_version in _versions and free_write:
-        raise fdp_exc.UserConfigError(
-            f"Trying to create existing version: {_new_version}"
-        )
-    elif _new_version not in _versions and not free_write:
-        raise fdp_exc.UserConfigError(
-            f"Trying to read non-existing version: {_new_version}"
-        )
-    elif _new_version == _zero:
-        raise fdp_exc.UserConfigError(f"Trying to work with version {_zero}")
-
-    return _new_version
-
-
-def default_bump(version: semver.VersionInfo) -> semver.VersionInfo:
-    """Perform default version bump
-
-    For FAIR-CLI the default version increment is patch
-
-    Parameters
-    ----------
-        version: semver.VersionInfo
-
-    Returns
-    -------
-        new version
-    """
-    return getattr(version, BUMP_FUNCS[DEFAULT_WRITE_VERSION])()
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+"""
+Versioning
+==========
+
+Methods for handling semantic versioning and parsing version formats
+
+Contents
+========
+
+Functions
+---------
+    parse_incrementer - parse version increment format
+
+"""
+
+
+import contextlib
+
+__date__ = "2021-08-05"
+
+import re
+import typing
+
+import semver
+
+import fair.exceptions as fdp_exc
+
+BUMP_FUNCS = {
+    "LATEST": None,
+    "MINOR": "bump_minor",
+    "MAJOR": "bump_major",
+    "PATCH": "bump_patch",
+    "BUILD": "bump_build",
+    "PRERELEASE": "bump_prerelease",
+}
+
+DEFAULT_WRITE_VERSION = "PATCH"
+DEFAULT_READ_VERSION = "LATEST"
+
+
+def parse_incrementer(incrementer: str) -> str:
+    """Convert an incrementer string in a config to the relevant bump function
+
+    Parameters
+    ----------
+        incrementer : str
+            config.yaml variable to describe how version increases are handled
+
+    Returns
+    -------
+        str
+            relevant member method of VersionInfo for 'bumping' the semantic version
+
+    """
+    # Sanity check to confirm all methods are still present in semver module
+    for func in BUMP_FUNCS.values():
+        if func and func not in dir(semver.VersionInfo):
+            raise fdp_exc.InternalError(
+                f"Unrecognised 'semver.VersionInfo' method '{func}'"
+            )
+
+    for component in BUMP_FUNCS:
+        try:
+            if re.findall(r"\$\{\{\s*" + component + r"\s*\}\}", incrementer):
+                return BUMP_FUNCS[component]
+        except TypeError as e:
+            raise fdp_exc.InternalError(
+                f"Failed to parse incrementer '{incrementer}' expected string"
+            ) from e
+
+    raise fdp_exc.UserConfigError(
+        f"Unrecognised version incrementer variable '{incrementer}'"
+    )
+
+
+def undo_incrementer(incrementer: str) -> str:
+    """Convert an incrementer string to just return the latest value
+
+    Parameters
+    ----------
+        incrementer : str
+            config.yaml variable to describe how version increases are handled for register
+
+    Returns
+    -------
+        str
+            correct value for version string for read
+
+    """
+    for component in BUMP_FUNCS:
+        if re.findall(r"\$\{\{\s*" + component + r"\s*\}\}", incrementer):
+            return re.sub(
+                r"\$\{\{\s*" + component + r"\s*\}\}",
+                "${{ LATEST }}",
+                incrementer,
+            )
+
+    return incrementer
+
+
+def get_latest_version(results_list: typing.List = None) -> semver.VersionInfo:
+    if not results_list:
+        return semver.VersionInfo.parse("0.0.0")
+
+    _versions = [
+        semver.VersionInfo.parse(i["version"])
+        for i in results_list
+        if "version" in i
+    ]
+
+    if not _versions:
+        return semver.VersionInfo.parse("0.0.0")
+
+    return max(_versions)
+
+
+def get_correct_version(
+    version: str, results_list: typing.List = None, free_write: bool = True
+) -> semver.VersionInfo:
+
+    # Version is already specified
+    if isinstance(version, semver.VersionInfo):
+        return version
+
+    with contextlib.suppress(ValueError):
+        return semver.VersionInfo.parse(version)
+    _zero = semver.VersionInfo.parse("0.0.0")
+
+    if results_list:
+        _versions = [
+            semver.VersionInfo.parse(i["version"])
+            for i in results_list
+            if "version" in i
+        ]
+    else:
+        _versions = []
+
+    try:
+        _bump_func = parse_incrementer(version)
+        if free_write:
+            _versions.append(_zero)
+
+        if not _versions:
+            raise fdp_exc.InternalError(
+                f"Version parsing failed for version={version}, free_write={free_write}"
+            )
+        _max_ver = max(_versions)
+
+        _new_version = (
+            getattr(_max_ver, _bump_func)() if _bump_func else _max_ver
+        )
+    except fdp_exc.UserConfigError:  # Not a command, try an exact version
+        _new_version = semver.VersionInfo.parse(version)
+
+    if _new_version in _versions and free_write:
+        raise fdp_exc.UserConfigError(
+            f"Trying to create existing version: {_new_version}"
+        )
+    elif _new_version not in _versions and not free_write:
+        raise fdp_exc.UserConfigError(
+            f"Trying to read non-existing version: {_new_version}"
+        )
+    elif _new_version == _zero:
+        raise fdp_exc.UserConfigError(f"Trying to work with version {_zero}")
+
+    return _new_version
+
+
+def default_bump(version: semver.VersionInfo) -> semver.VersionInfo:
+    """Perform default version bump
+
+    For FAIR-CLI the default version increment is patch
+
+    Parameters
+    ----------
+        version: semver.VersionInfo
+
+    Returns
+    -------
+        new version
+    """
+    return getattr(version, BUMP_FUNCS[DEFAULT_WRITE_VERSION])()
```

### Comparing `fair_cli-0.5.2/fair/run.py` & `fair_cli-0.7.0/fair/run.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-"""
-
-Execute Job
-===========
-
-Creates required files for job execution and runs the job itself using the
-retrieved metadata
-
-"""
-
-__date__ = "2021-06-30"
-
-import glob
-import hashlib
-import logging
-import os
-import typing
-
-import fair.common as fdp_com
-import fair.exceptions as fdp_exc
-
-logger = logging.getLogger("FAIRDataPipeline.Run")
-
-# Dictionary of recognised shell labels.
-SHELLS: typing.Dict[str, str] = {
-    "pwsh": {"exec": "pwsh -command \". '{0}'\"", "extension": "ps1"},
-    "batch": {"exec": "{0}", "extension": "bat"},
-    "powershell": {
-        "exec": "powershell -command \". '{0}'\"",
-        "extension": "ps1",
-    },
-    "python2": {"exec": "python2 {0}", "extension": "py"},
-    "python3": {"exec": "python3 {0}", "extension": "py"},
-    "python": {"exec": "python {0}", "extension": "py"},
-    "R": {"exec": "R -f {0}", "extension": "R"},
-    "julia": {"exec": "julia {0}", "extension": "jl"},
-    "bash": {
-        "exec": "bash -eo pipefail {0}",
-        "extension": "sh",
-    },
-    "java": {"exec": "java {0}", "extension": "java"},
-    "sh": {"exec": "sh -e {0}", "extension": "sh"},
-}
-
-
-def get_job_hash(job_dir: str) -> str:
-    """Retrieve the hash for a given job
-
-    NOTE: A job can consist of multiple code runs if the API implementation
-    called initiates multiple executions. "Job" here refers to a call of
-    'fair run'.
-
-    Parameters
-    ----------
-    job_dir : str
-        jobs directory
-
-    Returns
-    -------
-    str
-        hash of job
-    """
-    if not os.path.exists(job_dir):
-        raise fdp_exc.FileNotFoundError(
-            "Failed to find hash for job, "
-            f"directory '{job_dir}' does not exist."
-        )
-    _directory = os.path.abspath(job_dir)
-    return hashlib.sha1(_directory.encode("utf-8")).hexdigest()
-
-
-def get_job_dir(job_hash: str) -> str:
-    """Get job directory from a hash
-
-    Parameters
-    ----------
-    job_hash : str
-        hash for a given job
-
-    Returns
-    -------
-    str
-        associated job directory
-    """
-    _jobs = glob.glob(os.path.join(fdp_com.default_jobs_dir(), "*"))
-
-    for job in _jobs:
-        _hash = hashlib.sha1(os.path.abspath(job).encode("utf-8")).hexdigest()
-        if _hash == job_hash:
-            return job
-
-    return ""
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+"""
+
+Execute Job
+===========
+
+Creates required files for job execution and runs the job itself using the
+retrieved metadata
+
+"""
+
+__date__ = "2021-06-30"
+
+import glob
+import hashlib
+import logging
+import os
+import typing
+
+import fair.common as fdp_com
+import fair.exceptions as fdp_exc
+
+logger = logging.getLogger("FAIRDataPipeline.Run")
+
+# Dictionary of recognised shell labels.
+SHELLS: typing.Dict[str, str] = {
+    "pwsh": {"exec": "pwsh -command \". '{0}'\"", "extension": "ps1"},
+    "batch": {"exec": "{0}", "extension": "bat"},
+    "powershell": {
+        "exec": "powershell -command \". '{0}'\"",
+        "extension": "ps1",
+    },
+    "python2": {"exec": "python2 {0}", "extension": "py"},
+    "python3": {"exec": "python3 {0}", "extension": "py"},
+    "python": {"exec": "python {0}", "extension": "py"},
+    "R": {"exec": "R -f {0}", "extension": "R"},
+    "julia": {"exec": "julia {0}", "extension": "jl"},
+    "bash": {
+        "exec": "bash -eo pipefail {0}",
+        "extension": "sh",
+    },
+    "java": {"exec": "java {0}", "extension": "java"},
+    "sh": {"exec": "sh -e {0}", "extension": "sh"},
+}
+
+
+def get_job_hash(job_dir: str) -> str:
+    """Retrieve the hash for a given job
+
+    NOTE: A job can consist of multiple code runs if the API implementation
+    called initiates multiple executions. "Job" here refers to a call of
+    'fair run'.
+
+    Parameters
+    ----------
+    job_dir : str
+        jobs directory
+
+    Returns
+    -------
+    str
+        hash of job
+    """
+    if not os.path.exists(job_dir):
+        raise fdp_exc.FileNotFoundError(
+            "Failed to find hash for job, "
+            f"directory '{job_dir}' does not exist."
+        )
+    _directory = os.path.abspath(job_dir)
+    return hashlib.sha1(_directory.encode("utf-8")).hexdigest()
+
+
+def get_job_dir(job_hash: str) -> str:
+    """Get job directory from a hash
+
+    Parameters
+    ----------
+    job_hash : str
+        hash for a given job
+
+    Returns
+    -------
+    str
+        associated job directory
+    """
+    _jobs = glob.glob(os.path.join(fdp_com.default_jobs_dir(), "*"))
+
+    for job in _jobs:
+        _hash = hashlib.sha1(os.path.abspath(job).encode("utf-8")).hexdigest()
+        if _hash == job_hash:
+            return job
+
+    return ""
```

### Comparing `fair_cli-0.5.2/fair/staging.py` & `fair_cli-0.7.0/fair/staging.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,458 +1,485 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-"""
-Staging
-=======
-
-Manage object staging for pushing to a remote registry from the local registry
-
-Contents
-========
-
-Classes
--------
-
-    Staging - class handles staging of objects ready to be synchronised
-
-"""
-
-__date__ = "2021-07-13"
-
-import logging
-import os
-import typing
-
-import yaml
-
-import fair.common as fdp_com
-import fair.configuration as fdp_conf
-import fair.exceptions as fdp_exc
-import fair.registry.requests as fdp_req
-import fair.run as fdp_run
-
-
-class Stager:
-    """
-    The stager handles staging of jobs and other objects for synchronising
-    between local and remote registries. In a manner similar to git, objects
-    such as jobs can be tracked but not staged, for example if a job is a trial
-    or has issues.
-    """
-
-    _logger = logging.getLogger("FAIRDataPipeline.Staging")
-
-    def __init__(self, repo_root: str) -> None:
-        """Create a new stager instance for a given FAIR repository
-
-        Parameters
-        ----------
-        repo_root : str, optional
-            the root of the FAIR repository, by default find the root from the
-            current working directory
-        """
-        self._root = repo_root
-        self._staging_file = fdp_com.staging_cache(self._root)
-        self._logger.debug(
-            "Creating stager for FAIR repository '%s'", repo_root
-        )
-
-    def initialise(self) -> None:
-        """Initialise the stager, creating a staging cache file if one does not exist"""
-        # Only create the staging file if one is not already present within the
-        # specified directory
-        if not os.path.exists(self._staging_file):
-            self._logger.debug("Creating new staging cache file")
-            # If the stager is called before the rest of the directory tree
-            # has been created make the parent directories first
-            if not os.path.exists(os.path.dirname(self._staging_file)):
-                os.makedirs(os.path.dirname(self._staging_file), exist_ok=True)
-            self._create_staging_file()
-        else:
-            self._logger.debug("Existing staging cache found")
-
-    def _create_file_label(self, file_to_stage: str) -> str:
-        return os.path.relpath(
-            file_to_stage,
-            os.path.dirname(self._staging_file),
-        )
-
-    def _create_staging_file(self) -> None:
-        _staging_dict = {
-            "job": {},
-            "file": {},
-            "data_product": {},
-        }
-        yaml.dump(_staging_dict, open(self._staging_file, "w"))
-
-    def reset_staged(self) -> None:
-        """Change staging state of all items to unstaged"""
-        _staging_dict = yaml.safe_load(open(self._staging_file))
-        for obj_type in _staging_dict:
-            for item in _staging_dict[obj_type]:
-                _staging_dict[obj_type][item] = False
-        yaml.dump(_staging_dict, open(self._staging_file, "w"))
-
-    def add_to_staging(self, identifier: str, item_type: str) -> None:
-        """Add an item to tracking
-
-        Parameters
-        ----------
-        identifier : str
-            unique identifier for the item
-        item_type : str
-            the item type
-        """
-        # Open the staging dictionary first
-        with open(self._staging_file) as f:
-            _staging_dict = yaml.safe_load(f)
-
-        _staging_dict[item_type][identifier] = False
-
-        with open(self._staging_file, "w") as f:
-            yaml.dump(_staging_dict, f)
-
-    def change_stage_status(
-        self,
-        identifier: str,
-        item_type: str,
-        stage: bool = True,
-    ) -> None:
-        self._logger.debug(
-            "Setting %s '%s' status to staged=%s", item_type, identifier, stage
-        )
-
-        if not os.path.exists(self._staging_file):
-            raise fdp_exc.FileNotFoundError(
-                "Failed to update tracking, expected staging file"
-                f" '{self._staging_file}' but it does not exist"
-            )
-
-        # Open the staging dictionary first
-        _staging_dict = yaml.safe_load(open(self._staging_file))
-
-        if identifier not in _staging_dict[item_type]:
-            raise fdp_exc.StagingError(
-                f"Cannot stage '{item_type}' with label '{identifier}', "
-                "item does not exist."
-            )
-
-        _staging_dict[item_type][identifier] = stage
-
-        with open(self._staging_file, "w") as f:
-            yaml.dump(_staging_dict, f)
-
-    def change_data_product_stage_status(
-        self, data_product_id: str, stage: bool = True
-    ) -> None:
-        self.change_stage_status(data_product_id, "data_product", stage)
-
-    def change_job_stage_status(self, job_id: str, stage: bool = True) -> None:
-        """Stage a local code job ready to be pushed to the remote registry
-
-        Parameters
-        ----------
-        job_id : str
-            a valid uuid for the given job
-        stage : bool, optional
-            whether job is staged, default True
-        """
-
-        # When a job is completed by a language implementation the CLI should
-        # have already registered it into staging with a status of staged=False
-        if not fdp_run.get_job_dir(job_id):
-            raise fdp_exc.StagingError(
-                f"Failed to recognise job with ID '{job_id}'"
-            )
-
-        self.add_to_staging(job_id, "job")
-        self.change_stage_status(job_id, "job", stage)
-
-    def find_registry_entry_for_file(
-        self, local_uri: str, file_path: str
-    ) -> str:
-        """Performs a rough search for a file in the local registry
-
-        Parameters
-        ----------
-        file_path : str
-            local file system path
-
-        Returns
-        -------
-        str
-            URL of local registry entry
-        """
-        self._logger.debug(
-            "Retrieving registry entry for file '%s'", file_path
-        )
-
-        # Will search storage locations for a similar path by using
-        # parent_directory/file_name
-        _obj_type = "storage_location"
-
-        _results = fdp_req.get(
-            local_uri, _obj_type, fdp_req.local_token(), {"path": file_path}
-        )
-
-        if not _results:
-            raise fdp_exc.StagingError(
-                "Failed to find local registry entry for file "
-                f"'{file_path}'"
-            )
-
-        if len(_results) > 1:
-            raise fdp_exc.StagingError(
-                "Expected single result for local registry entry relating to "
-                f" file '{file_path} but got {len(_results)}"
-            )
-
-        self._logger.debug("Found config.yaml URL: %s", _results[0])
-
-        return _results[0]
-
-    def _get_code_run_entries(
-        self, local_uri: str, job_dir: str
-    ) -> typing.List[str]:
-        """Retrieve code_run URL list from a given CLI run directory
-
-        Parameters
-        ----------
-        local_uri : str
-            local registry endpoint
-        job_dir : str
-            CLI run directory
-
-        Returns
-        -------
-        typing.List[str]
-
-        Raises
-        ------
-        fdp_exc.ImplementationError
-            If the expected registry entries have not been created by an API
-            implementation
-        """
-        self._logger.debug(
-            "Retrieving code run URL for job '%s'", os.path.basename(job_dir)
-        )
-        # Check if any code_runs are present for the given job
-        _code_run_file = os.path.join(job_dir, "coderuns.txt")
-        _code_run_urls = []
-
-        if (
-            os.path.exists(_code_run_file)
-            and open(_code_run_file).read().strip()
-        ):
-            self._logger.debug("Found coderuns file, extracting runs")
-            _runs = [i.strip() for i in open(_code_run_file).readlines()]
-
-            for run in _runs:
-                _results = fdp_req.get(
-                    local_uri,
-                    "code_run",
-                    fdp_req.local_token(),
-                    params={"uuid": run},
-                )
-
-                if not _results:
-                    raise fdp_exc.ImplementationError(
-                        "Expected code_run with uuid "
-                        f"'{run}' in local registry, but no result found."
-                    )
-
-                _code_run_urls.append(_results[0]["url"])
-
-        return _code_run_urls
-
-    def _get_written_obj_entries(
-        self, local_uri: str, config_dict: typing.Dict
-    ):
-        if "write" not in config_dict:
-            return []
-
-        _data_product_urls: typing.List[str] = []
-
-        for write_obj in config_dict["write"]:
-            _data_product = write_obj["data_product"]
-            _results = fdp_req.get(
-                local_uri,
-                "data_product",
-                fdp_req.local_token(),
-                params={"name": _data_product},
-            )
-
-            if not _results:
-                raise fdp_exc.InternalError(
-                    "Expected data_product "
-                    f"'{_data_product}' in local registry, but no result found."
-                )
-
-            _data_product_urls.append(_results[0]["url"])
-
-        return _data_product_urls
-
-    def get_job_data(
-        self, local_uri, identifier: str
-    ) -> typing.Dict[str, str]:
-        self._logger.debug("Fetching job data for job %s", identifier)
-        # Firstly find the job directory
-        _directory = fdp_run.get_job_dir(identifier)
-        if not _directory:
-            raise fdp_exc.StagingError(
-                f"Could not retrieve directory for job '{identifier}'"
-            )
-
-        # Check for a config.yaml file
-        _config_yaml = os.path.join(_directory, fdp_com.USER_CONFIG_FILE)
-        if not os.path.exists(_config_yaml):
-            raise fdp_exc.FileNotFoundError(
-                f"Cannot stage job '{identifier}' "
-                f"Expected config.yaml in '{_directory}'"
-            )
-
-        # Find this config.yaml on the local registry, this involves
-        # firstly getting the path commencing from the 'jobs' folder
-        _config_rel_path = _config_yaml.split(fdp_com.JOBS_DIR)[1]
-        _config_rel_path = f"{fdp_com.JOBS_DIR}{_config_rel_path}"
-
-        _config_url = self.find_registry_entry_for_file(
-            fdp_conf.get_local_uri(), _config_rel_path
-        )["url"]
-
-        # Check for job script file
-        _config_yaml = os.path.join(_directory, fdp_com.USER_CONFIG_FILE)
-        if not os.path.exists(_config_yaml):
-            raise fdp_exc.FileNotFoundError(
-                f"Cannot stage job '{identifier}' "
-                f"Expected config.yaml in '{_directory}'"
-            )
-
-        # Find this job script on the local registry, as the script
-        # can have any name obtain this information from the config.yaml
-        _config_dict = yaml.safe_load(open(_config_yaml))
-
-        if (
-            "run_metadata" not in _config_dict
-            or "script_path" not in _config_dict["run_metadata"]
-        ):
-            _script_url = None
-        else:
-
-            _script_url = self._extracted_from_get_job_data_50(
-                _config_dict, local_uri
-            )
-        self._logger.debug("Retrieving code runs and written objects")
-
-        _code_run_urls = self._get_code_run_entries(local_uri, _directory)
-        _user_written_obj_urls = self._get_written_obj_entries(
-            local_uri, _config_dict
-        )
-
-        return {
-            "jobs": _code_run_urls,
-            "user_written_objects": _user_written_obj_urls,
-            "config_file": _config_url,
-            "script_file": _script_url,
-        }
-
-    # TODO Rename this here and in `get_job_data`
-    def _extracted_from_get_job_data_50(self, _config_dict, local_uri):
-        # Find the relevant script path on the local registry, this involves
-        # firstly getting the path commencing from the 'jobs' folder
-        self._logger.debug("Finding job script within local registry")
-        _script_path = _config_dict["run_metadata"]["script_path"]
-        _rel_script_path = _script_path.split(fdp_com.JOBS_DIR)[1]
-        _rel_script_path = f"{fdp_com.JOBS_DIR}{_rel_script_path}"
-
-        result = self.find_registry_entry_for_file(
-            local_uri, _rel_script_path
-        )["url"]
-
-        self._logger.debug("Script URL: %s", result)
-
-        return result
-
-    def remove_staging_entry(
-        self, identifier: str, stage_type: str = "job"
-    ) -> None:
-        """Remove an item of type 'stage_type' from staging
-
-        Parameters
-        ----------
-            identifier : str
-                name or ID of item
-            stage_type: str, optional
-                type of stage item either job (default) or file
-        """
-        # Open the staging dictionary first
-        _staging_dict = yaml.safe_load(open(self._staging_file))
-
-        if stage_type not in _staging_dict:
-            raise fdp_exc.StagingError(
-                f"Cannot remove staging item of unrecognised type '{stage_type}'"
-            )
-
-        if identifier not in _staging_dict[stage_type]:
-            raise fdp_exc.StagingError(
-                f"Cannot remove item '{identifier}' of stage type '{stage_type}', "
-                "item is not in staging."
-            )
-
-        del _staging_dict[stage_type][identifier]
-
-        with open(self._staging_file, "w") as f:
-            yaml.dump(_staging_dict, f)
-
-    def get_item_list(
-        self, staged: bool = True, stage_type: str = "job"
-    ) -> typing.List[str]:
-        """Returns a list of items of type 'stage_type' which are staged/unstaged
-
-        Parameters
-        ----------
-            staged : bool
-                list staged/unstaged items
-            stage_type : str, optional
-                type of stage item either job (default) or file
-        """
-        _staging_dict = yaml.safe_load(open(self._staging_file))
-
-        if stage_type not in _staging_dict:
-            raise fdp_exc.StagingError(
-                f"Cannot remove staging item of unrecognised type '{stage_type}'"
-            )
-
-        return [k for k, v in _staging_dict[stage_type].items() if v == staged]
-
-    def update_data_product_staging(self) -> None:
-        """Update DataProduct list in staging file."""
-        with open(self._staging_file) as f:
-            _staging_dict = yaml.safe_load(f)
-
-        result = fdp_req.url_get(
-            f"{fdp_com.DEFAULT_LOCAL_REGISTRY_URL}data_product",
-            fdp_req.local_token(),
-        )
-
-        for data_product in result:
-            namespace = fdp_req.url_get(
-                data_product["namespace"], fdp_req.local_token()
-            )["name"]
-            name = data_product["name"]
-            version = data_product["version"]
-            key = f"{namespace}:{name}@v{version}"
-            if key not in _staging_dict["data_product"]:
-                _staging_dict["data_product"][key] = False
-
-        with open(self._staging_file, "w") as f:
-            yaml.dump(_staging_dict, f)
-
-    def _load_from_file(self, file_name: str = None) -> typing.Dict[str, bool]:
-        if not file_name:
-            file_name = self._staging_file
-
-        with open(file_name, "w") as f:
-            _staging_dict = yaml.safe_load(f)
-
-        self._staging_file = file_name
-        return _staging_dict
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+"""
+Staging
+=======
+
+Manage object staging for pushing to a remote registry from the local registry
+
+Contents
+========
+
+Classes
+-------
+
+    Staging - class handles staging of objects ready to be synchronised
+
+"""
+
+__date__ = "2021-07-13"
+
+import logging
+import os
+import typing
+import re
+
+import yaml
+
+import fair.common as fdp_com
+import fair.configuration as fdp_conf
+import fair.exceptions as fdp_exc
+import fair.registry.requests as fdp_req
+import fair.run as fdp_run
+
+
+class Stager:
+    """
+    The stager handles staging of jobs and other objects for synchronising
+    between local and remote registries. In a manner similar to git, objects
+    such as jobs can be tracked but not staged, for example if a job is a trial
+    or has issues.
+    """
+
+    _logger = logging.getLogger("FAIRDataPipeline.Staging")
+
+    def __init__(self, repo_root: str) -> None:
+        """Create a new stager instance for a given FAIR repository
+
+        Parameters
+        ----------
+        repo_root : str, optional
+            the root of the FAIR repository, by default find the root from the
+            current working directory
+        """
+        self._root = repo_root
+        self._staging_file = fdp_com.staging_cache(self._root)
+        self._logger.debug(
+            "Creating stager for FAIR repository '%s'", repo_root
+        )
+
+    def initialise(self) -> None:
+        """Initialise the stager, creating a staging cache file if one does not exist"""
+        # Only create the staging file if one is not already present within the
+        # specified directory
+        if not os.path.exists(self._staging_file):
+            self._logger.debug("Creating new staging cache file")
+            # If the stager is called before the rest of the directory tree
+            # has been created make the parent directories first
+            if not os.path.exists(os.path.dirname(self._staging_file)):
+                os.makedirs(os.path.dirname(self._staging_file), exist_ok=True)
+            self._create_staging_file()
+        else:
+            self._logger.debug("Existing staging cache found")
+
+    def _create_file_label(self, file_to_stage: str) -> str:
+        return os.path.relpath(
+            file_to_stage,
+            os.path.dirname(self._staging_file),
+        )
+
+    def _create_staging_file(self) -> None:
+        _staging_dict = {
+            "job": {},
+            "file": {},
+            "data_product": {},
+            "code_run": {},
+        }
+        yaml.dump(_staging_dict, open(self._staging_file, "w"))
+
+    def reset_staged(self) -> None:
+        """Change staging state of all items to unstaged"""
+        _staging_dict = yaml.safe_load(open(self._staging_file))
+        for obj_type in _staging_dict:
+            for item in _staging_dict[obj_type]:
+                _staging_dict[obj_type][item] = False
+        yaml.dump(_staging_dict, open(self._staging_file, "w"))        
+
+    def add_to_staging(self, identifier: str, item_type: str) -> None:
+        """Add an item to tracking
+
+        Parameters
+        ----------
+        identifier : str
+            unique identifier for the item
+        item_type : str
+            the item type
+        """
+        # Open the staging dictionary first
+        with open(self._staging_file) as f:
+            _staging_dict = yaml.safe_load(f)
+
+        _staging_dict[item_type][identifier] = False
+
+        with open(self._staging_file, "w") as f:
+            yaml.dump(_staging_dict, f)
+
+    def change_stage_status(
+        self,
+        identifier: str,
+        item_type: str,
+        stage: bool = True,
+    ) -> None:
+        self._logger.debug(
+            "Setting %s '%s' status to staged=%s", item_type, identifier, stage
+        )
+
+        if not os.path.exists(self._staging_file):
+            raise fdp_exc.FileNotFoundError(
+                "Failed to update tracking, expected staging file"
+                f" '{self._staging_file}' but it does not exist"
+            )
+      
+        if not self.is_in_staging_dict(identifier, item_type):
+            raise fdp_exc.StagingError(
+                f"Cannot stage '{item_type}' with label '{identifier}', "
+                "item does not exist."
+            )
+        
+        # Open the staging dictionary first
+        _staging_dict = yaml.safe_load(open(self._staging_file))
+        _staging_dict[item_type][identifier] = stage
+
+        with open(self._staging_file, "w") as f:
+            yaml.dump(_staging_dict, f)
+
+    def is_in_staging_dict(self, identifier, item_type):
+        # Open the staging dictionary first
+        _staging_dict = yaml.safe_load(open(self._staging_file))
+
+        if identifier in _staging_dict[item_type]:
+            return True
+        return False
+
+    def change_data_product_stage_status(
+        self, data_product_id: str, stage: bool = True
+    ) -> None:
+        self.change_stage_status(data_product_id, "data_product", stage)
+
+    def change_job_stage_status(self, job_id: str, stage: bool = True) -> None:
+        """Stage a local code job ready to be pushed to the remote registry
+
+        Parameters
+        ----------
+        job_id : str
+            a valid uuid for the given job
+        stage : bool, optional
+            whether job is staged, default True
+        """
+
+        # When a job is completed by a language implementation the CLI should
+        # have already registered it into staging with a status of staged=False
+        if not fdp_run.get_job_dir(job_id):
+            raise fdp_exc.StagingError(
+                f"Failed to recognise job with ID '{job_id}'"
+            )
+
+        self.add_to_staging(job_id, "job")
+        self.change_stage_status(job_id, "job", stage)
+
+    def find_registry_entry_for_file(
+        self, local_uri: str, file_path: str
+    ) -> str:
+        """Performs a rough search for a file in the local registry
+
+        Parameters
+        ----------
+        file_path : str
+            local file system path
+
+        Returns
+        -------
+        str
+            URL of local registry entry
+        """
+        self._logger.debug(
+            "Retrieving registry entry for file '%s'", file_path
+        )
+
+        # Will search storage locations for a similar path by using
+        # parent_directory/file_name
+        _obj_type = "storage_location"
+
+        _results = fdp_req.get(
+            local_uri, _obj_type, fdp_req.local_token(), {"path": file_path}
+        )
+
+        if not _results:
+            raise fdp_exc.StagingError(
+                "Failed to find local registry entry for file "
+                f"'{file_path}'"
+            )
+
+        if len(_results) > 1:
+            raise fdp_exc.StagingError(
+                "Expected single result for local registry entry relating to "
+                f" file '{file_path} but got {len(_results)}"
+            )
+
+        self._logger.debug("Found config.yaml URL: %s", _results[0])
+
+        return _results[0]
+
+    def _get_code_run_entries(
+        self, local_uri: str, job_dir: str
+    ) -> typing.List[str]:
+        """Retrieve code_run URL list from a given CLI run directory
+
+        Parameters
+        ----------
+        local_uri : str
+            local registry endpoint
+        job_dir : str
+            CLI run directory
+
+        Returns
+        -------
+        typing.List[str]
+
+        Raises
+        ------
+        fdp_exc.ImplementationError
+            If the expected registry entries have not been created by an API
+            implementation
+        """
+        self._logger.debug(
+            "Retrieving code run URL for job '%s'", os.path.basename(job_dir)
+        )
+        # Check if any code_runs are present for the given job
+        _code_run_file = os.path.join(job_dir, "coderuns.txt")
+        _code_run_urls = []
+
+        if (
+            os.path.exists(_code_run_file)
+            and open(_code_run_file).read().strip()
+        ):
+            self._logger.debug("Found coderuns file, extracting runs")
+            _runs = [i.strip() for i in open(_code_run_file).readlines()]
+
+            for run in _runs:
+                _results = fdp_req.get(
+                    local_uri,
+                    "code_run",
+                    fdp_req.local_token(),
+                    params={"uuid": run},
+                )
+
+                if not _results:
+                    raise fdp_exc.ImplementationError(
+                        "Expected code_run with uuid "
+                        f"'{run}' in local registry, but no result found."
+                    )
+
+                _code_run_urls.append(_results[0]["url"])
+
+        return _code_run_urls
+
+    def _get_written_obj_entries(
+        self, local_uri: str, config_dict: typing.Dict
+    ):
+        if "write" not in config_dict:
+            return []
+
+        _data_product_urls: typing.List[str] = []
+
+        for write_obj in config_dict["write"]:
+            _data_product = write_obj["data_product"]
+            _results = fdp_req.get(
+                local_uri,
+                "data_product",
+                fdp_req.local_token(),
+                params={"name": _data_product},
+            )
+
+            if not _results:
+                raise fdp_exc.InternalError(
+                    "Expected data_product "
+                    f"'{_data_product}' in local registry, but no result found."
+                )
+
+            _data_product_urls.append(_results[0]["url"])
+
+        return _data_product_urls
+
+    def get_job_data(
+        self, local_uri, identifier: str
+    ) -> typing.Dict[str, str]:
+        self._logger.debug("Fetching job data for job %s", identifier)
+        # Firstly find the job directory
+        _directory = fdp_run.get_job_dir(identifier)
+        if not _directory:
+            raise fdp_exc.StagingError(
+                f"Could not retrieve directory for job '{identifier}'"
+            )
+
+        # Check for a config.yaml file
+        _config_yaml = os.path.join(_directory, fdp_com.USER_CONFIG_FILE)
+        if not os.path.exists(_config_yaml):
+            raise fdp_exc.FileNotFoundError(
+                f"Cannot stage job '{identifier}' "
+                f"Expected config.yaml in '{_directory}'"
+            )
+
+        # Find this config.yaml on the local registry, this involves
+        # firstly getting the path commencing from the 'jobs' folder
+        _config_rel_path = _config_yaml.split(fdp_com.JOBS_DIR)[1]
+        _config_rel_path = f"{fdp_com.JOBS_DIR}{_config_rel_path}"
+
+        _config_url = self.find_registry_entry_for_file(
+            fdp_conf.get_local_uri(), _config_rel_path
+        )["url"]
+
+        # Check for job script file
+        _config_yaml = os.path.join(_directory, fdp_com.USER_CONFIG_FILE)
+        if not os.path.exists(_config_yaml):
+            raise fdp_exc.FileNotFoundError(
+                f"Cannot stage job '{identifier}' "
+                f"Expected config.yaml in '{_directory}'"
+            )
+
+        # Find this job script on the local registry, as the script
+        # can have any name obtain this information from the config.yaml
+        _config_dict = yaml.safe_load(open(_config_yaml))
+
+        if (
+            "run_metadata" not in _config_dict
+            or "script_path" not in _config_dict["run_metadata"]
+        ):
+            _script_url = None
+        else:
+
+            _script_url = self._extracted_from_get_job_data_50(
+                _config_dict, local_uri
+            )
+        self._logger.debug("Retrieving code runs and written objects")
+
+        _code_run_urls = self._get_code_run_entries(local_uri, _directory)
+        _user_written_obj_urls = self._get_written_obj_entries(
+            local_uri, _config_dict
+        )
+
+        return {
+            "jobs": _code_run_urls,
+            "user_written_objects": _user_written_obj_urls,
+            "config_file": _config_url,
+            "script_file": _script_url,
+        }
+
+    # TODO Rename this here and in `get_job_data`
+    def _extracted_from_get_job_data_50(self, _config_dict, local_uri):
+        # Find the relevant script path on the local registry, this involves
+        # firstly getting the path commencing from the 'jobs' folder
+        self._logger.debug("Finding job script within local registry")
+        _script_path = _config_dict["run_metadata"]["script_path"]
+        _rel_script_path = _script_path.split(fdp_com.JOBS_DIR)[1]
+        _rel_script_path = f"{fdp_com.JOBS_DIR}{_rel_script_path}"
+
+        result = self.find_registry_entry_for_file(
+            local_uri, _rel_script_path
+        )["url"]
+
+        self._logger.debug("Script URL: %s", result)
+
+        return result
+
+    def remove_staging_entry(
+        self, identifier: str, stage_type: str = "job"
+    ) -> None:
+        """Remove an item of type 'stage_type' from staging
+
+        Parameters
+        ----------
+            identifier : str
+                name or ID of item
+            stage_type: str, optional
+                type of stage item either job (default) or file
+        """
+        # Open the staging dictionary first
+        _staging_dict = yaml.safe_load(open(self._staging_file))
+
+        if stage_type not in _staging_dict:
+            raise fdp_exc.StagingError(
+                f"Cannot remove staging item of unrecognised type '{stage_type}'"
+            )
+
+        if identifier not in _staging_dict[stage_type]:
+            raise fdp_exc.StagingError(
+                f"Cannot remove item '{identifier}' of stage type '{stage_type}', "
+                "item is not in staging."
+            )
+
+        del _staging_dict[stage_type][identifier]
+
+        with open(self._staging_file, "w") as f:
+            yaml.dump(_staging_dict, f)
+
+    def get_item_list(
+        self, staged: bool = True, stage_type: str = "job"
+    ) -> typing.List[str]:
+        """Returns a list of items of type 'stage_type' which are staged/unstaged
+
+        Parameters
+        ----------
+            staged : bool
+                list staged/unstaged items
+            stage_type : str, optional
+                type of stage item either job (default) or file
+        """
+        _staging_dict = yaml.safe_load(open(self._staging_file))
+
+        if stage_type not in _staging_dict:
+            raise fdp_exc.StagingError(
+                f"Cannot remove staging item of unrecognised type '{stage_type}'"
+            )
+
+        return [k for k, v in _staging_dict[stage_type].items() if v == staged]
+
+    def update_data_product_staging(self) -> None:
+        """Update DataProduct list in staging file."""
+        with open(self._staging_file) as f:
+            _staging_dict = yaml.safe_load(f)
+
+        result = fdp_req.url_get(
+            f"{fdp_com.DEFAULT_LOCAL_REGISTRY_URL}data_product",
+            fdp_req.local_token(),
+        )
+
+        for data_product in result:
+            namespace = fdp_req.url_get(
+                data_product["namespace"], fdp_req.local_token()
+            )["name"]
+            name = data_product["name"]
+            version = data_product["version"]
+            key = f"{namespace}:{name}@v{version}"
+            if key not in _staging_dict["data_product"]:
+                _staging_dict["data_product"][key] = False
+
+        with open(self._staging_file, "w") as f:
+            yaml.dump(_staging_dict, f)
+
+    def update_code_run_staging(self) -> None:
+        """Update code_run(s) list in staging file."""
+        with open(self._staging_file) as f:
+            _staging_dict = yaml.safe_load(f)
+
+        result = fdp_req.url_get(
+            f"{fdp_com.DEFAULT_LOCAL_REGISTRY_URL}code_run",
+            fdp_req.local_token(),
+        )
+
+        for code_run in result:
+            key = code_run["uuid"]
+            if key not in _staging_dict["code_run"]:
+                _staging_dict["code_run"][key] = False
+
+        with open(self._staging_file, "w") as f:
+            yaml.dump(_staging_dict, f)
+
+    def _load_from_file(self, file_name: str = None) -> typing.Dict[str, bool]:
+        if not file_name:
+            file_name = self._staging_file
+
+        with open(file_name, "w") as f:
+            _staging_dict = yaml.safe_load(f)
+
+        self._staging_file = file_name
+        return _staging_dict
```

### Comparing `fair_cli-0.5.2/fair/testing.py` & `fair_cli-0.7.0/fair/testing.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-import os
-import pathlib
-import tempfile
-import typing
-
-import git
-
-import fair.common as fdp_com
-import fair.identifiers as fdp_id
-
-
-def create_configurations(
-    registry_dir: str,
-    local_git_dir: typing.Optional[str] = None,
-    remote_reg_dir: typing.Optional[str] = None,
-    testing_dir: str = tempfile.mkdtemp(),
-    tokenless: bool = False,
-) -> typing.Dict:
-    """
-    Setup CLI for testing
-
-    Running without a token limits the functionality, this should only be used
-    when testing without need to access a local registry.
-
-    Parameters
-    ----------
-    registry_dir : str
-        directory of the local registry
-    testing_dir : str
-        working directory for the test
-    tokenless : optional, bool
-        create a fake token, default False
-
-    Returns
-    -------
-    typing.Dict
-        A CLI configuration dictionary that can be loaded for a the CLI session
-    """
-    if not registry_dir:
-        if "FAIR_REGISTRY_DIR" in os.environ:
-            registry_dir = os.environ["FAIR_REGISTRY_DIR"]
-        else:
-            registry_dir = fdp_com.DEFAULT_REGISTRY_LOCATION
-    if not remote_reg_dir:
-        remote_reg_dir = os.path.join(
-            os.path.dirname(fdp_com.DEFAULT_REGISTRY_LOCATION), "registry-rem"
-        )
-
-    _loc_data_store = os.path.join(testing_dir, "data_store") + os.path.sep
-    _proj_dir = os.path.join(testing_dir, "project")
-
-    if tokenless:
-        _token = "t35tt0k3n"
-        _token_file = os.path.join(registry_dir, "token.txt")
-        with open(_token_file, "w") as out_f:
-            out_f.write(_token)
-
-    if not local_git_dir:
-        local_git_dir = _no_git_setup(_proj_dir)
-    os.makedirs(_loc_data_store, exist_ok=True)
-    _local_uri = "http://127.0.0.1:8000/api/"
-    _origin_uri = "http://127.0.0.1:8001/api/"
-    return {
-        "namespaces": {"input": "testing", "output": "testing"},
-        "registries": {
-            "local": {
-                "data_store": _loc_data_store,
-                "directory": registry_dir,
-                "token": os.path.join(registry_dir, "token"),
-                "uri": _local_uri,
-            },
-            "origin": {
-                "data_store": os.path.join(remote_reg_dir, "data"),
-                "token": os.path.join(remote_reg_dir, "token"),
-                "uri": _origin_uri,
-            },
-        },
-        "user": {
-            "email": "test@noreply.com",
-            "family_name": "Test",
-            "given_names": "Interface",
-            "orcid": "000-0000-0000-0000",
-            "uri": f'{fdp_id.ID_URIS["orcid"]}000-0000-0000-0000',
-            "uuid": "2ddb2358-84bf-43ff-b2aa-3ac7dc3b49f1",
-        },
-        "git": {
-            "local_repo": local_git_dir,
-            "remote": "origin",
-            "remote_repo": "git@notagit.com/user/project.git",
-        },
-    }
-
-
-def _no_git_setup(_proj_dir):
-    _repo = git.Repo.init(_proj_dir)
-    _repo.create_remote("origin", url="git@notagit.com/nope")
-    result = _proj_dir
-    _demo_file = os.path.join(_proj_dir, "first_file")
-    pathlib.Path(_demo_file).touch()
-    _repo.index.add(_demo_file)
-    _repo.index.commit("First commit of test repository")
-
-    return result
+import os
+import pathlib
+import tempfile
+import typing
+
+import git
+
+import fair.common as fdp_com
+import fair.identifiers as fdp_id
+
+
+def create_configurations(
+    registry_dir: str,
+    local_git_dir: typing.Optional[str] = None,
+    remote_reg_dir: typing.Optional[str] = None,
+    testing_dir: str = tempfile.mkdtemp(),
+    tokenless: bool = False,
+) -> typing.Dict:
+    """
+    Setup CLI for testing
+
+    Running without a token limits the functionality, this should only be used
+    when testing without need to access a local registry.
+
+    Parameters
+    ----------
+    registry_dir : str
+        directory of the local registry
+    testing_dir : str
+        working directory for the test
+    tokenless : optional, bool
+        create a fake token, default False
+
+    Returns
+    -------
+    typing.Dict
+        A CLI configuration dictionary that can be loaded for a the CLI session
+    """
+    if not registry_dir:
+        if "FAIR_REGISTRY_DIR" in os.environ:
+            registry_dir = os.environ["FAIR_REGISTRY_DIR"]
+        else:
+            registry_dir = fdp_com.DEFAULT_REGISTRY_LOCATION
+    if not remote_reg_dir:
+        remote_reg_dir = os.path.join(
+            os.path.dirname(fdp_com.DEFAULT_REGISTRY_LOCATION), "registry-rem"
+        )
+
+    _loc_data_store = os.path.join(testing_dir, "data_store") + os.path.sep
+    _proj_dir = os.path.join(testing_dir, "project")
+
+    if tokenless:
+        _token = "t35tt0k3n"
+        _token_file = os.path.join(registry_dir, "token.txt")
+        with open(_token_file, "w") as out_f:
+            out_f.write(_token)
+
+    if not local_git_dir:
+        local_git_dir = _no_git_setup(_proj_dir)
+    os.makedirs(_loc_data_store, exist_ok=True)
+    _local_uri = "http://127.0.0.1:8000/api/"
+    _origin_uri = "http://127.0.0.1:8001/api/"
+    return {
+        "namespaces": {"input": "testing", "output": "testing"},
+        "registries": {
+            "local": {
+                "data_store": _loc_data_store,
+                "directory": registry_dir,
+                "token": os.path.join(registry_dir, "token"),
+                "uri": _local_uri,
+            },
+            "origin": {
+                "data_store": os.path.join(remote_reg_dir, "data"),
+                "token": os.path.join(remote_reg_dir, "token"),
+                "uri": _origin_uri,
+            },
+        },
+        "user": {
+            "email": "test@noreply.com",
+            "family_name": "Test",
+            "given_names": "Interface",
+            "orcid": "000-0000-0000-0000",
+            "uri": f'{fdp_id.ID_URIS["orcid"]}000-0000-0000-0000',
+            "uuid": "2ddb2358-84bf-43ff-b2aa-3ac7dc3b49f1",
+        },
+        "git": {
+            "local_repo": local_git_dir,
+            "remote": "origin",
+            "remote_repo": "git@notagit.com/user/project.git",
+        },
+    }
+
+
+def _no_git_setup(_proj_dir):
+    _repo = git.Repo.init(_proj_dir)
+    _repo.create_remote("origin", url="git@notagit.com/nope")
+    result = _proj_dir
+    _demo_file = os.path.join(_proj_dir, "first_file")
+    pathlib.Path(_demo_file).touch()
+    _repo.index.add(_demo_file)
+    _repo.index.commit("First commit of test repository")
+
+    return result
```

### Comparing `fair_cli-0.5.2/fair/user_config/globbing.py` & `fair_cli-0.7.0/fair/user_config/globbing.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-"""
-User Config Remote Globbing
-===========================
-
-Handles the inclusion of wildcards in configuration statements by speaking to
-the local registry and extracting items.
-
-
-Constants
----------
-
-    - DISPOSABLES: tuple of keys to be removed before adding to config.yaml
-
-"""
-import typing
-
-import fair.exceptions as fdp_exc
-import fair.registry.requests as fdp_req
-from fair.registry import SEARCH_KEYS
-
-__date__ = "2022-01-11"
-
-
-DISPOSABLES = (
-    "name",
-    "object",
-    "last_updated",
-    "namespace",
-    "release_date",
-    "updated_by",
-    "original_store",
-    "prov_report",
-    "external_object",
-    "internal_format",
-    "url",
-)
-
-
-def get_single_layer_objects(
-    results_list: typing.List[typing.Dict], object_type: str
-) -> typing.List[typing.Dict]:
-    """
-    Retrieve results for a wildcard search for the given object
-
-    This object should not have any requirements (other registry URLs)
-
-    Parameters
-    ----------
-    results_list : typing.List[typing.Dict]
-        results of registry search for the wildcard
-
-    Returns
-    -------
-    typing.List[typing.Dict]
-        entries for the config.yaml file
-    """
-    _new_entries: typing.List[typing.Dict] = []
-
-    for result in results_list:
-        _data = result.copy()
-        for key, value in result.items():
-            if not value:
-                _data.pop(key, None)
-        _data[object_type] = _data["name"]
-
-        for key in DISPOSABLES:
-            _data.pop(key, None)
-
-        _new_entries.append(_data)
-    return _new_entries
-
-
-def get_data_product_objects(
-    registry_token: str,
-    results_list: typing.List[typing.Dict],
-    block_type: str,
-    version: str = None,
-) -> typing.List[typing.Dict]:
-    """
-    Retrieve results for a wildcard search of a data_product
-
-    Parameters
-    ----------
-    results_list : typing.List[typing.Dict]
-        results of registry search for the wildcard
-
-    Returns
-    -------
-    typing.List[typing.Dict]
-        entries for the config.yaml file
-    """
-    _new_entries: typing.List[typing.Dict] = []
-
-    # If a data product need to retrieve the namespace name
-    for entry in results_list:
-        _data = entry.copy()
-
-        for key, value in entry.items():
-            if not value:
-                _data.pop(key, None)
-
-        _namespace = fdp_req.url_get(entry["namespace"], registry_token)
-
-        if not _namespace:
-            raise fdp_exc.InternalError(
-                "Failed to retrieve namespace for external_object "
-                f"{entry[SEARCH_KEYS['data_product']]}"
-            )
-
-        _version = entry["version"]
-
-        if block_type == "write" and version:
-            _version = version
-
-        _data["use"] = {}
-        _data["use"]["namespace"] = _namespace["name"]
-        _data["data_product"] = _data["name"]
-        _data["use"]["data_product"] = _data["name"]
-        _data["use"]["version"] = _version
-
-        for key in DISPOSABLES:
-            _data.pop(key, None)
-
-        _new_entries.append(_data)
-
-    return _new_entries
-
-
-def get_external_objects(
-    registry_token: str,
-    results_list: typing.List[typing.Dict],
-    block_type: str,
-    version: str = None,
-) -> typing.List[typing.Dict]:
-    """
-    Retrieve results for a wildcard search of a external_object
-
-    Parameters
-    ----------
-    results_list : typing.List[typing.Dict]
-        results of registry search for the wildcard
-
-    Returns
-    -------
-    typing.List[typing.Dict]
-        entries for the config.yaml file
-    """
-    _new_entries: typing.List[typing.Dict] = []
-
-    for result in results_list:
-        _data = result.copy()
-
-        for key, value in result.items():
-            if not value:
-                _data.pop(key, None)
-
-        _data_product = fdp_req.url_get(result["data_product"], registry_token)
-
-        if not _data_product:
-            raise fdp_exc.InternalError(
-                "Failed to retrieve data_product for external_object "
-                f"{result[SEARCH_KEYS['data_product']]}"
-            )
-
-        _namespace = fdp_req.url_get(
-            _data_product["namespace"], fdp_req.local_token()
-        )
-
-        if not _namespace:
-            raise fdp_exc.InternalError(
-                "Failed to retrieve namespace for external_object "
-                f"{result[SEARCH_KEYS['data_product']]}"
-            )
-
-        _version = result["version"]
-
-        if block_type == "write" and version:
-            _version = version
-
-        _data["use"] = {}
-        _data["use"]["namespace"] = (_namespace["name"],)
-        _data["use"]["version"] = _version
-        _data.pop("name", None)
-        _data.pop("last_updated", None)
-
-        for key in DISPOSABLES:
-            _data.pop(key, None)
-
-        _new_entries.append(_data)
-
-    return _new_entries
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+"""
+User Config Remote Globbing
+===========================
+
+Handles the inclusion of wildcards in configuration statements by speaking to
+the local registry and extracting items.
+
+
+Constants
+---------
+
+    - DISPOSABLES: tuple of keys to be removed before adding to config.yaml
+
+"""
+import typing
+
+import fair.exceptions as fdp_exc
+import fair.registry.requests as fdp_req
+from fair.registry import SEARCH_KEYS
+
+__date__ = "2022-01-11"
+
+
+DISPOSABLES = (
+    "name",
+    "object",
+    "last_updated",
+    "namespace",
+    "release_date",
+    "updated_by",
+    "original_store",
+    "prov_report",
+    "external_object",
+    "internal_format",
+    "url",
+)
+
+
+def get_single_layer_objects(
+    results_list: typing.List[typing.Dict], object_type: str
+) -> typing.List[typing.Dict]:
+    """
+    Retrieve results for a wildcard search for the given object
+
+    This object should not have any requirements (other registry URLs)
+
+    Parameters
+    ----------
+    results_list : typing.List[typing.Dict]
+        results of registry search for the wildcard
+
+    Returns
+    -------
+    typing.List[typing.Dict]
+        entries for the config.yaml file
+    """
+    _new_entries: typing.List[typing.Dict] = []
+
+    for result in results_list:
+        _data = result.copy()
+        for key, value in result.items():
+            if not value:
+                _data.pop(key, None)
+        _data[object_type] = _data["name"]
+
+        for key in DISPOSABLES:
+            _data.pop(key, None)
+
+        _new_entries.append(_data)
+    return _new_entries
+
+
+def get_data_product_objects(
+    registry_token: str,
+    results_list: typing.List[typing.Dict],
+    block_type: str,
+    version: str = None,
+) -> typing.List[typing.Dict]:
+    """
+    Retrieve results for a wildcard search of a data_product
+
+    Parameters
+    ----------
+    results_list : typing.List[typing.Dict]
+        results of registry search for the wildcard
+
+    Returns
+    -------
+    typing.List[typing.Dict]
+        entries for the config.yaml file
+    """
+    _new_entries: typing.List[typing.Dict] = []
+
+    # If a data product need to retrieve the namespace name
+    for entry in results_list:
+        _data = entry.copy()
+
+        for key, value in entry.items():
+            if not value:
+                _data.pop(key, None)
+
+        _namespace = fdp_req.url_get(entry["namespace"], registry_token)
+
+        if not _namespace:
+            raise fdp_exc.InternalError(
+                "Failed to retrieve namespace for external_object "
+                f"{entry[SEARCH_KEYS['data_product']]}"
+            )
+
+        _version = entry["version"]
+
+        if block_type == "write" and version:
+            _version = version
+
+        _data["use"] = {}
+        _data["use"]["namespace"] = _namespace["name"]
+        _data["data_product"] = _data["name"]
+        _data["use"]["data_product"] = _data["name"]
+        _data["use"]["version"] = _version
+
+        for key in DISPOSABLES:
+            _data.pop(key, None)
+
+        _new_entries.append(_data)
+
+    return _new_entries
+
+
+def get_external_objects(
+    registry_token: str,
+    results_list: typing.List[typing.Dict],
+    block_type: str,
+    version: str = None,
+) -> typing.List[typing.Dict]:
+    """
+    Retrieve results for a wildcard search of a external_object
+
+    Parameters
+    ----------
+    results_list : typing.List[typing.Dict]
+        results of registry search for the wildcard
+
+    Returns
+    -------
+    typing.List[typing.Dict]
+        entries for the config.yaml file
+    """
+    _new_entries: typing.List[typing.Dict] = []
+
+    for result in results_list:
+        _data = result.copy()
+
+        for key, value in result.items():
+            if not value:
+                _data.pop(key, None)
+
+        _data_product = fdp_req.url_get(result["data_product"], registry_token)
+
+        if not _data_product:
+            raise fdp_exc.InternalError(
+                "Failed to retrieve data_product for external_object "
+                f"{result[SEARCH_KEYS['data_product']]}"
+            )
+
+        _namespace = fdp_req.url_get(
+            _data_product["namespace"], fdp_req.local_token()
+        )
+
+        if not _namespace:
+            raise fdp_exc.InternalError(
+                "Failed to retrieve namespace for external_object "
+                f"{result[SEARCH_KEYS['data_product']]}"
+            )
+
+        _version = result["version"]
+
+        if block_type == "write" and version:
+            _version = version
+
+        _data["use"] = {}
+        _data["use"]["namespace"] = (_namespace["name"],)
+        _data["use"]["version"] = _version
+        _data.pop("name", None)
+        _data.pop("last_updated", None)
+
+        for key in DISPOSABLES:
+            _data.pop(key, None)
+
+        _new_entries.append(_data)
+
+    return _new_entries
```

### Comparing `fair_cli-0.5.2/fair/virtualenv.py` & `fair_cli-0.7.0/fair/virtualenv.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-"""
-Virtual Environment for Registries
-----------------------------------
-
-It was discovered that if building a FAIR-CLI binary "venv" would assume it
-had been called by "python" and not "fair" which would break the setting up
-of a virtual environment when installing a registry. As such a modified version
-of the class which sets the Python executable manually is required.
-
-"""
-
-__date__ = "2022-01-05"
-
-import logging
-import os
-import shutil
-import sys
-from types import SimpleNamespace
-from venv import EnvBuilder
-
-
-class PythonExecutableIdentificationError(Exception):
-    def __init__(self):
-        super().__init__("Failed to identify python executable")
-
-
-class FAIREnv(EnvBuilder):
-    _logger = logging.getLogger("FAIRDataPipeline.VirtualEnv")
-
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-
-    def ensure_directories(self, env_dir) -> SimpleNamespace:
-        self._logger.debug(f"Creating virtual environment in '{env_dir}'")
-        _context: SimpleNamespace = super().ensure_directories(env_dir)
-        _python_exe = sys.executable
-        if not _python_exe:
-            raise PythonExecutableIdentificationError
-
-        self._logger.debug(f"Using python '{_python_exe}' for setup")
-
-        _context.executable = _python_exe
-        _dirname, _exename = os.path.split(os.path.abspath(_python_exe))
-        _context.python_dir = _dirname
-        _context.python_exe = _exename
-        return _context
+"""
+Virtual Environment for Registries
+----------------------------------
+
+It was discovered that if building a FAIR-CLI binary "venv" would assume it
+had been called by "python" and not "fair" which would break the setting up
+of a virtual environment when installing a registry. As such a modified version
+of the class which sets the Python executable manually is required.
+
+"""
+
+__date__ = "2022-01-05"
+
+import logging
+import os
+import shutil
+import sys
+from types import SimpleNamespace
+from venv import EnvBuilder
+
+
+class PythonExecutableIdentificationError(Exception):
+    def __init__(self):
+        super().__init__("Failed to identify python executable")
+
+
+class FAIREnv(EnvBuilder):
+    _logger = logging.getLogger("FAIRDataPipeline.VirtualEnv")
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+    def ensure_directories(self, env_dir) -> SimpleNamespace:
+        self._logger.debug(f"Creating virtual environment in '{env_dir}'")
+        _context: SimpleNamespace = super().ensure_directories(env_dir)
+        _python_exe = sys.executable
+        if not _python_exe:
+            raise PythonExecutableIdentificationError
+
+        self._logger.debug(f"Using python '{_python_exe}' for setup")
+
+        _context.executable = _python_exe
+        _dirname, _exename = os.path.split(os.path.abspath(_python_exe))
+        _context.python_dir = _dirname
+        _context.python_exe = _exename
+        return _context
```

### Comparing `fair_cli-0.5.2/LICENSE` & `fair_cli-0.7.0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-BSD 2-Clause License
-
-Copyright (c) 2021, SCRC
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 2-Clause License
+
+Copyright (c) 2021, SCRC
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `fair_cli-0.5.2/README.md` & `fair_cli-0.7.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,281 +1,281 @@
-# FAIR Data Pipeline Command Line Interface
-
-[![PyPI](https://img.shields.io/pypi/v/fair-cli)](https://pypi.org/project/fair-cli/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fair-cli)](https://pypi.org/project/fair-cli/) [![DOI](https://zenodo.org/badge/377398464.svg)](https://zenodo.org/badge/latestdoi/377398464) ![PyPI - License](https://img.shields.io/pypi/l/fair-cli)  [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/5411/badge)](https://bestpractices.coreinfrastructure.org/projects/5411)
-
-[![FAIR Data Pipeline CLI](https://github.com/FAIRDataPipeline/FAIR-CLI/actions/workflows/fair-cli.yaml/badge.svg?branch=main)](https://github.com/FAIRDataPipeline/FAIR-CLI/actions/workflows/fair-cli.yaml)  [![codecov](https://codecov.io/gh/FAIRDataPipeline/FAIR-CLI/branch/dev/graph/badge.svg?token=h93TkTiiWf)](https://codecov.io/gh/FAIRDataPipeline/FAIR-CLI) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=FAIRDataPipeline_FAIR-CLI&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=FAIRDataPipeline_FAIR-CLI)
-
-FAIR-CLI forms the main interface for synchronising changes between local and shared remote FAIR Data Pipeline registries, it is also used to instantiate model runs/data submissions to the pipeline. Full documentation of the FAIR Data Pipeline can be found on the project [website](https://www.fairdatapipeline.org/).
-
-## Installation
-
-The package is installed using Pip:
-
-```sh
-pip install fair-cli
-```
-
-To enable tab completion you need to modify your shell:
-
-### Bash
-```
-_FAIR_COMPLETE=bash_source fair > ~/.config/.fair-complete.bash
-echo '. ~/.config/.fair-complete.bash' >> ~/.bashrc
-```
-
-### zsh
-```
-_FAIR_COMPLETE=zsh_source fair > ~/.fair-complete.zsh
-echo '. ~/.fair-complete.zsh' >> ~/.bashrc
-```
-
-### Fish
-```
-_FAIR_COMPLETE=bash_source fair > ~/.config/fish/.fair-complete.fish
-echo '. ~/.config/fish/.fair-complete.fish' >> ~/.bashrc
-```
-
-## Uninstallation
-To uninstall the CLI run:
-```
-fair purge --all
-pip uninstall fair
-```
-
-## The User Configuration File
-Job runs are configured via `config.yaml` files. Upon initialisation of a project, FAIR-CLI automatically generates a starter configuration file with all requirements in place. To execute a process (e.g. perform a model run from a compiled binary/script) an additional key of either `script` or `script_path` must be provided. Alternatively the command `fair run bash` can be used to append the key and run a command directly.
-
-By default the shell used to execute a process is `sh` or `batch` for UNIX and Windows systems respectively. This can be overwritten by assigning the optional `shell` key with one of the following values (where `{0}` is the script file):
-
-| **Shell**    | **Command**                     |
-| ------------ | ------------------------------- |
-| `bash`       | `bash -eo pipefail {0}`         |
-| `java`       | `java {0}`                      |
-| `julia`      | `julia {0}`                     |
-| `powershell` | `powershell -command ". '{0}'"` |
-| `pwsh`       | `pwsh -command ". '{0}'"`       |
-| `python2`    | `python2 {0}`                   |
-| `python3`    | `python3 {0}`                   |
-| `python`     | `python {0}`                    |
-| `R`          | `R -f {0}`                      |
-| `sh`         | `sh -e {0}`                     |
-| `batch`      | `{0}`                           |
-
-A full description of `config.yaml` files can be found [here](https://www.fairdatapipeline.org/docs/interface/config/).
-
-## Available Commands
-
-### `init`
-
-Initialises a new FAIR repository within the given directory. This should ideally be the same location as the `.git` folder for the current project, however during setup an option is given to specify an alternative. The command will ask the user a series of questions which will provide metadata for tracking run authors, and also allow for the creation of a starter `config.yaml` file. Initialisation will also configure the CLI itself.
-
-#### Custom CLI Configuration
-After setup is complete, the current CLI configuration can also be saved using the command:
-```
-fair init --export
-```
-the created file can then be re-read at a later point during setup. Alternatively, if creating a configuration from scratch the YAML file should contain the following information:
-
-```yaml
-namespaces:
-  input: testing
-  output: testing
-registries:
-  local:
-    data_store: /path/to/local/data_store/,
-    directory: /local/registry/install/directory
-    uri: http://127.0.0.1:8000/api/
-  origin:
-    data_store: /remote/registry/data/store/path/
-    token: /path/to/remote/token
-    uri: https://data.scrc.uk/api/'
-user:
-  email: 'test@noreply',
-  family_name: 'Test'
-  given_names: 'Interface'
-  orcid: None,
-  uuid: '2ddb2358-84bf-43ff-b2aa-3ac7dc3b49f1'
-git:
-  local_repo: /local/repo/path
-  remote: origin
-description: Testing Project
-```
-this file is then read during the initialisation:
-
-```sh
-fair init --using <cli-config.yaml file>
-```
-
-For integration into a CI workflow, the setup can be skipped by running:
-
-```sh
-fair init --ci
-```
-
-which will create temporary directories for some of the required location paths.
-
-
-### `run`
-
-The purpose of `run` is to execute a model/submission run and submit results to the local registry. Outputs of a run will be stored within the `coderun` folder in the directory specified under the `data_store` tag in the `config.yaml`, by default this is `$HOME/.fair/data/coderun`.
-
-```sh
-fair run
-```
-
-If you wish to use an alternative `config.yaml` then specify it as an additional argument:
-
-```sh
-fair run /path/to/config.yaml
-```
-
-You can also launch a bash command directly, this will be automatically written into the `config.yaml`:
-
-```sh
-fair run --script 'echo "Hello World"'
-```
-
-note the command itself must be quoted as it is a single argument.
-
-By default the CLI will not allow the user to perform a run if the state of the analysis repository is such that it is behind the git remote, or contains uncommitted changes. To override this behaviour use the `--dirty` flag.
-
-### `pull`
-
-The command `pull` will update any entries within the `config.yaml` under the `register` heading creating `external_object` and `data_product` objects on the registry and downloading the data to the local data storage. Any data required for a run is downloaded and stored within the local registry. In addition any data products requested that are available on the remote registry are pulled locally.
-
-```sh
-fair pull /path/to/config.yaml
-```
-
-### `status`
-This command displays objects which are awaiting staging or have been staged behaving in a manner similar to `git status`:
-```sh
-fair status
-```
-staged changes are displayed in green, and unstaged in red.
-
-### `add`
-Before changes can be pushed to the remote registry they must be staged. This command allows you to stage objects displayed when running `fair status` so that they can be sent to the remote registry. Data products are displayed and staged in the form `namespace:data_product_name@version`:
-```sh
-fair add my_namespace:data_object@v0.1.0
-```
-
-### `push`
-The `push` command will push any staged data products to the remote registry:
-
-```sh
-fair push
-```
-
-### `purge`
-
-The `purge` command removes setup of the current project so it can bereinitialised:
-
-```sh
-fair purge
-```
-
-To remove all configurations entirely (including those global to all projects) run:
-
-```sh
-fair purge --global
-```
-
-To remove the data directory itself run:
-
-```sh
-fair purge --data
-```
-
-**WARNING**: This is not recommended as the registry may still have entries pointing to this location!
-
-Finally to remove everything run:
-
-```sh
-fair purge --all
-```
-
-this will remove the current repository `.fair` folder and the global FAIR directory which also contains the local registry.
-
-You can skip any confirmation messages by running:
-
-```sh
-fair purge --yes
-```
-
-### `registry`
-
-By default the CLI will launch the registry whenever a synchronisation or run is called. The server will only be halted once all ongoing CLI processes (in the case of multiple parallel calls) have been completed.
-
-However the user may also specify a manual launch that will override this behaviour, instead leaving the server running constantly allowing them to view the registry in the browser.
-
-The commands:
-
-```sh
-fair registry start
-```
-
-and
-
-```sh
-fair registry stop
-```
-
-will launch and halt the server respectively.
-
-The registry can be installed using the CLI as well by running:
-```sh
-fair registry install
-```
-with the additional options to specify the installation location, and the data registry repository tag to install from:
-```sh
-fair registry install --directory ~/.fair/my_registry --version v1.0-rc5
-```
-
-### `log`
-
-Runs are logged locally within the local FAIR repository. A full list of runs is shown by running:
-
-```sh
-fair log
-```
-
-This will present a list of runs in a summary analogous to a `git log` call:
-
-```yaml
-run 0db35c20946a1ebeaafdc3b30103cd74a57eb6b6
-Author: Joe Bloggs <jbloggs@noreply.uk>
-Date:   Wed Jun 30 09:09:30 2021
-```
-
-| **NOTE**                                                                                                                            |
-| ----------------------------------------------------------------------------------------------------------------------------------- |
-| The SHA for a job is *not* related to a registry code run identifier as multiple code runs can be executed within a single job. |
-
-### `view`
-
-To view the `stdout` of a run given its SHA as shown by running `fair log` use the command:
-
-```sh
-fair view <sha>
-```
-
-you do not need to specify the full SHA but rather the first few unique characters.
-
-## Template Variables
-
-Within the `config.yaml` file, template variables can be specified by using the notation `${{ VAR }}`, the following variables are currently recognised:
-
-| **Variable**        | **Description**                                                                  |
-| ------------------- | -------------------------------------------------------------------------------- |
-| `DATE`              | Date in the form `%Y%m%d`                                                        |
-| `DATETIME`          | Date and time in the form `%Y-%m-%sT%H:%M:S`                                     |
-| `DATETIME-%Y%H%M`   | Date and time in custom format (where `%Y%H%M` can be any valid form)            |
-| `USER`              | The current user as defined in the CLI                                           |
-| `USER_ID`           | The unique identifier for the current user        |
-| `REPO_DIR`          | The FAIR repository root directory                                               |
-| `CONFIG_DIR`        | The directory containing the `config.yaml` after template substitution           |
-| `LOCAL_TOKEN`       | The token for access to the local registry                                       |
-| `SOURCE_CONFIG`     | Path of the user defined `config.yaml`                                           |
-| `GIT_BRANCH`        | Current branch of the `git` repository                                           |
-| `GIT_REMOTE`        | The URI of the git repository specified during setup                             |
-| `GIT_TAG`           | The latest tag on `git`                                                          |
+# FAIR Data Pipeline Command Line Interface
+
+[![PyPI](https://img.shields.io/pypi/v/fair-cli)](https://pypi.org/project/fair-cli/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fair-cli)](https://pypi.org/project/fair-cli/) [![DOI](https://zenodo.org/badge/377398464.svg)](https://zenodo.org/badge/latestdoi/377398464) ![PyPI - License](https://img.shields.io/pypi/l/fair-cli)  [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/5411/badge)](https://bestpractices.coreinfrastructure.org/projects/5411)
+
+[![FAIR Data Pipeline CLI](https://github.com/FAIRDataPipeline/FAIR-CLI/actions/workflows/fair-cli.yaml/badge.svg?branch=main)](https://github.com/FAIRDataPipeline/FAIR-CLI/actions/workflows/fair-cli.yaml)  [![codecov](https://codecov.io/gh/FAIRDataPipeline/FAIR-CLI/branch/dev/graph/badge.svg?token=h93TkTiiWf)](https://codecov.io/gh/FAIRDataPipeline/FAIR-CLI) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=FAIRDataPipeline_FAIR-CLI&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=FAIRDataPipeline_FAIR-CLI)
+
+FAIR-CLI forms the main interface for synchronising changes between local and shared remote FAIR Data Pipeline registries, it is also used to instantiate model runs/data submissions to the pipeline. Full documentation of the FAIR Data Pipeline can be found on the project [website](https://www.fairdatapipeline.org/).
+
+## Installation
+
+The package is installed using Pip:
+
+```sh
+pip install fair-cli
+```
+
+To enable tab completion you need to modify your shell:
+
+### Bash
+```
+_FAIR_COMPLETE=bash_source fair > ~/.config/.fair-complete.bash
+echo '. ~/.config/.fair-complete.bash' >> ~/.bashrc
+```
+
+### zsh
+```
+_FAIR_COMPLETE=zsh_source fair > ~/.fair-complete.zsh
+echo '. ~/.fair-complete.zsh' >> ~/.bashrc
+```
+
+### Fish
+```
+_FAIR_COMPLETE=bash_source fair > ~/.config/fish/.fair-complete.fish
+echo '. ~/.config/fish/.fair-complete.fish' >> ~/.bashrc
+```
+
+## Uninstallation
+To uninstall the CLI run:
+```
+fair purge --all
+pip uninstall fair
+```
+
+## The User Configuration File
+Job runs are configured via `config.yaml` files. Upon initialisation of a project, FAIR-CLI automatically generates a starter configuration file with all requirements in place. To execute a process (e.g. perform a model run from a compiled binary/script) an additional key of either `script` or `script_path` must be provided. Alternatively the command `fair run bash` can be used to append the key and run a command directly.
+
+By default the shell used to execute a process is `sh` or `batch` for UNIX and Windows systems respectively. This can be overwritten by assigning the optional `shell` key with one of the following values (where `{0}` is the script file):
+
+| **Shell**    | **Command**                     |
+| ------------ | ------------------------------- |
+| `bash`       | `bash -eo pipefail {0}`         |
+| `java`       | `java {0}`                      |
+| `julia`      | `julia {0}`                     |
+| `powershell` | `powershell -command ". '{0}'"` |
+| `pwsh`       | `pwsh -command ". '{0}'"`       |
+| `python2`    | `python2 {0}`                   |
+| `python3`    | `python3 {0}`                   |
+| `python`     | `python {0}`                    |
+| `R`          | `R -f {0}`                      |
+| `sh`         | `sh -e {0}`                     |
+| `batch`      | `{0}`                           |
+
+A full description of `config.yaml` files can be found [here](https://www.fairdatapipeline.org/docs/interface/config/).
+
+## Available Commands
+
+### `init`
+
+Initialises a new FAIR repository within the given directory. This should ideally be the same location as the `.git` folder for the current project, however during setup an option is given to specify an alternative. The command will ask the user a series of questions which will provide metadata for tracking run authors, and also allow for the creation of a starter `config.yaml` file. Initialisation will also configure the CLI itself.
+
+#### Custom CLI Configuration
+After setup is complete, the current CLI configuration can also be saved using the command:
+```
+fair init --export
+```
+the created file can then be re-read at a later point during setup. Alternatively, if creating a configuration from scratch the YAML file should contain the following information:
+
+```yaml
+namespaces:
+  input: testing
+  output: testing
+registries:
+  local:
+    data_store: /path/to/local/data_store/,
+    directory: /local/registry/install/directory
+    uri: http://127.0.0.1:8000/api/
+  origin:
+    data_store: /remote/registry/data/store/path/
+    token: /path/to/remote/token
+    uri: https://data.fairdatapipeline.org/api/'
+user:
+  email: 'test@noreply',
+  family_name: 'Test'
+  given_names: 'Interface'
+  orcid: None,
+  uuid: '2ddb2358-84bf-43ff-b2aa-3ac7dc3b49f1'
+git:
+  local_repo: /local/repo/path
+  remote: origin
+description: Testing Project
+```
+this file is then read during the initialisation:
+
+```sh
+fair init --using <cli-config.yaml file>
+```
+
+For integration into a CI workflow, the setup can be skipped by running:
+
+```sh
+fair init --ci
+```
+
+which will create temporary directories for some of the required location paths.
+
+
+### `run`
+
+The purpose of `run` is to execute a model/submission run and submit results to the local registry. Outputs of a run will be stored within the `coderun` folder in the directory specified under the `data_store` tag in the `config.yaml`, by default this is `$HOME/.fair/data/coderun`.
+
+```sh
+fair run
+```
+
+If you wish to use an alternative `config.yaml` then specify it as an additional argument:
+
+```sh
+fair run /path/to/config.yaml
+```
+
+You can also launch a bash command directly, this will be automatically written into the `config.yaml`:
+
+```sh
+fair run --script 'echo "Hello World"'
+```
+
+note the command itself must be quoted as it is a single argument.
+
+By default the CLI will not allow the user to perform a run if the state of the analysis repository is such that it is behind the git remote, or contains uncommitted changes. To override this behaviour use the `--dirty` flag.
+
+### `pull`
+
+The command `pull` will update any entries within the `config.yaml` under the `register` heading creating `external_object` and `data_product` objects on the registry and downloading the data to the local data storage. Any data required for a run is downloaded and stored within the local registry. In addition any data products requested that are available on the remote registry are pulled locally.
+
+```sh
+fair pull /path/to/config.yaml
+```
+
+### `status`
+This command displays objects which are awaiting staging or have been staged behaving in a manner similar to `git status`:
+```sh
+fair status
+```
+staged changes are displayed in green, and unstaged in red.
+
+### `add`
+Before changes can be pushed to the remote registry they must be staged. This command allows you to stage objects displayed when running `fair status` so that they can be sent to the remote registry. Data products are displayed and staged in the form `namespace:data_product_name@version`:
+```sh
+fair add my_namespace:data_object@v0.1.0
+```
+
+### `push`
+The `push` command will push any staged data products to the remote registry:
+
+```sh
+fair push
+```
+
+### `purge`
+
+The `purge` command removes setup of the current project so it can bereinitialised:
+
+```sh
+fair purge
+```
+
+To remove all configurations entirely (including those global to all projects) run:
+
+```sh
+fair purge --global
+```
+
+To remove the data directory itself run:
+
+```sh
+fair purge --data
+```
+
+**WARNING**: This is not recommended as the registry may still have entries pointing to this location!
+
+Finally to remove everything run:
+
+```sh
+fair purge --all
+```
+
+this will remove the current repository `.fair` folder and the global FAIR directory which also contains the local registry.
+
+You can skip any confirmation messages by running:
+
+```sh
+fair purge --yes
+```
+
+### `registry`
+
+By default the CLI will launch the registry whenever a synchronisation or run is called. The server will only be halted once all ongoing CLI processes (in the case of multiple parallel calls) have been completed.
+
+However the user may also specify a manual launch that will override this behaviour, instead leaving the server running constantly allowing them to view the registry in the browser.
+
+The commands:
+
+```sh
+fair registry start
+```
+
+and
+
+```sh
+fair registry stop
+```
+
+will launch and halt the server respectively.
+
+The registry can be installed using the CLI as well by running:
+```sh
+fair registry install
+```
+with the additional options to specify the installation location, and the data registry repository tag to install from:
+```sh
+fair registry install --directory ~/.fair/my_registry --version v1.0-rc5
+```
+
+### `log`
+
+Runs are logged locally within the local FAIR repository. A full list of runs is shown by running:
+
+```sh
+fair log
+```
+
+This will present a list of runs in a summary analogous to a `git log` call:
+
+```yaml
+run 0db35c20946a1ebeaafdc3b30103cd74a57eb6b6
+Author: Joe Bloggs <jbloggs@noreply.uk>
+Date:   Wed Jun 30 09:09:30 2021
+```
+
+| **NOTE**                                                                                                                            |
+| ----------------------------------------------------------------------------------------------------------------------------------- |
+| The SHA for a job is *not* related to a registry code run identifier as multiple code runs can be executed within a single job. |
+
+### `view`
+
+To view the `stdout` of a run given its SHA as shown by running `fair log` use the command:
+
+```sh
+fair view <sha>
+```
+
+you do not need to specify the full SHA but rather the first few unique characters.
+
+## Template Variables
+
+Within the `config.yaml` file, template variables can be specified by using the notation `${{ VAR }}`, the following variables are currently recognised:
+
+| **Variable**        | **Description**                                                                  |
+| ------------------- | -------------------------------------------------------------------------------- |
+| `DATE`              | Date in the form `%Y%m%d`                                                        |
+| `DATETIME`          | Date and time in the form `%Y-%m-%sT%H:%M:S`                                     |
+| `DATETIME-%Y%H%M`   | Date and time in custom format (where `%Y%H%M` can be any valid form)            |
+| `USER`              | The current user as defined in the CLI                                           |
+| `USER_ID`           | The unique identifier for the current user        |
+| `REPO_DIR`          | The FAIR repository root directory                                               |
+| `CONFIG_DIR`        | The directory containing the `config.yaml` after template substitution           |
+| `LOCAL_TOKEN`       | The token for access to the local registry                                       |
+| `SOURCE_CONFIG`     | Path of the user defined `config.yaml`                                           |
+| `GIT_BRANCH`        | Current branch of the `git` repository                                           |
+| `GIT_REMOTE`        | The URI of the git repository specified during setup                             |
+| `GIT_TAG`           | The latest tag on `git`                                                          |
```

### Comparing `fair_cli-0.5.2/PKG-INFO` & `fair_cli-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-cli
-Version: 0.5.2
+Version: 0.7.0
 Summary: Synchronization interface for the SCRC FAIR Data Pipeline registry
 Home-page: https://www.fairdatapipeline.org/
 License: BSD-2-Clause
 Keywords: FAIR Data Pipeline,FAIR,Data Management,Provenance
 Author: Richard Reeve
 Author-email: richard.reeve@glasgow.ac.uk
 Requires-Python: >=3.8.0,<4.0.0
@@ -17,18 +17,21 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering
+Provides-Extra: all
 Requires-Dist: GitPython (>=3.1.18,<4.0.0)
 Requires-Dist: Jinja2 (>=3.0.1,<4.0.0)
 Requires-Dist: PyYAML (>=5.4.1,<7.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: email-validator (>=1.1.3,<2.0.0)
 Requires-Dist: netCDF4 (>=1.5.8,<2.0.0)
 Requires-Dist: pre-commit (>=2.15.0,<3.0.0)
@@ -129,15 +132,15 @@
   local:
     data_store: /path/to/local/data_store/,
     directory: /local/registry/install/directory
     uri: http://127.0.0.1:8000/api/
   origin:
     data_store: /remote/registry/data/store/path/
     token: /path/to/remote/token
-    uri: https://data.scrc.uk/api/'
+    uri: https://data.fairdatapipeline.org/api/'
 user:
   email: 'test@noreply',
   family_name: 'Test'
   given_names: 'Interface'
   orcid: None,
   uuid: '2ddb2358-84bf-43ff-b2aa-3ac7dc3b49f1'
 git:
```

