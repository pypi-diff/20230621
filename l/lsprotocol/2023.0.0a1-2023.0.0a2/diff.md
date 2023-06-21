# Comparing `tmp/lsprotocol-2023.0.0a1.tar.gz` & `tmp/lsprotocol-2023.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsprotocol-2023.0.0a1.tar", last modified: Fri Mar  3 18:19:20 2023, max compression
+gzip compressed data, was "lsprotocol-2023.0.0a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lsprotocol-2023.0.0a1.tar` & `lsprotocol-2023.0.0a2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1162 2023-03-03 18:18:15.979245 lsprotocol-2023.0.0a1/LICENSE
--rw-r--r--   0        0        0     1152 2023-03-03 18:18:15.979245 lsprotocol-2023.0.0a1/README.md
--rw-r--r--   0        0        0       96 2023-03-03 18:18:15.979245 lsprotocol-2023.0.0a1/lsprotocol/__init__.py
--rw-r--r--   0        0        0    36745 2023-03-03 18:18:15.979245 lsprotocol-2023.0.0a1/lsprotocol/_hooks.py
--rw-r--r--   0        0        0      450 2023-03-03 18:18:15.979245 lsprotocol-2023.0.0a1/lsprotocol/converters.py
--rw-r--r--   0        0        0        0 2023-03-03 18:18:15.979245 lsprotocol-2023.0.0a1/lsprotocol/py.typed
--rw-r--r--   0        0        0   456171 2023-03-03 18:18:15.979245 lsprotocol-2023.0.0a1/lsprotocol/types.py
--rw-r--r--   0        0        0     1472 2023-03-03 18:18:15.979245 lsprotocol-2023.0.0a1/lsprotocol/validators.py
--rw-r--r--   0        0        0     1534 2023-03-03 18:18:15.979245 lsprotocol-2023.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     2109 1970-01-01 00:00:00.000000 lsprotocol-2023.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1162 2023-06-21 21:17:15.865019 lsprotocol-2023.0.0a2/LICENSE
+-rw-r--r--   0        0        0     1152 2023-06-21 21:17:15.865019 lsprotocol-2023.0.0a2/README.md
+-rw-r--r--   0        0        0       96 2023-06-21 21:17:15.865019 lsprotocol-2023.0.0a2/lsprotocol/__init__.py
+-rw-r--r--   0        0        0    37189 2023-06-21 21:17:15.865019 lsprotocol-2023.0.0a2/lsprotocol/_hooks.py
+-rw-r--r--   0        0        0      450 2023-06-21 21:17:15.865019 lsprotocol-2023.0.0a2/lsprotocol/converters.py
+-rw-r--r--   0        0        0        0 2023-06-21 21:17:15.865019 lsprotocol-2023.0.0a2/lsprotocol/py.typed
+-rw-r--r--   0        0        0   455298 2023-06-21 21:17:15.865019 lsprotocol-2023.0.0a2/lsprotocol/types.py
+-rw-r--r--   0        0        0     1467 2023-06-21 21:17:15.865019 lsprotocol-2023.0.0a2/lsprotocol/validators.py
+-rw-r--r--   0        0        0     1542 2023-06-21 21:17:15.865019 lsprotocol-2023.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2117 1970-01-01 00:00:00.000000 lsprotocol-2023.0.0a2/PKG-INFO
```

### Comparing `lsprotocol-2023.0.0a1/LICENSE` & `lsprotocol-2023.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `lsprotocol-2023.0.0a1/README.md` & `lsprotocol-2023.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `lsprotocol-2023.0.0a1/lsprotocol/_hooks.py` & `lsprotocol-2023.0.0a2/lsprotocol/_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 
 
 def _resolve_forward_references() -> None:
     """Resolve forward references for faster processing with cattrs."""
     global _resolved_forward_references
     if not _resolved_forward_references:
 
-        def _filter(p: Tuple[str, Union[type, object]]) -> bool:
+        def _filter(p: Tuple[str, object]) -> bool:
             return isinstance(p[1], type) and attrs.has(p[1])
 
         # Creating a concrete list here because `resolve_types` mutates the provided map.
         items = list(filter(_filter, lsp_types.ALL_TYPES_MAP.items()))
         for _, value in items:
             if isinstance(value, type):
-                attrs.resolve_types(value, lsp_types.ALL_TYPES_MAP, {})
+                attrs.resolve_types(value, lsp_types.ALL_TYPES_MAP, {})  # type: ignore
         _resolved_forward_references = True
 
 
 def register_hooks(converter: cattrs.Converter) -> cattrs.Converter:
     _resolve_forward_references()
     converter = _register_capabilities_hooks(converter)
     converter = _register_required_structure_hooks(converter)
@@ -379,14 +379,24 @@
         if isinstance(object_, (bool, int, str, float)):
             return object_
         if "id" in object_:
             return converter.structure(object_, lsp_types.InlayHintRegistrationOptions)
         else:
             return converter.structure(object_, lsp_types.InlayHintOptions)
 
+    def _inlay_hint_label_part_hook(
+        object_: Any, _: type
+    ) -> Union[str, List[lsp_types.InlayHintLabelPart]]:
+        if isinstance(object_, str):
+            return object_
+
+        return [
+            converter.structure(item, lsp_types.InlayHintLabelPart) for item in object_
+        ]
+
     def _diagnostic_provider_hook(
         object_: Any, _: type
     ) -> Union[
         OptionalPrimitive,
         lsp_types.DiagnosticRegistrationOptions,
         lsp_types.DiagnosticOptions,
     ]:
@@ -772,14 +782,18 @@
                     lsp_types.InlayHintOptions,
                     lsp_types.InlayHintRegistrationOptions,
                 ]
             ],
             _inlay_hint_provider_hook,
         ),
         (
+            Union[str, List[lsp_types.InlayHintLabelPart]],
+            _inlay_hint_label_part_hook,
+        ),
+        (
             Optional[
                 Union[
                     lsp_types.DiagnosticOptions, lsp_types.DiagnosticRegistrationOptions
                 ]
             ],
             _diagnostic_provider_hook,
         ),
```

### Comparing `lsprotocol-2023.0.0a1/lsprotocol/types.py` & `lsprotocol-2023.0.0a2/lsprotocol/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 from . import validators
 
 __lsp_version__ = "3.17.0"
 
 
 @enum.unique
 class SemanticTokenTypes(str, enum.Enum):
-    """A set of predefined token types. This set is not fixed an clients can
-    specify additional token types via the corresponding client capabilities.
+    """A set of predefined token types. This set is not fixed an clients can specify
+    additional token types via the corresponding client capabilities.
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
     Namespace = "namespace"
     Type = "type"
     """Represents a generic type.
 
-    Acts as a fallback for types which can't be mapped to a specific
-    type like class or enum.
+    Acts as a fallback for types which can't be mapped to a specific type like class or
+    enum.
     """
     Class = "class"
     Enum = "enum"
     Interface = "interface"
     Struct = "struct"
     TypeParameter = "typeParameter"
     Parameter = "parameter"
@@ -57,17 +57,16 @@
     Decorator = "decorator"
     """@since 3.17.0"""
     # Since: 3.17.0
 
 
 @enum.unique
 class SemanticTokenModifiers(str, enum.Enum):
-    """A set of predefined token modifiers. This set is not fixed an clients
-    can specify additional token types via the corresponding client
-    capabilities.
+    """A set of predefined token modifiers. This set is not fixed an clients can specify
+    additional token types via the corresponding client capabilities.
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
     Declaration = "declaration"
     Definition = "definition"
@@ -100,47 +99,46 @@
 
     ParseError = -32700
     InvalidRequest = -32600
     MethodNotFound = -32601
     InvalidParams = -32602
     InternalError = -32603
     ServerNotInitialized = -32002
-    """Error code indicating that a server received a notification or request
-    before the server has received the `initialize` request."""
+    """Error code indicating that a server received a notification or request before the
+    server has received the `initialize` request."""
     UnknownErrorCode = -32001
 
 
 class LSPErrorCodes(int, enum.Enum):
     RequestFailed = -32803
-    """A request failed but it was syntactically correct, e.g the method name
-    was known and the parameters were valid. The error message should contain
-    human readable information about why the request failed.
+    """A request failed but it was syntactically correct, e.g the method name was known
+    and the parameters were valid. The error message should contain human readable
+    information about why the request failed.
 
     @since 3.17.0
     """
     # Since: 3.17.0
     ServerCancelled = -32802
-    """The server cancelled the request. This error code should only be used
-    for requests that explicitly support being server cancellable.
+    """The server cancelled the request. This error code should only be used for
+    requests that explicitly support being server cancellable.
 
     @since 3.17.0
     """
     # Since: 3.17.0
     ContentModified = -32801
-    """The server detected that the content of a document got modified outside
-    normal conditions. A server should NOT send this error code if it detects a
-    content change in it unprocessed messages. The result even computed on an
-    older state might still be useful for the client.
+    """The server detected that the content of a document got modified outside normal
+    conditions. A server should NOT send this error code if it detects a content change
+    in it unprocessed messages. The result even computed on an older state might still
+    be useful for the client.
 
-    If a client decides that a result is not of any use anymore the
-    client should cancel the request.
+    If a client decides that a result is not of any use anymore the client should cancel
+    the request.
     """
     RequestCancelled = -32800
-    """The client has canceled a request and a server as detected the
-    cancel."""
+    """The client has canceled a request and a server as detected the cancel."""
 
 
 @enum.unique
 class FoldingRangeKind(str, enum.Enum):
     """A set of predefined range kinds."""
 
     Comment = "comment"
@@ -224,16 +222,16 @@
 
     # Since: 3.16.0
     Import = "import"
     """The moniker represent a symbol that is imported into a project."""
     Export = "export"
     """The moniker represents a symbol that is exported from a project."""
     Local = "local"
-    """The moniker represents a symbol that is local to a project (e.g. a local
-    variable of a function, a class not visible outside the project, ...)"""
+    """The moniker represents a symbol that is local to a project (e.g. a local variable
+    of a function, a class not visible outside the project, ...)"""
 
 
 @enum.unique
 class InlayHintKind(int, enum.Enum):
     """Inlay hint kinds.
 
     @since 3.17.0
@@ -258,36 +256,35 @@
     """An information message."""
     Log = 4
     """A log message."""
 
 
 @enum.unique
 class TextDocumentSyncKind(int, enum.Enum):
-    """Defines how the host (editor) should sync document changes to the
-    language server."""
+    """Defines how the host (editor) should sync document changes to the language
+    server."""
 
     None_ = 0
     """Documents should not be synced at all."""
     Full = 1
-    """Documents are synced by always sending the full content of the
-    document."""
+    """Documents are synced by always sending the full content of the document."""
     Incremental = 2
     """Documents are synced by sending the full content on open.
 
     After that only incremental updates to the document are send.
     """
 
 
 @enum.unique
 class TextDocumentSaveReason(int, enum.Enum):
     """Represents reasons why a text document is saved."""
 
     Manual = 1
-    """Manually triggered, e.g. by the user pressing save, by starting
-    debugging, or by an API call."""
+    """Manually triggered, e.g. by the user pressing save, by starting debugging, or by
+    an API call."""
     AfterDelay = 2
     """Automatic after a delay."""
     FocusOut = 3
     """When the editor lost focus."""
 
 
 @enum.unique
@@ -332,51 +329,50 @@
     # Since: 3.15.0
     Deprecated = 1
     """Render a completion as obsolete, usually using a strike-out."""
 
 
 @enum.unique
 class InsertTextFormat(int, enum.Enum):
-    """Defines whether the insert text in a completion item should be
-    interpreted as plain text or a snippet."""
+    """Defines whether the insert text in a completion item should be interpreted as
+    plain text or a snippet."""
 
     PlainText = 1
     """The primary text to be inserted is treated as a plain string."""
     Snippet = 2
     """The primary text to be inserted is treated as a snippet.
 
-    A snippet can define tab stops and placeholders with `$1`, `$2`
-    and `${3:foo}`. `$0` defines the final tab stop, it defaults to
-    the end of the snippet. Placeholders with equal identifiers are linked,
-    that is typing in one will update others too.
+    A snippet can define tab stops and placeholders with `$1`, `$2` and
+    `${3:foo}`. `$0` defines the final tab stop, it defaults to the end
+    of the snippet. Placeholders with equal identifiers are linked, that
+    is typing in one will update others too.
 
-    See also: https://microsoft.github.io/language-server-protocol/specifications/specification-current/#snippet_syntax
+    See also:
+    https://microsoft.github.io/language-server-protocol/specifications/specification-current/#snippet_syntax
     """
 
 
 @enum.unique
 class InsertTextMode(int, enum.Enum):
-    """How whitespace and indentation is handled during completion item
-    insertion.
+    """How whitespace and indentation is handled during completion item insertion.
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
     AsIs = 1
     """The insertion or replace strings is taken as it is.
 
-    If the value is multi line the lines below the cursor will be
-    inserted using the indentation defined in the string value. The
-    client will not apply any kind of adjustments to the string.
+    If the value is multi line the lines below the cursor will be inserted using the
+    indentation defined in the string value. The client will not apply any kind of
+    adjustments to the string.
     """
     AdjustIndentation = 2
-    """The editor adjusts leading whitespace of new lines so that they match
-    the indentation up to the cursor of the line for which the item is
-    accepted.
+    """The editor adjusts leading whitespace of new lines so that they match the
+    indentation up to the cursor of the line for which the item is accepted.
 
     Consider a line like this: <2tabs><cursor><3tabs>foo. Accepting a
     multi line completion item is indented using 2 tabs and all
     following lines inserted will be indented using 2 tabs as well.
     """
 
 
@@ -462,19 +458,19 @@
     """Trace messages only."""
     Verbose = "verbose"
     """Verbose message tracing."""
 
 
 @enum.unique
 class MarkupKind(str, enum.Enum):
-    """Describes the content type that a client supports in various result
-    literals like `Hover`, `ParameterInfo` or `CompletionItem`.
+    """Describes the content type that a client supports in various result literals like
+    `Hover`, `ParameterInfo` or `CompletionItem`.
 
-    Please note that `MarkupKinds` must not start with a `$`. This kinds
-    are reserved for internal usage.
+    Please note that `MarkupKinds` must not start with a `$`. This kinds are reserved
+    for internal usage.
     """
 
     PlainText = "plaintext"
     """Plain text is supported as a content format."""
     Markdown = "markdown"
     """Markdown is supported as a content format."""
 
@@ -484,24 +480,24 @@
     """A set of predefined position encoding kinds.
 
     @since 3.17.0
     """
 
     # Since: 3.17.0
     Utf8 = "utf-8"
-    """Character offsets count UTF-8 code units."""
+    """Character offsets count UTF-8 code units (e.g. bytes)."""
     Utf16 = "utf-16"
     """Character offsets count UTF-16 code units.
 
     This is the default and must always be supported by servers
     """
     Utf32 = "utf-32"
     """Character offsets count UTF-32 code units.
 
-    Implementation note: these are the same as Unicode code points, so
+    Implementation note: these are the same as Unicode codepoints, so
     this `PositionEncodingKind` may also be used for an encoding-
     agnostic representation of character offsets.
     """
 
 
 @enum.unique
 class FileChangeType(int, enum.Enum):
@@ -546,32 +542,31 @@
     @since 3.15.0
     """
 
     # Since: 3.15.0
     Unnecessary = 1
     """Unused or unnecessary code.
 
-    Clients are allowed to render diagnostics with this tag faded out
-    instead of having an error squiggle.
+    Clients are allowed to render diagnostics with this tag faded out instead of having
+    an error squiggle.
     """
     Deprecated = 2
     """Deprecated or obsolete code.
 
-    Clients are allowed to rendered diagnostics with this tag strike
-    through.
+    Clients are allowed to rendered diagnostics with this tag strike through.
     """
 
 
 @enum.unique
 class CompletionTriggerKind(int, enum.Enum):
     """How a completion was triggered."""
 
     Invoked = 1
-    """Completion was triggered by typing an identifier (24x7 code complete),
-    manual invocation (e.g Ctrl+Space) or via API."""
+    """Completion was triggered by typing an identifier (24x7 code complete), manual
+    invocation (e.g Ctrl+Space) or via API."""
     TriggerCharacter = 2
     """Completion was triggered by a trigger character specified by the
     `triggerCharacters` properties of the `CompletionRegistrationOptions`."""
     TriggerForIncompleteCompletions = 3
     """Completion was re-triggered as current completion list is incomplete."""
 
 
@@ -584,41 +579,39 @@
 
     # Since: 3.15.0
     Invoked = 1
     """Signature help was invoked manually by the user or by a command."""
     TriggerCharacter = 2
     """Signature help was triggered by a trigger character."""
     ContentChange = 3
-    """Signature help was triggered by the cursor moving or by the document
-    content changing."""
+    """Signature help was triggered by the cursor moving or by the document content
+    changing."""
 
 
 @enum.unique
 class CodeActionTriggerKind(int, enum.Enum):
     """The reason why code actions were requested.
 
     @since 3.17.0
     """
 
     # Since: 3.17.0
     Invoked = 1
-    """Code actions were explicitly requested by the user or by an
-    extension."""
+    """Code actions were explicitly requested by the user or by an extension."""
     Automatic = 2
     """Code actions were requested automatically.
 
-    This typically happens when current selection in a file changes, but
-    can also be triggered when file content changes.
+    This typically happens when current selection in a file changes, but can also be
+    triggered when file content changes.
     """
 
 
 @enum.unique
 class FileOperationPatternKind(str, enum.Enum):
-    """A pattern kind describing if a glob pattern matches a file a folder or
-    both.
+    """A pattern kind describing if a glob pattern matches a file a folder or both.
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
     File = "file"
     """The pattern matches a file only."""
@@ -649,44 +642,44 @@
     Delete = "delete"
     """Supports deleting existing files and folders."""
 
 
 @enum.unique
 class FailureHandlingKind(str, enum.Enum):
     Abort = "abort"
-    """Applying the workspace change is simply aborted if one of the changes
-    provided fails.
+    """Applying the workspace change is simply aborted if one of the changes provided
+    fails.
 
     All operations executed before the failing operation stay executed.
     """
     Transactional = "transactional"
     """All operations are executed transactional.
 
-    That means they either all succeed or no changes at all are applied
-    to the workspace.
+    That means they either all succeed or no changes at all are applied to the
+    workspace.
     """
     TextOnlyTransactional = "textOnlyTransactional"
-    """If the workspace edit contains only textual file changes they are
-    executed transactional.
+    """If the workspace edit contains only textual file changes they are executed
+    transactional.
 
-    If resource changes (create, rename or delete file) are part of the
-    change the failure handling strategy is abort.
+    If resource changes (create, rename or delete file) are part of the change the
+    failure handling strategy is abort.
     """
     Undo = "undo"
     """The client tries to undo the operations already executed.
 
     But there is no guarantee that this is succeeding.
     """
 
 
 @enum.unique
 class PrepareSupportDefaultBehavior(int, enum.Enum):
     Identifier = 1
-    """The client's default behavior is to select the identifier according the
-    to language's syntax rule."""
+    """The client's default behavior is to select the identifier according the to
+    language's syntax rule."""
 
 
 @enum.unique
 class TokenFormat(str, enum.Enum):
     Relative = "relative"
 
 
@@ -695,63 +688,61 @@
 
 @since 3.17.0
 """
 # Since: 3.17.0
 
 
 Definition = Union["Location", List["Location"]]
-"""The definition of a symbol represented as one or many {@link Location
-locations}. For most programming languages there is only one location at which
-a symbol is defined.
+"""The definition of a symbol represented as one or many {@link Location locations}. For
+most programming languages there is only one location at which a symbol is defined.
 
-Servers should prefer returning `DefinitionLink` over `Definition` if
-supported by the client.
+Servers should prefer returning `DefinitionLink` over `Definition` if supported by the
+client.
 """
 
 
 DefinitionLink = Union["LocationLink", "LocationLink"]
 """Information about where a symbol is defined.
 
-Provides additional metadata over normal {@link Location location}
-definitions, including the range of the defining symbol
+Provides additional metadata over normal {@link Location location} definitions,
+including the range of the defining symbol
 """
 
 
 LSPArray = List["LSPAny"]
 """LSP arrays.
 
 @since 3.17.0
 """
 # Since: 3.17.0
 
 
 LSPAny = Union[Any, None]
-"""The LSP any type. Please note that strictly speaking a property with the
-value `undefined` can't be converted into JSON preserving the property name.
-However for convenience it is allowed and assumed that all these properties are
-optional as well.
+"""The LSP any type. Please note that strictly speaking a property with the value
+`undefined` can't be converted into JSON preserving the property name. However for
+convenience it is allowed and assumed that all these properties are optional as well.
 
 @since 3.17.0
 """
 # Since: 3.17.0
 
 
 Declaration = Union["Location", List["Location"]]
 """The declaration of a symbol representation as one or many {@link Location
 locations}."""
 
 
 DeclarationLink = Union["LocationLink", "LocationLink"]
 """Information about where a symbol is declared.
 
-Provides additional metadata over normal {@link Location location} declarations, including the range of
-the declaring symbol.
+Provides additional metadata over normal {@link Location location} declarations,
+including the range of the declaring symbol.
 
-Servers should prefer returning `DeclarationLink` over `Declaration` if supported
-by the client.
+Servers should prefer returning `DeclarationLink` over `Declaration` if supported by the
+client.
 """
 
 
 InlineValue = Union[
     "InlineValueText", "InlineValueVariableLookup", "InlineValueEvaluatableExpression"
 ]
 """Inline value information can be provided by different means:
@@ -765,18 +756,18 @@
 """
 # Since: 3.17.0
 
 
 DocumentDiagnosticReport = Union[
     "RelatedFullDocumentDiagnosticReport", "RelatedUnchangedDocumentDiagnosticReport"
 ]
-"""The result of a document diagnostic pull request. A report can either be a
-full report containing all diagnostics for the requested document or an
-unchanged report indicating that nothing has changed in terms of diagnostics in
-comparison to the last pull request.
+"""The result of a document diagnostic pull request. A report can either be a full
+report containing all diagnostics for the requested document or an unchanged report
+indicating that nothing has changed in terms of diagnostics in comparison to the last
+pull request.
 
 @since 3.17.0
 """
 # Since: 3.17.0
 
 
 @attrs.define
@@ -795,27 +786,27 @@
     "Range", "PrepareRenameResult_Type1", "PrepareRenameResult_Type2"
 ]
 
 
 DocumentSelector = List["DocumentFilter"]
 """A document selector is the combination of one or many document filters.
 
-@sample `let sel:DocumentSelector = [{ language: 'typescript' }, { language: 'json', pattern: '**/tsconfig.json' }]`;
+@sample `let sel:DocumentSelector = [{ language: 'typescript' }, { language: 'json',
+pattern: '**/tsconfig.json' }]`;
 
 The use of a string as a document filter is deprecated @since 3.16.0.
 """
 # Since: 3.16.0.
 
 
 ProgressToken = Union[int, str]
 
 
 ChangeAnnotationIdentifier = str
-"""An identifier to refer to a change annotation stored with a workspace
-edit."""
+"""An identifier to refer to a change annotation stored with a workspace edit."""
 
 
 WorkspaceDocumentDiagnosticReport = Union[
     "WorkspaceFullDocumentDiagnosticReport",
     "WorkspaceUnchangedDocumentDiagnosticReport",
 ]
 """A workspace diagnostic document report.
@@ -849,47 +840,44 @@
 
 
 TextDocumentContentChangeEvent = Union[
     "TextDocumentContentChangeEvent_Type1", "TextDocumentContentChangeEvent_Type2"
 ]
 """An event describing a change to a text document.
 
-If only a text is provided it is considered to be the full content of
-the document.
+If only a text is provided it is considered to be the full content of the document.
 """
 
 
 @attrs.define
 class MarkedString_Type1:
     language: str = attrs.field(validator=attrs.validators.instance_of(str))
 
     value: str = attrs.field(validator=attrs.validators.instance_of(str))
 
 
 MarkedString = Union[str, "MarkedString_Type1"]
-"""MarkedString can be used to render human readable text. It is either a
-markdown string or a code-block that provides a language and a code snippet.
-The language identifier is semantically equal to the optional language
-identifier in fenced code blocks in GitHub issues. See
-https://help.github.com/articles/creating-and-highlighting-code-blocks/#syntax-
-highlighting.
+"""MarkedString can be used to render human readable text. It is either a markdown
+string or a code-block that provides a language and a code snippet. The language
+identifier is semantically equal to the optional language identifier in fenced code
+blocks in GitHub issues. See https://help.github.com/articles/creating-and-highlighting-
+code-blocks/#syntax- highlighting.
 
 The pair of a language and a value is an equivalent to markdown:
 ```${language}
 ${value}
 ```
 
 Note that markdown strings will be sanitized - that means html will be escaped.
 @deprecated use MarkupContent instead.
 """
 
 
 DocumentFilter = Union["TextDocumentFilter", "NotebookCellTextDocumentFilter"]
-"""A document filter describes a top level text document or a notebook cell
-document.
+"""A document filter describes a top level text document or a notebook cell document.
 
 @since 3.17.0 - proposed support for NotebookCellTextDocumentFilter.
 """
 # Since: 3.17.0 - proposed support for NotebookCellTextDocumentFilter.
 
 
 GlobPattern = Union["Pattern", "RelativePattern"]
@@ -954,17 +942,16 @@
     """A Uri {@link Uri.scheme scheme}, like `file` or `untitled`."""
 
 
 TextDocumentFilter = Union[
     "TextDocumentFilter_Type1", "TextDocumentFilter_Type2", "TextDocumentFilter_Type3"
 ]
 """A document filter denotes a document by different properties like the {@link
-TextDocument.languageId language}, the {@link Uri.scheme scheme} of its
-resource, or a glob-pattern that is applied to the {@link TextDocument.fileName
-path}.
+TextDocument.languageId language}, the {@link Uri.scheme scheme} of its resource, or a
+glob-pattern that is applied to the {@link TextDocument.fileName path}.
 
 Glob patterns can have the following syntax:
 - `*` to match one or more characters in a path segment
 - `?` to match on one character in a path segment
 - `**` to match any number of path segments, including none
 - `{}` to group sub patterns into an OR expression. (e.g. `**/*.{ts,js}` matches all TypeScript and JavaScript files)
 - `[]` to declare a range of characters to match in a path segment (e.g., `example.[0-9]` to match on `example.0`, `example.1`, …)
@@ -1033,17 +1020,16 @@
 
 
 NotebookDocumentFilter = Union[
     "NotebookDocumentFilter_Type1",
     "NotebookDocumentFilter_Type2",
     "NotebookDocumentFilter_Type3",
 ]
-"""A notebook document filter denotes a notebook document by different
-properties. The properties will be match against the notebook's URI (same as
-with documents)
+"""A notebook document filter denotes a notebook document by different properties. The
+properties will be match against the notebook's URI (same as with documents)
 
 @since 3.17.0
 """
 # Since: 3.17.0
 
 
 Pattern = str
@@ -1060,16 +1046,16 @@
 @since 3.17.0
 """
 # Since: 3.17.0
 
 
 @attrs.define
 class TextDocumentPositionParams:
-    """A parameter literal used in requests to pass a text document and a
-    position inside that document."""
+    """A parameter literal used in requests to pass a text document and a position
+    inside that document."""
 
     text_document: "TextDocumentIdentifier" = attrs.field()
     """The text document."""
 
     position: "Position" = attrs.field()
     """The position inside the text document."""
 
@@ -1101,16 +1087,15 @@
     partial_result_token: Optional[ProgressToken] = attrs.field(default=None)
     """An optional token that a server can use to report partial results (e.g.
     streaming) to the client."""
 
 
 @attrs.define
 class Location:
-    """Represents a location inside a resource, such as a line inside a text
-    file."""
+    """Represents a location inside a resource, such as a line inside a text file."""
 
     uri: str = attrs.field(validator=attrs.validators.instance_of(str))
 
     range: "Range" = attrs.field()
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, Location):
@@ -1126,16 +1111,15 @@
     """General text document registration options."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
 
 @attrs.define
 class WorkDoneProgressOptions:
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -1157,43 +1141,40 @@
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class ImplementationRegistrationOptions:
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class TypeDefinitionParams:
     text_document: "TextDocumentIdentifier" = attrs.field()
     """The text document."""
@@ -1220,31 +1201,29 @@
 @attrs.define
 class TypeDefinitionRegistrationOptions:
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class WorkspaceFolder:
     """A workspace folder inside a client."""
 
@@ -1256,16 +1235,15 @@
 
     Used to refer to this workspace folder in the user interface.
     """
 
 
 @attrs.define
 class DidChangeWorkspaceFoldersParams:
-    """The parameters of a `workspace/didChangeWorkspaceFolders`
-    notification."""
+    """The parameters of a `workspace/didChangeWorkspaceFolders` notification."""
 
     event: "WorkspaceFoldersChangeEvent" = attrs.field()
     """The actual workspace folder change event."""
 
 
 @attrs.define
 class ConfigurationParams:
@@ -1311,31 +1289,29 @@
 @attrs.define
 class DocumentColorRegistrationOptions:
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class ColorPresentationParams:
     """Parameters for a {@link ColorPresentationRequest}."""
 
@@ -1360,31 +1336,31 @@
 
 
 @attrs.define
 class ColorPresentation:
     label: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The label of this color presentation.
 
-    It will be shown on the color picker header. By default this is also
-    the text that is inserted when selecting this color presentation.
+    It will be shown on the color picker header. By default this is also the text that
+    is inserted when selecting this color presentation.
     """
 
     text_edit: Optional["TextEdit"] = attrs.field(default=None)
-    """An {@link TextEdit edit} which is applied to a document when selecting
-    this presentation for the color.
+    """An {@link TextEdit edit} which is applied to a document when selecting this
+    presentation for the color.
 
     When `falsy` the {@link ColorPresentation.label label} is used.
     """
 
     additional_text_edits: Optional[List["TextEdit"]] = attrs.field(default=None)
-    """An optional array of additional {@link TextEdit text edits} that are
-    applied when selecting this color presentation.
+    """An optional array of additional {@link TextEdit text edits} that are applied when
+    selecting this color presentation.
 
-    Edits must not overlap with the main {@link
-    ColorPresentation.textEdit edit} nor with themselves.
+    Edits must not overlap with the main {@link ColorPresentation.textEdit edit} nor
+    with themselves.
     """
 
 
 @attrs.define
 class FoldingRangeParams:
     """Parameters for a {@link FoldingRangeRequest}."""
 
@@ -1399,33 +1375,30 @@
     streaming) to the client."""
 
 
 @attrs.define
 class FoldingRange:
     """Represents a folding range.
 
-    To be valid, start and end line must be bigger than zero and smaller
-    than the number of lines in the document. Clients are free to ignore
-    invalid ranges.
+    To be valid, start and end line must be bigger than zero and smaller than the number
+    of lines in the document. Clients are free to ignore invalid ranges.
     """
 
     start_line: int = attrs.field(validator=validators.uinteger_validator)
     """The zero-based start line of the range to fold.
 
-    The folded area starts after the line's last character. To be valid,
-    the end must be zero or larger and smaller than the number of lines
-    in the document.
+    The folded area starts after the line's last character. To be valid, the end must be
+    zero or larger and smaller than the number of lines in the document.
     """
 
     end_line: int = attrs.field(validator=validators.uinteger_validator)
     """The zero-based end line of the range to fold.
 
-    The folded area ends with the line's last character. To be valid,
-    the end must be zero or larger and smaller than the number of lines
-    in the document.
+    The folded area ends with the line's last character. To be valid, the end must be
+    zero or larger and smaller than the number of lines in the document.
     """
 
     start_character: Optional[int] = attrs.field(
         validator=attrs.validators.optional(validators.uinteger_validator), default=None
     )
     """The zero-based character offset from where the folded range starts.
 
@@ -1439,26 +1412,24 @@
 
     If not defined, defaults to the length of the end line.
     """
 
     kind: Optional[Union[FoldingRangeKind, str]] = attrs.field(default=None)
     """Describes the kind of the folding range such as `comment' or 'region'.
 
-    The kind is used to categorize folding ranges and used by commands
-    like 'Fold all comments'. See {@link FoldingRangeKind} for an
-    enumeration of standardized kinds.
+    The kind is used to categorize folding ranges and used by commands like 'Fold all
+    comments'. See {@link FoldingRangeKind} for an enumeration of standardized kinds.
     """
 
     collapsed_text: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """The text that the client should show when the specified range is
-    collapsed. If not defined or not supported by the client, a default will be
-    chosen by the client.
+    """The text that the client should show when the specified range is collapsed. If
+    not defined or not supported by the client, a default will be chosen by the client.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
 
 @attrs.define
@@ -1472,31 +1443,29 @@
 @attrs.define
 class FoldingRangeRegistrationOptions:
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class DeclarationParams:
     text_document: "TextDocumentIdentifier" = attrs.field()
     """The text document."""
@@ -1528,26 +1497,24 @@
     )
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class SelectionRangeParams:
     """A parameter literal used in selection range requests."""
 
@@ -1565,16 +1532,15 @@
     streaming) to the client."""
 
 
 @attrs.define
 class SelectionRange:
     """A selection range represents a part of a selection hierarchy.
 
-    A selection range may have a parent selection range that contains
-    it.
+    A selection range may have a parent selection range that contains it.
     """
 
     range: "Range" = attrs.field()
     """The {@link Range range} of this selection range."""
 
     parent: Optional["SelectionRange"] = attrs.field(default=None)
     """The parent selection range containing this range.
@@ -1599,26 +1565,24 @@
     )
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class WorkDoneProgressCreateParams:
     token: ProgressToken = attrs.field()
     """The token to be used to report progress."""
@@ -1647,16 +1611,16 @@
 
     work_done_token: Optional[ProgressToken] = attrs.field(default=None)
     """An optional token that a server can use to report work done progress."""
 
 
 @attrs.define
 class CallHierarchyItem:
-    """Represents programming constructs like functions or constructors in the
-    context of call hierarchy.
+    """Represents programming constructs like functions or constructors in the context
+    of call hierarchy.
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
 
     name: str = attrs.field(validator=attrs.validators.instance_of(str))
@@ -1665,36 +1629,36 @@
     kind: SymbolKind = attrs.field()
     """The kind of this item."""
 
     uri: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The resource identifier of this item."""
 
     range: "Range" = attrs.field()
-    """The range enclosing this symbol not including leading/trailing
-    whitespace but everything else, e.g. comments and code."""
+    """The range enclosing this symbol not including leading/trailing whitespace but
+    everything else, e.g. comments and code."""
 
     selection_range: "Range" = attrs.field()
-    """The range that should be selected and revealed when this symbol is being
-    picked, e.g. the name of a function.
+    """The range that should be selected and revealed when this symbol is being picked,
+    e.g. the name of a function.
 
     Must be contained by the {@link CallHierarchyItem.range `range`}.
     """
 
     tags: Optional[List[SymbolTag]] = attrs.field(default=None)
     """Tags for this item."""
 
     detail: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """More detail for this item, e.g. the signature of a function."""
 
     data: Optional[LSPAny] = attrs.field(default=None)
-    """A data entry field that is preserved between a call hierarchy prepare
-    and incoming calls or outgoing calls requests."""
+    """A data entry field that is preserved between a call hierarchy prepare and
+    incoming calls or outgoing calls requests."""
 
 
 @attrs.define
 class CallHierarchyOptions:
     """Call hierarchy options used during static registration.
 
     @since 3.16.0
@@ -1718,31 +1682,29 @@
     # Since: 3.16.0
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class CallHierarchyIncomingCallsParams:
     """The parameter of a `callHierarchy/incomingCalls` request.
 
@@ -1772,16 +1734,16 @@
 
     from_: CallHierarchyItem = attrs.field()
     """The item that makes the call."""
 
     from_ranges: List["Range"] = attrs.field()
     """The ranges at which the calls appear.
 
-    This is relative to the caller denoted by {@link
-    CallHierarchyIncomingCall.from `this.from`}.
+    This is relative to the caller denoted by {@link CallHierarchyIncomingCall.from
+    `this.from`}.
     """
 
 
 @attrs.define
 class CallHierarchyOutgoingCallsParams:
     """The parameter of a `callHierarchy/outgoingCalls` request.
 
@@ -1798,16 +1760,16 @@
     partial_result_token: Optional[ProgressToken] = attrs.field(default=None)
     """An optional token that a server can use to report partial results (e.g.
     streaming) to the client."""
 
 
 @attrs.define
 class CallHierarchyOutgoingCall:
-    """Represents an outgoing call, e.g. calling a getter from a method or a
-    method from a constructor etc.
+    """Represents an outgoing call, e.g. calling a getter from a method or a method from
+    a constructor etc.
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
 
     to: CallHierarchyItem = attrs.field()
@@ -1850,18 +1812,17 @@
 
     result_id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """An optional result id.
 
-    If provided and clients support delta updating the client will
-    include the result id in the next semantic token request. A server
-    can then instead of computing all semantic tokens again simply send
-    a delta.
+    If provided and clients support delta updating the client will include the result id
+    in the next semantic token request. A server can then instead of computing all
+    semantic tokens again simply send a delta.
     """
 
 
 @attrs.define
 class SemanticTokensPartialResult:
     """@since 3.16.0"""
 
@@ -1885,16 +1846,15 @@
 
     # Since: 3.16.0
 
     legend: "SemanticTokensLegend" = attrs.field()
     """The legend used by the server."""
 
     range: Optional[Union[bool, Any]] = attrs.field(default=None)
-    """Server supports providing semantic tokens for a specific range of a
-    document."""
+    """Server supports providing semantic tokens for a specific range of a document."""
 
     full: Optional[Union[bool, "SemanticTokensOptionsFullType1"]] = attrs.field(
         default=None
     )
     """Server supports providing semantic tokens for a full document."""
 
     work_done_progress: Optional[bool] = attrs.field(
@@ -1922,21 +1882,19 @@
     """The legend used by the server."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     range: Optional[Union[bool, Any]] = attrs.field(default=None)
-    """Server supports providing semantic tokens for a specific range of a
-    document."""
+    """Server supports providing semantic tokens for a specific range of a document."""
 
     full: Optional[
         Union[bool, "SemanticTokensRegistrationOptionsFullType1"]
     ] = attrs.field(default=None)
     """Server supports providing semantic tokens for a full document."""
 
     work_done_progress: Optional[bool] = attrs.field(
@@ -1946,16 +1904,15 @@
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class SemanticTokensDeltaParams:
     """@since 3.16.0"""
 
@@ -1963,16 +1920,16 @@
 
     text_document: "TextDocumentIdentifier" = attrs.field()
     """The text document."""
 
     previous_result_id: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The result id of a previous response.
 
-    The result Id can either point to a full response or a delta
-    response depending on what was received last.
+    The result Id can either point to a full response or a delta response depending on
+    what was received last.
     """
 
     work_done_token: Optional[ProgressToken] = attrs.field(default=None)
     """An optional token that a server can use to report work done progress."""
 
     partial_result_token: Optional[ProgressToken] = attrs.field(default=None)
     """An optional token that a server can use to report partial results (e.g.
@@ -1982,16 +1939,15 @@
 @attrs.define
 class SemanticTokensDelta:
     """@since 3.16.0"""
 
     # Since: 3.16.0
 
     edits: List["SemanticTokensEdit"] = attrs.field()
-    """The semantic token edits to transform a previous result into a new
-    result."""
+    """The semantic token edits to transform a previous result into a new result."""
 
     result_id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
 
 
@@ -2022,50 +1978,49 @@
     partial_result_token: Optional[ProgressToken] = attrs.field(default=None)
     """An optional token that a server can use to report partial results (e.g.
     streaming) to the client."""
 
 
 @attrs.define
 class ShowDocumentParams:
-    """Params to show a document.
+    """Params to show a resource in the UI.
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
 
     uri: str = attrs.field(validator=attrs.validators.instance_of(str))
-    """The document uri to show."""
+    """The uri to show."""
 
     external: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Indicates to show the resource in an external program.
 
-    To show for example `https://code.visualstudio.com/` in the default
-    WEB browser set `external` to `true`.
+    To show, for example, `https://code.visualstudio.com/`
+    in the default WEB browser set `external` to `true`.
     """
 
     take_focus: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """An optional property to indicate whether the editor showing the document
-    should take focus or not.
+    """An optional property to indicate whether the editor showing the document should
+    take focus or not.
 
-    Clients might ignore this property if an external program is
-    started.
+    Clients might ignore this property if an external program is started.
     """
 
     selection: Optional["Range"] = attrs.field(default=None)
     """An optional selection range if the document is a text document.
 
-    Clients might ignore the property if an external program is started
-    or the file is not a text file.
+    Clients might ignore the property if an external program is started or the file is
+    not a text file.
     """
 
 
 @attrs.define
 class ShowDocumentResult:
     """The result of a showDocument request.
 
@@ -2098,27 +2053,26 @@
     """
 
     # Since: 3.16.0
 
     ranges: List["Range"] = attrs.field()
     """A list of ranges that can be edited together.
 
-    The ranges must have identical length and contain identical text
-    content. The ranges cannot overlap.
+    The ranges must have identical length and contain identical text content. The ranges
+    cannot overlap.
     """
 
     word_pattern: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """An optional word pattern (regular expression) that describes valid
-    contents for the given ranges.
+    """An optional word pattern (regular expression) that describes valid contents for
+    the given ranges.
 
-    If no pattern is provided, the client configuration's word pattern
-    will be used.
+    If no pattern is provided, the client configuration's word pattern will be used.
     """
 
 
 @attrs.define
 class LinkedEditingRangeOptions:
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -2129,90 +2083,91 @@
 @attrs.define
 class LinkedEditingRangeRegistrationOptions:
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class CreateFilesParams:
-    """The parameters sent in notifications/requests for user-initiated
-    creation of files.
+    """The parameters sent in notifications/requests for user-initiated creation of
+    files.
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
 
     files: List["FileCreate"] = attrs.field()
     """An array of all files/folders created in this operation."""
 
 
 @attrs.define
 class WorkspaceEdit:
-    """A workspace edit represents changes to many resources managed in the
-    workspace. The edit should either provide `changes` or `documentChanges`.
-    If documentChanges are present they are preferred over `changes` if the
-    client can handle versioned document edits.
-
-    Since version 3.13.0 a workspace edit can contain resource operations as well. If resource
-    operations are present clients need to execute the operations in the order in which they
-    are provided. So a workspace edit for example can consist of the following two changes:
-    (1) a create file a.txt and (2) a text document edit which insert text into file a.txt.
-
-    An invalid sequence (e.g. (1) delete file a.txt and (2) insert text into file a.txt) will
-    cause failure of the operation. How the client recovers from the failure is described by
-    the client capability: `workspace.workspaceEdit.failureHandling`
+    """A workspace edit represents changes to many resources managed in the workspace.
+    The edit should either provide `changes` or `documentChanges`. If documentChanges
+    are present they are preferred over `changes` if the client can handle versioned
+    document edits.
+
+    Since version 3.13.0 a workspace edit can contain resource
+    operations as well. If resource operations are present clients need
+    to execute the operations in the order in which they are provided.
+    So a workspace edit for example can consist of the following two
+    changes: (1) a create file a.txt and (2) a text document edit which
+    insert text into file a.txt.
+
+    An invalid sequence (e.g. (1) delete file a.txt and (2) insert text
+    into file a.txt) will cause failure of the operation. How the client
+    recovers from the failure is described by the client capability:
+    `workspace.workspaceEdit.failureHandling`
     """
 
     changes: Optional[Dict[str, List["TextEdit"]]] = attrs.field(default=None)
     """Holds changes to existing resources."""
 
     document_changes: Optional[
         List[Union["TextDocumentEdit", "CreateFile", "RenameFile", "DeleteFile"]]
     ] = attrs.field(default=None)
-    """Depending on the client capability
-    `workspace.workspaceEdit.resourceOperations` document changes are either an
-    array of `TextDocumentEdit`s to express changes to n different text
-    documents where each text document edit addresses a specific version of a
-    text document. Or it can contain above `TextDocumentEdit`s mixed with
-    create, rename and delete file / folder operations.
+    """Depending on the client capability `workspace.workspaceEdit.resourceOperations`
+    document changes are either an array of `TextDocumentEdit`s to express changes to n
+    different text documents where each text document edit addresses a specific version
+    of a text document. Or it can contain above `TextDocumentEdit`s mixed with create,
+    rename and delete file / folder operations.
 
     Whether a client supports versioned document edits is expressed via
     `workspace.workspaceEdit.documentChanges` client capability.
 
-    If a client neither supports `documentChanges` nor `workspace.workspaceEdit.resourceOperations` then
-    only plain `TextEdit`s using the `changes` property are supported.
+    If a client neither supports `documentChanges` nor
+    `workspace.workspaceEdit.resourceOperations` then only plain `TextEdit`s using the
+    `changes` property are supported.
     """
 
     change_annotations: Optional[
         Dict[ChangeAnnotationIdentifier, "ChangeAnnotation"]
     ] = attrs.field(default=None)
-    """A map of change annotations that can be referenced in
-    `AnnotatedTextEdit`s or create, rename and delete file / folder operations.
+    """A map of change annotations that can be referenced in `AnnotatedTextEdit`s or
+    create, rename and delete file / folder operations.
 
     Whether clients honor this property depends on the client capability `workspace.changeAnnotationSupport`.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
@@ -2228,34 +2183,33 @@
 
     filters: List["FileOperationFilter"] = attrs.field()
     """The actual filters."""
 
 
 @attrs.define
 class RenameFilesParams:
-    """The parameters sent in notifications/requests for user-initiated renames
-    of files.
+    """The parameters sent in notifications/requests for user-initiated renames of
+    files.
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
 
     files: List["FileRename"] = attrs.field()
     """An array of all files/folders renamed in this operation.
 
-    When a folder is renamed, only the folder will be included, and not
-    its children.
+    When a folder is renamed, only the folder will be included, and not its children.
     """
 
 
 @attrs.define
 class DeleteFilesParams:
-    """The parameters sent in notifications/requests for user-initiated deletes
-    of files.
+    """The parameters sent in notifications/requests for user-initiated deletes of
+    files.
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
 
     files: List["FileDelete"] = attrs.field()
@@ -2292,16 +2246,16 @@
 
     For example tsc or .Net
     """
 
     identifier: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The identifier of the moniker.
 
-    The value is opaque in LSIF however schema owners are allowed to
-    define the structure if they want.
+    The value is opaque in LSIF however schema owners are allowed to define the
+    structure if they want.
     """
 
     unique: UniquenessLevel = attrs.field()
     """The scope in which the moniker is unique."""
 
     kind: Optional[MonikerKind] = attrs.field(default=None)
     """The moniker kind if known."""
@@ -2318,16 +2272,15 @@
 @attrs.define
 class MonikerRegistrationOptions:
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
@@ -2363,40 +2316,39 @@
     kind: SymbolKind = attrs.field()
     """The kind of this item."""
 
     uri: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The resource identifier of this item."""
 
     range: "Range" = attrs.field()
-    """The range enclosing this symbol not including leading/trailing
-    whitespace but everything else, e.g. comments and code."""
+    """The range enclosing this symbol not including leading/trailing whitespace but
+    everything else, e.g. comments and code."""
 
     selection_range: "Range" = attrs.field()
-    """The range that should be selected and revealed when this symbol is being
-    picked, e.g. the name of a function. Must be contained by the.
+    """The range that should be selected and revealed when this symbol is being picked,
+    e.g. the name of a function.
 
-    {@link TypeHierarchyItem.range `range`}.
+    Must be contained by the {@link TypeHierarchyItem.range `range`}.
     """
 
     tags: Optional[List[SymbolTag]] = attrs.field(default=None)
     """Tags for this item."""
 
     detail: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """More detail for this item, e.g. the signature of a function."""
 
     data: Optional[LSPAny] = attrs.field(default=None)
-    """A data entry field that is preserved between a type hierarchy prepare
-    and supertypes or subtypes requests.
+    """A data entry field that is preserved between a type hierarchy prepare and
+    supertypes or subtypes requests.
 
-    It could also be used to identify the type hierarchy in the server,
-    helping improve the performance on resolving supertypes and
-    subtypes.
+    It could also be used to identify the type hierarchy in the server, helping improve
+    the performance on resolving supertypes and subtypes.
     """
 
 
 @attrs.define
 class TypeHierarchyOptions:
     """Type hierarchy options used during static registration.
 
@@ -2421,31 +2373,29 @@
     # Since: 3.17.0
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class TypeHierarchySupertypesParams:
     """The parameter of a `typeHierarchy/supertypes` request.
 
@@ -2536,26 +2486,24 @@
     )
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class InlayHintParams:
     """A parameter literal used in inlay hint requests.
 
@@ -2583,33 +2531,32 @@
 
     # Since: 3.17.0
 
     position: "Position" = attrs.field()
     """The position of this hint."""
 
     label: Union[str, List["InlayHintLabelPart"]] = attrs.field()
-    """The label of this hint. A human readable string or an array of
-    InlayHintLabelPart label parts.
+    """The label of this hint. A human readable string or an array of InlayHintLabelPart
+    label parts.
 
     *Note* that neither the string nor the label part can be empty.
     """
 
     kind: Optional[InlayHintKind] = attrs.field(default=None)
     """The kind of this hint.
 
-    Can be omitted in which case the client should fall back to a
-    reasonable default.
+    Can be omitted in which case the client should fall back to a reasonable default.
     """
 
     text_edits: Optional[List["TextEdit"]] = attrs.field(default=None)
     """Optional text edits that are performed when accepting this inlay hint.
 
-    *Note* that edits are expected to change the document so that the inlay
-    hint (or its nearest variant) is now part of the document and the inlay
-    hint itself is now obsolete.
+    *Note* that edits are expected to change the document so that the inlay hint (or its
+    nearest variant) is now part of the document and the inlay hint itself is now
+    obsolete.
     """
 
     tooltip: Optional[Union[str, "MarkupContent"]] = attrs.field(default=None)
     """The tooltip text when you hover over this item."""
 
     padding_left: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -2647,16 +2594,16 @@
 
     # Since: 3.17.0
 
     resolve_provider: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The server provides support to resolve additional information for an
-    inlay hint item."""
+    """The server provides support to resolve additional information for an inlay hint
+    item."""
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
 
@@ -2669,39 +2616,37 @@
 
     # Since: 3.17.0
 
     resolve_provider: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The server provides support to resolve additional information for an
-    inlay hint item."""
+    """The server provides support to resolve additional information for an inlay hint
+    item."""
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class DocumentDiagnosticParams:
     """Parameters of the document diagnostic request.
 
@@ -2767,32 +2712,31 @@
     """
 
     # Since: 3.17.0
 
     inter_file_dependencies: bool = attrs.field(
         validator=attrs.validators.instance_of(bool)
     )
-    """Whether the language has inter file dependencies meaning that editing
-    code in one file can result in a different diagnostic set in another file.
+    """Whether the language has inter file dependencies meaning that editing code in one
+    file can result in a different diagnostic set in another file.
 
-    Inter file dependencies are common for most programming languages
-    and typically uncommon for linters.
+    Inter file dependencies are common for most programming languages and typically
+    uncommon for linters.
     """
 
     workspace_diagnostics: bool = attrs.field(
         validator=attrs.validators.instance_of(bool)
     )
     """The server provides support for workspace diagnostics as well."""
 
     identifier: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """An optional identifier under which the diagnostics are managed by the
-    client."""
+    """An optional identifier under which the diagnostics are managed by the client."""
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
 
@@ -2804,70 +2748,66 @@
     """
 
     # Since: 3.17.0
 
     inter_file_dependencies: bool = attrs.field(
         validator=attrs.validators.instance_of(bool)
     )
-    """Whether the language has inter file dependencies meaning that editing
-    code in one file can result in a different diagnostic set in another file.
+    """Whether the language has inter file dependencies meaning that editing code in one
+    file can result in a different diagnostic set in another file.
 
-    Inter file dependencies are common for most programming languages
-    and typically uncommon for linters.
+    Inter file dependencies are common for most programming languages and typically
+    uncommon for linters.
     """
 
     workspace_diagnostics: bool = attrs.field(
         validator=attrs.validators.instance_of(bool)
     )
     """The server provides support for workspace diagnostics as well."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     identifier: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """An optional identifier under which the diagnostics are managed by the
-    client."""
+    """An optional identifier under which the diagnostics are managed by the client."""
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class WorkspaceDiagnosticParams:
     """Parameters of the workspace diagnostic request.
 
     @since 3.17.0
     """
 
     # Since: 3.17.0
 
     previous_result_ids: List["PreviousResultId"] = attrs.field()
-    """The currently known diagnostic reports with their previous result
-    ids."""
+    """The currently known diagnostic reports with their previous result ids."""
 
     identifier: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The additional identifier provided during registration."""
 
@@ -2927,17 +2867,17 @@
     """
 
     # Since: 3.17.0
 
     notebook_document: "VersionedNotebookDocumentIdentifier" = attrs.field()
     """The notebook document that did change.
 
-    The version number points to the version after all provided changes
-    have been applied. If only the text document content of a cell
-    changes the notebook version doesn't necessarily have to change.
+    The version number points to the version after all provided changes have been
+    applied. If only the text document content of a cell changes the notebook version
+    doesn't necessarily have to change.
     """
 
     change: "NotebookDocumentChangeEvent" = attrs.field()
     """The actual changes to the notebook document.
 
     The changes describe single state changes to the notebook document.
     So if there are two changes c1 (at array index 0) and c2 (at array
@@ -2975,16 +2915,16 @@
 
     # Since: 3.17.0
 
     notebook_document: "NotebookDocumentIdentifier" = attrs.field()
     """The notebook document that got closed."""
 
     cell_text_documents: List["TextDocumentIdentifier"] = attrs.field()
-    """The text documents that represent the content of a notebook cell that
-    got closed."""
+    """The text documents that represent the content of a notebook cell that got
+    closed."""
 
 
 @attrs.define
 class RegistrationParams:
     registrations: List["Registration"] = attrs.field()
 
 
@@ -3011,31 +2951,31 @@
 
     capabilities: "ClientCapabilities" = attrs.field()
     """The capabilities provided by the client (editor or tool)"""
 
     process_id: Optional[Union[int, None]] = attrs.field(default=None)
     """The process Id of the parent process that started the server.
 
-    Is `null` if the process has not been started by another process. If
-    the parent process is not alive then the server should exit.
+    Is `null` if the process has not been started by another process. If the parent
+    process is not alive then the server should exit.
     """
 
     client_info: Optional["InitializeParamsClientInfoType"] = attrs.field(default=None)
     """Information about the client.
 
     @since 3.15.0
     """
     # Since: 3.15.0
 
     locale: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """The locale the client is currently showing the user interface in. This
-    must not necessarily be the locale of the operating system.
+    """The locale the client is currently showing the user interface in. This must not
+    necessarily be the locale of the operating system.
 
     Uses IETF language tags as the value's syntax
     (See https://en.wikipedia.org/wiki/IETF_language_tag)
 
     @since 3.16.0
     """
     # Since: 3.16.0
@@ -3043,16 +2983,16 @@
     root_path: Optional[Union[str, None]] = attrs.field(default=None)
     """The rootPath of the workspace. Is null if no folder is open.
 
     @deprecated in favour of rootUri.
     """
 
     root_uri: Optional[Union[str, None]] = attrs.field(default=None)
-    """The rootUri of the workspace. Is null if no folder is open. If both
-    `rootPath` and `rootUri` are set `rootUri` wins.
+    """The rootUri of the workspace. Is null if no folder is open. If both `rootPath`
+    and `rootUri` are set `rootUri` wins.
 
     @deprecated in favour of workspaceFolders.
     """
 
     initialization_options: Optional[LSPAny] = attrs.field(default=None)
     """User provided initialization options."""
 
@@ -3086,31 +3026,31 @@
 class InitializeParams:
     capabilities: "ClientCapabilities" = attrs.field()
     """The capabilities provided by the client (editor or tool)"""
 
     process_id: Optional[Union[int, None]] = attrs.field(default=None)
     """The process Id of the parent process that started the server.
 
-    Is `null` if the process has not been started by another process. If
-    the parent process is not alive then the server should exit.
+    Is `null` if the process has not been started by another process. If the parent
+    process is not alive then the server should exit.
     """
 
     client_info: Optional["InitializeParamsClientInfoType"] = attrs.field(default=None)
     """Information about the client.
 
     @since 3.15.0
     """
     # Since: 3.15.0
 
     locale: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """The locale the client is currently showing the user interface in. This
-    must not necessarily be the locale of the operating system.
+    """The locale the client is currently showing the user interface in. This must not
+    necessarily be the locale of the operating system.
 
     Uses IETF language tags as the value's syntax
     (See https://en.wikipedia.org/wiki/IETF_language_tag)
 
     @since 3.16.0
     """
     # Since: 3.16.0
@@ -3118,16 +3058,16 @@
     root_path: Optional[Union[str, None]] = attrs.field(default=None)
     """The rootPath of the workspace. Is null if no folder is open.
 
     @deprecated in favour of rootUri.
     """
 
     root_uri: Optional[Union[str, None]] = attrs.field(default=None)
-    """The rootUri of the workspace. Is null if no folder is open. If both
-    `rootPath` and `rootUri` are set `rootUri` wins.
+    """The rootUri of the workspace. Is null if no folder is open. If both `rootPath`
+    and `rootUri` are set `rootUri` wins.
 
     @deprecated in favour of workspaceFolders.
     """
 
     initialization_options: Optional[LSPAny] = attrs.field(default=None)
     """User provided initialization options."""
 
@@ -3182,18 +3122,17 @@
 
 
 @attrs.define
 class InitializeError:
     """The data type of the ResponseError if the initialize request fails."""
 
     retry: bool = attrs.field(validator=attrs.validators.instance_of(bool))
-    """Indicates whether the client execute the following retry logic: (1) show
-    the message provided by the ResponseError to the user (2) user selects
-    retry or cancel (3) if user selected retry the initialize method is sent
-    again."""
+    """Indicates whether the client execute the following retry logic: (1) show the
+    message provided by the ResponseError to the user (2) user selects retry or cancel
+    (3) if user selected retry the initialize method is sent again."""
 
 
 @attrs.define
 class InitializedParams:
     pass
 
 
@@ -3270,48 +3209,46 @@
 @attrs.define
 class DidChangeTextDocumentParams:
     """The change text document notification's parameters."""
 
     text_document: "VersionedTextDocumentIdentifier" = attrs.field()
     """The document that did change.
 
-    The version number points to the version after all provided content
-    changes have been applied.
+    The version number points to the version after all provided content changes have
+    been applied.
     """
 
     content_changes: List[TextDocumentContentChangeEvent] = attrs.field()
-    """The actual content changes. The content changes describe single state
-    changes to the document. So if there are two content changes c1 (at array
-    index 0) and c2 (at array index 1) for a document in state S then c1 moves
-    the document from S to S' and c2 from S' to S''. So c1 is computed on the
-    state S and c2 is computed on the state S'.
+    """The actual content changes. The content changes describe single state changes to
+    the document. So if there are two content changes c1 (at array index 0) and c2 (at
+    array index 1) for a document in state S then c1 moves the document from S to S' and
+    c2 from S' to S''. So c1 is computed on the state S and c2 is computed on the state
+    S'.
 
     To mirror the content of a document using change events use the following approach:
     - start with the same initial content
     - apply the 'textDocument/didChange' notifications in the order you receive them.
     - apply the `TextDocumentContentChangeEvent`s in a single notification in the order
       you receive them.
     """
 
 
 @attrs.define
 class TextDocumentChangeRegistrationOptions:
-    """Describe options to be used when registered for text document change
-    events."""
+    """Describe options to be used when registered for text document change events."""
 
     sync_kind: TextDocumentSyncKind = attrs.field()
     """How documents are synced to the server."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
 
 @attrs.define
 class DidCloseTextDocumentParams:
     """The parameters sent in a close text document notification."""
 
@@ -3328,16 +3265,15 @@
 
     text: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """Optional the content when saved.
 
-    Depends on the includeText value when the save notification was
-    requested.
+    Depends on the includeText value when the save notification was requested.
     """
 
 
 @attrs.define
 class SaveOptions:
     """Save options."""
 
@@ -3353,16 +3289,15 @@
     """Save registration options."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     include_text: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """The client is supposed to include the content on save."""
@@ -3402,16 +3337,15 @@
 
     changes: List["FileEvent"] = attrs.field()
     """The actual file events."""
 
 
 @attrs.define
 class DidChangeWatchedFilesRegistrationOptions:
-    """Describe options to be used when registered for text document change
-    events."""
+    """Describe options to be used when registered for text document change events."""
 
     watchers: List["FileSystemWatcher"] = attrs.field()
     """The watchers to register."""
 
 
 @attrs.define
 class PublishDiagnosticsParams:
@@ -3422,16 +3356,15 @@
 
     diagnostics: List["Diagnostic"] = attrs.field()
     """An array of diagnostic information items."""
 
     version: Optional[int] = attrs.field(
         validator=attrs.validators.optional(validators.integer_validator), default=None
     )
-    """Optional the version number of the document the diagnostics are
-    published for.
+    """Optional the version number of the document the diagnostics are published for.
 
     @since 3.15.0
     """
     # Since: 3.15.0
 
 
 @attrs.define
@@ -3443,40 +3376,39 @@
 
     position: "Position" = attrs.field()
     """The position inside the text document."""
 
     context: Optional["CompletionContext"] = attrs.field(default=None)
     """The completion context.
 
-    This is only available it the client specifies to send this using
-    the client capability `textDocument.completion.contextSupport ===
-    true`
+    This is only available it the client specifies to send this using the client
+    capability `textDocument.completion.contextSupport === true`
     """
 
     work_done_token: Optional[ProgressToken] = attrs.field(default=None)
     """An optional token that a server can use to report work done progress."""
 
     partial_result_token: Optional[ProgressToken] = attrs.field(default=None)
     """An optional token that a server can use to report partial results (e.g.
     streaming) to the client."""
 
 
 @attrs.define
 class CompletionItem:
-    """A completion item represents a text snippet that is proposed to complete
-    text that is being typed."""
+    """A completion item represents a text snippet that is proposed to complete text
+    that is being typed."""
 
     label: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The label of this completion item.
 
-    The label property is also by default the text that
-    is inserted when selecting this completion.
+    The label property is also by default the text that is inserted when selecting this
+    completion.
 
-    If label details are provided the label itself should
-    be an unqualified name of the completion item.
+    If label details are provided the label itself should be an unqualified name of the
+    completion item.
     """
 
     label_details: Optional["CompletionItemLabelDetails"] = attrs.field(default=None)
     """Additional details for the label.
 
     @since 3.17.0
     """
@@ -3495,16 +3427,16 @@
     """
     # Since: 3.15.0
 
     detail: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """A human-readable string with additional information about this item,
-    like type or symbol information."""
+    """A human-readable string with additional information about this item, like type or
+    symbol information."""
 
     documentation: Optional[Union[str, "MarkupContent"]] = attrs.field(default=None)
     """A human-readable string that represents a doc-comment."""
 
     deprecated: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
@@ -3516,17 +3448,17 @@
 
     preselect: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Select this item when showing.
 
-    *Note* that only one completion item can be selected and that the
-    tool / client decides which item that is. The rule is that the *first*
-    item of those that match best is selected.
+    *Note* that only one completion item can be selected and that the tool / client
+    decides which item that is. The rule is that the *first* item of those that match
+    best is selected.
     """
 
     sort_text: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """A string that should be used when comparing this item with other items.
@@ -3543,51 +3475,47 @@
     When `falsy` the {@link CompletionItem.label label} is used.
     """
 
     insert_text: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """A string that should be inserted into a document when selecting this
-    completion. When `falsy` the {@link CompletionItem.label label} is used.
+    """A string that should be inserted into a document when selecting this completion.
+    When `falsy` the {@link CompletionItem.label label} is used.
 
-    The `insertText` is subject to interpretation by the client side.
-    Some tools might not take the string literally. For example VS Code
-    when code complete is requested in this example `con<cursor
-    position>` and a completion item with an `insertText` of `console`
-    is provided it will only insert `sole`. Therefore it is recommended
-    to use `textEdit` instead since it avoids additional client side
-    interpretation.
+    The `insertText` is subject to interpretation by the client side. Some tools might
+    not take the string literally. For example VS Code when code complete is requested
+    in this example `con<cursor position>` and a completion item with an `insertText` of
+    `console` is provided it will only insert `sole`. Therefore it is recommended to use
+    `textEdit` instead since it avoids additional client side interpretation.
     """
 
     insert_text_format: Optional[InsertTextFormat] = attrs.field(default=None)
-    """The format of the insert text. The format applies to both the
-    `insertText` property and the `newText` property of a provided `textEdit`.
-    If omitted defaults to `InsertTextFormat.PlainText`.
+    """The format of the insert text. The format applies to both the `insertText`
+    property and the `newText` property of a provided `textEdit`. If omitted defaults to
+    `InsertTextFormat.PlainText`.
 
-    Please note that the insertTextFormat doesn't apply to
-    `additionalTextEdits`.
+    Please note that the insertTextFormat doesn't apply to `additionalTextEdits`.
     """
 
     insert_text_mode: Optional[InsertTextMode] = attrs.field(default=None)
-    """How whitespace and indentation is handled during completion item
-    insertion. If not provided the clients default value depends on the
+    """How whitespace and indentation is handled during completion item insertion. If
+    not provided the clients default value depends on the
     `textDocument.completion.insertTextMode` client capability.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     text_edit: Optional[Union[TextEdit, "InsertReplaceEdit"]] = attrs.field(
         default=None
     )
-    """An {@link TextEdit edit} which is applied to a document when selecting
-    this completion. When an edit is provided the value of.
-
-    {@link CompletionItem.insertText insertText} is ignored.
+    """An {@link TextEdit edit} which is applied to a document when selecting this
+    completion. When an edit is provided the value of {@link CompletionItem.insertText
+    insertText} is ignored.
 
     Most editors support two different operations when accepting a completion
     item. One is to insert a completion text and the other is to replace an
     existing text with a completion text. Since this can usually not be
     predetermined by a server it can report both ranges. Clients need to
     signal support for `InsertReplaceEdits` via the
     `textDocument.completion.insertReplaceSupport` client capability
@@ -3604,61 +3532,56 @@
     """
     # Since: 3.16.0 additional type `InsertReplaceEdit`
 
     text_edit_text: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """The edit text used if the completion item is part of a CompletionList
-    and CompletionList defines an item default for the text edit range.
+    """The edit text used if the completion item is part of a CompletionList and
+    CompletionList defines an item default for the text edit range.
 
     Clients will only honor this property if they opt into completion list
     item defaults using the capability `completionList.itemDefaults`.
 
     If not provided and a list's default range is provided the label
     property is used as a text.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
     additional_text_edits: Optional[List[TextEdit]] = attrs.field(default=None)
-    """An optional array of additional {@link TextEdit text edits} that are
-    applied when selecting this completion. Edits must not overlap (including
-    the same insert position) with the main {@link CompletionItem.textEdit
-    edit} nor with themselves.
-
-    Additional text edits should be used to change text unrelated to the
-    current cursor position (for example adding an import statement at
-    the top of the file if the completion item will insert an
-    unqualified type).
+    """An optional array of additional {@link TextEdit text edits} that are applied when
+    selecting this completion. Edits must not overlap (including the same insert
+    position) with the main {@link CompletionItem.textEdit edit} nor with themselves.
+
+    Additional text edits should be used to change text unrelated to the current cursor
+    position (for example adding an import statement at the top of the file if the
+    completion item will insert an unqualified type).
     """
 
     commit_characters: Optional[List[str]] = attrs.field(default=None)
-    """An optional set of characters that when pressed while this completion is
-    active will accept it first and then type that character.
+    """An optional set of characters that when pressed while this completion is active
+    will accept it first and then type that character.
 
     *Note* that all commit characters should have `length=1` and that superfluous
     characters will be ignored.
     """
 
     command: Optional["Command"] = attrs.field(default=None)
-    """An optional {@link Command command} that is executed *after* inserting
-    this completion. *Note* that additional modifications to the current
-    document should be described with the.
+    """An optional {@link Command command} that is executed *after* inserting this
+    completion.
 
-    {@link CompletionItem.additionalTextEdits
-    additionalTextEdits}-property.
+    *Note* that additional modifications to the current document should be described
+    with the {@link CompletionItem.additionalTextEdits additionalTextEdits}-property.
     """
 
     data: Optional[LSPAny] = attrs.field(default=None)
-    """A data entry field that is preserved on a completion item between a.
-
-    {@link CompletionRequest} and a {@link CompletionResolveRequest}.
-    """
+    """A data entry field that is preserved on a completion item between a {@link
+    CompletionRequest} and a {@link CompletionResolveRequest}."""
 
 
 @attrs.define
 class CompletionListItemDefaultsTypeEditRangeType1:
     insert: "Range" = attrs.field()
 
     replace: "Range" = attrs.field()
@@ -3706,31 +3629,30 @@
 
 @attrs.define
 class CompletionList:
     """Represents a collection of {@link CompletionItem completion items} to be
     presented in the editor."""
 
     is_incomplete: bool = attrs.field(validator=attrs.validators.instance_of(bool))
-    """This list it not complete. Further typing results in recomputing this
-    list.
+    """This list it not complete. Further typing results in recomputing this list.
 
-    Recomputed lists have all their items replaced (not appended) in the
-    incomplete completion sessions.
+    Recomputed lists have all their items replaced (not appended) in the incomplete
+    completion sessions.
     """
 
     items: List[CompletionItem] = attrs.field()
     """The completion items."""
 
     item_defaults: Optional["CompletionListItemDefaultsType"] = attrs.field(
         default=None
     )
-    """In many cases the items of an actual completion result share the same
-    value for properties like `commitCharacters` or the range of a text edit. A
-    completion list can therefore define item defaults which will be used if a
-    completion item itself doesn't specify the value.
+    """In many cases the items of an actual completion result share the same value for
+    properties like `commitCharacters` or the range of a text edit. A completion list
+    can therefore define item defaults which will be used if a completion item itself
+    doesn't specify the value.
 
     If a completion list specifies a default value and a completion item
     also specifies a corresponding value the one from the item is used.
 
     Servers are only allowed to return default values if the client
     signals support for this via the `completionList.itemDefaults`
     capability.
@@ -3743,64 +3665,60 @@
 @attrs.define
 class CompletionOptionsCompletionItemType:
     label_details_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """The server has support for completion item label details (see also
-    `CompletionItemLabelDetails`) when receiving a completion item in a resolve
-    call.
+    `CompletionItemLabelDetails`) when receiving a completion item in a resolve call.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
 
 @attrs.define
 class CompletionOptions:
     """Completion options."""
 
     trigger_characters: Optional[List[str]] = attrs.field(default=None)
-    """Most tools trigger completion request automatically without explicitly
-    requesting it using a keyboard shortcut (e.g. Ctrl+Space). Typically they
-    do so when the user starts to type an identifier. For example if the user
-    types `c` in a JavaScript file code complete will automatically pop up
-    present `console` besides others as a completion item. Characters that make
-    up identifiers don't need to be listed here.
-
-    If code complete should automatically be trigger on characters not
-    being valid inside an identifier (for example `.` in JavaScript)
-    list them in `triggerCharacters`.
+    """Most tools trigger completion request automatically without explicitly requesting
+    it using a keyboard shortcut (e.g. Ctrl+Space). Typically they do so when the user
+    starts to type an identifier. For example if the user types `c` in a JavaScript file
+    code complete will automatically pop up present `console` besides others as a
+    completion item. Characters that make up identifiers don't need to be listed here.
+
+    If code complete should automatically be trigger on characters not being valid
+    inside an identifier (for example `.` in JavaScript) list them in
+    `triggerCharacters`.
     """
 
     all_commit_characters: Optional[List[str]] = attrs.field(default=None)
-    """The list of all possible characters that commit a completion. This field
-    can be used if clients don't support individual commit characters per
-    completion item. See `ClientCapabilities.textDocument.completion.completion
-    Item.commitCharactersSupport`
+    """The list of all possible characters that commit a completion. This field can be
+    used if clients don't support individual commit characters per completion item. See
+    `ClientCapabilities.textDocument.completion.completion Item.commitCharactersSupport`
 
     If a server provides both `allCommitCharacters` and commit characters on an individual
     completion item the ones on the completion item win.
 
     @since 3.2.0
     """
     # Since: 3.2.0
 
     resolve_provider: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The server provides support to resolve additional information for a
-    completion item."""
+    """The server provides support to resolve additional information for a completion
+    item."""
 
     completion_item: Optional["CompletionOptionsCompletionItemType"] = attrs.field(
         default=None
     )
-    """The server supports the following `CompletionItem` specific
-    capabilities.
+    """The server supports the following `CompletionItem` specific capabilities.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -3811,16 +3729,15 @@
 @attrs.define
 class CompletionRegistrationOptionsCompletionItemType:
     label_details_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """The server has support for completion item label details (see also
-    `CompletionItemLabelDetails`) when receiving a completion item in a resolve
-    call.
+    `CompletionItemLabelDetails`) when receiving a completion item in a resolve call.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
 
 @attrs.define
@@ -3828,56 +3745,52 @@
     """Registration options for a {@link CompletionRequest}."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     trigger_characters: Optional[List[str]] = attrs.field(default=None)
-    """Most tools trigger completion request automatically without explicitly
-    requesting it using a keyboard shortcut (e.g. Ctrl+Space). Typically they
-    do so when the user starts to type an identifier. For example if the user
-    types `c` in a JavaScript file code complete will automatically pop up
-    present `console` besides others as a completion item. Characters that make
-    up identifiers don't need to be listed here.
-
-    If code complete should automatically be trigger on characters not
-    being valid inside an identifier (for example `.` in JavaScript)
-    list them in `triggerCharacters`.
+    """Most tools trigger completion request automatically without explicitly requesting
+    it using a keyboard shortcut (e.g. Ctrl+Space). Typically they do so when the user
+    starts to type an identifier. For example if the user types `c` in a JavaScript file
+    code complete will automatically pop up present `console` besides others as a
+    completion item. Characters that make up identifiers don't need to be listed here.
+
+    If code complete should automatically be trigger on characters not being valid
+    inside an identifier (for example `.` in JavaScript) list them in
+    `triggerCharacters`.
     """
 
     all_commit_characters: Optional[List[str]] = attrs.field(default=None)
-    """The list of all possible characters that commit a completion. This field
-    can be used if clients don't support individual commit characters per
-    completion item. See `ClientCapabilities.textDocument.completion.completion
-    Item.commitCharactersSupport`
+    """The list of all possible characters that commit a completion. This field can be
+    used if clients don't support individual commit characters per completion item. See
+    `ClientCapabilities.textDocument.completion.completion Item.commitCharactersSupport`
 
     If a server provides both `allCommitCharacters` and commit characters on an individual
     completion item the ones on the completion item win.
 
     @since 3.2.0
     """
     # Since: 3.2.0
 
     resolve_provider: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The server provides support to resolve additional information for a
-    completion item."""
+    """The server provides support to resolve additional information for a completion
+    item."""
 
     completion_item: Optional[
         "CompletionRegistrationOptionsCompletionItemType"
     ] = attrs.field(default=None)
-    """The server supports the following `CompletionItem` specific
-    capabilities.
+    """The server supports the following `CompletionItem` specific capabilities.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -3903,16 +3816,16 @@
 class Hover:
     """The result of a hover request."""
 
     contents: Union["MarkupContent", MarkedString, List[MarkedString]] = attrs.field()
     """The hover's content."""
 
     range: Optional["Range"] = attrs.field(default=None)
-    """An optional range inside the text document that is used to visualize the
-    hover, e.g. by changing the background color."""
+    """An optional range inside the text document that is used to visualize the hover,
+    e.g. by changing the background color."""
 
 
 @attrs.define
 class HoverOptions:
     """Hover options."""
 
     work_done_progress: Optional[bool] = attrs.field(
@@ -3926,16 +3839,15 @@
     """Registration options for a {@link HoverRequest}."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
@@ -3947,62 +3859,60 @@
     text_document: "TextDocumentIdentifier" = attrs.field()
     """The text document."""
 
     position: "Position" = attrs.field()
     """The position inside the text document."""
 
     context: Optional["SignatureHelpContext"] = attrs.field(default=None)
-    """The signature help context. This is only available if the client
-    specifies to send this using the client capability
-    `textDocument.signatureHelp.contextSupport === true`
+    """The signature help context. This is only available if the client specifies to
+    send this using the client capability `textDocument.signatureHelp.contextSupport ===
+    true`
 
     @since 3.15.0
     """
     # Since: 3.15.0
 
     work_done_token: Optional[ProgressToken] = attrs.field(default=None)
     """An optional token that a server can use to report work done progress."""
 
 
 @attrs.define
 class SignatureHelp:
     """Signature help represents the signature of something callable.
 
-    There can be multiple signature but only one active and only one
-    active parameter.
+    There can be multiple signature but only one active and only one active parameter.
     """
 
     signatures: List["SignatureInformation"] = attrs.field()
     """One or more signatures."""
 
     active_signature: Optional[int] = attrs.field(
         validator=attrs.validators.optional(validators.uinteger_validator), default=None
     )
     """The active signature. If omitted or the value lies outside the range of
-    `signatures` the value defaults to zero or is ignored if the
-    `SignatureHelp` has no signatures.
+    `signatures` the value defaults to zero or is ignored if the `SignatureHelp` has no
+    signatures.
 
-    Whenever possible implementors should make an active decision about
-    the active signature and shouldn't rely on a default value.
+    Whenever possible implementors should make an active decision about the active
+    signature and shouldn't rely on a default value.
 
-    In future version of the protocol this property might become
-    mandatory to better express this.
+    In future version of the protocol this property might become mandatory to better
+    express this.
     """
 
     active_parameter: Optional[int] = attrs.field(
         validator=attrs.validators.optional(validators.uinteger_validator), default=None
     )
     """The active parameter of the active signature.
 
     If omitted or the value lies outside the range of
-    `signatures[activeSignature].parameters` defaults to 0 if the active
-    signature has parameters. If the active signature has no parameters
-    it is ignored. In future version of the protocol this property might
-    become mandatory to better express the active parameter if the
-    active signature does have any.
+    `signatures[activeSignature].parameters` defaults to 0 if the active signature has
+    parameters. If the active signature has no parameters it is ignored. In future
+    version of the protocol this property might become mandatory to better express the
+    active parameter if the active signature does have any.
     """
 
 
 @attrs.define
 class SignatureHelpOptions:
     """Server Capabilities for a {@link SignatureHelpRequest}."""
 
@@ -4030,16 +3940,15 @@
     """Registration options for a {@link SignatureHelpRequest}."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     trigger_characters: Optional[List[str]] = attrs.field(default=None)
     """List of characters that trigger signature help automatically."""
 
     retrigger_characters: Optional[List[str]] = attrs.field(default=None)
     """List of characters that re-trigger signature help.
@@ -4090,16 +3999,15 @@
     """Registration options for a {@link DefinitionRequest}."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
@@ -4139,16 +4047,15 @@
     """Registration options for a {@link ReferencesRequest}."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
@@ -4169,27 +4076,26 @@
     partial_result_token: Optional[ProgressToken] = attrs.field(default=None)
     """An optional token that a server can use to report partial results (e.g.
     streaming) to the client."""
 
 
 @attrs.define
 class DocumentHighlight:
-    """A document highlight is a range inside a text document which deserves
-    special attention.
+    """A document highlight is a range inside a text document which deserves special
+    attention.
 
-    Usually a document highlight is visualized by changing the
-    background color of its range.
+    Usually a document highlight is visualized by changing the background color of its
+    range.
     """
 
     range: "Range" = attrs.field()
     """The range this highlight applies to."""
 
     kind: Optional[DocumentHighlightKind] = attrs.field(default=None)
-    """The highlight kind, default is {@link DocumentHighlightKind.Text
-    text}."""
+    """The highlight kind, default is {@link DocumentHighlightKind.Text text}."""
 
 
 @attrs.define
 class DocumentHighlightOptions:
     """Provider options for a {@link DocumentHighlightRequest}."""
 
     work_done_progress: Optional[bool] = attrs.field(
@@ -4203,16 +4109,15 @@
     """Registration options for a {@link DocumentHighlightRequest}."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
@@ -4251,35 +4156,33 @@
 
     container_name: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The name of the symbol containing this symbol.
 
-    This information is for user interface purposes (e.g. to render a
-    qualifier in the user interface if necessary). It can't be used to
-    re-infer a hierarchy for the document symbols.
+    This information is for user interface purposes (e.g. to render a qualifier in the
+    user interface if necessary). It can't be used to re-infer a hierarchy for the
+    document symbols.
     """
 
 
 @attrs.define
 class SymbolInformation:
-    """Represents information about programming constructs like variables,
-    classes, interfaces etc."""
+    """Represents information about programming constructs like variables, classes,
+    interfaces etc."""
 
     location: Location = attrs.field()
-    """The location of this symbol. The location's range is used by a tool to
-    reveal the location in the editor. If the symbol is selected in the tool
-    the range's start information is used to position the cursor. So the range
-    usually spans more than the actual symbol's name and does normally include
-    things like visibility modifiers.
-
-    The range doesn't have to denote a node range in the sense of an
-    abstract syntax tree. It can therefore not be used to re-construct a
-    hierarchy of the symbols.
+    """The location of this symbol. The location's range is used by a tool to reveal the
+    location in the editor. If the symbol is selected in the tool the range's start
+    information is used to position the cursor. So the range usually spans more than the
+    actual symbol's name and does normally include things like visibility modifiers.
+
+    The range doesn't have to denote a node range in the sense of an abstract syntax
+    tree. It can therefore not be used to re-construct a hierarchy of the symbols.
     """
 
     name: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The name of this symbol."""
 
     kind: SymbolKind = attrs.field()
     """The kind of this symbol."""
@@ -4302,52 +4205,51 @@
 
     container_name: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The name of the symbol containing this symbol.
 
-    This information is for user interface purposes (e.g. to render a
-    qualifier in the user interface if necessary). It can't be used to
-    re-infer a hierarchy for the document symbols.
+    This information is for user interface purposes (e.g. to render a qualifier in the
+    user interface if necessary). It can't be used to re-infer a hierarchy for the
+    document symbols.
     """
 
 
 @attrs.define
 class DocumentSymbol:
-    """Represents programming constructs like variables, classes, interfaces
-    etc.
+    """Represents programming constructs like variables, classes, interfaces etc.
 
     that appear in a document. Document symbols can be hierarchical and
     they have two ranges: one that encloses its definition and one that
     points to its most interesting range, e.g. the range of an
     identifier.
     """
 
     name: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The name of this symbol.
 
-    Will be displayed in the user interface and therefore must not be an
-    empty string or a string only consisting of white spaces.
+    Will be displayed in the user interface and therefore must not be an empty string or
+    a string only consisting of white spaces.
     """
 
     kind: SymbolKind = attrs.field()
     """The kind of this symbol."""
 
     range: "Range" = attrs.field()
-    """The range enclosing this symbol not including leading/trailing
-    whitespace but everything else like comments.
+    """The range enclosing this symbol not including leading/trailing whitespace but
+    everything else like comments.
 
-    This information is typically used to determine if the clients
-    cursor is inside the symbol to reveal in the symbol in the UI.
+    This information is typically used to determine if the clients cursor is inside the
+    symbol to reveal in the symbol in the UI.
     """
 
     selection_range: "Range" = attrs.field()
-    """The range that should be selected and revealed when this symbol is being
-    picked, e.g the name of a function.
+    """The range that should be selected and revealed when this symbol is being picked,
+    e.g the name of a function.
 
     Must be contained by the `range`.
     """
 
     detail: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
@@ -4378,16 +4280,16 @@
 class DocumentSymbolOptions:
     """Provider options for a {@link DocumentSymbolRequest}."""
 
     label: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """A human-readable string that is shown when multiple outlines trees are
-    shown for the same document.
+    """A human-readable string that is shown when multiple outlines trees are shown for
+    the same document.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -4400,24 +4302,23 @@
     """Registration options for a {@link DocumentSymbolRequest}."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     label: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """A human-readable string that is shown when multiple outlines trees are
-    shown for the same document.
+    """A human-readable string that is shown when multiple outlines trees are shown for
+    the same document.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -4446,17 +4347,17 @@
     streaming) to the client."""
 
 
 @attrs.define
 class Command:
     """Represents a reference to a command.
 
-    Provides a title which will be used to represent a command in the UI
-    and, optionally, an array of arguments which will be passed to the
-    command handler function when invoked.
+    Provides a title which will be used to represent a command in the UI and,
+    optionally, an array of arguments which will be passed to the command handler
+    function when invoked.
     """
 
     title: str = attrs.field(validator=attrs.validators.instance_of(str))
     """Title of the command, like `save`."""
 
     command: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The identifier of the actual command handler."""
@@ -4472,20 +4373,19 @@
 
     This is displayed in the code actions UI.
     """
 
 
 @attrs.define
 class CodeAction:
-    """A code action represents a change that can be performed in code, e.g. to
-    fix a problem or to refactor code.
+    """A code action represents a change that can be performed in code, e.g. to fix a
+    problem or to refactor code.
 
-    A CodeAction must set either `edit` and/or a `command`. If both are
-    supplied, the `edit` is applied first, then the `command` is
-    executed.
+    A CodeAction must set either `edit` and/or a `command`. If both are supplied, the
+    `edit` is applied first, then the `command` is executed.
     """
 
     title: str = attrs.field(validator=attrs.validators.instance_of(str))
     """A short, human-readable, title for this code action."""
 
     kind: Optional[Union[CodeActionKind, str]] = attrs.field(default=None)
     """The kind of the code action.
@@ -4496,16 +4396,16 @@
     diagnostics: Optional[List["Diagnostic"]] = attrs.field(default=None)
     """The diagnostics that this code action resolves."""
 
     is_preferred: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Marks this as a preferred action. Preferred actions are used by the
-    `auto fix` command and can be targeted by keybindings.
+    """Marks this as a preferred action. Preferred actions are used by the `auto fix`
+    command and can be targeted by keybindings.
 
     A quick fix should be marked preferred if it properly addresses the underlying error.
     A refactoring should be marked preferred if it is the most reasonable choice of actions to take.
 
     @since 3.15.0
     """
     # Since: 3.15.0
@@ -4531,16 +4431,16 @@
 
     edit: Optional[WorkspaceEdit] = attrs.field(default=None)
     """The workspace edit this code action performs."""
 
     command: Optional[Command] = attrs.field(default=None)
     """A command this code action executes.
 
-    If a code action provides an edit and a command, first the edit is
-    executed and then the command.
+    If a code action provides an edit and a command, first the edit is executed and then
+    the command.
     """
 
     data: Optional[LSPAny] = attrs.field(default=None)
     """A data entry field that is preserved on a code action between a
     `textDocument/codeAction` and a `codeAction/resolve` request.
 
     @since 3.16.0
@@ -4553,24 +4453,23 @@
     """Provider options for a {@link CodeActionRequest}."""
 
     code_action_kinds: Optional[List[Union[CodeActionKind, str]]] = attrs.field(
         default=None
     )
     """CodeActionKinds that this server may return.
 
-    The list of kinds may be generic, such as `CodeActionKind.Refactor`,
-    or the server may list out every specific kind they provide.
+    The list of kinds may be generic, such as `CodeActionKind.Refactor`, or the server
+    may list out every specific kind they provide.
     """
 
     resolve_provider: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The server provides support to resolve additional information for a code
-    action.
+    """The server provides support to resolve additional information for a code action.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -4583,33 +4482,31 @@
     """Registration options for a {@link CodeActionRequest}."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     code_action_kinds: Optional[List[Union[CodeActionKind, str]]] = attrs.field(
         default=None
     )
     """CodeActionKinds that this server may return.
 
-    The list of kinds may be generic, such as `CodeActionKind.Refactor`,
-    or the server may list out every specific kind they provide.
+    The list of kinds may be generic, such as `CodeActionKind.Refactor`, or the server
+    may list out every specific kind they provide.
     """
 
     resolve_provider: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The server provides support to resolve additional information for a code
-    action.
+    """The server provides support to resolve additional information for a code action.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -4648,60 +4545,59 @@
 
     @since 3.17.0
     """
 
     # Since: 3.17.0
 
     location: Union[Location, "WorkspaceSymbolLocationType1"] = attrs.field()
-    """The location of the symbol. Whether a server is allowed to return a
-    location without a range depends on the client capability
-    `workspace.symbol.resolveSupport`.
+    """The location of the symbol. Whether a server is allowed to return a location
+    without a range depends on the client capability `workspace.symbol.resolveSupport`.
 
     See SymbolInformation#location for more details.
     """
 
     name: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The name of this symbol."""
 
     kind: SymbolKind = attrs.field()
     """The kind of this symbol."""
 
     data: Optional[LSPAny] = attrs.field(default=None)
-    """A data entry field that is preserved on a workspace symbol between a
-    workspace symbol request and a workspace symbol resolve request."""
+    """A data entry field that is preserved on a workspace symbol between a workspace
+    symbol request and a workspace symbol resolve request."""
 
     tags: Optional[List[SymbolTag]] = attrs.field(default=None)
     """Tags for this symbol.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     container_name: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The name of the symbol containing this symbol.
 
-    This information is for user interface purposes (e.g. to render a
-    qualifier in the user interface if necessary). It can't be used to
-    re-infer a hierarchy for the document symbols.
+    This information is for user interface purposes (e.g. to render a qualifier in the
+    user interface if necessary). It can't be used to re-infer a hierarchy for the
+    document symbols.
     """
 
 
 @attrs.define
 class WorkspaceSymbolOptions:
     """Server capabilities for a {@link WorkspaceSymbolRequest}."""
 
     resolve_provider: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The server provides support to resolve additional information for a
-    workspace symbol.
+    """The server provides support to resolve additional information for a workspace
+    symbol.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -4713,16 +4609,16 @@
 class WorkspaceSymbolRegistrationOptions:
     """Registration options for a {@link WorkspaceSymbolRequest}."""
 
     resolve_provider: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The server provides support to resolve additional information for a
-    workspace symbol.
+    """The server provides support to resolve additional information for a workspace
+    symbol.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -4743,38 +4639,33 @@
     partial_result_token: Optional[ProgressToken] = attrs.field(default=None)
     """An optional token that a server can use to report partial results (e.g.
     streaming) to the client."""
 
 
 @attrs.define
 class CodeLens:
-    """A code lens represents a {@link Command command} that should be shown
-    along with source text, like the number of references, a way to run tests,
-    etc.
-
-    A code lens is _unresolved_ when no command is associated to it. For
-    performance reasons the creation of a code lens and resolving should
-    be done in two stages.
+    """A code lens represents a {@link Command command} that should be shown along with
+    source text, like the number of references, a way to run tests, etc.
+
+    A code lens is _unresolved_ when no command is associated to it. For performance
+    reasons the creation of a code lens and resolving should be done in two stages.
     """
 
     range: "Range" = attrs.field()
     """The range in which this code lens is valid.
 
     Should only span a single line.
     """
 
     command: Optional[Command] = attrs.field(default=None)
     """The command this code lens represents."""
 
     data: Optional[LSPAny] = attrs.field(default=None)
-    """A data entry field that is preserved on a code lens item between a.
-
-    {@link CodeLensRequest} and a [CodeLensResolveRequest]
-    (#CodeLensResolveRequest)
-    """
+    """A data entry field that is preserved on a code lens item between a {@link
+    CodeLensRequest} and a [CodeLensResolveRequest] (#CodeLensResolveRequest)"""
 
 
 @attrs.define
 class CodeLensOptions:
     """Code Lens provider options of a {@link CodeLensRequest}."""
 
     resolve_provider: Optional[bool] = attrs.field(
@@ -4794,16 +4685,15 @@
     """Registration options for a {@link CodeLensRequest}."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     resolve_provider: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Code lens has a resolve provider as well."""
@@ -4827,16 +4717,16 @@
     partial_result_token: Optional[ProgressToken] = attrs.field(default=None)
     """An optional token that a server can use to report partial results (e.g.
     streaming) to the client."""
 
 
 @attrs.define
 class DocumentLink:
-    """A document link is a range in a text document that links to an internal
-    or external resource, like another text document or a web site."""
+    """A document link is a range in a text document that links to an internal or
+    external resource, like another text document or a web site."""
 
     range: "Range" = attrs.field()
     """The range this link applies to."""
 
     target: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
@@ -4886,16 +4776,15 @@
     """Registration options for a {@link DocumentLinkRequest}."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     resolve_provider: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Document links have a resolve provider as well."""
@@ -4935,16 +4824,15 @@
     """Registration options for a {@link DocumentFormattingRequest}."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
@@ -4981,16 +4869,15 @@
     """Registration options for a {@link DocumentRangeFormattingRequest}."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
@@ -5001,25 +4888,24 @@
 
     text_document: "TextDocumentIdentifier" = attrs.field()
     """The document to format."""
 
     position: "Position" = attrs.field()
     """The position around which the on type formatting should happen.
 
-    This is not necessarily the exact position where the character
-    denoted by the property `ch` got typed.
+    This is not necessarily the exact position where the character denoted by the
+    property `ch` got typed.
     """
 
     ch: str = attrs.field(validator=attrs.validators.instance_of(str))
-    """The character that has been typed that triggered the formatting on type
-    request.
+    """The character that has been typed that triggered the formatting on type request.
 
-    That is not necessarily the last character that got inserted into
-    the document since the client could auto insert characters as well
-    (e.g. like automatic brace completion).
+    That is not necessarily the last character that got inserted into the document since
+    the client could auto insert characters as well (e.g. like automatic brace
+    completion).
     """
 
     options: "FormattingOptions" = attrs.field()
     """The formatting options."""
 
 
 @attrs.define
@@ -5045,16 +4931,15 @@
     """A character on which formatting should be triggered, like `{`."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     more_trigger_character: Optional[List[str]] = attrs.field(default=None)
     """More trigger characters."""
 
 
 @attrs.define
@@ -5066,16 +4951,16 @@
 
     position: "Position" = attrs.field()
     """The position at which this request was sent."""
 
     new_name: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The new name of the symbol.
 
-    If the given name is not valid the request must return a {@link
-    ResponseError} with an appropriate message set.
+    If the given name is not valid the request must return a {@link ResponseError} with
+    an appropriate message set.
     """
 
     work_done_token: Optional[ProgressToken] = attrs.field(default=None)
     """An optional token that a server can use to report work done progress."""
 
 
 @attrs.define
@@ -5103,16 +4988,15 @@
     """Registration options for a {@link RenameRequest}."""
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
     prepare_provider: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Renames should be checked and tested before being executed.
@@ -5177,27 +5061,27 @@
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
 
 
 @attrs.define
 class ApplyWorkspaceEditParams:
-    """The parameters passed via a apply workspace edit request."""
+    """The parameters passed via an apply workspace edit request."""
 
     edit: WorkspaceEdit = attrs.field()
     """The edits to apply."""
 
     label: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """An optional label of the workspace edit.
 
-    This label is presented in the user interface for example on an undo
-    stack to undo the workspace edit.
+    This label is presented in the user interface for example on an undo stack to undo
+    the workspace edit.
     """
 
 
 @attrs.define
 class ApplyWorkspaceEditResult:
     """The result returned from the apply workspace edit request.
 
@@ -5211,72 +5095,70 @@
 
     failure_reason: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """An optional textual description for why the edit was not applied.
 
-    This may be used by the server for diagnostic logging or to provide
-    a suitable error for a request that triggered the edit.
+    This may be used by the server for diagnostic logging or to provide a suitable error
+    for a request that triggered the edit.
     """
 
     failed_change: Optional[int] = attrs.field(
         validator=attrs.validators.optional(validators.uinteger_validator), default=None
     )
-    """Depending on the client's failure handling strategy `failedChange` might
-    contain the index of the change that failed.
+    """Depending on the client's failure handling strategy `failedChange` might contain
+    the index of the change that failed.
 
-    This property is only available if the client signals a
-    `failureHandlingStrategy` in its client capabilities.
+    This property is only available if the client signals a `failureHandlingStrategy` in
+    its client capabilities.
     """
 
 
 @attrs.define
 class WorkDoneProgressBegin:
     title: str = attrs.field(validator=attrs.validators.instance_of(str))
-    """Mandatory title of the progress operation. Used to briefly inform about
-    the kind of operation being performed.
+    """Mandatory title of the progress operation. Used to briefly inform about the kind
+    of operation being performed.
 
     Examples: "Indexing" or "Linking dependencies".
     """
 
     kind: str = attrs.field(validator=attrs.validators.in_(["begin"]), default="begin")
 
     cancellable: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Controls if a cancel button should show to allow the user to cancel the
-    long running operation.
+    """Controls if a cancel button should show to allow the user to cancel the long
+    running operation.
 
-    Clients that don't support cancellation are allowed to ignore the
-    setting.
+    Clients that don't support cancellation are allowed to ignore the setting.
     """
 
     message: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """Optional, more detailed associated progress message. Contains
-    complementary information to the `title`.
+    """Optional, more detailed associated progress message. Contains complementary
+    information to the `title`.
 
     Examples: "3/25 files", "project/src/module2", "node_modules/some_dep".
     If unset, the previous progress message (if any) is still valid.
     """
 
     percentage: Optional[int] = attrs.field(
         validator=attrs.validators.optional(validators.uinteger_validator), default=None
     )
-    """Optional progress percentage to display (value 100 is considered 100%).
-    If not provided infinite progress is assumed and clients are allowed to
-    ignore the `percentage` value in subsequent in report notifications.
-
-    The value should be steadily rising. Clients are free to ignore
-    values that are not following this rule. The value range is [0,
-    100].
+    """Optional progress percentage to display (value 100 is considered 100%). If not
+    provided infinite progress is assumed and clients are allowed to ignore the
+    `percentage` value in subsequent in report notifications.
+
+    The value should be steadily rising. Clients are free to ignore values that are not
+    following this rule. The value range is [0, 100].
     """
 
 
 @attrs.define
 class WorkDoneProgressReport:
     kind: str = attrs.field(
         validator=attrs.validators.in_(["report"]), default="report"
@@ -5284,51 +5166,51 @@
 
     cancellable: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Controls enablement state of a cancel button.
 
-    Clients that don't support cancellation or don't support controlling
-    the button's enablement state are allowed to ignore the property.
+    Clients that don't support cancellation or don't support controlling the button's
+    enablement state are allowed to ignore the property.
     """
 
     message: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """Optional, more detailed associated progress message. Contains
-    complementary information to the `title`.
+    """Optional, more detailed associated progress message. Contains complementary
+    information to the `title`.
 
     Examples: "3/25 files", "project/src/module2", "node_modules/some_dep".
     If unset, the previous progress message (if any) is still valid.
     """
 
     percentage: Optional[int] = attrs.field(
         validator=attrs.validators.optional(validators.uinteger_validator), default=None
     )
-    """Optional progress percentage to display (value 100 is considered 100%).
-    If not provided infinite progress is assumed and clients are allowed to
-    ignore the `percentage` value in subsequent in report notifications.
+    """Optional progress percentage to display (value 100 is considered 100%). If not
+    provided infinite progress is assumed and clients are allowed to ignore the
+    `percentage` value in subsequent in report notifications.
 
-    The value should be steadily rising. Clients are free to ignore
-    values that are not following this rule. The value range is [0, 100]
+    The value should be steadily rising. Clients are free to ignore values that are not
+    following this rule. The value range is [0, 100]
     """
 
 
 @attrs.define
 class WorkDoneProgressEnd:
     kind: str = attrs.field(validator=attrs.validators.in_(["end"]), default="end")
 
     message: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """Optional, a final message indicating to for example indicate the outcome
-    of the operation."""
+    """Optional, a final message indicating to for example indicate the outcome of the
+    operation."""
 
 
 @attrs.define
 class SetTraceParams:
     value: TraceValues = attrs.field()
 
 
@@ -5357,50 +5239,47 @@
     """The progress data."""
 
 
 @attrs.define
 class LocationLink:
     """Represents the connection of two locations.
 
-    Provides additional metadata over normal {@link Location locations},
-    including an origin range.
+    Provides additional metadata over normal {@link Location locations}, including an
+    origin range.
     """
 
     target_uri: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The target resource identifier of this link."""
 
     target_range: "Range" = attrs.field()
     """The full target range of this link.
 
-    If the target for example is a symbol then target range is the range
-    enclosing this symbol not including leading/trailing whitespace but
-    everything else like comments. This information is typically used to
-    highlight the range in the editor.
+    If the target for example is a symbol then target range is the range enclosing this
+    symbol not including leading/trailing whitespace but everything else like comments.
+    This information is typically used to highlight the range in the editor.
     """
 
     target_selection_range: "Range" = attrs.field()
-    """The range that should be selected and revealed when this link is being
-    followed, e.g the name of a function.
+    """The range that should be selected and revealed when this link is being followed,
+    e.g the name of a function.
 
-    Must be contained by the `targetRange`. See also
-    `DocumentSymbol#range`
+    Must be contained by the `targetRange`. See also `DocumentSymbol#range`
     """
 
     origin_selection_range: Optional["Range"] = attrs.field(default=None)
     """Span of the origin of this link.
 
-    Used as the underlined span for mouse interaction. Defaults to the
-    word range at the definition position.
+    Used as the underlined span for mouse interaction. Defaults to the word range at the
+    definition position.
     """
 
 
 @attrs.define
 class Range:
-    """A range in a text document expressed as (zero-based) start and end
-    positions.
+    """A range in a text document expressed as (zero-based) start and end positions.
 
     If you want to specify a range that contains a line including the line ending
     character(s) then use an end position denoting the start of the next line.
     For example:
     ```ts
     {
         start: { line: 5, character: 23 }
@@ -5476,62 +5355,58 @@
 
 
 @attrs.define
 @functools.total_ordering
 class Position:
     """Position in a text document expressed as zero-based line and character
     offset. Prior to 3.17 the offsets were always based on a UTF-16 string
-    representation. So a string of the form `a𐐀b` the character offset of the
-    character `a` is 0, the character offset of `𐐀` is 1 and the character
-    offset of b is 3 since `𐐀` is represented using two code units in UTF-16.
-    Since 3.17 clients and servers can agree on a different string encoding
-    representation (e.g. UTF-8). The client announces it's supported encoding
-    via the client capability.
-
+    representation. So a string of the form `a𐐀b` the character offset of
+    the character `a` is 0, the character offset of `𐐀` is 1 and the
+    character offset of b is 3 since `𐐀` is represented using two code units
+    in UTF-16. Since 3.17 clients and servers can agree on a different string
+    encoding representation (e.g. UTF-8). The client announces it's supported
+    encoding via the client capability
     [`general.positionEncodings`](#clientCapabilities). The value is an array
     of position encodings the client supports, with decreasing preference (e.g.
     the encoding at index `0` is the most preferred one). To stay backwards
     compatible the only mandatory encoding is UTF-16 represented via the string
     `utf-16`. The server can pick one of the encodings offered by the client
     and signals that encoding back to the client via the initialize result's
-    property.
-
-    [`capabilities.positionEncoding`](#serverCapabilities). If the string value
-    `utf-16` is missing from the client's capability `general.positionEncodings`
-    servers can safely assume that the client supports UTF-16. If the server
-    omits the position encoding in its initialize result the encoding defaults
-    to the string value `utf-16`. Implementation considerations: since the
-    conversion from one encoding into another requires the content of the
-    file / line the conversion is best done where the file is read which is
-    usually on the server side.
+    property [`capabilities.positionEncoding`](#serverCapabilities). If the
+    string value `utf-16` is missing from the client's capability
+    `general.positionEncodings` servers can safely assume that the client
+    supports UTF-16. If the server omits the position encoding in its
+    initialize result the encoding defaults to the string value `utf-16`.
+    Implementation considerations: since the conversion from one encoding into
+    another requires the content of the file / line the conversion is best done
+    where the file is read which is usually on the server side.
 
     Positions are line end character agnostic. So you can not specify a position
     that denotes `\r|\n` or `\n|` where `|` represents the character offset.
 
     @since 3.17.0 - support for negotiated position encoding.
     """
 
     # Since: 3.17.0 - support for negotiated position encoding.
 
     line: int = attrs.field(validator=validators.uinteger_validator)
     """Line position in a document (zero-based).
 
-    If a line number is greater than the number of lines in a document,
-    it defaults back to the number of lines in the document. If a line
-    number is negative, it defaults to 0.
+    If a line number is greater than the number of lines in a document, it defaults back
+    to the number of lines in the document. If a line number is negative, it defaults to
+    0.
     """
 
     character: int = attrs.field(validator=validators.uinteger_validator)
     """Character offset on a line in a document (zero-based).
 
-    The meaning of this offset is determined by the negotiated
-    `PositionEncodingKind`.
+    The meaning of this offset is determined by the negotiated `PositionEncodingKind`.
 
-    If the character value is greater than the line length it defaults back to the
-    line length.
+    If the character value is greater than the line length it defaults back to the line
+    length.
     """
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, Position):
             return NotImplemented
         return (self.line, self.character) == (o.line, o.character)
 
@@ -5573,19 +5448,18 @@
     """A file:// URI for the location of the file/folder being created."""
 
 
 @attrs.define
 class TextDocumentEdit:
     """Describes textual changes on a text document.
 
-    A TextDocumentEdit describes all changes on a document version Si
-    and after they are applied move the document to version Si+1. So the
-    creator of a TextDocumentEdit doesn't need to sort the array of
-    edits or do any kind of ordering. However the edits must be non
-    overlapping.
+    A TextDocumentEdit describes all changes on a document version Si and after they are
+    applied move the document to version Si+1. So the creator of a TextDocumentEdit
+    doesn't need to sort the array of edits or do any kind of ordering. However the
+    edits must be non overlapping.
     """
 
     text_document: "OptionalVersionedTextDocumentIdentifier" = attrs.field()
     """The text document to change."""
 
     edits: List[Union[TextEdit, "AnnotatedTextEdit"]] = attrs.field()
     """The edits to be applied.
@@ -5698,29 +5572,29 @@
     The string is rendered prominent in the user interface.
     """
 
     needs_confirmation: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """A flag which indicates that user confirmation is needed before applying
-    the change."""
+    """A flag which indicates that user confirmation is needed before applying the
+    change."""
 
     description: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """A human-readable string which is rendered less prominent in the user
     interface."""
 
 
 @attrs.define
 class FileOperationFilter:
-    """A filter to describe in which file operation requests or notifications
-    the server is interested in receiving.
+    """A filter to describe in which file operation requests or notifications the server
+    is interested in receiving.
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
 
     pattern: "FileOperationPattern" = attrs.field()
@@ -5739,16 +5613,15 @@
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
 
     old_uri: str = attrs.field(validator=attrs.validators.instance_of(str))
-    """A file:// URI for the original location of the file/folder being
-    renamed."""
+    """A file:// URI for the original location of the file/folder being renamed."""
 
     new_uri: str = attrs.field(validator=attrs.validators.instance_of(str))
     """A file:// URI for the new location of the file/folder being renamed."""
 
 
 @attrs.define
 class FileDelete:
@@ -5771,16 +5644,16 @@
 
     frame_id: int = attrs.field(validator=validators.integer_validator)
     """The stack frame (as a DAP Id) where the execution has stopped."""
 
     stopped_location: Range = attrs.field()
     """The document range where execution has stopped.
 
-    Typically the end position of the range denotes the line where the
-    inline values are shown.
+    Typically the end position of the range denotes the line where the inline values are
+    shown.
     """
 
 
 @attrs.define
 class InlineValueText:
     """Provide inline value as text.
 
@@ -5794,29 +5667,27 @@
 
     text: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The text of the inline value."""
 
 
 @attrs.define
 class InlineValueVariableLookup:
-    """Provide inline value through a variable lookup. If only a range is
-    specified, the variable name will be extracted from the underlying
-    document. An optional variable name can be used to override the extracted
-    name.
+    """Provide inline value through a variable lookup. If only a range is specified, the
+    variable name will be extracted from the underlying document. An optional variable
+    name can be used to override the extracted name.
 
     @since 3.17.0
     """
 
     # Since: 3.17.0
 
     range: Range = attrs.field()
     """The document range for which the inline value applies.
 
-    The range is used to extract the variable name from the underlying
-    document.
+    The range is used to extract the variable name from the underlying document.
     """
 
     case_sensitive_lookup: bool = attrs.field(
         validator=attrs.validators.instance_of(bool)
     )
     """How to perform the lookup."""
 
@@ -5825,56 +5696,55 @@
         default=None,
     )
     """If specified the name of the variable to look up."""
 
 
 @attrs.define
 class InlineValueEvaluatableExpression:
-    """Provide an inline value through an expression evaluation. If only a
-    range is specified, the expression will be extracted from the underlying
-    document. An optional expression can be used to override the extracted
-    expression.
+    """Provide an inline value through an expression evaluation. If only a range is
+    specified, the expression will be extracted from the underlying document. An
+    optional expression can be used to override the extracted expression.
 
     @since 3.17.0
     """
 
     # Since: 3.17.0
 
     range: Range = attrs.field()
     """The document range for which the inline value applies.
 
-    The range is used to extract the evaluatable expression from the
-    underlying document.
+    The range is used to extract the evaluatable expression from the underlying
+    document.
     """
 
     expression: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """If specified the expression overrides the extracted expression."""
 
 
 @attrs.define
 class InlayHintLabelPart:
-    """An inlay hint label part allows for interactive and composite labels of
-    inlay hints.
+    """An inlay hint label part allows for interactive and composite labels of inlay
+    hints.
 
     @since 3.17.0
     """
 
     # Since: 3.17.0
 
     value: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The value of this label part."""
 
     tooltip: Optional[Union[str, "MarkupContent"]] = attrs.field(default=None)
     """The tooltip text when you hover over this label part.
 
-    Depending on the client capability `inlayHint.resolveSupport`
-    clients might resolve this property late using the resolve request.
+    Depending on the client capability `inlayHint.resolveSupport` clients might resolve
+    this property late using the resolve request.
     """
 
     location: Optional[Location] = attrs.field(default=None)
     """An optional source code location that represents this label part.
 
     The editor will use this location for the hover and for code navigation
     features: This part will become a clickable link that resolves to the
@@ -5885,24 +5755,24 @@
     Depending on the client capability `inlayHint.resolveSupport` clients
     might resolve this property late using the resolve request.
     """
 
     command: Optional[Command] = attrs.field(default=None)
     """An optional command for this label part.
 
-    Depending on the client capability `inlayHint.resolveSupport`
-    clients might resolve this property late using the resolve request.
+    Depending on the client capability `inlayHint.resolveSupport` clients might resolve
+    this property late using the resolve request.
     """
 
 
 @attrs.define
 class MarkupContent:
-    """A `MarkupContent` literal represents a string value which content is
-    interpreted base on its kind flag. Currently the protocol supports
-    `plaintext` and `markdown` as markup kinds.
+    """A `MarkupContent` literal represents a string value which content is interpreted
+    base on its kind flag. Currently the protocol supports `plaintext` and `markdown` as
+    markup kinds.
 
     If the kind is `markdown` then the value can contain fenced code blocks like in GitHub issues.
     See https://help.github.com/articles/creating-and-highlighting-code-blocks/#syntax-highlighting
 
     Here is an example how such a string can be constructed using JavaScript / TypeScript:
     ```ts
     let markdown: MarkdownContent = {
@@ -5945,16 +5815,15 @@
 
     result_id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """An optional result id.
 
-    If provided it will be sent on the next diagnostic request for the
-    same document.
+    If provided it will be sent on the next diagnostic request for the same document.
     """
 
 
 @attrs.define
 class RelatedFullDocumentDiagnosticReport:
     """A full diagnostic report with a set of related documents.
 
@@ -5968,51 +5837,48 @@
 
     related_documents: Optional[
         Dict[
             str,
             Union[FullDocumentDiagnosticReport, "UnchangedDocumentDiagnosticReport"],
         ]
     ] = attrs.field(default=None)
-    """Diagnostics of related documents. This information is useful in
-    programming languages where code in a file A can generate diagnostics in a
-    file B which A depends on. An example of such a language is C/C++ where
-    marco definitions in a file a.cpp and result in errors in a header file
-    b.hpp.
+    """Diagnostics of related documents. This information is useful in programming
+    languages where code in a file A can generate diagnostics in a file B which A
+    depends on. An example of such a language is C/C++ where marco definitions in a file
+    a.cpp and result in errors in a header file b.hpp.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
     kind: str = attrs.field(validator=attrs.validators.in_(["full"]), default="full")
     """A full document diagnostic report."""
 
     result_id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """An optional result id.
 
-    If provided it will be sent on the next diagnostic request for the
-    same document.
+    If provided it will be sent on the next diagnostic request for the same document.
     """
 
 
 @attrs.define
 class UnchangedDocumentDiagnosticReport:
-    """A diagnostic report indicating that the last returned report is still
-    accurate.
+    """A diagnostic report indicating that the last returned report is still accurate.
 
     @since 3.17.0
     """
 
     # Since: 3.17.0
 
     result_id: str = attrs.field(validator=attrs.validators.instance_of(str))
-    """A result id which will be sent on the next diagnostic request for the
-    same document."""
+    """A result id which will be sent on the next diagnostic request for the same
+    document."""
 
     kind: str = attrs.field(
         validator=attrs.validators.in_(["unchanged"]), default="unchanged"
     )
     """A document diagnostic report indicating no changes to the last result.
 
     A server can only return `unchanged` if result ids are provided.
@@ -6025,27 +5891,26 @@
 
     @since 3.17.0
     """
 
     # Since: 3.17.0
 
     result_id: str = attrs.field(validator=attrs.validators.instance_of(str))
-    """A result id which will be sent on the next diagnostic request for the
-    same document."""
+    """A result id which will be sent on the next diagnostic request for the same
+    document."""
 
     related_documents: Optional[
         Dict[
             str, Union[FullDocumentDiagnosticReport, UnchangedDocumentDiagnosticReport]
         ]
     ] = attrs.field(default=None)
-    """Diagnostics of related documents. This information is useful in
-    programming languages where code in a file A can generate diagnostics in a
-    file B which A depends on. An example of such a language is C/C++ where
-    marco definitions in a file a.cpp and result in errors in a header file
-    b.hpp.
+    """Diagnostics of related documents. This information is useful in programming
+    languages where code in a file A can generate diagnostics in a file B which A
+    depends on. An example of such a language is C/C++ where marco definitions in a file
+    a.cpp and result in errors in a header file b.hpp.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
     kind: str = attrs.field(
         validator=attrs.validators.in_(["unchanged"]), default="unchanged"
@@ -6201,16 +6066,15 @@
 
     uri: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The notebook document's uri."""
 
 
 @attrs.define
 class Registration:
-    """General parameters to to register for an notification or to register a
-    provider."""
+    """General parameters to register for a notification or to register a provider."""
 
     id: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The id used to register the request.
 
     The id can be used to deregister the request again.
     """
 
@@ -6243,31 +6107,30 @@
     """The server supports workspace folder.
 
     @since 3.6.0
     """
     # Since: 3.6.0
 
     file_operations: Optional["FileOperationOptions"] = attrs.field(default=None)
-    """The server is interested in notifications/requests for operations on
-    files.
+    """The server is interested in notifications/requests for operations on files.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
 
 @attrs.define
 class ServerCapabilities:
     """Defines the capabilities provided by a language server."""
 
     position_encoding: Optional[Union[PositionEncodingKind, str]] = attrs.field(
         default=None
     )
-    """The position encoding the server picked from the encodings offered by
-    the client via the client capability `general.positionEncodings`.
+    """The position encoding the server picked from the encodings offered by the client
+    via the client capability `general.positionEncodings`.
 
     If the client didn't provide any position encodings the only valid
     value that a server can return is 'utf-16'.
 
     If omitted it defaults to 'utf-16'.
 
     @since 3.17.0
@@ -6275,16 +6138,16 @@
     # Since: 3.17.0
 
     text_document_sync: Optional[
         Union["TextDocumentSyncOptions", TextDocumentSyncKind]
     ] = attrs.field(default=None)
     """Defines how text documents are synced.
 
-    Is either a detailed structure defining each notification or for
-    backwards compatibility the TextDocumentSyncKind number.
+    Is either a detailed structure defining each notification or for backwards
+    compatibility the TextDocumentSyncKind number.
     """
 
     notebook_document_sync: Optional[
         Union["NotebookDocumentSyncOptions", "NotebookDocumentSyncRegistrationOptions"]
     ] = attrs.field(default=None)
     """Defines how notebook documents are synced.
 
@@ -6337,17 +6200,16 @@
     """The server provides document symbol support."""
 
     code_action_provider: Optional[Union[bool, CodeActionOptions]] = attrs.field(
         default=None
     )
     """The server provides code actions.
 
-    CodeActionOptions may only be specified if the client states that it
-    supports `codeActionLiteralSupport` in its initial `initialize`
-    request.
+    CodeActionOptions may only be specified if the client states that it supports
+    `codeActionLiteralSupport` in its initial `initialize` request.
     """
 
     code_lens_provider: Optional[CodeLensOptions] = attrs.field(default=None)
     """The server provides code lens."""
 
     document_link_provider: Optional[DocumentLinkOptions] = attrs.field(default=None)
     """The server provides document link support."""
@@ -6376,16 +6238,16 @@
         DocumentOnTypeFormattingOptions
     ] = attrs.field(default=None)
     """The server provides document formatting on typing."""
 
     rename_provider: Optional[Union[bool, RenameOptions]] = attrs.field(default=None)
     """The server provides rename support.
 
-    RenameOptions may only be specified if the client states that it
-    supports `prepareSupport` in its initial `initialize` request.
+    RenameOptions may only be specified if the client states that it supports
+    `prepareSupport` in its initial `initialize` request.
     """
 
     folding_range_provider: Optional[
         Union[bool, FoldingRangeOptions, FoldingRangeRegistrationOptions]
     ] = attrs.field(default=None)
     """The server provides folding provider support."""
 
@@ -6476,16 +6338,15 @@
 
     experimental: Optional[LSPAny] = attrs.field(default=None)
     """Experimental server capabilities."""
 
 
 @attrs.define
 class VersionedTextDocumentIdentifier:
-    """A text document identifier to denote a specific version of a text
-    document."""
+    """A text document identifier to denote a specific version of a text document."""
 
     version: int = attrs.field(validator=validators.integer_validator)
     """The version number of this document."""
 
     uri: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The text document's uri."""
 
@@ -6500,26 +6361,25 @@
     type: FileChangeType = attrs.field()
     """The change type."""
 
 
 @attrs.define
 class FileSystemWatcher:
     glob_pattern: GlobPattern = attrs.field()
-    """The glob pattern to watch. See {@link GlobPattern glob pattern} for more
-    detail.
+    """The glob pattern to watch. See {@link GlobPattern glob pattern} for more detail.
 
     @since 3.17.0 support for relative patterns.
     """
     # Since: 3.17.0 support for relative patterns.
 
     kind: Optional[Union[WatchKind, int]] = attrs.field(default=None)
     """The kind of events of interest.
 
-    If omitted it defaults to WatchKind.Create | WatchKind.Change |
-    WatchKind.Delete which is 7.
+    If omitted it defaults to WatchKind.Create | WatchKind.Change | WatchKind.Delete
+    which is 7.
     """
 
 
 @attrs.define
 class Diagnostic:
     """Represents a diagnostic, such as a compiler error or warning.
 
@@ -6534,24 +6394,24 @@
 
     It usually appears in the user interface
     """
 
     severity: Optional[DiagnosticSeverity] = attrs.field(default=None)
     """The diagnostic's severity.
 
-    Can be omitted. If omitted it is up to the client to interpret
-    diagnostics as error, warning, info or hint.
+    Can be omitted. If omitted it is up to the client to interpret diagnostics as error,
+    warning, info or hint.
     """
 
     code: Optional[Union[int, str]] = attrs.field(default=None)
     """The diagnostic's code, which usually appear in the user interface."""
 
     code_description: Optional["CodeDescription"] = attrs.field(default=None)
-    """An optional property to describe the error code. Requires the code field
-    (above) to be present/not null.
+    """An optional property to describe the error code. Requires the code field (above)
+    to be present/not null.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     source: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
@@ -6569,44 +6429,41 @@
     @since 3.15.0
     """
     # Since: 3.15.0
 
     related_information: Optional[List["DiagnosticRelatedInformation"]] = attrs.field(
         default=None
     )
-    """An array of related diagnostic information, e.g. when symbol-names
-    within a scope collide all definitions can be marked via this property."""
+    """An array of related diagnostic information, e.g. when symbol-names within a scope
+    collide all definitions can be marked via this property."""
 
     data: Optional[LSPAny] = attrs.field(default=None)
-    """A data entry field that is preserved between a
-    `textDocument/publishDiagnostics` notification and
-    `textDocument/codeAction` request.
+    """A data entry field that is preserved between a `textDocument/publishDiagnostics`
+    notification and `textDocument/codeAction` request.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
 
 @attrs.define
 class CompletionContext:
-    """Contains additional information about the context in which a completion
-    request is triggered."""
+    """Contains additional information about the context in which a completion request
+    is triggered."""
 
     trigger_kind: CompletionTriggerKind = attrs.field()
     """How the completion was triggered."""
 
     trigger_character: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """The trigger character (a single character) that has trigger code
-    complete.
+    """The trigger character (a single character) that has trigger code complete.
 
-    Is undefined if `triggerKind !==
-    CompletionTriggerKind.TriggerCharacter`
+    Is undefined if `triggerKind !== CompletionTriggerKind.TriggerCharacter`
     """
 
 
 @attrs.define
 class CompletionItemLabelDetails:
     """Additional details for a completion item label.
 
@@ -6615,17 +6472,16 @@
 
     # Since: 3.17.0
 
     detail: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
-    """An optional string which is rendered less prominently directly after.
-
-    {@link CompletionItem.label label}, without any spacing.
+    """An optional string which is rendered less prominently directly after {@link
+    CompletionItem.label label}, without any spacing.
 
     Should be used for function signatures and type annotations.
     """
 
     description: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
@@ -6654,58 +6510,56 @@
 
     replace: Range = attrs.field()
     """The range if the replace is requested."""
 
 
 @attrs.define
 class SignatureHelpContext:
-    """Additional information about the context in which a signature help
-    request was triggered.
+    """Additional information about the context in which a signature help request was
+    triggered.
 
     @since 3.15.0
     """
 
     # Since: 3.15.0
 
     trigger_kind: SignatureHelpTriggerKind = attrs.field()
     """Action that caused signature help to be triggered."""
 
     is_retrigger: bool = attrs.field(validator=attrs.validators.instance_of(bool))
     """`true` if signature help was already showing when it was triggered.
 
-    Retriggers occurs when the signature help is already active and can
-    be caused by actions such as typing a trigger character, a cursor
-    move, or document content changes.
+    Retriggers occurs when the signature help is already active and can be caused by
+    actions such as typing a trigger character, a cursor move, or document content
+    changes.
     """
 
     trigger_character: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """Character that caused signature help to be triggered.
 
-    This is undefined when `triggerKind !==
-    SignatureHelpTriggerKind.TriggerCharacter`
+    This is undefined when `triggerKind !== SignatureHelpTriggerKind.TriggerCharacter`
     """
 
     active_signature_help: Optional[SignatureHelp] = attrs.field(default=None)
     """The currently active `SignatureHelp`.
 
-    The `activeSignatureHelp` has its `SignatureHelp.activeSignature`
-    field updated based on the user navigating through available
-    signatures.
+    The `activeSignatureHelp` has its `SignatureHelp.activeSignature` field updated
+    based on the user navigating through available signatures.
     """
 
 
 @attrs.define
 class SignatureInformation:
     """Represents the signature of something callable.
 
-    A signature can have a label, like a function-name, a doc-comment,
-    and a set of parameters.
+    A signature can have a label, like a function-name, a doc-comment, and a set of
+    parameters.
     """
 
     label: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The label of this signature.
 
     Will be shown in the UI.
     """
@@ -6729,46 +6583,42 @@
     @since 3.16.0
     """
     # Since: 3.16.0
 
 
 @attrs.define
 class ReferenceContext:
-    """Value-object that contains additional information when requesting
-    references."""
+    """Value-object that contains additional information when requesting references."""
 
     include_declaration: bool = attrs.field(
         validator=attrs.validators.instance_of(bool)
     )
     """Include the declaration of the current symbol."""
 
 
 @attrs.define
 class CodeActionContext:
-    """Contains additional diagnostic information about the context in which a.
-
-    {@link CodeActionProvider.provideCodeActions code action} is run.
-    """
+    """Contains additional diagnostic information about the context in which a {@link
+    CodeActionProvider.provideCodeActions code action} is run."""
 
     diagnostics: List[Diagnostic] = attrs.field()
-    """An array of diagnostics known on the client side overlapping the range
-    provided to the `textDocument/codeAction` request.
+    """An array of diagnostics known on the client side overlapping the range provided
+    to the `textDocument/codeAction` request.
 
-    They are provided so that the server knows which errors are
-    currently presented to the user for the given range. There is no
-    guarantee that these accurately reflect the error state of the
-    resource. The primary parameter to compute code actions is the
-    provided range.
+    They are provided so that the server knows which errors are currently presented to
+    the user for the given range. There is no guarantee that these accurately reflect
+    the error state of the resource. The primary parameter to compute code actions is
+    the provided range.
     """
 
     only: Optional[List[Union[CodeActionKind, str]]] = attrs.field(default=None)
     """Requested kind of actions to return.
 
-    Actions not of this kind are filtered out by the client before being
-    shown. So servers can omit computing them.
+    Actions not of this kind are filtered out by the client before being shown. So
+    servers can omit computing them.
     """
 
     trigger_kind: Optional[CodeActionTriggerKind] = attrs.field(default=None)
     """The reason why code actions were requested.
 
     @since 3.17.0
     """
@@ -6827,28 +6677,27 @@
 
     token_modifiers: List[str] = attrs.field()
     """The token modifiers a server uses."""
 
 
 @attrs.define
 class OptionalVersionedTextDocumentIdentifier:
-    """A text document identifier to optionally denote a specific version of a
-    text document."""
+    """A text document identifier to optionally denote a specific version of a text
+    document."""
 
     uri: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The text document's uri."""
 
     version: Optional[Union[int, None]] = attrs.field(default=None)
     """The version number of this document.
 
-    If a versioned text document identifier is sent from the server to
-    the client and the file is not open in the editor (the server has
-    not received an open notification before) the server can send `null`
-    to indicate that the version is unknown and the content on disk is
-    the truth (as specified with document content ownership).
+    If a versioned text document identifier is sent from the server to the client and
+    the file is not open in the editor (the server has not received an open notification
+    before) the server can send `null` to indicate that the version is unknown and the
+    content on disk is the truth (as specified with document content ownership).
     """
 
 
 @attrs.define
 class AnnotatedTextEdit:
     """A special text edit with an additional change annotation.
 
@@ -6928,16 +6777,16 @@
         default=None,
     )
     """Ignore the operation if the file doesn't exist."""
 
 
 @attrs.define
 class FileOperationPattern:
-    """A pattern to describe in which file operation requests or notifications
-    the server is interested in receiving.
+    """A pattern to describe in which file operation requests or notifications the
+    server is interested in receiving.
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
 
     glob: str = attrs.field(validator=attrs.validators.instance_of(str))
@@ -6987,35 +6836,33 @@
 
     result_id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """An optional result id.
 
-    If provided it will be sent on the next diagnostic request for the
-    same document.
+    If provided it will be sent on the next diagnostic request for the same document.
     """
 
 
 @attrs.define
 class WorkspaceUnchangedDocumentDiagnosticReport:
-    """An unchanged document diagnostic report for a workspace diagnostic
-    result.
+    """An unchanged document diagnostic report for a workspace diagnostic result.
 
     @since 3.17.0
     """
 
     # Since: 3.17.0
 
     uri: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The URI for which diagnostic information is reported."""
 
     result_id: str = attrs.field(validator=attrs.validators.instance_of(str))
-    """A result id which will be sent on the next diagnostic request for the
-    same document."""
+    """A result id which will be sent on the next diagnostic request for the same
+    document."""
 
     version: Optional[Union[int, None]] = attrs.field(default=None)
     """The version number for which the diagnostics are reported.
 
     If the document is not marked as open `null` can be provided.
     """
 
@@ -7055,16 +6902,15 @@
 
     execution_summary: Optional["ExecutionSummary"] = attrs.field(default=None)
     """Additional execution summary information if supported by the client."""
 
 
 @attrs.define
 class NotebookCellArrayChange:
-    """A change describing how to move a `NotebookCell` array from state S to
-    S'.
+    """A change describing how to move a `NotebookCell` array from state S to S'.
 
     @since 3.17.0
     """
 
     # Since: 3.17.0
 
     start: int = attrs.field(validator=validators.uinteger_validator)
@@ -7160,16 +7006,16 @@
 class NotebookDocumentSyncOptionsNotebookSelectorType1CellsType:
     language: str = attrs.field(validator=attrs.validators.instance_of(str))
 
 
 @attrs.define
 class NotebookDocumentSyncOptionsNotebookSelectorType1:
     notebook: Union[str, NotebookDocumentFilter] = attrs.field()
-    """The notebook to be synced If a string value is provided it matches
-    against the notebook type.
+    """The notebook to be synced If a string value is provided it matches against the
+    notebook type.
 
     '*' matches every notebook.
     """
 
     cells: Optional[
         List["NotebookDocumentSyncOptionsNotebookSelectorType1CellsType"]
     ] = attrs.field(default=None)
@@ -7185,25 +7031,24 @@
 class NotebookDocumentSyncOptionsNotebookSelectorType2:
     cells: List[
         "NotebookDocumentSyncOptionsNotebookSelectorType2CellsType"
     ] = attrs.field()
     """The cells of the matching notebook to be synced."""
 
     notebook: Optional[Union[str, NotebookDocumentFilter]] = attrs.field(default=None)
-    """The notebook to be synced If a string value is provided it matches
-    against the notebook type.
+    """The notebook to be synced If a string value is provided it matches against the
+    notebook type.
 
     '*' matches every notebook.
     """
 
 
 @attrs.define
 class NotebookDocumentSyncOptions:
-    """Options specific to a notebook plus its cells to be synced to the
-    server.
+    """Options specific to a notebook plus its cells to be synced to the server.
 
     If a selector provides a notebook document
     filter but no cell selector all cells of a
     matching notebook document will be synced.
 
     If a selector provides no notebook document
     filter but only a cell selector all notebook
@@ -7237,16 +7082,16 @@
 class NotebookDocumentSyncRegistrationOptionsNotebookSelectorType1CellsType:
     language: str = attrs.field(validator=attrs.validators.instance_of(str))
 
 
 @attrs.define
 class NotebookDocumentSyncRegistrationOptionsNotebookSelectorType1:
     notebook: Union[str, NotebookDocumentFilter] = attrs.field()
-    """The notebook to be synced If a string value is provided it matches
-    against the notebook type.
+    """The notebook to be synced If a string value is provided it matches against the
+    notebook type.
 
     '*' matches every notebook.
     """
 
     cells: Optional[
         List["NotebookDocumentSyncRegistrationOptionsNotebookSelectorType1CellsType"]
     ] = attrs.field(default=None)
@@ -7262,16 +7107,16 @@
 class NotebookDocumentSyncRegistrationOptionsNotebookSelectorType2:
     cells: List[
         "NotebookDocumentSyncRegistrationOptionsNotebookSelectorType2CellsType"
     ] = attrs.field()
     """The cells of the matching notebook to be synced."""
 
     notebook: Optional[Union[str, NotebookDocumentFilter]] = attrs.field(default=None)
-    """The notebook to be synced If a string value is provided it matches
-    against the notebook type.
+    """The notebook to be synced If a string value is provided it matches against the
+    notebook type.
 
     '*' matches every notebook.
     """
 
 
 @attrs.define
 class NotebookDocumentSyncRegistrationOptions:
@@ -7301,35 +7146,32 @@
 
     id: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """The id used to register the request.
 
-    The id can be used to deregister the request again. See also
-    Registration#id.
+    The id can be used to deregister the request again. See also Registration#id.
     """
 
 
 @attrs.define
 class WorkspaceFoldersServerCapabilities:
     supported: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """The server has support for workspace folders."""
 
     change_notifications: Optional[Union[str, bool]] = attrs.field(default=None)
-    """Whether the server wants to receive workspace folder change
-    notifications.
+    """Whether the server wants to receive workspace folder change notifications.
 
-    If a string is provided the string is treated as an ID under which
-    the notification is registered on the client side. The ID can be
-    used to unregister for these events using the
-    `client/unregisterCapability` request.
+    If a string is provided the string is treated as an ID under which the notification
+    is registered on the client side. The ID can be used to unregister for these events
+    using the `client/unregisterCapability` request.
     """
 
 
 @attrs.define
 class FileOperationOptions:
     """Options for notifications/requests for user operations on files.
 
@@ -7347,16 +7189,15 @@
     did_rename: Optional[FileOperationRegistrationOptions] = attrs.field(default=None)
     """The server is interested in receiving didRenameFiles notifications."""
 
     will_rename: Optional[FileOperationRegistrationOptions] = attrs.field(default=None)
     """The server is interested in receiving willRenameFiles requests."""
 
     did_delete: Optional[FileOperationRegistrationOptions] = attrs.field(default=None)
-    """The server is interested in receiving didDeleteFiles file
-    notifications."""
+    """The server is interested in receiving didDeleteFiles file notifications."""
 
     will_delete: Optional[FileOperationRegistrationOptions] = attrs.field(default=None)
     """The server is interested in receiving willDeleteFiles file requests."""
 
 
 @attrs.define
 class CodeDescription:
@@ -7371,16 +7212,16 @@
     """An URI to open with more information about the diagnostic error."""
 
 
 @attrs.define
 class DiagnosticRelatedInformation:
     """Represents a related message and source code location for a diagnostic.
 
-    This should be used to point to code locations that cause or related
-    to a diagnostics, e.g when duplicating a symbol in a scope.
+    This should be used to point to code locations that cause or related to a
+    diagnostics, e.g when duplicating a symbol in a scope.
     """
 
     location: Location = attrs.field()
     """The location of this related diagnostic information."""
 
     message: str = attrs.field(validator=attrs.validators.instance_of(str))
     """The message of this related diagnostic information."""
@@ -7392,54 +7233,55 @@
 
     A parameter can have a label and a doc-comment.
     """
 
     label: Union[str, Tuple[int, int]] = attrs.field()
     """The label of this parameter information.
 
-    Either a string or an inclusive start and exclusive end offsets within its containing
-    signature label. (see SignatureInformation.label). The offsets are based on a UTF-16
-    string representation as `Position` and `Range` does.
-
-    *Note*: a label of type string should be a substring of its containing signature label.
-    Its intended use case is to highlight the parameter label part in the `SignatureInformation.label`.
+    Either a string or an inclusive start and exclusive end offsets within its
+    containing signature label. (see SignatureInformation.label). The offsets are based
+    on a UTF-16 string representation as `Position` and `Range` does.
+
+    *Note*: a label of type string should be a substring of its containing signature
+    label. Its intended use case is to highlight the parameter label part in the
+    `SignatureInformation.label`.
     """
 
     documentation: Optional[Union[str, MarkupContent]] = attrs.field(default=None)
     """The human-readable doc-comment of this parameter.
 
     Will be shown in the UI but can be omitted.
     """
 
 
 @attrs.define
 class NotebookCellTextDocumentFilter:
-    """A notebook cell text document filter denotes a cell text document by
-    different properties.
+    """A notebook cell text document filter denotes a cell text document by different
+    properties.
 
     @since 3.17.0
     """
 
     # Since: 3.17.0
 
     notebook: Union[str, NotebookDocumentFilter] = attrs.field()
     """A filter that matches against the notebook containing the notebook cell.
 
-    If a string value is provided it matches against the notebook type.
-    '*' matches every notebook.
+    If a string value is provided it matches against the notebook type. '*' matches
+    every notebook.
     """
 
     language: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)),
         default=None,
     )
     """A language id like `python`.
 
-    Will be matched against the language id of the notebook cell
-    document. '*' matches every language.
+    Will be matched against the language id of the notebook cell document. '*' matches
+    every language.
     """
 
 
 @attrs.define
 class FileOperationPatternOptions:
     """Matching options for the file operation pattern.
 
@@ -7454,16 +7296,16 @@
     )
     """The pattern should be matched ignoring casing."""
 
 
 @attrs.define
 class ExecutionSummary:
     execution_order: int = attrs.field(validator=validators.uinteger_validator)
-    """A strict monotonically increasing value indicating the execution order
-    of a cell inside a notebook."""
+    """A strict monotonically increasing value indicating the execution order of a cell
+    inside a notebook."""
 
     success: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether the execution was successful or not if known by the client."""
 
@@ -7472,33 +7314,31 @@
 class WorkspaceClientCapabilities:
     """Workspace specific client capabilities."""
 
     apply_edit: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The client supports applying batch edits to the workspace by supporting
-    the request 'workspace/applyEdit'."""
+    """The client supports applying batch edits to the workspace by supporting the
+    request 'workspace/applyEdit'."""
 
     workspace_edit: Optional["WorkspaceEditClientCapabilities"] = attrs.field(
         default=None
     )
     """Capabilities specific to `WorkspaceEdit`s."""
 
     did_change_configuration: Optional[
         "DidChangeConfigurationClientCapabilities"
     ] = attrs.field(default=None)
-    """Capabilities specific to the `workspace/didChangeConfiguration`
-    notification."""
+    """Capabilities specific to the `workspace/didChangeConfiguration` notification."""
 
     did_change_watched_files: Optional[
         "DidChangeWatchedFilesClientCapabilities"
     ] = attrs.field(default=None)
-    """Capabilities specific to the `workspace/didChangeWatchedFiles`
-    notification."""
+    """Capabilities specific to the `workspace/didChangeWatchedFiles` notification."""
 
     symbol: Optional["WorkspaceSymbolClientCapabilities"] = attrs.field(default=None)
     """Capabilities specific to the `workspace/symbol` request."""
 
     execute_command: Optional["ExecuteCommandClientCapabilities"] = attrs.field(
         default=None
     )
@@ -7523,16 +7363,15 @@
     @since 3.6.0
     """
     # Since: 3.6.0
 
     semantic_tokens: Optional[
         "SemanticTokensWorkspaceClientCapabilities"
     ] = attrs.field(default=None)
-    """Capabilities specific to the semantic token requests scoped to the
-    workspace.
+    """Capabilities specific to the semantic token requests scoped to the workspace.
 
     @since 3.16.0.
     """
     # Since: 3.16.0.
 
     code_lens: Optional["CodeLensWorkspaceClientCapabilities"] = attrs.field(
         default=None
@@ -7542,45 +7381,42 @@
     @since 3.16.0.
     """
     # Since: 3.16.0.
 
     file_operations: Optional["FileOperationClientCapabilities"] = attrs.field(
         default=None
     )
-    """The client has support for file notifications/requests for user
-    operations on files.
+    """The client has support for file notifications/requests for user operations on
+    files.
 
     Since 3.16.0
     """
 
     inline_value: Optional["InlineValueWorkspaceClientCapabilities"] = attrs.field(
         default=None
     )
-    """Capabilities specific to the inline values requests scoped to the
-    workspace.
+    """Capabilities specific to the inline values requests scoped to the workspace.
 
     @since 3.17.0.
     """
     # Since: 3.17.0.
 
     inlay_hint: Optional["InlayHintWorkspaceClientCapabilities"] = attrs.field(
         default=None
     )
-    """Capabilities specific to the inlay hint requests scoped to the
-    workspace.
+    """Capabilities specific to the inlay hint requests scoped to the workspace.
 
     @since 3.17.0.
     """
     # Since: 3.17.0.
 
     diagnostics: Optional["DiagnosticWorkspaceClientCapabilities"] = attrs.field(
         default=None
     )
-    """Capabilities specific to the diagnostic requests scoped to the
-    workspace.
+    """Capabilities specific to the diagnostic requests scoped to the workspace.
 
     @since 3.17.0.
     """
     # Since: 3.17.0.
 
 
 @attrs.define
@@ -7633,16 +7469,15 @@
 
     references: Optional["ReferenceClientCapabilities"] = attrs.field(default=None)
     """Capabilities specific to the `textDocument/references` request."""
 
     document_highlight: Optional["DocumentHighlightClientCapabilities"] = attrs.field(
         default=None
     )
-    """Capabilities specific to the `textDocument/documentHighlight`
-    request."""
+    """Capabilities specific to the `textDocument/documentHighlight` request."""
 
     document_symbol: Optional["DocumentSymbolClientCapabilities"] = attrs.field(
         default=None
     )
     """Capabilities specific to the `textDocument/documentSymbol` request."""
 
     code_action: Optional["CodeActionClientCapabilities"] = attrs.field(default=None)
@@ -7701,16 +7536,15 @@
     @since 3.15.0
     """
     # Since: 3.15.0
 
     publish_diagnostics: Optional["PublishDiagnosticsClientCapabilities"] = attrs.field(
         default=None
     )
-    """Capabilities specific to the `textDocument/publishDiagnostics`
-    notification."""
+    """Capabilities specific to the `textDocument/publishDiagnostics` notification."""
 
     call_hierarchy: Optional["CallHierarchyClientCapabilities"] = attrs.field(
         default=None
     )
     """Capabilities specific to the various call hierarchy requests.
 
     @since 3.16.0
@@ -7792,16 +7626,16 @@
 
 @attrs.define
 class WindowClientCapabilities:
     work_done_progress: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """It indicates whether the client supports server initiated progress using
-    the `window/workDoneProgress/create` request.
+    """It indicates whether the client supports server initiated progress using the
+    `window/workDoneProgress/create` request.
 
     The capability also controls Whether client supports handling
     of progress notifications. If set servers are allowed to report a
     `workDoneProgress` property in the request specific server
     capabilities.
 
     @since 3.15.0
@@ -7829,33 +7663,33 @@
 
 @attrs.define
 class GeneralClientCapabilitiesStaleRequestSupportType:
     cancel: bool = attrs.field(validator=attrs.validators.instance_of(bool))
     """The client will actively cancel the request."""
 
     retry_on_content_modified: List[str] = attrs.field()
-    """The list of requests for which the client will retry the request if it
-    receives a response with error code `ContentModified`"""
+    """The list of requests for which the client will retry the request if it receives a
+    response with error code `ContentModified`"""
 
 
 @attrs.define
 class GeneralClientCapabilities:
     """General client capabilities.
 
     @since 3.16.0
     """
 
     # Since: 3.16.0
 
     stale_request_support: Optional[
         "GeneralClientCapabilitiesStaleRequestSupportType"
     ] = attrs.field(default=None)
-    """Client capability that signals how the client handles stale requests
-    (e.g. a request for which the client will not process the response anymore
-    since the information is outdated).
+    """Client capability that signals how the client handles stale requests (e.g. a
+    request for which the client will not process the response anymore since the
+    information is outdated).
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
     regular_expressions: Optional["RegularExpressionsClientCapabilities"] = attrs.field(
         default=None
@@ -7872,17 +7706,17 @@
     @since 3.16.0
     """
     # Since: 3.16.0
 
     position_encodings: Optional[List[Union[PositionEncodingKind, str]]] = attrs.field(
         default=None
     )
-    """The position encodings supported by the client. Client and server have
-    to agree on the same position encoding to ensure that offsets (e.g.
-    character position in a line) are interpreted the same on both sides.
+    """The position encodings supported by the client. Client and server have to agree
+    on the same position encoding to ensure that offsets (e.g. character position in a
+    line) are interpreted the same on both sides.
 
     To keep the protocol backwards compatible the following applies: if
     the value 'utf-16' is missing from the array of position encodings
     servers can assume that the client supports UTF-16. UTF-16 is
     therefore a mandatory encoding.
 
     If omitted it defaults to ['utf-16'].
@@ -7895,85 +7729,83 @@
     @since 3.17.0
     """
     # Since: 3.17.0
 
 
 @attrs.define
 class RelativePattern:
-    """A relative pattern is a helper to construct glob patterns that are
-    matched relatively to a base URI. The common value for a `baseUri` is a
-    workspace folder root, but it can be another absolute URI as well.
+    """A relative pattern is a helper to construct glob patterns that are matched
+    relatively to a base URI. The common value for a `baseUri` is a workspace folder
+    root, but it can be another absolute URI as well.
 
     @since 3.17.0
     """
 
     # Since: 3.17.0
 
     base_uri: Union[WorkspaceFolder, str] = attrs.field()
-    """A workspace folder or a base URI to which this pattern will be matched
-    against relatively."""
+    """A workspace folder or a base URI to which this pattern will be matched against
+    relatively."""
 
     pattern: Pattern = attrs.field()
     """The actual glob pattern;"""
 
 
 @attrs.define
 class WorkspaceEditClientCapabilitiesChangeAnnotationSupportType:
     groups_on_label: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the client groups edits with equal labels into tree nodes, for
-    instance all edits labelled with "Changes in Strings" would be a tree
-    node."""
+    """Whether the client groups edits with equal labels into tree nodes, for instance
+    all edits labelled with "Changes in Strings" would be a tree node."""
 
 
 @attrs.define
 class WorkspaceEditClientCapabilities:
     document_changes: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """The client supports versioned document changes in `WorkspaceEdit`s."""
 
     resource_operations: Optional[List[ResourceOperationKind]] = attrs.field(
         default=None
     )
-    """The resource operations the client supports. Clients should at least
-    support 'create', 'rename' and 'delete' files and folders.
+    """The resource operations the client supports. Clients should at least support
+    'create', 'rename' and 'delete' files and folders.
 
     @since 3.13.0
     """
     # Since: 3.13.0
 
     failure_handling: Optional[FailureHandlingKind] = attrs.field(default=None)
-    """The failure handling strategy of a client if applying the workspace edit
-    fails.
+    """The failure handling strategy of a client if applying the workspace edit fails.
 
     @since 3.13.0
     """
     # Since: 3.13.0
 
     normalizes_line_endings: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the client normalizes line endings to the client specific
-    setting. If set to `true` the client will normalize line ending characters
-    in a workspace edit to the client-specified new line character.
+    """Whether the client normalizes line endings to the client specific setting. If set
+    to `true` the client will normalize line ending characters in a workspace edit to
+    the client-specified new line character.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     change_annotation_support: Optional[
         "WorkspaceEditClientCapabilitiesChangeAnnotationSupportType"
     ] = attrs.field(default=None)
-    """Whether the client in general supports change annotations on text edits,
-    create file, rename file and delete file changes.
+    """Whether the client in general supports change annotations on text edits, create
+    file, rename file and delete file changes.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
 
 @attrs.define
@@ -7989,40 +7821,39 @@
 class DidChangeWatchedFilesClientCapabilities:
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Did change watched files notification supports dynamic registration.
 
-    Please note that the current protocol doesn't support static
-    configuration for file changes from the server side.
+    Please note that the current protocol doesn't support static configuration for file
+    changes from the server side.
     """
 
     relative_pattern_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the client has support for {@link  RelativePattern relative
-    pattern} or not.
+    """Whether the client has support for {@link  RelativePattern relative pattern} or
+    not.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
 
 @attrs.define
 class WorkspaceSymbolClientCapabilitiesSymbolKindType:
     value_set: Optional[List[SymbolKind]] = attrs.field(default=None)
-    """The symbol kind values the client supports. When this property exists
-    the client also guarantees that it will handle values outside its set
-    gracefully and falls back to a default value when unknown.
-
-    If this property is not present the client only supports the symbol
-    kinds from `File` to `Array` as defined in the initial version of
-    the protocol.
+    """The symbol kind values the client supports. When this property exists the client
+    also guarantees that it will handle values outside its set gracefully and falls back
+    to a default value when unknown.
+
+    If this property is not present the client only supports the symbol kinds from
+    `File` to `Array` as defined in the initial version of the protocol.
     """
 
 
 @attrs.define
 class WorkspaceSymbolClientCapabilitiesTagSupportType:
     value_set: List[SymbolTag] = attrs.field()
     """The tags supported by the client."""
@@ -8046,33 +7877,31 @@
         default=None,
     )
     """Symbol request supports dynamic registration."""
 
     symbol_kind: Optional[
         "WorkspaceSymbolClientCapabilitiesSymbolKindType"
     ] = attrs.field(default=None)
-    """Specific capabilities for the `SymbolKind` in the `workspace/symbol`
-    request."""
+    """Specific capabilities for the `SymbolKind` in the `workspace/symbol` request."""
 
     tag_support: Optional[
         "WorkspaceSymbolClientCapabilitiesTagSupportType"
     ] = attrs.field(default=None)
-    """The client supports tags on `SymbolInformation`. Clients supporting tags
-    have to handle unknown tags gracefully.
+    """The client supports tags on `SymbolInformation`. Clients supporting tags have to
+    handle unknown tags gracefully.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     resolve_support: Optional[
         "WorkspaceSymbolClientCapabilitiesResolveSupportType"
     ] = attrs.field(default=None)
-    """The client support partial workspace symbols. The client will send the
-    request `workspaceSymbol/resolve` to the server to resolve additional
-    properties.
+    """The client support partial workspace symbols. The client will send the request
+    `workspaceSymbol/resolve` to the server to resolve additional properties.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
 
 @attrs.define
@@ -8092,48 +7921,47 @@
 
     # Since: 3.16.0
 
     refresh_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the client implementation supports a refresh request sent from
-    the server to the client.
+    """Whether the client implementation supports a refresh request sent from the server
+    to the client.
 
-    Note that this event is global and will force the client to refresh
-    all semantic tokens currently shown. It should be used with absolute
-    care and is useful for situation where a server for example detects
-    a project wide change that requires such a calculation.
+    Note that this event is global and will force the client to refresh all semantic
+    tokens currently shown. It should be used with absolute care and is useful for
+    situation where a server for example detects a project wide change that requires
+    such a calculation.
     """
 
 
 @attrs.define
 class CodeLensWorkspaceClientCapabilities:
     """@since 3.16.0"""
 
     # Since: 3.16.0
 
     refresh_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the client implementation supports a refresh request sent from
-    the server to the client.
+    """Whether the client implementation supports a refresh request sent from the server
+    to the client.
 
-    Note that this event is global and will force the client to refresh
-    all code lenses currently shown. It should be used with absolute
-    care and is useful for situation where a server for example detect a
-    project wide change that requires such a calculation.
+    Note that this event is global and will force the client to refresh all code lenses
+    currently shown. It should be used with absolute care and is useful for situation
+    where a server for example detect a project wide change that requires such a
+    calculation.
     """
 
 
 @attrs.define
 class FileOperationClientCapabilities:
-    """Capabilities relating to events from file operations by the user in the
-    client.
+    """Capabilities relating to events from file operations by the user in the client.
 
     These events do not come from the file system, they come from user operations
     like renaming a file in the UI.
 
     @since 3.16.0
     """
 
@@ -8192,21 +8020,21 @@
 
     # Since: 3.17.0
 
     refresh_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the client implementation supports a refresh request sent from
-    the server to the client.
+    """Whether the client implementation supports a refresh request sent from the server
+    to the client.
 
-    Note that this event is global and will force the client to refresh
-    all inline values currently shown. It should be used with absolute
-    care and is useful for situation where a server for example detects
-    a project wide change that requires such a calculation.
+    Note that this event is global and will force the client to refresh all inline
+    values currently shown. It should be used with absolute care and is useful for
+    situation where a server for example detects a project wide change that requires
+    such a calculation.
     """
 
 
 @attrs.define
 class InlayHintWorkspaceClientCapabilities:
     """Client workspace capabilities specific to inlay hints.
 
@@ -8215,21 +8043,21 @@
 
     # Since: 3.17.0
 
     refresh_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the client implementation supports a refresh request sent from
-    the server to the client.
+    """Whether the client implementation supports a refresh request sent from the server
+    to the client.
 
-    Note that this event is global and will force the client to refresh
-    all inlay hints currently shown. It should be used with absolute
-    care and is useful for situation where a server for example detects
-    a project wide change that requires such a calculation.
+    Note that this event is global and will force the client to refresh all inlay hints
+    currently shown. It should be used with absolute care and is useful for situation
+    where a server for example detects a project wide change that requires such a
+    calculation.
     """
 
 
 @attrs.define
 class DiagnosticWorkspaceClientCapabilities:
     """Workspace client capabilities specific to diagnostic pull requests.
 
@@ -8238,21 +8066,21 @@
 
     # Since: 3.17.0
 
     refresh_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the client implementation supports a refresh request sent from
-    the server to the client.
+    """Whether the client implementation supports a refresh request sent from the server
+    to the client.
 
-    Note that this event is global and will force the client to refresh
-    all pulled diagnostics currently shown. It should be used with
-    absolute care and is useful for situation where a server for example
-    detects a project wide change that requires such a calculation.
+    Note that this event is global and will force the client to refresh all pulled
+    diagnostics currently shown. It should be used with absolute care and is useful for
+    situation where a server for example detects a project wide change that requires
+    such a calculation.
     """
 
 
 @attrs.define
 class TextDocumentSyncClientCapabilities:
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -8267,16 +8095,15 @@
     """The client supports sending will save notifications."""
 
     will_save_wait_until: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """The client supports sending a will save request and waits for a response
-    providing text edits which will be applied to the document before it is
-    saved."""
+    providing text edits which will be applied to the document before it is saved."""
 
     did_save: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """The client supports did save notifications."""
 
@@ -8302,29 +8129,27 @@
 class CompletionClientCapabilitiesCompletionItemType:
     snippet_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Client supports snippets as insert text.
 
-    A snippet can define tab stops and placeholders with `$1`, `$2` and
-    `${3:foo}`. `$0` defines the final tab stop, it defaults to the end
-    of the snippet. Placeholders with equal identifiers are linked, that
-    is typing in one will update others too.
+    A snippet can define tab stops and placeholders with `$1`, `$2` and `${3:foo}`. `$0`
+    defines the final tab stop, it defaults to the end of the snippet. Placeholders with
+    equal identifiers are linked, that is typing in one will update others too.
     """
 
     commit_characters_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Client supports commit characters on a completion item."""
 
     documentation_format: Optional[List[MarkupKind]] = attrs.field(default=None)
-    """Client supports the following content formats for the documentation
-    property.
+    """Client supports the following content formats for the documentation property.
 
     The order describes the preferred format of the client.
     """
 
     deprecated_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
@@ -8336,50 +8161,49 @@
         default=None,
     )
     """Client supports the preselect property on a completion item."""
 
     tag_support: Optional[
         "CompletionClientCapabilitiesCompletionItemTypeTagSupportType"
     ] = attrs.field(default=None)
-    """Client supports the tag property on a completion item. Clients
-    supporting tags have to handle unknown tags gracefully. Clients especially
-    need to preserve unknown tags when sending a completion item back to the
-    server in a resolve call.
+    """Client supports the tag property on a completion item. Clients supporting tags
+    have to handle unknown tags gracefully. Clients especially need to preserve unknown
+    tags when sending a completion item back to the server in a resolve call.
 
     @since 3.15.0
     """
     # Since: 3.15.0
 
     insert_replace_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Client support insert replace edit to control different behavior if a
-    completion item is inserted in the text or should replace text.
+    """Client support insert replace edit to control different behavior if a completion
+    item is inserted in the text or should replace text.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     resolve_support: Optional[
         "CompletionClientCapabilitiesCompletionItemTypeResolveSupportType"
     ] = attrs.field(default=None)
-    """Indicates which properties a client can resolve lazily on a completion
-    item. Before version 3.16.0 only the predefined properties `documentation`
-    and `details` could be resolved lazily.
+    """Indicates which properties a client can resolve lazily on a completion item.
+    Before version 3.16.0 only the predefined properties `documentation` and `details`
+    could be resolved lazily.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     insert_text_mode_support: Optional[
         "CompletionClientCapabilitiesCompletionItemTypeInsertTextModeSupportType"
     ] = attrs.field(default=None)
-    """The client supports the `insertTextMode` property on a completion item
-    to override the whitespace handling mode as defined by the client (see
+    """The client supports the `insertTextMode` property on a completion item to
+    override the whitespace handling mode as defined by the client (see
     `insertTextMode`).
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     label_details_support: Optional[bool] = attrs.field(
@@ -8393,21 +8217,20 @@
     """
     # Since: 3.17.0
 
 
 @attrs.define
 class CompletionClientCapabilitiesCompletionItemKindType:
     value_set: Optional[List[CompletionItemKind]] = attrs.field(default=None)
-    """The completion item kind values the client supports. When this property
-    exists the client also guarantees that it will handle values outside its
-    set gracefully and falls back to a default value when unknown.
-
-    If this property is not present the client only supports the
-    completion items kinds from `Text` to `Reference` as defined in the
-    initial version of the protocol.
+    """The completion item kind values the client supports. When this property exists
+    the client also guarantees that it will handle values outside its set gracefully and
+    falls back to a default value when unknown.
+
+    If this property is not present the client only supports the completion items kinds
+    from `Text` to `Reference` as defined in the initial version of the protocol.
     """
 
 
 @attrs.define
 class CompletionClientCapabilitiesCompletionListType:
     item_defaults: Optional[List[str]] = attrs.field(default=None)
     """The client supports the following itemDefaults on a completion list.
@@ -8430,25 +8253,23 @@
         default=None,
     )
     """Whether completion supports dynamic registration."""
 
     completion_item: Optional[
         "CompletionClientCapabilitiesCompletionItemType"
     ] = attrs.field(default=None)
-    """The client supports the following `CompletionItem` specific
-    capabilities."""
+    """The client supports the following `CompletionItem` specific capabilities."""
 
     completion_item_kind: Optional[
         "CompletionClientCapabilitiesCompletionItemKindType"
     ] = attrs.field(default=None)
 
     insert_text_mode: Optional[InsertTextMode] = attrs.field(default=None)
-    """Defines how the client handles whitespace and indentation when accepting
-    a completion item that uses multi line text in either `insertText` or
-    `textEdit`.
+    """Defines how the client handles whitespace and indentation when accepting a
+    completion item that uses multi line text in either `insertText` or `textEdit`.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
     context_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -8456,16 +8277,15 @@
     )
     """The client supports to send additional context information for a
     `textDocument/completion` request."""
 
     completion_list: Optional[
         "CompletionClientCapabilitiesCompletionListType"
     ] = attrs.field(default=None)
-    """The client supports the following `CompletionList` specific
-    capabilities.
+    """The client supports the following `CompletionList` specific capabilities.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
 
 @attrs.define
@@ -8485,42 +8305,40 @@
 
 @attrs.define
 class SignatureHelpClientCapabilitiesSignatureInformationTypeParameterInformationType:
     label_offset_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The client supports processing label offsets instead of a simple label
-    string.
+    """The client supports processing label offsets instead of a simple label string.
 
     @since 3.14.0
     """
     # Since: 3.14.0
 
 
 @attrs.define
 class SignatureHelpClientCapabilitiesSignatureInformationType:
     documentation_format: Optional[List[MarkupKind]] = attrs.field(default=None)
-    """Client supports the following content formats for the documentation
-    property.
+    """Client supports the following content formats for the documentation property.
 
     The order describes the preferred format of the client.
     """
 
     parameter_information: Optional[
         "SignatureHelpClientCapabilitiesSignatureInformationTypeParameterInformationType"
     ] = attrs.field(default=None)
     """Client capabilities specific to parameter information."""
 
     active_parameter_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The client supports the `activeParameter` property on
-    `SignatureInformation` literal.
+    """The client supports the `activeParameter` property on `SignatureInformation`
+    literal.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
 
 @attrs.define
@@ -8532,25 +8350,23 @@
         default=None,
     )
     """Whether signature help supports dynamic registration."""
 
     signature_information: Optional[
         "SignatureHelpClientCapabilitiesSignatureInformationType"
     ] = attrs.field(default=None)
-    """The client supports the following `SignatureInformation` specific
-    properties."""
+    """The client supports the following `SignatureInformation` specific properties."""
 
     context_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """The client supports to send additional context information for a
-    `textDocument/signatureHelp` request. A client that opts into
-    contextSupport will also support the `retriggerCharacters` on
-    `SignatureHelpOptions`.
+    `textDocument/signatureHelp` request. A client that opts into contextSupport will
+    also support the `retriggerCharacters` on `SignatureHelpOptions`.
 
     @since 3.15.0
     """
     # Since: 3.15.0
 
 
 @attrs.define
@@ -8562,24 +8378,23 @@
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether declaration supports dynamic registration.
 
     If this is set to `true` the client supports the new
-    `DeclarationRegistrationOptions` return value for the corresponding
-    server capability as well.
+    `DeclarationRegistrationOptions` return value for the corresponding server
+    capability as well.
     """
 
     link_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The client supports additional metadata in the form of declaration
-    links."""
+    """The client supports additional metadata in the form of declaration links."""
 
 
 @attrs.define
 class DefinitionClientCapabilities:
     """Client Capabilities for a {@link DefinitionRequest}."""
 
     dynamic_registration: Optional[bool] = attrs.field(
@@ -8606,16 +8421,16 @@
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether implementation supports dynamic registration.
 
     If this is set to `true` the client supports the new
-    `TypeDefinitionRegistrationOptions` return value for the
-    corresponding server capability as well.
+    `TypeDefinitionRegistrationOptions` return value for the corresponding server
+    capability as well.
     """
 
     link_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """The client supports additional metadata in the form of definition links.
@@ -8633,16 +8448,16 @@
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether implementation supports dynamic registration.
 
     If this is set to `true` the client supports the new
-    `ImplementationRegistrationOptions` return value for the
-    corresponding server capability as well.
+    `ImplementationRegistrationOptions` return value for the corresponding server
+    capability as well.
     """
 
     link_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """The client supports additional metadata in the form of definition links.
@@ -8673,21 +8488,20 @@
     )
     """Whether document highlight supports dynamic registration."""
 
 
 @attrs.define
 class DocumentSymbolClientCapabilitiesSymbolKindType:
     value_set: Optional[List[SymbolKind]] = attrs.field(default=None)
-    """The symbol kind values the client supports. When this property exists
-    the client also guarantees that it will handle values outside its set
-    gracefully and falls back to a default value when unknown.
-
-    If this property is not present the client only supports the symbol
-    kinds from `File` to `Array` as defined in the initial version of
-    the protocol.
+    """The symbol kind values the client supports. When this property exists the client
+    also guarantees that it will handle values outside its set gracefully and falls back
+    to a default value when unknown.
+
+    If this property is not present the client only supports the symbol kinds from
+    `File` to `Array` as defined in the initial version of the protocol.
     """
 
 
 @attrs.define
 class DocumentSymbolClientCapabilitiesTagSupportType:
     value_set: List[SymbolTag] = attrs.field()
     """The tags supported by the client."""
@@ -8702,54 +8516,53 @@
         default=None,
     )
     """Whether document symbol supports dynamic registration."""
 
     symbol_kind: Optional[
         "DocumentSymbolClientCapabilitiesSymbolKindType"
     ] = attrs.field(default=None)
-    """Specific capabilities for the `SymbolKind` in the
-    `textDocument/documentSymbol` request."""
+    """Specific capabilities for the `SymbolKind` in the `textDocument/documentSymbol`
+    request."""
 
     hierarchical_document_symbol_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """The client supports hierarchical document symbols."""
 
     tag_support: Optional[
         "DocumentSymbolClientCapabilitiesTagSupportType"
     ] = attrs.field(default=None)
     """The client supports tags on `SymbolInformation`. Tags are supported on
-    `DocumentSymbol` if `hierarchicalDocumentSymbolSupport` is set to true.
-    Clients supporting tags have to handle unknown tags gracefully.
+    `DocumentSymbol` if `hierarchicalDocumentSymbolSupport` is set to true. Clients
+    supporting tags have to handle unknown tags gracefully.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     label_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The client supports an additional label presented in the UI when
-    registering a document symbol provider.
+    """The client supports an additional label presented in the UI when registering a
+    document symbol provider.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
 
 @attrs.define
 class CodeActionClientCapabilitiesCodeActionLiteralSupportTypeCodeActionKindType:
     value_set: List[Union[CodeActionKind, str]] = attrs.field()
     """The code action kind values the client supports.
 
-    When this property exists the client also guarantees that it will
-    handle values outside its set gracefully and falls back to a default
-    value when unknown.
+    When this property exists the client also guarantees that it will handle values
+    outside its set gracefully and falls back to a default value when unknown.
     """
 
 
 @attrs.define
 class CodeActionClientCapabilitiesCodeActionLiteralSupportType:
     code_action_kind: "CodeActionClientCapabilitiesCodeActionLiteralSupportTypeCodeActionKindType" = (
         attrs.field()
@@ -8772,17 +8585,17 @@
         default=None,
     )
     """Whether code action supports dynamic registration."""
 
     code_action_literal_support: Optional[
         "CodeActionClientCapabilitiesCodeActionLiteralSupportType"
     ] = attrs.field(default=None)
-    """The client support code action literals of type `CodeAction` as a valid
-    response of the `textDocument/codeAction` request. If the property is not
-    set the request can only return `Command` literals.
+    """The client support code action literals of type `CodeAction` as a valid response
+    of the `textDocument/codeAction` request. If the property is not set the request can
+    only return `Command` literals.
 
     @since 3.8.0
     """
     # Since: 3.8.0
 
     is_preferred_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -8804,39 +8617,38 @@
     """
     # Since: 3.16.0
 
     data_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether code action supports the `data` property which is preserved
-    between a `textDocument/codeAction` and a `codeAction/resolve` request.
+    """Whether code action supports the `data` property which is preserved between a
+    `textDocument/codeAction` and a `codeAction/resolve` request.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     resolve_support: Optional[
         "CodeActionClientCapabilitiesResolveSupportType"
     ] = attrs.field(default=None)
-    """Whether the client supports resolving additional code action properties
-    via a separate `codeAction/resolve` request.
+    """Whether the client supports resolving additional code action properties via a
+    separate `codeAction/resolve` request.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
     honors_change_annotations: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the client honors the change annotations in text edits and
-    resource operations returned via the `CodeAction#edit` property by for
-    example presenting the workspace edit in the user interface and asking for
-    confirmation.
+    """Whether the client honors the change annotations in text edits and resource
+    operations returned via the `CodeAction#edit` property by for example presenting the
+    workspace edit in the user interface and asking for confirmation.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
 
 @attrs.define
@@ -8876,16 +8688,16 @@
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether implementation supports dynamic registration.
 
     If this is set to `true` the client supports the new
-    `DocumentColorRegistrationOptions` return value for the
-    corresponding server capability as well.
+    `DocumentColorRegistrationOptions` return value for the corresponding server
+    capability as well.
     """
 
 
 @attrs.define
 class DocumentFormattingClientCapabilities:
     """Client capabilities of a {@link DocumentFormattingRequest}."""
 
@@ -8926,16 +8738,15 @@
     )
     """Whether rename supports dynamic registration."""
 
     prepare_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Client supports testing for validity of rename operations before
-    execution.
+    """Client supports testing for validity of rename operations before execution.
 
     @since 3.12.0
     """
     # Since: 3.12.0
 
     prepare_support_default_behavior: Optional[
         PrepareSupportDefaultBehavior
@@ -8949,80 +8760,77 @@
     """
     # Since: 3.16.0
 
     honors_change_annotations: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the client honors the change annotations in text edits and
-    resource operations returned via the rename request's workspace edit by for
-    example presenting the workspace edit in the user interface and asking for
-    confirmation.
+    """Whether the client honors the change annotations in text edits and resource
+    operations returned via the rename request's workspace edit by for example
+    presenting the workspace edit in the user interface and asking for confirmation.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
 
 @attrs.define
 class FoldingRangeClientCapabilitiesFoldingRangeKindType:
     value_set: Optional[List[Union[FoldingRangeKind, str]]] = attrs.field(default=None)
     """The folding range kind values the client supports.
 
-    When this property exists the client also guarantees that it will
-    handle values outside its set gracefully and falls back to a default
-    value when unknown.
+    When this property exists the client also guarantees that it will handle values
+    outside its set gracefully and falls back to a default value when unknown.
     """
 
 
 @attrs.define
 class FoldingRangeClientCapabilitiesFoldingRangeType:
     collapsed_text: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """If set, the client signals that it supports setting collapsedText on
-    folding ranges to display custom labels instead of the default text.
+    """If set, the client signals that it supports setting collapsedText on folding
+    ranges to display custom labels instead of the default text.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
 
 @attrs.define
 class FoldingRangeClientCapabilities:
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether implementation supports dynamic registration for folding range
-    providers.
+    """Whether implementation supports dynamic registration for folding range providers.
 
     If this is set to `true` the client supports the new
-    `FoldingRangeRegistrationOptions` return value for the corresponding
-    server capability as well.
+    `FoldingRangeRegistrationOptions` return value for the corresponding server
+    capability as well.
     """
 
     range_limit: Optional[int] = attrs.field(
         validator=attrs.validators.optional(validators.uinteger_validator), default=None
     )
-    """The maximum number of folding ranges that the client prefers to receive
-    per document.
+    """The maximum number of folding ranges that the client prefers to receive per
+    document.
 
     The value serves as a hint, servers are free to follow the limit.
     """
 
     line_folding_only: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """If set, the client signals that it only supports folding complete lines.
 
-    If set, client will ignore specified `startCharacter` and
-    `endCharacter` properties in a FoldingRange.
+    If set, client will ignore specified `startCharacter` and `endCharacter` properties
+    in a FoldingRange.
     """
 
     folding_range_kind: Optional[
         "FoldingRangeClientCapabilitiesFoldingRangeKindType"
     ] = attrs.field(default=None)
     """Specific options for the folding range kind.
 
@@ -9046,16 +8854,16 @@
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether implementation supports dynamic registration for selection range
     providers.
 
     If this is set to `true` the client supports the new
-    `SelectionRangeRegistrationOptions` return value for the
-    corresponding server capability as well.
+    `SelectionRangeRegistrationOptions` return value for the corresponding server
+    capability as well.
     """
 
 
 @attrs.define
 class PublishDiagnosticsClientCapabilitiesTagSupportType:
     value_set: List[DiagnosticTag] = attrs.field()
     """The tags supported by the client."""
@@ -9070,16 +8878,16 @@
         default=None,
     )
     """Whether the clients accepts diagnostics with related information."""
 
     tag_support: Optional[
         "PublishDiagnosticsClientCapabilitiesTagSupportType"
     ] = attrs.field(default=None)
-    """Client supports the tag property to provide meta data about a
-    diagnostic. Clients supporting tags have to handle unknown tags gracefully.
+    """Client supports the tag property to provide meta data about a diagnostic. Clients
+    supporting tags have to handle unknown tags gracefully.
 
     @since 3.15.0
     """
     # Since: 3.15.0
 
     version_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
@@ -9102,17 +8910,16 @@
     """
     # Since: 3.16.0
 
     data_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether code action supports the `data` property which is preserved
-    between a `textDocument/publishDiagnostics` and `textDocument/codeAction`
-    request.
+    """Whether code action supports the `data` property which is preserved between a
+    `textDocument/publishDiagnostics` and `textDocument/codeAction` request.
 
     @since 3.16.0
     """
     # Since: 3.16.0
 
 
 @attrs.define
@@ -9124,59 +8931,58 @@
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether implementation supports dynamic registration.
 
     If this is set to `true` the client supports the new
-    `(TextDocumentRegistrationOptions & StaticRegistrationOptions)`
-    return value for the corresponding server capability as well.
+    `(TextDocumentRegistrationOptions & StaticRegistrationOptions)` return value for the
+    corresponding server capability as well.
     """
 
 
 @attrs.define
 class SemanticTokensClientCapabilitiesRequestsTypeFullType1:
     delta: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """The client will send the `textDocument/semanticTokens/full/delta`
-    request if the server provides a corresponding handler."""
+    """The client will send the `textDocument/semanticTokens/full/delta` request if the
+    server provides a corresponding handler."""
 
 
 @attrs.define
 class SemanticTokensClientCapabilitiesRequestsType:
     range: Optional[Union[bool, Any]] = attrs.field(default=None)
-    """The client will send the `textDocument/semanticTokens/range` request if
-    the server provides a corresponding handler."""
+    """The client will send the `textDocument/semanticTokens/range` request if the
+    server provides a corresponding handler."""
 
     full: Optional[
         Union[bool, "SemanticTokensClientCapabilitiesRequestsTypeFullType1"]
     ] = attrs.field(default=None)
-    """The client will send the `textDocument/semanticTokens/full` request if
-    the server provides a corresponding handler."""
+    """The client will send the `textDocument/semanticTokens/full` request if the server
+    provides a corresponding handler."""
 
 
 @attrs.define
 class SemanticTokensClientCapabilities:
     """@since 3.16.0"""
 
     # Since: 3.16.0
 
     requests: "SemanticTokensClientCapabilitiesRequestsType" = attrs.field()
-    """Which requests the client supports and might send to the server
-    depending on the server's capability.
+    """Which requests the client supports and might send to the server depending on the
+    server's capability.
 
-    Please note that clients might not show semantic tokens or degrade
-    some of the user experience if a range or full request is advertised
-    by the client but not provided by the server. If for example the
-    client capability `requests.full` and `request.range` are both set
-    to true but the server only provides a range provider the client
-    might not render a minimap correctly or might even decide to not
-    show any semantic tokens at all.
+    Please note that clients might not show semantic tokens or degrade some of the user
+    experience if a range or full request is advertised by the client but not provided
+    by the server. If for example the client capability `requests.full` and
+    `request.range` are both set to true but the server only provides a range provider
+    the client might not render a minimap correctly or might even decide to not show any
+    semantic tokens at all.
     """
 
     token_types: List[str] = attrs.field()
     """The token types that the client supports."""
 
     token_modifiers: List[str] = attrs.field()
     """The token modifiers that the client supports."""
@@ -9187,16 +8993,16 @@
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether implementation supports dynamic registration.
 
     If this is set to `true` the client supports the new
-    `(TextDocumentRegistrationOptions & StaticRegistrationOptions)`
-    return value for the corresponding server capability as well.
+    `(TextDocumentRegistrationOptions & StaticRegistrationOptions)` return value for the
+    corresponding server capability as well.
     """
 
     overlapping_token_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether the client supports tokens that can overlap each other."""
@@ -9207,30 +9013,30 @@
     )
     """Whether the client supports tokens that can span multiple lines."""
 
     server_cancel_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the client allows the server to actively cancel a semantic token
-    request, e.g. supports returning LSPErrorCodes.ServerCancelled. If a server
-    does the client needs to retrigger the request.
+    """Whether the client allows the server to actively cancel a semantic token request,
+    e.g. supports returning LSPErrorCodes.ServerCancelled. If a server does the client
+    needs to retrigger the request.
 
     @since 3.17.0
     """
     # Since: 3.17.0
 
     augments_syntax_tokens: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the client uses semantic tokens to augment existing syntax
-    tokens. If set to `true` client side created syntax tokens and semantic
-    tokens are both used for colorization. If set to `false` the client only
-    uses the returned semantic tokens for colorization.
+    """Whether the client uses semantic tokens to augment existing syntax tokens. If set
+    to `true` client side created syntax tokens and semantic tokens are both used for
+    colorization. If set to `false` the client only uses the returned semantic tokens
+    for colorization.
 
     If the value is `undefined` then the client behavior is not
     specified.
 
     @since 3.17.0
     """
     # Since: 3.17.0
@@ -9248,16 +9054,16 @@
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether implementation supports dynamic registration.
 
     If this is set to `true` the client supports the new
-    `(TextDocumentRegistrationOptions & StaticRegistrationOptions)`
-    return value for the corresponding server capability as well.
+    `(TextDocumentRegistrationOptions & StaticRegistrationOptions)` return value for the
+    corresponding server capability as well.
     """
 
 
 @attrs.define
 class MonikerClientCapabilities:
     """Client capabilities specific to the moniker request.
 
@@ -9268,17 +9074,16 @@
 
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether moniker supports dynamic registration.
 
-    If this is set to `true` the client supports the new
-    `MonikerRegistrationOptions` return value for the corresponding
-    server capability as well.
+    If this is set to `true` the client supports the new `MonikerRegistrationOptions`
+    return value for the corresponding server capability as well.
     """
 
 
 @attrs.define
 class TypeHierarchyClientCapabilities:
     """@since 3.17.0"""
 
@@ -9287,16 +9092,16 @@
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether implementation supports dynamic registration.
 
     If this is set to `true` the client supports the new
-    `(TextDocumentRegistrationOptions & StaticRegistrationOptions)`
-    return value for the corresponding server capability as well.
+    `(TextDocumentRegistrationOptions & StaticRegistrationOptions)` return value for the
+    corresponding server capability as well.
     """
 
 
 @attrs.define
 class InlineValueClientCapabilities:
     """Client capabilities specific to inline values.
 
@@ -9333,16 +9138,15 @@
         default=None,
     )
     """Whether inlay hints support dynamic registration."""
 
     resolve_support: Optional[
         "InlayHintClientCapabilitiesResolveSupportType"
     ] = attrs.field(default=None)
-    """Indicates which properties a client can resolve lazily on an inlay
-    hint."""
+    """Indicates which properties a client can resolve lazily on an inlay hint."""
 
 
 @attrs.define
 class DiagnosticClientCapabilities:
     """Client capabilities specific to diagnostic pull requests.
 
     @since 3.17.0
@@ -9353,24 +9157,23 @@
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether implementation supports dynamic registration.
 
     If this is set to `true` the client supports the new
-    `(TextDocumentRegistrationOptions & StaticRegistrationOptions)`
-    return value for the corresponding server capability as well.
+    `(TextDocumentRegistrationOptions & StaticRegistrationOptions)` return value for the
+    corresponding server capability as well.
     """
 
     related_document_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the clients supports related documents for document diagnostic
-    pulls."""
+    """Whether the clients supports related documents for document diagnostic pulls."""
 
 
 @attrs.define
 class NotebookDocumentSyncClientCapabilities:
     """Notebook specific client capabilities.
 
     @since 3.17.0
@@ -9381,16 +9184,16 @@
     dynamic_registration: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """Whether implementation supports dynamic registration.
 
     If this is set to `true` the client supports the new
-    `(TextDocumentRegistrationOptions & StaticRegistrationOptions)`
-    return value for the corresponding server capability as well.
+    `(TextDocumentRegistrationOptions & StaticRegistrationOptions)` return value for the
+    corresponding server capability as well.
     """
 
     execution_summary_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
     """The client supports sending execution summary data per cell."""
@@ -9398,16 +9201,16 @@
 
 @attrs.define
 class ShowMessageRequestClientCapabilitiesMessageActionItemType:
     additional_properties_support: Optional[bool] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(bool)),
         default=None,
     )
-    """Whether the client supports additional attributes which are preserved
-    and send back to the server in the request's response."""
+    """Whether the client supports additional attributes which are preserved and send
+    back to the server in the request's response."""
 
 
 @attrs.define
 class ShowMessageRequestClientCapabilities:
     """Show message request client capabilities."""
 
     message_action_item: Optional[
@@ -9482,28 +9285,27 @@
     )
 
     document_selector: Optional[Union[DocumentSelector, None]] = attrs.field(
         default=None
     )
     """A document selector to identify the scope of the registration.
 
-    If set to null the document selector provided on the client side
-    will be used.
+    If set to null the document selector provided on the client side will be used.
     """
 
 
 @attrs.define
 class ResponseError:
     code: int = attrs.field(validator=validators.integer_validator)
     """A number indicating the error type that occurred."""
     message: str = attrs.field(validator=attrs.validators.instance_of(str))
     """A string providing a short description of the error."""
     data: Optional[LSPAny] = attrs.field(default=None)
-    """A primitive or structured value that contains additional information
-    about the error.
+    """A primitive or structured value that contains additional information about the
+    error.
 
     Can be omitted.
     """
 
 
 @attrs.define
 class ResponseErrorMessage:
@@ -9512,20 +9314,20 @@
     error: Optional[ResponseError] = attrs.field(default=None)
     """The error object in case a request fails."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentImplementationRequest:
-    """A request to resolve the implementation locations of a symbol at a given
-    text document position.
+    """A request to resolve the implementation locations of a symbol at a given text
+    document position.
 
     The request's parameter is of type [TextDocumentPositionParams]
-    (#TextDocumentPositionParams) the response is of type {@link
-    Definition} or a Thenable that resolves to such.
+    (#TextDocumentPositionParams) the response is of type {@link Definition} or a
+    Thenable that resolves to such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: ImplementationParams = attrs.field()
     method: str = "textDocument/implementation"
     """The method to be invoked."""
@@ -9538,20 +9340,20 @@
     """The request id."""
     result: Union[Definition, List[DefinitionLink], None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentTypeDefinitionRequest:
-    """A request to resolve the type definition locations of a symbol at a
-    given text document position.
+    """A request to resolve the type definition locations of a symbol at a given text
+    document position.
 
     The request's parameter is of type [TextDocumentPositionParams]
-    (#TextDocumentPositionParams) the response is of type {@link
-    Definition} or a Thenable that resolves to such.
+    (#TextDocumentPositionParams) the response is of type {@link Definition} or a
+    Thenable that resolves to such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: TypeDefinitionParams = attrs.field()
     method: str = "textDocument/typeDefinition"
     """The method to be invoked."""
@@ -9564,16 +9366,16 @@
     """The request id."""
     result: Union[Definition, List[DefinitionLink], None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WorkspaceWorkspaceFoldersRequest:
-    """The `workspace/workspaceFolders` is sent from the server to the client
-    to fetch the open workspace folders."""
+    """The `workspace/workspaceFolders` is sent from the server to the client to fetch
+    the open workspace folders."""
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: Optional[None] = attrs.field(default=None)
     method: str = "workspace/workspaceFolders"
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
@@ -9588,23 +9390,22 @@
 
 
 WorkspaceConfigurationParams = ConfigurationParams
 
 
 @attrs.define
 class WorkspaceConfigurationRequest:
-    """The 'workspace/configuration' request is sent from the server to the
-    client to fetch a certain configuration setting.
+    """The 'workspace/configuration' request is sent from the server to the client to
+    fetch a certain configuration setting.
 
-    This pull model replaces the old push model were the client signaled
-    configuration change via an event. If the server still needs to
-    react to configuration changes (since the server caches the result
-    of `workspace/configuration` requests) the server should register
-    for an empty configuration change event and empty the cache if such
-    an event is received.
+    This pull model replaces the old push model were the client signaled configuration
+    change via an event. If the server still needs to react to configuration changes
+    (since the server caches the result of `workspace/configuration` requests) the
+    server should register for an empty configuration change event and empty the cache
+    if such an event is received.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: WorkspaceConfigurationParams = attrs.field()
     method: str = "workspace/configuration"
     """The method to be invoked."""
@@ -9619,17 +9420,17 @@
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentDocumentColorRequest:
     """A request to list all color symbols found in a given text document.
 
-    The request's parameter is of type {@link DocumentColorParams} the
-    response is of type {@link ColorInformation ColorInformation[]} or a
-    Thenable that resolves to such.
+    The request's parameter is of type {@link DocumentColorParams} the response is of
+    type {@link ColorInformation ColorInformation[]} or a Thenable that resolves to
+    such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: DocumentColorParams = attrs.field()
     method: str = "textDocument/documentColor"
     """The method to be invoked."""
@@ -9644,17 +9445,17 @@
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentColorPresentationRequest:
     """A request to list all presentation for a color.
 
-    The request's parameter is of type {@link ColorPresentationParams}
-    the response is of type {@link ColorInformation ColorInformation[]}
-    or a Thenable that resolves to such.
+    The request's parameter is of type {@link ColorPresentationParams} the response is
+    of type {@link ColorInformation ColorInformation[]} or a Thenable that resolves to
+    such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: ColorPresentationParams = attrs.field()
     method: str = "textDocument/colorPresentation"
     """The method to be invoked."""
@@ -9669,17 +9470,16 @@
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentFoldingRangeRequest:
     """A request to provide folding ranges in a document.
 
-    The request's parameter is of type {@link FoldingRangeParams}, the
-    response is of type {@link FoldingRangeList} or a Thenable that
-    resolves to such.
+    The request's parameter is of type {@link FoldingRangeParams}, the response is of
+    type {@link FoldingRangeList} or a Thenable that resolves to such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: FoldingRangeParams = attrs.field()
     method: str = "textDocument/foldingRange"
     """The method to be invoked."""
@@ -9692,21 +9492,20 @@
     """The request id."""
     result: Union[List[FoldingRange], None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentDeclarationRequest:
-    """A request to resolve the type definition locations of a symbol at a
-    given text document position.
+    """A request to resolve the type definition locations of a symbol at a given text
+    document position.
 
     The request's parameter is of type [TextDocumentPositionParams]
-    (#TextDocumentPositionParams) the response is of type {@link
-    Declaration} or a typed array of {@link DeclarationLink} or a
-    Thenable that resolves to such.
+    (#TextDocumentPositionParams) the response is of type {@link Declaration} or a typed
+    array of {@link DeclarationLink} or a Thenable that resolves to such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: DeclarationParams = attrs.field()
     method: str = "textDocument/declaration"
     """The method to be invoked."""
@@ -9721,17 +9520,16 @@
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentSelectionRangeRequest:
     """A request to provide selection ranges in a document.
 
-    The request's parameter is of type {@link SelectionRangeParams}, the
-    response is of type {@link SelectionRange SelectionRange[]} or a
-    Thenable that resolves to such.
+    The request's parameter is of type {@link SelectionRangeParams}, the response is of
+    type {@link SelectionRange SelectionRange[]} or a Thenable that resolves to such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: SelectionRangeParams = attrs.field()
     method: str = "textDocument/selectionRange"
     """The method to be invoked."""
@@ -9744,16 +9542,16 @@
     """The request id."""
     result: Union[List[SelectionRange], None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WindowWorkDoneProgressCreateRequest:
-    """The `window/workDoneProgress/create` request is sent from the server to
-    the client to initiate progress reporting from the server."""
+    """The `window/workDoneProgress/create` request is sent from the server to the
+    client to initiate progress reporting from the server."""
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: WorkDoneProgressCreateParams = attrs.field()
     method: str = "window/workDoneProgress/create"
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
@@ -9765,17 +9563,16 @@
     """The request id."""
     result: None = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentPrepareCallHierarchyRequest:
-    """A request to result a `CallHierarchyItem` in a document at a given
-    position. Can be used as an input to an incoming or outgoing call
-    hierarchy.
+    """A request to result a `CallHierarchyItem` in a document at a given position. Can
+    be used as an input to an incoming or outgoing call hierarchy.
 
     @since 3.16.0
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: CallHierarchyPrepareParams = attrs.field()
@@ -9916,18 +9713,17 @@
     """The request id."""
     result: None = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WindowShowDocumentRequest:
-    """A request to show a document. This request might open an external
-    program depending on the value of the URI to open. For example a request to
-    open `https://code.visualstudio.com/` will very likely open the URI in a
-    WEB browser.
+    """A request to show a document. This request might open an external program
+    depending on the value of the URI to open. For example a request to open
+    `https://code.visualstudio.com/` will very likely open the URI in a WEB browser.
 
     @since 3.16.0
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: ShowDocumentParams = attrs.field()
@@ -9965,17 +9761,20 @@
     """The request id."""
     result: Union[LinkedEditingRanges, None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WorkspaceWillCreateFilesRequest:
-    """The will create files request is sent from the client to the server
-    before files are actually created as long as the creation is triggered from
-    within the client.
+    """The will create files request is sent from the client to the server before files
+    are actually created as long as the creation is triggered from within the client.
+
+    The request can return a `WorkspaceEdit` which will be applied to workspace before the
+    files are created. Hence the `WorkspaceEdit` can not manipulate the content of the file
+    to be created.
 
     @since 3.16.0
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: CreateFilesParams = attrs.field()
@@ -9990,17 +9789,16 @@
     """The request id."""
     result: Union[WorkspaceEdit, None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WorkspaceWillRenameFilesRequest:
-    """The will rename files request is sent from the client to the server
-    before files are actually renamed as long as the rename is triggered from
-    within the client.
+    """The will rename files request is sent from the client to the server before files
+    are actually renamed as long as the rename is triggered from within the client.
 
     @since 3.16.0
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: RenameFilesParams = attrs.field()
@@ -10015,16 +9813,16 @@
     """The request id."""
     result: Union[WorkspaceEdit, None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WorkspaceWillDeleteFilesRequest:
-    """The did delete files notification is sent from the client to the server
-    when files were deleted from within the client.
+    """The did delete files notification is sent from the client to the server when
+    files were deleted from within the client.
 
     @since 3.16.0
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: DeleteFilesParams = attrs.field()
@@ -10039,19 +9837,18 @@
     """The request id."""
     result: Union[WorkspaceEdit, None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentMonikerRequest:
-    """A request to get the moniker of a symbol at a given text document
-    position.
+    """A request to get the moniker of a symbol at a given text document position.
 
-    The request parameter is of type {@link TextDocumentPositionParams}.
-    The response is of type {@link Moniker Moniker[]} or `null`.
+    The request parameter is of type {@link TextDocumentPositionParams}. The response is
+    of type {@link Moniker Moniker[]} or `null`.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: MonikerParams = attrs.field()
     method: str = "textDocument/moniker"
     """The method to be invoked."""
@@ -10064,17 +9861,16 @@
     """The request id."""
     result: Union[List[Moniker], None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentPrepareTypeHierarchyRequest:
-    """A request to result a `TypeHierarchyItem` in a document at a given
-    position. Can be used as an input to a subtypes or supertypes type
-    hierarchy.
+    """A request to result a `TypeHierarchyItem` in a document at a given position. Can
+    be used as an input to a subtypes or supertypes type hierarchy.
 
     @since 3.17.0
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: TypeHierarchyPrepareParams = attrs.field()
@@ -10135,18 +9931,17 @@
     """The request id."""
     result: Union[List[TypeHierarchyItem], None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentInlineValueRequest:
-    """A request to provide inline values in a document. The request's
-    parameter is of type {@link InlineValueParams}, the response is of type.
-
-    {@link InlineValue InlineValue[]} or a Thenable that resolves to such.
+    """A request to provide inline values in a document. The request's parameter is of
+    type {@link InlineValueParams}, the response is of type {@link InlineValue
+    InlineValue[]} or a Thenable that resolves to such.
 
     @since 3.17.0
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: InlineValueParams = attrs.field()
@@ -10181,18 +9976,17 @@
     """The request id."""
     result: None = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentInlayHintRequest:
-    """A request to provide inlay hints in a document. The request's parameter
-    is of type {@link InlayHintsParams}, the response is of type.
-
-    {@link InlayHint InlayHint[]} or a Thenable that resolves to such.
+    """A request to provide inlay hints in a document. The request's parameter is of
+    type {@link InlayHintsParams}, the response is of type {@link InlayHint InlayHint[]}
+    or a Thenable that resolves to such.
 
     @since 3.17.0
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: InlayHintParams = attrs.field()
@@ -10207,18 +10001,17 @@
     """The request id."""
     result: Union[List[InlayHint], None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class InlayHintResolveRequest:
-    """A request to resolve additional properties for an inlay hint. The
-    request's parameter is of type {@link InlayHint}, the response is of type.
-
-    {@link InlayHint} or a Thenable that resolves to such.
+    """A request to resolve additional properties for an inlay hint. The request's
+    parameter is of type {@link InlayHint}, the response is of type {@link InlayHint} or
+    a Thenable that resolves to such.
 
     @since 3.17.0
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: InlayHint = attrs.field()
@@ -10322,16 +10115,16 @@
     """The request id."""
     result: None = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class ClientRegisterCapabilityRequest:
-    """The `client/registerCapability` request is sent from the server to the
-    client to register a new capability handler on the client side."""
+    """The `client/registerCapability` request is sent from the server to the client to
+    register a new capability handler on the client side."""
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: RegistrationParams = attrs.field()
     method: str = "client/registerCapability"
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
@@ -10343,17 +10136,16 @@
     """The request id."""
     result: None = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class ClientUnregisterCapabilityRequest:
-    """The `client/unregisterCapability` request is sent from the server to the
-    client to unregister a previously registered capability handler on the
-    client side."""
+    """The `client/unregisterCapability` request is sent from the server to the client
+    to unregister a previously registered capability handler on the client side."""
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: UnregistrationParams = attrs.field()
     method: str = "client/unregisterCapability"
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
@@ -10367,18 +10159,17 @@
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class InitializeRequest:
     """The initialize request is sent from the client to the server.
 
-    It is sent once as the request after starting up the server. The
-    requests parameter is of type {@link InitializeParams} the response
-    if of type {@link InitializeResult} of a Thenable that resolves to
-    such.
+    It is sent once as the request after starting up the server. The requests parameter
+    is of type {@link InitializeParams} the response if of type {@link InitializeResult}
+    of a Thenable that resolves to such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: InitializeParams = attrs.field()
     method: str = "initialize"
     """The method to be invoked."""
@@ -10393,17 +10184,16 @@
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class ShutdownRequest:
     """A shutdown request is sent from the client to the server.
 
-    It is sent once when the client decides to shutdown the server. The
-    only notification that is sent after a shutdown request is the exit
-    event.
+    It is sent once when the client decides to shutdown the server. The only
+    notification that is sent after a shutdown request is the exit event.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: Optional[None] = attrs.field(default=None)
     method: str = "shutdown"
     """The method to be invoked."""
@@ -10416,16 +10206,16 @@
     """The request id."""
     result: None = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WindowShowMessageRequestRequest:
-    """The show message request is sent from the server to the client to show a
-    message and a set of options actions to the user."""
+    """The show message request is sent from the server to the client to show a message
+    and a set of options actions to the user."""
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: ShowMessageRequestParams = attrs.field()
     method: str = "window/showMessageRequest"
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
@@ -10437,22 +10227,21 @@
     """The request id."""
     result: Union[MessageActionItem, None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentWillSaveWaitUntilRequest:
-    """A document will save request is sent from the client to the server
-    before the document is actually saved.
+    """A document will save request is sent from the client to the server before the
+    document is actually saved.
 
-    The request can return an array of TextEdits which will be applied
-    to the text document before it is saved. Please note that clients
-    might drop results if computing the text edits took too long or if a
-    server constantly fails on this request. This is done to keep the
-    save fast and reliable.
+    The request can return an array of TextEdits which will be applied to the text
+    document before it is saved. Please note that clients might drop results if
+    computing the text edits took too long or if a server constantly fails on this
+    request. This is done to keep the save fast and reliable.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: WillSaveTextDocumentParams = attrs.field()
     method: str = "textDocument/willSaveWaitUntil"
     """The method to be invoked."""
@@ -10465,26 +10254,24 @@
     """The request id."""
     result: Union[List[TextEdit], None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentCompletionRequest:
-    """Request to request completion at a given text document position. The
-    request's parameter is of type {@link TextDocumentPosition} the response is
-    of type {@link CompletionItem CompletionItem[]} or {@link CompletionList}
-    or a Thenable that resolves to such.
+    """Request to request completion at a given text document position. The request's
+    parameter is of type {@link TextDocumentPosition} the response is of type {@link
+    CompletionItem CompletionItem[]} or {@link CompletionList} or a Thenable that
+    resolves to such.
 
-    The request can delay the computation of the {@link
-    CompletionItem.detail `detail`} and {@link
-    CompletionItem.documentation `documentation`} properties to the
-    `completionItem/resolve` request. However, properties that are
-    needed for the initial sorting and filtering, like `sortText`,
-    `filterText`, `insertText`, and `textEdit`, must not be changed
-    during resolve.
+    The request can delay the computation of the {@link CompletionItem.detail `detail`}
+    and {@link CompletionItem.documentation `documentation`} properties to the
+    `completionItem/resolve` request. However, properties that are needed for the
+    initial sorting and filtering, like `sortText`, `filterText`, `insertText`, and
+    `textEdit`, must not be changed during resolve.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: CompletionParams = attrs.field()
     method: str = "textDocument/completion"
     """The method to be invoked."""
@@ -10499,17 +10286,17 @@
         default=None
     )
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class CompletionItemResolveRequest:
-    """Request to resolve additional information for a given completion
-    item.The request's parameter is of type {@link CompletionItem} the response
-    is of type {@link CompletionItem} or a Thenable that resolves to such."""
+    """Request to resolve additional information for a given completion item.The
+    request's parameter is of type {@link CompletionItem} the response is of type {@link
+    CompletionItem} or a Thenable that resolves to such."""
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: CompletionItem = attrs.field()
     method: str = "completionItem/resolve"
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
@@ -10523,17 +10310,16 @@
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentHoverRequest:
     """Request to request hover information at a given text document position.
 
-    The request's parameter is of type {@link TextDocumentPosition} the
-    response is of type {@link Hover} or a Thenable that resolves to
-    such.
+    The request's parameter is of type {@link TextDocumentPosition} the response is of
+    type {@link Hover} or a Thenable that resolves to such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: HoverParams = attrs.field()
     method: str = "textDocument/hover"
     """The method to be invoked."""
@@ -10564,21 +10350,20 @@
     """The request id."""
     result: Union[SignatureHelp, None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentDefinitionRequest:
-    """A request to resolve the definition location of a symbol at a given text
-    document position.
+    """A request to resolve the definition location of a symbol at a given text document
+    position.
 
-    The request's parameter is of type [TextDocumentPosition]
-    (#TextDocumentPosition) the response is of either type {@link
-    Definition} or a typed array of {@link DefinitionLink} or a Thenable
-    that resolves to such.
+    The request's parameter is of type [TextDocumentPosition] (#TextDocumentPosition)
+    the response is of either type {@link Definition} or a typed array of {@link
+    DefinitionLink} or a Thenable that resolves to such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: DefinitionParams = attrs.field()
     method: str = "textDocument/definition"
     """The method to be invoked."""
@@ -10591,18 +10376,18 @@
     """The request id."""
     result: Union[Definition, List[DefinitionLink], None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentReferencesRequest:
-    """A request to resolve project-wide references for the symbol denoted by
-    the given text document position. The request's parameter is of type {@link
-    ReferenceParams} the response is of type.
+    """A request to resolve project-wide references for the symbol denoted by the given
+    text document position.
 
+    The request's parameter is of type {@link ReferenceParams} the response is of type
     {@link Location Location[]} or a Thenable that resolves to such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: ReferenceParams = attrs.field()
     method: str = "textDocument/references"
@@ -10619,18 +10404,17 @@
 
 
 @attrs.define
 class TextDocumentDocumentHighlightRequest:
     """Request to resolve a {@link DocumentHighlight} for a given text document
     position.
 
-    The request's parameter is of type [TextDocumentPosition]
-    (#TextDocumentPosition) the request response is of type
-    [DocumentHighlight[]] (#DocumentHighlight) or a Thenable that
-    resolves to such.
+    The request's parameter is of type [TextDocumentPosition] (#TextDocumentPosition)
+    the request response is of type [DocumentHighlight[]] (#DocumentHighlight) or a
+    Thenable that resolves to such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: DocumentHighlightParams = attrs.field()
     method: str = "textDocument/documentHighlight"
     """The method to be invoked."""
@@ -10645,17 +10429,17 @@
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentDocumentSymbolRequest:
     """A request to list all symbols found in a given text document.
 
-    The request's parameter is of type {@link TextDocumentIdentifier}
-    the response is of type {@link SymbolInformation
-    SymbolInformation[]} or a Thenable that resolves to such.
+    The request's parameter is of type {@link TextDocumentIdentifier} the response is of
+    type {@link SymbolInformation SymbolInformation[]} or a Thenable that resolves to
+    such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: DocumentSymbolParams = attrs.field()
     method: str = "textDocument/documentSymbol"
     """The method to be invoked."""
@@ -10690,19 +10474,17 @@
     """The request id."""
     result: Union[List[Union[Command, CodeAction]], None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class CodeActionResolveRequest:
-    """Request to resolve additional information for a given code action.The
-    request's parameter is of type {@link CodeAction} the response is of type.
-
-    {@link CodeAction} or a Thenable that resolves to such.
-    """
+    """Request to resolve additional information for a given code action.The request's
+    parameter is of type {@link CodeAction} the response is of type {@link CodeAction}
+    or a Thenable that resolves to such."""
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: CodeAction = attrs.field()
     method: str = "codeAction/resolve"
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
@@ -10714,17 +10496,17 @@
     """The request id."""
     result: CodeAction = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WorkspaceSymbolRequest:
-    """A request to list project-wide symbols matching the query string given
-    by the {@link WorkspaceSymbolParams}. The response is of type {@link
-    SymbolInformation SymbolInformation[]} or a Thenable that resolves to such.
+    """A request to list project-wide symbols matching the query string given by the
+    {@link WorkspaceSymbolParams}. The response is of type {@link SymbolInformation
+    SymbolInformation[]} or a Thenable that resolves to such.
 
     @since 3.17.0 - support for WorkspaceSymbol in the returned data. Clients
      need to advertise support for WorkspaceSymbols via the client capability
      `workspace.symbol.resolveSupport`.
     """
 
     id: Union[int, str] = attrs.field()
@@ -10851,16 +10633,16 @@
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class DocumentLinkResolveRequest:
     """Request to resolve additional information for a given document link.
 
-    The request's parameter is of type {@link DocumentLink} the response
-    is of type {@link DocumentLink} or a Thenable that resolves to such.
+    The request's parameter is of type {@link DocumentLink} the response is of type
+    {@link DocumentLink} or a Thenable that resolves to such.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: DocumentLink = attrs.field()
     method: str = "documentLink/resolve"
     """The method to be invoked."""
@@ -10873,15 +10655,15 @@
     """The request id."""
     result: DocumentLink = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentFormattingRequest:
-    """A request to to format a whole document."""
+    """A request to format a whole document."""
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: DocumentFormattingParams = attrs.field()
     method: str = "textDocument/formatting"
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
@@ -10893,15 +10675,15 @@
     """The request id."""
     result: Union[List[TextEdit], None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentRangeFormattingRequest:
-    """A request to to format a range in a document."""
+    """A request to format a range in a document."""
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: DocumentRangeFormattingParams = attrs.field()
     method: str = "textDocument/rangeFormatting"
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
@@ -10978,16 +10760,16 @@
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WorkspaceExecuteCommandRequest:
     """A request send from the client to the server to execute a command.
 
-    The request might return a workspace edit which the client will
-    apply to the workspace.
+    The request might return a workspace edit which the client will apply to the
+    workspace.
     """
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: ExecuteCommandParams = attrs.field()
     method: str = "workspace/executeCommand"
     """The method to be invoked."""
@@ -11000,16 +10782,15 @@
     """The request id."""
     result: Union[LSPAny, None] = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WorkspaceApplyEditRequest:
-    """A request sent from the server to the client to modified certain
-    resources."""
+    """A request sent from the server to the client to modified certain resources."""
 
     id: Union[int, str] = attrs.field()
     """The request id."""
     params: ApplyWorkspaceEditParams = attrs.field()
     method: str = "workspace/applyEdit"
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
@@ -11021,44 +10802,44 @@
     """The request id."""
     result: ApplyWorkspaceEditResult = attrs.field(default=None)
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WorkspaceDidChangeWorkspaceFoldersNotification:
-    """The `workspace/didChangeWorkspaceFolders` notification is sent from the
-    client to the server when the workspace folder configuration changes."""
+    """The `workspace/didChangeWorkspaceFolders` notification is sent from the client to
+    the server when the workspace folder configuration changes."""
 
     params: DidChangeWorkspaceFoldersParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["workspace/didChangeWorkspaceFolders"]),
         default="workspace/didChangeWorkspaceFolders",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WindowWorkDoneProgressCancelNotification:
-    """The `window/workDoneProgress/cancel` notification is sent from  the
-    client to the server to cancel a progress initiated on the server side."""
+    """The `window/workDoneProgress/cancel` notification is sent from  the client to the
+    server to cancel a progress initiated on the server side."""
 
     params: WorkDoneProgressCancelParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["window/workDoneProgress/cancel"]),
         default="window/workDoneProgress/cancel",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WorkspaceDidCreateFilesNotification:
-    """The did create files notification is sent from the client to the server
-    when files were created from within the client.
+    """The did create files notification is sent from the client to the server when
+    files were created from within the client.
 
     @since 3.16.0
     """
 
     params: CreateFilesParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["workspace/didCreateFiles"]),
@@ -11066,16 +10847,16 @@
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WorkspaceDidRenameFilesNotification:
-    """The did rename files notification is sent from the client to the server
-    when files were renamed from within the client.
+    """The did rename files notification is sent from the client to the server when
+    files were renamed from within the client.
 
     @since 3.16.0
     """
 
     params: RenameFilesParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["workspace/didRenameFiles"]),
@@ -11083,17 +10864,16 @@
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WorkspaceDidDeleteFilesNotification:
-    """The will delete files request is sent from the client to the server
-    before files are actually deleted as long as the deletion is triggered from
-    within the client.
+    """The will delete files request is sent from the client to the server before files
+    are actually deleted as long as the deletion is triggered from within the client.
 
     @since 3.16.0
     """
 
     params: DeleteFilesParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["workspace/didDeleteFiles"]),
@@ -11160,206 +10940,204 @@
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class InitializedNotification:
-    """The initialized notification is sent from the client to the server after
-    the client is fully initialized and the server is allowed to send requests
-    from the server to the client."""
+    """The initialized notification is sent from the client to the server after the
+    client is fully initialized and the server is allowed to send requests from the
+    server to the client."""
 
     params: InitializedParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["initialized"]),
         default="initialized",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class ExitNotification:
-    """The exit event is sent from the client to the server to ask the server
-    to exit its process."""
+    """The exit event is sent from the client to the server to ask the server to exit
+    its process."""
 
     params: Optional[None] = attrs.field(default=None)
     method: str = attrs.field(
         validator=attrs.validators.in_(["exit"]),
         default="exit",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WorkspaceDidChangeConfigurationNotification:
-    """The configuration change notification is sent from the client to the
-    server when the client's configuration has changed.
+    """The configuration change notification is sent from the client to the server when
+    the client's configuration has changed.
 
-    The notification contains the changed configuration as defined by
-    the language client.
+    The notification contains the changed configuration as defined by the language
+    client.
     """
 
     params: DidChangeConfigurationParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["workspace/didChangeConfiguration"]),
         default="workspace/didChangeConfiguration",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WindowShowMessageNotification:
-    """The show message notification is sent from a server to a client to ask
-    the client to display a particular message in the user interface."""
+    """The show message notification is sent from a server to a client to ask the client
+    to display a particular message in the user interface."""
 
     params: ShowMessageParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["window/showMessage"]),
         default="window/showMessage",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WindowLogMessageNotification:
-    """The log message notification is sent from the server to the client to
-    ask the client to log a particular message."""
+    """The log message notification is sent from the server to the client to ask the
+    client to log a particular message."""
 
     params: LogMessageParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["window/logMessage"]),
         default="window/logMessage",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TelemetryEventNotification:
-    """The telemetry event notification is sent from the server to the client
-    to ask the client to log telemetry data."""
+    """The telemetry event notification is sent from the server to the client to ask the
+    client to log telemetry data."""
 
     params: LSPAny = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["telemetry/event"]),
         default="telemetry/event",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentDidOpenNotification:
-    """The document open notification is sent from the client to the server to
-    signal newly opened text documents.
+    """The document open notification is sent from the client to the server to signal
+    newly opened text documents.
 
-    The document's truth is now managed by the client and the server
-    must not try to read the document's truth using the document's uri.
-    Open in this sense means it is managed by the client. It doesn't
-    necessarily mean that its content is presented in an editor. An open
-    notification must not be sent more than once without a corresponding
-    close notification send before. This means open and close
-    notification must be balanced and the max open count is one.
+    The document's truth is now managed by the client and the server must not try to
+    read the document's truth using the document's uri. Open in this sense means it is
+    managed by the client. It doesn't necessarily mean that its content is presented in
+    an editor. An open notification must not be sent more than once without a
+    corresponding close notification send before. This means open and close notification
+    must be balanced and the max open count is one.
     """
 
     params: DidOpenTextDocumentParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["textDocument/didOpen"]),
         default="textDocument/didOpen",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentDidChangeNotification:
-    """The document change notification is sent from the client to the server
-    to signal changes to a text document."""
+    """The document change notification is sent from the client to the server to signal
+    changes to a text document."""
 
     params: DidChangeTextDocumentParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["textDocument/didChange"]),
         default="textDocument/didChange",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentDidCloseNotification:
-    """The document close notification is sent from the client to the server
-    when the document got closed in the client.
+    """The document close notification is sent from the client to the server when the
+    document got closed in the client.
 
-    The document's truth now exists where the document's uri points to
-    (e.g. if the document's uri is a file uri the truth now exists on
-    disk). As with the open notification the close notification is about
-    managing the document's content. Receiving a close notification
-    doesn't mean that the document was open in an editor before. A close
-    notification requires a previous open notification to be sent.
+    The document's truth now exists where the document's uri points to (e.g. if the
+    document's uri is a file uri the truth now exists on disk). As with the open
+    notification the close notification is about managing the document's content.
+    Receiving a close notification doesn't mean that the document was open in an editor
+    before. A close notification requires a previous open notification to be sent.
     """
 
     params: DidCloseTextDocumentParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["textDocument/didClose"]),
         default="textDocument/didClose",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentDidSaveNotification:
-    """The document save notification is sent from the client to the server
-    when the document got saved in the client."""
+    """The document save notification is sent from the client to the server when the
+    document got saved in the client."""
 
     params: DidSaveTextDocumentParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["textDocument/didSave"]),
         default="textDocument/didSave",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentWillSaveNotification:
-    """A document will save notification is sent from the client to the server
-    before the document is actually saved."""
+    """A document will save notification is sent from the client to the server before
+    the document is actually saved."""
 
     params: WillSaveTextDocumentParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["textDocument/willSave"]),
         default="textDocument/willSave",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class WorkspaceDidChangeWatchedFilesNotification:
-    """The watched files notification is sent from the client to the server
-    when the client detects changes to file watched by the language client."""
+    """The watched files notification is sent from the client to the server when the
+    client detects changes to file watched by the language client."""
 
     params: DidChangeWatchedFilesParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["workspace/didChangeWatchedFiles"]),
         default="workspace/didChangeWatchedFiles",
     )
     """The method to be invoked."""
     jsonrpc: str = attrs.field(default="2.0")
 
 
 @attrs.define
 class TextDocumentPublishDiagnosticsNotification:
-    """Diagnostics notification are sent from the server to the client to
-    signal results of validation runs."""
+    """Diagnostics notification are sent from the server to the client to signal results
+    of validation runs."""
 
     params: PublishDiagnosticsParams = attrs.field()
     method: str = attrs.field(
         validator=attrs.validators.in_(["textDocument/publishDiagnostics"]),
         default="textDocument/publishDiagnostics",
     )
     """The method to be invoked."""
```

### Comparing `lsprotocol-2023.0.0a1/lsprotocol/validators.py` & `lsprotocol-2023.0.0a2/lsprotocol/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 
 
 def uinteger_validator(
     instance: Any,
     attribute: "attrs.Attribute[int]",
     value: Any,
 ) -> bool:
-    """Validates that unsigned integer value belongs in the range expected by
-    LSP."""
+    """Validates that unsigned integer value belongs in the range expected by LSP."""
     if not isinstance(value, int) or not (
         UINTEGER_MIN_VALUE <= value <= UINTEGER_MAX_VALUE
     ):
         name = attribute.name if hasattr(attribute, "name") else str(attribute)
         raise ValueError(
             f"{instance.__class__.__qualname__}.{name} should be in range [{UINTEGER_MIN_VALUE}:{UINTEGER_MAX_VALUE}], but was {value}."
         )
```

### Comparing `lsprotocol-2023.0.0a1/pyproject.toml` & `lsprotocol-2023.0.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "lsprotocol"
 description = 'Python implementation of the Language Server Protocol.'
-version = "2023.0.0a1"
+version = "2023.0.0a2"
 authors = [
   { name = "Microsoft Corporation", email = "lsprotocol-help@microsoft.com" },
 ]
 license = { file = "LICENSE" }
 readme = { "file" = "README.md", "content-type" = "text/markdown" }
 requires-python = ">=3.7"
 maintainers = [
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["attrs", "cattrs"]
+dependencies = ["attrs>=21.3.0", "cattrs"]
 
 [project.urls]
 Issues = "https://github.com/microsoft/lsprotocol/issues"
 Source = "https://github.com/microsoft/lsprotocol"
 
 [tool.flit.sdist]
 include = ["lsprotocol/", "README.md", "LICENSE"]
```

### Comparing `lsprotocol-2023.0.0a1/PKG-INFO` & `lsprotocol-2023.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lsprotocol
-Version: 2023.0.0a1
+Version: 2023.0.0a2
 Summary: Python implementation of the Language Server Protocol.
 Author-email: Microsoft Corporation <lsprotocol-help@microsoft.com>
 Maintainer-email: Brett Cannon <brett@python.org>, Karthik Nadig <kanadig@microsoft.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: attrs
+Requires-Dist: attrs>=21.3.0
 Requires-Dist: cattrs
 Project-URL: Issues, https://github.com/microsoft/lsprotocol/issues
 Project-URL: Source, https://github.com/microsoft/lsprotocol
 
 # Language Server Protocol Types implementation for Python
 
 `lsprotocol` is a python implementation of object types used in the Language Server Protocol (LSP). This repository contains the code generator and the generated types for LSP.
```

