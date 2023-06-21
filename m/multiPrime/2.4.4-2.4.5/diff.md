# Comparing `tmp/multiPrime-2.4.4.tar.gz` & `tmp/multiPrime-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiPrime-2.4.4.tar", last modified: Wed Jun 21 02:24:51 2023, max compression
+gzip compressed data, was "multiPrime-2.4.5.tar", last modified: Wed Jun 21 05:39:21 2023, max compression
```

## Comparing `multiPrime-2.4.4.tar` & `multiPrime-2.4.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 02:24:51.471939 multiPrime-2.4.4/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-06-21 01:58:41.000000 multiPrime-2.4.4/LICENSE
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    17013 2023-06-21 02:24:51.471939 multiPrime-2.4.4/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16860 2023-06-21 02:13:16.000000 multiPrime-2.4.4/README.md
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 02:24:51.470939 multiPrime-2.4.4/multiPrime/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-06-21 01:58:41.000000 multiPrime-2.4.4/multiPrime/__init__.py
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 02:24:51.470939 multiPrime-2.4.4/multiPrime.egg-info/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    17013 2023-06-21 02:24:51.000000 multiPrime-2.4.4/multiPrime.egg-info/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      274 2023-06-21 02:24:51.000000 multiPrime-2.4.4/multiPrime.egg-info/SOURCES.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-06-21 02:24:51.000000 multiPrime-2.4.4/multiPrime.egg-info/dependency_links.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-06-21 02:24:51.000000 multiPrime-2.4.4/multiPrime.egg-info/entry_points.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-06-21 02:24:51.000000 multiPrime-2.4.4/multiPrime.egg-info/top_level.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-06-21 02:24:51.471939 multiPrime-2.4.4/setup.cfg
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1798 2023-06-21 01:58:41.000000 multiPrime-2.4.4/setup.py
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 02:24:51.471939 multiPrime-2.4.4/src/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-06-21 02:17:27.000000 multiPrime-2.4.4/src/_version.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-06-21 01:58:41.000000 multiPrime-2.4.4/src/main.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    87717 2023-06-21 01:58:41.000000 multiPrime-2.4.4/src/src.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    26139 2023-06-21 02:24:17.000000 multiPrime-2.4.4/src/utils.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 05:39:21.444408 multiPrime-2.4.5/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-06-21 05:39:01.000000 multiPrime-2.4.5/LICENSE
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16984 2023-06-21 05:39:21.444408 multiPrime-2.4.5/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16831 2023-06-21 05:39:02.000000 multiPrime-2.4.5/README.md
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 05:39:21.443408 multiPrime-2.4.5/multiPrime/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-06-21 05:39:01.000000 multiPrime-2.4.5/multiPrime/__init__.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 05:39:21.443408 multiPrime-2.4.5/multiPrime.egg-info/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16984 2023-06-21 05:39:21.000000 multiPrime-2.4.5/multiPrime.egg-info/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      274 2023-06-21 05:39:21.000000 multiPrime-2.4.5/multiPrime.egg-info/SOURCES.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-06-21 05:39:21.000000 multiPrime-2.4.5/multiPrime.egg-info/dependency_links.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-06-21 05:39:21.000000 multiPrime-2.4.5/multiPrime.egg-info/entry_points.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-06-21 05:39:21.000000 multiPrime-2.4.5/multiPrime.egg-info/top_level.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-06-21 05:39:21.444408 multiPrime-2.4.5/setup.cfg
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1798 2023-06-21 05:39:02.000000 multiPrime-2.4.5/setup.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 05:39:21.444408 multiPrime-2.4.5/src/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-06-21 05:39:02.000000 multiPrime-2.4.5/src/_version.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2467 2023-06-21 05:39:02.000000 multiPrime-2.4.5/src/main.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    86841 2023-06-21 05:39:02.000000 multiPrime-2.4.5/src/src.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    27047 2023-06-21 05:39:02.000000 multiPrime-2.4.5/src/utils.py
```

### Comparing `multiPrime-2.4.4/LICENSE` & `multiPrime-2.4.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 The MIT License (MIT)
 
-Copyright (c) 2022 Junbo Yang <yang_junbo_hi@126.com> <1806389316@pku.edu.cn>
+Copyright (c) 2023 Junbo Yang <yang_junbo_hi@126.com> <1806389316@pku.edu.cn>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `multiPrime-2.4.4/PKG-INFO` & `multiPrime-2.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.4.4
+Version: 2.4.5
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
 
-`multiPrime is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
+`multiPrime (version=2.4.5) is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
 It proposes a solution for the maximal coverage degenerate primer design with error (MD-EDPD).
-version 2.4.2 is equal to the multiPrime pipeline (2.1.1) in https://github.com/joybio/multiPrime.` 
+pipeline links: https://github.com/joybio/multiPrime.` 
 
 ## 1. Install
 
 > pip
 
 ```
 pip3 install multiPrime
```

### Comparing `multiPrime-2.4.4/README.md` & `multiPrime-2.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # multiPrime
 
-`multiPrime is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
+`multiPrime (version=2.4.5) is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
 It proposes a solution for the maximal coverage degenerate primer design with error (MD-EDPD).
-version 2.4.2 is equal to the multiPrime pipeline (2.1.1) in https://github.com/joybio/multiPrime.` 
+pipeline links: https://github.com/joybio/multiPrime.` 
 
 ## 1. Install
 
 > pip
 
 ```
 pip3 install multiPrime
```

### Comparing `multiPrime-2.4.4/multiPrime.egg-info/PKG-INFO` & `multiPrime-2.4.5/multiPrime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.4.4
+Version: 2.4.5
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
 
-`multiPrime is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
+`multiPrime (version=2.4.5) is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
 It proposes a solution for the maximal coverage degenerate primer design with error (MD-EDPD).
-version 2.4.2 is equal to the multiPrime pipeline (2.1.1) in https://github.com/joybio/multiPrime.` 
+pipeline links: https://github.com/joybio/multiPrime.` 
 
 ## 1. Install
 
 > pip
 
 ```
 pip3 install multiPrime
```

### Comparing `multiPrime-2.4.4/setup.py` & `multiPrime-2.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.4.4/src/main.py` & `multiPrime-2.4.5/src/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def main():
     if len(sys.argv) < 2:
         main_Usage()
     elif sys.argv[1] == "DPrime":
         options, args = DPrime_argsParse()
         NN_APP = NN_degenerate(seq_file=options.input, primer_length=options.plen, coverage=options.fraction,
                                number_of_dege_bases=options.dnum, score_of_dege_bases=options.degeneracy,
-                               entropy_threshold=options.entropy, product_len=options.size, position=options.coordinate,
+                               raw_entropy_threshold=options.entropy, product_len=options.size, position=options.coordinate,
                                variation=options.variation, distance=options.away, GC=options.gc, nproc=options.proc,
                                outfile=options.out)
         NN_APP.run()
 
     elif sys.argv[1] == "Ppair":
         options, args = Ppair_argsParse()
         primer_pairs = Primers_filter(ref_file=options.ref, primer_file=options.input, adaptor=options.adaptor,
@@ -30,15 +30,16 @@
         (options, args) = Perfect_argsParse()
         results = Product_perfect(primer_file=options.input, output_file=options.out, ref_file=options.ref,
                                   file_format=options.format, coverage=options.stast, nproc=options.process)
         results.run()
 
     elif sys.argv[1] == "Errors":
         options, args = Errors_argsParse()
-        prediction = Errors(primer_file=options.input_file, term_length=options.len, reference_file=options.ref,
+        ref_index = Bowtie_index(options.ref, options.bowtie)
+        prediction = Errors(primer_file=options.input_file, term_length=options.len, reference_file=ref_index,
                             PCR_product_size=options.size, mismatch_num=options.seedmms, outfile=options.out,
                             term_threshold=options.term, bowtie=options.bowtie, nproc=options.proc)
         prediction.run()
     else:
         print("No subprocess!")
         sys.exit(1)
```

### Comparing `multiPrime-2.4.4/src/src.py` & `multiPrime-2.4.5/src/src.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,19 +299,19 @@
         for acc_id in Input_dict.keys():
             # start_dict[acc_id] = pattern_start.search(Input_dict[acc_id]).span()[0]
             # stop_dict[acc_id] = pattern_stop.search(Input_dict[acc_id]).span()[0] - 1
             t_length = len(Input_dict[acc_id])
             start_dict[acc_id] = t_length - len(Input_dict[acc_id].lstrip("-"))
             stop_dict[acc_id] = len(Input_dict[acc_id].rstrip("-"))
             # start position should contain [coverage] sequences at least.
-        start = np.quantile(np.array(list(start_dict.values())).reshape(1, -1), self.coverage, interpolation="higher")
+        start = np.quantile(np.array(list(start_dict.values())).reshape(1, -1), self.coverage, method="higher")
         # for python 3.9.9
         # start = np.quantile(np.array(list(start_dict.values())).reshape(1, -1), self.coverage, method="higher")
         # stop position should contain [coverage] sequences at least.
-        stop = np.quantile(np.array(list(stop_dict.values())).reshape(1, -1), self.coverage, interpolation="lower")
+        stop = np.quantile(np.array(list(stop_dict.values())).reshape(1, -1), self.coverage, method="lower")
         # stop = np.quantile(np.array(list(stop_dict.values())).reshape(1, -1), self.coverage, method="lower")
         if stop - start < int(self.product):
             print("Error: max length of PCR product is shorter than the default min Product length with {} "
                   "coverage! Non candidate primers !!!".format(self.coverage))
             sys.exit(1)
         else:
             return [start, stop, stop - start]
@@ -562,15 +562,15 @@
             self.mis_primer_check(cover_primer_set, ''.join(optimal_primer_list), cover,
                                   non_gap_seq_id)
         # print(optimal_coverage_init + F_mis_cover_cover)
         # print(optimal_coverage_init + R_mis_cover_cover)
         # print(cover_number)
         # print(optimal_primer_list)
         if optimal_coverage_init + F_mis_cover_cover < cover_number or \
-                    optimal_coverage_init + R_mis_cover_cover < cover_number:
+                optimal_coverage_init + R_mis_cover_cover < cover_number:
             while optimal_coverage_init + F_mis_cover_cover < cover_number or \
                     optimal_coverage_init + R_mis_cover_cover < cover_number:
                 # optimal_primer_update, coverage_update, NN_coverage_update,
                 # NN array_update, degeneracy_update, degenerate_update
                 optimal_primer_list, optimal_coverage_init, optimal_NN_coverage_update, \
                 NN_matrix, degeneracy, number_of_degenerate = \
                     self.refine_by_NN_array(optimal_primer_list, optimal_coverage_init, cover, optimal_NN_index,
@@ -591,15 +591,15 @@
                     break
                 else:
                     optimal_NN_coverage = optimal_NN_coverage_update
         # If the primer coverage does not increase after degeneration,
         # the process will backtrack and assess the original optimal primer.
         # print(optimal_primer_list)
         optimal_primer_current = ''.join(optimal_primer_list)
-        #print(optimal_primer_current)
+        # print(optimal_primer_current)
         information = self.primer_pre_filter(optimal_primer_current)
         # F_mis_cover_cover, F_non_cover_in_cover, R_mis_cover_cover, R_non_cover_in_cover = \
         #     self.mis_primer_check(cover_primer_set, optimal_primer_current, cover,
         #                           non_gap_seq_id)
         F_non_cover.update(F_non_cover_in_cover)
         R_non_cover.update(R_non_cover_in_cover)
         F_mis_cover = optimal_coverage_init + F_mis_cover_cover
@@ -858,15 +858,14 @@
                 json.dump(dict(gap_seq_id_out), fg, indent=4)
             fg.close()
             # get results before shutdown. Synchronous call mode: call, wait for the return value, decouple,
             # but slow.
         p.shutdown()
 
 
-
 class Primers_filter(object):
     def __init__(self, ref_file, primer_file, adaptor, rep_seq_number=500, distance=4, outfile="", diff_Tm=5,
                  size="300,700", position=9, GC="0.4,0.6", nproc=10, fraction=0.6):
         self.nproc = nproc
         self.primer_file = primer_file
         self.adaptor = adaptor
         self.size = size
@@ -1233,22 +1232,23 @@
                 # fo.write(ID + "\t" + "\t".join(headers) + "\t")
                 with open(self.outfile + ".fa", "w") as fa:
                     fo.write(ID + "\t")
                     primer_pairs_sort = sorted(primer_pairs, key=lambda k: k[3], reverse=True)
                     for i in primer_pairs_sort:
                         fo.write("\t".join(map(str, i)) + "\t")
                         start_stop = i[4].split(":")
-                        fa.write(primer_ID + "_" + start_stop[0] + "F\n" + i[0] + "\n" + primer_ID + "_" + start_stop[1]
-                                 + "R\n" + i[1] + "\n")
+                        fa.write(">" + primer_ID + "_" + start_stop[0] + "F\n" + i[0] + "\n>" + primer_ID + "_" +
+                            start_stop[1]+ "R\n" + i[1] + "\n")
                     # get results before shutdown. Synchronous call mode: call, wait for the return value, decouple,
                     # but slow.
                     fo.write("\n")
                     fo.close()
                     fa.close()
 
+
 class Product_perfect(object):
     def __init__(self, primer_file="", output_file="", ref_file="", file_format="fa", coverage="", nproc=10):
         self.nproc = nproc
         self.primers_file = primer_file
         self.ref_file = ref_file
         self.output_file = Path(output_file)
         self.file_format = file_format
@@ -1614,28 +1614,7 @@
                 total_dict = pickle.load(raw_total_seq_dict)
                 print(len(set(total_dict.keys())), len(target_seq))
                 unmatched_seq_set = set(total_dict.keys()) - target_seq
                 with open(self.outfile + ".total.acc.num", "a+") as fo3:
                     fo3.write("total target number is: {}\n".format(len(total_dict.keys())))
                 for unmatch in unmatched_seq_set:
                     out.write(total_dict[unmatch])
-
-def Bowtie_index(Input, method):
-    Bowtie_file = Path(Input).parent.joinpath("Bowtie_DB")
-    Bowtie_prefix = Path(Bowtie_file).joinpath(Path(Input).stem)
-    bowtie_cmd = method + "-build"
-    if re.search("bowtie2", method):
-        ref_index = Path(Bowtie_file).joinpath(Path(Input).name).with_suffix(".1.bt2")
-    elif re.search("bowtie", method):
-        ref_index = Path(Bowtie_file).joinpath(Path(Input).name).with_suffix(".1.ebwt")
-    else:
-        print("bowtie1 or bowtie2 must be specified !!!")
-        sys.exit(1)
-    if ref_index.exists():
-        return Bowtie_prefix
-    else:
-        if Bowtie_file.exists():
-            print("No Bowtie index found, start building ...")
-        else:
-            os.mkdir(Bowtie_file)
-        os.system("{} {} {}".format(bowtie_cmd, Input, Bowtie_prefix))
-        return Bowtie_prefix
```

### Comparing `multiPrime-2.4.4/src/utils.py` & `multiPrime-2.4.5/src/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 #!/usr/bin/env python3
-
+import os
+import re
 from optparse import OptionParser
+from pathlib import Path
+
 import numpy as np
 import sys
 import math
 from operator import mul
 from math import log10
 from functools import reduce
 from bisect import bisect_left
@@ -349,15 +352,15 @@
     elif options.out is None:
         parser.print_help()
         print("No output file provided !!!")
         sys.exit(1)
     return parser.parse_args()
 
 def main_Usage():
-    print('Usage (version 2.4.4): \n'
+    print('Usage (version 2.4.5): \n'
           'multiPrime DPrime:  Degenerate primer design through MD-DPD or MD-EDPD.\n'
           'multiPrime Ppair:   Primer pair selection from the result of multiPrime DPrime.\n'
           'multiPrime Perfect: Extract primer-contained sequences with non-mismatches.\n'
           'multiPrime Errors:  Extract primer-contained sequences with errors.\n')
 
 
 degenerate_base = {"-": ["-"], "A": ["A"], "G": ["G"], "C": ["C"], "T": ["T"], "R": ["A", "G"], "Y": ["C", "T"],
@@ -595,7 +598,28 @@
         # Equation B
         Tm = round(1 / ((1 / (delta_H / (delta_S + 1.9872 * math.log(primer_concentration / (4 * pow(10, 9)), math.e))))
                         + correction) - Kelvin, 2)
     return Tm
 
 
 ##############################################################################################
+
+def Bowtie_index(Input, method):
+    Bowtie_file = Path(Input).parent.joinpath("Bowtie_DB")
+    Bowtie_prefix = Path(Bowtie_file).joinpath(Path(Input).stem)
+    bowtie_cmd = method + "-build"
+    if re.search("bowtie2", method):
+        ref_index = Path(Bowtie_file).joinpath(Path(Input).name).with_suffix(".1.bt2")
+    elif re.search("bowtie", method):
+        ref_index = Path(Bowtie_file).joinpath(Path(Input).name).with_suffix(".1.ebwt")
+    else:
+        print("bowtie1 or bowtie2 must be specified !!!")
+        sys.exit(1)
+    if ref_index.exists():
+        return Bowtie_prefix
+    else:
+        if Bowtie_file.exists():
+            print("No Bowtie index found, start building ...")
+        else:
+            os.mkdir(Bowtie_file)
+        os.system("{} {} {}".format(bowtie_cmd, Input, Bowtie_prefix))
+        return Bowtie_prefix
```

