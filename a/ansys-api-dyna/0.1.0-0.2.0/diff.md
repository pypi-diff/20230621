# Comparing `tmp/ansys-api-dyna-0.1.0.tar.gz` & `tmp/ansys-api-dyna-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-dyna-0.1.0.tar", last modified: Tue Jun 20 12:12:36 2023, max compression
+gzip compressed data, was "ansys-api-dyna-0.2.0.tar", last modified: Wed Jun 21 06:09:05 2023, max compression
```

## Comparing `ansys-api-dyna-0.1.0.tar` & `ansys-api-dyna-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:12:36.151444 ansys-api-dyna-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-20 12:12:18.000000 ansys-api-dyna-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-20 12:12:36.151444 ansys-api-dyna-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-20 12:12:18.000000 ansys-api-dyna-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-20 12:12:18.000000 ansys-api-dyna-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 12:12:36.151444 ansys-api-dyna-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-20 12:12:18.000000 ansys-api-dyna-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:12:36.151444 ansys-api-dyna-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:12:36.151444 ansys-api-dyna-0.1.0/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:12:36.151444 ansys-api-dyna-0.1.0/src/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:12:36.151444 ansys-api-dyna-0.1.0/src/ansys/api/dyna/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 12:12:18.000000 ansys-api-dyna-0.1.0/src/ansys/api/dyna/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-20 12:12:18.000000 ansys-api-dyna-0.1.0/src/ansys/api/dyna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:12:18.000000 ansys-api-dyna-0.1.0/src/ansys/api/dyna/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:12:36.151444 ansys-api-dyna-0.1.0/src/ansys/api/dyna/v0/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-20 12:12:18.000000 ansys-api-dyna-0.1.0/src/ansys/api/dyna/v0/dynasolver.proto
--rw-r--r--   0 runner    (1001) docker     (123)    40512 2023-06-20 12:12:18.000000 ansys-api-dyna-0.1.0/src/ansys/api/dyna/v0/kwprocess.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:12:36.151444 ansys-api-dyna-0.1.0/src/ansys_api_dyna.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-20 12:12:36.000000 ansys-api-dyna-0.1.0/src/ansys_api_dyna.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-20 12:12:36.000000 ansys-api-dyna-0.1.0/src/ansys_api_dyna.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:12:36.000000 ansys-api-dyna-0.1.0/src/ansys_api_dyna.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-20 12:12:36.000000 ansys-api-dyna-0.1.0/src/ansys_api_dyna.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 12:12:36.000000 ansys-api-dyna-0.1.0/src/ansys_api_dyna.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 12:12:36.000000 ansys-api-dyna-0.1.0/src/ansys_api_dyna.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.707717 ansys-api-dyna-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-21 06:09:05.707717 ansys-api-dyna-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 06:09:05.707717 ansys-api-dyna-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.703717 ansys-api-dyna-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.703717 ansys-api-dyna-0.2.0/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.703717 ansys-api-dyna-0.2.0/src/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.703717 ansys-api-dyna-0.2.0/src/ansys/api/dyna/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/src/ansys/api/dyna/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/src/ansys/api/dyna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/src/ansys/api/dyna/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.703717 ansys-api-dyna-0.2.0/src/ansys/api/dyna/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/src/ansys/api/dyna/v0/dynasolver.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    42399 2023-06-21 06:08:43.000000 ansys-api-dyna-0.2.0/src/ansys/api/dyna/v0/kwprocess.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:09:05.707717 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-21 06:09:05.000000 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-21 06:09:05.000000 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 06:09:05.000000 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 06:09:05.000000 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 06:09:05.000000 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 06:09:05.000000 ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/top_level.txt
```

### Comparing `ansys-api-dyna-0.1.0/LICENSE` & `ansys-api-dyna-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-dyna-0.1.0/PKG-INFO` & `ansys-api-dyna-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-dyna
-Version: 0.1.0
-Summary: Autogenerated python gRPC interface package for ansys-api-dyna, built on 12:12:36 on 20 June 2023
+Version: 0.2.0
+Summary: Autogenerated python gRPC interface package for ansys-api-dyna, built on 06:09:05 on 21 June 2023
 Home-page: https://github.com/ansys/ansys-api-dyna
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-dyna-0.1.0/README.md` & `ansys-api-dyna-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-dyna-0.1.0/setup.py` & `ansys-api-dyna-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-api-dyna-0.1.0/src/ansys/api/dyna/v0/dynasolver.proto` & `ansys-api-dyna-0.2.0/src/ansys/api/dyna/v0/dynasolver.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-dyna-0.1.0/src/ansys/api/dyna/v0/kwprocess.proto` & `ansys-api-dyna-0.2.0/src/ansys/api/dyna/v0/kwprocess.proto`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,29 @@
 	string url = 1;
 }
 
 message kwFileNameReply {
 	bool ret = 1;
 }
 
+message IncludeTransformRequest {
+	string filename = 1;
+	int32 idnoff = 2;
+	int32 ideoff = 3;
+	int32 idpoff = 4;
+	int32 idmoff = 5;
+	int32 idsoff = 6;
+	int32 idfoff = 7;
+	int32 tranid = 8;
+}
+
+message IncludeTransformReply {
+	int32 answer = 1;
+}
+
 //---control_* card
 message TimestepRequest {
 	float tssfac = 1;
     int32 isdo = 2;
 	float dt2ms = 3;
 	int32 lctm = 4;
 }
@@ -690,27 +705,45 @@
 	float zh = 8;
 }
 
 message DefineVectorReply {
 	int32 answer = 1;
 }
 
+message DefineFunctionRequest {
+	string function = 1;
+}
+
+message DefineFunctionReply {
+	int32 id = 1;
+}
+
 message DefineBoxRequest {
 	float xmin = 1;
 	float xmax = 2;
 	float ymin = 3;
 	float ymax = 4;
 	float zmin = 5;
 	float zmax = 6;
 }
 
 message DefineBoxReply {
 	int32 boxid = 1;
 }
 
+message DefineTransformationRequest {
+    int32 tranid = 1;
+	repeated string option = 2;
+	repeated float param = 3;
+}
+
+message DefineTransformationReply {
+	int32 id = 1;
+}
+
 message DefineDEMeshSurfaceRequest {
     int32 sid = 1;
 	int32 type = 2;
 	int32 nquad = 3;
 	int32 despid = 4;
 	int32 desxid = 5;
 	int32 nsid = 6;
@@ -1143,14 +1176,15 @@
 
 message SaveFileRequest {
 	string name = 1;
 }
 
 message SaveFileReply {
 	int64 length = 1;
+	string outpath = 2;
 }
 
 message LoadFileRequest {
 	string name = 1;
 }
 
 message LoadFileReply {
@@ -1619,16 +1653,17 @@
 }
 
 //---EM
 message EMControlRequest {
     int32 emsol = 1;
 	int32 numls = 2;
 	float macrodt = 3;
-	int32 ncylfem = 4;
-	int32 ncylbem = 5;
+	int32 dimtype = 4;
+	int32 ncylfem = 5;
+	int32 ncylbem = 6;
 }
 
 message EMControlReply {
 	int32 answer = 1;
 }
 
 message EMTimestepRequest {
@@ -1691,14 +1726,15 @@
 	int32 id = 1;
 }
 
 message EMMat001Request {
     int32 mid = 1;
 	int32 mtype = 2;
 	float sigma = 3;
+	int32 eosid = 4;
 }
 
 message EMMat001Reply {
 	int32 answer = 1;
 }
 
 message EMMat002Request {
@@ -1709,14 +1745,61 @@
 	float murel = 5;
 }
 
 message EMMat002Reply {
 	int32 answer = 1;
 }
 
+message EMMat004Request {
+    int32 mid = 1;
+	int32 mtype = 2;
+	float sigma = 3;
+}
+
+message EMMat004Reply {
+	int32 answer = 1;
+}
+
+message EMIsopotentialRequest {
+    int32 isoid = 1;
+	int32 settype = 2;
+	int32 setid = 3;
+}
+
+message EMIsopotentialReply {
+	int32 id = 1;
+}
+
+message EMIsopotentialConnectRequest {
+    int32 conid = 1;
+	int32 contype = 2;
+	int32 isoid1 = 3;
+	int32 isoid2 = 4;
+	float val = 5;
+	int32 lcid = 6;
+	//contype==6
+	float l = 7;
+	float c = 8;
+    float v0 = 9;
+}
+
+message EMIsopotentialConnectReply {
+	int32 id = 1;
+}
+
+message EMIsopotentialRogoRequest {
+    int32 isoid = 1;
+	int32 settype = 2;
+	int32 setid = 3;
+}
+
+message EMIsopotentialRogoReply {
+	int32 id = 1;
+}
+
 message EMSolverBemRequest {
     float reltol = 1;
 	int32 maxite = 2;
 	int32 stype = 3;
 	int32 precon = 4;
 	int32 uselast = 5;
 	int32 ncylbem = 6;
@@ -1845,14 +1928,15 @@
 message GeneralKWDReply {
 	int32 answer = 1;
 }
 
 service kwC2S {
 	rpc kwSetFileName(kwFileName) returns(kwFileNameReply) {}
 	rpc Upload(stream Chunk) returns (kwFileReply) {}
+	rpc CreateIncludeTransform(IncludeTransformRequest) returns (IncludeTransformReply) {}
 	//---CONTROL
 	rpc CreateTimestep(TimestepRequest) returns (TimestepReply) {}
 	rpc CreateTermination(TerminationRequest) returns (TerminationReply) {}
 	rpc CreateControlOutput(ControlOutputRequest) returns (ControlOutputReply) {}
 	rpc CreateControlContact(ControlContactRequest) returns (ControlContactReply) {}
 	rpc CreateControlDiscreteElement(ControlDiscreteElementRequest) returns (ControlDiscreteElementReply) {}
 	rpc CreateControlAccuracy(ControlAccuracyRequest) returns (ControlAccuracyReply) {}
@@ -1931,15 +2015,17 @@
 	rpc CreateEOSGruneisen(EOSGruneisenRequest) returns (EOSGruneisenReply) {}
 
 	
 	//---DEFINE
 	rpc CreateDefineCurve(DefineCurveRequest) returns (DefineCurveReply) {}
 	rpc CreateDefineCurveFunction(DefineCurveFunctionRequest) returns (DefineCurveFunctionReply) {}
 	rpc CreateDefineVector(DefineVectorRequest) returns (DefineVectorReply) {}
+	rpc CreateDefineFunction(DefineFunctionRequest) returns (DefineFunctionReply) {}
 	rpc CreateDefineBox(DefineBoxRequest) returns (DefineBoxReply) {}
+	rpc CreateDefineTransformation(DefineTransformationRequest) returns (DefineTransformationReply) {}
 	rpc CreateDefineDEMeshSurface(DefineDEMeshSurfaceRequest) returns (DefineDEMeshSurfaceReply) {}
 	rpc CreateDefineOrientation(DefineOrientationRequest) returns (DefineOrientationReply) {}
 	rpc CreateDefineSPHMassflowPlane(DefineSPHMassflowPlaneRequest) returns (DefineSPHMassflowPlaneReply) {}
     rpc CreateDefineSPHMeshBox(DefineSPHMeshBoxRequest) returns (DefineSPHMeshBoxReply) {}
     rpc CreateDefineSPHMeshSurface(DefineSPHMeshSurfaceRequest) returns (DefineSPHMeshSurfaceReply) {}
 
 	rpc CreatePartSet(PartSetRequest) returns (PartSetReply) {}
@@ -2021,14 +2107,18 @@
     rpc CreateEMTimestep(EMTimestepRequest) returns (EMTimestepReply) {}
 	rpc CreateEMControlContact(EMControlContactRequest) returns (EMControlContactReply) {}
 	rpc CreateEMContact(EMContactRequest) returns (EMContactReply) {}
 	rpc CreateEMCircuitRogo(EMCircuitRogoRequest) returns (EMCircuitRogoReply) {}
 	rpc CreateEMCircuit(EMCircuitRequest) returns (EMCircuitReply) {}
 	rpc CreateEMMat001(EMMat001Request) returns (EMMat001Reply) {}
 	rpc CreateEMMat002(EMMat002Request) returns (EMMat002Reply) {}
+	rpc CreateEMMat004(EMMat004Request) returns (EMMat004Reply) {}
+	rpc CreateEMIsopotential(EMIsopotentialRequest) returns (EMIsopotentialReply) {}
+	rpc CreateEMIsopotentialConnect(EMIsopotentialConnectRequest) returns (EMIsopotentialConnectReply) {}
+	rpc CreateEMIsopotentialRogo(EMIsopotentialRogoRequest) returns (EMIsopotentialRogoReply) {}
 	rpc CreateEMSolverBem(EMSolverBemRequest) returns (EMSolverBemReply) {}
 	rpc CreateEMSolverFem(EMSolverFemRequest) returns (EMSolverFemReply) {}
 	rpc CreateEMSolverBemMat(EMSolverBemMatRequest) returns (EMSolverBemMatReply) {}
 	rpc CreateEMSolverFemBemMonolithic(EMSolverFemBemMonolithicRequest) returns (EMSolverFemBemMonolithicReply) {}
 	rpc CreateEMOutput(EMOutputRequest) returns (EMOutputReply) {}
 	rpc CreateEMDatabaseGlobalEnergy(EMDatabaseGlobalEnergyRequest) returns (EMDatabaseGlobalEnergyReply) {}
 	rpc CreateEMPermanentMagnet(EMPermanentMagnetRequest) returns (EMPermanentMagnetReply) {}
```

### Comparing `ansys-api-dyna-0.1.0/src/ansys_api_dyna.egg-info/PKG-INFO` & `ansys-api-dyna-0.2.0/src/ansys_api_dyna.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-dyna
-Version: 0.1.0
-Summary: Autogenerated python gRPC interface package for ansys-api-dyna, built on 12:12:36 on 20 June 2023
+Version: 0.2.0
+Summary: Autogenerated python gRPC interface package for ansys-api-dyna, built on 06:09:05 on 21 June 2023
 Home-page: https://github.com/ansys/ansys-api-dyna
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

