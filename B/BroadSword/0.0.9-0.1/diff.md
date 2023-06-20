# Comparing `tmp/BroadSword-0.0.9.tar.gz` & `tmp/BroadSword-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BroadSword-0.0.9.tar", last modified: Wed Jun  7 16:46:52 2023, max compression
+gzip compressed data, was "BroadSword-0.1.tar", last modified: Tue Jun  6 17:57:37 2023, max compression
```

## Comparing `BroadSword-0.0.9.tar` & `BroadSword-0.1.tar`

### file list

```diff
@@ -1,20 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:46:52.292773 BroadSword-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-07 16:46:42.000000 BroadSword-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-07 16:46:52.292773 BroadSword-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-07 16:46:42.000000 BroadSword-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 16:46:42.000000 BroadSword-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-07 16:46:52.292773 BroadSword-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:46:52.288773 BroadSword-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:46:52.292773 BroadSword-0.0.9/src/BroadSword/
--rw-r--r--   0 runner    (1001) docker     (123)    16658 2023-06-07 16:46:42.000000 BroadSword-0.0.9/src/BroadSword/BroadSword.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:46:42.000000 BroadSword-0.0.9/src/BroadSword/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33566 2023-06-07 16:46:42.000000 BroadSword-0.0.9/src/BroadSword/libmatrices.dylib
--rwxr-xr-x   0 runner    (1001) docker     (123)    20496 2023-06-07 16:46:42.000000 BroadSword-0.0.9/src/BroadSword/libmatrices.so
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-06-07 16:46:42.000000 BroadSword-0.0.9/src/BroadSword/matrices.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:46:52.292773 BroadSword-0.0.9/src/BroadSword.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-07 16:46:52.000000 BroadSword-0.0.9/src/BroadSword.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-07 16:46:52.000000 BroadSword-0.0.9/src/BroadSword.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:46:52.000000 BroadSword-0.0.9/src/BroadSword.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 16:46:52.000000 BroadSword-0.0.9/src/BroadSword.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 16:46:52.000000 BroadSword-0.0.9/src/BroadSword.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:46:52.000000 BroadSword-0.0.9/src/BroadSword.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:37.360304 BroadSword-0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-06 17:57:16.000000 BroadSword-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-06 17:57:37.360304 BroadSword-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 17:57:16.000000 BroadSword-0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 17:57:16.000000 BroadSword-0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-06 17:57:37.360304 BroadSword-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:37.360304 BroadSword-0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:37.360304 BroadSword-0.1/src/BroadSword/
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-06-06 17:57:16.000000 BroadSword-0.1/src/BroadSword/BroadSword.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:57:16.000000 BroadSword-0.1/src/BroadSword/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:37.360304 BroadSword-0.1/src/BroadSword.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/top_level.txt
```

### Comparing `BroadSword-0.0.9/LICENSE` & `BroadSword-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BroadSword-0.0.9/setup.cfg` & `BroadSword-0.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 [metadata]
 name = BroadSword
-version = 0.0.9
+version = 0.1
 author = Cody Somers
 author_email = cas003@usask.ca
 description = Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Cody-Somers/BroadSword
 project_urls = 
 	Beamline Information = https://reixs.lightsource.ca
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
-zip_safe = True
-include_package_data = True
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
+	ctypes
 	numpy
 	pandas
 	bokeh>=2.3.3,<3
 
 [options.packages.find]
 where = src
 
-[options.package_data]
-BroadSword = *.so, *.dylib, *.c
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `BroadSword-0.0.9/src/BroadSword/BroadSword.py` & `BroadSword-0.1/src/BroadSword/BroadSword.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import ctypes as C
 from ctypes import *
-import os
 import numpy as np
 import numpy.ctypeslib as npc
 import pandas as pd
+from reixs.LoadData import *
 
 
 # These are the input and output spectra of type float
 # ['Column'] = [0=Energy, 1=Counts]
 # ['Column'] = [0=Energy, 1=Counts, 2=CoreLifeXAS, 3=Intermediate Step, 4=Delta E, 5=Intermediate Step, 6=Final Gaussian Counts]
 # ['Row'] = data
 # ['XES, XANES'] = [0=XES, 1=XANES]
@@ -43,33 +43,30 @@
 # Misc
 bandshift = np.zeros([40,40])
 bands_temp = np.zeros([3500,40,40])
 bands_temp_count = np.zeros([40,40],dtype=int)
 BandGap = 0
 
 class Broaden():
-    """
-    Class to take in data and broaden it.
+    """Class to take in data and broaden it.
     We have to load the experimental, and then load the calculations. With the calculations we can load multiple different sets of files
     so that we account for the different sites that can exist. Just call the loadCalc function multiple times and it should account for the diffent sites.
     """
 
     def __init__(self):
-        self.data = list() # Why is this here?
+        self.data = list()
 
-    def loadExp(self, basedir, XES, XANES, fermi):
+    def loadExp(self, basedir, XES, XANES):
         """
         Parameters
         ----------
         basedir : string
             Specifiy the absolute or relative path to experimental data.
         XES, XANES : string
             Specify the file name (ASCII).
-        fermi : float
-            Specify the fermi energy for the ground state calculated spectra
         """
 
         with open(basedir+"/"+XES, "r") as xesFile:
             df = pd.read_csv(xesFile, delimiter='\s+',header=None) # Change to '\s*' and specify engine='python' if this breaks in jupyter notebook
             c1 = 0
             for i in range(len(df)): 
                 ExpSXS[0][c1][0] = df[0][c1] # Energy
@@ -81,35 +78,24 @@
             df = pd.read_csv(xanesFile, delimiter='\s+',header=None)
             c1 = 0
             for i in range(len(df)):
                 ExpSXS[0][c1][1] = df[0][c1] # Energy
                 ExpSXS[1][c1][1] = df[1][c1] # Counts
                 c1 += 1
             ExpSXSCount[1] = c1 # Length
-        
-        global CalcSXSCase
-        global Fermi
-        CalcSXSCase = 0
-        Fermi = fermi
         return
 
-    def loadCalc(self, basedir, XES, XAS, XANES, fermis, binds, edge="K", sites=1):
+    def loadCalc(self, basedir, XES, XAS, XANES, sites=1):
         """
         Parameters
         ----------
         basedir : string
             Specifiy the absolute or relative path to experimental data.
         XES, XAS, XANES : string
             Specify the file name (.txspec).
-        fermis : float
-            Specify the fermi energy for the excited state calculation
-        bind : float
-            Specify the binding energy of the ground state
-        edge : string
-            Specify the excitation edge "K","L2","L3","M4","M5"
         """
         global CalcSXSCase
         global Site
 
         with open(basedir+"/"+XES, "r") as xesFile:
             df = pd.read_csv(xesFile, delimiter='\s+',header=None)
             c1 = 0
@@ -133,18 +119,14 @@
             c1 = 0
             for i in range(len(df)):
                 CalcSXS[0][c1][2][CalcSXSCase] = df[0][c1] # Energy
                 CalcSXS[1][c1][2][CalcSXSCase] = df[1][c1] # Counts
                 c1 += 1
             CalcSXSCount[2][CalcSXSCase] = c1 # Length for each Site
 
-        # Update the global variables with the parameters for that site.
-        Fermis[CalcSXSCase] = fermis
-        Binds[CalcSXSCase] = binds
-        Edge[CalcSXSCase] = edge
         Site[CalcSXSCase] = sites
         CalcSXSCase += 1
         return
 
     def FindBands(self): # Perhaps change the while loops to for in range()
         c1 = 0
         while c1 < CalcSXSCase: # For each site (.loadCalc)
@@ -273,15 +255,15 @@
                 for c2 in range(BroadSXSCount[c3][c1]):
                     BroadSXS[1][c2][c3][c1] = BroadSXS[1][c2][c3][c1]*(BroadSXS[0][c2][c3][c1]/Econ)
         global BandGap
         BandGap = Econ - Eval
         print(BandGap)
         return
 
-    def broaden(self, libpath="./"):
+    def broaden(self):
         Econd = np.zeros(40)
         type = False
         energy_0 = 20
 
         if XESscale != 0:
             for c1 in range(CalcSXSCase):
                 for c2 in range(BandNum[c1]):
@@ -325,20 +307,15 @@
                         type = False
                         c3 += 1
                         if c3 > BandNum[c1]:
                             c3 = BandNum[c1]-1
                     else:
                         BroadSXS[2][c2][0][c1] = scaleXES[c1][c3]/100 * ((BroadSXS[0][c2][0][c1]-Econd[c1]) * (BroadSXS[0][c2][0][c1]-Econd[c1])) + corelifeXES
 
-        #mylib = cdll.LoadLibrary('./libmatrices.so')
-        try:
-            mylib = cdll.LoadLibrary(libpath + "libmatrices.so")
-        except:
-            mylib = cdll.LoadLibrary(libpath + "libmatrices.dylib")
-        
+        mylib = cdll.LoadLibrary('./libmatrices.so')
         cCalcSXSCase = C.c_int(CalcSXSCase)
 
         cBroadSXSCount = (C.c_int*40*3)()
         for c1 in range(3):
             for c2 in range(40):
                 cBroadSXSCount[c1][c2] = BroadSXSCount[c1][c2]
         
@@ -353,14 +330,39 @@
         cdisord = C.c_float(disord)
         print(BroadSXS[0][2000][1][0])
         print(BroadSXS[1][2000][1][0])
         mylib.broadXAS(cCalcSXSCase,cBroadSXSCount,BroadSXS,cdisord)
         print(BroadSXS[6][2000][1][0])
         return
 
+    def initParam(self, fermi, fermis, binds, edge):
+        """
+        Parameters
+        ----------
+        fermi : float
+            Specify the fermi energy for the ground state spectra
+        fermis : [float] A list of floats
+            Specify the fermi energy for all of the excited state calculations
+        bind : [float] A list of floats
+            Specify the binding energy of the ground states for each site
+        edge : [String] A list of strings
+            Specify the excitation edges
+        """
+        global Fermi
+        global Fermis
+        global Binds
+        global Edge
+        Fermi = fermi
+        Fermis = fermis # Might have to change this so that you keep the size of the arrays the same.
+        Binds = binds
+        Edge = edge
+        #TODO, put these parameters into loadCalc preferably. Same way that sites is being done
+
+        return
+
     def initResolution(self, XEScorelife, specResolution, monoResolution, disorder, XESscaling, XASscaling):
         """
         Parameters
         ----------
         XEScorelife : float
             Specify the corehole lifetime broadening factor
         specResolution : float
@@ -385,11 +387,7 @@
         corelifeXAS = XEScorelife
         spec = specResolution
         mono = monoResolution
         disord = disorder
         XESscale = XESscaling
         scaleXAS = XASscaling
         return
-    
-    def add(self):
-        # TODO: Need to add this function from original c file.
-        return
```

