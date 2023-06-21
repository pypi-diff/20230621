# Comparing `tmp/orr_sommerfeld_convmix_cgb-0.2.1.tar.gz` & `tmp/orr_sommerfeld_convmix_cgb-0.2.2.tar.gz`

## Comparing `orr_sommerfeld_convmix_cgb-0.2.1.tar` & `orr_sommerfeld_convmix_cgb-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.1/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.1/src/Orr_Sommerfeld_convmix_CGB/__init__.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.1/LICENSE
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.1/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.2/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.2/src/Orr_Sommerfeld_convmix_CGB/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.2/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.2/PKG-INFO
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.1/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py` & `orr_sommerfeld_convmix_cgb-0.2.2/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py`

 * *Files 5% similar despite different names*

```diff
@@ -244,31 +244,39 @@
     layout = go.Layout(title=dict(text=titulo), xaxis=dict(title='r$c_{r}$',titlefont=dict(size=18), tickfont=dict(family='latex')), 
                                                                    yaxis=dict(title=r'$c_{i}$',titlefont=dict(size=18), tickfont=dict(family='latex')),
                                                                    plot_bgcolor='rgba(0,0,0,0.1)',
                                                                    title_x=0.5)
     fig = go.Figure(data=[traza], layout=layout)
     iplot(fig)
     return
-def vector_perturbaciones(N,lam,V,n,alpha,beta):
+def vector_perturbaciones(N,lam,V,n,alpha,beta,Ra):
     D,D2,D4=Dmat(N)
     #Chekeado que Dmat funciona bien
-   
+    U,U1,U2=flujobase(N,Ra)
     #Calculo parámetros de mis ecuaciones
     I=eye(N-1)
     k2=(alpha*alpha)+(beta*beta)
     k22=k2*k2
    
     v=V[0:(N-1),n]
-    tita=V[(N-1):(2*(N-1)),n]
-    eta=V[2*(N-1):3*(N-1),n]
-    #Expresión de u
-    u= (1j*alpha*dot(D,v)/k2) + dot(beta/k2,eta)
-    #Expresión de w
-    w=((beta*u)-eta)/alpha
-    # Falta agregar la presion y las expresiones individuales de w y u
+    if Ra==0:
+        tita=zeros(N-1)
+        eta=dot((-(D4-2.*k2*D2+k2*k2*I)/(Re) + 1j*alpha*U*I - 1j*alpha*lam[n]*I),-1j*beta*dot(U1*I,v))
+        #Expresión de u
+        u= (1j*alpha*dot(D,v)/k2) + dot(beta/k2,(eta/1j))
+        #Expresión de w
+        w=((beta*u)-(eta/1j))/alpha
+    else:
+        tita=V[(N-1):(2*(N-1)),n]
+        eta=V[2*(N-1):3*(N-1),n]
+        #Expresión de u
+        u= (1j*alpha*dot(D,v)/k2) + dot(beta/k2,eta)
+        #Expresión de w
+        w=((beta*u)-eta)/alpha
+    # Falta agregar la presion 
     return  v,u,w,tita
 def normalizacion(v,u,w,tita):
     vr=v.real
     vi=v.imag
     #Busca el valor de màxima norma de u
     norm= vr*vr+vi*vi
     i=np.where(abs(norm) == np.max(norm))
@@ -292,15 +300,15 @@
     #plt.style.use('ggplot')
     #Vector y
     D,y = cheb(N)
     #Vectores de perturbaciones para un autovalor dado. En este caso tomo el mayor de todos dado que Orr_Sommerfeld() las ordena y voy a elegir n=0
     n=0
     lam,V,max_real,max_imag=Orr_Sommerfeld(N,Ra,Pr,Re,alpha,beta)
 
-    v,u,w,tita=vector_perturbaciones(N,lam,V,n,alpha,beta)
+    v,u,w,tita=vector_perturbaciones(N,lam,V,n,alpha,beta,Ra)
     v,u,w,tita=normalizacion(v,u,w,tita)
 
     realv = v.real
     imv = v.imag
     realtita = tita.real
     imtita = tita.imag
     realu = u.real
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.1/LICENSE` & `orr_sommerfeld_convmix_cgb-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.2.1/README.md` & `orr_sommerfeld_convmix_cgb-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 To understand the flow conditions that cause this transition mathematically and how it affects heat transfer, the linear stability theory can be used. This theory predicts when a laminar flow becomes turbulent by analyzing small disturbances and determining if they will grow or dissipate. If the disturbances grow, the laminar flow becomes unstable and transitions to turbulence. This package focuses on examining the temporal transition, using spatial variables as inputs.
 
 ## Technologies
 Project is created with:
 * [NumPy](https://numpy.org/)
 * [SciPy](https://scipy.org/)
-* [Plotly] (https://plotly.com/)
+* [Plotly](https://plotly.com/)
 * [Pandas](https://pandas.pydata.org/)
 * [PyPi](https://pypi.org/) to publish Python package.
 
 
 ## Installation
 It is possible to install using pip:
 ```Python
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.1/pyproject.toml` & `orr_sommerfeld_convmix_cgb-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "Orr_Sommerfeld_convmix_CGB"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Pablo Szuban", email="pablo.szuban@ib.edu.ar" },
 ]
 description = "Paquete para cálculo de autovalores y autofunciones."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.1/PKG-INFO` & `orr_sommerfeld_convmix_cgb-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orr_Sommerfeld_convmix_CGB
-Version: 0.2.1
+Version: 0.2.2
 Summary: Paquete para cálculo de autovalores y autofunciones.
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Project-URL: Source Code, https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb
 Author-email: Pablo Szuban <pablo.szuban@ib.edu.ar>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -28,15 +28,15 @@
 
 To understand the flow conditions that cause this transition mathematically and how it affects heat transfer, the linear stability theory can be used. This theory predicts when a laminar flow becomes turbulent by analyzing small disturbances and determining if they will grow or dissipate. If the disturbances grow, the laminar flow becomes unstable and transitions to turbulence. This package focuses on examining the temporal transition, using spatial variables as inputs.
 
 ## Technologies
 Project is created with:
 * [NumPy](https://numpy.org/)
 * [SciPy](https://scipy.org/)
-* [Plotly] (https://plotly.com/)
+* [Plotly](https://plotly.com/)
 * [Pandas](https://pandas.pydata.org/)
 * [PyPi](https://pypi.org/) to publish Python package.
 
 
 ## Installation
 It is possible to install using pip:
 ```Python
```

