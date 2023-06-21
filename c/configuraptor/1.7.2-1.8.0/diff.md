# Comparing `tmp/configuraptor-1.7.2.tar.gz` & `tmp/configuraptor-1.8.0.tar.gz`

## Comparing `configuraptor-1.7.2.tar` & `configuraptor-1.8.0.tar`

### file list

```diff
@@ -1,95 +1,93 @@
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 configuraptor-1.7.2/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.7.2/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.7.2/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.7.2/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.7.2/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.7.2/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.7.2/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/ages.toml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/dataclass.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/dumping.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/dumping.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/example_from_readme.json
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/example_from_readme.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/example_from_readme.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/example_from_readme.yaml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/existing_instance.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/main.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/postponed.py
--rw-r--r--   0        0        0     9464 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/readme.md
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.7.2/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_6c7dc8b73849fb97___init___py.html
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_6c7dc8b73849fb97__types_py.html
--rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
--rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
--rw-r--r--   0        0        0    12229 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html
--rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html
--rw-r--r--   0        0        0    17130 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
--rw-r--r--   0        0        0   131736 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html
--rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_dump_py.html
--rw-r--r--   0        0        0    30314 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
--rw-r--r--   0        0        0    12046 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     8038 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.7.2/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.7.2/pytest_examples/empty.toml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.7.2/pytest_examples/example.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.7.2/pytest_examples/example.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.7.2/pytest_examples/example.yaml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.7.2/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.7.2/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.7.2/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/__init__.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/cls.py
--rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/core.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/dump.py
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/helpers.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/postpone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/loaders/_types.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/loaders/loaders_310.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/loaders/loaders_311.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/loaders/loaders_shared.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.7.2/src/configuraptor/loaders/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.7.2/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.7.2/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.7.2/tests/test_about.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 configuraptor-1.7.2/tests/test_core.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 configuraptor-1.7.2/tests/test_dumps.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.7.2/tests/test_json_yaml.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 configuraptor-1.7.2/tests/test_mypy.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 configuraptor-1.7.2/tests/test_postponed.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.7.2/tests/test_singleton.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.7.2/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.7.2/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 configuraptor-1.7.2/tests/test_toml_existing.py
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 configuraptor-1.7.2/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.7.2/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.7.2/LICENSE.txt
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 configuraptor-1.7.2/README.md
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 configuraptor-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 configuraptor-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 configuraptor-1.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.8.0/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.8.0/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.8.0/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.8.0/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.8.0/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.8.0/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/ages.toml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/dataclass.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/dumping.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/dumping.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/example_from_readme.json
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/example_from_readme.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/example_from_readme.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/example_from_readme.yaml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/existing_instance.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/main.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/postponed.py
+-rw-r--r--   0        0        0     9464 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/readme.md
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.8.0/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0    12019 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97___init___py.html
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97__types_py.html
+-rw-r--r--   0        0        0     9120 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
+-rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
+-rw-r--r--   0        0        0    12225 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html
+-rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html
+-rw-r--r--   0        0        0    26392 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
+-rw-r--r--   0        0        0   131736 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html
+-rw-r--r--   0        0        0    22376 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_dump_py.html
+-rw-r--r--   0        0        0    30314 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.8.0/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/example.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/example.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/example.yaml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/core.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/dump.py
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/postpone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/loaders/_types.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/loaders/loaders_shared.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.8.0/src/configuraptor/loaders/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_about.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_core.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_dumps.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_json_yaml.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_mypy.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_postponed.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_singleton.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 configuraptor-1.8.0/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.8.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 configuraptor-1.8.0/README.md
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 configuraptor-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 configuraptor-1.8.0/PKG-INFO
```

### Comparing `configuraptor-1.7.2/CHANGELOG.md` & `configuraptor-1.8.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.8.0 (2023-06-21)
+### Feature
+* **format:** Allow TypedConfig._format ([`0b46646`](https://github.com/trialandsuccess/configuraptor/commit/0b46646fec153a6bcdfea0c40b872da884aa9146))
+
 ## v1.7.2 (2023-06-20)
 ### Fix
 * **toml:** Tomlkit had own types, move to tomli ([`0b5f0a4`](https://github.com/trialandsuccess/configuraptor/commit/0b5f0a4333f5767fc2329cebb040c6cf4c78eff9))
 
 ## v1.7.1 (2023-06-20)
 ### Fix
 * **310:** Backwards compatible code ([`8f90aec`](https://github.com/trialandsuccess/configuraptor/commit/8f90aec43fd1fcd403f1b68d26e4d605ea346014))
```

### Comparing `configuraptor-1.7.2/coverage.svg` & `configuraptor-1.8.0/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/_static/configuraptor_circle.png` & `configuraptor-1.8.0/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/_static/configuraptor_original.jpeg` & `configuraptor-1.8.0/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/_static/configuraptor_round.png` & `configuraptor-1.8.0/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/_static/configuraptor_transparent.png` & `configuraptor-1.8.0/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/examples/dataclass.py` & `configuraptor-1.8.0/examples/dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/examples/dumping.py` & `configuraptor-1.8.0/examples/dumping.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/examples/example_from_readme.py` & `configuraptor-1.8.0/examples/example_from_readme.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/examples/main.py` & `configuraptor-1.8.0/examples/main.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/examples/postponed.py` & `configuraptor-1.8.0/examples/postponed.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/examples/readme.md` & `configuraptor-1.8.0/examples/readme.md`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/examples/singleton.py` & `configuraptor-1.8.0/examples/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/examples/typedconfig_class.py` & `configuraptor-1.8.0/examples/typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/coverage_html.js` & `configuraptor-1.8.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.8.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.8.0/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_6c7dc8b73849fb97___init___py.html` & `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/loaders/__init__.py: 100%</title>
+    <title>Coverage for src/configuraptor/loaders/loaders_shared.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/configuraptor/loaders/__init__.py</b>:
+            <span class="text">Coverage for </span><b>src/configuraptor/loaders/loaders_shared.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">11 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">11<span class="text"> run</span></button>
+            <span class="text">14 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">14<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
-            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">1<span class="text"> excluded</span></button>
+            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97__types_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_postpone_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 16:40 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,59 +77,56 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Loads loaders based on Python version.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">File loaders that work regardless of Python version.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">_types</span> <span class="key">import</span> <span class="nam">T_config</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="com"># tomlkit used for every Python version now.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">loaders_shared</span> <span class="key">import</span> <span class="nam">json</span><span class="op">,</span> <span class="nam">toml</span><span class="op">,</span> <span class="nam">yaml</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="com"># if sys.version_info > (3, 11):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="com">#     from .loaders_311 import toml</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="com"># else:  # pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="com">#     from .loaders_310 import toml</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span><span class="str">"get"</span><span class="op">,</span> <span class="str">"toml"</span><span class="op">,</span> <span class="str">"json"</span><span class="op">,</span> <span class="str">"yaml"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="nam">T_loader</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Callable</span><span class="op">[</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">BinaryIO</span><span class="op">]</span><span class="op">,</span> <span class="nam">T_config</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">json</span> <span class="key">as</span> <span class="nam">json_lib</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">BinaryIO</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">tomli</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">yaml</span> <span class="key">as</span> <span class="nam">yaml_lib</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">_types</span> <span class="key">import</span> <span class="nam">T_config</span><span class="op">,</span> <span class="nam">as_tconfig</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">def</span> <span class="nam">json</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">    Load a JSON file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">json_lib</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">return</span> <span class="nam">as_tconfig</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">LOADERS</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T_loader</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="str">"toml"</span><span class="op">:</span> <span class="nam">toml</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="str">"json"</span><span class="op">:</span> <span class="nam">json</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="str">"yml"</span><span class="op">:</span> <span class="nam">yaml</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"yaml"</span><span class="op">:</span> <span class="nam">yaml</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="key">def</span> <span class="nam">yaml</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">    Load a YAML file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">yaml_lib</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">,</span> <span class="nam">yaml_lib</span><span class="op">.</span><span class="nam">SafeLoader</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="key">return</span> <span class="nam">as_tconfig</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="key">def</span> <span class="nam">get</span><span class="op">(</span><span class="nam">extension</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_loader</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="key">def</span> <span class="nam">toml</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    Get the right loader for a specific extension.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    Load a toml file.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">extension</span> <span class="op">=</span> <span class="nam">extension</span><span class="op">.</span><span class="nam">removeprefix</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">if</span> <span class="nam">loader</span> <span class="op">:=</span> <span class="nam">LOADERS</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">extension</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="key">return</span> <span class="nam">loader</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">f"Invalid extension {extension}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">tomli</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">return</span> <span class="nam">as_tconfig</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97__types_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_postpone_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 16:40 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,57 +1,54 @@
 
-****** Coverage for src/configuraptor/loaders/__init__.py: 100% ******
+****** Coverage for src/configuraptor/loaders/loaders_shared.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 11 statements   11 run 0 missing 1 excluded *****
+***** 14 statements   14 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 16:40 +0200
+at 2023-06-20 10:44 +0200
 
 
 1""" 
-2Loads loaders based on Python version. 
+2File loaders that work regardless of Python version. 
 3""" 
 4 
-5import typing 
-6 
-7from ._types import T_config 
-8 
-9# tomlkit used for every Python version now. 
-10from .loaders_shared import json, toml, yaml 
-11 
-12# if sys.version_info > (3, 11): 
-13# from .loaders_311 import toml 
-14# else: # pragma: no cover 
-15# from .loaders_310 import toml 
-16 
-17 
-18__all__ = ["get", "toml", "json", "yaml"] 
-19 
-20T_loader = typing.Callable[[typing.BinaryIO], T_config] 
+5import json as json_lib 
+6from typing import BinaryIO 
+7 
+8import tomli 
+9import yaml as yaml_lib 
+10 
+11from ._types import T_config, as_tconfig 
+12 
+13 
+14def json(f: BinaryIO) -> T_config: 
+15 """ 
+16 Load a JSON file. 
+17 """ 
+18 data = json_lib.load(f) 
+19 return as_tconfig(data) 
+20 
 21 
-22LOADERS: dict[str, T_loader] = { 
-23 "toml": toml, 
-24 "json": json, 
-25 "yml": yaml, 
-26 "yaml": yaml, 
-27} 
+22def yaml(f: BinaryIO) -> T_config: 
+23 """ 
+24 Load a YAML file. 
+25 """ 
+26 data = yaml_lib.load(f, yaml_lib.SafeLoader) 
+27 return as_tconfig(data) 
 28 
 29 
-30def get(extension: str) -> T_loader: 
+30def toml(f: BinaryIO) -> T_config: 
 31 """ 
-32 Get the right loader for a specific extension. 
+32 Load a toml file. 
 33 """ 
-34 extension = extension.removeprefix(".") 
-35 if loader := LOADERS.get(extension): 
-36 return loader 
-37 else: 
-38 raise ValueError(f"Invalid extension {extension}") 
+34 data = tomli.load(f) 
+35 return as_tconfig(data) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 16:40 +0200
+at 2023-06-20 10:44 +0200
```

### Comparing `configuraptor-1.7.2/htmlcov/d_6c7dc8b73849fb97__types_py.html` & `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97__types_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_310_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 12:24 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,26 +83,26 @@
     <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="nam">T_config</span> <span class="op">=</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">def</span> <span class="nam">as_tconfig</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="str">    Does not actually do anything, but tells mypy the 'data' of type Any (json, pyyaml, tomlkit) \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="str">    Does not actually do anything, but tells mypy the 'data' of type Any (json, pyyaml, tomli) \</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="str">    is actually a dict of string keys and Any values.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">T_config</span><span class="op">,</span> <span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_310_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 12:24 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,25 +7,25 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 4 statements   4 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 12:24 +0200
+at 2023-06-20 10:44 +0200
 
 
 1import typing 
 2 
 3T_config = dict[str, typing.Any] 
 4 
 5 
 6def as_tconfig(data: typing.Any) -> T_config: 
 7 """ 
 8 Does not actually do anything, but tells mypy the 'data' of type Any (json,
-pyyaml, tomlkit) \ 
+pyyaml, tomli) \ 
 9 is actually a dict of string keys and Any values. 
 10 """ 
 11 return typing.cast(T_config, data) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 12:24 +0200
+at 2023-06-20 10:44 +0200
```

### Comparing `configuraptor-1.7.2/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html` & `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/loaders/loaders_310.py: 100%</title>
+    <title>Coverage for src/configuraptor/loaders/loaders_310.py: 0%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/configuraptor/loaders/loaders_310.py</b>:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">0%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -51,25 +51,25 @@
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
             <span class="text">5 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">5<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">5<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">6<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97__types_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 12:24 +0200
+            created at 2023-06-20 10:45 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -80,21 +80,21 @@
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Loaders for Python 3.10.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">BinaryIO</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">BinaryIO</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">_types</span> <span class="key">import</span> <span class="nam">T_config</span><span class="op">,</span> <span class="nam">as_tconfig</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">_types</span> <span class="key">import</span> <span class="nam">T_config</span><span class="op">,</span> <span class="nam">as_tconfig</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">if</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">version_info</span> <span class="op">></span> <span class="op">(</span><span class="num">3</span><span class="op">,</span> <span class="num">11</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"Wrong Python version!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">if</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">version_info</span> <span class="op">></span> <span class="op">(</span><span class="num">3</span><span class="op">,</span> <span class="num">11</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"Wrong Python version!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="exc show_exc"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">else</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
     <p class="exc show_exc"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="key">import</span> <span class="nam">tomlkit</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="exc show_exc"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="key">def</span> <span class="nam">toml</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="exc show_exc"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">        Load a toml file.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
@@ -105,13 +105,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97__types_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-14 12:24 +0200
+            created at 2023-06-20 10:45 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 
-****** Coverage for src/configuraptor/loaders/loaders_310.py: 100% ******
+****** Coverage for src/configuraptor/loaders/loaders_310.py: 0% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 5 statements   5 run 0 missing 6 excluded *****
+***** 5 statements   0 run 5 missing 6 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 12:24 +0200
+at 2023-06-20 10:45 +0200
 
 
 1""" 
 2Loaders for Python 3.10. 
 3""" 
 4 
 5import sys 
@@ -32,8 +32,8 @@
 16 """ 
 17 Load a toml file. 
 18 """ 
 19 data = tomlkit.load(f) 
 20 return as_tconfig(data) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-14 12:24 +0200
+at 2023-06-20 10:45 +0200
```

### Comparing `configuraptor-1.7.2/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html` & `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/loaders/loaders_311.py: 100%</title>
+    <title>Coverage for src/configuraptor/loaders/loaders_311.py: 50%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/configuraptor/loaders/loaders_311.py</b>:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">50%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -51,25 +51,25 @@
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
             <span class="text">6 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">6<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">3<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">3<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">2<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_310_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_shared_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:32 +0200
+            created at 2023-06-20 10:45 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -87,29 +87,29 @@
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">BinaryIO</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">_types</span> <span class="key">import</span> <span class="nam">T_config</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="exc show_exc"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">if</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">version_info</span> <span class="op">&lt;</span> <span class="op">(</span><span class="num">3</span><span class="op">,</span> <span class="num">11</span><span class="op">)</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
     <p class="exc show_exc"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"Wrong Python version!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="key">import</span> <span class="nam">tomllib</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="key">import</span> <span class="nam">tomllib</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="key">def</span> <span class="nam">toml</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="key">def</span> <span class="nam">toml</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">        Load a toml file.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="key">return</span> <span class="nam">tomllib</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="key">return</span> <span class="nam">tomllib</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_310_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_shared_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:32 +0200
+            created at 2023-06-20 10:45 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 
-****** Coverage for src/configuraptor/loaders/loaders_311.py: 100% ******
+****** Coverage for src/configuraptor/loaders/loaders_311.py: 50% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 6 statements   6 run 0 missing 2 excluded *****
+***** 6 statements   3 run 3 missing 2 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:32 +0200
+at 2023-06-20 10:45 +0200
 
 
 1""" 
 2Loaders for Python 3.11+. 
 3""" 
 4import sys 
 5from typing import BinaryIO 
@@ -30,8 +30,8 @@
 14 def toml(f: BinaryIO) -> T_config: 
 15 """ 
 16 Load a toml file. 
 17 """ 
 18 return tomllib.load(f) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:32 +0200
+at 2023-06-20 10:45 +0200
```

### Comparing `configuraptor-1.7.2/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html` & `configuraptor-1.8.0/htmlcov/d_6c7dc8b73849fb97___init___py.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/loaders/loaders_shared.py: 100%</title>
+    <title>Coverage for src/configuraptor/loaders/__init__.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/configuraptor/loaders/loaders_shared.py</b>:
+            <span class="text">Coverage for </span><b>src/configuraptor/loaders/__init__.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">14 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">14<span class="text"> run</span></button>
+            <span class="text">11 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">11<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_postpone_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97__types_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 16:40 +0200
+            created at 2023-06-21 15:50 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,56 +77,53 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">File loaders that work regardless of Python version.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Loads loaders based on Python version.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">json</span> <span class="key">as</span> <span class="nam">json_lib</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">BinaryIO</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">tomlkit</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">yaml</span> <span class="key">as</span> <span class="nam">yaml_lib</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">_types</span> <span class="key">import</span> <span class="nam">T_config</span><span class="op">,</span> <span class="nam">as_tconfig</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">_types</span> <span class="key">import</span> <span class="nam">T_config</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="com"># tomli used for every Python version now.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">loaders_shared</span> <span class="key">import</span> <span class="nam">json</span><span class="op">,</span> <span class="nam">toml</span><span class="op">,</span> <span class="nam">yaml</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span><span class="str">"get"</span><span class="op">,</span> <span class="str">"toml"</span><span class="op">,</span> <span class="str">"json"</span><span class="op">,</span> <span class="str">"yaml"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">def</span> <span class="nam">json</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">    Load a JSON file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">json_lib</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">return</span> <span class="nam">as_tconfig</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="key">def</span> <span class="nam">yaml</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">    Load a YAML file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">yaml_lib</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">,</span> <span class="nam">yaml_lib</span><span class="op">.</span><span class="nam">SafeLoader</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="key">return</span> <span class="nam">as_tconfig</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="key">def</span> <span class="nam">toml</span><span class="op">(</span><span class="nam">f</span><span class="op">:</span> <span class="nam">BinaryIO</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    Load a toml file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">tomlkit</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">return</span> <span class="nam">as_tconfig</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="nam">T_loader</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Callable</span><span class="op">[</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">BinaryIO</span><span class="op">]</span><span class="op">,</span> <span class="nam">T_config</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="nam">LOADERS</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T_loader</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="str">"toml"</span><span class="op">:</span> <span class="nam">toml</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="str">"json"</span><span class="op">:</span> <span class="nam">json</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="str">"yml"</span><span class="op">:</span> <span class="nam">yaml</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="str">"yaml"</span><span class="op">:</span> <span class="nam">yaml</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="key">def</span> <span class="nam">get</span><span class="op">(</span><span class="nam">extension</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T_loader</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">    Get the right loader for a specific extension.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="nam">extension</span> <span class="op">=</span> <span class="nam">extension</span><span class="op">.</span><span class="nam">removeprefix</span><span class="op">(</span><span class="str">"."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="key">if</span> <span class="nam">loader</span> <span class="op">:=</span> <span class="nam">LOADERS</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">extension</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="key">return</span> <span class="nam">loader</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">f"Invalid extension {extension}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_311_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_postpone_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_6c7dc8b73849fb97__types_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 16:40 +0200
+            created at 2023-06-21 15:50 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,54 +1,51 @@
 
-****** Coverage for src/configuraptor/loaders/loaders_shared.py: 100% ******
+****** Coverage for src/configuraptor/loaders/__init__.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 14 statements   14 run 0 missing 0 excluded *****
+***** 11 statements   11 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 16:40 +0200
+at 2023-06-21 15:50 +0200
 
 
 1""" 
-2File loaders that work regardless of Python version. 
+2Loads loaders based on Python version. 
 3""" 
 4 
-5import json as json_lib 
-6from typing import BinaryIO 
-7 
-8import tomlkit 
-9import yaml as yaml_lib 
-10 
-11from ._types import T_config, as_tconfig 
-12 
+5import typing 
+6 
+7from ._types import T_config 
+8 
+9# tomli used for every Python version now. 
+10from .loaders_shared import json, toml, yaml 
+11 
+12__all__ = ["get", "toml", "json", "yaml"] 
 13 
-14def json(f: BinaryIO) -> T_config: 
-15 """ 
-16 Load a JSON file. 
-17 """ 
-18 data = json_lib.load(f) 
-19 return as_tconfig(data) 
-20 
-21 
-22def yaml(f: BinaryIO) -> T_config: 
-23 """ 
-24 Load a YAML file. 
+14T_loader = typing.Callable[[typing.BinaryIO], T_config] 
+15 
+16LOADERS: dict[str, T_loader] = { 
+17 "toml": toml, 
+18 "json": json, 
+19 "yml": yaml, 
+20 "yaml": yaml, 
+21} 
+22 
+23 
+24def get(extension: str) -> T_loader: 
 25 """ 
-26 data = yaml_lib.load(f, yaml_lib.SafeLoader) 
-27 return as_tconfig(data) 
-28 
-29 
-30def toml(f: BinaryIO) -> T_config: 
-31 """ 
-32 Load a toml file. 
-33 """ 
-34 data = tomlkit.load(f) 
-35 return as_tconfig(data) 
+26 Get the right loader for a specific extension. 
+27 """ 
+28 extension = extension.removeprefix(".") 
+29 if loader := LOADERS.get(extension): 
+30 return loader 
+31 else: 
+32 raise ValueError(f"Invalid extension {extension}") 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 16:40 +0200
+at 2023-06-21 15:50 +0200
```

### Comparing `configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40___about___py.html` & `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 16:40 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,23 +83,23 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">This file contains the module version.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.5.0"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.7.2"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 16:40 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,22 +7,22 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 1 statements   1 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 16:40 +0200
+at 2023-06-20 10:44 +0200
 
 
 1""" 
 2This file contains the module version. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 6# 
 7# SPDX-License-Identifier: MIT 
-8__version__ = "1.5.0" 
+8__version__ = "1.7.2" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 16:40 +0200
+at 2023-06-20 10:44 +0200
```

### Comparing `configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40___init___py.html` & `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 16:40 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,15 +83,15 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Exposes TypedConfig and load_into for this library.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">cls</span> <span class="key">import</span> <span class="nam">TypedConfig</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">cls</span> <span class="key">import</span> <span class="nam">TypedConfig</span><span class="op">,</span> <span class="nam">update</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="nam">all_annotations</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="nam">check_and_convert_data</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="nam">convert_config</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="nam">ensure_types</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="nam">load_into</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="nam">load_into_class</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
@@ -100,41 +100,42 @@
     <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">dump</span> <span class="key">import</span> <span class="nam">asdict</span><span class="op">,</span> <span class="nam">asjson</span><span class="op">,</span> <span class="nam">astoml</span><span class="op">,</span> <span class="nam">asyaml</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">postpone</span> <span class="key">import</span> <span class="nam">postpone</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">singleton</span> <span class="key">import</span> <span class="nam">Singleton</span><span class="op">,</span> <span class="nam">SingletonMeta</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">__all__</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="com"># cls</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="str">"TypedConfig"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="com"># singleton</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="str">"Singleton"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="str">"SingletonMeta"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="com"># core</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="str">"all_annotations"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"check_and_convert_data"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"convert_config"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="str">"ensure_types"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"load_into"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="str">"load_into_class"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="str">"load_into_instance"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="com"># postpone</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="str">"postpone"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="com"># dump</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="str">"asdict"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="str">"astoml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="str">"asyaml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="str">"asjson"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="str">"update"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="com"># singleton</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="str">"Singleton"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="str">"SingletonMeta"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="com"># core</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"all_annotations"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"check_and_convert_data"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="str">"convert_config"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"ensure_types"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="str">"load_into"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="str">"load_into_class"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="str">"load_into_instance"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="com"># postpone</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="str">"postpone"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="com"># dump</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="str">"asdict"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="str">"astoml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="str">"asyaml"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="str">"asjson"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_cls_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 16:40 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,26 +7,26 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 6 statements   6 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 16:40 +0200
+at 2023-06-20 10:44 +0200
 
 
 1""" 
 2Exposes TypedConfig and load_into for this library. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 6# 
 7# SPDX-License-Identifier: MIT 
-8from .cls import TypedConfig 
+8from .cls import TypedConfig, update 
 9from .core import ( 
 10 all_annotations, 
 11 check_and_convert_data, 
 12 convert_config, 
 13 ensure_types, 
 14 load_into, 
 15 load_into_class, 
@@ -35,29 +35,30 @@
 18from .dump import asdict, asjson, astoml, asyaml 
 19from .postpone import postpone 
 20from .singleton import Singleton, SingletonMeta 
 21 
 22__all__ = [ 
 23 # cls 
 24 "TypedConfig", 
-25 # singleton 
-26 "Singleton", 
-27 "SingletonMeta", 
-28 # core 
-29 "all_annotations", 
-30 "check_and_convert_data", 
-31 "convert_config", 
-32 "ensure_types", 
-33 "load_into", 
-34 "load_into_class", 
-35 "load_into_instance", 
-36 # postpone 
-37 "postpone", 
-38 # dump 
-39 "asdict", 
-40 "astoml", 
-41 "asyaml", 
-42 "asjson", 
-43] 
+25 "update", 
+26 # singleton 
+27 "Singleton", 
+28 "SingletonMeta", 
+29 # core 
+30 "all_annotations", 
+31 "check_and_convert_data", 
+32 "convert_config", 
+33 "ensure_types", 
+34 "load_into", 
+35 "load_into_class", 
+36 "load_into_instance", 
+37 # postpone 
+38 "postpone", 
+39 # dump 
+40 "asdict", 
+41 "astoml", 
+42 "asyaml", 
+43 "asjson", 
+44] 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 16:40 +0200
+at 2023-06-20 10:44 +0200
```

### Comparing `configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_cls_py.html` & `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_dump_py.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/cls.py: 100%</title>
+    <title>Coverage for src/configuraptor/dump.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/configuraptor/cls.py</b>:
+            <span class="text">Coverage for </span><b>src/configuraptor/dump.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">18 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">18<span class="text"> run</span></button>
+            <span class="text">31 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">31<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-19 17:38 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,63 +77,84 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Logic for the TypedConfig inheritable class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Method to dump classes to other formats.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">all_annotations</span><span class="op">,</span> <span class="nam">check_type</span><span class="op">,</span> <span class="nam">is_optional</span><span class="op">,</span> <span class="nam">load_into</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">errors</span> <span class="key">import</span> <span class="nam">ConfigErrorExtraKey</span><span class="op">,</span> <span class="nam">ConfigErrorInvalidType</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">C</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"C"</span><span class="op">,</span> <span class="nam">bound</span><span class="op">=</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedConfig</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">    Can be used instead of load_into.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">def</span> <span class="nam">load</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">        Load a class' config values from the config file.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">        SomeClass.load(data, ...) = load_into(SomeClass, data, ...).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="key">def</span> <span class="nam">update</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span> <span class="nam">allow_none</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">__class__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">json</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">tomli_w</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">yaml</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="nam">instance_of_custom_class</span><span class="op">,</span> <span class="nam">is_custom_class</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">camel_to_snake</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">def</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">_level</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">0</span><span class="op">,</span> <span class="op">/</span><span class="op">,</span> <span class="nam">with_top_level_key</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    Dump a config instance to a dictionary (recursively).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="nam">cls</span> <span class="op">=</span> <span class="nam">value</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">asdict</span><span class="op">(</span><span class="nam">_</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span> <span class="key">if</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">_</span><span class="op">)</span> <span class="key">else</span> <span class="nam">_</span> <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">dict</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">v</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span> <span class="key">if</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">v</span><span class="op">)</span> <span class="key">else</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">data</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">values</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">            <span class="key">if</span> <span class="nam">value</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">allow_none</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">                <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">            <span class="key">if</span> <span class="nam">strict</span> <span class="key">and</span> <span class="nam">key</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ConfigErrorExtraKey</span><span class="op">(</span><span class="nam">cls</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">__class__</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="key">if</span> <span class="nam">_level</span> <span class="op">==</span> <span class="num">0</span> <span class="key">and</span> <span class="nam">with_top_level_key</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="com"># top-level: add an extra key indicating the class' name</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">cls_name</span> <span class="op">=</span> <span class="nam">camel_to_snake</span><span class="op">(</span><span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span><span class="nam">cls_name</span><span class="op">:</span> <span class="nam">data</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">            <span class="key">if</span> <span class="nam">strict</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span><span class="op">)</span> <span class="key">and</span> <span class="key">not</span> <span class="op">(</span><span class="nam">value</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="nam">allow_none</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">expected_type</span><span class="op">=</span><span class="nam">annotations</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="nam">setattr</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="key">def</span> <span class="nam">astoml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">multiline_strings</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">    Dump a config instance to toml (recursively).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">return</span> <span class="nam">tomli_w</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">multiline_strings</span><span class="op">=</span><span class="nam">multiline_strings</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="key">def</span> <span class="nam">asjson</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="str">    Dump a config instance to json (recursively).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">return</span> <span class="nam">json</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="key">def</span> <span class="nam">asyaml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">    Dump a config instance to yaml (recursively).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="nam">output</span> <span class="op">=</span> <span class="nam">yaml</span><span class="op">.</span><span class="nam">dump</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="com"># output is already a str but mypy doesn't know that</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="nam">output</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-19 17:38 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,65 +1,85 @@
 
-****** Coverage for src/configuraptor/cls.py: 100% ******
+****** Coverage for src/configuraptor/dump.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 18 statements   18 run 0 missing 0 excluded *****
+***** 31 statements   31 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-19 17:38 +0200
+at 2023-06-20 10:44 +0200
 
 
 1""" 
-2Logic for the TypedConfig inheritable class. 
+2Method to dump classes to other formats. 
 3""" 
 4 
-5import typing 
-6 
-7from .core import T_data, all_annotations, check_type, is_optional, load_into 
-8from .errors import ConfigErrorExtraKey, ConfigErrorInvalidType 
-9 
-10C = typing.TypeVar("C", bound=typing.Any) 
-11 
-12 
-13class TypedConfig: 
-14 """ 
-15 Can be used instead of load_into. 
+5import json 
+6import typing 
+7 
+8import tomli_w 
+9import yaml 
+10 
+11from .core import instance_of_custom_class, is_custom_class 
+12from .helpers import camel_to_snake 
+13 
+14 
+15def asdict(inst: typing.Any, _level: int = 0, /, with_top_level_key: bool =
+True) -> dict[str, typing.Any]: 
 16 """ 
-17 
-18 @classmethod 
-19 def load( 
-20 cls: typing.Type[C], data: T_data, key: str = None, init: dict[str,
-typing.Any] = None, strict: bool = True 
-21 ) -> C: 
-22 """ 
-23 Load a class' config values from the config file. 
-24 
-25 SomeClass.load(data, ...) = load_into(SomeClass, data, ...). 
-26 """ 
-27 return load_into(cls, data, key=key, init=init, strict=strict) 
-28 
-29 def update(self, strict: bool = True, allow_none: bool = False, **values:
-typing.Any): 
-30 annotations = all_annotations(self.__class__) 
+17 Dump a config instance to a dictionary (recursively). 
+18 """ 
+19 data = {} 
+20 
+21 for key, value in inst.__dict__.items(): 
+22 cls = value.__class__ 
+23 if is_custom_class(cls): 
+24 value = asdict(value, _level + 1) 
+25 elif isinstance(value, list): 
+26 value = [asdict(_, _level + 1) if instance_of_custom_class(_) else _ for _
+in value] 
+27 elif isinstance(value, dict): 
+28 value = {k: asdict(v, _level + 1) if instance_of_custom_class(v) else v for
+k, v in value.items()} 
+29 
+30 data[key] = value 
 31 
-32 for key, value in values.items(): 
-33 if value is None and not allow_none: 
-34 continue 
-35 
-36 if strict and key not in annotations: 
-37 raise ConfigErrorExtraKey(cls=self.__class__, key=key, value=value) 
+32 if _level == 0 and with_top_level_key: 
+33 # top-level: add an extra key indicating the class' name 
+34 cls_name = camel_to_snake(inst.__class__.__name__) 
+35 return {cls_name: data} 
+36 
+37 return data 
 38 
-39 if strict and not check_type(value, annotations[key]) and not (value is None
-and allow_none): 
-40 raise ConfigErrorInvalidType(expected_type=annotations[key], key=key,
-value=value) 
-41 
-42 setattr(self, key, value) 
+39 
+40def astoml(inst: typing.Any, multiline_strings: bool = False) -> str: 
+41 """ 
+42 Dump a config instance to toml (recursively). 
+43 """ 
+44 data = asdict(inst) 
+45 return tomli_w.dumps(data, multiline_strings=multiline_strings) 
+46 
+47 
+48def asjson(inst: typing.Any, **kw: typing.Any) -> str: 
+49 """ 
+50 Dump a config instance to json (recursively). 
+51 """ 
+52 data = asdict(inst) 
+53 return json.dumps(data, **kw) 
+54 
+55 
+56def asyaml(inst: typing.Any, **kw: typing.Any) -> str: 
+57 """ 
+58 Dump a config instance to yaml (recursively). 
+59 """ 
+60 data = asdict(inst) 
+61 output = yaml.dump(data, encoding=None, **kw) 
+62 # output is already a str but mypy doesn't know that 
+63 return typing.cast(str, output) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-19 17:38 +0200
+at 2023-06-20 10:44 +0200
```

### Comparing `configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_core_py.html` & `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_dump_py.html` & `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/configuraptor/dump.py: 100%</title>
+    <title>Coverage for src/configuraptor/cls.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/configuraptor/dump.py</b>:
+            <span class="text">Coverage for </span><b>src/configuraptor/cls.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">31 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">31<span class="text"> run</span></button>
+            <span class="text">24 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">24<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 16:40 +0200
+            created at 2023-06-21 15:50 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,84 +77,100 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Method to dump classes to other formats.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Logic for the TypedConfig inheritable class.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">json</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">tomlkit</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">yaml</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="nam">instance_of_custom_class</span><span class="op">,</span> <span class="nam">is_custom_class</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">camel_to_snake</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">def</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">_level</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">0</span><span class="op">,</span> <span class="op">/</span><span class="op">,</span> <span class="nam">with_top_level_key</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">    Dump a config instance to a dictionary (recursively).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">inst</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="nam">cls</span> <span class="op">=</span> <span class="nam">value</span><span class="op">.</span><span class="nam">__class__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="key">if</span> <span class="nam">is_custom_class</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="nam">asdict</span><span class="op">(</span><span class="nam">_</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span> <span class="key">if</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">_</span><span class="op">)</span> <span class="key">else</span> <span class="nam">_</span> <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">value</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">dict</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">value</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">v</span><span class="op">,</span> <span class="nam">_level</span> <span class="op">+</span> <span class="num">1</span><span class="op">)</span> <span class="key">if</span> <span class="nam">instance_of_custom_class</span><span class="op">(</span><span class="nam">v</span><span class="op">)</span> <span class="key">else</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">value</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">data</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="key">if</span> <span class="nam">_level</span> <span class="op">==</span> <span class="num">0</span> <span class="key">and</span> <span class="nam">with_top_level_key</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="com"># top-level: add an extra key indicating the class' name</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">cls_name</span> <span class="op">=</span> <span class="nam">camel_to_snake</span><span class="op">(</span><span class="nam">inst</span><span class="op">.</span><span class="nam">__class__</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span><span class="nam">cls_name</span><span class="op">:</span> <span class="nam">data</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">all_annotations</span><span class="op">,</span> <span class="nam">check_type</span><span class="op">,</span> <span class="nam">load_into</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">errors</span> <span class="key">import</span> <span class="nam">ConfigErrorExtraKey</span><span class="op">,</span> <span class="nam">ConfigErrorInvalidType</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">C</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"C"</span><span class="op">,</span> <span class="nam">bound</span><span class="op">=</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedConfig</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">    Can be used instead of load_into.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">def</span> <span class="nam">load</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">T_data</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">init</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">C</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">        Load a class' config values from the config file.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">        SomeClass.load(data, ...) = load_into(SomeClass, data, ...).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">return</span> <span class="nam">load_into</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">init</span><span class="op">=</span><span class="nam">init</span><span class="op">,</span> <span class="nam">strict</span><span class="op">=</span><span class="nam">strict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="key">def</span> <span class="nam">_update</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">_strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">        Can be used if .update is overwritten with another value in the config.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">__class__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">values</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">            <span class="key">if</span> <span class="nam">value</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">_allow_none</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">                <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="key">def</span> <span class="nam">astoml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">sort_keys</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">    Dump a config instance to toml (recursively).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">return</span> <span class="nam">tomlkit</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">sort_keys</span><span class="op">=</span><span class="nam">sort_keys</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">            <span class="key">if</span> <span class="nam">_strict</span> <span class="key">and</span> <span class="nam">key</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ConfigErrorExtraKey</span><span class="op">(</span><span class="nam">cls</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">__class__</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="key">if</span> <span class="nam">_strict</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span><span class="op">)</span> <span class="key">and</span> <span class="key">not</span> <span class="op">(</span><span class="nam">value</span> <span class="key">is</span> <span class="key">None</span> <span class="key">and</span> <span class="nam">_allow_none</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ConfigErrorInvalidType</span><span class="op">(</span><span class="nam">expected_type</span><span class="op">=</span><span class="nam">annotations</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span><span class="op">,</span> <span class="nam">key</span><span class="op">=</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">            <span class="nam">setattr</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="key">def</span> <span class="nam">asjson</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="str">    Dump a config instance to json (recursively).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">return</span> <span class="nam">json</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="key">def</span> <span class="nam">asyaml</span><span class="op">(</span><span class="nam">inst</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">    Dump a config instance to yaml (recursively).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">asdict</span><span class="op">(</span><span class="nam">inst</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="nam">output</span> <span class="op">=</span> <span class="nam">yaml</span><span class="op">.</span><span class="nam">dump</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="com"># output is already a str but mypy doesn't know that</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="nam">output</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="key">def</span> <span class="nam">update</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">_strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t"><span class="str">        Update values on this config.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="str">            _strict: allow wrong types?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="str">            _allow_none: allow None or skip those entries?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t"><span class="str">            **values: key: value pairs in the right types to update.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_update</span><span class="op">(</span><span class="nam">_strict</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="key">def</span> <span class="nam">_format</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">string</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="str">        Format the config data into a string template.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="str">        Replacement for string.format(**config), which is only possible for MutableMappings.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="str">        MutableMapping does not work well with our Singleton Metaclass.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="key">return</span> <span class="nam">string</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="op">**</span><span class="nam">self</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="com"># also expose as separate function:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t"><span class="key">def</span> <span class="nam">update</span><span class="op">(</span><span class="nam">instance</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">_strict</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">True</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t"><span class="str">    Update values on a config.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t"><span class="str">        instance: config instance to update</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="str">        _strict: allow wrong types?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="str">        _allow_none: allow None or skip those entries?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="str">        **values: key: value pairs in the right types to update.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedConfig</span><span class="op">.</span><span class="nam">_update</span><span class="op">(</span><span class="nam">instance</span><span class="op">,</span> <span class="nam">_strict</span><span class="op">,</span> <span class="nam">_allow_none</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_errors_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_core_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 16:40 +0200
+            created at 2023-06-21 15:50 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,85 +1,105 @@
 
-****** Coverage for src/configuraptor/dump.py: 100% ******
+****** Coverage for src/configuraptor/cls.py: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 31 statements   31 run 0 missing 0 excluded *****
+***** 24 statements   24 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 16:40 +0200
+at 2023-06-21 15:50 +0200
 
 
 1""" 
-2Method to dump classes to other formats. 
+2Logic for the TypedConfig inheritable class. 
 3""" 
 4 
-5import json 
-6import typing 
-7 
-8import tomlkit 
-9import yaml 
-10 
-11from .core import instance_of_custom_class, is_custom_class 
-12from .helpers import camel_to_snake 
-13 
-14 
-15def asdict(inst: typing.Any, _level: int = 0, /, with_top_level_key: bool =
-True) -> dict[str, typing.Any]: 
+5import typing 
+6 
+7from .core import T_data, all_annotations, check_type, load_into 
+8from .errors import ConfigErrorExtraKey, ConfigErrorInvalidType 
+9 
+10C = typing.TypeVar("C", bound=typing.Any) 
+11 
+12 
+13class TypedConfig: 
+14 """ 
+15 Can be used instead of load_into. 
 16 """ 
-17 Dump a config instance to a dictionary (recursively). 
-18 """ 
-19 data = {} 
-20 
-21 for key, value in inst.__dict__.items(): 
-22 cls = value.__class__ 
-23 if is_custom_class(cls): 
-24 value = asdict(value, _level + 1) 
-25 elif isinstance(value, list): 
-26 value = [asdict(_, _level + 1) if instance_of_custom_class(_) else _ for _
-in value] 
-27 elif isinstance(value, dict): 
-28 value = {k: asdict(v, _level + 1) if instance_of_custom_class(v) else v for
-k, v in value.items()} 
-29 
-30 data[key] = value 
-31 
-32 if _level == 0 and with_top_level_key: 
-33 # top-level: add an extra key indicating the class' name 
-34 cls_name = camel_to_snake(inst.__class__.__name__) 
-35 return {cls_name: data} 
-36 
-37 return data 
+17 
+18 @classmethod 
+19 def load( 
+20 cls: typing.Type[C], data: T_data, key: str = None, init: dict[str,
+typing.Any] = None, strict: bool = True 
+21 ) -> C: 
+22 """ 
+23 Load a class' config values from the config file. 
+24 
+25 SomeClass.load(data, ...) = load_into(SomeClass, data, ...). 
+26 """ 
+27 return load_into(cls, data, key=key, init=init, strict=strict) 
+28 
+29 def _update(self, _strict: bool = True, _allow_none: bool = False, **values:
+typing.Any) -> None: 
+30 """ 
+31 Can be used if .update is overwritten with another value in the config. 
+32 """ 
+33 annotations = all_annotations(self.__class__) 
+34 
+35 for key, value in values.items(): 
+36 if value is None and not _allow_none: 
+37 continue 
 38 
-39 
-40def astoml(inst: typing.Any, sort_keys: bool = False) -> str: 
-41 """ 
-42 Dump a config instance to toml (recursively). 
-43 """ 
-44 data = asdict(inst) 
-45 return tomlkit.dumps(data, sort_keys=sort_keys) 
+39 if _strict and key not in annotations: 
+40 raise ConfigErrorExtraKey(cls=self.__class__, key=key, value=value) 
+41 
+42 if _strict and not check_type(value, annotations[key]) and not (value is
+None and _allow_none): 
+43 raise ConfigErrorInvalidType(expected_type=annotations[key], key=key,
+value=value) 
+44 
+45 setattr(self, key, value) 
 46 
-47 
-48def asjson(inst: typing.Any, **kw: typing.Any) -> str: 
-49 """ 
-50 Dump a config instance to json (recursively). 
-51 """ 
-52 data = asdict(inst) 
-53 return json.dumps(data, **kw) 
-54 
-55 
-56def asyaml(inst: typing.Any, **kw: typing.Any) -> str: 
-57 """ 
-58 Dump a config instance to yaml (recursively). 
+47 def update(self, _strict: bool = True, _allow_none: bool = False, **values:
+typing.Any) -> None: 
+48 """ 
+49 Update values on this config. 
+50 
+51 Args: 
+52 _strict: allow wrong types? 
+53 _allow_none: allow None or skip those entries? 
+54 **values: key: value pairs in the right types to update. 
+55 """ 
+56 return self._update(_strict, _allow_none, **values) 
+57 
+58 def _format(self, string: str) -> str: 
 59 """ 
-60 data = asdict(inst) 
-61 output = yaml.dump(data, encoding=None, **kw) 
-62 # output is already a str but mypy doesn't know that 
-63 return typing.cast(str, output) 
+60 Format the config data into a string template. 
+61 
+62 Replacement for string.format(**config), which is only possible for
+MutableMappings. 
+63 MutableMapping does not work well with our Singleton Metaclass. 
+64 """ 
+65 return string.format(**self.__dict__) 
+66 
+67 
+68# also expose as separate function: 
+69def update(instance: typing.Any, _strict: bool = True, _allow_none: bool =
+False, **values: typing.Any) -> None: 
+70 """ 
+71 Update values on a config. 
+72 
+73 Args: 
+74 instance: config instance to update 
+75 _strict: allow wrong types? 
+76 _allow_none: allow None or skip those entries? 
+77 **values: key: value pairs in the right types to update. 
+78 """ 
+79 return TypedConfig._update(instance, _strict, _allow_none, **values) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 16:40 +0200
+at 2023-06-21 15:50 +0200
```

### Comparing `configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_errors_py.html` & `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html` & `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html` & `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">8 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">8<span class="text"> run</span></button>
+            <span class="text">9 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">9<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_shared_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_singleton_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -80,54 +80,56 @@
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">File contains logic to do with the 'postpone' feature.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">errors</span> <span class="key">import</span> <span class="nam">IsPostponedError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">singleton</span> <span class="key">import</span> <span class="nam">Singleton</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">class</span> <span class="nam">Postponed</span><span class="op">(</span><span class="nam">Singleton</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="str">    Class returned by `postpone` below.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="key">def</span> <span class="nam">__get__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">instance</span><span class="op">:</span> <span class="nam">type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">owner</span><span class="op">:</span> <span class="nam">type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Never</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">        This magic method is called when a property is accessed.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="str">             someclass.someprop will trigger the __get__ of `someprop`</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">            instance: the class on which the postponed property is defined,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">            owner: `SingletonMeta`</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">raise</span> <span class="nam">IsPostponedError</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="key">def</span> <span class="nam">postpone</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    Can be used to mark a property as postponed, meaning the user will fill it in later (they promose).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="str">    If they don't fill it in and still try to use it, they will be met with a IsPostponedError.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="key">return</span> <span class="nam">Postponed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">typing_extensions</span> <span class="key">import</span> <span class="nam">Never</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">errors</span> <span class="key">import</span> <span class="nam">IsPostponedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">singleton</span> <span class="key">import</span> <span class="nam">Singleton</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">class</span> <span class="nam">Postponed</span><span class="op">(</span><span class="nam">Singleton</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="str">    Class returned by `postpone` below.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="key">def</span> <span class="nam">__get__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">instance</span><span class="op">:</span> <span class="nam">type</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">owner</span><span class="op">:</span> <span class="nam">type</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Never</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="str">        This magic method is called when a property is accessed.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">             someclass.someprop will trigger the __get__ of `someprop`</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">            instance: the class on which the postponed property is defined,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">            owner: `SingletonMeta`</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="key">raise</span> <span class="nam">IsPostponedError</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="key">def</span> <span class="nam">postpone</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="str">    Can be used to mark a property as postponed, meaning the user will fill it in later (they promose).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t"><span class="str">    If they don't fill it in and still try to use it, they will be met with a IsPostponedError.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">return</span> <span class="nam">Postponed</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_6c7dc8b73849fb97_loaders_shared_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40_singleton_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-15 14:30 +0200
+            created at 2023-06-20 10:44 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,54 +5,55 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 8 statements   8 run 0 missing 0 excluded *****
+***** 9 statements   9 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-20 10:44 +0200
 
 
 1""" 
 2File contains logic to do with the 'postpone' feature. 
 3""" 
 4 
-5import typing 
+5from typing import Any 
 6 
-7from .errors import IsPostponedError 
-8from .singleton import Singleton 
-9 
-10 
-11class Postponed(Singleton): 
-12 """ 
-13 Class returned by `postpone` below. 
+7from typing_extensions import Never 
+8 
+9from .errors import IsPostponedError 
+10from .singleton import Singleton 
+11 
+12 
+13class Postponed(Singleton): 
 14 """ 
-15 
-16 def __get__(self, instance: type[typing.Any], owner: type[typing.Any]) -
-> typing.Never: 
-17 """ 
-18 This magic method is called when a property is accessed. 
-19 
-20 Example: 
-21 someclass.someprop will trigger the __get__ of `someprop` 
-22 
-23 Args: 
-24 instance: the class on which the postponed property is defined, 
-25 owner: `SingletonMeta` 
-26 """ 
-27 raise IsPostponedError() 
-28 
-29 
-30def postpone() -> typing.Any: 
-31 """ 
-32 Can be used to mark a property as postponed, meaning the user will fill it
+15 Class returned by `postpone` below. 
+16 """ 
+17 
+18 def __get__(self, instance: type[Any], owner: type[Any]) -> Never: 
+19 """ 
+20 This magic method is called when a property is accessed. 
+21 
+22 Example: 
+23 someclass.someprop will trigger the __get__ of `someprop` 
+24 
+25 Args: 
+26 instance: the class on which the postponed property is defined, 
+27 owner: `SingletonMeta` 
+28 """ 
+29 raise IsPostponedError() 
+30 
+31 
+32def postpone() -> Any: 
+33 """ 
+34 Can be used to mark a property as postponed, meaning the user will fill it
 in later (they promose). 
-33 
-34 If they don't fill it in and still try to use it, they will be met with a
+35 
+36 If they don't fill it in and still try to use it, they will be met with a
 IsPostponedError. 
-35 """ 
-36 return Postponed() 
+37 """ 
+38 return Postponed() 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-15 14:30 +0200
+at 2023-06-20 10:44 +0200
```

### Comparing `configuraptor-1.7.2/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html` & `configuraptor-1.8.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/favicon_32.png` & `configuraptor-1.8.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/index.html` & `configuraptor-1.8.0/htmlcov/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-19 17:39 +0200
+            created at 2023-06-21 15:50 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -73,18 +73,18 @@
                 <td>6</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="6 6">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_cls_py.html">src/configuraptor/cls.py</a></td>
-                <td>18</td>
+                <td>24</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="18 18">100%</td>
+                <td class="right" data-ratio="24 24">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_core_py.html">src/configuraptor/core.py</a></td>
                 <td>156</td>
                 <td>0</td>
                 <td>3</td>
                 <td class="right" data-ratio="156 156">100%</td>
@@ -110,79 +110,65 @@
                 <td>0</td>
                 <td class="right" data-ratio="2 2">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_6c7dc8b73849fb97___init___py.html">src/configuraptor/loaders/__init__.py</a></td>
                 <td>11</td>
                 <td>0</td>
-                <td>1</td>
+                <td>0</td>
                 <td class="right" data-ratio="11 11">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_6c7dc8b73849fb97__types_py.html">src/configuraptor/loaders/_types.py</a></td>
                 <td>4</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="4 4">100%</td>
             </tr>
             <tr class="file">
-                <td class="name left"><a href="d_6c7dc8b73849fb97_loaders_310_py.html">src/configuraptor/loaders/loaders_310.py</a></td>
-                <td>5</td>
-                <td>0</td>
-                <td>6</td>
-                <td class="right" data-ratio="5 5">100%</td>
-            </tr>
-            <tr class="file">
-                <td class="name left"><a href="d_6c7dc8b73849fb97_loaders_311_py.html">src/configuraptor/loaders/loaders_311.py</a></td>
-                <td>6</td>
-                <td>0</td>
-                <td>2</td>
-                <td class="right" data-ratio="6 6">100%</td>
-            </tr>
-            <tr class="file">
                 <td class="name left"><a href="d_6c7dc8b73849fb97_loaders_shared_py.html">src/configuraptor/loaders/loaders_shared.py</a></td>
                 <td>14</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="14 14">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_postpone_py.html">src/configuraptor/postpone.py</a></td>
-                <td>8</td>
+                <td>9</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="8 8">100%</td>
+                <td class="right" data-ratio="9 9">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_eb75b6cf8f5eab40_singleton_py.html">src/configuraptor/singleton.py</a></td>
                 <td>13</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="13 13">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>314</td>
+                <td>310</td>
                 <td>0</td>
-                <td>12</td>
-                <td class="right" data-ratio="314 314">100%</td>
+                <td>3</td>
+                <td class="right" data-ratio="310 310">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-19 17:39 +0200
+            created at 2023-06-21 15:50 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_eb75b6cf8f5eab40_singleton_py.html"/>
         <a id="nextFileLink" class="nav" href="d_eb75b6cf8f5eab40___about___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -2,30 +2,28 @@
 ****** Coverage report: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-06-19 17:39 +0200
+coverage.py_v7.2.7, created at 2023-06-21 15:50 +0200
 
-Module                                   statements missing excluded coverage
-src/configuraptor/__about__.py           1          0       0        100%
-src/configuraptor/__init__.py            6          0       0        100%
-src/configuraptor/cls.py                 18         0       0        100%
-src/configuraptor/core.py                156        0       3        100%
-src/configuraptor/dump.py                31         0       0        100%
-src/configuraptor/errors.py              39         0       0        100%
-src/configuraptor/helpers.py             2          0       0        100%
-src/configuraptor/loaders/__init__.py    11         0       1        100%
-src/configuraptor/loaders/_types.py      4          0       0        100%
-src/configuraptor/loaders/loaders_310.py 5          0       6        100%
-src/configuraptor/loaders/loaders_311.py 6          0       2        100%
-src/configuraptor/loaders/               14         0       0        100%
+Module                                statements missing excluded coverage
+src/configuraptor/__about__.py        1          0       0        100%
+src/configuraptor/__init__.py         6          0       0        100%
+src/configuraptor/cls.py              24         0       0        100%
+src/configuraptor/core.py             156        0       3        100%
+src/configuraptor/dump.py             31         0       0        100%
+src/configuraptor/errors.py           39         0       0        100%
+src/configuraptor/helpers.py          2          0       0        100%
+src/configuraptor/loaders/__init__.py 11         0       0        100%
+src/configuraptor/loaders/_types.py   4          0       0        100%
+src/configuraptor/loaders/            14         0       0        100%
 loaders_shared.py
-src/configuraptor/postpone.py            8          0       0        100%
-src/configuraptor/singleton.py           13         0       0        100%
-Total                                    314        0       12       100%
+src/configuraptor/postpone.py         9          0       0        100%
+src/configuraptor/singleton.py        13         0       0        100%
+Total                                 310        0       3        100%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-06-19 17:39 +0200
+coverage.py_v7.2.7, created at 2023-06-21 15:50 +0200
  ____
```

### Comparing `configuraptor-1.7.2/htmlcov/keybd_closed.png` & `configuraptor-1.8.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/keybd_open.png` & `configuraptor-1.8.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/htmlcov/status.json` & `configuraptor-1.8.0/htmlcov/status.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9936342592592593%*

 * *Differences: {"'files'": "{'d_eb75b6cf8f5eab40___about___py': {'hash': '3e93cb54154f78c6f81f6feef3376f69'}, "*

 * *            "'d_eb75b6cf8f5eab40___init___py': {'hash': 'd5c1f5ac693aae2044dffde7eccaae57'}, "*

 * *            "'d_eb75b6cf8f5eab40_cls_py': {'hash': 'b1f068469f7f94c16e9d267b087e8806', 'index': "*

 * *            "{'nums': {insert: [(2, 24)], delete: [2]}}}, 'd_6c7dc8b73849fb97___init___py': "*

 * *            "{'hash': '2d2ad3b6f895f556c8c360fc94280b0f', 'index': {'nums': {insert: [(3, 0)], "*

 * *            "delete: [3]}}}, 'd […]*

```diff
@@ -184,32 +184,32 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/typedconfig/singleton.py"
             }
         },
         "d_6c7dc8b73849fb97___init___py": {
-            "hash": "2ef72ea4377e2966b657f2d94ba1a8c2",
+            "hash": "2d2ad3b6f895f556c8c360fc94280b0f",
             "index": {
                 "html_filename": "d_6c7dc8b73849fb97___init___py.html",
                 "nums": [
                     0,
                     1,
                     11,
-                    1,
+                    0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/__init__.py"
             }
         },
         "d_6c7dc8b73849fb97__types_py": {
-            "hash": "1a491a5575599b4c1c0e95472348d26b",
+            "hash": "d62d8dca9ea1bbb2963a68a70da33b71",
             "index": {
                 "html_filename": "d_6c7dc8b73849fb97__types_py.html",
                 "nums": [
                     0,
                     1,
                     4,
                     0,
@@ -218,49 +218,49 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/_types.py"
             }
         },
         "d_6c7dc8b73849fb97_loaders_310_py": {
-            "hash": "1afd90c369f649538d18695e2737585d",
+            "hash": "5369852c611fc5bc9cb9cc6724f53e1c",
             "index": {
                 "html_filename": "d_6c7dc8b73849fb97_loaders_310_py.html",
                 "nums": [
                     0,
                     1,
                     5,
                     6,
-                    0,
+                    5,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/loaders_310.py"
             }
         },
         "d_6c7dc8b73849fb97_loaders_311_py": {
-            "hash": "74469c8e02e9fa066fcf5c98bf9ca8a8",
+            "hash": "6b2bc95025fcd6cd3fc7c4b60c09878e",
             "index": {
                 "html_filename": "d_6c7dc8b73849fb97_loaders_311_py.html",
                 "nums": [
                     0,
                     1,
                     6,
                     2,
-                    0,
+                    3,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/loaders_311.py"
             }
         },
         "d_6c7dc8b73849fb97_loaders_shared_py": {
-            "hash": "3c629c3aee227f260f4f55d7d252b644",
+            "hash": "6a123f87678e906f6ec34f5b7b9cce20",
             "index": {
                 "html_filename": "d_6c7dc8b73849fb97_loaders_shared_py.html",
                 "nums": [
                     0,
                     1,
                     14,
                     0,
@@ -269,15 +269,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/loaders/loaders_shared.py"
             }
         },
         "d_eb75b6cf8f5eab40___about___py": {
-            "hash": "c751a6ade0f2b1e3c963979cd459801f",
+            "hash": "3e93cb54154f78c6f81f6feef3376f69",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40___about___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -286,15 +286,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/__about__.py"
             }
         },
         "d_eb75b6cf8f5eab40___init___py": {
-            "hash": "06dbb9f67d79162cdd2611932d9db344",
+            "hash": "d5c1f5ac693aae2044dffde7eccaae57",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40___init___py.html",
                 "nums": [
                     0,
                     1,
                     6,
                     0,
@@ -303,21 +303,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/__init__.py"
             }
         },
         "d_eb75b6cf8f5eab40_cls_py": {
-            "hash": "4e1850bc37aea80a61e66e116f397d18",
+            "hash": "b1f068469f7f94c16e9d267b087e8806",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_cls_py.html",
                 "nums": [
                     0,
                     1,
-                    18,
+                    24,
                     0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/cls.py"
@@ -337,15 +337,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/core.py"
             }
         },
         "d_eb75b6cf8f5eab40_dump_py": {
-            "hash": "d64f111484683805138ede1d7542d62d",
+            "hash": "233c5134a82e980ecd67b145aae52ea4",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_dump_py.html",
                 "nums": [
                     0,
                     1,
                     31,
                     0,
@@ -388,21 +388,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/helpers.py"
             }
         },
         "d_eb75b6cf8f5eab40_postpone_py": {
-            "hash": "5eb8807f612a5d71ec845af18bc94fd4",
+            "hash": "02772d48778436f9a987a27900770586",
             "index": {
                 "html_filename": "d_eb75b6cf8f5eab40_postpone_py.html",
                 "nums": [
                     0,
                     1,
-                    8,
+                    9,
                     0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/configuraptor/postpone.py"
```

### Comparing `configuraptor-1.7.2/htmlcov/style.css` & `configuraptor-1.8.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/pytest_examples/some.toml` & `configuraptor-1.8.0/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/src/configuraptor/__init__.py` & `configuraptor-1.8.0/src/configuraptor/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/src/configuraptor/cls.py` & `configuraptor-1.8.0/src/configuraptor/cls.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,14 +51,23 @@
         Args:
             _strict: allow wrong types?
             _allow_none: allow None or skip those entries?
             **values: key: value pairs in the right types to update.
         """
         return self._update(_strict, _allow_none, **values)
 
+    def _format(self, string: str) -> str:
+        """
+        Format the config data into a string template.
+
+        Replacement for string.format(**config), which is only possible for MutableMappings.
+        MutableMapping does not work well with our Singleton Metaclass.
+        """
+        return string.format(**self.__dict__)
+
 
 # also expose as separate function:
 def update(instance: typing.Any, _strict: bool = True, _allow_none: bool = False, **values: typing.Any) -> None:
     """
     Update values on a config.
 
     Args:
```

### Comparing `configuraptor-1.7.2/src/configuraptor/core.py` & `configuraptor-1.8.0/src/configuraptor/core.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/src/configuraptor/dump.py` & `configuraptor-1.8.0/src/configuraptor/dump.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/src/configuraptor/errors.py` & `configuraptor-1.8.0/src/configuraptor/errors.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/src/configuraptor/postpone.py` & `configuraptor-1.8.0/src/configuraptor/postpone.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/src/configuraptor/singleton.py` & `configuraptor-1.8.0/src/configuraptor/singleton.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Can be used as a metaclass:
     Example:
         class AbstractConfig(metaclass=Singleton):
 
     Source: https://stackoverflow.com/questions/6760685/creating-a-singleton-in-python
     """
 
-    _instances: dict[typing.Type[typing.Any], typing.Type[typing.Any]] = {}
+    _instances: typing.ClassVar[dict[typing.Type[typing.Any], typing.Type[typing.Any]]] = {}
 
     def __call__(self, *args: typing.Any, **kwargs: typing.Any) -> typing.Type[typing.Any]:
         """
         When a class is instantiated (e.g. `AbstractConfig()`), __call__ is called. This overrides the default behavior.
         """
         if self not in self._instances:
             self._instances[self] = super(SingletonMeta, self).__call__(*args, **kwargs)
```

### Comparing `configuraptor-1.7.2/src/configuraptor/loaders/loaders_shared.py` & `configuraptor-1.8.0/src/configuraptor/loaders/loaders_shared.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/tests/test_dumps.py` & `configuraptor-1.8.0/tests/test_dumps.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/tests/test_json_yaml.py` & `configuraptor-1.8.0/tests/test_json_yaml.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/tests/test_postponed.py` & `configuraptor-1.8.0/tests/test_postponed.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/tests/test_singleton.py` & `configuraptor-1.8.0/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/tests/test_toml_basic.py` & `configuraptor-1.8.0/tests/test_toml_basic.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/tests/test_toml_dataclass.py` & `configuraptor-1.8.0/tests/test_toml_dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/tests/test_toml_existing.py` & `configuraptor-1.8.0/tests/test_toml_existing.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/tests/test_toml_typedconfig_class.py` & `configuraptor-1.8.0/tests/test_toml_typedconfig_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import math
 import typing
 
 import pytest
 
 from src import configuraptor
 from src.configuraptor.errors import ConfigError, ConfigErrorInvalidType, ConfigErrorExtraKey
-
 from .constants import EMPTY_FILE, EXAMPLE_FILE, _load_toml
 
 
 def test_example_is_valid_toml():
     data = _load_toml()
 
     assert data
@@ -144,8 +143,13 @@
     config = MyConfig.load({"update": True}, key="")
 
     assert config.update == True
     config._update(update=False)
     assert config.update == False
 
     configuraptor.update(config, update=True)
-    assert config.update == True
+    assert config.update == True
+
+def test_mapping():
+    tool = Tool.load(EXAMPLE_FILE, key="tool")
+
+    assert tool._format("{first.string}") == "src"
```

### Comparing `configuraptor-1.7.2/LICENSE.txt` & `configuraptor-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/README.md` & `configuraptor-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `configuraptor-1.7.2/pyproject.toml` & `configuraptor-1.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 src-layout = true
 
 [tool.setuptools.package-data]
 "configuraptor" = ["py.typed"]
 
 [project.optional-dependencies]
 dev = [
-    "su6[all]; python_version >= '3.11'",
+    "su6[all]",
     "hatch",
     "types-PyYAML",
     "pytest-mypy-testing",
 ]
 
 [project.urls]
 Documentation = "https://github.com/trialandsuccess/configuraptor#readme"
@@ -120,14 +120,16 @@
 ]
 unfixable = [
     # Don't touch unused imports
     "F401",
 ]
 extend-exclude = ["*.bak/", "venv*/"]
 
+ignore = ["RUF013"] # = implicit Optional
+
 [tool.bandit]
 # bandit -c pyproject.toml -r .
 exclude_dirs = [".bak", "venv"]
 skips = [
     "B108", # hard coded /tmp/... files are fine for me tbh
 ]
```

### Comparing `configuraptor-1.7.2/PKG-INFO` & `configuraptor-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuraptor
-Version: 1.7.2
+Version: 1.8.0
 Summary: Load toml/yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/configuraptor#readme
 Project-URL: Issues, https://github.com/trialandsuccess/configuraptor/issues
 Project-URL: Source, https://github.com/trialandsuccess/configuraptor
 Author-email: Robin van der Noord <robin@trialandsuccess.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -19,15 +19,15 @@
 Requires-Dist: pyyaml
 Requires-Dist: tomli
 Requires-Dist: tomli-w
 Requires-Dist: typeguard
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: pytest-mypy-testing; extra == 'dev'
-Requires-Dist: su6[all]; python_version >= '3.11' and extra == 'dev'
+Requires-Dist: su6[all]; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img 
         align="center" 
         src="https://raw.githubusercontent.com/trialandsuccess/configuraptor/master/_static/configuraptor_circle.png"
```

