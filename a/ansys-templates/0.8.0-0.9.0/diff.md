# Comparing `tmp/ansys_templates-0.8.0.tar.gz` & `tmp/ansys_templates-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_templates-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_templates-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_templates-0.8.0.tar` & `ansys_templates-0.9.0.tar`

### file list

```diff
@@ -1,254 +1,276 @@
--rw-r--r--   0        0        0     1091 2023-06-08 09:01:59.005198 ansys_templates-0.8.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     9947 2023-06-08 09:01:59.005198 ansys_templates-0.8.0/README.rst
--rw-r--r--   0        0        0     3132 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2266 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/__init__.py
--rw-r--r--   0        0        0     1284 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/__main__.py
--rw-r--r--   0        0        0     3776 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/cli.py
--rw-r--r--   0        0        0     1106 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/licenses/LICENSE_MIT
--rw-r--r--   0        0        0      199 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/licenses/__init__.py
--rw-r--r--   0        0        0     3894 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/paths.py
--rw-r--r--   0        0        0      398 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/cookiecutter.json
--rw-r--r--   0        0        0       86 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
--rw-r--r--   0        0        0      356 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
--rw-r--r--   0        0        0      265 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0       59 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
--rw-r--r--   0        0        0      418 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0      119 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
--rw-r--r--   0        0        0      594 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
--rw-r--r--   0        0        0     3729 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     2779 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
--rw-r--r--   0        0        0     2987 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      764 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0       11 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0     2689 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0      282 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1052 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
--rw-r--r--   0        0        0      657 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rwxr-xr-x   0        0        0     1026 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      969 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       63 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0       50 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rwxr-xr-x   0        0        0     4076 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0      928 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
--rw-r--r--   0        0        0       11 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     3414 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0      196 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
--rw-r--r--   0        0        0       27 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0       81 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
--rw-r--r--   0        0        0       32 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0     1104 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      140 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     2377 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1087 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/cookiecutter.json
--rw-r--r--   0        0        0     2046 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3238 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     1187 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1134 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0        0 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
--rw-r--r--   0        0        0      825 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1495 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/cookiecutter.json
--rw-r--r--   0        0        0     4461 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
--rw-r--r--   0        0        0        0 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
--rw-r--r--   0        0        0      283 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0     5008 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3052 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      599 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      453 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
--rw-r--r--   0        0        0       11 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      213 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
--rw-r--r--   0        0        0     2689 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0     2566 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
--rw-r--r--   0        0        0     7566 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      655 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rw-r--r--   0        0        0      753 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      928 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       66 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0    17194 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
--rw-r--r--   0        0        0       50 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      439 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0     3349 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     4322 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0    38829 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
--rw-r--r--   0        0        0      105 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
--rw-r--r--   0        0        0      421 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
--rw-r--r--   0        0        0       47 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
--rw-r--r--   0        0        0       46 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
--rw-r--r--   0        0        0       47 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
--rw-r--r--   0        0        0      959 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py
--rw-r--r--   0        0        0      725 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
--rw-r--r--   0        0        0    10963 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/monitoring_step.py
--rw-r--r--   0        0        0    10614 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py
--rw-r--r--   0        0        0      916 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
--rw-r--r--   0        0        0     9913 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png
--rw-r--r--   0        0        0      756 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/style.css
--rw-r--r--   0        0        0      585 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/colorscale.py
--rw-r--r--   0        0        0    16026 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_page.py
--rw-r--r--   0        0        0     2533 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/design_table_page.py
--rw-r--r--   0        0        0     5572 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/project_summary_page.py
--rw-r--r--   0        0        0      647 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/result_files_page.py
--rw-r--r--   0        0        0      962 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/scenery_page.py
--rw-r--r--   0        0        0      742 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/status_overview_page.py
--rw-r--r--   0        0        0     4962 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/summary_page.py
--rw-r--r--   0        0        0    12146 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/visualization_page.py
--rw-r--r--   0        0        0     5165 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py
--rw-r--r--   0        0        0    11879 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/problem_setup_page.py
--rw-r--r--   0        0        0       20 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
--rw-r--r--   0        0        0      664 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      193 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
--rw-r--r--   0        0        0      193 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
--rw-r--r--   0        0        0     1498 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1560 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
--rw-r--r--   0        0        0     2903 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
--rw-r--r--   0        0        0      800 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1132 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       49 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      111 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       21 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0     1461 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      997 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      186 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      687 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1558 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/cookiecutter.json
--rw-r--r--   0        0        0     3070 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
--rw-r--r--   0        0        0      763 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1133 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       58 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      104 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       25 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
--rw-r--r--   0        0        0      621 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
--rw-r--r--   0        0        0      525 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
--rw-r--r--   0        0        0       21 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0       28 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1475 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0     1877 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      955 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
--rw-r--r--   0        0        0        0 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     1062 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1557 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json
--rw-r--r--   0        0        0     3055 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
--rw-r--r--   0        0        0      951 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1145 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0      630 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
--rw-r--r--   0        0        0       44 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      116 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      265 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0      850 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
--rw-r--r--   0        0        0        0 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1409 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      851 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0       23 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
--rw-r--r--   0        0        0      902 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
--rw-r--r--   0        0        0      408 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      641 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      961 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1556 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json
--rw-r--r--   0        0        0     2831 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
--rw-r--r--   0        0        0      860 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1129 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0      445 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0     1299 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
--rw-r--r--   0        0        0      622 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
--rw-r--r--   0        0        0      184 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0     1458 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys/cookiecutter.json
--rw-r--r--   0        0        0     1110 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3398 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1540 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
--rw-r--r--   0        0        0     2619 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
--rw-r--r--   0        0        0     6537 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1879 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
--rw-r--r--   0        0        0     1010 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
--rw-r--r--   0        0        0      241 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0     1599 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
--rw-r--r--   0        0        0     1857 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
--rw-r--r--   0        0        0     1726 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
--rw-r--r--   0        0        0     4317 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
--rw-r--r--   0        0        0        0 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
--rw-r--r--   0        0        0      975 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pybasic/cookiecutter.json
--rw-r--r--   0        0        0     1035 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3170 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      896 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      253 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1027 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/solution/cookiecutter.json
--rw-r--r--   0        0        0     2852 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/solution/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
--rw-r--r--   0        0        0        0 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
--rw-r--r--   0        0        0      187 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.env
--rw-r--r--   0        0        0      283 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0     5020 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3061 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      599 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      453 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
--rw-r--r--   0        0        0       11 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      213 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
--rw-r--r--   0        0        0     2689 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0     2566 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
--rw-r--r--   0        0        0     8363 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1545 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml
--rw-r--r--   0        0        0      655 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rw-r--r--   0        0        0      753 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      928 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       66 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0    17194 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
--rw-r--r--   0        0        0       50 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      439 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0     3349 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     3781 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0    35407 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
--rw-r--r--   0        0        0      105 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
--rw-r--r--   0        0        0      583 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
--rw-r--r--   0        0        0       52 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
--rw-r--r--   0        0        0       52 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
--rw-r--r--   0        0        0      803 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
--rw-r--r--   0        0        0      570 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
--rw-r--r--   0        0        0      274 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
--rw-r--r--   0        0        0      263 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
--rw-r--r--   0        0        0      916 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
--rw-r--r--   0        0        0     9913 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png
--rw-r--r--   0        0        0   749872 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/solution-workflow-sketch.png
--rw-r--r--   0        0        0      121 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/style.css
--rw-r--r--   0        0        0     2030 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/first_page.py
--rw-r--r--   0        0        0     4695 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/intro_page.py
--rw-r--r--   0        0        0     5241 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py
--rw-r--r--   0        0        0      593 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/second_page.py
--rw-r--r--   0        0        0       20 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
--rw-r--r--   0        0        0      664 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      193 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
--rw-r--r--   0        0        0      193 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
--rw-r--r--   0        0        0     1498 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     4035 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/testing.py
--rw-r--r--   0        0        0     6698 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/utils.py
--rw-r--r--   0        0        0    11435 1970-01-01 00:00:00.000000 ansys_templates-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     9947 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/README.rst
+-rw-r--r--   0        0        0     3122 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2266 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/__init__.py
+-rw-r--r--   0        0        0     1284 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/__main__.py
+-rw-r--r--   0        0        0     3776 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/cli.py
+-rw-r--r--   0        0        0     1106 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/licenses/LICENSE_MIT
+-rw-r--r--   0        0        0      199 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/licenses/__init__.py
+-rw-r--r--   0        0        0     3894 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/paths.py
+-rw-r--r--   0        0        0      398 2023-06-21 06:48:24.583505 ansys_templates-0.9.0/src/ansys/templates/python/common/cookiecutter.json
+-rw-r--r--   0        0        0       86 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
+-rw-r--r--   0        0        0      356 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
+-rw-r--r--   0        0        0      265 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0       59 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
+-rw-r--r--   0        0        0      418 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0      119 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
+-rw-r--r--   0        0        0      594 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
+-rw-r--r--   0        0        0     3713 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     2779 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
+-rw-r--r--   0        0        0     2987 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      764 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       11 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0     2689 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0      282 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1052 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
+-rw-r--r--   0        0        0      657 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rwxr-xr-x   0        0        0     1026 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      969 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       63 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0       50 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rwxr-xr-x   0        0        0     4076 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0      928 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
+-rw-r--r--   0        0        0       11 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     3414 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
+-rw-r--r--   0        0        0       27 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0       81 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
+-rw-r--r--   0        0        0       32 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0     1104 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      140 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     2377 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1087 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/cookiecutter.json
+-rw-r--r--   0        0        0     2046 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3238 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     1187 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1134 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
+-rw-r--r--   0        0        0      825 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1732 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/cookiecutter.json
+-rw-r--r--   0        0        0     6017 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      161 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.env
+-rw-r--r--   0        0        0      283 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     2365 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2147 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     3177 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      655 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3349 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-06-21 06:48:24.587505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0   220746 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.lock
+-rw-r--r--   0        0        0      199 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.toml
+-rw-r--r--   0        0        0     4222 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    39004 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      421 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       50 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
+-rw-r--r--   0        0        0       47 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0     6614 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/extract_system_hierarchy.py
+-rw-r--r--   0        0        0     1360 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py
+-rw-r--r--   0        0        0      725 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      248 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/monitoring_step.py
+-rw-r--r--   0        0        0    12171 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py
+-rw-r--r--   0        0        0      922 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0      755 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
+-rw-r--r--   0        0        0       41 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
+-rw-r--r--   0        0        0     9913 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0       37 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
+-rw-r--r--   0        0        0     2579 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py
+-rw-r--r--   0        0        0     3687 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py
+-rw-r--r--   0        0        0     3177 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py
+-rw-r--r--   0        0        0     5284 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py
+-rw-r--r--   0        0        0     1837 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py
+-rw-r--r--   0        0        0     2482 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py
+-rw-r--r--   0        0        0     5649 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py
+-rw-r--r--   0        0        0     1753 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py
+-rw-r--r--   0        0        0     4962 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py
+-rw-r--r--   0        0        0     4954 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
+-rw-r--r--   0        0        0     9719 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py
+-rw-r--r--   0        0        0     3165 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py
+-rw-r--r--   0        0        0     3676 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py
+-rw-r--r--   0        0        0      960 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py
+-rw-r--r--   0        0        0     3626 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py
+-rw-r--r--   0        0        0      543 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py
+-rw-r--r--   0        0        0      983 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py
+-rw-r--r--   0        0        0     1372 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py
+-rw-r--r--   0        0        0      296 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/result_files_page.py
+-rw-r--r--   0        0        0      714 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py
+-rw-r--r--   0        0        0      660 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py
+-rw-r--r--   0        0        0      793 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py
+-rw-r--r--   0        0        0      574 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py
+-rw-r--r--   0        0        0       20 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1560 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
+-rw-r--r--   0        0        0     2903 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      800 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1132 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       49 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      111 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       21 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0     1461 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      997 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      186 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      687 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1558 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/cookiecutter.json
+-rw-r--r--   0        0        0     3070 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      763 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1133 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       58 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      104 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       25 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
+-rw-r--r--   0        0        0      621 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
+-rw-r--r--   0        0        0      525 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
+-rw-r--r--   0        0        0       21 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1475 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0     1877 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      955 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     1062 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1557 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json
+-rw-r--r--   0        0        0     3055 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      951 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1145 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-06-21 06:48:24.591505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0      630 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
+-rw-r--r--   0        0        0       44 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      116 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      265 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0      850 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1409 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      851 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0       23 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
+-rw-r--r--   0        0        0      902 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
+-rw-r--r--   0        0        0      408 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      641 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      961 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1556 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json
+-rw-r--r--   0        0        0     2831 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      860 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1129 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0      445 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0     1299 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
+-rw-r--r--   0        0        0      622 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
+-rw-r--r--   0        0        0      184 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0     1458 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys/cookiecutter.json
+-rw-r--r--   0        0        0     1110 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3398 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1540 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
+-rw-r--r--   0        0        0     2619 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     6537 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1879 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
+-rw-r--r--   0        0        0     1010 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      241 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0     1599 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
+-rw-r--r--   0        0        0     1857 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
+-rw-r--r--   0        0        0     1726 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
+-rw-r--r--   0        0        0     4317 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
+-rw-r--r--   0        0        0      975 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pybasic/cookiecutter.json
+-rw-r--r--   0        0        0     1035 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3170 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      896 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      253 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1027 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/cookiecutter.json
+-rw-r--r--   0        0        0     3166 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      161 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.env
+-rw-r--r--   0        0        0      283 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     2365 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1710 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     2701 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1545 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml
+-rw-r--r--   0        0        0      655 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3349 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-06-21 06:48:24.595505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0   198506 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/poetry.lock
+-rw-r--r--   0        0        0     3782 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    35407 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      583 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       52 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
+-rw-r--r--   0        0        0       51 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
+-rw-r--r--   0        0        0       52 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      803 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      570 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
+-rw-r--r--   0        0        0      274 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
+-rw-r--r--   0        0        0      263 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
+-rw-r--r--   0        0        0      922 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0      755 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
+-rw-r--r--   0        0        0       18 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
+-rw-r--r--   0        0        0   749872 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png
+-rw-r--r--   0        0        0     9913 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0       37 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
+-rw-r--r--   0        0        0       18 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/README.md
+-rw-r--r--   0        0        0     2030 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py
+-rw-r--r--   0        0        0     4700 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py
+-rw-r--r--   0        0        0     5244 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
+-rw-r--r--   0        0        0      593 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py
+-rw-r--r--   0        0        0       20 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-06-21 06:48:24.599505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-06-21 06:48:24.603505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-06-21 06:48:24.603505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-06-21 06:48:24.603505 ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     4035 2023-06-21 06:48:24.603505 ansys_templates-0.9.0/src/ansys/templates/testing.py
+-rw-r--r--   0        0        0     6698 2023-06-21 06:48:24.603505 ansys_templates-0.9.0/src/ansys/templates/utils.py
+-rw-r--r--   0        0        0    11425 1970-01-01 00:00:00.000000 ansys_templates-0.9.0/PKG-INFO
```

### Comparing `ansys_templates-0.8.0/LICENSES/MIT.txt` & `ansys_templates-0.9.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/README.rst` & `ansys_templates-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/pyproject.toml` & `ansys_templates-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-templates"
-version = "0.8.0"
+version = "0.9.0"
 description = "Creates Python projects according to PyAnsys guidelines"
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSES/MIT.txt"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -54,15 +54,15 @@
     "click>=7.0,<8.0.0",
     "cookiecutter>=2.1.0",
     "isort>=5.10.1",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "pytest==7.3.1",
+    "pytest==7.3.2",
     "pytest-cov==4.0.0",
 ]
 doc = [
     "ansys-sphinx-theme==0.9.9",
     "numpydoc==1.5.0",
     "sphinx==7.0.1",
     "sphinx-copybutton==0.5.2",
@@ -71,15 +71,15 @@
 [tool.flit.module]
 name = "ansys.templates"
 
 [project.scripts]
 ansys-templates = "ansys.templates.cli:main"
 
 [project.urls]
-Source = "https://github.com/ansys-templates/ansys-templates"
+Source = "https://github.com/ansys/ansys-templates"
 Homepage = "https://templates.ansys.com/"
 Documentation = "https://templates.ansys.com/"
 Tracker = "https://github.com/ansys/ansys-templates/issues"
 
 [tool.black]
 force-exclude = ["src/ansys/templates/python/"]
 line-length = "100"
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/__init__.py` & `ansys_templates-0.9.0/src/ansys/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/__main__.py` & `ansys_templates-0.9.0/src/ansys/templates/__main__.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/cli.py` & `ansys_templates-0.9.0/src/ansys/templates/cli.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/licenses/LICENSE_MIT` & `ansys_templates-0.9.0/src/ansys/templates/licenses/LICENSE_MIT`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/paths.py` & `ansys_templates-0.9.0/src/ansys/templates/paths.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 
 jobs:
 
   code-style:
     name: "Code style"
     runs-on: ubuntu-latest
     steps:
-      - uses: pyansys/actions/code-style@v4
+      - uses: ansys/actions/code-style@v4
         with:
           python-version: {{ '${{ env.MAIN_PYTHON_VERSION }}' }}
 
   doc-style:
     name: "Documentation style"
     runs-on: ubuntu-latest
     steps:
-      - uses: pyansys/actions/doc-style@v4
+      - uses: ansys/actions/doc-style@v4
         with:
           token: {{ '${{ secrets.GITHUB_TOKEN }}' }}
 
   smoke-tests:
     name: "Build and Smoke tests"
     runs-on: {{ '${{ matrix.os }}' }}
     needs: [code-style]
@@ -48,15 +48,15 @@
         {%- for minor in range(7, 11) -%}
         {%- if minor >= required_minor -%}
         {{ python_versions.append("3." + minor | string ) or ''}}
         {%- endif -%}
         {%- endfor -%}
         python-version: {{ python_versions }}
     steps:
-      - uses: pyansys/actions/build-wheelhouse@v4
+      - uses: ansys/actions/build-wheelhouse@v4
         with:
           library-name: {{ '${{ env.LIBRARY_NAME }}' }}
           library-namespace: {{ '${{ env.LIBRARY_NAMESPACE }}' }}
           operating-system: {{ '${{ matrix.os }}' }}
           python-version: {{ '${{ matrix.python-version }}' }}
 
   tests:
@@ -72,53 +72,53 @@
        {%- if minor >= required_minor -%}
        {{ python_versions.append("3." + minor | string ) or ''}}
        {%- endif -%}
        {%- endfor -%}
        python-version: {{ python_versions }}
       fail-fast: false
     steps:
-      - uses: pyansys/actions/tests-pytest@v4
+      - uses: ansys/actions/tests-pytest@v4
         with:
           pytest-extra-args: "--cov=ansys --cov-report=term --cov-report=html:.cov/html"
 
   doc-build:
     name: "Build documentation"
     runs-on: ubuntu-latest
     needs: [doc-style]
     steps:
-      - uses: pyansys/actions/doc-build@v4
+      - uses: ansys/actions/doc-build@v4
         with:
           python-version: {{ '${{ env.MAIN_PYTHON_VERSION }}' }}
 
   build-library:
     name: "Build library basic example"
     runs-on: ubuntu-latest
     needs: [doc-build, tests]
     steps:
-      - uses: pyansys/actions/build-library@v4
+      - uses: ansys/actions/build-library@v4
         with:
           library-name: {{ '${{ env.LIBRARY_NAME }}' }}
           python-version: {{ '${{ env.MAIN_PYTHON_VERSION }}' }}
 
   doc-deploy-dev:
     name: "Deploy development documentation"
     runs-on: ubuntu-latest
     needs: [build-library]
     if: github.event_name == 'push' && !contains(github.ref, 'refs/tags')
     steps:
-      - uses: pyansys/actions/doc-deploy-dev@v4
+      - uses: ansys/actions/doc-deploy-dev@v4
         with:
           cname: {{ '${{ env.DOCUMENTATION_CNAME }}' }}
           token: {{ '${{ secrets.GITHUB_TOKEN }}' }}
 
   doc-deploy-stable:
     name: "Deploy stable documentation"
     runs-on: ubuntu-latest
     needs: [build-library]
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags')
     steps:
-      - uses: pyansys/actions/doc-deploy-stable@v4
+      - uses: ansys/actions/doc-deploy-stable@v4
         with:
           cname: {{ '${{ env.DOCUMENTATION_CNAME }}' }}
           token: {{ '${{ secrets.GITHUB_TOKEN }}' }}
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-0.9.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/doc_project/cookiecutter.json` & `ansys_templates-0.9.0/src/ansys/templates/python/doc_project/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py` & `ansys_templates-0.9.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-0.9.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/cookiecutter.json` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/cookiecutter.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9032258064516129%*

 * *Differences: {"'__optiSLang_metadata_file'": '"{{ '*

 * *                                "cookiecutter.optiSLang_metadata_file|lower|replace('\\\\\\\\', "*

 * *                                '\'/\') }} "',*

 * * "'__optiSLang_metadata_file_name'": '"{{ cookiecutter.__optiSLang_metadata_file.split(\'/\')[-1] '*

 * *                                     '}}"',*

 * * "'optiSLang_metadata_file'": "''"}*

```diff
@@ -2,14 +2,16 @@
     "__build_system": "poetry",
     "__coverage_source": "{{ cookiecutter.__project_name_slug }}",
     "__is_pyansys": "False",
     "__library_name_slug": "",
     "__logo": "solutions",
     "__logo_color": "black",
     "__max_linelength": "120",
+    "__optiSLang_metadata_file": "{{ cookiecutter.optiSLang_metadata_file|lower|replace('\\\\', '/') }} ",
+    "__optiSLang_metadata_file_name": "{{ cookiecutter.__optiSLang_metadata_file.split('/')[-1] }}",
     "__optiSLang_project_file": "{{ cookiecutter.optiSLang_project_file|lower|replace('\\\\', '/') }} ",
     "__optiSLang_project_file_name": "{{ cookiecutter.__optiSLang_project_file.split('/')[-1] }}",
     "__optiSLang_properties_file": "{{ cookiecutter.optiSLang_properties_file|lower|replace('\\\\', '/') }} ",
     "__optiSLang_properties_file_name": "{{ cookiecutter.__optiSLang_properties_file.split('/')[-1] }}",
     "__pkg_name": "ansys-solutions-{{ cookiecutter.solution_name.lower().replace('_', '-') }}",
     "__pkg_namespace": "ansys.solutions.{{ cookiecutter.__project_name_slug }}",
     "__product_name_slug": "",
@@ -20,13 +22,14 @@
     "__solution_definition_name": "{{ cookiecutter.__solution_name_slug.title() }}Solution",
     "__solution_name_slug": "{{ cookiecutter.solution_name.lower().replace('-', '_') }}",
     "__template_name": "osl-solution",
     "__version": "0.1.dev0",
     "_copy_without_render": [
         "*.html"
     ],
+    "optiSLang_metadata_file": "",
     "optiSLang_project_file": "",
     "optiSLang_properties_file": "",
     "project_name": "my-osl-solution",
     "solution_display_name": "My optiSLang Solution",
     "solution_name": "my_osl_solution"
 }
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,50 +16,66 @@
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/styles/.gitignore",
     "doc/.vale.ini",
     "doc/make.bat",
     "doc/Makefile",
     "examples/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/assets/README.md",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/scripts/extract_system_hierarchy.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/scripts/README.md",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/utils.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/solution/definition.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/solution/monitoring_step.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/solution/problem_setup_step.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/style.css",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/monitoring_tabs/design_table_page.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/monitoring_tabs/project_summary_page.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/monitoring_tabs/result_files_page.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/monitoring_tabs/scenery_page.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/monitoring_tabs/status_overview_page.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/monitoring_tabs/summary_page.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/monitoring_tabs/visualization_page.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/css/style.css",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/images/README.md",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/logos/ansys-solutions-horizontal-logo.png",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/scripts/README.md",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/components/actor_information_table.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/components/actor_logs_table.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/components/actor_statistics_table.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/components/design_table.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/components/logs_table.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/components/project_summary_table.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/components/summary_view.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/components/system_files.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/pages/monitoring_page.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/pages/page.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/pages/problem_setup_page.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/utils/alerts.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/utils/common_functions.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/utils/constants.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/utils/monitoring.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/utils/placeholders.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/views/design_table_page.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/views/project_summary_page.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/views/result_files_page.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/views/scenery_page.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/views/status_overview_page.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/views/summary_page.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/views/visualization_page.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/app.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/colorscale.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/monitoring_page.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/problem_setup_page.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/page.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/__init__.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/main.py",
     "tests/common_test_files/README.md",
     "tests/integration/test_integration_dummy.py",
     "tests/unit/test_unit_dummy.py",
     "tests/conftest.py",
     ".codespell.exclude",
     ".codespell.ignore",
+    ".env",
     ".flake8",
     ".gitignore",
     ".pre-commit-config.yaml",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CODEOWNERS",
     "CONTRIBUTING.md",
     "LICENSE.rst",
+    "poetry.lock",
     "pyproject.toml",
     "README.rst",
     "setup_environment.py",
     "tox.ini"
 ]
 """A list holding all desired files to be included in the project."""
 
@@ -73,23 +89,24 @@
         working_directory = os.path.dirname(os.getcwd())
         file_path = os.path.join(working_directory, file_path)
 
     if os.path.exists(file_path):
         shutil.copy(file_path, destination)
     else:
         print(f"Unable to find {file_path}.")
-        # raise FileNotFoundError(f"Unable to find {file_path}.")
 
 
 def main():
     """Entry point of the script."""
 
     keep_files(DESIRED_STRUCTURE)
 
     if len("{{ cookiecutter.__optiSLang_project_file }}".replace(" ", "")):
         copy_file_to_assets_folder("{{ cookiecutter.__optiSLang_project_file }}",  str(ASSETS_DIRCTORY / "{{ cookiecutter.__optiSLang_project_file_name }}"))
     if len("{{ cookiecutter.__optiSLang_properties_file }}".replace(" ", "")):
         copy_file_to_assets_folder("{{ cookiecutter.__optiSLang_properties_file }}", str(ASSETS_DIRCTORY / "{{ cookiecutter.__optiSLang_properties_file_name }}"))
+    if len("{{ cookiecutter.__optiSLang_metadata_file }}".replace(" ", "")):
+        copy_file_to_assets_folder("{{ cookiecutter.__optiSLang_metadata_file }}", str(ASSETS_DIRCTORY / "{{ cookiecutter.__optiSLang_metadata_file_name }}"))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -38,27 +38,28 @@
 url = "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple/"
 default = false
 secondary = true
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 ansys-dash-treeview = {version = "0.0.1.dev0", source = "solutions-private-pypi"}
-ansys-saf-glow = {version = "0.3.dev2", source = "solutions-private-pypi"}
-ansys-saf-portal = {version = "0.1.6", source = "solutions-private-pypi"}
-ansys-solutions-dash-lib = {version = "0.3.0", source = "solutions-private-pypi"}
-ansys-solutions-products-ecosystem = {version = "0.1.dev0", source = "solutions-private-pypi"}
-ansys-solutions-optislang-parser = {version = "0.1.dev5", source = "solutions-private-pypi"}
-ansys-solutions-optislang-wrapper = {version = "0.2.dev1", source = "solutions-private-pypi"}
-ansys-solutions-optislang-frontend-components = {version = "0.1.dev3", source = "solutions-private-pypi"}
-optislang-dash-lib = {version = "^0.0.1", source = "solutions-private-pypi"}
-dash = {version = "^2.6"}
-dash_bootstrap_components = {version = "^1.2"}
-dash-extensions = {version = "^0.1"}
-dash-iconify = {version = "^0.1"}
-dash-uploader = {version = "^0.6"}
+ansys-optislang-core = "^0.3.0"
+ansys-saf-glow = {version = "0.3.dev4", source = "solutions-private-pypi"}
+ansys-saf-portal = {version = "0.2.0", source = "solutions-private-pypi"}
+ansys-solutions-dash-lib = {version = "^0.3.0", source = "solutions-private-pypi"}
+ansys-solutions-products-ecosystem = {version = "^0.1.dev0", source = "solutions-private-pypi"}
+ansys-solutions-optislang-parser = {version = "^0.1.dev6", source = "solutions-private-pypi"}
+ansys-solutions-optislang-frontend-components = {version = "^0.1.dev3", source = "solutions-private-pypi"}
+optislang-dash-lib = {version = "^0.2.1", source = "solutions-private-pypi"}
+dash = "^2.6"
+dash_bootstrap_components = "^1.2"
+dash-extensions = "^0.1"
+dash-iconify = "^0.1"
+dash-uploader = "^0.6"
+pandas = "^2.0.0"
 
 [tool.poetry.group.doc]
 optional = true
 [tool.poetry.group.doc.dependencies]
 ansys-sphinx-theme = {version = "^0.8.0"}
 numpydoc = {version = "^1.4.0"}
 sphinx = {version = "5.1.0"}
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
+# CAPTURED v0.4.0 from:
+# https://github.com/Solution-Applications/common-files/blob/v0.4.0/setup-environment/setup_environment.py
 
 """
 A Python script to automate the setup of the Python ecosystem of a project.
 
 Prerequisites
 -------------
 
@@ -648,16 +650,17 @@
         check=True,
     )
     # Turn-on in-project
     subprocess.run([rf".\{venv_name}\Scripts\poetry", "config", "virtualenvs.create", "false", "--local"], check=True)
     # Declare credentials for private sources
     for source in private_sources:
         print(f"Declare credentials for {source['name']}")
-        # Get source PAT
-        if source["url"] == "https://pkgs.dev.azure.com/pyansys/_packaging/pyansys/pypi/simple/":
+        if source["name"].lower() == "pypi":
+            continue
+        elif source["url"] == "https://pkgs.dev.azure.com/pyansys/_packaging/pyansys/pypi/simple/":
             token = os.environ["PYANSYS_PRIVATE_PYPI_PAT"]
         elif source["url"] == "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple/":
             token = os.environ["SOLUTIONS_PRIVATE_PYPI_PAT"]
         else:
             raise Exception(f"Unknown private source {source['name']} with url {source['url']}.")
         # Store credentials
         if credentials_management_method == "keyring":
@@ -981,8 +984,8 @@
     print("Execution time: %.1f minutes." % (elapsed_time))
     print()
 
 
 # =================================================== [Execution] =================================================== #
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 
 # If folder doesn't exist, it will be created later
 UPLOAD_DIRECTORY = os.path.join(tempfile.gettempdir(), "GLOW")
 du.configure_upload(app, UPLOAD_DIRECTORY)
 
 # !IMPORTANT Keeping the import line here to adapt with dash_uploader config, moving the import above will fail the
 # dash uploader configuration
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.page import layout
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.pages.page import layout
 
 app.layout = layout
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/result_files_page.py` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Frontend of the second step."""
 
-import dash_bootstrap_components as dbc
+
 from dash_extensions.enrich import dcc, html
 
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.monitoring_step import MonitoringStep
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.second_step import SecondStep
 
 
-def layout(monitoring_step: MonitoringStep):
+def layout(step: SecondStep):
     """Layout of the second step UI."""
-
     return html.Div(
         [
+            dcc.Markdown("""#### Second step""", className="display-3"),
+            dcc.Markdown("""###### Subtitle.""", className="display-3"),
+            html.Hr(className="my-2"),
             html.Br(),
-            dbc.Row(
-                [
-                    dcc.Markdown("**Result files: Under construction**", style={"font-size": "15px"}),
-                ],
-            ),
         ]
     )
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/scenery_page.py` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 # ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
-"""Frontend of the scenery view tab."""
+"""Frontend of the scenery view."""
 
-import dash_bootstrap_components as dbc
 from dash_extensions.enrich import html
 import optislang_dash_lib
 
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.monitoring_step import MonitoringStep
 
+def layout(project_status_info: dict) -> html.Div:
+    """Layout of the scenery view."""
 
-def layout(monitoring_step: MonitoringStep):
-    """Layout of the scenery view tab."""
-
-    monitoring_step.get_project_state() # fetches data on page load
-
-    return html.Div(
-        [
-            html.Br(),
-            dbc.Row(
-                [
-                    html.Div(
-                        [
-                            optislang_dash_lib.SceneryComponent(
-                                id="input",
-                                project_state=monitoring_step.project_state,
-                            ),
-                        ]
-                    )
-                ],
-            ),
-        ]
-    )
+    if project_status_info:
+        return html.Div(
+            [
+                html.Br(),
+                html.Div(
+                    [
+                        optislang_dash_lib.SceneryComponent(
+                            id="input",
+                            project_state=project_status_info,
+                        ),
+                    ]
+                ),
+            ]
+        )
+    else:
+        return html.Div([])
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,40 +8,44 @@
 import dash_bootstrap_components as dbc
 from dash_extensions.enrich import Input, Output, callback, callback_context, dcc, html
 from dash_iconify import DashIconify
 
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.definition import (
     {{ cookiecutter.__solution_definition_name }},
 )
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui import problem_setup_page, monitoring_page
-
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.pages import intro_page, first_page, second_page
 
 step_list = [
     {
-        "key": "problem_setup_step",
-        "text": "Problem Setup",
+        "key": "intro_step",
+        "text": "Introduction",
         "depth": 0,
     },
     {
-        "key": "monitoring_step",
-        "text": "Monitoring",
+        "key": "first_step",
+        "text": "First Step",
         "depth": 0,
     },
+    {
+        "key": "second_step",
+        "text": "Second Step",
+        "depth": 0,
+    }
 ]
 
 
 layout = html.Div(
     [
         dcc.Location(id="url", refresh=False), # represents the browser address bar and doesn't render anything
         dbc.Stack(
             [
                 html.Div(
                     [
                         html.Img(
-                        src = r"/assets/Graphics/ansys-solutions-horizontal-logo.png",
+                        src = r"/assets/logos/ansys-solutions-horizontal-logo.png",
                         style={'width': '80%'}
                     )
                     ],
                 ),
                 html.Div(
                     [
                         dbc.Button(
@@ -93,15 +97,14 @@
 
 @callback(
     Output("return-to-portal", "children"),
     Input("url", "pathname"),
 )
 def return_to_portal(pathname):
     """Display Solution Portal when back-to-portal button gets selected."""
-
     portal_ui_url = DashClient.get_portal_ui_url()
     children = (
         []
         if portal_ui_url is None
         else [
             dbc.Button(
                 "Back to Projects",
@@ -118,42 +121,38 @@
 
 @callback(
     Output("project-name", "children"),
     Input("url", "pathname"),
 )
 def display_poject_name(pathname):
     """Display current project name."""
-
     project = DashClient[{{cookiecutter.__solution_definition_name}}].get_project(pathname)
     return f"Project Name: {project.project_display_name}"
 
 
+# this callback is essential for initializing the step based on the persisted
+# state of the project when the browser first displays the project to the user
+# given the project's URL
 @callback(
     Output("page-content", "children"),
     [
         Input("url", "pathname"),
         Input("navigation_tree", "focus"),
     ],
     prevent_initial_call=True,
 )
 def display_page(pathname, value):
-    """
-    Display page content.
-
-    this callback is essential for initializing the step based on the persisted
-    state of the project when the browser first displays the project to the user
-    given the project's URL.
-    """
-
+    """Display page content."""
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
     triggered_id = callback_context.triggered[0]["prop_id"].split(".")[0]
-
     if triggered_id == "url":
-        return problem_setup_page.layout(project.steps.problem_setup_step)
+        return intro_page.layout(project.steps.intro_step)
     if triggered_id == "navigation_tree":
         if value is None:
             page_layout = html.H1("Welcome!")
-        elif value == "problem_setup_step":
-            page_layout = problem_setup_page.layout(project.steps.problem_setup_step)
-        elif value == "monitoring_step":
-            page_layout = monitoring_page.layout(project.steps.monitoring_step, project.steps.problem_setup_step)
+        elif value == "intro_step":
+            page_layout = intro_page.layout(project.steps.intro_step)
+        elif value == "first_step":
+            page_layout = first_page.layout(project.steps.first_step)
+        elif value == "second_step":
+            page_layout = second_page.layout(project.steps.second_step)
         return page_layout
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/cookiecutter.json` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyansys/cookiecutter.json` & `ansys_templates-0.9.0/src/ansys/templates/python/pyansys/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-0.9.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json` & `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json` & `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml` & `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml` & `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml` & `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml` & `ansys_templates-0.9.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pybasic/cookiecutter.json` & `ansys_templates-0.9.0/src/ansys/templates/python/pybasic/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-0.9.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-0.9.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/cookiecutter.json` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/hooks/post_gen_project.py` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/hooks/post_gen_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,53 +12,58 @@
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/styles/.gitignore",
     "doc/.vale.ini",
     "doc/make.bat",
     "doc/Makefile",
     "examples/README.md",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/assets/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/scripts/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/model/README.md",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/solution/definition.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/solution/intro_step.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/solution/first_step.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/solution/second_step.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/__init__.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/main.py",
     "tests/common_test_files/README.md",
     "tests/integration/test_integration_dummy.py",
     "tests/unit/test_unit_dummy.py",
     "tests/conftest.py",
     ".codespell.exclude",
     ".codespell.ignore",
+    ".env",
     ".flake8",
     ".gitignore",
     ".pre-commit-config.yaml",
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
     "CODEOWNERS",
     "CONTRIBUTING.md",
     "LICENSE.rst",
+    "poetry.lock",
     "pyproject.toml",
     "README.rst",
     "setup_environment.py",
     "tox.ini",
     ".env"
 ]
 """A list holding all desired files to be included in the project."""
 
 UI_STRUCTURE = [
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/Graphics/solution-workflow-sketch.png",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/style.css",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/css/style.css",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/images/README.md",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/logos/ansys-solutions-horizontal-logo.png",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/assets/scripts/README.md",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/components/README.md",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/pages/first_page.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/pages/intro_page.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/pages/second_page.py",
+    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/pages/page.py",
     f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/app.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/intro_page.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/first_page.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/second_page.py",
-    f"src/ansys/solutions/{{ cookiecutter.__solution_name_slug }}/ui/page.py",
 ]
 
 # Add UI structure to desired structure if applicable
 if "{{ cookiecutter.with_dash_ui }}" == "yes":
     DESIRED_STRUCTURE = DESIRED_STRUCTURE + UI_STRUCTURE
 
 def main():
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files 27% similar despite different names*

```diff
@@ -86,49 +86,25 @@
 # Jupyter Notebook
 .ipynb_checkpoints
 
 # IPython
 profile_default/
 ipython_config.py
 
-# VS Code
-# .vscode/
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-poetry.lock
-
 # PEP 582; used by e.g. github.com/David-OConnor/pyflow
 __pypackages__/
 
 # Celery stuff
 celerybeat-schedule
 celerybeat.pid
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
-.poetry
-.env/
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["poetry-core>=1.0.0,<1.3.0", "setuptools>=65.0"]
 build-backend = "poetry.core.masonry.api"
 
 [build-system-requirements]
-build-system-version = "1.4.2"
+build-system-version = "1.5.2"
 
 [tool.poetry]
 name = "{{cookiecutter.__pkg_name}}"
 version = "{{cookiecutter.__version}}"
 description = "{{cookiecutter.__short_description}}"
 license = "Proprietary"
 authors = ["ANSYS, Inc. <solution-applications.maintainers@ansys.com>"]
@@ -40,16 +40,16 @@
 name = "PyPI"
 priority = "primary"
 
 # Main dependencies
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 ansys-dash-treeview = {version = "0.0.1.dev0", source = "solutions-private-pypi"}
-ansys-saf-glow = {version = "^0.2.0", source = "solutions-private-pypi" }
-ansys-saf-portal = {version = "^0.1.7", source = "solutions-private-pypi"}
+ansys-saf-glow = {version = "0.3.dev4", source = "solutions-private-pypi" }
+ansys-saf-portal = {version = "0.2.0", source = "solutions-private-pypi"}
 {% if cookiecutter.with_dash_ui == "yes" %}
 dash = {version = "^2.6"}
 dash_bootstrap_components = {version = "^1.2"}
 dash-extensions = {version = "^0.1"}
 dash-iconify = {version = "^0.1"}
 dash-uploader = {version = "^0.6"}
 {% endif %}
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 
 # If folder doesn't exist, it will be created later
 UPLOAD_DIRECTORY = os.path.join(tempfile.gettempdir(), "GLOW")
 du.configure_upload(app, UPLOAD_DIRECTORY)
 
 # !IMPORTANT Keeping the import line here to adapt with dash_uploader config, moving the import above will fail the
 # dash uploader configuration
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.page import layout
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.pages.page import layout
 
 app.layout = layout
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/solution-workflow-sketch.png` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/first_page.py` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/intro_page.py` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def layout(step: IntroStep):
     """Layout of the first step UI."""
 
     solution_workflow_sketch_encoded = base64.b64encode(
         open(
-            os.path.join(Path(__file__).parent.absolute(), "assets", "Graphics", "solution-workflow-sketch.png"), "rb"
+            os.path.join(Path(__file__).parent.parent.absolute(), "assets", "images", "solution-workflow-sketch.png"), "rb"
         ).read()
     )
 
     return html.Div(
         dbc.Container(
             [
                 html.H1("Add a title.", className="display-3", style={"font-size": "35px"}),
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py` & `ansys_templates-0.9.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,51 @@
 # ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Initialization of the frontend layout across all the steps."""
 
-
 from ansys.saf.glow.client.dashclient import DashClient
 from ansys_dash_treeview import AnsysDashTreeview
 import dash_bootstrap_components as dbc
 from dash_extensions.enrich import Input, Output, callback, callback_context, dcc, html
 from dash_iconify import DashIconify
 
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.definition import (
-    {{ cookiecutter.__solution_definition_name }},
-)
-from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui import intro_page, first_page, second_page
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.definition import {{ cookiecutter.__solution_definition_name }}
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.pages import monitoring_page, problem_setup_page
+from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.common_functions import extract_dict_by_key, read_system_hierarchy
 
-step_list = [
-    {
-        "key": "intro_step",
-        "text": "Introduction",
-        "depth": 0,
-    },
-    {
-        "key": "first_step",
-        "text": "First Step",
-        "depth": 0,
-    },
-    {
-        "key": "second_step",
-        "text": "Second Step",
-        "depth": 0,
-    }
-]
+step_list = read_system_hierarchy()
 
 
 layout = html.Div(
     [
-        dcc.Location(id="url", refresh=False), # represents the browser address bar and doesn't render anything
+        dcc.Location(id="url", refresh=False),  # represents the browser address bar and doesn't render anything
         dbc.Stack(
             [
                 html.Div(
-                    [
-                        html.Img(
-                        src = r"/assets/Graphics/ansys-solutions-horizontal-logo.png",
-                        style={'width': '80%'}
-                    )
-                    ],
+                    [html.Img(src=r"/assets/logos/ansys-solutions-horizontal-logo.png", style={"width": "80%"})],
                 ),
                 html.Div(
                     [
                         dbc.Button(
                             "Project Name:",
-                            id = "project-name",
-                            disabled = True,
+                            id="project-name",
+                            disabled=True,
                             style={
                                 "color": "rgba(0, 0, 0, 1)",
                                 "background-color": "rgba(255, 255, 255, 1)",
-                                "border-color": "rgba(0, 0, 0, 1)"
+                                "border-color": "rgba(0, 0, 0, 1)",
                             },
                         )
                     ],
                     className="ms-auto",
                 ),
                 html.Div(id="return-to-portal"),
             ],
-            direction = "horizontal",
-            gap = 3,
+            direction="horizontal",
+            gap=3,
         ),
         html.Br(),
         dbc.Row(
             [
                 dbc.Col(
                     AnsysDashTreeview(
                         id="navigation_tree",
@@ -78,21 +55,15 @@
                             DashIconify(icon="bi:caret-down-square-fill"),
                         ],
                         style={"showButtons": True, "focusColor": "#ffb71b", "itemHeight": "32"},  # Ansys gold
                     ),
                     width=2,
                     style={"background-color": "rgba(242, 242, 242, 0.6)"},  # Ansys grey
                 ),
-                dbc.Col(
-                    html.Div(
-                        id="page-content",
-                        style={"padding-right": "1%"}
-                    ),
-                    width=10
-                ),
+                dbc.Col(html.Div(id="page-content", style={"padding-right": "1%"}), width=10),
             ],
         ),
     ]
 )
 
 
 @callback(
@@ -104,55 +75,61 @@
     portal_ui_url = DashClient.get_portal_ui_url()
     children = (
         []
         if portal_ui_url is None
         else [
             dbc.Button(
                 "Back to Projects",
-                id = "return-to-portal",
-                className = "me-2",
-                n_clicks = 0,
-                href = portal_ui_url,
-                style = {"background-color": "rgba(0, 0, 0, 1)", "border-color": "rgba(0, 0, 0, 1)"},
+                id="return-to-portal",
+                className="me-2",
+                n_clicks=0,
+                href=portal_ui_url,
+                style={"background-color": "rgba(0, 0, 0, 1)", "border-color": "rgba(0, 0, 0, 1)"},
             )
         ]
     )
     return children
 
 
 @callback(
     Output("project-name", "children"),
     Input("url", "pathname"),
 )
 def display_poject_name(pathname):
     """Display current project name."""
-    project = DashClient[{{cookiecutter.__solution_definition_name}}].get_project(pathname)
+    project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
     return f"Project Name: {project.project_display_name}"
 
 
-# this callback is essential for initializing the step based on the persisted
-# state of the project when the browser first displays the project to the user
-# given the project's URL
 @callback(
     Output("page-content", "children"),
     [
         Input("url", "pathname"),
         Input("navigation_tree", "focus"),
     ],
     prevent_initial_call=True,
 )
 def display_page(pathname, value):
-    """Display page content."""
+    """
+    Display page content.
+
+    this callback is essential for initializing the step based on the persisted
+    state of the project when the browser first displays the project to the user
+    given the project's URL
+    """
+
     project = DashClient[{{ cookiecutter.__solution_definition_name }}].get_project(pathname)
     triggered_id = callback_context.triggered[0]["prop_id"].split(".")[0]
+
     if triggered_id == "url":
-        return intro_page.layout(project.steps.intro_step)
+        return problem_setup_page.layout(project.steps.problem_setup_step)
     if triggered_id == "navigation_tree":
         if value is None:
             page_layout = html.H1("Welcome!")
-        elif value == "intro_step":
-            page_layout = intro_page.layout(project.steps.intro_step)
-        elif value == "first_step":
-            page_layout = first_page.layout(project.steps.first_step)
-        elif value == "second_step":
-            page_layout = second_page.layout(project.steps.second_step)
+        elif value == "problem_setup_step":
+            page_layout = problem_setup_page.layout(project.steps.problem_setup_step)
+        else:
+            node_info = extract_dict_by_key(step_list, "key", value, expect_unique=True)
+            page_layout = monitoring_page.layout(
+                project.steps.problem_setup_step, project.steps.monitoring_step, node_info
+            )
         return page_layout
```

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-0.9.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/testing.py` & `ansys_templates-0.9.0/src/ansys/templates/testing.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/src/ansys/templates/utils.py` & `ansys_templates-0.9.0/src/ansys/templates/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-0.8.0/PKG-INFO` & `ansys_templates-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-templates
-Version: 0.8.0
+Version: 0.9.0
 Summary: Creates Python projects according to PyAnsys guidelines
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -19,19 +19,19 @@
 Requires-Dist: click>=7.0,<8.0.0
 Requires-Dist: cookiecutter>=2.1.0
 Requires-Dist: isort>=5.10.1
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
-Requires-Dist: pytest==7.3.1 ; extra == "tests"
+Requires-Dist: pytest==7.3.2 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
 Project-URL: Documentation, https://templates.ansys.com/
 Project-URL: Homepage, https://templates.ansys.com/
-Project-URL: Source, https://github.com/ansys-templates/ansys-templates
+Project-URL: Source, https://github.com/ansys/ansys-templates
 Project-URL: Tracker, https://github.com/ansys/ansys-templates/issues
 Provides-Extra: doc
 Provides-Extra: tests
 
 .. Copyright (C) 2023 ANSYS, Inc. and/or its affiliates.
 .. SPDX-License-Identifier: MIT
 ..
```

