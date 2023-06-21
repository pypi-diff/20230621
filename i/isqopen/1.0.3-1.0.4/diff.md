# Comparing `tmp/isqopen-1.0.3.tar.gz` & `tmp/isqopen-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/isqopen-1.0.3.tar", last modified: Tue May 30 02:39:13 2023, max compression
+gzip compressed data, was "dist/isqopen-1.0.4.tar", last modified: Wed Jun 21 07:08:45 2023, max compression
```

## Comparing `isqopen-1.0.3.tar` & `isqopen-1.0.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.916114 isqopen-1.0.3/
--rw-r--r--   0 huazhelou   (501) staff       (20)     1093 2022-09-07 10:16:53.000000 isqopen-1.0.3/LICENSE
--rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-05-30 02:39:13.916269 isqopen-1.0.3/PKG-INFO
--rw-r--r--   0 huazhelou   (501) staff       (20)      734 2022-09-24 07:03:24.000000 isqopen-1.0.3/README.md
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.889571 isqopen-1.0.3/isq/
--rw-r--r--   0 huazhelou   (501) staff       (20)      273 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/__init__.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.903533 isqopen-1.0.3/isq/compile/
--rw-r--r--   0 huazhelou   (501) staff       (20)     5836 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/QSyn.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    11380 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/Simplify.py
--rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5152 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/matlab_gsvd.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    15317 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/parser.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    25877 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/parsetab.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    36609 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/passes.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5111 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/qtypes.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2227 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/tokrules.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2539 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/compile/tools.py
--rw-r--r--   0 huazhelou   (501) staff       (20)       18 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/config.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.907285 isqopen-1.0.3/isq/device/
--rw-r--r--   0 huazhelou   (501) staff       (20)      142 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/device/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     6745 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/device/device.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     1882 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/device/grad.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     3166 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/device/task.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5354 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/device/translate.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.908686 isqopen-1.0.3/isq/draw/
--rw-r--r--   0 huazhelou   (501) staff       (20)       26 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/draw/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     7986 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/draw/drawer.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2652 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/errors.py
--rw-r--r--   0 huazhelou   (501) staff       (20)      644 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/globalVar.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    10006 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/mapping.py
--rw-r--r--   0 huazhelou   (501) staff       (20)      250 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/qpu.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     6707 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/quantum.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.910880 isqopen-1.0.3/isq/simulate/
--rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/simulate/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    13705 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/simulate/operation.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5523 2023-05-30 02:37:24.000000 isqopen-1.0.3/isq/simulate/simulator.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-30 02:39:13.915709 isqopen-1.0.3/isqopen.egg-info/
--rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-05-30 02:39:13.000000 isqopen-1.0.3/isqopen.egg-info/PKG-INFO
--rw-r--r--   0 huazhelou   (501) staff       (20)      775 2023-05-30 02:39:13.000000 isqopen-1.0.3/isqopen.egg-info/SOURCES.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-05-30 02:39:13.000000 isqopen-1.0.3/isqopen.egg-info/dependency_links.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-05-30 02:39:13.000000 isqopen-1.0.3/isqopen.egg-info/not-zip-safe
--rw-r--r--   0 huazhelou   (501) staff       (20)       57 2023-05-30 02:39:13.000000 isqopen-1.0.3/isqopen.egg-info/requires.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        4 2023-05-30 02:39:13.000000 isqopen-1.0.3/isqopen.egg-info/top_level.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)      107 2023-05-30 02:39:13.917122 isqopen-1.0.3/setup.cfg
--rw-r--r--   0 huazhelou   (501) staff       (20)      738 2023-05-30 02:37:49.000000 isqopen-1.0.3/setup.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-06-21 07:08:45.424347 isqopen-1.0.4/
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1093 2022-09-07 10:16:53.000000 isqopen-1.0.4/LICENSE
+-rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-06-21 07:08:45.424472 isqopen-1.0.4/PKG-INFO
+-rw-r--r--   0 huazhelou   (501) staff       (20)      734 2022-09-24 07:03:24.000000 isqopen-1.0.4/README.md
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-06-21 07:08:45.408417 isqopen-1.0.4/isq/
+-rw-r--r--   0 huazhelou   (501) staff       (20)      273 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/__init__.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-06-21 07:08:45.415936 isqopen-1.0.4/isq/compile/
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5836 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/compile/QSyn.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    11380 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/compile/Simplify.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/compile/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5152 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/compile/matlab_gsvd.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    15317 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/compile/parser.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    25877 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/compile/parsetab.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    36599 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/compile/passes.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5111 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/compile/qtypes.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2227 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/compile/tokrules.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2539 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/compile/tools.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)       18 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/config.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-06-21 07:08:45.419210 isqopen-1.0.4/isq/device/
+-rw-r--r--   0 huazhelou   (501) staff       (20)      142 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/device/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     6735 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/device/device.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1882 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/device/grad.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     3166 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/device/task.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5354 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/device/translate.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-06-21 07:08:45.420404 isqopen-1.0.4/isq/draw/
+-rw-r--r--   0 huazhelou   (501) staff       (20)       26 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/draw/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     7986 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/draw/drawer.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2652 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/errors.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)      644 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/globalVar.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    10006 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/mapping.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)      250 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/qpu.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     6707 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/quantum.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-06-21 07:08:45.421885 isqopen-1.0.4/isq/simulate/
+-rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/simulate/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    13705 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/simulate/operation.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5523 2023-06-21 07:05:34.000000 isqopen-1.0.4/isq/simulate/simulator.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-06-21 07:08:45.424101 isqopen-1.0.4/isqopen.egg-info/
+-rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-06-21 07:08:45.000000 isqopen-1.0.4/isqopen.egg-info/PKG-INFO
+-rw-r--r--   0 huazhelou   (501) staff       (20)      775 2023-06-21 07:08:45.000000 isqopen-1.0.4/isqopen.egg-info/SOURCES.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-06-21 07:08:45.000000 isqopen-1.0.4/isqopen.egg-info/dependency_links.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-06-21 07:08:45.000000 isqopen-1.0.4/isqopen.egg-info/not-zip-safe
+-rw-r--r--   0 huazhelou   (501) staff       (20)       57 2023-06-21 07:08:45.000000 isqopen-1.0.4/isqopen.egg-info/requires.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        4 2023-06-21 07:08:45.000000 isqopen-1.0.4/isqopen.egg-info/top_level.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)      107 2023-06-21 07:08:45.424966 isqopen-1.0.4/setup.cfg
+-rw-r--r--   0 huazhelou   (501) staff       (20)      738 2023-06-21 07:08:00.000000 isqopen-1.0.4/setup.py
```

### Comparing `isqopen-1.0.3/LICENSE` & `isqopen-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/PKG-INFO` & `isqopen-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isqopen
-Version: 1.0.3
+Version: 1.0.4
 Summary: isq quantum kernel
 Author: Lou Huazhe
 Author-email: louhz@arclightquantum.com
 Platform: python 3.8+
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `isqopen-1.0.3/README.md` & `isqopen-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/compile/QSyn.py` & `isqopen-1.0.4/isq/compile/QSyn.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/compile/Simplify.py` & `isqopen-1.0.4/isq/compile/Simplify.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/compile/matlab_gsvd.py` & `isqopen-1.0.4/isq/compile/matlab_gsvd.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/compile/parser.py` & `isqopen-1.0.4/isq/compile/parser.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/compile/parsetab.py` & `isqopen-1.0.4/isq/compile/parsetab.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,105 +23,105 @@
 for _k, _v in _lr_goto_items.items():
    for _x, _y in zip(_v[0], _v[1]):
        if not _x in _lr_goto: _lr_goto[_x] = {}
        _lr_goto[_x][_k] = _y
 del _lr_goto_items
 _lr_productions = [
   ("S' -> program","S'",1,None,None,None),
-  ('program -> varDef procedureBody','program',2,'p_program','parser.py',38),
-  ('program -> gateDef varDef procedureBody','program',3,'p_program','parser.py',39),
-  ('gateDef -> gateDefclause','gateDef',1,'p_gateDef','parser.py',51),
-  ('gateDef -> gateDefclause gateDef','gateDef',2,'p_gateDef','parser.py',52),
-  ('gDefID -> ID','gDefID',1,'p_gDefID','parser.py',59),
-  ('gateDefclause -> DEFGATE gDefID = [ matrixContents ] ;','gateDefclause',7,'p_gateDefclause','parser.py',68),
-  ('matrixContents -> CNUMBER','matrixContents',1,'p_matrixContents','parser.py',73),
-  ('matrixContents -> CNUMBER , matrixContents','matrixContents',3,'p_matrixContents','parser.py',74),
-  ('matrixContents -> CNUMBER ; matrixContents','matrixContents',3,'p_matrixContents','parser.py',75),
-  ('CNUMBER -> NumberExpr','CNUMBER',1,'p_CNUMBER','parser.py',82),
-  ('CNUMBER -> - NumberExpr','CNUMBER',2,'p_CNUMBER','parser.py',83),
-  ('NumberExpr -> NUMBER','NumberExpr',1,'p_NumberExpr','parser.py',90),
-  ('NumberExpr -> NUMBER + NUMBER','NumberExpr',3,'p_NumberExpr','parser.py',91),
-  ('NumberExpr -> NUMBER - NUMBER','NumberExpr',3,'p_NumberExpr','parser.py',92),
-  ('varDef -> defclause','varDef',1,'p_varDef','parser.py',98),
-  ('varDef -> varDef defclause','varDef',2,'p_varDef','parser.py',99),
-  ('defclause -> QBIT seen_Qbit id_list ;','defclause',4,'p_defclause','parser.py',107),
-  ('defclause -> QCOUPLE id_list ;','defclause',3,'p_defclause','parser.py',108),
-  ('defclause -> VAR ID = NUMBER ;','defclause',5,'p_defclause','parser.py',109),
-  ('defclause -> VAR ID [ NUMBER ] = { matrixContents } ;','defclause',10,'p_defclause','parser.py',110),
-  ('seen_Qbit -> <empty>','seen_Qbit',0,'p_seen_Qbit','parser.py',124),
-  ('id_list -> ID','id_list',1,'p_id_list','parser.py',130),
-  ('id_list -> id_list , ID','id_list',3,'p_id_list','parser.py',131),
-  ('id_list -> ID [ NUMBER ]','id_list',4,'p_id_list','parser.py',132),
-  ('id_list -> id_list , ID [ NUMBER ]','id_list',6,'p_id_list','parser.py',133),
-  ('procedureBody -> programBlock','procedureBody',1,'p_procedureBody','parser.py',169),
-  ('procedureBody -> PROCEDURE MAIN ( ) { programBlock }','procedureBody',7,'p_procedureBody','parser.py',170),
-  ('programStatement -> qbitUnitaryStatement','programStatement',1,'p_statement','parser.py',178),
-  ('programStatement -> measureStatement','programStatement',1,'p_statement','parser.py',179),
-  ('programStatement -> foreachStatement','programStatement',1,'p_statement','parser.py',180),
-  ('programStatement -> ifStatement','programStatement',1,'p_statement','parser.py',181),
-  ('programBlock -> programStatement','programBlock',1,'p_programBlock','parser.py',184),
-  ('programBlock -> programBlock programStatement','programBlock',2,'p_programBlock','parser.py',185),
-  ('rangeExpr -> optionalIntExpr : optionalIntExpr','rangeExpr',3,'p_rangeExpr','parser.py',199),
-  ('rangeExpr -> optionalIntExpr : optionalIntExpr : optionalIntExpr','rangeExpr',5,'p_rangeExpr','parser.py',200),
-  ('optionalIntExpr -> intExpr','optionalIntExpr',1,'p_optionalIntExpr','parser.py',207),
-  ('optionalIntExpr -> emptyStatement','optionalIntExpr',1,'p_optionalIntExpr','parser.py',208),
-  ('sectionExpr -> intExpr','sectionExpr',1,'p_section','parser.py',218),
-  ('sectionExpr -> sectionExpr , intExpr','sectionExpr',3,'p_section','parser.py',219),
-  ('qubitExpr -> ID','qubitExpr',1,'p_qubitExpr','parser.py',231),
-  ('qubitExpr -> ID [ sectionExpr ]','qubitExpr',4,'p_qubitExpr','parser.py',232),
-  ('qubitExpr -> ID [ rangeExpr ]','qubitExpr',4,'p_qubitExpr','parser.py',233),
-  ('qubitListExpr -> qubitExpr','qubitListExpr',1,'p_qubitListExpr','parser.py',245),
-  ('qubitListExpr -> qubitListExpr , qubitExpr','qubitListExpr',3,'p_qubitListExpr','parser.py',246),
-  ('intExprAtom -> ID','intExprAtom',1,'p_intExprAtom','parser.py',265),
-  ('intExprAtom -> NUMBER','intExprAtom',1,'p_intExprAtom','parser.py',266),
-  ('intExprAtom -> ID [ intExpr ]','intExprAtom',4,'p_intExprAtom','parser.py',267),
-  ('intExprAtom -> ( intExpr )','intExprAtom',3,'p_intExprAtom','parser.py',268),
-  ('intExprTier1 -> intExprAtom','intExprTier1',1,'p_intTier1Expr','parser.py',309),
-  ('intExprTier1 -> intExprTier1 * intExprAtom','intExprTier1',3,'p_intTier1Expr','parser.py',310),
-  ('intExprTier1 -> intExprTier1 / intExprAtom','intExprTier1',3,'p_intTier1Expr','parser.py',311),
-  ('intExprTier1 -> intExprTier1 % intExprAtom','intExprTier1',3,'p_intTier1Expr','parser.py',312),
-  ('intExprTier2 -> intExprTier1','intExprTier2',1,'p_intTier2Expr','parser.py',320),
-  ('intExprTier2 -> intExprTier2 + intExprTier1','intExprTier2',3,'p_intTier2Expr','parser.py',321),
-  ('intExprTier2 -> intExprTier2 - intExprTier1','intExprTier2',3,'p_intTier2Expr','parser.py',322),
-  ('intExprTier2 -> <empty>','intExprTier2',0,'p_intTier2Expr','parser.py',323),
-  ('intExpr -> intExprTier2','intExpr',1,'p_term','parser.py',331),
-  ('intExpr -> - intExprTier2','intExpr',2,'p_term','parser.py',332),
-  ('foreachStatement -> FOR ID IN rangeExpr { programBlock }','foreachStatement',7,'p_foreachStatement','parser.py',344),
-  ('asso -> EQ','asso',1,'p_asso','parser.py',351),
-  ('asso -> GE','asso',1,'p_asso','parser.py',352),
-  ('asso -> LE','asso',1,'p_asso','parser.py',353),
-  ('asso -> NE','asso',1,'p_asso','parser.py',354),
-  ('asso -> <','asso',1,'p_asso','parser.py',355),
-  ('asso -> >','asso',1,'p_asso','parser.py',356),
-  ('ifStatement -> IF ( intExpr asso intExpr ) { programBlock }','ifStatement',9,'p_ifStatement','parser.py',361),
-  ('ifStatement -> IF ( intExpr asso intExpr ) { programBlock } ELSE { programBlock }','ifStatement',13,'p_ifStatement','parser.py',362),
-  ('qbitUnitaryStatement -> uGate < qubitListExpr > ;','qbitUnitaryStatement',5,'p_qbitUnitaryStatement','parser.py',369),
-  ('qbitUnitaryStatement -> uGate ( qubitListExpr ) ;','qbitUnitaryStatement',5,'p_qbitUnitaryStatement','parser.py',370),
-  ('qbitUnitaryStatement -> rGate < intExpr , qubitListExpr > ;','qbitUnitaryStatement',7,'p_qbitUnitaryStatement','parser.py',371),
-  ('qbitUnitaryStatement -> rGate ( intExpr , qubitListExpr ) ;','qbitUnitaryStatement',7,'p_qbitUnitaryStatement','parser.py',372),
-  ('qbitUnitaryStatement -> rxyGate ( intExpr , intExpr , qubitListExpr ) ;','qbitUnitaryStatement',9,'p_qbitUnitaryStatement','parser.py',373),
-  ('qbitUnitaryStatement -> rxyGate < intExpr , intExpr , qubitListExpr > ;','qbitUnitaryStatement',9,'p_qbitUnitaryStatement','parser.py',374),
-  ('rxyGate -> RXY','rxyGate',1,'p_rxyGate','parser.py',389),
-  ('rGate -> RX','rGate',1,'p_rGate','parser.py',393),
-  ('rGate -> RY','rGate',1,'p_rGate','parser.py',394),
-  ('rGate -> RZ','rGate',1,'p_rGate','parser.py',395),
-  ('uGate -> H','uGate',1,'p_uGate','parser.py',399),
-  ('uGate -> X','uGate',1,'p_uGate','parser.py',400),
-  ('uGate -> Y','uGate',1,'p_uGate','parser.py',401),
-  ('uGate -> Z','uGate',1,'p_uGate','parser.py',402),
-  ('uGate -> S','uGate',1,'p_uGate','parser.py',403),
-  ('uGate -> T','uGate',1,'p_uGate','parser.py',404),
-  ('uGate -> SD','uGate',1,'p_uGate','parser.py',405),
-  ('uGate -> TD','uGate',1,'p_uGate','parser.py',406),
-  ('uGate -> X2P','uGate',1,'p_uGate','parser.py',407),
-  ('uGate -> X2M','uGate',1,'p_uGate','parser.py',408),
-  ('uGate -> Y2P','uGate',1,'p_uGate','parser.py',409),
-  ('uGate -> Y2M','uGate',1,'p_uGate','parser.py',410),
-  ('uGate -> CZ','uGate',1,'p_uGate','parser.py',411),
-  ('uGate -> CNOT','uGate',1,'p_uGate','parser.py',412),
-  ('uGate -> CX','uGate',1,'p_uGate','parser.py',413),
-  ('uGate -> CY','uGate',1,'p_uGate','parser.py',414),
-  ('uGate -> ID','uGate',1,'p_uGate','parser.py',415),
-  ('measureStatement -> M < qubitExpr > ;','measureStatement',5,'p_measureStatement','parser.py',421),
-  ('measureStatement -> M ( qubitExpr ) ;','measureStatement',5,'p_measureStatement','parser.py',422),
-  ('emptyStatement -> <empty>','emptyStatement',0,'p_emptyStatement','parser.py',427),
+  ('program -> varDef procedureBody','program',2,'p_program','parser.py',34),
+  ('program -> gateDef varDef procedureBody','program',3,'p_program','parser.py',35),
+  ('gateDef -> gateDefclause','gateDef',1,'p_gateDef','parser.py',47),
+  ('gateDef -> gateDefclause gateDef','gateDef',2,'p_gateDef','parser.py',48),
+  ('gDefID -> ID','gDefID',1,'p_gDefID','parser.py',55),
+  ('gateDefclause -> DEFGATE gDefID = [ matrixContents ] ;','gateDefclause',7,'p_gateDefclause','parser.py',64),
+  ('matrixContents -> CNUMBER','matrixContents',1,'p_matrixContents','parser.py',69),
+  ('matrixContents -> CNUMBER , matrixContents','matrixContents',3,'p_matrixContents','parser.py',70),
+  ('matrixContents -> CNUMBER ; matrixContents','matrixContents',3,'p_matrixContents','parser.py',71),
+  ('CNUMBER -> NumberExpr','CNUMBER',1,'p_CNUMBER','parser.py',78),
+  ('CNUMBER -> - NumberExpr','CNUMBER',2,'p_CNUMBER','parser.py',79),
+  ('NumberExpr -> NUMBER','NumberExpr',1,'p_NumberExpr','parser.py',86),
+  ('NumberExpr -> NUMBER + NUMBER','NumberExpr',3,'p_NumberExpr','parser.py',87),
+  ('NumberExpr -> NUMBER - NUMBER','NumberExpr',3,'p_NumberExpr','parser.py',88),
+  ('varDef -> defclause','varDef',1,'p_varDef','parser.py',94),
+  ('varDef -> varDef defclause','varDef',2,'p_varDef','parser.py',95),
+  ('defclause -> QBIT seen_Qbit id_list ;','defclause',4,'p_defclause','parser.py',103),
+  ('defclause -> QCOUPLE id_list ;','defclause',3,'p_defclause','parser.py',104),
+  ('defclause -> VAR ID = NUMBER ;','defclause',5,'p_defclause','parser.py',105),
+  ('defclause -> VAR ID [ NUMBER ] = { matrixContents } ;','defclause',10,'p_defclause','parser.py',106),
+  ('seen_Qbit -> <empty>','seen_Qbit',0,'p_seen_Qbit','parser.py',120),
+  ('id_list -> ID','id_list',1,'p_id_list','parser.py',126),
+  ('id_list -> id_list , ID','id_list',3,'p_id_list','parser.py',127),
+  ('id_list -> ID [ NUMBER ]','id_list',4,'p_id_list','parser.py',128),
+  ('id_list -> id_list , ID [ NUMBER ]','id_list',6,'p_id_list','parser.py',129),
+  ('procedureBody -> programBlock','procedureBody',1,'p_procedureBody','parser.py',165),
+  ('procedureBody -> PROCEDURE MAIN ( ) { programBlock }','procedureBody',7,'p_procedureBody','parser.py',166),
+  ('programStatement -> qbitUnitaryStatement','programStatement',1,'p_statement','parser.py',174),
+  ('programStatement -> measureStatement','programStatement',1,'p_statement','parser.py',175),
+  ('programStatement -> foreachStatement','programStatement',1,'p_statement','parser.py',176),
+  ('programStatement -> ifStatement','programStatement',1,'p_statement','parser.py',177),
+  ('programBlock -> programStatement','programBlock',1,'p_programBlock','parser.py',180),
+  ('programBlock -> programBlock programStatement','programBlock',2,'p_programBlock','parser.py',181),
+  ('rangeExpr -> optionalIntExpr : optionalIntExpr','rangeExpr',3,'p_rangeExpr','parser.py',195),
+  ('rangeExpr -> optionalIntExpr : optionalIntExpr : optionalIntExpr','rangeExpr',5,'p_rangeExpr','parser.py',196),
+  ('optionalIntExpr -> intExpr','optionalIntExpr',1,'p_optionalIntExpr','parser.py',203),
+  ('optionalIntExpr -> emptyStatement','optionalIntExpr',1,'p_optionalIntExpr','parser.py',204),
+  ('sectionExpr -> intExpr','sectionExpr',1,'p_section','parser.py',214),
+  ('sectionExpr -> sectionExpr , intExpr','sectionExpr',3,'p_section','parser.py',215),
+  ('qubitExpr -> ID','qubitExpr',1,'p_qubitExpr','parser.py',227),
+  ('qubitExpr -> ID [ sectionExpr ]','qubitExpr',4,'p_qubitExpr','parser.py',228),
+  ('qubitExpr -> ID [ rangeExpr ]','qubitExpr',4,'p_qubitExpr','parser.py',229),
+  ('qubitListExpr -> qubitExpr','qubitListExpr',1,'p_qubitListExpr','parser.py',241),
+  ('qubitListExpr -> qubitListExpr , qubitExpr','qubitListExpr',3,'p_qubitListExpr','parser.py',242),
+  ('intExprAtom -> ID','intExprAtom',1,'p_intExprAtom','parser.py',261),
+  ('intExprAtom -> NUMBER','intExprAtom',1,'p_intExprAtom','parser.py',262),
+  ('intExprAtom -> ID [ intExpr ]','intExprAtom',4,'p_intExprAtom','parser.py',263),
+  ('intExprAtom -> ( intExpr )','intExprAtom',3,'p_intExprAtom','parser.py',264),
+  ('intExprTier1 -> intExprAtom','intExprTier1',1,'p_intTier1Expr','parser.py',305),
+  ('intExprTier1 -> intExprTier1 * intExprAtom','intExprTier1',3,'p_intTier1Expr','parser.py',306),
+  ('intExprTier1 -> intExprTier1 / intExprAtom','intExprTier1',3,'p_intTier1Expr','parser.py',307),
+  ('intExprTier1 -> intExprTier1 % intExprAtom','intExprTier1',3,'p_intTier1Expr','parser.py',308),
+  ('intExprTier2 -> intExprTier1','intExprTier2',1,'p_intTier2Expr','parser.py',316),
+  ('intExprTier2 -> intExprTier2 + intExprTier1','intExprTier2',3,'p_intTier2Expr','parser.py',317),
+  ('intExprTier2 -> intExprTier2 - intExprTier1','intExprTier2',3,'p_intTier2Expr','parser.py',318),
+  ('intExprTier2 -> <empty>','intExprTier2',0,'p_intTier2Expr','parser.py',319),
+  ('intExpr -> intExprTier2','intExpr',1,'p_term','parser.py',327),
+  ('intExpr -> - intExprTier2','intExpr',2,'p_term','parser.py',328),
+  ('foreachStatement -> FOR ID IN rangeExpr { programBlock }','foreachStatement',7,'p_foreachStatement','parser.py',340),
+  ('asso -> EQ','asso',1,'p_asso','parser.py',347),
+  ('asso -> GE','asso',1,'p_asso','parser.py',348),
+  ('asso -> LE','asso',1,'p_asso','parser.py',349),
+  ('asso -> NE','asso',1,'p_asso','parser.py',350),
+  ('asso -> <','asso',1,'p_asso','parser.py',351),
+  ('asso -> >','asso',1,'p_asso','parser.py',352),
+  ('ifStatement -> IF ( intExpr asso intExpr ) { programBlock }','ifStatement',9,'p_ifStatement','parser.py',357),
+  ('ifStatement -> IF ( intExpr asso intExpr ) { programBlock } ELSE { programBlock }','ifStatement',13,'p_ifStatement','parser.py',358),
+  ('qbitUnitaryStatement -> uGate < qubitListExpr > ;','qbitUnitaryStatement',5,'p_qbitUnitaryStatement','parser.py',365),
+  ('qbitUnitaryStatement -> uGate ( qubitListExpr ) ;','qbitUnitaryStatement',5,'p_qbitUnitaryStatement','parser.py',366),
+  ('qbitUnitaryStatement -> rGate < intExpr , qubitListExpr > ;','qbitUnitaryStatement',7,'p_qbitUnitaryStatement','parser.py',367),
+  ('qbitUnitaryStatement -> rGate ( intExpr , qubitListExpr ) ;','qbitUnitaryStatement',7,'p_qbitUnitaryStatement','parser.py',368),
+  ('qbitUnitaryStatement -> rxyGate ( intExpr , intExpr , qubitListExpr ) ;','qbitUnitaryStatement',9,'p_qbitUnitaryStatement','parser.py',369),
+  ('qbitUnitaryStatement -> rxyGate < intExpr , intExpr , qubitListExpr > ;','qbitUnitaryStatement',9,'p_qbitUnitaryStatement','parser.py',370),
+  ('rxyGate -> RXY','rxyGate',1,'p_rxyGate','parser.py',385),
+  ('rGate -> RX','rGate',1,'p_rGate','parser.py',389),
+  ('rGate -> RY','rGate',1,'p_rGate','parser.py',390),
+  ('rGate -> RZ','rGate',1,'p_rGate','parser.py',391),
+  ('uGate -> H','uGate',1,'p_uGate','parser.py',395),
+  ('uGate -> X','uGate',1,'p_uGate','parser.py',396),
+  ('uGate -> Y','uGate',1,'p_uGate','parser.py',397),
+  ('uGate -> Z','uGate',1,'p_uGate','parser.py',398),
+  ('uGate -> S','uGate',1,'p_uGate','parser.py',399),
+  ('uGate -> T','uGate',1,'p_uGate','parser.py',400),
+  ('uGate -> SD','uGate',1,'p_uGate','parser.py',401),
+  ('uGate -> TD','uGate',1,'p_uGate','parser.py',402),
+  ('uGate -> X2P','uGate',1,'p_uGate','parser.py',403),
+  ('uGate -> X2M','uGate',1,'p_uGate','parser.py',404),
+  ('uGate -> Y2P','uGate',1,'p_uGate','parser.py',405),
+  ('uGate -> Y2M','uGate',1,'p_uGate','parser.py',406),
+  ('uGate -> CZ','uGate',1,'p_uGate','parser.py',407),
+  ('uGate -> CNOT','uGate',1,'p_uGate','parser.py',408),
+  ('uGate -> CX','uGate',1,'p_uGate','parser.py',409),
+  ('uGate -> CY','uGate',1,'p_uGate','parser.py',410),
+  ('uGate -> ID','uGate',1,'p_uGate','parser.py',411),
+  ('measureStatement -> M < qubitExpr > ;','measureStatement',5,'p_measureStatement','parser.py',417),
+  ('measureStatement -> M ( qubitExpr ) ;','measureStatement',5,'p_measureStatement','parser.py',418),
+  ('emptyStatement -> <empty>','emptyStatement',0,'p_emptyStatement','parser.py',423),
 ]
```

### Comparing `isqopen-1.0.3/isq/compile/passes.py` & `isqopen-1.0.4/isq/compile/passes.py`

 * *Files 0% similar despite different names*

```diff
@@ -719,15 +719,15 @@
         else:
             qid = q[0]
             offset = q[1]
         index = self.qDic.get(qid)
         if(index==None):
             ICE("bad variable")
         index += offset
-        return "Q{:0>2d}".format(index+1)
+        return "Q{:0>2d}".format(index)
 
     def get_qop(self, gate, qbit, param, pos):
         
         if self.target == 'openqasm':
             if gate == 'RXY':
                 ErrorThrow(f'openqasm can not support RXY, please decompose first')
             s = self.openqasm_gate[gate]
@@ -735,20 +735,20 @@
                 s += f' q[{int(qbit[0])}] -> c[{self.m_cnt}]'
                 self.m_cnt += 1
             else:
                 if gate in ['RX', 'RY', 'RZ']:
                     s += f'({param[0]})'
                 
                 if gate in ['CNOT', 'CX', 'CY', 'CZ']:
-                    s += f' q[{int(qbit[0])-1}], q[{int(qbit[1])-1}]'
+                    s += f' q[{int(qbit[0])}], q[{int(qbit[1])}]'
                 else:
-                    s += f' q[{int(qbit[0])-1}]'
+                    s += f' q[{int(qbit[0])}]'
             return s+';'
         else:
-            qbit = [str(int(q)+1) for q in qbit]
+            qbit = [str(int(q)) for q in qbit]
             s = gate
             if gate in ['CNOT', 'CX', 'CY', 'CZ']:
                 if self.hardware:
                     if (qbit[0] not in self.topo) or (qbit[1] not in self.topo[qbit[0]]):
                         ErrorThrow("in line {}, CZ can only operate adjacent qubit. [{}, {}] not adjacent\n".format(pos, qbit[0], qbit[1]))
                 s = f"{gate} Q{qbit[0]} Q{qbit[1]}"
             else:
```

### Comparing `isqopen-1.0.3/isq/compile/qtypes.py` & `isqopen-1.0.4/isq/compile/qtypes.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/compile/tokrules.py` & `isqopen-1.0.4/isq/compile/tokrules.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/compile/tools.py` & `isqopen-1.0.4/isq/compile/tools.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/device/device.py` & `isqopen-1.0.4/isq/device/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,16 +126,14 @@
         
     def probs(self, isq_str = '', file = None, mod = 0, **kwargs):
         
         args = self.compile_with_par(isq_str, file, "isq", **kwargs)
         
         return getprobs(self._ir, mod, **args)
 
-        
-
 
 class QcisDevice(Device):
 
     def __init__(
         self,
         login_key = None,
         machine_name = None,
```

### Comparing `isqopen-1.0.3/isq/device/grad.py` & `isqopen-1.0.4/isq/device/grad.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/device/task.py` & `isqopen-1.0.4/isq/device/task.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/device/translate.py` & `isqopen-1.0.4/isq/device/translate.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/draw/drawer.py` & `isqopen-1.0.4/isq/draw/drawer.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/errors.py` & `isqopen-1.0.4/isq/errors.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/globalVar.py` & `isqopen-1.0.4/isq/globalVar.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/mapping.py` & `isqopen-1.0.4/isq/mapping.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/quantum.py` & `isqopen-1.0.4/isq/quantum.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/simulate/operation.py` & `isqopen-1.0.4/isq/simulate/operation.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isq/simulate/simulator.py` & `isqopen-1.0.4/isq/simulate/simulator.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/isqopen.egg-info/PKG-INFO` & `isqopen-1.0.4/isqopen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isqopen
-Version: 1.0.3
+Version: 1.0.4
 Summary: isq quantum kernel
 Author: Lou Huazhe
 Author-email: louhz@arclightquantum.com
 Platform: python 3.8+
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `isqopen-1.0.3/isqopen.egg-info/SOURCES.txt` & `isqopen-1.0.4/isqopen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.3/setup.py` & `isqopen-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "isqopen",
-    version = "1.0.3",
+    version = "1.0.4",
     keyword = {"isq", "quantum", "cor"},
     description = "isq quantum kernel",
     platforms='python 3.8+',
     long_description=long_description,
 	long_description_content_type="text/markdown",
     author = "Lou Huazhe",
     author_email = "louhz@arclightquantum.com",
```

