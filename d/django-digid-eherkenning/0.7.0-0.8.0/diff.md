# Comparing `tmp/django-digid-eherkenning-0.7.0.tar.gz` & `tmp/django-digid-eherkenning-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-digid-eherkenning-0.7.0.tar", last modified: Tue Feb 21 09:36:58 2023, max compression
+gzip compressed data, was "django-digid-eherkenning-0.8.0.tar", last modified: Wed Jun 21 09:39:17 2023, max compression
```

## Comparing `django-digid-eherkenning-0.7.0.tar` & `django-digid-eherkenning-0.8.0.tar`

### file list

```diff
@@ -1,151 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.433599 django-digid-eherkenning-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-02-21 09:36:58.433599 django-digid-eherkenning-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.421599 django-digid-eherkenning-0.7.0/digid_eherkenning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/digid_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/eherkenning_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.417599 django-digid-eherkenning-0.7.0/digid_eherkenning/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.417599 django-digid-eherkenning-0.7.0/digid_eherkenning/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.421599 django-digid-eherkenning-0.7.0/digid_eherkenning/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.421599 django-digid-eherkenning-0.7.0/digid_eherkenning/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.421599 django-digid-eherkenning-0.7.0/digid_eherkenning/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/management/commands/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/management/commands/generate_digid_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/management/commands/generate_eherkenning_dienstcatalogus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/management/commands/generate_eherkenning_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/management/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/metadata_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.421599 django-digid-eherkenning-0.7.0/digid_eherkenning/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/migrations/0002_auto_20221102_1046.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.425599 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/digid_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.425599 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/idp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/idp/digid_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/idp/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.425599 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/idp/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/idp/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/idp/views/digid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.425599 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/mock/views/digid.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/mock_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.425599 django-digid-eherkenning-0.7.0/digid_eherkenning/models/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/models/digid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9034 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/models/eherkenning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.425599 django-digid-eherkenning-0.7.0/digid_eherkenning/saml2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/saml2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/saml2/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/saml2/digid.py
--rw-r--r--   0 runner    (1001) docker     (123)    16747 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/saml2/eherkenning.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.417599 django-digid-eherkenning-0.7.0/digid_eherkenning/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.425599 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.429599 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    21493 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/RO_DigiD_Logo_Homepage.svg
--rw-r--r--   0 runner    (1001) docker     (123)    69467 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextbold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    84044 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextitalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76489 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextregular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/ajaxLoader.gif
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/app.svg
--rw-r--r--   0 runner    (1001) docker     (123)    81640 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/application.css
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/assets_icons_info icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/digid_eo_rgb.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/digid_menu_digid_app_phone.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/digid_menu_nfc_reader.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/error-darkmode.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/error.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icon-mail.png
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icon-smartphone.png
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icon_error_full-red.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icon_error_full-yellow.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/info-darkmode.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/info.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/info_icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/loader.gif
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/loader.png
--rw-r--r--   0 runner    (1001) docker     (123)    10987 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/nfc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/password.png
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/ro-favicon-wit-0xffffff.png
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/session.svg
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/extra.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.429599 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid_eherkenning/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid_eherkenning/login_submit.css
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid_eherkenning/login_submit.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.417599 django-digid-eherkenning-0.7.0/digid_eherkenning/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.417599 django-digid-eherkenning-0.7.0/digid_eherkenning/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.417599 django-digid-eherkenning-0.7.0/digid_eherkenning/templates/admin/digid_eherkenning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.429599 django-digid-eherkenning-0.7.0/digid_eherkenning/templates/admin/digid_eherkenning/digidconfiguration/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/templates/admin/digid_eherkenning/digidconfiguration/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.429599 django-digid-eherkenning-0.7.0/digid_eherkenning/templates/admin/digid_eherkenning/eherkenningconfiguration/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/templates/admin/digid_eherkenning/eherkenningconfiguration/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.429599 django-digid-eherkenning-0.7.0/digid_eherkenning/templates/digid_eherkenning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.429599 django-digid-eherkenning-0.7.0/digid_eherkenning/templates/digid_eherkenning/mock/
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/templates/digid_eherkenning/mock/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/templates/digid_eherkenning/mock/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/templates/digid_eherkenning/mock/password.html
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/templates/digid_eherkenning/post_binding.html
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.429599 django-digid-eherkenning-0.7.0/digid_eherkenning/views/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/views/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/views/digid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/views/eherkenning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/views/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.433599 django-digid-eherkenning-0.7.0/digid_eherkenning/xsd/
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/xsd/eherkenning-dc.xml
--rw-r--r--   0 runner    (1001) docker     (123)    13393 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/xsd/saml-schema-assertion-2.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    16673 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/xsd/saml-schema-metadata-2.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/xsd/xenc-schema.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/digid_eherkenning/xsd/xmldsig-core-schema.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.433599 django-digid-eherkenning-0.7.0/django_digid_eherkenning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-02-21 09:36:58.000000 django-digid-eherkenning-0.7.0/django_digid_eherkenning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-02-21 09:36:58.000000 django-digid-eherkenning-0.7.0/django_digid_eherkenning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 09:36:58.000000 django-digid-eherkenning-0.7.0/django_digid_eherkenning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 09:36:58.000000 django-digid-eherkenning-0.7.0/django_digid_eherkenning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-21 09:36:58.000000 django-digid-eherkenning-0.7.0/django_digid_eherkenning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-21 09:36:58.000000 django-digid-eherkenning-0.7.0/django_digid_eherkenning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/information.md
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-02-21 09:36:58.433599 django-digid-eherkenning-0.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 09:36:58.433599 django-digid-eherkenning-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    30520 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/tests/test_dienst_catalogus_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)    27027 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/tests/test_digid_auth_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/tests/test_digid_logout_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    19555 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/tests/test_digid_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    26927 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/tests/test_eherkenning_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/tests/test_eherkenning_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/tests/test_metadata_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/tests/test_mock_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/tests/test_saml2_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-02-21 09:36:41.000000 django-digid-eherkenning-0.7.0/tests/test_saml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.483860 django-digid-eherkenning-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-21 09:39:17.483860 django-digid-eherkenning-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.459860 django-digid-eherkenning-0.8.0/digid_eherkenning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/digid_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/eherkenning_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.451860 django-digid-eherkenning-0.8.0/digid_eherkenning/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.451860 django-digid-eherkenning-0.8.0/digid_eherkenning/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.459860 django-digid-eherkenning-0.8.0/digid_eherkenning/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.459860 django-digid-eherkenning-0.8.0/digid_eherkenning/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.463860 django-digid-eherkenning-0.8.0/digid_eherkenning/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/management/commands/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/management/commands/generate_digid_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/management/commands/generate_eherkenning_dienstcatalogus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/management/commands/generate_eherkenning_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/management/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/metadata_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.463860 django-digid-eherkenning-0.8.0/digid_eherkenning/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/migrations/0002_auto_20221102_1046.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/migrations/0003_digidconfiguration_artifact_resolve_content_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.463860 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/digid_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.463860 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/idp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/idp/digid_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/idp/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.463860 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/idp/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/idp/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/idp/views/digid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.467860 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/mock/views/digid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/mock_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.467860 django-digid-eherkenning-0.8.0/digid_eherkenning/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/models/digid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/models/eherkenning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.467860 django-digid-eherkenning-0.8.0/digid_eherkenning/saml2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/saml2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/saml2/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/saml2/digid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/saml2/eherkenning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.451860 django-digid-eherkenning-0.8.0/digid_eherkenning/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.467860 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.475860 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    21493 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/RO_DigiD_Logo_Homepage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    69467 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextbold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    84044 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextitalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76489 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextregular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/ajaxLoader.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/app.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    81640 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/application.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/assets_icons_info icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/digid_eo_rgb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/digid_menu_digid_app_phone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/digid_menu_nfc_reader.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/error-darkmode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icon-mail.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icon-smartphone.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icon_error_full-red.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icon_error_full-yellow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/info-darkmode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/info_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/loader.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/loader.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10987 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/nfc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/password.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/ro-favicon-wit-0xffffff.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/session.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/extra.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.475860 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid_eherkenning/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid_eherkenning/login_submit.css
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid_eherkenning/login_submit.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.451860 django-digid-eherkenning-0.8.0/digid_eherkenning/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.451860 django-digid-eherkenning-0.8.0/digid_eherkenning/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.451860 django-digid-eherkenning-0.8.0/digid_eherkenning/templates/admin/digid_eherkenning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.475860 django-digid-eherkenning-0.8.0/digid_eherkenning/templates/admin/digid_eherkenning/digidconfiguration/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/templates/admin/digid_eherkenning/digidconfiguration/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.475860 django-digid-eherkenning-0.8.0/digid_eherkenning/templates/admin/digid_eherkenning/eherkenningconfiguration/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/templates/admin/digid_eherkenning/eherkenningconfiguration/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.475860 django-digid-eherkenning-0.8.0/digid_eherkenning/templates/digid_eherkenning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.475860 django-digid-eherkenning-0.8.0/digid_eherkenning/templates/digid_eherkenning/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/templates/digid_eherkenning/mock/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/templates/digid_eherkenning/mock/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/templates/digid_eherkenning/mock/password.html
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/templates/digid_eherkenning/post_binding.html
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.479860 django-digid-eherkenning-0.8.0/digid_eherkenning/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/views/digid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/views/eherkenning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/views/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.479860 django-digid-eherkenning-0.8.0/digid_eherkenning/xsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/xsd/eherkenning-dc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    13393 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/xsd/saml-schema-assertion-2.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    16673 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/xsd/saml-schema-metadata-2.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/xsd/xenc-schema.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/digid_eherkenning/xsd/xmldsig-core-schema.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.479860 django-digid-eherkenning-0.8.0/django_digid_eherkenning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-21 09:39:17.000000 django-digid-eherkenning-0.8.0/django_digid_eherkenning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-21 09:39:17.000000 django-digid-eherkenning-0.8.0/django_digid_eherkenning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:39:17.000000 django-digid-eherkenning-0.8.0/django_digid_eherkenning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:39:17.000000 django-digid-eherkenning-0.8.0/django_digid_eherkenning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-21 09:39:17.000000 django-digid-eherkenning-0.8.0/django_digid_eherkenning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 09:39:17.000000 django-digid-eherkenning-0.8.0/django_digid_eherkenning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/information.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-21 09:39:17.483860 django-digid-eherkenning-0.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:39:17.483860 django-digid-eherkenning-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30597 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/tests/test_dienst_catalogus_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28266 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/tests/test_digid_auth_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/tests/test_digid_logout_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/tests/test_digid_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27052 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/tests/test_eherkenning_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22531 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/tests/test_eherkenning_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/tests/test_metadata_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/tests/test_mock_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/tests/test_saml2_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-21 09:39:08.000000 django-digid-eherkenning-0.8.0/tests/test_saml_utils.py
```

### Comparing `django-digid-eherkenning-0.7.0/CHANGELOG.rst` & `django-digid-eherkenning-0.8.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =========
 Changelog
 =========
 
+0.8.0 (2023-06-21)
+==================
+
+Feature release
+
+* Added configurable Content-Type header for DigiD SAML
+* Implemented a way to override the global configuration defaults for Level Of Assurance (LOA)
+* [#30] Ensure generated metadata has xml tag
+* [#35] Confirmed support for Django 4.2
+
 0.7.0 (2023-02-21)
 ==================
 
 Quality of life updates
 
 * [#27] Removed Python 3.7 and 3.8 from test matrix (3.7 is EOL, 3.8 is not used in our
   envs anymore)
```

### Comparing `django-digid-eherkenning-0.7.0/LICENSE` & `django-digid-eherkenning-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/PKG-INFO` & `django-digid-eherkenning-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: django-digid-eherkenning
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Django app for DigiD/eHerkenning authentication flows
 Home-page: https://github.com/maykinmedia/django-digid-eherkenning
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Project-URL: Changelog, https://github.com/maykinmedia/django-digid-eherkenning/blob/master/docs/CHANGELOG.rst
 Project-URL: Bug Tracker, https://github.com/maykinmedia/django-digid-eherkenning/issues
 Project-URL: Source Code, https://github.com/maykinmedia/django-digid-eherkenning
 Keywords: django,authentication,digid,eherkenning,eidas,dutch,nl,netherlands
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: tests
 Provides-Extra: pep8
 Provides-Extra: coverage
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 ========================
 django-digid-eherkenning
 ========================
 
-:Version: 0.7.0
+:Version: 0.8.0
 :Source: https://github.com/maykinmedia/django-digid-eherkenning
 :Keywords: django, authentication, digid, eherkenning, eidas, dutch, nl, netherlands
 :PythonVersion: 3.7+
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `django-digid-eherkenning-0.7.0/README.rst` & `django-digid-eherkenning-0.8.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ========================
 django-digid-eherkenning
 ========================
 
-:Version: 0.7.0
+:Version: 0.8.0
 :Source: https://github.com/maykinmedia/django-digid-eherkenning
 :Keywords: django, authentication, digid, eherkenning, eidas, dutch, nl, netherlands
 :PythonVersion: 3.7+
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/admin.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         ),
         (
             _("SAML configuration"),
             {
                 "fields": (
                     "entity_id",
                     "base_url",
+                    "artifact_resolve_content_type",
                     "want_assertions_signed",
                     "want_assertions_encrypted",
                     "signature_algorithm",
                     "digest_algorithm",
                 ),
             },
         ),
```

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/backends.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/backends.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/choices.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/choices.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,10 +29,30 @@
     non_existent = "urn:etoegang:core:assurance-class:loa1", _("Non existent (1)")
     low = "urn:etoegang:core:assurance-class:loa2", _("Low (2)")
     low_plus = "urn:etoegang:core:assurance-class:loa2plus", _("Low (2+)")
     substantial = "urn:etoegang:core:assurance-class:loa3", _("Substantial (3)")
     high = "urn:etoegang:core:assurance-class:loa4", _("High (4)")
 
 
+# ref: https://www.logius.nl/domeinen/toegang/digid/documentatie/koppelvlakspecificatie-digid-saml-authenticatie#index-23
+class DigiDAssuranceLevels(models.TextChoices):
+    base = (
+        "urn:oasis:names:tc:SAML:2.0:ac:classes:PasswordProtectedTransport",
+        _("DigiD Basis"),
+    )
+    middle = (
+        "urn:oasis:names:tc:SAML:2.0:ac:classes:MobileTwoFactorContract",
+        _("DigiD Midden"),
+    )
+    substantial = (
+        "urn:oasis:names:tc:SAML:2.0:ac:classes:Smartcard",
+        _("DigiD Substantieel"),
+    )
+    high = (
+        "urn:oasis:names:tc:SAML:2.0:ac:classes:SmartcardPKI",
+        _("DigiD Hoog"),
+    )
+
+
 class XMLContentTypes(models.TextChoices):
     soap_xml = OneLogin_Saml2_Constants.SOAP_XML, "application/soap+xml"
     text_xml = OneLogin_Saml2_Constants.TEXT_XML, "text/xml"
```

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/digid_urls.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/digid_urls.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/locale/nl/LC_MESSAGES/django.mo` & `django-digid-eherkenning-0.8.0/digid_eherkenning/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/locale/nl/LC_MESSAGES/django.po` & `django-digid-eherkenning-0.8.0/digid_eherkenning/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/management/commands/_base.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/management/commands/generate_digid_metadata.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/management/commands/generate_digid_metadata.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/management/commands/generate_eherkenning_dienstcatalogus.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/management/commands/generate_eherkenning_dienstcatalogus.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/management/commands/generate_eherkenning_metadata.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/management/commands/generate_eherkenning_metadata.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/management/utils.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/management/utils.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/metadata_urls.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/metadata_urls.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/migrations/0001_initial.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/migrations/0002_auto_20221102_1046.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/migrations/0002_auto_20221102_1046.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/mock/backends.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/mock/backends.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/mock/conf.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/mock/conf.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/mock/idp/views/digid.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/mock/idp/views/digid.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/mock/views/digid.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/mock/views/digid.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/models/base.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.utils.encoding import force_str
 from django.utils.translation import gettext_lazy as _
 
 from privates.fields import PrivateMediaFileField
 from simple_certmanager.models import Certificate
 from solo.models import SingletonModel
 
-from ..choices import DigestAlgorithms, SignatureAlgorithms
+from ..choices import DigestAlgorithms, SignatureAlgorithms, XMLContentTypes
 
 
 class ConfigurationManager(models.Manager):
     def get_queryset(self):
         qs = super().get_queryset()
         return qs.select_related("certificate")
 
@@ -53,14 +53,24 @@
     )
     want_assertions_encrypted = models.BooleanField(
         _("want assertions encrypted"),
         default=False,
         help_text=_("If True the XML assertions need to be encrypted."),
         max_length=100,
     )
+    artifact_resolve_content_type = models.CharField(
+        _("resolve artifact binding content type"),
+        choices=XMLContentTypes.choices,
+        default=XMLContentTypes.soap_xml,
+        max_length=100,
+        help_text=_(
+            "'application/soap+xml' is considered legacy and modern brokers typically "
+            "expect 'text/xml'."
+        ),
+    )
     key_passphrase = models.CharField(
         _("key passphrase"),
         blank=True,
         help_text=_("Passphrase for the private key used by the SOAP client."),
         max_length=100,
     )
     signature_algorithm = models.CharField(
```

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/models/digid.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/models/digid.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,8 +84,9 @@
             "technical_contact_person_telephone": self.technical_contact_person_telephone
             or None,
             "technical_contact_person_email": self.technical_contact_person_email
             or None,
             "organization": organization,
             "session_age": get_setting("DIGID_SESSION_AGE"),
             "slo": self.slo,
+            "artifact_resolve_content_type": self.artifact_resolve_content_type,
         }
```

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/models/eherkenning.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/models/eherkenning.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uuid
 
 from django.core.exceptions import ImproperlyConfigured
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
-from ..choices import AssuranceLevels, XMLContentTypes
+from ..choices import AssuranceLevels
 from ..validators import oin_validator
 from .base import BaseConfiguration
 
 
 class EherkenningConfiguration(BaseConfiguration):
     loa = models.CharField(
         _("LoA"),
@@ -106,24 +106,14 @@
     )
     makelaar_id = models.CharField(
         _("broker ID"),
         help_text=_("OIN of the broker used to set up eHerkenning/eIDAS."),
         max_length=100,
         validators=[oin_validator],
     )
-    artifact_resolve_content_type = models.CharField(
-        _("resolve artifact binding content type"),
-        choices=XMLContentTypes.choices,
-        default=XMLContentTypes.soap_xml,
-        max_length=100,
-        help_text=_(
-            "'application/soap+xml' is considered legacy and modern brokers typically "
-            "expect 'text/xml'."
-        ),
-    )
     service_language = models.CharField(
         _("service language"),
         max_length=2,
         default="nl",
         help_text=_("Metadata for eHerkenning/eidas will contain this language key"),
     )
```

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/saml2/base.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/saml2/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,23 @@
             raise OneLogin_Saml2_ValidationError(
                 f"A different IP address ({authn_ip_address})"
                 f"was used when retrieving the AuthNRequest then for retrieving"
                 f" the request to the ACS ({client_ip_address}).",
                 OneLogin_Saml2_ValidationError.WRONG_INRESPONSETO,
             )
 
+        # I remember reading somewhere that the assurance level on the response
+        # SHOULD be checked. But they might not be present on the response.
+        # From the SAML spec (saml-core-2.0-os):
+        #
+        # If the <RequestedAuthnContext> element is present in the query, at least one
+        # <AuthnStatement> element in the set of returned assertions MUST contain an
+        # <AuthnContext> element that satisfies the element in the query (see Section 3.3.2.2.1). It is
+        # OPTIONAL for the complete set of all such matching assertions to be returned in the response.
+
     def create_config(self, config_dict):
         """
         Convert to the format expected by the OneLogin SAML2 library.
         """
         return OneLogin_Saml2_Settings(config_dict, **self.saml2_setting_kwargs)
 
     def create_config_dict(self, conf):
@@ -277,14 +286,17 @@
                 logger.warning(
                     "IDP with entity_id %s not found in metadata, excluding idp "
                     "from settings_dict",
                     conf["service_entity_id"],
                 )
             else:
                 setting_dict["idp"] = parsed_idp_metadata["idp"]
+                setting_dict["idp"]["resolveArtifactBindingContentType"] = conf.get(
+                    "artifact_resolve_content_type", "application/soap+xml"
+                )
 
         telephone = conf.get("technical_contact_person_telephone")
         email = conf.get("technical_contact_person_email")
         if telephone and email:
             setting_dict["contactPerson"] = {
                 "technical": {"telephoneNumber": telephone, "emailAddress": email}
             }
```

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/saml2/digid.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/saml2/digid.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 from django.urls import reverse
 
 from furl import furl
 
+from ..choices import DigiDAssuranceLevels
 from ..models import DigidConfiguration
 from .base import BaseSaml2Client
 
 
 def generate_digid_metadata() -> bytes:
     client = DigiDClient()
     client.saml2_setting_kwargs = {"sp_validation_only": True}
-    return client.create_metadata()
+    metadata = client.create_metadata()
+    return (
+        b"<?xml version='1.0' encoding='UTF-8'?>" + metadata
+        if not metadata.startswith(b"<?xml")
+        else metadata
+    )
 
 
 class DigiDClient(BaseSaml2Client):
     cache_key_prefix = "digid"
     cache_timeout = 60 * 60  # 1 hour
 
+    def __init__(
+        self,
+        *args,
+        loa: DigiDAssuranceLevels = DigiDAssuranceLevels.middle,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        self.loa = loa
+
     @property
     def conf(self) -> dict:
         if not hasattr(self, "_conf"):
             db_config = DigidConfiguration.get_solo()
             self._conf = db_config.as_dict()
             self._conf.setdefault("acs_path", reverse("digid:acs"))
         return self._conf
@@ -46,17 +61,15 @@
                 # None sent for digi-id.
                 "wantAttributeStatement": False,
                 # For DigiD, if the Metadata file expires, we sent them an update. So
                 # there is no need for an expiry date.
                 "metadataValidUntil": "",
                 "metadataCacheDuration": "",
                 "requestedAuthnContextComparison": "minimum",
-                "requestedAuthnContext": [
-                    "urn:oasis:names:tc:SAML:2.0:ac:classes:MobileTwoFactorContract",
-                ],
+                "requestedAuthnContext": [self.loa],
             }
         )
         return super().create_config(config_dict)
 
     def create_authn_request(self, request, return_to=None):
         return super().create_authn_request(
             request,
```

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/saml2/eherkenning.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/saml2/eherkenning.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import binascii
 from base64 import b64encode
 from io import BytesIO
-from typing import List, Optional
+from typing import List, Literal, Union
 from uuid import uuid4
 
 from django.urls import reverse
 from django.utils import timezone
 
 from defusedxml.lxml import tostring
 from furl.furl import furl
 from lxml.builder import ElementMaker
 from lxml.etree import Element
 from OpenSSL import crypto
 
+from ..choices import AssuranceLevels
 from ..models import EherkenningConfiguration
 from ..settings import EHERKENNING_DS_XSD
 from ..utils import validate_xml
 from .base import BaseSaml2Client, get_service_description, get_service_name
 
 namespaces = {
     "xs": "http://www.w3.org/2001/XMLSchema",
@@ -49,15 +50,20 @@
 
     return create_service_catalogus(settings)
 
 
 def generate_eherkenning_metadata():
     client = eHerkenningClient()
     client.saml2_setting_kwargs = {"sp_validation_only": True}
-    return client.create_metadata()
+    metadata = client.create_metadata()
+    return (
+        b"<?xml version='1.0' encoding='UTF-8'?>" + metadata
+        if not metadata.startswith(b"<?xml")
+        else metadata
+    )
 
 
 def xml_datetime(d):
     return d.isoformat(timespec="seconds")
 
 
 def create_language_elements(element_name, option_value, default_language="en"):
@@ -416,14 +422,23 @@
     return attribute_consuming_services
 
 
 class eHerkenningClient(BaseSaml2Client):
     cache_key_prefix = "eherkenning"
     cache_timeout = 60 * 60  # 1 hour
 
+    def __init__(
+        self,
+        *args,
+        loa: Union[AssuranceLevels, Literal[""]] = "",
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        self.loa = loa
+
     @property
     def conf(self) -> dict:
         if not hasattr(self, "_conf"):
             db_config = EherkenningConfiguration.get_solo()
             self._conf = db_config.as_dict()
             self._conf.setdefault("acs_path", reverse("eherkenning:acs"))
         return self._conf
@@ -453,34 +468,29 @@
                     "NameIDFormat": "urn:oasis:names:tc:SAML:1.1:nameid-format:unspecified",
                     "x509cert": certificate,
                     "privateKey": privkey,
                     "privateKeyPassphrase": conf.get("key_passphrase", None),
                 },
             }
         )
-
-        if "idp" in config_dict:
-            config_dict["idp"]["resolveArtifactBindingContentType"] = conf.get(
-                "artifact_resolve_content_type", "application/soap+xml"
-            )
         return config_dict
 
     def create_config(self, config_dict):
         config_dict["security"].update(
             {
                 # See comment in the python3-saml for in  OneLogin_Saml2_Response.validate_num_assertions (onelogin/saml2/response.py)
                 # for why we need this option.
                 "disableSignatureWrappingProtection": True,
                 # For eHerkenning, if the Metadata file expires, we sent them an update. So
                 # there is no need for an expiry date.
                 "metadataValidUntil": "",
                 "metadataCacheDuration": "",
                 "requestedAuthnContextComparison": "minimum",
                 "requestedAuthnContext": [
-                    self.conf["loa"],
+                    self.loa or self.conf["loa"],
                 ],
             }
         )
         return super().create_config(config_dict)
 
     def create_authn_request(
         self, request, return_to=None, attr_consuming_service_index=None, **kwargs
```

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/settings.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/settings.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/RO_DigiD_Logo_Homepage.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/RO_DigiD_Logo_Homepage.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextbold.woff` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextbold.woff`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextitalic.woff` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextitalic.woff`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextregular.woff` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/ROsanswebtextregular.woff`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/ajaxLoader.gif` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/ajaxLoader.gif`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/app.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/app.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/application.css` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/application.css`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/assets_icons_info icon.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/assets_icons_info icon.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/digid_eo_rgb.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/digid_eo_rgb.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/digid_menu_digid_app_phone.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/digid_menu_digid_app_phone.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/digid_menu_nfc_reader.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/digid_menu_nfc_reader.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/error-darkmode.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/error-darkmode.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/error.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/error.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icon-mail.png` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icon-mail.png`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icon-smartphone.png` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icon-smartphone.png`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icon_error_full-red.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icon_error_full-red.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icon_error_full-yellow.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icon_error_full-yellow.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icons.eot` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icons.eot`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icons.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icons.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icons.ttf` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icons.ttf`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icons.woff` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icons.woff`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/icons.woff2` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/icons.woff2`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/info-darkmode.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/info-darkmode.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/info.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/info.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/info_icon.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/info_icon.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/loader.gif` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/loader.gif`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/nfc.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/nfc.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/password.png` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/password.png`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/ro-favicon-wit-0xffffff.png` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/ro-favicon-wit-0xffffff.png`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/assets/session.svg` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/assets/session.svg`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/extra.css` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/extra.css`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/static/digid-mock/extra.js` & `django-digid-eherkenning-0.8.0/digid_eherkenning/static/digid-mock/extra.js`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/templates/digid_eherkenning/mock/base.html` & `django-digid-eherkenning-0.8.0/digid_eherkenning/templates/digid_eherkenning/mock/base.html`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/templates/digid_eherkenning/mock/login.html` & `django-digid-eherkenning-0.8.0/digid_eherkenning/templates/digid_eherkenning/mock/login.html`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/templates/digid_eherkenning/mock/password.html` & `django-digid-eherkenning-0.8.0/digid_eherkenning/templates/digid_eherkenning/mock/password.html`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/templates/digid_eherkenning/post_binding.html` & `django-digid-eherkenning-0.8.0/digid_eherkenning/templates/digid_eherkenning/post_binding.html`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/utils.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/utils.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/views/digid.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/views/digid.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from django.views.decorators.cache import never_cache
 from django.views.decorators.csrf import csrf_exempt
 from django.views.generic.base import TemplateView, View
 
 from onelogin.saml2.soap_logout_request import Soap_Logout_Request
 from onelogin.saml2.utils import OneLogin_Saml2_Error, OneLogin_Saml2_ValidationError
 
-from ..choices import SectorType
+from ..choices import DigiDAssuranceLevels, SectorType
+from ..compat import get_next_page
 from ..forms import SAML2Form
 from ..saml2.digid import DigiDClient
 from ..utils import logout_user
 from .base import get_redirect_url
 
 logger = logging.getLogger(__name__)
 
@@ -31,14 +32,22 @@
 class DigiDLoginView(TemplateView):
     """
     DigiD - 3.3.2 - Stap 2 Authenticatievraag
     """
 
     template_name = "digid_eherkenning/post_binding.html"
 
+    def get_level_of_assurance(self):
+        """
+        Override the default Level of Assurance (middle).
+
+        When overriding this, remember the user has control over the request!
+        """
+        return DigiDAssuranceLevels.middle
+
     def get_relay_state(self):
         """
         TODO: It might be a good idea to sign the relay state.
         But I can't think of a way this could be abused, since
         we re-check the url when processed by the ACS.
         """
         redirect_to = self.request.GET.get("next", "")
@@ -47,15 +56,16 @@
     #
     # TODO: It might be a good idea to change this to a post-verb.
     # I can't think of any realy attack-vectors, but seems like a good
     # idea anyways.
     #
     def get_context_data(self, **kwargs):
         context_data = super().get_context_data(**kwargs)
-        client = DigiDClient()
+        client = DigiDClient(loa=self.get_level_of_assurance())
+
         location, parameters = client.create_authn_request(self.request)
 
         context_data.update(
             {
                 "url": location,
                 "form": SAML2Form(
                     initial={
@@ -131,15 +141,15 @@
     def dispatch(self, request, *args, **kwargs):
         name_id = self.get_name_id(request)
 
         if not name_id:
             raise PermissionDenied(_("You are not authenticated with Digid"))
 
         client = DigiDClient()
-        return_to = self.get_next_page()
+        return_to = get_next_page(self)
         logout_url = client.create_logout_request(
             request, return_to=return_to, name_id=name_id
         )
 
         return HttpResponseRedirect(logout_url)
 
     @staticmethod
```

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/views/metadata.py` & `django-digid-eherkenning-0.8.0/digid_eherkenning/views/metadata.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/xsd/eherkenning-dc.xml` & `django-digid-eherkenning-0.8.0/digid_eherkenning/xsd/eherkenning-dc.xml`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/xsd/saml-schema-assertion-2.0.xsd` & `django-digid-eherkenning-0.8.0/digid_eherkenning/xsd/saml-schema-assertion-2.0.xsd`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/xsd/saml-schema-metadata-2.0.xsd` & `django-digid-eherkenning-0.8.0/digid_eherkenning/xsd/saml-schema-metadata-2.0.xsd`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/xsd/xenc-schema.xsd` & `django-digid-eherkenning-0.8.0/digid_eherkenning/xsd/xenc-schema.xsd`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/digid_eherkenning/xsd/xmldsig-core-schema.xsd` & `django-digid-eherkenning-0.8.0/digid_eherkenning/xsd/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/django_digid_eherkenning.egg-info/PKG-INFO` & `django-digid-eherkenning-0.8.0/django_digid_eherkenning.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: django-digid-eherkenning
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Django app for DigiD/eHerkenning authentication flows
 Home-page: https://github.com/maykinmedia/django-digid-eherkenning
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Project-URL: Changelog, https://github.com/maykinmedia/django-digid-eherkenning/blob/master/docs/CHANGELOG.rst
 Project-URL: Bug Tracker, https://github.com/maykinmedia/django-digid-eherkenning/issues
 Project-URL: Source Code, https://github.com/maykinmedia/django-digid-eherkenning
 Keywords: django,authentication,digid,eherkenning,eidas,dutch,nl,netherlands
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: tests
 Provides-Extra: pep8
 Provides-Extra: coverage
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 ========================
 django-digid-eherkenning
 ========================
 
-:Version: 0.7.0
+:Version: 0.8.0
 :Source: https://github.com/maykinmedia/django-digid-eherkenning
 :Keywords: django, authentication, digid, eherkenning, eidas, dutch, nl, netherlands
 :PythonVersion: 3.7+
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `django-digid-eherkenning-0.7.0/django_digid_eherkenning.egg-info/SOURCES.txt` & `django-digid-eherkenning-0.8.0/django_digid_eherkenning.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.cfg
 setup.py
 digid_eherkenning/__init__.py
 digid_eherkenning/admin.py
 digid_eherkenning/apps.py
 digid_eherkenning/backends.py
 digid_eherkenning/choices.py
+digid_eherkenning/compat.py
 digid_eherkenning/digid_urls.py
 digid_eherkenning/eherkenning_urls.py
 digid_eherkenning/exceptions.py
 digid_eherkenning/forms.py
 digid_eherkenning/managers.py
 digid_eherkenning/metadata_urls.py
 digid_eherkenning/mock_urls.py
@@ -28,14 +29,15 @@
 digid_eherkenning/management/commands/__init__.py
 digid_eherkenning/management/commands/_base.py
 digid_eherkenning/management/commands/generate_digid_metadata.py
 digid_eherkenning/management/commands/generate_eherkenning_dienstcatalogus.py
 digid_eherkenning/management/commands/generate_eherkenning_metadata.py
 digid_eherkenning/migrations/0001_initial.py
 digid_eherkenning/migrations/0002_auto_20221102_1046.py
+digid_eherkenning/migrations/0003_digidconfiguration_artifact_resolve_content_type.py
 digid_eherkenning/migrations/__init__.py
 digid_eherkenning/mock/__init__.py
 digid_eherkenning/mock/backends.py
 digid_eherkenning/mock/conf.py
 digid_eherkenning/mock/digid_urls.py
 digid_eherkenning/mock/idp/__init__.py
 digid_eherkenning/mock/idp/digid_urls.py
```

### Comparing `django-digid-eherkenning-0.7.0/information.md` & `django-digid-eherkenning-0.8.0/information.md`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/setup.cfg` & `django-digid-eherkenning-0.8.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-digid-eherkenning
-version = 0.7.0
+version = 0.8.0
 description = A Django app for DigiD/eHerkenning authentication flows
 long_description = file: README.rst
 url = https://github.com/maykinmedia/django-digid-eherkenning
 project_urls = 
 	Changelog = https://github.com/maykinmedia/django-digid-eherkenning/blob/master/docs/CHANGELOG.rst
 	Bug Tracker = https://github.com/maykinmedia/django-digid-eherkenning/issues
 	Source Code = https://github.com/maykinmedia/django-digid-eherkenning
@@ -13,28 +13,30 @@
 author_email = support@maykinmedia.nl
 keywords = django, authentication, digid, eherkenning, eidas, dutch, nl, netherlands
 classifiers = 
 	Development Status :: 4 - Beta
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	Operating System :: Unix
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	django ~= 3.2.0
+	django >= 3.2.0
 	django-sessionprofile
 	django-simple-certmanager
 	django-solo
 	lxml
 	defusedxml>=0.7.0
 	furl
 	maykin-python3-saml
@@ -99,14 +101,11 @@
 ignore = W293,W291,E501,E261
 exclude = migrations,static,media
 
 [flake8]
 max-line-length = 88
 exclude = env,.tox,doc
 
-[zest.releaser]
-create-wheel = yes
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-digid-eherkenning-0.7.0/tests/test_dienst_catalogus_creation.py` & `django-digid-eherkenning-0.8.0/tests/test_dienst_catalogus_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,14 +282,15 @@
         self.eherkenning_config.organization_name = "Test Organisation"
         self.eherkenning_config.organization_url = "http://test-organisation.nl"
         self.eherkenning_config.save()
 
         eherkenning_dienstcatalogus_metadata = generate_dienst_catalogus_metadata(
             self.eherkenning_config
         )
+        self.assertEqual(eherkenning_dienstcatalogus_metadata[:5], b"<?xml")
         service_catalogue_node = etree.XML(eherkenning_dienstcatalogus_metadata)
 
         signature_algorithm_node = service_catalogue_node.find(
             ".//ds:SignatureMethod",
             namespaces=NAMESPACES,
         )
         self.assertEqual(
```

### Comparing `django-digid-eherkenning-0.7.0/tests/test_digid_auth_views.py` & `django-digid-eherkenning-0.8.0/tests/test_digid_auth_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import urllib
 from base64 import b64decode
 from unittest import skip
 from unittest.mock import patch
 
 from django.conf import settings
 from django.contrib import auth
-from django.test import TestCase, override_settings
+from django.test import RequestFactory, TestCase, override_settings
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 
 import pytest
 import responses
 from freezegun import freeze_time
 from lxml import etree
 from onelogin.saml2.utils import OneLogin_Saml2_Utils
 
+from digid_eherkenning.choices import DigiDAssuranceLevels
+from digid_eherkenning.views import DigiDLoginView
+
 from .project.models import User
 from .utils import create_example_artifact, get_saml_element
 
 
 @pytest.mark.usefixtures("digid_config", "temp_private_root")
 class DigidLoginViewTests(TestCase):
     maxDiff = None
@@ -161,14 +164,43 @@
         self.assertXMLEqual(
             etree.tostring(signature, pretty_print=True).decode("utf-8"),
             etree.tostring(
                 etree.fromstring(expected_signature), pretty_print=True
             ).decode("utf-8"),
         )
 
+    def test_login_views_can_override_minimum_loa(self):
+        class CustomLoginView(DigiDLoginView):
+            def get_level_of_assurance(self):
+                return (
+                    DigiDAssuranceLevels.substantial
+                    if "special" in self.request.GET.get("next")
+                    else DigiDAssuranceLevels.middle
+                )
+
+        request = RequestFactory().get(reverse("digid:login") + "?next=/special")
+
+        response = CustomLoginView.as_view()(request)
+
+        saml_request = b64decode(
+            response.context_data["form"].initial["SAMLRequest"].encode("utf-8")
+        )
+        tree = etree.fromstring(saml_request)
+        auth_context_class_ref = tree.xpath(
+            "samlp:RequestedAuthnContext[@Comparison='minimum']/saml:AuthnContextClassRef",
+            namespaces={
+                "samlp": "urn:oasis:names:tc:SAML:2.0:protocol",
+                "saml": "urn:oasis:names:tc:SAML:2.0:assertion",
+            },
+        )[0]
+
+        self.assertEqual(
+            auth_context_class_ref.text, DigiDAssuranceLevels.substantial.value
+        )
+
 
 @freeze_time("2020-04-09T08:31:46Z")
 @override_settings(LOGIN_URL=reverse("admin:login"))
 @pytest.mark.usefixtures("digid_config", "temp_private_root")
 class DigidAssertionConsumerServiceViewTests(TestCase):
     maxDiff = None
```

### Comparing `django-digid-eherkenning-0.7.0/tests/test_digid_logout_views.py` & `django-digid-eherkenning-0.8.0/tests/test_digid_logout_views.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/tests/test_digid_metadata.py` & `django-digid-eherkenning-0.8.0/tests/test_digid_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             technical_contact_person_email="test@test.nl",
             organization_name="Test organisation",
             organization_url="http://test-organisation.nl",
             test=True,
         )
 
         output = stdout.getvalue()
-        entity_descriptor_node = etree.XML(output)
+        entity_descriptor_node = etree.XML(output.encode("utf-8"))
 
         self.assertEqual(
             "http://test-entity.id", entity_descriptor_node.attrib["entityID"]
         )
 
         sspo_descriptor_node = entity_descriptor_node.find(
             ".//md:SPSSODescriptor",
@@ -199,15 +199,15 @@
             service_description="Test Service Description",
             technical_contact_person_telephone="06123123123",
             test=True,
             stdout=stdout,
         )
 
         output = stdout.getvalue()
-        entity_descriptor_node = etree.XML(output)
+        entity_descriptor_node = etree.XML(output.encode("utf-8"))
 
         contact_email_node = entity_descriptor_node.find(
             ".//md:EmailAddress",
             namespaces=NAME_SPACES,
         )
         contact_telephone_node = entity_descriptor_node.find(
             ".//md:TelephoneNumber",
@@ -234,15 +234,15 @@
             service_name="Test Service Name",
             service_description="Test Service Description",
             organization_url="http://test-organisation.nl",
             test=True,
         )
 
         output = stdout.getvalue()
-        entity_descriptor_node = etree.XML(output)
+        entity_descriptor_node = etree.XML(output.encode("utf-8"))
 
         organisation_name_node = entity_descriptor_node.find(
             ".//md:OrganizationName",
             namespaces=NAME_SPACES,
         )
         organisation_display_node = entity_descriptor_node.find(
             ".//md:OrganizationDisplayName",
@@ -273,15 +273,15 @@
             base_url="http://test-entity.id",
             service_name="Test Service Name",
             service_description="Test Service Description",
             test=True,
         )
 
         output = stdout.getvalue()
-        entity_descriptor_node = etree.XML(output)
+        entity_descriptor_node = etree.XML(output.encode("utf-8"))
 
         single_logout_service_node = entity_descriptor_node.find(
             ".//md:SingleLogoutService",
             namespaces=NAME_SPACES,
         )
         self.assertIsNone(single_logout_service_node)
 
@@ -354,14 +354,15 @@
         self.digid_config.technical_contact_person_telephone = "06123123123"
         self.digid_config.technical_contact_person_email = "test@test.nl"
         self.digid_config.organization_name = "Test organisation"
         self.digid_config.organization_url = "http://test-organisation.nl"
         self.digid_config.save()
 
         digid_metadata = generate_digid_metadata()
+        self.assertEqual(digid_metadata[:5], b"<?xml")
 
         entity_descriptor_node = etree.XML(digid_metadata)
 
         self.assertEqual(
             "http://test-entity.id", entity_descriptor_node.attrib["entityID"]
         )
```

### Comparing `django-digid-eherkenning-0.7.0/tests/test_eherkenning_metadata.py` & `django-digid-eherkenning-0.8.0/tests/test_eherkenning_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             technical_contact_person_email="test@test.nl",
             organization_name="Test organisation",
             organization_url="http://test-organisation.nl",
             test=True,
         )
 
         output = stdout.getvalue()
-        entity_descriptor_node = etree.XML(output)
+        entity_descriptor_node = etree.XML(output.encode("utf-8"))
 
         self.assertEqual(
             "http://test-entity.id", entity_descriptor_node.attrib["entityID"]
         )
 
         sspo_descriptor_node = entity_descriptor_node.find(
             ".//md:SPSSODescriptor",
@@ -205,15 +205,15 @@
             service_name="Test Service Name",
             service_description="Test Service Description",
             technical_contact_person_telephone="06123123123",
             test=True,
         )
 
         output = stdout.getvalue()
-        entity_descriptor_node = etree.XML(output)
+        entity_descriptor_node = etree.XML(output.encode("utf-8"))
 
         contact_email_node = entity_descriptor_node.find(
             ".//md:EmailAddress",
             namespaces=NAME_SPACES,
         )
         contact_telephone_node = entity_descriptor_node.find(
             ".//md:TelephoneNumber",
@@ -240,15 +240,15 @@
             service_name="Test Service Name",
             service_description="Test Service Description",
             organization_url="http://test-organisation.nl",
             test=True,
         )
 
         output = stdout.getvalue()
-        entity_descriptor_node = etree.XML(output)
+        entity_descriptor_node = etree.XML(output.encode("utf-8"))
 
         organisation_name_node = entity_descriptor_node.find(
             ".//md:OrganizationName",
             namespaces=NAME_SPACES,
         )
         organisation_display_node = entity_descriptor_node.find(
             ".//md:OrganizationDisplayName",
@@ -287,15 +287,15 @@
             technical_contact_person_email="test@test.nl",
             organization_name="Test organisation",
             organization_url="http://test-organisation.nl",
             test=True,
         )
 
         output = stdout.getvalue()
-        entity_descriptor_node = etree.XML(output)
+        entity_descriptor_node = etree.XML(output.encode("utf-8"))
 
         attribute_consuming_service_nodes = entity_descriptor_node.findall(
             ".//md:AttributeConsumingService",
             namespaces=NAME_SPACES,
         )
         self.assertEqual(1, len(attribute_consuming_service_nodes))
 
@@ -500,14 +500,15 @@
         self.eherkenning_config.technical_contact_person_telephone = "06123123123"
         self.eherkenning_config.technical_contact_person_email = "test@test.nl"
         self.eherkenning_config.organization_name = "Test organisation"
         self.eherkenning_config.organization_url = "http://test-organisation.nl"
         self.eherkenning_config.save()
 
         eherkenning_metadata = generate_eherkenning_metadata()
+        self.assertEqual(eherkenning_metadata[:5], b"<?xml")
         entity_descriptor_node = etree.XML(eherkenning_metadata)
 
         self.assertEqual(
             "http://test-entity.id", entity_descriptor_node.attrib["entityID"]
         )
 
         sspo_descriptor_node = entity_descriptor_node.find(
```

### Comparing `django-digid-eherkenning-0.7.0/tests/test_eherkenning_views.py` & `django-digid-eherkenning-0.8.0/tests/test_eherkenning_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import urllib
 from base64 import b64decode
 from unittest.mock import patch
 
 from django.conf import settings
-from django.test import TestCase, override_settings
+from django.test import RequestFactory, TestCase, override_settings
 from django.urls import reverse
 from django.utils import timezone
 
 import pytest
 import responses
 from freezegun import freeze_time
 from furl import furl
 from lxml import etree
 from onelogin.saml2.utils import OneLogin_Saml2_Utils
 
+from digid_eherkenning.choices import AssuranceLevels
 from digid_eherkenning.models import EherkenningConfiguration
+from digid_eherkenning.views import eHerkenningLoginView
 
 from .project.models import User
 from .utils import create_example_artifact, get_saml_element
 
 
 @pytest.mark.usefixtures("eherkenning_config", "temp_private_root")
 class eHerkenningLoginViewTests(TestCase):
@@ -114,14 +116,41 @@
         self.assertXMLEqual(
             etree.tostring(signature, pretty_print=True).decode("utf-8"),
             etree.tostring(
                 etree.fromstring(expected_signature), pretty_print=True
             ).decode("utf-8"),
         )
 
+    def test_login_views_can_override_minimum_loa(self):
+        class CustomLoginView(eHerkenningLoginView):
+            def get_level_of_assurance(self):
+                return (
+                    AssuranceLevels.high
+                    if "special" in self.request.GET.get("next")
+                    else AssuranceLevels.middle
+                )
+
+        request = RequestFactory().get(reverse("eherkenning:login") + "?next=/special")
+
+        response = CustomLoginView.as_view()(request)
+
+        saml_request = b64decode(
+            response.context_data["form"].initial["SAMLRequest"].encode("utf-8")
+        )
+        tree = etree.fromstring(saml_request)
+        auth_context_class_ref = tree.xpath(
+            "samlp:RequestedAuthnContext[@Comparison='minimum']/saml:AuthnContextClassRef",
+            namespaces={
+                "samlp": "urn:oasis:names:tc:SAML:2.0:protocol",
+                "saml": "urn:oasis:names:tc:SAML:2.0:assertion",
+            },
+        )[0]
+
+        self.assertEqual(auth_context_class_ref.text, AssuranceLevels.high.value)
+
     @freeze_time("2020-04-09T08:31:46Z")
     @patch("onelogin.saml2.utils.uuid4")
     def test_login_with_attribute_consuming_service_index(self, uuid_mock):
         uuid_mock.hex = "80dd245883b84bd98dacbf3978af3d03"
         url = furl(reverse("eherkenning:login")).set(
             {"attr_consuming_service_index": "2"}
         )
```

### Comparing `django-digid-eherkenning-0.7.0/tests/test_metadata_views.py` & `django-digid-eherkenning-0.8.0/tests/test_metadata_views.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/tests/test_mock_views.py` & `django-digid-eherkenning-0.8.0/tests/test_mock_views.py`

 * *Files identical despite different names*

### Comparing `django-digid-eherkenning-0.7.0/tests/test_saml2_client.py` & `django-digid-eherkenning-0.8.0/tests/test_saml2_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,14 +32,45 @@
 
         digid_client = DigiDClient()
         config_dict = digid_client.create_config_dict(conf)
 
         self.assertIn("wantAssertionsSigned", config_dict["security"])
         self.assertFalse(config_dict["security"]["wantAssertionsSigned"])
 
+    def test_artifact_resolve_content_type_settings_default(self):
+        config = DigidConfiguration.get_solo()
+
+        conf = config.as_dict()
+        conf.setdefault("acs_path", reverse("digid:acs"))
+
+        digid_client = DigiDClient()
+        config_dict = digid_client.create_config_dict(conf)
+
+        self.assertIn("resolveArtifactBindingContentType", config_dict["idp"])
+        self.assertIn(
+            "application/soap+xml",
+            config_dict["idp"]["resolveArtifactBindingContentType"],
+        )
+
+    def test_artifact_resolve_content_type_settings(self):
+        config = DigidConfiguration.get_solo()
+        config.artifact_resolve_content_type = "text/xml"
+        config.save()
+
+        conf = config.as_dict()
+        conf.setdefault("acs_path", reverse("digid:acs"))
+
+        digid_client = DigiDClient()
+        config_dict = digid_client.create_config_dict(conf)
+
+        self.assertIn("resolveArtifactBindingContentType", config_dict["idp"])
+        self.assertIn(
+            "text/xml", config_dict["idp"]["resolveArtifactBindingContentType"]
+        )
+
 
 @pytest.mark.usefixtures("eherkenning_config_defaults", "temp_private_root")
 class EHerkenningClientTests(TestCase):
     def test_wants_assertions_signed_setting_default(self):
         config = EherkenningConfiguration.get_solo()
 
         conf = config.as_dict()
```

### Comparing `django-digid-eherkenning-0.7.0/tests/test_saml_utils.py` & `django-digid-eherkenning-0.8.0/tests/test_saml_utils.py`

 * *Files identical despite different names*

