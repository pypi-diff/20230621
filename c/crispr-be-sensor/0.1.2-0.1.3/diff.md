# Comparing `tmp/crispr_be_sensor-0.1.2.tar.gz` & `tmp/crispr_be_sensor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispr_be_sensor-0.1.2.tar", max compression
+gzip compressed data, was "crispr_be_sensor-0.1.3.tar", max compression
```

## Comparing `crispr_be_sensor-0.1.2.tar` & `crispr_be_sensor-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      131 2023-06-21 19:44:21.779087 crispr_be_sensor-0.1.2/crispr_be_sensor/__init__.py
--rw-r--r--   0        0        0    16830 2023-06-21 19:01:21.773413 crispr_be_sensor-0.1.2/crispr_be_sensor/_demultiplex.py
--rw-r--r--   0        0        0     1260 2023-06-21 19:10:53.906974 crispr_be_sensor-0.1.2/crispr_be_sensor/_visualization.py
--rw-r--r--   0        0        0      491 2023-06-21 19:44:33.332198 crispr_be_sensor-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 16:11:00.997989 crispr_be_sensor-0.1.2/README.md
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 crispr_be_sensor-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      131 2023-06-21 19:44:21.779087 crispr_be_sensor-0.1.3/crispr_be_sensor/__init__.py
+-rw-r--r--   0        0        0    16894 2023-06-21 19:47:15.511500 crispr_be_sensor-0.1.3/crispr_be_sensor/_demultiplex.py
+-rw-r--r--   0        0        0     1260 2023-06-21 19:10:53.906974 crispr_be_sensor-0.1.3/crispr_be_sensor/_visualization.py
+-rw-r--r--   0        0        0      491 2023-06-21 19:47:26.700361 crispr_be_sensor-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 16:11:00.997989 crispr_be_sensor-0.1.3/README.md
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 crispr_be_sensor-0.1.3/PKG-INFO
```

### Comparing `crispr_be_sensor-0.1.2/crispr_be_sensor/_demultiplex.py` & `crispr_be_sensor-0.1.3/crispr_be_sensor/_demultiplex.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 # EXPORT IN __init__.py
 ##
 # sample_indices_df_subset: DATAFRAME CONTAINING i5_INDEX DEMULTIPLEX SAMPLES - Must contain column "sub_library_name", "i5_index"
 # sample_pooling_df_subset: DATAFREAME CONTAINING U6PE1_BARCODE DEMULTIPLE SAMMPLES - Must contain column "i5_index" and U6PE1_Barcode
 ##
-def main_perform_demultiplex(read_demultiplex_strategy: ReadDemultiplexStrategy, data_root_dir:str, sample_sub_dirs: List[str], sample_indices_df_subset: pd.Dataframe, sample_pooling_df_subset: pd.Dataframe, read_cores: int = 1):
+def main_perform_demultiplex(read_demultiplex_strategy: ReadDemultiplexStrategy, data_root_dir:str, sample_sub_dirs: List[str], sample_indices_df_subset: pd.DataFrame, sample_pooling_df_subset: pd.DataFrame, read_cores: int = 1):
     
     # Start by creating the directory for the demultiplexed FASTQS
     if not os.path.exists(read_demultiplex_strategy.output_dir):
         os.makedirs(read_demultiplex_strategy.output_dir)
 
 
     #def process_sample_subdir(sample_sub_dir, read_demultiplex_strategy, sample_indices_df_subset, sample_pooling_df_subset):
@@ -52,15 +52,15 @@
         n_processes = min(len(sample_sub_dirs)+1, read_cores)
         with multiprocessing.Pool(processes=n_processes) as pool:
             _ = pool.map(process_sample_subdir_p, sample_sub_dirs)
 
 
 
 # EXPORT IN __init__.py
-def main_perform_demultiplex_qc(sample_sub_dirs, read_demultiplex_strategy, sample_indices_df_subset, sample_pooling_df_subset, read_cores: int = 1) -> dict:
+def main_perform_demultiplex_qc(sample_sub_dirs: List[str], read_demultiplex_strategy: ReadDemultiplexStrategy, sample_indices_df_subset: pd.DataFrame, sample_pooling_df_subset: pd.DataFrame, read_cores: int = 1) -> dict:
     
     ###
     ### Get counts of unrecognized barcodes
     ###
     process_demultiplex_qc_p = partial(process_demultiplex_qc, read_demultiplex_strategy=read_demultiplex_strategy, sample_indices_df_subset=sample_indices_df_subset, sample_pooling_df_subset=sample_pooling_df_subset)
     unique_barcode_counts_list = None
     if read_cores == 1:
```

### Comparing `crispr_be_sensor-0.1.2/crispr_be_sensor/_visualization.py` & `crispr_be_sensor-0.1.3/crispr_be_sensor/_visualization.py`

 * *Files identical despite different names*

### Comparing `crispr_be_sensor-0.1.2/PKG-INFO` & `crispr_be_sensor-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crispr-be-sensor
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Basheer Becerra
 Author-email: bbecerr@outlook.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

