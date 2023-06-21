# Comparing `tmp/sysml2py-0.1.2.tar.gz` & `tmp/sysml2py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysml2py-0.1.2.tar", last modified: Thu Jun  1 12:44:34 2023, max compression
+gzip compressed data, was "sysml2py-0.3.0.tar", last modified: Wed Jun 21 03:26:33 2023, max compression
```

## Comparing `sysml2py-0.1.2.tar` & `sysml2py-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:44:34.429178 sysml2py-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 12:44:14.000000 sysml2py-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-01 12:44:34.429178 sysml2py-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-01 12:44:14.000000 sysml2py-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-01 12:44:14.000000 sysml2py-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:44:34.429178 sysml2py-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:44:34.425178 sysml2py-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:44:34.429178 sysml2py-0.1.2/src/sysml2py/
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:44:34.429178 sysml2py-0.1.2/src/sysml2py/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)    22327 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/grammar/KerML.tx
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/grammar/KerMLExpressions.tx
--rw-r--r--   0 runner    (1001) docker     (123)    46559 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/grammar/SysML.tx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:44:34.429178 sysml2py-0.1.2/src/sysml2py/textx/
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/textx/xtext_to_textx.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-01 12:44:14.000000 sysml2py-0.1.2/src/sysml2py/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:44:34.429178 sysml2py-0.1.2/sysml2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-01 12:44:34.000000 sysml2py-0.1.2/sysml2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-01 12:44:34.000000 sysml2py-0.1.2/sysml2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:44:34.000000 sysml2py-0.1.2/sysml2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 12:44:34.000000 sysml2py-0.1.2/sysml2py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:26:33.945388 sysml2py-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 03:26:26.000000 sysml2py-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-21 03:26:33.945388 sysml2py-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-21 03:26:26.000000 sysml2py-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-21 03:26:26.000000 sysml2py-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 03:26:33.945388 sysml2py-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:26:33.937388 sysml2py-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:26:33.941388 sysml2py-0.3.0/src/sysml2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:26:33.941388 sysml2py-0.3.0/src/sysml2py/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)    22296 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/grammar/KerML.tx
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/grammar/KerMLExpressions.tx
+-rw-r--r--   0 runner    (1001) docker     (123)    48820 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/grammar/SysML.tx
+-rw-r--r--   0 runner    (1001) docker     (123)    80969 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/grammar/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:26:33.941388 sysml2py-0.3.0/src/sysml2py/textx/
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/textx/xtext_to_textx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-21 03:26:26.000000 sysml2py-0.3.0/src/sysml2py/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:26:33.945388 sysml2py-0.3.0/sysml2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-21 03:26:33.000000 sysml2py-0.3.0/sysml2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 03:26:33.000000 sysml2py-0.3.0/sysml2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:26:33.000000 sysml2py-0.3.0/sysml2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 03:26:33.000000 sysml2py-0.3.0/sysml2py.egg-info/top_level.txt
```

### Comparing `sysml2py-0.1.2/LICENSE` & `sysml2py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sysml2py-0.1.2/PKG-INFO` & `sysml2py-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysml2py
-Version: 0.1.2
+Version: 0.3.0
 Summary: SysML v2.0 Parser
 Author-email: Christopher Cox <chris.cox@westfall.io>
 Project-URL: Homepage, https://github.com/Westfall-io/sysml2py
 Project-URL: Bug Tracker, https://github.com/Westfall-io/sysml2py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sysml2py-0.1.2/README.md` & `sysml2py-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sysml2py-0.1.2/pyproject.toml` & `sysml2py-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysml2py"
-version = "0.1.2"
+version = "0.3.0"
 authors = [
   { name="Christopher Cox", email="chris.cox@westfall.io" },
 ]
 description = "SysML v2.0 Parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.setuptools]
-# ...
-# By default, include-package-data is true in pyproject.toml, so you do
-# NOT have to specify this line.
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src/sysml2py", "src"]
 
 [tool.setuptools.package-data]
 grammar = ["*.tx"]
 
+[tool.semantic_release]
+branch = "main"
+version_variable = "pyproject.toml:version"
+version_source = "tag"
+commit_version_number = true # required for version_source = "tag"
+tag_commit = true
+commit_parser = "semantic_release.history.emoji_parser"
+build_command = false
+upload_to_repository = false
+upload_to_release = false
+
 [project.urls]
 "Homepage" = "https://github.com/Westfall-io/sysml2py"
 "Bug Tracker" = "https://github.com/Westfall-io/sysml2py/issues"
```

### Comparing `sysml2py-0.1.2/src/sysml2py/__init__.py` & `sysml2py-0.3.0/src/sysml2py/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 """
 Created on Mon May 29 23:26:16 2023
 
 @author: christophercox
 """
 import io
 
-from textx import metamodel_from_str
+from textx import metamodel_from_file
 
-import pkg_resources
+import importlib.resources as pkg_resources
 
+import sysml2py
 from sysml2py.formatting import reformat
 
 __all__ = ["load", "loads"]
 __author__ = "Christopher Cox"
 
 
 def load(fp):
@@ -45,15 +46,15 @@
             f"the SysML object must be _io.TextIOWrapper, "
             f"not {fp.__class__.__name__}"
         )
 
     return loads(fp.read())
 
 
-def loads(s):
+def loads(s, formatting="json"):
     """SysML load from string
 
     Deserialize ``s`` (a ``str`` instance containing a SysML v2.0 document)
     to a Python dictionary object.
 
     Parameters
     ----------
@@ -68,33 +69,25 @@
 
     Raises
     ------
     TypeError
         Input was not str
 
     """
+
     if not isinstance(s, str):
         raise TypeError(f"the SysML object must be str, " f"not {s.__class__.__name__}")
 
     try:
-        stream = pkg_resources.resource_stream(__name__, "grammar/KerMLExpressions.tx")
-    except:
-        stream = open("src/sysml2py/grammar/KerMLExpressions.tx", "rb")
-    grammar = stream.read().decode("utf-8")
-    meta = metamodel_from_str(grammar)
-
-    try:
-        stream = pkg_resources.resource_stream(__name__, "grammar/KerML.tx")
+        grammar = str((pkg_resources.files(sysml2py) / "grammar/SysML.tx"))
     except:
-        stream = open("src/sysml2py/grammar/KerML.tx", "rb")
-    grammar = stream.read().decode("utf-8")
-    meta = metamodel_from_str(grammar, metamodel=meta)
-
-    try:
-        stream = pkg_resources.resource_stream(__name__, "grammar/SysML.tx")
-    except:
-        stream = open("src/sysml2py/grammar/SysML.tx", "rb")
-    grammar = stream.read().decode("utf-8")
-    meta = metamodel_from_str(grammar, metamodel=meta)
-    model = meta.model_from_str(s)
-
-    return reformat(model)
+        try:
+            grammar = "./src/sysml2py/grammar/SysML.tx"
+        except:
+            grammar = "./grammar/SysML.tx"
+    meta = metamodel_from_file(grammar)
+    model = meta.model_from_str(s, debug=True)
+
+    if formatting == "json":
+        return reformat(model)
+    else:
+        return model
```

### Comparing `sysml2py-0.1.2/src/sysml2py/grammar/KerML.tx` & `sysml2py-0.3.0/src/sysml2py/grammar/KerML.tx`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-//import grammar.KerMLExpressions
+import KerMLExpressions
 /*****************************************************************************
  * SysML 2 Pilot Implementation
  * Copyright (c) 2018-2023 Model Driven Solutions, Inc.
  * Copyright (c) 2018 IncQuery Labs Ltd.
  * Copyright (c) 2019 Maplesoft (Waterloo Maple, Inc.)
  * Copyright (c) 2019 Mgnite Inc.
  *
@@ -60,48 +60,49 @@
 ;
 
 /* DEPENDENCIES */
 
 Dependency :
 	( ownedRelationship += PrefixMetadataAnnotation )*
 	'dependency' ( Identification? 'from' )?
-    client += [QualifiedName] ( ',' client += [QualifiedName] )* 'to'
-    supplier += [QualifiedName] ( ',' supplier += [QualifiedName] )*
+    client += QualifiedName ( ',' client += QualifiedName )* 'to'
+    supplier += QualifiedName ( ',' supplier += QualifiedName )*
     RelationshipBody
 ;
 
 /* ANNOTATIONS */
 
 Annotation :
-	annotatedElement = [QualifiedName]
+	annotatedElement = QualifiedName
 ;
 
 OwnedAnnotation :
 	ownedRelatedElement += AnnotatingElement
 ;
 
 AnnotatingElement :
-	  Comment
+	  CommentKerML
 	| Documentation
 	| TextualRepresentation
 	| MetadataFeature
 ;
 
 /* Comments */
 
-Comment :
+CommentKerML :
+// Comment is reserved in TextX
 	( 'comment' Identification?
 	  ('about' ownedRelationship += Annotation
 	     ( ',' ownedRelationship += Annotation )* )?
 	)?
 	body = REGULAR_COMMENT
 ;
 
 Documentation :
-	'doc' Identification? body = REGULAR_COMMENT
+	'doc' Identification? body=REGULAR_COMMENT
 ;
 
 /* Textual Representation */
 
 TextualRepresentation :
     ( 'rep' Identification? )?
     'language' language = STRING_VALUE
@@ -152,15 +153,15 @@
 NamespaceFeatureMember :
 	MemberPrefix ownedRelatedElement += FeatureElement
 ;
 
 AliasMember :
 	MemberPrefix
 	'alias' ( '<' memberShortName = Name '>' )? ( memberName = Name )?
-	'for' memberElement = [QualifiedName]
+	'for' memberElement = QualifiedName
 	RelationshipBody
 ;
 
  ImportPrefix :
 	( visibility = VisibilityIndicator )?
 	'import' ( isImportAll ?= 'all' )?
 ;
@@ -171,27 +172,27 @@
 ;
 
 MembershipImport :
 	ImportPrefix ImportedMembership
 ;
 
  ImportedMembership :
-	importedMembership = [QualifiedName]
+	importedMembership = QualifiedName
 	( '::' isRecursive ?= '**' )?
 ;
 
 NamespaceImport :
 	ImportPrefix
 	( ImportedNamespace
 	| ownedRelatedElement += FilterPackage
 	)
 ;
 
  ImportedNamespace :
-	importedNamespace = [QualifiedName] '::' '*'
+	importedNamespace = QualifiedName '::' '*'
 	( '::' isRecursive ?= '**' )?
 ;
 
 FilterPackage :
 	ownedRelationship += FilterPackageImport
 	( ownedRelationship += FilterPackageMember )+
 ;
@@ -380,77 +381,77 @@
 ;
 
 /* Specialization */
 
 Specialization :
     ( 'specialization' Identification? )?
     'subtype'
-	( specific = [QualifiedName]
+	( specific = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain )
     ( ':>' | 'specializes')
-	( general = [QualifiedName]
+	( general = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain )
 	RelationshipBody
 ;
 
 OwnedSpecialization :
-	  general = [QualifiedName]
+	  general = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain
 ;
 
 /* Conjugation */
 
 Conjugation :
 	( 'conjugation' Identification? )?
     'conjugate'
-    ( conjugatedType = [QualifiedName]
+    ( conjugatedType = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain )
     ( '~' | 'conjugates')
-    ( originalType = [QualifiedName]
+    ( originalType = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain )
 	RelationshipBody
 ;
 
 OwnedConjugation :
-	  originalType = [QualifiedName]
+	  originalType = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain
 ;
 
 /* Disjoining */
 
 Disjoining :
 	( 'disjoining' Identification? )?
 	'disjoint'
-	( typeDisjoined = [QualifiedName]
+	( typeDisjoined = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain )
 	'from'
-	( disjoiningType = [QualifiedName]
+	( disjoiningType = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain )
 	RelationshipBody
 ;
 
 OwnedDisjoining :
-	  disjoiningType = [QualifiedName]
+	  disjoiningType = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain
 ;
 
 /* Unioning, Intersecting and Differencing */
 
 Unioning :
-	  unioningType = [QualifiedName]
+	  unioningType = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain
 ;
 
 Intersecting :
-	  intersectingType = [QualifiedName]
+	  intersectingType = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain
 ;
 
 Differencing :
-	  differencingType = [QualifiedName]
+	  differencingType = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain
 ;
 
 /* CLASSIFIERS */
 
 /* Classifiers */
 
@@ -475,27 +476,27 @@
 	( '~' | 'conjugates' ) ownedRelationship += ClassifierConjugation
 ;
 
 /* Subclassification */
 
 Subclassification :
 	( 'specialization' Identification? )?
-    'subclassifier' subclassifier = [QualifiedName]
-    ( ':>' | 'specializes') superclassifier = [QualifiedName]
+    'subclassifier' subclassifier = QualifiedName
+    ( ':>' | 'specializes') superclassifier = QualifiedName
     RelationshipBody
 ;
 
 Ownedsubclassification :
-	superclassifier = [QualifiedName]
+	superclassifier = QualifiedName
 ;
 
 /* Classifier Conjugation */
 
 ClassifierConjugation :
-	originalType = [QualifiedName]
+	originalType = QualifiedName
 ;
 
 /* FEATURES */
 
 /* Features */
 
  FeatureDirection :
@@ -559,19 +560,19 @@
 ( isOrdered ?= 'ordered' isNonunique ?= 'nonunique'
    | isNonunique2 ?= 'nonunique' isOrdered2 ?= 'ordered'
 )
 
 ;
 
  FeatureSpecialization :
-	Typings | Subsettings | References | Redefinitions
+	typings=Typings | Subsettings | References | Redefinitions
 ;
 
  Typings :
-	TypedBy ( ',' ownedRelationship += OwnedFeatureTyping )*
+	typedby=TypedBy ( ',' ownedRelationship += OwnedFeatureTyping )*
 ;
 
  TypedBy :
 	( ':' | 'typed' 'by' ) ownedRelationship += OwnedFeatureTyping
 ;
 
  Subsettings :
@@ -599,108 +600,107 @@
 ;
 
 /* Feature Inverting */
 
 FeatureInverting :
 	( 'inverting' Identification? )?
 	'inverse'
-	( featureInverted = [QualifiedName]
+	( featureInverted = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain )
 	'of'
-	( invertingFeature = [QualifiedName]
+	( invertingFeature = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain )
 	RelationshipBody
 ;
 
 OwnedFeatureInverting :
-	  invertingFeature = [QualifiedName]
+	  invertingFeature = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain
 ;
 
 /* Type Featuring */
 
 TypeFeaturing :
 	'featuring' ( Identification? 'of')?
-	featureOfType = [QualifiedName]
-	'by' featuringType = [QualifiedName]
+	featureOfType = QualifiedName
+	'by' featuringType = QualifiedName
 	RelationshipBody
 ;
 
 OwnedTypeFeaturing :
-	featuringType = [QualifiedName]
+	featuringType = QualifiedName
 ;
 
 /* Feature Typing */
 
 FeatureTyping :
 	( 'specialization' Identification? )?
-    'typing' typedFeature = [QualifiedName]
-    (':' | 'typed' 'by') FeatureType
+    'typing' typedFeature = QualifiedName
+    (':' | 'typed' 'by') type=FeatureType
     RelationshipBody
 ;
 
 
 OwnedFeatureTyping :
-	FeatureType
+	type=FeatureType
 ;
 
  FeatureType :
-	  type = [QualifiedName]
-	| ownedRelatedElement += OwnedFeatureChain
+	  type = QualifiedName | ownedRelatedElement += OwnedFeatureChain
 ;
 
 /* Subsetting */
 
 Subsetting :
 	( 'specialization' Identification? )?
     'subset'
-    ( subsettingFeature = [QualifiedName]
+    ( subsettingFeature = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain )
     ( ':>' | 'subsets' )
-    ( subsettedFeature = [QualifiedName]
+    ( subsettedFeature = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain )
 	RelationshipBody
 ;
 
 OwnedSubsetting :
-	  subsettedFeature = [QualifiedName]
+	  subsettedFeature = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain
 ;
 
 OwnedReferenceSubsetting :
-	  referencedFeature = [QualifiedName]
+	  referencedFeature = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain
 ;
 
 /* Redefinition */
 
 Redefinition :
 	( 'specialization' Identification? )?
     'redefinition'
-    ( redefiningFeature = [QualifiedName]
+    ( redefiningFeature = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain )
     ( ':>>' | 'redefines' )
-    ( redefinedFeature = [QualifiedName]
+    ( redefinedFeature = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain )
 	RelationshipBody
 ;
 
 OwnedRedefinition :
-	  redefinedFeature = [QualifiedName]
+	  redefinedFeature = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain
 ;
 
 /* Feature Conjugation */
 
  FeatureConjugationPart :
 	( '~' | 'conjugates' ) ownedRelationship += FeatureConjugation
 ;
 
 FeatureConjugation :
-	originalType = [QualifiedName]
+	originalType = QualifiedName
 ;
 
 /* FEATURE VALUES */
 
  ValuePart :
 	  ownedRelationship += FeatureValue
 	| ownedRelationship += FeatureValueExpression
@@ -1029,15 +1029,15 @@
 
 ItemFlowEnd :
 	( ownedRelationship += ItemFlowEndSubsetting )?
 	ownedRelationship += ItemFlowFeatureMember
 ;
 
 ItemFlowEndSubsetting :
-	  referencedFeature = [QualifiedName] '.'
+	  referencedFeature = QualifiedName '.'
 	| ownedRelatedElement += FeatureChainPrefix
 ;
 
 FeatureChainPrefix :
 	( ownedRelationship += OwnedFeatureChaining '.' )+
 	ownedRelationship += OwnedFeatureChaining '.'
 ;
@@ -1047,15 +1047,15 @@
 ;
 
 ItemFlowFeature :
 	ownedRelationship += ItemFlowRedefinition
 ;
 
 ItemFlowRedefinition :
-	redefinedFeature = [QualifiedName]
+	redefinedFeature = QualifiedName
 ;
 
 /* METADATA */
 
 Metaclass :
 	TypePrefix 'metaclass'
 	ClassifierDeclaration TypeBody
@@ -1082,15 +1082,15 @@
 ;
 
  MetadataFeatureDeclaration :
 	( Identification ( ':' | 'typed' 'by' ) )? ownedRelationship += MetadataTyping
 ;
 
 MetadataTyping :
-	type = [QualifiedName]
+	type = QualifiedName
 ;
 
  MetadataBody :
 	  ';'
 	| '{' ( ownedRelationship += NonFeatureMember
 		  | ownedRelationship += MetadataBodyFeatureMember
 		  | ownedRelationship += AliasMember
```

### Comparing `sysml2py-0.1.2/src/sysml2py/grammar/KerMLExpressions.tx` & `sysml2py-0.3.0/src/sysml2py/grammar/KerMLExpressions.tx`

 * *Files 6% similar despite different names*

```diff
@@ -33,37 +33,37 @@
 /* Operator Expressions */
 
 OwnedExpressionMember :
 	ownedRelatedElement += OwnedExpression
 ;
 
 OwnedExpression :
-	 ConditionalExpression
+	 expression=ConditionalExpression
 ;
 
 // Conditional Test Expressions
 
 OwnedExpressionReference :
 	ownedRelationship += OwnedExpressionMember
 ;
 
 ConditionalExpression :
-	  NullCoalescingExpression
+	  operand += NullCoalescingExpression
 	|  operator = ConditionalOperator operand += NullCoalescingExpression
 		  '?' operand += OwnedExpressionReference 'else' operand += OwnedExpressionReference
 ;
 
 ConditionalOperator :
 	'if'
 ;
 
 // Null Coalescing Expressions
 
 NullCoalescingExpression :
-	ImpliesExpression (
+	implies = ImpliesExpression (
 		operator = NullCoalescingOperator operand += ImpliesExpressionReference )*
 ;
 
 NullCoalescingOperator :
 	'??'
 ;
 
@@ -74,15 +74,15 @@
 ;
 
 ImpliesExpressionMember :
 	ownedRelatedElement += ImpliesExpression
 ;
 
 ImpliesExpression :
-	OrExpression (
+	or = OrExpression (
 		operator = ImpliesOperator operand += OrExpressionReference )*
 ;
 
 ImpliesOperator :
 	'implies'
 ;
 
@@ -91,15 +91,15 @@
 ;
 
 OrExpressionMember :
 	ownedRelatedElement += OrExpression
 ;
 
 OrExpression :
-	XorExpression (
+	xor=XorExpression (
 		( operator = OrOperator operand += XorExpression
 		| operator = ConditionalOrOperator operand += XorExpressionReference ) )*
 ;
 
 OrOperator :
 	'|'
 ;
@@ -113,24 +113,24 @@
 ;
 
 XorExpressionMember :
 	ownedRelatedElement += XorExpression
 ;
 
 XorExpression :
-	AndExpression (
+	and=AndExpression (
 		operator = XorOperator operand += AndExpression )*
 ;
 
 XorOperator :
 	'xor'
 ;
 
 AndExpression :
-	EqualityExpression (
+	equality=EqualityExpression (
 		( operator = AndOperator operand += EqualityExpression
 		| operator = ConditionalAndOperator operand += EqualityExpressionReference ) )*
 ;
 
 AndOperator :
     '&'
 ;
@@ -146,27 +146,27 @@
 ;
 
 EqualityExpressionMember :
 	ownedRelatedElement += EqualityExpression
 ;
 
 EqualityExpression :
-	ClassificationExpression (
+	classification=ClassificationExpression (
 		operator = EqualityOperator operand += ClassificationExpression )*
 
 ;
 
 EqualityOperator :
 	'==' | '!=' | '===' | '!=='
 ;
 
 // Classification Expressions
 
 ClassificationExpression :
-	  RelationalExpression
+	  relational=RelationalExpression
 	  (
 	  	operator = ClassificationTestOperator ownedRelationship += TypeReferenceMember
 	  |
 	    operator = CastOperator ownedRelationship += TypeResultMember
 	  )?
 	|  operand += SelfReferenceExpression
 	  operator = ClassificationTestOperator ownedRelationship += TypeReferenceMember
@@ -191,15 +191,15 @@
 ;
 
 MetaCastOperator :
 	'meta'
 ;
 
 MetadataReference :
-	referencedElement = [QualifiedName]
+	referencedElement = QualifiedName
 ;
 
 TypeReferenceMember :
 	ownedRelatedElement += TypeReference
 ;
 
 TypeResultMember :
@@ -207,15 +207,15 @@
 ;
 
 TypeReference :
 	ownedRelationship += ReferenceTyping
 ;
 
 ReferenceTyping :
-	  type = [QualifiedName]
+	  type = QualifiedName
 ;
 
 SelfReferenceExpression :
 	ownedRelationship += SelfReferenceMember
 ;
 
 SelfReferenceMember :
@@ -225,80 +225,80 @@
 EmptyFeature ://This doesn't work.
 	'emptyfeature'
 ;
 
 // Relational Expressions
 
 RelationalExpression :
-	RangeExpression (
+	range=RangeExpression (
 		operator = RelationalOperator operand += RangeExpression )*
 ;
 
 RelationalOperator :
 	'<' | '>' | '<=' | '>='
 ;
 
 // Range Expressions
 
 RangeExpression :
-	AdditiveExpression (
+	additive=AdditiveExpression (
 		operator = '..' operand += AdditiveExpression )?
 ;
 
 // Arithmetic Expressions
 
 AdditiveExpression :
-	MultiplicativeExpression (
+	multiplicitive=MultiplicativeExpression (
 		operator = AdditiveOperator operand += MultiplicativeExpression )*
 ;
 
 AdditiveOperator :
 	'+' | '-'
 ;
 
 MultiplicativeExpression :
-	ExponentiationExpression (
+	exponential=ExponentiationExpression (
 		operator = MultiplicativeOperator operand += ExponentiationExpression )*
 ;
 
 MultiplicativeOperator :
 	'*' | '/' | '%'
 ;
 
 ExponentiationExpression :
-	UnaryExpression (
+	unary=UnaryExpression (
 		operator = ExponentiationOperator operand += UnaryExpression )*
 ;
 
 ExponentiationOperator :
 	'**' | '^'
 ;
 
 // Unary Expressions
 
 UnaryExpression :
 	   operator = UnaryOperator operand += ExtentExpression
-	| ExtentExpression
+	| extent=ExtentExpression
 ;
 
 UnaryOperator :
 	'+' | '-' | '~' | 'not'
 ;
 
 // Extent Expressions
 
 ExtentExpression :
 	   operator = 'all' ownedRelationship += TypeResultMember
-	| PrimaryExpression
+	| primary=PrimaryExpression
 ;
 
 /* Primary Expressions */
 
 PrimaryExpression :
-	BaseExpression
+	base=BaseExpression
 	(  '.'
 	  ownedRelationship += FeatureChainMember
 	)?
 	( (
 	    operator = '#' '(' operand += SequenceExpression ')'
 	  |
 	    operator = '[' operand += SequenceExpression ']'
@@ -328,28 +328,28 @@
 ;
 
 FunctionReference :
 	ownedRelationship += ReferenceTyping
 ;
 
 FeatureChainMember :
-	  memberElement = [QualifiedName]
+	  memberElement = QualifiedName
 	|  ownedRelatedElement += OwnedFeatureChain
 ;
 
 /* Base Expressions */
 
 BaseExpression :
-	  NullExpression
-	| LiteralExpression
-	| FeatureReferenceExpression
-	| MetadataAccessExpression
-	| InvocationExpression
-	| BodyExpression
-	| '(' SequenceExpression ')'
+	  ownedRelationship=NullExpression
+	| ownedRelationship=LiteralExpression
+	| ownedRelationship=FeatureReferenceExpression
+	| ownedRelationship=MetadataAccessExpression
+	| ownedRelationship=InvocationExpression
+	| ownedRelationship=BodyExpression
+	| '(' ownedRelationship=SequenceExpression ')'
 ;
 
 // Expression Bodies
 
 BodyExpression :
 	ownedRelationship += ExpressionBodyMember
 ;
@@ -389,46 +389,46 @@
 // Feature Reference Expressions
 
 FeatureReferenceExpression :
 	ownedRelationship += FeatureReferenceMember
 ;
 
 FeatureReferenceMember :
-	memberElement = [QualifiedName]
+	memberElement = QualifiedName
 ;
 
 // Metadata Access Expressions
 
 MetadataAccessExpression :
-	referencedElement = [QualifiedName] '.' 'metadata'
+	referencedElement = QualifiedName '.' 'metadata'
 ;
 
 // Invocation Expressions
 
 InvocationExpression :
 	ownedRelationship += OwnedFeatureTyping ArgumentList
 ;
 
 OwnedFeatureTyping :
-	  type = [QualifiedName]
+	  type = QualifiedName
 	| ownedRelatedElement += OwnedFeatureChain
 ;
 
 OwnedFeatureChain :
-	FeatureChain
+	feature=FeatureChain
 ;
 
 // For use in KerML and SysML grammars
  FeatureChain :
-	ownedRelationship += OwnedFeatureChaining
-	( '.' ownedRelationship += OwnedFeatureChaining )+
+	ownedRelationship += OwnedFeatureChaining '.' ownedRelationship += OwnedFeatureChaining
+	( '.' ownedRelationship += OwnedFeatureChaining )*
 ;
 
 OwnedFeatureChaining :
-	chainingFeature = [QualifiedName]
+	chainingFeature = QualifiedName
 ;
 
  ArgumentList :
 	'(' ( PositionalArgumentList | NamedArgumentList )? ')'
 ;
 
  PositionalArgumentList :
@@ -454,15 +454,15 @@
 ;
 
 NamedArgument :
 	ownedRelationship += ParameterRedefinition '=' ownedRelationship += ArgumentValue
 ;
 
 ParameterRedefinition :
-	redefinedFeature = [QualifiedName]
+	redefinedFeature = QualifiedName
 ;
 
 ArgumentValue :
 	ownedRelatedElement += OwnedExpression
 ;
 
 // Null Expressions
@@ -502,50 +502,64 @@
 ;
 
 RealValue :
 	DECIMAL_VALUE? '.' ( DECIMAL_VALUE | EXP_VALUE ) | EXP_VALUE
 ;
 
 LiteralInfinity :
-	 '*'
+	 value='*'
 ;
 
 /* NAMES */
 
+ReservedKeyword:
+  'about' | 'to' | 'connect' | 'connection'
+;
+
 Name:
-	ID | UNRESTRICTED_NAME
+	!ReservedKeyword ID | UNRESTRICTED_NAME
 ;
 
 Qualification :
-	( Name '::' )+
+	( '::' Name )+
 ;
 
 QualifiedName:
-	Qualification? Name
+	name1=Name ( '::' names+=Name )*
 ;
 
 /* TERMINALS */
 
 DECIMAL_VALUE :
    /[0-9]*/;
 
 EXP_VALUE:
 	DECIMAL_VALUE ('e' | 'E') ('+' | '-')? DECIMAL_VALUE;
 
 ID :
    /[a-zA-Z_][a-zA-Z_0-9]*/;
 
 UNRESTRICTED_NAME :
-	/''' ('\' ('b' | 't' | 'n' | 'f' | 'r' | '"' | "'" | '\') | !('\' | '''))* '''/;
+  /* Old format?
+  /''' ('\' ('b' | 't' | 'n' | 'f' | 'r' | '"' | "'" | '\') | !('\' | '''))* '''/;
+  */
+  /[\'].*[\']/;
 
 STRING_VALUE :
-	/'"' ('\' ('b' | 't' | 'n' | 'f' | 'r' | '"' | "'" | '\') | !('\' | '"'))* '"'/;
+	/*/'"' ('\' ('b' | 't' | 'n' | 'f' | 'r' | '"' | "'" | '\') | !('\' | '"'))* '"'/;*/
+  /[\"].*[\"]/;
 
 REGULAR_COMMENT:
-	'/*''*/';
+  /\/\*(.|\n)*?\*\//
+;
+
+Comment:
+// Reserved for textx, but in the model
+  /\/\/.*$/
+;
 
 ML_NOTE:
 	/'\/*'->'*\/'/;
 
 SL_NOTE:
 	/'\/\/' (!('
 ' | '') !('
```

### Comparing `sysml2py-0.1.2/src/sysml2py/grammar/SysML.tx` & `sysml2py-0.3.0/src/sysml2py/grammar/SysML.tx`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-//import grammar.KerML
-//import grammar.KerMLExpressions
+import KerML
+import KerMLExpressions
 /*****************************************************************************
  * SysML 2 Pilot Implementation
  * Copyright (c) 2018-2023 Model Driven Solutions, Inc.
  * Copyright (c) 2018 IncQuery Labs Ltd.
  * Copyright (c) 2019 Maplesoft (Waterloo Maple, Inc.)
  * Copyright (c) 2019 Mgnite Inc.
  *
@@ -48,52 +48,53 @@
 ;
 
 /* DEPENDENCIES */
 
 Dependency :
 	( ownedRelationship += PrefixMetadataAnnotation )*
 	'dependency' ( Identification? 'from' )?
-    client += [QualifiedName] ( ',' client += [QualifiedName] )* 'to'
-    supplier += [QualifiedName] ( ',' supplier += [QualifiedName] )*
+    client += QualifiedName ( ',' client += QualifiedName )* 'to'
+    supplier += QualifiedName ( ',' supplier += QualifiedName )*
     RelationshipBody
 ;
 
 /* ANNOTATIONS */
 
 Annotation :
-	annotatedElement = [QualifiedName]
+	annotatedElement = QualifiedName
 ;
 
 OwnedAnnotation :
 	ownedRelatedElement += AnnotatingElement
 ;
 
 AnnotatingMember :
 	ownedRelatedElement += AnnotatingElement
 ;
 
 AnnotatingElement :
-	  Comment
-	| Documentation
-	| TextualRepresentation
-	| MetadataUsage
+	  ownedRelatedElement = CommentSysML
+	| ownedRelatedElement = Documentation
+	| ownedRelatedElement = TextualRepresentation
+	| ownedRelatedElement = MetadataUsage
 ;
 
 /* Comments */
 
-Comment :
-	( 'comment' Identification?
+CommentSysML :
+// Comment is reserved in TextX
+	( 'comment' identification=Identification?
 	  ('about' ownedRelationship += Annotation
 	     ( ',' ownedRelationship += Annotation )* )?
 	)?
 	body = REGULAR_COMMENT
 ;
 
 Documentation :
-	'doc' Identification? body = REGULAR_COMMENT
+	'doc' identification=Identification? body=REGULAR_COMMENT
 ;
 
 /* Textual Representation */
 
 TextualRepresentation :
     ( 'rep' Identification? )?
     'language' language = STRING_VALUE
@@ -141,15 +142,15 @@
 ;
 
  MetadataUsageDeclaration :
 	( Identification? DefinedByKeyword )? ownedRelationship += MetadataTyping
 ;
 
 MetadataTyping :
-	type = [QualifiedName]
+	type = QualifiedName
 ;
 
  MetadataBody :
 	  ';'
 	| '{' ( ownedRelationship += DefinitionMember
 		  | ownedRelationship += MetadataBodyUsageMember
 		  | ownedRelationship += AliasMember
@@ -161,34 +162,34 @@
 MetadataBodyUsageMember :
 	ownedRelatedElement += MetadataBodyUsage
 ;
 
 MetadataBodyUsage :
 	'ref'? ( ':>>' | 'redefines' )? ownedRelationship += OwnedRedefinition
 	FeatureSpecializationPart? ValuePart?
-	MetadataBody
+	body=MetadataBody
 ;
 
 /* PACKAGES */
 
 /* Packages */
 
 Package :
 	( ownedRelationship += PrefixMetadataMember )*
-	dec=PackageDeclaration body=PackageBody
+	declaration=PackageDeclaration body=PackageBody
 ;
 
 LibraryPackage :
 	( isStandard ?= 'standard' )? 'library'
 	( ownedRelationship += PrefixMetadataMember )*
 	PackageDeclaration PackageBody
 ;
 
- PackageDeclaration :
-	'package' id += Identification?
+PackageDeclaration :
+	'package' identification = Identification?
 ;
 
  PackageBody :
 	 ';'
 	| '{' ( // Note: PackageBodyElement is expanded here to avoid
 			// infinite loops in the incremental parser.
 		    ownedRelationship += PackageMember
@@ -208,65 +209,56 @@
 ;
 
  MemberPrefix :
     ( visibility = VisibilityIndicator )?
 ;
 
 PackageMember :
-	pre = MemberPrefix
-	( ownedRelatedElement += DefinitionElement
-	| ownedRelatedElement += UsageElement
-	)
+	prefix = MemberPrefix
+	( ownedRelatedElement = DefinitionElement | ownedRelatedElement = UsageElement)
 ;
 
 ElementFilterMember :
-	MemberPrefix
+	prefix = MemberPrefix
 	'filter' ownedRelatedElement += OwnedExpression ';'
 ;
 
 AliasMember :
-	MemberPrefix
+	prefix = MemberPrefix
 	'alias' ( '<' memberShortName = Name '>' )? ( memberName = Name )?
-	'for' memberElement = [QualifiedName]
-	RelationshipBody
+	'for' memberElement = QualifiedName
+	body = RelationshipBody
 ;
 
 ImportPrefix :
 	( visibility = VisibilityIndicator )?
 	'import' ( isImportAll ?= 'all' )?
 ;
 
-MembershipNamespace :
-  // Added
-  ( MembershipImport | NamespaceImport )
-;
-
 Import :
-	membership_namespace = MembershipNamespace
-	relationship_body = RelationshipBody
+	(ownedRelationship = NamespaceImport | ownedRelationship = MembershipImport)
+	body = RelationshipBody
 ;
 
 NamespaceImport :
-	import_prefix = ImportPrefix
-	( importedNamespace = ImportedNamespace | ownedRelatedElement += FilterPackage )
+	prefix = ImportPrefix
+	( namespace = ImportedNamespace | ownedRelatedElement += FilterPackage )
 ;
 
 MembershipImport :
-	import_prefix = ImportPrefix imported_membership=ImportedMembership
+	prefix = ImportPrefix membership=ImportedMembership
 ;
 
 ImportedNamespace :
-  // !TODO: This will not work on multi-layered names, qualification breaks the parsing
-	importedNamespace = Qualification* '*'
-	( '::' isRecursive ?= '**' )?
+  // !TODO: Figure out why this breaks
+  namespace = QualifiedName  !'::**' '::*'
 ;
 
 ImportedMembership :
-	importedMembership = QualifiedName
-  ( '::' isRecursive ?= '**' )?
+	importedMembership = QualifiedName ( '::' isRecursive ?= '**' )?
 ;
 
 
 
 FilterPackage :
 	ownedRelationship += FilterPackageImport
 	( ownedRelationship += FilterPackageMember )+
@@ -295,49 +287,49 @@
  VisibilityIndicator :
 	public = 'public' | private = 'private'| protected = 'protected'
 ;
 
 /* Package Elements */
 
 DefinitionElement :
-	  Package
-	| LibraryPackage
-	| AnnotatingElement
-	| Dependency
-	| AttributeDefinition
-	| EnumerationDefinition
-	| OccurrenceDefinition
-	| IndividualDefinition
-	| ItemDefinition
-	| MetadataDefinition
-	| PartDefinition
-	| ConnectionDefinition
-	| FlowConnectionDefinition
-	| InterfaceDefinition
-	| AllocationDefinition
-	| PortDefinition
-	| ActionDefinition
-	| CalculationDefinition
-	| StateDefinition
-	| ConstraintDefinition
-	| RequirementDefinition
-	| ConcernDefinition
-	| CaseDefinition
-	| AnalysisCaseDefinition
-	| VerificationCaseDefinition
-	| UseCaseDefinition
-	| ViewDefinition
-	| ViewpointDefinition
-	| RenderingDefinition
-	| ExtendedDefinition
+	  ownedRelatedElement = Package
+	| ownedRelatedElement = LibraryPackage
+	| ownedRelatedElement = AnnotatingElement
+	| ownedRelatedElement = Dependency
+	| ownedRelatedElement = AttributeDefinition
+	| ownedRelatedElement = EnumerationDefinition
+	| ownedRelatedElement = OccurrenceDefinition
+	| ownedRelatedElement = IndividualDefinition
+	| ownedRelatedElement = ItemDefinition
+	| ownedRelatedElement = MetadataDefinition
+	| ownedRelatedElement = PartDefinition
+	| ownedRelatedElement = ConnectionDefinition
+	| ownedRelatedElement = FlowConnectionDefinition
+	| ownedRelatedElement = InterfaceDefinition
+	| ownedRelatedElement = AllocationDefinition
+	| ownedRelatedElement = PortDefinition
+	| ownedRelatedElement = ActionDefinition
+	| ownedRelatedElement = CalculationDefinition
+	| ownedRelatedElement = StateDefinition
+	| ownedRelatedElement = ConstraintDefinition
+	| ownedRelatedElement = RequirementDefinition
+	| ownedRelatedElement = ConcernDefinition
+	| ownedRelatedElement = CaseDefinition
+	| ownedRelatedElement = AnalysisCaseDefinition
+	| ownedRelatedElement = VerificationCaseDefinition
+	| ownedRelatedElement = UseCaseDefinition
+	| ownedRelatedElement = ViewDefinition
+	| ownedRelatedElement = ViewpointDefinition
+	| ownedRelatedElement = RenderingDefinition
+	| ownedRelatedElement = ExtendedDefinition
 ;
 
 UsageElement :
-	  NonOccurrenceUsageElement
-	| OccurrenceUsageElement
+	  ownedRelatedElement = NonOccurrenceUsageElement
+	| ownedRelatedElement = OccurrenceUsageElement
 ;
 
 /* CLASSIFIERS */
 
 /* Superclassing */
 
  SubclassificationPart :
@@ -346,110 +338,112 @@
 ;
 
 SpecializesKeyword :
 	':>' | 'specializes'
 ;
 
 OwnedSubclassification :
-	superclassifier = [QualifiedName]
+	superclassifier = QualifiedName
 ;
 
 /* FEATURES */
 
 /* Features */
 
  FeatureDeclaration :
-	  Identification FeatureSpecializationPart?
-	| FeatureSpecializationPart
+	  identification=Identification specialization=FeatureSpecializationPart?
+	| specialization=FeatureSpecializationPart
 ;
 
  FeatureSpecializationPart :
-	  ( FeatureSpecialization )+ MultiplicityPart? FeatureSpecialization*
-	| MultiplicityPart FeatureSpecialization*
+	  ( specialization+=FeatureSpecialization )+ multiplicity=MultiplicityPart? specialization2+=FeatureSpecialization*
+	| multiplicity2=MultiplicityPart specialization+=FeatureSpecialization*
 ;
 
  MultiplicityPart :
 	  ownedRelationship += OwnedMultiplicity
 	| ( ownedRelationship += OwnedMultiplicity )?
 
 ( isOrdered ?= 'ordered' isNonunique ?= 'nonunique'
    | isNonunique2 ?= 'nonunique' isOrdered2 ?= 'ordered'
 )
 
 ;
 
  FeatureSpecialization :
-	Typings | Subsettings | References | Redefinitions
+	ownedRelationship=Typings | ownedRelationship=Subsettings | ownedRelationship=References | ownedRelationship=Redefinitions
 ;
 
  Typings :
-	TypedBy ( ',' ownedRelationship += FeatureTyping )*
+	typedby=TypedBy ( ',' ownedRelationship += FeatureTyping )*
 ;
 
  TypedBy :
 	DefinedByKeyword ownedRelationship += FeatureTyping
 ;
 
 DefinedByKeyword :
 	':' | 'defined' 'by'
 ;
 
  Subsettings :
-	Subsets ( ',' ownedRelationship += OwnedSubsetting )*
+	SubsetsKeyword ownedRelationship += OwnedSubsetting ( ',' ownedRelationship += OwnedSubsetting )*
 ;
 
- Subsets :
+/* Subsets :
 	SubsetsKeyword ownedRelationship += OwnedSubsetting
-;
+;*/
 
 SubsetsKeyword :
 	':>' | 'subsets'
 ;
 
  References :
 	ReferencesKeyword ownedRelationship += OwnedReferenceSubsetting
 ;
 
 ReferencesKeyword :
 	'::>' | 'references'
 ;
 
  Redefinitions :
-	Redefines ( ',' ownedRelationship += OwnedRedefinition )*
+	redefines=Redefines ( ',' ownedRelationship += OwnedRedefinition )*
 ;
 
  Redefines :
 	RedefinesKeyword ownedRelationship += OwnedRedefinition
 ;
 
 RedefinesKeyword :
 	':>>' | 'redefines'
 ;
 
 /* Feature Typing, Subsetting and Redefinition */
 
 FeatureTyping :
-	OwnedFeatureTyping | ConjugatedPortTyping
+	ownedRelationship = OwnedFeatureTyping | ownedRelationship = ConjugatedPortTyping
 ;
 
 // OwnedFeatureTyping inherited from Expression syntax.
 
 OwnedSubsetting :
-	  subsettedFeature = [QualifiedName]
-	| ownedRelatedElement += OwnedFeatureChain
+	  ownedRelatedElement += OwnedFeatureChain
+	| subsettedFeature = QualifiedName
 ;
 
 OwnedReferenceSubsetting :
-	  referencedFeature = [QualifiedName]
-	| ownedRelatedElement += OwnedFeatureChain
+	  ownedRelatedElement += OwnedFeatureChain
+	| referencedFeature = QualifiedName
+  // Always check for feature chain first.
+
 ;
 
 OwnedRedefinition :
-	  redefinedFeature = [QualifiedName]
-	| ownedRelatedElement += OwnedFeatureChain
+	  ownedRelatedElement += OwnedFeatureChain
+	| redefinedFeature = QualifiedName
 ;
 
 /* Multiplicity */
 
 OwnedMultiplicity :
 	ownedRelatedElement += MultiplicityRange
 ;
@@ -458,15 +452,15 @@
 	// TODO: Allow general expressions for bounds. (Causes LL parsing issues.)
 	'[' ownedRelationship += MultiplicityExpressionMember
 	      ( '..' ownedRelationship += MultiplicityExpressionMember )? ']'
 ;
 
 
 MultiplicityRelatedElement :
-    (LiteralExpression | FeatureReferenceExpression)
+    (ownedRelatedElement = LiteralExpression | ownedRelatedElement = FeatureReferenceExpression)
 ;
 
 MultiplicityExpressionMember :
     ownedRelatedElement += MultiplicityRelatedElement
 ;
 
 /* DEFINITION AND USAGE */
@@ -478,116 +472,116 @@
 ;
 
  DefinitionExtensionKeyword :
 	ownedRelationship += PrefixMetadataMember
 ;
 
  DefinitionPrefix :
-	BasicDefinitionPrefix? DefinitionExtensionKeyword*
+	prefix=BasicDefinitionPrefix? keyword+=DefinitionExtensionKeyword*
 ;
 
  Definition :
-	DefinitionDeclaration DefinitionBody
+	declaration=DefinitionDeclaration body=DefinitionBody
 ;
 
  DefinitionDeclaration :
-	Identification? SubclassificationPart?
+	identification=Identification? subclassificationpart=SubclassificationPart?
 ;
 
  DefinitionBody :
-	';' | '{' DefinitionBodyItem* '}'
+	';' | '{' ownedRelatedElement+=DefinitionBodyItem* '}'
 ;
 
  DefinitionBodyItem :
 	  ownedRelationship += DefinitionMember
 	| ownedRelationship += VariantUsageMember
 	| ownedRelationship += NonOccurrenceUsageMember
 	| ( ownedRelationship += EmptySuccessionMember )?
 	  ownedRelationship += OccurrenceUsageMember
 	| ownedRelationship += AliasMember
 	| ownedRelationship += Import
 ;
 
 DefinitionMember :
-	MemberPrefix
+	prefix = MemberPrefix
 	ownedRelatedElement += DefinitionElement
 ;
 
 VariantUsageMember :
 	MemberPrefix 'variant'
 	ownedRelatedElement += VariantUsageElement
 ;
 
 NonOccurrenceUsageMember :
-	MemberPrefix ownedRelatedElement += NonOccurrenceUsageElement
+	prefix=MemberPrefix ownedRelatedElement += NonOccurrenceUsageElement
 ;
 
 OccurrenceUsageMember :
-	MemberPrefix ownedRelatedElement += OccurrenceUsageElement
+	prefix=MemberPrefix ownedRelatedElement += OccurrenceUsageElement
 ;
 
 StructureUsageMember :
 	MemberPrefix ownedRelatedElement += StructureUsageElement
 ;
 
 BehaviorUsageMember :
 	MemberPrefix ownedRelatedElement += BehaviorUsageElement
 ;
 
 /* Usages */
 
  FeatureDirection :
-	in = 'in' | out = 'out' | inout = 'inout'
+	in = 'in ' | out = 'out' | inout = 'inout'
 ;
 
  RefPrefix :
 	( direction = FeatureDirection )?
 	( isAbstract ?= 'abstract' | isVariation ?= 'variation')?
 	( isReadOnly ?= 'readonly' )?
 	( isDerived ?= 'derived' )?
 	( isEnd ?= 'end' )?
 ;
 
  BasicUsagePrefix :
-	RefPrefix
+	prefix=RefPrefix
 	( isReference ?= 'ref' )?
 ;
 
  UsageExtensionKeyword :
 	ownedRelationship += PrefixMetadataMember
 ;
 
  UsagePrefix :
 	BasicUsagePrefix UsageExtensionKeyword*
 ;
 
  Usage :
-	UsageDeclaration? UsageCompletion
+	declaration=UsageDeclaration? completion=UsageCompletion
 ;
 
  UsageDeclaration :
-	  FeatureDeclaration
+	  declaration=FeatureDeclaration
 ;
 
  UsageCompletion :
-	ValuePart? UsageBody
+	valuepart=ValuePart? body=UsageBody
 ;
 
  UsageBody :
-	DefinitionBody
+	body=DefinitionBody
 ;
 
  ValuePart :
 	  ownedRelationship += FeatureValue
 	| ownedRelationship += FeatureValueExpression
 	  ownedRelationship += EmptyAssignmentActionMember
 ;
 
 FeatureValue :
-	( '=' | isDefault ?= 'default' ( '=' | isInitial ?= ':=' )? )
+	( '=' | isDefault ?= 'default' ( isEqual ?= '=' | isInitial ?= ':=' )? )
 	ownedRelatedElement += OwnedExpression
 ;
 
 FeatureValueExpression :
 	isInitial ?= ':='
 	ownedRelatedElement += OwnedExpression
 ;
@@ -616,58 +610,58 @@
 ;
 
 ReferenceUsageKeyword :
 	ReferenceKeyword
 ;
 
 DefaultReferenceUsage :
-	RefPrefix UsageDeclaration ValuePart? UsageBody
+	prefix=RefPrefix declaration=UsageDeclaration valuepart=ValuePart? body=UsageBody
 ;
 
 ReferenceUsage :
 	RefPrefix ReferenceUsageKeyword Usage
 ;
 
 VariantReference :
 	ownedRelationship += OwnedReferenceSubsetting
 	FeatureSpecialization* UsageBody
 ;
 
 /* Body Elements */
 
 NonOccurrenceUsageElement :
-	  DefaultReferenceUsage
-	| ReferenceUsage
-	| AttributeUsage
-	| EnumerationUsage
-	| BindingConnector
-	| Succession
-	| ExtendedUsage
+	  ownedRelatedElement = DefaultReferenceUsage
+	| ownedRelatedElement = ReferenceUsage
+	| ownedRelatedElement = AttributeUsage
+	| ownedRelatedElement = EnumerationUsage
+	| ownedRelatedElement = BindingConnector
+	| ownedRelatedElement = Succession
+	| ownedRelatedElement = ExtendedUsage
 ;
 
 OccurrenceUsageElement :
-	StructureUsageElement | BehaviorUsageElement
+	ownedRelatedElement = StructureUsageElement | ownedRelatedElement = BehaviorUsageElement
 ;
 
 StructureUsageElement :
-	  OccurrenceUsage
-	| IndividualUsage
-	| PortionUsage
-	| EventOccurrenceUsage
-	| ItemUsage
-	| PartUsage
-	| ViewUsage
-	| RenderingUsage
-	| PortUsage
-	| ConnectionUsage
-	| InterfaceUsage
-	| AllocationUsage
-	| Message
-	| FlowConnectionUsage
-	| SuccessionFlowConnectionUsage
+	  ownedRelatedElement = OccurrenceUsage
+	| ownedRelatedElement = IndividualUsage
+	| ownedRelatedElement = PortionUsage
+	| ownedRelatedElement = EventOccurrenceUsage
+	| ownedRelatedElement = ItemUsage
+	| ownedRelatedElement = PartUsage
+	| ownedRelatedElement = ViewUsage
+	| ownedRelatedElement = RenderingUsage
+	| ownedRelatedElement = PortUsage
+	| ownedRelatedElement = ConnectionUsage
+	| ownedRelatedElement = InterfaceUsage
+	| ownedRelatedElement = AllocationUsage
+	| ownedRelatedElement = Message
+	| ownedRelatedElement = FlowConnectionUsage
+	| ownedRelatedElement = SuccessionFlowConnectionUsage
 ;
 
 BehaviorUsageElement :
 	  ActionUsage
 	| CalculationUsage
 	| StateUsage
 	| ConstraintUsage
@@ -730,56 +724,58 @@
 ;
 
 AttributeUsageKeyword :
 	AttributeKeyword
 ;
 
 AttributeDefinition :
-	DefinitionPrefix AttributeDefKeyword Definition
+	prefix=DefinitionPrefix AttributeDefKeyword definition=Definition
 ;
 
 AttributeUsage :
-	UsagePrefix AttributeUsageKeyword Usage
+	prefix=UsagePrefix AttributeUsageKeyword usage=Usage
 ;
 
 /* ENUMERATIONS */
 
 EnumerationKeyword :
-	''
+	'enum'
 ;
 EnumerationDefKeyword :
 	EnumerationKeyword 'def'
 ;
 
 EnumerationUsageKeyword :
 	EnumerationKeyword
 ;
 
 EnumerationDefinition :
-	EnumerationDefKeyword DefinitionDeclaration EnumerationBody
+	EnumerationDefKeyword
+  declaration=DefinitionDeclaration
+  body=EnumerationBody
 ;
 
  EnumerationBody :
 	  ';'
 	| '{' ( ownedRelationship += AnnotatingMember
 		  | ownedRelationship += EnumerationUsageMember
 		  )*
 	  '}'
 ;
 
 EnumerationUsageMember :
-	MemberPrefix ownedRelatedElement += EnumeratedValue
+	prefix=MemberPrefix ownedRelatedElement += EnumeratedValue
 ;
 
 EnumeratedValue :
-	EnumerationUsageKeyword? Usage
+	keyword=EnumerationUsageKeyword? usage=Usage
 ;
 
 EnumerationUsage :
-	UsagePrefix EnumerationUsageKeyword Usage
+	prefix=UsagePrefix EnumerationUsageKeyword usage=Usage
 ;
 
 /* OCCURRENCES */
 
 /* Occurrence Definitions */
 
 OccurrenceKeyword :
@@ -787,17 +783,17 @@
 ;
 
 OccurrenceDefKeyword :
 	OccurrenceKeyword 'def'
 ;
 
  OccurrenceDefinitionPrefix :
-	BasicDefinitionPrefix?
+	prefix=BasicDefinitionPrefix?
 	( isIndividual ?= 'individual' ownedRelationship += LifeClassMembership )?
-	DefinitionExtensionKeyword*
+	keyword=DefinitionExtensionKeyword*
 ;
 
 OccurrenceDefinition :
 	OccurrenceDefinitionPrefix OccurrenceDefKeyword Definition
 ;
 
 IndividualDefinition :
@@ -817,27 +813,27 @@
 /* Occurrence Usages */
 
 OccurrenceUsageKeyword :
 	OccurrenceKeyword
 ;
 
  OccurrenceUsagePrefix :
-	  BasicUsagePrefix
+	  prefix=BasicUsagePrefix
 	  ( isIndividual ?= 'individual' )?
 	  ( portionKind = PortionKind )?
-	  UsageExtensionKeyword*
+	  usageExtension=UsageExtensionKeyword*
 ;
 
 OccurrenceUsage :
-	OccurrenceUsagePrefix OccurrenceUsageKeyword Usage
+	prefix=OccurrenceUsagePrefix OccurrenceUsageKeyword usage=Usage
 ;
 
 IndividualUsage :
-	BasicUsagePrefix isIndividual ?= 'individual'
-	UsageExtensionKeyword* Usage
+	prefix=BasicUsagePrefix isIndividual ?= 'individual'
+	UsageExtensionKeyword* usage=Usage
 ;
 
 PortionUsage :
 	BasicUsagePrefix ( isIndividual ?= 'individual' )?
 	portionKind = PortionKind
 	UsageExtensionKeyword* Usage
 ;
@@ -892,19 +888,19 @@
 ;
 
 ItemUsageKeyword :
 	ItemKeyword
 ;
 
 ItemDefinition :
-	OccurrenceDefinitionPrefix ItemDefKeyword Definition
+	prefix=OccurrenceDefinitionPrefix ItemDefKeyword definition=Definition
 ;
 
 ItemUsage :
-	OccurrenceUsagePrefix ItemUsageKeyword Usage
+	prefix=OccurrenceUsagePrefix ItemUsageKeyword usage=Usage
 ;
 
 /* PARTS */
 
 PartKeyword :
 	'part'
 ;
@@ -914,19 +910,19 @@
 ;
 
 PartUsageKeyword :
 	PartKeyword
 ;
 
 PartDefinition :
-	OccurrenceDefinitionPrefix PartDefKeyword Definition
+	prefix = OccurrenceDefinitionPrefix PartDefKeyword definition = Definition
 ;
 
 PartUsage :
-	OccurrenceUsagePrefix PartUsageKeyword Usage
+	prefix=OccurrenceUsagePrefix PartUsageKeyword usage=Usage
 ;
 
 /* PORTS */
 
 /* Port Definitions */
 
 PortKeyword :
@@ -934,16 +930,16 @@
 ;
 
 PortDefKeyword :
 	PortKeyword 'def'
 ;
 
 PortDefinition :
-	DefinitionPrefix PortDefKeyword Definition
-	ownedRelationship += ConjugatedPortDefinitionMember
+	prefix=DefinitionPrefix PortDefKeyword definition=Definition
+	//(ownedRelationship += ConjugatedPortDefinitionMember)
 ;
 
 ConjugatedPortDefinitionMember :
 	ownedRelatedElement += ConjugatedPortDefinition
 ;
 
 ConjugatedPortDefinition :
@@ -951,29 +947,29 @@
 ;
 
 PortConjugation ://This doesn't work.
 	'portconjugation'
 ;
 
 ConjugatedPortTyping :
-	conjugatedPortDefinition = [ConjugatedQualifiedName|ConjugatedQualifiedName]
+	conjugatedPortDefinition = ConjugatedQualifiedName
 ;
 
 ConjugatedQualifiedName :
 	'~' QualifiedName
 ;
 
 /* Port Usages */
 
 PortUsageKeyword :
 	PortKeyword
 ;
 
 PortUsage :
-	OccurrenceUsagePrefix PortUsageKeyword Usage
+	prefix=OccurrenceUsagePrefix PortUsageKeyword usage=Usage
 ;
 
 /* CONNECTIONS */
 
 /* Connectors */
 
 ConnectorEndMember :
@@ -1019,37 +1015,39 @@
 ;
 
 ConnectionDefKeyword :
 	ConnectionKeyword 'def'
 ;
 
 ConnectionDefinition :
-	OccurrenceDefinitionPrefix ConnectionDefKeyword Definition
+	prefix=OccurrenceDefinitionPrefix ConnectionDefKeyword definition=Definition
 ;
 
 /* Connection Usages */
 
 ConnectorKeyword :
 	'connect'
 ;
 
 ConnectionUsageKeyword :
 	ConnectionKeyword
 ;
 
 ConnectionUsage :
-	OccurrenceUsagePrefix
-	( ConnectionUsageKeyword UsageDeclaration?
-	  ( ConnectorKeyword ConnectorPart )?
-	| ConnectorKeyword ConnectorPart
-	) UsageBody
+	prefix=OccurrenceUsagePrefix
+	(
+    ConnectionUsageKeyword declaration=UsageDeclaration? ( ConnectorKeyword part=ConnectorPart )?
+  |
+    ConnectorKeyword part=ConnectorPart
+  )
+  body=UsageBody
 ;
 
  ConnectorPart :
-	BinaryConnectorPart | NaryConnectorPart
+	part=BinaryConnectorPart | part=NaryConnectorPart
 ;
 
  BinaryConnectorPart :
 	ownedRelationship += ConnectorEndMember 'to'
 	ownedRelationship += ConnectorEndMember
 ;
 
@@ -1165,15 +1163,15 @@
 
 FlowEnd :
 	( ownedRelationship += FlowEndSubsetting )?
 	ownedRelationship += FlowFeatureMember
 ;
 
 FlowEndSubsetting :
-	  referencedFeature = [QualifiedName] '.'
+	  referencedFeature = QualifiedName '.'
 	| ownedRelatedElement += FeatureChainPrefix
 ;
 
 FeatureChainPrefix :
 	( ownedRelationship += OwnedFeatureChaining '.' )+
 	ownedRelationship += OwnedFeatureChaining '.'
 ;
@@ -1183,15 +1181,15 @@
 ;
 
 FlowFeature :
 	ownedRelationship += FlowRedefinition
 ;
 
 FlowRedefinition :
-	redefinedFeature = [QualifiedName]
+	redefinedFeature = QualifiedName
 ;
 
 /* INTERFACES */
 
 /* Interface Definitions */
 
 InterfaceKeyword :
@@ -1199,19 +1197,19 @@
 ;
 
 InterfaceDefKeyword :
 	InterfaceKeyword 'def'
 ;
 
 InterfaceDefinition :
-	OccurrenceDefinitionPrefix InterfaceDefKeyword DefinitionDeclaration InterfaceBody
+	prefix=OccurrenceDefinitionPrefix InterfaceDefKeyword declaration=DefinitionDeclaration body=InterfaceBody
 ;
 
  InterfaceBody :
-	';' | '{' InterfaceBodyItem* '}'
+	';' | '{' item+=InterfaceBodyItem* '}'
 ;
 
  InterfaceBodyItem :
 	  ownedRelationship += DefinitionMember
 	| ownedRelationship += VariantUsageMember
 	| ownedRelationship += InterfaceNonOccurrenceUsageMember
 	| ( ownedRelationship += EmptySuccessionMember )?
@@ -1229,58 +1227,58 @@
 	| AttributeUsage
 	| EnumerationUsage
 	| BindingConnector
 	| Succession
 ;
 
 InterfaceOccurrenceUsageMember :
-	MemberPrefix ownedRelatedElement += InterfaceOccurrenceUsageElement
+	prefix=MemberPrefix ownedRelatedElement += InterfaceOccurrenceUsageElement
 ;
 
 InterfaceOccurrenceUsageElement :
-	DefaultInterfaceEnd | StructureUsageElement | BehaviorUsageElement
+	element=DefaultInterfaceEnd | element=StructureUsageElement | element=BehaviorUsageElement
 ;
 
 DefaultInterfaceEnd :
 	( direction = FeatureDirection )?
 	( isAbstract ?= 'abstract' | isVariation ?= 'variation')?
-	isEnd ?= 'end' Usage
+	isEnd ?= 'end' usage=Usage
 ;
 
 /* Interface Usages */
 
 InterfaceUsageKeyword :
 	InterfaceKeyword
 ;
 
 InterfaceUsage :
-	OccurrenceUsagePrefix InterfaceUsageKeyword InterfaceUsageDeclaration InterfaceBody
+	prefix=OccurrenceUsagePrefix InterfaceUsageKeyword declaration=InterfaceUsageDeclaration body=InterfaceBody
 ;
 
  InterfaceUsageDeclaration :
-	UsageDeclaration? ( ConnectorKeyword InterfacePart )? | InterfacePart
+	declaration=UsageDeclaration? ( ConnectorKeyword part1=InterfacePart )? | part2=InterfacePart
 ;
 
  InterfacePart :
-	BinaryInterfacePart | NaryInterfacePart
+	binarypart=BinaryInterfacePart | narypart=NaryInterfacePart
 ;
 
  BinaryInterfacePart :
 	ownedRelationship += InterfaceEndMember 'to'
 	ownedRelationship += InterfaceEndMember
 ;
 
  NaryInterfacePart :
 	'(' ownedRelationship += InterfaceEndMember ','
 	    ownedRelationship += InterfaceEndMember
 	    ( ',' ownedRelationship += InterfaceEndMember )* ')'
 ;
 
 InterfaceEndMember :
-	ownedRelatedElement += InterfaceEnd
+	ownedRelatedElement = InterfaceEnd
 ;
 
 InterfaceEnd :
 	( declaredName = Name ReferencesKeyword )?
 	ownedRelationship += OwnedReferenceSubsetting
 	( ownedRelationship += OwnedMultiplicity )?
 ;
@@ -1362,15 +1360,15 @@
 	  ownedRelationship += ActionBodyItemTarget
 	  ( ownedRelationship += TargetSuccessionMember )*
 	| ownedRelationship += GuardedSuccessionMember
 ;
 
 
 InitialNodeMember :
-	MemberPrefix 'first' memberElement = [QualifiedName]
+	MemberPrefix 'first' memberElement = QualifiedName
 	RelationshipBody
 ;
 
 ActionNodeMember :
 	MemberPrefix ownedRelatedElement += ActionNode
 ;
 
@@ -1850,16 +1848,16 @@
 	  ( ownedRelationship += EffectBehaviorMember )?
 	)?
 	'then' ownedRelationship += TransitionSuccessionMember
 	ActionBody
 ;
 
 TransitionSourceMember :
-	  memberElement = [QualifiedName]
-	|  ownedRelatedElement += OwnedFeatureChain
+	  ownedRelatedElement += OwnedFeatureChain
+	| memberElement = QualifiedName
 ;
 
 TriggerActionMember :
 	kind = TriggerFeatureKind ownedRelatedElement += TriggerAction
 ;
 
  TriggerFeatureKind :
```

### Comparing `sysml2py-0.1.2/src/sysml2py/textx/xtext_to_textx.py` & `sysml2py-0.3.0/src/sysml2py/textx/xtext_to_textx.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.1.2/sysml2py.egg-info/PKG-INFO` & `sysml2py-0.3.0/sysml2py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysml2py
-Version: 0.1.2
+Version: 0.3.0
 Summary: SysML v2.0 Parser
 Author-email: Christopher Cox <chris.cox@westfall.io>
 Project-URL: Homepage, https://github.com/Westfall-io/sysml2py
 Project-URL: Bug Tracker, https://github.com/Westfall-io/sysml2py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

