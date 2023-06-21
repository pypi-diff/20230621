# Comparing `tmp/etsy-apiv3-1.9.2.tar.gz` & `tmp/etsy-apiv3-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etsy-apiv3-1.9.2.tar", last modified: Fri Jun 16 14:14:27 2023, max compression
+gzip compressed data, was "etsy-apiv3-1.9.3.tar", last modified: Wed Jun 21 11:43:58 2023, max compression
```

## Comparing `etsy-apiv3-1.9.2.tar` & `etsy-apiv3-1.9.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 14:14:27.247527 etsy-apiv3-1.9.2/
--rw-rw-rw-   0        0        0     1089 2022-11-29 15:57:22.000000 etsy-apiv3-1.9.2/LICENSE
--rw-rw-rw-   0        0        0      342 2023-06-16 14:14:27.247527 etsy-apiv3-1.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     1120 2022-12-02 14:38:46.000000 etsy-apiv3-1.9.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 14:14:27.131656 etsy-apiv3-1.9.2/etsy_apiv3/
--rw-rw-rw-   0        0        0       23 2023-06-16 14:14:13.000000 etsy-apiv3-1.9.2/etsy_apiv3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:14:27.147277 etsy-apiv3-1.9.2/etsy_apiv3/exceptions/
--rw-rw-rw-   0        0        0      549 2023-05-15 08:29:30.000000 etsy-apiv3-1.9.2/etsy_apiv3/exceptions/TokenExpiredError.py
--rw-rw-rw-   0        0        0        0 2023-05-20 08:39:21.000000 etsy-apiv3-1.9.2/etsy_apiv3/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:14:27.216281 etsy-apiv3-1.9.2/etsy_apiv3/models/
--rw-rw-rw-   0        0        0      126 2023-01-05 12:58:42.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/Auth.py
--rw-rw-rw-   0        0        0      293 2023-01-05 11:18:24.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/File.py
--rw-rw-rw-   0        0        0      604 2022-06-06 13:20:33.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ListingImageModel.py
--rw-rw-rw-   0        0        0     3966 2023-04-25 14:30:59.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ListingModel.py
--rw-rw-rw-   0        0        0      293 2022-04-23 21:35:29.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ListingPropertyModel.py
--rw-rw-rw-   0        0        0      255 2022-11-29 15:27:15.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/OfferingModel.py
--rw-rw-rw-   0        0        0     2124 2023-01-12 13:28:51.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/PaymentModel.py
--rw-rw-rw-   0        0        0      116 2022-04-04 14:44:43.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/PriceModel.py
--rw-rw-rw-   0        0        0      334 2022-11-29 15:27:25.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ProductModel.py
--rw-rw-rw-   0        0        0      143 2022-04-05 14:24:47.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ProductionPartnerModel.py
--rw-rw-rw-   0        0        0      303 2022-07-02 07:06:56.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/PropertyValueModel.py
--rw-rw-rw-   0        0        0     1961 2022-11-29 15:27:49.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ReceiptModel.py
--rw-rw-rw-   0        0        0      199 2022-11-29 15:27:55.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/RefundModel.py
--rw-rw-rw-   0        0        0      245 2023-01-05 13:51:36.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ReturnPolicyModel.py
--rw-rw-rw-   0        0        0      394 2022-04-23 16:26:45.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ReviewModel.py
--rw-rw-rw-   0        0        0      254 2022-10-15 18:09:39.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ShipmentModel.py
--rw-rw-rw-   0        0        0      293 2023-01-06 08:26:38.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ShippingCarrierModel.py
--rw-rw-rw-   0        0        0      537 2023-01-28 10:35:20.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ShippingProfileDestinationModel.py
--rw-rw-rw-   0        0        0      698 2022-11-29 15:28:16.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ShippingProfileModel.py
--rw-rw-rw-   0        0        0      381 2022-11-29 15:28:31.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ShippingProfileUpgradeModel.py
--rw-rw-rw-   0        0        0     1609 2022-07-02 07:49:17.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ShopModel.py
--rw-rw-rw-   0        0        0      171 2023-01-05 13:22:47.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/ShopSection.py
--rw-rw-rw-   0        0        0      930 2023-01-06 07:39:02.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/TaxonomyModel.py
--rw-rw-rw-   0        0        0      146 2023-05-15 08:25:27.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/TokenModel.py
--rw-rw-rw-   0        0        0      974 2023-02-18 13:56:54.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/TransactionModel.py
--rw-rw-rw-   0        0        0      187 2022-04-05 14:20:33.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/TranslationModel.py
--rw-rw-rw-   0        0        0      728 2023-01-05 12:33:05.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/UserModel.py
--rw-rw-rw-   0        0        0      202 2022-04-05 14:03:40.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/VariationModel.py
--rw-rw-rw-   0        0        0     1224 2023-01-06 12:04:29.000000 etsy-apiv3-1.9.2/etsy_apiv3/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:14:27.231903 etsy-apiv3-1.9.2/etsy_apiv3/resources/
--rw-rw-rw-   0        0        0    17771 2023-05-31 13:58:29.000000 etsy-apiv3-1.9.2/etsy_apiv3/resources/ListingResource.py
--rw-rw-rw-   0        0        0     2645 2023-05-20 08:40:36.000000 etsy-apiv3-1.9.2/etsy_apiv3/resources/PaymentResource.py
--rw-rw-rw-   0        0        0     5940 2023-05-20 08:40:46.000000 etsy-apiv3-1.9.2/etsy_apiv3/resources/ReceiptResource.py
--rw-rw-rw-   0        0        0     1395 2023-05-20 08:41:00.000000 etsy-apiv3-1.9.2/etsy_apiv3/resources/ReviewResource.py
--rw-rw-rw-   0        0        0     6087 2023-05-20 08:41:07.000000 etsy-apiv3-1.9.2/etsy_apiv3/resources/ShippingProfileResource.py
--rw-rw-rw-   0        0        0     2792 2023-05-20 08:41:16.000000 etsy-apiv3-1.9.2/etsy_apiv3/resources/ShopPolicyResource.py
--rw-rw-rw-   0        0        0     3810 2023-05-20 08:41:27.000000 etsy-apiv3-1.9.2/etsy_apiv3/resources/ShopResource.py
--rw-rw-rw-   0        0        0      190 2023-01-06 12:19:53.000000 etsy-apiv3-1.9.2/etsy_apiv3/resources/UserResource.py
--rw-rw-rw-   0        0        0      222 2023-01-12 13:29:03.000000 etsy-apiv3-1.9.2/etsy_apiv3/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:14:27.231903 etsy-apiv3-1.9.2/etsy_apiv3/utils/
--rw-rw-rw-   0        0        0     4091 2023-04-06 13:41:59.000000 etsy-apiv3-1.9.2/etsy_apiv3/utils/APIV3.py
--rw-rw-rw-   0        0        0     5526 2023-06-16 14:14:05.000000 etsy-apiv3-1.9.2/etsy_apiv3/utils/EtsyOauth2Session.py
--rw-rw-rw-   0        0        0      474 2022-04-22 20:27:32.000000 etsy-apiv3-1.9.2/etsy_apiv3/utils/RequestException.py
--rw-rw-rw-   0        0        0      218 2022-07-02 14:30:58.000000 etsy-apiv3-1.9.2/etsy_apiv3/utils/Response.py
--rw-rw-rw-   0        0        0      154 2023-05-20 08:15:27.000000 etsy-apiv3-1.9.2/etsy_apiv3/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:14:27.147277 etsy-apiv3-1.9.2/etsy_apiv3.egg-info/
--rw-rw-rw-   0        0        0      342 2023-06-16 14:14:26.000000 etsy-apiv3-1.9.2/etsy_apiv3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1962 2023-06-16 14:14:27.000000 etsy-apiv3-1.9.2/etsy_apiv3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 14:14:26.000000 etsy-apiv3-1.9.2/etsy_apiv3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-06-16 14:14:26.000000 etsy-apiv3-1.9.2/etsy_apiv3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-16 14:14:26.000000 etsy-apiv3-1.9.2/etsy_apiv3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 14:14:27.247527 etsy-apiv3-1.9.2/setup.cfg
--rw-rw-rw-   0        0        0      746 2023-02-18 14:12:46.000000 etsy-apiv3-1.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:14:27.247527 etsy-apiv3-1.9.2/tests/
--rw-rw-rw-   0        0        0     2246 2023-01-12 13:49:46.000000 etsy-apiv3-1.9.2/tests/Payment.py
--rw-rw-rw-   0        0        0     3880 2023-03-15 09:02:53.000000 etsy-apiv3-1.9.2/tests/Receipt.py
--rw-rw-rw-   0        0        0        0 2023-03-15 09:02:44.000000 etsy-apiv3-1.9.2/tests/__init__.py
--rw-rw-rw-   0        0        0      539 2023-01-13 08:43:06.000000 etsy-apiv3-1.9.2/tests/taxonomy_test.py
--rw-rw-rw-   0        0        0      426 2023-01-12 11:25:14.000000 etsy-apiv3-1.9.2/tests/test_credentials.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:43:58.417062 etsy-apiv3-1.9.3/
+-rw-rw-rw-   0        0        0     1089 2022-11-29 15:57:22.000000 etsy-apiv3-1.9.3/LICENSE
+-rw-rw-rw-   0        0        0      342 2023-06-21 11:43:58.417062 etsy-apiv3-1.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1120 2022-12-02 14:38:46.000000 etsy-apiv3-1.9.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 11:43:58.034504 etsy-apiv3-1.9.3/etsy_apiv3/
+-rw-rw-rw-   0        0        0       23 2023-06-21 11:32:04.000000 etsy-apiv3-1.9.3/etsy_apiv3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:43:58.056861 etsy-apiv3-1.9.3/etsy_apiv3/exceptions/
+-rw-rw-rw-   0        0        0      549 2023-05-15 08:29:30.000000 etsy-apiv3-1.9.3/etsy_apiv3/exceptions/TokenExpiredError.py
+-rw-rw-rw-   0        0        0        0 2023-05-20 08:39:21.000000 etsy-apiv3-1.9.3/etsy_apiv3/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:43:58.291655 etsy-apiv3-1.9.3/etsy_apiv3/models/
+-rw-rw-rw-   0        0        0      126 2023-01-05 12:58:42.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/Auth.py
+-rw-rw-rw-   0        0        0      293 2023-01-05 11:18:24.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/File.py
+-rw-rw-rw-   0        0        0      604 2022-06-06 13:20:33.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ListingImageModel.py
+-rw-rw-rw-   0        0        0     3966 2023-04-25 14:30:59.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ListingModel.py
+-rw-rw-rw-   0        0        0      293 2022-04-23 21:35:29.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ListingPropertyModel.py
+-rw-rw-rw-   0        0        0      255 2022-11-29 15:27:15.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/OfferingModel.py
+-rw-rw-rw-   0        0        0     2124 2023-01-12 13:28:51.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/PaymentModel.py
+-rw-rw-rw-   0        0        0      116 2022-04-04 14:44:43.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/PriceModel.py
+-rw-rw-rw-   0        0        0      334 2022-11-29 15:27:25.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ProductModel.py
+-rw-rw-rw-   0        0        0      143 2022-04-05 14:24:47.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ProductionPartnerModel.py
+-rw-rw-rw-   0        0        0      303 2022-07-02 07:06:56.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/PropertyValueModel.py
+-rw-rw-rw-   0        0        0     1961 2022-11-29 15:27:49.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ReceiptModel.py
+-rw-rw-rw-   0        0        0      199 2022-11-29 15:27:55.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/RefundModel.py
+-rw-rw-rw-   0        0        0      245 2023-01-05 13:51:36.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ReturnPolicyModel.py
+-rw-rw-rw-   0        0        0      394 2022-04-23 16:26:45.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ReviewModel.py
+-rw-rw-rw-   0        0        0      254 2022-10-15 18:09:39.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ShipmentModel.py
+-rw-rw-rw-   0        0        0      293 2023-01-06 08:26:38.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ShippingCarrierModel.py
+-rw-rw-rw-   0        0        0      537 2023-01-28 10:35:20.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ShippingProfileDestinationModel.py
+-rw-rw-rw-   0        0        0      698 2022-11-29 15:28:16.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ShippingProfileModel.py
+-rw-rw-rw-   0        0        0      381 2022-11-29 15:28:31.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ShippingProfileUpgradeModel.py
+-rw-rw-rw-   0        0        0     1609 2022-07-02 07:49:17.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ShopModel.py
+-rw-rw-rw-   0        0        0      171 2023-01-05 13:22:47.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/ShopSection.py
+-rw-rw-rw-   0        0        0      930 2023-01-06 07:39:02.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/TaxonomyModel.py
+-rw-rw-rw-   0        0        0      146 2023-05-15 08:25:27.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/TokenModel.py
+-rw-rw-rw-   0        0        0      974 2023-02-18 13:56:54.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/TransactionModel.py
+-rw-rw-rw-   0        0        0      187 2022-04-05 14:20:33.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/TranslationModel.py
+-rw-rw-rw-   0        0        0      728 2023-01-05 12:33:05.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/UserModel.py
+-rw-rw-rw-   0        0        0      202 2022-04-05 14:03:40.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/VariationModel.py
+-rw-rw-rw-   0        0        0     1224 2023-01-06 12:04:29.000000 etsy-apiv3-1.9.3/etsy_apiv3/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:43:58.357062 etsy-apiv3-1.9.3/etsy_apiv3/resources/
+-rw-rw-rw-   0        0        0    17850 2023-06-21 09:28:24.000000 etsy-apiv3-1.9.3/etsy_apiv3/resources/ListingResource.py
+-rw-rw-rw-   0        0        0     2645 2023-05-20 08:40:36.000000 etsy-apiv3-1.9.3/etsy_apiv3/resources/PaymentResource.py
+-rw-rw-rw-   0        0        0     5940 2023-05-20 08:40:46.000000 etsy-apiv3-1.9.3/etsy_apiv3/resources/ReceiptResource.py
+-rw-rw-rw-   0        0        0     1395 2023-05-20 08:41:00.000000 etsy-apiv3-1.9.3/etsy_apiv3/resources/ReviewResource.py
+-rw-rw-rw-   0        0        0     6087 2023-05-20 08:41:07.000000 etsy-apiv3-1.9.3/etsy_apiv3/resources/ShippingProfileResource.py
+-rw-rw-rw-   0        0        0     2792 2023-05-20 08:41:16.000000 etsy-apiv3-1.9.3/etsy_apiv3/resources/ShopPolicyResource.py
+-rw-rw-rw-   0        0        0     3810 2023-05-20 08:41:27.000000 etsy-apiv3-1.9.3/etsy_apiv3/resources/ShopResource.py
+-rw-rw-rw-   0        0        0      190 2023-01-06 12:19:53.000000 etsy-apiv3-1.9.3/etsy_apiv3/resources/UserResource.py
+-rw-rw-rw-   0        0        0      222 2023-01-12 13:29:03.000000 etsy-apiv3-1.9.3/etsy_apiv3/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:43:58.386795 etsy-apiv3-1.9.3/etsy_apiv3/utils/
+-rw-rw-rw-   0        0        0     4091 2023-04-06 13:41:59.000000 etsy-apiv3-1.9.3/etsy_apiv3/utils/APIV3.py
+-rw-rw-rw-   0        0        0     5705 2023-06-21 09:28:33.000000 etsy-apiv3-1.9.3/etsy_apiv3/utils/EtsyOauth2Session.py
+-rw-rw-rw-   0        0        0      474 2022-04-22 20:27:32.000000 etsy-apiv3-1.9.3/etsy_apiv3/utils/RequestException.py
+-rw-rw-rw-   0        0        0      218 2022-07-02 14:30:58.000000 etsy-apiv3-1.9.3/etsy_apiv3/utils/Response.py
+-rw-rw-rw-   0        0        0      154 2023-05-20 08:15:27.000000 etsy-apiv3-1.9.3/etsy_apiv3/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:43:58.056861 etsy-apiv3-1.9.3/etsy_apiv3.egg-info/
+-rw-rw-rw-   0        0        0      342 2023-06-21 11:43:57.000000 etsy-apiv3-1.9.3/etsy_apiv3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1962 2023-06-21 11:43:57.000000 etsy-apiv3-1.9.3/etsy_apiv3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 11:43:57.000000 etsy-apiv3-1.9.3/etsy_apiv3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-06-21 11:43:57.000000 etsy-apiv3-1.9.3/etsy_apiv3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-21 11:43:57.000000 etsy-apiv3-1.9.3/etsy_apiv3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 11:43:58.417062 etsy-apiv3-1.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      746 2023-02-18 14:12:46.000000 etsy-apiv3-1.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 11:43:58.417062 etsy-apiv3-1.9.3/tests/
+-rw-rw-rw-   0        0        0     2246 2023-01-12 13:49:46.000000 etsy-apiv3-1.9.3/tests/Payment.py
+-rw-rw-rw-   0        0        0     3880 2023-03-15 09:02:53.000000 etsy-apiv3-1.9.3/tests/Receipt.py
+-rw-rw-rw-   0        0        0        0 2023-03-15 09:02:44.000000 etsy-apiv3-1.9.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      539 2023-01-13 08:43:06.000000 etsy-apiv3-1.9.3/tests/taxonomy_test.py
+-rw-rw-rw-   0        0        0      426 2023-01-12 11:25:14.000000 etsy-apiv3-1.9.3/tests/test_credentials.py
```

### Comparing `etsy-apiv3-1.9.2/LICENSE` & `etsy-apiv3-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/README.md` & `etsy-apiv3-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/exceptions/TokenExpiredError.py` & `etsy-apiv3-1.9.3/etsy_apiv3/exceptions/TokenExpiredError.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/models/ListingImageModel.py` & `etsy-apiv3-1.9.3/etsy_apiv3/models/ListingImageModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/models/ListingModel.py` & `etsy-apiv3-1.9.3/etsy_apiv3/models/ListingModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/models/PaymentModel.py` & `etsy-apiv3-1.9.3/etsy_apiv3/models/PaymentModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/models/ReceiptModel.py` & `etsy-apiv3-1.9.3/etsy_apiv3/models/ReceiptModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/models/ShippingProfileDestinationModel.py` & `etsy-apiv3-1.9.3/etsy_apiv3/models/ShippingProfileDestinationModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/models/ShippingProfileModel.py` & `etsy-apiv3-1.9.3/etsy_apiv3/models/ShippingProfileModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/models/ShopModel.py` & `etsy-apiv3-1.9.3/etsy_apiv3/models/ShopModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/models/TaxonomyModel.py` & `etsy-apiv3-1.9.3/etsy_apiv3/models/TaxonomyModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/models/TransactionModel.py` & `etsy-apiv3-1.9.3/etsy_apiv3/models/TransactionModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/models/UserModel.py` & `etsy-apiv3-1.9.3/etsy_apiv3/models/UserModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/models/__init__.py` & `etsy-apiv3-1.9.3/etsy_apiv3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/resources/ListingResource.py` & `etsy-apiv3-1.9.3/etsy_apiv3/resources/ListingResource.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,22 +251,25 @@
         data = {"variation_images": [image.dict() for image in variation_images]}
         response = self.session.request(endpoint, "POST", data=data)
         return Response[VariationImage](**response)
     
     def upload_listing_image(self, shop_id: int, listing_id: int, image: bytes, listing_image_id: int, rank: int = 1, overwrite: bool = False, is_watermarked: bool = False, alt_text: str = "") -> ListingImage:
         endpoint = f"shops/{shop_id}/listings/{listing_id}/images"
         data = {
-            "image": image,
-            "listing_image_id": listing_image_id,
+            #"image": image,
+            #"listing_image_id": None,
             "rank": rank,
             "overwrite": overwrite,
             "is_watermarked": is_watermarked,
             "alt_text": alt_text
         }
-        response = self.session.request(endpoint, "POST", data=data)
+        print(type(image))
+        response = self.session.request(endpoint, "POST", data=data, files={"image": image})
+        
+        
         return ListingImage(**response)
     
     def upload_multiple_images_to_listing(self, shop_id: int, listing_id: int, images: List[bytes], overwrite: bool = False, is_watermarked: bool = False, alt_text: str = "") -> List[ListingImage]:
         response = self.get_listing_images_by_id(listing_id=listing_id)
         new_listing_image_id = response.results[-1].listing_image_id + 1
         uploaded_images = []
         for image in images:
@@ -302,15 +305,15 @@
     def delete_listing_video(self, shop_id: int, listing_id: int, video_id: int) -> str:
         endpoint = f"shops/{shop_id}/listings/{listing_id}/videos/{video_id}"
         response = self.session.request(endpoint, "DELETE")
         return response
 
     def create_draft_listing(self, shop_id: int, listing: DraftListing) -> Listing:
         endpoint = f"shops/{shop_id}/listings"
-        response = self.session.request(endpoint, "POST", data=listing.dict())
+        response = self.session.request(endpoint, "POST", data=listing.dict(exclude_none=True))
         return Listing(**response)
     
     def get_buyer_taxonomy_nodes(self) -> Response[Taxonomy]:
         endpoint = "buyer-taxonomy/nodes"
         response = self.session.request(endpoint)
         return Response[Taxonomy](**response)
```

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/resources/PaymentResource.py` & `etsy-apiv3-1.9.3/etsy_apiv3/resources/PaymentResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/resources/ReceiptResource.py` & `etsy-apiv3-1.9.3/etsy_apiv3/resources/ReceiptResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/resources/ReviewResource.py` & `etsy-apiv3-1.9.3/etsy_apiv3/resources/ReviewResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/resources/ShippingProfileResource.py` & `etsy-apiv3-1.9.3/etsy_apiv3/resources/ShippingProfileResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/resources/ShopPolicyResource.py` & `etsy-apiv3-1.9.3/etsy_apiv3/resources/ShopPolicyResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/resources/ShopResource.py` & `etsy-apiv3-1.9.3/etsy_apiv3/resources/ShopResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/utils/APIV3.py` & `etsy-apiv3-1.9.3/etsy_apiv3/utils/APIV3.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3/utils/EtsyOauth2Session.py` & `etsy-apiv3-1.9.3/etsy_apiv3/utils/EtsyOauth2Session.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,18 +30,14 @@
         if self.token is not None:
             if token_updater is None:
                 self.token_updater = self._token_updater
             else:
                 self.token_updater = token_updater
                 
             self.headers["Authorization"] = f"{token.token_type} {token.access_token}"
-        
-        
-        
-        
         self.client_id = client_id
         self.client = Client(timeout=30.0)
         self.limits = APILimit(
             limit_per_second=None,
             remaining_this_second=None,
             limit_per_day=None,
             remaining_today=None
@@ -85,42 +81,50 @@
 
         Returns:
             json: Json From Request Response
         """
         base_endpoint = "https://openapi.etsy.com/v3/application/"
         url = f"{base_endpoint}{endpoint}"
         
-        res = self.client.request(method, url, headers=self.headers, *args, **kwargs)
+        headers = self.headers
+        if kwargs.get("headers") is not None:
+            headers.update(kwargs.get("headers"))
+            kwargs.pop("headers")
+        
+        print(headers)
+        print(kwargs.get("data"))
+        res = self.client.request(method, url, headers=headers, *args, **kwargs)
         res_json = res.json()
         
         if "X-Limit-Per-Day" in res.headers.keys():
             
             self.limits.limit_per_day = res.headers["X-Limit-Per-Day"]
             self.limits.limit_per_second = res.headers["X-Limit-Per-Second"]
             self.limits.remaining_this_second = res.headers["X-Remaining-This-Second"]
             self.limits.remaining_today = res.headers["X-Remaining-Today"]
         
         
-        if res.status_code == 200:
-            return res.json()
+        
+        print(res_json)
+        
+        if res.status_code == 200 or res.status_code == 201:
+            return res_json
         
         if res.status_code == 401:
             if res_json["error"] == "invalid_token":
                 updated = self.refresh_token()
                 if updated:
                     return self.request(endpoint, method, *args, **kwargs)
                 else:
                     raise TokenExpiredError(
                         status_code=res.status_code,
                         message=res_json["error_description"],
                         error=res_json["error"]
                     )
-
-            raise EtsyRequestException(res.status_code, res_json["error"])
-        else:
+            
             raise EtsyRequestException(res.status_code, res_json["error"])
             
         
     
 
 class EtsyOauth2Helper:
```

### Comparing `etsy-apiv3-1.9.2/etsy_apiv3.egg-info/SOURCES.txt` & `etsy-apiv3-1.9.3/etsy_apiv3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/setup.py` & `etsy-apiv3-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/tests/Payment.py` & `etsy-apiv3-1.9.3/tests/Payment.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/tests/Receipt.py` & `etsy-apiv3-1.9.3/tests/Receipt.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.9.2/tests/taxonomy_test.py` & `etsy-apiv3-1.9.3/tests/taxonomy_test.py`

 * *Files identical despite different names*

