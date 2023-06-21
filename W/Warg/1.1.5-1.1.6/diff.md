# Comparing `tmp/Warg-1.1.5.tar.gz` & `tmp/Warg-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Warg-1.1.5.tar", last modified: Mon Jun 12 13:03:27 2023, max compression
+gzip compressed data, was "Warg-1.1.6.tar", last modified: Wed Jun 21 08:55:19 2023, max compression
```

## Comparing `Warg-1.1.5.tar` & `Warg-1.1.6.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.869754 Warg-1.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.853754 Warg-1.1.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-12 13:03:21.000000 Warg-1.1.5/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:21.000000 Warg-1.1.5/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 13:03:21.000000 Warg-1.1.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 13:03:21.000000 Warg-1.1.5/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-12 13:03:21.000000 Warg-1.1.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-12 13:03:21.000000 Warg-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-12 13:03:27.869754 Warg-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-12 13:03:21.000000 Warg-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-12 13:03:21.000000 Warg-1.1.5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.853754 Warg-1.1.5/Warg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-12 13:03:27.000000 Warg-1.1.5/Warg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-12 13:03:27.000000 Warg-1.1.5/Warg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:03:27.000000 Warg-1.1.5/Warg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-12 13:03:27.000000 Warg-1.1.5/Warg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 13:03:27.000000 Warg-1.1.5/Warg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.853754 Warg-1.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 13:03:21.000000 Warg-1.1.5/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-12 13:03:21.000000 Warg-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 13:03:21.000000 Warg-1.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-12 13:03:27.869754 Warg-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-12 13:03:21.000000 Warg-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.857754 Warg-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-12 13:03:21.000000 Warg-1.1.5/tests/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-12 13:03:21.000000 Warg-1.1.5/tests/test_ast_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-12 13:03:21.000000 Warg-1.1.5/tests/test_auto_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-12 13:03:21.000000 Warg-1.1.5/tests/test_collective.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-12 13:03:21.000000 Warg-1.1.5/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-12 13:03:21.000000 Warg-1.1.5/tests/test_gdkc.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-12 13:03:21.000000 Warg-1.1.5/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-06-12 13:03:21.000000 Warg-1.1.5/tests/test_kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-12 13:03:21.000000 Warg-1.1.5/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-12 13:03:21.000000 Warg-1.1.5/tests/test_nod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-12 13:03:21.000000 Warg-1.1.5/tests/test_post_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-12 13:03:21.000000 Warg-1.1.5/tests/test_singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.861754 Warg-1.1.5/warg/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.861754 Warg-1.1.5/warg/ast_ops/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/ast_ops/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/ast_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/ast_ops/arg_indentifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/ast_ops/first_arg_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.861754 Warg-1.1.5/warg/bases/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/bases/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/bases/property_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/boolean_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/business.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.861754 Warg-1.1.5/warg/colors/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/colors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/colors/color_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/colors/css_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/colors/label_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/config_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/context_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.861754 Warg-1.1.5/warg/data_structures/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/data_structures/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/data_structures/auto_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/data_structures/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16671 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/data_structures/named_ordered_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/data_structures/ordered_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/data_structures/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/datetimes.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.861754 Warg-1.1.5/warg/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/decorators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.865754 Warg-1.1.5/warg/decorators/caching/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/decorators/caching/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/decorators/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/decorators/caching/look_up_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/decorators/caching/property_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/decorators/exporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/decorators/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/decorators/kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/decorators/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/decorators/wrapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/gdkc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.865754 Warg-1.1.5/warg/generators/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/generators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/generators/cyclic_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/generators/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/generators/mapping_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/generators/zipping_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/map_itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.865754 Warg-1.1.5/warg/math_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/math_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/math_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/math_utilities/multiples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/math_utilities/ordinals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/math_utilities/powers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.865754 Warg-1.1.5/warg/metas/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/metas/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/metas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/metas/post_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/metas/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.865754 Warg-1.1.5/warg/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/mixins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/mixins/dict_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/mixins/ordinal_index_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/mixins/private.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/ode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:27.869754 Warg-1.1.5/warg/os_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/os_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/os_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/os_utilities/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/os_utilities/os_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/os_utilities/path_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/os_utilities/path_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/os_utilities/platform_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/replication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/styling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-12 13:03:21.000000 Warg-1.1.5/warg/typing_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.820976 Warg-1.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.804974 Warg-1.1.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-21 08:55:06.000000 Warg-1.1.6/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:06.000000 Warg-1.1.6/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 08:55:06.000000 Warg-1.1.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 08:55:07.000000 Warg-1.1.6/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-21 08:55:07.000000 Warg-1.1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-21 08:55:07.000000 Warg-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-21 08:55:19.820976 Warg-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-21 08:55:07.000000 Warg-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-21 08:55:07.000000 Warg-1.1.6/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.804974 Warg-1.1.6/Warg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-21 08:55:19.000000 Warg-1.1.6/Warg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-21 08:55:19.000000 Warg-1.1.6/Warg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:55:19.000000 Warg-1.1.6/Warg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-21 08:55:19.000000 Warg-1.1.6/Warg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 08:55:19.000000 Warg-1.1.6/Warg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.804974 Warg-1.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 08:55:07.000000 Warg-1.1.6/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-21 08:55:07.000000 Warg-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 08:55:07.000000 Warg-1.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 08:55:19.820976 Warg-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-21 08:55:07.000000 Warg-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.808975 Warg-1.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_ast_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_auto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_gdkc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_nod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_post_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-21 08:55:07.000000 Warg-1.1.6/tests/test_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.812975 Warg-1.1.6/warg/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.812975 Warg-1.1.6/warg/ast_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/ast_ops/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/ast_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/ast_ops/arg_indentifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/ast_ops/first_arg_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.812975 Warg-1.1.6/warg/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/bases/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/bases/property_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/boolean_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/business.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.812975 Warg-1.1.6/warg/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/colors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/colors/color_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/colors/css_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/colors/label_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/config_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/context_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/contexts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.812975 Warg-1.1.6/warg/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/auto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16671 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/named_ordered_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/ordered_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/data_structures/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.816975 Warg-1.1.6/warg/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.816975 Warg-1.1.6/warg/decorators/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/caching/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/caching/look_up_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/caching/property_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/exporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/decorators/wrapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/gdkc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.816975 Warg-1.1.6/warg/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/generators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/generators/cyclic_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/generators/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/generators/mapping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/generators/zipping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/map_itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.816975 Warg-1.1.6/warg/math_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/math_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/math_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/math_utilities/multiples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/math_utilities/ordinals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/math_utilities/powers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.816975 Warg-1.1.6/warg/metas/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/metas/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/metas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/metas/post_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/metas/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.820976 Warg-1.1.6/warg/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/mixins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/mixins/dict_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/mixins/ordinal_index_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/mixins/private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/ode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:55:19.820976 Warg-1.1.6/warg/os_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/os_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/path_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/path_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/os_utilities/platform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-21 08:55:07.000000 Warg-1.1.6/warg/typing_extension.py
```

### Comparing `Warg-1.1.5/.github/CODE_OF_CONDUCT.md` & `Warg-1.1.6/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/LICENSE.md` & `Warg-1.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/PKG-INFO` & `Warg-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.1.5
+Version: 1.1.6
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -20,17 +20,17 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
-Provides-Extra: setup
 Provides-Extra: dev
 Provides-Extra: tests
+Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![warg](.github/images/warg.svg)-->
 
 <p align="center">
   <img src=".github/images/warg.svg" alt='Warg' />
```

### Comparing `Warg-1.1.5/README.md` & `Warg-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/SECURITY.md` & `Warg-1.1.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/Warg.egg-info/PKG-INFO` & `Warg-1.1.6/Warg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.1.5
+Version: 1.1.6
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -20,17 +20,17 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
-Provides-Extra: setup
 Provides-Extra: dev
 Provides-Extra: tests
+Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![warg](.github/images/warg.svg)-->
 
 <p align="center">
   <img src=".github/images/warg.svg" alt='Warg' />
```

### Comparing `Warg-1.1.5/Warg.egg-info/SOURCES.txt` & `Warg-1.1.6/Warg.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 warg/exceptions.py
 warg/functions.py
 warg/gdkc.py
 warg/importing.py
 warg/manipulation.py
 warg/map_itertools.py
 warg/ode.py
+warg/packages.py
 warg/plugin.py
 warg/replication.py
 warg/strings.py
 warg/styling.py
 warg/text.py
 warg/typing_extension.py
 warg/ast_ops/README.md
```

### Comparing `Warg-1.1.5/Warg.egg-info/requires.txt` & `Warg-1.1.6/Warg.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 setuptools>=60.9.3
 
 [all]
-pytest-runner
-pytest-cov>=2.6.1
-pip>=19.0.3
-black>=18.9b0
-tox
-pytest>=4.3.0
+apppath
 warg
+tox
+sphinxcontrib-programoutput
 setuptools>=60.9.3
-apppath
-coveralls>=1.6.0
 wheel>=0.33.0
-twine>=1.13.0
+black>=18.9b0
 sphinx
-sphinxcontrib-programoutput
-
-[dev]
-pytest-cov>=2.6.1
 pip>=19.0.3
-black>=18.9b0
-tox
 pytest-runner
+twine>=1.13.0
+coveralls>=1.6.0
+pytest-cov>=2.6.1
 pytest>=4.3.0
+
+[dev]
+apppath
+tox
 warg
+sphinxcontrib-programoutput
 setuptools>=60.9.3
-coveralls>=1.6.0
 wheel>=0.33.0
-apppath
-sphinxcontrib-programoutput
+black>=18.9b0
 sphinx
+pip>=19.0.3
+pytest-runner
 twine>=1.13.0
+coveralls>=1.6.0
+pytest-cov>=2.6.1
+pytest>=4.3.0
 
 [docs]
-warg
 apppath
-sphinx
+warg
 sphinxcontrib-programoutput
+sphinx
 
 [setup]
 pytest-runner
 
 [tests]
-pytest-cov>=2.6.1
 tox
+pytest-cov>=2.6.1
 pytest>=4.3.0
```

### Comparing `Warg-1.1.5/pyproject.toml` & `Warg-1.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/setup.py` & `Warg-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/tests/test_arguments.py` & `Warg-1.1.6/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/tests/test_ast_ops.py` & `Warg-1.1.6/tests/test_ast_ops.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/tests/test_auto_dict.py` & `Warg-1.1.6/tests/test_auto_dict.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/tests/test_collective.py` & `Warg-1.1.6/tests/test_collective.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/tests/test_gdkc.py` & `Warg-1.1.6/tests/test_gdkc.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/tests/test_imports.py` & `Warg-1.1.6/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/tests/test_kw_passing.py` & `Warg-1.1.6/tests/test_kw_passing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/tests/test_nod.py` & `Warg-1.1.6/tests/test_nod.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/tests/test_post_init.py` & `Warg-1.1.6/tests/test_post_init.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/tests/test_singleton.py` & `Warg-1.1.6/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/__init__.py` & `Warg-1.1.6/warg/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from warnings import warn
 
 import pkg_resources
 
 __project__ = "Warg"
 
 __author__ = "Christian Heider Nielsen"
-__version__ = "1.1.5"
+__version__ = "1.1.6"
 __doc__ = r"""
 Created on 27/04/2019
 
 @author: cnheider
 
 """
 
@@ -26,15 +26,14 @@
 #    __doc__ += this_init_file.read()
 
 # __all__ = ["PROJECT_APP_PATH", "PROJECT_NAME", "PROJECT_VERSION", "get_version"] # let everything be accessable from base warg import
 
 
 from typing import Any
 
-
 try:
     # from .ode import * # Silly thing
     from .data_structures import *
     from .arguments import *
     from .gdkc import *
     from .mixins import *
     from .decorators import *
@@ -58,37 +57,24 @@
     from .manipulation import *
     from .replication import *
     from .styling import *
     from .strings import *
     from .contexts import *
     from .config_shell import *
     from .colors import *
+    from .packages import *
 except ImportError as ix:
     this_package_name = Path(__file__).parent.name
     this_package_reqs = Path(__file__).parent.parent / f"requirements.txt"
     if this_package_reqs.exists():
         print(
             f"Make sure requirements is installed for {this_package_name}, see {this_package_reqs}"
         )  # TODO: PARSE WHAT is missing and print
     raise ix
 
-
-def dist_is_editable(dist: Any) -> bool:
-    """
-    Return True if given Distribution is an editable installation."""
-    import sys
-    from pathlib import Path
-
-    for path_item in sys.path:
-        egg_link = Path(path_item) / f"{dist.project_name}.egg-link"
-        if egg_link.is_file():
-            return True
-    return False
-
-
 PROJECT_NAME = __project__.lower().strip().replace(" ", "_")
 PROJECT_VERSION = __version__
 PROJECT_YEAR = 2018
 PROJECT_AUTHOR = __author__.lower().strip().replace(" ", "_")
 PROJECT_ORGANISATION = "pything"
 
 __url__ = f"https://github.com/{PROJECT_ORGANISATION}/{PROJECT_NAME}"
```

### Comparing `Warg-1.1.5/warg/arguments.py` & `Warg-1.1.6/warg/arguments.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/ast_ops/arg_indentifier.py` & `Warg-1.1.6/warg/ast_ops/arg_indentifier.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/ast_ops/first_arg_identifier.py` & `Warg-1.1.6/warg/ast_ops/first_arg_identifier.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/bases/property_settings.py` & `Warg-1.1.6/warg/bases/property_settings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/boolean_tests.py` & `Warg-1.1.6/warg/boolean_tests.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/business.py` & `Warg-1.1.6/warg/business.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/colors/color_conversion.py` & `Warg-1.1.6/warg/colors/color_conversion.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/colors/css_colors.py` & `Warg-1.1.6/warg/colors/css_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/colors/label_colors.py` & `Warg-1.1.6/warg/colors/label_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/config_shell.py` & `Warg-1.1.6/warg/config_shell.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/context_wrapper.py` & `Warg-1.1.6/warg/context_wrapper.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/contexts.py` & `Warg-1.1.6/warg/contexts.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/data_structures/auto_dict.py` & `Warg-1.1.6/warg/data_structures/auto_dict.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/data_structures/mappings.py` & `Warg-1.1.6/warg/data_structures/mappings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/data_structures/named_ordered_dictionary.py` & `Warg-1.1.6/warg/data_structures/named_ordered_dictionary.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/data_structures/ordered_set.py` & `Warg-1.1.6/warg/data_structures/ordered_set.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/data_structures/sequences.py` & `Warg-1.1.6/warg/data_structures/sequences.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/datetimes.py` & `Warg-1.1.6/warg/datetimes.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/debug.py` & `Warg-1.1.6/warg/debug.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/decorators/caching/look_up_table.py` & `Warg-1.1.6/warg/decorators/caching/look_up_table.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/decorators/caching/property_caching.py` & `Warg-1.1.6/warg/decorators/caching/property_caching.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/decorators/exporting.py` & `Warg-1.1.6/warg/decorators/exporting.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/decorators/hashing.py` & `Warg-1.1.6/warg/decorators/hashing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/decorators/kw_passing.py` & `Warg-1.1.6/warg/decorators/kw_passing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/decorators/timing.py` & `Warg-1.1.6/warg/decorators/timing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/decorators/wrapping.py` & `Warg-1.1.6/warg/decorators/wrapping.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/exceptions.py` & `Warg-1.1.6/warg/exceptions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/functions.py` & `Warg-1.1.6/warg/functions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/gdkc.py` & `Warg-1.1.6/warg/gdkc.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/generators/cyclic_generators.py` & `Warg-1.1.6/warg/generators/cyclic_generators.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/generators/filtering.py` & `Warg-1.1.6/warg/generators/filtering.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/generators/mapping_generator.py` & `Warg-1.1.6/warg/generators/mapping_generator.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/generators/zipping_generator.py` & `Warg-1.1.6/warg/generators/zipping_generator.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/importing.py` & `Warg-1.1.6/warg/importing.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 ]
 
 import importlib
 import sys
 from importlib import reload
 from importlib.util import find_spec
 from pathlib import Path
-from typing import Optional, Any, Union, List
+from typing import Optional, Any, Union, List, Iterable
 from warnings import warn
 
-from warg import passes_kws_to
+import pkg_resources
 
+from warg import passes_kws_to
 
 """
 PRELOADED_MODULES = set()
 def init():
   # local imports to keep things neat
   from sys import modules
 
@@ -55,29 +56,35 @@
     except:
       # there are some problems that are swept under the rug here
       pass
 init()
 """
 
 
-def contain(q, s):
+def contain(q: Any, s: Iterable) -> bool:
     return q in s
 
 
-def reload_module(module_name: str, containment_test: callable = contain):
+def reload_module(module_name: str, containment_test: callable = contain) -> None:
     if module_name in sys.modules:
-        reload_set = {x for x in sys.modules if contain(module_name, x)}
+        reload_set = {x for x in sys.modules if containment_test(module_name, x)}
         for a in reload_set:
             del sys.modules[a]
             # importlib.reload(sys.modules[mod_str]) #DOES NOT WORK ON FROM IMPORTS...
             sys.modules[a] = importlib.import_module(a)
     else:
         sys.modules[module_name] = importlib.import_module(module_name)
 
 
+def reload_requirements(requirements_path: Path, containment_test: callable = contain) -> None:
+    with open(requirements_path) as f:
+        for r in pkg_resources.parse_requirements(f.readlines()):
+            reload_module(r.project_name, containment_test=containment_test)
+
+
 def reload_all_modules(catch_exceptions: bool = True, verbose: bool = True) -> None:
     try:
         for mod in sys.modules.values():
             reload(mod)
     except Exception as e:
         if verbose:
             print(mod)
```

### Comparing `Warg-1.1.5/warg/manipulation.py` & `Warg-1.1.6/warg/manipulation.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/map_itertools.py` & `Warg-1.1.6/warg/map_itertools.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/math_utilities/ordinals.py` & `Warg-1.1.6/warg/math_utilities/ordinals.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/math_utilities/powers.py` & `Warg-1.1.6/warg/math_utilities/powers.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/metas/post_init.py` & `Warg-1.1.6/warg/metas/post_init.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/metas/singleton.py` & `Warg-1.1.6/warg/metas/singleton.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/mixins/dict_mixins.py` & `Warg-1.1.6/warg/mixins/dict_mixins.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/mixins/ordinal_index_mixin.py` & `Warg-1.1.6/warg/mixins/ordinal_index_mixin.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/ode.py` & `Warg-1.1.6/warg/ode.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/os_utilities/filtering.py` & `Warg-1.1.6/warg/os_utilities/filtering.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/os_utilities/os_platform.py` & `Warg-1.1.6/warg/os_utilities/os_platform.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/os_utilities/path_functions.py` & `Warg-1.1.6/warg/os_utilities/path_functions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/os_utilities/path_utilities.py` & `Warg-1.1.6/warg/os_utilities/path_utilities.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/os_utilities/platform_selection.py` & `Warg-1.1.6/warg/os_utilities/platform_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 
     :return:
     :rtype:
     """
     return SYSTEM
 
 
-# print(SYSTEM)
 if SYSTEM == "darwin":
     SYSTEM = SystemEnum.mac
 elif SYSTEM == "linux2" or SYSTEM == "linux":
     SYSTEM = SystemEnum.linux
 elif SYSTEM == "win32":
     SYSTEM = SystemEnum.windows
 else:
```

### Comparing `Warg-1.1.5/warg/plugin.py` & `Warg-1.1.6/warg/plugin.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/replication.py` & `Warg-1.1.6/warg/replication.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/strings.py` & `Warg-1.1.6/warg/strings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/styling.py` & `Warg-1.1.6/warg/styling.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/text.py` & `Warg-1.1.6/warg/text.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.5/warg/typing_extension.py` & `Warg-1.1.6/warg/typing_extension.py`

 * *Files identical despite different names*

