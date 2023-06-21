# Comparing `tmp/bl_hector-0.1.2.tar.gz` & `tmp/bl_hector-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_hector-0.1.2.tar", max compression
+gzip compressed data, was "bl_hector-0.2.0.tar", max compression
```

## Comparing `bl_hector-0.1.2.tar` & `bl_hector-0.2.0.tar`

### file list

```diff
@@ -1,90 +1,89 @@
--rw-r--r--   0        0        0    34523 2023-06-14 14:53:28.100751 bl_hector-0.1.2/LICENSE
--rw-r--r--   0        0        0     1854 2023-06-14 14:53:28.100751 bl_hector-0.1.2/README.md
--rw-r--r--   0        0        0      807 2023-06-14 14:53:28.100751 bl_hector-0.1.2/bl_hector/__init__.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.1.2/bl_hector/application/__init__.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.1.2/bl_hector/application/use_cases/__init__.py
--rw-r--r--   0        0        0     3803 2023-06-14 14:53:28.100751 bl_hector-0.1.2/bl_hector/application/use_cases/add_book.py
--rw-r--r--   0        0        0     2048 2023-06-14 14:53:28.100751 bl_hector-0.1.2/bl_hector/application/use_cases/display_book.py
--rw-r--r--   0        0        0     1975 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/application/use_cases/look_up_book.py
--rw-r--r--   0        0        0     3751 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/application/use_cases/search_books.py
--rw-r--r--   0        0        0     3801 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/application/use_cases/update_book.py
--rw-r--r--   0        0        0      944 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/configuration/__init__.py
--rw-r--r--   0        0        0      981 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/configuration/cli.py
--rw-r--r--   0        0        0      986 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/configuration/wsgi.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/__init__.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/administration/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/administration/entities.py
--rw-r--r--   0        0        0      808 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/administration/enumerations.py
--rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/administration/repositories.py
--rw-r--r--   0        0        0     1196 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/administration/services.py
--rw-r--r--   0        0        0      931 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/administration/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/__init__.py
--rw-r--r--   0        0        0     1563 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/entities.py
--rw-r--r--   0        0        0      996 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/errors.py
--rw-r--r--   0        0        0     1509 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/repositories.py
--rw-r--r--   0        0        0     1173 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/services.py
--rw-r--r--   0        0        0     1800 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/validators.py
--rw-r--r--   0        0        0     3325 2023-06-14 14:53:28.104751 bl_hector-0.1.2/bl_hector/domain/collection_management/value_objects.py
--rw-r--r--   0        0        0     1453 2023-06-14 14:53:28.108751 bl_hector-0.1.2/bl_hector/infrastructure/__init__.py
--rw-r--r--   0        0        0     3982 2023-06-16 08:33:27.027305 bl_hector-0.1.2/bl_hector/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1064 2023-06-14 14:53:28.108751 bl_hector-0.1.2/bl_hector/infrastructure/flask/aliases/__init__.py
--rw-r--r--   0        0        0     1693 2023-06-14 14:53:28.108751 bl_hector-0.1.2/bl_hector/infrastructure/flask/auth/__init__.py
--rw-r--r--   0        0        0     4282 2023-06-16 08:55:18.414785 bl_hector-0.1.2/bl_hector/infrastructure/flask/books/__init__.py
--rw-r--r--   0        0        0     3466 2023-06-14 14:53:28.108751 bl_hector-0.1.2/bl_hector/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-14 14:53:28.108751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0    73117 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
--rw-r--r--   0        0        0      664 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/css/hector.css
--rw-r--r--   0        0        0      655 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/favicon.svg
--rw-r--r--   0        0        0     1502 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
--rw-r--r--   0        0        0    42819 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0    97249 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
--rw-r--r--   0        0        0     6828 2023-06-14 14:53:28.112751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
--rw-r--r--   0        0        0   186112 2023-06-14 14:53:28.116751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   107460 2023-06-14 14:53:28.116751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    62048 2023-06-14 14:53:28.116751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25096 2023-06-14 14:53:28.116751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   397728 2023-06-14 14:53:28.120751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150472 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     2363 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/flask/totp/__init__.py
--rw-r--r--   0        0        0     1265 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     4544 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/flask/webauthn/__init__.py
--rw-r--r--   0        0        0     3282 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/flask/webauthn/security.py
--rw-r--r--   0        0        0     1789 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/isbnlib/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/requests/__init__.py
--rw-r--r--   0        0        0     2615 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/settings.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     8336 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2058 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/typer/__init__.py
--rw-r--r--   0        0        0     2886 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/typer/books.py
--rw-r--r--   0        0        0     2099 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/infrastructure/typer/services.py
--rw-r--r--   0        0        0     1845 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/interfaces/__init__.py
--rw-r--r--   0        0        0      761 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/interfaces/exceptions.py
--rw-r--r--   0        0        0     3371 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/interfaces/from_dict.py
--rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.124751 bl_hector-0.1.2/bl_hector/interfaces/from_json.py
--rw-r--r--   0        0        0     1435 2023-06-14 14:53:28.128751 bl_hector-0.1.2/bl_hector/interfaces/l10n/__init__.py
--rw-r--r--   0        0        0     4792 2023-06-16 06:26:43.520346 bl_hector-0.1.2/bl_hector/interfaces/l10n/en-GB/main.ftl
--rw-r--r--   0        0        0     5330 2023-06-16 06:26:43.520346 bl_hector-0.1.2/bl_hector/interfaces/l10n/fr-FR/main.ftl
--rw-r--r--   0        0        0     1407 2023-06-14 14:53:28.128751 bl_hector-0.1.2/bl_hector/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0    14822 2023-06-16 08:56:31.481861 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     1247 2023-06-16 06:26:43.520346 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
--rw-r--r--   0        0        0     4288 2023-06-16 09:51:27.024346 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
--rw-r--r--   0        0        0     2116 2023-06-16 09:56:40.596445 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
--rw-r--r--   0        0        0     2043 2023-06-14 14:53:28.128751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug
--rw-r--r--   0        0        0     5680 2023-06-16 09:53:48.126592 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
--rw-r--r--   0        0        0     3628 2023-06-16 09:55:40.101198 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
--rw-r--r--   0        0        0      982 2023-06-14 14:53:28.128751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/error.pug
--rw-r--r--   0        0        0     2028 2023-06-16 06:26:43.520346 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1127 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
--rw-r--r--   0        0        0     4129 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
--rw-r--r--   0        0        0     2008 2023-06-16 08:59:37.299508 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
--rw-r--r--   0        0        0     1678 2023-06-16 06:26:43.524346 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
--rw-r--r--   0        0        0     2010 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
--rw-r--r--   0        0        0     2045 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
--rw-r--r--   0        0        0     1310 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_http/as_json/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_terminal/__init__.py
--rw-r--r--   0        0        0     1885 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_terminal/as_json.py
--rw-r--r--   0        0        0     5280 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/to_terminal/as_text.py
--rw-r--r--   0        0        0     1519 2023-06-14 14:53:28.132751 bl_hector-0.1.2/bl_hector/interfaces/utils.py
--rw-r--r--   0        0        0     1570 2023-06-16 10:00:00.357940 bl_hector-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4676 2023-06-16 10:00:45.217874 bl_hector-0.1.2/setup.py
--rw-r--r--   0        0        0     3048 2023-06-16 10:00:45.218990 bl_hector-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-14 14:53:28.100751 bl_hector-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1854 2023-06-14 14:53:28.100751 bl_hector-0.2.0/README.md
+-rw-r--r--   0        0        0      807 2023-06-14 14:53:28.100751 bl_hector-0.2.0/bl_hector/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.2.0/bl_hector/application/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.2.0/bl_hector/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     3793 2023-06-21 08:04:15.986384 bl_hector-0.2.0/bl_hector/application/use_cases/add_book.py
+-rw-r--r--   0        0        0     2044 2023-06-21 08:04:15.986384 bl_hector-0.2.0/bl_hector/application/use_cases/display_book.py
+-rw-r--r--   0        0        0     1971 2023-06-21 08:04:15.990384 bl_hector-0.2.0/bl_hector/application/use_cases/look_up_book.py
+-rw-r--r--   0        0        0     3729 2023-06-21 08:04:15.990384 bl_hector-0.2.0/bl_hector/application/use_cases/search_books.py
+-rw-r--r--   0        0        0     3793 2023-06-21 08:30:56.399424 bl_hector-0.2.0/bl_hector/application/use_cases/update_book.py
+-rw-r--r--   0        0        0      944 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/configuration/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/configuration/cli.py
+-rw-r--r--   0        0        0      986 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/configuration/wsgi.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/administration/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/administration/entities.py
+-rw-r--r--   0        0        0      808 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/administration/enumerations.py
+-rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/administration/repositories.py
+-rw-r--r--   0        0        0     1196 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/administration/services.py
+-rw-r--r--   0        0        0      931 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/administration/value_objects.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/collection_management/__init__.py
+-rw-r--r--   0        0        0     1511 2023-06-21 08:04:15.990384 bl_hector-0.2.0/bl_hector/domain/collection_management/entities.py
+-rw-r--r--   0        0        0     1505 2023-06-21 08:10:22.593917 bl_hector-0.2.0/bl_hector/domain/collection_management/errors.py
+-rw-r--r--   0        0        0     1509 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/collection_management/repositories.py
+-rw-r--r--   0        0        0     1173 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/collection_management/services.py
+-rw-r--r--   0        0        0     1630 2023-06-21 08:14:45.342810 bl_hector-0.2.0/bl_hector/domain/collection_management/validators.py
+-rw-r--r--   0        0        0     3039 2023-06-21 08:13:37.175610 bl_hector-0.2.0/bl_hector/domain/collection_management/value_objects.py
+-rw-r--r--   0        0        0     1453 2023-06-14 14:53:28.108751 bl_hector-0.2.0/bl_hector/infrastructure/__init__.py
+-rw-r--r--   0        0        0     3547 2023-06-19 10:56:43.740572 bl_hector-0.2.0/bl_hector/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-14 14:53:28.108751 bl_hector-0.2.0/bl_hector/infrastructure/flask/aliases/__init__.py
+-rw-r--r--   0        0        0     1694 2023-06-19 12:33:58.012069 bl_hector-0.2.0/bl_hector/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     4178 2023-06-21 11:13:56.415653 bl_hector-0.2.0/bl_hector/infrastructure/flask/books/__init__.py
+-rw-r--r--   0        0        0     3466 2023-06-14 14:53:28.108751 bl_hector-0.2.0/bl_hector/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-06-14 14:53:28.108751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0    73117 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
+-rw-r--r--   0        0        0      664 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/css/hector.css
+-rw-r--r--   0        0        0      655 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/favicon.svg
+-rw-r--r--   0        0        0     1502 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
+-rw-r--r--   0        0        0    42819 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    97249 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
+-rw-r--r--   0        0        0     6828 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
+-rw-r--r--   0        0        0   186112 2023-06-14 14:53:28.116751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   107460 2023-06-14 14:53:28.116751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    62048 2023-06-14 14:53:28.116751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25096 2023-06-14 14:53:28.116751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   397728 2023-06-14 14:53:28.120751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150472 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     2364 2023-06-19 12:33:06.364676 bl_hector-0.2.0/bl_hector/infrastructure/flask/totp/__init__.py
+-rw-r--r--   0        0        0     1441 2023-06-19 16:02:47.674444 bl_hector-0.2.0/bl_hector/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     4546 2023-06-19 12:33:06.392676 bl_hector-0.2.0/bl_hector/infrastructure/flask/webauthn/__init__.py
+-rw-r--r--   0        0        0     3282 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/flask/webauthn/security.py
+-rw-r--r--   0        0        0     1789 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/isbnlib/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/requests/__init__.py
+-rw-r--r--   0        0        0     2615 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/settings.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     8336 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2058 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/typer/__init__.py
+-rw-r--r--   0        0        0     2886 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/typer/books.py
+-rw-r--r--   0        0        0     2099 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/typer/services.py
+-rw-r--r--   0        0        0     4007 2023-06-21 08:15:27.830313 bl_hector-0.2.0/bl_hector/interfaces/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/interfaces/exceptions.py
+-rw-r--r--   0        0        0     3363 2023-06-21 08:32:45.022087 bl_hector-0.2.0/bl_hector/interfaces/from_dict.py
+-rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/interfaces/from_json.py
+-rw-r--r--   0        0        0     1690 2023-06-19 10:56:43.684572 bl_hector-0.2.0/bl_hector/interfaces/l10n/__init__.py
+-rw-r--r--   0        0        0     5368 2023-06-21 08:27:19.978166 bl_hector-0.2.0/bl_hector/interfaces/l10n/en-GB/main.ftl
+-rw-r--r--   0        0        0     5976 2023-06-21 08:27:28.290073 bl_hector-0.2.0/bl_hector/interfaces/l10n/fr-FR/main.ftl
+-rw-r--r--   0        0        0     2848 2023-06-19 15:46:44.511709 bl_hector-0.2.0/bl_hector/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0    14664 2023-06-21 11:05:08.153809 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1350 2023-06-21 08:04:12.314430 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     4202 2023-06-21 10:59:40.789623 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
+-rw-r--r--   0        0        0     2100 2023-06-21 06:11:25.884842 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
+-rw-r--r--   0        0        0     5740 2023-06-21 10:57:51.862891 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
+-rw-r--r--   0        0        0     3569 2023-06-21 11:17:07.421426 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
+-rw-r--r--   0        0        0      982 2023-06-14 14:53:28.128751 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/error.pug
+-rw-r--r--   0        0        0     2045 2023-06-21 06:11:25.884842 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1127 2023-06-14 14:53:28.132751 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
+-rw-r--r--   0        0        0     4770 2023-06-21 11:06:30.368852 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
+-rw-r--r--   0        0        0     1992 2023-06-21 06:11:25.888841 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
+-rw-r--r--   0        0        0     1845 2023-06-21 06:11:25.888841 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
+-rw-r--r--   0        0        0     2010 2023-06-14 14:53:28.132751 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
+-rw-r--r--   0        0        0     2045 2023-06-14 14:53:28.132751 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
+-rw-r--r--   0        0        0     1310 2023-06-14 14:53:28.132751 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_json/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-14 14:53:28.132751 bl_hector-0.2.0/bl_hector/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1885 2023-06-14 14:53:28.132751 bl_hector-0.2.0/bl_hector/interfaces/to_terminal/as_json.py
+-rw-r--r--   0        0        0     5276 2023-06-21 08:04:15.994384 bl_hector-0.2.0/bl_hector/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1519 2023-06-19 12:33:41.408264 bl_hector-0.2.0/bl_hector/interfaces/utils.py
+-rw-r--r--   0        0        0     1570 2023-06-21 11:22:58.541331 bl_hector-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4606 2023-06-21 11:24:22.577414 bl_hector-0.2.0/setup.py
+-rw-r--r--   0        0        0     3048 2023-06-21 11:24:22.579179 bl_hector-0.2.0/PKG-INFO
```

### Comparing `bl_hector-0.1.2/LICENSE` & `bl_hector-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/README.md` & `bl_hector-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/__init__.py` & `bl_hector-0.2.0/bl_hector/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/application/__init__.py` & `bl_hector-0.2.0/bl_hector/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/application/use_cases/__init__.py` & `bl_hector-0.2.0/bl_hector/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/application/use_cases/add_book.py` & `bl_hector-0.2.0/bl_hector/application/use_cases/add_book.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from typing import Optional
 
 from bl_hector.domain.administration.enumerations import Permissions as P
 from bl_hector.domain.administration.repositories import Permissions
 from bl_hector.domain.administration.value_objects import UserId
 from bl_hector.domain.collection_management import validators
 from bl_hector.domain.collection_management.entities import Book
-from bl_hector.domain.collection_management.errors import IncorrectValue
+from bl_hector.domain.collection_management.errors import InvalidValue
 from bl_hector.domain.collection_management.repositories import Books
 from bl_hector.domain.collection_management.services import Calendar
 from bl_hector.domain.collection_management.value_objects import (
     Author,
     Cover,
     Genre,
     Isbn,
@@ -45,18 +45,18 @@
     authors: list[str]
     genres: list[str]
     cover: str = ""
 
 
 @dataclass
 class Errors:
-    isbn: Optional[IncorrectValue] = None
-    title: Optional[IncorrectValue] = None
-    year: Optional[IncorrectValue] = None
-    authors: Optional[IncorrectValue] = None
+    isbn: Optional[InvalidValue] = None
+    title: Optional[InvalidValue] = None
+    year: Optional[InvalidValue] = None
+    authors: Optional[InvalidValue] = None
 
     def __bool__(self) -> bool:
         return any([getattr(self, f.name) for f in fields(self)])
 
 
 class Presenter(ABC):
     @abstractmethod
```

### Comparing `bl_hector-0.1.2/bl_hector/application/use_cases/display_book.py` & `bl_hector-0.2.0/bl_hector/application/use_cases/display_book.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
 from bl_hector.domain.collection_management.entities import Book
-from bl_hector.domain.collection_management.errors import IncorrectValue
+from bl_hector.domain.collection_management.errors import InvalidValue
 from bl_hector.domain.collection_management.repositories import Books
 from bl_hector.domain.collection_management.value_objects import Isbn
 
 
 @dataclass(frozen=True)
 class Request:
     isbn: str
@@ -50,15 +50,15 @@
 class Interactor:
     presenter: Presenter
     books: Books
 
     def execute(self, request: Request) -> None:
         try:
             isbn = Isbn.instanciate(request.isbn)
-        except IncorrectValue:
+        except InvalidValue:
             return self.presenter.not_an_isbn(request.isbn)
 
         if not (book := self.books.by_isbn(isbn)):
             return self.presenter.book_not_found(isbn)
 
         self.presenter.book(book)
```

### Comparing `bl_hector-0.1.2/bl_hector/application/use_cases/look_up_book.py` & `bl_hector-0.2.0/bl_hector/application/use_cases/look_up_book.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
 from bl_hector.domain.collection_management.entities import Book
-from bl_hector.domain.collection_management.errors import IncorrectValue
+from bl_hector.domain.collection_management.errors import InvalidValue
 from bl_hector.domain.collection_management.services import (
     BookInfoProvider,
     CoverProvider,
 )
 from bl_hector.domain.collection_management.value_objects import Isbn
 
 
@@ -50,15 +50,15 @@
     presenter: Presenter
     info_provider: BookInfoProvider
     cover_provider: CoverProvider
 
     def execute(self, request: Request) -> None:
         try:
             isbn = Isbn.instanciate(request.isbn)
-        except IncorrectValue:
+        except InvalidValue:
             return self.presenter.not_an_isbn(request.isbn)
 
         if not (book := self.info_provider.look_up(isbn)):
             return self.presenter.book_not_found(isbn)
 
         book.cover = self.cover_provider.by_isbn(isbn)
```

### Comparing `bl_hector-0.1.2/bl_hector/application/use_cases/search_books.py` & `bl_hector-0.2.0/bl_hector/application/use_cases/search_books.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, fields
 from typing import Optional
 
 from bl_hector.domain.collection_management.entities import Book
-from bl_hector.domain.collection_management.errors import IncorrectValue
+from bl_hector.domain.collection_management.errors import InvalidValue
 from bl_hector.domain.collection_management.repositories import Books
 from bl_hector.domain.collection_management.value_objects import (
     Author,
     Genre,
     Isbn,
     Title,
     Year,
@@ -39,19 +39,19 @@
     genre: Optional[str] = None
     page_number: Optional[int] = None
     page_size: Optional[int] = None
 
 
 @dataclass
 class Errors:
-    isbn: Optional[IncorrectValue] = None
-    title: Optional[IncorrectValue] = None
-    year: Optional[IncorrectValue] = None
-    author: Optional[IncorrectValue] = None
-    genre: Optional[IncorrectValue] = None
+    isbn: Optional[InvalidValue] = None
+    title: Optional[InvalidValue] = None
+    year: Optional[InvalidValue] = None
+    author: Optional[InvalidValue] = None
+    genre: Optional[InvalidValue] = None
 
     def __bool__(self) -> bool:
         return any([getattr(self, f.name) for f in fields(self)])
 
 
 class Presenter(ABC):
     @abstractmethod
@@ -85,30 +85,30 @@
             self.presenter.book(book)
 
     def __validate_request(self, request: Request) -> Errors:
         errors = Errors()
         if request.isbn:
             try:
                 Isbn.instanciate(request.isbn)
-            except IncorrectValue as exc:
+            except InvalidValue as exc:
                 errors.isbn = exc
         if request.title:
             try:
                 Title.instanciate(request.title)
-            except IncorrectValue as exc:
+            except InvalidValue as exc:
                 errors.title = exc
         if request.year is not None:
             try:
                 Year.instanciate(request.year)
-            except IncorrectValue as exc:
+            except InvalidValue as exc:
                 errors.year = exc
         if request.author:
             try:
                 Author.instanciate(request.author)
-            except IncorrectValue as exc:
+            except InvalidValue as exc:
                 errors.author = exc
         if request.genre:
             try:
                 Genre.instanciate(request.genre)
-            except IncorrectValue as exc:
+            except InvalidValue as exc:
                 errors.genre = exc
         return errors
```

### Comparing `bl_hector-0.1.2/bl_hector/application/use_cases/update_book.py` & `bl_hector-0.2.0/bl_hector/application/use_cases/update_book.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from typing import Optional
 
 from bl_hector.domain.administration.enumerations import Permissions as P
 from bl_hector.domain.administration.repositories import Permissions
 from bl_hector.domain.administration.value_objects import UserId
 from bl_hector.domain.collection_management import validators
 from bl_hector.domain.collection_management.entities import Book
-from bl_hector.domain.collection_management.errors import IncorrectValue
+from bl_hector.domain.collection_management.errors import InvalidValue
 from bl_hector.domain.collection_management.repositories import Books
 from bl_hector.domain.collection_management.services import Calendar
 from bl_hector.domain.collection_management.value_objects import (
     Author,
     Cover,
     Genre,
     Isbn,
@@ -45,17 +45,17 @@
     authors: list[str]
     genres: list[str]
     cover: str = ""
 
 
 @dataclass
 class Errors:
-    title: Optional[IncorrectValue] = None
-    year: Optional[IncorrectValue] = None
-    authors: Optional[IncorrectValue] = None
+    title: Optional[InvalidValue] = None
+    year: Optional[InvalidValue] = None
+    authors: Optional[InvalidValue] = None
 
     def __bool__(self) -> bool:
         return any([getattr(self, f.name) for f in fields(self)])
 
 
 class Presenter(ABC):
     @abstractmethod
```

### Comparing `bl_hector-0.1.2/bl_hector/configuration/__init__.py` & `bl_hector-0.2.0/bl_hector/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/configuration/cli.py` & `bl_hector-0.2.0/bl_hector/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/configuration/wsgi.py` & `bl_hector-0.2.0/bl_hector/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/domain/__init__.py` & `bl_hector-0.2.0/bl_hector/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/domain/administration/__init__.py` & `bl_hector-0.2.0/bl_hector/domain/administration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/domain/administration/entities.py` & `bl_hector-0.2.0/bl_hector/domain/administration/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/domain/administration/enumerations.py` & `bl_hector-0.2.0/bl_hector/domain/administration/enumerations.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/domain/administration/repositories.py` & `bl_hector-0.2.0/bl_hector/domain/administration/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/domain/administration/services.py` & `bl_hector-0.2.0/bl_hector/domain/administration/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/domain/administration/value_objects.py` & `bl_hector-0.2.0/bl_hector/domain/administration/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/domain/collection_management/__init__.py` & `bl_hector-0.2.0/bl_hector/domain/collection_management/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/domain/collection_management/entities.py` & `bl_hector-0.2.0/bl_hector/domain/collection_management/entities.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
 from typing import Optional
 
-from .errors import IncorrectValue
+from .errors import MissingAuthor
 from .value_objects import Author, Cover, Date, Genre, Isbn, Title, Year
 
 
 @dataclass
 class Book:
     added_on: Date
     updated_on: Date
@@ -41,9 +41,9 @@
         title: Title,
         year: Year,
         authors: list[Author],
         genres: list[Genre],
         cover: Optional[Cover] = None,
     ) -> "Book":
         if not authors:
-            raise IncorrectValue("authors", "A book must have at least one author!")
+            raise MissingAuthor()
         return Book(added_on, updated_on, isbn, title, year, authors, genres, cover)
```

### Comparing `bl_hector-0.1.2/bl_hector/domain/collection_management/errors.py` & `bl_hector-0.2.0/bl_hector/infrastructure/sqlalchemy/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,22 +9,7 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
-
-
-class Error(Exception):
-    pass
-
-
-class IncorrectValue(Error):
-    def __init__(self, name: str, message: str) -> None:
-        self.name = name
-        self.message = message
-
-
-class UnknownBook(Error):
-    def __init__(self, isbn: str) -> None:
-        self.isbn = isbn
```

### Comparing `bl_hector-0.1.2/bl_hector/domain/collection_management/repositories.py` & `bl_hector-0.2.0/bl_hector/domain/collection_management/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/domain/collection_management/services.py` & `bl_hector-0.2.0/bl_hector/domain/collection_management/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/domain/collection_management/validators.py` & `bl_hector-0.2.0/bl_hector/domain/collection_management/validators.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,46 +12,43 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Optional
 
-from .errors import IncorrectValue
+from .errors import InvalidValue, MissingAuthor
 from .value_objects import Author, Isbn, Title, Year
 
 
-def isbn(value: str) -> Optional[IncorrectValue]:
+def isbn(value: str) -> Optional[InvalidValue]:
     try:
         Isbn.instanciate(value)
-    except IncorrectValue as exc:
+    except InvalidValue as exc:
         return exc
     return None
 
 
-def title(value: str) -> Optional[IncorrectValue]:
+def title(value: str) -> Optional[InvalidValue]:
     try:
         Title.instanciate(value)
-    except IncorrectValue as exc:
+    except InvalidValue as exc:
         return exc
     return None
 
 
-def year(value: int) -> Optional[IncorrectValue]:
+def year(value: int) -> Optional[InvalidValue]:
     try:
         Year.instanciate(value)
-    except TypeError:
-        # FIXME: This should be dealt with in the value object.
-        return IncorrectValue("year", "TypeError")
-    except IncorrectValue as exc:
+    except InvalidValue as exc:
         return exc
     return None
 
 
-def authors(value: list[str]) -> Optional[IncorrectValue]:
+def authors(value: list[str]) -> Optional[InvalidValue]:
     try:
         # FIXME: This domain constraint should live in the domain!
         if len([Author.instanciate(a) for a in value if a]) == 0:
-            raise IncorrectValue("authors", "Cannot be empty!")
-    except IncorrectValue as exc:
+            raise MissingAuthor()
+    except InvalidValue as exc:
         return exc
     return None
```

### Comparing `bl_hector-0.1.2/bl_hector/domain/collection_management/value_objects.py` & `bl_hector-0.2.0/bl_hector/domain/collection_management/value_objects.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,62 +16,52 @@
 
 import datetime
 from typing import Type
 
 import bl3d
 from isbnlib import is_isbn13, mask
 
-from bl_hector.domain.collection_management.errors import IncorrectValue
+from bl_hector.domain.collection_management import errors
 
 
 class String(bl3d.String):
     @classmethod
     def instanciate(cls: Type[bl3d.TypeString], value: str) -> bl3d.TypeString:
-        try:
-            return super().instanciate(value)
-        except bl3d.InvalidValue as exc:
-            raise IncorrectValue(cls.__name__, str(exc).split(":", 1)[1])
+        return super().instanciate(value)
 
 
 class Integer(bl3d.Integer):
     @classmethod
     def instanciate(cls: Type[bl3d.TypeInteger], value: int) -> bl3d.TypeInteger:
-        try:
-            return super().instanciate(value)
-        except bl3d.InvalidValue as exc:
-            raise IncorrectValue(cls.__name__, str(exc).split(":", 1)[1])
+        return super().instanciate(value)
 
 
 class Date(bl3d.Date):
     @classmethod
     def instanciate(cls: Type[bl3d.TypeDate], value: datetime.date) -> bl3d.TypeDate:
-        try:
-            return super().instanciate(value)
-        except bl3d.InvalidValue as exc:
-            raise IncorrectValue(cls.__name__, str(exc).split(":", 1)[1])
+        return super().instanciate(value)
 
 
 class Isbn(String):
     """
     The International Standard Book Number (ISBN) of a book,
     for instance 978-0-7653-9277-0.
     """
 
     MIN = 13
     MAX = 17  # 13 numbers plus 4 `-` for masked ISBN
 
     @classmethod
     def instanciate(cls, value: str) -> "Isbn":
-        __value = value.replace("-", "")
+        super().instanciate(value)
 
-        super().instanciate(__value)
+        __value = value.replace("-", "")
         if is_isbn13(__value):
             return cls(__value)
-
-        raise IncorrectValue(cls.__name__, "This value doesn't look like an ISBN-13.")
+        raise errors.NotAnIsbn(__value)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(value={self})"
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Isbn):
             return NotImplemented
@@ -106,12 +96,18 @@
 class Genre(String):
     MIN = 1
     MAX = 64
 
 
 class Year(Integer):
     # Books published before the introduction of the ISBN system can have an ISBN!
-    MIN = 1900
+    MIN = 1970
+
+    @classmethod
+    def instanciate(cls, value: int) -> "Year":
+        if value < cls.MIN:
+            raise errors.BeforeCreationOfIsbn(cls.MIN)
+        return cls(value)
 
 
 class Cover(String):
     MIN = 1
```

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/__init__.py` & `bl_hector-0.2.0/bl_hector/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/__init__.py` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,29 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from http import HTTPStatus as HTTP
 from typing import Any
 
-from flask import Flask, Response, g, get_flashed_messages, request, url_for
+from flask import Flask, g, get_flashed_messages, request, url_for
 from werkzeug.middleware.proxy_fix import ProxyFix
 
 from bl_hector import __version__
 from bl_hector.infrastructure.flask import services
 from bl_hector.infrastructure.flask.aliases import blueprint as aliases
 from bl_hector.infrastructure.flask.auth import blueprint as auth
 from bl_hector.infrastructure.flask.books import blueprint as books
 from bl_hector.infrastructure.flask.utils import presenter_to_response
 from bl_hector.infrastructure.settings import WsgiSettings
 from bl_hector.interfaces import l10n
 from bl_hector.interfaces.exceptions import BadRequest
-from bl_hector.interfaces.to_http.as_html import JinjaPresenter
+from bl_hector.interfaces.to_http import as_html
 
 
 def build_app(settings: WsgiSettings) -> Flask:
     services.define_settings(settings)
 
     app = Flask(__name__)
 
@@ -53,28 +52,18 @@
 
     @app.before_request
     def guess_locale() -> None:
         g.locale = (
             request.accept_languages.best_match(l10n.LOCALES) or l10n.DEFAULT_LOCALE
         )
 
-    @app.after_request
-    def disable_cache_for_htmx_requests(response: Response) -> Response:
-        if "Hx-Target" in request.headers:
-            response.headers["Cache-Control"] = "no-store, max-age=0"
-        return response
-
     @app.errorhandler(BadRequest)  # type: ignore[type-var]
     @presenter_to_response
     def handle_bad_request(e: Exception) -> Any:
-        presenter = JinjaPresenter(
-            "error",
-            message="You submitted a bad request! This should have never happened!?",
-        )
-        presenter.set_status_code(HTTP.BAD_REQUEST)
+        presenter = as_html.BadRequest(user=services.get_user())
         return presenter
 
     return app
 
 
 def register_blueprints(app: Flask, settings: WsgiSettings) -> None:
     app.register_blueprint(aliases, url_prefix="/")
```

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/aliases/__init__.py` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/auth/__init__.py` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/auth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 @presenter_to_response
 def login() -> Any:
     auth_links = current_app.auth_links  # type: ignore[attr-defined]
     if not auth_links:
         return Redirection(url_for("aliases.root"))
     if len(auth_links) == 1:
         return Redirection(url_for(auth_links[0]["route"]))
-    return as_html.JinjaPresenter(
+    return as_html.SimplePresenter(
         "auth/login", links=auth_links, user=services.get_user()
     )
 
 
 @blueprint.get("/logout")
 @presenter_to_response
 def logout() -> Any:
```

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/books/__init__.py` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/books/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     add_book,
     display_book,
     look_up_book,
     search_books,
     update_book,
 )
 from bl_hector.infrastructure.flask import services
-from bl_hector.infrastructure.flask.utils import presenter_to_response
+from bl_hector.infrastructure.flask.utils import htmx, presenter_to_response
 from bl_hector.interfaces import from_dict as controllers
 from bl_hector.interfaces.to_http import as_html as presenters
 
 blueprint = Blueprint("books", __name__)
 
 
 def notify(message: str, type: str) -> None:
@@ -38,39 +38,45 @@
     flash(message, type)
 
 
 @blueprint.get("")
 @presenter_to_response
 def search() -> Any:
     presenter = presenters.SearchBooks(
-        request.args,
-        fragment=request.headers.get("HX-Target", ""),
-        user=services.get_user(),
+        request.args, htmx(request).target, user=services.get_user()
     )
     interactor = search_books.Interactor(presenter, services.get_books())
-    controller = controllers.SearchBooks(
-        request.args, page_size=presenters.SearchBooks.PAGE_SIZE
-    )
+    controller = controllers.SearchBooks(request.args)
     controller.call(interactor)
     return presenter
 
 
+@blueprint.post("@<string:attribute>")
+@presenter_to_response
+def validate(attribute: str) -> Any:
+    return presenters.ValidateBook(
+        attribute, request.form.get(attribute, ""), user=services.get_user()
+    )
+
+
 @blueprint.get("__new__")
 @presenter_to_response
 def add() -> Any:
-    return presenters.AddBook(request.form, user=services.get_user())
+    return presenters.AddBook(
+        request.form, htmx(request).target, notify, user=services.get_user()
+    )
 
 
 @blueprint.post("__new__")
 @presenter_to_response
 def add_POST() -> Any:
     presenter = presenters.AddBook(
         request.form,
-        notify=notify,
-        fragment=request.headers.get("HX-Target", ""),
+        htmx(request).target,
+        notify,
         user=services.get_user(),
     )
     interactor = add_book.Interactor(
         presenter,
         services.get_books(),
         services.get_calendar(),
         services.get_permissions(),
@@ -90,49 +96,37 @@
     interactor.execute(look_up_book.Request(request.form.get("isbn", "")))
     return presenter
 
 
 @blueprint.get("<string:isbn>")
 @presenter_to_response
 def display(isbn: str) -> Any:
-    presenter = presenters.DisplayBook(notify=notify, user=services.get_user())
+    presenter = presenters.DisplayBook(notify, user=services.get_user())
     interactor = display_book.Interactor(presenter, services.get_books())
     interactor.execute(display_book.Request(isbn))
     return presenter
 
 
-@blueprint.get("<string:isbn>/__edit__")
+@blueprint.get("<string:isbn>/__update__")
 @presenter_to_response
 def update(isbn: str) -> Any:
-    presenter = presenters.DisplayBookToUpdate(
-        isbn, notify=notify, user=services.get_user()
-    )
+    presenter = presenters.DisplayBookToUpdate(isbn, notify, user=services.get_user())
     interactor = display_book.Interactor(presenter, services.get_books())
     interactor.execute(display_book.Request(isbn))
     return presenter
 
 
-@blueprint.post("<string:isbn>/__edit__")
+@blueprint.post("<string:isbn>/__update__")
 @presenter_to_response
 def update_POST(isbn: str) -> Any:
     presenter = presenters.UpdateBook(
-        isbn,
-        request.form,
-        notify=notify,
-        fragment=request.headers.get("HX-Target", ""),
-        user=services.get_user(),
+        isbn, request.form, htmx(request).target, notify, user=services.get_user()
     )
     interactor = update_book.Interactor(
         presenter,
         services.get_books(),
         services.get_calendar(),
         services.get_permissions(),
     )
     controller = controllers.UpdateBook(isbn, request.form, str(services.get_user().id))
     controller.call(interactor)
     return presenter
-
-
-@blueprint.post("@isbn")
-@presenter_to_response
-def validate_isbn() -> Any:
-    return presenters.ValidateIsbn(request.form, user=services.get_user())
```

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/services.py` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/css/hector.css` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/css/hector.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/favicon.svg` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/totp/__init__.py` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/totp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 blueprint = Blueprint("totp", __name__)
 
 
 @blueprint.get("/login")
 @presenter_to_response
 def login() -> Any:
-    return as_html.JinjaPresenter("totp/login", user=services.get_user())
+    return as_html.SimplePresenter("totp/login", user=services.get_user())
 
 
 @blueprint.post("/login")
 @presenter_to_response
 def login_POST() -> Any:
     # TOTP settings must be defined for this route to be accessible.
     # Other alternatives: 1) check presence with `if` or 2) ignore type.
```

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/utils.py` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,32 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+from dataclasses import dataclass
 from functools import wraps
 from typing import Any, Callable
 
-from flask import Response
+from flask import Request, Response
 
 from bl_hector.interfaces.to_http import HttpPresenter
 
 
+@dataclass
+class Htmx:
+    target: str
+
+
+def htmx(request: Request) -> Htmx:
+    return Htmx(request.headers.get("Hx-Target", ""))
+
+
 def presenter_to_response(f: Callable[..., HttpPresenter]) -> Callable[[], Response]:
     @wraps(f)
     def decorated_function(*args: Any, **kwargs: Any) -> Response:
         presenter = f(*args, **kwargs)
         return Response(
             status=presenter.status_code(),
             headers=presenter.headers(),
```

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/webauthn/__init__.py` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/webauthn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     if not (credentials := services.get_credentials().for_user(user)):
         return Redirection(url_for("webauthn.register"))
 
     challenge = create_challenge_for(user)
     services.get_challenges().add(challenge)
 
-    return as_html.JinjaPresenter(
+    return as_html.SimplePresenter(
         "webauthn/login",
         user=services.get_user(),
         options=security.authentication_options(
             services.get_relying_party(), user, credentials, challenge
         ),
     )
 
@@ -90,15 +90,15 @@
 
     if services.get_credentials().for_user(user):
         return Redirection(url_for("webauthn.login"))
 
     challenge = create_challenge_for(user)
     services.get_challenges().add(challenge)
 
-    return as_html.JinjaPresenter(
+    return as_html.SimplePresenter(
         "webauthn/register",
         user=services.get_user(),
         options=security.credential_creation_options(
             services.get_relying_party(), user, challenge
         ),
     )
```

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/flask/webauthn/security.py` & `bl_hector-0.2.0/bl_hector/infrastructure/flask/webauthn/security.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/isbnlib/__init__.py` & `bl_hector-0.2.0/bl_hector/infrastructure/isbnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/requests/__init__.py` & `bl_hector-0.2.0/bl_hector/infrastructure/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/settings.py` & `bl_hector-0.2.0/bl_hector/infrastructure/settings.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/sqlalchemy/__init__.py` & `bl_hector-0.2.0/bl_hector/interfaces/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,7 +9,11 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
+
+
+class BadRequest(Exception):
+    pass
```

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/sqlalchemy/repositories.py` & `bl_hector-0.2.0/bl_hector/infrastructure/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/typer/__init__.py` & `bl_hector-0.2.0/bl_hector/infrastructure/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/typer/books.py` & `bl_hector-0.2.0/bl_hector/infrastructure/typer/books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/infrastructure/typer/services.py` & `bl_hector-0.2.0/bl_hector/infrastructure/typer/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/__init__.py` & `bl_hector-0.2.0/bl_hector/interfaces/from_json.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,46 +10,40 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from dataclasses import dataclass
-from typing import Any, Optional
+import json
+import logging
+
+from bl_hector.application.use_cases import add_book
 
-from bl_hector.domain.administration.enumerations import Permissions
-from bl_hector.domain.collection_management import errors
-from bl_hector.interfaces.l10n import Translator
-
-
-@dataclass
-class User:
-    id: str
-    locale: str
-    permissions: list[Permissions]
-
-    def __getattribute__(self, name: str) -> Any:
-        PREFIX = "can_"
-        if name.startswith(PREFIX):
-            return self.has_permission(name[len(PREFIX) :].upper())
-        return super().__getattribute__(name)
-
-    def has_permission(self, permission: str) -> bool:
-        if not self.id:
-            return False
-        try:
-            return Permissions[permission] in self.permissions
-        except KeyError:
-            return False
 
+class AddBook:
+    def __init__(self, data: str, user_id: str = "") -> None:
+        self.__data = data
+        self.__user_id = user_id
 
-def translate_error(
-    translator: Translator, error: Optional[errors.IncorrectValue] = None
-) -> str:
-    if not error:
-        return ""
-
-    # Dispatching errors based on class is not very LSP!?
-    if isinstance(error, errors.IncorrectValue):
-        return translator("incorrect-value")
-    return translator("unknown-error")
+    def call(self, interactor: add_book.Interactor) -> None:
+        if not self.__data:
+            return
+
+        try:
+            data = json.loads(self.__data)
+        except Exception as exc:
+            logging.error(f"AddBook: {exc}")
+            logging.exception(exc)
+            data = {}
+
+        interactor.execute(
+            add_book.Request(
+                user_id=self.__user_id,
+                isbn=str(data.get("isbn", "")),
+                title=str(data.get("title", "")),
+                year=int(data.get("year", "0")),
+                authors=data.get("authors", []),
+                genres=data.get("genres", []),
+                cover=str(data.get("cover", "")),
+            )
+        )
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/from_dict.py` & `bl_hector-0.2.0/bl_hector/interfaces/from_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,30 +15,29 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Any, Optional
 
 from werkzeug.datastructures import MultiDict
 
 from bl_hector.application.use_cases import add_book, search_books, update_book
+from bl_hector.interfaces import Pager
 from bl_hector.interfaces.exceptions import BadRequest
 
 
 class SearchBooks:
-    def __init__(
-        self, data: MultiDict[str, Any], /, *, page_size: Optional[int] = None
-    ) -> None:
+    def __init__(self, data: MultiDict[str, Any]) -> None:
         self.__do_search = bool(data)
         self.request = search_books.Request(
             isbn=str(v) if (v := data.get("isbn")) else None,
             title=str(v) if (v := data.get("title")) else None,
             year=int(v) if (v := data.get("year")) else None,
             author=str(v) if (v := data.get("author")) else None,
             genre=str(v) if (v := data.get("genre")) else None,
             page_number=int(v) if (v := data.get("page")) else 1,
-            page_size=page_size,
+            page_size=Pager.PAGE_SIZE,
         )
 
     def call(self, interactor: search_books.Interactor) -> None:
         if self.__do_search:
             interactor.execute(self.request)
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/from_json.py` & `bl_hector-0.2.0/bl_hector/interfaces/to_terminal/as_json.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,39 +11,42 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import json
-import logging
+from typing import Callable
 
-from bl_hector.application.use_cases import add_book
+from bl_hector.domain.collection_management.entities import Book
+from bl_hector.domain.collection_management.value_objects import Isbn
+from bl_hector.interfaces.to_terminal import ExitCodes, LookUpBookInterface
+
+
+class LookUpBook(LookUpBookInterface):
+    def __init__(self, printer: Callable[[str], None]) -> None:
+        self.__printer = printer
+        self.__exit_code = ExitCodes.USAGE
+
+    def not_an_isbn(self, isbn: str) -> None:
+        self.__exit_code = ExitCodes.BAD_REQUEST
+
+    def book_not_found(self, isbn: Isbn) -> None:
+        self.__exit_code = ExitCodes.NOT_FOUND
+
+    def book(self, book: Book) -> None:
+        self.__exit_code = ExitCodes.OK
+        data = {
+            "isbn": str(book.isbn),
+            "title": str(book.title),
+            "year": int(book.year),
+            "authors": [str(b) for b in book.authors],
+        }
+        if book.genres:
+            data["genres"] = [str(g) for g in book.genres]
+        if book.cover:
+            data["cover"] = str(book.cover)
 
+        self.__printer(json.dumps(data))
 
-class AddBook:
-    def __init__(self, data: str, user_id: str = "") -> None:
-        self.__data = data
-        self.__user_id = user_id
-
-    def call(self, interactor: add_book.Interactor) -> None:
-        if not self.__data:
-            return
-
-        try:
-            data = json.loads(self.__data)
-        except Exception as exc:
-            logging.error(f"AddBook: {exc}")
-            logging.exception(exc)
-            data = {}
-
-        interactor.execute(
-            add_book.Request(
-                user_id=self.__user_id,
-                isbn=str(data.get("isbn", "")),
-                title=str(data.get("title", "")),
-                year=int(data.get("year", "0")),
-                authors=data.get("authors", []),
-                genres=data.get("genres", []),
-                cover=str(data.get("cover", "")),
-            )
-        )
+    def exit_code(self) -> int:
+        return self.__exit_code.value
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/l10n/__init__.py` & `bl_hector-0.2.0/bl_hector/interfaces/l10n/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,7 +34,16 @@
         return message_id
 
 
 def localization(locale: str) -> FluentLocalization:
     if locale not in LOCALES:
         raise RuntimeError(f"Locale `{locale}` is not defined!")
     return FluentLocalization([locale] + LOCALES, ["main.ftl"], LOADER)
+
+
+def translator_for(locale: str = DEFAULT_LOCALE) -> Translator:
+    l10n = localization(locale or DEFAULT_LOCALE)
+
+    def translate(message_id: str, **kwargs: Any) -> str:
+        return str(l10n.format_value(message_id, kwargs))
+
+    return translate
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/l10n/en-GB/main.ftl` & `bl_hector-0.2.0/bl_hector/interfaces/l10n/en-GB/main.ftl`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 # name (string) The name of the information to display
 # value (string) The value of the information to display
 info-line = { $name }: { $value }
 
 access-forbidden = Access forbidden!
 access-not-authorized = Access unauthorised!
 an-error-occurred = An error occurred!
+bad-request = You submitted a bad request! This should have never happened!?
 
 # date (Date) A date to format
 date = { $date }
 
 book = book
 books = books
 book-added-on = added on
@@ -58,15 +59,27 @@
 book-genre-description = One of the genres the book belongs to.
 book-genres = genres
 book-genres-description = The list of genres the book belongs to, comma separated.
 
 unknown-error = An unknown error has occurred!
 mandatory-value = This value is mandatory!
 incorrect-value = Incorrect value!
+# min (int) The minimum length
+string-too-short = The minimal length is { $min }.
+# max (int) The maximum length
+string-too-long = The maximal length is { $max }.
+# min (float) The minimum value
+number-too-small = The minimal value is { $min }.
+# max (float) The maximum value
+number-too-big = The maximal value is { $max }.
+unknown-book = Unknown book
 not-an-isbn = This is not an ISBN!
+missing-author = A book must have an author.
+# year (int) The year of creation
+before-creation-of-isbn = ISBN system was introduced in { $year }.
 
 auth-login-title = Log in
 # method (string) The sign in method
 auth-login-method = Sign in using { $method }
 
 webauthn-register-title = Device registration
 webauthn-register-description = Your browser should be asking you to tap your security device…
```

#### html2text {}

```diff
@@ -12,51 +12,58 @@
 (string) The years the copyright applies to. # holders (string) The names of
 the copyright holders. copyright = Version { $version } Â© { $years }
 { $holders }. # name (string) The name of the license. # url (string) The URL
 of the license file. license = Code is licensed under {_$name_}. # name
 (string) The name of the information to display # value (string) The value of
 the information to display info-line = { $name }: { $value } access-forbidden =
 Access forbidden! access-not-authorized = Access unauthorised! an-error-
-occurred = An error occurred! # date (Date) A date to format date = { $date }
+occurred = An error occurred! bad-request = You submitted a bad request! This
+should have never happened!? # date (Date) A date to format date = { $date }
 book = book books = books book-added-on = added on book-updated-on = update on
 book-isbn = ISBN book-isbn-description = The ISBN assigned to the book, for
 instance 978-0-7653-9277-0. book-title = title book-title-description = The
 title of the book. book-year = year book-year-description = The year the book
 was published in. book-author = author book-author-description = One of the
 authors of the book. book-authors = authors book-authors-description = The list
 of authors of the book, comma separated. book-genre = genre book-genre-
 description = One of the genres the book belongs to. book-genres = genres book-
 genres-description = The list of genres the book belongs to, comma separated.
 unknown-error = An unknown error has occurred! mandatory-value = This value is
-mandatory! incorrect-value = Incorrect value! not-an-isbn = This is not an
-ISBN! auth-login-title = Log in # method (string) The sign in method auth-
-login-method = Sign in using { $method } webauthn-register-title = Device
-registration webauthn-register-description = Your browser should be asking you
-to tap your security deviceâ¦ webauthn-register-success = Your security device
-has been succesfully registered! webauthn-register-failure = Your security
-device could not be registered!? webauthn-login-title = Log in webauthn-login-
-description = Your browser should be asking you to tap your security deviceâ¦
-webauthn-login-failure = You couldn't be logged in!? totp-login-title = Log in
-totp-login-description = Please enter your one-time password. totp-login-
-password = Password totp-login-pattern = An TOTP code is made up of 6 digits.
-totp-login-action = Log in add-book-requires-authentification = You must be
-authenticated before adding a book! add-book-title = Add a new book to the
-collection add-book-action = Add a book add-book-cancel = Cancel add-book-add =
-Add add-book-cover-help = Click to upload a cover add-book-cover-format-not-
-supported = The format of this cover is not supported! search-books-title =
-Search for a book search-books-action = Look up book search-books-clear = Clear
-search-books-search = Search search-books-no-result = No matching book! search-
-books-previous-page = Previous search-books-next-page = Next # title (string)
-The title of the book display-book-title = Details for "{ $title }" update-
-book-requires-authentification = You must be authenticated before editing a
-book! # isbn (string) The ISBN of the book update-book-title = Edit information
-for `{ $isbn }` update-book-action = Edit update-book-failure = Book cannot be
-updated! update-book-success = Book has been updated! update-book-cancel =
-Cancel update-book-update = Save update-book-cover-help = Click to upload a new
-cover update-book-cover-format-not-supported = The format of this cover is not
-supported! book-already-exists = Book already in the collection! # isbn
-(string) The ISBN of the book # url (string) The URL of the book book-added-
-html = Book {_$isbn_} successfully added! # isbn (string) The ISBN of the book
-book-added-text = Book { $isbn } successfully added! book-added = Book {_$isbn
-} successfully added! book-not-found = Book not found! book-cannot-be-added =
-The book cannot be added! books-cannot-be-found = The search cannot be
-performed!
+mandatory! incorrect-value = Incorrect value! # min (int) The minimum length
+string-too-short = The minimal length is { $min }. # max (int) The maximum
+length string-too-long = The maximal length is { $max }. # min (float) The
+minimum value number-too-small = The minimal value is { $min }. # max (float)
+The maximum value number-too-big = The maximal value is { $max }. unknown-book
+= Unknown book not-an-isbn = This is not an ISBN! missing-author = A book must
+have an author. # year (int) The year of creation before-creation-of-isbn =
+ISBN system was introduced in { $year }. auth-login-title = Log in # method
+(string) The sign in method auth-login-method = Sign in using { $method }
+webauthn-register-title = Device registration webauthn-register-description =
+Your browser should be asking you to tap your security deviceâ¦ webauthn-
+register-success = Your security device has been succesfully registered!
+webauthn-register-failure = Your security device could not be registered!?
+webauthn-login-title = Log in webauthn-login-description = Your browser should
+be asking you to tap your security deviceâ¦ webauthn-login-failure = You
+couldn't be logged in!? totp-login-title = Log in totp-login-description =
+Please enter your one-time password. totp-login-password = Password totp-login-
+pattern = An TOTP code is made up of 6 digits. totp-login-action = Log in add-
+book-requires-authentification = You must be authenticated before adding a
+book! add-book-title = Add a new book to the collection add-book-action = Add a
+book add-book-cancel = Cancel add-book-add = Add add-book-cover-help = Click to
+upload a cover add-book-cover-format-not-supported = The format of this cover
+is not supported! search-books-title = Search for a book search-books-action =
+Look up book search-books-clear = Clear search-books-search = Search search-
+books-no-result = No matching book! search-books-previous-page = Previous
+search-books-next-page = Next # title (string) The title of the book display-
+book-title = Details for "{ $title }" update-book-requires-authentification =
+You must be authenticated before editing a book! # isbn (string) The ISBN of
+the book update-book-title = Edit information for `{ $isbn }` update-book-
+action = Edit update-book-failure = Book cannot be updated! update-book-success
+= Book has been updated! update-book-cancel = Cancel update-book-update = Save
+update-book-cover-help = Click to upload a new cover update-book-cover-format-
+not-supported = The format of this cover is not supported! book-already-exists
+= Book already in the collection! # isbn (string) The ISBN of the book # url
+(string) The URL of the book book-added-html = Book {_$isbn_} successfully
+added! # isbn (string) The ISBN of the book book-added-text = Book { $isbn }
+successfully added! book-added = Book {_$isbn_} successfully added! book-not-
+found = Book not found! book-cannot-be-added = The book cannot be added! books-
+cannot-be-found = The search cannot be performed!
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/l10n/fr-FR/main.ftl` & `bl_hector-0.2.0/bl_hector/interfaces/l10n/fr-FR/main.ftl`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 # name (string) The name of the information to display
 # value (string) The value of the information to display
 info-line = { $name } : { $value }
 
 access-forbidden = Accès interdit !
 access-not-authorized = Accès non authorisé !
 an-error-occurred = Une erreur s'est produite !
+bad-request = Vous avez soumis une mauvaise requête ! Cela n'aurait jamais dû arriver !?
 
 # date (Date) A date to format
 date = { $date }
 
 book = livre
 books = livres
 book-added-on = ajouté le
@@ -58,15 +59,27 @@
 book-genre-description = Un des genres auxquels le livre se rattache.
 book-genres = genres
 book-genres-description = La liste des genres auxquels le livre se rattache, séparés par des virgules.
 
 unknown-error = Une erreur inconnue s'est produite !
 mandatory-value = Cette valeur est obligatoire !
 incorrect-value = Cette valeur est incorrecte !
+# min (int) The minimum length
+string-too-short = La longueur minimale est { $min }.
+# max (int) The maximum length
+string-too-long = La longueur maximale est { $max }.
+# min (float) The minimum value
+number-too-small = La valeur minimale est { $min }.
+# max (float) The maximum value
+number-too-big = La valeur maximale est { $max }.
+unknown-book = Livre inconnu.
 not-an-isbn = Ceci n'est pas un ISBN !
+missing-author = Un livre doit absolument avoir un·e aut·rice·eur.
+# year (int) The year of creation
+before-creation-of-isbn = Le système ISBN n'est entré en vigueur qu'en { $year }.
 
 auth-login-title = Connexion
 # method (string) The sign in method
 auth-login-method = Sign in using { $method }
 
 webauthn-register-title = Association du dispositif de sécurité
 webauthn-register-description = Votre navigateur devrait être en train de vous demander de toucher votre dispositif de sécurité…
```

#### html2text {}

```diff
@@ -12,58 +12,67 @@
 software. # years (string) The years the copyright applies to. # holders
 (string) The names of the copyright holders. copyright = Version { $version }
 Â© { $years } { $holders }. # name (string) The name of the license. # url
 (string) The URL of the license file. license = Le code est sous licence
 {_$name_}. # name (string) The name of the information to display # value
 (string) The value of the information to display info-line = { $name }Â :
 { $value } access-forbidden = AccÃ¨s interditÂ ! access-not-authorized = AccÃ¨s
-non authorisÃ©Â ! an-error-occurred = Une erreur s'est produiteÂ ! # date
-(Date) A date to format date = { $date } book = livre books = livres book-
-added-on = ajoutÃ© le book-updated-on = mis Ã  jour le book-isbn = ISBN book-
-isbn-description = Le numÃ©ro ISBN assignÃ© au livre, par exemple 978-0-7653-
-9277-0. book-title = titre book-title-description = Le titre du livre. book-
-year = annÃ©e book-year-description = L'annÃ©e de publication du livre. book-
-author = autÂ·riceÂ·eur book-author-description = UnÂ·e des autÂ·riceÂ·eurÂ·s
-du livre. book-authors = autÂ·riceÂ·eurÂ·s book-authors-description = La liste
-des autÂ·riceÂ·eurÂ·s du livre, sÃ©parÃ©Â·eÂ·s par des virgules. book-genre =
-genre book-genre-description = Un des genres auxquels le livre se rattache.
-book-genres = genres book-genres-description = La liste des genres auxquels le
-livre se rattache, sÃ©parÃ©s par des virgules. unknown-error = Une erreur
-inconnue s'est produiteÂ ! mandatory-value = Cette valeur est obligatoireÂ !
-incorrect-value = Cette valeur est incorrecteÂ ! not-an-isbn = Ceci n'est pas
-un ISBNÂ ! auth-login-title = Connexion # method (string) The sign in method
-auth-login-method = Sign in using { $method } webauthn-register-title =
-Association du dispositif de sÃ©curitÃ© webauthn-register-description = Votre
-navigateur devrait Ãªtre en train de vous demander de toucher votre dispositif
-de sÃ©curitÃ©â¦ webauthn-register-success = Votre dispositif de sÃ©curitÃ© a
-Ã©tÃ© correctement associÃ©Â ! webauthn-register-failure = Votre dispositif de
-sÃ©curitÃ© n'a pas pu Ãªtre associÃ©Â !? webauthn-login-title = Connexion
-webauthn-login-description = Votre navigateur devrait Ãªtre en train de vous
-demander de toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-login-failure =
-Vous n'avez pas pu Ãªtre connectÃ©Â·eÂ !? totp-login-title = Connexion totp-
-login-description = Merci de saisir votre mot de passe Ã  usage unique. totp-
-login-password = Mot de passe totp-login-pattern = Un code TOTP se compose de 6
-chiffres. totp-login-action = Se connecter add-book-requires-authentification =
-Vous devez Ãªtre authentifiÃ©Â·e pour pouvoir ajouter un livreÂ ! add-book-
-title = Ajouter un nouveau livre Ã  la collection add-book-action = Ajouter un
-livre add-book-cancel = Annuler add-book-add = Ajouter add-book-cover-help =
-Cliquez pour tÃ©lÃ©verser une couverture add-book-cover-format-not-supported =
-Le format de cette couverture n'est pas supportÃ©Â ! search-books-title =
-Chercher un livre dans la collection search-books-action = Chercher un livre
-search-books-clear = RÃ©initialiser search-books-search = Chercher search-
-books-no-result = Aucun livre ne correspondÂ ! search-books-previous-page =
-PrÃ©cÃ©dent search-books-next-page = Suivant # title (string) The title of the
-book display-book-title = DÃ©tails pour Â«Â { $title }Â Â» update-book-
-requires-authentification = Vous devez Ãªtre authentifiÃ©Â·e pour pouvoir
-Ã©diter un livreÂ ! # isbn (string) The ISBN of the book update-book-title =
-Ãditer les informations de `{ $isbn }` update-book-action = Ãditer update-
-book-failure = Le livre n'a pas pu Ãªtre mis Ã  jourÂ ! update-book-success =
-Le livre a bien Ã©tÃ© mis Ã  jourÂ ! update-book-cancel = Annuler update-book-
-update = Enregistrer update-book-cover-help = Cliquez pour tÃ©lÃ©verser une
-nouvelle couverture update-book-cover-format-not-supported = Le format de cette
-couverture n'est pas supportÃ©Â ! book-already-exists = Ce livre est dÃ©jÃ 
-dans la collectionÂ ! # isbn (string) The ISBN of the book # url (string) The
-URL of the book book-added-html = Le livre {_$isbn_} a bien Ã©tÃ© ajoutÃ©Â ! #
-isbn (string) The ISBN of the book book-added-text = Le livre { $isbn } a bien
-Ã©tÃ© ajoutÃ©Â ! book-not-found = Le livre n'a pas Ã©tÃ© trouvÃ©Â ! book-
-cannot-be-added = Le livre n'a pas pu Ãªtre ajoutÃ©Â ! books-cannot-be-found =
-La recherche n'a pas pu Ãªtre effectuÃ©eÂ !
+non authorisÃ©Â ! an-error-occurred = Une erreur s'est produiteÂ ! bad-request
+= Vous avez soumis une mauvaise requÃªteÂ ! Cela n'aurait jamais dÃ»
+arriverÂ !? # date (Date) A date to format date = { $date } book = livre books
+= livres book-added-on = ajoutÃ© le book-updated-on = mis Ã  jour le book-isbn
+= ISBN book-isbn-description = Le numÃ©ro ISBN assignÃ© au livre, par exemple
+978-0-7653-9277-0. book-title = titre book-title-description = Le titre du
+livre. book-year = annÃ©e book-year-description = L'annÃ©e de publication du
+livre. book-author = autÂ·riceÂ·eur book-author-description = UnÂ·e des
+autÂ·riceÂ·eurÂ·s du livre. book-authors = autÂ·riceÂ·eurÂ·s book-authors-
+description = La liste des autÂ·riceÂ·eurÂ·s du livre, sÃ©parÃ©Â·eÂ·s par des
+virgules. book-genre = genre book-genre-description = Un des genres auxquels le
+livre se rattache. book-genres = genres book-genres-description = La liste des
+genres auxquels le livre se rattache, sÃ©parÃ©s par des virgules. unknown-error
+= Une erreur inconnue s'est produiteÂ ! mandatory-value = Cette valeur est
+obligatoireÂ ! incorrect-value = Cette valeur est incorrecteÂ ! # min (int) The
+minimum length string-too-short = La longueur minimale est { $min }. # max
+(int) The maximum length string-too-long = La longueur maximale est { $max }. #
+min (float) The minimum value number-too-small = La valeur minimale est { $min
+}. # max (float) The maximum value number-too-big = La valeur maximale est
+{ $max }. unknown-book = Livre inconnu. not-an-isbn = Ceci n'est pas un ISBNÂ !
+missing-author = Un livre doit absolument avoir unÂ·e autÂ·riceÂ·eur. # year
+(int) The year of creation before-creation-of-isbn = Le systÃ¨me ISBN n'est
+entrÃ© en vigueur qu'en { $year }. auth-login-title = Connexion # method
+(string) The sign in method auth-login-method = Sign in using { $method }
+webauthn-register-title = Association du dispositif de sÃ©curitÃ© webauthn-
+register-description = Votre navigateur devrait Ãªtre en train de vous demander
+de toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-register-success = Votre
+dispositif de sÃ©curitÃ© a Ã©tÃ© correctement associÃ©Â ! webauthn-register-
+failure = Votre dispositif de sÃ©curitÃ© n'a pas pu Ãªtre associÃ©Â !?
+webauthn-login-title = Connexion webauthn-login-description = Votre navigateur
+devrait Ãªtre en train de vous demander de toucher votre dispositif de
+sÃ©curitÃ©â¦ webauthn-login-failure = Vous n'avez pas pu Ãªtre
+connectÃ©Â·eÂ !? totp-login-title = Connexion totp-login-description = Merci de
+saisir votre mot de passe Ã  usage unique. totp-login-password = Mot de passe
+totp-login-pattern = Un code TOTP se compose de 6 chiffres. totp-login-action =
+Se connecter add-book-requires-authentification = Vous devez Ãªtre
+authentifiÃ©Â·e pour pouvoir ajouter un livreÂ ! add-book-title = Ajouter un
+nouveau livre Ã  la collection add-book-action = Ajouter un livre add-book-
+cancel = Annuler add-book-add = Ajouter add-book-cover-help = Cliquez pour
+tÃ©lÃ©verser une couverture add-book-cover-format-not-supported = Le format de
+cette couverture n'est pas supportÃ©Â ! search-books-title = Chercher un livre
+dans la collection search-books-action = Chercher un livre search-books-clear =
+RÃ©initialiser search-books-search = Chercher search-books-no-result = Aucun
+livre ne correspondÂ ! search-books-previous-page = PrÃ©cÃ©dent search-books-
+next-page = Suivant # title (string) The title of the book display-book-title =
+DÃ©tails pour Â«Â { $title }Â Â» update-book-requires-authentification = Vous
+devez Ãªtre authentifiÃ©Â·e pour pouvoir Ã©diter un livreÂ ! # isbn (string)
+The ISBN of the book update-book-title = Ãditer les informations de `{ $isbn
+}` update-book-action = Ãditer update-book-failure = Le livre n'a pas pu Ãªtre
+mis Ã  jourÂ ! update-book-success = Le livre a bien Ã©tÃ© mis Ã  jourÂ !
+update-book-cancel = Annuler update-book-update = Enregistrer update-book-
+cover-help = Cliquez pour tÃ©lÃ©verser une nouvelle couverture update-book-
+cover-format-not-supported = Le format de cette couverture n'est pas
+supportÃ©Â ! book-already-exists = Ce livre est dÃ©jÃ  dans la collectionÂ ! #
+isbn (string) The ISBN of the book # url (string) The URL of the book book-
+added-html = Le livre {_$isbn_} a bien Ã©tÃ© ajoutÃ©Â ! # isbn (string) The
+ISBN of the book book-added-text = Le livre { $isbn } a bien Ã©tÃ© ajoutÃ©Â !
+book-not-found = Le livre n'a pas Ã©tÃ© trouvÃ©Â ! book-cannot-be-added = Le
+livre n'a pas pu Ãªtre ajoutÃ©Â ! books-cannot-be-found = La recherche n'a pas
+pu Ãªtre effectuÃ©eÂ !
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/__init__.py` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_json/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,38 +10,28 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from abc import ABC, abstractmethod
+import json
 from http import HTTPStatus as HTTP
+from typing import Any
 
-
-class HttpPresenter(ABC):
-    @abstractmethod
-    def status_code(self) -> int:
-        ...
-
-    @abstractmethod
-    def headers(self) -> dict[str, str]:
-        ...
-
-    @abstractmethod
-    def data(self) -> str:
-        ...
+from bl_hector.interfaces.to_http import HttpPresenter
 
 
-class Redirection(HttpPresenter):
-    def __init__(self, cible: str, code_statut: HTTP = HTTP.SEE_OTHER) -> None:
-        self.__cible = cible
-        self.__code_statut = code_statut
+class Dict(HttpPresenter):
+    def __init__(self, data: dict[str, Any], /, *, status_code: HTTP = HTTP.OK) -> None:
+        self.__status_code = status_code
+        self.__headers = {"Content-Type": "application/json"}
+        self.__data = data
 
     def status_code(self) -> int:
-        return self.__code_statut
+        return int(self.__status_code)
 
     def headers(self) -> dict[str, str]:
-        return {"Location": self.__cible}
+        return self.__headers
 
     def data(self) -> str:
-        return ""
+        return json.dumps(self.__data)
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/__init__.py` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-import logging
 from http import HTTPStatus as HTTP
 from pathlib import Path
 from typing import Any, Callable, Optional
 
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 from jinja2_fragments import render_block
 from werkzeug.datastructures import MultiDict
@@ -26,19 +25,19 @@
 from bl_hector.application.use_cases import (
     add_book,
     display_book,
     look_up_book,
     search_books,
     update_book,
 )
-from bl_hector.domain.collection_management import errors, validators
+from bl_hector.domain.collection_management import validators
 from bl_hector.domain.collection_management.entities import Book
 from bl_hector.domain.collection_management.value_objects import Isbn
-from bl_hector.interfaces import User, l10n, translate_error
-from bl_hector.interfaces.to_http import HttpPresenter
+from bl_hector.interfaces import Pager, User, l10n, translate_error
+from bl_hector.interfaces.to_http import HttpMeta, HttpPresenter
 
 ENVIRONMENT = Environment(
     loader=FileSystemLoader([Path(__file__).parent / "templates"]),
     autoescape=select_autoescape(),
     extensions=["bl_hector.interfaces.utils.PatchedPyPugJSExtension"],
 )
 
@@ -49,371 +48,373 @@
 
 def url_for(*args: Any, **kwargs: Any) -> str:
     if "url_for" not in ENVIRONMENT.globals:
         raise RuntimeError("`url_for` is not declared on the environment!")
     return ENVIRONMENT.globals["url_for"](*args, **kwargs)  # type: ignore
 
 
-class JinjaPresenter(HttpPresenter):
-    def __init__(
-        self,
-        template: str,
-        /,
-        *,
-        fragment: str = "",
-        user: Optional[User] = None,
-        **context: Any,
-    ) -> None:
-        self.__status_code = HTTP.OK
-        self.__headers = {"Content-Type": "text/html; charset=UTF-8"}
-        self.__template = template if template.endswith(".pug") else f"{template}.pug"
-        self.__fragment = fragment
-        self.__user = user
-        self.__context: dict[str, Any] = {**context, "_": self._, "user": user}
-        self.__error = ""
-
-        self.__adapt_to(user)
-
-    def __adapt_to(self, user: Optional[User] = None) -> None:
-        locale = user.locale if (user and user.locale) else l10n.DEFAULT_LOCALE
-        self.__localization = l10n.localization(locale)
+class HtmlMeta(HttpMeta):
+    def __init__(self, **kwargs: Any) -> None:
+        super().__init__("text/html; charset=UTF-8", **kwargs)
+
+
+class HtmlContent:
+    def __init__(self, target: str, context: Optional[dict[str, Any]] = None) -> None:
+        self.__template, self.__fragment = self.__parse(target)
+        self.__context = context or {}
+
+    def __parse(self, target: str) -> tuple[str, str]:
+        e = target.split("#", 1)
+        t, f = (e[0], "") if len(e) == 1 else (e[0], e[1])
+        return t.removesuffix(".pug") + ".pug", f
 
-    def _(self, message_id: str, **kwargs: Any) -> str:
-        return str(self.__localization.format_value(message_id, kwargs))
+    def __str__(self) -> str:
+        if self.__fragment:
+            return render_block(  # type: ignore
+                ENVIRONMENT, self.__template, self.__fragment, **self.__context
+            )
+        return ENVIRONMENT.get_template(self.__template).render(**self.__context)
 
-    def translate_error(self, error: Optional[errors.IncorrectValue] = None) -> str:
-        return translate_error(self._, error)
+    def set(self, key: str, value: Any) -> None:
+        self.__context[key] = value
 
-    def status_code(self) -> int:
-        return int(self.__status_code)
+    def append(self, key: str, value: Any) -> None:
+        if key not in self.__context:
+            self.__context[key] = []
+        self.__context[key].append(value)
+
+    def delete(self, key: str) -> None:
+        if key in self.__context:
+            del self.__context[key]
 
-    def headers(self) -> dict[str, str]:
-        return self.__headers
+    def not_authorized(self) -> None:
+        if "user" in self.__context:
+            self.__context["error"] = self.__translate("access-forbidden")
+        else:
+            self.__context["error"] = self.__translate("access-not-authorized")
 
-    def data(self) -> str:
-        return self.render()
+    def __translate(self, message: str) -> str:
+        if "_" in self.__context:
+            return str(self.__context["_"](message))
+        return message
 
-    def set_status_code(self, status_code: HTTP) -> None:
-        self.__status_code = status_code
 
-    def set_header(self, name: str, value: str) -> None:
-        self.__headers[name] = value
+class HtmlOverHttpMixin:
+    meta: HttpMeta
+    content: HtmlContent
 
-    def error(self, message: str, status_code: HTTP) -> None:
-        self.__error = message
-        self.set_status_code(status_code)
+    def status_code(self) -> int:
+        return self.meta.status_code()
 
-    def redirect(self, url: str, status_code: HTTP = HTTP.SEE_OTHER) -> None:
-        if "Content-Type" in self.__headers:
-            del self.__headers["Content-Type"]
-        if self.__fragment:
-            self.__headers["HX-Location"] = url
-        else:
-            self.__headers["Location"] = url
-        self.set_status_code(status_code)
+    def headers(self) -> dict[str, str]:
+        return self.meta.headers()
+
+    def data(self) -> str:
+        return str(self.content)
 
     def not_authorized(self) -> None:
-        if self.__user:
-            self.set_status_code(HTTP.FORBIDDEN)
-            self.__error = self._("access-forbidden")
-        else:
-            self.set_status_code(HTTP.UNAUTHORIZED)
-            self.__error = self._("access-not-authorized")
+        self.meta.not_authorized()
+        self.content.not_authorized()
 
-    def render(self, **context: Any) -> str:
-        if self.__error:
-            return ENVIRONMENT.get_template("error.pug").render(
-                **self.__context, **context, message=self.__error
-            )
-        if self.__fragment:
-            return render_block(  # type: ignore
-                ENVIRONMENT,
-                self.__template,
-                self.__fragment,
-                **self.__context,
+
+class SimplePresenter(HtmlOverHttpMixin, HttpPresenter):
+    def __init__(
+        self, template: str, /, *, user: Optional[User] = None, **context: Any
+    ) -> None:
+        self.meta = HtmlMeta()
+        self.content = HtmlContent(
+            template,
+            {
+                "user": user,
+                "_": l10n.translator_for(user.locale if user else ""),
                 **context,
-            )
-        return ENVIRONMENT.get_template(self.__template).render(
-            **self.__context, **context
+            },
         )
 
 
-class SearchBooks(JinjaPresenter, search_books.Presenter):
-    PAGE_SIZE = 9
+class BadRequest(HtmlOverHttpMixin, HttpPresenter):
+    def __init__(self, /, *, user: Optional[User] = None) -> None:
+        _ = l10n.translator_for(user.locale if user else "")
+        self.meta = HtmlMeta(status=HTTP.BAD_REQUEST)
+        self.content = HtmlContent(
+            "error", {"user": user, "_": _, "message": _("bad-request")}
+        )
+
 
+class SearchBooks(HtmlOverHttpMixin, HttpPresenter, search_books.Presenter):
     def __init__(
         self,
         data: MultiDict[str, Any],
+        fragment: str,
         /,
         *,
-        fragment: str = "",
         user: Optional[User] = None,
     ) -> None:
-        super().__init__("books/search", fragment=fragment, user=user)
-        self.__data = data
-        self.__context: dict[str, Any] = {"errors": {}}
+        self._ = l10n.translator_for(user.locale if user else "")
+        pager = Pager(url_for("books.search", **data))
 
-        self.__set_page_urls()
-
-        if data:
-            # Handle the case when the search returns no book.
-            self.__context["books"] = []
-
-    def __set_page_urls(self) -> None:
-        self.__context["previous_page_url"] = self.__build_url(
-            {**self.__data, "page": self.__previous_page_number()}
-        )
-        # FIXME How to know if there are more results?!
-        self.__context["next_page_url"] = self.__build_url(
-            {**self.__data, "page": self.__next_page_number()}
+        self.meta = HtmlMeta(is_htmx=bool(fragment))
+        self.content = HtmlContent(
+            f"books/search#{fragment}",
+            {"_": self._, "user": user, "data": data, "errors": {}, "pager": pager},
         )
 
-    def __build_url(self, params: dict[str, str]) -> str:
-        if params.get("page", "0") == "0":
-            return ""
-        return url_for("books.search") + "?" + self.__join_params(params)
-
-    def __join_params(self, params: dict[str, str]) -> str:
-        return "&".join([f"{k}={v}" for k, v in params.items() if v])
-
-    def __next_page_number(self) -> str:
-        n = int(self.__data.get("page", "1"))
-        return f"{n + 1}"
-
-    def __previous_page_number(self) -> str:
-        if n := int(self.__data.get("page", "0")):
-            return f"{n - 1}"
-        return ""
-
-    def render(self, **context: Any) -> str:
-        return super().render(**self.__context, **context, data=self.__data)
+        if data:  # Handle the case when the search returns no book.
+            self.content.set("books", [])
 
     def bad_request(self, errors: search_books.Errors) -> None:
-        self.set_status_code(HTTP.OK)
-        self.__context["errors"] = {
-            "isbn": self.translate_error(errors.isbn),
-            "title": self.translate_error(errors.title),
-            "year": self.translate_error(errors.year),
-            "author": self.translate_error(errors.author),
-            "genre": self.translate_error(errors.genre),
-        }
+        self.content.set(
+            "errors",
+            {
+                "isbn": translate_error(self._, errors.isbn),
+                "title": translate_error(self._, errors.title),
+                "year": translate_error(self._, errors.year),
+                "author": translate_error(self._, errors.author),
+                "genre": translate_error(self._, errors.genre),
+            },
+        )
+        self.content.delete("books")
 
     def book(self, book: Book) -> None:
-        if "books" not in self.__context:
-            self.__context["books"] = []
-        self.__context["books"].append(
+        self.content.append(
+            "books",
             {
                 "isbn": str(book.isbn),
                 "title": str(book.title),
                 "year": int(book.year),
                 "authors": [str(a) for a in book.authors],
                 "genres": [str(g) for g in book.genres],
                 "cover": str(book.cover) if book.cover else "",
-            }
+            },
         )
 
 
-class AddBook(JinjaPresenter, add_book.Presenter):
+class AddBook(HtmlOverHttpMixin, HttpPresenter, add_book.Presenter):
     def __init__(
         self,
         data: MultiDict[str, Any],
+        fragment: str,
+        notify: Callable[[str, str], None],
         /,
         *,
-        notify: Callable[[str, str], None] = lambda m, t: None,
-        **kwargs: Any,
+        user: Optional[User] = None,
     ) -> None:
-        super().__init__("books/add", **kwargs)
-        self.set_status_code(HTTP.OK)
-        self.__data = data
+        self._ = l10n.translator_for(user.locale if user else "")
+        self.meta = HtmlMeta(is_logged_in=bool(user), is_htmx=bool(fragment))
+        self.content = HtmlContent(
+            f"books/add#{fragment}",
+            {"user": user, "_": self._, "data": data, "errors": {}},
+        )
         self.__notify = notify
-        self.__context: dict[str, Any] = {"errors": {}}
-
-    def render(self, **context: Any) -> str:
-        return super().render(**self.__context, **context, data=self.__data)
 
     def bad_request(self, errors: add_book.Errors) -> None:
-        self.__context["errors"] = {
-            "isbn": self.translate_error(errors.isbn),
-            "title": self.translate_error(errors.title),
-            "year": self.translate_error(errors.year),
-            "authors": self.translate_error(errors.authors),
-        }
+        self.content.set(
+            "errors",
+            {
+                "isbn": translate_error(self._, errors.isbn),
+                "title": translate_error(self._, errors.title),
+                "year": translate_error(self._, errors.year),
+                "authors": translate_error(self._, errors.authors),
+            },
+        )
 
     def book_already_exists(self, book: Book) -> None:
         self.__notify(self._("book-already-exists"), "info")
-        self.redirect(url_for("books.display", isbn=str(book.isbn)))
+        self.meta.see_other(url_for("books.display", isbn=str(book.isbn)))
 
     def book_added(self, book: Book) -> None:
         self.__notify(
             self._(
                 "book-added-html",
                 isbn=str(book.isbn),
                 url=url_for("books.display", isbn=str(book.isbn)),
             ),
             "success",
         )
-        self.redirect(url_for("books.add"))
+        self.meta.see_other(url_for("books.add"))
 
 
-class LookUpBook(JinjaPresenter, look_up_book.Presenter):
+class LookUpBook(HtmlOverHttpMixin, HttpPresenter, look_up_book.Presenter):
     def __init__(self, /, *, user: Optional[User] = None) -> None:
-        super().__init__("books/add", fragment="form", user=user)
-        self.__data: dict[str, Any] = {}
-        self.__context: dict[str, Any] = {"errors": {}}
-
-    def render(self, **context: Any) -> str:
-        return super().render(**self.__context, **context, data=self.__data)
+        self._ = l10n.translator_for(user.locale if user else "")
+        self.meta = HtmlMeta()
+        self.content = HtmlContent(
+            "books/add#form", {"user": user, "_": self._, "data": {}, "errors": {}}
+        )
 
     def not_an_isbn(self, isbn: str) -> None:
-        self.__data["isbn"] = isbn
-        self.__context["errors"] = {"isbn": self._("not-an-isbn")}
-
-    def unknown_error(self, message: str) -> None:
-        logging.error(f"LookUpBook: {message}")
-        self.__context["errors"] = {"isbn": self._("unknown-error")}
+        self.content.set("isbn", isbn)
+        self.content.set("errors", {"isbn": self._("not-an-isbn")})
 
     def book_not_found(self, isbn: Isbn) -> None:
-        self.__data["isbn"] = str(isbn)
-        self.__context["errors"] = {"isbn": self._("unknown-isbn")}
+        self.content.set("isbn", str(isbn))
+        self.content.set("errors", {"isbn": self._("unknown-isbn")})
 
     def book(self, book: Book) -> None:
-        self.__data = {
-            "isbn": str(book.isbn),
-            "title": str(book.title),
-            "year": int(book.year),
-            "authors": ", ".join([str(a) for a in book.authors]),
-            "genres": ", ".join([str(g) for g in book.genres]),
-            "cover": str(book.cover),
-        }
+        self.content.set(
+            "data",
+            {
+                "isbn": str(book.isbn),
+                "title": str(book.title),
+                "year": int(book.year),
+                "authors": ", ".join([str(a) for a in book.authors]),
+                "genres": ", ".join([str(g) for g in book.genres]),
+                "cover": str(book.cover) if book.cover else "",
+            },
+        )
 
 
-class DisplayBook(JinjaPresenter, display_book.Presenter):
+class DisplayBook(HtmlOverHttpMixin, HttpPresenter, display_book.Presenter):
     def __init__(
-        self,
-        /,
-        *,
-        notify: Callable[[str, str], None] = lambda m, t: None,
-        user: Optional[User] = None,
+        self, notify: Callable[[str, str], None], /, *, user: Optional[User] = None
     ) -> None:
-        super().__init__("books/display", user=user)
-        self.__context: dict[str, Any] = {"book": {}}
+        self._ = l10n.translator_for(user.locale if user else "")
+        self.meta = HtmlMeta(is_logged_in=bool(user))
+        self.content = HtmlContent(
+            "books/display", {"user": user, "_": self._, "book": {}}
+        )
         self.__notify = notify
 
-    def render(self, **context: Any) -> str:
-        return super().render(**self.__context, **context)
-
     def not_an_isbn(self, isbn: str) -> None:
         self.__notify(self._("not-an-isbn"), "warning")
-        self.redirect(url_for("books.search"))
+        self.meta.see_other(url_for("books.search"))
 
     def book_not_found(self, isbn: Isbn) -> None:
         self.__notify(self._("book-does-not-exist"), "warning")
-        self.redirect(url_for("books.search"))
+        self.meta.see_other(url_for("books.search"))
 
     def see_other(self, isbn: Isbn) -> None:
-        self.redirect(url_for("books.display", isbn=str(isbn)), HTTP.MOVED_PERMANENTLY)
+        self.meta.see_other(url_for("books.display", isbn=str(isbn)), permanent=True)
 
     def book(self, book: Book) -> None:
-        self.__context["book"] = {
-            "added_on": self._("date", date=book.added_on.to_date()),
-            "updated_on": (
-                self._("date", date=book.updated_on.to_date())
-                if book.updated_on != book.added_on
-                else "-"
-            ),
-            "isbn": str(book.isbn),
-            "title": str(book.title),
-            "year": int(book.year),
-            "authors": ", ".join([str(a) for a in book.authors]),
-            "genres": ", ".join([str(g) for g in book.genres]),
-            "cover": str(book.cover) if book.cover else "",
-        }
+        self.content.set(
+            "book",
+            {
+                "added_on": self._("date", date=book.added_on.to_date()),
+                "updated_on": (
+                    self._("date", date=book.updated_on.to_date())
+                    if book.updated_on != book.added_on
+                    else "-"
+                ),
+                "isbn": str(book.isbn),
+                "title": str(book.title),
+                "year": int(book.year),
+                "authors": ", ".join([str(a) for a in book.authors]),
+                "genres": ", ".join([str(g) for g in book.genres]),
+                "cover": str(book.cover) if book.cover else "",
+            },
+        )
 
 
-class DisplayBookToUpdate(JinjaPresenter, display_book.Presenter):
+class DisplayBookToUpdate(HtmlOverHttpMixin, HttpPresenter, display_book.Presenter):
     def __init__(
         self,
         isbn: str,
+        notify: Callable[[str, str], None],
         /,
         *,
-        notify: Callable[[str, str], None] = lambda m, t: None,
         user: Optional[User] = None,
     ) -> None:
-        super().__init__("books/update", user=user)
-        self.__context: dict[str, Any] = {"isbn": isbn, "data": {}, "errors": {}}
+        self._ = l10n.translator_for(user.locale if user else "")
+        self.meta = HtmlMeta(is_logged_in=bool(user))
+        self.content = HtmlContent(
+            "books/update",
+            {"user": user, "_": self._, "isbn": isbn, "data": {}, "errors": {}},
+        )
         self.__notify = notify
 
-    def render(self, **context: Any) -> str:
-        return super().render(**self.__context, **context)
-
     def not_an_isbn(self, isbn: str) -> None:
         self.__notify(self._("not-an-isbn"), "warning")
-        self.redirect(url_for("books.search"))
+        self.meta.see_other(url_for("books.search"))
 
     def book_not_found(self, isbn: Isbn) -> None:
         self.__notify(self._("book-does-not-exist"), "warning")
-        self.redirect(url_for("books.search"))
+        self.meta.see_other(url_for("books.search"))
 
     def see_other(self, isbn: Isbn) -> None:
-        self.redirect(url_for("books.display", isbn=str(isbn)), HTTP.MOVED_PERMANENTLY)
+        self.meta.see_other(url_for("books.display", isbn=str(isbn)), permanent=True)
 
     def book(self, book: Book) -> None:
-        self.__context["data"] = {
-            "isbn": str(book.isbn),
-            "title": str(book.title),
-            "year": int(book.year),
-            "authors": ", ".join([str(a) for a in book.authors]),
-            "genres": ", ".join([str(g) for g in book.genres]),
-            "cover": str(book.cover) if book.cover else "",
-        }
+        self.content.set(
+            "data",
+            {
+                "isbn": str(book.isbn),
+                "title": str(book.title),
+                "year": int(book.year),
+                "authors": ", ".join([str(a) for a in book.authors]),
+                "genres": ", ".join([str(g) for g in book.genres]),
+                "cover": str(book.cover) if book.cover else "",
+            },
+        )
 
 
-class UpdateBook(JinjaPresenter, update_book.Presenter):
+class UpdateBook(HtmlOverHttpMixin, HttpPresenter, update_book.Presenter):
     def __init__(
         self,
         isbn: str,
         data: MultiDict[str, Any],
+        fragment: str,
+        notify: Callable[[str, str], None],
         /,
         *,
-        notify: Callable[[str, str], None] = lambda m, t: None,
-        **kwargs: Any,
+        user: Optional[User] = None,
     ) -> None:
-        super().__init__("books/update", **kwargs)
-        self.set_status_code(HTTP.FORBIDDEN)
-        self.__data = data
+        self._ = l10n.translator_for(user.locale if user else "")
+        self.meta = HtmlMeta(is_logged_in=bool(user), is_htmx=bool(fragment))
+        self.content = HtmlContent(
+            f"books/update#{fragment}",
+            {"user": user, "_": self._, "isbn": isbn, "data": data, "errors": {}},
+        )
         self.__notify = notify
-        self.__context: dict[str, Any] = {"isbn": isbn, "errors": {}}
-
-    def render(self, **context: Any) -> str:
-        return super().render(**self.__context, **context, data=self.__data)
 
     def bad_request(self, errors: update_book.Errors) -> None:
-        self.set_status_code(HTTP.OK)
-        self.__context["errors"] = {
-            "title": self.translate_error(errors.title),
-            "year": self.translate_error(errors.year),
-            "authors": self.translate_error(errors.authors),
-        }
+        self.content.set(
+            "errors",
+            {
+                "title": translate_error(self._, errors.title),
+                "year": translate_error(self._, errors.year),
+                "authors": translate_error(self._, errors.authors),
+            },
+        )
 
     def book_not_found(self, isbn: Isbn) -> None:
         self.__notify(self._("book-not-found"), "warning")
-        self.redirect(url_for("books.search"))
+        self.meta.see_other(url_for("books.search"))
 
     def book_updated(self, book: Book) -> None:
         self.__notify(self._("update-book-success"), "success")
-        self.redirect(url_for("books.display", isbn=str(book.isbn)))
+        self.meta.see_other(url_for("books.display", isbn=str(book.isbn)))
 
 
-class ValidateIsbn(JinjaPresenter):
+class ValidateBook(HtmlOverHttpMixin, HttpPresenter):
     def __init__(
-        self, data: MultiDict[str, Any], /, *, user: Optional[User] = None
+        self, attribute: str, value: str, /, *, user: Optional[User] = None
     ) -> None:
-        super().__init__("books/search", fragment="isbn", user=user)
-        self.__data = data
-        self.__errors = {}
-
-        if isbn := data.get("isbn", ""):
-            errors = add_book.Errors(isbn=validators.isbn(isbn))
-            self.__errors["isbn"] = self.translate_error(errors.isbn)
+        self._ = l10n.translator_for(user.locale if user else "")
+        errors = self.__validate(attribute, value)
+        context = {
+            "user": user,
+            "_": self._,
+            "data": {attribute: value},
+            "errors": errors,
+        }
+
+        self.meta = HtmlMeta()
+        # We use `search` as it contains all fields as not required.
+        self.content = HtmlContent(f"books/search#{attribute}", context)
+
+    def __validate(self, attribute: str, value: str) -> dict[str, str]:
+        errors: dict[str, str] = {}
+
+        if not value:
+            return errors
+
+        if attribute == "isbn":
+            errors["isbn"] = translate_error(
+                self._, add_book.Errors(isbn=validators.isbn(value)).isbn
+            )
+        if attribute == "year":
+            errors["year"] = translate_error(
+                self._, add_book.Errors(year=validators.year(int(value))).year
+            )
 
-    def render(self, **context: Any) -> str:
-        return super().render(**context, data=self.__data, errors=self.__errors)
+        return errors
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug`

 * *Files 5% similar despite different names*

```diff
@@ -25,11 +25,12 @@
       h1.title.is-3.has-text-centered= _("auth-login-title")
 
       .columns
         .column
         .column
           .buttons
             each link in links
-              a.button.is-fullwidth(href="#{url_for(link.route)}")
+              //- Some plugins, like WebAuthn, need the page to be loaded "normally".
+              a.button.is-fullwidth(href="#{url_for(link.route)}" hx-boost="false")
                 span.icon: i.fas(class="fa-#{link.icon}")
                 span= _("auth-login-method", method=link.label)
         .column
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/add.pug` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/add.pug`

 * *Files 6% similar despite different names*

```diff
@@ -67,39 +67,44 @@
               )
               input#coverInput.is-hidden(
                 name="cover"
                 type="text"
                 value="#{data.cover}"
               )
             .column
-              block isbn
-                .field.is-horizontal(_="on load remove @disabled from .button")
-                  .field-body
-                    include books/mixins/render_isbn
-                    +isbn_field(data.isbn, errors.isbn, required="1")
-
-                    .field.is-narrow
-                      p.control
-                        button.button.is-info(
-                          hx-post="#{url_for('books.look_up')}"
-                          hx-target="#form"
-                          disabled
-                          _="on htmx:beforeSend add .is-loading add @disabled"
-                        )
-                          span.icon: i.fas.fa-search
-                          span= _("search-books-action")
-
-              +text_field("title", data.title, errors.title, required="1", description=_("book-title-description"), icon="file", placeholder=_('book-title'))
-              +number_field("year", data.year, errors.year, required="1", description=_("book-year-description"), icon="calendar", placeholder=_('book-year'))
-              +text_field("authors", data.authors, errors.authors, required="1", description=_("book-authors-description"), icon="users", placeholder=_('book-authors'))
+              .field.is-horizontal
+                .field-body
+                  block isbn
+                    include mixins/form
+                    +isbn_field(data.isbn, errors.isbn)
+
+                  .field.is-narrow(_="on load remove @disabled from #lookUp")
+                    p.control
+                      button#lookUp.button.is-info(
+                        hx-post="#{url_for('books.look_up')}"
+                        hx-target="#form"
+                        disabled
+                        _="on htmx:beforeSend add .is-loading add @disabled"
+                      )
+                        span.icon: i.fas.fa-search
+                        span= _("search-books-action")
+
+              +text_field("title", data.title, errors.title, required=1, description=_("book-title-description"), icon="file", placeholder=_('book-title'))
+
+              block year
+                include mixins/form
+                +year_field(data.year, errors.year)
+
+              +text_field("authors", data.authors, errors.authors, required=1, description=_("book-authors-description"), icon="users", placeholder=_('book-authors'))
+
               +text_field("genres", data.genres, errors.genres, description=_("book-genres-description"), icon="crown", placeholder=_('book-genres'))
 
               .field
                 p.control
-                  a.button.is-light(href="#{url_for('books.search')}" hx-boost="true")
+                  a.button.is-light(href="#{url_for('books.search')}" hx-target="body")
                     span.icon: i.fas.fa-times
                     span= _("add-book-cancel")
                   button.button.is-primary
                     span.icon: i.fas.fa-plus
                     span= _("add-book-add")
 
         if error is defined
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/display.pug` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/display.pug`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 block content
   section.section
     .container
       //- Fixes a spacing problem.
       .buttons.is-pulled-right(style="margin-bottom: -1rem")
         if user.can_update_book
-          a.button.is-link(href="#{url_for('books.update', isbn=book.isbn)}" hx-boost="true")
+          a.button.is-link(href="#{url_for('books.update', isbn=book.isbn)}")
             span.icon: i.fas.fa-edit
             span= _("update-book-action")
         else
           button.button.is-link.is-disabled(disabled title=_("update-book-requires-authentification"))
             span.icon: i.fas.fa-edit
             span= _("update-book-action")
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/mixins/render_isbn.pug` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/layout.pug`

 * *Files 26% similar despite different names*

```diff
@@ -10,57 +10,47 @@
 //- but WITHOUT ANY WARRANTY; without even the implied warranty of
 //- MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 //- GNU Affero General Public License for more details.
 //-
 //- You should have received a copy of the GNU Affero General Public License
 //- along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-include mixins/form
+include mixins/flash
+include mixins/navbar
 
-mixin isbn_field(value, error, required="")
-  .field
-    p.control.has-icons-left.has-icons-right
-      if error
-        - var classes = "is-danger"
-      elif value
-        - var classes = "is-success"
-      else
-        - var classes = ""
-
-      //- Find a better way to set required!
-      if required
-        input.input(
-          type="text"
-          id="isbn"
-          name="isbn"
-          class=classes
-          value=value
-          required
-          placeholder=_("book-isbn")
-          hx-post=url_for("books.validate_isbn")
-          hx-trigger="search, blur"
-          hx-target="closest .field"
-          hx-swap="outerHTML"
-        )
-      else
-        input.input(
-          type="text"
-          id="isbn"
-          name="isbn"
-          class=classes
-          value=value
-          placeholder=_("book-isbn")
-          hx-post=url_for("books.validate_isbn")
-          hx-trigger="search, blur"
-          hx-target="closest .field"
-          hx-swap="outerHTML"
-        )
-      span.icon.is-small.is-left: i.fas.fa-book
-      if value
-        span.icon.is-small.is-right
-          if error
-            i.fas.fa-exclamation-triangle
-          else
-            i.fas.fa-check
+doctype html
+html
+  head
+    meta(charset="utf-8")
+    meta(name="viewport" content="width=device-width, initial-scale=1")
 
-    +error_message(error)
-    +help_message(_("book-isbn-description"))
+    block title
+      //- `title` tag inside the block to avoid some weird syntax highlighting problems
+      title= _("hector")
+
+    link(rel="icon" type="image/svg" href="#{url_for('static', filename='favicon.svg')}")
+    link(rel="stylesheet" href="#{url_for('static', filename='css/bulma@0.9.4.min.css')}")
+    link(rel="stylesheet" href="#{url_for('static', filename='css/font-awesome@5.14.0.css')}")
+    link(rel="stylesheet" href="#{url_for('static', filename='css/hector.css')}")
+    block links
+
+    block head_scripts
+
+  body(hx-boost="true")
+    +navbar()
+
+    .page
+      - var messages = get_flashed_messages(with_categories=true)
+      +flash(messages)
+
+      block content
+
+    footer.footer
+      .content.has-text-centered
+        p
+          span= _("copyright", version=version, years="2023", holders="Bioneland") | safe
+          br
+          span= _("license", name="AGPL", url="https://www.gnu.org/licenses/agpl-3.0.fr.html") | safe
+
+    script(src="#{url_for('static', filename='js/hyperscript@0.9.8.min.js')}")
+    script(src="#{url_for('static', filename='js/htmx@1.9.2.min.js')}")
+    block scripts
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/search.pug` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/search.pug`

 * *Files 12% similar despite different names*

```diff
@@ -20,109 +20,111 @@
   title= _("hector") + " – " + _("search-books-title")
 
 block content
   section.section
     .container
       .buttons.is-pulled-right
         if user.can_add_book
-          a.button.is-link(href="#{url_for('books.add')}" hx-boost="true")
+          a.button.is-link(href=url_for("books.add"))
             span.icon: i.fas.fa-plus
             span= _("add-book-action")
         else
           button.button.is-link.is-disabled(disabled title=_("add-book-requires-authentification"))
             span.icon: i.fas.fa-plus
             span= _("add-book-action")
 
       h1.title.is-3= _("search-books-title")
 
-      block form
-        include mixins/form
-        form#form(
-          method="GET"
-          action="#{url_for('books.search')}"
-          hx-get="#{url_for('books.search')}"
-          hx-target="#form"
-          hx-push-url="true"
-        )
-          +hidden_input("page", data.page or "1")
-
-          block isbn
-            include books/mixins/render_isbn
-            +isbn_field(data.isbn, errors.isbn)
-
-          +text_field("title", data.title, errors.title, description=_("book-title-description"), icon="file", placeholder=_('book-title'))
-          +number_field("year", data.year, errors.year, description=_("book-year-description"), icon="calendar", placeholder=_('book-year'))
-          +text_field("author", data.author, errors.author, description=_("book-author-description"), icon="users", placeholder=_('book-author'))
-          +text_field("genre", data.genre, errors.genre, description=_("book-genre-description"), icon="crown", placeholder=_('book-genre'))
-
-          .field
-            p.control
-              a.button.is-light(href="#{url_for('books.search')}" hx-boost="true" hx-target="body")
-                span.icon: i.fas.fa-trash
-                span= _("search-books-clear")
-              button.button.is-primary(_="on click add .is-loading")
-                span.icon: i.fas.fa-search
-                span= _("search-books-search")
-
-        if books is defined
-          if books|length > 0
-            #books.books
-              block books
-                mixin book_content(book)
-                  .card-content
-                    .media
-                      .media-left(style="width: 5em")
-                        figure.image.cover.is-2by3
-                          img(src="#{book.cover or url_for('static', filename='img/placeholders/320x480.png')}" alt="Book cover")
-                      .media-content
-                        h2.title.is-4(title="#{book.title}")= book.title|truncate(20)
-                        p.subtitle.is-6
-                          each author in book.authors
-                            if author == book.authors[-1]
-                              | #[a(href="#{url_for('books.search', author=author)}") #{author}]
-                            else
-                              | #[a(href="#{url_for('books.search', author=author)}") #{author}], 
-                        p
-                          small
-                            | #[time(datetime="#{book.year}-01-01") #{book.year}] / 
-                            a(href="#{url_for('books.display', isbn=book.isbn)}") #{book.isbn}
-                            br
-                            each genre in book.genres
-                              if genre == book.genres[-1]
-                                | #[a(href="#{url_for('books.search', genre=genre)}") #{genre}]
-                              else
-                                | #[a(href="#{url_for('books.search', genre=genre)}") #{genre}], 
-
-                each book in books
-                  if loop.last
-                    article.book.card(
-                      hx-get=next_page_url
-                      hx-trigger="revealed"
-                      hx-swap="beforeend"
-                      hx-target="#books"
-                      hx-indicator="#indicator"
-                    )
-                      +book_content(book)
-                  else
+      block search
+        #search
+          include mixins/form
+          form(
+            method="GET"
+            action=url_for("books.search")
+            hx-get=url_for("books.search")
+            hx-target="#search"
+            hx-push-url="true"
+          )
+            +hidden_input("page", data.page or "1")
+
+            block isbn
+              include mixins/form
+              +isbn_field(data.isbn, errors.isbn)
+
+            +text_field("title", data.title, errors.title, description=_("book-title-description"), icon="file", placeholder=_('book-title'))
+
+            block year
+              include mixins/form
+              +year_field(data.year, errors.year)
+
+            +text_field("author", data.author, errors.author, description=_("book-author-description"), icon="users", placeholder=_('book-author'))
+
+            +text_field("genre", data.genre, errors.genre, description=_("book-genre-description"), icon="crown", placeholder=_('book-genre'))
+
+            .field
+              p.control
+                a.button.is-light(href=url_for("books.search") hx-target="body")
+                  span.icon: i.fas.fa-trash
+                  span= _("search-books-clear")
+                button.button.is-primary(_="on click add .is-loading")
+                  span.icon: i.fas.fa-search
+                  span= _("search-books-search")
+
+          if books is defined
+            if books|length > 0
+              #books.books
+                block books
+                  each book in books
                     article.book.card
-                      +book_content(book)
-
-            #indicator.buttons.is-centered.mt-3.htmx-indicator.is-hidden(_="on load remove .is-hidden")
-                button.button.is-white.is-loading Loading indicator
-
-            if previous_page_url or next_page_url:
-              .buttons.is-centered.mt-3(_="on load remove me")
-                if previous_page_url:
-                  a#previous-page.button.is-link(href="#{previous_page_url}")
-                    span.icon: i.fa.fa-step-backward
-                    span= _("search-books-previous-page")
-                if next_page_url:
-                  a#next-page.button.is-link(href="#{next_page_url}")
-                    span= _("search-books-next-page")
-                    span.icon: i.fa.fa-step-forward
-          else
-            article.message.is-info
-              .message-body= _("search-books-no-result")
+                      .card-content
+                        .media
+                          .media-left(style="width: 5em")
+                            figure.image.cover.is-2by3
+                              img(src="#{book.cover or url_for('static', filename='img/placeholders/320x480.png')}" alt="Book cover")
+                              if loop.last
+                                span(
+                                  hx-get=pager.next
+                                  hx-trigger="revealed"
+                                  hx-swap="beforeend"
+                                  hx-target="#books"
+                                  hx-indicator="#indicator"
+                                  hx-push-url="false"
+                                )
+                          .media-content
+                            h2.title.is-4(title=book.title)= book.title|truncate(20)
+                            p.subtitle.is-6
+                              each author in book.authors
+                                if author == book.authors[-1]
+                                  | #[a(href=url_for("books.search", author=author)) #{author}]
+                                else
+                                  | #[a(href=url_for("books.search", author=author)) #{author}], 
+                            p
+                              small
+                                | #[time(datetime="#{book.year}-01-01") #{book.year}] / 
+                                a(href=url_for("books.display", isbn=book.isbn)) #{book.isbn}
+                                br
+                                each genre in book.genres
+                                  if genre == book.genres[-1]
+                                    | #[a(href=url_for("books.search", genre=genre)) #{genre}]
+                                  else
+                                    | #[a(href=url_for("books.search", genre=genre)) #{genre}], 
+
+              #indicator.buttons.is-centered.mt-3.htmx-indicator.is-hidden(_="on load remove .is-hidden")
+                  button.button.is-white.is-loading Loading indicator
+
+              if pager.previous or pager.next:
+                .buttons.is-centered.mt-3(_="on load remove me")
+                  if pager.previous:
+                    a#previous-page.button.is-link(href=pager.previous)
+                      span.icon: i.fa.fa-step-backward
+                      span= _("search-books-previous-page")
+                  if pager.next and books|length >= pager.PAGE_SIZE:
+                    a#next-page.button.is-link(href=pager.next)
+                      span= _("search-books-next-page")
+                      span.icon: i.fa.fa-step-forward
+            else
+              article.message.is-info
+                .message-body= _("search-books-no-result")
 
         if error is defined
           article.message.is-danger
             .message-body= error
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/books/update.pug` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/update.pug`

 * *Files 7% similar despite different names*

```diff
@@ -68,21 +68,26 @@
               input#coverInput.is-hidden(
                 name="cover"
                 type="text"
                 value="#{data.cover}"
               )
             .column
               +text_field("title", data.title, errors.title, required="1", description=_("book-title-description"), icon="file", placeholder=_('book-title'))
-              +number_field("year", data.year, errors.year, required="1", description=_("book-year-description"), icon="calendar", placeholder=_('book-year'))
+
+              block year
+                include mixins/form
+                +year_field(data.year, errors.year)
+
               +text_field("authors", data.authors, errors.authors, required="1", description=_("book-authors-description"), icon="users", placeholder=_('book-authors'))
+
               +text_field("genres", data.genres, errors.genres, description=_("book-genres-description"), icon="crown", placeholder=_('book-genres'))
 
               .field
                 p.control
-                  a.button.is-light(href="#{url_for('books.display', isbn=data.isbn)}" hx-boost="true" hx-target="body")
+                  a.button.is-light(href="#{url_for('books.display', isbn=data.isbn)}" hx-target="body")
                     span.icon: i.fas.fa-times
                     span= _("update-book-cancel")
                   button.button.is-primary
                     span.icon: i.fas.fa-plus
                     span= _("update-book-update")
 
         if error is defined
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/error.pug` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/error.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug`

 * *Files 21% similar despite different names*

```diff
@@ -108,14 +108,27 @@
 mixin render_description(field)
   if field.description
     p.help= field.description
 
 mixin render_hidden(field)
   input(type="hidden" name="#{field.name}" value="#{field.data}")
 
+
+mixin isbn_field(data, error)
+  .field(hx-trigger="blur from:#isbn" hx-post=url_for("books.validate", attribute="isbn") hx-target="this" hx-push-url="false")
+    +text_input("isbn", data, error=error, icon="calendar", placeholder=_('book-isbn'))
+    +error_message(error)
+    +help_message(_("book-isbn-description"))
+
+mixin year_field(data, error)
+  .field(hx-trigger="blur from:#year" hx-post=url_for("books.validate", attribute="year") hx-target="this" hx-push-url="false")
+    +number_input("year", data, error=error, icon="calendar", placeholder=_("book-year"))
+    +error_message(error)
+    +help_message(_("book-year-description"))
+
 //- At the bottom of the file for it f**ks up the highlighting!?
 mixin render_input(field, placeholder="")
   - var classes = "input"
   if field.errors
     - var classes = "input is-danger"
 
   | #{field(class=classes, placeholder=placeholder)}
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //- MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 //- GNU Affero General Public License for more details.
 //-
 //- You should have received a copy of the GNU Affero General Public License
 //- along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 mixin navbar()
-  nav.navbar(role="navigation" aria-label="main navigation" hx-boost="true")
+  nav.navbar(role="navigation" aria-label="main navigation")
     .container
       .navbar-brand
         a.navbar-item.is-size-5.has-text-weight-semibold(href="#{url_for('aliases.root')}")= _("hector")
         a.navbar-burger(
           role="button"
           aria-label="menu"
           aria-expanded="false"
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug`

 * *Files 5% similar despite different names*

```diff
@@ -26,23 +26,27 @@
 
       article.message.is-info
         p.message-body= _("totp-login-description")
 
       .columns
         .column
         .column.has-text-centered
-          form.box(method="POST")
+          form#form.box(
+            method="POST"
+            _="on load focus() the first <input/> in me"
+          )
             .field
               label.label= _("totp-login-password")
               .control
                 input.input.has-text-centered.is-size-5(
                   type="string"
                   name="password"
                   maxlength="6"
                   pattern="[\d]{6}"
                   oninvalid="#{'setCustomValidity(\'' + _('totp-login-pattern') + '\')'}"
                   style="width: 7rem"
+                  _="on keyup if the length of my value is 6 submit() the #form"
                 )
             .field
               .control
                 button.button.is-primary(type="submit")= _("totp-login-action")
         .column
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug` & `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_http/as_json/__init__.py` & `bl_hector-0.2.0/bl_hector/interfaces/to_terminal/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,28 +10,31 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-import json
-from http import HTTPStatus as HTTP
-from typing import Any
+from abc import ABC, abstractmethod
+from enum import Enum
 
-from bl_hector.interfaces.to_http import HttpPresenter
+from bl_hector.application.use_cases import look_up_book
 
 
-class Dict(HttpPresenter):
-    def __init__(self, data: dict[str, Any], /, *, status_code: HTTP = HTTP.OK) -> None:
-        self.__status_code = status_code
-        self.__headers = {"Content-Type": "application/json"}
-        self.__data = data
+class ExitCodes(Enum):
+    OK = 0
+    USAGE = 1
+    NOT_FOUND = 2
+    BAD_REQUEST = 3
 
-    def status_code(self) -> int:
-        return int(self.__status_code)
 
-    def headers(self) -> dict[str, str]:
-        return self.__headers
+class WithExitCode(ABC):
+    @abstractmethod
+    def exit_code(self) -> int:
+        ...
 
-    def data(self) -> str:
-        return json.dumps(self.__data)
+
+class LookUpBookInterface(look_up_book.Presenter, WithExitCode):
+    """
+    Interface required when using more than one presenter
+    inside a route/command, so MyPy can do it's job!
+    """
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/to_terminal/as_text.py` & `bl_hector-0.2.0/bl_hector/interfaces/to_terminal/as_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Callable, Optional
 
 from bl_hector.application.use_cases import add_book, display_book
 from bl_hector.domain.collection_management.entities import Book
-from bl_hector.domain.collection_management.errors import IncorrectValue
+from bl_hector.domain.collection_management.errors import InvalidValue
 from bl_hector.domain.collection_management.value_objects import Isbn
 from bl_hector.interfaces import translate_error
 from bl_hector.interfaces.l10n import DummyTranslator, Translator
 from bl_hector.interfaces.to_terminal import ExitCodes, LookUpBookInterface
 
 
 class DisplayBook(display_book.Presenter):
@@ -121,15 +121,15 @@
         self.__exit_code = ExitCodes.BAD_REQUEST
         self.__printer(self._("book-cannot-be-added"))
         self.__print_error("book-isbn", errors.isbn)
         self.__print_error("book-title", errors.title)
         self.__print_error("book-year", errors.year)
         self.__print_error("book-authors", errors.authors)
 
-    def __print_error(self, name: str, error: Optional[IncorrectValue]) -> None:
+    def __print_error(self, name: str, error: Optional[InvalidValue]) -> None:
         if not error:
             return
         self.__printer(
             self._("info-line", name=self._(name), value=translate_error(self._, error))
         )
 
     def book_already_exists(self, book: Book) -> None:
```

### Comparing `bl_hector-0.1.2/bl_hector/interfaces/utils.py` & `bl_hector-0.2.0/bl_hector/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.1.2/pyproject.toml` & `bl_hector-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bl_hector"
-version = "0.1.2"
+version = "0.2.0"
 description = "A collection manager."
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://git.easter-eggs.org/bioneland/hector"
 
 exclude = [
@@ -24,15 +24,15 @@
 Flask = "^2.3.2"
 pypugjs = "^5.9.12"
 bl-seth = "^0.2.0"
 isbnlib = "^3.10.14"
 jinja2-fragments = "^0.3.0"
 SQLAlchemy = "^2.0.15"
 typer = "^0.9.0"
-bl3d = "^0.3.0"
+bl3d = "^0.4.0"
 "fluent.runtime" = "^0.4.0"
 webauthn = {version = "^1.8.1", optional = true}
 requests = "^2.31.0"
 pyotp = {version = "^2.8.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
```

### Comparing `bl_hector-0.1.2/setup.py` & `bl_hector-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,24 +34,23 @@
                                     'static/img/placeholders/*',
                                     'static/js/*',
                                     'static/webfonts/*'],
  'bl_hector.interfaces.l10n': ['en-GB/*', 'fr-FR/*'],
  'bl_hector.interfaces.to_http.as_html': ['templates/*',
                                           'templates/auth/*',
                                           'templates/books/*',
-                                          'templates/books/mixins/*',
                                           'templates/mixins/*',
                                           'templates/totp/*',
                                           'templates/webauthn/*']}
 
 install_requires = \
 ['Flask>=2.3.2,<3.0.0',
  'SQLAlchemy>=2.0.15,<3.0.0',
  'bl-seth>=0.2.0,<0.3.0',
- 'bl3d>=0.3.0,<0.4.0',
+ 'bl3d>=0.4.0,<0.5.0',
  'fluent.runtime>=0.4.0,<0.5.0',
  'isbnlib>=3.10.14,<4.0.0',
  'jinja2-fragments>=0.3.0,<0.4.0',
  'pypugjs>=5.9.12,<6.0.0',
  'requests>=2.31.0,<3.0.0',
  'typer>=0.9.0,<0.10.0']
 
@@ -59,15 +58,15 @@
 {'totp': ['pyotp>=2.8.0,<3.0.0'], 'webauthn': ['webauthn>=1.8.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['hector = bl_hector.configuration.cli:cli']}
 
 setup_kwargs = {
     'name': 'bl-hector',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': 'A collection manager.',
     'long_description': '# Hector — a collection manager\n\n## Install\n\nHector is available on PyPI under the name `bl_hector`.\nTo install, just run `python -m pip install bl_hector`.\n\n\n## Configure\n\nHector is configured using environment variables.\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\nAll the variable names must be prefixed with `HECTOR_`. For instance\xa0:\n\n```console\n# The secret can be generated using the `secrets.token_hex()` function.\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n\n# Additional Python database drivers might be required depending on the DSN.\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN_ENABLED=1\n```\n\nTOTP authentication is provided to be able to login on servers that do not (yet) support\nthe `cryptography` module. You must install extra dependencies (`bl-hector[totp]`)\nand enable it explicitly by setting a base32 random secret:\n\n```console\n# The secret can be generated using the `pyotp.random_base32()` function.\n$ export HECTOR_TOTP_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX\n```\n\nNote that it is a highly insecure way of authenticating, as anyone gaining access to your\nOTP generator would be able to login.\n\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n\n\n## Contributing\n\nSee [CONTRIBUTING.md]() to set up a development environment.\n',
     'author': 'Tanguy Le Carrour',
     'author_email': 'tanguy@bioneland.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://git.easter-eggs.org/bioneland/hector',
```

### Comparing `bl_hector-0.1.2/PKG-INFO` & `bl_hector-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bl-hector
-Version: 0.1.2
+Version: 0.2.0
 Summary: A collection manager.
 Home-page: https://git.easter-eggs.org/bioneland/hector
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: totp
 Provides-Extra: webauthn
 Requires-Dist: Flask (>=2.3.2,<3.0.0)
 Requires-Dist: SQLAlchemy (>=2.0.15,<3.0.0)
 Requires-Dist: bl-seth (>=0.2.0,<0.3.0)
-Requires-Dist: bl3d (>=0.3.0,<0.4.0)
+Requires-Dist: bl3d (>=0.4.0,<0.5.0)
 Requires-Dist: fluent.runtime (>=0.4.0,<0.5.0)
 Requires-Dist: isbnlib (>=3.10.14,<4.0.0)
 Requires-Dist: jinja2-fragments (>=0.3.0,<0.4.0)
 Requires-Dist: pyotp (>=2.8.0,<3.0.0); extra == "totp"
 Requires-Dist: pypugjs (>=5.9.12,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
```

