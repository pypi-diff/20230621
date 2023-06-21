# Comparing `tmp/matgl-0.6.0.tar.gz` & `tmp/matgl-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.6.0.tar", last modified: Tue Jun 20 17:13:23 2023, max compression
+gzip compressed data, was "matgl-0.6.1.tar", last modified: Wed Jun 21 03:35:27 2023, max compression
```

## Comparing `matgl-0.6.0.tar` & `matgl-0.6.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.376536 matgl-0.6.0/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-06-13 15:50:33.000000 matgl-0.6.0/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)    12710 2023-06-20 17:13:23.376361 matgl-0.6.0/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)    11541 2023-06-18 20:24:30.000000 matgl-0.6.0/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.371466 matgl-0.6.0/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)      394 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.372420 matgl-0.6.0/matgl/apps/
--rw-r--r--   0 shyue      (501) staff       (20)      180 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/apps/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4160 2023-06-20 15:49:52.000000 matgl-0.6.0/matgl/apps/pes.py
--rw-r--r--   0 shyue      (501) staff       (20)     1996 2023-06-14 22:12:57.000000 matgl-0.6.0/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.372659 matgl-0.6.0/matgl/data/
--rw-r--r--   0 shyue      (501) staff       (20)       55 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/data/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2503 2023-06-13 19:04:59.000000 matgl-0.6.0/matgl/data/transformer.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.372995 matgl-0.6.0/matgl/ext/
--rw-r--r--   0 shyue      (501) staff       (20)      118 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/ext/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    15898 2023-06-20 15:38:59.000000 matgl-0.6.0/matgl/ext/ase.py
--rw-r--r--   0 shyue      (501) staff       (20)     5278 2023-06-20 15:33:59.000000 matgl-0.6.0/matgl/ext/pymatgen.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.373457 matgl-0.6.0/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       52 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5133 2023-06-20 15:44:52.000000 matgl-0.6.0/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)      513 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/graph/converters.py
--rw-r--r--   0 shyue      (501) staff       (20)    11614 2023-06-20 15:52:57.000000 matgl-0.6.0/matgl/graph/data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.374611 matgl-0.6.0/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)      676 2023-06-15 04:03:30.000000 matgl-0.6.0/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2030 2023-06-20 15:42:17.000000 matgl-0.6.0/matgl/layers/_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     2983 2023-06-20 15:39:42.000000 matgl-0.6.0/matgl/layers/_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     9428 2023-06-20 15:39:42.000000 matgl-0.6.0/matgl/layers/_basis.py
--rw-r--r--   0 shyue      (501) staff       (20)     2186 2023-06-20 15:39:42.000000 matgl-0.6.0/matgl/layers/_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     6029 2023-06-20 15:39:42.000000 matgl-0.6.0/matgl/layers/_core.py
--rw-r--r--   0 shyue      (501) staff       (20)     3509 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/layers/_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)    16602 2023-06-20 15:47:00.000000 matgl-0.6.0/matgl/layers/_graph_convolution.py
--rw-r--r--   0 shyue      (501) staff       (20)     3872 2023-06-20 15:39:42.000000 matgl-0.6.0/matgl/layers/_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     3944 2023-06-20 15:46:20.000000 matgl-0.6.0/matgl/layers/_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.375054 matgl-0.6.0/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)      187 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    11558 2023-06-20 15:53:17.000000 matgl-0.6.0/matgl/models/_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     9539 2023-06-20 15:39:42.000000 matgl-0.6.0/matgl/models/_megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     2147 2023-06-15 04:29:37.000000 matgl-0.6.0/matgl/models/_wrappers.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.375801 matgl-0.6.0/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       61 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      799 2023-06-13 19:01:28.000000 matgl-0.6.0/matgl/utils/cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)    10520 2023-06-17 15:05:12.000000 matgl-0.6.0/matgl/utils/io.py
--rw-r--r--   0 shyue      (501) staff       (20)     7129 2023-06-20 15:43:24.000000 matgl-0.6.0/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.6.0/matgl/utils/sb_roots.npy
--rw-r--r--   0 shyue      (501) staff       (20)    13317 2023-06-20 16:49:51.000000 matgl-0.6.0/matgl/utils/training.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.372173 matgl-0.6.0/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)    12710 2023-06-20 17:13:23.000000 matgl-0.6.0/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)      979 2023-06-20 17:13:23.000000 matgl-0.6.0/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-20 17:13:23.000000 matgl-0.6.0/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-20 17:13:23.000000 matgl-0.6.0/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-20 17:13:23.000000 matgl-0.6.0/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     2427 2023-06-14 21:01:08.000000 matgl-0.6.0/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-20 17:13:23.376589 matgl-0.6.0/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     2018 2023-06-20 17:12:29.000000 matgl-0.6.0/setup.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-20 17:13:23.375913 matgl-0.6.0/tests/
--rw-r--r--   0 shyue      (501) staff       (20)      194 2023-06-15 14:49:26.000000 matgl-0.6.0/tests/test_config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 03:35:27.365022 matgl-0.6.1/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-06-13 15:50:33.000000 matgl-0.6.1/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)    12710 2023-06-21 03:35:27.364842 matgl-0.6.1/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)    11541 2023-06-18 20:24:30.000000 matgl-0.6.1/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 03:35:27.359713 matgl-0.6.1/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      394 2023-06-13 19:01:28.000000 matgl-0.6.1/matgl/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 03:35:27.360713 matgl-0.6.1/matgl/apps/
+-rw-r--r--   0 shyue      (501) staff       (20)      180 2023-06-13 19:01:28.000000 matgl-0.6.1/matgl/apps/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4160 2023-06-20 15:49:52.000000 matgl-0.6.1/matgl/apps/pes.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1996 2023-06-14 22:12:57.000000 matgl-0.6.1/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 03:35:27.360942 matgl-0.6.1/matgl/data/
+-rw-r--r--   0 shyue      (501) staff       (20)       55 2023-06-13 19:01:28.000000 matgl-0.6.1/matgl/data/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2503 2023-06-13 19:04:59.000000 matgl-0.6.1/matgl/data/transformer.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 03:35:27.361272 matgl-0.6.1/matgl/ext/
+-rw-r--r--   0 shyue      (501) staff       (20)      118 2023-06-13 19:01:28.000000 matgl-0.6.1/matgl/ext/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15933 2023-06-21 03:19:58.000000 matgl-0.6.1/matgl/ext/ase.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5278 2023-06-20 15:33:59.000000 matgl-0.6.1/matgl/ext/pymatgen.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 03:35:27.361918 matgl-0.6.1/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       52 2023-06-13 19:01:28.000000 matgl-0.6.1/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5133 2023-06-20 15:44:52.000000 matgl-0.6.1/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)      513 2023-06-13 19:01:28.000000 matgl-0.6.1/matgl/graph/converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11614 2023-06-20 15:52:57.000000 matgl-0.6.1/matgl/graph/data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 03:35:27.363103 matgl-0.6.1/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)      676 2023-06-15 04:03:30.000000 matgl-0.6.1/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2037 2023-06-21 03:34:37.000000 matgl-0.6.1/matgl/layers/_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2983 2023-06-20 15:39:42.000000 matgl-0.6.1/matgl/layers/_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9428 2023-06-20 15:39:42.000000 matgl-0.6.1/matgl/layers/_basis.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2186 2023-06-20 15:39:42.000000 matgl-0.6.1/matgl/layers/_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6029 2023-06-20 15:39:42.000000 matgl-0.6.1/matgl/layers/_core.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3509 2023-06-13 19:01:28.000000 matgl-0.6.1/matgl/layers/_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16602 2023-06-20 15:47:00.000000 matgl-0.6.1/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3872 2023-06-20 15:39:42.000000 matgl-0.6.1/matgl/layers/_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3944 2023-06-20 15:46:20.000000 matgl-0.6.1/matgl/layers/_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 03:35:27.363537 matgl-0.6.1/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      187 2023-06-13 19:01:28.000000 matgl-0.6.1/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11557 2023-06-21 02:47:31.000000 matgl-0.6.1/matgl/models/_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9142 2023-06-21 02:48:19.000000 matgl-0.6.1/matgl/models/_megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2147 2023-06-15 04:29:37.000000 matgl-0.6.1/matgl/models/_wrappers.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 03:35:27.364274 matgl-0.6.1/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       61 2023-06-13 19:01:28.000000 matgl-0.6.1/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      799 2023-06-13 19:01:28.000000 matgl-0.6.1/matgl/utils/cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10520 2023-06-17 15:05:12.000000 matgl-0.6.1/matgl/utils/io.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7129 2023-06-20 15:43:24.000000 matgl-0.6.1/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.6.1/matgl/utils/sb_roots.npy
+-rw-r--r--   0 shyue      (501) staff       (20)    13296 2023-06-21 03:09:33.000000 matgl-0.6.1/matgl/utils/training.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 03:35:27.360418 matgl-0.6.1/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)    12710 2023-06-21 03:35:27.000000 matgl-0.6.1/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)      979 2023-06-21 03:35:27.000000 matgl-0.6.1/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-21 03:35:27.000000 matgl-0.6.1/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-21 03:35:27.000000 matgl-0.6.1/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-21 03:35:27.000000 matgl-0.6.1/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     2427 2023-06-14 21:01:08.000000 matgl-0.6.1/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-21 03:35:27.365072 matgl-0.6.1/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     2018 2023-06-21 03:31:38.000000 matgl-0.6.1/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-21 03:35:27.364399 matgl-0.6.1/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)      194 2023-06-15 14:49:26.000000 matgl-0.6.1/tests/test_config.py
```

### Comparing `matgl-0.6.0/LICENSE` & `matgl-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/PKG-INFO` & `matgl-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.6.0
+Version: 0.6.1
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `matgl-0.6.0/README.md` & `matgl-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/apps/pes.py` & `matgl-0.6.1/matgl/apps/pes.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/config.py` & `matgl-0.6.1/matgl/config.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/data/transformer.py` & `matgl-0.6.1/matgl/data/transformer.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/ext/ase.py` & `matgl-0.6.1/matgl/ext/ase.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,20 +106,20 @@
         g.edata["pbc_offshift"] = torch.matmul(tensor(images), tensor(lattice_matrix))
         return g, state_attr
 
 
 class M3GNetCalculator(Calculator):
     """M3GNet calculator for ASE."""
 
-    implemented_properties = ["energy", "free_energy", "forces", "stress", "hessian"]
+    implemented_properties = ("energy", "free_energy", "forces", "stress", "hessian")
 
     def __init__(
         self,
         potential: Potential,
-        state_attr: torch.Tensor = None,
+        state_attr: torch.Tensor | None = None,
         stress_weight: float = 1.0,
         **kwargs,
     ):
         """
         Init M3GNetCalculator with a Potential.
 
         Args:
@@ -174,16 +174,16 @@
 
 
 class Relaxer:
     """Relaxer is a class for structural relaxation."""
 
     def __init__(
         self,
-        potential: Potential = None,
-        state_attr: torch.Tensor = None,
+        potential: Potential | None = None,
+        state_attr: torch.Tensor | None = None,
         optimizer: Optimizer | str = "FIRE",
         relax_cell: bool = True,
         stress_weight: float = 0.01,
     ):
         """
         Args:
             potential (Potential): a M3GNet potential, a str path to a saved model or a short name for saved model
@@ -210,15 +210,15 @@
         self.ase_adaptor = AseAtomsAdaptor()
 
     def relax(
         self,
         atoms: Atoms,
         fmax: float = 0.1,
         steps: int = 500,
-        traj_file: str = None,
+        traj_file: str | None = None,
         interval=1,
         verbose=False,
         **kwargs,
     ):
         """
         Relax an input Atoms.
 
@@ -308,15 +308,15 @@
 class MolecularDynamics:
     """Molecular dynamics class."""
 
     def __init__(
         self,
         atoms: Atoms,
         potential: Potential,
-        state_attr: torch.Tensor = None,
+        state_attr: torch.Tensor | None = None,
         ensemble: str = "nvt",
         temperature: int = 300,
         timestep: float = 1.0,
         pressure: float = 1.01325 * units.bar,
         taut: float | None = None,
         taup: float | None = None,
         compressibility_au: float | None = None,
```

### Comparing `matgl-0.6.0/matgl/ext/pymatgen.py` & `matgl-0.6.1/matgl/ext/pymatgen.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/graph/compute.py` & `matgl-0.6.1/matgl/graph/compute.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/graph/converters.py` & `matgl-0.6.1/matgl/graph/converters.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/graph/data.py` & `matgl-0.6.1/matgl/graph/data.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/layers/__init__.py` & `matgl-0.6.1/matgl/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/layers/_activations.py` & `matgl-0.6.1/matgl/layers/_activations.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     When x < 0, SoftExponential(x,alpha) = -log(1-alpha(x+alpha))/alpha
     When x = 0, SoftExponential(x,alpha) = 0
     When x > 0, SoftExponential(x,alpha) = (exp(alpha*x)-1)/alpha + alpha.
 
     References: https://arxiv.org/pdf/1602.01321.pdf
     """
 
-    def __init__(self, alpha: float = None):
+    def __init__(self, alpha: float | None = None):
         """
         Init SoftExponential with alpha value.
 
         Args:
             alpha (float): adjustable Torch parameter during the training.
         """
         super().__init__()
```

### Comparing `matgl-0.6.0/matgl/layers/_atom_ref.py` & `matgl-0.6.1/matgl/layers/_atom_ref.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/layers/_basis.py` & `matgl-0.6.1/matgl/layers/_basis.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/layers/_bond.py` & `matgl-0.6.1/matgl/layers/_bond.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/layers/_core.py` & `matgl-0.6.1/matgl/layers/_core.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/layers/_embedding.py` & `matgl-0.6.1/matgl/layers/_embedding.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/layers/_graph_convolution.py` & `matgl-0.6.1/matgl/layers/_graph_convolution.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/layers/_readout.py` & `matgl-0.6.1/matgl/layers/_readout.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/layers/_three_body.py` & `matgl-0.6.1/matgl/layers/_three_body.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/models/_m3gnet.py` & `matgl-0.6.1/matgl/models/_m3gnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         niters_set2set: int = 3,
         nlayers_set2set: int = 3,
         field: str = "node_feat",
         include_state: bool = False,
         activation_type: str = "swish",
         **kwargs,
     ):
-        r"""
+        """
         Args:
             element_types (tuple): list of elements appearing in the dataset
             dim_node_embedding (int): number of embedded atomic features
             dim_edge_embedding (int): number of edge features
             dim_state_embedding (int): number of hidden neurons in state embedding
             dim_state_feats (int): number of state features after linear layer
             dim_state_types (int): number of state labels
```

### Comparing `matgl-0.6.0/matgl/models/_megnet.py` & `matgl-0.6.1/matgl/models/_megnet.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,15 +41,14 @@
         hidden_layer_sizes_output: tuple[int, ...] = (32, 16),
         nlayers_set2set: int = 1,
         niters_set2set: int = 2,
         activation_type: str = "softplus2",
         is_classification: bool = False,
         include_state: bool = True,
         dropout: float | None = None,
-        graph_transformations: list | None = None,
         element_types: tuple[str, ...] = DEFAULT_ELEMENT_TYPES,
         bond_expansion: BondExpansion | None = None,
         cutoff: float = 4.0,
         gauss_width: float = 0.5,
         **kwargs,
     ):
         """Useful defaults for all arguments have been specified based on MEGNet formation energy model.
@@ -69,16 +68,14 @@
             is_classification: Whether this is classification task or not
             layer_node_embedding: Architecture of embedding layer for node attributes
             layer_edge_embedding: Architecture of embedding layer for edge attributes
             layer_state_embedding: Architecture of embedding layer for state attributes
             include_state: Whether the state embedding is included
             dropout: Randomly zeroes some elements in the input tensor with given probability (0 < x < 1) according to
                 a Bernoulli distribution
-            graph_transformations: Perform a graph transformation, e.g., incorporate three-body interactions, prior to
-                performing the GCL updates.
             element_types: Elements included in the training set
             bond_expansion: Gaussian expansion for edge attributes
             cutoff: cutoff for forming bonds
             gauss_width: width of Gaussian function for bond expansion
             **kwargs: For future flexibility. Not used at the moment.
         """
         super().__init__()
@@ -147,15 +144,14 @@
             activation=activation,
             activate_last=False,
         )
 
         self.dropout = nn.Dropout(dropout) if dropout else None
 
         self.is_classification = is_classification
-        self.graph_transformations = graph_transformations or [nn.Identity()] * nblocks
         self.include_state_embedding = include_state
 
     def forward(
         self,
         graph: dgl.DGLGraph,
         edge_feat: torch.Tensor,
         node_feat: torch.Tensor,
@@ -168,22 +164,21 @@
             edge_feat: Edge features
             node_feat: Node features
             state_feat: State features.
 
         Returns:
             Prediction
         """
-        graph_transformations = self.graph_transformations
         node_feat, edge_feat, state_feat = self.embedding(node_feat, edge_feat, state_feat)
         edge_feat = self.edge_encoder(edge_feat)
         node_feat = self.node_encoder(node_feat)
         state_feat = self.state_encoder(state_feat)
 
-        for gt, block in zip(graph_transformations, self.blocks):
-            output = block(gt(graph), edge_feat, node_feat, state_feat)
+        for block in self.blocks:
+            output = block(graph, edge_feat, node_feat, state_feat)
             edge_feat, node_feat, state_feat = output
 
         node_vec = self.node_s2s(graph, node_feat)
         edge_vec = self.edge_s2s(graph, edge_feat)
 
         node_vec = torch.squeeze(node_vec)
         edge_vec = torch.squeeze(edge_vec)
```

### Comparing `matgl-0.6.0/matgl/models/_wrappers.py` & `matgl-0.6.1/matgl/models/_wrappers.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/utils/cutoff.py` & `matgl-0.6.1/matgl/utils/cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/utils/io.py` & `matgl-0.6.1/matgl/utils/io.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/utils/maths.py` & `matgl-0.6.1/matgl/utils/maths.py`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/utils/sb_roots.npy` & `matgl-0.6.1/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/matgl/utils/training.py` & `matgl-0.6.1/matgl/utils/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,26 +208,27 @@
         """
         g, labels, state_attr = batch
         preds = self(g=g, state_attr=state_attr)
         results = self.loss_fn(loss=self.loss, preds=preds, labels=labels)  # type: ignore
         batch_size = preds.numel()
         return results, batch_size
 
-    def loss_fn(self, loss: nn.Module, labels: tuple, preds: tuple):
+    def loss_fn(self, loss: nn.Module, labels: torch.Tensor, preds: torch.Tensor):
         """Args:
             loss: Loss function.
             labels: Labels to compute the loss.
             preds: Predictions.
 
         Returns:
             {"Total_Loss": total_loss, "MAE": mae, "RMSE": rmse}
         """
-        total_loss = loss(labels, torch.squeeze(preds * self.data_std + self.data_mean))
-        mae = self.mae(labels, torch.squeeze(preds * self.data_std + self.data_mean))
-        rmse = self.rmse(labels, torch.squeeze(preds * self.data_std + self.data_mean))
+        scaled_pred = torch.reshape(preds * self.data_std + self.data_mean, labels.size())
+        total_loss = loss(labels, scaled_pred)
+        mae = self.mae(labels, scaled_pred)
+        rmse = self.rmse(labels, scaled_pred)
         return {"Total_Loss": total_loss, "MAE": mae, "RMSE": rmse}
 
 
 class PotentialLightningModule(MatglLightningModuleMixin, pl.LightningModule):
     """A PyTorch.LightningModule for training MatGL potentials.
 
     This is slightly different from the ModelLightningModel due to the need to account for energy, forces and stress
```

### Comparing `matgl-0.6.0/matgl.egg-info/PKG-INFO` & `matgl-0.6.1/matgl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.6.0
+Version: 0.6.1
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `matgl-0.6.0/matgl.egg-info/SOURCES.txt` & `matgl-0.6.1/matgl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/pyproject.toml` & `matgl-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matgl-0.6.0/setup.py` & `matgl-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="matgl",
-    version="0.6.0",
+    version="0.6.1",
     author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong",
     author_email="t1ko@ucsd.edu, ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     maintainer_email="ongsp@ucsd.edu",
     description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

