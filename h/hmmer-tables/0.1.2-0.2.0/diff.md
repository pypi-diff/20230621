# Comparing `tmp/hmmer_tables-0.1.2.tar.gz` & `tmp/hmmer_tables-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmmer_tables-0.1.2.tar", max compression
+gzip compressed data, was "hmmer_tables-0.2.0.tar", max compression
```

## Comparing `hmmer_tables-0.1.2.tar` & `hmmer_tables-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/LICENSE
--rw-r--r--   0        0        0       15 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/hmmer_tables/__init__.py
--rw-r--r--   0        0        0      319 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/hmmer_tables/csv_iter.py
--rw-r--r--   0        0        0     3038 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/hmmer_tables/domtbl.py
--rw-r--r--   0        0        0     1885 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/hmmer_tables/interval.py
--rw-r--r--   0        0        0       72 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/hmmer_tables/path_like.py
--rw-r--r--   0        0        0     1747 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/hmmer_tables/tbl.py
--rw-r--r--   0        0        0      442 2023-06-19 10:44:39.025516 hmmer_tables-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 hmmer_tables-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-21 14:58:44.943275 hmmer_tables-0.2.0/LICENSE
+-rw-r--r--   0        0        0       15 2023-06-21 14:58:44.943275 hmmer_tables-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/hmmer_tables/__init__.py
+-rw-r--r--   0        0        0      367 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/hmmer_tables/csv_iter.py
+-rw-r--r--   0        0        0     3152 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/hmmer_tables/domtbl.py
+-rw-r--r--   0        0        0     1885 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/hmmer_tables/interval.py
+-rw-r--r--   0        0        0       72 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/hmmer_tables/path_like.py
+-rw-r--r--   0        0        0     1880 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/hmmer_tables/tbl.py
+-rw-r--r--   0        0        0      442 2023-06-21 14:58:44.947275 hmmer_tables-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 hmmer_tables-0.2.0/PKG-INFO
```

### Comparing `hmmer_tables-0.1.2/LICENSE` & `hmmer_tables-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.1.2/hmmer_tables/domtbl.py` & `hmmer_tables-0.2.0/hmmer_tables/domtbl.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dataclasses
-from typing import List
+from typing import List, Iterable
 
 from pydantic import BaseModel
 
 from hmmer_tables.csv_iter import csv_iter
 from hmmer_tables.interval import PyInterval, RInterval
 from hmmer_tables.path_like import PathLike
 
@@ -85,43 +85,48 @@
     def __iter__(self):
         return iter(self._asdict().values())
 
     def _field_types(self):
         return {f.name: f.type for f in dataclasses.fields(self)}
 
 
-def read_domtbl(filename: PathLike) -> List[DomTBLRow]:
+def _read_domtbl_stream(stream: Iterable[str]):
+    rows = []
+    for x in csv_iter(stream):
+        seq_score = DomTBLSeqScore(
+            e_value=float(x[6]), score=float(x[7]), bias=float(x[8])
+        )
+        domain = DomTBLDomScore(
+            id=int(x[9]),
+            size=int(x[10]),
+            c_value=float(x[11]),
+            i_value=float(x[12]),
+            score=float(x[13]),
+            bias=float(x[14]),
+        )
+        row = DomTBLRow(
+            target=DomTBLIndex(name=x[0], accession=x[1], length=int(x[2])),
+            query=DomTBLIndex(name=x[3], accession=x[4], length=int(x[5])),
+            full_sequence=seq_score,
+            domain=domain,
+            hmm_coord=DomTBLCoord(start=int(x[15]), stop=int(x[16])),
+            ali_coord=DomTBLCoord(start=int(x[17]), stop=int(x[18])),
+            env_coord=DomTBLCoord(start=int(x[19]), stop=int(x[20])),
+            acc=float(x[21]),
+            description=" ".join(x[22:]),
+        )
+        rows.append(row)
+    return rows
+
+
+def read_domtbl(
+    filename: PathLike | None = None, stream: Iterable[str] | None = None
+) -> List[DomTBLRow]:
     """
     Read domtbl file type.
-
-    Parameters
-    ----------
-    file
-        File path or file stream.
     """
-    rows = []
-    with open(filename, "r") as file:
-        for x in csv_iter(file):
-            seq_score = DomTBLSeqScore(
-                e_value=float(x[6]), score=float(x[7]), bias=float(x[8])
-            )
-            domain = DomTBLDomScore(
-                id=int(x[9]),
-                size=int(x[10]),
-                c_value=float(x[11]),
-                i_value=float(x[12]),
-                score=float(x[13]),
-                bias=float(x[14]),
-            )
-            row = DomTBLRow(
-                target=DomTBLIndex(name=x[0], accession=x[1], length=int(x[2])),
-                query=DomTBLIndex(name=x[3], accession=x[4], length=int(x[5])),
-                full_sequence=seq_score,
-                domain=domain,
-                hmm_coord=DomTBLCoord(start=int(x[15]), stop=int(x[16])),
-                ali_coord=DomTBLCoord(start=int(x[17]), stop=int(x[18])),
-                env_coord=DomTBLCoord(start=int(x[19]), stop=int(x[20])),
-                acc=float(x[21]),
-                description=" ".join(x[22:]),
-            )
-            rows.append(row)
-    return rows
+    if filename is not None:
+        assert stream is None
+        with open(filename, "r") as stream:
+            return _read_domtbl_stream(stream)
+    else:
+        return _read_domtbl_stream(stream)
```

### Comparing `hmmer_tables-0.1.2/hmmer_tables/interval.py` & `hmmer_tables-0.2.0/hmmer_tables/interval.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.1.2/PKG-INFO` & `hmmer_tables-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmmer-tables
-Version: 0.1.2
+Version: 0.2.0
 Summary: Read tables produced by HMMER software.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

