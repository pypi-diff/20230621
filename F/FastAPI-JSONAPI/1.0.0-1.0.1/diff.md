# Comparing `tmp/FastAPI-JSONAPI-1.0.0.tar.gz` & `tmp/fastapi_jsonapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastAPI-JSONAPI-1.0.0.tar", last modified: Thu Jun  1 15:49:43 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `FastAPI-JSONAPI-1.0.0.tar` & `fastapi_jsonapi-1.0.1.tar`

### file list

```diff
@@ -1,127 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.422194 FastAPI-JSONAPI-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-06-01 15:49:43.000000 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-01 15:49:43.000000 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:49:43.000000 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:49:43.000000 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-01 15:49:43.000000 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 15:49:43.000000 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-06-01 15:49:43.422194 FastAPI-JSONAPI-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/api/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/faker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/meta_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/meta_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/update_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/pydantic/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/sqlalchemy/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/api/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/faker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/meta_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/pydantic/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/tortoise/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/tortoise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/tortoise/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/data_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/fields/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/fields/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/fields/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/orm.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.422194 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sorting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sorting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)    23495 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sqlalchemy_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/tortoise_orm_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.422194 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/json_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/jsonapi_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14120 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/querystring.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-01 15:49:43.422194 FastAPI-JSONAPI-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.410194 FastAPI-JSONAPI-1.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.422194 FastAPI-JSONAPI-1.0.0/tests/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/tests/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/tests/misc/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/__init__.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/custom_filter_example.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/asgi.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/config.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/main.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/urls.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/__init__.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/base.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/child.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/parent.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/post.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/user.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/api/user_bio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/extensions/__init__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/extensions/sqlalchemy.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/__init__.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/exceptions.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/faker.py
+-rw-r--r--   0        0        0     9053 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/meta_base.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/post.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/user.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/user_bio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/__init__.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/exceptions.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/meta_base.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/update_post.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/update_user.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/child.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/enums.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/parent.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/parent_child_association.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/post.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/post_comment.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/user.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/user_bio.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/__init__.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/child.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/parent.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/parent_child_association.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/post.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/post_comment.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/user.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/user_bio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/__init__.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/asgi.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/main.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/urls.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/api/__init__.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/api/user.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/__init__.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/exceptions.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/faker.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/meta_base.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/__init__.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/update_user.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/enums.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/pydantic/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/pydantic/user.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/tortoise/__init__.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/tortoise/user.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/__init__.py
+-rw-r--r--   0        0        0    22987 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/api.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/jsonapi_typing.py
+-rw-r--r--   0        0        0    15106 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/methods.py
+-rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/querystring.py
+-rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/schema.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/schema_base.py
+-rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/signature.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/splitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/__init__.py
+-rw-r--r--   0        0        0    14282 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/base.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/data_typing.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/orm.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/shared.py
+-rw-r--r--   0        0        0    24198 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sqlalchemy_engine.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/tortoise_orm_engine.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/fields/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/fields/enum.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/fields/mixins.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/__init__.py
+-rw-r--r--   0        0        0    10236 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sorting/__init__.py
+-rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/exceptions/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/exceptions/base.py
+-rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/exceptions/json_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/views/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/views/detail_view.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/views/list_view.py
+-rw-r--r--   0        0        0    13121 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/fastapi_jsonapi/views/view_base.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/LICENSE
+-rw-r--r--   0        0        0     7059 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/README.md
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 fastapi_jsonapi-1.0.1/PKG-INFO
```

### Comparing `FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/PKG-INFO` & `fastapi_jsonapi-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,9 @@
-Metadata-Version: 2.1
-Name: FastAPI-JSONAPI
-Version: 1.0.0
-Summary: FastAPI extension to create REST web api according to JSON:API 1.0 specification with FastAPI, Pydantic and data provider of your choice (SQLAlchemy, Tortoise ORM)
-Home-page: https://github.com/mts-ai/FastAPI-JSONAPI
-Author: Team MTS AI
-Author-email: a.nekrasov@mts.ru
-License: MIT
-Keywords: fastapi jsonapi mts ai
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: tests
-Provides-Extra: docs
-Provides-Extra: tortoise-orm
-Provides-Extra: sqlalchemy
-License-File: LICENSE
+[![Documentation Status](https://readthedocs.org/projects/fastapi-jsonapi/badge/?version=latest)](https://fastapi-jsonapi.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/fastapi-jsonapi?label=PyPI)](https://pypi.org/project/FastAPI-JSONAPI/)
 
 # FastAPI-JSONAPI
 
 FastAPI-JSONAPI is a FastAPI extension for building REST APIs.
 Implementation of a strong specification [JSONAPI 1.0](http://jsonapi.org/).
 This framework is designed to quickly build REST APIs and fit the complexity
 of real life projects with legacy data and multiple data storages.
@@ -56,15 +35,14 @@
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.sql import Select
 
 from fastapi_jsonapi import RoutersJSONAPI
 from fastapi_jsonapi import SqlalchemyEngine
 from fastapi_jsonapi.data_layers.orm import DBORMType
-from fastapi_jsonapi.openapi import custom_openapi
 from fastapi_jsonapi.querystring import QueryStringManager
 from fastapi_jsonapi.schema import JSONAPIResultListSchema
 from fastapi_jsonapi.schema import collect_app_orm_schemas
 
 CURRENT_FILE = Path(__file__).resolve()
 CURRENT_DIR = CURRENT_FILE.parent
 PROJECT_DIR = CURRENT_DIR.parent.parent
@@ -135,15 +113,20 @@
 
     @classmethod
     async def get(cls, obj_id: int, session: AsyncSession = Depends(Connector.get_session)) -> UserSchema:
         user: User = (await session.execute(select(User).where(User.id == obj_id))).scalar_one()
         return UserSchema.from_orm(user)
 
     @classmethod
-    async def patch(cls, obj_id: int, data: UserPatchSchema, session: AsyncSession = Depends(Connector.get_session)) -> UserSchema:
+    async def patch(
+        cls,
+        obj_id: int,
+        data: UserPatchSchema,
+        session: AsyncSession = Depends(Connector.get_session),
+    ) -> UserSchema:
         user: User = (await session.execute(select(User).where(User.id == obj_id))).scalar_one()
         user.first_name = data.first_name
         await session.commit()
         return UserSchema.from_orm(user)
 
     @classmethod
     async def delete(cls, obj_id: int, session: AsyncSession = Depends(Connector.get_session)) -> None:
@@ -151,15 +134,17 @@
         await session.delete(user)
         await session.commit()
 
 
 class UserList:
     @classmethod
     async def get(
-            cls, query_params: QueryStringManager, session: AsyncSession = Depends(Connector.get_session)
+        cls,
+        query_params: QueryStringManager,
+        session: AsyncSession = Depends(Connector.get_session),
     ) -> Union[Select, JSONAPIResultListSchema]:
         user_query = select(User)
         dl = SqlalchemyEngine(query=user_query, schema=UserSchema, model=User, session=session)
         count, users_db = await dl.get_collection(qs=query_params)
         total_pages = count // query_params.pagination.size + (count % query_params.pagination.size and 1)
         users: List[UserSchema] = [UserSchema.from_orm(i_user) for i_user in users_db]
         return JSONAPIResultListSchema(
@@ -181,15 +166,15 @@
             "name": "User",
             "description": "",
         },
     ]
 
     routers: APIRouter = APIRouter()
     RoutersJSONAPI(
-        routers=routers,
+        router=routers,
         path="/user",
         tags=["User"],
         class_detail=UserDetail,
         class_list=UserList,
         schema=UserSchema,
         type_resource="user",
         schema_in_patch=UserPatchSchema,
@@ -220,22 +205,20 @@
         title="FastAPI and SQLAlchemy",
         debug=True,
         openapi_url="/openapi.json",
         docs_url="/docs",
     )
     add_routes(app)
     app.on_event("startup")(sqlalchemy_init)
-    custom_openapi(app, title="API for SQLAlchemy")
     collect_app_orm_schemas(app)
     return app
 
 
 app = create_app()
 
-
 if __name__ == "__main__":
     uvicorn.run(
         "test:app",
         host="0.0.0.0",
         port=8084,
         reload=True,
         app_dir=str(CURRENT_DIR),
```

### Comparing `FastAPI-JSONAPI-1.0.0/LICENSE` & `fastapi_jsonapi-1.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+THE SOFTWARE.
```

### Comparing `FastAPI-JSONAPI-1.0.0/PKG-INFO` & `fastapi_jsonapi-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 Metadata-Version: 2.1
 Name: FastAPI-JSONAPI
-Version: 1.0.0
+Version: 1.0.1
 Summary: FastAPI extension to create REST web api according to JSON:API 1.0 specification with FastAPI, Pydantic and data provider of your choice (SQLAlchemy, Tortoise ORM)
-Home-page: https://github.com/mts-ai/FastAPI-JSONAPI
-Author: Team MTS AI
-Author-email: a.nekrasov@mts.ru
-License: MIT
-Keywords: fastapi jsonapi mts ai
-Platform: any
-Classifier: Development Status :: 4 - Beta
+Project-URL: Documentation, https://fastapi-jsonapi.readthedocs.io/
+Project-URL: Source, https://github.com/mts-ai/FastAPI-JSONAPI
+Author-email: Aleksey Nekrasov <a.nekrasov@mts.ai>, Suren Khorenyan <s.khorenyan@mts.ai>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: fastapi,json:api,jsonapi
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
+Requires-Dist: fastapi>=0.79.0
+Requires-Dist: greenlet>=1.1.2
+Requires-Dist: pydantic>=1.9.1
+Requires-Dist: simplejson>=3.17.6
+Requires-Dist: sqlalchemy<2.0.0,>=1.4.39
+Requires-Dist: tortoise-orm>=0.19.2
+Requires-Dist: uvicorn>=0.18.2
 Provides-Extra: all
-Provides-Extra: tests
+Requires-Dist: pytest; extra == 'all'
+Requires-Dist: sphinx; extra == 'all'
+Requires-Dist: sqlalchemy<2.0.0,>=1.4.39; extra == 'all'
+Requires-Dist: tortoise-orm>=0.19.2; extra == 'all'
 Provides-Extra: docs
-Provides-Extra: tortoise-orm
+Requires-Dist: sphinx; extra == 'docs'
 Provides-Extra: sqlalchemy
-License-File: LICENSE
+Requires-Dist: sqlalchemy<2.0.0,>=1.4.39; extra == 'sqlalchemy'
+Provides-Extra: tests
+Requires-Dist: pytest; extra == 'tests'
+Provides-Extra: tortoise-orm
+Requires-Dist: tortoise-orm>=0.19.2; extra == 'tortoise-orm'
+Description-Content-Type: text/markdown
+
+[![Documentation Status](https://readthedocs.org/projects/fastapi-jsonapi/badge/?version=latest)](https://fastapi-jsonapi.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/fastapi-jsonapi?label=PyPI)](https://pypi.org/project/FastAPI-JSONAPI/)
 
 # FastAPI-JSONAPI
 
 FastAPI-JSONAPI is a FastAPI extension for building REST APIs.
 Implementation of a strong specification [JSONAPI 1.0](http://jsonapi.org/).
 This framework is designed to quickly build REST APIs and fit the complexity
 of real life projects with legacy data and multiple data storages.
@@ -56,15 +73,14 @@
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.sql import Select
 
 from fastapi_jsonapi import RoutersJSONAPI
 from fastapi_jsonapi import SqlalchemyEngine
 from fastapi_jsonapi.data_layers.orm import DBORMType
-from fastapi_jsonapi.openapi import custom_openapi
 from fastapi_jsonapi.querystring import QueryStringManager
 from fastapi_jsonapi.schema import JSONAPIResultListSchema
 from fastapi_jsonapi.schema import collect_app_orm_schemas
 
 CURRENT_FILE = Path(__file__).resolve()
 CURRENT_DIR = CURRENT_FILE.parent
 PROJECT_DIR = CURRENT_DIR.parent.parent
@@ -135,15 +151,20 @@
 
     @classmethod
     async def get(cls, obj_id: int, session: AsyncSession = Depends(Connector.get_session)) -> UserSchema:
         user: User = (await session.execute(select(User).where(User.id == obj_id))).scalar_one()
         return UserSchema.from_orm(user)
 
     @classmethod
-    async def patch(cls, obj_id: int, data: UserPatchSchema, session: AsyncSession = Depends(Connector.get_session)) -> UserSchema:
+    async def patch(
+        cls,
+        obj_id: int,
+        data: UserPatchSchema,
+        session: AsyncSession = Depends(Connector.get_session),
+    ) -> UserSchema:
         user: User = (await session.execute(select(User).where(User.id == obj_id))).scalar_one()
         user.first_name = data.first_name
         await session.commit()
         return UserSchema.from_orm(user)
 
     @classmethod
     async def delete(cls, obj_id: int, session: AsyncSession = Depends(Connector.get_session)) -> None:
@@ -151,15 +172,17 @@
         await session.delete(user)
         await session.commit()
 
 
 class UserList:
     @classmethod
     async def get(
-            cls, query_params: QueryStringManager, session: AsyncSession = Depends(Connector.get_session)
+        cls,
+        query_params: QueryStringManager,
+        session: AsyncSession = Depends(Connector.get_session),
     ) -> Union[Select, JSONAPIResultListSchema]:
         user_query = select(User)
         dl = SqlalchemyEngine(query=user_query, schema=UserSchema, model=User, session=session)
         count, users_db = await dl.get_collection(qs=query_params)
         total_pages = count // query_params.pagination.size + (count % query_params.pagination.size and 1)
         users: List[UserSchema] = [UserSchema.from_orm(i_user) for i_user in users_db]
         return JSONAPIResultListSchema(
@@ -181,15 +204,15 @@
             "name": "User",
             "description": "",
         },
     ]
 
     routers: APIRouter = APIRouter()
     RoutersJSONAPI(
-        routers=routers,
+        router=routers,
         path="/user",
         tags=["User"],
         class_detail=UserDetail,
         class_list=UserList,
         schema=UserSchema,
         type_resource="user",
         schema_in_patch=UserPatchSchema,
@@ -220,22 +243,20 @@
         title="FastAPI and SQLAlchemy",
         debug=True,
         openapi_url="/openapi.json",
         docs_url="/docs",
     )
     add_routes(app)
     app.on_event("startup")(sqlalchemy_init)
-    custom_openapi(app, title="API for SQLAlchemy")
     collect_app_orm_schemas(app)
     return app
 
 
 app = create_app()
 
-
 if __name__ == "__main__":
     uvicorn.run(
         "test:app",
         host="0.0.0.0",
         port=8084,
         reload=True,
         app_dir=str(CURRENT_DIR),
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py` & `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/extensions/sqlalchemy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from sqlalchemy.engine import make_url
 from sqlalchemy.ext.asyncio import AsyncSession, create_async_engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 
+from examples.api_for_sqlalchemy import config
 
 Base = declarative_base()
 
 
 def async_session() -> sessionmaker:
-    uri = "sqlite+aiosqlite:///db.sqlite3"
-    engine = create_async_engine(url=make_url(uri))
+    engine = create_async_engine(url=make_url(config.SQLA_URI), echo=config.SQLA_ECHO)
     _async_session = sessionmaker(bind=engine, class_=AsyncSession, expire_on_commit=False)
     return _async_session
 
 
 class Connector:
-
     @classmethod
     async def get_session(cls):
         """
         Получение сессии к БД.
 
         :return:
         """
-        async_session_ = async_session()
-        async with async_session_() as db_session:
-            async with db_session.begin():
-                yield db_session
+        sess = async_session()
+        async with sess() as db_session:
+            yield db_session
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/exceptions.py` & `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/exceptions.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/meta_base.py` & `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/meta_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,27 +9,27 @@
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
-from sqlalchemy.ext.asyncio import AsyncSession
+from tortoise import models
 
 from fastapi_jsonapi.data_layers.fields.enum import Enum
 from .exceptions import (
     ExceptionAfterCommit,
     ExceptionBeforeCreate,
     ExceptionNotFactory,
 )
 from fastapi_jsonapi.querystring import HeadersQueryStringManager
-from ...extensions.sqlalchemy import Base
+
 
 TYPE_VAR = TypeVar("TYPE_VAR")
-TYPE_MODEL = TypeVar("TYPE_MODEL", bound=Base)
+TYPE_MODEL = TypeVar("TypeModel", bound=models.Model)
 
 
 class FactoryUseMode(Enum):
     """Effects the creation of an object in a factory. In test mode data generated randomly."""
 
     test = 1  # for tests, that is, data is generated randomly (unless specified explicitly)
     production = 2  # working version, you can not allow random data generation
@@ -47,15 +47,19 @@
     awaitable_data = {
         'attribute_name': (lambda: Factories.get("example_factory").create, [<args_list>], {<kwargs_dict>}),
     }
     Warning!!! lambda function is required!
     """
 
     @classmethod
-    async def _get_data(cls, data: Optional[Dict[str, Any]] = None, mode: FactoryUseMode = FactoryUseMode.test) -> Dict:
+    async def _get_data(
+        cls,
+        data: Optional[Dict[str, Any]] = None,
+        mode: FactoryUseMode = FactoryUseMode.test,
+    ) -> Dict:
         new_kwargs = dict()
         if data:
             new_kwargs.update(data)
 
         if mode is FactoryUseMode.test:
             for name, val in cls.data.items():
                 if name not in new_kwargs:
@@ -69,15 +73,15 @@
     @classmethod
     async def create_batch(
         cls,
         count: int = 1,
         data: Optional[Dict[str, Any]] = None,
         save: bool = True,
         mode: FactoryUseMode = FactoryUseMode.test,
-    ) -> List[Base]:
+    ) -> List[models.MODEL]:
         """
         Create objects.
 
         :param cls: factory
         :param count: you can pass an optional parameter - the number of instances, default = 1
         :param data: named parameters for the factory
         :param save: flag save model to db or not (save by default)
@@ -106,41 +110,35 @@
     @classmethod
     async def create(
         cls,
         data: Optional[Dict[str, Any]] = None,
         header: Union[HeadersQueryStringManager, None] = None,
         save: bool = True,
         mode: FactoryUseMode = FactoryUseMode.test,
-        session: Optional[AsyncSession] = None,
-    ) -> Base:
+    ) -> models.MODEL:
         """
         Create objects.
 
         :param cls: factory
         :param data: named parameters for the factory
         :param header: header
         :param save: flag save model to db or not (save by default)
         :param mode: what is the factory used for
-        :param session:
         :return: created model.
         """
         new_kwargs = await cls._get_data(data=data, mode=mode)
 
         try:
             new_kwargs = await cls.before_create(many=False, mode=mode, model_kwargs=new_kwargs, header=header)
         except ExceptionBeforeCreate:
             pass
 
         result_data = cls.Meta.model(**new_kwargs)
         if save:
-            if session:
-                session.add(result_data)
-                await session.commit()
-            else:
-                await result_data.save()
+            await result_data.save()
 
         try:
             await cls.after_create(result_data=result_data, many=False, saved=save, mode=mode, header=header)
         except ExceptionAfterCommit:
             pass
 
         return result_data
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/user.py` & `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import (
     Any,
     Dict,
     Union,
 )
 
-from examples.api_for_sqlalchemy.models.enums import UserStatusEnum
+from examples.api_for_tortoise_orm.models.enums import UserStatusEnum
 
 from .exceptions import ErrorCreateObject
 from .faker import fake
 from .meta_base import (
     BaseFactory,
     FactoryUseMode,
 )
 from fastapi_jsonapi.querystring import HeadersQueryStringManager
-from ...models.sqlalchemy import User
+from ...models.tortoise import User
 
 
 class ErrorCreateUserObject(ErrorCreateObject):
     def __init__(self, description, field: str = ""):
         """Initialize constructor for exception while creating object."""
         super().__init__(User, description, field)
 
@@ -40,15 +40,14 @@
         model_kwargs: Dict,
         header: Union[HeadersQueryStringManager, None] = None,
     ) -> Dict:
         data_for_create_user: Dict[str, Any] = dict()
         cls._set_first_name(data_for_create_user, model_kwargs)
         cls._set_last_name(data_for_create_user, model_kwargs)
         cls._set_status(data_for_create_user, model_kwargs)
-        cls._set_age(data_for_create_user, model_kwargs)
         return data_for_create_user
 
     @classmethod
     def _set_first_name(cls, data_for_create_user: Dict, kwargs: Dict):
         """
         Set first name.
         """
@@ -58,17 +57,10 @@
     def _set_last_name(cls, data_for_create_user: Dict, kwargs: Dict):
         """
         Set first name.
         """
         data_for_create_user["last_name"] = kwargs.get("last_name", "Last name")
 
     @classmethod
-    def _set_age(cls, data_for_create_user: Dict, kwargs: Dict):
-        """
-        Set first name.
-        """
-        data_for_create_user["age"] = kwargs.get("age", 0)
-
-    @classmethod
     def _set_status(cls, data_for_create_user: Dict, kwargs: Dict):
         """Status setter."""
         data_for_create_user["status"] = UserStatusEnum.active
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/exceptions.py` & `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/exceptions.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/meta_base.py` & `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,85 +7,77 @@
     Iterable,
     Optional,
     Type,
     TypeVar,
     Union,
 )
 
-from sqlalchemy import select
-from sqlalchemy.ext.asyncio import AsyncSession
 from tortoise import models
 from tortoise.exceptions import DoesNotExist
 
 from fastapi_jsonapi.querystring import HeadersQueryStringManager
 
 from .exceptions import (
     ExceptionBeforeUpdate,
     ExceptionNotUpdater,
     ObjectNotFound,
 )
 
 TYPE_VAR = TypeVar("TYPE_VAR")
-TYPE_MODEL = TypeVar("TYPE_MODEL", bound=models.Model)
+TYPE_MODEL = TypeVar("TypeModel", bound=models.Model)
 
 
 class _BaseUpdater(Generic[TYPE_MODEL]):
     class Meta(object):
         model: Any
 
     @classmethod
     async def update(
         cls,
         model_or_id: Union[TYPE_MODEL, int],
         new_data: Dict[str, Any],
         header: Union[HeadersQueryStringManager, None] = None,
         save: bool = True,
         update_fields: Optional[Iterable[str]] = None,
-        session: Optional[AsyncSession] = None,
     ) -> TYPE_MODEL:
         """
         Create objects.
 
         :param cls: updater
         :param new_data: named parameters for the updater
         :param model_or_id: object or id
         :param header: header
         :param save: boolean flag: model saved to db or not
-        :param update_fields:
-        :param session:
         :return: created model.
         """
-        model_obj = await cls._preload_model(model_or_id, session)
+        model_obj = await cls._preload_model(model_or_id)
+        old_data = await model_obj.clone(pk=model_obj.id)  # type: ignore
 
         try:
             model_obj = await cls.before_update(obj=model_obj, new_data=new_data, header=header)
         except ExceptionBeforeUpdate:
             pass
 
         if save:
-            if session:
-                await session.commit()
-            else:
-                await model_obj.save(update_fields=update_fields)
+            await model_obj.save(update_fields=update_fields)
 
         return model_obj
 
     @classmethod
-    async def _preload_model(cls, model_or_id: Union[TYPE_MODEL, int], session: AsyncSession) -> TYPE_MODEL:
+    async def _preload_model(cls, model_or_id: Union[TYPE_MODEL, int]) -> TYPE_MODEL:
         """
         Preload model method.
 
         If updater initialize with int id - load from database with this id.
         :return: Model. Returns model from initialization or preloaded model.
         :raises ObjectNotFound: if object does not found.
         """
         if isinstance(model_or_id, int):
-
             try:
-                model = (await session.execute(select(cls.Meta.model).where(cls.Meta.model.id == model_or_id))).scalar_one()
+                model = await cls.Meta.model.get(id=model_or_id)
             except DoesNotExist:
                 raise ObjectNotFound(cls.Meta.model, description="Object does not exist")
 
             return model
         else:
             return model_or_id
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/update_user.py` & `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/update_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from fastapi_jsonapi.querystring import HeadersQueryStringManager
 from .exceptions import ErrorUpdateObject
 from .meta_base import (
     BaseUpdater,
 )
 from ...models.enums import UserStatusEnum
-from ...models.sqlalchemy import User
+from ...models.tortoise import User
 
 
 class ErrorUpdateUserObject(ErrorUpdateObject):
     """Exception class for user update helper."""
 
     def __init__(self, description, field: str = ""):
         """Initialize constructor for exception while updating object."""
@@ -35,30 +35,27 @@
     @classmethod
     async def before_update(
         cls,
         obj: User,
         new_data: Dict[str, Any],
         header: Union[HeadersQueryStringManager, None] = None,
     ) -> User:
-
         cls._update_first_name(obj, new_data)
         cls._update_last_name(obj, new_data)
         cls._update_status(obj, new_data)
         return obj
 
     @classmethod
     def _update_first_name(cls, obj: User, new_data: Dict[str, Any]) -> None:
-        """Balena_id setter."""
         first_name: Optional[str] = new_data.get("first_name")
         if first_name is not None and first_name != obj.first_name:
             obj.first_name = first_name
 
     @classmethod
     def _update_last_name(cls, obj: User, new_data: Dict[str, Any]) -> None:
-        """Balena_id setter."""
         last_name: Optional[str] = new_data.get("last_name")
         if last_name is not None and last_name != obj.last_name:
             obj.last_name = last_name
 
     @classmethod
     def _update_status(
         cls,
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/main.py` & `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 PROJECT_DIR = CURRENT_DIR.parent.parent
 
 sys.path.append(str(PROJECT_DIR))
 
 import uvicorn
 from fastapi import FastAPI
 
+from examples.api_for_sqlalchemy import config
 from examples.api_for_sqlalchemy.urls import add_routes
 from fastapi_jsonapi.schema import collect_app_orm_schemas
-from fastapi_jsonapi.openapi import custom_openapi
 
 
 async def sqlalchemy_init() -> None:
-    uri = "sqlite+aiosqlite:///db.sqlite3"
-    engine = create_async_engine(url=make_url(uri))
+    engine = create_async_engine(url=make_url(config.SQLA_URI), echo=config.SQLA_ECHO)
     async with engine.begin() as conn:
-        await conn.run_sync(Base.metadata.drop_all)
+        # We don't want to drop tables on each app restart!
+        # await conn.run_sync(Base.metadata.drop_all)
         await conn.run_sync(Base.metadata.create_all)
 
 
 def create_app() -> FastAPI:
     """
     Create app factory.
 
@@ -41,17 +41,17 @@
     """
     app = FastAPI(
         title="FastAPI and SQLAlchemy",
         debug=True,
         openapi_url="/openapi.json",
         docs_url="/docs",
     )
+    app.config = {"MAX_INCLUDE_DEPTH": 5}
     add_routes(app)
     app.on_event("startup")(sqlalchemy_init)
-    custom_openapi(app, title="API for SQLAlchemy")
     collect_app_orm_schemas(app)
     return app
 
 
 if __name__ == "__main__":
     uvicorn.run(
         "asgi:app",
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/pydantic/user.py` & `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/pydantic/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional
 
 from pydantic import (
     BaseModel,
     Field,
 )
 
-from examples.api_for_sqlalchemy.models.enums import UserStatusEnum
+from examples.api_for_tortoise_orm.models.enums import UserStatusEnum
 
 
 class UserBaseSchema(BaseModel):
     """User base schema."""
 
     class Config:
         """Pydantic schema config."""
@@ -22,15 +22,14 @@
     class Enum:
         """User enums."""
 
         status = UserStatusEnum
 
     first_name: Optional[str] = None
     last_name: Optional[str] = None
-    age: Optional[int] = None
     status: UserStatusEnum = Field(default=UserStatusEnum.active)
 
 
 class UserPatchSchema(UserBaseSchema):
     """User PATCH schema."""
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/urls.py` & `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,41 +11,42 @@
     FastAPI,
 )
 
 from fastapi_jsonapi import RoutersJSONAPI
 from fastapi_jsonapi.data_layers.orm import DBORMType
 from .models.pydantic import UserPatchSchema
 from .models.pydantic.user import (
-    UserSchema, UserInSchema,
+    UserSchema,
+    UserInSchema,
 )
 from .api.user import (
     UserDetail,
     UserList,
 )
-from .models.sqlalchemy import User
+from .models.tortoise import User
 
 
 def add_routes(app: FastAPI) -> List[Dict[str, Any]]:
     tags = [
         {
             "name": "User",
             "description": "",
         },
     ]
 
     routers: APIRouter = APIRouter()
     RoutersJSONAPI(
-        routers=routers,
+        router=routers,
         path="/user",
         tags=["User"],
         class_detail=UserDetail,
         class_list=UserList,
         schema=UserSchema,
         type_resource="user",
         schema_in_patch=UserPatchSchema,
         schema_in_post=UserInSchema,
         model=User,
-        engine=DBORMType.sqlalchemy,
+        engine=DBORMType.tortoise,
     )
 
     app.include_router(routers, prefix="")
     return tags
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py` & `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from datetime import datetime
-from typing import TypeVar, Generic, List
+from typing import Generic, List, TypeVar
 
 from sqlalchemy import (
     Column,
-    DateTime, inspect, delete, select,
+    DateTime,
+    delete,
+    inspect,
+    select,
 )
+from sqlalchemy.engine import Result
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.ext.declarative import declared_attr
 
 from examples.api_for_sqlalchemy.extensions.sqlalchemy import Base
 
 TypeBase = TypeVar("TypeBase", bound="Base")
-Model = TypeVar('Model', Base, Base)
+Model = TypeVar("Model", Base, Base)
 
 
 class BaseModelMixin(Generic[Model]):
     id: int
 
     @declared_attr
     def created_at(cls) -> Column:
@@ -42,32 +46,28 @@
         if commit:
             await session.commit()
         elif flush:
             await session.flush()
         return self
 
     async def delete(self, session: AsyncSession, commit: bool = True) -> "BaseModelMixin[Model]":
-        await session.execute(
-            delete(self)
-        )
+        await session.execute(delete(self))
         if commit:
             await session.commit()
         return self
 
     @classmethod
     async def get_all(cls, session: AsyncSession) -> List[Model]:
         result = await session.execute(select(Model))
         return result.scalars().all()
 
     @classmethod
     async def get_by_id(cls, id_: int, session: AsyncSession) -> Model:
-        result = await session.execute(
-            select(cls).where(cls.id == id_)
-        )
+        stmt = select(cls).where(cls.id == id_)
+        result: Result = await session.execute(stmt)
         return result.scalar_one()
 
     @classmethod
     async def get_or_none(cls, id_: int, session: AsyncSession) -> Model:
-        result = await session.execute(
-            select(cls).where(cls.id == id_)
-        )
-        return result.scalar()
+        stmt = select(cls).where(cls.id == id_)
+        result: Result = await session.execute(stmt)
+        return result.scalar_one_or_none()
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py` & `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,30 @@
-from typing import Union, Type, TypeVar
 from enum import Enum as EnumOriginal
+from typing import Type, TypeVar, Union
 
 from sqlalchemy import types
-
-from enum import Enum
-
 from sqlalchemy.engine import Dialect
 
+from fastapi_jsonapi.data_layers.fields.mixins import MixinEnum
 
-class MixinEnum(Enum):
-    @classmethod
-    def names(cls) -> str:
-        return ",".join(x.name for x in cls)
-
-    @classmethod
-    def values(cls) -> list:
-        return [value for _, value in cls._member_map_.items()]
-
-    @classmethod
-    def keys(cls) -> list:
-        return [key for key, _ in cls._member_map_.items()]
-
-    @classmethod
-    def inverse(cls) -> dict:
-        return {value: key for key, value in cls._member_map_.items()}
-
-    @classmethod
-    def value_to_enum(cls, value):
-        _value_to_enum = {value.value: value for _, value in cls._member_map_.items()}
-        return _value_to_enum.get(value)
-
-
-class Enum(MixinEnum):
-    pass
-
-
-TypeEnum = TypeVar("TypeEnum", bound="Enum")
+TypeEnum = TypeVar("TypeEnum", bound=MixinEnum)
 
 
 class EnumColumn(types.TypeDecorator):
     """
     Обычный Enum из python сохраняет в БД значение, а не ключ, как делает Enum sqlalchemy
     """
 
     impl = types.Text
     cache_ok = True
 
     def __init__(self, enum: Union[Type[EnumOriginal], Type[TypeEnum]], *args: list, **kwargs: dict):
         if not issubclass(enum, EnumOriginal):
-            raise TypeError(f"{enum} is not a subtype of Enum")
+            msg = f"{enum} is not a subtype of Enum"
+            raise TypeError(msg)
         self.enum = enum
         super().__init__(*args, **kwargs)
 
     def process_bind_param(self, value: Union[Type[EnumOriginal], Type[TypeEnum]], dialect: Dialect):
         if isinstance(value, EnumOriginal) and isinstance(value.value, (str, int)):
             return value.value
         if isinstance(value, str):
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/api/user.py` & `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/api/user.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py` & `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/factories/exceptions.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/user.py` & `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/factories/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from typing import (
     Any,
     Dict,
     Union,
 )
 
-from examples.api_for_tortoise_orm.models.enums import UserStatusEnum
+from examples.api_for_sqlalchemy.models import User
+from examples.api_for_sqlalchemy.models.enums import UserStatusEnum
+from fastapi_jsonapi.querystring import HeadersQueryStringManager
 
 from .exceptions import ErrorCreateObject
 from .faker import fake
 from .meta_base import (
     BaseFactory,
     FactoryUseMode,
 )
-from fastapi_jsonapi.querystring import HeadersQueryStringManager
-from ...models.tortoise import User
 
 
 class ErrorCreateUserObject(ErrorCreateObject):
     def __init__(self, description, field: str = ""):
         """Initialize constructor for exception while creating object."""
         super().__init__(User, description, field)
 
 
 class UserFactory(BaseFactory):
-    class Meta(object):
+    class Meta:
         model = User
 
     data = {
         "first_name": lambda: fake.word(),
         "last_name": lambda: fake.word(),
         "status": lambda: UserStatusEnum.active,
     }
@@ -36,18 +36,19 @@
     async def before_create(
         cls,
         many: bool,
         mode: FactoryUseMode,
         model_kwargs: Dict,
         header: Union[HeadersQueryStringManager, None] = None,
     ) -> Dict:
-        data_for_create_user: Dict[str, Any] = dict()
+        data_for_create_user: Dict[str, Any] = {}
         cls._set_first_name(data_for_create_user, model_kwargs)
         cls._set_last_name(data_for_create_user, model_kwargs)
         cls._set_status(data_for_create_user, model_kwargs)
+        cls._set_age(data_for_create_user, model_kwargs)
         return data_for_create_user
 
     @classmethod
     def _set_first_name(cls, data_for_create_user: Dict, kwargs: Dict):
         """
         Set first name.
         """
@@ -57,10 +58,17 @@
     def _set_last_name(cls, data_for_create_user: Dict, kwargs: Dict):
         """
         Set first name.
         """
         data_for_create_user["last_name"] = kwargs.get("last_name", "Last name")
 
     @classmethod
+    def _set_age(cls, data_for_create_user: Dict, kwargs: Dict):
+        """
+        Set first name.
+        """
+        data_for_create_user["age"] = kwargs.get("age", 0)
+
+    @classmethod
     def _set_status(cls, data_for_create_user: Dict, kwargs: Dict):
         """Status setter."""
         data_for_create_user["status"] = UserStatusEnum.active
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py` & `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py` & `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/helpers/updaters/update_user.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 from typing import (
     Any,
     Dict,
     Optional,
     Union,
 )
 
+from examples.api_for_sqlalchemy.models import User
+from examples.api_for_sqlalchemy.models.enums import UserStatusEnum
 from fastapi_jsonapi.querystring import HeadersQueryStringManager
+
 from .exceptions import ErrorUpdateObject
 from .meta_base import (
     BaseUpdater,
 )
-from ...models.enums import UserStatusEnum
-from ...models.tortoise import User
 
 
 class ErrorUpdateUserObject(ErrorUpdateObject):
     """Exception class for user update helper."""
 
     def __init__(self, description, field: str = ""):
         """Initialize constructor for exception while updating object."""
@@ -35,30 +36,27 @@
     @classmethod
     async def before_update(
         cls,
         obj: User,
         new_data: Dict[str, Any],
         header: Union[HeadersQueryStringManager, None] = None,
     ) -> User:
-
         cls._update_first_name(obj, new_data)
         cls._update_last_name(obj, new_data)
         cls._update_status(obj, new_data)
         return obj
 
     @classmethod
     def _update_first_name(cls, obj: User, new_data: Dict[str, Any]) -> None:
-        """Balena_id setter."""
         first_name: Optional[str] = new_data.get("first_name")
         if first_name is not None and first_name != obj.first_name:
             obj.first_name = first_name
 
     @classmethod
     def _update_last_name(cls, obj: User, new_data: Dict[str, Any]) -> None:
-        """Balena_id setter."""
         last_name: Optional[str] = new_data.get("last_name")
         if last_name is not None and last_name != obj.last_name:
             obj.last_name = last_name
 
     @classmethod
     def _update_status(
         cls,
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/main.py` & `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,24 +14,23 @@
 
 import uvicorn
 from fastapi import FastAPI
 from tortoise import Tortoise
 
 from examples.api_for_tortoise_orm.urls import add_routes
 from fastapi_jsonapi.schema import collect_app_orm_schemas
-from fastapi_jsonapi.openapi import custom_openapi
 
 
 async def tortoise_init() -> None:
     # Here we create a SQLite DB using file "db.sqlite3"
     #  also specify the app name of "models"
     #  which contain models from "app.models"
     await Tortoise.init(
-        db_url='sqlite://db.sqlite3',
-        modules={'models': ['models.tortoise']}
+        db_url="sqlite://db.sqlite3",
+        modules={"models": ["models.tortoise"]},
     )
     # Generate the schema
     await Tortoise.generate_schemas()
 
 
 def create_app() -> FastAPI:
     """
@@ -43,15 +42,14 @@
         title="FastAPI and Tortoise ORM",
         debug=True,
         openapi_url="/openapi.json",
         docs_url="/docs",
     )
     add_routes(app)
     app.on_event("startup")(tortoise_init)
-    custom_openapi(app, title="API for Tortoise ORM")
     collect_app_orm_schemas(app)
     return app
 
 
 if __name__ == "__main__":
     uvicorn.run(
         "asgi:app",
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/pydantic/user.py` & `fastapi_jsonapi-1.0.1/examples/api_for_sqlalchemy/models/schemas/user.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""User base schemas module."""
+"""User schemas module."""
 
 from datetime import datetime
-from typing import Optional
+from typing import TYPE_CHECKING, List, Optional
 
-from pydantic import (
-    BaseModel,
-    Field,
-)
+from examples.api_for_sqlalchemy.models.enums import UserStatusEnum
+from fastapi_jsonapi.schema_base import BaseModel, Field, RelationshipInfo
 
-from examples.api_for_tortoise_orm.models.enums import UserStatusEnum
+if TYPE_CHECKING:
+    from .post import PostSchema
+    from .user_bio import UserBioSchema
 
 
 class UserBaseSchema(BaseModel):
     """User base schema."""
 
     class Config:
         """Pydantic schema config."""
@@ -22,15 +22,17 @@
     class Enum:
         """User enums."""
 
         status = UserStatusEnum
 
     first_name: Optional[str] = None
     last_name: Optional[str] = None
+    age: Optional[int] = None
     status: UserStatusEnum = Field(default=UserStatusEnum.active)
+    email: str | None = None
 
 
 class UserPatchSchema(UserBaseSchema):
     """User PATCH schema."""
 
 
 class UserInSchema(UserBaseSchema):
@@ -40,12 +42,23 @@
 class UserSchema(UserInSchema):
     """User item schema."""
 
     class Config:
         """Pydantic model config."""
 
         orm_mode = True
-        model = "users"
 
     id: int
-    created_at: datetime = Field(description="Время создания данных")
-    modified_at: datetime = Field(description="Время изменения данных")
+    created_at: datetime = Field(description="Create datetime")
+    modified_at: datetime = Field(description="Update datetime")
+    posts: List["PostSchema"] = Field(
+        relationship=RelationshipInfo(
+            resource_type="post",
+            many=True,
+        ),
+    )
+
+    bio: Optional["UserBioSchema"] = Field(
+        relationship=RelationshipInfo(
+            resource_type="user_bio",
+        ),
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/tortoise/user.py` & `fastapi_jsonapi-1.0.1/examples/api_for_tortoise_orm/models/tortoise/user.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/base.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
     def __init__(self, kwargs):
         """
         Intialize an data layer instance with kwargs.
 
         :param dict kwargs: information about data layer instance
         """
-
         # initing this attribute here in the first place
         # because it can be easily overridden by kwargs below
 
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     def post_init(self):
@@ -55,287 +54,394 @@
 
         NOTE that the data layer is inited for each request
         :return:
         """
         pass
 
     async def create_object(self, data, view_kwargs):
-        """Create an object
+        """
+        Create an object
 
-        :param dict data: the data validated by pydantic
+        :param dict data: the data validated by schemas
         :param dict view_kwargs: kwargs from the resource view
         :return DeclarativeMeta: an object
         """
         raise NotImplementedError
 
     async def get_object(self, view_kwargs):
-        """Retrieve an object
+        """
+        Retrieve an object
 
         :params dict view_kwargs: kwargs from the resource view
         :return DeclarativeMeta: an object
         """
         raise NotImplementedError
 
     async def get_collection(self, qs, view_kwargs):
-        """Retrieve a collection of objects
+        """
+        Retrieve a collection of objects
 
         :param QueryStringManager qs: a querystring manager to retrieve information from url
         :param dict view_kwargs: kwargs from the resource view
         :return tuple: the number of object and the list of objects
         """
         raise NotImplementedError
 
     async def update_object(self, obj, data, view_kwargs):
-        """Update an object
+        """
+        Update an object
 
         :param DeclarativeMeta obj: an object
-        :param dict data: the data validated by pydantic
+        :param dict data: the data validated by schemas
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if object have changed else False
         """
         raise NotImplementedError
 
     async def delete_object(self, obj, view_kwargs):
-        """Delete an item through the data layer
+        """
+        Delete an item through the data layer
 
         :param DeclarativeMeta obj: an object
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
-    async def create_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
-        """Create a relationship
+    async def create_relationship(
+        self,
+        json_data,
+        relationship_field,
+        related_id_field,
+        view_kwargs,
+    ):
+        """
+        Create a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         raise NotImplementedError
 
-    async def get_relationship(self, relationship_field, related_type_, related_id_field, view_kwargs):
-        """Get information about a relationship
+    async def get_relationship(
+        self,
+        relationship_field,
+        related_type_,
+        related_id_field,
+        view_kwargs,
+    ):
+        """
+        Get information about a relationship
 
         :param str relationship_field: the model attribute used for relationship
         :param str related_type_: the related resource type
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return tuple: the object and related object(s)
         """
         raise NotImplementedError
 
-    async def update_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
-        """Update a relationship
+    async def update_relationship(
+        self,
+        json_data,
+        relationship_field,
+        related_id_field,
+        view_kwargs,
+    ):
+        """
+        Update a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         raise NotImplementedError
 
-    async def delete_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
-        """Delete a relationship
+    async def delete_relationship(
+        self,
+        json_data,
+        relationship_field,
+        related_id_field,
+        view_kwargs,
+    ):
+        """
+        Delete a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
     def query(self, view_kwargs):
-        """Construct the base query to retrieve wanted data
+        """
+        Construct the base query to retrieve wanted data
 
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
     def before_create_object(self, data, view_kwargs):
-        """Provide additional data before object creation
+        """
+        Provide additional data before object creation
 
-        :param dict data: the data validated by pydantic
+        :param dict data: the data validated by schemas
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
     def after_create_object(self, obj, data, view_kwargs):
-        """Provide additional data after object creation
+        """
+        Provide additional data after object creation
 
         :param obj: an object from data layer
-        :param dict data: the data validated by pydantic
+        :param dict data: the data validated by schemas
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
     async def before_get_object(self, view_kwargs):
-        """Make work before to retrieve an object
+        """
+        Make work before to retrieve an object
 
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
     async def after_get_object(self, obj, view_kwargs):
-        """Make work after to retrieve an object
+        """
+        Make work after to retrieve an object
 
         :param obj: an object from data layer
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
     async def before_get_collection(self, qs, view_kwargs):
-        """Make work before to retrieve a collection of objects
+        """
+        Make work before to retrieve a collection of objects
 
         :param QueryStringManager qs: a querystring manager to retrieve information from url
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
     async def after_get_collection(self, collection, qs, view_kwargs):
-        """Make work after to retrieve a collection of objects
+        """
+        Make work after to retrieve a collection of objects
 
         :param iterable collection: the collection of objects
         :param QueryStringManager qs: a querystring manager to retrieve information from url
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
     async def before_update_object(self, obj, data, view_kwargs):
-        """Make checks or provide additional data before update object
+        """
+        Make checks or provide additional data before update object
 
         :param obj: an object from data layer
-        :param dict data: the data validated by pydantic
+        :param dict data: the data validated by schemas
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
     def after_update_object(self, obj, data, view_kwargs):
-        """Make work after update object
+        """
+        Make work after update object
 
         :param obj: an object from data layer
-        :param dict data: the data validated by pydantic
+        :param dict data: the data validated by schemas
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
     def before_delete_object(self, obj, view_kwargs):
-        """Make checks before delete object
+        """
+        Make checks before delete object
 
         :param obj: an object from data layer
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
     def after_delete_object(self, obj, view_kwargs):
-        """Make work after delete object
+        """
+        Make work after delete object
 
         :param obj: an object from data layer
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
-    def before_create_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
-        """Make work before to create a relationship
+    def before_create_relationship(
+        self,
+        json_data,
+        relationship_field,
+        related_id_field,
+        view_kwargs,
+    ):
+        """
+        Make work before to create a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         raise NotImplementedError
 
-    def after_create_relationship(self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs):
-        """Make work after to create a relationship
+    def after_create_relationship(
+        self,
+        obj,
+        updated,
+        json_data,
+        relationship_field,
+        related_id_field,
+        view_kwargs,
+    ):
+        """
+        Make work after to create a relationship
 
         :param obj: an object from data layer
         :param bool updated: True if object was updated else False
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         raise NotImplementedError
 
-    async def before_get_relationship(self, relationship_field, related_type_, related_id_field, view_kwargs):
-        """Make work before to get information about a relationship
+    async def before_get_relationship(
+        self,
+        relationship_field,
+        related_type_,
+        related_id_field,
+        view_kwargs,
+    ):
+        """
+        Make work before to get information about a relationship
 
         :param str relationship_field: the model attribute used for relationship
         :param str related_type_: the related resource type
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return tuple: the object and related object(s)
         """
         raise NotImplementedError
 
     async def after_get_relationship(
-        self, obj, related_objects, relationship_field, related_type_, related_id_field, view_kwargs,
+        self,
+        obj,
+        related_objects,
+        relationship_field,
+        related_type_,
+        related_id_field,
+        view_kwargs,
     ):
-        """Make work after to get information about a relationship
+        """
+        Make work after to get information about a relationship
 
         :param obj: an object from data layer
         :param iterable related_objects: related objects of the object
         :param str relationship_field: the model attribute used for relationship
         :param str related_type_: the related resource type
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return tuple: the object and related object(s)
         """
         raise NotImplementedError
 
-    def before_update_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
-        """Make work before to update a relationship
+    def before_update_relationship(
+        self,
+        json_data,
+        relationship_field,
+        related_id_field,
+        view_kwargs,
+    ):
+        """
+        Make work before to update a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         raise NotImplementedError
 
-    def after_update_relationship(self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs):
-        """Make work after to update a relationship
+    def after_update_relationship(
+        self,
+        obj,
+        updated,
+        json_data,
+        relationship_field,
+        related_id_field,
+        view_kwargs,
+    ):
+        """
+        Make work after to update a relationship
 
         :param obj: an object from data layer
         :param bool updated: True if object was updated else False
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         :return boolean: True if relationship have changed else False
         """
         raise NotImplementedError
 
-    def before_delete_relationship(self, json_data, relationship_field, related_id_field, view_kwargs):
-        """Make work before to delete a relationship
+    def before_delete_relationship(
+        self,
+        json_data,
+        relationship_field,
+        related_id_field,
+        view_kwargs,
+    ):
+        """
+        Make work before to delete a relationship
 
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
-    def after_delete_relationship(self, obj, updated, json_data, relationship_field, related_id_field, view_kwargs):
-        """Make work after to delete a relationship
+    def after_delete_relationship(
+        self,
+        obj,
+        updated,
+        json_data,
+        relationship_field,
+        related_id_field,
+        view_kwargs,
+    ):
+        """
+        Make work after to delete a relationship
 
         :param obj: an object from data layer
         :param bool updated: True if object was updated else False
         :param dict json_data: the request params
         :param str relationship_field: the model attribute used for relationship
         :param str related_id_field: the identifier field of the related model
         :param dict view_kwargs: kwargs from the resource view
         """
         raise NotImplementedError
 
     def bound_rewritable_methods(self, methods):
-        """Bound additional methods to current instance
+        """
+        Bound additional methods to current instance
 
-        :param class meta: information from Meta class used to configure the data layer instance
+        :param class methods: methods
         """
         for key, value in methods.items():
             if key in self.REWRITABLE_METHODS:
                 setattr(self, key, types.MethodType(value, self))
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/fields/mixins.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/fields/mixins.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 """Helper to create sqlalchemy filters according to filter querystring parameter"""
 from typing import Any, List, Tuple, Type, Union
 
 from pydantic import BaseModel
 from pydantic.fields import ModelField
-from sqlalchemy import and_, or_, not_
-from sqlalchemy.orm import aliased, InstrumentedAttribute
+from sqlalchemy import and_, not_, or_
+from sqlalchemy.orm import InstrumentedAttribute, aliased
 from sqlalchemy.sql.elements import BinaryExpression
 
+from fastapi_jsonapi.data_layers.data_typing import TypeModel, TypeSchema
 from fastapi_jsonapi.data_layers.shared import create_filters_or_sorts
 from fastapi_jsonapi.exceptions import InvalidFilters, InvalidType
-
-from fastapi_jsonapi.data_layers.data_typing import TypeSchema, TypeModel
-from fastapi_jsonapi.schema import get_relationships, get_model_field
+from fastapi_jsonapi.schema import get_model_field, get_relationships
 from fastapi_jsonapi.splitter import SPLIT_REL
 
 Filter = BinaryExpression
 Join = List[Any]
 
 FilterAndJoins = Tuple[
     Filter,
     List[Join],
 ]
 
 
 def create_filters(model: Type[TypeModel], filter_info: Union[list, dict], schema: Type[TypeSchema]):
-    """Apply filters from filters information to base query
+    """
+    Apply filters from filters information to base query
     :param model: the model of the node
     :param filter_info: current node filter information
     :param schema: the resource
     """
     return create_filters_or_sorts(model, filter_info, Node, schema)
 
 
-class Node(object):
+class Node:
     """Helper to recursively create filters with sqlalchemy according to filter querystring parameter"""
 
     def __init__(self, model: Type[TypeModel], filter_: dict, schema: Type[TypeSchema]) -> None:
-        """Initialize an instance of a filter node
+        """
+        Initialize an instance of a filter node
 
         :param model: an sqlalchemy model
         :param dict filter_: filters information of the current node and deeper nodes
         :param schema: the serializer
         """
         self.model = model
         self.filter_ = filter_
@@ -52,105 +53,107 @@
         :param schema_field:
         :param model_column: column sqlalchemy
         :param operator:
         :param value:
         :return:
         """
         """
-        Custom sqlachemy filtering logic can be created in a pydantic field for any operator
+        Custom sqlachemy filtering logic can be created in a schemas field for any operator
         To implement a new filtering logic (override existing or create a new one)
         create a method inside a field following this pattern:
-        `_<your_op_name>_sql_filter_`. Each filtering method has to accept these params: 
-        * schema_field - pydantic field instance
+        `_<your_op_name>_sql_filter_`. Each filtering method has to accept these params:
+        * schema_field - schemas field instance
         * model_column - sqlalchemy column instance
         * value - filtering value
         * operator - your operator, for example: "eq", "in", "ilike_str_array", ...
         """
-        try:
-            f = getattr(schema_field, f'_{operator}_sql_filter_')
-        except AttributeError:
-            pass
-        else:
-            return f(
-                schema_field=schema_field,
-                model_column=model_column,
-                value=value,
-                operator=operator,
-            )
         # Here we have to deserialize and validate fields, that are used in filtering,
         # so the Enum fields are loaded correctly
 
-        if schema_field.sub_fields:
+        if schema_field.sub_fields:  # noqa: SIM108
             # Для случаев когда в схеме тип Union
-            fields = [i for i in schema_field.sub_fields]
+            fields = list(schema_field.sub_fields)
         else:
             fields = [schema_field]
         types = [i.type_ for i in fields]
         clear_value = None
         errors: List[str] = []
         for i_type in types:
             try:
-                if isinstance(value, list):
+                if isinstance(value, list):  # noqa: SIM108
                     clear_value = [i_type(item) for item in value]
                 else:
                     clear_value = i_type(value)
             except (TypeError, ValueError) as ex:
                 errors.append(str(ex))
         # Если None, при этом поле обязательное (среди типов в аннотации нет None, то кидаем ошибку)
-        if clear_value is None and not any([not i_f.required for i_f in fields]):
+        if clear_value is None and not any(not i_f.required for i_f in fields):
             raise InvalidType(detail=", ".join(errors))
         return getattr(model_column, self.operator)(clear_value)
 
-    def resolve(self) -> FilterAndJoins:
+    def resolve(self) -> FilterAndJoins:  # noqa: PLR0911
         """Create filter for a particular node of the filter tree"""
-        if 'or' in self.filter_:
-            return self._create_filters(type_filter='or')
-        elif 'and' in self.filter_:
-            return self._create_filters(type_filter='and')
-        elif 'not' in self.filter_:
-            filter_, joins = Node(self.model, self.filter_['not'], self.schema).resolve()
+        if "or" in self.filter_:
+            return self._create_filters(type_filter="or")
+        if "and" in self.filter_:
+            return self._create_filters(type_filter="and")
+        if "not" in self.filter_:
+            filter_, joins = Node(self.model, self.filter_["not"], self.schema).resolve()
             return not_(filter_), joins
-        else:
-            value = self.value
 
-            if isinstance(value, dict):
-                return self._relationship_filtering(value)
+        value = self.value
+        operator = self.filter_["op"]
+        schema_field: ModelField = self.schema.__fields__[self.name]
+
+        custom_filter = schema_field.field_info.extra.get(f"_{operator}_sql_filter_")
+        if custom_filter:
+            return custom_filter(
+                schema_field=schema_field,
+                model_column=self.column,
+                value=value,
+                operator=operator,
+            )
+
+        if SPLIT_REL in self.filter_.get("name", ""):
+            value = {
+                "name": SPLIT_REL.join(self.filter_["name"].split(SPLIT_REL)[1:]),
+                "op": operator,
+                "val": value,
+            }
+            return self._relationship_filtering(value)
 
-            if SPLIT_REL in self.filter_.get('name', ''):
-                value = {
-                    'name': SPLIT_REL.join(self.filter_['name'].split(SPLIT_REL)[1:]),
-                    'op': self.filter_['op'],
-                    'val': value,
-                }
-                return self._relationship_filtering(value)
-
-            schema_field: ModelField = self.schema.__fields__[self.name]
-            if schema_field.sub_fields:
-                # Для случаев когда в схеме тип Union
-                types = [i.type_ for i in schema_field.sub_fields]
-            else:
-                types = [schema_field.type_]
-            for i_type in types:
-                try:
-                    if issubclass(i_type, BaseModel):
-                        value = {
-                            'name': self.name,
-                            'op': self.filter_['op'],
-                            'val': value,
-                        }
-                        return self._relationship_filtering(value)
-                except (TypeError, ValueError):
-                    pass
+        if isinstance(value, dict):
+            return self._relationship_filtering(value)
+
+        if schema_field.sub_fields:  # noqa: SIM108
+            # Для случаев когда в схеме тип Union
+            types = [i.type_ for i in schema_field.sub_fields]
+        else:
+            types = [schema_field.type_]
+        for i_type in types:
+            try:
+                if issubclass(i_type, BaseModel):
+                    value = {
+                        "name": self.name,
+                        "op": operator,
+                        "val": value,
+                    }
+                    return self._relationship_filtering(value)
+            except (TypeError, ValueError):
+                pass
 
-            return self.create_filter(
+        return (
+            self.create_filter(
                 schema_field=schema_field,
                 model_column=self.column,
-                operator=self.filter_['op'],
+                operator=operator,
                 value=value,
-            ), []
+            ),
+            [],
+        )
 
     def _relationship_filtering(self, value):
         alias = aliased(self.related_model)
         joins = [[alias, self.column]]
         node = Node(alias, value, self.related_schema)
         filters, new_joins = node.resolve()
         joins.extend(new_joins)
@@ -162,112 +165,125 @@
         :param type_filter: 'or' или 'and'
         :return:
         """
         nodes = [Node(self.model, filter_, self.schema).resolve() for filter_ in self.filter_[type_filter]]
         joins = []
         for i_node in nodes:
             joins.extend(i_node[1])
-        op = and_ if type_filter == 'and' else or_
+        op = and_ if type_filter == "and" else or_
         return op(*[i_node[0] for i_node in nodes]), joins
 
     @property
     def name(self) -> str:
-        """Return the name of the node or raise a BadRequest exception
+        """
+        Return the name of the node or raise a BadRequest exception
 
         :return str: the name of the field to filter on
         """
-        name = self.filter_.get('name')
+        name = self.filter_.get("name")
 
         if name is None:
-            raise InvalidFilters("Can't find name of a filter")
+            msg = "Can't find name of a filter"
+            raise InvalidFilters(msg)
 
         if SPLIT_REL in name:
             name = name.split(SPLIT_REL)[0]
 
         if name not in self.schema.__fields__:
-            raise InvalidFilters("{} has no attribute {}".format(self.schema.__name__, name))
+            msg = "{} has no attribute {}".format(self.schema.__name__, name)
+            raise InvalidFilters(msg)
 
         return name
 
     @property
     def op(self) -> str:
-        """Return the operator of the node
+        """
+        Return the operator of the node
 
         :return str: the operator to use in the filter
         """
         try:
-            return self.filter_['op']
+            return self.filter_["op"]
         except KeyError:
-            raise InvalidFilters("Can't find op of a filter")
+            msg = "Can't find op of a filter"
+            raise InvalidFilters(msg)
 
     @property
     def column(self) -> InstrumentedAttribute:
-        """Get the column object
-        """
+        """Get the column object"""
         field = self.name
 
         model_field = get_model_field(self.schema, field)
 
         try:
             return getattr(self.model, model_field)
         except AttributeError:
-            raise InvalidFilters("{} has no attribute {}".format(self.model.__name__, model_field))
+            msg = "{} has no attribute {}".format(self.model.__name__, model_field)
+            raise InvalidFilters(msg)
 
     @property
     def operator(self) -> name:
-        """Get the function operator from his name
+        """
+        Get the function operator from his name
 
         :return callable: a callable to make operation on a column
         """
-        operators = (self.op, self.op + '_', '__' + self.op + '__')
+        operators = (self.op, self.op + "_", "__" + self.op + "__")
 
         for op in operators:
             if hasattr(self.column, op):
                 return op
 
-        raise InvalidFilters("{} has no operator {}".format(self.column.key, self.op))
+        msg = "{} has no operator {}".format(self.column.key, self.op)
+        raise InvalidFilters(msg)
 
     @property
     def value(self) -> Union[dict, list, int, str, float]:
-        """Get the value to filter on
+        """
+        Get the value to filter on
 
         :return: the value to filter on
         """
-        if self.filter_.get('field') is not None:
+        if self.filter_.get("field") is not None:
             try:
-                result = getattr(self.model, self.filter_['field'])
+                result = getattr(self.model, self.filter_["field"])
             except AttributeError:
-                raise InvalidFilters("{} has no attribute {}".format(self.model.__name__, self.filter_['field']))
+                msg = "{} has no attribute {}".format(self.model.__name__, self.filter_["field"])
+                raise InvalidFilters(msg)
             else:
                 return result
         else:
-            if 'val' not in self.filter_:
-                raise InvalidFilters("Can't find value or field in a filter")
+            if "val" not in self.filter_:
+                msg = "Can't find value or field in a filter"
+                raise InvalidFilters(msg)
 
-            return self.filter_['val']
+            return self.filter_["val"]
 
     @property
     def related_model(self):
-        """Get the related model of a relationship field
+        """
+        Get the related model of a relationship field
 
         :return DeclarativeMeta: the related model
         """
         relationship_field = self.name
 
         if relationship_field not in get_relationships(self.schema):
-            raise InvalidFilters("{} has no relationship attribute {}".format(self.schema.__name__, relationship_field))
+            msg = "{} has no relationship attribute {}".format(self.schema.__name__, relationship_field)
+            raise InvalidFilters(msg)
 
         return getattr(self.model, get_model_field(self.schema, relationship_field)).property.mapper.class_
 
     @property
     def related_schema(self):
-        """Get the related schema of a relationship field
+        """
+        Get the related schema of a relationship field
 
         :return Schema: the related schema
         """
         relationship_field = self.name
 
         if relationship_field not in get_relationships(self.schema):
-            raise InvalidFilters("{} has no relationship attribute {}".format(self.schema.__name__, relationship_field))
+            msg = "{} has no relationship attribute {}".format(self.schema.__name__, relationship_field)
+            raise InvalidFilters(msg)
 
         return self.schema.__fields__[relationship_field].type_
-
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Previously used: '__'
 """
 from typing import Protocol
 
+
 def add_suffix(field_name: str, suffix: str, sep: str = "__") -> str:
     """
     :param field_name:
     :param suffix:
     :param sep:
     :return:
     """
-    return "".join((field_name, sep, suffix,))
+    return "".join((field_name, sep, suffix))
 
 
 def type_op_any(field_name: str, type_op: str) -> str:
     """
     used to filter on to many relationships
     :param field_name:
     :param type_op:
@@ -268,15 +269,16 @@
     :param type_op:
     :return:
     """
     return add_suffix(field_name, "icontains")
 
 
 class ProcessTypeOperationFieldName(Protocol):
-    def __call__(self, field_name: str, type_op: str) -> str: ...
+    def __call__(self, field_name: str, type_op: str) -> str:
+        ...
 
 
 filters_dict: dict[str, ProcessTypeOperationFieldName] = {
     "any": type_op_any,
     "between": type_op_between,
     "endswith": type_op_endswith,
     "iendswith": type_op_iendswith,
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """Tortoise filters creator."""
 
 from typing import (
     Any,
+    Dict,
+    List,
+    Optional,
     Tuple,
-    Type, Generic,
+    Type,
+    Union,
 )
-from typing import Union, Dict, List, Optional
 
 from pydantic import BaseModel
 from pydantic.fields import ModelField
 from tortoise.expressions import Q
 from tortoise.queryset import QuerySet
 
-from fastapi_jsonapi.data_layers.data_typing import TypeQuery, TypeModel
+from fastapi_jsonapi.data_layers.data_typing import TypeModel
 from fastapi_jsonapi.data_layers.fields.enum import Enum
 from fastapi_jsonapi.data_layers.filtering.tortoise_operation import prepare_field_name_for_filtering
 from fastapi_jsonapi.data_layers.orm import DBORMOperandType
-from fastapi_jsonapi.exceptions import InvalidFilters
-from fastapi_jsonapi.exceptions import QueryError
+from fastapi_jsonapi.exceptions import InvalidFilters, QueryError
 from fastapi_jsonapi.jsonapi_typing import Filters
 from fastapi_jsonapi.querystring import QueryStringManager
 
 
 def prepare_filter_pair(field: Type[ModelField], field_name: str, type_op: str, value: Any) -> Tuple:
     """Prepare filter."""
     name_field_q: str = prepare_field_name_for_filtering(field_name, type_op)
     return name_field_q, value
 
 
 class FilterTortoiseORM:
-
     def __init__(self, model: TypeModel):
         self.model = model
 
     def create_query(self, filter_q: Union[tuple, Q]) -> Q:
         """Tortoise filter creation."""
         if isinstance(filter_q, tuple):
             return Q(**{filter_q[0]: filter_q[1]})
@@ -47,24 +48,24 @@
     ) -> Union[None, QuerySet, Dict[str, Union[QuerySet, List[QuerySet]]]]:
         """Filter for query to ORM."""
         if not filters:
             return None
         if op is DBORMOperandType.or_:
             result_filter = None
             for i_filter in filters:
-                i_filter = i_filter[0] if isinstance(i_filter, list) else i_filter
+                i_filter = i_filter[0] if isinstance(i_filter, list) else i_filter  # noqa: PLW2901
                 if result_filter is None:
                     result_filter = self.create_query(i_filter)
                 else:
                     result_filter |= self.create_query(i_filter)
             return result_filter
         if op is DBORMOperandType.and_:
             result_filter = None
             for i_filter in filters:
-                i_filter = i_filter[0] if isinstance(i_filter, list) else i_filter
+                i_filter = i_filter[0] if isinstance(i_filter, list) else i_filter  # noqa: PLW2901
                 if result_filter is None:
                     result_filter = self.create_query(i_filter)
                 else:
                     result_filter &= self.create_query(i_filter)
             return result_filter
         if op is DBORMOperandType.not_:
             return ~Q(**{filters[0][0][0]: filters[0][0][1]})
@@ -74,15 +75,15 @@
         self,
         schema: Type[BaseModel],
         filters: Filters,
     ) -> List:
         """
         Make a list with filters, which can be used in the tortoise filter.
 
-        :param schema: pydantic schema of object.
+        :param schema: schemas schema of object.
         :param filters: list of JSON API filters.
         :return: list of filters, prepared for use in tortoise model.
         :raises InvalidFilters: if the filter was created with an error.
         """
         converted_filters: List = []
         for i_filter in filters:
             if "or" in i_filter:
@@ -103,15 +104,15 @@
                 result = self.filter_converter(
                     schema.__fields__[name_field].type_,
                     [
                         {
                             "name": ".".join(model_fields[1:]),
                             "op": i_filter["op"],
                             "val": i_filter["val"],
-                        }
+                        },
                     ],
                 )
                 converted_filters.append(result)
             else:
                 val: Union[List[Any], Any]
                 field: ModelField = schema.__fields__[name_field]
                 if isinstance(i_filter["val"], list) and field.type_ is not list:
@@ -122,18 +123,18 @@
                     if errors:
                         raise InvalidFilters(str(errors), parameter=field.alias)
 
                 converted_filters.append(prepare_filter_pair(field, name_field, i_filter["op"], val))
         return converted_filters
 
     async def json_api_filter(
-            self,
-            query,
-            schema: Type[BaseModel],
-            query_params: QueryStringManager,
+        self,
+        query,
+        schema: Type[BaseModel],
+        query_params: QueryStringManager,
     ) -> QuerySet:
         """Make queries with filtering from request."""
         filters = self.filter_converter(
             schema=schema,
             filters=query_params.filters,
         )
         for i_filter in filters:
@@ -165,8 +166,9 @@
         :raises QueryError: if the field in the filter does not match the field in tortoise.
         """
         if isinstance(filter_q, Q):
             return Q(filter_q)
         elif filter_q is None:
             return None
         else:
-            raise QueryError("An unexpected argument for Q (result_filter={type})".format(type=type(filter_q)))
+            msg = "An unexpected argument for Q (result_filter={type})".format(type=type(filter_q))
+            raise QueryError(msg)
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/shared.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/shared.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Type, Union, Tuple, TYPE_CHECKING
+from typing import TYPE_CHECKING, Tuple, Type, Union
 
 from fastapi_jsonapi.data_layers.data_typing import TypeModel, TypeSchema
 
 if TYPE_CHECKING:
     from fastapi_jsonapi.data_layers.filtering.sqlalchemy import Node as NodeSQLAlchemy
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Helper to create sqlalchemy sortings according to filter querystring parameter"""
 from typing import Any, List, Tuple, Type, Union
 
 from pydantic.fields import ModelField
-from sqlalchemy.orm import aliased, InstrumentedAttribute, DeclarativeMeta
+from sqlalchemy.orm import DeclarativeMeta, InstrumentedAttribute, aliased
 from sqlalchemy.sql.elements import BinaryExpression
 
 from fastapi_jsonapi.data_layers.data_typing import TypeModel, TypeSchema
 from fastapi_jsonapi.data_layers.shared import create_filters_or_sorts
 from fastapi_jsonapi.exceptions import InvalidFilters, InvalidSort
-from fastapi_jsonapi.schema import get_relationships, get_model_field
+from fastapi_jsonapi.schema import get_model_field, get_relationships
 from fastapi_jsonapi.splitter import SPLIT_REL
 
-
 Sort = BinaryExpression
 Join = List[Any]
 
 SortAndJoins = Tuple[
     Sort,
     List[Join],
 ]
@@ -61,67 +60,70 @@
         Custom sqlachemy sorting logic can be created in a marshmallow field for any field
         You can override existing ('asc', 'desc') or create new - then follow this pattern:
         `_<custom_sort_name>_sql_sort_`. This method has to accept following params:
         * marshmallow_field - marshmallow field instance
         * model_column - sqlalchemy column instance
         """
         try:
-            f = getattr(schema_field, f'_{order}_sql_sort_')
+            f = getattr(schema_field, f"_{order}_sql_sort_")
         except AttributeError:
             pass
         else:
             return f(
                 schema_field=schema_field,
                 model_column=model_column,
             )
         return getattr(model_column, order)()
 
     def resolve(self) -> SortAndJoins:
         """
         Create sort for a particular node of the sort tree.
         """
-
-        field = self.sort_.get('field', '')
+        field = self.sort_.get("field", "")
         if not hasattr(self.model, field) and SPLIT_REL not in field:
-            raise InvalidSort("{} has no attribute {}".format(self.model.__name__, field))
+            msg = "{} has no attribute {}".format(self.model.__name__, field)
+            raise InvalidSort(msg)
 
         if SPLIT_REL in field:
-            value = {
-                'field': SPLIT_REL.join(field.split(SPLIT_REL)[1:]),
-                'order': self.sort_['order']
-            }
+            value = {"field": SPLIT_REL.join(field.split(SPLIT_REL)[1:]), "order": self.sort_["order"]}
             alias = aliased(self.related_model)
             joins = [[alias, self.column]]
             node = Node(alias, value, self.related_schema)
             filters, new_joins = node.resolve()
             joins.extend(new_joins)
             return filters, joins
 
-        return self.create_sort(
-            schema_field=self.schema.__fields__[self.name].type_,
-            model_column=self.column,
-            order=self.sort_['order']
-        ), []
+        return (
+            self.create_sort(
+                schema_field=self.schema.__fields__[self.name].type_,
+                model_column=self.column,
+                order=self.sort_["order"],
+            ),
+            [],
+        )
 
     @property
     def name(self) -> str:
-        """Return the name of the node or raise a BadRequest exception
+        """
+        Return the name of the node or raise a BadRequest exception
 
         :return str: the name of the sort to sort on
         """
-        name = self.sort_.get('field')
+        name = self.sort_.get("field")
 
         if name is None:
-            raise InvalidFilters("Can't find name of a sort")
+            msg = "Can't find name of a sort"
+            raise InvalidFilters(msg)
 
         if SPLIT_REL in name:
             name = name.split(SPLIT_REL)[0]
 
         if name not in self.schema.__fields__:
-            raise InvalidFilters("{} has no attribute {}".format(self.schema.__name__, name))
+            msg = "{} has no attribute {}".format(self.schema.__name__, name)
+            raise InvalidFilters(msg)
 
         return name
 
     @property
     def column(self) -> InstrumentedAttribute:
         """
         Get the column object.
@@ -131,36 +133,39 @@
         field = self.name
 
         model_field = get_model_field(self.schema, field)
 
         try:
             return getattr(self.model, model_field)
         except AttributeError:
-            raise InvalidFilters("{} has no attribute {}".format(self.model.__name__, model_field))
+            msg = "{} has no attribute {}".format(self.model.__name__, model_field)
+            raise InvalidFilters(msg)
 
     @property
     def related_model(self) -> DeclarativeMeta:
         """
         Get the related model of a relationship field.
 
         :return: the related model.
         """
         relationship_field = self.name
 
         if relationship_field not in get_relationships(self.schema):
-            raise InvalidFilters("{} has no relationship attribute {}".format(self.schema.__name__, relationship_field))
+            msg = "{} has no relationship attribute {}".format(self.schema.__name__, relationship_field)
+            raise InvalidFilters(msg)
 
         return getattr(self.model, get_model_field(self.schema, relationship_field)).property.mapper.class_
 
     @property
     def related_schema(self) -> TypeSchema:
         """
         Get the related schema of a relationship field.
 
         :return: the related schema
         """
         relationship_field = self.name
 
         if relationship_field not in get_relationships(self.schema):
-            raise InvalidFilters("{} has no relationship attribute {}".format(self.schema.__name__, relationship_field))
+            msg = "{} has no relationship attribute {}".format(self.schema.__name__, relationship_field)
+            raise InvalidFilters(msg)
 
         return self.schema.__fields__[relationship_field].type_
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import List, Dict
+from typing import Dict, List
 
 from tortoise.queryset import QuerySet
 
 
 class SortTortoiseORM:
-
     @classmethod
     def sort(
         cls,
         query: QuerySet,
         query_params_sorting: List[Dict[str, str]],
         default_sort: str = "",
     ) -> QuerySet:
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sqlalchemy_engine.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/sqlalchemy_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """This module is a CRUD interface between resource managers and the sqlalchemy ORM"""
-from typing import Any, Iterable, Type, Optional, Tuple
+from typing import Any, Iterable, Optional, Tuple, Type
 
-from sqlalchemy import select, func
+from sqlalchemy import func, select
 from sqlalchemy.exc import NoResultFound
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.inspection import inspect
-from sqlalchemy.orm import joinedload
+from sqlalchemy.orm import joinedload, selectinload
 from sqlalchemy.orm.attributes import InstrumentedAttribute
 from sqlalchemy.orm.collections import InstrumentedList
 from sqlalchemy.sql import Select
 
-from fastapi_jsonapi.querystring import QueryStringManager
 from fastapi_jsonapi.data_layers.base import BaseDataLayer
-from fastapi_jsonapi.data_layers.data_typing import TypeSchema, TypeModel
+from fastapi_jsonapi.data_layers.data_typing import TypeModel, TypeSchema
 from fastapi_jsonapi.data_layers.filtering.sqlalchemy import create_filters
 from fastapi_jsonapi.data_layers.sorting.sqlalchemy import create_sorts
 from fastapi_jsonapi.exceptions import (
-    RelationNotFound,
-    RelatedObjectNotFound,
-    ObjectNotFound,
     InvalidInclude,
+    ObjectNotFound,
+    RelatedObjectNotFound,
+    RelationNotFound,
 )
-from fastapi_jsonapi.querystring import PaginationQueryStringManager
+from fastapi_jsonapi.querystring import PaginationQueryStringManager, QueryStringManager
 from fastapi_jsonapi.schema import (
     get_model_field,
     get_related_schema,
 )
 from fastapi_jsonapi.splitter import SPLIT_REL
 
 
@@ -95,25 +94,32 @@
 
         await self.before_get_object(view_kwargs)
 
         id_name_field = self.id_name_field or inspect(self.model).primary_key[0].key
         try:
             filter_field = getattr(self.model, id_name_field)
         except Exception:
-            raise Exception(f"{self.model.__name__} has no attribute {id_name_field}")
+            msg = f"{self.model.__name__} has no attribute {id_name_field}"
+            raise Exception(msg)
 
-        url_field = getattr(self, "url_field", "id")
-        filter_value = view_kwargs[url_field]
+        filter_value = view_kwargs[self.url_field]
 
         query = self.retrieve_object_query(view_kwargs, filter_field, filter_value)
 
         if qs is not None:
             query = self.eagerload_includes(query, qs)
 
-        obj = (await self.session.execute(query)).scalars().first()
+        try:
+            obj = (await self.session.execute(query)).scalar_one()
+        except NoResultFound:
+            msg = f"{self.model.__name__} #{filter_value} not found"
+            raise ObjectNotFound(
+                msg,
+                parameter=self.url_field,
+            )
 
         await self.after_get_object(obj, view_kwargs)
 
         return obj
 
     async def get_collection_count(self, query: Select, qs: QueryStringManager, view_kwargs: dict) -> int:
         """
@@ -156,15 +162,15 @@
 
         query = self.paginate_query(query, qs.pagination)
 
         collection = (await self.session.execute(query)).scalars().all()
 
         collection = await self.after_get_collection(collection, qs, view_kwargs)
 
-        return objects_count, collection
+        return objects_count, list(collection)
 
     async def update_object(self, obj: Any, data: dict, view_kwargs: dict) -> bool:
         """
         Update an object through sqlalchemy.
 
         :params obj: an object from sqlalchemy.
         :params data: the data validated by pydantic.
@@ -218,28 +224,36 @@
         """
         await self.before_get_relationship(relationship_field, related_type_, related_id_field, view_kwargs)
 
         obj = await self.get_object(view_kwargs)
 
         if obj is None:
             filter_value = view_kwargs[self.url_field]
+            msg = f"{self.model.__name__}: {filter_value} not found"
             raise ObjectNotFound(
-                f"{self.model.__name__}: {filter_value} not found", parameter=self.url_field,
+                msg,
+                parameter=self.url_field,
             )
 
         if not hasattr(obj, relationship_field):
-            raise RelationNotFound(f"{obj.__class__.__name__} has no attribute {relationship_field}")
+            msg = f"{obj.__class__.__name__} has no attribute {relationship_field}"
+            raise RelationNotFound(msg)
 
         related_objects = getattr(obj, relationship_field)
 
         if related_objects is None:
             return obj, related_objects
 
         await self.after_get_relationship(
-            obj, related_objects, relationship_field, related_type_, related_id_field, view_kwargs,
+            obj,
+            related_objects,
+            relationship_field,
+            related_type_,
+            related_id_field,
+            view_kwargs,
         )
 
         if isinstance(related_objects, InstrumentedList):
             return obj, [{"type": related_type_, "id": getattr(obj_, related_id_field)} for obj_ in related_objects]
         else:
             return obj, {"type": related_type_, "id": getattr(related_objects, related_id_field)}
 
@@ -283,22 +297,20 @@
         Get a related object.
 
         :params related_model: an sqlalchemy model
         :params related_id_field: the identifier field of the related model
         :params obj: the sqlalchemy object to retrieve related objects from
         :return: a related object
         """
+        stmt = select(related_model).where(getattr(related_model, related_id_field) == obj["id"])
         try:
-            related_object = (
-                await self.session.execute(
-                    select(related_model).where(getattr(related_model, related_id_field) == obj["id"])
-                )
-            ).scalar_one()
+            related_object = (await self.session.execute(stmt)).scalar_one()
         except NoResultFound:
-            raise RelatedObjectNotFound(f"{related_model.__name__}.{related_id_field}: {obj['id']} not found")
+            msg = f"{related_model.__name__}.{related_id_field}: {obj['id']} not found"
+            raise RelatedObjectNotFound(msg)
 
         return related_object
 
     def filter_query(self, query: Select, filter_info: Optional[list]) -> Select:
         """
         Filter query according to jsonapi 1.0.
 
@@ -353,40 +365,40 @@
         Use eagerload feature of sqlalchemy to optimize data retrieval for include querystring parameter.
 
         :params query: sqlalchemy queryset.
         :params qs: a querystring manager to retrieve information from url.
         :return: the query with includes eagerloaded.
         """
         for include in qs.include:
-            joinload_object = None
-
-            if SPLIT_REL in include:
-                current_schema = self.schema
-                for obj in include.split(SPLIT_REL):
-                    try:
-                        field = get_model_field(current_schema, obj)
-                    except Exception as e:
-                        raise InvalidInclude(str(e))
-
-                    if joinload_object is None:
-                        joinload_object = joinedload(field)
-                    else:
-                        joinload_object = joinload_object.joinedload(field)
-
-                    current_schema = get_related_schema(current_schema, obj)
+            relation_join_object = None
 
-            else:
+            current_schema = self.schema
+            current_model = self.model
+            for related_field_name in include.split(SPLIT_REL):
                 try:
-                    field = get_model_field(self.schema, include)
+                    field_name_to_load = get_model_field(current_schema, related_field_name)
                 except Exception as e:
                     raise InvalidInclude(str(e))
 
-                joinload_object = joinedload(field)
+                field_to_load: InstrumentedAttribute = getattr(current_model, field_name_to_load)
+                is_many = field_to_load.property.uselist
+                if relation_join_object is None:
+                    relation_join_object = selectinload(field_to_load) if is_many else joinedload(field_to_load)
+                elif is_many:
+                    relation_join_object = relation_join_object.selectinload(field_to_load)
+                else:
+                    relation_join_object = relation_join_object.joinedload(field_to_load)
+
+                current_schema = get_related_schema(current_schema, related_field_name)
+
+                # the first entity is Mapper,
+                # the second entity is DeclarativeMeta
+                current_model = field_to_load.property.entity.entity
 
-            query = query.options(joinload_object)
+            query = query.options(relation_join_object)
 
         return query
 
     def retrieve_object_query(
         self,
         view_kwargs: dict,
         filter_field: InstrumentedAttribute,
@@ -396,15 +408,18 @@
         Build query to retrieve object.
 
         :params view_kwargs: kwargs from the resource view
         :params filter_field: the field to filter on
         :params filter_value: the value to filter with
         :return sqlalchemy query: a query from sqlalchemy
         """
-        return select(self.model).where(filter_field == filter_value)
+        query: Select = self.query(view_kwargs)
+        # noinspection PyNoneFunctionAssignment,PyTypeChecker
+        query: Select = query.where(filter_field == filter_value)
+        return query
 
     def query(self, view_kwargs: dict) -> Select:
         """
         Construct the base query to retrieve wanted data.
 
         :params view_kwargs: kwargs from the resource view
         """
@@ -468,25 +483,25 @@
         return collection
 
     async def before_update_object(self, obj: Any, data: dict, view_kwargs: dict):
         """
         Make checks or provide additional data before update object.
 
         :params obj: an object from data layer.
-        :params data: the data validated by pydantic.
+        :params data: the data validated by schemas.
         :params view_kwargs: kwargs from the resource view.
         """
         pass
 
     def after_update_object(self, obj: Any, data: dict, view_kwargs: dict):
         """
         Make work after update object.
 
         :params obj: an object from data layer.
-        :params data: the data validated by pydantic.
+        :params data: the data validated by schemas.
         :params view_kwargs: kwargs from the resource view.
         """
         pass
 
     def before_delete_object(self, obj: Any, view_kwargs: dict):
         """
         Make checks before delete object.
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/tortoise_orm_engine.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/data_layers/tortoise_orm_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """This module is a CRUD interface between resource managers and the sqlalchemy ORM"""
-from typing import Any, Iterable, Type, Optional, Tuple
+from typing import Any, Iterable, Optional, Tuple, Type
 
 from tortoise.queryset import QuerySet
 
-from fastapi_jsonapi.querystring import QueryStringManager, PaginationQueryStringManager
 from fastapi_jsonapi.data_layers.base import BaseDataLayer
-from fastapi_jsonapi.data_layers.data_typing import TypeSchema, TypeModel
+from fastapi_jsonapi.data_layers.data_typing import TypeModel, TypeSchema
 from fastapi_jsonapi.data_layers.filtering.tortoise_orm import FilterTortoiseORM
 from fastapi_jsonapi.data_layers.sorting.tortoise_orm import SortTortoiseORM
+from fastapi_jsonapi.querystring import PaginationQueryStringManager, QueryStringManager
 
 
 class TortoiseORMEngine(BaseDataLayer):
     """Sqlalchemy data layer"""
 
     def __init__(
         self,
@@ -110,15 +110,15 @@
         return objects_count, collection
 
     async def update_object(self, obj: Any, data: dict, view_kwargs: dict) -> bool:
         """
         Update an object through sqlalchemy.
 
         :params obj: an object from sqlalchemy.
-        :params data: the data validated by pydantic.
+        :params data: the data validated by schemas.
         :params view_kwargs: kwargs from the resource view.
         :return: True if object have changed else False.
         """
         pass
 
     async def delete_object(self, obj: Any, view_kwargs: dict):
         """
@@ -318,25 +318,25 @@
         return collection
 
     async def before_update_object(self, obj: Any, data: dict, view_kwargs: dict):
         """
         Make checks or provide additional data before update object.
 
         :params obj: an object from data layer.
-        :params data: the data validated by pydantic.
+        :params data: the data validated by schemas.
         :params view_kwargs: kwargs from the resource view.
         """
         pass
 
     def after_update_object(self, obj: Any, data: dict, view_kwargs: dict):
         """
         Make work after update object.
 
         :params obj: an object from data layer.
-        :params data: the data validated by pydantic.
+        :params data: the data validated by schemas.
         :params view_kwargs: kwargs from the resource view.
         """
         pass
 
     def before_delete_object(self, obj: Any, view_kwargs: dict):
         """
         Make checks before delete object.
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/__init__.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/exceptions/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     BadRequest,
     HTTPException,
     InvalidField,
     InvalidFilters,
     InvalidInclude,
     InvalidSort,
     InvalidType,
-    RelationNotFound,
-    RelatedObjectNotFound,
     ObjectNotFound,
+    RelatedObjectNotFound,
+    RelationNotFound,
 )
 
 __all__ = [
     "ExceptionResponseSchema",
     "ExceptionSchema",
     "ExceptionSourceSchema",
     "BadRequest",
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/base.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/json_api.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/exceptions/json_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
             errors = [self]
 
         super().__init__(errors[0].status_code, {"errors": [error._dict for error in errors]})
 
     @property
     def _dict(self):
-
         return {
             "status_code": self.status_code,
             "source": self.source,
             "title": self.title,
             "detail": self._detail,
         }
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/methods.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,33 +6,33 @@
     Callable,
     List,
     Optional,
     Type,
     TypeVar,
 )
 
-from fastapi import Query, Depends
+from fastapi import Query
 from pydantic import BaseModel
 from sqlalchemy.ext.asyncio import AsyncSession
 from starlette import status
 from starlette.requests import Request
 from starlette.responses import Response
 
 from fastapi_jsonapi.data_layers.data_typing import TypeModel
 from fastapi_jsonapi.data_layers.orm import DBORMType
 from fastapi_jsonapi.data_layers.sqlalchemy_engine import SqlalchemyEngine
 from fastapi_jsonapi.data_layers.tortoise_orm_engine import TortoiseORMEngine
 from fastapi_jsonapi.exceptions.json_api import UnsupportedFeatureORM
 from fastapi_jsonapi.querystring import QueryStringManager
+from fastapi_jsonapi.schema import JSONAPIResultDetailSchema, JSONAPIResultListSchema
 from fastapi_jsonapi.signature import update_signature
 
 
 def get_detail_jsonapi(
     schema: Type[BaseModel],
-    type_: str,
     schema_resp: Any,
     model: Type[TypeModel],
     engine: DBORMType,
 ) -> Callable:
     """GET DETAIL method router (Decorator for JSON API)."""
 
     def inner(func: Callable) -> Callable:
@@ -45,25 +45,29 @@
                     data_dict[i_name] = request
                 elif i_type.annotation is QueryStringManager:
                     data_dict[i_name] = query_params
 
             data_dict.update({i_k: i_v for i_k, i_v in kwargs.items() if i_k in func_signature})
             data_dict = {i_k: i_v for i_k, i_v in data_dict.items() if i_k in func_signature}
             data_schema: Any = await func(**data_dict)
+            if isinstance(data_schema, JSONAPIResultDetailSchema):
+                return data_schema
             return schema_resp(
                 data={
                     "id": data_schema.id,
                     "attributes": data_schema.dict(),
                 },
             )
 
         # mypy ругается что нет метода __signature__, как это обойти красиво- не знаю
         wrapper.__signature__ = update_signature(  # type: ignore
             sig=signature(wrapper),
+            schema=schema,
             other=OrderedDict(signature(func).parameters),
+            exclude_filters=True,
         )
 
         return wrapper
 
     return inner
 
 
@@ -86,23 +90,25 @@
     def inner(func: Callable) -> Callable:
         async def wrapper(request: Request, obj_id: int, data: schema_in, **kwargs):  # type: ignore
             query_params = QueryStringManager(request=request, schema=schema)
             data_dict = {"obj_id": obj_id}
             func_signature = signature(func).parameters
             for i_name, i_type in OrderedDict(func_signature).items():
                 if i_type.annotation is schema_in.__fields__["attributes"].type_:
-                    data_dict[i_name] = getattr(data, 'attributes', data)
+                    data_dict[i_name] = getattr(data, "attributes", data)
                 elif i_type.annotation is Request:
                     data_dict[i_name] = request
                 elif i_type.annotation is QueryStringManager:
                     data_dict[i_name] = query_params
 
             data_dict.update({i_k: i_v for i_k, i_v in kwargs.items() if i_k in func_signature})
             data_dict = {i_k: i_v for i_k, i_v in data_dict.items() if i_k in func_signature}
             data_schema: Any = await func(**data_dict)
+            if isinstance(data_schema, JSONAPIResultDetailSchema):
+                return data_schema
             return schema_resp(
                 data={
                     "id": data_schema.id,
                     "attributes": data_schema.dict(),
                 },
             )
 
@@ -160,17 +166,17 @@
     def inner(func: Callable) -> Callable:
         async def wrapper(
             request: Request,
             filters_list: Optional[str] = Query(
                 None,
                 alias="filter",
                 description="[Filtering docs](https://fastapi-jsonapi.readthedocs.io/en/latest/filtering.html)"
-                            "\nExamples:\n* filter for timestamp interval: "
-                            '`[{"name": "timestamp", "op": "ge", "val": "2020-07-16T11:35:33.383"},'
-                            '{"name": "timestamp", "op": "le", "val": "2020-07-21T11:35:33.383"}]`',
+                "\nExamples:\n* filter for timestamp interval: "
+                '`[{"name": "timestamp", "op": "ge", "val": "2020-07-16T11:35:33.383"},'
+                '{"name": "timestamp", "op": "le", "val": "2020-07-21T11:35:33.383"}]`',
             ),
             **kwargs,
         ):
             query_params = QueryStringManager(request=request, schema=schema)
             data_dict = {}
             func_signature = signature(func).parameters
             for i_name, i_type in OrderedDict(func_signature).items():
@@ -200,15 +206,15 @@
     query,
     query_params: QueryStringManager,
     schema: Type[BaseModel],
     type_: str,
     schema_resp: Any,
     model: Type[TypeModel],
     engine: DBORMType,
-    session: Optional[AsyncSession] = None
+    session: Optional[AsyncSession] = None,
 ) -> Any:
     if engine is DBORMType.sqlalchemy:
         dl = SqlalchemyEngine(schema=schema, model=model, session=session, query=query)
     elif engine is DBORMType.tortoise:
         dl = TortoiseORMEngine(schema=schema, model=model, query=query)
     else:
         raise UnsupportedFeatureORM()
@@ -244,16 +250,17 @@
                 alias="filter",
                 description="[Filtering docs](https://fastapi-jsonapi.readthedocs.io/en/latest/filtering.html)"
                 "\nExamples:\n* filter for timestamp interval: "
                 '`[{"name": "timestamp", "op": "ge", "val": "2020-07-16T11:35:33.383"},'
                 '{"name": "timestamp", "op": "le", "val": "2020-07-21T11:35:33.383"}]`',
             ),
             sort: Optional[str] = Query(
-                None, alias='sort', 
-                description="[Sorting docs](https://fastapi-jsonapi.readthedocs.io/en/latest/sorting.html)"
+                None,
+                alias="sort",
+                description="[Sorting docs](https://fastapi-jsonapi.readthedocs.io/en/latest/sorting.html)",
             ),
             **kwargs,
         ):
             query_params = QueryStringManager(request=request, schema=schema)
             data_dict = {}
             func_signature = signature(func).parameters
             for i_name, i_type in OrderedDict(func_signature).items():
@@ -262,44 +269,59 @@
                 elif i_type.annotation is QueryStringManager:
                     data_dict[i_name] = query_params
 
             data_dict.update({i_k: i_v for i_k, i_v in kwargs.items() if i_k in func_signature})
             data_dict = {i_k: i_v for i_k, i_v in data_dict.items() if i_k in func_signature}
             query = await func(**data_dict)
 
+            session = None
             if engine is DBORMType.sqlalchemy:
                 # Для SQLAlchemy нужно указывать session, для Tortoise достаточно модели
-                session_list = [i_v for i_k, i_v in func_signature.items() if isinstance(i_v, AsyncSession)]
-                session: Optional[AsyncSession] = session_list and session_list[0] or None
-            else:
-                session = None
+                session: Optional[AsyncSession] = next(
+                    # get first of type AsyncSession or None if not found
+                    filter(lambda v: isinstance(v, AsyncSession), func_signature.values()),
+                    None,
+                )
 
-            if isinstance(query, BaseModel):  # JSONAPIResultListSchema
+            if isinstance(query, JSONAPIResultListSchema):
                 return query
-            elif isinstance(query, list):
-                return schema_resp(data=[{"id": i_obj.id, "attributes": i_obj.dict(), "type": type_} for i_obj in query])
-            else:
-                if engine is DBORMType.sqlalchemy and session is None:
-                    raise UnsupportedFeatureORM("For SQLAlchemy you need to specify session in parameter")
-                return await _get_single_response(
-                    query,
-                    query_params,
-                    schema,
-                    type_,
-                    schema_resp,
-                    model=model,
-                    engine=engine,
-                    session=session,
-                )  # QuerySet
+
+            if isinstance(query, list):
+                return schema_resp(
+                    data=[{"id": i_obj.id, "attributes": i_obj.dict(), "type": type_} for i_obj in query],
+                )
+
+            session = None
+            if engine is DBORMType.sqlalchemy:
+                # Для SQLAlchemy нужно указывать session, для Tortoise достаточно модели
+                session: Optional[AsyncSession] = next(
+                    # get first of type AsyncSession or None if not found
+                    filter(lambda v: isinstance(v, AsyncSession), func_signature.values()),
+                    None,
+                )
+            if engine is DBORMType.sqlalchemy and session is None:
+                msg = "For SQLAlchemy you need to specify session in parameter"
+                raise UnsupportedFeatureORM(msg)
+            return await _get_single_response(
+                query,
+                query_params,
+                schema,
+                type_,
+                schema_resp,
+                model=model,
+                engine=engine,
+                session=session,
+            )  # QuerySet
 
         # mypy ругается что нет метода __signature__, как это обойти красиво- не знаю
         wrapper.__signature__ = update_signature(  # type: ignore
             sig=signature(wrapper),
             schema=schema,
             other=OrderedDict(signature(func).parameters),
+            # return_annotation=schema_resp,
         )
         return wrapper
 
     return inner
 
 
 def post_list_jsonapi(
@@ -316,35 +338,39 @@
     """
 
     def inner(func: Callable) -> Callable:
         async def wrapper(request: Request, data: schema_in, **kwargs):  # type: ignore
             query_params = QueryStringManager(request=request, schema=schema)
             data_dict = {}
             func_signature = signature(func).parameters
-            for i_name, i_type in OrderedDict(func_signature).items():
+            func_params = OrderedDict(func_signature)
+            for i_name, i_type in func_params.items():
                 if i_type.annotation is schema_in.__fields__["attributes"].type_:
-                    data_dict[i_name] = getattr(data, 'attributes', data)
+                    data_dict[i_name] = getattr(data, "attributes", data)
                 elif i_type.annotation is Request:
                     data_dict[i_name] = request
                 elif i_type.annotation is QueryStringManager:
                     data_dict[i_name] = query_params
 
-            params_function = OrderedDict(func_signature)
-            data_dict.update({i_k: i_v for i_k, i_v in kwargs.items() if i_k in params_function})
-            data_dict = {i_k: i_v for i_k, i_v in data_dict.items() if i_k in params_function}
+            data_dict.update({i_k: i_v for i_k, i_v in kwargs.items() if i_k in func_params})
+            data_dict = {i_k: i_v for i_k, i_v in data_dict.items() if i_k in func_params}
             data_pydantic: Any = await func(**data_dict)
+            if isinstance(data_pydantic, JSONAPIResultDetailSchema):
+                return data_pydantic
             return schema_resp(
                 data={
                     "id": data_pydantic.id,
                     "attributes": data_pydantic.dict(),
                 },
             )
 
         # mypy ругается что нет метода __signature__, как это обойти красиво- не знаю
         wrapper.__signature__ = update_signature(  # type: ignore
             sig=signature(wrapper),
+            schema=schema,
             other=OrderedDict(signature(func).parameters),
+            exclude_filters=True,
         )
 
         return wrapper
 
     return inner
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/querystring.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/querystring.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Helper to deal with querystring parameters according to jsonapi specification."""
 
 from typing import (
+    TYPE_CHECKING,
     Any,
     Dict,
     List,
     Optional,
     Type,
-    Union, TYPE_CHECKING,
+    Union,
 )
 from urllib.parse import unquote
 
 import simplejson as json
 from fastapi import (
     FastAPI,
     Request,
 )
 from pydantic import (
     BaseModel,
     Field,
 )
 
-
 from fastapi_jsonapi.exceptions import (
     BadRequest,
     InvalidField,
     InvalidFilters,
     InvalidInclude,
     InvalidSort,
 )
@@ -78,15 +78,15 @@
         Initialize instance.
 
         :param request
         """
         self.request: Request = request
         self.app: FastAPI = request.app
         self.qs: Dict[str, str] = dict(request.query_params)
-        self.config: Dict[str, Any] = getattr(self.app, "config", dict())
+        self.config: Dict[str, Any] = getattr(self.app, "config", {})
         self.schema: Type[BaseModel] = schema
         self.ALLOW_DISABLE_PAGINATION: bool = self.config.get("ALLOW_DISABLE_PAGINATION", True)
         self.MAX_PAGE_SIZE: int = self.config.get("MAX_PAGE_SIZE", 10000)
         self.MAX_INCLUDE_DEPTH: int = self.config.get("MAX_INCLUDE_DEPTH", 3)
         self._pagination: Optional[PaginationQueryStringManager] = None
         self.headers: HeadersQueryStringManager = HeadersQueryStringManager(**dict(self.request.headers))
 
@@ -94,15 +94,15 @@
         """
         Return a dict containing key / values items for a given key, used for items like filters, page, etc.
 
         :param name: name of the querystring parameter
         :return: a dict of key / values items
         :raises BadRequest: if an error occurred while parsing the querystring.
         """
-        results: Dict[str, Union[List[str], str]] = dict()
+        results: Dict[str, Union[List[str], str]] = {}
 
         for raw_key, value in self.qs.items():
             key = unquote(raw_key)
             try:
                 if not key.startswith(name):
                     continue
 
@@ -111,15 +111,16 @@
                 item_key = key[key_start:key_end]
 
                 if "," in value:
                     results.update({item_key: value.split(",")})
                 else:
                     results.update({item_key: value})
             except Exception:
-                raise BadRequest("Parse error", parameter=key)
+                msg = "Parse error"
+                raise BadRequest(msg, parameter=key)
 
         return results
 
     @classmethod
     def _simple_filters(cls, dict_: Dict[str, Any]) -> List[Dict[str, Any]]:
         """Filter creation."""
         return [{"name": key, "op": "eq", "val": value} for (key, value) in dict_.items()]
@@ -147,15 +148,16 @@
         """
         results = []
         filters = self.qs.get("filter")
         if filters is not None:
             try:
                 results.extend(json.loads(filters))
             except (ValueError, TypeError):
-                raise InvalidFilters("Parse error")
+                msg = "Parse error"
+                raise InvalidFilters(msg)
         if self._get_key_values("filter["):
             results.extend(self._simple_filters(self._get_key_values("filter[")))
         return results
 
     @property
     def pagination(self) -> PaginationQueryStringManager:
         """
@@ -183,15 +185,16 @@
         # check values type
         pagination_data: Dict[str, Union[List[str], str]] = self._get_key_values("page")
         self._pagination = PaginationQueryStringManager(**pagination_data)
         if pagination_data.get("size") is None:
             self._pagination.size = None
         if self._pagination.size:
             if self.ALLOW_DISABLE_PAGINATION is False and self._pagination.size == 0:
-                raise BadRequest("You are not allowed to disable pagination", parameter="page[size]")
+                msg = "You are not allowed to disable pagination"
+                raise BadRequest(msg, parameter="page[size]")
             if self.MAX_PAGE_SIZE and self._pagination.size > self.MAX_PAGE_SIZE:
                 self._pagination.size = self.MAX_PAGE_SIZE
 
         return self._pagination
 
     @property
     def fields(self) -> Dict[str, List[str]]:
@@ -205,24 +208,29 @@
             {
                 "user": ['name', 'email'],
             }
 
         :raises InvalidField: if result field not in schema.
         """
         if self.request.method != "GET":
-            raise InvalidField("attribute 'fields' allowed only for GET-method")
+            msg = "attribute 'fields' allowed only for GET-method"
+            raise InvalidField(msg)
         fields = self._get_key_values("fields")
         for key, value in fields.items():
             if not isinstance(value, list):
-                value = [value]
+                value = [value]  # noqa: PLW2901
                 fields[key] = value
             schema: Type[BaseModel] = get_schema_from_type(key, self.app)
             for field in value:
                 if field not in schema.__fields__:
-                    raise InvalidField("{schema} has no attribute {field}".format(schema=schema.__name__, field=field))
+                    msg = "{schema} has no attribute {field}".format(
+                        schema=schema.__name__,
+                        field=field,
+                    )
+                    raise InvalidField(msg)
 
         return fields
 
     @property
     def sorting(self) -> List[Dict[str, str]]:
         """
         Return fields to sort by including sort name for SQLAlchemy and row sort parameter for other ORMs.
@@ -239,24 +247,22 @@
         """
         if self.qs.get("sort"):
             sorting_results = []
             for sort_field in self.qs["sort"].split(","):
                 field = sort_field.replace("-", "")
                 if SPLIT_REL not in field:
                     if field not in self.schema.__fields__:
-                        raise InvalidSort(
-                            "{schema} has no attribute {field}".format(
-                                schema=self.schema.__name__,
-                                field=field,
-                            )
+                        msg = "{schema} has no attribute {field}".format(
+                            schema=self.schema.__name__,
+                            field=field,
                         )
+                        raise InvalidSort(msg)
                     if field in get_relationships(self.schema):
-                        raise InvalidSort(
-                            "You can't sort on {field} because it is a relationship field".format(field=field)
-                        )
+                        msg = "You can't sort on {field} because it is a relationship field".format(field=field)
+                        raise InvalidSort(msg)
                     field = get_model_field(self.schema, field)
                 order = "desc" if sort_field.startswith("-") else "asc"
                 sorting_results.append({"field": field, "order": order})
             return sorting_results
 
         return []
 
@@ -264,19 +270,18 @@
     def include(self) -> List[str]:
         """
         Return fields to include.
 
         :return: a list of include information.
         :raises InvalidInclude: if nesting is more than MAX_INCLUDE_DEPTH.
         """
-        include_param: str = self.qs.get("include", "")
+        include_param: str = self.qs.get("include")
+        includes = include_param.split(",") if include_param and isinstance(include_param, str) else []
 
         if self.MAX_INCLUDE_DEPTH is not None:
-            # TODO: does this really work? needs tests!
-            for include_path in include_param:
+            for include_path in includes:
                 if len(include_path.split(SPLIT_REL)) > self.MAX_INCLUDE_DEPTH:
-                    raise InvalidInclude(
-                        "You can't use include through more than {max_include_depth} relationships".format(
-                            max_include_depth=self.MAX_INCLUDE_DEPTH
-                        )
+                    msg = "You can't use include through more than {max_include_depth} relationships".format(
+                        max_include_depth=self.MAX_INCLUDE_DEPTH,
                     )
-        return include_param.split(",") if isinstance(include_param, str) and include_param else []
+                    raise InvalidInclude(msg)
+        return includes
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/schema.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,74 @@
-"""Helpers to deal with marshmallow schemas. Base JSON:API schemas."""
-import uuid
+"""
+Base JSON:API schemas.
+Pydantic (for FastAPI).
+"""
 from typing import (
+    TYPE_CHECKING,
     Dict,
-    Type,
     List,
     Optional,
-    Sequence, TYPE_CHECKING, Union,
+    Sequence,
+    Type,
 )
 
 from fastapi import FastAPI
 from fastapi.openapi.utils import get_flat_models_from_routes
-
 from pydantic import (
     BaseModel,
     Field,
 )
 
 if TYPE_CHECKING:
     from fastapi_jsonapi.data_layers.data_typing import TypeSchema
 
 
+class BaseJSONAPIRelationshipSchema(BaseModel):
+    id: str = Field(..., description="Related object ID")
+    type: str = Field(..., description="Type of the related resource object")
+
+
+class BaseJSONAPIRelationshipDataToOneSchema(BaseModel):
+    data: BaseJSONAPIRelationshipSchema
+
+
+class BaseJSONAPIRelationshipDataToManySchema(BaseModel):
+    data: List[BaseJSONAPIRelationshipSchema]
+
+
 class BaseJSONAPIItemSchema(BaseModel):
     """Base JSON:API item schema."""
 
-    type: str = Field(description="Тип ресурса")
-    attributes: dict = Field(description="Данные объекта")
+    type: str = Field(description="Resource type")
+    attributes: dict = Field(description="Resource object attributes")
 
 
 class BasePostJSONAPISchema(BaseJSONAPIItemSchema):
     """Base POST JSON:API schema."""
 
 
 class BaseJSONAPIObjectSchema(BaseJSONAPIItemSchema):
     """Base JSON:API object schema."""
 
-    id: str = Field(description="ID объекта")
+    id: str = Field(description="Resource object ID")
 
 
 class BasePatchJSONAPISchema(BaseJSONAPIObjectSchema):
     """Base PATCH JSON:API schema."""
 
 
 class JSONAPIResultListMetaSchema(BaseModel):
     """JSON:API list meta schema."""
 
     count: Optional[int]
     total_pages: Optional[int] = Field(alias="totalPages")
 
+    class Config:
+        allow_population_by_field_name = True
+
 
 class JSONAPIDocumentObjectSchema(BaseModel):
     """
     JSON:API Document Object Schema.
     https://jsonapi.org/format/#document-jsonapi-object
     """
 
@@ -62,28 +80,28 @@
 
 
 class BaseJSONAPIResultSchema(BaseModel):
     """
     JSON:API Required fields schema
     """
 
-    meta: Optional[JSONAPIResultListMetaSchema] = Field(description="Meta данные json-api")
+    meta: Optional[JSONAPIResultListMetaSchema] = Field(description="JSON:API metadata")
     jsonapi: JSONAPIDocumentObjectSchema = JSONAPIDocumentObjectSchema()
 
 
 class JSONAPIResultListSchema(BaseJSONAPIResultSchema):
     """JSON:API list base result schema."""
 
-    data: Sequence[JSONAPIObjectSchema] = Field(description="Список объектов")
+    data: Sequence[JSONAPIObjectSchema] = Field(description="Resource objects collection")
 
 
 class JSONAPIResultDetailSchema(BaseJSONAPIResultSchema):
     """JSON:API base detail schema."""
 
-    data: JSONAPIObjectSchema = Field(description="Данные объекта")
+    data: JSONAPIObjectSchema = Field(description="Resource object data")
 
 
 class BasicPipelineActionSchema(BaseModel):
     """Action schema."""
 
     name: str = Field(default="Default name", description="Человекочитаемое название параметра")
     type: str = Field(default="int", description="Type of a variable")
@@ -110,78 +128,82 @@
             "notlike",
             "notin_",
             "startswith",
         ],
         const=True,
     )
 
-    class Meta(object):
+    class Meta:
         """String parameter schema."""
 
         type = str
 
 
 class IntSchema(BasicPipelineActionSchema):
     """Int parameter schema."""
 
     name: str = Field(default="Число 1")
     type: str = Field(default="int", const=True)
     operation: List[str] = Field(default=["eq", "ne", "gt", "ge", "in_", "lt", "le", "notin_"], const=True)
 
-    class Meta(object):
+    class Meta:
         """Int parameter meta."""
 
         type = int
 
 
 class FloatSchema(BasicPipelineActionSchema):
     """Float parameter schema."""
 
     name: str = Field(default="Процент 1")
     type: str = Field(default="float", const=True)
     operation: List[str] = Field(default=["eq", "ne", "gt", "ge", "in_", "lt", "le", "notin_"], const=True)
 
-    class Meta(object):
+    class Meta:
         """Float parameter schema."""
 
         type = float
 
 
 class BoolSchema(BasicPipelineActionSchema):
     """Boolean action schema."""
 
     name: str = Field(default="Детектор сработал на событие Х")
     type: str = Field(default="bool", const=True)
     operation: List[str] = Field(default=["eq", "is_", "ne"], const=True)
 
-    class Meta(object):
+    class Meta:
         """Boolean parameter meta."""
 
         type = bool
 
 
 def get_model_field(schema: Type["TypeSchema"], field: str) -> str:
     """
     Get the model field of a schema field.
 
-    :param schema: a marshmallow schema
+    :param schema: a pydantic schema
     :param field: the name of the schema field
     :return: the name of the field in the model
     :raises Exception: if the schema from parameter has no attribute for parameter.
     """
     if schema.__fields__.get(field) is None:
-        raise Exception("{schema} has no attribute {field}".format(schema=schema.__name__, field=field))
+        msg = "{schema} has no attribute {field}".format(
+            schema=schema.__name__,
+            field=field,
+        )
+        raise Exception(msg)
     return field
 
 
 def get_relationships(schema: Type["TypeSchema"], model_field: bool = False) -> List[str]:
     """
     Return relationship fields of a schema.
 
-    :param schema: a pydantic schema
+    :param schema: a schemas schema
     :param model_field: list of relationship fields of a schema
     """
     relationships: List[str] = []
     for i_name, i_type in schema.__fields__.items():
         try:
             if issubclass(i_type.type_, BaseModel):
                 relationships.append(i_name)
@@ -203,15 +225,16 @@
     :return Schema: the schema class.
     :raises Exception: if the schema not found for this resource type.
     """
     schemas: Dict[str, Type[BaseModel]] = getattr(app, "schemas", {})
     try:
         return schemas[resource_type]
     except KeyError:
-        raise Exception("Couldn't find schema for type: {type}".format(type=resource_type))
+        msg = "Couldn't find schema for type: {type}".format(type=resource_type)
+        raise Exception(msg)
 
 
 def collect_app_orm_schemas(app: FastAPI) -> None:
     """
     Collect schemas if it has Config->model attributes.
 
     Need for JSON_API.
@@ -222,19 +245,22 @@
     flat_models = get_flat_models_from_routes(app.routes)
     for model in flat_models:
         if not hasattr(model, "Config"):
             continue
         model_type = getattr(getattr(model, "Config"), "model", None)
         if model_type:
             if model_type in models_dict:
-                raise RuntimeError(
-                    "Get duplication value of Config.model={name} for schema={model}. Duplicate in {model_copy}".format(
-                        name=model_type, model=model.__name__, model_copy=models_dict[model_type].__name__
-                    )
+                msg = (
+                    "Get duplication value of Config.model={name} for schema={model}. Duplicate in {model_copy}"
+                ).format(
+                    name=model_type,
+                    model=model.__name__,
+                    model_copy=models_dict[model_type].__name__,
                 )
+                raise RuntimeError(msg)
             models_dict[model_type] = model
     if models_dict:
         setattr(app, "schemas", models_dict)
 
 
 def get_related_schema(schema: Type["TypeSchema"], field: str) -> Type["TypeSchema"]:
     """
```

### Comparing `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/signature.py` & `fastapi_jsonapi-1.0.1/fastapi_jsonapi/signature.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,117 @@
 """Functions for extracting and updating signatures."""
-
+import inspect
+import logging
 from collections import OrderedDict
 from enum import Enum
 from inspect import (
     Parameter,
     Signature,
-    signature,
 )
+from types import GenericAlias
 from typing import (
-    Callable,
+    Any,
     Dict,
     List,
     Optional,
     Set,
+    Tuple,
     Type,
+)
+from typing import (
     OrderedDict as OrderedDictType,
 )
 
 from fastapi import Query
-from pydantic import BaseModel
+from pydantic import BaseModel as BaseModelOriginal
+from pydantic.fields import ModelField
 from starlette.requests import Request
 
 from fastapi_jsonapi.querystring import QueryStringManager
+from fastapi_jsonapi.schema_base import BaseModel, registry
+
+log = logging.getLogger(__name__)
+
+
+def create_filter_parameter(name: str, field: ModelField) -> Parameter:
+    if field.sub_fields:
+        default = Query(None, alias="filter[{alias}]".format(alias=field.alias))
+        type_field = field.type_
+    elif inspect.isclass(field.type_) and issubclass(field.type_, Enum) and hasattr(field.type_, "values"):
+        default = Query(None, alias="filter[{alias}]".format(alias=field.alias), enum=field.type_.values())
+        type_field = str
+    else:
+        default = Query(None, alias="filter[{alias}]".format(alias=field.alias))
+        type_field = field.type_
+
+    return Parameter(
+        name,
+        kind=Parameter.POSITIONAL_OR_KEYWORD,
+        annotation=Optional[type_field],
+        default=default,
+    )
+
+
+def create_additional_query_params(schema: Optional[Type[BaseModel]]) -> tuple[list[Parameter], list[Parameter]]:
+    filter_params = []
+    include_params = []
+    if not schema:
+        return filter_params, include_params
+
+    # TODO! ?
+    schema.update_forward_refs(**registry.schemas)
+    for name, field in (schema.__fields__ or {}).items():
+        try:
+            # skip collections
+            if inspect.isclass(field.type_):
+                if type(field.type_) is GenericAlias:
+                    continue
+                if issubclass(field.type_, (dict, list, tuple, set, Dict, List, Tuple, Set)):
+                    continue
+            # process inner models, find relationships
+            if inspect.isclass(field.type_) and issubclass(field.type_, (BaseModel, BaseModelOriginal)):
+                if field.field_info.extra.get("relationship"):
+                    # TODO?
+                    # build enum?
+                    pass
+                    # parameter = create_include_parameter(name=name, field=field)
+                    # include_params.append(parameter)
+                else:
+                    log.warning(
+                        "found nested schema %s for field %r. Consider marking it as relationship",
+                        field,
+                        name,
+                    )
+                continue
+
+            # create filter params
+            parameter = create_filter_parameter(
+                name=name,
+                field=field,
+            )
+            filter_params.append(parameter)
+        except Exception as ex:
+            log.warning("could not create filter for field %s %s", name, field, exc_info=ex)
+
+    include_param = Parameter(
+        "_jsonapi_include",
+        kind=Parameter.POSITIONAL_OR_KEYWORD,
+        annotation=Optional[str],
+        default=Query(None, alias="include"),
+    )
+    include_params.append(include_param)
+    return filter_params, include_params
 
 
 def update_signature(
-        sig: Signature,
-        schema: Optional[Type[BaseModel]] = None,
-        other: OrderedDictType[str, Parameter] = None,
+    sig: Signature,
+    schema: Optional[Type[BaseModel]] = None,
+    other: OrderedDictType[str, Parameter] = None,
+    exclude_filters: bool = False,
+    return_annotation: Any = None,
 ) -> Signature:
     """
     Add docs parameters to signature.
 
     :params sig: сигнатура декоратора библиотеки wrapper, которая оборачивает изначальную функцию.
     :params schema: которую нужно вставить в сигнатуру.
     :params other: список параметров из начальной функции.
@@ -61,44 +141,17 @@
     params_dict.pop("kwargs", None)
     params_dict.pop("cls", None)
     params_no_default = [
         i_param
         for i_name, i_param in other.items()
         if isinstance(i_param.default, type) and other[i_name].annotation is not QueryStringManager
     ]
-    params_default = [
-        i_param
-        for i_param in other.values()
-        if not isinstance(i_param.default, type)
-    ]
-    params: list = list(params_dict.values())
-    for name, field in (schema and schema.__fields__ or {}).items():
-        try:
-            if issubclass(field.type_, (dict, BaseModel, list, set, List, Set, Dict)):
-                continue
-            elif field.sub_fields:
-                default = Query(None, alias="filter[{alias}]".format(alias=field.alias))
-                type_field = field.type_
-            elif issubclass(field.type_, Enum):
-                default = Query(None, alias="filter[{alias}]".format(alias=field.alias), enum=field.type_.values())
-                type_field = str
-            else:
-                default = Query(None, alias="filter[{alias}]".format(alias=field.alias))
-                type_field = field.type_
-            params.append(
-                Parameter(
-                    name,
-                    kind=Parameter.POSITIONAL_OR_KEYWORD,
-                    annotation=Optional[type_field],
-                    default=default,
-                )
-            )
-        except Exception as ex:
-            pass
-
-    params: list = params + params_no_default + params_default
+    params_default = [i_param for i_param in other.values() if not isinstance(i_param.default, type)]
+    params = list(params_dict.values())
+    filter_params, include_params = create_additional_query_params(schema=schema)
+    params = params + ([] if exclude_filters else filter_params) + include_params + params_no_default + params_default
     # Убираем дубликаты
     params_dict: dict = {i_p.name: i_p for i_p in params}
     params: list = list(params_dict.values())
     params.sort(key=lambda x: not isinstance(x.default, type))
 
-    return sig.replace(parameters=params)
+    return sig.replace(parameters=params, return_annotation=return_annotation or sig.return_annotation)
```

