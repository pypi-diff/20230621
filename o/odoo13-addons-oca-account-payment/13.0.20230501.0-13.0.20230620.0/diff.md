# Comparing `tmp/odoo13_addons_oca_account_payment-13.0.20230501.0-py3-none-any.whl.zip` & `tmp/odoo13_addons_oca_account_payment-13.0.20230620.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1597 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1551 b- defN 23-May-02 03:05 odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 03:05 odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-02 03:05 odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      441 b- defN 23-May-02 03:05 odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/RECORD
-4 files, 2085 bytes uncompressed, 727 bytes compressed:  65.1%
+Zip file size: 1620 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1748 b- defN 23-Jun-21 02:47 odoo13_addons_oca_account_payment-13.0.20230620.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 02:47 odoo13_addons_oca_account_payment-13.0.20230620.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-21 02:47 odoo13_addons_oca_account_payment-13.0.20230620.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      441 b- defN 23-Jun-21 02:47 odoo13_addons_oca_account_payment-13.0.20230620.0.dist-info/RECORD
+4 files, 2282 bytes uncompressed, 750 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/METADATA
+Filename: odoo13_addons_oca_account_payment-13.0.20230620.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/WHEEL
+Filename: odoo13_addons_oca_account_payment-13.0.20230620.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/top_level.txt
+Filename: odoo13_addons_oca_account_payment-13.0.20230620.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/RECORD
+Filename: odoo13_addons_oca_account_payment-13.0.20230620.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo13_addons_oca_account_payment-13.0.20230501.0.dist-info/METADATA` & `odoo13_addons_oca_account_payment-13.0.20230620.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo13-addons-oca-account-payment
-Version: 13.0.20230501.0
+Version: 13.0.20230620.0
 Summary: Meta package for oca-account-payment Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 13.0
@@ -22,14 +22,17 @@
 Requires-Dist: odoo13-addon-account-payment-promissory-note
 Requires-Dist: odoo13-addon-account-payment-return
 Requires-Dist: odoo13-addon-account-payment-return-import
 Requires-Dist: odoo13-addon-account-payment-return-import-iso20022
 Requires-Dist: odoo13-addon-account-payment-show-invoice
 Requires-Dist: odoo13-addon-account-payment-term-extension
 Requires-Dist: odoo13-addon-account-payment-term-partner-holiday
+Requires-Dist: odoo13-addon-account-payment-term-restriction
+Requires-Dist: odoo13-addon-account-payment-term-restriction-purchase
+Requires-Dist: odoo13-addon-account-payment-term-restriction-sale
 Requires-Dist: odoo13-addon-account-payment-term-security
 Requires-Dist: odoo13-addon-partner-aging
 Requires-Dist: odoo13-addon-sale-payment-mgmt
 Requires-Dist: odoo13-addon-sale-payment-term-security
 
 UNKNOWN
```

