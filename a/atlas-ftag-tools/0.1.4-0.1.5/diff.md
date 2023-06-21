# Comparing `tmp/atlas-ftag-tools-0.1.4.tar.gz` & `tmp/atlas-ftag-tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-ftag-tools-0.1.4.tar", last modified: Fri May 19 12:34:10 2023, max compression
+gzip compressed data, was "atlas-ftag-tools-0.1.5.tar", last modified: Wed Jun 21 15:59:56 2023, max compression
```

## Comparing `atlas-ftag-tools-0.1.4.tar` & `atlas-ftag-tools-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:34:10.236859 atlas-ftag-tools-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-19 12:34:10.236859 atlas-ftag-tools-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:34:10.232859 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-19 12:34:10.000000 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-19 12:34:10.000000 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:34:10.000000 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-19 12:34:10.000000 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-19 12:34:10.000000 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 12:34:10.000000 atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:34:10.236859 atlas-ftag-tools-0.1.4/ftag/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/flavour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/flavours.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:34:10.236859 atlas-ftag-tools-0.1.4/ftag/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/hdf5/h5reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/hdf5/h5utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/hdf5/h5writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/vds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:34:10.236859 atlas-ftag-tools-0.1.4/ftag/wps/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/wps/discriminant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/ftag/wps/working_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-19 12:33:49.000000 atlas-ftag-tools-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:34:10.236859 atlas-ftag-tools-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:59:56.723033 atlas-ftag-tools-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-21 15:59:56.719033 atlas-ftag-tools-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:59:56.719033 atlas-ftag-tools-0.1.5/atlas_ftag_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-21 15:59:56.000000 atlas-ftag-tools-0.1.5/atlas_ftag_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-21 15:59:56.000000 atlas-ftag-tools-0.1.5/atlas_ftag_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:59:56.000000 atlas-ftag-tools-0.1.5/atlas_ftag_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 15:59:56.000000 atlas-ftag-tools-0.1.5/atlas_ftag_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 15:59:56.000000 atlas-ftag-tools-0.1.5/atlas_ftag_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 15:59:56.000000 atlas-ftag-tools-0.1.5/atlas_ftag_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:59:56.719033 atlas-ftag-tools-0.1.5/ftag/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/flavour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/flavours.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:59:56.719033 atlas-ftag-tools-0.1.5/ftag/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/hdf5/h5reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/hdf5/h5utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/hdf5/h5writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/vds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:59:56.719033 atlas-ftag-tools-0.1.5/ftag/wps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/wps/discriminant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/ftag/wps/working_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-21 15:59:35.000000 atlas-ftag-tools-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:59:56.723033 atlas-ftag-tools-0.1.5/setup.cfg
```

### Comparing `atlas-ftag-tools-0.1.4/PKG-INFO` & `atlas-ftag-tools-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-ftag-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: ATLAS Flavour Tagging Tools
 Author: Sam Van Stroud, Philipp Gadow
 License: MIT
 Project-URL: Homepage, https://github.com/umami-hep/atlas-ftag-tools/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `atlas-ftag-tools-0.1.4/README.md` & `atlas-ftag-tools-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/PKG-INFO` & `atlas-ftag-tools-0.1.5/atlas_ftag_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-ftag-tools
-Version: 0.1.4
+Version: 0.1.5
 Summary: ATLAS Flavour Tagging Tools
 Author: Sam Van Stroud, Philipp Gadow
 License: MIT
 Project-URL: Homepage, https://github.com/umami-hep/atlas-ftag-tools/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `atlas-ftag-tools-0.1.4/atlas_ftag_tools.egg-info/SOURCES.txt` & `atlas-ftag-tools-0.1.5/atlas_ftag_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.4/ftag/__init__.py` & `atlas-ftag-tools-0.1.5/ftag/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """atlas-ftag-tools - Common tools for ATLAS flavour tagging software."""
 
 
-__version__ = "v0.1.4"
+__version__ = "v0.1.5"
 
 
 import ftag.hdf5 as hdf5
 from ftag.cuts import Cuts
 from ftag.flavour import Flavour, Flavours
 from ftag.mock import get_mock_file
 from ftag.sample import Sample
```

### Comparing `atlas-ftag-tools-0.1.4/ftag/cuts.py` & `atlas-ftag-tools-0.1.5/ftag/cuts.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.4/ftag/flavour.py` & `atlas-ftag-tools-0.1.5/ftag/flavour.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.4/ftag/flavours.yaml` & `atlas-ftag-tools-0.1.5/ftag/flavours.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -45,20 +45,20 @@
   cuts: ["HadronConeExclExtendedTruthLabelID == 44"]
   label: $cc$-jets
   colour: gold
   category: single-btag-extended
 
 # Xbb tagging
 - name: hbb
-  label: Hbb
+  label: $H \rightarrow b\bar{b}$
   cuts: ["R10TruthLabel_R22v1 == 11"]
   colour: tab:blue
   category: xbb
 - name: hcc
-  label: Hcc
+  label: $H \rightarrow c\bar{c}$
   cuts: ["R10TruthLabel_R22v1 == 12"]
   colour: "#B45F06"
   category: xbb
 - name: top
   label: Top
   cuts: ["R10TruthLabel_R22v1 == 1"]
   colour: "#A300A3"
```

### Comparing `atlas-ftag-tools-0.1.4/ftag/hdf5/h5reader.py` & `atlas-ftag-tools-0.1.5/ftag/hdf5/h5reader.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,17 +22,18 @@
     jets_name: str = "jets"
     precision: str | None = None
     shuffle: bool = True
     do_remove_inf: bool = False
 
     def __post_init__(self) -> None:
         self.sample = Sample(self.fname)
-        if len(self.sample.virtual_file()) != 1:
+        fname = self.sample.virtual_file()
+        if len(fname) != 1:
             raise ValueError("H5SingleReader should only read a single file")
-        self.fname = self.sample.virtual_file()[0]
+        self.fname = fname[0]
 
     @cached_property
     def num_jets(self) -> int:
         with h5py.File(self.fname) as f:
             return len(f[self.jets_name])
 
     def get_attr(self, name, group=None):
@@ -53,29 +54,35 @@
     def remove_inf(self, data: dict) -> dict:
         keep_idx = np.full(len(data[self.jets_name]), True)
         for name, array in data.items():
             for var in array.dtype.names:
                 isinf = np.isinf(array[var])
                 keep_idx = keep_idx & ~isinf.any(axis=-1)
                 if num_inf := isinf.sum():
-                    log.warn(
+                    log.warning(
                         f"{num_inf} inf values detected for variable {var} in"
                         f" {name} array. Removing the affected jets."
                     )
         return {name: array[keep_idx] for name, array in data.items()}
 
     def stream(
-        self, variables: dict | None = None, num_jets: int | None = None, cuts: Cuts | None = None
+        self,
+        variables: dict | None = None,
+        num_jets: int | None = None,
+        cuts: Cuts | None = None,
     ) -> Generator:
         if num_jets is None:
             num_jets = self.num_jets
+
         if num_jets > self.num_jets:
-            raise ValueError(
-                f"{num_jets:,} jets requested but only {self.num_jets:,} available in {self.fname}"
+            log.warning(
+                f"{num_jets:,} jets requested but only {self.num_jets:,} available in {self.fname}."
+                " Set to maximum available number!"
             )
+            num_jets = self.num_jets
 
         if variables is None:
             variables = {self.jets_name: None}
 
         total = 0
         rng = np.random.default_rng(42)
         with h5py.File(self.fname) as f:
@@ -127,25 +134,36 @@
         Cast floats to given precision, by default None
     shuffle : bool, optional
         Read batches in a shuffled order, by default True
     weights : list[float] | None, optional
         Weights for different input datasets, by default None
     do_remove_inf : bool, optional
         Remove jets with inf values, by default False
+    equal_jets : bool, optional
+        Take the same number of jets (weighted) from each sample, by default True
+        If False, use all jets in each sample.
     """
 
     fname: Path | str | list[Path | str]
     batch_size: int = 100_000
     jets_name: str = "jets"
     precision: str | None = None
     shuffle: bool = True
     weights: list[float] | None = None
     do_remove_inf: bool = False
+    equal_jets: bool = True
 
     def __post_init__(self) -> None:
+        if not self.equal_jets:
+            log.warning(
+                "equal_jets is set to False, which will result in different number of jets taken"
+                " from each sample. Be aware that this can affect the resampling, so make sure you"
+                " know what you are doing."
+            )
+
         if isinstance(self.fname, (str, Path)):
             self.fname = [self.fname]
 
         # calculate batch sizes
         if self.weights is None:
             self.weights = [1 / len(self.fname)] * len(self.fname)
         self.batch_sizes = [int(w * self.batch_size) for w in self.weights]
@@ -187,60 +205,124 @@
             Selection cuts to apply, by default None
 
         Yields
         ------
         Generator
             Generator of batches of selected jets.
         """
+        # Check if number of jets is given, if not, set to maximum available
         if num_jets is None:
             num_jets = self.num_jets
+
+        # Check if variables if given, if not, set to all
         if variables is None:
             variables = {self.jets_name: None}
+
         if self.jets_name not in variables or variables[self.jets_name] is not None:
             jet_vars = variables.get(self.jets_name, [])
             variables[self.jets_name] = list(jet_vars) + (cuts.variables if cuts else [])
 
         # get streams for selected jets from each reader
         streams = [
             r.stream(variables, int(r.num_jets / self.num_jets * num_jets), cuts)
             for r in self.readers
         ]
 
         rng = np.random.default_rng(42)
         while True:
-            # yeild from each stream
             samples = []
-            for stream in streams:
-                try:
-                    samples.append(next(stream))
-                except StopIteration:
+            # Track which streams have been exhausted
+            streams_done = [False] * len(streams)
+
+            # for each unexhausted stream, get the next sample
+            for i, stream in enumerate(streams):
+                if not streams_done[i]:
+                    try:
+                        samples.append(next(stream))
+
+                    # if equal_jets is True, we can stop when any stream is done
+                    # otherwise if sample is exhausted, mark it as done
+                    except StopIteration:
+                        if self.equal_jets:
+                            return
+                        streams_done[i] = True
+
+                # if equal_jets is False, we need to keep going until all streams are done
+                if all(streams_done):
                     return
 
             # combine samples and shuffle
             data = {name: np.concatenate([s[name] for s in samples]) for name in variables}
             if self.shuffle:
                 idx = np.arange(len(data[self.jets_name]))
                 rng.shuffle(idx)
                 data = {name: array[idx] for name, array in data.items()}
 
-            # select
+            # yield batch
             yield data
 
     def load(
         self, variables: dict | None = None, num_jets: int | None = None, cuts: Cuts | None = None
     ) -> dict:
+        """Load multiple batches of selected jets into memory.
+
+        Parameters
+        ----------
+        variables : dict | None, optional
+            Dictionary of variables to for each group, by default use all jet variables.
+        num_jets : int | None, optional
+            Total number of selected jets to load, by default all.
+        cuts : Cuts | None, optional
+            Selection cuts to apply, by default None
+
+        Returns
+        -------
+        dict
+            Dictionary of arrays for each group.
+        """
+        # handle default arguments
         if num_jets == -1:
             num_jets = self.num_jets
         if variables is None:
             variables = {self.jets_name: None}
+
+        # get data from each sample
         data: dict[str, list] = {name: [] for name in variables}
-        for sample in self.stream(variables, num_jets, cuts):
-            for name, array in sample.items():
+        for batch in self.stream(variables, num_jets, cuts):
+            for name, array in batch.items():
                 if name in data:
                     data[name].append(array)
+
+        # concatenate batches
         return {name: np.concatenate(array) for name, array in data.items()}
 
     def estimate_available_jets(self, cuts: Cuts, num: int = 1_000_000) -> int:
-        """Estimate the number of jets available after selection cuts, rounded down."""
-        all_jets = self.load({self.jets_name: cuts.variables}, num)[self.jets_name]
-        estimated_num_jets = len(cuts(all_jets).values) / len(all_jets) * self.num_jets
+        """Estimate the number of jets available after selection cuts (round down).
+
+        Parameters
+        ----------
+        cuts : Cuts
+            Selection cuts to apply.
+        num : int, optional
+            Number of jets to use for the estimation, by default 1_000_000.
+
+        Returns
+        -------
+        int
+            Estimated number of jets available after selection cuts,
+            rounded down to nearest thousand.
+        """
+        # if equal jets is True, available jets is based on the smallest sample
+        if self.equal_jets:
+            num_jets = []
+            for r in self.readers:
+                stream = r.stream({self.jets_name: cuts.variables}, num)
+                all_jets = np.concatenate([batch[self.jets_name] for batch in stream])
+                frac_selected = len(cuts(all_jets).values) / len(all_jets)
+                num_jets.append(frac_selected * r.num_jets)
+            estimated_num_jets = min(num_jets) * len(self.readers)
+        # otherwise, available jets is based on all samples
+        else:
+            all_jets = self.load({self.jets_name: cuts.variables}, num)[self.jets_name]
+            frac_selected = len(cuts(all_jets).values) / len(all_jets)
+            estimated_num_jets = frac_selected * self.num_jets
         return math.floor(estimated_num_jets / 1_000) * 1_000
```

### Comparing `atlas-ftag-tools-0.1.4/ftag/hdf5/h5utils.py` & `atlas-ftag-tools-0.1.5/ftag/hdf5/h5utils.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.4/ftag/hdf5/h5writer.py` & `atlas-ftag-tools-0.1.5/ftag/hdf5/h5writer.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.4/ftag/mock.py` & `atlas-ftag-tools-0.1.5/ftag/mock.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.4/ftag/sample.py` & `atlas-ftag-tools-0.1.5/ftag/sample.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.4/ftag/vds.py` & `atlas-ftag-tools-0.1.5/ftag/vds.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.4/ftag/wps/discriminant.py` & `atlas-ftag-tools-0.1.5/ftag/wps/discriminant.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.4/ftag/wps/working_points.py` & `atlas-ftag-tools-0.1.5/ftag/wps/working_points.py`

 * *Files identical despite different names*

### Comparing `atlas-ftag-tools-0.1.4/pyproject.toml` & `atlas-ftag-tools-0.1.5/pyproject.toml`

 * *Files identical despite different names*

