# Comparing `tmp/uri_template-1.2.0.tar.gz` & `tmp/uri-template-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/open-source/uri_template/dist/tmpei77ymbm/uri_template-1.2.0.tar", last modified: Sat Mar 12 22:47:27 2022, max compression
+gzip compressed data, was "uri-template-1.3.0.tar", last modified: Wed Jun 21 01:48:08 2023, max compression
```

## Comparing `uri_template-1.2.0.tar` & `uri-template-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 22:47:27.000000 uri_template-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1321 2022-03-12 22:47:19.000000 uri_template-1.2.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2022-03-12 22:42:08.000000 uri_template-1.2.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 22:47:27.000000 uri_template-1.2.0/uri_template/
--rw-rw-rw-   0 root         (0) root         (0)      432 2022-03-12 22:42:08.000000 uri_template-1.2.0/uri_template/charset.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2022-03-12 22:42:08.000000 uri_template-1.2.0/uri_template/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5235 2022-03-12 22:42:08.000000 uri_template-1.2.0/uri_template/uritemplate.py
--rw-rw-rw-   0 root         (0) root         (0)    17218 2022-03-12 22:42:08.000000 uri_template-1.2.0/uri_template/expansions.py
--rw-rw-rw-   0 root         (0) root         (0)     2911 2022-03-12 22:42:08.000000 uri_template-1.2.0/uri_template/variable.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-03-12 22:42:08.000000 uri_template-1.2.0/uri_template/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     6499 2022-03-12 22:42:08.000000 uri_template-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-12 22:47:27.000000 uri_template-1.2.0/uri_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)      272 2022-03-12 22:47:27.000000 uri_template-1.2.0/uri_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      366 2022-03-12 22:47:27.000000 uri_template-1.2.0/uri_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     6985 2022-03-12 22:47:27.000000 uri_template-1.2.0/uri_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2022-03-12 22:47:27.000000 uri_template-1.2.0/uri_template.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-12 22:47:27.000000 uri_template-1.2.0/uri_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     6985 2022-03-12 22:47:27.000000 uri_template-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-03-12 22:47:27.000000 uri_template-1.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 01:48:08.266621 uri-template-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-06-21 01:46:34.000000 uri-template-1.3.0/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-06-21 01:46:34.000000 uri-template-1.3.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-21 01:46:34.000000 uri-template-1.3.0/.gitlab-ci.env
+-rw-rw-rw-   0 root         (0) root         (0)      297 2023-06-21 01:46:34.000000 uri-template-1.3.0/.gitlab-ci.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-06-21 01:46:34.000000 uri-template-1.3.0/.yamllint.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-21 01:46:34.000000 uri-template-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7792 2023-06-21 01:48:08.266621 uri-template-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6869 2023-06-21 01:46:34.000000 uri-template-1.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2023-06-21 01:46:34.000000 uri-template-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 01:48:08.266621 uri-template-1.3.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     4544 2023-06-21 01:48:06.000000 uri-template-1.3.0/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 01:48:08.266621 uri-template-1.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2890 2023-06-21 01:46:34.000000 uri-template-1.3.0/tests/corners.json
+-rw-rw-rw-   0 root         (0) root         (0)     5812 2023-06-21 01:46:34.000000 uri-template-1.3.0/tests/extended-tests.json
+-rw-rw-rw-   0 root         (0) root         (0)    14954 2023-06-21 01:46:34.000000 uri-template-1.3.0/tests/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     2233 2023-06-21 01:46:34.000000 uri-template-1.3.0/tests/negative-tests.json
+-rw-rw-rw-   0 root         (0) root         (0)    14416 2023-06-21 01:46:34.000000 uri-template-1.3.0/tests/spec-examples-by-section.json
+-rw-rw-rw-   0 root         (0) root         (0)     6610 2023-06-21 01:46:34.000000 uri-template-1.3.0/tests/spec-examples.json
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-06-21 01:46:34.000000 uri-template-1.3.0/uri-template.sublime-project
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 01:48:08.266621 uri-template-1.3.0/uri_template/
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-06-21 01:46:34.000000 uri-template-1.3.0/uri_template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-06-21 01:46:34.000000 uri-template-1.3.0/uri_template/charset.py
+-rw-rw-rw-   0 root         (0) root         (0)    17273 2023-06-21 01:46:34.000000 uri-template-1.3.0/uri_template/expansions.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-21 01:46:34.000000 uri-template-1.3.0/uri_template/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5255 2023-06-21 01:46:34.000000 uri-template-1.3.0/uri_template/uritemplate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3210 2023-06-21 01:46:34.000000 uri-template-1.3.0/uri_template/variable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 01:48:08.266621 uri-template-1.3.0/uri_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7792 2023-06-21 01:48:08.000000 uri-template-1.3.0/uri_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-21 01:48:08.000000 uri-template-1.3.0/uri_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 01:48:08.000000 uri-template-1.3.0/uri_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      339 2023-06-21 01:48:08.000000 uri-template-1.3.0/uri_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 01:48:08.000000 uri-template-1.3.0/uri_template.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `uri_template-1.2.0/LICENSE` & `uri-template-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uri_template-1.2.0/uri_template/__init__.py` & `uri-template-1.3.0/uri_template/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-"""Module to implement something."""
+"""Module for URI Template expansion."""
 
-from typing import Optional
+from __future__ import annotations
 
 from .expansions import ExpansionFailedError
 from .uritemplate import ExpansionInvalidError, ExpansionReservedError, URITemplate
 from .variable import Variable, VariableInvalidError
 
 
-__all__ = [
-    'URITemplate', 'Variable',
-    'ExpansionInvalidError', 'ExpansionReservedError', 'VariableInvalidError', 'ExpansionFailedError',
-]
+__all__ = (
+    'URITemplate',
+    'Variable',
+    'ExpansionInvalidError',
+    'ExpansionReservedError',
+    'VariableInvalidError',
+    'ExpansionFailedError',
+)
 
 
-def expand(template: str, **kwargs) -> Optional[str]:
+def expand(template: str, **kwargs) -> (str | None):
     try:
         templ = URITemplate(template)
         return templ.expand(**kwargs)
     except Exception:
         return None
 
 
-def partial(template: str, **kwargs) -> Optional[str]:
+def partial(template: str, **kwargs) -> (str | None):
     try:
         templ = URITemplate(template)
         return str(templ.partial(**kwargs))
     except Exception:
         return None
```

### Comparing `uri_template-1.2.0/uri_template/uritemplate.py` & `uri-template-1.3.0/uri_template/uritemplate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Process URI templates per http://tools.ietf.org/html/rfc6570."""
 
-import collections
+from __future__ import annotations
+
 import re
-from typing import Dict, Iterable, List
+from typing import TYPE_CHECKING
 
 from .expansions import (CommaExpansion, Expansion,
                          FormStyleQueryContinuation, FormStyleQueryExpansion,
                          FragmentExpansion, LabelExpansion, Literal,
                          PathExpansion, PathStyleExpansion,
                          ReservedCommaExpansion, ReservedExpansion, SimpleExpansion)
-from .variable import Variable
+
+if (TYPE_CHECKING):
+    from collections.abc import Iterable
+    from .variable import Variable
 
 
 class ExpansionReservedError(Exception):
     """Exception thrown for reserved but unsupported expansions."""
 
     expansion: str
 
@@ -34,22 +38,22 @@
         self.expansion = expansion
 
     def __str__(self) -> str:
         """Convert to string."""
         return 'Bad expansion: ' + self.expansion
 
 
-class URITemplate(object):
+class URITemplate:
     """
     URI Template object.
 
     Constructor may raise ExpansionReservedError, ExpansionInvalidError, or VariableInvalidError.
     """
 
-    expansions: List[Expansion]
+    expansions: list[Expansion]
 
     def __init__(self, template: str) -> None:
         self.expansions = []
         parts = re.split(r'(\{[^\}]*\})', template)
         for part in parts:
             if (part):
                 if (('{' == part[0]) and ('}' == part[-1])):
@@ -84,39 +88,39 @@
                         self.expansions.append(Literal(part))
                     else:
                         raise ExpansionInvalidError(part)
 
     @property
     def variables(self) -> Iterable[Variable]:
         """Get all variables in template."""
-        vars: Dict[str, Variable] = collections.OrderedDict()
+        vars: dict[str, Variable] = {}
         for expansion in self.expansions:
             for var in expansion.variables:
                 vars[var.name] = var
         return vars.values()
 
     @property
     def variable_names(self) -> Iterable[str]:
         """Get names of all variables in template."""
-        vars: Dict[str, Variable] = collections.OrderedDict()
+        vars: dict[str, Variable] = {}
         for expansion in self.expansions:
             for var in expansion.variables:
                 vars[var.name] = var
         return [var.name for var in vars.values()]
 
     def expand(self, **kwargs) -> str:
         """
         Expand the template.
 
         May raise ExpansionFailed if a composite value is passed to a variable with a prefix modifier.
         """
         expanded = [expansion.expand(kwargs) for expansion in self.expansions]
         return ''.join([expansion for expansion in expanded if (expansion is not None)])
 
-    def partial(self, **kwargs) -> 'URITemplate':
+    def partial(self, **kwargs) -> URITemplate:
         """
         Expand the template, preserving expansions for missing variables.
 
         May raise ExpansionFailed if a composite value is passed to a variable with a prefix modifier.
         """
         expanded = [expansion.partial(kwargs) for expansion in self.expansions]
         return URITemplate(''.join(expanded))
```

### Comparing `uri_template-1.2.0/uri_template/expansions.py` & `uri-template-1.3.0/uri_template/expansions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 """Process URI templates per http://tools.ietf.org/html/rfc6570."""
 
+from __future__ import annotations
+
 import collections
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, cast
+from typing import Any, TYPE_CHECKING, cast
 
 from .charset import Charset
 from .variable import Variable
 
+if (TYPE_CHECKING):
+    from collections.abc import Iterable, Mapping
+
 
 class ExpansionFailedError(Exception):
     """Exception thrown when expansions fail."""
 
     variable: str
 
     def __init__(self, variable: str) -> None:
         self.variable = variable
 
     def __str__(self) -> str:
         """Convert to string."""
         return 'Bad expansion: ' + self.variable
 
 
-class Expansion(object):
+class Expansion:
     """
     Base class for template expansions.
 
     https://tools.ietf.org/html/rfc6570#section-3
     """
 
     def __init__(self) -> None:
@@ -61,15 +66,15 @@
             index += 1
         return output
 
     def _uri_encode_value(self, value: str) -> str:
         """Encode a value into uri encoding."""
         return self._encode(value, Charset.UNRESERVED, False)
 
-    def _uri_encode_name(self, name: Union[str, int]) -> str:
+    def _uri_encode_name(self, name: (str | int)) -> str:
         """Encode a variable name into uri encoding."""
         return self._encode(str(name), Charset.UNRESERVED + Charset.RESERVED, True) if (name) else ''
 
     def _join(self, prefix: str, joiner: str, value: str) -> str:
         """Join a prefix to a value."""
         if (prefix):
             return prefix + joiner + value
@@ -79,35 +84,35 @@
         """Encode a string value for a variable."""
         if (variable.max_length):
             if (not first):
                 raise ExpansionFailedError(str(variable))
             return self._join(prefix, joiner, self._uri_encode_value(value[:variable.max_length]))
         return self._join(prefix, joiner, self._uri_encode_value(value))
 
-    def _encode_dict_item(self, variable: Variable, name: str, key: Union[int, str], item: Any,
-                          delim: str, prefix: str, joiner: str, first: bool) -> Optional[str]:
+    def _encode_dict_item(self, variable: Variable, name: str, key: (int | str), item: Any,
+                          delim: str, prefix: str, joiner: str, first: bool) -> (str | None):
         """Encode a dict item for a variable."""
         joiner = '=' if (variable.explode) else ','
         if (variable.array):
             name = self._uri_encode_name(key)
             prefix = (prefix + '[' + name + ']') if (prefix and not first) else name
         else:
             prefix = self._join(prefix, '.', self._uri_encode_name(key))
         return self._encode_var(variable, str(key), item, delim, prefix, joiner, False)
 
     def _encode_list_item(self, variable: Variable, name: str, index: int, item: Any,
-                          delim: str, prefix: str, joiner: str, first: bool) -> Optional[str]:
+                          delim: str, prefix: str, joiner: str, first: bool) -> (str | None):
         """Encode a list item for a variable."""
         if (variable.array):
             prefix = prefix + '[' + str(index) + ']' if (prefix) else ''
             return self._encode_var(variable, '', item, delim, prefix, joiner, False)
         return self._encode_var(variable, name, item, delim, prefix, '.', False)
 
     def _encode_var(self, variable: Variable, name: str, value: Any,
-                    delim: str = ',', prefix: str = '', joiner: str = '=', first: bool = True) -> Optional[str]:
+                    delim: str = ',', prefix: str = '', joiner: str = '=', first: bool = True) -> (str | None):
         """Encode a variable."""
         if (isinstance(value, str)):
             return self._encode_str(variable, name, value, prefix, joiner, first)
         elif (isinstance(value, collections.abc.Mapping)):
             if (len(value)):
                 encoded_items = [self._encode_dict_item(variable, name, key, value[key], delim, prefix, joiner, first)
                                  for key in value.keys()]
@@ -120,19 +125,19 @@
                 return delim.join([item for item in encoded_items if (item is not None)])
             return None
         elif (isinstance(value, bool)):
             return self._encode_str(variable, name, str(value).lower(), prefix, joiner, first)
         else:
             return self._encode_str(variable, name, str(value), prefix, joiner, first)
 
-    def expand(self, values: Dict[str, Any]) -> Optional[str]:
+    def expand(self, values: Mapping[str, Any]) -> (str | None):
         """Expand values."""
         return None
 
-    def partial(self, values: Dict[str, Any]) -> str:
+    def partial(self, values: Mapping[str, Any]) -> str:
         """Perform partial expansion."""
         return ''
 
 
 class Literal(Expansion):
     """
     A literal expansion.
@@ -142,15 +147,15 @@
 
     value: str
 
     def __init__(self, value: str) -> None:
         super().__init__()
         self.value = value
 
-    def expand(self, values: Dict[str, Any]) -> Optional[str]:
+    def expand(self, values: Mapping[str, Any]) -> (str | None):
         """Perform exansion."""
         return self._encode(self.value, (Charset.UNRESERVED + Charset.RESERVED), True)
 
     def __str__(self) -> str:
         """Convert to string."""
         return self.value
 
@@ -164,15 +169,15 @@
 
     operator = ''
     partial_operator = ','
     output_prefix = ''
     var_joiner = ','
     partial_joiner = ','
 
-    vars: List[Variable]
+    vars: list[Variable]
     trailing_joiner: str = ''
 
     def __init__(self, variables: str) -> None:
         super().__init__()
         if (variables and (variables[-1] in (',', '.', '/', ';', '&'))):
             self.trailing_joiner = variables[-1]
             variables = variables[:-1]
@@ -184,37 +189,37 @@
         return list(self.vars)
 
     @property
     def variable_names(self) -> Iterable[str]:
         """Get names of all variables."""
         return [var.name for var in self.vars]
 
-    def _expand_var(self, variable: Variable, value: Any) -> Optional[str]:
+    def _expand_var(self, variable: Variable, value: Any) -> (str | None):
         """Expand a single variable."""
         return self._encode_var(variable, self._uri_encode_name(variable.name), value)
 
-    def expand(self, values: Dict[str, Any]) -> Optional[str]:
+    def expand(self, values: Mapping[str, Any]) -> (str | None):
         """Expand all variables, skip missing values."""
-        expanded_vars: List[str] = []
+        expanded_vars: list[str] = []
         for var in self.vars:
-            value = values.get(var.name, var.default)
+            value = values.get(var.key, var.default)
             if (value is not None):
                 expanded_var = self._expand_var(var, value)
                 if (expanded_var is not None):
                     expanded_vars.append(expanded_var)
         if (expanded_vars):
             return ((self.output_prefix if (not self.trailing_joiner) else '') + self.var_joiner.join(expanded_vars)
                     + self.trailing_joiner)
         return None
 
-    def partial(self, values: Dict[str, Any]) -> str:
+    def partial(self, values: Mapping[str, Any]) -> str:
         """Expand all variables, replace missing values with expansions."""
-        expanded_vars: List[str] = []
-        missing_vars: List[Variable] = []
-        result: List[Tuple[Optional[List[str]], Optional[List[Variable]]]] = []
+        expanded_vars: list[str] = []
+        missing_vars: list[Variable] = []
+        result: list[tuple[(list[str] | None), (list[Variable] | None)]] = []
         for var in self.vars:
             value = values.get(var.name, var.default)
             if (value is not None):
                 expanded_var = self._expand_var(var, value)
                 if (expanded_var is not None):
                     if (missing_vars):
                         result.append((None, missing_vars))
@@ -236,15 +241,15 @@
             last = (index == (len(result) - 1))
             if (expanded):
                 output += ((self.output_prefix if (first and (not self.trailing_joiner)) else '')
                            + self.var_joiner.join(expanded) + self.trailing_joiner)
             else:
                 output += ((self.output_prefix if (first and not last) else (self.var_joiner if (not last) else ''))
                            + '{' + (self.operator if (first) else self.partial_operator)
-                           + ','.join([str(var) for var in cast(List[Variable], missing)])
+                           + ','.join([str(var) for var in cast('list[Variable]', missing)])
                            + (self.partial_joiner if (not last) else '') + '}')
             first = False
         return output
 
     def __str__(self) -> str:
         """Convert to string."""
         return ('{' + self.operator + ','.join([str(var) for var in self.vars]) + self.trailing_joiner + '}')
@@ -306,15 +311,15 @@
     output_prefix = '.'
     var_joiner = '.'
     partial_joiner = '.'
 
     def __init__(self, variables: str) -> None:
         super().__init__(variables[1:])
 
-    def _expand_var(self, variable: Variable, value: Any) -> Optional[str]:
+    def _expand_var(self, variable: Variable, value: Any) -> (str | None):
         """Expand a single variable."""
         return self._encode_var(variable, self._uri_encode_name(variable.name), value,
                                 delim=('.' if variable.explode else ','))
 
 
 class PathExpansion(ExpressionExpansion):
     """
@@ -328,15 +333,15 @@
     output_prefix = '/'
     var_joiner = '/'
     partial_joiner = '/'
 
     def __init__(self, variables: str) -> None:
         super().__init__(variables[1:])
 
-    def _expand_var(self, variable: Variable, value: Any) -> Optional[str]:
+    def _expand_var(self, variable: Variable, value: Any) -> (str | None):
         """Expand a single variable."""
         return self._encode_var(variable, self._uri_encode_name(variable.name), value,
                                 delim=('/' if variable.explode else ','))
 
 
 class PathStyleExpansion(ExpressionExpansion):
     """
@@ -359,16 +364,16 @@
         if (variable.array):
             if (name):
                 prefix = prefix + '[' + name + ']' if (prefix) else name
         elif (variable.explode):
             prefix = self._join(prefix, '.', name)
         return super()._encode_str(variable, name, value, prefix, joiner, first)
 
-    def _encode_dict_item(self, variable: Variable, name: str, key: Union[int, str], item: Any,
-                          delim: str, prefix: str, joiner: str, first: bool) -> Optional[str]:
+    def _encode_dict_item(self, variable: Variable, name: str, key: (int | str), item: Any,
+                          delim: str, prefix: str, joiner: str, first: bool) -> (str | None):
         """Encode a dict item for a variable."""
         if (variable.array):
             if (name):
                 prefix = prefix + '[' + name + ']' if (prefix) else name
             if (prefix and not first):
                 prefix = (prefix + '[' + self._uri_encode_name(key) + ']')
             else:
@@ -378,23 +383,23 @@
         else:
             prefix = self._join(prefix, '.', self._uri_encode_name(key))
             joiner = ','
         return self._encode_var(variable, self._uri_encode_name(key) if (not variable.array) else '', item,
                                 delim, prefix, joiner, False)
 
     def _encode_list_item(self, variable: Variable, name: str, index: int, item: Any,
-                          delim: str, prefix: str, joiner: str, first: bool) -> Optional[str]:
+                          delim: str, prefix: str, joiner: str, first: bool) -> (str | None):
         """Encode a list item for a variable."""
         if (variable.array):
             if (name):
                 prefix = prefix + '[' + name + ']' if (prefix) else name
             return self._encode_var(variable, str(index), item, delim, prefix, joiner, False)
         return self._encode_var(variable, name, item, delim, prefix, '=' if (variable.explode) else '.', False)
 
-    def _expand_var(self, variable: Variable, value: Any) -> Optional[str]:
+    def _expand_var(self, variable: Variable, value: Any) -> (str | None):
         """Expand a single variable."""
         if (variable.explode):
             return self._encode_var(variable, self._uri_encode_name(variable.name), value, delim=';')
         value = self._encode_var(variable, self._uri_encode_name(variable.name), value, delim=',')
         return (self._uri_encode_name(variable.name) + '=' + value) if (value) else variable.name
 
 
@@ -410,15 +415,15 @@
     output_prefix = '?'
     var_joiner = '&'
     partial_joiner = '&'
 
     def __init__(self, variables: str) -> None:
         super().__init__(variables)
 
-    def _expand_var(self, variable: Variable, value: Any) -> Optional[str]:
+    def _expand_var(self, variable: Variable, value: Any) -> (str | None):
         """Expand a single variable."""
         if (variable.explode):
             return self._encode_var(variable, self._uri_encode_name(variable.name), value, delim='&')
         value = self._encode_var(variable, self._uri_encode_name(variable.name), value, delim=',')
         return (self._uri_encode_name(variable.name) + '=' + value) if (value is not None) else None
 
 
@@ -447,15 +452,15 @@
 
     operator = ','
     output_prefix = ','
 
     def __init__(self, variables: str) -> None:
         super().__init__(variables[1:])
 
-    def _expand_var(self, variable: Variable, value: Any) -> Optional[str]:
+    def _expand_var(self, variable: Variable, value: Any) -> (str | None):
         """Expand a single variable."""
         return self._encode_var(variable, self._uri_encode_name(variable.name), value,
                                 delim=('.' if variable.explode else ','))
 
 
 class ReservedCommaExpansion(ReservedExpansion):
     """
@@ -466,11 +471,11 @@
 
     operator = ',+'
     output_prefix = ','
 
     def __init__(self, variables: str) -> None:
         super().__init__(variables[1:])
 
-    def _expand_var(self, variable: Variable, value: Any) -> Optional[str]:
+    def _expand_var(self, variable: Variable, value: Any) -> (str | None):
         """Expand a single variable."""
         return self._encode_var(variable, self._uri_encode_name(variable.name), value,
                                 delim=('.' if variable.explode else ','))
```

### Comparing `uri_template-1.2.0/uri_template/variable.py` & `uri-template-1.3.0/uri_template/variable.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Variable class for URITemplate."""
 
-from typing import Optional
+from __future__ import annotations
 
 from .charset import Charset
 
 
 class VariableInvalidError(Exception):
     """Exception thrown for invalid variables."""
 
@@ -14,29 +14,31 @@
         self.variable = variable
 
     def __str__(self) -> str:
         """Convert to string."""
         return 'Bad variable: ' + self.variable
 
 
-class Variable(object):
+class Variable:
     """
     A template variable.
 
     https://tools.ietf.org/html/rfc6570#section-2.3
     """
 
     name: str
+    key: str
     max_length: int
     explode: bool
     array: bool
-    default: Optional[str]
+    default: (str | None)
 
     def __init__(self, var_spec: str) -> None:
         self.name = ''
+        self.key = ''
         self.max_length = 0
         self.explode = False
         self.array = False
         self.default = None
 
         if (var_spec[0:1] not in Charset.VAR_START):
             raise VariableInvalidError(var_spec)
@@ -66,21 +68,28 @@
         index = 0
         while (index < len(var_spec)):
             codepoint = var_spec[index]
             if (('%' == codepoint)
                     and ((index + 2) < len(var_spec))
                     and (var_spec[index + 1] in Charset.HEX_DIGIT)
                     and (var_spec[index + 2] in Charset.HEX_DIGIT)):
-                self.name += var_spec[index:index + 3]
+                self.key += var_spec[index:index + 3]
                 index += 2
             elif (codepoint in Charset.VAR_CHAR):
-                self.name += codepoint
+                self.key += codepoint
+            elif ('/' == codepoint):
+                self.name = self.key
+                self.key = ''
             else:
                 raise VariableInvalidError(var_spec + ((':' + str(self.max_length)) if (self.max_length) else '')
                                            + ('[]' if (self.array) else ('*' if (self.explode) else '')))
             index += 1
 
+        self.name = (self.name or self.key)
+        self.key = (self.key or self.name)
+
     def __str__(self) -> str:
         """Convert to string."""
-        return (self.name + ((':' + str(self.max_length)) if (self.max_length) else '')
+        return (self.name + (f'/{self.key}' if (self.key and (self.key != self.name)) else '')
+                + (f':{self.max_length}' if (self.max_length) else '')
                 + ('*' if (self.explode and not self.array) else '') + ('[]' if (self.array) else '')
-                + (('=' + self.default) if (self.default is not None) else ''))
+                + (f'={self.default}' if (self.default is not None) else ''))
```

### Comparing `uri_template-1.2.0/README.md` & `uri-template-1.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# uri_template
+# uri-template
 
 An implementation of RFC 6570 URI Templates.
 
 This packages implements URI Template expansion in strict adherence to RFC 6570,
 but adds a few extensions.
 
 ## RFC 6570 Extensions
@@ -38,14 +38,23 @@
 ### Default Values
 
 This package allows default string values for variables per early drafts of RFC 6570.
 e.g. "{foo=bar}" will expand to "bar" if a value for `foo` is not given.
 
 List and associtative array default values are not supported at this time.
 
+### Specifying Value Keys
+
+Sometimes a URI Template is used to provide glue between an API and a given set of data.
+In this case, the names of values needed in the final URL may not match the data provided 
+for the expansion.
+
+This package allows specifying the key used to pass data into the template. 
+e.g. "{?foo/bar}" will expand to "?foo=<the value provided as bar>"
+
 ### Partial expansion
 
 This package allows partial expansion of URI Templates.
 
 In a partial expansion, missing values preseve their expansion in the resultant output.
 e.g. a partial expansion of "{one}/{two}" with a value for `one` of "foo" and `two` missing will result in:
 "foo/{two}".
@@ -80,22 +89,22 @@
 Reserved Comma Expansion prefixes the expansion output with a single comma ",",
 but otherwise performs a Reserved Expansion ({+var}).
 
 ## API 
 
 The package provides three functions:
 
-#### uri_template.expand(template: str, **kwargs) -> Optional[str]: ...
+#### uri_template.expand(template: str, **kwargs) -> (str | None): ...
 
 Expand the given template, skipping missing values per RFC 6570.
 
 Returns `None` if the template is invalid or expansion fails.
 
 
-#### uri_template.partial(template: str, **kwargs) -> Optional[str]: ...
+#### uri_template.partial(template: str, **kwargs) -> (str | None): ...
 
 Partially expand the given template, 
 replacing missing variables with further expansions.
 
 Returns `None` if the template is invalid or expansion fails.
 
 
@@ -165,15 +174,15 @@
 
 Explode modifier is present.
 
 #### Variable.array: bool
 
 Array modifier is present.
 
-#### Variable.default: Optional[str]
+#### Variable.default: (str | None)
 
 Specified default value, or `None`.
 
 #### Variable.__str__() -> str
 
 Convert the variable back to its original string form.
```

### Comparing `uri_template-1.2.0/uri_template.egg-info/PKG-INFO` & `uri-template-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
 Name: uri-template
-Version: 1.2.0
+Version: 1.3.0
 Summary: RFC 6570 URI Template Processor
-Home-page: https://github.com/plinss/uri_template/
-Author: Peter Linss
-Author-email: pypi@linss.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Author-email: Peter Linss <pypi@linss.com>
+License: MIT License
+Project-URL: homepage, https://gitlab.linss.com/open-source/python/uri-template
+Keywords: config
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# uri_template
+# uri-template
 
 An implementation of RFC 6570 URI Templates.
 
 This packages implements URI Template expansion in strict adherence to RFC 6570,
 but adds a few extensions.
 
 ## RFC 6570 Extensions
@@ -55,14 +62,23 @@
 ### Default Values
 
 This package allows default string values for variables per early drafts of RFC 6570.
 e.g. "{foo=bar}" will expand to "bar" if a value for `foo` is not given.
 
 List and associtative array default values are not supported at this time.
 
+### Specifying Value Keys
+
+Sometimes a URI Template is used to provide glue between an API and a given set of data.
+In this case, the names of values needed in the final URL may not match the data provided 
+for the expansion.
+
+This package allows specifying the key used to pass data into the template. 
+e.g. "{?foo/bar}" will expand to "?foo=<the value provided as bar>"
+
 ### Partial expansion
 
 This package allows partial expansion of URI Templates.
 
 In a partial expansion, missing values preseve their expansion in the resultant output.
 e.g. a partial expansion of "{one}/{two}" with a value for `one` of "foo" and `two` missing will result in:
 "foo/{two}".
@@ -97,22 +113,22 @@
 Reserved Comma Expansion prefixes the expansion output with a single comma ",",
 but otherwise performs a Reserved Expansion ({+var}).
 
 ## API 
 
 The package provides three functions:
 
-#### uri_template.expand(template: str, **kwargs) -> Optional[str]: ...
+#### uri_template.expand(template: str, **kwargs) -> (str | None): ...
 
 Expand the given template, skipping missing values per RFC 6570.
 
 Returns `None` if the template is invalid or expansion fails.
 
 
-#### uri_template.partial(template: str, **kwargs) -> Optional[str]: ...
+#### uri_template.partial(template: str, **kwargs) -> (str | None): ...
 
 Partially expand the given template, 
 replacing missing variables with further expansions.
 
 Returns `None` if the template is invalid or expansion fails.
 
 
@@ -182,15 +198,15 @@
 
 Explode modifier is present.
 
 #### Variable.array: bool
 
 Array modifier is present.
 
-#### Variable.default: Optional[str]
+#### Variable.default: (str | None)
 
 Specified default value, or `None`.
 
 #### Variable.__str__() -> str
 
 Convert the variable back to its original string form.
 
@@ -224,8 +240,7 @@
 
 
 ## Installation
 
 Install with pip:
 
     pip install uri-template
-
```

### Comparing `uri_template-1.2.0/PKG-INFO` & `uri-template-1.3.0/uri_template.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
-Name: uri_template
-Version: 1.2.0
+Name: uri-template
+Version: 1.3.0
 Summary: RFC 6570 URI Template Processor
-Home-page: https://github.com/plinss/uri_template/
-Author: Peter Linss
-Author-email: pypi@linss.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Author-email: Peter Linss <pypi@linss.com>
+License: MIT License
+Project-URL: homepage, https://gitlab.linss.com/open-source/python/uri-template
+Keywords: config
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# uri_template
+# uri-template
 
 An implementation of RFC 6570 URI Templates.
 
 This packages implements URI Template expansion in strict adherence to RFC 6570,
 but adds a few extensions.
 
 ## RFC 6570 Extensions
@@ -55,14 +62,23 @@
 ### Default Values
 
 This package allows default string values for variables per early drafts of RFC 6570.
 e.g. "{foo=bar}" will expand to "bar" if a value for `foo` is not given.
 
 List and associtative array default values are not supported at this time.
 
+### Specifying Value Keys
+
+Sometimes a URI Template is used to provide glue between an API and a given set of data.
+In this case, the names of values needed in the final URL may not match the data provided 
+for the expansion.
+
+This package allows specifying the key used to pass data into the template. 
+e.g. "{?foo/bar}" will expand to "?foo=<the value provided as bar>"
+
 ### Partial expansion
 
 This package allows partial expansion of URI Templates.
 
 In a partial expansion, missing values preseve their expansion in the resultant output.
 e.g. a partial expansion of "{one}/{two}" with a value for `one` of "foo" and `two` missing will result in:
 "foo/{two}".
@@ -97,22 +113,22 @@
 Reserved Comma Expansion prefixes the expansion output with a single comma ",",
 but otherwise performs a Reserved Expansion ({+var}).
 
 ## API 
 
 The package provides three functions:
 
-#### uri_template.expand(template: str, **kwargs) -> Optional[str]: ...
+#### uri_template.expand(template: str, **kwargs) -> (str | None): ...
 
 Expand the given template, skipping missing values per RFC 6570.
 
 Returns `None` if the template is invalid or expansion fails.
 
 
-#### uri_template.partial(template: str, **kwargs) -> Optional[str]: ...
+#### uri_template.partial(template: str, **kwargs) -> (str | None): ...
 
 Partially expand the given template, 
 replacing missing variables with further expansions.
 
 Returns `None` if the template is invalid or expansion fails.
 
 
@@ -182,15 +198,15 @@
 
 Explode modifier is present.
 
 #### Variable.array: bool
 
 Array modifier is present.
 
-#### Variable.default: Optional[str]
+#### Variable.default: (str | None)
 
 Specified default value, or `None`.
 
 #### Variable.__str__() -> str
 
 Convert the variable back to its original string form.
 
@@ -224,8 +240,7 @@
 
 
 ## Installation
 
 Install with pip:
 
     pip install uri-template
-
```

