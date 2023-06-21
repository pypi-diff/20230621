# Comparing `tmp/dwiqc-0.4.6-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.4.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 24429 bytes, number of entries: 22
+Zip file size: 24503 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      225 b- defN 23-Jun-08 18:05 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-Jun-20 14:26 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-21 12:23 dwiqc/__version__.py
 -rw-r--r--  2.0 unx     1352 b- defN 23-Jun-08 18:05 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       61 b- defN 23-Jun-12 14:27 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-Jun-08 18:05 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     5989 b- defN 23-Jun-08 18:05 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx     3801 b- defN 23-Jun-12 20:46 dwiqc/cli/tandem.py
 -rw-r--r--  2.0 unx      160 b- defN 23-Jun-08 18:05 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-Jun-08 18:05 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-Jun-08 18:05 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-Jun-08 18:05 dwiqc/tasks/__init__.py
 -rw-r--r--  2.0 unx    10168 b- defN 23-Jun-08 18:05 dwiqc/tasks/prequal.py
--rw-r--r--  2.0 unx     4415 b- defN 23-Jun-08 18:05 dwiqc/tasks/prequal_EQ.py
+-rw-r--r--  2.0 unx     4656 b- defN 23-Jun-21 11:45 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     6146 b- defN 23-Jun-08 18:05 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3872 b- defN 23-Jun-08 18:05 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    13083 b- defN 23-Jun-08 18:05 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     5783 b- defN 23-Jun-20 14:27 dwiqc-0.4.6.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-20 14:27 dwiqc-0.4.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      428 b- defN 23-Jun-20 14:27 dwiqc-0.4.6.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-20 14:27 dwiqc-0.4.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-20 14:27 dwiqc-0.4.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-20 14:27 dwiqc-0.4.6.dist-info/RECORD
-22 files, 68020 bytes uncompressed, 21677 bytes compressed:  68.1%
+-rwxr-xr-x  2.0 unx     5783 b- defN 23-Jun-21 12:24 dwiqc-0.4.7.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-21 12:24 dwiqc-0.4.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      428 b- defN 23-Jun-21 12:24 dwiqc-0.4.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-21 12:24 dwiqc-0.4.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-21 12:24 dwiqc-0.4.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-21 12:24 dwiqc-0.4.7.dist-info/RECORD
+22 files, 68261 bytes uncompressed, 21751 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.4.6.data/scripts/dwiQC.py
+Filename: dwiqc-0.4.7.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.4.6.dist-info/LICENSE
+Filename: dwiqc-0.4.7.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.4.6.dist-info/METADATA
+Filename: dwiqc-0.4.7.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.4.6.dist-info/WHEEL
+Filename: dwiqc-0.4.7.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.4.6.dist-info/top_level.txt
+Filename: dwiqc-0.4.7.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.4.6.dist-info/RECORD
+Filename: dwiqc-0.4.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.4.6'
+__version__ = '0.4.7'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/tasks/prequal_EQ.py

```diff
@@ -52,14 +52,23 @@
 				if 'slspec' in file and file.endswith('.txt'):
 					spec_file = file
 		except FileNotFoundError:
 			logging.error('spec file not found. exiting.')
 			sys.exit()
 
 
+		# rename all the eddy_results files to be {self._sub}_{self._ses}
+
+		for file in os.listdir():
+			if file.startswith("eddy_results"):
+				new_name = file.replace("eddy_results", f"{self._sub}_{self._ses}")
+				os.rename(file, new_name)
+
+
+
 		eddy_quad = f"""singularity exec \
 		-B /n/home_fasse/dasay/eddy_quad_mofication/quad_mot.py:/APPS/fsl/fslpython/envs/fslpython/lib/python3.7/site-packages/eddy_qc/QUAD/quad_mot.py \
 		/n/sw/ncf/containers/masilab/prequal/1.0.8/prequal.sif \
 		/APPS/fsl/bin/eddy_quad \
 		{self._sub}_{self._ses} \
 		-idx index.txt \
 		-par acqparams.txt \
```

## Comparing `dwiqc-0.4.6.data/scripts/dwiQC.py` & `dwiqc-0.4.7.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.4.6.dist-info/LICENSE` & `dwiqc-0.4.7.dist-info/LICENSE`

 * *Files identical despite different names*

