# Comparing `tmp/spatialdata_io-0.0.5.tar.gz` & `tmp/spatialdata_io-0.0.6.tar.gz`

## Comparing `spatialdata_io-0.0.5.tar` & `spatialdata_io-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.bumpversion.cfg
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.codecov.yaml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.editorconfig
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.flake8
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.mypy.ini
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.readthedocs.yaml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/_version.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.github/workflows/test_and_deploy.yaml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/Makefile
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/changelog.md
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/conf.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/contributing.md
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/index.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/make.bat
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/references.md
--rw-r--r--   0        0        0    16386 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/template_usage.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/extensions/.gitkeep
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/_docs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/_constants/__init__.py
--rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/_constants/_constants.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/_constants/_enum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/__init__.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/codex.py
--rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/cosmx.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/curio.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/mcmicro.py
--rw-r--r--   0        0        0     7492 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/merscope.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/metaspace.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/resolve.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/steinbock.py
--rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/visium.py
--rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/xenium.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/_utils/__init__.py
--rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/_utils/_read_10x_h5.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/src/spatialdata_io/readers/_utils/_utils.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/tests/test_basic.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/LICENSE
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/README.md
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 spatialdata_io-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.bumpversion.cfg
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.codecov.yaml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.editorconfig
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.flake8
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.mypy.ini
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.readthedocs.yaml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/_version.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.github/workflows/test_and_deploy.yaml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/Makefile
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/changelog.md
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/conf.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/contributing.md
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/index.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/make.bat
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/references.md
+-rw-r--r--   0        0        0    16386 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/template_usage.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/extensions/.gitkeep
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/_docs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/_constants/__init__.py
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/_constants/_constants.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/_constants/_enum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/__init__.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/codex.py
+-rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/cosmx.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/curio.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/mcmicro.py
+-rw-r--r--   0        0        0     7492 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/merscope.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/metaspace.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/resolve.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/steinbock.py
+-rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/visium.py
+-rw-r--r--   0        0        0     8080 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/xenium.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/_utils/__init__.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/_utils/_read_10x_h5.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/src/spatialdata_io/readers/_utils/_utils.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/tests/test_basic.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/README.md
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 spatialdata_io-0.0.6/PKG-INFO
```

### Comparing `spatialdata_io-0.0.5/.flake8` & `spatialdata_io-0.0.6/.flake8`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/.mypy.ini` & `spatialdata_io-0.0.6/.mypy.ini`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/.pre-commit-config.yaml` & `spatialdata_io-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/.github/workflows/build.yaml` & `spatialdata_io-0.0.6/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/.github/workflows/test_and_deploy.yaml` & `spatialdata_io-0.0.6/.github/workflows/test_and_deploy.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/docs/Makefile` & `spatialdata_io-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/docs/conf.py` & `spatialdata_io-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/docs/contributing.md` & `spatialdata_io-0.0.6/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/docs/make.bat` & `spatialdata_io-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/docs/references.bib` & `spatialdata_io-0.0.6/docs/references.bib`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/docs/template_usage.md` & `spatialdata_io-0.0.6/docs/template_usage.md`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/docs/_templates/autosummary/class.rst` & `spatialdata_io-0.0.6/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/docs/extensions/typed_returns.py` & `spatialdata_io-0.0.6/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/__init__.py` & `spatialdata_io-0.0.6/src/spatialdata_io/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/_docs.py` & `spatialdata_io-0.0.6/src/spatialdata_io/_docs.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/_constants/_constants.py` & `spatialdata_io-0.0.6/src/spatialdata_io/_constants/_constants.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/_constants/_enum.py` & `spatialdata_io-0.0.6/src/spatialdata_io/_constants/_enum.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/readers/codex.py` & `spatialdata_io-0.0.6/src/spatialdata_io/readers/codex.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,30 +68,28 @@
 
     xy = adata.obsm[CodexKeys.SPATIAL_KEY]
     shapes = ShapesModel.parse(xy, geometry=0, radius=1, index=adata.obs[CodexKeys.INSTANCE_KEY])
     region = adata.obs[CodexKeys.REGION_KEY].unique()[0]
     adata.obs[CodexKeys.REGION_KEY] = adata.obs[CodexKeys.REGION_KEY].astype("category")
     table = TableModel.parse(adata, region=region, region_key=CodexKeys.REGION_KEY, instance_key=CodexKeys.INSTANCE_KEY)
 
-    # convert list of one element to string
-
     im_patt = re.compile(".*.tif")
     path_files = [i for i in os.listdir(path) if im_patt.match(i)]
     if path_files and CodexKeys.IMAGE_TIF in path_files[0]:
         image = imread(path_files[0], **imread_kwargs)
         images = {
             "images": Image2DModel.parse(
                 image,
                 scale_factors=[2, 2],
             )
         }
         sdata = SpatialData(images=images, shapes={region: shapes}, table=table)
     else:
         logger.warning("Cannot find .tif file. Will build spatialdata with shapes and table only.")
-        sdata = SpatialData(shapes={"".join(str(x) for x in region): shapes}, table=table)
+        sdata = SpatialData(shapes={region: shapes}, table=table)
 
     return sdata
 
 
 def _codex_df_to_anndata(df: pd.DataFrame) -> ad.AnnData:
     """Convert a codex formatted .fcs dataframe or .csv file to anndata."""
     adata = ad.AnnData(df.filter(regex="cyc.*"))
```

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/readers/cosmx.py` & `spatialdata_io-0.0.6/src/spatialdata_io/readers/cosmx.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/readers/curio.py` & `spatialdata_io-0.0.6/src/spatialdata_io/readers/curio.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/readers/mcmicro.py` & `spatialdata_io-0.0.6/src/spatialdata_io/readers/mcmicro.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/readers/merscope.py` & `spatialdata_io-0.0.6/src/spatialdata_io/readers/merscope.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/readers/steinbock.py` & `spatialdata_io-0.0.6/src/spatialdata_io/readers/steinbock.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/readers/visium.py` & `spatialdata_io-0.0.6/src/spatialdata_io/readers/visium.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/readers/xenium.py` & `spatialdata_io-0.0.6/src/spatialdata_io/readers/xenium.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             specs,
             imread_kwargs,
             image_models_kwargs,
         )
     if morphology_focus:
         images["morphology_focus"] = _get_images(
             path,
-            XeniumKeys.MORPHOLOGY_MIP_FILE,
+            XeniumKeys.MORPHOLOGY_FOCUS_FILE,
             specs,
             imread_kwargs,
             image_models_kwargs,
         )
     if cells_as_shapes:
         return SpatialData(images=images, shapes=polygons | {specs["region"]: circles}, points=points, table=table)
     return SpatialData(images=images, shapes=polygons, points=points, table=table)
@@ -182,15 +182,15 @@
 
 
 def _get_tables_and_circles(
     path: Path, cells_as_shapes: bool, specs: dict[str, Any]
 ) -> AnnData | tuple[AnnData, AnnData]:
     adata = _read_10x_h5(path / XeniumKeys.CELL_FEATURE_MATRIX_FILE)
     metadata = pd.read_parquet(path / XeniumKeys.CELL_METADATA_FILE)
-    np.testing.assert_array_equal(metadata.cell_id.astype(str).values, adata.obs_names.values)
+    np.testing.assert_array_equal(metadata.cell_id.str.decode("utf-8").values, adata.obs_names.values)
     circ = metadata[[XeniumKeys.CELL_X, XeniumKeys.CELL_Y]].to_numpy()
     adata.obsm["spatial"] = circ
     metadata.drop([XeniumKeys.CELL_X, XeniumKeys.CELL_Y], axis=1, inplace=True)
     adata.obs = metadata
     adata.obs["region"] = specs["region"]
     table = TableModel.parse(adata, region=specs["region"], region_key="region", instance_key=str(XeniumKeys.CELL_ID))
     if cells_as_shapes:
```

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/readers/_utils/_read_10x_h5.py` & `spatialdata_io-0.0.6/src/spatialdata_io/readers/_utils/_read_10x_h5.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/src/spatialdata_io/readers/_utils/_utils.py` & `spatialdata_io-0.0.6/src/spatialdata_io/readers/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/LICENSE` & `spatialdata_io-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/README.md` & `spatialdata_io-0.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -13,24 +13,16 @@
 
 -   NanoString CosMx
 -   MCMICRO (output data)
 -   Steinbock (output data)
 -   10x Genomics Visium
 -   10x Genomics Xenium
 -   Curio Seeker
--   Vizgen MERSCOPE (MERFISH)
-
-Coming soon:
-
--   Spatial Genomics seqFISH
 -   Akoya PhenoCycler (formerly CODEX)
-
-Also coming soon:
-
--   Common image converters: .jpg <> .zarr
+-   Vizgen MERSCOPE (MERFISH)
 
 ## Getting started
 
 Please refer to the [documentation][link-docs]. In particular, the
 
 -   [API documentation][link-api].
```

### Comparing `spatialdata_io-0.0.5/pyproject.toml` & `spatialdata_io-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.5/PKG-INFO` & `spatialdata_io-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialdata-io
-Version: 0.0.5
+Version: 0.0.6
 Summary: SpatialData IO for common techs
 Project-URL: Documentation, https://spatialdata-io.readthedocs.io/
 Project-URL: Source, https://github.com/scverse/spatialdata-io
 Project-URL: Home-page, https://github.com/scverse/spatialdata-io
 Author: scverse
 Maintainer-email: scverse <scverse@scverse.scverse>
 License: BSD 3-Clause License
@@ -78,24 +78,16 @@
 
 -   NanoString CosMx
 -   MCMICRO (output data)
 -   Steinbock (output data)
 -   10x Genomics Visium
 -   10x Genomics Xenium
 -   Curio Seeker
--   Vizgen MERSCOPE (MERFISH)
-
-Coming soon:
-
--   Spatial Genomics seqFISH
 -   Akoya PhenoCycler (formerly CODEX)
-
-Also coming soon:
-
--   Common image converters: .jpg <> .zarr
+-   Vizgen MERSCOPE (MERFISH)
 
 ## Getting started
 
 Please refer to the [documentation][link-docs]. In particular, the
 
 -   [API documentation][link-api].
```

