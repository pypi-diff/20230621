# Comparing `tmp/scanRBP-0.1.4.tar.gz` & `tmp/scanRBP-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanRBP-0.1.4.tar", last modified: Tue Jun 13 13:29:47 2023, max compression
+gzip compressed data, was "scanRBP-0.1.5.tar", last modified: Wed Jun 21 14:34:36 2023, max compression
```

## Comparing `scanRBP-0.1.4.tar` & `scanRBP-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-13 13:29:47.967780 scanRBP-0.1.4/
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     4936 2023-06-13 13:29:47.967057 scanRBP-0.1.4/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     4606 2023-06-08 12:22:17.000000 scanRBP-0.1.4/README.md
-drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-13 13:29:47.961959 scanRBP-0.1.4/scanRBP/
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      507 2023-05-09 14:06:00.000000 scanRBP-0.1.4/scanRBP/__init__.py
-drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-13 13:29:47.965434 scanRBP-0.1.4/scanRBP/config/
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1478 2023-06-13 13:24:29.000000 scanRBP-0.1.4/scanRBP/config/__init__.py
-drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-13 13:29:47.966075 scanRBP-0.1.4/scanRBP/database/
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      795 2023-05-16 12:49:53.000000 scanRBP-0.1.4/scanRBP/database/__init__.py
-drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-13 13:29:47.966464 scanRBP-0.1.4/scanRBP/pwm/
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1465 2023-05-10 10:55:50.000000 scanRBP-0.1.4/scanRBP/pwm/__init__.py
--rwxrwxr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     8939 2023-06-13 13:24:47.000000 scanRBP-0.1.4/scanRBP/scanRBP
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      104 2023-05-09 11:28:18.000000 scanRBP-0.1.4/scanRBP/scanRBP.config.example
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        6 2023-06-13 13:29:28.000000 scanRBP-0.1.4/scanRBP/version
-drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-13 13:29:47.964789 scanRBP-0.1.4/scanRBP.egg-info/
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     4936 2023-06-13 13:29:47.962392 scanRBP-0.1.4/scanRBP.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      365 2023-06-13 13:29:47.962773 scanRBP-0.1.4/scanRBP.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        1 2023-06-13 13:29:47.963232 scanRBP-0.1.4/scanRBP.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        1 2023-05-09 11:24:46.000000 scanRBP-0.1.4/scanRBP.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)       41 2023-06-13 13:29:47.964386 scanRBP-0.1.4/scanRBP.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        8 2023-06-13 13:29:47.964865 scanRBP-0.1.4/scanRBP.egg-info/top_level.txt
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)       38 2023-06-13 13:29:47.967896 scanRBP-0.1.4/setup.cfg
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1041 2023-04-28 08:24:39.000000 scanRBP-0.1.4/setup.py
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-21 14:34:36.482974 scanRBP-0.1.5/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     4936 2023-06-21 14:34:36.482567 scanRBP-0.1.5/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     4606 2023-06-08 12:22:17.000000 scanRBP-0.1.5/README.md
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-21 14:34:36.477595 scanRBP-0.1.5/scanRBP/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      507 2023-05-09 14:06:00.000000 scanRBP-0.1.5/scanRBP/__init__.py
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-21 14:34:36.481079 scanRBP-0.1.5/scanRBP/config/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1478 2023-06-13 13:24:29.000000 scanRBP-0.1.5/scanRBP/config/__init__.py
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-21 14:34:36.481498 scanRBP-0.1.5/scanRBP/database/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      795 2023-05-16 12:49:53.000000 scanRBP-0.1.5/scanRBP/database/__init__.py
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-21 14:34:36.482128 scanRBP-0.1.5/scanRBP/pwm/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1465 2023-05-10 10:55:50.000000 scanRBP-0.1.5/scanRBP/pwm/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     9183 2023-06-21 08:36:55.000000 scanRBP-0.1.5/scanRBP/scanRBP
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      104 2023-05-09 11:28:18.000000 scanRBP-0.1.5/scanRBP/scanRBP.config.example
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        6 2023-06-21 14:34:18.000000 scanRBP-0.1.5/scanRBP/version
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-21 14:34:36.480652 scanRBP-0.1.5/scanRBP.egg-info/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     4936 2023-06-21 14:34:36.478070 scanRBP-0.1.5/scanRBP.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      365 2023-06-21 14:34:36.478426 scanRBP-0.1.5/scanRBP.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        1 2023-06-21 14:34:36.478961 scanRBP-0.1.5/scanRBP.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        1 2023-05-09 11:24:46.000000 scanRBP-0.1.5/scanRBP.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)       41 2023-06-21 14:34:36.480346 scanRBP-0.1.5/scanRBP.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        8 2023-06-21 14:34:36.480739 scanRBP-0.1.5/scanRBP.egg-info/top_level.txt
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)       38 2023-06-21 14:34:36.483064 scanRBP-0.1.5/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1041 2023-04-28 08:24:39.000000 scanRBP-0.1.5/setup.py
```

### Comparing `scanRBP-0.1.4/PKG-INFO` & `scanRBP-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanRBP
-Version: 0.1.4
+Version: 0.1.5
 Summary: scanRBP: RNA-protein binding toolkit
 Home-page: https://github.com/grexor/scanRBP
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: scanRBP,bioinformatics,RBP,RNA-protein binding,toolkit
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `scanRBP-0.1.4/README.md` & `scanRBP-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `scanRBP-0.1.4/scanRBP/config/__init__.py` & `scanRBP-0.1.5/scanRBP/config/__init__.py`

 * *Files identical despite different names*

### Comparing `scanRBP-0.1.4/scanRBP/database/__init__.py` & `scanRBP-0.1.5/scanRBP/database/__init__.py`

 * *Files identical despite different names*

### Comparing `scanRBP-0.1.4/scanRBP/pwm/__init__.py` & `scanRBP-0.1.5/scanRBP/pwm/__init__.py`

 * *Files identical despite different names*

### Comparing `scanRBP-0.1.4/scanRBP/scanRBP` & `scanRBP-0.1.5/scanRBP/scanRBP`

 * *Files 3% similar despite different names*

```diff
@@ -47,27 +47,29 @@
     * returns list of proteins available matching search_term
 
 Options:
      -annotate                Annotate each heatmap cell with the number
      -xlabels                 Display sequence (x-labels), default False
      -protein TARDBP.K562.00  Only analyze binding for the provided protein (default: analyze binding for all proteins in scanRBP database)
      -figsize "(10,20)"       Change matplotlib/seaborn figure size for the heatmap, example width=10, height=20
+     -fontscale               Change font scale, default 0.2
      -heatmap title           Make heatmap (png+pdf) with title
      -output_folder folder    Store all results to the output folder (default: current folder)
      -nonzero                 All negative vector values are set to 0, not enabled by default
      -CLIP                    Use actual CLIP data, do not use PWM
 """
 
 parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter, add_help=False)
 parser.add_argument('commands', help="command(s) to run", nargs='*')
 parser.add_argument("-help", "-h", "--help", action="store_true")
 parser.add_argument("-annotate", "--annotate", action="store_true", default=False)
 parser.add_argument("-xlabels", "--xlabels", action="store_true", default=False)
 parser.add_argument("-protein", "--protein", default=False)
 parser.add_argument("-figsize", "--figsize", default=False)
+parser.add_argument("-fontscale", "--fontscale", default=0.2, type=float)
 parser.add_argument("-title", "--title", default=False)
 parser.add_argument("-matrix", "--matrix", action="store_true", default=True)
 parser.add_argument("-CLIP", "--CLIP", action="store_true", default=False)
 parser.add_argument("-nonzero", "--nonzero", action="store_true", default=False)
 parser.add_argument("-heatmap", "--heatmap", default=False)
 parser.add_argument("-output_folder", "--output_folder", default=".")
 parser.add_argument("-version", "--version", help="Print version", action="store_true")
@@ -118,15 +120,15 @@
     if strand=="-":
         heatmap_rows.reverse()
     basename = output_fname.replace(".png", "").replace(".pdf", "")
     data = pandas.DataFrame(heatmap_data, index=heatmap_columns, columns=heatmap_rows)
     data.to_csv(args.output_folder+"/"+basename+"_CLIP.tab", sep="\t")
 
 
-def process(seq, output_fname, args):
+def process(seq, output_fname, args, title=None):
     heatmap_data = []
     heatmap_columns = []
 
     for scan_id, pssm in scanRBP.pwm.pssm.items():
         if args.protein: # only process a specific protein?
             if scan_id not in args.protein:
                 continue
@@ -146,15 +148,15 @@
     basename = output_fname.replace(".png", "").replace(".pdf", "")
     data = pandas.DataFrame(heatmap_data, index=heatmap_columns, columns=heatmap_rows)
     data.to_csv(args.output_folder+"/"+basename+"_PWM.tab", sep="\t")
 
     if args.heatmap!=False:
         plt.figure()
         sns.set(font="Arial")
-        sns.set(font_scale=0.4)
+        sns.set(font_scale=args.fontscale)
         sns.set_style("dark")
         sns.set_style("ticks")
 
         rdgn = sns.diverging_palette(h_neg=130, h_pos=10, s=99, l=55, sep=3, as_cmap=True)
         optional_params = {"linewidths":0.0}
         optional_params["col_cluster"] = False
         optional_params["annot"] = args.annotate
@@ -166,15 +168,18 @@
         optional_params["cbar_pos"] = None
 
         if args.figsize!=False:
             optional_params["figsize"] = eval(args.figsize)
         fig = sns.clustermap(data, **optional_params)
         fig.ax_col_dendrogram.set_visible(False)
 
-        plt.title(args.heatmap)
+        if title==None:
+            plt.title(args.heatmap)
+        else:
+            plt.title(title)
         plt.tight_layout() 
         plt.savefig(args.output_folder+"/"+basename+".png", dpi=300)
         plt.savefig(args.output_folder+"/"+basename+".pdf")
         plt.close()
 
 if len(args.commands)>0:
 
@@ -203,23 +208,23 @@
         sys.exit(0)
 
     if args.commands[0].lower().endswith(".fasta") or args.commands[0].lower().endswith(".fa"):
         import pybio
         data = pybio.data.Fasta(args.commands[0])
         while data.read():
             id = data.id.lstrip(" ")
-            id = id.split(" ")[0].replace("+", "plus").replace("-", "minus")
-            id_records = id.replace("plus", "+").replace("minus", "-").split("_")
-            chrstrand, start, stop = "_".join(id_records[:-2]), id_records[-2], id_records[-1] # chr name can have _ inside
-            start, stop = int(start), int(stop)
-            chr, strand = chrstrand[:-1], chrstrand[-1]
+            #id = id.split(" ")[0].replace("+", "plus").replace("-", "minus")
+            #id_records = id.replace("plus", "+").replace("minus", "-").split("_")
+            #chrstrand, start, stop = "_".join(id_records[:-2]), id_records[-2], id_records[-1] # chr name can have _ inside
+            #start, stop = int(start), int(stop)
+            #chr, strand = chrstrand[:-1], chrstrand[-1]
             seq = data.sequence
             # TODO
             #process_CLIP(chr, strand, start, stop, id)
-            process(seq, id, args)
+            process(seq, id, args, title=id)
     elif args.commands[0]=="bed":
         make_bedgraph()
     else:
         if len(args.commands)>=2:
             process(args.commands[0], args.commands[1], args)
         else:
             print(help_0)
```

### Comparing `scanRBP-0.1.4/scanRBP.egg-info/PKG-INFO` & `scanRBP-0.1.5/scanRBP.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanRBP
-Version: 0.1.4
+Version: 0.1.5
 Summary: scanRBP: RNA-protein binding toolkit
 Home-page: https://github.com/grexor/scanRBP
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: scanRBP,bioinformatics,RBP,RNA-protein binding,toolkit
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `scanRBP-0.1.4/setup.py` & `scanRBP-0.1.5/setup.py`

 * *Files identical despite different names*

