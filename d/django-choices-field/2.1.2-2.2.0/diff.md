# Comparing `tmp/django_choices_field-2.1.2.tar.gz` & `tmp/django_choices_field-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_choices_field-2.1.2.tar", max compression
+gzip compressed data, was "django_choices_field-2.2.0.tar", max compression
```

## Comparing `django_choices_field-2.1.2.tar` & `django_choices_field-2.2.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1077 2023-05-12 17:14:33.664796 django_choices_field-2.1.2/LICENSE
--rw-r--r--   0        0        0     2086 2023-05-12 17:14:33.664796 django_choices_field-2.1.2/README.md
--rw-r--r--   0        0        0      124 2023-05-12 17:14:33.664796 django_choices_field-2.1.2/django_choices_field/__init__.py
--rw-r--r--   0        0        0     3055 2023-05-12 17:14:33.664796 django_choices_field-2.1.2/django_choices_field/fields.py
--rw-r--r--   0        0        0     4848 2023-05-12 17:14:33.664796 django_choices_field-2.1.2/django_choices_field/fields.pyi
--rw-r--r--   0        0        0     3257 2023-05-12 17:14:33.668796 django_choices_field-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 django_choices_field-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/LICENSE
+-rw-r--r--   0        0        0     2822 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/README.md
+-rw-r--r--   0        0        0      188 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/django_choices_field/__init__.py
+-rw-r--r--   0        0        0     5249 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/django_choices_field/fields.py
+-rw-r--r--   0        0        0     7193 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/django_choices_field/fields.pyi
+-rw-r--r--   0        0        0      625 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/django_choices_field/types.py
+-rw-r--r--   0        0        0     3264 2023-06-21 18:18:36.403370 django_choices_field-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4141 1970-01-01 00:00:00.000000 django_choices_field-2.2.0/PKG-INFO
```

### Comparing `django_choices_field-2.1.2/LICENSE` & `django_choices_field-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_choices_field-2.1.2/README.md` & `django_choices_field-2.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -13,44 +13,64 @@
 ```bash
 pip install django-choices-field
 ```
 
 ## Usage
 
 ```python
+import enum
+
 from django.db import models
-from django_choices_field import TextChoicesField, IntegerChoicesField
+from django_choices_field import TextChoicesField, IntegerChoicesField, IntegerChoicesFlag
 
 
 class MyModel(models.Model):
     class TextEnum(models.TextChoices):
         FOO = "foo", "Foo Description"
         BAR = "bar", "Bar Description"
 
     class IntegerEnum(models.IntegerChoices):
         FIRST = 1, "First Description"
         SECOND = 2, "Second Description"
 
-    c_field = TextChoicesField(
+    class IntegerFlagEnum(IntegerChoicesFlag):
+        FIRST = enum.auto(), "First Option"
+        SECOND = enum.auto(), "Second Option"
+        THIRD = enum.auto(), "Third Option"
+
+    text_field = TextChoicesField(
         choices_enum=TextEnum,
         default=TextEnum.FOO,
     )
-    i_field = IntegerChoicesField(
+    integer_field = IntegerChoicesField(
         choices_enum=IntegerEnum,
         default=IntegerEnum.FIRST,
     )
+    flag_field = IntegerChoicesFlagField(
+        choices_enum=IntegerFlagEnum,
+        default=IntegerFlagEnum.FIRST | IntegerFlagEnum.SECOND,
+    )
 
 
 obj = MyModel()
-obj.c_field  # MyModel.TextEnum.FOO
-isinstance(obj.c_field, MyModel.TextEnum) # True
-obj.i_field  # MyModel.IntegerEnum.FIRST
-isinstance(obj.i_field, MyModel.IntegerEnum) # True
+reveal_type(obj.text_field)  # MyModel.TextEnum.FOO
+assert isinstance(obj.text_field, MyModel.TextEnum)
+assert obj.text_field == "foo"
+
+reveal_type(obj.integer_field)  # MyModel.IntegerEnum.FIRST
+assert isinstance(obj.integer_field, MyModel.IntegerEnum)
+assert obj.integer_field == 1
+
+reveal_type(obj.flag_field)  # MyModel.IntegerFlagEnum.FIRST | MyModel.IntegerFlagEnum.SECOND
+assert isinstance(obj.integer_field, MyModel.IntegerFlagEnum)
+assert obj.flag_field == 3
 ```
 
+NOTE: The `IntegerChoicesFlag` requires python 3.11+ to work properly.
+
 ## License
 
 This project is licensed under MIT licence (see `LICENSE` for more info)
 
 ## Contributing
 
 Make sure to have [poetry](https://python-poetry.org/) installed.
```

### Comparing `django_choices_field-2.1.2/django_choices_field/fields.pyi` & `django_choices_field-2.2.0/django_choices_field/fields.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     TypeVar,
     overload,
 )
 
 from django.db.models import Field, IntegerChoices, TextChoices
 from typing_extensions import TypeAlias
 
+from django_choices_field.types import IntegerChoicesFlag
+
 _ValidatorCallable: TypeAlias = Callable[..., None]
 _ErrorMessagesToOverride: TypeAlias = Dict[str, Any]
 
 _C = TypeVar("_C", bound=Optional[TextChoices])
 
 class TextChoicesField(Generic[_C], Field[_C, _C]):
     choices_enum: type[_C]
@@ -141,7 +143,72 @@
         error_messages: _ErrorMessagesToOverride | None = ...,
         path: str | Callable[..., str] = ...,
         match: str | None = ...,
         recursive: bool = ...,
         allow_files: bool = ...,
         allow_folders: bool = ...,
     ) -> IntegerChoicesField[_I | None]: ...
+
+_IF = TypeVar("_IF", bound=Optional[IntegerChoicesFlag])
+
+class IntegerChoicesFlagField(Generic[_IF], Field[_IF, _IF]):
+    choices_enum: type[_IF]
+    @overload
+    def __new__(
+        cls,
+        choices_enum: type[_IF],
+        verbose_name: str | None = ...,
+        name: str | None = ...,
+        primary_key: bool = ...,
+        max_length: int | None = ...,
+        unique: bool = ...,
+        blank: bool = ...,
+        null: Literal[False] = ...,
+        db_index: bool = ...,
+        default: _IF | Callable[[], _IF] = ...,
+        editable: bool = ...,
+        auto_created: bool = ...,
+        serialize: bool = ...,
+        unique_for_date: str | None = ...,
+        unique_for_month: str | None = ...,
+        unique_for_year: str | None = ...,
+        help_text: str = ...,
+        db_column: str | None = ...,
+        db_tablespace: str | None = ...,
+        validators: Iterable[_ValidatorCallable] = ...,
+        error_messages: _ErrorMessagesToOverride | None = ...,
+        path: str | Callable[..., str] = ...,
+        match: str | None = ...,
+        recursive: bool = ...,
+        allow_files: bool = ...,
+        allow_folders: bool = ...,
+    ) -> IntegerChoicesFlagField[_IF]: ...
+    @overload
+    def __new__(
+        cls,
+        choices_enum: type[_IF],
+        verbose_name: str | None = ...,
+        name: str | None = ...,
+        primary_key: bool = ...,
+        max_length: int | None = ...,
+        unique: bool = ...,
+        blank: bool = ...,
+        null: Literal[True] = ...,
+        db_index: bool = ...,
+        default: _IF | Callable[[], _IF] | None = ...,
+        editable: bool = ...,
+        auto_created: bool = ...,
+        serialize: bool = ...,
+        unique_for_date: str | None = ...,
+        unique_for_month: str | None = ...,
+        unique_for_year: str | None = ...,
+        help_text: str = ...,
+        db_column: str | None = ...,
+        db_tablespace: str | None = ...,
+        validators: Iterable[_ValidatorCallable] = ...,
+        error_messages: _ErrorMessagesToOverride | None = ...,
+        path: str | Callable[..., str] = ...,
+        match: str | None = ...,
+        recursive: bool = ...,
+        allow_files: bool = ...,
+        allow_folders: bool = ...,
+    ) -> IntegerChoicesFlagField[_IF | None]: ...
```

### Comparing `django_choices_field-2.1.2/pyproject.toml` & `django_choices_field-2.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-choices-field"
-version = "2.1.2"
+version = "2.2.0"
 description = "Django field that set/get django's new TextChoices/IntegerChoices enum."
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bellini666/django-choices-field"
 repository = "https://github.com/bellini666/django-choices-field"
 documentation = "https://django-choices-field.readthedocs.io"
@@ -28,24 +28,25 @@
   "Framework :: Django :: 4.2",
 ]
 packages = [{ include = "django_choices_field" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django = ">=3.2"
+typing_extensions = ">=4.0.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 codecov = "^2.1.11"
 django = "^4.0"
 django-types = "^0.17.0"
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
 pytest-django = "^4.2.0"
-ruff = "^0.0.265"
+ruff = "^0.0.274"
 
 [tool.black]
 line-length = 100
 target-version = ['py38']
 preview = true
 exclude = '''
 /(
@@ -131,16 +132,14 @@
   "__pycached__",
   "_build",
   "buck-out",
   "build",
   "dist",
 ]
 
-[tool.ruff.pyupgrade]
-
 [tool.ruff.isort]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.pyright]
 pythonVersion = "3.8"
```

### Comparing `django_choices_field-2.1.2/PKG-INFO` & `django_choices_field-2.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-choices-field
-Version: 2.1.2
+Version: 2.2.0
 Summary: Django field that set/get django's new TextChoices/IntegerChoices enum.
 Home-page: https://github.com/bellini666/django-choices-field
 License: MIT
 Keywords: django,enum
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
@@ -20,20 +20,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: django (>=3.2)
+Requires-Dist: typing_extensions (>=4.0.0)
 Project-URL: Documentation, https://django-choices-field.readthedocs.io
 Project-URL: Repository, https://github.com/bellini666/django-choices-field
 Description-Content-Type: text/markdown
 
 # django-choices-field
 
 [![build status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fbellini666%2Fdjango-choices-field%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/bellini666/django-choices-field/goto?ref=master)
@@ -49,44 +45,64 @@
 ```bash
 pip install django-choices-field
 ```
 
 ## Usage
 
 ```python
+import enum
+
 from django.db import models
-from django_choices_field import TextChoicesField, IntegerChoicesField
+from django_choices_field import TextChoicesField, IntegerChoicesField, IntegerChoicesFlag
 
 
 class MyModel(models.Model):
     class TextEnum(models.TextChoices):
         FOO = "foo", "Foo Description"
         BAR = "bar", "Bar Description"
 
     class IntegerEnum(models.IntegerChoices):
         FIRST = 1, "First Description"
         SECOND = 2, "Second Description"
 
-    c_field = TextChoicesField(
+    class IntegerFlagEnum(IntegerChoicesFlag):
+        FIRST = enum.auto(), "First Option"
+        SECOND = enum.auto(), "Second Option"
+        THIRD = enum.auto(), "Third Option"
+
+    text_field = TextChoicesField(
         choices_enum=TextEnum,
         default=TextEnum.FOO,
     )
-    i_field = IntegerChoicesField(
+    integer_field = IntegerChoicesField(
         choices_enum=IntegerEnum,
         default=IntegerEnum.FIRST,
     )
+    flag_field = IntegerChoicesFlagField(
+        choices_enum=IntegerFlagEnum,
+        default=IntegerFlagEnum.FIRST | IntegerFlagEnum.SECOND,
+    )
 
 
 obj = MyModel()
-obj.c_field  # MyModel.TextEnum.FOO
-isinstance(obj.c_field, MyModel.TextEnum) # True
-obj.i_field  # MyModel.IntegerEnum.FIRST
-isinstance(obj.i_field, MyModel.IntegerEnum) # True
+reveal_type(obj.text_field)  # MyModel.TextEnum.FOO
+assert isinstance(obj.text_field, MyModel.TextEnum)
+assert obj.text_field == "foo"
+
+reveal_type(obj.integer_field)  # MyModel.IntegerEnum.FIRST
+assert isinstance(obj.integer_field, MyModel.IntegerEnum)
+assert obj.integer_field == 1
+
+reveal_type(obj.flag_field)  # MyModel.IntegerFlagEnum.FIRST | MyModel.IntegerFlagEnum.SECOND
+assert isinstance(obj.integer_field, MyModel.IntegerFlagEnum)
+assert obj.flag_field == 3
 ```
 
+NOTE: The `IntegerChoicesFlag` requires python 3.11+ to work properly.
+
 ## License
 
 This project is licensed under MIT licence (see `LICENSE` for more info)
 
 ## Contributing
 
 Make sure to have [poetry](https://python-poetry.org/) installed.
```

