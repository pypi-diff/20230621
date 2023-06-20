# Comparing `tmp/kisao-2.30.tar.gz` & `tmp/kisao-2.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kisao-2.30.tar", last modified: Sun Oct 10 02:09:26 2021, max compression
+gzip compressed data, was "kisao-2.32.tar", last modified: Tue Jun 20 22:03:48 2023, max compression
```

## Comparing `kisao-2.30.tar` & `kisao-2.32.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-10 02:09:26.131995 kisao-2.30/
--rw-r--r--   0 runner    (1001) docker     (121)     8672 2021-10-10 02:09:20.000000 kisao-2.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-10-10 02:08:35.000000 kisao-2.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5163 2021-10-10 02:09:26.131995 kisao-2.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4402 2021-10-10 02:09:20.000000 kisao-2.30/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-10 02:09:26.131995 kisao-2.30/kisao/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2021-10-10 02:08:35.000000 kisao-2.30/kisao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-10-10 02:08:35.000000 kisao-2.30/kisao/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5077 2021-10-10 02:08:35.000000 kisao-2.30/kisao/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     6275 2021-10-10 02:08:35.000000 kisao-2.30/kisao/data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2021-10-10 02:08:35.000000 kisao-2.30/kisao/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)  1089405 2021-10-10 02:09:20.000000 kisao-2.30/kisao/kisao.owl
--rw-r--r--   0 runner    (1001) docker     (121)    21848 2021-10-10 02:08:35.000000 kisao-2.30/kisao/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2021-10-10 02:08:35.000000 kisao-2.30/kisao/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-10 02:09:26.131995 kisao-2.30/kisao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5163 2021-10-10 02:09:26.000000 kisao-2.30/kisao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      349 2021-10-10 02:09:26.000000 kisao-2.30/kisao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-10 02:09:26.000000 kisao-2.30/kisao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-10-10 02:09:26.000000 kisao-2.30/kisao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-10-10 02:09:26.000000 kisao-2.30/kisao.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-10-10 02:08:35.000000 kisao-2.30/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-10-10 02:09:26.131995 kisao-2.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2021-10-10 02:08:35.000000 kisao-2.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:03:48.289625 kisao-2.32/
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-06-20 22:03:41.000000 kisao-2.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-20 22:03:02.000000 kisao-2.32/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-20 22:03:48.289625 kisao-2.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-20 22:03:41.000000 kisao-2.32/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:03:48.289625 kisao-2.32/kisao/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-20 22:03:02.000000 kisao-2.32/kisao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 22:03:02.000000 kisao-2.32/kisao/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-20 22:03:02.000000 kisao-2.32/kisao/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-20 22:03:02.000000 kisao-2.32/kisao/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-20 22:03:02.000000 kisao-2.32/kisao/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1114330 2023-06-20 22:03:41.000000 kisao-2.32/kisao/kisao.owl
+-rw-r--r--   0 runner    (1001) docker     (123)    22733 2023-06-20 22:03:02.000000 kisao-2.32/kisao/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-20 22:03:02.000000 kisao-2.32/kisao/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:03:48.289625 kisao-2.32/kisao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-20 22:03:48.000000 kisao-2.32/kisao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-20 22:03:48.000000 kisao-2.32/kisao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:03:48.000000 kisao-2.32/kisao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-20 22:03:48.000000 kisao-2.32/kisao.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 22:03:48.000000 kisao-2.32/kisao.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 22:03:02.000000 kisao-2.32/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 22:03:48.289625 kisao-2.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-20 22:03:02.000000 kisao-2.32/setup.py
```

### Comparing `kisao-2.30/LICENSE` & `kisao-2.32/LICENSE`

 * *Files identical despite different names*

### Comparing `kisao-2.30/PKG-INFO` & `kisao-2.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kisao
-Version: 2.30
+Version: 2.32
 Summary: Utilities for working with the Kinetic Simulation Algorithm Ontology (KiSAO)
 Home-page: https://github.com/SED-ML/kisao
 Author: SED-ML Editors
 Author-email: sed-ml-editors@googlegroups.com
 License: Apache 2.0
 Download-URL: https://github.com/SED-ML/kisao
 Keywords: systems biology,modeling,simulation,algorithm,ontology,KiSAO,SED-ML,SBML
```

### Comparing `kisao-2.30/README.rst` & `kisao-2.32/README.rst`

 * *Files identical despite different names*

### Comparing `kisao-2.30/kisao/core.py` & `kisao-2.32/kisao/core.py`

 * *Files identical despite different names*

### Comparing `kisao-2.30/kisao/data_model.py` & `kisao-2.32/kisao/data_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import collections
 import enum
 
 __all__ = [
     'ID_HAS_CHARACTERISTIC_RELATIONSHIP',
     'ID_ODE_PROBLEM_CHARACTERISTIC',
     'ID_SDE_PROBLEM_CHARACTERISTIC',
+    'ID_STEADYSTATE_PROBLEM_CHARACTERISTIC',
     'ID_PDE_PROBLEM_CHARACTERISTIC',
     'ID_EXACT_SOLUTION_CHARACTERISTIC',
     'ID_APPROXIMATE_SOLUTION_CHARACTERISTIC',
     'ID_ALGORITHM',
     'ID_GILLESPIE_LIKE_ALGORITHM',
     'ID_TAU_LEAPING_ALGORITHM',
     'ID_RULE_BASED_ALGORITHM',
@@ -32,14 +33,15 @@
     'ALGORITHM_SUBSTITUTION_POLICY_NAMES',
 ]
 
 ID_HAS_CHARACTERISTIC_RELATIONSHIP = 'KISAO_0000245'  # has characteristic
 
 ID_ODE_PROBLEM_CHARACTERISTIC = 'KISAO_0000374'  # ordinary differential equation problem
 ID_SDE_PROBLEM_CHARACTERISTIC = 'KISAO_0000371'  # stochastic differential equation problem
+ID_STEADYSTATE_PROBLEM_CHARACTERISTIC = 'KISAO_0000696'  # steady state root-finding problem
 ID_PDE_PROBLEM_CHARACTERISTIC = 'KISAO_0000372'  # partial differential equation problem
 ID_EXACT_SOLUTION_CHARACTERISTIC = 'KISAO_0000236'  # exact solution
 ID_APPROXIMATE_SOLUTION_CHARACTERISTIC = 'KISAO_0000237'  # approximate solution
 
 ID_ALGORITHM = 'KISAO_0000000'  # modelling and simulation algorithm
 ID_GILLESPIE_LIKE_ALGORITHM = 'KISAO_0000241'  # Gillespie-like method
 ID_TAU_LEAPING_ALGORITHM = 'KISAO_0000039'  # tau-leaping method
```

### Comparing `kisao-2.30/kisao/kisao.owl` & `kisao-2.32/kisao/kisao.owl`

 * *Files 0% similar despite different names*

#### Comparing `kisao-2.30/kisao/kisao.owl` & `kisao-2.32/kisao/kisao.owl`

```diff
@@ -1,18 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
-<rdf:RDF xmlns="http://www.biomodels.net/kisao/KISAO#" xmlns:ont="http://www.co-ode.org/ontologies/ont.owl#" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:kisao="http://www.biomodels.net/kisao/KISAO#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:protege="http://protege.stanford.edu/plugins/owl/protege#" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:skos="http://www.w3.org/2004/02/skos/core#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:obo="http://purl.obolibrary.org/obo/" xmlns:dc="http://purl.org/dc/terms/" xml:base="http://www.biomodels.net/kisao/KISAO">
+<rdf:RDF xmlns="http://www.biomodels.net/kisao/KISAO#" xmlns:dc="http://purl.org/dc/terms/" xmlns:obo="http://purl.obolibrary.org/obo/" xmlns:ont="http://www.co-ode.org/ontologies/ont.owl#" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:skos="http://www.w3.org/2004/02/skos/core#" xmlns:kisao="http://www.biomodels.net/kisao/KISAO#" xmlns:protege="http://protege.stanford.edu/plugins/owl/protege#" xml:base="http://www.biomodels.net/kisao/KISAO">
   <owl:Ontology rdf:about="http://www.biomodels.net/kisao/KISAO#">
+    <protege:defaultLanguage>en</protege:defaultLanguage>
     <dc:rights>Artistic License 2.0</dc:rights>
-    <rdfs:seeAlso rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/pubmed/22027554</rdfs:seeAlso>
+    <rdfs:comment xml:lang="en">This is a core version which contains all but deprecated classes.</rdfs:comment>
     <rdfs:label xml:lang="en">Kinetic Simulation Algorithm Ontology (KiSAO)</rdfs:label>
-    <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#decimal">2.30</owl:versionInfo>
     <rdfs:seeAlso rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://co.mbine.org/standards/kisao</rdfs:seeAlso>
-    <protege:defaultLanguage>en</protege:defaultLanguage>
+    <rdfs:seeAlso rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/pubmed/22027554</rdfs:seeAlso>
+    <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#decimal">2.32</owl:versionInfo>
     <skos:definition xml:lang="en">The Kinetic Simulation Algorithm Ontology (KiSAO) classifies algorithms available for the simulation and analysis of models in biology, and their characteristics and the parameters required for their use.</skos:definition>
-    <rdfs:comment xml:lang="en">This is a core version which contains all but deprecated classes.</rdfs:comment>
   </owl:Ontology>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Annotation properties
     //
     ///////////////////////////////////////////////////////////////////////////////////////
@@ -2263,15 +2263,15 @@
     <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000093"/>
     <owl:annotatedProperty rdf:resource="http://www.w3.org/2004/02/skos/core#altLabel"/>
     <owl:annotatedTarget xml:lang="en">Livermore solver for ordinary differential equations for stiff and nonstiff systems with krylov corrector iteration</owl:annotatedTarget>
     <rdfs:comment xml:lang="en">EXACT</rdfs:comment>
   </owl:Axiom>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000094 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000094">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000000"/>
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000694"/>
     <rdfs:subClassOf>
       <owl:Class>
         <owl:complementOf>
           <owl:Restriction>
             <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
             <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000102"/>
           </owl:Restriction>
@@ -2389,14 +2389,20 @@
     <dc:creator xml:lang="en">NLN</dc:creator>
     <rdfs:label xml:lang="en">discrete variable</rdfs:label>
     <skos:definition xml:lang="en">Algorithm, possessing this characteristic, allows values of system's variables to change by discrete (integral) amounts.</skos:definition>
   </owl:Class>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000106 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000106">
     <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000098"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000104"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2008-07-08</dc:created>
     <dc:creator xml:lang="en">NLN</dc:creator>
     <rdfs:label xml:lang="en">continuous variable</rdfs:label>
     <skos:definition xml:lang="en">Algorithm, possessing this characteristic, allows the values of a system's variables to change by continuous (non-integral) amounts.</skos:definition>
   </owl:Class>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000107 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000107">
@@ -3863,43 +3869,31 @@
     <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000285"/>
     <owl:annotatedProperty rdf:resource="http://www.w3.org/2004/02/skos/core#altLabel"/>
     <owl:annotatedTarget xml:lang="en">FVM</owl:annotatedTarget>
     <rdfs:comment xml:lang="en">EXACT</rdfs:comment>
   </owl:Axiom>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000286 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000286">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000377"/>
-    <rdfs:subClassOf>
-      <owl:Restriction>
-        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000104"/>
-      </owl:Restriction>
-    </rdfs:subClassOf>
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000697"/>
     <rdfs:subClassOf>
       <owl:Restriction>
         <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
         <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000106"/>
       </owl:Restriction>
     </rdfs:subClassOf>
     <rdfs:subClassOf>
       <owl:Restriction>
         <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000108"/>
-      </owl:Restriction>
-    </rdfs:subClassOf>
-    <rdfs:subClassOf>
-      <owl:Restriction>
-        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
         <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000240"/>
       </owl:Restriction>
     </rdfs:subClassOf>
     <rdfs:subClassOf>
       <owl:Restriction>
-        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000371"/>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000483"/>
       </owl:Restriction>
     </rdfs:subClassOf>
     <rdfs:subClassOf>
       <owl:Restriction>
         <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000361"/>
         <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000261"/>
       </owl:Restriction>
@@ -3921,33 +3915,27 @@
     <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000286"/>
     <owl:annotatedProperty rdf:resource="http://www.w3.org/2004/02/skos/core#altLabel"/>
     <owl:annotatedTarget xml:lang="en">stochastic Euler scheme</owl:annotatedTarget>
     <rdfs:comment xml:lang="en">EXACT</rdfs:comment>
   </owl:Axiom>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000287 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000287">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000281"/>
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000697"/>
     <rdfs:subClassOf>
       <owl:Restriction>
         <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000104"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000106"/>
       </owl:Restriction>
     </rdfs:subClassOf>
     <rdfs:subClassOf>
       <owl:Restriction>
         <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
         <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000240"/>
       </owl:Restriction>
     </rdfs:subClassOf>
-    <rdfs:subClassOf>
-      <owl:Restriction>
-        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000371"/>
-      </owl:Restriction>
-    </rdfs:subClassOf>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2011-05-10</dc:created>
     <dc:creator xml:lang="en">AZ</dc:creator>
     <rdfs:label xml:lang="en">Milstein method</rdfs:label>
     <rdfs:seeAlso rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/isbn/079233213X</rdfs:seeAlso>
     <skos:definition xml:lang="en">The Milstein method is a technique for the approximate numerical solution of a stochastic differential equation.</skos:definition>
   </owl:Class>
   <owl:Axiom>
@@ -6590,15 +6578,15 @@
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2011-07-19</dc:created>
     <dc:creator xml:lang="en">AZ</dc:creator>
     <rdfs:label xml:lang="en">linearity of equation</rdfs:label>
     <skos:definition xml:lang="en">Linear differential equations are of the form Ly = f, where the differential operator L is a linear operator, y is the unknown function, and the right hand side f is a given function of the same nature as y.</skos:definition>
   </owl:Class>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000377 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000377">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000000"/>
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000694"/>
     <rdfs:subClassOf>
       <owl:Class>
         <owl:complementOf>
           <owl:Restriction>
             <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
             <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000102"/>
           </owl:Restriction>
@@ -7141,15 +7129,14 @@
     <dc:creator xml:lang="en">AZ</dc:creator>
     <isOrganizational rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</isOrganizational>
     <rdfs:label xml:lang="en">type of differential equation</rdfs:label>
   </owl:Class>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000407 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000407">
     <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000000"/>
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000622"/>
     <rdfs:subClassOf>
       <owl:Restriction>
         <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
         <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000106"/>
       </owl:Restriction>
     </rdfs:subClassOf>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2012-01-17</dc:created>
@@ -7210,15 +7197,15 @@
     <rdfs:comment xml:lang="en">Deuflhard, P. Newton Methods for Nonlinear Problems: Affine Invariance and Adaptive Algorithms, Springer Series in Computational Mathematics, Vol. 35, 1st ed. 2004.</rdfs:comment>
   </owl:Axiom>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000410 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000410">
     <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000408"/>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2012-01-18</dc:created>
     <dc:creator xml:lang="en">AZ</dc:creator>
-    <rdfs:label xml:lang="en">simlified Newton method</rdfs:label>
+    <rdfs:label xml:lang="en">simplified Newton method</rdfs:label>
     <rdfs:seeAlso rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/isbn/9783540210993</rdfs:seeAlso>
     <skos:definition xml:lang="en">A 'Newton-type method' [http://identifiers.org/biomodels.kisao/KISAO_0000408] which is characterized by keeping the initial derivative throughout the whole iteration: F'(x[0])deltax[k]=-F(x[k]), x[k+1]=x[k]+deltax[k], k=0,1,...</skos:definition>
   </owl:Class>
   <owl:Axiom>
     <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000410"/>
     <owl:annotatedProperty rdf:resource="http://www.w3.org/2000/01/rdf-schema#seeAlso"/>
     <owl:annotatedTarget rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/isbn/9783540210993</owl:annotatedTarget>
@@ -7730,15 +7717,15 @@
     <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000432"/>
     <owl:annotatedProperty rdf:resource="http://www.w3.org/2000/01/rdf-schema#seeAlso"/>
     <owl:annotatedTarget rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/doi/10.1145/1089014.1089020</owl:annotatedTarget>
     <rdfs:comment xml:lang="en">Hindmarsh, A. C., et al., SUNDIALS: Suite of Nonlinear and Differential/Algebraic Equation Solvers, ACM Trans. Math. Softw., 31:363-396, 2005.</rdfs:comment>
   </owl:Axiom>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000433 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000433">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000000"/>
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000694"/>
     <rdfs:subClassOf>
       <owl:Class>
         <owl:unionOf rdf:parseType="Collection">
           <owl:Restriction>
             <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000360"/>
             <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000280"/>
           </owl:Restriction>
@@ -8215,14 +8202,20 @@
     <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000000"/>
     <rdfs:subClassOf>
       <owl:Restriction>
         <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
         <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000237"/>
       </owl:Restriction>
     </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000689"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2015-04-23</dc:created>
     <dc:creator xml:lang="en">AZ</dc:creator>
     <isOrganizational rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</isOrganizational>
     <rdfs:label xml:lang="en">optimization algorithm</rdfs:label>
     <rdfs:seeAlso rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://en.wikipedia.org/wiki/Mathematical_optimization#Optimization_algorithms</rdfs:seeAlso>
     <rdfs:seeAlso rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/isbn/0691102872</rdfs:seeAlso>
     <skos:altLabel xml:lang="en">optimization method</skos:altLabel>
@@ -10407,25 +10400,31 @@
     <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000563"/>
     <owl:annotatedProperty rdf:resource="http://www.w3.org/2000/01/rdf-schema#seeAlso"/>
     <owl:annotatedTarget rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/doi/10.5555/1218112.1218421</owl:annotatedTarget>
     <rdfs:comment xml:lang="en">Sven Sahle, Ralph Gauges, Jürgen Pahle, Natalia Simus, Ursula Kummer, Stefan Hoops, Christine Lee, Mudita Singhal, Liang Xu &amp; Pedro Mendes. Simulation of biochemical networks using COPASI—a complex pathway simulator. Proceedings of the 2006 Winter Simulation Conference, Monterey, CA, USA, 1698–1706 (2006).</rdfs:comment>
   </owl:Axiom>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000564 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000564">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000064"/>
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000697"/>
     <rdfs:subClassOf>
       <owl:Restriction>
-        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000104"/>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000483"/>
       </owl:Restriction>
     </rdfs:subClassOf>
     <rdfs:subClassOf>
       <owl:Restriction>
-        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000371"/>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000361"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000261"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000275"/>
+        <owl:someValuesFrom rdf:resource="http://www.w3.org/2001/XMLSchema#integer"/>
       </owl:Restriction>
     </rdfs:subClassOf>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2020-10-29</dc:created>
     <dc:creator xml:lang="en">JRK</dc:creator>
     <rdfs:label xml:lang="en">stochastic Runge-Kutta method</rdfs:label>
     <rdfs:seeAlso rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://en.wikipedia.org/wiki/Runge%E2%80%93Kutta_method_(SDE)</rdfs:seeAlso>
     <skos:definition xml:lang="en">Technique for the approximate numerical solution of a systems of stochastic differential equations (SDEs). The method is a generalisation of the Runge-Kutta method for ordinary differential equations to stochastic differential equations.</skos:definition>
@@ -11044,14 +11043,15 @@
     <owl:annotatedProperty rdf:resource="http://www.w3.org/2004/02/skos/core#altLabel"/>
     <owl:annotatedTarget xml:lang="en">Implicit-Explicit Runge-Kutta method</owl:annotatedTarget>
     <rdfs:comment xml:lang="en">EXACT</rdfs:comment>
   </owl:Axiom>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000588 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000588">
     <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000407"/>
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000622"/>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2020-10-29</dc:created>
     <dc:creator xml:lang="en">JRK</dc:creator>
     <isOrganizational rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</isOrganizational>
     <rdfs:label xml:lang="en">flux sampling</rdfs:label>
     <skos:definition xml:lang="en">Method for sampling fluxes from the null space of a flux balance analysis model</skos:definition>
   </owl:Class>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000589 -->
@@ -11772,15 +11772,21 @@
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2021-04-27</dc:created>
     <dc:creator xml:lang="en">JRK</dc:creator>
     <isOrganizational rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</isOrganizational>
     <rdfs:label xml:lang="en">stochastic simulation leaping method</rdfs:label>
   </owl:Class>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000622 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000622">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000000"/>
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000685"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000691"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2021--04-27</dc:created>
     <dc:creator xml:lang="en">JRK</dc:creator>
     <isOrganizational rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</isOrganizational>
     <rdfs:label xml:lang="en">flux balance method</rdfs:label>
   </owl:Class>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000623 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000623">
@@ -11870,14 +11876,20 @@
     <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000000"/>
     <rdfs:subClassOf>
       <owl:Restriction>
         <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
         <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000106"/>
       </owl:Restriction>
     </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000696"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2021-06-01</dc:created>
     <dc:creator xml:lang="en">JRK</dc:creator>
     <isOrganizational rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</isOrganizational>
     <rdfs:label xml:lang="en">root-finding method</rdfs:label>
     <skos:definition xml:lang="en">Method for finding the root of a function (f(x) = 0).</skos:definition>
   </owl:Class>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000631 -->
@@ -12359,14 +12371,21 @@
     <owl:annotatedProperty rdf:resource="http://www.w3.org/2000/01/rdf-schema#seeAlso"/>
     <owl:annotatedTarget rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://dl.acm.org/doi/10.5555/148286</owl:annotatedTarget>
     <rdfs:comment xml:lang="en">William H. Press, Saul A. Teukolsky, William T. Vetterling &amp; Brian P. Flannery. Numerical Recipes in C. The Art of Scientific Computing, 2nd Edition, 1992. Chapter 16. Pages 739-741.</rdfs:comment>
   </owl:Axiom>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000669 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000669">
     <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000407"/>
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000685"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000692"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2021-08-12</dc:created>
     <dc:creator xml:lang="en">JRK</dc:creator>
     <isImplementedIn rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/biosimulators/rbapy</isImplementedIn>
     <rdfs:label xml:lang="en">Resource Balance Analysis</rdfs:label>
     <rdfs:seeAlso rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://doi.org/10.1016/j.automatica.2011.02.038</rdfs:seeAlso>
     <skos:altLabel xml:lang="en">RBA</skos:altLabel>
   </owl:Class>
@@ -12604,14 +12623,349 @@
   </owl:Class>
   <owl:Axiom>
     <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000684"/>
     <owl:annotatedProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#isImplementedIn"/>
     <owl:annotatedTarget rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/biosimulators/bionetgen</owl:annotatedTarget>
     <rdfs:comment xml:lang="en">BioNetgen</rdfs:comment>
   </owl:Axiom>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000685 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000685">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000000"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000690"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2022-03-27</dc:created>
+    <dc:creator xml:lang="en">EN</dc:creator>
+    <dc:creator xml:lang="en">JRK</dc:creator>
+    <dc:creator xml:lang="en">WL</dc:creator>
+    <isOrganizational rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</isOrganizational>
+    <rdfs:label xml:lang="en">biological state optimization method</rdfs:label>
+    <skos:definition xml:lang="en">A method for computing the optimal state of a biological system accordion to a particular objective.</skos:definition>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000686 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000686">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000685"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000106"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000691"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2022-03-27</dc:created>
+    <dc:creator xml:lang="en">EN</dc:creator>
+    <dc:creator xml:lang="en">JRK</dc:creator>
+    <dc:creator xml:lang="en">WL</dc:creator>
+    <isImplementedIn rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://gitlab.com/equilibrator/metabolic-pathway-analysis</isImplementedIn>
+    <rdfs:label xml:lang="en">Enzyme Cost Minimization</rdfs:label>
+    <rdfs:seeAlso rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/doi:10.1371/journal.pcbi.1005167</rdfs:seeAlso>
+    <skos:altLabel xml:lang="en">ECM</skos:altLabel>
+    <skos:definition xml:lang="en">For a given metabolic network model, the Enzyme Cost Minimization method determines plausible metabolite and enzyme concentrations (which determine thermodynamic forces and enzyme catalytic rates). Fluxes, enzyme kinetic constants, admissible metabolite concentration ranges, and enzyme cost weights (e.g. enzyme molecular masses) are given as input data. The method applies the principle that high enzyme (or enzyme plus metabolite) concentrations must be avoided, and maximizes a weighted sum of enzyme and  metabolite concentrations.</skos:definition>
+  </owl:Class>
+  <owl:Axiom>
+    <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000686"/>
+    <owl:annotatedProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#isImplementedIn"/>
+    <owl:annotatedTarget rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://gitlab.com/equilibrator/metabolic-pathway-analysis</owl:annotatedTarget>
+    <rdfs:comment xml:lang="en">Metabolic Pathway Analysis</rdfs:comment>
+  </owl:Axiom>
+  <owl:Axiom>
+    <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000686"/>
+    <owl:annotatedProperty rdf:resource="http://www.w3.org/2000/01/rdf-schema#seeAlso"/>
+    <owl:annotatedTarget rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/doi:10.1371/journal.pcbi.1005167</owl:annotatedTarget>
+    <rdfs:comment xml:lang="en">Elad Noor, Avi Flamholz, Arren Bar-Even, Dan Davidi, Ron Milo &amp; Wolfram Liebermeister. The Protein Cost of Metabolic Fluxes: Prediction from Enzymatic Rate Laws and Cost Minimization. PLoS Comput Biol 12 (11): e1005167 (2016).</rdfs:comment>
+  </owl:Axiom>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000687 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000687">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000685"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000106"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000691"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2022-03-27</dc:created>
+    <dc:creator xml:lang="en">EN</dc:creator>
+    <dc:creator xml:lang="en">JRK</dc:creator>
+    <dc:creator xml:lang="en">WL</dc:creator>
+    <isImplementedIn rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://gitlab.com/equilibrator/metabolic-pathway-analysis</isImplementedIn>
+    <rdfs:label xml:lang="en">Max-min Driving Force method</rdfs:label>
+    <rdfs:seeAlso rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/doi:10.1371/journal.pcbi.1003483</rdfs:seeAlso>
+    <skos:altLabel xml:lang="en">MDF</skos:altLabel>
+    <skos:definition xml:lang="en">For a given metabolic network model, the MDF method determines plausible metabolite concentrations and thermodynamic forces. Flux directions, equilibrium constants (or equivalently, standard Gibbs free energies of reactions) and admissible metabolite concentration ranges are given as input data. The method applies the principle that low thermodynamic forces must be avoided, and maximizes the minimum thermodynamic force across the entire network.</skos:definition>
+  </owl:Class>
+  <owl:Axiom>
+    <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000687"/>
+    <owl:annotatedProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#isImplementedIn"/>
+    <owl:annotatedTarget rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://gitlab.com/equilibrator/metabolic-pathway-analysis</owl:annotatedTarget>
+    <rdfs:comment xml:lang="en">Metabolic Pathway Analysis</rdfs:comment>
+  </owl:Axiom>
+  <owl:Axiom>
+    <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000687"/>
+    <owl:annotatedProperty rdf:resource="http://www.w3.org/2000/01/rdf-schema#seeAlso"/>
+    <owl:annotatedTarget rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">http://identifiers.org/doi:10.1371/journal.pcbi.1003483</owl:annotatedTarget>
+    <rdfs:comment xml:lang="en">Elad Noor, Arren Bar-Even, Avi Flamholz, Ed Reznik, Wolfram Liebermeister &amp; Ron Milo. Pathway thermodynamics highlights kinetic obstacles in central metabolism. PLOS Computational Biology 10(2): e1003483 (2014).</rdfs:comment>
+  </owl:Axiom>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000688 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000688">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000097"/>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2022-03-29</dc:created>
+    <dc:creator xml:lang="en">EN</dc:creator>
+    <dc:creator xml:lang="en">JRK</dc:creator>
+    <dc:creator xml:lang="en">WL</dc:creator>
+    <rdfs:label xml:lang="en">type of system described</rdfs:label>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000689 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000689">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000688"/>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2022-03-29</dc:created>
+    <dc:creator xml:lang="en">EN</dc:creator>
+    <dc:creator xml:lang="en">JRK</dc:creator>
+    <dc:creator xml:lang="en">WL</dc:creator>
+    <rdfs:label xml:lang="en">mathematical system</rdfs:label>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000690 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000690">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000688"/>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2022-03-29</dc:created>
+    <dc:creator xml:lang="en">EN</dc:creator>
+    <dc:creator xml:lang="en">JRK</dc:creator>
+    <dc:creator xml:lang="en">WL</dc:creator>
+    <rdfs:label xml:lang="en">biological system</rdfs:label>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000691 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000691">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000690"/>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2022-03-29</dc:created>
+    <dc:creator xml:lang="en">EN</dc:creator>
+    <dc:creator xml:lang="en">JRK</dc:creator>
+    <dc:creator xml:lang="en">WL</dc:creator>
+    <rdfs:label xml:lang="en">metabolic system</rdfs:label>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000692 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000692">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000690"/>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2022-03-29</dc:created>
+    <dc:creator xml:lang="en">EN</dc:creator>
+    <dc:creator xml:lang="en">JRK</dc:creator>
+    <dc:creator xml:lang="en">WL</dc:creator>
+    <rdfs:label xml:lang="en">cellular system</rdfs:label>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000693 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000693">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000690"/>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2022-03-29</dc:created>
+    <dc:creator xml:lang="en">EN</dc:creator>
+    <dc:creator xml:lang="en">JRK</dc:creator>
+    <dc:creator xml:lang="en">WL</dc:creator>
+    <rdfs:label xml:lang="en">biochemical system</rdfs:label>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000694 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000694">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000000"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000374"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:maxQualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:maxQualifiedCardinality>
+        <owl:onClass rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000209"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:maxQualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:maxQualifiedCardinality>
+        <owl:onClass rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000211"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:maxQualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:maxQualifiedCardinality>
+        <owl:onClass rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000415"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:maxQualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:maxQualifiedCardinality>
+        <owl:onClass rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000475"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:maxQualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:maxQualifiedCardinality>
+        <owl:onClass rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000476"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:maxQualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:maxQualifiedCardinality>
+        <owl:onClass rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000477"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:maxQualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:maxQualifiedCardinality>
+        <owl:onClass rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000478"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:maxQualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:maxQualifiedCardinality>
+        <owl:onClass rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000479"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:maxQualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:maxQualifiedCardinality>
+        <owl:onClass rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000480"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:maxQualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:maxQualifiedCardinality>
+        <owl:onClass rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000481"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:maxQualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:maxQualifiedCardinality>
+        <owl:onClass rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000543"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:maxQualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:maxQualifiedCardinality>
+        <owl:onClass rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000570"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
+        <owl:maxQualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</owl:maxQualifiedCardinality>
+        <owl:onClass rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000571"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2023-05-19</dc:created>
+    <dc:creator xml:lang="en">lps</dc:creator>
+    <isOrganizational rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">false</isOrganizational>
+    <rdfs:label xml:lang="en">ODE solver</rdfs:label>
+    <skos:altLabel xml:lang="en">ordinary differential equation solver</skos:altLabel>
+    <skos:definition xml:lang="en">An ODE solver is the general category of packages such as CVODE-like methods [http://identifiers.org/biomodels.kisao/KISAO_0000433] or Livermore solvers [http://identifiers.org/biomodels.kisao/KISAO_0000094] that solve systems of ordinary differential equations.</skos:definition>
+  </owl:Class>
+  <owl:Axiom>
+    <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000694"/>
+    <owl:annotatedProperty rdf:resource="http://www.w3.org/2004/02/skos/core#altLabel"/>
+    <owl:annotatedTarget xml:lang="en">ordinary differential equation solver</owl:annotatedTarget>
+    <rdfs:comment xml:lang="en">EXACT</rdfs:comment>
+  </owl:Axiom>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000695 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000695">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000201"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000251"/>
+        <owl:someValuesFrom rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <dc:created>2023/05/19</dc:created>
+    <dc:creator>lps</dc:creator>
+    <rdfs:label>parameters for</rdfs:label>
+    <skos:definition xml:lang="en">The children parameters of this term are applied when the parent general term is implented as the more-specific value of this term.  For example:  a 'parameters for' term might be used as a child of an 'ODE Solver' ([http://identifiers.org/biomodels.kisao/KISAO_0000694]), have a value of 'KISAO_0000019' (CVODE)', and have a child term 'use stiff method' of 'true' ([http://identifiers.org/biomodels.kisao/KISAO_0000671])</skos:definition>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000696 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000696">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000370"/>
+    <dc:creator xml:lang="en">LPS</dc:creator>
+    <rdfs:label>steady state root-finding problem</rdfs:label>
+    <skos:altLabel xml:lang="en">steady state problem</skos:altLabel>
+  </owl:Class>
+  <owl:Axiom>
+    <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000696"/>
+    <owl:annotatedProperty rdf:resource="http://www.w3.org/2004/02/skos/core#altLabel"/>
+    <owl:annotatedTarget xml:lang="en">steady state problem</owl:annotatedTarget>
+    <rdfs:comment xml:lang="en">EXACT</rdfs:comment>
+  </owl:Axiom>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000697 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000697">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000000"/>
+    <rdfs:subClassOf>
+      <owl:Class>
+        <owl:complementOf>
+          <owl:Restriction>
+            <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+            <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000102"/>
+          </owl:Restriction>
+        </owl:complementOf>
+      </owl:Class>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000104"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000108"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000237"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000371"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2023-06-06</dc:created>
+    <dc:creator xml:lang="en">lps</dc:creator>
+    <isOrganizational rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">false</isOrganizational>
+    <rdfs:label>SDE solver</rdfs:label>
+    <skos:altLabel xml:lang="en">stochastic differential equation solver</skos:altLabel>
+    <skos:definition xml:lang="en">An SDE solver is the general category of packages that provide stochastic solutions to a system of differential equations with propensities.</skos:definition>
+  </owl:Class>
+  <owl:Axiom>
+    <owl:annotatedSource rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000697"/>
+    <owl:annotatedProperty rdf:resource="http://www.w3.org/2004/02/skos/core#altLabel"/>
+    <owl:annotatedTarget xml:lang="en">stochastic differential equation solver</owl:annotatedTarget>
+    <rdfs:comment xml:lang="en">EXACT</rdfs:comment>
+  </owl:Axiom>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000800 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000800">
     <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000831"/>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">06-03-2021</dc:created>
     <dc:creator xml:lang="en">LPS</dc:creator>
     <isOrganizational rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</isOrganizational>
     <rdfs:label xml:lang="en">systems property</rdfs:label>
@@ -12906,14 +13260,121 @@
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000830">
     <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000824"/>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2021-10-09</dc:created>
     <dc:creator xml:lang="en">MK</dc:creator>
     <rdfs:label xml:lang="en">maximum</rdfs:label>
     <skos:definition xml:lang="en">The maximum of a set of values. If the values contain NaN the maximum is NaN.</skos:definition>
   </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000831 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000831">
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">06-03-2021</dc:created>
+    <dc:creator xml:lang="en">LPS</dc:creator>
+    <isOrganizational rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</isOrganizational>
+    <rdfs:label xml:lang="en">model and simulation property</rdfs:label>
+    <skos:definition xml:lang="en">A variable of a model or simulation.</skos:definition>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000832 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000832">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000831"/>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">06-03-2021</dc:created>
+    <dc:creator xml:lang="en">LPS</dc:creator>
+    <rdfs:label xml:lang="en">time</rdfs:label>
+    <skos:definition xml:lang="en">The implied time variable of the model state.</skos:definition>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000834 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000834">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000831"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000647"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000655"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">06-03-2021</dc:created>
+    <dc:creator xml:lang="en">LPS</dc:creator>
+    <rdfs:label xml:lang="en">rate of change</rdfs:label>
+    <skos:altLabel xml:lang="en">rate</skos:altLabel>
+    <skos:definition xml:lang="en">The rate of change of one variable with respect to a second variable.</skos:definition>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000835 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000835">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000800"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000634"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">06-03-2021</dc:created>
+    <dc:creator xml:lang="en">LPS</dc:creator>
+    <rdfs:label xml:lang="en">concentration control coefficient matrix (scaled)</rdfs:label>
+    <skos:definition xml:lang="en">The scaled concentration control coefficient matrix. The dimensions are species by reactions.</skos:definition>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000836 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000836">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000831"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000822"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <dc:created>06-03-2021</dc:created>
+    <dc:creator>LPS</dc:creator>
+    <rdfs:label xml:lang="en">amount</rdfs:label>
+    <skos:definition>The extensive quantity amount.</skos:definition>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000837 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000837">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000831"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000822"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <dc:created>06-03-2021</dc:created>
+    <dc:creator>LPS</dc:creator>
+    <rdfs:label xml:lang="en">particle number</rdfs:label>
+    <skos:definition>The extensive quantity particle number, or, the molar amount of the entity multiplied by Avogadro's number.</skos:definition>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000838 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000838">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000831"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000821"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <dc:created>06-03-2021</dc:created>
+    <dc:creator>LPS</dc:creator>
+    <rdfs:label xml:lang="en">concentration</rdfs:label>
+    <skos:definition>The intensive quantity concentration, or, the amount of the entity with respect to the entity in which it resides.</skos:definition>
+  </owl:Class>
+  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000839 -->
+  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000839">
+    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000831"/>
+    <rdfs:subClassOf>
+      <owl:Restriction>
+        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
+        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000821"/>
+      </owl:Restriction>
+    </rdfs:subClassOf>
+    <dc:created>06-03-2021</dc:created>
+    <dc:creator>LPS</dc:creator>
+    <rdfs:label xml:lang="en">temperature</rdfs:label>
+    <skos:definition>The intensive quantity temperature.</skos:definition>
+  </owl:Class>
   <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000840 -->
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000840">
     <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000824"/>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2021-10-09</dc:created>
     <dc:creator xml:lang="en">MK</dc:creator>
     <rdfs:label xml:lang="en">minimum</rdfs:label>
     <skos:definition xml:lang="en">The minimum of a set of values. If the values contain NaN the minimum is NaN.</skos:definition>
@@ -13066,121 +13527,14 @@
   <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000859">
     <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000824"/>
     <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">2021-10-09</dc:created>
     <dc:creator xml:lang="en">MK</dc:creator>
     <rdfs:label xml:lang="en">variance</rdfs:label>
     <skos:definition xml:lang="en">The variance of a set of values. If the values contain NaN the variance is NaN.</skos:definition>
   </owl:Class>
-  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000831 -->
-  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000831">
-    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">06-03-2021</dc:created>
-    <dc:creator xml:lang="en">LPS</dc:creator>
-    <isOrganizational rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</isOrganizational>
-    <rdfs:label xml:lang="en">model and simulation property</rdfs:label>
-    <skos:definition xml:lang="en">A variable of a model or simulation.</skos:definition>
-  </owl:Class>
-  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000832 -->
-  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000832">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000831"/>
-    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">06-03-2021</dc:created>
-    <dc:creator xml:lang="en">LPS</dc:creator>
-    <rdfs:label xml:lang="en">time</rdfs:label>
-    <skos:definition xml:lang="en">The implied time variable of the model state.</skos:definition>
-  </owl:Class>
-  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000834 -->
-  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000834">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000831"/>
-    <rdfs:subClassOf>
-      <owl:Restriction>
-        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000647"/>
-      </owl:Restriction>
-    </rdfs:subClassOf>
-    <rdfs:subClassOf>
-      <owl:Restriction>
-        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000655"/>
-      </owl:Restriction>
-    </rdfs:subClassOf>
-    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">06-03-2021</dc:created>
-    <dc:creator xml:lang="en">LPS</dc:creator>
-    <rdfs:label xml:lang="en">rate of change</rdfs:label>
-    <skos:altLabel xml:lang="en">rate</skos:altLabel>
-    <skos:definition xml:lang="en">The rate of change of one variable with respect to a second variable.</skos:definition>
-  </owl:Class>
-  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000835 -->
-  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000835">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000800"/>
-    <rdfs:subClassOf>
-      <owl:Restriction>
-        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000634"/>
-      </owl:Restriction>
-    </rdfs:subClassOf>
-    <dc:created rdf:datatype="http://www.w3.org/2001/XMLSchema#date">06-03-2021</dc:created>
-    <dc:creator xml:lang="en">LPS</dc:creator>
-    <rdfs:label xml:lang="en">concentration control coefficient matrix (scaled)</rdfs:label>
-    <skos:definition xml:lang="en">The scaled concentration control coefficient matrix. The dimensions are species by reactions.</skos:definition>
-  </owl:Class>
-  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000836 -->
-  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000836">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000831"/>
-    <rdfs:subClassOf>
-      <owl:Restriction>
-        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000822"/>
-      </owl:Restriction>
-    </rdfs:subClassOf>
-    <dc:created>06-03-2021</dc:created>
-    <dc:creator>LPS</dc:creator>
-    <rdfs:label xml:lang="en">amount</rdfs:label>
-    <skos:definition>The extensive quantity amount.</skos:definition>
-  </owl:Class>
-  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000837 -->
-  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000837">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000831"/>
-    <rdfs:subClassOf>
-      <owl:Restriction>
-        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000822"/>
-      </owl:Restriction>
-    </rdfs:subClassOf>
-    <dc:created>06-03-2021</dc:created>
-    <dc:creator>LPS</dc:creator>
-    <rdfs:label xml:lang="en">particle number</rdfs:label>
-    <skos:definition>The extensive quantity particle number, or, the molar amount of the entity multiplied by Avogadro's number.</skos:definition>
-  </owl:Class>
-  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000838 -->
-  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000838">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000831"/>
-    <rdfs:subClassOf>
-      <owl:Restriction>
-        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000821"/>
-      </owl:Restriction>
-    </rdfs:subClassOf>
-    <dc:created>06-03-2021</dc:created>
-    <dc:creator>LPS</dc:creator>
-    <rdfs:label xml:lang="en">concentration</rdfs:label>
-    <skos:definition>The intensive quantity concentration, or, the amount of the entity with respect to the entity in which it resides.</skos:definition>
-  </owl:Class>
-  <!-- http://www.biomodels.net/kisao/KISAO#KISAO_0000839 -->
-  <owl:Class rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000839">
-    <rdfs:subClassOf rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000831"/>
-    <rdfs:subClassOf>
-      <owl:Restriction>
-        <owl:onProperty rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000245"/>
-        <owl:someValuesFrom rdf:resource="http://www.biomodels.net/kisao/KISAO#KISAO_0000821"/>
-      </owl:Restriction>
-    </rdfs:subClassOf>
-    <dc:created>06-03-2021</dc:created>
-    <dc:creator>LPS</dc:creator>
-    <rdfs:label xml:lang="en">temperature</rdfs:label>
-    <skos:definition>The intensive quantity temperature.</skos:definition>
-  </owl:Class>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Annotations
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
@@ -13957,8 +14311,8 @@
       <rdf:Description rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000259"/>
       <rdf:Description rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000268"/>
       <rdf:Description rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000359"/>
       <rdf:Description rdf:about="http://www.biomodels.net/kisao/KISAO#KISAO_0000360"/>
     </owl:members>
   </rdf:Description>
 </rdf:RDF>
-<!-- Generated by the OWL API (version 4.2.8.20170104-2310) https://github.com/owlcs/owlapi -->
+<!-- Generated by the OWL API (version 4.5.9.2019-02-01T07:24:44Z) https://github.com/owlcs/owlapi -->
```

### Comparing `kisao-2.30/kisao/utils.py` & `kisao-2.32/kisao/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 from .core import Kisao
 from .data_model import (AlgorithmSubstitutionPolicy, ALGORITHM_SUBSTITUTION_POLICY_LEVELS, IdDialect,
                          ID_HAS_CHARACTERISTIC_RELATIONSHIP,
                          ID_ODE_PROBLEM_CHARACTERISTIC,
                          ID_SDE_PROBLEM_CHARACTERISTIC,
+                         ID_STEADYSTATE_PROBLEM_CHARACTERISTIC,
                          ID_PDE_PROBLEM_CHARACTERISTIC,
                          ID_EXACT_SOLUTION_CHARACTERISTIC,
                          ID_APPROXIMATE_SOLUTION_CHARACTERISTIC,
                          ID_ALGORITHM,
                          ID_GILLESPIE_LIKE_ALGORITHM,
                          ID_TAU_LEAPING_ALGORITHM,
                          ID_RULE_BASED_ALGORITHM,
@@ -207,14 +208,26 @@
     Returns:
         :obj:`set` of :obj:`pronto.Term`: terms
     """
     return get_terms_with_characteristics([ID_ALGORITHM], [ID_SDE_PROBLEM_CHARACTERISTIC])
 
 
 @ functools.lru_cache(maxsize=None)
+def get_steadystate_algorithms():
+    """ Get the terms for rule-based simulation algorithms (KISAO_0000363).::
+
+        'rule-based simulation method'
+
+    Returns:
+        :obj:`set` of :obj:`pronto.Term`: terms
+    """
+    return get_terms_with_characteristics([ID_ALGORITHM], [ID_STEADYSTATE_PROBLEM_CHARACTERISTIC])
+
+
+@ functools.lru_cache(maxsize=None)
 def get_pde_algorithms():
     """ Get the terms for rule-based simulation algorithms (KISAO_0000363).::
 
         'rule-based simulation method'
 
     Returns:
         :obj:`set` of :obj:`pronto.Term`: terms
@@ -278,14 +291,24 @@
 
     Returns:
         :obj:`set` of :obj:`pronto.Term`: terms
     """
     return get_terms_with_characteristics([ID_HYBRID_ALGORITHM])
 
 
+@ functools.lru_cache(maxsize=None)
+def get_parents_and_children_of(term):
+    """ Get the parents and children of the given term.::
+
+    Returns:
+        :obj:`set` of :obj:`pronto.Term`: terms
+    """
+    return get_terms_with_characteristics([ID_HYBRID_ALGORITHM])
+
+
 def get_substitutable_algorithms_for_policy(algorithm, substitution_policy=AlgorithmSubstitutionPolicy.SIMILAR_VARIABLES):
     """ Get a set of algorithms that an algorithm can be substituted for a given substitution policy.
 
     Args:
         algorithm (:obj:`pronto.Term`): target algorithm (e.g., requested to be executed in a SED-ML document)
         substitution_policy (:obj:`AlgorithmSubstitutionPolicy`, optional): algorithm substitution policy; defines the degree to which
             alternative algorithms can be substituted
@@ -303,28 +326,30 @@
 
     elif substitution_policy == AlgorithmSubstitutionPolicy.SAME_MATH:
         alg_set_funcs = [
             (False, get_ode_algorithms),
             (True, functools.partial(get_gillespie_like_algorithms, exact=True, approximate=False)),
             (False, get_tau_leaping_algorithms),
             (False, get_sde_algorithms),
+            (False, get_steadystate_algorithms),
             (False, get_pde_algorithms),
             (False, get_logical_simulation_algorithms),
             (True, get_logical_stable_state_search_algorithms),
             (True, get_logical_trap_space_search_algorithms),
             (False, get_flux_balance_algorithms),
         ]
         alt_algs = _find_substitutable_algorithms(algorithm, alg_set_funcs)
 
     elif substitution_policy == AlgorithmSubstitutionPolicy.SIMILAR_APPROXIMATIONS:
         alg_set_funcs = [
             (True, get_ode_algorithms),
             (True, functools.partial(get_gillespie_like_algorithms, exact=True, approximate=False)),
             (True, get_tau_leaping_algorithms),
             (True, get_sde_algorithms),
+            (True, get_steadystate_algorithms),
             (True, get_pde_algorithms),
             (False, get_logical_simulation_algorithms),
             (True, get_logical_stable_state_search_algorithms),
             (True, get_logical_trap_space_search_algorithms),
             (False, get_flux_balance_algorithms),
         ]
         alt_algs = _find_substitutable_algorithms(algorithm, alg_set_funcs)
@@ -334,28 +359,30 @@
         <= ALGORITHM_SUBSTITUTION_POLICY_LEVELS[AlgorithmSubstitutionPolicy.SIMILAR_VARIABLES]
     ):
         alg_set_funcs = [
             (True, get_ode_algorithms),
             (True, lambda: get_gillespie_like_algorithms(
                 exact=True, approximate=False) | get_tau_leaping_algorithms()),
             (True, get_sde_algorithms),
+            (True, get_steadystate_algorithms),
             (True, get_pde_algorithms),
             (True, get_logical_simulation_algorithms),
             (True, get_logical_stable_state_search_algorithms),
             (True, get_logical_trap_space_search_algorithms),
             # (False, get_flux_balance_algorithms),
         ]
         alt_algs = _find_substitutable_algorithms(algorithm, alg_set_funcs)
 
     elif substitution_policy == AlgorithmSubstitutionPolicy.SAME_FRAMEWORK:
         alg_set_funcs = [
             (True, get_ode_algorithms),
             (True, lambda: get_gillespie_like_algorithms(
                 exact=True, approximate=False) | get_tau_leaping_algorithms()),
             (True, get_sde_algorithms),
+            (True, get_steadystate_algorithms),
             (True, get_pde_algorithms),
             (True, get_flux_balance_algorithms),
             (True, get_logical_simulation_algorithms),
             (True, get_logical_stable_state_search_algorithms),
             (True, get_logical_trap_space_search_algorithms),
         ]
         alt_algs = _find_substitutable_algorithms(algorithm, alg_set_funcs)
@@ -466,15 +493,15 @@
             ).format(
                 algorithm.name, algorithm.id.partition('#')[2], substitution_policy.name,
                 '\n  '.join(sorted('{}: {}'.format(alt_algorithm.id.partition('#')[2], alt_algorithm.name)
                                    for alt_algorithm in alt_algorithms))
             ))
 
     if alt_algorithm != algorithm:
-        msg = "'{}' ({}) will be substituted for '{}'' ({}) at substitution policy '{}'.".format(
+        msg = "'{}' ({}) will be substituted for '{}' ({}) at substitution policy '{}'.".format(
             alt_algorithm.name, alt_algorithm.id.partition('#')[2],
             algorithm.name, algorithm.id.partition('#')[2],
             substitution_policy.name)
         warnings.warn(termcolor.colored(msg, 'yellow'), AlgorithmSubstitutedWarning)
 
     return alt_algorithm
```

### Comparing `kisao-2.30/kisao.egg-info/PKG-INFO` & `kisao-2.32/kisao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kisao
-Version: 2.30
+Version: 2.32
 Summary: Utilities for working with the Kinetic Simulation Algorithm Ontology (KiSAO)
 Home-page: https://github.com/SED-ML/kisao
 Author: SED-ML Editors
 Author-email: sed-ml-editors@googlegroups.com
 License: Apache 2.0
 Download-URL: https://github.com/SED-ML/kisao
 Keywords: systems biology,modeling,simulation,algorithm,ontology,KiSAO,SED-ML,SBML
```

### Comparing `kisao-2.30/setup.py` & `kisao-2.32/setup.py`

 * *Files identical despite different names*

