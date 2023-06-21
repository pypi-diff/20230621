# Comparing `tmp/orr_sommerfeld_convmix_cgb-0.2.3.tar.gz` & `tmp/orr_sommerfeld_convmix_cgb-0.2.4.tar.gz`

## Comparing `orr_sommerfeld_convmix_cgb-0.2.3.tar` & `orr_sommerfeld_convmix_cgb-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.3/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.3/src/Orr_Sommerfeld_convmix_CGB/__init__.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.3/LICENSE
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.3/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    12044 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.4/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.4/src/Orr_Sommerfeld_convmix_CGB/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.4/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.4/PKG-INFO
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.3/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py` & `orr_sommerfeld_convmix_cgb-0.2.4/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,16 +314,16 @@
     realu = u.real
     imu = u.imag 
     realw = w.real 
     imw = w.imag
 
     plt.plot(y,realv,c='red',label= "$v_r(y)$")
     plt.plot(y,imv,"--",c='red',label= "$v_i(y)$")
-    plt.plot(y,realtita,"-",c='blue',label= r'$\theta_{r}(y)$')
-    plt.plot(y,imtita,"--",c='blue',label= r'$\theta_{i}(y)$')
+    plt.plot(y,realtita,"-",c='blue',label= r'$\Tilde{\theta}_{r}(y)$')
+    plt.plot(y,imtita,"--",c='blue',label= r'$\Tilde{\theta}_{i}(y)$')
     plt.plot(y,realu,c='lightgreen',label= r'$u_{r}(y)$')
     plt.plot(y,imu,"--",c='lightgreen',label= r'$u_{i}(y)$')
     #plt.plot(y,realw,c='pink',label= r'$w_{r}(y)$')
     #plt.plot(y,imw,"--",c='pink',label= r'$w_{i}(y)$')
 
 
     plt.xlim(-1,1)
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.3/LICENSE` & `orr_sommerfeld_convmix_cgb-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.2.3/README.md` & `orr_sommerfeld_convmix_cgb-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 ```
 * Can compute the spectrum of temporal eigenvalues (disturbances frecuency) and their respective eigenvectors, which are the amplitude of the disturbances. Also can obtain the real and imaginary parts of the eigenvalue which its imaginary part is the maximum:
 ```Python
 [lam,V,max_real,max_imag]=OS_CM.Orr_Sommerfeld(N,Ra,Pr,Re,alpha,beta)
 ```
 * The lam array is sorted from highest imaginary part to lowest imaginary part, and it contains all the eigenvalues. To obtain the eigenvectors corresponding to a given eigenvalue, you can do:
 ```Python
-[v,u,w,tita]=OS_CM.vector_perturbaciones(N,lam,V,0,alpha,beta)
+[v,u,w,tita]=OS_CM.vector_perturbaciones(N,lam,V,0,alpha,beta,Re,Ra)
 ```
 * Where v, u and w are de amplitudes of the velocity disturbances and tita is the amplitude of the temperature disturbance. In this example, the eigenvalue choosen was the first one in lam. 
 * There is also available a function to normalize the disturbances such that when the phase of v is zero, its norm is maximum and equal to 1:
 ```Python
 [v,u,w,tita]=OS_CM.normalizacion(v,u,w,tita)
 ```
 * Additionally, there is a function that plots the eigenvalues using the matplotlib library. The package also includes an interactive plot of the eigenvalues using pandas
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.3/pyproject.toml` & `orr_sommerfeld_convmix_cgb-0.2.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "Orr_Sommerfeld_convmix_CGB"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Pablo Szuban", email="pablo.szuban@ib.edu.ar" },
 ]
 description = "Paquete para cálculo de autovalores y autofunciones."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.3/PKG-INFO` & `orr_sommerfeld_convmix_cgb-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orr_Sommerfeld_convmix_CGB
-Version: 0.2.3
+Version: 0.2.4
 Summary: Paquete para cálculo de autovalores y autofunciones.
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Project-URL: Source Code, https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb
 Author-email: Pablo Szuban <pablo.szuban@ib.edu.ar>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
 ```
 * Can compute the spectrum of temporal eigenvalues (disturbances frecuency) and their respective eigenvectors, which are the amplitude of the disturbances. Also can obtain the real and imaginary parts of the eigenvalue which its imaginary part is the maximum:
 ```Python
 [lam,V,max_real,max_imag]=OS_CM.Orr_Sommerfeld(N,Ra,Pr,Re,alpha,beta)
 ```
 * The lam array is sorted from highest imaginary part to lowest imaginary part, and it contains all the eigenvalues. To obtain the eigenvectors corresponding to a given eigenvalue, you can do:
 ```Python
-[v,u,w,tita]=OS_CM.vector_perturbaciones(N,lam,V,0,alpha,beta)
+[v,u,w,tita]=OS_CM.vector_perturbaciones(N,lam,V,0,alpha,beta,Re,Ra)
 ```
 * Where v, u and w are de amplitudes of the velocity disturbances and tita is the amplitude of the temperature disturbance. In this example, the eigenvalue choosen was the first one in lam. 
 * There is also available a function to normalize the disturbances such that when the phase of v is zero, its norm is maximum and equal to 1:
 ```Python
 [v,u,w,tita]=OS_CM.normalizacion(v,u,w,tita)
 ```
 * Additionally, there is a function that plots the eigenvalues using the matplotlib library. The package also includes an interactive plot of the eigenvalues using pandas
```

