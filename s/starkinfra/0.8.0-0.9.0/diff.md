# Comparing `tmp/starkinfra-0.8.0.tar.gz` & `tmp/starkinfra-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starkinfra-0.8.0.tar", last modified: Thu May 11 17:41:38 2023, max compression
+gzip compressed data, was "starkinfra-0.9.0.tar", last modified: Wed Jun 21 14:42:38 2023, max compression
```

## Comparing `starkinfra-0.8.0.tar` & `starkinfra-0.9.0.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.736128 starkinfra-0.8.0/
--rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-01 13:39:31.000000 starkinfra-0.8.0/LICENSE.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-01 13:39:31.000000 starkinfra-0.8.0/MANIFEST.in
--rw-r--r--   0 caiodottori   (501) staff       (20)    71335 2023-05-11 17:41:38.735823 starkinfra-0.8.0/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)    70917 2023-05-11 17:39:45.000000 starkinfra-0.8.0/README.md
--rw-r--r--   0 caiodottori   (501) staff       (20)       38 2023-05-11 17:41:38.736191 starkinfra-0.8.0/setup.cfg
--rw-r--r--   0 caiodottori   (501) staff       (20)      828 2023-04-27 20:25:01.000000 starkinfra-0.8.0/setup.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.561650 starkinfra-0.8.0/starkinfra/
--rw-r--r--   0 caiodottori   (501) staff       (20)     3392 2023-05-11 17:40:28.000000 starkinfra-0.8.0/starkinfra/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.566926 starkinfra-0.8.0/starkinfra/brcodepreview/
--rw-r--r--   0 caiodottori   (501) staff       (20)     5446 2023-05-11 17:39:45.000000 starkinfra-0.8.0/starkinfra/brcodepreview/__brcodepreview.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       37 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/brcodepreview/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.569365 starkinfra-0.8.0/starkinfra/cardmethod/
--rw-r--r--   0 caiodottori   (501) staff       (20)     1297 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/cardmethod/__cardmethod.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       32 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/cardmethod/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.572285 starkinfra-0.8.0/starkinfra/creditholmes/
--rw-r--r--   0 caiodottori   (501) staff       (20)     6542 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/creditholmes/__creditholmes.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       98 2022-12-21 18:15:18.000000 starkinfra-0.8.0/starkinfra/creditholmes/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.575012 starkinfra-0.8.0/starkinfra/creditholmes/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-12-21 18:15:18.000000 starkinfra-0.8.0/starkinfra/creditholmes/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5157 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/creditholmes/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.580477 starkinfra-0.8.0/starkinfra/creditnote/
--rw-r--r--   0 caiodottori   (501) staff       (20)    12304 2023-05-11 17:39:45.000000 starkinfra-0.8.0/starkinfra/creditnote/__creditnote.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      325 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/creditnote/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     3535 2022-06-03 20:41:22.000000 starkinfra-0.8.0/starkinfra/creditnote/__transfer.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.586553 starkinfra-0.8.0/starkinfra/creditnote/invoice/
--rw-r--r--   0 caiodottori   (501) staff       (20)      534 2022-06-03 20:41:22.000000 starkinfra-0.8.0/starkinfra/creditnote/invoice/__description.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      507 2022-06-03 20:41:22.000000 starkinfra-0.8.0/starkinfra/creditnote/invoice/__discount.py
--rw-r--r--   0 caiodottori   (501) staff       (20)        0 2022-06-03 20:41:22.000000 starkinfra-0.8.0/starkinfra/creditnote/invoice/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5403 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/creditnote/invoice/__invoice.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.589079 starkinfra-0.8.0/starkinfra/creditnote/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/creditnote/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5163 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/creditnote/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.593145 starkinfra-0.8.0/starkinfra/creditpreview/
--rw-r--r--   0 caiodottori   (501) staff       (20)     3364 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/creditpreview/__creditnotepreview.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1995 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/creditpreview/__creditpreview.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      102 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/creditpreview/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.595710 starkinfra-0.8.0/starkinfra/creditsigner/
--rw-r--r--   0 caiodottori   (501) staff       (20)      756 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/creditsigner/__creditsigner.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       55 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/creditsigner/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.599671 starkinfra-0.8.0/starkinfra/dynamicbrcode/
--rw-r--r--   0 caiodottori   (501) staff       (20)    15774 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/dynamicbrcode/__dynamicbrcode.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       94 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/dynamicbrcode/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.602628 starkinfra-0.8.0/starkinfra/event/
--rw-r--r--   0 caiodottori   (501) staff       (20)     8846 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/event/__event.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      122 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/event/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.605533 starkinfra-0.8.0/starkinfra/event/attempt/
--rw-r--r--   0 caiodottori   (501) staff       (20)     4981 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/event/attempt/__attempt.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       40 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/event/attempt/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.609033 starkinfra-0.8.0/starkinfra/individualdocument/
--rw-r--r--   0 caiodottori   (501) staff       (20)     7065 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/individualdocument/__individualdocument.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      104 2022-10-25 22:30:46.000000 starkinfra-0.8.0/starkinfra/individualdocument/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.612021 starkinfra-0.8.0/starkinfra/individualdocument/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-10-25 22:30:46.000000 starkinfra-0.8.0/starkinfra/individualdocument/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5257 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/individualdocument/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.614783 starkinfra-0.8.0/starkinfra/individualidentity/
--rw-r--r--   0 caiodottori   (501) staff       (20)     7874 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/individualidentity/__individualidentity.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-10-25 22:30:46.000000 starkinfra-0.8.0/starkinfra/individualidentity/__init__.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.617362 starkinfra-0.8.0/starkinfra/individualidentity/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-10-25 22:30:46.000000 starkinfra-0.8.0/starkinfra/individualidentity/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5249 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/individualidentity/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.619987 starkinfra-0.8.0/starkinfra/issuingbalance/
--rw-r--r--   0 caiodottori   (501) staff       (20)       34 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/issuingbalance/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1603 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/issuingbalance/__issuingbalance.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.623561 starkinfra-0.8.0/starkinfra/issuingcard/
--rw-r--r--   0 caiodottori   (501) staff       (20)      113 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/issuingcard/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    11393 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingcard/__issuingcard.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.626208 starkinfra-0.8.0/starkinfra/issuingcard/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/issuingcard/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5260 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingcard/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.628989 starkinfra-0.8.0/starkinfra/issuingdesign/
--rw-r--r--   0 caiodottori   (501) staff       (20)       51 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingdesign/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     4754 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingdesign/__issuingdesign.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.631352 starkinfra-0.8.0/starkinfra/issuingembossingkit/
--rw-r--r--   0 caiodottori   (501) staff       (20)       52 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingembossingkit/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5269 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingembossingkit/__issuingembossingkit.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.634248 starkinfra-0.8.0/starkinfra/issuingembossingrequest/
--rw-r--r--   0 caiodottori   (501) staff       (20)      109 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingembossingrequest/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     8738 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingembossingrequest/__issuingembossingrequest.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.636706 starkinfra-0.8.0/starkinfra/issuingembossingrequest/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingembossingrequest/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6001 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingembossingrequest/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.639099 starkinfra-0.8.0/starkinfra/issuingholder/
--rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/issuingholder/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     8239 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingholder/__issuingholder.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.641607 starkinfra-0.8.0/starkinfra/issuingholder/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/issuingholder/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5225 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingholder/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.646557 starkinfra-0.8.0/starkinfra/issuinginvoice/
--rw-r--r--   0 caiodottori   (501) staff       (20)      100 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/issuinginvoice/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6663 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuinginvoice/__issuinginvoice.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.649211 starkinfra-0.8.0/starkinfra/issuinginvoice/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/issuinginvoice/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     4939 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuinginvoice/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.651631 starkinfra-0.8.0/starkinfra/issuingproduct/
--rw-r--r--   0 caiodottori   (501) staff       (20)       42 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/issuingproduct/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2825 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/issuingproduct/__issuingproduct.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.654489 starkinfra-0.8.0/starkinfra/issuingpurchase/
--rw-r--r--   0 caiodottori   (501) staff       (20)      104 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/issuingpurchase/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    13027 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingpurchase/__issuingpurchase.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.656742 starkinfra-0.8.0/starkinfra/issuingpurchase/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/issuingpurchase/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5986 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingpurchase/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.658870 starkinfra-0.8.0/starkinfra/issuingrestock/
--rw-r--r--   0 caiodottori   (501) staff       (20)      100 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingrestock/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6412 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingrestock/__issuingrestock.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.660875 starkinfra-0.8.0/starkinfra/issuingrestock/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingrestock/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5242 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingrestock/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.663334 starkinfra-0.8.0/starkinfra/issuingrule/
--rw-r--r--   0 caiodottori   (501) staff       (20)       78 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/issuingrule/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     3925 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingrule/__issuingrule.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.665518 starkinfra-0.8.0/starkinfra/issuingstock/
--rw-r--r--   0 caiodottori   (501) staff       (20)       90 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingstock/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5619 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingstock/__issuingstock.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.668239 starkinfra-0.8.0/starkinfra/issuingstock/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.8.0/starkinfra/issuingstock/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5270 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingstock/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.670992 starkinfra-0.8.0/starkinfra/issuingtransaction/
--rw-r--r--   0 caiodottori   (501) staff       (20)       51 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/issuingtransaction/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5402 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingtransaction/__issuingtransaction.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.675453 starkinfra-0.8.0/starkinfra/issuingwithdrawal/
--rw-r--r--   0 caiodottori   (501) staff       (20)       58 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/issuingwithdrawal/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     6033 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/issuingwithdrawal/__issuingwithdrawal.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.678139 starkinfra-0.8.0/starkinfra/merchantcategory/
--rw-r--r--   0 caiodottori   (501) staff       (20)       38 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/merchantcategory/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1757 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/merchantcategory/__merchantcategory.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.680294 starkinfra-0.8.0/starkinfra/merchantcountry/
--rw-r--r--   0 caiodottori   (501) staff       (20)       37 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/merchantcountry/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1403 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/merchantcountry/__merchantcountry.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.682236 starkinfra-0.8.0/starkinfra/pixbalance/
--rw-r--r--   0 caiodottori   (501) staff       (20)       30 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/pixbalance/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1635 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixbalance/__pixbalance.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.684771 starkinfra-0.8.0/starkinfra/pixchargeback/
--rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixchargeback/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    10153 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixchargeback/__pixchargeback.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.686969 starkinfra-0.8.0/starkinfra/pixchargeback/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixchargeback/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5370 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixchargeback/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.690072 starkinfra-0.8.0/starkinfra/pixclaim/
--rw-r--r--   0 caiodottori   (501) staff       (20)      102 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/pixclaim/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    10003 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixclaim/__pixclaim.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.692452 starkinfra-0.8.0/starkinfra/pixclaim/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/pixclaim/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5518 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixclaim/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.695340 starkinfra-0.8.0/starkinfra/pixdirector/
--rw-r--r--   0 caiodottori   (501) staff       (20)       34 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/pixdirector/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2165 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixdirector/__pixdirector.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.698640 starkinfra-0.8.0/starkinfra/pixdomain/
--rw-r--r--   0 caiodottori   (501) staff       (20)      457 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixdomain/__certificate.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       70 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixdomain/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1382 2022-08-26 19:22:07.000000 starkinfra-0.8.0/starkinfra/pixdomain/__pixdomain.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.701091 starkinfra-0.8.0/starkinfra/pixinfraction/
--rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixinfraction/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     9589 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixinfraction/__pixinfraction.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.703182 starkinfra-0.8.0/starkinfra/pixinfraction/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixinfraction/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5368 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixinfraction/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.705492 starkinfra-0.8.0/starkinfra/pixkey/
--rw-r--r--   0 caiodottori   (501) staff       (20)      108 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/pixkey/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    10238 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixkey/__pixkey.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.707380 starkinfra-0.8.0/starkinfra/pixkey/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/pixkey/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5107 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixkey/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.709868 starkinfra-0.8.0/starkinfra/pixrequest/
--rw-r--r--   0 caiodottori   (501) staff       (20)      113 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/pixrequest/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    13971 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixrequest/__pixrequest.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.711969 starkinfra-0.8.0/starkinfra/pixrequest/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/pixrequest/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5534 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixrequest/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.714771 starkinfra-0.8.0/starkinfra/pixreversal/
--rw-r--r--   0 caiodottori   (501) staff       (20)      114 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/pixreversal/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)    10438 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixreversal/__pixreversal.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.717594 starkinfra-0.8.0/starkinfra/pixreversal/log/
--rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/pixreversal/log/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5138 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixreversal/log/__log.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.720527 starkinfra-0.8.0/starkinfra/pixstatement/
--rw-r--r--   0 caiodottori   (501) staff       (20)       58 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/pixstatement/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     5856 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/pixstatement/__pixstatement.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.721539 starkinfra-0.8.0/starkinfra/staticbrcode/
--rw-r--r--   0 caiodottori   (501) staff       (20)       53 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/staticbrcode/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     7081 2023-05-11 17:39:45.000000 starkinfra-0.8.0/starkinfra/staticbrcode/__staticbrcode.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.733214 starkinfra-0.8.0/starkinfra/utils/
--rw-r--r--   0 caiodottori   (501) staff       (20)       88 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/utils/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      451 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/utils/bacenid.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      360 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/utils/endtoendid.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      151 2022-07-08 00:58:09.000000 starkinfra-0.8.0/starkinfra/utils/parse.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      579 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/utils/relay.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      510 2022-05-01 13:39:31.000000 starkinfra-0.8.0/starkinfra/utils/rest.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      354 2022-05-01 20:57:34.000000 starkinfra-0.8.0/starkinfra/utils/returnid.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.735498 starkinfra-0.8.0/starkinfra/webhook/
--rw-r--r--   0 caiodottori   (501) staff       (20)       56 2022-05-24 01:07:12.000000 starkinfra-0.8.0/starkinfra/webhook/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     4765 2023-04-27 20:24:01.000000 starkinfra-0.8.0/starkinfra/webhook/__webhook.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-05-11 17:41:38.562970 starkinfra-0.8.0/starkinfra.egg-info/
--rw-r--r--   0 caiodottori   (501) staff       (20)    71335 2023-05-11 17:41:38.000000 starkinfra-0.8.0/starkinfra.egg-info/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)     5195 2023-05-11 17:41:38.000000 starkinfra-0.8.0/starkinfra.egg-info/SOURCES.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)        1 2023-05-11 17:41:38.000000 starkinfra-0.8.0/starkinfra.egg-info/dependency_links.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       17 2023-05-11 17:41:38.000000 starkinfra-0.8.0/starkinfra.egg-info/requires.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       17 2023-05-11 17:41:38.000000 starkinfra-0.8.0/starkinfra.egg-info/top_level.txt
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.304013 starkinfra-0.9.0/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-01 13:39:31.000000 starkinfra-0.9.0/LICENSE.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-01 13:39:31.000000 starkinfra-0.9.0/MANIFEST.in
+-rw-r--r--   0 caiodottori   (501) staff       (20)    71335 2023-06-21 14:42:38.303765 starkinfra-0.9.0/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)    70917 2023-05-11 17:39:45.000000 starkinfra-0.9.0/README.md
+-rw-r--r--   0 caiodottori   (501) staff       (20)       38 2023-06-21 14:42:38.304091 starkinfra-0.9.0/setup.cfg
+-rw-r--r--   0 caiodottori   (501) staff       (20)      828 2023-04-27 20:25:01.000000 starkinfra-0.9.0/setup.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.024373 starkinfra-0.9.0/starkinfra/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     3392 2023-06-21 14:39:47.000000 starkinfra-0.9.0/starkinfra/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.033205 starkinfra-0.9.0/starkinfra/brcodepreview/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5446 2023-05-11 17:39:45.000000 starkinfra-0.9.0/starkinfra/brcodepreview/__brcodepreview.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       37 2022-08-26 19:22:07.000000 starkinfra-0.9.0/starkinfra/brcodepreview/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.037924 starkinfra-0.9.0/starkinfra/cardmethod/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1297 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/cardmethod/__cardmethod.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       32 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/cardmethod/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.043880 starkinfra-0.9.0/starkinfra/creditholmes/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6542 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/creditholmes/__creditholmes.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       98 2022-12-21 18:15:18.000000 starkinfra-0.9.0/starkinfra/creditholmes/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.047719 starkinfra-0.9.0/starkinfra/creditholmes/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-12-21 18:15:18.000000 starkinfra-0.9.0/starkinfra/creditholmes/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5157 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/creditholmes/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.057692 starkinfra-0.9.0/starkinfra/creditnote/
+-rw-r--r--   0 caiodottori   (501) staff       (20)    12304 2023-05-11 17:39:45.000000 starkinfra-0.9.0/starkinfra/creditnote/__creditnote.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      325 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/creditnote/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     3535 2022-06-03 20:41:22.000000 starkinfra-0.9.0/starkinfra/creditnote/__transfer.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.067735 starkinfra-0.9.0/starkinfra/creditnote/invoice/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      534 2022-06-03 20:41:22.000000 starkinfra-0.9.0/starkinfra/creditnote/invoice/__description.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      507 2022-06-03 20:41:22.000000 starkinfra-0.9.0/starkinfra/creditnote/invoice/__discount.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)        0 2022-06-03 20:41:22.000000 starkinfra-0.9.0/starkinfra/creditnote/invoice/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5403 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/creditnote/invoice/__invoice.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.072208 starkinfra-0.9.0/starkinfra/creditnote/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/creditnote/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5163 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/creditnote/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.078887 starkinfra-0.9.0/starkinfra/creditpreview/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     3364 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/creditpreview/__creditnotepreview.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1995 2022-08-26 19:22:07.000000 starkinfra-0.9.0/starkinfra/creditpreview/__creditpreview.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      102 2022-08-26 19:22:07.000000 starkinfra-0.9.0/starkinfra/creditpreview/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.081327 starkinfra-0.9.0/starkinfra/creditsigner/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      756 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/creditsigner/__creditsigner.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       55 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/creditsigner/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.085609 starkinfra-0.9.0/starkinfra/dynamicbrcode/
+-rw-r--r--   0 caiodottori   (501) staff       (20)    15774 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/dynamicbrcode/__dynamicbrcode.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       94 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/dynamicbrcode/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.090037 starkinfra-0.9.0/starkinfra/event/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     8846 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/event/__event.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      122 2022-05-01 20:57:34.000000 starkinfra-0.9.0/starkinfra/event/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.092944 starkinfra-0.9.0/starkinfra/event/attempt/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     4981 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/event/attempt/__attempt.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       40 2022-05-01 20:57:34.000000 starkinfra-0.9.0/starkinfra/event/attempt/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.096331 starkinfra-0.9.0/starkinfra/individualdocument/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     7065 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/individualdocument/__individualdocument.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      104 2022-10-25 22:30:46.000000 starkinfra-0.9.0/starkinfra/individualdocument/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.098803 starkinfra-0.9.0/starkinfra/individualdocument/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-10-25 22:30:46.000000 starkinfra-0.9.0/starkinfra/individualdocument/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5257 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/individualdocument/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.104434 starkinfra-0.9.0/starkinfra/individualidentity/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     7874 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/individualidentity/__individualidentity.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-10-25 22:30:46.000000 starkinfra-0.9.0/starkinfra/individualidentity/__init__.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.107451 starkinfra-0.9.0/starkinfra/individualidentity/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-10-25 22:30:46.000000 starkinfra-0.9.0/starkinfra/individualidentity/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5249 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/individualidentity/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.110326 starkinfra-0.9.0/starkinfra/issuingbalance/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       34 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/issuingbalance/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1603 2022-08-26 19:22:07.000000 starkinfra-0.9.0/starkinfra/issuingbalance/__issuingbalance.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.114374 starkinfra-0.9.0/starkinfra/issuingcard/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      113 2022-05-24 01:07:12.000000 starkinfra-0.9.0/starkinfra/issuingcard/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    11393 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingcard/__issuingcard.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.116941 starkinfra-0.9.0/starkinfra/issuingcard/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/issuingcard/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5260 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingcard/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.119342 starkinfra-0.9.0/starkinfra/issuingdesign/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       51 2022-11-23 18:02:54.000000 starkinfra-0.9.0/starkinfra/issuingdesign/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     4754 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingdesign/__issuingdesign.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.121428 starkinfra-0.9.0/starkinfra/issuingembossingkit/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       52 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingembossingkit/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5269 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingembossingkit/__issuingembossingkit.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.124058 starkinfra-0.9.0/starkinfra/issuingembossingrequest/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      109 2022-11-23 18:02:54.000000 starkinfra-0.9.0/starkinfra/issuingembossingrequest/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     8738 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingembossingrequest/__issuingembossingrequest.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.128132 starkinfra-0.9.0/starkinfra/issuingembossingrequest/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.9.0/starkinfra/issuingembossingrequest/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6001 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingembossingrequest/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.131173 starkinfra-0.9.0/starkinfra/issuingholder/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.9.0/starkinfra/issuingholder/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     8239 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingholder/__issuingholder.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.136126 starkinfra-0.9.0/starkinfra/issuingholder/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/issuingholder/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5225 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingholder/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.139341 starkinfra-0.9.0/starkinfra/issuinginvoice/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      100 2022-05-01 20:57:34.000000 starkinfra-0.9.0/starkinfra/issuinginvoice/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6663 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuinginvoice/__issuinginvoice.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.143873 starkinfra-0.9.0/starkinfra/issuinginvoice/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.9.0/starkinfra/issuinginvoice/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     4939 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuinginvoice/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.146673 starkinfra-0.9.0/starkinfra/issuingproduct/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       42 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/issuingproduct/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2825 2022-08-26 19:22:07.000000 starkinfra-0.9.0/starkinfra/issuingproduct/__issuingproduct.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.151978 starkinfra-0.9.0/starkinfra/issuingpurchase/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      104 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/issuingpurchase/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    13228 2023-06-20 20:14:49.000000 starkinfra-0.9.0/starkinfra/issuingpurchase/__issuingpurchase.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.157440 starkinfra-0.9.0/starkinfra/issuingpurchase/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/issuingpurchase/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5986 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingpurchase/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.161545 starkinfra-0.9.0/starkinfra/issuingrestock/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      100 2022-11-23 18:02:54.000000 starkinfra-0.9.0/starkinfra/issuingrestock/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6412 2022-11-23 18:02:54.000000 starkinfra-0.9.0/starkinfra/issuingrestock/__issuingrestock.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.165590 starkinfra-0.9.0/starkinfra/issuingrestock/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.9.0/starkinfra/issuingrestock/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5242 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingrestock/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.170440 starkinfra-0.9.0/starkinfra/issuingrule/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       78 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/issuingrule/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     3925 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingrule/__issuingrule.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.181498 starkinfra-0.9.0/starkinfra/issuingstock/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       90 2022-11-23 18:02:54.000000 starkinfra-0.9.0/starkinfra/issuingstock/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5619 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingstock/__issuingstock.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.185403 starkinfra-0.9.0/starkinfra/issuingstock/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-11-23 18:02:54.000000 starkinfra-0.9.0/starkinfra/issuingstock/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5270 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingstock/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.189032 starkinfra-0.9.0/starkinfra/issuingtransaction/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       51 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/issuingtransaction/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5402 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingtransaction/__issuingtransaction.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.192690 starkinfra-0.9.0/starkinfra/issuingwithdrawal/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       58 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/issuingwithdrawal/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     6033 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/issuingwithdrawal/__issuingwithdrawal.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.196192 starkinfra-0.9.0/starkinfra/merchantcategory/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       38 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/merchantcategory/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1757 2022-08-26 19:22:07.000000 starkinfra-0.9.0/starkinfra/merchantcategory/__merchantcategory.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.200860 starkinfra-0.9.0/starkinfra/merchantcountry/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       37 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/merchantcountry/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1403 2022-08-26 19:22:07.000000 starkinfra-0.9.0/starkinfra/merchantcountry/__merchantcountry.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.203505 starkinfra-0.9.0/starkinfra/pixbalance/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       30 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/pixbalance/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1635 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixbalance/__pixbalance.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.207715 starkinfra-0.9.0/starkinfra/pixchargeback/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.9.0/starkinfra/pixchargeback/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    10153 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixchargeback/__pixchargeback.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.212007 starkinfra-0.9.0/starkinfra/pixchargeback/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.9.0/starkinfra/pixchargeback/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5370 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixchargeback/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.222521 starkinfra-0.9.0/starkinfra/pixclaim/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      102 2022-05-01 20:57:34.000000 starkinfra-0.9.0/starkinfra/pixclaim/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    10003 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixclaim/__pixclaim.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.226351 starkinfra-0.9.0/starkinfra/pixclaim/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 20:57:34.000000 starkinfra-0.9.0/starkinfra/pixclaim/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5518 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixclaim/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.229562 starkinfra-0.9.0/starkinfra/pixdirector/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       34 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/pixdirector/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2165 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixdirector/__pixdirector.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.234433 starkinfra-0.9.0/starkinfra/pixdomain/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      457 2022-05-24 01:07:12.000000 starkinfra-0.9.0/starkinfra/pixdomain/__certificate.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       70 2022-05-24 01:07:12.000000 starkinfra-0.9.0/starkinfra/pixdomain/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1382 2022-08-26 19:22:07.000000 starkinfra-0.9.0/starkinfra/pixdomain/__pixdomain.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.237326 starkinfra-0.9.0/starkinfra/pixinfraction/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      115 2022-05-24 01:07:12.000000 starkinfra-0.9.0/starkinfra/pixinfraction/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     9589 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixinfraction/__pixinfraction.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.240747 starkinfra-0.9.0/starkinfra/pixinfraction/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-24 01:07:12.000000 starkinfra-0.9.0/starkinfra/pixinfraction/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5368 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixinfraction/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.243570 starkinfra-0.9.0/starkinfra/pixkey/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      108 2022-05-24 01:07:12.000000 starkinfra-0.9.0/starkinfra/pixkey/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    10238 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixkey/__pixkey.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.248237 starkinfra-0.9.0/starkinfra/pixkey/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 20:57:34.000000 starkinfra-0.9.0/starkinfra/pixkey/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5107 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixkey/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.252907 starkinfra-0.9.0/starkinfra/pixrequest/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      113 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/pixrequest/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    13971 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixrequest/__pixrequest.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.256424 starkinfra-0.9.0/starkinfra/pixrequest/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/pixrequest/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5534 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixrequest/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.259363 starkinfra-0.9.0/starkinfra/pixreversal/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      114 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/pixreversal/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)    10438 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixreversal/__pixreversal.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.262955 starkinfra-0.9.0/starkinfra/pixreversal/log/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       36 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/pixreversal/log/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5138 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixreversal/log/__log.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.268109 starkinfra-0.9.0/starkinfra/pixstatement/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       58 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/pixstatement/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5856 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/pixstatement/__pixstatement.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.272662 starkinfra-0.9.0/starkinfra/staticbrcode/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       53 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/staticbrcode/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     7081 2023-05-11 17:39:45.000000 starkinfra-0.9.0/starkinfra/staticbrcode/__staticbrcode.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.286949 starkinfra-0.9.0/starkinfra/utils/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       88 2022-05-01 20:57:34.000000 starkinfra-0.9.0/starkinfra/utils/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      451 2022-05-01 20:57:34.000000 starkinfra-0.9.0/starkinfra/utils/bacenid.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      360 2022-05-01 20:57:34.000000 starkinfra-0.9.0/starkinfra/utils/endtoendid.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      151 2022-07-08 00:58:09.000000 starkinfra-0.9.0/starkinfra/utils/parse.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      579 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/utils/relay.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      510 2022-05-01 13:39:31.000000 starkinfra-0.9.0/starkinfra/utils/rest.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      354 2022-05-01 20:57:34.000000 starkinfra-0.9.0/starkinfra/utils/returnid.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.303259 starkinfra-0.9.0/starkinfra/webhook/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       56 2022-05-24 01:07:12.000000 starkinfra-0.9.0/starkinfra/webhook/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     4765 2023-04-27 20:24:01.000000 starkinfra-0.9.0/starkinfra/webhook/__webhook.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2023-06-21 14:42:38.027753 starkinfra-0.9.0/starkinfra.egg-info/
+-rw-r--r--   0 caiodottori   (501) staff       (20)    71335 2023-06-21 14:42:37.000000 starkinfra-0.9.0/starkinfra.egg-info/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)     5195 2023-06-21 14:42:38.000000 starkinfra-0.9.0/starkinfra.egg-info/SOURCES.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)        1 2023-06-21 14:42:37.000000 starkinfra-0.9.0/starkinfra.egg-info/dependency_links.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       17 2023-06-21 14:42:37.000000 starkinfra-0.9.0/starkinfra.egg-info/requires.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       17 2023-06-21 14:42:37.000000 starkinfra-0.9.0/starkinfra.egg-info/top_level.txt
```

### Comparing `starkinfra-0.8.0/LICENSE.txt` & `starkinfra-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/PKG-INFO` & `starkinfra-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starkinfra
-Version: 0.8.0
+Version: 0.9.0
 Summary: SDK to facilitate Python integrations with Stark Infra
 Home-page: https://github.com/starkinfra/sdk-python
 Author: Stark Infra
 Author-email: developers@starkbank.com
 License: MIT License
 Keywords: stark infra,starkinfra,sdk,open banking,openbanking,banking,open,stark
 Platform: UNKNOWN
```

### Comparing `starkinfra-0.8.0/README.md` & `starkinfra-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/setup.py` & `starkinfra-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/__init__.py` & `starkinfra-0.9.0/starkinfra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version = "0.8.0"
+version = "0.9.0"
 language = "en-US"
 timeout = 15
 user = None
 
 from starkcore import Project, Organization, key, error
 
 from . import event
```

### Comparing `starkinfra-0.8.0/starkinfra/brcodepreview/__brcodepreview.py` & `starkinfra-0.9.0/starkinfra/brcodepreview/__brcodepreview.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/cardmethod/__cardmethod.py` & `starkinfra-0.9.0/starkinfra/cardmethod/__cardmethod.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/creditholmes/__creditholmes.py` & `starkinfra-0.9.0/starkinfra/creditholmes/__creditholmes.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/creditholmes/log/__log.py` & `starkinfra-0.9.0/starkinfra/creditholmes/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/creditnote/__creditnote.py` & `starkinfra-0.9.0/starkinfra/creditnote/__creditnote.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/creditnote/__transfer.py` & `starkinfra-0.9.0/starkinfra/creditnote/__transfer.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/creditnote/invoice/__description.py` & `starkinfra-0.9.0/starkinfra/creditnote/invoice/__description.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/creditnote/invoice/__invoice.py` & `starkinfra-0.9.0/starkinfra/creditnote/invoice/__invoice.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/creditnote/log/__log.py` & `starkinfra-0.9.0/starkinfra/creditnote/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/creditpreview/__creditnotepreview.py` & `starkinfra-0.9.0/starkinfra/creditpreview/__creditnotepreview.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/creditpreview/__creditpreview.py` & `starkinfra-0.9.0/starkinfra/creditpreview/__creditpreview.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/creditsigner/__creditsigner.py` & `starkinfra-0.9.0/starkinfra/creditsigner/__creditsigner.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/dynamicbrcode/__dynamicbrcode.py` & `starkinfra-0.9.0/starkinfra/dynamicbrcode/__dynamicbrcode.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/event/__event.py` & `starkinfra-0.9.0/starkinfra/event/__event.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/event/attempt/__attempt.py` & `starkinfra-0.9.0/starkinfra/event/attempt/__attempt.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/individualdocument/__individualdocument.py` & `starkinfra-0.9.0/starkinfra/individualdocument/__individualdocument.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/individualdocument/log/__log.py` & `starkinfra-0.9.0/starkinfra/individualdocument/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/individualidentity/__individualidentity.py` & `starkinfra-0.9.0/starkinfra/individualidentity/__individualidentity.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/individualidentity/log/__log.py` & `starkinfra-0.9.0/starkinfra/individualidentity/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingbalance/__issuingbalance.py` & `starkinfra-0.9.0/starkinfra/issuingbalance/__issuingbalance.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingcard/__issuingcard.py` & `starkinfra-0.9.0/starkinfra/issuingcard/__issuingcard.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingcard/log/__log.py` & `starkinfra-0.9.0/starkinfra/issuingcard/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingdesign/__issuingdesign.py` & `starkinfra-0.9.0/starkinfra/issuingdesign/__issuingdesign.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingembossingkit/__issuingembossingkit.py` & `starkinfra-0.9.0/starkinfra/issuingembossingkit/__issuingembossingkit.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingembossingrequest/__issuingembossingrequest.py` & `starkinfra-0.9.0/starkinfra/issuingembossingrequest/__issuingembossingrequest.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingembossingrequest/log/__log.py` & `starkinfra-0.9.0/starkinfra/issuingembossingrequest/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingholder/__issuingholder.py` & `starkinfra-0.9.0/starkinfra/issuingholder/__issuingholder.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingholder/log/__log.py` & `starkinfra-0.9.0/starkinfra/issuingholder/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuinginvoice/__issuinginvoice.py` & `starkinfra-0.9.0/starkinfra/issuinginvoice/__issuinginvoice.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuinginvoice/log/__log.py` & `starkinfra-0.9.0/starkinfra/issuinginvoice/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingproduct/__issuingproduct.py` & `starkinfra-0.9.0/starkinfra/issuingproduct/__issuingproduct.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingpurchase/__issuingpurchase.py` & `starkinfra-0.9.0/starkinfra/issuingpurchase/__issuingpurchase.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     - merchant_currency_code [string]: merchant currency code. ex: "USD"
     - merchant_currency_symbol [string]: merchant currency symbol. ex: "$"
     - merchant_category_code [string]: merchant category code. ex: "fastFoodRestaurants"
     - merchant_country_code [string]: merchant country code. ex: "USA"
     - acquirer_id [string]: acquirer ID. ex: "5656565656565656"
     - merchant_id [string]: merchant ID. ex: "5656565656565656"
     - merchant_name [string]: merchant name. ex: "Google Cloud Platform"
+    - metadata [dictionary]: dictionary object used to store additional information about the IssuingPurchase object. ex: { authorizationId: 'OjZAqj' }.
     - merchant_fee [integer]: fee charged by the merchant to cover specific costs, such as ATM withdrawal logistics, etc. ex: 200 (= R$ 2.00)
     - wallet_id [string]: virtual wallet ID. ex: "5656565656565656"
     - method_code [string]: method code. Options: "chip", "token", "server", "manual", "magstripe" or "contactless"
     - score [float]: internal score calculated for the authenticity of the purchase. None in case of insufficient data. ex: 7.6
     - end_to_end_id [string]: Unique id used to identify the transaction through all of its life cycle, even before the purchase is denied or approved and gets its usual id. ex: "679cd385-642b-49d0-96b7-89491e1249a5"
     - tags [list of strings]: list of strings for tagging returned by the sub-issuer during the authorization. ex: ["travel", "food"]
     - zip_code [string]: zip code of the merchant location. ex: "02101234"
@@ -47,15 +48,15 @@
     - holder_tags [list of strings]: tags of the IssuingHolder responsible for this purchase. ex: ["technology", "john snow"]
     """
 
     def __init__(self, id=None, holder_name=None, product_id=None, card_id=None, card_ending=None, purpose=None,
                 amount=None, tax=None, issuer_amount=None, issuer_currency_code=None, issuer_currency_symbol=None,
                 merchant_amount=None, merchant_currency_code=None, merchant_currency_symbol=None,
                 merchant_category_code=None, merchant_country_code=None, acquirer_id=None, merchant_id=None,
-                merchant_name=None, merchant_fee=None, wallet_id=None, method_code=None, score=None, end_to_end_id=None,
+                merchant_name=None, metadata=None, merchant_fee=None, wallet_id=None, method_code=None, score=None, end_to_end_id=None,
                 tags=None, zip_code=None, issuing_transaction_ids=None, status=None, updated=None, created=None,
                 is_partial_allowed=None, card_tags=None, holder_tags=None):
         Resource.__init__(self, id=id)
 
         self.holder_name = holder_name
         self.product_id = product_id
         self.card_id = card_id
@@ -70,14 +71,15 @@
         self.merchant_currency_code = merchant_currency_code
         self.merchant_currency_symbol = merchant_currency_symbol
         self.merchant_category_code = merchant_category_code
         self.merchant_country_code = merchant_country_code
         self.acquirer_id = acquirer_id
         self.merchant_id = merchant_id
         self.merchant_name = merchant_name
+        self.metadata = metadata
         self.merchant_fee = merchant_fee
         self.wallet_id = wallet_id
         self.method_code = method_code
         self.score = score
         self.end_to_end_id = end_to_end_id
         self.tags = tags
         self.zip_code = zip_code
```

### Comparing `starkinfra-0.8.0/starkinfra/issuingpurchase/log/__log.py` & `starkinfra-0.9.0/starkinfra/issuingpurchase/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingrestock/__issuingrestock.py` & `starkinfra-0.9.0/starkinfra/issuingrestock/__issuingrestock.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingrestock/log/__log.py` & `starkinfra-0.9.0/starkinfra/issuingrestock/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingrule/__issuingrule.py` & `starkinfra-0.9.0/starkinfra/issuingrule/__issuingrule.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingstock/__issuingstock.py` & `starkinfra-0.9.0/starkinfra/issuingstock/__issuingstock.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingstock/log/__log.py` & `starkinfra-0.9.0/starkinfra/issuingstock/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingtransaction/__issuingtransaction.py` & `starkinfra-0.9.0/starkinfra/issuingtransaction/__issuingtransaction.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/issuingwithdrawal/__issuingwithdrawal.py` & `starkinfra-0.9.0/starkinfra/issuingwithdrawal/__issuingwithdrawal.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/merchantcategory/__merchantcategory.py` & `starkinfra-0.9.0/starkinfra/merchantcategory/__merchantcategory.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/merchantcountry/__merchantcountry.py` & `starkinfra-0.9.0/starkinfra/merchantcountry/__merchantcountry.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixbalance/__pixbalance.py` & `starkinfra-0.9.0/starkinfra/pixbalance/__pixbalance.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixchargeback/__pixchargeback.py` & `starkinfra-0.9.0/starkinfra/pixchargeback/__pixchargeback.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixchargeback/log/__log.py` & `starkinfra-0.9.0/starkinfra/pixchargeback/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixclaim/__pixclaim.py` & `starkinfra-0.9.0/starkinfra/pixclaim/__pixclaim.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixclaim/log/__log.py` & `starkinfra-0.9.0/starkinfra/pixclaim/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixdirector/__pixdirector.py` & `starkinfra-0.9.0/starkinfra/pixdirector/__pixdirector.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixdomain/__pixdomain.py` & `starkinfra-0.9.0/starkinfra/pixdomain/__pixdomain.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixinfraction/__pixinfraction.py` & `starkinfra-0.9.0/starkinfra/pixinfraction/__pixinfraction.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixinfraction/log/__log.py` & `starkinfra-0.9.0/starkinfra/pixinfraction/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixkey/__pixkey.py` & `starkinfra-0.9.0/starkinfra/pixkey/__pixkey.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixkey/log/__log.py` & `starkinfra-0.9.0/starkinfra/pixkey/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixrequest/__pixrequest.py` & `starkinfra-0.9.0/starkinfra/pixrequest/__pixrequest.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixrequest/log/__log.py` & `starkinfra-0.9.0/starkinfra/pixrequest/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixreversal/__pixreversal.py` & `starkinfra-0.9.0/starkinfra/pixreversal/__pixreversal.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixreversal/log/__log.py` & `starkinfra-0.9.0/starkinfra/pixreversal/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/pixstatement/__pixstatement.py` & `starkinfra-0.9.0/starkinfra/pixstatement/__pixstatement.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/staticbrcode/__staticbrcode.py` & `starkinfra-0.9.0/starkinfra/staticbrcode/__staticbrcode.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/utils/relay.py` & `starkinfra-0.9.0/starkinfra/utils/relay.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra/webhook/__webhook.py` & `starkinfra-0.9.0/starkinfra/webhook/__webhook.py`

 * *Files identical despite different names*

### Comparing `starkinfra-0.8.0/starkinfra.egg-info/PKG-INFO` & `starkinfra-0.9.0/starkinfra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starkinfra
-Version: 0.8.0
+Version: 0.9.0
 Summary: SDK to facilitate Python integrations with Stark Infra
 Home-page: https://github.com/starkinfra/sdk-python
 Author: Stark Infra
 Author-email: developers@starkbank.com
 License: MIT License
 Keywords: stark infra,starkinfra,sdk,open banking,openbanking,banking,open,stark
 Platform: UNKNOWN
```

### Comparing `starkinfra-0.8.0/starkinfra.egg-info/SOURCES.txt` & `starkinfra-0.9.0/starkinfra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

