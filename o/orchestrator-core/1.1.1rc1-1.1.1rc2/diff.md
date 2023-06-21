# Comparing `tmp/orchestrator_core-1.1.1rc1.tar.gz` & `tmp/orchestrator_core-1.1.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrator_core-1.1.1rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orchestrator_core-1.1.1rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orchestrator_core-1.1.1rc1.tar` & `orchestrator_core-1.1.1rc2.tar`

### file list

```diff
@@ -1,374 +1,386 @@
--rw-r--r--   0        0        0      341 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.bumpversion.cfg
--rw-r--r--   0        0        0       33 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.coveragerc
--rw-r--r--   0        0        0     2620 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.github/workflows/README.md
--rw-r--r--   0        0        0     1851 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.github/workflows/build-push-container.yml
--rw-r--r--   0        0        0      291 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2341 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      371 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      550 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1163 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     2113 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1985 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1809 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.gitignore
--rw-r--r--   0        0        0     2099 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/.stignore
--rw-r--r--   0        0        0    29970 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/CHANGELOG.md
--rw-r--r--   0        0        0      333 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/Dockerfile
--rw-r--r--   0        0        0    11409 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/LICENSE
--rw-r--r--   0        0        0      150 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/NOTICE
--rw-r--r--   0        0        0     4965 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/README.md
--rw-r--r--   0        0        0       76 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/codecov.yml
--rw-r--r--   0        0        0       45 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/architecture/application/api.md
--rw-r--r--   0        0        0    16572 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/architecture/application/cli.md
--rw-r--r--   0        0        0    10741 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/architecture/application/domainmodels.md
--rw-r--r--   0        0        0    13931 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/architecture/application/forms.md
--rw-r--r--   0        0        0    48867 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/architecture/application/openapi.json
--rw-r--r--   0        0        0     1565 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/architecture/application/python.md
--rw-r--r--   0        0        0     5585 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/architecture/application/scaling.md
--rw-r--r--   0        0        0     5514 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/architecture/application/tasks.md
--rw-r--r--   0        0        0     2371 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/architecture/application/websockets.md
--rw-r--r--   0        0        0    11465 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/architecture/application/workflow.md
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/architecture/orchestration/philosophy.md
--rw-r--r--   0        0        0     2080 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/architecture/tldr.md
--rw-r--r--   0        0        0     1694 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/contributing/guidelines.md
--rw-r--r--   0        0        0    10000 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/contributing/testing.md
--rw-r--r--   0        0        0      452 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/css/custom.css
--rw-r--r--   0        0        0     2165 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/css/termynal.css
--rw-r--r--   0        0        0     2135 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/getting-started/base.md
--rw-r--r--   0        0        0      928 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/getting-started/development.md
--rw-r--r--   0        0        0     2367 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/index.md
--rw-r--r--   0        0        0     3897 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/js/termynal.js
--rw-r--r--   0        0        0     8925 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/advanced/circuit-workflow.md
--rw-r--r--   0        0        0      254 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/advanced/database-migration.md
--rw-r--r--   0        0        0     3776 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/advanced/docker-installation.md
--rw-r--r--   0        0        0     2563 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/advanced/domain-models.md
--rw-r--r--   0        0        0     4126 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/advanced/node-workflow.md
--rw-r--r--   0        0        0     3079 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/advanced/overview.md
--rw-r--r--   0        0        0     1750 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/advanced/scenario.md
--rw-r--r--   0        0        0     4369 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/advanced/workflow-introduction.md
--rw-r--r--   0        0        0     5605 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/create-user-group.md
--rw-r--r--   0        0        0     4438 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/create-user.md
--rw-r--r--   0        0        0     7471 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/database-migration.md
--rw-r--r--   0        0        0     3700 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/debian.md
--rw-r--r--   0        0        0     3063 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/docker.md
--rw-r--r--   0        0        0     6106 2023-06-14 08:33:47.109676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/domain-models.md
--rw-r--r--   0        0        0     1952 2023-06-14 08:33:47.113676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/explore.md
--rw-r--r--   0        0        0     3996 2023-06-14 08:33:47.113676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/input-forms.md
--rw-r--r--   0        0        0     3595 2023-06-14 08:33:47.113676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/macos.md
--rw-r--r--   0        0        0     3411 2023-06-14 08:33:47.113676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/modify-user-group.md
--rw-r--r--   0        0        0     2143 2023-06-14 08:33:47.113676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/modify-user.md
--rw-r--r--   0        0        0     2885 2023-06-14 08:33:47.113676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/overview.md
--rw-r--r--   0        0        0     4547 2023-06-14 08:33:47.113676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/register-workflows.md
--rw-r--r--   0        0        0      786 2023-06-14 08:33:47.113676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/scenario.md
--rw-r--r--   0        0        0     1013 2023-06-14 08:33:47.113676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/start-applications.md
--rw-r--r--   0        0        0     2988 2023-06-14 08:33:47.113676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/terminate-user-group.md
--rw-r--r--   0        0        0     1332 2023-06-14 08:33:47.113676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/terminate-user.md
--rw-r--r--   0        0        0     3637 2023-06-14 08:33:47.113676 orchestrator_core-1.1.1rc1/docs/workshops/beginner/workflow-introduction.md
--rw-r--r--   0        0        0    46296 2023-06-14 08:33:47.113676 orchestrator_core-1.1.1rc1/docs/workshops/images/metadata_products.png
--rw-r--r--   0        0        0   983304 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/docs/workshops/images/netbox_devices_active.png
--rw-r--r--   0        0        0      771 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/examples/basic/basic_orchestrator.py
--rw-r--r--   0        0        0     4214 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/mkdocs.yml
--rw-r--r--   0        0        0     1267 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/mutmut_config.py
--rw-r--r--   0        0        0     1098 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/__init__.py
--rw-r--r--   0        0        0      571 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/__init__.py
--rw-r--r--   0        0        0      571 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/__init__.py
--rw-r--r--   0        0        0     2871 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/api.py
--rw-r--r--   0        0        0      571 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     2841 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/fixed_input.py
--rw-r--r--   0        0        0     1236 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/health.py
--rw-r--r--   0        0        0    12955 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/processes.py
--rw-r--r--   0        0        0     2703 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/product_blocks.py
--rw-r--r--   0        0        0     3331 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/products.py
--rw-r--r--   0        0        0     2552 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/resource_types.py
--rw-r--r--   0        0        0     5803 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/settings.py
--rw-r--r--   0        0        0     2866 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
--rw-r--r--   0        0        0    11864 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/subscriptions.py
--rw-r--r--   0        0        0      996 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/translations.py
--rw-r--r--   0        0        0     1833 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/user.py
--rw-r--r--   0        0        0     1961 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/workflows.py
--rw-r--r--   0        0        0     1543 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/error_handling.py
--rw-r--r--   0        0        0    11705 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/helpers.py
--rw-r--r--   0        0        0     5636 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/api/models.py
--rw-r--r--   0        0        0     7395 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/app.py
--rw-r--r--   0        0        0      571 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0    13831 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/cli/database.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/cli/domain_gen_helpers/__init__.py
--rw-r--r--   0        0        0     6853 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
--rw-r--r--   0        0        0     1953 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/cli/domain_gen_helpers/helpers.py
--rw-r--r--   0        0        0    10653 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
--rw-r--r--   0        0        0     9423 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py
--rw-r--r--   0        0        0    24095 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
--rw-r--r--   0        0        0     1439 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/cli/domain_gen_helpers/types.py
--rw-r--r--   0        0        0     2371 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/cli/generate.md
--rw-r--r--   0        0        0     5168 2023-06-14 08:33:47.117676 orchestrator_core-1.1.1rc1/orchestrator/cli/generate.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/__init__.py
--rw-r--r--   0        0        0     1758 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/fixed_input.py
--rw-r--r--   0        0        0     2626 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/helpers.py
--rw-r--r--   0        0        0     2607 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/migration.py
--rw-r--r--   0        0        0     2152 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/product.py
--rw-r--r--   0        0        0     5811 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/product_block.py
--rw-r--r--   0        0        0     1400 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/settings.py
--rw-r--r--   0        0        0     1794 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/translations.py
--rw-r--r--   0        0        0     4234 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/unittest.py
--rw-r--r--   0        0        0     1957 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/validations.py
--rw-r--r--   0        0        0     6559 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/workflow.py
--rw-r--r--   0        0        0      779 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/products/workshop/circuit.yaml
--rw-r--r--   0        0        0      557 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/products/workshop/node.yaml
--rw-r--r--   0        0        0      553 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/products/workshop/user.yaml
--rw-r--r--   0        0        0      380 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/products/workshop/user_group.yaml
--rw-r--r--   0        0        0      289 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/constrained_int_definitions.j2
--rw-r--r--   0        0        0     4196 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/create_product.j2
--rw-r--r--   0        0        0      337 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/list_definitions.j2
--rw-r--r--   0        0        0      520 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/macros.j2
--rw-r--r--   0        0        0     4405 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/modify_product.j2
--rw-r--r--   0        0        0     2639 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/new_product_migration.j2
--rw-r--r--   0        0        0     1675 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/product.j2
--rw-r--r--   0        0        0     2275 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/product_block.j2
--rw-r--r--   0        0        0      514 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/shared_forms.j2
--rw-r--r--   0        0        0     2808 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/terminate_product.j2
--rw-r--r--   0        0        0     1764 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/test_create_workflow.j2
--rw-r--r--   0        0        0     1689 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/test_modify_workflow.j2
--rw-r--r--   0        0        0     1860 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/test_product_type.j2
--rw-r--r--   0        0        0     1518 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/test_terminate_workflow.j2
--rw-r--r--   0        0        0      984 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/test_validate_workflow.j2
--rw-r--r--   0        0        0     2391 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/validate_product.j2
--rw-r--r--   0        0        0      571 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1165 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/helpers/input_helpers.py
--rw-r--r--   0        0        0      830 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/helpers/print_helpers.py
--rw-r--r--   0        0        0      983 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/main.py
--rwxr-xr-x   0        0        0    20183 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/migrate_domain_models.py
--rwxr-xr-x   0        0        0     8943 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/migrate_workflows.py
--rw-r--r--   0        0        0     4113 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/migration_helpers.py
--rw-r--r--   0        0        0     1896 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/cli/scheduler.py
--rw-r--r--   0        0        0      571 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/config/__init__.py
--rw-r--r--   0        0        0      770 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/config/assignee.py
--rw-r--r--   0        0        0     2984 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/db/__init__.py
--rw-r--r--   0        0        0    10288 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/db/database.py
--rw-r--r--   0        0        0      301 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/db/filters/__init__.py
--rw-r--r--   0        0        0     3415 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/db/filters/filters.py
--rw-r--r--   0        0        0     4507 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/db/filters/process.py
--rw-r--r--   0        0        0     1924 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/db/filters/product.py
--rw-r--r--   0        0        0    23603 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/db/models.py
--rw-r--r--   0        0        0      104 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/db/range/__init__.py
--rw-r--r--   0        0        0     1439 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/db/range/range.py
--rw-r--r--   0        0        0      240 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/db/sorting/__init__.py
--rw-r--r--   0        0        0      368 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/db/sorting/process.py
--rw-r--r--   0        0        0      346 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/db/sorting/product.py
--rw-r--r--   0        0        0     3413 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/db/sorting/sorting.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/devtools/__init__.py
--rw-r--r--   0        0        0    16866 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/devtools/populator.py
--rw-r--r--   0        0        0     2508 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/distlock/__init__.py
--rw-r--r--   0        0        0     2533 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/distlock/distlock_manager.py
--rw-r--r--   0        0        0      571 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/distlock/managers/__init__.py
--rw-r--r--   0        0        0     3062 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/distlock/managers/memory_distlock_manager.py
--rw-r--r--   0        0        0     3329 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/distlock/managers/redis_distlock_manager.py
--rw-r--r--   0        0        0      924 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/domain/__init__.py
--rw-r--r--   0        0        0    62844 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/domain/base.py
--rw-r--r--   0        0        0     2694 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/domain/lifecycle.py
--rw-r--r--   0        0        0     2977 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/exception_handlers.py
--rw-r--r--   0        0        0     5434 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/forms/__init__.py
--rw-r--r--   0        0        0     2145 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/forms/network_type_validators.py
--rw-r--r--   0        0        0    11483 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/forms/validators.py
--rw-r--r--   0        0        0     5091 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/__init__.py
--rw-r--r--   0        0        0     1350 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/extensions/ErrorCollectorExtension.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/extensions/__init__.py
--rw-r--r--   0        0        0     4325 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py
--rw-r--r--   0        0        0     2105 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/pagination.py
--rw-r--r--   0        0        0      317 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/resolvers/__init__.py
--rw-r--r--   0        0        0     4097 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/resolvers/process.py
--rw-r--r--   0        0        0     2576 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/resolvers/product.py
--rw-r--r--   0        0        0     3727 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/resolvers/settings.py
--rw-r--r--   0        0        0      203 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/schemas/errors.py
--rw-r--r--   0        0        0      513 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/schemas/fixed_input.py
--rw-r--r--   0        0        0     2259 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/schemas/process.py
--rw-r--r--   0        0        0      690 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/schemas/product.py
--rw-r--r--   0        0        0      530 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/schemas/product_block.py
--rw-r--r--   0        0        0      305 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/schemas/resource_type.py
--rw-r--r--   0        0        0      980 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/schemas/settings.py
--rw-r--r--   0        0        0      172 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/schemas/workflow.py
--rw-r--r--   0        0        0     2056 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/types.py
--rw-r--r--   0        0        0      114 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/utils/__init__.py
--rw-r--r--   0        0        0      992 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/graphql/utils/get_selected_fields.py
--rw-r--r--   0        0        0       39 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/migrations/README
--rw-r--r--   0        0        0      873 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/migrations/alembic.ini
--rwxr-xr-x   0        0        0     3365 2023-06-14 08:33:47.121676 orchestrator_core-1.1.1rc1/orchestrator/migrations/env.py
--rw-r--r--   0        0        0    40397 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/helpers.py
--rw-r--r--   0        0        0      510 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/script.py.mako
--rw-r--r--   0        0        0      905 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/templates/alembic.ini.j2
--rwxr-xr-x   0        0        0     2821 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/templates/env.py.j2
--rw-r--r--   0        0        0       98 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/templates/helpers.py.j2
--rw-r--r--   0        0        0     2641 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
--rw-r--r--   0        0        0     1266 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
--rw-r--r--   0        0        0    38591 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
--rw-r--r--   0        0        0      951 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
--rw-r--r--   0        0        0     1213 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
--rw-r--r--   0        0        0     1556 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
--rw-r--r--   0        0        0     5105 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
--rw-r--r--   0        0        0     7723 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
--rw-r--r--   0        0        0      989 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/py.typed
--rw-r--r--   0        0        0     1090 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schedules/__init__.py
--rw-r--r--   0        0        0      832 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schedules/resume_workflows.py
--rw-r--r--   0        0        0     1535 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schedules/scheduling.py
--rw-r--r--   0        0        0      821 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schedules/task_vacuum.py
--rw-r--r--   0        0        0     1053 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schedules/validate_products.py
--rw-r--r--   0        0        0     2131 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schedules/validate_subscriptions.py
--rw-r--r--   0        0        0     2631 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schemas/__init__.py
--rw-r--r--   0        0        0      886 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schemas/base.py
--rw-r--r--   0        0        0     1293 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schemas/engine_settings.py
--rw-r--r--   0        0        0     1346 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schemas/fixed_input.py
--rw-r--r--   0        0        0      842 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schemas/problem_detail.py
--rw-r--r--   0        0        0     3390 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schemas/process.py
--rw-r--r--   0        0        0     1670 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schemas/product.py
--rw-r--r--   0        0        0     1735 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schemas/product_block.py
--rw-r--r--   0        0        0      951 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schemas/resource_type.py
--rw-r--r--   0        0        0     3180 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schemas/subscription.py
--rw-r--r--   0        0        0     1013 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schemas/subscription_descriptions.py
--rw-r--r--   0        0        0     1803 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/schemas/workflow.py
--rw-r--r--   0        0        0     1797 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/security.py
--rw-r--r--   0        0        0      571 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/services/__init__.py
--rw-r--r--   0        0        0     3586 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/services/celery.py
--rw-r--r--   0        0        0    22605 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/services/processes.py
--rw-r--r--   0        0        0     1530 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/services/products.py
--rw-r--r--   0        0        0     3879 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/services/settings.py
--rw-r--r--   0        0        0    24525 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/services/subscriptions.py
--rw-r--r--   0        0        0     5708 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/services/tasks.py
--rw-r--r--   0        0        0     1719 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/services/translations.py
--rw-r--r--   0        0        0     3708 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/settings.py
--rw-r--r--   0        0        0      766 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/targets.py
--rw-r--r--   0        0        0     9397 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/types.py
--rw-r--r--   0        0        0      571 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/__init__.py
--rw-r--r--   0        0        0     5593 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/crypt.py
--rw-r--r--   0        0        0     1477 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/datetime.py
--rw-r--r--   0        0        0     6207 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/docs.py
--rw-r--r--   0        0        0     3839 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/errors.py
--rw-r--r--   0        0        0     8079 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/functional.py
--rw-r--r--   0        0        0     2785 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/helpers.py
--rw-r--r--   0        0        0     8512 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/json.py
--rw-r--r--   0        0        0     3376 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/redis.py
--rw-r--r--   0        0        0     2972 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/show_process.py
--rw-r--r--   0        0        0     2395 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/speed.py
--rw-r--r--   0        0        0    13148 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/state.py
--rw-r--r--   0        0        0     1077 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/strings.py
--rw-r--r--   0        0        0     7231 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/utils/vlans.py
--rw-r--r--   0        0        0     1323 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/version.py
--rw-r--r--   0        0        0     4476 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/websocket/__init__.py
--rw-r--r--   0        0        0     3535 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py
--rw-r--r--   0        0        0     3312 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/websocket/managers/memory_websocket_manager.py
--rw-r--r--   0        0        0     2900 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/websocket/websocket_manager.py
--rw-r--r--   0        0        0    33615 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/workflow.py
--rw-r--r--   0        0        0     4085 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2135 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/workflows/modify_note.py
--rw-r--r--   0        0        0      909 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/workflows/removed_workflow.py
--rw-r--r--   0        0        0     9204 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/workflows/steps.py
--rw-r--r--   0        0        0      571 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     1510 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py
--rw-r--r--   0        0        0     2120 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/workflows/tasks/resume_workflows.py
--rw-r--r--   0        0        0     8335 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/workflows/tasks/validate_products.py
--rw-r--r--   0        0        0      684 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/workflows/translations/en-GB.json
--rw-r--r--   0        0        0    12830 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/orchestrator/workflows/utils.py
--rw-r--r--   0        0        0     4593 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/pyproject.toml
--rw-r--r--   0        0        0     2413 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/setup.cfg
--rw-r--r--   0        0        0      665 2023-06-14 08:33:47.125676 orchestrator_core-1.1.1rc1/setup.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/acceptance_tests/__init__.py
--rw-r--r--   0        0        0     3199 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/acceptance_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
--rw-r--r--   0        0        0     1855 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
--rw-r--r--   0        0        0     1544 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
--rw-r--r--   0        0        0     1608 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2828 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
--rw-r--r--   0        0        0      588 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/acceptance_tests/test_test_product.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/__init__.py
--rw-r--r--   0        0        0     5159 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_caching.py
--rw-r--r--   0        0        0     1578 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_fixed_inputs.py
--rw-r--r--   0        0        0     1192 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_health.py
--rw-r--r--   0        0        0     3049 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_helpers.py
--rw-r--r--   0        0        0     1747 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_models.py
--rw-r--r--   0        0        0    20143 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_processes.py
--rw-r--r--   0        0        0    16019 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_processes_ws.py
--rw-r--r--   0        0        0     3742 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_product_blocks.py
--rw-r--r--   0        0        0     7942 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_products.py
--rw-r--r--   0        0        0     2486 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_resource_types.py
--rw-r--r--   0        0        0     1772 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_settings.py
--rw-r--r--   0        0        0     2985 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_subscription_customer_descriptions.py
--rw-r--r--   0        0        0    37706 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_subscriptions.py
--rw-r--r--   0        0        0     2367 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/api/test_workflows.py
--rw-r--r--   0        0        0    25724 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
--rw-r--r--   0        0        0    27170 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
--rw-r--r--   0        0        0      511 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/config.py
--rw-r--r--   0        0        0    21642 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/domain/__init__.py
--rw-r--r--   0        0        0    50537 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/domain/test_base.py
--rw-r--r--   0        0        0     8092 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/domain/test_base_with_list_union.py
--rw-r--r--   0        0        0     4493 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/domain/test_base_with_union.py
--rw-r--r--   0        0        0     2824 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/__init__.py
--rw-r--r--   0        0        0     7530 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/processes.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1683 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
--rw-r--r--   0        0        0     2569 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
--rw-r--r--   0        0        0     1609 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
--rw-r--r--   0        0        0     2642 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
--rw-r--r--   0        0        0     2590 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
--rw-r--r--   0        0        0     1232 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
--rw-r--r--   0        0        0     1055 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/__init__.py
--rw-r--r--   0        0        0     2372 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
--rw-r--r--   0        0        0     2262 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
--rw-r--r--   0        0        0     4191 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
--rw-r--r--   0        0        0     3240 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py
--rw-r--r--   0        0        0     2341 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
--rw-r--r--   0        0        0     2977 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
--rw-r--r--   0        0        0     2298 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
--rw-r--r--   0        0        0     2282 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
--rw-r--r--   0        0        0     1671 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
--rw-r--r--   0        0        0     1898 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py
--rw-r--r--   0        0        0      527 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/resource_types.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/forms/__init__.py
--rw-r--r--   0        0        0     1462 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/forms/shared.py
--rw-r--r--   0        0        0    25426 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/forms/test_generic_validators.py
--rw-r--r--   0        0        0     7644 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/forms/test_network_validators.py
--rw-r--r--   0        0        0     6626 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/forms/test_post_process.py
--rw-r--r--   0        0        0    10123 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/graphql/test_processes.py
--rw-r--r--   0        0        0     4594 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/graphql/test_product.py
--rw-r--r--   0        0        0     5174 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/graphql/test_settings.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/schedules/__init__.py
--rw-r--r--   0        0        0      807 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/schedules/test_scheduling.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/services/__init__.py
--rw-r--r--   0        0        0    26695 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/services/test_processes.py
--rw-r--r--   0        0        0     1083 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/services/test_products.py
--rw-r--r--   0        0        0     5830 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/services/test_subscriptions.py
--rw-r--r--   0        0        0     2100 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/services/test_translations.py
--rw-r--r--   0        0        0     7353 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/test_db.py
--rw-r--r--   0        0        0      385 2023-06-14 08:33:47.129676 orchestrator_core-1.1.1rc1/test/unit_tests/test_types.py
--rw-r--r--   0        0        0    12048 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/test_workflow.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/utils/__init__.py
--rw-r--r--   0        0        0      163 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1871 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_errors.py
--rw-r--r--   0        0        0     3517 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_functional.py
--rw-r--r--   0        0        0     3052 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_json.py
--rw-r--r--   0        0        0     1144 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_speed.py
--rw-r--r--   0        0        0    11501 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_state.py
--rw-r--r--   0        0        0      192 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_strings.py
--rw-r--r--   0        0        0     8339 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_vlans.py
--rw-r--r--   0        0        0    12492 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/workflows/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/workflows/conftest.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/workflows/shared/__init__.py
--rw-r--r--   0        0        0     2091 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py
--rw-r--r--   0        0        0        0 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     2039 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
--rw-r--r--   0        0        0     2584 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py
--rw-r--r--   0        0        0      288 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/workflows/tasks/test_validate_products.py
--rw-r--r--   0        0        0     3390 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/workflows/test_config_db_code.py
--rw-r--r--   0        0        0     1877 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/workflows/test_generic_workflow_steps.py
--rw-r--r--   0        0        0      987 2023-06-14 08:33:47.133676 orchestrator_core-1.1.1rc1/test/unit_tests/workflows/test_modify_note.py
--rw-r--r--   0        0        0     5331 1970-01-01 00:00:00.000000 orchestrator_core-1.1.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      341 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.bumpversion.cfg
+-rw-r--r--   0        0        0       33 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.coveragerc
+-rw-r--r--   0        0        0     2620 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/README.md
+-rw-r--r--   0        0        0     1851 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/build-push-container.yml
+-rw-r--r--   0        0        0      291 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2341 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      371 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      550 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1163 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     2113 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1985 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1809 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.gitignore
+-rw-r--r--   0        0        0     2099 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.stignore
+-rw-r--r--   0        0        0    29970 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/Dockerfile
+-rw-r--r--   0        0        0    11409 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/LICENSE
+-rw-r--r--   0        0        0      150 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/NOTICE
+-rw-r--r--   0        0        0     4965 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/README.md
+-rw-r--r--   0        0        0       76 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/codecov.yml
+-rw-r--r--   0        0        0       45 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/api.md
+-rw-r--r--   0        0        0    16572 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/cli.md
+-rw-r--r--   0        0        0    10741 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/domainmodels.md
+-rw-r--r--   0        0        0    13931 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/forms.md
+-rw-r--r--   0        0        0    48867 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/openapi.json
+-rw-r--r--   0        0        0     1565 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/python.md
+-rw-r--r--   0        0        0     5585 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/scaling.md
+-rw-r--r--   0        0        0     5514 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/tasks.md
+-rw-r--r--   0        0        0     2371 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/websockets.md
+-rw-r--r--   0        0        0    11465 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/workflow.md
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/orchestration/philosophy.md
+-rw-r--r--   0        0        0     2080 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/tldr.md
+-rw-r--r--   0        0        0     1694 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/contributing/guidelines.md
+-rw-r--r--   0        0        0    10000 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/contributing/testing.md
+-rw-r--r--   0        0        0      452 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/css/custom.css
+-rw-r--r--   0        0        0     2165 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/css/termynal.css
+-rw-r--r--   0        0        0     2135 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/getting-started/base.md
+-rw-r--r--   0        0        0      928 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/getting-started/development.md
+-rw-r--r--   0        0        0     2367 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/index.md
+-rw-r--r--   0        0        0     3897 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/js/termynal.js
+-rw-r--r--   0        0        0     8925 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/circuit-workflow.md
+-rw-r--r--   0        0        0      254 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/database-migration.md
+-rw-r--r--   0        0        0     3776 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/docker-installation.md
+-rw-r--r--   0        0        0     2563 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/domain-models.md
+-rw-r--r--   0        0        0     4126 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/node-workflow.md
+-rw-r--r--   0        0        0     3079 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/overview.md
+-rw-r--r--   0        0        0     1750 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/scenario.md
+-rw-r--r--   0        0        0     4369 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/workflow-introduction.md
+-rw-r--r--   0        0        0     5605 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/create-user-group.md
+-rw-r--r--   0        0        0     4438 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/create-user.md
+-rw-r--r--   0        0        0     7471 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/database-migration.md
+-rw-r--r--   0        0        0     3700 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/debian.md
+-rw-r--r--   0        0        0     3063 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/docker.md
+-rw-r--r--   0        0        0     6106 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/domain-models.md
+-rw-r--r--   0        0        0     1952 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/explore.md
+-rw-r--r--   0        0        0     3996 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/input-forms.md
+-rw-r--r--   0        0        0     3595 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/macos.md
+-rw-r--r--   0        0        0     3411 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/modify-user-group.md
+-rw-r--r--   0        0        0     2143 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/modify-user.md
+-rw-r--r--   0        0        0     2885 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/overview.md
+-rw-r--r--   0        0        0     4547 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/register-workflows.md
+-rw-r--r--   0        0        0      786 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/scenario.md
+-rw-r--r--   0        0        0     1013 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/start-applications.md
+-rw-r--r--   0        0        0     2988 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/terminate-user-group.md
+-rw-r--r--   0        0        0     1332 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/terminate-user.md
+-rw-r--r--   0        0        0     3637 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/workflow-introduction.md
+-rw-r--r--   0        0        0    46296 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/images/metadata_products.png
+-rw-r--r--   0        0        0   983304 2023-06-21 12:35:30.027623 orchestrator_core-1.1.1rc2/docs/workshops/images/netbox_devices_active.png
+-rw-r--r--   0        0        0      771 2023-06-21 12:35:30.027623 orchestrator_core-1.1.1rc2/examples/basic/basic_orchestrator.py
+-rw-r--r--   0        0        0     4214 2023-06-21 12:35:30.027623 orchestrator_core-1.1.1rc2/mkdocs.yml
+-rw-r--r--   0        0        0     1267 2023-06-21 12:35:30.027623 orchestrator_core-1.1.1rc2/mutmut_config.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.027623 orchestrator_core-1.1.1rc2/orchestrator/.stignore
+-rw-r--r--   0        0        0     1098 2023-06-21 12:35:30.027623 orchestrator_core-1.1.1rc2/orchestrator/__init__.py
+-rw-r--r--   0        0        0      571 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/__init__.py
+-rw-r--r--   0        0        0      571 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     2871 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/api.py
+-rw-r--r--   0        0        0      571 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     2841 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/fixed_input.py
+-rw-r--r--   0        0        0     1236 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/health.py
+-rw-r--r--   0        0        0    12955 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/processes.py
+-rw-r--r--   0        0        0     2703 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/product_blocks.py
+-rw-r--r--   0        0        0     3331 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/products.py
+-rw-r--r--   0        0        0     2552 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/resource_types.py
+-rw-r--r--   0        0        0     5803 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/settings.py
+-rw-r--r--   0        0        0     2866 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    11864 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/subscriptions.py
+-rw-r--r--   0        0        0      996 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/translations.py
+-rw-r--r--   0        0        0     1833 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/user.py
+-rw-r--r--   0        0        0     1961 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/workflows.py
+-rw-r--r--   0        0        0     1543 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/error_handling.py
+-rw-r--r--   0        0        0    11705 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/helpers.py
+-rw-r--r--   0        0        0     5636 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/models.py
+-rw-r--r--   0        0        0     7395 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/app.py
+-rw-r--r--   0        0        0      571 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0    13831 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/database.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/__init__.py
+-rw-r--r--   0        0        0     6853 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
+-rw-r--r--   0        0        0     1953 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/helpers.py
+-rw-r--r--   0        0        0    10653 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
+-rw-r--r--   0        0        0     9423 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py
+-rw-r--r--   0        0        0    24095 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
+-rw-r--r--   0        0        0     1439 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/types.py
+-rw-r--r--   0        0        0     2371 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generate.md
+-rw-r--r--   0        0        0     5168 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generate.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/__init__.py
+-rw-r--r--   0        0        0     1758 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/fixed_input.py
+-rw-r--r--   0        0        0     2626 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/helpers.py
+-rw-r--r--   0        0        0     2607 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/migration.py
+-rw-r--r--   0        0        0     2152 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/product.py
+-rw-r--r--   0        0        0     5811 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/product_block.py
+-rw-r--r--   0        0        0     1400 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/settings.py
+-rw-r--r--   0        0        0     1794 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/translations.py
+-rw-r--r--   0        0        0     4234 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/unittest.py
+-rw-r--r--   0        0        0     1957 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/validations.py
+-rw-r--r--   0        0        0     6559 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/workflow.py
+-rw-r--r--   0        0        0      779 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/circuit.yaml
+-rw-r--r--   0        0        0      557 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/node.yaml
+-rw-r--r--   0        0        0      553 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/user.yaml
+-rw-r--r--   0        0        0      380 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/user_group.yaml
+-rw-r--r--   0        0        0      289 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/constrained_int_definitions.j2
+-rw-r--r--   0        0        0     4196 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/create_product.j2
+-rw-r--r--   0        0        0      337 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/list_definitions.j2
+-rw-r--r--   0        0        0      520 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/macros.j2
+-rw-r--r--   0        0        0     4405 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/modify_product.j2
+-rw-r--r--   0        0        0     2639 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/new_product_migration.j2
+-rw-r--r--   0        0        0     1675 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/product.j2
+-rw-r--r--   0        0        0     2275 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/product_block.j2
+-rw-r--r--   0        0        0      514 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/shared_forms.j2
+-rw-r--r--   0        0        0     2808 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/terminate_product.j2
+-rw-r--r--   0        0        0     1764 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_create_workflow.j2
+-rw-r--r--   0        0        0     1689 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_modify_workflow.j2
+-rw-r--r--   0        0        0     1860 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_product_type.j2
+-rw-r--r--   0        0        0     1518 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_terminate_workflow.j2
+-rw-r--r--   0        0        0      984 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_validate_workflow.j2
+-rw-r--r--   0        0        0     2391 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/validate_product.j2
+-rw-r--r--   0        0        0      571 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1165 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/helpers/input_helpers.py
+-rw-r--r--   0        0        0      830 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/helpers/print_helpers.py
+-rw-r--r--   0        0        0      983 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/main.py
+-rwxr-xr-x   0        0        0    20183 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/migrate_domain_models.py
+-rwxr-xr-x   0        0        0     8943 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/migrate_workflows.py
+-rw-r--r--   0        0        0     4113 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/migration_helpers.py
+-rw-r--r--   0        0        0     1896 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/scheduler.py
+-rw-r--r--   0        0        0      571 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/config/__init__.py
+-rw-r--r--   0        0        0      770 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/config/assignee.py
+-rw-r--r--   0        0        0     2984 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0    10288 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/database.py
+-rw-r--r--   0        0        0      303 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/__init__.py
+-rw-r--r--   0        0        0     3618 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/filters.py
+-rw-r--r--   0        0        0      774 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/__init__.py
+-rw-r--r--   0        0        0      992 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/bool_filter.py
+-rw-r--r--   0        0        0      952 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/is_like_filter.py
+-rw-r--r--   0        0        0     2542 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/range_filter.py
+-rw-r--r--   0        0        0      993 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/values_in_column_filter.py
+-rw-r--r--   0        0        0     3592 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/process.py
+-rw-r--r--   0        0        0     1251 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/product.py
+-rw-r--r--   0        0        0     3203 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/subscription.py
+-rw-r--r--   0        0        0    23630 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/models.py
+-rw-r--r--   0        0        0      104 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/range/__init__.py
+-rw-r--r--   0        0        0     1439 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/range/range.py
+-rw-r--r--   0        0        0      419 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/sorting/__init__.py
+-rw-r--r--   0        0        0      603 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/sorting/process.py
+-rw-r--r--   0        0        0      418 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/db/sorting/product.py
+-rw-r--r--   0        0        0     4427 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/db/sorting/sorting.py
+-rw-r--r--   0        0        0      606 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/db/sorting/subscription.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/devtools/__init__.py
+-rw-r--r--   0        0        0    16866 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/devtools/populator.py
+-rw-r--r--   0        0        0     2508 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/distlock/__init__.py
+-rw-r--r--   0        0        0     2533 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/distlock/distlock_manager.py
+-rw-r--r--   0        0        0      571 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/distlock/managers/__init__.py
+-rw-r--r--   0        0        0     3062 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/distlock/managers/memory_distlock_manager.py
+-rw-r--r--   0        0        0     3329 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/distlock/managers/redis_distlock_manager.py
+-rw-r--r--   0        0        0      924 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/domain/__init__.py
+-rw-r--r--   0        0        0    62844 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/domain/base.py
+-rw-r--r--   0        0        0     2694 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/domain/lifecycle.py
+-rw-r--r--   0        0        0     2977 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/exception_handlers.py
+-rw-r--r--   0        0        0     5434 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/forms/__init__.py
+-rw-r--r--   0        0        0     2145 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/forms/network_type_validators.py
+-rw-r--r--   0        0        0    11483 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/forms/validators.py
+-rw-r--r--   0        0        0     5373 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/extensions/__init__.py
+-rw-r--r--   0        0        0     4325 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py
+-rw-r--r--   0        0        0     1777 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/extensions/error_collector_extension.py
+-rw-r--r--   0        0        0     2334 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/pagination.py
+-rw-r--r--   0        0        0      420 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/__init__.py
+-rw-r--r--   0        0        0     3674 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/process.py
+-rw-r--r--   0        0        0     2154 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/product.py
+-rw-r--r--   0        0        0     3727 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/settings.py
+-rw-r--r--   0        0        0     2907 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/subscription.py
+-rw-r--r--   0        0        0      203 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/errors.py
+-rw-r--r--   0        0        0      513 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/fixed_input.py
+-rw-r--r--   0        0        0     3674 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/process.py
+-rw-r--r--   0        0        0     1776 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/product.py
+-rw-r--r--   0        0        0      530 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/product_block.py
+-rw-r--r--   0        0        0      305 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/resource_type.py
+-rw-r--r--   0        0        0      980 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/settings.py
+-rw-r--r--   0        0        0     7736 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/subscription.py
+-rw-r--r--   0        0        0      172 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/workflow.py
+-rw-r--r--   0        0        0     1789 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/types.py
+-rw-r--r--   0        0        0      114 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/utils/__init__.py
+-rw-r--r--   0        0        0     1071 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/utils/create_resolver_error_handler.py
+-rw-r--r--   0        0        0      992 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/utils/get_selected_fields.py
+-rw-r--r--   0        0        0       39 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/README
+-rw-r--r--   0        0        0      873 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/alembic.ini
+-rwxr-xr-x   0        0        0     3365 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/env.py
+-rw-r--r--   0        0        0    40397 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/script.py.mako
+-rw-r--r--   0        0        0      905 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/templates/alembic.ini.j2
+-rwxr-xr-x   0        0        0     2821 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/templates/env.py.j2
+-rw-r--r--   0        0        0       98 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/templates/helpers.py.j2
+-rw-r--r--   0        0        0     2641 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
+-rw-r--r--   0        0        0     1266 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
+-rw-r--r--   0        0        0    38591 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
+-rw-r--r--   0        0        0      951 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
+-rw-r--r--   0        0        0     1213 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
+-rw-r--r--   0        0        0     1556 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
+-rw-r--r--   0        0        0     5105 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
+-rw-r--r--   0        0        0     7723 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
+-rw-r--r--   0        0        0      989 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/py.typed
+-rw-r--r--   0        0        0     1090 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schedules/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schedules/resume_workflows.py
+-rw-r--r--   0        0        0     1535 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schedules/scheduling.py
+-rw-r--r--   0        0        0      821 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schedules/task_vacuum.py
+-rw-r--r--   0        0        0     1053 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schedules/validate_products.py
+-rw-r--r--   0        0        0     2131 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schedules/validate_subscriptions.py
+-rw-r--r--   0        0        0     2631 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/__init__.py
+-rw-r--r--   0        0        0      886 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/base.py
+-rw-r--r--   0        0        0     1293 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/engine_settings.py
+-rw-r--r--   0        0        0     1346 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/fixed_input.py
+-rw-r--r--   0        0        0      842 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/problem_detail.py
+-rw-r--r--   0        0        0     3390 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/process.py
+-rw-r--r--   0        0        0     1670 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/product.py
+-rw-r--r--   0        0        0     1735 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/product_block.py
+-rw-r--r--   0        0        0      951 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/resource_type.py
+-rw-r--r--   0        0        0     3180 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/subscription.py
+-rw-r--r--   0        0        0     1013 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/subscription_descriptions.py
+-rw-r--r--   0        0        0     1803 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/workflow.py
+-rw-r--r--   0        0        0     1797 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/security.py
+-rw-r--r--   0        0        0      571 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0     3586 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/services/celery.py
+-rw-r--r--   0        0        0    22605 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/services/processes.py
+-rw-r--r--   0        0        0     1530 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/services/products.py
+-rw-r--r--   0        0        0     3879 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/services/settings.py
+-rw-r--r--   0        0        0    24525 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/services/subscriptions.py
+-rw-r--r--   0        0        0     5708 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/services/tasks.py
+-rw-r--r--   0        0        0     1719 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/services/translations.py
+-rw-r--r--   0        0        0     3708 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/settings.py
+-rw-r--r--   0        0        0      766 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/targets.py
+-rw-r--r--   0        0        0     9449 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/types.py
+-rw-r--r--   0        0        0      571 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/__init__.py
+-rw-r--r--   0        0        0     5593 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/crypt.py
+-rw-r--r--   0        0        0     1477 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/datetime.py
+-rw-r--r--   0        0        0     6207 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/docs.py
+-rw-r--r--   0        0        0     3839 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/errors.py
+-rw-r--r--   0        0        0     8079 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/functional.py
+-rw-r--r--   0        0        0     2785 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/helpers.py
+-rw-r--r--   0        0        0     8512 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/json.py
+-rw-r--r--   0        0        0     3376 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/redis.py
+-rw-r--r--   0        0        0     2972 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/show_process.py
+-rw-r--r--   0        0        0     2395 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/speed.py
+-rw-r--r--   0        0        0    13148 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/state.py
+-rw-r--r--   0        0        0     1077 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/strings.py
+-rw-r--r--   0        0        0     7231 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/vlans.py
+-rw-r--r--   0        0        0     1323 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/version.py
+-rw-r--r--   0        0        0     4476 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/websocket/__init__.py
+-rw-r--r--   0        0        0     3535 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py
+-rw-r--r--   0        0        0     3312 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/websocket/managers/memory_websocket_manager.py
+-rw-r--r--   0        0        0     2900 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/websocket/websocket_manager.py
+-rw-r--r--   0        0        0    33615 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflow.py
+-rw-r--r--   0        0        0     4085 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2135 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/modify_note.py
+-rw-r--r--   0        0        0      909 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/removed_workflow.py
+-rw-r--r--   0        0        0     9204 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/steps.py
+-rw-r--r--   0        0        0      571 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     1510 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py
+-rw-r--r--   0        0        0     2120 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/resume_workflows.py
+-rw-r--r--   0        0        0     8335 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/validate_products.py
+-rw-r--r--   0        0        0      684 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/translations/en-GB.json
+-rw-r--r--   0        0        0    12830 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/utils.py
+-rw-r--r--   0        0        0     4618 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/pyproject.toml
+-rw-r--r--   0        0        0     2413 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/setup.cfg
+-rw-r--r--   0        0        0      665 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/setup.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/__init__.py
+-rw-r--r--   0        0        0     3199 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
+-rw-r--r--   0        0        0     1855 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
+-rw-r--r--   0        0        0     1544 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1608 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2828 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
+-rw-r--r--   0        0        0      588 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/test_test_product.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0     5159 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_caching.py
+-rw-r--r--   0        0        0     1578 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_fixed_inputs.py
+-rw-r--r--   0        0        0     1192 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_health.py
+-rw-r--r--   0        0        0     3049 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_helpers.py
+-rw-r--r--   0        0        0     1747 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_models.py
+-rw-r--r--   0        0        0    19964 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_processes.py
+-rw-r--r--   0        0        0    16019 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_processes_ws.py
+-rw-r--r--   0        0        0     3742 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_product_blocks.py
+-rw-r--r--   0        0        0     7942 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_products.py
+-rw-r--r--   0        0        0     2486 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_resource_types.py
+-rw-r--r--   0        0        0     1772 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_settings.py
+-rw-r--r--   0        0        0     2985 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    37706 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_subscriptions.py
+-rw-r--r--   0        0        0     2367 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_workflows.py
+-rw-r--r--   0        0        0    25724 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
+-rw-r--r--   0        0        0    27170 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
+-rw-r--r--   0        0        0      511 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/config.py
+-rw-r--r--   0        0        0    22649 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/domain/__init__.py
+-rw-r--r--   0        0        0    50537 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/domain/test_base.py
+-rw-r--r--   0        0        0     8092 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/domain/test_base_with_list_union.py
+-rw-r--r--   0        0        0     4493 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/domain/test_base_with_union.py
+-rw-r--r--   0        0        0     2824 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     7530 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/processes.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1683 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
+-rw-r--r--   0        0        0     2569 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
+-rw-r--r--   0        0        0     1609 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
+-rw-r--r--   0        0        0     2642 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
+-rw-r--r--   0        0        0     2590 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
+-rw-r--r--   0        0        0     1232 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
+-rw-r--r--   0        0        0     1055 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/__init__.py
+-rw-r--r--   0        0        0     2372 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
+-rw-r--r--   0        0        0     2262 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
+-rw-r--r--   0        0        0     4191 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
+-rw-r--r--   0        0        0     3240 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py
+-rw-r--r--   0        0        0     2341 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
+-rw-r--r--   0        0        0     2977 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
+-rw-r--r--   0        0        0     2298 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
+-rw-r--r--   0        0        0     2282 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
+-rw-r--r--   0        0        0     1671 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
+-rw-r--r--   0        0        0     1898 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py
+-rw-r--r--   0        0        0      527 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/resource_types.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/forms/__init__.py
+-rw-r--r--   0        0        0     1462 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/forms/shared.py
+-rw-r--r--   0        0        0    25426 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/forms/test_generic_validators.py
+-rw-r--r--   0        0        0     7644 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/forms/test_network_validators.py
+-rw-r--r--   0        0        0     6626 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/forms/test_post_process.py
+-rw-r--r--   0        0        0    11107 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_processes.py
+-rw-r--r--   0        0        0     7301 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_product.py
+-rw-r--r--   0        0        0     5174 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_settings.py
+-rw-r--r--   0        0        0    23655 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_subscriptions.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/schedules/__init__.py
+-rw-r--r--   0        0        0      807 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/schedules/test_scheduling.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/services/__init__.py
+-rw-r--r--   0        0        0    26695 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/services/test_processes.py
+-rw-r--r--   0        0        0     1083 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/services/test_products.py
+-rw-r--r--   0        0        0     5830 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/services/test_subscriptions.py
+-rw-r--r--   0        0        0     2100 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/services/test_translations.py
+-rw-r--r--   0        0        0     7353 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/test_db.py
+-rw-r--r--   0        0        0      385 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/test_types.py
+-rw-r--r--   0        0        0    12048 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1871 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_errors.py
+-rw-r--r--   0        0        0     3517 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_functional.py
+-rw-r--r--   0        0        0     3052 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_json.py
+-rw-r--r--   0        0        0     1144 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_speed.py
+-rw-r--r--   0        0        0    11501 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_state.py
+-rw-r--r--   0        0        0      192 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_strings.py
+-rw-r--r--   0        0        0     8339 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_vlans.py
+-rw-r--r--   0        0        0    12492 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/shared/__init__.py
+-rw-r--r--   0        0        0     2091 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py
+-rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     2039 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
+-rw-r--r--   0        0        0     2584 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py
+-rw-r--r--   0        0        0      288 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/tasks/test_validate_products.py
+-rw-r--r--   0        0        0     3390 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/test_config_db_code.py
+-rw-r--r--   0        0        0     1877 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/test_generic_workflow_steps.py
+-rw-r--r--   0        0        0      987 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/test_modify_note.py
+-rw-r--r--   0        0        0     5364 1970-01-01 00:00:00.000000 orchestrator_core-1.1.1rc2/PKG-INFO
```

### Comparing `orchestrator_core-1.1.1rc1/.github/workflows/README.md` & `orchestrator_core-1.1.1rc2/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/.github/workflows/build-push-container.yml` & `orchestrator_core-1.1.1rc2/.github/workflows/build-push-container.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/.github/workflows/codeql-analysis.yml` & `orchestrator_core-1.1.1rc2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/.github/workflows/publish-package.yml` & `orchestrator_core-1.1.1rc2/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/.github/workflows/run-linting-tests.yml` & `orchestrator_core-1.1.1rc2/.github/workflows/run-linting-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/.github/workflows/run-unit-tests.yml` & `orchestrator_core-1.1.1rc2/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/.github/workflows/scheduled-build.yml` & `orchestrator_core-1.1.1rc2/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/.gitignore` & `orchestrator_core-1.1.1rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/.pre-commit-config.yaml` & `orchestrator_core-1.1.1rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/.stignore` & `orchestrator_core-1.1.1rc2/.stignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/CHANGELOG.md` & `orchestrator_core-1.1.1rc2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/LICENSE` & `orchestrator_core-1.1.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/README.md` & `orchestrator_core-1.1.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/architecture/application/cli.md` & `orchestrator_core-1.1.1rc2/docs/architecture/application/cli.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/architecture/application/domainmodels.md` & `orchestrator_core-1.1.1rc2/docs/architecture/application/domainmodels.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/architecture/application/forms.md` & `orchestrator_core-1.1.1rc2/docs/architecture/application/forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/architecture/application/openapi.json` & `orchestrator_core-1.1.1rc2/docs/architecture/application/openapi.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/architecture/application/python.md` & `orchestrator_core-1.1.1rc2/docs/architecture/application/python.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/architecture/application/scaling.md` & `orchestrator_core-1.1.1rc2/docs/architecture/application/scaling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/architecture/application/tasks.md` & `orchestrator_core-1.1.1rc2/docs/architecture/application/tasks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/architecture/application/websockets.md` & `orchestrator_core-1.1.1rc2/docs/architecture/application/websockets.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/architecture/application/workflow.md` & `orchestrator_core-1.1.1rc2/docs/architecture/application/workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/architecture/tldr.md` & `orchestrator_core-1.1.1rc2/docs/architecture/tldr.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/contributing/guidelines.md` & `orchestrator_core-1.1.1rc2/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/contributing/testing.md` & `orchestrator_core-1.1.1rc2/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/css/termynal.css` & `orchestrator_core-1.1.1rc2/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/getting-started/base.md` & `orchestrator_core-1.1.1rc2/docs/getting-started/base.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/getting-started/development.md` & `orchestrator_core-1.1.1rc2/docs/getting-started/development.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/index.md` & `orchestrator_core-1.1.1rc2/docs/index.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/js/custom.js` & `orchestrator_core-1.1.1rc2/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/js/termynal.js` & `orchestrator_core-1.1.1rc2/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/advanced/circuit-workflow.md` & `orchestrator_core-1.1.1rc2/docs/workshops/advanced/circuit-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/advanced/docker-installation.md` & `orchestrator_core-1.1.1rc2/docs/workshops/advanced/docker-installation.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/advanced/domain-models.md` & `orchestrator_core-1.1.1rc2/docs/workshops/advanced/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/advanced/node-workflow.md` & `orchestrator_core-1.1.1rc2/docs/workshops/advanced/node-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/advanced/overview.md` & `orchestrator_core-1.1.1rc2/docs/workshops/advanced/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/advanced/scenario.md` & `orchestrator_core-1.1.1rc2/docs/workshops/advanced/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/advanced/workflow-introduction.md` & `orchestrator_core-1.1.1rc2/docs/workshops/advanced/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/create-user-group.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/create-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/create-user.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/create-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/database-migration.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/database-migration.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/debian.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/debian.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/docker.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/docker.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/domain-models.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/explore.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/explore.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/input-forms.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/input-forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/macos.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/macos.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/modify-user-group.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/modify-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/modify-user.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/modify-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/overview.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/register-workflows.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/register-workflows.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/scenario.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/start-applications.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/start-applications.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/terminate-user-group.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/terminate-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/terminate-user.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/terminate-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/beginner/workflow-introduction.md` & `orchestrator_core-1.1.1rc2/docs/workshops/beginner/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/images/metadata_products.png` & `orchestrator_core-1.1.1rc2/docs/workshops/images/metadata_products.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/docs/workshops/images/netbox_devices_active.png` & `orchestrator_core-1.1.1rc2/docs/workshops/images/netbox_devices_active.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/examples/basic/basic_orchestrator.py` & `orchestrator_core-1.1.1rc2/examples/basic/basic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/mkdocs.yml` & `orchestrator_core-1.1.1rc2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/mutmut_config.py` & `orchestrator_core-1.1.1rc2/mutmut_config.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the orchestrator workflow engine."""
 
-__version__ = "1.1.1rc1"
+__version__ = "1.1.1rc2"
 
 from orchestrator.app import OrchestratorCore
 from orchestrator.settings import app_settings, oauth2_settings
 from orchestrator.workflow import begin, conditional, done, focussteps, inputstep, retrystep, step, steplens, workflow
 
 __all__ = [
     "OrchestratorCore",
```

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/api.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/api.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/fixed_input.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/health.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/processes.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/product_blocks.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/products.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/resource_types.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/settings.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/subscriptions.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/translations.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/user.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/api_v1/endpoints/workflows.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/error_handling.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/error_handling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/helpers.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/api/models.py` & `orchestrator_core-1.1.1rc2/orchestrator/api/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/app.py` & `orchestrator_core-1.1.1rc2/orchestrator/app.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/database.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/domain_gen_helpers/helpers.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/domain_gen_helpers/types.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generate.md` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generate.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generate.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/fixed_input.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/helpers.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/migration.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/product.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/product_block.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/settings.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/translations.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/unittest.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/unittest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/validations.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/validations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/generator/workflow.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/products/workshop/circuit.yaml` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/circuit.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/products/workshop/node.yaml` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/node.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/products/workshop/user.yaml` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/user.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/create_product.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/create_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/macros.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/macros.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/modify_product.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/modify_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/new_product_migration.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/new_product_migration.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/product.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/product_block.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/product_block.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/shared_forms.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/shared_forms.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/terminate_product.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/terminate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/test_create_workflow.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_create_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/test_modify_workflow.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_modify_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/test_product_type.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_product_type.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/test_terminate_workflow.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_terminate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/test_validate_workflow.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_validate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/generator/templates/validate_product.j2` & `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/validate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/helpers/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/helpers/input_helpers.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/helpers/input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/helpers/print_helpers.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/helpers/print_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/main.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/migrate_domain_models.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/migrate_domain_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/migrate_workflows.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/migrate_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/migration_helpers.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/cli/scheduler.py` & `orchestrator_core-1.1.1rc2/orchestrator/cli/scheduler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/config/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/config/assignee.py` & `orchestrator_core-1.1.1rc2/orchestrator/config/assignee.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/db/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/db/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/db/database.py` & `orchestrator_core-1.1.1rc2/orchestrator/db/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/db/filters/filters.py` & `orchestrator_core-1.1.1rc2/orchestrator/db/filters/filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2020 SURF.
+# Copyright 2019-2023 SURF.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
@@ -16,15 +16,15 @@
 from more_itertools import partition
 from pydantic import BaseModel
 
 from orchestrator.api.error_handling import ProblemDetailException
 from orchestrator.db.database import SearchQuery
 
 
-class CallableErrorHander(Protocol):
+class CallableErrorHandler(Protocol):
     def __call__(self, message: str, **kwargs: Any) -> None:
         ...
 
 
 class Filter(BaseModel):
     field: str
     value: str
@@ -44,45 +44,51 @@
         return partition(_is_valid_filter, filter_by)
 
     return _validate_filters
 
 
 def generic_apply_filters(
     valid_filter_functions_by_column: ValidFilterFunctionsByColumnType,
-) -> Callable[[QueryType, Iterator[Filter], CallableErrorHander], QueryType]:
+) -> Callable[[QueryType, Iterator[Filter], CallableErrorHandler], QueryType]:
     def _apply_filters(
-        query: QueryType, filter_by: Iterator[Filter], handle_filter_error: CallableErrorHander
+        query: QueryType, filter_by: Iterator[Filter], handle_filter_error: CallableErrorHandler
     ) -> QueryType:
         for item in filter_by:
-            field = item.field.lower()
+            field = item.field
             filter_fn = valid_filter_functions_by_column[field]
             try:
                 query = filter_fn(query, item.value)
             except ProblemDetailException as exception:
                 handle_filter_error(
                     exception.detail,
                     field=field,
                     value=item.value,
                 )
+            except ValueError as exception:
+                handle_filter_error(
+                    str(exception),
+                    field=field,
+                    value=item.value,
+                )
         return query
 
     return _apply_filters
 
 
 def generic_filter(
     valid_filter_functions_by_column: ValidFilterFunctionsByColumnType,
-) -> Callable[[QueryType, list[Filter], CallableErrorHander], QueryType]:
+) -> Callable[[QueryType, list[Filter], CallableErrorHandler], QueryType]:
     valid_filter_functions_by_column_KEYS = list(valid_filter_functions_by_column.keys())
     _validate_filters = generic_filters_validate(valid_filter_functions_by_column)
     _apply_filters = generic_apply_filters(valid_filter_functions_by_column)
 
     def _filter(
         query: QueryType,
         filter_by: list[Filter],
-        handle_filter_error: CallableErrorHander,
+        handle_filter_error: CallableErrorHandler,
     ) -> QueryType:
         invalid_filter_items, valid_filter_items = _validate_filters(filter_by)
         if invalid_list := [item.dict() for item in invalid_filter_items]:
             handle_filter_error(
                 "Invalid filter arguments",
                 invalid_filters=invalid_list,
                 valid_filter_keys=valid_filter_functions_by_column_KEYS,
```

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/db/models.py` & `orchestrator_core-1.1.1rc2/orchestrator/db/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     This column type always returns timestamps with the UTC timezone, regardless of the database/connection time zone
     configuration. It also guards against accidentally trying to store Python naive timestamps (those without a time
     zone).
     """
 
     impl = sqlalchemy.types.TIMESTAMP(timezone=True)
     cache_ok = False
+    python_type = datetime
 
     def process_bind_param(self, value: Optional[datetime], dialect: Dialect) -> Optional[datetime]:
         if value is not None:
             if value.tzinfo is None:
                 raise UtcTimestampException(f"Expected timestamp with tzinfo. Got naive timestamp {value!r} instead")
         return value
```

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/db/range/range.py` & `orchestrator_core-1.1.1rc2/orchestrator/db/range/range.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/db/sorting/sorting.py` & `orchestrator_core-1.1.1rc2/orchestrator/db/sorting/sorting.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,95 +10,114 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from enum import Enum
 from typing import Callable, Iterator, TypeVar
 
+import strawberry
 from more_itertools import partition
 from pydantic import BaseModel
+from sqlalchemy import Column
 from sqlalchemy.sql import expression
 
-from orchestrator.db.database import BaseModel as SqlBaseModel
+from orchestrator.api.error_handling import ProblemDetailException
 from orchestrator.db.database import SearchQuery
-from orchestrator.db.filters import CallableErrorHander
+from orchestrator.db.filters import CallableErrorHandler
 
 
+@strawberry.enum(description="Sort order (ASC or DESC)")
 class SortOrder(Enum):
     ASC = "asc"
     DESC = "desc"
 
 
 class Sort(BaseModel):
     field: str
     order: SortOrder
 
-    class Config:
-        use_enum_values = True
-
 
 GenericType = TypeVar("GenericType")
 QueryType = SearchQuery
+ValidSortFunctionsByColumnType = dict[str, Callable[[QueryType, SortOrder], QueryType]]
 
 
 def generic_sorts_validate(
-    valid_sort_dict: dict[str, str]
+    valid_sort_functions_by_column: ValidSortFunctionsByColumnType,
 ) -> Callable[[list[Sort]], tuple[Iterator[Sort], Iterator[Sort]]]:
     """Create generic validate sort factory that creates a validate function based on the valid sort dict.
 
     Args:
         - valid_sort_dict: dict of column names by valid sort keys
             - key: sort key.
             - value: column name.
 
     Returns function that takes sort parameters and returns a list of invalid and valid Sort items.
     """
 
     def validate_sort_items(sort_by: list[Sort]) -> tuple[Iterator[Sort], Iterator[Sort]]:
-        return partition(lambda item: item.field in valid_sort_dict, sort_by)
+        def _is_valid_sort(item: Sort) -> bool:
+            return item.field in valid_sort_functions_by_column
+
+        return partition(_is_valid_sort, sort_by)
 
     return validate_sort_items
 
 
-def generic_apply_sorts(
-    valid_sort_dict: dict[str, str], model: SqlBaseModel
-) -> Callable[[QueryType, Iterator[Sort]], QueryType]:
-    def _apply_sorts(query: QueryType, sort_by: Iterator[Sort]) -> QueryType:
+def generic_apply_sorting(
+    valid_sort_functions_by_column: ValidSortFunctionsByColumnType,
+) -> Callable[[QueryType, Iterator[Sort], CallableErrorHandler], QueryType]:
+    def _apply_sorting(query: QueryType, sort_by: Iterator[Sort], handle_sort_error: CallableErrorHandler) -> QueryType:
         for item in sort_by:
-            field = item.field.lower()
-            sort_key = valid_sort_dict[field]
-
-            if item.order == SortOrder.DESC.value:  # type: ignore
-                query = query.order_by(expression.desc(model.__dict__[sort_key]))
-            else:
-                query = query.order_by(expression.asc(model.__dict__[sort_key]))
+            field = item.field
+            sort_fn = valid_sort_functions_by_column[field]
+            try:
+                query = sort_fn(query, item.order)
+            except ProblemDetailException as exception:
+                handle_sort_error(
+                    exception.detail,
+                    field=field,
+                    order=item.order,
+                )
+            except ValueError as exception:
+                handle_sort_error(
+                    str(exception),
+                    field=field,
+                    order=item.order,
+                )
         return query
 
-    return _apply_sorts
+    return _apply_sorting
 
 
 def generic_sort(
-    valid_sort_dict: dict[str, str],
-    model: SqlBaseModel,
-) -> Callable[[QueryType, list[Sort], CallableErrorHander], QueryType]:
-    valid_sort_keys = list(valid_sort_dict.keys())
-    _validate_sorts = generic_sorts_validate(valid_sort_dict)
-    _apply_sorts = generic_apply_sorts(valid_sort_dict, model)
+    valid_sort_functions_by_column: ValidSortFunctionsByColumnType,
+) -> Callable[[QueryType, list[Sort], CallableErrorHandler], QueryType]:
+    valid_sort_functions_by_column_KEYS = list(valid_sort_functions_by_column.keys())
+    _validate_sorts = generic_sorts_validate(valid_sort_functions_by_column)
+    _apply_sorting = generic_apply_sorting(valid_sort_functions_by_column)
 
     def _sort(
         query: QueryType,
         sort_by: list[Sort],
-        handle_sort_error: CallableErrorHander,
+        handle_sort_error: CallableErrorHandler,
     ) -> QueryType:
-        if sort_by:
-            invalid_sort_items, valid_sort_items = _validate_sorts(sort_by)
-            if invalid_list := [item.dict() for item in invalid_sort_items]:
-                handle_sort_error(
-                    "Invalid sort arguments",
-                    invalid_filters=invalid_list,
-                    valid_filter_keys=valid_sort_keys,
-                )
+        invalid_sort_items, valid_sort_items = _validate_sorts(sort_by)
+        if invalid_list := [{"field": item.field, "order": item.order.value.upper()} for item in invalid_sort_items]:
+            handle_sort_error(
+                "Invalid sort arguments",
+                invalid_sorting=invalid_list,
+                valid_sort_keys=valid_sort_functions_by_column_KEYS,
+            )
 
-            query = _apply_sorts(query, valid_sort_items)
-        return query
+        return _apply_sorting(query, valid_sort_items, handle_sort_error)
 
     return _sort
+
+
+def generic_column_sort(field: Column) -> Callable[[SearchQuery, SortOrder], SearchQuery]:
+    def sort_function(query: SearchQuery, order: SortOrder) -> SearchQuery:
+        if order == SortOrder.DESC:
+            return query.order_by(expression.desc(field))
+        return query.order_by(expression.asc(field))
+
+    return sort_function
```

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/devtools/populator.py` & `orchestrator_core-1.1.1rc2/orchestrator/devtools/populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/distlock/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/distlock/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/distlock/distlock_manager.py` & `orchestrator_core-1.1.1rc2/orchestrator/distlock/distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/distlock/managers/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/distlock/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/distlock/managers/memory_distlock_manager.py` & `orchestrator_core-1.1.1rc2/orchestrator/distlock/managers/memory_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/distlock/managers/redis_distlock_manager.py` & `orchestrator_core-1.1.1rc2/orchestrator/distlock/managers/redis_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/domain/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/domain/base.py` & `orchestrator_core-1.1.1rc2/orchestrator/domain/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/domain/lifecycle.py` & `orchestrator_core-1.1.1rc2/orchestrator/domain/lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/exception_handlers.py` & `orchestrator_core-1.1.1rc2/orchestrator/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/forms/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/forms/network_type_validators.py` & `orchestrator_core-1.1.1rc2/orchestrator/forms/network_type_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/forms/validators.py` & `orchestrator_core-1.1.1rc2/orchestrator/forms/validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/graphql/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/graphql/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,20 +25,27 @@
 from strawberry.fastapi import GraphQLRouter
 from strawberry.http import GraphQLHTTPResponse
 from strawberry.tools import merge_types
 from strawberry.types import ExecutionContext, ExecutionResult
 from strawberry.utils.logging import StrawberryLogger
 
 from orchestrator.graphql.extensions.deprecation_checker_extension import make_deprecation_checker_extension
-from orchestrator.graphql.extensions.ErrorCollectorExtension import ErrorCollectorExtension
+from orchestrator.graphql.extensions.error_collector_extension import ErrorCollectorExtension
 from orchestrator.graphql.pagination import Connection
-from orchestrator.graphql.resolvers import SettingsMutation, resolve_processes, resolve_products, resolve_settings
+from orchestrator.graphql.resolvers import (
+    SettingsMutation,
+    resolve_processes,
+    resolve_products,
+    resolve_settings,
+    resolve_subscriptions,
+)
 from orchestrator.graphql.schemas.process import ProcessType
 from orchestrator.graphql.schemas.product import ProductType
 from orchestrator.graphql.schemas.settings import StatusType
+from orchestrator.graphql.schemas.subscription import SubscriptionType
 from orchestrator.graphql.types import CustomContext
 from orchestrator.security import get_oidc_user, get_opa_security_graphql
 from orchestrator.settings import app_settings
 
 api_router = APIRouter()
 
 logger = structlog.get_logger(__name__)
@@ -48,14 +55,17 @@
 class Query:
     processes: Connection[ProcessType] = authenticated_field(
         resolver=resolve_processes, description="Returns list of processes"
     )
     products: Connection[ProductType] = authenticated_field(
         resolver=resolve_products, description="Returns list of products"
     )
+    subscriptions: Connection[SubscriptionType] = authenticated_field(
+        resolver=resolve_subscriptions, description="Returns list of subscriptions"
+    )
     settings: StatusType = authenticated_field(
         resolver=resolve_settings,
         description="Returns information about cache, workers, and global engine settings",
     )
 
 
 Mutation = merge_types("Mutation", (SettingsMutation,))
```

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/graphql/extensions/ErrorCollectorExtension.py` & `orchestrator_core-1.1.1rc2/orchestrator/graphql/extensions/error_collector_extension.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,51 @@
-# Copyright 2022-2023 SURF.
+# Copyright 2019-2023 SURF.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from collections.abc import Generator
+from contextvars import ContextVar
+from typing import Optional
 
-from typing import Any, Generator
-
+import structlog
 from graphql import GraphQLError
 from strawberry.extensions import SchemaExtension
 
-from orchestrator.graphql.types import CustomInfo
-
+logger = structlog.get_logger(__name__)
 
-class ErrorCollectorExtension(SchemaExtension):
-    errors: list[GraphQLError] = []
+error_bucket: ContextVar[Optional[list[GraphQLError]]] = ContextVar("error_bucket", default=None)
 
-    def resolve(self, _next: Any, root: Any, info: CustomInfo, *args, **kwargs) -> Any:  # type: ignore
-        info.context.errors = self.errors
-        return _next(root, info, *args, **kwargs)
 
+class ErrorCollectorExtension(SchemaExtension):
     def on_execute(self) -> Generator[None, None, None]:
-        self.errors.clear()
+        error_bucket.set([])
+
         yield
-        if self.execution_context.result:
-            if not self.execution_context.result.errors:
-                self.execution_context.result.errors = []
-            self.execution_context.result.errors.extend(self.errors)
+
+        result = self.execution_context.result
+        if result and (collected_errors := error_bucket.get()):
+            if not result.errors:
+                result.errors = []
+            result.errors.extend(collected_errors)
+
+
+def register_error(error: GraphQLError) -> None:
+    """Register a GraphQLError encountered during the query execution.
+
+    Use this to collect errors from multiple resolvers and return them in the response.
+    """
+    errors = error_bucket.get()
+    if errors is None:
+        logger.debug("ErrorCollectorExtension disabled, dropping error", error=error)
+        return
+
+    logger.debug("Registering error", error=error)
+    errors.append(error)
+    error_bucket.set(errors)
```

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py` & `orchestrator_core-1.1.1rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/graphql/pagination.py` & `orchestrator_core-1.1.1rc2/orchestrator/graphql/pagination.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Generic, TypeVar, Union
+from typing import Any, Generic, TypeVar, Union
 
 import strawberry
 
 GenericType = TypeVar("GenericType")
 
 
 @strawberry.type(description="Represents a paginated relationship between two entities")
@@ -53,7 +53,19 @@
 
 @strawberry.type(description="An edge may contain additional information of the relationship")
 class Edge(Generic[GenericType]):
     """An edge may contain additional information of the relationship. This is the trivial case."""
 
     node: GenericType
     cursor: str
+
+
+EMPTY_PAGE: Connection[Any] = Connection(
+    page=[],
+    page_info=PageInfo(
+        has_previous_page=False,
+        has_next_page=False,
+        start_cursor=0,
+        end_cursor=-1,
+        total_items="0",
+    ),
+)
```

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/graphql/resolvers/process.py` & `orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/process.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,60 +10,49 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Union
 
 import structlog
-from graphql import GraphQLError
 from sqlalchemy.orm import defer, joinedload
 
 from orchestrator.db import ProcessSubscriptionTable, ProcessTable, SubscriptionTable
-from orchestrator.db.filters import CallableErrorHander, Filter
+from orchestrator.db.filters import Filter
 from orchestrator.db.filters.process import filter_processes
 from orchestrator.db.range import apply_range_to_query
 from orchestrator.db.sorting import Sort
 from orchestrator.db.sorting.process import sort_processes
 from orchestrator.graphql.pagination import Connection, PageInfo
 from orchestrator.graphql.schemas.process import ProcessGraphqlSchema, ProcessType
 from orchestrator.graphql.types import CustomInfo, GraphqlFilter, GraphqlSort
+from orchestrator.graphql.utils.create_resolver_error_handler import create_resolver_error_handler
 from orchestrator.services.processes import load_process
 from orchestrator.utils.show_process import show_process
 
 logger = structlog.get_logger(__name__)
 
 
 def enrich_process(process: ProcessTable) -> ProcessGraphqlSchema:
     p = load_process(process)
     data = show_process(process, p)
     return ProcessGraphqlSchema(**data)
 
 
-def handle_process_error(info: CustomInfo) -> CallableErrorHander:
-    def _handle_process_error(message: str, **kwargs) -> None:  # type: ignore
-        logger.debug(message, **kwargs)
-        extra_values = dict(kwargs.items()) if kwargs else {}
-        info.context.errors.append(GraphQLError(message=message, path=info.path, extensions=extra_values))
-
-    return _handle_process_error
-
-
 async def resolve_processes(
     info: CustomInfo,
     filter_by: Union[list[GraphqlFilter], None] = None,
     sort_by: Union[list[GraphqlSort], None] = None,
     first: int = 10,
     after: int = 0,
 ) -> Connection[ProcessType]:
-    _error_handler = handle_process_error(info)
-
-    _range: Union[list[int], None] = [after, after + first] if after is not None and first else None
+    _error_handler = create_resolver_error_handler(info)
     pydantic_filter_by: list[Filter] = [item.to_pydantic() for item in filter_by] if filter_by else []
     pydantic_sort_by: list[Sort] = [item.to_pydantic() for item in sort_by] if sort_by else []
-    logger.info("resolve_processes() called", range=_range, sort=sort_by, filter=pydantic_filter_by)
+    logger.info("resolve_processes() called", range=[after, after + first], sort=sort_by, filter=pydantic_filter_by)
 
     # the joinedload on ProcessSubscriptionTable.subscription via ProcessBaseSchema.process_subscriptions prevents a query for every subscription later.
     # tracebacks are not presented in the list of processes and can be really large.
     query = ProcessTable.query.options(
         joinedload(ProcessTable.process_subscriptions)
         .joinedload(ProcessSubscriptionTable.subscription)
         .joinedload(SubscriptionTable.product),
```

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/graphql/resolvers/product.py` & `orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/product.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,37 @@
 from typing import Union
 
 import structlog
-from graphql import GraphQLError
 
-from orchestrator.db.filters import CallableErrorHander, Filter
+from orchestrator.db.filters import Filter
 from orchestrator.db.filters.product import filter_products
 from orchestrator.db.models import ProductTable
 from orchestrator.db.range.range import apply_range_to_query
 from orchestrator.db.sorting.product import sort_products
 from orchestrator.db.sorting.sorting import Sort
 from orchestrator.graphql.pagination import Connection, PageInfo
 from orchestrator.graphql.schemas.product import ProductType
 from orchestrator.graphql.types import CustomInfo, GraphqlFilter, GraphqlSort
+from orchestrator.graphql.utils.create_resolver_error_handler import create_resolver_error_handler
 
 logger = structlog.get_logger(__name__)
 
 
-def handle_product_error(info: CustomInfo) -> CallableErrorHander:
-    def _handle_product_error(message: str, **kwargs) -> None:  # type: ignore
-        logger.debug(message, **kwargs)
-        extra_values = dict(kwargs.items()) if kwargs else {}
-        info.context.errors.append(GraphQLError(message=message, path=info.path, extensions=extra_values))
-
-    return _handle_product_error
-
-
 async def resolve_products(
     info: CustomInfo,
     filter_by: Union[list[GraphqlFilter], None] = None,
     sort_by: Union[list[GraphqlSort], None] = None,
     first: int = 10,
     after: int = 0,
 ) -> Connection[ProductType]:
-    _error_handler = handle_product_error(info)
+    _error_handler = create_resolver_error_handler(info)
 
-    _range: Union[list[int], None] = [after, after + first] if after is not None and first else None
     pydantic_filter_by: list[Filter] = [item.to_pydantic() for item in filter_by] if filter_by else []
     pydantic_sort_by: list[Sort] = [item.to_pydantic() for item in sort_by] if sort_by else []
-    logger.info("resolve_products() called", range=_range, sort=sort_by, filter=pydantic_filter_by)
+    logger.info("resolve_products() called", range=[after, after + first], sort=sort_by, filter=pydantic_filter_by)
 
     query = filter_products(ProductTable.query, pydantic_filter_by, _error_handler)
     query = sort_products(query, pydantic_sort_by, _error_handler)
     total = query.count()
     query = apply_range_to_query(query, after, first)
 
     products = query.all()
```

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/graphql/resolvers/settings.py` & `orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/graphql/schemas/fixed_input.py` & `orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/graphql/schemas/product.py` & `orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/product_block.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,18 @@
+from typing import Optional
+
 import strawberry
 
-from orchestrator.graphql.schemas.fixed_input import FixedInput
-from orchestrator.graphql.schemas.product_block import ProductBlock
-from orchestrator.graphql.schemas.workflow import Workflow
-from orchestrator.schemas.product import ProductSchema
+from orchestrator.graphql.schemas.resource_type import ResourceType
+from orchestrator.schemas.product_block import ProductBlockSchema
 
 
-@strawberry.experimental.pydantic.type(model=ProductSchema)
-class ProductType:
-    product_id: strawberry.auto
+@strawberry.experimental.pydantic.type(model=ProductBlockSchema)
+class ProductBlock:
+    product_block_id: strawberry.auto
     name: strawberry.auto
     description: strawberry.auto
-    product_type: strawberry.auto
-    status: strawberry.auto
     tag: strawberry.auto
+    status: strawberry.auto
     created_at: strawberry.auto
     end_date: strawberry.auto
-    product_blocks: list[ProductBlock]
-    fixed_inputs: list[FixedInput]
-    workflows: list[Workflow]
+    resource_types: Optional[list[ResourceType]]
```

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/graphql/schemas/settings.py` & `orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/graphql/types.py` & `orchestrator_core-1.1.1rc2/orchestrator/graphql/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Map some Orchestrator types to scalars
-from enum import Enum
 from typing import Callable
 
 import strawberry
 from graphql import GraphQLError
 from oauth2_lib.fastapi import OIDCUserModel
 from strawberry.fastapi import BaseContext
 from strawberry.types import Info
@@ -33,26 +32,17 @@
         self.get_opa_decision = get_opa_decision
         super().__init__()
 
 
 CustomInfo = Info[CustomContext, RootValueType]
 
 
-@strawberry.enum(description="Sort order (ASC or DESC)")
-class GraphqlSortOrder(Enum):
-    ASC = "asc"
-    DESC = "desc"
-
-
 @strawberry.experimental.pydantic.input(model=Sort)
 class GraphqlSort:
     field: str = strawberry.field(description="Field to sort on")
-    order: GraphqlSortOrder = strawberry.field(default=GraphqlSortOrder.ASC, description="Sort order (ASC or DESC")
-
-    def to_pydantic(self) -> Sort:
-        return Sort(field=self.field, order=SortOrder[self.order.name])
+    order: SortOrder = strawberry.field(default=SortOrder.ASC, description="Sort order (ASC or DESC")
 
 
 @strawberry.experimental.pydantic.input(model=Filter)
 class GraphqlFilter:
     field: str = strawberry.field(description="Field to filter on")
     value: str = strawberry.field(description="Value to sort the field on")
```

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/graphql/utils/get_selected_fields.py` & `orchestrator_core-1.1.1rc2/orchestrator/graphql/utils/get_selected_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/alembic.ini` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/env.py` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/helpers.py` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/templates/alembic.ini.j2` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/templates/alembic.ini.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/templates/env.py.j2` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/templates/env.py.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py` & `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schedules/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schedules/resume_workflows.py` & `orchestrator_core-1.1.1rc2/orchestrator/schedules/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schedules/scheduling.py` & `orchestrator_core-1.1.1rc2/orchestrator/schedules/scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schedules/task_vacuum.py` & `orchestrator_core-1.1.1rc2/orchestrator/schedules/task_vacuum.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schedules/validate_products.py` & `orchestrator_core-1.1.1rc2/orchestrator/schedules/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schedules/validate_subscriptions.py` & `orchestrator_core-1.1.1rc2/orchestrator/schedules/validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schemas/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schemas/base.py` & `orchestrator_core-1.1.1rc2/orchestrator/schemas/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schemas/engine_settings.py` & `orchestrator_core-1.1.1rc2/orchestrator/schemas/engine_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schemas/fixed_input.py` & `orchestrator_core-1.1.1rc2/orchestrator/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schemas/problem_detail.py` & `orchestrator_core-1.1.1rc2/orchestrator/schemas/problem_detail.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schemas/process.py` & `orchestrator_core-1.1.1rc2/orchestrator/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schemas/product.py` & `orchestrator_core-1.1.1rc2/orchestrator/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schemas/product_block.py` & `orchestrator_core-1.1.1rc2/orchestrator/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schemas/resource_type.py` & `orchestrator_core-1.1.1rc2/orchestrator/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schemas/subscription.py` & `orchestrator_core-1.1.1rc2/orchestrator/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schemas/subscription_descriptions.py` & `orchestrator_core-1.1.1rc2/orchestrator/schemas/subscription_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/schemas/workflow.py` & `orchestrator_core-1.1.1rc2/orchestrator/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/security.py` & `orchestrator_core-1.1.1rc2/orchestrator/security.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/services/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/services/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/services/celery.py` & `orchestrator_core-1.1.1rc2/orchestrator/services/celery.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/services/processes.py` & `orchestrator_core-1.1.1rc2/orchestrator/services/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/services/products.py` & `orchestrator_core-1.1.1rc2/orchestrator/services/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/services/settings.py` & `orchestrator_core-1.1.1rc2/orchestrator/services/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/services/subscriptions.py` & `orchestrator_core-1.1.1rc2/orchestrator/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/services/tasks.py` & `orchestrator_core-1.1.1rc2/orchestrator/services/tasks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/services/translations.py` & `orchestrator_core-1.1.1rc2/orchestrator/services/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/settings.py` & `orchestrator_core-1.1.1rc2/orchestrator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/targets.py` & `orchestrator_core-1.1.1rc2/orchestrator/targets.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/types.py` & `orchestrator_core-1.1.1rc2/orchestrator/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # limitations under the License.
 
 from enum import Enum
 from http import HTTPStatus
 from typing import Any, Callable, Dict, Generator, List, Literal, Optional, Tuple, Type, TypedDict, TypeVar, Union
 from uuid import UUID
 
+import strawberry
 from pydantic import BaseModel
 from pydantic.typing import get_args, get_origin, is_union
 
 UUIDstr = str
 State = Dict[str, Any]
 JSON = Any
 # ErrorState is either a string containing an error message, a catched Exception or a tuple containing a message and
@@ -41,23 +42,25 @@
         return self.value
 
     @classmethod
     def values(cls) -> List:
         return [obj.value for obj in cls]
 
 
+@strawberry.enum
 class SubscriptionLifecycle(strEnum):
     INITIAL = "initial"
     ACTIVE = "active"
     MIGRATING = "migrating"
     DISABLED = "disabled"
     TERMINATED = "terminated"
     PROVISIONING = "provisioning"
 
 
+@strawberry.enum
 class AcceptItemType(strEnum):
     INFO = "info"
     LABEL = "label"
     WARNING = "warning"
     URL = "url"
     CHECKBOX = "checkbox"
     SUBCHECKBOX = ">checkbox"
```

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/crypt.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/datetime.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/docs.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/docs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/errors.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/functional.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/helpers.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/json.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/redis.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/redis.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/show_process.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/show_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/speed.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/state.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/strings.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/strings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/utils/vlans.py` & `orchestrator_core-1.1.1rc2/orchestrator/utils/vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/version.py` & `orchestrator_core-1.1.1rc2/orchestrator/version.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/websocket/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py` & `orchestrator_core-1.1.1rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/websocket/managers/memory_websocket_manager.py` & `orchestrator_core-1.1.1rc2/orchestrator/websocket/managers/memory_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/websocket/websocket_manager.py` & `orchestrator_core-1.1.1rc2/orchestrator/websocket/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/workflow.py` & `orchestrator_core-1.1.1rc2/orchestrator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/workflows/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/workflows/modify_note.py` & `orchestrator_core-1.1.1rc2/orchestrator/workflows/modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/workflows/removed_workflow.py` & `orchestrator_core-1.1.1rc2/orchestrator/workflows/removed_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/workflows/steps.py` & `orchestrator_core-1.1.1rc2/orchestrator/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/workflows/tasks/__init__.py` & `orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py` & `orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/workflows/tasks/resume_workflows.py` & `orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/workflows/tasks/validate_products.py` & `orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/workflows/translations/en-GB.json` & `orchestrator_core-1.1.1rc2/orchestrator/workflows/translations/en-GB.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/orchestrator/workflows/utils.py` & `orchestrator_core-1.1.1rc2/orchestrator/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/pyproject.toml` & `orchestrator_core-1.1.1rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.9",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "alembic==1.5.4",
+    "anyio>=3.7.0",
     "broadcaster[redis]==0.2.0",
     "click==8.0.3",
     "deepmerge==0.1.0",
     "fastapi~=0.91.0",
     "fastapi-etag==0.4.0",
     "more-itertools~=9.0.0",
     "itsdangerous==2.1.2",
@@ -55,17 +56,17 @@
     "opentelemetry-instrumentation-sqlalchemy",
     "orjson==3.8.0",
     "psycopg2-binary==2.9.5",
     "pydantic[email]==1.10.2",
     "python-dateutil==2.8.2",
     "python-rapidjson==1.9",
     "pytz==2022.7.1",
-    "redis~=4.4.2",
+    "redis>=4.5.5,<4.6",
     "schedule==1.1.0",
-    "sentry-sdk[fastapi]==1.15.0",
+    "sentry-sdk[fastapi]==1.25.1",
     "SQLAlchemy==1.4.28",
     "SQLAlchemy-Utils==0.40.0",
     "typer==0.7.0",
     "uvicorn[standard]~=0.20.0",
     "nwa-stdlib~=1.4.7",
     "oauth2-lib~=1.2.9",
     "markupsafe==2.0.1",
```

### Comparing `orchestrator_core-1.1.1rc1/setup.cfg` & `orchestrator_core-1.1.1rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/setup.py` & `orchestrator_core-1.1.1rc2/setup.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/acceptance_tests/conftest.py` & `orchestrator_core-1.1.1rc2/test/acceptance_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py` & `orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py` & `orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py` & `orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py` & `orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py` & `orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/acceptance_tests/test_test_product.py` & `orchestrator_core-1.1.1rc2/test/acceptance_tests/test_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_caching.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_caching.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_fixed_inputs.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_health.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_helpers.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_models.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_processes.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_processes.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     WorkflowTable,
     db,
 )
 from orchestrator.services.processes import shutdown_thread_pool
 from orchestrator.settings import app_settings
 from orchestrator.targets import Target
 from orchestrator.workflow import ProcessStatus, done, init, step, workflow
-from test.unit_tests.conftest import CUSTOMER_ID
 from test.unit_tests.workflows import WorkflowInstanceForTests
 
 test_condition = Condition()
 
 
 @pytest.fixture
 def long_running_workflow():
@@ -395,16 +394,14 @@
     product_name = SubscriptionTable.query.get(generic_subscription_1).product.name
     response = test_client.get(f"/api/processes?filter=product,{product_name}")
     assert 4 == len(response.json())
     response = test_client.get("/api/processes?sort=assignee,asc")
     assert response.json()[0]["assignee"] == "NOC"
     response = test_client.get("/api/processes?sort=started&filter=istask,y")
     assert 4 == len(response.json())
-    response = test_client.get(f"/api/processes?filter=istask,y,organisation,{CUSTOMER_ID}")
-    assert 2 == len(response.json())
 
 
 def test_processes_filterable_response_model(
     test_client, mocked_processes, generic_subscription_2, generic_subscription_1
 ):
     response = test_client.get("/api/processes/?sort=started,asc")
     assert HTTPStatus.OK == response.status_code
```

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_processes_ws.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_processes_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_product_blocks.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_products.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_resource_types.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_settings.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_subscription_customer_descriptions.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_subscriptions.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/api/test_workflows.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/conftest.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import os
 import typing
 from contextlib import closing
 from typing import Any, Optional, cast
 
 import pytest
 import requests
@@ -537,27 +538,58 @@
 
     yield GenericProductTwoInactive, GenericProductTwo
 
     del SUBSCRIPTION_MODEL_REGISTRY["Product 2"]
 
 
 @pytest.fixture
-def generic_subscription_1(generic_product_1, generic_product_type_1):
-    GenericProductOneInactive, _ = generic_product_type_1
-    gen_subscription = GenericProductOneInactive.from_product_id(
-        generic_product_1.product_id, customer_id=CUSTOMER_ID, insync=True
-    )
-    gen_subscription.pb_1.rt_1 = "Value1"
-    gen_subscription.pb_2.rt_2 = 42
-    gen_subscription.pb_2.rt_3 = "Value2"
-    gen_subscription = SubscriptionModel.from_other_lifecycle(gen_subscription, SubscriptionLifecycle.ACTIVE)
-    gen_subscription.description = "Generic Subscription One"
-    gen_subscription.save()
-    db.session.commit()
-    return str(gen_subscription.subscription_id)
+def product_type_1_subscription_factory(generic_product_1, generic_product_type_1):
+    def subscription_create(
+        description="Generic Subscription One",
+        start_date="2023-05-24T00:00:00+00:00",
+        rt_1="Value1",
+        rt_2=42,
+        rt_3="Value2",
+    ):
+        GenericProductOneInactive, _ = generic_product_type_1
+        gen_subscription = GenericProductOneInactive.from_product_id(
+            generic_product_1.product_id, customer_id=CUSTOMER_ID, insync=True
+        )
+        gen_subscription.pb_1.rt_1 = rt_1
+        gen_subscription.pb_2.rt_2 = rt_2
+        gen_subscription.pb_2.rt_3 = rt_3
+        gen_subscription = SubscriptionModel.from_other_lifecycle(gen_subscription, SubscriptionLifecycle.ACTIVE)
+        gen_subscription.description = description
+        gen_subscription.start_date = start_date
+        gen_subscription.save()
+        db.session.commit()
+        return str(gen_subscription.subscription_id)
+
+    return subscription_create
+
+
+@pytest.fixture
+def product_type_1_subscriptions_factory(product_type_1_subscription_factory):
+    def subscriptions_create(amount=1):
+        return [
+            product_type_1_subscription_factory(
+                description=f"Subscription {i}",
+                start_date=(
+                    datetime.datetime.fromisoformat("2023-05-24T00:00:00+00:00") + datetime.timedelta(days=i)
+                ).replace(tzinfo=datetime.timezone.utc),
+            )
+            for i in range(0, amount)
+        ]
+
+    return subscriptions_create
+
+
+@pytest.fixture
+def generic_subscription_1(product_type_1_subscription_factory):
+    return product_type_1_subscription_factory()
 
 
 @pytest.fixture
 def generic_subscription_2(generic_product_2, generic_product_type_2):
     GenericProductTwoInactive, _ = generic_product_type_2
     gen_subscription = GenericProductTwoInactive.from_product_id(
         generic_product_2.product_id, customer_id=CUSTOMER_ID, insync=True
```

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/domain/test_base.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/domain/test_base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/domain/test_base_with_list_union.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/domain/test_base_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/domain/test_base_with_union.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/domain/test_base_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/__init__.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/processes.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/fixtures/products/resource_types.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/forms/shared.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/forms/shared.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/forms/test_generic_validators.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/forms/test_generic_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/forms/test_network_validators.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/forms/test_network_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/forms/test_post_process.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/forms/test_post_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/graphql/test_processes.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_processes.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 process_fields = [
     "assignee",
     "createdBy",
     "failedReason",
     "isTask",
     "lastStep",
     "traceback",
-    "customer",
     "id",
     "lastModified",
     "started",
     "workflowName",
     "status",
     "step",
     "product",
@@ -44,15 +43,14 @@
     page {
       assignee
       createdBy
       failedReason
       isTask
       lastStep
       traceback
-      customer
       id
       lastModified
       started
       workflowName
       status
       step
       product
@@ -77,14 +75,74 @@
                 "sortBy": sort_by if sort_by else [],
                 "filterBy": filter_by if filter_by else [],
             },
         }
     ).encode("utf-8")
 
 
+def get_processes_query_with_subscriptions(
+    first: int = 10,
+    after: int = 0,
+    filter_by: Union[list[str], None] = None,
+    sort_by: Union[list[dict[str, str]], None] = None,
+) -> bytes:
+    query = """
+query ProcessQuery($first: Int!, $after: Int!, $sortBy: [GraphqlSort!], $filterBy: [GraphqlFilter!]) {
+  processes(first: $first, after: $after, sortBy: $sortBy, filterBy: $filterBy) {
+    page {
+      assignee
+      createdBy
+      failedReason
+      isTask
+      lastStep
+      traceback
+      id
+      lastModified
+      started
+      workflowName
+      status
+      step
+      product
+      subscriptions {
+        page {
+          description
+          subscriptionId
+          productId
+          status
+          insync
+          note
+          startDate
+          endDate
+        }
+      }
+    }
+    pageInfo {
+      startCursor
+      totalItems
+      hasPreviousPage
+      endCursor
+      hasNextPage
+    }
+  }
+}
+    """
+    return json.dumps(
+        {
+            "operationName": "ProcessQuery",
+            "query": query,
+            "variables": {
+                "first": first,
+                "after": after,
+                "sortBy": sort_by if sort_by else [],
+                "filterBy": filter_by if filter_by else [],
+            },
+        }
+    ).encode("utf-8")
+
+
 def test_processes_has_next_page(
     test_client, mocked_processes, mocked_processes_resumeall, generic_subscription_2, generic_subscription_1
 ):
     data = get_processes_query()
     response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
     assert HTTPStatus.OK == response.status_code
     result = response.json()
@@ -250,18 +308,18 @@
                 "valid_filter_keys": [
                     "pid",
                     "istask",
                     "assignee",
                     "status",
                     "workflow",
                     "creator",
-                    "organisation",
                     "product",
                     "tag",
                     "subscription",
+                    "subscriptionId",
                     "target",
                 ],
             },
         }
     ]
     assert pageinfo == {
         "hasPreviousPage": False,
@@ -271,65 +329,49 @@
         "totalItems": "4",
     }
 
     for process in processes:
         assert process["status"] == "COMPLETED"
 
 
-def test_processes_filtering_with_invalid_organisation(
+def test_single_process(
     test_client, mocked_processes, mocked_processes_resumeall, generic_subscription_2, generic_subscription_1
 ):
+    process_pid = str(mocked_processes[0])
     # when
 
-    data = get_processes_query(
-        filter_by=[
-            {"field": "status", "value": "completed"},
-            {"field": "organisation", "value": "54321447"},
-        ]
-    )
+    data = get_processes_query(filter_by=[{"field": "pid", "value": process_pid}])
     response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     # then
 
     assert HTTPStatus.OK == response.status_code
     result = response.json()
     processes_data = result["data"]["processes"]
-    errors = result["errors"]
     processes = processes_data["page"]
     pageinfo = processes_data["pageInfo"]
 
-    assert errors == [
-        {
-            "message": "Not a valid organisation, must be a UUID: '54321447'",
-            "path": [None, "processes", "Query"],
-            "extensions": {
-                "field": "organisation",
-                "value": "54321447",
-            },
-        }
-    ]
+    assert len(processes) == 1
     assert pageinfo == {
         "hasPreviousPage": False,
         "hasNextPage": False,
         "startCursor": 0,
-        "endCursor": 3,
-        "totalItems": "4",
+        "endCursor": 0,
+        "totalItems": "1",
     }
-
-    for process in processes:
-        assert process["status"] == "COMPLETED"
+    assert processes[0]["id"] == process_pid
 
 
-def test_single_subscription(
+def test_single_process_with_subscriptions(
     test_client, mocked_processes, mocked_processes_resumeall, generic_subscription_2, generic_subscription_1
 ):
     process_pid = str(mocked_processes[0])
     # when
 
-    data = get_processes_query(filter_by=[{"field": "pid", "value": process_pid}])
+    data = get_processes_query_with_subscriptions(filter_by=[{"field": "pid", "value": process_pid}])
     response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     # then
 
     assert HTTPStatus.OK == response.status_code
     result = response.json()
     processes_data = result["data"]["processes"]
@@ -341,7 +383,8 @@
         "hasPreviousPage": False,
         "hasNextPage": False,
         "startCursor": 0,
         "endCursor": 0,
         "totalItems": "1",
     }
     assert processes[0]["id"] == process_pid
+    assert processes[0]["subscriptions"]["page"][0]["subscriptionId"] == generic_subscription_1
```

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/graphql/test_product.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_product.py`

 * *Files 24% similar despite different names*

```diff
@@ -72,14 +72,97 @@
                 "sortBy": sort_by if sort_by else [],
                 "filterBy": filter_by if filter_by else [],
             },
         }
     ).encode("utf-8")
 
 
+def get_products_with_related_subscriptions_query(
+    first: int = 10,
+    after: int = 0,
+    filter_by: Union[list[str], None] = None,
+    sort_by: Union[list[dict[str, str]], None] = None,
+) -> bytes:
+    query = """
+query ProductQuery($first: Int!, $after: Int!, $filterBy: [GraphqlFilter!], $sortBy: [GraphqlSort!]) {
+  products(first: $first, after: $after, filterBy: $filterBy, sortBy: $sortBy) {
+    page {
+      createdAt
+      description
+      endDate
+      fixedInputs {
+        createdAt
+        fixedInputId
+        name
+        productId
+        value
+      }
+      name
+      productBlocks {
+        createdAt
+        description
+        endDate
+        name
+        productBlockId
+        resourceTypes {
+          description
+          resourceType
+          resourceTypeId
+        }
+        status
+        tag
+      }
+      productId
+      productType
+      status
+      tag
+      workflows {
+        createdAt
+        description
+        target
+        name
+        workflowId
+      }
+      subscriptions {
+        page {
+          description
+          subscriptionId
+          productId
+          status
+          insync
+          note
+          startDate
+          endDate
+        }
+      }
+    }
+    pageInfo {
+      endCursor
+      hasNextPage
+      hasPreviousPage
+      startCursor
+      totalItems
+    }
+  }
+}
+    """
+    return json.dumps(
+        {
+            "operationName": "ProductQuery",
+            "query": query,
+            "variables": {
+                "first": first,
+                "after": after,
+                "sortBy": sort_by if sort_by else [],
+                "filterBy": filter_by if filter_by else [],
+            },
+        }
+    ).encode("utf-8")
+
+
 def test_product_query(test_client, generic_product_1, generic_product_2, generic_product_3):
     data = get_product_query(first=2)
     response: Response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     assert HTTPStatus.OK == response.status_code
     result = response.json()
     products_data = result["data"]["products"]
@@ -157,7 +240,36 @@
     assert pageinfo == {
         "endCursor": 2,
         "hasNextPage": False,
         "hasPreviousPage": False,
         "startCursor": 0,
         "totalItems": "3",
     }
+
+
+def test_single_product_with_subscriptions(
+    test_client, mocked_processes, generic_product_1, generic_subscription_2, generic_subscription_1
+):
+    product_id = str(generic_product_1.product_id)
+    # when
+
+    data = get_products_with_related_subscriptions_query(filter_by=[{"field": "product_id", "value": product_id}])
+    response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
+
+    # then
+
+    assert HTTPStatus.OK == response.status_code
+    result = response.json()
+    products_data = result["data"]["products"]
+    products = products_data["page"]
+    pageinfo = products_data["pageInfo"]
+
+    assert len(products) == 1
+    assert pageinfo == {
+        "hasPreviousPage": False,
+        "hasNextPage": False,
+        "startCursor": 0,
+        "endCursor": 0,
+        "totalItems": "1",
+    }
+    assert products[0]["productId"] == product_id
+    assert products[0]["subscriptions"]["page"][0]["subscriptionId"] == generic_subscription_1
```

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/graphql/test_settings.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/schedules/test_scheduling.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/schedules/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/services/test_processes.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/services/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/services/test_products.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/services/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/services/test_subscriptions.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/services/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/services/test_translations.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/services/test_translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/test_db.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/test_db.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/test_workflow.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_errors.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_functional.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_json.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_speed.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_state.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/utils/test_vlans.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/workflows/__init__.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/workflows/test_config_db_code.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/test_config_db_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/workflows/test_generic_workflow_steps.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/test_generic_workflow_steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/test/unit_tests/workflows/test_modify_note.py` & `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/test_modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc1/PKG-INFO` & `orchestrator_core-1.1.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrator-core
-Version: 1.1.1rc1
+Version: 1.1.1rc2
 Summary: Open source orchestration software for NREN's
 Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: alembic==1.5.4
+Requires-Dist: anyio>=3.7.0
 Requires-Dist: broadcaster[redis]==0.2.0
 Requires-Dist: click==8.0.3
 Requires-Dist: deepmerge==0.1.0
 Requires-Dist: fastapi~=0.91.0
 Requires-Dist: fastapi-etag==0.4.0
 Requires-Dist: more-itertools~=9.0.0
 Requires-Dist: itsdangerous==2.1.2
@@ -45,17 +46,17 @@
 Requires-Dist: opentelemetry-instrumentation-sqlalchemy
 Requires-Dist: orjson==3.8.0
 Requires-Dist: psycopg2-binary==2.9.5
 Requires-Dist: pydantic[email]==1.10.2
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-rapidjson==1.9
 Requires-Dist: pytz==2022.7.1
-Requires-Dist: redis~=4.4.2
+Requires-Dist: redis>=4.5.5,<4.6
 Requires-Dist: schedule==1.1.0
-Requires-Dist: sentry-sdk[fastapi]==1.15.0
+Requires-Dist: sentry-sdk[fastapi]==1.25.1
 Requires-Dist: SQLAlchemy==1.4.28
 Requires-Dist: SQLAlchemy-Utils==0.40.0
 Requires-Dist: typer==0.7.0
 Requires-Dist: uvicorn[standard]~=0.20.0
 Requires-Dist: nwa-stdlib~=1.4.7
 Requires-Dist: oauth2-lib~=1.2.9
 Requires-Dist: markupsafe==2.0.1
```

