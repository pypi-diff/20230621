# Comparing `tmp/sphecerix-0.3.0-py3-none-any.whl.zip` & `tmp/sphecerix-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6717 bytes, number of entries: 9
--rw-r--r--  2.0 unx      245 b- defN 23-Jun-08 19:14 sphecerix/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-08 19:14 sphecerix/_version.py
--rw-r--r--  2.0 unx     3394 b- defN 23-Jun-08 19:14 sphecerix/atomic_wave_functions.py
--rw-r--r--  2.0 unx     1220 b- defN 23-Jun-08 19:14 sphecerix/tesseral.py
--rw-r--r--  2.0 unx     7925 b- defN 23-Jun-08 19:14 sphecerix/wignerd.py
--rw-r--r--  2.0 unx     2873 b- defN 23-Jun-08 19:14 sphecerix-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 19:14 sphecerix-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-08 19:14 sphecerix-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      705 b- defN 23-Jun-08 19:14 sphecerix-0.3.0.dist-info/RECORD
-9 files, 16485 bytes uncompressed, 5505 bytes compressed:  66.6%
+Zip file size: 6952 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      296 b- defN 23-Jun-21 07:21 sphecerix/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-21 07:21 sphecerix/_version.py
+-rw-r--r--  2.0 unx     3394 b- defN 23-Jun-21 07:21 sphecerix/atomic_wave_functions.py
+-rw-r--r--  2.0 unx     1220 b- defN 23-Jun-21 07:21 sphecerix/tesseral.py
+-rw-r--r--  2.0 unx    10070 b- defN 23-Jun-21 07:21 sphecerix/wignerd.py
+-rw-r--r--  2.0 unx     2873 b- defN 23-Jun-21 07:21 sphecerix-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 07:21 sphecerix-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-21 07:21 sphecerix-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      706 b- defN 23-Jun-21 07:21 sphecerix-0.4.0.dist-info/RECORD
+9 files, 18682 bytes uncompressed, 5740 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: sphecerix/tesseral.py
 Comment: 
 
 Filename: sphecerix/wignerd.py
 Comment: 
 
-Filename: sphecerix-0.3.0.dist-info/METADATA
+Filename: sphecerix-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: sphecerix-0.3.0.dist-info/WHEEL
+Filename: sphecerix-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: sphecerix-0.3.0.dist-info/top_level.txt
+Filename: sphecerix-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sphecerix-0.3.0.dist-info/RECORD
+Filename: sphecerix-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sphecerix/__init__.py

```diff
@@ -1,5 +1,6 @@
-from .wignerd import tesseral_wigner_D, wigner_D, tesseral_wigner_D_mirror
+from .wignerd import tesseral_wigner_D, wigner_D, tesseral_wigner_D_mirror,\
+                     tesseral_wigner_D_improper
 from .tesseral import tesseral_transformation, permutation_sh_car
 from .atomic_wave_functions import wfcart, wf, wffield, wffield_l
 
 from ._version import __version__
```

## sphecerix/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.3.0"
+__version__ = "0.4.0"
```

## sphecerix/wignerd.py

```diff
@@ -4,15 +4,15 @@
 from scipy.special import factorial
 from scipy.spatial.transform import Rotation as R
 from .tesseral import tesseral_transformation
 import warnings
 
 def tesseral_wigner_D(l, Robj):
     """
-    Produce the Wigner D-matrix for tesseral spherical harmonics
+    Produce the Wigner D-matrix for tesseral spherical harmonics for a rotation
 
     Parameters
     ----------
     l : int
         Order of the spherical harmonics
     Robj : scipy.spatial.transform.Rotation
         Rotation in :math:`\mathbb{R}^{3}`
@@ -119,14 +119,76 @@
         warnings.filterwarnings('ignore', r'Gimbal lock detected. Setting third angle to zero since it is not possible to uniquely determine all angles.')
         alpha, beta, gamma = Robj.as_euler('zyz', degrees=False)
         
     D = wigner_D(l, Robj)
     
     return inv * np.real(T @ D @ T.conjugate().transpose())
 
+def tesseral_wigner_D_improper(l, Robj):
+    """
+    Produce the Wigner D-matrix for tesseral spherical harmonics under an
+    improper rotation
+
+    Parameters
+    ----------
+    l : int
+        Order of the spherical harmonics
+    Robj : scipy.spatial.transform.Rotation
+        Rotation in :math:`\mathbb{R}^{3}`
+
+    Returns
+    -------
+    D : numpy.ndarray
+        Real-valued Wigner-D matrix with dimensions :math:`(2l+1) \\times (2l+1)`
+
+    Raises
+    ------
+    TypeError
+        If the Robj object is not of type scipy.spatial.transform.R.
+        
+    Examples
+    --------
+    >>> from sphecerix import tesseral_wigner_D_improper
+    ... from scipy.spatial.transform import Rotation as R
+    ... import numpy as np
+    ... 
+    ... # construct (improper) rotation vector
+    ... axis = np.array([1,0,0])
+    ... Robj = R.from_rotvec(axis * np.pi / 2)
+    ... 
+    ... # construct wigner D matrix
+    ... D = tesseral_wigner_D_improper(1, Robj)
+    ... 
+    ... print(D)
+    [[ 7.49879891e-33 -1.00000000e+00  1.83697020e-16]
+     [ 1.00000000e+00 -2.24963967e-32 -1.83697020e-16]
+     [-1.83697020e-16 -1.83697020e-16 -1.00000000e+00]]
+
+    Construct the Wigner-D matrix for the tesseral p-orbitals for an improper
+    rotation by 90 degrees around the cartesian x-axis.
+    """
+    # verify that Robj is a rotation object
+    if not isinstance(Robj, R):
+        raise TypeError('Second argument Robj should be of type scipy.spatial.transform.R')
+    
+    T = tesseral_transformation(l)
+    with warnings.catch_warnings():
+        warnings.filterwarnings('ignore', r'Gimbal lock detected. Setting third angle to zero since it is not possible to uniquely determine all angles.')
+        alpha, beta, gamma = Robj.as_euler('zyz', degrees=False)
+        
+    D = wigner_D(l, Robj)
+    
+    # extract rotation vector from rotation object and use it to construct
+    # a mirror matrix
+    normal = Robj.as_rotvec()
+    normal /= np.linalg.norm(normal)
+    M = tesseral_wigner_D_mirror(l, normal)
+    
+    return M @ np.real(T @ D @ T.conjugate().transpose())
+
 def wigner_D(l, Robj):
     """
     Produce Wigner D-matrix for canonical spherical harmonics
 
     Parameters
     ----------
     l : int
```

## Comparing `sphecerix-0.3.0.dist-info/METADATA` & `sphecerix-0.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphecerix
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python package for constructing Wigner-D matrices
 Home-page: https://github.com/ifilot/sphecerix
 Author: Ivo Filot
 Author-email: ivo@ivofilot.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

