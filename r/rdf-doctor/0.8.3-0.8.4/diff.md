# Comparing `tmp/rdf_doctor-0.8.3-py3-none-any.whl.zip` & `tmp/rdf_doctor-0.8.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18117 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-19 02:18 doctor/__init__.py
+Zip file size: 18542 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-21 08:19 doctor/__init__.py
 -rw-r--r--  2.0 unx      631 b- defN 23-Jun-19 02:18 doctor/consts.py
--rw-r--r--  2.0 unx    29745 b- defN 23-Jun-19 02:18 doctor/doctor.py
+-rw-r--r--  2.0 unx    31152 b- defN 23-Jun-21 08:15 doctor/doctor.py
 -rw-r--r--  2.0 unx    20305 b- defN 23-Jun-19 02:18 doctor/reference/correct-prefixes.tsv
 -rw-r--r--  2.0 unx       90 b- defN 23-Jun-19 02:18 doctor/reference/refine-classes.tsv
 -rw-r--r--  2.0 unx      679 b- defN 23-Jun-19 02:18 doctor/reference/refine-prefixes.tsv
--rw-r--r--  2.0 unx     1061 b- defN 23-Jun-19 02:22 rdf_doctor-0.8.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     8844 b- defN 23-Jun-19 02:22 rdf_doctor-0.8.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 02:22 rdf_doctor-0.8.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jun-19 02:22 rdf_doctor-0.8.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-19 02:22 rdf_doctor-0.8.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      994 b- defN 23-Jun-19 02:22 rdf_doctor-0.8.3.dist-info/RECORD
-12 files, 62522 bytes uncompressed, 16433 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-21 08:32 rdf_doctor-0.8.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8844 b- defN 23-Jun-21 08:32 rdf_doctor-0.8.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 08:32 rdf_doctor-0.8.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-21 08:32 rdf_doctor-0.8.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-21 08:32 rdf_doctor-0.8.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      994 b- defN 23-Jun-21 08:32 rdf_doctor-0.8.4.dist-info/RECORD
+12 files, 63929 bytes uncompressed, 16858 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: doctor/reference/refine-classes.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefixes.tsv
 Comment: 
 
-Filename: rdf_doctor-0.8.3.dist-info/LICENSE
+Filename: rdf_doctor-0.8.4.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-0.8.3.dist-info/METADATA
+Filename: rdf_doctor-0.8.4.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-0.8.3.dist-info/WHEEL
+Filename: rdf_doctor-0.8.4.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-0.8.3.dist-info/entry_points.txt
+Filename: rdf_doctor-0.8.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-0.8.3.dist-info/top_level.txt
+Filename: rdf_doctor-0.8.4.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-0.8.3.dist-info/RECORD
+Filename: rdf_doctor-0.8.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.8.3"
+__version__ = "0.8.4"
```

## doctor/doctor.py

```diff
@@ -2,15 +2,18 @@
 import sys
 import argparse
 import gzip
 import rdflib
 import re
 import csv
 import codecs
+import time
 import datetime
+import threading
+import queue
 from doctor.consts import VERSION_FILE, REPORT_FORMAT_SHEX, REPORT_FORMAT_MD, REPORT_FORMAT_MARKDOWN, \
                             TARGET_CLASS_ALL, EXTENSION_NT, EXTENSION_TTL, EXTENSION_GZ, CORRECT_PREFIXES_FILE_PATH, \
                             CLASS_ERRATA_FILE_PATH, PREFIX_ERRATA_FILE_PATH, HELP_LINK_URL
 from shexer.shaper import Shaper
 from shexer.consts import NT, TURTLE, GZ, MIXED_INSTANCES
 from unidecode import unidecode
 from collections import defaultdict
@@ -24,50 +27,78 @@
     validation_result, error_msg = validate_command_line_args(args)
     if validation_result == False:
         print(error_msg)
         return
 
     compression_mode = get_compression_mode(args.input[0])
     input_format = get_input_format(args.input[0], compression_mode)
-    output_result = []
+    result_queue = queue.Queue()
 
     try:
         # Processing branch by report format
         if args.report == REPORT_FORMAT_SHEX:
             # shex
-            output_result = get_shex_result(args, input_format, compression_mode)
+            thread_calc = threading.Thread(target=get_shex_result, args=(args, input_format, compression_mode, result_queue,))
 
         elif args.report == REPORT_FORMAT_MARKDOWN or args.report == REPORT_FORMAT_MD:
             # markdown/md
-            output_result = get_markdown_result(args, input_format, compression_mode)
+            thread_calc = threading.Thread(target=get_markdown_result, args=(args, input_format, compression_mode, result_queue,))
 
         else:
             # Else case does not occur.
             # Prevented by validate_command_line_args function.
             raise ValueError(args.report + '" is an unsupported report format. "' + REPORT_FORMAT_SHEX + '" and "' + REPORT_FORMAT_MD+ '"(same as "' + REPORT_FORMAT_MARKDOWN + '") are supported.')
 
+        thread_calc.setDaemon(True)
+        thread_calc.start()
+        if args.verbose:
+            # Thread for displaying dots during processing
+            thread_monitor = threading.Thread(target=monitor_thread, args=(result_queue,))
+            thread_monitor.setDaemon(True)
+            thread_monitor.start()
+
+        thread_calc.join()
+        if args.verbose:
+            thread_monitor.join()
+
         # Output result to specified destination (standard output or file)
         if args.output is None:
-            print("".join(output_result))
+            print_overwrite("".join(result_queue.get()))
         else:
             with open(args.output, "w", encoding="utf-8") as f:
-                f.write("".join(output_result))
+                f.write("".join(result_queue.get()))
 
         if args.verbose:
-            print(get_dt_now() + " -- Done!")
+            print_overwrite(get_dt_now() + " -- Done!")
 
     except ValueError as e:
         print(e)
 
+    except KeyboardInterrupt:
+        print ("Keyboard interrupt occurred.")
+
     except:
         print("An exception error occurred. Input data format may not be correct. Please review the data.")
 
     return
 
 
+# Function for displaying dots during processing
+def monitor_thread(result_queue):
+    i = 0
+    spin_char = ["⠋", "⠙", "⠹", "⠸", "⠼", "⠴", "⠦", "⠧", "⠇", "⠏"]
+    while result_queue.empty():
+        print(spin_char[i], end="\r")
+        if i == len(spin_char) - 1:
+            i = 0
+        else:
+            i += 1
+        time.sleep(0.2)
+
+
 def read(rel_path):
     here = os.path.abspath(os.path.dirname(__file__))
     with codecs.open(os.path.join(here, rel_path), 'r') as fp:
         return fp.read()
 
 
 def get_version(rel_path):
@@ -245,43 +276,43 @@
         return False, error_msg
 
 
     return True, None
 
 
 # Processing when the report format is "shex"
-def get_shex_result(args, input_format, compression_mode):
+def get_shex_result(args, input_format, compression_mode, result_queue):
 
     # Get Prefix when input file is turtle format
     if input_format == TURTLE:
         if args.verbose:
-            print(get_dt_now() + " -- Getting prefixes from input file...")
+            print_overwrite(get_dt_now() + " -- Getting prefixes from input file...")
 
         input_prefixes, duplicated_prefixes = get_input_prefixes(args.input, compression_mode)
     else:
         input_prefixes = []
         duplicated_prefixes = []
 
     shaper_result = get_shaper_result(args, input_format, compression_mode, input_prefixes)
 
     # Prefixes with the same QName but different URIs at the same time
     if args.verbose:
-        print(get_dt_now() + " -- Checking for duplicate prefixes...")
+        print_overwrite(get_dt_now() + " -- Checking for duplicate prefixes...")
 
     result_duplicated_prefixes = []
     if len(duplicated_prefixes) != 0:
         result_duplicated_prefixes.append("# Duplicate prefixes found.\n")
         result_duplicated_prefixes.append("\n")
         result_duplicated_prefixes.append("# Input QName\tURI\n")
         result_duplicated_prefixes.extend(["# " + s for s in duplicated_prefixes])
         result_duplicated_prefixes.append("\n\n")
 
     # Suggest QName based on URI of validation expression output by sheXer and correct-prefixes.tsv
     if args.verbose:
-        print(get_dt_now() + " -- Creating suggestions for QName...")
+        print_overwrite(get_dt_now() + " -- Creating suggestions for QName...")
 
     result_suggested_qname = []
     correct_prefixes = get_correct_prefixes()
     suggested_qname = get_suggested_qname(shaper_result, input_prefixes, correct_prefixes)
     if len(suggested_qname) != 0:
         result_suggested_qname.append("# There may be a better QName.\n\n")
         result_suggested_qname.append("# Input QName\tSuggested QName\tURI\n")
@@ -293,34 +324,34 @@
     shex_final_result.extend(shaper_result)
     if len(result_duplicated_prefixes) != 0:
         shex_final_result.extend(result_duplicated_prefixes)
 
     if len(result_suggested_qname) != 0:
         shex_final_result.extend(result_suggested_qname)
 
-    return shex_final_result
+    result_queue.put(shex_final_result)
 
 
 # Processing when the report format is "md/markdown"
-def get_markdown_result(args, input_format, compression_mode):
+def get_markdown_result(args, input_format, compression_mode, result_queue):
 
     # Processing related to prefixes ------------------
     # Get Prefix when input file is turtle format
     if input_format == TURTLE:
         if args.verbose:
-            print(get_dt_now() + " -- Getting prefixes from input file...")
+            print_overwrite(get_dt_now() + " -- Getting prefixes from input file...")
 
         input_prefixes, duplicated_prefixes = get_input_prefixes(args.input, compression_mode)
     else:
         input_prefixes = []
         duplicated_prefixes = []
 
     # Get list for result output about prefix reuse percentage
     if args.verbose:
-        print(get_dt_now() + " -- Calculating prefix reuse percentage...")
+        print_overwrite(get_dt_now() + " -- Calculating prefix reuse percentage...")
 
     result_prefix_reuse_percentage = []
     result_prefix_reuse_percentage.append("## Prefix reuse percentage ([?](" + HELP_LINK_URL + "))\n")
     result_prefix_reuse_percentage.append("Percentage of prefixes used in the input file that are included in the predefined prefix list inside rdf-doctor.\n")
     prefix_reuse_percentage = get_prefix_reuse_percentage(input_prefixes)
     if prefix_reuse_percentage == None:
         result_prefix_reuse_percentage.append("```\n")
@@ -329,15 +360,15 @@
     else:
         result_prefix_reuse_percentage.append("```\n")
         result_prefix_reuse_percentage.append(str(prefix_reuse_percentage) + "%\n")
         result_prefix_reuse_percentage.append("```\n\n")
 
     # Refer to the errata of prefixes and obtain a list for result output that combines incorrect prefixes and correct prefixes
     if args.verbose:
-        print(get_dt_now() + " -- Comparing with prefix dictionary (errata)...")
+        print_overwrite(get_dt_now() + " -- Comparing with prefix dictionary (errata)...")
 
     result_prefix_errata = []
     prefix_comparison_result = get_prefix_comparison_result(input_prefixes, args.prefix_dict)
     # When there is data to output
     if len(prefix_comparison_result) != 0:
         result_prefix_errata.append("Found prefixes that looks incorrect.\n")
         result_prefix_errata.append("```\n")
@@ -351,37 +382,37 @@
         result_duplicated_prefixes.append("```\n")
         result_duplicated_prefixes.append("Input QName\tURI\n")
         result_duplicated_prefixes.extend([s for s in duplicated_prefixes])
         result_duplicated_prefixes.append("```\n\n")
     # -------------------------------------------------
 
     if args.verbose:
-        print(get_dt_now() + " -- Getting classes from input file...")
+        print_overwrite(get_dt_now() + " -- Getting classes from input file...")
 
     # Processing related to classes -------------------
     input_classes = get_input_classes(args.input, input_format, compression_mode, args.classes)
 
     # Refers to the errata list of the class, acquires the list for result output that combines the incorrect class and the correct class,
     # and returns the class corresponding to each key in fingerprint format stored in dictionary format.
     if args.verbose:
-        print(get_dt_now() + " -- Comparing with class dictionary (errata)...")
+        print_overwrite(get_dt_now() + " -- Comparing with class dictionary (errata)...")
 
     result_class_errata = []
     class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, args.class_dict)
     # When there is data to output
     if len(class_comparison_result) != 0:
         result_class_errata.append("Found class names that looks incorrect.\n")
         result_class_errata.append("```\n")
         result_class_errata.append("Input class name\tSuggested class name\n")
         result_class_errata.extend(class_comparison_result)
         result_class_errata.append("```\n\n")
 
     # Get a result output list to notify about different class strings with the same key as a result of fingerprinting
     if args.verbose:
-        print(get_dt_now() + " -- Comparing with fingerprint method results...")
+        print_overwrite(get_dt_now() + " -- Comparing with fingerprint method results...")
 
     result_class_fingerprint = []
     fingerprint_comparison_result = get_fingerprint_comparison_result(fingerprint_class_dict)
     # When there is data to output
     if len(fingerprint_comparison_result) != 0:
         result_class_fingerprint.append("Found multiple strings that appear to represent the same class name.\n")
         result_class_fingerprint.append("```")
@@ -410,15 +441,15 @@
 
     class_result_exists = len(result_class_errata) != 0 or len(result_class_fingerprint) != 0
     if class_result_exists:
         md_final_result.append("## Refine classes ([?](" + HELP_LINK_URL + "))\n")
         md_final_result.extend(result_class_errata)
         md_final_result.extend(result_class_fingerprint)
 
-    return md_final_result
+    result_queue.put(md_final_result)
 
 
 # Call the shex_graph method of shexer's shaper class and output the result
 def get_shaper_result(args, input_format, compression_mode, input_prefixes):
     # Set parameters when calling the shaper class depending on whether the class is specified as an argument
     if TARGET_CLASS_ALL in args.classes:
         target_classes = None
@@ -679,14 +710,20 @@
 def default_namespaces():
     return {
             "http://www.w3.org/2002/07/owl#": "owl",
             "http://www.w3.org/1999/02/22-rdf-syntax-ns#": "rdf",
             "http://www.w3.org/2000/01/rdf-schema#": "rdfs",
             "http://www.w3.org/2001/XMLSchema#": "xsd",
             "http://www.w3.org/XML/1998/namespace": "xml",
+            "http://www.w3.org/2004/02/skos/core#": "skos",
+            "http://purl.obolibrary.org/obo/": "obo",
             }
 
 # Get current date and time
 # dd/MM/yyyy HH:mm:ss
 # This function will only be called if verbose parameter is True.
 def get_dt_now():
     return datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')
+
+# Overwrites the current line of the console with the string passed as argument
+def print_overwrite(string):
+    print("\r" + string)
```

## Comparing `rdf_doctor-0.8.3.dist-info/LICENSE` & `rdf_doctor-0.8.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-0.8.3.dist-info/METADATA` & `rdf_doctor-0.8.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 0.8.3
+Version: 0.8.4
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

