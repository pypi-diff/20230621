# Comparing `tmp/pysatochip-0.14.1.tar.gz` & `tmp/pysatochip-0.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysatochip-0.14.1.tar", last modified: Mon Dec  6 10:50:04 2021, max compression
+gzip compressed data, was "dist/pysatochip-0.14.2.tar", last modified: Fri Feb 11 16:44:07 2022, max compression
```

## Comparing `pysatochip-0.14.1.tar` & `pysatochip-0.14.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 satochip  (1000) satochip  (1000)        0 2021-12-06 10:50:04.000000 pysatochip-0.14.1/
--rwxr-xr-x   0 satochip  (1000) satochip  (1000)     1638 2021-07-09 17:38:14.000000 pysatochip-0.14.1/setup.py
-drwxrwxr-x   0 satochip  (1000) satochip  (1000)        0 2021-12-06 10:50:04.000000 pysatochip-0.14.1/pysatochip/
--rw-rw-r--   0 satochip  (1000) satochip  (1000)   100685 2021-12-06 10:46:52.000000 pysatochip-0.14.1/pysatochip/CardConnector.py
--rw-r--r--   0 satochip  (1000) satochip  (1000)     3693 2021-07-09 17:38:14.000000 pysatochip-0.14.1/pysatochip/util.py
--rw-r--r--   0 satochip  (1000) satochip  (1000)       73 2020-06-04 08:01:42.000000 pysatochip-0.14.1/pysatochip/__init__.py
--rw-rw-r--   0 satochip  (1000) satochip  (1000)     1817 2021-12-06 10:46:52.000000 pysatochip-0.14.1/pysatochip/version.py
-drwxrwxr-x   0 satochip  (1000) satochip  (1000)        0 2021-12-06 10:50:04.000000 pysatochip-0.14.1/pysatochip/__pycache__/
--rw-r--r--   0 satochip  (1000) satochip  (1000)      217 2020-06-05 12:56:41.000000 pysatochip-0.14.1/pysatochip/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 satochip  (1000) satochip  (1000)     3868 2021-07-13 08:10:45.000000 pysatochip-0.14.1/pysatochip/__pycache__/util.cpython-36.pyc
--rw-rw-r--   0 satochip  (1000) satochip  (1000)     3065 2021-11-08 20:28:50.000000 pysatochip-0.14.1/pysatochip/__pycache__/SecureChannel.cpython-36.pyc
--rw-rw-r--   0 satochip  (1000) satochip  (1000)      640 2021-12-06 10:50:01.000000 pysatochip-0.14.1/pysatochip/__pycache__/version.cpython-36.pyc
--rw-r--r--   0 satochip  (1000) satochip  (1000)    14414 2020-06-07 09:58:45.000000 pysatochip-0.14.1/pysatochip/__pycache__/ecc.cpython-36.pyc
--rw-r--r--   0 satochip  (1000) satochip  (1000)     5498 2020-05-29 11:36:46.000000 pysatochip-0.14.1/pysatochip/__pycache__/SatochipCard.cpython-36.pyc
--rw-r--r--   0 satochip  (1000) satochip  (1000)     5770 2020-05-22 20:38:00.000000 pysatochip-0.14.1/pysatochip/__pycache__/TxParser.cpython-36.pyc
--rw-r--r--   0 satochip  (1000) satochip  (1000)     1238 2020-09-18 19:39:19.000000 pysatochip-0.14.1/pysatochip/__pycache__/bip39.cpython-36.pyc
--rw-rw-r--   0 satochip  (1000) satochip  (1000)    18245 2021-11-09 09:35:05.000000 pysatochip-0.14.1/pysatochip/__pycache__/CardDataParser.cpython-36.pyc
--rw-rw-r--   0 satochip  (1000) satochip  (1000)     6554 2021-11-08 20:28:50.000000 pysatochip-0.14.1/pysatochip/__pycache__/JCconstants.cpython-36.pyc
--rw-rw-r--   0 satochip  (1000) satochip  (1000)    66641 2021-12-03 20:21:11.000000 pysatochip-0.14.1/pysatochip/__pycache__/CardConnector.cpython-36.pyc
--rw-r--r--   0 satochip  (1000) satochip  (1000)     1983 2021-07-13 08:10:45.000000 pysatochip-0.14.1/pysatochip/__pycache__/Satochip2FA.cpython-36.pyc
--rw-rw-r--   0 satochip  (1000) satochip  (1000)     5808 2021-11-08 20:28:50.000000 pysatochip-0.14.1/pysatochip/__pycache__/certificate_validator.cpython-36.pyc
--rw-rw-r--   0 satochip  (1000) satochip  (1000)    11244 2021-12-06 10:46:52.000000 pysatochip-0.14.1/pysatochip/JCconstants.py
-drwxrwxr-x   0 satochip  (1000) satochip  (1000)        0 2021-12-06 10:50:04.000000 pysatochip-0.14.1/pysatochip/cert/
--rw-r--r--   0 satochip  (1000) satochip  (1000)     2367 2021-07-09 17:38:14.000000 pysatochip-0.14.1/pysatochip/cert/test-subca-seedkeeper.cert
--rw-r--r--   0 satochip  (1000) satochip  (1000)     2592 2021-07-09 17:38:14.000000 pysatochip-0.14.1/pysatochip/cert/ca.cert
--rw-r--r--   0 satochip  (1000) satochip  (1000)     2419 2021-07-09 17:38:14.000000 pysatochip-0.14.1/pysatochip/cert/subca-satochip.cert
--rw-r--r--   0 satochip  (1000) satochip  (1000)     2479 2021-07-09 17:38:14.000000 pysatochip-0.14.1/pysatochip/cert/test-ca.cert
--rw-rw-r--   0 satochip  (1000) satochip  (1000)     2359 2021-12-06 10:46:52.000000 pysatochip-0.14.1/pysatochip/cert/test-subca-satodime.cert
--rw-r--r--   0 satochip  (1000) satochip  (1000)     2416 2021-07-09 17:38:14.000000 pysatochip-0.14.1/pysatochip/cert/subca-satodime.cert
--rw-r--r--   0 satochip  (1000) satochip  (1000)     2427 2021-07-09 17:38:14.000000 pysatochip-0.14.1/pysatochip/cert/subca-seedkeeper.cert
--rw-rw-r--   0 satochip  (1000) satochip  (1000)     2359 2021-12-06 10:46:52.000000 pysatochip-0.14.1/pysatochip/cert/test-subca-satochip.cert
--rw-rw-r--   0 satochip  (1000) satochip  (1000)    11504 2021-12-06 10:46:52.000000 pysatochip-0.14.1/pysatochip/certificate_validator.py
--rw-rw-r--   0 satochip  (1000) satochip  (1000)    31454 2021-12-06 10:46:52.000000 pysatochip-0.14.1/pysatochip/CardDataParser.py
--rw-r--r--   0 satochip  (1000) satochip  (1000)     9611 2019-12-18 10:25:02.000000 pysatochip-0.14.1/pysatochip/TxParser.py
--rw-r--r--   0 satochip  (1000) satochip  (1000)     4108 2021-07-09 17:38:14.000000 pysatochip-0.14.1/pysatochip/Satochip2FA.py
--rw-r--r--   0 satochip  (1000) satochip  (1000)    18939 2020-06-05 15:16:12.000000 pysatochip-0.14.1/pysatochip/ecc.py
--rw-rw-r--   0 satochip  (1000) satochip  (1000)     4186 2021-11-08 20:26:29.000000 pysatochip-0.14.1/pysatochip/SecureChannel.py
--rw-r--r--   0 satochip  (1000) satochip  (1000)       85 2021-06-28 09:12:08.000000 pysatochip-0.14.1/MANIFEST.in
--rw-rw-r--   0 satochip  (1000) satochip  (1000)     4676 2021-12-06 10:50:04.000000 pysatochip-0.14.1/PKG-INFO
--rw-rw-r--   0 satochip  (1000) satochip  (1000)     2413 2021-12-06 10:46:52.000000 pysatochip-0.14.1/CHANGELOG.md
--rw-r--r--   0 satochip  (1000) satochip  (1000)     3441 2021-06-28 09:12:08.000000 pysatochip-0.14.1/README.md
--rw-rw-r--   0 satochip  (1000) satochip  (1000)       38 2021-12-06 10:50:04.000000 pysatochip-0.14.1/setup.cfg
--rw-r--r--   0 satochip  (1000) satochip  (1000)      132 2021-08-09 07:45:00.000000 pysatochip-0.14.1/requirements.txt
--rw-r--r--   0 satochip  (1000) satochip  (1000)     7652 2020-05-27 19:30:38.000000 pysatochip-0.14.1/LICENSE
-drwxrwxr-x   0 satochip  (1000) satochip  (1000)        0 2021-12-06 10:50:04.000000 pysatochip-0.14.1/pysatochip.egg-info/
--rw-r--r--   0 satochip  (1000) satochip  (1000)        1 2021-12-06 10:50:02.000000 pysatochip-0.14.1/pysatochip.egg-info/dependency_links.txt
--rw-r--r--   0 satochip  (1000) satochip  (1000)     4676 2021-12-06 10:50:02.000000 pysatochip-0.14.1/pysatochip.egg-info/PKG-INFO
--rw-r--r--   0 satochip  (1000) satochip  (1000)       11 2021-12-06 10:50:02.000000 pysatochip-0.14.1/pysatochip.egg-info/top_level.txt
--rw-r--r--   0 satochip  (1000) satochip  (1000)       86 2021-12-06 10:50:02.000000 pysatochip-0.14.1/pysatochip.egg-info/requires.txt
--rw-r--r--   0 satochip  (1000) satochip  (1000)     1440 2021-12-06 10:50:02.000000 pysatochip-0.14.1/pysatochip.egg-info/SOURCES.txt
+drwxrwxr-x   0 satochip  (1000) satochip  (1000)        0 2022-02-11 16:44:07.000000 pysatochip-0.14.2/
+-rwxr-xr-x   0 satochip  (1000) satochip  (1000)     1638 2021-07-09 17:38:14.000000 pysatochip-0.14.2/setup.py
+drwxrwxr-x   0 satochip  (1000) satochip  (1000)        0 2022-02-11 16:44:07.000000 pysatochip-0.14.2/pysatochip/
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)   100876 2022-02-09 19:45:58.000000 pysatochip-0.14.2/pysatochip/CardConnector.py
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     3693 2021-07-09 17:38:14.000000 pysatochip-0.14.2/pysatochip/util.py
+-rw-r--r--   0 satochip  (1000) satochip  (1000)       73 2020-06-04 08:01:42.000000 pysatochip-0.14.2/pysatochip/__init__.py
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)     1817 2022-02-11 15:01:13.000000 pysatochip-0.14.2/pysatochip/version.py
+drwxrwxr-x   0 satochip  (1000) satochip  (1000)        0 2022-02-11 16:44:07.000000 pysatochip-0.14.2/pysatochip/__pycache__/
+-rw-r--r--   0 satochip  (1000) satochip  (1000)      217 2020-06-05 12:56:41.000000 pysatochip-0.14.2/pysatochip/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     3868 2021-07-13 08:10:45.000000 pysatochip-0.14.2/pysatochip/__pycache__/util.cpython-36.pyc
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)     3065 2021-11-08 20:28:50.000000 pysatochip-0.14.2/pysatochip/__pycache__/SecureChannel.cpython-36.pyc
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)      645 2022-02-11 16:44:05.000000 pysatochip-0.14.2/pysatochip/__pycache__/version.cpython-36.pyc
+-rw-r--r--   0 satochip  (1000) satochip  (1000)    14414 2020-06-07 09:58:45.000000 pysatochip-0.14.2/pysatochip/__pycache__/ecc.cpython-36.pyc
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     5498 2020-05-29 11:36:46.000000 pysatochip-0.14.2/pysatochip/__pycache__/SatochipCard.cpython-36.pyc
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     5770 2020-05-22 20:38:00.000000 pysatochip-0.14.2/pysatochip/__pycache__/TxParser.cpython-36.pyc
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     1238 2020-09-18 19:39:19.000000 pysatochip-0.14.2/pysatochip/__pycache__/bip39.cpython-36.pyc
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)    18330 2022-02-10 15:47:28.000000 pysatochip-0.14.2/pysatochip/__pycache__/CardDataParser.cpython-36.pyc
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)     6554 2022-02-03 14:20:03.000000 pysatochip-0.14.2/pysatochip/__pycache__/JCconstants.cpython-36.pyc
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)    66706 2022-02-09 20:10:46.000000 pysatochip-0.14.2/pysatochip/__pycache__/CardConnector.cpython-36.pyc
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     1983 2021-07-13 08:10:45.000000 pysatochip-0.14.2/pysatochip/__pycache__/Satochip2FA.cpython-36.pyc
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)     5808 2022-02-03 14:20:03.000000 pysatochip-0.14.2/pysatochip/__pycache__/certificate_validator.cpython-36.pyc
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)    11244 2021-12-06 10:46:52.000000 pysatochip-0.14.2/pysatochip/JCconstants.py
+drwxrwxr-x   0 satochip  (1000) satochip  (1000)        0 2022-02-11 16:44:07.000000 pysatochip-0.14.2/pysatochip/cert/
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     2367 2021-07-09 17:38:14.000000 pysatochip-0.14.2/pysatochip/cert/test-subca-seedkeeper.cert
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     2592 2021-07-09 17:38:14.000000 pysatochip-0.14.2/pysatochip/cert/ca.cert
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     2419 2021-07-09 17:38:14.000000 pysatochip-0.14.2/pysatochip/cert/subca-satochip.cert
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     2479 2021-07-09 17:38:14.000000 pysatochip-0.14.2/pysatochip/cert/test-ca.cert
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)     2359 2021-12-06 10:46:52.000000 pysatochip-0.14.2/pysatochip/cert/test-subca-satodime.cert
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     2416 2021-07-09 17:38:14.000000 pysatochip-0.14.2/pysatochip/cert/subca-satodime.cert
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     2427 2021-07-09 17:38:14.000000 pysatochip-0.14.2/pysatochip/cert/subca-seedkeeper.cert
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)     2359 2021-12-06 10:46:52.000000 pysatochip-0.14.2/pysatochip/cert/test-subca-satochip.cert
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)    11504 2021-12-06 10:46:52.000000 pysatochip-0.14.2/pysatochip/certificate_validator.py
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)    31556 2022-02-10 15:44:45.000000 pysatochip-0.14.2/pysatochip/CardDataParser.py
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     9611 2019-12-18 10:25:02.000000 pysatochip-0.14.2/pysatochip/TxParser.py
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     4108 2021-07-09 17:38:14.000000 pysatochip-0.14.2/pysatochip/Satochip2FA.py
+-rw-r--r--   0 satochip  (1000) satochip  (1000)    18939 2020-06-05 15:16:12.000000 pysatochip-0.14.2/pysatochip/ecc.py
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)     4186 2021-11-08 20:26:29.000000 pysatochip-0.14.2/pysatochip/SecureChannel.py
+-rw-r--r--   0 satochip  (1000) satochip  (1000)       85 2021-06-28 09:12:08.000000 pysatochip-0.14.2/MANIFEST.in
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)     4676 2022-02-11 16:44:07.000000 pysatochip-0.14.2/PKG-INFO
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)     2648 2022-02-11 16:24:51.000000 pysatochip-0.14.2/CHANGELOG.md
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     3441 2021-06-28 09:12:08.000000 pysatochip-0.14.2/README.md
+-rw-rw-r--   0 satochip  (1000) satochip  (1000)       38 2022-02-11 16:44:07.000000 pysatochip-0.14.2/setup.cfg
+-rw-r--r--   0 satochip  (1000) satochip  (1000)      132 2021-08-09 07:45:00.000000 pysatochip-0.14.2/requirements.txt
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     7652 2020-05-27 19:30:38.000000 pysatochip-0.14.2/LICENSE
+drwxrwxr-x   0 satochip  (1000) satochip  (1000)        0 2022-02-11 16:44:07.000000 pysatochip-0.14.2/pysatochip.egg-info/
+-rw-r--r--   0 satochip  (1000) satochip  (1000)        1 2022-02-11 16:44:05.000000 pysatochip-0.14.2/pysatochip.egg-info/dependency_links.txt
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     4676 2022-02-11 16:44:05.000000 pysatochip-0.14.2/pysatochip.egg-info/PKG-INFO
+-rw-r--r--   0 satochip  (1000) satochip  (1000)       11 2022-02-11 16:44:05.000000 pysatochip-0.14.2/pysatochip.egg-info/top_level.txt
+-rw-r--r--   0 satochip  (1000) satochip  (1000)       86 2022-02-11 16:44:05.000000 pysatochip-0.14.2/pysatochip.egg-info/requires.txt
+-rw-r--r--   0 satochip  (1000) satochip  (1000)     1440 2022-02-11 16:44:06.000000 pysatochip-0.14.2/pysatochip.egg-info/SOURCES.txt
```

### Comparing `pysatochip-0.14.1/setup.py` & `pysatochip-0.14.2/setup.py`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/CardConnector.py` & `pysatochip-0.14.2/pysatochip/CardConnector.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,19 +173,20 @@
         self.setup_done= None
         self.needs_secure_channel= None
         self.sc = None
         # cache PIN
         self.pin_nbr=None
         self.pin=None
         # cache unlock_secret (Satodime)
+        self.is_owner= False # the owner is the user (device) that knows the unlock_secret
         self.unlock_secret= SIZE_UNLOCK_SECRET*[0x00]
         self.unlock_counter= SIZE_UNLOCK_COUNTER*[0x00]
         # Satodime, SeedKeeper or Satochip?
         self.card_filter= card_filter # limit card_select to a subset of [satochip, seedkeeper, satodime]
-        self.card_type= None
+        self.card_type= "card"
         self.cert_pem=None # PEM certificate of device, if any
         # cardservice
         self.cardservice= None #will be instantiated when a card is inserted
         try:
             self.cardrequest = CardRequest(timeout=0, cardType=self.cardtype)
             self.cardservice = self.cardrequest.waitforcard()
             #TODO check ATR and check if more than 1 card?
@@ -287,15 +288,15 @@
         self.pin= None #reset PIN
         self.pin_nbr= None
         self.is_seeded= None
         self.needs_2FA = None
         self.setup_done= None
         self.needs_secure_channel= None
         self.card_present= False
-        self.card_type= None
+        self.card_type= "card"
         if self.cardservice:
             self.cardservice.connection.disconnect()
             self.cardservice= None
         if self.client is not None:
             self.client.request('update_status',False)
         # reset authentikey
         self.parser.authentikey=None
@@ -485,14 +486,15 @@
         (response, sw1, sw2) = self.card_transmit(apdu)
         if (sw1==0x90) and (sw2== 0x00):
             self.set_pin(0, pin0) #cache PIN value
             
             if self.card_type=='Satodime': # cache values 
                self.satodime_set_unlock_counter(response[0:SIZE_UNLOCK_COUNTER])
                self.satodime_set_unlock_secret(response[SIZE_UNLOCK_COUNTER:(SIZE_UNLOCK_COUNTER+SIZE_UNLOCK_SECRET)])
+               self.is_owner= True
                     
         return (response, sw1, sw2)
 
     ###########################################
     #                        BIP32 commands                      #
     ###########################################
 
@@ -2000,15 +2002,17 @@
     #################################
     #                  SATODIME                   #
     #################################
     
     def satodime_set_unlock_secret(self, unlock_secret=[]):
         if unlock_secret==[]:
             unlock_secret= SIZE_UNLOCK_SECRET*[0x00]
+            self.is_owner= False
         self.unlock_secret=unlock_secret
+        self.is_owner= True
     def satodime_set_unlock_counter(self, unlock_counter=[]):
         if unlock_counter==[]:
             unlock_counter= SIZE_UNLOCK_COUNTER*[0x00]
         self.unlock_counter=unlock_counter
     def satodime_increment_unlock_counter(self):
         counter_int= int.from_bytes( self.unlock_counter, byteorder='big', signed=False)
         counter_int+=1
```

### Comparing `pysatochip-0.14.1/pysatochip/util.py` & `pysatochip-0.14.2/pysatochip/util.py`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/version.py` & `pysatochip-0.14.2/pysatochip/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,9 +32,9 @@
 # v0.11.4: minor improvements & more error checks
 # v0.12.1: add SeedKeeper support
 # v0.12.2: add list of 2FA servers to select
 # v0.12.3: patch: downgrade pyscard version in requirements to solve conflicts
 # v0.14.1: add Satodime support
 PYSATOCHIP_MAJOR_VERSION= 0
 PYSATOCHIP_MINOR_VERSION= 14
-PYSATOCHIP_REVISION= 1
+PYSATOCHIP_REVISION= 2
 PYSATOCHIP_VERSION= str(PYSATOCHIP_MAJOR_VERSION) + '.' + str(PYSATOCHIP_MINOR_VERSION) + '.' + str(PYSATOCHIP_REVISION)
```

### Comparing `pysatochip-0.14.1/pysatochip/__pycache__/util.cpython-36.pyc` & `pysatochip-0.14.2/pysatochip/__pycache__/util.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/__pycache__/SecureChannel.cpython-36.pyc` & `pysatochip-0.14.2/pysatochip/__pycache__/SecureChannel.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/__pycache__/version.cpython-36.pyc` & `pysatochip-0.14.2/pysatochip/__pycache__/version.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-00000000: 330d 0d0a 1cea ad61 1907 0000 e300 0000  3......a........
+00000000: 330d 0d0a 397a 0662 1907 0000 e300 0000  3...9z.b........
 00000010: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
 00000020: 0073 6c00 0000 6400 5a00 6401 5a01 6500  .sl...d.Z.d.Z.e.
 00000030: 6402 3e00 6501 1700 5a02 6400 5a03 6403  d.>.e...Z.d.Z.d.
 00000040: 5a04 6503 6402 3e00 6504 1700 5a05 6400  Z.e.d.>.e...Z.d.
 00000050: 5a06 6403 5a07 6506 6402 3e00 6507 1700  Z.d.Z.e.d.>.e...
-00000060: 5a08 6400 5a09 6404 5a0a 6403 5a0b 650c  Z.d.Z.d.Z.d.Z.e.
-00000070: 6509 8301 6405 1700 650c 650a 8301 1700  e...d...e.e.....
-00000080: 6405 1700 650c 650b 8301 1700 5a0d 6406  d...e.e.....Z.d.
-00000090: 5300 2907 e900 0000 00e9 0c00 0000 e908  S.).............
-000000a0: 0000 00e9 0100 0000 e90e 0000 00da 012e  ................
-000000b0: 4e29 0e5a 1f53 4154 4f43 4849 505f 5052  N).Z.SATOCHIP_PR
-000000c0: 4f54 4f43 4f4c 5f4d 414a 4f52 5f56 4552  OTOCOL_MAJOR_VER
-000000d0: 5349 4f4e 5a1f 5341 544f 4348 4950 5f50  SIONZ.SATOCHIP_P
-000000e0: 524f 544f 434f 4c5f 4d49 4e4f 525f 5645  ROTOCOL_MINOR_VE
-000000f0: 5253 494f 4e5a 1953 4154 4f43 4849 505f  RSIONZ.SATOCHIP_
-00000100: 5052 4f54 4f43 4f4c 5f56 4552 5349 4f4e  PROTOCOL_VERSION
-00000110: 5a21 5345 4544 4b45 4550 4552 5f50 524f  Z!SEEDKEEPER_PRO
-00000120: 544f 434f 4c5f 4d41 4a4f 525f 5645 5253  TOCOL_MAJOR_VERS
-00000130: 494f 4e5a 2153 4545 444b 4545 5045 525f  IONZ!SEEDKEEPER_
-00000140: 5052 4f54 4f43 4f4c 5f4d 494e 4f52 5f56  PROTOCOL_MINOR_V
-00000150: 4552 5349 4f4e 5a1b 5345 4544 4b45 4550  ERSIONZ.SEEDKEEP
-00000160: 4552 5f50 524f 544f 434f 4c5f 5645 5253  ER_PROTOCOL_VERS
-00000170: 494f 4e5a 1f53 4154 4f44 494d 455f 5052  IONZ.SATODIME_PR
-00000180: 4f54 4f43 4f4c 5f4d 414a 4f52 5f56 4552  OTOCOL_MAJOR_VER
-00000190: 5349 4f4e 5a1f 5341 544f 4449 4d45 5f50  SIONZ.SATODIME_P
-000001a0: 524f 544f 434f 4c5f 4d49 4e4f 525f 5645  ROTOCOL_MINOR_VE
-000001b0: 5253 494f 4e5a 1953 4154 4f44 494d 455f  RSIONZ.SATODIME_
-000001c0: 5052 4f54 4f43 4f4c 5f56 4552 5349 4f4e  PROTOCOL_VERSION
-000001d0: 5a18 5059 5341 544f 4348 4950 5f4d 414a  Z.PYSATOCHIP_MAJ
-000001e0: 4f52 5f56 4552 5349 4f4e 5a18 5059 5341  OR_VERSIONZ.PYSA
-000001f0: 544f 4348 4950 5f4d 494e 4f52 5f56 4552  TOCHIP_MINOR_VER
-00000200: 5349 4f4e 5a13 5059 5341 544f 4348 4950  SIONZ.PYSATOCHIP
-00000210: 5f52 4556 4953 494f 4eda 0373 7472 da12  _REVISION..str..
-00000220: 5059 5341 544f 4348 4950 5f56 4552 5349  PYSATOCHIP_VERSI
-00000230: 4f4e a900 7209 0000 0072 0900 0000 fa15  ON..r....r......
-00000240: 7079 7361 746f 6368 6970 2f76 6572 7369  pysatochip/versi
-00000250: 6f6e 2e70 79da 083c 6d6f 6475 6c65 3e0b  on.py..<module>.
-00000260: 0000 0073 1800 0000 0401 0401 0c04 0401  ...s............
-00000270: 0401 0c04 0401 0401 0c0c 0401 0401 0401  ................
+00000060: 5a08 6400 5a09 6404 5a0a 6405 5a0b 650c  Z.d.Z.d.Z.d.Z.e.
+00000070: 6509 8301 6406 1700 650c 650a 8301 1700  e...d...e.e.....
+00000080: 6406 1700 650c 650b 8301 1700 5a0d 6407  d...e.e.....Z.d.
+00000090: 5300 2908 e900 0000 00e9 0c00 0000 e908  S.).............
+000000a0: 0000 00e9 0100 0000 e90e 0000 00e9 0200  ................
+000000b0: 0000 da01 2e4e 290e 5a1f 5341 544f 4348  .....N).Z.SATOCH
+000000c0: 4950 5f50 524f 544f 434f 4c5f 4d41 4a4f  IP_PROTOCOL_MAJO
+000000d0: 525f 5645 5253 494f 4e5a 1f53 4154 4f43  R_VERSIONZ.SATOC
+000000e0: 4849 505f 5052 4f54 4f43 4f4c 5f4d 494e  HIP_PROTOCOL_MIN
+000000f0: 4f52 5f56 4552 5349 4f4e 5a19 5341 544f  OR_VERSIONZ.SATO
+00000100: 4348 4950 5f50 524f 544f 434f 4c5f 5645  CHIP_PROTOCOL_VE
+00000110: 5253 494f 4e5a 2153 4545 444b 4545 5045  RSIONZ!SEEDKEEPE
+00000120: 525f 5052 4f54 4f43 4f4c 5f4d 414a 4f52  R_PROTOCOL_MAJOR
+00000130: 5f56 4552 5349 4f4e 5a21 5345 4544 4b45  _VERSIONZ!SEEDKE
+00000140: 4550 4552 5f50 524f 544f 434f 4c5f 4d49  EPER_PROTOCOL_MI
+00000150: 4e4f 525f 5645 5253 494f 4e5a 1b53 4545  NOR_VERSIONZ.SEE
+00000160: 444b 4545 5045 525f 5052 4f54 4f43 4f4c  DKEEPER_PROTOCOL
+00000170: 5f56 4552 5349 4f4e 5a1f 5341 544f 4449  _VERSIONZ.SATODI
+00000180: 4d45 5f50 524f 544f 434f 4c5f 4d41 4a4f  ME_PROTOCOL_MAJO
+00000190: 525f 5645 5253 494f 4e5a 1f53 4154 4f44  R_VERSIONZ.SATOD
+000001a0: 494d 455f 5052 4f54 4f43 4f4c 5f4d 494e  IME_PROTOCOL_MIN
+000001b0: 4f52 5f56 4552 5349 4f4e 5a19 5341 544f  OR_VERSIONZ.SATO
+000001c0: 4449 4d45 5f50 524f 544f 434f 4c5f 5645  DIME_PROTOCOL_VE
+000001d0: 5253 494f 4e5a 1850 5953 4154 4f43 4849  RSIONZ.PYSATOCHI
+000001e0: 505f 4d41 4a4f 525f 5645 5253 494f 4e5a  P_MAJOR_VERSIONZ
+000001f0: 1850 5953 4154 4f43 4849 505f 4d49 4e4f  .PYSATOCHIP_MINO
+00000200: 525f 5645 5253 494f 4e5a 1350 5953 4154  R_VERSIONZ.PYSAT
+00000210: 4f43 4849 505f 5245 5649 5349 4f4e da03  OCHIP_REVISION..
+00000220: 7374 72da 1250 5953 4154 4f43 4849 505f  str..PYSATOCHIP_
+00000230: 5645 5253 494f 4ea9 0072 0a00 0000 720a  VERSION..r....r.
+00000240: 0000 00fa 1570 7973 6174 6f63 6869 702f  .....pysatochip/
+00000250: 7665 7273 696f 6e2e 7079 da08 3c6d 6f64  version.py..<mod
+00000260: 756c 653e 0b00 0000 7318 0000 0004 0104  ule>....s.......
+00000270: 010c 0404 0104 010c 0404 0104 010c 0c04  ................
+00000280: 0104 0104 01                             .....
```

### Comparing `pysatochip-0.14.1/pysatochip/__pycache__/ecc.cpython-36.pyc` & `pysatochip-0.14.2/pysatochip/__pycache__/ecc.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/__pycache__/SatochipCard.cpython-36.pyc` & `pysatochip-0.14.2/pysatochip/__pycache__/SatochipCard.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/__pycache__/TxParser.cpython-36.pyc` & `pysatochip-0.14.2/pysatochip/__pycache__/TxParser.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/__pycache__/bip39.cpython-36.pyc` & `pysatochip-0.14.2/pysatochip/__pycache__/bip39.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/__pycache__/CardDataParser.cpython-36.pyc` & `pysatochip-0.14.2/pysatochip/__pycache__/CardDataParser.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a c994 8961 de7a 0000 e300 0000  3......a.z......
+00000000: 330d 0d0a ed32 0562 447b 0000 e300 0000  3....2.bD{......
 00000010: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
 00000020: 0073 a800 0000 6400 5a00 6401 6402 6c01  .s....d.Z.d.d.l.
 00000030: 5a01 6401 6402 6c02 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6401 6406 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0c 6d0d 5a0d 0100 6408 6409 6c0e  d.l.m.Z...d.d.l.
@@ -857,15 +857,15 @@
 00003580: 6f6e 7365 5f70 6b69 0d02 0000 731e 0000  onse_pki....s...
 00003590: 0000 010a 0214 0310 011c 0114 0112 0112  ................
 000035a0: 0316 0102 0112 0104 010e 0104 010e 017a  ...............z
 000035b0: 2c43 6172 6444 6174 6150 6172 7365 722e  ,CardDataParser.
 000035c0: 7665 7269 6679 5f63 6861 6c6c 656e 6765  verify_challenge
 000035d0: 5f72 6573 706f 6e73 655f 706b 6929 0272  _response_pki).r
 000035e0: 3300 0000 721d 0000 0063 0200 0000 0000  3...r....c......
-000035f0: 0000 1700 0000 1000 0000 4300 0000 73c2  ..........C...s.
+000035f0: 0000 1900 0000 1100 0000 4300 0000 73d4  ..........C...s.
 00003600: 0100 0074 007c 0183 017d 027c 0274 016b  ...t.|...}.|.t.k
 00003610: 0072 2474 0264 017c 029b 0064 0274 019b  .r$t.d.|...d.t..
 00003620: 009d 0483 0182 0164 037d 037c 017c 0319  .......d.}.|.|..
 00003630: 007d 047c 0364 0437 007d 037c 017c 0319  .}.|.d.7.}.|.|..
 00003640: 007d 057c 0364 0437 007d 037c 017c 0319  .}.|.d.7.}.|.|..
 00003650: 007d 067c 0364 0437 007d 037c 017c 037c  .}.|.d.7.}.|.|.|
 00003660: 0374 0317 0085 0219 007d 077c 0374 0337  .t.......}.|.t.7
@@ -875,267 +875,272 @@
 000036a0: 007d 037c 017c 037c 0374 0617 0085 0219  .}.|.|.|.t......
 000036b0: 007d 0a7c 0374 0637 007d 0374 076a 087c  .}.|.t.7.}.t.j.|
 000036c0: 0464 057c 049b 009d 0283 027d 0b74 096a  .d.|.......}.t.j
 000036d0: 087c 0664 057c 069b 009d 0283 027d 0c74  .|.d.|.......}.t
 000036e0: 0a7c 0783 016a 0b83 007d 0d7c 0864 0419  .|...j...}.|.d..
 000036f0: 007d 0e64 0674 0a7c 0864 0764 077c 0e17  .}.d.t.|.d.d.|..
 00003700: 0085 0219 0083 016a 0b83 0017 007d 0f7c  .......j.....}.|
-00003710: 0964 0419 007d 1064 0674 0a7c 0964 0764  .d...}.d.t.|.d.d
-00003720: 077c 1017 0085 0219 0083 016a 0b83 0017  .|.........j....
-00003730: 007d 117c 0a64 0419 007d 1274 0a7c 0a64  .}.|.d...}.t.|.d
-00003740: 0764 077c 1217 0085 0219 0083 016a 0c64  .d.|.........j.d
-00003750: 0883 017d 1364 097d 1464 097d 157c 0674  ...}.d.}.d.}.|.t
-00003760: 0d64 0319 006b 0590 0172 7a7c 0674 0d64  .d...k...rz|.t.d
-00003770: 0419 006b 0090 0172 7a64 0a7d 147c 0674  ...k...rzd.}.|.t
-00003780: 0e64 0319 006b 0590 0172 9a7c 0674 0e64  .d...k...r.|.t.d
-00003790: 0419 006b 0090 0172 9a64 0a7d 157c 047c  ...k...r.d.}.|.|
-000037a0: 057c 067c 077c 087c 097c 0a7c 0b7c 0c7c  .|.|.|.|.|.|.|.|
-000037b0: 0d7c 0f7c 117c 137c 147c 1564 0b9c 0f7d  .|.|.|.|.|.d...}
-000037c0: 167c 1653 0029 0c4e 7a35 5361 746f 6469  .|.S.).Nz5Satodi
-000037d0: 6d65 2065 7272 6f72 3a20 7772 6f6e 6720  me error: wrong 
-000037e0: 6b65 7973 6c6f 7420 7374 6174 7573 2072  keyslot status r
-000037f0: 6573 706f 6e73 6520 6c65 6e67 7468 207a  esponse length z
-00003800: 0b2c 2065 7870 6563 7465 6420 7201 0000  ., expected r...
-00003810: 0072 0800 0000 7a0d 556e 6b6e 6f77 6e20  .r....z.Unknown 
-00003820: 636f 6465 20da 0230 7872 2f00 0000 7a05  code ..0xr/...z.
-00003830: 7574 662d 3846 5429 0fda 0a6b 6579 5f73  utf-8FT)...key_s
-00003840: 7461 7475 73da 086b 6579 5f74 7970 65da  tatus..key_type.
-00003850: 096b 6579 5f61 7373 6574 da0a 6b65 795f  .key_asset..key_
-00003860: 736c 6970 3434 da0c 6b65 795f 636f 6e74  slip44..key_cont
-00003870: 7261 6374 da0b 6b65 795f 746f 6b65 6e69  ract..key_tokeni
-00003880: 64da 086b 6579 5f64 6174 61da 0e6b 6579  d..key_data..key
-00003890: 5f73 7461 7475 735f 7478 74da 0d6b 6579  _status_txt..key
-000038a0: 5f61 7373 6574 5f74 7874 da0e 6b65 795f  _asset_txt..key_
-000038b0: 736c 6970 3434 5f68 6578 da10 6b65 795f  slip44_hex..key_
-000038c0: 636f 6e74 7261 6374 5f68 6578 da0f 6b65  contract_hex..ke
-000038d0: 795f 746f 6b65 6e69 645f 6865 78da 0c6b  y_tokenid_hex..k
-000038e0: 6579 5f64 6174 615f 7478 74da 0869 735f  ey_data_txt..is_
-000038f0: 746f 6b65 6eda 0669 735f 6e66 7429 0f72  token..is_nft).r
-00003900: 2600 0000 da11 5349 5a45 5f4b 4559 5f4d  &.....SIZE_KEY_M
-00003910: 4554 4144 4154 4172 6800 0000 da0b 5349  ETADATArh.....SI
-00003920: 5a45 5f53 4c49 5034 34da 0d53 495a 455f  ZE_SLIP44..SIZE_
-00003930: 434f 4e54 5241 4354 da0c 5349 5a45 5f54  CONTRACT..SIZE_T
-00003940: 4f4b 454e 4944 da09 5349 5a45 5f44 4154  OKENID..SIZE_DAT
-00003950: 41da 0944 4943 5f53 5441 5445 da03 6765  A..DIC_STATE..ge
-00003960: 74da 1144 4943 5f41 5353 4554 5f42 595f  t..DIC_ASSET_BY_
-00003970: 434f 4445 725c 0000 0072 4d00 0000 728b  CODEr\...rM...r.
-00003980: 0000 00da 0b54 4f4b 454e 5f52 414e 4745  .....TOKEN_RANGE
-00003990: da09 4e46 545f 5241 4e47 4529 1772 1700  ..NFT_RANGE).r..
-000039a0: 0000 7233 0000 005a 0b73 7461 7475 735f  ..r3...Z.status_
-000039b0: 7369 7a65 726f 0000 0072 a700 0000 72a8  sizero...r....r.
-000039c0: 0000 0072 a900 0000 72aa 0000 0072 ab00  ...r....r....r..
-000039d0: 0000 72ac 0000 0072 ad00 0000 72ae 0000  ..r....r....r...
-000039e0: 0072 af00 0000 72b0 0000 005a 0d73 697a  .r....r....Z.siz
-000039f0: 655f 636f 6e74 7261 6374 72b1 0000 005a  e_contractr....Z
-00003a00: 0c73 697a 655f 746f 6b65 6e69 6472 b200  .size_tokenidr..
-00003a10: 0000 5a09 7369 7a65 5f64 6174 6172 b300  ..Z.size_datar..
-00003a20: 0000 72b4 0000 0072 b500 0000 da0e 6b65  ..r....r......ke
-00003a30: 7973 6c6f 745f 7374 6174 7573 7219 0000  yslot_statusr...
-00003a40: 0072 1900 0000 721a 0000 00da 2170 6172  .r....r.....!par
-00003a50: 7365 5f73 6174 6f64 696d 655f 6765 745f  se_satodime_get_
-00003a60: 6b65 7973 6c6f 745f 7374 6174 7573 2802  keyslot_status(.
-00003a70: 0000 7352 0000 0000 0308 0108 0114 0104  ..sR............
-00003a80: 0308 0108 0108 0108 0108 0108 0110 0108  ................
-00003a90: 0110 0108 0110 0108 0110 0108 0412 0112  ................
-00003aa0: 010c 0208 011c 0208 011c 0208 011a 0404  ................
-00003ab0: 0104 011c 0104 011c 0104 0204 0106 0104  ................
-00003ac0: 0102 0104 0104 010c 027a 3043 6172 6444  .........z0CardD
-00003ad0: 6174 6150 6172 7365 722e 7061 7273 655f  ataParser.parse_
-00003ae0: 7361 746f 6469 6d65 5f67 6574 5f6b 6579  satodime_get_key
-00003af0: 736c 6f74 5f73 7461 7475 7363 0200 0000  slot_statusc....
-00003b00: 0000 0000 0c00 0000 0700 0000 4300 0000  ............C...
-00003b10: 73aa 0100 0074 007c 0183 017d 0264 017d  s....t.|...}.d.}
-00003b20: 037c 027d 047c 0464 026b 0072 2c74 0164  .|.}.|.d.k.r,t.d
-00003b30: 037c 029b 0064 0464 029b 009d 0483 0182  .|...d.d........
-00003b40: 017c 0164 0119 0064 0514 007c 0164 0619  .|.d...d...|.d..
-00003b50: 0017 007d 057c 0364 0237 007d 037c 0464  ...}.|.d.7.}.|.d
-00003b60: 0238 007d 047c 047c 056b 0072 7074 0164  .8.}.|.|.k.rpt.d
-00003b70: 037c 029b 0064 0464 027c 0517 009b 009d  .|...d.d.|......
-00003b80: 0483 0182 017c 017c 037c 037c 0517 0085  .....|.|.|.|....
-00003b90: 0219 007d 067c 037c 0537 007d 037c 047c  ...}.|.|.7.}.|.|
-00003ba0: 0538 007d 047c 0464 026b 0072 b474 0164  .8.}.|.d.k.r.t.d
-00003bb0: 037c 029b 0064 0464 027c 0517 0064 0217  .|...d.d.|...d..
-00003bc0: 009b 009d 0483 0182 017c 017c 0319 0064  .........|.|...d
-00003bd0: 0514 007c 017c 0364 0617 0019 0017 007d  ...|.|.d.......}
-00003be0: 077c 0364 0237 007d 037c 0464 0238 007d  .|.d.7.}.|.d.8.}
-00003bf0: 047c 047c 076b 0090 0172 0674 0164 037c  .|.|.k...r.t.d.|
-00003c00: 029b 0064 0464 027c 0517 0064 0217 007c  ...d.d.|...d...|
-00003c10: 0717 009b 009d 0483 0182 017c 017c 037c  ...........|.|.|
-00003c20: 037c 0717 0085 0219 007d 087c 037c 0737  .|.......}.|.|.7
-00003c30: 007d 037c 047c 0738 007d 0474 027c 0683  .}.|.|.8.}.t.|..
-00003c40: 016a 0383 007d 0974 046a 0564 077c 099b  .j...}.t.j.d.|..
-00003c50: 0064 087c 006a 066a 0764 0964 0a8d 016a  .d.|.j.j.d.d...j
-00003c60: 0383 009b 009d 0483 0101 007c 006a 087c  ...........|.j.|
-00003c70: 0164 0164 027c 0517 0085 0219 007c 087c  .d.d.|.......|.|
-00003c80: 006a 0683 0301 007c 0664 0b19 0064 0216  .j.....|.d...d..
-00003c90: 007d 0a7c 0664 0164 0c85 0219 007d 0b7c  .}.|.d.d.....}.|
-00003ca0: 0a64 016b 0290 0172 9864 026e 0264 0d7c  .d.k...r.d.n.d.|
-00003cb0: 0b64 013c 007c 067c 0b7c 0866 0353 0029  .d.<.|.|.|.f.S.)
-00003cc0: 0e4e 7201 0000 0072 2f00 0000 7a31 5361  .Nr....r/...z1Sa
-00003cd0: 746f 6469 6d65 2065 7272 6f72 3a20 7772  todime error: wr
-00003ce0: 6f6e 6720 6765 745f 7075 626b 6579 2072  ong get_pubkey r
-00003cf0: 6573 706f 6e73 6520 6c65 6e67 7468 207a  esponse length z
-00003d00: 142c 2065 7870 6563 7465 6420 6174 206c  ., expected at l
-00003d10: 6561 7374 2072 6500 0000 7208 0000 007a  east re...r....z
-00003d20: 1956 6572 6966 7969 6e67 2073 6967 2066  .Verifying sig f
-00003d30: 6f72 2070 7562 6b65 7920 7a13 2075 7369  or pubkey z. usi
-00003d40: 6e67 2061 7574 6865 6e74 696b 6579 2046  ng authentikey F
-00003d50: 2901 724a 0000 0072 7600 0000 723f 0000  ).rJ...rv...r?..
-00003d60: 0072 7400 0000 2909 7226 0000 0072 6800  .rt...).r&...rh.
-00003d70: 0000 725c 0000 0072 4d00 0000 7211 0000  ..r\...rM...r...
-00003d80: 0072 1300 0000 7214 0000 0072 4b00 0000  .r....r....rK...
-00003d90: 7264 0000 0029 0c72 1700 0000 7233 0000  rd...).r....r3..
-00003da0: 00da 0d72 6573 706f 6e73 655f 7369 7a65  ...response_size
-00003db0: 726f 0000 00da 0672 656d 6169 6e72 6b00  ro.....remainrk.
-00003dc0: 0000 da0b 7075 626b 6579 5f6c 6973 7472  ....pubkey_listr
-00003dd0: 3800 0000 da08 7369 675f 6c69 7374 726c  8.....sig_listrl
-00003de0: 0000 005a 0670 6172 6974 79da 1070 7562  ...Z.parity..pub
-00003df0: 6b65 795f 636f 6d70 5f6c 6973 7472 1900  key_comp_listr..
-00003e00: 0000 7219 0000 0072 1a00 0000 da19 7061  ..r....r......pa
-00003e10: 7273 655f 7361 746f 6469 6d65 5f67 6574  rse_satodime_get
-00003e20: 5f70 7562 6b65 7962 0200 0073 3c00 0000  _pubkeyb...s<...
-00003e30: 0003 0801 0401 0403 0801 1401 1401 0801  ................
-00003e40: 0801 0801 1801 1001 0801 0802 0801 1c01  ................
-00003e50: 1801 0801 0801 0a01 2001 1001 0801 0803  ........ .......
-00003e60: 0c01 2401 1c03 0c01 0c01 1601 7a28 4361  ..$.........z(Ca
-00003e70: 7264 4461 7461 5061 7273 6572 2e70 6172  rdDataParser.par
-00003e80: 7365 5f73 6174 6f64 696d 655f 6765 745f  se_satodime_get_
-00003e90: 7075 626b 6579 6303 0000 0000 0000 0011  pubkeyc.........
-00003ea0: 0000 0008 0000 0043 0000 0073 2203 0000  .......C...s"...
-00003eb0: 7400 7c01 8301 7d03 6401 7d04 7c03 7d05  t.|...}.d.}.|.}.
-00003ec0: 7c05 6402 6b00 722c 7401 6403 7c03 9b00  |.d.k.r,t.d.|...
-00003ed0: 6404 6402 9b00 9d04 8301 8201 7c01 6401  d.d.........|.d.
-00003ee0: 1900 6405 1400 7c01 6406 1900 1700 7d06  ..d...|.d.....}.
-00003ef0: 7c04 6402 3700 7d04 7c05 6402 3800 7d05  |.d.7.}.|.d.8.}.
-00003f00: 7c05 7c06 6b00 7270 7401 6403 7c03 9b00  |.|.k.rpt.d.|...
-00003f10: 6404 6402 7c06 1700 9b00 9d04 8301 8201  d.d.|...........
-00003f20: 7c01 7c04 7c04 7402 1700 7403 1700 7402  |.|.|.t...t...t.
-00003f30: 1700 8502 1900 7d07 7c01 7c04 7c04 7402  ......}.|.|.|.t.
-00003f40: 1700 8502 1900 7d08 7c04 7402 3700 7d04  ......}.|.t.7.}.
-00003f50: 7c05 7402 3800 7d05 7c01 7c04 7c04 7403  |.t.8.}.|.|.|.t.
-00003f60: 1700 8502 1900 7d09 7c04 7403 3700 7d04  ......}.|.t.7.}.
-00003f70: 7c05 7403 3800 7d05 7c01 7c04 7c04 7402  |.t.8.}.|.|.|.t.
-00003f80: 1700 8502 1900 7d0a 7c04 7402 3700 7d04  ......}.|.t.7.}.
-00003f90: 7c05 7402 3800 7d05 7c05 6402 6b00 9001  |.t.8.}.|.d.k...
-00003fa0: 720e 7401 6403 7c03 9b00 6404 6402 7c06  r.t.d.|...d.d.|.
-00003fb0: 1700 6402 1700 9b00 9d04 8301 8201 7c01  ..d...........|.
-00003fc0: 7c04 1900 6405 1400 7c01 7c04 6406 1700  |...d...|.|.d...
-00003fd0: 1900 1700 7d0b 7c04 6402 3700 7d04 7c05  ....}.|.d.7.}.|.
-00003fe0: 6402 3800 7d05 7c05 7c0b 6b00 9001 7260  d.8.}.|.|.k...r`
-00003ff0: 7401 6403 7c03 9b00 6404 6402 7c06 1700  t.d.|...d.d.|...
-00004000: 6402 1700 7c0b 1700 9b00 9d04 8301 8201  d...|...........
-00004010: 7c01 7c04 7c04 7c0b 1700 8502 1900 7d0c  |.|.|.|.......}.
-00004020: 7c04 7c0b 3700 7d04 7c05 7c0b 3800 7d05  |.|.7.}.|.|.8.}.
-00004030: 7c05 6402 6b00 9001 72ae 7401 6403 7c03  |.d.k...r.t.d.|.
-00004040: 9b00 6404 6402 7c06 1700 6402 1700 7c0b  ..d.d.|...d...|.
-00004050: 1700 6402 1700 9b00 9d04 8301 8201 7c01  ..d...........|.
-00004060: 7c04 1900 6405 1400 7c01 7c04 6406 1700  |...d...|.|.d...
-00004070: 1900 1700 7d0d 7c04 6402 3700 7d04 7c05  ....}.|.d.7.}.|.
-00004080: 6402 3800 7d05 7c05 7c0d 6b00 9002 7208  d.8.}.|.|.k...r.
-00004090: 7401 6403 7c03 9b00 6404 6402 7c06 1700  t.d.|...d.d.|...
-000040a0: 6402 1700 7c0b 1700 6402 1700 7c0d 1700  d...|...d...|...
-000040b0: 9b00 9d04 8301 8201 7c01 7c04 7c04 7c0d  ........|.|.|.|.
-000040c0: 1700 8502 1900 7d0e 7c04 7c0d 3700 7d04  ......}.|.|.7.}.
-000040d0: 7c05 7c0d 3800 7d05 7c00 6a04 7c01 6401  |.|.8.}.|.j.|.d.
-000040e0: 6402 7c06 1700 6402 1700 7c0b 1700 8502  d.|...d...|.....
-000040f0: 1900 7c0e 7c00 6a05 8303 0100 7c09 7c00  ..|.|.j.....|.|.
-00004100: 6a06 6b03 9002 7282 7401 6407 7407 7c09  j.k...r.t.d.t.|.
-00004110: 8301 6a08 8300 9b00 6408 7c02 9b00 6409  ..j.....d.|...d.
-00004120: 7407 7406 8301 6a08 8300 9b00 9d06 8301  t.t...j.........
-00004130: 8201 7409 8300 7d0f 7c0f 6a0a 7407 7c07  ..t...}.|.j.t.|.
-00004140: 8301 8301 0100 7c0f 6a0b 8300 7d10 740c  ......|.j...}.t.
-00004150: 7c10 8301 7c0c 6b03 9003 7218 740d 6a0e  |...|.k...r.t.j.
-00004160: 640a 8301 0100 740d 6a0e 640b 7407 7c07  d.....t.j.d.t.|.
-00004170: 8301 6a08 8300 9b00 9d02 8301 0100 740d  ..j...........t.
-00004180: 6a0e 640c 7407 7c10 8301 6a08 8300 9b00  j.d.t.|...j.....
-00004190: 9d02 8301 0100 740d 6a0e 640d 7407 7c0c  ......t.j.d.t.|.
-000041a0: 8301 6a08 8300 9b00 9d02 8301 0100 740d  ..j...........t.
-000041b0: 6a0e 640e 8301 0100 7401 640f 7c02 9b00  j.d.....t.d.|...
-000041c0: 6410 9d03 8301 8201 7c07 7c0c 7c0e 6603  d.......|.|.|.f.
-000041d0: 5300 2911 4e72 0100 0000 722f 0000 007a  S.).Nr....r/...z
-000041e0: 3253 6174 6f64 696d 6520 6572 726f 723a  2Satodime error:
-000041f0: 2077 726f 6e67 2067 6574 5f70 7269 766b   wrong get_privk
-00004200: 6579 2072 6573 706f 6e73 6520 6c65 6e67  ey response leng
-00004210: 7468 207a 142c 2065 7870 6563 7465 6420  th z., expected 
-00004220: 6174 206c 6561 7374 2072 6500 0000 7208  at least re...r.
-00004230: 0000 007a 1f53 6174 6f64 696d 6520 6572  ...z.Satodime er
-00004240: 726f 723a 2065 6e74 726f 7079 5f63 6f6f  ror: entropy_coo
-00004250: 7264 7820 7a0d 2066 6f72 206b 6579 736c  rdx z. for keysl
-00004260: 6f74 207a 2320 646f 6573 206e 6f74 206d  ot z# does not m
-00004270: 6174 6368 2061 7574 6865 6e74 696b 6579  atch authentikey
-00004280: 5f63 6f6f 7264 7820 7a28 2323 2323 2323  _coordx z(######
-00004290: 2320 4445 4255 4720 454e 5452 4f50 5920  # DEBUG ENTROPY 
-000042a0: 3d3e 2050 5249 564b 4559 2023 2323 2323  => PRIVKEY #####
-000042b0: 2323 7a0e 656e 7472 6f70 795f 6c69 7374  ##z.entropy_list
-000042c0: 3a20 7a14 656e 7472 6f70 795f 6861 7368  : z.entropy_hash
-000042d0: 5f62 7974 6573 3a20 7a0e 7072 6976 6b65  _bytes: z.privke
-000042e0: 795f 6c69 7374 3a20 7a29 2323 2323 2323  y_list: z)######
-000042f0: 2320 2323 2323 2323 2323 2323 2323 2323  # ##############
-00004300: 2323 2323 2323 2323 2323 2320 2323 2323  ########### ####
-00004310: 2323 237a 3253 6174 6f64 696d 6520 6572  ###z2Satodime er
-00004320: 726f 723a 2072 6563 6f76 6572 6564 2070  ror: recovered p
-00004330: 7269 7661 7465 206b 6579 2066 6f72 206b  rivate key for k
-00004340: 6579 736c 6f74 207a 1820 646f 6573 206e  eyslot z. does n
-00004350: 6f74 206d 6174 6368 2065 6e74 726f 7079  ot match entropy
-00004360: 2129 0f72 2600 0000 7268 0000 00da 0c53  !).r&...rh.....S
-00004370: 495a 455f 454e 5452 4f50 59da 0d53 495a  IZE_ENTROPY..SIZ
-00004380: 455f 4543 434f 4f52 4458 7264 0000 0072  E_ECCOORDXrd...r
-00004390: 1400 0000 7215 0000 0072 5c00 0000 724d  ....r....r\...rM
-000043a0: 0000 0072 0300 0000 7261 0000 0072 6200  ...r....ra...rb.
-000043b0: 0000 da04 6c69 7374 7211 0000 0072 1300  ....listr....r..
-000043c0: 0000 2911 7217 0000 0072 3300 0000 da07  ..).r....r3.....
-000043d0: 6b65 795f 6e62 7272 c200 0000 726f 0000  key_nbrr....ro..
-000043e0: 0072 c300 0000 5a0c 656e 7472 6f70 795f  .r....Z.entropy_
-000043f0: 7369 7a65 da0c 656e 7472 6f70 795f 6c69  size..entropy_li
-00004400: 7374 da0c 656e 7472 6f70 795f 7573 6572  st..entropy_user
-00004410: 5a0e 656e 7472 6f70 795f 636f 6f72 6478  Z.entropy_coordx
-00004420: 5a0c 656e 7472 6f70 795f 6361 7264 5a0c  Z.entropy_cardZ.
-00004430: 7072 6976 6b65 795f 7369 7a65 da0c 7072  privkey_size..pr
-00004440: 6976 6b65 795f 6c69 7374 7238 0000 0072  ivkey_listr8...r
-00004450: c500 0000 7262 0000 005a 1265 6e74 726f  ....rb...Z.entro
-00004460: 7079 5f68 6173 685f 6279 7465 7372 1900  py_hash_bytesr..
-00004470: 0000 7219 0000 0072 1a00 0000 da1a 7061  ..r....r......pa
-00004480: 7273 655f 7361 746f 6469 6d65 5f67 6574  rse_satodime_get
-00004490: 5f70 7269 766b 6579 8b02 0000 736c 0000  _privkey....sl..
-000044a0: 0000 0308 0104 0104 0308 0114 0114 0108  ................
-000044b0: 0108 0108 0118 0118 0110 0108 0108 0110  ................
-000044c0: 0108 0108 0110 0108 0108 030a 011c 0118  ................
-000044d0: 0108 0108 010a 0120 0110 0208 0108 020a  ....... ........
-000044e0: 0124 0118 0108 0108 010a 0128 0110 0108  .$.........(....
-000044f0: 0108 0324 030c 012a 0306 010e 0108 010e  ...$...*........
-00004500: 010a 0118 0118 0118 010a 0110 027a 2943  .............z)C
-00004510: 6172 6444 6174 6150 6172 7365 722e 7061  ardDataParser.pa
-00004520: 7273 655f 7361 746f 6469 6d65 5f67 6574  rse_satodime_get
-00004530: 5f70 7269 766b 6579 4e29 1fda 085f 5f6e  _privkeyN)...__n
-00004540: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00004550: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00004560: 076c 6f67 6769 6e67 da07 5741 524e 494e  .logging..WARNIN
-00004570: 4772 1b00 0000 726a 0000 0072 2800 0000  Gr....rj...r(...
-00004580: 725c 0000 0072 2c00 0000 723b 0000 0072  r\...r,...r;...r
-00004590: 3c00 0000 7249 0000 0072 4e00 0000 725a  <...rI...rN...rZ
-000045a0: 0000 0072 0900 0000 7260 0000 0072 3100  ...r....r`...r1.
-000045b0: 0000 7264 0000 0072 6e00 0000 7272 0000  ..rd...rn...rr..
-000045c0: 0072 5200 0000 728f 0000 0072 9500 0000  .rR...r....r....
-000045d0: 729c 0000 0072 a500 0000 7202 0000 00da  r....r....r.....
-000045e0: 0464 6963 7472 c100 0000 72c7 0000 0072  .dictr....r....r
-000045f0: cf00 0000 7219 0000 0072 1900 0000 7219  ....r....r....r.
-00004600: 0000 0072 1a00 0000 7210 0000 0027 0000  ...r....r....'..
-00004610: 0073 2800 0000 0802 0e07 1412 0819 0806  .s(.............
-00004620: 0822 0822 081f 124b 0825 081d 0813 0818  ."."...K.%......
-00004630: 0843 082f 0813 080c 081b 143a 0829 7210  .C./.......:.)r.
-00004640: 0000 0029 1dda 075f 5f64 6f63 5f5f 72d3  ...)...__doc__r.
-00004650: 0000 0072 9800 0000 5a06 7479 7069 6e67  ...r....Z.typing
-00004660: 7202 0000 00da 0768 6173 686c 6962 7203  r......hashlibr.
-00004670: 0000 005a 0673 7472 7563 7472 0400 0000  ...Z.structr....
-00004680: 7205 0000 005a 0c65 6364 7361 2e63 7572  r....Z.ecdsa.cur
-00004690: 7665 7372 0600 0000 5a0a 6563 6473 612e  vesr....Z.ecdsa.
-000046a0: 7574 696c 7207 0000 00da 0365 6363 7209  utilr......eccr.
-000046b0: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
-000046c0: 0000 720d 0000 0072 0e00 0000 da0b 4a43  ..r....r......JC
-000046d0: 636f 6e73 7461 6e74 73da 0967 6574 4c6f  constants..getLo
-000046e0: 6767 6572 72d0 0000 0072 1100 0000 7212  ggerr....r....r.
-000046f0: 0000 00da 0544 4542 5547 7232 0000 0072  .....DEBUGr2...r
-00004700: 1000 0000 7219 0000 0072 1900 0000 7219  ....r....r....r.
-00004710: 0000 0072 1a00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00004720: 653e 1300 0000 731a 0000 0004 0108 0108  e>....s.........
-00004730: 010c 010c 0110 010c 010c 0220 0108 020a  ........... ....
-00004740: 010c 0204 05                             .....
+00003710: 0964 0419 007d 1074 0a7c 0964 0764 077c  .d...}.t.|.d.d.|
+00003720: 1017 0085 0219 0083 017d 1164 067c 116a  .........}.d.|.j
+00003730: 0b83 0017 007d 1274 0c6a 0d7c 1164 0883  .....}.t.j.|.d..
+00003740: 027d 137c 0a64 0419 007d 1474 0a7c 0a64  .}.|.d...}.t.|.d
+00003750: 0764 077c 1417 0085 0219 0083 016a 0e64  .d.|.........j.d
+00003760: 0983 017d 1564 0a7d 1664 0a7d 177c 0674  ...}.d.}.d.}.|.t
+00003770: 0f64 0319 006b 0590 0172 8a7c 0674 0f64  .d...k...r.|.t.d
+00003780: 0419 006b 0090 0172 8a64 0b7d 167c 0674  ...k...r.d.}.|.t
+00003790: 1064 0319 006b 0590 0172 aa7c 0674 1064  .d...k...r.|.t.d
+000037a0: 0419 006b 0090 0172 aa64 0b7d 177c 047c  ...k...r.d.}.|.|
+000037b0: 057c 067c 077c 087c 097c 0a7c 0b7c 0c7c  .|.|.|.|.|.|.|.|
+000037c0: 0d7c 0f7c 127c 137c 157c 167c 1764 0c9c  .|.|.|.|.|.|.d..
+000037d0: 107d 187c 1853 0029 0d4e 7a35 5361 746f  .}.|.S.).Nz5Sato
+000037e0: 6469 6d65 2065 7272 6f72 3a20 7772 6f6e  dime error: wron
+000037f0: 6720 6b65 7973 6c6f 7420 7374 6174 7573  g keyslot status
+00003800: 2072 6573 706f 6e73 6520 6c65 6e67 7468   response length
+00003810: 207a 0b2c 2065 7870 6563 7465 6420 7201   z., expected r.
+00003820: 0000 0072 0800 0000 7a0d 556e 6b6e 6f77  ...r....z.Unknow
+00003830: 6e20 636f 6465 20da 0230 7872 2f00 0000  n code ..0xr/...
+00003840: da03 6269 677a 0575 7466 2d38 4654 2910  ..bigz.utf-8FT).
+00003850: da0a 6b65 795f 7374 6174 7573 da08 6b65  ..key_status..ke
+00003860: 795f 7479 7065 da09 6b65 795f 6173 7365  y_type..key_asse
+00003870: 74da 0a6b 6579 5f73 6c69 7034 34da 0c6b  t..key_slip44..k
+00003880: 6579 5f63 6f6e 7472 6163 74da 0b6b 6579  ey_contract..key
+00003890: 5f74 6f6b 656e 6964 da08 6b65 795f 6461  _tokenid..key_da
+000038a0: 7461 da0e 6b65 795f 7374 6174 7573 5f74  ta..key_status_t
+000038b0: 7874 da0d 6b65 795f 6173 7365 745f 7478  xt..key_asset_tx
+000038c0: 74da 0e6b 6579 5f73 6c69 7034 345f 6865  t..key_slip44_he
+000038d0: 78da 106b 6579 5f63 6f6e 7472 6163 745f  x..key_contract_
+000038e0: 6865 78da 0f6b 6579 5f74 6f6b 656e 6964  hex..key_tokenid
+000038f0: 5f68 6578 da0f 6b65 795f 746f 6b65 6e69  _hex..key_tokeni
+00003900: 645f 696e 74da 0c6b 6579 5f64 6174 615f  d_int..key_data_
+00003910: 7478 74da 0869 735f 746f 6b65 6eda 0669  txt..is_token..i
+00003920: 735f 6e66 7429 1172 2600 0000 da11 5349  s_nft).r&.....SI
+00003930: 5a45 5f4b 4559 5f4d 4554 4144 4154 4172  ZE_KEY_METADATAr
+00003940: 6800 0000 da0b 5349 5a45 5f53 4c49 5034  h.....SIZE_SLIP4
+00003950: 34da 0d53 495a 455f 434f 4e54 5241 4354  4..SIZE_CONTRACT
+00003960: da0c 5349 5a45 5f54 4f4b 454e 4944 da09  ..SIZE_TOKENID..
+00003970: 5349 5a45 5f44 4154 41da 0944 4943 5f53  SIZE_DATA..DIC_S
+00003980: 5441 5445 da03 6765 74da 1144 4943 5f41  TATE..get..DIC_A
+00003990: 5353 4554 5f42 595f 434f 4445 725c 0000  SSET_BY_CODEr\..
+000039a0: 0072 4d00 0000 7228 0000 00da 0a66 726f  .rM...r(.....fro
+000039b0: 6d5f 6279 7465 7372 8b00 0000 da0b 544f  m_bytesr......TO
+000039c0: 4b45 4e5f 5241 4e47 45da 094e 4654 5f52  KEN_RANGE..NFT_R
+000039d0: 414e 4745 2919 7217 0000 0072 3300 0000  ANGE).r....r3...
+000039e0: 5a0b 7374 6174 7573 5f73 697a 6572 6f00  Z.status_sizero.
+000039f0: 0000 72a8 0000 0072 a900 0000 72aa 0000  ..r....r....r...
+00003a00: 0072 ab00 0000 72ac 0000 0072 ad00 0000  .r....r....r....
+00003a10: 72ae 0000 0072 af00 0000 72b0 0000 0072  r....r....r....r
+00003a20: b100 0000 5a0d 7369 7a65 5f63 6f6e 7472  ....Z.size_contr
+00003a30: 6163 7472 b200 0000 5a0c 7369 7a65 5f74  actr....Z.size_t
+00003a40: 6f6b 656e 6964 5a11 6b65 795f 746f 6b65  okenidZ.key_toke
+00003a50: 6e69 645f 6279 7465 7372 b300 0000 72b4  nid_bytesr....r.
+00003a60: 0000 005a 0973 697a 655f 6461 7461 72b5  ...Z.size_datar.
+00003a70: 0000 0072 b600 0000 72b7 0000 00da 0e6b  ...r....r......k
+00003a80: 6579 736c 6f74 5f73 7461 7475 7372 1900  eyslot_statusr..
+00003a90: 0000 7219 0000 0072 1a00 0000 da21 7061  ..r....r.....!pa
+00003aa0: 7273 655f 7361 746f 6469 6d65 5f67 6574  rse_satodime_get
+00003ab0: 5f6b 6579 736c 6f74 5f73 7461 7475 7328  _keyslot_status(
+00003ac0: 0200 0073 5600 0000 0003 0801 0801 1401  ...sV...........
+00003ad0: 0403 0801 0801 0801 0801 0801 0801 1001  ................
+00003ae0: 0801 1001 0801 1001 0801 1001 0804 1201  ................
+00003af0: 1201 0c02 0801 1c02 0801 1401 0c01 0c02  ................
+00003b00: 0801 1a04 0401 0401 1c01 0401 1c01 0402  ................
+00003b10: 0401 0601 0401 0201 0401 0601 0c02 7a30  ..............z0
+00003b20: 4361 7264 4461 7461 5061 7273 6572 2e70  CardDataParser.p
+00003b30: 6172 7365 5f73 6174 6f64 696d 655f 6765  arse_satodime_ge
+00003b40: 745f 6b65 7973 6c6f 745f 7374 6174 7573  t_keyslot_status
+00003b50: 6302 0000 0000 0000 000c 0000 0007 0000  c...............
+00003b60: 0043 0000 0073 aa01 0000 7400 7c01 8301  .C...s....t.|...
+00003b70: 7d02 6401 7d03 7c02 7d04 7c04 6402 6b00  }.d.}.|.}.|.d.k.
+00003b80: 722c 7401 6403 7c02 9b00 6404 6402 9b00  r,t.d.|...d.d...
+00003b90: 9d04 8301 8201 7c01 6401 1900 6405 1400  ......|.d...d...
+00003ba0: 7c01 6406 1900 1700 7d05 7c03 6402 3700  |.d.....}.|.d.7.
+00003bb0: 7d03 7c04 6402 3800 7d04 7c04 7c05 6b00  }.|.d.8.}.|.|.k.
+00003bc0: 7270 7401 6403 7c02 9b00 6404 6402 7c05  rpt.d.|...d.d.|.
+00003bd0: 1700 9b00 9d04 8301 8201 7c01 7c03 7c03  ..........|.|.|.
+00003be0: 7c05 1700 8502 1900 7d06 7c03 7c05 3700  |.......}.|.|.7.
+00003bf0: 7d03 7c04 7c05 3800 7d04 7c04 6402 6b00  }.|.|.8.}.|.d.k.
+00003c00: 72b4 7401 6403 7c02 9b00 6404 6402 7c05  r.t.d.|...d.d.|.
+00003c10: 1700 6402 1700 9b00 9d04 8301 8201 7c01  ..d...........|.
+00003c20: 7c03 1900 6405 1400 7c01 7c03 6406 1700  |...d...|.|.d...
+00003c30: 1900 1700 7d07 7c03 6402 3700 7d03 7c04  ....}.|.d.7.}.|.
+00003c40: 6402 3800 7d04 7c04 7c07 6b00 9001 7206  d.8.}.|.|.k...r.
+00003c50: 7401 6403 7c02 9b00 6404 6402 7c05 1700  t.d.|...d.d.|...
+00003c60: 6402 1700 7c07 1700 9b00 9d04 8301 8201  d...|...........
+00003c70: 7c01 7c03 7c03 7c07 1700 8502 1900 7d08  |.|.|.|.......}.
+00003c80: 7c03 7c07 3700 7d03 7c04 7c07 3800 7d04  |.|.7.}.|.|.8.}.
+00003c90: 7402 7c06 8301 6a03 8300 7d09 7404 6a05  t.|...j...}.t.j.
+00003ca0: 6407 7c09 9b00 6408 7c00 6a06 6a07 6409  d.|...d.|.j.j.d.
+00003cb0: 640a 8d01 6a03 8300 9b00 9d04 8301 0100  d...j...........
+00003cc0: 7c00 6a08 7c01 6401 6402 7c05 1700 8502  |.j.|.d.d.|.....
+00003cd0: 1900 7c08 7c00 6a06 8303 0100 7c06 640b  ..|.|.j.....|.d.
+00003ce0: 1900 6402 1600 7d0a 7c06 6401 640c 8502  ..d...}.|.d.d...
+00003cf0: 1900 7d0b 7c0a 6401 6b02 9001 7298 6402  ..}.|.d.k...r.d.
+00003d00: 6e02 640d 7c0b 6401 3c00 7c06 7c0b 7c08  n.d.|.d.<.|.|.|.
+00003d10: 6603 5300 290e 4e72 0100 0000 722f 0000  f.S.).Nr....r/..
+00003d20: 007a 3153 6174 6f64 696d 6520 6572 726f  .z1Satodime erro
+00003d30: 723a 2077 726f 6e67 2067 6574 5f70 7562  r: wrong get_pub
+00003d40: 6b65 7920 7265 7370 6f6e 7365 206c 656e  key response len
+00003d50: 6774 6820 7a14 2c20 6578 7065 6374 6564  gth z., expected
+00003d60: 2061 7420 6c65 6173 7420 7265 0000 0072   at least re...r
+00003d70: 0800 0000 7a19 5665 7269 6679 696e 6720  ....z.Verifying 
+00003d80: 7369 6720 666f 7220 7075 626b 6579 207a  sig for pubkey z
+00003d90: 1320 7573 696e 6720 6175 7468 656e 7469  . using authenti
+00003da0: 6b65 7920 4629 0172 4a00 0000 7276 0000  key F).rJ...rv..
+00003db0: 0072 3f00 0000 7274 0000 0029 0972 2600  .r?...rt...).r&.
+00003dc0: 0000 7268 0000 0072 5c00 0000 724d 0000  ..rh...r\...rM..
+00003dd0: 0072 1100 0000 7213 0000 0072 1400 0000  .r....r....r....
+00003de0: 724b 0000 0072 6400 0000 290c 7217 0000  rK...rd...).r...
+00003df0: 0072 3300 0000 da0d 7265 7370 6f6e 7365  .r3.....response
+00003e00: 5f73 697a 6572 6f00 0000 da06 7265 6d61  _sizero.....rema
+00003e10: 696e 726b 0000 00da 0b70 7562 6b65 795f  inrk.....pubkey_
+00003e20: 6c69 7374 7238 0000 00da 0873 6967 5f6c  listr8.....sig_l
+00003e30: 6973 7472 6c00 0000 5a06 7061 7269 7479  istrl...Z.parity
+00003e40: da10 7075 626b 6579 5f63 6f6d 705f 6c69  ..pubkey_comp_li
+00003e50: 7374 7219 0000 0072 1900 0000 721a 0000  str....r....r...
+00003e60: 00da 1970 6172 7365 5f73 6174 6f64 696d  ...parse_satodim
+00003e70: 655f 6765 745f 7075 626b 6579 6402 0000  e_get_pubkeyd...
+00003e80: 733c 0000 0000 0308 0104 0104 0308 0114  s<..............
+00003e90: 0114 0108 0108 0108 0118 0110 0108 0108  ................
+00003ea0: 0208 011c 0118 0108 0108 010a 0120 0110  ............. ..
+00003eb0: 0108 0108 030c 0124 011c 030c 010c 0116  .......$........
+00003ec0: 017a 2843 6172 6444 6174 6150 6172 7365  .z(CardDataParse
+00003ed0: 722e 7061 7273 655f 7361 746f 6469 6d65  r.parse_satodime
+00003ee0: 5f67 6574 5f70 7562 6b65 7963 0300 0000  _get_pubkeyc....
+00003ef0: 0000 0000 1100 0000 0800 0000 4300 0000  ............C...
+00003f00: 7322 0300 0074 007c 0183 017d 0364 017d  s"...t.|...}.d.}
+00003f10: 047c 037d 057c 0564 026b 0072 2c74 0164  .|.}.|.d.k.r,t.d
+00003f20: 037c 039b 0064 0464 029b 009d 0483 0182  .|...d.d........
+00003f30: 017c 0164 0119 0064 0514 007c 0164 0619  .|.d...d...|.d..
+00003f40: 0017 007d 067c 0464 0237 007d 047c 0564  ...}.|.d.7.}.|.d
+00003f50: 0238 007d 057c 057c 066b 0072 7074 0164  .8.}.|.|.k.rpt.d
+00003f60: 037c 039b 0064 0464 027c 0617 009b 009d  .|...d.d.|......
+00003f70: 0483 0182 017c 017c 047c 0474 0217 0074  .....|.|.|.t...t
+00003f80: 0317 0074 0217 0085 0219 007d 077c 017c  ...t.......}.|.|
+00003f90: 047c 0474 0217 0085 0219 007d 087c 0474  .|.t.......}.|.t
+00003fa0: 0237 007d 047c 0574 0238 007d 057c 017c  .7.}.|.t.8.}.|.|
+00003fb0: 047c 0474 0317 0085 0219 007d 097c 0474  .|.t.......}.|.t
+00003fc0: 0337 007d 047c 0574 0338 007d 057c 017c  .7.}.|.t.8.}.|.|
+00003fd0: 047c 0474 0217 0085 0219 007d 0a7c 0474  .|.t.......}.|.t
+00003fe0: 0237 007d 047c 0574 0238 007d 057c 0564  .7.}.|.t.8.}.|.d
+00003ff0: 026b 0090 0172 0e74 0164 037c 039b 0064  .k...r.t.d.|...d
+00004000: 0464 027c 0617 0064 0217 009b 009d 0483  .d.|...d........
+00004010: 0182 017c 017c 0419 0064 0514 007c 017c  ...|.|...d...|.|
+00004020: 0464 0617 0019 0017 007d 0b7c 0464 0237  .d.......}.|.d.7
+00004030: 007d 047c 0564 0238 007d 057c 057c 0b6b  .}.|.d.8.}.|.|.k
+00004040: 0090 0172 6074 0164 037c 039b 0064 0464  ...r`t.d.|...d.d
+00004050: 027c 0617 0064 0217 007c 0b17 009b 009d  .|...d...|......
+00004060: 0483 0182 017c 017c 047c 047c 0b17 0085  .....|.|.|.|....
+00004070: 0219 007d 0c7c 047c 0b37 007d 047c 057c  ...}.|.|.7.}.|.|
+00004080: 0b38 007d 057c 0564 026b 0090 0172 ae74  .8.}.|.d.k...r.t
+00004090: 0164 037c 039b 0064 0464 027c 0617 0064  .d.|...d.d.|...d
+000040a0: 0217 007c 0b17 0064 0217 009b 009d 0483  ...|...d........
+000040b0: 0182 017c 017c 0419 0064 0514 007c 017c  ...|.|...d...|.|
+000040c0: 0464 0617 0019 0017 007d 0d7c 0464 0237  .d.......}.|.d.7
+000040d0: 007d 047c 0564 0238 007d 057c 057c 0d6b  .}.|.d.8.}.|.|.k
+000040e0: 0090 0272 0874 0164 037c 039b 0064 0464  ...r.t.d.|...d.d
+000040f0: 027c 0617 0064 0217 007c 0b17 0064 0217  .|...d...|...d..
+00004100: 007c 0d17 009b 009d 0483 0182 017c 017c  .|...........|.|
+00004110: 047c 047c 0d17 0085 0219 007d 0e7c 047c  .|.|.......}.|.|
+00004120: 0d37 007d 047c 057c 0d38 007d 057c 006a  .7.}.|.|.8.}.|.j
+00004130: 047c 0164 0164 027c 0617 0064 0217 007c  .|.d.d.|...d...|
+00004140: 0b17 0085 0219 007c 0e7c 006a 0583 0301  .......|.|.j....
+00004150: 007c 097c 006a 066b 0390 0272 8274 0164  .|.|.j.k...r.t.d
+00004160: 0774 077c 0983 016a 0883 009b 0064 087c  .t.|...j.....d.|
+00004170: 029b 0064 0974 0774 0683 016a 0883 009b  ...d.t.t...j....
+00004180: 009d 0683 0182 0174 0983 007d 0f7c 0f6a  .......t...}.|.j
+00004190: 0a74 077c 0783 0183 0101 007c 0f6a 0b83  .t.|.......|.j..
+000041a0: 007d 1074 0c7c 1083 017c 0c6b 0390 0372  .}.t.|...|.k...r
+000041b0: 1874 0d6a 0e64 0a83 0101 0074 0d6a 0e64  .t.j.d.....t.j.d
+000041c0: 0b74 077c 0783 016a 0883 009b 009d 0283  .t.|...j........
+000041d0: 0101 0074 0d6a 0e64 0c74 077c 1083 016a  ...t.j.d.t.|...j
+000041e0: 0883 009b 009d 0283 0101 0074 0d6a 0e64  ...........t.j.d
+000041f0: 0d74 077c 0c83 016a 0883 009b 009d 0283  .t.|...j........
+00004200: 0101 0074 0d6a 0e64 0e83 0101 0074 0164  ...t.j.d.....t.d
+00004210: 0f7c 029b 0064 109d 0383 0182 017c 077c  .|...d.......|.|
+00004220: 0c7c 0e66 0353 0029 114e 7201 0000 0072  .|.f.S.).Nr....r
+00004230: 2f00 0000 7a32 5361 746f 6469 6d65 2065  /...z2Satodime e
+00004240: 7272 6f72 3a20 7772 6f6e 6720 6765 745f  rror: wrong get_
+00004250: 7072 6976 6b65 7920 7265 7370 6f6e 7365  privkey response
+00004260: 206c 656e 6774 6820 7a14 2c20 6578 7065   length z., expe
+00004270: 6374 6564 2061 7420 6c65 6173 7420 7265  cted at least re
+00004280: 0000 0072 0800 0000 7a1f 5361 746f 6469  ...r....z.Satodi
+00004290: 6d65 2065 7272 6f72 3a20 656e 7472 6f70  me error: entrop
+000042a0: 795f 636f 6f72 6478 207a 0d20 666f 7220  y_coordx z. for 
+000042b0: 6b65 7973 6c6f 7420 7a23 2064 6f65 7320  keyslot z# does 
+000042c0: 6e6f 7420 6d61 7463 6820 6175 7468 656e  not match authen
+000042d0: 7469 6b65 795f 636f 6f72 6478 207a 2823  tikey_coordx z(#
+000042e0: 2323 2323 2323 2044 4542 5547 2045 4e54  ###### DEBUG ENT
+000042f0: 524f 5059 203d 3e20 5052 4956 4b45 5920  ROPY => PRIVKEY 
+00004300: 2323 2323 2323 237a 0e65 6e74 726f 7079  #######z.entropy
+00004310: 5f6c 6973 743a 207a 1465 6e74 726f 7079  _list: z.entropy
+00004320: 5f68 6173 685f 6279 7465 733a 207a 0e70  _hash_bytes: z.p
+00004330: 7269 766b 6579 5f6c 6973 743a 207a 2923  rivkey_list: z)#
+00004340: 2323 2323 2323 2023 2323 2323 2323 2323  ###### #########
+00004350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004360: 2023 2323 2323 2323 7a32 5361 746f 6469   #######z2Satodi
+00004370: 6d65 2065 7272 6f72 3a20 7265 636f 7665  me error: recove
+00004380: 7265 6420 7072 6976 6174 6520 6b65 7920  red private key 
+00004390: 666f 7220 6b65 7973 6c6f 7420 7a18 2064  for keyslot z. d
+000043a0: 6f65 7320 6e6f 7420 6d61 7463 6820 656e  oes not match en
+000043b0: 7472 6f70 7921 290f 7226 0000 0072 6800  tropy!).r&...rh.
+000043c0: 0000 da0c 5349 5a45 5f45 4e54 524f 5059  ....SIZE_ENTROPY
+000043d0: da0d 5349 5a45 5f45 4343 4f4f 5244 5872  ..SIZE_ECCOORDXr
+000043e0: 6400 0000 7214 0000 0072 1500 0000 725c  d...r....r....r\
+000043f0: 0000 0072 4d00 0000 7203 0000 0072 6100  ...rM...r....ra.
+00004400: 0000 7262 0000 00da 046c 6973 7472 1100  ..rb.....listr..
+00004410: 0000 7213 0000 0029 1172 1700 0000 7233  ..r....).r....r3
+00004420: 0000 00da 076b 6579 5f6e 6272 72c5 0000  .....key_nbrr...
+00004430: 0072 6f00 0000 72c6 0000 005a 0c65 6e74  .ro...r....Z.ent
+00004440: 726f 7079 5f73 697a 65da 0c65 6e74 726f  ropy_size..entro
+00004450: 7079 5f6c 6973 74da 0c65 6e74 726f 7079  py_list..entropy
+00004460: 5f75 7365 725a 0e65 6e74 726f 7079 5f63  _userZ.entropy_c
+00004470: 6f6f 7264 785a 0c65 6e74 726f 7079 5f63  oordxZ.entropy_c
+00004480: 6172 645a 0c70 7269 766b 6579 5f73 697a  ardZ.privkey_siz
+00004490: 65da 0c70 7269 766b 6579 5f6c 6973 7472  e..privkey_listr
+000044a0: 3800 0000 72c8 0000 0072 6200 0000 5a12  8...r....rb...Z.
+000044b0: 656e 7472 6f70 795f 6861 7368 5f62 7974  entropy_hash_byt
+000044c0: 6573 7219 0000 0072 1900 0000 721a 0000  esr....r....r...
+000044d0: 00da 1a70 6172 7365 5f73 6174 6f64 696d  ...parse_satodim
+000044e0: 655f 6765 745f 7072 6976 6b65 798d 0200  e_get_privkey...
+000044f0: 0073 6c00 0000 0003 0801 0401 0403 0801  .sl.............
+00004500: 1401 1401 0801 0801 0801 1801 1801 1001  ................
+00004510: 0801 0801 1001 0801 0801 1001 0801 0803  ................
+00004520: 0a01 1c01 1801 0801 0801 0a01 2001 1002  ............ ...
+00004530: 0801 0802 0a01 2401 1801 0801 0801 0a01  ......$.........
+00004540: 2801 1001 0801 0803 2403 0c01 2a03 0601  (.......$...*...
+00004550: 0e01 0801 0e01 0a01 1801 1801 1801 0a01  ................
+00004560: 1002 7a29 4361 7264 4461 7461 5061 7273  ..z)CardDataPars
+00004570: 6572 2e70 6172 7365 5f73 6174 6f64 696d  er.parse_satodim
+00004580: 655f 6765 745f 7072 6976 6b65 794e 291f  e_get_privkeyN).
+00004590: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+000045a0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+000045b0: 6d65 5f5f da07 6c6f 6767 696e 67da 0757  me__..logging..W
+000045c0: 4152 4e49 4e47 721b 0000 0072 6a00 0000  ARNINGr....rj...
+000045d0: 7228 0000 0072 5c00 0000 722c 0000 0072  r(...r\...r,...r
+000045e0: 3b00 0000 723c 0000 0072 4900 0000 724e  ;...r<...rI...rN
+000045f0: 0000 0072 5a00 0000 7209 0000 0072 6000  ...rZ...r....r`.
+00004600: 0000 7231 0000 0072 6400 0000 726e 0000  ..r1...rd...rn..
+00004610: 0072 7200 0000 7252 0000 0072 8f00 0000  .rr...rR...r....
+00004620: 7295 0000 0072 9c00 0000 72a5 0000 0072  r....r....r....r
+00004630: 0200 0000 da04 6469 6374 72c4 0000 0072  ......dictr....r
+00004640: ca00 0000 72d2 0000 0072 1900 0000 7219  ....r....r....r.
+00004650: 0000 0072 1900 0000 721a 0000 0072 1000  ...r....r....r..
+00004660: 0000 2700 0000 7328 0000 0008 020e 0714  ..'...s(........
+00004670: 1208 1908 0608 2208 2208 1f12 4b08 2508  ......"."...K.%.
+00004680: 1d08 1308 1808 4308 2f08 1308 0c08 1b14  ......C./.......
+00004690: 3c08 2972 1000 0000 291d da07 5f5f 646f  <.)r....)...__do
+000046a0: 635f 5f72 d600 0000 7298 0000 005a 0674  c__r....r....Z.t
+000046b0: 7970 696e 6772 0200 0000 da07 6861 7368  ypingr......hash
+000046c0: 6c69 6272 0300 0000 5a06 7374 7275 6374  libr....Z.struct
+000046d0: 7204 0000 0072 0500 0000 5a0c 6563 6473  r....r....Z.ecds
+000046e0: 612e 6375 7276 6573 7206 0000 005a 0a65  a.curvesr....Z.e
+000046f0: 6364 7361 2e75 7469 6c72 0700 0000 da03  cdsa.utilr......
+00004700: 6563 6372 0900 0000 720a 0000 0072 0b00  eccr....r....r..
+00004710: 0000 720c 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00004720: 00da 0b4a 4363 6f6e 7374 616e 7473 da09  ...JCconstants..
+00004730: 6765 744c 6f67 6765 7272 d300 0000 7211  getLoggerr....r.
+00004740: 0000 0072 1200 0000 da05 4445 4255 4772  ...r......DEBUGr
+00004750: 3200 0000 7210 0000 0072 1900 0000 7219  2...r....r....r.
+00004760: 0000 0072 1900 0000 721a 0000 00da 083c  ...r....r......<
+00004770: 6d6f 6475 6c65 3e13 0000 0073 1a00 0000  module>....s....
+00004780: 0401 0801 0801 0c01 0c01 1001 0c01 0c02  ................
+00004790: 2001 0802 0a01 0c02 0405                  .........
```

### Comparing `pysatochip-0.14.1/pysatochip/__pycache__/JCconstants.cpython-36.pyc` & `pysatochip-0.14.2/pysatochip/__pycache__/JCconstants.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 7a88 8961 ec2b 0000 e300 0000  3...z..a.+......
+00000000: 330d 0d0a 1cea ad61 ec2b 0000 e300 0000  3......a.+......
 00000010: 0000 0000 0000 0000 000a 0000 0040 0000  .............@..
 00000020: 0073 c000 0000 6400 5a00 6401 5a01 6402  .s....d.Z.d.Z.d.
 00000030: 5a02 6403 5a03 6402 5a04 6402 5a05 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a06 6405 5a07 6405 5a08 6404 5a09 6420  Z.d.Z.d.Z.d.Z.d 
 00000050: 5a0a 6421 5a0b 6422 5a0c 6407 6509 1700  Z.d!Z.d"Z.d.e...
 00000060: 650a 1700 650b 1700 650c 1700 5a0d 6408  e...e...e...Z.d.
 00000070: 5a0e 6409 5a0f 6406 5a10 640a 640b 640c  Z.d.Z.d.Z.d.d.d.
```

### Comparing `pysatochip-0.14.1/pysatochip/__pycache__/CardConnector.cpython-36.pyc` & `pysatochip-0.14.2/pysatochip/__pycache__/CardConnector.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a b825 aa61 4d89 0100 e300 0000  3....%.aM.......
+00000000: 330d 0d0a f619 0462 0c8a 0100 e300 0000  3......b........
 00000010: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
 00000020: 0073 8002 0000 6400 6401 6c00 6d01 5a01  .s....d.d.l.m.Z.
 00000030: 0100 6400 6402 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000040: 6403 6c04 6d05 5a05 0100 6400 6404 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 6d08 5a08 0100 6400 6405 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 6d0b 5a0b 0100 6400 6406 6c0c  m.Z.m.Z...d.d.l.
 00000070: 6d0d 5a0d 6d0e 5a0e 0100 6400 6407 6c0f  m.Z.m.Z...d.d.l.
@@ -286,15 +286,15 @@
 000011d0: 6e6e 656c da1c 6361 7264 5f69 6e69 7469  nnel..card_initi
 000011e0: 6174 655f 7365 6375 7265 5f63 6861 6e6e  ate_secure_chann
 000011f0: 656c da06 636c 6965 6e74 da07 7265 7175  el..client..requ
 00001200: 6573 74da 0b63 6172 645f 6669 6c74 6572  est..card_filter
 00001210: 290f 7236 0000 005a 0a6f 6273 6572 7661  ).r6...Z.observa
 00001220: 626c 655a 0761 6374 696f 6e73 5a0a 6164  bleZ.actionsZ.ad
 00001230: 6465 6463 6172 6473 5a0c 7265 6d6f 7665  dedcardsZ.remove
-00001240: 6463 6172 6473 5a04 6361 7264 5a0d 7265  dcardsZ.cardZ.re
+00001240: 6463 6172 6473 da04 6361 7264 5a0d 7265  dcards..cardZ.re
 00001250: 7370 6f6e 7365 5f43 504c 43da 0373 7731  sponse_CPLC..sw1
 00001260: da03 7377 325a 0c72 6573 706f 6e73 655f  ..sw2Z.response_
 00001270: 4949 4e5a 0c72 6573 706f 6e73 655f 4349  IINZ.response_CI
 00001280: 4eda 0365 7863 7222 0000 00da 0673 7461  N..excr".....sta
 00001290: 7475 73da 036d 7367 7237 0000 0072 3700  tus..msgr7...r7.
 000012a0: 0000 7238 0000 0072 3900 0000 5a00 0000  ..r8...r9...Z...
 000012b0: 7354 0000 0000 0108 010e 0216 0108 0108  sT..............
@@ -360,3807 +360,3811 @@
 00001670: 0029 a9da 0d43 6172 6443 6f6e 6e65 6374  .)...CardConnect
 00001680: 6f72 7201 0000 00e9 a400 0000 7243 0000  orr.........rC..
 00001690: 00e9 5300 0000 e961 0000 00e9 7400 0000  ..S....a....t...
 000016a0: e96f 0000 00e9 4300 0000 e968 0000 00e9  .o....C....h....
 000016b0: 6900 0000 e970 0000 00e9 6500 0000 e964  i....p....e....d
 000016c0: 0000 00e9 4b00 0000 e972 0000 00e9 4400  ....K....r....D.
 000016d0: 0000 e96d 0000 004e 6304 0000 0000 0000  ...m...Nc.......
-000016e0: 0004 0000 000b 0000 0043 0000 0073 1801  .........C...s..
+000016e0: 0004 0000 000b 0000 0043 0000 0073 1e01  .........C...s..
 000016f0: 0000 7400 6a01 7c02 8301 0100 7400 6a02  ..t.j.|.....t.j.
 00001700: 6401 7403 7c02 8301 9b00 9d02 8301 0100  d.t.|...........
 00001710: 7400 6a04 6402 8301 0100 7400 7c00 5f00  t.j.d.....t.|._.
 00001720: 7405 7c02 8301 7c00 5f06 7c01 7c00 5f07  t.|...|._.|.|._.
 00001730: 7c00 6a07 6400 6b09 7250 7c00 7c00 6a07  |.j.d.k.rP|.|.j.
 00001740: 5f08 7409 8300 7c00 5f0a 6400 7c00 5f0b  _.t...|._.d.|._.
 00001750: 6400 7c00 5f0c 6400 7c00 5f0d 6400 7c00  d.|._.d.|._.d.|.
 00001760: 5f0e 6400 7c00 5f0f 6400 7c00 5f10 6400  _.d.|._.d.|._.d.
-00001770: 7c00 5f11 7412 6403 6701 1400 7c00 5f13  |._.t.d.g...|._.
-00001780: 7414 6403 6701 1400 7c00 5f15 7c03 7c00  t.d.g...|._.|.|.
-00001790: 5f16 6400 7c00 5f17 6400 7c00 5f18 6400  _.d.|._.d.|._.d.
-000017a0: 7c00 5f19 7926 741a 6403 7c00 6a0a 6404  |._.y&t.d.|.j.d.
-000017b0: 8d02 7c00 5f1b 7c00 6a1b 6a1c 8300 7c00  ..|._.|.j.j...|.
-000017c0: 5f19 6405 7c00 5f1d 5700 6e1a 0400 741e  _.d.|._.W.n...t.
-000017d0: 6b0a 72f2 0100 0100 0100 6406 7c00 5f1d  k.r.......d.|._.
-000017e0: 5900 6e02 5800 741f 8300 7c00 5f20 7421  Y.n.X.t...|._ t!
-000017f0: 7c00 8301 7c00 5f22 7c00 6a20 6a23 7c00  |...|._"|.j j#|.
-00001800: 6a22 8301 0100 6400 5300 2907 4e7a 164c  j"....d.S.).Nz.L
-00001810: 6f67 6769 6e67 2073 6574 2074 6f20 6c65  ogging set to le
-00001820: 7665 6c3a 207a 0b49 6e20 5f5f 696e 6974  vel: z.In __init
-00001830: 5f5f 7201 0000 0029 02da 0774 696d 656f  __r....)...timeo
-00001840: 7574 5a08 6361 7264 5479 7065 5446 2924  utZ.cardTypeTF)$
-00001850: 7227 0000 00da 0873 6574 4c65 7665 6c72  r'.....setLevelr
-00001860: 2800 0000 da03 7374 7272 3400 0000 720e  (.....strr4...r.
-00001870: 0000 00da 0670 6172 7365 7272 5a00 0000  .....parserrZ...
-00001880: 723e 0000 0072 0200 0000 5a08 6361 7264  r>...r....Z.card
-00001890: 7479 7065 da09 6e65 6564 735f 3246 41da  type..needs_2FA.
-000018a0: 0969 735f 7365 6564 6564 da0a 7365 7475  .is_seeded..setu
-000018b0: 705f 646f 6e65 7258 0000 00da 0273 63da  p_donerX.....sc.
-000018c0: 0770 696e 5f6e 6272 da03 7069 6eda 1253  .pin_nbr..pin..S
-000018d0: 495a 455f 554e 4c4f 434b 5f53 4543 5245  IZE_UNLOCK_SECRE
-000018e0: 54da 0d75 6e6c 6f63 6b5f 7365 6372 6574  T..unlock_secret
-000018f0: da13 5349 5a45 5f55 4e4c 4f43 4b5f 434f  ..SIZE_UNLOCK_CO
-00001900: 554e 5445 52da 0e75 6e6c 6f63 6b5f 636f  UNTER..unlock_co
-00001910: 756e 7465 7272 5c00 0000 da09 6361 7264  unterr\.....card
-00001920: 5f74 7970 65da 0863 6572 745f 7065 6d72  _type..cert_pemr
-00001930: 4700 0000 7203 0000 005a 0b63 6172 6472  G...r....Z.cardr
-00001940: 6571 7565 7374 5a0b 7761 6974 666f 7263  equestZ.waitforc
-00001950: 6172 6472 4600 0000 7208 0000 0072 0500  ardrF...r....r..
-00001960: 0000 5a0b 6361 7264 6d6f 6e69 746f 7272  ..Z.cardmonitorr
-00001970: 3d00 0000 5a0c 6361 7264 6f62 7365 7276  =...Z.cardobserv
-00001980: 6572 7249 0000 0029 0472 3600 0000 725a  errI...).r6...rZ
-00001990: 0000 005a 086c 6f67 6c65 7665 6c72 5c00  ...Z.loglevelr\.
-000019a0: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
-000019b0: 0072 4000 0000 a100 0000 733e 0000 0000  .r@.......s>....
-000019c0: 010a 0114 010a 0106 010a 0106 010a 0108  ................
-000019d0: 0108 0106 0106 0106 0106 0106 0206 0106  ................
-000019e0: 020c 010c 0206 0106 0106 0206 0102 0110  ................
-000019f0: 010c 020a 010e 010c 0208 010a 017a 1643  .............z.C
-00001a00: 6172 6443 6f6e 6e65 6374 6f72 2e5f 5f69  ardConnector.__i
-00001a10: 6e69 745f 5f63 0200 0000 0000 0000 0700  nit__c..........
-00001a20: 0000 0500 0000 4300 0000 7394 0100 0074  ......C...s....t
-00001a30: 006a 0164 0183 0101 0090 0178 7a7c 006a  .j.d.......xz|.j
-00001a40: 0290 0172 867c 0164 0219 007d 027c 006a  ...r.|.d...}.|.j
-00001a50: 0372 427c 0264 0364 0464 0574 046a 0567  .rB|.d.d.d.t.j.g
-00001a60: 046b 0772 427c 006a 067c 0183 017d 036e  .k.rB|.j.|...}.n
-00001a70: 047c 017d 037c 006a 076a 086a 097c 0383  .|.}.|.j.j.j.|..
-00001a80: 015c 037d 047d 057d 067c 0564 066b 0272  .\.}.}.}.|.d.k.r
-00001a90: 967c 0664 076b 0272 967c 006a 0372 8c7c  .|.d.k.r.|.j.r.|
-00001aa0: 0264 0364 0464 0574 046a 0567 046b 0772  .d.d.d.t.j.g.k.r
-00001ab0: 8c7c 006a 0a7c 0483 017d 047c 047c 057c  .|.j.|...}.|.|.|
-00001ac0: 0666 0353 007c 0564 086b 0272 b67c 0664  .f.S.|.d.k.r.|.d
-00001ad0: 096b 0272 b67c 006a 0b83 005c 037d 047d  .k.r.|.j...\.}.}
-00001ae0: 057d 0671 0e7c 0564 0a6b 0272 d47c 0664  .}.q.|.d.k.r.|.d
-00001af0: 056b 0272 d474 0c64 0b7c 0264 0c8d 0282  .k.r.t.d.|.d....
-00001b00: 0171 0e7c 0564 086b 0272 f27c 0664 0d6b  .q.|.d.k.r.|.d.k
-00001b10: 0272 f274 0d64 0e7c 0264 0c8d 0282 0171  .r.t.d.|.d.....q
-00001b20: 0e7c 0564 086b 0290 0172 147c 0664 0f6b  .|.d.k...r.|.d.k
-00001b30: 0290 0172 1474 0e64 107c 0264 0c8d 0282  ...r.t.d.|.d....
-00001b40: 0171 0e7c 0564 086b 0290 0172 367c 0664  .q.|.d.k...r6|.d
-00001b50: 116b 0290 0172 3674 0f64 127c 0264 0c8d  .k...r6t.d.|.d..
-00001b60: 0282 0171 0e7c 0564 086b 0290 0172 587c  ...q.|.d.k...rX|
-00001b70: 0664 136b 0290 0172 5874 1064 147c 0264  .d.k...rXt.d.|.d
-00001b80: 0c8d 0282 0171 0e7c 0564 086b 0290 0172  .....q.|.d.k...r
-00001b90: 7a7c 0664 156b 0290 0172 7a74 1164 167c  z|.d.k...rzt.d.|
-00001ba0: 0264 0c8d 0282 0171 0e7c 047c 057c 0666  .d.....q.|.|.|.f
-00001bb0: 0353 0071 0e57 0074 1264 1783 0182 0164  .S.q.W.t.d.....d
-00001bc0: 0053 0029 184e 7a10 496e 2063 6172 645f  .S.).Nz.In card_
-00001bd0: 7472 616e 736d 6974 720c 0000 0072 6400  transmitr....rd.
-00001be0: 0000 e981 0000 00e9 8200 0000 7241 0000  ............rA..
-00001bf0: 0072 0100 0000 7242 0000 00e9 0600 0000  .r....rB........
-00001c00: e96a 0000 007a 1043 6172 6453 656c 6563  .j...z.CardSelec
-00001c10: 7420 6572 726f 7229 01da 0369 6e73 e910  t error)...ins..
-00001c20: 0000 007a 1f41 5044 5520 6572 726f 723a  ...z.APDU error:
-00001c30: 2077 726f 6e67 2050 3120 7061 7261 6d65   wrong P1 parame
-00001c40: 7465 7273 e951 0000 007a 2553 6174 6f64  ters.Q...z%Satod
-00001c50: 696d 6520 6572 726f 723a 2069 6e63 6f72  ime error: incor
-00001c60: 7265 6374 2075 6e6c 6f63 6b20 636f 6465  rect unlock code
-00001c70: e952 0000 007a 2753 6174 6f64 696d 6520  .R...z'Satodime 
-00001c80: 6572 726f 723a 2069 6e63 6f72 7265 6374  error: incorrect
-00001c90: 206b 6579 736c 6f74 2073 7461 7465 7265   keyslot statere
-00001ca0: 0000 007a 2853 6174 6f64 696d 6520 6572  ...z(Satodime er
-00001cb0: 726f 723a 2069 6e63 6f72 7265 6374 2070  ror: incorrect p
-00001cc0: 726f 746f 636f 6c20 6d65 6469 61e9 5400  rotocol media.T.
-00001cd0: 0000 7a26 5361 746f 6469 6d65 2065 7272  ..z&Satodime err
-00001ce0: 6f72 3a20 756e 6b6e 6f77 6e20 7072 6f74  or: unknown prot
-00001cf0: 6f63 6f6c 206d 6564 6961 7a22 4e6f 2063  ocol mediaz"No c
-00001d00: 6172 6420 666f 756e 6421 2050 6c65 6173  ard found! Pleas
-00001d10: 6520 696e 7365 7274 2063 6172 6421 2913  e insert card!).
-00001d20: 7227 0000 0072 3400 0000 7246 0000 0072  r'...r4...rF...r
-00001d30: 5800 0000 722b 0000 00da 0e49 4e53 5f47  X...r+.....INS_G
-00001d40: 4554 5f53 5441 5455 53da 1b63 6172 645f  ET_STATUS..card_
-00001d50: 656e 6372 7970 745f 7365 6375 7265 5f63  encrypt_secure_c
-00001d60: 6861 6e6e 656c 7247 0000 0072 4800 0000  hannelrG...rH...
-00001d70: da08 7472 616e 736d 6974 da1b 6361 7264  ..transmit..card
-00001d80: 5f64 6563 7279 7074 5f73 6563 7572 655f  _decrypt_secure_
-00001d90: 6368 616e 6e65 6cda 0f63 6172 645f 7665  channel..card_ve
-00001da0: 7269 6679 5f50 494e da0f 4361 7264 5365  rify_PIN..CardSe
-00001db0: 6c65 6374 4572 726f 72da 1049 6e63 6f72  lectError..Incor
-00001dc0: 7265 6374 5031 4572 726f 72da 1849 6e63  rectP1Error..Inc
-00001dd0: 6f72 7265 6374 556e 6c6f 636b 436f 6465  orrectUnlockCode
-00001de0: 4572 726f 72da 1a49 6e63 6f72 7265 6374  Error..Incorrect
-00001df0: 4b65 7973 6c6f 7453 7461 7465 4572 726f  KeyslotStateErro
-00001e00: 72da 1b49 6e63 6f72 7265 6374 5072 6f74  r..IncorrectProt
-00001e10: 6f63 6f6c 4d65 6469 6145 7272 6f72 da19  ocolMediaError..
-00001e20: 556e 6b6e 6f77 6e50 726f 746f 636f 6c4d  UnknownProtocolM
-00001e30: 6564 6961 4572 726f 72da 1343 6172 644e  ediaError..CardN
-00001e40: 6f74 5072 6573 656e 7445 7272 6f72 2907  otPresentError).
-00001e50: 7236 0000 005a 0a70 6c61 696e 5f61 7064  r6...Z.plain_apd
-00001e60: 7572 8700 0000 da04 6170 6475 7222 0000  ur......apdur"..
-00001e70: 0072 5d00 0000 725e 0000 0072 3700 0000  .r]...r^...r7...
-00001e80: 7237 0000 0072 3800 0000 da0d 6361 7264  r7...r8.....card
-00001e90: 5f74 7261 6e73 6d69 74cc 0000 0073 3600  _transmit....s6.
-00001ea0: 0000 0001 0a01 0c03 0801 1801 0c02 0403  ................
-00001eb0: 1403 1001 1801 0a01 0a02 1001 1001 1001  ................
-00001ec0: 0e03 1001 0e01 1401 0e01 1401 0e01 1401  ................
-00001ed0: 0e01 1401 0e04 0e03 7a1b 4361 7264 436f  ........z.CardCo
-00001ee0: 6e6e 6563 746f 722e 6361 7264 5f74 7261  nnector.card_tra
-00001ef0: 6e73 6d69 7463 0100 0000 0000 0000 0100  nsmitc..........
-00001f00: 0000 0200 0000 4300 0000 7316 0000 0074  ......C...s....t
-00001f10: 006a 0164 0183 0101 007c 006a 026a 036a  .j.d.....|.j.j.j
-00001f20: 0483 0053 0029 024e 7a11 496e 2063 6172  ...S.).Nz.In car
-00001f30: 645f 6765 745f 4154 5228 2929 0572 2700  d_get_ATR()).r'.
-00001f40: 0000 7234 0000 0072 4700 0000 7248 0000  ..r4...rG...rH..
-00001f50: 005a 0667 6574 4154 5229 0172 3600 0000  .Z.getATR).r6...
-00001f60: 7237 0000 0072 3700 0000 7238 0000 00da  r7...r7...r8....
-00001f70: 0c63 6172 645f 6765 745f 4154 52f8 0000  .card_get_ATR...
-00001f80: 0073 0400 0000 0001 0a01 7a1a 4361 7264  .s........z.Card
-00001f90: 436f 6e6e 6563 746f 722e 6361 7264 5f67  Connector.card_g
-00001fa0: 6574 5f41 5452 6301 0000 0000 0000 0009  et_ATRc.........
-00001fb0: 0000 0004 0000 0043 0000 0073 4400 0000  .......C...sD...
-00001fc0: 7400 6a01 6401 8301 0100 6402 7d01 6403  t.j.d.....d.}.d.
-00001fd0: 7d02 6404 7d03 6405 7d04 7c01 7c02 7c03  }.d.}.d.}.|.|.|.
-00001fe0: 7c04 6704 7d05 7c00 6a02 6a03 6a04 7c05  |.g.}.|.j.j.j.|.
-00001ff0: 8301 5c03 7d06 7d07 7d08 7c06 7c07 7c08  ..\.}.}.}.|.|.|.
-00002000: 6603 5300 2906 4e7a 1049 6e20 6361 7264  f.S.).Nz.In card
-00002010: 5f67 6574 5f43 504c 43e9 8000 0000 e9ca  _get_CPLC.......
-00002020: 0000 00e9 9f00 0000 e97f 0000 0029 0572  .............).r
-00002030: 2700 0000 7234 0000 0072 4700 0000 7248  '...r4...rG...rH
-00002040: 0000 0072 8e00 0000 2909 7236 0000 00da  ...r....).r6....
-00002050: 0363 6c61 7287 0000 00da 0270 31da 0270  .clar......p1..p
-00002060: 3272 9800 0000 7222 0000 0072 5d00 0000  2r....r"...r]...
-00002070: 725e 0000 0072 3700 0000 7237 0000 0072  r^...r7...r7...r
-00002080: 3800 0000 724a 0000 00fc 0000 0073 1000  8...rJ.......s..
-00002090: 0000 0001 0a01 0401 0401 0401 0401 0c02  ................
-000020a0: 1401 7a1b 4361 7264 436f 6e6e 6563 746f  ..z.CardConnecto
-000020b0: 722e 6361 7264 5f67 6574 5f43 504c 4363  r.card_get_CPLCc
-000020c0: 0100 0000 0000 0000 0900 0000 0400 0000  ................
-000020d0: 4300 0000 7344 0000 0074 006a 0164 0183  C...sD...t.j.d..
-000020e0: 0101 0064 027d 0164 037d 0264 047d 0364  ...d.}.d.}.d.}.d
-000020f0: 057d 047c 017c 027c 037c 0467 047d 057c  .}.|.|.|.|.g.}.|
-00002100: 006a 026a 036a 047c 0583 015c 037d 067d  .j.j.j.|...\.}.}
-00002110: 077d 087c 067c 077c 0866 0353 0029 064e  .}.|.|.|.f.S.).N
-00002120: 7a0f 496e 2063 6172 645f 6765 745f 4949  z.In card_get_II
-00002130: 4e72 9b00 0000 729c 0000 0072 0100 0000  Nr....r....r....
-00002140: e942 0000 0029 0572 2700 0000 7234 0000  .B...).r'...r4..
-00002150: 0072 4700 0000 7248 0000 0072 8e00 0000  .rG...rH...r....
-00002160: 2909 7236 0000 0072 9f00 0000 7287 0000  ).r6...r....r...
-00002170: 0072 a000 0000 72a1 0000 0072 9800 0000  .r....r....r....
-00002180: 7222 0000 0072 5d00 0000 725e 0000 0072  r"...r]...r^...r
-00002190: 3700 0000 7237 0000 0072 3800 0000 724d  7...r7...r8...rM
-000021a0: 0000 0007 0100 0073 1000 0000 0001 0a01  .......s........
-000021b0: 0401 0401 0401 0401 0c02 1401 7a1a 4361  ............z.Ca
-000021c0: 7264 436f 6e6e 6563 746f 722e 6361 7264  rdConnector.card
-000021d0: 5f67 6574 5f49 494e 6301 0000 0000 0000  _get_IINc.......
-000021e0: 0009 0000 0004 0000 0043 0000 0073 4400  .........C...sD.
-000021f0: 0000 7400 6a01 6401 8301 0100 6402 7d01  ..t.j.d.....d.}.
-00002200: 6403 7d02 6404 7d03 6405 7d04 7c01 7c02  d.}.d.}.d.}.|.|.
-00002210: 7c03 7c04 6704 7d05 7c00 6a02 6a03 6a04  |.|.g.}.|.j.j.j.
-00002220: 7c05 8301 5c03 7d06 7d07 7d08 7c06 7c07  |...\.}.}.}.|.|.
-00002230: 7c08 6603 5300 2906 4e7a 0f49 6e20 6361  |.f.S.).Nz.In ca
-00002240: 7264 5f67 6574 5f43 494e 729b 0000 0072  rd_get_CINr....r
-00002250: 9c00 0000 7201 0000 00e9 4500 0000 2905  ....r.....E...).
-00002260: 7227 0000 0072 3400 0000 7247 0000 0072  r'...r4...rG...r
-00002270: 4800 0000 728e 0000 0029 0972 3600 0000  H...r....).r6...
-00002280: 729f 0000 0072 8700 0000 72a0 0000 0072  r....r....r....r
-00002290: a100 0000 7298 0000 0072 2200 0000 725d  ....r....r"...r]
-000022a0: 0000 0072 5e00 0000 7237 0000 0072 3700  ...r^...r7...r7.
-000022b0: 0000 7238 0000 0072 4e00 0000 1201 0000  ..r8...rN.......
-000022c0: 7310 0000 0000 010a 0104 0104 0104 0104  s...............
-000022d0: 010c 0214 017a 1a43 6172 6443 6f6e 6e65  .....z.CardConne
-000022e0: 6374 6f72 2e63 6172 645f 6765 745f 4349  ctor.card_get_CI
-000022f0: 4e63 0100 0000 0000 0000 0100 0000 0300  Nc..............
-00002300: 0000 4300 0000 7386 0000 0074 006a 0164  ..C...s....t.j.d
-00002310: 0183 0101 0064 007c 005f 0264 007c 005f  .....d.|._.d.|._
-00002320: 0364 007c 005f 0464 007c 005f 0564 007c  .d.|._.d.|._.d.|
-00002330: 005f 0664 007c 005f 0764 027c 005f 0864  ._.d.|._.d.|._.d
-00002340: 007c 005f 097c 006a 0a72 527c 006a 0a6a  .|._.|.j.rR|.j.j
-00002350: 0b6a 0c83 0001 0064 007c 005f 0a7c 006a  .j.....d.|._.|.j
-00002360: 0d64 006b 0972 6a7c 006a 0d6a 0e64 0364  .d.k.rj|.j.j.d.d
-00002370: 0283 0201 0064 007c 006a 0f5f 1064 007c  .....d.|.j._.d.|
-00002380: 006a 0f5f 1164 007c 006a 0f5f 1264 0053  .j._.d.|.j._.d.S
-00002390: 0029 044e 7a14 496e 2063 6172 645f 6469  .).Nz.In card_di
-000023a0: 7363 6f6e 6e65 6374 2829 4672 4400 0000  sconnect()FrD...
-000023b0: 2913 7227 0000 0072 3400 0000 727c 0000  ).r'...r4...r|..
-000023c0: 0072 7b00 0000 7278 0000 0072 7700 0000  .r{...rx...rw...
-000023d0: 7279 0000 0072 5800 0000 7246 0000 0072  ry...rX...rF...r
-000023e0: 8100 0000 7247 0000 0072 4800 0000 7220  ....rG...rH...r 
-000023f0: 0000 0072 5a00 0000 725b 0000 0072 7600  ...rZ...r[...rv.
-00002400: 0000 da0b 6175 7468 656e 7469 6b65 795a  ....authentikeyZ
-00002410: 1261 7574 6865 6e74 696b 6579 5f63 6f6f  .authentikey_coo
-00002420: 7264 785a 1861 7574 6865 6e74 696b 6579  rdxZ.authentikey
-00002430: 5f66 726f 6d5f 7374 6f72 6167 6529 0172  _from_storage).r
-00002440: 3600 0000 7237 0000 0072 3700 0000 7238  6...r7...r7...r8
-00002450: 0000 0072 5600 0000 1d01 0000 7322 0000  ...rV.......s"..
-00002460: 0000 010a 0106 0106 0106 0106 0106 0106  ................
-00002470: 0106 0106 0106 010c 0106 010a 010e 0208  ................
-00002480: 0108 017a 1d43 6172 6443 6f6e 6e65 6374  ...z.CardConnect
-00002490: 6f72 2e63 6172 645f 6469 7363 6f6e 6e65  or.card_disconne
-000024a0: 6374 6303 0000 0000 0000 0003 0000 0002  ctc.............
-000024b0: 0000 0043 0000 0073 0c00 0000 6401 7c01  ...C...s....d.|.
-000024c0: 1400 7c02 1700 5300 2902 4e72 8800 0000  ..|...S.).Nr....
-000024d0: 7237 0000 0029 0372 3600 0000 725d 0000  r7...).r6...r]..
-000024e0: 0072 5e00 0000 7237 0000 0072 3700 0000  .r^...r7...r7...
-000024f0: 7238 0000 00da 0867 6574 5f73 7731 3232  r8.....get_sw122
-00002500: 0100 0073 0200 0000 0001 7a16 4361 7264  ...s......z.Card
-00002510: 436f 6e6e 6563 746f 722e 6765 745f 7377  Connector.get_sw
-00002520: 3132 6301 0000 0000 0000 0003 0000 0011  12c.............
-00002530: 0000 0043 0000 0073 b000 0000 7400 6a01  ...C...s....t.j.
-00002540: 6401 8301 0100 7c00 6a02 6400 6b02 7222  d.....|.j.d.k.r"
-00002550: 6402 6403 6404 6703 7c00 5f02 6e16 7403  d.d.d.g.|._.n.t.
-00002560: 7c00 6a02 7404 8302 7238 7c00 6a02 6701  |.j.t...r8|.j.g.
-00002570: 7c00 5f02 7866 7c00 6a02 4400 5d5c 7d01  |._.xf|.j.D.]\}.
-00002580: 7934 7c01 6402 6b02 7256 7c00 6a05 8300  y4|.d.k.rV|.j...
-00002590: 5300 7c01 6403 6b02 7266 7c00 6a06 8300  S.|.d.k.rf|.j...
-000025a0: 5300 7c01 6404 6b02 7276 7c00 6a07 8300  S.|.d.k.rv|.j...
-000025b0: 5300 5700 7140 0400 7408 6b0a 729a 0100  S.W.q@..t.k.r...
-000025c0: 7d02 0100 7a06 5700 5900 6400 6400 7d02  }...z.W.Y.d.d.}.
-000025d0: 7e02 5800 7140 5800 7140 5700 7408 6405  ~.X.q@X.q@W.t.d.
-000025e0: 6406 6407 8d02 8201 6400 5300 2908 4e7a  d.d.....d.S.).Nz
-000025f0: 0e49 6e20 6361 7264 5f73 656c 6563 745a  .In card_selectZ
-00002600: 0873 6174 6f63 6869 705a 0a73 6565 646b  .satochipZ.seedk
-00002610: 6565 7065 72da 0873 6174 6f64 696d 657a  eeper..satodimez
-00002620: 1043 6172 6453 656c 6563 7420 6572 726f  .CardSelect erro
-00002630: 7272 6400 0000 2901 7287 0000 0029 0972  rrd...).r....).r
-00002640: 2700 0000 7234 0000 0072 5c00 0000 da0a  '...r4...r\.....
-00002650: 6973 696e 7374 616e 6365 7275 0000 00da  isinstanceru....
-00002660: 1463 6172 645f 7365 6c65 6374 5f73 6174  .card_select_sat
-00002670: 6f63 6869 70da 1663 6172 645f 7365 6c65  ochip..card_sele
-00002680: 6374 5f73 6565 646b 6565 7065 72da 1463  ct_seedkeeper..c
-00002690: 6172 645f 7365 6c65 6374 5f73 6174 6f64  ard_select_satod
-000026a0: 696d 6572 9100 0000 2903 7236 0000 005a  imer....).r6...Z
-000026b0: 0b63 6172 645f 6170 706c 6574 da02 6578  .card_applet..ex
-000026c0: 7237 0000 0072 3700 0000 7238 0000 0072  r7...r7...r8...r
-000026d0: 5500 0000 3501 0000 7320 0000 0000 010a  U...5...s ......
-000026e0: 030a 010e 010c 010a 030c 0102 0108 0108  ................
-000026f0: 0108 0108 0108 010c 0110 0116 037a 1943  .............z.C
-00002700: 6172 6443 6f6e 6e65 6374 6f72 2e63 6172  ardConnector.car
-00002710: 645f 7365 6c65 6374 6301 0000 0000 0000  d_selectc.......
-00002720: 0005 0000 0003 0000 0043 0000 0073 4200  .........C...sB.
-00002730: 0000 7400 6a01 7402 7400 6a03 8301 6701  ..t.j.t.t.j...g.
-00002740: 1700 7400 6a03 1700 7d01 7c00 6a04 7c01  ..t.j...}.|.j.|.
-00002750: 8301 5c03 7d02 7d03 7d04 6401 7c00 5f05  ..\.}.}.}.d.|._.
-00002760: 7406 6a07 6402 8301 0100 7c02 7c03 7c04  t.j.d.....|.|.|.
-00002770: 6603 5300 2903 4e5a 0853 6174 6f63 6869  f.S.).NZ.Satochi
-00002780: 707a 1146 6f75 6e64 2061 2053 6174 6f63  pz.Found a Satoc
-00002790: 6869 7021 2908 7263 0000 00da 0653 454c  hip!).rc.....SEL
-000027a0: 4543 5472 3500 0000 da0c 5341 544f 4348  ECTr5.....SATOCH
-000027b0: 4950 5f41 4944 7299 0000 0072 8100 0000  IP_AIDr....r....
-000027c0: 7227 0000 0072 3400 0000 2905 7236 0000  r'...r4...).r6..
-000027d0: 0072 9800 0000 7222 0000 0072 5d00 0000  .r....r"...r]...
-000027e0: 725e 0000 0072 3700 0000 7237 0000 0072  r^...r7...r7...r
-000027f0: 3800 0000 72a8 0000 004d 0100 0073 0a00  8...r....M...s..
-00002800: 0000 0001 1801 1001 0601 0a01 7a22 4361  ............z"Ca
-00002810: 7264 436f 6e6e 6563 746f 722e 6361 7264  rdConnector.card
-00002820: 5f73 656c 6563 745f 7361 746f 6368 6970  _select_satochip
-00002830: 6301 0000 0000 0000 0005 0000 0003 0000  c...............
-00002840: 0043 0000 0073 4200 0000 7400 6a01 7402  .C...sB...t.j.t.
-00002850: 7400 6a03 8301 6701 1700 7400 6a03 1700  t.j...g...t.j...
-00002860: 7d01 7c00 6a04 7c01 8301 5c03 7d02 7d03  }.|.j.|...\.}.}.
-00002870: 7d04 6401 7c00 5f05 7406 6a07 6402 8301  }.d.|._.t.j.d...
-00002880: 0100 7c02 7c03 7c04 6603 5300 2903 4e5a  ..|.|.|.f.S.).NZ
-00002890: 0a53 6565 644b 6565 7065 727a 1346 6f75  .SeedKeeperz.Fou
-000028a0: 6e64 2061 2053 6565 644b 6565 7065 7221  nd a SeedKeeper!
-000028b0: 2908 7263 0000 0072 ac00 0000 7235 0000  ).rc...r....r5..
-000028c0: 00da 0e53 4545 444b 4545 5045 525f 4149  ...SEEDKEEPER_AI
-000028d0: 4472 9900 0000 7281 0000 0072 2700 0000  Dr....r....r'...
-000028e0: 7234 0000 0029 0572 3600 0000 7298 0000  r4...).r6...r...
-000028f0: 0072 2200 0000 725d 0000 0072 5e00 0000  .r"...r]...r^...
-00002900: 7237 0000 0072 3700 0000 7238 0000 0072  r7...r7...r8...r
-00002910: a900 0000 5401 0000 730a 0000 0000 0118  ....T...s.......
-00002920: 0110 0106 010a 017a 2443 6172 6443 6f6e  .......z$CardCon
-00002930: 6e65 6374 6f72 2e63 6172 645f 7365 6c65  nector.card_sele
-00002940: 6374 5f73 6565 646b 6565 7065 7263 0100  ct_seedkeeperc..
-00002950: 0000 0000 0000 0500 0000 0300 0000 4300  ..............C.
-00002960: 0000 7342 0000 0074 006a 0174 0274 006a  ..sB...t.j.t.t.j
-00002970: 0383 0167 0117 0074 006a 0317 007d 017c  ...g...t.j...}.|
-00002980: 006a 047c 0183 015c 037d 027d 037d 0464  .j.|...\.}.}.}.d
-00002990: 017c 005f 0574 066a 0764 0283 0101 007c  .|._.t.j.d.....|
-000029a0: 027c 037c 0466 0353 0029 034e da08 5361  .|.|.f.S.).N..Sa
-000029b0: 746f 6469 6d65 7a11 466f 756e 6420 6120  todimez.Found a 
-000029c0: 5361 746f 6469 6d65 2129 0872 6300 0000  Satodime!).rc...
-000029d0: 72ac 0000 0072 3500 0000 da0c 5341 544f  r....r5.....SATO
-000029e0: 4449 4d45 5f41 4944 7299 0000 0072 8100  DIME_AIDr....r..
-000029f0: 0000 7227 0000 0072 3400 0000 2905 7236  ..r'...r4...).r6
-00002a00: 0000 0072 9800 0000 7222 0000 0072 5d00  ...r....r"...r].
-00002a10: 0000 725e 0000 0072 3700 0000 7237 0000  ..r^...r7...r7..
-00002a20: 0072 3800 0000 72aa 0000 005b 0100 0073  .r8...r....[...s
-00002a30: 0a00 0000 0001 1801 1001 0601 0a01 7a22  ..............z"
-00002a40: 4361 7264 436f 6e6e 6563 746f 722e 6361  CardConnector.ca
-00002a50: 7264 5f73 656c 6563 745f 7361 746f 6469  rd_select_satodi
-00002a60: 6d65 6301 0000 0000 0000 000a 0000 0005  mec.............
-00002a70: 0000 0043 0000 0073 2602 0000 7400 6a01  ...C...s&...t.j.
-00002a80: 6401 8301 0100 7402 6a03 7d01 7402 6a04  d.....t.j.}.t.j.
-00002a90: 7d02 6402 7d03 6402 7d04 7c01 7c02 7c03  }.d.}.d.}.|.|.|.
-00002aa0: 7c04 6704 7d05 7c00 6a05 7c05 8301 5c03  |.g.}.|.j.|...\.
-00002ab0: 7d06 7d07 7d08 6900 7d09 7c07 6403 6b02  }.}.}.i.}.|.d.k.
-00002ac0: 6f4c 7c08 6402 6b02 9001 72bc 7c06 6402  oL|.d.k...r.|.d.
-00002ad0: 1900 7c09 6404 3c00 7c06 6405 1900 7c09  ..|.d.<.|.d...|.
-00002ae0: 6406 3c00 7c06 6407 1900 7c09 6408 3c00  d.<.|.d...|.d.<.
-00002af0: 7c06 6409 1900 7c09 640a 3c00 7c09 6404  |.d...|.d.<.|.d.
-00002b00: 1900 640b 3e00 7c09 6406 1900 1700 7c09  ..d.>.|.d.....|.
-00002b10: 640c 3c00 7406 7c06 8301 640b 6b05 72e2  d.<.t.|...d.k.r.
-00002b20: 7c06 640d 1900 7c09 640e 3c00 7c06 640f  |.d...|.d.<.|.d.
-00002b30: 1900 7c09 6410 3c00 7c06 6411 1900 7c09  ..|.d.<.|.d...|.
-00002b40: 6412 3c00 7c06 6413 1900 7c09 6414 3c00  d.<.|.d...|.d.<.
-00002b50: 6415 0400 7c00 5f07 7c09 6416 3c00 7406  d...|._.|.d.<.t.
-00002b60: 7c06 8301 6417 6b05 9001 7210 7c06 640b  |...d.k...r.|.d.
-00002b70: 1900 6402 6b02 9001 7202 6415 6e02 6418  ..d.k...r.d.n.d.
-00002b80: 0400 7c00 5f07 7c09 6416 3c00 7406 7c06  ..|._.|.d.<.t.|.
-00002b90: 8301 6419 6b05 9001 723e 7c06 6417 1900  ..d.k...r>|.d...
-00002ba0: 6402 6b02 9001 7230 6415 6e02 6418 0400  d.k...r0d.n.d...
-00002bb0: 7c00 5f08 7c09 641a 3c00 7406 7c06 8301  |._.|.d.<.t.|...
-00002bc0: 641b 6b05 9001 726e 7c06 6419 1900 6402  d.k...rn|.d...d.
-00002bd0: 6b02 9001 725e 6415 6e02 6418 0400 7c00  k...r^d.n.d...|.
-00002be0: 5f09 7c09 641c 3c00 6e0e 6418 0400 7c00  _.|.d.<.n.d...|.
-00002bf0: 5f09 7c09 641c 3c00 7406 7c06 8301 641d  _.|.d.<.t.|...d.
-00002c00: 6b05 9001 72ac 7c06 641b 1900 6402 6b02  k...r.|.d...d.k.
-00002c10: 9001 729c 6415 6e02 6418 0400 7c00 5f0a  ..r.d.n.d...|._.
-00002c20: 7c09 641e 3c00 6e0e 6415 0400 7c00 5f0a  |.d.<.n.d...|._.
-00002c30: 7c09 641e 3c00 6e5e 7c07 641f 6b02 9001  |.d.<.n^|.d.k...
-00002c40: 72fc 7c08 640d 6b02 9001 72fc 6415 0400  r.|.d.k...r.d...
-00002c50: 7c00 5f09 7c09 641c 3c00 6415 0400 7c00  |._.|.d.<.d...|.
-00002c60: 5f08 7c09 641a 3c00 6415 0400 7c00 5f0a  _.|.d.<.d...|._.
-00002c70: 7c09 641e 3c00 6e1e 7400 6a0b 6420 740c  |.d.<.n.t.j.d t.
-00002c80: 6421 7c07 1400 7c08 1700 8301 9b00 6422  d!|...|.......d"
-00002c90: 9d03 8301 0100 7c06 7c07 7c08 7c09 6604  ......|.|.|.|.f.
-00002ca0: 5300 2923 4e7a 1249 6e20 6361 7264 5f67  S.)#Nz.In card_g
-00002cb0: 6574 5f73 7461 7475 7372 0100 0000 7241  et_statusr....rA
-00002cc0: 0000 005a 1670 726f 746f 636f 6c5f 6d61  ...Z.protocol_ma
-00002cd0: 6a6f 725f 7665 7273 696f 6e72 0c00 0000  jor_versionr....
-00002ce0: 5a16 7072 6f74 6f63 6f6c 5f6d 696e 6f72  Z.protocol_minor
-00002cf0: 5f76 6572 7369 6f6e 7223 0000 005a 1461  _versionr#...Z.a
-00002d00: 7070 6c65 745f 6d61 6a6f 725f 7665 7273  pplet_major_vers
-00002d10: 696f 6ee9 0300 0000 5a14 6170 706c 6574  ion.....Z.applet
-00002d20: 5f6d 696e 6f72 5f76 6572 7369 6f6e e908  _minor_version..
-00002d30: 0000 005a 1070 726f 746f 636f 6c5f 7665  ...Z.protocol_ve
-00002d40: 7273 696f 6e72 4300 0000 da14 5049 4e30  rsionrC.....PIN0
-00002d50: 5f72 656d 6169 6e69 6e67 5f74 7269 6573  _remaining_tries
-00002d60: 7221 0000 00da 1450 554b 305f 7265 6d61  r!.....PUK0_rema
-00002d70: 696e 696e 675f 7472 6965 7372 8500 0000  ining_triesr....
-00002d80: 5a14 5049 4e31 5f72 656d 6169 6e69 6e67  Z.PIN1_remaining
-00002d90: 5f74 7269 6573 e907 0000 005a 1450 554b  _tries.....Z.PUK
-00002da0: 315f 7265 6d61 696e 696e 675f 7472 6965  1_remaining_trie
-00002db0: 7346 5a08 6e65 6564 7332 4641 e909 0000  sFZ.needs2FA....
-00002dc0: 0054 e90a 0000 0072 7800 0000 e90b 0000  .T.....rx.......
-00002dd0: 0072 7900 0000 e90c 0000 0072 5800 0000  .ry........rX...
-00002de0: 7242 0000 007a 2a55 6e6b 6e6f 776e 2065  rB...z*Unknown e
-00002df0: 7272 6f72 2069 6e20 6765 745f 7374 6174  rror in get_stat
-00002e00: 7573 2829 2028 6572 726f 7220 636f 6465  us() (error code
-00002e10: 20e9 0001 0000 fa01 2929 0d72 2700 0000   .......)).r'...
-00002e20: 7234 0000 0072 2b00 0000 da0c 4361 7264  r4...r+.....Card
-00002e30: 4564 6765 5f43 4c41 728c 0000 0072 9900  Edge_CLAr....r..
-00002e40: 0000 7235 0000 0072 7700 0000 7278 0000  ..r5...rw...rx..
-00002e50: 0072 7900 0000 7258 0000 0072 5400 0000  .ry...rX...rT...
-00002e60: 724c 0000 0029 0a72 3600 0000 729f 0000  rL...).r6...r...
-00002e70: 0072 8700 0000 72a0 0000 0072 a100 0000  .r....r....r....
-00002e80: 7298 0000 0072 2200 0000 725d 0000 0072  r....r"...r]...r
-00002e90: 5e00 0000 da01 6472 3700 0000 7237 0000  ^.....dr7...r7..
-00002ea0: 0072 3800 0000 7257 0000 0062 0100 0073  .r8...rW...b...s
-00002eb0: 4800 0000 0001 0a01 0601 0601 0401 0401  H...............
-00002ec0: 0c01 1001 0401 1201 0c01 0c01 0c01 0c01  ................
-00002ed0: 1801 0c01 0c01 0c01 0c01 0c01 0e01 0e01  ................
-00002ee0: 2001 0e01 2001 0e01 2202 0e01 0e01 2202   ... ...".....".
-00002ef0: 1002 1401 0e01 0e01 1003 1e03 7a1d 4361  ............z.Ca
-00002f00: 7264 436f 6e6e 6563 746f 722e 6361 7264  rdConnector.card
-00002f10: 5f67 6574 5f73 7461 7475 7363 0100 0000  _get_statusc....
-00002f20: 0000 0000 0c00 0000 1200 0000 4300 0000  ............C...
-00002f30: 73ea 0000 0074 006a 0164 0183 0101 0074  s....t.j.d.....t
-00002f40: 026a 037d 0164 027d 0264 037d 0364 047d  .j.}.d.}.d.}.d.}
-00002f50: 047c 017c 027c 037c 0467 047d 057c 006a  .|.|.|.|.g.}.|.j
-00002f60: 047c 0583 015c 037d 067d 077d 087c 0764  .|...\.}.}.}.|.d
-00002f70: 056b 0272 ae7c 0864 036b 0272 ae7c 0664  .k.r.|.d.k.r.|.d
-00002f80: 0319 007d 0979 1a74 057c 0664 0464 0085  ...}.y.t.|.d.d..
-00002f90: 0219 0083 016a 0664 0683 017d 0a57 0071  .....j.d...}.W.q
-00002fa0: de04 0074 076b 0a72 aa01 007d 0b01 007a  ...t.k.r...}...z
-00002fb0: 2474 006a 0864 0783 0101 0074 0974 057c  $t.j.d.....t.t.|
-00002fc0: 0664 0464 0085 0219 0083 0183 017d 0a57  .d.d.........}.W
-00002fd0: 0059 0064 0064 007d 0b7e 0b58 0071 de58  .Y.d.d.}.~.X.q.X
-00002fe0: 006e 307c 0764 086b 0272 c47c 0864 036b  .n0|.d.k.r.|.d.k
-00002ff0: 0272 c464 097d 0a6e 1a74 006a 0864 0a7c  .r.d.}.n.t.j.d.|
-00003000: 079b 0064 0b7c 089b 009d 0483 0101 0064  ...d.|.........d
-00003010: 0c7d 0a7c 067c 077c 087c 0a66 0453 0029  .}.|.|.|.|.f.S.)
-00003020: 0d4e 7a11 496e 2063 6172 645f 6765 745f  .Nz.In card_get_
-00003030: 6c61 6265 6ce9 3d00 0000 7201 0000 0072  label.=...r....r
-00003040: 0c00 0000 7241 0000 00da 0475 7466 387a  ....rA.....utf8z
-00003050: 2e55 6e69 636f 6465 4465 636f 6465 4572  .UnicodeDecodeEr
-00003060: 726f 7220 7768 696c 6520 6465 636f 6469  ror while decodi
-00003070: 6e67 2063 6172 6420 6c61 6265 6c20 2172  ng card label !r
-00003080: 7200 0000 7a06 286e 6f6e 6529 7a23 4572  r...z.(none)z#Er
-00003090: 726f 7220 7768 696c 6520 7265 636f 7665  ror while recove
-000030a0: 7269 6e67 2063 6172 6420 6c61 6265 6c3a  ring card label:
-000030b0: 2072 2400 0000 7a09 2875 6e6b 6e6f 776e   r$...z.(unknown
-000030c0: 2929 0a72 2700 0000 7234 0000 0072 2b00  )).r'...r4...r+.
-000030d0: 0000 72bc 0000 0072 9900 0000 724b 0000  ..r....r....rK..
-000030e0: 00da 0664 6563 6f64 65da 1255 6e69 636f  ...decode..Unico
-000030f0: 6465 4465 636f 6465 4572 726f 7272 5400  deDecodeErrorrT.
-00003100: 0000 7275 0000 0029 0c72 3600 0000 729f  ..ru...).r6...r.
-00003110: 0000 0072 8700 0000 72a0 0000 0072 a100  ...r....r....r..
-00003120: 0000 7298 0000 0072 2200 0000 725d 0000  ..r....r"...r]..
-00003130: 0072 5e00 0000 da0a 6c61 6265 6c5f 7369  .r^.....label_si
-00003140: 7a65 da05 6c61 6265 6cda 0165 7237 0000  ze..label..er7..
-00003150: 0072 3700 0000 7238 0000 00da 0e63 6172  .r7...r8.....car
-00003160: 645f 6765 745f 6c61 6265 6c93 0100 0073  d_get_label....s
-00003170: 2600 0000 0002 0a01 0601 0401 0401 0401  &...............
-00003180: 0c01 1002 1001 0801 0201 1a01 1001 0a01  ................
-00003190: 2801 1001 0602 1601 0402 7a1c 4361 7264  (.........z.Card
-000031a0: 436f 6e6e 6563 746f 722e 6361 7264 5f67  Connector.card_g
-000031b0: 6574 5f6c 6162 656c 6302 0000 0000 0000  et_labelc.......
-000031c0: 000d 0000 0005 0000 0043 0000 0073 6c00  .........C...sl.
-000031d0: 0000 7400 6a01 6401 8301 0100 7402 6a03  ..t.j.d.....t.j.
-000031e0: 7d02 6402 7d03 6403 7d04 6403 7d05 7404  }.d.}.d.}.d.}.t.
-000031f0: 7c01 6a05 6404 8301 8301 7d06 7406 7c06  |.j.d.....}.t.|.
-00003200: 8301 6701 7c06 1700 7d07 7406 7c07 8301  ..g.|...}.t.|...
-00003210: 7d08 7c02 7c03 7c04 7c05 7c08 6705 7c07  }.|.|.|.|.|.g.|.
-00003220: 1700 7d09 7c00 6a07 7c09 8301 5c03 7d0a  ..}.|.j.|...\.}.
-00003230: 7d0b 7d0c 7c0a 7c0b 7c0c 6603 5300 2905  }.}.|.|.|.f.S.).
-00003240: 4e7a 1149 6e20 6361 7264 5f73 6574 5f6c  Nz.In card_set_l
-00003250: 6162 656c 72be 0000 0072 0100 0000 72bf  abelr....r....r.
-00003260: 0000 0029 0872 2700 0000 7234 0000 0072  ...).r'...r4...r
-00003270: 2b00 0000 72bc 0000 00da 046c 6973 74da  +...r......list.
-00003280: 0665 6e63 6f64 6572 3500 0000 7299 0000  .encoder5...r...
-00003290: 0029 0d72 3600 0000 72c3 0000 0072 9f00  .).r6...r....r..
-000032a0: 0000 7287 0000 0072 a000 0000 72a1 0000  ..r....r....r...
-000032b0: 00da 0a6c 6162 656c 5f6c 6973 74da 0464  ...label_list..d
-000032c0: 6174 61da 026c 6372 9800 0000 7222 0000  ata..lcr....r"..
-000032d0: 0072 5d00 0000 725e 0000 0072 3700 0000  .r]...r^...r7...
-000032e0: 7237 0000 0072 3800 0000 da0e 6361 7264  r7...r8.....card
-000032f0: 5f73 6574 5f6c 6162 656c ac01 0000 7316  _set_label....s.
-00003300: 0000 0000 010a 0106 0104 0104 0104 020e  ................
-00003310: 010e 0108 0112 0110 027a 1c43 6172 6443  .........z.CardC
-00003320: 6f6e 6e65 6374 6f72 2e63 6172 645f 7365  onnector.card_se
-00003330: 745f 6c61 6265 6c63 1100 0000 0000 0000  t_labelc........
-00003340: 1d00 0000 0800 0000 4300 0000 73e6 0100  ........C...s...
-00003350: 0074 006a 0164 0183 0101 0064 0264 0364  .t.j.d.....d.d.d
-00003360: 0464 0564 0664 0764 0864 0867 087d 1174  .d.d.d.d.d.g.}.t
-00003370: 026a 037d 1274 026a 047d 1364 097d 1464  .j.}.t.j.}.d.}.d
-00003380: 097d 157c 127c 137c 147c 1567 047d 167c  .}.|.|.|.|.g.}.|
-00003390: 0e64 096b 0272 4c64 097d 176e 167c 0e64  .d.k.rLd.}.n.|.d
-000033a0: 0a40 0064 0a6b 0272 5e64 0b7d 176e 0464  .@.d.k.r^d.}.n.d
-000033b0: 0c7d 1764 0d74 057c 1183 0117 0074 057c  .}.d.t.|.....t.|
-000033c0: 0383 0117 0074 057c 0783 0117 0074 057c  .....t.|.....t.|
-000033d0: 0483 0117 0074 057c 0883 0117 007c 1717  .....t.|.....|..
-000033e0: 007d 187c 167c 1867 0137 007d 167c 1674  .}.|.|.g.7.}.|.t
-000033f0: 057c 1183 0167 017c 1117 0037 007d 167c  .|...g.|...7.}.|
-00003400: 167c 017c 0274 057c 0383 0167 037c 0317  .|.|.t.|...g.|..
-00003410: 0074 057c 0483 0167 0117 007c 0417 0037  .t.|...g...|...7
-00003420: 007d 167c 167c 057c 0674 057c 0783 0167  .}.|.|.|.t.|...g
-00003430: 037c 0717 0074 057c 0883 0167 0117 007c  .|...t.|...g...|
-00003440: 0817 0037 007d 167c 167c 0964 0e3f 007c  ...7.}.|.|.d.?.|
-00003450: 0964 0f40 007c 0a64 0e3f 007c 0a64 0f40  .d.@.|.d.?.|.d.@
-00003460: 0067 0437 007d 167c 167c 0b7c 0c7c 0d67  .g.7.}.|.|.|.|.g
-00003470: 0337 007d 167c 0e64 096b 0390 0172 787c  .7.}.|.d.k...rx|
-00003480: 167c 0e64 0e3f 007c 0e64 0f40 0067 0237  .|.d.?.|.d.@.g.7
-00003490: 007d 167c 167c 0f37 007d 1678 2c74 0674  .}.|.|.7.}.x,t.t
-000034a0: 0764 0e83 0183 0144 005d 1c7d 197c 167c  .d.....D.].}.|.|
-000034b0: 1064 0e7c 1914 003f 0064 0f40 0067 0137  .d.|...?.d.@.g.7
-000034c0: 007d 1690 0171 5857 007c 006a 087c 1683  .}...qXW.|.j.|..
-000034d0: 015c 037d 1a7d 1b7d 1c7c 1b64 106b 0290  .\.}.}.}.|.d.k..
-000034e0: 0172 dc7c 1c64 096b 0290 0172 dc7c 006a  .r.|.d.k...r.|.j
-000034f0: 0964 097c 0383 0201 007c 006a 0a64 116b  .d.|.....|.j.d.k
-00003500: 0290 0172 dc7c 006a 0b7c 1a64 0974 0c85  ...r.|.j.|.d.t..
-00003510: 0219 0083 0101 007c 006a 0d7c 1a74 0c74  .......|.j.|.t.t
-00003520: 0c74 0e17 0085 0219 0083 0101 007c 1a7c  .t...........|.|
-00003530: 1b7c 1c66 0353 0029 124e 7a0d 496e 2063  .|.f.S.).Nz.In c
-00003540: 6172 645f 7365 7475 70e9 4d00 0000 e975  ard_setup.M....u
-00003550: 0000 00e9 7300 0000 e963 0000 00e9 6c00  ....s....c....l.
-00003560: 0000 726d 0000 00e9 3000 0000 7201 0000  ..rm....0...r...
-00003570: 0069 0080 0000 e91e 0000 0072 2300 0000  .i.........r#...
-00003580: 7288 0000 0072 b200 0000 e9ff 0000 0072  r....r.........r
-00003590: 4100 0000 72af 0000 0029 0f72 2700 0000  A...r....).r'...
-000035a0: 7234 0000 0072 2b00 0000 72bc 0000 0072  r4...r+...r....r
-000035b0: 2c00 0000 7235 0000 00da 0872 6576 6572  ,...r5.....rever
-000035c0: 7365 64da 0572 616e 6765 7299 0000 00da  sed..ranger.....
-000035d0: 0773 6574 5f70 696e 7281 0000 00da 1b73  .set_pinr......s
-000035e0: 6174 6f64 696d 655f 7365 745f 756e 6c6f  atodime_set_unlo
-000035f0: 636b 5f63 6f75 6e74 6572 727f 0000 00da  ck_counterr.....
-00003600: 1a73 6174 6f64 696d 655f 7365 745f 756e  .satodime_set_un
-00003610: 6c6f 636b 5f73 6563 7265 7472 7d00 0000  lock_secretr}...
-00003620: 291d 7236 0000 005a 0a70 696e 5f74 7269  ).r6...Z.pin_tri
-00003630: 6573 305a 0b75 626c 6b5f 7472 6965 7330  es0Z.ublk_tries0
-00003640: 5a04 7069 6e30 5a05 7562 6c6b 305a 0a70  Z.pin0Z.ublk0Z.p
-00003650: 696e 5f74 7269 6573 315a 0b75 626c 6b5f  in_tries1Z.ublk_
-00003660: 7472 6965 7331 5a04 7069 6e31 5a05 7562  tries1Z.pin1Z.ub
-00003670: 6c6b 315a 076d 656d 7369 7a65 5a08 6d65  lk1Z.memsizeZ.me
-00003680: 6d73 697a 6532 5a11 6372 6561 7465 5f6f  msize2Z.create_o
-00003690: 626a 6563 745f 4143 4c5a 0e63 7265 6174  bject_ACLZ.creat
-000036a0: 655f 6b65 795f 4143 4c5a 0e63 7265 6174  e_key_ACLZ.creat
-000036b0: 655f 7069 6e5f 4143 4c5a 0c6f 7074 696f  e_pin_ACLZ.optio
-000036c0: 6e5f 666c 6167 73da 0e68 6d61 6373 6861  n_flags..hmacsha
-000036d0: 3136 305f 6b65 79da 0c61 6d6f 756e 745f  160_key..amount_
-000036e0: 6c69 6d69 7472 7c00 0000 729f 0000 0072  limitr|...r....r
-000036f0: 8700 0000 72a0 0000 0072 a100 0000 7298  ....r....r....r.
-00003700: 0000 005a 0a6f 7074 696f 6e73 697a 6572  ...Z.optionsizer
-00003710: ca00 0000 da01 6972 2200 0000 725d 0000  ......ir"...r]..
-00003720: 0072 5e00 0000 7237 0000 0072 3700 0000  .r^...r7...r7...
-00003730: 7238 0000 00da 0a63 6172 645f 7365 7475  r8.....card_setu
-00003740: 70bb 0100 0073 3e00 0000 0007 0a02 1401  p....s>.........
-00003750: 0601 0601 0401 0401 0c07 0801 0601 0c01  ................
-00003760: 0602 0401 3002 0a01 1201 2401 2401 2001  ....0.....$.$. .
-00003770: 0e01 0a01 1401 0801 1201 1c03 1001 1401  ................
-00003780: 0c02 0c01 1201 1602 7a18 4361 7264 436f  ........z.CardCo
-00003790: 6e6e 6563 746f 722e 6361 7264 5f73 6574  nnector.card_set
-000037a0: 7570 6302 0000 0000 0000 000d 0000 0005  upc.............
-000037b0: 0000 0043 0000 0073 0a01 0000 7400 7c01  ...C...s....t.|.
-000037c0: 8301 7401 6b08 721c 7402 7403 6a04 7c01  ..t.k.r.t.t.j.|.
-000037d0: 8301 8301 7d01 6e14 7400 7c01 8301 7403  ....}.n.t.|...t.
-000037e0: 6b08 7230 7402 7c01 8301 7d01 7405 6a06  k.r0t.|...}.t.j.
-000037f0: 6401 8301 0100 7407 6a08 7d02 7407 6a09  d.....t.j.}.t.j.
-00003800: 7d03 740a 7c01 8301 7d04 6402 7d05 740a  }.t.|...}.d.}.t.
-00003810: 7c01 8301 7d06 7c02 7c03 7c04 7c05 7c06  |...}.|.|.|.|.|.
-00003820: 6705 7c01 1700 7d07 7c00 6a0b 7c07 8301  g.|...}.|.j.|...
-00003830: 5c03 7d08 7d09 7d0a 6403 7d0b 7c09 6404  \.}.}.}.d.}.|.d.
-00003840: 6b02 72be 7c0a 6402 6b02 72be 7c00 6a0c  k.r.|.d.k.r.|.j.
-00003850: 7c08 8301 7d0b 7c0b 6a0d 6405 8301 6a0e  |...}.|.j.d...j.
-00003860: 8300 7d0c 7405 6a06 6406 7c0c 1700 8301  ..}.t.j.d.|.....
-00003870: 0100 6405 7c00 5f0f 6e48 7c09 6407 6b02  ..d.|._.nH|.d.k.
-00003880: 72e2 7c0a 6408 6b02 72e2 7405 6a10 6409  r.|.d.k.r.t.j.d.
-00003890: 8301 0100 7411 640a 8301 8201 6e24 7c09  ....t.d.....n$|.
-000038a0: 6407 6b02 6ff0 7c0a 640b 6b02 9001 7206  d.k.o.|.d.k...r.
-000038b0: 7405 6a10 640c 8301 0100 7411 640c 8301  t.j.d.....t.d...
-000038c0: 8201 7c0b 5300 290d 7aed 2049 6d70 6f72  ..|.S.).z. Impor
-000038d0: 7420 6120 7365 6564 2069 6e74 6f20 7468  t a seed into th
-000038e0: 6520 6465 7669 6365 0a20 2020 2020 2020  e device.       
-000038f0: 200a 2020 2020 2020 2020 5061 7261 6d65   .        Parame
-00003900: 7465 7273 3a20 0a20 2020 2020 2020 2073  ters: .        s
-00003910: 6565 6420 2873 7472 207c 2062 7974 6573  eed (str | bytes
-00003920: 207c 206c 6973 7429 3a20 7468 6520 7365   | list): the se
-00003930: 6564 2061 7320 6120 6865 785f 7374 7269  ed as a hex_stri
-00003940: 6e67 206f 7220 6279 7465 7320 6f72 206c  ng or bytes or l
-00003950: 6973 7420 6f66 2069 6e74 0a0a 2020 2020  ist of int..    
-00003960: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
-00003970: 2020 2020 2020 6175 7468 656e 7469 6b65        authentike
-00003980: 793a 2045 4350 7562 6b65 7920 6f62 6a65  y: ECPubkey obje
-00003990: 6374 2074 6861 7420 6964 656e 7469 6669  ct that identifi
-000039a0: 6573 2074 6865 2020 6465 7669 6365 0a20  es the  device. 
-000039b0: 2020 2020 2020 207a 1949 6e20 6361 7264         z.In card
-000039c0: 5f62 6970 3332 5f69 6d70 6f72 745f 7365  _bip32_import_se
-000039d0: 6564 7201 0000 004e 7241 0000 0054 7a2b  edr....NrA...Tz+
-000039e0: 5b63 6172 645f 6269 7033 325f 696d 706f  [card_bip32_impo
-000039f0: 7274 5f73 6565 645d 2061 7574 6865 6e74  rt_seed] authent
-00003a00: 696b 6579 5f63 6172 643d 2072 4200 0000  ikey_card= rB...
-00003a10: e917 0000 007a 3b45 7272 6f72 2064 7572  .....z;Error dur
-00003a20: 696e 6720 7365 6372 6574 2069 6d70 6f72  ing secret impor
-00003a30: 743a 2063 6172 6420 6973 2061 6c72 6561  t: card is alrea
-00003a40: 6479 2073 6565 6465 6420 2830 7839 4331  dy seeded (0x9C1
-00003a50: 3729 7a36 5365 6375 7265 2069 6d70 6f72  7)z6Secure impor
-00003a60: 7420 6661 696c 6564 3a20 6361 7264 2069  t failed: card i
-00003a70: 7320 616c 7265 6164 7920 7365 6564 6564  s already seeded
-00003a80: 2028 3078 3943 3137 2921 e90f 0000 007a   (0x9C17)!.....z
-00003a90: 3645 7272 6f72 2064 7572 696e 6720 7365  6Error during se
-00003aa0: 6372 6574 2069 6d70 6f72 743a 2069 6e76  cret import: inv
-00003ab0: 616c 6964 2070 6172 616d 6574 6572 2028  alid parameter (
-00003ac0: 3078 3943 3046 2929 1272 2600 0000 7275  0x9C0F)).r&...ru
-00003ad0: 0000 0072 c600 0000 724b 0000 00da 0766  ...r....rK.....f
-00003ae0: 726f 6d68 6578 7227 0000 0072 3400 0000  romhexr'...r4...
-00003af0: 722b 0000 0072 bc00 0000 722e 0000 0072  r+...r....r....r
-00003b00: 3500 0000 7299 0000 00da 2163 6172 645f  5...r.....!card_
-00003b10: 6269 7033 325f 7365 745f 6175 7468 656e  bip32_set_authen
-00003b20: 7469 6b65 795f 7075 626b 6579 da14 6765  tikey_pubkey..ge
-00003b30: 745f 7075 626c 6963 5f6b 6579 5f62 7974  t_public_key_byt
-00003b40: 6573 724c 0000 0072 7800 0000 da05 6572  esrL...rx.....er
-00003b50: 726f 72da 0943 6172 6445 7272 6f72 290d  ror..CardError).
-00003b60: 7236 0000 00da 0473 6565 6472 9f00 0000  r6.....seedr....
-00003b70: 7287 0000 0072 a000 0000 72a1 0000 0072  r....r....r....r
-00003b80: ca00 0000 7298 0000 0072 2200 0000 725d  ....r....r"...r]
-00003b90: 0000 0072 5e00 0000 72a4 0000 00da 0f61  ...r^...r......a
-00003ba0: 7574 6865 6e74 696b 6579 5f68 6578 7237  uthentikey_hexr7
-00003bb0: 0000 0072 3700 0000 7238 0000 00da 1663  ...r7...r8.....c
-00003bc0: 6172 645f 6269 7033 325f 696d 706f 7274  ard_bip32_import
-00003bd0: 5f73 6565 64f3 0100 0073 3200 0000 0009  _seed....s2.....
-00003be0: 0c01 1001 0c01 0802 0a01 0601 0601 0801  ................
-00003bf0: 0401 0801 1203 1003 0401 1001 0a01 0e01  ................
-00003c00: 0e08 0801 1001 0a01 0a01 1201 0a01 0802  ................
-00003c10: 7a24 4361 7264 436f 6e6e 6563 746f 722e  z$CardConnector.
-00003c20: 6361 7264 5f62 6970 3332 5f69 6d70 6f72  card_bip32_impor
-00003c30: 745f 7365 6564 6302 0000 0000 0000 0013  t_seedc.........
-00003c40: 0000 0005 0000 0043 0000 0073 8002 0000  .......C...s....
-00003c50: 7400 6a01 6401 8301 0100 7402 6a03 7d02  t.j.d.....t.j.}.
-00003c60: 6402 7d03 6403 7d04 6403 7d05 7404 7405  d.}.d.}.d.}.t.t.
-00003c70: 6a06 7c01 6404 1900 8301 8301 6405 6429  j.|.d.......d.d)
-00003c80: 8502 1900 7d06 7404 7405 6a06 7c01 6407  ....}.t.t.j.|.d.
-00003c90: 1900 8301 8301 7d07 7404 7405 6a06 7c01  ......}.t.t.j.|.
-00003ca0: 6408 1900 8301 8301 7d08 7404 7405 6a06  d.......}.t.t.j.
-00003cb0: 7c01 6409 1900 8301 8301 7d09 7c06 7c07  |.d.......}.|.|.
-00003cc0: 1700 7407 7c08 8301 640a 3f00 7407 7c08  ..t.|...d.?.t.|.
-00003cd0: 8301 640b 1600 6702 1700 7c08 1700 7407  ..d...g...|...t.
-00003ce0: 7c09 8301 6701 1700 7c09 1700 7d0a 7407  |...g...|...}.t.
-00003cf0: 7c0a 8301 7d0b 7c02 7c03 7c04 7c05 7c0b  |...}.|.|.|.|.|.
-00003d00: 6705 7c0a 1700 7d0c 7c00 6a08 7c0c 8301  g.|...}.|.j.|...
-00003d10: 5c03 7d0d 7d0e 7d0f 7c0e 640c 6b02 72dc  \.}.}.}.|.d.k.r.
-00003d20: 7c0f 6403 6b02 72dc 9001 6e54 7c0e 640d  |.d.k.r...nT|.d.
-00003d30: 6b02 6fea 7c0f 6403 6b02 9001 7204 7400  k.o.|.d.k...r.t.
-00003d40: 6a09 640e 8301 0100 740a 640e 8301 8201  j.d.....t.d.....
-00003d50: 9001 6e2c 7c0e 640f 6b02 9001 722e 7c0f  ..n,|.d.k...r.|.
-00003d60: 6410 6b02 9001 722e 7400 6a09 6411 8301  d.k...r.t.j.d...
-00003d70: 0100 740a 6412 8301 8201 9001 6e02 7c0e  ..t.d.......n.|.
-00003d80: 640f 6b02 9001 7256 7c0f 6413 6b02 9001  d.k...rV|.d.k...
-00003d90: 7256 7400 6a09 6414 8301 0100 740a 6415  rVt.j.d.....t.d.
-00003da0: 8301 8201 6eda 7c0e 640f 6b02 9001 727e  ....n.|.d.k...r~
-00003db0: 7c0f 6416 6b02 9001 727e 7400 6a09 6417  |.d.k...r~t.j.d.
-00003dc0: 8301 0100 740a 6417 8301 8201 6eb2 7c0e  ....t.d.....n.|.
-00003dd0: 640f 6b02 9001 72a6 7c0f 6418 6b02 9001  d.k...r.|.d.k...
-00003de0: 72a6 7400 6a09 6419 8301 0100 740a 641a  r.t.j.d.....t.d.
-00003df0: 8301 8201 6e8a 7c0e 640f 6b02 9001 72ce  ....n.|.d.k...r.
-00003e00: 7c0f 641b 6b02 9001 72ce 7400 6a09 641c  |.d.k...r.t.j.d.
-00003e10: 8301 0100 740a 641d 8301 8201 6e62 7c0e  ....t.d.....nb|.
-00003e20: 640f 6b02 9001 72f6 7c0f 641e 6b02 9001  d.k...r.|.d.k...
-00003e30: 72f6 7400 6a09 641f 8301 0100 740a 6420  r.t.j.d.....t.d 
-00003e40: 8301 8201 6e3a 7400 6a09 6421 740b 640b  ....n:t.j.d!t.d.
-00003e50: 7c0e 1400 7c0f 1700 8301 9b00 6422 9d03  |...|.......d"..
-00003e60: 8301 0100 740c 6423 740b 640b 7c0e 1400  ....t.d#t.d.|...
-00003e70: 7c0f 1700 8301 9b00 6422 9d03 8301 8201  |.......d"......
-00003e80: 7c06 6403 1900 7d10 7c10 6424 6b02 9002  |.d...}.|.d$k...
-00003e90: 726e 7c00 6a0d 6a0e 7c0d 8301 7d11 7c11  rn|.j.j.|...}.|.
-00003ea0: 6a0f 6425 8301 6a0b 8300 7d12 7400 6a01  j.d%..j...}.t.j.
-00003eb0: 6426 7c12 1700 8301 0100 7c11 5300 7c10  d&|.......|.S.|.
-00003ec0: 6427 6b02 9002 727c 6428 5300 6428 5300  d'k...r|d(S.d(S.
-00003ed0: 292a 61aa 0200 0049 6d70 6f72 7420 616e  )*a....Import an
-00003ee0: 2065 6e63 7279 7074 6564 2073 6563 7265   encrypted secre
-00003ef0: 7420 2842 4950 3332 206d 6173 7465 7273  t (BIP32 masters
-00003f00: 6565 6420 6f72 2032 4641 2073 6563 7265  eed or 2FA secre
-00003f10: 7429 2065 7870 6f72 7465 6420 6672 6f6d  t) exported from
-00003f20: 2061 2053 6565 644b 6565 7065 722e 0a20   a SeedKeeper.. 
-00003f30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003f40: 5468 6520 7365 6372 6574 2069 7320 656e  The secret is en
-00003f50: 6372 7970 7465 6420 7573 696e 6720 6120  crypted using a 
-00003f60: 7368 6172 6564 206b 6579 2067 656e 6572  shared key gener
-00003f70: 6174 6564 2075 7369 6e67 2045 4344 4820  ated using ECDH 
-00003f80: 7769 7468 2074 6865 2032 2064 6576 6963  with the 2 devic
-00003f90: 6573 2061 7574 6865 6e74 696b 6579 732e  es authentikeys.
-00003fa0: 0a20 2020 2020 2020 2042 6566 6f72 6520  .        Before 
-00003fb0: 696d 706f 7274 2063 616e 2062 6520 646f  import can be do
-00003fc0: 6e65 2c20 7468 6520 7477 6f20 6465 7669  ne, the two devi
-00003fd0: 6365 2073 686f 756c 6420 6265 2070 6169  ce should be pai
-00003fe0: 7265 6420 6279 2069 6d70 6f72 7469 6e67  red by importing
-00003ff0: 2074 6865 200a 2020 2020 2020 2020 5361   the .        Sa
-00004000: 746f 6368 6970 2d61 7574 6865 6e74 696b  tochip-authentik
-00004010: 6579 2069 6e20 7468 6520 5365 6564 4b65  ey in the SeedKe
-00004020: 6570 6572 2077 6974 6820 7365 6564 6b65  eper with seedke
-00004030: 6570 6572 5f69 6d70 6f72 745f 7365 6372  eper_import_secr
-00004040: 6574 2829 2c20 0a20 2020 2020 2020 2061  et(), .        a
-00004050: 6e64 2074 6865 2053 6565 644b 6565 7065  nd the SeedKeepe
-00004060: 722d 6175 7468 656e 7469 6b65 7920 696e  r-authentikey in
-00004070: 2074 6865 2053 6174 6f63 6869 7020 7769   the Satochip wi
-00004080: 7468 2063 6172 645f 696d 706f 7274 5f74  th card_import_t
-00004090: 7275 7374 6564 5f70 7562 6b65 7928 292e  rusted_pubkey().
-000040a0: 0a20 2020 2020 2020 2020 0a20 2020 2020  .         .     
-000040b0: 2020 2050 6172 616d 6574 6572 733a 200a     Parameters: .
-000040c0: 2020 2020 2020 2020 7365 6372 6574 5f64          secret_d
-000040d0: 6963 3a20 6120 6469 6374 696f 6e6e 6172  ic: a dictionnar
-000040e0: 7920 7468 6174 2064 6566 696e 6573 2074  y that defines t
-000040f0: 6865 2073 6563 7265 742c 2061 7320 7265  he secret, as re
-00004100: 7475 726e 6564 2062 7920 7365 6564 6b65  turned by seedke
-00004110: 6570 6572 5f65 7870 6f72 745f 7365 6372  eper_export_secr
-00004120: 6574 2829 0a0a 2020 2020 2020 2020 5265  et()..        Re
-00004130: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
-00004140: 6175 7468 656e 7469 6b65 793a 2045 4350  authentikey: ECP
-00004150: 7562 6b65 7920 6f62 6a65 6374 2074 6861  ubkey object tha
-00004160: 7420 6964 656e 7469 6669 6573 2074 6865  t identifies the
-00004170: 2020 6465 7669 6365 0a20 2020 2020 2020    device.       
-00004180: 207a 1f49 6e20 6361 7264 5f69 6d70 6f72   z.In card_impor
-00004190: 745f 656e 6372 7970 7465 645f 7365 6372  t_encrypted_secr
-000041a0: 6574 e9ac 0000 0072 0100 0000 da06 6865  et.....r......he
-000041b0: 6164 6572 7223 0000 0072 b900 0000 da02  aderr#...r......
-000041c0: 6976 da10 7365 6372 6574 5f65 6e63 7279  iv..secret_encry
-000041d0: 7074 6564 da04 686d 6163 72b2 0000 0072  pted..hmacr....r
-000041e0: ba00 0000 7241 0000 0072 7200 0000 7a48  ....rA...rr...zH
-000041f0: 4572 726f 7220 6475 7269 6e67 2073 6563  Error during sec
-00004200: 7265 7420 696d 706f 7274 3a20 6f70 6572  ret import: oper
-00004210: 6174 696f 6e20 6e6f 7420 7375 7070 6f72  ation not suppor
-00004220: 7465 6420 6279 2074 6865 2063 6172 6420  ted by the card 
-00004230: 2830 7836 4430 3029 7242 0000 0072 dd00  (0x6D00)rB...r..
-00004240: 0000 7a3b 4572 726f 7220 6475 7269 6e67  ..z;Error during
-00004250: 2073 6563 7265 7420 696d 706f 7274 3a20   secret import: 
-00004260: 6361 7264 2069 7320 616c 7265 6164 7920  card is already 
-00004270: 7365 6564 6564 2028 3078 3943 3137 297a  seeded (0x9C17)z
-00004280: 3653 6563 7572 6520 696d 706f 7274 2066  6Secure import f
-00004290: 6169 6c65 643a 2063 6172 6420 6973 2061  ailed: card is a
-000042a0: 6c72 6561 6479 2073 6565 6465 6420 2830  lready seeded (0
-000042b0: 7839 4331 3729 21e9 1800 0000 7a3e 4572  x9C17)!.....z>Er
-000042c0: 726f 7220 6475 7269 6e67 2073 6563 7265  ror during secre
-000042d0: 7420 696d 706f 7274 3a20 6361 7264 2061  t import: card a
-000042e0: 6c72 6561 6479 2072 6571 7569 7265 7320  lready requires 
-000042f0: 3246 4120 2830 7839 4331 3829 7a39 5365  2FA (0x9C18)z9Se
-00004300: 6375 7265 2069 6d70 6f72 7420 6661 696c  cure import fail
-00004310: 6564 3a20 6361 7264 2061 6c72 6561 6479  ed: card already
-00004320: 2072 6571 7569 7265 7320 3246 4120 2830   requires 2FA (0
-00004330: 7839 4331 3829 2172 de00 0000 7a36 4572  x9C18)!r....z6Er
-00004340: 726f 7220 6475 7269 6e67 2073 6563 7265  ror during secre
-00004350: 7420 696d 706f 7274 3a20 696e 7661 6c69  t import: invali
-00004360: 6420 7061 7261 6d65 7465 7220 2830 7839  d parameter (0x9
-00004370: 4330 4629 e933 0000 007a 2e45 7272 6f72  C0F).3...z.Error
-00004380: 2064 7572 696e 6720 7365 6372 6574 2069   during secret i
-00004390: 6d70 6f72 743a 2077 726f 6e67 204d 4143  mport: wrong MAC
-000043a0: 2028 3078 3943 3333 297a 2953 6563 7572   (0x9C33)z)Secur
-000043b0: 6520 696d 706f 7274 2066 6169 6c65 643a  e import failed:
+00001770: 7c00 5f11 6403 7c00 5f12 7413 6404 6701  |._.d.|._.t.d.g.
+00001780: 1400 7c00 5f14 7415 6404 6701 1400 7c00  ..|._.t.d.g...|.
+00001790: 5f16 7c03 7c00 5f17 6405 7c00 5f18 6400  _.|.|._.d.|._.d.
+000017a0: 7c00 5f19 6400 7c00 5f1a 7926 741b 6404  |._.d.|._.y&t.d.
+000017b0: 7c00 6a0a 6406 8d02 7c00 5f1c 7c00 6a1c  |.j.d...|._.|.j.
+000017c0: 6a1d 8300 7c00 5f1a 6407 7c00 5f1e 5700  j...|._.d.|._.W.
+000017d0: 6e1a 0400 741f 6b0a 72f8 0100 0100 0100  n...t.k.r.......
+000017e0: 6403 7c00 5f1e 5900 6e02 5800 7420 8300  d.|._.Y.n.X.t ..
+000017f0: 7c00 5f21 7422 7c00 8301 7c00 5f23 7c00  |._!t"|...|._#|.
+00001800: 6a21 6a24 7c00 6a23 8301 0100 6400 5300  j!j$|.j#....d.S.
+00001810: 2908 4e7a 164c 6f67 6769 6e67 2073 6574  ).Nz.Logging set
+00001820: 2074 6f20 6c65 7665 6c3a 207a 0b49 6e20   to level: z.In 
+00001830: 5f5f 696e 6974 5f5f 4672 0100 0000 725d  __init__Fr....r]
+00001840: 0000 0029 02da 0774 696d 656f 7574 5a08  ...)...timeoutZ.
+00001850: 6361 7264 5479 7065 5429 2572 2700 0000  cardTypeT)%r'...
+00001860: da08 7365 744c 6576 656c 7228 0000 00da  ..setLevelr(....
+00001870: 0373 7472 7234 0000 0072 0e00 0000 da06  .strr4...r......
+00001880: 7061 7273 6572 725a 0000 0072 3e00 0000  parserrZ...r>...
+00001890: 7202 0000 005a 0863 6172 6474 7970 65da  r....Z.cardtype.
+000018a0: 096e 6565 6473 5f32 4641 da09 6973 5f73  .needs_2FA..is_s
+000018b0: 6565 6465 64da 0a73 6574 7570 5f64 6f6e  eeded..setup_don
+000018c0: 6572 5800 0000 da02 7363 da07 7069 6e5f  erX.....sc..pin_
+000018d0: 6e62 72da 0370 696e da08 6973 5f6f 776e  nbr..pin..is_own
+000018e0: 6572 da12 5349 5a45 5f55 4e4c 4f43 4b5f  er..SIZE_UNLOCK_
+000018f0: 5345 4352 4554 da0d 756e 6c6f 636b 5f73  SECRET..unlock_s
+00001900: 6563 7265 74da 1353 495a 455f 554e 4c4f  ecret..SIZE_UNLO
+00001910: 434b 5f43 4f55 4e54 4552 da0e 756e 6c6f  CK_COUNTER..unlo
+00001920: 636b 5f63 6f75 6e74 6572 725c 0000 00da  ck_counterr\....
+00001930: 0963 6172 645f 7479 7065 da08 6365 7274  .card_type..cert
+00001940: 5f70 656d 7247 0000 0072 0300 0000 5a0b  _pemrG...r....Z.
+00001950: 6361 7264 7265 7175 6573 745a 0b77 6169  cardrequestZ.wai
+00001960: 7466 6f72 6361 7264 7246 0000 0072 0800  tforcardrF...r..
+00001970: 0000 7205 0000 005a 0b63 6172 646d 6f6e  ..r....Z.cardmon
+00001980: 6974 6f72 723d 0000 005a 0c63 6172 646f  itorr=...Z.cardo
+00001990: 6273 6572 7665 7272 4900 0000 2904 7236  bserverrI...).r6
+000019a0: 0000 0072 5a00 0000 5a08 6c6f 676c 6576  ...rZ...Z.loglev
+000019b0: 656c 725c 0000 0072 3700 0000 7237 0000  elr\...r7...r7..
+000019c0: 0072 3800 0000 7240 0000 00a1 0000 0073  .r8...r@.......s
+000019d0: 4000 0000 0001 0a01 1401 0a01 0601 0a01  @...............
+000019e0: 0601 0a01 0801 0801 0601 0601 0601 0601  ................
+000019f0: 0602 0601 0602 0601 0c01 0c02 0601 0601  ................
+00001a00: 0602 0601 0201 1001 0c02 0a01 0e01 0c02  ................
+00001a10: 0801 0a01 7a16 4361 7264 436f 6e6e 6563  ....z.CardConnec
+00001a20: 746f 722e 5f5f 696e 6974 5f5f 6302 0000  tor.__init__c...
+00001a30: 0000 0000 0007 0000 0005 0000 0043 0000  .............C..
+00001a40: 0073 9401 0000 7400 6a01 6401 8301 0100  .s....t.j.d.....
+00001a50: 9001 787a 7c00 6a02 9001 7286 7c01 6402  ..xz|.j...r.|.d.
+00001a60: 1900 7d02 7c00 6a03 7242 7c02 6403 6404  ..}.|.j.rB|.d.d.
+00001a70: 6405 7404 6a05 6704 6b07 7242 7c00 6a06  d.t.j.g.k.rB|.j.
+00001a80: 7c01 8301 7d03 6e04 7c01 7d03 7c00 6a07  |...}.n.|.}.|.j.
+00001a90: 6a08 6a09 7c03 8301 5c03 7d04 7d05 7d06  j.j.|...\.}.}.}.
+00001aa0: 7c05 6406 6b02 7296 7c06 6407 6b02 7296  |.d.k.r.|.d.k.r.
+00001ab0: 7c00 6a03 728c 7c02 6403 6404 6405 7404  |.j.r.|.d.d.d.t.
+00001ac0: 6a05 6704 6b07 728c 7c00 6a0a 7c04 8301  j.g.k.r.|.j.|...
+00001ad0: 7d04 7c04 7c05 7c06 6603 5300 7c05 6408  }.|.|.|.f.S.|.d.
+00001ae0: 6b02 72b6 7c06 6409 6b02 72b6 7c00 6a0b  k.r.|.d.k.r.|.j.
+00001af0: 8300 5c03 7d04 7d05 7d06 710e 7c05 640a  ..\.}.}.}.q.|.d.
+00001b00: 6b02 72d4 7c06 6405 6b02 72d4 740c 640b  k.r.|.d.k.r.t.d.
+00001b10: 7c02 640c 8d02 8201 710e 7c05 6408 6b02  |.d.....q.|.d.k.
+00001b20: 72f2 7c06 640d 6b02 72f2 740d 640e 7c02  r.|.d.k.r.t.d.|.
+00001b30: 640c 8d02 8201 710e 7c05 6408 6b02 9001  d.....q.|.d.k...
+00001b40: 7214 7c06 640f 6b02 9001 7214 740e 6410  r.|.d.k...r.t.d.
+00001b50: 7c02 640c 8d02 8201 710e 7c05 6408 6b02  |.d.....q.|.d.k.
+00001b60: 9001 7236 7c06 6411 6b02 9001 7236 740f  ..r6|.d.k...r6t.
+00001b70: 6412 7c02 640c 8d02 8201 710e 7c05 6408  d.|.d.....q.|.d.
+00001b80: 6b02 9001 7258 7c06 6413 6b02 9001 7258  k...rX|.d.k...rX
+00001b90: 7410 6414 7c02 640c 8d02 8201 710e 7c05  t.d.|.d.....q.|.
+00001ba0: 6408 6b02 9001 727a 7c06 6415 6b02 9001  d.k...rz|.d.k...
+00001bb0: 727a 7411 6416 7c02 640c 8d02 8201 710e  rzt.d.|.d.....q.
+00001bc0: 7c04 7c05 7c06 6603 5300 710e 5700 7412  |.|.|.f.S.q.W.t.
+00001bd0: 6417 8301 8201 6400 5300 2918 4e7a 1049  d.....d.S.).Nz.I
+00001be0: 6e20 6361 7264 5f74 7261 6e73 6d69 7472  n card_transmitr
+00001bf0: 0c00 0000 7265 0000 00e9 8100 0000 e982  ....re..........
+00001c00: 0000 0072 4100 0000 7201 0000 0072 4200  ...rA...r....rB.
+00001c10: 0000 e906 0000 00e9 6a00 0000 7a10 4361  ........j...z.Ca
+00001c20: 7264 5365 6c65 6374 2065 7272 6f72 2901  rdSelect error).
+00001c30: da03 696e 73e9 1000 0000 7a1f 4150 4455  ..ins.....z.APDU
+00001c40: 2065 7272 6f72 3a20 7772 6f6e 6720 5031   error: wrong P1
+00001c50: 2070 6172 616d 6574 6572 73e9 5100 0000   parameters.Q...
+00001c60: 7a25 5361 746f 6469 6d65 2065 7272 6f72  z%Satodime error
+00001c70: 3a20 696e 636f 7272 6563 7420 756e 6c6f  : incorrect unlo
+00001c80: 636b 2063 6f64 65e9 5200 0000 7a27 5361  ck code.R...z'Sa
+00001c90: 746f 6469 6d65 2065 7272 6f72 3a20 696e  todime error: in
+00001ca0: 636f 7272 6563 7420 6b65 7973 6c6f 7420  correct keyslot 
+00001cb0: 7374 6174 6572 6600 0000 7a28 5361 746f  staterf...z(Sato
+00001cc0: 6469 6d65 2065 7272 6f72 3a20 696e 636f  dime error: inco
+00001cd0: 7272 6563 7420 7072 6f74 6f63 6f6c 206d  rrect protocol m
+00001ce0: 6564 6961 e954 0000 007a 2653 6174 6f64  edia.T...z&Satod
+00001cf0: 696d 6520 6572 726f 723a 2075 6e6b 6e6f  ime error: unkno
+00001d00: 776e 2070 726f 746f 636f 6c20 6d65 6469  wn protocol medi
+00001d10: 617a 224e 6f20 6361 7264 2066 6f75 6e64  az"No card found
+00001d20: 2120 506c 6561 7365 2069 6e73 6572 7420  ! Please insert 
+00001d30: 6361 7264 2129 1372 2700 0000 7234 0000  card!).r'...r4..
+00001d40: 0072 4600 0000 7258 0000 0072 2b00 0000  .rF...rX...r+...
+00001d50: da0e 494e 535f 4745 545f 5354 4154 5553  ..INS_GET_STATUS
+00001d60: da1b 6361 7264 5f65 6e63 7279 7074 5f73  ..card_encrypt_s
+00001d70: 6563 7572 655f 6368 616e 6e65 6c72 4700  ecure_channelrG.
+00001d80: 0000 7248 0000 00da 0874 7261 6e73 6d69  ..rH.....transmi
+00001d90: 74da 1b63 6172 645f 6465 6372 7970 745f  t..card_decrypt_
+00001da0: 7365 6375 7265 5f63 6861 6e6e 656c da0f  secure_channel..
+00001db0: 6361 7264 5f76 6572 6966 795f 5049 4eda  card_verify_PIN.
+00001dc0: 0f43 6172 6453 656c 6563 7445 7272 6f72  .CardSelectError
+00001dd0: da10 496e 636f 7272 6563 7450 3145 7272  ..IncorrectP1Err
+00001de0: 6f72 da18 496e 636f 7272 6563 7455 6e6c  or..IncorrectUnl
+00001df0: 6f63 6b43 6f64 6545 7272 6f72 da1a 496e  ockCodeError..In
+00001e00: 636f 7272 6563 744b 6579 736c 6f74 5374  correctKeyslotSt
+00001e10: 6174 6545 7272 6f72 da1b 496e 636f 7272  ateError..Incorr
+00001e20: 6563 7450 726f 746f 636f 6c4d 6564 6961  ectProtocolMedia
+00001e30: 4572 726f 72da 1955 6e6b 6e6f 776e 5072  Error..UnknownPr
+00001e40: 6f74 6f63 6f6c 4d65 6469 6145 7272 6f72  otocolMediaError
+00001e50: da13 4361 7264 4e6f 7450 7265 7365 6e74  ..CardNotPresent
+00001e60: 4572 726f 7229 0772 3600 0000 5a0a 706c  Error).r6...Z.pl
+00001e70: 6169 6e5f 6170 6475 7289 0000 00da 0461  ain_apdur......a
+00001e80: 7064 7572 2200 0000 725e 0000 0072 5f00  pdur"...r^...r_.
+00001e90: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
+00001ea0: 00da 0d63 6172 645f 7472 616e 736d 6974  ...card_transmit
+00001eb0: cd00 0000 7336 0000 0000 010a 010c 0308  ....s6..........
+00001ec0: 0118 010c 0204 0314 0310 0118 010a 010a  ................
+00001ed0: 0210 0110 0110 010e 0310 010e 0114 010e  ................
+00001ee0: 0114 010e 0114 010e 0114 010e 040e 037a  ...............z
+00001ef0: 1b43 6172 6443 6f6e 6e65 6374 6f72 2e63  .CardConnector.c
+00001f00: 6172 645f 7472 616e 736d 6974 6301 0000  ard_transmitc...
+00001f10: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00001f20: 0073 1600 0000 7400 6a01 6401 8301 0100  .s....t.j.d.....
+00001f30: 7c00 6a02 6a03 6a04 8300 5300 2902 4e7a  |.j.j.j...S.).Nz
+00001f40: 1149 6e20 6361 7264 5f67 6574 5f41 5452  .In card_get_ATR
+00001f50: 2829 2905 7227 0000 0072 3400 0000 7247  ()).r'...r4...rG
+00001f60: 0000 0072 4800 0000 5a06 6765 7441 5452  ...rH...Z.getATR
+00001f70: 2901 7236 0000 0072 3700 0000 7237 0000  ).r6...r7...r7..
+00001f80: 0072 3800 0000 da0c 6361 7264 5f67 6574  .r8.....card_get
+00001f90: 5f41 5452 f900 0000 7304 0000 0000 010a  _ATR....s.......
+00001fa0: 017a 1a43 6172 6443 6f6e 6e65 6374 6f72  .z.CardConnector
+00001fb0: 2e63 6172 645f 6765 745f 4154 5263 0100  .card_get_ATRc..
+00001fc0: 0000 0000 0000 0900 0000 0400 0000 4300  ..............C.
+00001fd0: 0000 7344 0000 0074 006a 0164 0183 0101  ..sD...t.j.d....
+00001fe0: 0064 027d 0164 037d 0264 047d 0364 057d  .d.}.d.}.d.}.d.}
+00001ff0: 047c 017c 027c 037c 0467 047d 057c 006a  .|.|.|.|.g.}.|.j
+00002000: 026a 036a 047c 0583 015c 037d 067d 077d  .j.j.|...\.}.}.}
+00002010: 087c 067c 077c 0866 0353 0029 064e 7a10  .|.|.|.f.S.).Nz.
+00002020: 496e 2063 6172 645f 6765 745f 4350 4c43  In card_get_CPLC
+00002030: e980 0000 00e9 ca00 0000 e99f 0000 00e9  ................
+00002040: 7f00 0000 2905 7227 0000 0072 3400 0000  ....).r'...r4...
+00002050: 7247 0000 0072 4800 0000 7290 0000 0029  rG...rH...r....)
+00002060: 0972 3600 0000 da03 636c 6172 8900 0000  .r6.....clar....
+00002070: da02 7031 da02 7032 729a 0000 0072 2200  ..p1..p2r....r".
+00002080: 0000 725e 0000 0072 5f00 0000 7237 0000  ..r^...r_...r7..
+00002090: 0072 3700 0000 7238 0000 0072 4a00 0000  .r7...r8...rJ...
+000020a0: fd00 0000 7310 0000 0000 010a 0104 0104  ....s...........
+000020b0: 0104 0104 010c 0214 017a 1b43 6172 6443  .........z.CardC
+000020c0: 6f6e 6e65 6374 6f72 2e63 6172 645f 6765  onnector.card_ge
+000020d0: 745f 4350 4c43 6301 0000 0000 0000 0009  t_CPLCc.........
+000020e0: 0000 0004 0000 0043 0000 0073 4400 0000  .......C...sD...
+000020f0: 7400 6a01 6401 8301 0100 6402 7d01 6403  t.j.d.....d.}.d.
+00002100: 7d02 6404 7d03 6405 7d04 7c01 7c02 7c03  }.d.}.d.}.|.|.|.
+00002110: 7c04 6704 7d05 7c00 6a02 6a03 6a04 7c05  |.g.}.|.j.j.j.|.
+00002120: 8301 5c03 7d06 7d07 7d08 7c06 7c07 7c08  ..\.}.}.}.|.|.|.
+00002130: 6603 5300 2906 4e7a 0f49 6e20 6361 7264  f.S.).Nz.In card
+00002140: 5f67 6574 5f49 494e 729d 0000 0072 9e00  _get_IINr....r..
+00002150: 0000 7201 0000 00e9 4200 0000 2905 7227  ..r.....B...).r'
+00002160: 0000 0072 3400 0000 7247 0000 0072 4800  ...r4...rG...rH.
+00002170: 0000 7290 0000 0029 0972 3600 0000 72a1  ..r....).r6...r.
+00002180: 0000 0072 8900 0000 72a2 0000 0072 a300  ...r....r....r..
+00002190: 0000 729a 0000 0072 2200 0000 725e 0000  ..r....r"...r^..
+000021a0: 0072 5f00 0000 7237 0000 0072 3700 0000  .r_...r7...r7...
+000021b0: 7238 0000 0072 4d00 0000 0801 0000 7310  r8...rM.......s.
+000021c0: 0000 0000 010a 0104 0104 0104 0104 010c  ................
+000021d0: 0214 017a 1a43 6172 6443 6f6e 6e65 6374  ...z.CardConnect
+000021e0: 6f72 2e63 6172 645f 6765 745f 4949 4e63  or.card_get_IINc
+000021f0: 0100 0000 0000 0000 0900 0000 0400 0000  ................
+00002200: 4300 0000 7344 0000 0074 006a 0164 0183  C...sD...t.j.d..
+00002210: 0101 0064 027d 0164 037d 0264 047d 0364  ...d.}.d.}.d.}.d
+00002220: 057d 047c 017c 027c 037c 0467 047d 057c  .}.|.|.|.|.g.}.|
+00002230: 006a 026a 036a 047c 0583 015c 037d 067d  .j.j.j.|...\.}.}
+00002240: 077d 087c 067c 077c 0866 0353 0029 064e  .}.|.|.|.f.S.).N
+00002250: 7a0f 496e 2063 6172 645f 6765 745f 4349  z.In card_get_CI
+00002260: 4e72 9d00 0000 729e 0000 0072 0100 0000  Nr....r....r....
+00002270: e945 0000 0029 0572 2700 0000 7234 0000  .E...).r'...r4..
+00002280: 0072 4700 0000 7248 0000 0072 9000 0000  .rG...rH...r....
+00002290: 2909 7236 0000 0072 a100 0000 7289 0000  ).r6...r....r...
+000022a0: 0072 a200 0000 72a3 0000 0072 9a00 0000  .r....r....r....
+000022b0: 7222 0000 0072 5e00 0000 725f 0000 0072  r"...r^...r_...r
+000022c0: 3700 0000 7237 0000 0072 3800 0000 724e  7...r7...r8...rN
+000022d0: 0000 0013 0100 0073 1000 0000 0001 0a01  .......s........
+000022e0: 0401 0401 0401 0401 0c02 1401 7a1a 4361  ............z.Ca
+000022f0: 7264 436f 6e6e 6563 746f 722e 6361 7264  rdConnector.card
+00002300: 5f67 6574 5f43 494e 6301 0000 0000 0000  _get_CINc.......
+00002310: 0001 0000 0003 0000 0043 0000 0073 8600  .........C...s..
+00002320: 0000 7400 6a01 6401 8301 0100 6400 7c00  ..t.j.d.....d.|.
+00002330: 5f02 6400 7c00 5f03 6400 7c00 5f04 6400  _.d.|._.d.|._.d.
+00002340: 7c00 5f05 6400 7c00 5f06 6400 7c00 5f07  |._.d.|._.d.|._.
+00002350: 6402 7c00 5f08 6403 7c00 5f09 7c00 6a0a  d.|._.d.|._.|.j.
+00002360: 7252 7c00 6a0a 6a0b 6a0c 8300 0100 6400  rR|.j.j.j.....d.
+00002370: 7c00 5f0a 7c00 6a0d 6400 6b09 726a 7c00  |._.|.j.d.k.rj|.
+00002380: 6a0d 6a0e 6404 6402 8302 0100 6400 7c00  j.j.d.d.....d.|.
+00002390: 6a0f 5f10 6400 7c00 6a0f 5f11 6400 7c00  j._.d.|.j._.d.|.
+000023a0: 6a0f 5f12 6400 5300 2905 4e7a 1449 6e20  j._.d.S.).Nz.In 
+000023b0: 6361 7264 5f64 6973 636f 6e6e 6563 7428  card_disconnect(
+000023c0: 2946 725d 0000 0072 4400 0000 2913 7227  )Fr]...rD...).r'
+000023d0: 0000 0072 3400 0000 727d 0000 0072 7c00  ...r4...r}...r|.
+000023e0: 0000 7279 0000 0072 7800 0000 727a 0000  ..ry...rx...rz..
+000023f0: 0072 5800 0000 7246 0000 0072 8300 0000  .rX...rF...r....
+00002400: 7247 0000 0072 4800 0000 7220 0000 0072  rG...rH...r ...r
+00002410: 5a00 0000 725b 0000 0072 7700 0000 da0b  Z...r[...rw.....
+00002420: 6175 7468 656e 7469 6b65 795a 1261 7574  authentikeyZ.aut
+00002430: 6865 6e74 696b 6579 5f63 6f6f 7264 785a  hentikey_coordxZ
+00002440: 1861 7574 6865 6e74 696b 6579 5f66 726f  .authentikey_fro
+00002450: 6d5f 7374 6f72 6167 6529 0172 3600 0000  m_storage).r6...
+00002460: 7237 0000 0072 3700 0000 7238 0000 0072  r7...r7...r8...r
+00002470: 5600 0000 1e01 0000 7322 0000 0000 010a  V.......s"......
+00002480: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00002490: 0106 010c 0106 010a 010e 0208 0108 017a  ...............z
+000024a0: 1d43 6172 6443 6f6e 6e65 6374 6f72 2e63  .CardConnector.c
+000024b0: 6172 645f 6469 7363 6f6e 6e65 6374 6303  ard_disconnectc.
+000024c0: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
+000024d0: 0000 0073 0c00 0000 6401 7c01 1400 7c02  ...s....d.|...|.
+000024e0: 1700 5300 2902 4e72 8a00 0000 7237 0000  ..S.).Nr....r7..
+000024f0: 0029 0372 3600 0000 725e 0000 0072 5f00  .).r6...r^...r_.
+00002500: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
+00002510: 00da 0867 6574 5f73 7731 3233 0100 0073  ...get_sw123...s
+00002520: 0200 0000 0001 7a16 4361 7264 436f 6e6e  ......z.CardConn
+00002530: 6563 746f 722e 6765 745f 7377 3132 6301  ector.get_sw12c.
+00002540: 0000 0000 0000 0003 0000 0011 0000 0043  ...............C
+00002550: 0000 0073 b000 0000 7400 6a01 6401 8301  ...s....t.j.d...
+00002560: 0100 7c00 6a02 6400 6b02 7222 6402 6403  ..|.j.d.k.r"d.d.
+00002570: 6404 6703 7c00 5f02 6e16 7403 7c00 6a02  d.g.|._.n.t.|.j.
+00002580: 7404 8302 7238 7c00 6a02 6701 7c00 5f02  t...r8|.j.g.|._.
+00002590: 7866 7c00 6a02 4400 5d5c 7d01 7934 7c01  xf|.j.D.]\}.y4|.
+000025a0: 6402 6b02 7256 7c00 6a05 8300 5300 7c01  d.k.rV|.j...S.|.
+000025b0: 6403 6b02 7266 7c00 6a06 8300 5300 7c01  d.k.rf|.j...S.|.
+000025c0: 6404 6b02 7276 7c00 6a07 8300 5300 5700  d.k.rv|.j...S.W.
+000025d0: 7140 0400 7408 6b0a 729a 0100 7d02 0100  q@..t.k.r...}...
+000025e0: 7a06 5700 5900 6400 6400 7d02 7e02 5800  z.W.Y.d.d.}.~.X.
+000025f0: 7140 5800 7140 5700 7408 6405 6406 6407  q@X.q@W.t.d.d.d.
+00002600: 8d02 8201 6400 5300 2908 4e7a 0e49 6e20  ....d.S.).Nz.In 
+00002610: 6361 7264 5f73 656c 6563 745a 0873 6174  card_selectZ.sat
+00002620: 6f63 6869 705a 0a73 6565 646b 6565 7065  ochipZ.seedkeepe
+00002630: 72da 0873 6174 6f64 696d 657a 1043 6172  r..satodimez.Car
+00002640: 6453 656c 6563 7420 6572 726f 7272 6500  dSelect errorre.
+00002650: 0000 2901 7289 0000 0029 0972 2700 0000  ..).r....).r'...
+00002660: 7234 0000 0072 5c00 0000 da0a 6973 696e  r4...r\.....isin
+00002670: 7374 616e 6365 7276 0000 00da 1463 6172  stancerv.....car
+00002680: 645f 7365 6c65 6374 5f73 6174 6f63 6869  d_select_satochi
+00002690: 70da 1663 6172 645f 7365 6c65 6374 5f73  p..card_select_s
+000026a0: 6565 646b 6565 7065 72da 1463 6172 645f  eedkeeper..card_
+000026b0: 7365 6c65 6374 5f73 6174 6f64 696d 6572  select_satodimer
+000026c0: 9300 0000 2903 7236 0000 005a 0b63 6172  ....).r6...Z.car
+000026d0: 645f 6170 706c 6574 da02 6578 7237 0000  d_applet..exr7..
+000026e0: 0072 3700 0000 7238 0000 0072 5500 0000  .r7...r8...rU...
+000026f0: 3601 0000 7320 0000 0000 010a 030a 010e  6...s ..........
+00002700: 010c 010a 030c 0102 0108 0108 0108 0108  ................
+00002710: 0108 010c 0110 0116 037a 1943 6172 6443  .........z.CardC
+00002720: 6f6e 6e65 6374 6f72 2e63 6172 645f 7365  onnector.card_se
+00002730: 6c65 6374 6301 0000 0000 0000 0005 0000  lectc...........
+00002740: 0003 0000 0043 0000 0073 4200 0000 7400  .....C...sB...t.
+00002750: 6a01 7402 7400 6a03 8301 6701 1700 7400  j.t.t.j...g...t.
+00002760: 6a03 1700 7d01 7c00 6a04 7c01 8301 5c03  j...}.|.j.|...\.
+00002770: 7d02 7d03 7d04 6401 7c00 5f05 7406 6a07  }.}.}.d.|._.t.j.
+00002780: 6402 8301 0100 7c02 7c03 7c04 6603 5300  d.....|.|.|.f.S.
+00002790: 2903 4e5a 0853 6174 6f63 6869 707a 1146  ).NZ.Satochipz.F
+000027a0: 6f75 6e64 2061 2053 6174 6f63 6869 7021  ound a Satochip!
+000027b0: 2908 7264 0000 00da 0653 454c 4543 5472  ).rd.....SELECTr
+000027c0: 3500 0000 da0c 5341 544f 4348 4950 5f41  5.....SATOCHIP_A
+000027d0: 4944 729b 0000 0072 8300 0000 7227 0000  IDr....r....r'..
+000027e0: 0072 3400 0000 2905 7236 0000 0072 9a00  .r4...).r6...r..
+000027f0: 0000 7222 0000 0072 5e00 0000 725f 0000  ..r"...r^...r_..
+00002800: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
+00002810: 72aa 0000 004e 0100 0073 0a00 0000 0001  r....N...s......
+00002820: 1801 1001 0601 0a01 7a22 4361 7264 436f  ........z"CardCo
+00002830: 6e6e 6563 746f 722e 6361 7264 5f73 656c  nnector.card_sel
+00002840: 6563 745f 7361 746f 6368 6970 6301 0000  ect_satochipc...
+00002850: 0000 0000 0005 0000 0003 0000 0043 0000  .............C..
+00002860: 0073 4200 0000 7400 6a01 7402 7400 6a03  .sB...t.j.t.t.j.
+00002870: 8301 6701 1700 7400 6a03 1700 7d01 7c00  ..g...t.j...}.|.
+00002880: 6a04 7c01 8301 5c03 7d02 7d03 7d04 6401  j.|...\.}.}.}.d.
+00002890: 7c00 5f05 7406 6a07 6402 8301 0100 7c02  |._.t.j.d.....|.
+000028a0: 7c03 7c04 6603 5300 2903 4e5a 0a53 6565  |.|.f.S.).NZ.See
+000028b0: 644b 6565 7065 727a 1346 6f75 6e64 2061  dKeeperz.Found a
+000028c0: 2053 6565 644b 6565 7065 7221 2908 7264   SeedKeeper!).rd
+000028d0: 0000 0072 ae00 0000 7235 0000 00da 0e53  ...r....r5.....S
+000028e0: 4545 444b 4545 5045 525f 4149 4472 9b00  EEDKEEPER_AIDr..
+000028f0: 0000 7283 0000 0072 2700 0000 7234 0000  ..r....r'...r4..
+00002900: 0029 0572 3600 0000 729a 0000 0072 2200  .).r6...r....r".
+00002910: 0000 725e 0000 0072 5f00 0000 7237 0000  ..r^...r_...r7..
+00002920: 0072 3700 0000 7238 0000 0072 ab00 0000  .r7...r8...r....
+00002930: 5501 0000 730a 0000 0000 0118 0110 0106  U...s...........
+00002940: 010a 017a 2443 6172 6443 6f6e 6e65 6374  ...z$CardConnect
+00002950: 6f72 2e63 6172 645f 7365 6c65 6374 5f73  or.card_select_s
+00002960: 6565 646b 6565 7065 7263 0100 0000 0000  eedkeeperc......
+00002970: 0000 0500 0000 0300 0000 4300 0000 7342  ..........C...sB
+00002980: 0000 0074 006a 0174 0274 006a 0383 0167  ...t.j.t.t.j...g
+00002990: 0117 0074 006a 0317 007d 017c 006a 047c  ...t.j...}.|.j.|
+000029a0: 0183 015c 037d 027d 037d 0464 017c 005f  ...\.}.}.}.d.|._
+000029b0: 0574 066a 0764 0283 0101 007c 027c 037c  .t.j.d.....|.|.|
+000029c0: 0466 0353 0029 034e da08 5361 746f 6469  .f.S.).N..Satodi
+000029d0: 6d65 7a11 466f 756e 6420 6120 5361 746f  mez.Found a Sato
+000029e0: 6469 6d65 2129 0872 6400 0000 72ae 0000  dime!).rd...r...
+000029f0: 0072 3500 0000 da0c 5341 544f 4449 4d45  .r5.....SATODIME
+00002a00: 5f41 4944 729b 0000 0072 8300 0000 7227  _AIDr....r....r'
+00002a10: 0000 0072 3400 0000 2905 7236 0000 0072  ...r4...).r6...r
+00002a20: 9a00 0000 7222 0000 0072 5e00 0000 725f  ....r"...r^...r_
+00002a30: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
+00002a40: 0000 72ac 0000 005c 0100 0073 0a00 0000  ..r....\...s....
+00002a50: 0001 1801 1001 0601 0a01 7a22 4361 7264  ..........z"Card
+00002a60: 436f 6e6e 6563 746f 722e 6361 7264 5f73  Connector.card_s
+00002a70: 656c 6563 745f 7361 746f 6469 6d65 6301  elect_satodimec.
+00002a80: 0000 0000 0000 000a 0000 0005 0000 0043  ...............C
+00002a90: 0000 0073 2602 0000 7400 6a01 6401 8301  ...s&...t.j.d...
+00002aa0: 0100 7402 6a03 7d01 7402 6a04 7d02 6402  ..t.j.}.t.j.}.d.
+00002ab0: 7d03 6402 7d04 7c01 7c02 7c03 7c04 6704  }.d.}.|.|.|.|.g.
+00002ac0: 7d05 7c00 6a05 7c05 8301 5c03 7d06 7d07  }.|.j.|...\.}.}.
+00002ad0: 7d08 6900 7d09 7c07 6403 6b02 6f4c 7c08  }.i.}.|.d.k.oL|.
+00002ae0: 6402 6b02 9001 72bc 7c06 6402 1900 7c09  d.k...r.|.d...|.
+00002af0: 6404 3c00 7c06 6405 1900 7c09 6406 3c00  d.<.|.d...|.d.<.
+00002b00: 7c06 6407 1900 7c09 6408 3c00 7c06 6409  |.d...|.d.<.|.d.
+00002b10: 1900 7c09 640a 3c00 7c09 6404 1900 640b  ..|.d.<.|.d...d.
+00002b20: 3e00 7c09 6406 1900 1700 7c09 640c 3c00  >.|.d.....|.d.<.
+00002b30: 7406 7c06 8301 640b 6b05 72e2 7c06 640d  t.|...d.k.r.|.d.
+00002b40: 1900 7c09 640e 3c00 7c06 640f 1900 7c09  ..|.d.<.|.d...|.
+00002b50: 6410 3c00 7c06 6411 1900 7c09 6412 3c00  d.<.|.d...|.d.<.
+00002b60: 7c06 6413 1900 7c09 6414 3c00 6415 0400  |.d...|.d.<.d...
+00002b70: 7c00 5f07 7c09 6416 3c00 7406 7c06 8301  |._.|.d.<.t.|...
+00002b80: 6417 6b05 9001 7210 7c06 640b 1900 6402  d.k...r.|.d...d.
+00002b90: 6b02 9001 7202 6415 6e02 6418 0400 7c00  k...r.d.n.d...|.
+00002ba0: 5f07 7c09 6416 3c00 7406 7c06 8301 6419  _.|.d.<.t.|...d.
+00002bb0: 6b05 9001 723e 7c06 6417 1900 6402 6b02  k...r>|.d...d.k.
+00002bc0: 9001 7230 6415 6e02 6418 0400 7c00 5f08  ..r0d.n.d...|._.
+00002bd0: 7c09 641a 3c00 7406 7c06 8301 641b 6b05  |.d.<.t.|...d.k.
+00002be0: 9001 726e 7c06 6419 1900 6402 6b02 9001  ..rn|.d...d.k...
+00002bf0: 725e 6415 6e02 6418 0400 7c00 5f09 7c09  r^d.n.d...|._.|.
+00002c00: 641c 3c00 6e0e 6418 0400 7c00 5f09 7c09  d.<.n.d...|._.|.
+00002c10: 641c 3c00 7406 7c06 8301 641d 6b05 9001  d.<.t.|...d.k...
+00002c20: 72ac 7c06 641b 1900 6402 6b02 9001 729c  r.|.d...d.k...r.
+00002c30: 6415 6e02 6418 0400 7c00 5f0a 7c09 641e  d.n.d...|._.|.d.
+00002c40: 3c00 6e0e 6415 0400 7c00 5f0a 7c09 641e  <.n.d...|._.|.d.
+00002c50: 3c00 6e5e 7c07 641f 6b02 9001 72fc 7c08  <.n^|.d.k...r.|.
+00002c60: 640d 6b02 9001 72fc 6415 0400 7c00 5f09  d.k...r.d...|._.
+00002c70: 7c09 641c 3c00 6415 0400 7c00 5f08 7c09  |.d.<.d...|._.|.
+00002c80: 641a 3c00 6415 0400 7c00 5f0a 7c09 641e  d.<.d...|._.|.d.
+00002c90: 3c00 6e1e 7400 6a0b 6420 740c 6421 7c07  <.n.t.j.d t.d!|.
+00002ca0: 1400 7c08 1700 8301 9b00 6422 9d03 8301  ..|.......d"....
+00002cb0: 0100 7c06 7c07 7c08 7c09 6604 5300 2923  ..|.|.|.|.f.S.)#
+00002cc0: 4e7a 1249 6e20 6361 7264 5f67 6574 5f73  Nz.In card_get_s
+00002cd0: 7461 7475 7372 0100 0000 7241 0000 005a  tatusr....rA...Z
+00002ce0: 1670 726f 746f 636f 6c5f 6d61 6a6f 725f  .protocol_major_
+00002cf0: 7665 7273 696f 6e72 0c00 0000 5a16 7072  versionr....Z.pr
+00002d00: 6f74 6f63 6f6c 5f6d 696e 6f72 5f76 6572  otocol_minor_ver
+00002d10: 7369 6f6e 7223 0000 005a 1461 7070 6c65  sionr#...Z.apple
+00002d20: 745f 6d61 6a6f 725f 7665 7273 696f 6ee9  t_major_version.
+00002d30: 0300 0000 5a14 6170 706c 6574 5f6d 696e  ....Z.applet_min
+00002d40: 6f72 5f76 6572 7369 6f6e e908 0000 005a  or_version.....Z
+00002d50: 1070 726f 746f 636f 6c5f 7665 7273 696f  .protocol_versio
+00002d60: 6e72 4300 0000 da14 5049 4e30 5f72 656d  nrC.....PIN0_rem
+00002d70: 6169 6e69 6e67 5f74 7269 6573 7221 0000  aining_triesr!..
+00002d80: 00da 1450 554b 305f 7265 6d61 696e 696e  ...PUK0_remainin
+00002d90: 675f 7472 6965 7372 8700 0000 5a14 5049  g_triesr....Z.PI
+00002da0: 4e31 5f72 656d 6169 6e69 6e67 5f74 7269  N1_remaining_tri
+00002db0: 6573 e907 0000 005a 1450 554b 315f 7265  es.....Z.PUK1_re
+00002dc0: 6d61 696e 696e 675f 7472 6965 7346 5a08  maining_triesFZ.
+00002dd0: 6e65 6564 7332 4641 e909 0000 0054 e90a  needs2FA.....T..
+00002de0: 0000 0072 7900 0000 e90b 0000 0072 7a00  ...ry........rz.
+00002df0: 0000 e90c 0000 0072 5800 0000 7242 0000  .......rX...rB..
+00002e00: 007a 2a55 6e6b 6e6f 776e 2065 7272 6f72  .z*Unknown error
+00002e10: 2069 6e20 6765 745f 7374 6174 7573 2829   in get_status()
+00002e20: 2028 6572 726f 7220 636f 6465 20e9 0001   (error code ...
+00002e30: 0000 fa01 2929 0d72 2700 0000 7234 0000  ....)).r'...r4..
+00002e40: 0072 2b00 0000 da0c 4361 7264 4564 6765  .r+.....CardEdge
+00002e50: 5f43 4c41 728e 0000 0072 9b00 0000 7235  _CLAr....r....r5
+00002e60: 0000 0072 7800 0000 7279 0000 0072 7a00  ...rx...ry...rz.
+00002e70: 0000 7258 0000 0072 5400 0000 724c 0000  ..rX...rT...rL..
+00002e80: 0029 0a72 3600 0000 72a1 0000 0072 8900  .).r6...r....r..
+00002e90: 0000 72a2 0000 0072 a300 0000 729a 0000  ..r....r....r...
+00002ea0: 0072 2200 0000 725e 0000 0072 5f00 0000  .r"...r^...r_...
+00002eb0: da01 6472 3700 0000 7237 0000 0072 3800  ..dr7...r7...r8.
+00002ec0: 0000 7257 0000 0063 0100 0073 4800 0000  ..rW...c...sH...
+00002ed0: 0001 0a01 0601 0601 0401 0401 0c01 1001  ................
+00002ee0: 0401 1201 0c01 0c01 0c01 0c01 1801 0c01  ................
+00002ef0: 0c01 0c01 0c01 0c01 0e01 0e01 2001 0e01  ............ ...
+00002f00: 2001 0e01 2202 0e01 0e01 2202 1002 1401   ...".....".....
+00002f10: 0e01 0e01 1003 1e03 7a1d 4361 7264 436f  ........z.CardCo
+00002f20: 6e6e 6563 746f 722e 6361 7264 5f67 6574  nnector.card_get
+00002f30: 5f73 7461 7475 7363 0100 0000 0000 0000  _statusc........
+00002f40: 0c00 0000 1200 0000 4300 0000 73ea 0000  ........C...s...
+00002f50: 0074 006a 0164 0183 0101 0074 026a 037d  .t.j.d.....t.j.}
+00002f60: 0164 027d 0264 037d 0364 047d 047c 017c  .d.}.d.}.d.}.|.|
+00002f70: 027c 037c 0467 047d 057c 006a 047c 0583  .|.|.g.}.|.j.|..
+00002f80: 015c 037d 067d 077d 087c 0764 056b 0272  .\.}.}.}.|.d.k.r
+00002f90: ae7c 0864 036b 0272 ae7c 0664 0319 007d  .|.d.k.r.|.d...}
+00002fa0: 0979 1a74 057c 0664 0464 0085 0219 0083  .y.t.|.d.d......
+00002fb0: 016a 0664 0683 017d 0a57 0071 de04 0074  .j.d...}.W.q...t
+00002fc0: 076b 0a72 aa01 007d 0b01 007a 2474 006a  .k.r...}...z$t.j
+00002fd0: 0864 0783 0101 0074 0974 057c 0664 0464  .d.....t.t.|.d.d
+00002fe0: 0085 0219 0083 0183 017d 0a57 0059 0064  .........}.W.Y.d
+00002ff0: 0064 007d 0b7e 0b58 0071 de58 006e 307c  .d.}.~.X.q.X.n0|
+00003000: 0764 086b 0272 c47c 0864 036b 0272 c464  .d.k.r.|.d.k.r.d
+00003010: 097d 0a6e 1a74 006a 0864 0a7c 079b 0064  .}.n.t.j.d.|...d
+00003020: 0b7c 089b 009d 0483 0101 0064 0c7d 0a7c  .|.........d.}.|
+00003030: 067c 077c 087c 0a66 0453 0029 0d4e 7a11  .|.|.|.f.S.).Nz.
+00003040: 496e 2063 6172 645f 6765 745f 6c61 6265  In card_get_labe
+00003050: 6ce9 3d00 0000 7201 0000 0072 0c00 0000  l.=...r....r....
+00003060: 7241 0000 00da 0475 7466 387a 2e55 6e69  rA.....utf8z.Uni
+00003070: 636f 6465 4465 636f 6465 4572 726f 7220  codeDecodeError 
+00003080: 7768 696c 6520 6465 636f 6469 6e67 2063  while decoding c
+00003090: 6172 6420 6c61 6265 6c20 2172 7300 0000  ard label !rs...
+000030a0: 7a06 286e 6f6e 6529 7a23 4572 726f 7220  z.(none)z#Error 
+000030b0: 7768 696c 6520 7265 636f 7665 7269 6e67  while recovering
+000030c0: 2063 6172 6420 6c61 6265 6c3a 2072 2400   card label: r$.
+000030d0: 0000 7a09 2875 6e6b 6e6f 776e 2929 0a72  ..z.(unknown)).r
+000030e0: 2700 0000 7234 0000 0072 2b00 0000 72be  '...r4...r+...r.
+000030f0: 0000 0072 9b00 0000 724b 0000 00da 0664  ...r....rK.....d
+00003100: 6563 6f64 65da 1255 6e69 636f 6465 4465  ecode..UnicodeDe
+00003110: 636f 6465 4572 726f 7272 5400 0000 7276  codeErrorrT...rv
+00003120: 0000 0029 0c72 3600 0000 72a1 0000 0072  ...).r6...r....r
+00003130: 8900 0000 72a2 0000 0072 a300 0000 729a  ....r....r....r.
+00003140: 0000 0072 2200 0000 725e 0000 0072 5f00  ...r"...r^...r_.
+00003150: 0000 da0a 6c61 6265 6c5f 7369 7a65 da05  ....label_size..
+00003160: 6c61 6265 6cda 0165 7237 0000 0072 3700  label..er7...r7.
+00003170: 0000 7238 0000 00da 0e63 6172 645f 6765  ..r8.....card_ge
+00003180: 745f 6c61 6265 6c94 0100 0073 2600 0000  t_label....s&...
+00003190: 0002 0a01 0601 0401 0401 0401 0c01 1002  ................
+000031a0: 1001 0801 0201 1a01 1001 0a01 2801 1001  ............(...
+000031b0: 0602 1601 0402 7a1c 4361 7264 436f 6e6e  ......z.CardConn
+000031c0: 6563 746f 722e 6361 7264 5f67 6574 5f6c  ector.card_get_l
+000031d0: 6162 656c 6302 0000 0000 0000 000d 0000  abelc...........
+000031e0: 0005 0000 0043 0000 0073 6c00 0000 7400  .....C...sl...t.
+000031f0: 6a01 6401 8301 0100 7402 6a03 7d02 6402  j.d.....t.j.}.d.
+00003200: 7d03 6403 7d04 6403 7d05 7404 7c01 6a05  }.d.}.d.}.t.|.j.
+00003210: 6404 8301 8301 7d06 7406 7c06 8301 6701  d.....}.t.|...g.
+00003220: 7c06 1700 7d07 7406 7c07 8301 7d08 7c02  |...}.t.|...}.|.
+00003230: 7c03 7c04 7c05 7c08 6705 7c07 1700 7d09  |.|.|.|.g.|...}.
+00003240: 7c00 6a07 7c09 8301 5c03 7d0a 7d0b 7d0c  |.j.|...\.}.}.}.
+00003250: 7c0a 7c0b 7c0c 6603 5300 2905 4e7a 1149  |.|.|.f.S.).Nz.I
+00003260: 6e20 6361 7264 5f73 6574 5f6c 6162 656c  n card_set_label
+00003270: 72c0 0000 0072 0100 0000 72c1 0000 0029  r....r....r....)
+00003280: 0872 2700 0000 7234 0000 0072 2b00 0000  .r'...r4...r+...
+00003290: 72be 0000 00da 046c 6973 74da 0665 6e63  r......list..enc
+000032a0: 6f64 6572 3500 0000 729b 0000 0029 0d72  oder5...r....).r
+000032b0: 3600 0000 72c5 0000 0072 a100 0000 7289  6...r....r....r.
+000032c0: 0000 0072 a200 0000 72a3 0000 00da 0a6c  ...r....r......l
+000032d0: 6162 656c 5f6c 6973 74da 0464 6174 61da  abel_list..data.
+000032e0: 026c 6372 9a00 0000 7222 0000 0072 5e00  .lcr....r"...r^.
+000032f0: 0000 725f 0000 0072 3700 0000 7237 0000  ..r_...r7...r7..
+00003300: 0072 3800 0000 da0e 6361 7264 5f73 6574  .r8.....card_set
+00003310: 5f6c 6162 656c ad01 0000 7316 0000 0000  _label....s.....
+00003320: 010a 0106 0104 0104 0104 020e 010e 0108  ................
+00003330: 0112 0110 027a 1c43 6172 6443 6f6e 6e65  .....z.CardConne
+00003340: 6374 6f72 2e63 6172 645f 7365 745f 6c61  ctor.card_set_la
+00003350: 6265 6c63 1100 0000 0000 0000 1d00 0000  belc............
+00003360: 0800 0000 4300 0000 73ec 0100 0074 006a  ....C...s....t.j
+00003370: 0164 0183 0101 0064 0264 0364 0464 0564  .d.....d.d.d.d.d
+00003380: 0664 0764 0864 0867 087d 1174 026a 037d  .d.d.d.g.}.t.j.}
+00003390: 1274 026a 047d 1364 097d 1464 097d 157c  .t.j.}.d.}.d.}.|
+000033a0: 127c 137c 147c 1567 047d 167c 0e64 096b  .|.|.|.g.}.|.d.k
+000033b0: 0272 4c64 097d 176e 167c 0e64 0a40 0064  .rLd.}.n.|.d.@.d
+000033c0: 0a6b 0272 5e64 0b7d 176e 0464 0c7d 1764  .k.r^d.}.n.d.}.d
+000033d0: 0d74 057c 1183 0117 0074 057c 0383 0117  .t.|.....t.|....
+000033e0: 0074 057c 0783 0117 0074 057c 0483 0117  .t.|.....t.|....
+000033f0: 0074 057c 0883 0117 007c 1717 007d 187c  .t.|.....|...}.|
+00003400: 167c 1867 0137 007d 167c 1674 057c 1183  .|.g.7.}.|.t.|..
+00003410: 0167 017c 1117 0037 007d 167c 167c 017c  .g.|...7.}.|.|.|
+00003420: 0274 057c 0383 0167 037c 0317 0074 057c  .t.|...g.|...t.|
+00003430: 0483 0167 0117 007c 0417 0037 007d 167c  ...g...|...7.}.|
+00003440: 167c 057c 0674 057c 0783 0167 037c 0717  .|.|.t.|...g.|..
+00003450: 0074 057c 0883 0167 0117 007c 0817 0037  .t.|...g...|...7
+00003460: 007d 167c 167c 0964 0e3f 007c 0964 0f40  .}.|.|.d.?.|.d.@
+00003470: 007c 0a64 0e3f 007c 0a64 0f40 0067 0437  .|.d.?.|.d.@.g.7
+00003480: 007d 167c 167c 0b7c 0c7c 0d67 0337 007d  .}.|.|.|.|.g.7.}
+00003490: 167c 0e64 096b 0390 0172 787c 167c 0e64  .|.d.k...rx|.|.d
+000034a0: 0e3f 007c 0e64 0f40 0067 0237 007d 167c  .?.|.d.@.g.7.}.|
+000034b0: 167c 0f37 007d 1678 2c74 0674 0764 0e83  .|.7.}.x,t.t.d..
+000034c0: 0183 0144 005d 1c7d 197c 167c 1064 0e7c  ...D.].}.|.|.d.|
+000034d0: 1914 003f 0064 0f40 0067 0137 007d 1690  ...?.d.@.g.7.}..
+000034e0: 0171 5857 007c 006a 087c 1683 015c 037d  .qXW.|.j.|...\.}
+000034f0: 1a7d 1b7d 1c7c 1b64 106b 0290 0172 e27c  .}.}.|.d.k...r.|
+00003500: 1c64 096b 0290 0172 e27c 006a 0964 097c  .d.k...r.|.j.d.|
+00003510: 0383 0201 007c 006a 0a64 116b 0290 0172  .....|.j.d.k...r
+00003520: e27c 006a 0b7c 1a64 0974 0c85 0219 0083  .|.j.|.d.t......
+00003530: 0101 007c 006a 0d7c 1a74 0c74 0c74 0e17  ...|.j.|.t.t.t..
+00003540: 0085 0219 0083 0101 0064 127c 005f 0f7c  .........d.|._.|
+00003550: 1a7c 1b7c 1c66 0353 0029 134e 7a0d 496e  .|.|.f.S.).Nz.In
+00003560: 2063 6172 645f 7365 7475 70e9 4d00 0000   card_setup.M...
+00003570: e975 0000 00e9 7300 0000 e963 0000 00e9  .u....s....c....
+00003580: 6c00 0000 726e 0000 00e9 3000 0000 7201  l...rn....0...r.
+00003590: 0000 0069 0080 0000 e91e 0000 0072 2300  ...i.........r#.
+000035a0: 0000 728a 0000 0072 b400 0000 e9ff 0000  ..r....r........
+000035b0: 0072 4100 0000 72b1 0000 0054 2910 7227  .rA...r....T).r'
+000035c0: 0000 0072 3400 0000 722b 0000 0072 be00  ...r4...r+...r..
+000035d0: 0000 722c 0000 0072 3500 0000 da08 7265  ..r,...r5.....re
+000035e0: 7665 7273 6564 da05 7261 6e67 6572 9b00  versed..ranger..
+000035f0: 0000 da07 7365 745f 7069 6e72 8300 0000  ....set_pinr....
+00003600: da1b 7361 746f 6469 6d65 5f73 6574 5f75  ..satodime_set_u
+00003610: 6e6c 6f63 6b5f 636f 756e 7465 7272 8100  nlock_counterr..
+00003620: 0000 da1a 7361 746f 6469 6d65 5f73 6574  ....satodime_set
+00003630: 5f75 6e6c 6f63 6b5f 7365 6372 6574 727f  _unlock_secretr.
+00003640: 0000 0072 7e00 0000 291d 7236 0000 005a  ...r~...).r6...Z
+00003650: 0a70 696e 5f74 7269 6573 305a 0b75 626c  .pin_tries0Z.ubl
+00003660: 6b5f 7472 6965 7330 5a04 7069 6e30 5a05  k_tries0Z.pin0Z.
+00003670: 7562 6c6b 305a 0a70 696e 5f74 7269 6573  ublk0Z.pin_tries
+00003680: 315a 0b75 626c 6b5f 7472 6965 7331 5a04  1Z.ublk_tries1Z.
+00003690: 7069 6e31 5a05 7562 6c6b 315a 076d 656d  pin1Z.ublk1Z.mem
+000036a0: 7369 7a65 5a08 6d65 6d73 697a 6532 5a11  sizeZ.memsize2Z.
+000036b0: 6372 6561 7465 5f6f 626a 6563 745f 4143  create_object_AC
+000036c0: 4c5a 0e63 7265 6174 655f 6b65 795f 4143  LZ.create_key_AC
+000036d0: 4c5a 0e63 7265 6174 655f 7069 6e5f 4143  LZ.create_pin_AC
+000036e0: 4c5a 0c6f 7074 696f 6e5f 666c 6167 73da  LZ.option_flags.
+000036f0: 0e68 6d61 6373 6861 3136 305f 6b65 79da  .hmacsha160_key.
+00003700: 0c61 6d6f 756e 745f 6c69 6d69 7472 7d00  .amount_limitr}.
+00003710: 0000 72a1 0000 0072 8900 0000 72a2 0000  ..r....r....r...
+00003720: 0072 a300 0000 729a 0000 005a 0a6f 7074  .r....r....Z.opt
+00003730: 696f 6e73 697a 6572 cc00 0000 da01 6972  ionsizer......ir
+00003740: 2200 0000 725e 0000 0072 5f00 0000 7237  "...r^...r_...r7
+00003750: 0000 0072 3700 0000 7238 0000 00da 0a63  ...r7...r8.....c
+00003760: 6172 645f 7365 7475 70bc 0100 0073 4000  ard_setup....s@.
+00003770: 0000 0007 0a02 1401 0601 0601 0401 0401  ................
+00003780: 0c07 0801 0601 0c01 0602 0401 3002 0a01  ............0...
+00003790: 1201 2401 2401 2001 0e01 0a01 1401 0801  ..$.$. .........
+000037a0: 1201 1c03 1001 1401 0c02 0c01 1201 1601  ................
+000037b0: 0602 7a18 4361 7264 436f 6e6e 6563 746f  ..z.CardConnecto
+000037c0: 722e 6361 7264 5f73 6574 7570 6302 0000  r.card_setupc...
+000037d0: 0000 0000 000d 0000 0005 0000 0043 0000  .............C..
+000037e0: 0073 0a01 0000 7400 7c01 8301 7401 6b08  .s....t.|...t.k.
+000037f0: 721c 7402 7403 6a04 7c01 8301 8301 7d01  r.t.t.j.|.....}.
+00003800: 6e14 7400 7c01 8301 7403 6b08 7230 7402  n.t.|...t.k.r0t.
+00003810: 7c01 8301 7d01 7405 6a06 6401 8301 0100  |...}.t.j.d.....
+00003820: 7407 6a08 7d02 7407 6a09 7d03 740a 7c01  t.j.}.t.j.}.t.|.
+00003830: 8301 7d04 6402 7d05 740a 7c01 8301 7d06  ..}.d.}.t.|...}.
+00003840: 7c02 7c03 7c04 7c05 7c06 6705 7c01 1700  |.|.|.|.|.g.|...
+00003850: 7d07 7c00 6a0b 7c07 8301 5c03 7d08 7d09  }.|.j.|...\.}.}.
+00003860: 7d0a 6403 7d0b 7c09 6404 6b02 72be 7c0a  }.d.}.|.d.k.r.|.
+00003870: 6402 6b02 72be 7c00 6a0c 7c08 8301 7d0b  d.k.r.|.j.|...}.
+00003880: 7c0b 6a0d 6405 8301 6a0e 8300 7d0c 7405  |.j.d...j...}.t.
+00003890: 6a06 6406 7c0c 1700 8301 0100 6405 7c00  j.d.|.......d.|.
+000038a0: 5f0f 6e48 7c09 6407 6b02 72e2 7c0a 6408  _.nH|.d.k.r.|.d.
+000038b0: 6b02 72e2 7405 6a10 6409 8301 0100 7411  k.r.t.j.d.....t.
+000038c0: 640a 8301 8201 6e24 7c09 6407 6b02 6ff0  d.....n$|.d.k.o.
+000038d0: 7c0a 640b 6b02 9001 7206 7405 6a10 640c  |.d.k...r.t.j.d.
+000038e0: 8301 0100 7411 640c 8301 8201 7c0b 5300  ....t.d.....|.S.
+000038f0: 290d 7aed 2049 6d70 6f72 7420 6120 7365  ).z. Import a se
+00003900: 6564 2069 6e74 6f20 7468 6520 6465 7669  ed into the devi
+00003910: 6365 0a20 2020 2020 2020 200a 2020 2020  ce.        .    
+00003920: 2020 2020 5061 7261 6d65 7465 7273 3a20      Parameters: 
+00003930: 0a20 2020 2020 2020 2073 6565 6420 2873  .        seed (s
+00003940: 7472 207c 2062 7974 6573 207c 206c 6973  tr | bytes | lis
+00003950: 7429 3a20 7468 6520 7365 6564 2061 7320  t): the seed as 
+00003960: 6120 6865 785f 7374 7269 6e67 206f 7220  a hex_string or 
+00003970: 6279 7465 7320 6f72 206c 6973 7420 6f66  bytes or list of
+00003980: 2069 6e74 0a0a 2020 2020 2020 2020 5265   int..        Re
+00003990: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
+000039a0: 6175 7468 656e 7469 6b65 793a 2045 4350  authentikey: ECP
+000039b0: 7562 6b65 7920 6f62 6a65 6374 2074 6861  ubkey object tha
+000039c0: 7420 6964 656e 7469 6669 6573 2074 6865  t identifies the
+000039d0: 2020 6465 7669 6365 0a20 2020 2020 2020    device.       
+000039e0: 207a 1949 6e20 6361 7264 5f62 6970 3332   z.In card_bip32
+000039f0: 5f69 6d70 6f72 745f 7365 6564 7201 0000  _import_seedr...
+00003a00: 004e 7241 0000 0054 7a2b 5b63 6172 645f  .NrA...Tz+[card_
+00003a10: 6269 7033 325f 696d 706f 7274 5f73 6565  bip32_import_see
+00003a20: 645d 2061 7574 6865 6e74 696b 6579 5f63  d] authentikey_c
+00003a30: 6172 643d 2072 4200 0000 e917 0000 007a  ard= rB........z
+00003a40: 3b45 7272 6f72 2064 7572 696e 6720 7365  ;Error during se
+00003a50: 6372 6574 2069 6d70 6f72 743a 2063 6172  cret import: car
+00003a60: 6420 6973 2061 6c72 6561 6479 2073 6565  d is already see
+00003a70: 6465 6420 2830 7839 4331 3729 7a36 5365  ded (0x9C17)z6Se
+00003a80: 6375 7265 2069 6d70 6f72 7420 6661 696c  cure import fail
+00003a90: 6564 3a20 6361 7264 2069 7320 616c 7265  ed: card is alre
+00003aa0: 6164 7920 7365 6564 6564 2028 3078 3943  ady seeded (0x9C
+00003ab0: 3137 2921 e90f 0000 007a 3645 7272 6f72  17)!.....z6Error
+00003ac0: 2064 7572 696e 6720 7365 6372 6574 2069   during secret i
+00003ad0: 6d70 6f72 743a 2069 6e76 616c 6964 2070  mport: invalid p
+00003ae0: 6172 616d 6574 6572 2028 3078 3943 3046  arameter (0x9C0F
+00003af0: 2929 1272 2600 0000 7276 0000 0072 c800  )).r&...rv...r..
+00003b00: 0000 724b 0000 00da 0766 726f 6d68 6578  ..rK.....fromhex
+00003b10: 7227 0000 0072 3400 0000 722b 0000 0072  r'...r4...r+...r
+00003b20: be00 0000 722e 0000 0072 3500 0000 729b  ....r....r5...r.
+00003b30: 0000 00da 2163 6172 645f 6269 7033 325f  ....!card_bip32_
+00003b40: 7365 745f 6175 7468 656e 7469 6b65 795f  set_authentikey_
+00003b50: 7075 626b 6579 da14 6765 745f 7075 626c  pubkey..get_publ
+00003b60: 6963 5f6b 6579 5f62 7974 6573 724c 0000  ic_key_bytesrL..
+00003b70: 0072 7900 0000 da05 6572 726f 72da 0943  .ry.....error..C
+00003b80: 6172 6445 7272 6f72 290d 7236 0000 00da  ardError).r6....
+00003b90: 0473 6565 6472 a100 0000 7289 0000 0072  .seedr....r....r
+00003ba0: a200 0000 72a3 0000 0072 cc00 0000 729a  ....r....r....r.
+00003bb0: 0000 0072 2200 0000 725e 0000 0072 5f00  ...r"...r^...r_.
+00003bc0: 0000 72a6 0000 00da 0f61 7574 6865 6e74  ..r......authent
+00003bd0: 696b 6579 5f68 6578 7237 0000 0072 3700  ikey_hexr7...r7.
+00003be0: 0000 7238 0000 00da 1663 6172 645f 6269  ..r8.....card_bi
+00003bf0: 7033 325f 696d 706f 7274 5f73 6565 64f5  p32_import_seed.
+00003c00: 0100 0073 3200 0000 0009 0c01 1001 0c01  ...s2...........
+00003c10: 0802 0a01 0601 0601 0801 0401 0801 1203  ................
+00003c20: 1003 0401 1001 0a01 0e01 0e08 0801 1001  ................
+00003c30: 0a01 0a01 1201 0a01 0802 7a24 4361 7264  ..........z$Card
+00003c40: 436f 6e6e 6563 746f 722e 6361 7264 5f62  Connector.card_b
+00003c50: 6970 3332 5f69 6d70 6f72 745f 7365 6564  ip32_import_seed
+00003c60: 6302 0000 0000 0000 0013 0000 0005 0000  c...............
+00003c70: 0043 0000 0073 8002 0000 7400 6a01 6401  .C...s....t.j.d.
+00003c80: 8301 0100 7402 6a03 7d02 6402 7d03 6403  ....t.j.}.d.}.d.
+00003c90: 7d04 6403 7d05 7404 7405 6a06 7c01 6404  }.d.}.t.t.j.|.d.
+00003ca0: 1900 8301 8301 6405 6429 8502 1900 7d06  ......d.d)....}.
+00003cb0: 7404 7405 6a06 7c01 6407 1900 8301 8301  t.t.j.|.d.......
+00003cc0: 7d07 7404 7405 6a06 7c01 6408 1900 8301  }.t.t.j.|.d.....
+00003cd0: 8301 7d08 7404 7405 6a06 7c01 6409 1900  ..}.t.t.j.|.d...
+00003ce0: 8301 8301 7d09 7c06 7c07 1700 7407 7c08  ....}.|.|...t.|.
+00003cf0: 8301 640a 3f00 7407 7c08 8301 640b 1600  ..d.?.t.|...d...
+00003d00: 6702 1700 7c08 1700 7407 7c09 8301 6701  g...|...t.|...g.
+00003d10: 1700 7c09 1700 7d0a 7407 7c0a 8301 7d0b  ..|...}.t.|...}.
+00003d20: 7c02 7c03 7c04 7c05 7c0b 6705 7c0a 1700  |.|.|.|.|.g.|...
+00003d30: 7d0c 7c00 6a08 7c0c 8301 5c03 7d0d 7d0e  }.|.j.|...\.}.}.
+00003d40: 7d0f 7c0e 640c 6b02 72dc 7c0f 6403 6b02  }.|.d.k.r.|.d.k.
+00003d50: 72dc 9001 6e54 7c0e 640d 6b02 6fea 7c0f  r...nT|.d.k.o.|.
+00003d60: 6403 6b02 9001 7204 7400 6a09 640e 8301  d.k...r.t.j.d...
+00003d70: 0100 740a 640e 8301 8201 9001 6e2c 7c0e  ..t.d.......n,|.
+00003d80: 640f 6b02 9001 722e 7c0f 6410 6b02 9001  d.k...r.|.d.k...
+00003d90: 722e 7400 6a09 6411 8301 0100 740a 6412  r.t.j.d.....t.d.
+00003da0: 8301 8201 9001 6e02 7c0e 640f 6b02 9001  ......n.|.d.k...
+00003db0: 7256 7c0f 6413 6b02 9001 7256 7400 6a09  rV|.d.k...rVt.j.
+00003dc0: 6414 8301 0100 740a 6415 8301 8201 6eda  d.....t.d.....n.
+00003dd0: 7c0e 640f 6b02 9001 727e 7c0f 6416 6b02  |.d.k...r~|.d.k.
+00003de0: 9001 727e 7400 6a09 6417 8301 0100 740a  ..r~t.j.d.....t.
+00003df0: 6417 8301 8201 6eb2 7c0e 640f 6b02 9001  d.....n.|.d.k...
+00003e00: 72a6 7c0f 6418 6b02 9001 72a6 7400 6a09  r.|.d.k...r.t.j.
+00003e10: 6419 8301 0100 740a 641a 8301 8201 6e8a  d.....t.d.....n.
+00003e20: 7c0e 640f 6b02 9001 72ce 7c0f 641b 6b02  |.d.k...r.|.d.k.
+00003e30: 9001 72ce 7400 6a09 641c 8301 0100 740a  ..r.t.j.d.....t.
+00003e40: 641d 8301 8201 6e62 7c0e 640f 6b02 9001  d.....nb|.d.k...
+00003e50: 72f6 7c0f 641e 6b02 9001 72f6 7400 6a09  r.|.d.k...r.t.j.
+00003e60: 641f 8301 0100 740a 6420 8301 8201 6e3a  d.....t.d ....n:
+00003e70: 7400 6a09 6421 740b 640b 7c0e 1400 7c0f  t.j.d!t.d.|...|.
+00003e80: 1700 8301 9b00 6422 9d03 8301 0100 740c  ......d"......t.
+00003e90: 6423 740b 640b 7c0e 1400 7c0f 1700 8301  d#t.d.|...|.....
+00003ea0: 9b00 6422 9d03 8301 8201 7c06 6403 1900  ..d"......|.d...
+00003eb0: 7d10 7c10 6424 6b02 9002 726e 7c00 6a0d  }.|.d$k...rn|.j.
+00003ec0: 6a0e 7c0d 8301 7d11 7c11 6a0f 6425 8301  j.|...}.|.j.d%..
+00003ed0: 6a0b 8300 7d12 7400 6a01 6426 7c12 1700  j...}.t.j.d&|...
+00003ee0: 8301 0100 7c11 5300 7c10 6427 6b02 9002  ....|.S.|.d'k...
+00003ef0: 727c 6428 5300 6428 5300 292a 61aa 0200  r|d(S.d(S.)*a...
+00003f00: 0049 6d70 6f72 7420 616e 2065 6e63 7279  .Import an encry
+00003f10: 7074 6564 2073 6563 7265 7420 2842 4950  pted secret (BIP
+00003f20: 3332 206d 6173 7465 7273 6565 6420 6f72  32 masterseed or
+00003f30: 2032 4641 2073 6563 7265 7429 2065 7870   2FA secret) exp
+00003f40: 6f72 7465 6420 6672 6f6d 2061 2053 6565  orted from a See
+00003f50: 644b 6565 7065 722e 0a20 2020 2020 2020  dKeeper..       
+00003f60: 200a 2020 2020 2020 2020 5468 6520 7365   .        The se
+00003f70: 6372 6574 2069 7320 656e 6372 7970 7465  cret is encrypte
+00003f80: 6420 7573 696e 6720 6120 7368 6172 6564  d using a shared
+00003f90: 206b 6579 2067 656e 6572 6174 6564 2075   key generated u
+00003fa0: 7369 6e67 2045 4344 4820 7769 7468 2074  sing ECDH with t
+00003fb0: 6865 2032 2064 6576 6963 6573 2061 7574  he 2 devices aut
+00003fc0: 6865 6e74 696b 6579 732e 0a20 2020 2020  hentikeys..     
+00003fd0: 2020 2042 6566 6f72 6520 696d 706f 7274     Before import
+00003fe0: 2063 616e 2062 6520 646f 6e65 2c20 7468   can be done, th
+00003ff0: 6520 7477 6f20 6465 7669 6365 2073 686f  e two device sho
+00004000: 756c 6420 6265 2070 6169 7265 6420 6279  uld be paired by
+00004010: 2069 6d70 6f72 7469 6e67 2074 6865 200a   importing the .
+00004020: 2020 2020 2020 2020 5361 746f 6368 6970          Satochip
+00004030: 2d61 7574 6865 6e74 696b 6579 2069 6e20  -authentikey in 
+00004040: 7468 6520 5365 6564 4b65 6570 6572 2077  the SeedKeeper w
+00004050: 6974 6820 7365 6564 6b65 6570 6572 5f69  ith seedkeeper_i
+00004060: 6d70 6f72 745f 7365 6372 6574 2829 2c20  mport_secret(), 
+00004070: 0a20 2020 2020 2020 2061 6e64 2074 6865  .        and the
+00004080: 2053 6565 644b 6565 7065 722d 6175 7468   SeedKeeper-auth
+00004090: 656e 7469 6b65 7920 696e 2074 6865 2053  entikey in the S
+000040a0: 6174 6f63 6869 7020 7769 7468 2063 6172  atochip with car
+000040b0: 645f 696d 706f 7274 5f74 7275 7374 6564  d_import_trusted
+000040c0: 5f70 7562 6b65 7928 292e 0a20 2020 2020  _pubkey()..     
+000040d0: 2020 2020 0a20 2020 2020 2020 2050 6172      .        Par
+000040e0: 616d 6574 6572 733a 200a 2020 2020 2020  ameters: .      
+000040f0: 2020 7365 6372 6574 5f64 6963 3a20 6120    secret_dic: a 
+00004100: 6469 6374 696f 6e6e 6172 7920 7468 6174  dictionnary that
+00004110: 2064 6566 696e 6573 2074 6865 2073 6563   defines the sec
+00004120: 7265 742c 2061 7320 7265 7475 726e 6564  ret, as returned
+00004130: 2062 7920 7365 6564 6b65 6570 6572 5f65   by seedkeeper_e
+00004140: 7870 6f72 745f 7365 6372 6574 2829 0a0a  xport_secret()..
+00004150: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00004160: 200a 2020 2020 2020 2020 6175 7468 656e   .        authen
+00004170: 7469 6b65 793a 2045 4350 7562 6b65 7920  tikey: ECPubkey 
+00004180: 6f62 6a65 6374 2074 6861 7420 6964 656e  object that iden
+00004190: 7469 6669 6573 2074 6865 2020 6465 7669  tifies the  devi
+000041a0: 6365 0a20 2020 2020 2020 207a 1f49 6e20  ce.        z.In 
+000041b0: 6361 7264 5f69 6d70 6f72 745f 656e 6372  card_import_encr
+000041c0: 7970 7465 645f 7365 6372 6574 e9ac 0000  ypted_secret....
+000041d0: 0072 0100 0000 da06 6865 6164 6572 7223  .r......headerr#
+000041e0: 0000 0072 bb00 0000 da02 6976 da10 7365  ...r......iv..se
+000041f0: 6372 6574 5f65 6e63 7279 7074 6564 da04  cret_encrypted..
+00004200: 686d 6163 72b4 0000 0072 bc00 0000 7241  hmacr....r....rA
+00004210: 0000 0072 7300 0000 7a48 4572 726f 7220  ...rs...zHError 
+00004220: 6475 7269 6e67 2073 6563 7265 7420 696d  during secret im
+00004230: 706f 7274 3a20 6f70 6572 6174 696f 6e20  port: operation 
+00004240: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
+00004250: 2074 6865 2063 6172 6420 2830 7836 4430   the card (0x6D0
+00004260: 3029 7242 0000 0072 df00 0000 7a3b 4572  0)rB...r....z;Er
+00004270: 726f 7220 6475 7269 6e67 2073 6563 7265  ror during secre
+00004280: 7420 696d 706f 7274 3a20 6361 7264 2069  t import: card i
+00004290: 7320 616c 7265 6164 7920 7365 6564 6564  s already seeded
+000042a0: 2028 3078 3943 3137 297a 3653 6563 7572   (0x9C17)z6Secur
+000042b0: 6520 696d 706f 7274 2066 6169 6c65 643a  e import failed:
+000042c0: 2063 6172 6420 6973 2061 6c72 6561 6479   card is already
+000042d0: 2073 6565 6465 6420 2830 7839 4331 3729   seeded (0x9C17)
+000042e0: 21e9 1800 0000 7a3e 4572 726f 7220 6475  !.....z>Error du
+000042f0: 7269 6e67 2073 6563 7265 7420 696d 706f  ring secret impo
+00004300: 7274 3a20 6361 7264 2061 6c72 6561 6479  rt: card already
+00004310: 2072 6571 7569 7265 7320 3246 4120 2830   requires 2FA (0
+00004320: 7839 4331 3829 7a39 5365 6375 7265 2069  x9C18)z9Secure i
+00004330: 6d70 6f72 7420 6661 696c 6564 3a20 6361  mport failed: ca
+00004340: 7264 2061 6c72 6561 6479 2072 6571 7569  rd already requi
+00004350: 7265 7320 3246 4120 2830 7839 4331 3829  res 2FA (0x9C18)
+00004360: 2172 e000 0000 7a36 4572 726f 7220 6475  !r....z6Error du
+00004370: 7269 6e67 2073 6563 7265 7420 696d 706f  ring secret impo
+00004380: 7274 3a20 696e 7661 6c69 6420 7061 7261  rt: invalid para
+00004390: 6d65 7465 7220 2830 7839 4330 4629 e933  meter (0x9C0F).3
+000043a0: 0000 007a 2e45 7272 6f72 2064 7572 696e  ...z.Error durin
+000043b0: 6720 7365 6372 6574 2069 6d70 6f72 743a  g secret import:
 000043c0: 2077 726f 6e67 204d 4143 2028 3078 3943   wrong MAC (0x9C
-000043d0: 3333 2921 e934 0000 007a 3645 7272 6f72  33)!.4...z6Error
-000043e0: 2064 7572 696e 6720 7365 6372 6574 2069   during secret i
-000043f0: 6d70 6f72 743a 2077 726f 6e67 2066 696e  mport: wrong fin
-00004400: 6765 7270 7269 6e74 2028 3078 3943 3334  gerprint (0x9C34
-00004410: 297a 3153 6563 7572 6520 696d 706f 7274  )z1Secure import
-00004420: 2066 6169 6c65 643a 2077 726f 6e67 2066   failed: wrong f
-00004430: 696e 6765 7270 7269 6e74 2028 3078 3943  ingerprint (0x9C
-00004440: 3334 2921 e935 0000 007a 3545 7272 6f72  34)!.5...z5Error
-00004450: 2064 7572 696e 6720 7365 6372 6574 2069   during secret i
-00004460: 6d70 6f72 743a 206e 6f20 5472 7573 7465  mport: no Truste
-00004470: 6450 7562 6b65 7920 2830 7839 4333 3529  dPubkey (0x9C35)
-00004480: 7a2d 5365 6375 7265 2069 6d70 6f72 7420  z-Secure import 
-00004490: 6661 696c 6564 3a20 5472 7573 7465 6450  failed: TrustedP
-000044a0: 7562 6b65 7920 2830 7839 4333 3529 217a  ubkey (0x9C35)!z
-000044b0: 2745 7272 6f72 2064 7572 696e 6720 7365  'Error during se
-000044c0: 6372 6574 2069 6d70 6f72 7420 2865 7272  cret import (err
-000044d0: 6f72 2063 6f64 6520 72bb 0000 007a 3955  or code r....z9U
-000044e0: 6e65 7870 6563 7465 6420 6572 726f 7220  nexpected error 
-000044f0: 6475 7269 6e67 2073 6563 7572 6520 7365  during secure se
-00004500: 6372 6574 2069 6d70 6f72 7420 2865 7272  cret import (err
-00004510: 6f72 2063 6f64 6520 7288 0000 0054 7a12  or code r....Tz.
-00004520: 6175 7468 656e 7469 6b65 795f 6361 7264  authentikey_card
-00004530: 3d20 e9b0 0000 004e e90e 0000 0029 1072  = .....N.....).r
-00004540: 2700 0000 7234 0000 0072 2b00 0000 72bc  '...r4...r+...r.
-00004550: 0000 0072 c600 0000 724b 0000 0072 df00  ...r....rK...r..
-00004560: 0000 7235 0000 0072 9900 0000 72e2 0000  ..r5...r....r...
-00004570: 0072 e300 0000 724c 0000 00da 1355 6e65  .r....rL.....Une
-00004580: 7870 6563 7465 6453 5731 3245 7272 6f72  xpectedSW12Error
-00004590: 7276 0000 00da 1b70 6172 7365 5f62 6970  rv.....parse_bip
-000045a0: 3332 5f67 6574 5f61 7574 6865 6e74 696b  32_get_authentik
-000045b0: 6579 72e1 0000 0029 1372 3600 0000 da0a  eyr....).r6.....
-000045c0: 7365 6372 6574 5f64 6963 729f 0000 0072  secret_dicr....r
-000045d0: 8700 0000 72a0 0000 0072 a100 0000 72e8  ....r....r....r.
-000045e0: 0000 0072 e900 0000 da0b 7365 6372 6574  ...r......secret
-000045f0: 5f6c 6973 7472 eb00 0000 72c9 0000 0072  _listr....r....r
-00004600: ca00 0000 7298 0000 0072 2200 0000 725d  ....r....r"...r]
-00004610: 0000 0072 5e00 0000 da0b 7365 6372 6574  ...r^.....secret
-00004620: 5f74 7970 6572 a400 0000 72e5 0000 0072  _typer....r....r
-00004630: 3700 0000 7237 0000 0072 3800 0000 da1c  7...r7...r8.....
-00004640: 6361 7264 5f69 6d70 6f72 745f 656e 6372  card_import_encr
-00004650: 7970 7465 645f 7365 6372 6574 2302 0000  ypted_secret#...
-00004660: 735c 0000 0000 0e0a 0206 0104 0104 0104  s\..............
-00004670: 011a 0112 0112 0112 0132 0108 0112 0110  .........2......
-00004680: 0110 0104 0112 010a 010c 0114 010a 010c  ................
-00004690: 0114 010a 010a 0114 010a 010a 0114 010a  ................
-000046a0: 010a 0114 010a 010a 0114 010a 010a 021e  ................
-000046b0: 011c 0208 010a 010c 010e 010e 0104 010a  ................
-000046c0: 017a 2a43 6172 6443 6f6e 6e65 6374 6f72  .z*CardConnector
-000046d0: 2e63 6172 645f 696d 706f 7274 5f65 6e63  .card_import_enc
-000046e0: 7279 7074 6564 5f73 6563 7265 7463 0200  rypted_secretc..
-000046f0: 0000 0000 0000 0e00 0000 0500 0000 4300  ..............C.
-00004700: 0000 7324 0100 0074 006a 0164 0183 0101  ..s$...t.j.d....
-00004710: 0074 027c 0183 0174 036b 0872 2674 0474  .t.|...t.k.r&t.t
-00004720: 056a 067c 0183 0183 017d 016e 1474 027c  .j.|.....}.n.t.|
-00004730: 0183 0174 056b 0872 3a74 047c 0183 017d  ...t.k.r:t.|...}
-00004740: 0174 076a 087d 0264 027d 0364 037d 0464  .t.j.}.d.}.d.}.d
-00004750: 037d 0574 097c 0183 017d 067c 0664 046b  .}.t.|...}.|.d.k
-00004760: 0372 6a74 0a64 057c 069b 009d 0283 0182  .rjt.d.|........
-00004770: 017c 0664 063f 007c 0664 0716 0067 027c  .|.d.?.|.d...g.|
-00004780: 0117 007d 0774 097c 0783 017d 087c 027c  ...}.t.|...}.|.|
-00004790: 037c 047c 057c 0867 057c 0717 007d 097c  .|.|.|.g.|...}.|
-000047a0: 006a 0b7c 0983 015c 037d 0a7d 0b7d 0c7c  .j.|...\.}.}.}.|
-000047b0: 0b64 086b 0272 cc7c 0c64 036b 0272 cc74  .d.k.r.|.d.k.r.t
-000047c0: 006a 0c64 0983 0101 0074 0d64 0983 0182  .j.d.....t.d....
-000047d0: 016e 487c 0b64 0a6b 0272 f07c 0c64 0b6b  .nH|.d.k.r.|.d.k
-000047e0: 0272 f074 006a 0c64 0c83 0101 0074 0d64  .r.t.j.d.....t.d
-000047f0: 0d83 0182 016e 247c 0b64 0a6b 026f fe7c  .....n$|.d.k.o.|
-00004800: 0c64 0e6b 0290 0172 1474 006a 0c64 0f83  .d.k...r.t.j.d..
-00004810: 0101 0074 0d64 0f83 0182 017c 006a 0e6a  ...t.d.....|.j.j
-00004820: 0f7c 0a83 017d 0d7c 0d53 0029 1061 4901  .|...}.|.S.).aI.
-00004830: 0000 2049 6d70 6f72 7420 6120 7472 7573  .. Import a trus
-00004840: 7465 6420 6563 2070 7562 6b65 7920 696e  ted ec pubkey in
-00004850: 746f 2074 6865 2064 6576 6963 652e 2054  to the device. T
-00004860: 6869 7320 7075 626b 6579 2077 696c 6c20  his pubkey will 
-00004870: 6265 2075 7365 6420 666f 7220 7468 6520  be used for the 
-00004880: 7365 6375 7265 2069 6d70 6f72 7420 6f66  secure import of
-00004890: 2061 2073 6563 7265 740a 2020 2020 2020   a secret.      
-000048a0: 2020 0a20 2020 2020 2020 2050 6172 616d    .        Param
-000048b0: 6574 6572 733a 200a 2020 2020 2020 2020  eters: .        
-000048c0: 7075 626b 6579 5f6c 6973 743a 2074 6865  pubkey_list: the
-000048d0: 2070 7562 6b65 7920 696e 2075 6e63 6f6d   pubkey in uncom
-000048e0: 7072 6573 7365 6420 666f 726d 2028 3635  pressed form (65
-000048f0: 2062 7974 6573 2920 6173 2061 2068 6578   bytes) as a hex
-00004900: 5f73 7472 696e 6720 6f72 2062 7974 6573  _string or bytes
-00004910: 206f 7220 6c69 7374 206f 6620 696e 740a   or list of int.
-00004920: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00004930: 3a20 0a20 2020 2020 2020 2070 7562 6b65  : .        pubke
-00004940: 795f 6865 783a 2074 6865 2070 7562 6b65  y_hex: the pubke
-00004950: 7920 6173 2061 2068 6578 2073 7472 696e  y as a hex strin
-00004960: 6720 2836 352a 3220 6865 7820 6368 6172  g (65*2 hex char
-00004970: 7329 0a20 2020 2020 2020 207a 1d49 6e20  s).        z.In 
-00004980: 6361 7264 5f69 6d70 6f72 745f 7472 7573  card_import_trus
-00004990: 7465 645f 7075 626b 6579 e9aa 0000 0072  ted_pubkey.....r
-000049a0: 0100 0000 e941 0000 007a 5045 7272 6f72  .....A...zPError
-000049b0: 2064 7572 696e 6720 7472 7573 7465 6420   during trusted 
-000049c0: 7075 626b 6579 2069 6d70 6f72 743a 2077  pubkey import: w
-000049d0: 726f 6e67 2070 7562 6b65 7920 7369 7a65  rong pubkey size
-000049e0: 2c20 6578 7065 6374 6564 2036 3520 6275  , expected 65 bu
-000049f0: 7420 7265 6365 6976 6564 2072 b200 0000  t received r....
-00004a00: 72ba 0000 0072 7200 0000 7a48 4572 726f  r....rr...zHErro
-00004a10: 7220 6475 7269 6e67 2073 6563 7265 7420  r during secret 
-00004a20: 696d 706f 7274 3a20 6f70 6572 6174 696f  import: operatio
-00004a30: 6e20 6e6f 7420 7375 7070 6f72 7465 6420  n not supported 
-00004a40: 6279 2074 6865 2063 6172 6420 2830 7836  by the card (0x6
-00004a50: 4430 3029 7242 0000 0072 dd00 0000 7a3b  D00)rB...r....z;
-00004a60: 4572 726f 7220 6475 7269 6e67 2073 6563  Error during sec
-00004a70: 7265 7420 696d 706f 7274 3a20 6361 7264  ret import: card
-00004a80: 2069 7320 616c 7265 6164 7920 7365 6564   is already seed
-00004a90: 6564 2028 3078 3943 3137 297a 3653 6563  ed (0x9C17)z6Sec
-00004aa0: 7572 6520 696d 706f 7274 2066 6169 6c65  ure import faile
-00004ab0: 643a 2063 6172 6420 6973 2061 6c72 6561  d: card is alrea
-00004ac0: 6479 2073 6565 6465 6420 2830 7839 4331  dy seeded (0x9C1
-00004ad0: 3729 2172 de00 0000 7a36 4572 726f 7220  7)!r....z6Error 
-00004ae0: 6475 7269 6e67 2073 6563 7265 7420 696d  during secret im
-00004af0: 706f 7274 3a20 696e 7661 6c69 6420 7061  port: invalid pa
-00004b00: 7261 6d65 7465 7220 2830 7839 4330 4629  rameter (0x9C0F)
-00004b10: 2910 7227 0000 0072 3400 0000 7226 0000  ).r'...r4...r&..
-00004b20: 0072 7500 0000 72c6 0000 0072 4b00 0000  .ru...r....rK...
-00004b30: 72df 0000 0072 2b00 0000 72bc 0000 0072  r....r+...r....r
-00004b40: 3500 0000 da0c 5275 6e74 696d 6545 7272  5.....RuntimeErr
-00004b50: 6f72 7299 0000 0072 e200 0000 72e3 0000  orr....r....r...
-00004b60: 0072 7600 0000 da12 6765 745f 7472 7573  .rv.....get_trus
-00004b70: 7465 645f 7075 626b 6579 290e 7236 0000  ted_pubkey).r6..
-00004b80: 00da 0b70 7562 6b65 795f 6c69 7374 729f  ...pubkey_listr.
-00004b90: 0000 0072 8700 0000 72a0 0000 0072 a100  ...r....r....r..
-00004ba0: 0000 5a0b 7075 626b 6579 5f73 697a 6572  ..Z.pubkey_sizer
-00004bb0: c900 0000 72ca 0000 0072 9800 0000 7222  ....r....r....r"
-00004bc0: 0000 0072 5d00 0000 725e 0000 00da 0a70  ...r]...r^.....p
-00004bd0: 7562 6b65 795f 6865 7872 3700 0000 7237  ubkey_hexr7...r7
-00004be0: 0000 0072 3800 0000 da1a 6361 7264 5f69  ...r8.....card_i
-00004bf0: 6d70 6f72 745f 7472 7573 7465 645f 7075  mport_trusted_pu
-00004c00: 626b 6579 6302 0000 7336 0000 0000 090a  bkeyc...s6......
-00004c10: 010c 0110 010c 0108 0206 0104 0104 0104  ................
-00004c20: 0108 0108 010e 0114 0108 0112 0110 0110  ................
-00004c30: 010a 010a 0110 010a 010a 0112 010a 0108  ................
-00004c40: 020c 017a 2843 6172 6443 6f6e 6e65 6374  ...z(CardConnect
-00004c50: 6f72 2e63 6172 645f 696d 706f 7274 5f74  or.card_import_t
-00004c60: 7275 7374 6564 5f70 7562 6b65 7963 0100  rusted_pubkeyc..
-00004c70: 0000 0000 0000 0a00 0000 0400 0000 4300  ..............C.
-00004c80: 0000 7378 0000 0074 006a 0164 0183 0101  ..sx...t.j.d....
-00004c90: 0074 026a 037d 0164 027d 0264 037d 0364  .t.j.}.d.}.d.}.d
-00004ca0: 037d 047c 017c 027c 037c 0467 047d 057c  .}.|.|.|.|.g.}.|
-00004cb0: 006a 047c 0583 015c 037d 067d 077d 087c  .j.|...\.}.}.}.|
-00004cc0: 0764 046b 0272 507c 0864 056b 0272 5064  .d.k.rP|.d.k.rPd
-00004cd0: 0664 0714 0053 007c 0764 086b 0272 687c  .d...S.|.d.k.rh|
-00004ce0: 0864 036b 0272 6864 0664 0914 0053 007c  .d.k.rhd.d...S.|
-00004cf0: 006a 056a 067c 0683 017d 097c 0953 0029  .j.j.|...}.|.S.)
-00004d00: 0a7a c820 4578 706f 7274 2074 6865 2074  .z. Export the t
-00004d10: 7275 7374 6564 2065 6320 7075 626b 6579  rusted ec pubkey
-00004d20: 2066 726f 6d20 7468 6520 6465 7669 6365   from the device
-00004d30: 2e20 5468 6973 2070 7562 6b65 7920 6973  . This pubkey is
-00004d40: 2075 7365 6420 666f 7220 7468 6520 7365   used for the se
-00004d50: 6375 7265 2069 6d70 6f72 7420 6f66 2061  cure import of a
-00004d60: 2073 6563 7265 740a 2020 2020 2020 2020   secret.        
-00004d70: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00004d80: 3a20 0a20 2020 2020 2020 2070 7562 6b65  : .        pubke
-00004d90: 795f 6865 783a 2074 6865 2070 7562 6b65  y_hex: the pubke
-00004da0: 7920 6173 2061 2068 6578 2073 7472 696e  y as a hex strin
-00004db0: 6720 2836 352a 3220 6865 7820 6368 6172  g (65*2 hex char
-00004dc0: 7329 0a20 2020 2020 2020 207a 1d49 6e20  s).        z.In 
-00004dd0: 6361 7264 5f65 7870 6f72 745f 7472 7573  card_export_trus
-00004de0: 7465 645f 7075 626b 6579 e9ab 0000 0072  ted_pubkey.....r
-00004df0: 0100 0000 7242 0000 0072 ef00 0000 72f9  ....rB...r....r.
-00004e00: 0000 005a 0230 3072 7200 0000 5a02 4646  ...Z.00rr...Z.FF
-00004e10: 2907 7227 0000 0072 3400 0000 722b 0000  ).r'...r4...r+..
-00004e20: 0072 bc00 0000 7299 0000 0072 7600 0000  .r....r....rv...
-00004e30: 72fb 0000 0029 0a72 3600 0000 729f 0000  r....).r6...r...
-00004e40: 0072 8700 0000 72a0 0000 0072 a100 0000  .r....r....r....
-00004e50: 7298 0000 0072 2200 0000 725d 0000 0072  r....r"...r]...r
-00004e60: 5e00 0000 72fd 0000 0072 3700 0000 7237  ^...r....r7...r7
-00004e70: 0000 0072 3800 0000 da1a 6361 7264 5f65  ...r8.....card_e
-00004e80: 7870 6f72 745f 7472 7573 7465 645f 7075  xport_trusted_pu
-00004e90: 626b 6579 8a02 0000 731a 0000 0000 060a  bkey....s.......
-00004ea0: 0106 0104 0104 0104 010c 0110 0110 0108  ................
-00004eb0: 0110 0108 020c 017a 2843 6172 6443 6f6e  .......z(CardCon
-00004ec0: 6e65 6374 6f72 2e63 6172 645f 6578 706f  nector.card_expo
-00004ed0: 7274 5f74 7275 7374 6564 5f70 7562 6b65  rt_trusted_pubke
-00004ee0: 7963 0100 0000 0000 0000 0a00 0000 0500  yc..............
-00004ef0: 0000 4300 0000 73be 0000 0074 006a 0164  ..C...s....t.j.d
-00004f00: 0183 0101 0074 026a 037d 0164 027d 0264  .....t.j.}.d.}.d
-00004f10: 037d 0364 037d 047c 017c 027c 037c 0467  .}.d.}.|.|.|.|.g
-00004f20: 047d 057c 006a 047c 0583 015c 037d 067d  .}.|.j.|...\.}.}
-00004f30: 077d 087c 0764 046b 0272 587c 0864 036b  .}.|.d.k.rX|.d.k
-00004f40: 0272 587c 006a 056a 067c 0683 017d 097c  .rX|.j.j.|...}.|
-00004f50: 0953 007c 0764 056b 0272 807c 0864 066b  .S.|.d.k.r.|.d.k
-00004f60: 0272 8074 006a 0764 0783 0101 0074 0864  .r.t.j.d.....t.d
-00004f70: 0874 0917 0083 0182 016e 3a74 006a 0a64  .t.......n:t.j.d
-00004f80: 0974 0b64 0a7c 0714 007c 0817 0083 019b  .t.d.|...|......
-00004f90: 0064 0b9d 0383 0101 0074 0c64 0974 0b64  .d.......t.d.t.d
-00004fa0: 0a7c 0714 007c 0817 0083 019b 0064 0b9d  .|...|.......d..
-00004fb0: 0383 0182 0164 0c53 0029 0d61 3a01 0000  .....d.S.).a:...
-00004fc0: 2045 7870 6f72 7420 7468 6520 6465 7669   Export the devi
-00004fd0: 6365 2061 7574 6865 6e74 696b 6579 2e0a  ce authentikey..
-00004fe0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004ff0: 2054 6865 2061 7574 6865 6e74 696b 6579   The authentikey
-00005000: 2069 6465 6e74 6966 6965 7320 756e 6971   identifies uniq
-00005010: 7565 6c79 2074 6865 2064 6576 6963 6520  uely the device 
-00005020: 616e 6420 6973 2061 6c73 6f20 7573 6564  and is also used
-00005030: 2066 6f72 2073 6574 7469 6e67 2061 0a20   for setting a. 
-00005040: 2020 2020 2020 2073 6563 7572 6520 6368         secure ch
-00005050: 616e 6e65 6c20 7768 656e 2064 6f69 6e67  annel when doing
-00005060: 2061 2073 6563 7572 6520 696d 706f 7274   a secure import
-00005070: 2077 6974 6820 6361 7264 5f69 6d70 6f72   with card_impor
-00005080: 745f 656e 6372 7970 7465 645f 7365 6372  t_encrypted_secr
-00005090: 6574 2829 2e0a 2020 2020 2020 2020 0a20  et()..        . 
-000050a0: 2020 2020 2020 2052 6574 7572 6e73 3a20         Returns: 
-000050b0: 0a20 2020 2020 2020 2061 7574 6865 6e74  .        authent
-000050c0: 696b 6579 3a20 4543 5075 626b 6579 206f  ikey: ECPubkey o
-000050d0: 626a 6563 7420 7468 6174 2069 6465 6e74  bject that ident
-000050e0: 6966 6965 7320 7468 6520 2064 6576 6963  ifies the  devic
-000050f0: 650a 2020 2020 2020 2020 7a1a 496e 2063  e.        z.In c
-00005100: 6172 645f 6578 706f 7274 5f61 7574 6865  ard_export_authe
-00005110: 6e74 696b 6579 e9ad 0000 0072 0100 0000  ntikey.....r....
-00005120: 7241 0000 0072 4200 0000 7243 0000 007a  rA...rB...rC...z
-00005130: 4b63 6172 645f 6269 7033 325f 6765 745f  Kcard_bip32_get_
-00005140: 6175 7468 656e 7469 6b65 7928 293a 2053  authentikey(): S
-00005150: 6174 6f63 6869 7020 6973 206e 6f74 2069  atochip is not i
-00005160: 6e69 7469 616c 697a 6564 203d 3e20 5261  nitialized => Ra
-00005170: 6973 696e 6720 6572 726f 7221 7a3e 5361  ising error!z>Sa
-00005180: 746f 6368 6970 2069 7320 6e6f 7420 696e  tochip is not in
-00005190: 6974 6961 6c69 7a65 6421 2059 6f75 2073  itialized! You s
-000051a0: 686f 756c 6420 6372 6561 7465 2061 206e  hould create a n
-000051b0: 6577 2077 616c 6c65 7421 0a0a 7a37 556e  ew wallet!..z7Un
-000051c0: 6578 7065 6374 6564 2065 7272 6f72 2064  expected error d
-000051d0: 7572 696e 6720 6175 7468 656e 7469 6b65  uring authentike
-000051e0: 7920 6578 706f 7274 2028 6572 726f 7220  y export (error 
-000051f0: 636f 6465 2072 ba00 0000 72bb 0000 004e  code r....r....N
-00005200: 290d 7227 0000 0072 3400 0000 722b 0000  ).r'...r4...r+..
-00005210: 0072 bc00 0000 7299 0000 0072 7600 0000  .r....r....rv...
-00005220: 72f3 0000 0072 2800 0000 da16 556e 696e  r....r(.....Unin
-00005230: 6974 6961 6c69 7a65 6453 6565 6445 7272  itializedSeedErr
-00005240: 6f72 da0b 4d53 475f 5741 524e 494e 4772  or..MSG_WARNINGr
-00005250: 5400 0000 724c 0000 0072 f200 0000 290a  T...rL...r....).
-00005260: 7236 0000 0072 9f00 0000 7287 0000 0072  r6...r....r....r
-00005270: a000 0000 72a1 0000 0072 9800 0000 7222  ....r....r....r"
-00005280: 0000 0072 5d00 0000 725e 0000 0072 a400  ...r]...r^...r..
-00005290: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
-000052a0: 00da 1763 6172 645f 6578 706f 7274 5f61  ...card_export_a
-000052b0: 7574 6865 6e74 696b 6579 9f02 0000 731e  uthentikey....s.
-000052c0: 0000 0000 090a 0106 0104 0104 0104 010c  ................
-000052d0: 0310 0110 020c 0104 0110 010a 010e 021e  ................
-000052e0: 017a 2543 6172 6443 6f6e 6e65 6374 6f72  .z%CardConnector
-000052f0: 2e63 6172 645f 6578 706f 7274 5f61 7574  .card_export_aut
-00005300: 6865 6e74 696b 6579 6303 0000 0000 0000  hentikeyc.......
-00005310: 000d 0000 0005 0000 0043 0000 0073 d600  .........C...s..
-00005320: 0000 7400 6a01 6401 8301 0100 7402 7c01  ..t.j.d.....t.|.
-00005330: 8301 7403 6b08 7226 7404 7c01 6a05 6402  ..t.k.r&t.|.j.d.
-00005340: 8301 8301 7d01 6e14 7402 7c01 8301 7406  ....}.n.t.|...t.
-00005350: 6b08 723a 7404 7c03 8301 7d03 7402 7c02  k.r:t.|...}.t.|.
-00005360: 8301 7403 6b08 7256 7404 7406 6a07 7c02  ..t.k.rVt.t.j.|.
-00005370: 8301 8301 7d02 6e14 7402 7c02 8301 7406  ....}.n.t.|...t.
-00005380: 6b08 726a 7404 7c02 8301 7d02 7408 6a09  k.rjt.|...}.t.j.
-00005390: 7d04 6403 7d05 740a 7c01 8301 7d06 6404  }.d.}.t.|...}.d.
-000053a0: 7d07 740a 7c01 8301 740a 7c02 8301 1700  }.t.|...t.|.....
-000053b0: 7d08 7c04 7c05 7c06 7c07 7c08 6705 7c01  }.|.|.|.|.|.g.|.
-000053c0: 1700 7c02 1700 7d09 7c00 6a0b 7c09 8301  ..|...}.|.j.|...
-000053d0: 5c03 7d0a 7d0b 7d0c 7c0b 6405 6b02 72cc  \.}.}.}.|.d.k.r.
-000053e0: 7c0c 6404 6b02 72cc 6406 7c00 5f0c 7c0a  |.d.k.r.d.|._.|.
-000053f0: 7c0b 7c0c 6603 5300 2907 6126 0100 0020  |.|.f.S.).a&... 
-00005400: 5265 7365 7420 7468 6520 7365 6564 0a20  Reset the seed. 
-00005410: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00005420: 5061 7261 6d65 7465 7273 3a20 0a20 2020  Parameters: .   
-00005430: 2020 2020 2070 696e 2020 2868 6578 2d73       pin  (hex-s
-00005440: 7472 696e 6720 7c20 6279 7465 7320 7c20  tring | bytes | 
-00005450: 6c69 7374 293a 2074 6865 2070 696e 2072  list): the pin r
-00005460: 6571 7569 7265 6420 746f 2075 6e6c 6f63  equired to unloc
-00005470: 6b20 7468 6520 6465 7669 6365 0a20 2020  k the device.   
-00005480: 2020 2020 2068 6d61 6320 2868 6578 2d73       hmac (hex-s
-00005490: 7472 696e 6720 7c20 6279 7465 7320 7c20  tring | bytes | 
-000054a0: 6c69 7374 293a 2074 6865 2032 302d 6279  list): the 20-by
-000054b0: 7465 2063 6f64 6520 7265 7175 6972 6564  te code required
-000054c0: 2069 6620 3246 4120 6973 2065 6e61 626c   if 2FA is enabl
-000054d0: 6564 0a20 2020 2020 2020 200a 2020 2020  ed.        .    
-000054e0: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
-000054f0: 2020 2020 2020 2872 6573 706f 6e73 652c        (response,
-00005500: 2073 7731 2c20 7377 3229 3a20 286c 6973   sw1, sw2): (lis
-00005510: 742c 2069 6e74 2c20 696e 7429 0a20 2020  t, int, int).   
-00005520: 2020 2020 207a 1249 6e20 6361 7264 5f72       z.In card_r
-00005530: 6573 6574 5f73 6565 647a 0575 7466 2d38  eset_seedz.utf-8
-00005540: e977 0000 0072 0100 0000 7241 0000 0046  .w...r....rA...F
-00005550: 290d 7227 0000 0072 3400 0000 7226 0000  ).r'...r4...r&..
-00005560: 0072 7500 0000 72c6 0000 0072 c700 0000  .ru...r....r....
-00005570: 724b 0000 0072 df00 0000 722b 0000 0072  rK...r....r+...r
-00005580: bc00 0000 7235 0000 0072 9900 0000 7278  ....r5...r....rx
-00005590: 0000 0029 0d72 3600 0000 727c 0000 0072  ...).r6...r|...r
-000055a0: eb00 0000 72e4 0000 0072 9f00 0000 7287  ....r....r....r.
-000055b0: 0000 0072 a000 0000 72a1 0000 0072 ca00  ...r....r....r..
-000055c0: 0000 7298 0000 0072 2200 0000 725d 0000  ..r....r"...r]..
-000055d0: 0072 5e00 0000 7237 0000 0072 3700 0000  .r^...r7...r7...
-000055e0: 7238 0000 00da 0f63 6172 645f 7265 7365  r8.....card_rese
-000055f0: 745f 7365 6564 bd02 0000 7326 0000 0000  t_seed....s&....
-00005600: 0a0a 010c 0110 010c 0108 020c 0110 010c  ................
-00005610: 0108 0206 0104 0108 0104 0110 0116 0210  ................
-00005620: 0110 0106 017a 1d43 6172 6443 6f6e 6e65  .....z.CardConne
-00005630: 6374 6f72 2e63 6172 645f 7265 7365 745f  ctor.card_reset_
-00005640: 7365 6564 6301 0000 0000 0000 000a 0000  seedc...........
-00005650: 0004 0000 0043 0000 0073 ae00 0000 7400  .....C...s....t.
-00005660: 6a01 6401 8301 0100 7402 6a03 7d01 7402  j.d.....t.j.}.t.
-00005670: 6a04 7d02 6402 7d03 6402 7d04 7c01 7c02  j.}.d.}.d.}.|.|.
-00005680: 7c03 7c04 6704 7d05 7c00 6a05 7c05 8301  |.|.g.}.|.j.|...
-00005690: 5c03 7d06 7d07 7d08 7c07 6403 6b02 7260  \.}.}.}.|.d.k.r`
-000056a0: 7c08 6404 6b02 7260 7400 6a06 6405 8301  |.d.k.r`t.j.d...
-000056b0: 0100 7407 6406 7408 1700 8301 8201 7c07  ..t.d.t.......|.
-000056c0: 6403 6b02 7286 7c08 6407 6b02 7286 7400  d.k.r.|.d.k.r.t.
-000056d0: 6a06 6408 8301 0100 7407 6409 7408 1700  j.d.....t.d.t...
-000056e0: 8301 8201 640a 7d09 7c07 640b 6b02 72aa  ....d.}.|.d.k.r.
-000056f0: 7c08 6402 6b02 72aa 7c00 6a09 7c06 8301  |.d.k.r.|.j.|...
-00005700: 7d09 640c 7c00 5f0a 7c09 5300 290d 7aea  }.d.|._.|.S.).z.
-00005710: 2052 6574 7572 6e20 7468 6520 6175 7468   Return the auth
-00005720: 656e 7469 6b65 7920 2020 2020 200a 2020  entikey      .  
-00005730: 2020 2020 2020 0a20 2020 2020 2020 2043        .        C
-00005740: 6f6d 7061 7265 6420 746f 2063 6172 645f  ompared to card_
-00005750: 6578 706f 7274 5f61 7574 6865 6e74 696b  export_authentik
-00005760: 6579 2829 2c20 7468 6973 206d 6574 686f  ey(), this metho
-00005770: 6420 7261 6973 6520 556e 696e 6974 6961  d raise Uninitia
-00005780: 6c69 7a65 6453 6565 6445 7272 6f72 2069  lizedSeedError i
-00005790: 6620 6e6f 2073 6565 6420 6973 2063 6f6e  f no seed is con
-000057a0: 6669 6775 7265 6420 696e 2074 6865 2064  figured in the d
-000057b0: 6576 6963 650a 2020 2020 2020 2020 0a20  evice.        . 
-000057c0: 2020 2020 2020 2052 6574 7572 6e73 3a20         Returns: 
-000057d0: 0a20 2020 2020 2020 2061 7574 6865 6e74  .        authent
-000057e0: 696b 6579 3a20 616e 2045 4350 7562 6b65  ikey: an ECPubke
-000057f0: 790a 2020 2020 2020 2020 7a1d 496e 2063  y.        z.In c
-00005800: 6172 645f 6269 7033 325f 6765 745f 6175  ard_bip32_get_au
-00005810: 7468 656e 7469 6b65 7972 0100 0000 7242  thentikeyr....rB
-00005820: 0000 00e9 1400 0000 7a47 6361 7264 5f62  ........zGcard_b
-00005830: 6970 3332 5f67 6574 5f61 7574 6865 6e74  ip32_get_authent
-00005840: 696b 6579 2829 3a20 5365 6564 2069 7320  ikey(): Seed is 
-00005850: 6e6f 7420 696e 6974 6961 6c69 7a65 6420  not initialized 
-00005860: 3d3e 2052 6169 7369 6e67 2065 7272 6f72  => Raising error
-00005870: 217a 2453 6174 6f63 6869 7020 7365 6564  !z$Satochip seed
-00005880: 2069 7320 6e6f 7420 696e 6974 6961 6c69   is not initiali
-00005890: 7a65 6421 0a0a 2072 4300 0000 7a4b 6361  zed!.. rC...zKca
-000058a0: 7264 5f62 6970 3332 5f67 6574 5f61 7574  rd_bip32_get_aut
-000058b0: 6865 6e74 696b 6579 2829 3a20 5361 746f  hentikey(): Sato
-000058c0: 6368 6970 2069 7320 6e6f 7420 696e 6974  chip is not init
-000058d0: 6961 6c69 7a65 6420 3d3e 2052 6169 7369  ialized => Raisi
-000058e0: 6e67 2065 7272 6f72 217a 3e53 6174 6f63  ng error!z>Satoc
-000058f0: 6869 7020 6973 206e 6f74 2069 6e69 7469  hip is not initi
-00005900: 616c 697a 6564 2120 596f 7520 7368 6f75  alized! You shou
-00005910: 6c64 2063 7265 6174 6520 6120 6e65 7720  ld create a new 
-00005920: 7761 6c6c 6574 210a 0a4e 7241 0000 0054  wallet!..NrA...T
-00005930: 290b 7227 0000 0072 3400 0000 722b 0000  ).r'...r4...r+..
-00005940: 0072 bc00 0000 5a19 494e 535f 4249 5033  .r....Z.INS_BIP3
-00005950: 325f 4745 545f 4155 5448 454e 5449 4b45  2_GET_AUTHENTIKE
-00005960: 5972 9900 0000 7228 0000 0072 0201 0000  Yr....r(...r....
-00005970: 7203 0100 0072 e000 0000 7278 0000 0029  r....r....rx...)
-00005980: 0a72 3600 0000 729f 0000 0072 8700 0000  .r6...r....r....
-00005990: 72a0 0000 0072 a100 0000 7298 0000 0072  r....r....r....r
-000059a0: 2200 0000 725d 0000 0072 5e00 0000 72a4  "...r]...r^...r.
-000059b0: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
-000059c0: 0000 da1a 6361 7264 5f62 6970 3332 5f67  ....card_bip32_g
-000059d0: 6574 5f61 7574 6865 6e74 696b 6579 de02  et_authentikey..
-000059e0: 0000 7324 0000 0000 080a 0106 0106 0104  ..s$............
-000059f0: 0104 010c 0310 0110 010a 010c 0110 010a  ................
-00005a00: 010c 0204 0110 010a 0106 017a 2843 6172  ...........z(Car
-00005a10: 6443 6f6e 6e65 6374 6f72 2e63 6172 645f  dConnector.card_
-00005a20: 6269 7033 325f 6765 745f 6175 7468 656e  bip32_get_authen
-00005a30: 7469 6b65 7963 0200 0000 0000 0000 0d00  tikeyc..........
-00005a40: 0000 0500 0000 4300 0000 7396 0000 0074  ......C...s....t
-00005a50: 006a 0164 0183 0101 0074 026a 037d 0264  .j.d.....t.j.}.d
-00005a60: 027d 0364 037d 0464 037d 057c 006a 046a  .}.d.}.d.}.|.j.j
-00005a70: 057c 0183 017d 067c 0672 927c 066a 0664  .|...}.|.r.|.j.d
-00005a80: 0464 058d 017d 0774 077c 0764 0664 0785  .d...}.t.|.d.d..
-00005a90: 0219 0083 017d 077c 0174 087c 0783 0164  .....}.|.t.|...d
-00005aa0: 0840 0074 087c 0783 0164 0940 0067 0217  .@.t.|...d.@.g..
-00005ab0: 007c 0717 007d 0874 087c 0883 017d 097c  .|...}.t.|...}.|
-00005ac0: 027c 037c 047c 057c 0967 057c 0817 007d  .|.|.|.|.g.|...}
-00005ad0: 0a7c 006a 097c 0a83 015c 037d 017d 0b7d  .|.j.|...\.}.}.}
-00005ae0: 0c7c 0653 0029 0a7a 9820 416c 6c6f 7773  .|.S.).z. Allows
-00005af0: 2074 6f20 636f 6d70 7574 6520 636f 6f72   to compute coor
-00005b00: 6479 206f 6620 6175 7468 656e 7469 6b65  dy of authentike
-00005b10: 7920 6578 7465 726e 616c 6c79 2074 6f20  y externally to 
-00005b20: 6f70 7469 6d69 7a65 2063 6f6d 7075 7461  optimize computa
-00005b30: 7469 6f6e 2074 696d 652d 6f75 740a 2020  tion time-out.  
-00005b40: 2020 2020 2020 636f 6f72 6479 2076 616c        coordy val
-00005b50: 7565 2069 7320 7665 7269 6669 6564 2062  ue is verified b
-00005b60: 7920 7468 6520 6368 6970 2062 6566 6f72  y the chip befor
-00005b70: 6520 6265 696e 6720 6163 6365 7074 6564  e being accepted
-00005b80: 207a 2449 6e20 6361 7264 5f62 6970 3332   z$In card_bip32
-00005b90: 5f73 6574 5f61 7574 6865 6e74 696b 6579  _set_authentikey
-00005ba0: 5f70 7562 6b65 7972 cd00 0000 7201 0000  _pubkeyr....r...
-00005bb0: 0046 2901 da0a 636f 6d70 7265 7373 6564  .F)...compressed
-00005bc0: e921 0000 004e 6900 ff00 0072 d300 0000  .!...Ni....r....
-00005bd0: 290a 7227 0000 0072 3400 0000 722b 0000  ).r'...r4...r+..
-00005be0: 0072 bc00 0000 7276 0000 0072 f300 0000  .r....rv...r....
-00005bf0: 72e1 0000 0072 c600 0000 7235 0000 0072  r....r....r5...r
-00005c00: 9900 0000 290d 7236 0000 0072 2200 0000  ....).r6...r"...
-00005c10: 729f 0000 0072 8700 0000 72a0 0000 0072  r....r....r....r
-00005c20: a100 0000 72a4 0000 00da 0663 6f6f 7264  ....r......coord
-00005c30: 7972 c900 0000 72ca 0000 0072 9800 0000  yr....r....r....
-00005c40: 725d 0000 0072 5e00 0000 7237 0000 0072  r]...r^...r7...r
-00005c50: 3700 0000 7238 0000 0072 e000 0000 fc02  7...r8...r......
-00005c60: 0000 731c 0000 0000 030a 0106 0104 0104  ..s.............
-00005c70: 0104 020c 0104 010c 0110 0120 0108 0112  ........... ....
-00005c80: 0110 017a 2f43 6172 6443 6f6e 6e65 6374  ...z/CardConnect
-00005c90: 6f72 2e63 6172 645f 6269 7033 325f 7365  or.card_bip32_se
-00005ca0: 745f 6175 7468 656e 7469 6b65 795f 7075  t_authentikey_pu
-00005cb0: 626b 6579 6302 0000 0000 0000 0016 0000  bkeyc...........
-00005cc0: 0006 0000 0043 0000 0073 d601 0000 7400  .....C...s....t.
-00005cd0: 7c01 8301 7401 6b02 721c 7c00 6a02 6a03  |...t.k.r.|.j.j.
-00005ce0: 7c01 8301 5c02 7d02 7d01 7404 6a05 6401  |...\.}.}.t.j.d.
-00005cf0: 8301 0100 7406 6a07 7d03 7406 6a08 7d04  ....t.j.}.t.j.}.
-00005d00: 7409 7c01 8301 6402 1a00 7d05 6403 7d06  t.|...d...}.d.}.
-00005d10: 7409 7c01 8301 7d07 7c03 7c04 7c05 7c06  t.|...}.|.|.|.|.
-00005d20: 7c07 6705 7d08 7c08 7c01 3700 7d08 7c00  |.g.}.|.|.7.}.|.
-00005d30: 6a02 6a0a 6404 6b08 7274 7c00 6a0b 8300  j.j.d.k.rt|.j...
-00005d40: 0100 9001 785a 7c00 6a0c 7c08 8301 5c03  ....xZ|.j.|...\.
-00005d50: 7d09 7d0a 7d0b 7c0a 6405 6b02 72d2 7c0b  }.}.}.|.d.k.r.|.
-00005d60: 6406 6b02 72d2 7404 6a0d 6407 8301 0100  d.k.r.t.j.d.....
-00005d70: 7c08 6408 1900 6409 4100 7c08 6408 3c00  |.d...d.A.|.d.<.
-00005d80: 7c00 6a0c 7c08 8301 5c03 7d09 7d0a 7d0b  |.j.|...\.}.}.}.
-00005d90: 7c08 6408 1900 640a 4000 7c08 6408 3c00  |.d...d.@.|.d.<.
-00005da0: 7c0a 640b 6b03 73e4 7c0b 640c 6b03 9001  |.d.k.s.|.d.k...
-00005db0: 7202 740e 640d 740f 640e 7c0a 1400 7c0b  r.t.d.t.d.|...|.
-00005dc0: 1700 8301 9b00 640f 9d03 8301 8201 7178  ......d.......qx
-00005dd0: 7c09 6410 1900 6409 4000 6409 6b02 9001  |.d...d.@.d.k...
-00005de0: 72b6 7404 6a0d 6411 8301 0100 7c00 6a02  r.t.j.d.....|.j.
-00005df0: 6a10 7c09 8301 5c02 7d0c 7d0d 7c0c 6a11  j.|...\.}.}.|.j.
-00005e00: 6412 6413 8d01 7d0e 7412 7c0e 6414 6404  d.d...}.t.|.d.d.
-00005e10: 8502 1900 8301 7d0e 7c00 6a02 6a0a 6a11  ......}.|.j.j.j.
-00005e20: 6412 6413 8d01 7d0f 7412 7c0f 6414 6404  d.d...}.t.|.d.d.
-00005e30: 8502 1900 8301 7d0f 7c09 7409 7c0e 8301  ......}.|.t.|...
-00005e40: 6415 4000 7409 7c0e 8301 6416 4000 6702  d.@.t.|...d.@.g.
-00005e50: 1700 7c0e 1700 7d10 7c03 6417 640c 640c  ..|...}.|.d.d.d.
-00005e60: 7409 7c10 8301 6705 7d11 7c11 7c10 1700  t.|...g.}.|.|...
-00005e70: 7d11 7c00 6a0c 7c11 8301 5c03 7d12 7d13  }.|.j.|...\.}.}.
-00005e80: 7d14 7178 7c00 6a02 6a10 7c09 8301 5c02  }.qx|.j.j.|...\.
-00005e90: 7d15 7d0d 7c15 7c0d 6602 5300 7178 5700  }.}.|.|.f.S.qxW.
-00005ea0: 6404 5300 2918 6119 0100 0020 4765 7420  d.S.).a.... Get 
-00005eb0: 7468 6520 4249 5033 3220 6578 7465 6e64  the BIP32 extend
-00005ec0: 6564 206b 6579 2066 6f72 2067 6976 656e  ed key for given
-00005ed0: 2070 6174 680a 2020 2020 2020 2020 0a20   path.        . 
-00005ee0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00005ef0: 733a 200a 2020 2020 2020 2020 7061 7468  s: .        path
-00005f00: 2028 7374 7220 7c20 6279 7465 7329 3a20   (str | bytes): 
-00005f10: 7468 6520 7061 7468 3b20 6966 2067 6976  the path; if giv
-00005f20: 656e 2061 7320 6120 7374 7269 6e67 2c20  en as a string, 
-00005f30: 6974 2077 696c 6c20 6265 2063 6f6e 7665  it will be conve
-00005f40: 7274 6564 2074 6f20 6279 7465 7320 2834  rted to bytes (4
-00005f50: 2062 7974 6573 2066 6f72 2065 6163 6820   bytes for each 
-00005f60: 7061 7468 2069 6e64 6578 290a 0a20 2020  path index)..   
-00005f70: 2020 2020 2052 6574 7572 6e73 3a20 0a20       Returns: . 
-00005f80: 2020 2020 2020 2070 7562 6b65 793a 2045         pubkey: E
-00005f90: 4350 7562 6b65 7920 6f62 6a65 6374 0a20  CPubkey object. 
-00005fa0: 2020 2020 2020 2063 6861 696e 636f 6465         chaincode
-00005fb0: 3a20 6279 7465 6172 7261 790a 2020 2020  : bytearray.    
-00005fc0: 2020 2020 7a1d 496e 2063 6172 645f 6269      z.In card_bi
-00005fd0: 7033 325f 6765 745f 6578 7465 6e64 6564  p32_get_extended
-00005fe0: 6b65 7972 4300 0000 e940 0000 004e 7242  keyrC....@...NrB
-00005ff0: 0000 0072 0c00 0000 7a2c 5b63 6172 645f  ...r....z,[card_
-00006000: 6269 7033 325f 6765 745f 6578 7465 6e64  bip32_get_extend
-00006010: 6564 6b65 795d 2052 6573 6574 206d 656d  edkey] Reset mem
-00006020: 6f72 792e 2e2e 72b1 0000 0072 9b00 0000  ory...r....r....
-00006030: 729e 0000 0072 4100 0000 7201 0000 007a  r....rA...r....z
-00006040: 1e55 6e65 7870 6563 7465 6420 6572 726f  .Unexpected erro
-00006050: 7220 2028 6572 726f 7220 636f 6465 2072  r  (error code r
-00006060: ba00 0000 72bb 0000 00e9 2000 0000 7a3d  ....r..... ...z=
-00006070: 5b63 6172 645f 6269 7033 325f 6765 745f  [card_bip32_get_
-00006080: 6578 7465 6e64 6564 6b65 795d 2043 6869  extendedkey] Chi
-00006090: 6c64 2044 6572 6976 6174 696f 6e20 6f70  ld Derivation op
-000060a0: 7469 6d69 7a61 7469 6f6e 2e2e 2e46 2901  timization...F).
-000060b0: 7209 0100 0072 0a01 0000 6900 ff00 0072  r....r....i....r
-000060c0: d300 0000 7267 0000 0029 1372 2600 0000  ....rg...).r&...
-000060d0: 7275 0000 0072 7600 0000 da0f 6269 7033  ru...rv.....bip3
-000060e0: 3270 6174 6832 6279 7465 7372 2700 0000  2path2bytesr'...
-000060f0: 7234 0000 0072 2b00 0000 72bc 0000 005a  r4...r+...r....Z
-00006100: 1a49 4e53 5f42 4950 3332 5f47 4554 5f45  .INS_BIP32_GET_E
-00006110: 5854 454e 4445 445f 4b45 5972 3500 0000  XTENDED_KEYr5...
-00006120: 72a4 0000 0072 0801 0000 7299 0000 0072  r....r....r....r
-00006130: 2800 0000 72f2 0000 0072 4c00 0000 5a1b  (...r....rL...Z.
-00006140: 7061 7273 655f 6269 7033 325f 6765 745f  parse_bip32_get_
-00006150: 6578 7465 6e64 6564 6b65 7972 e100 0000  extendedkeyr....
-00006160: 72c6 0000 0029 1672 3600 0000 da04 7061  r....).r6.....pa
-00006170: 7468 da05 6465 7074 6872 9f00 0000 7287  th..depthr....r.
-00006180: 0000 0072 a000 0000 72a1 0000 0072 ca00  ...r....r....r..
-00006190: 0000 7298 0000 0072 2200 0000 725d 0000  ..r....r"...r]..
-000061a0: 0072 5e00 0000 da06 7075 626b 6579 5a09  .r^.....pubkeyZ.
-000061b0: 6368 6169 6e63 6f64 6572 0b01 0000 5a0a  chaincoder....Z.
-000061c0: 6175 7468 636f 6f72 6479 72c9 0000 005a  authcoordyr....Z
-000061d0: 0861 7064 755f 6f70 745a 0c72 6573 706f  .apdu_optZ.respo
-000061e0: 6e73 655f 6f70 745a 0773 7731 5f6f 7074  nse_optZ.sw1_opt
-000061f0: 5a07 7377 325f 6f70 74da 036b 6579 7237  Z.sw2_opt..keyr7
-00006200: 0000 0072 3700 0000 7238 0000 00da 1a63  ...r7...r8.....c
-00006210: 6172 645f 6269 7033 325f 6765 745f 6578  ard_bip32_get_ex
-00006220: 7465 6e64 6564 6b65 790f 0300 0073 4400  tendedkey....sD.
-00006230: 0000 000a 0c01 1002 0a01 0601 0601 0c01  ................
-00006240: 0401 0801 0e01 0802 0c01 0803 0401 1004  ................
-00006250: 1001 0a01 1001 1001 1002 1201 1e02 1201  ................
-00006260: 0a01 1001 0c01 1001 1001 1001 2001 1201  ............ ...
-00006270: 0801 1203 1001 7a28 4361 7264 436f 6e6e  ......z(CardConn
-00006280: 6563 746f 722e 6361 7264 5f62 6970 3332  ector.card_bip32
-00006290: 5f67 6574 5f65 7874 656e 6465 646b 6579  _get_extendedkey
-000062a0: 6304 0000 0000 0000 000e 0000 0005 0000  c...............
-000062b0: 0043 0000 0073 2001 0000 7c02 7400 6b06  .C...s ...|.t.k.
-000062c0: 730c 7401 8201 7402 6a03 6401 7404 7c01  s.t...t.j.d.t.|.
-000062d0: 8301 9b00 9d02 8301 0100 7405 7c01 8301  ..........t.|...
-000062e0: 7404 6b02 723c 7c00 6a06 6a07 7c01 8301  t.k.r<|.j.j.|...
-000062f0: 5c02 7d04 7d05 7c00 6a08 7c05 8301 5c02  \.}.}.|.j.|...\.
-00006300: 7d06 7d07 7c04 6402 6b02 7274 7409 6402  }.}.|.d.k.rtt.d.
-00006310: 6402 6402 6402 6704 8301 7d08 7409 6402  d.d.d.g...}.t.d.
-00006320: 6402 6402 6402 6704 8301 7d09 6e3a 7c00  d.d.d.g...}.n:|.
-00006330: 6a08 7c05 6402 6409 8502 1900 8301 5c02  j.|.d.d.......\.
-00006340: 7d0a 7d0b 740a 7c0a 6a0b 6404 6405 8d01  }.}.t.|.j.d.d...
-00006350: 8301 6402 6403 8502 1900 7d08 7c05 640a  ..d.d.....}.|.d.
-00006360: 6406 8502 1900 7d09 7c03 72ba 740c 7c02  d.....}.|.r.t.|.
-00006370: 1900 6e06 740d 7c02 1900 7d0c 7409 6a0e  ..n.t.|...}.t.j.
-00006380: 7c0c 8301 7409 7c04 6701 8301 1700 7c08  |...t.|.g.....|.
-00006390: 1700 7c09 1700 7c07 1700 7c06 6a0b 6404  ..|...|...|.j.d.
-000063a0: 6405 8d01 1700 7d0d 740f 7c0d 8301 6407  d.....}.t.|...d.
-000063b0: 6b02 9001 7300 7401 8201 7410 7c0d 8301  k...s.t...t.|...
-000063c0: 7d0d 7402 6a03 6408 7404 7c0d 8301 9b00  }.t.j.d.t.|.....
-000063d0: 9d02 8301 0100 7c0d 5300 290b 61b1 0100  ......|.S.).a...
-000063e0: 0020 4765 7420 7468 6520 4249 5033 3220  . Get the BIP32 
-000063f0: 7870 7562 2066 6f72 2067 6976 656e 2070  xpub for given p
-00006400: 6174 682e 0a20 2020 2020 2020 200a 2020  ath..        .  
-00006410: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00006420: 3a20 0a20 2020 2020 2020 2070 6174 6820  : .        path 
-00006430: 2873 7472 207c 2062 7974 6573 293a 2074  (str | bytes): t
-00006440: 6865 2070 6174 683b 2069 6620 6769 7665  he path; if give
-00006450: 6e20 6173 2061 2073 7472 696e 672c 2069  n as a string, i
-00006460: 7420 7769 6c6c 2062 6520 636f 6e76 6572  t will be conver
-00006470: 7465 6420 746f 2062 7974 6573 2028 3420  ted to bytes (4 
-00006480: 6279 7465 7320 666f 7220 6561 6368 2070  bytes for each p
-00006490: 6174 6820 696e 6465 7829 0a20 2020 2020  ath index).     
-000064a0: 2020 2078 7479 7065 2028 7374 7229 3a20     xtype (str): 
-000064b0: 7468 6520 7479 7065 206f 6620 7472 616e  the type of tran
-000064c0: 7361 6374 696f 6e20 7375 6368 2061 7320  saction such as 
-000064d0: 2027 7374 616e 6461 7264 272c 2027 7032   'standard', 'p2
-000064e0: 7770 6b68 2d70 3273 6827 2c20 2770 3277  wpkh-p2sh', 'p2w
-000064f0: 706b 6827 2c20 2770 3277 7368 2d70 3273  pkh', 'p2wsh-p2s
-00006500: 6827 2c20 2770 3277 7368 270a 2020 2020  h', 'p2wsh'.    
-00006510: 2020 2020 6973 5f6d 6169 6e6e 6574 2028      is_mainnet (
-00006520: 626f 6f6c 293a 2069 7320 6d61 696e 6e65  bool): is mainne
-00006530: 7420 6f72 2074 6573 746e 6574 200a 2020  t or testnet .  
-00006540: 2020 2020 2020 0a20 2020 2020 2020 2052        .        R
-00006550: 6574 7572 6e73 3a20 0a20 2020 2020 2020  eturns: .       
-00006560: 2078 7075 6220 2873 7472 293a 2074 6865   xpub (str): the
-00006570: 2063 6f72 7265 7370 6f6e 6469 6e67 2078   corresponding x
-00006580: 7075 6220 7661 6c75 650a 2020 2020 2020  pub value.      
-00006590: 2020 7a1c 6361 7264 5f62 6970 3332 5f67    z.card_bip32_g
-000065a0: 6574 5f78 7075 6228 293a 2070 6174 683d  et_xpub(): path=
-000065b0: 7201 0000 0072 4300 0000 5429 0172 0901  r....rC...T).r..
-000065c0: 0000 4ee9 4e00 0000 7a1c 6361 7264 5f62  ..N.N...z.card_b
-000065d0: 6970 3332 5f67 6574 5f78 7075 6228 293a  ip32_get_xpub():
-000065e0: 2078 7075 623d e9fc ffff ff72 1501 0000   xpub=.....r....
-000065f0: 2911 da10 5355 5050 4f52 5445 445f 5854  )...SUPPORTED_XT
-00006600: 5950 4553 da0e 4173 7365 7274 696f 6e45  YPES..AssertionE
-00006610: 7272 6f72 7227 0000 0072 2800 0000 7275  rrorr'...r(...ru
-00006620: 0000 0072 2600 0000 7276 0000 0072 0e01  ...r&...rv...r..
-00006630: 0000 7213 0100 0072 4b00 0000 7215 0000  ..r....rK...r...
-00006640: 0072 e100 0000 da14 5850 5542 5f48 4541  .r......XPUB_HEA
-00006650: 4445 5253 5f4d 4149 4e4e 4554 da14 5850  DERS_MAINNET..XP
-00006660: 5542 5f48 4541 4445 5253 5f54 4553 544e  UB_HEADERS_TESTN
-00006670: 4554 72df 0000 0072 3500 0000 7216 0000  ETr....r5...r...
-00006680: 0029 0e72 3600 0000 720f 0100 005a 0578  .).r6...r....Z.x
-00006690: 7479 7065 5a0a 6973 5f6d 6169 6e6e 6574  typeZ.is_mainnet
-000066a0: 7210 0100 005a 0862 7974 6570 6174 685a  r....Z.bytepathZ
-000066b0: 0863 6869 6c64 6b65 795a 0e63 6869 6c64  .childkeyZ.child
-000066c0: 6368 6169 6e63 6f64 65da 0b66 696e 6765  chaincode..finge
-000066d0: 7270 7269 6e74 5a0c 6368 696c 645f 6e75  rprintZ.child_nu
-000066e0: 6d62 6572 5a09 7061 7265 6e74 6b65 795a  mberZ.parentkeyZ
-000066f0: 0f70 6172 656e 7463 6861 696e 636f 6465  .parentchaincode
-00006700: 5a0b 7870 7562 5f68 6561 6465 725a 0478  Z.xpub_headerZ.x
-00006710: 7075 6272 3700 0000 7237 0000 0072 3800  pubr7...r7...r8.
-00006720: 0000 da13 6361 7264 5f62 6970 3332 5f67  ....card_bip32_g
-00006730: 6574 5f78 7075 6247 0300 0073 2200 0000  et_xpubG...s"...
-00006740: 000b 0c03 1401 0c01 1002 0e01 0801 1001  ................
-00006750: 1202 1601 1801 0c02 1401 2c01 1201 0801  ..........,.....
-00006760: 1401 7a21 4361 7264 436f 6e6e 6563 746f  ..z!CardConnecto
-00006770: 722e 6361 7264 5f62 6970 3332 5f67 6574  r.card_bip32_get
-00006780: 5f78 7075 62f3 0000 0000 6306 0000 0000  _xpub.....c.....
-00006790: 0000 0015 0000 0005 0000 0043 0000 0073  ...........C...s
-000067a0: 2602 0000 7400 6a01 6401 8301 0100 7402  &...t.j.d.....t.
-000067b0: 7c03 8301 7403 6b02 7220 7c03 6a04 6402  |...t.k.r |.j.d.
-000067c0: 8301 7d03 7402 7c05 8301 7403 6b02 7236  ..}.t.|...t.k.r6
-000067d0: 7c05 6a04 6402 8301 7d05 6403 7d06 6404  |.j.d...}.d.}.d.
-000067e0: 7d07 7405 7c03 8301 7d08 7406 6a07 7d09  }.t.|...}.t.j.}.
-000067f0: 7406 6a08 7d0a 7c01 7d0b 7406 6a09 7d0c  t.j.}.|.}.t.j.}.
-00006800: 7c05 7364 6405 6e0a 640f 7405 7c05 8301  |.sdd.n.d.t.|...
-00006810: 1700 7d0d 7c09 7c0a 7c0b 7c0c 7c0d 6705  ..}.|.|.|.|.|.g.
-00006820: 7d0e 782a 740a 740b 6405 8301 8301 4400  }.x*t.t.d.....D.
-00006830: 5d1a 7d0f 7c0e 7c08 6407 7c0f 1400 3f00  ].}.|.|.d.|...?.
-00006840: 6408 4000 6701 3700 7d0e 718c 5700 7c05  d.@.g.7.}.q.W.|.
-00006850: 72c4 7c0e 7405 7c05 8301 6701 3700 7d0e  r.|.t.|...g.7.}.
-00006860: 7c0e 7c05 3700 7d0e 7c00 6a0c 7c0e 8301  |.|.7.}.|.j.|...
-00006870: 5c03 7d10 7d11 7d12 7876 7c08 7c06 6b04  \.}.}.}.xv|.|.k.
-00006880: 9001 724a 7406 6a0d 7d0c 6409 7c06 1700  ..rJt.j.}.d.|...
-00006890: 7d0d 7c09 7c0a 7c0b 7c0c 7c0d 6705 7d0e  }.|.|.|.|.|.g.}.
-000068a0: 7c0e 7c06 6407 3f00 6408 4000 7c06 6408  |.|.d.?.d.@.|.d.
-000068b0: 4000 6702 3700 7d0e 7c0e 7c03 7c07 7c07  @.g.7.}.|.|.|.|.
-000068c0: 7c06 1700 8502 1900 3700 7d0e 7c07 7c06  |.......7.}.|.|.
-000068d0: 3700 7d07 7c08 7c06 3800 7d08 7c00 6a0c  7.}.|.|.8.}.|.j.
-000068e0: 7c0e 8301 5c03 7d10 7d11 7d12 71d6 5700  |...\.}.}.}.q.W.
-000068f0: 7c08 7d06 7406 6a0e 7d0c 6409 7c06 1700  |.}.t.j.}.d.|...
-00006900: 7405 7c04 8301 1700 7d0d 7c09 7c0a 7c0b  t.|.....}.|.|.|.
-00006910: 7c0c 7c0d 6705 7d0e 7c0e 7c06 6407 3f00  |.|.g.}.|.|.d.?.
-00006920: 6408 4000 7c06 6408 4000 6702 3700 7d0e  d.@.|.d.@.g.7.}.
-00006930: 7c0e 7c03 7c07 7c07 7c06 1700 8502 1900  |.|.|.|.|.......
-00006940: 7c04 1700 3700 7d0e 7c07 7c06 3700 7d07  |...7.}.|.|.7.}.
-00006950: 7c08 7c06 3800 7d08 7c00 6a0c 7c0e 8301  |.|.8.}.|.j.|...
-00006960: 5c03 7d10 7d11 7d12 7c11 640a 6b03 9001  \.}.}.}.|.d.k...
-00006970: 73d8 7c12 6404 6b03 9001 72fc 7400 6a0f  s.|.d.k...r.t.j.
-00006980: 640b 7410 640c 7c11 1400 7c12 1700 8301  d.t.d.|...|.....
-00006990: 9b00 640d 9d03 8301 0100 640e 7d13 6e1e  ..d.......d.}.n.
-000069a0: 7411 7412 7c03 7c05 8302 8301 7d14 7c00  t.t.|.|.....}.|.
-000069b0: 6a13 6a14 7c10 7c14 7c02 8303 7d13 7c10  j.j.|.|.|...}.|.
-000069c0: 7c11 7c12 7c13 6604 5300 2910 6134 0300  |.|.|.f.S.).a4..
-000069d0: 0020 5369 676e 2074 6865 206d 6573 7361  . Sign the messa
-000069e0: 6765 2077 6974 6820 7468 6520 6465 7669  ge with the devi
-000069f0: 6365 0a20 2020 2020 2020 200a 2020 2020  ce.        .    
-00006a00: 2020 2020 4d65 7373 6167 6520 6973 2070      Message is p
-00006a10: 7265 7065 6e64 6564 2077 6974 6820 6120  repended with a 
-00006a20: 7370 6563 6966 6963 2068 6561 6465 7220  specific header 
-00006a30: 6173 2064 6573 6372 6962 6564 2068 6572  as described her
-00006a40: 653a 0a20 2020 2020 2020 2068 7474 7073  e:.        https
-00006a50: 3a2f 2f62 6974 636f 696e 2e73 7461 636b  ://bitcoin.stack
-00006a60: 6578 6368 616e 6765 2e63 6f6d 2f71 7565  exchange.com/que
-00006a70: 7374 696f 6e73 2f37 3733 3234 2f68 6f77  stions/77324/how
-00006a80: 2d61 7265 2d62 6974 636f 696e 2d73 6967  -are-bitcoin-sig
-00006a90: 6e65 642d 6d65 7373 6167 6573 2d67 656e  ned-messages-gen
-00006aa0: 6572 6174 6564 0a20 2020 2020 2020 200a  erated.        .
-00006ab0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00006ac0: 7273 3a20 0a20 2020 2020 2020 206b 6579  rs: .        key
-00006ad0: 6e62 7220 2869 6e74 293a 2074 6865 206b  nbr (int): the k
-00006ae0: 6579 2074 6f20 7573 6520 2830 7846 4620  ey to use (0xFF 
-00006af0: 666f 7220 6269 7033 3220 6b65 7929 0a20  for bip32 key). 
-00006b00: 2020 2020 2020 2070 7562 6b65 7920 2845         pubkey (E
-00006b10: 4350 7562 6b65 7929 3a20 7468 6520 7075  CPubkey): the pu
-00006b20: 626b 6579 2075 7365 6420 666f 7220 7369  bkey used for si
-00006b30: 676e 696e 673b 2074 6869 7320 6973 2075  gning; this is u
-00006b40: 7365 6420 666f 7220 6b65 7920 7265 636f  sed for key reco
-00006b50: 7665 7279 0a20 2020 2020 2020 206d 6573  very.        mes
-00006b60: 7361 6765 2028 7374 7220 7c20 6279 7465  sage (str | byte
-00006b70: 7329 3a20 7468 6520 6d65 7373 6167 6520  s): the message 
-00006b80: 746f 2073 6967 6e0a 2020 2020 2020 2020  to sign.        
-00006b90: 686d 6163 3a20 7468 6520 3230 2d62 7974  hmac: the 20-byt
-00006ba0: 6520 686d 6163 2063 6f64 6520 7265 7175  e hmac code requ
-00006bb0: 6972 6564 2069 6620 3246 4120 6973 2065  ired if 2FA is e
-00006bc0: 6e61 626c 6564 0a20 2020 2020 2020 2061  nabled.        a
-00006bd0: 6c74 636f 696e 2028 7374 7220 7c20 6279  ltcoin (str | by
-00006be0: 7465 7329 3a20 666f 7220 616c 7463 6f69  tes): for altcoi
-00006bf0: 6e20 7369 676e 696e 670a 2020 2020 2020  n signing.      
-00006c00: 2020 0a20 2020 2020 2020 2052 6574 7572    .        Retur
-00006c10: 6e73 3a20 0a20 2020 2020 2020 2028 7265  ns: .        (re
-00006c20: 7370 6f6e 7365 2c20 7377 312c 2073 7732  sponse, sw1, sw2
-00006c30: 2c20 636f 6d70 7369 6729 3a20 286c 6973  , compsig): (lis
-00006c40: 742c 2069 6e74 2c20 696e 742c 2062 7974  t, int, int, byt
-00006c50: 6573 290a 2020 2020 2020 2020 636f 6d70  es).        comp
-00006c60: 7369 6720 6973 2074 6865 2073 6967 6e61  sig is the signa
-00006c70: 7475 7265 2069 6e20 2063 6f6d 7061 6374  ture in  compact
-00006c80: 2036 352d 6279 7465 2066 6f72 6d61 7420   65-byte format 
-00006c90: 0a20 2020 2020 2020 2028 6874 7470 733a  .        (https:
-00006ca0: 2f2f 6269 7463 6f69 6e2e 7374 6163 6b65  //bitcoin.stacke
-00006cb0: 7863 6861 6e67 652e 636f 6d2f 7175 6573  xchange.com/ques
-00006cc0: 7469 6f6e 732f 3132 3535 342f 7768 792d  tions/12554/why-
-00006cd0: 7468 652d 7369 676e 6174 7572 652d 6973  the-signature-is
-00006ce0: 2d61 6c77 6179 732d 3635 2d31 3332 3332  -always-65-13232
-00006cf0: 2d62 7974 6573 2d6c 6f6e 6729 0a20 2020  -bytes-long).   
-00006d00: 2020 2020 207a 1449 6e20 6361 7264 5f73       z.In card_s
-00006d10: 6967 6e5f 6d65 7373 6167 6572 bf00 0000  ign_messager....
-00006d20: 729b 0000 0072 0100 0000 7243 0000 0072  r....r....rC...r
-00006d30: 0c00 0000 72b2 0000 0072 d300 0000 7223  ....r....r....r#
-00006d40: 0000 0072 4100 0000 7a34 556e 6578 7065  ...rA...z4Unexpe
-00006d50: 6374 6564 2065 7272 6f72 2069 6e20 6361  cted error in ca
-00006d60: 7264 5f73 6967 6e5f 6d65 7373 6167 6528  rd_sign_message(
-00006d70: 2920 2865 7272 6f72 2063 6f64 6520 72ba  ) (error code r.
-00006d80: 0000 0072 bb00 0000 721c 0100 0072 2100  ...r....r....r!.
-00006d90: 0000 2915 7227 0000 0072 3400 0000 7226  ..).r'...r4...r&
-00006da0: 0000 0072 7500 0000 72c7 0000 0072 3500  ...ru...r....r5.
-00006db0: 0000 722b 0000 0072 bc00 0000 5a10 494e  ..r+...r....Z.IN
-00006dc0: 535f 5349 474e 5f4d 4553 5341 4745 da07  S_SIGN_MESSAGE..
-00006dd0: 4f50 5f49 4e49 5472 d400 0000 72d5 0000  OP_INITr....r...
-00006de0: 0072 9900 0000 da0a 4f50 5f50 524f 4345  .r......OP_PROCE
-00006df0: 5353 da0b 4f50 5f46 494e 414c 495a 4572  SS..OP_FINALIZEr
-00006e00: 5400 0000 724c 0000 0072 1400 0000 7213  T...rL...r....r.
-00006e10: 0000 0072 7600 0000 5a17 7061 7273 655f  ...rv...Z.parse_
-00006e20: 6d65 7373 6167 655f 7369 676e 6174 7572  message_signatur
-00006e30: 6529 1572 3600 0000 da06 6b65 796e 6272  e).r6.....keynbr
-00006e40: 7211 0100 00da 076d 6573 7361 6765 72eb  r......messager.
-00006e50: 0000 005a 0761 6c74 636f 696e da05 6368  ...Z.altcoin..ch
-00006e60: 756e 6bda 0d62 7566 6665 725f 6f66 6673  unk..buffer_offs
-00006e70: 6574 da0b 6275 6666 6572 5f6c 6566 7472  et..buffer_leftr
-00006e80: 9f00 0000 7287 0000 0072 a000 0000 72a1  ....r....r....r.
-00006e90: 0000 0072 ca00 0000 7298 0000 0072 db00  ...r....r....r..
-00006ea0: 0000 7222 0000 0072 5d00 0000 725e 0000  ..r"...r]...r^..
-00006eb0: 005a 0763 6f6d 7073 6967 da04 6861 7368  .Z.compsig..hash
-00006ec0: 7237 0000 0072 3700 0000 7238 0000 00da  r7...r7...r8....
-00006ed0: 1163 6172 645f 7369 676e 5f6d 6573 7361  .card_sign_messa
-00006ee0: 6765 6d03 0000 7358 0000 0000 120a 010c  gem...sX........
-00006ef0: 010a 010c 010a 0404 0104 0108 0306 0106  ................
-00006f00: 0104 0106 0114 010e 0112 011a 0104 010e  ................
-00006f10: 0108 0310 030c 0406 0108 010e 0118 0114  ................
-00006f20: 0108 0108 0214 0304 0406 0110 010e 0118  ................
-00006f30: 0118 0108 0108 0210 0314 011e 0106 030e  ................
-00006f40: 0110 027a 1f43 6172 6443 6f6e 6e65 6374  ...z.CardConnect
-00006f50: 6f72 2e63 6172 645f 7369 676e 5f6d 6573  or.card_sign_mes
-00006f60: 7361 6765 4629 01da 0b74 7261 6e73 6163  sageF)...transac
-00006f70: 7469 6f6e 6303 0000 0000 0000 0010 0000  tionc...........
-00006f80: 0005 0000 0043 0000 0073 a400 0000 7400  .....C...s....t.
-00006f90: 6a01 6401 8301 0100 7402 6a03 7d03 7402  j.d.....t.j.}.t.
-00006fa0: 6a04 7d04 7402 6a05 7d05 7c02 7224 6402  j.}.t.j.}.|.r$d.
-00006fb0: 6e02 6403 7d06 7406 7c01 8301 7d07 7854  n.d.}.t.|...}.xT
-00006fc0: 7c07 6a07 8300 7384 7c02 7246 7c07 6a08  |.j...s.|.rF|.j.
-00006fd0: 8300 6e06 7c07 6a09 8300 7d08 740a 7c08  ..n.|.j...}.t.|.
-00006fe0: 8301 7d09 7c03 7c04 7c05 7c06 7c09 6705  ..}.|.|.|.|.|.g.
-00006ff0: 7d0a 7c0a 7c08 3700 7d0a 7c00 6a0b 7c0a  }.|.|.7.}.|.j.|.
-00007000: 8301 5c03 7d0b 7d0c 7d0d 7402 6a0c 7d05  ..\.}.}.}.t.j.}.
-00007010: 7132 5700 7c00 6a0d 6a0e 7c0b 8301 5c02  q2W.|.j.j.|...\.
-00007020: 7d0e 7d0f 7c0b 7c0c 7c0d 7c0e 7c0f 6605  }.}.|.|.|.|.|.f.
-00007030: 5300 2904 615a 0100 0020 5061 7273 6520  S.).aZ... Parse 
-00007040: 6120 7472 616e 7361 6374 696f 6e20 746f  a transaction to
-00007050: 2062 6520 7369 676e 6564 2062 7920 7468   be signed by th
-00007060: 6520 6465 7669 6365 0a20 2020 2020 2020  e device.       
-00007070: 200a 2020 2020 2020 2020 5061 7261 6d65   .        Parame
-00007080: 7465 7273 3a20 0a20 2020 2020 2020 2074  ters: .        t
-00007090: 7261 6e73 6163 7469 6f6e 2028 6279 7465  ransaction (byte
-000070a0: 7329 3a20 7468 6520 7472 616e 7361 6374  s): the transact
-000070b0: 696f 6e20 746f 2070 6172 7365 0a20 2020  ion to parse.   
-000070c0: 2020 2020 2069 735f 7365 6777 6974 2028       is_segwit (
-000070d0: 626f 6f6c 290a 2020 2020 2020 2020 0a20  bool).        . 
-000070e0: 2020 2020 2020 2052 6574 7572 6e73 3a20         Returns: 
-000070f0: 0a20 2020 2020 2020 2028 7265 7370 6f6e  .        (respon
-00007100: 7365 2c20 7377 312c 2073 7732 2c20 7478  se, sw1, sw2, tx
-00007110: 5f68 6173 682c 206e 6565 6473 5f32 6661  _hash, needs_2fa
-00007120: 290a 2020 2020 2020 2020 7478 5f68 6173  ).        tx_has
-00007130: 6820 286c 6973 7429 3a20 6861 7368 2061  h (list): hash a
-00007140: 7320 636f 6d70 7574 6564 2062 7920 7468  s computed by th
-00007150: 6520 6465 7669 6365 0a20 2020 2020 2020  e device.       
-00007160: 206e 6565 6473 5f32 4641 2028 626f 6f6c   needs_2FA (bool
-00007170: 293a 2077 6865 7468 6572 2032 4641 2069  ): whether 2FA i
-00007180: 7320 7265 7175 6972 6564 0a20 2020 2020  s required.     
-00007190: 2020 207a 1949 6e20 6361 7264 5f70 6172     z.In card_par
-000071a0: 7365 5f74 7261 6e73 6163 7469 6f6e 720c  se_transactionr.
-000071b0: 0000 0072 0100 0000 290f 7227 0000 0072  ...r....).r'...r
-000071c0: 3400 0000 722b 0000 0072 bc00 0000 5a15  4...r+...r....Z.
-000071d0: 494e 535f 5041 5253 455f 5452 414e 5341  INS_PARSE_TRANSA
-000071e0: 4354 494f 4e72 1d01 0000 720f 0000 005a  CTIONr....r....Z
-000071f0: 0969 735f 7061 7273 6564 5a18 7061 7273  .is_parsedZ.pars
-00007200: 655f 7365 6777 6974 5f74 7261 6e73 6163  e_segwit_transac
-00007210: 7469 6f6e 5a11 7061 7273 655f 7472 616e  tionZ.parse_tran
-00007220: 7361 6374 696f 6e72 3500 0000 7299 0000  sactionr5...r...
-00007230: 0072 1e01 0000 7276 0000 005a 1770 6172  .r....rv...Z.par
-00007240: 7365 5f70 6172 7365 5f74 7261 6e73 6163  se_parse_transac
-00007250: 7469 6f6e 2910 7236 0000 0072 2701 0000  tion).r6...r'...
-00007260: 5a09 6973 5f73 6567 7769 7472 9f00 0000  Z.is_segwitr....
-00007270: 7287 0000 0072 a000 0000 72a1 0000 005a  r....r....r....Z
-00007280: 0874 7870 6172 7365 7272 2201 0000 72ca  .txparserr"...r.
-00007290: 0000 0072 9800 0000 7222 0000 0072 5d00  ...r....r"...r].
-000072a0: 0000 725e 0000 005a 0774 785f 6861 7368  ..r^...Z.tx_hash
-000072b0: 5a09 6e65 6564 735f 3266 6172 3700 0000  Z.needs_2far7...
-000072c0: 7237 0000 0072 3800 0000 da16 6361 7264  r7...r8.....card
-000072d0: 5f70 6172 7365 5f74 7261 6e73 6163 7469  _parse_transacti
-000072e0: 6f6e c403 0000 731e 0000 0000 0c0a 0106  on....s.........
-000072f0: 0106 0106 010c 0308 010a 0214 0108 010e  ................
-00007300: 0108 0c10 030a 0310 027a 2443 6172 6443  .........z$CardC
-00007310: 6f6e 6e65 6374 6f72 2e63 6172 645f 7061  onnector.card_pa
-00007320: 7273 655f 7472 616e 7361 6374 696f 6e63  rse_transactionc
-00007330: 0400 0000 0000 0000 0e00 0000 0500 0000  ................
-00007340: 4300 0000 73c0 0000 0074 006a 0164 0183  C...s....t.j.d..
-00007350: 0101 0074 026a 037d 0474 026a 047d 057c  ...t.j.}.t.j.}.|
-00007360: 017d 0664 027d 0774 057c 0283 0164 036b  .}.d.}.t.|...d.k
-00007370: 0372 4474 0664 0474 0774 057c 0283 0183  .rDt.d.t.t.|....
-00007380: 0117 0064 0517 0083 0182 016e 487c 0364  ...d.......nH|.d
-00007390: 066b 0272 527c 027d 086e 3a74 057c 0383  .k.rR|.}.n:t.|..
-000073a0: 0164 076b 0372 7674 0664 0874 0774 057c  .d.k.rvt.d.t.t.|
-000073b0: 0383 0183 0117 0064 0917 0083 0182 017c  .......d.......|
-000073c0: 0274 0874 096a 0a64 0a83 0183 0117 007c  .t.t.j.d.......|
-000073d0: 0317 007d 0874 057c 0883 017d 097c 047c  ...}.t.|...}.|.|
-000073e0: 057c 067c 077c 0967 057c 0817 007d 0a7c  .|.|.|.g.|...}.|
-000073f0: 006a 0b7c 0a83 015c 037d 0b7d 0c7d 0d7c  .j.|...\.}.}.}.|
-00007400: 0b7c 0c7c 0d66 0353 0029 0b61 7401 0000  .|.|.f.S.).at...
-00007410: 2053 6967 6e20 7468 6520 7472 616e 7361   Sign the transa
-00007420: 6374 696f 6e20 696e 2074 6865 2064 6576  ction in the dev
-00007430: 6963 650a 2020 2020 2020 2020 0a20 2020  ice.        .   
-00007440: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
-00007450: 200a 2020 2020 2020 2020 6b65 796e 6272   .        keynbr
-00007460: 2028 696e 7429 3a20 7468 6520 6b65 7920   (int): the key 
-00007470: 746f 2075 7365 2028 3078 4646 2066 6f72  to use (0xFF for
-00007480: 2062 6970 3332 206b 6579 290a 2020 2020   bip32 key).    
-00007490: 2020 2020 7478 6861 7368 2028 6c69 7374      txhash (list
-000074a0: 293a 2074 6865 2074 7261 6e73 6163 7469  ): the transacti
-000074b0: 6f6e 2068 6173 6820 6173 2072 6574 7572  on hash as retur
-000074c0: 6e65 6420 6279 2074 6865 2064 6576 6963  ned by the devic
-000074d0: 650a 2020 2020 2020 2020 6368 616c 7265  e.        chalre
-000074e0: 7370 6f6e 7365 2028 6c69 7374 293a 2074  sponse (list): t
-000074f0: 6865 2068 6d61 6320 636f 6465 2069 6620  he hmac code if 
-00007500: 3246 4120 6973 2065 6e61 626c 6564 0a20  2FA is enabled. 
-00007510: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007520: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
-00007530: 2020 2872 6573 706f 6e73 652c 2073 7731    (response, sw1
-00007540: 2c20 7377 3229 0a20 2020 2020 2020 2072  , sw2).        r
-00007550: 6573 706f 6e73 6520 286c 6973 7429 3a20  esponse (list): 
-00007560: 7468 6520 7369 676e 6174 7572 6520 696e  the signature in
-00007570: 2044 4552 2066 6f72 6d61 740a 2020 2020   DER format.    
-00007580: 2020 2020 7a18 496e 2063 6172 645f 7369      z.In card_si
-00007590: 676e 5f74 7261 6e73 6163 7469 6f6e 7201  gn_transactionr.
-000075a0: 0000 0072 0d01 0000 7a15 5772 6f6e 6720  ...r....z.Wrong 
-000075b0: 7478 6861 7368 206c 656e 6774 683a 207a  txhash length: z
-000075c0: 0e28 7368 6f75 6c64 2062 6520 3332 294e  .(should be 32)N
-000075d0: 7207 0100 007a 2057 726f 6e67 2043 6861  r....z Wrong Cha
-000075e0: 6c6c 656e 6765 2072 6573 706f 6e73 6520  llenge response 
-000075f0: 6c65 6e67 7468 3a7a 0e28 7368 6f75 6c64  length:z.(should
-00007600: 2062 6520 3230 29da 0438 3030 3029 0c72   be 20)..8000).r
-00007610: 2700 0000 7234 0000 0072 2b00 0000 72bc  '...r4...r+...r.
-00007620: 0000 005a 1449 4e53 5f53 4947 4e5f 5452  ...Z.INS_SIGN_TR
-00007630: 414e 5341 4354 494f 4e72 3500 0000 da0a  ANSACTIONr5.....
-00007640: 5661 6c75 6545 7272 6f72 7275 0000 0072  ValueErrorru...r
-00007650: c600 0000 724b 0000 0072 df00 0000 7299  ....rK...r....r.
-00007660: 0000 0029 0e72 3600 0000 7220 0100 00da  ...).r6...r ....
-00007670: 0674 7868 6173 68da 0c63 6861 6c72 6573  .txhash..chalres
-00007680: 706f 6e73 6572 9f00 0000 7287 0000 0072  ponser....r....r
-00007690: a000 0000 72a1 0000 0072 c900 0000 72ca  ....r....r....r.
-000076a0: 0000 0072 9800 0000 7222 0000 0072 5d00  ...r....r"...r].
-000076b0: 0000 725e 0000 0072 3700 0000 7237 0000  ..r^...r7...r7..
-000076c0: 0072 3800 0000 da15 6361 7264 5f73 6967  .r8.....card_sig
-000076d0: 6e5f 7472 616e 7361 6374 696f 6ef3 0300  n_transaction...
-000076e0: 0073 2000 0000 000c 0a03 0601 0601 0401  .s .............
-000076f0: 0402 0c01 1a01 0801 0602 0c01 1801 1601  ................
-00007700: 0801 1203 1001 7a23 4361 7264 436f 6e6e  ......z#CardConn
-00007710: 6563 746f 722e 6361 7264 5f73 6967 6e5f  ector.card_sign_
-00007720: 7472 616e 7361 6374 696f 6e63 0400 0000  transactionc....
-00007730: 0000 0000 0e00 0000 0500 0000 4300 0000  ............C...
-00007740: 73be 0000 0074 006a 0164 0183 0101 0074  s....t.j.d.....t
-00007750: 026a 037d 0464 027d 057c 017d 0664 037d  .j.}.d.}.|.}.d.}
-00007760: 0774 047c 0283 0164 046b 0372 4274 0564  .t.|...d.k.rBt.d
-00007770: 0574 0674 047c 0283 0183 0117 0064 0617  .t.t.|.......d..
-00007780: 0083 0182 016e 487c 0364 076b 0272 507c  .....nH|.d.k.rP|
-00007790: 027d 086e 3a74 047c 0383 0164 086b 0372  .}.n:t.|...d.k.r
-000077a0: 7474 0564 0974 0674 047c 0383 0183 0117  tt.d.t.t.|......
-000077b0: 0064 0a17 0083 0182 017c 0274 0774 086a  .d.......|.t.t.j
-000077c0: 0964 0b83 0183 0117 007c 0317 007d 0874  .d.......|...}.t
-000077d0: 047c 0883 017d 097c 047c 057c 067c 077c  .|...}.|.|.|.|.|
-000077e0: 0967 057c 0817 007d 0a7c 006a 0a7c 0a83  .g.|...}.|.j.|..
-000077f0: 015c 037d 0b7d 0c7d 0d7c 0b7c 0c7c 0d66  .\.}.}.}.|.|.|.f
-00007800: 0353 0029 0c61 6001 0000 2053 6967 6e20  .S.).a`... Sign 
-00007810: 7468 6520 7472 616e 7361 6374 696f 6e20  the transaction 
-00007820: 6861 7368 2069 6e20 7468 6520 6465 7669  hash in the devi
-00007830: 6365 0a20 2020 2020 2020 200a 2020 2020  ce.        .    
-00007840: 2020 2020 5061 7261 6d65 7465 7273 3a20      Parameters: 
-00007850: 0a20 2020 2020 2020 206b 6579 6e62 7220  .        keynbr 
-00007860: 2869 6e74 293a 2074 6865 206b 6579 2074  (int): the key t
-00007870: 6f20 7573 6520 2830 7846 4620 666f 7220  o use (0xFF for 
-00007880: 6269 7033 3220 6b65 7929 0a20 2020 2020  bip32 key).     
-00007890: 2020 2074 7868 6173 6820 286c 6973 7429     txhash (list)
-000078a0: 3a20 7468 6520 7472 616e 7361 6374 696f  : the transactio
-000078b0: 6e20 6861 7368 200a 2020 2020 2020 2020  n hash .        
-000078c0: 6368 616c 7265 7370 6f6e 7365 2028 6c69  chalresponse (li
-000078d0: 7374 293a 2074 6865 2068 6d61 6320 636f  st): the hmac co
-000078e0: 6465 2069 6620 3246 4120 6973 2065 6e61  de if 2FA is ena
-000078f0: 626c 6564 0a20 2020 2020 2020 200a 2020  bled.        .  
-00007900: 2020 2020 2020 5265 7475 726e 733a 200a        Returns: .
-00007910: 2020 2020 2020 2020 2872 6573 706f 6e73          (respons
-00007920: 652c 2073 7731 2c20 7377 3229 0a20 2020  e, sw1, sw2).   
-00007930: 2020 2020 2072 6573 706f 6e73 6520 286c       response (l
-00007940: 6973 7429 3a20 7468 6520 7369 676e 6174  ist): the signat
-00007950: 7572 6520 696e 2044 4552 2066 6f72 6d61  ure in DER forma
-00007960: 740a 2020 2020 2020 2020 7a1d 496e 2063  t.        z.In c
-00007970: 6172 645f 7369 676e 5f74 7261 6e73 6163  ard_sign_transac
-00007980: 7469 6f6e 5f68 6173 68e9 7a00 0000 7201  tion_hash.z...r.
-00007990: 0000 0072 0d01 0000 7a15 5772 6f6e 6720  ...r....z.Wrong 
-000079a0: 7478 6861 7368 206c 656e 6774 683a 207a  txhash length: z
-000079b0: 0e28 7368 6f75 6c64 2062 6520 3332 294e  .(should be 32)N
-000079c0: 7207 0100 007a 2057 726f 6e67 2043 6861  r....z Wrong Cha
-000079d0: 6c6c 656e 6765 2072 6573 706f 6e73 6520  llenge response 
-000079e0: 6c65 6e67 7468 3a7a 0e28 7368 6f75 6c64  length:z.(should
-000079f0: 2062 6520 3230 2972 2901 0000 290b 7227   be 20)r)...).r'
-00007a00: 0000 0072 3400 0000 722b 0000 0072 bc00  ...r4...r+...r..
-00007a10: 0000 7235 0000 0072 2a01 0000 7275 0000  ..r5...r*...ru..
-00007a20: 0072 c600 0000 724b 0000 0072 df00 0000  .r....rK...r....
-00007a30: 7299 0000 0029 0e72 3600 0000 7220 0100  r....).r6...r ..
-00007a40: 0072 2b01 0000 722c 0100 0072 9f00 0000  .r+...r,...r....
-00007a50: 7287 0000 0072 a000 0000 72a1 0000 0072  r....r....r....r
-00007a60: c900 0000 72ca 0000 0072 9800 0000 7222  ....r....r....r"
-00007a70: 0000 0072 5d00 0000 725e 0000 0072 3700  ...r]...r^...r7.
-00007a80: 0000 7237 0000 0072 3800 0000 da1a 6361  ..r7...r8.....ca
-00007a90: 7264 5f73 6967 6e5f 7472 616e 7361 6374  rd_sign_transact
-00007aa0: 696f 6e5f 6861 7368 1604 0000 7320 0000  ion_hash....s ..
-00007ab0: 0000 0c0a 0306 0104 0104 0104 020c 011a  ................
-00007ac0: 0108 0106 020c 0118 0116 0108 0112 0310  ................
-00007ad0: 017a 2843 6172 6443 6f6e 6e65 6374 6f72  .z(CardConnector
-00007ae0: 2e63 6172 645f 7369 676e 5f74 7261 6e73  .card_sign_trans
-00007af0: 6163 7469 6f6e 5f68 6173 6863 0300 0000  action_hashc....
-00007b00: 0000 0000 0d00 0000 0500 0000 4300 0000  ............C...
-00007b10: 73c2 0000 0074 007c 0183 0174 016b 0872  s....t.|...t.k.r
-00007b20: 1c74 0274 036a 047c 0183 0183 017d 016e  .t.t.j.|.....}.n
-00007b30: 1474 007c 0183 0174 036b 0872 3074 027c  .t.|...t.k.r0t.|
-00007b40: 0183 017d 0174 056a 0664 0183 0101 0074  ...}.t.j.d.....t
-00007b50: 076a 087d 0364 027d 0464 037d 0564 037d  .j.}.d.}.d.}.d.}
-00007b60: 0664 047d 077c 037c 047c 057c 067c 0767  .d.}.|.|.|.|.|.g
-00007b70: 057d 087c 087c 0137 007d 0878 2a74 0974  .}.|.|.7.}.x*t.t
-00007b80: 0a64 0583 0183 0144 005d 1a7d 097c 087c  .d.....D.].}.|.|
-00007b90: 0264 057c 0914 003f 0064 0640 0067 0137  .d.|...?.d.@.g.7
-00007ba0: 007d 0871 7457 007c 006a 0b7c 0883 015c  .}.qtW.|.j.|...\
-00007bb0: 037d 0a7d 0b7d 0c7c 0b64 076b 0272 b87c  .}.}.}.|.d.k.r.|
-00007bc0: 0c64 036b 0272 b864 087c 005f 0c7c 0a7c  .d.k.r.d.|._.|.|
-00007bd0: 0b7c 0c66 0353 0029 097a e620 456e 6162  .|.f.S.).z. Enab
-00007be0: 6c65 2061 6e64 2069 6d70 6f72 7420 3246  le and import 2F
-00007bf0: 4120 696e 2074 6865 2064 6576 6963 650a  A in the device.
-00007c00: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00007c10: 2050 6172 616d 6574 6572 733a 200a 2020   Parameters: .  
-00007c20: 2020 2020 2020 686d 6163 7368 6131 3630        hmacsha160
-00007c30: 5f6b 6579 2028 6279 7465 7320 7c20 6c69  _key (bytes | li
-00007c40: 7374 293a 2074 6865 2032 302d 6279 7465  st): the 20-byte
-00007c50: 7320 7365 6372 6574 0a20 2020 2020 2020  s secret.       
-00007c60: 2061 6d6f 756e 745f 6c69 6d69 7420 2869   amount_limit (i
-00007c70: 6e74 293a 2074 6865 2061 6d6f 756e 7420  nt): the amount 
-00007c80: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00007c90: 2020 5265 7475 726e 733a 200a 2020 2020    Returns: .    
-00007ca0: 2020 2020 2872 6573 706f 6e73 652c 2073      (response, s
-00007cb0: 7731 2c20 7377 3229 0a20 2020 2020 2020  w1, sw2).       
-00007cc0: 207a 1349 6e20 6361 7264 5f73 6574 5f32   z.In card_set_2
-00007cd0: 4641 5f6b 6579 e979 0000 0072 0100 0000  FA_key.y...r....
-00007ce0: e91c 0000 0072 b200 0000 72d3 0000 0072  .....r....r....r
-00007cf0: 4100 0000 5429 0d72 2600 0000 7275 0000  A...T).r&...ru..
-00007d00: 0072 c600 0000 724b 0000 0072 df00 0000  .r....rK...r....
-00007d10: 7227 0000 0072 3400 0000 722b 0000 0072  r'...r4...r+...r
-00007d20: bc00 0000 72d4 0000 0072 d500 0000 7299  ....r....r....r.
-00007d30: 0000 0072 7700 0000 290d 7236 0000 0072  ...rw...).r6...r
-00007d40: d900 0000 72da 0000 0072 9f00 0000 7287  ....r....r....r.
-00007d50: 0000 0072 a000 0000 72a1 0000 0072 ca00  ...r....r....r..
-00007d60: 0000 7298 0000 0072 db00 0000 7222 0000  ..r....r....r"..
-00007d70: 0072 5d00 0000 725e 0000 0072 3700 0000  .r]...r^...r7...
-00007d80: 7237 0000 0072 3800 0000 da10 6361 7264  r7...r8.....card
-00007d90: 5f73 6574 5f32 4641 5f6b 6579 3d04 0000  _set_2FA_key=...
-00007da0: 7324 0000 0000 0a0c 0110 010c 0108 020a  s$..............
-00007db0: 0106 0104 0104 0104 0104 010e 0208 0112  ................
-00007dc0: 011a 0310 0110 0106 017a 1e43 6172 6443  .........z.CardC
-00007dd0: 6f6e 6e65 6374 6f72 2e63 6172 645f 7365  onnector.card_se
-00007de0: 745f 3246 415f 6b65 7963 0200 0000 0000  t_2FA_keyc......
-00007df0: 0000 0b00 0000 0500 0000 4300 0000 7396  ..........C...s.
-00007e00: 0000 0074 006a 0164 0183 0101 0074 027c  ...t.j.d.....t.|
-00007e10: 0183 0174 036b 0872 2674 0474 056a 067c  ...t.k.r&t.t.j.|
-00007e20: 0183 0183 017d 016e 1474 027c 0183 0174  .....}.n.t.|...t
-00007e30: 056b 0872 3a74 047c 0183 017d 0174 076a  .k.r:t.|...}.t.j
-00007e40: 087d 0264 027d 0364 037d 0464 037d 0564  .}.d.}.d.}.d.}.d
-00007e50: 047d 067c 027c 037c 047c 057c 0667 057d  .}.|.|.|.|.|.g.}
-00007e60: 077c 077c 0137 007d 077c 006a 097c 0783  .|.|.7.}.|.j.|..
-00007e70: 015c 037d 087d 097d 0a7c 0964 056b 0272  .\.}.}.}.|.d.k.r
-00007e80: 8c7c 0a64 036b 0272 8c64 067c 005f 0a7c  .|.d.k.r.d.|._.|
-00007e90: 087c 097c 0a66 0353 0029 077a b820 4469  .|.|.f.S.).z. Di
-00007ea0: 7361 626c 6520 3246 412e 0a20 2020 2020  sable 2FA..     
-00007eb0: 2020 200a 2020 2020 2020 2020 5061 7261     .        Para
-00007ec0: 6d65 7465 7273 3a20 0a20 2020 2020 2020  meters: .       
-00007ed0: 2063 6861 6c72 6573 706f 6e73 6520 286c   chalresponse (l
-00007ee0: 6973 7420 7c20 6279 7465 7320 7c20 6865  ist | bytes | he
-00007ef0: 785f 7374 7229 3a20 7468 6520 3230 2d62  x_str): the 20-b
-00007f00: 7974 6573 2063 6f64 6520 746f 2063 6f6e  ytes code to con
-00007f10: 6669 726d 0a20 2020 2020 2020 200a 2020  firm.        .  
-00007f20: 2020 2020 2020 5265 7475 726e 733a 200a        Returns: .
-00007f30: 2020 2020 2020 2020 2872 6573 706f 6e73          (respons
-00007f40: 652c 2073 7731 2c20 7377 3229 0a20 2020  e, sw1, sw2).   
-00007f50: 2020 2020 207a 1549 6e20 6361 7264 5f72       z.In card_r
-00007f60: 6573 6574 5f32 4641 5f6b 6579 e978 0000  eset_2FA_key.x..
-00007f70: 0072 0100 0000 7207 0100 0072 4100 0000  .r....r....rA...
-00007f80: 4629 0b72 2700 0000 7234 0000 0072 2600  F).r'...r4...r&.
-00007f90: 0000 7275 0000 0072 c600 0000 724b 0000  ..ru...r....rK..
-00007fa0: 0072 df00 0000 722b 0000 0072 bc00 0000  .r....r+...r....
-00007fb0: 7299 0000 0072 7700 0000 290b 7236 0000  r....rw...).r6..
-00007fc0: 0072 2c01 0000 729f 0000 0072 8700 0000  .r,...r....r....
-00007fd0: 72a0 0000 0072 a100 0000 72ca 0000 0072  r....r....r....r
-00007fe0: 9800 0000 7222 0000 0072 5d00 0000 725e  ....r"...r]...r^
-00007ff0: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
-00008000: 0000 da12 6361 7264 5f72 6573 6574 5f32  ....card_reset_2
-00008010: 4641 5f6b 6579 5e04 0000 7320 0000 0000  FA_key^...s ....
-00008020: 090a 010c 0110 010c 0108 0206 0104 0104  ................
-00008030: 0104 0104 010e 0108 0310 0110 0106 017a  ...............z
-00008040: 2043 6172 6443 6f6e 6e65 6374 6f72 2e63   CardConnector.c
-00008050: 6172 645f 7265 7365 745f 3246 415f 6b65  ard_reset_2FA_ke
-00008060: 7954 6303 0000 0000 0000 0018 0000 0005  yTc.............
-00008070: 0000 0043 0000 0073 7803 0000 7400 6a01  ...C...sx...t.j.
-00008080: 6401 8301 0100 7402 7c01 8301 7403 6b02  d.....t.|...t.k.
-00008090: 7220 7c01 6a04 6402 8301 7d01 7405 7c01  r |.j.d...}.t.|.
-000080a0: 8301 7d01 6700 7d03 7406 6a07 7d04 6403  ..}.g.}.t.j.}.d.
-000080b0: 7d05 7406 6a08 7d06 6404 7d07 7c02 9001  }.t.j.}.d.}.|...
-000080c0: 7222 6405 7d08 6406 7d09 7c04 7c05 7c08  r"d.}.d.}.|.|.|.
-000080d0: 7c06 7c09 6705 7d0a 7409 7c01 8301 7d0b  |.|.g.}.t.|...}.
-000080e0: 7c07 7c0b 7c07 1600 1800 7d0c 7c01 7c0c  |.|.|.....}.|.|.
-000080f0: 6701 7c0c 1400 1700 7d01 7c00 6a0a 7c0a  g.|.....}.|.j.|.
-00008100: 8301 5c03 7d0d 7d0e 7d0f 7c0e 6407 6b02  ..\.}.}.}.|.d.k.
-00008110: 72d8 7c0f 6406 6b02 72d8 7c0d 6406 6404  r.|.d.k.r.|.d.d.
-00008120: 8502 1900 7d10 7c0d 6404 6408 8502 1900  ....}.|.d.d.....
-00008130: 7d11 7c10 7d03 6406 6409 6c0b 6d0c 7d12  }.|.}.d.d.l.m.}.
-00008140: 0100 7c12 740d 7c11 8301 8301 6a0e 8300  ..|.t.|.....j...
-00008150: 7d11 6e48 7c0e 640a 6b02 6fe6 7c0f 640b  }.nH|.d.k.o.|.d.
-00008160: 6b02 9001 7206 740f 640c 7410 640d 7c0e  k...r.t.d.t.d.|.
-00008170: 1400 7c0f 1700 8301 9b00 9d02 8301 8201  ..|.............
-00008180: 6e1a 7411 640e 7410 640d 7c0e 1400 7c0f  n.t.d.t.d.|...|.
-00008190: 1700 8301 9b00 9d02 8301 8201 6ec2 640f  ............n.d.
-000081a0: 7d08 6404 7d09 7c04 7c05 7c08 7c06 7c09  }.d.}.|.|.|.|.|.
-000081b0: 6705 7d0a 7c01 6406 6404 8502 1900 7d10  g.}.|.d.d.....}.
-000081c0: 7c01 6404 6400 8502 1900 7d01 7c0a 7c10  |.d.d.....}.|.|.
-000081d0: 1700 7d0a 7409 7c01 8301 7c07 1600 6406  ..}.t.|...|...d.
-000081e0: 6b03 9001 7274 7400 6a12 6410 8301 0100  k...rtt.j.d.....
-000081f0: 7c00 6a0a 7c0a 8301 5c03 7d0d 7d0e 7d0f  |.j.|...\.}.}.}.
-00008200: 7c0e 6407 6b02 9001 729a 7c0f 6406 6b02  |.d.k...r.|.d.k.
-00008210: 9001 729a 6e4a 7c0e 640a 6b02 9001 72ca  ..r.nJ|.d.k...r.
-00008220: 7c0f 640b 6b02 9001 72ca 740f 640c 7410  |.d.k...r.t.d.t.
-00008230: 640d 7c0e 1400 7c0f 1700 8301 9b00 9d02  d.|...|.........
-00008240: 8301 8201 6e1a 7411 640e 7410 640d 7c0e  ....n.t.d.t.d.|.
-00008250: 1400 7c0f 1700 8301 9b00 9d02 8301 8201  ..|.............
-00008260: 6411 7d13 6406 7d14 7409 7c01 8301 7d15  d.}.d.}.t.|...}.
-00008270: 78a0 7c15 7c13 6b04 9002 7294 7406 6a13  x.|.|.k...r.t.j.
-00008280: 7d06 6405 7c13 1700 7d09 7c04 7c05 7c08  }.d.|...}.|.|.|.
-00008290: 7c06 7c09 6705 7d0a 7c0a 7c13 6412 3f00  |.|.g.}.|.|.d.?.
-000082a0: 6413 4000 7c13 6413 4000 6702 3700 7d0a  d.@.|.d.@.g.7.}.
-000082b0: 7c0a 7c01 7c14 7c14 7c13 1700 8502 1900  |.|.|.|.|.......
-000082c0: 3700 7d0a 7c14 7c13 3700 7d14 7c15 7c13  7.}.|.|.7.}.|.|.
-000082d0: 3800 7d15 7c00 6a0a 7c0a 8301 5c03 7d0d  8.}.|.j.|...\.}.
-000082e0: 7d0e 7d0f 7c0d 6406 1900 6412 3e00 7c0d  }.}.|.d...d.>.|.
-000082f0: 640f 1900 1700 7d16 7c03 7c0d 6405 6405  d.....}.|.|.d.d.
-00008300: 7c16 1700 8502 1900 3700 7d03 9001 71f6  |.......7.}...q.
-00008310: 5700 7c15 7d13 7406 6a14 7d06 6405 7c13  W.|.}.t.j.}.d.|.
-00008320: 1700 7d09 7c04 7c05 7c08 7c06 7c09 6705  ..}.|.|.|.|.|.g.
-00008330: 7d0a 7c0a 7c13 6412 3f00 6413 4000 7c13  }.|.|.d.?.d.@.|.
-00008340: 6413 4000 6702 3700 7d0a 7c0a 7c01 7c14  d.@.g.7.}.|.|.|.
-00008350: 7c14 7c13 1700 8502 1900 3700 7d0a 7c14  |.|.......7.}.|.
-00008360: 7c13 3700 7d14 7c15 7c13 3800 7d15 7c00  |.7.}.|.|.8.}.|.
-00008370: 6a0a 7c0a 8301 5c03 7d0d 7d0e 7d0f 7c0d  j.|...\.}.}.}.|.
-00008380: 6406 1900 6412 3e00 7c0d 640f 1900 1700  d...d.>.|.d.....
-00008390: 7d16 7c03 7c0d 6405 6405 7c16 1700 8502  }.|.|.d.d.|.....
-000083a0: 1900 3700 7d03 7c02 9003 724c 7415 6a16  ..7.}.|...rLt.j.
-000083b0: 740d 7c03 8301 8301 6a17 6414 8301 7d03  t.|.....j.d...}.
-000083c0: 7c11 7c03 6602 5300 7c03 6416 1900 7d17  |.|.f.S.|.d...}.
-000083d0: 7c03 6406 7c17 0b00 8502 1900 7d03 740d  |.d.|.......}.t.
-000083e0: 7c03 8301 6a17 6415 8301 7d03 7c03 5300  |...j.d...}.|.S.
-000083f0: 6400 5300 2917 4e7a 1d49 6e20 6361 7264  d.S.).Nz.In card
-00008400: 5f63 7279 7074 5f74 7261 6e73 6163 7469  _crypt_transacti
-00008410: 6f6e 5f32 4641 72bf 0000 00e9 7600 0000  on_2FAr.....v...
-00008420: 7288 0000 0072 2300 0000 7201 0000 0072  r....r#...r....r
-00008430: 4100 0000 e924 0000 0029 01da 0673 6861  A....$...)...sha
-00008440: 3235 3672 4200 0000 e919 0000 007a 2745  256rB........z'E
-00008450: 7272 6f72 3a20 3246 4120 6973 206e 6f74  rror: 2FA is not
-00008460: 2065 6e61 626c 6564 2028 6572 726f 7220   enabled (error 
-00008470: 636f 6465 3a20 72ba 0000 007a 1755 6e65  code: r....z.Une
-00008480: 7870 6563 7465 6420 6572 726f 7220 636f  xpected error co
-00008490: 6465 3a20 720c 0000 007a 0e50 6164 6469  de: r....z.Paddi
-000084a0: 6e67 2065 7272 6f72 2172 9b00 0000 72b2  ng error!r....r.
-000084b0: 0000 0072 d300 0000 da05 6173 6369 697a  ...r......asciiz
-000084c0: 076c 6174 696e 2d31 e9ff ffff ff29 1872  .latin-1.....).r
-000084d0: 2700 0000 7234 0000 0072 2600 0000 7275  '...r4...r&...ru
-000084e0: 0000 0072 c700 0000 72c6 0000 0072 2b00  ...r....r....r+.
-000084f0: 0000 72bc 0000 0072 1d01 0000 7235 0000  ..r....r....r5..
-00008500: 0072 9900 0000 724f 0000 0072 3701 0000  .r....rO...r7...
-00008510: 724b 0000 0072 5100 0000 72fa 0000 0072  rK...rQ...r....r
-00008520: 4c00 0000 72f2 0000 0072 2800 0000 721e  L...r....r(...r.
-00008530: 0100 0072 1f01 0000 da06 6261 7365 3634  ...r......base64
-00008540: 5a09 6236 3465 6e63 6f64 6572 c000 0000  Z.b64encoder....
-00008550: 2918 7236 0000 0072 6100 0000 5a0a 6973  ).r6...ra...Z.is
-00008560: 5f65 6e63 7279 7074 5a07 6d73 675f 6f75  _encryptZ.msg_ou
-00008570: 7472 9f00 0000 7287 0000 0072 a100 0000  tr....r....r....
-00008580: 5a09 626c 6f63 6b73 697a 6572 a000 0000  Z.blocksizer....
-00008590: 72ca 0000 0072 9800 0000 da04 7369 7a65  r....r......size
-000085a0: 5a07 7061 6473 697a 6572 2200 0000 725d  Z.padsizer"...r]
-000085b0: 0000 0072 5e00 0000 5a02 4956 5a06 6964  ...r^...Z.IVZ.id
-000085c0: 5f32 4641 7237 0100 0072 2201 0000 7223  _2FAr7...r"...r#
-000085d0: 0100 0072 2401 0000 5a08 6f75 745f 7369  ...r$...Z.out_si
-000085e0: 7a65 5a03 7061 6472 3700 0000 7237 0000  zeZ.padr7...r7..
-000085f0: 0072 3800 0000 da1a 6361 7264 5f63 7279  .r8.....card_cry
-00008600: 7074 5f74 7261 6e73 6163 7469 6f6e 5f32  pt_transaction_2
-00008610: 4641 7b04 0000 7390 0000 0000 010a 010c  FA{...s.........
-00008620: 010a 0108 0104 0306 0104 0106 0104 0106  ................
-00008630: 0104 0104 010e 0208 010c 010e 0210 0110  ................
-00008640: 020c 010c 0104 020c 0112 0112 011c 021c  ................
-00008650: 0204 0104 010e 020c 010c 0108 0112 010a  ................
-00008660: 0210 0114 0102 0114 011c 021a 0704 0104  ................
-00008670: 0108 020c 0106 0108 010e 0118 0114 0108  ................
-00008680: 0108 0210 0214 011a 0304 0106 0108 010e  ................
-00008690: 0118 0114 0108 0108 0210 0214 0114 0206  ................
-000086a0: 0214 0108 0308 010e 010e 017a 2843 6172  ...........z(Car
-000086b0: 6443 6f6e 6e65 6374 6f72 2e63 6172 645f  dConnector.card_
-000086c0: 6372 7970 745f 7472 616e 7361 6374 696f  crypt_transactio
-000086d0: 6e5f 3246 4163 0500 0000 0000 0000 0e00  n_2FAc..........
-000086e0: 0000 0500 0000 4300 0000 737a 0000 0074  ......C...sz...t
-000086f0: 006a 0164 0183 0101 0074 026a 037d 0574  .j.d.....t.j.}.t
-00008700: 026a 047d 067c 017d 077c 027d 0864 0274  .j.}.|.}.|.}.d.t
-00008710: 057c 0383 0117 0064 0217 0074 057c 0483  .|.....d...t.|..
-00008720: 0117 007d 097c 057c 067c 077c 087c 0967  ...}.|.|.|.|.|.g
-00008730: 0574 057c 0383 0167 0117 007c 0317 0074  .t.|...g...|...t
-00008740: 057c 0483 0167 0117 007c 0417 007d 0a7c  .|...g...|...}.|
-00008750: 006a 067c 0a83 015c 037d 0b7d 0c7d 0d7c  .j.|...\.}.}.}.|
-00008760: 0b7c 0c7c 0d66 0353 0029 034e 7a12 496e  .|.|.f.S.).Nz.In
-00008770: 2063 6172 645f 6372 6561 7465 5f50 494e   card_create_PIN
-00008780: 720c 0000 0029 0772 2700 0000 7234 0000  r....).r'...r4..
-00008790: 0072 2b00 0000 72bc 0000 0072 3000 0000  .r+...r....r0...
-000087a0: 7235 0000 0072 9900 0000 290e 7236 0000  r5...r....).r6..
-000087b0: 0072 7b00 0000 5a09 7069 6e5f 7472 6965  .r{...Z.pin_trie
-000087c0: 7372 7c00 0000 da04 7562 6c6b 729f 0000  sr|.....ublkr...
-000087d0: 0072 8700 0000 72a0 0000 0072 a100 0000  .r....r....r....
-000087e0: 72ca 0000 0072 9800 0000 7222 0000 0072  r....r....r"...r
-000087f0: 5d00 0000 725e 0000 0072 3700 0000 7237  ]...r^...r7...r7
-00008800: 0000 0072 3800 0000 da0f 6361 7264 5f63  ...r8.....card_c
-00008810: 7265 6174 655f 5049 4ee5 0400 0073 1200  reate_PIN....s..
-00008820: 0000 0001 0a01 0601 0601 0401 0401 1801  ................
-00008830: 2a03 1001 7a1d 4361 7264 436f 6e6e 6563  *...z.CardConnec
-00008840: 746f 722e 6361 7264 5f63 7265 6174 655f  tor.card_create_
-00008850: 5049 4e63 0300 0000 0000 0000 0c00 0000  PINc............
-00008860: 0500 0000 4300 0000 7352 0000 0074 006a  ....C...sR...t.j
-00008870: 0164 0183 0101 0074 026a 037d 0374 026a  .d.....t.j.}.t.j
-00008880: 047d 047c 017d 0564 027d 0674 057c 0283  .}.|.}.d.}.t.|..
-00008890: 017d 077c 037c 047c 057c 067c 0767 057c  .}.|.|.|.|.|.g.|
-000088a0: 0217 007d 087c 006a 067c 0883 015c 037d  ...}.|.j.|...\.}
-000088b0: 097d 0a7d 0b7c 097c 0a7c 0b66 0353 0029  .}.}.|.|.|.f.S.)
-000088c0: 034e 7a1d 496e 2063 6172 645f 7665 7269  .Nz.In card_veri
-000088d0: 6679 5f50 494e 5f64 6570 7265 6361 7465  fy_PIN_deprecate
-000088e0: 6472 0100 0000 2907 7227 0000 0072 3400  dr....).r'...r4.
-000088f0: 0000 722b 0000 0072 bc00 0000 7231 0000  ..r+...r....r1..
-00008900: 0072 3500 0000 7299 0000 0029 0c72 3600  .r5...r....).r6.
-00008910: 0000 727b 0000 0072 7c00 0000 729f 0000  ..r{...r|...r...
-00008920: 0072 8700 0000 72a0 0000 0072 a100 0000  .r....r....r....
-00008930: 72ca 0000 0072 9800 0000 7222 0000 0072  r....r....r"...r
-00008940: 5d00 0000 725e 0000 0072 3700 0000 7237  ]...r^...r7...r7
-00008950: 0000 0072 3800 0000 da1a 6361 7264 5f76  ...r8.....card_v
-00008960: 6572 6966 795f 5049 4e5f 6465 7072 6563  erify_PIN_deprec
-00008970: 6174 6564 f304 0000 7312 0000 0000 010a  ated....s.......
-00008980: 0106 0106 0104 0104 0108 0112 0210 017a  ...............z
-00008990: 2843 6172 6443 6f6e 6e65 6374 6f72 2e63  (CardConnector.c
-000089a0: 6172 645f 7665 7269 6679 5f50 494e 5f64  ard_verify_PIN_d
-000089b0: 6570 7265 6361 7465 6463 0100 0000 0000  eprecatedc......
-000089c0: 0000 0f00 0000 0600 0000 4300 0000 734e  ..........C...sN
-000089d0: 0200 0074 006a 0164 0183 0101 0090 0278  ...t.j.d.......x
-000089e0: 187c 006a 0290 0272 247c 006a 0364 006b  .|.j...r$|.j.d.k
-000089f0: 0872 6664 027d 017c 006a 0464 006b 0972  .rfd.}.|.j.d.k.r
-00008a00: 4c64 037c 006a 059b 0064 049d 037d 027c  Ld.|.j...d...}.|
-00008a10: 006a 046a 067c 0283 015c 027d 017d 037c  .j.j.|...\.}.}.|
-00008a20: 0164 026b 0872 5c74 0764 0583 0182 0174  .d.k.r\t.d.....t
-00008a30: 087c 0383 017d 036e 067c 006a 037d 0374  .|...}.n.|.j.}.t
-00008a40: 096a 0a7d 0474 096a 0b7d 057c 047c 0564  .j.}.t.j.}.|.|.d
-00008a50: 0664 0674 0c7c 0383 0167 057c 0317 007d  .d.t.|...g.|...}
-00008a60: 067c 006a 0d72 9e7c 006a 0e7c 0683 017d  .|.j.r.|.j.|...}
-00008a70: 067c 006a 0f6a 106a 117c 0683 015c 037d  .|.j.j.j.|...\.}
-00008a80: 077d 087d 097c 0864 076b 0272 d87c 0964  .}.}.|.d.k.r.|.d
-00008a90: 066b 0272 d87c 006a 1264 067c 0383 0201  .k.r.|.j.d.|....
-00008aa0: 007c 077c 087c 0966 0353 007c 0864 086b  .|.|.|.f.S.|.d.k
-00008ab0: 026f ea7c 0964 0940 0064 096b 0290 0172  .o.|.d.@.d.k...r
-00008ac0: 287c 006a 1264 0664 0083 0201 007c 0964  (|.j.d.d.....|.d
-00008ad0: 1640 007d 0a64 0a6a 137c 0a83 017d 027c  .@.}.d.j.|...}.|
-00008ae0: 006a 0464 006b 0990 0272 227c 006a 046a  .j.d.k...r"|.j.j
-00008af0: 1464 0b7c 0283 0201 0071 0e7c 0864 0c6b  .d.|.....q.|.d.k
-00008b00: 0290 0172 8a7c 0964 0d6b 0290 0172 8a7c  ...r.|.d.k...r.|
-00008b10: 006a 1264 0664 0083 0201 007c 006a 1583  .j.d.d.....|.j..
-00008b20: 005c 047d 0b7d 0c7d 0d7d 0e7c 0e6a 1664  .\.}.}.}.}.|.j.d
-00008b30: 0e64 1783 027d 0a64 0a6a 137c 0a83 017d  .d...}.d.j.|...}
-00008b40: 027c 006a 0464 006b 0990 0272 227c 006a  .|.j.d.k...r"|.j
-00008b50: 046a 1464 0b7c 0283 0201 0071 0e7c 0864  .j.d.|.....q.|.d
-00008b60: 0c6b 0290 0172 da7c 0964 106b 0290 0172  .k...r.|.d.k...r
-00008b70: da64 1174 1764 127c 0814 007c 0917 0083  .d.t.d.|...|....
-00008b80: 019b 0064 139d 037d 027c 006a 0464 006b  ...d...}.|.j.d.k
-00008b90: 0990 0172 d07c 006a 046a 1464 0b7c 0283  ...r.|.j.j.d.|..
-00008ba0: 0201 0074 077c 0283 0182 0171 0e7c 006a  ...t.|.....q.|.j
-00008bb0: 1264 0664 0083 0201 0064 1474 1764 127c  .d.d.....d.t.d.|
-00008bc0: 0814 007c 0917 0083 019b 0064 139d 037d  ...|.......d...}
-00008bd0: 027c 006a 0464 006b 0990 0272 187c 006a  .|.j.d.k...r.|.j
-00008be0: 046a 1464 0b7c 0283 0201 007c 077c 087c  .j.d.|.....|.|.|
-00008bf0: 0966 0353 0071 0e57 007c 006a 0464 006b  .f.S.q.W.|.j.d.k
-00008c00: 0990 0272 427c 006a 046a 1464 0b64 1583  ...rB|.j.j.d.d..
-00008c10: 0201 006e 0874 0764 1583 0182 0164 0053  ...n.t.d.....d.S
-00008c20: 0029 184e 7a12 496e 2063 6172 645f 7665  .).Nz.In card_ve
-00008c30: 7269 6679 5f50 494e 467a 1745 6e74 6572  rify_PINFz.Enter
-00008c40: 2074 6865 2050 494e 2066 6f72 2079 6f75   the PIN for you
-00008c50: 7220 fa01 3a7a 2b44 6576 6963 6520 6361  r ..:z+Device ca
-00008c60: 6e6e 6f74 2062 6520 756e 6c6f 636b 6564  nnot be unlocked
-00008c70: 2077 6974 686f 7574 2050 494e 2063 6f64   without PIN cod
-00008c80: 6521 7201 0000 0072 4100 0000 72cf 0000  e!r....rA...r...
-00008c90: 00e9 c000 0000 7a1e 5772 6f6e 6720 5049  ......z.Wrong PI
-00008ca0: 4e21 207b 7d20 7472 6965 7320 7265 6d61  N! {} tries rema
-00008cb0: 696e 696e 6721 7245 0000 0072 4200 0000  ining!rE...rB...
-00008cc0: 7223 0000 0072 b300 0000 720c 0000 0072  r#...r....r....r
-00008cd0: b900 0000 7a6b 546f 6f20 6d61 6e79 2066  ....zkToo many f
-00008ce0: 6169 6c65 6420 6174 7465 6d70 7473 2120  ailed attempts! 
-00008cf0: 596f 7572 2064 6576 6963 6520 6861 7320  Your device has 
-00008d00: 6265 656e 2062 6c6f 636b 6564 2120 0a0a  been blocked! ..
-00008d10: 596f 7520 6e65 6564 2079 6f75 7220 5055  You need your PU
-00008d20: 4b20 636f 6465 2074 6f20 756e 626c 6f63  K code to unbloc
-00008d30: 6b20 6974 2028 6572 726f 7220 636f 6465  k it (error code
-00008d40: 2072 ba00 0000 72bb 0000 007a 3550 6c65   r....r....z5Ple
-00008d50: 6173 6520 6368 6563 6b20 796f 7572 2063  ase check your c
-00008d60: 6172 6421 2055 6e65 7870 6563 7465 6420  ard! Unexpected 
-00008d70: 6572 726f 7220 2865 7272 6f72 2063 6f64  error (error cod
-00008d80: 6520 7a22 4e6f 2063 6172 6420 666f 756e  e z"No card foun
-00008d90: 6421 2050 6c65 6173 6520 696e 7365 7274  d! Please insert
-00008da0: 2063 6172 6421 693f ffff ff72 3a01 0000   card!i?...r:...
-00008db0: 2918 7227 0000 0072 3400 0000 7246 0000  ).r'...r4...rF..
-00008dc0: 0072 7c00 0000 725a 0000 0072 8100 0000  .r|...rZ...r....
-00008dd0: 5a0a 5049 4e5f 6469 616c 6f67 72fa 0000  Z.PIN_dialogr...
-00008de0: 0072 c600 0000 722b 0000 0072 bc00 0000  .r....r+...r....
-00008df0: 7231 0000 0072 3500 0000 7258 0000 0072  r1...r5...rX...r
-00008e00: 8d00 0000 7247 0000 0072 4800 0000 728e  ....rG...rH...r.
-00008e10: 0000 0072 d600 0000 da06 666f 726d 6174  ...r......format
-00008e20: 725b 0000 0072 5700 0000 da03 6765 7472  r[...rW.....getr
-00008e30: 4c00 0000 290f 7236 0000 005a 0669 735f  L...).r6...Z.is_
-00008e40: 5049 4e72 6100 0000 5a05 7069 6e5f 3072  PINra...Z.pin_0r
-00008e50: 9f00 0000 7287 0000 0072 9800 0000 7222  ....r....r....r"
-00008e60: 0000 0072 5d00 0000 725e 0000 00da 0870  ...r]...r^.....p
-00008e70: 696e 5f6c 6566 74da 0972 6573 706f 6e73  in_left..respons
-00008e80: 6532 da04 7377 3162 da04 7377 3262 72bd  e2..sw1b..sw2br.
-00008e90: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
-00008ea0: 0000 7290 0000 00ff 0400 0073 5e00 0000  ..r........s^...
-00008eb0: 0001 0a02 0c01 0a01 0401 0a01 0e01 1001  ................
-00008ec0: 0801 0801 0a02 0601 0601 0601 1602 0601  ................
-00008ed0: 0a01 1403 1001 0c01 0a02 1601 0c01 0801  ................
-00008ee0: 0a01 0c01 1002 1401 0c01 1001 0c01 0a01  ................
-00008ef0: 0c01 1002 1401 1801 0c01 0e01 0a03 0c01  ................
-00008f00: 1801 0c01 0e01 0e03 0c01 1002 0801 7a1d  ..............z.
-00008f10: 4361 7264 436f 6e6e 6563 746f 722e 6361  CardConnector.ca
-00008f20: 7264 5f76 6572 6966 795f 5049 4e63 0300  rd_verify_PINc..
-00008f30: 0000 0000 0000 0300 0000 0200 0000 4300  ..............C.
-00008f40: 0000 7310 0000 007c 017c 005f 007c 027c  ..s....|.|._.|.|
-00008f50: 005f 0164 0053 0029 014e 2902 727b 0000  ._.d.S.).N).r{..
-00008f60: 0072 7c00 0000 2903 7236 0000 0072 7b00  .r|...).r6...r{.
-00008f70: 0000 727c 0000 0072 3700 0000 7237 0000  ..r|...r7...r7..
-00008f80: 0072 3800 0000 72d6 0000 003d 0500 0073  .r8...r....=...s
-00008f90: 0600 0000 0001 0601 0601 7a15 4361 7264  ..........z.Card
-00008fa0: 436f 6e6e 6563 746f 722e 7365 745f 7069  Connector.set_pi
-00008fb0: 6e63 0400 0000 0000 0000 1300 0000 0500  nc..............
-00008fc0: 0000 4300 0000 739c 0100 0074 006a 0164  ..C...s....t.j.d
-00008fd0: 0183 0101 0074 026a 037d 0474 026a 047d  .....t.j.}.t.j.}
-00008fe0: 057c 017d 0664 027d 0764 0374 057c 0283  .|.}.d.}.d.t.|..
-00008ff0: 0117 0064 0317 0074 057c 0383 0117 007d  ...d...t.|.....}
-00009000: 087c 047c 057c 067c 077c 0867 0574 057c  .|.|.|.|.|.g.t.|
-00009010: 0283 0167 0117 007c 0217 0074 057c 0383  ...g...|...t.|..
-00009020: 0167 0117 007c 0317 007d 097c 006a 067c  .g...|...}.|.j.|
-00009030: 0983 015c 037d 0a7d 0b7d 0c7c 0b64 046b  ...\.}.}.}.|.d.k
-00009040: 0272 907c 0c64 026b 0272 907c 006a 077c  .r.|.d.k.r.|.j.|
-00009050: 017c 0383 0201 0090 016e 027c 0b64 056b  .|.......n.|.d.k
-00009060: 0272 dc7c 0c64 0640 0064 066b 0272 dc7c  .r.|.d.@.d.k.r.|
-00009070: 006a 077c 0164 0083 0201 007c 0c64 1040  .j.|.d.....|.d.@
-00009080: 007d 0d64 076a 087c 0d83 017d 0e7c 006a  .}.d.j.|...}.|.j
-00009090: 0964 006b 0972 da7c 006a 096a 0a64 087c  .d.k.r.|.j.j.d.|
-000090a0: 0e83 0201 006e b67c 0b64 096b 026f ea7c  .....n.|.d.k.o.|
-000090b0: 0c64 0a6b 0290 0172 447c 006a 077c 0164  .d.k...rD|.j.|.d
-000090c0: 0083 0201 007c 006a 0b83 005c 047d 0f7d  .....|.j...\.}.}
-000090d0: 107d 117d 127c 126a 0c64 0b64 1183 027d  .}.}.|.j.d.d...}
-000090e0: 0d64 076a 087c 0d83 017d 0e7c 006a 0964  .d.j.|...}.|.j.d
-000090f0: 006b 0990 0172 3a7c 006a 096a 0a64 087c  .k...r:|.j.j.d.|
-00009100: 0e83 0201 0074 0d7c 0e83 0182 016e 4e7c  .....t.|.....nN|
-00009110: 0b64 096b 0290 0172 927c 0c64 0c6b 0290  .d.k...r.|.d.k..
-00009120: 0172 9264 0d74 0e64 0e7c 0b14 007c 0c17  .r.d.t.d.|...|..
-00009130: 0083 019b 0064 0f9d 037d 0e7c 006a 0964  .....d...}.|.j.d
-00009140: 006b 0990 0172 8a7c 006a 096a 0a64 087c  .k...r.|.j.j.d.|
-00009150: 0e83 0201 0074 0d7c 0e83 0182 017c 0a7c  .....t.|.....|.|
-00009160: 0b7c 0c66 0353 0029 124e 7a12 496e 2063  .|.f.S.).Nz.In c
-00009170: 6172 645f 6368 616e 6765 5f50 494e 7201  ard_change_PINr.
-00009180: 0000 0072 0c00 0000 7241 0000 0072 cf00  ...r....rA...r..
-00009190: 0000 7242 0100 007a 1e57 726f 6e67 2050  ..rB...z.Wrong P
-000091a0: 494e 2120 7b7d 2074 7269 6573 2072 656d  IN! {} tries rem
-000091b0: 6169 6e69 6e67 2172 4500 0000 7242 0000  aining!rE...rB..
-000091c0: 0072 2300 0000 72b3 0000 0072 b900 0000  .r#...r....r....
-000091d0: 7a6b 546f 6f20 6d61 6e79 2066 6169 6c65  zkToo many faile
-000091e0: 6420 6174 7465 6d70 7473 2120 596f 7572  d attempts! Your
-000091f0: 2064 6576 6963 6520 6861 7320 6265 656e   device has been
-00009200: 2062 6c6f 636b 6564 2120 0a0a 596f 7520   blocked! ..You 
-00009210: 6e65 6564 2079 6f75 7220 5055 4b20 636f  need your PUK co
-00009220: 6465 2074 6f20 756e 626c 6f63 6b20 6974  de to unblock it
-00009230: 2028 6572 726f 7220 636f 6465 2072 ba00   (error code r..
-00009240: 0000 72bb 0000 0069 3fff ffff 723a 0100  ..r....i?...r:..
-00009250: 0029 0f72 2700 0000 7234 0000 0072 2b00  .).r'...r4...r+.
-00009260: 0000 72bc 0000 0072 3200 0000 7235 0000  ..r....r2...r5..
-00009270: 0072 9900 0000 72d6 0000 0072 4301 0000  .r....r....rC...
-00009280: 725a 0000 0072 5b00 0000 7257 0000 0072  rZ...r[...rW...r
-00009290: 4401 0000 72fa 0000 0072 4c00 0000 2913  D...r....rL...).
-000092a0: 7236 0000 0072 7b00 0000 5a07 6f6c 645f  r6...r{...Z.old_
-000092b0: 7069 6e5a 076e 6577 5f70 696e 729f 0000  pinZ.new_pinr...
-000092c0: 0072 8700 0000 72a0 0000 0072 a100 0000  .r....r....r....
-000092d0: 72ca 0000 0072 9800 0000 7222 0000 0072  r....r....r"...r
-000092e0: 5d00 0000 725e 0000 0072 4501 0000 7261  ]...r^...rE...ra
-000092f0: 0000 0072 4601 0000 7247 0100 0072 4801  ...rF...rG...rH.
-00009300: 0000 72bd 0000 0072 3700 0000 7237 0000  ..r....r7...r7..
-00009310: 0072 3800 0000 da0f 6361 7264 5f63 6861  .r8.....card_cha
-00009320: 6e67 655f 5049 4e42 0500 0073 3c00 0000  nge_PINB...s<...
-00009330: 0001 0a01 0601 0601 0401 0401 1801 2a02  ..............*.
-00009340: 1003 1001 1002 1401 0c01 0801 0a01 0a01  ................
-00009350: 1002 1201 0c01 1001 0c01 0a01 0c01 0e01  ................
-00009360: 0a02 1401 1801 0c01 0e01 0802 7a1d 4361  ............z.Ca
-00009370: 7264 436f 6e6e 6563 746f 722e 6361 7264  rdConnector.card
-00009380: 5f63 6861 6e67 655f 5049 4e63 0300 0000  _change_PINc....
-00009390: 0000 0000 1200 0000 0500 0000 4300 0000  ............C...
-000093a0: 7348 0100 0074 006a 0164 0183 0101 0074  sH...t.j.d.....t
-000093b0: 026a 037d 0374 026a 047d 047c 017d 0564  .j.}.t.j.}.|.}.d
-000093c0: 027d 0674 057c 0283 017d 077c 037c 047c  .}.t.|...}.|.|.|
-000093d0: 057c 067c 0767 057c 0217 007d 087c 006a  .|.|.g.|...}.|.j
-000093e0: 067c 0883 015c 037d 097d 0a7d 0b7c 0a64  .|...\.}.}.}.|.d
-000093f0: 036b 0272 947c 0b64 0440 0064 046b 0272  .k.r.|.d.@.d.k.r
-00009400: 947c 006a 077c 0164 0083 0201 007c 0b64  .|.j.|.d.....|.d
-00009410: 0f40 007d 0c64 056a 087c 0c83 017d 0d7c  .@.}.d.j.|...}.|
-00009420: 006a 0964 006b 0972 927c 006a 096a 0a64  .j.d.k.r.|.j.j.d
-00009430: 067c 0d83 0201 006e aa7c 0a64 076b 0272  .|.....n.|.d.k.r
-00009440: f07c 0b64 086b 0272 f07c 006a 077c 0164  .|.d.k.r.|.j.|.d
-00009450: 0083 0201 007c 006a 0b83 005c 047d 0e7d  .....|.j...\.}.}
-00009460: 0f7d 107d 117c 116a 0c64 0964 1083 027d  .}.}.|.j.d.d...}
-00009470: 0c64 056a 087c 0c83 017d 0d7c 006a 0964  .d.j.|...}.|.j.d
-00009480: 006b 0972 ee7c 006a 096a 0a64 067c 0d83  .k.r.|.j.j.d.|..
-00009490: 0201 006e 4e7c 0a64 076b 0290 0172 3e7c  ...nN|.d.k...r>|
-000094a0: 0b64 0b6b 0290 0172 3e64 0c74 0d64 0d7c  .d.k...r>d.t.d.|
-000094b0: 0a14 007c 0b17 0083 019b 0064 0e9d 037d  ...|.......d...}
-000094c0: 0d7c 006a 0964 006b 0990 0172 367c 006a  .|.j.d.k...r6|.j
-000094d0: 096a 0a64 067c 0d83 0201 0074 0e7c 0d83  .j.d.|.....t.|..
-000094e0: 0182 017c 097c 0a7c 0b66 0353 0029 114e  ...|.|.|.f.S.).N
-000094f0: 7a13 496e 2063 6172 645f 756e 626c 6f63  z.In card_unbloc
-00009500: 6b5f 5049 4e72 0100 0000 72cf 0000 0072  k_PINr....r....r
-00009510: 4201 0000 7a1e 5772 6f6e 6720 5055 4b21  B...z.Wrong PUK!
-00009520: 207b 7d20 7472 6965 7320 7265 6d61 696e   {} tries remain
-00009530: 696e 6721 7245 0000 0072 4200 0000 7223  ing!rE...rB...r#
-00009540: 0000 0072 b400 0000 720c 0000 0072 b900  ...r....r....r..
-00009550: 0000 7a6b 546f 6f20 6d61 6e79 2066 6169  ..zkToo many fai
-00009560: 6c65 6420 6174 7465 6d70 7473 2120 596f  led attempts! Yo
-00009570: 7572 2064 6576 6963 6520 6861 7320 6265  ur device has be
-00009580: 656e 2062 6c6f 636b 6564 2120 0a0a 596f  en blocked! ..Yo
-00009590: 7520 6e65 6564 2079 6f75 7220 5055 4b20  u need your PUK 
-000095a0: 636f 6465 2074 6f20 756e 626c 6f63 6b20  code to unblock 
-000095b0: 6974 2028 6572 726f 7220 636f 6465 2072  it (error code r
-000095c0: ba00 0000 72bb 0000 0069 3fff ffff 723a  ....r....i?...r:
-000095d0: 0100 0029 0f72 2700 0000 7234 0000 0072  ...).r'...r4...r
-000095e0: 2b00 0000 72bc 0000 0072 3300 0000 7235  +...r....r3...r5
-000095f0: 0000 0072 9900 0000 72d6 0000 0072 4301  ...r....r....rC.
-00009600: 0000 725a 0000 0072 5b00 0000 7257 0000  ..rZ...r[...rW..
-00009610: 0072 4401 0000 724c 0000 0072 fa00 0000  .rD...rL...r....
-00009620: 2912 7236 0000 0072 7b00 0000 723e 0100  ).r6...r{...r>..
-00009630: 0072 9f00 0000 7287 0000 0072 a000 0000  .r....r....r....
-00009640: 72a1 0000 0072 ca00 0000 7298 0000 0072  r....r....r....r
-00009650: 2200 0000 725d 0000 0072 5e00 0000 7245  "...r]...r^...rE
-00009660: 0100 0072 6100 0000 7246 0100 0072 4701  ...ra...rF...rG.
-00009670: 0000 7248 0100 0072 bd00 0000 7237 0000  ..rH...r....r7..
-00009680: 0072 3700 0000 7238 0000 00da 1063 6172  .r7...r8.....car
-00009690: 645f 756e 626c 6f63 6b5f 5049 4e69 0500  d_unblock_PINi..
-000096a0: 0073 3600 0000 0001 0a01 0601 0601 0401  .s6.............
-000096b0: 0401 0801 1202 1003 1401 0c01 0801 0a01  ................
-000096c0: 0a01 1002 1001 0c01 1001 0c01 0a01 0a01  ................
-000096d0: 1002 1401 1801 0c01 0e01 0802 7a1e 4361  ............z.Ca
-000096e0: 7264 436f 6e6e 6563 746f 722e 6361 7264  rdConnector.card
-000096f0: 5f75 6e62 6c6f 636b 5f50 494e 6301 0000  _unblock_PINc...
-00009700: 0000 0000 000a 0000 0005 0000 0043 0000  .............C..
-00009710: 0073 5600 0000 7400 6a01 6401 8301 0100  .sV...t.j.d.....
-00009720: 7402 6a03 7d01 7402 6a04 7d02 6402 7d03  t.j.}.t.j.}.d.}.
-00009730: 6402 7d04 6402 7d05 7c01 7c02 7c03 7c04  d.}.d.}.|.|.|.|.
-00009740: 7c05 6705 7d06 7c00 6a05 7c06 8301 5c03  |.g.}.|.j.|...\.
-00009750: 7d07 7d08 7d09 7c00 6a06 6402 6400 8302  }.}.}.|.j.d.d...
-00009760: 0100 7c07 7c08 7c09 6603 5300 2903 4e7a  ..|.|.|.f.S.).Nz
-00009770: 1249 6e20 6361 7264 5f6c 6f67 6f75 745f  .In card_logout_
-00009780: 616c 6c72 0100 0000 2907 7227 0000 0072  allr....).r'...r
-00009790: 3400 0000 722b 0000 0072 bc00 0000 5a0e  4...r+...r....Z.
-000097a0: 494e 535f 4c4f 474f 5554 5f41 4c4c 7299  INS_LOGOUT_ALLr.
-000097b0: 0000 0072 d600 0000 290a 7236 0000 0072  ...r....).r6...r
-000097c0: 9f00 0000 7287 0000 0072 a000 0000 72a1  ....r....r....r.
-000097d0: 0000 0072 ca00 0000 7298 0000 0072 2200  ...r....r....r".
-000097e0: 0000 725d 0000 0072 5e00 0000 7237 0000  ..r]...r^...r7..
-000097f0: 0072 3700 0000 7238 0000 00da 0f63 6172  .r7...r8.....car
-00009800: 645f 6c6f 676f 7574 5f61 6c6c 8c05 0000  d_logout_all....
-00009810: 7314 0000 0000 010a 0106 0106 0104 0104  s...............
-00009820: 0104 010e 0210 010c 017a 1d43 6172 6443  .........z.CardC
-00009830: 6f6e 6e65 6374 6f72 2e63 6172 645f 6c6f  onnector.card_lo
-00009840: 676f 7574 5f61 6c6c 6301 0000 0000 0000  gout_allc.......
-00009850: 000d 0000 0005 0000 0043 0000 0073 8800  .........C...s..
-00009860: 0000 7400 6a01 6401 8301 0100 7402 6a03  ..t.j.d.....t.j.
-00009870: 7d01 6402 7d02 6403 7d03 6403 7d04 7404  }.d.}.d.}.d.}.t.
-00009880: 7400 6a05 8300 8301 7c00 5f06 7407 7c00  t.j.....|._.t.|.
-00009890: 6a06 6a08 8301 7d05 7409 7c05 8301 7d06  j.j...}.t.|...}.
-000098a0: 7c01 7c02 7c03 7c04 7c06 6705 7c05 1700  |.|.|.|.|.g.|...
-000098b0: 7d07 7c00 6a0a 7c07 8301 5c03 7d08 7d09  }.|.j.|...\.}.}.
-000098c0: 7d0a 7c00 6a0b 6a0c 7c08 8301 7d0b 7c0b  }.|.j.j.|...}.|.
-000098d0: 6a0d 6404 6405 8d01 7d0c 7c00 6a06 6a0e  j.d.d...}.|.j.j.
-000098e0: 7c0c 8301 0100 7c0b 5300 2906 4e7a 2149  |.....|.S.).Nz!I
-000098f0: 6e20 6361 7264 5f69 6e69 7469 6174 655f  n card_initiate_
-00009900: 7365 6375 7265 5f63 6861 6e6e 656c 2829  secure_channel()
-00009910: 7283 0000 0072 0100 0000 4629 0172 0901  r....r....F).r..
-00009920: 0000 290f 7227 0000 0072 3400 0000 722b  ..).r'...r4...r+
-00009930: 0000 0072 bc00 0000 7212 0000 00da 1167  ...r....r......g
-00009940: 6574 4566 6665 6374 6976 654c 6576 656c  etEffectiveLevel
-00009950: 727a 0000 0072 c600 0000 5a14 7363 5f70  rz...r....Z.sc_p
-00009960: 7562 6b65 795f 7365 7269 616c 697a 6564  ubkey_serialized
-00009970: 7235 0000 0072 9900 0000 7276 0000 005a  r5...r....rv...Z
-00009980: 1d70 6172 7365 5f69 6e69 7469 6174 655f  .parse_initiate_
-00009990: 7365 6375 7265 5f63 6861 6e6e 656c 72e1  secure_channelr.
-000099a0: 0000 005a 1769 6e69 7469 6174 655f 7365  ...Z.initiate_se
-000099b0: 6375 7265 5f63 6861 6e6e 656c 290d 7236  cure_channel).r6
-000099c0: 0000 0072 9f00 0000 7287 0000 0072 a000  ...r....r....r..
-000099d0: 0000 72a1 0000 0072 1101 0000 72ca 0000  ..r....r....r...
-000099e0: 0072 9800 0000 7222 0000 0072 5d00 0000  .r....r"...r]...
-000099f0: 725e 0000 005a 0b70 6565 725f 7075 626b  r^...Z.peer_pubk
-00009a00: 6579 5a11 7065 6572 5f70 7562 6b65 795f  eyZ.peer_pubkey_
-00009a10: 6279 7465 7372 3700 0000 7237 0000 0072  bytesr7...r7...r
-00009a20: 3800 0000 7259 0000 009d 0500 0073 1c00  8...rY.......s..
-00009a30: 0000 0001 0a01 0601 0401 0401 0403 0e01  ................
-00009a40: 0c01 0801 1203 1003 0c01 0c01 0c02 7a2a  ..............z*
-00009a50: 4361 7264 436f 6e6e 6563 746f 722e 6361  CardConnector.ca
-00009a60: 7264 5f69 6e69 7469 6174 655f 7365 6375  rd_initiate_secu
-00009a70: 7265 5f63 6861 6e6e 656c 6302 0000 0000  re_channelc.....
-00009a80: 0000 000c 0000 0009 0000 0043 0000 0073  ...........C...s
-00009a90: 0601 0000 7400 6a01 6401 8301 0100 7402  ....t.j.d.....t.
-00009aa0: 6a03 7d02 6402 7d03 6403 7d04 6403 7d05  j.}.d.}.d.}.d.}.
-00009ab0: 7c01 6404 1900 7402 6a04 7402 6a05 7402  |.d...t.j.t.j.t.
-00009ac0: 6a06 7402 6a07 7402 6a08 7402 6a09 7402  j.t.j.t.j.t.j.t.
-00009ad0: 6a0a 7402 6a0b 6608 6b06 7276 7400 6a01  j.t.j.f.k.rvt.j.
-00009ae0: 6405 740c 7c01 6403 6406 8502 1900 8301  d.t.|.d.d.......
-00009af0: 9b00 740d 7c01 8301 6406 1800 6407 1400  ..t.|...d...d...
-00009b00: 9b00 9d03 8301 0100 6e14 7400 6a01 6405  ........n.t.j.d.
-00009b10: 740c 7c01 8301 9b00 9d02 8301 0100 7c00  t.|...........|.
-00009b20: 6a0e 6a0f 7410 7c01 8301 8301 5c03 7d06  j.j.t.|.....\.}.
-00009b30: 7d07 7d08 7411 7c06 8301 740d 7c07 8301  }.}.t.|...t.|...
-00009b40: 6408 3f00 740d 7c07 8301 6409 4000 6702  d.?.t.|...d.@.g.
-00009b50: 1700 7411 7c07 8301 1700 740d 7c08 8301  ..t.|.....t.|...
-00009b60: 6408 3f00 740d 7c08 8301 6409 4000 6702  d.?.t.|...d.@.g.
-00009b70: 1700 7411 7c08 8301 1700 7d09 740d 7c09  ..t.|.....}.t.|.
-00009b80: 8301 7d0a 7c02 7c03 7c04 7c05 7c0a 6705  ..}.|.|.|.|.|.g.
-00009b90: 7c09 1700 7d0b 7c0b 5300 290a 4e7a 2049  |...}.|.S.).Nz I
-00009ba0: 6e20 6361 7264 5f65 6e63 7279 7074 5f73  n card_encrypt_s
-00009bb0: 6563 7572 655f 6368 616e 6e65 6c28 2972  ecure_channel()r
-00009bc0: 8400 0000 7201 0000 0072 0c00 0000 7a12  ....r....r....z.
-00009bd0: 506c 6169 6e74 6578 7420 432d 4150 4455  Plaintext C-APDU
-00009be0: 3a20 7221 0000 007a 0220 2a72 b200 0000  : r!...z. *r....
-00009bf0: 72d3 0000 0029 1272 2700 0000 7234 0000  r....).r'...r4..
-00009c00: 0072 2b00 0000 72bc 0000 0072 2c00 0000  .r+...r....r,...
-00009c10: 722d 0000 0072 2e00 0000 722f 0000 0072  r-...r....r/...r
-00009c20: 3000 0000 7231 0000 0072 3200 0000 7233  0...r1...r2...r3
-00009c30: 0000 0072 0900 0000 7235 0000 0072 7a00  ...r....r5...rz.
-00009c40: 0000 5a16 656e 6372 7970 745f 7365 6375  ..Z.encrypt_secu
-00009c50: 7265 5f63 6861 6e6e 656c 724b 0000 0072  re_channelrK...r
-00009c60: c600 0000 290c 7236 0000 0072 9800 0000  ....).r6...r....
-00009c70: 729f 0000 0072 8700 0000 72a0 0000 0072  r....r....r....r
-00009c80: a100 0000 72e9 0000 00da 0a63 6970 6865  ....r......ciphe
-00009c90: 7274 6578 74da 036d 6163 72c9 0000 0072  rtext..macr....r
-00009ca0: ca00 0000 5a0e 656e 6372 7970 7465 645f  ....Z.encrypted_
-00009cb0: 6170 6475 7237 0000 0072 3700 0000 7238  apdur7...r7...r8
-00009cc0: 0000 0072 8d00 0000 b405 0000 7320 0000  ...r........s ..
-00009cd0: 0000 010a 0106 0104 0104 0104 030e 0108  ................
-00009ce0: 0108 010e 012e 0214 0216 0148 0108 0212  ...........H....
-00009cf0: 027a 2943 6172 6443 6f6e 6e65 6374 6f72  .z)CardConnector
-00009d00: 2e63 6172 645f 656e 6372 7970 745f 7365  .card_encrypt_se
-00009d10: 6375 7265 5f63 6861 6e6e 656c 6302 0000  cure_channelc...
-00009d20: 0000 0000 0006 0000 0007 0000 0043 0000  .............C..
-00009d30: 0073 c600 0000 7400 6a01 6401 8301 0100  .s....t.j.d.....
-00009d40: 7402 7c01 8301 6402 6b02 721a 7c01 5300  t.|...d.k.r.|.S.
-00009d50: 7402 7c01 8301 6403 6b00 722e 7403 6404  t.|...d.k.r.t.d.
-00009d60: 8301 8201 7404 7c01 6402 6405 8502 1900  ....t.|.d.d.....
-00009d70: 8301 7d02 7c01 6405 1900 6406 4000 6407  ..}.|.d...d.@.d.
-00009d80: 3e00 7c01 6408 1900 6406 4000 1700 7d03  >.|.d...d.@...}.
-00009d90: 7404 7c01 6403 6400 8502 1900 8301 7d04  t.|.d.d.......}.
-00009da0: 7402 7c04 8301 7c03 6b03 72a0 7400 6a05  t.|...|.k.r.t.j.
-00009db0: 6409 7406 7c03 8301 9b00 640a 7406 7402  d.t.|.....d.t.t.
-00009dc0: 7c04 8301 8301 9b00 9d04 8301 0100 7403  |.............t.
-00009dd0: 640b 8301 8201 7c00 6a07 6a08 7c02 7c04  d.....|.j.j.|.|.
-00009de0: 8302 7d05 7400 6a01 640c 7409 7c05 8301  ..}.t.j.d.t.|...
-00009df0: 9b00 9d02 8301 0100 7c05 5300 290d 4e7a  ........|.S.).Nz
-00009e00: 1e49 6e20 6361 7264 5f64 6563 7279 7074  .In card_decrypt
-00009e10: 5f73 6563 7572 655f 6368 616e 6e65 6c72  _secure_channelr
-00009e20: 0100 0000 e912 0000 007a 2445 6e63 7279  .........z$Encry
-00009e30: 7074 6564 2072 6573 706f 6e73 6520 6861  pted response ha
-00009e40: 7320 7772 6f6e 6720 6c65 6e67 6874 2172  s wrong lenght!r
-00009e50: 8800 0000 72d3 0000 0072 b200 0000 e911  ....r....r......
-00009e60: 0000 007a 4649 6e20 6361 7264 5f64 6563  ...zFIn card_dec
-00009e70: 7279 7074 5f73 6563 7572 655f 6368 616e  rypt_secure_chan
-00009e80: 6e65 6c3a 2063 6970 6865 7274 6578 7420  nel: ciphertext 
-00009e90: 6861 7320 7772 6f6e 6720 6c65 6e67 7468  has wrong length
-00009ea0: 3a20 6578 7065 6374 6564 207a 0520 676f  : expected z. go
-00009eb0: 7420 7a1c 4369 7068 6572 7465 7874 2068  t z.Ciphertext h
-00009ec0: 6173 2077 726f 6e67 206c 656e 6768 7421  as wrong lenght!
-00009ed0: 7a12 506c 6169 6e74 6578 7420 522d 4150  z.Plaintext R-AP
-00009ee0: 4455 3a20 290a 7227 0000 0072 3400 0000  DU: ).r'...r4...
-00009ef0: 7235 0000 0072 fa00 0000 724b 0000 0072  r5...r....rK...r
-00009f00: 5400 0000 7275 0000 0072 7a00 0000 5a16  T...ru...rz...Z.
-00009f10: 6465 6372 7970 745f 7365 6375 7265 5f63  decrypt_secure_c
-00009f20: 6861 6e6e 656c 7209 0000 0029 0672 3600  hannelr....).r6.
-00009f30: 0000 7222 0000 0072 e900 0000 723c 0100  ..r"...r....r<..
-00009f40: 0072 4d01 0000 5a09 706c 6169 6e74 6578  .rM...Z.plaintex
-00009f50: 7472 3700 0000 7237 0000 0072 3800 0000  tr7...r7...r8...
-00009f60: 728f 0000 00cc 0500 0073 1c00 0000 0001  r........s......
-00009f70: 0a02 0c01 0401 0c01 0802 1001 1c01 1001  ................
-00009f80: 0c01 2201 0802 0e03 1402 7a29 4361 7264  ..".......z)Card
-00009f90: 436f 6e6e 6563 746f 722e 6361 7264 5f64  Connector.card_d
-00009fa0: 6563 7279 7074 5f73 6563 7572 655f 6368  ecrypt_secure_ch
-00009fb0: 616e 6e65 6c29 0172 c300 0000 6304 0000  annel).r....c...
-00009fc0: 0000 0000 0012 0000 0005 0000 0043 0000  .............C..
-00009fd0: 0073 e000 0000 7400 6a01 6401 8301 0100  .s....t.j.d.....
-00009fe0: 7402 6a03 7d04 6402 7d05 7c01 7d06 7c02  t.j.}.d.}.|.}.|.
-00009ff0: 7d07 7404 7c03 6a05 6403 8301 8301 7d03  }.t.|.j.d.....}.
-0000a000: 7406 7c03 8301 7d08 7c08 6701 7c03 1700  t.|...}.|.g.|...
-0000a010: 7d09 7406 7c09 8301 7d0a 7c04 7c05 7c06  }.t.|...}.|.|.|.
-0000a020: 7c07 7c0a 6705 7c09 1700 7d0b 7c00 6a07  |.|.g.|...}.|.j.
-0000a030: 7c0b 8301 5c03 7d0c 7d0d 7d0e 7c0d 6404  |...\.}.}.}.|.d.
-0000a040: 6b02 72b4 7c0e 6405 6b02 72b4 7c0c 6405  k.r.|.d.k.r.|.d.
-0000a050: 1900 6406 3e00 7c0c 6407 1900 1700 7d0f  ..d.>.|.d.....}.
-0000a060: 7400 6a01 6408 7c0f 9b00 9d02 8301 0100  t.j.d.|.........
-0000a070: 7c0c 6409 640d 8502 1900 7d10 7408 7c10  |.d.d.....}.t.|.
-0000a080: 8301 6a09 8300 7d11 6e1e 7400 6a0a 640b  ..j...}.n.t.j.d.
-0000a090: 7c0d 9b00 640c 7c0e 9b00 9d04 8301 0100  |...d.|.........
-0000a0a0: 6400 7d0f 6400 7d11 7c0c 7c0d 7c0e 7c0f  d.}.d.}.|.|.|.|.
-0000a0b0: 7c11 6605 5300 290e 4e7a 2149 6e20 7365  |.f.S.).Nz!In se
-0000a0c0: 6564 6b65 6570 6572 5f67 656e 6572 6174  edkeeper_generat
-0000a0d0: 655f 6d61 7374 6572 7365 6564 e9a0 0000  e_masterseed....
-0000a0e0: 007a 0575 7466 2d38 7241 0000 0072 0100  .z.utf-8rA...r..
-0000a0f0: 0000 72b2 0000 0072 0c00 0000 7a2b 4d61  ..r....r....z+Ma
-0000a100: 7374 6572 7365 6564 2067 656e 6572 6174  sterseed generat
-0000a110: 6564 2073 7563 6365 7373 6675 6c6c 7920  ed successfully 
-0000a120: 7769 7468 2069 643a 2072 2300 0000 7243  with id: r#...rC
-0000a130: 0000 007a 2445 7272 6f72 2064 7572 696e  ...z$Error durin
-0000a140: 6720 6d61 7374 6572 7365 6564 2067 656e  g masterseed gen
-0000a150: 6572 6174 696f 6e3a 2072 2400 0000 7285  eration: r$...r.
-0000a160: 0000 0029 0b72 2700 0000 7234 0000 0072  ...).r'...r4...r
-0000a170: 2b00 0000 72bc 0000 0072 c600 0000 72c7  +...r....r....r.
-0000a180: 0000 0072 3500 0000 7299 0000 0072 4b00  ...r5...r....rK.
-0000a190: 0000 724c 0000 0072 e200 0000 2912 7236  ..rL...r....).r6
-0000a1a0: 0000 005a 0973 6565 645f 7369 7a65 da0d  ...Z.seed_size..
-0000a1b0: 6578 706f 7274 5f72 6967 6874 7372 c300  export_rightsr..
-0000a1c0: 0000 729f 0000 0072 8700 0000 72a0 0000  ..r....r....r...
-0000a1d0: 0072 a100 0000 72c2 0000 0072 c900 0000  .r....r....r....
-0000a1e0: 72ca 0000 0072 9800 0000 7222 0000 0072  r....r....r"...r
-0000a1f0: 5d00 0000 725e 0000 00da 0269 64da 1066  ]...r^.....id..f
-0000a200: 696e 6765 7270 7269 6e74 5f6c 6973 7472  ingerprint_listr
-0000a210: 1a01 0000 7237 0000 0072 3700 0000 7238  ....r7...r7...r8
-0000a220: 0000 00da 1e73 6565 646b 6565 7065 725f  .....seedkeeper_
-0000a230: 6765 6e65 7261 7465 5f6d 6173 7465 7273  generate_masters
-0000a240: 6565 64e6 0500 0073 2800 0000 0001 0a01  eed....s(.......
-0000a250: 0601 0401 0401 0402 0e01 0801 0a02 0801  ................
-0000a260: 1203 1001 1001 1401 1001 0c01 0e02 1601  ................
-0000a270: 0401 0402 7a2c 4361 7264 436f 6e6e 6563  ....z,CardConnec
-0000a280: 746f 722e 7365 6564 6b65 6570 6572 5f67  tor.seedkeeper_g
-0000a290: 656e 6572 6174 655f 6d61 7374 6572 7365  enerate_masterse
-0000a2a0: 6564 6303 0000 0000 0000 0011 0000 0005  edc.............
-0000a2b0: 0000 0043 0000 0073 e000 0000 7400 6a01  ...C...s....t.j.
-0000a2c0: 6401 8301 0100 7402 6a03 7d03 6402 7d04  d.....t.j.}.d.}.
-0000a2d0: 6403 7d05 7c01 7d06 7404 7c02 6a05 6404  d.}.|.}.t.|.j.d.
-0000a2e0: 8301 8301 7d02 7406 7c02 8301 7d07 7c07  ....}.t.|...}.|.
-0000a2f0: 6701 7c02 1700 7d08 7406 7c08 8301 7d09  g.|...}.t.|...}.
-0000a300: 7c03 7c04 7c05 7c06 7c09 6705 7c08 1700  |.|.|.|.|.g.|...
-0000a310: 7d0a 7c00 6a07 7c0a 8301 5c03 7d0b 7d0c  }.|.j.|...\.}.}.
-0000a320: 7d0d 7c0c 6405 6b02 72b4 7c0d 6403 6b02  }.|.d.k.r.|.d.k.
-0000a330: 72b4 7c0b 6403 1900 6406 3e00 7c0b 6407  r.|.d...d.>.|.d.
-0000a340: 1900 1700 7d0e 7400 6a01 6408 7c0e 9b00  ....}.t.j.d.|...
-0000a350: 9d02 8301 0100 7c0b 6409 640d 8502 1900  ......|.d.d.....
-0000a360: 7d0f 7408 7c0f 8301 6a09 8300 7d10 6e1e  }.t.|...j...}.n.
-0000a370: 7400 6a0a 640b 7c0c 9b00 640c 7c0d 9b00  t.j.d.|...d.|...
-0000a380: 9d04 8301 0100 6400 7d0e 6400 7d10 7c0b  ......d.}.d.}.|.
-0000a390: 7c0c 7c0d 7c0e 7c10 6605 5300 290e 4e7a  |.|.|.|.f.S.).Nz
-0000a3a0: 2149 6e20 7365 6564 6b65 6570 6572 5f67  !In seedkeeper_g
-0000a3b0: 656e 6572 6174 655f 3246 415f 7365 6372  enerate_2FA_secr
-0000a3c0: 6574 e9ae 0000 0072 0100 0000 7a05 7574  et.....r....z.ut
-0000a3d0: 662d 3872 4100 0000 72b2 0000 0072 0c00  f-8rA...r....r..
-0000a3e0: 0000 7a2b 3246 4120 7365 6372 6574 2067  ..z+2FA secret g
-0000a3f0: 656e 6572 6174 6564 2073 7563 6365 7373  enerated success
-0000a400: 6675 6c6c 7920 7769 7468 2069 643a 2072  fully with id: r
-0000a410: 2300 0000 7243 0000 007a 2445 7272 6f72  #...rC...z$Error
-0000a420: 2064 7572 696e 6720 6d61 7374 6572 7365   during masterse
-0000a430: 6564 2067 656e 6572 6174 696f 6e3a 2072  ed generation: r
-0000a440: 2400 0000 7285 0000 0029 0b72 2700 0000  $...r....).r'...
-0000a450: 7234 0000 0072 2b00 0000 72bc 0000 0072  r4...r+...r....r
-0000a460: c600 0000 72c7 0000 0072 3500 0000 7299  ....r....r5...r.
-0000a470: 0000 0072 4b00 0000 724c 0000 0072 e200  ...rK...rL...r..
-0000a480: 0000 2911 7236 0000 0072 5201 0000 72c3  ..).r6...rR...r.
-0000a490: 0000 0072 9f00 0000 7287 0000 0072 a000  ...r....r....r..
-0000a4a0: 0000 72a1 0000 0072 c200 0000 72c9 0000  ..r....r....r...
-0000a4b0: 0072 ca00 0000 7298 0000 0072 2200 0000  .r....r....r"...
-0000a4c0: 725d 0000 0072 5e00 0000 7253 0100 0072  r]...r^...rS...r
-0000a4d0: 5401 0000 721a 0100 0072 3700 0000 7237  T...r....r7...r7
-0000a4e0: 0000 0072 3800 0000 da1e 7365 6564 6b65  ...r8.....seedke
-0000a4f0: 6570 6572 5f67 656e 6572 6174 655f 3246  eper_generate_2F
-0000a500: 415f 7365 6372 6574 0206 0000 7328 0000  A_secret....s(..
-0000a510: 0000 010a 0106 0104 0104 0104 020e 0108  ................
-0000a520: 010a 0208 0112 0310 0110 0114 0110 010c  ................
-0000a530: 010e 0216 0104 0104 027a 2c43 6172 6443  .........z,CardC
-0000a540: 6f6e 6e65 6374 6f72 2e73 6565 646b 6565  onnector.seedkee
-0000a550: 7065 725f 6765 6e65 7261 7465 5f32 4641  per_generate_2FA
-0000a560: 5f73 6563 7265 7463 0300 0000 0000 0000  _secretc........
-0000a570: 1900 0000 0600 0000 4300 0000 7392 0300  ........C...s...
-0000a580: 0074 006a 0164 0183 0101 007c 0264 006b  .t.j.d.....|.d.k
-0000a590: 0872 1664 026e 0264 037d 0374 026a 037d  .r.d.n.d.}.t.j.}
-0000a5a0: 0464 047d 057c 0372 2c64 056e 0264 067d  .d.}.|.r,d.n.d.}
-0000a5b0: 0664 067d 0774 0474 056a 067c 0164 0719  .d.}.t.t.j.|.d..
-0000a5c0: 0064 0864 0085 0219 0083 0183 017d 087c  .d.d.........}.|
-0000a5d0: 087d 097c 0372 8474 0474 056a 067c 0164  .}.|.r.t.t.j.|.d
-0000a5e0: 0919 0083 0183 017d 0a7c 097c 0264 0a3f  .......}.|.|.d.?
-0000a5f0: 0064 0b16 007c 0264 0b16 0067 027c 0a17  .d...|.d...g.|..
-0000a600: 0037 007d 0974 077c 0983 017d 0b7c 047c  .7.}.t.|...}.|.|
-0000a610: 057c 067c 077c 0b67 057c 0917 007d 0c7c  .|.|.|.g.|...}.|
-0000a620: 006a 087c 0c83 015c 037d 0d7d 0e7d 0f7c  .j.|...\.}.}.}.|
-0000a630: 0e64 0c6b 0373 be7c 0f64 0d6b 0372 f474  .d.k.s.|.d.k.r.t
-0000a640: 006a 0964 0e7c 0e64 0b14 007c 0f17 0064  .j.d.|.d...|...d
-0000a650: 0f9b 049d 0283 0101 0074 0a64 1074 0b64  .........t.d.t.d
-0000a660: 0b7c 0e14 007c 0f17 0083 019b 0064 119d  .|...|.......d..
-0000a670: 0383 0182 0164 057d 0764 127d 107c 0390  .....d.}.d.}.|..
-0000a680: 0172 1674 0474 056a 067c 0164 1319 0083  .r.t.t.j.|.d....
-0000a690: 0183 017d 116e 087c 0164 1419 007d 1164  ...}.n.|.d...}.d
-0000a6a0: 0d7d 1274 077c 1183 017d 1378 b87c 137c  .}.t.|...}.x.|.|
-0000a6b0: 106b 0490 0172 e27c 1064 0a3f 007c 1064  .k...r.|.d.?.|.d
-0000a6c0: 0b16 0067 027c 117c 127c 127c 1017 0085  ...g.|.|.|.|....
-0000a6d0: 0219 0017 007d 0974 077c 0983 017d 0b7c  .....}.t.|...}.|
-0000a6e0: 047c 057c 067c 077c 0b67 057c 0917 007d  .|.|.|.|.g.|...}
-0000a6f0: 0c7c 006a 087c 0c83 015c 037d 0d7d 0e7d  .|.j.|...\.}.}.}
-0000a700: 0f7c 0e64 0c6b 0390 0173 947c 0f64 0d6b  .|.d.k...s.|.d.k
-0000a710: 0390 0172 ce74 006a 0964 1574 0b64 0b7c  ...r.t.j.d.t.d.|
-0000a720: 0e14 007c 0f17 0083 019b 0064 119d 0383  ...|.......d....
-0000a730: 0101 0074 0a64 1074 0b64 0b7c 0e14 007c  ...t.d.t.d.|...|
-0000a740: 0f17 0083 019b 0064 119d 0383 0182 017c  .......d.......|
-0000a750: 127c 1037 007d 127c 137c 1038 007d 1390  .|.7.}.|.|.8.}..
-0000a760: 0171 2c57 0064 167d 077c 1364 0a3f 007c  .q,W.d.}.|.d.?.|
-0000a770: 1364 0b16 0067 027c 117c 127c 127c 1317  .d...g.|.|.|.|..
-0000a780: 0085 0219 0017 007d 097c 0390 0272 3274  .......}.|...r2t
-0000a790: 0474 056a 067c 0164 1719 0083 0183 017d  .t.j.|.d.......}
-0000a7a0: 147c 0974 077c 1483 0167 017c 1417 0037  .|.t.|...g.|...7
-0000a7b0: 007d 0974 077c 0983 017d 0b7c 047c 057c  .}.t.|...}.|.|.|
-0000a7c0: 067c 077c 0b67 057c 0917 007d 0c7c 006a  .|.|.g.|...}.|.j
-0000a7d0: 087c 0c83 015c 037d 0d7d 0e7d 0f7c 0e64  .|...\.}.}.}.|.d
-0000a7e0: 186b 0290 0272 ac7c 0f64 196b 0290 0272  .k...r.|.d.k...r
-0000a7f0: ac74 006a 0964 1a74 0b64 0b7c 0e14 007c  .t.j.d.t.d.|...|
-0000a800: 0f17 0083 019b 0064 119d 0383 0101 0074  .......d.......t
-0000a810: 0c64 1b74 0b64 0b7c 0e14 007c 0f17 0083  .d.t.d.|...|....
-0000a820: 019b 0064 119d 0383 0182 016e 4e7c 0e64  ...d.......nN|.d
-0000a830: 0c6b 0390 0273 c07c 0f64 0d6b 0390 0272  .k...s.|.d.k...r
-0000a840: fa74 006a 0964 1c74 0b64 0b7c 0e14 007c  .t.j.d.t.d.|...|
-0000a850: 0f17 0083 019b 0064 119d 0383 0101 0074  .......d.......t
-0000a860: 0a64 1074 0b64 0b7c 0e14 007c 0f17 0083  .d.t.d.|...|....
-0000a870: 019b 0064 119d 0383 0182 017c 127c 1037  ...d.......|.|.7
-0000a880: 007d 1264 0d7d 137c 0d64 0d19 0064 0b14  .}.d.}.|.d...d..
-0000a890: 007c 0d64 0619 0017 007d 157c 0d64 0564  .|.d.....}.|.d.d
-0000a8a0: 1d85 0219 007d 1674 057c 1683 016a 0b83  .....}.t.|...j..
-0000a8b0: 007d 177c 0390 0372 427c 0164 1e19 007d  .}.|...rB|.d...}
-0000a8c0: 186e 1a74 0d6a 0e74 057c 1183 0183 016a  .n.t.j.t.|.....j
-0000a8d0: 0f83 0064 0d64 0a85 0219 007d 187c 187c  ...d.d.....}.|.|
-0000a8e0: 176b 0290 0372 7274 006a 0164 1f83 0101  .k...rrt.j.d....
-0000a8f0: 006e 1874 006a 0964 207c 189b 0064 217c  .n.t.j.d |...d!|
-0000a900: 179b 0064 229d 0583 0101 007c 157c 1766  ...d"......|.|.f
-0000a910: 0253 0029 234e 7a1b 496e 2073 6565 646b  .S.)#Nz.In seedk
-0000a920: 6565 7065 725f 696d 706f 7274 5f73 6563  eeper_import_sec
-0000a930: 7265 7446 54e9 a100 0000 7223 0000 0072  retFT.....r#...r
-0000a940: 0c00 0000 72e8 0000 0072 4300 0000 72e9  ....r....rC...r.
-0000a950: 0000 0072 b200 0000 72ba 0000 0072 4100  ...r....r....rA.
-0000a960: 0000 7201 0000 007a 2645 7272 6f72 2064  ..r....z&Error d
-0000a970: 7572 696e 6720 7365 6372 6574 2069 6d70  uring secret imp
-0000a980: 6f72 7420 2d20 4f50 5f49 4e49 543a 207a  ort - OP_INIT: z
-0000a990: 0430 3e34 587a 3955 6e65 7870 6563 7465  .0>4Xz9Unexpecte
-0000a9a0: 6420 6572 726f 7220 6475 7269 6e67 2073  d error during s
-0000a9b0: 6563 7572 6520 7365 6372 6574 2069 6d70  ecure secret imp
-0000a9c0: 6f72 7420 2865 7272 6f72 2063 6f64 6520  ort (error code 
-0000a9d0: 72bb 0000 0072 9b00 0000 72ea 0000 0072  r....r....r....r
-0000a9e0: f500 0000 7a34 4572 726f 7220 6475 7269  ....z4Error duri
-0000a9f0: 6e67 2073 6563 7265 7420 696d 706f 7274  ng secret import
-0000aa00: 202d 204f 505f 5052 4f43 4553 5320 2865   - OP_PROCESS (e
-0000aa10: 7272 6f72 2063 6f64 6520 72b1 0000 0072  rror code r....r
-0000aa20: eb00 0000 7242 0000 0072 ed00 0000 7a3d  ....rB...r....z=
-0000aa30: 4572 726f 7220 6475 7269 6e67 2073 6563  Error during sec
-0000aa40: 7265 7420 696d 706f 7274 202d 204f 505f  ret import - OP_
-0000aa50: 4649 4e41 4c3a 2077 726f 6e67 206d 6163  FINAL: wrong mac
-0000aa60: 2028 6572 726f 7220 636f 6465 207a 3245   (error code z2E
-0000aa70: 7272 6f72 2064 7572 696e 6720 7365 6372  rror during secr
-0000aa80: 6574 2069 6d70 6f72 743a 2077 726f 6e67  et import: wrong
-0000aa90: 206d 6163 2028 6572 726f 7220 636f 6465   mac (error code
-0000aaa0: 207a 3245 7272 6f72 2064 7572 696e 6720   z2Error during 
-0000aab0: 7365 6372 6574 2069 6d70 6f72 7420 2d20  secret import - 
-0000aac0: 4f50 5f46 494e 414c 2028 6572 726f 7220  OP_FINAL (error 
-0000aad0: 636f 6465 2072 8500 0000 721a 0100 007a  code r....r....z
-0000aae0: 1446 696e 6765 7270 7269 6e74 7320 6d61  .Fingerprints ma
-0000aaf0: 7463 6820 217a 1f46 696e 6765 7270 7269  tch !z.Fingerpri
-0000ab00: 6e74 206d 6973 6d61 7463 683a 2065 7870  nt mismatch: exp
-0000ab10: 6563 7465 6420 7a0f 2062 7574 2072 6563  ected z. but rec
-0000ab20: 6f76 6572 6564 2072 2400 0000 2910 7227  overed r$...).r'
-0000ab30: 0000 0072 3400 0000 722b 0000 0072 bc00  ...r4...r+...r..
-0000ab40: 0000 72c6 0000 0072 4b00 0000 72df 0000  ..r....rK...r...
-0000ab50: 0072 3500 0000 7299 0000 0072 e200 0000  .r5...r....r....
-0000ab60: 72f2 0000 0072 4c00 0000 da0f 5365 6564  r....rL.....Seed
-0000ab70: 4b65 6570 6572 4572 726f 7272 4f00 0000  KeeperErrorrO...
-0000ab80: 7237 0100 0072 5100 0000 2919 7236 0000  r7...rQ...).r6..
-0000ab90: 0072 f400 0000 da0a 7369 645f 7075 626b  .r......sid_pubk
-0000aba0: 6579 5a10 6973 5f73 6563 7572 655f 696d  eyZ.is_secure_im
-0000abb0: 706f 7274 729f 0000 0072 8700 0000 72a0  portr....r....r.
-0000abc0: 0000 0072 a100 0000 72e8 0000 0072 c900  ...r....r....r..
-0000abd0: 0000 72e9 0000 0072 ca00 0000 7298 0000  ..r....r....r...
-0000abe0: 0072 2200 0000 725d 0000 0072 5e00 0000  .r"...r]...r^...
-0000abf0: da0a 6368 756e 6b5f 7369 7a65 72f5 0000  ..chunk_sizer...
-0000ac00: 005a 0d73 6563 7265 745f 6f66 6673 6574  .Z.secret_offset
-0000ac10: 5a10 7365 6372 6574 5f72 656d 6169 6e69  Z.secret_remaini
-0000ac20: 6e67 72eb 0000 0072 5301 0000 7254 0100  ngr....rS...rT..
-0000ac30: 005a 1b66 696e 6765 7270 7269 6e74 5f66  .Z.fingerprint_f
-0000ac40: 726f 6d5f 7365 6564 6b65 6570 6572 da17  rom_seedkeeper..
-0000ac50: 6669 6e67 6572 7072 696e 745f 6672 6f6d  fingerprint_from
-0000ac60: 5f73 6563 7265 7472 3700 0000 7237 0000  _secretr7...r7..
-0000ac70: 0072 3800 0000 da18 7365 6564 6b65 6570  .r8.....seedkeep
-0000ac80: 6572 5f69 6d70 6f72 745f 7365 6372 6574  er_import_secret
-0000ac90: 1e06 0000 7378 0000 0000 010a 0210 0206  ....sx..........
-0000aca0: 0104 010c 0304 011a 0304 0104 0112 011c  ................
-0000acb0: 0108 0112 0110 0110 011a 011c 0304 0104  ................
-0000acc0: 0106 0114 0208 0104 0108 010c 0120 0108  ............. ..
-0000acd0: 0112 0110 0114 011e 011c 0108 010e 0304  ................
-0000ace0: 0120 0106 0112 0112 0108 0112 0110 0114  . ..............
-0000acf0: 011e 011e 0114 011e 011c 0108 0104 0314  ................
-0000ad00: 010c 010c 0106 010a 021a 010a 010c 0218  ................
-0000ad10: 027a 2643 6172 6443 6f6e 6e65 6374 6f72  .z&CardConnector
-0000ad20: 2e73 6565 646b 6565 7065 725f 696d 706f  .seedkeeper_impo
-0000ad30: 7274 5f73 6563 7265 7463 0300 0000 0000  rt_secretc......
-0000ad40: 0000 1800 0000 0600 0000 4300 0000 734e  ..........C...sN
-0000ad50: 0300 0074 006a 0164 0183 0101 007c 0264  ...t.j.d.....|.d
-0000ad60: 006b 0872 1664 026e 0264 037d 0374 026a  .k.r.d.n.d.}.t.j
-0000ad70: 037d 0464 047d 057c 0372 2c64 056e 0264  .}.d.}.|.r,d.n.d
-0000ad80: 067d 0664 067d 077c 0164 073f 0064 0816  .}.d.}.|.d.?.d..
-0000ad90: 007c 0164 0816 0067 027d 087c 0372 647c  .|.d...g.}.|.rd|
-0000ada0: 087c 0264 073f 0064 0816 007c 0264 0816  .|.d.?.d...|.d..
-0000adb0: 0067 0237 007d 0874 047c 0883 017d 097c  .g.7.}.t.|...}.|
-0000adc0: 047c 057c 067c 077c 0967 057c 0817 007d  .|.|.|.|.g.|...}
-0000add0: 0a7c 006a 057c 0a83 015c 037d 0b7d 0c7d  .|.j.|...\.}.}.}
-0000ade0: 0d7c 0c64 096b 0272 a07c 0d64 0a6b 0272  .|.d.k.r.|.d.k.r
-0000adf0: a06e a87c 0c64 0b6b 0272 c47c 0d64 0c6b  .n.|.d.k.r.|.d.k
-0000ae00: 0272 c474 006a 0664 0d83 0101 0074 0764  .r.t.j.d.....t.d
-0000ae10: 0d83 0182 016e 847c 0c64 0b6b 0272 e87c  .....n.|.d.k.r.|
-0000ae20: 0d64 076b 0272 e874 006a 0664 0e83 0101  .d.k.r.t.j.d....
-0000ae30: 0074 0764 0e83 0182 016e 607c 0c64 0b6b  .t.d.....n`|.d.k
-0000ae40: 026f f67c 0d64 0f6b 0290 0172 0e74 006a  .o.|.d.k...r.t.j
-0000ae50: 0664 1083 0101 0074 0764 1083 0182 016e  .d.....t.d.....n
-0000ae60: 3a74 006a 0664 1174 0864 087c 0c14 007c  :t.j.d.t.d.|...|
-0000ae70: 0d17 0083 019b 0064 129d 0383 0101 0074  .......d.......t
-0000ae80: 0964 1174 0864 087c 0c14 007c 0d17 0083  .d.t.d.|...|....
-0000ae90: 019b 0064 129d 0383 0182 017c 006a 0a6a  ...d.......|.j.j
-0000aea0: 0b7c 0b83 017d 0e7c 0390 0172 947c 0b64  .|...}.|...r.|.d
-0000aeb0: 2864 0085 0219 007d 0f74 006a 0164 1474  (d.....}.t.j.d.t
-0000aec0: 0c7c 0f83 016a 0883 0017 0083 0101 007c  .|...j.........|
-0000aed0: 0f7c 0e64 153c 0074 0c7c 0f83 016a 0883  .|.d.<.t.|...j..
-0000aee0: 007c 0e64 163c 0067 007d 1064 057d 077c  .|.d.<.g.}.d.}.|
-0000aef0: 047c 057c 067c 077c 0967 057c 0817 007d  .|.|.|.|.g.|...}
-0000af00: 0a90 0178 067c 006a 057c 0a83 015c 037d  ...x.|.j.|...\.}
-0000af10: 0b7d 0c7d 0d74 047c 0b83 017d 117c 0b64  .}.}.t.|...}.|.d
-0000af20: 0a19 0064 073e 007c 0b64 0619 0017 007d  ...d.>.|.d.....}
-0000af30: 127c 0b64 0564 057c 1217 0085 0219 007d  .|.d.d.|.......}
-0000af40: 137c 107c 1337 007d 107c 1264 0517 007c  .|.|.7.}.|.d...|
-0000af50: 116b 0090 0172 b27c 1264 0517 007d 147c  .k...r.|.d...}.|
-0000af60: 0b7c 1419 0064 073e 007c 0b7c 1464 0617  .|...d.>.|.|.d..
-0000af70: 0019 0017 007d 157c 1464 0537 007d 147c  .....}.|.d.7.}.|
-0000af80: 0b7c 147c 147c 1517 0085 0219 007d 167c  .|.|.|.......}.|
-0000af90: 0e64 1719 007c 1017 007d 177c 1564 186b  .d...|...}.|.d.k
-0000afa0: 0290 0272 6c7c 167c 0e64 193c 0074 0c7c  ...rl|.|.d.<.t.|
-0000afb0: 1683 016a 0883 007c 0e64 1a3c 006e 2c7c  ...j...|.d.<.n,|
-0000afc0: 006a 0a6a 0d7c 177c 167c 006a 0a6a 0e83  .j.j.|.|.|.j.j..
-0000afd0: 0301 007c 167c 0e64 1b3c 0074 0c7c 1683  ...|.|.d.<.t.|..
-0000afe0: 016a 0883 007c 0e64 1c3c 007c 177c 0e64  .j...|.d.<.|.|.d
-0000aff0: 1d3c 0074 0c7c 1783 016a 0883 007c 0e64  .<.t.|...j...|.d
-0000b000: 1e3c 0050 0090 0171 b257 007c 107c 0e64  .<.P...q.W.|.|.d
-0000b010: 1f3c 007c 0390 0272 d874 0c7c 1083 016a  .<.|...r.t.|...j
-0000b020: 0883 007c 0e64 203c 006e 1074 0c7c 1083  ...|.d <.n.t.|..
-0000b030: 016a 0883 007c 0e64 213c 007c 0390 0373  .j...|.d!<.|...s
-0000b040: 4a74 0f6a 1074 0c7c 1083 0183 016a 1183  Jt.j.t.|.....j..
-0000b050: 0064 0a64 0785 0219 007c 0e64 223c 007c  .d.d.....|.d"<.|
-0000b060: 0e64 2219 007c 0e64 2319 006b 0290 0372  .d"..|.d#..k...r
-0000b070: 2a74 006a 0164 2483 0101 006e 2074 006a  *t.j.d$....n t.j
-0000b080: 1264 257c 0e64 2319 009b 0064 267c 0e64  .d%|.d#....d&|.d
-0000b090: 2219 009b 0064 279d 0583 0101 007c 0e53  "....d'......|.S
-0000b0a0: 0029 294e 7a1b 496e 2073 6565 646b 6565  .))Nz.In seedkee
-0000b0b0: 7065 725f 6578 706f 7274 5f73 6563 7265  per_export_secre
-0000b0c0: 7446 54e9 a200 0000 7223 0000 0072 0c00  tFT.....r#...r..
-0000b0d0: 0000 72b2 0000 0072 ba00 0000 7241 0000  ..r....r....rA..
-0000b0e0: 0072 0100 0000 7242 0000 00e9 3100 0000  .r....rB....1...
-0000b0f0: 7a37 4578 706f 7274 2066 6169 6c65 643a  z7Export failed:
-0000b100: 2065 7870 6f72 7420 6e6f 7420 616c 6c6f   export not allo
-0000b110: 7765 6420 6279 2053 6565 644b 6565 7065  wed by SeedKeepe
-0000b120: 7220 706f 6c69 6379 2e7a 1f45 7870 6f72  r policy.z.Expor
-0000b130: 7420 6661 696c 6564 3a20 7365 6372 6574  t failed: secret
-0000b140: 206e 6f74 2066 6f75 6e64 72d1 0000 007a   not foundr....z
-0000b150: 2545 7870 6f72 7420 6661 696c 6564 3a20  %Export failed: 
-0000b160: 6c6f 636b 2065 7272 6f72 202d 2074 7279  lock error - try
-0000b170: 2061 6761 696e 7a1d 556e 6578 7065 6374   againz.Unexpect
-0000b180: 6564 2065 7272 6f72 2028 6572 726f 7220  ed error (error 
-0000b190: 636f 6465 2072 bb00 0000 7288 0000 007a  code r....r....z
-0000b1a0: 0349 563a 5a07 6976 5f6c 6973 7472 e900  .IV:Z.iv_listr..
-0000b1b0: 0000 da0b 6865 6164 6572 5f6c 6973 7472  ....header_listr
-0000b1c0: 0701 0000 5a09 686d 6163 5f6c 6973 7472  ....Z.hmac_listr
-0000b1d0: eb00 0000 5a09 7369 676e 5f6c 6973 74da  ....Z.sign_list.
-0000b1e0: 0473 6967 6e5a 0e66 756c 6c5f 6461 7461  .signZ.full_data
-0000b1f0: 5f6c 6973 74da 0966 756c 6c5f 6461 7461  _list..full_data
-0000b200: 72f5 0000 0072 ea00 0000 da06 7365 6372  r....r......secr
-0000b210: 6574 725c 0100 0072 1a01 0000 7a14 4669  etr\...r....z.Fi
-0000b220: 6e67 6572 7072 696e 7473 206d 6174 6368  ngerprints match
-0000b230: 2021 7a1f 4669 6e67 6572 7072 696e 7420   !z.Fingerprint 
-0000b240: 6d69 736d 6174 6368 3a20 6578 7065 6374  mismatch: expect
-0000b250: 6564 207a 0f20 6275 7420 7265 636f 7665  ed z. but recove
-0000b260: 7265 6420 7224 0000 0069 f0ff ffff 2913  red r$...i....).
-0000b270: 7227 0000 0072 3400 0000 722b 0000 0072  r'...r4...r+...r
-0000b280: bc00 0000 7235 0000 0072 9900 0000 7254  ....r5...r....rT
-0000b290: 0000 0072 5901 0000 724c 0000 0072 f200  ...rY...rL...r..
-0000b2a0: 0000 7276 0000 00da 1770 6172 7365 5f73  ..rv.....parse_s
-0000b2b0: 6565 646b 6565 7065 725f 6865 6164 6572  eedkeeper_header
-0000b2c0: 724b 0000 005a 1076 6572 6966 795f 7369  rK...Z.verify_si
-0000b2d0: 676e 6174 7572 6572 a400 0000 724f 0000  gnaturer....rO..
-0000b2e0: 0072 3701 0000 7251 0000 0072 e200 0000  .r7...rQ...r....
-0000b2f0: 2918 7236 0000 005a 0373 6964 725a 0100  ).r6...Z.sidrZ..
-0000b300: 005a 1069 735f 7365 6375 7265 5f65 7870  .Z.is_secure_exp
-0000b310: 6f72 7472 9f00 0000 7287 0000 0072 a000  ortr....r....r..
-0000b320: 0000 72a1 0000 0072 c900 0000 72ca 0000  ..r....r....r...
-0000b330: 0072 9800 0000 7222 0000 0072 5d00 0000  .r....r"...r]...
-0000b340: 725e 0000 00da 0b73 6563 7265 745f 6469  r^.....secret_di
-0000b350: 6374 72e9 0000 0072 6301 0000 5a0d 7265  ctr....rc...Z.re
-0000b360: 7370 6f6e 7365 5f73 697a 6572 5b01 0000  sponse_sizer[...
-0000b370: 7222 0100 00da 066f 6666 7365 745a 0973  r".....offsetZ.s
-0000b380: 6967 6e5f 7369 7a65 7261 0100 0072 6201  ign_sizera...rb.
-0000b390: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
-0000b3a0: 00da 1873 6565 646b 6565 7065 725f 6578  ...seedkeeper_ex
-0000b3b0: 706f 7274 5f73 6563 7265 746c 0600 0073  port_secretl...s
-0000b3c0: 8200 0000 0001 0a02 1002 0601 0401 0c01  ................
-0000b3d0: 0402 1401 0401 1801 0801 1203 1001 1001  ................
-0000b3e0: 0201 1001 0a01 0a01 1001 0a01 0a01 1201  ................
-0000b3f0: 0a02 0a02 1e01 1c03 0c02 0601 0c01 1601  ................
-0000b400: 0801 1002 0401 0401 1201 0402 1002 0801  ................
-0000b410: 1401 1001 0803 0e01 0801 1801 0801 1003  ................
-0000b420: 0c01 0a01 0801 1202 1401 0801 1001 0801  ................
-0000b430: 1001 0801 0801 0601 1202 1005 0601 1e01  ................
-0000b440: 1201 0c02 2002 7a26 4361 7264 436f 6e6e  .... .z&CardConn
-0000b450: 6563 746f 722e 7365 6564 6b65 6570 6572  ector.seedkeeper
-0000b460: 5f65 7870 6f72 745f 7365 6372 6574 6301  _export_secretc.
-0000b470: 0000 0000 0000 000b 0000 0005 0000 0043  ...............C
-0000b480: 0000 0073 2401 0000 7400 6a01 6401 8301  ...s$...t.j.d...
-0000b490: 0100 7402 6a03 7d01 6402 7d02 6403 7d03  ..t.j.}.d.}.d.}.
-0000b4a0: 6700 7d04 6404 7d05 7c01 7c02 7c03 7c05  g.}.d.}.|.|.|.|.
-0000b4b0: 6704 7d06 7c00 6a04 7c06 8301 5c03 7d07  g.}.|.j.|...\.}.
-0000b4c0: 7d08 7d09 784a 7c08 6405 6b02 7286 7c09  }.}.xJ|.d.k.r.|.
-0000b4d0: 6403 6b02 7286 7c00 6a05 6a06 7c07 8301  d.k.r.|.j.j.|...
-0000b4e0: 7d0a 7c04 7c0a 6701 3700 7d04 6406 7d05  }.|.|.g.7.}.d.}.
-0000b4f0: 7c01 7c02 7c03 7c05 6704 7d06 7c00 6a04  |.|.|.|.g.}.|.j.
-0000b500: 7c06 8301 5c03 7d07 7d08 7d09 713e 5700  |...\.}.}.}.q>W.
-0000b510: 7c08 6405 6b02 729a 7c09 6403 6b02 729a  |.d.k.r.|.d.k.r.
-0000b520: 6e86 7c08 6407 6b02 72b6 7c09 6408 6b02  n.|.d.k.r.|.d.k.
-0000b530: 72b6 7400 6a01 6409 8301 0100 6e6a 7c08  r.t.j.d.....nj|.
-0000b540: 6407 6b02 72e6 7c09 640a 6b02 72e6 7400  d.k.r.|.d.k.r.t.
-0000b550: 6a07 640b 7c08 9b00 640c 7c09 9b00 9d04  j.d.|...d.|.....
-0000b560: 8301 0100 7408 640d 8301 8201 6e3a 7400  ....t.d.....n:t.
-0000b570: 6a07 640e 7409 640f 7c08 1400 7c09 1700  j.d.t.d.|...|...
-0000b580: 8301 9b00 6410 9d03 8301 0100 740a 640e  ....d.......t.d.
-0000b590: 7409 640f 7c08 1400 7c09 1700 8301 9b00  t.d.|...|.......
-0000b5a0: 6410 9d03 8301 8201 7c04 5300 2911 4e7a  d.......|.S.).Nz
-0000b5b0: 2149 6e20 7365 6564 6b65 6570 6572 5f6c  !In seedkeeper_l
-0000b5c0: 6973 745f 7365 6372 6574 5f68 6561 6465  ist_secret_heade
-0000b5d0: 7273 e9a6 0000 0072 0100 0000 720c 0000  rs.....r....r...
-0000b5e0: 0072 4100 0000 7223 0000 0072 4200 0000  .rA...r#...rB...
-0000b5f0: 724f 0100 007a 184e 6f20 6d6f 7265 206f  rO...z.No more o
-0000b600: 626a 6563 7420 696e 206d 656d 6f72 7972  bject in memoryr
-0000b610: 4300 0000 7a2e 556e 696e 6974 6961 6c69  C...z.Uninitiali
-0000b620: 7a65 6453 6565 6445 7272 6f72 2064 7572  zedSeedError dur
-0000b630: 696e 6720 6f62 6a65 6374 206c 6973 7469  ing object listi
-0000b640: 6e67 3a20 7224 0000 007a 1e53 6565 644b  ng: r$...z.SeedK
-0000b650: 6565 7065 7220 6973 206e 6f74 2069 6e69  eeper is not ini
-0000b660: 7469 616c 697a 6564 217a 3355 6e65 7870  tialized!z3Unexp
-0000b670: 6563 7465 6420 6572 726f 7220 6475 7269  ected error duri
-0000b680: 6e67 206f 626a 6563 7420 6c69 7374 696e  ng object listin
-0000b690: 6720 2865 7272 6f72 2063 6f64 6520 72ba  g (error code r.
-0000b6a0: 0000 0072 bb00 0000 290b 7227 0000 0072  ...r....).r'...r
-0000b6b0: 3400 0000 722b 0000 0072 bc00 0000 7299  4...r+...r....r.
-0000b6c0: 0000 0072 7600 0000 7264 0100 0072 5400  ...rv...rd...rT.
-0000b6d0: 0000 7202 0100 0072 4c00 0000 72f2 0000  ..r....rL...r...
-0000b6e0: 0029 0b72 3600 0000 729f 0000 0072 8700  .).r6...r....r..
-0000b6f0: 0000 72a0 0000 005a 0768 6561 6465 7273  ..r....Z.headers
-0000b700: 72a1 0000 0072 9800 0000 7222 0000 0072  r....r....r"...r
-0000b710: 5d00 0000 725e 0000 0072 6501 0000 7237  ]...r^...re...r7
-0000b720: 0000 0072 3700 0000 7238 0000 00da 1e73  ...r7...r8.....s
-0000b730: 6565 646b 6565 7065 725f 6c69 7374 5f73  eedkeeper_list_s
-0000b740: 6563 7265 745f 6865 6164 6572 73c8 0600  ecret_headers...
-0000b750: 0073 3000 0000 0001 0a01 0601 0401 0403  .s0.............
-0000b760: 0401 0401 0c01 1002 1201 0c01 0a04 0401  ................
-0000b770: 0c01 1402 1001 0201 1001 0c01 1001 1601  ................
-0000b780: 0a02 1e01 1c02 7a2c 4361 7264 436f 6e6e  ......z,CardConn
-0000b790: 6563 746f 722e 7365 6564 6b65 6570 6572  ector.seedkeeper
-0000b7a0: 5f6c 6973 745f 7365 6372 6574 5f68 6561  _list_secret_hea
-0000b7b0: 6465 7273 6302 0000 0000 0000 0015 0000  dersc...........
-0000b7c0: 000d 0000 0043 0000 0073 f602 0000 7400  .....C...s....t.
-0000b7d0: 6a01 6401 8301 0100 7402 6a03 7d02 6402  j.d.....t.j.}.d.
-0000b7e0: 7d03 6403 7d04 6404 7d05 7c02 7c03 7c04  }.d.}.d.}.|.|.|.
-0000b7f0: 7c05 6704 7d06 7c00 6a04 7c06 8301 5c03  |.g.}.|.j.|...\.
-0000b800: 7d07 7d08 7d09 6700 7d0a 6405 7d0b 7c08  }.}.}.g.}.d.}.|.
-0000b810: 6406 6b02 6f4e 7c09 6403 6b02 9001 7204  d.k.oN|.d.k...r.
-0000b820: 7c07 6403 1900 6407 1400 7c07 6404 1900  |.d...d...|.d...
-0000b830: 1700 7d0c 7c07 6408 1900 6407 1400 7c07  ..}.|.d...d...|.
-0000b840: 6409 1900 1700 7d0d 7400 6a01 640a 7405  d.....}.t.j.d.t.
-0000b850: 7c0c 8301 1700 8301 0100 7400 6a01 640b  |.........t.j.d.
-0000b860: 7405 7c0d 8301 1700 8301 0100 7406 7c07  t.|.........t.|.
-0000b870: 8301 640c 7c0b 1700 6b05 72f8 7c00 6a07  ..d.|...k.r.|.j.
-0000b880: 6a08 7c07 640c 640c 7c0b 1700 8502 1900  j.|.d.d.|.......
-0000b890: 8301 5c04 7d0e 7d0f 7d10 7d11 7c0a 7c0e  ..\.}.}.}.}.|.|.
-0000b8a0: 7c0f 7c10 7c11 6704 6701 1700 7d0a 7400  |.|.|.g.g...}.t.
-0000b8b0: 6a01 640d 7405 7c0a 6403 1900 8301 1700  j.d.t.|.d.......
-0000b8c0: 8301 0100 6e0a 7400 6a01 640e 8301 0100  ....n.t.j.d.....
-0000b8d0: 6e6e 7c08 640f 6b02 9001 7238 7c09 640c  nn|.d.k...r8|.d.
-0000b8e0: 6b02 9001 7238 7400 6a09 6410 7c08 9b00  k...r8t.j.d.|...
-0000b8f0: 6411 7c09 9b00 9d04 8301 0100 740a 6412  d.|.........t.d.
-0000b900: 8301 8201 6e3a 7400 6a09 6413 740b 6407  ....n:t.j.d.t.d.
-0000b910: 7c08 1400 7c09 1700 8301 9b00 6414 9d03  |...|.......d...
-0000b920: 8301 0100 740c 6413 740b 6407 7c08 1400  ....t.d.t.d.|...
-0000b930: 7c09 1700 8301 9b00 6414 9d03 8301 8201  |.......d.......
-0000b940: 6408 7d05 7c02 7c03 7c04 7c05 6704 7d06  d.}.|.|.|.|.g.}.
-0000b950: 6403 7d12 78ce 7c01 9002 7254 7c08 6406  d.}.x.|...rT|.d.
-0000b960: 6b02 9002 7254 7c09 6403 6b02 9002 7254  k...rT|.d.k...rT
-0000b970: 7c00 6a04 7c06 8301 5c03 7d07 7d08 7d09  |.j.|...\.}.}.}.
-0000b980: 7406 7c07 8301 6403 6b02 9001 72c2 5000  t.|...d.k...r.P.
-0000b990: 7868 7406 7c07 8301 7c0b 6b05 9002 722a  xht.|...|.k...r*
-0000b9a0: 7c00 6a07 6a08 7c07 6403 7c0b 8502 1900  |.j.j.|.d.|.....
-0000b9b0: 8301 5c04 7d0e 7d0f 7d10 7d11 7400 6a01  ..\.}.}.}.}.t.j.
-0000b9c0: 6415 7405 7c0e 7c0f 7c10 7c11 6704 8301  d.t.|.|.|.|.g...
-0000b9d0: 1700 8301 0100 7c0a 7c0e 7c0f 7c10 7c11  ......|.|.|.|.|.
-0000b9e0: 6704 6701 1700 7d0a 7c07 7c0b 6400 8502  g.g...}.|.|.d...
-0000b9f0: 1900 7d07 9001 71c4 5700 7c12 6404 3700  ..}...q.W.|.d.7.
-0000ba00: 7d12 7c12 6416 6b04 9001 7288 7400 6a09  }.|.d.k...r.t.j.
-0000ba10: 6417 7c12 9b00 9d02 8301 0100 5000 9001  d.|.........P...
-0000ba20: 7188 5700 7c08 6406 6b03 9002 736a 7c09  q.W.|.d.k...sj|.
-0000ba30: 6403 6b03 9002 7280 7400 6a09 6418 7c08  d.k...r.t.j.d.|.
-0000ba40: 9b00 6411 7c09 9b00 9d04 8301 0100 7400  ..d.|.........t.
-0000ba50: 6a01 6419 7406 7c0a 8301 9b00 9d02 8301  j.d.t.|.........
-0000ba60: 0100 6403 7d13 7852 7c0a 4400 5d4a 7d14  ..d.}.xR|.D.]J}.
-0000ba70: 7c14 5c04 7d0e 7d0f 7d10 7d11 7400 6a01  |.\.}.}.}.}.t.j.
-0000ba80: 641a 7c13 9b00 641b 740b 7c0e 8301 9b00  d.|...d.t.|.....
-0000ba90: 6411 7c0f 9b00 6411 7c10 9b00 6411 740b  d.|...d.|...d.t.
-0000baa0: 7c11 8301 9b00 9d0a 8301 0100 7c13 6404  |...........|.d.
-0000bab0: 3700 7d13 9002 719e 5700 7c0a 7c0c 7c0d  7.}...q.W.|.|.|.
-0000bac0: 6603 5300 291c 4e7a 1849 6e20 7365 6564  f.S.).Nz.In seed
-0000bad0: 6b65 6570 6572 5f70 7269 6e74 5f6c 6f67  keeper_print_log
-0000bae0: 73e9 a900 0000 7201 0000 0072 0c00 0000  s.....r....r....
-0000baf0: 72b5 0000 0072 4100 0000 72ba 0000 0072  r....rA...r....r
-0000bb00: 2300 0000 72b1 0000 007a 0e6e 6274 6f74  #...r....z.nbtot
-0000bb10: 616c 5f6c 6f67 733a 207a 0e6e 6261 7661  al_logs: z.nbava
-0000bb20: 696c 5f6c 6f67 733a 2072 4300 0000 7a0c  il_logs: rC...z.
-0000bb30: 4c61 7465 7374 206c 6f67 3a20 7a12 4e6f  Latest log: z.No
-0000bb40: 206c 6f67 7320 6176 6169 6c61 626c 6521   logs available!
-0000bb50: 7242 0000 007a 2e55 6e69 6e69 7469 616c  rB...z.Uninitial
-0000bb60: 697a 6564 5365 6564 4572 726f 7220 6475  izedSeedError du
-0000bb70: 7269 6e67 206f 626a 6563 7420 6c69 7374  ring object list
-0000bb80: 696e 673a 2072 2400 0000 7a1e 5365 6564  ing: r$...z.Seed
-0000bb90: 4b65 6570 6572 2069 7320 6e6f 7420 696e  Keeper is not in
-0000bba0: 6974 6961 6c69 7a65 6421 7a33 556e 6578  itialized!z3Unex
-0000bbb0: 7065 6374 6564 2065 7272 6f72 2064 7572  pected error dur
-0000bbc0: 696e 6720 6f62 6a65 6374 206c 6973 7469  ing object listi
-0000bbd0: 6e67 2028 6572 726f 7220 636f 6465 2072  ng (error code r
-0000bbe0: bb00 0000 7a0a 4e65 7874 206c 6f67 3a20  ....z.Next log: 
-0000bbf0: 726e 0000 007a 2643 6f75 6e74 6572 2065  rn...z&Counter e
-0000bc00: 7863 6565 6465 6420 6475 7269 6e67 206c  xceeded during l
-0000bc10: 6f67 2070 7269 6e74 696e 673a 207a 1b45  og printing: z.E
-0000bc20: 7272 6f72 2064 7572 696e 6720 6c6f 6720  rror during log 
-0000bc30: 7072 696e 7469 6e67 3a20 7a0b 4c4f 4753  printing: z.LOGS
-0000bc40: 2073 697a 653a 207a 0769 6e64 6578 3a20   size: z.index: 
-0000bc50: 7a03 207c 2029 0d72 2700 0000 7234 0000  z. | ).r'...r4..
-0000bc60: 0072 2b00 0000 72bc 0000 0072 9900 0000  .r+...r....r....
-0000bc70: 7275 0000 0072 3500 0000 7276 0000 005a  ru...r5...rv...Z
-0000bc80: 1470 6172 7365 5f73 6565 646b 6565 7065  .parse_seedkeepe
-0000bc90: 725f 6c6f 6772 5400 0000 7202 0100 0072  r_logrT...r....r
-0000bca0: 4c00 0000 72f2 0000 0029 1572 3600 0000  L...r....).r6...
-0000bcb0: 5a09 7072 696e 745f 616c 6c72 9f00 0000  Z.print_allr....
-0000bcc0: 7287 0000 0072 a000 0000 72a1 0000 0072  r....r....r....r
-0000bcd0: 9800 0000 7222 0000 0072 5d00 0000 725e  ....r"...r]...r^
-0000bce0: 0000 005a 046c 6f67 735a 086c 6f67 5f73  ...Z.logsZ.log_s
-0000bcf0: 697a 655a 0c6e 6274 6f74 616c 5f6c 6f67  izeZ.nbtotal_log
-0000bd00: 735a 0c6e 6261 7661 696c 5f6c 6f67 735a  sZ.nbavail_logsZ
-0000bd10: 056f 7069 6e73 5a03 6964 315a 0369 6432  .opinsZ.id1Z.id2
-0000bd20: da03 7265 735a 0763 6f75 6e74 6572 72db  ..resZ.counterr.
-0000bd30: 0000 00da 036c 6f67 7237 0000 0072 3700  .....logr7...r7.
-0000bd40: 0000 7238 0000 00da 1573 6565 646b 6565  ..r8.....seedkee
-0000bd50: 7065 725f 7072 696e 745f 6c6f 6773 eb06  per_print_logs..
-0000bd60: 0000 7362 0000 0000 010a 0106 0104 0104  ..sb............
-0000bd70: 0304 010c 0110 0304 0104 0112 0114 0114  ................
-0000bd80: 0112 0112 0110 0120 0112 0118 020c 0114  ....... ........
-0000bd90: 0116 010a 021e 011c 0304 010c 0104 011c  ................
-0000bda0: 0210 010e 0102 0210 011c 011a 0112 0112  ................
-0000bdb0: 0208 010a 0110 0108 0214 0116 0314 0104  ................
-0000bdc0: 010a 010c 0130 010e 027a 2343 6172 6443  .....0...z#CardC
-0000bdd0: 6f6e 6e65 6374 6f72 2e73 6565 646b 6565  onnector.seedkee
-0000bde0: 7065 725f 7072 696e 745f 6c6f 6773 6304  per_print_logsc.
-0000bdf0: 0000 0000 0000 0011 0000 000a 0000 0043  ...............C
-0000be00: 0000 0073 cc00 0000 6401 6402 6403 6404  ...s....d.d.d.d.
-0000be10: 6405 6405 6406 6407 6408 6409 9c09 7d04  d.d.d.d.d.d...}.
-0000be20: 640a 640b 640c 9c02 7d05 640b 6404 6701  d.d.d...}.d.d.g.
-0000be30: 1400 7d06 7400 7c01 8301 7401 6b08 7242  ..}.t.|...t.k.rB
-0000be40: 7c04 7c01 1900 7d07 6e04 7c01 7d07 6404  |.|...}.n.|.}.d.
-0000be50: 7d08 7400 7c02 8301 7401 6b08 7260 7c05  }.t.|...t.k.r`|.
-0000be60: 7c02 1900 7d09 6e04 7c02 7d09 640d 6404  |...}.n.|.}.d.d.
-0000be70: 6701 1400 7d0a 640e 6404 6701 1400 7d0b  g...}.d.d.g...}.
-0000be80: 640b 6404 6701 1400 7d0c 7402 7c03 8301  d.d.g...}.t.|...
-0000be90: 7d0d 7403 7c03 6a04 640f 8301 8301 7d0e  }.t.|.j.d.....}.
-0000bea0: 7c06 7c07 7c08 7c09 6703 1700 7c0a 1700  |.|.|.|.g...|...
-0000beb0: 7c0b 1700 7c0c 1700 7c0d 6701 1700 7c0e  |...|...|.g...|.
-0000bec0: 1700 7d0f 7405 7c0f 8301 6a06 8300 7d10  ..}.t.|...j...}.
-0000bed0: 7c10 5300 2910 4e72 d100 0000 720c 0100  |.S.).Nr....r...
-0000bee0: 0072 8800 0000 7201 0000 0072 6c00 0000  .r....r....rl...
-0000bef0: 7241 0000 0072 5101 0000 72f0 0000 0029  rA...rQ...r....)
-0000bf00: 097a 0e42 4950 3339 206d 6e65 6d6f 6e69  .z.BIP39 mnemoni
-0000bf10: 637a 1145 6c65 6374 7275 6d20 6d6e 656d  cz.Electrum mnem
-0000bf20: 6f6e 6963 5a0a 4d61 7374 6572 7365 6564  onicZ.Masterseed
-0000bf30: 7a17 5365 6375 7265 2069 6d70 6f72 7420  z.Secure import 
-0000bf40: 6672 6f6d 206a 736f 6e7a 0a50 7562 6c69  from jsonz.Publi
-0000bf50: 6320 4b65 797a 1b41 7574 6865 6e74 696b  c Keyz.Authentik
-0000bf60: 6579 2066 726f 6d20 5472 7573 7453 746f  ey from TrustSto
-0000bf70: 7265 5a08 5061 7373 776f 7264 7a17 4175  reZ.Passwordz.Au
-0000bf80: 7468 656e 7469 6b65 7920 6365 7274 6966  thentikey certif
-0000bf90: 6963 6174 657a 0a32 4641 2073 6563 7265  icatez.2FA secre
-0000bfa0: 7472 0c00 0000 7223 0000 0029 027a 1b45  tr....r#...).z.E
-0000bfb0: 7870 6f72 7420 696e 2070 6c61 696e 7465  xport in plainte
-0000bfc0: 7874 2061 6c6c 6f77 6564 7a15 4578 706f  xt allowedz.Expo
-0000bfd0: 7274 2065 6e63 7279 7074 6564 206f 6e6c  rt encrypted onl
-0000bfe0: 7972 b100 0000 7243 0000 0072 bf00 0000  yr....rC...r....
-0000bff0: 2907 7226 0000 0072 7500 0000 7235 0000  ).r&...ru...r5..
-0000c000: 0072 c600 0000 72c7 0000 0072 4b00 0000  .r....r....rK...
-0000c010: 724c 0000 0029 1172 3600 0000 72f6 0000  rL...).r6...r...
-0000c020: 0072 5201 0000 72c3 0000 005a 0864 6963  .rR...r....Z.dic
-0000c030: 5f74 7970 655a 1164 6963 5f65 7870 6f72  _typeZ.dic_expor
-0000c040: 745f 7269 6768 7473 7253 0100 005a 0569  t_rightsrS...Z.i
-0000c050: 7479 7065 da06 6f72 6967 696e 5a06 6578  type..originZ.ex
-0000c060: 706f 7274 5a0f 6578 706f 7274 5f63 6f75  portZ.export_cou
-0000c070: 6e74 6572 7372 1a01 0000 5a03 7266 7572  ntersr....Z.rfur
-0000c080: c200 0000 72c8 0000 0072 6001 0000 5a0a  ....r....r`...Z.
-0000c090: 6865 6164 6572 5f68 6578 7237 0000 0072  header_hexr7...r
-0000c0a0: 3700 0000 7238 0000 00da 0b6d 616b 655f  7...r8.....make_
-0000c0b0: 6865 6164 6572 2d07 0000 7326 0000 0000  header-...s&....
-0000c0c0: 0108 0110 010a 010a 010c 010a 0204 0104  ................
-0000c0d0: 010c 010a 0204 010a 010a 010a 0108 010e  ................
-0000c0e0: 0124 010c 017a 1943 6172 6443 6f6e 6e65  .$...z.CardConne
-0000c0f0: 6374 6f72 2e6d 616b 655f 6865 6164 6572  ctor.make_header
-0000c100: 6301 0000 0000 0000 0009 0000 0005 0000  c...............
-0000c110: 0043 0000 0073 ae00 0000 7400 6a01 6401  .C...s....t.j.d.
-0000c120: 8301 0100 7402 6a03 7d01 7402 6a04 7d02  ....t.j.}.t.j.}.
-0000c130: 6402 7d03 6402 7d04 7c01 7c02 7c03 7c04  d.}.d.}.|.|.|.|.
-0000c140: 6704 7d05 7c00 6a05 7c05 8301 5c03 7d06  g.}.|.j.|...\.}.
-0000c150: 7d07 7d08 7c07 6403 6b02 724c 7c08 6402  }.}.|.d.k.rL|.d.
-0000c160: 6b02 724c 6e5e 7c07 6404 6b02 7270 7c08  k.rLn^|.d.k.rp|.
-0000c170: 6402 6b02 7270 7400 6a06 6405 8301 0100  d.k.rpt.j.d.....
-0000c180: 7407 6406 8301 8201 6e3a 7400 6a06 6407  t.d.....n:t.j.d.
-0000c190: 7408 6408 7c07 1400 7c08 1700 8301 9b00  t.d.|...|.......
-0000c1a0: 6409 9d03 8301 0100 7409 6407 7408 6408  d.......t.d.t.d.
-0000c1b0: 7c07 1400 7c08 1700 8301 9b00 6409 9d03  |...|.......d...
-0000c1c0: 8301 8201 7c06 5300 290a 4e7a 1b49 6e20  ....|.S.).Nz.In 
-0000c1d0: 6361 7264 5f65 7870 6f72 745f 7065 7273  card_export_pers
-0000c1e0: 6f5f 7075 626b 6579 7201 0000 0072 4100  o_pubkeyr....rA.
-0000c1f0: 0000 7272 0000 007a 4645 7272 6f72 2064  ..rr...zFError d
-0000c200: 7572 696e 6720 7065 7273 6f6e 616c 697a  uring personaliz
-0000c210: 6174 696f 6e20 7075 626b 6579 2065 7870  ation pubkey exp
-0000c220: 6f72 743a 2063 6f6d 6d61 6e64 2075 6e73  ort: command uns
-0000c230: 7570 706f 7274 6564 2830 7836 4430 307a  upported(0x6D00z
-0000c240: 4845 7272 6f72 2064 7572 696e 6720 7065  HError during pe
-0000c250: 7273 6f6e 616c 697a 6174 696f 6e20 7075  rsonalization pu
-0000c260: 626b 6579 2065 7870 6f72 743a 2063 6f6d  bkey export: com
-0000c270: 6d61 6e64 2075 6e73 7570 706f 7274 6564  mand unsupported
-0000c280: 2028 3078 3644 3030 297a 3745 7272 6f72   (0x6D00)z7Error
-0000c290: 2064 7572 696e 6720 7065 7273 6f6e 616c   during personal
-0000c2a0: 697a 6174 696f 6e20 7075 626b 6579 2065  ization pubkey e
-0000c2b0: 7870 6f72 7420 2865 7272 6f72 2063 6f64  xport (error cod
-0000c2c0: 6520 72ba 0000 0072 bb00 0000 290a 7227  e r....r....).r'
-0000c2d0: 0000 0072 3400 0000 722b 0000 0072 bc00  ...r4...r+...r..
-0000c2e0: 0000 5a15 494e 535f 4558 504f 5254 5f50  ..Z.INS_EXPORT_P
-0000c2f0: 4b49 5f50 5542 4b45 5972 9900 0000 72e2  KI_PUBKEYr....r.
-0000c300: 0000 0072 e300 0000 724c 0000 0072 f200  ...r....rL...r..
-0000c310: 0000 2909 7236 0000 0072 9f00 0000 7287  ..).r6...r....r.
-0000c320: 0000 0072 a000 0000 72a1 0000 0072 9800  ...r....r....r..
-0000c330: 0000 7222 0000 0072 5d00 0000 725e 0000  ..r"...r]...r^..
-0000c340: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
-0000c350: da18 6361 7264 5f65 7870 6f72 745f 7065  ..card_export_pe
-0000c360: 7273 6f5f 7075 626b 6579 4707 0000 731e  rso_pubkeyG...s.
-0000c370: 0000 0000 010a 0106 0106 0104 0104 010c  ................
-0000c380: 0110 0110 0102 0110 010a 010a 021e 011c  ................
-0000c390: 017a 2643 6172 6443 6f6e 6e65 6374 6f72  .z&CardConnector
-0000c3a0: 2e63 6172 645f 6578 706f 7274 5f70 6572  .card_export_per
-0000c3b0: 736f 5f70 7562 6b65 7963 0100 0000 0000  so_pubkeyc......
-0000c3c0: 0000 1000 0000 0600 0000 4300 0000 730e  ..........C...s.
-0000c3d0: 0200 0074 006a 0164 0183 0101 0074 026a  ...t.j.d.....t.j
-0000c3e0: 037d 0174 026a 047d 0264 027d 0364 037d  .}.t.j.}.d.}.d.}
-0000c3f0: 047c 017c 027c 037c 0467 047d 057c 006a  .|.|.|.|.g.}.|.j
-0000c400: 057c 0583 015c 037d 067d 077d 087c 0764  .|...\.}.}.}.|.d
-0000c410: 046b 0272 4c7c 0864 026b 0272 4c6e 827c  .k.rL|.d.k.rLn.|
-0000c420: 0764 056b 0272 707c 0864 026b 0272 7074  .d.k.rp|.d.k.rpt
-0000c430: 006a 0664 0683 0101 0074 0764 0783 0182  .j.d.....t.d....
-0000c440: 016e 5e7c 0764 026b 0272 947c 0864 026b  .n^|.d.k.r.|.d.k
-0000c450: 0272 9474 006a 0664 0883 0101 0074 0864  .r.t.j.d.....t.d
-0000c460: 0983 0182 016e 3a74 006a 0664 0a74 0964  .....n:t.j.d.t.d
-0000c470: 0b7c 0714 007c 0817 0083 019b 0064 0c9d  .|...|.......d..
-0000c480: 0383 0101 0074 0a64 0a74 0964 0b7c 0714  .....t.d.t.d.|..
-0000c490: 007c 0817 0083 019b 0064 0c9d 0383 0182  .|.......d......
-0000c4a0: 017c 0664 0219 0064 0d40 0064 0b14 007c  .|.d...d.@.d...|
-0000c4b0: 0664 0319 0064 0d40 0017 007d 097c 0964  .d...d.@...}.|.d
-0000c4c0: 026b 0272 f664 0e53 0064 0f7d 047c 0964  .k.r.d.S.d.}.|.d
-0000c4d0: 0267 0114 007d 0a64 107d 0b67 007d 0c7c  .g...}.d.}.g.}.|
-0000c4e0: 097d 0d64 027d 0e78 827c 0d64 106b 0490  .}.d.}.x.|.d.k..
-0000c4f0: 0172 967c 0e64 113f 0064 0d40 007c 0e64  .r.|.d.?.d.@.|.d
-0000c500: 0d40 0067 027d 0f7c 0f64 027c 0b64 0d40  .@.g.}.|.d.|.d.@
-0000c510: 0067 0237 007d 0f7c 017c 027c 037c 0474  .g.7.}.|.|.|.|.t
-0000c520: 0b7c 0f83 0167 057c 0f17 007d 057c 006a  .|...g.|...}.|.j
-0000c530: 057c 0583 015c 037d 067d 077d 087c 0664  .|...\.}.}.}.|.d
-0000c540: 027c 0b85 0219 007c 0a7c 0e7c 0e7c 0b17  .|.....|.|.|.|..
-0000c550: 0085 023c 007c 0d7c 0b38 007d 0d7c 0e7c  ...<.|.|.8.}.|.|
-0000c560: 0b37 007d 0e90 0171 1657 007c 0e64 113f  .7.}...q.W.|.d.?
-0000c570: 0064 0d40 007c 0e64 0d40 0067 027d 0f7c  .d.@.|.d.@.g.}.|
-0000c580: 0f64 027c 0d64 0d40 0067 0237 007d 0f7c  .d.|.d.@.g.7.}.|
-0000c590: 017c 027c 037c 0474 0b7c 0f83 0167 057c  .|.|.|.t.|...g.|
-0000c5a0: 0f17 007d 057c 006a 057c 0583 015c 037d  ...}.|.j.|...\.}
-0000c5b0: 067d 077d 087c 0664 027c 0d85 0219 007c  .}.}.|.d.|.....|
-0000c5c0: 0a7c 0e7c 0e7c 0d17 0085 023c 007c 006a  .|.|.|.....<.|.j
-0000c5d0: 0c6a 0d7c 0a83 017c 005f 0e7c 006a 0e53  .j.|...|._.|.j.S
-0000c5e0: 0029 124e 7a20 496e 2063 6172 645f 6578  .).Nz In card_ex
-0000c5f0: 706f 7274 5f70 6572 736f 5f63 6572 7469  port_perso_certi
-0000c600: 6669 6361 7465 7201 0000 0072 0c00 0000  ficater....r....
-0000c610: 7241 0000 0072 7200 0000 7a4c 4572 726f  rA...rr...zLErro
-0000c620: 7220 6475 7269 6e67 2070 6572 736f 6e61  r during persona
-0000c630: 6c69 7a61 7469 6f6e 2063 6572 7469 6669  lization certifi
-0000c640: 6361 7465 2065 7870 6f72 743a 2063 6f6d  cate export: com
-0000c650: 6d61 6e64 2075 6e73 7570 706f 7274 6564  mand unsupported
-0000c660: 2830 7836 4430 3029 7a4d 4572 726f 7220  (0x6D00)zMError 
-0000c670: 6475 7269 6e67 2070 6572 736f 6e61 6c69  during personali
-0000c680: 7a61 7469 6f6e 2063 6572 7469 6669 6361  zation certifica
-0000c690: 7465 2065 7870 6f72 743a 2063 6f6d 6d61  te export: comma
-0000c6a0: 6e64 2075 6e73 7570 706f 7274 6564 2028  nd unsupported (
-0000c6b0: 3078 3644 3030 297a 4845 7272 6f72 2064  0x6D00)zHError d
-0000c6c0: 7572 696e 6720 7065 7273 6f6e 616c 697a  uring personaliz
-0000c6d0: 6174 696f 6e20 6365 7274 6966 6963 6174  ation certificat
-0000c6e0: 6520 6578 706f 7274 3a20 6e6f 2063 6172  e export: no car
-0000c6f0: 6420 7072 6573 656e 7428 3078 3030 3030  d present(0x0000
-0000c700: 297a 4945 7272 6f72 2064 7572 696e 6720  )zIError during 
-0000c710: 7065 7273 6f6e 616c 697a 6174 696f 6e20  personalization 
-0000c720: 6365 7274 6966 6963 6174 6520 6578 706f  certificate expo
-0000c730: 7274 3a20 6e6f 2063 6172 6420 7072 6573  rt: no card pres
-0000c740: 656e 7420 2830 7830 3030 3029 7a3d 4572  ent (0x0000)z=Er
-0000c750: 726f 7220 6475 7269 6e67 2070 6572 736f  ror during perso
-0000c760: 6e61 6c69 7a61 7469 6f6e 2063 6572 7469  nalization certi
-0000c770: 6669 6361 7465 2065 7870 6f72 743a 2028  ficate export: (
-0000c780: 6572 726f 7220 636f 6465 2072 ba00 0000  error code r....
-0000c790: 72bb 0000 0072 d300 0000 7a07 2865 6d70  r....r....z.(emp
-0000c7a0: 7479 2972 2300 0000 729b 0000 0072 b200  ty)r#...r....r..
-0000c7b0: 0000 290f 7227 0000 0072 3400 0000 722b  ..).r'...r4...r+
-0000c7c0: 0000 0072 bc00 0000 5a1a 494e 535f 4558  ...r....Z.INS_EX
-0000c7d0: 504f 5254 5f50 4b49 5f43 4552 5449 4649  PORT_PKI_CERTIFI
-0000c7e0: 4341 5445 7299 0000 0072 e200 0000 72e3  CATEr....r....r.
-0000c7f0: 0000 0072 9700 0000 724c 0000 0072 f200  ...r....rL...r..
-0000c800: 0000 7235 0000 0072 7600 0000 5a1b 636f  ..r5...rv...Z.co
-0000c810: 6e76 6572 745f 6279 7465 735f 746f 5f73  nvert_bytes_to_s
-0000c820: 7472 696e 675f 7065 6d72 8200 0000 2910  tring_pemr....).
-0000c830: 7236 0000 0072 9f00 0000 7287 0000 0072  r6...r....r....r
-0000c840: a000 0000 72a1 0000 0072 9800 0000 7222  ....r....r....r"
-0000c850: 0000 0072 5d00 0000 725e 0000 005a 1063  ...r]...r^...Z.c
-0000c860: 6572 7469 6669 6361 7465 5f73 697a 655a  ertificate_sizeZ
-0000c870: 0b63 6572 7469 6669 6361 7465 725b 0100  .certificater[..
-0000c880: 0072 2201 0000 5a0e 7265 6d61 696e 696e  .r"...Z.remainin
-0000c890: 675f 7369 7a65 5a0b 6365 7274 5f6f 6666  g_sizeZ.cert_off
-0000c8a0: 7365 7472 c900 0000 7237 0000 0072 3700  setr....r7...r7.
-0000c8b0: 0000 7238 0000 00da 1d63 6172 645f 6578  ..r8.....card_ex
-0000c8c0: 706f 7274 5f70 6572 736f 5f63 6572 7469  port_perso_certi
-0000c8d0: 6669 6361 7465 5907 0000 7352 0000 0000  ficateY...sR....
-0000c8e0: 010a 0106 0106 0104 0104 030c 0110 0110  ................
-0000c8f0: 0102 0110 010a 010a 0110 010a 010a 021e  ................
-0000c900: 011c 021c 0108 0104 0304 010a 0104 0104  ................
-0000c910: 0104 0104 010c 0214 0110 0116 0110 0118  ................
-0000c920: 0108 010e 0314 0110 0116 0110 0118 030e  ................
-0000c930: 017a 2b43 6172 6443 6f6e 6e65 6374 6f72  .z+CardConnector
-0000c940: 2e63 6172 645f 6578 706f 7274 5f70 6572  .card_export_per
-0000c950: 736f 5f63 6572 7469 6669 6361 7465 6302  so_certificatec.
-0000c960: 0000 0000 0000 000c 0000 0006 0000 0043  ...............C
-0000c970: 0000 0073 6400 0000 7400 6a01 6401 8301  ...sd...t.j.d...
-0000c980: 0100 7402 6a03 7d02 7402 6a04 7d03 6402  ..t.j.}.t.j.}.d.
-0000c990: 7d04 6402 7d05 7405 6403 8301 7d06 7c02  }.d.}.t.d...}.|.
-0000c9a0: 7c03 7c04 7c05 7406 7c06 8301 6705 7407  |.|.|.t.|...g.t.
-0000c9b0: 7c06 8301 1700 7d07 7c00 6a08 7c07 8301  |.....}.|.j.|...
-0000c9c0: 5c03 7d08 7d09 7d0a 7c00 6a09 6a0a 7c08  \.}.}.}.|.j.j.|.
-0000c9d0: 7c06 7c01 8303 7d0b 7c0b 5300 2904 4e7a  |.|...}.|.S.).Nz
-0000c9e0: 1e49 6e20 6361 7264 5f63 6861 6c6c 656e  .In card_challen
-0000c9f0: 6765 5f72 6573 706f 6e73 655f 706b 6972  ge_response_pkir
-0000ca00: 0100 0000 720d 0100 0029 0b72 2700 0000  ....r....).r'...
-0000ca10: 7234 0000 0072 2b00 0000 72bc 0000 005a  r4...r+...r....Z
-0000ca20: 1a49 4e53 5f43 4841 4c4c 454e 4745 5f52  .INS_CHALLENGE_R
-0000ca30: 4553 504f 4e53 455f 504b 4972 1800 0000  ESPONSE_PKIr....
-0000ca40: 7235 0000 0072 c600 0000 7299 0000 0072  r5...r....r....r
-0000ca50: 7600 0000 5a1d 7665 7269 6679 5f63 6861  v...Z.verify_cha
-0000ca60: 6c6c 656e 6765 5f72 6573 706f 6e73 655f  llenge_response_
-0000ca70: 706b 6929 0c72 3600 0000 7211 0100 0072  pki).r6...r....r
-0000ca80: 9f00 0000 7287 0000 0072 a000 0000 72a1  ....r....r....r.
-0000ca90: 0000 005a 1363 6861 6c6c 656e 6765 5f66  ...Z.challenge_f
-0000caa0: 726f 6d5f 686f 7374 7298 0000 0072 2200  rom_hostr....r".
-0000cab0: 0000 725d 0000 0072 5e00 0000 5a05 7665  ..r]...r^...Z.ve
-0000cac0: 7269 6672 3700 0000 7237 0000 0072 3800  rifr7...r7...r8.
-0000cad0: 0000 da1b 6361 7264 5f63 6861 6c6c 656e  ....card_challen
-0000cae0: 6765 5f72 6573 706f 6e73 655f 706b 698f  ge_response_pki.
-0000caf0: 0700 0073 1400 0000 0001 0a01 0601 0601  ...s............
-0000cb00: 0401 0402 0802 1a01 1003 1002 7a29 4361  ............z)Ca
-0000cb10: 7264 436f 6e6e 6563 746f 722e 6361 7264  rdConnector.card
-0000cb20: 5f63 6861 6c6c 656e 6765 5f72 6573 706f  _challenge_respo
-0000cb30: 6e73 655f 706b 6963 0100 0000 0000 0000  nse_pkic........
-0000cb40: 0f00 0000 1400 0000 4300 0000 73c0 0100  ........C...s...
-0000cb50: 0074 006a 0164 0183 0101 0064 0204 007d  .t.j.d.....d...}
-0000cb60: 017d 0279 1e7c 006a 0283 007d 0174 006a  .}.y.|.j...}.t.j
-0000cb70: 0164 0374 037c 0183 0117 0083 0101 0057  .d.t.|.........W
-0000cb80: 006e 8004 0074 046b 0a72 6001 007d 0301  .n...t.k.r`..}..
-0000cb90: 007a 1464 026a 0564 0464 0567 0283 017d  .z.d.j.d.d.g...}
-0000cba0: 0257 0059 0064 0064 007d 037e 0358 006e  .W.Y.d.d.}.~.X.n
-0000cbb0: 5204 0074 066b 0a72 8401 007d 0301 007a  R..t.k.r...}...z
-0000cbc0: 0a64 067d 0257 0059 0064 0064 007d 037e  .d.}.W.Y.d.d.}.~
-0000cbd0: 0358 006e 2e04 0074 076b 0a72 b001 007d  .X.n...t.k.r...}
-0000cbe0: 0301 007a 1264 0774 037c 0383 0117 007d  ...z.d.t.|.....}
-0000cbf0: 0257 0059 0064 0064 007d 037e 0358 006e  .W.Y.d.d.}.~.X.n
-0000cc00: 0258 007c 0164 086b 0272 be64 097d 027c  .X.|.d.k.r.d.}.|
-0000cc10: 0264 026b 0372 d464 0a64 0864 0864 087c  .d.k.r.d.d.d.d.|
-0000cc20: 0266 0553 0074 0883 007d 047c 046a 097c  .f.S.t...}.|.j.|
-0000cc30: 017c 006a 0a83 025c 067d 057d 067d 077d  .|.j...\.}.}.}.}
-0000cc40: 087d 097d 027c 0590 0173 0864 0a7c 077c  .}.}.|...s.d.|.|
-0000cc50: 087c 097c 0266 0553 007c 006a 0b7c 0683  .|.|.f.S.|.j.|..
-0000cc60: 015c 027d 0a7d 027c 0a90 0173 2a64 0a7c  .\.}.}.|...s*d.|
-0000cc70: 077c 087c 097c 0266 0553 007c 046a 0c7c  .|.|.|.f.S.|.j.|
-0000cc80: 0183 017d 0b7c 0b64 0b19 007d 0c74 006a  ...}.|.d...}.t.j
-0000cc90: 0164 0c7c 0c9b 009d 0283 0101 007c 0c6a  .d.|.........|.j
-0000cca0: 0d64 0d64 0083 026a 0e64 0e83 017d 0d74  .d.d...j.d...}.t
-0000ccb0: 006a 0164 0f7c 0d9b 009d 0283 0101 0074  .j.d.|.........t
-0000ccc0: 006a 0164 107c 006a 0f9b 009d 0283 0101  .j.d.|.j........
-0000ccd0: 007c 0d6a 1083 007c 006a 0f6a 1083 006b  .|.j...|.j.j...k
-0000cce0: 0290 0172 9a64 117d 0e6e 1864 0a7d 0e64  ...r.d.}.n.d.}.d
-0000ccf0: 127c 0d9b 0064 137c 006a 0f9b 0064 149d  .|...d.|.j...d..
-0000cd00: 057d 027c 0e7c 077c 087c 097c 0266 0553  .}.|.|.|.|.|.f.S
-0000cd10: 0029 154e 7a1b 496e 2063 6172 645f 7665  .).Nz.In card_ve
-0000cd20: 7269 6679 5f61 7574 6865 6e74 6963 6974  rify_authenticit
-0000cd30: 79da 007a 0a43 6572 7420 5045 4d3a 207a  y..z.Cert PEM: z
-0000cd40: 3855 6e61 626c 6520 746f 2067 6574 2064  8Unable to get d
-0000cd50: 6576 6963 6520 6365 7274 6966 6963 6174  evice certificat
-0000cd60: 653a 2066 6561 7475 7265 2075 6e73 7570  e: feature unsup
-0000cd70: 706f 7274 6564 2120 0a7a 5141 7574 6865  ported! .zQAuthe
-0000cd80: 6e74 6963 6974 7920 7661 6c69 6461 7469  nticity validati
-0000cd90: 6f6e 2069 7320 6f6e 6c79 2061 7661 696c  on is only avail
-0000cda0: 6162 6c65 2073 7461 7274 696e 6720 7769  able starting wi
-0000cdb0: 7468 2053 6174 6f63 6869 7020 7630 2e31  th Satochip v0.1
-0000cdc0: 3220 616e 6420 6869 6768 6572 7a22 4e6f  2 and higherz"No
-0000cdd0: 2063 6172 6420 666f 756e 6421 2050 6c65   card found! Ple
-0000cde0: 6173 6520 696e 7365 7274 2063 6172 642e  ase insert card.
-0000cdf0: 7a2c 4578 6365 7074 696f 6e20 6475 7269  z,Exception duri
-0000ce00: 6e67 2064 6576 6963 6520 6365 7274 6966  ng device certif
-0000ce10: 6963 6174 6520 6578 706f 7274 3a20 7a07  icate export: z.
-0000ce20: 2865 6d70 7479 297a 4044 6576 6963 6520  (empty)z@Device 
-0000ce30: 6365 7274 6966 6963 6174 6520 6973 2065  certificate is e
-0000ce40: 6d70 7479 3a20 7468 6520 6361 7264 2068  mpty: the card h
-0000ce50: 6173 206e 6f74 2062 6565 6e20 7065 7273  as not been pers
-0000ce60: 6f6e 616c 697a 6564 2146 da07 7375 626a  onalized!F..subj
-0000ce70: 6563 747a 2a49 6e20 6361 7264 5f76 6572  ectz*In card_ver
-0000ce80: 6966 795f 6175 7468 656e 7469 6369 7479  ify_authenticity
-0000ce90: 2073 7562 6a65 6374 5f64 6963 743d 2073   subject_dict= s
-0000cea0: 0200 0000 434e 7a05 7574 662d 387a 2549  ....CNz.utf-8z%I
-0000ceb0: 6e20 6361 7264 5f76 6572 6966 795f 6175  n card_verify_au
-0000cec0: 7468 656e 7469 6369 7479 2073 7562 6a65  thenticity subje
-0000ced0: 6374 3d20 7a26 496e 2063 6172 645f 7665  ct= z&In card_ve
-0000cee0: 7269 6679 5f61 7574 6865 6e74 6963 6974  rify_authenticit
-0000cef0: 7920 5549 445f 5348 4131 3d20 547a 1443  y UID_SHA1= Tz.C
-0000cf00: 6572 7469 6669 6361 7465 2073 7562 6a65  ertificate subje
-0000cf10: 6374 207a 2720 646f 6573 206e 6f74 206d  ct z' does not m
-0000cf20: 6174 6368 2074 6865 2063 6172 6420 7365  atch the card se
-0000cf30: 7269 616c 206e 756d 6265 7220 fa01 2129  rial number ..!)
-0000cf40: 1172 2700 0000 7234 0000 0072 7101 0000  .r'...r4...rq...
-0000cf50: 7275 0000 0072 e300 0000 da04 6a6f 696e  ru...r......join
-0000cf60: 7297 0000 0072 f200 0000 7217 0000 005a  r....r....r....Z
-0000cf70: 1a76 616c 6964 6174 655f 6365 7274 6966  .validate_certif
-0000cf80: 6963 6174 655f 6368 6169 6e72 8100 0000  icate_chainr....
-0000cf90: 7272 0100 005a 1570 6172 7365 5f70 656d  rr...Z.parse_pem
-0000cfa0: 5f63 6572 7469 6669 6361 7465 7244 0100  _certificaterD..
-0000cfb0: 0072 c000 0000 7252 0000 00da 056c 6f77  .r....rR.....low
-0000cfc0: 6572 290f 7236 0000 0072 8200 0000 5a09  er).r6...r....Z.
-0000cfd0: 7478 745f 6572 726f 7272 ab00 0000 5a09  txt_errorr....Z.
-0000cfe0: 7661 6c69 6461 746f 725a 0e69 735f 7661  validatorZ.is_va
-0000cff0: 6c69 645f 6368 6169 6e5a 0d64 6576 6963  lid_chainZ.devic
-0000d000: 655f 7075 626b 6579 5a06 7478 745f 6361  e_pubkeyZ.txt_ca
-0000d010: 5a09 7478 745f 7375 6263 615a 0a74 7874  Z.txt_subcaZ.txt
-0000d020: 5f64 6576 6963 655a 1169 735f 7661 6c69  _deviceZ.is_vali
-0000d030: 645f 6368 616c 7265 7370 5a09 6365 7274  d_chalrespZ.cert
-0000d040: 5f64 6963 745a 0c73 7562 6a65 6374 5f64  _dictZ.subject_d
-0000d050: 6963 7472 7401 0000 5a16 6973 5f76 616c  ictrt...Z.is_val
-0000d060: 6964 5f73 6572 6961 6c5f 6e75 6d62 6572  id_serial_number
-0000d070: 7237 0000 0072 3700 0000 7238 0000 00da  r7...r7...r8....
-0000d080: 1863 6172 645f 7665 7269 6679 5f61 7574  .card_verify_aut
-0000d090: 6865 6e74 6963 6974 79a0 0700 0073 4400  henticity....sD.
-0000d0a0: 0000 0001 0a03 0801 0201 0801 1601 1001  ................
-0000d0b0: 0601 1801 1001 1401 1001 1e02 0801 0402  ................
-0000d0c0: 0801 0e03 0601 1a01 0601 0e03 0e01 0601  ................
-0000d0d0: 0e03 0a01 0801 1001 1201 1001 1201 1401  ................
-0000d0e0: 0602 0401 1402 7a26 4361 7264 436f 6e6e  ......z&CardConn
-0000d0f0: 6563 746f 722e 6361 7264 5f76 6572 6966  ector.card_verif
-0000d100: 795f 6175 7468 656e 7469 6369 7479 6302  y_authenticityc.
-0000d110: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-0000d120: 0000 0073 1c00 0000 7c01 6700 6b02 7212  ...s....|.g.k.r.
-0000d130: 7400 6401 6701 1400 7d01 7c01 7c00 5f01  t.d.g...}.|.|._.
-0000d140: 6400 5300 2902 4e72 0100 0000 2902 727d  d.S.).Nr....).r}
-0000d150: 0000 0072 7e00 0000 2902 7236 0000 0072  ...r~...).r6...r
-0000d160: 7e00 0000 7237 0000 0072 3700 0000 7238  ~...r7...r7...r8
-0000d170: 0000 0072 d800 0000 d407 0000 7306 0000  ...r........s...
-0000d180: 0000 0108 010a 017a 2843 6172 6443 6f6e  .......z(CardCon
-0000d190: 6e65 6374 6f72 2e73 6174 6f64 696d 655f  nector.satodime_
-0000d1a0: 7365 745f 756e 6c6f 636b 5f73 6563 7265  set_unlock_secre
-0000d1b0: 7463 0200 0000 0000 0000 0200 0000 0200  tc..............
-0000d1c0: 0000 4300 0000 731c 0000 007c 0167 006b  ..C...s....|.g.k
-0000d1d0: 0272 1274 0064 0167 0114 007d 017c 017c  .r.t.d.g...}.|.|
-0000d1e0: 005f 0164 0053 0029 024e 7201 0000 0029  ._.d.S.).Nr....)
-0000d1f0: 0272 7f00 0000 7280 0000 0029 0272 3600  .r....r....).r6.
-0000d200: 0000 7280 0000 0072 3700 0000 7237 0000  ..r....r7...r7..
-0000d210: 0072 3800 0000 72d7 0000 00d8 0700 0073  .r8...r........s
-0000d220: 0600 0000 0001 0801 0a01 7a29 4361 7264  ..........z)Card
-0000d230: 436f 6e6e 6563 746f 722e 7361 746f 6469  Connector.satodi
-0000d240: 6d65 5f73 6574 5f75 6e6c 6f63 6b5f 636f  me_set_unlock_co
-0000d250: 756e 7465 7263 0100 0000 0000 0000 0200  unterc..........
-0000d260: 0000 0600 0000 4300 0000 7334 0000 0074  ......C...s4...t
-0000d270: 006a 017c 006a 0264 0164 0264 038d 037d  .j.|.j.d.d.d...}
-0000d280: 017c 0164 0437 007d 0174 037c 016a 0464  .|.d.7.}.t.|.j.d
-0000d290: 0564 0164 0264 038d 0383 017c 005f 0264  .d.d.d.....|._.d
-0000d2a0: 0053 0029 064e 5a03 6269 6746 2902 da09  .S.).NZ.bigF)...
-0000d2b0: 6279 7465 6f72 6465 725a 0673 6967 6e65  byteorderZ.signe
-0000d2c0: 6472 0c00 0000 7243 0000 0029 05da 0369  dr....rC...)...i
-0000d2d0: 6e74 da0a 6672 6f6d 5f62 7974 6573 7280  nt..from_bytesr.
-0000d2e0: 0000 0072 c600 0000 da08 746f 5f62 7974  ...r......to_byt
-0000d2f0: 6573 2902 7236 0000 005a 0b63 6f75 6e74  es).r6...Z.count
-0000d300: 6572 5f69 6e74 7237 0000 0072 3700 0000  er_intr7...r7...
-0000d310: 7238 0000 00da 2173 6174 6f64 696d 655f  r8....!satodime_
-0000d320: 696e 6372 656d 656e 745f 756e 6c6f 636b  increment_unlock
-0000d330: 5f63 6f75 6e74 6572 dc07 0000 7306 0000  _counter....s...
-0000d340: 0000 0112 0108 017a 2f43 6172 6443 6f6e  .......z/CardCon
-0000d350: 6e65 6374 6f72 2e73 6174 6f64 696d 655f  nector.satodime_
-0000d360: 696e 6372 656d 656e 745f 756e 6c6f 636b  increment_unlock
-0000d370: 5f63 6f75 6e74 6572 6301 0000 0000 0000  _counterc.......
-0000d380: 000b 0000 0005 0000 0043 0000 0073 2a01  .........C...s*.
-0000d390: 0000 7400 6a01 6401 8301 0100 7402 6a03  ..t.j.d.....t.j.
-0000d3a0: 7d01 6402 7d02 6403 7d03 6403 7d04 7c01  }.d.}.d.}.d.}.|.
-0000d3b0: 7c02 7c03 7c04 6704 7d05 7c00 6a04 7c05  |.|.|.g.}.|.j.|.
-0000d3c0: 8301 5c03 7d06 7d07 7d08 7c07 6404 6b02  ..\.}.}.}.|.d.k.
-0000d3d0: 724a 7c08 6403 6b02 724a 6e82 7c07 6403  rJ|.d.k.rJn.|.d.
-0000d3e0: 6b02 726e 7c08 6403 6b02 726e 7400 6a05  k.rn|.d.k.rnt.j.
-0000d3f0: 6405 8301 0100 7406 6405 8301 8201 6e5e  d.....t.d.....n^
-0000d400: 7c07 6406 6b02 7292 7c08 6407 6b02 7292  |.d.k.r.|.d.k.r.
-0000d410: 7400 6a05 6408 8301 0100 7407 6409 8301  t.j.d.....t.d...
-0000d420: 8201 6e3a 7400 6a05 640a 7408 640b 7c07  ..n:t.j.d.t.d.|.
-0000d430: 1400 7c08 1700 8301 9b00 640c 9d03 8301  ..|.......d.....
-0000d440: 0100 7409 640a 7408 640b 7c07 1400 7c08  ..t.d.t.d.|...|.
-0000d450: 1700 8301 9b00 640c 9d03 8301 8201 6403  ......d.......d.
-0000d460: 7d09 6900 7d0a 7c06 7c09 7c09 740a 1700  }.i.}.|.|.|.t...
-0000d470: 8502 1900 7c0a 640d 3c00 7c0a 640d 1900  ....|.d.<.|.d...
-0000d480: 7c00 5f0b 7c09 740a 3700 7d09 7c06 7c09  |._.|.t.7.}.|.|.
-0000d490: 1900 7c0a 640e 3c00 7c09 640f 3700 7d09  ..|.d.<.|.d.7.}.
-0000d4a0: 7c06 7c09 6410 8502 1900 7c0a 6411 3c00  |.|.d.....|.d.<.
-0000d4b0: 7c06 7c07 7c08 7c0a 6604 5300 2912 7a27  |.|.|.|.f.S.).z'
-0000d4c0: 5265 7475 726e 2073 7461 7475 7320 696e  Return status in
-0000d4d0: 666f 2073 7065 6369 6669 6320 746f 2053  fo specific to S
-0000d4e0: 6174 6f64 696d 657a 1649 6e20 7361 746f  atodimez.In sato
-0000d4f0: 6469 6d65 5f67 6574 5f73 7461 7475 73e9  dime_get_status.
-0000d500: 5000 0000 7201 0000 0072 4100 0000 7a43  P...r....rA...zC
-0000d510: 4572 726f 7220 7768 696c 6520 6665 7463  Error while fetc
-0000d520: 6869 6e67 2053 6174 6f64 696d 6520 7374  hing Satodime st
-0000d530: 6174 7573 3a20 6e6f 2063 6172 6420 7072  atus: no card pr
-0000d540: 6573 656e 7420 2863 6f64 6520 3078 3030  esent (code 0x00
-0000d550: 3030 2972 4200 0000 7243 0000 007a 4245  00)rB...rC...zBE
-0000d560: 7272 6f72 2077 6869 6c65 2066 6574 6368  rror while fetch
-0000d570: 696e 6720 5361 746f 6469 6d65 2073 7461  ing Satodime sta
-0000d580: 7475 733a 2073 6574 7570 206e 6f74 2064  tus: setup not d
-0000d590: 6f6e 6520 2863 6f64 6520 3078 3030 3030  one (code 0x0000
-0000d5a0: 297a 4245 7272 6f72 2077 6869 6c65 2066  )zBError while f
-0000d5b0: 6574 6368 696e 6720 5361 746f 6469 6d65  etching Satodime
-0000d5c0: 2073 7461 7475 733a 2073 6574 7570 206e   status: setup n
-0000d5d0: 6f74 2064 6f6e 6520 2863 6f64 6520 3078  ot done (code 0x
-0000d5e0: 3963 3034 297a 3245 7272 6f72 2077 6869  9c04)z2Error whi
-0000d5f0: 6c65 2066 6574 6368 696e 6720 5361 746f  le fetching Sato
-0000d600: 6469 6d65 2073 7461 7475 733a 2028 6572  dime status: (er
-0000d610: 726f 7220 636f 6465 2072 ba00 0000 72bb  ror code r....r.
-0000d620: 0000 0072 8000 0000 da0c 6d61 785f 6e75  ...r......max_nu
-0000d630: 6d5f 6b65 7973 720c 0000 004e da14 7361  m_keysr....N..sa
-0000d640: 746f 6469 6d65 5f6b 6579 735f 7374 6174  todime_keys_stat
-0000d650: 7573 290c 7227 0000 0072 3400 0000 722b  us).r'...r4...r+
-0000d660: 0000 0072 bc00 0000 7299 0000 0072 e200  ...r....r....r..
-0000d670: 0000 7297 0000 00da 1543 6172 6453 6574  ..r......CardSet
-0000d680: 7570 4e6f 7444 6f6e 6545 7272 6f72 724c  upNotDoneErrorrL
-0000d690: 0000 0072 f200 0000 727f 0000 0072 8000  ...r....r....r..
-0000d6a0: 0000 290b 7236 0000 0072 9f00 0000 7287  ..).r6...r....r.
-0000d6b0: 0000 0072 a000 0000 72a1 0000 0072 9800  ...r....r....r..
-0000d6c0: 0000 7222 0000 0072 5d00 0000 725e 0000  ..r"...r]...r^..
-0000d6d0: 0072 6601 0000 5a0f 7361 746f 6469 6d65  .rf...Z.satodime
-0000d6e0: 5f73 7461 7475 7372 3700 0000 7237 0000  _statusr7...r7..
-0000d6f0: 0072 3800 0000 da13 7361 746f 6469 6d65  .r8.....satodime
-0000d700: 5f67 6574 5f73 7461 7475 73e1 0700 0073  _get_status....s
-0000d710: 3400 0000 0002 0a01 0601 0401 0401 0401  4...............
-0000d720: 0c01 1002 1001 0201 1001 0a01 0a01 1001  ................
-0000d730: 0a01 0a02 1e01 1c02 0401 0401 1401 0a01  ................
-0000d740: 0801 0c01 0801 1001 7a21 4361 7264 436f  ........z!CardCo
-0000d750: 6e6e 6563 746f 722e 7361 746f 6469 6d65  nnector.satodime
-0000d760: 5f67 6574 5f73 7461 7475 7329 01da 076b  _get_status)...k
-0000d770: 6579 5f6e 6272 6302 0000 0000 0000 000b  ey_nbrc.........
-0000d780: 0000 0004 0000 0043 0000 0073 9800 0000  .......C...s....
-0000d790: 7400 6a01 6401 8301 0100 7402 6a03 7d02  t.j.d.....t.j.}.
-0000d7a0: 6402 7d03 7c01 6403 1600 7d04 6404 7d05  d.}.|.d...}.d.}.
-0000d7b0: 7c02 7c03 7c04 7c05 6704 7d06 7c00 6a04  |.|.|.|.g.}.|.j.
-0000d7c0: 7c06 8301 5c03 7d07 7d08 7d09 7c08 6405  |...\.}.}.}.|.d.
-0000d7d0: 6b02 724e 7c09 6404 6b02 724e 6e32 7c08  k.rN|.d.k.rNn2|.
-0000d7e0: 6404 6b02 7280 7c09 6404 6b02 7280 7400  d.k.r.|.d.k.r.t.
-0000d7f0: 6a05 6406 7c01 9b00 6407 9d03 8301 0100  j.d.|...d.......
-0000d800: 7406 6406 7c01 9b00 6407 9d03 8301 8201  t.d.|...d.......
-0000d810: 7c00 6a07 6a08 7c07 8301 7d0a 7c07 7c08  |.j.j.|...}.|.|.
-0000d820: 7c09 7c0a 6604 5300 2908 4e7a 1e49 6e20  |.|.f.S.).Nz.In 
-0000d830: 7361 746f 6469 6d65 5f67 6574 5f6b 6579  satodime_get_key
-0000d840: 736c 6f74 5f73 7461 7475 7372 8900 0000  slot_statusr....
-0000d850: 72ba 0000 0072 0100 0000 7241 0000 007a  r....r....rA...z
-0000d860: 2245 7272 6f72 2077 6869 6c65 2066 6574  "Error while fet
-0000d870: 6368 696e 6720 5361 746f 6469 6d65 206b  ching Satodime k
-0000d880: 6579 207a 2620 7374 6174 7573 3a20 6e6f  ey z& status: no
-0000d890: 2063 6172 6420 7072 6573 656e 7420 2863   card present (c
-0000d8a0: 6f64 6520 3078 3030 3030 2929 0972 2700  ode 0x0000)).r'.
-0000d8b0: 0000 7234 0000 0072 2b00 0000 72bc 0000  ..r4...r+...r...
-0000d8c0: 0072 9900 0000 72e2 0000 0072 9700 0000  .r....r....r....
-0000d8d0: 7276 0000 005a 2170 6172 7365 5f73 6174  rv...Z!parse_sat
-0000d8e0: 6f64 696d 655f 6765 745f 6b65 7973 6c6f  odime_get_keyslo
-0000d8f0: 745f 7374 6174 7573 290b 7236 0000 0072  t_status).r6...r
-0000d900: 8301 0000 729f 0000 0072 8700 0000 72a0  ....r....r....r.
-0000d910: 0000 0072 a100 0000 7298 0000 0072 2200  ...r....r....r".
-0000d920: 0000 725d 0000 0072 5e00 0000 5a0e 6b65  ..r]...r^...Z.ke
-0000d930: 7973 6c6f 745f 7374 6174 7573 7237 0000  yslot_statusr7..
-0000d940: 0072 3700 0000 7238 0000 00da 1b73 6174  .r7...r8.....sat
-0000d950: 6f64 696d 655f 6765 745f 6b65 7973 6c6f  odime_get_keyslo
-0000d960: 745f 7374 6174 7573 0408 0000 731c 0000  t_status....s...
-0000d970: 0000 010a 0106 0104 0108 0104 010c 0210  ................
-0000d980: 0210 0102 0110 0112 0110 030c 017a 2943  .............z)C
-0000d990: 6172 6443 6f6e 6e65 6374 6f72 2e73 6174  ardConnector.sat
-0000d9a0: 6f64 696d 655f 6765 745f 6b65 7973 6c6f  odime_get_keyslo
-0000d9b0: 745f 7374 6174 7573 2904 7283 0100 00da  t_status).r.....
-0000d9c0: 0452 4655 31da 0452 4655 32da 096b 6579  .RFU1..RFU2..key
-0000d9d0: 5f61 7373 6574 6308 0000 0000 0000 0014  _assetc.........
-0000d9e0: 0000 0006 0000 0043 0000 0073 5e01 0000  .......C...s^...
-0000d9f0: 7400 6a01 6401 8301 0100 7402 6a03 7d08  t.j.d.....t.j.}.
-0000da00: 6402 7d09 7c01 6403 1600 7d0a 6404 7d0b  d.}.|.d...}.d.}.
-0000da10: 7404 7405 1700 6405 1700 7406 1700 7407  t.t...d...t...t.
-0000da20: 1700 7408 1700 7d0c 7c08 7c09 7c0a 7c0b  ..t...}.|.|.|.|.
-0000da30: 7c0c 6705 7d0d 7c05 6700 6b02 725a 6406  |.g.}.|.g.k.rZd.
-0000da40: 6404 6404 6404 6704 7d05 7c06 6700 6b02  d.d.d.g.}.|.g.k.
-0000da50: 726c 7407 6404 6701 1400 7d06 7c07 6700  rlt.d.g...}.|.g.
-0000da60: 6b02 727e 7408 6404 6701 1400 7d07 7409  k.r~t.d.g...}.t.
-0000da70: 7c05 8301 740a 6b08 7292 740b 7c05 8301  |...t.k.r.t.|...
-0000da80: 7d05 7409 7c06 8301 740a 6b08 72a6 740b  }.t.|...t.k.r.t.
-0000da90: 7c06 8301 7d06 7409 7c07 8301 740a 6b08  |...}.t.|...t.k.
-0000daa0: 72ba 740b 7c07 8301 7d07 740b 740c 6a0d  r.t.|...}.t.t.j.
-0000dab0: 740a 7c00 6a0e 8301 740a 7c0d 7c00 6a0f  t.|.j...t.|.|.j.
-0000dac0: 1700 8301 7410 6a11 8303 6a12 8300 8301  ....t.j...j.....
-0000dad0: 7d0e 7c00 6a0f 7c0e 1700 7c02 6403 1600  }.|.j.|...|.d...
-0000dae0: 7c03 6403 1600 7c04 6403 1600 6703 1700  |.d...|.d...g...
-0000daf0: 7c05 1700 7c06 1700 7c07 1700 7d0f 7413  |...|...|...}.t.
-0000db00: 7c0f 8301 7c0c 6b03 9001 7234 7414 6407  |...|.k...r4t.d.
-0000db10: 7413 7c0f 8301 9b00 6408 7c0c 9b00 9d04  t.|.....d.|.....
-0000db20: 8301 8201 7c0d 7c0f 1700 7d10 7c00 6a15  ....|.|...}.|.j.
-0000db30: 7c10 8301 5c03 7d11 7d12 7d13 7c00 6a16  |...\.}.}.}.|.j.
-0000db40: 8300 0100 7c11 7c12 7c13 6603 5300 2909  ....|.|.|.f.S.).
-0000db50: 4e7a 1e49 6e20 7361 746f 6469 6d65 5f73  Nz.In satodime_s
-0000db60: 6574 5f6b 6579 736c 6f74 5f73 7461 7475  et_keyslot_statu
-0000db70: 7372 8a00 0000 72ba 0000 0072 0100 0000  sr....r....r....
-0000db80: 72b1 0000 0072 9b00 0000 7a3a 4572 726f  r....r....z:Erro
-0000db90: 7220 696e 2073 6174 6f64 696d 655f 7365  r in satodime_se
-0000dba0: 745f 6b65 7973 6c6f 745f 7374 6174 7573  t_keyslot_status
-0000dbb0: 3a20 7772 6f6e 6720 7374 6174 7573 206c  : wrong status l
-0000dbc0: 656e 6774 6820 7a0c 2069 6e73 7465 6164  ength z. instead
-0000dbd0: 206f 6620 2917 7227 0000 0072 3400 0000   of ).r'...r4...
-0000dbe0: 722b 0000 0072 bc00 0000 727f 0000 00da  r+...r....r.....
-0000dbf0: 1053 495a 455f 554e 4c4f 434b 5f43 4f44  .SIZE_UNLOCK_COD
-0000dc00: 455a 0b53 495a 455f 534c 4950 3434 5a0d  EZ.SIZE_SLIP44Z.
-0000dc10: 5349 5a45 5f43 4f4e 5452 4143 545a 0c53  SIZE_CONTRACTZ.S
-0000dc20: 495a 455f 544f 4b45 4e49 4472 2600 0000  IZE_TOKENIDr&...
-0000dc30: 724b 0000 0072 c600 0000 72eb 0000 00da  rK...r....r.....
-0000dc40: 036e 6577 727e 0000 0072 8000 0000 724f  .newr~...r....rO
-0000dc50: 0000 0072 5000 0000 da06 6469 6765 7374  ...rP.....digest
-0000dc60: 7235 0000 0072 5300 0000 7299 0000 0072  r5...rS...r....r
-0000dc70: 7d01 0000 2914 7236 0000 0072 8301 0000  }...).r6...r....
-0000dc80: 7285 0100 0072 8601 0000 7287 0100 005a  r....r....r....Z
-0000dc90: 0a6b 6579 5f73 6c69 7034 345a 0c6b 6579  .key_slip44Z.key
-0000dca0: 5f63 6f6e 7472 6163 745a 0b6b 6579 5f74  _contractZ.key_t
-0000dcb0: 6f6b 656e 6964 729f 0000 0072 8700 0000  okenidr....r....
-0000dcc0: 72a0 0000 0072 a100 0000 da08 6461 7461  r....r......data
-0000dcd0: 7369 7a65 da0a 6170 6475 6865 6164 6572  size..apduheader
-0000dce0: da0b 756e 6c6f 636b 5f63 6f64 6572 c900  ..unlock_coder..
-0000dcf0: 0000 7298 0000 0072 2200 0000 725d 0000  ..r....r"...r]..
-0000dd00: 0072 5e00 0000 7237 0000 0072 3700 0000  .r^...r7...r7...
-0000dd10: 7238 0000 00da 2173 6174 6f64 696d 655f  r8....!satodime_
-0000dd20: 7365 745f 6b65 7973 6c6f 745f 7374 6174  set_keyslot_stat
-0000dd30: 7573 5f70 6172 7430 1808 0000 7336 0000  us_part0....s6..
-0000dd40: 0000 020a 0106 0104 0108 0104 0118 010e  ................
-0000dd50: 0208 000c 0108 000a 0108 000a 010c 0008  ................
-0000dd60: 010c 0008 010c 0008 0328 022c 010e 0118  .........(.,....
-0000dd70: 0108 0210 0108 027a 2f43 6172 6443 6f6e  .......z/CardCon
-0000dd80: 6e65 6374 6f72 2e73 6174 6f64 696d 655f  nector.satodime_
-0000dd90: 7365 745f 6b65 7973 6c6f 745f 7374 6174  set_keyslot_stat
-0000dda0: 7573 5f70 6172 7430 6303 0000 0000 0000  us_part0c.......
-0000ddb0: 000f 0000 0006 0000 0043 0000 0073 e400  .........C...s..
-0000ddc0: 0000 7400 6a01 6401 8301 0100 7402 6a03  ..t.j.d.....t.j.
-0000ddd0: 7d03 6402 7d04 7c01 6403 1600 7d05 6404  }.d.}.|.d...}.d.
-0000dde0: 7d06 7404 7405 1700 7406 1700 7d07 7c03  }.t.t...t...}.|.
-0000ddf0: 7c04 7c05 7c06 7c07 6705 7d08 7c02 6700  |.|.|.|.g.}.|.g.
-0000de00: 6b02 724c 7406 6405 6701 1400 7d02 7407  k.rLt.d.g...}.t.
-0000de10: 7c02 8301 7408 6b08 7260 7409 7c02 8301  |...t.k.r`t.|...
-0000de20: 7d02 7409 740a 6a0b 7408 7c00 6a0c 8301  }.t.t.j.t.|.j...
-0000de30: 7408 7c08 7c00 6a0d 1700 8301 740e 6a0f  t.|.|.j.....t.j.
-0000de40: 8303 6a10 8300 8301 7d09 7c00 6a0d 7c09  ..j.....}.|.j.|.
-0000de50: 1700 7c02 1700 7d0a 7411 7c0a 8301 7c07  ..|...}.t.|...|.
-0000de60: 6b03 72ba 7412 6406 7411 7c0a 8301 9b00  k.r.t.d.t.|.....
-0000de70: 6407 7c07 9b00 9d04 8301 8201 7c08 7c0a  d.|.........|.|.
-0000de80: 1700 7d0b 7c00 6a13 7c0b 8301 5c03 7d0c  ..}.|.j.|...\.}.
-0000de90: 7d0d 7d0e 7c00 6a14 8300 0100 7c0c 7c0d  }.}.|.j.....|.|.
-0000dea0: 7c0e 6603 5300 2908 4e7a 1e49 6e20 7361  |.f.S.).Nz.In sa
-0000deb0: 746f 6469 6d65 5f73 6574 5f6b 6579 736c  todime_set_keysl
-0000dec0: 6f74 5f73 7461 7475 7372 8a00 0000 72ba  ot_statusr....r.
-0000ded0: 0000 0072 0c00 0000 7201 0000 007a 3a45  ...r....r....z:E
-0000dee0: 7272 6f72 2069 6e20 7361 746f 6469 6d65  rror in satodime
-0000def0: 5f73 6574 5f6b 6579 736c 6f74 5f73 7461  _set_keyslot_sta
-0000df00: 7475 733a 2077 726f 6e67 2073 7461 7475  tus: wrong statu
-0000df10: 7320 6c65 6e67 7468 207a 0c20 696e 7374  s length z. inst
-0000df20: 6561 6420 6f66 2029 1572 2700 0000 7234  ead of ).r'...r4
-0000df30: 0000 0072 2b00 0000 72bc 0000 0072 7f00  ...r+...r....r..
-0000df40: 0000 7288 0100 005a 0953 495a 455f 4441  ..r....Z.SIZE_DA
-0000df50: 5441 7226 0000 0072 4b00 0000 72c6 0000  TAr&...rK...r...
-0000df60: 0072 eb00 0000 7289 0100 0072 7e00 0000  .r....r....r~...
-0000df70: 7280 0000 0072 4f00 0000 7250 0000 0072  r....rO...rP...r
-0000df80: 8a01 0000 7235 0000 0072 5300 0000 7299  ....r5...rS...r.
-0000df90: 0000 0072 7d01 0000 290f 7236 0000 0072  ...r}...).r6...r
-0000dfa0: 8301 0000 5a08 6b65 795f 6461 7461 729f  ....Z.key_datar.
-0000dfb0: 0000 0072 8700 0000 72a0 0000 0072 a100  ...r....r....r..
-0000dfc0: 0000 728b 0100 0072 8c01 0000 728d 0100  ..r....r....r...
-0000dfd0: 0072 c900 0000 7298 0000 0072 2200 0000  .r....r....r"...
-0000dfe0: 725d 0000 0072 5e00 0000 7237 0000 0072  r]...r^...r7...r
-0000dff0: 3700 0000 7238 0000 00da 2173 6174 6f64  7...r8....!satod
-0000e000: 696d 655f 7365 745f 6b65 7973 6c6f 745f  ime_set_keyslot_
-0000e010: 7374 6174 7573 5f70 6172 7431 3608 0000  status_part16...
-0000e020: 7326 0000 0000 020a 0106 0104 0108 0104  s&..............
-0000e030: 010c 010e 0208 000a 010c 0008 0328 020e  .............(..
-0000e040: 010c 0118 0108 0210 0108 027a 2f43 6172  ...........z/Car
-0000e050: 6443 6f6e 6e65 6374 6f72 2e73 6174 6f64  dConnector.satod
-0000e060: 696d 655f 7365 745f 6b65 7973 6c6f 745f  ime_set_keyslot_
-0000e070: 7374 6174 7573 5f70 6172 7431 6302 0000  status_part1c...
-0000e080: 0000 0000 000d 0000 0005 0000 0043 0000  .............C..
-0000e090: 0073 5c00 0000 7400 6a01 6401 8301 0100  .s\...t.j.d.....
-0000e0a0: 7402 6a03 7d02 6402 7d03 7c01 6403 1600  t.j.}.d.}.|.d...
-0000e0b0: 7d04 6404 7d05 7c02 7c03 7c04 7c05 6704  }.d.}.|.|.|.|.g.
-0000e0c0: 7d06 7c00 6a04 7c06 8301 5c03 7d07 7d08  }.|.j.|...\.}.}.
-0000e0d0: 7d09 7c00 6a05 6a06 7c07 8301 5c03 7d0a  }.|.j.j.|...\.}.
-0000e0e0: 7d0b 7d0c 7c07 7c08 7c09 7c0a 7c0b 6605  }.}.|.|.|.|.|.f.
-0000e0f0: 5300 2905 4e7a 1649 6e20 7361 746f 6469  S.).Nz.In satodi
-0000e100: 6d65 5f67 6574 5f70 7562 6b65 79e9 5500  me_get_pubkey.U.
-0000e110: 0000 72ba 0000 0072 0100 0000 2907 7227  ..r....r....).r'
-0000e120: 0000 0072 3400 0000 722b 0000 0072 bc00  ...r4...r+...r..
-0000e130: 0000 7299 0000 0072 7600 0000 da19 7061  ..r....rv.....pa
-0000e140: 7273 655f 7361 746f 6469 6d65 5f67 6574  rse_satodime_get
-0000e150: 5f70 7562 6b65 7929 0d72 3600 0000 7283  _pubkey).r6...r.
-0000e160: 0100 0072 9f00 0000 7287 0000 0072 a000  ...r....r....r..
-0000e170: 0000 72a1 0000 0072 9800 0000 7222 0000  ..r....r....r"..
-0000e180: 0072 5d00 0000 725e 0000 0072 fc00 0000  .r]...r^...r....
-0000e190: da10 7075 626b 6579 5f63 6f6d 705f 6c69  ..pubkey_comp_li
-0000e1a0: 7374 da08 7369 675f 6c69 7374 7237 0000  st..sig_listr7..
-0000e1b0: 0072 3700 0000 7238 0000 00da 1373 6174  .r7...r8.....sat
-0000e1c0: 6f64 696d 655f 6765 745f 7075 626b 6579  odime_get_pubkey
-0000e1d0: 5008 0000 7312 0000 0000 010a 0106 0104  P...s...........
-0000e1e0: 0108 0104 020c 0110 0312 027a 2143 6172  ...........z!Car
-0000e1f0: 6443 6f6e 6e65 6374 6f72 2e73 6174 6f64  dConnector.satod
-0000e200: 696d 655f 6765 745f 7075 626b 6579 6302  ime_get_pubkeyc.
-0000e210: 0000 0000 0000 0011 0000 0006 0000 0043  ...............C
-0000e220: 0000 0073 ce00 0000 7400 6a01 6401 8301  ...s....t.j.d...
-0000e230: 0100 7402 6a03 7d02 6402 7d03 7c01 6403  ..t.j.}.d.}.|.d.
-0000e240: 1600 7d04 6404 7d05 7404 7405 1700 7d06  ..}.d.}.t.t...}.
-0000e250: 7c02 7c03 7c04 7c05 7c06 6705 7d07 7406  |.|.|.|.|.g.}.t.
-0000e260: 7407 6a08 7409 7c00 6a0a 8301 7409 7c07  t.j.t.|.j...t.|.
-0000e270: 7c00 6a0b 1700 8301 740c 6a0d 8303 6a0e  |.j.....t.j...j.
-0000e280: 8300 8301 7d08 7c00 6a0b 7c08 1700 7d09  ....}.|.j.|...}.
-0000e290: 740f 7c09 8301 7c06 6b03 728c 7410 6405  t.|...|.k.r.t.d.
-0000e2a0: 740f 7c09 8301 9b00 6406 7c06 9b00 9d04  t.|.....d.|.....
-0000e2b0: 8301 8201 7c07 7c09 1700 7d0a 7c00 6a11  ....|.|...}.|.j.
-0000e2c0: 7c0a 8301 5c03 7d0b 7d0c 7d0d 7c00 6a12  |...\.}.}.}.|.j.
-0000e2d0: 8300 0100 7c00 6a13 6a14 7c0b 7c01 8302  ....|.j.j.|.|...
-0000e2e0: 5c03 7d0e 7d0f 7d10 7c0b 7c0c 7c0d 7c0e  \.}.}.}.|.|.|.|.
-0000e2f0: 7c0f 6605 5300 2907 4e7a 1749 6e20 7361  |.f.S.).Nz.In sa
-0000e300: 746f 6469 6d65 5f67 6574 5f70 7269 766b  todime_get_privk
-0000e310: 6579 e956 0000 0072 ba00 0000 7201 0000  ey.V...r....r...
-0000e320: 007a 2e45 7272 6f72 2069 6e20 7361 746f  .z.Error in sato
-0000e330: 6469 6d65 5f73 6561 6c5f 6b65 793a 2077  dime_seal_key: w
-0000e340: 726f 6e67 2064 6174 6120 6c65 6e67 7468  rong data length
-0000e350: 207a 0c20 696e 7374 6561 6420 6f66 2029   z. instead of )
-0000e360: 1572 2700 0000 7234 0000 0072 2b00 0000  .r'...r4...r+...
-0000e370: 72bc 0000 0072 7f00 0000 7288 0100 0072  r....r....r....r
-0000e380: c600 0000 72eb 0000 0072 8901 0000 724b  ....r....r....rK
-0000e390: 0000 0072 7e00 0000 7280 0000 0072 4f00  ...r~...r....rO.
-0000e3a0: 0000 7250 0000 0072 8a01 0000 7235 0000  ..rP...r....r5..
-0000e3b0: 0072 5300 0000 7299 0000 0072 7d01 0000  .rS...r....r}...
-0000e3c0: 7276 0000 00da 1a70 6172 7365 5f73 6174  rv.....parse_sat
-0000e3d0: 6f64 696d 655f 6765 745f 7072 6976 6b65  odime_get_privke
-0000e3e0: 7929 1172 3600 0000 7283 0100 0072 9f00  y).r6...r....r..
-0000e3f0: 0000 7287 0000 0072 a000 0000 72a1 0000  ..r....r....r...
-0000e400: 0072 8b01 0000 728c 0100 0072 8d01 0000  .r....r....r....
-0000e410: 72c9 0000 0072 9800 0000 7222 0000 0072  r....r....r"...r
-0000e420: 5d00 0000 725e 0000 00da 0c65 6e74 726f  ]...r^.....entro
-0000e430: 7079 5f6c 6973 74da 0c70 7269 766b 6579  py_list..privkey
-0000e440: 5f6c 6973 7472 9301 0000 7237 0000 0072  _listr....r7...r
-0000e450: 3700 0000 7238 0000 00da 1473 6174 6f64  7...r8.....satod
-0000e460: 696d 655f 6765 745f 7072 6976 6b65 795f  ime_get_privkey_
-0000e470: 0800 0073 2000 0000 0001 0a01 0601 0401  ...s ...........
-0000e480: 0801 0401 0801 0e03 2802 0a01 0c01 1801  ........(.......
-0000e490: 0801 1001 0803 1402 7a22 4361 7264 436f  ........z"CardCo
-0000e4a0: 6e6e 6563 746f 722e 7361 746f 6469 6d65  nnector.satodime
-0000e4b0: 5f67 6574 5f70 7269 766b 6579 6303 0000  _get_privkeyc...
-0000e4c0: 0000 0000 0012 0000 0006 0000 0043 0000  .............C..
-0000e4d0: 0073 e800 0000 7400 6a01 6401 8301 0100  .s....t.j.d.....
-0000e4e0: 7402 6a03 7d03 6402 7d04 7c01 6403 1600  t.j.}.d.}.|.d...
-0000e4f0: 7d05 6404 7d06 7404 7405 1700 7406 1700  }.d.}.t.t...t...
-0000e500: 7d07 7c03 7c04 7c05 7c06 7c07 6705 7d08  }.|.|.|.|.|.g.}.
-0000e510: 7407 7c02 8301 7408 6b08 724e 7409 7c02  t.|...t.k.rNt.|.
-0000e520: 8301 7d02 7409 740a 6a0b 7408 7c00 6a0c  ..}.t.t.j.t.|.j.
-0000e530: 8301 7408 7c08 7c00 6a0d 1700 8301 740e  ..t.|.|.j.....t.
-0000e540: 6a0f 8303 6a10 8300 8301 7d09 7c00 6a0d  j...j.....}.|.j.
-0000e550: 7c09 1700 7c02 1700 7d0a 7411 7c0a 8301  |...|...}.t.|...
-0000e560: 7c07 6b03 72a8 7412 6405 7411 7c0a 8301  |.k.r.t.d.t.|...
-0000e570: 9b00 6406 7c07 9b00 9d04 8301 8201 7c08  ..d.|.........|.
-0000e580: 7c0a 1700 7d0b 7c00 6a13 7c0b 8301 5c03  |...}.|.j.|...\.
-0000e590: 7d0c 7d0d 7d0e 7c00 6a14 8300 0100 7c00  }.}.}.|.j.....|.
-0000e5a0: 6a15 6a16 7c0c 8301 5c03 7d0f 7d10 7d11  j.j.|...\.}.}.}.
-0000e5b0: 7c0c 7c0d 7c0e 7c0f 7c10 6605 5300 2907  |.|.|.|.|.f.S.).
-0000e5c0: 4e7a 1449 6e20 7361 746f 6469 6d65 5f73  Nz.In satodime_s
-0000e5d0: 6561 6c5f 6b65 79e9 5700 0000 72ba 0000  eal_key.W...r...
-0000e5e0: 0072 0100 0000 7a2e 4572 726f 7220 696e  .r....z.Error in
-0000e5f0: 2073 6174 6f64 696d 655f 7365 616c 5f6b   satodime_seal_k
-0000e600: 6579 3a20 7772 6f6e 6720 6461 7461 206c  ey: wrong data l
-0000e610: 656e 6774 6820 7a0c 2069 6e73 7465 6164  ength z. instead
-0000e620: 206f 6620 2917 7227 0000 0072 3400 0000   of ).r'...r4...
-0000e630: 722b 0000 0072 bc00 0000 727f 0000 0072  r+...r....r....r
-0000e640: 8801 0000 5a0c 5349 5a45 5f45 4e54 524f  ....Z.SIZE_ENTRO
-0000e650: 5059 7226 0000 0072 4b00 0000 72c6 0000  PYr&...rK...r...
-0000e660: 0072 eb00 0000 7289 0100 0072 7e00 0000  .r....r....r~...
-0000e670: 7280 0000 0072 4f00 0000 7250 0000 0072  r....rO...rP...r
-0000e680: 8a01 0000 7235 0000 0072 5300 0000 7299  ....r5...rS...r.
-0000e690: 0000 0072 7d01 0000 7276 0000 0072 9101  ...r}...rv...r..
-0000e6a0: 0000 2912 7236 0000 0072 8301 0000 5a0c  ..).r6...r....Z.
-0000e6b0: 656e 7472 6f70 795f 7573 6572 729f 0000  entropy_userr...
-0000e6c0: 0072 8700 0000 72a0 0000 0072 a100 0000  .r....r....r....
-0000e6d0: 728b 0100 0072 8c01 0000 728d 0100 0072  r....r....r....r
-0000e6e0: c900 0000 7298 0000 0072 2200 0000 725d  ....r....r"...r]
-0000e6f0: 0000 0072 5e00 0000 72fc 0000 0072 9201  ...r^...r....r..
-0000e700: 0000 7293 0100 0072 3700 0000 7237 0000  ..r....r7...r7..
-0000e710: 0072 3800 0000 da11 7361 746f 6469 6d65  .r8.....satodime
-0000e720: 5f73 6561 6c5f 6b65 7977 0800 0073 2400  _seal_keyw...s$.
-0000e730: 0000 0002 0a01 0601 0401 0801 0401 0c01  ................
-0000e740: 0e02 0c00 0803 2802 0e01 0c01 1801 0802  ......(.........
-0000e750: 1001 0803 1202 7a1f 4361 7264 436f 6e6e  ......z.CardConn
-0000e760: 6563 746f 722e 7361 746f 6469 6d65 5f73  ector.satodime_s
-0000e770: 6561 6c5f 6b65 7963 0200 0000 0000 0000  eal_keyc........
-0000e780: 1100 0000 0600 0000 4300 0000 73ce 0000  ........C...s...
-0000e790: 0074 006a 0164 0183 0101 0074 026a 037d  .t.j.d.....t.j.}
-0000e7a0: 0264 027d 037c 0164 0316 007d 0464 047d  .d.}.|.d...}.d.}
-0000e7b0: 0574 0474 0517 007d 067c 027c 037c 047c  .t.t...}.|.|.|.|
-0000e7c0: 057c 0667 057d 0774 0674 076a 0874 097c  .|.g.}.t.t.j.t.|
-0000e7d0: 006a 0a83 0174 097c 077c 006a 0b17 0083  .j...t.|.|.j....
-0000e7e0: 0174 0c6a 0d83 036a 0e83 0083 017d 087c  .t.j...j.....}.|
-0000e7f0: 006a 0b7c 0817 007d 0974 0f7c 0983 017c  .j.|...}.t.|...|
-0000e800: 066b 0372 8c74 1064 0574 0f7c 0983 019b  .k.r.t.d.t.|....
-0000e810: 0064 067c 069b 009d 0483 0182 017c 077c  .d.|.........|.|
-0000e820: 0917 007d 0a7c 006a 117c 0a83 015c 037d  ...}.|.j.|...\.}
-0000e830: 0b7d 0c7d 0d7c 006a 1283 0001 007c 006a  .}.}.|.j.....|.j
-0000e840: 136a 147c 0b7c 0183 025c 037d 0e7d 0f7d  .j.|.|...\.}.}.}
-0000e850: 107c 0b7c 0c7c 0d7c 0e7c 0f66 0553 0029  .|.|.|.|.|.f.S.)
-0000e860: 074e 7a16 496e 2073 6174 6f64 696d 655f  .Nz.In satodime_
-0000e870: 756e 7365 616c 5f6b 6579 e958 0000 0072  unseal_key.X...r
-0000e880: ba00 0000 7201 0000 007a 3045 7272 6f72  ....r....z0Error
-0000e890: 2069 6e20 7361 746f 6469 6d65 5f75 6e73   in satodime_uns
-0000e8a0: 6561 6c5f 6b65 793a 2077 726f 6e67 2064  eal_key: wrong d
-0000e8b0: 6174 6120 6c65 6e67 7468 207a 0c20 696e  ata length z. in
-0000e8c0: 7374 6561 6420 6f66 2029 1572 2700 0000  stead of ).r'...
-0000e8d0: 7234 0000 0072 2b00 0000 72bc 0000 0072  r4...r+...r....r
-0000e8e0: 7f00 0000 7288 0100 0072 c600 0000 72eb  ....r....r....r.
-0000e8f0: 0000 0072 8901 0000 724b 0000 0072 7e00  ...r....rK...r~.
-0000e900: 0000 7280 0000 0072 4f00 0000 7250 0000  ..r....rO...rP..
-0000e910: 0072 8a01 0000 7235 0000 0072 5300 0000  .r....r5...rS...
-0000e920: 7299 0000 0072 7d01 0000 7276 0000 0072  r....r}...rv...r
-0000e930: 9601 0000 2911 7236 0000 0072 8301 0000  ....).r6...r....
-0000e940: 729f 0000 0072 8700 0000 72a0 0000 0072  r....r....r....r
-0000e950: a100 0000 728b 0100 0072 8c01 0000 728d  ....r....r....r.
-0000e960: 0100 0072 c900 0000 7298 0000 0072 2200  ...r....r....r".
-0000e970: 0000 725d 0000 0072 5e00 0000 7297 0100  ..r]...r^...r...
-0000e980: 0072 9801 0000 7293 0100 0072 3700 0000  .r....r....r7...
-0000e990: 7237 0000 0072 3800 0000 da13 7361 746f  r7...r8.....sato
-0000e9a0: 6469 6d65 5f75 6e73 6561 6c5f 6b65 7993  dime_unseal_key.
-0000e9b0: 0800 0073 2000 0000 0001 0a01 0601 0401  ...s ...........
-0000e9c0: 0801 0401 0801 0e03 2802 0a01 0c01 1801  ........(.......
-0000e9d0: 0802 1001 0803 1402 7a21 4361 7264 436f  ........z!CardCo
-0000e9e0: 6e6e 6563 746f 722e 7361 746f 6469 6d65  nnector.satodime
-0000e9f0: 5f75 6e73 6561 6c5f 6b65 7963 0200 0000  _unseal_keyc....
-0000ea00: 0000 0000 0e00 0000 0600 0000 4300 0000  ............C...
-0000ea10: 73b6 0000 0074 006a 0164 0183 0101 0074  s....t.j.d.....t
-0000ea20: 026a 037d 0264 027d 037c 0164 0316 007d  .j.}.d.}.|.d...}
-0000ea30: 0464 047d 0574 0474 0517 007d 067c 027c  .d.}.t.t...}.|.|
-0000ea40: 037c 047c 057c 0667 057d 0774 0674 076a  .|.|.|.g.}.t.t.j
-0000ea50: 0874 097c 006a 0a83 0174 097c 077c 006a  .t.|.j...t.|.|.j
-0000ea60: 0b17 0083 0174 0c6a 0d83 036a 0e83 0083  .....t.j...j....
-0000ea70: 017d 087c 006a 0b7c 0817 007d 0974 0f7c  .}.|.j.|...}.t.|
-0000ea80: 0983 017c 066b 0372 8c74 1064 0574 0f7c  ...|.k.r.t.d.t.|
-0000ea90: 0983 019b 0064 067c 069b 009d 0483 0182  .....d.|........
-0000eaa0: 017c 077c 0917 007d 0a7c 006a 117c 0a83  .|.|...}.|.j.|..
-0000eab0: 015c 037d 0b7d 0c7d 0d7c 006a 1283 0001  .\.}.}.}.|.j....
-0000eac0: 007c 0b7c 0c7c 0d66 0353 0029 074e 7a15  .|.|.|.f.S.).Nz.
-0000ead0: 496e 2073 6174 6f64 696d 655f 7265 7365  In satodime_rese
-0000eae0: 745f 6b65 79e9 5900 0000 72ba 0000 0072  t_key.Y...r....r
-0000eaf0: 0100 0000 7a30 4572 726f 7220 696e 2073  ....z0Error in s
-0000eb00: 6174 6f64 696d 655f 756e 7365 616c 5f6b  atodime_unseal_k
-0000eb10: 6579 3a20 7772 6f6e 6720 6461 7461 206c  ey: wrong data l
-0000eb20: 656e 6774 6820 7a0c 2069 6e73 7465 6164  ength z. instead
-0000eb30: 206f 6620 2913 7227 0000 0072 3400 0000   of ).r'...r4...
-0000eb40: 722b 0000 0072 bc00 0000 727f 0000 0072  r+...r....r....r
-0000eb50: 8801 0000 72c6 0000 0072 eb00 0000 7289  ....r....r....r.
-0000eb60: 0100 0072 4b00 0000 727e 0000 0072 8000  ...rK...r~...r..
-0000eb70: 0000 724f 0000 0072 5000 0000 728a 0100  ..rO...rP...r...
-0000eb80: 0072 3500 0000 7253 0000 0072 9900 0000  .r5...rS...r....
-0000eb90: 727d 0100 0029 0e72 3600 0000 7283 0100  r}...).r6...r...
-0000eba0: 0072 9f00 0000 7287 0000 0072 a000 0000  .r....r....r....
-0000ebb0: 72a1 0000 0072 8b01 0000 728c 0100 0072  r....r....r....r
-0000ebc0: 8d01 0000 72c9 0000 0072 9800 0000 7222  ....r....r....r"
-0000ebd0: 0000 0072 5d00 0000 725e 0000 0072 3700  ...r]...r^...r7.
-0000ebe0: 0000 7237 0000 0072 3800 0000 da12 7361  ..r7...r8.....sa
-0000ebf0: 746f 6469 6d65 5f72 6573 6574 5f6b 6579  todime_reset_key
-0000ec00: ac08 0000 731e 0000 0000 010a 0106 0104  ....s...........
-0000ec10: 0108 0104 0108 010e 0328 020a 010c 0118  .........(......
-0000ec20: 0108 0210 0108 027a 2043 6172 6443 6f6e  .......z CardCon
-0000ec30: 6e65 6374 6f72 2e73 6174 6f64 696d 655f  nector.satodime_
-0000ec40: 7265 7365 745f 6b65 7963 0100 0000 0000  reset_keyc......
-0000ec50: 0000 0d00 0000 0600 0000 4300 0000 738e  ..........C...s.
-0000ec60: 0000 0074 006a 0164 0183 0101 0074 026a  ...t.j.d.....t.j
-0000ec70: 037d 0164 027d 0264 037d 0364 037d 0474  .}.d.}.d.}.d.}.t
-0000ec80: 0474 0517 007d 057c 017c 027c 037c 047c  .t...}.|.|.|.|.|
-0000ec90: 0567 057d 0674 0674 076a 0874 097c 006a  .g.}.t.t.j.t.|.j
-0000eca0: 0a83 0174 097c 067c 006a 0b17 0083 0174  ...t.|.|.j.....t
-0000ecb0: 0c6a 0d83 036a 0e83 0083 017d 077c 006a  .j...j.....}.|.j
-0000ecc0: 0b7c 0717 007d 087c 067c 0817 007d 097c  .|...}.|.|...}.|
-0000ecd0: 006a 0f7c 0983 015c 037d 0a7d 0b7d 0c7c  .j.|...\.}.}.}.|
-0000ece0: 006a 1083 0001 007c 0a7c 0b7c 0c66 0353  .j.....|.|.|.f.S
-0000ecf0: 0029 044e 7a27 496e 2073 6174 6f64 696d  .).Nz'In satodim
-0000ed00: 655f 696e 6974 6961 7465 5f6f 776e 6572  e_initiate_owner
-0000ed10: 7368 6970 5f74 7261 6e73 6665 72e9 5a00  ship_transfer.Z.
-0000ed20: 0000 7201 0000 0029 1172 2700 0000 7234  ..r....).r'...r4
-0000ed30: 0000 0072 2b00 0000 72bc 0000 0072 7f00  ...r+...r....r..
-0000ed40: 0000 7288 0100 0072 c600 0000 72eb 0000  ..r....r....r...
-0000ed50: 0072 8901 0000 724b 0000 0072 7e00 0000  .r....rK...r~...
-0000ed60: 7280 0000 0072 4f00 0000 7250 0000 0072  r....rO...rP...r
-0000ed70: 8a01 0000 7299 0000 0072 7d01 0000 290d  ....r....r}...).
-0000ed80: 7236 0000 0072 9f00 0000 7287 0000 0072  r6...r....r....r
-0000ed90: a000 0000 72a1 0000 0072 8b01 0000 728c  ....r....r....r.
-0000eda0: 0100 0072 8d01 0000 72c9 0000 0072 9800  ...r....r....r..
-0000edb0: 0000 7222 0000 0072 5d00 0000 725e 0000  ..r"...r]...r^..
-0000edc0: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
-0000edd0: da24 7361 746f 6469 6d65 5f69 6e69 7469  .$satodime_initi
-0000ede0: 6174 655f 6f77 6e65 7273 6869 705f 7472  ate_ownership_tr
-0000edf0: 616e 7366 6572 c208 0000 731a 0000 0000  ansfer....s.....
-0000ee00: 020a 0106 0104 0104 0104 0108 010e 0328  ...............(
-0000ee10: 020a 0108 0110 0108 027a 3243 6172 6443  .........z2CardC
-0000ee20: 6f6e 6e65 6374 6f72 2e73 6174 6f64 696d  onnector.satodim
-0000ee30: 655f 696e 6974 6961 7465 5f6f 776e 6572  e_initiate_owner
-0000ee40: 7368 6970 5f74 7261 6e73 6665 7263 0200  ship_transferc..
-0000ee50: 0000 0000 0000 0800 0000 0400 0000 4300  ..............C.
-0000ee60: 0000 735a 0000 0074 0064 0164 0283 027d  ..sZ...t.d.d...}
-0000ee70: 0274 007c 0183 017d 0374 016a 027c 027c  .t.|...}.t.j.|.|
-0000ee80: 0374 036a 0483 036a 0583 0064 0364 0485  .t.j...j...d.d..
-0000ee90: 0219 007d 0474 067c 0483 017d 057c 056a  ...}.t.|...}.|.j
-0000eea0: 0764 0583 017d 067c 066a 0883 007d 0774  .d...}.|.j...}.t
-0000eeb0: 096a 0a64 067c 0717 0083 0101 007c 0753  .j.d.|.......|.S
-0000eec0: 0029 074e 7a0d 4269 7463 6f69 6e20 7365  .).Nz.Bitcoin se
-0000eed0: 6564 3272 bf00 0000 7201 0000 0072 0d01  ed2r....r....r..
-0000eee0: 0000 547a 1341 7574 6865 6e74 696b 6579  ..Tz.Authentikey
-0000eef0: 5f6c 6f63 616c 3d20 290b 724b 0000 0072  _local= ).rK...r
-0000ef00: eb00 0000 7289 0100 0072 4f00 0000 5a06  ....r....rO...Z.
-0000ef10: 7368 6135 3132 728a 0100 0072 1100 0000  sha512r....r....
-0000ef20: 72e1 0000 0072 4c00 0000 7227 0000 0072  r....rL...r'...r
-0000ef30: 3400 0000 2908 7236 0000 005a 0a6d 6173  4...).r6...Z.mas
-0000ef40: 7465 7273 6565 645a 0762 7974 656b 6579  terseedZ.bytekey
-0000ef50: 5a08 6279 7465 7365 6564 724e 0100 005a  Z.byteseedrN...Z
-0000ef60: 0470 7269 765a 0370 7562 5a07 7075 625f  .privZ.pubZ.pub_
-0000ef70: 6865 7872 3700 0000 7237 0000 0072 3800  hexr7...r7...r8.
-0000ef80: 0000 da1f 6765 745f 6175 7468 656e 7469  ....get_authenti
-0000ef90: 6b65 795f 6672 6f6d 5f6d 6173 7465 7273  key_from_masters
-0000efa0: 6565 64db 0800 0073 1000 0000 0003 0a01  eed....s........
-0000efb0: 0801 1c01 0801 0a01 0801 0e02 7a2d 4361  ............z-Ca
-0000efc0: 7264 436f 6e6e 6563 746f 722e 6765 745f  rdConnector.get_
-0000efd0: 6175 7468 656e 7469 6b65 795f 6672 6f6d  authentikey_from
-0000efe0: 5f6d 6173 7465 7273 6565 6429 0372 0100  _masterseed).r..
-0000eff0: 0000 4e72 0100 0000 2902 721c 0100 004e  ..Nr....).r....N
-0000f000: 2901 4629 0154 2901 4e29 014e 2901 5429  ).F).T).N).N).T)
-0000f010: 5072 3a00 0000 723b 0000 0072 3c00 0000  Pr:...r;...r<...
-0000f020: 72ac 0000 0072 ad00 0000 72ae 0000 0072  r....r....r....r
-0000f030: b000 0000 da07 6c6f 6767 696e 67da 0757  ......logging..W
-0000f040: 4152 4e49 4e47 7240 0000 0072 9900 0000  ARNINGr@...r....
-0000f050: 729a 0000 0072 4a00 0000 724d 0000 0072  r....rJ...rM...r
-0000f060: 4e00 0000 7256 0000 0072 a500 0000 7255  N...rV...r....rU
-0000f070: 0000 0072 a800 0000 72a9 0000 0072 aa00  ...r....r....r..
-0000f080: 0000 7257 0000 0072 c500 0000 72cb 0000  ..rW...r....r...
-0000f090: 0072 dc00 0000 72e6 0000 0072 f700 0000  .r....r....r....
-0000f0a0: 72fe 0000 0072 0001 0000 7204 0100 0072  r....r....r....r
-0000f0b0: 0601 0000 7208 0100 0072 e000 0000 7213  ....r....r....r.
-0000f0c0: 0100 0072 1b01 0000 7226 0100 0072 4b00  ...r....r&...rK.
-0000f0d0: 0000 7228 0100 0072 2d01 0000 722f 0100  ..r(...r-...r/..
-0000f0e0: 0072 3201 0000 7234 0100 0072 3d01 0000  .r2...r4...r=...
-0000f0f0: 723f 0100 0072 4001 0000 7290 0000 0072  r?...r@...r....r
-0000f100: d600 0000 7249 0100 0072 4a01 0000 724b  ....rI...rJ...rK
-0000f110: 0100 0072 5900 0000 728d 0000 0072 8f00  ...rY...r....r..
-0000f120: 0000 7275 0000 0072 5501 0000 7257 0100  ..ru...rU...rW..
-0000f130: 0072 5d01 0000 7267 0100 0072 6901 0000  .r]...rg...ri...
-0000f140: 726d 0100 0072 6f01 0000 7270 0100 0072  rm...ro...rp...r
-0000f150: 7101 0000 7272 0100 0072 7801 0000 72d8  q...rr...rx...r.
-0000f160: 0000 0072 d700 0000 727d 0100 0072 8201  ...r....r}...r..
-0000f170: 0000 727a 0100 0072 8401 0000 728e 0100  ..rz...r....r...
-0000f180: 0072 8f01 0000 7294 0100 0072 9901 0000  .r....r....r....
-0000f190: 729b 0100 0072 9d01 0000 729f 0100 0072  r....r....r....r
-0000f1a0: a101 0000 72a2 0100 0072 3700 0000 7237  ....r....r7...r7
-0000f1b0: 0000 0072 3700 0000 7238 0000 0072 6300  ...r7...r8...rc.
-0000f1c0: 0000 8f00 0000 7390 0000 0008 0d0c 0114  ......s.........
-0000f1d0: 0118 0114 0212 2b08 2c08 0408 0b08 0b08  ......+.,.......
-0000f1e0: 0b08 1508 0308 1808 0708 0708 0708 3108  ..............1.
-0000f1f0: 1908 140a 3308 3008 4008 2708 1508 1e0c  ....3.0.@.'.....
-0000f200: 2108 1e08 1308 3808 260a 5710 2f08 2308  !.....8.&.W./.#.
-0000f210: 2708 2108 1d0a 6a08 0e08 0c08 3e08 0508  '.!...j.....>...
-0000f220: 2708 2308 1108 1708 1808 1a0e 1c0e 1c0a  '.#.............
-0000f230: 4e0a 5c08 230a 4208 1a08 1208 3608 1108  N.\.#.B.....6...
-0000f240: 340c 040c 0408 0508 230e 1414 1e0e 1a0e  4.......#.......
-0000f250: 0f0e 180e 1c0e 190e 1608 1972 6300 0000  ...........rc...
-0000f260: 6300 0000 0000 0000 0000 0000 0004 0000  c...............
-0000f270: 0000 0000 0073 2600 0000 6500 5a01 6400  .....s&...e.Z.d.
-0000f280: 5a02 6401 6401 6401 6700 6604 8700 6601  Z.d.d.d.g.f...f.
-0000f290: 6402 6403 8409 5a03 8700 0400 5a04 5300  d.d...Z.....Z.S.
-0000f2a0: 2904 da09 4170 6475 4572 726f 7272 0100  )...ApduErrorr..
-0000f2b0: 0000 6306 0000 0000 0000 0006 0000 0002  ..c.............
-0000f2c0: 0000 0003 0000 0073 2800 0000 7400 8300  .......s(...t...
-0000f2d0: 6a01 7c01 8301 0100 7c02 7c00 5f02 7c03  j.|.....|.|._.|.
-0000f2e0: 7c00 5f03 7c04 7c00 5f04 7c05 7c00 5f05  |._.|.|._.|.|._.
-0000f2f0: 6400 5300 2901 4e29 06da 0573 7570 6572  d.S.).N)...super
-0000f300: 7240 0000 0072 5d00 0000 725e 0000 0072  r@...r]...r^...r
-0000f310: 8700 0000 7222 0000 0029 0672 3600 0000  ....r"...).r6...
-0000f320: 7221 0100 0072 5d00 0000 725e 0000 0072  r!...r]...r^...r
-0000f330: 8700 0000 7222 0000 0029 01da 095f 5f63  ....r"...)...__c
-0000f340: 6c61 7373 5f5f 7237 0000 0072 3800 0000  lass__r7...r8...
-0000f350: 7240 0000 00ee 0800 0073 0a00 0000 0001  r@.......s......
-0000f360: 0c01 0601 0601 0601 7a12 4170 6475 4572  ........z.ApduEr
-0000f370: 726f 722e 5f5f 696e 6974 5f5f 2905 723a  ror.__init__).r:
-0000f380: 0000 0072 3b00 0000 723c 0000 0072 4000  ...r;...r<...r@.
-0000f390: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
-0000f3a0: 5f72 3700 0000 7237 0000 0029 0172 a701  _r7...r7...).r..
-0000f3b0: 0000 7238 0000 0072 a501 0000 ed08 0000  ..r8...r........
-0000f3c0: 7302 0000 0008 0172 a501 0000 6300 0000  s......r....c...
-0000f3d0: 0000 0000 0000 0000 0004 0000 0000 0000  ................
-0000f3e0: 0073 2200 0000 6500 5a01 6400 5a02 6401  .s"...e.Z.d.Z.d.
-0000f3f0: 6700 6602 8700 6601 6402 6403 8409 5a03  g.f...f.d.d...Z.
-0000f400: 8700 0400 5a04 5300 2904 7291 0000 0072  ....Z.S.).r....r
-0000f410: 0100 0000 6304 0000 0000 0000 0004 0000  ....c...........
-0000f420: 0006 0000 0003 0000 0073 1800 0000 7400  .........s....t.
-0000f430: 8300 6a01 7c01 6401 6402 7c02 7c03 8305  ..j.|.d.d.|.|...
-0000f440: 0100 6400 5300 2903 4e72 8600 0000 7284  ..d.S.).Nr....r.
-0000f450: 0000 0029 0272 a601 0000 7240 0000 0029  ...).r....r@...)
-0000f460: 0472 3600 0000 7221 0100 0072 8700 0000  .r6...r!...r....
-0000f470: 7222 0000 0029 0172 a701 0000 7237 0000  r"...).r....r7..
-0000f480: 0072 3800 0000 7240 0000 00f7 0800 0073  .r8...r@.......s
-0000f490: 0200 0000 0001 7a18 4361 7264 5365 6c65  ......z.CardSele
-0000f4a0: 6374 4572 726f 722e 5f5f 696e 6974 5f5f  ctError.__init__
-0000f4b0: 2905 723a 0000 0072 3b00 0000 723c 0000  ).r:...r;...r<..
-0000f4c0: 0072 4000 0000 72a8 0100 0072 3700 0000  .r@...r....r7...
-0000f4d0: 7237 0000 0029 0172 a701 0000 7238 0000  r7...).r....r8..
-0000f4e0: 0072 9100 0000 f608 0000 7302 0000 0008  .r........s.....
-0000f4f0: 0172 9100 0000 6300 0000 0000 0000 0000  .r....c.........
-0000f500: 0000 0004 0000 0000 0000 0073 2200 0000  ...........s"...
-0000f510: 6500 5a01 6400 5a02 6401 6700 6602 8700  e.Z.d.Z.d.g.f...
-0000f520: 6601 6402 6403 8409 5a03 8700 0400 5a04  f.d.d...Z.....Z.
-0000f530: 5300 2904 7281 0100 0072 0100 0000 6304  S.).r....r....c.
-0000f540: 0000 0000 0000 0004 0000 0006 0000 0003  ................
-0000f550: 0000 0073 1800 0000 7400 8300 6a01 7c01  ...s....t...j.|.
-0000f560: 6401 6402 7c02 7c03 8305 0100 6400 5300  d.d.|.|.....d.S.
-0000f570: 2903 4e72 4200 0000 7243 0000 0029 0272  ).NrB...rC...).r
-0000f580: a601 0000 7240 0000 0029 0472 3600 0000  ....r@...).r6...
-0000f590: 7221 0100 0072 8700 0000 7222 0000 0029  r!...r....r"...)
-0000f5a0: 0172 a701 0000 7237 0000 0072 3800 0000  .r....r7...r8...
-0000f5b0: 7240 0000 00fc 0800 0073 0200 0000 0001  r@.......s......
-0000f5c0: 7a1e 4361 7264 5365 7475 704e 6f74 446f  z.CardSetupNotDo
-0000f5d0: 6e65 4572 726f 722e 5f5f 696e 6974 5f5f  neError.__init__
-0000f5e0: 2905 723a 0000 0072 3b00 0000 723c 0000  ).r:...r;...r<..
-0000f5f0: 0072 4000 0000 72a8 0100 0072 3700 0000  .r@...r....r7...
-0000f600: 7237 0000 0029 0172 a701 0000 7238 0000  r7...).r....r8..
-0000f610: 0072 8101 0000 fb08 0000 7302 0000 0008  .r........s.....
-0000f620: 0172 8101 0000 6300 0000 0000 0000 0000  .r....c.........
-0000f630: 0000 0004 0000 0000 0000 0073 2200 0000  ...........s"...
-0000f640: 6500 5a01 6400 5a02 6401 6700 6602 8700  e.Z.d.Z.d.g.f...
-0000f650: 6601 6402 6403 8409 5a03 8700 0400 5a04  f.d.d...Z.....Z.
-0000f660: 5300 2904 7292 0000 0072 0100 0000 6304  S.).r....r....c.
-0000f670: 0000 0000 0000 0004 0000 0006 0000 0003  ................
-0000f680: 0000 0073 1800 0000 7400 8300 6a01 7c01  ...s....t...j.|.
-0000f690: 6401 6402 7c02 7c03 8305 0100 6400 5300  d.d.|.|.....d.S.
-0000f6a0: 2903 4e72 4200 0000 7288 0000 0029 0272  ).NrB...r....).r
-0000f6b0: a601 0000 7240 0000 0029 0472 3600 0000  ....r@...).r6...
-0000f6c0: 7221 0100 0072 8700 0000 7222 0000 0029  r!...r....r"...)
-0000f6d0: 0172 a701 0000 7237 0000 0072 3800 0000  .r....r7...r8...
-0000f6e0: 7240 0000 0000 0900 0073 0200 0000 0001  r@.......s......
-0000f6f0: 7a19 496e 636f 7272 6563 7450 3145 7272  z.IncorrectP1Err
-0000f700: 6f72 2e5f 5f69 6e69 745f 5f29 0572 3a00  or.__init__).r:.
-0000f710: 0000 723b 0000 0072 3c00 0000 7240 0000  ..r;...r<...r@..
-0000f720: 0072 a801 0000 7237 0000 0072 3700 0000  .r....r7...r7...
-0000f730: 2901 72a7 0100 0072 3800 0000 7292 0000  ).r....r8...r...
-0000f740: 00ff 0800 0073 0200 0000 0801 7292 0000  .....s......r...
-0000f750: 0063 0000 0000 0000 0000 0000 0000 0400  .c..............
-0000f760: 0000 0000 0000 7322 0000 0065 005a 0164  ......s"...e.Z.d
-0000f770: 005a 0264 0167 0066 0287 0066 0164 0264  .Z.d.g.f...f.d.d
-0000f780: 0384 095a 0387 0004 005a 0453 0029 0472  ...Z.....Z.S.).r
-0000f790: 9600 0000 7201 0000 0063 0400 0000 0000  ....r....c......
-0000f7a0: 0000 0400 0000 0600 0000 0300 0000 7318  ..............s.
-0000f7b0: 0000 0074 0083 006a 017c 0164 0164 027c  ...t...j.|.d.d.|
-0000f7c0: 027c 0383 0501 0064 0053 0029 034e 7242  .|.....d.S.).NrB
-0000f7d0: 0000 0072 8b00 0000 2902 72a6 0100 0072  ...r....).r....r
-0000f7e0: 4000 0000 2904 7236 0000 0072 2101 0000  @...).r6...r!...
-0000f7f0: 7287 0000 0072 2200 0000 2901 72a7 0100  r....r"...).r...
-0000f800: 0072 3700 0000 7238 0000 0072 4000 0000  .r7...r8...r@...
-0000f810: 0509 0000 7302 0000 0000 017a 2255 6e6b  ....s......z"Unk
-0000f820: 6e6f 776e 5072 6f74 6f63 6f6c 4d65 6469  nownProtocolMedi
-0000f830: 6145 7272 6f72 2e5f 5f69 6e69 745f 5f29  aError.__init__)
-0000f840: 0572 3a00 0000 723b 0000 0072 3c00 0000  .r:...r;...r<...
-0000f850: 7240 0000 0072 a801 0000 7237 0000 0072  r@...r....r7...r
-0000f860: 3700 0000 2901 72a7 0100 0072 3800 0000  7...).r....r8...
-0000f870: 7296 0000 0004 0900 0073 0200 0000 0801  r........s......
-0000f880: 7296 0000 0063 0000 0000 0000 0000 0000  r....c..........
-0000f890: 0000 0400 0000 0000 0000 7322 0000 0065  ..........s"...e
-0000f8a0: 005a 0164 005a 0264 0167 0066 0287 0066  .Z.d.Z.d.g.f...f
-0000f8b0: 0164 0264 0384 095a 0387 0004 005a 0453  .d.d...Z.....Z.S
-0000f8c0: 0029 0472 9500 0000 7201 0000 0063 0400  .).r....r....c..
-0000f8d0: 0000 0000 0000 0400 0000 0600 0000 0300  ................
-0000f8e0: 0000 7318 0000 0074 0083 006a 017c 0164  ..s....t...j.|.d
-0000f8f0: 0164 027c 027c 0383 0501 0064 0053 0029  .d.|.|.....d.S.)
-0000f900: 034e 7242 0000 0072 6500 0000 2902 72a6  .NrB...re...).r.
-0000f910: 0100 0072 4000 0000 2904 7236 0000 0072  ...r@...).r6...r
-0000f920: 2101 0000 7287 0000 0072 2200 0000 2901  !...r....r"...).
-0000f930: 72a7 0100 0072 3700 0000 7238 0000 0072  r....r7...r8...r
-0000f940: 4000 0000 0909 0000 7302 0000 0000 017a  @.......s......z
-0000f950: 2449 6e63 6f72 7265 6374 5072 6f74 6f63  $IncorrectProtoc
-0000f960: 6f6c 4d65 6469 6145 7272 6f72 2e5f 5f69  olMediaError.__i
-0000f970: 6e69 745f 5f29 0572 3a00 0000 723b 0000  nit__).r:...r;..
-0000f980: 0072 3c00 0000 7240 0000 0072 a801 0000  .r<...r@...r....
-0000f990: 7237 0000 0072 3700 0000 2901 72a7 0100  r7...r7...).r...
-0000f9a0: 0072 3800 0000 7295 0000 0008 0900 0073  .r8...r........s
-0000f9b0: 0200 0000 0801 7295 0000 0063 0000 0000  ......r....c....
-0000f9c0: 0000 0000 0000 0000 0400 0000 0000 0000  ................
-0000f9d0: 7322 0000 0065 005a 0164 005a 0264 0167  s"...e.Z.d.Z.d.g
-0000f9e0: 0066 0287 0066 0164 0264 0384 095a 0387  .f...f.d.d...Z..
-0000f9f0: 0004 005a 0453 0029 0472 9400 0000 7201  ...Z.S.).r....r.
-0000fa00: 0000 0063 0400 0000 0000 0000 0400 0000  ...c............
-0000fa10: 0600 0000 0300 0000 7318 0000 0074 0083  ........s....t..
-0000fa20: 006a 017c 0164 0164 027c 027c 0383 0501  .j.|.d.d.|.|....
-0000fa30: 0064 0053 0029 034e 7242 0000 0072 8a00  .d.S.).NrB...r..
-0000fa40: 0000 2902 72a6 0100 0072 4000 0000 2904  ..).r....r@...).
-0000fa50: 7236 0000 0072 2101 0000 7287 0000 0072  r6...r!...r....r
-0000fa60: 2200 0000 2901 72a7 0100 0072 3700 0000  "...).r....r7...
-0000fa70: 7238 0000 0072 4000 0000 0d09 0000 7302  r8...r@.......s.
-0000fa80: 0000 0000 017a 2349 6e63 6f72 7265 6374  .....z#Incorrect
-0000fa90: 4b65 7973 6c6f 7453 7461 7465 4572 726f  KeyslotStateErro
-0000faa0: 722e 5f5f 696e 6974 5f5f 2905 723a 0000  r.__init__).r:..
-0000fab0: 0072 3b00 0000 723c 0000 0072 4000 0000  .r;...r<...r@...
-0000fac0: 72a8 0100 0072 3700 0000 7237 0000 0029  r....r7...r7...)
-0000fad0: 0172 a701 0000 7238 0000 0072 9400 0000  .r....r8...r....
-0000fae0: 0c09 0000 7302 0000 0008 0172 9400 0000  ....s......r....
-0000faf0: 6300 0000 0000 0000 0000 0000 0004 0000  c...............
-0000fb00: 0000 0000 0073 2200 0000 6500 5a01 6400  .....s"...e.Z.d.
-0000fb10: 5a02 6401 6700 6602 8700 6601 6402 6403  Z.d.g.f...f.d.d.
-0000fb20: 8409 5a03 8700 0400 5a04 5300 2904 7293  ..Z.....Z.S.).r.
-0000fb30: 0000 0072 0100 0000 6304 0000 0000 0000  ...r....c.......
-0000fb40: 0004 0000 0006 0000 0003 0000 0073 1800  .............s..
-0000fb50: 0000 7400 8300 6a01 7c01 6401 6402 7c02  ..t...j.|.d.d.|.
-0000fb60: 7c03 8305 0100 6400 5300 2903 4e72 4200  |.....d.S.).NrB.
-0000fb70: 0000 7289 0000 0029 0272 a601 0000 7240  ..r....).r....r@
-0000fb80: 0000 0029 0472 3600 0000 7221 0100 0072  ...).r6...r!...r
-0000fb90: 8700 0000 7222 0000 0029 0172 a701 0000  ....r"...).r....
-0000fba0: 7237 0000 0072 3800 0000 7240 0000 0011  r7...r8...r@....
-0000fbb0: 0900 0073 0200 0000 0001 7a21 496e 636f  ...s......z!Inco
-0000fbc0: 7272 6563 7455 6e6c 6f63 6b43 6f64 6545  rrectUnlockCodeE
-0000fbd0: 7272 6f72 2e5f 5f69 6e69 745f 5f29 0572  rror.__init__).r
-0000fbe0: 3a00 0000 723b 0000 0072 3c00 0000 7240  :...r;...r<...r@
-0000fbf0: 0000 0072 a801 0000 7237 0000 0072 3700  ...r....r7...r7.
-0000fc00: 0000 2901 72a7 0100 0072 3800 0000 7293  ..).r....r8...r.
-0000fc10: 0000 0010 0900 0073 0200 0000 0801 7293  .......s......r.
-0000fc20: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-0000fc30: 0400 0000 0000 0000 7322 0000 0065 005a  ........s"...e.Z
-0000fc40: 0164 005a 0264 0167 0066 0287 0066 0164  .d.Z.d.g.f...f.d
-0000fc50: 0264 0384 095a 0387 0004 005a 0453 0029  .d...Z.....Z.S.)
-0000fc60: 04da 1b49 6e63 6f72 7265 6374 556e 6c6f  ...IncorrectUnlo
-0000fc70: 636b 436f 756e 7465 7245 7272 6f72 7201  ckCounterErrorr.
-0000fc80: 0000 0063 0400 0000 0000 0000 0400 0000  ...c............
-0000fc90: 0600 0000 0300 0000 7318 0000 0074 0083  ........s....t..
-0000fca0: 006a 017c 0164 0164 027c 027c 0383 0501  .j.|.d.d.|.|....
-0000fcb0: 0064 0053 0029 034e 7242 0000 0072 7e01  .d.S.).NrB...r~.
-0000fcc0: 0000 2902 72a6 0100 0072 4000 0000 2904  ..).r....r@...).
-0000fcd0: 7236 0000 0072 2101 0000 7287 0000 0072  r6...r!...r....r
-0000fce0: 2200 0000 2901 72a7 0100 0072 3700 0000  "...).r....r7...
-0000fcf0: 7238 0000 0072 4000 0000 1509 0000 7302  r8...r@.......s.
-0000fd00: 0000 0000 017a 2449 6e63 6f72 7265 6374  .....z$Incorrect
-0000fd10: 556e 6c6f 636b 436f 756e 7465 7245 7272  UnlockCounterErr
-0000fd20: 6f72 2e5f 5f69 6e69 745f 5f29 0572 3a00  or.__init__).r:.
-0000fd30: 0000 723b 0000 0072 3c00 0000 7240 0000  ..r;...r<...r@..
-0000fd40: 0072 a801 0000 7237 0000 0072 3700 0000  .r....r7...r7...
-0000fd50: 2901 72a7 0100 0072 3800 0000 72a9 0100  ).r....r8...r...
-0000fd60: 0014 0900 0073 0200 0000 0801 72a9 0100  .....s......r...
-0000fd70: 0063 0000 0000 0000 0000 0000 0000 0100  .c..............
-0000fd80: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
-0000fd90: 005a 0264 015a 0364 0253 0029 03da 1341  .Z.d.Z.d.S.)...A
-0000fda0: 7574 6865 6e74 6963 6174 696f 6e45 7272  uthenticationErr
-0000fdb0: 6f72 7a35 5261 6973 6564 2077 6865 6e20  orz5Raised when 
-0000fdc0: 7468 6520 636f 6d6d 616e 6420 7265 7175  the command requ
-0000fdd0: 6972 6573 2061 7574 6865 6e74 6963 6174  ires authenticat
-0000fde0: 696f 6e20 6669 7273 744e 2904 723a 0000  ion firstN).r:..
-0000fdf0: 0072 3b00 0000 723c 0000 0072 6200 0000  .r;...r<...rb...
-0000fe00: 7237 0000 0072 3700 0000 7237 0000 0072  r7...r7...r7...r
-0000fe10: 3800 0000 72aa 0100 0019 0900 0073 0400  8...r........s..
-0000fe20: 0000 0801 0401 72aa 0100 0063 0000 0000  ......r....c....
-0000fe30: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-0000fe40: 7310 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-0000fe50: 0364 0253 0029 0372 0201 0000 7a28 5261  .d.S.).r....z(Ra
-0000fe60: 6973 6564 2077 6865 6e20 7468 6520 6465  ised when the de
-0000fe70: 7669 6365 2069 7320 6e6f 7420 7965 7420  vice is not yet 
-0000fe80: 7365 6564 6564 4e29 0472 3a00 0000 723b  seededN).r:...r;
-0000fe90: 0000 0072 3c00 0000 7262 0000 0072 3700  ...r<...rb...r7.
-0000fea0: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
-0000feb0: 0072 0201 0000 1d09 0000 7304 0000 0008  .r........s.....
-0000fec0: 0104 0172 0201 0000 6300 0000 0000 0000  ...r....c.......
-0000fed0: 0000 0000 0001 0000 0040 0000 0073 1000  .........@...s..
-0000fee0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-0000fef0: 5300 2903 72f2 0000 007a 3752 6169 7365  S.).r....z7Raise
-0000ff00: 6420 7768 656e 2074 6865 2064 6576 6963  d when the devic
-0000ff10: 6520 7265 7475 726e 7320 616e 2075 6e65  e returns an une
-0000ff20: 7870 6563 7465 6420 6572 726f 7220 636f  xpected error co
-0000ff30: 6465 4e29 0472 3a00 0000 723b 0000 0072  deN).r:...r;...r
-0000ff40: 3c00 0000 7262 0000 0072 3700 0000 7237  <...rb...r7...r7
-0000ff50: 0000 0072 3700 0000 7238 0000 0072 f200  ...r7...r8...r..
-0000ff60: 0000 2109 0000 7304 0000 0008 0104 0172  ..!...s........r
-0000ff70: f200 0000 6300 0000 0000 0000 0000 0000  ....c...........
-0000ff80: 0001 0000 0040 0000 0073 1000 0000 6500  .....@...s....e.
-0000ff90: 5a01 6400 5a02 6401 5a03 6402 5300 2903  Z.d.Z.d.Z.d.S.).
-0000ffa0: 72e3 0000 007a 2c52 6169 7365 6420 7768  r....z,Raised wh
-0000ffb0: 656e 2074 6865 2064 6576 6963 6520 7265  en the device re
-0000ffc0: 7475 726e 7320 616e 2065 7272 6f72 2063  turns an error c
-0000ffd0: 6f64 654e 2904 723a 0000 0072 3b00 0000  odeN).r:...r;...
-0000ffe0: 723c 0000 0072 6200 0000 7237 0000 0072  r<...rb...r7...r
-0000fff0: 3700 0000 7237 0000 0072 3800 0000 72e3  7...r7...r8...r.
-00010000: 0000 0024 0900 0073 0400 0000 0801 0401  ...$...s........
-00010010: 72e3 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00010020: 0000 0100 0000 4000 0000 7310 0000 0065  ......@...s....e
-00010030: 005a 0164 005a 0264 015a 0364 0253 0029  .Z.d.Z.d.Z.d.S.)
-00010040: 0372 9700 0000 7a2c 5261 6973 6564 2077  .r....z,Raised w
-00010050: 6865 6e20 7468 6520 6465 7669 6365 2072  hen the device r
-00010060: 6574 7572 6e73 2061 6e20 6572 726f 7220  eturns an error 
-00010070: 636f 6465 4e29 0472 3a00 0000 723b 0000  codeN).r:...r;..
-00010080: 0072 3c00 0000 7262 0000 0072 3700 0000  .r<...rb...r7...
-00010090: 7237 0000 0072 3700 0000 7238 0000 0072  r7...r7...r8...r
-000100a0: 9700 0000 2809 0000 7304 0000 0008 0104  ....(...s.......
-000100b0: 0172 9700 0000 6300 0000 0000 0000 0000  .r....c.........
-000100c0: 0000 0001 0000 0040 0000 0073 1000 0000  .......@...s....
-000100d0: 6500 5a01 6400 5a02 6401 5a03 6402 5300  e.Z.d.Z.d.Z.d.S.
-000100e0: 2903 7259 0100 007a 3252 6169 7365 6420  ).rY...z2Raised 
-000100f0: 7768 656e 2061 6e20 6572 726f 7220 6973  when an error is
-00010100: 2072 6574 7572 6e65 6420 6279 2074 6865   returned by the
-00010110: 2053 6565 644b 6565 7065 724e 2904 723a   SeedKeeperN).r:
-00010120: 0000 0072 3b00 0000 723c 0000 0072 6200  ...r;...r<...rb.
-00010130: 0000 7237 0000 0072 3700 0000 7237 0000  ..r7...r7...r7..
-00010140: 0072 3800 0000 7259 0100 002c 0900 0073  .r8...rY...,...s
-00010150: 0400 0000 0801 0401 7259 0100 00da 085f  ........rY....._
-00010160: 5f6d 6169 6e5f 5f29 0572 1900 0000 721a  _main__).r....r.
-00010170: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
-00010180: 0000 2947 5a12 736d 6172 7463 6172 642e  ..)GZ.smartcard.
-00010190: 4361 7264 5479 7065 7202 0000 005a 1573  CardTyper....Z.s
-000101a0: 6d61 7274 6361 7264 2e43 6172 6452 6571  martcard.CardReq
-000101b0: 7565 7374 7203 0000 005a 2073 6d61 7274  uestr....Z smart
-000101c0: 6361 7264 2e43 6172 6443 6f6e 6e65 6374  card.CardConnect
-000101d0: 696f 6e4f 6273 6572 7665 7272 0400 0000  ionObserverr....
-000101e0: 5a18 736d 6172 7463 6172 642e 4361 7264  Z.smartcard.Card
-000101f0: 4d6f 6e69 746f 7269 6e67 7205 0000 0072  Monitoringr....r
-00010200: 0600 0000 5a14 736d 6172 7463 6172 642e  ....Z.smartcard.
-00010210: 4578 6365 7074 696f 6e73 7207 0000 0072  Exceptionsr....r
-00010220: 0800 0000 5a0e 736d 6172 7463 6172 642e  ....Z.smartcard.
-00010230: 7574 696c 7209 0000 0072 0a00 0000 5a19  utilr....r....Z.
-00010240: 736d 6172 7463 6172 642e 7377 2e53 5745  smartcard.sw.SWE
-00010250: 7863 6570 7469 6f6e 7372 0b00 0000 722b  xceptionsr....r+
-00010260: 0000 0072 0e00 0000 720f 0000 005a 0365  ...r....r....Z.e
-00010270: 6363 7210 0000 0072 1100 0000 7212 0000  ccr....r....r...
-00010280: 00da 0475 7469 6c72 1300 0000 7214 0000  ...utilr....r...
-00010290: 0072 1500 0000 7216 0000 005a 1563 6572  .r....r....Z.cer
-000102a0: 7469 6669 6361 7465 5f76 616c 6964 6174  tificate_validat
-000102b0: 6f72 7217 0000 0072 4f00 0000 72eb 0000  orr....rO...r...
-000102c0: 0072 3b01 0000 72a3 0100 00da 026f 7372  .r;...r......osr
-000102d0: 1800 0000 da09 6765 744c 6f67 6765 7272  ......getLoggerr
-000102e0: 3a00 0000 7227 0000 0072 7400 0000 da05  :...r'...rt.....
-000102f0: 4445 4255 4772 0301 0000 5a0b 4d53 475f  DEBUGr....Z.MSG_
-00010300: 5553 455f 3246 4172 1601 0000 7218 0100  USE_2FAr....r...
-00010310: 0072 1901 0000 721e 0000 0072 3d00 0000  .r....r....r=...
-00010320: 7263 0000 0072 5300 0000 72a5 0100 0072  rc...rS...r....r
-00010330: 9100 0000 7281 0100 0072 9200 0000 7296  ....r....r....r.
-00010340: 0000 0072 9500 0000 7294 0000 0072 9300  ...r....r....r..
-00010350: 0000 72a9 0100 0072 aa01 0000 7202 0100  ..r....r....r...
-00010360: 0072 f200 0000 72e3 0000 0072 9700 0000  .r....r....r....
-00010370: 7259 0100 005a 0d63 6172 6463 6f6e 6e65  rY...Z.cardconne
-00010380: 6374 6f72 729a 0000 0072 5500 0000 7208  ctorr....rU...r.
-00010390: 0100 0072 5600 0000 7237 0000 0072 3700  ...rV...r7...r7.
-000103a0: 0000 7237 0000 0072 3800 0000 da08 3c6d  ..r7...r8.....<m
-000103b0: 6f64 756c 653e 0100 0000 7392 0000 000c  odule>....s.....
-000103c0: 010c 010c 0110 0110 0110 010c 0208 010c  ................
-000103d0: 010c 0110 010c 0118 010c 0208 0108 0108  ................
-000103e0: 0108 010c 060a 010c 0204 0504 0804 0202  ................
-000103f0: 0102 0102 0102 0108 0302 0102 0102 0102  ................
-00010400: 0108 0410 1510 3e0e 7f00 7f00 7f00 7f00  ......>.........
-00010410: 7f00 7f00 7f00 7f00 7f00 7f00 7f00 7f00  ................
-00010420: 7f00 7f00 7f00 7f00 6e10 0910 0510 0410  ........n.......
-00010430: 0510 0410 0410 0410 0410 0510 0410 0410  ................
-00010440: 0310 0410 0410 050a 0206 0108 0108 0208  ................
-00010450: 02                                       .
+000043d0: 3333 297a 2953 6563 7572 6520 696d 706f  33)z)Secure impo
+000043e0: 7274 2066 6169 6c65 643a 2077 726f 6e67  rt failed: wrong
+000043f0: 204d 4143 2028 3078 3943 3333 2921 e934   MAC (0x9C33)!.4
+00004400: 0000 007a 3645 7272 6f72 2064 7572 696e  ...z6Error durin
+00004410: 6720 7365 6372 6574 2069 6d70 6f72 743a  g secret import:
+00004420: 2077 726f 6e67 2066 696e 6765 7270 7269   wrong fingerpri
+00004430: 6e74 2028 3078 3943 3334 297a 3153 6563  nt (0x9C34)z1Sec
+00004440: 7572 6520 696d 706f 7274 2066 6169 6c65  ure import faile
+00004450: 643a 2077 726f 6e67 2066 696e 6765 7270  d: wrong fingerp
+00004460: 7269 6e74 2028 3078 3943 3334 2921 e935  rint (0x9C34)!.5
+00004470: 0000 007a 3545 7272 6f72 2064 7572 696e  ...z5Error durin
+00004480: 6720 7365 6372 6574 2069 6d70 6f72 743a  g secret import:
+00004490: 206e 6f20 5472 7573 7465 6450 7562 6b65   no TrustedPubke
+000044a0: 7920 2830 7839 4333 3529 7a2d 5365 6375  y (0x9C35)z-Secu
+000044b0: 7265 2069 6d70 6f72 7420 6661 696c 6564  re import failed
+000044c0: 3a20 5472 7573 7465 6450 7562 6b65 7920  : TrustedPubkey 
+000044d0: 2830 7839 4333 3529 217a 2745 7272 6f72  (0x9C35)!z'Error
+000044e0: 2064 7572 696e 6720 7365 6372 6574 2069   during secret i
+000044f0: 6d70 6f72 7420 2865 7272 6f72 2063 6f64  mport (error cod
+00004500: 6520 72bd 0000 007a 3955 6e65 7870 6563  e r....z9Unexpec
+00004510: 7465 6420 6572 726f 7220 6475 7269 6e67  ted error during
+00004520: 2073 6563 7572 6520 7365 6372 6574 2069   secure secret i
+00004530: 6d70 6f72 7420 2865 7272 6f72 2063 6f64  mport (error cod
+00004540: 6520 728a 0000 0054 7a12 6175 7468 656e  e r....Tz.authen
+00004550: 7469 6b65 795f 6361 7264 3d20 e9b0 0000  tikey_card= ....
+00004560: 004e e90e 0000 0029 1072 2700 0000 7234  .N.....).r'...r4
+00004570: 0000 0072 2b00 0000 72be 0000 0072 c800  ...r+...r....r..
+00004580: 0000 724b 0000 0072 e100 0000 7235 0000  ..rK...r....r5..
+00004590: 0072 9b00 0000 72e4 0000 0072 e500 0000  .r....r....r....
+000045a0: 724c 0000 00da 1355 6e65 7870 6563 7465  rL.....Unexpecte
+000045b0: 6453 5731 3245 7272 6f72 7277 0000 00da  dSW12Errorrw....
+000045c0: 1b70 6172 7365 5f62 6970 3332 5f67 6574  .parse_bip32_get
+000045d0: 5f61 7574 6865 6e74 696b 6579 72e3 0000  _authentikeyr...
+000045e0: 0029 1372 3600 0000 da0a 7365 6372 6574  .).r6.....secret
+000045f0: 5f64 6963 72a1 0000 0072 8900 0000 72a2  _dicr....r....r.
+00004600: 0000 0072 a300 0000 72ea 0000 0072 eb00  ...r....r....r..
+00004610: 0000 da0b 7365 6372 6574 5f6c 6973 7472  ....secret_listr
+00004620: ed00 0000 72cb 0000 0072 cc00 0000 729a  ....r....r....r.
+00004630: 0000 0072 2200 0000 725e 0000 0072 5f00  ...r"...r^...r_.
+00004640: 0000 da0b 7365 6372 6574 5f74 7970 6572  ....secret_typer
+00004650: a600 0000 72e7 0000 0072 3700 0000 7237  ....r....r7...r7
+00004660: 0000 0072 3800 0000 da1c 6361 7264 5f69  ...r8.....card_i
+00004670: 6d70 6f72 745f 656e 6372 7970 7465 645f  mport_encrypted_
+00004680: 7365 6372 6574 2502 0000 735c 0000 0000  secret%...s\....
+00004690: 0e0a 0206 0104 0104 0104 011a 0112 0112  ................
+000046a0: 0112 0132 0108 0112 0110 0110 0104 0112  ...2............
+000046b0: 010a 010c 0114 010a 010c 0114 010a 010a  ................
+000046c0: 0114 010a 010a 0114 010a 010a 0114 010a  ................
+000046d0: 010a 0114 010a 010a 021e 011c 0208 010a  ................
+000046e0: 010c 010e 010e 0104 010a 017a 2a43 6172  ...........z*Car
+000046f0: 6443 6f6e 6e65 6374 6f72 2e63 6172 645f  dConnector.card_
+00004700: 696d 706f 7274 5f65 6e63 7279 7074 6564  import_encrypted
+00004710: 5f73 6563 7265 7463 0200 0000 0000 0000  _secretc........
+00004720: 0e00 0000 0500 0000 4300 0000 7324 0100  ........C...s$..
+00004730: 0074 006a 0164 0183 0101 0074 027c 0183  .t.j.d.....t.|..
+00004740: 0174 036b 0872 2674 0474 056a 067c 0183  .t.k.r&t.t.j.|..
+00004750: 0183 017d 016e 1474 027c 0183 0174 056b  ...}.n.t.|...t.k
+00004760: 0872 3a74 047c 0183 017d 0174 076a 087d  .r:t.|...}.t.j.}
+00004770: 0264 027d 0364 037d 0464 037d 0574 097c  .d.}.d.}.d.}.t.|
+00004780: 0183 017d 067c 0664 046b 0372 6a74 0a64  ...}.|.d.k.rjt.d
+00004790: 057c 069b 009d 0283 0182 017c 0664 063f  .|.........|.d.?
+000047a0: 007c 0664 0716 0067 027c 0117 007d 0774  .|.d...g.|...}.t
+000047b0: 097c 0783 017d 087c 027c 037c 047c 057c  .|...}.|.|.|.|.|
+000047c0: 0867 057c 0717 007d 097c 006a 0b7c 0983  .g.|...}.|.j.|..
+000047d0: 015c 037d 0a7d 0b7d 0c7c 0b64 086b 0272  .\.}.}.}.|.d.k.r
+000047e0: cc7c 0c64 036b 0272 cc74 006a 0c64 0983  .|.d.k.r.t.j.d..
+000047f0: 0101 0074 0d64 0983 0182 016e 487c 0b64  ...t.d.....nH|.d
+00004800: 0a6b 0272 f07c 0c64 0b6b 0272 f074 006a  .k.r.|.d.k.r.t.j
+00004810: 0c64 0c83 0101 0074 0d64 0d83 0182 016e  .d.....t.d.....n
+00004820: 247c 0b64 0a6b 026f fe7c 0c64 0e6b 0290  $|.d.k.o.|.d.k..
+00004830: 0172 1474 006a 0c64 0f83 0101 0074 0d64  .r.t.j.d.....t.d
+00004840: 0f83 0182 017c 006a 0e6a 0f7c 0a83 017d  .....|.j.j.|...}
+00004850: 0d7c 0d53 0029 1061 4901 0000 2049 6d70  .|.S.).aI... Imp
+00004860: 6f72 7420 6120 7472 7573 7465 6420 6563  ort a trusted ec
+00004870: 2070 7562 6b65 7920 696e 746f 2074 6865   pubkey into the
+00004880: 2064 6576 6963 652e 2054 6869 7320 7075   device. This pu
+00004890: 626b 6579 2077 696c 6c20 6265 2075 7365  bkey will be use
+000048a0: 6420 666f 7220 7468 6520 7365 6375 7265  d for the secure
+000048b0: 2069 6d70 6f72 7420 6f66 2061 2073 6563   import of a sec
+000048c0: 7265 740a 2020 2020 2020 2020 0a20 2020  ret.        .   
+000048d0: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
+000048e0: 200a 2020 2020 2020 2020 7075 626b 6579   .        pubkey
+000048f0: 5f6c 6973 743a 2074 6865 2070 7562 6b65  _list: the pubke
+00004900: 7920 696e 2075 6e63 6f6d 7072 6573 7365  y in uncompresse
+00004910: 6420 666f 726d 2028 3635 2062 7974 6573  d form (65 bytes
+00004920: 2920 6173 2061 2068 6578 5f73 7472 696e  ) as a hex_strin
+00004930: 6720 6f72 2062 7974 6573 206f 7220 6c69  g or bytes or li
+00004940: 7374 206f 6620 696e 740a 0a20 2020 2020  st of int..     
+00004950: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+00004960: 2020 2020 2070 7562 6b65 795f 6865 783a       pubkey_hex:
+00004970: 2074 6865 2070 7562 6b65 7920 6173 2061   the pubkey as a
+00004980: 2068 6578 2073 7472 696e 6720 2836 352a   hex string (65*
+00004990: 3220 6865 7820 6368 6172 7329 0a20 2020  2 hex chars).   
+000049a0: 2020 2020 207a 1d49 6e20 6361 7264 5f69       z.In card_i
+000049b0: 6d70 6f72 745f 7472 7573 7465 645f 7075  mport_trusted_pu
+000049c0: 626b 6579 e9aa 0000 0072 0100 0000 e941  bkey.....r.....A
+000049d0: 0000 007a 5045 7272 6f72 2064 7572 696e  ...zPError durin
+000049e0: 6720 7472 7573 7465 6420 7075 626b 6579  g trusted pubkey
+000049f0: 2069 6d70 6f72 743a 2077 726f 6e67 2070   import: wrong p
+00004a00: 7562 6b65 7920 7369 7a65 2c20 6578 7065  ubkey size, expe
+00004a10: 6374 6564 2036 3520 6275 7420 7265 6365  cted 65 but rece
+00004a20: 6976 6564 2072 b400 0000 72bc 0000 0072  ived r....r....r
+00004a30: 7300 0000 7a48 4572 726f 7220 6475 7269  s...zHError duri
+00004a40: 6e67 2073 6563 7265 7420 696d 706f 7274  ng secret import
+00004a50: 3a20 6f70 6572 6174 696f 6e20 6e6f 7420  : operation not 
+00004a60: 7375 7070 6f72 7465 6420 6279 2074 6865  supported by the
+00004a70: 2063 6172 6420 2830 7836 4430 3029 7242   card (0x6D00)rB
+00004a80: 0000 0072 df00 0000 7a3b 4572 726f 7220  ...r....z;Error 
+00004a90: 6475 7269 6e67 2073 6563 7265 7420 696d  during secret im
+00004aa0: 706f 7274 3a20 6361 7264 2069 7320 616c  port: card is al
+00004ab0: 7265 6164 7920 7365 6564 6564 2028 3078  ready seeded (0x
+00004ac0: 3943 3137 297a 3653 6563 7572 6520 696d  9C17)z6Secure im
+00004ad0: 706f 7274 2066 6169 6c65 643a 2063 6172  port failed: car
+00004ae0: 6420 6973 2061 6c72 6561 6479 2073 6565  d is already see
+00004af0: 6465 6420 2830 7839 4331 3729 2172 e000  ded (0x9C17)!r..
+00004b00: 0000 7a36 4572 726f 7220 6475 7269 6e67  ..z6Error during
+00004b10: 2073 6563 7265 7420 696d 706f 7274 3a20   secret import: 
+00004b20: 696e 7661 6c69 6420 7061 7261 6d65 7465  invalid paramete
+00004b30: 7220 2830 7839 4330 4629 2910 7227 0000  r (0x9C0F)).r'..
+00004b40: 0072 3400 0000 7226 0000 0072 7600 0000  .r4...r&...rv...
+00004b50: 72c8 0000 0072 4b00 0000 72e1 0000 0072  r....rK...r....r
+00004b60: 2b00 0000 72be 0000 0072 3500 0000 da0c  +...r....r5.....
+00004b70: 5275 6e74 696d 6545 7272 6f72 729b 0000  RuntimeErrorr...
+00004b80: 0072 e400 0000 72e5 0000 0072 7700 0000  .r....r....rw...
+00004b90: da12 6765 745f 7472 7573 7465 645f 7075  ..get_trusted_pu
+00004ba0: 626b 6579 290e 7236 0000 00da 0b70 7562  bkey).r6.....pub
+00004bb0: 6b65 795f 6c69 7374 72a1 0000 0072 8900  key_listr....r..
+00004bc0: 0000 72a2 0000 0072 a300 0000 5a0b 7075  ..r....r....Z.pu
+00004bd0: 626b 6579 5f73 697a 6572 cb00 0000 72cc  bkey_sizer....r.
+00004be0: 0000 0072 9a00 0000 7222 0000 0072 5e00  ...r....r"...r^.
+00004bf0: 0000 725f 0000 00da 0a70 7562 6b65 795f  ..r_.....pubkey_
+00004c00: 6865 7872 3700 0000 7237 0000 0072 3800  hexr7...r7...r8.
+00004c10: 0000 da1a 6361 7264 5f69 6d70 6f72 745f  ....card_import_
+00004c20: 7472 7573 7465 645f 7075 626b 6579 6502  trusted_pubkeye.
+00004c30: 0000 7336 0000 0000 090a 010c 0110 010c  ..s6............
+00004c40: 0108 0206 0104 0104 0104 0108 0108 010e  ................
+00004c50: 0114 0108 0112 0110 0110 010a 010a 0110  ................
+00004c60: 010a 010a 0112 010a 0108 020c 017a 2843  .............z(C
+00004c70: 6172 6443 6f6e 6e65 6374 6f72 2e63 6172  ardConnector.car
+00004c80: 645f 696d 706f 7274 5f74 7275 7374 6564  d_import_trusted
+00004c90: 5f70 7562 6b65 7963 0100 0000 0000 0000  _pubkeyc........
+00004ca0: 0a00 0000 0400 0000 4300 0000 7378 0000  ........C...sx..
+00004cb0: 0074 006a 0164 0183 0101 0074 026a 037d  .t.j.d.....t.j.}
+00004cc0: 0164 027d 0264 037d 0364 037d 047c 017c  .d.}.d.}.d.}.|.|
+00004cd0: 027c 037c 0467 047d 057c 006a 047c 0583  .|.|.g.}.|.j.|..
+00004ce0: 015c 037d 067d 077d 087c 0764 046b 0272  .\.}.}.}.|.d.k.r
+00004cf0: 507c 0864 056b 0272 5064 0664 0714 0053  P|.d.k.rPd.d...S
+00004d00: 007c 0764 086b 0272 687c 0864 036b 0272  .|.d.k.rh|.d.k.r
+00004d10: 6864 0664 0914 0053 007c 006a 056a 067c  hd.d...S.|.j.j.|
+00004d20: 0683 017d 097c 0953 0029 0a7a c820 4578  ...}.|.S.).z. Ex
+00004d30: 706f 7274 2074 6865 2074 7275 7374 6564  port the trusted
+00004d40: 2065 6320 7075 626b 6579 2066 726f 6d20   ec pubkey from 
+00004d50: 7468 6520 6465 7669 6365 2e20 5468 6973  the device. This
+00004d60: 2070 7562 6b65 7920 6973 2075 7365 6420   pubkey is used 
+00004d70: 666f 7220 7468 6520 7365 6375 7265 2069  for the secure i
+00004d80: 6d70 6f72 7420 6f66 2061 2073 6563 7265  mport of a secre
+00004d90: 740a 2020 2020 2020 2020 0a20 2020 2020  t.        .     
+00004da0: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+00004db0: 2020 2020 2070 7562 6b65 795f 6865 783a       pubkey_hex:
+00004dc0: 2074 6865 2070 7562 6b65 7920 6173 2061   the pubkey as a
+00004dd0: 2068 6578 2073 7472 696e 6720 2836 352a   hex string (65*
+00004de0: 3220 6865 7820 6368 6172 7329 0a20 2020  2 hex chars).   
+00004df0: 2020 2020 207a 1d49 6e20 6361 7264 5f65       z.In card_e
+00004e00: 7870 6f72 745f 7472 7573 7465 645f 7075  xport_trusted_pu
+00004e10: 626b 6579 e9ab 0000 0072 0100 0000 7242  bkey.....r....rB
+00004e20: 0000 0072 f100 0000 72fb 0000 005a 0230  ...r....r....Z.0
+00004e30: 3072 7300 0000 5a02 4646 2907 7227 0000  0rs...Z.FF).r'..
+00004e40: 0072 3400 0000 722b 0000 0072 be00 0000  .r4...r+...r....
+00004e50: 729b 0000 0072 7700 0000 72fd 0000 0029  r....rw...r....)
+00004e60: 0a72 3600 0000 72a1 0000 0072 8900 0000  .r6...r....r....
+00004e70: 72a2 0000 0072 a300 0000 729a 0000 0072  r....r....r....r
+00004e80: 2200 0000 725e 0000 0072 5f00 0000 72ff  "...r^...r_...r.
+00004e90: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
+00004ea0: 0000 da1a 6361 7264 5f65 7870 6f72 745f  ....card_export_
+00004eb0: 7472 7573 7465 645f 7075 626b 6579 8c02  trusted_pubkey..
+00004ec0: 0000 731a 0000 0000 060a 0106 0104 0104  ..s.............
+00004ed0: 0104 010c 0110 0110 0108 0110 0108 020c  ................
+00004ee0: 017a 2843 6172 6443 6f6e 6e65 6374 6f72  .z(CardConnector
+00004ef0: 2e63 6172 645f 6578 706f 7274 5f74 7275  .card_export_tru
+00004f00: 7374 6564 5f70 7562 6b65 7963 0100 0000  sted_pubkeyc....
+00004f10: 0000 0000 0a00 0000 0500 0000 4300 0000  ............C...
+00004f20: 73be 0000 0074 006a 0164 0183 0101 0074  s....t.j.d.....t
+00004f30: 026a 037d 0164 027d 0264 037d 0364 037d  .j.}.d.}.d.}.d.}
+00004f40: 047c 017c 027c 037c 0467 047d 057c 006a  .|.|.|.|.g.}.|.j
+00004f50: 047c 0583 015c 037d 067d 077d 087c 0764  .|...\.}.}.}.|.d
+00004f60: 046b 0272 587c 0864 036b 0272 587c 006a  .k.rX|.d.k.rX|.j
+00004f70: 056a 067c 0683 017d 097c 0953 007c 0764  .j.|...}.|.S.|.d
+00004f80: 056b 0272 807c 0864 066b 0272 8074 006a  .k.r.|.d.k.r.t.j
+00004f90: 0764 0783 0101 0074 0864 0874 0917 0083  .d.....t.d.t....
+00004fa0: 0182 016e 3a74 006a 0a64 0974 0b64 0a7c  ...n:t.j.d.t.d.|
+00004fb0: 0714 007c 0817 0083 019b 0064 0b9d 0383  ...|.......d....
+00004fc0: 0101 0074 0c64 0974 0b64 0a7c 0714 007c  ...t.d.t.d.|...|
+00004fd0: 0817 0083 019b 0064 0b9d 0383 0182 0164  .......d.......d
+00004fe0: 0c53 0029 0d61 3a01 0000 2045 7870 6f72  .S.).a:... Expor
+00004ff0: 7420 7468 6520 6465 7669 6365 2061 7574  t the device aut
+00005000: 6865 6e74 696b 6579 2e0a 2020 2020 2020  hentikey..      
+00005010: 2020 0a20 2020 2020 2020 2054 6865 2061    .        The a
+00005020: 7574 6865 6e74 696b 6579 2069 6465 6e74  uthentikey ident
+00005030: 6966 6965 7320 756e 6971 7565 6c79 2074  ifies uniquely t
+00005040: 6865 2064 6576 6963 6520 616e 6420 6973  he device and is
+00005050: 2061 6c73 6f20 7573 6564 2066 6f72 2073   also used for s
+00005060: 6574 7469 6e67 2061 0a20 2020 2020 2020  etting a.       
+00005070: 2073 6563 7572 6520 6368 616e 6e65 6c20   secure channel 
+00005080: 7768 656e 2064 6f69 6e67 2061 2073 6563  when doing a sec
+00005090: 7572 6520 696d 706f 7274 2077 6974 6820  ure import with 
+000050a0: 6361 7264 5f69 6d70 6f72 745f 656e 6372  card_import_encr
+000050b0: 7970 7465 645f 7365 6372 6574 2829 2e0a  ypted_secret()..
+000050c0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000050d0: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
+000050e0: 2020 2061 7574 6865 6e74 696b 6579 3a20     authentikey: 
+000050f0: 4543 5075 626b 6579 206f 626a 6563 7420  ECPubkey object 
+00005100: 7468 6174 2069 6465 6e74 6966 6965 7320  that identifies 
+00005110: 7468 6520 2064 6576 6963 650a 2020 2020  the  device.    
+00005120: 2020 2020 7a1a 496e 2063 6172 645f 6578      z.In card_ex
+00005130: 706f 7274 5f61 7574 6865 6e74 696b 6579  port_authentikey
+00005140: e9ad 0000 0072 0100 0000 7241 0000 0072  .....r....rA...r
+00005150: 4200 0000 7243 0000 007a 4b63 6172 645f  B...rC...zKcard_
+00005160: 6269 7033 325f 6765 745f 6175 7468 656e  bip32_get_authen
+00005170: 7469 6b65 7928 293a 2053 6174 6f63 6869  tikey(): Satochi
+00005180: 7020 6973 206e 6f74 2069 6e69 7469 616c  p is not initial
+00005190: 697a 6564 203d 3e20 5261 6973 696e 6720  ized => Raising 
+000051a0: 6572 726f 7221 7a3e 5361 746f 6368 6970  error!z>Satochip
+000051b0: 2069 7320 6e6f 7420 696e 6974 6961 6c69   is not initiali
+000051c0: 7a65 6421 2059 6f75 2073 686f 756c 6420  zed! You should 
+000051d0: 6372 6561 7465 2061 206e 6577 2077 616c  create a new wal
+000051e0: 6c65 7421 0a0a 7a37 556e 6578 7065 6374  let!..z7Unexpect
+000051f0: 6564 2065 7272 6f72 2064 7572 696e 6720  ed error during 
+00005200: 6175 7468 656e 7469 6b65 7920 6578 706f  authentikey expo
+00005210: 7274 2028 6572 726f 7220 636f 6465 2072  rt (error code r
+00005220: bc00 0000 72bd 0000 004e 290d 7227 0000  ....r....N).r'..
+00005230: 0072 3400 0000 722b 0000 0072 be00 0000  .r4...r+...r....
+00005240: 729b 0000 0072 7700 0000 72f5 0000 0072  r....rw...r....r
+00005250: 2800 0000 da16 556e 696e 6974 6961 6c69  (.....Uninitiali
+00005260: 7a65 6453 6565 6445 7272 6f72 da0b 4d53  zedSeedError..MS
+00005270: 475f 5741 524e 494e 4772 5400 0000 724c  G_WARNINGrT...rL
+00005280: 0000 0072 f400 0000 290a 7236 0000 0072  ...r....).r6...r
+00005290: a100 0000 7289 0000 0072 a200 0000 72a3  ....r....r....r.
+000052a0: 0000 0072 9a00 0000 7222 0000 0072 5e00  ...r....r"...r^.
+000052b0: 0000 725f 0000 0072 a600 0000 7237 0000  ..r_...r....r7..
+000052c0: 0072 3700 0000 7238 0000 00da 1763 6172  .r7...r8.....car
+000052d0: 645f 6578 706f 7274 5f61 7574 6865 6e74  d_export_authent
+000052e0: 696b 6579 a102 0000 731e 0000 0000 090a  ikey....s.......
+000052f0: 0106 0104 0104 0104 010c 0310 0110 020c  ................
+00005300: 0104 0110 010a 010e 021e 017a 2543 6172  ...........z%Car
+00005310: 6443 6f6e 6e65 6374 6f72 2e63 6172 645f  dConnector.card_
+00005320: 6578 706f 7274 5f61 7574 6865 6e74 696b  export_authentik
+00005330: 6579 6303 0000 0000 0000 000d 0000 0005  eyc.............
+00005340: 0000 0043 0000 0073 d600 0000 7400 6a01  ...C...s....t.j.
+00005350: 6401 8301 0100 7402 7c01 8301 7403 6b08  d.....t.|...t.k.
+00005360: 7226 7404 7c01 6a05 6402 8301 8301 7d01  r&t.|.j.d.....}.
+00005370: 6e14 7402 7c01 8301 7406 6b08 723a 7404  n.t.|...t.k.r:t.
+00005380: 7c03 8301 7d03 7402 7c02 8301 7403 6b08  |...}.t.|...t.k.
+00005390: 7256 7404 7406 6a07 7c02 8301 8301 7d02  rVt.t.j.|.....}.
+000053a0: 6e14 7402 7c02 8301 7406 6b08 726a 7404  n.t.|...t.k.rjt.
+000053b0: 7c02 8301 7d02 7408 6a09 7d04 6403 7d05  |...}.t.j.}.d.}.
+000053c0: 740a 7c01 8301 7d06 6404 7d07 740a 7c01  t.|...}.d.}.t.|.
+000053d0: 8301 740a 7c02 8301 1700 7d08 7c04 7c05  ..t.|.....}.|.|.
+000053e0: 7c06 7c07 7c08 6705 7c01 1700 7c02 1700  |.|.|.g.|...|...
+000053f0: 7d09 7c00 6a0b 7c09 8301 5c03 7d0a 7d0b  }.|.j.|...\.}.}.
+00005400: 7d0c 7c0b 6405 6b02 72cc 7c0c 6404 6b02  }.|.d.k.r.|.d.k.
+00005410: 72cc 6406 7c00 5f0c 7c0a 7c0b 7c0c 6603  r.d.|._.|.|.|.f.
+00005420: 5300 2907 6126 0100 0020 5265 7365 7420  S.).a&... Reset 
+00005430: 7468 6520 7365 6564 0a20 2020 2020 2020  the seed.       
+00005440: 200a 2020 2020 2020 2020 5061 7261 6d65   .        Parame
+00005450: 7465 7273 3a20 0a20 2020 2020 2020 2070  ters: .        p
+00005460: 696e 2020 2868 6578 2d73 7472 696e 6720  in  (hex-string 
+00005470: 7c20 6279 7465 7320 7c20 6c69 7374 293a  | bytes | list):
+00005480: 2074 6865 2070 696e 2072 6571 7569 7265   the pin require
+00005490: 6420 746f 2075 6e6c 6f63 6b20 7468 6520  d to unlock the 
+000054a0: 6465 7669 6365 0a20 2020 2020 2020 2068  device.        h
+000054b0: 6d61 6320 2868 6578 2d73 7472 696e 6720  mac (hex-string 
+000054c0: 7c20 6279 7465 7320 7c20 6c69 7374 293a  | bytes | list):
+000054d0: 2074 6865 2032 302d 6279 7465 2063 6f64   the 20-byte cod
+000054e0: 6520 7265 7175 6972 6564 2069 6620 3246  e required if 2F
+000054f0: 4120 6973 2065 6e61 626c 6564 0a20 2020  A is enabled.   
+00005500: 2020 2020 200a 2020 2020 2020 2020 5265       .        Re
+00005510: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
+00005520: 2872 6573 706f 6e73 652c 2073 7731 2c20  (response, sw1, 
+00005530: 7377 3229 3a20 286c 6973 742c 2069 6e74  sw2): (list, int
+00005540: 2c20 696e 7429 0a20 2020 2020 2020 207a  , int).        z
+00005550: 1249 6e20 6361 7264 5f72 6573 6574 5f73  .In card_reset_s
+00005560: 6565 647a 0575 7466 2d38 e977 0000 0072  eedz.utf-8.w...r
+00005570: 0100 0000 7241 0000 0046 290d 7227 0000  ....rA...F).r'..
+00005580: 0072 3400 0000 7226 0000 0072 7600 0000  .r4...r&...rv...
+00005590: 72c8 0000 0072 c900 0000 724b 0000 0072  r....r....rK...r
+000055a0: e100 0000 722b 0000 0072 be00 0000 7235  ....r+...r....r5
+000055b0: 0000 0072 9b00 0000 7279 0000 0029 0d72  ...r....ry...).r
+000055c0: 3600 0000 727d 0000 0072 ed00 0000 72e6  6...r}...r....r.
+000055d0: 0000 0072 a100 0000 7289 0000 0072 a200  ...r....r....r..
+000055e0: 0000 72a3 0000 0072 cc00 0000 729a 0000  ..r....r....r...
+000055f0: 0072 2200 0000 725e 0000 0072 5f00 0000  .r"...r^...r_...
+00005600: 7237 0000 0072 3700 0000 7238 0000 00da  r7...r7...r8....
+00005610: 0f63 6172 645f 7265 7365 745f 7365 6564  .card_reset_seed
+00005620: bf02 0000 7326 0000 0000 0a0a 010c 0110  ....s&..........
+00005630: 010c 0108 020c 0110 010c 0108 0206 0104  ................
+00005640: 0108 0104 0110 0116 0210 0110 0106 017a  ...............z
+00005650: 1d43 6172 6443 6f6e 6e65 6374 6f72 2e63  .CardConnector.c
+00005660: 6172 645f 7265 7365 745f 7365 6564 6301  ard_reset_seedc.
+00005670: 0000 0000 0000 000a 0000 0004 0000 0043  ...............C
+00005680: 0000 0073 ae00 0000 7400 6a01 6401 8301  ...s....t.j.d...
+00005690: 0100 7402 6a03 7d01 7402 6a04 7d02 6402  ..t.j.}.t.j.}.d.
+000056a0: 7d03 6402 7d04 7c01 7c02 7c03 7c04 6704  }.d.}.|.|.|.|.g.
+000056b0: 7d05 7c00 6a05 7c05 8301 5c03 7d06 7d07  }.|.j.|...\.}.}.
+000056c0: 7d08 7c07 6403 6b02 7260 7c08 6404 6b02  }.|.d.k.r`|.d.k.
+000056d0: 7260 7400 6a06 6405 8301 0100 7407 6406  r`t.j.d.....t.d.
+000056e0: 7408 1700 8301 8201 7c07 6403 6b02 7286  t.......|.d.k.r.
+000056f0: 7c08 6407 6b02 7286 7400 6a06 6408 8301  |.d.k.r.t.j.d...
+00005700: 0100 7407 6409 7408 1700 8301 8201 640a  ..t.d.t.......d.
+00005710: 7d09 7c07 640b 6b02 72aa 7c08 6402 6b02  }.|.d.k.r.|.d.k.
+00005720: 72aa 7c00 6a09 7c06 8301 7d09 640c 7c00  r.|.j.|...}.d.|.
+00005730: 5f0a 7c09 5300 290d 7aea 2052 6574 7572  _.|.S.).z. Retur
+00005740: 6e20 7468 6520 6175 7468 656e 7469 6b65  n the authentike
+00005750: 7920 2020 2020 200a 2020 2020 2020 2020  y      .        
+00005760: 0a20 2020 2020 2020 2043 6f6d 7061 7265  .        Compare
+00005770: 6420 746f 2063 6172 645f 6578 706f 7274  d to card_export
+00005780: 5f61 7574 6865 6e74 696b 6579 2829 2c20  _authentikey(), 
+00005790: 7468 6973 206d 6574 686f 6420 7261 6973  this method rais
+000057a0: 6520 556e 696e 6974 6961 6c69 7a65 6453  e UninitializedS
+000057b0: 6565 6445 7272 6f72 2069 6620 6e6f 2073  eedError if no s
+000057c0: 6565 6420 6973 2063 6f6e 6669 6775 7265  eed is configure
+000057d0: 6420 696e 2074 6865 2064 6576 6963 650a  d in the device.
+000057e0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000057f0: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
+00005800: 2020 2061 7574 6865 6e74 696b 6579 3a20     authentikey: 
+00005810: 616e 2045 4350 7562 6b65 790a 2020 2020  an ECPubkey.    
+00005820: 2020 2020 7a1d 496e 2063 6172 645f 6269      z.In card_bi
+00005830: 7033 325f 6765 745f 6175 7468 656e 7469  p32_get_authenti
+00005840: 6b65 7972 0100 0000 7242 0000 00e9 1400  keyr....rB......
+00005850: 0000 7a47 6361 7264 5f62 6970 3332 5f67  ..zGcard_bip32_g
+00005860: 6574 5f61 7574 6865 6e74 696b 6579 2829  et_authentikey()
+00005870: 3a20 5365 6564 2069 7320 6e6f 7420 696e  : Seed is not in
+00005880: 6974 6961 6c69 7a65 6420 3d3e 2052 6169  itialized => Rai
+00005890: 7369 6e67 2065 7272 6f72 217a 2453 6174  sing error!z$Sat
+000058a0: 6f63 6869 7020 7365 6564 2069 7320 6e6f  ochip seed is no
+000058b0: 7420 696e 6974 6961 6c69 7a65 6421 0a0a  t initialized!..
+000058c0: 2072 4300 0000 7a4b 6361 7264 5f62 6970   rC...zKcard_bip
+000058d0: 3332 5f67 6574 5f61 7574 6865 6e74 696b  32_get_authentik
+000058e0: 6579 2829 3a20 5361 746f 6368 6970 2069  ey(): Satochip i
+000058f0: 7320 6e6f 7420 696e 6974 6961 6c69 7a65  s not initialize
+00005900: 6420 3d3e 2052 6169 7369 6e67 2065 7272  d => Raising err
+00005910: 6f72 217a 3e53 6174 6f63 6869 7020 6973  or!z>Satochip is
+00005920: 206e 6f74 2069 6e69 7469 616c 697a 6564   not initialized
+00005930: 2120 596f 7520 7368 6f75 6c64 2063 7265  ! You should cre
+00005940: 6174 6520 6120 6e65 7720 7761 6c6c 6574  ate a new wallet
+00005950: 210a 0a4e 7241 0000 0054 290b 7227 0000  !..NrA...T).r'..
+00005960: 0072 3400 0000 722b 0000 0072 be00 0000  .r4...r+...r....
+00005970: 5a19 494e 535f 4249 5033 325f 4745 545f  Z.INS_BIP32_GET_
+00005980: 4155 5448 454e 5449 4b45 5972 9b00 0000  AUTHENTIKEYr....
+00005990: 7228 0000 0072 0401 0000 7205 0100 0072  r(...r....r....r
+000059a0: e200 0000 7279 0000 0029 0a72 3600 0000  ....ry...).r6...
+000059b0: 72a1 0000 0072 8900 0000 72a2 0000 0072  r....r....r....r
+000059c0: a300 0000 729a 0000 0072 2200 0000 725e  ....r....r"...r^
+000059d0: 0000 0072 5f00 0000 72a6 0000 0072 3700  ...r_...r....r7.
+000059e0: 0000 7237 0000 0072 3800 0000 da1a 6361  ..r7...r8.....ca
+000059f0: 7264 5f62 6970 3332 5f67 6574 5f61 7574  rd_bip32_get_aut
+00005a00: 6865 6e74 696b 6579 e002 0000 7324 0000  hentikey....s$..
+00005a10: 0000 080a 0106 0106 0104 0104 010c 0310  ................
+00005a20: 0110 010a 010c 0110 010a 010c 0204 0110  ................
+00005a30: 010a 0106 017a 2843 6172 6443 6f6e 6e65  .....z(CardConne
+00005a40: 6374 6f72 2e63 6172 645f 6269 7033 325f  ctor.card_bip32_
+00005a50: 6765 745f 6175 7468 656e 7469 6b65 7963  get_authentikeyc
+00005a60: 0200 0000 0000 0000 0d00 0000 0500 0000  ................
+00005a70: 4300 0000 7396 0000 0074 006a 0164 0183  C...s....t.j.d..
+00005a80: 0101 0074 026a 037d 0264 027d 0364 037d  ...t.j.}.d.}.d.}
+00005a90: 0464 037d 057c 006a 046a 057c 0183 017d  .d.}.|.j.j.|...}
+00005aa0: 067c 0672 927c 066a 0664 0464 058d 017d  .|.r.|.j.d.d...}
+00005ab0: 0774 077c 0764 0664 0785 0219 0083 017d  .t.|.d.d.......}
+00005ac0: 077c 0174 087c 0783 0164 0840 0074 087c  .|.t.|...d.@.t.|
+00005ad0: 0783 0164 0940 0067 0217 007c 0717 007d  ...d.@.g...|...}
+00005ae0: 0874 087c 0883 017d 097c 027c 037c 047c  .t.|...}.|.|.|.|
+00005af0: 057c 0967 057c 0817 007d 0a7c 006a 097c  .|.g.|...}.|.j.|
+00005b00: 0a83 015c 037d 017d 0b7d 0c7c 0653 0029  ...\.}.}.}.|.S.)
+00005b10: 0a7a 9820 416c 6c6f 7773 2074 6f20 636f  .z. Allows to co
+00005b20: 6d70 7574 6520 636f 6f72 6479 206f 6620  mpute coordy of 
+00005b30: 6175 7468 656e 7469 6b65 7920 6578 7465  authentikey exte
+00005b40: 726e 616c 6c79 2074 6f20 6f70 7469 6d69  rnally to optimi
+00005b50: 7a65 2063 6f6d 7075 7461 7469 6f6e 2074  ze computation t
+00005b60: 696d 652d 6f75 740a 2020 2020 2020 2020  ime-out.        
+00005b70: 636f 6f72 6479 2076 616c 7565 2069 7320  coordy value is 
+00005b80: 7665 7269 6669 6564 2062 7920 7468 6520  verified by the 
+00005b90: 6368 6970 2062 6566 6f72 6520 6265 696e  chip before bein
+00005ba0: 6720 6163 6365 7074 6564 207a 2449 6e20  g accepted z$In 
+00005bb0: 6361 7264 5f62 6970 3332 5f73 6574 5f61  card_bip32_set_a
+00005bc0: 7574 6865 6e74 696b 6579 5f70 7562 6b65  uthentikey_pubke
+00005bd0: 7972 cf00 0000 7201 0000 0046 2901 da0a  yr....r....F)...
+00005be0: 636f 6d70 7265 7373 6564 e921 0000 004e  compressed.!...N
+00005bf0: 6900 ff00 0072 d500 0000 290a 7227 0000  i....r....).r'..
+00005c00: 0072 3400 0000 722b 0000 0072 be00 0000  .r4...r+...r....
+00005c10: 7277 0000 0072 f500 0000 72e3 0000 0072  rw...r....r....r
+00005c20: c800 0000 7235 0000 0072 9b00 0000 290d  ....r5...r....).
+00005c30: 7236 0000 0072 2200 0000 72a1 0000 0072  r6...r"...r....r
+00005c40: 8900 0000 72a2 0000 0072 a300 0000 72a6  ....r....r....r.
+00005c50: 0000 00da 0663 6f6f 7264 7972 cb00 0000  .....coordyr....
+00005c60: 72cc 0000 0072 9a00 0000 725e 0000 0072  r....r....r^...r
+00005c70: 5f00 0000 7237 0000 0072 3700 0000 7238  _...r7...r7...r8
+00005c80: 0000 0072 e200 0000 fe02 0000 731c 0000  ...r........s...
+00005c90: 0000 030a 0106 0104 0104 0104 020c 0104  ................
+00005ca0: 010c 0110 0120 0108 0112 0110 017a 2f43  ..... .......z/C
+00005cb0: 6172 6443 6f6e 6e65 6374 6f72 2e63 6172  ardConnector.car
+00005cc0: 645f 6269 7033 325f 7365 745f 6175 7468  d_bip32_set_auth
+00005cd0: 656e 7469 6b65 795f 7075 626b 6579 6302  entikey_pubkeyc.
+00005ce0: 0000 0000 0000 0016 0000 0006 0000 0043  ...............C
+00005cf0: 0000 0073 d601 0000 7400 7c01 8301 7401  ...s....t.|...t.
+00005d00: 6b02 721c 7c00 6a02 6a03 7c01 8301 5c02  k.r.|.j.j.|...\.
+00005d10: 7d02 7d01 7404 6a05 6401 8301 0100 7406  }.}.t.j.d.....t.
+00005d20: 6a07 7d03 7406 6a08 7d04 7409 7c01 8301  j.}.t.j.}.t.|...
+00005d30: 6402 1a00 7d05 6403 7d06 7409 7c01 8301  d...}.d.}.t.|...
+00005d40: 7d07 7c03 7c04 7c05 7c06 7c07 6705 7d08  }.|.|.|.|.|.g.}.
+00005d50: 7c08 7c01 3700 7d08 7c00 6a02 6a0a 6404  |.|.7.}.|.j.j.d.
+00005d60: 6b08 7274 7c00 6a0b 8300 0100 9001 785a  k.rt|.j.......xZ
+00005d70: 7c00 6a0c 7c08 8301 5c03 7d09 7d0a 7d0b  |.j.|...\.}.}.}.
+00005d80: 7c0a 6405 6b02 72d2 7c0b 6406 6b02 72d2  |.d.k.r.|.d.k.r.
+00005d90: 7404 6a0d 6407 8301 0100 7c08 6408 1900  t.j.d.....|.d...
+00005da0: 6409 4100 7c08 6408 3c00 7c00 6a0c 7c08  d.A.|.d.<.|.j.|.
+00005db0: 8301 5c03 7d09 7d0a 7d0b 7c08 6408 1900  ..\.}.}.}.|.d...
+00005dc0: 640a 4000 7c08 6408 3c00 7c0a 640b 6b03  d.@.|.d.<.|.d.k.
+00005dd0: 73e4 7c0b 640c 6b03 9001 7202 740e 640d  s.|.d.k...r.t.d.
+00005de0: 740f 640e 7c0a 1400 7c0b 1700 8301 9b00  t.d.|...|.......
+00005df0: 640f 9d03 8301 8201 7178 7c09 6410 1900  d.......qx|.d...
+00005e00: 6409 4000 6409 6b02 9001 72b6 7404 6a0d  d.@.d.k...r.t.j.
+00005e10: 6411 8301 0100 7c00 6a02 6a10 7c09 8301  d.....|.j.j.|...
+00005e20: 5c02 7d0c 7d0d 7c0c 6a11 6412 6413 8d01  \.}.}.|.j.d.d...
+00005e30: 7d0e 7412 7c0e 6414 6404 8502 1900 8301  }.t.|.d.d.......
+00005e40: 7d0e 7c00 6a02 6a0a 6a11 6412 6413 8d01  }.|.j.j.j.d.d...
+00005e50: 7d0f 7412 7c0f 6414 6404 8502 1900 8301  }.t.|.d.d.......
+00005e60: 7d0f 7c09 7409 7c0e 8301 6415 4000 7409  }.|.t.|...d.@.t.
+00005e70: 7c0e 8301 6416 4000 6702 1700 7c0e 1700  |...d.@.g...|...
+00005e80: 7d10 7c03 6417 640c 640c 7409 7c10 8301  }.|.d.d.d.t.|...
+00005e90: 6705 7d11 7c11 7c10 1700 7d11 7c00 6a0c  g.}.|.|...}.|.j.
+00005ea0: 7c11 8301 5c03 7d12 7d13 7d14 7178 7c00  |...\.}.}.}.qx|.
+00005eb0: 6a02 6a10 7c09 8301 5c02 7d15 7d0d 7c15  j.j.|...\.}.}.|.
+00005ec0: 7c0d 6602 5300 7178 5700 6404 5300 2918  |.f.S.qxW.d.S.).
+00005ed0: 6119 0100 0020 4765 7420 7468 6520 4249  a.... Get the BI
+00005ee0: 5033 3220 6578 7465 6e64 6564 206b 6579  P32 extended key
+00005ef0: 2066 6f72 2067 6976 656e 2070 6174 680a   for given path.
+00005f00: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00005f10: 2050 6172 616d 6574 6572 733a 200a 2020   Parameters: .  
+00005f20: 2020 2020 2020 7061 7468 2028 7374 7220        path (str 
+00005f30: 7c20 6279 7465 7329 3a20 7468 6520 7061  | bytes): the pa
+00005f40: 7468 3b20 6966 2067 6976 656e 2061 7320  th; if given as 
+00005f50: 6120 7374 7269 6e67 2c20 6974 2077 696c  a string, it wil
+00005f60: 6c20 6265 2063 6f6e 7665 7274 6564 2074  l be converted t
+00005f70: 6f20 6279 7465 7320 2834 2062 7974 6573  o bytes (4 bytes
+00005f80: 2066 6f72 2065 6163 6820 7061 7468 2069   for each path i
+00005f90: 6e64 6578 290a 0a20 2020 2020 2020 2052  ndex)..        R
+00005fa0: 6574 7572 6e73 3a20 0a20 2020 2020 2020  eturns: .       
+00005fb0: 2070 7562 6b65 793a 2045 4350 7562 6b65   pubkey: ECPubke
+00005fc0: 7920 6f62 6a65 6374 0a20 2020 2020 2020  y object.       
+00005fd0: 2063 6861 696e 636f 6465 3a20 6279 7465   chaincode: byte
+00005fe0: 6172 7261 790a 2020 2020 2020 2020 7a1d  array.        z.
+00005ff0: 496e 2063 6172 645f 6269 7033 325f 6765  In card_bip32_ge
+00006000: 745f 6578 7465 6e64 6564 6b65 7972 4300  t_extendedkeyrC.
+00006010: 0000 e940 0000 004e 7242 0000 0072 0c00  ...@...NrB...r..
+00006020: 0000 7a2c 5b63 6172 645f 6269 7033 325f  ..z,[card_bip32_
+00006030: 6765 745f 6578 7465 6e64 6564 6b65 795d  get_extendedkey]
+00006040: 2052 6573 6574 206d 656d 6f72 792e 2e2e   Reset memory...
+00006050: 72b3 0000 0072 9d00 0000 72a0 0000 0072  r....r....r....r
+00006060: 4100 0000 7201 0000 007a 1e55 6e65 7870  A...r....z.Unexp
+00006070: 6563 7465 6420 6572 726f 7220 2028 6572  ected error  (er
+00006080: 726f 7220 636f 6465 2072 bc00 0000 72bd  ror code r....r.
+00006090: 0000 00e9 2000 0000 7a3d 5b63 6172 645f  .... ...z=[card_
+000060a0: 6269 7033 325f 6765 745f 6578 7465 6e64  bip32_get_extend
+000060b0: 6564 6b65 795d 2043 6869 6c64 2044 6572  edkey] Child Der
+000060c0: 6976 6174 696f 6e20 6f70 7469 6d69 7a61  ivation optimiza
+000060d0: 7469 6f6e 2e2e 2e46 2901 720b 0100 0072  tion...F).r....r
+000060e0: 0c01 0000 6900 ff00 0072 d500 0000 7268  ....i....r....rh
+000060f0: 0000 0029 1372 2600 0000 7276 0000 0072  ...).r&...rv...r
+00006100: 7700 0000 da0f 6269 7033 3270 6174 6832  w.....bip32path2
+00006110: 6279 7465 7372 2700 0000 7234 0000 0072  bytesr'...r4...r
+00006120: 2b00 0000 72be 0000 005a 1a49 4e53 5f42  +...r....Z.INS_B
+00006130: 4950 3332 5f47 4554 5f45 5854 454e 4445  IP32_GET_EXTENDE
+00006140: 445f 4b45 5972 3500 0000 72a6 0000 0072  D_KEYr5...r....r
+00006150: 0a01 0000 729b 0000 0072 2800 0000 72f4  ....r....r(...r.
+00006160: 0000 0072 4c00 0000 5a1b 7061 7273 655f  ...rL...Z.parse_
+00006170: 6269 7033 325f 6765 745f 6578 7465 6e64  bip32_get_extend
+00006180: 6564 6b65 7972 e300 0000 72c8 0000 0029  edkeyr....r....)
+00006190: 1672 3600 0000 da04 7061 7468 da05 6465  .r6.....path..de
+000061a0: 7074 6872 a100 0000 7289 0000 0072 a200  pthr....r....r..
+000061b0: 0000 72a3 0000 0072 cc00 0000 729a 0000  ..r....r....r...
+000061c0: 0072 2200 0000 725e 0000 0072 5f00 0000  .r"...r^...r_...
+000061d0: da06 7075 626b 6579 5a09 6368 6169 6e63  ..pubkeyZ.chainc
+000061e0: 6f64 6572 0d01 0000 5a0a 6175 7468 636f  oder....Z.authco
+000061f0: 6f72 6479 72cb 0000 005a 0861 7064 755f  ordyr....Z.apdu_
+00006200: 6f70 745a 0c72 6573 706f 6e73 655f 6f70  optZ.response_op
+00006210: 745a 0773 7731 5f6f 7074 5a07 7377 325f  tZ.sw1_optZ.sw2_
+00006220: 6f70 74da 036b 6579 7237 0000 0072 3700  opt..keyr7...r7.
+00006230: 0000 7238 0000 00da 1a63 6172 645f 6269  ..r8.....card_bi
+00006240: 7033 325f 6765 745f 6578 7465 6e64 6564  p32_get_extended
+00006250: 6b65 7911 0300 0073 4400 0000 000a 0c01  key....sD.......
+00006260: 1002 0a01 0601 0601 0c01 0401 0801 0e01  ................
+00006270: 0802 0c01 0803 0401 1004 1001 0a01 1001  ................
+00006280: 1001 1002 1201 1e02 1201 0a01 1001 0c01  ................
+00006290: 1001 1001 1001 2001 1201 0801 1203 1001  ...... .........
+000062a0: 7a28 4361 7264 436f 6e6e 6563 746f 722e  z(CardConnector.
+000062b0: 6361 7264 5f62 6970 3332 5f67 6574 5f65  card_bip32_get_e
+000062c0: 7874 656e 6465 646b 6579 6304 0000 0000  xtendedkeyc.....
+000062d0: 0000 000e 0000 0005 0000 0043 0000 0073  ...........C...s
+000062e0: 2001 0000 7c02 7400 6b06 730c 7401 8201   ...|.t.k.s.t...
+000062f0: 7402 6a03 6401 7404 7c01 8301 9b00 9d02  t.j.d.t.|.......
+00006300: 8301 0100 7405 7c01 8301 7404 6b02 723c  ....t.|...t.k.r<
+00006310: 7c00 6a06 6a07 7c01 8301 5c02 7d04 7d05  |.j.j.|...\.}.}.
+00006320: 7c00 6a08 7c05 8301 5c02 7d06 7d07 7c04  |.j.|...\.}.}.|.
+00006330: 6402 6b02 7274 7409 6402 6402 6402 6402  d.k.rtt.d.d.d.d.
+00006340: 6704 8301 7d08 7409 6402 6402 6402 6402  g...}.t.d.d.d.d.
+00006350: 6704 8301 7d09 6e3a 7c00 6a08 7c05 6402  g...}.n:|.j.|.d.
+00006360: 6409 8502 1900 8301 5c02 7d0a 7d0b 740a  d.......\.}.}.t.
+00006370: 7c0a 6a0b 6404 6405 8d01 8301 6402 6403  |.j.d.d.....d.d.
+00006380: 8502 1900 7d08 7c05 640a 6406 8502 1900  ....}.|.d.d.....
+00006390: 7d09 7c03 72ba 740c 7c02 1900 6e06 740d  }.|.r.t.|...n.t.
+000063a0: 7c02 1900 7d0c 7409 6a0e 7c0c 8301 7409  |...}.t.j.|...t.
+000063b0: 7c04 6701 8301 1700 7c08 1700 7c09 1700  |.g.....|...|...
+000063c0: 7c07 1700 7c06 6a0b 6404 6405 8d01 1700  |...|.j.d.d.....
+000063d0: 7d0d 740f 7c0d 8301 6407 6b02 9001 7300  }.t.|...d.k...s.
+000063e0: 7401 8201 7410 7c0d 8301 7d0d 7402 6a03  t...t.|...}.t.j.
+000063f0: 6408 7404 7c0d 8301 9b00 9d02 8301 0100  d.t.|...........
+00006400: 7c0d 5300 290b 61b1 0100 0020 4765 7420  |.S.).a.... Get 
+00006410: 7468 6520 4249 5033 3220 7870 7562 2066  the BIP32 xpub f
+00006420: 6f72 2067 6976 656e 2070 6174 682e 0a20  or given path.. 
+00006430: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00006440: 5061 7261 6d65 7465 7273 3a20 0a20 2020  Parameters: .   
+00006450: 2020 2020 2070 6174 6820 2873 7472 207c       path (str |
+00006460: 2062 7974 6573 293a 2074 6865 2070 6174   bytes): the pat
+00006470: 683b 2069 6620 6769 7665 6e20 6173 2061  h; if given as a
+00006480: 2073 7472 696e 672c 2069 7420 7769 6c6c   string, it will
+00006490: 2062 6520 636f 6e76 6572 7465 6420 746f   be converted to
+000064a0: 2062 7974 6573 2028 3420 6279 7465 7320   bytes (4 bytes 
+000064b0: 666f 7220 6561 6368 2070 6174 6820 696e  for each path in
+000064c0: 6465 7829 0a20 2020 2020 2020 2078 7479  dex).        xty
+000064d0: 7065 2028 7374 7229 3a20 7468 6520 7479  pe (str): the ty
+000064e0: 7065 206f 6620 7472 616e 7361 6374 696f  pe of transactio
+000064f0: 6e20 7375 6368 2061 7320 2027 7374 616e  n such as  'stan
+00006500: 6461 7264 272c 2027 7032 7770 6b68 2d70  dard', 'p2wpkh-p
+00006510: 3273 6827 2c20 2770 3277 706b 6827 2c20  2sh', 'p2wpkh', 
+00006520: 2770 3277 7368 2d70 3273 6827 2c20 2770  'p2wsh-p2sh', 'p
+00006530: 3277 7368 270a 2020 2020 2020 2020 6973  2wsh'.        is
+00006540: 5f6d 6169 6e6e 6574 2028 626f 6f6c 293a  _mainnet (bool):
+00006550: 2069 7320 6d61 696e 6e65 7420 6f72 2074   is mainnet or t
+00006560: 6573 746e 6574 200a 2020 2020 2020 2020  estnet .        
+00006570: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00006580: 3a20 0a20 2020 2020 2020 2078 7075 6220  : .        xpub 
+00006590: 2873 7472 293a 2074 6865 2063 6f72 7265  (str): the corre
+000065a0: 7370 6f6e 6469 6e67 2078 7075 6220 7661  sponding xpub va
+000065b0: 6c75 650a 2020 2020 2020 2020 7a1c 6361  lue.        z.ca
+000065c0: 7264 5f62 6970 3332 5f67 6574 5f78 7075  rd_bip32_get_xpu
+000065d0: 6228 293a 2070 6174 683d 7201 0000 0072  b(): path=r....r
+000065e0: 4300 0000 5429 0172 0b01 0000 4ee9 4e00  C...T).r....N.N.
+000065f0: 0000 7a1c 6361 7264 5f62 6970 3332 5f67  ..z.card_bip32_g
+00006600: 6574 5f78 7075 6228 293a 2078 7075 623d  et_xpub(): xpub=
+00006610: e9fc ffff ff72 1701 0000 2911 da10 5355  .....r....)...SU
+00006620: 5050 4f52 5445 445f 5854 5950 4553 da0e  PPORTED_XTYPES..
+00006630: 4173 7365 7274 696f 6e45 7272 6f72 7227  AssertionErrorr'
+00006640: 0000 0072 2800 0000 7276 0000 0072 2600  ...r(...rv...r&.
+00006650: 0000 7277 0000 0072 1001 0000 7215 0100  ..rw...r....r...
+00006660: 0072 4b00 0000 7215 0000 0072 e300 0000  .rK...r....r....
+00006670: da14 5850 5542 5f48 4541 4445 5253 5f4d  ..XPUB_HEADERS_M
+00006680: 4149 4e4e 4554 da14 5850 5542 5f48 4541  AINNET..XPUB_HEA
+00006690: 4445 5253 5f54 4553 544e 4554 72e1 0000  DERS_TESTNETr...
+000066a0: 0072 3500 0000 7216 0000 0029 0e72 3600  .r5...r....).r6.
+000066b0: 0000 7211 0100 005a 0578 7479 7065 5a0a  ..r....Z.xtypeZ.
+000066c0: 6973 5f6d 6169 6e6e 6574 7212 0100 005a  is_mainnetr....Z
+000066d0: 0862 7974 6570 6174 685a 0863 6869 6c64  .bytepathZ.child
+000066e0: 6b65 795a 0e63 6869 6c64 6368 6169 6e63  keyZ.childchainc
+000066f0: 6f64 65da 0b66 696e 6765 7270 7269 6e74  ode..fingerprint
+00006700: 5a0c 6368 696c 645f 6e75 6d62 6572 5a09  Z.child_numberZ.
+00006710: 7061 7265 6e74 6b65 795a 0f70 6172 656e  parentkeyZ.paren
+00006720: 7463 6861 696e 636f 6465 5a0b 7870 7562  tchaincodeZ.xpub
+00006730: 5f68 6561 6465 725a 0478 7075 6272 3700  _headerZ.xpubr7.
+00006740: 0000 7237 0000 0072 3800 0000 da13 6361  ..r7...r8.....ca
+00006750: 7264 5f62 6970 3332 5f67 6574 5f78 7075  rd_bip32_get_xpu
+00006760: 6249 0300 0073 2200 0000 000b 0c03 1401  bI...s".........
+00006770: 0c01 1002 0e01 0801 1001 1202 1601 1801  ................
+00006780: 0c02 1401 2c01 1201 0801 1401 7a21 4361  ....,.......z!Ca
+00006790: 7264 436f 6e6e 6563 746f 722e 6361 7264  rdConnector.card
+000067a0: 5f62 6970 3332 5f67 6574 5f78 7075 62f3  _bip32_get_xpub.
+000067b0: 0000 0000 6306 0000 0000 0000 0015 0000  ....c...........
+000067c0: 0005 0000 0043 0000 0073 2602 0000 7400  .....C...s&...t.
+000067d0: 6a01 6401 8301 0100 7402 7c03 8301 7403  j.d.....t.|...t.
+000067e0: 6b02 7220 7c03 6a04 6402 8301 7d03 7402  k.r |.j.d...}.t.
+000067f0: 7c05 8301 7403 6b02 7236 7c05 6a04 6402  |...t.k.r6|.j.d.
+00006800: 8301 7d05 6403 7d06 6404 7d07 7405 7c03  ..}.d.}.d.}.t.|.
+00006810: 8301 7d08 7406 6a07 7d09 7406 6a08 7d0a  ..}.t.j.}.t.j.}.
+00006820: 7c01 7d0b 7406 6a09 7d0c 7c05 7364 6405  |.}.t.j.}.|.sdd.
+00006830: 6e0a 640f 7405 7c05 8301 1700 7d0d 7c09  n.d.t.|.....}.|.
+00006840: 7c0a 7c0b 7c0c 7c0d 6705 7d0e 782a 740a  |.|.|.|.g.}.x*t.
+00006850: 740b 6405 8301 8301 4400 5d1a 7d0f 7c0e  t.d.....D.].}.|.
+00006860: 7c08 6407 7c0f 1400 3f00 6408 4000 6701  |.d.|...?.d.@.g.
+00006870: 3700 7d0e 718c 5700 7c05 72c4 7c0e 7405  7.}.q.W.|.r.|.t.
+00006880: 7c05 8301 6701 3700 7d0e 7c0e 7c05 3700  |...g.7.}.|.|.7.
+00006890: 7d0e 7c00 6a0c 7c0e 8301 5c03 7d10 7d11  }.|.j.|...\.}.}.
+000068a0: 7d12 7876 7c08 7c06 6b04 9001 724a 7406  }.xv|.|.k...rJt.
+000068b0: 6a0d 7d0c 6409 7c06 1700 7d0d 7c09 7c0a  j.}.d.|...}.|.|.
+000068c0: 7c0b 7c0c 7c0d 6705 7d0e 7c0e 7c06 6407  |.|.|.g.}.|.|.d.
+000068d0: 3f00 6408 4000 7c06 6408 4000 6702 3700  ?.d.@.|.d.@.g.7.
+000068e0: 7d0e 7c0e 7c03 7c07 7c07 7c06 1700 8502  }.|.|.|.|.|.....
+000068f0: 1900 3700 7d0e 7c07 7c06 3700 7d07 7c08  ..7.}.|.|.7.}.|.
+00006900: 7c06 3800 7d08 7c00 6a0c 7c0e 8301 5c03  |.8.}.|.j.|...\.
+00006910: 7d10 7d11 7d12 71d6 5700 7c08 7d06 7406  }.}.}.q.W.|.}.t.
+00006920: 6a0e 7d0c 6409 7c06 1700 7405 7c04 8301  j.}.d.|...t.|...
+00006930: 1700 7d0d 7c09 7c0a 7c0b 7c0c 7c0d 6705  ..}.|.|.|.|.|.g.
+00006940: 7d0e 7c0e 7c06 6407 3f00 6408 4000 7c06  }.|.|.d.?.d.@.|.
+00006950: 6408 4000 6702 3700 7d0e 7c0e 7c03 7c07  d.@.g.7.}.|.|.|.
+00006960: 7c07 7c06 1700 8502 1900 7c04 1700 3700  |.|.......|...7.
+00006970: 7d0e 7c07 7c06 3700 7d07 7c08 7c06 3800  }.|.|.7.}.|.|.8.
+00006980: 7d08 7c00 6a0c 7c0e 8301 5c03 7d10 7d11  }.|.j.|...\.}.}.
+00006990: 7d12 7c11 640a 6b03 9001 73d8 7c12 6404  }.|.d.k...s.|.d.
+000069a0: 6b03 9001 72fc 7400 6a0f 640b 7410 640c  k...r.t.j.d.t.d.
+000069b0: 7c11 1400 7c12 1700 8301 9b00 640d 9d03  |...|.......d...
+000069c0: 8301 0100 640e 7d13 6e1e 7411 7412 7c03  ....d.}.n.t.t.|.
+000069d0: 7c05 8302 8301 7d14 7c00 6a13 6a14 7c10  |.....}.|.j.j.|.
+000069e0: 7c14 7c02 8303 7d13 7c10 7c11 7c12 7c13  |.|...}.|.|.|.|.
+000069f0: 6604 5300 2910 6134 0300 0020 5369 676e  f.S.).a4... Sign
+00006a00: 2074 6865 206d 6573 7361 6765 2077 6974   the message wit
+00006a10: 6820 7468 6520 6465 7669 6365 0a20 2020  h the device.   
+00006a20: 2020 2020 200a 2020 2020 2020 2020 4d65       .        Me
+00006a30: 7373 6167 6520 6973 2070 7265 7065 6e64  ssage is prepend
+00006a40: 6564 2077 6974 6820 6120 7370 6563 6966  ed with a specif
+00006a50: 6963 2068 6561 6465 7220 6173 2064 6573  ic header as des
+00006a60: 6372 6962 6564 2068 6572 653a 0a20 2020  cribed here:.   
+00006a70: 2020 2020 2068 7474 7073 3a2f 2f62 6974       https://bit
+00006a80: 636f 696e 2e73 7461 636b 6578 6368 616e  coin.stackexchan
+00006a90: 6765 2e63 6f6d 2f71 7565 7374 696f 6e73  ge.com/questions
+00006aa0: 2f37 3733 3234 2f68 6f77 2d61 7265 2d62  /77324/how-are-b
+00006ab0: 6974 636f 696e 2d73 6967 6e65 642d 6d65  itcoin-signed-me
+00006ac0: 7373 6167 6573 2d67 656e 6572 6174 6564  ssages-generated
+00006ad0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00006ae0: 2020 5061 7261 6d65 7465 7273 3a20 0a20    Parameters: . 
+00006af0: 2020 2020 2020 206b 6579 6e62 7220 2869         keynbr (i
+00006b00: 6e74 293a 2074 6865 206b 6579 2074 6f20  nt): the key to 
+00006b10: 7573 6520 2830 7846 4620 666f 7220 6269  use (0xFF for bi
+00006b20: 7033 3220 6b65 7929 0a20 2020 2020 2020  p32 key).       
+00006b30: 2070 7562 6b65 7920 2845 4350 7562 6b65   pubkey (ECPubke
+00006b40: 7929 3a20 7468 6520 7075 626b 6579 2075  y): the pubkey u
+00006b50: 7365 6420 666f 7220 7369 676e 696e 673b  sed for signing;
+00006b60: 2074 6869 7320 6973 2075 7365 6420 666f   this is used fo
+00006b70: 7220 6b65 7920 7265 636f 7665 7279 0a20  r key recovery. 
+00006b80: 2020 2020 2020 206d 6573 7361 6765 2028         message (
+00006b90: 7374 7220 7c20 6279 7465 7329 3a20 7468  str | bytes): th
+00006ba0: 6520 6d65 7373 6167 6520 746f 2073 6967  e message to sig
+00006bb0: 6e0a 2020 2020 2020 2020 686d 6163 3a20  n.        hmac: 
+00006bc0: 7468 6520 3230 2d62 7974 6520 686d 6163  the 20-byte hmac
+00006bd0: 2063 6f64 6520 7265 7175 6972 6564 2069   code required i
+00006be0: 6620 3246 4120 6973 2065 6e61 626c 6564  f 2FA is enabled
+00006bf0: 0a20 2020 2020 2020 2061 6c74 636f 696e  .        altcoin
+00006c00: 2028 7374 7220 7c20 6279 7465 7329 3a20   (str | bytes): 
+00006c10: 666f 7220 616c 7463 6f69 6e20 7369 676e  for altcoin sign
+00006c20: 696e 670a 2020 2020 2020 2020 0a20 2020  ing.        .   
+00006c30: 2020 2020 2052 6574 7572 6e73 3a20 0a20       Returns: . 
+00006c40: 2020 2020 2020 2028 7265 7370 6f6e 7365         (response
+00006c50: 2c20 7377 312c 2073 7732 2c20 636f 6d70  , sw1, sw2, comp
+00006c60: 7369 6729 3a20 286c 6973 742c 2069 6e74  sig): (list, int
+00006c70: 2c20 696e 742c 2062 7974 6573 290a 2020  , int, bytes).  
+00006c80: 2020 2020 2020 636f 6d70 7369 6720 6973        compsig is
+00006c90: 2074 6865 2073 6967 6e61 7475 7265 2069   the signature i
+00006ca0: 6e20 2063 6f6d 7061 6374 2036 352d 6279  n  compact 65-by
+00006cb0: 7465 2066 6f72 6d61 7420 0a20 2020 2020  te format .     
+00006cc0: 2020 2028 6874 7470 733a 2f2f 6269 7463     (https://bitc
+00006cd0: 6f69 6e2e 7374 6163 6b65 7863 6861 6e67  oin.stackexchang
+00006ce0: 652e 636f 6d2f 7175 6573 7469 6f6e 732f  e.com/questions/
+00006cf0: 3132 3535 342f 7768 792d 7468 652d 7369  12554/why-the-si
+00006d00: 676e 6174 7572 652d 6973 2d61 6c77 6179  gnature-is-alway
+00006d10: 732d 3635 2d31 3332 3332 2d62 7974 6573  s-65-13232-bytes
+00006d20: 2d6c 6f6e 6729 0a20 2020 2020 2020 207a  -long).        z
+00006d30: 1449 6e20 6361 7264 5f73 6967 6e5f 6d65  .In card_sign_me
+00006d40: 7373 6167 6572 c100 0000 729d 0000 0072  ssager....r....r
+00006d50: 0100 0000 7243 0000 0072 0c00 0000 72b4  ....rC...r....r.
+00006d60: 0000 0072 d500 0000 7223 0000 0072 4100  ...r....r#...rA.
+00006d70: 0000 7a34 556e 6578 7065 6374 6564 2065  ..z4Unexpected e
+00006d80: 7272 6f72 2069 6e20 6361 7264 5f73 6967  rror in card_sig
+00006d90: 6e5f 6d65 7373 6167 6528 2920 2865 7272  n_message() (err
+00006da0: 6f72 2063 6f64 6520 72bc 0000 0072 bd00  or code r....r..
+00006db0: 0000 721e 0100 0072 2100 0000 2915 7227  ..r....r!...).r'
+00006dc0: 0000 0072 3400 0000 7226 0000 0072 7600  ...r4...r&...rv.
+00006dd0: 0000 72c9 0000 0072 3500 0000 722b 0000  ..r....r5...r+..
+00006de0: 0072 be00 0000 5a10 494e 535f 5349 474e  .r....Z.INS_SIGN
+00006df0: 5f4d 4553 5341 4745 da07 4f50 5f49 4e49  _MESSAGE..OP_INI
+00006e00: 5472 d600 0000 72d7 0000 0072 9b00 0000  Tr....r....r....
+00006e10: da0a 4f50 5f50 524f 4345 5353 da0b 4f50  ..OP_PROCESS..OP
+00006e20: 5f46 494e 414c 495a 4572 5400 0000 724c  _FINALIZErT...rL
+00006e30: 0000 0072 1400 0000 7213 0000 0072 7700  ...r....r....rw.
+00006e40: 0000 5a17 7061 7273 655f 6d65 7373 6167  ..Z.parse_messag
+00006e50: 655f 7369 676e 6174 7572 6529 1572 3600  e_signature).r6.
+00006e60: 0000 da06 6b65 796e 6272 7213 0100 00da  ....keynbrr.....
+00006e70: 076d 6573 7361 6765 72ed 0000 005a 0761  .messager....Z.a
+00006e80: 6c74 636f 696e da05 6368 756e 6bda 0d62  ltcoin..chunk..b
+00006e90: 7566 6665 725f 6f66 6673 6574 da0b 6275  uffer_offset..bu
+00006ea0: 6666 6572 5f6c 6566 7472 a100 0000 7289  ffer_leftr....r.
+00006eb0: 0000 0072 a200 0000 72a3 0000 0072 cc00  ...r....r....r..
+00006ec0: 0000 729a 0000 0072 dd00 0000 7222 0000  ..r....r....r"..
+00006ed0: 0072 5e00 0000 725f 0000 005a 0763 6f6d  .r^...r_...Z.com
+00006ee0: 7073 6967 da04 6861 7368 7237 0000 0072  psig..hashr7...r
+00006ef0: 3700 0000 7238 0000 00da 1163 6172 645f  7...r8.....card_
+00006f00: 7369 676e 5f6d 6573 7361 6765 6f03 0000  sign_messageo...
+00006f10: 7358 0000 0000 120a 010c 010a 010c 010a  sX..............
+00006f20: 0404 0104 0108 0306 0106 0104 0106 0114  ................
+00006f30: 010e 0112 011a 0104 010e 0108 0310 030c  ................
+00006f40: 0406 0108 010e 0118 0114 0108 0108 0214  ................
+00006f50: 0304 0406 0110 010e 0118 0118 0108 0108  ................
+00006f60: 0210 0314 011e 0106 030e 0110 027a 1f43  .............z.C
+00006f70: 6172 6443 6f6e 6e65 6374 6f72 2e63 6172  ardConnector.car
+00006f80: 645f 7369 676e 5f6d 6573 7361 6765 4629  d_sign_messageF)
+00006f90: 01da 0b74 7261 6e73 6163 7469 6f6e 6303  ...transactionc.
+00006fa0: 0000 0000 0000 0010 0000 0005 0000 0043  ...............C
+00006fb0: 0000 0073 a400 0000 7400 6a01 6401 8301  ...s....t.j.d...
+00006fc0: 0100 7402 6a03 7d03 7402 6a04 7d04 7402  ..t.j.}.t.j.}.t.
+00006fd0: 6a05 7d05 7c02 7224 6402 6e02 6403 7d06  j.}.|.r$d.n.d.}.
+00006fe0: 7406 7c01 8301 7d07 7854 7c07 6a07 8300  t.|...}.xT|.j...
+00006ff0: 7384 7c02 7246 7c07 6a08 8300 6e06 7c07  s.|.rF|.j...n.|.
+00007000: 6a09 8300 7d08 740a 7c08 8301 7d09 7c03  j...}.t.|...}.|.
+00007010: 7c04 7c05 7c06 7c09 6705 7d0a 7c0a 7c08  |.|.|.|.g.}.|.|.
+00007020: 3700 7d0a 7c00 6a0b 7c0a 8301 5c03 7d0b  7.}.|.j.|...\.}.
+00007030: 7d0c 7d0d 7402 6a0c 7d05 7132 5700 7c00  }.}.t.j.}.q2W.|.
+00007040: 6a0d 6a0e 7c0b 8301 5c02 7d0e 7d0f 7c0b  j.j.|...\.}.}.|.
+00007050: 7c0c 7c0d 7c0e 7c0f 6605 5300 2904 615a  |.|.|.|.f.S.).aZ
+00007060: 0100 0020 5061 7273 6520 6120 7472 616e  ... Parse a tran
+00007070: 7361 6374 696f 6e20 746f 2062 6520 7369  saction to be si
+00007080: 676e 6564 2062 7920 7468 6520 6465 7669  gned by the devi
+00007090: 6365 0a20 2020 2020 2020 200a 2020 2020  ce.        .    
+000070a0: 2020 2020 5061 7261 6d65 7465 7273 3a20      Parameters: 
+000070b0: 0a20 2020 2020 2020 2074 7261 6e73 6163  .        transac
+000070c0: 7469 6f6e 2028 6279 7465 7329 3a20 7468  tion (bytes): th
+000070d0: 6520 7472 616e 7361 6374 696f 6e20 746f  e transaction to
+000070e0: 2070 6172 7365 0a20 2020 2020 2020 2069   parse.        i
+000070f0: 735f 7365 6777 6974 2028 626f 6f6c 290a  s_segwit (bool).
+00007100: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00007110: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
+00007120: 2020 2028 7265 7370 6f6e 7365 2c20 7377     (response, sw
+00007130: 312c 2073 7732 2c20 7478 5f68 6173 682c  1, sw2, tx_hash,
+00007140: 206e 6565 6473 5f32 6661 290a 2020 2020   needs_2fa).    
+00007150: 2020 2020 7478 5f68 6173 6820 286c 6973      tx_hash (lis
+00007160: 7429 3a20 6861 7368 2061 7320 636f 6d70  t): hash as comp
+00007170: 7574 6564 2062 7920 7468 6520 6465 7669  uted by the devi
+00007180: 6365 0a20 2020 2020 2020 206e 6565 6473  ce.        needs
+00007190: 5f32 4641 2028 626f 6f6c 293a 2077 6865  _2FA (bool): whe
+000071a0: 7468 6572 2032 4641 2069 7320 7265 7175  ther 2FA is requ
+000071b0: 6972 6564 0a20 2020 2020 2020 207a 1949  ired.        z.I
+000071c0: 6e20 6361 7264 5f70 6172 7365 5f74 7261  n card_parse_tra
+000071d0: 6e73 6163 7469 6f6e 720c 0000 0072 0100  nsactionr....r..
+000071e0: 0000 290f 7227 0000 0072 3400 0000 722b  ..).r'...r4...r+
+000071f0: 0000 0072 be00 0000 5a15 494e 535f 5041  ...r....Z.INS_PA
+00007200: 5253 455f 5452 414e 5341 4354 494f 4e72  RSE_TRANSACTIONr
+00007210: 1f01 0000 720f 0000 005a 0969 735f 7061  ....r....Z.is_pa
+00007220: 7273 6564 5a18 7061 7273 655f 7365 6777  rsedZ.parse_segw
+00007230: 6974 5f74 7261 6e73 6163 7469 6f6e 5a11  it_transactionZ.
+00007240: 7061 7273 655f 7472 616e 7361 6374 696f  parse_transactio
+00007250: 6e72 3500 0000 729b 0000 0072 2001 0000  nr5...r....r ...
+00007260: 7277 0000 005a 1770 6172 7365 5f70 6172  rw...Z.parse_par
+00007270: 7365 5f74 7261 6e73 6163 7469 6f6e 2910  se_transaction).
+00007280: 7236 0000 0072 2901 0000 5a09 6973 5f73  r6...r)...Z.is_s
+00007290: 6567 7769 7472 a100 0000 7289 0000 0072  egwitr....r....r
+000072a0: a200 0000 72a3 0000 005a 0874 7870 6172  ....r....Z.txpar
+000072b0: 7365 7272 2401 0000 72cc 0000 0072 9a00  serr$...r....r..
+000072c0: 0000 7222 0000 0072 5e00 0000 725f 0000  ..r"...r^...r_..
+000072d0: 005a 0774 785f 6861 7368 5a09 6e65 6564  .Z.tx_hashZ.need
+000072e0: 735f 3266 6172 3700 0000 7237 0000 0072  s_2far7...r7...r
+000072f0: 3800 0000 da16 6361 7264 5f70 6172 7365  8.....card_parse
+00007300: 5f74 7261 6e73 6163 7469 6f6e c603 0000  _transaction....
+00007310: 731e 0000 0000 0c0a 0106 0106 0106 010c  s...............
+00007320: 0308 010a 0214 0108 010e 0108 0c10 030a  ................
+00007330: 0310 027a 2443 6172 6443 6f6e 6e65 6374  ...z$CardConnect
+00007340: 6f72 2e63 6172 645f 7061 7273 655f 7472  or.card_parse_tr
+00007350: 616e 7361 6374 696f 6e63 0400 0000 0000  ansactionc......
+00007360: 0000 0e00 0000 0500 0000 4300 0000 73c0  ..........C...s.
+00007370: 0000 0074 006a 0164 0183 0101 0074 026a  ...t.j.d.....t.j
+00007380: 037d 0474 026a 047d 057c 017d 0664 027d  .}.t.j.}.|.}.d.}
+00007390: 0774 057c 0283 0164 036b 0372 4474 0664  .t.|...d.k.rDt.d
+000073a0: 0474 0774 057c 0283 0183 0117 0064 0517  .t.t.|.......d..
+000073b0: 0083 0182 016e 487c 0364 066b 0272 527c  .....nH|.d.k.rR|
+000073c0: 027d 086e 3a74 057c 0383 0164 076b 0372  .}.n:t.|...d.k.r
+000073d0: 7674 0664 0874 0774 057c 0383 0183 0117  vt.d.t.t.|......
+000073e0: 0064 0917 0083 0182 017c 0274 0874 096a  .d.......|.t.t.j
+000073f0: 0a64 0a83 0183 0117 007c 0317 007d 0874  .d.......|...}.t
+00007400: 057c 0883 017d 097c 047c 057c 067c 077c  .|...}.|.|.|.|.|
+00007410: 0967 057c 0817 007d 0a7c 006a 0b7c 0a83  .g.|...}.|.j.|..
+00007420: 015c 037d 0b7d 0c7d 0d7c 0b7c 0c7c 0d66  .\.}.}.}.|.|.|.f
+00007430: 0353 0029 0b61 7401 0000 2053 6967 6e20  .S.).at... Sign 
+00007440: 7468 6520 7472 616e 7361 6374 696f 6e20  the transaction 
+00007450: 696e 2074 6865 2064 6576 6963 650a 2020  in the device.  
+00007460: 2020 2020 2020 0a20 2020 2020 2020 2050        .        P
+00007470: 6172 616d 6574 6572 733a 200a 2020 2020  arameters: .    
+00007480: 2020 2020 6b65 796e 6272 2028 696e 7429      keynbr (int)
+00007490: 3a20 7468 6520 6b65 7920 746f 2075 7365  : the key to use
+000074a0: 2028 3078 4646 2066 6f72 2062 6970 3332   (0xFF for bip32
+000074b0: 206b 6579 290a 2020 2020 2020 2020 7478   key).        tx
+000074c0: 6861 7368 2028 6c69 7374 293a 2074 6865  hash (list): the
+000074d0: 2074 7261 6e73 6163 7469 6f6e 2068 6173   transaction has
+000074e0: 6820 6173 2072 6574 7572 6e65 6420 6279  h as returned by
+000074f0: 2074 6865 2064 6576 6963 650a 2020 2020   the device.    
+00007500: 2020 2020 6368 616c 7265 7370 6f6e 7365      chalresponse
+00007510: 2028 6c69 7374 293a 2074 6865 2068 6d61   (list): the hma
+00007520: 6320 636f 6465 2069 6620 3246 4120 6973  c code if 2FA is
+00007530: 2065 6e61 626c 6564 0a20 2020 2020 2020   enabled.       
+00007540: 200a 2020 2020 2020 2020 5265 7475 726e   .        Return
+00007550: 733a 200a 2020 2020 2020 2020 2872 6573  s: .        (res
+00007560: 706f 6e73 652c 2073 7731 2c20 7377 3229  ponse, sw1, sw2)
+00007570: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00007580: 6520 286c 6973 7429 3a20 7468 6520 7369  e (list): the si
+00007590: 676e 6174 7572 6520 696e 2044 4552 2066  gnature in DER f
+000075a0: 6f72 6d61 740a 2020 2020 2020 2020 7a18  ormat.        z.
+000075b0: 496e 2063 6172 645f 7369 676e 5f74 7261  In card_sign_tra
+000075c0: 6e73 6163 7469 6f6e 7201 0000 0072 0f01  nsactionr....r..
+000075d0: 0000 7a15 5772 6f6e 6720 7478 6861 7368  ..z.Wrong txhash
+000075e0: 206c 656e 6774 683a 207a 0e28 7368 6f75   length: z.(shou
+000075f0: 6c64 2062 6520 3332 294e 7209 0100 007a  ld be 32)Nr....z
+00007600: 2057 726f 6e67 2043 6861 6c6c 656e 6765   Wrong Challenge
+00007610: 2072 6573 706f 6e73 6520 6c65 6e67 7468   response length
+00007620: 3a7a 0e28 7368 6f75 6c64 2062 6520 3230  :z.(should be 20
+00007630: 29da 0438 3030 3029 0c72 2700 0000 7234  )..8000).r'...r4
+00007640: 0000 0072 2b00 0000 72be 0000 005a 1449  ...r+...r....Z.I
+00007650: 4e53 5f53 4947 4e5f 5452 414e 5341 4354  NS_SIGN_TRANSACT
+00007660: 494f 4e72 3500 0000 da0a 5661 6c75 6545  IONr5.....ValueE
+00007670: 7272 6f72 7276 0000 0072 c800 0000 724b  rrorrv...r....rK
+00007680: 0000 0072 e100 0000 729b 0000 0029 0e72  ...r....r....).r
+00007690: 3600 0000 7222 0100 00da 0674 7868 6173  6...r".....txhas
+000076a0: 68da 0c63 6861 6c72 6573 706f 6e73 6572  h..chalresponser
+000076b0: a100 0000 7289 0000 0072 a200 0000 72a3  ....r....r....r.
+000076c0: 0000 0072 cb00 0000 72cc 0000 0072 9a00  ...r....r....r..
+000076d0: 0000 7222 0000 0072 5e00 0000 725f 0000  ..r"...r^...r_..
+000076e0: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
+000076f0: da15 6361 7264 5f73 6967 6e5f 7472 616e  ..card_sign_tran
+00007700: 7361 6374 696f 6ef5 0300 0073 2000 0000  saction....s ...
+00007710: 000c 0a03 0601 0601 0401 0402 0c01 1a01  ................
+00007720: 0801 0602 0c01 1801 1601 0801 1203 1001  ................
+00007730: 7a23 4361 7264 436f 6e6e 6563 746f 722e  z#CardConnector.
+00007740: 6361 7264 5f73 6967 6e5f 7472 616e 7361  card_sign_transa
+00007750: 6374 696f 6e63 0400 0000 0000 0000 0e00  ctionc..........
+00007760: 0000 0500 0000 4300 0000 73be 0000 0074  ......C...s....t
+00007770: 006a 0164 0183 0101 0074 026a 037d 0464  .j.d.....t.j.}.d
+00007780: 027d 057c 017d 0664 037d 0774 047c 0283  .}.|.}.d.}.t.|..
+00007790: 0164 046b 0372 4274 0564 0574 0674 047c  .d.k.rBt.d.t.t.|
+000077a0: 0283 0183 0117 0064 0617 0083 0182 016e  .......d.......n
+000077b0: 487c 0364 076b 0272 507c 027d 086e 3a74  H|.d.k.rP|.}.n:t
+000077c0: 047c 0383 0164 086b 0372 7474 0564 0974  .|...d.k.rtt.d.t
+000077d0: 0674 047c 0383 0183 0117 0064 0a17 0083  .t.|.......d....
+000077e0: 0182 017c 0274 0774 086a 0964 0b83 0183  ...|.t.t.j.d....
+000077f0: 0117 007c 0317 007d 0874 047c 0883 017d  ...|...}.t.|...}
+00007800: 097c 047c 057c 067c 077c 0967 057c 0817  .|.|.|.|.|.g.|..
+00007810: 007d 0a7c 006a 0a7c 0a83 015c 037d 0b7d  .}.|.j.|...\.}.}
+00007820: 0c7d 0d7c 0b7c 0c7c 0d66 0353 0029 0c61  .}.|.|.|.f.S.).a
+00007830: 6001 0000 2053 6967 6e20 7468 6520 7472  `... Sign the tr
+00007840: 616e 7361 6374 696f 6e20 6861 7368 2069  ansaction hash i
+00007850: 6e20 7468 6520 6465 7669 6365 0a20 2020  n the device.   
+00007860: 2020 2020 200a 2020 2020 2020 2020 5061       .        Pa
+00007870: 7261 6d65 7465 7273 3a20 0a20 2020 2020  rameters: .     
+00007880: 2020 206b 6579 6e62 7220 2869 6e74 293a     keynbr (int):
+00007890: 2074 6865 206b 6579 2074 6f20 7573 6520   the key to use 
+000078a0: 2830 7846 4620 666f 7220 6269 7033 3220  (0xFF for bip32 
+000078b0: 6b65 7929 0a20 2020 2020 2020 2074 7868  key).        txh
+000078c0: 6173 6820 286c 6973 7429 3a20 7468 6520  ash (list): the 
+000078d0: 7472 616e 7361 6374 696f 6e20 6861 7368  transaction hash
+000078e0: 200a 2020 2020 2020 2020 6368 616c 7265   .        chalre
+000078f0: 7370 6f6e 7365 2028 6c69 7374 293a 2074  sponse (list): t
+00007900: 6865 2068 6d61 6320 636f 6465 2069 6620  he hmac code if 
+00007910: 3246 4120 6973 2065 6e61 626c 6564 0a20  2FA is enabled. 
+00007920: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00007930: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
+00007940: 2020 2872 6573 706f 6e73 652c 2073 7731    (response, sw1
+00007950: 2c20 7377 3229 0a20 2020 2020 2020 2072  , sw2).        r
+00007960: 6573 706f 6e73 6520 286c 6973 7429 3a20  esponse (list): 
+00007970: 7468 6520 7369 676e 6174 7572 6520 696e  the signature in
+00007980: 2044 4552 2066 6f72 6d61 740a 2020 2020   DER format.    
+00007990: 2020 2020 7a1d 496e 2063 6172 645f 7369      z.In card_si
+000079a0: 676e 5f74 7261 6e73 6163 7469 6f6e 5f68  gn_transaction_h
+000079b0: 6173 68e9 7a00 0000 7201 0000 0072 0f01  ash.z...r....r..
+000079c0: 0000 7a15 5772 6f6e 6720 7478 6861 7368  ..z.Wrong txhash
+000079d0: 206c 656e 6774 683a 207a 0e28 7368 6f75   length: z.(shou
+000079e0: 6c64 2062 6520 3332 294e 7209 0100 007a  ld be 32)Nr....z
+000079f0: 2057 726f 6e67 2043 6861 6c6c 656e 6765   Wrong Challenge
+00007a00: 2072 6573 706f 6e73 6520 6c65 6e67 7468   response length
+00007a10: 3a7a 0e28 7368 6f75 6c64 2062 6520 3230  :z.(should be 20
+00007a20: 2972 2b01 0000 290b 7227 0000 0072 3400  )r+...).r'...r4.
+00007a30: 0000 722b 0000 0072 be00 0000 7235 0000  ..r+...r....r5..
+00007a40: 0072 2c01 0000 7276 0000 0072 c800 0000  .r,...rv...r....
+00007a50: 724b 0000 0072 e100 0000 729b 0000 0029  rK...r....r....)
+00007a60: 0e72 3600 0000 7222 0100 0072 2d01 0000  .r6...r"...r-...
+00007a70: 722e 0100 0072 a100 0000 7289 0000 0072  r....r....r....r
+00007a80: a200 0000 72a3 0000 0072 cb00 0000 72cc  ....r....r....r.
+00007a90: 0000 0072 9a00 0000 7222 0000 0072 5e00  ...r....r"...r^.
+00007aa0: 0000 725f 0000 0072 3700 0000 7237 0000  ..r_...r7...r7..
+00007ab0: 0072 3800 0000 da1a 6361 7264 5f73 6967  .r8.....card_sig
+00007ac0: 6e5f 7472 616e 7361 6374 696f 6e5f 6861  n_transaction_ha
+00007ad0: 7368 1804 0000 7320 0000 0000 0c0a 0306  sh....s ........
+00007ae0: 0104 0104 0104 020c 011a 0108 0106 020c  ................
+00007af0: 0118 0116 0108 0112 0310 017a 2843 6172  ...........z(Car
+00007b00: 6443 6f6e 6e65 6374 6f72 2e63 6172 645f  dConnector.card_
+00007b10: 7369 676e 5f74 7261 6e73 6163 7469 6f6e  sign_transaction
+00007b20: 5f68 6173 6863 0300 0000 0000 0000 0d00  _hashc..........
+00007b30: 0000 0500 0000 4300 0000 73c2 0000 0074  ......C...s....t
+00007b40: 007c 0183 0174 016b 0872 1c74 0274 036a  .|...t.k.r.t.t.j
+00007b50: 047c 0183 0183 017d 016e 1474 007c 0183  .|.....}.n.t.|..
+00007b60: 0174 036b 0872 3074 027c 0183 017d 0174  .t.k.r0t.|...}.t
+00007b70: 056a 0664 0183 0101 0074 076a 087d 0364  .j.d.....t.j.}.d
+00007b80: 027d 0464 037d 0564 037d 0664 047d 077c  .}.d.}.d.}.d.}.|
+00007b90: 037c 047c 057c 067c 0767 057d 087c 087c  .|.|.|.|.g.}.|.|
+00007ba0: 0137 007d 0878 2a74 0974 0a64 0583 0183  .7.}.x*t.t.d....
+00007bb0: 0144 005d 1a7d 097c 087c 0264 057c 0914  .D.].}.|.|.d.|..
+00007bc0: 003f 0064 0640 0067 0137 007d 0871 7457  .?.d.@.g.7.}.qtW
+00007bd0: 007c 006a 0b7c 0883 015c 037d 0a7d 0b7d  .|.j.|...\.}.}.}
+00007be0: 0c7c 0b64 076b 0272 b87c 0c64 036b 0272  .|.d.k.r.|.d.k.r
+00007bf0: b864 087c 005f 0c7c 0a7c 0b7c 0c66 0353  .d.|._.|.|.|.f.S
+00007c00: 0029 097a e620 456e 6162 6c65 2061 6e64  .).z. Enable and
+00007c10: 2069 6d70 6f72 7420 3246 4120 696e 2074   import 2FA in t
+00007c20: 6865 2064 6576 6963 650a 2020 2020 2020  he device.      
+00007c30: 2020 0a20 2020 2020 2020 2050 6172 616d    .        Param
+00007c40: 6574 6572 733a 200a 2020 2020 2020 2020  eters: .        
+00007c50: 686d 6163 7368 6131 3630 5f6b 6579 2028  hmacsha160_key (
+00007c60: 6279 7465 7320 7c20 6c69 7374 293a 2074  bytes | list): t
+00007c70: 6865 2032 302d 6279 7465 7320 7365 6372  he 20-bytes secr
+00007c80: 6574 0a20 2020 2020 2020 2061 6d6f 756e  et.        amoun
+00007c90: 745f 6c69 6d69 7420 2869 6e74 293a 2074  t_limit (int): t
+00007ca0: 6865 2061 6d6f 756e 7420 0a20 2020 2020  he amount .     
+00007cb0: 2020 200a 2020 2020 2020 2020 5265 7475     .        Retu
+00007cc0: 726e 733a 200a 2020 2020 2020 2020 2872  rns: .        (r
+00007cd0: 6573 706f 6e73 652c 2073 7731 2c20 7377  esponse, sw1, sw
+00007ce0: 3229 0a20 2020 2020 2020 207a 1349 6e20  2).        z.In 
+00007cf0: 6361 7264 5f73 6574 5f32 4641 5f6b 6579  card_set_2FA_key
+00007d00: e979 0000 0072 0100 0000 e91c 0000 0072  .y...r.........r
+00007d10: b400 0000 72d5 0000 0072 4100 0000 5429  ....r....rA...T)
+00007d20: 0d72 2600 0000 7276 0000 0072 c800 0000  .r&...rv...r....
+00007d30: 724b 0000 0072 e100 0000 7227 0000 0072  rK...r....r'...r
+00007d40: 3400 0000 722b 0000 0072 be00 0000 72d6  4...r+...r....r.
+00007d50: 0000 0072 d700 0000 729b 0000 0072 7800  ...r....r....rx.
+00007d60: 0000 290d 7236 0000 0072 db00 0000 72dc  ..).r6...r....r.
+00007d70: 0000 0072 a100 0000 7289 0000 0072 a200  ...r....r....r..
+00007d80: 0000 72a3 0000 0072 cc00 0000 729a 0000  ..r....r....r...
+00007d90: 0072 dd00 0000 7222 0000 0072 5e00 0000  .r....r"...r^...
+00007da0: 725f 0000 0072 3700 0000 7237 0000 0072  r_...r7...r7...r
+00007db0: 3800 0000 da10 6361 7264 5f73 6574 5f32  8.....card_set_2
+00007dc0: 4641 5f6b 6579 3f04 0000 7324 0000 0000  FA_key?...s$....
+00007dd0: 0a0c 0110 010c 0108 020a 0106 0104 0104  ................
+00007de0: 0104 0104 010e 0208 0112 011a 0310 0110  ................
+00007df0: 0106 017a 1e43 6172 6443 6f6e 6e65 6374  ...z.CardConnect
+00007e00: 6f72 2e63 6172 645f 7365 745f 3246 415f  or.card_set_2FA_
+00007e10: 6b65 7963 0200 0000 0000 0000 0b00 0000  keyc............
+00007e20: 0500 0000 4300 0000 7396 0000 0074 006a  ....C...s....t.j
+00007e30: 0164 0183 0101 0074 027c 0183 0174 036b  .d.....t.|...t.k
+00007e40: 0872 2674 0474 056a 067c 0183 0183 017d  .r&t.t.j.|.....}
+00007e50: 016e 1474 027c 0183 0174 056b 0872 3a74  .n.t.|...t.k.r:t
+00007e60: 047c 0183 017d 0174 076a 087d 0264 027d  .|...}.t.j.}.d.}
+00007e70: 0364 037d 0464 037d 0564 047d 067c 027c  .d.}.d.}.d.}.|.|
+00007e80: 037c 047c 057c 0667 057d 077c 077c 0137  .|.|.|.g.}.|.|.7
+00007e90: 007d 077c 006a 097c 0783 015c 037d 087d  .}.|.j.|...\.}.}
+00007ea0: 097d 0a7c 0964 056b 0272 8c7c 0a64 036b  .}.|.d.k.r.|.d.k
+00007eb0: 0272 8c64 067c 005f 0a7c 087c 097c 0a66  .r.d.|._.|.|.|.f
+00007ec0: 0353 0029 077a b820 4469 7361 626c 6520  .S.).z. Disable 
+00007ed0: 3246 412e 0a20 2020 2020 2020 200a 2020  2FA..        .  
+00007ee0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00007ef0: 3a20 0a20 2020 2020 2020 2063 6861 6c72  : .        chalr
+00007f00: 6573 706f 6e73 6520 286c 6973 7420 7c20  esponse (list | 
+00007f10: 6279 7465 7320 7c20 6865 785f 7374 7229  bytes | hex_str)
+00007f20: 3a20 7468 6520 3230 2d62 7974 6573 2063  : the 20-bytes c
+00007f30: 6f64 6520 746f 2063 6f6e 6669 726d 0a20  ode to confirm. 
+00007f40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00007f50: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
+00007f60: 2020 2872 6573 706f 6e73 652c 2073 7731    (response, sw1
+00007f70: 2c20 7377 3229 0a20 2020 2020 2020 207a  , sw2).        z
+00007f80: 1549 6e20 6361 7264 5f72 6573 6574 5f32  .In card_reset_2
+00007f90: 4641 5f6b 6579 e978 0000 0072 0100 0000  FA_key.x...r....
+00007fa0: 7209 0100 0072 4100 0000 4629 0b72 2700  r....rA...F).r'.
+00007fb0: 0000 7234 0000 0072 2600 0000 7276 0000  ..r4...r&...rv..
+00007fc0: 0072 c800 0000 724b 0000 0072 e100 0000  .r....rK...r....
+00007fd0: 722b 0000 0072 be00 0000 729b 0000 0072  r+...r....r....r
+00007fe0: 7800 0000 290b 7236 0000 0072 2e01 0000  x...).r6...r....
+00007ff0: 72a1 0000 0072 8900 0000 72a2 0000 0072  r....r....r....r
+00008000: a300 0000 72cc 0000 0072 9a00 0000 7222  ....r....r....r"
+00008010: 0000 0072 5e00 0000 725f 0000 0072 3700  ...r^...r_...r7.
+00008020: 0000 7237 0000 0072 3800 0000 da12 6361  ..r7...r8.....ca
+00008030: 7264 5f72 6573 6574 5f32 4641 5f6b 6579  rd_reset_2FA_key
+00008040: 6004 0000 7320 0000 0000 090a 010c 0110  `...s ..........
+00008050: 010c 0108 0206 0104 0104 0104 0104 010e  ................
+00008060: 0108 0310 0110 0106 017a 2043 6172 6443  .........z CardC
+00008070: 6f6e 6e65 6374 6f72 2e63 6172 645f 7265  onnector.card_re
+00008080: 7365 745f 3246 415f 6b65 7954 6303 0000  set_2FA_keyTc...
+00008090: 0000 0000 0018 0000 0005 0000 0043 0000  .............C..
+000080a0: 0073 7803 0000 7400 6a01 6401 8301 0100  .sx...t.j.d.....
+000080b0: 7402 7c01 8301 7403 6b02 7220 7c01 6a04  t.|...t.k.r |.j.
+000080c0: 6402 8301 7d01 7405 7c01 8301 7d01 6700  d...}.t.|...}.g.
+000080d0: 7d03 7406 6a07 7d04 6403 7d05 7406 6a08  }.t.j.}.d.}.t.j.
+000080e0: 7d06 6404 7d07 7c02 9001 7222 6405 7d08  }.d.}.|...r"d.}.
+000080f0: 6406 7d09 7c04 7c05 7c08 7c06 7c09 6705  d.}.|.|.|.|.|.g.
+00008100: 7d0a 7409 7c01 8301 7d0b 7c07 7c0b 7c07  }.t.|...}.|.|.|.
+00008110: 1600 1800 7d0c 7c01 7c0c 6701 7c0c 1400  ....}.|.|.g.|...
+00008120: 1700 7d01 7c00 6a0a 7c0a 8301 5c03 7d0d  ..}.|.j.|...\.}.
+00008130: 7d0e 7d0f 7c0e 6407 6b02 72d8 7c0f 6406  }.}.|.d.k.r.|.d.
+00008140: 6b02 72d8 7c0d 6406 6404 8502 1900 7d10  k.r.|.d.d.....}.
+00008150: 7c0d 6404 6408 8502 1900 7d11 7c10 7d03  |.d.d.....}.|.}.
+00008160: 6406 6409 6c0b 6d0c 7d12 0100 7c12 740d  d.d.l.m.}...|.t.
+00008170: 7c11 8301 8301 6a0e 8300 7d11 6e48 7c0e  |.....j...}.nH|.
+00008180: 640a 6b02 6fe6 7c0f 640b 6b02 9001 7206  d.k.o.|.d.k...r.
+00008190: 740f 640c 7410 640d 7c0e 1400 7c0f 1700  t.d.t.d.|...|...
+000081a0: 8301 9b00 9d02 8301 8201 6e1a 7411 640e  ..........n.t.d.
+000081b0: 7410 640d 7c0e 1400 7c0f 1700 8301 9b00  t.d.|...|.......
+000081c0: 9d02 8301 8201 6ec2 640f 7d08 6404 7d09  ......n.d.}.d.}.
+000081d0: 7c04 7c05 7c08 7c06 7c09 6705 7d0a 7c01  |.|.|.|.|.g.}.|.
+000081e0: 6406 6404 8502 1900 7d10 7c01 6404 6400  d.d.....}.|.d.d.
+000081f0: 8502 1900 7d01 7c0a 7c10 1700 7d0a 7409  ....}.|.|...}.t.
+00008200: 7c01 8301 7c07 1600 6406 6b03 9001 7274  |...|...d.k...rt
+00008210: 7400 6a12 6410 8301 0100 7c00 6a0a 7c0a  t.j.d.....|.j.|.
+00008220: 8301 5c03 7d0d 7d0e 7d0f 7c0e 6407 6b02  ..\.}.}.}.|.d.k.
+00008230: 9001 729a 7c0f 6406 6b02 9001 729a 6e4a  ..r.|.d.k...r.nJ
+00008240: 7c0e 640a 6b02 9001 72ca 7c0f 640b 6b02  |.d.k...r.|.d.k.
+00008250: 9001 72ca 740f 640c 7410 640d 7c0e 1400  ..r.t.d.t.d.|...
+00008260: 7c0f 1700 8301 9b00 9d02 8301 8201 6e1a  |.............n.
+00008270: 7411 640e 7410 640d 7c0e 1400 7c0f 1700  t.d.t.d.|...|...
+00008280: 8301 9b00 9d02 8301 8201 6411 7d13 6406  ..........d.}.d.
+00008290: 7d14 7409 7c01 8301 7d15 78a0 7c15 7c13  }.t.|...}.x.|.|.
+000082a0: 6b04 9002 7294 7406 6a13 7d06 6405 7c13  k...r.t.j.}.d.|.
+000082b0: 1700 7d09 7c04 7c05 7c08 7c06 7c09 6705  ..}.|.|.|.|.|.g.
+000082c0: 7d0a 7c0a 7c13 6412 3f00 6413 4000 7c13  }.|.|.d.?.d.@.|.
+000082d0: 6413 4000 6702 3700 7d0a 7c0a 7c01 7c14  d.@.g.7.}.|.|.|.
+000082e0: 7c14 7c13 1700 8502 1900 3700 7d0a 7c14  |.|.......7.}.|.
+000082f0: 7c13 3700 7d14 7c15 7c13 3800 7d15 7c00  |.7.}.|.|.8.}.|.
+00008300: 6a0a 7c0a 8301 5c03 7d0d 7d0e 7d0f 7c0d  j.|...\.}.}.}.|.
+00008310: 6406 1900 6412 3e00 7c0d 640f 1900 1700  d...d.>.|.d.....
+00008320: 7d16 7c03 7c0d 6405 6405 7c16 1700 8502  }.|.|.d.d.|.....
+00008330: 1900 3700 7d03 9001 71f6 5700 7c15 7d13  ..7.}...q.W.|.}.
+00008340: 7406 6a14 7d06 6405 7c13 1700 7d09 7c04  t.j.}.d.|...}.|.
+00008350: 7c05 7c08 7c06 7c09 6705 7d0a 7c0a 7c13  |.|.|.|.g.}.|.|.
+00008360: 6412 3f00 6413 4000 7c13 6413 4000 6702  d.?.d.@.|.d.@.g.
+00008370: 3700 7d0a 7c0a 7c01 7c14 7c14 7c13 1700  7.}.|.|.|.|.|...
+00008380: 8502 1900 3700 7d0a 7c14 7c13 3700 7d14  ....7.}.|.|.7.}.
+00008390: 7c15 7c13 3800 7d15 7c00 6a0a 7c0a 8301  |.|.8.}.|.j.|...
+000083a0: 5c03 7d0d 7d0e 7d0f 7c0d 6406 1900 6412  \.}.}.}.|.d...d.
+000083b0: 3e00 7c0d 640f 1900 1700 7d16 7c03 7c0d  >.|.d.....}.|.|.
+000083c0: 6405 6405 7c16 1700 8502 1900 3700 7d03  d.d.|.......7.}.
+000083d0: 7c02 9003 724c 7415 6a16 740d 7c03 8301  |...rLt.j.t.|...
+000083e0: 8301 6a17 6414 8301 7d03 7c11 7c03 6602  ..j.d...}.|.|.f.
+000083f0: 5300 7c03 6416 1900 7d17 7c03 6406 7c17  S.|.d...}.|.d.|.
+00008400: 0b00 8502 1900 7d03 740d 7c03 8301 6a17  ......}.t.|...j.
+00008410: 6415 8301 7d03 7c03 5300 6400 5300 2917  d...}.|.S.d.S.).
+00008420: 4e7a 1d49 6e20 6361 7264 5f63 7279 7074  Nz.In card_crypt
+00008430: 5f74 7261 6e73 6163 7469 6f6e 5f32 4641  _transaction_2FA
+00008440: 72c1 0000 00e9 7600 0000 728a 0000 0072  r.....v...r....r
+00008450: 2300 0000 7201 0000 0072 4100 0000 e924  #...r....rA....$
+00008460: 0000 0029 01da 0673 6861 3235 3672 4200  ...)...sha256rB.
+00008470: 0000 e919 0000 007a 2745 7272 6f72 3a20  .......z'Error: 
+00008480: 3246 4120 6973 206e 6f74 2065 6e61 626c  2FA is not enabl
+00008490: 6564 2028 6572 726f 7220 636f 6465 3a20  ed (error code: 
+000084a0: 72bc 0000 007a 1755 6e65 7870 6563 7465  r....z.Unexpecte
+000084b0: 6420 6572 726f 7220 636f 6465 3a20 720c  d error code: r.
+000084c0: 0000 007a 0e50 6164 6469 6e67 2065 7272  ...z.Padding err
+000084d0: 6f72 2172 9d00 0000 72b4 0000 0072 d500  or!r....r....r..
+000084e0: 0000 da05 6173 6369 697a 076c 6174 696e  ....asciiz.latin
+000084f0: 2d31 e9ff ffff ff29 1872 2700 0000 7234  -1.....).r'...r4
+00008500: 0000 0072 2600 0000 7276 0000 0072 c900  ...r&...rv...r..
+00008510: 0000 72c8 0000 0072 2b00 0000 72be 0000  ..r....r+...r...
+00008520: 0072 1f01 0000 7235 0000 0072 9b00 0000  .r....r5...r....
+00008530: 724f 0000 0072 3901 0000 724b 0000 0072  rO...r9...rK...r
+00008540: 5100 0000 72fc 0000 0072 4c00 0000 72f4  Q...r....rL...r.
+00008550: 0000 0072 2800 0000 7220 0100 0072 2101  ...r(...r ...r!.
+00008560: 0000 da06 6261 7365 3634 5a09 6236 3465  ....base64Z.b64e
+00008570: 6e63 6f64 6572 c200 0000 2918 7236 0000  ncoder....).r6..
+00008580: 0072 6200 0000 5a0a 6973 5f65 6e63 7279  .rb...Z.is_encry
+00008590: 7074 5a07 6d73 675f 6f75 7472 a100 0000  ptZ.msg_outr....
+000085a0: 7289 0000 0072 a300 0000 5a09 626c 6f63  r....r....Z.bloc
+000085b0: 6b73 697a 6572 a200 0000 72cc 0000 0072  ksizer....r....r
+000085c0: 9a00 0000 da04 7369 7a65 5a07 7061 6473  ......sizeZ.pads
+000085d0: 697a 6572 2200 0000 725e 0000 0072 5f00  izer"...r^...r_.
+000085e0: 0000 5a02 4956 5a06 6964 5f32 4641 7239  ..Z.IVZ.id_2FAr9
+000085f0: 0100 0072 2401 0000 7225 0100 0072 2601  ...r$...r%...r&.
+00008600: 0000 5a08 6f75 745f 7369 7a65 5a03 7061  ..Z.out_sizeZ.pa
+00008610: 6472 3700 0000 7237 0000 0072 3800 0000  dr7...r7...r8...
+00008620: da1a 6361 7264 5f63 7279 7074 5f74 7261  ..card_crypt_tra
+00008630: 6e73 6163 7469 6f6e 5f32 4641 7d04 0000  nsaction_2FA}...
+00008640: 7390 0000 0000 010a 010c 010a 0108 0104  s...............
+00008650: 0306 0104 0106 0104 0106 0104 0104 010e  ................
+00008660: 0208 010c 010e 0210 0110 020c 010c 0104  ................
+00008670: 020c 0112 0112 011c 021c 0204 0104 010e  ................
+00008680: 020c 010c 0108 0112 010a 0210 0114 0102  ................
+00008690: 0114 011c 021a 0704 0104 0108 020c 0106  ................
+000086a0: 0108 010e 0118 0114 0108 0108 0210 0214  ................
+000086b0: 011a 0304 0106 0108 010e 0118 0114 0108  ................
+000086c0: 0108 0210 0214 0114 0206 0214 0108 0308  ................
+000086d0: 010e 010e 017a 2843 6172 6443 6f6e 6e65  .....z(CardConne
+000086e0: 6374 6f72 2e63 6172 645f 6372 7970 745f  ctor.card_crypt_
+000086f0: 7472 616e 7361 6374 696f 6e5f 3246 4163  transaction_2FAc
+00008700: 0500 0000 0000 0000 0e00 0000 0500 0000  ................
+00008710: 4300 0000 737a 0000 0074 006a 0164 0183  C...sz...t.j.d..
+00008720: 0101 0074 026a 037d 0574 026a 047d 067c  ...t.j.}.t.j.}.|
+00008730: 017d 077c 027d 0864 0274 057c 0383 0117  .}.|.}.d.t.|....
+00008740: 0064 0217 0074 057c 0483 0117 007d 097c  .d...t.|.....}.|
+00008750: 057c 067c 077c 087c 0967 0574 057c 0383  .|.|.|.|.g.t.|..
+00008760: 0167 0117 007c 0317 0074 057c 0483 0167  .g...|...t.|...g
+00008770: 0117 007c 0417 007d 0a7c 006a 067c 0a83  ...|...}.|.j.|..
+00008780: 015c 037d 0b7d 0c7d 0d7c 0b7c 0c7c 0d66  .\.}.}.}.|.|.|.f
+00008790: 0353 0029 034e 7a12 496e 2063 6172 645f  .S.).Nz.In card_
+000087a0: 6372 6561 7465 5f50 494e 720c 0000 0029  create_PINr....)
+000087b0: 0772 2700 0000 7234 0000 0072 2b00 0000  .r'...r4...r+...
+000087c0: 72be 0000 0072 3000 0000 7235 0000 0072  r....r0...r5...r
+000087d0: 9b00 0000 290e 7236 0000 0072 7c00 0000  ....).r6...r|...
+000087e0: 5a09 7069 6e5f 7472 6965 7372 7d00 0000  Z.pin_triesr}...
+000087f0: da04 7562 6c6b 72a1 0000 0072 8900 0000  ..ublkr....r....
+00008800: 72a2 0000 0072 a300 0000 72cc 0000 0072  r....r....r....r
+00008810: 9a00 0000 7222 0000 0072 5e00 0000 725f  ....r"...r^...r_
+00008820: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
+00008830: 0000 da0f 6361 7264 5f63 7265 6174 655f  ....card_create_
+00008840: 5049 4ee7 0400 0073 1200 0000 0001 0a01  PIN....s........
+00008850: 0601 0601 0401 0401 1801 2a03 1001 7a1d  ..........*...z.
+00008860: 4361 7264 436f 6e6e 6563 746f 722e 6361  CardConnector.ca
+00008870: 7264 5f63 7265 6174 655f 5049 4e63 0300  rd_create_PINc..
+00008880: 0000 0000 0000 0c00 0000 0500 0000 4300  ..............C.
+00008890: 0000 7352 0000 0074 006a 0164 0183 0101  ..sR...t.j.d....
+000088a0: 0074 026a 037d 0374 026a 047d 047c 017d  .t.j.}.t.j.}.|.}
+000088b0: 0564 027d 0674 057c 0283 017d 077c 037c  .d.}.t.|...}.|.|
+000088c0: 047c 057c 067c 0767 057c 0217 007d 087c  .|.|.|.g.|...}.|
+000088d0: 006a 067c 0883 015c 037d 097d 0a7d 0b7c  .j.|...\.}.}.}.|
+000088e0: 097c 0a7c 0b66 0353 0029 034e 7a1d 496e  .|.|.f.S.).Nz.In
+000088f0: 2063 6172 645f 7665 7269 6679 5f50 494e   card_verify_PIN
+00008900: 5f64 6570 7265 6361 7465 6472 0100 0000  _deprecatedr....
+00008910: 2907 7227 0000 0072 3400 0000 722b 0000  ).r'...r4...r+..
+00008920: 0072 be00 0000 7231 0000 0072 3500 0000  .r....r1...r5...
+00008930: 729b 0000 0029 0c72 3600 0000 727c 0000  r....).r6...r|..
+00008940: 0072 7d00 0000 72a1 0000 0072 8900 0000  .r}...r....r....
+00008950: 72a2 0000 0072 a300 0000 72cc 0000 0072  r....r....r....r
+00008960: 9a00 0000 7222 0000 0072 5e00 0000 725f  ....r"...r^...r_
+00008970: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
+00008980: 0000 da1a 6361 7264 5f76 6572 6966 795f  ....card_verify_
+00008990: 5049 4e5f 6465 7072 6563 6174 6564 f504  PIN_deprecated..
+000089a0: 0000 7312 0000 0000 010a 0106 0106 0104  ..s.............
+000089b0: 0104 0108 0112 0210 017a 2843 6172 6443  .........z(CardC
+000089c0: 6f6e 6e65 6374 6f72 2e63 6172 645f 7665  onnector.card_ve
+000089d0: 7269 6679 5f50 494e 5f64 6570 7265 6361  rify_PIN_depreca
+000089e0: 7465 6463 0100 0000 0000 0000 0f00 0000  tedc............
+000089f0: 0600 0000 4300 0000 734e 0200 0074 006a  ....C...sN...t.j
+00008a00: 0164 0183 0101 0090 0278 187c 006a 0290  .d.......x.|.j..
+00008a10: 0272 247c 006a 0364 006b 0872 6664 027d  .r$|.j.d.k.rfd.}
+00008a20: 017c 006a 0464 006b 0972 4c64 037c 006a  .|.j.d.k.rLd.|.j
+00008a30: 059b 0064 049d 037d 027c 006a 046a 067c  ...d...}.|.j.j.|
+00008a40: 0283 015c 027d 017d 037c 0164 026b 0872  ...\.}.}.|.d.k.r
+00008a50: 5c74 0764 0583 0182 0174 087c 0383 017d  \t.d.....t.|...}
+00008a60: 036e 067c 006a 037d 0374 096a 0a7d 0474  .n.|.j.}.t.j.}.t
+00008a70: 096a 0b7d 057c 047c 0564 0664 0674 0c7c  .j.}.|.|.d.d.t.|
+00008a80: 0383 0167 057c 0317 007d 067c 006a 0d72  ...g.|...}.|.j.r
+00008a90: 9e7c 006a 0e7c 0683 017d 067c 006a 0f6a  .|.j.|...}.|.j.j
+00008aa0: 106a 117c 0683 015c 037d 077d 087d 097c  .j.|...\.}.}.}.|
+00008ab0: 0864 076b 0272 d87c 0964 066b 0272 d87c  .d.k.r.|.d.k.r.|
+00008ac0: 006a 1264 067c 0383 0201 007c 077c 087c  .j.d.|.....|.|.|
+00008ad0: 0966 0353 007c 0864 086b 026f ea7c 0964  .f.S.|.d.k.o.|.d
+00008ae0: 0940 0064 096b 0290 0172 287c 006a 1264  .@.d.k...r(|.j.d
+00008af0: 0664 0083 0201 007c 0964 1640 007d 0a64  .d.....|.d.@.}.d
+00008b00: 0a6a 137c 0a83 017d 027c 006a 0464 006b  .j.|...}.|.j.d.k
+00008b10: 0990 0272 227c 006a 046a 1464 0b7c 0283  ...r"|.j.j.d.|..
+00008b20: 0201 0071 0e7c 0864 0c6b 0290 0172 8a7c  ...q.|.d.k...r.|
+00008b30: 0964 0d6b 0290 0172 8a7c 006a 1264 0664  .d.k...r.|.j.d.d
+00008b40: 0083 0201 007c 006a 1583 005c 047d 0b7d  .....|.j...\.}.}
+00008b50: 0c7d 0d7d 0e7c 0e6a 1664 0e64 1783 027d  .}.}.|.j.d.d...}
+00008b60: 0a64 0a6a 137c 0a83 017d 027c 006a 0464  .d.j.|...}.|.j.d
+00008b70: 006b 0990 0272 227c 006a 046a 1464 0b7c  .k...r"|.j.j.d.|
+00008b80: 0283 0201 0071 0e7c 0864 0c6b 0290 0172  .....q.|.d.k...r
+00008b90: da7c 0964 106b 0290 0172 da64 1174 1764  .|.d.k...r.d.t.d
+00008ba0: 127c 0814 007c 0917 0083 019b 0064 139d  .|...|.......d..
+00008bb0: 037d 027c 006a 0464 006b 0990 0172 d07c  .}.|.j.d.k...r.|
+00008bc0: 006a 046a 1464 0b7c 0283 0201 0074 077c  .j.j.d.|.....t.|
+00008bd0: 0283 0182 0171 0e7c 006a 1264 0664 0083  .....q.|.j.d.d..
+00008be0: 0201 0064 1474 1764 127c 0814 007c 0917  ...d.t.d.|...|..
+00008bf0: 0083 019b 0064 139d 037d 027c 006a 0464  .....d...}.|.j.d
+00008c00: 006b 0990 0272 187c 006a 046a 1464 0b7c  .k...r.|.j.j.d.|
+00008c10: 0283 0201 007c 077c 087c 0966 0353 0071  .....|.|.|.f.S.q
+00008c20: 0e57 007c 006a 0464 006b 0990 0272 427c  .W.|.j.d.k...rB|
+00008c30: 006a 046a 1464 0b64 1583 0201 006e 0874  .j.j.d.d.....n.t
+00008c40: 0764 1583 0182 0164 0053 0029 184e 7a12  .d.....d.S.).Nz.
+00008c50: 496e 2063 6172 645f 7665 7269 6679 5f50  In card_verify_P
+00008c60: 494e 467a 1745 6e74 6572 2074 6865 2050  INFz.Enter the P
+00008c70: 494e 2066 6f72 2079 6f75 7220 fa01 3a7a  IN for your ..:z
+00008c80: 2b44 6576 6963 6520 6361 6e6e 6f74 2062  +Device cannot b
+00008c90: 6520 756e 6c6f 636b 6564 2077 6974 686f  e unlocked witho
+00008ca0: 7574 2050 494e 2063 6f64 6521 7201 0000  ut PIN code!r...
+00008cb0: 0072 4100 0000 72d1 0000 00e9 c000 0000  .rA...r.........
+00008cc0: 7a1e 5772 6f6e 6720 5049 4e21 207b 7d20  z.Wrong PIN! {} 
+00008cd0: 7472 6965 7320 7265 6d61 696e 696e 6721  tries remaining!
+00008ce0: 7245 0000 0072 4200 0000 7223 0000 0072  rE...rB...r#...r
+00008cf0: b500 0000 720c 0000 0072 bb00 0000 7a6b  ....r....r....zk
+00008d00: 546f 6f20 6d61 6e79 2066 6169 6c65 6420  Too many failed 
+00008d10: 6174 7465 6d70 7473 2120 596f 7572 2064  attempts! Your d
+00008d20: 6576 6963 6520 6861 7320 6265 656e 2062  evice has been b
+00008d30: 6c6f 636b 6564 2120 0a0a 596f 7520 6e65  locked! ..You ne
+00008d40: 6564 2079 6f75 7220 5055 4b20 636f 6465  ed your PUK code
+00008d50: 2074 6f20 756e 626c 6f63 6b20 6974 2028   to unblock it (
+00008d60: 6572 726f 7220 636f 6465 2072 bc00 0000  error code r....
+00008d70: 72bd 0000 007a 3550 6c65 6173 6520 6368  r....z5Please ch
+00008d80: 6563 6b20 796f 7572 2063 6172 6421 2055  eck your card! U
+00008d90: 6e65 7870 6563 7465 6420 6572 726f 7220  nexpected error 
+00008da0: 2865 7272 6f72 2063 6f64 6520 7a22 4e6f  (error code z"No
+00008db0: 2063 6172 6420 666f 756e 6421 2050 6c65   card found! Ple
+00008dc0: 6173 6520 696e 7365 7274 2063 6172 6421  ase insert card!
+00008dd0: 693f ffff ff72 3c01 0000 2918 7227 0000  i?...r<...).r'..
+00008de0: 0072 3400 0000 7246 0000 0072 7d00 0000  .r4...rF...r}...
+00008df0: 725a 0000 0072 8300 0000 5a0a 5049 4e5f  rZ...r....Z.PIN_
+00008e00: 6469 616c 6f67 72fc 0000 0072 c800 0000  dialogr....r....
+00008e10: 722b 0000 0072 be00 0000 7231 0000 0072  r+...r....r1...r
+00008e20: 3500 0000 7258 0000 0072 8f00 0000 7247  5...rX...r....rG
+00008e30: 0000 0072 4800 0000 7290 0000 0072 d800  ...rH...r....r..
+00008e40: 0000 da06 666f 726d 6174 725b 0000 0072  ....formatr[...r
+00008e50: 5700 0000 da03 6765 7472 4c00 0000 290f  W.....getrL...).
+00008e60: 7236 0000 005a 0669 735f 5049 4e72 6200  r6...Z.is_PINrb.
+00008e70: 0000 5a05 7069 6e5f 3072 a100 0000 7289  ..Z.pin_0r....r.
+00008e80: 0000 0072 9a00 0000 7222 0000 0072 5e00  ...r....r"...r^.
+00008e90: 0000 725f 0000 00da 0870 696e 5f6c 6566  ..r_.....pin_lef
+00008ea0: 74da 0972 6573 706f 6e73 6532 da04 7377  t..response2..sw
+00008eb0: 3162 da04 7377 3262 72bf 0000 0072 3700  1b..sw2br....r7.
+00008ec0: 0000 7237 0000 0072 3800 0000 7292 0000  ..r7...r8...r...
+00008ed0: 0001 0500 0073 5e00 0000 0001 0a02 0c01  .....s^.........
+00008ee0: 0a01 0401 0a01 0e01 1001 0801 0801 0a02  ................
+00008ef0: 0601 0601 0601 1602 0601 0a01 1403 1001  ................
+00008f00: 0c01 0a02 1601 0c01 0801 0a01 0c01 1002  ................
+00008f10: 1401 0c01 1001 0c01 0a01 0c01 1002 1401  ................
+00008f20: 1801 0c01 0e01 0a03 0c01 1801 0c01 0e01  ................
+00008f30: 0e03 0c01 1002 0801 7a1d 4361 7264 436f  ........z.CardCo
+00008f40: 6e6e 6563 746f 722e 6361 7264 5f76 6572  nnector.card_ver
+00008f50: 6966 795f 5049 4e63 0300 0000 0000 0000  ify_PINc........
+00008f60: 0300 0000 0200 0000 4300 0000 7310 0000  ........C...s...
+00008f70: 007c 017c 005f 007c 027c 005f 0164 0053  .|.|._.|.|._.d.S
+00008f80: 0029 014e 2902 727c 0000 0072 7d00 0000  .).N).r|...r}...
+00008f90: 2903 7236 0000 0072 7c00 0000 727d 0000  ).r6...r|...r}..
+00008fa0: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
+00008fb0: 72d8 0000 003f 0500 0073 0600 0000 0001  r....?...s......
+00008fc0: 0601 0601 7a15 4361 7264 436f 6e6e 6563  ....z.CardConnec
+00008fd0: 746f 722e 7365 745f 7069 6e63 0400 0000  tor.set_pinc....
+00008fe0: 0000 0000 1300 0000 0500 0000 4300 0000  ............C...
+00008ff0: 739c 0100 0074 006a 0164 0183 0101 0074  s....t.j.d.....t
+00009000: 026a 037d 0474 026a 047d 057c 017d 0664  .j.}.t.j.}.|.}.d
+00009010: 027d 0764 0374 057c 0283 0117 0064 0317  .}.d.t.|.....d..
+00009020: 0074 057c 0383 0117 007d 087c 047c 057c  .t.|.....}.|.|.|
+00009030: 067c 077c 0867 0574 057c 0283 0167 0117  .|.|.g.t.|...g..
+00009040: 007c 0217 0074 057c 0383 0167 0117 007c  .|...t.|...g...|
+00009050: 0317 007d 097c 006a 067c 0983 015c 037d  ...}.|.j.|...\.}
+00009060: 0a7d 0b7d 0c7c 0b64 046b 0272 907c 0c64  .}.}.|.d.k.r.|.d
+00009070: 026b 0272 907c 006a 077c 017c 0383 0201  .k.r.|.j.|.|....
+00009080: 0090 016e 027c 0b64 056b 0272 dc7c 0c64  ...n.|.d.k.r.|.d
+00009090: 0640 0064 066b 0272 dc7c 006a 077c 0164  .@.d.k.r.|.j.|.d
+000090a0: 0083 0201 007c 0c64 1040 007d 0d64 076a  .....|.d.@.}.d.j
+000090b0: 087c 0d83 017d 0e7c 006a 0964 006b 0972  .|...}.|.j.d.k.r
+000090c0: da7c 006a 096a 0a64 087c 0e83 0201 006e  .|.j.j.d.|.....n
+000090d0: b67c 0b64 096b 026f ea7c 0c64 0a6b 0290  .|.d.k.o.|.d.k..
+000090e0: 0172 447c 006a 077c 0164 0083 0201 007c  .rD|.j.|.d.....|
+000090f0: 006a 0b83 005c 047d 0f7d 107d 117d 127c  .j...\.}.}.}.}.|
+00009100: 126a 0c64 0b64 1183 027d 0d64 076a 087c  .j.d.d...}.d.j.|
+00009110: 0d83 017d 0e7c 006a 0964 006b 0990 0172  ...}.|.j.d.k...r
+00009120: 3a7c 006a 096a 0a64 087c 0e83 0201 0074  :|.j.j.d.|.....t
+00009130: 0d7c 0e83 0182 016e 4e7c 0b64 096b 0290  .|.....nN|.d.k..
+00009140: 0172 927c 0c64 0c6b 0290 0172 9264 0d74  .r.|.d.k...r.d.t
+00009150: 0e64 0e7c 0b14 007c 0c17 0083 019b 0064  .d.|...|.......d
+00009160: 0f9d 037d 0e7c 006a 0964 006b 0990 0172  ...}.|.j.d.k...r
+00009170: 8a7c 006a 096a 0a64 087c 0e83 0201 0074  .|.j.j.d.|.....t
+00009180: 0d7c 0e83 0182 017c 0a7c 0b7c 0c66 0353  .|.....|.|.|.f.S
+00009190: 0029 124e 7a12 496e 2063 6172 645f 6368  .).Nz.In card_ch
+000091a0: 616e 6765 5f50 494e 7201 0000 0072 0c00  ange_PINr....r..
+000091b0: 0000 7241 0000 0072 d100 0000 7244 0100  ..rA...r....rD..
+000091c0: 007a 1e57 726f 6e67 2050 494e 2120 7b7d  .z.Wrong PIN! {}
+000091d0: 2074 7269 6573 2072 656d 6169 6e69 6e67   tries remaining
+000091e0: 2172 4500 0000 7242 0000 0072 2300 0000  !rE...rB...r#...
+000091f0: 72b5 0000 0072 bb00 0000 7a6b 546f 6f20  r....r....zkToo 
+00009200: 6d61 6e79 2066 6169 6c65 6420 6174 7465  many failed atte
+00009210: 6d70 7473 2120 596f 7572 2064 6576 6963  mpts! Your devic
+00009220: 6520 6861 7320 6265 656e 2062 6c6f 636b  e has been block
+00009230: 6564 2120 0a0a 596f 7520 6e65 6564 2079  ed! ..You need y
+00009240: 6f75 7220 5055 4b20 636f 6465 2074 6f20  our PUK code to 
+00009250: 756e 626c 6f63 6b20 6974 2028 6572 726f  unblock it (erro
+00009260: 7220 636f 6465 2072 bc00 0000 72bd 0000  r code r....r...
+00009270: 0069 3fff ffff 723c 0100 0029 0f72 2700  .i?...r<...).r'.
+00009280: 0000 7234 0000 0072 2b00 0000 72be 0000  ..r4...r+...r...
+00009290: 0072 3200 0000 7235 0000 0072 9b00 0000  .r2...r5...r....
+000092a0: 72d8 0000 0072 4501 0000 725a 0000 0072  r....rE...rZ...r
+000092b0: 5b00 0000 7257 0000 0072 4601 0000 72fc  [...rW...rF...r.
+000092c0: 0000 0072 4c00 0000 2913 7236 0000 0072  ...rL...).r6...r
+000092d0: 7c00 0000 5a07 6f6c 645f 7069 6e5a 076e  |...Z.old_pinZ.n
+000092e0: 6577 5f70 696e 72a1 0000 0072 8900 0000  ew_pinr....r....
+000092f0: 72a2 0000 0072 a300 0000 72cc 0000 0072  r....r....r....r
+00009300: 9a00 0000 7222 0000 0072 5e00 0000 725f  ....r"...r^...r_
+00009310: 0000 0072 4701 0000 7262 0000 0072 4801  ...rG...rb...rH.
+00009320: 0000 7249 0100 0072 4a01 0000 72bf 0000  ..rI...rJ...r...
+00009330: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
+00009340: da0f 6361 7264 5f63 6861 6e67 655f 5049  ..card_change_PI
+00009350: 4e44 0500 0073 3c00 0000 0001 0a01 0601  ND...s<.........
+00009360: 0601 0401 0401 1801 2a02 1003 1001 1002  ........*.......
+00009370: 1401 0c01 0801 0a01 0a01 1002 1201 0c01  ................
+00009380: 1001 0c01 0a01 0c01 0e01 0a02 1401 1801  ................
+00009390: 0c01 0e01 0802 7a1d 4361 7264 436f 6e6e  ......z.CardConn
+000093a0: 6563 746f 722e 6361 7264 5f63 6861 6e67  ector.card_chang
+000093b0: 655f 5049 4e63 0300 0000 0000 0000 1200  e_PINc..........
+000093c0: 0000 0500 0000 4300 0000 7348 0100 0074  ......C...sH...t
+000093d0: 006a 0164 0183 0101 0074 026a 037d 0374  .j.d.....t.j.}.t
+000093e0: 026a 047d 047c 017d 0564 027d 0674 057c  .j.}.|.}.d.}.t.|
+000093f0: 0283 017d 077c 037c 047c 057c 067c 0767  ...}.|.|.|.|.|.g
+00009400: 057c 0217 007d 087c 006a 067c 0883 015c  .|...}.|.j.|...\
+00009410: 037d 097d 0a7d 0b7c 0a64 036b 0272 947c  .}.}.}.|.d.k.r.|
+00009420: 0b64 0440 0064 046b 0272 947c 006a 077c  .d.@.d.k.r.|.j.|
+00009430: 0164 0083 0201 007c 0b64 0f40 007d 0c64  .d.....|.d.@.}.d
+00009440: 056a 087c 0c83 017d 0d7c 006a 0964 006b  .j.|...}.|.j.d.k
+00009450: 0972 927c 006a 096a 0a64 067c 0d83 0201  .r.|.j.j.d.|....
+00009460: 006e aa7c 0a64 076b 0272 f07c 0b64 086b  .n.|.d.k.r.|.d.k
+00009470: 0272 f07c 006a 077c 0164 0083 0201 007c  .r.|.j.|.d.....|
+00009480: 006a 0b83 005c 047d 0e7d 0f7d 107d 117c  .j...\.}.}.}.}.|
+00009490: 116a 0c64 0964 1083 027d 0c64 056a 087c  .j.d.d...}.d.j.|
+000094a0: 0c83 017d 0d7c 006a 0964 006b 0972 ee7c  ...}.|.j.d.k.r.|
+000094b0: 006a 096a 0a64 067c 0d83 0201 006e 4e7c  .j.j.d.|.....nN|
+000094c0: 0a64 076b 0290 0172 3e7c 0b64 0b6b 0290  .d.k...r>|.d.k..
+000094d0: 0172 3e64 0c74 0d64 0d7c 0a14 007c 0b17  .r>d.t.d.|...|..
+000094e0: 0083 019b 0064 0e9d 037d 0d7c 006a 0964  .....d...}.|.j.d
+000094f0: 006b 0990 0172 367c 006a 096a 0a64 067c  .k...r6|.j.j.d.|
+00009500: 0d83 0201 0074 0e7c 0d83 0182 017c 097c  .....t.|.....|.|
+00009510: 0a7c 0b66 0353 0029 114e 7a13 496e 2063  .|.f.S.).Nz.In c
+00009520: 6172 645f 756e 626c 6f63 6b5f 5049 4e72  ard_unblock_PINr
+00009530: 0100 0000 72d1 0000 0072 4401 0000 7a1e  ....r....rD...z.
+00009540: 5772 6f6e 6720 5055 4b21 207b 7d20 7472  Wrong PUK! {} tr
+00009550: 6965 7320 7265 6d61 696e 696e 6721 7245  ies remaining!rE
+00009560: 0000 0072 4200 0000 7223 0000 0072 b600  ...rB...r#...r..
+00009570: 0000 720c 0000 0072 bb00 0000 7a6b 546f  ..r....r....zkTo
+00009580: 6f20 6d61 6e79 2066 6169 6c65 6420 6174  o many failed at
+00009590: 7465 6d70 7473 2120 596f 7572 2064 6576  tempts! Your dev
+000095a0: 6963 6520 6861 7320 6265 656e 2062 6c6f  ice has been blo
+000095b0: 636b 6564 2120 0a0a 596f 7520 6e65 6564  cked! ..You need
+000095c0: 2079 6f75 7220 5055 4b20 636f 6465 2074   your PUK code t
+000095d0: 6f20 756e 626c 6f63 6b20 6974 2028 6572  o unblock it (er
+000095e0: 726f 7220 636f 6465 2072 bc00 0000 72bd  ror code r....r.
+000095f0: 0000 0069 3fff ffff 723c 0100 0029 0f72  ...i?...r<...).r
+00009600: 2700 0000 7234 0000 0072 2b00 0000 72be  '...r4...r+...r.
+00009610: 0000 0072 3300 0000 7235 0000 0072 9b00  ...r3...r5...r..
+00009620: 0000 72d8 0000 0072 4501 0000 725a 0000  ..r....rE...rZ..
+00009630: 0072 5b00 0000 7257 0000 0072 4601 0000  .r[...rW...rF...
+00009640: 724c 0000 0072 fc00 0000 2912 7236 0000  rL...r....).r6..
+00009650: 0072 7c00 0000 7240 0100 0072 a100 0000  .r|...r@...r....
+00009660: 7289 0000 0072 a200 0000 72a3 0000 0072  r....r....r....r
+00009670: cc00 0000 729a 0000 0072 2200 0000 725e  ....r....r"...r^
+00009680: 0000 0072 5f00 0000 7247 0100 0072 6200  ...r_...rG...rb.
+00009690: 0000 7248 0100 0072 4901 0000 724a 0100  ..rH...rI...rJ..
+000096a0: 0072 bf00 0000 7237 0000 0072 3700 0000  .r....r7...r7...
+000096b0: 7238 0000 00da 1063 6172 645f 756e 626c  r8.....card_unbl
+000096c0: 6f63 6b5f 5049 4e6b 0500 0073 3600 0000  ock_PINk...s6...
+000096d0: 0001 0a01 0601 0601 0401 0401 0801 1202  ................
+000096e0: 1003 1401 0c01 0801 0a01 0a01 1002 1001  ................
+000096f0: 0c01 1001 0c01 0a01 0a01 1002 1401 1801  ................
+00009700: 0c01 0e01 0802 7a1e 4361 7264 436f 6e6e  ......z.CardConn
+00009710: 6563 746f 722e 6361 7264 5f75 6e62 6c6f  ector.card_unblo
+00009720: 636b 5f50 494e 6301 0000 0000 0000 000a  ck_PINc.........
+00009730: 0000 0005 0000 0043 0000 0073 5600 0000  .......C...sV...
+00009740: 7400 6a01 6401 8301 0100 7402 6a03 7d01  t.j.d.....t.j.}.
+00009750: 7402 6a04 7d02 6402 7d03 6402 7d04 6402  t.j.}.d.}.d.}.d.
+00009760: 7d05 7c01 7c02 7c03 7c04 7c05 6705 7d06  }.|.|.|.|.|.g.}.
+00009770: 7c00 6a05 7c06 8301 5c03 7d07 7d08 7d09  |.j.|...\.}.}.}.
+00009780: 7c00 6a06 6402 6400 8302 0100 7c07 7c08  |.j.d.d.....|.|.
+00009790: 7c09 6603 5300 2903 4e7a 1249 6e20 6361  |.f.S.).Nz.In ca
+000097a0: 7264 5f6c 6f67 6f75 745f 616c 6c72 0100  rd_logout_allr..
+000097b0: 0000 2907 7227 0000 0072 3400 0000 722b  ..).r'...r4...r+
+000097c0: 0000 0072 be00 0000 5a0e 494e 535f 4c4f  ...r....Z.INS_LO
+000097d0: 474f 5554 5f41 4c4c 729b 0000 0072 d800  GOUT_ALLr....r..
+000097e0: 0000 290a 7236 0000 0072 a100 0000 7289  ..).r6...r....r.
+000097f0: 0000 0072 a200 0000 72a3 0000 0072 cc00  ...r....r....r..
+00009800: 0000 729a 0000 0072 2200 0000 725e 0000  ..r....r"...r^..
+00009810: 0072 5f00 0000 7237 0000 0072 3700 0000  .r_...r7...r7...
+00009820: 7238 0000 00da 0f63 6172 645f 6c6f 676f  r8.....card_logo
+00009830: 7574 5f61 6c6c 8e05 0000 7314 0000 0000  ut_all....s.....
+00009840: 010a 0106 0106 0104 0104 0104 010e 0210  ................
+00009850: 010c 017a 1d43 6172 6443 6f6e 6e65 6374  ...z.CardConnect
+00009860: 6f72 2e63 6172 645f 6c6f 676f 7574 5f61  or.card_logout_a
+00009870: 6c6c 6301 0000 0000 0000 000d 0000 0005  llc.............
+00009880: 0000 0043 0000 0073 8800 0000 7400 6a01  ...C...s....t.j.
+00009890: 6401 8301 0100 7402 6a03 7d01 6402 7d02  d.....t.j.}.d.}.
+000098a0: 6403 7d03 6403 7d04 7404 7400 6a05 8300  d.}.d.}.t.t.j...
+000098b0: 8301 7c00 5f06 7407 7c00 6a06 6a08 8301  ..|._.t.|.j.j...
+000098c0: 7d05 7409 7c05 8301 7d06 7c01 7c02 7c03  }.t.|...}.|.|.|.
+000098d0: 7c04 7c06 6705 7c05 1700 7d07 7c00 6a0a  |.|.g.|...}.|.j.
+000098e0: 7c07 8301 5c03 7d08 7d09 7d0a 7c00 6a0b  |...\.}.}.}.|.j.
+000098f0: 6a0c 7c08 8301 7d0b 7c0b 6a0d 6404 6405  j.|...}.|.j.d.d.
+00009900: 8d01 7d0c 7c00 6a06 6a0e 7c0c 8301 0100  ..}.|.j.j.|.....
+00009910: 7c0b 5300 2906 4e7a 2149 6e20 6361 7264  |.S.).Nz!In card
+00009920: 5f69 6e69 7469 6174 655f 7365 6375 7265  _initiate_secure
+00009930: 5f63 6861 6e6e 656c 2829 7285 0000 0072  _channel()r....r
+00009940: 0100 0000 4629 0172 0b01 0000 290f 7227  ....F).r....).r'
+00009950: 0000 0072 3400 0000 722b 0000 0072 be00  ...r4...r+...r..
+00009960: 0000 7212 0000 00da 1167 6574 4566 6665  ..r......getEffe
+00009970: 6374 6976 654c 6576 656c 727b 0000 0072  ctiveLevelr{...r
+00009980: c800 0000 5a14 7363 5f70 7562 6b65 795f  ....Z.sc_pubkey_
+00009990: 7365 7269 616c 697a 6564 7235 0000 0072  serializedr5...r
+000099a0: 9b00 0000 7277 0000 005a 1d70 6172 7365  ....rw...Z.parse
+000099b0: 5f69 6e69 7469 6174 655f 7365 6375 7265  _initiate_secure
+000099c0: 5f63 6861 6e6e 656c 72e3 0000 005a 1769  _channelr....Z.i
+000099d0: 6e69 7469 6174 655f 7365 6375 7265 5f63  nitiate_secure_c
+000099e0: 6861 6e6e 656c 290d 7236 0000 0072 a100  hannel).r6...r..
+000099f0: 0000 7289 0000 0072 a200 0000 72a3 0000  ..r....r....r...
+00009a00: 0072 1301 0000 72cc 0000 0072 9a00 0000  .r....r....r....
+00009a10: 7222 0000 0072 5e00 0000 725f 0000 005a  r"...r^...r_...Z
+00009a20: 0b70 6565 725f 7075 626b 6579 5a11 7065  .peer_pubkeyZ.pe
+00009a30: 6572 5f70 7562 6b65 795f 6279 7465 7372  er_pubkey_bytesr
+00009a40: 3700 0000 7237 0000 0072 3800 0000 7259  7...r7...r8...rY
+00009a50: 0000 009f 0500 0073 1c00 0000 0001 0a01  .......s........
+00009a60: 0601 0401 0401 0403 0e01 0c01 0801 1203  ................
+00009a70: 1003 0c01 0c01 0c02 7a2a 4361 7264 436f  ........z*CardCo
+00009a80: 6e6e 6563 746f 722e 6361 7264 5f69 6e69  nnector.card_ini
+00009a90: 7469 6174 655f 7365 6375 7265 5f63 6861  tiate_secure_cha
+00009aa0: 6e6e 656c 6302 0000 0000 0000 000c 0000  nnelc...........
+00009ab0: 0009 0000 0043 0000 0073 0601 0000 7400  .....C...s....t.
+00009ac0: 6a01 6401 8301 0100 7402 6a03 7d02 6402  j.d.....t.j.}.d.
+00009ad0: 7d03 6403 7d04 6403 7d05 7c01 6404 1900  }.d.}.d.}.|.d...
+00009ae0: 7402 6a04 7402 6a05 7402 6a06 7402 6a07  t.j.t.j.t.j.t.j.
+00009af0: 7402 6a08 7402 6a09 7402 6a0a 7402 6a0b  t.j.t.j.t.j.t.j.
+00009b00: 6608 6b06 7276 7400 6a01 6405 740c 7c01  f.k.rvt.j.d.t.|.
+00009b10: 6403 6406 8502 1900 8301 9b00 740d 7c01  d.d.........t.|.
+00009b20: 8301 6406 1800 6407 1400 9b00 9d03 8301  ..d...d.........
+00009b30: 0100 6e14 7400 6a01 6405 740c 7c01 8301  ..n.t.j.d.t.|...
+00009b40: 9b00 9d02 8301 0100 7c00 6a0e 6a0f 7410  ........|.j.j.t.
+00009b50: 7c01 8301 8301 5c03 7d06 7d07 7d08 7411  |.....\.}.}.}.t.
+00009b60: 7c06 8301 740d 7c07 8301 6408 3f00 740d  |...t.|...d.?.t.
+00009b70: 7c07 8301 6409 4000 6702 1700 7411 7c07  |...d.@.g...t.|.
+00009b80: 8301 1700 740d 7c08 8301 6408 3f00 740d  ....t.|...d.?.t.
+00009b90: 7c08 8301 6409 4000 6702 1700 7411 7c08  |...d.@.g...t.|.
+00009ba0: 8301 1700 7d09 740d 7c09 8301 7d0a 7c02  ....}.t.|...}.|.
+00009bb0: 7c03 7c04 7c05 7c0a 6705 7c09 1700 7d0b  |.|.|.|.g.|...}.
+00009bc0: 7c0b 5300 290a 4e7a 2049 6e20 6361 7264  |.S.).Nz In card
+00009bd0: 5f65 6e63 7279 7074 5f73 6563 7572 655f  _encrypt_secure_
+00009be0: 6368 616e 6e65 6c28 2972 8600 0000 7201  channel()r....r.
+00009bf0: 0000 0072 0c00 0000 7a12 506c 6169 6e74  ...r....z.Plaint
+00009c00: 6578 7420 432d 4150 4455 3a20 7221 0000  ext C-APDU: r!..
+00009c10: 007a 0220 2a72 b400 0000 72d5 0000 0029  .z. *r....r....)
+00009c20: 1272 2700 0000 7234 0000 0072 2b00 0000  .r'...r4...r+...
+00009c30: 72be 0000 0072 2c00 0000 722d 0000 0072  r....r,...r-...r
+00009c40: 2e00 0000 722f 0000 0072 3000 0000 7231  ....r/...r0...r1
+00009c50: 0000 0072 3200 0000 7233 0000 0072 0900  ...r2...r3...r..
+00009c60: 0000 7235 0000 0072 7b00 0000 5a16 656e  ..r5...r{...Z.en
+00009c70: 6372 7970 745f 7365 6375 7265 5f63 6861  crypt_secure_cha
+00009c80: 6e6e 656c 724b 0000 0072 c800 0000 290c  nnelrK...r....).
+00009c90: 7236 0000 0072 9a00 0000 72a1 0000 0072  r6...r....r....r
+00009ca0: 8900 0000 72a2 0000 0072 a300 0000 72eb  ....r....r....r.
+00009cb0: 0000 00da 0a63 6970 6865 7274 6578 74da  .....ciphertext.
+00009cc0: 036d 6163 72cb 0000 0072 cc00 0000 5a0e  .macr....r....Z.
+00009cd0: 656e 6372 7970 7465 645f 6170 6475 7237  encrypted_apdur7
+00009ce0: 0000 0072 3700 0000 7238 0000 0072 8f00  ...r7...r8...r..
+00009cf0: 0000 b605 0000 7320 0000 0000 010a 0106  ......s ........
+00009d00: 0104 0104 0104 030e 0108 0108 010e 012e  ................
+00009d10: 0214 0216 0148 0108 0212 027a 2943 6172  .....H.....z)Car
+00009d20: 6443 6f6e 6e65 6374 6f72 2e63 6172 645f  dConnector.card_
+00009d30: 656e 6372 7970 745f 7365 6375 7265 5f63  encrypt_secure_c
+00009d40: 6861 6e6e 656c 6302 0000 0000 0000 0006  hannelc.........
+00009d50: 0000 0007 0000 0043 0000 0073 c600 0000  .......C...s....
+00009d60: 7400 6a01 6401 8301 0100 7402 7c01 8301  t.j.d.....t.|...
+00009d70: 6402 6b02 721a 7c01 5300 7402 7c01 8301  d.k.r.|.S.t.|...
+00009d80: 6403 6b00 722e 7403 6404 8301 8201 7404  d.k.r.t.d.....t.
+00009d90: 7c01 6402 6405 8502 1900 8301 7d02 7c01  |.d.d.......}.|.
+00009da0: 6405 1900 6406 4000 6407 3e00 7c01 6408  d...d.@.d.>.|.d.
+00009db0: 1900 6406 4000 1700 7d03 7404 7c01 6403  ..d.@...}.t.|.d.
+00009dc0: 6400 8502 1900 8301 7d04 7402 7c04 8301  d.......}.t.|...
+00009dd0: 7c03 6b03 72a0 7400 6a05 6409 7406 7c03  |.k.r.t.j.d.t.|.
+00009de0: 8301 9b00 640a 7406 7402 7c04 8301 8301  ....d.t.t.|.....
+00009df0: 9b00 9d04 8301 0100 7403 640b 8301 8201  ........t.d.....
+00009e00: 7c00 6a07 6a08 7c02 7c04 8302 7d05 7400  |.j.j.|.|...}.t.
+00009e10: 6a01 640c 7409 7c05 8301 9b00 9d02 8301  j.d.t.|.........
+00009e20: 0100 7c05 5300 290d 4e7a 1e49 6e20 6361  ..|.S.).Nz.In ca
+00009e30: 7264 5f64 6563 7279 7074 5f73 6563 7572  rd_decrypt_secur
+00009e40: 655f 6368 616e 6e65 6c72 0100 0000 e912  e_channelr......
+00009e50: 0000 007a 2445 6e63 7279 7074 6564 2072  ...z$Encrypted r
+00009e60: 6573 706f 6e73 6520 6861 7320 7772 6f6e  esponse has wron
+00009e70: 6720 6c65 6e67 6874 2172 8a00 0000 72d5  g lenght!r....r.
+00009e80: 0000 0072 b400 0000 e911 0000 007a 4649  ...r.........zFI
+00009e90: 6e20 6361 7264 5f64 6563 7279 7074 5f73  n card_decrypt_s
+00009ea0: 6563 7572 655f 6368 616e 6e65 6c3a 2063  ecure_channel: c
+00009eb0: 6970 6865 7274 6578 7420 6861 7320 7772  iphertext has wr
+00009ec0: 6f6e 6720 6c65 6e67 7468 3a20 6578 7065  ong length: expe
+00009ed0: 6374 6564 207a 0520 676f 7420 7a1c 4369  cted z. got z.Ci
+00009ee0: 7068 6572 7465 7874 2068 6173 2077 726f  phertext has wro
+00009ef0: 6e67 206c 656e 6768 7421 7a12 506c 6169  ng lenght!z.Plai
+00009f00: 6e74 6578 7420 522d 4150 4455 3a20 290a  ntext R-APDU: ).
+00009f10: 7227 0000 0072 3400 0000 7235 0000 0072  r'...r4...r5...r
+00009f20: fc00 0000 724b 0000 0072 5400 0000 7276  ....rK...rT...rv
+00009f30: 0000 0072 7b00 0000 5a16 6465 6372 7970  ...r{...Z.decryp
+00009f40: 745f 7365 6375 7265 5f63 6861 6e6e 656c  t_secure_channel
+00009f50: 7209 0000 0029 0672 3600 0000 7222 0000  r....).r6...r"..
+00009f60: 0072 eb00 0000 723e 0100 0072 4f01 0000  .r....r>...rO...
+00009f70: 5a09 706c 6169 6e74 6578 7472 3700 0000  Z.plaintextr7...
+00009f80: 7237 0000 0072 3800 0000 7291 0000 00ce  r7...r8...r.....
+00009f90: 0500 0073 1c00 0000 0001 0a02 0c01 0401  ...s............
+00009fa0: 0c01 0802 1001 1c01 1001 0c01 2201 0802  ............"...
+00009fb0: 0e03 1402 7a29 4361 7264 436f 6e6e 6563  ....z)CardConnec
+00009fc0: 746f 722e 6361 7264 5f64 6563 7279 7074  tor.card_decrypt
+00009fd0: 5f73 6563 7572 655f 6368 616e 6e65 6c29  _secure_channel)
+00009fe0: 0172 c500 0000 6304 0000 0000 0000 0012  .r....c.........
+00009ff0: 0000 0005 0000 0043 0000 0073 e000 0000  .......C...s....
+0000a000: 7400 6a01 6401 8301 0100 7402 6a03 7d04  t.j.d.....t.j.}.
+0000a010: 6402 7d05 7c01 7d06 7c02 7d07 7404 7c03  d.}.|.}.|.}.t.|.
+0000a020: 6a05 6403 8301 8301 7d03 7406 7c03 8301  j.d.....}.t.|...
+0000a030: 7d08 7c08 6701 7c03 1700 7d09 7406 7c09  }.|.g.|...}.t.|.
+0000a040: 8301 7d0a 7c04 7c05 7c06 7c07 7c0a 6705  ..}.|.|.|.|.|.g.
+0000a050: 7c09 1700 7d0b 7c00 6a07 7c0b 8301 5c03  |...}.|.j.|...\.
+0000a060: 7d0c 7d0d 7d0e 7c0d 6404 6b02 72b4 7c0e  }.}.}.|.d.k.r.|.
+0000a070: 6405 6b02 72b4 7c0c 6405 1900 6406 3e00  d.k.r.|.d...d.>.
+0000a080: 7c0c 6407 1900 1700 7d0f 7400 6a01 6408  |.d.....}.t.j.d.
+0000a090: 7c0f 9b00 9d02 8301 0100 7c0c 6409 640d  |.........|.d.d.
+0000a0a0: 8502 1900 7d10 7408 7c10 8301 6a09 8300  ....}.t.|...j...
+0000a0b0: 7d11 6e1e 7400 6a0a 640b 7c0d 9b00 640c  }.n.t.j.d.|...d.
+0000a0c0: 7c0e 9b00 9d04 8301 0100 6400 7d0f 6400  |.........d.}.d.
+0000a0d0: 7d11 7c0c 7c0d 7c0e 7c0f 7c11 6605 5300  }.|.|.|.|.|.f.S.
+0000a0e0: 290e 4e7a 2149 6e20 7365 6564 6b65 6570  ).Nz!In seedkeep
+0000a0f0: 6572 5f67 656e 6572 6174 655f 6d61 7374  er_generate_mast
+0000a100: 6572 7365 6564 e9a0 0000 007a 0575 7466  erseed.....z.utf
+0000a110: 2d38 7241 0000 0072 0100 0000 72b4 0000  -8rA...r....r...
+0000a120: 0072 0c00 0000 7a2b 4d61 7374 6572 7365  .r....z+Masterse
+0000a130: 6564 2067 656e 6572 6174 6564 2073 7563  ed generated suc
+0000a140: 6365 7373 6675 6c6c 7920 7769 7468 2069  cessfully with i
+0000a150: 643a 2072 2300 0000 7243 0000 007a 2445  d: r#...rC...z$E
+0000a160: 7272 6f72 2064 7572 696e 6720 6d61 7374  rror during mast
+0000a170: 6572 7365 6564 2067 656e 6572 6174 696f  erseed generatio
+0000a180: 6e3a 2072 2400 0000 7287 0000 0029 0b72  n: r$...r....).r
+0000a190: 2700 0000 7234 0000 0072 2b00 0000 72be  '...r4...r+...r.
+0000a1a0: 0000 0072 c800 0000 72c9 0000 0072 3500  ...r....r....r5.
+0000a1b0: 0000 729b 0000 0072 4b00 0000 724c 0000  ..r....rK...rL..
+0000a1c0: 0072 e400 0000 2912 7236 0000 005a 0973  .r....).r6...Z.s
+0000a1d0: 6565 645f 7369 7a65 da0d 6578 706f 7274  eed_size..export
+0000a1e0: 5f72 6967 6874 7372 c500 0000 72a1 0000  _rightsr....r...
+0000a1f0: 0072 8900 0000 72a2 0000 0072 a300 0000  .r....r....r....
+0000a200: 72c4 0000 0072 cb00 0000 72cc 0000 0072  r....r....r....r
+0000a210: 9a00 0000 7222 0000 0072 5e00 0000 725f  ....r"...r^...r_
+0000a220: 0000 00da 0269 64da 1066 696e 6765 7270  .....id..fingerp
+0000a230: 7269 6e74 5f6c 6973 7472 1c01 0000 7237  rint_listr....r7
+0000a240: 0000 0072 3700 0000 7238 0000 00da 1e73  ...r7...r8.....s
+0000a250: 6565 646b 6565 7065 725f 6765 6e65 7261  eedkeeper_genera
+0000a260: 7465 5f6d 6173 7465 7273 6565 64e8 0500  te_masterseed...
+0000a270: 0073 2800 0000 0001 0a01 0601 0401 0401  .s(.............
+0000a280: 0402 0e01 0801 0a02 0801 1203 1001 1001  ................
+0000a290: 1401 1001 0c01 0e02 1601 0401 0402 7a2c  ..............z,
+0000a2a0: 4361 7264 436f 6e6e 6563 746f 722e 7365  CardConnector.se
+0000a2b0: 6564 6b65 6570 6572 5f67 656e 6572 6174  edkeeper_generat
+0000a2c0: 655f 6d61 7374 6572 7365 6564 6303 0000  e_masterseedc...
+0000a2d0: 0000 0000 0011 0000 0005 0000 0043 0000  .............C..
+0000a2e0: 0073 e000 0000 7400 6a01 6401 8301 0100  .s....t.j.d.....
+0000a2f0: 7402 6a03 7d03 6402 7d04 6403 7d05 7c01  t.j.}.d.}.d.}.|.
+0000a300: 7d06 7404 7c02 6a05 6404 8301 8301 7d02  }.t.|.j.d.....}.
+0000a310: 7406 7c02 8301 7d07 7c07 6701 7c02 1700  t.|...}.|.g.|...
+0000a320: 7d08 7406 7c08 8301 7d09 7c03 7c04 7c05  }.t.|...}.|.|.|.
+0000a330: 7c06 7c09 6705 7c08 1700 7d0a 7c00 6a07  |.|.g.|...}.|.j.
+0000a340: 7c0a 8301 5c03 7d0b 7d0c 7d0d 7c0c 6405  |...\.}.}.}.|.d.
+0000a350: 6b02 72b4 7c0d 6403 6b02 72b4 7c0b 6403  k.r.|.d.k.r.|.d.
+0000a360: 1900 6406 3e00 7c0b 6407 1900 1700 7d0e  ..d.>.|.d.....}.
+0000a370: 7400 6a01 6408 7c0e 9b00 9d02 8301 0100  t.j.d.|.........
+0000a380: 7c0b 6409 640d 8502 1900 7d0f 7408 7c0f  |.d.d.....}.t.|.
+0000a390: 8301 6a09 8300 7d10 6e1e 7400 6a0a 640b  ..j...}.n.t.j.d.
+0000a3a0: 7c0c 9b00 640c 7c0d 9b00 9d04 8301 0100  |...d.|.........
+0000a3b0: 6400 7d0e 6400 7d10 7c0b 7c0c 7c0d 7c0e  d.}.d.}.|.|.|.|.
+0000a3c0: 7c10 6605 5300 290e 4e7a 2149 6e20 7365  |.f.S.).Nz!In se
+0000a3d0: 6564 6b65 6570 6572 5f67 656e 6572 6174  edkeeper_generat
+0000a3e0: 655f 3246 415f 7365 6372 6574 e9ae 0000  e_2FA_secret....
+0000a3f0: 0072 0100 0000 7a05 7574 662d 3872 4100  .r....z.utf-8rA.
+0000a400: 0000 72b4 0000 0072 0c00 0000 7a2b 3246  ..r....r....z+2F
+0000a410: 4120 7365 6372 6574 2067 656e 6572 6174  A secret generat
+0000a420: 6564 2073 7563 6365 7373 6675 6c6c 7920  ed successfully 
+0000a430: 7769 7468 2069 643a 2072 2300 0000 7243  with id: r#...rC
+0000a440: 0000 007a 2445 7272 6f72 2064 7572 696e  ...z$Error durin
+0000a450: 6720 6d61 7374 6572 7365 6564 2067 656e  g masterseed gen
+0000a460: 6572 6174 696f 6e3a 2072 2400 0000 7287  eration: r$...r.
+0000a470: 0000 0029 0b72 2700 0000 7234 0000 0072  ...).r'...r4...r
+0000a480: 2b00 0000 72be 0000 0072 c800 0000 72c9  +...r....r....r.
+0000a490: 0000 0072 3500 0000 729b 0000 0072 4b00  ...r5...r....rK.
+0000a4a0: 0000 724c 0000 0072 e400 0000 2911 7236  ..rL...r....).r6
+0000a4b0: 0000 0072 5401 0000 72c5 0000 0072 a100  ...rT...r....r..
+0000a4c0: 0000 7289 0000 0072 a200 0000 72a3 0000  ..r....r....r...
+0000a4d0: 0072 c400 0000 72cb 0000 0072 cc00 0000  .r....r....r....
+0000a4e0: 729a 0000 0072 2200 0000 725e 0000 0072  r....r"...r^...r
+0000a4f0: 5f00 0000 7255 0100 0072 5601 0000 721c  _...rU...rV...r.
+0000a500: 0100 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
+0000a510: 0000 da1e 7365 6564 6b65 6570 6572 5f67  ....seedkeeper_g
+0000a520: 656e 6572 6174 655f 3246 415f 7365 6372  enerate_2FA_secr
+0000a530: 6574 0406 0000 7328 0000 0000 010a 0106  et....s(........
+0000a540: 0104 0104 0104 020e 0108 010a 0208 0112  ................
+0000a550: 0310 0110 0114 0110 010c 010e 0216 0104  ................
+0000a560: 0104 027a 2c43 6172 6443 6f6e 6e65 6374  ...z,CardConnect
+0000a570: 6f72 2e73 6565 646b 6565 7065 725f 6765  or.seedkeeper_ge
+0000a580: 6e65 7261 7465 5f32 4641 5f73 6563 7265  nerate_2FA_secre
+0000a590: 7463 0300 0000 0000 0000 1900 0000 0600  tc..............
+0000a5a0: 0000 4300 0000 7392 0300 0074 006a 0164  ..C...s....t.j.d
+0000a5b0: 0183 0101 007c 0264 006b 0872 1664 026e  .....|.d.k.r.d.n
+0000a5c0: 0264 037d 0374 026a 037d 0464 047d 057c  .d.}.t.j.}.d.}.|
+0000a5d0: 0372 2c64 056e 0264 067d 0664 067d 0774  .r,d.n.d.}.d.}.t
+0000a5e0: 0474 056a 067c 0164 0719 0064 0864 0085  .t.j.|.d...d.d..
+0000a5f0: 0219 0083 0183 017d 087c 087d 097c 0372  .......}.|.}.|.r
+0000a600: 8474 0474 056a 067c 0164 0919 0083 0183  .t.t.j.|.d......
+0000a610: 017d 0a7c 097c 0264 0a3f 0064 0b16 007c  .}.|.|.d.?.d...|
+0000a620: 0264 0b16 0067 027c 0a17 0037 007d 0974  .d...g.|...7.}.t
+0000a630: 077c 0983 017d 0b7c 047c 057c 067c 077c  .|...}.|.|.|.|.|
+0000a640: 0b67 057c 0917 007d 0c7c 006a 087c 0c83  .g.|...}.|.j.|..
+0000a650: 015c 037d 0d7d 0e7d 0f7c 0e64 0c6b 0373  .\.}.}.}.|.d.k.s
+0000a660: be7c 0f64 0d6b 0372 f474 006a 0964 0e7c  .|.d.k.r.t.j.d.|
+0000a670: 0e64 0b14 007c 0f17 0064 0f9b 049d 0283  .d...|...d......
+0000a680: 0101 0074 0a64 1074 0b64 0b7c 0e14 007c  ...t.d.t.d.|...|
+0000a690: 0f17 0083 019b 0064 119d 0383 0182 0164  .......d.......d
+0000a6a0: 057d 0764 127d 107c 0390 0172 1674 0474  .}.d.}.|...r.t.t
+0000a6b0: 056a 067c 0164 1319 0083 0183 017d 116e  .j.|.d.......}.n
+0000a6c0: 087c 0164 1419 007d 1164 0d7d 1274 077c  .|.d...}.d.}.t.|
+0000a6d0: 1183 017d 1378 b87c 137c 106b 0490 0172  ...}.x.|.|.k...r
+0000a6e0: e27c 1064 0a3f 007c 1064 0b16 0067 027c  .|.d.?.|.d...g.|
+0000a6f0: 117c 127c 127c 1017 0085 0219 0017 007d  .|.|.|.........}
+0000a700: 0974 077c 0983 017d 0b7c 047c 057c 067c  .t.|...}.|.|.|.|
+0000a710: 077c 0b67 057c 0917 007d 0c7c 006a 087c  .|.g.|...}.|.j.|
+0000a720: 0c83 015c 037d 0d7d 0e7d 0f7c 0e64 0c6b  ...\.}.}.}.|.d.k
+0000a730: 0390 0173 947c 0f64 0d6b 0390 0172 ce74  ...s.|.d.k...r.t
+0000a740: 006a 0964 1574 0b64 0b7c 0e14 007c 0f17  .j.d.t.d.|...|..
+0000a750: 0083 019b 0064 119d 0383 0101 0074 0a64  .....d.......t.d
+0000a760: 1074 0b64 0b7c 0e14 007c 0f17 0083 019b  .t.d.|...|......
+0000a770: 0064 119d 0383 0182 017c 127c 1037 007d  .d.......|.|.7.}
+0000a780: 127c 137c 1038 007d 1390 0171 2c57 0064  .|.|.8.}...q,W.d
+0000a790: 167d 077c 1364 0a3f 007c 1364 0b16 0067  .}.|.d.?.|.d...g
+0000a7a0: 027c 117c 127c 127c 1317 0085 0219 0017  .|.|.|.|........
+0000a7b0: 007d 097c 0390 0272 3274 0474 056a 067c  .}.|...r2t.t.j.|
+0000a7c0: 0164 1719 0083 0183 017d 147c 0974 077c  .d.......}.|.t.|
+0000a7d0: 1483 0167 017c 1417 0037 007d 0974 077c  ...g.|...7.}.t.|
+0000a7e0: 0983 017d 0b7c 047c 057c 067c 077c 0b67  ...}.|.|.|.|.|.g
+0000a7f0: 057c 0917 007d 0c7c 006a 087c 0c83 015c  .|...}.|.j.|...\
+0000a800: 037d 0d7d 0e7d 0f7c 0e64 186b 0290 0272  .}.}.}.|.d.k...r
+0000a810: ac7c 0f64 196b 0290 0272 ac74 006a 0964  .|.d.k...r.t.j.d
+0000a820: 1a74 0b64 0b7c 0e14 007c 0f17 0083 019b  .t.d.|...|......
+0000a830: 0064 119d 0383 0101 0074 0c64 1b74 0b64  .d.......t.d.t.d
+0000a840: 0b7c 0e14 007c 0f17 0083 019b 0064 119d  .|...|.......d..
+0000a850: 0383 0182 016e 4e7c 0e64 0c6b 0390 0273  .....nN|.d.k...s
+0000a860: c07c 0f64 0d6b 0390 0272 fa74 006a 0964  .|.d.k...r.t.j.d
+0000a870: 1c74 0b64 0b7c 0e14 007c 0f17 0083 019b  .t.d.|...|......
+0000a880: 0064 119d 0383 0101 0074 0a64 1074 0b64  .d.......t.d.t.d
+0000a890: 0b7c 0e14 007c 0f17 0083 019b 0064 119d  .|...|.......d..
+0000a8a0: 0383 0182 017c 127c 1037 007d 1264 0d7d  .....|.|.7.}.d.}
+0000a8b0: 137c 0d64 0d19 0064 0b14 007c 0d64 0619  .|.d...d...|.d..
+0000a8c0: 0017 007d 157c 0d64 0564 1d85 0219 007d  ...}.|.d.d.....}
+0000a8d0: 1674 057c 1683 016a 0b83 007d 177c 0390  .t.|...j...}.|..
+0000a8e0: 0372 427c 0164 1e19 007d 186e 1a74 0d6a  .rB|.d...}.n.t.j
+0000a8f0: 0e74 057c 1183 0183 016a 0f83 0064 0d64  .t.|.....j...d.d
+0000a900: 0a85 0219 007d 187c 187c 176b 0290 0372  .....}.|.|.k...r
+0000a910: 7274 006a 0164 1f83 0101 006e 1874 006a  rt.j.d.....n.t.j
+0000a920: 0964 207c 189b 0064 217c 179b 0064 229d  .d |...d!|...d".
+0000a930: 0583 0101 007c 157c 1766 0253 0029 234e  .....|.|.f.S.)#N
+0000a940: 7a1b 496e 2073 6565 646b 6565 7065 725f  z.In seedkeeper_
+0000a950: 696d 706f 7274 5f73 6563 7265 7446 54e9  import_secretFT.
+0000a960: a100 0000 7223 0000 0072 0c00 0000 72ea  ....r#...r....r.
+0000a970: 0000 0072 4300 0000 72eb 0000 0072 b400  ...rC...r....r..
+0000a980: 0000 72bc 0000 0072 4100 0000 7201 0000  ..r....rA...r...
+0000a990: 007a 2645 7272 6f72 2064 7572 696e 6720  .z&Error during 
+0000a9a0: 7365 6372 6574 2069 6d70 6f72 7420 2d20  secret import - 
+0000a9b0: 4f50 5f49 4e49 543a 207a 0430 3e34 587a  OP_INIT: z.0>4Xz
+0000a9c0: 3955 6e65 7870 6563 7465 6420 6572 726f  9Unexpected erro
+0000a9d0: 7220 6475 7269 6e67 2073 6563 7572 6520  r during secure 
+0000a9e0: 7365 6372 6574 2069 6d70 6f72 7420 2865  secret import (e
+0000a9f0: 7272 6f72 2063 6f64 6520 72bd 0000 0072  rror code r....r
+0000aa00: 9d00 0000 72ec 0000 0072 f700 0000 7a34  ....r....r....z4
+0000aa10: 4572 726f 7220 6475 7269 6e67 2073 6563  Error during sec
+0000aa20: 7265 7420 696d 706f 7274 202d 204f 505f  ret import - OP_
+0000aa30: 5052 4f43 4553 5320 2865 7272 6f72 2063  PROCESS (error c
+0000aa40: 6f64 6520 72b3 0000 0072 ed00 0000 7242  ode r....r....rB
+0000aa50: 0000 0072 ef00 0000 7a3d 4572 726f 7220  ...r....z=Error 
+0000aa60: 6475 7269 6e67 2073 6563 7265 7420 696d  during secret im
+0000aa70: 706f 7274 202d 204f 505f 4649 4e41 4c3a  port - OP_FINAL:
+0000aa80: 2077 726f 6e67 206d 6163 2028 6572 726f   wrong mac (erro
+0000aa90: 7220 636f 6465 207a 3245 7272 6f72 2064  r code z2Error d
+0000aaa0: 7572 696e 6720 7365 6372 6574 2069 6d70  uring secret imp
+0000aab0: 6f72 743a 2077 726f 6e67 206d 6163 2028  ort: wrong mac (
+0000aac0: 6572 726f 7220 636f 6465 207a 3245 7272  error code z2Err
+0000aad0: 6f72 2064 7572 696e 6720 7365 6372 6574  or during secret
+0000aae0: 2069 6d70 6f72 7420 2d20 4f50 5f46 494e   import - OP_FIN
+0000aaf0: 414c 2028 6572 726f 7220 636f 6465 2072  AL (error code r
+0000ab00: 8700 0000 721c 0100 007a 1446 696e 6765  ....r....z.Finge
+0000ab10: 7270 7269 6e74 7320 6d61 7463 6820 217a  rprints match !z
+0000ab20: 1f46 696e 6765 7270 7269 6e74 206d 6973  .Fingerprint mis
+0000ab30: 6d61 7463 683a 2065 7870 6563 7465 6420  match: expected 
+0000ab40: 7a0f 2062 7574 2072 6563 6f76 6572 6564  z. but recovered
+0000ab50: 2072 2400 0000 2910 7227 0000 0072 3400   r$...).r'...r4.
+0000ab60: 0000 722b 0000 0072 be00 0000 72c8 0000  ..r+...r....r...
+0000ab70: 0072 4b00 0000 72e1 0000 0072 3500 0000  .rK...r....r5...
+0000ab80: 729b 0000 0072 e400 0000 72f4 0000 0072  r....r....r....r
+0000ab90: 4c00 0000 da0f 5365 6564 4b65 6570 6572  L.....SeedKeeper
+0000aba0: 4572 726f 7272 4f00 0000 7239 0100 0072  ErrorrO...r9...r
+0000abb0: 5100 0000 2919 7236 0000 0072 f600 0000  Q...).r6...r....
+0000abc0: da0a 7369 645f 7075 626b 6579 5a10 6973  ..sid_pubkeyZ.is
+0000abd0: 5f73 6563 7572 655f 696d 706f 7274 72a1  _secure_importr.
+0000abe0: 0000 0072 8900 0000 72a2 0000 0072 a300  ...r....r....r..
+0000abf0: 0000 72ea 0000 0072 cb00 0000 72eb 0000  ..r....r....r...
+0000ac00: 0072 cc00 0000 729a 0000 0072 2200 0000  .r....r....r"...
+0000ac10: 725e 0000 0072 5f00 0000 da0a 6368 756e  r^...r_.....chun
+0000ac20: 6b5f 7369 7a65 72f7 0000 005a 0d73 6563  k_sizer....Z.sec
+0000ac30: 7265 745f 6f66 6673 6574 5a10 7365 6372  ret_offsetZ.secr
+0000ac40: 6574 5f72 656d 6169 6e69 6e67 72ed 0000  et_remainingr...
+0000ac50: 0072 5501 0000 7256 0100 005a 1b66 696e  .rU...rV...Z.fin
+0000ac60: 6765 7270 7269 6e74 5f66 726f 6d5f 7365  gerprint_from_se
+0000ac70: 6564 6b65 6570 6572 da17 6669 6e67 6572  edkeeper..finger
+0000ac80: 7072 696e 745f 6672 6f6d 5f73 6563 7265  print_from_secre
+0000ac90: 7472 3700 0000 7237 0000 0072 3800 0000  tr7...r7...r8...
+0000aca0: da18 7365 6564 6b65 6570 6572 5f69 6d70  ..seedkeeper_imp
+0000acb0: 6f72 745f 7365 6372 6574 2006 0000 7378  ort_secret ...sx
+0000acc0: 0000 0000 010a 0210 0206 0104 010c 0304  ................
+0000acd0: 011a 0304 0104 0112 011c 0108 0112 0110  ................
+0000ace0: 0110 011a 011c 0304 0104 0106 0114 0208  ................
+0000acf0: 0104 0108 010c 0120 0108 0112 0110 0114  ....... ........
+0000ad00: 011e 011c 0108 010e 0304 0120 0106 0112  ........... ....
+0000ad10: 0112 0108 0112 0110 0114 011e 011e 0114  ................
+0000ad20: 011e 011c 0108 0104 0314 010c 010c 0106  ................
+0000ad30: 010a 021a 010a 010c 0218 027a 2643 6172  ...........z&Car
+0000ad40: 6443 6f6e 6e65 6374 6f72 2e73 6565 646b  dConnector.seedk
+0000ad50: 6565 7065 725f 696d 706f 7274 5f73 6563  eeper_import_sec
+0000ad60: 7265 7463 0300 0000 0000 0000 1800 0000  retc............
+0000ad70: 0600 0000 4300 0000 734e 0300 0074 006a  ....C...sN...t.j
+0000ad80: 0164 0183 0101 007c 0264 006b 0872 1664  .d.....|.d.k.r.d
+0000ad90: 026e 0264 037d 0374 026a 037d 0464 047d  .n.d.}.t.j.}.d.}
+0000ada0: 057c 0372 2c64 056e 0264 067d 0664 067d  .|.r,d.n.d.}.d.}
+0000adb0: 077c 0164 073f 0064 0816 007c 0164 0816  .|.d.?.d...|.d..
+0000adc0: 0067 027d 087c 0372 647c 087c 0264 073f  .g.}.|.rd|.|.d.?
+0000add0: 0064 0816 007c 0264 0816 0067 0237 007d  .d...|.d...g.7.}
+0000ade0: 0874 047c 0883 017d 097c 047c 057c 067c  .t.|...}.|.|.|.|
+0000adf0: 077c 0967 057c 0817 007d 0a7c 006a 057c  .|.g.|...}.|.j.|
+0000ae00: 0a83 015c 037d 0b7d 0c7d 0d7c 0c64 096b  ...\.}.}.}.|.d.k
+0000ae10: 0272 a07c 0d64 0a6b 0272 a06e a87c 0c64  .r.|.d.k.r.n.|.d
+0000ae20: 0b6b 0272 c47c 0d64 0c6b 0272 c474 006a  .k.r.|.d.k.r.t.j
+0000ae30: 0664 0d83 0101 0074 0764 0d83 0182 016e  .d.....t.d.....n
+0000ae40: 847c 0c64 0b6b 0272 e87c 0d64 076b 0272  .|.d.k.r.|.d.k.r
+0000ae50: e874 006a 0664 0e83 0101 0074 0764 0e83  .t.j.d.....t.d..
+0000ae60: 0182 016e 607c 0c64 0b6b 026f f67c 0d64  ...n`|.d.k.o.|.d
+0000ae70: 0f6b 0290 0172 0e74 006a 0664 1083 0101  .k...r.t.j.d....
+0000ae80: 0074 0764 1083 0182 016e 3a74 006a 0664  .t.d.....n:t.j.d
+0000ae90: 1174 0864 087c 0c14 007c 0d17 0083 019b  .t.d.|...|......
+0000aea0: 0064 129d 0383 0101 0074 0964 1174 0864  .d.......t.d.t.d
+0000aeb0: 087c 0c14 007c 0d17 0083 019b 0064 129d  .|...|.......d..
+0000aec0: 0383 0182 017c 006a 0a6a 0b7c 0b83 017d  .....|.j.j.|...}
+0000aed0: 0e7c 0390 0172 947c 0b64 2864 0085 0219  .|...r.|.d(d....
+0000aee0: 007d 0f74 006a 0164 1474 0c7c 0f83 016a  .}.t.j.d.t.|...j
+0000aef0: 0883 0017 0083 0101 007c 0f7c 0e64 153c  .........|.|.d.<
+0000af00: 0074 0c7c 0f83 016a 0883 007c 0e64 163c  .t.|...j...|.d.<
+0000af10: 0067 007d 1064 057d 077c 047c 057c 067c  .g.}.d.}.|.|.|.|
+0000af20: 077c 0967 057c 0817 007d 0a90 0178 067c  .|.g.|...}...x.|
+0000af30: 006a 057c 0a83 015c 037d 0b7d 0c7d 0d74  .j.|...\.}.}.}.t
+0000af40: 047c 0b83 017d 117c 0b64 0a19 0064 073e  .|...}.|.d...d.>
+0000af50: 007c 0b64 0619 0017 007d 127c 0b64 0564  .|.d.....}.|.d.d
+0000af60: 057c 1217 0085 0219 007d 137c 107c 1337  .|.......}.|.|.7
+0000af70: 007d 107c 1264 0517 007c 116b 0090 0172  .}.|.d...|.k...r
+0000af80: b27c 1264 0517 007d 147c 0b7c 1419 0064  .|.d...}.|.|...d
+0000af90: 073e 007c 0b7c 1464 0617 0019 0017 007d  .>.|.|.d.......}
+0000afa0: 157c 1464 0537 007d 147c 0b7c 147c 147c  .|.d.7.}.|.|.|.|
+0000afb0: 1517 0085 0219 007d 167c 0e64 1719 007c  .......}.|.d...|
+0000afc0: 1017 007d 177c 1564 186b 0290 0272 6c7c  ...}.|.d.k...rl|
+0000afd0: 167c 0e64 193c 0074 0c7c 1683 016a 0883  .|.d.<.t.|...j..
+0000afe0: 007c 0e64 1a3c 006e 2c7c 006a 0a6a 0d7c  .|.d.<.n,|.j.j.|
+0000aff0: 177c 167c 006a 0a6a 0e83 0301 007c 167c  .|.|.j.j.....|.|
+0000b000: 0e64 1b3c 0074 0c7c 1683 016a 0883 007c  .d.<.t.|...j...|
+0000b010: 0e64 1c3c 007c 177c 0e64 1d3c 0074 0c7c  .d.<.|.|.d.<.t.|
+0000b020: 1783 016a 0883 007c 0e64 1e3c 0050 0090  ...j...|.d.<.P..
+0000b030: 0171 b257 007c 107c 0e64 1f3c 007c 0390  .q.W.|.|.d.<.|..
+0000b040: 0272 d874 0c7c 1083 016a 0883 007c 0e64  .r.t.|...j...|.d
+0000b050: 203c 006e 1074 0c7c 1083 016a 0883 007c   <.n.t.|...j...|
+0000b060: 0e64 213c 007c 0390 0373 4a74 0f6a 1074  .d!<.|...sJt.j.t
+0000b070: 0c7c 1083 0183 016a 1183 0064 0a64 0785  .|.....j...d.d..
+0000b080: 0219 007c 0e64 223c 007c 0e64 2219 007c  ...|.d"<.|.d"..|
+0000b090: 0e64 2319 006b 0290 0372 2a74 006a 0164  .d#..k...r*t.j.d
+0000b0a0: 2483 0101 006e 2074 006a 1264 257c 0e64  $....n t.j.d%|.d
+0000b0b0: 2319 009b 0064 267c 0e64 2219 009b 0064  #....d&|.d"....d
+0000b0c0: 279d 0583 0101 007c 0e53 0029 294e 7a1b  '......|.S.))Nz.
+0000b0d0: 496e 2073 6565 646b 6565 7065 725f 6578  In seedkeeper_ex
+0000b0e0: 706f 7274 5f73 6563 7265 7446 54e9 a200  port_secretFT...
+0000b0f0: 0000 7223 0000 0072 0c00 0000 72b4 0000  ..r#...r....r...
+0000b100: 0072 bc00 0000 7241 0000 0072 0100 0000  .r....rA...r....
+0000b110: 7242 0000 00e9 3100 0000 7a37 4578 706f  rB....1...z7Expo
+0000b120: 7274 2066 6169 6c65 643a 2065 7870 6f72  rt failed: expor
+0000b130: 7420 6e6f 7420 616c 6c6f 7765 6420 6279  t not allowed by
+0000b140: 2053 6565 644b 6565 7065 7220 706f 6c69   SeedKeeper poli
+0000b150: 6379 2e7a 1f45 7870 6f72 7420 6661 696c  cy.z.Export fail
+0000b160: 6564 3a20 7365 6372 6574 206e 6f74 2066  ed: secret not f
+0000b170: 6f75 6e64 72d3 0000 007a 2545 7870 6f72  oundr....z%Expor
+0000b180: 7420 6661 696c 6564 3a20 6c6f 636b 2065  t failed: lock e
+0000b190: 7272 6f72 202d 2074 7279 2061 6761 696e  rror - try again
+0000b1a0: 7a1d 556e 6578 7065 6374 6564 2065 7272  z.Unexpected err
+0000b1b0: 6f72 2028 6572 726f 7220 636f 6465 2072  or (error code r
+0000b1c0: bd00 0000 728a 0000 007a 0349 563a 5a07  ....r....z.IV:Z.
+0000b1d0: 6976 5f6c 6973 7472 eb00 0000 da0b 6865  iv_listr......he
+0000b1e0: 6164 6572 5f6c 6973 7472 0901 0000 5a09  ader_listr....Z.
+0000b1f0: 686d 6163 5f6c 6973 7472 ed00 0000 5a09  hmac_listr....Z.
+0000b200: 7369 676e 5f6c 6973 74da 0473 6967 6e5a  sign_list..signZ
+0000b210: 0e66 756c 6c5f 6461 7461 5f6c 6973 74da  .full_data_list.
+0000b220: 0966 756c 6c5f 6461 7461 72f7 0000 0072  .full_datar....r
+0000b230: ec00 0000 da06 7365 6372 6574 725e 0100  ......secretr^..
+0000b240: 0072 1c01 0000 7a14 4669 6e67 6572 7072  .r....z.Fingerpr
+0000b250: 696e 7473 206d 6174 6368 2021 7a1f 4669  ints match !z.Fi
+0000b260: 6e67 6572 7072 696e 7420 6d69 736d 6174  ngerprint mismat
+0000b270: 6368 3a20 6578 7065 6374 6564 207a 0f20  ch: expected z. 
+0000b280: 6275 7420 7265 636f 7665 7265 6420 7224  but recovered r$
+0000b290: 0000 0069 f0ff ffff 2913 7227 0000 0072  ...i....).r'...r
+0000b2a0: 3400 0000 722b 0000 0072 be00 0000 7235  4...r+...r....r5
+0000b2b0: 0000 0072 9b00 0000 7254 0000 0072 5b01  ...r....rT...r[.
+0000b2c0: 0000 724c 0000 0072 f400 0000 7277 0000  ..rL...r....rw..
+0000b2d0: 00da 1770 6172 7365 5f73 6565 646b 6565  ...parse_seedkee
+0000b2e0: 7065 725f 6865 6164 6572 724b 0000 005a  per_headerrK...Z
+0000b2f0: 1076 6572 6966 795f 7369 676e 6174 7572  .verify_signatur
+0000b300: 6572 a600 0000 724f 0000 0072 3901 0000  er....rO...r9...
+0000b310: 7251 0000 0072 e400 0000 2918 7236 0000  rQ...r....).r6..
+0000b320: 005a 0373 6964 725c 0100 005a 1069 735f  .Z.sidr\...Z.is_
+0000b330: 7365 6375 7265 5f65 7870 6f72 7472 a100  secure_exportr..
+0000b340: 0000 7289 0000 0072 a200 0000 72a3 0000  ..r....r....r...
+0000b350: 0072 cb00 0000 72cc 0000 0072 9a00 0000  .r....r....r....
+0000b360: 7222 0000 0072 5e00 0000 725f 0000 00da  r"...r^...r_....
+0000b370: 0b73 6563 7265 745f 6469 6374 72eb 0000  .secret_dictr...
+0000b380: 0072 6501 0000 5a0d 7265 7370 6f6e 7365  .re...Z.response
+0000b390: 5f73 697a 6572 5d01 0000 7224 0100 00da  _sizer]...r$....
+0000b3a0: 066f 6666 7365 745a 0973 6967 6e5f 7369  .offsetZ.sign_si
+0000b3b0: 7a65 7263 0100 0072 6401 0000 7237 0000  zerc...rd...r7..
+0000b3c0: 0072 3700 0000 7238 0000 00da 1873 6565  .r7...r8.....see
+0000b3d0: 646b 6565 7065 725f 6578 706f 7274 5f73  dkeeper_export_s
+0000b3e0: 6563 7265 746e 0600 0073 8200 0000 0001  ecretn...s......
+0000b3f0: 0a02 1002 0601 0401 0c01 0402 1401 0401  ................
+0000b400: 1801 0801 1203 1001 1001 0201 1001 0a01  ................
+0000b410: 0a01 1001 0a01 0a01 1201 0a02 0a02 1e01  ................
+0000b420: 1c03 0c02 0601 0c01 1601 0801 1002 0401  ................
+0000b430: 0401 1201 0402 1002 0801 1401 1001 0803  ................
+0000b440: 0e01 0801 1801 0801 1003 0c01 0a01 0801  ................
+0000b450: 1202 1401 0801 1001 0801 1001 0801 0801  ................
+0000b460: 0601 1202 1005 0601 1e01 1201 0c02 2002  .............. .
+0000b470: 7a26 4361 7264 436f 6e6e 6563 746f 722e  z&CardConnector.
+0000b480: 7365 6564 6b65 6570 6572 5f65 7870 6f72  seedkeeper_expor
+0000b490: 745f 7365 6372 6574 6301 0000 0000 0000  t_secretc.......
+0000b4a0: 000b 0000 0005 0000 0043 0000 0073 2401  .........C...s$.
+0000b4b0: 0000 7400 6a01 6401 8301 0100 7402 6a03  ..t.j.d.....t.j.
+0000b4c0: 7d01 6402 7d02 6403 7d03 6700 7d04 6404  }.d.}.d.}.g.}.d.
+0000b4d0: 7d05 7c01 7c02 7c03 7c05 6704 7d06 7c00  }.|.|.|.|.g.}.|.
+0000b4e0: 6a04 7c06 8301 5c03 7d07 7d08 7d09 784a  j.|...\.}.}.}.xJ
+0000b4f0: 7c08 6405 6b02 7286 7c09 6403 6b02 7286  |.d.k.r.|.d.k.r.
+0000b500: 7c00 6a05 6a06 7c07 8301 7d0a 7c04 7c0a  |.j.j.|...}.|.|.
+0000b510: 6701 3700 7d04 6406 7d05 7c01 7c02 7c03  g.7.}.d.}.|.|.|.
+0000b520: 7c05 6704 7d06 7c00 6a04 7c06 8301 5c03  |.g.}.|.j.|...\.
+0000b530: 7d07 7d08 7d09 713e 5700 7c08 6405 6b02  }.}.}.q>W.|.d.k.
+0000b540: 729a 7c09 6403 6b02 729a 6e86 7c08 6407  r.|.d.k.r.n.|.d.
+0000b550: 6b02 72b6 7c09 6408 6b02 72b6 7400 6a01  k.r.|.d.k.r.t.j.
+0000b560: 6409 8301 0100 6e6a 7c08 6407 6b02 72e6  d.....nj|.d.k.r.
+0000b570: 7c09 640a 6b02 72e6 7400 6a07 640b 7c08  |.d.k.r.t.j.d.|.
+0000b580: 9b00 640c 7c09 9b00 9d04 8301 0100 7408  ..d.|.........t.
+0000b590: 640d 8301 8201 6e3a 7400 6a07 640e 7409  d.....n:t.j.d.t.
+0000b5a0: 640f 7c08 1400 7c09 1700 8301 9b00 6410  d.|...|.......d.
+0000b5b0: 9d03 8301 0100 740a 640e 7409 640f 7c08  ......t.d.t.d.|.
+0000b5c0: 1400 7c09 1700 8301 9b00 6410 9d03 8301  ..|.......d.....
+0000b5d0: 8201 7c04 5300 2911 4e7a 2149 6e20 7365  ..|.S.).Nz!In se
+0000b5e0: 6564 6b65 6570 6572 5f6c 6973 745f 7365  edkeeper_list_se
+0000b5f0: 6372 6574 5f68 6561 6465 7273 e9a6 0000  cret_headers....
+0000b600: 0072 0100 0000 720c 0000 0072 4100 0000  .r....r....rA...
+0000b610: 7223 0000 0072 4200 0000 7251 0100 007a  r#...rB...rQ...z
+0000b620: 184e 6f20 6d6f 7265 206f 626a 6563 7420  .No more object 
+0000b630: 696e 206d 656d 6f72 7972 4300 0000 7a2e  in memoryrC...z.
+0000b640: 556e 696e 6974 6961 6c69 7a65 6453 6565  UninitializedSee
+0000b650: 6445 7272 6f72 2064 7572 696e 6720 6f62  dError during ob
+0000b660: 6a65 6374 206c 6973 7469 6e67 3a20 7224  ject listing: r$
+0000b670: 0000 007a 1e53 6565 644b 6565 7065 7220  ...z.SeedKeeper 
+0000b680: 6973 206e 6f74 2069 6e69 7469 616c 697a  is not initializ
+0000b690: 6564 217a 3355 6e65 7870 6563 7465 6420  ed!z3Unexpected 
+0000b6a0: 6572 726f 7220 6475 7269 6e67 206f 626a  error during obj
+0000b6b0: 6563 7420 6c69 7374 696e 6720 2865 7272  ect listing (err
+0000b6c0: 6f72 2063 6f64 6520 72bc 0000 0072 bd00  or code r....r..
+0000b6d0: 0000 290b 7227 0000 0072 3400 0000 722b  ..).r'...r4...r+
+0000b6e0: 0000 0072 be00 0000 729b 0000 0072 7700  ...r....r....rw.
+0000b6f0: 0000 7266 0100 0072 5400 0000 7204 0100  ..rf...rT...r...
+0000b700: 0072 4c00 0000 72f4 0000 0029 0b72 3600  .rL...r....).r6.
+0000b710: 0000 72a1 0000 0072 8900 0000 72a2 0000  ..r....r....r...
+0000b720: 005a 0768 6561 6465 7273 72a3 0000 0072  .Z.headersr....r
+0000b730: 9a00 0000 7222 0000 0072 5e00 0000 725f  ....r"...r^...r_
+0000b740: 0000 0072 6701 0000 7237 0000 0072 3700  ...rg...r7...r7.
+0000b750: 0000 7238 0000 00da 1e73 6565 646b 6565  ..r8.....seedkee
+0000b760: 7065 725f 6c69 7374 5f73 6563 7265 745f  per_list_secret_
+0000b770: 6865 6164 6572 73ca 0600 0073 3000 0000  headers....s0...
+0000b780: 0001 0a01 0601 0401 0403 0401 0401 0c01  ................
+0000b790: 1002 1201 0c01 0a04 0401 0c01 1402 1001  ................
+0000b7a0: 0201 1001 0c01 1001 1601 0a02 1e01 1c02  ................
+0000b7b0: 7a2c 4361 7264 436f 6e6e 6563 746f 722e  z,CardConnector.
+0000b7c0: 7365 6564 6b65 6570 6572 5f6c 6973 745f  seedkeeper_list_
+0000b7d0: 7365 6372 6574 5f68 6561 6465 7273 6302  secret_headersc.
+0000b7e0: 0000 0000 0000 0015 0000 000d 0000 0043  ...............C
+0000b7f0: 0000 0073 f602 0000 7400 6a01 6401 8301  ...s....t.j.d...
+0000b800: 0100 7402 6a03 7d02 6402 7d03 6403 7d04  ..t.j.}.d.}.d.}.
+0000b810: 6404 7d05 7c02 7c03 7c04 7c05 6704 7d06  d.}.|.|.|.|.g.}.
+0000b820: 7c00 6a04 7c06 8301 5c03 7d07 7d08 7d09  |.j.|...\.}.}.}.
+0000b830: 6700 7d0a 6405 7d0b 7c08 6406 6b02 6f4e  g.}.d.}.|.d.k.oN
+0000b840: 7c09 6403 6b02 9001 7204 7c07 6403 1900  |.d.k...r.|.d...
+0000b850: 6407 1400 7c07 6404 1900 1700 7d0c 7c07  d...|.d.....}.|.
+0000b860: 6408 1900 6407 1400 7c07 6409 1900 1700  d...d...|.d.....
+0000b870: 7d0d 7400 6a01 640a 7405 7c0c 8301 1700  }.t.j.d.t.|.....
+0000b880: 8301 0100 7400 6a01 640b 7405 7c0d 8301  ....t.j.d.t.|...
+0000b890: 1700 8301 0100 7406 7c07 8301 640c 7c0b  ......t.|...d.|.
+0000b8a0: 1700 6b05 72f8 7c00 6a07 6a08 7c07 640c  ..k.r.|.j.j.|.d.
+0000b8b0: 640c 7c0b 1700 8502 1900 8301 5c04 7d0e  d.|.........\.}.
+0000b8c0: 7d0f 7d10 7d11 7c0a 7c0e 7c0f 7c10 7c11  }.}.}.|.|.|.|.|.
+0000b8d0: 6704 6701 1700 7d0a 7400 6a01 640d 7405  g.g...}.t.j.d.t.
+0000b8e0: 7c0a 6403 1900 8301 1700 8301 0100 6e0a  |.d...........n.
+0000b8f0: 7400 6a01 640e 8301 0100 6e6e 7c08 640f  t.j.d.....nn|.d.
+0000b900: 6b02 9001 7238 7c09 640c 6b02 9001 7238  k...r8|.d.k...r8
+0000b910: 7400 6a09 6410 7c08 9b00 6411 7c09 9b00  t.j.d.|...d.|...
+0000b920: 9d04 8301 0100 740a 6412 8301 8201 6e3a  ......t.d.....n:
+0000b930: 7400 6a09 6413 740b 6407 7c08 1400 7c09  t.j.d.t.d.|...|.
+0000b940: 1700 8301 9b00 6414 9d03 8301 0100 740c  ......d.......t.
+0000b950: 6413 740b 6407 7c08 1400 7c09 1700 8301  d.t.d.|...|.....
+0000b960: 9b00 6414 9d03 8301 8201 6408 7d05 7c02  ..d.......d.}.|.
+0000b970: 7c03 7c04 7c05 6704 7d06 6403 7d12 78ce  |.|.|.g.}.d.}.x.
+0000b980: 7c01 9002 7254 7c08 6406 6b02 9002 7254  |...rT|.d.k...rT
+0000b990: 7c09 6403 6b02 9002 7254 7c00 6a04 7c06  |.d.k...rT|.j.|.
+0000b9a0: 8301 5c03 7d07 7d08 7d09 7406 7c07 8301  ..\.}.}.}.t.|...
+0000b9b0: 6403 6b02 9001 72c2 5000 7868 7406 7c07  d.k...r.P.xht.|.
+0000b9c0: 8301 7c0b 6b05 9002 722a 7c00 6a07 6a08  ..|.k...r*|.j.j.
+0000b9d0: 7c07 6403 7c0b 8502 1900 8301 5c04 7d0e  |.d.|.......\.}.
+0000b9e0: 7d0f 7d10 7d11 7400 6a01 6415 7405 7c0e  }.}.}.t.j.d.t.|.
+0000b9f0: 7c0f 7c10 7c11 6704 8301 1700 8301 0100  |.|.|.g.........
+0000ba00: 7c0a 7c0e 7c0f 7c10 7c11 6704 6701 1700  |.|.|.|.|.g.g...
+0000ba10: 7d0a 7c07 7c0b 6400 8502 1900 7d07 9001  }.|.|.d.....}...
+0000ba20: 71c4 5700 7c12 6404 3700 7d12 7c12 6416  q.W.|.d.7.}.|.d.
+0000ba30: 6b04 9001 7288 7400 6a09 6417 7c12 9b00  k...r.t.j.d.|...
+0000ba40: 9d02 8301 0100 5000 9001 7188 5700 7c08  ......P...q.W.|.
+0000ba50: 6406 6b03 9002 736a 7c09 6403 6b03 9002  d.k...sj|.d.k...
+0000ba60: 7280 7400 6a09 6418 7c08 9b00 6411 7c09  r.t.j.d.|...d.|.
+0000ba70: 9b00 9d04 8301 0100 7400 6a01 6419 7406  ........t.j.d.t.
+0000ba80: 7c0a 8301 9b00 9d02 8301 0100 6403 7d13  |...........d.}.
+0000ba90: 7852 7c0a 4400 5d4a 7d14 7c14 5c04 7d0e  xR|.D.]J}.|.\.}.
+0000baa0: 7d0f 7d10 7d11 7400 6a01 641a 7c13 9b00  }.}.}.t.j.d.|...
+0000bab0: 641b 740b 7c0e 8301 9b00 6411 7c0f 9b00  d.t.|.....d.|...
+0000bac0: 6411 7c10 9b00 6411 740b 7c11 8301 9b00  d.|...d.t.|.....
+0000bad0: 9d0a 8301 0100 7c13 6404 3700 7d13 9002  ......|.d.7.}...
+0000bae0: 719e 5700 7c0a 7c0c 7c0d 6603 5300 291c  q.W.|.|.|.f.S.).
+0000baf0: 4e7a 1849 6e20 7365 6564 6b65 6570 6572  Nz.In seedkeeper
+0000bb00: 5f70 7269 6e74 5f6c 6f67 73e9 a900 0000  _print_logs.....
+0000bb10: 7201 0000 0072 0c00 0000 72b7 0000 0072  r....r....r....r
+0000bb20: 4100 0000 72bc 0000 0072 2300 0000 72b3  A...r....r#...r.
+0000bb30: 0000 007a 0e6e 6274 6f74 616c 5f6c 6f67  ...z.nbtotal_log
+0000bb40: 733a 207a 0e6e 6261 7661 696c 5f6c 6f67  s: z.nbavail_log
+0000bb50: 733a 2072 4300 0000 7a0c 4c61 7465 7374  s: rC...z.Latest
+0000bb60: 206c 6f67 3a20 7a12 4e6f 206c 6f67 7320   log: z.No logs 
+0000bb70: 6176 6169 6c61 626c 6521 7242 0000 007a  available!rB...z
+0000bb80: 2e55 6e69 6e69 7469 616c 697a 6564 5365  .UninitializedSe
+0000bb90: 6564 4572 726f 7220 6475 7269 6e67 206f  edError during o
+0000bba0: 626a 6563 7420 6c69 7374 696e 673a 2072  bject listing: r
+0000bbb0: 2400 0000 7a1e 5365 6564 4b65 6570 6572  $...z.SeedKeeper
+0000bbc0: 2069 7320 6e6f 7420 696e 6974 6961 6c69   is not initiali
+0000bbd0: 7a65 6421 7a33 556e 6578 7065 6374 6564  zed!z3Unexpected
+0000bbe0: 2065 7272 6f72 2064 7572 696e 6720 6f62   error during ob
+0000bbf0: 6a65 6374 206c 6973 7469 6e67 2028 6572  ject listing (er
+0000bc00: 726f 7220 636f 6465 2072 bd00 0000 7a0a  ror code r....z.
+0000bc10: 4e65 7874 206c 6f67 3a20 726f 0000 007a  Next log: ro...z
+0000bc20: 2643 6f75 6e74 6572 2065 7863 6565 6465  &Counter exceede
+0000bc30: 6420 6475 7269 6e67 206c 6f67 2070 7269  d during log pri
+0000bc40: 6e74 696e 673a 207a 1b45 7272 6f72 2064  nting: z.Error d
+0000bc50: 7572 696e 6720 6c6f 6720 7072 696e 7469  uring log printi
+0000bc60: 6e67 3a20 7a0b 4c4f 4753 2073 697a 653a  ng: z.LOGS size:
+0000bc70: 207a 0769 6e64 6578 3a20 7a03 207c 2029   z.index: z. | )
+0000bc80: 0d72 2700 0000 7234 0000 0072 2b00 0000  .r'...r4...r+...
+0000bc90: 72be 0000 0072 9b00 0000 7276 0000 0072  r....r....rv...r
+0000bca0: 3500 0000 7277 0000 005a 1470 6172 7365  5...rw...Z.parse
+0000bcb0: 5f73 6565 646b 6565 7065 725f 6c6f 6772  _seedkeeper_logr
+0000bcc0: 5400 0000 7204 0100 0072 4c00 0000 72f4  T...r....rL...r.
+0000bcd0: 0000 0029 1572 3600 0000 5a09 7072 696e  ...).r6...Z.prin
+0000bce0: 745f 616c 6c72 a100 0000 7289 0000 0072  t_allr....r....r
+0000bcf0: a200 0000 72a3 0000 0072 9a00 0000 7222  ....r....r....r"
+0000bd00: 0000 0072 5e00 0000 725f 0000 005a 046c  ...r^...r_...Z.l
+0000bd10: 6f67 735a 086c 6f67 5f73 697a 655a 0c6e  ogsZ.log_sizeZ.n
+0000bd20: 6274 6f74 616c 5f6c 6f67 735a 0c6e 6261  btotal_logsZ.nba
+0000bd30: 7661 696c 5f6c 6f67 735a 056f 7069 6e73  vail_logsZ.opins
+0000bd40: 5a03 6964 315a 0369 6432 da03 7265 735a  Z.id1Z.id2..resZ
+0000bd50: 0763 6f75 6e74 6572 72dd 0000 00da 036c  .counterr......l
+0000bd60: 6f67 7237 0000 0072 3700 0000 7238 0000  ogr7...r7...r8..
+0000bd70: 00da 1573 6565 646b 6565 7065 725f 7072  ...seedkeeper_pr
+0000bd80: 696e 745f 6c6f 6773 ed06 0000 7362 0000  int_logs....sb..
+0000bd90: 0000 010a 0106 0104 0104 0304 010c 0110  ................
+0000bda0: 0304 0104 0112 0114 0114 0112 0112 0110  ................
+0000bdb0: 0120 0112 0118 020c 0114 0116 010a 021e  . ..............
+0000bdc0: 011c 0304 010c 0104 011c 0210 010e 0102  ................
+0000bdd0: 0210 011c 011a 0112 0112 0208 010a 0110  ................
+0000bde0: 0108 0214 0116 0314 0104 010a 010c 0130  ...............0
+0000bdf0: 010e 027a 2343 6172 6443 6f6e 6e65 6374  ...z#CardConnect
+0000be00: 6f72 2e73 6565 646b 6565 7065 725f 7072  or.seedkeeper_pr
+0000be10: 696e 745f 6c6f 6773 6304 0000 0000 0000  int_logsc.......
+0000be20: 0011 0000 000a 0000 0043 0000 0073 cc00  .........C...s..
+0000be30: 0000 6401 6402 6403 6404 6405 6405 6406  ..d.d.d.d.d.d.d.
+0000be40: 6407 6408 6409 9c09 7d04 640a 640b 640c  d.d.d...}.d.d.d.
+0000be50: 9c02 7d05 640b 6404 6701 1400 7d06 7400  ..}.d.d.g...}.t.
+0000be60: 7c01 8301 7401 6b08 7242 7c04 7c01 1900  |...t.k.rB|.|...
+0000be70: 7d07 6e04 7c01 7d07 6404 7d08 7400 7c02  }.n.|.}.d.}.t.|.
+0000be80: 8301 7401 6b08 7260 7c05 7c02 1900 7d09  ..t.k.r`|.|...}.
+0000be90: 6e04 7c02 7d09 640d 6404 6701 1400 7d0a  n.|.}.d.d.g...}.
+0000bea0: 640e 6404 6701 1400 7d0b 640b 6404 6701  d.d.g...}.d.d.g.
+0000beb0: 1400 7d0c 7402 7c03 8301 7d0d 7403 7c03  ..}.t.|...}.t.|.
+0000bec0: 6a04 640f 8301 8301 7d0e 7c06 7c07 7c08  j.d.....}.|.|.|.
+0000bed0: 7c09 6703 1700 7c0a 1700 7c0b 1700 7c0c  |.g...|...|...|.
+0000bee0: 1700 7c0d 6701 1700 7c0e 1700 7d0f 7405  ..|.g...|...}.t.
+0000bef0: 7c0f 8301 6a06 8300 7d10 7c10 5300 2910  |...j...}.|.S.).
+0000bf00: 4e72 d300 0000 720e 0100 0072 8a00 0000  Nr....r....r....
+0000bf10: 7201 0000 0072 6d00 0000 7241 0000 0072  r....rm...rA...r
+0000bf20: 5301 0000 72f2 0000 0029 097a 0e42 4950  S...r....).z.BIP
+0000bf30: 3339 206d 6e65 6d6f 6e69 637a 1145 6c65  39 mnemonicz.Ele
+0000bf40: 6374 7275 6d20 6d6e 656d 6f6e 6963 5a0a  ctrum mnemonicZ.
+0000bf50: 4d61 7374 6572 7365 6564 7a17 5365 6375  Masterseedz.Secu
+0000bf60: 7265 2069 6d70 6f72 7420 6672 6f6d 206a  re import from j
+0000bf70: 736f 6e7a 0a50 7562 6c69 6320 4b65 797a  sonz.Public Keyz
+0000bf80: 1b41 7574 6865 6e74 696b 6579 2066 726f  .Authentikey fro
+0000bf90: 6d20 5472 7573 7453 746f 7265 5a08 5061  m TrustStoreZ.Pa
+0000bfa0: 7373 776f 7264 7a17 4175 7468 656e 7469  sswordz.Authenti
+0000bfb0: 6b65 7920 6365 7274 6966 6963 6174 657a  key certificatez
+0000bfc0: 0a32 4641 2073 6563 7265 7472 0c00 0000  .2FA secretr....
+0000bfd0: 7223 0000 0029 027a 1b45 7870 6f72 7420  r#...).z.Export 
+0000bfe0: 696e 2070 6c61 696e 7465 7874 2061 6c6c  in plaintext all
+0000bff0: 6f77 6564 7a15 4578 706f 7274 2065 6e63  owedz.Export enc
+0000c000: 7279 7074 6564 206f 6e6c 7972 b300 0000  rypted onlyr....
+0000c010: 7243 0000 0072 c100 0000 2907 7226 0000  rC...r....).r&..
+0000c020: 0072 7600 0000 7235 0000 0072 c800 0000  .rv...r5...r....
+0000c030: 72c9 0000 0072 4b00 0000 724c 0000 0029  r....rK...rL...)
+0000c040: 1172 3600 0000 72f8 0000 0072 5401 0000  .r6...r....rT...
+0000c050: 72c5 0000 005a 0864 6963 5f74 7970 655a  r....Z.dic_typeZ
+0000c060: 1164 6963 5f65 7870 6f72 745f 7269 6768  .dic_export_righ
+0000c070: 7473 7255 0100 005a 0569 7479 7065 da06  tsrU...Z.itype..
+0000c080: 6f72 6967 696e 5a06 6578 706f 7274 5a0f  originZ.exportZ.
+0000c090: 6578 706f 7274 5f63 6f75 6e74 6572 7372  export_countersr
+0000c0a0: 1c01 0000 5a03 7266 7572 c400 0000 72ca  ....Z.rfur....r.
+0000c0b0: 0000 0072 6201 0000 5a0a 6865 6164 6572  ...rb...Z.header
+0000c0c0: 5f68 6578 7237 0000 0072 3700 0000 7238  _hexr7...r7...r8
+0000c0d0: 0000 00da 0b6d 616b 655f 6865 6164 6572  .....make_header
+0000c0e0: 2f07 0000 7326 0000 0000 0108 0110 010a  /...s&..........
+0000c0f0: 010a 010c 010a 0204 0104 010c 010a 0204  ................
+0000c100: 010a 010a 010a 0108 010e 0124 010c 017a  ...........$...z
+0000c110: 1943 6172 6443 6f6e 6e65 6374 6f72 2e6d  .CardConnector.m
+0000c120: 616b 655f 6865 6164 6572 6301 0000 0000  ake_headerc.....
+0000c130: 0000 0009 0000 0005 0000 0043 0000 0073  ...........C...s
+0000c140: ae00 0000 7400 6a01 6401 8301 0100 7402  ....t.j.d.....t.
+0000c150: 6a03 7d01 7402 6a04 7d02 6402 7d03 6402  j.}.t.j.}.d.}.d.
+0000c160: 7d04 7c01 7c02 7c03 7c04 6704 7d05 7c00  }.|.|.|.|.g.}.|.
+0000c170: 6a05 7c05 8301 5c03 7d06 7d07 7d08 7c07  j.|...\.}.}.}.|.
+0000c180: 6403 6b02 724c 7c08 6402 6b02 724c 6e5e  d.k.rL|.d.k.rLn^
+0000c190: 7c07 6404 6b02 7270 7c08 6402 6b02 7270  |.d.k.rp|.d.k.rp
+0000c1a0: 7400 6a06 6405 8301 0100 7407 6406 8301  t.j.d.....t.d...
+0000c1b0: 8201 6e3a 7400 6a06 6407 7408 6408 7c07  ..n:t.j.d.t.d.|.
+0000c1c0: 1400 7c08 1700 8301 9b00 6409 9d03 8301  ..|.......d.....
+0000c1d0: 0100 7409 6407 7408 6408 7c07 1400 7c08  ..t.d.t.d.|...|.
+0000c1e0: 1700 8301 9b00 6409 9d03 8301 8201 7c06  ......d.......|.
+0000c1f0: 5300 290a 4e7a 1b49 6e20 6361 7264 5f65  S.).Nz.In card_e
+0000c200: 7870 6f72 745f 7065 7273 6f5f 7075 626b  xport_perso_pubk
+0000c210: 6579 7201 0000 0072 4100 0000 7273 0000  eyr....rA...rs..
+0000c220: 007a 4645 7272 6f72 2064 7572 696e 6720  .zFError during 
+0000c230: 7065 7273 6f6e 616c 697a 6174 696f 6e20  personalization 
+0000c240: 7075 626b 6579 2065 7870 6f72 743a 2063  pubkey export: c
+0000c250: 6f6d 6d61 6e64 2075 6e73 7570 706f 7274  ommand unsupport
+0000c260: 6564 2830 7836 4430 307a 4845 7272 6f72  ed(0x6D00zHError
+0000c270: 2064 7572 696e 6720 7065 7273 6f6e 616c   during personal
+0000c280: 697a 6174 696f 6e20 7075 626b 6579 2065  ization pubkey e
+0000c290: 7870 6f72 743a 2063 6f6d 6d61 6e64 2075  xport: command u
+0000c2a0: 6e73 7570 706f 7274 6564 2028 3078 3644  nsupported (0x6D
+0000c2b0: 3030 297a 3745 7272 6f72 2064 7572 696e  00)z7Error durin
+0000c2c0: 6720 7065 7273 6f6e 616c 697a 6174 696f  g personalizatio
+0000c2d0: 6e20 7075 626b 6579 2065 7870 6f72 7420  n pubkey export 
+0000c2e0: 2865 7272 6f72 2063 6f64 6520 72bc 0000  (error code r...
+0000c2f0: 0072 bd00 0000 290a 7227 0000 0072 3400  .r....).r'...r4.
+0000c300: 0000 722b 0000 0072 be00 0000 5a15 494e  ..r+...r....Z.IN
+0000c310: 535f 4558 504f 5254 5f50 4b49 5f50 5542  S_EXPORT_PKI_PUB
+0000c320: 4b45 5972 9b00 0000 72e4 0000 0072 e500  KEYr....r....r..
+0000c330: 0000 724c 0000 0072 f400 0000 2909 7236  ..rL...r....).r6
+0000c340: 0000 0072 a100 0000 7289 0000 0072 a200  ...r....r....r..
+0000c350: 0000 72a3 0000 0072 9a00 0000 7222 0000  ..r....r....r"..
+0000c360: 0072 5e00 0000 725f 0000 0072 3700 0000  .r^...r_...r7...
+0000c370: 7237 0000 0072 3800 0000 da18 6361 7264  r7...r8.....card
+0000c380: 5f65 7870 6f72 745f 7065 7273 6f5f 7075  _export_perso_pu
+0000c390: 626b 6579 4907 0000 731e 0000 0000 010a  bkeyI...s.......
+0000c3a0: 0106 0106 0104 0104 010c 0110 0110 0102  ................
+0000c3b0: 0110 010a 010a 021e 011c 017a 2643 6172  ...........z&Car
+0000c3c0: 6443 6f6e 6e65 6374 6f72 2e63 6172 645f  dConnector.card_
+0000c3d0: 6578 706f 7274 5f70 6572 736f 5f70 7562  export_perso_pub
+0000c3e0: 6b65 7963 0100 0000 0000 0000 1000 0000  keyc............
+0000c3f0: 0600 0000 4300 0000 730e 0200 0074 006a  ....C...s....t.j
+0000c400: 0164 0183 0101 0074 026a 037d 0174 026a  .d.....t.j.}.t.j
+0000c410: 047d 0264 027d 0364 037d 047c 017c 027c  .}.d.}.d.}.|.|.|
+0000c420: 037c 0467 047d 057c 006a 057c 0583 015c  .|.g.}.|.j.|...\
+0000c430: 037d 067d 077d 087c 0764 046b 0272 4c7c  .}.}.}.|.d.k.rL|
+0000c440: 0864 026b 0272 4c6e 827c 0764 056b 0272  .d.k.rLn.|.d.k.r
+0000c450: 707c 0864 026b 0272 7074 006a 0664 0683  p|.d.k.rpt.j.d..
+0000c460: 0101 0074 0764 0783 0182 016e 5e7c 0764  ...t.d.....n^|.d
+0000c470: 026b 0272 947c 0864 026b 0272 9474 006a  .k.r.|.d.k.r.t.j
+0000c480: 0664 0883 0101 0074 0864 0983 0182 016e  .d.....t.d.....n
+0000c490: 3a74 006a 0664 0a74 0964 0b7c 0714 007c  :t.j.d.t.d.|...|
+0000c4a0: 0817 0083 019b 0064 0c9d 0383 0101 0074  .......d.......t
+0000c4b0: 0a64 0a74 0964 0b7c 0714 007c 0817 0083  .d.t.d.|...|....
+0000c4c0: 019b 0064 0c9d 0383 0182 017c 0664 0219  ...d.......|.d..
+0000c4d0: 0064 0d40 0064 0b14 007c 0664 0319 0064  .d.@.d...|.d...d
+0000c4e0: 0d40 0017 007d 097c 0964 026b 0272 f664  .@...}.|.d.k.r.d
+0000c4f0: 0e53 0064 0f7d 047c 0964 0267 0114 007d  .S.d.}.|.d.g...}
+0000c500: 0a64 107d 0b67 007d 0c7c 097d 0d64 027d  .d.}.g.}.|.}.d.}
+0000c510: 0e78 827c 0d64 106b 0490 0172 967c 0e64  .x.|.d.k...r.|.d
+0000c520: 113f 0064 0d40 007c 0e64 0d40 0067 027d  .?.d.@.|.d.@.g.}
+0000c530: 0f7c 0f64 027c 0b64 0d40 0067 0237 007d  .|.d.|.d.@.g.7.}
+0000c540: 0f7c 017c 027c 037c 0474 0b7c 0f83 0167  .|.|.|.|.t.|...g
+0000c550: 057c 0f17 007d 057c 006a 057c 0583 015c  .|...}.|.j.|...\
+0000c560: 037d 067d 077d 087c 0664 027c 0b85 0219  .}.}.}.|.d.|....
+0000c570: 007c 0a7c 0e7c 0e7c 0b17 0085 023c 007c  .|.|.|.|.....<.|
+0000c580: 0d7c 0b38 007d 0d7c 0e7c 0b37 007d 0e90  .|.8.}.|.|.7.}..
+0000c590: 0171 1657 007c 0e64 113f 0064 0d40 007c  .q.W.|.d.?.d.@.|
+0000c5a0: 0e64 0d40 0067 027d 0f7c 0f64 027c 0d64  .d.@.g.}.|.d.|.d
+0000c5b0: 0d40 0067 0237 007d 0f7c 017c 027c 037c  .@.g.7.}.|.|.|.|
+0000c5c0: 0474 0b7c 0f83 0167 057c 0f17 007d 057c  .t.|...g.|...}.|
+0000c5d0: 006a 057c 0583 015c 037d 067d 077d 087c  .j.|...\.}.}.}.|
+0000c5e0: 0664 027c 0d85 0219 007c 0a7c 0e7c 0e7c  .d.|.....|.|.|.|
+0000c5f0: 0d17 0085 023c 007c 006a 0c6a 0d7c 0a83  .....<.|.j.j.|..
+0000c600: 017c 005f 0e7c 006a 0e53 0029 124e 7a20  .|._.|.j.S.).Nz 
+0000c610: 496e 2063 6172 645f 6578 706f 7274 5f70  In card_export_p
+0000c620: 6572 736f 5f63 6572 7469 6669 6361 7465  erso_certificate
+0000c630: 7201 0000 0072 0c00 0000 7241 0000 0072  r....r....rA...r
+0000c640: 7300 0000 7a4c 4572 726f 7220 6475 7269  s...zLError duri
+0000c650: 6e67 2070 6572 736f 6e61 6c69 7a61 7469  ng personalizati
+0000c660: 6f6e 2063 6572 7469 6669 6361 7465 2065  on certificate e
+0000c670: 7870 6f72 743a 2063 6f6d 6d61 6e64 2075  xport: command u
+0000c680: 6e73 7570 706f 7274 6564 2830 7836 4430  nsupported(0x6D0
+0000c690: 3029 7a4d 4572 726f 7220 6475 7269 6e67  0)zMError during
+0000c6a0: 2070 6572 736f 6e61 6c69 7a61 7469 6f6e   personalization
+0000c6b0: 2063 6572 7469 6669 6361 7465 2065 7870   certificate exp
+0000c6c0: 6f72 743a 2063 6f6d 6d61 6e64 2075 6e73  ort: command uns
+0000c6d0: 7570 706f 7274 6564 2028 3078 3644 3030  upported (0x6D00
+0000c6e0: 297a 4845 7272 6f72 2064 7572 696e 6720  )zHError during 
+0000c6f0: 7065 7273 6f6e 616c 697a 6174 696f 6e20  personalization 
+0000c700: 6365 7274 6966 6963 6174 6520 6578 706f  certificate expo
+0000c710: 7274 3a20 6e6f 2063 6172 6420 7072 6573  rt: no card pres
+0000c720: 656e 7428 3078 3030 3030 297a 4945 7272  ent(0x0000)zIErr
+0000c730: 6f72 2064 7572 696e 6720 7065 7273 6f6e  or during person
+0000c740: 616c 697a 6174 696f 6e20 6365 7274 6966  alization certif
+0000c750: 6963 6174 6520 6578 706f 7274 3a20 6e6f  icate export: no
+0000c760: 2063 6172 6420 7072 6573 656e 7420 2830   card present (0
+0000c770: 7830 3030 3029 7a3d 4572 726f 7220 6475  x0000)z=Error du
+0000c780: 7269 6e67 2070 6572 736f 6e61 6c69 7a61  ring personaliza
+0000c790: 7469 6f6e 2063 6572 7469 6669 6361 7465  tion certificate
+0000c7a0: 2065 7870 6f72 743a 2028 6572 726f 7220   export: (error 
+0000c7b0: 636f 6465 2072 bc00 0000 72bd 0000 0072  code r....r....r
+0000c7c0: d500 0000 7a07 2865 6d70 7479 2972 2300  ....z.(empty)r#.
+0000c7d0: 0000 729d 0000 0072 b400 0000 290f 7227  ..r....r....).r'
+0000c7e0: 0000 0072 3400 0000 722b 0000 0072 be00  ...r4...r+...r..
+0000c7f0: 0000 5a1a 494e 535f 4558 504f 5254 5f50  ..Z.INS_EXPORT_P
+0000c800: 4b49 5f43 4552 5449 4649 4341 5445 729b  KI_CERTIFICATEr.
+0000c810: 0000 0072 e400 0000 72e5 0000 0072 9900  ...r....r....r..
+0000c820: 0000 724c 0000 0072 f400 0000 7235 0000  ..rL...r....r5..
+0000c830: 0072 7700 0000 5a1b 636f 6e76 6572 745f  .rw...Z.convert_
+0000c840: 6279 7465 735f 746f 5f73 7472 696e 675f  bytes_to_string_
+0000c850: 7065 6d72 8400 0000 2910 7236 0000 0072  pemr....).r6...r
+0000c860: a100 0000 7289 0000 0072 a200 0000 72a3  ....r....r....r.
+0000c870: 0000 0072 9a00 0000 7222 0000 0072 5e00  ...r....r"...r^.
+0000c880: 0000 725f 0000 005a 1063 6572 7469 6669  ..r_...Z.certifi
+0000c890: 6361 7465 5f73 697a 655a 0b63 6572 7469  cate_sizeZ.certi
+0000c8a0: 6669 6361 7465 725d 0100 0072 2401 0000  ficater]...r$...
+0000c8b0: 5a0e 7265 6d61 696e 696e 675f 7369 7a65  Z.remaining_size
+0000c8c0: 5a0b 6365 7274 5f6f 6666 7365 7472 cb00  Z.cert_offsetr..
+0000c8d0: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
+0000c8e0: 00da 1d63 6172 645f 6578 706f 7274 5f70  ...card_export_p
+0000c8f0: 6572 736f 5f63 6572 7469 6669 6361 7465  erso_certificate
+0000c900: 5b07 0000 7352 0000 0000 010a 0106 0106  [...sR..........
+0000c910: 0104 0104 030c 0110 0110 0102 0110 010a  ................
+0000c920: 010a 0110 010a 010a 021e 011c 021c 0108  ................
+0000c930: 0104 0304 010a 0104 0104 0104 0104 010c  ................
+0000c940: 0214 0110 0116 0110 0118 0108 010e 0314  ................
+0000c950: 0110 0116 0110 0118 030e 017a 2b43 6172  ...........z+Car
+0000c960: 6443 6f6e 6e65 6374 6f72 2e63 6172 645f  dConnector.card_
+0000c970: 6578 706f 7274 5f70 6572 736f 5f63 6572  export_perso_cer
+0000c980: 7469 6669 6361 7465 6302 0000 0000 0000  tificatec.......
+0000c990: 000c 0000 0006 0000 0043 0000 0073 6400  .........C...sd.
+0000c9a0: 0000 7400 6a01 6401 8301 0100 7402 6a03  ..t.j.d.....t.j.
+0000c9b0: 7d02 7402 6a04 7d03 6402 7d04 6402 7d05  }.t.j.}.d.}.d.}.
+0000c9c0: 7405 6403 8301 7d06 7c02 7c03 7c04 7c05  t.d...}.|.|.|.|.
+0000c9d0: 7406 7c06 8301 6705 7407 7c06 8301 1700  t.|...g.t.|.....
+0000c9e0: 7d07 7c00 6a08 7c07 8301 5c03 7d08 7d09  }.|.j.|...\.}.}.
+0000c9f0: 7d0a 7c00 6a09 6a0a 7c08 7c06 7c01 8303  }.|.j.j.|.|.|...
+0000ca00: 7d0b 7c0b 5300 2904 4e7a 1e49 6e20 6361  }.|.S.).Nz.In ca
+0000ca10: 7264 5f63 6861 6c6c 656e 6765 5f72 6573  rd_challenge_res
+0000ca20: 706f 6e73 655f 706b 6972 0100 0000 720f  ponse_pkir....r.
+0000ca30: 0100 0029 0b72 2700 0000 7234 0000 0072  ...).r'...r4...r
+0000ca40: 2b00 0000 72be 0000 005a 1a49 4e53 5f43  +...r....Z.INS_C
+0000ca50: 4841 4c4c 454e 4745 5f52 4553 504f 4e53  HALLENGE_RESPONS
+0000ca60: 455f 504b 4972 1800 0000 7235 0000 0072  E_PKIr....r5...r
+0000ca70: c800 0000 729b 0000 0072 7700 0000 5a1d  ....r....rw...Z.
+0000ca80: 7665 7269 6679 5f63 6861 6c6c 656e 6765  verify_challenge
+0000ca90: 5f72 6573 706f 6e73 655f 706b 6929 0c72  _response_pki).r
+0000caa0: 3600 0000 7213 0100 0072 a100 0000 7289  6...r....r....r.
+0000cab0: 0000 0072 a200 0000 72a3 0000 005a 1363  ...r....r....Z.c
+0000cac0: 6861 6c6c 656e 6765 5f66 726f 6d5f 686f  hallenge_from_ho
+0000cad0: 7374 729a 0000 0072 2200 0000 725e 0000  str....r"...r^..
+0000cae0: 0072 5f00 0000 5a05 7665 7269 6672 3700  .r_...Z.verifr7.
+0000caf0: 0000 7237 0000 0072 3800 0000 da1b 6361  ..r7...r8.....ca
+0000cb00: 7264 5f63 6861 6c6c 656e 6765 5f72 6573  rd_challenge_res
+0000cb10: 706f 6e73 655f 706b 6991 0700 0073 1400  ponse_pki....s..
+0000cb20: 0000 0001 0a01 0601 0601 0401 0402 0802  ................
+0000cb30: 1a01 1003 1002 7a29 4361 7264 436f 6e6e  ......z)CardConn
+0000cb40: 6563 746f 722e 6361 7264 5f63 6861 6c6c  ector.card_chall
+0000cb50: 656e 6765 5f72 6573 706f 6e73 655f 706b  enge_response_pk
+0000cb60: 6963 0100 0000 0000 0000 0f00 0000 1400  ic..............
+0000cb70: 0000 4300 0000 73c0 0100 0074 006a 0164  ..C...s....t.j.d
+0000cb80: 0183 0101 0064 0204 007d 017d 0279 1e7c  .....d...}.}.y.|
+0000cb90: 006a 0283 007d 0174 006a 0164 0374 037c  .j...}.t.j.d.t.|
+0000cba0: 0183 0117 0083 0101 0057 006e 8004 0074  .........W.n...t
+0000cbb0: 046b 0a72 6001 007d 0301 007a 1464 026a  .k.r`..}...z.d.j
+0000cbc0: 0564 0464 0567 0283 017d 0257 0059 0064  .d.d.g...}.W.Y.d
+0000cbd0: 0064 007d 037e 0358 006e 5204 0074 066b  .d.}.~.X.nR..t.k
+0000cbe0: 0a72 8401 007d 0301 007a 0a64 067d 0257  .r...}...z.d.}.W
+0000cbf0: 0059 0064 0064 007d 037e 0358 006e 2e04  .Y.d.d.}.~.X.n..
+0000cc00: 0074 076b 0a72 b001 007d 0301 007a 1264  .t.k.r...}...z.d
+0000cc10: 0774 037c 0383 0117 007d 0257 0059 0064  .t.|.....}.W.Y.d
+0000cc20: 0064 007d 037e 0358 006e 0258 007c 0164  .d.}.~.X.n.X.|.d
+0000cc30: 086b 0272 be64 097d 027c 0264 026b 0372  .k.r.d.}.|.d.k.r
+0000cc40: d464 0a64 0864 0864 087c 0266 0553 0074  .d.d.d.d.|.f.S.t
+0000cc50: 0883 007d 047c 046a 097c 017c 006a 0a83  ...}.|.j.|.|.j..
+0000cc60: 025c 067d 057d 067d 077d 087d 097d 027c  .\.}.}.}.}.}.}.|
+0000cc70: 0590 0173 0864 0a7c 077c 087c 097c 0266  ...s.d.|.|.|.|.f
+0000cc80: 0553 007c 006a 0b7c 0683 015c 027d 0a7d  .S.|.j.|...\.}.}
+0000cc90: 027c 0a90 0173 2a64 0a7c 077c 087c 097c  .|...s*d.|.|.|.|
+0000cca0: 0266 0553 007c 046a 0c7c 0183 017d 0b7c  .f.S.|.j.|...}.|
+0000ccb0: 0b64 0b19 007d 0c74 006a 0164 0c7c 0c9b  .d...}.t.j.d.|..
+0000ccc0: 009d 0283 0101 007c 0c6a 0d64 0d64 0083  .......|.j.d.d..
+0000ccd0: 026a 0e64 0e83 017d 0d74 006a 0164 0f7c  .j.d...}.t.j.d.|
+0000cce0: 0d9b 009d 0283 0101 0074 006a 0164 107c  .........t.j.d.|
+0000ccf0: 006a 0f9b 009d 0283 0101 007c 0d6a 1083  .j.........|.j..
+0000cd00: 007c 006a 0f6a 1083 006b 0290 0172 9a64  .|.j.j...k...r.d
+0000cd10: 117d 0e6e 1864 0a7d 0e64 127c 0d9b 0064  .}.n.d.}.d.|...d
+0000cd20: 137c 006a 0f9b 0064 149d 057d 027c 0e7c  .|.j...d...}.|.|
+0000cd30: 077c 087c 097c 0266 0553 0029 154e 7a1b  .|.|.|.f.S.).Nz.
+0000cd40: 496e 2063 6172 645f 7665 7269 6679 5f61  In card_verify_a
+0000cd50: 7574 6865 6e74 6963 6974 79da 007a 0a43  uthenticity..z.C
+0000cd60: 6572 7420 5045 4d3a 207a 3855 6e61 626c  ert PEM: z8Unabl
+0000cd70: 6520 746f 2067 6574 2064 6576 6963 6520  e to get device 
+0000cd80: 6365 7274 6966 6963 6174 653a 2066 6561  certificate: fea
+0000cd90: 7475 7265 2075 6e73 7570 706f 7274 6564  ture unsupported
+0000cda0: 2120 0a7a 5141 7574 6865 6e74 6963 6974  ! .zQAuthenticit
+0000cdb0: 7920 7661 6c69 6461 7469 6f6e 2069 7320  y validation is 
+0000cdc0: 6f6e 6c79 2061 7661 696c 6162 6c65 2073  only available s
+0000cdd0: 7461 7274 696e 6720 7769 7468 2053 6174  tarting with Sat
+0000cde0: 6f63 6869 7020 7630 2e31 3220 616e 6420  ochip v0.12 and 
+0000cdf0: 6869 6768 6572 7a22 4e6f 2063 6172 6420  higherz"No card 
+0000ce00: 666f 756e 6421 2050 6c65 6173 6520 696e  found! Please in
+0000ce10: 7365 7274 2063 6172 642e 7a2c 4578 6365  sert card.z,Exce
+0000ce20: 7074 696f 6e20 6475 7269 6e67 2064 6576  ption during dev
+0000ce30: 6963 6520 6365 7274 6966 6963 6174 6520  ice certificate 
+0000ce40: 6578 706f 7274 3a20 7a07 2865 6d70 7479  export: z.(empty
+0000ce50: 297a 4044 6576 6963 6520 6365 7274 6966  )z@Device certif
+0000ce60: 6963 6174 6520 6973 2065 6d70 7479 3a20  icate is empty: 
+0000ce70: 7468 6520 6361 7264 2068 6173 206e 6f74  the card has not
+0000ce80: 2062 6565 6e20 7065 7273 6f6e 616c 697a   been personaliz
+0000ce90: 6564 2146 da07 7375 626a 6563 747a 2a49  ed!F..subjectz*I
+0000cea0: 6e20 6361 7264 5f76 6572 6966 795f 6175  n card_verify_au
+0000ceb0: 7468 656e 7469 6369 7479 2073 7562 6a65  thenticity subje
+0000cec0: 6374 5f64 6963 743d 2073 0200 0000 434e  ct_dict= s....CN
+0000ced0: 7a05 7574 662d 387a 2549 6e20 6361 7264  z.utf-8z%In card
+0000cee0: 5f76 6572 6966 795f 6175 7468 656e 7469  _verify_authenti
+0000cef0: 6369 7479 2073 7562 6a65 6374 3d20 7a26  city subject= z&
+0000cf00: 496e 2063 6172 645f 7665 7269 6679 5f61  In card_verify_a
+0000cf10: 7574 6865 6e74 6963 6974 7920 5549 445f  uthenticity UID_
+0000cf20: 5348 4131 3d20 547a 1443 6572 7469 6669  SHA1= Tz.Certifi
+0000cf30: 6361 7465 2073 7562 6a65 6374 207a 2720  cate subject z' 
+0000cf40: 646f 6573 206e 6f74 206d 6174 6368 2074  does not match t
+0000cf50: 6865 2063 6172 6420 7365 7269 616c 206e  he card serial n
+0000cf60: 756d 6265 7220 fa01 2129 1172 2700 0000  umber ..!).r'...
+0000cf70: 7234 0000 0072 7301 0000 7276 0000 0072  r4...rs...rv...r
+0000cf80: e500 0000 da04 6a6f 696e 7299 0000 0072  ......joinr....r
+0000cf90: f400 0000 7217 0000 005a 1a76 616c 6964  ....r....Z.valid
+0000cfa0: 6174 655f 6365 7274 6966 6963 6174 655f  ate_certificate_
+0000cfb0: 6368 6169 6e72 8300 0000 7274 0100 005a  chainr....rt...Z
+0000cfc0: 1570 6172 7365 5f70 656d 5f63 6572 7469  .parse_pem_certi
+0000cfd0: 6669 6361 7465 7246 0100 0072 c200 0000  ficaterF...r....
+0000cfe0: 7252 0000 00da 056c 6f77 6572 290f 7236  rR.....lower).r6
+0000cff0: 0000 0072 8400 0000 5a09 7478 745f 6572  ...r....Z.txt_er
+0000d000: 726f 7272 ad00 0000 5a09 7661 6c69 6461  rorr....Z.valida
+0000d010: 746f 725a 0e69 735f 7661 6c69 645f 6368  torZ.is_valid_ch
+0000d020: 6169 6e5a 0d64 6576 6963 655f 7075 626b  ainZ.device_pubk
+0000d030: 6579 5a06 7478 745f 6361 5a09 7478 745f  eyZ.txt_caZ.txt_
+0000d040: 7375 6263 615a 0a74 7874 5f64 6576 6963  subcaZ.txt_devic
+0000d050: 655a 1169 735f 7661 6c69 645f 6368 616c  eZ.is_valid_chal
+0000d060: 7265 7370 5a09 6365 7274 5f64 6963 745a  respZ.cert_dictZ
+0000d070: 0c73 7562 6a65 6374 5f64 6963 7472 7601  .subject_dictrv.
+0000d080: 0000 5a16 6973 5f76 616c 6964 5f73 6572  ..Z.is_valid_ser
+0000d090: 6961 6c5f 6e75 6d62 6572 7237 0000 0072  ial_numberr7...r
+0000d0a0: 3700 0000 7238 0000 00da 1863 6172 645f  7...r8.....card_
+0000d0b0: 7665 7269 6679 5f61 7574 6865 6e74 6963  verify_authentic
+0000d0c0: 6974 79a2 0700 0073 4400 0000 0001 0a03  ity....sD.......
+0000d0d0: 0801 0201 0801 1601 1001 0601 1801 1001  ................
+0000d0e0: 1401 1001 1e02 0801 0402 0801 0e03 0601  ................
+0000d0f0: 1a01 0601 0e03 0e01 0601 0e03 0a01 0801  ................
+0000d100: 1001 1201 1001 1201 1401 0602 0401 1402  ................
+0000d110: 7a26 4361 7264 436f 6e6e 6563 746f 722e  z&CardConnector.
+0000d120: 6361 7264 5f76 6572 6966 795f 6175 7468  card_verify_auth
+0000d130: 656e 7469 6369 7479 6302 0000 0000 0000  enticityc.......
+0000d140: 0002 0000 0002 0000 0043 0000 0073 2800  .........C...s(.
+0000d150: 0000 7c01 6700 6b02 7218 7400 6401 6701  ..|.g.k.r.t.d.g.
+0000d160: 1400 7d01 6402 7c00 5f01 7c01 7c00 5f02  ..}.d.|._.|.|._.
+0000d170: 6403 7c00 5f01 6400 5300 2904 4e72 0100  d.|._.d.S.).Nr..
+0000d180: 0000 4654 2903 727f 0000 0072 7e00 0000  ..FT).r....r~...
+0000d190: 7280 0000 0029 0272 3600 0000 7280 0000  r....).r6...r...
+0000d1a0: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
+0000d1b0: 72da 0000 00d6 0700 0073 0a00 0000 0001  r........s......
+0000d1c0: 0801 0a01 0601 0601 7a28 4361 7264 436f  ........z(CardCo
+0000d1d0: 6e6e 6563 746f 722e 7361 746f 6469 6d65  nnector.satodime
+0000d1e0: 5f73 6574 5f75 6e6c 6f63 6b5f 7365 6372  _set_unlock_secr
+0000d1f0: 6574 6302 0000 0000 0000 0002 0000 0002  etc.............
+0000d200: 0000 0043 0000 0073 1c00 0000 7c01 6700  ...C...s....|.g.
+0000d210: 6b02 7212 7400 6401 6701 1400 7d01 7c01  k.r.t.d.g...}.|.
+0000d220: 7c00 5f01 6400 5300 2902 4e72 0100 0000  |._.d.S.).Nr....
+0000d230: 2902 7281 0000 0072 8200 0000 2902 7236  ).r....r....).r6
+0000d240: 0000 0072 8200 0000 7237 0000 0072 3700  ...r....r7...r7.
+0000d250: 0000 7238 0000 0072 d900 0000 dc07 0000  ..r8...r........
+0000d260: 7306 0000 0000 0108 010a 017a 2943 6172  s..........z)Car
+0000d270: 6443 6f6e 6e65 6374 6f72 2e73 6174 6f64  dConnector.satod
+0000d280: 696d 655f 7365 745f 756e 6c6f 636b 5f63  ime_set_unlock_c
+0000d290: 6f75 6e74 6572 6301 0000 0000 0000 0002  ounterc.........
+0000d2a0: 0000 0006 0000 0043 0000 0073 3400 0000  .......C...s4...
+0000d2b0: 7400 6a01 7c00 6a02 6401 6402 6403 8d03  t.j.|.j.d.d.d...
+0000d2c0: 7d01 7c01 6404 3700 7d01 7403 7c01 6a04  }.|.d.7.}.t.|.j.
+0000d2d0: 6405 6401 6402 6403 8d03 8301 7c00 5f02  d.d.d.d.....|._.
+0000d2e0: 6400 5300 2906 4e5a 0362 6967 4629 02da  d.S.).NZ.bigF)..
+0000d2f0: 0962 7974 656f 7264 6572 5a06 7369 676e  .byteorderZ.sign
+0000d300: 6564 720c 0000 0072 4300 0000 2905 da03  edr....rC...)...
+0000d310: 696e 74da 0a66 726f 6d5f 6279 7465 7372  int..from_bytesr
+0000d320: 8200 0000 72c8 0000 00da 0874 6f5f 6279  ....r......to_by
+0000d330: 7465 7329 0272 3600 0000 5a0b 636f 756e  tes).r6...Z.coun
+0000d340: 7465 725f 696e 7472 3700 0000 7237 0000  ter_intr7...r7..
+0000d350: 0072 3800 0000 da21 7361 746f 6469 6d65  .r8....!satodime
+0000d360: 5f69 6e63 7265 6d65 6e74 5f75 6e6c 6f63  _increment_unloc
+0000d370: 6b5f 636f 756e 7465 72e0 0700 0073 0600  k_counter....s..
+0000d380: 0000 0001 1201 0801 7a2f 4361 7264 436f  ........z/CardCo
+0000d390: 6e6e 6563 746f 722e 7361 746f 6469 6d65  nnector.satodime
+0000d3a0: 5f69 6e63 7265 6d65 6e74 5f75 6e6c 6f63  _increment_unloc
+0000d3b0: 6b5f 636f 756e 7465 7263 0100 0000 0000  k_counterc......
+0000d3c0: 0000 0b00 0000 0500 0000 4300 0000 732a  ..........C...s*
+0000d3d0: 0100 0074 006a 0164 0183 0101 0074 026a  ...t.j.d.....t.j
+0000d3e0: 037d 0164 027d 0264 037d 0364 037d 047c  .}.d.}.d.}.d.}.|
+0000d3f0: 017c 027c 037c 0467 047d 057c 006a 047c  .|.|.|.g.}.|.j.|
+0000d400: 0583 015c 037d 067d 077d 087c 0764 046b  ...\.}.}.}.|.d.k
+0000d410: 0272 4a7c 0864 036b 0272 4a6e 827c 0764  .rJ|.d.k.rJn.|.d
+0000d420: 036b 0272 6e7c 0864 036b 0272 6e74 006a  .k.rn|.d.k.rnt.j
+0000d430: 0564 0583 0101 0074 0664 0583 0182 016e  .d.....t.d.....n
+0000d440: 5e7c 0764 066b 0272 927c 0864 076b 0272  ^|.d.k.r.|.d.k.r
+0000d450: 9274 006a 0564 0883 0101 0074 0764 0983  .t.j.d.....t.d..
+0000d460: 0182 016e 3a74 006a 0564 0a74 0864 0b7c  ...n:t.j.d.t.d.|
+0000d470: 0714 007c 0817 0083 019b 0064 0c9d 0383  ...|.......d....
+0000d480: 0101 0074 0964 0a74 0864 0b7c 0714 007c  ...t.d.t.d.|...|
+0000d490: 0817 0083 019b 0064 0c9d 0383 0182 0164  .......d.......d
+0000d4a0: 037d 0969 007d 0a7c 067c 097c 0974 0a17  .}.i.}.|.|.|.t..
+0000d4b0: 0085 0219 007c 0a64 0d3c 007c 0a64 0d19  .....|.d.<.|.d..
+0000d4c0: 007c 005f 0b7c 0974 0a37 007d 097c 067c  .|._.|.t.7.}.|.|
+0000d4d0: 0919 007c 0a64 0e3c 007c 0964 0f37 007d  ...|.d.<.|.d.7.}
+0000d4e0: 097c 067c 0964 1085 0219 007c 0a64 113c  .|.|.d.....|.d.<
+0000d4f0: 007c 067c 077c 087c 0a66 0453 0029 127a  .|.|.|.|.f.S.).z
+0000d500: 2752 6574 7572 6e20 7374 6174 7573 2069  'Return status i
+0000d510: 6e66 6f20 7370 6563 6966 6963 2074 6f20  nfo specific to 
+0000d520: 5361 746f 6469 6d65 7a16 496e 2073 6174  Satodimez.In sat
+0000d530: 6f64 696d 655f 6765 745f 7374 6174 7573  odime_get_status
+0000d540: e950 0000 0072 0100 0000 7241 0000 007a  .P...r....rA...z
+0000d550: 4345 7272 6f72 2077 6869 6c65 2066 6574  CError while fet
+0000d560: 6368 696e 6720 5361 746f 6469 6d65 2073  ching Satodime s
+0000d570: 7461 7475 733a 206e 6f20 6361 7264 2070  tatus: no card p
+0000d580: 7265 7365 6e74 2028 636f 6465 2030 7830  resent (code 0x0
+0000d590: 3030 3029 7242 0000 0072 4300 0000 7a42  000)rB...rC...zB
+0000d5a0: 4572 726f 7220 7768 696c 6520 6665 7463  Error while fetc
+0000d5b0: 6869 6e67 2053 6174 6f64 696d 6520 7374  hing Satodime st
+0000d5c0: 6174 7573 3a20 7365 7475 7020 6e6f 7420  atus: setup not 
+0000d5d0: 646f 6e65 2028 636f 6465 2030 7830 3030  done (code 0x000
+0000d5e0: 3029 7a42 4572 726f 7220 7768 696c 6520  0)zBError while 
+0000d5f0: 6665 7463 6869 6e67 2053 6174 6f64 696d  fetching Satodim
+0000d600: 6520 7374 6174 7573 3a20 7365 7475 7020  e status: setup 
+0000d610: 6e6f 7420 646f 6e65 2028 636f 6465 2030  not done (code 0
+0000d620: 7839 6330 3429 7a32 4572 726f 7220 7768  x9c04)z2Error wh
+0000d630: 696c 6520 6665 7463 6869 6e67 2053 6174  ile fetching Sat
+0000d640: 6f64 696d 6520 7374 6174 7573 3a20 2865  odime status: (e
+0000d650: 7272 6f72 2063 6f64 6520 72bc 0000 0072  rror code r....r
+0000d660: bd00 0000 7282 0000 00da 0c6d 6178 5f6e  ....r......max_n
+0000d670: 756d 5f6b 6579 7372 0c00 0000 4eda 1473  um_keysr....N..s
+0000d680: 6174 6f64 696d 655f 6b65 7973 5f73 7461  atodime_keys_sta
+0000d690: 7475 7329 0c72 2700 0000 7234 0000 0072  tus).r'...r4...r
+0000d6a0: 2b00 0000 72be 0000 0072 9b00 0000 72e4  +...r....r....r.
+0000d6b0: 0000 0072 9900 0000 da15 4361 7264 5365  ...r......CardSe
+0000d6c0: 7475 704e 6f74 446f 6e65 4572 726f 7272  tupNotDoneErrorr
+0000d6d0: 4c00 0000 72f4 0000 0072 8100 0000 7282  L...r....r....r.
+0000d6e0: 0000 0029 0b72 3600 0000 72a1 0000 0072  ...).r6...r....r
+0000d6f0: 8900 0000 72a2 0000 0072 a300 0000 729a  ....r....r....r.
+0000d700: 0000 0072 2200 0000 725e 0000 0072 5f00  ...r"...r^...r_.
+0000d710: 0000 7268 0100 005a 0f73 6174 6f64 696d  ..rh...Z.satodim
+0000d720: 655f 7374 6174 7573 7237 0000 0072 3700  e_statusr7...r7.
+0000d730: 0000 7238 0000 00da 1373 6174 6f64 696d  ..r8.....satodim
+0000d740: 655f 6765 745f 7374 6174 7573 e507 0000  e_get_status....
+0000d750: 7334 0000 0000 020a 0106 0104 0104 0104  s4..............
+0000d760: 010c 0110 0210 0102 0110 010a 010a 0110  ................
+0000d770: 010a 010a 021e 011c 0204 0104 0114 010a  ................
+0000d780: 0108 010c 0108 0110 017a 2143 6172 6443  .........z!CardC
+0000d790: 6f6e 6e65 6374 6f72 2e73 6174 6f64 696d  onnector.satodim
+0000d7a0: 655f 6765 745f 7374 6174 7573 2901 da07  e_get_status)...
+0000d7b0: 6b65 795f 6e62 7263 0200 0000 0000 0000  key_nbrc........
+0000d7c0: 0b00 0000 0400 0000 4300 0000 7398 0000  ........C...s...
+0000d7d0: 0074 006a 0164 0183 0101 0074 026a 037d  .t.j.d.....t.j.}
+0000d7e0: 0264 027d 037c 0164 0316 007d 0464 047d  .d.}.|.d...}.d.}
+0000d7f0: 057c 027c 037c 047c 0567 047d 067c 006a  .|.|.|.|.g.}.|.j
+0000d800: 047c 0683 015c 037d 077d 087d 097c 0864  .|...\.}.}.}.|.d
+0000d810: 056b 0272 4e7c 0964 046b 0272 4e6e 327c  .k.rN|.d.k.rNn2|
+0000d820: 0864 046b 0272 807c 0964 046b 0272 8074  .d.k.r.|.d.k.r.t
+0000d830: 006a 0564 067c 019b 0064 079d 0383 0101  .j.d.|...d......
+0000d840: 0074 0664 067c 019b 0064 079d 0383 0182  .t.d.|...d......
+0000d850: 017c 006a 076a 087c 0783 017d 0a7c 077c  .|.j.j.|...}.|.|
+0000d860: 087c 097c 0a66 0453 0029 084e 7a1e 496e  .|.|.f.S.).Nz.In
+0000d870: 2073 6174 6f64 696d 655f 6765 745f 6b65   satodime_get_ke
+0000d880: 7973 6c6f 745f 7374 6174 7573 728b 0000  yslot_statusr...
+0000d890: 0072 bc00 0000 7201 0000 0072 4100 0000  .r....r....rA...
+0000d8a0: 7a22 4572 726f 7220 7768 696c 6520 6665  z"Error while fe
+0000d8b0: 7463 6869 6e67 2053 6174 6f64 696d 6520  tching Satodime 
+0000d8c0: 6b65 7920 7a26 2073 7461 7475 733a 206e  key z& status: n
+0000d8d0: 6f20 6361 7264 2070 7265 7365 6e74 2028  o card present (
+0000d8e0: 636f 6465 2030 7830 3030 3029 2909 7227  code 0x0000)).r'
+0000d8f0: 0000 0072 3400 0000 722b 0000 0072 be00  ...r4...r+...r..
+0000d900: 0000 729b 0000 0072 e400 0000 7299 0000  ..r....r....r...
+0000d910: 0072 7700 0000 5a21 7061 7273 655f 7361  .rw...Z!parse_sa
+0000d920: 746f 6469 6d65 5f67 6574 5f6b 6579 736c  todime_get_keysl
+0000d930: 6f74 5f73 7461 7475 7329 0b72 3600 0000  ot_status).r6...
+0000d940: 7285 0100 0072 a100 0000 7289 0000 0072  r....r....r....r
+0000d950: a200 0000 72a3 0000 0072 9a00 0000 7222  ....r....r....r"
+0000d960: 0000 0072 5e00 0000 725f 0000 005a 0e6b  ...r^...r_...Z.k
+0000d970: 6579 736c 6f74 5f73 7461 7475 7372 3700  eyslot_statusr7.
+0000d980: 0000 7237 0000 0072 3800 0000 da1b 7361  ..r7...r8.....sa
+0000d990: 746f 6469 6d65 5f67 6574 5f6b 6579 736c  todime_get_keysl
+0000d9a0: 6f74 5f73 7461 7475 7308 0800 0073 1c00  ot_status....s..
+0000d9b0: 0000 0001 0a01 0601 0401 0801 0401 0c02  ................
+0000d9c0: 1002 1001 0201 1001 1201 1003 0c01 7a29  ..............z)
+0000d9d0: 4361 7264 436f 6e6e 6563 746f 722e 7361  CardConnector.sa
+0000d9e0: 746f 6469 6d65 5f67 6574 5f6b 6579 736c  todime_get_keysl
+0000d9f0: 6f74 5f73 7461 7475 7329 0472 8501 0000  ot_status).r....
+0000da00: da04 5246 5531 da04 5246 5532 da09 6b65  ..RFU1..RFU2..ke
+0000da10: 795f 6173 7365 7463 0800 0000 0000 0000  y_assetc........
+0000da20: 1400 0000 0600 0000 4300 0000 735e 0100  ........C...s^..
+0000da30: 0074 006a 0164 0183 0101 0074 026a 037d  .t.j.d.....t.j.}
+0000da40: 0864 027d 097c 0164 0316 007d 0a64 047d  .d.}.|.d...}.d.}
+0000da50: 0b74 0474 0517 0064 0517 0074 0617 0074  .t.t...d...t...t
+0000da60: 0717 0074 0817 007d 0c7c 087c 097c 0a7c  ...t...}.|.|.|.|
+0000da70: 0b7c 0c67 057d 0d7c 0567 006b 0272 5a64  .|.g.}.|.g.k.rZd
+0000da80: 0664 0464 0464 0467 047d 057c 0667 006b  .d.d.d.g.}.|.g.k
+0000da90: 0272 6c74 0764 0467 0114 007d 067c 0767  .rlt.d.g...}.|.g
+0000daa0: 006b 0272 7e74 0864 0467 0114 007d 0774  .k.r~t.d.g...}.t
+0000dab0: 097c 0583 0174 0a6b 0872 9274 0b7c 0583  .|...t.k.r.t.|..
+0000dac0: 017d 0574 097c 0683 0174 0a6b 0872 a674  .}.t.|...t.k.r.t
+0000dad0: 0b7c 0683 017d 0674 097c 0783 0174 0a6b  .|...}.t.|...t.k
+0000dae0: 0872 ba74 0b7c 0783 017d 0774 0b74 0c6a  .r.t.|...}.t.t.j
+0000daf0: 0d74 0a7c 006a 0e83 0174 0a7c 0d7c 006a  .t.|.j...t.|.|.j
+0000db00: 0f17 0083 0174 106a 1183 036a 1283 0083  .....t.j...j....
+0000db10: 017d 0e7c 006a 0f7c 0e17 007c 0264 0316  .}.|.j.|...|.d..
+0000db20: 007c 0364 0316 007c 0464 0316 0067 0317  .|.d...|.d...g..
+0000db30: 007c 0517 007c 0617 007c 0717 007d 0f74  .|...|...|...}.t
+0000db40: 137c 0f83 017c 0c6b 0390 0172 3474 1464  .|...|.k...r4t.d
+0000db50: 0774 137c 0f83 019b 0064 087c 0c9b 009d  .t.|.....d.|....
+0000db60: 0483 0182 017c 0d7c 0f17 007d 107c 006a  .....|.|...}.|.j
+0000db70: 157c 1083 015c 037d 117d 127d 137c 006a  .|...\.}.}.}.|.j
+0000db80: 1683 0001 007c 117c 127c 1366 0353 0029  .....|.|.|.f.S.)
+0000db90: 094e 7a1e 496e 2073 6174 6f64 696d 655f  .Nz.In satodime_
+0000dba0: 7365 745f 6b65 7973 6c6f 745f 7374 6174  set_keyslot_stat
+0000dbb0: 7573 728c 0000 0072 bc00 0000 7201 0000  usr....r....r...
+0000dbc0: 0072 b300 0000 729d 0000 007a 3a45 7272  .r....r....z:Err
+0000dbd0: 6f72 2069 6e20 7361 746f 6469 6d65 5f73  or in satodime_s
+0000dbe0: 6574 5f6b 6579 736c 6f74 5f73 7461 7475  et_keyslot_statu
+0000dbf0: 733a 2077 726f 6e67 2073 7461 7475 7320  s: wrong status 
+0000dc00: 6c65 6e67 7468 207a 0c20 696e 7374 6561  length z. instea
+0000dc10: 6420 6f66 2029 1772 2700 0000 7234 0000  d of ).r'...r4..
+0000dc20: 0072 2b00 0000 72be 0000 0072 8100 0000  .r+...r....r....
+0000dc30: da10 5349 5a45 5f55 4e4c 4f43 4b5f 434f  ..SIZE_UNLOCK_CO
+0000dc40: 4445 5a0b 5349 5a45 5f53 4c49 5034 345a  DEZ.SIZE_SLIP44Z
+0000dc50: 0d53 495a 455f 434f 4e54 5241 4354 5a0c  .SIZE_CONTRACTZ.
+0000dc60: 5349 5a45 5f54 4f4b 454e 4944 7226 0000  SIZE_TOKENIDr&..
+0000dc70: 0072 4b00 0000 72c8 0000 0072 ed00 0000  .rK...r....r....
+0000dc80: da03 6e65 7772 8000 0000 7282 0000 0072  ..newr....r....r
+0000dc90: 4f00 0000 7250 0000 00da 0664 6967 6573  O...rP.....diges
+0000dca0: 7472 3500 0000 7253 0000 0072 9b00 0000  tr5...rS...r....
+0000dcb0: 727f 0100 0029 1472 3600 0000 7285 0100  r....).r6...r...
+0000dcc0: 0072 8701 0000 7288 0100 0072 8901 0000  .r....r....r....
+0000dcd0: 5a0a 6b65 795f 736c 6970 3434 5a0c 6b65  Z.key_slip44Z.ke
+0000dce0: 795f 636f 6e74 7261 6374 5a0b 6b65 795f  y_contractZ.key_
+0000dcf0: 746f 6b65 6e69 6472 a100 0000 7289 0000  tokenidr....r...
+0000dd00: 0072 a200 0000 72a3 0000 00da 0864 6174  .r....r......dat
+0000dd10: 6173 697a 65da 0a61 7064 7568 6561 6465  asize..apduheade
+0000dd20: 72da 0b75 6e6c 6f63 6b5f 636f 6465 72cb  r..unlock_coder.
+0000dd30: 0000 0072 9a00 0000 7222 0000 0072 5e00  ...r....r"...r^.
+0000dd40: 0000 725f 0000 0072 3700 0000 7237 0000  ..r_...r7...r7..
+0000dd50: 0072 3800 0000 da21 7361 746f 6469 6d65  .r8....!satodime
+0000dd60: 5f73 6574 5f6b 6579 736c 6f74 5f73 7461  _set_keyslot_sta
+0000dd70: 7475 735f 7061 7274 301c 0800 0073 3600  tus_part0....s6.
+0000dd80: 0000 0002 0a01 0601 0401 0801 0401 1801  ................
+0000dd90: 0e02 0800 0c01 0800 0a01 0800 0a01 0c00  ................
+0000dda0: 0801 0c00 0801 0c00 0803 2802 2c01 0e01  ..........(.,...
+0000ddb0: 1801 0802 1001 0802 7a2f 4361 7264 436f  ........z/CardCo
+0000ddc0: 6e6e 6563 746f 722e 7361 746f 6469 6d65  nnector.satodime
+0000ddd0: 5f73 6574 5f6b 6579 736c 6f74 5f73 7461  _set_keyslot_sta
+0000dde0: 7475 735f 7061 7274 3063 0300 0000 0000  tus_part0c......
+0000ddf0: 0000 0f00 0000 0600 0000 4300 0000 73e4  ..........C...s.
+0000de00: 0000 0074 006a 0164 0183 0101 0074 026a  ...t.j.d.....t.j
+0000de10: 037d 0364 027d 047c 0164 0316 007d 0564  .}.d.}.|.d...}.d
+0000de20: 047d 0674 0474 0517 0074 0617 007d 077c  .}.t.t...t...}.|
+0000de30: 037c 047c 057c 067c 0767 057d 087c 0267  .|.|.|.|.g.}.|.g
+0000de40: 006b 0272 4c74 0664 0567 0114 007d 0274  .k.rLt.d.g...}.t
+0000de50: 077c 0283 0174 086b 0872 6074 097c 0283  .|...t.k.r`t.|..
+0000de60: 017d 0274 0974 0a6a 0b74 087c 006a 0c83  .}.t.t.j.t.|.j..
+0000de70: 0174 087c 087c 006a 0d17 0083 0174 0e6a  .t.|.|.j.....t.j
+0000de80: 0f83 036a 1083 0083 017d 097c 006a 0d7c  ...j.....}.|.j.|
+0000de90: 0917 007c 0217 007d 0a74 117c 0a83 017c  ...|...}.t.|...|
+0000dea0: 076b 0372 ba74 1264 0674 117c 0a83 019b  .k.r.t.d.t.|....
+0000deb0: 0064 077c 079b 009d 0483 0182 017c 087c  .d.|.........|.|
+0000dec0: 0a17 007d 0b7c 006a 137c 0b83 015c 037d  ...}.|.j.|...\.}
+0000ded0: 0c7d 0d7d 0e7c 006a 1483 0001 007c 0c7c  .}.}.|.j.....|.|
+0000dee0: 0d7c 0e66 0353 0029 084e 7a1e 496e 2073  .|.f.S.).Nz.In s
+0000def0: 6174 6f64 696d 655f 7365 745f 6b65 7973  atodime_set_keys
+0000df00: 6c6f 745f 7374 6174 7573 728c 0000 0072  lot_statusr....r
+0000df10: bc00 0000 720c 0000 0072 0100 0000 7a3a  ....r....r....z:
+0000df20: 4572 726f 7220 696e 2073 6174 6f64 696d  Error in satodim
+0000df30: 655f 7365 745f 6b65 7973 6c6f 745f 7374  e_set_keyslot_st
+0000df40: 6174 7573 3a20 7772 6f6e 6720 7374 6174  atus: wrong stat
+0000df50: 7573 206c 656e 6774 6820 7a0c 2069 6e73  us length z. ins
+0000df60: 7465 6164 206f 6620 2915 7227 0000 0072  tead of ).r'...r
+0000df70: 3400 0000 722b 0000 0072 be00 0000 7281  4...r+...r....r.
+0000df80: 0000 0072 8a01 0000 5a09 5349 5a45 5f44  ...r....Z.SIZE_D
+0000df90: 4154 4172 2600 0000 724b 0000 0072 c800  ATAr&...rK...r..
+0000dfa0: 0000 72ed 0000 0072 8b01 0000 7280 0000  ..r....r....r...
+0000dfb0: 0072 8200 0000 724f 0000 0072 5000 0000  .r....rO...rP...
+0000dfc0: 728c 0100 0072 3500 0000 7253 0000 0072  r....r5...rS...r
+0000dfd0: 9b00 0000 727f 0100 0029 0f72 3600 0000  ....r....).r6...
+0000dfe0: 7285 0100 005a 086b 6579 5f64 6174 6172  r....Z.key_datar
+0000dff0: a100 0000 7289 0000 0072 a200 0000 72a3  ....r....r....r.
+0000e000: 0000 0072 8d01 0000 728e 0100 0072 8f01  ...r....r....r..
+0000e010: 0000 72cb 0000 0072 9a00 0000 7222 0000  ..r....r....r"..
+0000e020: 0072 5e00 0000 725f 0000 0072 3700 0000  .r^...r_...r7...
+0000e030: 7237 0000 0072 3800 0000 da21 7361 746f  r7...r8....!sato
+0000e040: 6469 6d65 5f73 6574 5f6b 6579 736c 6f74  dime_set_keyslot
+0000e050: 5f73 7461 7475 735f 7061 7274 313a 0800  _status_part1:..
+0000e060: 0073 2600 0000 0002 0a01 0601 0401 0801  .s&.............
+0000e070: 0401 0c01 0e02 0800 0a01 0c00 0803 2802  ..............(.
+0000e080: 0e01 0c01 1801 0802 1001 0802 7a2f 4361  ............z/Ca
+0000e090: 7264 436f 6e6e 6563 746f 722e 7361 746f  rdConnector.sato
+0000e0a0: 6469 6d65 5f73 6574 5f6b 6579 736c 6f74  dime_set_keyslot
+0000e0b0: 5f73 7461 7475 735f 7061 7274 3163 0200  _status_part1c..
+0000e0c0: 0000 0000 0000 0d00 0000 0500 0000 4300  ..............C.
+0000e0d0: 0000 735c 0000 0074 006a 0164 0183 0101  ..s\...t.j.d....
+0000e0e0: 0074 026a 037d 0264 027d 037c 0164 0316  .t.j.}.d.}.|.d..
+0000e0f0: 007d 0464 047d 057c 027c 037c 047c 0567  .}.d.}.|.|.|.|.g
+0000e100: 047d 067c 006a 047c 0683 015c 037d 077d  .}.|.j.|...\.}.}
+0000e110: 087d 097c 006a 056a 067c 0783 015c 037d  .}.|.j.j.|...\.}
+0000e120: 0a7d 0b7d 0c7c 077c 087c 097c 0a7c 0b66  .}.}.|.|.|.|.|.f
+0000e130: 0553 0029 054e 7a16 496e 2073 6174 6f64  .S.).Nz.In satod
+0000e140: 696d 655f 6765 745f 7075 626b 6579 e955  ime_get_pubkey.U
+0000e150: 0000 0072 bc00 0000 7201 0000 0029 0772  ...r....r....).r
+0000e160: 2700 0000 7234 0000 0072 2b00 0000 72be  '...r4...r+...r.
+0000e170: 0000 0072 9b00 0000 7277 0000 00da 1970  ...r....rw.....p
+0000e180: 6172 7365 5f73 6174 6f64 696d 655f 6765  arse_satodime_ge
+0000e190: 745f 7075 626b 6579 290d 7236 0000 0072  t_pubkey).r6...r
+0000e1a0: 8501 0000 72a1 0000 0072 8900 0000 72a2  ....r....r....r.
+0000e1b0: 0000 0072 a300 0000 729a 0000 0072 2200  ...r....r....r".
+0000e1c0: 0000 725e 0000 0072 5f00 0000 72fe 0000  ..r^...r_...r...
+0000e1d0: 00da 1070 7562 6b65 795f 636f 6d70 5f6c  ...pubkey_comp_l
+0000e1e0: 6973 74da 0873 6967 5f6c 6973 7472 3700  ist..sig_listr7.
+0000e1f0: 0000 7237 0000 0072 3800 0000 da13 7361  ..r7...r8.....sa
+0000e200: 746f 6469 6d65 5f67 6574 5f70 7562 6b65  todime_get_pubke
+0000e210: 7954 0800 0073 1200 0000 0001 0a01 0601  yT...s..........
+0000e220: 0401 0801 0402 0c01 1003 1202 7a21 4361  ............z!Ca
+0000e230: 7264 436f 6e6e 6563 746f 722e 7361 746f  rdConnector.sato
+0000e240: 6469 6d65 5f67 6574 5f70 7562 6b65 7963  dime_get_pubkeyc
+0000e250: 0200 0000 0000 0000 1100 0000 0600 0000  ................
+0000e260: 4300 0000 73ce 0000 0074 006a 0164 0183  C...s....t.j.d..
+0000e270: 0101 0074 026a 037d 0264 027d 037c 0164  ...t.j.}.d.}.|.d
+0000e280: 0316 007d 0464 047d 0574 0474 0517 007d  ...}.d.}.t.t...}
+0000e290: 067c 027c 037c 047c 057c 0667 057d 0774  .|.|.|.|.|.g.}.t
+0000e2a0: 0674 076a 0874 097c 006a 0a83 0174 097c  .t.j.t.|.j...t.|
+0000e2b0: 077c 006a 0b17 0083 0174 0c6a 0d83 036a  .|.j.....t.j...j
+0000e2c0: 0e83 0083 017d 087c 006a 0b7c 0817 007d  .....}.|.j.|...}
+0000e2d0: 0974 0f7c 0983 017c 066b 0372 8c74 1064  .t.|...|.k.r.t.d
+0000e2e0: 0574 0f7c 0983 019b 0064 067c 069b 009d  .t.|.....d.|....
+0000e2f0: 0483 0182 017c 077c 0917 007d 0a7c 006a  .....|.|...}.|.j
+0000e300: 117c 0a83 015c 037d 0b7d 0c7d 0d7c 006a  .|...\.}.}.}.|.j
+0000e310: 1283 0001 007c 006a 136a 147c 0b7c 0183  .....|.j.j.|.|..
+0000e320: 025c 037d 0e7d 0f7d 107c 0b7c 0c7c 0d7c  .\.}.}.}.|.|.|.|
+0000e330: 0e7c 0f66 0553 0029 074e 7a17 496e 2073  .|.f.S.).Nz.In s
+0000e340: 6174 6f64 696d 655f 6765 745f 7072 6976  atodime_get_priv
+0000e350: 6b65 79e9 5600 0000 72bc 0000 0072 0100  key.V...r....r..
+0000e360: 0000 7a2e 4572 726f 7220 696e 2073 6174  ..z.Error in sat
+0000e370: 6f64 696d 655f 7365 616c 5f6b 6579 3a20  odime_seal_key: 
+0000e380: 7772 6f6e 6720 6461 7461 206c 656e 6774  wrong data lengt
+0000e390: 6820 7a0c 2069 6e73 7465 6164 206f 6620  h z. instead of 
+0000e3a0: 2915 7227 0000 0072 3400 0000 722b 0000  ).r'...r4...r+..
+0000e3b0: 0072 be00 0000 7281 0000 0072 8a01 0000  .r....r....r....
+0000e3c0: 72c8 0000 0072 ed00 0000 728b 0100 0072  r....r....r....r
+0000e3d0: 4b00 0000 7280 0000 0072 8200 0000 724f  K...r....r....rO
+0000e3e0: 0000 0072 5000 0000 728c 0100 0072 3500  ...rP...r....r5.
+0000e3f0: 0000 7253 0000 0072 9b00 0000 727f 0100  ..rS...r....r...
+0000e400: 0072 7700 0000 da1a 7061 7273 655f 7361  .rw.....parse_sa
+0000e410: 746f 6469 6d65 5f67 6574 5f70 7269 766b  todime_get_privk
+0000e420: 6579 2911 7236 0000 0072 8501 0000 72a1  ey).r6...r....r.
+0000e430: 0000 0072 8900 0000 72a2 0000 0072 a300  ...r....r....r..
+0000e440: 0000 728d 0100 0072 8e01 0000 728f 0100  ..r....r....r...
+0000e450: 0072 cb00 0000 729a 0000 0072 2200 0000  .r....r....r"...
+0000e460: 725e 0000 0072 5f00 0000 da0c 656e 7472  r^...r_.....entr
+0000e470: 6f70 795f 6c69 7374 da0c 7072 6976 6b65  opy_list..privke
+0000e480: 795f 6c69 7374 7295 0100 0072 3700 0000  y_listr....r7...
+0000e490: 7237 0000 0072 3800 0000 da14 7361 746f  r7...r8.....sato
+0000e4a0: 6469 6d65 5f67 6574 5f70 7269 766b 6579  dime_get_privkey
+0000e4b0: 6308 0000 7320 0000 0000 010a 0106 0104  c...s ..........
+0000e4c0: 0108 0104 0108 010e 0328 020a 010c 0118  .........(......
+0000e4d0: 0108 0110 0108 0314 027a 2243 6172 6443  .........z"CardC
+0000e4e0: 6f6e 6e65 6374 6f72 2e73 6174 6f64 696d  onnector.satodim
+0000e4f0: 655f 6765 745f 7072 6976 6b65 7963 0300  e_get_privkeyc..
+0000e500: 0000 0000 0000 1200 0000 0600 0000 4300  ..............C.
+0000e510: 0000 73e8 0000 0074 006a 0164 0183 0101  ..s....t.j.d....
+0000e520: 0074 026a 037d 0364 027d 047c 0164 0316  .t.j.}.d.}.|.d..
+0000e530: 007d 0564 047d 0674 0474 0517 0074 0617  .}.d.}.t.t...t..
+0000e540: 007d 077c 037c 047c 057c 067c 0767 057d  .}.|.|.|.|.|.g.}
+0000e550: 0874 077c 0283 0174 086b 0872 4e74 097c  .t.|...t.k.rNt.|
+0000e560: 0283 017d 0274 0974 0a6a 0b74 087c 006a  ...}.t.t.j.t.|.j
+0000e570: 0c83 0174 087c 087c 006a 0d17 0083 0174  ...t.|.|.j.....t
+0000e580: 0e6a 0f83 036a 1083 0083 017d 097c 006a  .j...j.....}.|.j
+0000e590: 0d7c 0917 007c 0217 007d 0a74 117c 0a83  .|...|...}.t.|..
+0000e5a0: 017c 076b 0372 a874 1264 0574 117c 0a83  .|.k.r.t.d.t.|..
+0000e5b0: 019b 0064 067c 079b 009d 0483 0182 017c  ...d.|.........|
+0000e5c0: 087c 0a17 007d 0b7c 006a 137c 0b83 015c  .|...}.|.j.|...\
+0000e5d0: 037d 0c7d 0d7d 0e7c 006a 1483 0001 007c  .}.}.}.|.j.....|
+0000e5e0: 006a 156a 167c 0c83 015c 037d 0f7d 107d  .j.j.|...\.}.}.}
+0000e5f0: 117c 0c7c 0d7c 0e7c 0f7c 1066 0553 0029  .|.|.|.|.|.f.S.)
+0000e600: 074e 7a14 496e 2073 6174 6f64 696d 655f  .Nz.In satodime_
+0000e610: 7365 616c 5f6b 6579 e957 0000 0072 bc00  seal_key.W...r..
+0000e620: 0000 7201 0000 007a 2e45 7272 6f72 2069  ..r....z.Error i
+0000e630: 6e20 7361 746f 6469 6d65 5f73 6561 6c5f  n satodime_seal_
+0000e640: 6b65 793a 2077 726f 6e67 2064 6174 6120  key: wrong data 
+0000e650: 6c65 6e67 7468 207a 0c20 696e 7374 6561  length z. instea
+0000e660: 6420 6f66 2029 1772 2700 0000 7234 0000  d of ).r'...r4..
+0000e670: 0072 2b00 0000 72be 0000 0072 8100 0000  .r+...r....r....
+0000e680: 728a 0100 005a 0c53 495a 455f 454e 5452  r....Z.SIZE_ENTR
+0000e690: 4f50 5972 2600 0000 724b 0000 0072 c800  OPYr&...rK...r..
+0000e6a0: 0000 72ed 0000 0072 8b01 0000 7280 0000  ..r....r....r...
+0000e6b0: 0072 8200 0000 724f 0000 0072 5000 0000  .r....rO...rP...
+0000e6c0: 728c 0100 0072 3500 0000 7253 0000 0072  r....r5...rS...r
+0000e6d0: 9b00 0000 727f 0100 0072 7700 0000 7293  ....r....rw...r.
+0000e6e0: 0100 0029 1272 3600 0000 7285 0100 005a  ...).r6...r....Z
+0000e6f0: 0c65 6e74 726f 7079 5f75 7365 7272 a100  .entropy_userr..
+0000e700: 0000 7289 0000 0072 a200 0000 72a3 0000  ..r....r....r...
+0000e710: 0072 8d01 0000 728e 0100 0072 8f01 0000  .r....r....r....
+0000e720: 72cb 0000 0072 9a00 0000 7222 0000 0072  r....r....r"...r
+0000e730: 5e00 0000 725f 0000 0072 fe00 0000 7294  ^...r_...r....r.
+0000e740: 0100 0072 9501 0000 7237 0000 0072 3700  ...r....r7...r7.
+0000e750: 0000 7238 0000 00da 1173 6174 6f64 696d  ..r8.....satodim
+0000e760: 655f 7365 616c 5f6b 6579 7b08 0000 7324  e_seal_key{...s$
+0000e770: 0000 0000 020a 0106 0104 0108 0104 010c  ................
+0000e780: 010e 020c 0008 0328 020e 010c 0118 0108  .......(........
+0000e790: 0210 0108 0312 027a 1f43 6172 6443 6f6e  .......z.CardCon
+0000e7a0: 6e65 6374 6f72 2e73 6174 6f64 696d 655f  nector.satodime_
+0000e7b0: 7365 616c 5f6b 6579 6302 0000 0000 0000  seal_keyc.......
+0000e7c0: 0011 0000 0006 0000 0043 0000 0073 ce00  .........C...s..
+0000e7d0: 0000 7400 6a01 6401 8301 0100 7402 6a03  ..t.j.d.....t.j.
+0000e7e0: 7d02 6402 7d03 7c01 6403 1600 7d04 6404  }.d.}.|.d...}.d.
+0000e7f0: 7d05 7404 7405 1700 7d06 7c02 7c03 7c04  }.t.t...}.|.|.|.
+0000e800: 7c05 7c06 6705 7d07 7406 7407 6a08 7409  |.|.g.}.t.t.j.t.
+0000e810: 7c00 6a0a 8301 7409 7c07 7c00 6a0b 1700  |.j...t.|.|.j...
+0000e820: 8301 740c 6a0d 8303 6a0e 8300 8301 7d08  ..t.j...j.....}.
+0000e830: 7c00 6a0b 7c08 1700 7d09 740f 7c09 8301  |.j.|...}.t.|...
+0000e840: 7c06 6b03 728c 7410 6405 740f 7c09 8301  |.k.r.t.d.t.|...
+0000e850: 9b00 6406 7c06 9b00 9d04 8301 8201 7c07  ..d.|.........|.
+0000e860: 7c09 1700 7d0a 7c00 6a11 7c0a 8301 5c03  |...}.|.j.|...\.
+0000e870: 7d0b 7d0c 7d0d 7c00 6a12 8300 0100 7c00  }.}.}.|.j.....|.
+0000e880: 6a13 6a14 7c0b 7c01 8302 5c03 7d0e 7d0f  j.j.|.|...\.}.}.
+0000e890: 7d10 7c0b 7c0c 7c0d 7c0e 7c0f 6605 5300  }.|.|.|.|.|.f.S.
+0000e8a0: 2907 4e7a 1649 6e20 7361 746f 6469 6d65  ).Nz.In satodime
+0000e8b0: 5f75 6e73 6561 6c5f 6b65 79e9 5800 0000  _unseal_key.X...
+0000e8c0: 72bc 0000 0072 0100 0000 7a30 4572 726f  r....r....z0Erro
+0000e8d0: 7220 696e 2073 6174 6f64 696d 655f 756e  r in satodime_un
+0000e8e0: 7365 616c 5f6b 6579 3a20 7772 6f6e 6720  seal_key: wrong 
+0000e8f0: 6461 7461 206c 656e 6774 6820 7a0c 2069  data length z. i
+0000e900: 6e73 7465 6164 206f 6620 2915 7227 0000  nstead of ).r'..
+0000e910: 0072 3400 0000 722b 0000 0072 be00 0000  .r4...r+...r....
+0000e920: 7281 0000 0072 8a01 0000 72c8 0000 0072  r....r....r....r
+0000e930: ed00 0000 728b 0100 0072 4b00 0000 7280  ....r....rK...r.
+0000e940: 0000 0072 8200 0000 724f 0000 0072 5000  ...r....rO...rP.
+0000e950: 0000 728c 0100 0072 3500 0000 7253 0000  ..r....r5...rS..
+0000e960: 0072 9b00 0000 727f 0100 0072 7700 0000  .r....r....rw...
+0000e970: 7298 0100 0029 1172 3600 0000 7285 0100  r....).r6...r...
+0000e980: 0072 a100 0000 7289 0000 0072 a200 0000  .r....r....r....
+0000e990: 72a3 0000 0072 8d01 0000 728e 0100 0072  r....r....r....r
+0000e9a0: 8f01 0000 72cb 0000 0072 9a00 0000 7222  ....r....r....r"
+0000e9b0: 0000 0072 5e00 0000 725f 0000 0072 9901  ...r^...r_...r..
+0000e9c0: 0000 729a 0100 0072 9501 0000 7237 0000  ..r....r....r7..
+0000e9d0: 0072 3700 0000 7238 0000 00da 1373 6174  .r7...r8.....sat
+0000e9e0: 6f64 696d 655f 756e 7365 616c 5f6b 6579  odime_unseal_key
+0000e9f0: 9708 0000 7320 0000 0000 010a 0106 0104  ....s ..........
+0000ea00: 0108 0104 0108 010e 0328 020a 010c 0118  .........(......
+0000ea10: 0108 0210 0108 0314 027a 2143 6172 6443  .........z!CardC
+0000ea20: 6f6e 6e65 6374 6f72 2e73 6174 6f64 696d  onnector.satodim
+0000ea30: 655f 756e 7365 616c 5f6b 6579 6302 0000  e_unseal_keyc...
+0000ea40: 0000 0000 000e 0000 0006 0000 0043 0000  .............C..
+0000ea50: 0073 b600 0000 7400 6a01 6401 8301 0100  .s....t.j.d.....
+0000ea60: 7402 6a03 7d02 6402 7d03 7c01 6403 1600  t.j.}.d.}.|.d...
+0000ea70: 7d04 6404 7d05 7404 7405 1700 7d06 7c02  }.d.}.t.t...}.|.
+0000ea80: 7c03 7c04 7c05 7c06 6705 7d07 7406 7407  |.|.|.|.g.}.t.t.
+0000ea90: 6a08 7409 7c00 6a0a 8301 7409 7c07 7c00  j.t.|.j...t.|.|.
+0000eaa0: 6a0b 1700 8301 740c 6a0d 8303 6a0e 8300  j.....t.j...j...
+0000eab0: 8301 7d08 7c00 6a0b 7c08 1700 7d09 740f  ..}.|.j.|...}.t.
+0000eac0: 7c09 8301 7c06 6b03 728c 7410 6405 740f  |...|.k.r.t.d.t.
+0000ead0: 7c09 8301 9b00 6406 7c06 9b00 9d04 8301  |.....d.|.......
+0000eae0: 8201 7c07 7c09 1700 7d0a 7c00 6a11 7c0a  ..|.|...}.|.j.|.
+0000eaf0: 8301 5c03 7d0b 7d0c 7d0d 7c00 6a12 8300  ..\.}.}.}.|.j...
+0000eb00: 0100 7c0b 7c0c 7c0d 6603 5300 2907 4e7a  ..|.|.|.f.S.).Nz
+0000eb10: 1549 6e20 7361 746f 6469 6d65 5f72 6573  .In satodime_res
+0000eb20: 6574 5f6b 6579 e959 0000 0072 bc00 0000  et_key.Y...r....
+0000eb30: 7201 0000 007a 3045 7272 6f72 2069 6e20  r....z0Error in 
+0000eb40: 7361 746f 6469 6d65 5f75 6e73 6561 6c5f  satodime_unseal_
+0000eb50: 6b65 793a 2077 726f 6e67 2064 6174 6120  key: wrong data 
+0000eb60: 6c65 6e67 7468 207a 0c20 696e 7374 6561  length z. instea
+0000eb70: 6420 6f66 2029 1372 2700 0000 7234 0000  d of ).r'...r4..
+0000eb80: 0072 2b00 0000 72be 0000 0072 8100 0000  .r+...r....r....
+0000eb90: 728a 0100 0072 c800 0000 72ed 0000 0072  r....r....r....r
+0000eba0: 8b01 0000 724b 0000 0072 8000 0000 7282  ....rK...r....r.
+0000ebb0: 0000 0072 4f00 0000 7250 0000 0072 8c01  ...rO...rP...r..
+0000ebc0: 0000 7235 0000 0072 5300 0000 729b 0000  ..r5...rS...r...
+0000ebd0: 0072 7f01 0000 290e 7236 0000 0072 8501  .r....).r6...r..
+0000ebe0: 0000 72a1 0000 0072 8900 0000 72a2 0000  ..r....r....r...
+0000ebf0: 0072 a300 0000 728d 0100 0072 8e01 0000  .r....r....r....
+0000ec00: 728f 0100 0072 cb00 0000 729a 0000 0072  r....r....r....r
+0000ec10: 2200 0000 725e 0000 0072 5f00 0000 7237  "...r^...r_...r7
+0000ec20: 0000 0072 3700 0000 7238 0000 00da 1273  ...r7...r8.....s
+0000ec30: 6174 6f64 696d 655f 7265 7365 745f 6b65  atodime_reset_ke
+0000ec40: 79b0 0800 0073 1e00 0000 0001 0a01 0601  y....s..........
+0000ec50: 0401 0801 0401 0801 0e03 2802 0a01 0c01  ..........(.....
+0000ec60: 1801 0802 1001 0802 7a20 4361 7264 436f  ........z CardCo
+0000ec70: 6e6e 6563 746f 722e 7361 746f 6469 6d65  nnector.satodime
+0000ec80: 5f72 6573 6574 5f6b 6579 6301 0000 0000  _reset_keyc.....
+0000ec90: 0000 000d 0000 0006 0000 0043 0000 0073  ...........C...s
+0000eca0: 8e00 0000 7400 6a01 6401 8301 0100 7402  ....t.j.d.....t.
+0000ecb0: 6a03 7d01 6402 7d02 6403 7d03 6403 7d04  j.}.d.}.d.}.d.}.
+0000ecc0: 7404 7405 1700 7d05 7c01 7c02 7c03 7c04  t.t...}.|.|.|.|.
+0000ecd0: 7c05 6705 7d06 7406 7407 6a08 7409 7c00  |.g.}.t.t.j.t.|.
+0000ece0: 6a0a 8301 7409 7c06 7c00 6a0b 1700 8301  j...t.|.|.j.....
+0000ecf0: 740c 6a0d 8303 6a0e 8300 8301 7d07 7c00  t.j...j.....}.|.
+0000ed00: 6a0b 7c07 1700 7d08 7c06 7c08 1700 7d09  j.|...}.|.|...}.
+0000ed10: 7c00 6a0f 7c09 8301 5c03 7d0a 7d0b 7d0c  |.j.|...\.}.}.}.
+0000ed20: 7c00 6a10 8300 0100 7c0a 7c0b 7c0c 6603  |.j.....|.|.|.f.
+0000ed30: 5300 2904 4e7a 2749 6e20 7361 746f 6469  S.).Nz'In satodi
+0000ed40: 6d65 5f69 6e69 7469 6174 655f 6f77 6e65  me_initiate_owne
+0000ed50: 7273 6869 705f 7472 616e 7366 6572 e95a  rship_transfer.Z
+0000ed60: 0000 0072 0100 0000 2911 7227 0000 0072  ...r....).r'...r
+0000ed70: 3400 0000 722b 0000 0072 be00 0000 7281  4...r+...r....r.
+0000ed80: 0000 0072 8a01 0000 72c8 0000 0072 ed00  ...r....r....r..
+0000ed90: 0000 728b 0100 0072 4b00 0000 7280 0000  ..r....rK...r...
+0000eda0: 0072 8200 0000 724f 0000 0072 5000 0000  .r....rO...rP...
+0000edb0: 728c 0100 0072 9b00 0000 727f 0100 0029  r....r....r....)
+0000edc0: 0d72 3600 0000 72a1 0000 0072 8900 0000  .r6...r....r....
+0000edd0: 72a2 0000 0072 a300 0000 728d 0100 0072  r....r....r....r
+0000ede0: 8e01 0000 728f 0100 0072 cb00 0000 729a  ....r....r....r.
+0000edf0: 0000 0072 2200 0000 725e 0000 0072 5f00  ...r"...r^...r_.
+0000ee00: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
+0000ee10: 00da 2473 6174 6f64 696d 655f 696e 6974  ..$satodime_init
+0000ee20: 6961 7465 5f6f 776e 6572 7368 6970 5f74  iate_ownership_t
+0000ee30: 7261 6e73 6665 72c6 0800 0073 1a00 0000  ransfer....s....
+0000ee40: 0002 0a01 0601 0401 0401 0401 0801 0e03  ................
+0000ee50: 2802 0a01 0801 1001 0802 7a32 4361 7264  (.........z2Card
+0000ee60: 436f 6e6e 6563 746f 722e 7361 746f 6469  Connector.satodi
+0000ee70: 6d65 5f69 6e69 7469 6174 655f 6f77 6e65  me_initiate_owne
+0000ee80: 7273 6869 705f 7472 616e 7366 6572 6302  rship_transferc.
+0000ee90: 0000 0000 0000 0008 0000 0004 0000 0043  ...............C
+0000eea0: 0000 0073 5a00 0000 7400 6401 6402 8302  ...sZ...t.d.d...
+0000eeb0: 7d02 7400 7c01 8301 7d03 7401 6a02 7c02  }.t.|...}.t.j.|.
+0000eec0: 7c03 7403 6a04 8303 6a05 8300 6403 6404  |.t.j...j...d.d.
+0000eed0: 8502 1900 7d04 7406 7c04 8301 7d05 7c05  ....}.t.|...}.|.
+0000eee0: 6a07 6405 8301 7d06 7c06 6a08 8300 7d07  j.d...}.|.j...}.
+0000eef0: 7409 6a0a 6406 7c07 1700 8301 0100 7c07  t.j.d.|.......|.
+0000ef00: 5300 2907 4e7a 0d42 6974 636f 696e 2073  S.).Nz.Bitcoin s
+0000ef10: 6565 6432 72c1 0000 0072 0100 0000 720f  eed2r....r....r.
+0000ef20: 0100 0054 7a13 4175 7468 656e 7469 6b65  ...Tz.Authentike
+0000ef30: 795f 6c6f 6361 6c3d 2029 0b72 4b00 0000  y_local= ).rK...
+0000ef40: 72ed 0000 0072 8b01 0000 724f 0000 005a  r....r....rO...Z
+0000ef50: 0673 6861 3531 3272 8c01 0000 7211 0000  .sha512r....r...
+0000ef60: 0072 e300 0000 724c 0000 0072 2700 0000  .r....rL...r'...
+0000ef70: 7234 0000 0029 0872 3600 0000 5a0a 6d61  r4...).r6...Z.ma
+0000ef80: 7374 6572 7365 6564 5a07 6279 7465 6b65  sterseedZ.byteke
+0000ef90: 795a 0862 7974 6573 6565 6472 5001 0000  yZ.byteseedrP...
+0000efa0: 5a04 7072 6976 5a03 7075 625a 0770 7562  Z.privZ.pubZ.pub
+0000efb0: 5f68 6578 7237 0000 0072 3700 0000 7238  _hexr7...r7...r8
+0000efc0: 0000 00da 1f67 6574 5f61 7574 6865 6e74  .....get_authent
+0000efd0: 696b 6579 5f66 726f 6d5f 6d61 7374 6572  ikey_from_master
+0000efe0: 7365 6564 df08 0000 7310 0000 0000 030a  seed....s.......
+0000eff0: 0108 011c 0108 010a 0108 010e 027a 2d43  .............z-C
+0000f000: 6172 6443 6f6e 6e65 6374 6f72 2e67 6574  ardConnector.get
+0000f010: 5f61 7574 6865 6e74 696b 6579 5f66 726f  _authentikey_fro
+0000f020: 6d5f 6d61 7374 6572 7365 6564 2903 7201  m_masterseed).r.
+0000f030: 0000 004e 7201 0000 0029 0272 1e01 0000  ...Nr....).r....
+0000f040: 4e29 0146 2901 5429 014e 2901 4e29 0154  N).F).T).N).N).T
+0000f050: 2950 723a 0000 0072 3b00 0000 723c 0000  )Pr:...r;...r<..
+0000f060: 0072 ae00 0000 72af 0000 0072 b000 0000  .r....r....r....
+0000f070: 72b2 0000 00da 076c 6f67 6769 6e67 da07  r......logging..
+0000f080: 5741 524e 494e 4772 4000 0000 729b 0000  WARNINGr@...r...
+0000f090: 0072 9c00 0000 724a 0000 0072 4d00 0000  .r....rJ...rM...
+0000f0a0: 724e 0000 0072 5600 0000 72a7 0000 0072  rN...rV...r....r
+0000f0b0: 5500 0000 72aa 0000 0072 ab00 0000 72ac  U...r....r....r.
+0000f0c0: 0000 0072 5700 0000 72c7 0000 0072 cd00  ...rW...r....r..
+0000f0d0: 0000 72de 0000 0072 e800 0000 72f9 0000  ..r....r....r...
+0000f0e0: 0072 0001 0000 7202 0100 0072 0601 0000  .r....r....r....
+0000f0f0: 7208 0100 0072 0a01 0000 72e2 0000 0072  r....r....r....r
+0000f100: 1501 0000 721d 0100 0072 2801 0000 724b  ....r....r(...rK
+0000f110: 0000 0072 2a01 0000 722f 0100 0072 3101  ...r*...r/...r1.
+0000f120: 0000 7234 0100 0072 3601 0000 723f 0100  ..r4...r6...r?..
+0000f130: 0072 4101 0000 7242 0100 0072 9200 0000  .rA...rB...r....
+0000f140: 72d8 0000 0072 4b01 0000 724c 0100 0072  r....rK...rL...r
+0000f150: 4d01 0000 7259 0000 0072 8f00 0000 7291  M...rY...r....r.
+0000f160: 0000 0072 7600 0000 7257 0100 0072 5901  ...rv...rW...rY.
+0000f170: 0000 725f 0100 0072 6901 0000 726b 0100  ..r_...ri...rk..
+0000f180: 0072 6f01 0000 7271 0100 0072 7201 0000  .ro...rq...rr...
+0000f190: 7273 0100 0072 7401 0000 727a 0100 0072  rs...rt...rz...r
+0000f1a0: da00 0000 72d9 0000 0072 7f01 0000 7284  ....r....r....r.
+0000f1b0: 0100 0072 7c01 0000 7286 0100 0072 9001  ...r|...r....r..
+0000f1c0: 0000 7291 0100 0072 9601 0000 729b 0100  ..r....r....r...
+0000f1d0: 0072 9d01 0000 729f 0100 0072 a101 0000  .r....r....r....
+0000f1e0: 72a3 0100 0072 a401 0000 7237 0000 0072  r....r....r7...r
+0000f1f0: 3700 0000 7237 0000 0072 3800 0000 7264  7...r7...r8...rd
+0000f200: 0000 008f 0000 0073 9000 0000 080d 0c01  .......s........
+0000f210: 1401 1801 1402 122c 082c 0804 080b 080b  .......,.,......
+0000f220: 080b 0815 0803 0818 0807 0807 0807 0831  ...............1
+0000f230: 0819 0814 0a34 0830 0840 0827 0815 081e  .....4.0.@.'....
+0000f240: 0c21 081e 0813 0838 0826 0a57 102f 0823  .!.....8.&.W./.#
+0000f250: 0827 0821 081d 0a6a 080e 080c 083e 0805  .'.!...j.....>..
+0000f260: 0827 0823 0811 0817 0818 081a 0e1c 0e1c  .'.#............
+0000f270: 0a4e 0a5c 0823 0a42 081a 0812 0836 0811  .N.\.#.B.....6..
+0000f280: 0834 0c06 0c04 0805 0823 0e14 141e 0e1a  .4.......#......
+0000f290: 0e0f 0e18 0e1c 0e19 0e16 0819 7264 0000  ............rd..
+0000f2a0: 0063 0000 0000 0000 0000 0000 0000 0400  .c..............
+0000f2b0: 0000 0000 0000 7326 0000 0065 005a 0164  ......s&...e.Z.d
+0000f2c0: 005a 0264 0164 0164 0167 0066 0487 0066  .Z.d.d.d.g.f...f
+0000f2d0: 0164 0264 0384 095a 0387 0004 005a 0453  .d.d...Z.....Z.S
+0000f2e0: 0029 04da 0941 7064 7545 7272 6f72 7201  .)...ApduErrorr.
+0000f2f0: 0000 0063 0600 0000 0000 0000 0600 0000  ...c............
+0000f300: 0200 0000 0300 0000 7328 0000 0074 0083  ........s(...t..
+0000f310: 006a 017c 0183 0101 007c 027c 005f 027c  .j.|.....|.|._.|
+0000f320: 037c 005f 037c 047c 005f 047c 057c 005f  .|._.|.|._.|.|._
+0000f330: 0564 0053 0029 014e 2906 da05 7375 7065  .d.S.).N)...supe
+0000f340: 7272 4000 0000 725e 0000 0072 5f00 0000  rr@...r^...r_...
+0000f350: 7289 0000 0072 2200 0000 2906 7236 0000  r....r"...).r6..
+0000f360: 0072 2301 0000 725e 0000 0072 5f00 0000  .r#...r^...r_...
+0000f370: 7289 0000 0072 2200 0000 2901 da09 5f5f  r....r"...)...__
+0000f380: 636c 6173 735f 5f72 3700 0000 7238 0000  class__r7...r8..
+0000f390: 0072 4000 0000 f208 0000 730a 0000 0000  .r@.......s.....
+0000f3a0: 010c 0106 0106 0106 017a 1241 7064 7545  .........z.ApduE
+0000f3b0: 7272 6f72 2e5f 5f69 6e69 745f 5f29 0572  rror.__init__).r
+0000f3c0: 3a00 0000 723b 0000 0072 3c00 0000 7240  :...r;...r<...r@
+0000f3d0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+0000f3e0: 5f5f 7237 0000 0072 3700 0000 2901 72a9  __r7...r7...).r.
+0000f3f0: 0100 0072 3800 0000 72a7 0100 00f1 0800  ...r8...r.......
+0000f400: 0073 0200 0000 0801 72a7 0100 0063 0000  .s......r....c..
+0000f410: 0000 0000 0000 0000 0000 0400 0000 0000  ................
+0000f420: 0000 7322 0000 0065 005a 0164 005a 0264  ..s"...e.Z.d.Z.d
+0000f430: 0167 0066 0287 0066 0164 0264 0384 095a  .g.f...f.d.d...Z
+0000f440: 0387 0004 005a 0453 0029 0472 9300 0000  .....Z.S.).r....
+0000f450: 7201 0000 0063 0400 0000 0000 0000 0400  r....c..........
+0000f460: 0000 0600 0000 0300 0000 7318 0000 0074  ..........s....t
+0000f470: 0083 006a 017c 0164 0164 027c 027c 0383  ...j.|.d.d.|.|..
+0000f480: 0501 0064 0053 0029 034e 7288 0000 0072  ...d.S.).Nr....r
+0000f490: 8600 0000 2902 72a8 0100 0072 4000 0000  ....).r....r@...
+0000f4a0: 2904 7236 0000 0072 2301 0000 7289 0000  ).r6...r#...r...
+0000f4b0: 0072 2200 0000 2901 72a9 0100 0072 3700  .r"...).r....r7.
+0000f4c0: 0000 7238 0000 0072 4000 0000 fb08 0000  ..r8...r@.......
+0000f4d0: 7302 0000 0000 017a 1843 6172 6453 656c  s......z.CardSel
+0000f4e0: 6563 7445 7272 6f72 2e5f 5f69 6e69 745f  ectError.__init_
+0000f4f0: 5f29 0572 3a00 0000 723b 0000 0072 3c00  _).r:...r;...r<.
+0000f500: 0000 7240 0000 0072 aa01 0000 7237 0000  ..r@...r....r7..
+0000f510: 0072 3700 0000 2901 72a9 0100 0072 3800  .r7...).r....r8.
+0000f520: 0000 7293 0000 00fa 0800 0073 0200 0000  ..r........s....
+0000f530: 0801 7293 0000 0063 0000 0000 0000 0000  ..r....c........
+0000f540: 0000 0000 0400 0000 0000 0000 7322 0000  ............s"..
+0000f550: 0065 005a 0164 005a 0264 0167 0066 0287  .e.Z.d.Z.d.g.f..
+0000f560: 0066 0164 0264 0384 095a 0387 0004 005a  .f.d.d...Z.....Z
+0000f570: 0453 0029 0472 8301 0000 7201 0000 0063  .S.).r....r....c
+0000f580: 0400 0000 0000 0000 0400 0000 0600 0000  ................
+0000f590: 0300 0000 7318 0000 0074 0083 006a 017c  ....s....t...j.|
+0000f5a0: 0164 0164 027c 027c 0383 0501 0064 0053  .d.d.|.|.....d.S
+0000f5b0: 0029 034e 7242 0000 0072 4300 0000 2902  .).NrB...rC...).
+0000f5c0: 72a8 0100 0072 4000 0000 2904 7236 0000  r....r@...).r6..
+0000f5d0: 0072 2301 0000 7289 0000 0072 2200 0000  .r#...r....r"...
+0000f5e0: 2901 72a9 0100 0072 3700 0000 7238 0000  ).r....r7...r8..
+0000f5f0: 0072 4000 0000 0009 0000 7302 0000 0000  .r@.......s.....
+0000f600: 017a 1e43 6172 6453 6574 7570 4e6f 7444  .z.CardSetupNotD
+0000f610: 6f6e 6545 7272 6f72 2e5f 5f69 6e69 745f  oneError.__init_
+0000f620: 5f29 0572 3a00 0000 723b 0000 0072 3c00  _).r:...r;...r<.
+0000f630: 0000 7240 0000 0072 aa01 0000 7237 0000  ..r@...r....r7..
+0000f640: 0072 3700 0000 2901 72a9 0100 0072 3800  .r7...).r....r8.
+0000f650: 0000 7283 0100 00ff 0800 0073 0200 0000  ..r........s....
+0000f660: 0801 7283 0100 0063 0000 0000 0000 0000  ..r....c........
+0000f670: 0000 0000 0400 0000 0000 0000 7322 0000  ............s"..
+0000f680: 0065 005a 0164 005a 0264 0167 0066 0287  .e.Z.d.Z.d.g.f..
+0000f690: 0066 0164 0264 0384 095a 0387 0004 005a  .f.d.d...Z.....Z
+0000f6a0: 0453 0029 0472 9400 0000 7201 0000 0063  .S.).r....r....c
+0000f6b0: 0400 0000 0000 0000 0400 0000 0600 0000  ................
+0000f6c0: 0300 0000 7318 0000 0074 0083 006a 017c  ....s....t...j.|
+0000f6d0: 0164 0164 027c 027c 0383 0501 0064 0053  .d.d.|.|.....d.S
+0000f6e0: 0029 034e 7242 0000 0072 8a00 0000 2902  .).NrB...r....).
+0000f6f0: 72a8 0100 0072 4000 0000 2904 7236 0000  r....r@...).r6..
+0000f700: 0072 2301 0000 7289 0000 0072 2200 0000  .r#...r....r"...
+0000f710: 2901 72a9 0100 0072 3700 0000 7238 0000  ).r....r7...r8..
+0000f720: 0072 4000 0000 0409 0000 7302 0000 0000  .r@.......s.....
+0000f730: 017a 1949 6e63 6f72 7265 6374 5031 4572  .z.IncorrectP1Er
+0000f740: 726f 722e 5f5f 696e 6974 5f5f 2905 723a  ror.__init__).r:
+0000f750: 0000 0072 3b00 0000 723c 0000 0072 4000  ...r;...r<...r@.
+0000f760: 0000 72aa 0100 0072 3700 0000 7237 0000  ..r....r7...r7..
+0000f770: 0029 0172 a901 0000 7238 0000 0072 9400  .).r....r8...r..
+0000f780: 0000 0309 0000 7302 0000 0008 0172 9400  ......s......r..
+0000f790: 0000 6300 0000 0000 0000 0000 0000 0004  ..c.............
+0000f7a0: 0000 0000 0000 0073 2200 0000 6500 5a01  .......s"...e.Z.
+0000f7b0: 6400 5a02 6401 6700 6602 8700 6601 6402  d.Z.d.g.f...f.d.
+0000f7c0: 6403 8409 5a03 8700 0400 5a04 5300 2904  d...Z.....Z.S.).
+0000f7d0: 7298 0000 0072 0100 0000 6304 0000 0000  r....r....c.....
+0000f7e0: 0000 0004 0000 0006 0000 0003 0000 0073  ...............s
+0000f7f0: 1800 0000 7400 8300 6a01 7c01 6401 6402  ....t...j.|.d.d.
+0000f800: 7c02 7c03 8305 0100 6400 5300 2903 4e72  |.|.....d.S.).Nr
+0000f810: 4200 0000 728d 0000 0029 0272 a801 0000  B...r....).r....
+0000f820: 7240 0000 0029 0472 3600 0000 7223 0100  r@...).r6...r#..
+0000f830: 0072 8900 0000 7222 0000 0029 0172 a901  .r....r"...).r..
+0000f840: 0000 7237 0000 0072 3800 0000 7240 0000  ..r7...r8...r@..
+0000f850: 0009 0900 0073 0200 0000 0001 7a22 556e  .....s......z"Un
+0000f860: 6b6e 6f77 6e50 726f 746f 636f 6c4d 6564  knownProtocolMed
+0000f870: 6961 4572 726f 722e 5f5f 696e 6974 5f5f  iaError.__init__
+0000f880: 2905 723a 0000 0072 3b00 0000 723c 0000  ).r:...r;...r<..
+0000f890: 0072 4000 0000 72aa 0100 0072 3700 0000  .r@...r....r7...
+0000f8a0: 7237 0000 0029 0172 a901 0000 7238 0000  r7...).r....r8..
+0000f8b0: 0072 9800 0000 0809 0000 7302 0000 0008  .r........s.....
+0000f8c0: 0172 9800 0000 6300 0000 0000 0000 0000  .r....c.........
+0000f8d0: 0000 0004 0000 0000 0000 0073 2200 0000  ...........s"...
+0000f8e0: 6500 5a01 6400 5a02 6401 6700 6602 8700  e.Z.d.Z.d.g.f...
+0000f8f0: 6601 6402 6403 8409 5a03 8700 0400 5a04  f.d.d...Z.....Z.
+0000f900: 5300 2904 7297 0000 0072 0100 0000 6304  S.).r....r....c.
+0000f910: 0000 0000 0000 0004 0000 0006 0000 0003  ................
+0000f920: 0000 0073 1800 0000 7400 8300 6a01 7c01  ...s....t...j.|.
+0000f930: 6401 6402 7c02 7c03 8305 0100 6400 5300  d.d.|.|.....d.S.
+0000f940: 2903 4e72 4200 0000 7266 0000 0029 0272  ).NrB...rf...).r
+0000f950: a801 0000 7240 0000 0029 0472 3600 0000  ....r@...).r6...
+0000f960: 7223 0100 0072 8900 0000 7222 0000 0029  r#...r....r"...)
+0000f970: 0172 a901 0000 7237 0000 0072 3800 0000  .r....r7...r8...
+0000f980: 7240 0000 000d 0900 0073 0200 0000 0001  r@.......s......
+0000f990: 7a24 496e 636f 7272 6563 7450 726f 746f  z$IncorrectProto
+0000f9a0: 636f 6c4d 6564 6961 4572 726f 722e 5f5f  colMediaError.__
+0000f9b0: 696e 6974 5f5f 2905 723a 0000 0072 3b00  init__).r:...r;.
+0000f9c0: 0000 723c 0000 0072 4000 0000 72aa 0100  ..r<...r@...r...
+0000f9d0: 0072 3700 0000 7237 0000 0029 0172 a901  .r7...r7...).r..
+0000f9e0: 0000 7238 0000 0072 9700 0000 0c09 0000  ..r8...r........
+0000f9f0: 7302 0000 0008 0172 9700 0000 6300 0000  s......r....c...
+0000fa00: 0000 0000 0000 0000 0004 0000 0000 0000  ................
+0000fa10: 0073 2200 0000 6500 5a01 6400 5a02 6401  .s"...e.Z.d.Z.d.
+0000fa20: 6700 6602 8700 6601 6402 6403 8409 5a03  g.f...f.d.d...Z.
+0000fa30: 8700 0400 5a04 5300 2904 7296 0000 0072  ....Z.S.).r....r
+0000fa40: 0100 0000 6304 0000 0000 0000 0004 0000  ....c...........
+0000fa50: 0006 0000 0003 0000 0073 1800 0000 7400  .........s....t.
+0000fa60: 8300 6a01 7c01 6401 6402 7c02 7c03 8305  ..j.|.d.d.|.|...
+0000fa70: 0100 6400 5300 2903 4e72 4200 0000 728c  ..d.S.).NrB...r.
+0000fa80: 0000 0029 0272 a801 0000 7240 0000 0029  ...).r....r@...)
+0000fa90: 0472 3600 0000 7223 0100 0072 8900 0000  .r6...r#...r....
+0000faa0: 7222 0000 0029 0172 a901 0000 7237 0000  r"...).r....r7..
+0000fab0: 0072 3800 0000 7240 0000 0011 0900 0073  .r8...r@.......s
+0000fac0: 0200 0000 0001 7a23 496e 636f 7272 6563  ......z#Incorrec
+0000fad0: 744b 6579 736c 6f74 5374 6174 6545 7272  tKeyslotStateErr
+0000fae0: 6f72 2e5f 5f69 6e69 745f 5f29 0572 3a00  or.__init__).r:.
+0000faf0: 0000 723b 0000 0072 3c00 0000 7240 0000  ..r;...r<...r@..
+0000fb00: 0072 aa01 0000 7237 0000 0072 3700 0000  .r....r7...r7...
+0000fb10: 2901 72a9 0100 0072 3800 0000 7296 0000  ).r....r8...r...
+0000fb20: 0010 0900 0073 0200 0000 0801 7296 0000  .....s......r...
+0000fb30: 0063 0000 0000 0000 0000 0000 0000 0400  .c..............
+0000fb40: 0000 0000 0000 7322 0000 0065 005a 0164  ......s"...e.Z.d
+0000fb50: 005a 0264 0167 0066 0287 0066 0164 0264  .Z.d.g.f...f.d.d
+0000fb60: 0384 095a 0387 0004 005a 0453 0029 0472  ...Z.....Z.S.).r
+0000fb70: 9500 0000 7201 0000 0063 0400 0000 0000  ....r....c......
+0000fb80: 0000 0400 0000 0600 0000 0300 0000 7318  ..............s.
+0000fb90: 0000 0074 0083 006a 017c 0164 0164 027c  ...t...j.|.d.d.|
+0000fba0: 027c 0383 0501 0064 0053 0029 034e 7242  .|.....d.S.).NrB
+0000fbb0: 0000 0072 8b00 0000 2902 72a8 0100 0072  ...r....).r....r
+0000fbc0: 4000 0000 2904 7236 0000 0072 2301 0000  @...).r6...r#...
+0000fbd0: 7289 0000 0072 2200 0000 2901 72a9 0100  r....r"...).r...
+0000fbe0: 0072 3700 0000 7238 0000 0072 4000 0000  .r7...r8...r@...
+0000fbf0: 1509 0000 7302 0000 0000 017a 2149 6e63  ....s......z!Inc
+0000fc00: 6f72 7265 6374 556e 6c6f 636b 436f 6465  orrectUnlockCode
+0000fc10: 4572 726f 722e 5f5f 696e 6974 5f5f 2905  Error.__init__).
+0000fc20: 723a 0000 0072 3b00 0000 723c 0000 0072  r:...r;...r<...r
+0000fc30: 4000 0000 72aa 0100 0072 3700 0000 7237  @...r....r7...r7
+0000fc40: 0000 0029 0172 a901 0000 7238 0000 0072  ...).r....r8...r
+0000fc50: 9500 0000 1409 0000 7302 0000 0008 0172  ........s......r
+0000fc60: 9500 0000 6300 0000 0000 0000 0000 0000  ....c...........
+0000fc70: 0004 0000 0000 0000 0073 2200 0000 6500  .........s"...e.
+0000fc80: 5a01 6400 5a02 6401 6700 6602 8700 6601  Z.d.Z.d.g.f...f.
+0000fc90: 6402 6403 8409 5a03 8700 0400 5a04 5300  d.d...Z.....Z.S.
+0000fca0: 2904 da1b 496e 636f 7272 6563 7455 6e6c  )...IncorrectUnl
+0000fcb0: 6f63 6b43 6f75 6e74 6572 4572 726f 7272  ockCounterErrorr
+0000fcc0: 0100 0000 6304 0000 0000 0000 0004 0000  ....c...........
+0000fcd0: 0006 0000 0003 0000 0073 1800 0000 7400  .........s....t.
+0000fce0: 8300 6a01 7c01 6401 6402 7c02 7c03 8305  ..j.|.d.d.|.|...
+0000fcf0: 0100 6400 5300 2903 4e72 4200 0000 7280  ..d.S.).NrB...r.
+0000fd00: 0100 0029 0272 a801 0000 7240 0000 0029  ...).r....r@...)
+0000fd10: 0472 3600 0000 7223 0100 0072 8900 0000  .r6...r#...r....
+0000fd20: 7222 0000 0029 0172 a901 0000 7237 0000  r"...).r....r7..
+0000fd30: 0072 3800 0000 7240 0000 0019 0900 0073  .r8...r@.......s
+0000fd40: 0200 0000 0001 7a24 496e 636f 7272 6563  ......z$Incorrec
+0000fd50: 7455 6e6c 6f63 6b43 6f75 6e74 6572 4572  tUnlockCounterEr
+0000fd60: 726f 722e 5f5f 696e 6974 5f5f 2905 723a  ror.__init__).r:
+0000fd70: 0000 0072 3b00 0000 723c 0000 0072 4000  ...r;...r<...r@.
+0000fd80: 0000 72aa 0100 0072 3700 0000 7237 0000  ..r....r7...r7..
+0000fd90: 0029 0172 a901 0000 7238 0000 0072 ab01  .).r....r8...r..
+0000fda0: 0000 1809 0000 7302 0000 0008 0172 ab01  ......s......r..
+0000fdb0: 0000 6300 0000 0000 0000 0000 0000 0001  ..c.............
+0000fdc0: 0000 0040 0000 0073 1000 0000 6500 5a01  ...@...s....e.Z.
+0000fdd0: 6400 5a02 6401 5a03 6402 5300 2903 da13  d.Z.d.Z.d.S.)...
+0000fde0: 4175 7468 656e 7469 6361 7469 6f6e 4572  AuthenticationEr
+0000fdf0: 726f 727a 3552 6169 7365 6420 7768 656e  rorz5Raised when
+0000fe00: 2074 6865 2063 6f6d 6d61 6e64 2072 6571   the command req
+0000fe10: 7569 7265 7320 6175 7468 656e 7469 6361  uires authentica
+0000fe20: 7469 6f6e 2066 6972 7374 4e29 0472 3a00  tion firstN).r:.
+0000fe30: 0000 723b 0000 0072 3c00 0000 7263 0000  ..r;...r<...rc..
+0000fe40: 0072 3700 0000 7237 0000 0072 3700 0000  .r7...r7...r7...
+0000fe50: 7238 0000 0072 ac01 0000 1d09 0000 7304  r8...r........s.
+0000fe60: 0000 0008 0104 0172 ac01 0000 6300 0000  .......r....c...
+0000fe70: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+0000fe80: 0073 1000 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+0000fe90: 5a03 6402 5300 2903 7204 0100 007a 2852  Z.d.S.).r....z(R
+0000fea0: 6169 7365 6420 7768 656e 2074 6865 2064  aised when the d
+0000feb0: 6576 6963 6520 6973 206e 6f74 2079 6574  evice is not yet
+0000fec0: 2073 6565 6465 644e 2904 723a 0000 0072   seededN).r:...r
+0000fed0: 3b00 0000 723c 0000 0072 6300 0000 7237  ;...r<...rc...r7
+0000fee0: 0000 0072 3700 0000 7237 0000 0072 3800  ...r7...r7...r8.
+0000fef0: 0000 7204 0100 0021 0900 0073 0400 0000  ..r....!...s....
+0000ff00: 0801 0401 7204 0100 0063 0000 0000 0000  ....r....c......
+0000ff10: 0000 0000 0000 0100 0000 4000 0000 7310  ..........@...s.
+0000ff20: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+0000ff30: 0253 0029 0372 f400 0000 7a37 5261 6973  .S.).r....z7Rais
+0000ff40: 6564 2077 6865 6e20 7468 6520 6465 7669  ed when the devi
+0000ff50: 6365 2072 6574 7572 6e73 2061 6e20 756e  ce returns an un
+0000ff60: 6578 7065 6374 6564 2065 7272 6f72 2063  expected error c
+0000ff70: 6f64 654e 2904 723a 0000 0072 3b00 0000  odeN).r:...r;...
+0000ff80: 723c 0000 0072 6300 0000 7237 0000 0072  r<...rc...r7...r
+0000ff90: 3700 0000 7237 0000 0072 3800 0000 72f4  7...r7...r8...r.
+0000ffa0: 0000 0025 0900 0073 0400 0000 0801 0401  ...%...s........
+0000ffb0: 72f4 0000 0063 0000 0000 0000 0000 0000  r....c..........
+0000ffc0: 0000 0100 0000 4000 0000 7310 0000 0065  ......@...s....e
+0000ffd0: 005a 0164 005a 0264 015a 0364 0253 0029  .Z.d.Z.d.Z.d.S.)
+0000ffe0: 0372 e500 0000 7a2c 5261 6973 6564 2077  .r....z,Raised w
+0000fff0: 6865 6e20 7468 6520 6465 7669 6365 2072  hen the device r
+00010000: 6574 7572 6e73 2061 6e20 6572 726f 7220  eturns an error 
+00010010: 636f 6465 4e29 0472 3a00 0000 723b 0000  codeN).r:...r;..
+00010020: 0072 3c00 0000 7263 0000 0072 3700 0000  .r<...rc...r7...
+00010030: 7237 0000 0072 3700 0000 7238 0000 0072  r7...r7...r8...r
+00010040: e500 0000 2809 0000 7304 0000 0008 0104  ....(...s.......
+00010050: 0172 e500 0000 6300 0000 0000 0000 0000  .r....c.........
+00010060: 0000 0001 0000 0040 0000 0073 1000 0000  .......@...s....
+00010070: 6500 5a01 6400 5a02 6401 5a03 6402 5300  e.Z.d.Z.d.Z.d.S.
+00010080: 2903 7299 0000 007a 2c52 6169 7365 6420  ).r....z,Raised 
+00010090: 7768 656e 2074 6865 2064 6576 6963 6520  when the device 
+000100a0: 7265 7475 726e 7320 616e 2065 7272 6f72  returns an error
+000100b0: 2063 6f64 654e 2904 723a 0000 0072 3b00   codeN).r:...r;.
+000100c0: 0000 723c 0000 0072 6300 0000 7237 0000  ..r<...rc...r7..
+000100d0: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
+000100e0: 7299 0000 002c 0900 0073 0400 0000 0801  r....,...s......
+000100f0: 0401 7299 0000 0063 0000 0000 0000 0000  ..r....c........
+00010100: 0000 0000 0100 0000 4000 0000 7310 0000  ........@...s...
+00010110: 0065 005a 0164 005a 0264 015a 0364 0253  .e.Z.d.Z.d.Z.d.S
+00010120: 0029 0372 5b01 0000 7a32 5261 6973 6564  .).r[...z2Raised
+00010130: 2077 6865 6e20 616e 2065 7272 6f72 2069   when an error i
+00010140: 7320 7265 7475 726e 6564 2062 7920 7468  s returned by th
+00010150: 6520 5365 6564 4b65 6570 6572 4e29 0472  e SeedKeeperN).r
+00010160: 3a00 0000 723b 0000 0072 3c00 0000 7263  :...r;...r<...rc
+00010170: 0000 0072 3700 0000 7237 0000 0072 3700  ...r7...r7...r7.
+00010180: 0000 7238 0000 0072 5b01 0000 3009 0000  ..r8...r[...0...
+00010190: 7304 0000 0008 0104 0172 5b01 0000 da08  s........r[.....
+000101a0: 5f5f 6d61 696e 5f5f 2905 7219 0000 0072  __main__).r....r
+000101b0: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
+000101c0: 0000 0029 475a 1273 6d61 7274 6361 7264  ...)GZ.smartcard
+000101d0: 2e43 6172 6454 7970 6572 0200 0000 5a15  .CardTyper....Z.
+000101e0: 736d 6172 7463 6172 642e 4361 7264 5265  smartcard.CardRe
+000101f0: 7175 6573 7472 0300 0000 5a20 736d 6172  questr....Z smar
+00010200: 7463 6172 642e 4361 7264 436f 6e6e 6563  tcard.CardConnec
+00010210: 7469 6f6e 4f62 7365 7276 6572 7204 0000  tionObserverr...
+00010220: 005a 1873 6d61 7274 6361 7264 2e43 6172  .Z.smartcard.Car
+00010230: 644d 6f6e 6974 6f72 696e 6772 0500 0000  dMonitoringr....
+00010240: 7206 0000 005a 1473 6d61 7274 6361 7264  r....Z.smartcard
+00010250: 2e45 7863 6570 7469 6f6e 7372 0700 0000  .Exceptionsr....
+00010260: 7208 0000 005a 0e73 6d61 7274 6361 7264  r....Z.smartcard
+00010270: 2e75 7469 6c72 0900 0000 720a 0000 005a  .utilr....r....Z
+00010280: 1973 6d61 7274 6361 7264 2e73 772e 5357  .smartcard.sw.SW
+00010290: 4578 6365 7074 696f 6e73 720b 0000 0072  Exceptionsr....r
+000102a0: 2b00 0000 720e 0000 0072 0f00 0000 5a03  +...r....r....Z.
+000102b0: 6563 6372 1000 0000 7211 0000 0072 1200  eccr....r....r..
+000102c0: 0000 da04 7574 696c 7213 0000 0072 1400  ....utilr....r..
+000102d0: 0000 7215 0000 0072 1600 0000 5a15 6365  ..r....r....Z.ce
+000102e0: 7274 6966 6963 6174 655f 7661 6c69 6461  rtificate_valida
+000102f0: 746f 7272 1700 0000 724f 0000 0072 ed00  torr....rO...r..
+00010300: 0000 723d 0100 0072 a501 0000 da02 6f73  ..r=...r......os
+00010310: 7218 0000 00da 0967 6574 4c6f 6767 6572  r......getLogger
+00010320: 723a 0000 0072 2700 0000 7275 0000 00da  r:...r'...ru....
+00010330: 0544 4542 5547 7205 0100 005a 0b4d 5347  .DEBUGr....Z.MSG
+00010340: 5f55 5345 5f32 4641 7218 0100 0072 1a01  _USE_2FAr....r..
+00010350: 0000 721b 0100 0072 1e00 0000 723d 0000  ..r....r....r=..
+00010360: 0072 6400 0000 7253 0000 0072 a701 0000  .rd...rS...r....
+00010370: 7293 0000 0072 8301 0000 7294 0000 0072  r....r....r....r
+00010380: 9800 0000 7297 0000 0072 9600 0000 7295  ....r....r....r.
+00010390: 0000 0072 ab01 0000 72ac 0100 0072 0401  ...r....r....r..
+000103a0: 0000 72f4 0000 0072 e500 0000 7299 0000  ..r....r....r...
+000103b0: 0072 5b01 0000 5a0d 6361 7264 636f 6e6e  .r[...Z.cardconn
+000103c0: 6563 746f 7272 9c00 0000 7255 0000 0072  ectorr....rU...r
+000103d0: 0a01 0000 7256 0000 0072 3700 0000 7237  ....rV...r7...r7
+000103e0: 0000 0072 3700 0000 7238 0000 00da 083c  ...r7...r8.....<
+000103f0: 6d6f 6475 6c65 3e01 0000 0073 9200 0000  module>....s....
+00010400: 0c01 0c01 0c01 1001 1001 1001 0c02 0801  ................
+00010410: 0c01 0c01 1001 0c01 1801 0c02 0801 0801  ................
+00010420: 0801 0801 0c06 0a01 0c02 0405 0408 0402  ................
+00010430: 0201 0201 0201 0201 0803 0201 0201 0201  ................
+00010440: 0201 0804 1015 103e 0e7f 007f 007f 007f  .......>........
+00010450: 007f 007f 007f 007f 007f 007f 007f 007f  ................
+00010460: 007f 007f 007f 007f 0072 1009 1005 1004  .........r......
+00010470: 1005 1004 1004 1004 1004 1005 1004 1004  ................
+00010480: 1003 1004 1004 1005 0a02 0601 0801 0802  ................
+00010490: 0802                                     ..
```

### Comparing `pysatochip-0.14.1/pysatochip/__pycache__/Satochip2FA.cpython-36.pyc` & `pysatochip-0.14.2/pysatochip/__pycache__/Satochip2FA.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/__pycache__/certificate_validator.cpython-36.pyc` & `pysatochip-0.14.2/pysatochip/__pycache__/certificate_validator.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 7b88 8961 f02c 0000 e300 0000  3...{..a.,......
+00000000: 330d 0d0a 1cea ad61 f02c 0000 e300 0000  3......a.,......
 00000010: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
 00000020: 0073 4800 0000 6400 6401 6c00 5a00 6400  .sH...d.d.l.Z.d.
 00000030: 6401 6c01 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6502 6a04 6505 8301 5a06  d.l.Z.e.j.e...Z.
 00000050: 6506 6a07 6502 6a08 8301 0100 4700 6402  e.j.e.j.....G.d.
 00000060: 6403 8400 6403 8302 5a09 6401 5300 2904  d...d...Z.d.S.).
 00000070: e900 0000 004e 6300 0000 0000 0000 0000  .....Nc.........
```

### Comparing `pysatochip-0.14.1/pysatochip/JCconstants.py` & `pysatochip-0.14.2/pysatochip/JCconstants.py`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/cert/test-subca-seedkeeper.cert` & `pysatochip-0.14.2/pysatochip/cert/test-subca-seedkeeper.cert`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/cert/ca.cert` & `pysatochip-0.14.2/pysatochip/cert/ca.cert`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/cert/subca-satochip.cert` & `pysatochip-0.14.2/pysatochip/cert/subca-satochip.cert`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/cert/test-ca.cert` & `pysatochip-0.14.2/pysatochip/cert/test-ca.cert`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/cert/test-subca-satodime.cert` & `pysatochip-0.14.2/pysatochip/cert/test-subca-satodime.cert`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/cert/subca-satodime.cert` & `pysatochip-0.14.2/pysatochip/cert/subca-satodime.cert`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/cert/subca-seedkeeper.cert` & `pysatochip-0.14.2/pysatochip/cert/subca-seedkeeper.cert`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/cert/test-subca-satochip.cert` & `pysatochip-0.14.2/pysatochip/cert/test-subca-satochip.cert`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/certificate_validator.py` & `pysatochip-0.14.2/pysatochip/certificate_validator.py`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/CardDataParser.py` & `pysatochip-0.14.2/pysatochip/CardDataParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -579,16 +579,18 @@
         key_asset_txt= DIC_ASSET_BY_CODE.get(key_asset, f"Unknown code {key_asset}")
         key_slip44_hex= bytes(key_slip44).hex() # todo!
         
         size_contract= key_contract[1]
         key_contract_hex= "0x"+ bytes(key_contract[2:(2+size_contract)]).hex() # parse as tlv
         #key_contract_hex= bytes(key_contract).hex() # todo: parse as tlv
         size_tokenid= key_tokenid[1]
-        key_tokenid_hex= "0x"+ bytes(key_tokenid[2:(2+size_tokenid)]).hex() # parse as tlv
-        #key_tokenid_hex= bytes(key_tokenid).hex() #todo
+        key_tokenid_bytes= bytes(key_tokenid[2:(2+size_tokenid)]) 
+        key_tokenid_hex= "0x"+ key_tokenid_bytes.hex() # parse as tlv
+        key_tokenid_int= int.from_bytes( key_tokenid_bytes, "big")  
+        
         size_data= key_data[1] # key_data[0] is RFU (could be used as a type tag)
         key_data_txt= bytes(key_data[2:(2+size_data)]).decode("utf-8")  #parse as tlv-encoded utf8 string
         #key_data_txt= bytes(key_data).hex() #todo
         
         # token/nft
         is_token= False
         is_nft= False
@@ -598,15 +600,15 @@
             is_nft= True
         
         keyslot_status={'key_status':key_status, 'key_type':key_type, 
                                 'key_asset':key_asset, 'key_slip44':key_slip44, 'key_contract':key_contract, 
                                 'key_tokenid':key_tokenid, 'key_data':key_data,
                                 'key_status_txt':key_status_txt, 
                                 'key_asset_txt':key_asset_txt, 'key_slip44_hex':key_slip44_hex,
-                                'key_contract_hex':key_contract_hex, 'key_tokenid_hex':key_tokenid_hex,
+                                'key_contract_hex':key_contract_hex, 'key_tokenid_hex':key_tokenid_hex, 'key_tokenid_int':key_tokenid_int,
                                 'key_data_txt':key_data_txt, 'is_token':is_token, 'is_nft':is_nft}
         
         return keyslot_status
         
     def parse_satodime_get_pubkey(self, response):
     
         # response= [ pubkey_size(2b) | pubkey | sig_size(2b) | sig ]
```

### Comparing `pysatochip-0.14.1/pysatochip/TxParser.py` & `pysatochip-0.14.2/pysatochip/TxParser.py`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/Satochip2FA.py` & `pysatochip-0.14.2/pysatochip/Satochip2FA.py`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/ecc.py` & `pysatochip-0.14.2/pysatochip/ecc.py`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip/SecureChannel.py` & `pysatochip-0.14.2/pysatochip/SecureChannel.py`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/PKG-INFO` & `pysatochip-0.14.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysatochip
-Version: 0.14.1
+Version: 0.14.2
 Summary: Simple python library to communicate with a Satochip hardware wallet
 Home-page: https://github.com/Toporin/pysatochip
 Author: Toporin
 Author-email: satochip.wallet@gmail.com
 License: UNKNOWN
 Project-URL: Github, https://github.com/Toporin
 Project-URL: Webshop, https://satochip.io/
```

### Comparing `pysatochip-0.14.1/CHANGELOG.md` & `pysatochip-0.14.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.14.2]:
+
+Some minor improvements & corrections to support Satochip & Satodime.
+ - Patch https://github.com/Toporin/pysatochip/issues/3
+ - Satodime support: add is_owner field
+ - Satodime support: add key_tokenid_int field
+
 ## [0.14.1]:
 
 - Add support for Satodime : the open-source bearer crypto card
 Website: satodime.io
 Github: https://github.com/Toporin/Satodime-Applet
 
 ### Added
```

### Comparing `pysatochip-0.14.1/README.md` & `pysatochip-0.14.2/README.md`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/LICENSE` & `pysatochip-0.14.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysatochip-0.14.1/pysatochip.egg-info/PKG-INFO` & `pysatochip-0.14.2/pysatochip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysatochip
-Version: 0.14.1
+Version: 0.14.2
 Summary: Simple python library to communicate with a Satochip hardware wallet
 Home-page: https://github.com/Toporin/pysatochip
 Author: Toporin
 Author-email: satochip.wallet@gmail.com
 License: UNKNOWN
 Project-URL: Github, https://github.com/Toporin
 Project-URL: Webshop, https://satochip.io/
```

### Comparing `pysatochip-0.14.1/pysatochip.egg-info/SOURCES.txt` & `pysatochip-0.14.2/pysatochip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

