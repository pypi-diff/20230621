# Comparing `tmp/pretix-mpesa-mz-1.3.1.tar.gz` & `tmp/pretix-mpesa-mz-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-mpesa-mz-1.3.1.tar", last modified: Wed May 17 15:08:12 2023, max compression
+gzip compressed data, was "pretix-mpesa-mz-1.4.0.tar", last modified: Wed Jun 21 18:14:02 2023, max compression
```

## Comparing `pretix-mpesa-mz-1.3.1.tar` & `pretix-mpesa-mz-1.4.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.858750 pretix-mpesa-mz-1.3.1/
--rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1844 2023-05-17 15:08:12.858750 pretix-mpesa-mz-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1549 2023-05-12 13:58:54.000000 pretix-mpesa-mz-1.3.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.632745 pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/
--rw-rw-rw-   0        0        0     1844 2023-05-17 15:08:11.000000 pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1156 2023-05-17 15:08:12.000000 pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 15:08:11.000000 pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-17 15:08:11.000000 pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-17 15:08:11.000000 pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.697746 pretix-mpesa-mz-1.3.1/pretix_mpesamz/
--rw-rw-rw-   0        0        0       23 2023-05-17 15:05:58.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/__init__.py
--rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.535745 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.531745 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de/
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.713746 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.722754 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de_Informal/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de_Informal/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.742749 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     8665 2023-05-17 14:50:26.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/mpesa_api.py
--rw-rw-rw-   0        0        0    15276 2023-05-17 14:49:07.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/payment.py
--rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/signals.py
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.545749 pretix-mpesa-mz-1.3.1/pretix_mpesamz/static/
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.747748 pretix-mpesa-mz-1.3.1/pretix_mpesamz/static/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.551747 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.827750 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
--rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
--rw-rw-rw-   0        0        0     4010 2023-05-03 14:29:30.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
--rw-rw-rw-   0        0        0      377 2023-05-11 17:08:48.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/control.html
--rw-rw-rw-   0        0        0      225 2023-05-11 16:56:59.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/order.html
--rw-rw-rw-   0        0        0      452 2023-05-11 14:57:44.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/payment_pending.html
--rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
--rw-rw-rw-   0        0        0      295 2023-05-12 15:41:12.000000 pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/refund_control.html
--rw-rw-rw-   0        0        0      903 2023-05-17 15:08:12.864749 pretix-mpesa-mz-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-05-11 17:36:42.000000 pretix-mpesa-mz-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 15:08:12.842753 pretix-mpesa-mz-1.3.1/tests/
--rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.3.1/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:14:02.349963 pretix-mpesa-mz-1.4.0/
+-rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1844 2023-06-21 18:14:02.349963 pretix-mpesa-mz-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1549 2023-05-12 13:58:54.000000 pretix-mpesa-mz-1.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-21 18:14:02.212973 pretix-mpesa-mz-1.4.0/pretix_mpesa_mz.egg-info/
+-rw-rw-rw-   0        0        0     1844 2023-06-21 18:14:01.000000 pretix-mpesa-mz-1.4.0/pretix_mpesa_mz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1280 2023-06-21 18:14:01.000000 pretix-mpesa-mz-1.4.0/pretix_mpesa_mz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 18:14:01.000000 pretix-mpesa-mz-1.4.0/pretix_mpesa_mz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-06-21 18:14:01.000000 pretix-mpesa-mz-1.4.0/pretix_mpesa_mz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 18:14:01.000000 pretix-mpesa-mz-1.4.0/pretix_mpesa_mz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 18:14:02.240969 pretix-mpesa-mz-1.4.0/pretix_mpesamz/
+-rw-rw-rw-   0        0        0       23 2023-06-21 18:13:21.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:14:02.138968 pretix-mpesa-mz-1.4.0/pretix_mpesamz/locale/
+drwxrwxrwx   0        0        0        0 2023-06-21 18:14:02.136971 pretix-mpesa-mz-1.4.0/pretix_mpesamz/locale/de/
+drwxrwxrwx   0        0        0        0 2023-06-21 18:14:02.253968 pretix-mpesa-mz-1.4.0/pretix_mpesamz/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-06-21 18:14:02.259969 pretix-mpesa-mz-1.4.0/pretix_mpesamz/locale/de_Informal/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/locale/de_Informal/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-06-21 18:14:02.269968 pretix-mpesa-mz-1.4.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     8665 2023-05-17 14:50:26.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/mpesa_api.py
+-rw-rw-rw-   0        0        0    16623 2023-06-21 18:04:07.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/payment.py
+-rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/signals.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:14:02.144969 pretix-mpesa-mz-1.4.0/pretix_mpesamz/static/
+drwxrwxrwx   0        0        0        0 2023-06-21 18:14:02.276983 pretix-mpesa-mz-1.4.0/pretix_mpesamz/static/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-06-21 18:14:02.148969 pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/
+drwxrwxrwx   0        0        0        0 2023-06-21 18:14:02.338967 pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
+-rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
+-rw-rw-rw-   0        0        0     4010 2023-05-03 14:29:30.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
+-rw-rw-rw-   0        0        0      439 2023-06-21 18:07:10.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/pretix_mpesamz/control.html
+-rw-rw-rw-   0        0        0      225 2023-05-11 16:56:59.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/pretix_mpesamz/order.html
+-rw-rw-rw-   0        0        0      431 2023-06-21 15:38:31.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/pretix_mpesamz/payment_failed.html
+-rw-rw-rw-   0        0        0      246 2023-06-21 15:42:38.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/pretix_mpesamz/payment_pending.html
+-rw-rw-rw-   0        0        0      173 2023-06-21 17:56:52.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/pretix_mpesamz/payment_successful.html
+-rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
+-rw-rw-rw-   0        0        0      295 2023-05-12 15:41:12.000000 pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/pretix_mpesamz/refund_control.html
+-rw-rw-rw-   0        0        0      903 2023-06-21 18:14:02.352970 pretix-mpesa-mz-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-05-11 17:36:42.000000 pretix-mpesa-mz-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 18:14:02.344968 pretix-mpesa-mz-1.4.0/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.0/tests/test_main.py
```

### Comparing `pretix-mpesa-mz-1.3.1/LICENSE` & `pretix-mpesa-mz-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.1/PKG-INFO` & `pretix-mpesa-mz-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mpesa-mz
-Version: 1.3.1
+Version: 1.4.0
 Summary: A plugin to allow payments through the M-Pesa mobile payment platform
 Home-page: https://github.com/ivanruby/pretix-mpesa-mz
 Author: Ivan Ruby
 Author-email: ivanrubyds@gmail.com
 License: Apache
 License-File: LICENSE
```

### Comparing `pretix-mpesa-mz-1.3.1/README.rst` & `pretix-mpesa-mz-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/PKG-INFO` & `pretix-mpesa-mz-1.4.0/pretix_mpesa_mz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mpesa-mz
-Version: 1.3.1
+Version: 1.4.0
 Summary: A plugin to allow payments through the M-Pesa mobile payment platform
 Home-page: https://github.com/ivanruby/pretix-mpesa-mz
 Author: Ivan Ruby
 Author-email: ivanrubyds@gmail.com
 License: Apache
 License-File: LICENSE
```

### Comparing `pretix-mpesa-mz-1.3.1/pretix_mpesa_mz.egg-info/SOURCES.txt` & `pretix-mpesa-mz-1.4.0/pretix_mpesa_mz.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,11 +20,13 @@
 pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
 pretix_mpesamz/static/pretix_mpesamz/.gitkeep
 pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
 pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
 pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
 pretix_mpesamz/templates/pretix_mpesamz/control.html
 pretix_mpesamz/templates/pretix_mpesamz/order.html
+pretix_mpesamz/templates/pretix_mpesamz/payment_failed.html
 pretix_mpesamz/templates/pretix_mpesamz/payment_pending.html
+pretix_mpesamz/templates/pretix_mpesamz/payment_successful.html
 pretix_mpesamz/templates/pretix_mpesamz/redirect.html
 pretix_mpesamz/templates/pretix_mpesamz/refund_control.html
 tests/test_main.py
```

### Comparing `pretix-mpesa-mz-1.3.1/pretix_mpesamz/apps.py` & `pretix-mpesa-mz-1.4.0/pretix_mpesamz/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.1/pretix_mpesamz/mpesa_api.py` & `pretix-mpesa-mz-1.4.0/pretix_mpesamz/mpesa_api.py`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.1/pretix_mpesamz/payment.py` & `pretix-mpesa-mz-1.4.0/pretix_mpesamz/payment.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from django.utils.translation import ugettext_lazy as _
 from django.template.loader import get_template
 from django import forms
 
 from random import randint
 from pretix_mpesamz.mpesa_api import execute_mpesa_c2b
 from pretix_mpesamz.mpesa_api import execute_mpesa_reversal
+import requests
 
 
 class MpesaPayment(BasePaymentProvider):
     identifier = 'mpesa'
 
     ########################################################
     #                   General Settings
@@ -48,14 +49,24 @@
 
     @property
     def payment_completed_text(self):
         return rich_text(self.settings.get('payment_completed_text', as_type=LazyI18nString))
 
     @property
     def settings_form_fields(self):
+        env_field = forms.CharField(
+            label=_('Ambiente'),
+            help_text=_('dev ou prod')
+        )
+
+        backend_field = forms.CharField(
+            label=_('Backend para Callbacks do M-Pesa'),
+            help_text=_('URL da API')
+        )
+
         service_provider_code_field = forms.CharField(
             label=_('Código de Provedor de Serviço M-Pesa'),
             help_text=_('Identificador da entidade fornecido pelo M-Pesa')
         )
 
         api_url_field = forms.CharField(
             label=_('API URL'),
@@ -87,14 +98,16 @@
             label=_('Payment completed text'),
             help_text=_(
                 'Shown to the user when viewing an order with completed payment.'),
             widget=I18nTextarea,
         )
 
         settingsList = [
+            ('env', env_field),
+            ('backend', backend_field),
             ('service_provider_code', service_provider_code_field),
             ('api_url', api_url_field),
             ('api_key', api_key_field),
             ('public_key', public_key_field),
             ('information_text', info_field),
             ('payment_pending_text', pending_field),
             ('payment_completed_text', completed_field)
@@ -131,25 +144,25 @@
                                 'invalid': 'Por favor, introduza um número 84 ou 85 válido'}
                         ))
         return OrderedDict([
             msisdn_field,
         ])
 
     def payment_form_render(self, request):
-
         form = self.payment_form(request)
         template = get_template('pretix_mpesamz/checkout_payment_form.html')
         ctx = {
             'request': request,
             'form': form,
             'information_text': self.information_text,
         }
         return template.render(ctx)
 
     def checkout_confirm_render(self, request):
+        pprint(request)
         template = get_template('pretix_mpesamz/order.html')
         ctx = {
             'information_text': self.information_text,
             'msisdn': request.session.get('payment_%s_msisdn' % self.identifier)
         }
         return template.render(ctx)
 
@@ -167,48 +180,73 @@
                 'msisdn': "258" + str(msisdn),
                 'reference': payment.order.event.slug.replace('-', ''),
                 'third_party_reference': payment.order.code,
                 'amount': str(int(float(payment.amount))),
                 'service_provider_code': self.settings.get('service_provider_code')
             }
 
+            # pprint(vars(payment.order)
+
+            # In production, Returning first leg of async communication
             result = execute_mpesa_c2b(config, payment_data)
             pprint(result)
 
             if result['output_ResponseCode'] == 'INS-0':
-                success_payload = json.dumps({
-                    'success': True,
+                transactionPayload = {
+                    'order': {
+                        'id': payment.order.code,
+                        'event': payment.order.event.slug,
+                        'organizer': payment.order.event.organizer.slug
+                    },
+                    'customer': {
+                        'name': payment.order.invoice_address.name_cached,
+                        'email': payment.order.email,
+                        'phone': str(msisdn)
+                    },
+                    'amount': str(int(float(payment.amount))),
+                    'source': 'ticketing',
+                    'asyncTrackingId': result['output_ConversationID'],
+                }
+
+                pprint(transactionPayload)
+
+                txLocalPayload = json.dumps({
+                    'status': 'pending',
                     'code': result['output_ResponseCode'],
                     'msisdn': msisdn,
                     'conversation': result['output_ConversationID'],
-                    'description': result['output_ResponseDesc'],
-                    'transaction': result['output_TransactionID']
+                    'description': result['output_ResponseDesc']
                 })
-                # Displayed in control panel but not on API order response
-                payment.info = success_payload
 
+                payment.info = txLocalPayload
                 payment.save(update_fields=['info'])
-                payment.confirm()
+
+                backend_url = self.settings.get('backend')
+                requests.post(backend_url, json=transactionPayload, headers={"Content-Type": "application/json"})
+
+                # End leg with pending status
+                return None
             else:
                 error_payload = json.dumps({
-                    'success': False,
+                    'status': 'failed',
                     'code': result['output_ResponseCode'],
                     'msisdn': msisdn,
                     'conversation': result['output_ConversationID'],
                     'description': result['output_ResponseDesc'],
                     'transaction': result['output_TransactionID']
                 })
 
                 # Displayed in control panel but not on API order response
                 payment.info = error_payload
 
                 payment.save(update_fields=['info'])
                 payment.fail()
 
-            return
+                return None
+
         except Exception as e:
             print(repr(e))
 
     def payment_prepare(self, request, payment):
         msisdn = request.session.get('payment_%s_msisdn' % self.identifier, '')
 
         try:
@@ -260,14 +298,15 @@
 
             return
         except Exception as e:
             print(repr(e))
 
     def payment_pending_render(self, request, payment) -> str:
         template = get_template('pretix_mpesamz/payment_pending.html')
+
         if payment.info is not None and 'conversation' in payment.info:
             payment_info = json.loads(payment.info)
         else:
             return _("No payment information available.")
 
         if payment_info['code'] == "INS-6":
             reason = "PIN incorreto"
@@ -374,20 +413,20 @@
     #                   Called to display Order
     #                   info in Control Panel
     ########################################################
 
     def payment_control_render(self, request, payment) -> str:
         template = get_template('pretix_mpesamz/control.html')
 
-        if payment.info is not None and 'conversation' in payment.info:
+        if payment.info is not None and 'status' in payment.info:
             payment_info = json.loads(payment.info)
         else:
             return _("Pagamento via M-Pesa sem sucesso.")
 
         ctx = {
-            'conversationID': payment_info['conversation'],
+            'conversation': payment_info['conversation'],
             'msisdn': payment_info['msisdn'],
             'description': payment_info['description'],
             'code': payment_info['code'],
-            'transaction': payment_info['transaction']
+            'status': payment_info['status']
         }
         return template.render(ctx)
```

### Comparing `pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html` & `pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.1/pretix_mpesamz/templates/pretix_mpesamz/redirect.html` & `pretix-mpesa-mz-1.4.0/pretix_mpesamz/templates/pretix_mpesamz/redirect.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.1/setup.cfg` & `pretix-mpesa-mz-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.3.1/setup.py` & `pretix-mpesa-mz-1.4.0/setup.py`

 * *Files identical despite different names*

