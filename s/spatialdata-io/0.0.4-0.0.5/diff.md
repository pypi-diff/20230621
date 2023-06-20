# Comparing `tmp/spatialdata_io-0.0.4.tar.gz` & `tmp/spatialdata_io-0.0.5.tar.gz`

## Comparing `spatialdata_io-0.0.4.tar` & `spatialdata_io-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,51 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.bumpversion.cfg
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.codecov.yaml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.editorconfig
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.flake8
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.mypy.ini
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.readthedocs.yaml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/_version.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.github/workflows/test_and_deploy.yaml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/Makefile
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/changelog.md
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/conf.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/contributing.md
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/index.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/make.bat
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/references.md
--rw-r--r--   0        0        0    16386 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/template_usage.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/extensions/.gitkeep
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/_docs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/_constants/__init__.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/_constants/_constants.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/_constants/_enum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/__init__.py
--rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/cosmx.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/curio.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/mcmicro.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/metaspace.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/resolve.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/steinbock.py
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/visium.py
--rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/xenium.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/_utils/__init__.py
--rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/_utils/_read_10x_h5.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/src/spatialdata_io/readers/_utils/_utils.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/tests/test_basic.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/LICENSE
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/README.md
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 spatialdata_io-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.bumpversion.cfg
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.codecov.yaml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.editorconfig
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.flake8
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.mypy.ini
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/_version.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.github/workflows/test_and_deploy.yaml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/Makefile
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/changelog.md
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/conf.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/contributing.md
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/index.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/make.bat
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/references.md
+-rw-r--r--   0        0        0    16386 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/template_usage.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/extensions/.gitkeep
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/_docs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/_constants/__init__.py
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/_constants/_constants.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/_constants/_enum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/__init__.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/codex.py
+-rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/cosmx.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/curio.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/mcmicro.py
+-rw-r--r--   0        0        0     7492 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/merscope.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/metaspace.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/resolve.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/steinbock.py
+-rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/visium.py
+-rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/xenium.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/_utils/__init__.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/_utils/_read_10x_h5.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/_utils/_utils.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/tests/test_basic.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/README.md
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/PKG-INFO
```

### Comparing `spatialdata_io-0.0.4/.flake8` & `spatialdata_io-0.0.5/.flake8`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/.mypy.ini` & `spatialdata_io-0.0.5/.mypy.ini`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/.pre-commit-config.yaml` & `spatialdata_io-0.0.5/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -11,29 +11,29 @@
       hooks:
           - id: black
     - repo: https://github.com/pre-commit/mirrors-prettier
       rev: v3.0.0-alpha.9-for-vscode
       hooks:
           - id: prettier
     - repo: https://github.com/asottile/blacken-docs
-      rev: 1.13.0
+      rev: 1.14.0
       hooks:
           - id: blacken-docs
     - repo: https://github.com/PyCQA/isort
       rev: 5.12.0
       hooks:
           - id: isort
     - repo: https://github.com/pre-commit/mirrors-mypy
-      rev: v1.2.0
+      rev: v1.3.0
       hooks:
           - id: mypy
             additional_dependencies: [numpy]
             exclude: docs/
     - repo: https://github.com/asottile/yesqa
-      rev: v1.4.0
+      rev: v1.5.0
       hooks:
           - id: yesqa
             additional_dependencies:
                 - flake8-tidy-imports
                 - flake8-docstrings
                 - flake8-rst-docstrings
                 - flake8-comprehensions
@@ -66,15 +66,15 @@
                 - flake8-tidy-imports
                 - flake8-docstrings
                 - flake8-rst-docstrings
                 - flake8-comprehensions
                 - flake8-bugbear
                 - flake8-blind-except
     - repo: https://github.com/asottile/pyupgrade
-      rev: v3.3.2
+      rev: v3.7.0
       hooks:
           - id: pyupgrade
             args: [--py3-plus, --py39-plus, --keep-runtime-typing]
     - repo: local
       hooks:
           - id: forbid-to-commit
             name: Don't commit rej files
```

### Comparing `spatialdata_io-0.0.4/.github/workflows/build.yaml` & `spatialdata_io-0.0.5/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/.github/workflows/test_and_deploy.yaml` & `spatialdata_io-0.0.5/.github/workflows/test_and_deploy.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/docs/Makefile` & `spatialdata_io-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/docs/conf.py` & `spatialdata_io-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/docs/contributing.md` & `spatialdata_io-0.0.5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/docs/make.bat` & `spatialdata_io-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/docs/references.bib` & `spatialdata_io-0.0.5/docs/references.bib`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/docs/template_usage.md` & `spatialdata_io-0.0.5/docs/template_usage.md`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/docs/_templates/autosummary/class.rst` & `spatialdata_io-0.0.5/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/docs/extensions/typed_returns.py` & `spatialdata_io-0.0.5/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/src/spatialdata_io/_docs.py` & `spatialdata_io-0.0.5/src/spatialdata_io/_docs.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/src/spatialdata_io/_constants/_constants.py` & `spatialdata_io-0.0.5/src/spatialdata_io/_constants/_constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,41 @@
 from enum import unique
 
 from spatialdata_io._constants._enum import ModeEnum
 
 
 @unique
+class CodexKeys(ModeEnum):
+    """Keys for *CODEX* formatted dataset."""
+
+    # files and directories
+    FCS_FILE = ".fcs"
+    FCS_FILE_CSV = ".csv"
+    # metadata
+    REGION_KEY = "region"
+    INSTANCE_KEY = "cell_id"
+    SPATIAL_KEY = "spatial"
+    # images
+    IMAGE_TIF = ".tif"
+
+
 class CurioKeys(ModeEnum):
     """Keys for *Curio* formatted dataset."""
 
     # files and directories
-    ANNDATA_FILE = ".h5ad"
+    ANNDATA_FILE = "anndata.h5ad"
     CLUSTER_ASSIGNMENT = "cluster_assignment.txt"
     METRICS_FILE = "Metrics.csv"
     VAR_FEATURES_CLUSTERS = "variable_features_clusters.txt"
-    VAR_FEATURES_MORANSI = "variable_features_moransi.txt"
+    VAR_FEATURES_MORANSI = "variable_features_spatial_moransi.txt"
     # metadata
     CATEGORY = "Category"
+    REGION = "cells"
+    REGION_KEY = "region"
+    INSTANCE_KEY = "instance_id"
     TOP_CLUSTER_DEFINING_FEATURES = "Top_cluster_defining_features"
 
 
 @unique
 class CosmxKeys(ModeEnum):
     """Keys for *Nanostring Cosmx* formatted dataset."""
 
@@ -86,24 +103,23 @@
 
     # files and directories
     COUNTS_FILE = "filtered_feature_bc_matrix.h5"
 
     # images
     IMAGE_HIRES_FILE = "spatial/tissue_hires_image.png"
     IMAGE_LOWRES_FILE = "spatial/tissue_lowres_image.png"
-    IMAGE_TIF_SUFFIX = "_tissue_image.tif"
-    IMAGE_TIF_ALTERNATIVE_SUFFIX = "_image.tif"
 
     # scalefactors
-    SCALEFACTORS_FILE = "spatial/scalefactors_json.json"
+    SCALEFACTORS_FILE = "scalefactors_json.json"
     SCALEFACTORS_HIRES = "tissue_hires_scalef"
     SCALEFACTORS_LOWRES = "tissue_lowres_scalef"
 
     # spots
-    SPOTS_FILE = "spatial/tissue_positions.csv"
+    SPOTS_FILE_1 = "tissue_positions_list.csv"
+    SPOTS_FILE_2 = "tissue_positions.csv"
     SPOTS_X = "pxl_row_in_fullres"
     SPOTS_Y = "pxl_col_in_fullres"
 
 
 @unique
 class SteinbockKeys(ModeEnum):
     """Keys for *Steinbock* formatted dataset."""
@@ -132,7 +148,37 @@
     LABELS_DIR = "segmentation"
     LABELS_PREFIX = "unmicst-"
 
     # metadata
     COORDS_X = "X_centroid"
     COORDS_Y = "Y_centroid"
     INSTANCE_KEY = "CellID"
+
+
+@unique
+class MerscopeKeys(ModeEnum):
+    """Keys for *MERSCOPE* data (Vizgen plateform)"""
+
+    # files and directories
+    IMAGES_DIR = "images"
+    TRANSFORMATION_FILE = "micron_to_mosaic_pixel_transform.csv"
+    TRANSCRIPTS_FILE = "detected_transcripts.csv"
+    BOUNDARIES_FILE = "cell_boundaries.parquet"
+    COUNTS_FILE = "cell_by_gene.csv"
+    CELL_METADATA_FILE = "cell_metadata.csv"
+
+    # VPT default outputs
+    CELLPOSE_BOUNDARIES = "cellpose_micron_space.parquet"
+    WATERSHED_BOUNDARIES = "watershed_micron_space.parquet"
+    VPT_NAME_COUNTS = "cell_by_gene"
+    VPT_NAME_OBS = "cell_metadata"
+    VPT_NAME_BOUNDARIES = "cell_boundaries"
+
+    # metadata
+    INSTANCE_KEY = "EntityID"
+    COUNTS_CELL_KEY = "cell"
+    CELL_X = "center_x"
+    CELL_Y = "center_y"
+    GLOBAL_X = "global_x"
+    GLOBAL_Y = "global_y"
+    GLOBAL_Z = "global_z"
+    Z_INDEX = "ZIndex"
```

### Comparing `spatialdata_io-0.0.4/src/spatialdata_io/_constants/_enum.py` & `spatialdata_io-0.0.5/src/spatialdata_io/_constants/_enum.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/src/spatialdata_io/readers/cosmx.py` & `spatialdata_io-0.0.5/src/spatialdata_io/readers/cosmx.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/src/spatialdata_io/readers/curio.py` & `spatialdata_io-0.0.5/src/spatialdata_io/readers/curio.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,101 @@
 from __future__ import annotations
 
+import os
 from pathlib import Path
-from typing import Optional
 
 import anndata as ad
+import numpy as np
 import pandas as pd
 from spatialdata import SpatialData
-from spatialdata.models import TableModel
+from spatialdata.models import ShapesModel, TableModel
 
 from spatialdata_io._constants._constants import CurioKeys
 from spatialdata_io._docs import inject_docs
 
 __all__ = ["curio"]
 
 
 @inject_docs(vx=CurioKeys)
 def curio(
     path: str | Path,
-    dataset_id: Optional[str] = None,
 ) -> SpatialData:
     """
     Read *Curio* formatted dataset.
 
     This function reads the following files:
 
         - ``<dataset_id>_`{vx.ANNDATA_FILE!r}```: Counts and metadata file.
         - ``<dataset_id>_`{vx.CLUSTER_ASSIGNMENT!r}```: Cluster assignment file.
         - ``<dataset_id>_`{vx.METRICS_FILE!r}```: Metrics file.
         - ``<dataset_id>_`{vx.VAR_FEATURES_CLUSTERS!r}```: Variable features clusters file.
         - ``<dataset_id>_`{vx.VAR_FEATURES_MORANSI!r}```: Variable features Moran's I file.
 
-    .. seealso::
-
-        - `CODEX output <https://help.codex.bio/codex/processor/technical-notes/expected-output>`_.
+    <dataset_id> is automatically inferred from the path.
 
     Parameters
     ----------
     path
         Path to the directory containing the data.
-    dataset_id
-        Dataset identifier.
-    imread_kwargs
-        Keyword arguments passed to :func:`dask_image.imread.imread`.
-    image_models_kwargs
-        Keyword arguments passed to :class:`spatialdata.models.Image2DModel`.
 
     Returns
     -------
     :class:`spatialdata.SpatialData`
     """
     path = Path(path)
-    path_files = [
+    path_files = (
         CurioKeys.ANNDATA_FILE,
         CurioKeys.CLUSTER_ASSIGNMENT,
         CurioKeys.METRICS_FILE,
         CurioKeys.VAR_FEATURES_CLUSTERS,
         CurioKeys.VAR_FEATURES_MORANSI,
-    ]
+    )
 
-    if dataset_id is not None:
-        file_names = [f"{dataset_id}_{file_name}" for file_name in path_files]
-    else:
-        file_names = []
-        for file_name in path_files:
-            file_names.extend(str(path.glob(file_name)))
-
-    adata = ad.read_h5ad(path / file_names[0])
-    cluster_assign = pd.read_csv(path / file_names[1], sep="\t", header=None)
-    metrics = pd.read_csv(path / file_names[2], sep=r"\,", header=0)
-    var_features_clusters = pd.read_csv(path / file_names[3], sep="\t", header=0)
-    var_features_moransi = pd.read_csv(path / file_names[4], sep="\t", header=0)
+    file_names = {}
+    for i in os.listdir(path):
+        if os.path.isfile(os.path.join(path, i)):
+            for path_file in path_files:
+                if path_file in i:
+                    file_names[path_file] = i
+    assert len(file_names) == len(path_files), f"Missing files: {set(path_files) - set(file_names.keys())}"
+
+    adata = ad.read_h5ad(path / file_names[CurioKeys.ANNDATA_FILE])
+    cluster_assign = pd.read_csv(path / file_names[CurioKeys.CLUSTER_ASSIGNMENT], sep="\t", header=None)
+    metrics = pd.read_csv(path / file_names[CurioKeys.METRICS_FILE], sep=r"\,", header=0)
+    var_features_clusters = pd.read_csv(path / file_names[CurioKeys.VAR_FEATURES_CLUSTERS], sep="\t", header=0)
+    var_features_moransi = pd.read_csv(path / file_names[CurioKeys.VAR_FEATURES_MORANSI], sep="\t", header=0)
 
+    # adding cluster information in adata.obs
+    assert np.array_equal(cluster_assign[0].to_numpy(), adata.obs.index.to_numpy())
     adata.obs = adata.obs.assign(cluster=cluster_assign[1].values)
+    adata.obs["cluster"] = adata.obs["cluster"].astype("category")
+
+    # adding metrics information in adata.uns
     categories = metrics[CurioKeys.CATEGORY].unique()
     for cat in categories:
         df = metrics.loc[metrics[CurioKeys.CATEGORY] == cat]
         adata.uns[cat] = dict(zip(df.iloc[:, 0], df.iloc[:, 1]))
     adata.uns[CurioKeys.TOP_CLUSTER_DEFINING_FEATURES] = var_features_clusters
+
+    # adding Moran's I information in adata.var, for the variable for which it is available
+    assert set(adata.var_names).issuperset(var_features_moransi.index)
     adata.var.join(var_features_moransi, how="outer")
 
-    table = TableModel.parse(adata)
+    adata.obs[CurioKeys.REGION_KEY] = CurioKeys.REGION
+    adata.obs[CurioKeys.REGION_KEY] = adata.obs[CurioKeys.REGION_KEY].astype("category")
+    adata.obs[CurioKeys.INSTANCE_KEY] = adata.obs.index
+
+    table = TableModel.parse(
+        adata,
+        region=CurioKeys.REGION.value,
+        region_key=CurioKeys.REGION_KEY.value,
+        instance_key=CurioKeys.INSTANCE_KEY.value,
+    )
+
+    # adding geometry information in a shapes element (we redundantly leave it in obsm['spatial'])
+    assert np.array_equal(adata.obsm["spatial"], adata.obsm["X_spatial"])
+    xy = adata.obsm["spatial"]
+    del adata.obsm["X_spatial"]
+
+    shapes = ShapesModel.parse(xy, geometry=0, radius=10, index=adata.obs[CurioKeys.INSTANCE_KEY])
 
-    return SpatialData(table=table)
+    return SpatialData(table=table, shapes={CurioKeys.REGION.value: shapes})
```

### Comparing `spatialdata_io-0.0.4/src/spatialdata_io/readers/mcmicro.py` & `spatialdata_io-0.0.5/src/spatialdata_io/readers/mcmicro.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/src/spatialdata_io/readers/steinbock.py` & `spatialdata_io-0.0.5/src/spatialdata_io/readers/steinbock.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/src/spatialdata_io/readers/visium.py` & `spatialdata_io-0.0.5/src/spatialdata_io/readers/visium.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import json
 import os
 import re
 from collections.abc import Mapping
+from functools import partial
 from pathlib import Path
 from types import MappingProxyType
 from typing import Any, Optional
 
 import numpy as np
 import pandas as pd
 from dask_image.imread import imread
@@ -24,89 +25,135 @@
 __all__ = ["visium"]
 
 
 @inject_docs(vx=VisiumKeys)
 def visium(
     path: str | Path,
     dataset_id: Optional[str] = None,
+    counts_file: str = VisiumKeys.COUNTS_FILE,
+    fullres_image_file: Optional[str | Path] = None,
+    tissue_positions_file: Optional[str | Path] = None,
+    scalefactors_file: Optional[str | Path] = None,
     imread_kwargs: Mapping[str, Any] = MappingProxyType({}),
     image_models_kwargs: Mapping[str, Any] = MappingProxyType({}),
     **kwargs: Any,
 ) -> SpatialData:
     """
     Read *10x Genomics* Visium formatted dataset.
 
     This function reads the following files:
 
-        - ``<dataset_id>_`{vx.COUNTS_FILE!r}```: Counts and metadata file.
+        - ``{vx.COUNTS_FILE!r}``: Counts and metadata file.
         - ``{vx.IMAGE_HIRES_FILE!r}``: High resolution image.
         - ``{vx.IMAGE_LOWRES_FILE!r}``: Low resolution image.
-        - ``<dataset_id>_`{vx.IMAGE_TIF_SUFFIX!r}```: High resolution tif image.
-        - ``<dataset_id>_`{vx.IMAGE_TIF_ALTERNATIVE_SUFFIX!r}```: High resolution tif image, old naming convention.
         - ``{vx.SCALEFACTORS_FILE!r}``: Scalefactors file.
-        - ``{vx.SPOTS_FILE!r}``: Spots positions file.
+        - ``{vx.SPOTS_FILE_1!r}`` (SpaceRanger 1) or ``{vx.SPOTS_FILE_2!r}`` (SpaceRanger 2):
+            Spots positions file.
+        - ``fullres_image_file``: large microscopy image used as input for space ranger.
 
     .. seealso::
 
         - `Space Ranger output <https://support.10xgenomics.com/spatial-gene-expression/software/pipelines/latest/output/overview>`_.
 
     Parameters
     ----------
     path
         Path to the directory containing the data.
     dataset_id
-        Dataset identifier.
+        Dataset identifier. If not given will be determined automatically
+        from the ``{vx.COUNTS_FILE!r}`` file.
+    counts_file
+        Name of the counts file. Use only if counts is not in `h5` format.
+    fullres_image_file
+        Path to the full-resolution image.
+    tissue_positions_file
+        Path to the tissue positions file.
+    scalefactors_file
+        Path to the scalefactors file.
     imread_kwargs
         Keyword arguments passed to :func:`dask_image.imread.imread`.
     image_models_kwargs
         Keyword arguments passed to :class:`spatialdata.models.Image2DModel`.
 
     Returns
     -------
     :class:`spatialdata.SpatialData`
     """
     path = Path(path)
+    imread_kwargs = dict(imread_kwargs)
+    image_models_kwargs = dict(image_models_kwargs)
     # get library_id
-    patt = re.compile(f".*{VisiumKeys.COUNTS_FILE}")
-    first_file = [i for i in os.listdir(path) if patt.match(i)][0]
-    if f"_{VisiumKeys.COUNTS_FILE}" in first_file:
-        library_id = first_file.replace(f"_{VisiumKeys.COUNTS_FILE}", "")
-    else:
-        raise ValueError(
-            f"Cannot determine the library_id. Expecting a file with format <library_id>_{VisiumKeys.COUNTS_FILE}. Has "
-            f"the files been renamed?"
-        )
+    try:
+        patt = re.compile(f".*{VisiumKeys.COUNTS_FILE}")
+        first_file = [i for i in os.listdir(path) if patt.match(i)][0]
+
+        if f"_{VisiumKeys.COUNTS_FILE}" in first_file:
+            library_id = first_file.replace(f"_{VisiumKeys.COUNTS_FILE}", "")
+        else:
+            raise ValueError(
+                f"Cannot determine the library_id. Expecting a file with format <library_id>_{VisiumKeys.COUNTS_FILE}. Has "
+                f"the files been renamed?"
+            )
+        counts_file = f"{library_id}_{VisiumKeys.COUNTS_FILE}"
+    except IndexError as e:
+        logger.error(e)
+        if dataset_id is None:
+            raise ValueError("Cannot determine the `library_id`. Please provide `dataset_id`.")
+        library_id = dataset_id
+        if counts_file is None:
+            raise ValueError("Cannot determine the library_id. Please provide `counts_file`.")
+
     if dataset_id is not None:
         if dataset_id != library_id:
             logger.warning(
                 f"`dataset_id: {dataset_id}` does not match `library_id: {library_id}`. `dataset_id: {dataset_id}` "
                 f"will be used to build SpatialData."
             )
     else:
         dataset_id = library_id
 
-    adata, library_id = _read_counts(
-        path, count_file=f"{library_id}_{VisiumKeys.COUNTS_FILE}", library_id=library_id, **kwargs
-    )
+    adata, dataset_id = _read_counts(path, counts_file=counts_file, library_id=dataset_id, **kwargs)
+
+    if (path / "spatial" / VisiumKeys.SPOTS_FILE_1).exists() or (
+        tissue_positions_file is not None and str(VisiumKeys.SPOTS_FILE_1) in str(tissue_positions_file)
+    ):
+        read_coords = partial(pd.read_csv, header=None, index_col=0)
+        tissue_positions_file = (
+            path / "spatial" / VisiumKeys.SPOTS_FILE_1
+            if tissue_positions_file is None
+            else path / tissue_positions_file
+        )
+    elif (path / "spatial" / VisiumKeys.SPOTS_FILE_2).exists() or (
+        tissue_positions_file is not None and str(VisiumKeys.SPOTS_FILE_2) in str(tissue_positions_file)
+    ):
+        read_coords = partial(pd.read_csv, header=1, index_col=0)
+        tissue_positions_file = (
+            path / "spatial" / VisiumKeys.SPOTS_FILE_2
+            if tissue_positions_file is None
+            else path / tissue_positions_file
+        )
+    else:
+        raise ValueError(f"Cannot find `tissue_positions` file in `{path}`.")
+    coords = read_coords(tissue_positions_file)
 
-    coords = pd.read_csv(
-        path / VisiumKeys.SPOTS_FILE,
-        header=0,
-        index_col=0,
-    )
     coords.columns = ["in_tissue", "array_row", "array_col", "pxl_col_in_fullres", "pxl_row_in_fullres"]
 
     adata.obs = pd.merge(adata.obs, coords, how="left", left_index=True, right_index=True)
     coords = adata.obs[[VisiumKeys.SPOTS_X, VisiumKeys.SPOTS_Y]].values
     adata.obsm["spatial"] = coords
     adata.obs.drop(columns=[VisiumKeys.SPOTS_X, VisiumKeys.SPOTS_Y], inplace=True)
     adata.obs["spot_id"] = np.arange(len(adata))
     adata.var_names_make_unique()
-
-    scalefactors = json.loads((path / VisiumKeys.SCALEFACTORS_FILE).read_bytes())
+    if (path / "spatial" / VisiumKeys.SCALEFACTORS_FILE).exists() or (
+        scalefactors_file is not None and (path / scalefactors_file).exists()
+    ):
+        scalefactors_file = (
+            path / "spatial" / VisiumKeys.SCALEFACTORS_FILE if scalefactors_file is None else path / scalefactors_file
+        )
+        scalefactors = json.loads(scalefactors_file.read_bytes())
 
     transform_original = Identity()
     transform_lowres = Scale(
         np.array([scalefactors[VisiumKeys.SCALEFACTORS_LOWRES], scalefactors[VisiumKeys.SCALEFACTORS_LOWRES]]),
         axes=("y", "x"),
     )
     transform_hires = Scale(
@@ -125,43 +172,40 @@
             "downscaled_lowres": transform_lowres,
         },
     )
     shapes[dataset_id] = circles
     adata.obs["region"] = dataset_id
     table = TableModel.parse(adata, region=dataset_id, region_key="region", instance_key="spot_id")
 
-    if (path / f"{dataset_id}{VisiumKeys.IMAGE_TIF_SUFFIX}").exists():
-        tif_path = path / f"{dataset_id}{VisiumKeys.IMAGE_TIF_SUFFIX}"
-    elif (path / f"{dataset_id}{VisiumKeys.IMAGE_TIF_ALTERNATIVE_SUFFIX}").exists():
-        tif_path = path / f"{dataset_id}{VisiumKeys.IMAGE_TIF_ALTERNATIVE_SUFFIX}"
-    else:
-        raise FileNotFoundError(
-            f"Cannot find {VisiumKeys.IMAGE_TIF_SUFFIX} or {VisiumKeys.IMAGE_TIF_ALTERNATIVE_SUFFIX}."
-        )
-
-    full_image = imread(tif_path, **imread_kwargs).squeeze().transpose(2, 0, 1)
-    full_image = DataArray(full_image, dims=("c", "y", "x"), name=dataset_id)
-
-    image_hires = imread(path / VisiumKeys.IMAGE_HIRES_FILE, **imread_kwargs).squeeze().transpose(2, 0, 1)
-    image_hires = DataArray(image_hires, dims=("c", "y", "x"), name=dataset_id)
-
-    image_lowres = imread(path / VisiumKeys.IMAGE_LOWRES_FILE, **imread_kwargs).squeeze().transpose(2, 0, 1)
-    image_lowres = DataArray(image_lowres, dims=("c", "y", "x"), name=dataset_id)
-
-    full_image_parsed = Image2DModel.parse(
-        # drop alpha channel
-        full_image.sel({"c": slice(0, 3)}),
-        scale_factors=[2, 2, 2, 2],
-        transformations={"global": transform_original},
-        **image_models_kwargs,
-    )
-
-    image_hires_parsed = Image2DModel.parse(image_hires, transformations={"downscaled_hires": Identity()})
-    image_lowres_parsed = Image2DModel.parse(image_lowres, transformations={"downscaled_lowres": Identity()})
+    images = {}
+    if fullres_image_file is not None:
+        fullres_image_file = path / Path(fullres_image_file)
+        if fullres_image_file.exists():
+            if "MAX_IMAGE_PIXELS" in imread_kwargs:
+                from PIL import Image as ImagePIL
+
+                ImagePIL.MAX_IMAGE_PIXELS = imread_kwargs.pop("MAX_IMAGE_PIXELS")
+            full_image = imread(fullres_image_file, **imread_kwargs).squeeze().transpose(2, 0, 1)
+            full_image = DataArray(full_image, dims=("c", "y", "x"), name=dataset_id)
+            images[dataset_id + "_full_image"] = Image2DModel.parse(
+                full_image,
+                scale_factors=[2, 2, 2, 2],
+                transformations={"global": transform_original},
+                **image_models_kwargs,
+            )
+        else:
+            logger.warning(f"File {fullres_image_file} does not exist, skipping...")
 
-    images = {
-        dataset_id + "_lowres_image": image_lowres_parsed,
-        dataset_id + "_hires_image": image_hires_parsed,
-        dataset_id + "_full_image": full_image_parsed,
-    }
+    if (path / VisiumKeys.IMAGE_HIRES_FILE).exists():
+        image_hires = imread(path / VisiumKeys.IMAGE_HIRES_FILE, **imread_kwargs).squeeze().transpose(2, 0, 1)
+        image_hires = DataArray(image_hires, dims=("c", "y", "x"), name=dataset_id)
+        images[dataset_id + "_hires_image"] = Image2DModel.parse(
+            image_hires, transformations={"downscaled_hires": Identity()}
+        )
+    if (path / VisiumKeys.IMAGE_LOWRES_FILE).exists():
+        image_lowres = imread(path / VisiumKeys.IMAGE_LOWRES_FILE, **imread_kwargs).squeeze().transpose(2, 0, 1)
+        image_lowres = DataArray(image_lowres, dims=("c", "y", "x"), name=dataset_id)
+        images[dataset_id + "_lowres_image"] = Image2DModel.parse(
+            image_lowres, transformations={"downscaled_lowres": Identity()}
+        )
 
     return SpatialData(images=images, shapes=shapes, table=table)
```

### Comparing `spatialdata_io-0.0.4/src/spatialdata_io/readers/xenium.py` & `spatialdata_io-0.0.5/src/spatialdata_io/readers/xenium.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 def _get_points(path: Path, specs: dict[str, Any]) -> Table:
     table = read_parquet(path / XeniumKeys.TRANSCRIPTS_FILE)
     table["feature_name"] = table["feature_name"].apply(lambda x: x.decode("utf-8"), meta=("feature_name", "object"))
 
     transform = Scale([1.0 / specs["pixel_size"], 1.0 / specs["pixel_size"]], axes=("x", "y"))
     points = PointsModel.parse(
         table,
-        coordinates={"x": XeniumKeys.TRANSCRIPTS_X, "y": XeniumKeys.TRANSCRIPTS_Y, "z": XeniumKeys.TRANSCRIPTS_Y},
+        coordinates={"x": XeniumKeys.TRANSCRIPTS_X, "y": XeniumKeys.TRANSCRIPTS_Y, "z": XeniumKeys.TRANSCRIPTS_Z},
         feature_key=XeniumKeys.FEATURE_NAME,
         instance_key=XeniumKeys.CELL_ID,
         transformations={"global": transform},
     )
     return points
```

### Comparing `spatialdata_io-0.0.4/src/spatialdata_io/readers/_utils/_read_10x_h5.py` & `spatialdata_io-0.0.5/src/spatialdata_io/readers/_utils/_read_10x_h5.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/LICENSE` & `spatialdata_io-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.4/README.md` & `spatialdata_io-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,18 +8,29 @@
 [badge-tests]: https://github.com/scverse/spatialdata-io/actions/workflows/test_and_deploy.yaml/badge.svg
 [link-tests]: https://github.com/scverse/spatialdata-io/actions/workflows/test_and_deploy.yaml
 [badge-docs]: https://img.shields.io/readthedocs/spatialdata-io
 
 This package contains reader functions to load common spatial omics formats into SpatialData. Currently, we provide support for:
 
 -   NanoString CosMx
--   MCMICRO
--   Steinbock
+-   MCMICRO (output data)
+-   Steinbock (output data)
 -   10x Genomics Visium
 -   10x Genomics Xenium
+-   Curio Seeker
+-   Vizgen MERSCOPE (MERFISH)
+
+Coming soon:
+
+-   Spatial Genomics seqFISH
+-   Akoya PhenoCycler (formerly CODEX)
+
+Also coming soon:
+
+-   Common image converters: .jpg <> .zarr
 
 ## Getting started
 
 Please refer to the [documentation][link-docs]. In particular, the
 
 -   [API documentation][link-api].
 
@@ -49,10 +60,10 @@
 
 ## Citation
 
 [L Marconato*, G Palla*, KA Yamauchi*, I Virshup*, E Heidari, T Treis, M Toth, R Shrestha, H Vöhringer, W Huber, M Gerstung, J Moore, FJ Theis, O Stegle, bioRxiv, 2023](https://www.biorxiv.org/content/10.1101/2023.05.05.539647v1). \* = equal contribution
 
 [scverse-discourse]: https://discourse.scverse.org/
 [issue-tracker]: https://github.com/scverse/spatialdata-io/issues
-[changelog]: https://spatialdata-io.readthedocs.io/latest/changelog.html
-[link-docs]: https://spatialdata-io.readthedocs.io
-[link-api]: https://spatialdata-io.readthedocs.io/latest/api.html
+[changelog]: https://spatialdata.scverse.org/projects/io/en/latest/changelog.html
+[link-docs]: https://spatialdata.scverse.org/projects/io/en/latest/
+[link-api]: https://spatialdata.scverse.org/projects/io/en/latest/api.html
```

### Comparing `spatialdata_io-0.0.4/pyproject.toml` & `spatialdata_io-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "spatialdata",
     "scikit-image",
     "h5py",
     "joblib",
     "imagecodecs",
     "dask-image",
     "pyarrow",
+    "readfcs",
 ]
 
 [project.optional-dependencies]
 dev = [
     # CLI for bumping the version number
     "bump2version",
     "pre-commit"
```

### Comparing `spatialdata_io-0.0.4/PKG-INFO` & `spatialdata_io-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialdata-io
-Version: 0.0.4
+Version: 0.0.5
 Summary: SpatialData IO for common techs
 Project-URL: Documentation, https://spatialdata-io.readthedocs.io/
 Project-URL: Source, https://github.com/scverse/spatialdata-io
 Project-URL: Home-page, https://github.com/scverse/spatialdata-io
 Author: scverse
 Maintainer-email: scverse <scverse@scverse.scverse>
 License: BSD 3-Clause License
@@ -39,14 +39,15 @@
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: dask-image
 Requires-Dist: h5py
 Requires-Dist: imagecodecs
 Requires-Dist: joblib
 Requires-Dist: pyarrow
+Requires-Dist: readfcs
 Requires-Dist: scikit-image
 Requires-Dist: spatialdata
 Provides-Extra: dev
 Requires-Dist: bump2version; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: ipython>=8.6.0; extra == 'doc'
@@ -72,18 +73,29 @@
 [badge-tests]: https://github.com/scverse/spatialdata-io/actions/workflows/test_and_deploy.yaml/badge.svg
 [link-tests]: https://github.com/scverse/spatialdata-io/actions/workflows/test_and_deploy.yaml
 [badge-docs]: https://img.shields.io/readthedocs/spatialdata-io
 
 This package contains reader functions to load common spatial omics formats into SpatialData. Currently, we provide support for:
 
 -   NanoString CosMx
--   MCMICRO
--   Steinbock
+-   MCMICRO (output data)
+-   Steinbock (output data)
 -   10x Genomics Visium
 -   10x Genomics Xenium
+-   Curio Seeker
+-   Vizgen MERSCOPE (MERFISH)
+
+Coming soon:
+
+-   Spatial Genomics seqFISH
+-   Akoya PhenoCycler (formerly CODEX)
+
+Also coming soon:
+
+-   Common image converters: .jpg <> .zarr
 
 ## Getting started
 
 Please refer to the [documentation][link-docs]. In particular, the
 
 -   [API documentation][link-api].
 
@@ -113,10 +125,10 @@
 
 ## Citation
 
 [L Marconato*, G Palla*, KA Yamauchi*, I Virshup*, E Heidari, T Treis, M Toth, R Shrestha, H Vöhringer, W Huber, M Gerstung, J Moore, FJ Theis, O Stegle, bioRxiv, 2023](https://www.biorxiv.org/content/10.1101/2023.05.05.539647v1). \* = equal contribution
 
 [scverse-discourse]: https://discourse.scverse.org/
 [issue-tracker]: https://github.com/scverse/spatialdata-io/issues
-[changelog]: https://spatialdata-io.readthedocs.io/latest/changelog.html
-[link-docs]: https://spatialdata-io.readthedocs.io
-[link-api]: https://spatialdata-io.readthedocs.io/latest/api.html
+[changelog]: https://spatialdata.scverse.org/projects/io/en/latest/changelog.html
+[link-docs]: https://spatialdata.scverse.org/projects/io/en/latest/
+[link-api]: https://spatialdata.scverse.org/projects/io/en/latest/api.html
```

