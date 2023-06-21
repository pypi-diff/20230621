# Comparing `tmp/easytree-0.1.9.tar.gz` & `tmp/easytree-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytree-0.1.9.tar", last modified: Mon Jun 21 22:38:28 2021, max compression
+gzip compressed data, was "easytree-0.2.0.tar", last modified: Wed Jun 21 21:52:32 2023, max compression
```

## Comparing `easytree-0.1.9.tar` & `easytree-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2021-06-21 22:38:28.019868 easytree-0.1.9/
--rw-r--r--   0 dschenck   (501) staff       (20)     3000 2021-06-21 22:38:28.019687 easytree-0.1.9/PKG-INFO
--rw-r--r--   0 dschenck   (501) staff       (20)     1920 2021-06-20 16:17:19.000000 easytree-0.1.9/README.md
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2021-06-21 22:38:28.018561 easytree-0.1.9/easytree/
--rw-r--r--   0 dschenck   (501) staff       (20)      233 2021-06-13 18:21:49.000000 easytree-0.1.9/easytree/__init__.py
--rw-r--r--   0 dschenck   (501) staff       (20)    20833 2021-06-21 22:36:32.000000 easytree-0.1.9/easytree/tree.py
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2021-06-21 22:38:28.019109 easytree-0.1.9/easytree.egg-info/
--rw-r--r--   0 dschenck   (501) staff       (20)     3000 2021-06-21 22:38:27.000000 easytree-0.1.9/easytree.egg-info/PKG-INFO
--rw-r--r--   0 dschenck   (501) staff       (20)      216 2021-06-21 22:38:27.000000 easytree-0.1.9/easytree.egg-info/SOURCES.txt
--rw-r--r--   0 dschenck   (501) staff       (20)        1 2021-06-21 22:38:27.000000 easytree-0.1.9/easytree.egg-info/dependency_links.txt
--rw-r--r--   0 dschenck   (501) staff       (20)       15 2021-06-21 22:38:27.000000 easytree-0.1.9/easytree.egg-info/top_level.txt
--rw-r--r--   0 dschenck   (501) staff       (20)       38 2021-06-21 22:38:28.019919 easytree-0.1.9/setup.cfg
--rw-r--r--   0 dschenck   (501) staff       (20)      713 2021-06-21 22:24:52.000000 easytree-0.1.9/setup.py
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2021-06-21 22:38:28.019317 easytree-0.1.9/tests/
--rw-r--r--   0 dschenck   (501) staff       (20)        0 2021-06-13 18:21:49.000000 easytree-0.1.9/tests/__init__.py
--rw-r--r--   0 dschenck   (501) staff       (20)    11227 2021-06-21 22:34:43.000000 easytree-0.1.9/tests/tree.py
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2023-06-21 21:52:32.841304 easytree-0.2.0/
+-rw-r--r--   0 dschenck   (501) staff       (20)     1070 2022-02-14 20:33:47.000000 easytree-0.2.0/LICENSE
+-rw-r--r--   0 dschenck   (501) staff       (20)     2325 2023-06-21 21:52:32.841114 easytree-0.2.0/PKG-INFO
+-rw-r--r--   0 dschenck   (501) staff       (20)     1813 2023-06-14 20:51:03.000000 easytree-0.2.0/README.md
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2023-06-21 21:52:32.838708 easytree-0.2.0/easytree/
+-rw-r--r--   0 dschenck   (501) staff       (20)      295 2023-06-03 13:38:22.000000 easytree-0.2.0/easytree/__init__.py
+-rw-r--r--   0 dschenck   (501) staff       (20)    21764 2023-06-14 20:42:20.000000 easytree-0.2.0/easytree/tree.py
+-rw-r--r--   0 dschenck   (501) staff       (20)    22883 2023-06-20 20:38:30.000000 easytree-0.2.0/easytree/types.py
+-rw-r--r--   0 dschenck   (501) staff       (20)     5349 2023-06-20 21:35:33.000000 easytree-0.2.0/easytree/utils.py
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2023-06-21 21:52:32.839529 easytree-0.2.0/easytree.egg-info/
+-rw-r--r--   0 dschenck   (501) staff       (20)     2325 2023-06-21 21:52:32.000000 easytree-0.2.0/easytree.egg-info/PKG-INFO
+-rw-r--r--   0 dschenck   (501) staff       (20)      290 2023-06-21 21:52:32.000000 easytree-0.2.0/easytree.egg-info/SOURCES.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)        1 2023-06-21 21:52:32.000000 easytree-0.2.0/easytree.egg-info/dependency_links.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)       15 2023-06-21 21:52:32.000000 easytree-0.2.0/easytree.egg-info/top_level.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)       38 2023-06-21 21:52:32.841352 easytree-0.2.0/setup.cfg
+-rw-r--r--   0 dschenck   (501) staff       (20)      710 2023-06-13 19:07:30.000000 easytree-0.2.0/setup.py
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2023-06-21 21:52:32.840664 easytree-0.2.0/tests/
+-rw-r--r--   0 dschenck   (501) staff       (20)        0 2021-06-13 18:21:49.000000 easytree-0.2.0/tests/__init__.py
+-rw-r--r--   0 dschenck   (501) staff       (20)    17529 2023-06-04 07:02:31.000000 easytree-0.2.0/tests/tree.py
+-rw-r--r--   0 dschenck   (501) staff       (20)    16090 2023-06-18 08:15:22.000000 easytree-0.2.0/tests/types.py
+-rw-r--r--   0 dschenck   (501) staff       (20)     3830 2023-06-07 20:41:31.000000 easytree-0.2.0/tests/utils.py
```

### Comparing `easytree-0.1.9/easytree/tree.py` & `easytree-0.2.0/easytree/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,342 +1,211 @@
-import json
-import collections.abc as abc
+import builtins
 
 
-class AmbiguityError(Exception):
-    pass
-
+def cast(value, **kwargs):
+    """
+    Convert a value to an easytree object, when possible, based on its type.
 
-class NODETYPES:
-    DICT = "dict"
-    LIST = "list"
-    UNDEFINED = "undefined"
+    - dict instances are cast to easytree.dict instances.
+    - lists instances are cast to easytree.list instances
+    - other types are returns as is, without further transformations
 
+    Parameters
+    ----------
+    value : any
+        the value to cast to an easytree type
+    kwargs : dict
+        additional parameters to pass to the easytree.dict or easytree.list
+        initialisation (sealed, frozen)
 
-class Node:
+    Returns
+    -------
+    cast : any
+        the cast value, or value itself, as the case may be
     """
-    A recursive tree structure, supporting both dict and list nodes. New children nodes can be read and written as attributes, and dynamically becomes nodes themselves. 
+    if isinstance(value, builtins.dict):
+        return dict(value, **kwargs)
+    if isinstance(value, builtins.list):
+        return list(value, **kwargs)
+    if isinstance(value, tuple):
+        return tuple(cast(x, **kwargs) for x in value)
+    if isinstance(value, set):
+        return {cast(x, **kwargs) for x in value}
+    return value
 
-    Example
-    -------------
-    >>> root = easytree.Tree()
-    >>> root.user.firstname = "foo"
-    >>> root.user.firstname == root["user"]["firstname"] == "foo"
-    True
-    >>> root.user.friends.append(username="@jack")
-    >>> root
-    {
-        "user":{
-            "firstname":"foo"
-        },
-        "friends":[
-            {
-                "username":"@jack"
-            }
-        ]
-    }
 
-    The type of a newly-accessed node is initially *undefined*, but is cast as a dict or a list depending on subsequent interactions.
+class list(builtins.list):
+    """
+    easytree.list
 
-    Example
-    ------------
-    >>> root = easytree.Tree()
-    >>> root.abc                              #abc is an undefined node
-    >>> root.abc.xyz                          #abc is cast to a dict node; xyz is undefined
-    >>> root.abc.xyz.append(firstname="Bob")  #xyz is cast to a list node with one dict node
-
-    A tree can be *serialized* back to native python objects using the :code:`serialize` method
-    
-    Example
-    -------------
-    >>> tree = easytree.Tree()
-    >>> tree.abc.xyz.append(44)
-    >>> tree.serialize()
-    {
-        "abc":{
-            "xyz:[
-                44
-            ]
-        }
-    }
+    Parameters
+    ----------
+    args : iterable, None
+        an iterable values
 
-    A tree can be *sealed* or *frozen* to prevent further changes
+    sealed : bool
+        True if list is sealed, False otherwise
 
-    Example
-    --------------
-    >>> tree = easytree.Tree({"abc":{"xyz":True}}, sealed=True)
-    >>> tree.abc.xyz = False
-    >>> tree.foo = "bar"
-    AttributeError: cannot set new attribute 'foo' on sealed node
-    """
+    frozen : bool
+        True if list is frozen, False otherwise
 
-    __hash__ = None
+    Note
+    ----
+    Lists and dicts included or appended in the list
+    are recursively sealed and frozen as per its containing parent.
+    """
 
-    def __new__(cls, value=None, *args, **kwargs):
-        if cls is not Node:
-            return super().__new__(cls)
-        if value is None or isinstance(
-            value, (list, tuple, set, range, zip, dict, abc.KeysView, abc.ValuesView)
-        ):
-            return super().__new__(cls)
-        # keep subclass instances intact
-        if isinstance(value, Node) and type(value) is Node:
-            return super().__new__(cls)
-        return value
-
-    def __init__(self, value=None, *, sealed=False, frozen=False):
-        if isinstance(value, Node):
-            value = value.serialize()
-        if isinstance(value, dict):
-            value = {k: Node(v, sealed=sealed, frozen=frozen) for k, v in value.items()}
-        elif isinstance(
-            value, (list, tuple, set, range, zip, abc.KeysView, abc.ValuesView)
-        ):
-            value = [Node(v, sealed=sealed, frozen=frozen) for v in value]
-        elif value is not None:
-            raise TypeError(
-                "tree node must be initialized with either None, dict, or list"
-            )
-        self._value = value
-        self._frozen = frozen
+    def __init__(self, args=None, sealed=False, frozen=False):
+        super().__init__(
+            [cast(arg, sealed=sealed, frozen=frozen) for arg in (args or [])]
+        )
         self._sealed = sealed
+        self._frozen = frozen
 
-    def __repr__(self):
-        return f"Tree({repr(serialize(self))})"
-
-    def __str__(self):
-        return str(serialize(self))
-
-    @property
-    def __nodetype(self):
-        """
-        Returns the type of the node
+    def __setitem__(self, key, value):
         """
-        if "_value" not in self.__dict__ or self._value is None:
-            return NODETYPES.UNDEFINED
-        if isinstance(self._value, list):
-            return NODETYPES.LIST
-        if isinstance(self._value, dict):
-            return NODETYPES.DICT
-        raise RuntimeError
+        Set a value in the list at an index or slice
 
-    def __getattr__(self, name):
-        """
-        Retrieves an attribute by name for dict nodes.
+        If the value is a list or a dict, the value is cast to
+        an :code:`easytree.list` or :code:`easytree.dict`
+
+        Parameters
+        ----------
+        key : int, slice
+            the index or slice of indices
+        value : any
+            the value
 
-        If the node is undefined, this operations casts the node to a dict node.
+        Returns
+        -------
+        None
 
-        Raises an AttributeError for list nodes. 
+        Raises
+        ------
+        TypeError
+            if the list is sealed or frozen
         """
-        if name == "_ipython_canary_method_should_not_exist_":
-            return True  # ipython workaround
-        if name in ("_frozen", "_sealed"):
-            return False  # defaults for inheritence
-        if self.__nodetype == NODETYPES.LIST:
-            raise AttributeError(f"list node has no attribute '{name}'")
-        if self.__nodetype == NODETYPES.UNDEFINED:
-            if self._frozen:
-                raise AttributeError(f"frozen node has no attribute '{name}'")
-            if self._sealed:
-                raise AttributeError(f"sealed node has no attribute '{name}'")
-            self._value = {}
-        if name not in self._value:
-            if self._frozen:
-                raise AttributeError(f"frozen node has no attribute '{name}'")
-            if self._sealed:
-                raise AttributeError(f"sealed node has no attribute '{name}'")
-            self._value[name] = Node(sealed=self._sealed, frozen=self._frozen)
-        return self._value[name]
+        if self._frozen:
+            raise TypeError("cannot set item on frozen easytree.list")
+        if self._sealed:
+            raise TypeError("cannot set item on sealed easytree.list")
+        return super().__setitem__(
+            key, cast(value, frozen=self._frozen, sealed=self._sealed)
+        )
 
-    def __setattr__(self, name, value):
+    def __delitem__(self, key):
         """
-        Sets the value at an attribute for dict nodes. 
+        Delete an item from the list by its index
 
-        If the node is undefined, this operation casts the node to a dict node.
+        Parameter
+        ---------
+        key : int, slice
+            the index or slice of indices
 
-        Raises an AttributeError for list nodes. 
-        """
-        if name in ("_value", "_frozen", "_sealed"):
-            return super().__setattr__(name, value)
-        if name in {"serialize", "get", "append"}:
-            raise AttributeError(f"Attribute '{name}' is read-only")
-        if self.__nodetype == NODETYPES.UNDEFINED:
-            if self._frozen:
-                raise AttributeError(
-                    f"cannot set new attribute '{name}' on frozen node"
-                )
-            if self._sealed:
-                raise AttributeError(
-                    f"cannot set new attribute '{name}' on sealed node"
-                )
-            self._value = {}
-        if self.__nodetype == NODETYPES.DICT:
-            if self._frozen:
-                raise AttributeError(f"cannot set attribute '{name}' on frozen node")
-            if name not in self._value and self._sealed:
-                raise AttributeError(
-                    f"cannot set new attribute '{name}' on sealed node"
-                )
-            self._value[name] = Node(value, sealed=self._sealed, frozen=self._frozen)
-            return
-        raise AttributeError(f"list node has no attribute '{name}'")
+        Returns
+        -------
+        None
 
-    def __delattr__(self, name):
+        Raises
+        ------
+        TypeError
+            if the list is sealed or frozen
         """
-        Remove an attribute by name
-        """
-        if name in {
-            "__nodetype",
-            "_value",
-            "_frozen",
-            "_sealed",
-            "serialize",
-            "get",
-            "append",
-        }:
-            raise AttributeError(f"Attribute '{name}' is read-only")
-        if self.__nodetype == NODETYPES.UNDEFINED:
-            raise AttributeError(f"undefined node has no attribute '{name}'")
         if self._frozen:
-            raise AttributeError(f"cannot delete attribute '{name}' on frozen node")
+            raise TypeError("cannot delete item from frozen easytree.list")
         if self._sealed:
-            raise AttributeError(f"cannot delete attribute '{name}' on sealed node")
-        del self._value[name]
-
-    def __getitem__(self, name):
-        """
-        Retrieves an item at an index (for list nodes) or at a key (for dict nodes). 
+            raise TypeError("cannot delete item from sealed easytree.list")
+        return super().__delitem__(key)
 
-        If the node is undefined, this operation casts the node to a dict node, unless the given key/index is an integer; instead, an AmbiguityError error is raised.
+    def __enter__(self):
         """
-        if self.__nodetype == NODETYPES.UNDEFINED:
-            if self._frozen:
-                raise KeyError(f"frozen node has no value for '{name}'")
-            if self._sealed:
-                raise KeyError(f"sealed node has no value for '{name}'")
-            if isinstance(name, (int, slice)):
-                raise AmbiguityError(
-                    "Node type is undefined: cast to dict node or list node to disambiguate"
-                )
-            else:
-                self._value = {}
-        if self.__nodetype == NODETYPES.DICT:
-            if name not in self._value:
-                if self._frozen:
-                    raise KeyError(f"frozen node has no value for '{name}'")
-                if self._sealed:
-                    raise KeyError(f"sealed node has no value for '{name}'")
-                self._value[name] = Node(sealed=self._sealed, frozen=self._frozen)
-            return self._value[name]
-        if self.__nodetype == NODETYPES.LIST:
-            if not isinstance(name, (int, slice)):
-                raise TypeError(
-                    f"list indices must be integers or slices, not {type(name).__name__}"
-                )
-            return self._value[name]
-        raise RuntimeError
+        For convenience, you can use a context manager to write to deeply
+        nested trees.
 
-    def __setitem__(self, name, value):
-        """
-        Sets the value at an index (for list nodes) or at a key (for dict node). 
+        The context manager has no side effect.
 
-        If the node is undefined, this operation casts the node to a dict node, unlesss the given key/index is a slice object. 
+        Returns
+        -------
+        self : list
+            the list itself
         """
-        if self._frozen:
-            raise TypeError(f"cannot set item '{name}' on frozen node")
-        if self.__nodetype == NODETYPES.UNDEFINED:
-            if isinstance(name, int):
-                raise IndexError("list assignment index out of range")
-            elif isinstance(name, slice):
-                self._value = []
-            else:
-                self._value = {}
-        if self.__nodetype == NODETYPES.DICT:
-            if name not in self._value and self._sealed:
-                raise TypeError(f"cannot set new item '{name}' on sealed node")
-            self._value[name] = Node(value, sealed=self._sealed, frozen=self._frozen)
-            return
-        if self.__nodetype == NODETYPES.LIST:
-            if not isinstance(name, (int, slice)):
-                raise TypeError(f"cannot index list with {type(name)}")
-            self._value[name] = Node(value, sealed=self._sealed, frozen=self._frozen)
-            return
-        raise RuntimeError
+        return self
 
-    def __delitem__(self, name):
+    def __exit__(self, *args, **kwargs):
         """
-        Deletes the value at an index (for list nodes) or at a key (for dict node). 
+        Exit the context manager
         """
-        if self._frozen:
-            raise TypeError(f"cannot delete item '{name}' on frozen node")
-        if self._sealed:
-            raise TypeError(f"cannot delete item '{name}' on sealed node")
-        if self.__nodetype == NODETYPES.UNDEFINED:
-            raise AttributeError("undefined node has no attribute '{name}'")
-        del self._value[name]
+        pass
 
-    def __iter__(self):
+    def __reduce__(self):
         """
-        Iterates over the underlying value.
+        Pickling reducer
         """
-        if self.__nodetype == NODETYPES.UNDEFINED:
-            raise TypeError("undefined node is not iterable")
-        return iter(self._value)
+        return self.__class__, (), self.__dict__, iter(self), None
 
-    def __len__(self):
+    def __setstate__(self, state):
         """
-        Returns the length of the underlying value.
+        Pickling setter
         """
-        if self.__nodetype == NODETYPES.UNDEFINED:
-            raise TypeError("undefined node has no length")
-        return len(self._value)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_value, exc_traceback):
-        pass
-
-    def __contains__(self, value):
-        if self.__nodetype == NODETYPES.UNDEFINED:
-            raise TypeError("undefined node is not iterable")
-        return self._value.__contains__(value)
-
-    def __bool__(self):
-        return bool(self._value)
+        self.__dict__.update(state)
 
     def append(self, *args, **kwargs):
         """
-        Appends a value to a list node. If the node type was previously undefined, the node becomes a list. 
+        Append a value to the list
 
         Note
         ---------
-        The append method can take either one positional argument or one-to-many named (keyword) arguments. If passed one-to-many keyword arguments, the kwargs dictionary is added to the list.
+        The :code:`append` method can take either one positional argument or
+        one-to-many named (keyword) arguments. If passed keyword
+        arguments, the kwargs dictionary is added to the list as an
+        :code:`easytree.dict`.
+
+        Returns
+        -------
+        item : any
+            the last added item
+
+        Raises
+        ------
+        TypeError
+            if the list is sealed or frozen
+        ValueError
+            if neither a value nor a set of kwargs is given
 
         Example
-        ---------
-        >>> tree = easytree.Tree()                                 #undefined node
-        >>> tree.append("hello world")                            #casts node to list
-        >>> tree.append(name="David", age=29)                     #call with kwargs
-        >>> tree.append({"animal":"elephant", "country":"India"}) #call with args
-        >>> tree.serialize()
-        ["Hello world",{"name":"David","age":29},{"animal":"elephant", "country":"India"}]
+        -------
+        >>> tree = easytree.list()                                # list node
+        >>> tree.append("hello world")                            # simple append
+        >>> tree.append(name="David", age=29)                     # call with kwargs
+        >>> tree.append({"animal":"elephant", "country":"India"}) # call with dict
+        >>> tree
+        [
+            "Hello world",
+            {
+                "name": "David",
+                "age": 29
+            },
+            {
+                "animal": "elephant",
+                "country": "India"
+            }
+        ]
 
         Note
         ---------
-        The append method intentionally returns a reference to the last-added item, if that item is a new node. This allows for fluent code using the context manager. 
+        The append method intentionally returns a reference to the last-added item. This allows for fluent code using the context manager.
 
         Example
-        -----------
-        >>> chart = easytree.Tree()
-        >>> with chart.axes.append({}) as axis: 
+        -------
+        >>> chart = easytree.dict()
+        >>> with chart.axes.append({}) as axis:
         ...     axis.title.text = "primary axis"
-        >>> with chart.axes.append({}) as axis: 
+        >>> with chart.axes.append({}) as axis:
         ...     axis.title.text = "secondary axis"
-        >>> chart.serialize()
+        >>> chart
         {
             "axes": [
                 {
                     "title": {
                         "text": "primary axis"
                     }
                 },
@@ -344,287 +213,647 @@
                     "title": {
                         "text": "secondary axis"
                     }
                 }
             ]
         }
         """
-        if self._frozen or self._sealed:
-            raise TypeError("cannot append value to frozen or sealed node")
+        if self._frozen:
+            raise TypeError("cannot append value to frozen easytree.list")
+        if self._sealed:
+            raise TypeError("cannot append value to sealed easytree.list")
         if (
             len(args) > 1
             or (len(args) != 0 and len(kwargs) != 0)
             or (len(args) == len(kwargs) == 0)
         ):
             raise ValueError(
                 "append must take either one positional argument or one-to-many named arguments"
             )
-        value = args[0] if args else kwargs
-        if self.__nodetype == NODETYPES.UNDEFINED:
-            self._value = []
-        if self.__nodetype == NODETYPES.LIST:
-            value = Node(value, sealed=self._sealed, frozen=self._frozen)
-            self._value.append(value)
-            return value if isinstance(value, Node) else None
-        raise AttributeError("dict node has no attribute 'append'")
 
-    def get(self, key, default=None):
+        super().append(
+            cast(args[0] if args else kwargs, sealed=self._sealed, frozen=self._frozen)
+        )
+        return self[len(self) - 1]
+
+    def extend(self, other):
         """
-        Returns the value at a given key, or default if the key does not exists.
+        Extend the list by appending all the items from another iterable.
 
-        Example
-        ---------------------
-        >>> config = easytree.Tree({"context":{"starting":"2016-03-31"}})
-        >>> config.context.get("starting", "2014-01-01")
-        2016-03-31
-        >>> config.context.get("ending", "2021-12-31")
-        2021-12-31
-        >>> config.context.get("calendar")
+        list or dict items from other are cast to :code:`easytree.list` or
+        :code:`easytree.dict` values respectively.
+
+        Parameters
+        ----------
+        other : iterable
+            the other iterable
+
+        Returns
+        -------
         None
-        """
-        if self.__nodetype == NODETYPES.LIST:
-            raise AttributeError("list node has no attribute 'get'")
-        if self.__nodetype == NODETYPES.UNDEFINED:
-            return default
-        if key in self._value:
-            return self._value[key]
-        return default
 
-    def serialize(self):
+        Raises
+        ------
+        TypeError
+            if the list is sealed or frozen
         """
-        Recursively converts itself to a native python type (dict, list or None).
+        if self._frozen:
+            raise TypeError("cannot extend frozen easytree.list")
+        if self._sealed:
+            raise TypeError("cannot extend sealed easytree.list")
+        return super().extend(
+            [cast(v, sealed=self._sealed, frozen=self._frozen) for v in other]
+        )
 
-        Example
-        ---------------------
-        >>> chart = easytree.Tree()
-        >>> chart.chart.type = "bar"
-        >>> chart.title.text = "France Olympic Medals"
-        >>> chart.xAxis.categories = ["Gold", "Silver", "Bronze"]
-        >>> chart.yAxis.title.text = "Count"
-        >>> chart.series.append(name="2016", data=[10, 18, 14])
-        >>> chart.series.append({"name":"2012", "data":[11,11,13]})
-        >>> chart.serialize()
-        {
-            "chart": {
-                "type": "bar"
-            },
-            "title": {
-                "text": "France Olympic Medals"
-            },
-            "xAxis": {
-                "categories": [
-                    "Gold",
-                    "Silver",
-                    "Bronze"
-                ]
-            },
-            "yAxis": {
-                "title": {
-                    "text": "Count"
-                }
-            },
-            "series": [
-                {
-                    "name": "2016",
-                    "data": [
-                        10,
-                        18,
-                        14
-                    ]
-                },
-                {
-                    "name": "2012",
-                    "data": [
-                        11,
-                        11,
-                        13
-                    ]
-                }
-            ]
-        }
+    def insert(self, index, value):
         """
-        return serialize(self)
+        Insert an item into the list at a given position.
 
+        If the value is a list or a dict, the value is cast to
+        an :code:`easytree.list` or :code:`easytree.dict`
 
-def serialize(tree):
-    """
-    Recursively converts an :code:`easytree.Tree` back to a native python type.
+        Parameters
+        ----------
+        index : int
+            the index at which to insert the value
+        value : any
+            the inserted value
 
-    Example
-    ---------------------
-    >>> chart = easytree.Tree()
-    >>> chart.chart.type = "bar"
-    >>> chart.title.text = "France Olympic Medals"
-    >>> chart.xAxis.categories = ["Gold", "Silver", "Bronze"]
-    >>> chart.yAxis.title.text = "Count"
-    >>> chart.series.append(name="2016", data=[10, 18, 14])
-    >>> chart.series.append({"name":"2012", "data":[11,11,13]})
-    >>> easytree.serialize(chart)
-    {
-        "chart": {
-            "type": "bar"
-        },
-        "title": {
-            "text": "France Olympic Medals"
-        },
-        "xAxis": {
-            "categories": [
-                "Gold",
-                "Silver",
-                "Bronze"
-            ]
-        },
-        "yAxis": {
-            "title": {
-                "text": "Count"
-            }
-        },
-        "series": [
-            {
-                "name": "2016",
-                "data": [
-                    10,
-                    18,
-                    14
-                ]
-            },
-            {
-                "name": "2012",
-                "data": [
-                    11,
-                    11,
-                    13
-                ]
-            }
-        ]
-    }
-    """
-    if not isinstance(tree, Node):
-        return tree
-    if tree._Node__nodetype == NODETYPES.UNDEFINED:
-        return None
-    if tree._Node__nodetype == NODETYPES.LIST:
-        return [serialize(value) for value in tree._value]
-    if tree._Node__nodetype == NODETYPES.DICT:
-        return {key: serialize(value) for key, value in tree._value.items()}
-    raise RuntimeError
+        Returns
+        -------
+        None
 
+        Raises
+        ------
+        TypeError
+            if the list is sealed or frozen
+        """
+        if self._frozen:
+            raise TypeError("cannot insert into frozen easytree.list")
+        if self._sealed:
+            raise TypeError("cannot insert into sealed easytree.list")
+        return super().insert(
+            index, cast(value, sealed=self._sealed, frozen=self._frozen)
+        )
 
-def new(root=None, *, sealed=False, frozen=False):
-    """
-    Creates a new :code:`easytree.Tree`
-    """
-    return Node(root, sealed=sealed, frozen=frozen)
+    def remove(self, x):
+        """
+        Remove the first item from the list whose value is equal to x.
 
+        Parameters
+        ----------
+        x : any
+            the value to remove
 
-def load(stream, *args, frozen=False, sealed=False, **kwargs):
-    """
-    Deserialize a text file or binary file containing a JSON document to an :code:`Tree` object 
+        Returns
+        -------
+        None
 
+        Raises
+        ------
+        TypeError
+            if the list is sealed or frozen
+        ValueError
+            if there is no such item
+        """
+        if self._frozen:
+            raise TypeError("cannot remove from frozen easytree.list")
+        if self._sealed:
+            raise TypeError("cannot remove from sealed easytree.list")
+        return super().remove(x)
 
-    :code:`*args` and :code:`**kwargs` are passed to the :code:`json.load` function
+    def pop(self, *args):
+        """
+        Remove the item at the given position in the list,
+        and return it.
 
-    Example
-    -------------
-    >>> with open("data.json", "r") as file: 
-    ...     tree = easytree.load(file)
-    """
-    return Node(json.load(stream, *args, **kwargs), sealed=sealed, frozen=frozen)
+        Returns
+        -------
+        item : any
+            the popped item
+
+        Raises
+        ------
+        TypeError
+            if the list is sealed or frozen
+        """
+        if self._frozen:
+            raise TypeError("cannot pop from frozen easytree.list")
+        if self._sealed:
+            raise TypeError("cannot pop from sealed easytree.list")
+        return super().pop(*args)
 
+    def clear(self):
+        """
+        Remove all items from the list.
 
-def loads(s, *args, frozen=False, sealed=False, **kwargs):
-    """
-    Deserialize s (a str, bytes or bytearray instance containing a JSON document) to an :code:`Tree` object 
+        Returns
+        -------
+        None
 
-    :code:`*args` and :code:`**kwargs` are passed to the :code:`json.loads` function
-    """
-    return Node(json.loads(s, *args, **kwargs), sealed=sealed, frozen=frozen)
+        Raises
+        ------
+        TypeError
+            if the list is sealed or frozen
+        """
+        if self._frozen:
+            raise TypeError("cannot clear frozen easytree.list")
+        if self._sealed:
+            raise TypeError("cannot clear sealed easytree.list")
+        return super().clear()
 
+    def sort(self, *, key=None, reverse=False):
+        """
+        Sort the items of the list in place
 
-def dump(obj, stream, *args, **kwargs):
-    """
-    Serialize :code:`Tree` object as a JSON formatted string to stream (a .write()-supporting file-like object). 
+        Returns
+        -------
+        None
 
-    :code:`*args` and :code:`**kwargs` are passed to the :code:`json.dump` function
+        Raises
+        ------
+        TypeError
+            if the list is frozen
+        """
+        if self._frozen:
+            raise TypeError("cannot sort frozen easytree.list")
+        return super().sort(key=key, reverse=reverse)
 
-    Example
-    -------------
-    >>> tree = easytree.Tree({"foo": "bar"})
-    >>> with open("data.json", "w") as file: 
-    ...     easytree.dump(tree, file, indent=4)
-    """
-    return json.dump(serialize(obj), stream, *args, **kwargs)
+    def reverse(self):
+        """
+        Reverse the elements of the list in place.
 
+        Returns
+        -------
+        None
 
-def dumps(obj, *args, **kwargs):
-    """
-    Serialize :code:`Tree` to a JSON formatted string. 
+        Raises
+        ------
+        TypeError
+            if the list is sealed or frozen
+        """
+        if self._frozen:
+            raise TypeError("cannot reverse frozen easytree.list")
+        return super().reverse()
 
-    :code:`*args` and :code:`**kwargs` are passed to the :code:`json.dumps` function
-    """
-    return json.dumps(serialize(obj), *args, **kwargs)
+    def copy(self):
+        """
+        Return a shallow copy of the list
+
+        Returns
+        -------
+        copy : list
+            the new list
+        """
+        return list(self, frozen=self._frozen, sealed=self._sealed)
 
 
-def frozen(tree):
+class dict(builtins.dict):
     """
-    Returns :code:`True` if the tree is frozen
+    recursive dot-styled defaultdict
     """
-    if not isinstance(tree, Node):
-        raise TypeError(
-            f"Expected tree to be instance of easytree.Tree, received {type(tree)}"
+
+    def __init__(self, *args, sealed=False, frozen=False, **kwargs):
+        super().__init__(
+            {
+                k: cast(v, sealed=sealed, frozen=frozen)
+                for k, v in builtins.dict(*args, **kwargs).items()
+            }
         )
-    return tree._frozen
+        self._sealed = sealed
+        self._frozen = frozen
 
+    def __getitem__(self, key):
+        """
+        Returns a value at a key, or :code:`undefined` if
+        key does not exist
 
-def freeze(tree):
-    """
-    Returns a new frozen copy of the tree
-    """
-    if not isinstance(tree, Node):
-        raise TypeError(
-            f"Expected tree to be instance of easytree.Tree, received {type(tree)}"
-        )
-    return Node(tree, frozen=True)
+        Raises
+        ------
+        KeyError
+            if the dict is frozen or sealed, and the key does not
+            exist in the dict
+        """
+        try:
+            return super().__getitem__(key)
+        except KeyError:
+            if self._frozen:
+                raise KeyError(f"frozen easytree.dict has no value for {key}") from None
+            if self._sealed:
+                raise KeyError(f"sealed easytree.dict has no value for {key}") from None
+        return undefined(parent=self, key=key)
 
+    def __setitem__(self, key, value):
+        """
+        Set a value at a key
 
-def unfreeze(tree):
-    """
-    Returns a new unfrozen copy of the tree
-    """
-    if not isinstance(tree, Node):
-        raise TypeError(
-            f"Expected tree to be instance of easytree.Tree, received {type(tree)}"
-        )
-    return Node(tree, frozen=False)
+        Returns
+        -------
+        None
+
+        Raises
+        ------
+        KeyError
+            if the dict is frozen, or if the dict is sealed and the key does not exist in the dict
+        """
+        if self._frozen:
+            raise KeyError(f"cannot define value for {key} on frozen easytree.dict")
+        if self._sealed and key not in self:
+            raise KeyError(f"sealed define value for {key} on sealed easytree.dict")
+        super().__setitem__(key, value)
 
+    def __getattr__(self, key):
+        """
+        Returns a value at a key, or :code:`undefined` if
+        key does not exist
 
-def sealed(tree):
-    """
-    Returns :code:`True` if the tree is sealed
-    """
-    if not isinstance(tree, Node):
-        raise TypeError(
-            f"Expected tree to be instance of easytree.Tree, received {type(tree)}"
+        Note
+        ----
+        if key is :code:`_frozen` or :code:`_sealed`,
+        then the instance is an instance of a subclass
+        to :code:`easytree.dict` which overrode the
+        default :code:`__init__`
+
+        Raises
+        ------
+        AttributeError
+            if the dict is frozen and the key does not exist in the dict, or
+            if the dict is sealed and the key does not exist in the dict
+        """
+        try:
+            return super().__getitem__(key)
+        except KeyError:
+            if key in ["_frozen", "_sealed"]:
+                return False  # if subclass overrides the init (see note)
+            if self._frozen:
+                raise AttributeError(
+                    f"frozen easytree.dict has no attribute {key}"
+                ) from None
+            if self._sealed:
+                raise AttributeError(
+                    f"sealed easytree.dict has no attribute {key}"
+                ) from None
+        return undefined(parent=self, key=key)
+
+    def __setattr__(self, key, value):
+        """
+        Sets a value at a key, recursively casting the value
+        to a :code:`easytree.dict` or :code:`easytree.list`.
+
+        Raises
+        ------
+        AttributeError
+            if the dict is frozen, or if the dict is sealed and the key does not exist in the dict
+        """
+        if key in ["_sealed", "_frozen"]:
+            return super().__setattr__(key, value)
+        if self._frozen:
+            raise AttributeError(f"cannot set attribute {key} on frozen easytree.dict")
+        if self._sealed and key not in self:
+            raise AttributeError(
+                f"cannot define attribute {key} on sealed easytree.dict"
+            )
+        self[key] = cast(value, sealed=self._sealed, frozen=self._frozen)
+
+    def __delattr__(self, key: str) -> None:
+        """
+        Remove an attribute
+
+        Raises
+        ------
+        AttributeError
+            if the dict is frozen or sealed
+        """
+        if self._frozen:
+            raise AttributeError(
+                f"cannot delete attribute '{key}' from frozen easytree.dict"
+            )
+        if self._sealed:
+            raise AttributeError(
+                f"cannot delete attribute '{key}' from sealed easytree.dict"
+            )
+        del self[key]
+
+    def __reduce__(self):
+        """
+        Pickling
+        """
+        return self.__class__, (), self.__dict__, None, iter(self.items())
+
+    def __setstate__(self, state):
+        """
+        Unpickling
+        """
+        self.__dict__.update(state)
+
+    def setdefault(self, key, default):
+        """
+        Insert key with a value of default if key is not in the dictionary.
+
+        Return the value for key if key is in the dictionary, else default.
+
+        Parameters
+        ----------
+        key : any
+            the key
+        default : any
+            the default value to insert if the key does not exist
+
+        Raises
+        ------
+        AttributeError
+            if the dict is frozen, or if the dict is sealed and the key does not exist in the dict
+        """
+        try:
+            return self[key]
+        except KeyError:
+            if self._frozen:
+                raise AttributeError(f"Cannot set {key} on frozen easytree.dict")
+            if self._sealed and key not in self:
+                raise AttributeError(f"Cannot set {key} on sealed easytree.dict")
+        return super().setdefault(
+            key, cast(default, sealed=self._sealed, frozen=self._frozen)
         )
-    return tree._frozen
 
+    def get(self, key, default=None):
+        """
+        Get item by key, if it is exists; otherwise, return default
+
+        If key is list, recursively traverses the tree
 
-def seal(tree):
-    """
-    Returns a new sealed copy of the tree
-    """
-    if not isinstance(tree, Node):
-        raise TypeError(
-            f"Expected tree to be instance of easytree.Tree, received {type(tree)}"
+        Parameters
+        ----------
+        key : hashable, list[hashable]
+            the key (or path of keys)
+
+        Returns
+        -------
+        value : any
+
+        Example
+        -------
+        >>> person = easytree.dict({"age":31, "friends":[{"firstname":"Michael"}]})
+        >>> person.get("age")
+        31
+        >>> person.get("address")
+        None
+        >>> person.get(["friends",0,"firstname"])
+        "Michael"
+        >>> person.get(["friends",1,"firstname"])
+        None
+        >>> person.get(["friends",0,"avatar"],"N/A")
+        "N/A"
+        """
+        if isinstance(key, builtins.list):
+            if len(key) == 0:
+                return default
+
+            current = self
+            while len(key) > 0:
+                try:
+                    current = current[key.pop(0)]
+                except (KeyError, IndexError):
+                    return default
+                if isinstance(current, undefined):
+                    return default
+            return current
+
+        return super().get(key, default)
+
+    @classmethod
+    def fromkeys(cls, keys, value):
+        """
+        Create a dict from a set of keys and a fixed value
+        """
+        return super().fromkeys(keys, cast(value))
+
+    def update(self, other):
+        """
+        Update the dict from keys and values of another mapping
+        object
+
+        Parameters
+        ----------
+        other : mapping
+            other dictionary
+
+        Raises
+        ------
+        AttributeError
+            if the dict is frozen, or if the dict is sealed and a key of other does not exist in the dict
+        """
+        if self._frozen:
+            raise AttributeError(f"Cannot update frozen easytree.dict")
+        if self._sealed:
+            if any(key not in self for key in other):
+                raise AttributeError(
+                    f"Cannot update sealed easytree.dict with new keys"
+                )
+        return super().update(
+            {
+                k: cast(v, sealed=self._sealed, frozen=self._frozen)
+                for k, v in other.items()
+            }
         )
-    return Node(tree, sealed=False)
+
+    def popitem(self):
+        """
+        Remove and return the last item (key, value pair)
+        inserted into the dictionary
+
+        Raises
+        ------
+        KeyError
+            if the dict is empty
+
+        AttributeError
+            if the dict is frozen
+            if the dict is sealed
+        """
+        if self._frozen:
+            raise AttributeError(f"Cannot popitem from frozen easytree.dict")
+        if self._sealed:
+            raise AttributeError(f"Cannot popitem from sealed easytree.dict")
+        return super().popitem()
+
+    def pop(self, *args):
+        """
+        Remove and return an element from a dictionary
+        having the given key.
+
+        Parameters
+        ----------
+        key : any
+            the key to pop
+        default : any
+            the default value, if the key does not exist
+
+        Raises
+        ------
+        KeyError
+            if the given key does not exist, and no default value is given
+
+        AttributeError
+            if the dict is frozen, or if the dict is sealed
+        """
+        if self._frozen:
+            raise AttributeError(f"Cannot pop from frozen easytree.dict")
+        if self._sealed:
+            raise AttributeError(f"Cannot pop from sealed easytree.dict")
+        return super().pop(*args)
+
+    def __enter__(self):
+        """
+        Context manager
+
+        Returns
+        -------
+        self : dict
+            a reference to self
+        """
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_traceback):
+        """
+        Context manager
+        """
+        pass
 
 
-def unseal(tree):
+class undefined:
     """
-    Returns a new unsealed copy of the tree
+    undefined
+
+    Parameters
+    ----------
+    key : hashable
+        the key of the undefined value in its parent
+    parent : list, dict
+        the containing parent
     """
-    if not isinstance(tree, Node):
-        raise TypeError(
-            f"Expected tree to be instance of easytree.Tree, received {type(tree)}"
-        )
-    return Node(tree, sealed=False)
+
+    def __init__(self, parent, key):
+        self.key = key
+        self._parent = parent
+
+    def __bool__(self):
+        """
+        Return False
+        """
+        return False
+
+    def __getitem__(self, key):
+        """
+        Return a new undefined node
+        """
+        return undefined(parent=self, key=key)
+
+    def __getattr__(self, key):
+        """
+        Return a new undefined node
+        """
+        return self[key]
+
+    def __setitem__(self, key, value):
+        """
+        Set a value at a key, casting the
+        undefined value to a dict value
+
+        Returns
+        -------
+        None
+        """
+        if self.key in self._parent:
+            self._parent[self.key][key] = value
+            return
+
+        self._parent[self.key] = dict({key: value})
+
+    def __setattr__(self, key, value):
+        """
+        Set a value at a key, casting the
+        undefined value to a dict value
+
+        Returns
+        -------
+        None
+        """
+        if key in ["key", "_parent"]:
+            return super().__setattr__(key, value)
+        self[key] = value
+
+    def __contains__(self, value):
+        """
+        Return False
+        """
+        return False
+
+    def __iter__(self):
+        """
+        Iterate over empty list
+        """
+        return iter([])
+
+    def append(self, *args, **kwargs):
+        """
+        Cast undefined node to list and append value
+        """
+        if (
+            len(args) > 1
+            or (len(args) != 0 and len(kwargs) != 0)
+            or (len(args) == len(kwargs) == 0)
+        ):
+            raise ValueError(
+                "append must take either one positional argument or one-to-many named arguments"
+            )
+        value = args[0] if len(args) > 0 else kwargs
+        self._parent[self.key] = list([value])
+        return self._parent[self.key][-1]
+
+    def extend(self, other):
+        """
+        Cast undefined node to list and extend with other
+        """
+        self._parent[self.key] = list(other)
+
+    def get(self, key, default=None):
+        """
+        Return default value
+        """
+        return default
+
+    def setdefault(self, key, default):
+        """
+        Cast node to dict and insert default value at key
+        """
+        self._parent[self.key] = dict({key: default})
+
+    def update(self, other):
+        """
+        Cast node to dict and insert items from other
+        """
+        self._parent[self.key] = dict(other)
+        return self._parent
+
+    def __enter__(self):
+        """
+        Return self
+        """
+        return self
+
+    def __exit__(self, *args, **kwargs):
+        """
+        Context manager
+        """
+        pass
+
+    def __len__(self):
+        """
+        Return 0
+        """
+        return 0
+
+    def __repr__(self):
+        """
+        Return representation
+        """
+        return f"<Node '{self.key}'>"
```

### Comparing `easytree-0.1.9/setup.py` & `easytree-0.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="easytree",
-    version="0.1.9",
-    author="david.schenck@outlook.com",
+    version="0.2.0",
+    author="David Schenck",
     author_email="david.schenck@outlook.com",
-    description="A fluent tree builder, useful to create multi-level, nested JSON configurations.",
+    description="A lightweight library designed to easily read and write deeply-nested tree configurations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://easytree.readthedocs.io/en/latest",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

