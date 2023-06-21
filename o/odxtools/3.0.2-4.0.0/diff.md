# Comparing `tmp/odxtools-3.0.2.tar.gz` & `tmp/odxtools-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odxtools-3.0.2.tar", last modified: Fri Jan 27 13:39:17 2023, max compression
+gzip compressed data, was "odxtools-4.0.0.tar", last modified: Wed Jun 21 06:52:47 2023, max compression
```

## Comparing `odxtools-3.0.2.tar` & `odxtools-4.0.0.tar`

### file list

```diff
@@ -1,108 +1,127 @@
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-01-27 13:39:17.101223 odxtools-3.0.2/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1069 2022-03-09 15:55:44.000000 odxtools-3.0.2/LICENSE
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-01-27 13:39:17.101223 odxtools-3.0.2/PKG-INFO
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    22767 2022-12-12 08:24:18.000000 odxtools-3.0.2/README.md
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-01-27 13:39:17.081222 odxtools-3.0.2/examples/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       65 2023-01-27 13:39:15.000000 odxtools-3.0.2/examples/__init__.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1658 2023-01-27 13:39:15.000000 odxtools-3.0.2/examples/isotp_send.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)      811 2023-01-27 13:39:15.000000 odxtools-3.0.2/examples/mksomersaultpdx.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1612 2023-01-27 13:39:15.000000 odxtools-3.0.2/examples/pdxcopy.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    76454 2023-01-27 13:39:15.000000 odxtools-3.0.2/examples/somersaultecu.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    19444 2023-01-27 13:39:15.000000 odxtools-3.0.2/examples/somersaultlazy.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-01-27 13:39:17.089222 odxtools-3.0.2/odxtools/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2925 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      153 2023-01-13 13:17:58.000000 odxtools-3.0.2/odxtools/__main__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6656 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/admindata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3962 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/audience.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-01-27 13:39:17.093222 odxtools-3.0.2/odxtools/cli/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      140 2023-01-13 13:17:58.000000 odxtools-3.0.2/odxtools/cli/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/cli/_parser_utils.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3297 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/cli/_print_utils.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14094 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/cli/browse.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1171 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/cli/dummy_sub_parser.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5974 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/cli/find.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6654 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/cli/list.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1809 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/cli/main.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7471 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/cli/snoop.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5166 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/communicationparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7151 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/companydata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    10195 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/comparam_subset.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-01-27 13:39:17.097222 odxtools-3.0.2/odxtools/compumethods/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      840 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/compumethods/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      894 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/compumethods/compumethodbase.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      210 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/compumethods/compurationalcoeffs.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1489 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/compumethods/compuscale.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7485 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/compumethods/createanycompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      843 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/compumethods/identicalcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2531 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/compumethods/limit.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8228 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/compumethods/linearcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1692 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/compumethods/scalelinearcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6252 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/compumethods/tabintpcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2502 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/compumethods/texttablecompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5848 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/database.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    15166 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/dataobjectproperty.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      699 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/decodestate.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    27285 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/diagcodedtypes.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6882 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/diagdatadictionaryspec.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    40908 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/diaglayer.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      570 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/diaglayertype.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6952 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/ecu_variant_matcher.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3427 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/ecu_variant_patterns.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1190 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/encodestate.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7010 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/endofpdufield.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2645 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/envdata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4530 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/envdatadesc.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/exceptions.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1102 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/functionalclass.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      173 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/globals.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12104 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/isotp_state_machine.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      452 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/load_file.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      310 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/load_odx_d_file.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      334 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/load_pdx_file.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      963 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/message.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11648 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/multiplexer.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4114 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/nameditemlist.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1209 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/obd.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8438 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/odxlink.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3469 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/odxtypes.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3467 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameter_info.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-01-27 13:39:17.101223 odxtools-3.0.2/odxtools/parameters/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      832 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4330 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/codedconstparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9282 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/createanyparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1566 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/dynamicparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1387 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/lengthkeyparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2970 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/matchingrequestparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4851 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/nrcconstparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7051 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/parameterbase.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3906 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/parameterwithdop.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3263 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/physicalconstantparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2787 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/reservedparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1805 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/systemparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1090 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/tableentryparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2023 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/tablekeyparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1230 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/tablestructparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3130 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/parameters/valueparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2372 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/physicaltype.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    13080 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/service.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    15046 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/singleecujob.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4406 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/specialdata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1087 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/state.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1478 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/state_transition.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    24114 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/structures.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7522 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/table.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4409 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/uds.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    10674 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/units.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1885 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/utils.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       87 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/version.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6009 2023-01-27 13:39:15.000000 odxtools-3.0.2/odxtools/write_pdx_file.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-01-27 13:39:17.093222 odxtools-3.0.2/odxtools.egg-info/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-01-27 13:39:16.000000 odxtools-3.0.2/odxtools.egg-info/PKG-INFO
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2856 2023-01-27 13:39:16.000000 odxtools-3.0.2/odxtools.egg-info/SOURCES.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)        1 2023-01-27 13:39:16.000000 odxtools-3.0.2/odxtools.egg-info/dependency_links.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       53 2023-01-27 13:39:16.000000 odxtools-3.0.2/odxtools.egg-info/entry_points.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      100 2023-01-27 13:39:16.000000 odxtools-3.0.2/odxtools.egg-info/requires.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       18 2023-01-27 13:39:16.000000 odxtools-3.0.2/odxtools.egg-info/top_level.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      382 2023-01-27 13:39:15.000000 odxtools-3.0.2/pyproject.toml
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       38 2023-01-27 13:39:17.101223 odxtools-3.0.2/setup.cfg
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     2005 2023-01-27 13:39:15.000000 odxtools-3.0.2/setup.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-21 06:52:47.406999 odxtools-4.0.0/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1069 2022-03-09 15:55:44.000000 odxtools-4.0.0/LICENSE
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-06-21 06:52:47.406999 odxtools-4.0.0/PKG-INFO
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    22767 2022-12-12 08:24:18.000000 odxtools-4.0.0/README.md
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-21 06:52:47.386999 odxtools-4.0.0/examples/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       65 2023-01-27 13:39:15.000000 odxtools-4.0.0/examples/__init__.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1686 2023-06-21 06:52:15.000000 odxtools-4.0.0/examples/isotp_send.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)      811 2023-01-27 13:39:15.000000 odxtools-4.0.0/examples/mksomersaultpdx.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1612 2023-01-27 13:39:15.000000 odxtools-4.0.0/examples/pdxcopy.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    77899 2023-06-21 06:52:15.000000 odxtools-4.0.0/examples/somersaultecu.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    19444 2023-01-27 13:39:15.000000 odxtools-4.0.0/examples/somersaultlazy.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-21 06:52:47.394999 odxtools-4.0.0/odxtools/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2925 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      153 2023-01-13 13:17:58.000000 odxtools-4.0.0/odxtools/__main__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7853 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/admindata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4267 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/audience.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-21 06:52:47.398999 odxtools-4.0.0/odxtools/cli/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      140 2023-01-13 13:17:58.000000 odxtools-4.0.0/odxtools/cli/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/cli/_parser_utils.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3287 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/cli/_print_utils.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14094 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/cli/browse.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1171 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/cli/dummy_sub_parser.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5974 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/cli/find.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6728 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/cli/list.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1809 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/cli/main.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7471 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/cli/snoop.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5302 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/communicationparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8722 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/companydata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11567 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/comparam_subset.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-21 06:52:47.402999 odxtools-4.0.0/odxtools/compumethods/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      840 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/compumethods/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      894 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/compumethods/compumethodbase.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      210 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/compumethods/compurationalcoeffs.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1489 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/compumethods/compuscale.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7485 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/compumethods/createanycompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      843 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/compumethods/identicalcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2531 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/compumethods/limit.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8228 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/compumethods/linearcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1692 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/compumethods/scalelinearcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6252 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/compumethods/tabintpcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2502 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/compumethods/texttablecompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5667 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/database.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    15371 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/dataobjectproperty.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      699 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/decodestate.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    27425 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/diagcodedtypes.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6643 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/diagdatadictionaryspec.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    38635 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/diaglayer.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5957 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/diaglayercontainer.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11411 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/diaglayerraw.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      908 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/diaglayertype.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6946 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/ecu_variant_matcher.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3427 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/ecu_variant_patterns.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1190 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/encodestate.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7285 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/endofpdufield.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2429 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/envdata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5382 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/envdatadesc.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/exceptions.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1249 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/functionalclass.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      173 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/globals.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12104 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/isotp_state_machine.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      452 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/load_file.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      310 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/load_odx_d_file.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      334 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/load_pdx_file.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      963 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/message.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12896 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/multiplexer.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4185 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/nameditemlist.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1209 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/obd.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8438 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/odxlink.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3469 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/odxtypes.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3467 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameter_info.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-21 06:52:47.406999 odxtools-4.0.0/odxtools/parameters/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      832 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameters/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4330 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameters/codedconstparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9282 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameters/createanyparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1566 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameters/dynamicparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1387 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameters/lengthkeyparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2970 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameters/matchingrequestparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4851 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameters/nrcconstparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7208 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/parameters/parameterbase.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4022 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/parameters/parameterwithdop.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3263 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameters/physicalconstantparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2787 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameters/reservedparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1805 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameters/systemparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1090 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameters/tableentryparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2565 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/parameters/tablekeyparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1230 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameters/tablestructparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3130 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/parameters/valueparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3304 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/parentref.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2372 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/physicaltype.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    13653 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/service.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    16374 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/singleecujob.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5290 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/specialdata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1234 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/state.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3495 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/statechart.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2553 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/statetransition.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    24316 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/structures.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8058 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/table.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4409 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/uds.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11672 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/units.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1885 2023-01-27 13:39:15.000000 odxtools-4.0.0/odxtools/utils.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       87 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/version.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5907 2023-06-21 06:52:15.000000 odxtools-4.0.0/odxtools/write_pdx_file.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-21 06:52:47.398999 odxtools-4.0.0/odxtools.egg-info/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-06-21 06:52:47.000000 odxtools-4.0.0/odxtools.egg-info/PKG-INFO
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3342 2023-06-21 06:52:47.000000 odxtools-4.0.0/odxtools.egg-info/SOURCES.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)        1 2023-06-21 06:52:47.000000 odxtools-4.0.0/odxtools.egg-info/dependency_links.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       53 2023-06-21 06:52:47.000000 odxtools-4.0.0/odxtools.egg-info/entry_points.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      100 2023-06-21 06:52:47.000000 odxtools-4.0.0/odxtools.egg-info/requires.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       18 2023-06-21 06:52:47.000000 odxtools-4.0.0/odxtools.egg-info/top_level.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      382 2023-01-27 13:39:15.000000 odxtools-4.0.0/pyproject.toml
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       38 2023-06-21 06:52:47.406999 odxtools-4.0.0/setup.cfg
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     2005 2023-01-27 13:39:15.000000 odxtools-4.0.0/setup.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-06-21 06:52:47.406999 odxtools-4.0.0/tests/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    10427 2023-01-27 13:39:15.000000 odxtools-4.0.0/tests/test_compu_methods.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    51723 2023-06-21 06:52:15.000000 odxtools-4.0.0/tests/test_decoding.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    36363 2023-06-21 06:52:15.000000 odxtools-4.0.0/tests/test_diag_coded_types.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9192 2023-06-21 06:52:15.000000 odxtools-4.0.0/tests/test_diag_data_dictionary_spec.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14065 2023-06-21 06:52:15.000000 odxtools-4.0.0/tests/test_ecu_variant_matching.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2499 2023-01-13 13:17:58.000000 odxtools-4.0.0/tests/test_ecu_variant_patterns.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    10314 2023-06-21 06:52:15.000000 odxtools-4.0.0/tests/test_encoding.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3827 2023-01-27 13:39:15.000000 odxtools-4.0.0/tests/test_odxtools.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1962 2023-01-27 13:39:15.000000 odxtools-4.0.0/tests/test_odxtypes.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1639 2023-01-27 13:39:15.000000 odxtools-4.0.0/tests/test_readparameters.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    17020 2023-06-21 06:52:15.000000 odxtools-4.0.0/tests/test_singleecujob.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    10873 2023-06-21 06:52:15.000000 odxtools-4.0.0/tests/test_somersault.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8220 2023-06-21 06:52:15.000000 odxtools-4.0.0/tests/test_unit_spec.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      745 2023-01-13 13:17:58.000000 odxtools-4.0.0/tests/test_utils.py
```

### Comparing `odxtools-3.0.2/LICENSE` & `odxtools-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/PKG-INFO` & `odxtools-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odxtools
-Version: 3.0.2
+Version: 4.0.0
 Summary: Utilities to work with the automotive diagnostics standard ODX.
 Home-page: https://github.com/Daimler/odxtools
 Author: Katrin Bauer, Andreas Lauser
 Author-email: katrin.b.bauer@mbition.io, andreas.lauser@mbition.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Daimler/odxtools/issues
 Keywords: can,can bus,odx,pdx,obd,uds,automotive,diagnostics
```

### Comparing `odxtools-3.0.2/README.md` & `odxtools-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/examples/isotp_send.py` & `odxtools-4.0.0/examples/isotp_send.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 # set the ISO-TP flow control options:
 #
 # stmin: minimum frame separation time [ms]
 # bs: maximum block size. (Must be smaller than 4096?)
 isotp_socket.set_fc_opts(stmin=5, bs=100)
 
-can_bus = can.Bus(channel=channel, bustype="socketcan")
+can_bus = can.Bus(channel=channel, interface="socketcan")  # type: ignore[abstract]
 
 # note that we specify the CAN IDs from the ECU's point of view, i.e.,
 # from the tester's (our) perspective, they are reversed.
 isotp_addr = isotp.Address(rxid=tx_id, txid=rx_id)
 
 isotp_stack = isotp.CanStack(can_bus, address=isotp_addr, error_handler=isotp_error_handler)
```

### Comparing `odxtools-3.0.2/examples/mksomersaultpdx.py` & `odxtools-4.0.0/examples/mksomersaultpdx.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/examples/pdxcopy.py` & `odxtools-4.0.0/examples/pdxcopy.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/examples/somersaultecu.py` & `odxtools-4.0.0/examples/somersaultecu.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,26 +16,30 @@
 from odxtools.companydata import CompanyData, CompanySpecificInfo, RelatedDoc, TeamMember, XDoc
 from odxtools.comparam_subset import ComparamSubset
 from odxtools.compumethods import CompuScale, IdenticalCompuMethod, Limit, TexttableCompuMethod
 from odxtools.database import Database
 from odxtools.dataobjectproperty import DataObjectProperty
 from odxtools.diagcodedtypes import StandardLengthType
 from odxtools.diagdatadictionaryspec import DiagDataDictionarySpec
-from odxtools.diaglayer import DiagLayer, DiagLayerContainer
-from odxtools.diaglayertype import DIAG_LAYER_TYPE
+from odxtools.diaglayer import DiagLayer
+from odxtools.diaglayercontainer import DiagLayerContainer
+from odxtools.diaglayerraw import DiagLayerRaw
+from odxtools.diaglayertype import DiagLayerType
 from odxtools.envdata import EnvironmentData
 from odxtools.envdatadesc import EnvironmentDataDescription
 from odxtools.functionalclass import FunctionalClass
+from odxtools.globals import logger
 from odxtools.multiplexer import (Multiplexer, MultiplexerCase, MultiplexerDefaultCase,
                                   MultiplexerSwitchKey)
 from odxtools.nameditemlist import NamedItemList
 from odxtools.odxlink import OdxDocFragment, OdxLinkId, OdxLinkRef
 from odxtools.odxtypes import DataType
 from odxtools.parameters import (CodedConstParameter, MatchingRequestParameter, NrcConstParameter,
                                  ValueParameter)
+from odxtools.parentref import ParentRef
 from odxtools.physicaltype import PhysicalType
 from odxtools.service import DiagService
 from odxtools.singleecujob import ProgCode, SingleEcuJob
 from odxtools.structures import Request, Response
 from odxtools.table import Table, TableRow
 from odxtools.units import PhysicalDimension, Unit, UnitGroup, UnitSpec
 from odxtools.utils import short_name_as_id
@@ -515,14 +519,17 @@
 # muxs
 somersault_muxs = {
     "flip_preference":
         Multiplexer(
             odx_id=OdxLinkId("somersault.multiplexer.flip_preference", doc_frags),
             short_name="flip_preference",
             long_name="Flip Preference",
+            description=None,
+            is_visible_raw=None,
+            sdgs=[],
             byte_position=0,
             switch_key=MultiplexerSwitchKey(
                 byte_position=0,
                 bit_position=0,
                 dop_ref=OdxLinkRef.from_id(somersault_dops["num_flips"].odx_id),
             ),
             default_case=MultiplexerDefaultCase(
@@ -553,14 +560,15 @@
 somersault_env_datas = {
     "flip_env_data":
         EnvironmentData(
             odx_id=OdxLinkId("somersault.env_data.flip_env_data", doc_frags),
             short_name="flip_env_data",
             long_name="Flip Env Data",
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             byte_size=None,
             dtc_values=[],
             parameters=[
                 ValueParameter(
                     short_name="flip_speed",
                     long_name="Flip Speed",
@@ -610,14 +618,15 @@
 somersault_requests = {
     "start_session":
         Request(
             odx_id=OdxLinkId("somersault.RQ.start_session", doc_frags),
             short_name="start_session",
             long_name="Start the diagnostic session & do some mischief",
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             parameters=[
                 CodedConstParameter(
                     short_name="sid",
                     long_name=None,
                     semantic=None,
                     description=None,
@@ -643,14 +652,15 @@
         ),
     "stop_session":
         Request(
             odx_id=OdxLinkId("somersault.RQ.stop_session", doc_frags),
             short_name="stop_session",
             long_name="Terminate the current diagnostic session",
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             parameters=[
                 CodedConstParameter(
                     short_name="sid",
                     long_name=None,
                     semantic=None,
                     description=None,
@@ -676,14 +686,15 @@
         ),
     "tester_present":
         Request(
             odx_id=OdxLinkId("somersault.RQ.tester_present", doc_frags),
             short_name="tester_present",
             long_name="Prevent the current diagnostic session from timing out",
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             parameters=[
                 CodedConstParameter(
                     short_name="sid",
                     long_name=None,
                     semantic=None,
                     description=None,
@@ -710,14 +721,15 @@
     "set_operation_params":
         Request(
             odx_id=OdxLinkId("somersault.RQ.set_operation_params", doc_frags),
             short_name="set_operation_params",
             long_name="Specify the mode of operation for the ECU; e.g. if rings "
             "of fire ought to be used for maximum effect",
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             parameters=[
                 CodedConstParameter(
                     short_name="sid",
                     long_name=None,
                     semantic=None,
                     description=None,
@@ -744,14 +756,15 @@
         ),
     "forward_flips":
         Request(
             odx_id=OdxLinkId("somersault.RQ.do_forward_flips", doc_frags),
             short_name="do_forward_flips",
             long_name="Do forward somersaults & some other mischief",
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             parameters=[
                 CodedConstParameter(
                     short_name="sid",
                     long_name=None,
                     semantic=None,
                     description=None,
@@ -791,14 +804,15 @@
         ),
     "backward_flips":
         Request(
             odx_id=OdxLinkId("somersault.RQ.do_backward_flips", doc_frags),
             short_name="do_backward_flips",
             long_name="Do a backward somersault & some other mischief",
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             parameters=[
                 CodedConstParameter(
                     short_name="sid",
                     long_name=None,
                     semantic=None,
                     description=None,
@@ -838,14 +852,15 @@
         ),
     "report_status":
         Request(
             odx_id=OdxLinkId("somersault.RQ.report_status", doc_frags),
             short_name="report_status",
             long_name="Report back the current level of dizzy- & happiness.",
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             parameters=[
                 CodedConstParameter(
                     short_name="sid",
                     long_name=None,
                     semantic=None,
                     description=None,
@@ -875,14 +890,15 @@
 somersault_positive_responses = {
     "session":
         Response(
             odx_id=OdxLinkId("somersault.PR.session_start", doc_frags),
             short_name="session",
             long_name=None,
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             response_type="POS-RESPONSE",
             parameters=NamedItemList(
                 short_name_as_id,
                 [
                     CodedConstParameter(
                         short_name="sid",
@@ -914,14 +930,15 @@
         ),
     "tester_ok":
         Response(
             odx_id=OdxLinkId("somersault.PR.tester_present", doc_frags),
             short_name="tester_present",
             long_name=None,
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             response_type="POS-RESPONSE",
             parameters=NamedItemList(
                 short_name_as_id,
                 [
                     CodedConstParameter(
                         short_name="sid",
@@ -952,14 +969,15 @@
         ),
     "forward_flips_grudgingly_done":
         Response(
             odx_id=OdxLinkId("somersault.PR.grudging_forward", doc_frags),
             short_name="grudging_forward",
             long_name=None,
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             response_type="POS-RESPONSE",
             parameters=NamedItemList(
                 short_name_as_id,
                 [
                     CodedConstParameter(
                         short_name="sid",
@@ -990,14 +1008,15 @@
         ),
     "forward_flips_happily_done":
         Response(
             odx_id=OdxLinkId("somersault.PR.happy_forward", doc_frags),
             short_name="happy_forward",
             long_name=None,
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             response_type="POS-RESPONSE",
             parameters=NamedItemList(
                 short_name_as_id,
                 [
                     CodedConstParameter(
                         short_name="sid",
@@ -1040,14 +1059,15 @@
         ),
     "backward_flips_grudgingly_done":
         Response(
             odx_id=OdxLinkId("somersault.PR.grudging_backward", doc_frags),
             short_name="grudging_backward",
             long_name=None,
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             response_type="POS-RESPONSE",
             parameters=NamedItemList(
                 short_name_as_id,
                 [
                     CodedConstParameter(
                         short_name="sid",
@@ -1080,14 +1100,15 @@
     # Note that there is no such thing as a "backwards flip done happily"!
     "status_report":
         Response(
             odx_id=OdxLinkId("somersault.PR.status_report", doc_frags),
             short_name="status_report",
             long_name=None,
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             response_type="POS-RESPONSE",
             parameters=NamedItemList(
                 short_name_as_id,
                 [
                     CodedConstParameter(
                         short_name="sid",
@@ -1131,14 +1152,15 @@
         ),
     "set_operation_params":
         Response(
             odx_id=OdxLinkId("somersault.PR.set_operation_params", doc_frags),
             short_name="set_operation_params",
             long_name=None,
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             response_type="POS-RESPONSE",
             parameters=NamedItemList(
                 short_name_as_id,
                 [
                     CodedConstParameter(
                         short_name="sid",
@@ -1162,14 +1184,15 @@
 somersault_negative_responses = {
     "general":
         Response(
             odx_id=OdxLinkId("somersault.NR.general_negative_response", doc_frags),
             short_name="general_negative_response",
             long_name=None,
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             response_type="NEG-RESPONSE",
             parameters=NamedItemList(
                 short_name_as_id,
                 [
                     CodedConstParameter(
                         short_name="sid",
@@ -1214,14 +1237,15 @@
     # to extract it for the COMPARAMS.
     "tester_nok":
         Response(
             odx_id=OdxLinkId("somersault.NR.tester_nok", doc_frags),
             short_name="tester_nok",
             long_name=None,
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             response_type="NEG-RESPONSE",
             parameters=NamedItemList(
                 short_name_as_id,
                 [
                     CodedConstParameter(
                         short_name="sid",
@@ -1251,14 +1275,15 @@
         ),
     "flips_not_done":
         Response(
             odx_id=OdxLinkId("somersault.NR.flips_not_done", doc_frags),
             short_name="flips_not_done",
             long_name=None,
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             response_type="NEG-RESPONSE",
             parameters=NamedItemList(
                 short_name_as_id,
                 [
                     CodedConstParameter(
                         short_name="sid",
@@ -1539,14 +1564,15 @@
             prog_codes=[
                 ProgCode(
                     code_file="jobs.jar",
                     encryption=None,
                     syntax="JAR",
                     entrypoint="com.supervisor.jobs.CompulsoryProgram",
                     revision="1.23.4",
+                    library_refs=[],
                 ),
             ],
             input_params=[],
             output_params=[],
             neg_output_params=[],
             is_mandatory_raw=None,
             is_executable_raw=None,
@@ -1706,139 +1732,102 @@
         physical_dimensions=list(somersault_physical_dimensions.values()),
         sdgs=[],
     ),
     tables=NamedItemList(short_name_as_id, somersault_tables.values()),
     muxs=NamedItemList(short_name_as_id, somersault_muxs.values()),
     env_datas=NamedItemList(short_name_as_id, somersault_env_datas.values()),
     env_data_descs=NamedItemList(short_name_as_id, somersault_env_data_descs.values()),
-    dtc_dops=NamedItemList(short_name_as_id, []),
-    structures=NamedItemList(short_name_as_id, []),
-    end_of_pdu_fields=NamedItemList(short_name_as_id, []),
+    dtc_dops=NamedItemList(short_name_as_id),
+    structures=NamedItemList(short_name_as_id),
+    end_of_pdu_fields=NamedItemList(short_name_as_id),
     sdgs=[],
 )
 
 # diagnostics layer
-somersault_diaglayer = DiagLayer(
-    variant_type=DIAG_LAYER_TYPE.BASE_VARIANT,
+somersault_diaglayer_raw = DiagLayerRaw(
+    variant_type=DiagLayerType.BASE_VARIANT,
     odx_id=OdxLinkId("somersault", doc_frags),
     short_name="somersault",
     long_name="Somersault base variant",
     description="<p>Base variant of the somersault ECU &amp; cetera</p>",
-    requests=list(somersault_requests.values()),
-    services=list(somersault_services.values()),
-    single_ecu_jobs=list(somersault_single_ecu_jobs.values()),
-    positive_responses=list(somersault_positive_responses.values()),
-    negative_responses=list(somersault_negative_responses.values()),
+    admin_data=None,
+    company_datas=NamedItemList(short_name_as_id),
+    functional_classes=NamedItemList(short_name_as_id, somersault_functional_classes.values()),
     diag_data_dictionary_spec=somersault_diag_data_dictionary_spec,
-    communication_parameters=somersault_communication_parameters,
-    additional_audiences=list(somersault_additional_audiences.values()),
-    functional_classes=list(somersault_functional_classes.values()),
-    states=[],
-    state_transitions=[],
+    diag_comms=[*somersault_services.values(), *somersault_single_ecu_jobs.values()],
+    requests=NamedItemList(short_name_as_id, somersault_requests.values()),
+    positive_responses=NamedItemList(short_name_as_id, somersault_positive_responses.values()),
+    negative_responses=NamedItemList(short_name_as_id, somersault_negative_responses.values()),
+    global_negative_responses=NamedItemList(short_name_as_id),
     import_refs=[],
-    diag_comm_refs=[],
-    parent_refs=[],
+    state_charts=NamedItemList(short_name_as_id),
+    additional_audiences=NamedItemList(short_name_as_id, somersault_additional_audiences.values()),
     sdgs=[],
+    parent_refs=[],
+    communication_parameters=somersault_communication_parameters,
+    ecu_variant_patterns=[],
 )
+somersault_diaglayer = DiagLayer(diag_layer_raw=somersault_diaglayer_raw)
 
 ##################
 # Lazy variant of Somersault ECU: this one is lazy and cuts corners
 ##################
 
-# TODO: inheritance (without too much code duplication)
-somersault_lazy_diaglayer = DiagLayer(
-    variant_type=DIAG_LAYER_TYPE.ECU_VARIANT,
+somersault_lazy_diaglayer_raw = DiagLayerRaw(
+    variant_type=DiagLayerType.ECU_VARIANT,
     odx_id=OdxLinkId("somersault_lazy", doc_frags),
     short_name="somersault_lazy",
     long_name="Somersault lazy ECU",
     description="<p>Sloppy variant of the somersault ECU (lazy &lt; assiduous)</p>",
+    admin_data=None,
+    company_datas=NamedItemList(short_name_as_id),
+    functional_classes=NamedItemList(short_name_as_id),
+    diag_data_dictionary_spec=None,
+    diag_comms=[],
+    requests=NamedItemList(short_name_as_id),
+    positive_responses=NamedItemList(short_name_as_id),
+    negative_responses=NamedItemList(short_name_as_id),
+    global_negative_responses=NamedItemList(short_name_as_id),
+    import_refs=[],
+    state_charts=NamedItemList(short_name_as_id),
+    additional_audiences=NamedItemList(short_name_as_id),
+    sdgs=[],
     parent_refs=[
-        DiagLayer.ParentRef(  # <- TODO: this is a bit sketchy IMO
-            parent=OdxLinkRef.from_id(somersault_diaglayer.odx_id),
-            ref_type="BASE-VARIANT-REF",
+        ParentRef(
+            layer_ref=OdxLinkRef.from_id(somersault_diaglayer.odx_id),
             # this variant does not do backflips
             not_inherited_diag_comms=[
                 somersault_requests["backward_flips"].short_name,
                 somersault_requests["set_operation_params"].short_name,
             ],
             not_inherited_dops=[],
+            not_inherited_variables=[],
+            not_inherited_tables=[],
+            not_inherited_global_neg_responses=[],
         )
     ],
     communication_parameters=somersault_communication_parameters,
-    requests=[],
-    positive_responses=[],
-    negative_responses=[],
-    services=[],
-    single_ecu_jobs=[],
-    diag_comm_refs=[],
-    diag_data_dictionary_spec=None,
-    additional_audiences=[],
-    functional_classes=[],
-    states=[],
-    state_transitions=[],
-    import_refs=[],
-    sdgs=[],
+    ecu_variant_patterns=[],
 )
+somersault_lazy_diaglayer = DiagLayer(diag_layer_raw=somersault_lazy_diaglayer_raw)
 
 ##################
 # Assiduous production variant of Somersault ECU: This one works
 # harder than it needs to
 ##################
 
-# TODO: inheritance (without too much code duplication)
-somersault_assiduous_diaglayer = DiagLayer(
-    variant_type=DIAG_LAYER_TYPE.ECU_VARIANT,
-    odx_id=OdxLinkId("somersault_assiduous", doc_frags),
-    short_name="somersault_assiduous",
-    long_name="Somersault assiduous ECU",
-    description="<p>Hard-working variant of the somersault ECU (lazy &lt; assiduous)</p>",
-    diag_data_dictionary_spec=DiagDataDictionarySpec(
-        dtc_dops=NamedItemList(short_name_as_id, []),
-        data_object_props=NamedItemList(short_name_as_id, []),
-        structures=NamedItemList(short_name_as_id, []),
-        end_of_pdu_fields=NamedItemList(short_name_as_id, []),
-        tables=NamedItemList(short_name_as_id, []),
-        env_data_descs=NamedItemList(short_name_as_id, []),
-        env_datas=NamedItemList(short_name_as_id, []),
-        muxs=NamedItemList(short_name_as_id, []),
-        unit_spec=None,
-        sdgs=[],
-    ),
-    parent_refs=[
-        DiagLayer.ParentRef(  # <- TODO: this is a bit sketchy IMO
-            parent=OdxLinkRef.from_id(somersault_diaglayer.odx_id),
-            ref_type="BASE-VARIANT-REF",
-            # this variant does everything which the base variant does
-            not_inherited_diag_comms=[],
-            not_inherited_dops=[],
-        )
-    ],
-    communication_parameters=somersault_communication_parameters,
-    requests=[],
-    positive_responses=[],
-    negative_responses=[],
-    services=[],
-    single_ecu_jobs=[],
-    diag_comm_refs=[],
-    additional_audiences=[],
-    functional_classes=[],
-    states=[],
-    state_transitions=[],
-    import_refs=[],
-    sdgs=[],
-)
-
 # the assiduous ECU also does headstands...
 somersault_assiduous_requests = {
     "headstand":
         Request(
             odx_id=OdxLinkId("somersault_assiduous.RQ.do_headstand", doc_frags),
             short_name="do_headstand",
             long_name="Do a headstand & whatever else is required to entertain the customer",
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             parameters=[
                 CodedConstParameter(
                     short_name="sid",
                     long_name=None,
                     semantic=None,
                     description=None,
@@ -1869,14 +1858,15 @@
 somersault_assiduous_positive_responses = {
     "headstand_done":
         Response(
             odx_id=OdxLinkId("somersault_assiduous.PR.headstand_done", doc_frags),
             short_name="headstand_done",
             long_name=None,
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             response_type="POS-RESPONSE",
             parameters=NamedItemList(
                 short_name_as_id,
                 [
                     CodedConstParameter(
                         short_name="sid",
@@ -1911,14 +1901,15 @@
 somersault_assiduous_negative_responses = {
     "fell_over":
         Response(
             odx_id=OdxLinkId("somersault_assiduous.NR.fell_over", doc_frags),
             short_name="fell_over",
             long_name=None,
             description=None,
+            sdgs=[],
             is_visible_raw=None,
             response_type="POS-RESPONSE",
             parameters=NamedItemList(
                 short_name_as_id,
                 [
                     CodedConstParameter(
                         short_name="sid",
@@ -1981,22 +1972,61 @@
                 is_aftersales_raw=None,
                 is_aftermarket_raw=None,
             ),
             sdgs=[],
         ),
 }
 
-# fill the diagnostics layer object
-somersault_assiduous_diaglayer.requests = list(somersault_assiduous_requests.values())
-somersault_assiduous_diaglayer._local_services = NamedItemList(
-    short_name_as_id, somersault_assiduous_services.values())
-somersault_assiduous_diaglayer.positive_responses = NamedItemList(
-    short_name_as_id, somersault_assiduous_positive_responses.values())
-somersault_assiduous_diaglayer.negative_responses = NamedItemList(
-    short_name_as_id, somersault_assiduous_negative_responses.values())
+somersault_assiduous_diaglayer_raw = DiagLayerRaw(
+    variant_type=DiagLayerType.ECU_VARIANT,
+    odx_id=OdxLinkId("somersault_assiduous", doc_frags),
+    short_name="somersault_assiduous",
+    long_name="Somersault assiduous ECU",
+    description="<p>Hard-working variant of the somersault ECU (lazy &lt; assiduous)</p>",
+    admin_data=None,
+    company_datas=NamedItemList(short_name_as_id),
+    functional_classes=NamedItemList(short_name_as_id),
+    diag_data_dictionary_spec=DiagDataDictionarySpec(
+        dtc_dops=NamedItemList(short_name_as_id),
+        data_object_props=NamedItemList(short_name_as_id),
+        structures=NamedItemList(short_name_as_id),
+        end_of_pdu_fields=NamedItemList(short_name_as_id),
+        tables=NamedItemList(short_name_as_id),
+        env_data_descs=NamedItemList(short_name_as_id),
+        env_datas=NamedItemList(short_name_as_id),
+        muxs=NamedItemList(short_name_as_id),
+        unit_spec=None,
+        sdgs=[],
+    ),
+    diag_comms=list(somersault_assiduous_services.values()),
+    requests=NamedItemList(short_name_as_id, somersault_assiduous_requests.values()),
+    positive_responses=NamedItemList(short_name_as_id,
+                                     somersault_assiduous_positive_responses.values()),
+    negative_responses=NamedItemList(short_name_as_id,
+                                     somersault_assiduous_negative_responses.values()),
+    global_negative_responses=NamedItemList(short_name_as_id),
+    import_refs=[],
+    state_charts=NamedItemList(short_name_as_id),
+    additional_audiences=NamedItemList(short_name_as_id),
+    sdgs=[],
+    parent_refs=[
+        ParentRef(
+            layer_ref=OdxLinkRef.from_id(somersault_diaglayer.odx_id),
+            # this variant does everything which the base variant does
+            not_inherited_diag_comms=[],
+            not_inherited_dops=[],
+            not_inherited_variables=[],
+            not_inherited_tables=[],
+            not_inherited_global_neg_responses=[],
+        )
+    ],
+    communication_parameters=somersault_communication_parameters,
+    ecu_variant_patterns=[],
+)
+somersault_assiduous_diaglayer = DiagLayer(diag_layer_raw=somersault_assiduous_diaglayer_raw)
 
 ##################
 # Container with all ECUs
 ##################
 
 # create a "diagnosis layer container" object
 somersault_dlc = DiagLayerContainer(
@@ -2036,15 +2066,15 @@
 
 # create a database object
 database = Database()
 database._diag_layer_containers = NamedItemList(short_name_as_id, [somersault_dlc])
 database._comparam_subsets = NamedItemList(short_name_as_id, comparam_subsets)
 
 # Create ID mapping and resolve references
-database.finalize_init()
+database.refresh()
 
 # delete all variables except "database"
 for name in dir():
     if name not in (
             "database",
             "SID",
     ):
```

### Comparing `odxtools-3.0.2/examples/somersaultlazy.py` & `odxtools-4.0.0/examples/somersaultlazy.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/__init__.py` & `odxtools-4.0.0/odxtools/__init__.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/admindata.py` & `odxtools-4.0.0/odxtools/admindata.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 from xml.etree import ElementTree
 
 from .companydata import CompanyData, TeamMember
 from .nameditemlist import NamedItemList
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from .specialdata import SpecialDataGroup, create_sdgs_from_et
 from .utils import create_description_from_et
 
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
+
 
 @dataclass
 class CompanyDocInfo:
     company_data_ref: OdxLinkRef
     team_member_ref: Optional[OdxLinkRef]
     doc_label: Optional[str]
     sdgs: List[SpecialDataGroup]
@@ -47,37 +50,50 @@
         result = {}
 
         for sdg in self.sdgs:
             result.update(sdg._build_odxlinks())
 
         return result
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase):
         self._company_data = odxlinks.resolve(self.company_data_ref, CompanyData)
 
         self._team_member: Optional[TeamMember] = None
         if self.team_member_ref is not None:
             self._team_member = odxlinks.resolve(self.team_member_ref, TeamMember)
 
         for sdg in self.sdgs:
-            sdg._resolve_references(odxlinks)
+            sdg._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer"):
+        for sdg in self.sdgs:
+            sdg._resolve_snrefs(diag_layer)
 
 
 @dataclass
 class Modification:
     change: Optional[str]
     reason: Optional[str]
 
     @staticmethod
     def from_et(et_element: ElementTree.Element, doc_frags: List[OdxDocFragment]) -> "Modification":
         change = et_element.findtext("CHANGE")
         reason = et_element.findtext("REASON")
 
         return Modification(change=change, reason=reason)
 
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase):
+        pass
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer"):
+        pass
+
 
 @dataclass
 class CompanyRevisionInfo:
     company_data_ref: OdxLinkRef
     revision_label: Optional[str]
     state: Optional[str]
 
@@ -94,17 +110,23 @@
         assert company_data_ref is not None
         revision_label = et_element.findtext("REVISION_LABEL")
         state = et_element.findtext("STATE")
 
         return CompanyRevisionInfo(
             company_data_ref=company_data_ref, revision_label=revision_label, state=state)
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase):
         self._company_data = odxlinks.resolve(self.company_data_ref, CompanyData)
 
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
 
 @dataclass
 class DocRevision:
     """
     Representation of a single revision of the relevant object.
     """
 
@@ -147,21 +169,34 @@
             state=state,
             date=date,
             tool=tool,
             company_revision_infos=crilist,
             modifications=modlist,
         )
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase):
         self._team_member: Optional[TeamMember] = None
         if self.team_member_ref is not None:
             self._team_member = odxlinks.resolve(self.team_member_ref, TeamMember)
 
         for cri in self.company_revision_infos:
-            cri._resolve_references(odxlinks)
+            cri._resolve_odxlinks(odxlinks)
+
+        for mod in self.modifications:
+            mod._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        for cri in self.company_revision_infos:
+            cri._resolve_snrefs(diag_layer)
+
+        for mod in self.modifications:
+            mod._resolve_snrefs(diag_layer)
 
 
 @dataclass
 class AdminData:
     language: Optional[str]
     company_doc_infos: List[CompanyDocInfo]
     doc_revisions: List[DocRevision]
@@ -192,13 +227,20 @@
         result: Dict[OdxLinkId, Any] = {}
 
         for cdi in self.company_doc_infos:
             result.update(cdi._build_odxlinks())
 
         return result
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        for cdi in self.company_doc_infos:
+            cdi._resolve_odxlinks(odxlinks)
+
+        for dr in self.doc_revisions:
+            dr._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
         for cdi in self.company_doc_infos:
-            cdi._resolve_references(odxlinks)
+            cdi._resolve_snrefs(diag_layer)
 
         for dr in self.doc_revisions:
-            dr._resolve_references(odxlinks)
+            dr._resolve_snrefs(diag_layer)
```

### Comparing `odxtools-3.0.2/odxtools/audience.py` & `odxtools-4.0.0/odxtools/audience.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from .odxtypes import odxstr_to_bool
 from .utils import create_description_from_et
 
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
+
 
 @dataclass
 class AdditionalAudience:
     """
     Corresponds to ADDITIONAL-AUDIENCE.
     """
 
@@ -31,15 +34,18 @@
 
         return AdditionalAudience(
             odx_id=odx_id, short_name=short_name, long_name=long_name, description=description)
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
         return {self.odx_id: self}
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        pass
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
         pass
 
 
 @dataclass
 class Audience:
     enabled_audience_refs: List[OdxLinkRef]
     disabled_audience_refs: List[OdxLinkRef]
@@ -107,14 +113,20 @@
             is_supplier_raw=is_supplier_raw,
             is_development_raw=is_development_raw,
             is_manufacturing_raw=is_manufacturing_raw,
             is_aftersales_raw=is_aftersales_raw,
             is_aftermarket_raw=is_aftermarket_raw,
         )
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         self._enabled_audiences = [
             odxlinks.resolve(ref, AdditionalAudience) for ref in self.enabled_audience_refs
         ]
         self._disabled_audiences = [
             odxlinks.resolve(ref, AdditionalAudience) for ref in self.disabled_audience_refs
         ]
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
```

### Comparing `odxtools-3.0.2/odxtools/cli/_parser_utils.py` & `odxtools-4.0.0/odxtools/cli/_parser_utils.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/cli/_print_utils.py` & `odxtools-4.0.0/odxtools/cli/_print_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         pre_condition_states_short_names = [
             pre_condition_state.short_name for pre_condition_state in service.pre_condition_states
         ]
         print(f"  Pre-Condition-States: {', '.join(pre_condition_states_short_names)}")
 
     if print_state_transitions and len(service.state_transitions) > 0:
         state_transitions = [
-            f"{state_transition.source_short_name} -> {state_transition.target_short_name}"
+            f"{state_transition.source_snref} -> {state_transition.target_snref}"
             for state_transition in service.state_transitions
         ]
         print(f"  State-Transitions: {', '.join(state_transitions)}")
 
     if print_audiences and service.audience:
         enabled_audiences_short_names = [
             enabled_audience.short_name for enabled_audience in service.audience.enabled_audiences
```

### Comparing `odxtools-3.0.2/odxtools/cli/browse.py` & `odxtools-4.0.0/odxtools/cli/browse.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/cli/dummy_sub_parser.py` & `odxtools-4.0.0/odxtools/cli/dummy_sub_parser.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/cli/find.py` & `odxtools-4.0.0/odxtools/cli/find.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/cli/list.py` & `odxtools-4.0.0/odxtools/cli/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 import argparse
-from typing import List, Union, cast
+from typing import Collection, List, Union, cast
 
 from ..database import Database
+from ..dataobjectproperty import DopBase
 from ..diaglayer import DiagLayer
 from ..service import DiagService
 from ..singleecujob import SingleEcuJob
 from . import _parser_utils
 from ._print_utils import format_desc, print_diagnostic_service
 
 # name of the tool
@@ -36,15 +37,15 @@
             print(f"The variant '{dl_sn}' could not be found!")
             continue
 
         assert isinstance(dl, DiagLayer)
         all_services: List[Union[DiagService, SingleEcuJob]] = sorted(
             dl.services, key=lambda x: x.short_name)
 
-        data_object_properties = dl.data_object_properties
+        data_object_properties = dl.diag_data_dictionary_spec.data_object_props
         com_params = dl.communication_parameters
 
         print(f"{dl.variant_type} '{dl.short_name}'")
         print(
             f" num services: {len(all_services)}, num DOPs: {len(data_object_properties)}, num communication parameters: {len(com_params)}."
         )
```

### Comparing `odxtools-3.0.2/odxtools/cli/main.py` & `odxtools-4.0.0/odxtools/cli/main.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/cli/snoop.py` & `odxtools-4.0.0/odxtools/cli/snoop.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/communicationparameter.py` & `odxtools-4.0.0/odxtools/communicationparameter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 import warnings
-from typing import Any, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 from .comparam_subset import (BaseComparam, Comparam, ComplexComparam, ComplexValue,
                               create_complex_value_from_et)
-from .diaglayertype import DIAG_LAYER_TYPE
+from .diaglayertype import DiagLayerType
 from .exceptions import OdxWarning
-from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkRef
+from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from .utils import create_description_from_et
 
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
+
 
 class CommunicationParameterRef:
 
     def __init__(
         self,
         *,
         value: Union[str, ComplexValue],
@@ -25,33 +28,34 @@
     ) -> None:
         self.value = value
         self.id_ref = id_ref
         self.is_functional = is_functional
         self.description = description
         self.protocol_snref = protocol_snref
         self.prot_stack_snref = prot_stack_snref
-        self.comparam: Optional[BaseComparam] = None
+
+        self._comparam: BaseComparam
 
     @staticmethod
     def from_et(et_element, doc_frags: List[OdxDocFragment],
-                dl_type: DIAG_LAYER_TYPE) -> "CommunicationParameterRef":
+                dl_type: DiagLayerType) -> "CommunicationParameterRef":
         id_ref = OdxLinkRef.from_et(et_element, doc_frags)
         assert id_ref is not None
 
         # ODX standard v2.0.0 defined only VALUE. ODX v2.0.1 decided
         # to break things and change it to choice between SIMPLE-VALUE
         # and COMPLEX-VALUE
         if et_element.find("VALUE") is not None:
             value = et_element.findtext("VALUE")
         elif et_element.find("SIMPLE-VALUE") is not None:
             value = et_element.findtext("SIMPLE-VALUE")
         else:
             value = create_complex_value_from_et(et_element.find("COMPLEX-VALUE"))
 
-        is_functional = dl_type == DIAG_LAYER_TYPE.FUNCTIONAL_GROUP
+        is_functional = dl_type == DiagLayerType.FUNCTIONAL_GROUP
         description = create_description_from_et(et_element.find("DESC"))
 
         prot_stack_snref = None
         if (psnref_elem := et_element.find("PROT-STACK-SNREF")) is not None:
             prot_stack_snref = psnref_elem.get("SHORT-NAME")
 
         protocol_snref = None
@@ -63,28 +67,35 @@
             id_ref=id_ref,
             is_functional=is_functional,
             description=description,
             protocol_snref=protocol_snref,
             prot_stack_snref=prot_stack_snref,
         )
 
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        self._comparam = odxlinks.resolve(self.id_ref)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
     def __repr__(self) -> str:
         val = self.value
         if isinstance(val, str):
             val = f"'{val}'"
         return f"CommunicationParameter('{self.short_name}', value={val})"
 
     def __str__(self) -> str:
         return self.__repr__()
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
-        # Temporary lenient until tests are updated
-        self.comparam = odxlinks.resolve_lenient(self.id_ref)
-        if not self.comparam:
-            warnings.warn(f"Could not resolve COMPARAM '{self.id_ref}'", OdxWarning)
+    @property
+    def comparam(self) -> BaseComparam:
+        return self._comparam
 
     def get_value(self) -> Optional[str]:
         """Retrieve the value of a simple communication parameter
 
         This takes the default value of the comparam (if any) into
         account.
         """
```

### Comparing `odxtools-3.0.2/odxtools/companydata.py` & `odxtools-4.0.0/odxtools/companydata.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,67 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 from xml.etree import ElementTree
 
 from .nameditemlist import NamedItemList
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId
 from .specialdata import SpecialDataGroup, create_sdgs_from_et
 from .utils import create_description_from_et, short_name_as_id
 
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
+
 
 @dataclass
 class XDoc:
     short_name: str
     long_name: Optional[str]
     description: Optional[str]
     number: Optional[str]
     state: Optional[str]
     date: Optional[str]
     publisher: Optional[str]
     url: Optional[str]
     position: Optional[str]
 
     @staticmethod
-    def from_et(xdoc) -> "XDoc":
-        short_name = xdoc.findtext("SHORT-NAME")
-        long_name = xdoc.findtext("LONG-NAME")
-        description = create_description_from_et(xdoc.find("DESC"))
-        number = xdoc.findtext("NUMBER")
-        state = xdoc.findtext("STATE")
-        date = xdoc.findtext("DATE")
-        publisher = xdoc.findtext("PUBLISHER")
-        url = xdoc.findtext("URL")
-        position = xdoc.findtext("POSITION")
+    def from_et(et_element) -> "XDoc":
+        short_name = et_element.findtext("SHORT-NAME")
+        long_name = et_element.findtext("LONG-NAME")
+        description = create_description_from_et(et_element.find("DESC"))
+        number = et_element.findtext("NUMBER")
+        state = et_element.findtext("STATE")
+        date = et_element.findtext("DATE")
+        publisher = et_element.findtext("PUBLISHER")
+        url = et_element.findtext("URL")
+        position = et_element.findtext("POSITION")
 
         return XDoc(
             short_name=short_name,
             long_name=long_name,
             description=description,
             number=number,
             state=state,
             date=date,
             publisher=publisher,
             url=url,
             position=position,
         )
 
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        pass
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
 
 @dataclass
 class RelatedDoc:
     description: Optional[str]
     xdoc: Optional[XDoc]
 
     @staticmethod
@@ -60,14 +72,30 @@
             xdoc = XDoc.from_et(xdoc)
 
         return RelatedDoc(
             description=description,
             xdoc=xdoc,
         )
 
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        result = {}
+
+        if self.xdoc:
+            result.update(self.xdoc._build_odxlinks())
+
+        return result
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        if self.xdoc:
+            self.xdoc._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        if self.xdoc:
+            self.xdoc._resolve_snrefs(diag_layer)
+
 
 @dataclass
 class CompanySpecificInfo:
     related_docs: List[RelatedDoc]
     sdgs: List[SpecialDataGroup]
 
     @staticmethod
@@ -88,17 +116,27 @@
         result = {}
 
         for sdg in self.sdgs:
             result.update(sdg._build_odxlinks())
 
         return result
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        for rd in self.related_docs:
+            rd._resolve_odxlinks(odxlinks)
+
         for sdg in self.sdgs:
-            sdg._resolve_references(odxlinks)
+            sdg._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        for rd in self.related_docs:
+            rd._resolve_snrefs(diag_layer)
+
+        for sdg in self.sdgs:
+            sdg._resolve_snrefs(diag_layer)
 
 
 @dataclass
 class TeamMember:
     odx_id: OdxLinkId
     short_name: str
     long_name: Optional[str]
@@ -147,14 +185,25 @@
             zip=zip,
             city=city,
             phone=phone,
             fax=fax,
             email=email,
         )
 
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        result = {self.odx_id: self}
+
+        return result
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        pass
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
 
 @dataclass
 class CompanyData:
     odx_id: OdxLinkId
     short_name: str
     long_name: Optional[str]
     description: Optional[str]
@@ -175,53 +224,57 @@
             rlist = list()
 
             for role in roles.iterfind("ROLE"):
                 rlist.append(role.text)
 
             roles = rlist
 
-        team_members = et_element.find("TEAM-MEMBERS")
-        if team_members is not None:
-            tml = NamedItemList(short_name_as_id)  # type: ignore
-
-            for tm in team_members.iterfind("TEAM-MEMBER"):
-                tml.append(TeamMember.from_et(tm, doc_frags))
-
-            team_members = tml
-
+        team_members = [
+            TeamMember.from_et(tm, doc_frags)
+            for tm in et_element.iterfind("TEAM-MEMBERS/TEAM-MEMBER")
+        ]
         company_specific_info = et_element.find("COMPANY-SPECIFIC-INFO")
         if company_specific_info is not None:
             company_specific_info = CompanySpecificInfo.from_et(company_specific_info, doc_frags)
 
         return CompanyData(
             odx_id=odx_id,
             short_name=short_name,
             long_name=long_name,
             description=description,
             roles=roles,
-            team_members=team_members,
+            team_members=NamedItemList(short_name_as_id, team_members),
             company_specific_info=company_specific_info,
         )
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
         result = {self.odx_id: self}
 
         # team members
-        if self.team_members is not None:
-            for tm in self.team_members:
-                result[tm.odx_id] = tm
+        for tm in self.team_members:
+            result.update(tm._build_odxlinks())
 
         if self.company_specific_info:
             result.update(self.company_specific_info._build_odxlinks())
 
         return result
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        for tm in self.team_members:
+            tm._resolve_odxlinks(odxlinks)
+
+        if self.company_specific_info:
+            self.company_specific_info._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        for tm in self.team_members:
+            tm._resolve_snrefs(diag_layer)
+
         if self.company_specific_info:
-            self.company_specific_info._resolve_references(odxlinks)
+            self.company_specific_info._resolve_snrefs(diag_layer)
 
 
 def create_company_datas_from_et(et_element,
                                  doc_frags: List[OdxDocFragment]) -> NamedItemList[CompanyData]:
     if et_element is None:
         return NamedItemList(short_name_as_id)
```

### Comparing `odxtools-3.0.2/odxtools/comparam_subset.py` & `odxtools-4.0.0/odxtools/comparam_subset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Literal, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional, Union
 from xml.etree.ElementTree import Element
 
 from .admindata import AdminData
 from .companydata import CompanyData, create_company_datas_from_et
 from .dataobjectproperty import DataObjectProperty
 from .nameditemlist import NamedItemList
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from .odxtypes import odxstr_to_bool
 from .specialdata import SpecialDataGroup, create_sdgs_from_et
 from .units import UnitSpec
 from .utils import create_description_from_et, short_name_as_id
 
-StandardizationLevel = Literal["STANDARD", "OEM-SPECIFIC", "OPTIONAL", "OEM-OPTIONAL",]
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
 
-Usage = Literal["ECU-SOFTWARE", "ECU-COMM", "APPLICATION", "TESTER",]
+StandardizationLevel = Literal[
+    "STANDARD",
+    "OEM-SPECIFIC",
+    "OPTIONAL",
+    "OEM-OPTIONAL",
+]
+
+Usage = Literal[
+    "ECU-SOFTWARE",
+    "ECU-COMM",
+    "APPLICATION",
+    "TESTER",
+]
 
 ComplexValue = List[Union[str, "ComplexValue"]]
 
 
 def create_complex_value_from_et(et_element) -> ComplexValue:
     result = []
     for el in et_element:
@@ -49,20 +62,23 @@
         self.description = create_description_from_et(et_element.find("DESC"))
         self.param_class = et_element.attrib.get("PARAM-CLASS")
         self.cptype = et_element.attrib.get("CPTYPE")
         self.cpusage = et_element.attrib.get("CPUSAGE")
         dl = et_element.attrib.get("DISPLAY_LEVEL")
         self.display_level = None if dl is None else int(dl)
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
-        pass
-
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
         return {self.odx_id: self}
 
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        pass
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
 
 @dataclass
 class ComplexComparam(BaseComparam):
     comparams: NamedItemList[BaseComparam]
     complex_physical_default_value: Optional[ComplexValue]
     allow_multiple_values_raw: Optional[bool]
 
@@ -88,30 +104,36 @@
         super().__init_from_et__(et_element, doc_frags)
 
         self.comparams = NamedItemList(short_name_as_id)
         for cp_el in et_element:
             if cp_el.tag in ("COMPARAM", "COMPLEX-COMPARAM"):
                 self.comparams.append(create_any_comparam_from_et(cp_el, doc_frags))
 
+        self.complex_physical_default_value = None
         if cpdv_elem := et_element.find("COMPLEX-PHYSICAL-DEFAULT-VALUE"):
             self.complex_physical_default_value = create_complex_value_from_et(cpdv_elem)
 
         self.allow_multiple_values_raw = odxstr_to_bool(et_element.get("ALLOW-MULTIPLE-VALUES"))
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
-        super()._resolve_references(odxlinks)
-        for comparam in self.comparams:
-            comparam._resolve_references(odxlinks)
-
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
         odxlinks = super()._build_odxlinks()
         for comparam in self.comparams:
             odxlinks.update(comparam._build_odxlinks())
         return odxlinks
 
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        super()._resolve_odxlinks(odxlinks)
+        for comparam in self.comparams:
+            comparam._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        super()._resolve_snrefs(diag_layer)
+        for comparam in self.comparams:
+            comparam._resolve_snrefs(diag_layer)
+
 
 @dataclass
 class Comparam(BaseComparam):
     dop_ref: OdxLinkRef
     physical_default_value: Optional[str]
 
     @staticmethod
@@ -138,21 +160,27 @@
         self.physical_default_value = et_element.findtext("PHYSICAL-DEFAULT-VALUE")
 
     @property
     def dop(self) -> DataObjectProperty:
         """The data object property describing this parameter."""
         return self._dop
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return super()._build_odxlinks()
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         """Resolves the reference to the dop"""
-        super()._resolve_references(odxlinks)
+        super()._resolve_odxlinks(odxlinks)
 
         self._dop = odxlinks.resolve(self.dop_ref)
         assert isinstance(self._dop, DataObjectProperty)
 
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        super()._resolve_snrefs(diag_layer)
+
 
 @dataclass
 class ComparamSubset:
     odx_id: Optional[OdxLinkId]
     short_name: str
     # mandatory in ODX 2.2, but non existent in ODX 2.0
     category: Optional[str]
@@ -240,36 +268,59 @@
                 odxlinks.update(cd._build_odxlinks())
 
         for sdg in self.sdgs:
             odxlinks.update(sdg._build_odxlinks())
 
         return odxlinks
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        for dop in self.data_object_props:
+            dop._resolve_odxlinks(odxlinks)
+
+        for comparam in self.comparams:
+            comparam._resolve_odxlinks(odxlinks)
+
+        for comparam in self.complex_comparams:
+            comparam._resolve_odxlinks(odxlinks)
+
+        if self.unit_spec:
+            self.unit_spec._resolve_odxlinks(odxlinks)
+
+        if self.admin_data is not None:
+            self.admin_data._resolve_odxlinks(odxlinks)
+
+        if self.company_datas is not None:
+            for cd in self.company_datas:
+                cd._resolve_odxlinks(odxlinks)
+
+        for sdg in self.sdgs:
+            sdg._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
         for dop in self.data_object_props:
-            dop._resolve_references(odxlinks)
+            dop._resolve_snrefs(diag_layer)
 
         for comparam in self.comparams:
-            comparam._resolve_references(odxlinks)
+            comparam._resolve_snrefs(diag_layer)
 
         for comparam in self.complex_comparams:
-            comparam._resolve_references(odxlinks)
+            comparam._resolve_snrefs(diag_layer)
 
         if self.unit_spec:
-            self.unit_spec._resolve_references(odxlinks)
+            self.unit_spec._resolve_snrefs(diag_layer)
 
         if self.admin_data is not None:
-            self.admin_data._resolve_references(odxlinks)
+            self.admin_data._resolve_snrefs(diag_layer)
 
         if self.company_datas is not None:
             for cd in self.company_datas:
-                cd._resolve_references(odxlinks)
+                cd._resolve_snrefs(diag_layer)
 
         for sdg in self.sdgs:
-            sdg._resolve_references(odxlinks)
+            sdg._resolve_snrefs(diag_layer)
 
 
 def create_any_comparam_from_et(et_element, doc_frags: List[OdxDocFragment]) -> BaseComparam:
     if et_element.tag == "COMPARAM":
         return Comparam.from_et(et_element, doc_frags)
     elif et_element.tag == "COMPLEX-COMPARAM":
         return ComplexComparam.from_et(et_element, doc_frags)
```

### Comparing `odxtools-3.0.2/odxtools/compumethods/__init__.py` & `odxtools-4.0.0/odxtools/compumethods/__init__.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/compumethods/compumethodbase.py` & `odxtools-4.0.0/odxtools/compumethods/compumethodbase.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/compumethods/compuscale.py` & `odxtools-4.0.0/odxtools/compumethods/compuscale.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/compumethods/createanycompumethod.py` & `odxtools-4.0.0/odxtools/compumethods/createanycompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/compumethods/identicalcompumethod.py` & `odxtools-4.0.0/odxtools/compumethods/identicalcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/compumethods/limit.py` & `odxtools-4.0.0/odxtools/compumethods/limit.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/compumethods/linearcompumethod.py` & `odxtools-4.0.0/odxtools/compumethods/linearcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/compumethods/scalelinearcompumethod.py` & `odxtools-4.0.0/odxtools/compumethods/scalelinearcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/compumethods/tabintpcompumethod.py` & `odxtools-4.0.0/odxtools/compumethods/tabintpcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/compumethods/texttablecompumethod.py` & `odxtools-4.0.0/odxtools/compumethods/texttablecompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/database.py` & `odxtools-4.0.0/odxtools/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from pathlib import Path
 from typing import List, Optional, Set
 from xml.etree import ElementTree
 from xml.etree.ElementTree import Element
 from zipfile import ZipFile
 
 from .comparam_subset import ComparamSubset
-from .diaglayer import DiagLayer, DiagLayerContainer
-from .diaglayertype import DIAG_LAYER_TYPE
+from .diaglayer import DiagLayer
+from .diaglayercontainer import DiagLayerContainer
+from .diaglayertype import DiagLayerType
 from .globals import logger
 from .nameditemlist import NamedItemList
 from .odxlink import OdxLinkDatabase
 from .utils import short_name_as_id
 
 
 def version(v: str):
@@ -29,16 +30,16 @@
     def __init__(self,
                  *,
                  pdx_zip: Optional[ZipFile] = None,
                  odx_d_file_name: Optional[str] = None) -> None:
 
         if pdx_zip is None and odx_d_file_name is None:
             # create an empty database object
-            self._diag_layer_containers = NamedItemList(short_name_as_id, [])
-            self._comparam_subsets = NamedItemList(short_name_as_id, [])
+            self._diag_layer_containers = NamedItemList(short_name_as_id)
+            self._comparam_subsets = NamedItemList(short_name_as_id)
             return
 
         if pdx_zip is not None and odx_d_file_name is not None:
             raise TypeError("The 'pdx_zip' and 'odx_d_file_name' parameters are mutually exclusive")
 
         documents: List[Element] = []
         if pdx_zip is not None:
@@ -77,77 +78,75 @@
                 if subset is not None:
                     comparam_subsets.append(ComparamSubset.from_et(subset))
 
         self._diag_layer_containers = NamedItemList(short_name_as_id, dlcs)
         self._diag_layer_containers.sort(key=short_name_as_id)
         self._comparam_subsets = NamedItemList(short_name_as_id, comparam_subsets)
         self._comparam_subsets.sort(key=short_name_as_id)
-        self.finalize_init()
 
-    def finalize_init(self) -> None:
+        self.refresh()
+
+    def refresh(self) -> None:
         # Create wrapper objects
         self._diag_layers = NamedItemList(
             short_name_as_id, chain(*[dlc.diag_layers for dlc in self.diag_layer_containers]))
+
+        self._protocols = NamedItemList(
+            short_name_as_id, chain(*[dlc.protocols for dlc in self.diag_layer_containers]))
+
         self._ecus = NamedItemList(short_name_as_id,
                                    chain(*[dlc.ecu_variants for dlc in self.diag_layer_containers]))
 
         # Build odxlinks
         self._odxlinks = OdxLinkDatabase()
 
         for subset in self.comparam_subsets:
             self._odxlinks.update(subset._build_odxlinks())
 
         for dlc in self.diag_layer_containers:
             self._odxlinks.update(dlc._build_odxlinks())
 
-        for dl in self.diag_layers:
-            self._odxlinks.update(dl._build_odxlinks())
-
-        # Resolve references
+        # Resolve ODXLINK references
         for subset in self.comparam_subsets:
-            subset._resolve_references(self._odxlinks)
+            subset._resolve_odxlinks(self._odxlinks)
+
         for dlc in self.diag_layer_containers:
-            dlc._resolve_references(self._odxlinks)
+            dlc._resolve_odxlinks(self._odxlinks)
 
-        for dl_type_name in DIAG_LAYER_TYPE:
-            for dl in self.diag_layers:
-                if dl.variant_type == dl_type_name:
-                    dl._resolve_references(self._odxlinks)
+        # let the diaglayers sort out the inherited objects and the
+        # short name references
+        for dlc in self.diag_layer_containers:
+            dlc._finalize_init(self._odxlinks)
 
     @property
     def odxlinks(self) -> OdxLinkDatabase:
         """A map from odx_id to object"""
         return self._odxlinks
 
     @property
+    def protocols(self) -> NamedItemList[DiagLayer]:
+        """
+        All protocols defined by this database
+        """
+        return self._protocols
+
+    @property
     def ecus(self) -> NamedItemList[DiagLayer]:
-        """ECU-variants defined in the data base"""
+        """ECU-variants defined in the database"""
         return self._ecus
 
     @property
     def diag_layers(self) -> NamedItemList[DiagLayer]:
-        """all diagnostic layers defined in the data base"""
+        """All diagnostic layers defined in the database"""
         return self._diag_layers
 
     @property
     def diag_layer_containers(self):
         return self._diag_layer_containers
 
     @diag_layer_containers.setter
     def diag_layer_containers(self, value):
         self._diag_layer_containers = value
 
     @property
     def comparam_subsets(self):
         return self._comparam_subsets
-
-    @property
-    def protocols(self) -> NamedItemList[DiagLayer]:
-        """
-        Return a list of all protocols defined by this database
-        """
-        result_dict = dict()
-        for dl in self.diag_layers:
-            if dl.variant_type == DIAG_LAYER_TYPE.PROTOCOL:
-                result_dict[dl.short_name] = dl
-
-        return NamedItemList(short_name_as_id, list(result_dict.values()))
```

### Comparing `odxtools-3.0.2/odxtools/dataobjectproperty.py` & `odxtools-4.0.0/odxtools/dataobjectproperty.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union, cast
 
 from .compumethods import CompuMethod, create_any_compu_method_from_et
 from .decodestate import DecodeState
 from .diagcodedtypes import DiagCodedType, StandardLengthType, create_any_diag_coded_type_from_et
 from .encodestate import EncodeState
 from .exceptions import DecodeError, EncodeError
 from .globals import logger
@@ -13,40 +13,59 @@
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from .odxtypes import odxstr_to_bool
 from .physicaltype import PhysicalType
 from .specialdata import SpecialDataGroup, create_sdgs_from_et
 from .units import Unit
 from .utils import create_description_from_et, short_name_as_id
 
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
 
+
+@dataclass
 class DopBase:
     """Base class for all DOPs.
 
     Any class that a parameter can reference via a DOP-REF should inherit from this class.
     """
 
-    def __init__(self, *, odx_id, short_name, long_name, description, is_visible_raw, sdgs=[]):
-        self.odx_id = odx_id
-        self.short_name = short_name
-        self.long_name = long_name
-        self.description = description
-        self.is_visible_raw = is_visible_raw
-        self.sdgs = sdgs
+    odx_id: OdxLinkId
+    short_name: str
+    long_name: Optional[str]
+    description: Optional[str]
+    is_visible_raw: Optional[bool]
+    sdgs: List[SpecialDataGroup]
+
+    def __hash__(self) -> int:
+        result = 0
+
+        result += hash(self.short_name)
+        result += hash(self.long_name)
+        result += hash(self.description)
+        result += hash(self.is_visible_raw)
+        for sdg in self.sdgs:
+            result += hash(sdg)
+
+        return result
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
-        result = {}
+        result = {self.odx_id: self}
 
         for sdg in self.sdgs:
             result.update(sdg._build_odxlinks())
 
         return result
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         for sdg in self.sdgs:
-            sdg._resolve_references(odxlinks)
+            sdg._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        for sdg in self.sdgs:
+            sdg._resolve_snrefs(diag_layer)
 
     @property
     def is_visible(self) -> bool:
         return self.is_visible_raw in (None, True)
 
     def convert_physical_to_bytes(self, physical_value, encode_state: EncodeState,
                                   bit_position: int) -> bytes:
@@ -60,38 +79,26 @@
 
 class DataObjectProperty(DopBase):
     """This class represents a DATA-OBJECT-PROP."""
 
     def __init__(
         self,
         *,
-        odx_id: OdxLinkId,
-        short_name: str,
         diag_coded_type: DiagCodedType,
         physical_type: PhysicalType,
         compu_method: CompuMethod,
         unit_ref: Optional[OdxLinkRef],
-        long_name: Optional[str],
-        description: Optional[str],
-        is_visible_raw: Optional[bool],
-        sdgs: List[SpecialDataGroup],
+        **kwargs,
     ):
-        super().__init__(
-            odx_id=odx_id,
-            short_name=short_name,
-            long_name=long_name,
-            description=description,
-            is_visible_raw=is_visible_raw,
-            sdgs=sdgs,
-        )
+        super().__init__(**kwargs)
+
         self.diag_coded_type = diag_coded_type
         self.physical_type = physical_type
         self.compu_method = compu_method
         self.unit_ref = unit_ref
-        self._unit = None
 
     @staticmethod
     def from_et(et_element, doc_frags: List[OdxDocFragment]) -> "DataObjectProperty":
         """Reads a DATA-OBJECT-PROP or a DTC-DOP."""
         odx_id = OdxLinkId.from_et(et_element, doc_frags)
         assert odx_id is not None
         short_name = et_element.findtext("SHORT-NAME")
@@ -131,15 +138,15 @@
                 for dtc_proxy_elem in dtcs_elem:
                     if dtc_proxy_elem.tag == "DTC":
                         dtclist.append(DiagnosticTroubleCode.from_et(dtc_proxy_elem, doc_frags))
                     elif dtc_proxy_elem.tag == "DTC-REF":
                         dtclist.append(OdxLinkRef.from_et(dtc_proxy_elem, doc_frags))
 
             # TODO: NOT-INHERITED-DTC-SNREFS
-            linked_dtc_dops = [
+            linked_dtc_dop_refs = [
                 cast(OdxLinkRef, OdxLinkRef.from_et(dtc_ref_elem, doc_frags))
                 for dtc_ref_elem in et_element.iterfind("LINKED-DTC-DOPS/"
                                                         "LINKED-DTC-DOP/"
                                                         "DTC-DOP-REF")
             ]
 
             dop = DtcDop(
@@ -148,20 +155,34 @@
                 long_name=long_name,
                 description=description,
                 diag_coded_type=diag_coded_type,
                 physical_type=physical_type,
                 compu_method=compu_method,
                 unit_ref=unit_ref,
                 dtcs_raw=dtclist,
-                linked_dtc_dops=linked_dtc_dops,
+                linked_dtc_dop_refs=linked_dtc_dop_refs,
                 is_visible_raw=is_visible_raw,
                 sdgs=sdgs,
             )
         return dop
 
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return super()._build_odxlinks()
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase):
+        """Resolves the reference to the unit"""
+        super()._resolve_odxlinks(odxlinks)
+
+        self._unit: Optional[Unit] = None
+        if self.unit_ref:
+            self._unit = odxlinks.resolve(self.unit_ref, Unit)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        super()._resolve_snrefs(diag_layer)
+
     @property
     def unit(self) -> Optional[Unit]:
         return self._unit
 
     @property
     def bit_length(self):
         # TODO: The DiagCodedTypes except StandardLengthType don't have a bit length.
@@ -206,21 +227,14 @@
 
     def is_valid_physical_value(self, physical_value):
         return self.compu_method.is_valid_physical_value(physical_value)
 
     def get_valid_physical_values(self):
         return self.compu_method.get_valid_physical_values()
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
-        """Resolves the reference to the unit"""
-        super()._resolve_references(odxlinks)
-
-        if self.unit_ref:
-            self._unit = odxlinks.resolve(self.unit_ref)
-
     def __repr__(self) -> str:
         return (f"DataObjectProperty('{self.short_name}', " + ", ".join([
             f"category='{self.compu_method.category}'",
             f"internal_type='{self.diag_coded_type}'",
             f"physical_type={self.physical_type}",
             f"unit_ref='{self.unit_ref}'",
         ]) + ")")
@@ -272,64 +286,55 @@
             display_trouble_code=display_trouble_code,
             level=level,
             is_temporary_raw=is_temporary_raw,
             sdgs=sdgs,
         )
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
-        result = {}
+        result: Dict[OdxLinkId, Any] = {}
+
+        if self.odx_id is not None:
+            result[self.odx_id] = self
 
         for sdg in self.sdgs:
             result.update(sdg._build_odxlinks())
 
         return result
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        for sdg in self.sdgs:
+            sdg._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer"):
         for sdg in self.sdgs:
-            sdg._resolve_references(odxlinks)
+            sdg._resolve_snrefs(diag_layer)
 
 
 class DtcDop(DataObjectProperty):
     """A DOP describing a diagnostic trouble code"""
 
     def __init__(
         self,
         *,
-        odx_id: OdxLinkId,
-        short_name: str,
-        diag_coded_type: DiagCodedType,
-        physical_type: PhysicalType,
-        compu_method: CompuMethod,
-        unit_ref: Optional[OdxLinkRef],
         dtcs_raw: List[Union[DiagnosticTroubleCode, OdxLinkRef]],
-        is_visible_raw: bool,
-        linked_dtc_dops: List[OdxLinkRef],
-        long_name: Optional[str],
-        description: Optional[str],
-        sdgs: List[SpecialDataGroup],
+        linked_dtc_dop_refs: List[OdxLinkRef],
+        **kwargs,
     ):
-        super().__init__(
-            odx_id=odx_id,
-            short_name=short_name,
-            long_name=long_name,
-            description=description,
-            diag_coded_type=diag_coded_type,
-            physical_type=physical_type,
-            compu_method=compu_method,
-            unit_ref=unit_ref,
-            is_visible_raw=is_visible_raw,
-            sdgs=sdgs,
-        )
+        super().__init__(**kwargs)
         self.dtcs_raw = dtcs_raw
-        self.linked_dtc_dops = linked_dtc_dops
+        self.linked_dtc_dop_refs = linked_dtc_dop_refs
 
     @property
     def dtcs(self) -> NamedItemList[DiagnosticTroubleCode]:
         return self._dtcs
 
+    @property
+    def linked_dtc_dops(self) -> NamedItemList["DtcDop"]:
+        return self._linked_dtc_dops
+
     def convert_bytes_to_physical(self, decode_state, bit_position: int = 0):
         trouble_code, next_byte = super().convert_bytes_to_physical(
             decode_state, bit_position=bit_position)
 
         dtcs = [x for x in self.dtcs if x.trouble_code == trouble_code]
 
         assert len(dtcs) < 2, f"Multiple matching DTCs for trouble code 0x{trouble_code:06x}"
@@ -369,26 +374,34 @@
             raise EncodeError(f"The DTC-DOP {self.short_name} expected a"
                               f" DiagnosticTroubleCode but got {physical_value}.")
 
         return super().convert_physical_to_bytes(trouble_code, encode_state, bit_position)
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
         odxlinks = super()._build_odxlinks()
-        odxlinks[self.odx_id] = self
+
         for dtc_proxy in self.dtcs_raw:
             if isinstance(dtc_proxy, DiagnosticTroubleCode):
-                assert dtc_proxy.odx_id is not None
-                odxlinks[dtc_proxy.odx_id] = dtc_proxy
                 odxlinks.update(dtc_proxy._build_odxlinks())
 
         return odxlinks
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
-        super()._resolve_references(odxlinks)
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase):
+        super()._resolve_odxlinks(odxlinks)
 
         self._dtcs: NamedItemList[DiagnosticTroubleCode] = NamedItemList(short_name_as_id)
         for dtc_proxy in self.dtcs_raw:
             if isinstance(dtc_proxy, DiagnosticTroubleCode):
                 self._dtcs.append(dtc_proxy)
             elif isinstance(dtc_proxy, OdxLinkRef):
                 dtc = odxlinks.resolve(dtc_proxy, DiagnosticTroubleCode)
                 self._dtcs.append(dtc)
+
+        linked_dtc_dops = [odxlinks.resolve(x, DtcDop) for x in self.linked_dtc_dop_refs]
+        self._linked_dtc_dops = NamedItemList(short_name_as_id, linked_dtc_dops)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer"):
+        super()._resolve_snrefs(diag_layer)
+
+        for dtc_proxy in self.dtcs_raw:
+            if isinstance(dtc_proxy, DiagnosticTroubleCode):
+                dtc_proxy._resolve_snrefs(diag_layer)
```

### Comparing `odxtools-3.0.2/odxtools/decodestate.py` & `odxtools-4.0.0/odxtools/decodestate.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/diagcodedtypes.py` & `odxtools-4.0.0/odxtools/diagcodedtypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,16 +224,16 @@
         super().__init__(
             base_data_type=base_data_type,
             dct_type="LEADING-LENGTH-INFO-TYPE",
             base_type_encoding=base_type_encoding,
             is_highlow_byte_order_raw=is_highlow_byte_order_raw,
         )
         self.bit_length = bit_length
-        assert (self.bit_length >
-                0), "A Leading length info type with bit length == 0 does not make sense."
+        assert (self.bit_length
+                > 0), "A Leading length info type with bit length == 0 does not make sense."
         assert self.base_data_type in [
             DataType.A_BYTEFIELD,
             DataType.A_ASCIISTRING,
             DataType.A_UNICODE2STRING,
             DataType.A_UTF8STRING,
         ], f"A leading length info type cannot have the base data type {self.base_data_type}."
 
@@ -636,15 +636,16 @@
             bit_length=bit_length,
             base_type_encoding=base_type_encoding,
             is_highlow_byte_order_raw=is_highlow_byte_order_raw,
         )
     elif dct_type == "MIN-MAX-LENGTH-TYPE":
         min_length = int(et_element.findtext("MIN-LENGTH"))
         max_length = None
-        if et_element.find("MAX-LENGTH"):
+        # comparison has to be 'is not None' as Element overwrites __bool__(), and always returns false for MAX-LENGTH elements
+        if et_element.find("MAX-LENGTH") is not None:
             max_length = int(et_element.findtext("MAX-LENGTH"))
         termination = et_element.get("TERMINATION")
 
         return MinMaxLengthType(
             base_data_type=base_data_type,
             min_length=min_length,
             max_length=max_length,
```

### Comparing `odxtools-3.0.2/odxtools/diagdatadictionaryspec.py` & `odxtools-4.0.0/odxtools/diagdatadictionaryspec.py`

 * *Files 7% similar despite different names*

```diff
@@ -127,22 +127,16 @@
             env_data_descs=NamedItemList(short_name_as_id, env_data_descs),
             env_datas=NamedItemList(short_name_as_id, env_datas),
             muxs=NamedItemList(short_name_as_id, muxs),
             sdgs=sdgs,
         )
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        # note that DataDictionarySpec objects do not exhibit an ODXLINK id.
         odxlinks = {}
-        for obj in chain(
-                self.data_object_props,
-                self.structures,
-                self.end_of_pdu_fields,
-                self.tables,
-        ):
-            odxlinks[obj.odx_id] = obj
 
         for obj in chain(
                 self.data_object_props,
                 self.dtc_dops,
                 self.env_data_descs,
                 self.env_datas,
                 self.muxs,
@@ -154,34 +148,29 @@
             odxlinks.update(obj._build_odxlinks())
 
         if self.unit_spec is not None:
             odxlinks.update(self.unit_spec._build_odxlinks())
 
         return odxlinks
 
-    def _resolve_references(self, parent_dl: "DiagLayer", odxlinks: OdxLinkDatabase):
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+
+        for obj in chain(self.data_object_props, self.dtc_dops, self.end_of_pdu_fields,
+                         self.env_data_descs, self.env_datas, self.muxs, self.sdgs, self.structures,
+                         self.tables):
+            obj._resolve_odxlinks(odxlinks)
+
+        if self.unit_spec:
+            self.unit_spec._resolve_odxlinks(odxlinks)
 
-        for obj in self.data_object_props:
-            obj._resolve_references(odxlinks)
-        for obj in self.dtc_dops:
-            obj._resolve_references(odxlinks)
-        for obj in self.end_of_pdu_fields:
-            obj._resolve_references(parent_dl, odxlinks)
-        for obj in self.env_data_descs:
-            obj._resolve_references(odxlinks)
-        for obj in self.env_datas:
-            obj._resolve_references(parent_dl, odxlinks)
-        for obj in self.muxs:
-            obj._resolve_references(odxlinks)
-        for obj in self.sdgs:
-            obj._resolve_references(odxlinks)
-        for obj in self.structures:
-            obj._resolve_references(parent_dl, odxlinks)
-        for obj in self.tables:
-            obj._resolve_references(odxlinks)
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        for obj in chain(self.data_object_props, self.dtc_dops, self.end_of_pdu_fields,
+                         self.env_data_descs, self.env_datas, self.muxs, self.sdgs, self.structures,
+                         self.tables):
+            obj._resolve_snrefs(diag_layer)
 
         if self.unit_spec:
-            self.unit_spec._resolve_references(odxlinks)
+            self.unit_spec._resolve_snrefs(diag_layer)
 
     @property
     def all_data_object_properties(self):
         return self._all_data_object_properties
```

### Comparing `odxtools-3.0.2/odxtools/ecu_variant_matcher.py` & `odxtools-4.0.0/odxtools/ecu_variant_matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2023 MBition GmbH
 
 from enum import Enum
 from typing import ByteString, Dict, Generator, List, Optional, Union
 
 from odxtools.diaglayer import DiagLayer
-from odxtools.diaglayertype import DIAG_LAYER_TYPE
+from odxtools.diaglayertype import DiagLayerType
 from odxtools.ecu_variant_patterns import MatchingParameter
 from odxtools.exceptions import OdxError
 from odxtools.service import DiagService
 from odxtools.structures import Response
 
 
 class EcuVariantMatcher:
@@ -17,15 +17,15 @@
     ECU-VARIANT-PATTERN according to ISO 22901-1.
 
     Usage (example):
 
     ```python
 
     # initialize the matcher with a list of ecu variants,
-    # i.e., DiagLayer instances of variant_type == DIAG_LAYER_TYPE.ECU-VARIANT
+    # i.e., DiagLayer instances of variant_type == DiagLayerType.ECU-VARIANT
     matcher = EcuVariantMatcher(ecu_variant_candidates=[...], use_cache=use_cache)
 
     # run the request loop to obtain responses for every request
     for req in matcher.request_loop():
         resp = ... # make a UDS request
         matcher.evaluate(resp)
 
@@ -91,15 +91,15 @@
         raise OdxError(f"The snref or snpathref '{matching_param.out_param_if}' is cannot be \
                 resolved for any positive or negative response.")
 
     def __init__(self, ecu_variant_candidates: List[DiagLayer], use_cache: bool = True):
 
         self.ecus = ecu_variant_candidates
         for ecu in self.ecus:
-            assert ecu.variant_type == DIAG_LAYER_TYPE.ECU_VARIANT
+            assert ecu.variant_type == DiagLayerType.ECU_VARIANT
 
         self.use_cache = use_cache
         self.req_resp_cache: Dict[ByteString, bytes] = {}
         self._recent_ident_response: Optional[bytes] = None
 
         self._state = EcuVariantMatcher.State.PENDING
```

### Comparing `odxtools-3.0.2/odxtools/ecu_variant_patterns.py` & `odxtools-4.0.0/odxtools/ecu_variant_patterns.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/encodestate.py` & `odxtools-4.0.0/odxtools/encodestate.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/endofpdufield.py` & `odxtools-4.0.0/odxtools/endofpdufield.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TYPE_CHECKING, List, Optional, Union
 
 from .dataobjectproperty import DopBase
 from .decodestate import DecodeState
 from .encodestate import EncodeState
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from .odxtypes import odxstr_to_bool
+from .specialdata import create_sdgs_from_et
 from .structures import BasicStructure
 from .utils import create_description_from_et
 
 if TYPE_CHECKING:
     from .diaglayer import DiagLayer
 
 
@@ -50,14 +51,15 @@
     @staticmethod
     def from_et(et_element, doc_frags: List[OdxDocFragment]) -> "EndOfPduField":
         odx_id = OdxLinkId.from_et(et_element, doc_frags)
         assert odx_id is not None
         short_name = et_element.findtext("SHORT-NAME")
         long_name = et_element.findtext("LONG-NAME")
         description = create_description_from_et(et_element.find("DESC"))
+        sdgs = create_sdgs_from_et(et_element.find("SDGS"), doc_frags)
 
         structure_ref = OdxLinkRef.from_et(et_element.find("BASIC-STRUCTURE-REF"), doc_frags)
         structure_snref = None
         if (edsnr_elem := et_element.find("BASIC-STRUCTURE-SNREF")) is not None:
             structure_snref = edsnr_elem.get("SHORT-NAME")
 
         env_data_desc_ref = OdxLinkRef.from_et(et_element.find("ENV-DATA-DESC-REF"), doc_frags)
@@ -76,14 +78,15 @@
 
         is_visible_raw = odxstr_to_bool(et_element.get("IS-VISIBLE"))
         eopf = EndOfPduField(
             odx_id=odx_id,
             short_name=short_name,
             long_name=long_name,
             description=description,
+            sdgs=sdgs,
             structure_ref=structure_ref,
             structure_snref=structure_snref,
             env_data_desc_ref=env_data_desc_ref,
             env_data_desc_snref=env_data_desc_snref,
             min_number_of_items=min_number_of_items,
             max_number_of_items=max_number_of_items,
             is_visible_raw=is_visible_raw,
@@ -138,26 +141,31 @@
                 decode_state, bit_position=bit_position)
             # Update next byte_position
             decode_state = decode_state._replace(next_byte_position=next_byte_position)
             value.append(new_value)
 
         return value, next_byte_position
 
-    def _resolve_references(  # type: ignore[override]
-            self, parent_dl: "DiagLayer", odxlinks: OdxLinkDatabase) -> None:
-        """Recursively resolve any references (odxlinks or sn-refs)"""
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        """Recursively resolve any odxlinks references"""
         if self.structure_ref is not None:
             self._structure = odxlinks.resolve(self.structure_ref)
-        elif self.structure_snref is not None:
-            self._structure = parent_dl.data_object_properties[self.structure_snref]
 
         if self.env_data_desc_ref is not None:
             self._env_data_desc = odxlinks.resolve(self.env_data_desc_ref)
-        elif self.env_data_desc_snref is not None:
-            self._env_data_desc = parent_dl.data_object_properties[self.env_data_desc_snref]
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        """Recursively resolve any short-name references"""
+        if self.structure_snref is not None:
+            dops = diag_layer.diag_data_dictionary_spec.data_object_props
+            self._structure = dops[self.structure_snref]
+
+        if self.env_data_desc_snref is not None:
+            dops = diag_layer.diag_data_dictionary_spec.data_object_props
+            self._env_data_desc = dops[self.env_data_desc_snref]
 
     def __repr__(self) -> str:
         return f"EndOfPduField(short_name='{self.short_name}', ref='{self.structure.odx_id}')"
 
     def __str__(self):
         return "\n".join(
             [f"EndOfPduField(short_name='{self.short_name}', ref='{self.structure.odx_id}')"] +
```

### Comparing `odxtools-3.0.2/odxtools/envdata.py` & `odxtools-4.0.0/odxtools/envdata.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from .globals import logger
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId
 from .odxtypes import odxstr_to_bool
 from .parameters import create_any_parameter_from_et
 from .parameters.parameterbase import Parameter
+from .specialdata import create_sdgs_from_et
 from .structures import BasicStructure
 from .utils import create_description_from_et
 
 if TYPE_CHECKING:
     from .diaglayer import DiagLayer
 
 
@@ -29,14 +30,15 @@
     def from_et(et_element, doc_frags: List[OdxDocFragment]) -> "EnvironmentData":
         """Reads Environment Data from Diag Layer."""
         odx_id = OdxLinkId.from_et(et_element, doc_frags)
         assert odx_id is not None
         short_name = et_element.findtext("SHORT-NAME")
         long_name = et_element.findtext("LONG-NAME")
         description = create_description_from_et(et_element.find("DESC"))
+        sdgs = create_sdgs_from_et(et_element.find("SDGS"), doc_frags)
         is_visible_raw = odxstr_to_bool(et_element.get("IS-VISIBLE"))
         parameters = [
             create_any_parameter_from_et(et_parameter, doc_frags)
             for et_parameter in et_element.iterfind("PARAMS/PARAM")
         ]
         byte_size_text = et_element.findtext("BYTE-SIZE")
         byte_size = None if byte_size_text is None else int(byte_size_text)
@@ -45,27 +47,17 @@
         ]
 
         return EnvironmentData(
             odx_id=odx_id,
             short_name=short_name,
             long_name=long_name,
             description=description,
+            sdgs=sdgs,
             is_visible_raw=is_visible_raw,
             parameters=parameters,
             byte_size=byte_size,
             dtc_values=dtc_values,
         )
 
-    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
-        odxlinks = super()._build_odxlinks()
-
-        odxlinks[self.odx_id] = self
-
-        return odxlinks
-
-    def _resolve_references(  # type: ignore[override]
-            self, parent_dl: "DiagLayer", odxlinks: OdxLinkDatabase) -> None:
-        super()._resolve_references(parent_dl, odxlinks)
-
     def __repr__(self) -> str:
         return (f"EnvironmentData('{self.short_name}', " +
                 ", ".join([f"odx_id='{self.odx_id}'", f"parameters='{self.parameters}'"]) + ")")
```

### Comparing `odxtools-3.0.2/odxtools/envdatadesc.py` & `odxtools-4.0.0/odxtools/envdatadesc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from .dataobjectproperty import DopBase
 from .decodestate import DecodeState
 from .encodestate import EncodeState
 from .envdata import EnvironmentData
 from .exceptions import DecodeError, EncodeError
 from .globals import logger
-from .odxlink import OdxDocFragment, OdxLinkId, OdxLinkRef
+from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from .odxtypes import odxstr_to_bool
+from .specialdata import create_sdgs_from_et
 from .utils import create_description_from_et
 
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
+
 
 class EnvironmentDataDescription(DopBase):
     """This class represents Environment Data Description, which is a complex DOP
     that is used to define the interpretation of environment data."""
 
     def __init__(
         self,
@@ -42,14 +46,15 @@
     def from_et(et_element, doc_frags: List[OdxDocFragment]) -> "EnvironmentDataDescription":
         """Reads Environment Data Description from Diag Layer."""
         odx_id = OdxLinkId.from_et(et_element, doc_frags)
         assert odx_id is not None
         short_name = et_element.findtext("SHORT-NAME")
         long_name = et_element.findtext("LONG-NAME")
         description = create_description_from_et(et_element.find("DESC"))
+        sdgs = create_sdgs_from_et(et_element.find("SDGS"), doc_frags)
         is_visible_raw = odxstr_to_bool(et_element.get("IS-VISIBLE"))
         param_snref = None
         if et_element.find("PARAM-SNREF") is not None:
             param_snref = et_element.find("PARAM-SNREF").get("SHORT-NAME")
         param_snpathref = None
         if et_element.find("PARAM-SNPATHREF") is not None:
             param_snpathref = et_element.find("PARAM-SNPATHREF").get("SHORT-NAME-PATH")
@@ -68,30 +73,46 @@
         logger.debug("Parsing ENV-DATA-DESC " + short_name)
 
         return EnvironmentDataDescription(
             odx_id=odx_id,
             short_name=short_name,
             long_name=long_name,
             description=description,
+            sdgs=sdgs,
             is_visible_raw=is_visible_raw,
             param_snref=param_snref,
             param_snpathref=param_snpathref,
             env_datas=env_datas,
             env_data_refs=env_data_refs,
         )
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
-        odxlinks = {}
-        odxlinks[self.odx_id] = self
+        odxlinks = {self.odx_id: self}
 
         for ed in self.env_datas:
             odxlinks.update(ed._build_odxlinks())
 
         return odxlinks
 
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        # ODX 2.0 specifies environment data objects here, ODX 2.2
+        # uses references
+        if self.env_data_refs:
+            self.env_datas = [odxlinks.resolve(x) for x in self.env_data_refs]
+        else:
+            for ed in self.env_datas:
+                ed._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        # ODX 2.0 specifies environment data objects here, ODX 2.2
+        # uses references
+        if self.env_data_refs:
+            for ed in self.env_datas:
+                ed._resolve_snrefs(diag_layer)
+
     def __repr__(self) -> str:
         return (f"EnvironmentDataDescription('{self.short_name}', " + ", ".join([
             f"odx_id='{self.odx_id}'",
             f"param_snref='{self.param_snref}'",
             f"param_snpathref='{self.param_snpathref}'",
             f"env_data_refs='{self.env_data_refs}'",
         ]) + ")")
```

### Comparing `odxtools-3.0.2/odxtools/exceptions.py` & `odxtools-4.0.0/odxtools/exceptions.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/functionalclass.py` & `odxtools-4.0.0/odxtools/functionalclass.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId
 from .utils import create_description_from_et
 
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
+
 
 @dataclass
 class FunctionalClass:
     """
     Corresponds to FUNCT-CLASS.
     """
 
@@ -29,9 +32,12 @@
 
         return FunctionalClass(
             odx_id=odx_id, short_name=short_name, long_name=long_name, description=description)
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
         return {self.odx_id: self}
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        pass
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
         pass
```

### Comparing `odxtools-3.0.2/odxtools/isotp_state_machine.py` & `odxtools-4.0.0/odxtools/isotp_state_machine.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/message.py` & `odxtools-4.0.0/odxtools/message.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/multiplexer.py` & `odxtools-4.0.0/odxtools/multiplexer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 from collections import OrderedDict
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from .dataobjectproperty import DataObjectProperty, DopBase
 from .decodestate import DecodeState
 from .encodestate import EncodeState
 from .exceptions import DecodeError, EncodeError
 from .globals import logger
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
+from .odxtypes import odxstr_to_bool
+from .specialdata import create_sdgs_from_et
 from .structures import BasicStructure
+from .utils import create_description_from_et
+
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
 
 
 @dataclass
 class MultiplexerCase:
     """This class represents a Case which represents multiple options in a Multiplexer."""
 
     short_name: str
@@ -40,17 +46,23 @@
             short_name=short_name,
             long_name=long_name,
             structure_ref=structure_ref,
             lower_limit=lower_limit,
             upper_limit=upper_limit,
         )
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         self._structure = odxlinks.resolve(self.structure_ref)
 
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
     def __repr__(self) -> str:
         return (f"MultiplexerCase('{self.short_name}', " + ", ".join([
             f"lower_limit='{self.lower_limit}'",
             f"upper_limit='{self.upper_limit}'",
             f"structure_ref='{self.structure_ref}'",
         ]) + ")")
 
@@ -76,18 +88,24 @@
 
         return MultiplexerDefaultCase(
             short_name=short_name,
             long_name=long_name,
             structure_ref=structure_ref,
         )
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         if self.structure_ref is not None:
             self._structure = odxlinks.resolve(self.structure_ref)
 
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
     def __repr__(self) -> str:
         return (f"MultiplexerDefaultCase('{self.short_name}', " + ", ".join([
             f"structure_ref='{self.structure_ref}'",
         ]) + ")")
 
 
 @dataclass
@@ -113,50 +131,56 @@
 
         return MultiplexerSwitchKey(
             byte_position=byte_position,
             bit_position=bit_position,
             dop_ref=dop_ref,
         )
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         dop = odxlinks.resolve(self.dop_ref)
         if isinstance(dop, DataObjectProperty):
             self._dop = dop
         else:
             logger.warning(
                 f"DATA-OBJECT-PROP-REF '{self.dop_ref}' could not be resolved in SWITCH-KEY.")
 
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
     def __repr__(self) -> str:
         return (f"MultiplexerSwitchKey(" + ", ".join([
             f"byte_position={self.byte_position}",
             f"bit_position={self.bit_position}",
             f"dop_ref={self.dop_ref}",
         ]) + ")")
 
 
 @dataclass
 class Multiplexer(DopBase):
     """This class represents a Multiplexer (MUX) which are used to interpret data stream depending on the value
     of a switch-key (similar to switch-case statements in programming languages like C or Java)."""
 
-    odx_id: OdxLinkId
-    short_name: str
-    long_name: str
     byte_position: int
     switch_key: MultiplexerSwitchKey
     default_case: Optional[MultiplexerDefaultCase]
     cases: List[MultiplexerCase]
 
     @staticmethod
     def from_et(et_element, doc_frags: List[OdxDocFragment]) -> "Multiplexer":
         """Reads a Multiplexer from Diag Layer."""
         odx_id = OdxLinkId.from_et(et_element, doc_frags)
         assert odx_id is not None
         short_name = et_element.findtext("SHORT-NAME")
         long_name = et_element.findtext("LONG-NAME")
+        description = create_description_from_et(et_element.find("DESC"))
+        is_visible_raw = odxstr_to_bool(et_element.get("IS-VISIBLE"))
+        sdgs = create_sdgs_from_et(et_element.find("SDGS"), doc_frags)
         byte_position = int(et_element.findtext("BYTE-POSITION", "0"))
         switch_key = MultiplexerSwitchKey.from_et(et_element.find("SWITCH-KEY"), doc_frags)
 
         default_case = None
         if et_element.find("DEFAULT-CASE") is not None:
             default_case = MultiplexerDefaultCase.from_et(
                 et_element.find("DEFAULT-CASE"), doc_frags)
@@ -170,14 +194,17 @@
 
         logger.debug("Parsing MUX " + short_name)
 
         return Multiplexer(
             odx_id=odx_id,
             short_name=short_name,
             long_name=long_name,
+            description=description,
+            sdgs=sdgs,
+            is_visible_raw=is_visible_raw,
             byte_position=byte_position,
             switch_key=switch_key,
             default_case=default_case,
             cases=cases,
         )
 
     @property
@@ -273,25 +300,37 @@
 
         mux_value = OrderedDict({case.short_name: case_value})
         mux_next_byte = decode_state.next_byte_position + max(
             key_next_byte + self.switch_key.byte_position, case_next_byte + self.byte_position)
         return mux_value, mux_next_byte
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
-        odxlinks = {}
-        odxlinks.update({self.odx_id: self})
+        odxlinks = super()._build_odxlinks()
+
         return odxlinks
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
-        self.switch_key._resolve_references(odxlinks)
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        super()._resolve_odxlinks(odxlinks)
+
+        self.switch_key._resolve_odxlinks(odxlinks)
         if self.default_case is not None:
-            self.default_case._resolve_references(odxlinks)
+            self.default_case._resolve_odxlinks(odxlinks)
 
-        for case in self.cases or []:
-            case._resolve_references(odxlinks)
+        for case in self.cases:
+            case._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer"):
+        super()._resolve_snrefs(diag_layer)
+
+        self.switch_key._resolve_snrefs(diag_layer)
+        if self.default_case is not None:
+            self.default_case._resolve_snrefs(diag_layer)
+
+        for case in self.cases:
+            case._resolve_snrefs(diag_layer)
 
     def __repr__(self) -> str:
         return (f"Multiplexer('{self.short_name}', " + ", ".join([
             f"odx_id='{self.odx_id}'",
             f"byte_position='{self.byte_position}'",
             f"switch_key='{self.switch_key}'",
             f"default_case='{self.default_case}'",
```

### Comparing `odxtools-3.0.2/odxtools/nameditemlist.py` & `odxtools-4.0.0/odxtools/nameditemlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 
             i += 1
             tmp = f"{item_name}_{i}"
 
     def sort(self, key=None, reverse=False):
         return self._list.sort(key=key, reverse=reverse)
 
+    def __contains__(self, x) -> bool:
+        return x in self._list
+
     def __len__(self):
         return len(self._list)
 
     def __getitem__(self, key: Union[int, str, slice]) -> T:
         if isinstance(key, int):
             if abs(key) < -len(self._list) or key >= len(self._list):
                 # we want to raise a KeyError instead of an IndexError
```

### Comparing `odxtools-3.0.2/odxtools/obd.py` & `odxtools-4.0.0/odxtools/obd.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/odxlink.py` & `odxtools-4.0.0/odxtools/odxlink.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/odxtypes.py` & `odxtools-4.0.0/odxtools/odxtypes.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameter_info.py` & `odxtools-4.0.0/odxtools/parameter_info.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameters/__init__.py` & `odxtools-4.0.0/odxtools/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameters/codedconstparameter.py` & `odxtools-4.0.0/odxtools/parameters/codedconstparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameters/createanyparameter.py` & `odxtools-4.0.0/odxtools/parameters/createanyparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameters/dynamicparameter.py` & `odxtools-4.0.0/odxtools/parameters/dynamicparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameters/lengthkeyparameter.py` & `odxtools-4.0.0/odxtools/parameters/lengthkeyparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameters/matchingrequestparameter.py` & `odxtools-4.0.0/odxtools/parameters/matchingrequestparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameters/nrcconstparameter.py` & `odxtools-4.0.0/odxtools/parameters/nrcconstparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameters/parameterbase.py` & `odxtools-4.0.0/odxtools/parameters/parameterbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 import abc
 import warnings
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 from ..decodestate import DecodeState
 from ..encodestate import EncodeState
 from ..exceptions import OdxWarning
 from ..globals import logger
-from ..odxlink import OdxLinkDatabase
+from ..odxlink import OdxLinkDatabase, OdxLinkId
 from ..specialdata import SpecialDataGroup
 
 if TYPE_CHECKING:
     from ..diaglayer import DiagLayer
 
 
 class Parameter(abc.ABC):
@@ -34,25 +34,29 @@
         self.byte_position: Optional[int] = byte_position
         self.bit_position: Optional[int] = bit_position
         self.parameter_type: str = parameter_type
         self.semantic: Optional[str] = semantic
         self.description: Optional[str] = description
         self.sdgs = sdgs
 
-    def _build_odxlinks(self):
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
         result = {}
 
         for sdg in self.sdgs:
             result.update(sdg._build_odxlinks())
 
         return result
 
-    def _resolve_references(self, parent_dl: "DiagLayer", odxlinks: OdxLinkDatabase) -> None:
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         for sdg in self.sdgs:
-            sdg._resolve_references(odxlinks)
+            sdg._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        for sdg in self.sdgs:
+            sdg._resolve_snrefs(diag_layer)
 
     @property
     def bit_length(self) -> Optional[int]:
         return None
 
     @abc.abstractmethod
     def is_required(self):
```

### Comparing `odxtools-3.0.2/odxtools/parameters/parameterwithdop.py` & `odxtools-4.0.0/odxtools/parameters/parameterwithdop.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 from ..dataobjectproperty import DataObjectProperty, DopBase, DtcDop
 from ..decodestate import DecodeState
 from ..encodestate import EncodeState
 from ..globals import logger
-from ..odxlink import OdxLinkDatabase, OdxLinkRef
+from ..odxlink import OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from ..physicaltype import PhysicalType
 from .parameterbase import Parameter
 
 if TYPE_CHECKING:
     from ..diaglayer import DiagLayer
 
 
@@ -24,39 +24,42 @@
         dop_snref: Optional[str],
         **kwargs,
     ) -> None:
         super().__init__(parameter_type=parameter_type, **kwargs)
         self.dop_ref = dop_ref
         self.dop_snref = dop_snref
 
-    @property
-    def dop(self) -> Optional[DopBase]:
-        """may be a DataObjectProperty, a Structure or None"""
+        self._dop: Optional[DopBase] = None
+        if dop_snref is None and dop_ref is None:
+            logger.warn(f"Param {self.short_name} without DOP-(SN)REF should not exist!")
 
-        return self._dop
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return super()._build_odxlinks()
 
-    def _resolve_references(self, parent_dl: "DiagLayer", odxlinks: OdxLinkDatabase) -> None:
-        super()._resolve_references(parent_dl, odxlinks)
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        super()._resolve_odxlinks(odxlinks)
 
-        self._dop: Optional[DopBase] = None
+        if self.dop_ref is not None:
+            assert self.dop_snref is None
+            # TODO: do not do lenient resolves here. The problem is
+            # that currently not all kinds of DOPs are internalized
+            # (e.g., static and dynamic fields)
+            self._dop = odxlinks.resolve_lenient(self.dop_ref)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        super()._resolve_snrefs(diag_layer)
 
         if self.dop_snref:
-            dop = parent_dl.data_object_properties.get(self.dop_snref)
-            if dop is None:
-                logger.info(f"Param {self.short_name} could not resolve DOP-SNREF {self.dop_snref}")
-            else:
-                self._dop = dop
-        elif self.dop_ref:
-            dop = odxlinks.resolve_lenient(self.dop_ref)  # TODO: non-lenient!
-            if dop is None:
-                logger.info(f"Param {self.short_name} could not resolve DOP-REF {self.dop_ref}")
-            else:
-                self._dop = dop
-        else:
-            logger.warn(f"Param {self.short_name} without DOP-(SN)REF should not exist!")
+            self._dop = diag_layer.diag_data_dictionary_spec.data_object_props[self.dop_snref]
+
+    @property
+    def dop(self) -> Optional[DopBase]:
+        """may be a DataObjectProperty, a Structure or None"""
+
+        return self._dop
 
     @property
     def bit_length(self):
         if self.dop is not None:
             return self.dop.bit_length
         else:
             return None
```

### Comparing `odxtools-3.0.2/odxtools/parameters/physicalconstantparameter.py` & `odxtools-4.0.0/odxtools/parameters/physicalconstantparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameters/reservedparameter.py` & `odxtools-4.0.0/odxtools/parameters/reservedparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameters/systemparameter.py` & `odxtools-4.0.0/odxtools/parameters/systemparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameters/tableentryparameter.py` & `odxtools-4.0.0/odxtools/parameters/tableentryparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameters/tablekeyparameter.py` & `odxtools-4.0.0/odxtools/parameters/tablekeyparameter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,72 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Dict
 
-from ..odxlink import OdxLinkDatabase
+from ..odxlink import OdxLinkDatabase, OdxLinkId
 from .parameterbase import Parameter
 
 if TYPE_CHECKING:
+    from ..table import Table, TableRow
     from .diaglayer import DiagLayer
 
 
 class TableKeyParameter(Parameter):
 
     def __init__(self, *, odx_id, table_ref, table_snref, table_row_snref, table_row_ref, **kwargs):
         super().__init__(parameter_type="TABLE-KEY", **kwargs)
         self.odx_id = odx_id
         self.table_ref = table_ref
         self.table_row_ref = table_row_ref
         self.table_snref = table_snref
         self.table_row_snref = table_row_snref
 
+        if self.table_ref is None and self.table_snref is None and \
+           self.table_row_ref is None and self.table_row_snref is None:
+            raise ValueError("Either a table or a table row must be defined.")
+
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        result = super()._build_odxlinks()
+
+        result[self.odx_id] = self
+
+        return result
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        super()._resolve_odxlinks(odxlinks)
+
+        if self.table_ref:
+            self._table = odxlinks.resolve(self.table_ref)
+        if self.table_row_ref:
+            self._table_row = odxlinks.resolve(self.table_row_ref)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        super()._resolve_snrefs(diag_layer)
+
+        if self.table_snref:
+            self._table = diag_layer.local_diag_data_dictionary_spec.tables[self.table_snref]
+        if self.table_row_snref:
+            self._table_row = diag_layer.local_diag_data_dictionary_spec.tables[
+                self.table_row_snref]
+
+    @property
+    def table(self) -> "Table":
+        return self._table
+
+    @property
+    def table_row(self) -> "TableRow":
+        return self._table_row
+
     def is_required(self):
         raise NotImplementedError("TableKeyParameter.is_required is not implemented yet.")
 
     def is_optional(self):
         raise NotImplementedError("TableKeyParameter.is_optional is not implemented yet.")
 
     def get_coded_value(self):
         raise NotImplementedError("Encoding a TableKeyParameter is not implemented yet.")
 
     def get_coded_value_as_bytes(self):
         raise NotImplementedError("Encoding a TableKeyParameter is not implemented yet.")
 
     def decode_from_pdu(self, coded_message, default_byte_position=None):
         raise NotImplementedError("Decoding a TableKeyParameter is not implemented yet.")
-
-    def _resolve_references(self, parent_dl: "DiagLayer", odxlinks: OdxLinkDatabase) -> None:
-        super()._resolve_references(parent_dl, odxlinks)
-        self.table = None
-        if self.table_snref:
-            self.table = parent_dl.local_diag_data_dictionary_spec.tables[self.table_snref]
-        if self.table_ref:
-            self.table = odxlinks.resolve(self.table_ref)
-
-        if self.table_row_ref:
-            self.table_row = odxlinks.resolve(self.table_row_ref)
-        if self.table_row_snref:
-            self.table_row = parent_dl.local_diag_data_dictionary_spec.tables[self.table_row_snref]
-
-        if self.table is None:
-            raise ValueError("Either table_key_ref or table_key_snref must be defined.")
```

### Comparing `odxtools-3.0.2/odxtools/parameters/tablestructparameter.py` & `odxtools-4.0.0/odxtools/parameters/tablestructparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/parameters/valueparameter.py` & `odxtools-4.0.0/odxtools/parameters/valueparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/physicaltype.py` & `odxtools-4.0.0/odxtools/physicaltype.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/service.py` & `odxtools-4.0.0/odxtools/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
-from typing import Iterable, List, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Union, cast
 from xml.etree import ElementTree
 
 from .admindata import AdminData
 from .audience import Audience
 from .exceptions import DecodeError
 from .functionalclass import FunctionalClass
 from .message import Message
 from .nameditemlist import NamedItemList
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from .parameters import Parameter
 from .specialdata import SpecialDataGroup, create_sdgs_from_et
 from .state import State
-from .state_transition import StateTransition
+from .statetransition import StateTransition
 from .structures import Request, Response
 from .utils import create_description_from_et, short_name_as_id
 
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
+
 
 class DiagService:
 
     def __init__(
         self,
         *,
         odx_id: OdxLinkId,
@@ -51,14 +54,15 @@
         negative_responses: List[OdxLinkRef] | List[Response]
         """
         self.odx_id: OdxLinkId = odx_id
         self.short_name: str = short_name
         self.long_name: Optional[str] = long_name
         self.description: Optional[str] = description
         self.semantic: Optional[str] = semantic
+        self.admin_data: Optional[AdminData] = admin_data
         self.audience: Optional[Audience] = audience
         self.functional_class_refs: List[OdxLinkRef] = list(functional_class_refs)
         self._functional_classes: Union[List[FunctionalClass], NamedItemList[FunctionalClass]] = []
         self.pre_condition_state_refs: List[OdxLinkRef] = list(pre_condition_state_refs)
         self._pre_condition_states: Union[List[State], NamedItemList[State]] = []
         self.state_transition_refs: List[OdxLinkRef] = list(state_transition_refs)
         self._state_transitions: Union[List[StateTransition], NamedItemList[StateTransition]] = []
@@ -214,23 +218,23 @@
     def pre_condition_states(self):
         return self._pre_condition_states
 
     @property
     def state_transitions(self):
         return self._state_transitions
 
-    def _build_odxlinks(self):
-        result = {}
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        result = {self.odx_id: self}
 
         for sdg in self.sdgs:
             result.update(sdg._build_odxlinks())
 
         return result
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         self._request = odxlinks.resolve(self.request_ref)
         self._positive_responses = NamedItemList(short_name_as_id, [
             odxlinks.resolve(pr_id) for pr_id in self.pos_res_refs
         ])
         self._negative_responses = NamedItemList(short_name_as_id, [
             odxlinks.resolve(nr_id) for nr_id in self.neg_res_refs
         ])
@@ -239,19 +243,33 @@
         ])
         self._pre_condition_states = NamedItemList(short_name_as_id, [
             odxlinks.resolve(st_id) for st_id in self.pre_condition_state_refs
         ])
         self._state_transitions = NamedItemList(short_name_as_id, [
             odxlinks.resolve(stt_id) for stt_id in self.state_transition_refs
         ])
+
+        if self.admin_data:
+            self.admin_data._resolve_odxlinks(odxlinks)
+
+        if self.audience:
+            self.audience._resolve_odxlinks(odxlinks)
+
+        for sdg in self.sdgs:
+            sdg._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        if self.admin_data:
+            self.admin_data._resolve_snrefs(diag_layer)
+
         if self.audience:
-            self.audience._resolve_references(odxlinks)
+            self.audience._resolve_snrefs(diag_layer)
 
         for sdg in self.sdgs:
-            sdg._resolve_references(odxlinks)
+            sdg._resolve_snrefs(diag_layer)
 
     def decode_message(self, message: Union[bytes, bytearray]) -> Message:
 
         # Check if message is a request or positive or negative response
         interpretable_message_types = []
 
         if (self.request is None or self.positive_responses is None or
```

### Comparing `odxtools-3.0.2/odxtools/singleecujob.py` & `odxtools-4.0.0/odxtools/singleecujob.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Literal, Optional, Union, cast
+from itertools import chain
+from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional, Union, cast
 
 from .admindata import AdminData
 from .audience import Audience
 from .dataobjectproperty import DopBase
 from .exceptions import DecodeError, EncodeError
 from .functionalclass import FunctionalClass
 from .globals import logger
 from .message import Message
 from .nameditemlist import NamedItemList
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from .odxtypes import odxstr_to_bool
 from .specialdata import SpecialDataGroup, create_sdgs_from_et
 from .utils import create_description_from_et, short_name_as_id
 
-DiagClassType = Literal["STARTCOMM", "STOPCOMM", "VARIANTIDENTIFICATION",
-                        "READ-DYN-DEFINED-MESSAGE", "DYN-DEF-MESSAGE", "CLEAR-DYN-DEF-MESSAGE",]
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
+
+DiagClassType = Literal[
+    "STARTCOMM",
+    "STOPCOMM",
+    "VARIANTIDENTIFICATION",
+    "READ-DYN-DEFINED-MESSAGE",
+    "DYN-DEF-MESSAGE",
+    "CLEAR-DYN-DEF-MESSAGE",
+]
 
 
 @dataclass
 class InputParam:
     short_name: str
     dop_base_ref: OdxLinkRef
     long_name: Optional[str]
@@ -49,17 +59,23 @@
             description=description,
             dop_base_ref=dop_base_ref,
             physical_default_value=physical_default_value,
             semantic=semantic,
             oid=oid,
         )
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         self._dop = odxlinks.resolve(self.dop_base_ref, DopBase)
 
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
     @property
     def dop(self) -> DopBase:
         """The data object property describing this parameter."""
         return self._dop
 
 
 @dataclass
@@ -96,17 +112,23 @@
             long_name=long_name,
             description=description,
             dop_base_ref=dop_base_ref,
             semantic=semantic,
             oid=oid,
         )
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         self._dop = odxlinks.resolve(self.dop_base_ref)
 
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
     @property
     def dop(self) -> Optional[DopBase]:
         """The data object property describing this parameter."""
         return self._dop
 
 
 @dataclass
@@ -132,17 +154,23 @@
         return NegOutputParam(
             short_name=short_name,
             long_name=long_name,
             description=description,
             dop_base_ref=dop_base_ref,
         )
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         self._dop = odxlinks.resolve(self.dop_base_ref)
 
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
     @property
     def dop(self) -> Optional[DopBase]:
         """The data object property describing this parameter."""
         return self._dop
 
 
 @dataclass
@@ -150,19 +178,15 @@
     """A reference to code that is executed by a single ECU job"""
 
     code_file: str
     syntax: Literal["JAVA", "CLASS", "JAR"]
     revision: str
     encryption: Optional[str]
     entrypoint: Optional[str]
-    library_refs: List[OdxLinkRef] = field(default_factory=list)
-
-    def __post_init__(self):
-        if not self.library_refs:
-            self.library_refs = []
+    library_refs: List[OdxLinkRef]
 
     @staticmethod
     def from_et(et_element, doc_frags: List[OdxDocFragment]) -> "ProgCode":
         code_file = et_element.findtext("CODE-FILE")
 
         encryption = et_element.findtext("ENCRYPTION")
 
@@ -182,17 +206,23 @@
             syntax=syntax,
             revision=revision,
             encryption=encryption,
             entrypoint=entrypoint,
             library_refs=library_refs,
         )
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         # TODO: Libraries are currently not internalized.
-        #       Once they are internalized, resolve the references `library_refs` here.
+        #       Once they are internalized, resolve the `library_refs` references here.
+        pass
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
         pass
 
 
 @dataclass
 class SingleEcuJob:
     """A single ECU job is a diagnostic communication primitive.
 
@@ -246,19 +276,19 @@
     def __post_init__(self) -> None:
         if not self.functional_class_refs:
             self.functional_class_refs = []
         self._functional_classes: Optional[NamedItemList[FunctionalClass]] = None
 
         # Replace None attributes by empty lists
         if not self.input_params:
-            self.input_params = NamedItemList(short_name_as_id, [])
+            self.input_params = NamedItemList(short_name_as_id)
         if not self.output_params:
-            self.output_params = NamedItemList(short_name_as_id, [])
+            self.output_params = NamedItemList(short_name_as_id)
         if not self.neg_output_params:
-            self.neg_output_params = NamedItemList(short_name_as_id, [])
+            self.neg_output_params = NamedItemList(short_name_as_id)
 
     @staticmethod
     def from_et(et_element, doc_frags: List[OdxDocFragment]) -> "SingleEcuJob":
 
         logger.info(f"Parsing service based on ET DiagService element: {et_element}")
         odx_id = OdxLinkId.from_et(et_element, doc_frags)
         assert odx_id is not None
@@ -329,50 +359,66 @@
     @property
     def functional_classes(self) -> Optional[NamedItemList[FunctionalClass]]:
         """The functional classes referenced by this job.
         This is None iff the references were not resolved.
         """
         return self._functional_classes
 
-    def _build_odxlinks(self):
-        result = {}
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        result = {self.odx_id: self}
+
+        for obj in chain(self.prog_codes, self.input_params, self.output_params,
+                         self.neg_output_params, self.sdgs):
+            result.update(obj._build_odxlinks())
+
+        if self.admin_data:
+            result.update(self.admin_data._build_odxlinks())
 
-        for sdg in self.sdgs:
-            result.update(sdg._build_odxlinks())
+        if self.audience:
+            result.update(self.audience._build_odxlinks())
 
         return result
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        for code in self.prog_codes:
+            code._resolve_odxlinks(odxlinks)
+
         # Resolve references to functional classes
         self._functional_classes = NamedItemList[FunctionalClass](short_name_as_id, [])
         for fc_ref in self.functional_class_refs:
             fc = odxlinks.resolve(fc_ref)
             if isinstance(fc, FunctionalClass):
                 self._functional_classes.append(fc)
             else:
                 logger.warning(f"Functional class ID {fc_ref!r} resolved to {fc!r}.")
 
+        for obj in chain(self.prog_codes, self.input_params, self.output_params,
+                         self.neg_output_params, self.sdgs):
+            obj._resolve_odxlinks(odxlinks)
+
+        # Resolve references of admin data
+        if self.admin_data:
+            self.admin_data._resolve_odxlinks(odxlinks)
+
         # Resolve references of audience
         if self.audience:
-            self.audience._resolve_references(odxlinks)
-
-        # Resolve references of params
-        params: List[Union[InputParam, OutputParam, NegOutputParam]] = [
-            *self.input_params,
-            *self.output_params,
-            *self.neg_output_params,
-        ]
-        for p in params:
-            p._resolve_references(odxlinks)
+            self.audience._resolve_odxlinks(odxlinks)
 
-        for code in self.prog_codes:
-            code._resolve_references(odxlinks)
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        for obj in chain(self.prog_codes, self.input_params, self.output_params,
+                         self.neg_output_params, self.sdgs):
+            obj._resolve_snrefs(diag_layer)
+
+        # Resolve references of admin data
+        if self.admin_data:
+            self.admin_data._resolve_snrefs(diag_layer)
 
-        for sdg in self.sdgs:
-            sdg._resolve_references(odxlinks)
+        # Resolve references of audience
+        if self.audience:
+            self.audience._resolve_snrefs(diag_layer)
 
     def decode_message(self, message: Union[bytes, bytearray]) -> Message:
         """This function's signature matches `DiagService.decode_message`
         and only raises an informative error.
         """
         raise DecodeError(
             f"Single ECU jobs are completely executed on the tester and thus cannot be decoded."
```

### Comparing `odxtools-3.0.2/odxtools/specialdata.py` & `odxtools-4.0.0/odxtools/specialdata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 import warnings
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 from xml.etree import ElementTree
 
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from .utils import create_description_from_et, short_name_as_id
 
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
+
 
 @dataclass
 class SpecialDataGroupCaption:
     odx_id: OdxLinkId
     short_name: str
     long_name: Optional[str]
     description: Optional[str]
@@ -27,31 +30,40 @@
         long_name = et_element.findtext("LONG-NAME")
         description = create_description_from_et(et_element.find("DESC"))
 
         return SpecialDataGroupCaption(
             odx_id=odx_id, short_name=short_name, long_name=long_name, description=description)
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
-        result = {}
+        result = {self.odx_id: self}
 
         result[self.odx_id] = self
 
         return result
 
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        pass
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
 
 @dataclass
 class SpecialData:
     semantic_info: Optional[str]  # the "SI" attribute
     text_identifier: Optional[str]  # the "TI" attribute, specifies the language used
     value: str
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
         return {}
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        pass
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
         pass
 
     @staticmethod
     def from_et(et_element: ElementTree.Element, doc_frags: List[OdxDocFragment]) -> "SpecialData":
         semantic_info = et_element.get("SI")
         text_identifier = et_element.get("TI")
         value = et_element.text or ""
@@ -106,22 +118,33 @@
             result.update(self.sdg_caption._build_odxlinks())
 
         for val in self.values:
             result.update(val._build_odxlinks())
 
         return result
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         if self.sdg_caption_ref is not None:
-            caption = odxlinks.resolve(self.sdg_caption_ref)
-            assert isinstance(caption, SpecialDataGroupCaption)
-            self.sdg_caption = caption
+            self.sdg_caption = odxlinks.resolve(self.sdg_caption_ref, SpecialDataGroupCaption)
+        elif self.sdg_caption is not None:
+            # resolve the ODXLINK references of the caption, but only
+            # if the caption was specified by value, not by reference
+            self.sdg_caption._resolve_odxlinks(odxlinks)
+
+        for val in self.values:
+            val._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        # resolve the SNREFs of the caption, but only if the caption
+        # was specified by value, not by reference
+        if self.sdg_caption is not None and self.sdg_caption_ref is None:
+            self.sdg_caption._resolve_snrefs(diag_layer)
 
         for val in self.values:
-            val._resolve_references(odxlinks)
+            val._resolve_snrefs(diag_layer)
 
 
 def create_sdgs_from_et(et_element: Optional[ElementTree.Element],
                         doc_frags: List[OdxDocFragment]) -> List[SpecialDataGroup]:
 
     if not et_element:
         return []
```

### Comparing `odxtools-3.0.2/odxtools/state.py` & `odxtools-4.0.0/odxtools/state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId
 from .utils import create_description_from_et
 
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
+
 
 @dataclass
 class State:
     """
     Corresponds to STATE.
     """
 
@@ -29,9 +32,12 @@
 
         return State(
             odx_id=odx_id, short_name=short_name, long_name=long_name, description=description)
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
         return {self.odx_id: self}
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        pass
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
         pass
```

### Comparing `odxtools-3.0.2/odxtools/structures.py` & `odxtools-4.0.0/odxtools/structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -297,26 +297,32 @@
             isinstance(struct_param.dop, BasicStructure)
         })
         return param_dict
 
     def _build_odxlinks(self):
         result = super()._build_odxlinks()
 
-        for param in self.parameters:
-            result.update(param._build_odxlinks())
+        for p in self.parameters:
+            result.update(p._build_odxlinks())
 
         return result
 
-    def _resolve_references(  # type: ignore[override]
-            self, parent_dl: "DiagLayer", odxlinks: OdxLinkDatabase) -> None:
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        """Recursively resolve any references (odxlinks or sn-refs)"""
+        super()._resolve_odxlinks(odxlinks)
+
+        for p in self.parameters:
+            p._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
         """Recursively resolve any references (odxlinks or sn-refs)"""
-        super()._resolve_references(odxlinks)
+        super()._resolve_snrefs(diag_layer)
 
         for p in self.parameters:
-            p._resolve_references(parent_dl, odxlinks)
+            p._resolve_snrefs(diag_layer)
 
     def __message_format_lines(self, allow_unknown_lengths: bool = False) -> List[str]:
         # sort parameters
         sorted_params: list = list(self.parameters)  # copy list
 
         def param_sort_key(param: Union[Parameter, "EndOfPduField"]) -> Tuple[int, int]:
             if not isinstance(param, Parameter):
@@ -497,16 +503,16 @@
 
     def __init__(self, *, response_type: str, **kwargs):  # "POS-RESPONSE" or "NEG-RESPONSE"
         super().__init__(**kwargs)
 
         self.response_type = response_type
 
     def encode(self, coded_request: Optional[ByteString] = None, **params) -> ByteString:
-        logger.info(f"Compose response message to the request {coded_request}")
         if coded_request is not None:
+            logger.info(f"Compose response message to the request {coded_request.hex()}")
             # Extract MATCHING-REQUEST-PARAMs from the coded request
             for param in self.parameters:
                 if param.parameter_type == "MATCHING-REQUEST-PARAM":
                     logger.info(f"set matching request param value {param.short_name}")
                     byte_pos = param.request_byte_position
                     byte_length = param.byte_length
 
@@ -543,15 +549,15 @@
             long_name=long_name,
             description=description,
             is_visible_raw=None,
             parameters=parameters,
             byte_size=None,
             sdgs=sdgs,
         )
-    elif et_element.tag in ["POS-RESPONSE", "NEG-RESPONSE"]:
+    elif et_element.tag in ["POS-RESPONSE", "NEG-RESPONSE", "GLOBAL-NEG-RESPONSE"]:
         res = Response(
             odx_id=odx_id,
             short_name=short_name,
             response_type=et_element.tag,
             long_name=long_name,
             description=description,
             is_visible_raw=None,
```

### Comparing `odxtools-3.0.2/odxtools/table.py` & `odxtools-4.0.0/odxtools/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 import abc
 from dataclasses import dataclass, field
-from typing import Any, Dict, Iterable, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional
 
 from .dataobjectproperty import DopBase
 from .globals import logger
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from .specialdata import SpecialDataGroup, create_sdgs_from_et
 from .utils import create_description_from_et
 
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
+
 
 class TableBase(abc.ABC):
     """Base class for all Tables."""
 
     def __init__(
         self,
         *,
@@ -24,24 +27,28 @@
     ):
         self.odx_id = odx_id
         self.short_name = short_name
         self.long_name = long_name
         self.sdgs = sdgs
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
-        result = {}
+        result = {self.odx_id: self}
 
         for sdg in self.sdgs:
             result.update(sdg._build_odxlinks())
 
         return result
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        for sdg in self.sdgs:
+            sdg._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
         for sdg in self.sdgs:
-            sdg._resolve_references(odxlinks)
+            sdg._resolve_snrefs(diag_layer)
 
 
 @dataclass
 class TableRow:
     """This class represents a TABLE-ROW."""
 
     odx_id: OdxLinkId
@@ -86,31 +93,33 @@
             key=key,
             structure_ref=structure_ref,
             dop_ref=dop_ref,
             sdgs=sdgs,
         )
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
-        result = {}
-
-        result[self.odx_id] = self
+        result = {self.odx_id: self}
 
         for sdg in self.sdgs:
             result.update(sdg._build_odxlinks())
 
         return result
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         if self.structure_ref is not None:
             self._structure = odxlinks.resolve(self.structure_ref)
         if self.dop_ref is not None:
             self._dop = odxlinks.resolve(self.dop_ref)
 
         for sdg in self.sdgs:
-            sdg._resolve_references(odxlinks)
+            sdg._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        for sdg in self.sdgs:
+            sdg._resolve_snrefs(diag_layer)
 
     @property
     def structure(self) -> Optional[DopBase]:
         """The structure associated with this table row."""
         return self._structure
 
     @property
@@ -146,15 +155,15 @@
             odx_id=odx_id,
             short_name=short_name,
             long_name=long_name,
             sdgs=sdgs,
         )
         self._local_table_rows = table_rows
         self._ref_table_rows: List[TableRow] = []
-        self._table_row_refs = table_row_refs or []
+        self._table_row_refs = table_row_refs
         self.key_dop_ref = key_dop_ref
         self._key_dop = None
         self.description = description
         self.semantic = semantic
 
     @staticmethod
     def from_et(et_element, doc_frags: List[OdxDocFragment]) -> "Table":
@@ -208,25 +217,31 @@
         result = super()._build_odxlinks()
 
         for tr in self._local_table_rows:
             result.update(tr._build_odxlinks())
 
         return result
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
-        super()._resolve_references(odxlinks)
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        super()._resolve_odxlinks(odxlinks)
 
         if self.key_dop_ref is not None:
             self._key_dop = odxlinks.resolve(self.key_dop_ref)
 
         for table_row in self._local_table_rows:
-            table_row._resolve_references(odxlinks)
+            table_row._resolve_odxlinks(odxlinks)
 
         self._ref_table_rows = []
         for ref in self._table_row_refs:
             tr = odxlinks.resolve(ref)
             assert isinstance(tr, TableRow)
             self._ref_table_rows.append(tr)
 
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        super()._resolve_snrefs(diag_layer)
+
+        for table_row in self._local_table_rows:
+            table_row._resolve_snrefs(diag_layer)
+
     def __repr__(self) -> str:
         return (f"Table('{self.short_name}', " + ", ".join(
             [f"table_rows='{self.table_rows}'", f"key_dop_ref='{self.key_dop_ref}'"]) + ")")
```

### Comparing `odxtools-3.0.2/odxtools/uds.py` & `odxtools-4.0.0/odxtools/uds.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/units.py` & `odxtools-4.0.0/odxtools/units.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022 MBition GmbH
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Literal, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional, Union
 
 from .nameditemlist import NamedItemList
 from .odxlink import OdxDocFragment, OdxLinkDatabase, OdxLinkId, OdxLinkRef
 from .specialdata import SpecialDataGroup, create_sdgs_from_et
 from .utils import create_description_from_et, short_name_as_id
 
+if TYPE_CHECKING:
+    from .diaglayer import DiagLayer
+
 UnitGroupCategory = Literal["COUNTRY", "EQUIV-UNITS"]
 
 
 @dataclass
 class PhysicalDimension:
     """A physical dimension is a formal definition of a unit.
 
@@ -63,16 +66,16 @@
         assert odx_id is not None
         oid = et_element.get("OID")
         short_name = et_element.findtext("SHORT-NAME")
         long_name = et_element.findtext("LONG-NAME")
         description = create_description_from_et(et_element.find("DESC"))
 
         def read_optional_int(element, name):
-            if element.findtext(name):
-                return int(element.findtext(name))
+            if val_str := element.findtext(name):
+                return int(val_str)
             else:
                 return 0
 
         length_exp = read_optional_int(et_element, "LENGTH-EXP")
         mass_exp = read_optional_int(et_element, "MASS-EXP")
         time_exp = read_optional_int(et_element, "TIME-EXP")
         current_exp = read_optional_int(et_element, "CURRENT-EXP")
@@ -91,14 +94,23 @@
             time_exp=time_exp,
             current_exp=current_exp,
             temperature_exp=temperature_exp,
             molar_amount_exp=molar_amount_exp,
             luminous_intensity_exp=luminous_intensity_exp,
         )
 
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {self.odx_id: self}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        pass
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
 
 @dataclass
 class Unit:
     """
     A unit consists of an ID, short name and a display name.
 
     Additionally, a unit may reference an SI unit (`.physical_dimension`)
@@ -184,22 +196,28 @@
             physical_dimension_ref=physical_dimension_ref,
         )
 
     @property
     def physical_dimension(self) -> PhysicalDimension:
         return self._physical_dimension
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase) -> None:
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {self.odx_id: self}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         if self.physical_dimension_ref:
             self._physical_dimension = odxlinks.resolve(self.physical_dimension_ref)
 
             assert isinstance(self._physical_dimension, PhysicalDimension), (
                 f"The physical_dimension_ref must be resolved to a PhysicalDimension."
                 f" {self.physical_dimension_ref} referenced {self._physical_dimension}")
 
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
 
 @dataclass
 class UnitGroup:
     """A group of units.
 
     There are two categories of groups: COUNTRY and EQUIV-UNITS.
     """
@@ -237,18 +255,24 @@
             category=category,
             unit_refs=unit_refs,
             oid=oid,
             long_name=long_name,
             description=description,
         )
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
+    def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
+        return {}
+
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
         self._units = NamedItemList[Unit](short_name_as_id,
                                           [odxlinks.resolve(ref) for ref in self.unit_refs])
 
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
+        pass
+
     @property
     def units(self) -> NamedItemList[Unit]:
         return self._units
 
 
 @dataclass
 class UnitSpec:
@@ -289,23 +313,32 @@
         return UnitSpec(
             unit_groups=unit_groups,
             units=units,
             physical_dimensions=physical_dimensions,
             sdgs=sdgs)
 
     def _build_odxlinks(self) -> Dict[OdxLinkId, Any]:
-        odxlinks = {}
-        odxlinks.update({unit.odx_id: unit for unit in self.units})
-        odxlinks.update({dim.odx_id: dim for dim in self.physical_dimensions})
-
+        odxlinks: Dict[OdxLinkId, Any] = {}
+        for unit in self.units:
+            odxlinks.update(unit._build_odxlinks())
+        for dim in self.physical_dimensions:
+            odxlinks.update(dim._build_odxlinks())
         for sdg in self.sdgs:
             odxlinks.update(sdg._build_odxlinks())
 
         return odxlinks
 
-    def _resolve_references(self, odxlinks: OdxLinkDatabase):
+    def _resolve_odxlinks(self, odxlinks: OdxLinkDatabase) -> None:
+        for unit in self.units:
+            unit._resolve_odxlinks(odxlinks)
+        for group in self.unit_groups:
+            group._resolve_odxlinks(odxlinks)
+        for sdg in self.sdgs:
+            sdg._resolve_odxlinks(odxlinks)
+
+    def _resolve_snrefs(self, diag_layer: "DiagLayer") -> None:
         for unit in self.units:
-            unit._resolve_references(odxlinks)
+            unit._resolve_snrefs(diag_layer)
         for group in self.unit_groups:
-            group._resolve_references(odxlinks)
+            group._resolve_snrefs(diag_layer)
         for sdg in self.sdgs:
-            sdg._resolve_references(odxlinks)
+            sdg._resolve_snrefs(diag_layer)
```

### Comparing `odxtools-3.0.2/odxtools/utils.py` & `odxtools-4.0.0/odxtools/utils.py`

 * *Files identical despite different names*

### Comparing `odxtools-3.0.2/odxtools/write_pdx_file.py` & `odxtools-4.0.0/odxtools/write_pdx_file.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 import zipfile
 from typing import Any, Dict, List, Optional, Tuple
 
 import jinja2
 
 import odxtools
 
-from .comparam_subset import BaseComparam, Comparam, ComplexComparam
-from .exceptions import OdxError
 from .odxtypes import bool_to_odxstr
 
 odxdatabase = None
 
 
 def jinja2_odxraise_helper(msg: str) -> None:
     raise Exception(msg)
```

### Comparing `odxtools-3.0.2/odxtools.egg-info/PKG-INFO` & `odxtools-4.0.0/odxtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odxtools
-Version: 3.0.2
+Version: 4.0.0
 Summary: Utilities to work with the automotive diagnostics standard ODX.
 Home-page: https://github.com/Daimler/odxtools
 Author: Katrin Bauer, Andreas Lauser
 Author-email: katrin.b.bauer@mbition.io, andreas.lauser@mbition.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Daimler/odxtools/issues
 Keywords: can,can bus,odx,pdx,obd,uds,automotive,diagnostics
```

### Comparing `odxtools-3.0.2/odxtools.egg-info/SOURCES.txt` & `odxtools-4.0.0/odxtools.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 odxtools/comparam_subset.py
 odxtools/database.py
 odxtools/dataobjectproperty.py
 odxtools/decodestate.py
 odxtools/diagcodedtypes.py
 odxtools/diagdatadictionaryspec.py
 odxtools/diaglayer.py
+odxtools/diaglayercontainer.py
+odxtools/diaglayerraw.py
 odxtools/diaglayertype.py
 odxtools/ecu_variant_matcher.py
 odxtools/ecu_variant_patterns.py
 odxtools/encodestate.py
 odxtools/endofpdufield.py
 odxtools/envdata.py
 odxtools/envdatadesc.py
@@ -38,20 +40,22 @@
 odxtools/message.py
 odxtools/multiplexer.py
 odxtools/nameditemlist.py
 odxtools/obd.py
 odxtools/odxlink.py
 odxtools/odxtypes.py
 odxtools/parameter_info.py
+odxtools/parentref.py
 odxtools/physicaltype.py
 odxtools/service.py
 odxtools/singleecujob.py
 odxtools/specialdata.py
 odxtools/state.py
-odxtools/state_transition.py
+odxtools/statechart.py
+odxtools/statetransition.py
 odxtools/structures.py
 odxtools/table.py
 odxtools/uds.py
 odxtools/units.py
 odxtools/utils.py
 odxtools/version.py
 odxtools/write_pdx_file.py
@@ -92,8 +96,22 @@
 odxtools/parameters/parameterwithdop.py
 odxtools/parameters/physicalconstantparameter.py
 odxtools/parameters/reservedparameter.py
 odxtools/parameters/systemparameter.py
 odxtools/parameters/tableentryparameter.py
 odxtools/parameters/tablekeyparameter.py
 odxtools/parameters/tablestructparameter.py
-odxtools/parameters/valueparameter.py
+odxtools/parameters/valueparameter.py
+tests/test_compu_methods.py
+tests/test_decoding.py
+tests/test_diag_coded_types.py
+tests/test_diag_data_dictionary_spec.py
+tests/test_ecu_variant_matching.py
+tests/test_ecu_variant_patterns.py
+tests/test_encoding.py
+tests/test_odxtools.py
+tests/test_odxtypes.py
+tests/test_readparameters.py
+tests/test_singleecujob.py
+tests/test_somersault.py
+tests/test_unit_spec.py
+tests/test_utils.py
```

### Comparing `odxtools-3.0.2/setup.py` & `odxtools-4.0.0/setup.py`

 * *Files identical despite different names*

