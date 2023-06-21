# Comparing `tmp/clarusui-0.8-py2.py3-none-any.whl.zip` & `tmp/clarusui-0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 11703 bytes, number of entries: 19
+Zip file size: 11711 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx       81 b- defN 17-Oct-05 17:57 clarusui/base_content.html
 -rw-rw-r--  2.0 unx      211 b- defN 17-Oct-06 13:24 clarusui/__init__.py
 -rw-rw-r--  2.0 unx     7056 b- defN 17-Oct-06 12:26 clarusui/layout.py
 -rw-rw-r--  2.0 unx     5208 b- defN 17-Oct-06 12:26 clarusui/table.py
 -rw-rw-r--  2.0 unx       19 b- defN 17-Oct-05 17:57 clarusui/version.py
 -rw-rw-r--  2.0 unx      114 b- defN 17-Oct-05 17:57 clarusui/iframe.html
 -rw-rw-r--  2.0 unx     6527 b- defN 17-Oct-06 12:26 clarusui/chart.py
 -rw-rw-r--  2.0 unx      479 b- defN 17-Oct-05 17:57 clarusui/table.html
 -rw-rw-r--  2.0 unx       71 b- defN 17-Oct-05 17:57 clarusui/div.html
--rw-rw-r--  2.0 unx     1183 b- defN 17-Oct-05 17:57 clarusui/base.html
+-rw-rw-r--  2.0 unx     1210 b- defN 17-Oct-06 17:13 clarusui/base.html
 -rw-rw-r--  2.0 unx      426 b- defN 17-Oct-05 17:57 clarusui/layout.html
 -rw-rw-r--  2.0 unx     4339 b- defN 17-Oct-05 17:57 clarusui/colours.py
 -rw-rw-r--  2.0 unx      784 b- defN 17-Oct-06 12:26 clarusui/iframe.py
--rw-rw-r--  2.0 unx       10 b- defN 17-Oct-06 14:49 clarusui-0.8.dist-info/DESCRIPTION.rst
--rw-rw-r--  2.0 unx      451 b- defN 17-Oct-06 14:49 clarusui-0.8.dist-info/metadata.json
--rw-rw-r--  2.0 unx        9 b- defN 17-Oct-06 14:49 clarusui-0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      110 b- defN 17-Oct-06 14:49 clarusui-0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx      273 b- defN 17-Oct-06 14:49 clarusui-0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx     1475 b- defN 17-Oct-06 14:49 clarusui-0.8.dist-info/RECORD
-19 files, 28826 bytes uncompressed, 9345 bytes compressed:  67.6%
+-rw-rw-r--  2.0 unx       10 b- defN 17-Oct-06 17:16 clarusui-0.9.dist-info/DESCRIPTION.rst
+-rw-rw-r--  2.0 unx      451 b- defN 17-Oct-06 17:16 clarusui-0.9.dist-info/metadata.json
+-rw-rw-r--  2.0 unx        9 b- defN 17-Oct-06 17:16 clarusui-0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      110 b- defN 17-Oct-06 17:16 clarusui-0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      273 b- defN 17-Oct-06 17:16 clarusui-0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx     1475 b- defN 17-Oct-06 17:16 clarusui-0.9.dist-info/RECORD
+19 files, 28853 bytes uncompressed, 9353 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -33,26 +33,26 @@
 
 Filename: clarusui/colours.py
 Comment: 
 
 Filename: clarusui/iframe.py
 Comment: 
 
-Filename: clarusui-0.8.dist-info/DESCRIPTION.rst
+Filename: clarusui-0.9.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: clarusui-0.8.dist-info/metadata.json
+Filename: clarusui-0.9.dist-info/metadata.json
 Comment: 
 
-Filename: clarusui-0.8.dist-info/top_level.txt
+Filename: clarusui-0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: clarusui-0.8.dist-info/WHEEL
+Filename: clarusui-0.9.dist-info/WHEEL
 Comment: 
 
-Filename: clarusui-0.8.dist-info/METADATA
+Filename: clarusui-0.9.dist-info/METADATA
 Comment: 
 
-Filename: clarusui-0.8.dist-info/RECORD
+Filename: clarusui-0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clarusui/base.html

```diff
@@ -14,19 +14,21 @@
 </head>
 <body>
 <div class="container-fluid">
 {% block body %}{% endblock %}
 </div>
 
 <script>
-var pl = document.getElementsByClassName("plotly-graph-div")
-for (var i = 0; i < pl.length; i++) {
-	var chartDiv = document.getElementById(pl[i].id);
-	addResizeListener(chartDiv)
-}
+$(function() {
+	var pl = document.getElementsByClassName("plotly-graph-div")
+	for (var i = 0; i < pl.length; i++) {
+		var chartDiv = document.getElementById(pl[i].id);
+		addResizeListener(chartDiv)
+	}
+	});
 function addResizeListener(chartDiv){
 	window.addEventListener('resize', function() { Plotly.Plots.resize(chartDiv); });
 }
 </script>
 </body>
 </html>
```

## Comparing `clarusui-0.8.dist-info/RECORD` & `clarusui-0.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 clarusui/__init__.py,sha256=zvyfvF0mJ0Fioj0aiX7h0xC_RI-mrTg685BuOkpbMeg,211
-clarusui/base.html,sha256=_IADHQP_Twfb5Yma2M1oPYvfP2xxuhllos2gKME8gL0,1183
+clarusui/base.html,sha256=4sz3MUj9Bm8WkAIdfSqle2_KBiTz6B9d76FF_EH9644,1210
 clarusui/base_content.html,sha256=NPKW869hwWPCom0ION66_vl6twdbN6vV9pHp8QHwa5o,81
 clarusui/chart.py,sha256=JHB8cno5NCYLwjpisS3jrX-6VWWCOPAQp1Ejnhf40Pw,6527
 clarusui/colours.py,sha256=0imtcozMY-fWi-oJDAtyFbEpMCf5q1UtmiDihuLetH4,4339
 clarusui/div.html,sha256=pgLOfpB6BND-_kkM2cbj0C4NAWyEcTFiwSMAA5stiFM,71
 clarusui/iframe.html,sha256=I4YPh48Ub1dLP1oO6nULHCKtAi7aLDNqrrtRr5bZI84,114
 clarusui/iframe.py,sha256=JQyWjZKHV1TdmzA0CwohSmZzZ1_kcWT_jFMEwaPFaL0,784
 clarusui/layout.html,sha256=huMyaJ3PNMVTNnSXohr8kATu6ZHG7ocqEkL1C5NNUrM,426
 clarusui/layout.py,sha256=Mw-loYxmffGqwsgSvoIDZNx2Ose4nZkjozfKy-Cjkho,7056
 clarusui/table.html,sha256=XVLRkpMoJ-_J3Z2k_hZideKBZa85rGSqgoapE-CNIh4,479
 clarusui/table.py,sha256=Z3xHuY8dqkjUa04kQav4RtCn0BEv3pOJJZGchqMZiAE,5208
 clarusui/version.py,sha256=dTaMG_cL1ZhDIskmq1gg2YRVlKLYe3add4hcaOgkj98,19
-clarusui-0.8.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
-clarusui-0.8.dist-info/METADATA,sha256=UcK1Up5LEEt8pL1JolRiiaAT1zHiROrXNZulU7-chBI,273
-clarusui-0.8.dist-info/RECORD,,
-clarusui-0.8.dist-info/WHEEL,sha256=o2k-Qa-RMNIJmUdIc7KU6VWR_ErNRbWNlxDIpl7lm34,110
-clarusui-0.8.dist-info/metadata.json,sha256=A7rdIcLAoejI41D90sxsvYKGJEvIzeaAnUzTU3nNOCc,451
-clarusui-0.8.dist-info/top_level.txt,sha256=ABci4qEp2pLc0FuuqxBo_6lDhcrSoqJs7W21OGZt14Q,9
+clarusui-0.9.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
+clarusui-0.9.dist-info/METADATA,sha256=O9zUh1-iSLLY4DaixRsbXhsPT7s72u4WmceSW_8Mec4,273
+clarusui-0.9.dist-info/RECORD,,
+clarusui-0.9.dist-info/WHEEL,sha256=o2k-Qa-RMNIJmUdIc7KU6VWR_ErNRbWNlxDIpl7lm34,110
+clarusui-0.9.dist-info/metadata.json,sha256=8DHxtlDUMcukLNydBAEL95gIE3bp3cRA_luswt-_CV8,451
+clarusui-0.9.dist-info/top_level.txt,sha256=ABci4qEp2pLc0FuuqxBo_6lDhcrSoqJs7W21OGZt14Q,9
```

