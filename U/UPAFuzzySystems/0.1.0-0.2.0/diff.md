# Comparing `tmp/UPAFuzzySystems-0.1.0.tar.gz` & `tmp/UPAFuzzySystems-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UPAFuzzySystems-0.1.0.tar", last modified: Tue Nov  8 15:53:54 2022, max compression
+gzip compressed data, was "UPAFuzzySystems-0.2.0.tar", last modified: Thu Jan 12 16:01:51 2023, max compression
```

## Comparing `UPAFuzzySystems-0.1.0.tar` & `UPAFuzzySystems-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-11-08 15:53:54.627323 UPAFuzzySystems-0.1.0/
--rw-rw-rw-   0        0        0     1099 2022-10-29 19:07:07.000000 UPAFuzzySystems-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1098 2022-11-08 15:53:54.626322 UPAFuzzySystems-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      617 2022-11-03 22:04:19.000000 UPAFuzzySystems-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-08 15:53:54.617336 UPAFuzzySystems-0.1.0/UPAFuzzySystems/
--rw-rw-rw-   0        0        0    32554 2022-11-08 15:43:09.000000 UPAFuzzySystems-0.1.0/UPAFuzzySystems/UPAFuzzySystems.py
--rw-rw-rw-   0        0        0      286 2022-11-03 19:51:00.000000 UPAFuzzySystems-0.1.0/UPAFuzzySystems/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-08 15:53:54.624322 UPAFuzzySystems-0.1.0/UPAFuzzySystems.egg-info/
--rw-rw-rw-   0        0        0     1098 2022-11-08 15:53:54.000000 UPAFuzzySystems-0.1.0/UPAFuzzySystems.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2022-11-08 15:53:54.000000 UPAFuzzySystems-0.1.0/UPAFuzzySystems.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-08 15:53:54.000000 UPAFuzzySystems-0.1.0/UPAFuzzySystems.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2022-11-08 15:53:54.000000 UPAFuzzySystems-0.1.0/UPAFuzzySystems.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-11-08 15:53:54.000000 UPAFuzzySystems-0.1.0/UPAFuzzySystems.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-08 15:53:54.630330 UPAFuzzySystems-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1462 2022-11-08 15:53:22.000000 UPAFuzzySystems-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:01:50.996456 UPAFuzzySystems-0.2.0/
+-rw-rw-rw-   0        0        0     1099 2022-10-29 19:07:07.000000 UPAFuzzySystems-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1073 2023-01-12 16:01:50.995463 UPAFuzzySystems-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2023-01-12 15:06:46.000000 UPAFuzzySystems-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-01-12 16:01:50.965539 UPAFuzzySystems-0.2.0/UPAFuzzySystems/
+-rw-rw-rw-   0        0        0    34230 2023-01-10 21:49:58.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems/UPAFuzzySystems.py
+-rw-rw-rw-   0        0        0      286 2022-11-03 19:51:00.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:01:50.993463 UPAFuzzySystems-0.2.0/UPAFuzzySystems.egg-info/
+-rw-rw-rw-   0        0        0     1073 2023-01-12 16:01:50.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-01-12 16:01:50.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-12 16:01:50.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-01-12 16:01:50.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-01-12 16:01:50.000000 UPAFuzzySystems-0.2.0/UPAFuzzySystems.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-01-12 16:01:50.996456 UPAFuzzySystems-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1462 2023-01-12 15:56:10.000000 UPAFuzzySystems-0.2.0/setup.py
```

### Comparing `UPAFuzzySystems-0.1.0/LICENSE` & `UPAFuzzySystems-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `UPAFuzzySystems-0.1.0/PKG-INFO` & `UPAFuzzySystems-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: UPAFuzzySystems
-Version: 0.1.0
+Version: 0.2.0
 Summary: UPAFuzzySystems package for definition and simulation of Fuzzy Inference Systems for general and control applications.
 Home-page: https://github.com/UniversidadPolitecnicaAguascalientes/UPAFuzzySystems/
 Author: Dr. Martin Montes Rivera (Universidad Politécnica de Aguascalientes)
 Author-email: <martin.montes@upa.edu.mx>
-License: UNKNOWN
-Description: UPAFuzzySystems library allows defining Fuzzy Inference Systems for different applications with continuous and discrete universes, it also deploys structures for simulation of fuzzy control with transfer functions and state space models.
 Keywords: python,fuzzy logic,fuzzy control,fuzzy inference systems,artificial intelligence
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+UPAFuzzySystems library allows defining Fuzzy Inference Systems for different applications with continuous and discrete universes, it also deploys structures for simulation of fuzzy control with transfer functions and state space models.
```

### Comparing `UPAFuzzySystems-0.1.0/UPAFuzzySystems/UPAFuzzySystems.py` & `UPAFuzzySystems-0.2.0/UPAFuzzySystems/UPAFuzzySystems.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 
 from skfuzzy import defuzz, trapmf, trimf, trimf, gaussmf, gbellmf
-from numpy import array, arange, matrix, meshgrid, linspace, radians, fmin, fmax, max, zeros, minimum, maximum, isscalar, sum, prod
+from numpy import array, arange, matrix, meshgrid, linspace, radians, fmin, fmax, max, zeros, minimum, maximum, isscalar, sum, prod, multiply, repeat
 import matplotlib.pyplot as plt
 from control import NonlinearIOSystem, sample_system, InterconnectedSystem, LinearIOSystem, tf2ss, tfdata
 
 
 class fuzzy_universe():
     """Create a Universe Discrete or Continuous for Describe Inputs and Outputs in an 
     inference system.
@@ -67,15 +67,18 @@
         Returns:
             fuzzy_set (dict): Dictionary containing universe and membership values of the fuzzy set.
         """
         membershipvalues=[]
         X = self.structure['universe']
         membershipfuntion = self.structure[name][0]
         vertices = self.structure[name][1]
-        exec('membershipvalues.append('+membershipfuntion+'(X,'+str(vertices)+'))')
+        if membershipfuntion =='gaussmf':
+            exec('membershipvalues.append('+membershipfuntion+'(X,'+str(vertices[0])+','+str(vertices[1])+'))')
+        else:
+            exec('membershipvalues.append('+membershipfuntion+'(X,'+str(vertices)+'))')
         return {'universe':X,'membership values':membershipvalues[0]}
     def view_fuzzy(self):
 
         """Plots the the corresponding universe with all its fuzzy sets.
         
 
         Args:
@@ -310,24 +313,24 @@
         if isinstance(input_val, list):
             input_val = array(input_val).reshape(len(input_val),)
         if isscalar(input_val):
             input_val = [input_val]
             input_val = array(input_val).reshape(len(input_val),)
         if (func == 'trapmf'):
             membership=trapmf(input_val, vertex)
-        if (func == "trimf"):
+        elif (func == "trimf"):
             membership=trimf(input_val, vertex)
-        if (func == "gaussmf"):
+        elif (func == "gaussmf"):
             membership=gaussmf(input_val, vertex[0],vertex[1])
-        if (func == "gbellmf"):
+        elif (func == "gbellmf"):
             membership=gbellmf(input_val, vertex[0],vertex[1],vertex[2])
-        if (func == "eq"):
-            x = input_val
+        elif (func == "eq"):
+            x = input_val.transpose()
             membership = eval(vertex)
-        if (func == "raw"):
+        elif (func == "raw"):
             v = array(vertex)
             membership = v[input_val==universe]
         return array(membership)
     def defuzzification(self,sc,universe,func):
         """ Defuzzifies the given fuzzy set with the method given.
 
         Args:
@@ -340,74 +343,88 @@
                 `'mom'`: Mean of maxima.
                 `'som'`: Smallest of maxima.
                 `'lom'`: Largest of maxima.
         Returns:
             defuzzifiedv (float): Defuzzified value.
         """
         try:
-            defuzzific = defuzz(universe,sc,func)
+                defuzzific = array([0 if sum(i)==0 else defuzz(universe,i,func)  for i in sc]) 
         except:
             defuzzific = 0
         return defuzzific
 
     def fuzzy_system_sim(self, inputs_val):
         """Simulate an input and returns the output of the defined inference system, rembember to check that all universes of premises and consequences have the same number of elements.
 
         Args:
-            inputs_val (list): Input value per input premise in a list.
+            inputs_val (ndarray): Input value ndarray nxp with n as the number of samples and p the number of premises or list with p elements in first dimension and n samples in second dimension.
 
         Returns:
             output_val (ndarray): Output of the inference system.
         """
-        IM = tuple([zeros((len(self.structure['Rules']),len(i))) for i in self.structure['output_universes']])
-        miuo = zeros(len(self.structure['output_universes']))
-        out_def = zeros(len(self.structure['output_universes']))
-        for i in range(len(self.structure['Rules'])):
-            conectorsv = self.structure['Rules'][i]['conectors'].copy()
-            a = self.fuzzification(self.structure['Rules'][i]['antecedent'][0][0],self.structure['Rules'][i]['antecedent'][0][1],inputs_val[0],self.structure['Rules'][i]['antecedent'][0][2])
-            for j in range(len(self.structure['Rules'][i]['antecedent'])-1):
-                conect = conectorsv.pop(0)
-                if conect =='and' and self.structure['AndConector']=='min':
-                    a = minimum(a,self.fuzzification(self.structure['Rules'][i]['antecedent'][j+1][0],self.structure['Rules'][i]['antecedent'][j+1][1],inputs_val[j+1],self.structure['Rules'][i]['antecedent'][0][2]))
-                if conect =='or' and self.structure['OrConector']=='max':
-                    a = maximum(a,self.fuzzification(self.structure['Rules'][i]['antecedent'][j+1][0],self.structure['Rules'][i]['antecedent'][j+1][1],inputs_val[j+1],self.structure['Rules'][i]['antecedent'][0][2]))
-                if conect =='and' and self.structure['AndConector']=='prod':
-                    a = a*self.fuzzification(self.structure['Rules'][i]['antecedent'][j+1][0],self.structure['Rules'][i]['antecedent'][j+1][1],inputs_val[j+1],self.structure['Rules'][i]['antecedent'][0][2])
-                if conect =='or' and self.structure['OrConector']=='probsum':
-                    b = self.fuzzification(self.structure['Rules'][i]['antecedent'][j+1][0],self.structure['Rules'][i]['antecedent'][j+1][1],inputs_val[j+1],self.structure['Rules'][i]['antecedent'][0][2])
-                    a = (a+b)-(a*b)
-            for k in range(len(self.structure['Rules'][i]['consequent'])):
-                if isinstance(self.structure['Rules'][i]['consequent'][k][0],str) and  self.structure['Defuzz'] != 'centroidTS':
-                    self.structure['Rules'][i]['consequent'][k] = self.fuzzification(self.structure['Rules'][i]['consequent'][k][0],self.structure['Rules'][i]['consequent'][k][1],self.structure['output_universes'][self.structure['Rules'][i]['output_universes'][k]],self.structure['Rules'][i]['antecedent'][0][2])
-                if self.structure['Defuzz'] != 'centroidTS':
-                    if self.structure['Implication'] =='min':
-                        IM[k][i,:] = fmin(a,self.structure['Rules'][i]['consequent'][k])
-                    if self.structure['Implication'] =='prod':
-                        IM[k][i,:] = a*self.structure['Rules'][i]['consequent'][k]
+        a =True
+        if isinstance(inputs_val,list):
+            inputs_val = array(inputs_val)
+            if inputs_val.shape[0] == len(self.premises):
+                if len(inputs_val.shape)>1:
+                    inputs_val=inputs_val.reshape(inputs_val.shape[1],inputs_val.shape[0])
                 else:
-                    x = inputs_val
-                    if self.structure['Implication'] =='min':
-                        IM[k][i,0] = fmin(a,self.fuzzification(self.structure['Rules'][i]['consequent'][k][0],self.structure['Rules'][i]['consequent'][k][1],inputs_val,self.structure['Rules'][i]['antecedent'][0][2]))
-                        miuo[k] = miuo[k] + a
-                    if self.structure['Implication'] =='prod':
-                        IM[k][i,0] = a*self.fuzzification(self.structure['Rules'][i]['consequent'][k][0],self.structure['Rules'][i]['consequent'][k][1],inputs_val,self.structure['Rules'][i]['antecedent'][0][2])
-                        miuo[k] = miuo[k] + a
-        for k in range(len(self.structure['output_universes'])):
-            if self.structure['Defuzz'] != 'centroidTS':
-                if self.structure['Agregattor'] =='max':
-                    outf = max(IM[k],axis=0)
-                if self.structure['Agregattor'] =='probsum':
-                    outf = sum(IM[k],axis = 0)-prod(IM[k], axis= 0)
-                out_def[k] = self.defuzzification(outf,self.structure['output_universes'][k],self.structure['Defuzz'])
+                    inputs_val=inputs_val.reshape(1,inputs_val.shape[0])
             else:
-                if miuo[k]>0:
-                    out_def[k] = sum(IM[k][:,0])/miuo[k]
+                a = False
+                print("Wrong dimensions for inputs try Input value ndarray nxp with n as the number of samples and p the number of premises or list with p elements in first dimension and n samples in second dimension.")
+            
+            
+        if a:
+            IM = tuple([zeros((len(self.structure['Rules']),inputs_val.shape[0],len(i))) for i in self.structure['output_universes']])
+            miuo = zeros((len(self.structure['output_universes']),inputs_val.shape[0]))
+            out_def = zeros((len(self.structure['output_universes']),inputs_val.shape[0]))
+            for i in range(len(self.structure['Rules'])):
+                conectorsv = self.structure['Rules'][i]['conectors'].copy()
+                a = self.fuzzification(self.structure['Rules'][i]['antecedent'][0][0],self.structure['Rules'][i]['antecedent'][0][1],inputs_val[:,0],self.structure['Rules'][i]['antecedent'][0][2])
+                for j in range(len(self.structure['Rules'][i]['antecedent'])-1):
+                    conect = conectorsv.pop(0)
+                    if conect =='and' and self.structure['AndConector']=='min':
+                        a = minimum(a,self.fuzzification(self.structure['Rules'][i]['antecedent'][j+1][0],self.structure['Rules'][i]['antecedent'][j+1][1],inputs_val[:,j+1],self.structure['Rules'][i]['antecedent'][0][2]))
+                    elif conect =='or' and self.structure['OrConector']=='max':
+                        a = maximum(a,self.fuzzification(self.structure['Rules'][i]['antecedent'][j+1][0],self.structure['Rules'][i]['antecedent'][j+1][1],inputs_val[:,j+1],self.structure['Rules'][i]['antecedent'][0][2]))
+                    elif conect =='and' and self.structure['AndConector']=='prod':
+                        a = multiply(a,self.fuzzification(self.structure['Rules'][i]['antecedent'][j+1][0],self.structure['Rules'][i]['antecedent'][j+1][1],inputs_val[:,j+1],self.structure['Rules'][i]['antecedent'][0][2]))
+                    elif conect =='or' and self.structure['OrConector']=='probsum':
+                        b = self.fuzzification(self.structure['Rules'][i]['antecedent'][j+1][0],self.structure['Rules'][i]['antecedent'][j+1][1],inputs_val[:,j+1],self.structure['Rules'][i]['antecedent'][0][2])
+                        a = (a+b)-multiply(a,b)
+                for k in range(len(self.structure['Rules'][i]['consequent'])):
+                    if isinstance(self.structure['Rules'][i]['consequent'][k][0],str) and  self.structure['Defuzz'] != 'centroidTS':
+                        self.structure['Rules'][i]['consequent'][k] = self.fuzzification(self.structure['Rules'][i]['consequent'][k][0],self.structure['Rules'][i]['consequent'][k][1],self.structure['output_universes'][self.structure['Rules'][i]['output_universes'][k]],self.structure['Rules'][i]['antecedent'][0][2])
+                    if self.structure['Defuzz'] != 'centroidTS':
+                        if self.structure['Implication'] =='min':
+                            IM[k][i,:] = fmin(a.reshape(a.shape[0],1),repeat((self.structure['Rules'][i]['consequent'][k]).reshape((1,self.structure['Rules'][i]['consequent'][k].shape[0])),a.shape[0],axis = 0))
+                        elif self.structure['Implication'] =='prod':
+                            IM[k][i,:] = (a.reshape(a.shape[0],1).repeat(len(self.structure['Rules'][i]['consequent'][k]),axis = 1)*self.structure['Rules'][i]['consequent'][k])
+                    else:
+                        x = inputs_val
+                        if self.structure['Implication'] =='min':
+                            IM[k][i,0] = fmin(a,self.fuzzification(self.structure['Rules'][i]['consequent'][k][0],self.structure['Rules'][i]['consequent'][k][1],inputs_val,self.structure['Rules'][i]['antecedent'][0][2]))
+                            miuo[k] = miuo[k] + a
+                        if self.structure['Implication'] =='prod':
+                            IM[k][i,:,0] = multiply(a,self.fuzzification(self.structure['Rules'][i]['consequent'][k][0],self.structure['Rules'][i]['consequent'][k][1],inputs_val,self.structure['Rules'][i]['antecedent'][0][2]))
+                            miuo[k] = miuo[k] + a
+            for k in range(len(self.structure['output_universes'])):
+                if self.structure['Defuzz'] != 'centroidTS':
+                    if self.structure['Agregattor'] =='max':
+                        outf = max(IM[k],axis=0)
+                    if self.structure['Agregattor'] =='probsum':
+                        outf = sum(IM[k],axis = 0)-prod(IM[k], axis= 0)
+                    out_def[k] = self.defuzzification(outf,self.structure['output_universes'][k],self.structure['Defuzz'])
                 else:
-                    out_def[k] = 0
-        return out_def
+                    if max(miuo[k]>0):
+                        out_def[k] = sum(IM[k][:,:,0],axis=0)/miuo[k]
+                    else:
+                        out_def[k] = zeros(miuo[k].shape)
+            return out_def
 
     def surface_fuzzy_system(self, inputvals=[],figsizeU=(15,15)):
         
         """Plots the response of the inference system for the list of input arrays for each premise, remember to check that premises and consequences universes have the same number of elements.
         
 
         Args:
@@ -415,33 +432,34 @@
 
         Returns:
         none
         """
         
         surface_out = []
         if len(inputvals)==2:
-            surface = array([[self.fuzzy_system_sim([i,j]) for j in inputvals[1]] for i in inputvals[0]]).reshape((len(inputvals[0]),len(inputvals[1])))
+            surfinputs = array([[([i,j]) for j in inputvals[1]] for i in inputvals[0]]).reshape(inputvals[0].shape[0]*inputvals[1].shape[0],len(inputvals))
+            surface = self.fuzzy_system_sim(surfinputs).reshape(inputvals[0].shape[0],inputvals[1].shape[0]) 
             X, Y = meshgrid(inputvals[0], inputvals[1])
             plt.figure(figsize=figsizeU)
             ax = plt.axes(projection='3d')
             print(X.shape)
             print(Y.shape)
             print(surface.shape)
             ax.plot_surface(X, Y, surface.transpose(), rstride=1, cstride=1,
                             cmap='viridis', edgecolor='none')
             ax.set_title('Surface Response: '+self.name)
             ax.set_xlabel(self.premises[0].name)
             ax.set_ylabel(self.premises[1].name)
             plt.show()
         if len(inputvals)==1:
-            surface = array([self.fuzzy_system_sim([i]) for i in inputvals[0]]).reshape((len(inputvals[0])))
+            surface = self.fuzzy_system_sim(inputvals) 
             plt.figure(figsize=figsizeU)
             ax = plt.axes()
-            ax.plot(inputvals[0], surface)
-            ax.set_title('Surface Response: '+self.name);
+            ax.plot(inputvals[0], surface[0])
+            ax.set_title('Surface Response: '+self.name)
             ax.set_xlabel(self.premises[0].name)
             plt.show()
 
 class fuzzy_controller():
 
     """Allows to implement a fuzzy controller system based on an inference system.
     
@@ -475,15 +493,15 @@
         self.GIE = GIE
         self.typec = typec
         self.DT = DT
         self.controller = []
         self.tf =tf
         self.inference_system = inference_system
     def error_vals(self,t, x, u, params):
-        error = u
+        error = u[0]
         accumulated_error = x[0]+error
         previous_error = x[0]
         return [error,previous_error,accumulated_error]
     def error_val(self,t, x, u, params):
         error = [u[0]-u[1]]
         return error
     def fuzzy_PDIcontrol(self,t, x, u, params):
```

### Comparing `UPAFuzzySystems-0.1.0/UPAFuzzySystems.egg-info/PKG-INFO` & `UPAFuzzySystems-0.2.0/UPAFuzzySystems.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: UPAFuzzySystems
-Version: 0.1.0
+Version: 0.2.0
 Summary: UPAFuzzySystems package for definition and simulation of Fuzzy Inference Systems for general and control applications.
 Home-page: https://github.com/UniversidadPolitecnicaAguascalientes/UPAFuzzySystems/
 Author: Dr. Martin Montes Rivera (Universidad Politécnica de Aguascalientes)
 Author-email: <martin.montes@upa.edu.mx>
-License: UNKNOWN
-Description: UPAFuzzySystems library allows defining Fuzzy Inference Systems for different applications with continuous and discrete universes, it also deploys structures for simulation of fuzzy control with transfer functions and state space models.
 Keywords: python,fuzzy logic,fuzzy control,fuzzy inference systems,artificial intelligence
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+UPAFuzzySystems library allows defining Fuzzy Inference Systems for different applications with continuous and discrete universes, it also deploys structures for simulation of fuzzy control with transfer functions and state space models.
```

### Comparing `UPAFuzzySystems-0.1.0/setup.py` & `UPAFuzzySystems-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.1.0'
+VERSION = '0.2.0'
 DESCRIPTION = 'UPAFuzzySystems package for definition and simulation of Fuzzy Inference Systems for general and control applications.'
 LONG_DESCRIPTION = 'UPAFuzzySystems library allows defining Fuzzy Inference Systems for different applications with continuous and discrete universes, it also deploys structures for simulation of fuzzy control with transfer functions and state space models.'
 
 # Setting up
 setup(
     name="UPAFuzzySystems",
     version=VERSION,
```

