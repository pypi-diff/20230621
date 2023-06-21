# Comparing `tmp/snakemake_wrapper_utils-0.5.3.tar.gz` & `tmp/snakemake_wrapper_utils-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_wrapper_utils-0.5.3.tar", max compression
+gzip compressed data, was "snakemake_wrapper_utils-0.6.0.tar", max compression
```

## Comparing `snakemake_wrapper_utils-0.5.3.tar` & `snakemake_wrapper_utils-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1090 2023-03-22 07:42:44.686094 snakemake_wrapper_utils-0.5.3/LICENSE.md
--rw-r--r--   0        0        0      434 2023-03-22 07:43:02.382271 snakemake_wrapper_utils-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-22 07:42:44.686094 snakemake_wrapper_utils-0.5.3/snakemake_wrapper_utils/__init__.py
--rw-r--r--   0        0        0     5290 2023-03-22 07:42:44.686094 snakemake_wrapper_utils-0.5.3/snakemake_wrapper_utils/bcftools.py
--rw-r--r--   0        0        0     2608 2023-03-22 07:42:44.686094 snakemake_wrapper_utils-0.5.3/snakemake_wrapper_utils/java.py
--rw-r--r--   0        0        0     2635 2023-03-22 07:42:44.686094 snakemake_wrapper_utils-0.5.3/snakemake_wrapper_utils/samtools.py
--rw-r--r--   0        0        0      584 2023-03-22 07:42:44.686094 snakemake_wrapper_utils-0.5.3/snakemake_wrapper_utils/snakemake.py
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 snakemake_wrapper_utils-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-21 13:15:30.588173 snakemake_wrapper_utils-0.6.0/LICENSE.md
+-rw-r--r--   0        0        0      434 2023-06-21 13:15:47.388283 snakemake_wrapper_utils-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-21 13:15:30.588173 snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/__init__.py
+-rw-r--r--   0        0        0     5076 2023-06-21 13:15:30.588173 snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/bcftools.py
+-rw-r--r--   0        0        0     1638 2023-06-21 13:15:30.588173 snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/java.py
+-rw-r--r--   0        0        0     2761 2023-06-21 13:15:30.588173 snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/samtools.py
+-rw-r--r--   0        0        0      747 2023-06-21 13:15:30.588173 snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/snakemake.py
+-rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 snakemake_wrapper_utils-0.6.0/PKG-INFO
```

### Comparing `snakemake_wrapper_utils-0.5.3/LICENSE.md` & `snakemake_wrapper_utils-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `snakemake_wrapper_utils-0.5.3/snakemake_wrapper_utils/bcftools.py` & `snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/bcftools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+from snakemake_wrapper_utils.snakemake import get_mem, is_arg
 
 
 def infer_out_format(output, uncompressed_bcf=False):
     if output.endswith(".vcf"):
         return "v"
     elif output.endswith(".vcf.gz"):
         return "z"
@@ -30,118 +31,116 @@
     bcftools_opts = ""
     extra = snakemake.params.get("extra", "")
 
     ###############
     ### Threads ###
     ###############
     if parse_threads:
-        if "--threads" in extra:
+        if is_arg("--threads", extra):
             sys.exit(
                 "You have specified number of threads (`--threads`) in `params.extra`; please use `threads`."
             )
         bcftools_opts += (
             ""
             if snakemake.threads <= 1
             else "--threads {}".format(snakemake.threads - 1)
         )
 
     ######################
     ### Reference file ###
     ######################
     if parse_ref:
-        if "-f" in extra or "--fasta-ref" in extra:
+        if is_arg("-f", extra) or is_arg("--fasta-ref", extra):
             sys.exit(
                 "You have specified reference file (`-f/--fasta-ref`) in `params.extra`; this is automatically infered from the `ref` input file."
             )
 
         if snakemake.input.get("ref"):
             bcftools_opts += f" --fasta-ref {snakemake.input.ref}"
 
     ####################
     ### Regions file ###
     ####################
     if parse_regions:
-        if "--regions-file" in extra or "-R" in extra:
+        if is_arg("--regions-file", extra) or is_arg("-R", extra):
             sys.exit(
                 "You have specified regions file (`-R/--regions-file`) in `params.extra`; this is automatically infered from the `regions` input file."
             )
 
         if snakemake.input.get("regions"):
             if not snakemake.input.get("index"):
                 sys.exit(
-                    "You have specified a `regions=` file in `input:`; this implies the `--regions-file` option of bcftools and thus also requires an `index=` file specified in the `input:`, but none was found."
+                    "You have specified a `regions` file in `input:`; this implies the `--regions-file` option of bcftools and thus also requires an `index=` file specified in the `input:`, but none was found."
                 )
             bcftools_opts += f" --regions-file {snakemake.input.regions}"
 
     ####################
     ### Samples file ###
     ####################
     if parse_samples:
-        if "-S" in extra or "--samples-file" in extra:
+        if is_arg("-S", extra) or is_arg("--samples-file", extra):
             sys.exit(
                 "You have specified samples file (`-S/--samples-file`) in `params.extra`; this is automatically infered from the `samples` input file."
             )
 
         if snakemake.input.get("samples"):
             bcftools_opts += f" --samples-file {snakemake.input.samples}"
 
     ####################
     ### Targets file ###
     ####################
     if parse_targets:
-        if "-T" in extra or "--targets-file" in extra:
+        if is_arg("-T", extra) or is_arg("--targets-file", extra):
             sys.exit(
                 "You have specified targets file (`-T/--targets-file`) in `params.extra`; this is automatically infered from the `targets` input file."
             )
 
         if snakemake.input.get("targets"):
             bcftools_opts += f" --targets-file {snakemake.input.targets}"
 
     ###################
     ### Output file ###
     ###################
     if parse_output:
-        if "-o" in extra or "--output" in extra:
+        if is_arg("-o", extra) or is_arg("--output", extra):
             sys.exit(
                 "You have specified output file (`-o/--output`) in `params.extra`; this is automatically infered from the first output file."
             )
         bcftools_opts += f" --output {snakemake.output[0]}"
 
     #####################
     ### Output format ###
     #####################
     if parse_output_format:
-        if "-O" in extra or "--output-type" in extra:
+        if is_arg("-O", extra) or is_arg("--output-type", extra):
             sys.exit(
                 "You have specified output format (`-O/--output-type`) in `params.extra`; this is automatically infered from output file extension."
             )
 
         out_format = infer_out_format(
             snakemake.output[0], snakemake.params.get("uncompressed_bcf", False)
         )
         bcftools_opts += f" --output-type {out_format}"
 
     ##############
     ### Memory ###
     ##############
     if parse_memory:
-        if "-m" in extra or "--max-mem" in extra:
+        if is_arg("-m", extra) or is_arg("--max-mem", extra):
             sys.exit(
                 "You have provided `-m/--max-mem` in `params.extra`; please use `resources.mem_mb`."
             )
-        # Getting memory in megabytes, as advised in documentation.
-        if "mem_mb" in snakemake.resources.keys():
-            bcftools_opts += " --max-mem {}M".format(snakemake.resources["mem_mb"])
-        # Getting memory in gigabytes, for user convenience. Please prefer the use
-        # of mem_mb over mem_gb as advised in documentation.
-        elif "mem_gb" in snakemake.resources.keys():
-            bcftools_opts += " --max-mem {}G".format(snakemake.resources["mem_gb"])
+        bcftools_opts += " --max-mem {}M".format(get_mem(snakemake))
 
     ################
     ### Temp dir ###
     ################
-    if "-T" in extra or "--temp-dir" in extra or "--temp-prefix" in extra:
+    if (
+        is_arg("-T", extra)
+        or is_arg("--temp-dir", extra)
+        or is_arg("--temp-prefix", extra)
+    ):
         sys.exit(
             "You have provided `-T/--temp-dir/--temp-prefix` in `params.extra`; please use the `tmpdir` resource."
         )
 
     return bcftools_opts
```

### Comparing `snakemake_wrapper_utils-0.5.3/snakemake_wrapper_utils/samtools.py` & `snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/samtools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,85 @@
 import sys
 from os import path
+from snakemake_wrapper_utils.snakemake import is_arg
 
 
 def infer_out_format(file_name):
     out_name, out_ext = path.splitext(file_name)
     return out_ext[1:].upper()
 
 
 def get_samtools_opts(
     snakemake,
     parse_threads=True,
     parse_ref=True,
     parse_write_index=True,
     parse_output=True,
     parse_output_format=True,
+    param_name="extra",
 ):
     """Obtain samtools_opts from output, params, and handle resource definitions in resources."""
     samtools_opts = ""
-    extra = snakemake.params.get("extra", "")
+    extra = snakemake.params.get(param_name, "")
     idx = snakemake.output.get("idx", "")
 
     ###############
     ### Threads ###
     ###############
     if parse_threads:
-        if "-@" in extra or "--threads" in extra:
+        if is_arg("-@", extra) or is_arg("--threads", extra):
             sys.exit(
-                "You have specified number of threads (`-@/--threads`) in params.extra; please use only `threads`."
+                "You have specified number of threads (`-@/--threads`) in `params.extra`; please use only `threads`."
             )
         samtools_opts += (
             ""
             if snakemake.threads <= 1
             else " --threads {}".format(snakemake.threads - 1)
         )
 
     ######################
     ### Reference file ###
     ######################
     if parse_ref:
-        if "--reference" in extra:
+        if is_arg("--reference", extra):
             sys.exit(
-                "You have specified reference file (`--reference`) in `params.extra`; this is automatically infered from the `ref` input file."
+                "You have specified reference file (`--reference`) in `params.extra`; this is automatically infered from `ref` input file."
             )
 
         if snakemake.input.get("ref"):
             samtools_opts += f" --reference {snakemake.input.ref}"
 
     ###################
     ### Write index ###
     ###################
     if parse_write_index:
-        if "--write-index" in extra:
+        if is_arg("--write-index", extra):
             sys.exit(
-                "You have specified writing index (`--write-index`) in params.extra; this is automatically infered from `idx` output file."
+                "You have specified writing index (`--write-index`) in `params.extra`; this is automatically infered from `idx` output file."
             )
         if idx:
             samtools_opts += " --write-index"
 
     ###################
     ### Output file ###
     ###################
     if parse_output:
-        if "-o" in extra:
+        if is_arg("-o", extra):
             sys.exit(
-                "You have specified output file (`-o`) in params.extra; this is automatically infered from the first output file."
+                "You have specified output file (`-o`) in `params.extra`; this is automatically infered from the first output file."
             )
         samtools_opts += f" -o {snakemake.output[0]}"
         if idx:
             samtools_opts += f"##idx##{idx}"
 
     #####################
     ### Output format ###
     #####################
     if parse_output_format:
-        if "-O" in extra or "--output-fmt" in extra:
+        if is_arg("-O", extra) or is_arg("--output-fmt", extra):
             sys.exit(
-                "You have specified output format (`-O/--output-fmt`) in params.extra; this is automatically infered from output file extension."
+                "You have specified output format (`-O/--output-fmt`) in `params.extra`; this is automatically infered from output file extension."
             )
         out_ext = infer_out_format(snakemake.output[0])
         samtools_opts += f" --output-fmt {out_ext}"
 
     return samtools_opts
```

### Comparing `snakemake_wrapper_utils-0.5.3/snakemake_wrapper_utils/snakemake.py` & `snakemake_wrapper_utils-0.6.0/snakemake_wrapper_utils/snakemake.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,7 +13,15 @@
         return mem_mb * 1024
     elif out_unit == "MiB":
         return mem_mb
     elif out_unit == "GiB":
         return mem_mb / 1024
     else:
         raise valueError("invalid output unit. Only KiB, MiB and GiB supported.")
+
+
+def is_arg(arg, cmd):
+    """Check command for the presence of argument"""
+    if arg in cmd.replace("=", " ").split(" "):
+        return True
+
+    return False
```

### Comparing `snakemake_wrapper_utils-0.5.3/PKG-INFO` & `snakemake_wrapper_utils-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-wrapper-utils
-Version: 0.5.3
+Version: 0.6.0
 Summary: A collection of utils for Snakemake wrappers.
 License: MIT
 Author: Johannes Köster
 Author-email: johannes.koester@tu-dortmund.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

