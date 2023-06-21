# Comparing `tmp/multiPrime-2.4.3.tar.gz` & `tmp/multiPrime-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiPrime-2.4.3.tar", last modified: Wed Apr 19 08:18:42 2023, max compression
+gzip compressed data, was "multiPrime-2.4.4.tar", last modified: Wed Jun 21 02:24:51 2023, max compression
```

## Comparing `multiPrime-2.4.3.tar` & `multiPrime-2.4.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-19 08:18:42.136580 multiPrime-2.4.3/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-04-19 08:13:53.000000 multiPrime-2.4.3/LICENSE
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16020 2023-04-19 08:18:42.136580 multiPrime-2.4.3/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    15867 2023-04-19 08:14:19.000000 multiPrime-2.4.3/README.md
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-19 08:18:42.135580 multiPrime-2.4.3/multiPrime.egg-info/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16020 2023-04-19 08:18:42.000000 multiPrime-2.4.3/multiPrime.egg-info/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      267 2023-04-19 08:18:42.000000 multiPrime-2.4.3/multiPrime.egg-info/SOURCES.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-04-19 08:18:42.000000 multiPrime-2.4.3/multiPrime.egg-info/dependency_links.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-04-19 08:18:42.000000 multiPrime-2.4.3/multiPrime.egg-info/entry_points.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-04-19 08:18:42.000000 multiPrime-2.4.3/multiPrime.egg-info/top_level.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-04-19 08:18:42.136580 multiPrime-2.4.3/setup.cfg
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1795 2023-04-19 08:13:53.000000 multiPrime-2.4.3/setup.py
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-19 08:18:42.136580 multiPrime-2.4.3/src/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-04-19 08:14:29.000000 multiPrime-2.4.3/src/__init__.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-04-19 08:18:27.000000 multiPrime-2.4.3/src/_version.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-04-19 08:18:18.000000 multiPrime-2.4.3/src/main.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    85935 2023-04-19 08:14:29.000000 multiPrime-2.4.3/src/src.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    25251 2023-04-19 08:14:29.000000 multiPrime-2.4.3/src/utils.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 02:24:51.471939 multiPrime-2.4.4/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-06-21 01:58:41.000000 multiPrime-2.4.4/LICENSE
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    17013 2023-06-21 02:24:51.471939 multiPrime-2.4.4/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16860 2023-06-21 02:13:16.000000 multiPrime-2.4.4/README.md
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 02:24:51.470939 multiPrime-2.4.4/multiPrime/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-06-21 01:58:41.000000 multiPrime-2.4.4/multiPrime/__init__.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 02:24:51.470939 multiPrime-2.4.4/multiPrime.egg-info/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    17013 2023-06-21 02:24:51.000000 multiPrime-2.4.4/multiPrime.egg-info/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      274 2023-06-21 02:24:51.000000 multiPrime-2.4.4/multiPrime.egg-info/SOURCES.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-06-21 02:24:51.000000 multiPrime-2.4.4/multiPrime.egg-info/dependency_links.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-06-21 02:24:51.000000 multiPrime-2.4.4/multiPrime.egg-info/entry_points.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-06-21 02:24:51.000000 multiPrime-2.4.4/multiPrime.egg-info/top_level.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-06-21 02:24:51.471939 multiPrime-2.4.4/setup.cfg
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1798 2023-06-21 01:58:41.000000 multiPrime-2.4.4/setup.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-06-21 02:24:51.471939 multiPrime-2.4.4/src/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-06-21 02:17:27.000000 multiPrime-2.4.4/src/_version.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-06-21 01:58:41.000000 multiPrime-2.4.4/src/main.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    87717 2023-06-21 01:58:41.000000 multiPrime-2.4.4/src/src.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    26139 2023-06-21 02:24:17.000000 multiPrime-2.4.4/src/utils.py
```

### Comparing `multiPrime-2.4.3/LICENSE` & `multiPrime-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multiPrime-2.4.3/PKG-INFO` & `multiPrime-2.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.4.3
+Version: 2.4.4
 License: MIT
-Requires-Python: >=3.9
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
 
 `multiPrime is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
 It proposes a solution for the maximal coverage degenerate primer design with error (MD-EDPD).
@@ -91,24 +91,25 @@
 | -o/--out     | Output_dir. default: PCR_product.                                                                                                                                                                              |
 | -s/--stast   | Stast information: number of coverage and total. Default: Coverage.xls.                                                                                                                                        |
 ```
 multiPrime Errors -i [input] -r [bowtie index] -l [150,2000] -p [10]-o [output]
 ```
 Parameters：
 
-| Parameters   | Description                                                                                                                |
-|--------------|----------------------------------------------------------------------------------------------------------------------------|
-| -i/--input   | input file: primer.fa.                                                                                                     |
-| -r/--ref     | reference file: the fasta of raw input.                                                                                    |
-| -l/--len     | Length of primer, which is used for mapping. Default: 18                                                                   |
-| -t/--term    | Position of mismatch is not allowed in the 3 term of primer. Default: 4                                                    |
-| -b/--bowtie  | bowtie or bowtie2 was employed for mapping. Default: bowtie2                                                               |
-| -m/--seedmms | Bowtie: Mismatches in seed (can be 0 - 3, default: -n 1).Bowtie2: Gap or mismatches in seed (can be 0 - 1, default: -n 1). |
-| -p/--process | Number of process to launch. Default: 20.                                                                                  |
-| -o/--out     | Output file: PCR product with primers.                                                                                     |
+| Parameters   | Description                                                                                                                                                                                    |
+|--------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| -i/--input   | input file: primer.fa.                                                                                                                                                                         |
+| -r/--ref     | reference file: the fasta of raw input.                                                                                                                                                        |
+| -l/--len     | Length of primer, which is used for mapping. If the length of the primer used for mapping is set to 0, the entire length of the primer will be utilized. Default: 0                            |
+| -d/--dict    | It is used to extract non-coverd sequences and can be obtained from prepare_fa_pickle.py (https://github.com/joybio/multiPrime). Dictionary of targets sequences, binary format. Default: None |
+| -t/--term    | Position of mismatch is not allowed in the 3 term of primer. Default: 4                                                                                                                        |
+| -b/--bowtie  | bowtie/ABS_path(bowtie) or bowtie2/ABS_path(bowtie2) was employed for mapping. Default: bowtie2                                                                                                |
+| -m/--seedmms | Bowtie: Mismatches in seed (can be 0 - 3, default: -n 1).Bowtie2: Gap or mismatches in seed (can be 0 - 1, default: -n 1).                                                                     |
+| -p/--process | Number of process to launch. Default: 20.                                                                                                                                                      |
+| -o/--out     | Output file: PCR product with primers.                                                                                                                                                         |
 
 
 ## 3. Results
 
 multiPrime DPrime
 + `output`：Information of primer.
 + `output.gap_seq_id_json`: Positions and non-contained sequences caused by errors (number of errors are greater than threshold).
@@ -121,14 +122,15 @@
 + `output`：PCR_product
 + `Coverage.xls`：Total coverage for all primers.
 
 multiPrime Errors 
 + `output`：PCR product with primer pairs.
 + `output.pair.num`：Target amplicon number with primer pairs.
 + `others`：Temp files.
++ `unmatched.fa`: the sequences that were not captured by the core primer set with setting mismatches.
 
 ## 4. test dir
 
 
 multiPrime/example
```

### Comparing `multiPrime-2.4.3/README.md` & `multiPrime-2.4.4/multiPrime.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: multiPrime
+Version: 2.4.4
+License: MIT
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # multiPrime
 
 `multiPrime is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
 It proposes a solution for the maximal coverage degenerate primer design with error (MD-EDPD).
 version 2.4.2 is equal to the multiPrime pipeline (2.1.1) in https://github.com/joybio/multiPrime.` 
 
 ## 1. Install
@@ -83,24 +91,25 @@
 | -o/--out     | Output_dir. default: PCR_product.                                                                                                                                                                              |
 | -s/--stast   | Stast information: number of coverage and total. Default: Coverage.xls.                                                                                                                                        |
 ```
 multiPrime Errors -i [input] -r [bowtie index] -l [150,2000] -p [10]-o [output]
 ```
 Parameters：
 
-| Parameters   | Description                                                                                                                |
-|--------------|----------------------------------------------------------------------------------------------------------------------------|
-| -i/--input   | input file: primer.fa.                                                                                                     |
-| -r/--ref     | reference file: the fasta of raw input.                                                                                    |
-| -l/--len     | Length of primer, which is used for mapping. Default: 18                                                                   |
-| -t/--term    | Position of mismatch is not allowed in the 3 term of primer. Default: 4                                                    |
-| -b/--bowtie  | bowtie or bowtie2 was employed for mapping. Default: bowtie2                                                               |
-| -m/--seedmms | Bowtie: Mismatches in seed (can be 0 - 3, default: -n 1).Bowtie2: Gap or mismatches in seed (can be 0 - 1, default: -n 1). |
-| -p/--process | Number of process to launch. Default: 20.                                                                                  |
-| -o/--out     | Output file: PCR product with primers.                                                                                     |
+| Parameters   | Description                                                                                                                                                                                    |
+|--------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| -i/--input   | input file: primer.fa.                                                                                                                                                                         |
+| -r/--ref     | reference file: the fasta of raw input.                                                                                                                                                        |
+| -l/--len     | Length of primer, which is used for mapping. If the length of the primer used for mapping is set to 0, the entire length of the primer will be utilized. Default: 0                            |
+| -d/--dict    | It is used to extract non-coverd sequences and can be obtained from prepare_fa_pickle.py (https://github.com/joybio/multiPrime). Dictionary of targets sequences, binary format. Default: None |
+| -t/--term    | Position of mismatch is not allowed in the 3 term of primer. Default: 4                                                                                                                        |
+| -b/--bowtie  | bowtie/ABS_path(bowtie) or bowtie2/ABS_path(bowtie2) was employed for mapping. Default: bowtie2                                                                                                |
+| -m/--seedmms | Bowtie: Mismatches in seed (can be 0 - 3, default: -n 1).Bowtie2: Gap or mismatches in seed (can be 0 - 1, default: -n 1).                                                                     |
+| -p/--process | Number of process to launch. Default: 20.                                                                                                                                                      |
+| -o/--out     | Output file: PCR product with primers.                                                                                                                                                         |
 
 
 ## 3. Results
 
 multiPrime DPrime
 + `output`：Information of primer.
 + `output.gap_seq_id_json`: Positions and non-contained sequences caused by errors (number of errors are greater than threshold).
@@ -113,14 +122,15 @@
 + `output`：PCR_product
 + `Coverage.xls`：Total coverage for all primers.
 
 multiPrime Errors 
 + `output`：PCR product with primer pairs.
 + `output.pair.num`：Target amplicon number with primer pairs.
 + `others`：Temp files.
++ `unmatched.fa`: the sequences that were not captured by the core primer set with setting mismatches.
 
 ## 4. test dir
 
 
 multiPrime/example
```

### Comparing `multiPrime-2.4.3/multiPrime.egg-info/PKG-INFO` & `multiPrime-2.4.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: multiPrime
-Version: 2.4.3
-License: MIT
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # multiPrime
 
 `multiPrime is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
 It proposes a solution for the maximal coverage degenerate primer design with error (MD-EDPD).
 version 2.4.2 is equal to the multiPrime pipeline (2.1.1) in https://github.com/joybio/multiPrime.` 
 
 ## 1. Install
@@ -91,24 +83,25 @@
 | -o/--out     | Output_dir. default: PCR_product.                                                                                                                                                                              |
 | -s/--stast   | Stast information: number of coverage and total. Default: Coverage.xls.                                                                                                                                        |
 ```
 multiPrime Errors -i [input] -r [bowtie index] -l [150,2000] -p [10]-o [output]
 ```
 Parameters：
 
-| Parameters   | Description                                                                                                                |
-|--------------|----------------------------------------------------------------------------------------------------------------------------|
-| -i/--input   | input file: primer.fa.                                                                                                     |
-| -r/--ref     | reference file: the fasta of raw input.                                                                                    |
-| -l/--len     | Length of primer, which is used for mapping. Default: 18                                                                   |
-| -t/--term    | Position of mismatch is not allowed in the 3 term of primer. Default: 4                                                    |
-| -b/--bowtie  | bowtie or bowtie2 was employed for mapping. Default: bowtie2                                                               |
-| -m/--seedmms | Bowtie: Mismatches in seed (can be 0 - 3, default: -n 1).Bowtie2: Gap or mismatches in seed (can be 0 - 1, default: -n 1). |
-| -p/--process | Number of process to launch. Default: 20.                                                                                  |
-| -o/--out     | Output file: PCR product with primers.                                                                                     |
+| Parameters   | Description                                                                                                                                                                                    |
+|--------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| -i/--input   | input file: primer.fa.                                                                                                                                                                         |
+| -r/--ref     | reference file: the fasta of raw input.                                                                                                                                                        |
+| -l/--len     | Length of primer, which is used for mapping. If the length of the primer used for mapping is set to 0, the entire length of the primer will be utilized. Default: 0                            |
+| -d/--dict    | It is used to extract non-coverd sequences and can be obtained from prepare_fa_pickle.py (https://github.com/joybio/multiPrime). Dictionary of targets sequences, binary format. Default: None |
+| -t/--term    | Position of mismatch is not allowed in the 3 term of primer. Default: 4                                                                                                                        |
+| -b/--bowtie  | bowtie/ABS_path(bowtie) or bowtie2/ABS_path(bowtie2) was employed for mapping. Default: bowtie2                                                                                                |
+| -m/--seedmms | Bowtie: Mismatches in seed (can be 0 - 3, default: -n 1).Bowtie2: Gap or mismatches in seed (can be 0 - 1, default: -n 1).                                                                     |
+| -p/--process | Number of process to launch. Default: 20.                                                                                                                                                      |
+| -o/--out     | Output file: PCR product with primers.                                                                                                                                                         |
 
 
 ## 3. Results
 
 multiPrime DPrime
 + `output`：Information of primer.
 + `output.gap_seq_id_json`: Positions and non-contained sequences caused by errors (number of errors are greater than threshold).
@@ -121,14 +114,15 @@
 + `output`：PCR_product
 + `Coverage.xls`：Total coverage for all primers.
 
 multiPrime Errors 
 + `output`：PCR product with primer pairs.
 + `output.pair.num`：Target amplicon number with primer pairs.
 + `others`：Temp files.
++ `unmatched.fa`: the sequences that were not captured by the core primer set with setting mismatches.
 
 ## 4. test dir
 
 
 multiPrime/example
```

### Comparing `multiPrime-2.4.3/setup.py` & `multiPrime-2.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,32 +41,33 @@
 
 def getdes():
     des = ""
     with open(os.path.join(os.getcwd(), "README.md")) as fi:
         des = fi.read()
     return des
 
+
 def get_requirement():
     requires = []
     with open(os.path.join(os.path.dirname(__file__), "requirements.txt")) as fi:
         for line in fi:
             line = line.strip()
             requires.append(line)
     return requires
 
 
 setup(
     name=PKG,
     version=get_version(),
     packages=[PKG],
     license="MIT",
-    package_dir={PKG: "src"},
-    #install_requires=get_requirement(),
-    python_requires='>=3.9',
-    #ext_modules=getExtension(),
+    #package_dir={PKG: "src"},
+    # install_requires=get_requirement(),
+    python_requires='>=3.6',
+    ext_modules=getExtension(),
     long_description=getdes(),
     long_description_content_type='text/markdown',
     entry_points={
         'console_scripts': [
             '%s = %s.main:main' % (PKG, PKG),
         ]
     }
```

### Comparing `multiPrime-2.4.3/src/main.py` & `multiPrime-2.4.4/src/main.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.4.3/src/src.py` & `multiPrime-2.4.4/src/src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+import pickle
 
 from .utils import *
 from multiprocessing import Manager
 from collections import defaultdict
 import re
 import os
 from concurrent.futures import ProcessPoolExecutor
@@ -59,78 +60,50 @@
     ################# pre_filter #####################
     ##################################################
 
     ################### hairpin ######################
     def hairpin_check(self, primer):
         n = 0
         distance = self.distance
-        check = "FALSE"
         while n <= len(primer) - 5 - 5 - distance:
             kmer = self.degenerate_seq(primer[n:n + 5])
             left = self.degenerate_seq(primer[n + 5 + distance:])
             for k in kmer:
                 for l in left:
                     if re.search(RC(k), l):
-                        check = "TRUE"
-                        break
-                if check == "TRUE":
-                    break
-            if check == "TRUE":
-                break
+                        return True
             n += 1
-
-        if check == "TRUE":
-            return True
-        else:
-            return False
+        return False
 
     ################# GC content #####################
     def GC_fraction(self, sequence):
         sequence_expand = self.degenerate_seq(sequence)
         GC_list = []
         for seq in sequence_expand:
             GC_list.append(round((list(seq).count("G") + list(seq).count("C")) / len(list(seq)), 3))
         GC_average = round(mean(GC_list), 2)
         return GC_average
 
     ################# di_nucleotide #####################
     def di_nucleotide(self, primer):
-        Check = "False"
         primers = self.degenerate_seq(primer)
         for m in primers:
             for n in di_nucleotides:
                 if re.search(n, m):
-                    Check = "True"
-                    break
-                else:
-                    pass
-            if Check == "True":
-                break
-        if Check == "True":
-            return True
-        else:
-            return False
-
-    ##################################################
-    ################### filter #######################
-    ##################################################
+                    return True
+        return False
 
     ################## GC Clamp ######################
     def GC_clamp(self, primer, num=4, length=13):
-        check = False
         for i in range(num, (num + length)):
             s = primer[-i:]
             gc_fraction = self.GC_fraction(s)
             if gc_fraction > 0.6:
-                check = True
-                break
-        if check:
-            return True
-        else:
-            return False
+                return True
+        return False
 
     ################# position of degenerate base #####################
     def dege_filter_in_term_N_bp(self, sequence):
         term = self.position
         if term == 0:
             term_base = ["A"]
         else:
@@ -154,15 +127,14 @@
                         acc_id = i[0]
                     else:
                         # carefully !, make sure that Ns have been replaced!
                         sequence = re.sub("[^ACGTRYMKSWHBVD]", "-", i.strip().upper())
                         seq_dict[acc_id] += sequence
         return seq_dict, len(seq_dict)
 
-
     def current_end(self, primer, adaptor="", num=5, length=14):
         primer_extend = adaptor + primer
         end_seq = []
         for i in range(num, (num + length)):
             s = primer_extend[-i:]
             if s:
                 end_seq.extend(self.degenerate_seq(s))
@@ -171,15 +143,16 @@
     def deltaG(self, sequence):
         Delta_G_list = []
         Na = 50
         for seq in self.degenerate_seq(sequence):
             Delta_G = 0
             for n in range(len(seq) - 1):
                 base_i, base_j = base2bit[seq[n + 1]], base2bit[seq[n]]
-                Delta_G += freedom_of_H_37_table[base_i][base_j] * H_bonds_number[base_i][base_j] + penalty_of_H_37_table[base_i][base_j]
+                Delta_G += freedom_of_H_37_table[base_i][base_j] * H_bonds_number[base_i][base_j] + \
+                           penalty_of_H_37_table[base_i][base_j]
             term5 = sequence[-2:]
             if term5 == "TA":
                 Delta_G += adjust_initiation[seq[0]] + adjust_initiation[seq[-1]] + adjust_terminal_TA
             else:
                 Delta_G += adjust_initiation[seq[0]] + adjust_initiation[seq[-1]]
             # adjust by concentration of Na+
             Delta_G -= (0.175 * math.log(Na / 1000, math.e) + 0.20) * len(seq)
@@ -187,35 +160,28 @@
                 Delta_G += symmetry_correction
             Delta_G_list.append(Delta_G)
         return round(max(Delta_G_list), 2)
 
     def dimer_check(self, primer):
         current_end = self.current_end(primer)
         current_end_sort = sorted(current_end, key=lambda i: len(i), reverse=True)
-        dimer = False
         for end in current_end_sort:
             for p in self.degenerate_seq(primer):
                 idx = p.find(RC(end))
                 if idx >= 0:
                     end_length = len(end)
                     end_GC = end.count("G") + end.count("C")
                     end_d1 = 0
                     end_d2 = len(p) - len(end) - idx
                     Loss = Penalty_points(
                         end_length, end_GC, end_d1, end_d2)
                     delta_G = self.deltaG(end)
                     if Loss >= 3 or (delta_G < -5 and (end_d1 == end_d2)):
-                        dimer = True
-                        break
-            if dimer:
-                break
-        if dimer:
-            return True
-        else:
-            return False
+                        return True
+        return False
 
     ####################################################################
     ##### pre-filter by GC content / di-nucleotide / hairpin ###########
     def primer_pre_filter(self, primer):
         information = []
         min_GC, max_GC = self.GC
         primer_GC_content = self.GC_fraction(primer)
@@ -344,26 +310,25 @@
         stop = np.quantile(np.array(list(stop_dict.values())).reshape(1, -1), self.coverage, interpolation="lower")
         # stop = np.quantile(np.array(list(stop_dict.values())).reshape(1, -1), self.coverage, method="lower")
         if stop - start < int(self.product):
             print("Error: max length of PCR product is shorter than the default min Product length with {} "
                   "coverage! Non candidate primers !!!".format(self.coverage))
             sys.exit(1)
         else:
-            return [start, stop, stop-start]
+            return [start, stop, stop - start]
 
     def entropy_threshold_adjust(self, length):
         if length < 5000:
             return self.raw_entropy_threshold
         else:
             if length < 10000:
                 return self.raw_entropy_threshold * 0.95
             else:
                 return self.raw_entropy_threshold * 0.9
 
-
     def get_primers(self, sequence_dict, primer_start):  # , primer_info, non_cov_primer_out
         # record sequence and acc id
         non_gap_seq_id = defaultdict(list)
         # record sequence (no gap) and number
         cover = defaultdict(int)
         cover_for_MM = defaultdict(int)
         # record total coverage sequence number
@@ -475,15 +440,15 @@
         # mis-coverage in the following step.
         cover_primer_set = set(cover.keys())
         # if full_degenerate_primer is ok, then return full_degenerate_primer
         # mismatch_coverage, non_cov_primer_info = {}, {}
         F_non_cover, R_non_cover = {}, {}
         ######################################################################################################
         ############ need prone. not all primers is proper for primer-F or primer-R ##########################
-        ## if primer located in the start region, you do not need to calculate coverage for primer-R #########
+        # If a primer is located in the start region, there is no need to calculate its coverage for primer-R#
         ## here is a suggestion. we can assert candidate primer as primer-F or primer-R by primer attribute ##
         ######################################################################################################
         if self.pre_degenerate_primer_check(full_degenerate_primer):
             information = self.primer_pre_filter(full_degenerate_primer)
             optimal_primer_current = full_degenerate_primer
             F_mis_cover_cover, F_non_cover_in_cover, R_mis_cover_cover, R_non_cover_in_cover = \
                 self.mis_primer_check(cover_primer_set, full_degenerate_primer, cover,
@@ -569,15 +534,14 @@
         primer_degenerate_number = dege_number(optimal_primer_current)
         Tm, coverage = [], []
         for seq in self.degenerate_seq(optimal_primer_current):
             Tm.append(Calc_Tm_v2(seq))
             coverage.append(cover[seq])
         Tm_average = round(mean(Tm), 2)
         perfect_coverage = sum(coverage)
-        # print(optimal_coverage_init)
         out_mismatch_coverage = [primer_start, [cBit, tBit, optimal_primer_current, primer_degenerate_number,
                                                 nonsense_primer_number, perfect_coverage, F_mis_cover,
                                                 R_mis_cover, Tm_average, information]]
         non_cov_primer_info = [primer_start, [F_non_cover, R_non_cover]]
         return out_mismatch_coverage, non_cov_primer_info
 
     def coverage_stast(self, cover, optimal_primer_index, NN_matrix, optimal_coverage_init, cover_number,
@@ -589,40 +553,61 @@
         for idx in range(len(optimal_primer_index) - 1):
             # NN index
             optimal_NN_index.append([optimal_primer_index[idx], optimal_primer_index[idx + 1]])
             # NN coverage
             # Is the minimum number in NN coverage = optimal_primer_coverage ? No!
             optimal_NN_coverage.append(
                 NN_matrix[idx, optimal_primer_index[idx], optimal_primer_index[idx + 1]])
-        while optimal_coverage_init < cover_number:
-            # optimal_primer_update, coverage_update, NN_coverage_update,
-            # NN array_update, degeneracy_update, degenerate_update
-            optimal_primer_list, optimal_coverage_init, optimal_NN_coverage_update, \
-            NN_matrix, degeneracy, number_of_degenerate = \
-                self.refine_by_NN_array(optimal_primer_list, optimal_coverage_init, cover, optimal_NN_index,
-                                        optimal_NN_coverage, NN_matrix)
-            if optimal_NN_coverage_update == optimal_NN_coverage:
-                # NN_coverage not change means bugs or there are continuous positions mismatch
-                break
-            elif degeneracy >= self.score_of_dege_bases or number_of_degenerate >= self.number_of_dege_bases:
-                break
-            else:
-                optimal_NN_coverage = optimal_NN_coverage_update
-        optimal_primer_current = ''.join(optimal_primer_list)
-        information = self.primer_pre_filter(optimal_primer_current)
+        # mis-coverage initialization
         F_mis_cover_cover, F_non_cover_in_cover, R_mis_cover_cover, R_non_cover_in_cover = \
-            self.mis_primer_check(cover_primer_set, optimal_primer_current, cover,
+            self.mis_primer_check(cover_primer_set, ''.join(optimal_primer_list), cover,
                                   non_gap_seq_id)
+        # print(optimal_coverage_init + F_mis_cover_cover)
+        # print(optimal_coverage_init + R_mis_cover_cover)
+        # print(cover_number)
+        # print(optimal_primer_list)
+        if optimal_coverage_init + F_mis_cover_cover < cover_number or \
+                    optimal_coverage_init + R_mis_cover_cover < cover_number:
+            while optimal_coverage_init + F_mis_cover_cover < cover_number or \
+                    optimal_coverage_init + R_mis_cover_cover < cover_number:
+                # optimal_primer_update, coverage_update, NN_coverage_update,
+                # NN array_update, degeneracy_update, degenerate_update
+                optimal_primer_list, optimal_coverage_init, optimal_NN_coverage_update, \
+                NN_matrix, degeneracy, number_of_degenerate = \
+                    self.refine_by_NN_array(optimal_primer_list, optimal_coverage_init, cover, optimal_NN_index,
+                                            optimal_NN_coverage, NN_matrix)
+                F_mis_cover_cover, F_non_cover_in_cover, R_mis_cover_cover, R_non_cover_in_cover = \
+                    self.mis_primer_check(cover_primer_set, ''.join(optimal_primer_list), cover,
+                                          non_gap_seq_id)
+                # If there is no increase in NN_coverage,
+                # it suggests the presence of bugs or a mismatch in continuous positions.
+                # Is this step necessary? or shall we use DegePrime method? or shall we use machine learning?
+                if F_mis_cover_cover == R_mis_cover_cover == cover_number - optimal_coverage_init:
+                    break
+                elif optimal_NN_coverage_update == optimal_NN_coverage:
+                    break
+                # If the degeneracy exceeds the threshold, the loop will break.
+                elif 2 * degeneracy > self.score_of_dege_bases or 3 * degeneracy / 2 > self.score_of_dege_bases \
+                        or number_of_degenerate == self.number_of_dege_bases:
+                    break
+                else:
+                    optimal_NN_coverage = optimal_NN_coverage_update
+        # If the primer coverage does not increase after degeneration,
+        # the process will backtrack and assess the original optimal primer.
+        # print(optimal_primer_list)
+        optimal_primer_current = ''.join(optimal_primer_list)
+        #print(optimal_primer_current)
+        information = self.primer_pre_filter(optimal_primer_current)
+        # F_mis_cover_cover, F_non_cover_in_cover, R_mis_cover_cover, R_non_cover_in_cover = \
+        #     self.mis_primer_check(cover_primer_set, optimal_primer_current, cover,
+        #                           non_gap_seq_id)
         F_non_cover.update(F_non_cover_in_cover)
         R_non_cover.update(R_non_cover_in_cover)
         F_mis_cover = optimal_coverage_init + F_mis_cover_cover
         R_mis_cover = optimal_coverage_init + R_mis_cover_cover
-        # print(optimal_coverage_init)
-        # print(F_mis_cover_cover)
-        # print(R_mis_cover_cover)
         return optimal_primer_current, F_mis_cover, R_mis_cover, information, F_non_cover, R_non_cover
 
     def refine_by_NN_array(self, optimal_primer_list, optimal_coverage_init, cover,
                            optimal_NN_index, optimal_NN_coverage, NN_array):
         # use minimum index of optimal_NN_coverage as the position to refine
         refine_index = np.where(optimal_NN_coverage == np.min(optimal_NN_coverage))[0]  # np.where[0] is a list
         # build dict to record coverage and NN array
@@ -820,35 +805,35 @@
                     F_non_cover[uncover_primer] = non_gap_seq_id[uncover_primer]
                 else:
                     F_mis_cover += cover[uncover_primer]
                 if len(set(Y_dist).intersection(self.Y_strict_R)) > 0:
                     R_non_cover[uncover_primer] = non_gap_seq_id[uncover_primer]
                 else:
                     R_mis_cover += cover[uncover_primer]
-        # print(F_mis_cover)
-        # print(R_mis_cover)
         return F_mis_cover, F_non_cover, R_mis_cover, R_non_cover
 
     ################# get_primers #####################
     def run(self):
         p = ProcessPoolExecutor(self.nproc)  #
         sequence_dict = self.seq_dict
         start_primer = self.start_position
         stop_primer = self.stop_position
         # primer_info = Manager().list()
         # non_cov_primer_out = Manager().list()
+        # for position in range(1245,  stop_primer - self.primer_length):
         for position in range(start_primer, stop_primer - self.primer_length):
             # print(position)
             p.submit(self.get_primers(sequence_dict, position))  # , primer_info, non_cov_primer_out
             # This will submit all tasks to one place without blocking, and then each
             # thread in the thread pool will fetch tasks.
         n = 0
         candidate_list, non_cov_primer_out, gap_seq_id_out = [], [], []
         with open(self.outfile, "w") as fo:
-            headers = ["Position", "Entropy of cover (bit)", "Entropy of total (bit)", "Optimal_primer", "primer_degenerate_number",
+            headers = ["Position", "Entropy of cover (bit)", "Entropy of total (bit)", "Optimal_primer",
+                       "primer_degenerate_number",
                        "nonsense_primer_number", "Optimal_coverage", "Mis-F-coverage", "Mis-R-coverage", "Tm",
                        "Information"]
             fo.write("\t".join(map(str, headers)) + "\n")
             while n < stop_primer - start_primer - self.primer_length:
                 res = self.resQ.get()
                 # The get method can read and delete an element from the queue. Similarly, the get method has two
                 # optional parameters: blocked and timeout. If blocked is true (the default value) and timeout is
@@ -873,14 +858,15 @@
                 json.dump(dict(gap_seq_id_out), fg, indent=4)
             fg.close()
             # get results before shutdown. Synchronous call mode: call, wait for the return value, decouple,
             # but slow.
         p.shutdown()
 
 
+
 class Primers_filter(object):
     def __init__(self, ref_file, primer_file, adaptor, rep_seq_number=500, distance=4, outfile="", diff_Tm=5,
                  size="300,700", position=9, GC="0.4,0.6", nproc=10, fraction=0.6):
         self.nproc = nproc
         self.primer_file = primer_file
         self.adaptor = adaptor
         self.size = size
@@ -1402,30 +1388,31 @@
                 "Coveraged number of sequence:\t{}\n"
                 "Rate of coverage:\t> {}\n".format(seq_number, len(Product_seq_id),
                                                    round(float(len(Product_seq_id)) / seq_number, 2)))
         c.close()
 
 
 class Errors(object):
-    def __init__(self, primer_file, term_length=9, reference_file="", mismatch_num=1, term_threshold=4, bowtie="bowtie",
-                 PCR_product_size="150,2000", outfile="", nproc=10):
+    def __init__(self, primer_file, term_length=18, reference_file="", mismatch_num=1, term_threshold=4, bowtie="",
+                 PCR_product_size="150,2000", outfile="", nproc=10, targets="None"):
         #  If an attribute in a Python class does not want to be accessed externally,
         #  we can start with a double underscore (__) when naming the attribute,
         #  Then the attribute cannot be accessed with the original variable name, making it private.
         #  If an attribute is marked with "__xxxx_" Is defined, then it can be accessed externally.
         self.bowtie = bowtie
         self.term_threshold = term_threshold
         self.nproc = nproc
         self.term_len = term_length
         self.primer_file = primer_file
         self.reference_file = reference_file
         self.outfile = outfile
         self.PCR_size = PCR_product_size
         self.resQ = Manager().Queue()
         self.mismatch_num = mismatch_num
+        self.targets = targets
 
     @staticmethod
     def degenerate_seq(primer):
         seq = []
         cs = ""
         for s in primer:
             if s not in degenerate_base:
@@ -1444,16 +1431,20 @@
         term_list = defaultdict(list)
         seq_ID = defaultdict(list)
         with open(Input, "r") as f:
             for i in f:
                 if i.startswith(">"):
                     value = i.strip().lstrip(">")
                 else:
-                    key = i.strip()[-l:]
-                    term_list[key].append(value)
+                    if l == 0:
+                        key = i.strip()
+                        term_list[key].append(value)
+                    else:
+                        key = i.strip()[-l:]
+                        term_list[key].append(value)
 
         for k in term_list.keys():
             sequence = k
             term_set = set(term_list[k])
             Id = "_".join(list(term_set))
             expand_seq = self.degenerate_seq(sequence)
             if len(expand_seq) > 1:
@@ -1466,30 +1457,14 @@
         with open(Output, "w") as fo:
             for seq in seq_ID.keys():
                 # print(">" + '_'.join(seq_ID[seq]))
                 # print(seq)
                 fo.write(">" + '_'.join(seq_ID[seq]) + "\n" + seq + "\n")
         return seq_ID
 
-    def Bowtie_index(self, Input, method):
-        Bowtie_file = Path(Input).parent.joinpath("Bowtie_DB")
-        Bowtie_prefix = Path(Bowtie_file).joinpath(Path(Input).stem)
-        bowtie_cmd = method + "-build"
-        if Bowtie_file.exists():
-            size = os.listdir(Bowtie_file)
-            if not size:
-                print("No bowtie index found, start building ...")
-                os.system("{} {} {}".format(bowtie_cmd, Input, Bowtie_prefix))
-            else:
-                print("Bowtie index is OK.")
-                pass
-        else:
-            os.mkdir(Bowtie_file)
-            os.system("{} {} {}".format(bowtie_cmd, Input, Bowtie_prefix))
-
     def build_dict(self, Input):
         Input_dict = defaultdict(list)
         threshold = self.term_threshold
         with open(Input, "r") as f:
             position_pattern_1 = re.compile('MD:Z:(\w+)')
             position_pattern = re.compile("[A-Z]?(\d+)")
             for i in f:
@@ -1506,25 +1481,26 @@
                         pass
                     else:
                         Input_dict[gene].append([primer_match_start, primer])
         return Input_dict
 
     def bowtie_map(self):
         fa = Path(self.primer_file).parent.joinpath(Path(self.primer_file).stem).with_suffix(".term.fa")
-        ref_index = Path(self.reference_file).parent.joinpath("Bowtie_DB").joinpath(Path(self.reference_file).stem)
+        ref_index = self.reference_file
         out = Path(self.primer_file).parent.joinpath(Path(self.primer_file).stem).with_suffix(".sam")
         for_out = Path(self.primer_file).parent.joinpath(Path(self.primer_file).stem).with_suffix(".for.sam")
         rev_out = Path(self.primer_file).parent.joinpath(Path(self.primer_file).stem).with_suffix(".rev.sam")
         nproc = self.nproc
         if for_out.exists() and rev_out.exists():
             pass
         else:
             if re.search('bowtie2', self.bowtie):
                 os.system("{} -p {} -N {} -L 8 -a -x {} -f -U {} -S {}".format(self.bowtie, self.nproc,
-                                                                               self.mismatch_num, ref_index, fa, out))
+                                                                               self.mismatch_num, ref_index, fa,
+                                                                               out))
             elif re.search('bowtie', self.bowtie):
                 os.system(
                     "{} -p {} -f -n {} -l 8 -a --best --strata {} {} -S {}".format(self.bowtie, self.nproc,
                                                                                    self.mismatch_num, ref_index, fa,
                                                                                    out))
             else:
                 print("mapping software must be bowtie or bowtie2 !")
@@ -1586,15 +1562,14 @@
                             # still stored in that process. In fact, this variable in the main process is equivalent
                             # to not being modified. In order to synchronize the changes of other processes to the
                             # main process, you need to create variables that can be shared among multiple processes.
         self.resQ.put(None)
 
     def run(self):
         self.get_term()
-        self.Bowtie_index(self.reference_file, self.bowtie)
         self.bowtie_map()
         target_gene, forward_dict, reverse_dict = self.build_dict_run()
         p = ProcessPoolExecutor(self.nproc)
         for gene in target_gene:
             p.submit(self.PCR_product(gene, forward_dict, reverse_dict))
         # This will submit all tasks to one place without blocking, and then each
         # thread in the thread pool will fetch tasks.
@@ -1620,14 +1595,47 @@
                 primer_pair_acc[res[3] + "\t" + res[4]].append(res[0])
                 acc_id.add(res[0])
                 fo.write("\t".join(map(str, res)) + "\n")
                 # get results before shutdown. Synchronous call mode: call, wait for the return value, decouple,
                 # but slow.
         p.shutdown()
         primer_pair_id_sort = sorted(primer_pair_id.items(), key=lambda x: x[1], reverse=True)
+        target_seq = set()
         with open(self.outfile + ".pair.num", "w") as fo:
             fo.write("Primer_F\tPrimer_R\tPair_num\ttarget accession number\n")
             for k in primer_pair_id_sort:
                 primer_pair_acc_set = set(primer_pair_acc[k[0]])
+                target_seq = target_seq.union(primer_pair_acc_set)
                 fo.write(k[0] + "\t" + str(k[1]) + "\t" + str(len(primer_pair_acc_set)) + "\n")
         with open(self.outfile + ".total.acc.num", "w") as fo2:
-            fo2.write("total coverage of primer set (PS) is: {}".format(len(acc_id)))
+            fo2.write("total coverage of primer set (PS) is: {}\n".format(len(acc_id)))
+        if self.targets != "None":
+            with open(self.outfile + ".unmatched.fa", "w") as out:
+                raw_total_seq_dict = open(self.targets, "rb")
+                total_dict = pickle.load(raw_total_seq_dict)
+                print(len(set(total_dict.keys())), len(target_seq))
+                unmatched_seq_set = set(total_dict.keys()) - target_seq
+                with open(self.outfile + ".total.acc.num", "a+") as fo3:
+                    fo3.write("total target number is: {}\n".format(len(total_dict.keys())))
+                for unmatch in unmatched_seq_set:
+                    out.write(total_dict[unmatch])
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

### Comparing `multiPrime-2.4.3/src/utils.py` & `multiPrime-2.4.4/src/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,68 +265,81 @@
         parser.print_help()
         print("No output file provided !!!")
         sys.exit(1)
     return parser.parse_args()
 
 
 def Errors_argsParse():
-    parser = OptionParser('Usage: %prog Errors -i [input] -r [reference fasta] -l [150,2000] -p [10]-o [output]')
+    parser = OptionParser('Usage: %prog -i [input] -r [reference fasta] -l [150,2000] -p [10]-o [output]',
+                          version="%prog 0.0.8")
 
     parser.add_option('-i', '--input',
                       dest='input_file',
                       help='input file: primer.fa.')
 
     parser.add_option('-r', '--ref',
                       dest='ref',
-                      help='reference file: fasta format.')
+                      help='Reference file.The program will first search for Bowtie index files using the parameter '
+                           'you provided as the prefix.'
+                           'If the files are not found, it will build an index using the prefix you provided. '
+                           'else, the program will use the Bowtie index prefix you provided.')
 
     parser.add_option('-l', '--len',
                       dest='len',
-                      default=18,
+                      default=0,
                       type="int",
-                      help='Length of primer, which is used for mapping. Default: 18')
+                      help='Length of primer, which is used for mapping. '
+                           'If the length of the primer used for mapping is set to 0, '
+                           'the entire length of the primer will be utilized. '
+                           'Default: 0')
 
     parser.add_option('-t', '--term',
                       dest='term',
                       default=4,
                       type="int",
                       help='Position of mismatch is not allowed in the 3 term of primer. Default: 4')
 
     parser.add_option('-s', '--s',
                       dest='size',
-                      default="150,2000",
+                      default="100,1500",
                       type="str",
-                      help='Length of PCR product, default: 150,2000.')
+                      help='Length of PCR product, default: 100,1500.')
 
     parser.add_option('-p', '--proc',
                       dest='proc',
                       default="20",
                       type="int",
                       help='Number of process. Default: 20')
 
     parser.add_option('-b', '--bowtie',
                       dest='bowtie',
                       default="bowtie2",
                       type="string",
                       help='bowtie/ABS_path(bowtie) or bowtie2/ABS_path(bowtie2) was employed for mapping. '
-                           'Default: bowtie2 ')
+                           'Default: bowtie2')
 
     parser.add_option('-m', '--seedmms',
                       dest='seedmms',
                       default="1",
                       type="int",
                       help='Bowtie: Mismatches in seed (can be 0 - 3, default: -n 1).'
                            'Bowtie2: Gap or mismatches in seed (can be 0 - 1, default: -n 1).')
 
+    parser.add_option('-d', '--dict',
+                      dest='dict',
+                      default="None",
+                      help='Dictionary of targets sequences, binary format. '
+                           'It can be obtained from prepare_fa_pickle.py (https://github.com/joybio/multiPrime).')
+
     parser.add_option('-o', '--out',
                       dest='out',
-                      help='PCR product with primers.')
+                      help='Prodcut of PCR product with primers.')
 
     (options, args) = parser.parse_args()
-    if len(sys.argv) == 2:
+    if len(sys.argv) == 1:
         parser.print_help()
         sys.exit(1)
     elif options.input_file is None:
         parser.print_help()
         print("Input file must be specified !!!")
         sys.exit(1)
     elif options.ref is None:
@@ -336,15 +349,15 @@
     elif options.out is None:
         parser.print_help()
         print("No output file provided !!!")
         sys.exit(1)
     return parser.parse_args()
 
 def main_Usage():
-    print('Usage (version 2.3.7): \n'
+    print('Usage (version 2.4.4): \n'
           'multiPrime DPrime:  Degenerate primer design through MD-DPD or MD-EDPD.\n'
           'multiPrime Ppair:   Primer pair selection from the result of multiPrime DPrime.\n'
           'multiPrime Perfect: Extract primer-contained sequences with non-mismatches.\n'
           'multiPrime Errors:  Extract primer-contained sequences with errors.\n')
 
 
 degenerate_base = {"-": ["-"], "A": ["A"], "G": ["G"], "C": ["C"], "T": ["T"], "R": ["A", "G"], "Y": ["C", "T"],
```

