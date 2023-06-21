# Comparing `tmp/oxrdflib-0.3.4.tar.gz` & `tmp/oxrdflib-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxrdflib-0.3.4.tar", last modified: Sat Apr 22 05:32:22 2023, max compression
+gzip compressed data, was "oxrdflib-0.3.5.tar", last modified: Wed Jun 21 19:54:38 2023, max compression
```

## Comparing `oxrdflib-0.3.4.tar` & `oxrdflib-0.3.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/oxrdflib/
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/oxrdflib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/oxrdflib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/oxrdflib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-22 05:32:22.000000 oxrdflib-0.3.4/oxrdflib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-22 05:32:22.000000 oxrdflib-0.3.4/oxrdflib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 05:32:22.000000 oxrdflib-0.3.4/oxrdflib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-22 05:32:22.000000 oxrdflib-0.3.4/oxrdflib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-22 05:32:22.000000 oxrdflib-0.3.4/oxrdflib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 05:32:22.000000 oxrdflib-0.3.4/oxrdflib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:32:22.679813 oxrdflib-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/tests/test_graph_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/tests/test_sparql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-22 05:32:13.000000 oxrdflib-0.3.4/tests/test_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:38.870157 oxrdflib-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:38.866157 oxrdflib-0.3.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:38.866157 oxrdflib-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-21 19:54:38.870157 oxrdflib-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:38.866157 oxrdflib-0.3.5/oxrdflib/
+-rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/oxrdflib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/oxrdflib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:38.870157 oxrdflib-0.3.5/oxrdflib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-21 19:54:38.000000 oxrdflib-0.3.5/oxrdflib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-21 19:54:38.000000 oxrdflib-0.3.5/oxrdflib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:54:38.000000 oxrdflib-0.3.5/oxrdflib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-21 19:54:38.000000 oxrdflib-0.3.5/oxrdflib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 19:54:38.000000 oxrdflib-0.3.5/oxrdflib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 19:54:38.000000 oxrdflib-0.3.5/oxrdflib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:54:38.870157 oxrdflib-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:54:38.870157 oxrdflib-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/tests/test_graph_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/tests/test_sparql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-21 19:54:29.000000 oxrdflib-0.3.5/tests/test_store.py
```

### Comparing `oxrdflib-0.3.4/.github/workflows/build.yml` & `oxrdflib-0.3.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.4/.pre-commit-config.yaml` & `oxrdflib-0.3.5/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -20,19 +20,19 @@
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: fix-byte-order-marker
       - id: mixed-line-ending
       - id: requirements-txt-fixer
       - id: trailing-whitespace
   - repo: https://github.com/ambv/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.257
+    rev: v0.0.272
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.3.0
     hooks:
       - id: mypy
```

### Comparing `oxrdflib-0.3.4/CHANGELOG.md` & `oxrdflib-0.3.5/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+## [0.3.5] - 2023-06-21
+
+### Changed
+- Fixes `Store.triples` and `Store.context` return types.
+
+
 ## [0.3.4] - 2023-04-22
 
 ### Changed
 - Fixes support of rdflib `Query` object in `Store.query`.
 
 
 ## [0.3.3] - 2023-03-20
 
 ### Added
 - Implements directly `Store.addN` method.
-- Allows to Allows to inject the `pyoxigraph.Store` object directly into `OxigraphStore`.
+- Allows to inject the `pyoxigraph.Store` object directly into `OxigraphStore`.
 
 ### Changed
 - Migrates setuptools configuration to `pyproject.toml`.
 - Adds type annotation.
 
 
 ## [0.3.2] - 2022-08-03
```

### Comparing `oxrdflib-0.3.4/LICENSE.md` & `oxrdflib-0.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.4/PKG-INFO` & `oxrdflib-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxrdflib
-Version: 0.3.4
+Version: 0.3.5
 Summary: rdflib stores based on pyoxigraph
 Author-email: Tpt <thomas@pellissier-tanon.fr>
 License: BSD-3-Clause
 Project-URL: Changelog, https://github.com/oxigraph/oxrdflib/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/oxigraph/oxrdflib/blob/main/README.md
 Project-URL: Homepage, https://github.com/oxigraph/oxrdflib
 Project-URL: Source, https://github.com/oxigraph/oxrdflib
```

### Comparing `oxrdflib-0.3.4/README.md` & `oxrdflib-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.4/oxrdflib/__init__.py` & `oxrdflib-0.3.5/oxrdflib/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -82,26 +82,34 @@
         super().remove(triple, context)
 
     def triples(
         self,
         triple_pattern: _TriplePattern,
         context: Optional[Graph] = None,
     ) -> Iterator[Tuple[_Triple, Iterator[Optional[Graph]]]]:
-        return (_from_ox(q) for q in self._inner.quads_for_pattern(*_to_ox_quad_pattern(triple_pattern, context)))
+        return (
+            (
+                (_from_ox(q.subject), _from_ox(q.predicate), _from_ox(q.object)),
+                iter(((_from_ox_graph_name(q.graph_name, self) if q.graph_name != ox.DefaultGraph() else None),)),
+            )
+            for q in self._inner.quads_for_pattern(*_to_ox_quad_pattern(triple_pattern, context))
+        )
 
     def __len__(self, context: Optional[Graph] = None) -> int:
         if context is None:
             # TODO: very bad
             return len({q.triple for q in self._inner})
         return sum(1 for _ in self._inner.quads_for_pattern(None, None, None, _to_ox(context)))
 
     def contexts(self, triple: Optional[_Triple] = None) -> Generator[Graph, None, None]:
         if triple is None:
-            return (_from_ox(g) for g in self._inner.named_graphs())
-        return (_from_ox(q[3]) for q in self._inner.quads_for_pattern(*_to_ox_quad_pattern(triple)))
+            return (_from_ox_graph_name(g, self) for g in self._inner.named_graphs())
+        return (
+            _from_ox_graph_name(q.graph_name, self) for q in self._inner.quads_for_pattern(*_to_ox_quad_pattern(triple))
+        )
 
     def query(
         self,
         query: Union[Query, str],
         initNs: Mapping[str, Any],  # noqa: N803
         initBindings: Mapping[str, Identifier],  # noqa: N803
         queryGraph: str,  # noqa: N803
@@ -187,15 +195,17 @@
     def namespace(self, prefix: str) -> Optional[URIRef]:
         return self._namespace_for_prefix.get(prefix)
 
     def namespaces(self) -> Iterator[Tuple[str, URIRef]]:
         yield from self._namespace_for_prefix.items()
 
 
-def _to_ox(term: Union[Node, _Triple, _Quad, Graph], context: Optional[Graph] = None):
+def _to_ox(
+    term: Optional[Union[Node, _Triple, _Quad, Graph]], context: Optional[Graph] = None
+) -> Optional[Union[ox.NamedNode, ox.BlankNode, ox.Literal, ox.DefaultGraph, ox.Quad]]:
     if term is None:
         return None
     if term == DATASET_DEFAULT_GRAPH_ID:
         return ox.DefaultGraph()
     if isinstance(term, URIRef):
         return ox.NamedNode(term)
     if isinstance(term, BNode):
@@ -205,47 +215,57 @@
     if isinstance(term, Graph):
         return _to_ox(term.identifier)
     if isinstance(term, tuple):
         if len(term) == 3:
             return ox.Quad(_to_ox(term[0]), _to_ox(term[1]), _to_ox(term[2]), _to_ox(context))
         if len(term) == 4:
             return ox.Quad(_to_ox(term[0]), _to_ox(term[1]), _to_ox(term[2]), _to_ox(term[3]))
-    raise ValueError(f"Unexpected rdflib term: {repr(term)}")
+    raise ValueError(f"Unexpected rdflib term: {term!r}")
 
 
 def _to_ox_quad_pattern(triple: _TriplePattern, context: Optional[Graph] = None):
     (s, p, o) = triple
     return _to_ox_term_pattern(s), _to_ox_term_pattern(p), _to_ox_term_pattern(o), _to_ox_term_pattern(context)
 
 
-def _to_ox_term_pattern(term):
+def _to_ox_term_pattern(
+    term: Optional[Union[URIRef, BNode, Literal, Graph]]
+) -> Optional[Union[ox.NamedNode, ox.BlankNode, ox.Literal]]:
     if term is None:
         return None
     if isinstance(term, URIRef):
         return ox.NamedNode(term)
     if isinstance(term, BNode):
         return ox.BlankNode(term)
     if isinstance(term, Literal):
         return ox.Literal(term, language=term.language, datatype=ox.NamedNode(term.datatype) if term.datatype else None)
     if isinstance(term, Graph):
         return _to_ox(term.identifier)
-    raise ValueError(f"Unexpected rdflib term: {repr(term)}")
+    raise ValueError(f"Unexpected rdflib term: {term!r}")
 
 
-def _from_ox(term):
+def _from_ox_graph_name(graph_name: Union[ox.NamedNode, ox.BlankNode, ox.DefaultGraph], store: OxigraphStore) -> Graph:
+    if isinstance(graph_name, ox.NamedNode):
+        return Graph(identifier=URIRef(graph_name.value), store=store)
+    if isinstance(graph_name, ox.BlankNode):
+        return Graph(identifier=BNode(graph_name.value), store=store)
+    if isinstance(graph_name, ox.DefaultGraph):
+        return Graph(identifier=DATASET_DEFAULT_GRAPH_ID, store=store)
+    raise ValueError(f"Unexpected Oxigraph graph name: {graph_name!r}")
+
+
+def _from_ox(
+    term: Optional[Union[ox.NamedNode, ox.BlankNode, ox.Literal, ox.Triple]]
+) -> Optional[Union[Node, Tuple[Node, Node, Node]]]:
     if term is None:
         return None
     if isinstance(term, ox.NamedNode):
         return URIRef(term.value)
     if isinstance(term, ox.BlankNode):
         return BNode(term.value)
     if isinstance(term, ox.Literal):
         if term.language:
             return Literal(term.value, lang=term.language)
         return Literal(term.value, datatype=URIRef(term.datatype.value))
-    if isinstance(term, ox.DefaultGraph):
-        return None
     if isinstance(term, ox.Triple):
         return _from_ox(term.subject), _from_ox(term.predicate), _from_ox(term.object)
-    if isinstance(term, ox.Quad):
-        return (_from_ox(term.subject), _from_ox(term.predicate), _from_ox(term.object)), _from_ox(term.graph_name)
-    raise ValueError(f"Unexpected Oxigraph term: {repr(term)}")
+    raise ValueError(f"Unexpected Oxigraph term: {term!r}")
```

### Comparing `oxrdflib-0.3.4/oxrdflib.egg-info/PKG-INFO` & `oxrdflib-0.3.5/oxrdflib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxrdflib
-Version: 0.3.4
+Version: 0.3.5
 Summary: rdflib stores based on pyoxigraph
 Author-email: Tpt <thomas@pellissier-tanon.fr>
 License: BSD-3-Clause
 Project-URL: Changelog, https://github.com/oxigraph/oxrdflib/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/oxigraph/oxrdflib/blob/main/README.md
 Project-URL: Homepage, https://github.com/oxigraph/oxrdflib
 Project-URL: Source, https://github.com/oxigraph/oxrdflib
```

### Comparing `oxrdflib-0.3.4/pyproject.toml` & `oxrdflib-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.4/tests/test_dataset.py` & `oxrdflib-0.3.5/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.4/tests/test_graph.py` & `oxrdflib-0.3.5/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.4/tests/test_graph_context.py` & `oxrdflib-0.3.5/tests/test_graph_context.py`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.4/tests/test_sparql.py` & `oxrdflib-0.3.5/tests/test_sparql.py`

 * *Files identical despite different names*

### Comparing `oxrdflib-0.3.4/tests/test_store.py` & `oxrdflib-0.3.5/tests/test_store.py`

 * *Files identical despite different names*

