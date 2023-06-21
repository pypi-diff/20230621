# Comparing `tmp/emdfile-0.0.8.tar.gz` & `tmp/emdfile-0.0.9.tar.gz`

## Comparing `emdfile-0.0.8.tar` & `emdfile-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,39 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.8/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.8/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.8/.pytest_cache/README.md
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 emdfile-0.0.8/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 emdfile-0.0.8/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.8/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/__init__.py
--rw-r--r--   0        0        0    10788 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/read.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/tqdmnd.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/version.py
--rw-r--r--   0        0        0    31055 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/write.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/array.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/custom.py
--rw-r--r--   0        0        0    10379 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/metadata.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/pointlist.py
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/pointlistarray.py
--rw-r--r--   0        0        0    23911 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/tree.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/utils.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/clear_h5_files.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/test_base_classes.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/test_emd.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/test_header.py
--rw-r--r--   0        0        0    28996 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/test_tree.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0   384837 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/emdfile_intro_example.ipynb
--rw-r--r--   0        0        0   167826 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/emdfile_package_walkthrough.ipynb
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/test_custom_classes.py
--rw-r--r--   0        0        0    81358 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/pngs/node.png
--rw-r--r--   0        0        0    41590 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/pngs/tree.png
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/sample_custom_emd_classes/__init__.py
--rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/sample_custom_emd_classes/custom_class_TEMPLATE.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/sample_custom_emd_classes/my_custom_classes.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 emdfile-0.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emdfile-0.0.8/LICENSE
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 emdfile-0.0.8/README.md
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 emdfile-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 emdfile-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 emdfile-0.0.9/src/emdfile/__init__.py
+-rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 emdfile-0.0.9/src/emdfile/read.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 emdfile-0.0.9/src/emdfile/tqdmnd.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 emdfile-0.0.9/src/emdfile/version.py
+-rw-r--r--   0        0        0    31063 2020-02-02 00:00:00.000000 emdfile-0.0.9/src/emdfile/write.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 emdfile-0.0.9/src/emdfile/classes/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 emdfile-0.0.9/src/emdfile/classes/array.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 emdfile-0.0.9/src/emdfile/classes/custom.py
+-rw-r--r--   0        0        0    10379 2020-02-02 00:00:00.000000 emdfile-0.0.9/src/emdfile/classes/metadata.py
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 emdfile-0.0.9/src/emdfile/classes/pointlist.py
+-rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 emdfile-0.0.9/src/emdfile/classes/pointlistarray.py
+-rw-r--r--   0        0        0    23877 2020-02-02 00:00:00.000000 emdfile-0.0.9/src/emdfile/classes/tree.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 emdfile-0.0.9/src/emdfile/classes/utils.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 emdfile-0.0.9/test/clear_h5_files.py
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 emdfile-0.0.9/test/test_base_classes.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 emdfile-0.0.9/test/test_emd.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 emdfile-0.0.9/test/test_header.py
+-rw-r--r--   0        0        0    29168 2020-02-02 00:00:00.000000 emdfile-0.0.9/test/test_tree.py
+-rw-r--r--   0        0        0   384837 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/emdfile_intro_example.ipynb
+-rw-r--r--   0        0        0   167826 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/emdfile_package_walkthrough.ipynb
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/test_custom_classes.py
+-rw-r--r--   0        0        0    81358 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/pngs/node.png
+-rw-r--r--   0        0        0    41590 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/pngs/tree.png
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/sample_custom_emd_classes/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/sample_custom_emd_classes/array_subclass_TEMPLATE.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/sample_custom_emd_classes/array_subclass_sample1.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/sample_custom_emd_classes/array_subclass_sample2.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/sample_custom_emd_classes/custom_subclass_TEMPLATE.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/sample_custom_emd_classes/custom_subclass_sample.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/sample_custom_emd_classes/my_custom_classes.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/sample_custom_emd_classes/points_subclass_TEMPLATE.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/sample_custom_emd_classes/points_subclass_sample.py
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/sample_custom_emd_classes/raggedarray_subclass_TEMPLATE.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 emdfile-0.0.9/tutorials/sample_custom_emd_classes/raggedarray_subclass_sample.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 emdfile-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emdfile-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 emdfile-0.0.9/README.md
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 emdfile-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 emdfile-0.0.9/PKG-INFO
```

### Comparing `emdfile-0.0.8/src/emdfile/__init__.py` & `emdfile-0.0.9/src/emdfile/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 # classes
 
 from emdfile.classes import (
     Metadata,
     Node,
     Root,
-    RootedNode,
     Array,
     PointList,
     PointListArray,
     Custom
 )
```

### Comparing `emdfile-0.0.8/src/emdfile/read.py` & `emdfile-0.0.9/src/emdfile/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import warnings
 
 
 # Classes
 from emdfile.classes import (
     Root,
     Node,
-    RootedNode,
     Metadata
 )
 from emdfile.classes.utils import (
     _get_class,
     EMD_data_group_types
 )
 
@@ -275,20 +274,15 @@
     keys = [k for k in keys if group[k].attrs['emd_group_type'] in \
         EMD_data_group_types]
 
     for key in keys:
         #print(f"Reading group {group[key].name}")
         new_node = _read_single_node(group[key])
         count += 1
-        # Handle RootedNodes, which need to be grafted rather than added
-        if isinstance(new_node,RootedNode):
-            new_node.graft(node)
-            new_node._add_root_links(node)
-        else:
-            node.add_to_tree(new_node)
+        node.add_to_tree(new_node)
         _populate_tree(
             new_node,
             group[key],
             count = count
         )
     return count
```

### Comparing `emdfile-0.0.8/src/emdfile/tqdmnd.py` & `emdfile-0.0.9/src/emdfile/tqdmnd.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/src/emdfile/write.py` & `emdfile-0.0.9/src/emdfile/write.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     # `data` should now be a Node!
     assert(isinstance(data,Node)), f"invalid type {type(data)} found for `data`"
 
     # handle rootless data
     added_a_root = False
     if data._root is None:
         added_a_root = True
-        root = Root(name=data.name)
+        root = Root(name=data.name+"_root")
         root.add_to_tree(data)
     else:
         # get the root
         root = data.root
```

### Comparing `emdfile-0.0.8/src/emdfile/classes/array.py` & `emdfile-0.0.9/src/emdfile/classes/array.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/src/emdfile/classes/custom.py` & `emdfile-0.0.9/src/emdfile/classes/custom.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/src/emdfile/classes/metadata.py` & `emdfile-0.0.9/src/emdfile/classes/metadata.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/src/emdfile/classes/pointlist.py` & `emdfile-0.0.9/src/emdfile/classes/pointlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,19 @@
         super().__init__()
 
         # populate data and metadata
         self.data = data
         self.name = name
         self._dtype = self.data.dtype
         self._fields = self.data.dtype.names
-        self._types = tuple([self.data.dtype.fields[f][0] for f in self.fields])
-
+        if self._fields is not None:
+            self._types = tuple([self.data.dtype.fields[f][0] for f in self.fields])
+        else:
+            self._fields = ('',)
+            self._types = (self._dtype,)
 
 
     # properties
     @property
     def dtype(self):
         return self._dtype
     @dtype.setter
@@ -61,30 +64,42 @@
         self.data.dtype.names = x
         self._fields = x
 
     @property
     def types(self):
         return self._types
 
+    def __len__(self):
+        return np.atleast_1d(self.data).shape[0]
     @property
     def length(self):
-        return np.atleast_1d(self.data).shape[0]
-
+        return len(self)
 
 
     ## Add, remove, sort data
 
-    def add(self, data):
+    def __add__(self, data):
         """
-        Appends a numpy structured array. Its dtypes must agree with the existing data.
+        Append a numpy structured array and return the concatenated pointlist.
+        The dtypes must agree.
         """
         assert self.dtype == data.dtype, "Error: dtypes must agree"
         if isinstance(data,PointList):
             data = data.data
-        self.data = np.append(self.data, data)
+        ans = np.append(self.data, data)
+        return PointList(
+            name = self.name,
+            data = ans
+        )
+
+    def add(self, data):
+        """
+        Appends a numpy structured array. Its dtypes must agree with the existing data.
+        """
+        self.data = (self + data).data
 
     def remove(self, mask):
         """ Removes points wherever mask==True
         """
         assert np.atleast_1d(mask).shape[0] == self.length, "deletemask must be same length as the data"
         inds = mask.nonzero()[0]
         self.data = np.delete(self.data, inds)
```

### Comparing `emdfile-0.0.8/src/emdfile/classes/pointlistarray.py` & `emdfile-0.0.9/src/emdfile/classes/pointlistarray.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,44 +37,48 @@
         super().__init__()
 
         self.name = name
         self.shape = shape
 
         self.dtype = np.dtype(dtype)
         self.fields = self.dtype.names
-        self.types = tuple([self.dtype.fields[f][0] for f in self.fields])
+        if self.fields is not None:
+            self.types = tuple([self.dtype.fields[f][0] for f in self.fields])
+        else:
+            self.fields = ('',)
+            self.types = (dtype,)
 
 
         # Populate with empty PointLists
         self._pointlists = [[PointList(data=np.zeros(0,dtype=self.dtype), name=f"{i},{j}")
                              for j in range(self.shape[1])] for i in range(self.shape[0])]
 
 
     ## get/set pointlists
 
-    def get_pointlist(self, i, j, name=None):
-        """
-        Returns the pointlist at i,j
-        """
-        pl = self._pointlists[i][j]
-        if name is not None:
-            pl = pl.copy(name=name)
-        return pl
-
     def __getitem__(self, tup):
         l = len(tup) if isinstance(tup,tuple) else 1
         assert(l==2), f"Expected 2 slice values, recieved {l}"
         return self.get_pointlist(tup[0],tup[1])
 
     def __setitem__(self, tup, pointlist):
         l = len(tup) if isinstance(tup,tuple) else 1
         assert(l==2), f"Expected 2 slice values, recieved {l}"
         assert(pointlist.fields == self.fields), "fields must match"
         self._pointlists[tup[0]][tup[1]] = pointlist
 
+    def get_pointlist(self, i, j, name=None):
+        """
+        Returns the pointlist at i,j
+        """
+        pl = self._pointlists[i][j]
+        if name is not None:
+            pl = pl.copy(name=name)
+        return pl
+
 
 
     ## Make copies
 
     def copy(self, name=''):
         """
         Returns a copy of itself.
```

### Comparing `emdfile-0.0.8/src/emdfile/classes/tree.py` & `emdfile-0.0.9/src/emdfile/classes/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,28 +215,33 @@
         if name == '':
             return self.root
         elif name[0] != '/':
             return self._branch[name]
         else:
             return self.root._branch[name]
 
-    def graft(self,node,merge_metadata=True):
+    def _graft(self,node,merge_metadata=True):
         """
-        Moves a branch from one tree, starting at this node,
-        onto another tree at target `node`.
+        Moves the branch beginning at this node onto another tree at
+        targed point `node`.
+
+        This is the reverse of the behavior of self.graft(node), which moves
+        the branch on some other tree beginning at `node` onto this tree
+        starting at this node. In other words, self.graft() grafts onto self,
+        while self._graft() grafts from self.
 
         Accepts:
             node (Node):
             merge_metadata (True, False, or 'copy'): if True adds the old root's
                 metadata to the new root; if False adds no metadata to the new
                 root; if 'copy' adds copies of all metadata from the old root to
                 the new root.
 
         Returns:
-            (Node) the new tree's root node
+            (Node) the root node of the receiving tree
         """
         assert(self.root is not None), "Can't graft an unrooted node; try using .tree(add=node) instead."
         assert(node.root is not None), "Can't graft onto an unrooted node"
 
         # find upstream and root nodes
         old_root = self.root
         node_list = self._treepath.split('/')
@@ -263,16 +268,14 @@
             for k in keys:
                 n = upstream_node.tree(k)
                 n._root = None
                 node.add_to_tree(n)
                 # remove upstream connections
                 del(upstream_node._branch[k])
 
-#                upstream_node.tree(k).graft(node, merge_metadata=False)
-
 
         # add old root metadata to this node
         assert(merge_metadata in [True,False,'copy'])
         if merge_metadata is False:
             # add no root metadata
             pass
         elif merge_metadata is True:
@@ -282,14 +285,35 @@
         else:
             # add copies of old root metadata to new root
             for key in old_root.metadata.keys():
                 node.root.metadata = old_root.metadata[key].copy()
         # return
         return node.root
 
+
+    def graft(self,node,merge_metadata=True):
+        """
+        Moves the branch beginning node onto this tree at this node.
+
+        For the reverse (i.e. grafting from this tree onto another tree)
+        either use that tree's .graft method, or use this tree's ._graft.
+
+        Accepts:
+            node (Node):
+            merge_metadata (True, False, or 'copy'): if True adds the old root's
+                metadata to the new root; if False adds no metadata to the new
+                root; if 'copy' adds copies of all metadata from the old root to
+                the new root.
+
+        Returns:
+            (Node) this tree's root node
+        """
+        return node._graft(self)
+
+
     def cut_from_tree(self,root_metadata=True):
         """
         Removes a branch from an object tree at this node.
 
         A new root node is created under this object
         with this object's name.  Metadata from
         the current root is transferred/not transferred
@@ -301,15 +325,15 @@
                 root; if 'copy' adds copies of all metadata from the old root to
                 the new root.
 
         Returns:
             (Node) the new root node
         """
         new_root = Root( name=self.root.name+'_cut_'+self.name)
-        return self.graft(new_root,merge_metadata=root_metadata)
+        return self._graft(new_root,merge_metadata=root_metadata)
 
 
     def tree(
         self,
         arg = None,
         **kwargs,
         ):
@@ -321,15 +345,15 @@
             >>> .tree(show=False)   # show from current node
             >>> .tree(add=node)     # add a child node
             >>> .tree(get='path')   # return a '/' delimited child node
             >>> .tree(get='/path')  # as above, starting at root
             >>> .tree(cut=True)     # remove/return a branch, keep root metadata
             >>> .tree(cut=False)    # remove/return a branch, discard root md
             >>> .tree(cut='copy')   # remove/return a branch, copy root metadata
-            >>> .tree(graft=node)   # remove/graft a branch, keep root metadata
+            >>> .tree(graft=node)   # remove/graft a branch, keeping root metadata
             >>> .tree(graft=(node,True))    # as above
             >>> .tree(graft=(node,False))   # as above, discard root metadata
             >>> .tree(graft=(node,'copy'))  # as above, copy root metadata
 
         The show, add, and get methods can be accessed directly with
 
             >>> .tree(arg)
@@ -582,39 +606,14 @@
         self._treepath = ''
         self._root = self
 
 
 
 
 
-class RootedNode:
-
-    """
-    RootedNodes are nodes that are required to have a root. When __init__
-    is run, if a root doesn't already exist, it creates one with its own
-    name and attaches to it.
-    """
-
-    def __init__(self):
-        assert(hasattr(self,'root')), "RootedNode must already be initialized as a Node"
-        if self.root is None:
-            root = Root( name = self.name )
-            root.add_to_tree( self )
-
-
-    def _add_root_links(self,node):
-        """
-        This method is run while reading from a file, after a new instance has
-        been created and grafted from it's own root onto the tree from its H5
-        file of origin. This is useful for linking to other data/metadata
-        in the tree, which are not available earlier in the read process (and
-        which may need to be overwritted because they're obligate attrs which
-        were generated in initialization)
-        """
-        pass
 
 
 
 
 
 class Branch:
```

### Comparing `emdfile-0.0.8/src/emdfile/classes/utils.py` & `emdfile-0.0.9/src/emdfile/classes/utils.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/test/clear_h5_files.py` & `emdfile-0.0.9/test/clear_h5_files.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/test/test_emd.py` & `emdfile-0.0.9/test/test_emd.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/test/test_header.py` & `emdfile-0.0.9/test/test_header.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/test/test_tree.py` & `emdfile-0.0.9/test/test_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,37 +320,49 @@
 
     def test_graft(self):
         """
         Confirms correct grafting behavior
         """
         # make a new tree to graft onto
         new_root = self.pl4.tree(cut=True)
-        # graft from the old tree to the new one
-        self.pla.tree(graft=self.pl4)
-        assert(new_root.tree('pointlist4/pointlistarray/pointlist') == self.pl)
+        # graft
+        self.pla.tree( graft=new_root.tree('pointlist4') )
+        # check
+        data = self.root.tree('array/pointlistarray/pointlist4')
+        assert(isinstance(data,PointList))
+        assert(data == self.pl4)
 
     def test_graft2(self):
         """
         Confirms correct grafting behavior with alternative syntax
         """
         # make a new tree to graft onto
         new_root = self.pl4.tree(cut=True)
-        # graft from the old tree to the new one
-        self.pla.graft(self.pl4) # alt syntax
-        assert(new_root.tree('pointlist4/pointlistarray/pointlist') == self.pl)
+        # graft
+        self.pla.graft( new_root.tree('pointlist4') )
+        # check
+        data = self.root.tree('array/pointlistarray/pointlist4')
+        assert(isinstance(data,PointList))
+        assert(data == self.pl4)
+
+
 
     def test_graft3(self):
         """
         Confirms correct grafting behavior with alternative syntax
         """
         # make a new tree to graft onto
         new_root = self.pl4.tree(cut=True)
-        # graft from the old tree to the new one
-        self.pla.tree(graft=(self.pl4,True)) # alt syntax
-        assert(new_root.tree('pointlist4/pointlistarray/pointlist') == self.pl)
+        # graft
+        self.pla.tree( graft=(new_root.tree('pointlist4'),True) )
+        # check
+        data = self.root.tree('array/pointlistarray/pointlist4')
+        assert(isinstance(data,PointList))
+        assert(data == self.pl4)
+
 
 
 
 class TestTreeIO(TreeBuilder):
 
     @classmethod
     def setup_class(cls):
```

### Comparing `emdfile-0.0.8/tutorials/emdfile_intro_example.ipynb` & `emdfile-0.0.9/tutorials/emdfile_intro_example.ipynb`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/tutorials/emdfile_package_walkthrough.ipynb` & `emdfile-0.0.9/tutorials/emdfile_package_walkthrough.ipynb`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/tutorials/pngs/node.png` & `emdfile-0.0.9/tutorials/pngs/node.png`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/tutorials/pngs/tree.png` & `emdfile-0.0.9/tutorials/pngs/tree.png`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/tutorials/sample_custom_emd_classes/my_custom_classes.py` & `emdfile-0.0.9/tutorials/sample_custom_emd_classes/my_custom_classes.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/LICENSE` & `emdfile-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/README.md` & `emdfile-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/pyproject.toml` & `emdfile-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.8/PKG-INFO` & `emdfile-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emdfile
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: github, https://github.com/py4dstem/emdfile
 Project-URL: emdatasets, https://emdatasets.com/format/
 Author-email: "Benjamin H. Savitzky" <ben.savitzky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

