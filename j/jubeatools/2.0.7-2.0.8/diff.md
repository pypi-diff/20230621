# Comparing `tmp/jubeatools-2.0.7.tar.gz` & `tmp/jubeatools-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jubeatools-2.0.7.tar", max compression
+gzip compressed data, was "jubeatools-2.0.8.tar", max compression
```

## Comparing `jubeatools-2.0.7.tar` & `jubeatools-2.0.8.tar`

### file list

```diff
@@ -1,125 +1,124 @@
--rw-r--r--   0        0        0     1534 2022-11-03 20:53:30.403535 jubeatools-2.0.7/README.md
--rw-r--r--   0        0        0        0 2021-10-22 23:38:11.869169 jubeatools-2.0.7/jubeatools/__init__.py
--rw-r--r--   0        0        0        0 2021-10-22 23:38:11.869169 jubeatools-2.0.7/jubeatools/cli/__init__.py
--rw-r--r--   0        0        0     2433 2022-02-19 15:09:58.505860 jubeatools-2.0.7/jubeatools/cli/cli.py
--rw-r--r--   0        0        0     1172 2021-12-08 02:14:37.630342 jubeatools-2.0.7/jubeatools/cli/helpers.py
--rw-r--r--   0        0        0        0 2021-12-08 02:14:37.630342 jubeatools-2.0.7/jubeatools/cli/tests/__init__.py
--rw-r--r--   0        0        0    33964 2021-12-08 02:14:37.630342 jubeatools-2.0.7/jubeatools/cli/tests/data/Life Without You.eve
--rw-r--r--   0        0        0      110 2021-12-08 02:14:37.634342 jubeatools-2.0.7/jubeatools/cli/tests/data/__init__.py
--rw-r--r--   0        0        0      596 2022-02-19 15:09:58.505860 jubeatools-2.0.7/jubeatools/cli/tests/data/memon_merge/Sky Bus For Hire ADV.memon
--rw-r--r--   0        0        0      596 2022-02-19 15:09:58.505860 jubeatools-2.0.7/jubeatools/cli/tests/data/memon_merge/Sky Bus For Hire BSC.memon
--rw-r--r--   0        0        0      598 2022-02-19 15:09:58.505860 jubeatools-2.0.7/jubeatools/cli/tests/data/memon_merge/Sky Bus For Hire EXT.memon
--rw-r--r--   0        0        0     2699 2022-08-30 17:08:59.497169 jubeatools-2.0.7/jubeatools/cli/tests/test_cli.py
--rw-r--r--   0        0        0      153 2022-02-19 15:09:58.505860 jubeatools-2.0.7/jubeatools/formats/__init__.py
--rw-r--r--   0        0        0     5001 2022-12-24 13:00:59.671557 jubeatools-2.0.7/jubeatools/formats/dump_tools.py
--rw-r--r--   0        0        0      485 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/filetypes.py
--rw-r--r--   0        0        0      363 2022-02-19 15:09:58.505860 jubeatools-2.0.7/jubeatools/formats/format_names.py
--rw-r--r--   0        0        0     4273 2022-09-21 11:12:20.519794 jubeatools-2.0.7/jubeatools/formats/guess.py
--rw-r--r--   0        0        0      972 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/__init__.py
--rw-r--r--   0        0        0     5905 2021-12-08 02:21:07.806909 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/command.py
--rw-r--r--   0        0        0     8906 2022-02-19 15:09:58.509860 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/dump_tools.py
--rw-r--r--   0        0        0    16801 2023-02-01 21:51:24.442126 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/load_tools.py
--rw-r--r--   0        0        0      715 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo/__init__.py
--rw-r--r--   0        0        0     9835 2022-08-30 17:08:59.501169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo/dump.py
--rw-r--r--   0        0        0    13208 2023-01-26 22:20:16.459866 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo/load.py
--rw-r--r--   0        0        0      468 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo1/__init__.py
--rw-r--r--   0        0        0     8925 2022-08-30 17:08:59.501169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo1/dump.py
--rw-r--r--   0        0        0    12591 2022-02-19 15:09:58.509860 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo1/load.py
--rw-r--r--   0        0        0      268 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo2/__init__.py
--rw-r--r--   0        0        0    11955 2022-08-30 17:08:59.501169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo2/dump.py
--rw-r--r--   0        0        0    17376 2022-09-06 10:13:11.438915 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo2/load.py
--rw-r--r--   0        0        0      975 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/mono_column/__init__.py
--rw-r--r--   0        0        0     5239 2022-08-30 17:08:59.501169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/mono_column/dump.py
--rw-r--r--   0        0        0    10008 2023-01-26 22:22:02.105288 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/mono_column/load.py
--rw-r--r--   0        0        0     1716 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/symbol_definition.py
--rw-r--r--   0        0        0     1692 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/symbols.py
--rw-r--r--   0        0        0        0 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/__init__.py
--rw-r--r--   0        0        0    10918 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/data/Booths_of_Fighters_memo.txt
--rw-r--r--   0        0        0     5116 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/data/MTC_Mimi_EXT.txt
--rw-r--r--   0        0        0     5700 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/data/MTC_Nageki_no_Ki_EXT.txt
--rw-r--r--   0        0        0    11175 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/data/RorataJin's example.txt
--rw-r--r--   0        0        0      110 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/data/__init__.py
--rw-r--r--   0        0        0     6678 2022-09-15 22:09:23.832751 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/data/beat(1).txt
--rw-r--r--   0        0        0     8865 2023-02-01 21:47:24.302656 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/data/女の子は強い_#4.txt
--rw-r--r--   0        0        0        0 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo/__init__.py
--rw-r--r--   0        0        0     2523 2021-10-22 23:38:11.873169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo/example1.py
--rw-r--r--   0        0        0      667 2021-12-26 01:38:55.266501 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo/example2.py
--rw-r--r--   0        0        0      792 2021-12-26 01:38:55.266501 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo/example3.py
--rw-r--r--   0        0        0     1860 2022-02-19 15:09:58.509860 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo/test_memo.py
--rw-r--r--   0        0        0        0 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo1/__init__.py
--rw-r--r--   0        0        0     1058 2021-12-26 01:38:55.266501 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo1/example1.py
--rw-r--r--   0        0        0     1701 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo1/test_memo1.py
--rw-r--r--   0        0        0        0 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo2/__init__.py
--rw-r--r--   0        0        0      791 2021-12-26 01:38:55.266501 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo2/example1.py
--rw-r--r--   0        0        0      791 2021-12-26 01:38:55.266501 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo2/example2.py
--rw-r--r--   0        0        0      791 2021-12-26 01:38:55.266501 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo2/example3.py
--rw-r--r--   0        0        0     1841 2023-01-29 01:28:26.459932 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo2/test_memo2.py
--rw-r--r--   0        0        0        0 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/mono_column/__init__.py
--rw-r--r--   0        0        0     7851 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/mono_column/test_mono_column.py
--rw-r--r--   0        0        0     3132 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/mono_column/test_mono_column_hypothesis.py
--rw-r--r--   0        0        0      337 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/test_command.py
--rw-r--r--   0        0        0     1905 2023-02-01 22:02:49.411440 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/test_examples.py
--rw-r--r--   0        0        0     1784 2021-12-26 01:38:21.994072 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/test_utils.py
--rw-r--r--   0        0        0      402 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/typing.py
--rw-r--r--   0        0        0       75 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/konami/__init__.py
--rw-r--r--   0        0        0     6400 2023-01-24 22:06:18.811804 jubeatools-2.0.7/jubeatools/formats/konami/commons.py
--rw-r--r--   0        0        0     4490 2022-08-30 17:08:59.505169 jubeatools-2.0.7/jubeatools/formats/konami/dump_tools.py
--rw-r--r--   0        0        0      631 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/konami/eve/__init__.py
--rw-r--r--   0        0        0      773 2022-02-19 15:09:58.509860 jubeatools-2.0.7/jubeatools/formats/konami/eve/dump.py
--rw-r--r--   0        0        0     2437 2023-01-26 21:53:25.697626 jubeatools-2.0.7/jubeatools/formats/konami/eve/load.py
--rw-r--r--   0        0        0        0 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/konami/eve/tests/__init__.py
--rw-r--r--   0        0        0    64680 2023-01-24 22:14:34.458708 jubeatools-2.0.7/jubeatools/formats/konami/eve/tests/data/351450202_ext.eve
--rw-r--r--   0        0        0      110 2023-01-24 22:14:15.970457 jubeatools-2.0.7/jubeatools/formats/konami/eve/tests/data/__init__.py
--rw-r--r--   0        0        0      511 2022-08-30 17:08:59.505169 jubeatools-2.0.7/jubeatools/formats/konami/eve/tests/test_bpm_value.py
--rw-r--r--   0        0        0     1101 2023-01-24 22:52:28.899818 jubeatools-2.0.7/jubeatools/formats/konami/eve/tests/test_eve.py
--rw-r--r--   0        0        0      780 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/konami/eve/tests/test_events.py
--rw-r--r--   0        0        0      979 2023-01-24 22:53:30.676607 jubeatools-2.0.7/jubeatools/formats/konami/eve/tests/test_examples.py
--rw-r--r--   0        0        0     1953 2023-01-26 22:20:16.251863 jubeatools-2.0.7/jubeatools/formats/konami/eve/tests/test_timemap.py
--rw-r--r--   0        0        0      280 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/konami/jbsq/__init__.py
--rw-r--r--   0        0        0     1150 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/konami/jbsq/construct.py
--rw-r--r--   0        0        0     4221 2023-01-29 01:36:19.665744 jubeatools-2.0.7/jubeatools/formats/konami/jbsq/dump.py
--rw-r--r--   0        0        0     1920 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/konami/jbsq/jbsq.ksy
--rw-r--r--   0        0        0     1429 2022-08-30 17:08:59.505169 jubeatools-2.0.7/jubeatools/formats/konami/jbsq/load.py
--rw-r--r--   0        0        0        0 2022-09-21 10:02:03.206563 jubeatools-2.0.7/jubeatools/formats/konami/jbsq/tests/__init__.py
--rw-r--r--   0        0        0      575 2022-09-21 10:00:52.945606 jubeatools-2.0.7/jubeatools/formats/konami/jbsq/tests/example1.py
--rw-r--r--   0        0        0     1191 2022-09-21 10:01:13.489886 jubeatools-2.0.7/jubeatools/formats/konami/jbsq/tests/test_jbsq.py
--rw-r--r--   0        0        0     4581 2023-01-24 22:52:29.015819 jubeatools-2.0.7/jubeatools/formats/konami/load_tools.py
--rw-r--r--   0        0        0     1829 2022-08-30 17:08:59.509169 jubeatools-2.0.7/jubeatools/formats/konami/testutils.py
--rw-r--r--   0        0        0     1709 2021-12-22 00:58:14.552105 jubeatools-2.0.7/jubeatools/formats/load_tools.py
--rw-r--r--   0        0        0     1424 2022-09-19 23:45:19.349719 jubeatools-2.0.7/jubeatools/formats/loaders_and_dumpers.py
--rw-r--r--   0        0        0      440 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/malody/__init__.py
--rw-r--r--   0        0        0     3484 2022-02-19 15:09:58.509860 jubeatools-2.0.7/jubeatools/formats/malody/dump.py
--rw-r--r--   0        0        0     3831 2022-12-24 13:02:58.521940 jubeatools-2.0.7/jubeatools/formats/malody/load.py
--rw-r--r--   0        0        0     2458 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/malody/schema.py
--rw-r--r--   0        0        0        0 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/malody/tests/__init__.py
--rw-r--r--   0        0        0    52913 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/malody/tests/data/1533908574.mc
--rw-r--r--   0        0        0      110 2021-10-22 23:38:11.877169 jubeatools-2.0.7/jubeatools/formats/malody/tests/data/__init__.py
--rw-r--r--   0        0        0      266 2022-11-03 22:27:01.548435 jubeatools-2.0.7/jubeatools/formats/malody/tests/test_examples.py
--rw-r--r--   0        0        0     2618 2022-08-30 17:08:59.509169 jubeatools-2.0.7/jubeatools/formats/malody/tests/test_malody.py
--rw-r--r--   0        0        0      528 2022-02-19 15:09:58.509860 jubeatools-2.0.7/jubeatools/formats/memon/__init__.py
--rw-r--r--   0        0        0     1683 2022-02-19 15:09:58.513860 jubeatools-2.0.7/jubeatools/formats/memon/tools.py
--rw-r--r--   0        0        0        0 2022-02-19 15:09:58.513860 jubeatools-2.0.7/jubeatools/formats/memon/v0/__init__.py
--rw-r--r--   0        0        0     8590 2022-02-19 15:09:58.513860 jubeatools-2.0.7/jubeatools/formats/memon/v0/dump.py
--rw-r--r--   0        0        0     5587 2022-02-19 15:09:58.513860 jubeatools-2.0.7/jubeatools/formats/memon/v0/load.py
--rw-r--r--   0        0        0     3916 2023-01-26 22:16:18.940733 jubeatools-2.0.7/jubeatools/formats/memon/v0/schema.py
--rw-r--r--   0        0        0     2666 2022-09-06 10:13:11.438915 jubeatools-2.0.7/jubeatools/formats/memon/v0/test_v0.py
--rw-r--r--   0        0        0        0 2022-02-19 15:09:58.513860 jubeatools-2.0.7/jubeatools/formats/memon/v1/__init__.py
--rw-r--r--   0        0        0     5300 2022-12-24 13:02:11.300954 jubeatools-2.0.7/jubeatools/formats/memon/v1/dump.py
--rw-r--r--   0        0        0     4361 2022-12-24 13:02:00.560728 jubeatools-2.0.7/jubeatools/formats/memon/v1/load.py
--rw-r--r--   0        0        0     5331 2022-02-19 15:09:58.513860 jubeatools-2.0.7/jubeatools/formats/memon/v1/schema.py
--rw-r--r--   0        0        0        0 2022-02-19 15:09:58.513860 jubeatools-2.0.7/jubeatools/formats/memon/v1/tests/__init__.py
--rw-r--r--   0        0        0     1675 2022-02-19 15:09:58.513860 jubeatools-2.0.7/jubeatools/formats/memon/v1/tests/test_v1.py
--rw-r--r--   0        0        0        0 2021-10-22 23:38:11.881169 jubeatools-2.0.7/jubeatools/formats/tests/__init__.py
--rw-r--r--   0        0        0      488 2021-12-22 00:58:14.552105 jubeatools-2.0.7/jubeatools/formats/tests/test_decimal_to_beats.py
--rw-r--r--   0        0        0     7713 2023-01-26 22:20:16.355865 jubeatools-2.0.7/jubeatools/formats/timemap.py
--rw-r--r--   0        0        0     1266 2022-02-19 15:09:58.513860 jubeatools-2.0.7/jubeatools/formats/typing.py
--rw-r--r--   0        0        0      104 2023-02-01 22:32:23.472988 jubeatools-2.0.7/jubeatools/info.py
--rw-r--r--   0        0        0    11188 2022-09-20 22:34:14.036720 jubeatools-2.0.7/jubeatools/song.py
--rw-r--r--   0        0        0       28 2021-10-22 23:38:11.881169 jubeatools-2.0.7/jubeatools/testutils/__init__.py
--rw-r--r--   0        0        0      379 2023-01-24 22:51:16.494894 jubeatools-2.0.7/jubeatools/testutils/resources.py
--rw-r--r--   0        0        0     8771 2022-12-24 13:03:11.934217 jubeatools-2.0.7/jubeatools/testutils/strategies.py
--rw-r--r--   0        0        0     1878 2022-08-30 17:08:59.509169 jubeatools-2.0.7/jubeatools/testutils/test_patterns.py
--rw-r--r--   0        0        0     2283 2023-01-26 22:20:16.267864 jubeatools-2.0.7/jubeatools/utils.py
--rw-r--r--   0        0        0     1182 2023-02-01 22:32:23.416987 jubeatools-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     3908 2023-02-01 22:45:21.841376 jubeatools-2.0.7/setup.py
--rw-r--r--   0        0        0     2665 2023-02-01 22:45:21.841781 jubeatools-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1534 2022-11-03 20:53:30.000000 jubeatools-2.0.8/README.md
+-rw-r--r--   0        0        0        0 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/cli/__init__.py
+-rw-r--r--   0        0        0     2433 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/cli/cli.py
+-rw-r--r--   0        0        0     1172 2021-12-08 02:14:37.000000 jubeatools-2.0.8/jubeatools/cli/helpers.py
+-rw-r--r--   0        0        0        0 2021-12-08 02:14:37.000000 jubeatools-2.0.8/jubeatools/cli/tests/__init__.py
+-rw-r--r--   0        0        0    33964 2021-12-08 02:14:37.000000 jubeatools-2.0.8/jubeatools/cli/tests/data/Life Without You.eve
+-rw-r--r--   0        0        0      110 2021-12-08 02:14:37.000000 jubeatools-2.0.8/jubeatools/cli/tests/data/__init__.py
+-rw-r--r--   0        0        0      596 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/cli/tests/data/memon_merge/Sky Bus For Hire ADV.memon
+-rw-r--r--   0        0        0      596 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/cli/tests/data/memon_merge/Sky Bus For Hire BSC.memon
+-rw-r--r--   0        0        0      598 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/cli/tests/data/memon_merge/Sky Bus For Hire EXT.memon
+-rw-r--r--   0        0        0     2699 2022-08-30 17:08:59.000000 jubeatools-2.0.8/jubeatools/cli/tests/test_cli.py
+-rw-r--r--   0        0        0      153 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/__init__.py
+-rw-r--r--   0        0        0     5001 2022-12-24 13:00:59.000000 jubeatools-2.0.8/jubeatools/formats/dump_tools.py
+-rw-r--r--   0        0        0      485 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/filetypes.py
+-rw-r--r--   0        0        0      363 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/format_names.py
+-rw-r--r--   0        0        0     4273 2022-09-21 11:12:20.000000 jubeatools-2.0.8/jubeatools/formats/guess.py
+-rw-r--r--   0        0        0      972 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/__init__.py
+-rw-r--r--   0        0        0     5905 2021-12-08 02:21:07.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/command.py
+-rw-r--r--   0        0        0     8906 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/dump_tools.py
+-rw-r--r--   0        0        0    16801 2023-02-01 21:51:24.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/load_tools.py
+-rw-r--r--   0        0        0      715 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo/__init__.py
+-rw-r--r--   0        0        0     9835 2022-08-30 17:08:59.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo/dump.py
+-rw-r--r--   0        0        0    13208 2023-01-26 22:20:16.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo/load.py
+-rw-r--r--   0        0        0      468 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo1/__init__.py
+-rw-r--r--   0        0        0     8925 2022-08-30 17:08:59.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo1/dump.py
+-rw-r--r--   0        0        0    12591 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo1/load.py
+-rw-r--r--   0        0        0      268 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo2/__init__.py
+-rw-r--r--   0        0        0    11955 2022-08-30 17:08:59.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo2/dump.py
+-rw-r--r--   0        0        0    17376 2022-09-06 10:13:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo2/load.py
+-rw-r--r--   0        0        0      975 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/mono_column/__init__.py
+-rw-r--r--   0        0        0     5239 2022-08-30 17:08:59.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/mono_column/dump.py
+-rw-r--r--   0        0        0    10008 2023-01-26 22:22:02.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/mono_column/load.py
+-rw-r--r--   0        0        0     1716 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/symbol_definition.py
+-rw-r--r--   0        0        0     1692 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/symbols.py
+-rw-r--r--   0        0        0        0 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/__init__.py
+-rw-r--r--   0        0        0    10918 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/data/Booths_of_Fighters_memo.txt
+-rw-r--r--   0        0        0     5116 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/data/MTC_Mimi_EXT.txt
+-rw-r--r--   0        0        0     5700 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/data/MTC_Nageki_no_Ki_EXT.txt
+-rw-r--r--   0        0        0    11175 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/data/RorataJin's example.txt
+-rw-r--r--   0        0        0      110 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/data/__init__.py
+-rw-r--r--   0        0        0     6678 2022-09-15 22:09:23.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/data/beat(1).txt
+-rw-r--r--   0        0        0     8865 2023-02-01 21:47:24.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/data/女の子は強い_#4.txt
+-rw-r--r--   0        0        0        0 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo/__init__.py
+-rw-r--r--   0        0        0     2523 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo/example1.py
+-rw-r--r--   0        0        0      667 2021-12-26 01:38:55.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo/example2.py
+-rw-r--r--   0        0        0      792 2021-12-26 01:38:55.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo/example3.py
+-rw-r--r--   0        0        0     1860 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo/test_memo.py
+-rw-r--r--   0        0        0        0 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo1/__init__.py
+-rw-r--r--   0        0        0     1058 2021-12-26 01:38:55.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo1/example1.py
+-rw-r--r--   0        0        0     1701 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo1/test_memo1.py
+-rw-r--r--   0        0        0        0 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo2/__init__.py
+-rw-r--r--   0        0        0      791 2021-12-26 01:38:55.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo2/example1.py
+-rw-r--r--   0        0        0      791 2021-12-26 01:38:55.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo2/example2.py
+-rw-r--r--   0        0        0      791 2021-12-26 01:38:55.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo2/example3.py
+-rw-r--r--   0        0        0     1841 2023-01-29 01:28:26.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo2/test_memo2.py
+-rw-r--r--   0        0        0        0 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/mono_column/__init__.py
+-rw-r--r--   0        0        0     7851 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/mono_column/test_mono_column.py
+-rw-r--r--   0        0        0     3132 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/mono_column/test_mono_column_hypothesis.py
+-rw-r--r--   0        0        0      337 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/test_command.py
+-rw-r--r--   0        0        0     1905 2023-02-01 22:02:49.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/test_examples.py
+-rw-r--r--   0        0        0     1784 2021-12-26 01:38:21.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/test_utils.py
+-rw-r--r--   0        0        0      402 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/typing.py
+-rw-r--r--   0        0        0       75 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/konami/__init__.py
+-rw-r--r--   0        0        0     6400 2023-01-24 22:06:18.000000 jubeatools-2.0.8/jubeatools/formats/konami/commons.py
+-rw-r--r--   0        0        0     4490 2022-08-30 17:08:59.000000 jubeatools-2.0.8/jubeatools/formats/konami/dump_tools.py
+-rw-r--r--   0        0        0      631 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/konami/eve/__init__.py
+-rw-r--r--   0        0        0      773 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/konami/eve/dump.py
+-rw-r--r--   0        0        0     2437 2023-01-26 21:53:25.000000 jubeatools-2.0.8/jubeatools/formats/konami/eve/load.py
+-rw-r--r--   0        0        0        0 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/konami/eve/tests/__init__.py
+-rw-r--r--   0        0        0    64680 2023-01-24 22:14:34.000000 jubeatools-2.0.8/jubeatools/formats/konami/eve/tests/data/351450202_ext.eve
+-rw-r--r--   0        0        0      110 2023-01-24 22:14:15.000000 jubeatools-2.0.8/jubeatools/formats/konami/eve/tests/data/__init__.py
+-rw-r--r--   0        0        0      511 2022-08-30 17:08:59.000000 jubeatools-2.0.8/jubeatools/formats/konami/eve/tests/test_bpm_value.py
+-rw-r--r--   0        0        0     1101 2023-01-24 22:52:28.000000 jubeatools-2.0.8/jubeatools/formats/konami/eve/tests/test_eve.py
+-rw-r--r--   0        0        0      780 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/konami/eve/tests/test_events.py
+-rw-r--r--   0        0        0      979 2023-01-24 22:53:30.000000 jubeatools-2.0.8/jubeatools/formats/konami/eve/tests/test_examples.py
+-rw-r--r--   0        0        0     1953 2023-01-26 22:20:16.000000 jubeatools-2.0.8/jubeatools/formats/konami/eve/tests/test_timemap.py
+-rw-r--r--   0        0        0      280 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/konami/jbsq/__init__.py
+-rw-r--r--   0        0        0     1150 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/konami/jbsq/construct.py
+-rw-r--r--   0        0        0     4221 2023-01-29 01:36:19.000000 jubeatools-2.0.8/jubeatools/formats/konami/jbsq/dump.py
+-rw-r--r--   0        0        0     1920 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/konami/jbsq/jbsq.ksy
+-rw-r--r--   0        0        0     1429 2022-08-30 17:08:59.000000 jubeatools-2.0.8/jubeatools/formats/konami/jbsq/load.py
+-rw-r--r--   0        0        0        0 2022-09-21 10:02:03.000000 jubeatools-2.0.8/jubeatools/formats/konami/jbsq/tests/__init__.py
+-rw-r--r--   0        0        0      575 2022-09-21 10:00:52.000000 jubeatools-2.0.8/jubeatools/formats/konami/jbsq/tests/example1.py
+-rw-r--r--   0        0        0     1191 2022-09-21 10:01:13.000000 jubeatools-2.0.8/jubeatools/formats/konami/jbsq/tests/test_jbsq.py
+-rw-r--r--   0        0        0     4581 2023-01-24 22:52:29.000000 jubeatools-2.0.8/jubeatools/formats/konami/load_tools.py
+-rw-r--r--   0        0        0     1829 2022-08-30 17:08:59.000000 jubeatools-2.0.8/jubeatools/formats/konami/testutils.py
+-rw-r--r--   0        0        0     1709 2021-12-22 00:58:14.000000 jubeatools-2.0.8/jubeatools/formats/load_tools.py
+-rw-r--r--   0        0        0     1424 2022-09-19 23:45:19.000000 jubeatools-2.0.8/jubeatools/formats/loaders_and_dumpers.py
+-rw-r--r--   0        0        0      440 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/malody/__init__.py
+-rw-r--r--   0        0        0     3484 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/malody/dump.py
+-rw-r--r--   0        0        0     3891 2023-06-21 12:52:35.147151 jubeatools-2.0.8/jubeatools/formats/malody/load.py
+-rw-r--r--   0        0        0     2458 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/malody/schema.py
+-rw-r--r--   0        0        0        0 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/malody/tests/__init__.py
+-rw-r--r--   0        0        0    52913 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/malody/tests/data/1533908574.mc
+-rw-r--r--   0        0        0      110 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/malody/tests/data/__init__.py
+-rw-r--r--   0        0        0      266 2022-11-03 22:27:01.000000 jubeatools-2.0.8/jubeatools/formats/malody/tests/test_examples.py
+-rw-r--r--   0        0        0     2618 2022-08-30 17:08:59.000000 jubeatools-2.0.8/jubeatools/formats/malody/tests/test_malody.py
+-rw-r--r--   0        0        0      528 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/memon/__init__.py
+-rw-r--r--   0        0        0     1683 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/memon/tools.py
+-rw-r--r--   0        0        0        0 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/memon/v0/__init__.py
+-rw-r--r--   0        0        0     8590 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/memon/v0/dump.py
+-rw-r--r--   0        0        0     5587 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/memon/v0/load.py
+-rw-r--r--   0        0        0     3916 2023-01-26 22:16:18.000000 jubeatools-2.0.8/jubeatools/formats/memon/v0/schema.py
+-rw-r--r--   0        0        0     2666 2022-09-06 10:13:11.000000 jubeatools-2.0.8/jubeatools/formats/memon/v0/test_v0.py
+-rw-r--r--   0        0        0        0 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/memon/v1/__init__.py
+-rw-r--r--   0        0        0     5300 2022-12-24 13:02:11.000000 jubeatools-2.0.8/jubeatools/formats/memon/v1/dump.py
+-rw-r--r--   0        0        0     4361 2022-12-24 13:02:00.000000 jubeatools-2.0.8/jubeatools/formats/memon/v1/load.py
+-rw-r--r--   0        0        0     5331 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/memon/v1/schema.py
+-rw-r--r--   0        0        0        0 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/memon/v1/tests/__init__.py
+-rw-r--r--   0        0        0     1675 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/memon/v1/tests/test_v1.py
+-rw-r--r--   0        0        0        0 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/formats/tests/__init__.py
+-rw-r--r--   0        0        0      488 2021-12-22 00:58:14.000000 jubeatools-2.0.8/jubeatools/formats/tests/test_decimal_to_beats.py
+-rw-r--r--   0        0        0     7713 2023-01-26 22:20:16.000000 jubeatools-2.0.8/jubeatools/formats/timemap.py
+-rw-r--r--   0        0        0     1266 2022-02-19 15:09:58.000000 jubeatools-2.0.8/jubeatools/formats/typing.py
+-rw-r--r--   0        0        0      104 2023-06-21 13:24:18.152433 jubeatools-2.0.8/jubeatools/info.py
+-rw-r--r--   0        0        0    11188 2022-09-20 22:34:14.000000 jubeatools-2.0.8/jubeatools/song.py
+-rw-r--r--   0        0        0       28 2021-10-22 23:38:11.000000 jubeatools-2.0.8/jubeatools/testutils/__init__.py
+-rw-r--r--   0        0        0      379 2023-01-24 22:51:16.000000 jubeatools-2.0.8/jubeatools/testutils/resources.py
+-rw-r--r--   0        0        0     8771 2022-12-24 13:03:11.000000 jubeatools-2.0.8/jubeatools/testutils/strategies.py
+-rw-r--r--   0        0        0     1878 2022-08-30 17:08:59.000000 jubeatools-2.0.8/jubeatools/testutils/test_patterns.py
+-rw-r--r--   0        0        0     2283 2023-01-26 22:20:16.000000 jubeatools-2.0.8/jubeatools/utils.py
+-rw-r--r--   0        0        0     1112 2023-06-21 13:24:18.108432 jubeatools-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 jubeatools-2.0.8/PKG-INFO
```

### Comparing `jubeatools-2.0.7/README.md` & `jubeatools-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/cli/cli.py` & `jubeatools-2.0.8/jubeatools/cli/cli.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/cli/helpers.py` & `jubeatools-2.0.8/jubeatools/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/cli/tests/data/Life Without You.eve` & `jubeatools-2.0.8/jubeatools/cli/tests/data/Life Without You.eve`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/cli/tests/data/memon_merge/Sky Bus For Hire ADV.memon` & `jubeatools-2.0.8/jubeatools/cli/tests/data/memon_merge/Sky Bus For Hire ADV.memon`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/cli/tests/data/memon_merge/Sky Bus For Hire BSC.memon` & `jubeatools-2.0.8/jubeatools/cli/tests/data/memon_merge/Sky Bus For Hire BSC.memon`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/cli/tests/data/memon_merge/Sky Bus For Hire EXT.memon` & `jubeatools-2.0.8/jubeatools/cli/tests/data/memon_merge/Sky Bus For Hire EXT.memon`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/cli/tests/test_cli.py` & `jubeatools-2.0.8/jubeatools/cli/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/dump_tools.py` & `jubeatools-2.0.8/jubeatools/formats/dump_tools.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/guess.py` & `jubeatools-2.0.8/jubeatools/formats/guess.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/__init__.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/__init__.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/command.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/command.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/dump_tools.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/dump_tools.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/load_tools.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/load_tools.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo/__init__.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo/__init__.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo/dump.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo/dump.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo/load.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo/load.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo1/dump.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo1/dump.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo1/load.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo1/load.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo2/dump.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo2/dump.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/memo2/load.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/memo2/load.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/mono_column/__init__.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/mono_column/__init__.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/mono_column/dump.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/mono_column/dump.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/mono_column/load.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/mono_column/load.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/symbol_definition.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/symbol_definition.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/symbols.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/symbols.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/data/Booths_of_Fighters_memo.txt` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/data/Booths_of_Fighters_memo.txt`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/data/MTC_Mimi_EXT.txt` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/data/MTC_Mimi_EXT.txt`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/data/MTC_Nageki_no_Ki_EXT.txt` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/data/MTC_Nageki_no_Ki_EXT.txt`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/data/RorataJin's example.txt` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/data/RorataJin's example.txt`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/data/beat(1).txt` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/data/beat(1).txt`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/data/女の子は強い_#4.txt` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/data/女の子は強い_#4.txt`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo/example1.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo/example1.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo/example2.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo/example2.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo/example3.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo/example3.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo/test_memo.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo/test_memo.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo1/example1.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo1/example1.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo1/test_memo1.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo1/test_memo1.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo2/example1.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo2/example1.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo2/example2.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo2/example2.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo2/example3.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo2/example3.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/memo2/test_memo2.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/memo2/test_memo2.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/mono_column/test_mono_column.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/mono_column/test_mono_column.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/mono_column/test_mono_column_hypothesis.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/mono_column/test_mono_column_hypothesis.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/test_examples.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/jubeat_analyser/tests/test_utils.py` & `jubeatools-2.0.8/jubeatools/formats/jubeat_analyser/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/commons.py` & `jubeatools-2.0.8/jubeatools/formats/konami/commons.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/dump_tools.py` & `jubeatools-2.0.8/jubeatools/formats/konami/dump_tools.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/eve/__init__.py` & `jubeatools-2.0.8/jubeatools/formats/konami/eve/__init__.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/eve/dump.py` & `jubeatools-2.0.8/jubeatools/formats/konami/eve/dump.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/eve/load.py` & `jubeatools-2.0.8/jubeatools/formats/konami/eve/load.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/eve/tests/data/351450202_ext.eve` & `jubeatools-2.0.8/jubeatools/formats/konami/eve/tests/data/351450202_ext.eve`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/eve/tests/test_eve.py` & `jubeatools-2.0.8/jubeatools/formats/konami/eve/tests/test_eve.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/eve/tests/test_events.py` & `jubeatools-2.0.8/jubeatools/formats/konami/eve/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/eve/tests/test_examples.py` & `jubeatools-2.0.8/jubeatools/formats/konami/eve/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/eve/tests/test_timemap.py` & `jubeatools-2.0.8/jubeatools/formats/konami/eve/tests/test_timemap.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/jbsq/construct.py` & `jubeatools-2.0.8/jubeatools/formats/konami/jbsq/construct.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/jbsq/dump.py` & `jubeatools-2.0.8/jubeatools/formats/konami/jbsq/dump.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/jbsq/jbsq.ksy` & `jubeatools-2.0.8/jubeatools/formats/konami/jbsq/jbsq.ksy`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/jbsq/load.py` & `jubeatools-2.0.8/jubeatools/formats/konami/jbsq/load.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/jbsq/tests/example1.py` & `jubeatools-2.0.8/jubeatools/formats/konami/jbsq/tests/example1.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/jbsq/tests/test_jbsq.py` & `jubeatools-2.0.8/jubeatools/formats/konami/jbsq/tests/test_jbsq.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/load_tools.py` & `jubeatools-2.0.8/jubeatools/formats/konami/load_tools.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/konami/testutils.py` & `jubeatools-2.0.8/jubeatools/formats/konami/testutils.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/load_tools.py` & `jubeatools-2.0.8/jubeatools/formats/load_tools.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/loaders_and_dumpers.py` & `jubeatools-2.0.8/jubeatools/formats/loaders_and_dumpers.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/malody/dump.py` & `jubeatools-2.0.8/jubeatools/formats/malody/dump.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/malody/load.py` & `jubeatools-2.0.8/jubeatools/formats/malody/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,17 @@
         ],
         offset=offset,
     )
 
 
 def load_notes(events: List[malody.Event]) -> List[Union[song.TapNote, song.LongNote]]:
     # filter out sound events
-    notes = [e for e in events if isinstance(e, (malody.TapNote, malody.LongNote))]
+    notes: List[Union[malody.TapNote, malody.LongNote]] = [
+        e for e in events if isinstance(e, (malody.TapNote, malody.LongNote))
+    ]
     return [load_note(n) for n in notes]
 
 
 @singledispatch
 def load_note(
     n: Union[malody.TapNote, malody.LongNote]
 ) -> Union[song.TapNote, song.LongNote]:
```

### Comparing `jubeatools-2.0.7/jubeatools/formats/malody/schema.py` & `jubeatools-2.0.8/jubeatools/formats/malody/schema.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/malody/tests/data/1533908574.mc` & `jubeatools-2.0.8/jubeatools/formats/malody/tests/data/1533908574.mc`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/malody/tests/test_malody.py` & `jubeatools-2.0.8/jubeatools/formats/malody/tests/test_malody.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/memon/__init__.py` & `jubeatools-2.0.8/jubeatools/formats/memon/__init__.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/memon/tools.py` & `jubeatools-2.0.8/jubeatools/formats/memon/tools.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/memon/v0/dump.py` & `jubeatools-2.0.8/jubeatools/formats/memon/v0/dump.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/memon/v0/load.py` & `jubeatools-2.0.8/jubeatools/formats/memon/v0/load.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/memon/v0/schema.py` & `jubeatools-2.0.8/jubeatools/formats/memon/v0/schema.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/memon/v0/test_v0.py` & `jubeatools-2.0.8/jubeatools/formats/memon/v0/test_v0.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/memon/v1/dump.py` & `jubeatools-2.0.8/jubeatools/formats/memon/v1/dump.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/memon/v1/load.py` & `jubeatools-2.0.8/jubeatools/formats/memon/v1/load.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/memon/v1/schema.py` & `jubeatools-2.0.8/jubeatools/formats/memon/v1/schema.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/memon/v1/tests/test_v1.py` & `jubeatools-2.0.8/jubeatools/formats/memon/v1/tests/test_v1.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/timemap.py` & `jubeatools-2.0.8/jubeatools/formats/timemap.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/formats/typing.py` & `jubeatools-2.0.8/jubeatools/formats/typing.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/song.py` & `jubeatools-2.0.8/jubeatools/song.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/testutils/strategies.py` & `jubeatools-2.0.8/jubeatools/testutils/strategies.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/testutils/test_patterns.py` & `jubeatools-2.0.8/jubeatools/testutils/test_patterns.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/jubeatools/utils.py` & `jubeatools-2.0.8/jubeatools/utils.py`

 * *Files identical despite different names*

### Comparing `jubeatools-2.0.7/pyproject.toml` & `jubeatools-2.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jubeatools"
-version = "2.0.7"
+version = "2.0.8"
 description = "A toolbox for jubeat file formats"
 authors = ["Stepland <10530295-Buggyroom@users.noreply.gitlab.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/square-game-liberation-front/jubeatools"
 documentation = "https://jubeatools.readthedocs.io/en/latest/"
 
 [tool.poetry.dependencies]
@@ -14,32 +14,31 @@
 marshmallow = "^3.6.0"
 parsimonious = "^0.10.0"
 more-itertools = "^8.4.0"
 sortedcontainers = "^2.3.0"
 python-constraint = "^1.4.0"
 construct = "^2.10"
 construct-typing = "^0.5.3"
-marshmallow-dataclass = {extras = ["enum", "union"], version = "^8.5.3"}
-typing-inspect = "= 0.7.1" # 0.8.0 breaks something in marshmallow-dataclass
+marshmallow-dataclass = {extras = ["enum", "union"], version = "^8.5.14"}
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.3"
+[tool.poetry.scripts]
+jubeatools = 'jubeatools.cli.cli:convert'
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.2"
 rope = "^0.17.0"
 black = "^22.1.0"
 hypothesis = "^6.23.4"
 mypy = "^0.991"
 isort = "^5.10.1"
 toml = "^0.10.2"
 flake8 = "^3.9.1"
 autoimport = "^1.2.2"
 types-simplejson = "^3.17.1"
 types-toml = "^0.10.1"
 
-[tool.poetry.scripts]
-jubeatools = 'jubeatools.cli.cli:convert'
-
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `jubeatools-2.0.7/PKG-INFO` & `jubeatools-2.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: jubeatools
-Version: 2.0.7
+Version: 2.0.8
 Summary: A toolbox for jubeat file formats
 Home-page: https://gitlab.com/square-game-liberation-front/jubeatools
 Author: Stepland
 Author-email: 10530295-Buggyroom@users.noreply.gitlab.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: construct (>=2.10,<3.0)
 Requires-Dist: construct-typing (>=0.5.3,<0.6.0)
 Requires-Dist: marshmallow (>=3.6.0,<4.0.0)
-Requires-Dist: marshmallow-dataclass[union,enum] (>=8.5.3,<9.0.0)
+Requires-Dist: marshmallow-dataclass[enum,union] (>=8.5.14,<9.0.0)
 Requires-Dist: more-itertools (>=8.4.0,<9.0.0)
 Requires-Dist: parsimonious (>=0.10.0,<0.11.0)
 Requires-Dist: python-constraint (>=1.4.0,<2.0.0)
 Requires-Dist: simplejson (>=3.17.0,<4.0.0)
 Requires-Dist: sortedcontainers (>=2.3.0,<3.0.0)
-Requires-Dist: typing-inspect (==0.7.1)
 Project-URL: Documentation, https://jubeatools.readthedocs.io/en/latest/
 Project-URL: Repository, https://gitlab.com/square-game-liberation-front/jubeatools
 Description-Content-Type: text/markdown
 
 # Jubeatools
 
 [![docs status badge](https://readthedocs.org/projects/jubeatools/badge/)](https://jubeatools.readthedocs.io)
```

