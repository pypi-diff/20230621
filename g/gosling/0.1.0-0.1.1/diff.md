# Comparing `tmp/gosling-0.1.0.tar.gz` & `tmp/gosling-0.1.1.tar.gz`

## Comparing `gosling-0.1.0.tar` & `gosling-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/_version.py
--rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/api.py
--rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/display.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/plugin_registry.py
--rw-r--r--   0        0        0    20141 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/schemapi.py
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/data/__init__.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/data/_tilesets.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/data/tests/test_data_server.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/__init__.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/area_chart.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/bar_chart.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/between_link_pandas.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/brushing_and_linking.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/circos.py
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/comparative_matrices.py
--rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/corces.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/covid.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/genes.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/heatmap.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/ideograms.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/line_chart.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/multiscale_lollipop_plot.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/multiscale_sequence.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/overview_detail.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/point_plot.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/examples/text_marks.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/schema/__init__.py
--rw-r--r--   0        0        0    32752 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/schema/channels.py
--rw-r--r--   0        0        0   104964 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/schema/core.py
--rw-r--r--   0        0        0   303941 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/schema/gosling-schema.json
--rw-r--r--   0        0        0    27321 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/schema/mixins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/sphinxext/__init__.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/sphinxext/gallery.py
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/sphinxext/plot.py
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/tests/test_api.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/tests/test_data.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/tests/test_plugin_registry.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/utils/__init__.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/utils/core.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 gosling-0.1.0/gosling/utils/execeval.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 gosling-0.1.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 gosling-0.1.0/LICENSE
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 gosling-0.1.0/README.md
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 gosling-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 gosling-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/_version.py
+-rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/api.py
+-rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/display.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/plugin_registry.py
+-rw-r--r--   0        0        0    20141 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/schemapi.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/data/__init__.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/data/_tilesets.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/data/tests/test_data_server.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/__init__.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/area_chart.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/bar_chart.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/between_link_pandas.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/brushing_and_linking.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/circos.py
+-rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/comparative_matrices.py
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/corces.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/covid.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/genes.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/heatmap.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/ideograms.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/line_chart.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/multiscale_lollipop_plot.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/multiscale_sequence.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/overview_detail.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/point_plot.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/examples/text_marks.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/schema/__init__.py
+-rw-r--r--   0        0        0    32752 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/schema/channels.py
+-rw-r--r--   0        0        0   106194 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/schema/core.py
+-rw-r--r--   0        0        0   305193 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/schema/gosling-schema.json
+-rw-r--r--   0        0        0    27321 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/schema/mixins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/sphinxext/__init__.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/sphinxext/gallery.py
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/sphinxext/plot.py
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/tests/test_api.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/tests/test_data.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/tests/test_plugin_registry.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/utils/__init__.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/utils/core.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 gosling-0.1.1/gosling/utils/execeval.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 gosling-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 gosling-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 gosling-0.1.1/README.md
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 gosling-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 gosling-0.1.1/PKG-INFO
```

### Comparing `gosling-0.1.0/gosling/__init__.py` & `gosling-0.1.1/gosling/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pandas as pd
 
 from gosling.schema import *
 from gosling.api import *
 from gosling.data import (
     GoslingDataServer,
     bam,
+    bed,
     beddb,
     bigwig,
     csv,
     data_server,
     json,
     matrix,
     multivec,
@@ -25,9 +26,9 @@
 @pd.api.extensions.register_dataframe_accessor("gos")  # type: ignore
 class GosAccessor:
     def __init__(self, df: pd.DataFrame):
         self._df = df
 
     def csv(self, **kwargs):
         content = self._df.to_csv(index=False) or ""
-        url = data_server(content, extension="csv")
+        url = data_server(content, extension=".csv")
         return dict(type="csv", url=url, **kwargs)
```

### Comparing `gosling-0.1.0/gosling/api.py` & `gosling-0.1.1/gosling/api.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/display.py` & `gosling-0.1.1/gosling/display.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/plugin_registry.py` & `gosling-0.1.1/gosling/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/schemapi.py` & `gosling-0.1.1/gosling/schemapi.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/data/__init__.py` & `gosling-0.1.1/gosling/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,13 +131,14 @@
     return dict(type="json", values=values, **kwargs)
 
 
 # file resources
 bam = _create_loader("bam")
 csv = _create_loader("csv")
 bigwig = _create_loader("bigwig")
+bed = _create_loader("bed")
 
 # tileset resources
 beddb = _create_loader("beddb", tilesets.beddb)
 vector = _create_loader("vector", tilesets.bigwig)
 matrix = _create_loader("matrix", tilesets.cooler)
 multivec = _create_loader("multivec", tilesets.multivec)
```

### Comparing `gosling-0.1.0/gosling/data/_tilesets.py` & `gosling-0.1.1/gosling/data/_tilesets.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/data/tests/test_data_server.py` & `gosling-0.1.1/gosling/data/tests/test_data_server.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/area_chart.py` & `gosling-0.1.1/gosling/examples/area_chart.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/bar_chart.py` & `gosling-0.1.1/gosling/examples/bar_chart.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/between_link_pandas.py` & `gosling-0.1.1/gosling/examples/between_link_pandas.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/brushing_and_linking.py` & `gosling-0.1.1/gosling/examples/brushing_and_linking.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/circos.py` & `gosling-0.1.1/gosling/examples/circos.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/comparative_matrices.py` & `gosling-0.1.1/gosling/examples/comparative_matrices.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/corces.py` & `gosling-0.1.1/gosling/examples/corces.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/covid.py` & `gosling-0.1.1/gosling/examples/covid.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/genes.py` & `gosling-0.1.1/gosling/examples/genes.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/ideograms.py` & `gosling-0.1.1/gosling/examples/ideograms.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/line_chart.py` & `gosling-0.1.1/gosling/examples/line_chart.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/multiscale_lollipop_plot.py` & `gosling-0.1.1/gosling/examples/multiscale_lollipop_plot.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/multiscale_sequence.py` & `gosling-0.1.1/gosling/examples/multiscale_sequence.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/overview_detail.py` & `gosling-0.1.1/gosling/examples/overview_detail.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/point_plot.py` & `gosling-0.1.1/gosling/examples/point_plot.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/examples/text_marks.py` & `gosling-0.1.1/gosling/examples/text_marks.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/schema/channels.py` & `gosling-0.1.1/gosling/schema/channels.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/schema/core.py` & `gosling-0.1.1/gosling/schema/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,17 +170,17 @@
         super(Color, self).__init__(domain=domain, field=field, legend=legend, range=range, scale=scale,
                                     scaleOffset=scaleOffset, title=title, type=type, **kwds)
 
 
 class DataDeep(GoslingSchema):
     """DataDeep schema wrapper
 
-    anyOf(:class:`JsonData`, :class:`CsvData`, :class:`BigWigData`, :class:`MultivecData`,
-    :class:`BeddbData`, :class:`VectorData`, :class:`MatrixData`, :class:`BamData`,
-    :class:`VcfData`)
+    anyOf(:class:`JsonData`, :class:`CsvData`, :class:`BedData`, :class:`BigWigData`,
+    :class:`MultivecData`, :class:`BeddbData`, :class:`VectorData`, :class:`MatrixData`,
+    :class:`BamData`, :class:`VcfData`)
     """
     _schema = {'$ref': '#/definitions/DataDeep'}
     _rootschema = GoslingSchema._rootschema
 
     def __init__(self, *args, **kwds):
         super(DataDeep, self).__init__(*args, **kwds)
 
@@ -219,14 +219,47 @@
                  junctionMinCoverage=Undefined, loadMates=Undefined, maxInsertSize=Undefined, **kwds):
         super(BamData, self).__init__(indexUrl=indexUrl, type=type, url=url,
                                       extractJunction=extractJunction,
                                       junctionMinCoverage=junctionMinCoverage, loadMates=loadMates,
                                       maxInsertSize=maxInsertSize, **kwds)
 
 
+class BedData(DataDeep):
+    """BedData schema wrapper
+
+    Mapping(required=[type, url, indexUrl])
+    BED file format
+
+    Attributes
+    ----------
+
+    indexUrl : string
+        Specify the URL address of the data file index.
+    type : string
+
+    url : string
+        Specify the URL address of the data file.
+    customFields : List(string)
+        An array of strings, where each string is the name of a non-standard field in the
+        BED file. If there are `n` custom fields, we assume that the last `n` columns of the
+        BED file correspond to the custom fields.
+    sampleLength : float
+        Specify the number of rows loaded from the URL.
+
+        __Default:__ `1000`
+    """
+    _schema = {'$ref': '#/definitions/BedData'}
+    _rootschema = GoslingSchema._rootschema
+
+    def __init__(self, indexUrl=Undefined, type=Undefined, url=Undefined, customFields=Undefined,
+                 sampleLength=Undefined, **kwds):
+        super(BedData, self).__init__(indexUrl=indexUrl, type=type, url=url, customFields=customFields,
+                                      sampleLength=sampleLength, **kwds)
+
+
 class BeddbData(DataDeep):
     """BeddbData schema wrapper
 
     Mapping(required=[type, url, genomicFields])
     Regular BED or similar files can be pre-aggregated for the scalable data exploration. Find
     our more about this format at [HiGlass
     Docs](https://docs.higlass.io/data_preparation.html#bed-files).
@@ -305,15 +338,16 @@
     type : string
 
     url : string
         Specify the URL address of the data file.
     chromosomeField : string
         Specify the name of chromosome data fields.
     chromosomePrefix : string
-        experimental
+        Specify the chromosome prefix if chromosomes are denoted using a prefix besides
+        "chr" or a number
     genomicFields : List(string)
         Specify the name of genomic data fields.
     genomicFieldsToConvert : List(Mapping(required=[chromosomeField, genomicFields]))
         experimental
     headerNames : List(string)
         Specify the names of data fields if a CSV file does not contain a header.
     longToWideId : string
```

### Comparing `gosling-0.1.0/gosling/schema/gosling-schema.json` & `gosling-0.1.1/gosling/schema/gosling-schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978084935897437%*

 * *Differences: {"'definitions'": "{'CsvData': {'properties': {'chromosomePrefix': {'description': 'Specify the "*

 * *                  'chromosome prefix if chromosomes are denoted using a prefix besides "chr" or a '*

 * *                  "number'}}}, 'DataDeep': {'anyOf': {insert: [(2, OrderedDict([('$ref', "*

 * *                  "'#/definitions/BedData')]))]}}, 'BedData': "*

 * *                  "OrderedDict([('additionalProperties', False), ('description', 'BED file "*

 * *                  "format'), ('properties', OrderedDict([('customF […]*

```diff
@@ -97,14 +97,49 @@
             "required": [
                 "type",
                 "url",
                 "indexUrl"
             ],
             "type": "object"
         },
+        "BedData": {
+            "additionalProperties": false,
+            "description": "BED file format",
+            "properties": {
+                "customFields": {
+                    "description": "An array of strings, where each string is the name of a non-standard field in the BED file. If there are `n` custom fields, we assume that the last `n` columns of the BED file correspond to the custom fields.",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "indexUrl": {
+                    "description": "Specify the URL address of the data file index.",
+                    "type": "string"
+                },
+                "sampleLength": {
+                    "description": "Specify the number of rows loaded from the URL.\n\n__Default:__ `1000`",
+                    "type": "number"
+                },
+                "type": {
+                    "const": "bed",
+                    "type": "string"
+                },
+                "url": {
+                    "description": "Specify the URL address of the data file.",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "type",
+                "url",
+                "indexUrl"
+            ],
+            "type": "object"
+        },
         "BeddbData": {
             "additionalProperties": false,
             "description": "Regular BED or similar files can be pre-aggregated for the scalable data exploration. Find our more about this format at [HiGlass Docs](https://docs.higlass.io/data_preparation.html#bed-files).",
             "properties": {
                 "exonIntervalFields": {
                     "description": "experimental",
                     "items": [
@@ -416,15 +451,15 @@
             "description": "Any small enough tabular data files, such as tsv, csv, BED, BEDPE, and GFF, can be loaded using \"csv\" data specification.",
             "properties": {
                 "chromosomeField": {
                     "description": "Specify the name of chromosome data fields.",
                     "type": "string"
                 },
                 "chromosomePrefix": {
-                    "description": "experimental",
+                    "description": "Specify the chromosome prefix if chromosomes are denoted using a prefix besides \"chr\" or a number",
                     "type": "string"
                 },
                 "genomicFields": {
                     "description": "Specify the name of genomic data fields.",
                     "items": {
                         "type": "string"
                     },
@@ -492,14 +527,17 @@
                 {
                     "$ref": "#/definitions/JsonData"
                 },
                 {
                     "$ref": "#/definitions/CsvData"
                 },
                 {
+                    "$ref": "#/definitions/BedData"
+                },
+                {
                     "$ref": "#/definitions/BigWigData"
                 },
                 {
                     "$ref": "#/definitions/MultivecData"
                 },
                 {
                     "$ref": "#/definitions/BeddbData"
```

### Comparing `gosling-0.1.0/gosling/schema/mixins.py` & `gosling-0.1.1/gosling/schema/mixins.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/sphinxext/gallery.py` & `gosling-0.1.1/gosling/sphinxext/gallery.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/sphinxext/plot.py` & `gosling-0.1.1/gosling/sphinxext/plot.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/tests/test_api.py` & `gosling-0.1.1/gosling/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/tests/test_data.py` & `gosling-0.1.1/gosling/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/tests/test_plugin_registry.py` & `gosling-0.1.1/gosling/tests/test_plugin_registry.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/utils/core.py` & `gosling-0.1.1/gosling/utils/core.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/gosling/utils/execeval.py` & `gosling-0.1.1/gosling/utils/execeval.py`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/LICENSE` & `gosling-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/README.md` & `gosling-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gosling-0.1.0/pyproject.toml` & `gosling-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -59,7 +59,8 @@
 [tool.hatch.envs.default]
 features = ["dev", "all"]
 
 [tool.hatch.envs.default.scripts]
 test = "pytest --ignore gosling/examples --ignore tools/altair --doctest-modules gosling"
 clean = "rm -rf doc/_build doc/user_guide/generated/ doc/gallery"
 docs = "sphinx-build -b html doc dist"
+generate-schema-wrapper = "python tools/generate_schema_wrapper.py"
```

### Comparing `gosling-0.1.0/PKG-INFO` & `gosling-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gosling
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python bindings to generate Gosling visualizations
 Project-URL: homepage, https://github.com/gosling-lang/gos
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

