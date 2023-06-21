# Comparing `tmp/dls-slurmjob-1.0.2.tar.gz` & `tmp/dls-slurmjob-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-slurmjob-1.0.2.tar", last modified: Tue Jun 13 13:16:30 2023, max compression
+gzip compressed data, was "dls-slurmjob-1.0.3.tar", last modified: Wed Jun 21 12:26:31 2023, max compression
```

## Comparing `dls-slurmjob-1.0.2.tar` & `dls-slurmjob-1.0.3.tar`

### file list

```diff
@@ -1,136 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.798451 dls-slurmjob-1.0.2/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.798451 dls-slurmjob-1.0.2/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.798451 dls-slurmjob-1.0.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.798451 dls-slurmjob-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.794449 dls-slurmjob-1.0.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/configurations/dummy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.794449 dls-slurmjob-1.0.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/explanations/slurm_openapi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.802452 dls-slurmjob-1.0.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/docs/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.798451 dls-slurmjob-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/interfaces/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/job_summary_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/dbv0/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/dbv0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75101 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/dbv0/field_0.py
--rw-r--r--   0 runner    (1001) docker     (123)   531009 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/openapi.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/v0/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   109493 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/v0/field_0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.806454 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/restds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/query_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/submit_job.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/src/dls_slurmjob_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 13:16:30.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/src/dls_slurmjob_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/configurations/dummy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:16:30.810456 dls-slurmjob-1.0.2/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/scripts/hello.sh
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/scripts/hello1.json
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/scripts/hello2.json
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/scripts/hello_bxflow.json
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/scripts/hello_bxflow.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-13 13:16:19.000000 dls-slurmjob-1.0.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.407292 dls-slurmjob-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.395292 dls-slurmjob-1.0.3/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.395292 dls-slurmjob-1.0.3/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.395292 dls-slurmjob-1.0.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.395292 dls-slurmjob-1.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.391292 dls-slurmjob-1.0.3/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.395292 dls-slurmjob-1.0.3/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.395292 dls-slurmjob-1.0.3/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.395292 dls-slurmjob-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.395292 dls-slurmjob-1.0.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-06-21 12:26:31.407292 dls-slurmjob-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.395292 dls-slurmjob-1.0.3/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/configurations/dummy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.399292 dls-slurmjob-1.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.391292 dls-slurmjob-1.0.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.399292 dls-slurmjob-1.0.3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.399292 dls-slurmjob-1.0.3/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/explanations/slurm_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/explanations/slurm_openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.399292 dls-slurmjob-1.0.3/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.399292 dls-slurmjob-1.0.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.399292 dls-slurmjob-1.0.3/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.399292 dls-slurmjob-1.0.3/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 12:26:31.407292 dls-slurmjob-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.395292 dls-slurmjob-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.399292 dls-slurmjob-1.0.3/src/dls_slurmjob.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-06-21 12:26:31.000000 dls-slurmjob-1.0.3/src/dls_slurmjob.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-21 12:26:31.000000 dls-slurmjob-1.0.3/src/dls_slurmjob.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:26:31.000000 dls-slurmjob-1.0.3/src/dls_slurmjob.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-21 12:26:31.000000 dls-slurmjob-1.0.3/src/dls_slurmjob.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-21 12:26:31.000000 dls-slurmjob-1.0.3/src/dls_slurmjob.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 12:26:31.000000 dls-slurmjob-1.0.3/src/dls_slurmjob.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.399292 dls-slurmjob-1.0.3/src/dls_slurmjob_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.399292 dls-slurmjob-1.0.3/src/dls_slurmjob_api/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/interfaces/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.399292 dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/job_summary_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.403293 dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.403293 dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/openapi/dbv0/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/openapi/dbv0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75101 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/openapi/dbv0/field_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)   531009 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/openapi/openapi.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.403293 dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/openapi/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/openapi/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109493 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/openapi/v0/field_0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.403293 dls-slurmjob-1.0.3/src/dls_slurmjob_api/restds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/restds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/restds/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/restds/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/restds/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/restds/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_api/restds/restds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.403293 dls-slurmjob-1.0.3/src/dls_slurmjob_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.403293 dls-slurmjob-1.0.3/src/dls_slurmjob_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_cli/subcommands/query_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_cli/subcommands/submit_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.403293 dls-slurmjob-1.0.3/src/dls_slurmjob_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 12:26:31.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/src/dls_slurmjob_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.403293 dls-slurmjob-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.403293 dls-slurmjob-1.0.3/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/tests/configurations/dummy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:26:31.407292 dls-slurmjob-1.0.3/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/tests/scripts/hello.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/tests/scripts/hello1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/tests/scripts/hello2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/tests/scripts/hello_bxflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/tests/scripts/hello_bxflow.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/tests/scripts/mib_convert1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/tests/scripts/mib_convert1.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-21 12:26:20.000000 dls-slurmjob-1.0.3/tests/test_cli.py
```

### Comparing `dls-slurmjob-1.0.2/.dae-devops/Makefile` & `dls-slurmjob-1.0.3/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.dae-devops/docs/conventions.rst` & `dls-slurmjob-1.0.3/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.dae-devops/docs/developing.rst` & `dls-slurmjob-1.0.3/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.dae-devops/docs/devops.rst` & `dls-slurmjob-1.0.3/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.dae-devops/docs/docs_structure.rst` & `dls-slurmjob-1.0.3/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.dae-devops/docs/documenting.rst` & `dls-slurmjob-1.0.3/.dae-devops/docs/documenting.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.dae-devops/docs/installing.rst` & `dls-slurmjob-1.0.3/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.dae-devops/docs/testing.rst` & `dls-slurmjob-1.0.3/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.dae-devops/project.yaml` & `dls-slurmjob-1.0.3/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.devcontainer/Dockerfile` & `dls-slurmjob-1.0.3/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.devcontainer/devcontainer.json` & `dls-slurmjob-1.0.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.github/CONTRIBUTING.rst` & `dls-slurmjob-1.0.3/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.github/actions/install_requirements/action.yml` & `dls-slurmjob-1.0.3/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.github/dependabot.yml` & `dls-slurmjob-1.0.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.github/pages/index.html` & `dls-slurmjob-1.0.3/.github/pages/index.html`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.github/pages/make_switcher.py` & `dls-slurmjob-1.0.3/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.github/workflows/code.yml` & `dls-slurmjob-1.0.3/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.github/workflows/docs.yml` & `dls-slurmjob-1.0.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.github/workflows/docs_clean.yml` & `dls-slurmjob-1.0.3/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.github/workflows/linkcheck.yml` & `dls-slurmjob-1.0.3/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.gitignore` & `dls-slurmjob-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.gitlab-ci.yml` & `dls-slurmjob-1.0.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/.vscode/launch.json` & `dls-slurmjob-1.0.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/LICENSE` & `dls-slurmjob-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/PKG-INFO` & `dls-slurmjob-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-slurmjob
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simplified job submit and status using Slurm REST.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-slurmjob-1.0.2/docs/conf.py` & `dls-slurmjob-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/docs/explanations/slurm_openapi.rst` & `dls-slurmjob-1.0.3/docs/explanations/slurm_openapi.rst`

 * *Files 9% similar despite different names*

```diff
@@ -17,13 +17,15 @@
 I'm not exactly sure the best way to insulate the code from having to know too much about the OpenAPI version.
 
 You can try these curls::
 
     $ curl -s -H X-SLURM-USER-NAME:${USER} -H X-SLURM-USER-TOKEN:${SLURM_JWT} -H "Content-Type: application/json" -X POST https://slurm-rest.diamond.ac.uk:8443/slurm/v0.0.38/job/submit -d@tests/scripts/hello1.json -v
     $ curl -s -H X-SLURM-USER-NAME:${USER} -H X-SLURM-USER-TOKEN:${SLURM_JWT} -H "Content-Type: application/json" -X POST https://slurm-rest.diamond.ac.uk:8443/slurm/v0.0.38/job/submit -d@tests/scripts/hello2.json -v
 
+sbatch tests/scripts/mib_convert1.sh
+
 Some references
 - OpenAPI Specification https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.0.2.md#data-types
 - datamodel-code-generator https://koxudaxi.github.io/datamodel-code-generator/
 - Pydantic's section on Code Generation https://docs.pydantic.dev/latest/datamodel_code_generator/
 - Slurm's Specification https://slurm.schedmd.com/rest_api.html
```

### Comparing `dls-slurmjob-1.0.2/docs/images/dls-favicon.ico` & `dls-slurmjob-1.0.3/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/docs/images/dls-logo.svg` & `dls-slurmjob-1.0.3/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/pyproject.toml` & `dls-slurmjob-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/PKG-INFO` & `dls-slurmjob-1.0.3/src/dls_slurmjob.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-slurmjob
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simplified job submit and status using Slurm REST.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob.egg-info/SOURCES.txt` & `dls-slurmjob-1.0.3/src/dls_slurmjob.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 configurations/dummy.yaml
 docs/conf.py
 docs/index.rst
 docs/_static/css/custom.css
 docs/explanations/conventions.rst
 docs/explanations/docs_structure.rst
 docs/explanations/index.rst
+docs/explanations/slurm_examples.rst
 docs/explanations/slurm_openapi.rst
 docs/explanations/todo.rst
 docs/how-to/developing.rst
 docs/how-to/devops.rst
 docs/how-to/documenting.rst
 docs/how-to/index.rst
 docs/how-to/installing.rst
@@ -93,8 +94,10 @@
 tests/conftest.py
 tests/test_cli.py
 tests/configurations/dummy.yaml
 tests/scripts/hello.sh
 tests/scripts/hello1.json
 tests/scripts/hello2.json
 tests/scripts/hello_bxflow.json
-tests/scripts/hello_bxflow.sh
+tests/scripts/hello_bxflow.sh
+tests/scripts/mib_convert1.json
+tests/scripts/mib_convert1.sh
```

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_api/aiohttp_client.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_api/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_api/interfaces/client.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_api/interfaces/client.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/job_summary_model.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/job_summary_model.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/dbv0/field_0.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/openapi/dbv0/field_0.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/openapi.json` & `dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/openapi/openapi.json`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_api/models/openapi/v0/field_0.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_api/models/openapi/v0/field_0.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/aiohttp.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_api/restds/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/context.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_api/restds/context.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/dummy.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_api/restds/dummy.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_api/restds/restds.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_api/restds/restds.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_cli/main.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_cli/main.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/base.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/query_jobs.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_cli/subcommands/query_jobs.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_cli/subcommands/submit_job.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_cli/subcommands/submit_job.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_cli/version.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_cli/version.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_lib/__main__.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_lib/envvar.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/src/dls_slurmjob_lib/version.py` & `dls-slurmjob-1.0.3/src/dls_slurmjob_lib/version.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/tests/base_tester.py` & `dls-slurmjob-1.0.3/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/tests/conftest.py` & `dls-slurmjob-1.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/tests/scripts/hello_bxflow.json` & `dls-slurmjob-1.0.3/tests/scripts/hello_bxflow.json`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/tests/scripts/hello_bxflow.sh` & `dls-slurmjob-1.0.3/tests/scripts/hello_bxflow.sh`

 * *Files identical despite different names*

### Comparing `dls-slurmjob-1.0.2/tests/test_cli.py` & `dls-slurmjob-1.0.3/tests/test_cli.py`

 * *Files identical despite different names*

