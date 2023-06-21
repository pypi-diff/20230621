# Comparing `tmp/qtgql-0.119.9.tar.gz` & `tmp/qtgql-0.120.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.119.9.tar", max compression
+gzip compressed data, was "qtgql-0.120.0.tar", max compression
```

## Comparing `qtgql-0.119.9.tar` & `qtgql-0.120.0.tar`

### file list

```diff
@@ -1,26 +1,32 @@
--rw-r--r--   0        0        0     1064 2023-06-06 13:37:08.285462 qtgql-0.119.9/LICENSE
--rw-r--r--   0        0        0     1805 2023-06-06 13:37:08.285462 qtgql-0.119.9/README.md
--rw-r--r--   0        0        0     4445 2023-06-06 13:37:29.057539 qtgql-0.119.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0        0 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/compiler/__init__.py
--rw-r--r--   0        0        0     1782 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/compiler/builtin_scalars.py
--rw-r--r--   0        0        0    13094 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/compiler/operation.py
--rw-r--r--   0        0        0     3940 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/compiler/template.py
--rw-r--r--   0        0        0     2167 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/config.py
--rw-r--r--   0        0        0     1246 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/cppref.py
--rw-r--r--   0        0        0       41 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/exceptions.py
--rw-r--r--   0        0        0     3187 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/graphql_ref.py
--rw-r--r--   0        0        0    18043 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/introspection.py
--rw-r--r--   0        0        0    12771 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/objecttype.py
--rw-r--r--   0        0        0        0 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/runtime/__init__.py
--rw-r--r--   0        0        0     1571 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/runtime/custom_scalars.py
--rw-r--r--   0        0        0      488 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0      536 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/templates/config.jinja.hpp
--rw-r--r--   0        0        0     5385 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/templates/macros.jinja.hpp
--rw-r--r--   0        0        0     5042 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0      816 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/templates/schema.jinja.cpp
--rw-r--r--   0        0        0     4552 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0     1028 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-21 14:34:56.020885 qtgql-0.120.0/LICENSE
+-rw-r--r--   0        0        0     1805 2023-06-21 14:34:56.020885 qtgql-0.120.0/README.md
+-rw-r--r--   0        0        0     4428 2023-06-21 14:35:17.905132 qtgql-0.120.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     1919 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1548 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3105 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1179 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3226 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     4207 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    13536 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0      749 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0        0 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4164 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8458 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0      445 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1524 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3059 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     1187 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0     2330 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     2930 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     4806 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3250 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    16334 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1151 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 qtgql-0.120.0/PKG-INFO
```

### Comparing `qtgql-0.119.9/LICENSE` & `qtgql-0.120.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.9/README.md` & `qtgql-0.120.0/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.9/pyproject.toml` & `qtgql-0.120.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.119.9"
+version = "0.120.0"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/nrbnlulu/qtgql"
 "Documentation" = "https://nrbnlulu.github.io/qtgql/"
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-attrs = "^22.2.0"
+attrs = ">=22.2.0"
 # codegen
 graphql-core = "^3.2.3"
 jinja2 = {version = "^3.1.2", optional=true}
-typingref = "^0.100.0"
 typer = "^0.9.0"
 rich = "^13.3.5"
 frozendict = "^2.3.8"
 
 
 
 [tool.poetry.group.dev.dependencies]
-pytest-cov = "^4.0.0"
 aiohttp = {extras = ["speedups"], version = "^3.8.3"}
 faker = ">=15.3.4,<19.0.0"
 mypy = ">=1.0.1"
 strawberry-graphql = ">=0.158.2"
-aqtinstall = ">=3.1.6"
+aqtinstall = "v3.1.6"
 conan = ">=2.0.4"
 cmake = ">=3.25.0"
 pygithub = ">=1.58.2"
 githubrelease = ">=1.5.9"
 httpx = ">=0.18.2"
-autopub = ">=0.2.2"
+autopub = "0.3.0"
 mimesis = ">=10.1.0"
+pytest = "7.3.1"
+pytest-cov = ">=4.1.0"
+
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.0.5"
 mike = "^1.1.2"
 markdown-include = "^0.8.0"
 mkdocstrings = {extras = ["python"], version = ">=0.19.1,<0.22.0"}
 pygments = "^2.14.0"
@@ -84,15 +85,14 @@
 '''
 
 [tool.ruff]
 line-length = 100
 select = ["ALL"]
 target-version = "py38"
 ignore = [
-    "I001", # isort, handled by pc-hook.
     "TID252",
     # we use asserts in tests and to hint mypy
     "E501", # line too long, handled by black.
     "S101",
     "S102",
     "S104",
     "S324",
@@ -124,16 +124,14 @@
     "N811",
     "N804",
     "N818",
     # Variable `T` in function should be lowercase
     # this seems a potential bug or opportunity for improvement in ruff
     "N806",
 
-    # first argument should named self (found in tests)
-    "N805",
 
     "N815",
 
     # shadowing builtins
     "A001",
     "A002",
     "A003",
@@ -204,30 +202,38 @@
 
     "PLR",
     "INP",
     "TRY",
     "SIM300",
     "SIM114",
     "DJ008",
+
+    # https://beta.ruff.rs/docs/rules/#flake8-fixme-fix
+    "FIX002",
+    # https://beta.ruff.rs/docs/rules/#flake8-bandit-s
+    "S603",
+    "S607",
+    "TD002",
+    "TD003",
 ]
+
 fix = true
 src = ["qtgqlcodegen", "tests"]
 [tool.ruff.flake8-annotations]
 suppress-none-returning = true
 
-[tool.ruff.pyupgrade]
-keep-runtime-typing = true
-
+[tool.ruff.isort]
+combine-as-imports = true
 
 [tool.pytest.ini_options]
 addopts = "--cov-config=pyproject.toml --ignore=qtgqlcodegen/codegen/py/templates/"
-markers = [
-    "no_captcha: This test requires that `LOGIN_REQUIRE_CAPTCHA=False` on the server",
-]
+
+
 [tool.coverage.run]
+source = ["qtgqlcodegen"]
 omit = ['test_*', 'tests/*', '**/*.jinja.py']
 relative_files = true
 
 [tool.coverage.report]
 show_missing = true
 exclude_lines = [
   "pragma: no cover",
```

### Comparing `qtgql-0.119.9/qtgqlcodegen/cli.py` & `qtgql-0.120.0/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.9/qtgqlcodegen/compiler/operation.py` & `qtgql-0.120.0/qtgqlcodegen/operation/evaluation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,355 +1,390 @@
 from __future__ import annotations
 
-import uuid
 from collections import defaultdict
-from functools import cached_property
-from typing import Optional
 from typing import TYPE_CHECKING
 
-import attrs
 import graphql
-from attr import define
-from frozendict import frozendict
-from typingref import UNSET
-
-from qtgqlcodegen.compiler.template import config_template
-from qtgqlcodegen.compiler.template import ConfigContext
-from qtgqlcodegen.graphql_ref import has_id_selection
-from qtgqlcodegen.graphql_ref import has_typename_selection
-from qtgqlcodegen.graphql_ref import inject_id_selection
-from qtgqlcodegen.graphql_ref import inject_typename_selection
-from qtgqlcodegen.graphql_ref import is_field_node
-from qtgqlcodegen.graphql_ref import is_inline_fragment
+from graphql import OperationDefinitionNode, OperationType, language as gql_lang
+from graphql.language import visitor
 
-if TYPE_CHECKING:
-    from graphql import language as gql_lang
-    from graphql.type import definition as gql_def
+from qtgqlcodegen.core.graphql_ref import (
+    has_id_selection,
+    has_typename_selection,
+    inject_id_selection,
+    inject_typename_selection,
+    is_field_node,
+    is_inline_fragment,
+    is_named_type_node,
+    is_nonnull_node,
+    is_operation_def_node,
+)
+from qtgqlcodegen.operation.definitions import (
+    OperationTypeInfo,
+    QtGqlOperationDefinition,
+    QtGqlQueriedField,
+    QtGqlVariableUse,
+)
+from qtgqlcodegen.schema.definitions import (
+    QtGqlFieldDefinition,
+    QtGqlVariableDefinition,
+    SchemaTypeInfo,
+)
+from qtgqlcodegen.schema.evaluation import evaluate_graphql_type
+from qtgqlcodegen.types import (
+    QtGqlInterface,
+    QtGqlList,
+    QtGqlOptional,
+    QtGqlQueriedInterface,
+    QtGqlQueriedObjectType,
+    QtGqlQueriedUnion,
+    QtGqlUnion,
+)
+from qtgqlcodegen.utils import require
 
-    from qtgqlcodegen.introspection import SchemaEvaluator
-    from qtgqlcodegen.objecttype import QtGqlVariableDefinition, GqlTypeHinter
-    from qtgqlcodegen.objecttype import QtGqlFieldDefinition
-    from qtgqlcodegen.objecttype import QtGqlObjectTypeDefinition
+if TYPE_CHECKING:
+    from qtgqlcodegen.types import QtGqlObjectType, QtGqlTypeABC
 
 
 def is_type_name_selection(field_node: gql_lang.FieldNode):
     # typename is not a 'real' selection and is handled with special care.
     if field_node.name.value == "__typename":
         return True
     return False
 
 
-def get_field_from_field_node(
-    selection: gql_lang.FieldNode,
-    field_type: QtGqlObjectTypeDefinition,
-    operation: QtGqlOperationDefinition,
-    parent_interface_field: Optional[QtGqlQueriedField] = UNSET,
-) -> QtGqlQueriedField:
-    field_node = is_field_node(selection)
-    assert field_node
-    return QtGqlQueriedField.from_field(
-        field_type.fields_dict[field_node.name.value],
-        selection_set=field_node.selection_set,
-        operation=operation,
-        parent_interface_field=parent_interface_field,
+def _evaluate_variable_uses(
+    type_info: OperationTypeInfo,
+    field: QtGqlFieldDefinition,
+    arguments: tuple[gql_lang.ArgumentNode, ...],
+) -> list[QtGqlVariableUse]:
+    ret: list[QtGqlVariableUse] = []
+    for arg in arguments:
+        index = field.index_for_argument(arg.name.value)
+        var_name = arg.value.name.value  # type: ignore[attr-defined]
+        for variable in type_info.variables:
+            if var_name == variable.name:
+                ret.append(
+                    QtGqlVariableUse(argument=(index, field.arguments[index]), variable=variable),
+                )
+    assert len(ret) == len(arguments), "could not find all variable uses"
+    return ret
+
+
+def _evaluate_variable_node_type(
+    type_info: SchemaTypeInfo,
+    node: graphql.TypeNode,
+) -> QtGqlTypeABC:
+    if nonnull := is_nonnull_node(node):
+        return evaluate_graphql_type(
+            type_info,
+            graphql.type.GraphQLNonNull(
+                type_info.schema_definition.get_type(nonnull.type.name.value),  # type: ignore
+            ),
+        )
+
+    if named_type := is_named_type_node(node):
+        gql_concrete = type_info.schema_definition.get_type(named_type.name.value)
+        assert gql_concrete
+        return evaluate_graphql_type(type_info, gql_concrete)
+    raise NotImplementedError(node, "Type is not supported as a variable ATM")
+
+
+def _evaluate_variable(
+    type_info: SchemaTypeInfo,
+    var: gql_lang.VariableDefinitionNode,
+) -> QtGqlVariableDefinition:
+    return QtGqlVariableDefinition(
+        name=var.variable.name.value,
+        type=_evaluate_variable_node_type(type_info, var.type),
     )
 
 
-@attrs.define(frozen=True, slots=False)
-class QtGqlQueriedField:
-    definition: QtGqlFieldDefinition
-    operation: QtGqlOperationDefinition
-    choices: frozendict[str, dict[str, QtGqlQueriedField]] = attrs.Factory(frozendict)
-    selections: dict[str, QtGqlQueriedField] = attrs.Factory(dict)
-    narrowed_type: Optional[QtGqlQueriedObjectType] = None
-    is_root: bool = False
-
-    def __repr__(self):
-        return (
-            f"{self.definition.name}[{', '.join(self.selections.keys())}\n"
-            + "...on".join([f"{k} {repr(v)}" for k, v in self.choices.items()])
-            + "]"
+def _evaluate_selection_set_type(
+    type_info: OperationTypeInfo,
+    concrete_type: QtGqlTypeABC,
+    selection_set_node: gql_lang.SelectionSetNode | None,
+    path: str,
+) -> QtGqlTypeABC:
+    ret: QtGqlTypeABC | None = None
+    if not selection_set_node:
+        # these types have no selections
+        assert (
+            concrete_type.is_builtin_scalar
+            or concrete_type.is_custom_scalar
+            or concrete_type.is_enum
+        )
+        ret = concrete_type  # currently there is no need for a "proxied" type.
+
+    elif obj_type := concrete_type.is_object_type:
+        ret = _evaluate_object_type(
+            type_info=type_info,
+            concrete=obj_type,
+            selection_set=selection_set_node,
+            path=path,
         )
+    elif lst := concrete_type.is_model:
+        ret = _evaluate_list(
+            type_info=type_info,
+            concrete=lst,
+            selection_set=selection_set_node,
+            path=path,
+        )
+    elif interface := concrete_type.is_interface:
+        ret = _evaluate_interface(
+            type_info=type_info,
+            concrete=interface,
+            selection_set=selection_set_node,
+            path=path,
+        )
+    elif is_union := concrete_type.is_union:
+        ret = _evaluate_union(
+            type_info=type_info,
+            concrete=is_union,
+            selection_set=selection_set_node,
+            path=path,
+        )
+    if not ret:  # pragma: no cover
+        raise NotImplementedError(f"type {concrete_type} not supported yet")
+
+    if concrete_type.is_optional:
+        return QtGqlOptional(of_type=ret)
+    return ret
+
+
+def _evaluate_field(
+    type_info: OperationTypeInfo,
+    concrete_field: QtGqlFieldDefinition,
+    field_node: gql_lang.FieldNode,
+    path: str,
+    origin: QtGqlObjectType,
+) -> QtGqlQueriedField:
+    path += concrete_field.name
+    return QtGqlQueriedField(
+        type=_evaluate_selection_set_type(
+            type_info,
+            concrete_field.type,
+            field_node.selection_set,
+            path,
+        ),
+        concrete=concrete_field,
+        variable_uses=_evaluate_variable_uses(type_info, concrete_field, field_node.arguments),
+        origin=origin,
+        type_info=type_info,
+    )
+
 
-    @cached_property
-    def type(self) -> GqlTypeHinter:
-        return self.definition.type
-
-    @cached_property
-    def type_name(self) -> str:
-        if self.type.is_object_type:
-            assert self.narrowed_type
-            return self.narrowed_type.name
-
-        if model_of := self.type.is_model:
-            if model_of.is_object_type:
-                assert self.narrowed_type
-                return f"qtgql::bases::ListModelABC<{self.narrowed_type.name}>"
-
-        return self.type.member_type
-
-    @cached_property
-    def property_type(self) -> str:
-        tp = self.definition.type
-        if tp.is_object_type:
-            assert self.narrowed_type
-            return f"{self.type_name} *"
-
-        if cs := tp.is_custom_scalar:
-            return cs.type_for_proxy
-
-        if model_of := tp.is_model:
-            if model_of.is_object_type:
-                return f"{self.type_name} *"
-
-        return self.type_name
-
-    @cached_property
-    def name(self) -> str:
-        if self.is_root:
-            return "data"
-        return self.definition.name
-
-    @cached_property
-    def private_name(self):
-        if self.is_root:
-            return f"m_{self.name}"
-        return self.definition.private_name
-
-    @classmethod
-    def from_field(
-        cls,
-        field_definition: QtGqlFieldDefinition,
-        selection_set: Optional[gql_lang.SelectionSetNode],
-        operation: QtGqlOperationDefinition,
-        parent_interface_field: Optional[QtGqlQueriedField] = UNSET,
-        is_root: bool = False,
-    ) -> QtGqlQueriedField:
-        """Main purpose here is to find inner selections of fields, this could
-        be an object type, interface, union or a list.
-
-        Any other fields should not have inner selections.
-        """
-        assert parent_interface_field is not UNSET
-        if not hasattr(selection_set, "selections"):
-            return cls(definition=field_definition, operation=operation, is_root=is_root)
-        assert selection_set
-        tp = field_definition.type
-        if (
-            tp.is_model
-        ):  # GraphQL's lists are basically the object beneath them in terms of selections.
-            tp = tp.is_model
-
-        tp_is_union = tp.is_union
-
-        # inject id selection for types that supports it. unions are handled below.
-        if field_definition.can_select_id and not has_id_selection(selection_set):
-            inject_id_selection(selection_set)
-
-        selections: dict[str, QtGqlQueriedField] = {}
-        choices: defaultdict[str, dict[str, QtGqlQueriedField]] = defaultdict(dict)
-        narrowed_type: Optional[QtGqlQueriedObjectType] = None
-        # inject parent interface selections.
-        if (tp.is_object_type or tp.is_interface) and parent_interface_field:
-            selections.update({f.name: f for f in parent_interface_field.selections.values()})
-
-        if tp_is_union:
-            for selection in selection_set.selections:
-                fragment = is_inline_fragment(selection)
-                assert fragment
-
-                type_name = fragment.type_condition.name.value
-                concrete = operation.evaluator.get_objecttype_by_name(type_name)
-                assert concrete
-                if not has_typename_selection(fragment.selection_set):
-                    inject_typename_selection(fragment.selection_set)
-                if not has_id_selection(fragment.selection_set) and concrete.implements_node:
-                    inject_id_selection(fragment.selection_set)
-
-                for selection_node in fragment.selection_set.selections:
-                    field_node = is_field_node(selection_node)
-                    assert field_node
-
-                    if not is_type_name_selection(field_node):
-                        __f = get_field_from_field_node(
-                            field_node,
-                            concrete,
-                            operation,
-                            parent_interface_field,
-                        )
-                        choices[type_name][field_definition.name] = __f
-
-        elif interface_def := tp.is_interface:
-            # first get all linear selections.
-            for selection in selection_set.selections:
-                if not is_inline_fragment(selection):
-                    field_node = is_field_node(selection)
-                    assert field_node
-                    if not is_type_name_selection(field_node):
-                        __f = get_field_from_field_node(
-                            field_node,
-                            interface_def,
-                            operation,
-                            parent_interface_field,
-                        )
-                        selections[__f.name] = __f
-
-            for selection in selection_set.selections:
-                if inline_frag := is_inline_fragment(selection):
-                    type_name = inline_frag.type_condition.name.value
-                    # no need to validate inner types are implementation, graphql-core does this.
-                    concrete = operation.evaluator.get_objecttype_by_name(
-                        type_name,
-                    ) or operation.evaluator.get_interface_by_name(type_name)
-                    assert concrete
-                    for inner_selection in inline_frag.selection_set.selections:
-                        field_node = is_field_node(inner_selection)
-                        assert field_node
-                        if not is_type_name_selection(field_node):
-                            __f = get_field_from_field_node(
-                                field_node,
-                                concrete,
-                                operation,
-                                parent_interface_field,
-                            )
-                            choices[type_name][field_definition.name] = __f
-
-        else:  # object types.
-            obj_def = tp.is_object_type
-            assert obj_def
-            for selection in selection_set.selections:
-                field_node = is_field_node(selection)
-                assert field_node
-                if not is_type_name_selection(field_node):
-                    __f = get_field_from_field_node(
-                        field_node,
-                        obj_def,
-                        operation,
-                        parent_interface_field,
+def _evaluate_list(
+    type_info: OperationTypeInfo,
+    concrete: QtGqlList,
+    selection_set: gql_lang.SelectionSetNode,
+    path: str,
+) -> QtGqlList:
+    return QtGqlList(
+        of_type=_evaluate_selection_set_type(
+            type_info,
+            concrete_type=concrete.of_type,
+            selection_set_node=selection_set,
+            path=path,
+        ),
+    )
+
+
+def _evaluate_union(
+    type_info: OperationTypeInfo,
+    concrete: QtGqlUnion,
+    selection_set: gql_lang.SelectionSetNode,
+    path: str,
+) -> QtGqlQueriedUnion:
+    choices: defaultdict[str, dict[str, QtGqlQueriedField]] = defaultdict(dict)
+    for selection in selection_set.selections:
+        fragment = is_inline_fragment(selection)
+        assert fragment
+        type_name = fragment.type_condition.name.value
+        # unions support only object types http://spec.graphql.org/October2021/#sec-Unions
+        resolved_type = require(concrete.get_by_name(type_name))
+        if not has_typename_selection(fragment.selection_set):
+            inject_typename_selection(fragment.selection_set)
+        if not has_id_selection(fragment.selection_set) and resolved_type.implements_node:
+            inject_id_selection(fragment.selection_set)
+
+        for selection_node in fragment.selection_set.selections:
+            inner_field_node = require(is_field_node(selection_node))
+            if not is_type_name_selection(inner_field_node):
+                concrete_field = resolved_type.fields_dict[inner_field_node.name.value]
+                __f = _evaluate_field(
+                    type_info=type_info,
+                    concrete_field=concrete_field,
+                    field_node=inner_field_node,
+                    path=path,
+                    origin=resolved_type,
+                )
+                choices[type_name][concrete_field.name] = __f
+
+    return QtGqlQueriedUnion(
+        concrete=concrete,
+        choices=choices,
+    )
+
+
+def _evaluate_interface(
+    type_info: OperationTypeInfo,
+    concrete: QtGqlInterface,
+    selection_set: gql_lang.SelectionSetNode,
+    path: str,  # current path in the query tree.
+) -> QtGqlQueriedInterface:
+    # first get all linear selections.
+    linear_fields: dict[str, QtGqlQueriedField] = {}
+    choices: defaultdict[str, dict[str, QtGqlQueriedField]] = defaultdict(dict)
+
+    for selection in selection_set.selections:
+        if not is_inline_fragment(selection):
+            inner_field_node = is_field_node(selection)
+            assert inner_field_node
+            if not is_type_name_selection(inner_field_node):
+                __f = _evaluate_field(
+                    type_info=type_info,
+                    concrete_field=concrete.fields_dict[inner_field_node.name.value],
+                    field_node=inner_field_node,
+                    path=path,
+                    origin=concrete,
+                )
+                linear_fields[__f.name] = __f
+
+    # evaluate type conditions
+    for selection in selection_set.selections:
+        if inline_frag := is_inline_fragment(selection):
+            type_name = inline_frag.type_condition.name.value
+            # no need to validate inner types are implementation, graphql-core does this.
+            resolved_type = type_info.schema_type_info.get_object_type(
+                type_name,
+            ) or type_info.schema_type_info.get_interface(type_name)
+            assert resolved_type
+            for inner_selection in inline_frag.selection_set.selections:
+                inner_field_node = is_field_node(inner_selection)
+                assert inner_field_node
+                if not is_type_name_selection(inner_field_node):
+                    __f = _evaluate_field(
+                        type_info=type_info,
+                        concrete_field=resolved_type.fields_dict[inner_field_node.name.value],
+                        field_node=inner_field_node,
+                        path=path,
+                        origin=resolved_type,
                     )
-                    selections[__f.name] = __f
-            queried_obj = QtGqlQueriedObjectType(
-                definition=obj_def,
-                fields_dict=selections,
-            )
-            operation.narrowed_types_map[queried_obj.name] = queried_obj
-            narrowed_type = queried_obj
+                    choices[type_name][inner_field_node.name.value] = __f
+    for choice in choices.values():
+        choice.update(linear_fields)
+
+    name = f"{concrete.name}__{path}"
+    ret = QtGqlQueriedInterface(
+        name=name,
+        concrete=concrete,
+        choices=choices,
+        fields_dict=linear_fields,
+    )
+    type_info.narrowed_interfaces_map[name] = ret
+    return ret
 
-        def sorted_distinct_fields(
-            fields: dict[str, QtGqlQueriedField],
-        ) -> dict[str, QtGqlQueriedField]:
-            return dict(sorted(fields.items()))
-
-        return cls(
-            definition=field_definition,
-            selections=sorted_distinct_fields(selections),
-            choices=frozendict({k: sorted_distinct_fields(v) for k, v in choices.items()}),
-            operation=operation,
-            narrowed_type=narrowed_type,
-            is_root=is_root,
-        )
 
-    def as_conf_string(self) -> str:
-        return config_template(
-            context=ConfigContext(self),
-        )
+def _evaluate_object_type(
+    type_info: OperationTypeInfo,
+    concrete: QtGqlObjectType,
+    selection_set: gql_lang.SelectionSetNode,
+    path: str,  # current path in the query tree.
+) -> QtGqlQueriedObjectType:
+    # inject id selection for node implementors, it is required for caching purposes.
+    if concrete.implements_node and not has_id_selection(selection_set):
+        inject_id_selection(selection_set)
+
+    fields: dict[str, QtGqlQueriedField] = {}
+    for selection in selection_set.selections:
+        if f_node := is_field_node(selection):
+            concrete_field = concrete.fields_dict[f_node.name.value]
+            fields[concrete_field.name] = _evaluate_field(
+                type_info=type_info,
+                concrete_field=concrete_field,
+                field_node=f_node,
+                path=path,
+                origin=concrete,
+            )
 
+    name = f"{concrete.name}__{path}"
+    if ret := type_info.narrowed_types_map.get(name, None):
+        return ret
+
+    ret = QtGqlQueriedObjectType(
+        name=name,
+        concrete=concrete,
+        fields_dict=fields,
+    )
+    type_info.narrowed_types_map[name] = ret
+    return ret
 
-@define(slots=False)
-class QtGqlQueriedObjectType:
-    definition: QtGqlObjectTypeDefinition = attrs.field(on_setattr=attrs.setters.frozen)
-    fields_dict: dict[str, QtGqlQueriedField] = attrs.Factory(dict)
-    is_root_field: bool = False
-
-    @cached_property
-    def fields(self) -> tuple[QtGqlQueriedField, ...]:
-        return tuple(self.fields_dict.values())
-
-    @cached_property
-    def name(self) -> str:
-        return f"{self.definition.name}__{'$'.join(sorted(self.fields_dict.keys()))}"
-
-    @cached_property
-    def doc_fields(self) -> str:
-        return "{} {{\n  {}\n}}".format(
-            self.definition.name,
-            "\n   ".join(self.fields_dict.keys()),
-        )
 
-    @cached_property
-    def references(self) -> list[QtGqlQueriedField]:
-        return [f for f in self.fields if f.type.is_object_type]
-
-    @cached_property
-    def models(self) -> list[QtGqlQueriedField]:
-        return [f for f in self.fields if f.type.is_model]
-
-    @cached_property
-    def private_name(self) -> str:
-        return f"m_{self.name}"
-
-
-@define(slots=False)
-class QtGqlOperationDefinition:
-    operation_def: gql_def.OperationDefinitionNode
-    evaluator: SchemaEvaluator
-    directives: list[str] = attrs.Factory(list)
-    fragments: list[str] = attrs.Factory(list)
-    variables: list[QtGqlVariableDefinition] = attrs.Factory(list)
-    narrowed_types_map: dict[str, QtGqlQueriedObjectType] = attrs.Factory(dict)
-
-    @cached_property
-    def operation_id(self) -> str:
-        return uuid.uuid4().hex
-
-    def __attrs_post_init__(self) -> None:
-        # instantiating the queried fields here, they build the narrowed types.
-        self.root_field  # noqa
-
-    @property
-    def operation_config(self) -> str:
-        return self.root_field.as_conf_string()
-
-    @property
-    def name(self) -> str:
-        assert self.operation_def.name
-        return self.operation_def.name.value
-
-    @cached_property
-    def query(self) -> str:
-        return graphql.print_ast(self.operation_def)
-
-    @cached_property
-    def narrowed_types(self) -> tuple[QtGqlQueriedObjectType, ...]:
-        return tuple(self.narrowed_types_map.values())
-
-    @cached_property
-    def _root_type(self) -> QtGqlObjectTypeDefinition:
-        root_type = self.evaluator.operation_types.get(self.operation_def.operation, None)
-        assert root_type, f"You don't have a {self.operation_def.operation} type on your schema"
-        return root_type
-
-    @cached_property
-    def root_field(self) -> QtGqlQueriedField:
-        root_field_def: gql_lang.FieldNode = self.operation_def.selection_set.selections[0]  # type: ignore
-        return QtGqlQueriedField.from_field(
-            self._root_type.fields_dict[root_field_def.name.value],
-            root_field_def.selection_set,
-            self,
-            parent_interface_field=None,
-            is_root=True,
-        )
+def _evaluate_operation(
+    operation: OperationDefinitionNode,
+    schema_type_info: SchemaTypeInfo,
+) -> QtGqlOperationDefinition:
+    """Each operation generates a whole new "proxy" schema. That schema will
+    contain only the fields that are currently queried. The way we do that is
+    creating a so-called "proxy objects".
+
+    - Each proxy object mirrors a concrete object at schema level.
+    - Each proxy object contains only the fields that was queried for this field in the tree.
+
+    And because of that, one object type (at the concrete schema) might have many proxy objects.
+    """
+    type_info = OperationTypeInfo(schema_type_info)
+
+    # input variables
+    if variables_def := operation.variable_definitions:
+        for var in variables_def:
+            type_info.variables.append(_evaluate_variable(type_info.schema_type_info, var))
+
+    selections = operation.selection_set
+    root_type = type_info.schema_type_info.operation_types[operation.operation.value]
+    assert root_type, f"Make sure you have {operation.operation.name} type defined in your schema"
+    root_proxy_type = _evaluate_object_type(
+        type_info=type_info,
+        concrete=root_type,
+        selection_set=selections,
+        path="",
+    )
+    assert len(root_proxy_type.fields) == 1
+    root_field = root_proxy_type.fields[0]
+    return QtGqlOperationDefinition(
+        root_field=root_field,
+        root_type=root_proxy_type,
+        operation_def=operation,
+        variables=type_info.variables,
+        narrowed_types=tuple(type_info.narrowed_types_map.values()),
+    )
 
-    @classmethod
-    def from_definition(
-        cls,
-        operation_def: gql_def.OperationDefinitionNode,
-        evaluator: SchemaEvaluator,
-        directives: list[str],
-        variables: list[QtGqlVariableDefinition],
-    ):
-        return cls(
-            operation_def=operation_def,
-            evaluator=evaluator,
-            directives=directives,
-            variables=variables,
-        )
+
+class _OperationsVisitor(visitor.Visitor):
+    def __init__(self, type_info: SchemaTypeInfo):
+        super().__init__()
+        self.schema_type_info = type_info
+        self.operations: dict[str, QtGqlOperationDefinition] = {}
+
+    def enter_operation_definition(self, node, key, parent, path, ancestors) -> None:
+        if operation := is_operation_def_node(node):
+            if operation.operation in (
+                OperationType.QUERY,
+                OperationType.MUTATION,
+                OperationType.SUBSCRIPTION,
+            ):
+                assert operation.name, "QtGql enforces operations to have names."
+                self.operations[operation.name.value] = _evaluate_operation(
+                    operation,
+                    self.schema_type_info,
+                )
+
+
+def evaluate_operations(
+    operations_document: graphql.DocumentNode,
+    type_info: SchemaTypeInfo,
+) -> dict[str, QtGqlOperationDefinition]:
+    operation_visitor = _OperationsVisitor(type_info)
+    graphql.visit(operations_document, operation_visitor)
+    assert operation_visitor.operations
+    return operation_visitor.operations
```

### Comparing `qtgql-0.119.9/qtgqlcodegen/graphql_ref.py` & `qtgql-0.120.0/qtgqlcodegen/core/graphql_ref.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from __future__ import annotations
 
-from typing import Callable
-from typing import Optional
-from typing import Type
-from typing import TypeVar
+from typing import Callable, TypeVar
 
 from graphql import language as gql_lang
 from graphql.type import definition as gql_def
 
 T_AST_Node = TypeVar("T_AST_Node", bound=gql_lang.Node)
 
 
 def ast_identifier_factory(
-    expected: Type[T_AST_Node],
-) -> Callable[[gql_lang.Node], Optional[T_AST_Node]]:
-    def type_guarder(node: gql_lang.ast.Node) -> Optional[T_AST_Node]:
+    expected: type[T_AST_Node],
+) -> Callable[[gql_lang.Node], T_AST_Node | None]:
+    def type_guarder(node: gql_lang.ast.Node) -> T_AST_Node | None:
         if isinstance(node, expected):
             return node
 
     return type_guarder
 
 
 is_selection_set = ast_identifier_factory(gql_lang.ast.SelectionSetNode)
@@ -29,17 +26,17 @@
 is_named_type_node = ast_identifier_factory(gql_lang.NamedTypeNode)
 
 
 T_Definition = TypeVar("T_Definition", bound=gql_def.GraphQLType)
 
 
 def definition_identifier_factory(
-    expected: Type[T_Definition],
-) -> Callable[[gql_def.GraphQLType], Optional[T_Definition]]:
-    def type_guarder(definition: gql_def.GraphQLType) -> Optional[T_Definition]:
+    expected: type[T_Definition],
+) -> Callable[[gql_def.GraphQLType], T_Definition | None]:
+    def type_guarder(definition: gql_def.GraphQLType) -> T_Definition | None:
         if isinstance(definition, expected):
             return definition
 
     return type_guarder
 
 
 is_object_definition = definition_identifier_factory(gql_def.GraphQLObjectType)
```

### Comparing `qtgql-0.119.9/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.120.0/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,150 +1,148 @@
-{% import "macros.jinja.hpp" as macros -%}
+{%- from "macros/initialize_proxy_field.jinja.hpp" import initialize_proxy_field -%}
+{%- from "macros/deserialize_concrete_field.jinja.hpp" import  deserialize_concrete_field -%}
 #pragma once
 #include "./schema.hpp"
 #include <qtgql/gqlwstransport/gqlwstransport.hpp>
 #include <QObject>
 
-namespace 👉 context.config.env_name 👈{
-namespace 👉context.ns👈{
+namespace 👉 context.config.env_name 👈::👉context.ns👈{
+class 👉 context.operation.name 👈;
 
+namespace deserializers{
+{% for t in context.operation.narrowed_types -%}
+std::shared_ptr<👉 t.concrete.name 👈> des_👉 t.name 👈(const QJsonObject& data, const 👉 context.operation.name 👈 * operation);
+{% endfor -%}
+{% for t in context.operation.interfaces -%}
+std::shared_ptr<👉 t.concrete.name 👈> des_👉 t.name 👈(const QJsonObject& data, const 👉 context.operation.name 👈 * operation);
+{% endfor -%}
+};
+
+namespace updaters{
+{% for t in context.operation.narrowed_types -%}
+void update_👉 t.name 👈(👉 t.concrete.member_type 👈 &inst, const QJsonObject &data, const 👉 context.operation.name 👈 * operation);
+{% endfor -%}
+
+};
+
+// ------------ Narrowed Object types ------------
 {% for t in context.operation.narrowed_types %}
 class 👉 t.name 👈: public QObject{
-/*
-👉 t.doc_fields 👈
- */
     Q_OBJECT
 {% for f in t.fields -%}
-Q_PROPERTY(const 👉 f.property_type 👈 👉 f.name 👈 READ 👉 f.definition.getter_name 👈 NOTIFY 👉 f.definition.signal_name 👈);
+Q_PROPERTY(const 👉 f.property_type 👈 👉 f.name 👈 READ 👉 f.concrete.getter_name 👈 NOTIFY 👉 f.concrete.signal_name 👈);
 {% endfor %}
 signals:
 {%for f in t.fields -%}
-void 👉 f.definition.signal_name 👈();
+void 👉 f.concrete.signal_name 👈();
 {% endfor %}
 
 {# members #}
 {% if context.debug -%}
 public: // WARNING: members are public because you have debug=True in your config file.
 {% else %}
 protected:
 {% endif %}
-std::shared_ptr<👉context.schema_ns👈::👉 t.definition.name 👈> m_inst;
+const std::shared_ptr<👉context.schema_ns👈::👉 t.concrete.name 👈> m_inst;
 {% for ref_field in t.references -%}
-👉ref_field.property_type👈 m_👉ref_field.name👈 = {};
+const 👉ref_field.property_type👈 m_👉ref_field.name👈 = {};
 {% endfor %}
 {%- for model_field in t.models -%}
 👉 model_field.property_type 👈 m_👉model_field.name👈;
 {% endfor %}
 
 public:
-👉 t.name 👈(QObject * parent,
-        const std::shared_ptr<👉 t.definition.name 👈> &inst,
-        qtgql::bases::OperationMetadata & metadata): m_inst{inst}, QObject::QObject(parent){
-{% for field in t.fields -%}
-👉 macros.initialize_proxy_field(field) 👈
-{# updates logic -#}
-connect(m_inst.get(), &👉context.schema_ns👈::👉t.definition.name👈::👉 field.definition.signal_name 👈, this,
-        [&](){emit 👉 field.definition.signal_name 👈();});
-{% endfor %}
-}
-{%- for f in t.fields %}
-{% if f.type.is_object_type or f.type.is_model %}
-[[nodiscard]] inline const 👉 f.property_type 👈  👉 f.definition.getter_name 👈() const {
+👉 t.name 👈(👉 context.operation.name 👈 * operation, const std::shared_ptr<👉 t.concrete.name 👈> &inst);
+
+{% for f in t.fields -%}
+{%- if f.type.is_queried_object_type or f.type.is_model %}
+[[nodiscard]] inline const 👉 f.property_type 👈  👉 f.concrete.getter_name 👈() const {
     return m_👉f.name👈;
-{% else %}
-{# TODO: this is probably redundan #}
-[[nodiscard]] inline const 👉 f.property_type 👈 & 👉 f.definition.getter_name 👈() const {
-    {% if f.type.is_object_type %}
+{%- else -%}
+[[nodiscard]] inline const 👉 f.property_type 👈 👉 f.concrete.getter_name 👈() const {
+    {% if f.type.is_queried_object_type -%}
     return *m_👉f.name👈;
-    {% else %}
-    return m_inst->👉 f.definition.getter_name 👈();
-    {% endif %}
-{% endif %}
+    {% else -%}
+    return m_inst->👉 f.concrete.getter_name 👈();
+    {% endif -%}
+{%- endif -%}
 };
 {% endfor -%}
 };
 {% endfor %}
-class 👉 context.operation.name 👈: public qtgql::gqlwstransport::OperationHandlerABC {
+
+struct 👉 context.operation.generated_variables_type 👈{
+{% for var in context.operation.variables -%}
+std::optional<👉 var.type.member_type 👈> 👉 var.name 👈 = {};
+{% endfor -%}
+
+    QJsonObject to_json() const{
+    QJsonObject ret;
+    {% for var in context.operation.variables -%}
+    if (👉 var.name 👈.has_value()){
+    ret.insert("👉 var.name 👈",  👉 var.json_repr() 👈);
+    }
+    {% endfor -%}
+    return ret;
+    }
+};
+
+class 👉 context.operation.name 👈: public qtgql::gqlwstransport::OperationHandlerABC{
     Q_OBJECT
-Q_PROPERTY(const 👉 context.operation.root_field.property_type 👈 data READ get_data NOTIFY dataChanged);
+Q_PROPERTY(const 👉 context.operation.root_type.name 👈 * data READ data NOTIFY dataChanged);
 
-std::optional<👉 context.operation.root_field.property_type 👈> m_data = {};
+std::optional<👉 context.operation.root_type.name 👈 *> m_data = {};
 
 
 
 inline const QString &ENV_NAME() override{
     static const auto ret = QString("👉 context.config.env_name 👈");
     return ret;
     }
-inline const qtgql::bases::SelectionsConfig & SELECTIONS_CONFIG() override{
-    static auto ret = qtgql::bases::SelectionsConfig(
-        {👉 context.operation.root_field.as_conf_string() 👈}
-    );
-    return ret;
-}
-
+signals:
+    void dataChanged();
 
 public:
+👉 context.operation.generated_variables_type 👈 vars_inst;
+
 👉 context.operation.name 👈(): qtgql::gqlwstransport::OperationHandlerABC(qtgql::gqlwstransport::GqlWsTrnsMsgWithID(qtgql::gqlwstransport::OperationPayload(
         {%- for line in context.operation.query.splitlines() %}"👉 line 👈"{% endfor -%}
         ))){
 m_message_template.op_id = m_operation_id;
 };
 
-QTGQL_STATIC_MAKE_SHARED(👉 context.operation.name 👈)
-
-inline qtgql::bases::OperationMetadata operation_metadata() override{
-return qtgql::bases::OperationMetadata(operation_id());
-};
 
+QTGQL_STATIC_MAKE_SHARED(👉 context.operation.name 👈)
 
 inline const QUuid & operation_id() const override{
 return m_operation_id;
 }
 
 
 void on_next(const QJsonObject &message) override{
-    if (!m_data && message.contains("data")){
+    if (!m_data){
         auto data = message.value("data").toObject();
-        auto metadata = operation_metadata();
-        if (data.contains("👉 context.operation.root_field.definition.name 👈")){
-{%- set do_after_deserialized -%} 👉 macros.initialize_proxy_field(context.operation.root_field) 👈 {% endset -%}
-            👉 macros.deserialize_field(context.operation.root_field.definition,
-                                    "auto concrete", False,
-                                    "SELECTIONS_CONFIG()",
-                                    "metadata",
-                                    do_after_deserialized,
-                                    ) 👈
-        }
+        m_data = new 👉 context.operation.root_type.name👈(this, 👉 context.operation.root_type.deserializer_name 👈(data, this));
+        emit dataChanged();
+    }
+    else{
+    throw qtgql::exceptions::NotImplementedError({"Updates on root types is not implemented yet."});
     }
 }
-inline const 👉 context.operation.root_field.property_type 👈 get_data(){
-    return m_data.value();
-}
-inline void loose() override{
-    {% if context.operation.root_field.type.is_object_type %}
-    👉 context.operation.root_field.type.is_object_type.name 👈::INST_STORE().get_node(m_data.value()->get_id()).value()->loose(operation_metadata());
-    {% else %}
-    throw "not implemented";
-    {% endif %}
+
+inline const 👉 context.operation.root_type.name 👈 * data() const{
+    if (m_data){
+        return m_data.value();
+    }
+    return nullptr;
 }
 
 {% if context.operation.variables %}
-void set_variables(
-{% for var in context.operation.variables -%}
-const std::optional<👉 var.type.type_name 👈> & 👉 var.name 👈 {% if not loop.last %},{% endif %}
-{% endfor -%}){
-{% for var in context.operation.variables %}
-if (👉 var.name 👈.has_value()){
-    m_variables.insert("👉 var.name 👈",  👉 var.json_repr() 👈);
-}
-{% endfor %}
+void set_variables(👉 context.operation.generated_variables_type 👈 vars){
+vars_inst = vars;
+m_variables = vars_inst.to_json();
 }
 {% endif %}
 
-signals:
-void dataChanged();
-
-};
 };
 };
```

### Comparing `qtgql-0.119.9/qtgqlcodegen/utils.py` & `qtgql-0.120.0/qtgqlcodegen/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import re
-from pathlib import Path
-from typing import Any
-from typing import Optional
-from typing import Type
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, Literal, TypeVar
 
 from attr import define
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 @define
 class FileSpec:
     path: Path
     content: str
 
     def dump(self) -> None:
@@ -29,14 +30,24 @@
     type_map: dict
 
     @classmethod
     def resolve(cls) -> Any:
         return cls.type_map[cls.name]
 
 
-def anti_forward_ref(name: str, type_map: dict) -> Type[AntiForwardRef]:
+def anti_forward_ref(name: str, type_map: dict) -> type[AntiForwardRef]:
     return type(name, (AntiForwardRef,), {"name": name, "type_map": type_map})
 
 
-def get_operation_name(query: str) -> Optional[str]:
-    if match := re.search(r"(subscription|mutation|query)(.*?({|\())", query):
-        return match.group(2).replace(" ", "").strip("{").strip("(")
+UNSET: Any = Literal["UNSET"]
+
+T = TypeVar("T")
+
+
+def require(v: T | None) -> T:  # pragma: no cover
+    if not v:
+        raise AttributeError(f"{v} returned no value")
+    return v
+
+
+def freeze(self, key, value):  # pragma: no cover
+    raise PermissionError("setattr called on frozen type")
```

### Comparing `qtgql-0.119.9/PKG-INFO` & `qtgql-0.120.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.119.9
+Version: 0.120.0
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: attrs (>=22.2.0,<23.0.0)
+Requires-Dist: attrs (>=22.2.0)
 Requires-Dist: frozendict (>=2.3.8,<3.0.0)
 Requires-Dist: graphql-core (>=3.2.3,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
-Requires-Dist: typingref (>=0.100.0,<0.101.0)
 Project-URL: Documentation, https://nrbnlulu.github.io/qtgql/
 Project-URL: Homepage, https://github.com/nrbnlulu/qtgql
 Description-Content-Type: text/markdown
 
 ###  Qt framework for building graphql driven QML applications
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qtgql?style=for-the-badge)](https://pypi.org/project/qtgql/)
 [![PyPI](https://img.shields.io/pypi/v/qtgql?style=for-the-badge)](https://pypi.org/project/qtgql/)
```

