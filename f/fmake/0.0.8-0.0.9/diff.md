# Comparing `tmp/fmake-0.0.8.tar.gz` & `tmp/fmake-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmake-0.0.8.tar", last modified: Sat Jan 21 00:11:18 2023, max compression
+gzip compressed data, was "fmake-0.0.9.tar", last modified: Sun Mar 12 23:44:06 2023, max compression
```

## Comparing `fmake-0.0.8.tar` & `fmake-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-01-21 00:11:18.713071 fmake-0.0.8/
--rw-rw-rw-   0        0        0      404 2023-01-21 00:11:18.709063 fmake-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-11-30 21:12:37.000000 fmake-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-21 00:11:18.665125 fmake-0.0.8/fmake.egg-info/
--rw-rw-rw-   0        0        0      404 2023-01-21 00:11:18.000000 fmake-0.0.8/fmake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1361 2023-01-21 00:11:18.000000 fmake-0.0.8/fmake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-21 00:11:18.000000 fmake-0.0.8/fmake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-01-21 00:11:18.000000 fmake-0.0.8/fmake.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-01-21 00:11:18.000000 fmake-0.0.8/fmake.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-01-21 00:11:18.000000 fmake-0.0.8/fmake.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-21 00:11:18.714058 fmake-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      884 2023-01-21 00:11:01.000000 fmake-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-21 00:11:18.700061 fmake-0.0.8/vhdl_build_system/
--rw-rw-rw-   0        0        0     1769 2022-12-08 22:16:53.000000 fmake-0.0.8/vhdl_build_system/Convert2CSV.py
--rw-rw-rw-   0        0        0      396 2022-12-21 04:23:01.000000 fmake-0.0.8/vhdl_build_system/__init__.py
--rw-rw-rw-   0        0        0     8651 2023-01-07 02:07:24.000000 fmake-0.0.8/vhdl_build_system/entity_to_data_frame.py
--rw-rw-rw-   0        0        0     1774 2022-12-18 02:31:41.000000 fmake-0.0.8/vhdl_build_system/extract_files.py
--rw-rw-rw-   0        0        0     5856 2022-12-13 03:02:54.000000 fmake-0.0.8/vhdl_build_system/generic_helper.py
--rw-rw-rw-   0        0        0      541 2022-12-08 09:30:24.000000 fmake-0.0.8/vhdl_build_system/main_vhdl_make.py
--rw-rw-rw-   0        0        0     1128 2022-12-12 02:08:58.000000 fmake-0.0.8/vhdl_build_system/make_build_system.py
--rw-rw-rw-   0        0        0     3887 2022-12-23 00:05:14.000000 fmake-0.0.8/vhdl_build_system/make_test_bench_stimulus.py
--rw-rw-rw-   0        0        0     3578 2023-01-21 00:10:53.000000 fmake-0.0.8/vhdl_build_system/run_ise.py
-drwxrwxrwx   0        0        0        0 2023-01-21 00:11:18.708064 fmake-0.0.8/vhdl_build_system/vhdl_csv_io/
--rw-rw-rw-   0        0        0     4814 2022-12-11 05:02:08.000000 fmake-0.0.8/vhdl_build_system/vhdl_csv_io/CSV_UtilityPkg.py
--rw-rw-rw-   0        0        0      447 2022-12-11 05:01:54.000000 fmake-0.0.8/vhdl_build_system/vhdl_csv_io/ClockGenerator.py
--rw-rw-rw-   0        0        0      389 2022-12-11 05:04:03.000000 fmake-0.0.8/vhdl_build_system/vhdl_csv_io/__init__.py
--rw-rw-rw-   0        0        0     1134 2022-12-11 05:02:29.000000 fmake-0.0.8/vhdl_build_system/vhdl_csv_io/e_csv_read_file.py
--rw-rw-rw-   0        0        0     1641 2022-12-11 09:43:08.000000 fmake-0.0.8/vhdl_build_system/vhdl_csv_io/e_csv_write_file.py
--rw-rw-rw-   0        0        0     6973 2022-12-11 05:03:51.000000 fmake-0.0.8/vhdl_build_system/vhdl_csv_io/type_conversions_helper.py
--rw-rw-rw-   0        0        0     5331 2022-12-07 03:05:28.000000 fmake-0.0.8/vhdl_build_system/vhdl_dependency_db.py
--rw-rw-rw-   0        0        0     6328 2022-12-07 03:20:21.000000 fmake-0.0.8/vhdl_build_system/vhdl_entity_class.py
--rw-rw-rw-   0        0        0     3203 2022-11-16 15:43:22.000000 fmake-0.0.8/vhdl_build_system/vhdl_get_entity_def.py
--rw-rw-rw-   0        0        0     1003 2022-12-01 03:36:23.000000 fmake-0.0.8/vhdl_build_system/vhdl_get_list_of_files.py
--rw-rw-rw-   0        0        0     3129 2022-12-08 05:10:41.000000 fmake-0.0.8/vhdl_build_system/vhdl_get_type_def.py
--rw-rw-rw-   0        0        0      799 2022-11-16 15:43:22.000000 fmake-0.0.8/vhdl_build_system/vhdl_load_file_without_comments.py
--rw-rw-rw-   0        0        0     1881 2022-12-10 01:58:51.000000 fmake-0.0.8/vhdl_build_system/vhdl_make_simulation.py
--rw-rw-rw-   0        0        0    14142 2022-12-22 21:41:18.000000 fmake-0.0.8/vhdl_build_system/vhdl_make_test_bench.py
--rw-rw-rw-   0        0        0     1113 2022-11-16 15:43:22.000000 fmake-0.0.8/vhdl_build_system/vhdl_make_test_bench_names.py
--rw-rw-rw-   0        0        0     3199 2022-12-11 04:55:06.000000 fmake-0.0.8/vhdl_build_system/vhdl_merge_split_test_cases.py
--rw-rw-rw-   0        0        0     7906 2023-01-03 07:28:20.000000 fmake-0.0.8/vhdl_build_system/vhdl_parser.py
--rw-rw-rw-   0        0        0      451 2022-12-07 23:12:58.000000 fmake-0.0.8/vhdl_build_system/vhdl_programm_list.py
--rw-rw-rw-   0        0        0     2646 2023-01-19 00:26:43.000000 fmake-0.0.8/vhdl_build_system/vhdl_run_vivado.py
+drwxrwxrwx   0        0        0        0 2023-03-12 23:44:06.848583 fmake-0.0.9/
+-rw-rw-rw-   0        0        0      404 2023-03-12 23:44:06.847585 fmake-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-11-30 21:12:37.000000 fmake-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-12 23:44:06.803060 fmake-0.0.9/fmake/
+-rw-rw-rw-   0        0        0     1745 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/Convert2CSV.py
+-rw-rw-rw-   0        0        0      288 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/__init__.py
+-rw-rw-rw-   0        0        0     8603 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/entity_to_data_frame.py
+-rw-rw-rw-   0        0        0     1750 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/extract_files.py
+-rw-rw-rw-   0        0        0     5856 2022-12-13 03:02:54.000000 fmake-0.0.9/fmake/generic_helper.py
+-rw-rw-rw-   0        0        0      529 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/main_vhdl_make.py
+-rw-rw-rw-   0        0        0     1092 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/make_build_system.py
+-rw-rw-rw-   0        0        0     3815 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/make_test_bench_stimulus.py
+-rw-rw-rw-   0        0        0     3587 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/run_ise.py
+-rw-rw-rw-   0        0        0     7687 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/send_axi_stream_udp.py
+drwxrwxrwx   0        0        0        0 2023-03-12 23:44:06.843582 fmake-0.0.9/fmake/vhdl_csv_io/
+-rw-rw-rw-   0        0        0     4814 2022-12-11 05:02:08.000000 fmake-0.0.9/fmake/vhdl_csv_io/CSV_UtilityPkg.py
+-rw-rw-rw-   0        0        0      447 2022-12-11 05:01:54.000000 fmake-0.0.9/fmake/vhdl_csv_io/ClockGenerator.py
+-rw-rw-rw-   0        0        0      329 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/vhdl_csv_io/__init__.py
+-rw-rw-rw-   0        0        0     1134 2022-12-11 05:02:29.000000 fmake-0.0.9/fmake/vhdl_csv_io/e_csv_read_file.py
+-rw-rw-rw-   0        0        0     1641 2022-12-11 09:43:08.000000 fmake-0.0.9/fmake/vhdl_csv_io/e_csv_write_file.py
+-rw-rw-rw-   0        0        0     6973 2022-12-11 05:03:51.000000 fmake-0.0.9/fmake/vhdl_csv_io/type_conversions_helper.py
+-rw-rw-rw-   0        0        0     5331 2022-12-07 03:05:28.000000 fmake-0.0.9/fmake/vhdl_dependency_db.py
+-rw-rw-rw-   0        0        0     6328 2022-12-07 03:20:21.000000 fmake-0.0.9/fmake/vhdl_entity_class.py
+-rw-rw-rw-   0        0        0     3203 2022-11-16 15:43:22.000000 fmake-0.0.9/fmake/vhdl_get_entity_def.py
+-rw-rw-rw-   0        0        0     1003 2022-12-01 03:36:23.000000 fmake-0.0.9/fmake/vhdl_get_list_of_files.py
+-rw-rw-rw-   0        0        0     3129 2022-12-08 05:10:41.000000 fmake-0.0.9/fmake/vhdl_get_type_def.py
+-rw-rw-rw-   0        0        0      799 2022-11-16 15:43:22.000000 fmake-0.0.9/fmake/vhdl_load_file_without_comments.py
+-rw-rw-rw-   0        0        0     1833 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/vhdl_make_simulation.py
+-rw-rw-rw-   0        0        0    14058 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/vhdl_make_test_bench.py
+-rw-rw-rw-   0        0        0     1113 2022-11-16 15:43:22.000000 fmake-0.0.9/fmake/vhdl_make_test_bench_names.py
+-rw-rw-rw-   0        0        0     3187 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/vhdl_merge_split_test_cases.py
+-rw-rw-rw-   0        0        0     7906 2023-01-03 07:28:20.000000 fmake-0.0.9/fmake/vhdl_parser.py
+-rw-rw-rw-   0        0        0      451 2022-12-07 23:12:58.000000 fmake-0.0.9/fmake/vhdl_programm_list.py
+-rw-rw-rw-   0        0        0     2598 2023-03-12 23:40:03.000000 fmake-0.0.9/fmake/vhdl_run_vivado.py
+drwxrwxrwx   0        0        0        0 2023-03-12 23:44:06.830062 fmake-0.0.9/fmake.egg-info/
+-rw-rw-rw-   0        0        0      404 2023-03-12 23:44:06.000000 fmake-0.0.9/fmake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2023-03-12 23:44:06.000000 fmake-0.0.9/fmake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-12 23:44:06.000000 fmake-0.0.9/fmake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-03-12 23:44:06.000000 fmake-0.0.9/fmake.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-03-12 23:44:06.000000 fmake-0.0.9/fmake.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-03-12 23:44:06.000000 fmake-0.0.9/fmake.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-12 23:44:06.849582 fmake-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      872 2023-03-12 23:43:33.000000 fmake-0.0.9/setup.py
```

### Comparing `fmake-0.0.8/setup.py` & `fmake-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fmake", 
-    version="0.0.8",
+    version="0.0.9",
     author="Richard Peschke",
     author_email="peschke@hawaii.edu",
     description="build scripts for firmware projects",
     long_description="long_description",
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
@@ -25,10 +25,10 @@
           'wget',
           'openpyxl',
           'uproot'
     ],
     python_requires='>=3.8',
     
     entry_points = {
-        'console_scripts': ['fmake=vhdl_build_system.main_vhdl_make:main_vhdl_make'],
+        'console_scripts': ['fmake=fmake.main_vhdl_make:main_vhdl_make'],
     }
 )
```

### Comparing `fmake-0.0.8/vhdl_build_system/Convert2CSV.py` & `fmake-0.0.9/fmake/Convert2CSV.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 
 from shutil import copyfile
 import pandas as pd
 
 
 import argparse
-from vhdl_build_system.vhdl_programm_list import add_programm
-from vhdl_build_system.generic_helper import  extract_cl_arguments
+from fmake.vhdl_programm_list import add_programm
+from fmake.generic_helper import  extract_cl_arguments
 
 
 def Convert2CSV(XlsFile,Sheet,OutputFile,drop):
     if XlsFile == "":
         return 
     data_xls = pd.read_excel(XlsFile, Sheet, index_col=None)
     print(data_xls.columns)
```

### Comparing `fmake-0.0.8/vhdl_build_system/entity_to_data_frame.py` & `fmake-0.0.9/fmake/entity_to_data_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 import pandas as pd
 import copy
 
 
-from vhdl_build_system.vhdl_load_file_without_comments import load_file_witout_comments
-from vhdl_build_system.generic_helper import get_text_between_outtermost
-from  vhdl_build_system.vhdl_entity_class            import vhdl_entity
-from vhdl_build_system.vhdl_parser import vhdl_parser ,parse_get_top_level_candidates
+from fmake.vhdl_load_file_without_comments import load_file_witout_comments
+from fmake.generic_helper import get_text_between_outtermost
+from  fmake.vhdl_entity_class            import vhdl_entity
+from fmake.vhdl_parser import vhdl_parser ,parse_get_top_level_candidates
 
 
 import dataframe_helpers as dfh
 
 def get_ports(filename):
     entetyCl  =  vhdl_entity(filename)
     df = entetyCl.ports()
```

### Comparing `fmake-0.0.8/vhdl_build_system/extract_files.py` & `fmake-0.0.9/fmake/extract_files.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import zipfile
 
 import shutil
 import os
-from  vhdl_build_system.vhdl_programm_list           import add_programm 
-from  vhdl_build_system.generic_helper               import  vprint, extract_cl_arguments
+from  fmake.vhdl_programm_list           import add_programm 
+from  fmake.generic_helper               import  vprint, extract_cl_arguments
 import argparse
 
 build_folder = "build/"
 
 def extract_bitfiles(in_zip_file, ouput_path = None):
     basename = os.path.basename(in_zip_file) 
     out_folder = build_folder+basename+"/zip/"
```

### Comparing `fmake-0.0.8/vhdl_build_system/generic_helper.py` & `fmake-0.0.9/fmake/generic_helper.py`

 * *Files identical despite different names*

### Comparing `fmake-0.0.8/vhdl_build_system/main_vhdl_make.py` & `fmake-0.0.9/fmake/main_vhdl_make.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from vhdl_build_system.vhdl_programm_list import get_function,  print_list_of_programs
+from fmake.vhdl_programm_list import get_function,  print_list_of_programs
 
     
     
 def main_vhdl_make():
     if len(sys.argv) < 2:
         print("not enough arguments")
         print("use one of these programms:")
```

### Comparing `fmake-0.0.8/vhdl_build_system/make_build_system.py` & `fmake-0.0.9/fmake/make_build_system.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from vhdl_build_system.vhdl_programm_list import add_programm
-from vhdl_build_system.generic_helper import  extract_cl_arguments, try_make_dir, save_file
+from fmake.vhdl_programm_list import add_programm
+from fmake.generic_helper import  extract_cl_arguments, try_make_dir, save_file
 import argparse
 
-import vhdl_build_system.vhdl_csv_io as csv_io
+import fmake.vhdl_csv_io as csv_io
 
 
 def make_build_wrap(x):
     parser = argparse.ArgumentParser(description='Excel To CSV Converter')
     args = extract_cl_arguments(parser , x)
     try_make_dir("build")
     save_file("build/fmake.txt",  "")
```

### Comparing `fmake-0.0.8/vhdl_build_system/make_test_bench_stimulus.py` & `fmake-0.0.9/fmake/make_test_bench_stimulus.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pandas as pd
 import numpy as np
 import uproot
 import argparse
 
-from vhdl_build_system.vhdl_programm_list import add_programm
-import vhdl_build_system.vhdl_load_file_without_comments as ld
-from vhdl_build_system.vhdl_dependency_db import  get_dependency_db
+from fmake.vhdl_programm_list import add_programm
+import fmake.vhdl_load_file_without_comments as ld
+from fmake.vhdl_dependency_db import  get_dependency_db
 
-from  vhdl_build_system.generic_helper               import save_file, try_make_dir, cl_add_entity, join_str
-from  vhdl_build_system.vhdl_programm_list           import add_programm 
-from  vhdl_build_system.generic_helper               import  vprint, extract_cl_arguments
+from  fmake.generic_helper               import save_file, try_make_dir, cl_add_entity, join_str
+from  fmake.vhdl_programm_list           import add_programm 
+from  fmake.generic_helper               import  vprint, extract_cl_arguments
 
 
 
 def append_dataframe(df, df_append):
     df_append = df_append[[x for x in df_append.columns if x in df.columns]]
     df = pd.concat( [df, df_append] )
```

### Comparing `fmake-0.0.8/vhdl_build_system/run_ise.py` & `fmake-0.0.9/fmake/run_ise.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import argparse
 import os
 import shutil 
 import platform
 
-from vhdl_build_system.vhdl_programm_list import add_programm
+from fmake.vhdl_programm_list import add_programm
 
-from vhdl_build_system.generic_helper import  vprint, try_remove_file , save_file , load_file 
-from vhdl_build_system.generic_helper import extract_cl_arguments, cl_add_entity , cl_add_OutputCSV, cl_add_gui
+from fmake.generic_helper import  vprint, try_remove_file , save_file , load_file 
+from fmake.generic_helper import extract_cl_arguments, cl_add_entity , cl_add_OutputCSV, cl_add_gui
 
-from vhdl_build_system.Convert2CSV import Convert2CSV , Convert2CSV_add_CL_args
+from fmake.Convert2CSV import Convert2CSV , Convert2CSV_add_CL_args
 
 
 
 def make_tcl_file(entity_name, intermediate_csv,tcl_file, do_quit = ""):
     onerror = '{' +'resume}'
     clock_speed_file= "build/"+entity_name+"/"+"clock_speed.txt"
     clock_speed=int(load_file(clock_speed_file))
@@ -51,16 +51,17 @@
     cmd_arg_gui = " -gui &" if Run_with_gui else ""
     
     
     
     if input_xls!= "":
         try_remove_file(intermediate_csv)
         Convert2CSV( input_xls, Sheet,intermediate_csv, drop )
-        
-    os.system("killall " +programm_name)
+    cmd = run_in_bash("killall " +programm_name)   
+    vprint(2)("command: " + cmd) 
+    os.system(cmd )
     
     def build_program():
         if  Run_with_gui:
             return
         try_remove_file(build_path + programm_name )
         cmd = "source " + ise_path + " && cd " + build_path + " && " + "fuse -intstyle ise -incremental -lib secureip -o " + programm_name+ " -prj "+ project_name + "  work." + entity_name
         cmd = run_in_bash(cmd)
```

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_csv_io/CSV_UtilityPkg.py` & `fmake-0.0.9/fmake/vhdl_csv_io/CSV_UtilityPkg.py`

 * *Files identical despite different names*

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_csv_io/e_csv_read_file.py` & `fmake-0.0.9/fmake/vhdl_csv_io/e_csv_read_file.py`

 * *Files identical despite different names*

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_csv_io/e_csv_write_file.py` & `fmake-0.0.9/fmake/vhdl_csv_io/e_csv_write_file.py`

 * *Files identical despite different names*

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_csv_io/type_conversions_helper.py` & `fmake-0.0.9/fmake/vhdl_csv_io/type_conversions_helper.py`

 * *Files identical despite different names*

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_dependency_db.py` & `fmake-0.0.9/fmake/vhdl_dependency_db.py`

 * *Files identical despite different names*

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_entity_class.py` & `fmake-0.0.9/fmake/vhdl_entity_class.py`

 * *Files identical despite different names*

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_get_entity_def.py` & `fmake-0.0.9/fmake/vhdl_get_entity_def.py`

 * *Files identical despite different names*

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_get_list_of_files.py` & `fmake-0.0.9/fmake/vhdl_get_list_of_files.py`

 * *Files identical despite different names*

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_get_type_def.py` & `fmake-0.0.9/fmake/vhdl_get_type_def.py`

 * *Files identical despite different names*

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_load_file_without_comments.py` & `fmake-0.0.9/fmake/vhdl_load_file_without_comments.py`

 * *Files identical despite different names*

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_make_simulation.py` & `fmake-0.0.9/fmake/vhdl_make_simulation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 
 import argparse
-from vhdl_build_system.generic_helper import try_make_dir,save_file,load_file, cl_add_entity
+from fmake.generic_helper import try_make_dir,save_file,load_file, cl_add_entity
 
-from vhdl_build_system.vhdl_dependency_db  import get_dependency_db
+from fmake.vhdl_dependency_db  import get_dependency_db
 
 
-from vhdl_build_system.vhdl_programm_list import  add_programm
+from fmake.vhdl_programm_list import  add_programm
 
-from vhdl_build_system.generic_helper import  vprint, extract_cl_arguments
+from fmake.generic_helper import  vprint, extract_cl_arguments
 
 def vhdl_make_simulation_intern(entity,BuildFolder = "build/"):  
     OutputPath = BuildFolder + entity + "/"
     
     CSV_readFile=OutputPath+entity+".csv" 
     CSV_writeFile=OutputPath+entity+"_out.csv" 
     try_make_dir(OutputPath)
```

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_make_test_bench.py` & `fmake-0.0.9/fmake/vhdl_make_test_bench.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 
 
 
-from  vhdl_build_system.vhdl_make_test_bench_names   import get_IO_pgk_name, get_writer_record_name, get_reader_record_name, get_reader_entity_name, get_includes, get_writer_entity_name
+from  fmake.vhdl_make_test_bench_names   import get_IO_pgk_name, get_writer_record_name, get_reader_record_name, get_reader_entity_name, get_includes, get_writer_entity_name
 
-from  vhdl_build_system.vhdl_dependency_db           import get_dependency_db
-from  vhdl_build_system.vhdl_entity_class            import vhdl_entity
-from  vhdl_build_system.vhdl_merge_split_test_cases  import merge_test_case
-from  vhdl_build_system.generic_helper               import save_file, try_make_dir, cl_add_entity, join_str
-from  vhdl_build_system.vhdl_programm_list           import add_programm 
-from  vhdl_build_system.generic_helper               import vprint, extract_cl_arguments
+from  fmake.vhdl_dependency_db           import get_dependency_db
+from  fmake.vhdl_entity_class            import vhdl_entity
+from  fmake.vhdl_merge_split_test_cases  import merge_test_case
+from  fmake.generic_helper               import save_file, try_make_dir, cl_add_entity, join_str
+from  fmake.vhdl_programm_list           import add_programm 
+from  fmake.generic_helper               import vprint, extract_cl_arguments
 
 import argparse
 import numpy as np 
 
 import pandas as pd
 import wget
```

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_make_test_bench_names.py` & `fmake-0.0.9/fmake/vhdl_make_test_bench_names.py`

 * *Files identical despite different names*

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_merge_split_test_cases.py` & `fmake-0.0.9/fmake/vhdl_merge_split_test_cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 
 import pandas as pd
 
 from .generic_helper import load_file, save_file
 import argparse
-from vhdl_build_system.vhdl_programm_list import add_programm
+from fmake.vhdl_programm_list import add_programm
 
 
 def Convert2CSV(XlsFile,Sheet,OutputFile):
 
     data_xls = pd.read_excel(XlsFile, Sheet, index_col=None , engine = 'openpyxl')
 
     data_xls.to_csv(OutputFile, encoding='utf-8',index =False)
```

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_parser.py` & `fmake-0.0.9/fmake/vhdl_parser.py`

 * *Files identical despite different names*

### Comparing `fmake-0.0.8/vhdl_build_system/vhdl_run_vivado.py` & `fmake-0.0.9/fmake/vhdl_run_vivado.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import shutil
 
 import pandas as pd
 import argparse
 
-from vhdl_build_system.vhdl_programm_list import add_programm
+from fmake.vhdl_programm_list import add_programm
 
-from vhdl_build_system.generic_helper import  vprint, try_remove_file , save_file , load_file 
+from fmake.generic_helper import  vprint, try_remove_file , save_file , load_file 
 
 
-from vhdl_build_system.generic_helper import extract_cl_arguments, cl_add_entity ,cl_add_OutputCSV, cl_add_gui
+from fmake.generic_helper import extract_cl_arguments, cl_add_entity ,cl_add_OutputCSV, cl_add_gui
 
-from vhdl_build_system.Convert2CSV import Convert2CSV , Convert2CSV_add_CL_args 
+from fmake.Convert2CSV import Convert2CSV , Convert2CSV_add_CL_args 
 
 
 
 
 
 
 def vivado_run(args):
```

